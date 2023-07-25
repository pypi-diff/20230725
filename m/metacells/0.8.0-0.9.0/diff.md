# Comparing `tmp/metacells-0.8.0.tar.gz` & `tmp/metacells-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/metacells-0.8.0.tar", last modified: Mon Apr  4 06:01:47 2022, max compression
+gzip compressed data, was "metacells-0.9.0.tar", last modified: Tue Jul 25 17:41:47 2023, max compression
```

## Comparing `metacells-0.8.0.tar` & `metacells-0.9.0.tar`

### file list

```diff
@@ -1,119 +1,121 @@
-drwxrwx---   0 obk       (2045) dialout     (18)        0 2022-04-04 06:01:47.000000 metacells-0.8.0/
--rw-rw----   0 obk       (2045) dialout     (18)      886 2022-03-04 15:12:22.000000 metacells-0.8.0/HISTORY.rst
--rw-rw----   0 obk       (2045) dialout     (18)     1123 2021-11-12 15:09:48.000000 metacells-0.8.0/LICENSE.rst
--rw-rw----   0 obk       (2045) dialout     (18)      422 2021-11-12 17:44:22.000000 metacells-0.8.0/MANIFEST.in
--rw-rw----   0 obk       (2045) dialout     (18)     9187 2022-04-04 06:01:47.000000 metacells-0.8.0/PKG-INFO
--rw-rw----   0 obk       (2045) dialout     (18)     7389 2022-04-03 11:43:28.000000 metacells-0.8.0/README.rst
-drwxrwx---   0 obk       (2045) dialout     (18)        0 2022-04-04 06:01:47.000000 metacells-0.8.0/metacells/
--rw-rw----   0 obk       (2045) dialout     (18)      415 2022-04-03 11:43:28.000000 metacells-0.8.0/metacells/__init__.py
--rw-rw----   0 obk       (2045) dialout     (18)    10056 2022-01-26 11:03:38.000000 metacells-0.8.0/metacells/auroc.cpp
--rw-rw----   0 obk       (2045) dialout     (18)     1719 2021-12-30 15:42:34.000000 metacells-0.8.0/metacells/check_avx2.py
--rw-rw----   0 obk       (2045) dialout     (18)    12940 2022-01-26 11:03:38.000000 metacells-0.8.0/metacells/choose_seeds.cpp
--rw-rw----   0 obk       (2045) dialout     (18)    26798 2022-01-26 11:03:38.000000 metacells-0.8.0/metacells/correlate.cpp
--rw-rw----   0 obk       (2045) dialout     (18)    11378 2022-01-26 11:03:38.000000 metacells-0.8.0/metacells/cover.cpp
--rw-rw----   0 obk       (2045) dialout     (18)     8502 2022-01-26 11:03:38.000000 metacells-0.8.0/metacells/downsample.cpp
--rw-rw----   0 obk       (2045) dialout     (18)     2280 2022-01-26 11:03:38.000000 metacells-0.8.0/metacells/extensions.cpp
--rw-rw----   0 obk       (2045) dialout     (18)    18713 2022-01-26 11:04:25.000000 metacells-0.8.0/metacells/extensions.h
--rw-rw----   0 obk       (2045) dialout     (18)    10198 2022-01-26 11:03:38.000000 metacells-0.8.0/metacells/folds.cpp
--rw-rw----   0 obk       (2045) dialout     (18)     6114 2022-01-26 11:03:38.000000 metacells-0.8.0/metacells/logistics.cpp
--rw-rw----   0 obk       (2045) dialout     (18)    50092 2022-03-20 12:47:01.000000 metacells-0.8.0/metacells/parameters.py
--rw-rw----   0 obk       (2045) dialout     (18)    49127 2022-01-26 11:03:38.000000 metacells-0.8.0/metacells/partitions.cpp
-drwxrwx---   0 obk       (2045) dialout     (18)        0 2022-04-04 06:01:47.000000 metacells-0.8.0/metacells/pipeline/
--rw-rw----   0 obk       (2045) dialout     (18)      760 2021-12-23 12:38:43.000000 metacells-0.8.0/metacells/pipeline/__init__.py
--rw-rw----   0 obk       (2045) dialout     (18)    10462 2021-12-20 07:34:45.000000 metacells-0.8.0/metacells/pipeline/clean.py
--rw-rw----   0 obk       (2045) dialout     (18)     6489 2021-11-12 18:02:55.000000 metacells-0.8.0/metacells/pipeline/collect.py
--rw-rw----   0 obk       (2045) dialout     (18)    10094 2021-11-12 18:10:32.000000 metacells-0.8.0/metacells/pipeline/consistency.py
--rw-rw----   0 obk       (2045) dialout     (18)    20506 2022-03-14 11:57:21.000000 metacells-0.8.0/metacells/pipeline/direct.py
--rw-rw----   0 obk       (2045) dialout     (18)    99094 2022-03-29 13:21:30.000000 metacells-0.8.0/metacells/pipeline/divide_and_conquer.py
--rw-rw----   0 obk       (2045) dialout     (18)     6199 2022-03-13 14:53:37.000000 metacells-0.8.0/metacells/pipeline/feature.py
--rw-rw----   0 obk       (2045) dialout     (18)     5970 2022-03-02 12:42:30.000000 metacells-0.8.0/metacells/pipeline/mcview.py
--rw-rw----   0 obk       (2045) dialout     (18)    79937 2022-03-31 15:02:50.000000 metacells-0.8.0/metacells/pipeline/projection.py
--rw-rw----   0 obk       (2045) dialout     (18)     6776 2021-11-12 19:41:57.000000 metacells-0.8.0/metacells/pipeline/related_genes.py
--rw-rw----   0 obk       (2045) dialout     (18)    10159 2022-04-03 09:56:54.000000 metacells-0.8.0/metacells/pipeline/umap.py
--rw-rw----   0 obk       (2045) dialout     (18)     6153 2022-01-26 11:03:38.000000 metacells-0.8.0/metacells/prune_per.cpp
--rw-rw----   0 obk       (2045) dialout     (18)        0 2021-12-30 15:42:34.000000 metacells-0.8.0/metacells/py.typed
--rw-rw----   0 obk       (2045) dialout     (18)     4172 2022-01-26 11:03:38.000000 metacells-0.8.0/metacells/rank.cpp
--rw-rw----   0 obk       (2045) dialout     (18)     8999 2022-01-26 11:03:38.000000 metacells-0.8.0/metacells/relayout.cpp
-drwxrwx---   0 obk       (2045) dialout     (18)        0 2022-04-04 06:01:47.000000 metacells-0.8.0/metacells/scripts/
--rw-rw----   0 obk       (2045) dialout     (18)       55 2021-11-12 17:54:50.000000 metacells-0.8.0/metacells/scripts/__init__.py
--rw-rw----   0 obk       (2045) dialout     (18)     9349 2021-11-12 18:33:39.000000 metacells-0.8.0/metacells/scripts/timing.py
--rw-rw----   0 obk       (2045) dialout     (18)       99 2022-04-04 06:01:47.000000 metacells-0.8.0/metacells/should_check_avx2.py
--rw-rw----   0 obk       (2045) dialout     (18)     5554 2022-01-26 11:03:38.000000 metacells-0.8.0/metacells/shuffle.cpp
-drwxrwx---   0 obk       (2045) dialout     (18)        0 2022-04-04 06:01:47.000000 metacells-0.8.0/metacells/tools/
--rw-rw----   0 obk       (2045) dialout     (18)     1147 2021-11-15 15:12:52.000000 metacells-0.8.0/metacells/tools/__init__.py
--rw-rw----   0 obk       (2045) dialout     (18)     6922 2021-11-12 19:41:57.000000 metacells-0.8.0/metacells/tools/apply.py
--rw-rw----   0 obk       (2045) dialout     (18)    31578 2022-01-26 10:56:49.000000 metacells-0.8.0/metacells/tools/candidates.py
--rw-rw----   0 obk       (2045) dialout     (18)     6756 2021-12-13 08:55:14.000000 metacells-0.8.0/metacells/tools/convey.py
--rw-rw----   0 obk       (2045) dialout     (18)    18030 2022-03-27 13:54:04.000000 metacells-0.8.0/metacells/tools/deviants.py
--rw-rw----   0 obk       (2045) dialout     (18)    10509 2021-12-30 17:24:52.000000 metacells-0.8.0/metacells/tools/dissolve.py
--rw-rw----   0 obk       (2045) dialout     (18)     9468 2021-12-30 08:14:31.000000 metacells-0.8.0/metacells/tools/distinct.py
--rw-rw----   0 obk       (2045) dialout     (18)     4182 2022-03-13 15:09:29.000000 metacells-0.8.0/metacells/tools/downsample.py
--rw-rw----   0 obk       (2045) dialout     (18)     4153 2021-11-12 18:02:42.000000 metacells-0.8.0/metacells/tools/filter.py
--rw-rw----   0 obk       (2045) dialout     (18)     5941 2021-11-12 19:41:57.000000 metacells-0.8.0/metacells/tools/group.py
--rw-rw----   0 obk       (2045) dialout     (18)    16422 2022-01-17 16:04:18.000000 metacells-0.8.0/metacells/tools/high.py
--rw-rw----   0 obk       (2045) dialout     (18)    15729 2022-01-26 10:57:07.000000 metacells-0.8.0/metacells/tools/knn_graph.py
--rw-rw----   0 obk       (2045) dialout     (18)     5920 2021-11-12 18:02:04.000000 metacells-0.8.0/metacells/tools/layout.py
--rw-rw----   0 obk       (2045) dialout     (18)     4028 2022-01-16 13:48:15.000000 metacells-0.8.0/metacells/tools/mask.py
--rw-rw----   0 obk       (2045) dialout     (18)     1952 2021-11-12 18:01:57.000000 metacells-0.8.0/metacells/tools/named.py
--rw-rw----   0 obk       (2045) dialout     (18)    10404 2022-01-26 10:57:19.000000 metacells-0.8.0/metacells/tools/noisy_lonely.py
--rw-rw----   0 obk       (2045) dialout     (18)    32696 2022-03-28 17:19:45.000000 metacells-0.8.0/metacells/tools/project.py
--rw-rw----   0 obk       (2045) dialout     (18)     5395 2021-11-12 18:01:54.000000 metacells-0.8.0/metacells/tools/properly_sampled.py
--rw-rw----   0 obk       (2045) dialout     (18)    43523 2022-03-20 13:48:07.000000 metacells-0.8.0/metacells/tools/quality.py
--rw-rw----   0 obk       (2045) dialout     (18)    29750 2022-03-21 13:40:49.000000 metacells-0.8.0/metacells/tools/rare.py
--rw-rw----   0 obk       (2045) dialout     (18)     8343 2022-02-24 09:09:56.000000 metacells-0.8.0/metacells/tools/similarity.py
--rw-rw----   0 obk       (2045) dialout     (18)     4042 2022-01-26 11:03:38.000000 metacells-0.8.0/metacells/top_per.cpp
-drwxrwx---   0 obk       (2045) dialout     (18)        0 2022-04-04 06:01:47.000000 metacells-0.8.0/metacells/utilities/
--rw-rw----   0 obk       (2045) dialout     (18)      423 2022-03-28 17:08:32.000000 metacells-0.8.0/metacells/utilities/__init__.py
--rw-rw----   0 obk       (2045) dialout     (18)    35864 2022-02-04 15:49:39.000000 metacells-0.8.0/metacells/utilities/annotation.py
--rw-rw----   0 obk       (2045) dialout     (18)    85403 2022-03-07 09:05:48.000000 metacells-0.8.0/metacells/utilities/computation.py
--rw-rw----   0 obk       (2045) dialout     (18)     1925 2021-11-12 19:08:40.000000 metacells-0.8.0/metacells/utilities/documentation.py
--rw-rw----   0 obk       (2045) dialout     (18)    25984 2022-03-28 17:06:01.000000 metacells-0.8.0/metacells/utilities/logging.py
--rw-rw----   0 obk       (2045) dialout     (18)     9666 2022-03-29 09:39:58.000000 metacells-0.8.0/metacells/utilities/parallel.py
--rw-rw----   0 obk       (2045) dialout     (18)     5265 2022-03-29 16:13:53.000000 metacells-0.8.0/metacells/utilities/progress.py
--rw-rw----   0 obk       (2045) dialout     (18)        0 2021-11-12 17:21:33.000000 metacells-0.8.0/metacells/utilities/py.typed
--rw-rw----   0 obk       (2045) dialout     (18)    15049 2022-03-07 17:36:08.000000 metacells-0.8.0/metacells/utilities/timing.py
--rw-rw----   0 obk       (2045) dialout     (18)    31706 2022-03-02 10:52:36.000000 metacells-0.8.0/metacells/utilities/typing.py
-drwxrwx---   0 obk       (2045) dialout     (18)        0 2022-04-04 06:01:47.000000 metacells-0.8.0/metacells.egg-info/
--rw-rw----   0 obk       (2045) dialout     (18)     9187 2022-04-04 06:01:47.000000 metacells-0.8.0/metacells.egg-info/PKG-INFO
--rw-rw----   0 obk       (2045) dialout     (18)     3045 2022-04-04 06:01:47.000000 metacells-0.8.0/metacells.egg-info/SOURCES.txt
--rw-rw----   0 obk       (2045) dialout     (18)        1 2022-04-04 06:01:47.000000 metacells-0.8.0/metacells.egg-info/dependency_links.txt
--rw-rw----   0 obk       (2045) dialout     (18)       68 2022-04-04 06:01:47.000000 metacells-0.8.0/metacells.egg-info/entry_points.txt
--rw-rw----   0 obk       (2045) dialout     (18)      222 2022-04-04 06:01:47.000000 metacells-0.8.0/metacells.egg-info/requires.txt
--rw-rw----   0 obk       (2045) dialout     (18)       10 2022-04-04 06:01:47.000000 metacells-0.8.0/metacells.egg-info/top_level.txt
-drwxrwx---   0 obk       (2045) dialout     (18)        0 2022-04-04 06:01:47.000000 metacells-0.8.0/pybind11/
-drwxrwx---   0 obk       (2045) dialout     (18)        0 2022-04-04 06:01:47.000000 metacells-0.8.0/pybind11/include/
-drwxrwx---   0 obk       (2045) dialout     (18)        0 2022-04-04 06:01:47.000000 metacells-0.8.0/pybind11/include/pybind11/
--rw-rw----   0 obk       (2045) dialout     (18)    20302 2021-11-12 17:22:18.000000 metacells-0.8.0/pybind11/include/pybind11/attr.h
--rw-rw----   0 obk       (2045) dialout     (18)     4962 2021-11-12 17:22:18.000000 metacells-0.8.0/pybind11/include/pybind11/buffer_info.h
--rw-rw----   0 obk       (2045) dialout     (18)    93351 2021-11-12 17:22:18.000000 metacells-0.8.0/pybind11/include/pybind11/cast.h
--rw-rw----   0 obk       (2045) dialout     (18)     7737 2021-11-12 17:22:18.000000 metacells-0.8.0/pybind11/include/pybind11/chrono.h
--rw-rw----   0 obk       (2045) dialout     (18)      120 2021-11-12 17:22:18.000000 metacells-0.8.0/pybind11/include/pybind11/common.h
--rw-rw----   0 obk       (2045) dialout     (18)     2037 2021-11-12 17:22:18.000000 metacells-0.8.0/pybind11/include/pybind11/complex.h
-drwxrwx---   0 obk       (2045) dialout     (18)        0 2022-04-04 06:01:47.000000 metacells-0.8.0/pybind11/include/pybind11/detail/
--rw-rw----   0 obk       (2045) dialout     (18)    26382 2021-11-12 17:22:18.000000 metacells-0.8.0/pybind11/include/pybind11/detail/class.h
--rw-rw----   0 obk       (2045) dialout     (18)    38908 2021-11-12 17:22:18.000000 metacells-0.8.0/pybind11/include/pybind11/detail/common.h
--rw-rw----   0 obk       (2045) dialout     (18)     3602 2021-11-12 17:22:18.000000 metacells-0.8.0/pybind11/include/pybind11/detail/descr.h
--rw-rw----   0 obk       (2045) dialout     (18)    16376 2021-11-12 17:22:18.000000 metacells-0.8.0/pybind11/include/pybind11/detail/init.h
--rw-rw----   0 obk       (2045) dialout     (18)    16064 2021-11-12 17:22:18.000000 metacells-0.8.0/pybind11/include/pybind11/detail/internals.h
--rw-rw----   0 obk       (2045) dialout     (18)     1486 2021-11-12 17:22:18.000000 metacells-0.8.0/pybind11/include/pybind11/detail/typeid.h
--rw-rw----   0 obk       (2045) dialout     (18)    29079 2021-11-12 17:22:18.000000 metacells-0.8.0/pybind11/include/pybind11/eigen.h
--rw-rw----   0 obk       (2045) dialout     (18)     7955 2021-11-12 17:22:18.000000 metacells-0.8.0/pybind11/include/pybind11/embed.h
--rw-rw----   0 obk       (2045) dialout     (18)     4382 2021-11-12 17:22:18.000000 metacells-0.8.0/pybind11/include/pybind11/eval.h
--rw-rw----   0 obk       (2045) dialout     (18)     3635 2021-11-12 17:22:18.000000 metacells-0.8.0/pybind11/include/pybind11/functional.h
--rw-rw----   0 obk       (2045) dialout     (18)     5709 2021-11-12 17:22:18.000000 metacells-0.8.0/pybind11/include/pybind11/iostream.h
--rw-rw----   0 obk       (2045) dialout     (18)    68080 2021-11-12 17:22:18.000000 metacells-0.8.0/pybind11/include/pybind11/numpy.h
--rw-rw----   0 obk       (2045) dialout     (18)     9085 2021-11-12 17:22:18.000000 metacells-0.8.0/pybind11/include/pybind11/operators.h
--rw-rw----   0 obk       (2045) dialout     (18)     2049 2021-11-12 17:22:18.000000 metacells-0.8.0/pybind11/include/pybind11/options.h
--rw-rw----   0 obk       (2045) dialout     (18)   100078 2021-11-12 17:22:18.000000 metacells-0.8.0/pybind11/include/pybind11/pybind11.h
--rw-rw----   0 obk       (2045) dialout     (18)    63033 2021-11-12 17:22:18.000000 metacells-0.8.0/pybind11/include/pybind11/pytypes.h
--rw-rw----   0 obk       (2045) dialout     (18)    14109 2021-11-12 17:22:18.000000 metacells-0.8.0/pybind11/include/pybind11/stl.h
--rw-rw----   0 obk       (2045) dialout     (18)    23293 2021-11-12 17:22:18.000000 metacells-0.8.0/pybind11/include/pybind11/stl_bind.h
--rw-r-----   0 obk       (2045) dialout     (18)      104 2021-11-12 17:11:30.000000 metacells-0.8.0/requirements.txt
--rw-r-----   0 obk       (2045) dialout     (18)      111 2022-03-14 11:49:38.000000 metacells-0.8.0/requirements_dev.txt
--rw-r-----   0 obk       (2045) dialout     (18)       25 2021-11-12 17:18:46.000000 metacells-0.8.0/requirements_test.txt
--rw-rw----   0 obk       (2045) dialout     (18)     1115 2022-04-04 06:01:47.000000 metacells-0.8.0/setup.cfg
--rw-rw----   0 obk       (2045) dialout     (18)     3618 2022-04-03 11:43:28.000000 metacells-0.8.0/setup.py
-drwxrwx---   0 obk       (2045) dialout     (18)        0 2022-04-04 06:01:47.000000 metacells-0.8.0/tests/
--rw-rw----   0 obk       (2045) dialout     (18)        0 2021-11-12 17:21:34.000000 metacells-0.8.0/tests/__init__.py
--rw-rw----   0 obk       (2045) dialout     (18)     2968 2022-03-21 13:58:40.000000 metacells-0.8.0/tests/test_data.py
--rw-rw----   0 obk       (2045) dialout     (18)    19902 2021-11-12 17:54:51.000000 metacells-0.8.0/tests/test_utilities.py
+drwxrwx---   0 obk       (2045) dialout     (18)        0 2023-07-25 17:41:47.585851 metacells-0.9.0/
+-rw-rw----   0 obk       (2045) dialout     (18)     1195 2023-01-29 13:49:38.000000 metacells-0.9.0/HISTORY.rst
+-rw-rw----   0 obk       (2045) dialout     (18)     1122 2023-07-25 14:10:15.000000 metacells-0.9.0/LICENSE.rst
+-rw-rw----   0 obk       (2045) dialout     (18)      422 2021-11-12 17:44:22.000000 metacells-0.9.0/MANIFEST.in
+-rw-rw----   0 obk       (2045) dialout     (18)    35765 2023-07-25 17:41:47.586853 metacells-0.9.0/PKG-INFO
+-rw-rw----   0 obk       (2045) dialout     (18)    33678 2023-07-25 14:10:01.000000 metacells-0.9.0/README.rst
+drwxrwx---   0 obk       (2045) dialout     (18)        0 2023-07-25 17:41:47.468850 metacells-0.9.0/metacells/
+-rw-rw----   0 obk       (2045) dialout     (18)      415 2023-07-25 14:04:38.000000 metacells-0.9.0/metacells/__init__.py
+-rw-rw----   0 obk       (2045) dialout     (18)    10056 2023-05-12 15:23:36.000000 metacells-0.9.0/metacells/auroc.cpp
+-rw-rw----   0 obk       (2045) dialout     (18)     1717 2023-05-12 15:35:55.000000 metacells-0.9.0/metacells/check_avx2.py
+-rw-rw----   0 obk       (2045) dialout     (18)    18125 2023-05-12 15:23:36.000000 metacells-0.9.0/metacells/choose_seeds.cpp
+-rw-rw----   0 obk       (2045) dialout     (18)    26798 2023-05-12 15:23:36.000000 metacells-0.9.0/metacells/correlate.cpp
+-rw-rw----   0 obk       (2045) dialout     (18)    11378 2023-05-12 15:23:36.000000 metacells-0.9.0/metacells/cover.cpp
+-rw-rw----   0 obk       (2045) dialout     (18)     9054 2023-05-12 15:23:36.000000 metacells-0.9.0/metacells/downsample.cpp
+-rw-rw----   0 obk       (2045) dialout     (18)     2318 2023-05-12 15:23:36.000000 metacells-0.9.0/metacells/extensions.cpp
+-rw-rw----   0 obk       (2045) dialout     (18)    19578 2023-05-12 15:23:36.000000 metacells-0.9.0/metacells/extensions.h
+-rw-rw----   0 obk       (2045) dialout     (18)    11330 2023-05-12 15:23:36.000000 metacells-0.9.0/metacells/folds.cpp
+-rw-rw----   0 obk       (2045) dialout     (18)    10398 2023-05-12 15:23:36.000000 metacells-0.9.0/metacells/gaps.cpp
+-rw-rw----   0 obk       (2045) dialout     (18)     6114 2023-05-12 15:23:36.000000 metacells-0.9.0/metacells/logistics.cpp
+-rw-rw----   0 obk       (2045) dialout     (18)    51319 2023-07-22 15:26:40.000000 metacells-0.9.0/metacells/parameters.py
+-rw-rw----   0 obk       (2045) dialout     (18)    60032 2023-05-12 15:29:07.000000 metacells-0.9.0/metacells/partitions.cpp
+drwxrwx---   0 obk       (2045) dialout     (18)        0 2023-07-25 17:41:47.494849 metacells-0.9.0/metacells/pipeline/
+-rw-rw----   0 obk       (2045) dialout     (18)      781 2023-01-17 12:47:00.000000 metacells-0.9.0/metacells/pipeline/__init__.py
+-rw-rw----   0 obk       (2045) dialout     (18)    14848 2023-07-25 13:48:34.000000 metacells-0.9.0/metacells/pipeline/collect.py
+-rw-rw----   0 obk       (2045) dialout     (18)     9490 2023-05-12 15:35:55.000000 metacells-0.9.0/metacells/pipeline/consistency.py
+-rw-rw----   0 obk       (2045) dialout     (18)    18936 2023-05-09 17:16:29.000000 metacells-0.9.0/metacells/pipeline/direct.py
+-rw-rw----   0 obk       (2045) dialout     (18)    64655 2023-06-04 11:20:41.000000 metacells-0.9.0/metacells/pipeline/divide_and_conquer.py
+-rw-rw----   0 obk       (2045) dialout     (18)     9737 2023-05-02 12:07:29.000000 metacells-0.9.0/metacells/pipeline/exclude.py
+-rw-rw----   0 obk       (2045) dialout     (18)     9188 2023-06-13 10:56:50.000000 metacells-0.9.0/metacells/pipeline/mark.py
+-rw-rw----   0 obk       (2045) dialout     (18)     7266 2023-05-12 15:20:49.000000 metacells-0.9.0/metacells/pipeline/mcview.py
+-rw-rw----   0 obk       (2045) dialout     (18)    85403 2023-07-22 15:42:42.000000 metacells-0.9.0/metacells/pipeline/projection.py
+-rw-rw----   0 obk       (2045) dialout     (18)     9040 2023-05-16 07:01:33.000000 metacells-0.9.0/metacells/pipeline/related_genes.py
+-rw-rw----   0 obk       (2045) dialout     (18)     5973 2023-05-09 14:13:08.000000 metacells-0.9.0/metacells/pipeline/select.py
+-rw-rw----   0 obk       (2045) dialout     (18)    12574 2023-07-09 13:34:29.000000 metacells-0.9.0/metacells/pipeline/umap.py
+-rw-rw----   0 obk       (2045) dialout     (18)     6153 2023-05-12 15:23:36.000000 metacells-0.9.0/metacells/prune_per.cpp
+-rw-rw----   0 obk       (2045) dialout     (18)        0 2021-12-30 15:42:34.000000 metacells-0.9.0/metacells/py.typed
+-rw-rw----   0 obk       (2045) dialout     (18)     4172 2023-05-12 15:23:36.000000 metacells-0.9.0/metacells/rank.cpp
+-rw-rw----   0 obk       (2045) dialout     (18)     8999 2023-05-12 15:29:07.000000 metacells-0.9.0/metacells/relayout.cpp
+drwxrwx---   0 obk       (2045) dialout     (18)        0 2023-07-25 17:41:47.497849 metacells-0.9.0/metacells/scripts/
+-rw-rw----   0 obk       (2045) dialout     (18)       55 2021-11-12 17:54:50.000000 metacells-0.9.0/metacells/scripts/__init__.py
+-rw-rw----   0 obk       (2045) dialout     (18)     9359 2023-05-02 12:45:18.000000 metacells-0.9.0/metacells/scripts/timing.py
+-rw-rw----   0 obk       (2045) dialout     (18)       99 2023-07-25 17:41:46.000000 metacells-0.9.0/metacells/should_check_avx2.py
+-rw-rw----   0 obk       (2045) dialout     (18)     5554 2023-05-12 15:23:36.000000 metacells-0.9.0/metacells/shuffle.cpp
+drwxrwx---   0 obk       (2045) dialout     (18)        0 2023-07-25 17:41:47.527851 metacells-0.9.0/metacells/tools/
+-rw-rw----   0 obk       (2045) dialout     (18)     1148 2022-12-13 18:23:20.000000 metacells-0.9.0/metacells/tools/__init__.py
+-rw-rw----   0 obk       (2045) dialout     (18)     6922 2021-11-12 19:41:57.000000 metacells-0.9.0/metacells/tools/apply.py
+-rw-rw----   0 obk       (2045) dialout     (18)     9812 2023-05-02 12:45:18.000000 metacells-0.9.0/metacells/tools/bursty_lonely.py
+-rw-rw----   0 obk       (2045) dialout     (18)    32880 2023-05-12 15:40:14.000000 metacells-0.9.0/metacells/tools/candidates.py
+-rw-rw----   0 obk       (2045) dialout     (18)     8401 2023-05-02 12:45:18.000000 metacells-0.9.0/metacells/tools/convey.py
+-rw-rw----   0 obk       (2045) dialout     (18)    29577 2023-03-30 09:53:45.000000 metacells-0.9.0/metacells/tools/deviants.py
+-rw-rw----   0 obk       (2045) dialout     (18)     9323 2023-03-13 12:28:32.000000 metacells-0.9.0/metacells/tools/dissolve.py
+-rw-rw----   0 obk       (2045) dialout     (18)     9289 2023-02-12 20:13:47.000000 metacells-0.9.0/metacells/tools/distinct.py
+-rw-rw----   0 obk       (2045) dialout     (18)     4170 2023-04-11 12:53:50.000000 metacells-0.9.0/metacells/tools/downsample.py
+-rw-rw----   0 obk       (2045) dialout     (18)     4153 2023-05-09 13:01:01.000000 metacells-0.9.0/metacells/tools/filter.py
+-rw-rw----   0 obk       (2045) dialout     (18)     7131 2023-05-02 12:41:15.000000 metacells-0.9.0/metacells/tools/group.py
+-rw-rw----   0 obk       (2045) dialout     (18)    13788 2023-05-02 12:42:10.000000 metacells-0.9.0/metacells/tools/high.py
+-rw-rw----   0 obk       (2045) dialout     (18)    15429 2023-06-18 09:46:49.000000 metacells-0.9.0/metacells/tools/knn_graph.py
+-rw-rw----   0 obk       (2045) dialout     (18)     6020 2023-05-02 12:45:17.000000 metacells-0.9.0/metacells/tools/layout.py
+-rw-rw----   0 obk       (2045) dialout     (18)     3768 2023-05-02 12:15:33.000000 metacells-0.9.0/metacells/tools/mask.py
+-rw-rw----   0 obk       (2045) dialout     (18)     3012 2023-07-06 08:56:26.000000 metacells-0.9.0/metacells/tools/named.py
+-rw-rw----   0 obk       (2045) dialout     (18)    21027 2023-07-09 13:35:11.000000 metacells-0.9.0/metacells/tools/project.py
+-rw-rw----   0 obk       (2045) dialout     (18)     5828 2023-05-02 12:41:58.000000 metacells-0.9.0/metacells/tools/properly_sampled.py
+-rw-rw----   0 obk       (2045) dialout     (18)    37341 2023-07-22 15:26:00.000000 metacells-0.9.0/metacells/tools/quality.py
+-rw-rw----   0 obk       (2045) dialout     (18)    29363 2023-06-18 09:46:49.000000 metacells-0.9.0/metacells/tools/rare.py
+-rw-rw----   0 obk       (2045) dialout     (18)     9318 2023-05-16 07:22:01.000000 metacells-0.9.0/metacells/tools/similarity.py
+-rw-rw----   0 obk       (2045) dialout     (18)     4042 2023-05-12 15:23:36.000000 metacells-0.9.0/metacells/top_per.cpp
+drwxrwx---   0 obk       (2045) dialout     (18)        0 2023-07-25 17:41:47.541852 metacells-0.9.0/metacells/utilities/
+-rw-rw----   0 obk       (2045) dialout     (18)      423 2022-03-28 17:08:32.000000 metacells-0.9.0/metacells/utilities/__init__.py
+-rw-rw----   0 obk       (2045) dialout     (18)    37159 2023-06-18 11:06:13.000000 metacells-0.9.0/metacells/utilities/annotation.py
+-rw-rw----   0 obk       (2045) dialout     (18)    91947 2023-06-18 09:46:50.000000 metacells-0.9.0/metacells/utilities/computation.py
+-rw-rw----   0 obk       (2045) dialout     (18)     1925 2021-11-12 19:08:40.000000 metacells-0.9.0/metacells/utilities/documentation.py
+-rw-rw----   0 obk       (2045) dialout     (18)    27494 2023-06-18 09:46:50.000000 metacells-0.9.0/metacells/utilities/logging.py
+-rw-rw----   0 obk       (2045) dialout     (18)    10270 2023-04-03 13:41:21.000000 metacells-0.9.0/metacells/utilities/parallel.py
+-rw-rw----   0 obk       (2045) dialout     (18)     5560 2023-05-15 14:52:37.000000 metacells-0.9.0/metacells/utilities/progress.py
+-rw-rw----   0 obk       (2045) dialout     (18)        0 2021-11-12 17:21:33.000000 metacells-0.9.0/metacells/utilities/py.typed
+-rw-rw----   0 obk       (2045) dialout     (18)    15037 2023-05-02 12:44:38.000000 metacells-0.9.0/metacells/utilities/timing.py
+-rw-rw----   0 obk       (2045) dialout     (18)    31693 2023-05-12 15:36:59.000000 metacells-0.9.0/metacells/utilities/typing.py
+drwxrwx---   0 obk       (2045) dialout     (18)        0 2023-07-25 17:41:47.476850 metacells-0.9.0/metacells.egg-info/
+-rw-rw----   0 obk       (2045) dialout     (18)    35765 2023-07-25 17:41:47.000000 metacells-0.9.0/metacells.egg-info/PKG-INFO
+-rw-rw----   0 obk       (2045) dialout     (18)     3093 2023-07-25 17:41:47.000000 metacells-0.9.0/metacells.egg-info/SOURCES.txt
+-rw-rw----   0 obk       (2045) dialout     (18)        1 2023-07-25 17:41:47.000000 metacells-0.9.0/metacells.egg-info/dependency_links.txt
+-rw-rw----   0 obk       (2045) dialout     (18)       67 2023-07-25 17:41:47.000000 metacells-0.9.0/metacells.egg-info/entry_points.txt
+-rw-rw----   0 obk       (2045) dialout     (18)      234 2023-07-25 17:41:47.000000 metacells-0.9.0/metacells.egg-info/requires.txt
+-rw-rw----   0 obk       (2045) dialout     (18)       83 2023-07-25 17:41:47.000000 metacells-0.9.0/metacells.egg-info/top_level.txt
+drwxrwx---   0 obk       (2045) dialout     (18)        0 2023-07-25 17:41:47.427848 metacells-0.9.0/pybind11/
+drwxrwx---   0 obk       (2045) dialout     (18)        0 2023-07-25 17:41:47.427854 metacells-0.9.0/pybind11/include/
+drwxrwx---   0 obk       (2045) dialout     (18)        0 2023-07-25 17:41:47.570852 metacells-0.9.0/pybind11/include/pybind11/
+-rw-rw----   0 obk       (2045) dialout     (18)    20302 2021-11-12 17:22:18.000000 metacells-0.9.0/pybind11/include/pybind11/attr.h
+-rw-rw----   0 obk       (2045) dialout     (18)     4962 2021-11-12 17:22:18.000000 metacells-0.9.0/pybind11/include/pybind11/buffer_info.h
+-rw-rw----   0 obk       (2045) dialout     (18)    93351 2021-11-12 17:22:18.000000 metacells-0.9.0/pybind11/include/pybind11/cast.h
+-rw-rw----   0 obk       (2045) dialout     (18)     7737 2021-11-12 17:22:18.000000 metacells-0.9.0/pybind11/include/pybind11/chrono.h
+-rw-rw----   0 obk       (2045) dialout     (18)      120 2021-11-12 17:22:18.000000 metacells-0.9.0/pybind11/include/pybind11/common.h
+-rw-rw----   0 obk       (2045) dialout     (18)     2037 2021-11-12 17:22:18.000000 metacells-0.9.0/pybind11/include/pybind11/complex.h
+drwxrwx---   0 obk       (2045) dialout     (18)        0 2023-07-25 17:41:47.580849 metacells-0.9.0/pybind11/include/pybind11/detail/
+-rw-rw----   0 obk       (2045) dialout     (18)    26382 2021-11-12 17:22:18.000000 metacells-0.9.0/pybind11/include/pybind11/detail/class.h
+-rw-rw----   0 obk       (2045) dialout     (18)    38908 2021-11-12 17:22:18.000000 metacells-0.9.0/pybind11/include/pybind11/detail/common.h
+-rw-rw----   0 obk       (2045) dialout     (18)     3602 2021-11-12 17:22:18.000000 metacells-0.9.0/pybind11/include/pybind11/detail/descr.h
+-rw-rw----   0 obk       (2045) dialout     (18)    16376 2021-11-12 17:22:18.000000 metacells-0.9.0/pybind11/include/pybind11/detail/init.h
+-rw-rw----   0 obk       (2045) dialout     (18)    16064 2021-11-12 17:22:18.000000 metacells-0.9.0/pybind11/include/pybind11/detail/internals.h
+-rw-rw----   0 obk       (2045) dialout     (18)     1486 2021-11-12 17:22:18.000000 metacells-0.9.0/pybind11/include/pybind11/detail/typeid.h
+-rw-rw----   0 obk       (2045) dialout     (18)    29079 2021-11-12 17:22:18.000000 metacells-0.9.0/pybind11/include/pybind11/eigen.h
+-rw-rw----   0 obk       (2045) dialout     (18)     7955 2021-11-12 17:22:18.000000 metacells-0.9.0/pybind11/include/pybind11/embed.h
+-rw-rw----   0 obk       (2045) dialout     (18)     4382 2021-11-12 17:22:18.000000 metacells-0.9.0/pybind11/include/pybind11/eval.h
+-rw-rw----   0 obk       (2045) dialout     (18)     3635 2021-11-12 17:22:18.000000 metacells-0.9.0/pybind11/include/pybind11/functional.h
+-rw-rw----   0 obk       (2045) dialout     (18)     5709 2021-11-12 17:22:18.000000 metacells-0.9.0/pybind11/include/pybind11/iostream.h
+-rw-rw----   0 obk       (2045) dialout     (18)    68080 2021-11-12 17:22:18.000000 metacells-0.9.0/pybind11/include/pybind11/numpy.h
+-rw-rw----   0 obk       (2045) dialout     (18)     9085 2021-11-12 17:22:18.000000 metacells-0.9.0/pybind11/include/pybind11/operators.h
+-rw-rw----   0 obk       (2045) dialout     (18)     2049 2021-11-12 17:22:18.000000 metacells-0.9.0/pybind11/include/pybind11/options.h
+-rw-rw----   0 obk       (2045) dialout     (18)   100078 2021-11-12 17:22:18.000000 metacells-0.9.0/pybind11/include/pybind11/pybind11.h
+-rw-rw----   0 obk       (2045) dialout     (18)    63033 2021-11-12 17:22:18.000000 metacells-0.9.0/pybind11/include/pybind11/pytypes.h
+-rw-rw----   0 obk       (2045) dialout     (18)    14109 2021-11-12 17:22:18.000000 metacells-0.9.0/pybind11/include/pybind11/stl.h
+-rw-rw----   0 obk       (2045) dialout     (18)    23293 2021-11-12 17:22:18.000000 metacells-0.9.0/pybind11/include/pybind11/stl_bind.h
+-rw-r-----   0 obk       (2045) dialout     (18)      116 2023-05-13 20:06:52.000000 metacells-0.9.0/requirements.txt
+-rw-r-----   0 obk       (2045) dialout     (18)      111 2022-03-14 11:49:38.000000 metacells-0.9.0/requirements_dev.txt
+-rw-r-----   0 obk       (2045) dialout     (18)       25 2021-11-12 17:18:46.000000 metacells-0.9.0/requirements_test.txt
+-rw-rw----   0 obk       (2045) dialout     (18)     1121 2023-07-25 17:41:47.587854 metacells-0.9.0/setup.cfg
+-rw-rw----   0 obk       (2045) dialout     (18)     3837 2023-07-25 17:40:46.000000 metacells-0.9.0/setup.py
+drwxrwx---   0 obk       (2045) dialout     (18)        0 2023-07-25 17:41:47.584851 metacells-0.9.0/tests/
+-rw-rw----   0 obk       (2045) dialout     (18)        0 2021-11-12 17:21:34.000000 metacells-0.9.0/tests/__init__.py
+-rw-rw----   0 obk       (2045) dialout     (18)     2995 2023-05-16 07:32:31.000000 metacells-0.9.0/tests/test_data.py
+-rw-rw----   0 obk       (2045) dialout     (18)    19833 2023-05-09 13:36:43.000000 metacells-0.9.0/tests/test_utilities.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `metacells-0.8.0/LICENSE.rst` & `metacells-0.9.0/LICENSE.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 The MIT License (MIT)
 =====================
 
-Copyright © 2020, 2021 Weizmann Institute of Science
+Copyright © 2020-2023 Weizmann Institute of Science
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
 persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the
```

### Comparing `metacells-0.8.0/metacells/auroc.cpp` & `metacells-0.9.0/metacells/auroc.cpp`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/metacells/check_avx2.py` & `metacells-0.9.0/metacells/check_avx2.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 import os
 from warnings import warn
 
 HAS_AVX2 = None
 try:
-    with (open("/proc/cpuinfo", encoding="utf8") if os.path.exists("/proc/cpuinfo") else os.popen("sysctl -a")) as file:
+    with open("/proc/cpuinfo", encoding="utf8") if os.path.exists("/proc/cpuinfo") else os.popen("sysctl -a") as file:
         for line in file.readlines():
             if line.startswith("flags"):
                 features = line.split(" ")
                 HAS_AVX2 = "avx2" in features and "fma" in features
                 break
 except BaseException:  # pylint: disable=broad-except
     pass
```

### Comparing `metacells-0.8.0/metacells/choose_seeds.cpp` & `metacells-0.9.0/metacells/choose_seeds.cpp`

 * *Files 22% similar despite different names*

```diff
@@ -157,14 +157,87 @@
                                         [&](size_t candidate_node_index) {
                                             return connected_nodes[candidate_node_index].size() == 0;
                                         }),
                          tmp_candidates.end());
     return tmp_candidates.size() > 0;
 }
 
+static bool
+connect_node(size_t node_index,
+             ArraySlice<int32_t> seed_of_nodes,
+             ConstCompressedMatrix<float32_t, int32_t, int32_t>& outgoing_weights,
+             ConstCompressedMatrix<float32_t, int32_t, int32_t>& incoming_weights,
+             std::vector<float32_t>& seed_weights) {
+    if (seed_of_nodes[node_index] >= 0) {
+        return true;
+    }
+
+    std::fill(seed_weights.begin(), seed_weights.end(), 0.0);
+
+    auto incoming_node_indices = incoming_weights.get_band_indices(node_index);
+    auto incoming_edge_weights = incoming_weights.get_band_data(node_index);
+    size_t incoming_nodes_count = incoming_node_indices.size();
+    for (size_t position = 0; position < incoming_nodes_count; ++position) {
+        auto other_node_index = incoming_node_indices[position];
+        auto other_node_seed = seed_of_nodes[other_node_index];
+        if (other_node_seed >= 0) {
+            seed_weights[other_node_seed] += incoming_edge_weights[position];
+        }
+    }
+
+    auto outgoing_node_indices = outgoing_weights.get_band_indices(node_index);
+    auto outgoing_edge_weights = outgoing_weights.get_band_data(node_index);
+    size_t outgoing_nodes_count = outgoing_node_indices.size();
+    for (size_t position = 0; position < outgoing_nodes_count; ++position) {
+        auto other_node_index = outgoing_node_indices[position];
+        auto other_node_seed = seed_of_nodes[other_node_index];
+        if (other_node_seed >= 0) {
+            seed_weights[other_node_seed] += outgoing_edge_weights[position];
+        }
+    }
+
+    auto max_seed_weight = std::max_element(seed_weights.begin(), seed_weights.end());
+    if (*max_seed_weight == 0.0) {
+        return false;
+    }
+
+    size_t max_seed_index = max_seed_weight - seed_weights.begin();
+    seed_of_nodes[node_index] = max_seed_index;
+    return true;
+}
+
+static void
+do_complete_seeds(ArraySlice<int32_t> seed_of_nodes,
+                  size_t seeds_count,
+                  ConstCompressedMatrix<float32_t, int32_t, int32_t>& outgoing_weights,
+                  ConstCompressedMatrix<float32_t, int32_t, int32_t>& incoming_weights) {
+    size_t nodes_count = seed_of_nodes.size();
+    std::vector<float32_t> seed_weights(seeds_count);
+
+    std::vector<size_t> old_disconnected_nodes;
+    std::vector<size_t> new_disconnected_nodes;
+
+    for (size_t node_index = 0; node_index < nodes_count; ++node_index) {
+        if (!connect_node(node_index, seed_of_nodes, outgoing_weights, incoming_weights, seed_weights)) {
+            new_disconnected_nodes.push_back(node_index);
+        }
+    }
+
+    while (new_disconnected_nodes.size() > 0) {
+        std::swap(old_disconnected_nodes, new_disconnected_nodes);
+        new_disconnected_nodes.clear();
+        for (size_t node_index : old_disconnected_nodes) {
+            if (!connect_node(node_index, seed_of_nodes, outgoing_weights, incoming_weights, seed_weights)) {
+                new_disconnected_nodes.push_back(node_index);
+            }
+        }
+        FastAssertCompare(new_disconnected_nodes.size(), <, old_disconnected_nodes.size());
+    }
+}
+
 /// See the Python `metacell.tools.candidates._choose_seeds` function.
 void
 choose_seeds(const pybind11::array_t<float32_t>& outgoing_weights_data_array,
              const pybind11::array_t<int32_t>& outgoing_weights_indices_array,
              const pybind11::array_t<int32_t>& outgoing_weights_indptr_array,
              const pybind11::array_t<float32_t>& incoming_weights_data_array,
              const pybind11::array_t<int32_t>& incoming_weights_indices_array,
@@ -229,17 +302,14 @@
                         tmp_candidates,
                         connected_nodes,
                         seed_of_nodes,
                         mean_seed_size);
         ++seeds_count;
     }
 
-    size_t strong_seeds_count = seeds_count;
-    FastAssertCompare(strong_seeds_count, >, given_seeds_count);
-
     if (seeds_count < max_seeds_count) {
         tmp_candidates.clear();
         for (size_t node_index = 0; node_index < nodes_count; ++node_index) {
             if (seed_of_nodes[node_index] < 0) {
                 tmp_candidates.push_back(node_index);
             }
         }
@@ -259,15 +329,51 @@
             tmp_candidates.pop_back();
             seed_of_nodes[node_index] = int32_t(seeds_count);
             ++seeds_count;
         }
     }
 
     FastAssertCompare(seeds_count, ==, max_seeds_count);
+
+    do_complete_seeds(seed_of_nodes, seeds_count, outgoing_weights, incoming_weights);
+}
+
+static void
+complete_seeds(const pybind11::array_t<float32_t>& outgoing_weights_data_array,
+               const pybind11::array_t<int32_t>& outgoing_weights_indices_array,
+               const pybind11::array_t<int32_t>& outgoing_weights_indptr_array,
+               const pybind11::array_t<float32_t>& incoming_weights_data_array,
+               const pybind11::array_t<int32_t>& incoming_weights_indices_array,
+               const pybind11::array_t<int32_t>& incoming_weights_indptr_array,
+               size_t seeds_count,
+               pybind11::array_t<int32_t>& seed_of_nodes_array) {
+    WithoutGil without_gil{};
+    ArraySlice<int32_t> seed_of_nodes = ArraySlice<int32_t>(seed_of_nodes_array, "seed_of_nodes");
+    size_t nodes_count = seed_of_nodes.size();
+    FastAssertCompare(nodes_count, >, 0);
+
+    ConstCompressedMatrix<float32_t, int32_t, int32_t>
+        outgoing_weights(ConstArraySlice<float32_t>(outgoing_weights_data_array, "outgoing_weights_data"),
+                         ConstArraySlice<int32_t>(outgoing_weights_indices_array, "outgoing_weights_indices"),
+                         ConstArraySlice<int32_t>(outgoing_weights_indptr_array, "outgoing_weights_indptr"),
+                         int32_t(nodes_count),
+                         "outgoing_weights");
+    FastAssertCompare(outgoing_weights.bands_count(), ==, nodes_count);
+
+    ConstCompressedMatrix<float32_t, int32_t, int32_t>
+        incoming_weights(ConstArraySlice<float32_t>(incoming_weights_data_array, "incoming_weights_data"),
+                         ConstArraySlice<int32_t>(incoming_weights_indices_array, "incoming_weights_indices"),
+                         ConstArraySlice<int32_t>(incoming_weights_indptr_array, "incoming_weights_indptr"),
+                         int32_t(nodes_count),
+                         "incoming_weights");
+    FastAssertCompare(incoming_weights.bands_count(), ==, nodes_count);
+
+    do_complete_seeds(seed_of_nodes, seeds_count, outgoing_weights, incoming_weights);
 }
 
 void
 register_choose_seeds(pybind11::module& module) {
     module.def("choose_seeds", &metacells::choose_seeds, "Choose seed partitions for computing metacells.");
+    module.def("complete_seeds", &metacells::complete_seeds, "Complete seed partitions for computing metacells.");
 }
 
 }
```

### Comparing `metacells-0.8.0/metacells/correlate.cpp` & `metacells-0.9.0/metacells/correlate.cpp`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/metacells/cover.cpp` & `metacells-0.9.0/metacells/cover.cpp`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/metacells/downsample.cpp` & `metacells-0.9.0/metacells/downsample.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -76,87 +76,91 @@
             random = right_random;
         }
     }
 }
 
 template<typename D, typename O>
 static void
-downsample_slice(ConstArraySlice<D> input, ArraySlice<O> output, const size_t samples, const size_t random_seed) {
-    FastAssertCompare(samples, >=, 0);
+downsample_slice(ConstArraySlice<D> input, ArraySlice<O> output, const int32_t samples, const size_t random_seed) {
     FastAssertCompare(output.size(), ==, input.size());
 
-    if (input.size() == 0) {
+    if (samples < 0 || input.size() == 0) {
         return;
     }
 
     if (input.size() == 1) {
         output[0] = O(float64_t(samples) < float64_t(input[0]) ? samples : input[0]);
         return;
     }
 
     TmpVectorSizeT raii_tree;
     auto tree = raii_tree.array_slice("tmp_tree", downsample_tmp_size(input.size()));
     initialize_tree(input, tree);
     size_t& total = tree[tree.size() - 1];
 
-    if (total <= samples) {
+    if (total <= size_t(samples)) {
         if (static_cast<const void*>(output.begin()) != static_cast<const void*>(input.begin())) {
             std::copy(input.begin(), input.end(), output.begin());
         }
         return;
     }
 
     std::fill(output.begin(), output.end(), O(0));
 
     std::minstd_rand random(random_seed);
-    for (size_t index = 0; index < samples; ++index) {
+    for (size_t index = 0; index < size_t(samples); ++index) {
         ++output[random_sample(tree, random() % total)];
     }
 }
 
 /// See the Python `metacell.utilities.computation.downsample_array` function.
 template<typename D, typename O>
 static void
 downsample_array(const pybind11::array_t<D>& input_array,
                  pybind11::array_t<O>& output_array,
-                 const size_t samples,
+                 const int32_t samples,
                  const size_t random_seed) {
     WithoutGil without_gil{};
 
     ConstArraySlice<D> input{ input_array, "input_array" };
     ArraySlice<O> output{ output_array, "output_array" };
 
     downsample_slice(input, output, samples, random_seed);
 }
 
 /// See the Python `metacell.utilities.computation.downsample_matrix` function.
 template<typename D, typename O>
 static void
 downsample_dense(const pybind11::array_t<D>& input_matrix,
                  pybind11::array_t<O>& output_array,
-                 const size_t samples,
+                 const pybind11::array_t<int32_t>& samples_array,
                  const size_t random_seed) {
     WithoutGil without_gil{};
 
     ConstMatrixSlice<D> input{ input_matrix, "input_matrix" };
     MatrixSlice<O> output{ output_array, "output_array" };
+    ConstArraySlice<int32_t> samples{ samples_array, "samples_array" };
+
+    FastAssertCompare(output.columns_count(), ==, input.columns_count());
+    FastAssertCompare(output.rows_count(), ==, input.rows_count());
+    FastAssertCompare(samples.size(), ==, input.rows_count());
 
     parallel_loop(input.rows_count(), [&](const size_t row_index) {
         size_t slice_seed = random_seed == 0 ? 0 : random_seed + row_index * 997;
-        downsample_slice(input.get_row(row_index), output.get_row(row_index), samples, slice_seed);
+        downsample_slice(input.get_row(row_index), output.get_row(row_index), samples[row_index], slice_seed);
     });
 }
 
 template<typename D, typename P, typename O>
 static void
 downsample_band(const size_t band_index,
                 ConstArraySlice<D> input_data,
                 ConstArraySlice<P> input_indptr,
                 ArraySlice<O> output,
-                const size_t samples,
+                const int32_t samples,
                 const size_t random_seed) {
     auto start_element_offset = input_indptr[band_index];
     auto stop_element_offset = input_indptr[band_index + 1];
 
     auto band_input = input_data.slice(start_element_offset, stop_element_offset);
     auto band_output = output.slice(start_element_offset, stop_element_offset);
 
@@ -165,25 +169,29 @@
 
 /// See the Python `metacell.utilities.computation.downsample_matrix` function.
 template<typename D, typename P, typename O>
 static void
 downsample_compressed(const pybind11::array_t<D>& input_data_array,
                       const pybind11::array_t<P>& input_indptr_array,
                       pybind11::array_t<O>& output_array,
-                      const size_t samples,
+                      const pybind11::array_t<int32_t>& samples_array,
                       const size_t random_seed) {
     WithoutGil without_gil{};
 
     ConstArraySlice<D> input_data{ input_data_array, "input_data_array" };
     ConstArraySlice<P> input_indptr{ input_indptr_array, "input_indptr_array" };
     ArraySlice<O> output{ output_array, "output_array" };
+    ConstArraySlice<int32_t> samples{ samples_array, "samples_array" };
+
+    FastAssertCompare(output.size(), ==, input_data.size());
+    FastAssertCompare(samples.size(), ==, input_indptr.size() - 1);
 
     parallel_loop(input_indptr.size() - 1, [&](size_t band_index) {
         size_t band_seed = random_seed == 0 ? 0 : random_seed + band_index * 997;
-        downsample_band(band_index, input_data, input_indptr, output, samples, band_seed);
+        downsample_band(band_index, input_data, input_indptr, output, samples[band_index], band_seed);
     });
 }
 
 void
 register_downsample(pybind11::module& module) {
 #define REGISTER_D_O(D, O)                                                                        \
     module.def("downsample_array_" #D "_" #O, &downsample_array<D, O>, "Downsample array data."); \
```

### Comparing `metacells-0.8.0/metacells/extensions.cpp` & `metacells-0.9.0/metacells/extensions.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 
     metacells::register_auroc(module);
     metacells::register_choose_seeds(module);
     metacells::register_correlate(module);
     metacells::register_cover(module);
     metacells::register_downsample(module);
     metacells::register_folds(module);
+    metacells::register_gaps(module);
     metacells::register_logistics(module);
     metacells::register_partitions(module);
     metacells::register_prune_per(module);
     metacells::register_rank(module);
     metacells::register_relayout(module);
     metacells::register_shuffle(module);
     metacells::register_top_per(module);
```

### Comparing `metacells-0.8.0/metacells/extensions.h` & `metacells-0.9.0/metacells/extensions.h`

 * *Files 9% similar despite different names*

```diff
@@ -151,16 +151,17 @@
 
     ConstArraySlice(const T* const data, const size_t size, const char* const name)
       : m_data(data), m_size(size), m_name(name) {}
 
     ConstArraySlice(const pybind11::array_t<T>& array, const char* const name)
       : ConstArraySlice(array.data(), array.size(), name) {
         FastAssertCompareWhat(array.ndim(), ==, 1, name);
-        FastAssertCompareWhat(array.size(), >, 0, name);
-        FastAssertCompareWhat(array.data(1) - array.data(0), ==, 1, name);
+        if (array.size() > 0) {
+            FastAssertCompareWhat(array.data(1) - array.data(0), ==, 1, name);
+        }
     }
 
     std::pair<ConstArraySlice, ConstArraySlice> split(const size_t size) const {
         return std::make_pair(slice(0, size), slice(size, m_size));
     }
 
     ConstArraySlice slice(const size_t start, const size_t stop) const {
@@ -198,16 +199,17 @@
       : m_data(&vector[0]), m_size(vector.size()), m_name(name) {}
 
     ArraySlice(T* const data, const size_t size, const char* const name) : m_data(data), m_size(size), m_name(name) {}
 
     ArraySlice(pybind11::array_t<T>& array, const char* const name)
       : ArraySlice(array.mutable_data(), array.size(), name) {
         FastAssertCompareWhat(array.ndim(), ==, 1, name);
-        FastAssertCompareWhat(array.size(), >, 0, name);
-        FastAssertCompareWhat(array.data(1) - array.data(0), ==, 1, name);
+        if (array.size() > 0) {
+            FastAssertCompareWhat(array.data(1) - array.data(0), ==, 1, name);
+        }
     }
 
     std::pair<ArraySlice, ArraySlice> split(const size_t size) {
         return std::make_pair(slice(0, size), slice(size, m_size));
     }
 
     ArraySlice slice(const size_t start, const size_t stop) {
@@ -232,17 +234,15 @@
     operator ConstArraySlice<T>() const { return ConstArraySlice<T>(m_data, m_size, m_name); }
 };
 
 template<typename T>
 static size_t
 matrix_step(const pybind11::array_t<T>& array, const char* const name) {
     FastAssertCompareWhat(array.ndim(), ==, 2, name);
-    FastAssertCompareWhat(array.shape(0), >, 0, name);
-    FastAssertCompareWhat(array.shape(1), >, 0, name);
-    if (array.shape(0) == 0) {
+    if (array.shape(0) == 0 || array.shape(1) == 0) {
         return 0;
     } else {
         return array.data(1, 0) - array.data(0, 0);
     }
 }
 
 /// An immutable row-major slice of a matrix of type ``T``.
@@ -266,18 +266,28 @@
       , m_columns_count(columns_count)
       , m_rows_offset(rows_offset)
       , m_name(name) {}
 
     ConstMatrixSlice(const pybind11::array_t<T>& array, const char* const name)
       : ConstMatrixSlice(array.data(), array.shape(0), array.shape(1), matrix_step(array, name), name) {
         FastAssertCompareWhat(array.ndim(), ==, 2, name);
-        FastAssertCompareWhat(array.data(0, 1) - array.data(0, 0), ==, 1, name);
+        if (array.shape(0) > 0 && array.shape(1) > 1) {
+            FastAssertCompareWhat(array.data(0, 1) - array.data(0, 0), ==, 1, name);
+        }
         FastAssertCompareWhat(m_columns_count, <=, m_rows_offset, name);
     }
 
+    T operator()(size_t row_index, size_t column_index) const {
+        SlowAssertCompareWhat(0, <=, row_index, m_name);
+        SlowAssertCompareWhat(row_index, <, m_rows_count, m_name);
+        SlowAssertCompareWhat(0, <=, column_index, m_name);
+        SlowAssertCompareWhat(column_index, <, m_columns_count, m_name);
+        return m_data[row_index * m_rows_offset + column_index];
+    }
+
     ConstArraySlice<T> get_row(size_t row_index) const {
         FastAssertCompareWhat(0, <=, row_index, m_name);
         FastAssertCompareWhat(row_index, <, m_rows_count, m_name);
         return ConstArraySlice<T>(m_data + row_index * m_rows_offset, m_columns_count, m_name);
     }
 
     size_t rows_count() const { return m_rows_count; }
@@ -306,18 +316,28 @@
       , m_columns_count(columns_count)
       , m_rows_offset(rows_offset)
       , m_name(name) {}
 
     MatrixSlice(pybind11::array_t<T>& array, const char* const name)
       : MatrixSlice(array.mutable_data(), array.shape(0), array.shape(1), matrix_step(array, name), name) {
         FastAssertCompareWhat(array.ndim(), ==, 2, name);
-        FastAssertCompareWhat(array.data(0, 1) - array.data(0, 0), ==, 1, name);
+        if (array.shape(0) > 0 && array.shape(1) > 1) {
+            FastAssertCompareWhat(array.data(0, 1) - array.data(0, 0), ==, 1, name);
+        }
         FastAssertCompareWhat(m_columns_count, <=, m_rows_offset, name);
     }
 
+    T& operator()(size_t row_index, size_t column_index) {
+        SlowAssertCompareWhat(0, <=, row_index, m_name);
+        SlowAssertCompareWhat(row_index, <, m_rows_count, m_name);
+        SlowAssertCompareWhat(0, <=, column_index, m_name);
+        SlowAssertCompareWhat(column_index, <, m_columns_count, m_name);
+        return m_data[row_index * m_rows_offset + column_index];
+    }
+
     ArraySlice<T> get_row(size_t row_index) const {
         FastAssertCompareWhat(0, <=, row_index, m_name);
         FastAssertCompareWhat(row_index, <, m_rows_count, m_name);
         return ArraySlice<T>(m_data + row_index * m_rows_offset, m_columns_count, m_name);
     }
 
     size_t rows_count() const { return m_rows_count; }
@@ -530,14 +550,16 @@
 extern void
 register_cover(pybind11::module& module);
 extern void
 register_downsample(pybind11::module& module);
 extern void
 register_folds(pybind11::module& module);
 extern void
+register_gaps(pybind11::module& module);
+extern void
 register_logistics(pybind11::module& module);
 extern void
 register_partitions(pybind11::module& module);
 extern void
 register_prune_per(pybind11::module& module);
 extern void
 register_rank(pybind11::module& module);
```

### Comparing `metacells-0.8.0/metacells/folds.cpp` & `metacells-0.9.0/metacells/folds.cpp`

 * *Files 24% similar despite different names*

```diff
@@ -2,67 +2,45 @@
 
 namespace metacells {
 
 /// See the Python `metacell.tools.outlier_cells._collect_fold_factors` function.
 template<typename D>
 static void
 fold_factor_dense(pybind11::array_t<D>& data_array,
-                  const float64_t min_gene_fold_factor,
-                  const bool abs_folds,
                   const pybind11::array_t<D>& total_of_rows_array,
                   const pybind11::array_t<D>& fraction_of_columns_array) {
     WithoutGil without_gil{};
     MatrixSlice<D> data(data_array, "data");
     ConstArraySlice<D> total_of_rows(total_of_rows_array, "total_of_rows");
     ConstArraySlice<D> fraction_of_columns(fraction_of_columns_array, "fraction_of_columns");
 
     FastAssertCompare(total_of_rows.size(), ==, data.rows_count());
     FastAssertCompare(fraction_of_columns.size(), ==, data.columns_count());
 
     const size_t rows_count = data.rows_count();
     const size_t columns_count = data.columns_count();
-    if (abs_folds) {
-        parallel_loop(rows_count, [&](size_t row_index) {
-            const auto row_total = total_of_rows[row_index];
-            auto row_data = data.get_row(row_index);
-            for (size_t column_index = 0; column_index < columns_count; ++column_index) {
-                const auto column_fraction = fraction_of_columns[column_index];
-                const auto expected = row_total * column_fraction;
-                auto& value = row_data[column_index];
-                value = D(log((value + 1.0) / (expected + 1.0)) * LOG2_SCALE);
-                if (abs(value) < min_gene_fold_factor) {
-                    value = 0;
-                }
-            }
-        });
-    } else {
-        parallel_loop(rows_count, [&](size_t row_index) {
-            const auto row_total = total_of_rows[row_index];
-            auto row_data = data.get_row(row_index);
-            for (size_t column_index = 0; column_index < columns_count; ++column_index) {
-                const auto column_fraction = fraction_of_columns[column_index];
-                const auto expected = row_total * column_fraction;
-                auto& value = row_data[column_index];
-                value = D(log((value + 1.0) / (expected + 1.0)) * LOG2_SCALE);
-                if (value < min_gene_fold_factor) {
-                    value = 0;
-                }
-            }
-        });
-    }
+    parallel_loop(rows_count, [&](size_t row_index) {
+        const auto row_total = total_of_rows[row_index];
+        auto row_data = data.get_row(row_index);
+        for (size_t column_index = 0; column_index < columns_count; ++column_index) {
+            const auto column_fraction = fraction_of_columns[column_index];
+            const auto expected = row_total * column_fraction;
+            auto& value = row_data[column_index];
+            const auto actual = row_total * value;
+            value = abs(D(log((actual + 1.0) / (expected + 1.0)) * LOG2_SCALE));
+        }
+    });
 }
 
 /// See the Python `metacell.tools.outlier_cells._collect_fold_factors` function.
 template<typename D, typename I, typename P>
 static void
 fold_factor_compressed(pybind11::array_t<D>& data_array,
                        pybind11::array_t<I>& indices_array,
                        pybind11::array_t<P>& indptr_array,
-                       const float64_t min_gene_fold_factor,
-                       const bool abs_folds,
                        const pybind11::array_t<D>& total_of_bands_array,
                        const pybind11::array_t<D>& fraction_of_elements_array) {
     WithoutGil without_gil{};
     ConstArraySlice<D> total_of_bands(total_of_bands_array, "total_of_bands");
     ConstArraySlice<D> fraction_of_elements(fraction_of_elements_array, "fraction_of_elements");
 
     const size_t bands_count = total_of_bands.size();
@@ -78,99 +56,63 @@
 
     parallel_loop(bands_count, [&](size_t band_index) {
         const auto band_total = total_of_bands[band_index];
         auto band_indices = data.get_band_indices(band_index);
         auto band_data = data.get_band_data(band_index);
 
         const size_t band_elements_count = band_indices.size();
-        if (abs_folds) {
-            for (size_t position = 0; position < band_elements_count; ++position) {
-                const auto element_index = band_indices[position];
-                const auto element_fraction = fraction_of_elements[element_index];
-                const auto expected = band_total * element_fraction;
-                auto& value = band_data[position];
-                value = D(log((value + 1.0) / (expected + 1.0)) * LOG2_SCALE);
-                if (abs(value) < min_gene_fold_factor) {
-                    value = 0;
-                }
-            }
-        } else {
-            for (size_t position = 0; position < band_elements_count; ++position) {
-                const auto element_index = band_indices[position];
-                const auto element_fraction = fraction_of_elements[element_index];
-                const auto expected = band_total * element_fraction;
-                auto& value = band_data[position];
-                value = D(log((value + 1.0) / (expected + 1.0)) * LOG2_SCALE);
-                if (value < min_gene_fold_factor) {
-                    value = 0;
-                }
-            }
+        for (size_t position = 0; position < band_elements_count; ++position) {
+            const auto element_index = band_indices[position];
+            const auto element_fraction = fraction_of_elements[element_index];
+            const auto expected = band_total * element_fraction;
+            auto& value = band_data[position];
+            const auto actual = band_total * value;
+            value = abs(D(log((actual + 1.0) / (expected + 1.0)) * LOG2_SCALE));
         }
     });
 }
 
 template<typename D>
 static void
 collect_distinct_folds(ArraySlice<int32_t> gene_indices,
                        ArraySlice<float32_t> gene_folds,
-                       ConstArraySlice<D> fold_in_cell,
-                       bool abs_folds) {
+                       ConstArraySlice<D> fold_in_cell) {
     TmpVectorSizeT raii_indices;
     auto tmp_indices = raii_indices.array_slice("tmp_indices", fold_in_cell.size());
     std::iota(tmp_indices.begin(), tmp_indices.end(), 0);
 
-    if (abs_folds) {
-        std::nth_element(tmp_indices.begin(),
-                         tmp_indices.begin() + gene_indices.size(),
-                         tmp_indices.end(),
-                         [&](const size_t left_gene_index, const size_t right_gene_index) {
-                             const auto left_value = fold_in_cell[left_gene_index];
-                             const auto right_value = fold_in_cell[right_gene_index];
-                             return abs(left_value) > abs(right_value);
-                         });
-
-        std::sort(tmp_indices.begin(),
-                  tmp_indices.begin() + gene_indices.size(),
-                  [&](const size_t left_gene_index, const size_t right_gene_index) {
-                      const auto left_value = fold_in_cell[left_gene_index];
-                      const auto right_value = fold_in_cell[right_gene_index];
-                      return abs(left_value) > abs(right_value);
-                  });
-    } else {
-        std::nth_element(tmp_indices.begin(),
-                         tmp_indices.begin() + gene_indices.size(),
-                         tmp_indices.end(),
-                         [&](const size_t left_gene_index, const size_t right_gene_index) {
-                             const auto left_value = fold_in_cell[left_gene_index];
-                             const auto right_value = fold_in_cell[right_gene_index];
-                             return left_value > right_value;
-                         });
-
-        std::sort(tmp_indices.begin(),
-                  tmp_indices.begin() + gene_indices.size(),
-                  [&](const size_t left_gene_index, const size_t right_gene_index) {
-                      const auto left_value = fold_in_cell[left_gene_index];
-                      const auto right_value = fold_in_cell[right_gene_index];
-                      return left_value > right_value;
-                  });
-    }
+    std::nth_element(tmp_indices.begin(),
+                     tmp_indices.begin() + gene_indices.size(),
+                     tmp_indices.end(),
+                     [&](const size_t left_gene_index, const size_t right_gene_index) {
+                         const auto left_value = fold_in_cell[left_gene_index];
+                         const auto right_value = fold_in_cell[right_gene_index];
+                         return abs(left_value) > abs(right_value);
+                     });
+
+    std::sort(tmp_indices.begin(),
+              tmp_indices.begin() + gene_indices.size(),
+              [&](const size_t left_gene_index, const size_t right_gene_index) {
+                  const auto left_value = fold_in_cell[left_gene_index];
+                  const auto right_value = fold_in_cell[right_gene_index];
+                  return abs(left_value) > abs(right_value);
+              });
 
     for (size_t position = 0; position < gene_indices.size(); ++position) {
         size_t gene_index = tmp_indices[position];
         gene_indices[position] = int32_t(gene_index);
         gene_folds[position] = float32_t(fold_in_cell[gene_index]);
     }
 }
 
 template<typename D>
 static void
 top_distinct(pybind11::array_t<int32_t>& gene_indices_array,
              pybind11::array_t<float32_t>& gene_folds_array,
-             const pybind11::array_t<D>& fold_in_cells_array,
-             bool abs_folds) {
+             const pybind11::array_t<D>& fold_in_cells_array) {
     WithoutGil without_gil{};
     MatrixSlice<float32_t> gene_folds(gene_folds_array, "gene_folds");
     MatrixSlice<int32_t> gene_indices(gene_indices_array, "gene_indices");
     ConstMatrixSlice<D> fold_in_cells(fold_in_cells_array, "fold_in_cells");
 
     size_t cells_count = fold_in_cells.rows_count();
     size_t genes_count = fold_in_cells.columns_count();
@@ -180,32 +122,118 @@
     FastAssertCompare(gene_indices.rows_count(), ==, cells_count);
     FastAssertCompare(gene_folds.rows_count(), ==, cells_count);
     FastAssertCompare(gene_folds.columns_count(), ==, distinct_count);
 
     parallel_loop(cells_count, [&](size_t cell_index) {
         collect_distinct_folds(gene_indices.get_row(cell_index),
                                gene_folds.get_row(cell_index),
-                               fold_in_cells.get_row(cell_index),
-                               abs_folds);
+                               fold_in_cells.get_row(cell_index));
     });
 }
 
+/// See the Python `metacell.utilities.computation._median_sparse` function.
+template<typename D, typename I, typename P>
+static void
+median_compressed(const pybind11::array_t<D>& data_array,
+                  const pybind11::array_t<I>& indices_array,
+                  const pybind11::array_t<P>& indptr_array,
+                  const size_t elements_count,
+                  pybind11::array_t<D>& medians_array) {
+    WithoutGil without_gil{};
+
+    ConstCompressedMatrix<D, I, P> data(ConstArraySlice<D>(data_array, "data"),
+                                        ConstArraySlice<I>(indices_array, "indices"),
+                                        ConstArraySlice<P>(indptr_array, "indptr"),
+                                        elements_count,
+                                        "data");
+
+    ArraySlice<D> medians(medians_array, "medians");
+
+    const size_t bands_count = medians_array.size();
+
+    FastAssertCompare(elements_count, >, 0);
+    FastAssertCompare(data.bands_count(), ==, bands_count);
+
+    if (elements_count % 2 == 1) {
+        const size_t median_rank = elements_count / 2;
+        parallel_loop(bands_count, [&](size_t band_index) {
+            auto band_data = data.get_band_data(band_index);
+            const size_t nnz_count = band_data.size();
+            const size_t zeros_count = elements_count - nnz_count;
+
+            if (median_rank < zeros_count) {
+                medians[band_index] = 0;
+            } else {
+                size_t median_position = median_rank - zeros_count;
+
+                TmpVectorSizeT raii_indices;
+                auto tmp_indices = raii_indices.array_slice("tmp_indices", nnz_count);
+                std::iota(tmp_indices.begin(), tmp_indices.end(), 0);
+
+                std::nth_element(tmp_indices.begin(),
+                                 tmp_indices.begin() + median_position,
+                                 tmp_indices.end(),
+                                 [&](auto left, auto right) { return band_data[left] < band_data[right]; });
+                medians[band_index] = band_data[tmp_indices[median_position]];
+            }
+        });
+
+    } else {
+        const size_t high_rank = elements_count / 2;
+        const size_t low_rank = high_rank - 1;
+        parallel_loop(bands_count, [&](size_t band_index) {
+            auto band_data = data.get_band_data(band_index);
+            const size_t nnz_count = band_data.size();
+            const size_t zeros_count = elements_count - nnz_count;
+
+            if (high_rank < zeros_count) {
+                medians[band_index] = 0;
+            } else {
+                size_t high_position = high_rank - zeros_count;
+
+                TmpVectorSizeT raii_indices;
+                auto tmp_indices = raii_indices.array_slice("tmp_indices", nnz_count);
+                std::iota(tmp_indices.begin(), tmp_indices.end(), 0);
+
+                std::nth_element(tmp_indices.begin(),
+                                 tmp_indices.begin() + high_position,
+                                 tmp_indices.end(),
+                                 [&](auto left, auto right) { return band_data[left] < band_data[right]; });
+                auto high_value = band_data[tmp_indices[high_position]];
+
+                D low_value = 0;
+                if (low_rank >= zeros_count) {
+                    size_t low_index =
+                        *std::max_element(tmp_indices.begin(),
+                                          tmp_indices.begin() + high_position,
+                                          [&](auto left, auto right) { return band_data[left] < band_data[right]; });
+                    low_value = band_data[low_index];
+                }
+                medians[band_index] = (low_value + high_value) / 2;
+            }
+        });
+    }
+}
+
 void
 register_folds(pybind11::module& module) {
 #define REGISTER_F(F)                                                                                   \
     module.def("top_distinct_" #F, &metacells::top_distinct<F>, "Collect the topmost distinct genes."); \
     module.def("fold_factor_dense_" #F, &metacells::fold_factor_dense<F>, "Fold factors of dense data.");
 
     REGISTER_F(float32_t)
     REGISTER_F(float64_t)
 
 #define REGISTER_F_I_P(F, I, P)                             \
     module.def("fold_factor_compressed_" #F "_" #I "_" #P,  \
                &metacells::fold_factor_compressed<F, I, P>, \
-               "Fold factors of compressed data.");
+               "Fold factors of compressed data.");         \
+    module.def("median_compressed_" #F "_" #I "_" #P,       \
+               &metacells::median_compressed<F, I, P>,      \
+               "Medians of compressed data.");
 
 #define REGISTER_FS_I_P(I, P)       \
     REGISTER_F_I_P(float32_t, I, P) \
     REGISTER_F_I_P(float64_t, I, P)
 
 #define REGISTER_FS_IS_P(P)      \
     REGISTER_FS_I_P(int8_t, P)   \
```

### Comparing `metacells-0.8.0/metacells/logistics.cpp` & `metacells-0.9.0/metacells/logistics.cpp`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/metacells/parameters.py` & `metacells-0.9.0/metacells/parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,185 +5,168 @@
 
 from math import sqrt
 from typing import Optional
 from typing import Union
 
 import metacells.utilities.typing as utt
 
-#: The generic random seed. The default of ``0`` makes for a different result each time the code is
-#: run. For reproducible results, provide a non-zero value, and also see
-#: :py:func:`metacells.parameters.reproducible`. Used by too many functions to list here.
-random_seed: int = 0
-
-#: Whether to make the results reproducible, possibly at the cost of some slowdown. For reproducible
-#: results, specify a ``True`` values, and also see :py:func:`metacells.parameters.random_seed`.
-#: Used by too many functions to list here.
-reproducible: bool = False
-
 #: The generic minimal "significant" gene fraction. See
 #: :py:func:`metacells.tools.high.find_high_fraction_genes`.
 significant_gene_fraction: float = 1e-5
 
 #: The generic minimal "significant" gene normalized variance. See
 #: :py:func:`metacells.tools.high.find_high_normalized_variance_genes`.
-significant_gene_normalized_variance: float = 2 ** 2.5
+significant_gene_normalized_variance: float = 2**2.5
 
 #: The generic minimal "significant" gene relative variance. See
 #: :py:func:`metacells.tools.high.find_high_relative_variance_genes`.
 significant_gene_relative_variance: float = 0.1
 
 #: The generic minimal "significant" gene similarity. See
-#: :py:const:`noisy_lonely_max_gene_similarity`
+#: :py:const:`bursty_lonely_max_gene_similarity`
 #: and
 #: :py:const:`rare_min_module_correlation`.
 significant_gene_similarity: float = 0.1
 
 #: The generic "significant" fold factor. See
 #: :py:const:`deviants_min_gene_fold_factor`
 #: and
 #: :py:const:`dissolve_min_convincing_gene_fold_factor`.
 significant_gene_fold_factor: float = 3.0
 
-#: Whether to use the absolute folds when considering fold factors. See
-#: :py:const:`deviants_abs_folds`,
-#: :py:const:`distinct_abs_folds`,
-#: :py:const:`inner_abs_folds`,
-#: :py:const:`outliers_abs_folds`,
-#: :py:const:`project_abs_folds`,
+#: The generic additional "significant" fold factor for noisy genes, in addition to
+#: :py:const:`significant_gene_fold_factor`. See
+#: :py:const:`deviants_min_gene_fold_factor`
 #: and
-#: :py:func:`inner_abs_folds`.
-abs_folds: bool = True
+#: :py:const:`dissolve_min_convincing_gene_fold_factor`.
+significant_noisy_gene_fold_factor: float = 2.0
 
 #: The generic minimal value (number of UMIs) we can say is "significant" given the technical noise. See
 #: :py:const:`rare_min_gene_maximum`,
 #: :py:const:`rare_min_cell_module_total`,
 #: and
-#: :py:const:`cells_similarity_value_normalization`.
+#: :py:const:`cells_similarity_value_regularization`.
 significant_value: int = 7
 
 #: The generic minimal samples to use for downsampling the cells for some purpose. See
-#: :py:const:`noisy_lonely_downsample_min_samples`,
-#: :py:const:`feature_downsample_min_samples`,
+#: :py:const:`bursty_lonely_downsample_min_samples`,
+#: :py:const:`select_downsample_min_samples`,
 #: and
 #: :py:func:`metacells.tools.downsample.downsample_cells`.
 downsample_min_samples: int = 750
 
 #: The generic minimal quantile of the cells total size to use for downsampling the cells for some
 #: purpose. See
-#: :py:const:`noisy_lonely_downsample_min_cell_quantile`,
-#: :py:const:`feature_downsample_min_cell_quantile`,
+#: :py:const:`bursty_lonely_downsample_min_cell_quantile`,
+#: :py:const:`select_downsample_min_cell_quantile`,
 #: and
 #: :py:func:`metacells.tools.downsample.downsample_cells`.
 downsample_min_cell_quantile: float = 0.05
 
 #: The generic maximal quantile of the cells total size to use for downsampling the cells for some
 #: purpose. See
-#: :py:const:`noisy_lonely_downsample_max_cell_quantile`,
-#: :py:const:`feature_downsample_max_cell_quantile`,
+#: :py:const:`bursty_lonely_downsample_max_cell_quantile`,
+#: :py:const:`select_downsample_max_cell_quantile`,
 #: and
 #: :py:func:`metacells.tools.downsample.downsample_cells`.
 downsample_max_cell_quantile: float = 0.5
 
 #: The window size to use to compute relative variance. See
 #: :py:func:`metacells.utilities.computation.relative_variance_per`
 #: and
 #: :py:func:`metacells.tools.high.find_high_relative_variance_genes`.
 relative_variance_window_size: int = 100
 
 #: The method to use to compute similarities. See
 #: :py:func:`metacells.tools.similarity.compute_obs_obs_similarity`,
 #: and
 #: :py:func:`metacells.tools.similarity.compute_var_var_similarity`.
-similarity_method: str = "pearson"
+similarity_method: str = "abs_pearson"
 
 #: The default location for the logistics function. See
-#: :py:func:`metacells.pipeline.umap.compute_umap_by_features`,
+#: :py:func:`metacells.pipeline.umap.compute_umap_by_markers`,
 #: :py:func:`metacells.tools.similarity.compute_obs_obs_similarity`,
 #: :py:func:`metacells.tools.similarity.compute_var_var_similarity`.
 #: and
 #: :py:func:`metacells.utilities.computation.logistics`.
 logistics_location: float = 0.8
 
 #: The default slope for the logistics function. See
-#: :py:func:`metacells.pipeline.umap.compute_umap_by_features`,
+#: :py:func:`metacells.pipeline.umap.compute_umap_by_markers`,
 #: :py:func:`metacells.tools.similarity.compute_obs_obs_similarity`,
 #: :py:func:`metacells.tools.similarity.compute_var_var_similarity`.
 #: and
 #: :py:func:`metacells.utilities.computation.logistics`.
 logistics_slope: float = 0.5
 
 #: The minimal target number of observations (cells) in a pile, allowing us to
 #: directly compute groups (metacells) for it. See
 #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
 #: and
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
-min_target_pile_size: int = 10000
+min_target_pile_size: int = 8000
 
 #: The maximal target number of observations (cells) in a pile, allowing us to
 #: directly compute groups (metacells) for it. See
 #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
 #: and
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
-max_target_pile_size: int = 30000
+max_target_pile_size: int = 32000
 
 #: The target number of metacells computed in each pile. See
 #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
 #: and
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
 target_metacells_in_pile: int = 100
 
-#: The generic target total metacell size. See
+#: The generic target total metacell size (by default, in cells). See
 #: :py:const:`candidates_target_metacell_size`,
 #: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
 #: and
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
-target_metacell_size: float = 160000
+target_metacell_size: float = 96
 
-#: The maximal cell size (total UMIs) to use. See
-#: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
-#: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`,
-#: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`
-#: and
-#: :py:func:`metacells.pipeline.collect.collect_metacells`.
-max_cell_size: Optional[float] = None
+#: Whether to use geometrical mean to compute metacell gene fractions.
+#: See :py:func:`metacells.pipeline.collect.collect_metacells`.
+metacell_geo_mean: bool = True
 
-#: The maximal cell size as a factor of the median cell size. See
-#: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
-#: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`,
-#: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`
-#: and
+#: The number of UMIs to use for regularization when computing metacell gene fractions geometrical mean.
+#: See :py:func:`metacells.pipeline.collect.collect_metacells`.
+metacell_umis_regularization: float = 1 / 16.0
+
+#: The quantile of the cell sizes to use for computing the number of zero-valued cells.
+#: See
 #: :py:func:`metacells.pipeline.collect.collect_metacells`.
-max_cell_size_factor: Optional[float] = 2.0
+zeros_cell_size_quantile: float = 0.1
 
 #: The genetic size of each cell for computing each metacell's size. See
 #: :py:const:`candidates_cell_sizes`,
 #: :py:const:`dissolve_cell_sizes`,
 #: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`
 #: and
 #: :py:func:`metacells.pipeline.collect.collect_metacells`.
-cell_sizes: Union[str, utt.Vector] = "__x__|sum"
+cell_sizes: Optional[Union[str, utt.Vector]] = None
 
 #: The generic maximal group size factor, above which we should split it. See
-#: :py:const:`pile_min_split_size_factor`
+#: :py:const:`piles_min_split_size_factor`
 #: and
 #: :py:const:`candidates_min_split_size_factor`.
 min_split_size_factor: float = 2.0
 
 #: The generic minimal group size factor, below which we should consider dissolving it. See
-#: :py:const:`pile_min_robust_size_factor`
+#: :py:const:`piles_min_robust_size_factor`
 #: and
 #: :py:const:`dissolve_min_robust_size_factor`.
 min_robust_size_factor: float = 0.5
 
 #: The generic maximal group size factor, below which we should merge it. See
-#: :py:const:`rare_min_modules_size_factor`,
-#: :py:const:`pile_max_merge_size_factor`,
+#: :py:const:`piles_max_merge_size_factor`,
 #: :py:const:`candidates_max_merge_size_factor`,
 #: and
 #: :py:const:`dissolve_min_convincing_size_factor`.
 max_merge_size_factor: float = 0.25
 
 #: The minimal number of cells in a metacell, below which we would merge it. See
 #: :py:const:`rare_min_cells_of_modules`,
@@ -203,180 +186,147 @@
 min_cut_seed_cells: int = 7
 
 #: The minimal size factor of a pile, above which we can split it. See
 #: :py:const:`min_split_size_factor`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
 #: and
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
-pile_min_split_size_factor: float = 1.25
+piles_min_split_size_factor: float = 1.25
 
 #: The minimal pile size factor, below which we should consider dissolving it. See
 #: :py:const:`min_robust_size_factor`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
 #: and
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
-pile_min_robust_size_factor: float = min_robust_size_factor
+piles_min_robust_size_factor: float = 0.3
 
 #: The maximal size factor of a pile, below which we should merge it. See
 #: :py:const:`min_robust_size_factor`,
 #: :py:const:`max_merge_size_factor`,
 #: :py:const:`dissolve_min_convincing_size_factor`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
 #: and
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
-pile_max_merge_size_factor: float = max_merge_size_factor
+piles_max_merge_size_factor: float = 0.15
 
 #: The minimal total value for a cell to be considered "properly sampled". See
 #: :py:func:`metacells.tools.properly_sampled.find_properly_sampled_cells`
 #: and
-#: :py:func:`metacells.pipeline.clean.extract_clean_data`.
+#: :py:func:`metacells.pipeline.exclude.extract_clean_data`.
 #:
 #: .. note::
 #:
 #:    There's no "reasonable" default value here. This must be tailored to the data.
 properly_sampled_min_cell_total: Optional[int] = None
 
 #: The maximal total value for a cell to be considered "properly sampled". See
 #: :py:func:`metacells.tools.properly_sampled.find_properly_sampled_cells`
 #: and
-#: :py:func:`metacells.pipeline.clean.extract_clean_data`.
+#: :py:func:`metacells.pipeline.exclude.extract_clean_data`.
 #:
 #: .. note::
 #:
 #:    There's no "reasonable" default value here. This must be tailored to the data.
 properly_sampled_max_cell_total: Optional[int] = None
 
 #: The minimal total value for a gene to be considered "properly sampled". See
 #: :py:func:`metacells.tools.properly_sampled.find_properly_sampled_genes`
 #: and
-#: :py:func:`metacells.pipeline.clean.extract_clean_data`.
+#: :py:func:`metacells.pipeline.exclude.extract_clean_data`.
 properly_sampled_min_gene_total: int = 1
 
 #: The maximal fraction of excluded gene UMIs from a cell for it to be considered
 #: "properly_sampled". See
 #: :py:func:`metacells.tools.properly_sampled.find_properly_sampled_cells`
 #: and
-#: :py:func:`metacells.pipeline.clean.extract_clean_data`.
+#: :py:func:`metacells.pipeline.exclude.extract_clean_data`.
 #:
 #: .. note::
 #:
 #:    There's no "reasonable" default value here. This must be tailored to the data.
 properly_sampled_max_excluded_genes_fraction: Optional[float] = None
 
 #: The number of randomly selected cells to use for computing related genes. See
-#: :py:func:`metacells.pipeline.related_genes.relate_genes`.
+#: :py:func:`metacells.pipeline.related_genes.relate_to_lateral_genes`.
 related_max_sampled_cells: int = 10000
 
 #: How to compute gene-gene similarity for computing the related genes. See
-#: :py:func:`metacells.pipeline.related_genes.relate_genes`.
-related_genes_similarity_method: str = "repeated_pearson"
+#: :py:func:`metacells.pipeline.related_genes.relate_to_lateral_genes`.
+related_genes_similarity_method: str = "abs_pearson"
 
 #: The hierarchical clustering method to use for computing the related genes. See
-#: :py:func:`metacells.pipeline.related_genes.relate_genes`.
+#: :py:func:`metacells.pipeline.related_genes.relate_to_lateral_genes`.
 related_genes_cluster_method: str = "ward"
 
-#: The minimal number of genes in a related gene module. See
-#: :py:func:`metacells.pipeline.related_genes.relate_genes`.
-related_min_genes_of_modules: int = 16
-
-#: The minimal samples to use for downsampling the cells for computing related genes. See
-#: :py:const:`downsample_min_samples`,
-#: :py:func:`metacells.tools.downsample.downsample_cells`,
-#: :py:func:`metacells.pipeline.feature.extract_feature_data`,
-#: and
-#: :py:func:`metacells.pipeline.related_genes.relate_genes`.
-related_downsample_min_samples: int = downsample_min_samples
-
-#: The minimal quantile of the cells total size to use for downsampling the cells for computing
-#: "feature" genes. See
-#: :py:const:`downsample_min_cell_quantile`,
-#: :py:func:`metacells.tools.downsample.downsample_cells`,
-#: :py:func:`metacells.pipeline.feature.extract_feature_data`,
-#: and
-#: :py:func:`metacells.pipeline.related_genes.relate_genes`.
-related_downsample_min_cell_quantile: float = downsample_min_cell_quantile
-
-#: The maximal quantile of the cells total size to use for downsampling the cells for computing
-#: "feature" genes. See
-#: :py:const:`downsample_max_cell_quantile`,
-#: :py:func:`metacells.tools.downsample.downsample_cells`,
-#: :py:func:`metacells.pipeline.feature.extract_feature_data`,
-#: and
-#: :py:func:`metacells.pipeline.related_genes.relate_genes`.
-related_downsample_max_cell_quantile: float = downsample_max_cell_quantile
-
-#: The minimal relative variance of a gene to be considered a "feature". See
-#: :py:func:`metacells.tools.high.find_high_relative_variance_genes`,
-#: :py:func:`metacells.pipeline.feature.extract_feature_data`,
-#: and
-#: :py:func:`metacells.pipeline.related_genes.relate_genes`.
-related_min_gene_relative_variance: float = 0.1
+#: The maximal number of genes in a related gene module. See
+#: :py:func:`metacells.pipeline.related_genes.relate_to_lateral_genes`.
+related_max_genes_of_modules: int = 64
 
-#: The minimal number of downsampled UMIs of a gene to be considered a "feature". See
-#: :py:func:`metacells.tools.high.find_high_total_genes`,
-#: :py:func:`metacells.pipeline.feature.extract_feature_data`,
-#: and
-#: :py:func:`metacells.pipeline.related_genes.relate_genes`.
-related_min_gene_total: int = 50
+#: The minimal mean fraction of a related gene. See
+#: :py:func:`metacells.pipeline.related_genes.relate_to_lateral_genes`.
+related_min_mean_gene_fraction: float = 1e-5
 
-#: The minimal number of the top-3rd downsampled UMIs of a gene to be considered a "feature". See
-#: :py:func:`metacells.tools.high.find_high_topN_genes`,
-#: :py:func:`metacells.pipeline.feature.extract_feature_data`,
-#: and
-#: :py:func:`metacells.pipeline.related_genes.relate_genes`.
-related_min_gene_top3: int = 1
+#: The minimal correlation of a related gene to the base gene(s). See
+#: :py:func:`metacells.pipeline.related_genes.relate_to_lateral_genes`.
+related_min_gene_correlation: float = 0.1
 
-#: The number of randomly selected cells to use for computing "noisy lonely" genes. See
-#: :py:func:`metacells.tools.noisy_lonely.find_noisy_lonely_genes`
+#: The number of randomly selected cells to use for computing "bursty lonely" genes. See
+#: :py:func:`metacells.tools.bursty_lonely.find_bursty_lonely_genes`
 #: and
-#: :py:func:`metacells.pipeline.clean.extract_clean_data`.
-noisy_lonely_max_sampled_cells: int = 10000
+#: :py:func:`metacells.pipeline.exclude.extract_clean_data`.
+bursty_lonely_max_sampled_cells: int = 10000
 
-#: The minimal samples to use for downsampling the cells for computing "noisy lonely" genes. See
+#: The minimal samples to use for downsampling the cells for computing "bursty lonely" genes. See
 #: :py:const:`downsample_min_cell_quantile`,
-#: :py:func:`metacells.tools.noisy_lonely.find_noisy_lonely_genes`,
+#: :py:func:`metacells.tools.bursty_lonely.find_bursty_lonely_genes`,
 #: and
-#: :py:func:`metacells.pipeline.clean.extract_clean_data`.
-noisy_lonely_downsample_min_samples: int = downsample_min_samples
+#: :py:func:`metacells.pipeline.exclude.extract_clean_data`.
+bursty_lonely_downsample_min_samples: int = downsample_min_samples
 
 #: The minimal quantile of the cells total size to use for downsampling the cells for computing
-#: "noisy lonely" genes. See
+#: "bursty lonely" genes. See
 #: :py:const:`downsample_min_cell_quantile`,
-#: :py:func:`metacells.tools.noisy_lonely.find_noisy_lonely_genes`,
+#: :py:func:`metacells.tools.bursty_lonely.find_bursty_lonely_genes`,
 #: and
-#: :py:func:`metacells.pipeline.clean.extract_clean_data`.
-noisy_lonely_downsample_min_cell_quantile: float = downsample_min_cell_quantile
+#: :py:func:`metacells.pipeline.exclude.extract_clean_data`.
+bursty_lonely_downsample_min_cell_quantile: float = downsample_min_cell_quantile
 
 #: The maximal quantile of the cells total size to use for downsampling the cells for computing
-#: "noisy lonely" genes. See
+#: "bursty lonely" genes. See
 #: :py:const:`downsample_min_cell_quantile`,
-#: :py:func:`metacells.tools.noisy_lonely.find_noisy_lonely_genes`,
+#: :py:func:`metacells.tools.bursty_lonely.find_bursty_lonely_genes`,
 #: and
-#: :py:func:`metacells.pipeline.clean.extract_clean_data`.
-noisy_lonely_downsample_max_cell_quantile: float = downsample_max_cell_quantile
+#: :py:func:`metacells.pipeline.exclude.extract_clean_data`.
+bursty_lonely_downsample_max_cell_quantile: float = downsample_max_cell_quantile
 
 #: The minimal total UMIs in the downsamples selected cells of a gene to be considered when
 #: computing "lonely" genes. See
-#: :py:func:`metacells.tools.noisy_lonely.find_noisy_lonely_genes` and
+#: :py:func:`metacells.tools.bursty_lonely.find_bursty_lonely_genes` and
 #: :py:func:`metacells.tools.high.find_high_total_genes`.
-noisy_lonely_min_gene_total: int = 100
+bursty_lonely_min_gene_total: int = 100
 
-#: The minimal normalized variance of a gene to be considered "noisy". See
+#: The minimal normalized variance of a gene to be considered "bursty". See
 #: :py:const:`significant_gene_normalized_variance`,
-#: :py:func:`metacells.tools.noisy_lonely.find_noisy_lonely_genes`
+#: :py:func:`metacells.tools.bursty_lonely.find_bursty_lonely_genes`
 #: and
-#: :py:func:`metacells.pipeline.clean.extract_clean_data`.
-noisy_lonely_min_gene_normalized_variance: float = significant_gene_normalized_variance
+#: :py:func:`metacells.pipeline.exclude.extract_clean_data`.
+bursty_lonely_min_gene_normalized_variance: float = significant_gene_normalized_variance
 
 #: The maximal similarity between a gene and another gene to be considered "lonely". See
 #: :py:const:`significant_gene_similarity`,
-#: :py:func:`metacells.tools.noisy_lonely.find_noisy_lonely_genes`
+#: :py:func:`metacells.tools.bursty_lonely.find_bursty_lonely_genes`
+#: and
+#: :py:func:`metacells.pipeline.exclude.extract_clean_data`.
+bursty_lonely_max_gene_similarity: float = significant_gene_similarity
+
+#: The maximal number of candidate rare genes. See
+#: :py:func:`metacells.tools.rare.find_rare_gene_modules`
 #: and
-#: :py:func:`metacells.pipeline.clean.extract_clean_data`.
-noisy_lonely_max_gene_similarity: float = significant_gene_similarity
+#: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
+rare_max_genes: int = 500
 
 #: The maximal fraction of the cells where a gene is expressed to be considered "rare". See
 #: :py:func:`metacells.tools.rare.find_rare_gene_modules`
 #: and
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
 rare_max_gene_cell_fraction: float = 1e-3
 
@@ -409,30 +359,22 @@
 #: The minimal number of cells in a rare gene module. See
 #: :py:const:`min_metacell_cells`,
 #: :py:func:`metacells.tools.rare.find_rare_gene_modules`
 #: and
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
 rare_min_cells_of_modules: int = min_metacell_cells
 
-#: The maximal mean number of cells (as a fraction of the mean metacell size) in a random pile for a rare gene module to
-#: be considered rare. See
+#: The maximal mean number of cells (as a fraction of the target metacell size) in a random pile for a rare gene module
+#: to be considered rare. See
 #: :py:const:`min_metacell_cells`,
 #: :py:func:`metacells.tools.rare.find_rare_gene_modules`
 #: and
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
 rare_max_cells_factor_of_random_pile: float = 0.5
 
-#: The minimal total UMIs of all the cells in a rare gene module (as a fraction
-#: of the :py:const:`target_metacell_size`). See
-#: :py:const:`max_merge_size_factor`,
-#: :py:func:`metacells.tools.rare.find_rare_gene_modules`
-#: and
-#: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
-rare_min_modules_size_factor: float = 0
-
 #: The minimal average correlation between the genes in a rare gene module. See
 #: :py:func:`metacells.parameters.significant_gene_similarity`,
 #: :py:func:`metacells.tools.rare.find_rare_gene_modules`
 #: and
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
 rare_min_module_correlation: float = significant_gene_similarity
 
@@ -453,88 +395,102 @@
 #: The minimal number of UMIs of a rare gene module in a cell to be considered as expressing the
 #: rare behavior. See
 #: :py:func:`metacells.tools.rare.find_rare_gene_modules`
 #: and
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
 rare_min_cell_module_total: int = int((significant_value + 1) / 2)
 
-#: The minimal samples to use for downsampling the cells for computing "feature" genes. See
+#: The maximal fraction of cells to mark as "deviants" in rare gene module piles. See
+#: :py:func:`metacells.tools.deviants.find_deviant_cells`,
+#: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
+#: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
+#: and
+#: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
+rare_deviants_max_cell_fraction: Optional[float] = 0.25
+
+#: Whether to compute metacells more quickly with lower quality. See
+#: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
+#: and
+#: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
+quick_and_dirty: bool = False
+
+#: The minimal samples to use for downsampling the cells for computing "select" genes. See
 #: :py:const:`downsample_min_samples`,
 #: :py:func:`metacells.tools.downsample.downsample_cells`,
-#: :py:func:`metacells.pipeline.feature.extract_feature_data`,
+#: :py:func:`metacells.pipeline.select.extract_selected_data`,
 #: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
 #: and
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
-feature_downsample_min_samples: int = downsample_min_samples
+select_downsample_min_samples: int = downsample_min_samples
 
 #: The minimal quantile of the cells total size to use for downsampling the cells for computing
-#: "feature" genes. See
+#: "select" genes. See
 #: :py:const:`downsample_min_cell_quantile`,
 #: :py:func:`metacells.tools.downsample.downsample_cells`,
-#: :py:func:`metacells.pipeline.feature.extract_feature_data`,
+#: :py:func:`metacells.pipeline.select.extract_selected_data`,
 #: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
 #: and
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
-feature_downsample_min_cell_quantile: float = downsample_min_cell_quantile
+select_downsample_min_cell_quantile: float = downsample_min_cell_quantile
 
 #: The maximal quantile of the cells total size to use for downsampling the cells for computing
-#: "feature" genes. See
+#: "select" genes. See
 #: :py:const:`downsample_max_cell_quantile`,
 #: :py:func:`metacells.tools.downsample.downsample_cells`,
-#: :py:func:`metacells.pipeline.feature.extract_feature_data`,
+#: :py:func:`metacells.pipeline.select.extract_selected_data`,
 #: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
 #: and
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
-feature_downsample_max_cell_quantile: float = downsample_max_cell_quantile
+select_downsample_max_cell_quantile: float = downsample_max_cell_quantile
 
-#: The minimal relative variance of a gene to be considered a "feature". See
+#: The minimal relative variance of a gene to be considered a "select". See
 #: :py:func:`metacells.tools.high.find_high_relative_variance_genes`,
-#: :py:func:`metacells.pipeline.feature.extract_feature_data`,
+#: :py:func:`metacells.pipeline.select.extract_selected_data`,
 #: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
 #: and
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
-feature_min_gene_relative_variance: Optional[float] = 0.1
+select_min_gene_relative_variance: Optional[float] = 0.1
 
-#: The minimal number of downsampled UMIs of a gene to be considered a "feature". See
+#: The minimal number of downsampled UMIs of a gene to be "select". See
 #: :py:func:`metacells.tools.high.find_high_total_genes`,
-#: :py:func:`metacells.pipeline.feature.extract_feature_data`,
+#: :py:func:`metacells.pipeline.select.extract_selected_data`,
 #: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
 #: and
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
-feature_min_gene_total: Optional[int] = 50
+select_min_gene_total: Optional[int] = 50
 
-#: The minimal number of the top-3rd downsampled UMIs of a gene to be considered a "feature". See
+#: The minimal number of the top-3rd downsampled UMIs of a gene to be "select". See
 #: :py:func:`metacells.tools.high.find_high_topN_genes`,
-#: :py:func:`metacells.pipeline.feature.extract_feature_data`,
+#: :py:func:`metacells.pipeline.select.extract_selected_data`,
 #: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
 #: and
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
-feature_min_gene_top3: Optional[int] = 4
+select_min_gene_top3: Optional[int] = 4
 
 #: Whether to compute cell-cell similarity using the log (base 2) of the data. See
 #: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
 #: and
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
 cells_similarity_log_data: bool = True
 
-#: The normalization factor to use if/when computing the fractions of the data for directly
+#: The regularization factor to use if/when computing the fractions of the data for directly
 #: computing the metacells. See
 #: :py:const:`significant_value`,
 #: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
 #: and
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
-cells_similarity_value_normalization: float = 1 / significant_value
+cells_similarity_value_regularization: float = 1 / significant_value
 
 #: The method to use to compute cell-cell similarity. See
 #: :py:func:`metacells.tools.similarity.compute_obs_obs_similarity`,
 #: :py:func:`metacells.pipeline.direct.compute_direct_metacells`
 #: and
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
 cells_similarity_method: str = similarity_method
@@ -552,18 +508,18 @@
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
 groups_similarity_method: str = similarity_method
 
 #: Whether to compute group self-similarity using the log (base 2) of the data. See
 #: :py:func:`metacells.pipeline.consistency.compute_groups_self_consistency`.
 self_similarity_log_data: bool = True
 
-#: The normalization factor to use after computing the fractions of the data for
+#: The regularization factor to use after computing the fractions of the data for
 #: computing group self similarity. See
 #: :py:func:`metacells.pipeline.consistency.compute_groups_self_consistency`.
-self_similarity_value_normalization: float = 1e-5
+self_similarity_value_regularization: float = 1e-5
 
 #: The method to use to compute group self-consistency. See
 #: :py:func:`metacells.tools.similarity.compute_obs_obs_similarity`,
 #: :py:func:`metacells.pipeline.consistency.compute_groups_self_consistency`.
 self_similarity_method: str = "logistics"
 
 #: The target K for building the K-Nearest-Neighbors graph. See
@@ -571,14 +527,38 @@
 #: :py:func:`metacells.tools.knn_graph.compute_var_var_knn_graph`,
 #: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
 #: and
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
 knn_k: Optional[int] = None
 
+#: The size of the default K for building the K-Nearest-Neighbors graph when computing metacells, multiplied
+#: by the median number of cells needed to reach the :py:const:`target_metacell_size`. See
+#: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
+#: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`,
+#: and
+#: :py:func:`metacells.pipeline.direct.compute_direct_metacells`.
+candidates_knn_k_size_factor: int = 2
+
+#: The size of the default K for building the K-Nearest-Neighbors graph when computing groups of metacells, multiplied
+#: by the median number of cells needed to reach the :py:const:`target_metacell_size`. See
+#: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
+#: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`,
+#: and
+#: :py:func:`metacells.pipeline.direct.compute_direct_metacells`.
+piles_knn_k_size_factor: int = 3
+
+#: The size of the default K for building the K-Nearest-Neighbors graph, based
+#: on the number of cells needed to reach the :py:const:`target_metacell_size` for a quantile of the cells. See
+#: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
+#: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`,
+#: and
+#: :py:func:`metacells.pipeline.direct.compute_direct_metacells`.
+knn_k_size_quantile: float = 0.1
+
 #: The minimal target K for building the K-Nearest-Neighbors graph. See
 #: :py:func:`metacells.tools.knn_graph.compute_obs_obs_knn_graph`,
 #: :py:func:`metacells.tools.knn_graph.compute_var_var_knn_graph`,
 #: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
 #: and
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
@@ -588,37 +568,37 @@
 #: K-Nearest-Neighbors graph. See
 #: :py:func:`metacells.tools.knn_graph.compute_obs_obs_knn_graph`,
 #: :py:func:`metacells.tools.knn_graph.compute_var_var_knn_graph`,
 #: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`
 #: and
-#: :py:func:`metacells.pipeline.umap.compute_umap_by_features`.
+#: :py:func:`metacells.pipeline.umap.compute_umap_by_markers`.
 knn_balanced_ranks_factor: float = sqrt(10)
 
 #: The factor of K of edges to keep when pruning the incoming edges of the K-Nearest-Neighbors
 #: graph. See
 #: :py:func:`metacells.tools.knn_graph.compute_obs_obs_knn_graph`,
 #: :py:func:`metacells.tools.knn_graph.compute_var_var_knn_graph`,
 #: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`
 #: and
-#: :py:func:`metacells.pipeline.umap.compute_umap_by_features`.
+#: :py:func:`metacells.pipeline.umap.compute_umap_by_markers`.
 knn_incoming_degree_factor: float = 3.0
 
 #: The factor of K of edges to keep when pruning the outgoing edges of the K-Nearest-Neighbors
 #: graph. See
 #: :py:func:`metacells.tools.knn_graph.compute_obs_obs_knn_graph`,
 #: :py:func:`metacells.tools.knn_graph.compute_var_var_knn_graph`,
 #: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`
 #: and
-#: :py:func:`metacells.pipeline.umap.compute_umap_by_features`.
+#: :py:func:`metacells.pipeline.umap.compute_umap_by_markers`.
 knn_outgoing_degree_factor: float = 1.0
 
 #: The minimal quantile of a seed to be selected. See
 #: :py:func:`metacells.tools.candidates.choose_seeds`,
 #: :py:func:`metacells.tools.candidates.compute_candidate_metacells`,
 #: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
@@ -669,15 +649,15 @@
 #: The size of each node for clustering the nodes of the K-Nearest-Neighbors graph. See
 #: :py:const:`cell_sizes`
 #: :py:func:`metacells.tools.candidates.compute_candidate_metacells`,
 #: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
 #: and
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
-candidates_cell_sizes: Union[str, utt.Vector] = cell_sizes
+candidates_cell_sizes: Optional[Union[str, utt.Vector]] = cell_sizes
 
 #: The minimal size factor of clusters to split when clustering the nodes of the
 #: K-Nearest-Neighbors graph. See
 #: :py:const:`min_split_size_factor`,
 #: :py:func:`metacells.tools.candidates.compute_candidate_metacells`,
 #: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
@@ -697,33 +677,86 @@
 
 #: The minimal number of cells in a metacell, below which we would merge it. See
 #: :py:const:`min_metacell_cells`
 #: and
 #: :py:func:`metacells.tools.candidates.compute_candidate_metacells`.
 candidates_min_metacell_cells: int = min_metacell_cells
 
-#: The maximal number of times to recursively collect and attempt to group outliers when computing
-#: the final metacells in the divide and conquer algorithm. See
-#: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`
+#: The policy to use for deciding which cell is "deviant". See
+#: :py:func:`metacells.tools.deviants.find_deviant_cells`,
+#: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
+#: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
+#: and
+#: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
+deviants_policy: str = "gaps"
+
+#: If using the ``gaps`` deviants policy, how many cells to skip ahead when computing gap sizes
+#: (``0``, ``1``, ``2``). See
+#: :py:func:`metacells.tools.deviants.find_deviant_cells`,
+#: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
+#: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
+#: and
+#: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
+deviants_gap_skip_cells: int = 1
+
+#: Do not mark deviants by a gene in a metacell if it causes more than this number of cells to become deviant
+#: (unless the count is no more than :py:const:`deviants_max_gap_cells_fraction`). See
+#: :py:func:`metacells.tools.deviants.find_deviant_cells`,
+#: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
+#: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
+#: and
+#: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
+deviants_max_gap_cells_count: int = 3
+
+#: Do not mark deviants by a gene in a metacell if it causes more than this fraction of cells to become deviant
+#: (unless the count is no more than :py:const:`deviants_max_gap_cells_count`). See
+#: :py:func:`metacells.tools.deviants.find_deviant_cells`,
+#: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
+#: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
+#: and
+#: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
+deviants_max_gap_cells_fraction: float = 0.1
+
+#: Use this quantile to pick the minimal cell size for the regularization factor when
+# computing deviants. See
+#: :py:func:`metacells.tools.deviants.find_deviant_cells`,
+#: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
+#: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
 #: and
-#: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`.
-final_max_outliers_levels: Optional[int] = 1
+#: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
+deviant_cells_regularization_quantile: float = 0.25
 
 #: The minimal fold factor for a gene to indicate a cell is "deviant". See
 #: :py:const:`significant_gene_fold_factor`,
 #: :py:func:`metacells.tools.deviants.find_deviant_cells`,
 #: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
 #: and
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
 deviants_min_gene_fold_factor: float = significant_gene_fold_factor
 
-#: Whether to consider the absolute fold factor when computing deviant cells. See
-#: :py:func:`metacells.tools.distinct.find_deviant_cells`.
-deviants_abs_folds: bool = False
+#: The minimal number of UMIs in the gene for two cells for using it as a certificate for a gap between
+#: the expression level of the gene in the cells for computinng deviants. See
+#: :py:const:`significant_gene_fold_factor`,
+#: :py:func:`metacells.tools.deviants.find_deviant_cells`,
+#: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
+#: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
+#: and
+#: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
+deviants_min_compare_umis: int = 8
+
+#: The minimal additional fold factor for a noisy gene to indicate a cell is "deviant",
+# in addition to :py:const:`deviants_min_gene_fold_factor`. See
+#: :py:const:`significant_gene_fold_factor`,
+#: :py:func:`metacells.tools.deviants.find_deviant_cells`,
+#: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
+#: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
+#: and
+#: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
+deviants_min_noisy_gene_fold_factor: float = significant_noisy_gene_fold_factor
 
 #: The maximal fraction of genes to use to indicate cell are "deviants". See
 #: :py:func:`metacells.tools.deviants.find_deviant_cells`,
 #: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
 #: and
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
@@ -740,15 +773,15 @@
 #: The size of each cell for for dissolving too-small metacells. See
 #: :py:const:`cell_sizes`,
 #: :py:func:`metacells.tools.dissolve.dissolve_metacells`,
 #: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
 #: and
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
-dissolve_cell_sizes: Union[str, utt.Vector] = cell_sizes
+dissolve_cell_sizes: Optional[Union[str, utt.Vector]] = cell_sizes
 
 #: The minimal size factor for a metacell to be considered "robust". See
 #: :py:const:`min_robust_size_factor`
 #: :py:func:`metacells.tools.dissolve.dissolve_metacells`,
 #: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
 #: and
@@ -775,15 +808,15 @@
 #: The minimal size factor for a metacell to be kept if it is "convincing". See
 #: :py:const:`max_merge_size_factor`
 #: :py:func:`metacells.tools.dissolve.dissolve_metacells`,
 #: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
 #: and
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
-dissolve_min_convincing_size_factor: Optional[float] = max_merge_size_factor
+dissolve_min_convincing_size_factor: Optional[float] = 0.125
 
 #: The minimal size factor for a metacell to be kept if it is "convincing" when grouping rare gene
 #: module cells. See
 #: :py:const:`max_merge_size_factor`
 #: :py:func:`metacells.tools.dissolve.dissolve_metacells`,
 #: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
@@ -796,240 +829,223 @@
 #: :py:func:`metacells.tools.dissolve.dissolve_metacells`,
 #: :py:func:`metacells.pipeline.direct.compute_direct_metacells`,
 #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`
 #: and
 #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`.
 dissolve_min_convincing_gene_fold_factor: float = significant_gene_fold_factor
 
-#: Whether to consider the absolute fold factor when dissolving metacells. See
-#: :py:func:`metacells.tools.distinct.dissolve_metacells`.
-dissolve_abs_folds: bool = False
-
 #: The number of most-distinct genes to collect for each cell. See
 #: :py:func:`metacells.tools.distinct.find_distinct_genes`.
 distinct_genes_count: int = 20
 
-#: Whether to consider the absolute fold factor when collecting most-distinct genes for each cell. See
-#: :py:func:`metacells.tools.distinct.find_distinct_genes`.
-distinct_abs_folds: bool = abs_folds
+#: The maximal number of marker genes to use for UMAP.
+#: See
+#: :py:func:`metacells.pipeline.umap.compute_knn_by_markers` and
+#: :py:func:`metacells.pipeline.umap.compute_umap_by_markers`.
+umap_max_marker_genes: int = 1000
 
-#: The normalization factor to use if/when computing the fractions of the data for UMAP.
+#: Whether to ignore lateral genes when computing the UMAP.
 #: See
-#: :py:const:`metacells.parameters.target_metacell_size`
+#: :py:func:`metacells.pipeline.umap.compute_knn_by_markers` and
+#: :py:func:`metacells.pipeline.umap.compute_umap_by_markers`.
+umap_ignore_lateral_genes: bool = True
+
+#: The regularization factor to use if/when computing the fractions of the data for UMAP.
+#: See
+#: :py:const:`metacells.parameters.significant_gene_fraction`
 #: and
-#: :py:func:`metacells.pipeline.umap.compute_umap_by_features`.
-umap_similarity_value_normalization: float = 1 / target_metacell_size
+#: :py:func:`metacells.pipeline.umap.compute_umap_by_markers`.
+umap_similarity_value_regularization: float = significant_gene_fraction
 
 #: Whether to compute metacell-metacell similarity using the log (base 2) of the data for UMAP. See
-#: :py:func:`metacells.pipeline.umap.compute_umap_by_features`.
+#: :py:func:`metacells.pipeline.umap.compute_umap_by_markers`.
 umap_similarity_log_data: bool = True
 
 #: The method to use to compute similarities for UMAP. See
 #: :py:func:`metacells.tools.similarity.compute_obs_obs_similarity`,
 #: :py:func:`metacells.tools.similarity.compute_var_var_similarity`,
 #: and
-#: :py:func:`metacells.pipeline.umap.compute_umap_by_features`.
-umap_similarity_method: str = "logistics_pearson"
+#: :py:func:`metacells.pipeline.umap.compute_umap_by_markers`.
+umap_similarity_method: str = "logistics_abs_pearson"
 
 #: The minimal UMAP point distance. See :py:const:`umap_spread` and
 #: :py:func:`metacells.tools.layout.umap_by_distances`
 #: and
-#: :py:func:`metacells.pipeline.umap.compute_umap_by_features`.
+#: :py:func:`metacells.pipeline.umap.compute_umap_by_markers`.
 umap_min_dist: float = 0.5
 
 #: The minimal UMAP spread. This is automatically raised if the :py:const:`umap_min_dist` is higher.
 #: See :py:func:`metacells.tools.layout.umap_by_distances`
 #: and
-#: :py:func:`metacells.pipeline.umap.compute_umap_by_features`.
+#: :py:func:`metacells.pipeline.umap.compute_umap_by_markers`.
 umap_spread: float = 1.0
 
 #: The UMAP KNN graph degree. See
 #: :py:func:`metacells.tools.layout.umap_by_distances`
 #: and
-#: :py:func:`metacells.pipeline.umap.compute_umap_by_features`.
+#: :py:func:`metacells.pipeline.umap.compute_umap_by_markers`.
 umap_k: int = 15
 
 #: The UMAP KNN skeleton graph degree. See
 #: :py:func:`metacells.tools.knn_graph.compute_obs_obs_knn_graph`,
 #: :py:func:`metacells.tools.knn_graph.compute_var_var_knn_graph`,
 #: and
-#: :py:func:`metacells.pipeline.umap.compute_umap_by_features`.
+#: :py:func:`metacells.pipeline.umap.compute_umap_by_markers`.
 skeleton_k: int = 4
 
-#: The maximal number of top feature genes to pick.
-#: See :py:func:`metacells.tools.high.find_top_feature_genes`
-#: and
-#: :py:func:`metacells.pipeline.umap.compute_umap_by_features`.
-max_top_feature_genes: int = 1000
-
 #: The value to add to gene fractions before applying the log function. See
-#: See :py:func:`metacells.pipeline.umap.compute_umap_by_features`.
-umap_fraction_normalization: float = 1e-5
+#: See :py:func:`metacells.pipeline.umap.compute_umap_by_markers`.
+umap_fraction_regularization: float = 1e-5
 
 #: The fraction of the UMAP plot area to cover with points. See
 #: :py:func:`metacells.utilities.computation.cover_diameter`,
 #: :py:func:`metacells.utilities.computation.cover_coordinates`
 #: and
 #: :py:func:`metacells.tools.layout.umap_by_distances`,
-cover_fraction: float = 1 / 3.0
+spread_cover_fraction: float = 1 / 3.0
 
 #: The noise to add to the UMAP plot area. See
 #: :py:func:`metacells.utilities.computation.cover_coordinates`
 #: and
 #: :py:func:`metacells.tools.layout.umap_by_distances`,
-noise_fraction: float = 0.1
+spread_noise_fraction: float = 0.1
 
 #: The minimal total number of UMIs for a gene to compute meaningful quality statistics for it.
-#: See :py:func:`metacells.tools.quality.compute_inner_normalized_variance`.
+#: See :py:func:`metacells.tools.quality.compute_stdev_logs`,
+#: :py:func:`metacells.tools.quality.compute_inner_folds`, and
+#: :py:func:`metacells.tools.quality.compute_outliers_fold_factors`.
 quality_min_gene_total: int = 40
 
 #: The maximal amount of memory to use when guessing the number of parallel piles. If zero or
 #: negative, is the fraction of the machine's total RAM to use as a safety buffer. See
 #: :py:func:`metacells.pipeline.divide_and_conquer.guess_max_parallel_piles`.
 max_gbs: float = -0.1
 
-#: Whether to compute projections based on the log of the data instead of the data itself. See
-#: :py:func:`metacells.tools.project.project_query_onto_atlas`.
-project_log_data: bool = True
+#: Whether the projection will ignore genes where the ranges of the corrected vs. the projected expression is too low.
+#: See :py:func:`metacells.pipeline.projection.projection_pipeline`.
+project_filter_ranges: bool = True
+
+#: The quantile to use (on both low and high ends) to compute the range of expression of a corrected of a projected
+#: gene. See :py:func:`metacells.pipeline.projection.projection_pipeline`.
+project_ignore_range_quantile: float = 0.02
+
+#: The minimal overlap (shared range divided by query range) for genes to keep projecting. See
+#: :py:func:`metacells.pipeline.projection.projection_pipeline`.
+project_ignore_range_min_overlap_fraction: float = 0.5
 
-#: The normalization factor to use when computing fold factors for projecting a query onto an atlas. See
-#: :py:func:`metacells.tools.project.project_query_onto_atlas`.
-project_fold_normalization: float = 1e-5
+#: The minimal fraction of the query marker genes that are fitted for a query metacell to be considered "similar" to the
+#: atlas. See :py:func:`metacells.pipeline.projection.projection_pipeline`.
+project_min_query_markers_fraction: float = 1 / 3
+
+#: The regularization factor to use when computing fold factors for projecting a query onto an atlas. See
+#: :py:func:`metacells.tools.project.compute_projection_weights`.
+project_fold_regularization: float = 1e-5
 
 #: The minimal number of UMIs for a gene to be a potential cause to mark a metacell as dissimilar. See
-#: :py:func:`metacells.tools.project.project_query_onto_atlas`.
-project_min_significant_gene_value: float = 40
+#: :py:func:`metacells.tools.project.compute_projection_weights`.
+project_min_significant_gene_umis: int = 40
 
 #: The number of atlas candidates to consider when projecting a query onto an atlas. See
-#: :py:func:`metacells.tools.project.project_query_onto_atlas`.
+#: :py:func:`metacells.tools.project.compute_projection_weights`.
 project_candidates_count: int = 50
 
+#: The minimal number of atlas candidates to use even if they fail the consistency check as a fraction of
+#: :py:const:`project_candidates_count`. See
+#: :py:func:`metacells.tools.project.compute_projection_weights`.
+project_min_candidates_fraction: float = 1.0 / 3.0
+
 #: The minimal weight of an atlas metacell used for the projection of a query metacell. See
-#: :py:func:`metacells.tools.project.project_query_onto_atlas`.
+#: :py:func:`metacells.tools.project.compute_projection_weights`.
 project_min_usage_weight: float = 1e-5
 
 #: The maximal fold factor of genes between the projection and the query metacell. See
-#: :py:func:`metacells.tools.project.project_query_onto_atlas`.
+#: :py:func:`metacells.tools.project.compute_projection_weights`.
 project_max_projection_fold_factor: float = significant_gene_fold_factor
 
-#: Whether to consider the absolute fold factor when evaluating the projection of the query metacells . See
-#: :py:func:`metacells.tools.project.project_query_onto_atlas`.
-project_abs_folds: bool = abs_folds
+#: The maximal additional fold factor of noisy genes between the projection and the query metacell,
+# in addition to :py:const:`project_max_projection_fold_factor`. See
+#: :py:func:`metacells.tools.project.compute_projection_weights`.
+project_max_projection_noisy_fold_factor: float = significant_noisy_gene_fold_factor
 
 #: The maximal fold factor of genes between the atlas metacells used for the projection of a query metacell. See
-#: :py:func:`metacells.tools.project.project_query_onto_atlas`.
+#: :py:func:`metacells.tools.project.compute_projection_weights`.
 project_max_consistency_fold_factor: float = significant_gene_fold_factor - 1.0
 
-#: The minimal fold factor for a gene to be significant for metacell quality. See
-#: :py:func:`metacell.tools.compute_inner_fold_factors`.
-min_gene_inner_fold_factor: float = significant_gene_fold_factor
-
-#: The minimal fold factor for a gene entry in a metacell to be significant for metacell quality. See
-#: :py:func:`metacell.tools.compute_inner_fold_factors`.
-min_entry_inner_fold_factor: float = significant_gene_fold_factor - 1.0
-
-#: Whether to consider the absolute fold factor when evaluating the inner folds. See
-#: :py:func:`metacells.tools.distinct.compute_inner_fold_factors`.
-inner_abs_folds: bool = abs_folds
-
-#: The minimal fold factor for a gene to be significant for outliers. See
-#: :py:func:`metacell.tools.compute_outliers_fold_factors`.
-min_gene_outliers_fold_factor: float = significant_gene_fold_factor
-
-#: The minimal fold factor for a gene entry in a metacell to be significant for outliers. See
-#: :py:func:`metacell.tools.compute_outliers_fold_factors`.
-min_entry_outliers_fold_factor: float = significant_gene_fold_factor - 1.0
-
-#: Whether to consider the absolute fold factor when evaluating the outliers folds. See
-#: :py:func:`metacells.tools.distinct.compute_outliers_fold_factors`.
-outliers_abs_folds: bool = abs_folds
-
-#: The minimal fold factor for a gene entry in a metacell to be significant for metacell projection quality. See
-#: :py:func:`metacell.tools.compute_project_fold_factors`.
-min_entry_project_fold_factor: float = significant_gene_fold_factor - 1.0
+#: Whether to compute projectio the log (base 2) of the data. See
+#: :py:func:`metacells.tools.project.compute_projection_weights`.
+project_log_data: bool = True
 
-#: The normalization factor to use when computing log of fractions for finding the most similar group for outliers. See
+#: The regularization factor to use when computing log of fractions for finding the most similar group for outliers. See
 #: :py:func:`metacells.tools.quality.compute_outliers_matches`.
-outliers_fold_normalization: float = 1e-5
+outliers_fold_regularization: float = 1e-5
+
+#: Whether to ignore the lateral genes of the atlas when computing projections. See
+#: :py:func:`metacells.pipeline.projection.projection_pipeline`.
+ignore_atlas_lateral_genes: bool = True
+
+#: Whether to ignore the noisy genes of the atlas when computing projections. See
+#: :py:func:`metacells.pipeline.projection.projection_pipeline`.
+consider_atlas_noisy_genes: bool = True
+
+#: Whether to ignore the non-marker genes of the atlas when computing projections. See
+#: :py:func:`metacells.pipeline.projection.projection_pipeline`.
+only_atlas_marker_genes: bool = True
+
+#: Whether to ignore the non-marker genes of the query when computing projections. See
+#: :py:func:`metacells.pipeline.projection.projection_pipeline`.
+only_query_marker_genes: bool = False
 
-#: Whether to ignore the forbidden genes of the atlas when computing projections. See
-#: :py:func:`metacells.pipeline.projection.direct_projection_pipeline`
-#: and :py:func:`metacells.pipeline.projection.projection_pipeline`.
-ignore_atlas_forbidden_genes: bool = True
-
-#: Whether to ignore the insignificant genes of the atlas when computing projections. See
-#: :py:func:`metacells.pipeline.projection.direct_projection_pipeline`
-#: and :py:func:`metacells.pipeline.projection.projection_pipeline`.
-ignore_atlas_insignificant_genes: bool = True
-
-#: Whether to ignore the insignificant genes of the query when computing projections. See
-#: :py:func:`metacells.pipeline.projection.direct_projection_pipeline`
-#: and :py:func:`metacells.pipeline.projection.projection_pipeline`.
-ignore_query_insignificant_genes: bool = False
-
-#: Whether to ignore the forbidden genes of the query when computing projections. See
-#: :py:func:`metacells.pipeline.projection.direct_projection_pipeline`
-#: and :py:func:`metacells.pipeline.projection.projection_pipeline`.
-ignore_query_forbidden_genes: bool = False
-
-#: The quantile of the gene value to use for the query gene expressions when looking for systematic genes. See
-#: :py:func:`metacells.tools.project.find_systematic_genes`,
-#: :py:func:`metacells.pipeline.projection.direct_projection_pipeline`
-#: and :py:func:`metacells.pipeline.projection.projection_pipeline`.
-systematic_low_gene_quantile: float = 0.05
-
-#: The quantile of the gene value to use for the atlas gene expressions when looking for systematic genes. See
-#: :py:func:`metacells.tools.project.find_systematic_genes`
-#: :py:func:`metacells.pipeline.projection.direct_projection_pipeline`
-#: and :py:func:`metacells.pipeline.projection.projection_pipeline`.
-systematic_high_gene_quantile: float = 0.95
-
-#: The minimal fraction of metacells where a gene has a high projection fold factor to mark the gene as biased.
-#: See :py:func:`metacells.tools.project.find_biased_genes`,
-#: :py:func:`metacells.pipeline.projection.direct_projection_pipeline`
-#: and :py:func:`metacells.pipeline.projection.projection_pipeline`.
-biased_min_metacells_fraction: float = 0.5
-
-#: The minimal fold between the maximal and minimal gene expression in metacells to be significant.
-#: See :py:func:`metacells.tools.high.find_significant_metacells_genes`.
-min_significant_metacells_gene_range_fold_factor: float = 2.0
+#: Whether to ignore the lateral genes of the query when computing projections. See
+#: :py:func:`metacells.pipeline.projection.projection_pipeline`.
+ignore_query_lateral_genes: bool = True
 
-#: The normalization factor to use after computing the fractions of the data for
+#: Whether to ignore the noisy genes of the query when computing projections. See
+#: :py:func:`metacells.pipeline.projection.projection_pipeline`.
+consider_query_noisy_genes: bool = True
+
+#: The minimal fraction of metacells where a gene has a high projection fold factor to mark the gene as "misfit".
+#: See :py:func:`metacells.pipeline.projection.projection_pipeline`.
+misfit_min_metacells_fraction: float = 0.5
+
+#: The minimal fold between the maximal and minimal gene expression in metacells to be a "marker".
+#: See :py:func:`metacells.tools.high.find_metacells_marker_genes`.
+min_marker_metacells_gene_range_fold_factor: float = 2.0
+
+#: The regularization factor to use after computing the fractions of the data for
 #: computing metacell gene range folds. See
-#: :py:func:`metacells.tools.high.find_significant_metacells_genes`.
-metacells_gene_range_normalization: float = 1e-5
+#: :py:func:`metacells.tools.high.find_metacells_marker_genes`.
+metacells_gene_range_regularization: float = 1e-5
 
-#: The minimal maximal gene expression in metacells to be significant.
-#: See :py:func:`metacells.tools.high.find_significant_metacells_genes`.
-min_significant_metacells_gene_fraction: float = 1e-4
+#: The minimal maximal gene expression in metacells to be a "marker".
+#: See :py:func:`metacells.tools.high.find_metacells_marker_genes`.
+min_marker_max_metacells_gene_fraction: float = 1e-4
 
 #: Whether to renormalize the query to account for missing atlas genes when computing projections.
-#: See :py:func:`metacells.pipeline.projection.direct_projection_pipeline`
-#: and :py:func:`metacells.pipeline.projection.projection_pipeline`.
+#: :py:func:`metacells.pipeline.projection.projection_pipeline`.
 project_renormalize_query: bool = False
 
-#: The minimal correlation between observed and projected genes for considering linear correction of the query gene
-#: value.
+#: Whether to compute linear corrections for genes between the query and the atlas.
 #: See :py:func:`metacells.pipeline.projection.projection_pipeline`.
+project_corrections: bool = False
+
+#: The minimal correlation between observed and projected genes for considering linear correction of the query gene
+#: value. See :py:func:`metacells.pipeline.projection.projection_pipeline`.
 project_min_corrected_gene_correlation: float = 0.8
 
 #: The minimal strength of the correction between the mean query and projected mean value (for correlated genes).
 #: See :py:func:`metacells.pipeline.projection.projection_pipeline`.
 project_min_corrected_gene_factor: float = 0.15
 
-#: The m aximal correlation between observed and projected genes for ignoring the gene as uncorrelated.
-#: See :py:func:`metacells.pipeline.projection.projection_pipeline`.
-project_max_uncorrelated_gene_correlation: float = 0.5
-
 #: The maximal number of deviant genes allowed for saying a query is similar to the projection in the atlas.
 #: See :py:func:`metacells.tools.quality.compute_similar_query_metacells`
 # and :py:func:`metacells.pipeline.projection.projection_pipeline`.
-project_max_dissimilar_genes: int = 3
-
-#: Whether to add a pseudo-gene to the query to renormalize its total UMIs so that the fractions of the common genes
-#: would be as expected. See :py:func:`metacells.tools.project.renormalize_query_by_atlas` and
-#: :py:func:`metacells.pipeline.projection.projection_pipeline`.
-renormalize_query_by_atlas: bool = True
+project_max_misfit_genes: int = 3
 
 #: The quantile of each gene's normalized variance across the metacells to use for the overall gene's variability.
-#: See :py:func:`metacells.tools.quality.compute_type_gene_normalized_variance`.
+#: See :py:func:`metacells.tools.quality.compute_type_genes_normalized_variances`.
 type_gene_normalized_variance_quantile: float = 0.95
+
+#: Minimal fraction of atlas essential genes required for saying a query is similar to the projection in the
+#: atlas.
+#: See :py:func:`metacells.tools.quality.compute_similar_query_metacells`
+# and :py:func:`metacells.pipeline.projection.projection_pipeline`.
+project_min_essential_genes_fraction: float = 0.75
```

### Comparing `metacells-0.8.0/metacells/partitions.cpp` & `metacells-0.9.0/metacells/partitions.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,44 @@
 #include "metacells/extensions.h"
 
 namespace metacells {
 
+static float64_t
+mass_factor(float64_t mass, float64_t low_mass, float64_t target_mass, float64_t high_mass) {
+    const float64_t inner_slope = 0.02;
+    const float64_t outer_slope = 0.5;
+    if (mass < low_mass) {
+        return log2((1 - inner_slope) * low_mass / (low_mass + (1 / (1 - outer_slope) - 1) * (low_mass - mass)));
+    }
+    if (mass < target_mass) {
+        return log2(1 - inner_slope * (target_mass - mass) / (target_mass - low_mass));
+    }
+    if (mass < high_mass) {
+        return log2(1 - inner_slope * (mass - target_mass) / (high_mass - target_mass));
+    }
+    return log2((1 - inner_slope) * low_mass / (low_mass + (1 / (1 - outer_slope) - 1) * (mass - high_mass)));
+}
+
+struct CandidatePartitions {
+    std::vector<size_t>& connectivity_partitions;
+    std::vector<size_t>& goal_partitions;
+    std::vector<size_t>& both_partitions;
+
+    CandidatePartitions(TmpVectorSizeT& raii, size_t partitions_count)
+      : connectivity_partitions(raii.vector(partitions_count))
+      , goal_partitions(raii.vector(partitions_count))
+      , both_partitions(raii.vector(partitions_count)) {}
+
+    void clear() {
+        connectivity_partitions.clear();
+        goal_partitions.clear();
+        both_partitions.clear();
+    }
+};
+
 // Score information for one node for one partition.
 struct NodeScore {
 private:
     float64_t m_total_outgoing_weights;
     float64_t m_total_incoming_weights;
     float64_t m_score;
 
@@ -22,26 +55,28 @@
     void update_incoming(const int direction, const float64_t edge_weight) {
         m_total_incoming_weights += direction * edge_weight;
         SlowAssertCompare(m_total_incoming_weights, >=, -EPSILON);
         m_total_incoming_weights = std::max(m_total_incoming_weights, 0.0);
         m_score = NaN;
     }
 
+    int connectivity() const { return int(m_total_outgoing_weights > EPSILON) + int(m_total_incoming_weights > 0); }
+
     float64_t total_outgoing_weights() const { return m_total_outgoing_weights; }
 
     float64_t total_incoming_weights() const { return m_total_incoming_weights; }
 
     float64_t score() const {
         SlowAssertCompare(std::isnan(m_score), ==, false);
         return m_score;
     }
 
     float64_t rescore() {
         SlowAssertCompare(m_total_outgoing_weights, >=, 0);
-        SlowAssertCompare(m_total_outgoing_weights, <=, 1 + EPSILON);
+        SlowAssertCompare(m_total_outgoing_weights, <, 1 + EPSILON);
         SlowAssertCompare(m_total_incoming_weights, >=, 0);
         m_score = log2(EPSILON + m_total_outgoing_weights * m_total_incoming_weights) / 2.0;
         return m_score;
     }
 };
 
 static std::ostream&
@@ -51,17 +86,15 @@
 }
 
 static std::vector<size_t>
 initial_size_of_partitions(ConstArraySlice<int32_t> partitions_of_nodes) {
     std::vector<size_t> size_of_partitions;
 
     for (int32_t partition_index : partitions_of_nodes) {
-        if (partition_index < 0) {
-            continue;
-        }
+        FastAssertCompare(partition_index, >=, 0);
         if (size_t(partition_index) >= size_of_partitions.size()) {
             size_of_partitions.resize(partition_index + 1);
         }
         ++size_of_partitions[partition_index];
     }
 
     for (size_t partition_index = 0; partition_index < size_of_partitions.size(); ++partition_index) {
@@ -134,27 +167,23 @@
                 << " from node_index: " << node_index                //
                 << " from partition_index: " << partition_index      //
                 << " to_node_index: " << other_node_index            //
                 << " to_partition_index: " << other_partition_index  //
                 << " edge weight: " << edge_weight                   //
                 << std::endl;
 
-            if (other_partition_index >= 0) {
-                score_of_nodes_of_partitions[other_partition_index][node_index].update_outgoing(+1, edge_weight);
-                score_of_nodes_of_partitions[other_partition_index][node_index].rescore();
-            }
+            score_of_nodes_of_partitions[other_partition_index][node_index].update_outgoing(+1, edge_weight);
+            score_of_nodes_of_partitions[other_partition_index][node_index].rescore();
 
-            if (partition_index >= 0) {
-                score_of_nodes_of_partitions[partition_index][other_node_index].update_incoming(+1, edge_weight);
-                score_of_nodes_of_partitions[partition_index][other_node_index].rescore();
-            }
+            score_of_nodes_of_partitions[partition_index][other_node_index].update_incoming(+1, edge_weight);
+            score_of_nodes_of_partitions[partition_index][other_node_index].rescore();
         }
 
 #if ASSERT_LEVEL > 0
-        FastAssertCompare(total_outgoing_weights, >, 1 - EPSILON);
+        FastAssertCompare(total_outgoing_weights, >=, 1 - EPSILON);
         FastAssertCompare(total_outgoing_weights, <, 1 + EPSILON);
 #endif
     }
 
     for (size_t node_index = 0; node_index < nodes_count; ++node_index) {
         for (size_t partition_index = 0; partition_index < partitions_count; ++partition_index) {
             if (int32_t(partition_index) == partition_of_nodes[node_index]) {
@@ -181,99 +210,113 @@
                             ConstArraySlice<int32_t> partitions_of_nodes,
                             const size_t partitions_count,
                             const std::vector<std::vector<NodeScore>>& score_of_nodes_of_partitions) {
     std::vector<float64_t> score_of_partitions(partitions_count, 0);
 
     for (size_t node_index = 0; node_index < nodes_count; ++node_index) {
         const int partition_index = partitions_of_nodes[node_index];
-        if (partition_index >= 0) {
-            score_of_partitions[partition_index] += score_of_nodes_of_partitions[partition_index][node_index].score();
-        }
+        score_of_partitions[partition_index] += score_of_nodes_of_partitions[partition_index][node_index].score();
     }
 
     return score_of_partitions;
 }
 
+static std::vector<float64_t>
+initial_mass_of_partitions(size_t nodes_count,
+                           ConstArraySlice<int32_t> partitions_of_nodes,
+                           const size_t partitions_count,
+                           ConstArraySlice<float32_t> mass_of_nodes) {
+    std::vector<float64_t> mass_of_partitions(partitions_count, 0);
+
+    for (size_t node_index = 0; node_index < nodes_count; ++node_index) {
+        const int partition_index = partitions_of_nodes[node_index];
+        mass_of_partitions[partition_index] += mass_of_nodes[node_index];
+    }
+
+    return mass_of_partitions;
+}
+
 #if ASSERT_LEVEL > 0
 std::function<void()> g_verify;
 #endif
 
 // Optimize the partition of a graph.
 struct OptimizePartitions {
     ConstCompressedMatrix<float32_t, int32_t, int32_t> outgoing_weights;
     ConstCompressedMatrix<float32_t, int32_t, int32_t> incoming_weights;
     const size_t nodes_count;
+    float64_t low_mass;
+    float64_t target_mass;
+    float64_t high_mass;
+    ConstArraySlice<float32_t> mass_of_nodes;
     ArraySlice<int32_t> partition_of_nodes;
     std::vector<float64_t> temperature_of_nodes;
     std::vector<size_t> size_of_partitions;
     const size_t partitions_count;
     float64_t incoming_scale;
     std::vector<std::vector<NodeScore>> score_of_nodes_of_partitions;
+    std::vector<float64_t> mass_of_partitions;
     std::vector<float64_t> score_of_partitions;
 
     OptimizePartitions(const pybind11::array_t<float32_t>& outgoing_weights_array,
                        const pybind11::array_t<int32_t>& outgoing_indices_array,
                        const pybind11::array_t<int32_t>& outgoing_indptr_array,
                        const pybind11::array_t<float32_t>& incoming_weights_array,
                        const pybind11::array_t<int32_t>& incoming_indices_array,
                        const pybind11::array_t<int32_t>& incoming_indptr_array,
+                       const float64_t low_mass,
+                       const float64_t target_mass,
+                       const float64_t high_mass,
+                       const pybind11::array_t<float32_t>& mass_of_nodes_array,
                        pybind11::array_t<int32_t>& partition_of_nodes_array)
       : outgoing_weights(ConstCompressedMatrix<float32_t, int32_t, int32_t>(
           ConstArraySlice<float32_t>(outgoing_weights_array, "outgoing_weights_array"),
           ConstArraySlice<int32_t>(outgoing_indices_array, "outgoing_indices_array"),
           ConstArraySlice<int32_t>(outgoing_indptr_array, "outgoing_indptr_array"),
           int32_t(outgoing_indptr_array.size() - 1),
           "outgoing_weights"))
       , incoming_weights(ConstCompressedMatrix<float32_t, int32_t, int32_t>(
             ConstArraySlice<float32_t>(incoming_weights_array, "incoming_weights_array"),
             ConstArraySlice<int32_t>(incoming_indices_array, "incoming_indices_array"),
             ConstArraySlice<int32_t>(incoming_indptr_array, "incoming_indptr_array"),
             int32_t(incoming_indptr_array.size() - 1),
             "incoming_weights"))
       , nodes_count(outgoing_weights.bands_count())
+      , low_mass(low_mass)
+      , target_mass(target_mass)
+      , high_mass(high_mass)
+      , mass_of_nodes(mass_of_nodes_array, "mass_of_nodes")
       , partition_of_nodes(partition_of_nodes_array, "partition_of_nodes")
       , temperature_of_nodes(nodes_count, 1.0)
       , size_of_partitions(initial_size_of_partitions(partition_of_nodes))
       , partitions_count(size_of_partitions.size())
       , incoming_scale(initial_incoming_scale(incoming_weights))
       , score_of_nodes_of_partitions(initial_score_of_nodes_of_partitions(outgoing_weights,
                                                                           incoming_weights,
                                                                           partition_of_nodes,
                                                                           partitions_count))
+      , mass_of_partitions(initial_mass_of_partitions(nodes_count, partition_of_nodes, partitions_count, mass_of_nodes))
       , score_of_partitions(initial_score_of_partitions(nodes_count,
                                                         partition_of_nodes,
                                                         partitions_count,
-                                                        score_of_nodes_of_partitions)) {}
+                                                        score_of_nodes_of_partitions)) {
+        FastAssertCompare(0.0, <, low_mass);
+        FastAssertCompare(low_mass, <, target_mass);
+        FastAssertCompare(target_mass, <, high_mass);
+    }
 
     float64_t score(bool with_orphans = true) const {
-        /*
-        if (!with_orphans) {
-            std::cerr << "node,partition,total_outgoing,total_incoming" << std::endl;
-            for (size_t node_index = 0; node_index < nodes_count; ++node_index) {
-                for (size_t partition_index = 0; partition_index < partitions_count;
-                     ++partition_index) {
-                    std::cerr << node_index << ","       //
-                              << partition_index << ","  //
-                              << score_of_nodes_of_partitions[partition_index][node_index]
-                                     .total_outgoing_weights()
-                              << ","  //
-                              << score_of_nodes_of_partitions[partition_index][node_index]
-                                     .total_incoming_weights()  //
-                              << std::endl;
-                }
-            }
-        }
-        */
-
         float64_t total_score = nodes_count * log2(float64_t(nodes_count)) - incoming_scale;
         size_t orphans_count = nodes_count;
         for (size_t partition_index = 0; partition_index < partitions_count; ++partition_index) {
             const float64_t score_of_partition = score_of_partitions[partition_index];
+            const float64_t mass_of_partition = mass_of_partitions[partition_index];
             const size_t size_of_partition = size_of_partitions[partition_index];
             total_score += score_of_partition - size_of_partition * log2(float64_t(size_of_partition));
+            total_score += size_of_partition * mass_factor(mass_of_partition, low_mass, target_mass, high_mass);
             orphans_count -= size_of_partition;
         }
         if (with_orphans) {
             total_score += orphans_count * NodeScore().score();
             return total_score / nodes_count;
         } else {
             return total_score / (nodes_count - orphans_count);
@@ -281,16 +324,15 @@
     }
 
 #if ASSERT_LEVEL > 0
     void verify(const OptimizePartitions& other) {
 #    define ASSERT_SAME(CONTEXT, FIELD, EPSILON)                                                                 \
         if (fabs(double(this_##FIELD) - double(other_##FIELD)) > EPSILON) {                                      \
             std::cerr << "OOPS! " << #CONTEXT << ": " << CONTEXT << " actual " << #FIELD << ": " << this_##FIELD \
-                      << ": "                                                                                    \
-                      << " computed " << #FIELD << ": " << other_##FIELD << ": " << std::endl;                   \
+                      << " != computed " << #FIELD << ": " << other_##FIELD << ": " << std::endl;                \
             assert(false);                                                                                       \
         } else
 
         ConstArraySlice<int32_t> other_partition_of_nodes = other.partition_of_nodes;
         for (size_t node_index = 0; node_index < nodes_count; ++node_index) {
             auto this_partition_index = partition_of_nodes[node_index];
             auto other_partition_index = other_partition_of_nodes[node_index];
@@ -299,35 +341,36 @@
 
         for (size_t partition_index = 0; partition_index < partitions_count; ++partition_index) {
             for (size_t node_index = 0; node_index < nodes_count; ++node_index) {
                 const auto& this_score_of_node = score_of_nodes_of_partitions[partition_index][node_index];
                 const auto& other_score_of_node = other.score_of_nodes_of_partitions[partition_index][node_index];
 
 #    define ASSERT_SCORE_FIELD(FIELD)                                                                                \
-        if (fabs(this_score_of_node.FIELD() - other_score_of_node.FIELD()) >= EPSILON) {                             \
+        if (fabs(this_score_of_node.FIELD() - other_score_of_node.FIELD()) > EPSILON) {                              \
             std::cerr << "OOPS! partition_index: " << partition_index << " node_index: " << node_index << " actual " \
-                      << #FIELD << ": " << this_score_of_node.FIELD() << " computed " << #FIELD << " : "             \
+                      << #FIELD << ": " << this_score_of_node.FIELD() << " != computed " << #FIELD << " : "          \
                       << other_score_of_node.FIELD() << std::endl;                                                   \
             assert(false);                                                                                           \
         } else
 
                 ASSERT_SCORE_FIELD(total_outgoing_weights);
                 ASSERT_SCORE_FIELD(total_incoming_weights);
                 ASSERT_SCORE_FIELD(score);
             }
 
-            auto this_partition_score = score_of_partitions[partition_index];
-            auto other_partition_score = other.score_of_partitions[partition_index];
+            const float64_t this_partition_score = score_of_partitions[partition_index];
+            const float64_t other_partition_score = other.score_of_partitions[partition_index];
             ASSERT_SAME(partition_index, partition_score, 1e-3);
+
+            const float64_t this_partition_mass = mass_of_partitions[partition_index];
+            const float64_t other_partition_mass = other.mass_of_partitions[partition_index];
+            ASSERT_SAME(partition_index, partition_mass, 1e-3);
         }
 
-        auto this_score = score();
-        auto other_score = other.score();
-        LOCATED_LOG(false) << " score: " << this_score << " ~ " << other_score << std::endl;
-        assert(fabs(this_score - other_score) < 1e-3);
+        assert(fabs(score() - other.score()) < 1e-3);
     }
 #endif
 
     void optimize(const size_t random_seed,
                   float64_t cooldown_pass,
                   float64_t cooldown_node,
                   int32_t cold_partitions,
@@ -350,50 +393,54 @@
                 frozen_nodes[node_index] = 1;
                 ++frozen_count;
             } else if (partition_index >= -1) {
                 temperature_of_nodes[node_index] = 1.0;
                 frozen_nodes[node_index] = 0;
             }
             LOCATED_LOG(false)                                           //
-                << " node: " << node_index                               //
+                << " node_index: " << node_index                         //
                 << " temperature: " << temperature_of_nodes[node_index]  //
                 << std::endl;
         }
 
-        TmpVectorSizeT partitions_raii;
-        auto tmp_partitions = partitions_raii.vector(partitions_count);
+        TmpVectorSizeT size_t_raii;
+        CandidatePartitions tmp_candidate_partitions(size_t_raii, partitions_count);
 
         TmpVectorFloat64 partition_cold_diffs_raii;
         auto tmp_partition_cold_diffs = partition_cold_diffs_raii.vector(partitions_count);
 
         TmpVectorFloat64 partition_hot_diffs_raii;
         auto tmp_partition_hot_diffs = partition_hot_diffs_raii.vector(partitions_count);
 
+        TmpVectorFloat64 partition_connectivity_diffs_raii;
+        auto tmp_partition_connectivity_diffs = partition_connectivity_diffs_raii.vector(partitions_count);
+
         FastAssertCompare(cooldown_node, >=, 0.0);
         FastAssertCompare(cooldown_node, <=, 1.0);
         if (cooldown_pass != 0.0) {
             FastAssertCompare(cooldown_pass, >, 0.0);
             FastAssertCompare(cooldown_pass, <, 1.0);
         }
         float64_t cooldown_rate = 1.0 - cooldown_pass / nodes_count;
         float64_t temperature = 1.0;
 
         bool did_improve = true;
         bool did_skip = false;
+        size_t total_unimproved = 0;
         size_t total_skipped = 0;
         size_t total_improved = 0;
-        size_t total_unimproved = 0;
         while (temperature > 0 || did_improve) {
             LOCATED_LOG(false)                          //
                 << " temperature: " << temperature      //
                 << " cooldown_rate: " << cooldown_rate  //
                 << " score: " << score()                //
                 << " did_improve: " << did_improve      //
                 << " did_skip: " << did_skip            //
                 << std::endl;
+
             if (did_improve) {
                 did_improve = false;
                 did_skip = false;
             } else {
                 if (did_skip) {
                     did_skip = false;
                     for (size_t node_index = 0; node_index < nodes_count; ++node_index) {
@@ -411,115 +458,128 @@
             }
 
             std::shuffle(tmp_indices.begin(), tmp_indices.end(), random);
             size_t skipped = 0;
             size_t improved = 0;
             size_t unimproved = 0;
             for (size_t node_index : tmp_indices) {
-                auto partition_index = partition_of_nodes[node_index];
-                if (partition_index < -1) {
-                    continue;
-                }
                 temperature *= cooldown_rate;
                 LOCATED_LOG(false)                                           //
                     << " cooldown_rate: " << cooldown_rate                   //
                     << " temperature: " << temperature                       //
-                    << " node: " << node_index                               //
+                    << " node_index: " << node_index                         //
                     << " temperature: " << temperature_of_nodes[node_index]  //
                     << std::endl;
                 if (temperature_of_nodes[node_index] < temperature) {
                     did_skip = true;
                     ++skipped;
-                    LOCATED_LOG(false)              //
-                        << " node: " << node_index  //
-                        << " skipped"               //
+                    LOCATED_LOG(false)                    //
+                        << " node_index: " << node_index  //
+                        << " skipped"                     //
                         << std::endl;
                 } else if (improve_node(node_index,
-                                        tmp_partitions,
+                                        tmp_candidate_partitions,
                                         tmp_partition_cold_diffs,
                                         tmp_partition_hot_diffs,
+                                        tmp_partition_connectivity_diffs,
                                         random,
                                         temperature)) {
                     frozen_count -= frozen_nodes[node_index];
                     frozen_nodes[node_index] = uint8_t(0);
                     did_improve = true;
                     ++improved;
-                    LOCATED_LOG(false)              //
-                        << " node: " << node_index  //
-                        << " improved"              //
+                    LOCATED_LOG(false)                    //
+                        << " node_index: " << node_index  //
+                        << " improved"                    //
                         << std::endl;
                 } else {
                     frozen_count -= frozen_nodes[node_index];
                     frozen_nodes[node_index] = uint8_t(0);
                     temperature_of_nodes[node_index] = temperature * (1 - cooldown_node);
                     ++unimproved;
                     LOCATED_LOG(false)                                           //
-                        << " node: " << node_index                               //
+                        << " node_index: " << node_index                         //
                         << " unimproved"                                         //
                         << " temperature: " << temperature_of_nodes[node_index]  //
                         << std::endl;
                 }
             }
             LOCATED_LOG(false)                                      //
                 << " improved: " << improved                        //
                 << " unimproved: " << unimproved                    //
                 << " skipped: " << skipped                          //
                 << " total: " << (improved + unimproved + skipped)  //
                 << " frozen: " << frozen_count                      //
+                << " out of: " << nodes_count                       //
                 << std::endl;
             total_improved += improved;
             total_skipped += skipped;
             total_unimproved += unimproved;
         }
 
         LOCATED_LOG(false)                                                        //
             << " improved: " << total_improved                                    //
             << " unimproved: " << total_unimproved                                //
             << " skipped: " << total_skipped                                      //
             << " total: " << (total_improved + total_unimproved + total_skipped)  //
             << " frozen: " << frozen_count                                        //
+            << " out of: " << nodes_count                                         //
             << std::endl;
         LOCATED_LOG(false)                          //
             << " temperature: " << temperature      //
             << " cooldown_rate: " << cooldown_rate  //
             << " score: " << score()                //
             << std::endl;
     }
 
     bool improve_node(size_t node_index,
-                      std::vector<size_t>& tmp_partitions,
+                      CandidatePartitions& tmp_candidate_partitions,
                       std::vector<float64_t>& tmp_partition_cold_diffs,
                       std::vector<float64_t>& tmp_partition_hot_diffs,
+                      std::vector<float64_t>& tmp_partition_connectivity_diffs,
                       std::minstd_rand& random,
                       const float64_t temperature) {
         const auto current_partition_index = partition_of_nodes[node_index];
-        LOCATED_LOG(false)                                                                                   //
-            << " node: " << node_index                                                                       //
-            << " current_partition_index: " << current_partition_index                                       //
-            << " size: " << (current_partition_index < 0 ? 0 : size_of_partitions[current_partition_index])  //
+        LOCATED_LOG(false)                                               //
+            << " node_index: " << node_index                             //
+            << " current_partition_index: " << current_partition_index   //
+            << " size: " << size_of_partitions[current_partition_index]  //
             << std::endl;
 
-        if (current_partition_index >= 0 && size_of_partitions[current_partition_index] < 2) {
+        if (size_of_partitions[current_partition_index] < 2) {
             return false;
         }
 
         collect_initial_partition_diffs(node_index,
                                         current_partition_index,
                                         tmp_partition_cold_diffs,
                                         tmp_partition_hot_diffs);
 
-        collect_cold_partition_diffs(node_index, current_partition_index, tmp_partition_cold_diffs);
+        collect_cold_partition_diffs(node_index,
+                                     current_partition_index,
+                                     tmp_partition_cold_diffs,
+                                     tmp_partition_connectivity_diffs);
+
+        LOCATED_LOG(false)                                                //
+            << " node_index: " << node_index                              //
+            << " current_partition_index: " << current_partition_index    //
+            << " connectivity_diff: "                                     //
+            << tmp_partition_connectivity_diffs[current_partition_index]  //
+            << std::endl;
 
-        const float64_t current_cold_diff = collect_candidate_partitions(current_partition_index,
+        const float64_t current_cold_diff = collect_candidate_partitions(node_index,
+                                                                         current_partition_index,
                                                                          tmp_partition_cold_diffs,
                                                                          tmp_partition_hot_diffs,
+                                                                         tmp_partition_connectivity_diffs,
                                                                          temperature,
-                                                                         tmp_partitions);
+                                                                         tmp_candidate_partitions);
 
-        const int32_t chosen_partition_index = choose_target_partition(current_partition_index, random, tmp_partitions);
+        const int32_t chosen_partition_index =
+            choose_target_partition(current_partition_index, random, tmp_candidate_partitions);
         if (chosen_partition_index < 0) {
             return false;
         }
 
         const float64_t chosen_cold_diff = tmp_partition_cold_diffs[chosen_partition_index];
         LOCATED_LOG(false)                                //
             << " chosen_cold_diff: " << chosen_cold_diff  //
@@ -532,14 +592,16 @@
         update_sizes_of_partitions(current_partition_index, chosen_partition_index);
 
         update_scores_of_partition(current_partition_index,
                                    current_cold_diff,
                                    chosen_partition_index,
                                    chosen_cold_diff);
 
+        update_masses_of_partition(node_index, current_partition_index, chosen_partition_index);
+
 #if ASSERT_LEVEL > 0
         if (g_verify) {
             g_verify();
         }
 #endif
 
         return true;
@@ -550,26 +612,26 @@
                                          std::vector<float64_t>& tmp_partition_cold_diffs,
                                          std::vector<float64_t>& tmp_partition_hot_diffs) {
         for (size_t partition_index = 0; partition_index < partitions_count; ++partition_index) {
             const int direction = 1 - 2 * (int32_t(partition_index) == current_partition_index);
             const auto score = direction * score_of_nodes_of_partitions[partition_index][node_index].score();
             tmp_partition_cold_diffs[partition_index] = score;
             tmp_partition_hot_diffs[partition_index] = score;
-            LOCATED_LOG(false)                                                  //
-                << " node_index: " << node_index                                //
-                << " partition_index: " << partition_index                      //
-                << " cold_diff: " << tmp_partition_cold_diffs[partition_index]  //
-                << " hot_diff: " << tmp_partition_hot_diffs[partition_index]    //
+            LOCATED_LOG(false)                              //
+                << " node_index: " << node_index            //
+                << " partition_index: " << partition_index  //
+                << " initial_diff: " << score               //
                 << std::endl;
         }
     }
 
     void collect_cold_partition_diffs(const size_t node_index,
                                       const int32_t current_partition_index,
-                                      std::vector<float64_t>& tmp_partition_cold_diffs) {
+                                      std::vector<float64_t>& tmp_partition_cold_diffs,
+                                      std::vector<float64_t>& tmp_partition_connectivity_diffs) {
         const auto& node_outgoing_indices = outgoing_weights.get_band_indices(node_index);
         const auto& node_incoming_indices = incoming_weights.get_band_indices(node_index);
 
         const auto& node_outgoing_weights = outgoing_weights.get_band_data(node_index);
         const auto& node_incoming_weights = incoming_weights.get_band_data(node_index);
 
         size_t outgoing_count = node_outgoing_indices.size();
@@ -583,61 +645,92 @@
 
         auto outgoing_node_index = node_outgoing_indices[outgoing_position];
         auto incoming_node_index = node_incoming_indices[incoming_position];
 
         auto outgoing_edge_weight = node_outgoing_weights[outgoing_position];
         auto incoming_edge_weight = node_incoming_weights[incoming_position];
 
+        const auto& current_score = score_of_nodes_of_partitions[current_partition_index][node_index];
+        const float64_t current_connectivity = current_score.connectivity();
+
+        LOCATED_LOG(false)                                              //
+            << " node_index: " << node_index                            //
+            << " current_partition_index: " << current_partition_index  //
+            << " current_connectivity" << current_connectivity          //
+            << std::endl;
+
+        for (size_t partition_index = 0; partition_index < partitions_count; ++partition_index) {
+            if (partition_index == size_t(current_partition_index)) {
+                tmp_partition_connectivity_diffs[partition_index] = 0.0;
+                continue;
+            }
+
+            const auto& partition_score = score_of_nodes_of_partitions[partition_index][node_index];
+            const float64_t partition_connectivity = partition_score.connectivity();
+
+            LOCATED_LOG(false)                                      //
+                << " node_index: " << node_index                    //
+                << " other_partition_index: " << partition_index    //
+                << " other_connectivity" << partition_connectivity  //
+                << std::endl;
+
+            tmp_partition_connectivity_diffs[partition_index] = partition_connectivity - current_connectivity;
+        }
+
         while (outgoing_position < outgoing_count || incoming_position < incoming_count) {
             const auto other_node_index = std::min(outgoing_node_index, incoming_node_index);
             const auto other_partition_index = partition_of_nodes[other_node_index];
 
             const int is_outgoing = int(outgoing_node_index == other_node_index);
             const int is_incoming = int(incoming_node_index == other_node_index);
 
             LOCATED_LOG(false)                                          //
                 << " consider other_node " << other_node_index          //
                 << " other_partition_index: " << other_partition_index  //
                 << std::endl;
 
-            if (other_partition_index >= 0) {
-                NodeScore other_score = score_of_nodes_of_partitions[other_partition_index][other_node_index];
-                const float64_t old_score = other_score.score();
-
-                LOCATED_LOG(false)                                          //
-                    << " other_node_index: " << other_node_index            //
-                    << " other_partition_index: " << other_partition_index  //
-                    << " old score: " << other_score                        //
-                    << std::endl;
+            NodeScore other_score = score_of_nodes_of_partitions[other_partition_index][other_node_index];
+            const float64_t old_score = other_score.score();
+            const float64_t old_connectivity = other_score.connectivity();
+
+            LOCATED_LOG(false)                                          //
+                << " other_node_index: " << other_node_index            //
+                << " other_partition_index: " << other_partition_index  //
+                << " old score: " << other_score                        //
+                << " old connectivity: " << old_connectivity            //
+                << std::endl;
 
-                const int direction = 1 - 2 * (other_partition_index == current_partition_index);
+            const int direction = 1 - 2 * (other_partition_index == current_partition_index);
 
-                other_score.update_incoming(direction * is_outgoing, outgoing_edge_weight);
-                LOCATED_LOG(false && is_outgoing)                         //
-                    << " other_node_index: " << other_node_index          //
-                    << " direction: " << direction                        //
-                    << " outgoing_edge_weight: " << outgoing_edge_weight  //
-                    << std::endl;
+            other_score.update_incoming(direction * is_outgoing, outgoing_edge_weight);
+            LOCATED_LOG(false && is_outgoing)                         //
+                << " other_node_index: " << other_node_index          //
+                << " direction: " << direction                        //
+                << " outgoing_edge_weight: " << outgoing_edge_weight  //
+                << std::endl;
 
-                other_score.update_outgoing(direction * is_incoming, incoming_edge_weight);
-                LOCATED_LOG(false && is_incoming)                         //
-                    << " other_node_index: " << other_node_index          //
-                    << " direction: " << direction                        //
-                    << " incoming_edge_weight: " << incoming_edge_weight  //
-                    << std::endl;
+            other_score.update_outgoing(direction * is_incoming, incoming_edge_weight);
+            LOCATED_LOG(false && is_incoming)                         //
+                << " other_node_index: " << other_node_index          //
+                << " direction: " << direction                        //
+                << " incoming_edge_weight: " << incoming_edge_weight  //
+                << std::endl;
 
-                const float64_t new_score = other_score.rescore();
-                LOCATED_LOG(false)                                          //
-                    << " other_node_index: " << other_node_index            //
-                    << " other_partition_index: " << other_partition_index  //
-                    << " new score: " << other_score                        //
-                    << std::endl;
+            const float64_t new_score = other_score.rescore();
+            const int new_connectivity = other_score.connectivity();
 
-                tmp_partition_cold_diffs[other_partition_index] += new_score - old_score;
-            }
+            LOCATED_LOG(false)                                          //
+                << " other_node_index: " << other_node_index            //
+                << " other_partition_index: " << other_partition_index  //
+                << " new score: " << other_score                        //
+                << " new connectivity: " << new_connectivity            //
+                << std::endl;
+
+            tmp_partition_cold_diffs[other_partition_index] += new_score - old_score;
+            tmp_partition_connectivity_diffs[other_partition_index] += new_connectivity - old_connectivity;
 
             outgoing_position += is_outgoing;
             incoming_position += is_incoming;
 
             if (outgoing_position < outgoing_count) {
                 outgoing_node_index = node_outgoing_indices[outgoing_position];
                 outgoing_edge_weight = node_outgoing_weights[outgoing_position];
@@ -652,112 +745,180 @@
             } else {
                 incoming_node_index = int32_t(nodes_count);
                 incoming_edge_weight = 0;
             }
         }
     }
 
-    float64_t collect_candidate_partitions(const int32_t current_partition_index,
+    float64_t collect_candidate_partitions(const size_t node_index,
+                                           const int32_t current_partition_index,
                                            const std::vector<float64_t>& tmp_partition_cold_diffs,
                                            const std::vector<float64_t>& tmp_partition_hot_diffs,
+                                           const std::vector<float64_t>& tmp_partition_connectivity_diffs,
                                            const float64_t temperature,
-                                           std::vector<size_t>& tmp_partitions) {
-        float64_t current_hot_diff = 0;
-        float64_t current_cold_diff = 0;
-        float64_t current_adjusted_cold_diff = 0;
-
-        if (current_partition_index >= 0) {
-            const float64_t hot_diff = tmp_partition_hot_diffs[current_partition_index];
-            const size_t old_size = size_of_partitions[current_partition_index];
-            const size_t new_size = old_size - 1;
-            const float64_t old_score = score_of_partitions[current_partition_index];
-            const float64_t old_adjusted_score = old_score - old_size * log2(float64_t(old_size));
-            const float64_t cold_diff = tmp_partition_cold_diffs[current_partition_index];
-            const float64_t new_score = old_score + cold_diff;
-            const float64_t new_adjusted_score = new_score - new_size * log2(float64_t(new_size));
-            const float64_t adjusted_cold_diff = new_adjusted_score - old_adjusted_score;
-            LOCATED_LOG(false)                                              //
-                << " current_partition_index: " << current_partition_index  //
-                << " hot_diff: " << hot_diff                                //
-                << " old_score: " << old_score                              //
-                << " new_score: " << new_score                              //
-                << " cold_diff: " << cold_diff                              //
-                << " old_size: " << old_size                                //
-                << " new_size: " << new_size                                //
-                << " old_adjusted_score: " << old_adjusted_score            //
-                << " new_adjusted_score: " << new_adjusted_score            //
-                << " adjusted_cold_diff: " << adjusted_cold_diff            //
-                << std::endl;
-            current_cold_diff = cold_diff;
-            current_hot_diff = hot_diff;
-            current_adjusted_cold_diff = adjusted_cold_diff;
-        }
+                                           CandidatePartitions& tmp_candidate_partitions) {
+        float32_t node_mass = mass_of_nodes[node_index];
+
+        const float64_t current_hot_diff = tmp_partition_hot_diffs[current_partition_index];
+        const float64_t current_cold_diff = tmp_partition_cold_diffs[current_partition_index];
+
+        const size_t old_size = size_of_partitions[current_partition_index];
+        const float64_t old_mass = mass_of_partitions[current_partition_index];
+        const float64_t old_mass_factor = mass_factor(old_mass, low_mass, target_mass, high_mass);
+        const float64_t old_score = score_of_partitions[current_partition_index];
+        float64_t old_adjusted_score = old_score - old_size * log2(float64_t(old_size));
+        old_adjusted_score += old_size * old_mass_factor;
+
+        LOCATED_LOG(false)                                              //
+            << " current_partition_index: " << current_partition_index  //
+            << " old_size: " << old_size                                //
+            << " old_mass: " << old_mass                                //
+            << " old_mass_factor: " << old_mass_factor                  //
+            << " old_score: " << old_score                              //
+            << " old_adjusted_score: " << old_adjusted_score            //
+            << std::endl;
+
+        const size_t new_size = old_size - 1;
+        const float64_t new_mass = old_mass - node_mass;
+        const float64_t new_mass_factor = mass_factor(new_mass, low_mass, target_mass, high_mass);
+        const float64_t new_score = old_score + current_cold_diff;
+        float64_t new_adjusted_score = new_score - new_size * log2(float64_t(new_size));
+        new_adjusted_score += new_size * new_mass_factor;
+
+        LOCATED_LOG(false)                                              //
+            << " current_partition_index: " << current_partition_index  //
+            << " new_size: " << new_size                                //
+            << " new_mass: " << new_mass                                //
+            << " new_mass_factor: " << new_mass_factor                  //
+            << " new_score: " << new_score                              //
+            << " new_adjusted_score: " << new_adjusted_score            //
+            << std::endl;
 
-        tmp_partitions.clear();
+        const float64_t current_adjusted_cold_diff = new_adjusted_score - old_adjusted_score;
+        const float64_t current_connectivity_diff = tmp_partition_connectivity_diffs[current_partition_index];
+
+        LOCATED_LOG(false)                                              //
+            << " current_partition_index: " << current_partition_index  //
+            << " hot_diff: " << current_hot_diff                        //
+            << " cold_diff: " << current_cold_diff                      //
+            << " adjusted_cold_diff: " << current_adjusted_cold_diff    //
+            << " connectivity_diff: " << current_connectivity_diff      //
+            << std::endl;
+
+        tmp_candidate_partitions.clear();
         for (size_t partition_index = 0; partition_index < partitions_count; ++partition_index) {
             if (int32_t(partition_index) == current_partition_index) {
                 continue;
             }
+
+            const float64_t partition_connectivity_diff = tmp_partition_connectivity_diffs[partition_index];
+            const float64_t adjusted_connectivity_diff = partition_connectivity_diff + current_connectivity_diff;
+            LOCATED_LOG(false)                                                    //
+                << " partition_index: " << partition_index                        //
+                << " connectivity_diff: " << partition_connectivity_diff          //
+                << " adjusted_connectivity_diff: " << adjusted_connectivity_diff  //
+                << std::endl;
+
+            if (adjusted_connectivity_diff < 0) {
+                continue;
+            }
+
             const float64_t hot_diff = tmp_partition_hot_diffs[partition_index];
+            const float64_t cold_diff = tmp_partition_cold_diffs[partition_index];
             const size_t old_size = size_of_partitions[partition_index];
-            const size_t new_size = old_size + 1;
+            const float64_t old_mass = mass_of_partitions[partition_index];
+            const float64_t old_mass_factor = mass_factor(old_mass, low_mass, target_mass, high_mass);
             const float64_t old_score = score_of_partitions[partition_index];
-            const float64_t cold_diff = tmp_partition_cold_diffs[partition_index];
+            float64_t old_adjusted_score = old_score - old_size * log2(float64_t(old_size));
+            old_adjusted_score += old_size * old_mass_factor;
+
+            LOCATED_LOG(false)                                    //
+                << " partition_index: " << partition_index        //
+                << " old_size: " << old_size                      //
+                << " old_mass: " << old_mass                      //
+                << " old_score: " << old_score                    //
+                << " old_mass_factor: " << old_mass_factor        //
+                << " old_adjusted_score: " << old_adjusted_score  //
+                << std::endl;
+
+            const size_t new_size = old_size + 1;
+            const float64_t new_mass = old_mass + node_mass;
+            const float64_t new_mass_factor = mass_factor(new_mass, low_mass, target_mass, high_mass);
             const float64_t new_score = old_score + cold_diff;
-            const float64_t old_adjusted_score = old_score - old_size * log2(float64_t(old_size));
-            const float64_t new_adjusted_score = new_score - new_size * log2(float64_t(new_size));
+            float64_t new_adjusted_score = new_score - new_size * log2(float64_t(new_size));
+            new_adjusted_score += new_size * new_mass_factor;
+
+            LOCATED_LOG(false)                                    //
+                << " partition_index: " << partition_index        //
+                << " new_size: " << new_size                      //
+                << " new_mass: " << new_mass                      //
+                << " new_score: " << new_score                    //
+                << " new_mass_factor: " << new_mass_factor        //
+                << " new_adjusted_score: " << new_adjusted_score  //
+                << std::endl;
+
             const float64_t adjusted_cold_diff = new_adjusted_score - old_adjusted_score;
             const float64_t total_diff = (current_hot_diff + hot_diff) * temperature
                                          + (current_adjusted_cold_diff + adjusted_cold_diff) * (1.0 - temperature);
+
             LOCATED_LOG(false)                                    //
                 << " partition_index: " << partition_index        //
-                << " old_score: " << old_score                    //
-                << " new_score: " << new_score                    //
                 << " hot_diff: " << hot_diff                      //
                 << " cold_diff: " << cold_diff                    //
-                << " old_size: " << old_size                      //
-                << " new_size: " << new_size                      //
-                << " old_adjusted_score: " << old_adjusted_score  //
-                << " new_adjusted_score: " << new_adjusted_score  //
                 << " adjusted_cold_diff: " << adjusted_cold_diff  //
                 << " total_diff: " << total_diff                  //
                 << std::endl;
-            if (total_diff > EPSILON) {
-                tmp_partitions.push_back(partition_index);
+
+            if (adjusted_connectivity_diff > 0) {
+                if (total_diff >= EPSILON) {
+                    tmp_candidate_partitions.both_partitions.push_back(partition_index);
+                } else {
+                    tmp_candidate_partitions.connectivity_partitions.push_back(partition_index);
+                }
+            } else if (total_diff >= EPSILON) {
+                tmp_candidate_partitions.goal_partitions.push_back(partition_index);
             }
         }
 
         return current_cold_diff;
     }
 
     int32_t choose_target_partition(const int32_t current_partition_index,
                                     std::minstd_rand& random,
-                                    const std::vector<size_t>& tmp_partitions) {
+                                    const CandidatePartitions& tmp_candidate_partitions) {
         int32_t chosen_partition_index = -1;
-        if (tmp_partitions.size() == 0) {
-            if (current_partition_index >= 0) {
-                return -1;
-            }
-            chosen_partition_index = random() % partitions_count;
-        } else {
-            chosen_partition_index = int32_t(tmp_partitions[random() % tmp_partitions.size()]);
-        }
 
-        LOCATED_LOG(false)                                            //
-            << " chosen_partition_index: " << chosen_partition_index  //
-            << std::endl;
+        if (tmp_candidate_partitions.both_partitions.size() > 0) {
+            chosen_partition_index = int32_t(
+                tmp_candidate_partitions.both_partitions[random() % tmp_candidate_partitions.both_partitions.size()]);
+            LOCATED_LOG(false)                                                 //
+                << " chosen both partition_index: " << chosen_partition_index  //
+                << std::endl;
+        } else if (tmp_candidate_partitions.connectivity_partitions.size() > 0) {
+            chosen_partition_index = int32_t(
+                tmp_candidate_partitions
+                    .connectivity_partitions[random() % tmp_candidate_partitions.connectivity_partitions.size()]);
+            LOCATED_LOG(false)                                                         //
+                << " chosen connectivity partition_index: " << chosen_partition_index  //
+                << std::endl;
+        } else if (tmp_candidate_partitions.goal_partitions.size() > 0) {
+            chosen_partition_index = int32_t(
+                tmp_candidate_partitions.goal_partitions[random() % tmp_candidate_partitions.goal_partitions.size()]);
+            LOCATED_LOG(false)                                                 //
+                << " chosen goal partition_index: " << chosen_partition_index  //
+                << std::endl;
+        }
 
         return chosen_partition_index;
     }
 
     void update_scores_of_nodes(const size_t node_index,
                                 const int32_t from_partition_index,
                                 const int32_t to_partition_index) {
-        auto score_of_nodes_of_from_partition =
-            from_partition_index < 0 ? nullptr : &score_of_nodes_of_partitions[from_partition_index];
+        auto& score_of_nodes_of_from_partition = score_of_nodes_of_partitions[from_partition_index];
         auto& score_of_nodes_of_to_partition = score_of_nodes_of_partitions[to_partition_index];
 
         const auto& node_outgoing_indices = outgoing_weights.get_band_indices(node_index);
         const auto& node_incoming_indices = incoming_weights.get_band_indices(node_index);
 
         const auto& node_outgoing_weights = outgoing_weights.get_band_data(node_index);
         const auto& node_incoming_weights = incoming_weights.get_band_data(node_index);
@@ -779,32 +940,30 @@
 
         while (outgoing_position < outgoing_count || incoming_position < incoming_count) {
             const auto other_node_index = std::min(outgoing_node_index, incoming_node_index);
 
             const int is_outgoing = int(outgoing_node_index == other_node_index);
             const int is_incoming = int(incoming_node_index == other_node_index);
 
-            if (score_of_nodes_of_from_partition) {
-                auto& other_node_from_score = (*score_of_nodes_of_from_partition)[other_node_index];
-                LOCATED_LOG(false)                                        //
-                    << " other_node_index: " << other_node_index          //
-                    << " from_partition_index: " << from_partition_index  //
-                    << " old score: " << other_node_from_score            //
-                    << std::endl;
+            auto& other_node_from_score = score_of_nodes_of_from_partition[other_node_index];
+            LOCATED_LOG(false)                                        //
+                << " other_node_index: " << other_node_index          //
+                << " from_partition_index: " << from_partition_index  //
+                << " old score: " << other_node_from_score            //
+                << std::endl;
 
-                other_node_from_score.update_incoming(-is_outgoing, outgoing_edge_weight);
-                other_node_from_score.update_outgoing(-is_incoming, incoming_edge_weight);
-                other_node_from_score.rescore();
-
-                LOCATED_LOG(false)                                        //
-                    << " other_node_index: " << other_node_index          //
-                    << " from_partition_index: " << from_partition_index  //
-                    << " new score: " << other_node_from_score            //
-                    << std::endl;
-            }
+            other_node_from_score.update_incoming(-is_outgoing, outgoing_edge_weight);
+            other_node_from_score.update_outgoing(-is_incoming, incoming_edge_weight);
+            other_node_from_score.rescore();
+
+            LOCATED_LOG(false)                                        //
+                << " other_node_index: " << other_node_index          //
+                << " from_partition_index: " << from_partition_index  //
+                << " new score: " << other_node_from_score            //
+                << std::endl;
 
             auto& other_node_to_score = score_of_nodes_of_to_partition[other_node_index];
             LOCATED_LOG(false)                                    //
                 << " other_node_index: " << other_node_index      //
                 << " to_partition_index: " << to_partition_index  //
                 << " old score: " << other_node_to_score          //
                 << std::endl;
@@ -849,114 +1008,156 @@
             << " set node_index: " << node_index                  //
             << " from_partition_index: " << from_partition_index  //
             << " to_partition_index: " << to_partition_index      //
             << std::endl;
     }
 
     void update_sizes_of_partitions(const int32_t from_partition_index, const int32_t to_partition_index) {
-        if (from_partition_index >= 0) {
-            SlowAssertCompare(size_of_partitions[from_partition_index], >, 1);
-            size_of_partitions[from_partition_index] -= 1;
-        }
-
+        SlowAssertCompare(size_of_partitions[from_partition_index], >, 1);
+        size_of_partitions[from_partition_index] -= 1;
         ++size_of_partitions[to_partition_index];
     }
 
-    void update_scores_of_partition(size_t current_partition_index,
-                                    float64_t current_cold_diff,
-                                    size_t chosen_partition_index,
-                                    float64_t chosen_cold_diff) {
-        if (current_partition_index >= 0) {
-            LOCATED_LOG(false)                                                     //
-                << " from_partition_index: " << current_partition_index            //
-                << " old score: " << score_of_partitions[current_partition_index]  //
-                << " from_cold_diff: " << current_cold_diff                        //
-                << std::endl;
-            score_of_partitions[current_partition_index] += current_cold_diff;
-            LOCATED_LOG(false)                                                     //
-                << " from_partition_index: " << current_partition_index            //
-                << " new score: " << score_of_partitions[current_partition_index]  //
-                << std::endl;
-        }
+    void update_scores_of_partition(const int32_t current_partition_index,
+                                    const float64_t current_cold_diff,
+                                    const int32_t chosen_partition_index,
+                                    const float64_t chosen_cold_diff) {
+        LOCATED_LOG(false)                                                     //
+            << " from_partition_index: " << current_partition_index            //
+            << " old score: " << score_of_partitions[current_partition_index]  //
+            << " from_cold_diff: " << current_cold_diff                        //
+            << std::endl;
+        score_of_partitions[current_partition_index] += current_cold_diff;
+        LOCATED_LOG(false)                                                     //
+            << " from_partition_index: " << current_partition_index            //
+            << " new score: " << score_of_partitions[current_partition_index]  //
+            << std::endl;
 
         LOCATED_LOG(false)                                                    //
             << " to_partition_index: " << chosen_partition_index              //
             << " old score: " << score_of_partitions[chosen_partition_index]  //
             << " to_cold_diff: " << chosen_cold_diff                          //
             << std::endl;
         score_of_partitions[chosen_partition_index] += chosen_cold_diff;
         LOCATED_LOG(false)                                                    //
             << " to_partition_index: " << chosen_partition_index              //
             << " new score: " << score_of_partitions[chosen_partition_index]  //
             << std::endl;
     }
+
+    void update_masses_of_partition(const size_t node_index,
+                                    const int32_t current_partition_index,
+                                    const int32_t chosen_partition_index) {
+        const float32_t node_mass = mass_of_nodes[node_index];
+
+        LOCATED_LOG(false)                                                   //
+            << " from_partition_index: " << current_partition_index          //
+            << " old mass: " << mass_of_partitions[current_partition_index]  //
+            << std::endl;
+        mass_of_partitions[current_partition_index] -= node_mass;
+        LOCATED_LOG(false)                                                   //
+            << " from_partition_index: " << current_partition_index          //
+            << " new mass: " << mass_of_partitions[current_partition_index]  //
+            << std::endl;
+
+        LOCATED_LOG(false)                                                  //
+            << " to_partition_index: " << chosen_partition_index            //
+            << " old mass: " << mass_of_partitions[chosen_partition_index]  //
+            << std::endl;
+        mass_of_partitions[chosen_partition_index] += node_mass;
+        LOCATED_LOG(false)                                                  //
+            << " to_partition_index: " << chosen_partition_index            //
+            << " new mass: " << mass_of_partitions[chosen_partition_index]  //
+            << std::endl;
+    }
 };
 
 static float64_t
 optimize_partitions(const pybind11::array_t<float32_t>& outgoing_weights_array,
                     const pybind11::array_t<int32_t>& outgoing_indices_array,
                     const pybind11::array_t<int32_t>& outgoing_indptr_array,
                     const pybind11::array_t<float32_t>& incoming_weights_array,
                     const pybind11::array_t<int32_t>& incoming_indices_array,
                     const pybind11::array_t<int32_t>& incoming_indptr_array,
                     const unsigned int random_seed,
+                    float64_t low_mass,
+                    float64_t target_mass,
+                    float64_t high_mass,
+                    const pybind11::array_t<float32_t>& mass_of_nodes_array,
                     float64_t cooldown_pass,
                     float64_t cooldown_node,
                     pybind11::array_t<int32_t>& partition_of_nodes_array,
                     int32_t cold_partitions,
                     float64_t cold_temperature) {
     WithoutGil without_gil{};
     OptimizePartitions optimizer(outgoing_weights_array,
                                  outgoing_indices_array,
                                  outgoing_indptr_array,
                                  incoming_weights_array,
                                  incoming_indices_array,
                                  incoming_indptr_array,
+                                 low_mass,
+                                 target_mass,
+                                 high_mass,
+                                 mass_of_nodes_array,
                                  partition_of_nodes_array);
 
 #if ASSERT_LEVEL > 1
     g_verify = [&]() {
         LOCATED_LOG(false) << " VERIFY" << std::endl;
         OptimizePartitions verifier(outgoing_weights_array,
                                     outgoing_indices_array,
                                     outgoing_indptr_array,
                                     incoming_weights_array,
                                     incoming_indices_array,
                                     incoming_indptr_array,
+                                    low_mass,
+                                    target_mass,
+                                    high_mass,
+                                    mass_of_nodes_array,
                                     partition_of_nodes_array);
         LOCATED_LOG(false) << " COMPARE" << std::endl;
         verifier.verify(optimizer);
         LOCATED_LOG(false) << " VERIFIED" << std::endl;
     };
 #else
     g_verify = nullptr;
 #endif
 
     optimizer.optimize(random_seed, cooldown_pass, cooldown_node, cold_partitions, cold_temperature);
 
     float64_t score = optimizer.score();
+    LOCATED_LOG(false) << " SCORE: " << score << std::endl;
     return score;
 }
 
 static float64_t
 score_partitions(const pybind11::array_t<float32_t>& outgoing_weights_array,
                  const pybind11::array_t<int32_t>& outgoing_indices_array,
                  const pybind11::array_t<int32_t>& outgoing_indptr_array,
                  const pybind11::array_t<float32_t>& incoming_weights_array,
                  const pybind11::array_t<int32_t>& incoming_indices_array,
                  const pybind11::array_t<int32_t>& incoming_indptr_array,
+                 const float64_t low_mass,
+                 const float64_t target_mass,
+                 const float64_t high_mass,
+                 const pybind11::array_t<float32_t>& mass_of_nodes_array,
                  pybind11::array_t<int32_t>& partition_of_nodes_array,
                  bool with_orphans) {
     WithoutGil without_gil{};
     OptimizePartitions optimizer(outgoing_weights_array,
                                  outgoing_indices_array,
                                  outgoing_indptr_array,
                                  incoming_weights_array,
                                  incoming_indices_array,
                                  incoming_indptr_array,
+                                 low_mass,
+                                 target_mass,
+                                 high_mass,
+                                 mass_of_nodes_array,
                                  partition_of_nodes_array);
     return optimizer.score(with_orphans);
 }
 
 void
 register_partitions(pybind11::module& module) {
     module.def("optimize_partitions",
```

### Comparing `metacells-0.8.0/metacells/pipeline/__init__.py` & `metacells-0.9.0/metacells/pipeline/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 This pipeline can be configured by tweaking the (many) parameters, but for any deeper customization
 (adding and/or removing steps) just provide your own pipeline instead. You can use the
 implementation here as a starting point.
 
 All the functions included here are exported under ``metacells.pl``.
 """
 
-from .clean import *
 from .collect import *
 from .consistency import *
 from .direct import *
 from .divide_and_conquer import *
-from .feature import *
+from .exclude import *
+from .mark import *
 from .mcview import *
 from .projection import *
 from .related_genes import *
+from .select import *
 from .umap import *
```

### Comparing `metacells-0.8.0/metacells/pipeline/clean.py` & `metacells-0.9.0/metacells/pipeline/exclude.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
-Clean
------
+Exclude
+-------
 
-Raw single-cell RNA sequencing data is notoriously noisy and "dirty". The pipeline steps here
-performs initial analysis of the data and extract just the "clean" data for actually computing the
-metacells. The steps provided here are expected to be generically useful, but as always specific
-data sets may require custom cleaning steps on a case-by-case basis.
+Raw single-cell RNA sequencing data is notoriously noisy and "dirty". The pipeline steps here performs initial analysis
+of the data and exclude some of it, so it would not harm the metacells computation. The steps provided here are expected
+to be generically useful, but as always specific data sets may require custom cleaning steps on a case-by-case basis.
 """
 
 from re import Pattern
 from typing import Collection
 from typing import List
 from typing import Optional
 from typing import Union
@@ -17,269 +16,232 @@
 from anndata import AnnData  # type: ignore
 
 import metacells.parameters as pr
 import metacells.tools as tl
 import metacells.utilities as ut
 
 __all__ = [
-    "analyze_clean_genes",
-    "pick_clean_genes",
-    "analyze_clean_cells",
-    "pick_clean_cells",
+    "exclude_genes",
+    "exclude_cells",
     "extract_clean_data",
 ]
 
 
 @ut.logged()
 @ut.timed_call()
 @ut.expand_doc()
-def analyze_clean_genes(
+def exclude_genes(
     adata: AnnData,
     what: Union[str, ut.Matrix] = "__x__",
     *,
-    properly_sampled_min_gene_total: int = pr.properly_sampled_min_gene_total,
-    noisy_lonely_max_sampled_cells: int = pr.noisy_lonely_max_sampled_cells,
-    noisy_lonely_downsample_min_samples: int = pr.noisy_lonely_downsample_min_samples,
-    noisy_lonely_downsample_min_cell_quantile: float = pr.noisy_lonely_downsample_min_cell_quantile,
-    noisy_lonely_downsample_max_cell_quantile: float = pr.noisy_lonely_downsample_max_cell_quantile,
-    noisy_lonely_min_gene_total: int = pr.noisy_lonely_min_gene_total,
-    noisy_lonely_min_gene_normalized_variance: float = pr.noisy_lonely_min_gene_normalized_variance,
-    noisy_lonely_max_gene_similarity: float = pr.noisy_lonely_max_gene_similarity,
+    bursty_max_sampled_cells: Optional[int] = pr.bursty_lonely_max_sampled_cells,
+    bursty_downsample_min_samples: int = pr.bursty_lonely_downsample_min_samples,
+    bursty_downsample_min_cell_quantile: float = pr.bursty_lonely_downsample_max_cell_quantile,
+    bursty_downsample_max_cell_quantile: float = pr.bursty_lonely_downsample_min_cell_quantile,
+    bursty_min_gene_total: int = pr.bursty_lonely_min_gene_total,
+    bursty_min_gene_normalized_variance: float = pr.bursty_lonely_min_gene_normalized_variance,
+    bursty_max_gene_similarity: float = pr.bursty_lonely_max_gene_similarity,
+    properly_sampled_min_gene_total: Optional[int] = pr.properly_sampled_min_gene_total,
     excluded_gene_names: Optional[Collection[str]] = None,
     excluded_gene_patterns: Optional[Collection[Union[str, Pattern]]] = None,
-    random_seed: int = pr.random_seed,
+    random_seed: int,
 ) -> None:
     """
-    Analyze genes in preparation for picking the "clean" subset of the ``adata``.
+    Exclude a subset of the genes from the metacells computation.
+
+    You can also just manually set the ``excluded_gene`` mask, or further manipulate it after calling this function.
 
     **Input**
 
     Annotated ``adata``, where the observations are cells and the variables are genes.
 
     **Returns**
 
     Sets the following in the data:
 
     Variable (gene) annotations:
         ``properly_sampled_gene``
             A mask of the "properly sampled" genes.
 
-        ``noisy_lonely_gene``
-            A mask of the "noisy lonely" genes.
-
         ``excluded_gene``
-            A mask of the genes which were excluded by name.
+            A mask of the genes which were excluded (by name or due to not being properly sampled).
 
     **Computation Parameters**
 
-    1. Invoke :py:func:`metacells.tools.properly_sampled.find_properly_sampled_genes` using
-       ``properly_sampled_min_gene_total`` (default: {properly_sampled_min_gene_total}).
-
-    2. Invoke :py:func:`metacells.tools.noisy_lonely.find_noisy_lonely_genes` using
-       ``noisy_lonely_max_sampled_cells`` (default: {noisy_lonely_max_sampled_cells}),
-       ``noisy_lonely_downsample_min_samples`` (default: {noisy_lonely_downsample_min_samples}),
-       ``noisy_lonely_downsample_min_cell_quantile`` (default:
-       {noisy_lonely_downsample_min_cell_quantile}), ``noisy_lonely_downsample_max_cell_quantile``
-       (default: {noisy_lonely_downsample_max_cell_quantile}), ``noisy_lonely_min_gene_total``
-       (default: {noisy_lonely_min_gene_total}), ``noisy_lonely_min_gene_normalized_variance``
-       (default: {noisy_lonely_min_gene_normalized_variance}), and
-       ``noisy_lonely_max_gene_similarity`` (default: {noisy_lonely_max_gene_similarity}).
-
-    3. Invoke :py:func:`metacells.tools.named.find_named_genes` to exclude genes based on their
-       name, using the ``excluded_gene_names`` (default: {excluded_gene_names}) and
-       ``excluded_gene_patterns`` (default: {excluded_gene_patterns}). This is stored in a
-       per-variable (gene) ``excluded_genes`` boolean mask.
-    """
-    tl.find_properly_sampled_genes(adata, what, min_gene_total=properly_sampled_min_gene_total)
+    1. Invoke :py:func:`metacells.tools.bursty_lonely.find_bursty_lonely_genes` using
+       ``bursty_max_sampled_cells`` (default: {bursty_max_sampled_cells}),
+       ``bursty_downsample_min_samples`` (default: {bursty_downsample_min_samples}),
+       ``bursty_downsample_min_cell_quantile`` (default: {bursty_downsample_min_cell_quantile}),
+       ``bursty_downsample_max_cell_quantile`` (default: {bursty_downsample_max_cell_quantile}),
+       ``bursty_min_gene_total`` (default: {bursty_min_gene_total}),
+       ``bursty_min_gene_normalized_variance`` (default: {bursty_min_gene_normalized_variance}),
+       ``bursty_max_gene_similarity`` (default: {bursty_max_gene_similarity}),
+       and ``random_seed``.
+       Any "bursty_lonely_genes" will be excluded.
+
+    2. Invoke :py:func:`metacells.tools.properly_sampled.find_properly_sampled_genes` using
+       ``properly_sampled_min_gene_total`` (default: {properly_sampled_min_gene_total}). Genes which are not properly
+       sampled will be excluded.
+
+    3. Invoke :py:func:`metacells.tools.named.find_named_genes` to also exclude genes based on their name, using the
+       ``excluded_gene_names`` (default: {excluded_gene_names}) and ``excluded_gene_patterns`` (default:
+       {excluded_gene_patterns}).
+    """
+    if (
+        bursty_max_sampled_cells is None
+        and properly_sampled_min_gene_total is None
+        and excluded_gene_names is None
+        and excluded_gene_patterns is None
+    ):
+        return
+
+    bursty_lonely_genes_mask: Optional[ut.NumpyVector] = None
+    if bursty_max_sampled_cells is not None:
+        tl.find_bursty_lonely_genes(
+            adata,
+            what,
+            max_sampled_cells=bursty_max_sampled_cells,
+            downsample_min_samples=bursty_downsample_min_samples,
+            downsample_min_cell_quantile=bursty_downsample_min_cell_quantile,
+            downsample_max_cell_quantile=bursty_downsample_max_cell_quantile,
+            min_gene_total=bursty_min_gene_total,
+            min_gene_normalized_variance=bursty_min_gene_normalized_variance,
+            max_gene_similarity=bursty_max_gene_similarity,
+            random_seed=random_seed,
+        )
+        bursty_lonely_genes_mask = ut.get_v_numpy(adata, "bursty_lonely_gene")
+
+    properly_sampled_genes_mask: Optional[ut.NumpyVector] = None
+    if properly_sampled_min_gene_total is not None:
+        tl.find_properly_sampled_genes(adata, what, min_gene_total=properly_sampled_min_gene_total)
+        properly_sampled_genes_mask = ut.get_v_numpy(adata, "properly_sampled_gene")
 
-    excluded_genes_mask: Optional[str]
+    named_genes_mask: Optional[ut.NumpyVector] = None
     if excluded_gene_names is not None or excluded_gene_patterns is not None:
-        excluded_genes_mask = "excluded_gene"
-        tl.find_named_genes(adata, to="excluded_gene", names=excluded_gene_names, patterns=excluded_gene_patterns)
-    else:
-        excluded_genes_mask = None
-
-    tl.find_noisy_lonely_genes(
-        adata,
-        what,
-        excluded_genes_mask=excluded_genes_mask,
-        max_sampled_cells=noisy_lonely_max_sampled_cells,
-        downsample_min_samples=noisy_lonely_downsample_min_samples,
-        downsample_min_cell_quantile=noisy_lonely_downsample_min_cell_quantile,
-        downsample_max_cell_quantile=noisy_lonely_downsample_max_cell_quantile,
-        min_gene_total=noisy_lonely_min_gene_total,
-        min_gene_normalized_variance=noisy_lonely_min_gene_normalized_variance,
-        max_gene_similarity=noisy_lonely_max_gene_similarity,
-        random_seed=random_seed,
-    )
+        named_genes_series = tl.find_named_genes(
+            adata, names=excluded_gene_names, patterns=excluded_gene_patterns, to=None
+        )
+        assert named_genes_series is not None
+        named_genes_mask = named_genes_series.values
+
+    excluded_genes_mask: Optional[ut.NumpyVector] = None
+    if bursty_lonely_genes_mask is not None:
+        excluded_genes_mask = bursty_lonely_genes_mask
+
+    if properly_sampled_genes_mask is not None:
+        if excluded_genes_mask is None:
+            excluded_genes_mask = ~properly_sampled_genes_mask
+        else:
+            excluded_genes_mask = excluded_genes_mask | ~properly_sampled_genes_mask
+
+    if named_genes_mask is not None:
+        if excluded_genes_mask is None:
+            excluded_genes_mask = named_genes_mask
+        else:
+            excluded_genes_mask = excluded_genes_mask | named_genes_mask
 
-
-CLEAN_GENES_MASKS = ["properly_sampled_gene?", "~noisy_lonely_gene?", "~excluded_gene?"]
-
-
-@ut.timed_call()
-@ut.expand_doc(masks=", ".join(CLEAN_GENES_MASKS))
-def pick_clean_genes(  # pylint: disable=dangerous-default-value
-    adata: AnnData, *, masks: List[str] = CLEAN_GENES_MASKS, to: str = "clean_gene"
-) -> None:
-    """
-    Create a mask of the "clean" genes that will be used to actually compute the metacells.
-
-    **Input**
-
-    Annotated ``adata``, where the observations are cells and the variables are genes.
-
-    **Returns**
-
-    Sets the following in the data:
-
-    Variable (gene) annotations:
-        ``to`` (default: {to})
-            A mask of the "clean" genes to use for actually computing the metacells.
-
-    **Computation Parameters**
-
-    1. This simply AND-s the specified ``masks`` (default: {masks}) using
-       :py:func:`metacells.tools.mask.combine_masks`.
-    """
-    tl.combine_masks(adata, masks, to=to)
+    assert excluded_genes_mask is not None
+    ut.set_v_data(adata, "excluded_gene", excluded_genes_mask)
 
 
 @ut.logged()
 @ut.timed_call()
-def analyze_clean_cells(
+def exclude_cells(
     adata: AnnData,
     what: Union[str, ut.Matrix] = "__x__",
     *,
     properly_sampled_min_cell_total: Optional[int],
     properly_sampled_max_cell_total: Optional[int],
     properly_sampled_max_excluded_genes_fraction: Optional[float],
+    additional_cells_masks: Optional[List[str]] = None,
 ) -> None:
     """
-    Analyze cells in preparation for extracting the "clean" subset of the ``adata``.
+    Exclude a subset of the cells from the metacells computation.
 
-    Raw single-cell RNA sequencing data is notoriously noisy and "dirty". This pipeline step
-    performs initial analysis of the cells to allow us to extract just the "clean" data for
-    processing. The steps provided here are expected to be generically useful, but as always
-    specific data sets may require custom cleaning steps on a case-by-case basis.
+    You can also just manually set the ``excluded_cell`` mask, or further manipulate it after calling this function.
 
     **Input**
 
-    Annotated ``adata``, where the observations are cells and the variables are genes.
+    Annotated ``adata``, where the observations are cells and the variables are genes. Optionally, may contain an
+    ``excluded_gene`` mask of genes to be excluded from the metacells computation. That is, invoke this after
+    calling :py:func:`exclude_genes` (if you wish to exclude any genes).
 
     **Returns**
 
     Sets the following in the full data:
 
     Observation (cell) annotations:
         ``properly_sampled_cell``
             A mask of the "properly sampled" cells.
 
+        ``excluded_cell``
+            A mask of the genes which were excluded (inverse of ``properly_sampled_cell``).
+
     **Computation Parameters**
 
-    1. If ``properly_sampled_max_excluded_genes_fraction`` is not ``None``, then consider all the
-       genes not covered by the ``clean_gene`` per-variable mask as "excluded" for computing the
-       excluded genes fraction for each cell.
-
-    2. Invoke :py:func:`metacells.tools.properly_sampled.find_properly_sampled_cells` using
-       ``properly_sampled_min_cell_total`` (no default), ``properly_sampled_max_cell_total`` (no
-       default) and ``properly_sampled_max_excluded_genes_fraction`` (no default).
-    """
-    excluded_adata: Optional[AnnData] = None
-    if properly_sampled_max_excluded_genes_fraction is not None:
-        excluded_genes = tl.filter_data(adata, name="dirty_genes", top_level=False, var_masks=["~clean_gene"])
-        if excluded_genes is not None:
-            excluded_adata = excluded_genes[0]
-
-    if excluded_genes is None:
-        max_excluded_genes_fraction = None
-    else:
-        max_excluded_genes_fraction = properly_sampled_max_excluded_genes_fraction
+    1. Invoke :py:func:`metacells.tools.properly_sampled.find_properly_sampled_cells` using
+       ``properly_sampled_min_cell_total`` (no default), ``properly_sampled_max_cell_total`` (no default) and
+       ``properly_sampled_max_excluded_genes_fraction`` (no default).
 
+    2. Exclude any cells which are not properly sampled (``|~properly_sampled_cell``), with optional additional
+       following ``additional_cells_masks`` (using  :py:func:`metacells.tools.mask.combine_masks`).
+    """
     tl.find_properly_sampled_cells(
         adata,
         what,
         min_cell_total=properly_sampled_min_cell_total,
         max_cell_total=properly_sampled_max_cell_total,
-        excluded_adata=excluded_adata,
-        max_excluded_genes_fraction=max_excluded_genes_fraction,
+        max_excluded_genes_fraction=properly_sampled_max_excluded_genes_fraction,
     )
 
-
-CLEAN_CELLS_MASKS = ["properly_sampled_cell"]
-
-
-@ut.timed_call()
-@ut.expand_doc(masks=", ".join(CLEAN_CELLS_MASKS))
-def pick_clean_cells(  # pylint: disable=dangerous-default-value
-    adata: AnnData, *, masks: List[str] = CLEAN_CELLS_MASKS, to: str = "clean_cell"
-) -> None:
-    """
-    Create a mask of the "clean" cells that will be used to actually compute the metacells.
-
-    **Input**
-
-    Annotated ``adata``, where the observations are cells and the variables are genes.
-
-    **Returns**
-
-    Sets the following in the data:
-
-    Observation (cell) annotations:
-        ``to`` (default: {to})
-            A mask of the "clean" cells to use for actually computing the metacells.
-
-    **Computation Parameters**
-
-    1. This simply AND-s the specified ``masks`` (default: {masks}) using
-       :py:func:`metacells.tools.mask.combine_masks`.
-    """
-    tl.combine_masks(adata, masks, to=to)
+    excluded_cells_masks = ["|~properly_sampled_cell"] + (additional_cells_masks or [])
+    tl.combine_masks(adata, excluded_cells_masks, to="excluded_cell")
 
 
 @ut.logged()
 @ut.timed_call()
 @ut.expand_doc()
 def extract_clean_data(
     adata: AnnData,
-    obs_mask: str = "clean_cell",
-    var_mask: str = "clean_gene",
     *,
     name: Optional[str] = ".clean",
     top_level: bool = True,
 ) -> Optional[AnnData]:
     """
     Extract a "clean" subset of the ``adata`` to compute metacells for.
 
+    .. todo::
+
+        Allow computing metacells on the full data, obeying the ``excluded_cell`` and ``excluded_gene`` masks.
+
     **Input**
 
-    Annotated ``adata``, where the observations are cells and the variables are genes.
+    Annotated ``adata``, where the observations are cells and the variables are genes. This may contain per-gene
+    ``excluded_gene`` and per-cell ``excluded_cell`` annotations.
 
     **Returns**
 
-    Annotated sliced data containing the "clean" subset of the original data. By default, the
-    ``name`` of this data is {name}. If this starts with a ``.``, this will be appended to the
-    current name of the data (if any).
+    Annotated sliced data containing the "clean" subset of the original data (that is, everything not
+    marked as excluded).
 
-    The returned data will have ``full_cell_index`` and ``full_gene_index`` per-observation (cell)
-    and per-variable (gene) annotations to allow mapping the results back to the original data.
+    The returned data will have ``full_cell_index`` and ``full_gene_index`` per-observation (cell) and per-variable
+    (gene) annotations to allow mapping the results back to the original data.
 
     **Computation Parameters**
 
-    1. This simply :py:func:`metacells.tools.filter.filter_data` to slice just the
-       ``obs_mask`` (default: {obs_mask}) and ``var_mask`` (default: {var_mask}) data using the
-       ``name`` (default: {name}), and tracking the original ``full_cell_index`` and
-       ``full_gene_index``.
+    1. This simply :py:func:`metacells.tools.filter.filter_data` to slice just the genes not in the ``excluded_gene``
+       mask and the cells not in the ``excluded_cell`` mask, data using the ``name`` (default: {name}), and tracking the
+       original ``full_cell_index`` and ``full_gene_index``.
     """
     results = tl.filter_data(
         adata,
         name=name,
         top_level=top_level,
         track_obs="full_cell_index",
         track_var="full_gene_index",
-        obs_masks=[obs_mask],
-        var_masks=[var_mask],
+        obs_masks=["&~excluded_cell?"],
+        var_masks=["&~excluded_gene?"],
     )
+
     if results is None:
         return None
-
     return results[0]
```

### Comparing `metacells-0.8.0/metacells/pipeline/consistency.py` & `metacells-0.9.0/metacells/pipeline/consistency.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 """
 Split
 -----
 """
 
-from re import Pattern
-from typing import Collection
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 from anndata import AnnData  # type: ignore
 
@@ -28,35 +26,31 @@
 @ut.timed_call()
 @ut.expand_doc()
 def split_groups(
     adata: AnnData,
     what: Union[str, ut.Matrix] = "__x__",
     *,
     group: str = "metacell",
-    feature_downsample_min_samples: int = pr.feature_downsample_min_samples,
-    feature_downsample_min_cell_quantile: float = pr.feature_downsample_min_cell_quantile,
-    feature_downsample_max_cell_quantile: float = pr.feature_downsample_max_cell_quantile,
-    feature_min_gene_total: Optional[int] = None,
-    feature_min_gene_top3: Optional[int] = None,
-    feature_min_gene_relative_variance: Optional[float] = pr.feature_min_gene_relative_variance,
-    forbidden_gene_names: Optional[Collection[str]] = None,
-    forbidden_gene_patterns: Optional[Collection[Union[str, Pattern]]] = None,
-    cells_similarity_value_normalization: float = pr.cells_similarity_value_normalization,
+    select_downsample_min_samples: int = pr.select_downsample_min_samples,
+    select_downsample_min_cell_quantile: float = pr.select_downsample_min_cell_quantile,
+    select_downsample_max_cell_quantile: float = pr.select_downsample_max_cell_quantile,
+    select_min_gene_total: Optional[int] = None,
+    select_min_gene_top3: Optional[int] = None,
+    select_min_gene_relative_variance: Optional[float] = pr.select_min_gene_relative_variance,
+    cells_similarity_value_regularization: float = pr.cells_similarity_value_regularization,
     cells_similarity_log_data: bool = pr.cells_similarity_log_data,
     cells_similarity_method: str = pr.cells_similarity_method,
-    max_cell_size: Optional[float] = pr.max_cell_size,
-    max_cell_size_factor: Optional[float] = pr.max_cell_size_factor,
     knn_balanced_ranks_factor: float = pr.knn_balanced_ranks_factor,
     knn_incoming_degree_factor: float = pr.knn_incoming_degree_factor,
     knn_outgoing_degree_factor: float = pr.knn_outgoing_degree_factor,
     min_seed_size_quantile: float = pr.min_seed_size_quantile,
     max_seed_size_quantile: float = pr.max_seed_size_quantile,
     candidates_cooldown_pass: float = pr.cooldown_pass,
     candidates_cooldown_node: float = pr.cooldown_node,
-    random_seed: int = pr.random_seed,
+    random_seed: int,
 ) -> None:
     """
     Split each metacell into two parts using ``what`` (default: {what}) data.
 
     This creates a new partition of cells into half-metacells, which can used to
     :py:func:`compute_groups_self_consistency`.
 
@@ -95,54 +89,50 @@
         assert np.any(group_cells_mask)
         name = f".{group}-{group_index}/{groups_count}"
         gdata = ut.slice(adata, name=name, top_level=False, obs=group_cells_mask, track_obs="complete_cell_index")
         target_metacell_size = (gdata.n_obs + 1) // 2
         compute_direct_metacells(
             gdata,
             what,
-            feature_downsample_min_samples=feature_downsample_min_samples,
-            feature_downsample_min_cell_quantile=feature_downsample_min_cell_quantile,
-            feature_downsample_max_cell_quantile=feature_downsample_max_cell_quantile,
-            feature_min_gene_total=feature_min_gene_total,
-            feature_min_gene_top3=feature_min_gene_top3,
-            feature_min_gene_relative_variance=feature_min_gene_relative_variance,
-            forbidden_gene_names=forbidden_gene_names,
-            forbidden_gene_patterns=forbidden_gene_patterns,
-            cells_similarity_value_normalization=cells_similarity_value_normalization,
+            select_downsample_min_samples=select_downsample_min_samples,
+            select_downsample_min_cell_quantile=select_downsample_min_cell_quantile,
+            select_downsample_max_cell_quantile=select_downsample_max_cell_quantile,
+            select_min_gene_total=select_min_gene_total,
+            select_min_gene_top3=select_min_gene_top3,
+            select_min_gene_relative_variance=select_min_gene_relative_variance,
+            cells_similarity_value_regularization=cells_similarity_value_regularization,
             cells_similarity_log_data=cells_similarity_log_data,
             cells_similarity_method=cells_similarity_method,
             target_metacell_size=target_metacell_size,
-            max_cell_size=max_cell_size,
-            max_cell_size_factor=max_cell_size_factor,
             cell_sizes=None,
             knn_k=target_metacell_size,
             min_knn_k=target_metacell_size,
             knn_balanced_ranks_factor=knn_balanced_ranks_factor,
             knn_incoming_degree_factor=knn_incoming_degree_factor,
             knn_outgoing_degree_factor=knn_outgoing_degree_factor,
             min_seed_size_quantile=min_seed_size_quantile,
             max_seed_size_quantile=max_seed_size_quantile,
             candidates_cooldown_pass=candidates_cooldown_pass,
             candidates_cooldown_node=candidates_cooldown_node,
-            candidates_min_split_size_factor=None,
-            candidates_max_merge_size_factor=None,
+            candidates_min_split_size_factor=1e6,
+            candidates_max_merge_size_factor=1e-6,
             candidates_min_metacell_cells=1,
             must_complete_cover=True,
             random_seed=random_seed,
         )
         direct_groups = ut.get_o_numpy(gdata, "metacell")
         zero_count = np.sum(direct_groups == 0)
         one_count = np.sum(direct_groups == 1)
         ut.log_calc(f"group: {group_index} size: {len(direct_groups)} " f"split into: {zero_count} + {one_count}")
         assert zero_count + one_count == len(direct_groups)
         assert zero_count > 0
         assert one_count > 0
         return (group_cells_mask, group_index + groups_count * direct_groups)
 
-    for (group_cells_mask, group_cells_halves) in ut.parallel_map(split_group, groups_count):
+    for group_cells_mask, group_cells_halves in ut.parallel_map(split_group, groups_count):
         half_groups_of_cells[group_cells_mask] = group_cells_halves
 
     ut.set_o_data(adata, f"half_{group}", half_groups_of_cells, formatter=ut.groups_description)
 
 
 @ut.logged()
 @ut.timed_call()
@@ -150,17 +140,17 @@
 def compute_groups_self_consistency(
     adata: AnnData,
     what: Union[str, ut.Matrix] = "__x__",
     *,
     group: str = "metacell",
     genes_mask: Optional[ut.NumpyVector] = None,
     self_similarity_log_data: bool = pr.self_similarity_log_data,
-    self_similarity_value_normalization: float = pr.self_similarity_value_normalization,
+    self_similarity_value_regularization: float = pr.self_similarity_value_regularization,
     self_similarity_method: str = pr.self_similarity_method,
-    reproducible: bool = pr.reproducible,
+    reproducible: bool,
     logistics_location: float = pr.logistics_location,
     logistics_slope: float = pr.logistics_slope,
 ) -> ut.NumpyVector:
     """
     Compute the self consistency (similarity between two halves) of some groups.
 
     **Input**
@@ -179,31 +169,31 @@
 
     1. For each group, compute the sum of values in each half and normalize it to fractions (sum of 1).
 
     2. If ``genes_mask`` is specified, select only the genes specified in it. Note the sum of the
        fractions of the genes of each group in the result will be less than or equal to 1.
 
     3. If ``self_similarity_log_data`` (default: {self_similarity_log_data}), log2 the values using
-       ``self_similarity_value_normalization`` (default: {self_similarity_value_normalization}).
+       ``self_similarity_value_regularization`` (default: {self_similarity_value_regularization}).
 
     4. Compute the ``self_similarity_method`` (default: {self_similarity_method}) between the two
        halves. If this is the ``logistics`` similarity, then this will use ``logistics_location``
        (default: {logistics_location}) and ``logistics_slope`` (default: {logistics_slope}). If this
-       is ``pearson``, and if ``reproducible`` (default: {reproducible}) is ``True``, a slower
+       is ``pearson``, and if ``reproducible`` is ``True``, a slower
        (still parallel) but reproducible algorithm will be used to compute Pearson correlations.
     """
     hdata = tl.group_obs_data(adata, what, groups=f"half_{group}", name=".halves")
     assert hdata is not None
 
     sum_of_halves = ut.get_o_numpy(hdata, f"{what}|sum")
     halves_values = ut.to_numpy_matrix(ut.get_vo_proper(hdata, what, layout="row_major"))
     halves_data = ut.mustbe_numpy_matrix(ut.scale_by(halves_values, sum_of_halves, by="row"))
 
-    if self_similarity_value_normalization > 0:
-        halves_data += self_similarity_value_normalization
+    if self_similarity_value_regularization > 0:
+        halves_data += self_similarity_value_regularization
 
     if self_similarity_log_data:
         halves_data = ut.log_data(halves_data, base=2)
 
     if genes_mask is not None:
         halves_data = halves_data[:, genes_mask]
```

### Comparing `metacells-0.8.0/metacells/pipeline/direct.py` & `metacells-0.9.0/metacells/pipeline/direct.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,122 +1,118 @@
 """
 Direct
 ------
 """
 
-from re import Pattern
 from typing import Callable
-from typing import Collection
 from typing import Optional
 from typing import Union
 
 import numpy as np
 from anndata import AnnData  # type: ignore
 
 import metacells.parameters as pr
 import metacells.tools as tl
 import metacells.utilities as ut
 
-from .collect import compute_effective_cell_sizes
-from .feature import extract_feature_data
+from .select import extract_selected_data
 
 __all__ = [
     "compute_direct_metacells",
 ]
 
 try:
     from mypy_extensions import NamedArg
 
-    #: A function to correct the extracted feature values before computing cell-cell similarity.
+    #: A function to correct the extracted selected values before computing cell-cell similarity.
     #:
     #: This function takes the following named arguments:
     #:
     #: ``adata`` - The full annotated data of the cells.
     #:
-    #: ``fdata`` - The feature genes annotated data of the cells (a slice of ``adata``). This has a
+    #: ``sdata`` - The selected genes annotated data of the cells (a slice of ``adata``). This has a
     #: ``downsample_samples`` unstructured annotation with the target number of samples per cell.
     #:
-    #: ``downsampled`` - A dense matrix of the downsampled UMIs of the features of the cells (a copy of the
-    #: ``downsampled`` layer of ``fdata``).
+    #: ``downsampled`` - A dense matrix of the downsampled UMIs of the selected genes of the cells (a copy of the
+    #: ``downsampled`` layer of ``sdata``).
     #:
     #: The function is free to modify ``downsampled`` as it sees fit to perform any type of correction (typically, some
     #: form of batch correction). The data type of ``downsampled`` is ``float32`` so the corrected values need not be
     #: integers (even though their initial values will be).
     #:
     #: Note that this is only invoked for metacells-of-cells by
     #: :py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline` or
     #: :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`, and is not invoked for
     #: computing groups of metacelles. Therefore the function can access any metadata of the original input.
     #:
     #: See :py:func:`compute_direct_metacells`.
     FeatureCorrection = Callable[
         [
             NamedArg(AnnData, "adata"),  # noqa: F821
-            NamedArg(AnnData, "fdata"),  # noqa: F821
+            NamedArg(AnnData, "sdata"),  # noqa: F821
             NamedArg(ut.NumpyMatrix, "downsampled"),  # noqa: F821
         ],
         None,
     ]
 
 except ModuleNotFoundError:
     FeatureCorrection = Callable  # type: ignore
 
 
 @ut.logged()
 @ut.timed_call()
 @ut.expand_doc()
-def compute_direct_metacells(  # pylint: disable=too-many-statements,too-many-branches
+def compute_direct_metacells(  # pylint: disable=too-many-branches,too-many-statements
     adata: AnnData,
     what: Union[str, ut.Matrix] = "__x__",
     *,
-    feature_downsample_min_samples: int = pr.feature_downsample_min_samples,
-    feature_downsample_min_cell_quantile: float = pr.feature_downsample_min_cell_quantile,
-    feature_downsample_max_cell_quantile: float = pr.feature_downsample_max_cell_quantile,
-    feature_min_gene_total: Optional[int] = pr.feature_min_gene_total,
-    feature_min_gene_top3: Optional[int] = pr.feature_min_gene_top3,
-    feature_min_gene_relative_variance: Optional[float] = pr.feature_min_gene_relative_variance,
-    feature_gene_names: Optional[Collection[str]] = None,
-    feature_gene_patterns: Optional[Collection[Union[str, Pattern]]] = None,
-    forbidden_gene_names: Optional[Collection[str]] = None,
-    forbidden_gene_patterns: Optional[Collection[Union[str, Pattern]]] = None,
-    feature_correction: Optional[FeatureCorrection] = None,
-    cells_similarity_value_normalization: float = pr.cells_similarity_value_normalization,
+    select_downsample_min_samples: int = pr.select_downsample_min_samples,
+    select_downsample_min_cell_quantile: float = pr.select_downsample_min_cell_quantile,
+    select_downsample_max_cell_quantile: float = pr.select_downsample_max_cell_quantile,
+    select_min_gene_total: Optional[int] = pr.select_min_gene_total,
+    select_min_gene_top3: Optional[int] = pr.select_min_gene_top3,
+    select_min_gene_relative_variance: Optional[float] = pr.select_min_gene_relative_variance,
+    select_correction: Optional[FeatureCorrection] = None,
+    cells_similarity_value_regularization: float = pr.cells_similarity_value_regularization,
     cells_similarity_log_data: bool = pr.cells_similarity_log_data,
     cells_similarity_method: str = pr.cells_similarity_method,
     target_metacell_size: float = pr.target_metacell_size,
-    max_cell_size: Optional[float] = pr.max_cell_size,
-    max_cell_size_factor: Optional[float] = pr.max_cell_size_factor,
     cell_sizes: Optional[Union[str, ut.Vector]] = pr.cell_sizes,
     knn_k: Optional[int] = pr.knn_k,
+    knn_k_size_factor: float = pr.candidates_knn_k_size_factor,
+    knn_k_size_quantile: float = pr.knn_k_size_quantile,
     min_knn_k: Optional[int] = pr.min_knn_k,
     knn_balanced_ranks_factor: float = pr.knn_balanced_ranks_factor,
     knn_incoming_degree_factor: float = pr.knn_incoming_degree_factor,
     knn_outgoing_degree_factor: float = pr.knn_outgoing_degree_factor,
-    candidates_cell_seeds: Optional[Union[str, ut.Vector]] = None,
     min_seed_size_quantile: float = pr.min_seed_size_quantile,
     max_seed_size_quantile: float = pr.max_seed_size_quantile,
     candidates_cooldown_pass: float = pr.cooldown_pass,
     candidates_cooldown_node: float = pr.cooldown_node,
     candidates_cooldown_phase: float = pr.cooldown_phase,
-    candidates_min_split_size_factor: Optional[float] = pr.candidates_min_split_size_factor,
-    candidates_max_merge_size_factor: Optional[float] = pr.candidates_max_merge_size_factor,
-    candidates_min_metacell_cells: Optional[int] = pr.min_metacell_cells,
+    candidates_min_split_size_factor: float = pr.candidates_min_split_size_factor,
+    candidates_max_merge_size_factor: float = pr.candidates_max_merge_size_factor,
+    candidates_min_metacell_cells: Optional[int] = pr.candidates_min_metacell_cells,
     candidates_max_split_min_cut_strength: Optional[float] = pr.max_split_min_cut_strength,
-    candidates_min_cut_seed_cells: Optional[int] = pr.min_cut_seed_cells,
+    candidates_min_cut_seed_cells: int = pr.min_cut_seed_cells,
     must_complete_cover: bool = False,
+    deviants_policy: str = pr.deviants_policy,
     deviants_min_gene_fold_factor: float = pr.deviants_min_gene_fold_factor,
-    deviants_abs_folds: bool = pr.deviants_abs_folds,
-    deviants_max_gene_fraction: Optional[float] = pr.deviants_max_gene_fraction,
+    deviants_gap_skip_cells: int = pr.deviants_gap_skip_cells,
+    deviants_min_noisy_gene_fold_factor: float = pr.deviants_min_noisy_gene_fold_factor,
+    deviants_max_gene_fraction: float = pr.deviants_max_gene_fraction,
     deviants_max_cell_fraction: Optional[float] = pr.deviants_max_cell_fraction,
+    deviants_max_gap_cells_count: int = pr.deviants_max_gap_cells_count,
+    deviants_max_gap_cells_fraction: float = pr.deviants_max_gap_cells_fraction,
     dissolve_min_robust_size_factor: Optional[float] = pr.dissolve_min_robust_size_factor,
     dissolve_min_convincing_size_factor: Optional[float] = pr.dissolve_min_convincing_size_factor,
     dissolve_min_convincing_gene_fold_factor: float = pr.dissolve_min_convincing_gene_fold_factor,
     dissolve_min_metacell_cells: int = pr.dissolve_min_metacell_cells,
-    random_seed: int = pr.random_seed,
-) -> AnnData:
+    random_seed: int,
+) -> None:
     """
     Directly compute metacells using ``what`` (default: {what}) data.
 
     This directly computes the metacells on the whole data. Like any method that directly looks at
     the whole data at once, the amount of CPU and memory needed becomes unreasonable when the data
     size grows. Above O(10,000) you are much better off using the divide-and-conquer method.
 
@@ -148,281 +144,235 @@
     are genes, where ``what`` is a per-variable-per-observation matrix or the name of a
     per-variable-per-observation annotation containing such a matrix.
 
     **Returns**
 
     Sets the following annotations in ``adata``:
 
+    Unstructured Annotations
+        ``downsample_samples``
+            The target total number of samples in each downsampled cell.
+
+    Observation-Variable (Cell-Gene) Annotations:
+        ``downsampled``
+            The downsampled data where the total number of samples in each cell is at most ``downsample_samples``.
+
     Variable (Gene) Annotations
         ``high_total_gene``
-            A boolean mask of genes with "high" expression level.
+            A boolean mask of genes with "high" expression level (unless a ``select_gene`` mask exists).
 
         ``high_relative_variance_gene``
-            A boolean mask of genes with "high" normalized variance, relative to other genes with a
-            similar expression level.
+            A boolean mask of genes with "high" normalized variance, relative to other genes with a similar expression
+            level (unless a ``select_gene`` mask exists).
 
-        ``forbidden_gene``
-            A boolean mask of genes which are forbidden from being chosen as "feature" genes based
-            on their name.
-
-        ``feature_gene``
-            A boolean mask of the "feature" genes.
-
-        ``gene_deviant_votes``
-            The number of cells each gene marked as deviant (if zero, the gene did not mark any cell
-            as deviant). This will be zero for non-"feature" genes.
+        ``selected_gene``
+            A boolean mask of the actually selected genes.
 
     Observation (Cell) Annotations
-        ``seed``
-            The index of the seed metacell each cell was assigned to to. This is ``-1`` for
-            non-"clean" cells.
-
-        ``candidate``
-            The index of the candidate metacell each cell was assigned to to. This is ``-1`` for
-            non-"clean" cells.
-
-        ``cell_deviant_votes``
-            The number of genes that were the reason the cell was marked as deviant (if zero, the
-            cell is not deviant).
-
-        ``dissolved``
-            A boolean mask of the cells contained in a dissolved metacell.
-
         ``metacell``
             The integer index of the metacell each cell belongs to. The metacells are in no
             particular order. Cells with no metacell assignment ("outliers") are given a metacell
             index of ``-1``.
 
-        ``outlier``
-            A boolean mask of the cells contained in no metacell.
-
     **Computation Parameters**
 
-    1. Invoke :py:func:`metacells.pipeline.feature.extract_feature_data` to extract "feature" data
+    1. Invoke :py:func:`metacells.pipeline.select.extract_selected_data` to extract "select" data
        from the clean data, using the
-       ``feature_downsample_min_samples`` (default: {feature_downsample_min_samples}),
-       ``feature_downsample_min_cell_quantile`` (default: {feature_downsample_min_cell_quantile}),
-       ``feature_downsample_max_cell_quantile`` (default: {feature_downsample_max_cell_quantile}),
-       ``feature_min_gene_total`` (default: {feature_min_gene_total}), ``feature_min_gene_top3``
-       (default: {feature_min_gene_top3}), ``feature_min_gene_relative_variance`` (default:
-       {feature_min_gene_relative_variance}), ``feature_gene_names`` (default:
-       {feature_gene_names}), ``feature_gene_patterns`` (default: {feature_gene_patterns}),
-       ``forbidden_gene_names`` (default: {forbidden_gene_names}), ``forbidden_gene_patterns``
-       (default: {forbidden_gene_patterns}) and ``random_seed`` (default: {random_seed}) to make
-       this replicable.
+       ``select_downsample_min_samples`` (default: {select_downsample_min_samples}),
+       ``select_downsample_min_cell_quantile`` (default: {select_downsample_min_cell_quantile}),
+       ``select_downsample_max_cell_quantile`` (default: {select_downsample_max_cell_quantile}),
+       ``select_min_gene_total`` (default: {select_min_gene_total}),
+       ``select_min_gene_top3`` (default: {select_min_gene_top3}),
+       ``select_min_gene_relative_variance`` (default: {select_min_gene_relative_variance}) and
+       ``random_seed``.
 
-    2. Apply the ``feature_correction`` function, if any, to modify the downsampled features data.
+    2. Apply the ``select_correction`` function, if any, to modify the downsampled selects data.
 
     3. Compute the fractions of each variable in each cell, and add the
-       ``cells_similarity_value_normalization`` (default: {cells_similarity_value_normalization}) to
+       ``cells_similarity_value_regularization`` (default: {cells_similarity_value_regularization}) to
        it.
 
     4. If ``cells_similarity_log_data`` (default: {cells_similarity_log_data}), invoke the
        :py:func:`metacells.utilities.computation.log_data` function to compute the log (base 2) of
        the data.
 
     5. Invoke :py:func:`metacells.tools.similarity.compute_obs_obs_similarity` to compute the
        similarity between each pair of cells, using the
        ``cells_similarity_method`` (default: {cells_similarity_method}).
 
-    6. Invoke :py:func:`metacells.pipeline.collect.compute_effective_cell_sizes` using
-       ``max_cell_size`` (default: {max_cell_size}), ``max_cell_size_factor`` (default:
-       {max_cell_size_factor}) and ``cell_sizes`` (default: {cell_sizes}) to get the effective cell
-       sizes to use.
-
-    7. Invoke :py:func:`metacells.tools.knn_graph.compute_obs_obs_knn_graph` to compute a
-       K-Nearest-Neighbors graph, using the
-       ``knn_balanced_ranks_factor`` (default: {knn_balanced_ranks_factor}),
-       ``knn_incoming_degree_factor`` (default: {knn_incoming_degree_factor})
-       and
-       ``knn_outgoing_degree_factor`` (default: {knn_outgoing_degree_factor}).
-       If ``knn_k`` (default: {knn_k}) is not specified, then it is
-       chosen to be the median number of cells required to reach the target metacell size,
-       but at least ``min_knn_k`` (default: {min_knn_k}).
+    6. Invoke :py:func:`metacells.tools.knn_graph.compute_obs_obs_knn_graph` to compute a K-Nearest-Neighbors graph,
+       using the ``knn_balanced_ranks_factor`` (default: {knn_balanced_ranks_factor}), ``knn_incoming_degree_factor``
+       (default: {knn_incoming_degree_factor}) and ``knn_outgoing_degree_factor`` (default:
+       {knn_outgoing_degree_factor}). If ``knn_k`` (default: {knn_k}) is not specified, then it is chosen to be the
+       ``knn_k_size_factor`` (default: {knn_k_size_factor} times the median number of cells required to reach the target
+       metacell size, or the ``knn_k_size_quantile`` (default: {knn_k_size_quantile}) the number of cells required, or
+       ``min_knn_k`` (default: {min_knn_k}), whichever is largest.
 
-    8. Invoke :py:func:`metacells.tools.candidates.compute_candidate_metacells` to compute
+    7. Invoke :py:func:`metacells.tools.candidates.compute_candidate_metacells` to compute
        the candidate metacells, using the
-       ``candidates_cell_seeds`` (default: {candidates_cell_seeds}),
        ``min_seed_size_quantile`` (default: {min_seed_size_quantile}),
        ``max_seed_size_quantile`` (default: {max_seed_size_quantile}),
        ``candidates_cooldown_pass`` (default: {candidates_cooldown_pass}),
        ``candidates_cooldown_node`` (default: {candidates_cooldown_node}),
        ``candidates_cooldown_phase`` (default: {candidates_cooldown_phase}),
        ``candidates_min_split_size_factor`` (default: {candidates_min_split_size_factor}),
        ``candidates_max_merge_size_factor`` (default: {candidates_max_merge_size_factor}),
        ``candidates_min_metacell_cells`` (default: {candidates_min_metacell_cells}),
        and
-       ``random_seed`` (default: {random_seed})
-       to make this replicable. This tries to build metacells of the
+       ``random_seed``. This tries to build metacells of the
        ``target_metacell_size`` (default: {target_metacell_size})
        using the effective cell sizes.
 
-    9. Unless ``must_complete_cover`` (default: {must_complete_cover}), invoke
+    8. Unless ``must_complete_cover`` (default: {must_complete_cover}), invoke
        :py:func:`metacells.tools.deviants.find_deviant_cells` to remove deviants from the candidate
        metacells, using the
+       ``deviants_policy`` (default: {deviants_policy}),
        ``deviants_min_gene_fold_factor`` (default: {deviants_min_gene_fold_factor}),
-       ``deviants_abs_folds`` (default: {deviants_abs_folds}),
+       ``deviants_gap_skip_cells`` (default: {deviants_gap_skip_cells}),
+       ``deviants_min_noisy_gene_fold_factor`` (default: {deviants_min_noisy_gene_fold_factor}),
        ``deviants_max_gene_fraction`` (default: {deviants_max_gene_fraction})
        and
        ``deviants_max_cell_fraction`` (default: {deviants_max_cell_fraction}).
 
-    10. Unless ``must_complete_cover`` (default: {must_complete_cover}), invoke
+    9. Unless ``must_complete_cover`` (default: {must_complete_cover}), invoke
        :py:func:`metacells.tools.dissolve.dissolve_metacells` to dissolve small unconvincing
        metacells, using the same
        ``target_metacell_size`` (default: {target_metacell_size}),
        and the effective cell sizes
        and the
        ``dissolve_min_robust_size_factor`` (default: {dissolve_min_robust_size_factor}),
        ``dissolve_min_convincing_size_factor`` (default: {dissolve_min_convincing_size_factor}),
        ``dissolve_min_convincing_gene_fold_factor`` (default: {dissolve_min_convincing_size_factor})
        and
        ``dissolve_min_metacell_cells`` (default: ``dissolve_min_metacell_cells``).
     """
-    fdata = extract_feature_data(
-        adata,
-        what,
-        top_level=False,
-        downsample_min_samples=feature_downsample_min_samples,
-        downsample_min_cell_quantile=feature_downsample_min_cell_quantile,
-        downsample_max_cell_quantile=feature_downsample_max_cell_quantile,
-        min_gene_relative_variance=feature_min_gene_relative_variance,
-        min_gene_total=feature_min_gene_total,
-        min_gene_top3=feature_min_gene_top3,
-        forced_gene_names=feature_gene_names,
-        forced_gene_patterns=feature_gene_patterns,
-        forbidden_gene_names=forbidden_gene_names,
-        forbidden_gene_patterns=forbidden_gene_patterns,
-        random_seed=random_seed,
-    )
-
-    if fdata is None:
-        raise ValueError("Empty feature data, giving up")
-
-    effective_cell_sizes, max_cell_size, _cell_scale_factors = compute_effective_cell_sizes(
-        adata, max_cell_size=max_cell_size, max_cell_size_factor=max_cell_size_factor, cell_sizes=cell_sizes
-    )
-    ut.log_calc("effective_cell_sizes", effective_cell_sizes, formatter=ut.sizes_description)
-
-    if max_cell_size is not None:
-        if candidates_min_metacell_cells is not None:
-            target_metacell_size = max(target_metacell_size, max_cell_size * candidates_min_metacell_cells)
-
-        if dissolve_min_metacell_cells is not None:
-            target_metacell_size = max(target_metacell_size, max_cell_size * dissolve_min_metacell_cells)
-
-        if candidates_min_metacell_cells is not None or dissolve_min_metacell_cells is not None:
-            ut.log_calc("target_metacell_size", target_metacell_size)
-
-    data = ut.get_vo_proper(fdata, "downsampled", layout="row_major")
-    data = ut.to_numpy_matrix(data, copy=True)
-
-    if feature_correction is not None:
-        feature_correction(adata=adata, fdata=fdata, downsampled=data)
-
-    if cells_similarity_value_normalization > 0:
-        data += cells_similarity_value_normalization
-
-    if cells_similarity_log_data:
-        data = ut.log_data(data, base=2)
-
-    if knn_k is None:
-        if effective_cell_sizes is None:
-            median_cell_size = 1.0
-        else:
-            median_cell_size = float(np.median(effective_cell_sizes))
-        knn_k = int(round(target_metacell_size / median_cell_size))
-        if min_knn_k is not None:
-            knn_k = max(knn_k, min_knn_k)
-
-    if knn_k == 0:
-        ut.log_calc("knn_k: 0 (too small, try single metacell)")
-        ut.set_o_data(fdata, "candidate", np.full(fdata.n_obs, 0, dtype="int32"), formatter=lambda _: "* <- 0")
-    elif knn_k >= fdata.n_obs:
-        ut.log_calc(f"knn_k: {knn_k} (too large, try single metacell)")
-        ut.set_o_data(fdata, "candidate", np.full(fdata.n_obs, 0, dtype="int32"), formatter=lambda _: "* <- 0")
-
+    assert (
+        target_metacell_size < 1000 or cell_sizes is not None
+    ), f"target_metacell_size: {target_metacell_size} seems to be in UMIs, should be in cells"
+
+    cell_sizes = ut.maybe_o_numpy(adata, cell_sizes, formatter=ut.sizes_description)
+    if cell_sizes is not None:
+        ut.log_calc("cell_sizes", cell_sizes, formatter=ut.sizes_description)
+        is_small = np.sum(cell_sizes) <= target_metacell_size * candidates_min_split_size_factor
     else:
-        ut.log_calc("knn_k", knn_k)
-
-        tl.compute_obs_obs_similarity(fdata, data, method=cells_similarity_method, reproducible=(random_seed != 0))
+        is_small = adata.n_obs <= target_metacell_size * candidates_min_split_size_factor
+    ut.log_calc("is_small", is_small)
 
-        tl.compute_obs_obs_knn_graph(
-            fdata,
-            k=knn_k,
-            balanced_ranks_factor=knn_balanced_ranks_factor,
-            incoming_degree_factor=knn_incoming_degree_factor,
-            outgoing_degree_factor=knn_outgoing_degree_factor,
-        )
+    if is_small:
+        candidate_of_cells = np.zeros(adata.n_obs, dtype="int32")
+        ut.set_v_data(adata, "selected_gene", np.zeros(adata.n_vars, dtype="bool"))
 
-        tl.compute_candidate_metacells(
-            fdata,
-            target_metacell_size=target_metacell_size,
-            cell_sizes=effective_cell_sizes,
-            cell_seeds=candidates_cell_seeds,
-            min_seed_size_quantile=min_seed_size_quantile,
-            max_seed_size_quantile=max_seed_size_quantile,
-            cooldown_pass=candidates_cooldown_pass,
-            cooldown_node=candidates_cooldown_node,
-            cooldown_phase=candidates_cooldown_phase,
-            min_split_size_factor=candidates_min_split_size_factor,
-            max_merge_size_factor=candidates_max_merge_size_factor,
-            min_metacell_cells=candidates_min_metacell_cells,
-            max_split_min_cut_strength=candidates_max_split_min_cut_strength,
-            min_cut_seed_cells=candidates_min_cut_seed_cells,
-            must_complete_cover=must_complete_cover,
+    else:
+        sdata = extract_selected_data(
+            adata,
+            what,
+            top_level=False,
+            downsample_min_samples=select_downsample_min_samples,
+            downsample_min_cell_quantile=select_downsample_min_cell_quantile,
+            downsample_max_cell_quantile=select_downsample_max_cell_quantile,
+            min_gene_relative_variance=select_min_gene_relative_variance,
+            min_gene_total=select_min_gene_total,
+            min_gene_top3=select_min_gene_top3,
             random_seed=random_seed,
         )
 
-        ut.set_oo_data(adata, "obs_similarity", ut.get_oo_proper(fdata, "obs_similarity"))
-
-        ut.set_oo_data(adata, "obs_outgoing_weights", ut.get_oo_proper(fdata, "obs_outgoing_weights"))
-
-        seed_of_cells = ut.get_o_numpy(fdata, "seed", formatter=ut.groups_description)
+        data = ut.get_vo_proper(sdata, "downsampled", layout="row_major")
+        data = ut.to_numpy_matrix(data, copy=True)
 
-        ut.set_o_data(adata, "seed", seed_of_cells, formatter=ut.groups_description)
+        if select_correction is not None:
+            select_correction(adata=adata, sdata=sdata, downsampled=data)
 
-    candidate_of_cells = ut.get_o_numpy(fdata, "candidate", formatter=ut.groups_description)
+        if cells_similarity_value_regularization > 0:
+            data += cells_similarity_value_regularization
 
-    ut.set_o_data(adata, "candidate", candidate_of_cells, formatter=ut.groups_description)
-
-    if must_complete_cover:
-        assert np.min(candidate_of_cells) == 0
+        if cells_similarity_log_data:
+            data = ut.log_data(data, base=2)
+
+        if knn_k is None:
+            if cell_sizes is None:
+                median_cell_size = 1.0
+                quantile_cell_size = 1.0
+            else:
+                median_cell_size = float(np.median(cell_sizes))
+                quantile_cell_size = np.quantile(cell_sizes, knn_k_size_quantile)
+            knn_k_of_median = int(round(target_metacell_size / median_cell_size))
+            knn_k_median = int(round(knn_k_size_factor * target_metacell_size / median_cell_size))
+            knn_k_quantile = int(round(target_metacell_size / quantile_cell_size))
+            ut.log_calc("median_cell_size", median_cell_size)
+            ut.log_calc("knn_k by median_cell_size", knn_k_median)
+            ut.log_calc("quantile_cell_size", quantile_cell_size)
+            ut.log_calc("knn_k by quantile_cell_size", knn_k_quantile)
+            knn_k = max(
+                int(round(knn_k_size_factor * target_metacell_size / median_cell_size)),
+                int(round(target_metacell_size / quantile_cell_size)),
+                min_knn_k or 0,
+            )
+
+        if knn_k == 0:
+            ut.log_calc("knn_k: 0 (too small, trying a single metacell)")
+            ut.set_o_data(sdata, "candidate", np.full(sdata.n_obs, 0, dtype="int32"), formatter=lambda _: "* <- 0")
+        elif knn_k_of_median >= sdata.n_obs:
+            ut.log_calc(f"knn_k of median: {knn_k_of_median} (too large, trying a single metacell)")
+            ut.set_o_data(sdata, "candidate", np.full(sdata.n_obs, 0, dtype="int32"), formatter=lambda _: "* <- 0")
 
-        deviant_votes_of_genes = np.zeros(adata.n_vars, dtype="float32")
-        deviant_votes_of_cells = np.zeros(adata.n_obs, dtype="float32")
-        dissolved_of_cells = np.zeros(adata.n_obs, dtype="bool")
+        else:
+            ut.log_calc("knn_k", knn_k)
 
-        ut.set_v_data(adata, "gene_deviant_votes", deviant_votes_of_genes, formatter=ut.mask_description)
+            tl.compute_obs_obs_similarity(sdata, data, method=cells_similarity_method, reproducible=random_seed != 0)
 
-        ut.set_o_data(adata, "cell_deviant_votes", deviant_votes_of_cells, formatter=ut.mask_description)
+            tl.compute_obs_obs_knn_graph(
+                sdata,
+                k=knn_k,
+                balanced_ranks_factor=knn_balanced_ranks_factor,
+                incoming_degree_factor=knn_incoming_degree_factor,
+                outgoing_degree_factor=knn_outgoing_degree_factor,
+            )
+
+            tl.compute_candidate_metacells(
+                sdata,
+                target_metacell_size=target_metacell_size,
+                cell_sizes=cell_sizes,
+                min_seed_size_quantile=min_seed_size_quantile,
+                max_seed_size_quantile=max_seed_size_quantile,
+                cooldown_pass=candidates_cooldown_pass,
+                cooldown_node=candidates_cooldown_node,
+                cooldown_phase=candidates_cooldown_phase,
+                min_split_size_factor=candidates_min_split_size_factor,
+                max_merge_size_factor=candidates_max_merge_size_factor,
+                min_metacell_cells=candidates_min_metacell_cells,
+                max_split_min_cut_strength=candidates_max_split_min_cut_strength,
+                min_cut_seed_cells=candidates_min_cut_seed_cells,
+                must_complete_cover=must_complete_cover,
+                random_seed=random_seed,
+            )
 
-        ut.set_o_data(adata, "dissolved", dissolved_of_cells, formatter=ut.mask_description)
+        candidate_of_cells = ut.get_o_numpy(sdata, "candidate", formatter=ut.groups_description)
 
+    if must_complete_cover:
+        assert np.min(candidate_of_cells) == 0
         ut.set_o_data(adata, "metacell", candidate_of_cells, formatter=ut.groups_description)
 
     else:
-        tl.find_deviant_cells(
+        deviants = tl.find_deviant_cells(
             adata,
             candidates=candidate_of_cells,
+            policy=deviants_policy,
             min_gene_fold_factor=deviants_min_gene_fold_factor,
-            abs_folds=deviants_abs_folds,
+            gap_skip_cells=deviants_gap_skip_cells,
+            min_noisy_gene_fold_factor=deviants_min_noisy_gene_fold_factor,
             max_gene_fraction=deviants_max_gene_fraction,
             max_cell_fraction=deviants_max_cell_fraction,
+            max_gap_cells_count=deviants_max_gap_cells_count,
+            max_gap_cells_fraction=deviants_max_gap_cells_fraction,
         )
 
         tl.dissolve_metacells(
             adata,
             candidates=candidate_of_cells,
+            deviants=deviants,
             target_metacell_size=target_metacell_size,
-            cell_sizes=effective_cell_sizes,
+            cell_sizes=cell_sizes,
             min_robust_size_factor=dissolve_min_robust_size_factor,
             min_convincing_size_factor=dissolve_min_convincing_size_factor,
             min_convincing_gene_fold_factor=dissolve_min_convincing_gene_fold_factor,
             min_metacell_cells=dissolve_min_metacell_cells,
         )
-
-        metacell_of_cells = ut.get_o_numpy(adata, "metacell", formatter=ut.groups_description)
-
-        outlier_of_cells = metacell_of_cells < 0
-        ut.set_o_data(adata, "outlier", outlier_of_cells, formatter=ut.mask_description)
-
-    return fdata
```

### Comparing `metacells-0.8.0/metacells/pipeline/projection.py` & `metacells-0.9.0/metacells/pipeline/projection.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,1810 +1,1783 @@
 """
 Projection
 ----------
 """
 
-from re import Pattern
+from math import ceil
 from typing import Any
-from typing import Collection
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Set
 from typing import Tuple
-from typing import Union
 
 import numpy as np
 import scipy.sparse as sp  # type: ignore
 from anndata import AnnData  # type: ignore
 
 import metacells.parameters as pr
 import metacells.tools as tl
 import metacells.utilities as ut
+from metacells import __version__  # pylint: disable=cyclic-import
 
 __all__ = [
     "projection_pipeline",
     "outliers_projection_pipeline",
+    "write_projection_weights",
 ]
 
 
 @ut.logged()
 @ut.timed_call()
 @ut.expand_doc()
 def projection_pipeline(
     what: str = "__x__",
     *,
     adata: AnnData,
     qdata: AnnData,
-    ignored_gene_names: Optional[Collection[str]] = None,
-    ignored_gene_patterns: Optional[Collection[Union[str, Pattern]]] = None,
-    ignore_atlas_insignificant_genes: bool = pr.ignore_atlas_insignificant_genes,
-    ignore_query_insignificant_genes: bool = pr.ignore_query_insignificant_genes,
-    ignore_atlas_forbidden_genes: bool = pr.ignore_atlas_forbidden_genes,
-    ignore_query_forbidden_genes: bool = pr.ignore_query_forbidden_genes,
-    systematic_low_gene_quantile: float = pr.systematic_low_gene_quantile,
-    systematic_high_gene_quantile: float = pr.systematic_high_gene_quantile,
-    biased_min_metacells_fraction: float = pr.biased_min_metacells_fraction,
-    project_fold_normalization: float = pr.project_fold_normalization,
+    only_atlas_marker_genes: bool = pr.only_atlas_marker_genes,
+    only_query_marker_genes: bool = pr.only_query_marker_genes,
+    ignore_atlas_lateral_genes: bool = pr.ignore_atlas_lateral_genes,
+    ignore_query_lateral_genes: bool = pr.ignore_query_lateral_genes,
+    consider_atlas_noisy_genes: bool = pr.consider_atlas_noisy_genes,
+    consider_query_noisy_genes: bool = pr.consider_query_noisy_genes,
+    misfit_min_metacells_fraction: float = pr.misfit_min_metacells_fraction,
+    project_log_data: bool = pr.project_log_data,
+    project_fold_regularization: float = pr.project_fold_regularization,
     project_candidates_count: int = pr.project_candidates_count,
-    project_min_significant_gene_value: float = pr.project_min_significant_gene_value,
+    project_min_candidates_fraction: float = pr.project_min_candidates_fraction,
+    project_min_significant_gene_umis: int = pr.project_min_significant_gene_umis,
     project_min_usage_weight: float = pr.project_min_usage_weight,
+    project_filter_ranges: bool = pr.project_filter_ranges,
+    project_ignore_range_quantile: float = pr.project_ignore_range_quantile,
+    project_ignore_range_min_overlap_fraction: float = pr.project_ignore_range_min_overlap_fraction,
+    project_min_query_markers_fraction: float = pr.project_min_query_markers_fraction,
     project_max_consistency_fold_factor: float = pr.project_max_consistency_fold_factor,
     project_max_projection_fold_factor: float = pr.project_max_projection_fold_factor,
-    project_max_dissimilar_genes: int = pr.project_max_dissimilar_genes,
-    min_entry_project_fold_factor: float = pr.min_entry_project_fold_factor,
-    project_abs_folds: bool = pr.project_abs_folds,
-    ignored_gene_names_of_type: Optional[Dict[str, Collection[str]]] = None,
-    ignored_gene_patterns_of_type: Optional[Dict[str, Collection[str]]] = None,
+    project_max_projection_noisy_fold_factor: float = pr.project_max_projection_noisy_fold_factor,
+    project_max_misfit_genes: int = pr.project_max_misfit_genes,
+    project_min_essential_genes_fraction: Optional[float] = pr.project_min_essential_genes_fraction,
     atlas_type_property_name: str = "type",
+    project_corrections: bool = pr.project_corrections,
     project_min_corrected_gene_correlation: float = pr.project_min_corrected_gene_correlation,
     project_min_corrected_gene_factor: float = pr.project_min_corrected_gene_factor,
-    project_max_uncorrelated_gene_correlation: float = pr.project_max_uncorrelated_gene_correlation,
-    renormalize_query_by_atlas: bool = pr.renormalize_query_by_atlas,
-    renormalize_var_annotations: Optional[Dict[str, Any]] = None,
-    renormalize_layers: Optional[Dict[str, Any]] = None,
-    renormalize_varp_annotations: Optional[Dict[str, Any]] = None,
     reproducible: bool,
     top_level_parallel: bool = True,
-) -> Tuple[ut.CompressedMatrix, AnnData]:
+) -> ut.CompressedMatrix:
     """
     Complete pipeline for projecting query metacells onto an atlas of metacells for the ``what`` (default: {what}) data.
 
     **Input**
 
     Annotated query ``qdata`` and atlas ``adata``, where the observations are cells and the variables are genes, where
     ``what`` is a per-variable-per-observation matrix or the name of a per-variable-per-observation annotation
-    containing such a matrix. The atlas should also contain a ``type`` per-observation (metacell) annotation.
+    containing such a matrix, containing the fraction of each gene in each cell. The atlas should also contain a
+    ``type`` per-observation (metacell) annotation.
+
+    The ``qdata`` may include per-gene masks, ``ignored_gene`` and ``ignored_gene_of_<type>``, which force the code
+    below to ignore the marked genes from either the preliminary projection or the following refined type-specific
+    projections.
 
     **Returns**
 
     A matrix whose rows are query metacells and columns are atlas metacells, where each entry is the weight of the atlas
     metacell in the projection of the query metacells. The sum of weights in each row (that is, for a single query
     metacell) is 1. The weighted sum of the atlas metacells using these weights is the "projected" image of the query
     metacell onto the atlas.
 
-    For "similar" query metacells (see below), these weights are all located in a small region of the atlas manifold.
-    For "dissimilar" query metacells, these weights will include atlas metacells in a secondary region of the atlas
-    attempting to cover the residual differences between the query and the main atlas manifold region. This tries to
-    identify doublets.
-
-    In addition, a modified version of ``qdata`` with a new ``ATLASNORM`` gene (if requested), and the following
-    additional annotations:
-
     Variable (Gene) Annotations
-        ``correction_factor``
-            The ratio between the original query and the corrected values (>1 if the gene was increased, <1 if it was
-            reduced).
-
-        ``projected_correlation``
-            For each gene, the correlation between the (corrected) query expression level and the projected expression
-            level.
-
-        ``correlated_gene``
-            A boolean mask of genes which were ignored because they were very correlated between the query and the
-            atlas.
-
-        ``uncorrelated_gene``
-            A boolean mask of genes which were ignored because they were too uncorrelated between the query and the
-            atlas.
-
-        ``systematic_gene``
-            A boolean mask indicating whether the gene is systematically higher or lower in the query compared to the
-            atlas.
-
-        ``biased_gene``
-            A boolean mask indicating whether the gene has a strong bias in the query compared to the atlas.
-
-        ``manually_ignored_gene``
-            A boolean mask indicating whether the gene was manually ignored (by its name).
-
         ``atlas_gene``
-            A boolean mask indicating whether the gene exists in the atlas.
-
-        ``atlas_significant_gene`` (``ignore_atlas_insignificant_genes`` requires an atlas ``significant_gene`` mask)
-            A boolean mask indicating whether the gene is considered significant in the atlas.
-
-        ``atlas_forbidden_gene`` (``ignore_atlas_forbidden_genes`` requires an atlas has ``forbidden_gene`` mask)
-            A boolean mask indicating whether the gene was forbidden from being a feature in the atlas (and hence
-            ignored).
-
-        ``ignored_gene``
-            A boolean mask indicating whether the gene was ignored by the projection (for any reason).
-
-        ``systematic_gene_of_<type>``
-            For each query metacell type, a boolean mask indicating whether the gene is systematically higher or lower
-            in the query metacells of this type compared to the atlas metacells of this type.
+            A mask of the query genes that also exist in the atlas. We match genes by their name; if projecting query
+            data from a different technology, we expect the caller to modify the query gene names to match the atlas
+            before projecting it.
+
+        ``atlas_lateral_gene``, ``atlas_noisy_gene``, ``atlas_marker_gene``, ``essential_gene_of_<type>``
+            Copied from the atlas to the query (``False`` for non-``atlas_gene``).
+
+        ``projected_noisy_gene``
+            The mask of the genes that were considered "noisy" when computing the projection. By default this is the
+            union of the noisy atlas and query genes.
+
+        ``correction_factor`` (if ``project_corrections``)
+            If projecting a query on an atlas with different technologies (e.g., 10X v3 to 10X v2), an automatically
+            computed factor we multiplied the query gene fractions by to compensate for the systematic difference
+            between the technologies (1.0 for uncorrected genes and 0.0 for non-``atlas_gene``).
+
+        ``fitted_gene_of_<type>``
+            For each type, the genes that were projected well from the query to the atlas for most cells of that
+            type; any ``atlas_gene`` outside this mask failed to project well from the query to the atlas for most
+            metacells of this type. For non-``atlas_gene`` this is set to ``False``.
 
-        ``biased_gene_of_<type>``
+        ``misfit_gene_of_<type>``
             For each query metacell type, a boolean mask indicating whether the gene has a strong bias in the query
             metacells of this type compared to the atlas metacells of this type.
 
-        ``manually_ignored_gene_of_<type>``
-            For each query metacell type, a boolean mask indicating whether the gene was manually ignored (by its name)
-            when computing the projection for metacells of this type.
-
         ``ignored_gene_of_<type>``
             For each query metacell type, a boolean mask indicating whether the gene was ignored by the projection (for
             any reason) when computing the projection for metacells of this type.
 
     Observation (Cell) Annotations
-        ``similar``
-            A boolean mask indicating whether the corrected query metacell is similar to its projection onto the atlas
-            (ignoring the ``ignored_genes``). If ``False`` the metacell is said to be "dissimilar", which may indicate
-            the query contains cell states that do not appear in the atlas. If ``True`` the metacell is said to be
-            "similar", but there may still be significant systematic differences between the query and the atlas as
-            captured by the various per-gene annotations. In addition, the projection on the atlas might indicate the
-            query metacell is a doublet combining two different points in the atlas (see below). In either case, being
-            "similar" doesn't guarantee we have a good query metacell that exists in the atlas.
-
-        ``dissimilar_genes_count``
-            The number of genes whose fold factor between the query metacell and its projection on the atlas is above
-            the threshold.
+        ``total_atlas_umis``
+            The total UMIs of the ``atlas_gene`` in each query metacell. This is used in the analysis as described for
+            ``total_umis`` above, that is, to ensure comparing expression levels will ignore cases where the total
+            number of UMIs of both compared gene profiles is too low to make a reliable determination. In such cases we
+            take the fold factor to be 0.
 
         ``projected_type``
-            The type assigned to each query metacell by its projection on the atlas. This should not be taken as gospel,
-            even for "similar" metacells, as there may still be significant systematic differences between the query and
-            the atlas as captured by the various per-gene annotations.
+            For each query metacell, the best atlas ``type`` we can assign to it based on its projection. Note this does
+            not indicate that the query metacell is "truly" of this type; to make this determination one needs to look
+            at the quality control data below.
 
         ``projected_secondary_type``
-            If the query metacell is "similar" to its projection to a single point in the atlas, this will be the empty
-            string. Otherwise, we try to project it using two distinct points in the atlas, in which case this would
-            contain the type associated with that second point. Thus, if a query metacell contains doublet cells, it
-            might end up being "similar" but to a combination of two types in the atlas. For a truly novel query
-            metacell type, this will also end up being "dissimilar", and the secondary type may or may not be helpful.
-            Also, even if the query metacell ends up being "similar" to a combination of two atlas points, this can be
-            either due to the query metacell containing true doublet cells, or possibly due to the atlas having
-            metacells that span some gradient where the query has only one metacell that covers a "too large" range of
-            this gradient (in this case the secondary type might even end up being the same as the main projected type).
-            In either case, having a non-empty value here doesn't guarantee this is a metacell of doublets.
+            In some cases, a query metacell may fail to project well to a single region of the atlas, but does project
+            well to a combination of two distinct atlas regions. This may be due to the query metacell containing
+            doublets, of a mixture of cells which match different atlas regions (e.g. due to sparsity of data in the
+            query data set). Either way, if this happens, we place here the type that best describes the secondary
+            region the query metacell was projected to; otherwise this would be the empty string. Note that the
+            ``weights`` matrix above does not distinguish between the regions.
+
+        ``projected_correlation`` per query metacell
+            The correlation between between the ``corrected_fraction`` and the ``projected_fraction`` for only the
+            ``fitted_gene`` expression levels of each query metacell. This serves as a very rough estimator for the
+            quality of the projection for this query metacell (e.g. can be used to compute R^2 values).
+
+            In general we expect high correlation (more than 0.9 in most metacells) since we restricted the
+            ``fitted_gene`` mask only to genes we projected well.
+
+        ``similar`` mask per query metacell
+            A conservative determination of whether the query metacell is "similar" to its projection on the atlas. This
+            is based on whether the number of ``misfit_gene`` for the query metacell is low enough (by default, up to 3
+            genes), and also that at least 75% of the ``essential_gene`` of the query metacell were not ``misfit_gene``.
+            Note that this explicitly allows for a ``projected_secondary_type``, that is, a metacell of doublets will be
+            "similar" to the atlas, but a metacell of a novel state missing from the atlas will be "dissimilar".
+
+            The final determination of whether to accept the projection is, as always, up to the analyst, based on prior
+            biological knowledge, the context of the collection of the query (and atlas) data sets, etc. The analyst
+            need not (indeed, *should not*) blindly accept the ``similar`` determination without examining the rest of
+            the quality control data listed above.
 
     Observation-Variable (Cell-Gene) Annotations
-        ``projected``
-            A matrix of UMIs where the sum of UMIs for each corrected query metacell is the same as the sum of ``what``
-            UMIs, describing the "projected" image of the query metacell onto the atlas. This projection is a weighted
-            average of some atlas metacells (using the computed weights returned by this function).
-
-        ``projected_fold``
-            For each gene and query metacell, the fold factor of this gene between the query and its projection (unless
-            the value is too low to be of interest, in which case it will be zero).
+        ``corrected_fraction`` per gene per query metacell
+            For each ``atlas_gene``, its fraction in each query metacell, out of only the atlas genes. This may be
+            further corrected (see below) if projecting between different scRNA-seq technologies (e.g. 10X v2 and 10X
+            v3). For non-``atlas_gene`` this is 0.
+
+        ``projected_fraction`` per gene per query metacell
+            For each ``atlas_gene``, its fraction in its projection on the atlas. This projection is computed as a
+            weighted average of some atlas metacells (see below), which are all sufficiently close to each other (in
+            terms of gene expression), so averaging them is reasonable to capture the fact the query metacell may be
+            along some position on some gradient that isn't an exact match for any specific atlas metacell. For
+            non-``atlas_gene`` this is 0.
+
+        ``fitted`` mask per gene per query metacell
+            For each ``atlas_gene`` for each query metacell, whether the gene was expected to be projected well, based
+            on the query metacell ``projected_type`` (and the ``projected_secondary_type``, if any). For
+            non-``atlas_gene`` this is set to ``False``. This does not guarantee the gene was actually projected well.
+
+        ``misfit``
+            For each ``atlas_gene`` for each query metacell, whether the ``corrected_fraction`` of the gene was
+            significantly different from the ``projected_fractions`` (that is, whether the gene was not projected well
+            for this metacell). For non-``atlas_gene`` this is set to ``False``, to make it easier to identify
+            problematic genes.
+
+            This is expected to be rare for ``fitted_gene`` and common for the rest of the ``atlas_gene``. If too many
+            ``fitted_gene`` are also ``misfit_gene``, then one should be suspicious whether the query metacell is
+            "truly" of the ``projected_type``.
+
+        ``essential``
+            Which of the ``atlas_gene`` were also listed in the ``essential_gene_of_<type>`` for the ``projected_type``
+            (and also the ``projected_secondary_type``, if any) of each query metacell.
+
+            If an ``essential_gene`` is also a ``misfit_gene``, then one should be very suspicious whether the query
+            metacell is "truly" of the ``projected_type``.
+
+        ``projected_fold`` per gene per query metacell
+            The fold factor between the ``corrected_fraction`` and the ``projected_fraction`` (0 for
+            non-``atlas_gene``). If the absolute value of this is high (3 for 8x ratio) then the gene was not projected
+            well for this metacell. This will be 0 for non-``atlas_gene``.
+
+            It is expected this would have low values for most ``fitted_gene`` and high values for the rest of the
+            ``atlas_gene``, but specific values will vary from one query metacell to another. This allows the analyst to
+            make fine-grained determination about the quality of the projection, and/or identify quantitative
+            differences between the query and the atlas (e.g., when studying perturbed systems such as knockouts or
+            disease models).
 
     **Computation Parameters**
 
     0. Find the subset of genes that exist in both the query and the atlas. All computations will be done on this common
-       subset.
+       subset. Normalize the fractions of the fitted gene fractions to sum to 1 in each metacell.
+
+    Compute preliminary projection:
 
-    1. Invoke :py:func:`metacells.tools.project.find_systematic_genes` using ``systematic_low_gene_quantile`` (default:
-       {systematic_low_gene_quantile}) and ``systematic_high_gene_quantile`` (default: {systematic_high_gene_quantile}).
+    1. Compute a mask of fitted genes, ignoring any genes included in ``ignored_gene``. If ``only_atlas_marker_genes``
+       (default: ``only_atlas_marker_genes``), ignore any non-``marker_gene`` of the atlas. If
+       ``only_query_marker_genes`` (default: ``only_query_marker_genes``), ignore any non-``marker_gene`` of the query.
+       If ``ignore_atlas_lateral_genes`` (default: {ignore_atlas_lateral_genes}), ignore the ``lateral_gene`` of the
+       atlas. If ``ignore_query_lateral_genes`` (default: {ignore_query_lateral_genes}), ignore the ``lateral_gene`` of
+       the atlas. Normalize the fractions of the fitted gene fractions to sum to 1 in each metacell.
+
+    2. Invoke :py:func:`metacells.tools.project.compute_projection_weights`
+       to project each query metacell onto the atlas, using the ``project_log_data`` (default: {project_log_data}),
+       ``project_fold_regularization`` (default: {project_fold_regularization}), ``project_min_significant_gene_umis``
+       (default: {project_min_significant_gene_umis}), ``project_max_consistency_fold_factor`` (default:
+       {project_max_consistency_fold_factor}), ``project_candidates_count`` (default: {project_candidates_count}),
+       ``project_min_usage_weight`` (default: {project_min_usage_weight}), and ``reproducible``.
 
-    2. Compute a mask of ignored genes, containing any genes named in ``ignored_gene_names`` or that match any of the
-       ``ignored_gene_patterns``. If ``ignore_atlas_insignificant_genes`` (default:
-       ``ignore_atlas_insignificant_genes``), ignore genes the atlas did not mark as significant (and store the
-       ``atlas_significant_gene`` mask). If ``ignore_query_insignificant_genes`` (default:
-       ``ignore_query_insignificant_genes``), ignore genes the query did not mark as significant. If
-       ``ignore_atlas_forbidden_genes`` (default: {ignore_atlas_forbidden_genes}), also ignore the ``forbidden_gene`` of
-       the atlas (and store them as an ``atlas_forbidden_gene`` mask). If ``ignore_query_forbidden_genes`` (default:
-       {ignore_query_forbidden_genes}), also ignore the ``forbidden_gene`` of the query. All these genes are ignored by
-       the following code.
-
-    3. Invoke :py:func:`metacells.tools.project.project_query_onto_atlas` and
-       :py:func:`metacells.tools.project.compute_query_projection` to project each query metacell onto the atlas, using
-       the ``project_fold_normalization`` (default: {project_fold_normalization}),
-       ``project_min_significant_gene_value`` (default: {project_min_significant_gene_value}),
-       ``project_candidates_count`` (default: {project_candidates_count}), ``project_min_usage_weight`` (default:
-       {project_min_usage_weight}), ``project_abs_folds`` (default: {project_abs_folds}) and ``reproducible``.
-
-    4. Invoke :py:func:`metacells.tools.project.compute_significant_projected_fold_factors` to compute the significant
-       fold factors between the query and its projection, using the ``project_fold_normalization`` (default:
-       {project_fold_normalization}), ``project_max_projection_fold_factor`` (default:
-       {project_max_projection_fold_factor}), ``min_entry_project_fold_factor`` (default:
-       {min_entry_project_fold_factor}), ``project_min_significant_gene_value`` (default:
-       {project_min_significant_gene_value}) and ``project_abs_folds`` (default: {project_abs_folds}).
-
-    5. Invoke :py:func:`metacells.tools.project.find_biased_genes` using the ``project_max_projection_fold_factor``
-        (default: {project_max_projection_fold_factor}), ``biased_min_metacells_fraction`` (default:
-        {biased_min_metacells_fraction}), and ``project_abs_folds`` (default: {project_abs_folds}). If any such genes
-        are found, add them to the ignored genes and repeat steps 3-4.
-
-    6. Invoke :py:func:`metacells.tools.quality.compute_similar_query_metacells` to annotate the query metacells
-       similar to their projection on the atlas using ``project_max_projection_fold_factor`` (default:
-       {project_max_projection_fold_factor}) and the ``project_max_dissimilar_genes`` (default:
-       {project_max_dissimilar_genes}).
+    3. If ``project_corrections`` (default: {project_corrections}: Correlate the expression levels of each gene between
+       the query and projection. If this is at least ``project_min_corrected_gene_correlation`` (default:
+       {project_min_corrected_gene_correlation}), compute the ratio between the mean expression of the gene in the
+       projection and the query. If this is at most 1/(1+``project_min_corrected_gene_factor``) or at least
+       (1+``project_min_corrected_gene_factor``) (default: {project_min_corrected_gene_factor}), then multiply the
+       gene's value by this factor so its level would match the atlas. As usual, ignore genes which do not have at least
+       ``project_min_significant_gene_umis``. If any genes were corrected, then repeat steps 2-3 (but do these steps no
+       more than 3 times).
+
+    4. If ``project_filter_ranges`` (default: {project_filter_ranges}): Compute for each gene its expression range
+       (lowest and highest ``project_ignore_range_quantile`` (default: {project_ignore_range_quantile}) in both the
+       projected and the corrected values. Compute the overlap between these ranges (shared range divided by the query
+       range). If this is less than ``project_ignore_range_min_overlap_fraction`` (default:
+       {project_ignore_range_min_overlap_fraction}), then ignore the gene. If any genes were ignored, repeat steps 2-4
+       (but do this step no more than 3 times).
 
-    7. Invoke :py:func:`metacells.tools.project.project_atlas_to_query` to assign a projected type to each of the
+    5. Invoke :py:func:`metacells.tools.project.convey_atlas_to_query` to assign a projected type to each of the
        query metacells based on the ``atlas_type_property_name`` (default: {atlas_type_property_name}).
 
-    For each type of query metacells:
+    Then, for each type of query metacells:
 
     If ``top_level_parallel`` (default: ``top_level_parallel``), do this in parallel. This seems to work better than
     doing this serially and using parallelism within each type. However this is still inefficient compared to using both
     types of parallelism at once, which the code currently can't do without non-trivial coding (this would have been
     trivial in Julia...).
 
-    8. Invoke :py:func:`metacells.tools.project.find_systematic_genes` to compute the systematic genes using only
-       metacells of this type in both the query and the atlas. Use these to create a list of type-specific ignored
-       genes, instead of the global systematic genes list.
-
-    9. Invoke :py:func:`metacells.tools.project.project_query_onto_atlas` and
-       :py:func:`metacells.tools.project.compute_query_projection` to project each query metacell onto the atlas, using
-       the type-specific ignored genes in addition to the global ignored genes. Note that this projection is not
-       restricted to using atlas metacells of the specific type.
-
-    10. Invoke :py:func:`metacells.tools.project.compute_significant_projected_fold_factors` to compute the significant
-       fold factors between the query and its projection.
-
-    .. todo::
-        Implement a more clever typed projection algorithm that maximizes parallelism both across types and within each
-        type. Which would have been trivial in a language like Julia with true multi-threading w/o a GIL and a global
-        work-stealing scheduler.
-
-    11. Invoke :py:func:`metacells.tools.project.find_biased_genes` to identify type-specific biased genes. If any such
-       genes are found, add them to the type-specific ignored genes (instead of the global biased genes list) and repeat
-       steps 9-10.
+    6. Further reduce the mask of type-specific fitted genes by ignoring any genes in ``ignored_gene_of_<type>``, if
+       this annotation exists in the query. Normalize the sum of the fitted gene fractions to 1 in each metacell.
 
-    And then:
+    7. Invoke :py:func:`metacells.tools.project.compute_projection_weights` to project each query metacell of the type
+       onto the atlas. Note that even though we only look at query metacells (tentatively) assigned the type, their
+       projection on the atlas may use metacells of any type.
+
+    8. Invoke :py:func:`metacells.tools.quality.compute_projected_folds` to compute the significant fold factors
+       between the query and its projection.
+
+    9. Identify type-specific misfit genes whose fold factor is above ``project_max_projection_fold_factor``. If
+       ``consider_atlas_noisy_genes`` and/or ``consider_query_noisy_genes``, then any gene listed in either is allowed
+       an additional ``project_max_projection_noisy_fold_factor``. If any gene has such a high fold factor in at least
+       ``misfit_min_metacells_fraction``, remove it from the fitted genes mask and repeat steps 6-9.
+
+    10. Invoke :py:func:`metacells.tools.quality.compute_similar_query_metacells` to verify which query metacells
+        ended up being sufficiently similar to their projection, using ``project_max_consistency_fold_factor`` (default:
+        {project_max_consistency_fold_factor}), ``project_max_projection_noisy_fold_factor`` (default:
+        {project_max_projection_noisy_fold_factor}), ``project_max_misfit_genes`` (default: {project_max_misfit_genes}),
+        and if needed, the the ``essential_gene_of_<type>``. Also compute the correlation between the corrected
+        and projected gene fractions for each metacell.
 
-    12. If steps 8-11 changed the type assigned to a query metacell (an extremely rate occurrence), repeat them (but do
-       these steps no more than 3 times).
+    And then:
 
-    13. Correlate the expression levels of each gene between the query and projection. If this is less than
-       ``project_max_uncorrelated_gene_correlation`` (default: {project_max_uncorrelated_gene_correlation}), then mark
-       the gene as ignored. If this is at least ``project_min_corrected_gene_correlation`` (default:
-       {project_min_corrected_gene_correlation}), compute the ratio between the mean expression of the gene in the
-       projection and the query. If this is at most 1/(1+``project_min_corrected_gene_factor``) or at least
-       (1+``project_min_corrected_gene_factor``) (default: {project_min_corrected_gene_factor}), then multiply the
-       gene's value by this factor so its level would match the atlas. If any genes were ignored or corrected, then
-       start over from step 2 ignoring the uncorrelated genes and using the corrected gene expression levels (but do
-       these steps no more than 3 times).
-
-    14. Invoke :py:func:`metacells.tools.quality.compute_similar_query_metacells` to validate the updated projection.
-
-    15. If ``renormalize_query_by_atlas`` (default: {renormalize_query_by_atlas}), then invoke
-       :py:func:`metacells.tools.project.renormalize_query_by_atlas` using the ``renormalize_var_annotations``,
-       ``renormalize_layers`` and ``renormalize_varp_annotations``, if any, to add an ``ATLASNORM`` pseudo-gene so that
-       the fraction out of the total UMIs in the query of the genes common to the atlas would be the same on average as
-       their fraction out of the total UMIs in the atlas.
+    11. Invoke :py:func:`metacells.tools.project.convey_atlas_to_query` to assign an updated projected type to each of
+        the query metacells based on the ``atlas_type_property_name`` (default: {atlas_type_property_name}). If this
+        changed the type assigned to any query metacell, repeat steps 6-11 (but do this step no more than 3 times).
+
+    For each query metacell that ended up being dissimilar, try to project them as a combination of two atlas regions:
+
+    12. Reduce the list of fitted genes for the metacell based on the ``ignored_gene_of_<type>`` for both the primary
+        (initially from the above) query metacell type and the secondary query metacell type (initially empty).
+        Normalize the sum of the gene fractions in the metacell to 1.
+
+    13. Invoke :py:func:`metacells.tools.project.compute_projection_weights` just for this metacell, allowing the
+        projection to use a secondary location in the atlas based on the residuals of the atlas metacells relative to
+        the primary query projection.
+
+    14. Invoke :py:func:`metacells.tools.project.convey_atlas_to_query` twice, once for the weights of the primary
+        location and once for the weights of the secondary location, to obtain a primary and secondary type for
+        the query metacell. If these have changed, repeat steps 13-14 (but do these steps no more than 3 times; note
+        will will always do them twice as the 1st run will generate some non-empty secondary type).
+
+    15. Invoke :py:func:`metacells.tools.quality.compute_projected_folds` and
+        :py:func:`metacells.tools.quality.compute_similar_query_metacells` to update the projection and evaluation of
+        the query metacell. If it is now similar, then use the results for the metacell; otherwise, keep the original
+        results as they were at the end of step 10.
     """
     assert project_min_corrected_gene_factor >= 0
+    use_essential_genes = project_min_essential_genes_fraction is not None and _has_any_essential_genes(adata)
+
+    ut.set_m_data(qdata, "project_max_projection_fold_factor", project_max_projection_fold_factor)
+    ut.set_m_data(qdata, "project_max_projection_noisy_fold_factor", project_max_projection_noisy_fold_factor)
+    ut.set_m_data(qdata, "project_max_misfit_genes", project_max_misfit_genes)
 
-    qdata = qdata.copy()
+    atlas_common_gene_indices, query_common_gene_indices = _common_gene_indices(adata, qdata)
 
-    _fill_manually_ignored_genes(
+    type_names = _initialize_atlas_data_in_query(
+        adata,
         qdata,
-        ignored_gene_names=ignored_gene_names,
-        ignored_gene_patterns=ignored_gene_patterns,
-        ignored_gene_names_of_type=ignored_gene_names_of_type,
-        ignored_gene_patterns_of_type=ignored_gene_patterns_of_type,
+        atlas_type_property_name=atlas_type_property_name,
+        atlas_common_gene_indices=atlas_common_gene_indices,
+        query_common_gene_indices=query_common_gene_indices,
+        consider_atlas_noisy_genes=consider_atlas_noisy_genes,
+        consider_query_noisy_genes=consider_query_noisy_genes,
+        use_essential_genes=use_essential_genes,
     )
 
-    common_adata, common_qdata = _common_data(
-        adata=adata,
-        qdata=qdata,
-        project_max_projection_fold_factor=project_max_projection_fold_factor,
-        project_max_dissimilar_genes=project_max_dissimilar_genes,
-        ignore_atlas_insignificant_genes=ignore_atlas_insignificant_genes,
-        ignore_atlas_forbidden_genes=ignore_atlas_forbidden_genes,
-    )
+    common_adata = _initialize_common_adata(adata, what, atlas_common_gene_indices)
+    common_qdata = _initialize_common_qdata(qdata, what, query_common_gene_indices)
 
-    atlas_total_common_umis = ut.get_o_numpy(common_adata, what, sum=True)
+    query_marker_genes_mask = ut.get_v_numpy(common_qdata, "marker_gene")
+    min_fitted_query_marker_genes = np.sum(query_marker_genes_mask) * project_min_query_markers_fraction
+    ut.log_calc("min_fitted_query_marker_genes", min_fitted_query_marker_genes)
 
-    repeat = 0
-    while True:
-        repeat += 1
-        ut.log_calc("correlation repeat", repeat)
-
-        query_total_common_umis = ut.get_o_numpy(common_qdata, what, sum=True)
+    min_essential_genes_of_type = _min_essential_genes_of_type(
+        adata=adata,
+        common_adata=common_adata,
+        type_names=type_names,
+        project_min_essential_genes_fraction=project_min_essential_genes_fraction,
+    )
 
-        _compute_preliminary_projection(
-            what=what,
-            common_adata=common_adata,
-            common_qdata=common_qdata,
-            atlas_total_common_umis=atlas_total_common_umis,
-            query_total_common_umis=query_total_common_umis,
-            systematic_low_gene_quantile=systematic_low_gene_quantile,
-            systematic_high_gene_quantile=systematic_high_gene_quantile,
-            ignore_atlas_insignificant_genes=ignore_atlas_insignificant_genes,
-            ignore_query_insignificant_genes=ignore_query_insignificant_genes,
-            ignore_atlas_forbidden_genes=ignore_atlas_forbidden_genes,
-            ignore_query_forbidden_genes=ignore_query_forbidden_genes,
-            project_fold_normalization=project_fold_normalization,
-            project_min_significant_gene_value=project_min_significant_gene_value,
-            project_max_consistency_fold_factor=project_max_consistency_fold_factor,
-            project_candidates_count=project_candidates_count,
-            project_min_usage_weight=project_min_usage_weight,
-            project_max_projection_fold_factor=project_max_projection_fold_factor,
-            min_entry_project_fold_factor=min_entry_project_fold_factor,
-            biased_min_metacells_fraction=biased_min_metacells_fraction,
-            project_abs_folds=project_abs_folds,
-            atlas_type_property_name=atlas_type_property_name,
-            reproducible=reproducible,
-        )
+    preliminary_fitted_genes_mask = _preliminary_fitted_genes_mask(
+        common_adata=common_adata,
+        common_qdata=common_qdata,
+        only_atlas_marker_genes=only_atlas_marker_genes,
+        only_query_marker_genes=only_query_marker_genes,
+        ignore_atlas_lateral_genes=ignore_atlas_lateral_genes,
+        ignore_query_lateral_genes=ignore_query_lateral_genes,
+        min_significant_gene_umis=project_min_significant_gene_umis,
+    )
 
-        weights = _compute_per_type_projection(
-            what=what,
-            common_adata=common_adata,
-            common_qdata=common_qdata,
-            atlas_total_common_umis=atlas_total_common_umis,
-            query_total_common_umis=query_total_common_umis,
-            systematic_low_gene_quantile=systematic_low_gene_quantile,
-            systematic_high_gene_quantile=systematic_high_gene_quantile,
-            biased_min_metacells_fraction=biased_min_metacells_fraction,
-            project_fold_normalization=project_fold_normalization,
-            project_candidates_count=project_candidates_count,
-            project_min_significant_gene_value=project_min_significant_gene_value,
-            project_min_usage_weight=project_min_usage_weight,
-            project_max_consistency_fold_factor=project_max_consistency_fold_factor,
-            project_max_projection_fold_factor=project_max_projection_fold_factor,
-            project_max_dissimilar_genes=project_max_dissimilar_genes,
-            min_entry_project_fold_factor=min_entry_project_fold_factor,
-            project_abs_folds=project_abs_folds,
-            atlas_type_property_name=atlas_type_property_name,
-            top_level_parallel=top_level_parallel,
-            reproducible=reproducible,
-        )
+    _compute_preliminary_projection(
+        common_adata=common_adata,
+        common_qdata=common_qdata,
+        preliminary_fitted_genes_mask=preliminary_fitted_genes_mask,
+        project_log_data=project_log_data,
+        project_fold_regularization=project_fold_regularization,
+        project_min_significant_gene_umis=project_min_significant_gene_umis,
+        project_filter_ranges=project_filter_ranges,
+        project_ignore_range_quantile=project_ignore_range_quantile,
+        project_ignore_range_min_overlap_fraction=project_ignore_range_min_overlap_fraction,
+        project_max_consistency_fold_factor=project_max_consistency_fold_factor,
+        project_candidates_count=project_candidates_count,
+        project_min_usage_weight=project_min_usage_weight,
+        project_corrections=project_corrections,
+        project_min_corrected_gene_correlation=project_min_corrected_gene_correlation,
+        project_min_corrected_gene_factor=project_min_corrected_gene_factor,
+        atlas_type_property_name=atlas_type_property_name,
+        reproducible=reproducible,
+    )
 
-        if repeat > 2 or not _correct_correlated_genes(
-            what=what,
-            common_qdata=common_qdata,
-            project_max_uncorrelated_gene_correlation=project_max_uncorrelated_gene_correlation,
-            project_min_corrected_gene_correlation=project_min_corrected_gene_correlation,
-            project_min_corrected_gene_factor=project_min_corrected_gene_factor,
-            reproducible=reproducible,
-        ):
-            break
+    weights = _compute_per_type_projection(
+        common_adata=common_adata,
+        common_qdata=common_qdata,
+        type_names=type_names,
+        preliminary_fitted_genes_mask=preliminary_fitted_genes_mask,
+        misfit_min_metacells_fraction=misfit_min_metacells_fraction,
+        project_log_data=project_log_data,
+        project_fold_regularization=project_fold_regularization,
+        project_candidates_count=project_candidates_count,
+        project_min_significant_gene_umis=project_min_significant_gene_umis,
+        project_min_usage_weight=project_min_usage_weight,
+        project_max_consistency_fold_factor=project_max_consistency_fold_factor,
+        project_max_projection_fold_factor=project_max_projection_fold_factor,
+        project_max_projection_noisy_fold_factor=project_max_projection_noisy_fold_factor,
+        project_max_misfit_genes=project_max_misfit_genes,
+        min_fitted_query_marker_genes=min_fitted_query_marker_genes,
+        min_essential_genes_of_type=min_essential_genes_of_type,
+        atlas_type_property_name=atlas_type_property_name,
+        top_level_parallel=top_level_parallel,
+        reproducible=reproducible,
+    )
 
-    weights = _compute_dissimilar_residuals_projection(
-        what=what,
-        weights=weights,
+    _compute_dissimilar_residuals_projection(
+        weights_per_atlas_per_query_metacell=weights,
         common_adata=common_adata,
         common_qdata=common_qdata,
-        atlas_total_common_umis=atlas_total_common_umis,
-        query_total_common_umis=query_total_common_umis,
-        project_fold_normalization=project_fold_normalization,
+        project_log_data=project_log_data,
+        project_fold_regularization=project_fold_regularization,
         project_candidates_count=project_candidates_count,
-        project_min_significant_gene_value=project_min_significant_gene_value,
+        project_min_candidates_fraction=project_min_candidates_fraction,
+        project_min_significant_gene_umis=project_min_significant_gene_umis,
         project_min_usage_weight=project_min_usage_weight,
         project_max_consistency_fold_factor=project_max_consistency_fold_factor,
         project_max_projection_fold_factor=project_max_projection_fold_factor,
-        project_max_dissimilar_genes=project_max_dissimilar_genes,
-        min_entry_project_fold_factor=min_entry_project_fold_factor,
-        project_abs_folds=project_abs_folds,
+        project_max_projection_noisy_fold_factor=project_max_projection_noisy_fold_factor,
+        project_max_misfit_genes=project_max_misfit_genes,
+        min_fitted_query_marker_genes=min_fitted_query_marker_genes,
+        min_essential_genes_of_type=min_essential_genes_of_type,
         atlas_type_property_name=atlas_type_property_name,
         top_level_parallel=top_level_parallel,
         reproducible=reproducible,
     )
 
-    _convey_query_common_to_full_data(what=what, qdata=qdata, common_qdata=common_qdata)
+    tl.compute_projected_fractions(
+        adata=common_adata,
+        qdata=common_qdata,
+        log_data=project_log_data,
+        fold_regularization=project_fold_regularization,
+        weights=weights,
+    )
 
-    qdata = _renormalize_query(
-        adata=adata,
+    _common_data_to_full(
         qdata=qdata,
-        atlas_type_property_name=atlas_type_property_name,
-        renormalize_query_by_atlas=renormalize_query_by_atlas,
-        renormalize_var_annotations=renormalize_var_annotations,
-        renormalize_layers=renormalize_layers,
-        renormalize_varp_annotations=renormalize_varp_annotations,
+        common_qdata=common_qdata,
+        project_corrections=project_corrections,
+        type_names=type_names,
+        use_essential_genes=use_essential_genes,
     )
 
-    return sp.csr_matrix(weights), qdata
+    ut.set_m_data(qdata, "projection_algorithm", f"metacells.{__version__}")
+    return sp.csr_matrix(weights)
 
 
-@ut.logged()
-@ut.timed_call()
-def _fill_manually_ignored_genes(
-    qdata: AnnData,
-    ignored_gene_names: Optional[Collection[str]],
-    ignored_gene_patterns: Optional[Collection[Union[str, Pattern]]],
-    ignored_gene_names_of_type: Optional[Dict[str, Collection[str]]],
-    ignored_gene_patterns_of_type: Optional[Dict[str, Collection[str]]],
-) -> None:
-    if ignored_gene_names is not None or ignored_gene_patterns is not None:
-        tl.find_named_genes(qdata, to="manually_ignored_gene", names=ignored_gene_names, patterns=ignored_gene_patterns)
+def _common_gene_indices(adata: AnnData, qdata: AnnData) -> Tuple[ut.NumpyVector, ut.NumpyVector]:
+    if list(qdata.var_names) == list(adata.var_names):
+        atlas_common_gene_indices = query_common_gene_indices = np.array(range(qdata.n_vars), dtype="int32")
+    else:
+        atlas_genes_list = list(adata.var_names)
+        query_genes_list = list(qdata.var_names)
+        common_genes_list = list(sorted(set(atlas_genes_list) & set(query_genes_list)))
+        assert len(common_genes_list) > 0
+        atlas_common_gene_indices = np.array([atlas_genes_list.index(gene) for gene in common_genes_list])
+        query_common_gene_indices = np.array([query_genes_list.index(gene) for gene in common_genes_list])
+
+    return atlas_common_gene_indices, query_common_gene_indices
+
+
+def _has_any_essential_genes(adata: AnnData) -> bool:
+    for property_name in adata.var.keys():
+        if property_name.startswith("essential_gene_of_"):
+            return True
+    return False
 
-    if ignored_gene_names_of_type is None:
-        ignored_gene_names_of_type = {}
-    if ignored_gene_patterns_of_type is None:
-        ignored_gene_patterns_of_type = {}
-
-    ignored_type_names = list(set(ignored_gene_names_of_type.keys()) | set(ignored_gene_patterns_of_type.keys()))
-    for type_name in ignored_type_names:
-        tl.find_named_genes(
+
+def _initialize_atlas_data_in_query(
+    adata: AnnData,
+    qdata: AnnData,
+    *,
+    atlas_type_property_name: str,
+    atlas_common_gene_indices: ut.NumpyVector,
+    query_common_gene_indices: ut.NumpyVector,
+    consider_atlas_noisy_genes: bool,
+    consider_query_noisy_genes: bool,
+    use_essential_genes: bool,
+) -> List[str]:
+    atlas_genes_mask = np.zeros(qdata.n_vars, dtype="bool")
+    atlas_genes_mask[query_common_gene_indices] = True
+    ut.set_v_data(qdata, "atlas_gene", atlas_genes_mask)
+
+    type_names = list(np.unique(ut.get_o_numpy(adata, atlas_type_property_name)))
+
+    genes_mask_names = ["lateral_gene", "noisy_gene", "marker_gene"]
+    if consider_atlas_noisy_genes:
+        genes_mask_names.append("noisy_gene")
+    if use_essential_genes:
+        genes_mask_names += [f"essential_gene_of_{type_name}" for type_name in type_names]
+
+    for genes_mask_name in genes_mask_names:
+        if not ut.has_data(adata, genes_mask_name):
+            continue
+        atlas_mask = ut.get_v_numpy(adata, genes_mask_name)
+        query_mask = np.zeros(qdata.n_vars, dtype="bool")
+        query_mask[query_common_gene_indices] = atlas_mask[atlas_common_gene_indices]
+        ut.set_v_data(
             qdata,
-            to=f"manually_ignored_gene_of_{type_name}",
-            names=ignored_gene_names_of_type.get(type_name),
-            patterns=ignored_gene_patterns_of_type.get(type_name),
+            genes_mask_name if genes_mask_name.startswith("essential_gene_of_") else "atlas_" + genes_mask_name,
+            query_mask,
         )
 
+    noisy_masks: List[str] = []
+    if consider_atlas_noisy_genes and ut.has_data(qdata, "atlas_noisy_gene"):
+        noisy_masks.append("|atlas_noisy_gene")
 
-@ut.logged()
-@ut.timed_call()
-def _common_data(
-    *,
+    if consider_query_noisy_genes and ut.has_data(qdata, "noisy_gene"):
+        noisy_masks.append("|noisy_gene")
+
+    if len(noisy_masks) > 0:
+        tl.combine_masks(qdata, noisy_masks, to="projected_noisy_gene")
+
+    return type_names
+
+
+def _initialize_common_adata(adata: AnnData, what: str, atlas_common_gene_indices: ut.NumpyVector) -> AnnData:
+    common_adata = ut.slice(adata, name=".common", vars=atlas_common_gene_indices, top_level=False)
+
+    atlas_total_common_umis = ut.get_o_numpy(common_adata, "total_umis", sum=True)
+    ut.set_o_data(common_adata, "total_umis", atlas_total_common_umis)
+
+    _normalize_corrected_fractions(common_adata, what)
+
+    return common_adata
+
+
+def _initialize_common_qdata(
     qdata: AnnData,
+    what: str,
+    query_common_gene_indices: ut.NumpyVector,
+) -> AnnData:
+    common_qdata = ut.slice(
+        qdata,
+        name=".common",
+        vars=query_common_gene_indices,
+        track_var="full_gene_index_of_qdata",
+        top_level=False,
+    )
+
+    query_total_common_umis = ut.get_o_numpy(common_qdata, "total_umis", sum=True)
+    ut.set_o_data(common_qdata, "total_umis", query_total_common_umis)
+    ut.set_o_data(qdata, "total_atlas_umis", query_total_common_umis)
+
+    _normalize_corrected_fractions(common_qdata, what)
+
+    return common_qdata
+
+
+def _min_essential_genes_of_type(
+    *,
     adata: AnnData,
-    project_max_projection_fold_factor: float,
-    project_max_dissimilar_genes: int,
-    ignore_atlas_insignificant_genes: bool,
-    ignore_atlas_forbidden_genes: bool,
-) -> Tuple[AnnData, AnnData]:
-    ut.set_m_data(qdata, "project_max_projection_fold_factor", project_max_projection_fold_factor)
-    ut.set_m_data(qdata, "project_max_dissimilar_genes", project_max_dissimilar_genes)
+    common_adata: AnnData,
+    type_names: List[str],
+    project_min_essential_genes_fraction: Optional[float],
+) -> Dict[Tuple[str, str], Optional[int]]:
+    min_essential_genes_of_type: Dict[Tuple[str, str], Optional[int]] = {
+        (type_name, other_type_name): None for type_name in type_names for other_type_name in type_names
+    }
+
+    has_any_essential_genes = False
+    if project_min_essential_genes_fraction is not None:
+        for type_name in type_names:
+            if type_name != "Outliers" and ut.has_data(adata, f"essential_gene_of_{type_name}"):
+                has_any_essential_genes = True
+                break
+
+    if not has_any_essential_genes:
+        return min_essential_genes_of_type
+    assert project_min_essential_genes_fraction is not None
+
+    for type_name in type_names:
+        if type_name == "Outliers":
+            min_essential_genes_count: Optional[int] = None
+        else:
+            atlas_essential_genes_mask = ut.get_v_numpy(adata, f"essential_gene_of_{type_name}")
+            atlas_essential_genes_count = np.sum(atlas_essential_genes_mask)
 
-    if list(qdata.var_names) != list(adata.var_names):
-        atlas_genes_list = list(adata.var_names)
-        query_genes_list = list(qdata.var_names)
-        common_genes_list = list(sorted(set(atlas_genes_list) & set(query_genes_list)))
-        assert len(common_genes_list) > 0
-        atlas_gene_indices = np.array([atlas_genes_list.index(gene) for gene in common_genes_list])
-        query_gene_indices = np.array([query_genes_list.index(gene) for gene in common_genes_list])
-        common_adata = ut.slice(adata, name=".common", vars=atlas_gene_indices)
-        common_qdata = ut.slice(
-            qdata,
-            name=".common",
-            vars=query_gene_indices,
-            track_obs="full_metacell_index_of_qdata",
-            track_var="full_gene_index_of_qdata",
-        )
-    else:
-        common_adata = adata
-        common_qdata = qdata
-        ut.set_o_data(common_qdata, "full_metacell_index_of_qdata", np.arange(qdata.n_obs))
-        ut.set_v_data(common_qdata, "full_gene_index_of_qdata", np.arange(qdata.n_vars))
-
-    assert list(common_qdata.var_names) == list(common_adata.var_names)
-
-    ut.set_o_data(common_qdata, "common_cell_index_of_qdata", np.arange(common_qdata.n_obs))
-    ut.set_v_data(common_qdata, "common_gene_index_of_qdata", np.arange(common_qdata.n_vars))
-    ut.set_v_data(common_qdata, "biased_gene", np.full(common_qdata.n_vars, False))
-    ut.set_v_data(common_qdata, "uncorrelated_gene", np.zeros(common_qdata.n_vars, dtype="bool"))
-    ut.set_v_data(common_qdata, "correction_factor", np.full(common_qdata.n_vars, 1.0, dtype="float32"))
-    ut.set_v_data(common_qdata, "atlas_gene", np.full(common_qdata.n_vars, True))
-
-    if ignore_atlas_insignificant_genes:
-        atlas_significant_mask = ut.get_v_numpy(common_adata, "significant_gene")
-        ut.set_v_data(common_qdata, "atlas_significant_gene", atlas_significant_mask)
-
-    if ignore_atlas_forbidden_genes:
-        atlas_forbiden_mask = ut.get_v_numpy(common_adata, "forbidden_gene")
-        ut.set_v_data(common_qdata, "atlas_forbidden_gene", atlas_forbiden_mask)
+            common_essential_genes_mask = ut.get_v_numpy(common_adata, f"essential_gene_of_{type_name}")
+            common_essential_genes_count = np.sum(common_essential_genes_mask)
 
-    return common_adata, common_qdata
+            min_essential_genes_count = ceil(project_min_essential_genes_fraction * atlas_essential_genes_count)
+            assert min_essential_genes_count is not None
+            assert min_essential_genes_count >= 0
+
+            if min_essential_genes_count > common_essential_genes_count:
+                atlas_essential_genes_names = sorted(adata.var_names[atlas_essential_genes_mask])
+                common_essential_genes_names = sorted(common_adata.var_names[common_essential_genes_mask])
+                missing_essential_genes_names = sorted(
+                    set(atlas_essential_genes_names) - set(common_essential_genes_names)
+                )
+                ut.logger().warning(  # pylint: disable=logging-fstring-interpolation
+                    f"the {common_essential_genes_count} "
+                    f"common essential gene(s) {', '.join(common_essential_genes_names)} "
+                    f"for the type {type_name} "
+                    f"are not enough for the required {min_essential_genes_count}; "
+                    "reducing the minimal requirement "
+                    f" (the non-common essential gene(s) are: {', '.join(missing_essential_genes_names)})"
+                )
+                min_essential_genes_count = common_essential_genes_count
+
+        min_essential_genes_of_type[(type_name, type_name)] = min_essential_genes_count
+        ut.log_calc(f"min_essential_genes_of_type[{type_name}]", min_essential_genes_count)
+
+        if min_essential_genes_count is None:
+            continue
+
+        for other_type_name in type_names:
+            if other_type_name <= type_name or other_type_name == "Outliers":
+                continue
+
+            other_atlas_essential_genes_mask = ut.get_v_numpy(adata, f"essential_gene_of_{type_name}")
+            pair_atlas_essential_genes_mask = atlas_essential_genes_mask | other_atlas_essential_genes_mask
+            pair_atlas_essential_genes_count = np.sum(pair_atlas_essential_genes_mask)
+
+            other_common_essential_genes_mask = ut.get_v_numpy(common_adata, f"essential_gene_of_{type_name}")
+            pair_common_essential_genes_mask = common_essential_genes_mask | other_common_essential_genes_mask
+            pair_common_essential_genes_count = np.sum(pair_common_essential_genes_mask)
+
+            missing_essential_genes_count = pair_atlas_essential_genes_count - pair_common_essential_genes_count
+            assert missing_essential_genes_count >= 0
+
+            min_essential_genes_count = ceil(project_min_essential_genes_fraction * pair_atlas_essential_genes_count)
+            assert min_essential_genes_count is not None
+            ut.log_calc(f"min_essential_genes_of_type[{type_name}, {other_type_name}]", min_essential_genes_count)
+            min_essential_genes_of_type[(type_name, other_type_name)] = min_essential_genes_count
+            min_essential_genes_of_type[(other_type_name, type_name)] = min_essential_genes_count
 
+    return min_essential_genes_of_type
 
-@ut.logged()
-@ut.timed_call()
-def _convey_query_common_to_full_data(
+
+def _preliminary_fitted_genes_mask(
     *,
-    what: str,
-    qdata: AnnData,
+    common_adata: AnnData,
     common_qdata: AnnData,
-) -> None:
-    if id(qdata) == id(common_qdata):
-        for data_name in ["full_metacell_index_of_qdata", "common_cell_index_of_qdata"]:
-            del qdata.obs[data_name]
+    only_atlas_marker_genes: bool,
+    only_query_marker_genes: bool,
+    ignore_atlas_lateral_genes: bool,
+    ignore_query_lateral_genes: bool,
+    min_significant_gene_umis: int,
+) -> ut.NumpyVector:
+    atlas_total_umis_per_gene = ut.get_v_numpy(common_adata, "total_umis", sum=True)
+    query_total_umis_per_gene = ut.get_v_numpy(common_qdata, "total_umis", sum=True)
+    total_umis_per_gene = atlas_total_umis_per_gene + query_total_umis_per_gene
+    preliminary_fitted_genes_mask = total_umis_per_gene >= min_significant_gene_umis
+    ut.log_calc("total_umis_mask", preliminary_fitted_genes_mask)
 
-        for data_name in ["full_gene_index_of_qdata", "common_gene_index_of_qdata"]:
-            del qdata.var[data_name]
+    if only_atlas_marker_genes and ut.has_data(common_adata, "marker_gene"):
+        preliminary_fitted_genes_mask &= ut.get_v_numpy(common_adata, "marker_gene")
 
-        return
+    if only_query_marker_genes and ut.has_data(common_qdata, "marker_gene"):
+        preliminary_fitted_genes_mask &= ut.get_v_numpy(common_qdata, "marker_gene")
 
-    assert common_qdata.n_obs == qdata.n_obs
+    if ignore_atlas_lateral_genes and ut.has_data(common_adata, "lateral_gene"):
+        preliminary_fitted_genes_mask &= ~ut.get_v_numpy(common_adata, "lateral_gene")
 
-    for data_name in ["similar", "projected_type", "projected_secondary_type"]:
-        ut.set_o_data(qdata, data_name, ut.get_o_numpy(common_qdata, data_name))
+    if ignore_query_lateral_genes and ut.has_data(common_qdata, "lateral_gene"):
+        preliminary_fitted_genes_mask &= ~ut.get_v_numpy(common_qdata, "lateral_gene")
 
-    dissimilar_genes_count = ut.get_o_numpy(common_qdata, "dissimilar_genes_count")
-    ut.log_calc("max dissimilar_genes_count", np.max(dissimilar_genes_count))
-    ut.set_o_data(qdata, "dissimilar_genes_count", dissimilar_genes_count, formatter=ut.mask_description)
+    if ut.has_data(common_qdata, "ignored_gene"):
+        preliminary_fitted_genes_mask &= ~ut.get_v_numpy(common_qdata, "ignored_gene")
 
-    full_gene_index_of_common_qdata = ut.get_v_numpy(common_qdata, "full_gene_index_of_qdata")
+    return preliminary_fitted_genes_mask
 
-    for (data_name, dtype, default) in [
-        ("atlas_gene", "bool", False),
-        ("atlas_forbidden_gene", "bool", False),
-        ("atlas_significant_gene", "bool", False),
-        ("biased_gene", "bool", False),
-        ("systematic_gene", "bool", False),
-        ("ignored_gene", "bool", True),
-        ("projected_correlation", "float32", 0.0),
-        ("correlated_gene", "bool", False),
-        ("uncorrelated_gene", "bool", False),
-        ("correction_factor", "float32", 1.0),
-    ]:
-        if ut.has_data(common_qdata, data_name):
-            full_data = np.full(qdata.n_vars, default, dtype=dtype)
-            full_data[full_gene_index_of_common_qdata] = ut.get_v_numpy(common_qdata, data_name)
-            ut.set_v_data(qdata, data_name, full_data)
-
-    for type_name in np.unique(ut.get_o_numpy(qdata, "projected_type")):
-        for data_name in ["systematic_gene", "ignored_gene", "biased_gene"]:
-            type_data_name = f"{data_name}_of_{type_name}"
-            full_data = np.zeros(qdata.n_vars, dtype="bool")
-            full_data[full_gene_index_of_common_qdata] = ut.get_v_numpy(common_qdata, type_data_name)
-            ut.set_v_data(qdata, type_data_name, full_data)
-
-    common_corrected_data = ut.to_numpy_matrix(ut.get_vo_proper(common_qdata, what)).copy()
-    full_corrected_data = ut.to_numpy_matrix(ut.get_vo_proper(qdata, what)).copy()
-    full_corrected_data[:, full_gene_index_of_common_qdata] = common_corrected_data
-    ut.set_vo_data(qdata, what, full_corrected_data)
-
-    common_projected_fold = ut.get_vo_proper(common_qdata, "projected_fold")
-    full_projected_fold = np.zeros(qdata.shape, dtype="float32")
-    full_projected_fold[:, full_gene_index_of_common_qdata] = ut.to_numpy_matrix(common_projected_fold)
-    ut.set_vo_data(qdata, "projected_fold", sp.csr_matrix(full_projected_fold))
-
-    common_projected = ut.get_vo_proper(common_qdata, "projected")
-    full_projected = np.zeros(qdata.shape, dtype="float32")
-    full_projected[:, full_gene_index_of_common_qdata] = ut.to_numpy_matrix(common_projected)
-    ut.set_vo_data(qdata, "projected", full_projected)
 
-
-@ut.logged()
-@ut.timed_call()
-def _renormalize_query(
+def _common_data_to_full(
     *,
-    adata: AnnData,
     qdata: AnnData,
-    atlas_type_property_name: str,
-    renormalize_query_by_atlas: bool,
-    renormalize_var_annotations: Optional[Dict[str, Any]],
-    renormalize_layers: Optional[Dict[str, Any]],
-    renormalize_varp_annotations: Optional[Dict[str, Any]],
-) -> AnnData:
-    if not renormalize_query_by_atlas:
-        return qdata
+    common_qdata: AnnData,
+    project_corrections: bool,
+    use_essential_genes: bool,
+    type_names: List[str],
+) -> None:
+    if use_essential_genes:
+        primary_type_per_metacell = ut.get_o_numpy(common_qdata, "projected_type")
+        secondary_type_per_metacell = ut.get_o_numpy(common_qdata, "projected_secondary_type")
+        essential_per_gene_per_metacell = np.zeros(qdata.shape, dtype="bool")
+        essential_gene_per_type = {
+            type_name: ut.get_v_numpy(qdata, f"essential_gene_of_{type_name}")
+            for type_name in type_names
+            if type_name != "Outliers"
+        }
+        for metacell_index in range(qdata.n_obs):
+            primary_type_of_metacell = primary_type_per_metacell[metacell_index]
+            if primary_type_of_metacell != "Outliers":
+                essential_per_gene_per_metacell[metacell_index, :] = essential_gene_per_type[primary_type_of_metacell]
+
+            secondary_type_of_metacell = secondary_type_per_metacell[metacell_index]
+            if secondary_type_of_metacell not in ("", "Outliers", primary_type_of_metacell):
+                essential_per_gene_per_metacell[metacell_index, :] |= essential_gene_per_type[
+                    secondary_type_of_metacell
+                ]
 
-    var_annotations = dict(
-        # Standard MC2 gene annotations.
-        clean_gene=False,
-        excluded_gene=False,
-        feature_gene=False,
-        forbidden_gene=False,
-        gene_deviant_votes=0,
-        high_relative_variance_gene=False,
-        high_total_gene=False,
-        noisy_lonely_gene=False,
-        pre_feature_gene=False,
-        pre_gene_deviant_votes=0,
-        pre_high_relative_variance_gene=False,
-        pre_high_total_gene=False,
-        properly_sampled_gene=False,
-        rare_gene=False,
-        rare_gene_module=-1,
-        related_genes_module=-1,
-        significant_gene=False,
-        top_feature_gene=False,
-        # Annotations added here (except for per-type).
-        atlas_forbidden_gene=False,
-        atlas_gene=False,
-        atlas_significant_gene=False,
-        biased_gene=False,
-        correction_factor=1.0,
-        correlated_gene=False,
-        ignored_gene=False,
-        manually_ignored_gene=False,
-        projected_correlation=0.0,
-        systematic_gene=False,
-        uncorrelated_gene=False,
-    )
-
-    if renormalize_var_annotations is not None:
-        var_annotations.update(renormalize_var_annotations)
-
-    layers = dict(inner_fold=0.0, projected=0.0, projected_fold=0.0)
-
-    if renormalize_layers is not None:
-        layers.update(renormalize_layers)
-
-    varp_annotations = dict(var_similarity=0.0)
-    if renormalize_varp_annotations is not None:
-        varp_annotations.update(renormalize_varp_annotations)
-
-    for type_name in np.unique(ut.get_o_numpy(adata, atlas_type_property_name)):
-        var_annotations[f"systematic_gene_of_{type_name}"] = False
-        var_annotations[f"biased_gene_of_{type_name}"] = False
-        var_annotations[f"manually_ignored_gene_of_{type_name}"] = False
-        var_annotations[f"ignored_gene_of_{type_name}"] = False
+        ut.set_vo_data(qdata, "essential", sp.csr_matrix(essential_per_gene_per_metacell))
 
-    renormalized_qdata = tl.renormalize_query_by_atlas(
-        adata=adata,
-        qdata=qdata,
-        var_annotations=var_annotations,
-        layers=layers,
-        varp_annotations=varp_annotations,
-    )
+    full_gene_index_of_common_qdata = ut.get_v_numpy(common_qdata, "full_gene_index_of_qdata")
 
-    if renormalized_qdata is not None:
-        return renormalized_qdata
+    for property_name in (
+        "corrected_fraction",
+        "projected_fraction",
+        "fitted",
+        "misfit",
+        "projected_fold",
+    ):
+        data_per_common_gene_per_metacell = ut.get_vo_proper(common_qdata, property_name)
+        data_per_gene_per_metacell = np.zeros(qdata.shape, dtype=ut.shaped_dtype(data_per_common_gene_per_metacell))
+        data_per_gene_per_metacell[:, full_gene_index_of_common_qdata] = ut.to_numpy_matrix(
+            data_per_common_gene_per_metacell
+        )
+        ut.set_vo_data(qdata, property_name, sp.csr_matrix(data_per_gene_per_metacell))
 
-    return qdata
+    property_names = [f"fitted_gene_of_{type_name}" for type_name in type_names]
+    if project_corrections:
+        property_names.append("correction_factor")
+
+    for property_name in property_names:
+        data_per_common_gene = ut.get_v_numpy(common_qdata, property_name)
+        data_per_full_gene = np.zeros(qdata.n_vars, dtype=data_per_common_gene.dtype)
+        data_per_full_gene[full_gene_index_of_common_qdata] = data_per_common_gene
+        ut.set_v_data(qdata, property_name, data_per_full_gene)
+
+    for property_name, formatter in (
+        ("projected_type", None),
+        ("projected_secondary_type", None),
+        ("projected_correlation", ut.sizes_description),
+        ("similar", None),
+    ):
+        data_per_metacell = ut.get_o_numpy(common_qdata, property_name, formatter=formatter)
+        ut.set_o_data(qdata, property_name, data_per_metacell, formatter=formatter)
 
 
 @ut.logged()
 @ut.timed_call()
 def _compute_preliminary_projection(
     *,
-    what: str,
     common_adata: AnnData,
     common_qdata: AnnData,
-    atlas_total_common_umis: ut.NumpyVector,
-    query_total_common_umis: ut.NumpyVector,
-    systematic_low_gene_quantile: float,
-    systematic_high_gene_quantile: float,
-    ignore_atlas_insignificant_genes: bool,
-    ignore_query_insignificant_genes: bool,
-    ignore_atlas_forbidden_genes: bool,
-    ignore_query_forbidden_genes: bool,
-    project_fold_normalization: float,
-    project_min_significant_gene_value: float,
+    preliminary_fitted_genes_mask: ut.NumpyVector,
+    project_log_data: bool,
+    project_fold_regularization: float,
+    project_min_significant_gene_umis: float,
+    project_filter_ranges: bool,
+    project_ignore_range_quantile: float,
+    project_ignore_range_min_overlap_fraction: float,
     project_max_consistency_fold_factor: float,
     project_candidates_count: int,
     project_min_usage_weight: float,
-    project_max_projection_fold_factor: float,
-    min_entry_project_fold_factor: float,
-    biased_min_metacells_fraction: float,
+    project_corrections: bool,
+    project_min_corrected_gene_correlation: float,
+    project_min_corrected_gene_factor: float,
     atlas_type_property_name: str,
-    project_abs_folds: bool,
     reproducible: bool,
 ) -> None:
-    ignored_mask_names = _initial_ignored_mask_names(
-        what=what,
-        common_adata=common_adata,
-        common_qdata=common_qdata,
-        atlas_total_common_umis=atlas_total_common_umis,
-        query_total_common_umis=query_total_common_umis,
-        ignore_atlas_insignificant_genes=ignore_atlas_insignificant_genes,
-        ignore_query_insignificant_genes=ignore_query_insignificant_genes,
-        ignore_atlas_forbidden_genes=ignore_atlas_forbidden_genes,
-        ignore_query_forbidden_genes=ignore_query_forbidden_genes,
-        systematic_low_gene_quantile=systematic_low_gene_quantile,
-        systematic_high_gene_quantile=systematic_high_gene_quantile,
-    )
-
-    included_adata = common_adata
-    included_qdata = common_qdata
+    correction_factor_per_gene = np.full(common_qdata.n_vars, 1.0, dtype="float32")
 
     repeat = 0
     while True:
         repeat += 1
-        ut.log_calc("biased repeat", repeat)
+        ut.log_calc("preliminary repeat", repeat)
 
-        weights, included_adata, included_qdata = _compute_global_projection(
-            what=what,
-            included_adata=included_adata,
-            included_qdata=included_qdata,
-            atlas_total_common_umis=atlas_total_common_umis,
-            query_total_common_umis=query_total_common_umis,
-            ignored_mask_names=ignored_mask_names,
-            project_fold_normalization=project_fold_normalization,
-            project_min_significant_gene_value=project_min_significant_gene_value,
+        fitted_adata, weights = _compute_correction_factors(
+            common_adata=common_adata,
+            common_qdata=common_qdata,
+            correction_factor_per_gene=correction_factor_per_gene,
+            preliminary_fitted_genes_mask=preliminary_fitted_genes_mask,
+            project_log_data=project_log_data,
+            project_fold_regularization=project_fold_regularization,
+            project_min_significant_gene_umis=project_min_significant_gene_umis,
             project_max_consistency_fold_factor=project_max_consistency_fold_factor,
             project_candidates_count=project_candidates_count,
             project_min_usage_weight=project_min_usage_weight,
-            project_max_projection_fold_factor=project_max_projection_fold_factor,
-            min_entry_project_fold_factor=min_entry_project_fold_factor,
-            project_abs_folds=project_abs_folds,
+            project_corrections=project_corrections,
+            project_min_corrected_gene_correlation=project_min_corrected_gene_correlation,
+            project_min_corrected_gene_factor=project_min_corrected_gene_factor,
             reproducible=reproducible,
         )
 
-        if not _detect_global_biased_genes(
-            weights=weights,
-            common_adata=common_adata,
-            common_qdata=common_qdata,
-            included_qdata=included_qdata,
-            project_max_projection_fold_factor=project_max_projection_fold_factor,
-            biased_min_metacells_fraction=biased_min_metacells_fraction,
-            atlas_type_property_name=atlas_type_property_name,
-            project_abs_folds=project_abs_folds,
+        if (
+            repeat > 2
+            or not project_filter_ranges
+            or not _filter_range_genes(
+                common_qdata=common_qdata,
+                project_fold_regularization=project_fold_regularization,
+                project_ignore_range_quantile=project_ignore_range_quantile,
+                project_ignore_range_min_overlap_fraction=project_ignore_range_min_overlap_fraction,
+                preliminary_fitted_genes_mask=preliminary_fitted_genes_mask,
+            )
         ):
+            ut.log_calc("preliminary last repeat", repeat)
             break
 
-        ignored_mask_names = ["biased_gene"]
+    if project_corrections:
+        ut.set_v_data(common_qdata, "correction_factor", correction_factor_per_gene)
 
-    _convey_query_included_to_common_data(common_qdata=common_qdata, included_qdata=included_qdata)
+    tl.convey_atlas_to_query(
+        adata=fitted_adata,
+        qdata=common_qdata,
+        weights=weights,
+        property_name=atlas_type_property_name,
+        to_property_name="projected_type",
+    )
 
 
-def _convey_query_included_to_common_data(
+@ut.logged()
+@ut.timed_call()
+def _compute_correction_factors(
     *,
+    common_adata: AnnData,
     common_qdata: AnnData,
-    included_qdata: AnnData,
-) -> None:
-    common_gene_index_of_included_qdata = ut.get_v_numpy(included_qdata, "common_gene_index_of_qdata")
-    ignored_genes_mask = np.full(common_qdata.n_vars, True)
-    ignored_genes_mask[common_gene_index_of_included_qdata] = False
-    ut.set_v_data(common_qdata, "ignored_gene", ignored_genes_mask)
+    correction_factor_per_gene: ut.NumpyVector,
+    preliminary_fitted_genes_mask: ut.NumpyVector,
+    project_log_data: bool,
+    project_fold_regularization: float,
+    project_min_significant_gene_umis: float,
+    project_max_consistency_fold_factor: float,
+    project_candidates_count: int,
+    project_min_usage_weight: float,
+    project_corrections: bool,
+    project_min_corrected_gene_correlation: float,
+    project_min_corrected_gene_factor: float,
+    reproducible: bool,
+) -> Tuple[AnnData, ut.ProperMatrix]:
+    repeat = 0
+    while True:
+        repeat += 1
+        ut.log_calc("corrections repeat", repeat)
 
-    projected_types = ut.get_o_numpy(included_qdata, "projected_type")
-    ut.set_o_data(common_qdata, "projected_type", projected_types)
+        fitted_adata = ut.slice(common_adata, name=".fitted", vars=preliminary_fitted_genes_mask, top_level=False)
 
+        fitted_qdata = ut.slice(
+            common_qdata,
+            name=".fitted",
+            vars=preliminary_fitted_genes_mask,
+            track_var="common_gene_index_of_qdata",
+            top_level=False,
+        )
 
-@ut.logged()
-@ut.timed_call()
-def _initial_ignored_mask_names(
+        weights = tl.compute_projection_weights(
+            adata=fitted_adata,
+            qdata=fitted_qdata,
+            log_data=project_log_data,
+            fold_regularization=project_fold_regularization,
+            min_significant_gene_umis=project_min_significant_gene_umis,
+            max_consistency_fold_factor=project_max_consistency_fold_factor,
+            candidates_count=project_candidates_count,
+            min_usage_weight=project_min_usage_weight,
+            reproducible=reproducible,
+        )
+
+        tl.compute_projected_fractions(
+            adata=common_adata,
+            qdata=common_qdata,
+            log_data=project_log_data,
+            fold_regularization=project_fold_regularization,
+            weights=weights,
+        )
+
+        if (
+            repeat > 2
+            or not project_corrections
+            or not _correct_correlated_genes(
+                common_adata=common_adata,
+                common_qdata=common_qdata,
+                preliminary_fitted_genes_mask=preliminary_fitted_genes_mask,
+                project_min_corrected_gene_correlation=project_min_corrected_gene_correlation,
+                project_min_corrected_gene_factor=project_min_corrected_gene_factor,
+                correction_factor_per_gene=correction_factor_per_gene,
+                reproducible=reproducible,
+            )
+        ):
+            ut.log_calc("corrections last repeat", repeat)
+            return fitted_adata, weights
+
+
+def _correct_correlated_genes(
     *,
-    what: str,
     common_adata: AnnData,
     common_qdata: AnnData,
-    atlas_total_common_umis: ut.NumpyVector,
-    query_total_common_umis: ut.NumpyVector,
-    ignore_atlas_insignificant_genes: bool,
-    ignore_query_insignificant_genes: bool,
-    ignore_atlas_forbidden_genes: bool,
-    ignore_query_forbidden_genes: bool,
-    systematic_low_gene_quantile: float,
-    systematic_high_gene_quantile: float,
-) -> List[str]:
-    ignored_mask_names = ["|uncorrelated_gene", "|manually_ignored_gene?"]
+    preliminary_fitted_genes_mask: ut.NumpyVector,
+    project_min_corrected_gene_correlation: float,
+    project_min_corrected_gene_factor: float,
+    correction_factor_per_gene: ut.NumpyVector,
+    reproducible: bool,
+) -> bool:
+    corrected_fractions_per_gene_per_metacell = ut.to_numpy_matrix(
+        ut.get_vo_proper(common_qdata, "corrected_fraction", layout="column_major")
+    )
 
-    tl.find_systematic_genes(
-        what,
-        adata=common_adata,
-        qdata=common_qdata,
-        atlas_total_umis=atlas_total_common_umis,
-        query_total_umis=query_total_common_umis,
-        low_gene_quantile=systematic_low_gene_quantile,
-        high_gene_quantile=systematic_high_gene_quantile,
+    projected_fractions_per_gene_per_metacell = ut.to_numpy_matrix(
+        ut.get_vo_proper(common_qdata, "projected_fraction", layout="column_major")
     )
-    ignored_mask_names.append("|systematic_gene")
 
-    if ignore_atlas_insignificant_genes:
-        ignored_mask_names.append("|~atlas_significant_gene")
+    preliminary_fitted_genes_indices = np.where(preliminary_fitted_genes_mask)[0]
+    corrected_fractions_per_fitted_gene_per_metacell = corrected_fractions_per_gene_per_metacell[
+        :, preliminary_fitted_genes_indices
+    ]
+    projected_fractions_per_fitted_gene_per_metacell = projected_fractions_per_gene_per_metacell[
+        :, preliminary_fitted_genes_indices
+    ]
+
+    correlation_per_fitted_gene = np.full(len(preliminary_fitted_genes_indices), -2, dtype="float32")
+    correlation_per_fitted_gene = ut.pairs_corrcoef_rows(
+        corrected_fractions_per_fitted_gene_per_metacell.transpose(),
+        projected_fractions_per_fitted_gene_per_metacell.transpose(),
+        reproducible=reproducible,
+    )
 
-    if ignore_query_insignificant_genes:
-        ignored_mask_names.append("|~significant_gene")
+    correlated_fitted_genes_mask = correlation_per_fitted_gene >= project_min_corrected_gene_correlation
+    ut.log_calc("correlated_fitted_genes_mask", correlated_fitted_genes_mask)
+    if not np.any(correlated_fitted_genes_mask):
+        return False
 
-    if ignore_atlas_forbidden_genes:
-        ignored_mask_names.append("|atlas_forbidden_gene")
+    total_corrected_fractions_per_fitted_gene = ut.sum_per(
+        corrected_fractions_per_fitted_gene_per_metacell, per="column"
+    )
+    total_projected_fractions_per_fitted_gene = ut.sum_per(
+        projected_fractions_per_fitted_gene_per_metacell, per="column"
+    )
 
-    if ignore_query_forbidden_genes:
-        ignored_mask_names.append("|forbidden_gene")
+    zero_fitted_genes_mask = (total_projected_fractions_per_fitted_gene == 0) | (
+        total_corrected_fractions_per_fitted_gene == 0
+    )
+    ut.log_calc("zero_fitted_genes_mask", zero_fitted_genes_mask)
+    total_corrected_fractions_per_fitted_gene[zero_fitted_genes_mask] = 1.0
+    total_projected_fractions_per_fitted_gene[zero_fitted_genes_mask] = 1.0
 
-    return ignored_mask_names
+    current_correction_factor_per_fitted_gene = (
+        total_projected_fractions_per_fitted_gene / total_corrected_fractions_per_fitted_gene
+    )
+
+    high_factor = 1 + project_min_corrected_gene_factor
+    low_factor = 1.0 / high_factor
+    factor_fitted_genes_mask = (current_correction_factor_per_fitted_gene <= low_factor) | (
+        current_correction_factor_per_fitted_gene >= high_factor
+    )
+    factor_genes_mask = np.zeros(common_adata.n_vars, dtype="bool")
+    factor_genes_mask[preliminary_fitted_genes_indices] = factor_fitted_genes_mask
+    ut.log_calc("factor_fitted_genes_mask", factor_fitted_genes_mask)
+    if not np.any(factor_fitted_genes_mask):
+        return False
+
+    corrected_fitted_genes_mask = correlated_fitted_genes_mask & factor_fitted_genes_mask
+    ut.log_calc("corrected_fitted_genes_mask", corrected_fitted_genes_mask)
+    if not np.any(corrected_fitted_genes_mask):
+        return False
+
+    corrected_genes_mask = np.zeros(common_adata.n_vars, dtype="bool")
+    corrected_genes_mask[preliminary_fitted_genes_indices] = corrected_fitted_genes_mask
+    ut.log_calc("corrected_genes_mask", corrected_genes_mask)
+
+    correction_factor_per_corrected_gene = current_correction_factor_per_fitted_gene[corrected_fitted_genes_mask]
+    correction_factor_per_gene[corrected_genes_mask] *= correction_factor_per_corrected_gene
+
+    corrected_fractions_per_gene_per_metacell[:, corrected_genes_mask] *= correction_factor_per_corrected_gene[
+        np.newaxis, :
+    ]
+    corrected_fractions_per_gene_per_metacell = ut.fraction_by(  # type: ignore
+        ut.to_layout(corrected_fractions_per_gene_per_metacell, layout="row_major"), by="row"
+    )
+    ut.set_vo_data(common_qdata, "corrected_fraction", sp.csr_matrix(corrected_fractions_per_gene_per_metacell))
+
+    return True
 
 
 @ut.logged()
 @ut.timed_call()
-def _compute_global_projection(
+def _filter_range_genes(
     *,
-    what: str,
-    included_adata: AnnData,
-    included_qdata: AnnData,
-    atlas_total_common_umis: ut.NumpyVector,
-    query_total_common_umis: ut.NumpyVector,
-    ignored_mask_names: List[str],
-    project_fold_normalization: float,
-    project_min_significant_gene_value: float,
-    project_max_consistency_fold_factor: float,
-    project_candidates_count: int,
-    project_min_usage_weight: float,
-    project_max_projection_fold_factor: float,
-    min_entry_project_fold_factor: float,
-    project_abs_folds: bool,
-    reproducible: bool,
-) -> Tuple[ut.CompressedMatrix, AnnData, AnnData]:
-    tl.combine_masks(included_qdata, ignored_mask_names, to="ignored_gene")
-    included_genes_mask = ~ut.get_v_numpy(included_qdata, "ignored_gene")
+    common_qdata: AnnData,
+    project_fold_regularization: float,
+    project_ignore_range_quantile: float,
+    project_ignore_range_min_overlap_fraction: float,
+    preliminary_fitted_genes_mask: ut.NumpyVector,
+) -> bool:
+    corrected_fractions_per_gene_per_metacell = ut.to_numpy_matrix(
+        ut.get_vo_proper(common_qdata, "corrected_fraction", layout="column_major")
+    )
+    projected_fractions_per_gene_per_metacell = ut.to_numpy_matrix(
+        ut.get_vo_proper(common_qdata, "projected_fraction", layout="column_major")
+    )
 
-    included_adata = ut.slice(included_adata, name=".included", vars=included_genes_mask)
-    included_qdata = ut.slice(included_qdata, name=".included", vars=included_genes_mask)
+    preliminary_fitted_genes_indices = np.where(preliminary_fitted_genes_mask)[0]
 
-    weights = tl.project_query_onto_atlas(
-        what,
-        adata=included_adata,
-        qdata=included_qdata,
-        atlas_total_umis=atlas_total_common_umis,
-        query_total_umis=query_total_common_umis,
-        fold_normalization=project_fold_normalization,
-        min_significant_gene_value=project_min_significant_gene_value,
-        max_consistency_fold_factor=project_max_consistency_fold_factor,
-        candidates_count=project_candidates_count,
-        min_usage_weight=project_min_usage_weight,
-        reproducible=reproducible,
-    )
+    corrected_fractions_per_fitted_gene_per_metacell = corrected_fractions_per_gene_per_metacell[
+        :, preliminary_fitted_genes_indices
+    ]
+    projected_fractions_per_fitted_gene_per_metacell = projected_fractions_per_gene_per_metacell[
+        :, preliminary_fitted_genes_indices
+    ]
 
-    tl.compute_query_projection(
-        adata=included_adata,
-        qdata=included_qdata,
-        weights=weights,
-        atlas_total_umis=atlas_total_common_umis,
-        query_total_umis=query_total_common_umis,
+    corrected_log_fractions_per_fitted_gene_per_metacell = (
+        corrected_fractions_per_fitted_gene_per_metacell + project_fold_regularization
+    )
+    projected_log_fractions_per_fitted_gene_per_metacell = (
+        projected_fractions_per_fitted_gene_per_metacell + project_fold_regularization
     )
 
-    tl.compute_significant_projected_fold_factors(
-        included_qdata,
-        what,
-        total_umis=query_total_common_umis,
-        fold_normalization=project_fold_normalization,
-        min_gene_fold_factor=project_max_projection_fold_factor,
-        min_entry_fold_factor=min_entry_project_fold_factor,
-        min_significant_gene_value=project_min_significant_gene_value,
-        abs_folds=project_abs_folds,
+    np.log2(
+        corrected_log_fractions_per_fitted_gene_per_metacell, out=corrected_log_fractions_per_fitted_gene_per_metacell
+    )
+    np.log2(
+        projected_log_fractions_per_fitted_gene_per_metacell, out=projected_log_fractions_per_fitted_gene_per_metacell
     )
 
-    return weights, included_adata, included_qdata
+    low_corrected_log_fractions_per_fitted_gene = ut.quantile_per(
+        corrected_log_fractions_per_fitted_gene_per_metacell, project_ignore_range_quantile, per="column"
+    )
+    low_projected_log_fractions_per_fitted_gene = ut.quantile_per(
+        projected_log_fractions_per_fitted_gene_per_metacell, project_ignore_range_quantile, per="column"
+    )
 
+    high_corrected_log_fractions_per_fitted_gene = ut.quantile_per(
+        corrected_log_fractions_per_fitted_gene_per_metacell, 1.0 - project_ignore_range_quantile, per="column"
+    )
+    high_projected_log_fractions_per_fitted_gene = ut.quantile_per(
+        projected_log_fractions_per_fitted_gene_per_metacell, 1.0 - project_ignore_range_quantile, per="column"
+    )
 
-def _detect_global_biased_genes(
-    *,
-    weights: ut.CompressedMatrix,
-    common_adata: AnnData,
-    common_qdata: AnnData,
-    included_qdata: AnnData,
-    project_max_projection_fold_factor: float,
-    biased_min_metacells_fraction: float,
-    atlas_type_property_name: str,
-    project_abs_folds: bool,
-) -> bool:
-    tl.project_atlas_to_query(
-        adata=common_adata,
-        qdata=included_qdata,
-        weights=weights,
-        property_name=atlas_type_property_name,
-        to_property_name="projected_type",
+    low_common_log_fractions_per_fitted_gene = np.maximum(
+        low_corrected_log_fractions_per_fitted_gene, low_projected_log_fractions_per_fitted_gene
+    )
+    high_common_log_fractions_per_fitted_gene = np.minimum(
+        high_corrected_log_fractions_per_fitted_gene, high_projected_log_fractions_per_fitted_gene
     )
 
-    tl.find_biased_genes(
-        included_qdata,
-        max_projection_fold_factor=project_max_projection_fold_factor,
-        min_metacells_fraction=biased_min_metacells_fraction,
-        abs_folds=project_abs_folds,
+    corrected_range_log_fractions_per_fitted_gene = (
+        high_corrected_log_fractions_per_fitted_gene - low_corrected_log_fractions_per_fitted_gene
     )
+    common_range_log_fractions_per_fitted_gene = (
+        high_common_log_fractions_per_fitted_gene - low_common_log_fractions_per_fitted_gene
+    )
+
+    corrected_range_log_fractions_per_fitted_gene[corrected_range_log_fractions_per_fitted_gene == 0] = 1
+    overlap_per_fitted_gene = common_range_log_fractions_per_fitted_gene / corrected_range_log_fractions_per_fitted_gene
 
-    included_biased_genes_mask = ut.get_v_numpy(included_qdata, "biased_gene")
-    if not np.any(included_biased_genes_mask):
+    ignore_fitted_genes_mask = overlap_per_fitted_gene < project_ignore_range_min_overlap_fraction
+    ut.log_calc("ignore_fitted_genes_mask", ignore_fitted_genes_mask)
+    if not np.any(ignore_fitted_genes_mask):
         return False
 
-    common_biased_genes_mask = ut.get_v_numpy(common_qdata, "biased_gene").copy()
-    common_gene_index_of_included_qdata = ut.get_v_numpy(included_qdata, "common_gene_index_of_qdata")
-    common_biased_genes_mask[common_gene_index_of_included_qdata] = included_biased_genes_mask
-    ut.set_v_data(common_qdata, "biased_gene", common_biased_genes_mask)
+    ignore_gene_indices = preliminary_fitted_genes_indices[ignore_fitted_genes_mask]
+    preliminary_fitted_genes_mask[ignore_gene_indices] = False
+    ut.log_calc("preliminary_fitted_genes_mask", preliminary_fitted_genes_mask)
 
     return True
 
 
 @ut.logged()
 @ut.timed_call()
-def _compute_per_type_projection(  # pylint: disable=too-many-statements
+def _compute_per_type_projection(
     *,
-    what: str,
     common_adata: AnnData,
     common_qdata: AnnData,
-    atlas_total_common_umis: ut.NumpyVector,
-    query_total_common_umis: ut.NumpyVector,
-    systematic_low_gene_quantile: float,
-    systematic_high_gene_quantile: float,
-    biased_min_metacells_fraction: float,
-    project_fold_normalization: float,
+    type_names: List[str],
+    preliminary_fitted_genes_mask: ut.NumpyVector,
+    misfit_min_metacells_fraction: float,
+    project_log_data: bool,
+    project_fold_regularization: float,
     project_candidates_count: int,
-    project_min_significant_gene_value: float,
+    project_min_significant_gene_umis: float,
     project_min_usage_weight: float,
     project_max_consistency_fold_factor: float,
     project_max_projection_fold_factor: float,
-    project_max_dissimilar_genes: int,
-    min_entry_project_fold_factor: float,
-    project_abs_folds: bool,
+    project_max_projection_noisy_fold_factor: float,
+    project_max_misfit_genes: int,
+    min_fitted_query_marker_genes: float,
+    min_essential_genes_of_type: Dict[Tuple[str, str], Optional[int]],
     atlas_type_property_name: str,
     top_level_parallel: bool,
     reproducible: bool,
 ) -> ut.NumpyMatrix:
-    taboo_types: List[Set[str]] = []
+    old_types_per_metacell: List[Set[str]] = []
     for _metacell_index in range(common_qdata.n_obs):
-        taboo_types.append(set())
+        old_types_per_metacell.append(set())
+
+    fitted_genes_mask_per_type = _initial_fitted_genes_mask_per_type(
+        common_qdata=common_qdata, type_names=type_names, preliminary_fitted_genes_mask=preliminary_fitted_genes_mask
+    )
+
+    misfit_per_gene_per_metacell = np.empty(common_qdata.shape, dtype="bool")
+    projected_correlation_per_metacell = np.empty(common_qdata.n_obs, dtype="float32")
+    projected_fold_per_gene_per_metacell = np.empty(common_qdata.shape, dtype="float32")
+    weights_per_atlas_per_query_metacell = np.empty((common_qdata.n_obs, common_adata.n_obs), dtype="float32")
+    similar_per_metacell = np.empty(common_qdata.n_obs, dtype="bool")
 
     repeat = 0
     while True:
         repeat += 1
         ut.log_calc("types repeat", repeat)
 
-        all_types = np.unique(ut.get_o_numpy(common_adata, atlas_type_property_name))
-        for type_name in all_types:
-            for data_name in ["systematic_gene", "biased_gene", "ignored_gene"]:
-                full_name = f"{data_name}_of_{type_name}"
-                if full_name in common_qdata.var:
-                    del common_qdata.var[full_name]
-
-        type_of_atlas_metacells = ut.get_o_numpy(common_adata, atlas_type_property_name)
-        atlas_unique_types = np.unique(type_of_atlas_metacells)
-
         type_of_query_metacells = ut.get_o_numpy(common_qdata, "projected_type")
-        query_unique_types = np.unique(type_of_query_metacells)
+        query_type_names = list(np.unique(type_of_query_metacells))
 
-        similar = np.zeros(common_qdata.n_obs, dtype="bool")
-        dissimilar_genes_count = np.zeros(common_qdata.n_obs, dtype="int32")
-        weights = np.zeros((common_qdata.n_obs, common_adata.n_obs), dtype="float32")
-        projected_folds = np.zeros(common_qdata.shape, dtype="float32")
-        systematic_gene_of_types = np.zeros((len(query_unique_types), common_qdata.n_vars), dtype="bool")
-        biased_gene_of_types = np.zeros((len(query_unique_types), common_qdata.n_vars), dtype="bool")
-        ignored_gene_of_types = np.zeros((len(query_unique_types), common_qdata.n_vars), dtype="bool")
+        misfit_per_gene_per_metacell[:, :] = False
+        projected_fold_per_gene_per_metacell[:, :] = 0.0
 
         @ut.timed_call("single_type_projection")
         def _single_type_projection(
             type_index: int,
-        ) -> Tuple[
-            ut.NumpyVector,
-            ut.NumpyVector,
-            ut.ProperMatrix,
-            ut.ProperMatrix,
-            ut.NumpyVector,
-            ut.NumpyVector,
-            ut.NumpyVector,
-        ]:
+        ) -> Dict[str, Any]:
             return _compute_single_type_projection(
-                what=what,
-                type_name=query_unique_types[type_index],
+                type_name=query_type_names[type_index],
                 common_adata=common_adata,
                 common_qdata=common_qdata,
-                atlas_total_common_umis=atlas_total_common_umis,
-                query_total_common_umis=query_total_common_umis,
-                systematic_low_gene_quantile=systematic_low_gene_quantile,
-                systematic_high_gene_quantile=systematic_high_gene_quantile,
-                biased_min_metacells_fraction=biased_min_metacells_fraction,
-                project_fold_normalization=project_fold_normalization,
+                fitted_genes_mask_per_type=fitted_genes_mask_per_type,
+                misfit_min_metacells_fraction=misfit_min_metacells_fraction,
+                project_log_data=project_log_data,
+                project_fold_regularization=project_fold_regularization,
                 project_candidates_count=project_candidates_count,
-                project_min_significant_gene_value=project_min_significant_gene_value,
+                project_min_significant_gene_umis=project_min_significant_gene_umis,
                 project_min_usage_weight=project_min_usage_weight,
                 project_max_consistency_fold_factor=project_max_consistency_fold_factor,
                 project_max_projection_fold_factor=project_max_projection_fold_factor,
-                project_max_dissimilar_genes=project_max_dissimilar_genes,
-                min_entry_project_fold_factor=min_entry_project_fold_factor,
-                project_abs_folds=project_abs_folds,
-                atlas_type_property_name=atlas_type_property_name,
+                project_max_projection_noisy_fold_factor=project_max_projection_noisy_fold_factor,
+                project_max_misfit_genes=project_max_misfit_genes,
+                min_fitted_query_marker_genes=min_fitted_query_marker_genes,
+                min_essential_genes_of_type=min_essential_genes_of_type,
                 top_level_parallel=top_level_parallel,
                 reproducible=reproducible,
             )
 
-        def _collect_type_result(
+        @ut.logged()
+        def _collect_single_type_result(
             type_index: int,
-            similar_of_type: ut.NumpyVector,
-            dissimilar_genes_count_of_type: ut.NumpyVector,
-            weights_of_type: ut.ProperMatrix,
-            projected_folds_of_type: ut.ProperMatrix,
-            systematic_gene_of_type: ut.NumpyVector,
-            biased_gene_of_type: ut.NumpyVector,
-            ignored_gene_of_type: ut.NumpyVector,
+            *,
+            query_metacell_indices_of_type: ut.NumpyVector,
+            fitted_genes_indices_of_type: ut.NumpyVector,
+            similar_per_metacell_of_type: ut.NumpyVector,
+            misfit_per_gene_per_metacell_of_type: ut.ProperMatrix,
+            projected_correlation_per_metacell_of_type: ut.NumpyVector,
+            projected_fold_per_gene_per_metacell_of_type: ut.ProperMatrix,
+            weights_per_atlas_per_query_metacell_of_type: ut.ProperMatrix,
         ) -> None:
-            nonlocal similar
-            similar |= similar_of_type
-            nonlocal dissimilar_genes_count
-            dissimilar_genes_count += dissimilar_genes_count_of_type
-            nonlocal weights
-            weights += weights_of_type  # type: ignore
-            nonlocal projected_folds
-            projected_folds += projected_folds_of_type  # type: ignore
-            nonlocal systematic_gene_of_types
-            systematic_gene_of_types[type_index, :] = systematic_gene_of_type
-            nonlocal biased_gene_of_types
-            biased_gene_of_types[type_index, :] = biased_gene_of_type
-            nonlocal ignored_gene_of_types
-            ignored_gene_of_types[type_index, :] = ignored_gene_of_type
-
-        if top_level_parallel:
-            for type_index, result in enumerate(ut.parallel_map(_single_type_projection, len(query_unique_types))):
-                _collect_type_result(type_index, *result)
-        else:
-            for type_index in range(len(query_unique_types)):
-                result = _single_type_projection(type_index)
-                _collect_type_result(type_index, *result)
-
-        for type_index, type_name in enumerate(query_unique_types):
-            ut.set_v_data(
-                common_qdata,
-                f"systematic_gene_of_{type_name}",
-                ut.to_numpy_vector(systematic_gene_of_types[type_index, :]),
+            fitted_genes_mask_per_type[query_type_names[type_index]][:] = False
+            fitted_genes_mask_per_type[query_type_names[type_index]][fitted_genes_indices_of_type] = True
+            similar_per_metacell[query_metacell_indices_of_type] = similar_per_metacell_of_type
+            projected_correlation_per_metacell[
+                query_metacell_indices_of_type
+            ] = projected_correlation_per_metacell_of_type
+            misfit_per_gene_per_metacell[query_metacell_indices_of_type, :] = ut.to_numpy_matrix(
+                misfit_per_gene_per_metacell_of_type
             )
-            ut.set_v_data(
-                common_qdata, f"biased_gene_of_{type_name}", ut.to_numpy_vector(biased_gene_of_types[type_index, :])
+            projected_fold_per_gene_per_metacell[query_metacell_indices_of_type, :] = ut.to_numpy_matrix(
+                projected_fold_per_gene_per_metacell_of_type
             )
-            ut.set_v_data(
-                common_qdata, f"ignored_gene_of_{type_name}", ut.to_numpy_vector(ignored_gene_of_types[type_index, :])
+            weights_per_atlas_per_query_metacell[query_metacell_indices_of_type, :] = ut.to_numpy_matrix(
+                weights_per_atlas_per_query_metacell_of_type
             )
 
-        for type_name in set(atlas_unique_types) - set(query_unique_types):
-            ut.set_v_data(common_qdata, f"systematic_gene_of_{type_name}", np.zeros(common_qdata.n_vars, dtype="bool"))
-            ut.set_v_data(common_qdata, f"biased_gene_of_{type_name}", np.zeros(common_qdata.n_vars, dtype="bool"))
-            ut.set_v_data(common_qdata, f"ignored_gene_of_{type_name}", np.zeros(common_qdata.n_vars, dtype="bool"))
-
-        ut.set_o_data(common_qdata, "similar", similar)
-        ut.log_calc("max dissimilar_genes_count", np.max(dissimilar_genes_count))
-        ut.set_o_data(common_qdata, "dissimilar_genes_count", dissimilar_genes_count, formatter=ut.mask_description)
+        if top_level_parallel:
+            for type_index, result in enumerate(ut.parallel_map(_single_type_projection, len(query_type_names))):
+                _collect_single_type_result(type_index, **result)
+        else:
+            for type_index in range(len(query_type_names)):
+                result = _single_type_projection(type_index)
+                _collect_single_type_result(type_index, **result)
 
         if repeat > 2 or not _changed_projected_types(
             common_adata=common_adata,
             common_qdata=common_qdata,
-            weights=weights,
+            old_type_of_query_metacells=type_of_query_metacells,
+            weights_per_atlas_per_query_metacell=weights_per_atlas_per_query_metacell,
             atlas_type_property_name=atlas_type_property_name,
-            taboo_types=taboo_types,
+            old_types_per_metacell=old_types_per_metacell,
         ):
+            ut.log_calc("types last repeat", repeat)
             break
 
-    tl.compute_query_projection(
+    for type_name, fitted_genes_mask_of_type in fitted_genes_mask_per_type.items():
+        ut.set_v_data(common_qdata, f"fitted_gene_of_{type_name}", fitted_genes_mask_of_type)
+
+    projected_type_per_metacell = ut.get_o_numpy(common_qdata, "projected_type")
+    fitted_mask_per_gene_per_metacell = np.vstack(
+        [fitted_genes_mask_per_type[type_name] for type_name in projected_type_per_metacell]
+    )
+    ut.set_vo_data(common_qdata, "fitted", fitted_mask_per_gene_per_metacell)
+
+    ut.set_o_data(common_qdata, "similar", similar_per_metacell)
+    ut.set_o_data(common_qdata, "projected_correlation", projected_correlation_per_metacell)
+
+    ut.set_vo_data(common_qdata, "misfit", misfit_per_gene_per_metacell)
+    ut.set_vo_data(common_qdata, "projected_fold", projected_fold_per_gene_per_metacell)
+
+    tl.compute_projected_fractions(
         adata=common_adata,
         qdata=common_qdata,
-        weights=weights,
-        atlas_total_umis=atlas_total_common_umis,
-        query_total_umis=query_total_common_umis,
+        log_data=project_log_data,
+        fold_regularization=project_fold_regularization,
+        weights=weights_per_atlas_per_query_metacell,
     )
 
-    ut.set_vo_data(common_qdata, "projected_fold", projected_folds)
+    return weights_per_atlas_per_query_metacell
 
-    return weights
+
+def _initial_fitted_genes_mask_per_type(
+    common_qdata: AnnData,
+    type_names: List[str],
+    preliminary_fitted_genes_mask: ut.NumpyVector,
+) -> Dict[str, ut.NumpyVector]:
+    fitted_genes_mask_per_type: Dict[str, ut.NumpyVector] = {}
+    for type_name in type_names:
+        fitted_genes_mask_of_type = preliminary_fitted_genes_mask.copy()
+        property_name = f"ignored_gene_of_{type_name}"
+        if ut.has_data(common_qdata, property_name):
+            ignored_gene_mask_of_type = ut.get_v_numpy(common_qdata, property_name)
+            fitted_genes_mask_of_type &= ~ignored_gene_mask_of_type
+        fitted_genes_mask_per_type[type_name] = fitted_genes_mask_of_type
+    return fitted_genes_mask_per_type
 
 
 @ut.logged()
 @ut.timed_call()
 def _compute_single_type_projection(
     *,
-    what: str,
     type_name: str,
     common_adata: AnnData,
     common_qdata: AnnData,
-    atlas_total_common_umis: ut.NumpyVector,
-    query_total_common_umis: ut.NumpyVector,
-    systematic_low_gene_quantile: float,
-    systematic_high_gene_quantile: float,
-    biased_min_metacells_fraction: float,
-    project_fold_normalization: float,
+    fitted_genes_mask_per_type: Dict[str, ut.NumpyVector],
+    misfit_min_metacells_fraction: float,
+    project_log_data: bool,
+    project_fold_regularization: float,
     project_candidates_count: int,
-    project_min_significant_gene_value: float,
+    project_min_significant_gene_umis: float,
     project_min_usage_weight: float,
     project_max_consistency_fold_factor: float,
     project_max_projection_fold_factor: float,
-    project_max_dissimilar_genes: int,
-    min_entry_project_fold_factor: float,
-    project_abs_folds: bool,
-    atlas_type_property_name: str,
+    project_max_projection_noisy_fold_factor: float,
+    project_max_misfit_genes: int,
+    min_fitted_query_marker_genes: float,
+    min_essential_genes_of_type: Dict[Tuple[str, str], Optional[int]],
     top_level_parallel: bool,
     reproducible: bool,
-) -> Tuple[
-    ut.NumpyVector,
-    ut.NumpyVector,
-    ut.NumpyMatrix,
-    ut.NumpyMatrix,
-    ut.NumpyVector,
-    ut.NumpyVector,
-    ut.NumpyVector,
-]:
-    similar = np.zeros(common_qdata.n_obs, dtype="bool")
-    dissimilar_genes_count = np.zeros(common_qdata.n_obs, dtype="int32")
-    weights = np.zeros((common_qdata.n_obs, common_adata.n_obs), dtype="float32")
-    projected_folds = np.zeros(common_qdata.shape, dtype="float32")
-    systematic_gene_of_type = np.zeros(common_qdata.n_vars, dtype="bool")
-    biased_gene_of_type = np.zeros(common_qdata.n_vars, dtype="bool")
-    ignored_gene_of_type = np.zeros(common_qdata.n_vars, dtype="bool")
+) -> Dict[str, Any]:
+    projected_type_per_metacell = ut.get_o_numpy(common_qdata, "projected_type")
+    query_metacell_mask_of_type = projected_type_per_metacell == type_name
+    ut.log_calc("query_metacell_mask_of_type", query_metacell_mask_of_type)
+    assert np.any(query_metacell_mask_of_type)
+    type_common_qdata = ut.slice(common_qdata, name=f".{type_name}", obs=query_metacell_mask_of_type, top_level=False)
+    corrected_fractions = ut.get_vo_proper(type_common_qdata, "corrected_fraction")
 
-    (
-        type_common_adata,
-        type_common_qdata,
-        atlas_type_total_common_umis,
-        query_type_total_common_umis,
-    ) = _common_type_data(
-        type_name=type_name,
-        common_adata=common_adata,
-        common_qdata=common_qdata,
-        atlas_total_common_umis=atlas_total_common_umis,
-        query_total_common_umis=query_total_common_umis,
-        atlas_type_property_name=atlas_type_property_name,
-    )
-
-    type_ignored_mask_names = _initial_type_ignored_mask_names(
-        what=what,
-        type_name=type_name,
-        type_common_adata=type_common_adata,
-        type_common_qdata=type_common_qdata,
-        atlas_type_total_common_umis=atlas_type_total_common_umis,
-        query_type_total_common_umis=query_type_total_common_umis,
-        systematic_low_gene_quantile=systematic_low_gene_quantile,
-        systematic_high_gene_quantile=systematic_high_gene_quantile,
-        systematic_gene_of_type=systematic_gene_of_type,
-    )
-
-    type_included_adata = common_adata
-    type_included_qdata = type_common_qdata
+    fitted_genes_mask_of_type = fitted_genes_mask_per_type[type_name]
+    assert np.any(fitted_genes_mask_of_type)
 
     repeat = 0
     while True:
         repeat += 1
-        ut.log_calc(f"{type_name} biased repeat", repeat)
+        ut.log_calc(f"{type_name} misfit repeat", repeat)
 
-        type_included_adata, type_included_qdata, type_weights = _compute_type_projection(
-            what=what,
-            type_name=type_name,
-            type_included_adata=type_included_adata,
-            type_included_qdata=type_included_qdata,
-            atlas_total_common_umis=atlas_total_common_umis,
-            query_type_total_common_umis=query_type_total_common_umis,
-            type_ignored_mask_names=type_ignored_mask_names,
-            project_fold_normalization=project_fold_normalization,
-            project_min_significant_gene_value=project_min_significant_gene_value,
-            project_max_consistency_fold_factor=project_max_consistency_fold_factor,
-            project_candidates_count=project_candidates_count,
-            project_min_usage_weight=project_min_usage_weight,
-            project_max_projection_fold_factor=project_max_projection_fold_factor,
-            min_entry_project_fold_factor=min_entry_project_fold_factor,
-            project_abs_folds=project_abs_folds,
+        type_fitted_adata = ut.slice(
+            common_adata, name=f".{type_name}.fitted", vars=fitted_genes_mask_of_type, top_level=False
+        )
+
+        type_fitted_qdata = ut.slice(
+            type_common_qdata,
+            name=".fitted",
+            vars=fitted_genes_mask_of_type,
+            track_var="common_gene_index_of_qdata",
+            top_level=False,
+        )
+
+        type_weights = tl.compute_projection_weights(
+            adata=type_fitted_adata,
+            qdata=type_fitted_qdata,
+            log_data=project_log_data,
+            fold_regularization=project_fold_regularization,
+            min_significant_gene_umis=project_min_significant_gene_umis,
+            max_consistency_fold_factor=project_max_consistency_fold_factor,
+            candidates_count=project_candidates_count,
+            min_usage_weight=project_min_usage_weight,
             reproducible=reproducible,
         )
-        if not _detect_type_biased_genes(
-            type_name=type_name,
-            type_included_qdata=type_included_qdata,
-            project_max_projection_fold_factor=project_max_projection_fold_factor,
-            biased_min_metacells_fraction=biased_min_metacells_fraction,
-            project_abs_folds=project_abs_folds,
-            biased_gene_of_type=biased_gene_of_type,
+
+        tl.compute_projected_fractions(
+            adata=common_adata,
+            qdata=type_common_qdata,
+            log_data=project_log_data,
+            fold_regularization=project_fold_regularization,
+            weights=type_weights,
+        )
+        projected_fractions = ut.get_vo_proper(type_common_qdata, "projected_fraction")
+
+        tl.compute_projected_folds(
+            type_common_qdata,
+            fold_regularization=project_fold_regularization,
+            min_significant_gene_umis=project_min_significant_gene_umis,
+        )
+        projected_fold_per_gene_per_metacell_of_type = ut.get_vo_proper(type_common_qdata, "projected_fold")
+
+        if not _detect_type_misfit_genes(
+            type_common_qdata=type_common_qdata,
+            projected_fold_per_gene_per_metacell_of_type=projected_fold_per_gene_per_metacell_of_type,
+            max_projection_fold_factor=project_max_projection_fold_factor,
+            max_projection_noisy_fold_factor=project_max_projection_noisy_fold_factor,
+            misfit_min_metacells_fraction=misfit_min_metacells_fraction,
+            fitted_genes_mask_of_type=fitted_genes_mask_of_type,
         ):
+            ut.log_calc(f"{type_name} misfit last repeat", repeat)
             break
-        type_ignored_mask_names = [f"biased_gene_of_{type_name}"]
 
     tl.compute_similar_query_metacells(
-        type_included_qdata,
+        type_common_qdata,
         max_projection_fold_factor=project_max_projection_fold_factor,
-        max_dissimilar_genes=project_max_dissimilar_genes,
-        abs_folds=project_abs_folds,
-    )
-
-    _convey_query_type_to_common_data(
-        type_weights=type_weights,
-        weights=weights,
-        projected_folds=projected_folds,
-        type_included_qdata=type_included_qdata,
-        similar=similar,
-        dissimilar_genes_count=dissimilar_genes_count,
-        ignored_gene_of_type=ignored_gene_of_type,
+        max_projection_noisy_fold_factor=project_max_projection_noisy_fold_factor,
+        max_misfit_genes=project_max_misfit_genes,
+        min_fitted_query_marker_genes=min_fitted_query_marker_genes,
+        essential_genes_property=f"essential_gene_of_{type_name}",
+        min_essential_genes=min_essential_genes_of_type[(type_name, type_name)],
+        fitted_genes_mask=fitted_genes_mask_of_type,
+    )
+    similar_per_metacell_of_type = ut.get_o_numpy(type_common_qdata, "similar")
+    misfit_per_gene_per_metacell_of_type = ut.get_vo_proper(type_common_qdata, "misfit")
+
+    fitted_corrected_fractions = corrected_fractions[:, fitted_genes_mask_of_type]
+    fitted_projected_fractions = projected_fractions[:, fitted_genes_mask_of_type]
+    projected_correlation_per_metacell_of_type = ut.pairs_corrcoef_rows(
+        ut.to_layout(ut.to_numpy_matrix(fitted_corrected_fractions), layout="row_major"),
+        ut.to_layout(ut.to_numpy_matrix(fitted_projected_fractions), layout="row_major"),
+        reproducible=reproducible,
     )
 
     if top_level_parallel:
-        weights = sp.csr_matrix(weights)
-        projected_folds = sp.csr_matrix(projected_folds)
+        if not isinstance(misfit_per_gene_per_metacell_of_type, sp.csr_matrix):
+            misfit_per_gene_per_metacell_of_type = sp.csr_matrix(misfit_per_gene_per_metacell_of_type)
+        if not isinstance(projected_fold_per_gene_per_metacell_of_type, sp.csr_matrix):
+            projected_fold_per_gene_per_metacell_of_type = sp.csr_matrix(projected_fold_per_gene_per_metacell_of_type)
+        if not isinstance(type_weights, sp.csr_matrix):
+            type_weights = sp.csr_matrix(type_weights)
+
+    ut.log_return("query_metacell_mask_of_type", query_metacell_mask_of_type)
+    ut.log_return("fitted_genes_mask_of_type", fitted_genes_mask_of_type)
+    ut.log_return("similar_per_metacell_of_type", similar_per_metacell_of_type)
+    ut.log_return("misfit_per_gene_per_metacell_of_type", misfit_per_gene_per_metacell_of_type)
+    ut.log_return("projected_correlation_per_metacell_of_type", projected_correlation_per_metacell_of_type)
+    ut.log_return("projected_fold_per_gene_per_metacell_of_type", projected_fold_per_gene_per_metacell_of_type)
+    ut.log_return("weights", type_weights)
+
+    return {
+        "query_metacell_indices_of_type": np.where(query_metacell_mask_of_type)[0],
+        "fitted_genes_indices_of_type": np.where(fitted_genes_mask_of_type)[0],
+        "similar_per_metacell_of_type": similar_per_metacell_of_type,
+        "misfit_per_gene_per_metacell_of_type": misfit_per_gene_per_metacell_of_type,
+        "projected_correlation_per_metacell_of_type": projected_correlation_per_metacell_of_type,
+        "projected_fold_per_gene_per_metacell_of_type": projected_fold_per_gene_per_metacell_of_type,
+        "weights_per_atlas_per_query_metacell_of_type": type_weights,
+    }
 
-    return (
-        similar,
-        dissimilar_genes_count,
-        weights,
-        projected_folds,
-        systematic_gene_of_type,
-        biased_gene_of_type,
-        ignored_gene_of_type,
-    )
 
-
-def _convey_query_type_to_common_data(
+def _detect_type_misfit_genes(
     *,
-    type_weights: ut.CompressedMatrix,
-    weights: ut.NumpyMatrix,
-    projected_folds: ut.NumpyMatrix,
-    type_included_qdata: AnnData,
-    similar: ut.NumpyVector,
-    dissimilar_genes_count: ut.NumpyVector,
-    ignored_gene_of_type: ut.NumpyVector,
-) -> None:
-    common_gene_index_of_type_included_qdata = ut.get_v_numpy(type_included_qdata, "common_gene_index_of_qdata")
-    ignored_gene_of_type[common_gene_index_of_type_included_qdata] = False
-
-    full_cell_index_of_type_qdata = ut.get_o_numpy(type_included_qdata, "full_metacell_index_of_qdata")
-    similar[full_cell_index_of_type_qdata] = ut.get_o_numpy(type_included_qdata, "similar")
-    ignored_gene_of_type[:] = True
-    common_gene_index_of_type_qdata = ut.get_v_numpy(type_included_qdata, "common_gene_index_of_qdata")
-    ignored_gene_of_type[common_gene_index_of_type_qdata] = False
-    dissimilar_genes_count[full_cell_index_of_type_qdata] = ut.get_o_numpy(
-        type_included_qdata, "dissimilar_genes_count", formatter=ut.mask_description
-    )
-
-    weights[full_cell_index_of_type_qdata, :] = ut.to_numpy_matrix(type_weights)
-    type_projected_fold = ut.to_numpy_matrix(ut.get_vo_proper(type_included_qdata, "projected_fold"))
-    projected_folds[
-        full_cell_index_of_type_qdata[:, None], common_gene_index_of_type_included_qdata[None, :]
-    ] = type_projected_fold
-
-
-@ut.logged()
-@ut.timed_call()
-def _common_type_data(
-    *,
-    type_name: str,
-    common_adata: AnnData,
-    common_qdata: AnnData,
-    atlas_total_common_umis: ut.NumpyVector,
-    query_total_common_umis: ut.NumpyVector,
-    atlas_type_property_name: str,
-) -> Tuple[AnnData, AnnData, ut.NumpyVector, ut.NumpyVector]:
-    type_of_atlas_metacells = ut.get_o_numpy(common_adata, atlas_type_property_name)
-    type_of_query_metacells = ut.get_o_numpy(common_qdata, "projected_type")
-
-    atlas_type_mask = type_of_atlas_metacells == type_name
-    query_type_mask = type_of_query_metacells == type_name
-
-    ut.log_calc("atlas cells mask", atlas_type_mask)
-    ut.log_calc("query cells mask", query_type_mask)
-
-    type_common_adata = ut.slice(common_adata, obs=atlas_type_mask, name=f".{type_name}")
-    type_common_qdata = ut.slice(
-        common_qdata, obs=query_type_mask, name=f".{type_name}", track_var="full_metacell_index_of_qdata"
-    )
-
-    atlas_type_total_common_umis = atlas_total_common_umis[atlas_type_mask]
-    query_type_total_common_umis = query_total_common_umis[query_type_mask]
-
-    return type_common_adata, type_common_qdata, atlas_type_total_common_umis, query_type_total_common_umis
-
-
-@ut.logged()
-@ut.timed_call()
-def _initial_type_ignored_mask_names(
-    *,
-    what: str,
-    type_name: str,
-    type_common_adata: AnnData,
     type_common_qdata: AnnData,
-    atlas_type_total_common_umis: ut.NumpyVector,
-    query_type_total_common_umis: ut.NumpyVector,
-    systematic_low_gene_quantile: float,
-    systematic_high_gene_quantile: float,
-    systematic_gene_of_type: ut.NumpyVector,
-) -> List[str]:
-    type_ignored_mask_names = ["|ignored_gene", f"|manually_ignored_gene_of_{type_name}?"]
-
-    tl.find_systematic_genes(
-        what,
-        adata=type_common_adata,
-        qdata=type_common_qdata,
-        atlas_total_umis=atlas_type_total_common_umis,
-        query_total_umis=query_type_total_common_umis,
-        low_gene_quantile=systematic_low_gene_quantile,
-        high_gene_quantile=systematic_high_gene_quantile,
-        to_property_name=f"systematic_gene_of_{type_name}",
-    )
-    type_ignored_mask_names.append(f"|systematic_gene_of_{type_name}")
-
-    systematic_gene_of_type[:] = ut.get_v_numpy(type_common_qdata, f"systematic_gene_of_{type_name}")
-
-    return type_ignored_mask_names
-
-
-@ut.logged()
-@ut.timed_call()
-def _compute_type_projection(
-    *,
-    what: str,
-    type_name: str,
-    type_included_adata: AnnData,
-    type_included_qdata: AnnData,
-    atlas_total_common_umis: ut.NumpyVector,
-    query_type_total_common_umis: ut.NumpyVector,
-    type_ignored_mask_names: List[str],
-    project_fold_normalization: float,
-    project_min_significant_gene_value: float,
-    project_max_consistency_fold_factor: float,
-    project_candidates_count: int,
-    project_min_usage_weight: float,
-    project_max_projection_fold_factor: float,
-    min_entry_project_fold_factor: float,
-    project_abs_folds: bool,
-    reproducible: bool,
-) -> Tuple[AnnData, AnnData, ut.CompressedMatrix]:
-    tl.combine_masks(type_included_qdata, type_ignored_mask_names, to=f"ignored_gene_of_{type_name}")
-    type_included_genes_mask = ~ut.get_v_numpy(type_included_qdata, f"ignored_gene_of_{type_name}")
-    type_included_adata = ut.slice(type_included_adata, name=".included", vars=type_included_genes_mask)
-    type_included_qdata = ut.slice(type_included_qdata, name=".included", vars=type_included_genes_mask)
-
-    type_weights = tl.project_query_onto_atlas(
-        what,
-        adata=type_included_adata,
-        qdata=type_included_qdata,
-        atlas_total_umis=atlas_total_common_umis,
-        query_total_umis=query_type_total_common_umis,
-        fold_normalization=project_fold_normalization,
-        min_significant_gene_value=project_min_significant_gene_value,
-        max_consistency_fold_factor=project_max_consistency_fold_factor,
-        candidates_count=project_candidates_count,
-        min_usage_weight=project_min_usage_weight,
-        reproducible=reproducible,
+    projected_fold_per_gene_per_metacell_of_type: ut.ProperMatrix,
+    max_projection_fold_factor: float,
+    max_projection_noisy_fold_factor: float,
+    misfit_min_metacells_fraction: float,
+    fitted_genes_mask_of_type: ut.NumpyVector,
+) -> bool:
+    assert max_projection_fold_factor >= 0
+    assert max_projection_noisy_fold_factor >= 0
+    assert 0 <= misfit_min_metacells_fraction <= 1
+
+    if ut.has_data(type_common_qdata, "projected_noisy_gene"):
+        max_projection_fold_factor_per_gene = np.full(
+            type_common_qdata.n_vars, max_projection_fold_factor, dtype="float32"
+        )
+        noisy_per_gene = ut.get_v_numpy(type_common_qdata, "projected_noisy_gene")
+        max_projection_fold_factor_per_gene[noisy_per_gene] += max_projection_noisy_fold_factor
+        high_projection_fold_per_gene_per_metacell_of_type = (
+            projected_fold_per_gene_per_metacell_of_type > max_projection_fold_factor_per_gene[np.newaxis, :]
+        )
+    else:
+        high_projection_fold_per_gene_per_metacell_of_type = (
+            ut.to_numpy_matrix(projected_fold_per_gene_per_metacell_of_type) > max_projection_fold_factor
+        )
+    ut.log_calc(
+        "high_projection_fold_per_gene_per_metacell_of_type", high_projection_fold_per_gene_per_metacell_of_type
     )
 
-    tl.compute_query_projection(
-        adata=type_included_adata,
-        qdata=type_included_qdata,
-        weights=type_weights,
-        atlas_total_umis=atlas_total_common_umis,
-        query_total_umis=query_type_total_common_umis,
+    high_projection_metacells_per_gene = ut.sum_per(
+        ut.to_layout(high_projection_fold_per_gene_per_metacell_of_type, layout="column_major"), per="column"
     )
-
-    tl.compute_significant_projected_fold_factors(
-        type_included_qdata,
-        what,
-        total_umis=query_type_total_common_umis,
-        fold_normalization=project_fold_normalization,
-        min_gene_fold_factor=project_max_projection_fold_factor,
-        min_entry_fold_factor=min_entry_project_fold_factor,
-        min_significant_gene_value=project_min_significant_gene_value,
-        abs_folds=project_abs_folds,
+    ut.log_calc(
+        "high_projection_metacells_per_gene", high_projection_metacells_per_gene, formatter=ut.sizes_description
     )
 
-    return type_included_adata, type_included_qdata, type_weights
+    min_high_projection_metacells = type_common_qdata.n_obs * misfit_min_metacells_fraction
+    ut.log_calc("min_high_projection_metacells", min_high_projection_metacells)
 
-
-def _detect_type_biased_genes(
-    *,
-    type_name: str,
-    type_included_qdata: AnnData,
-    project_max_projection_fold_factor: float,
-    biased_min_metacells_fraction: float,
-    project_abs_folds: bool,
-    biased_gene_of_type: ut.NumpyVector,
-) -> bool:
-    tl.find_biased_genes(
-        type_included_qdata,
-        max_projection_fold_factor=project_max_projection_fold_factor,
-        min_metacells_fraction=biased_min_metacells_fraction,
-        abs_folds=project_abs_folds,
-        to_property_name=f"biased_gene_of_{type_name}",
-    )
-
-    new_type_biased_genes_mask = ut.get_v_numpy(type_included_qdata, f"biased_gene_of_{type_name}")
-    if not np.any(new_type_biased_genes_mask):
+    high_projection_genes_mask = high_projection_metacells_per_gene >= min_high_projection_metacells
+    type_misfit_genes_mask = fitted_genes_mask_of_type & high_projection_genes_mask
+    ut.log_calc("type_misfit_genes_mask", type_misfit_genes_mask)
+    if not np.any(type_misfit_genes_mask):
         return False
 
-    common_gene_index_of_type_included_qdata = ut.get_v_numpy(type_included_qdata, "common_gene_index_of_qdata")
-    biased_gene_of_type[common_gene_index_of_type_included_qdata] = new_type_biased_genes_mask
+    fitted_genes_mask_of_type[type_misfit_genes_mask] = False
+    ut.log_calc("fitted_genes_mask_of_type", fitted_genes_mask_of_type)
+
     return True
 
 
 @ut.logged()
 @ut.timed_call()
 def _changed_projected_types(
     *,
     common_adata: AnnData,
     common_qdata: AnnData,
-    weights: ut.NumpyMatrix,
+    old_type_of_query_metacells: ut.NumpyVector,
+    weights_per_atlas_per_query_metacell: ut.NumpyMatrix,
     atlas_type_property_name: str,
-    taboo_types: List[Set[str]],
+    old_types_per_metacell: List[Set[str]],
 ) -> bool:
-    old_type_of_query_metacells = ut.get_o_numpy(common_qdata, "projected_type").copy()
-    for metacell_index, old_type in enumerate(old_type_of_query_metacells):
-        taboo_types[metacell_index].add(old_type)
-
-    tl.project_atlas_to_query(
+    tl.convey_atlas_to_query(
         adata=common_adata,
         qdata=common_qdata,
-        weights=weights,
+        weights=weights_per_atlas_per_query_metacell,
         property_name=atlas_type_property_name,
         to_property_name="projected_type",
     )
-
     new_type_of_query_metacells = ut.get_o_numpy(common_qdata, "projected_type")
+
     has_changed = False
-    for metacell_index, new_type in enumerate(new_type_of_query_metacells):
-        if new_type not in taboo_types[metacell_index]:
-            old_type = old_type_of_query_metacells[metacell_index]
-            ut.log_calc(f"metacell: {metacell_index} changed from: {old_type} to", new_type)
-            taboo_types[metacell_index].add(new_type)
+    for metacell_index, old_types_of_metacell in enumerate(old_types_per_metacell):
+        old_type = old_type_of_query_metacells[metacell_index]
+        old_types_of_metacell.add(old_type)
+
+        new_type = new_type_of_query_metacells[metacell_index]
+        if new_type not in old_types_of_metacell:
+            ut.log_calc(f"metacell: {metacell_index} changed from old type: {old_type} to new type", new_type)
             has_changed = True
+        elif new_type != old_type:
+            ut.log_calc(f"metacell: {metacell_index} changed from old type: {old_type} to older type", new_type)
 
     ut.log_return("has_changed", has_changed)
     return has_changed
 
 
-def _correct_correlated_genes(
-    *,
-    what: str,
-    common_qdata: AnnData,
-    project_max_uncorrelated_gene_correlation: float,
-    project_min_corrected_gene_correlation: float,
-    project_min_corrected_gene_factor: float,
-    reproducible: bool,
-) -> bool:
-    projected_gene_columns = ut.to_numpy_matrix(ut.get_vo_proper(common_qdata, "projected", layout="column_major"))
-    projected_gene_rows = projected_gene_columns.transpose()
-
-    observed_gene_columns = ut.to_numpy_matrix(ut.get_vo_proper(common_qdata, what, layout="column_major"))
-    observed_gene_rows = observed_gene_columns.transpose()
-
-    common_gene_correlations = ut.pairs_corrcoef_rows(
-        projected_gene_rows, observed_gene_rows, reproducible=reproducible
-    )
-    assert len(common_gene_correlations) == common_qdata.n_vars
-    ut.set_v_data(common_qdata, "projected_correlation", common_gene_correlations)
-
-    prev_common_uncorrelated_genes_mask = ut.get_v_numpy(common_qdata, "uncorrelated_gene")
-
-    did_correct = False
-
-    new_common_uncorrelated_genes_mask = common_gene_correlations <= project_max_uncorrelated_gene_correlation
-    add_common_uncorrelated_genes_mask = new_common_uncorrelated_genes_mask & ~prev_common_uncorrelated_genes_mask
-    ut.log_calc("add_common_uncorrelated_genes_mask", add_common_uncorrelated_genes_mask)
-    if np.any(add_common_uncorrelated_genes_mask):
-        new_common_uncorrelated_genes_mask |= prev_common_uncorrelated_genes_mask
-        ut.set_v_data(common_qdata, "uncorrelated_gene", new_common_uncorrelated_genes_mask)
-        did_correct = True
-
-    correlated_common_genes_mask = common_gene_correlations >= project_min_corrected_gene_correlation
-    ut.set_v_data(common_qdata, "correlated_gene", correlated_common_genes_mask)
-
-    if np.any(correlated_common_genes_mask):
-        correlated_common_gene_indices = np.where(correlated_common_genes_mask)[0]
-        projected_correlated_gene_rows = projected_gene_rows[correlated_common_gene_indices, :]
-        observed_correlated_gene_rows = observed_gene_rows[correlated_common_gene_indices, :]
-        projected_correlated_genes_totals = ut.sum_per(projected_correlated_gene_rows, per="row")
-        observed_correlated_genes_totals = ut.sum_per(observed_correlated_gene_rows, per="row")
-        correlated_common_genes_correction_factors = (
-            projected_correlated_genes_totals / observed_correlated_genes_totals
-        )
-
-        corrected_genes_mask = (
-            correlated_common_genes_correction_factors < (1.0 / (1 + project_min_corrected_gene_factor))
-        ) | (correlated_common_genes_correction_factors > (1 + project_min_corrected_gene_factor))
-
-        if ut.has_data(common_qdata, "atlas_significant_gene"):
-            atlas_significant_mask = ut.get_v_numpy(common_qdata, "atlas_significant_gene")
-            corrected_genes_mask &= atlas_significant_mask[correlated_common_gene_indices]
-
-        ut.log_calc("corrected_genes_mask", corrected_genes_mask)
-        if np.any(corrected_genes_mask):
-            corrected_common_gene_indices = correlated_common_gene_indices[corrected_genes_mask]
-            corrected_gene_factors = correlated_common_genes_correction_factors[corrected_genes_mask]
-            prev_common_genes_correction_factors = ut.get_v_numpy(common_qdata, "correction_factor")
-            new_common_genes_correction_factors = prev_common_genes_correction_factors.copy()
-            new_common_genes_correction_factors[corrected_common_gene_indices] *= corrected_gene_factors
-            ut.set_v_data(common_qdata, "correction_factor", new_common_genes_correction_factors)
-            corrected_data = observed_gene_columns.copy()
-            corrected_data[:, corrected_common_gene_indices] *= corrected_gene_factors[None, :]
-            ut.set_vo_data(common_qdata, what, corrected_data)
-            did_correct = True
-
-    return did_correct
-
-
-@ut.logged()
-@ut.timed_call()
-@ut.expand_doc()
-def outliers_projection_pipeline(
-    what: str = "__x__",
-    *,
-    adata: AnnData,
-    odata: AnnData,
-    fold_normalization: float = pr.outliers_fold_normalization,
-    min_gene_outliers_fold_factor: float = pr.min_gene_outliers_fold_factor,
-    min_entry_outliers_fold_factor: float = pr.min_entry_outliers_fold_factor,
-    abs_folds: bool = pr.outliers_abs_folds,
-    reproducible: bool,
-) -> None:
-    """
-    Project outliers on an atlas.
-
-    **Returns**
-
-    Sets the following in ``odata``:
-
-    Per-Observation (Cell) Annotations
-
-        ``atlas_most_similar``
-            For each observation (outlier), the index of the "most similar" atlas metacell.
-
-    Per-Variable Per-Observation (Gene-Cell) Annotations
-
-        ``atlas_most_similar_fold``
-            The fold factor between the outlier gene expression and their expression in the most similar atlas metacell
-            (unless the value is too low to be of interest, in which case it will be zero).
-
-    **Computation Parameters**
-
-    1. Invoke :py:func:`metacells.tools.quality.compute_outliers_matches` using the ``fold_normalization``
-       (default: {fold_normalization}) and ``reproducible``.
-
-    2. Invoke :py:func:`metacells.tools.quality.compute_outliers_fold_factors` using the ``fold_normalization``
-       (default: {fold_normalization}), ``min_gene_outliers_fold_factor`` (default: {min_gene_outliers_fold_factor}),
-       ``min_entry_outliers_fold_factor`` (default: {min_entry_outliers_fold_factor}) and ``abs_folds`` (default:
-       {abs_folds}).
-    """
-    if list(odata.var_names) != list(adata.var_names):
-        atlas_genes_list = list(adata.var_names)
-        query_genes_list = list(odata.var_names)
-        common_genes_list = list(sorted(set(atlas_genes_list) & set(query_genes_list)))
-        atlas_gene_indices = np.array([atlas_genes_list.index(gene) for gene in common_genes_list])
-        query_gene_indices = np.array([query_genes_list.index(gene) for gene in common_genes_list])
-        common_adata = ut.slice(adata, name=".common", vars=atlas_gene_indices)
-        common_odata = ut.slice(
-            odata,
-            name=".common",
-            vars=query_gene_indices,
-            track_var="full_gene_index_of_odata",
-        )
-    else:
-        common_adata = adata
-        common_odata = odata
-
-    tl.compute_outliers_matches(
-        what,
-        adata=common_odata,
-        gdata=common_adata,
-        most_similar="atlas_most_similar",
-        value_normalization=fold_normalization,
-        reproducible=reproducible,
-    )
-
-    tl.compute_outliers_fold_factors(
-        what,
-        adata=common_odata,
-        gdata=common_adata,
-        most_similar="atlas_most_similar",
-        fold_normalization=fold_normalization,
-        min_gene_outliers_fold_factor=min_gene_outliers_fold_factor,
-        min_entry_outliers_fold_factor=min_entry_outliers_fold_factor,
-        abs_folds=abs_folds,
-    )
-
-    if list(odata.var_names) != list(adata.var_names):
-        atlas_most_similar = ut.get_o_numpy(common_odata, "atlas_most_similar")
-        ut.set_o_data(odata, "atlas_most_similar", atlas_most_similar)
-
-        common_gene_indices = ut.get_v_numpy(common_odata, "full_gene_index_of_odata")
-        common_folds = ut.get_vo_proper(common_odata, "atlas_most_similar_fold")
-        atlas_most_similar_fold = sp.csr_matrix(odata.shape, dtype="float32")
-        atlas_most_similar_fold[:, common_gene_indices] = common_folds
-        ut.set_vo_data(odata, "atlas_most_similar_fold", atlas_most_similar_fold)
-
-
 @ut.timed_call()
 @ut.logged()
 def _compute_dissimilar_residuals_projection(
     *,
-    what: str,
     common_adata: AnnData,
     common_qdata: AnnData,
-    weights: ut.NumpyMatrix,
-    atlas_total_common_umis: ut.NumpyVector,
-    query_total_common_umis: ut.NumpyVector,
-    project_fold_normalization: float,
+    weights_per_atlas_per_query_metacell: ut.NumpyMatrix,
+    project_log_data: bool,
+    project_fold_regularization: float,
     project_candidates_count: int,
-    project_min_significant_gene_value: float,
+    project_min_candidates_fraction: float,
+    project_min_significant_gene_umis: float,
     project_min_usage_weight: float,
     project_max_consistency_fold_factor: float,
     project_max_projection_fold_factor: float,
-    project_max_dissimilar_genes: int,
-    min_entry_project_fold_factor: float,
-    project_abs_folds: bool,
+    project_max_projection_noisy_fold_factor: float,
+    project_max_misfit_genes: int,
+    min_fitted_query_marker_genes: float,
+    min_essential_genes_of_type: Dict[Tuple[str, str], Optional[int]],
     atlas_type_property_name: str,
     top_level_parallel: bool,
     reproducible: bool,
-) -> ut.NumpyMatrix:
+) -> None:
     secondary_type = [""] * common_qdata.n_obs
-    dissimilar_mask = ~ut.get_o_numpy(common_qdata, "similar")
-    if not np.any(dissimilar_mask):
+    dissimilar_metacells_mask = ~ut.get_o_numpy(common_qdata, "similar")
+    if not np.any(dissimilar_metacells_mask):
         ut.set_o_data(common_qdata, "projected_secondary_type", np.array(secondary_type))
-        return weights
-
-    dissimilar_qdata = ut.slice(common_qdata, obs=dissimilar_mask, name=".dissimilar")
-    dissimilar_total_common_umis = query_total_common_umis[dissimilar_mask]
+        return
+    dissimilar_metacell_indices = np.where(dissimilar_metacells_mask)[0]
 
     @ut.timed_call("single_metacell_residuals")
     def _single_metacell_residuals(
-        dissimilar_metacell_index: int,
-    ) -> Tuple[ut.NumpyVector, ut.NumpyVector, ut.NumpyVector, str, str, bool]:
+        dissimilar_metacell_position: int,
+    ) -> Optional[Dict[str, Any]]:
         return _compute_single_metacell_residuals(
-            dissimilar_metacell_index=dissimilar_metacell_index,
-            what=what,
+            dissimilar_metacell_index=dissimilar_metacell_indices[dissimilar_metacell_position],
             common_adata=common_adata,
-            dissimilar_qdata=dissimilar_qdata,
-            atlas_total_common_umis=atlas_total_common_umis,
-            dissimilar_total_common_umis=dissimilar_total_common_umis,
-            project_fold_normalization=project_fold_normalization,
+            common_qdata=common_qdata,
+            project_log_data=project_log_data,
+            project_fold_regularization=project_fold_regularization,
             project_candidates_count=project_candidates_count,
-            project_min_significant_gene_value=project_min_significant_gene_value,
+            project_min_candidates_fraction=project_min_candidates_fraction,
+            project_min_significant_gene_umis=project_min_significant_gene_umis,
             project_min_usage_weight=project_min_usage_weight,
             project_max_consistency_fold_factor=project_max_consistency_fold_factor,
             project_max_projection_fold_factor=project_max_projection_fold_factor,
-            project_max_dissimilar_genes=project_max_dissimilar_genes,
-            min_entry_project_fold_factor=min_entry_project_fold_factor,
-            project_abs_folds=project_abs_folds,
+            project_max_projection_noisy_fold_factor=project_max_projection_noisy_fold_factor,
+            project_max_misfit_genes=project_max_misfit_genes,
+            min_fitted_query_marker_genes=min_fitted_query_marker_genes,
+            min_essential_genes_of_type=min_essential_genes_of_type,
             atlas_type_property_name=atlas_type_property_name,
             reproducible=reproducible,
         )
 
     if top_level_parallel:
-        results = ut.parallel_map(_single_metacell_residuals, dissimilar_qdata.n_obs)
+        results = ut.parallel_map(_single_metacell_residuals, len(dissimilar_metacell_indices))
     else:
-        results = []
-        for dissimilar_metacell_index in range(dissimilar_qdata.n_obs):
-            results.append(_single_metacell_residuals(dissimilar_metacell_index))
-
-    primary_type = ut.get_o_numpy(common_qdata, "projected_type").copy()
-    projected_folds = ut.to_numpy_matrix(ut.get_vo_proper(common_qdata, "projected_fold"), copy=True)
-    similar = ut.get_o_numpy(common_qdata, "similar").copy()
-
-    for (
-        dissimilar_metacell_index,
-        (
-            metacell_weights,
-            metacell_gene_indices,
-            metacell_projected_folds,
-            metacell_primary_type,
-            metacell_secondary_type,
-            metacell_similar,
-        ),
-    ) in enumerate(results):
-        metacell_index = ut.get_o_numpy(dissimilar_qdata, "full_metacell_index_of_qdata")[dissimilar_metacell_index]
-        ut.log_calc("metacell_index", metacell_index)
-        weights[metacell_index, :] = metacell_weights
-        projected_folds[metacell_index, :] = 0.0
-        projected_folds[metacell_index, metacell_gene_indices] = metacell_projected_folds
-        primary_type[metacell_index] = metacell_primary_type
-        secondary_type[metacell_index] = metacell_secondary_type
-        similar[metacell_index] = metacell_similar
-
-    ut.set_vo_data(common_qdata, "projected_fold", sp.csr_matrix(projected_folds))
-    ut.set_o_data(common_qdata, "projected_type", primary_type)
-    ut.set_o_data(common_qdata, "projected_secondary_type", np.array(secondary_type))
-    ut.set_o_data(common_qdata, "similar", similar)
+        results = [
+            _single_metacell_residuals(dissimilar_metacell_position)
+            for dissimilar_metacell_position in range(len(dissimilar_metacell_indices))
+        ]
 
-    tl.compute_query_projection(
-        adata=common_adata,
-        qdata=common_qdata,
-        weights=weights,
-        atlas_total_umis=atlas_total_common_umis,
-        query_total_umis=query_total_common_umis,
+    similar_per_metacell = ut.get_o_numpy(common_qdata, "similar").copy()
+    primary_type_per_metacell = ut.get_o_numpy(common_qdata, "projected_type").copy()
+    secondary_type_per_metacell = [""] * common_qdata.n_obs
+    fitted_per_gene_per_metacell = ut.to_numpy_matrix(ut.get_vo_proper(common_qdata, "fitted"), copy=True)
+    misfit_per_gene_per_metacell = ut.to_numpy_matrix(ut.get_vo_proper(common_qdata, "misfit"), copy=True)
+    projected_correlation_per_metacell = ut.get_o_numpy(common_qdata, "projected_correlation").copy()
+    projected_fold_per_gene_per_metacell = ut.to_numpy_matrix(
+        ut.get_vo_proper(common_qdata, "projected_fold"), copy=True
     )
 
-    return weights
+    def _collect_metacell_residuals(
+        dissimilar_metacell_index: int,
+        primary_type: str,
+        secondary_type: str,
+        fitted_genes_mask: ut.NumpyVector,
+        misfit_genes_mask: ut.NumpyVector,
+        projected_correlation: float,
+        projected_fold_per_gene: ut.NumpyVector,
+        weights: ut.ProperMatrix,
+    ) -> None:
+        similar_per_metacell[dissimilar_metacell_index] = True
+        primary_type_per_metacell[dissimilar_metacell_index] = primary_type
+        secondary_type_per_metacell[dissimilar_metacell_index] = secondary_type
+        projected_correlation_per_metacell[dissimilar_metacell_index] = projected_correlation
+
+        fitted_per_gene_per_metacell[dissimilar_metacell_index, :] = fitted_genes_mask
+        misfit_per_gene_per_metacell[dissimilar_metacell_index, :] = misfit_genes_mask
+        projected_fold_per_gene_per_metacell[dissimilar_metacell_index, :] = projected_fold_per_gene
+        weights_per_atlas_per_query_metacell[dissimilar_metacell_index, :] = weights
+
+    for dissimilar_metacell_index, result in zip(dissimilar_metacell_indices, results):
+        if result is not None:
+            _collect_metacell_residuals(dissimilar_metacell_index, **result)
+
+    ut.set_o_data(common_qdata, "similar", similar_per_metacell)
+    ut.set_o_data(common_qdata, "projected_type", primary_type_per_metacell)
+    ut.set_o_data(common_qdata, "projected_secondary_type", np.array(secondary_type_per_metacell))
+    ut.set_o_data(common_qdata, "projected_correlation", projected_correlation_per_metacell)
+
+    ut.set_vo_data(common_qdata, "fitted", fitted_per_gene_per_metacell)
+    ut.set_vo_data(common_qdata, "misfit", misfit_per_gene_per_metacell)
+    ut.set_vo_data(common_qdata, "projected_fold", projected_fold_per_gene_per_metacell)
 
 
 @ut.timed_call()
 @ut.logged()
-def _compute_single_metacell_residuals(
+def _compute_single_metacell_residuals(  # pylint: disable=too-many-statements
     *,
     dissimilar_metacell_index: int,
-    what: str,
     common_adata: AnnData,
-    dissimilar_qdata: AnnData,
-    atlas_total_common_umis: ut.NumpyVector,
-    dissimilar_total_common_umis: ut.NumpyVector,
-    project_fold_normalization: float,
+    common_qdata: AnnData,
+    project_log_data: bool,
+    project_fold_regularization: float,
     project_candidates_count: int,
-    project_min_significant_gene_value: float,
+    project_min_candidates_fraction: float,
+    project_min_significant_gene_umis: float,
     project_min_usage_weight: float,
     project_max_consistency_fold_factor: float,
     project_max_projection_fold_factor: float,
-    project_max_dissimilar_genes: int,
-    min_entry_project_fold_factor: float,
-    project_abs_folds: bool,
+    project_max_projection_noisy_fold_factor: float,
+    project_max_misfit_genes: int,
+    min_fitted_query_marker_genes: float,
+    min_essential_genes_of_type: Dict[Tuple[str, str], Optional[int]],
     atlas_type_property_name: str,
     reproducible: bool,
-) -> Tuple[ut.NumpyVector, ut.NumpyVector, ut.NumpyVector, str, str, bool]:
-    primary_type = ut.get_o_numpy(dissimilar_qdata, "projected_type")[dissimilar_metacell_index]
+) -> Optional[Dict[str, Any]]:
+    dissimilar_qdata = ut.slice(
+        common_qdata, name=f".dissimilar.{dissimilar_metacell_index}", obs=[dissimilar_metacell_index], top_level=False
+    )
+    corrected_fractions = ut.get_vo_proper(dissimilar_qdata, "corrected_fraction")
+
+    primary_type = ut.get_o_numpy(dissimilar_qdata, "projected_type")[0]
     secondary_type = ""
 
     repeat = 0
     while True:
         repeat += 1
-        ut.log_calc("types repeat", repeat)
+        ut.log_calc("residuals repeat", repeat)
         ut.log_calc("primary_type", primary_type)
         ut.log_calc("secondary_type", secondary_type)
 
-        ignored_genes_mask = ut.get_v_numpy(dissimilar_qdata, f"ignored_gene_of_{primary_type}")
+        fitted_genes_mask = ut.get_v_numpy(dissimilar_qdata, f"fitted_gene_of_{primary_type}")
         if secondary_type != "":
-            ignored_genes_mask = ignored_genes_mask | ut.get_v_numpy(
-                dissimilar_qdata, f"ignored_gene_of_{secondary_type}"
-            )
-
-        included_adata = ut.slice(common_adata, vars=~ignored_genes_mask, name=".included")
+            fitted_genes_mask = fitted_genes_mask | ut.get_v_numpy(dissimilar_qdata, f"fitted_gene_of_{secondary_type}")
 
-        metacell_included_qdata = ut.slice(
-            dissimilar_qdata, obs=[dissimilar_metacell_index], vars=~ignored_genes_mask, name=".single"
+        fitted_adata = ut.slice(
+            common_adata,
+            name=f".dissimilar.{dissimilar_metacell_index}.fitted",
+            vars=fitted_genes_mask,
+            top_level=False,
         )
-        metacell_total_common_umis = dissimilar_total_common_umis[
-            dissimilar_metacell_index : dissimilar_metacell_index + 1
-        ]
 
-        second_anchor_indices: List[int] = []
+        metacell_fitted_qdata = ut.slice(dissimilar_qdata, name=".fitted", vars=fitted_genes_mask, top_level=False)
 
-        weights = tl.project_query_onto_atlas(
-            what,
-            adata=included_adata,
-            qdata=metacell_included_qdata,
-            atlas_total_umis=atlas_total_common_umis,
-            query_total_umis=metacell_total_common_umis,
-            fold_normalization=project_fold_normalization,
-            min_significant_gene_value=project_min_significant_gene_value,
+        second_anchor_indices: List[int] = []
+        weights = tl.compute_projection_weights(
+            adata=fitted_adata,
+            qdata=metacell_fitted_qdata,
+            log_data=project_log_data,
+            fold_regularization=project_fold_regularization,
+            min_significant_gene_umis=project_min_significant_gene_umis,
             max_consistency_fold_factor=project_max_consistency_fold_factor,
             candidates_count=project_candidates_count,
+            min_candidates_fraction=project_min_candidates_fraction,
             min_usage_weight=project_min_usage_weight,
             reproducible=reproducible,
             second_anchor_indices=second_anchor_indices,
         )
-
-        tl.compute_query_projection(
-            adata=included_adata,
-            qdata=metacell_included_qdata,
+        tl.compute_projected_fractions(
+            adata=common_adata,
+            qdata=dissimilar_qdata,
+            log_data=project_log_data,
+            fold_regularization=project_fold_regularization,
             weights=weights,
-            atlas_total_umis=atlas_total_common_umis,
-            query_total_umis=metacell_total_common_umis,
         )
+        projected_fractions = ut.get_vo_proper(dissimilar_qdata, "projected_fraction")
 
         first_anchor_weights = weights.copy()
         first_anchor_weights[:, second_anchor_indices] = 0.0
 
-        tl.project_atlas_to_query(
-            adata=included_adata,
-            qdata=metacell_included_qdata,
-            weights=first_anchor_weights,
-            property_name=atlas_type_property_name,
-            to_property_name="projected_type",
-        )
-        new_primary_type = ut.get_o_numpy(metacell_included_qdata, "projected_type")[0]
-
         if len(second_anchor_indices) == 0:
             new_secondary_type = ""
         else:
             second_anchor_weights = weights - first_anchor_weights  # type: ignore
 
-            tl.project_atlas_to_query(
-                adata=included_adata,
-                qdata=metacell_included_qdata,
+            tl.convey_atlas_to_query(
+                adata=common_adata,
+                qdata=dissimilar_qdata,
                 weights=second_anchor_weights,
                 property_name=atlas_type_property_name,
                 to_property_name="projected_secondary_type",
             )
-            new_secondary_type = ut.get_o_numpy(metacell_included_qdata, "projected_secondary_type")[0]
+            new_secondary_type = ut.get_o_numpy(dissimilar_qdata, "projected_secondary_type")[0]
+
+        if np.sum(first_anchor_weights.data) == 0:
+            new_primary_type = new_secondary_type
+            new_secondary_type = ""
+        else:
+            tl.convey_atlas_to_query(
+                adata=common_adata,
+                qdata=dissimilar_qdata,
+                weights=first_anchor_weights,
+                property_name=atlas_type_property_name,
+                to_property_name="projected_type",
+            )
+            new_primary_type = ut.get_o_numpy(dissimilar_qdata, "projected_type")[0]
 
         if repeat > 2 or (new_primary_type == primary_type and new_secondary_type == secondary_type):
+            ut.log_calc("residuals last repeat", repeat)
             break
 
         primary_type = new_primary_type
         secondary_type = new_secondary_type
 
-    tl.compute_query_projection(
-        adata=included_adata,
-        qdata=metacell_included_qdata,
-        weights=weights,
-        atlas_total_umis=atlas_total_common_umis,
-        query_total_umis=metacell_total_common_umis,
-    )
-
-    tl.compute_significant_projected_fold_factors(
-        metacell_included_qdata,
-        what,
-        total_umis=metacell_total_common_umis,
-        fold_normalization=project_fold_normalization,
-        min_gene_fold_factor=project_max_projection_fold_factor,
-        min_entry_fold_factor=min_entry_project_fold_factor,
-        min_significant_gene_value=project_min_significant_gene_value,
-        abs_folds=project_abs_folds,
-    )
+    projected_correlation = ut.pairs_corrcoef_rows(
+        ut.to_numpy_matrix(corrected_fractions), ut.to_numpy_matrix(projected_fractions), reproducible=reproducible
+    )[0]
+
+    tl.compute_projected_folds(
+        dissimilar_qdata,
+        fold_regularization=project_fold_regularization,
+        min_significant_gene_umis=project_min_significant_gene_umis,
+    )
+    projected_fold_per_gene = ut.to_numpy_vector(ut.get_vo_proper(dissimilar_qdata, "projected_fold"))
+
+    essential_genes_properties = [f"essential_gene_of_{primary_type}"]
+    if secondary_type == "":
+        min_essential_genes = min_essential_genes_of_type[(primary_type, primary_type)]
+    else:
+        min_essential_genes = min_essential_genes_of_type[(primary_type, secondary_type)]
+        essential_genes_properties.append(f"essential_gene_of_{secondary_type}")
 
     tl.compute_similar_query_metacells(
-        metacell_included_qdata,
+        dissimilar_qdata,
         max_projection_fold_factor=project_max_projection_fold_factor,
-        max_dissimilar_genes=project_max_dissimilar_genes,
-        abs_folds=project_abs_folds,
+        max_projection_noisy_fold_factor=project_max_projection_noisy_fold_factor,
+        max_misfit_genes=project_max_misfit_genes,
+        essential_genes_property=essential_genes_properties,
+        min_essential_genes=min_essential_genes,
+        min_fitted_query_marker_genes=min_fitted_query_marker_genes,
+        fitted_genes_mask=fitted_genes_mask,
     )
 
-    weights_vector = ut.to_numpy_vector(weights)
-    gene_indices = ut.get_v_numpy(metacell_included_qdata, "common_gene_index_of_qdata")
-    projected_folds = ut.to_numpy_vector(ut.get_vo_proper(metacell_included_qdata, "projected_fold"))
-    similar = ut.get_o_numpy(metacell_included_qdata, "similar")[0]
-
-    ut.log_return("weights", weights_vector)
-    ut.log_return("gene_indices", gene_indices)
-    ut.log_return("projected_folds", projected_folds)
+    similar = ut.get_o_numpy(dissimilar_qdata, "similar")[0]
+    ut.log_return("similar", False)
+    if not similar:
+        return None
+
+    misfit_genes_mask = ut.to_numpy_vector(ut.get_vo_proper(dissimilar_qdata, "misfit")[0, :])
+
     ut.log_return("primary_type", primary_type)
     ut.log_return("secondary_type", secondary_type)
-    ut.log_return("similar", similar)
+    ut.log_return("fitted_genes_mask", fitted_genes_mask)
+    ut.log_return("misfit_genes_mask", misfit_genes_mask)
+    ut.log_return("projected_correlation", projected_correlation)
+    ut.log_return("projected_fold_per_gene", projected_fold_per_gene)
+
+    return {
+        "primary_type": primary_type,
+        "secondary_type": secondary_type,
+        "fitted_genes_mask": fitted_genes_mask,
+        "misfit_genes_mask": misfit_genes_mask,
+        "projected_correlation": projected_correlation,
+        "projected_fold_per_gene": projected_fold_per_gene,
+        "weights": ut.to_numpy_vector(weights),
+    }
+
+
+def _normalize_corrected_fractions(adata: AnnData, what: str) -> None:
+    fractions_data = ut.get_vo_proper(adata, what, layout="row_major")
+    corrected_data = ut.fraction_by(fractions_data, by="row")
+    ut.set_vo_data(adata, "corrected_fraction", corrected_data)
+
+
+@ut.logged()
+@ut.timed_call()
+@ut.expand_doc()
+def outliers_projection_pipeline(
+    what: str = "__x__",
+    *,
+    adata: AnnData,
+    odata: AnnData,
+    fold_regularization: float = pr.outliers_fold_regularization,
+    project_min_significant_gene_umis: int = pr.project_min_significant_gene_umis,
+    reproducible: bool,
+) -> None:
+    """
+    Project outliers on an atlas.
+
+    **Returns**
+
+    Sets the following in ``odata``:
+
+    Per-Observation (Cell) Annotations
+
+        ``atlas_most_similar``
+            For each observation (outlier), the index of the "most similar" atlas metacell.
+
+    Per-Variable Per-Observation (Gene-Cell) Annotations
+
+        ``atlas_most_similar_fold``
+            The fold factor between the outlier gene expression and their expression in the most similar atlas metacell
+            (unless the value is too low to be of interest, in which case it will be zero).
+
+    **Computation Parameters**
+
+    1. Invoke :py:func:`metacells.tools.quality.compute_outliers_matches` using the ``fold_regularization``
+       (default: {fold_regularization}) and ``reproducible``.
+
+    2. Invoke :py:func:`metacells.tools.quality.compute_outliers_fold_factors` using the ``fold_regularization``
+       (default: {fold_regularization}).
+    """
+    if list(odata.var_names) != list(adata.var_names):
+        atlas_genes_list = list(adata.var_names)
+        query_genes_list = list(odata.var_names)
+        common_genes_list = list(sorted(set(atlas_genes_list) & set(query_genes_list)))
+        atlas_common_gene_indices = np.array([atlas_genes_list.index(gene) for gene in common_genes_list])
+        query_common_gene_indices = np.array([query_genes_list.index(gene) for gene in common_genes_list])
+        common_adata = ut.slice(adata, name=".common", vars=atlas_common_gene_indices, top_level=False)
+        common_odata = ut.slice(
+            odata,
+            name=".common",
+            vars=query_common_gene_indices,
+            top_level=False,
+        )
+    else:
+        common_adata = adata
+        common_odata = odata
 
-    assert secondary_type is not None
-    return weights_vector, gene_indices, projected_folds, primary_type, secondary_type, similar
+    tl.compute_outliers_matches(
+        what,
+        adata=common_odata,
+        gdata=common_adata,
+        most_similar="atlas_most_similar",
+        value_regularization=fold_regularization,
+        reproducible=reproducible,
+    )
+
+    tl.compute_outliers_fold_factors(
+        what,
+        adata=common_odata,
+        gdata=common_adata,
+        most_similar="atlas_most_similar",
+        min_gene_total=project_min_significant_gene_umis,
+    )
+
+    if list(odata.var_names) != list(adata.var_names):
+        atlas_most_similar = ut.get_o_numpy(common_odata, "atlas_most_similar")
+        ut.set_o_data(odata, "atlas_most_similar", atlas_most_similar)
+
+        common_folds = ut.get_vo_proper(common_odata, "atlas_most_similar_fold")
+        atlas_most_similar_fold = np.zeros(odata.shape, dtype="float32")
+        atlas_most_similar_fold[:, query_common_gene_indices] = common_folds
+        ut.set_vo_data(odata, "atlas_most_similar_fold", sp.csr_matrix(atlas_most_similar_fold))
+
+
+def write_projection_weights(path: str, adata: AnnData, qdata: AnnData, weights: ut.CompressedMatrix) -> None:
+    """
+    Write into the ``path`` the ``weights`` computed for the projection of the query ``qdata`` on the atlas ``adata``.
+
+    Since the weights are (very) sparse, we just write them as a CSV file. This is also what ``MCView`` expect.
+    """
+    with open(path, "w", encoding="utf8") as file:
+        file.write("query,atlas,weight\n")
+        for query_index, atlas_index in zip(*weights.nonzero()):
+            weight = weights[query_index, atlas_index]
+            file.write(f"{qdata.obs_names[query_index]},{adata.obs_names[atlas_index]},{weight}\n")
```

### Comparing `metacells-0.8.0/metacells/pipeline/related_genes.py` & `metacells-0.9.0/metacells/pipeline/related_genes.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,182 +1,214 @@
 """
 Related Genes
 -------------
 """
 
-from re import Pattern
-from typing import Collection
 from typing import List
-from typing import Optional
 from typing import Tuple
 from typing import Union
 
+import fastcluster as fc  # type: ignore
 import numpy as np
 import pandas as pd  # type: ignore
-import scipy.cluster.hierarchy as sch  # type: ignore
 import scipy.sparse as sp  # type: ignore
 import scipy.spatial.distance as scd  # type: ignore
 from anndata import AnnData  # type: ignore
 
 import metacells.parameters as pr
 import metacells.tools as tl
 import metacells.utilities as ut
 
-from .feature import extract_feature_data
-
 __all__ = [
-    "relate_genes",
+    "relate_to_lateral_genes",
 ]
 
 
 @ut.logged()
 @ut.timed_call()
 @ut.expand_doc()
-def relate_genes(
+def relate_to_lateral_genes(  # pylint: disable=too-many-statements
     adata: AnnData,
     what: Union[str, ut.Matrix] = "__x__",
     *,
     max_sampled_cells: int = pr.related_max_sampled_cells,
-    downsample_min_samples: float = pr.related_downsample_min_samples,
-    downsample_min_cell_quantile: float = pr.related_downsample_min_cell_quantile,
-    downsample_max_cell_quantile: float = pr.related_downsample_max_cell_quantile,
-    min_gene_relative_variance: float = pr.related_min_gene_relative_variance,
-    min_gene_total: int = pr.related_min_gene_total,
-    min_gene_top3: int = pr.related_min_gene_top3,
-    forbidden_gene_names: Optional[Collection[str]] = None,
-    forbidden_gene_patterns: Optional[Collection[Union[str, Pattern]]] = None,
     genes_similarity_method: str = pr.related_genes_similarity_method,
     genes_cluster_method: str = pr.related_genes_cluster_method,
-    min_genes_of_modules: int = pr.related_min_genes_of_modules,
+    max_genes_of_modules: int = pr.related_max_genes_of_modules,
+    min_mean_gene_fraction: float = pr.related_min_mean_gene_fraction,
+    min_gene_correlation: float = pr.related_min_gene_correlation,
     random_seed: int = 0,
 ) -> None:
     """
-    Detect coarse relations between genes based on ``what`` (default: {what}) data.
+    Detect coarse relations between genes and lateral genes based on ``what`` (default: {what}) data.
 
-    This is a quick-and-dirty way to group genes together and shouldn't only be used as a starting
-    point for more precise forms of gene relationship analysis.
+    This is a quick-and-dirty way to look for genes highly correlated with lateral genes.
 
     **Input**
 
-    Annotated ``adata``, where the observations are cells and the variables are genes, where
-    ``what`` is a per-variable-per-observation matrix or the name of a per-variable-per-observation
-    annotation containing such a matrix.
+    Annotated ``adata``, where the observations are cells and the variables are genes, where ``what`` is a
+    per-variable-per-observation matrix or the name of a per-variable-per-observation annotation containing such a
+    matrix. The data should contain a ``lateral_gene`` mask containing some known-to-be lateral genes.
 
     **Returns**
 
     Variable-pair (Gene) Annotations
-        ``related_genes_similarity``
-            The similarity between each two related genes.
+        ``lateral_genes_similarity``
+            The similarity between each genes related to lateral genes.
 
     Variable (Gene) Annotations
-        ``related_genes_module``
-            The index of the gene module for each gene.
+        ``lateral_genes_module``
+            The index of the related to lateral gene module for each gene.
 
     **Computation Parameters**
 
     1. If we have more than ``max_sampled_cells`` (default: {max_sampled_cells}), pick this number
        of random cells from the data using the ``random_seed``.
 
-    2. Pick candidate genes using :py:func:`metacells.pipeline.feature.extract_feature_data`.
+    2. Start by marking as "related genes" all the genes listed in ``lateral_gene``.
+
+    3. Pick as candidates genes whose mean fraction in the population is at least the (very low)
+       ``min_mean_gene_fraction`` (default: {min_mean_gene_fraction}) (and that are not lateral genes).
+
+    4. Compute the correlation between the related genes and the candidate genes. Move from the candidate genes to the
+       lateral genes any genes whose correlation is at least ``min_gene_correlation`` (default: {min_gene_correlation}).
+
+    5. Repeat step 4 until no additional related genes are found.
 
-    3. Compute the similarity between the feature genes using
-       :py:func:`metacells.tools.similarity.compute_var_var_similarity` using the
-       ``genes_similarity_method`` (default: {genes_similarity_method}).
+    6. Compute the similarity between the all related genes using
+       :py:func:`metacells.tools.similarity.compute_var_var_similarity` using the ``genes_similarity_method`` (default:
+       {genes_similarity_method}).
 
-    4. Create a hierarchical clustering of the candidate genes using the ``genes_cluster_method``
+    7. Create a hierarchical clustering of the candidate genes using the ``genes_cluster_method``
        (default: {genes_cluster_method}).
 
-    5. Identify gene modules in the hierarchical clustering which contain at least
-       ``min_genes_of_modules`` genes.
+    8. Identify gene modules in the hierarchical clustering by bottom-up combining genes as long as we have at most
+       ``max_genes_of_modules`` (default: {max_genes_of_modules}). Note that this may leave modules with a smaller
+       number of genes, and modules that do not contain any lateral genes.
     """
     if max_sampled_cells < adata.n_obs:
         np.random.seed(random_seed)
         cell_indices = np.random.choice(np.arange(adata.n_obs), size=max_sampled_cells, replace=False)
         sdata = ut.slice(adata, obs=cell_indices, name=".sampled", top_level=False)
     else:
         sdata = ut.copy_adata(adata, top_level=False)
 
-    fdata = extract_feature_data(
-        sdata,
-        what,
-        top_level=False,
-        downsample_min_samples=downsample_min_samples,
-        downsample_min_cell_quantile=downsample_min_cell_quantile,
-        downsample_max_cell_quantile=downsample_max_cell_quantile,
-        min_gene_relative_variance=min_gene_relative_variance,
-        min_gene_total=min_gene_total,
-        min_gene_top3=min_gene_top3,
-        forbidden_gene_names=forbidden_gene_names,
-        forbidden_gene_patterns=forbidden_gene_patterns,
-        random_seed=random_seed,
-    )
-    assert fdata is not None
+    umis_per_cell_per_gene = ut.get_vo_proper(sdata, what)
+    fraction_per_gene_per_cell = ut.fraction_by(umis_per_cell_per_gene, by="row")
+    fraction_per_gene_per_cell = ut.to_layout(fraction_per_gene_per_cell, layout="column_major")
+
+    mean_fraction_per_gene = ut.mean_per(fraction_per_gene_per_cell, per="column")
+    candidate_genes_mask = mean_fraction_per_gene >= min_mean_gene_fraction
+    ut.log_calc("candidate_genes_mask", candidate_genes_mask)
+
+    related_genes_mask = np.zeros(sdata.n_vars, dtype="bool")
+    additional_genes_mask = ut.get_v_numpy(sdata, "lateral_gene").copy()
+
+    while np.any(additional_genes_mask):
+        related_genes_mask |= additional_genes_mask
+        ut.log_calc("related_genes_mask", related_genes_mask)
+
+        candidate_genes_mask &= ~additional_genes_mask
+        ut.log_calc("candidate_genes_mask", candidate_genes_mask)
+        if not np.any(candidate_genes_mask):
+            break
+
+        fraction_per_candidate_gene_per_cell = ut.to_numpy_matrix(fraction_per_gene_per_cell[:, candidate_genes_mask])
+        fraction_per_additional_gene_per_cell = ut.to_numpy_matrix(fraction_per_gene_per_cell[:, additional_genes_mask])
+
+        fraction_per_cell_per_candidate_gene = np.transpose(fraction_per_candidate_gene_per_cell)
+        fraction_per_cell_per_additional_gene = np.transpose(fraction_per_additional_gene_per_cell)
+
+        fraction_per_cell_per_candidate_gene = ut.to_layout(fraction_per_cell_per_candidate_gene, layout="row_major")
+        fraction_per_cell_per_additional_gene = ut.to_layout(fraction_per_cell_per_additional_gene, layout="row_major")
+
+        correlation_per_related_per_candidate = ut.cross_corrcoef_rows(
+            fraction_per_cell_per_candidate_gene,
+            fraction_per_cell_per_additional_gene,
+            reproducible=random_seed != 0,
+        )
+        max_correlation_per_candidate = ut.max_per(correlation_per_related_per_candidate, per="row")
+        assert len(max_correlation_per_candidate) == np.sum(candidate_genes_mask)
+
+        additional_genes_mask = np.zeros(sdata.n_vars, dtype="bool")
+        additional_genes_mask[candidate_genes_mask] = max_correlation_per_candidate >= min_gene_correlation
+        ut.log_calc("additional_genes_mask", additional_genes_mask)
+
+    name = (ut.get_name(sdata) or "cells") + ".related"
+    var_names = sdata.var_names[related_genes_mask]
+    sdata = AnnData(fraction_per_gene_per_cell[:, related_genes_mask])
+    sdata.var_names = var_names
+    ut.set_name(sdata, name)
 
     frame = tl.compute_var_var_similarity(
-        fdata, what, method=genes_similarity_method, reproducible=(random_seed != 0), inplace=False
+        sdata, what, method=genes_similarity_method, reproducible=(random_seed != 0), inplace=False
     )
     assert frame is not None
     similarity = ut.to_layout(ut.to_numpy_matrix(frame), layout="row_major")
+    ut.log_calc("similarity", similarity)
 
     linkage = _cluster_genes(similarity, genes_cluster_method)
-    clusters = _linkage_to_clusters(linkage, min_genes_of_modules, fdata.n_vars)
+    ut.log_calc("linkage")
+    clusters = _linkage_to_clusters(linkage, max_genes_of_modules, sdata.n_vars)
+    ut.log_calc("cluster")
 
     cluster_of_genes = pd.Series(np.full(adata.n_vars, -1, dtype="int32"), index=adata.var_names)
     for cluster_index, gene_indices in enumerate(clusters):
-        cluster_of_genes[fdata.var_names[gene_indices]] = cluster_index
+        cluster_of_genes[sdata.var_names[gene_indices]] = cluster_index
 
-    ut.set_v_data(adata, "related_genes_module", cluster_of_genes, formatter=ut.groups_description)
+    ut.set_v_data(adata, "lateral_genes_module", cluster_of_genes, formatter=ut.groups_description)
 
-    feature_gene_indices = ut.get_v_numpy(fdata, "full_gene_index")
+    related_gene_indices = np.where(related_genes_mask)[0]
     data = similarity.flatten(order="C")
-    rows = np.repeat(feature_gene_indices, len(feature_gene_indices))
-    cols = np.tile(feature_gene_indices, len(feature_gene_indices))
-    full_similarity = sp.csr_matrix((data, (rows, cols)), shape=(adata.n_vars, adata.n_vars))
+    rows = np.repeat(related_gene_indices, len(related_gene_indices))
+    columns = np.tile(related_gene_indices, len(related_gene_indices))
+    full_similarity = sp.csr_matrix((data, (rows, columns)), shape=(adata.n_vars, adata.n_vars))
 
-    ut.set_vv_data(adata, "related_genes_similarity", full_similarity)
+    ut.set_vv_data(adata, "lateral_genes_similarity", full_similarity)
 
 
 # TODO: Replicated in metacell.tools.rare
 @ut.timed_call()
 def _cluster_genes(
     similarities_between_candidate_genes: ut.NumpyMatrix,
     genes_cluster_method: str,
 ) -> List[Tuple[int, int]]:
     with ut.timed_step("scipy.pdist"):
         ut.timed_parameters(size=similarities_between_candidate_genes.shape[0])
         distances = scd.pdist(similarities_between_candidate_genes)
 
     with ut.timed_step("scipy.linkage"):
         ut.timed_parameters(size=distances.shape[0], method=genes_cluster_method)
-        linkage = sch.linkage(distances, method=genes_cluster_method)
+        linkage = fc.linkage(distances, method=genes_cluster_method)
 
     return linkage
 
 
 @ut.timed_call()
 def _linkage_to_clusters(
     linkage: List[Tuple[int, int]],
-    min_entries_of_modules: int,
+    max_entries_of_modules: int,
     entries_count: int,
 ) -> List[List[int]]:
     entries_of_cluster = {index: [index] for index in range(entries_count)}
 
     for link_index, link_data in enumerate(linkage):
         link_index += entries_count
 
         left_index = int(link_data[0])
         right_index = int(link_data[1])
 
         left_entries = entries_of_cluster.get(left_index)
         right_entries = entries_of_cluster.get(right_index)
 
-        if left_entries is None or len(left_entries) > min_entries_of_modules:
-            continue
-
-        if right_entries is None or len(right_entries) > min_entries_of_modules:
+        if (
+            left_entries is None
+            or right_entries is None
+            or len(left_entries) + len(right_entries) > max_entries_of_modules
+        ):
             continue
 
         entries_of_cluster[link_index] = sorted(left_entries + right_entries)
         del entries_of_cluster[left_index]
         del entries_of_cluster[right_index]
 
     return list(entries_of_cluster.values())
```

### Comparing `metacells-0.8.0/metacells/pipeline/umap.py` & `metacells-0.9.0/metacells/pipeline/umap.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,62 +3,68 @@
 ----
 
 It is useful to project the metacells data to a 2D scatter plot (where each point is a metacell).
 The steps provided here are expected to yield a reasonable such projection, though as always you
 might need to tweak the parameters or even the overall flow for specific data sets.
 """
 
+from re import Pattern
+from typing import Collection
+from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import igraph as ig  # type: ignore
 import numpy as np
 from anndata import AnnData  # type: ignore
 from scipy import sparse  # type: ignore
 
 import metacells.parameters as pr
 import metacells.tools as tl
 import metacells.utilities as ut
 
 __all__ = [
-    "compute_knn_by_features",
-    "compute_umap_by_features",
+    "compute_knn_by_markers",
+    "compute_umap_by_markers",
 ]
 
 
 @ut.logged()
 @ut.timed_call()
 @ut.expand_doc()
-def compute_knn_by_features(
+def compute_knn_by_markers(
     adata: AnnData,
     what: Union[str, ut.Matrix] = "__x__",
     *,
-    max_top_feature_genes: int = pr.max_top_feature_genes,
-    similarity_value_normalization: float = pr.umap_similarity_value_normalization,
+    marker_gene_names: Optional[Collection[str]] = None,
+    marker_gene_patterns: Optional[Collection[Union[str, Pattern]]] = None,
+    max_marker_genes: Optional[int] = pr.umap_max_marker_genes,
+    ignore_lateral_genes: bool = pr.umap_ignore_lateral_genes,
+    similarity_value_regularization: float = pr.umap_similarity_value_regularization,
     similarity_log_data: bool = pr.umap_similarity_log_data,
     similarity_method: str = pr.umap_similarity_method,
     logistics_location: float = pr.logistics_location,
     logistics_slope: float = pr.logistics_slope,
     k: int,
     balanced_ranks_factor: float = pr.knn_balanced_ranks_factor,
     incoming_degree_factor: float = pr.knn_incoming_degree_factor,
     outgoing_degree_factor: float = pr.knn_outgoing_degree_factor,
-    reproducible: bool = pr.reproducible,
+    reproducible: bool,
 ) -> ut.PandasFrame:
     """
-    Compute KNN graph between metacells based on feature genes.
+    Compute KNN graph between metacells based on marker genes.
 
-    If ``reproducible`` (default: {reproducible}) is ``True``, a slower (still parallel) but
-    reproducible algorithm will be used to compute pearson correlations.
+    If ``reproducible`` is ``True``, a slower (still parallel) but
+    reproducible algorithm will be used to compute Pearson correlations.
 
     **Input**
 
-    Annotated ``adata`` where each observation is a metacells and the variables are genes,
-    are genes, where ``what`` is a per-variable-per-observation matrix or the name of a
-    per-variable-per-observation annotation containing such a matrix.
+    Annotated ``adata`` where each observation is a metacells and the variables are genes, are genes, where ``what`` is
+    a per-variable-per-observation matrix or the name of a per-variable-per-observation annotation containing such a
+    matrix. Should contain a ``marker_gene`` mask unless explicitly specifying the marker genes.
 
     **Returns**
 
     Sets the following in ``adata``:
 
     Observations-Pair (Metacells) Annotations
         ``obs_outgoing_weights``
@@ -66,57 +72,80 @@
             of cells or genes, where the sum of the weights of the outgoing edges for each element
             is 1 (there is always at least one such edge).
 
     Also return a pandas data frame of the similarities between the observations (metacells).
 
     **Computation Parameters**
 
-    1. Invoke :py:func:`metacells.tools.high.find_top_feature_genes` using ``max_top_feature_genes``
-       (default: {max_top_feature_genes}) to pick the feature genes to use to compute similarities
-       between the metacells.
-
-    2. Compute the fractions of each gene in each cell, and add the
-       ``similarity_value_normalization`` (default: {similarity_value_normalization}) to
-       it.
+    1. If ``marker_gene_names`` and/or ``marker_gene_patterns`` were specified, use the matching genes.
+       Otherwise, use the ``marker_gene`` mask.
 
-    3. If ``similarity_log_data`` (default: {similarity_log_data}), invoke the
+    2. If ``ignore_lateral_genes`` (default: {ignore_lateral_genes}), then remove any genes marked as lateral
+       from the mask.
+
+    3. If ``max_marker_genes`` (default: {max_marker_genes}) is not ``None``, then pick this number
+       of marker genes with the highest variance.
+
+    4. Compute the fractions of each ``marker_gene`` in each cell, and add the
+       ``similarity_value_regularization`` (default: {similarity_value_regularization}) to it.
+
+    5. If ``similarity_log_data`` (default: {similarity_log_data}), invoke the
        :py:func:`metacells.utilities.computation.log_data` function to compute the log (base 2) of
        the data.
 
-    4. Invoke :py:func:`metacells.tools.similarity.compute_obs_obs_similarity` using
+    6. Invoke :py:func:`metacells.tools.similarity.compute_obs_obs_similarity` using
        ``similarity_method`` (default: {similarity_method}), ``logistics_location`` (default:
        {logistics_slope}) and ``logistics_slope`` (default: {logistics_slope}) and convert this
        to distances.
 
-    5. Invoke :py:func:`metacells.tools.knn_graph.compute_obs_obs_knn_graph` using the distances,
+    7. Invoke :py:func:`metacells.tools.knn_graph.compute_obs_obs_knn_graph` using the distances,
        ``k`` (no default!), ``balanced_ranks_factor`` (default: {balanced_ranks_factor}),
        ``incoming_degree_factor`` (default: {incoming_degree_factor}), ``outgoing_degree_factor``
        (default: {outgoing_degree_factor}) to compute a "skeleton" graph to overlay on top of the
        UMAP graph.
     """
-    tl.find_top_feature_genes(adata, max_genes=max_top_feature_genes)
-
-    all_data = ut.get_vo_proper(adata, what, layout="row_major")
-    all_fractions = ut.fraction_by(all_data, by="row")
+    assert max_marker_genes is None or max_marker_genes > 0
+    if marker_gene_names is None and marker_gene_patterns is None:
+        marker_genes_mask = ut.get_v_numpy(adata, "marker_gene")
+    else:
+        marker_genes_series = tl.find_named_genes(adata, names=marker_gene_names, patterns=marker_gene_patterns)
+        assert marker_genes_series is not None
+        marker_genes_mask = ut.to_numpy_vector(marker_genes_series)
+
+    if ignore_lateral_genes:
+        lateral_genes_mask = ut.get_v_numpy(adata, "lateral_gene")
+        marker_genes_mask = marker_genes_mask & ~lateral_genes_mask
+        ut.log_calc("marker_genes_mask", marker_genes_mask)
+
+    all_fractions = ut.get_vo_proper(adata, what, layout="row_major")
+
+    index_per_marker_gene = np.where(marker_genes_mask)[0]
+    fraction_per_metacell_per_marker_gene = ut.to_numpy_matrix(all_fractions[:, index_per_marker_gene])
+
+    if max_marker_genes is not None and max_marker_genes < len(index_per_marker_gene):
+        fraction_per_metacell_per_marker_gene = ut.to_layout(
+            fraction_per_metacell_per_marker_gene, layout="column_major"
+        )
+        variance_per_marker_gene = ut.variance_per(fraction_per_metacell_per_marker_gene, per="column")
+        variance_per_marker_gene *= -1
+        chosen_positions = np.argpartition(variance_per_marker_gene, max_marker_genes)[:max_marker_genes]
+        ut.log_calc("chosen_positions", chosen_positions)
+        index_per_marker_gene = index_per_marker_gene[chosen_positions]
+        fraction_per_metacell_per_marker_gene = fraction_per_metacell_per_marker_gene[:, chosen_positions]
 
-    top_feature_genes_mask = ut.get_v_numpy(adata, "top_feature_gene")
-
-    top_feature_genes_fractions = all_fractions[:, top_feature_genes_mask]
-    top_feature_genes_fractions = ut.to_layout(top_feature_genes_fractions, layout="row_major")
-    top_feature_genes_fractions = ut.to_numpy_matrix(top_feature_genes_fractions)
-
-    top_feature_genes_fractions += similarity_value_normalization
+    fraction_per_metacell_per_marker_gene = ut.to_layout(fraction_per_metacell_per_marker_gene, layout="row_major")
+    fraction_per_metacell_per_marker_gene += similarity_value_regularization
 
     if similarity_log_data:
-        top_feature_genes_fractions = ut.log_data(top_feature_genes_fractions, base=2)
+        fraction_per_metacell_per_marker_gene = ut.log_data(fraction_per_metacell_per_marker_gene, base=2)
 
-    tdata = ut.slice(adata, vars=top_feature_genes_mask)
+    tdata = ut.slice(adata, vars=index_per_marker_gene)
     similarities = tl.compute_obs_obs_similarity(
         tdata,
-        top_feature_genes_fractions,
+        fraction_per_metacell_per_marker_gene,
         method=similarity_method,
         reproducible=reproducible,
         logistics_location=logistics_location,
         logistics_slope=logistics_slope,
         inplace=False,
     )
     assert similarities is not None
@@ -132,89 +161,94 @@
 
     return similarities
 
 
 @ut.logged()
 @ut.timed_call()
 @ut.expand_doc()
-def compute_umap_by_features(
+def compute_umap_by_markers(
     adata: AnnData,
     what: Union[str, ut.Matrix] = "__x__",
     *,
-    max_top_feature_genes: int = pr.max_top_feature_genes,
-    similarity_value_normalization: float = pr.umap_similarity_value_normalization,
+    marker_gene_names: Optional[Collection[str]] = None,
+    marker_gene_patterns: Optional[Collection[Union[str, Pattern]]] = None,
+    max_marker_genes: Optional[int] = pr.umap_max_marker_genes,
+    ignore_lateral_genes: bool = pr.umap_ignore_lateral_genes,
+    similarity_value_regularization: float = pr.umap_similarity_value_regularization,
     similarity_log_data: bool = pr.umap_similarity_log_data,
     similarity_method: str = pr.umap_similarity_method,
     logistics_location: float = pr.logistics_location,
     logistics_slope: float = pr.logistics_slope,
     skeleton_k: int = pr.skeleton_k,
     balanced_ranks_factor: float = pr.knn_balanced_ranks_factor,
     incoming_degree_factor: float = pr.knn_incoming_degree_factor,
     outgoing_degree_factor: float = pr.knn_outgoing_degree_factor,
     umap_k: int = pr.umap_k,
     dimensions: int = 2,
     min_dist: float = pr.umap_min_dist,
     spread: float = pr.umap_spread,
-    random_seed: int = pr.random_seed,
+    random_seed: int,
 ) -> None:
     """
     Compute a UMAP projection of the (meta)cells.
 
     **Input**
 
-    Annotated ``adata`` where each observation is a metacells and the variables are genes,
-    are genes, where ``what`` is a per-variable-per-observation matrix or the name of a
-    per-variable-per-observation annotation containing such a matrix.
+    Annotated ``adata`` where each observation is a metacells and the variables are genes, are genes, where ``what`` is
+    a per-variable-per-observation matrix or the name of a per-variable-per-observation annotation containing such a
+    matrix. Should contain a ``marker_gene`` mask unless explicitly specifying the marker genes.
 
     **Returns**
 
     Sets the following annotations in ``adata``:
 
-    Variable (Gene) Annotations
-        ``top_feature_gene``
-            A boolean mask of the top feature genes used to compute similarities between the
-            metacells.
-
     Observation-Observation (Metacell-Metacell) Annotations
         ``umap_distances``
             A sparse symmetric matrix of the graph of distances between the metacells.
 
     Observation (Metacell) Annotations
-        ``umap_x``, ``umap_y``
+        ``x``, ``y`` (if ``dimensions`` is 2)
             The X and Y coordinates of each metacell in the UMAP projection.
 
+        ``u``, ``v``, ``w`` (if ``dimensions`` is 3)
+            The U, V, W coordinates of each metacell in the UMAP projection.
+
     **Computation Parameters**
 
-    1. Invoke :py:func:`metacells.pipeline.umap.compute_knn_by_features` using
-       ``max_top_feature_genes`` (default: {max_top_feature_genes}),
-       ``similarity_value_normalization`` (default: {similarity_value_normalization}),
-       ``similarity_log_data`` (default: {similarity_log_data}), ``similarity_method`` (default:
-       {similarity_method}), ``logistics_location`` (default: {logistics_location}),
-       ``logistics_slope`` (default: {logistics_slope}), ``skeleton_k`` (default: {skeleton_k}),
-       ``balanced_ranks_factor`` (default: {balanced_ranks_factor}), ``incoming_degree_factor``
-       (default: {incoming_degree_factor}), ``outgoing_degree_factor`` (default:
-       {outgoing_degree_factor}) to compute a "skeleton" graph to overlay on top of the UMAP graph.
+    1. Invoke :py:func:`metacells.pipeline.umap.compute_knn_by_markers` using
+       ``marker_gene_names`` (default: {marker_gene_names}), ``marker_gene_patterns`` (default: {marker_gene_patterns}),
+       ``max_marker_genes`` (default: {max_marker_genes}), ``ignore_lateral_genes`` (default: {ignore_lateral_genes}),
+       ``similarity_value_regularization`` (default: {similarity_value_regularization}), ``similarity_log_data``
+       (default: {similarity_log_data}), ``similarity_method`` (default: {similarity_method}), ``logistics_location``
+       (default: {logistics_location}), ``logistics_slope`` (default: {logistics_slope}), ``skeleton_k`` (default:
+       {skeleton_k}), ``balanced_ranks_factor`` (default: {balanced_ranks_factor}), ``incoming_degree_factor`` (default:
+       {incoming_degree_factor}) and ``outgoing_degree_factor`` (default: {outgoing_degree_factor}) to compute a
+       "skeleton" graph to overlay on top of the UMAP graph. Specify a non-zero ``random_seed`` to make this
+       reproducible.
 
     2. Invoke :py:func:`metacells.tools.layout.umap_by_distances` using the distances, ``umap_k``
        (default: {umap_k}), ``min_dist`` (default: {min_dist}), ``spread`` (default: {spread}),
-       dimensions (default: {dimensions})
+       dimensions (default: {dimensions}) and ``random_seed``.
 
     .. note::
 
         Keep in mind that the KNN graph used by UMAP (controlled by ``umap_k``) is *not* identical to the KNN graph we
         compute (controlled by ``skeleton_k``). By default, we choose ``skeleton_k < umap_k``, as the purpose of the
         skeleton KNN is to highlight the "strong" structure of the data; in practice this strong skeleton is highly
         compatible with the structure used by UMAP, so it serves it purpose reasonably well. It would have been nice to
         make these compatible, but UMAP is not friendly towards dictating a KNN graph from the outside.
     """
-    similarities = compute_knn_by_features(
+    similarities = compute_knn_by_markers(
         adata,
         what,
-        max_top_feature_genes=max_top_feature_genes,
-        similarity_value_normalization=similarity_value_normalization,
+        marker_gene_names=marker_gene_names,
+        marker_gene_patterns=marker_gene_patterns,
+        max_marker_genes=max_marker_genes,
+        ignore_lateral_genes=ignore_lateral_genes,
+        similarity_value_regularization=similarity_value_regularization,
         similarity_log_data=similarity_log_data,
         similarity_method=similarity_method,
         logistics_location=logistics_location,
         logistics_slope=logistics_slope,
         k=skeleton_k,
         balanced_ranks_factor=balanced_ranks_factor,
         incoming_degree_factor=incoming_degree_factor,
```

### Comparing `metacells-0.8.0/metacells/prune_per.cpp` & `metacells-0.9.0/metacells/prune_per.cpp`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/metacells/rank.cpp` & `metacells-0.9.0/metacells/rank.cpp`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/metacells/relayout.cpp` & `metacells-0.9.0/metacells/relayout.cpp`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/metacells/scripts/timing.py` & `metacells-0.9.0/metacells/scripts/timing.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,17 +227,17 @@
     if output_path is None:
         output_file = sys.stdout
     else:
         output_file = open(output_path, "w", encoding="utf8")  # pylint: disable=consider-using-with
 
     for name, data in data_by_name.items():
         if seconds:
-            datum = dict(invocations=data[0], elapsed=data[1] / 1_000_000_000, cpu=data[2] / 1_000_000_000)
+            datum = {"invocations": data[0], "elapsed": data[1] / 1_000_000_000, "cpu": data[2] / 1_000_000_000}
         else:
-            datum = dict(invocations=data[0], elapsed=int(round(data[1])), cpu=int(round(data[2])))
+            datum = {"invocations": data[0], "elapsed": int(round(data[1])), "cpu": int(round(data[2]))}
         html = (
             "Elapsed Time: %.2f<br/>"  # pylint: disable=consider-using-f-string
             "CPU Time: %.2f<br/>"
             "Utilization: %.0f%%<br/>"
             "Invocations: %s<br/>"
             % (datum["elapsed"], datum["cpu"], 100 * datum["cpu"] / datum["elapsed"], datum["invocations"])
         )
```

### Comparing `metacells-0.8.0/metacells/shuffle.cpp` & `metacells-0.9.0/metacells/shuffle.cpp`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/metacells/tools/__init__.py` & `metacells-0.9.0/metacells/tools/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 static typing or analysis to ensure that the input of the next tool was actually created by previous
 tool(s).
 
 All the functions included here are exported under ``metacells.tl``.
 """
 
 from .apply import *
+from .bursty_lonely import *
 from .candidates import *
 from .convey import *
 from .deviants import *
 from .dissolve import *
 from .distinct import *
 from .downsample import *
 from .filter import *
 from .group import *
 from .high import *
 from .knn_graph import *
 from .layout import *
 from .mask import *
 from .named import *
-from .noisy_lonely import *
 from .project import *
 from .properly_sampled import *
 from .quality import *
 from .rare import *
 from .similarity import *
```

### Comparing `metacells-0.8.0/metacells/tools/apply.py` & `metacells-0.9.0/metacells/tools/apply.py`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/metacells/tools/candidates.py` & `metacells-0.9.0/metacells/tools/candidates.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,33 +27,32 @@
     "score_partitions",
 ]
 
 
 @ut.logged()
 @ut.timed_call()
 @ut.expand_doc()
-def compute_candidate_metacells(  # pylint: disable=too-many-statements,too-many-branches
+def compute_candidate_metacells(  # pylint: disable=too-many-statements
     adata: AnnData,
     what: Union[str, ut.Matrix] = "obs_outgoing_weights",
     *,
     target_metacell_size: float,
     cell_sizes: Optional[Union[str, ut.Vector]] = pr.candidates_cell_sizes,
-    cell_seeds: Optional[Union[str, ut.Vector]] = None,
     min_seed_size_quantile: float = pr.min_seed_size_quantile,
     max_seed_size_quantile: float = pr.max_seed_size_quantile,
     cooldown_pass: float = pr.cooldown_pass,
     cooldown_node: float = pr.cooldown_node,
     cooldown_phase: float = pr.cooldown_phase,
-    min_split_size_factor: Optional[float] = pr.candidates_min_split_size_factor,
-    max_merge_size_factor: Optional[float] = pr.candidates_max_merge_size_factor,
+    min_split_size_factor: float = pr.candidates_min_split_size_factor,
+    max_merge_size_factor: float = pr.candidates_max_merge_size_factor,
     min_metacell_cells: Optional[int] = pr.candidates_min_metacell_cells,
     max_split_min_cut_strength: Optional[float] = pr.max_split_min_cut_strength,
-    min_cut_seed_cells: Optional[int] = pr.min_cut_seed_cells,
+    min_cut_seed_cells: int = pr.min_cut_seed_cells,
     must_complete_cover: bool = False,
-    random_seed: int = 0,
+    random_seed: int,
     inplace: bool = True,
 ) -> Optional[ut.PandasSeries]:
     """
     Assign observations (cells) to (raw, candidate) metacells based on ``what`` data. (a weighted
     directed graph).
 
     These candidate metacells typically go through additional vetting (e.g. deviant detection and
@@ -78,19 +77,17 @@
 
     **Computation Parameters**
 
     1. We are trying to build metacells of ``target_metacell_size``, using the ``cell_sizes``
        (default: {cell_sizes}) to assign a size for each node (cell). This can be a string name of a
        per-observation annotation or a vector of values.
 
-    2. We start with some an assignment of cells to ``cell_seeds`` (default: {cell_seeds}). If no
-       seeds are provided, we use :py:func:`choose_seeds` using ``min_seed_size_quantile`` (default:
-       {min_seed_size_quantile}) and ``max_seed_size_quantile`` (default: {max_seed_size_quantile})
-       to compute them, picking a number of seeds such that the average metacell size would match
-       the target.
+    2. We start with some an assignment of cells to seeds using :py:func:`choose_seeds` using ``min_seed_size_quantile``
+       (default: {min_seed_size_quantile}) and ``max_seed_size_quantile`` (default: {max_seed_size_quantile}) to compute
+       them, picking a number of seeds such that the average metacell size would match the target.
 
     3. We optimize the seeds using :py:func:`optimize_partitions` to obtain initial communities by
        maximizing the "stability" of the solution (probability of starting at a random node and
        moving either forward or backward in the graph and staying within the same metacell, divided
        by the probability of staying in the metacell if the edges connected random nodes). We pass
        it the ``cooldown_pass`` {cooldown_pass}) and ``cooldown_node`` (default: {cooldown_node}).
 
@@ -101,28 +98,30 @@
        1 - ``cooldown_phase`` (default: {cooldown_phase}).
 
     5. If ``max_split_min_cut_strength`` (default: {max_split_min_cut_strength}) is specified, and
        the minimal cut of a candidate is lower, split it into two. If one of the partitions is
        smaller than ``min_cut_seed_cells``, then mark the cells in it as outliers, or if
        ``must_complete_cover`` is ``True``, skip the cut altogether.
 
-    5. If ``max_merge_size_factor`` (default: {max_merge_size_factor}) or ``min_metacell_cells``
+    6. If ``max_merge_size_factor`` (default: {max_merge_size_factor}) or ``min_metacell_cells``
        (default: {min_metacell_cells}) are specified, make outliers of cells of a community whose
        size is at most ``target_metacell_size * max_merge_size_factor`` or contains less cells and
        re-optimize, which will assign these cells to other metacells (resulting on one less
        metacell). We again apply the ``cooldown_phase`` every time we re-optimize.
 
-    6. Repeat the above steps until all metacells candidates are in the acceptable size range.
+    7. Repeat the above steps until all metacells candidates are in the acceptable size range.
     """
-    edge_weights = ut.get_oo_proper(adata, what, layout="row_major")
-    assert edge_weights.shape[0] == edge_weights.shape[1]
+    assert 0.0 < max_merge_size_factor < min_split_size_factor
+    assert target_metacell_size > 0
     assert 0.0 < cooldown_pass < 1.0
     assert 0.0 <= cooldown_node <= 1.0
     assert 0.0 < cooldown_phase <= 1.0
 
+    edge_weights = ut.get_oo_proper(adata, what, layout="row_major")
+    assert edge_weights.shape[0] == edge_weights.shape[1]
     size = edge_weights.shape[0]
 
     outgoing_edge_weights = ut.mustbe_compressed_matrix(edge_weights)
 
     assert ut.is_layout(outgoing_edge_weights, "row_major")
     incoming_edge_weights = ut.mustbe_compressed_matrix(ut.to_layout(outgoing_edge_weights, layout="column_major"))
     assert ut.is_layout(incoming_edge_weights, "column_major")
@@ -130,65 +129,48 @@
     assert outgoing_edge_weights.data.dtype == "float32"
     assert outgoing_edge_weights.indices.dtype == "int32"
     assert outgoing_edge_weights.indptr.dtype == "int32"
     assert incoming_edge_weights.data.dtype == "float32"
     assert incoming_edge_weights.indices.dtype == "int32"
     assert incoming_edge_weights.indptr.dtype == "int32"
 
-    node_sizes = ut.maybe_o_numpy(adata, cell_sizes, formatter=ut.sizes_description)
-    if node_sizes is None:
+    if cell_sizes is None:
         node_sizes = np.full(size, 1.0, dtype="float32")
     else:
-        node_sizes = node_sizes.astype("float32")
+        cell_sizes = ut.get_o_numpy(adata, cell_sizes, formatter=ut.sizes_description)
+        node_sizes = cell_sizes.astype("float32")
     ut.log_calc("node_sizes", node_sizes, formatter=ut.sizes_description)
 
-    assert target_metacell_size > 0
-    max_metacell_size = None
-    min_metacell_size = None
+    min_metacell_size = floor(target_metacell_size * max_merge_size_factor) + 1
+    ut.log_calc("min_metacell_size", min_metacell_size)
 
-    if min_split_size_factor is not None:
-        assert min_split_size_factor > 0
-        max_metacell_size = ceil(target_metacell_size * min_split_size_factor) - 1
+    max_metacell_size = ceil(target_metacell_size * min_split_size_factor) - 1
     ut.log_calc("max_metacell_size", max_metacell_size)
-
-    if max_merge_size_factor is not None:
-        assert max_merge_size_factor > 0
-        min_metacell_size = floor(target_metacell_size * max_merge_size_factor) + 1
-    ut.log_calc("min_metacell_size", min_metacell_size)
+    if max_metacell_size == min_metacell_size:
+        max_metacell_size += 1
 
     target_metacell_cells = max(
         1.0 if min_metacell_cells is None else float(min_metacell_cells),
         float(target_metacell_size / np.mean(node_sizes)),
     )
     ut.log_calc("target_metacell_cells", target_metacell_cells)
 
-    if min_split_size_factor is not None and max_merge_size_factor is not None:
-        assert max_merge_size_factor < min_split_size_factor
-        assert min_metacell_size is not None
-        assert max_metacell_size is not None
-        assert min_metacell_size <= max_metacell_size
-
-    community_of_nodes = ut.maybe_o_numpy(adata, cell_seeds, formatter=ut.groups_description)
-
-    if community_of_nodes is not None:
-        assert community_of_nodes.dtype == "int32"
-    else:
-        target_seeds_count = ceil(size / target_metacell_cells)
-        ut.log_calc("target_seeds_count", target_seeds_count)
+    initial_seeds_count = ceil(size / target_metacell_cells)
+    ut.log_calc("initial_seeds_count", initial_seeds_count)
 
-        community_of_nodes = np.full(size, -1, dtype="int32")
-        _choose_seeds(
-            outgoing_edge_weights=outgoing_edge_weights,
-            incoming_edge_weights=incoming_edge_weights,
-            seed_of_cells=community_of_nodes,
-            max_seeds_count=target_seeds_count,
-            min_seed_size_quantile=min_seed_size_quantile,
-            max_seed_size_quantile=max_seed_size_quantile,
-            random_seed=random_seed,
-        )
+    community_of_nodes = np.full(size, -1, dtype="int32")
+    _choose_seeds(
+        outgoing_edge_weights=outgoing_edge_weights,
+        incoming_edge_weights=incoming_edge_weights,
+        seed_of_cells=community_of_nodes,
+        max_seeds_count=initial_seeds_count,
+        min_seed_size_quantile=min_seed_size_quantile,
+        max_seed_size_quantile=max_seed_size_quantile,
+        random_seed=random_seed,
+    )
 
     ut.set_o_data(adata, "seed", community_of_nodes, formatter=ut.groups_description)
     community_of_nodes = community_of_nodes.copy()
 
     np.random.seed(random_seed)
 
     cold_temperature = 1 - cooldown_pass
@@ -196,20 +178,22 @@
     old_score = 1e9
     old_communities = community_of_nodes
     old_small_nodes_count = len(community_of_nodes)
     atomic_candidates: Set[Tuple[int, ...]] = set()
     kept_communities_count = 0
 
     while True:
-        cold_temperature, score = _optimize_split_communities(  #
+        cold_temperature, score = _reduce_communities(
             outgoing_edge_weights=outgoing_edge_weights,
             incoming_edge_weights=incoming_edge_weights,
             community_of_nodes=community_of_nodes,
             node_sizes=node_sizes,
             target_metacell_size=target_metacell_size,
+            min_metacell_cells=min_metacell_cells,
+            min_metacell_size=min_metacell_size,
             max_metacell_size=max_metacell_size,
             max_split_min_cut_strength=max_split_min_cut_strength,
             min_cut_seed_cells=min_cut_seed_cells,
             must_complete_cover=must_complete_cover,
             min_seed_size_quantile=min_seed_size_quantile,
             max_seed_size_quantile=max_seed_size_quantile,
             random_seed=random_seed,
@@ -224,14 +208,16 @@
         small_communities, small_nodes_count = _find_small_communities(
             community_of_nodes=community_of_nodes,
             node_sizes=node_sizes,
             min_metacell_size=min_metacell_size,
             min_metacell_cells=min_metacell_cells,
         )
 
+        ut.log_calc("small communities", len(small_communities))
+
         small_communities_count = len(small_communities)
         if small_communities_count < 2:
             break
 
         if (old_small_nodes_count, old_score) <= (small_nodes_count, score):
             ut.logger().debug("is not better, revert")
             community_of_nodes = old_communities
@@ -254,263 +240,268 @@
             seed_of_cells=community_of_nodes,
             max_seeds_count=kept_communities_count + small_communities_count - 1,
             min_seed_size_quantile=min_seed_size_quantile,
             max_seed_size_quantile=max_seed_size_quantile,
             random_seed=random_seed,
         )
 
+    assert np.all(community_of_nodes >= 0)
+
     if inplace:
         ut.set_o_data(adata, "candidate", community_of_nodes, formatter=ut.groups_description)
         return None
 
-    if must_complete_cover:
-        assert np.min(community_of_nodes) == 0
-    else:
-        community_of_nodes[community_of_nodes < 0] = -1
-
     ut.log_return("candidate", community_of_nodes, formatter=ut.groups_description)
     return ut.to_pandas_series(community_of_nodes, index=adata.obs_names)
 
 
-def _optimize_split_communities(
+def _reduce_communities(
     outgoing_edge_weights: ut.CompressedMatrix,
     incoming_edge_weights: ut.CompressedMatrix,
     community_of_nodes: ut.NumpyVector,
     node_sizes: ut.NumpyVector,
     target_metacell_size: float,
-    max_metacell_size: Optional[float],
+    min_metacell_cells: Optional[int],
+    min_metacell_size: float,
+    max_metacell_size: float,
     max_split_min_cut_strength: Optional[float],
-    min_cut_seed_cells: Optional[int],
+    min_cut_seed_cells: int,
     must_complete_cover: bool,
     min_seed_size_quantile: float,
     max_seed_size_quantile: float,
     random_seed: int,
     cooldown_pass: float,
     cooldown_node: float,
     cooldown_phase: float,
     kept_communities_count: int,
     cold_temperature: float,
     atomic_candidates: Set[Tuple[int, ...]],
 ) -> Tuple[float, float]:
+    np.random.seed(random_seed)
     while True:
         ut.log_calc("cold_temperature", cold_temperature)
         score = _optimize_partitions(
             outgoing_edge_weights=outgoing_edge_weights,
             incoming_edge_weights=incoming_edge_weights,
             community_of_nodes=community_of_nodes,
+            low_partition_size=min_metacell_size,
+            target_partition_size=target_metacell_size,
+            high_partition_size=max_metacell_size,
+            node_sizes=node_sizes,
             random_seed=random_seed,
             cooldown_pass=cooldown_pass,
             cooldown_node=cooldown_node,
             cold_communities_count=kept_communities_count,
             cold_temperature=cold_temperature,
         )
 
         cold_temperature = cold_temperature * (1 - cooldown_phase)
         ut.log_calc("communities", community_of_nodes, formatter=ut.groups_description)
 
-        modified_communities_count, new_communities_count, kept_communities_count = _split_communities(
+        split_communities_count, cut_communities_count = _cut_split_communities(
             outgoing_edge_weights=outgoing_edge_weights,
             community_of_nodes=community_of_nodes,
             node_sizes=node_sizes,
-            target_metacell_size=target_metacell_size,
+            min_metacell_cells=min_metacell_cells,
             max_metacell_size=max_metacell_size,
             max_split_min_cut_strength=max_split_min_cut_strength,
             min_cut_seed_cells=min_cut_seed_cells,
             must_complete_cover=must_complete_cover,
             atomic_candidates=atomic_candidates,
         )
 
-        if new_communities_count > 0:
-            assert modified_communities_count > 0
+        if split_communities_count + cut_communities_count == 0:
+            return cold_temperature, score
+
+        kept_communities_count = np.max(community_of_nodes) + 1
+
+        if cut_communities_count > 0:
             _choose_seeds(
                 outgoing_edge_weights=outgoing_edge_weights,
                 incoming_edge_weights=incoming_edge_weights,
                 seed_of_cells=community_of_nodes,
-                max_seeds_count=kept_communities_count + new_communities_count,
+                max_seeds_count=np.max(community_of_nodes) + 2,
                 min_seed_size_quantile=min_seed_size_quantile,
                 max_seed_size_quantile=max_seed_size_quantile,
                 random_seed=random_seed,
             )
 
-        if modified_communities_count == 0:
-            return cold_temperature, score
-
 
-def _split_communities(
+def _cut_split_communities(
     *,
     outgoing_edge_weights: ut.CompressedMatrix,
     community_of_nodes: ut.NumpyVector,
     node_sizes: ut.NumpyVector,
-    target_metacell_size: float,
+    min_metacell_cells: Optional[int],
     max_metacell_size: Optional[float],
     max_split_min_cut_strength: Optional[float],
-    min_cut_seed_cells: Optional[int],
+    min_cut_seed_cells: int,
     must_complete_cover: bool,
     atomic_candidates: Set[Tuple[int, ...]],
-) -> Tuple[int, int, int]:
+) -> Tuple[int, int]:
     communities_count = np.max(community_of_nodes) + 1
     assert communities_count > 0
 
     if max_metacell_size is None and max_split_min_cut_strength is None:
         ut.logger().debug("no communities need to be split")
-        return (0, 0, communities_count)
+        return (False, False)
 
-    cancelled_communities: Set[int] = set()
     split_communities_count = 0
     cut_communities_count = 0
     next_new_community_index = communities_count
-    cancelled_total_size = 0
 
-    did_not_add = False
     for community_index in range(communities_count):
         community_mask = community_of_nodes == community_index
-        community_size = np.sum(node_sizes[community_mask])
+        community_node_sizes = node_sizes[community_mask]
+        community_size = np.sum(community_node_sizes)
 
-        if max_metacell_size is not None and community_size > max_metacell_size:
+        if (
+            max_metacell_size is not None
+            and community_size > max_metacell_size
+            and (min_metacell_cells is None or np.sum(community_mask) >= 2 * min_metacell_cells)
+        ):
             ut.logger().debug(
                 "community: %s nodes: %s size: %s is too large", community_index, np.sum(community_mask), community_size
             )
-            cancelled_total_size += community_size
-            cancelled_communities.add(community_index)
+            large_community_indices = np.where(community_mask)[0]
+            second_partition_indices = large_community_indices[
+                np.random.choice([False, True], size=len(large_community_indices))
+            ]
+            community_of_nodes[second_partition_indices] = next_new_community_index
+            next_new_community_index += 1
+            split_communities_count += 1
             continue
 
-    if len(cancelled_communities) == 0 and max_split_min_cut_strength is not None:
+    if split_communities_count == 0 and max_split_min_cut_strength is not None:
         for community_index in range(communities_count):
             community_mask = community_of_nodes == community_index
 
             community_indices = tuple(np.where(community_mask)[0])
             if community_indices in atomic_candidates:
                 continue
 
-            did_cut, did_split = _min_cut_community(
+            action = _min_cut_community(
                 outgoing_edge_weights=outgoing_edge_weights,
                 community_of_nodes=community_of_nodes,
                 cut_community_index=community_index,
                 max_split_min_cut_strength=max_split_min_cut_strength,
                 min_cut_seed_cells=min_cut_seed_cells,
                 must_complete_cover=must_complete_cover,
                 new_community_index=next_new_community_index,
             )
 
-            if not did_cut:
+            if action == "unchanged":
                 atomic_candidates.add(community_indices)
                 continue
 
-            cut_communities_count += 1
             ut.logger().debug(
-                "community: %s nodes: %s size: %s is too divided",
+                "community: %s nodes: %s size: %s was %s",
                 community_index,
                 np.sum(community_mask),
-                np.sum(node_sizes[community_mask]),
+                community_size,
+                action,
             )
-            if did_split:
+            if action == "split":
                 split_communities_count += 1
                 next_new_community_index += 1
+            else:
+                cut_communities_count += 1
 
-    cancelled_communities_count = len(cancelled_communities)
-    modified_communities_count = cut_communities_count + cancelled_communities_count
-    if modified_communities_count == 0:
-        ut.logger().debug("no communities were modified")
-        return (0, 0, communities_count)
-
-    ut.logger().debug("all communities: %s", communities_count)
-    ut.logger().debug("cut communities: %s", cut_communities_count)
-    ut.logger().debug("split communities: %s", split_communities_count)
-    ut.logger().debug("cancelled communities: %s", cancelled_communities_count)
-
-    if cancelled_communities_count > 0:
-        new_communities_count = max(ceil(cancelled_total_size / target_metacell_size), cancelled_communities_count + 1)
+    if split_communities_count + cut_communities_count > 0:
+        ut.logger().debug("old communities: %s", communities_count)
+        ut.logger().debug("cut communities: %s", cut_communities_count)
+        ut.logger().debug("split communities: %s", split_communities_count)
+        ut.logger().debug("total communities: %s", communities_count + split_communities_count)
     else:
-        new_communities_count = 0
-
-    if did_not_add and new_communities_count == 0:
-        new_communities_count = 1
-
-    ut.logger().debug("reclaimed communities: %s", new_communities_count)
+        ut.logger().debug("no communities were cut or split")
 
-    kept_communities_count = _cancel_communities(community_of_nodes, cancelled_communities)
-    ut.logger().debug("kept communities: %s", kept_communities_count)
-    assert kept_communities_count == communities_count + split_communities_count - cancelled_communities_count
-
-    return (modified_communities_count, new_communities_count, kept_communities_count)
+    return (split_communities_count, cut_communities_count)
 
 
 def _min_cut_community(
     outgoing_edge_weights: ut.CompressedMatrix,
     community_of_nodes: ut.NumpyVector,
     cut_community_index: int,
     max_split_min_cut_strength: float,
-    min_cut_seed_cells: Optional[int],
+    min_cut_seed_cells: int,
     must_complete_cover: bool,
     new_community_index: int,
-) -> Tuple[bool, bool]:
+) -> str:
     community_mask = community_of_nodes == cut_community_index
     if np.sum(community_mask) < 2:
-        return (False, False)
+        return "unchanged"
     community_edge_weights = outgoing_edge_weights[community_mask, :][:, community_mask]
     community_edge_weights += community_edge_weights.T
 
     cut, cut_strength = ut.min_cut(community_edge_weights)
     if cut_strength is None:
-        return (False, False)
+        return "unchanged"
+
+    if cut_strength == 0:
+        community_indices = np.where(community_mask)[0]
+        if len(cut.partition[0]) < len(cut.partition[1]):
+            small_partition = 0
+        else:
+            small_partition = 1
+        small_community_indices = community_indices[cut.partition[small_partition]]
+
+    if cut_strength > max_split_min_cut_strength:
+        return "unchanged"
 
     ut.logger().debug(
         "min cut community: %s partitions: %s + %s = %s strength: %s",
         cut_community_index,
         len(cut.partition[0]),
         len(cut.partition[1]),
         community_edge_weights.shape[0],
         cut_strength,
     )
 
-    if cut_strength > max_split_min_cut_strength:
-        return (False, False)
-
     community_indices = np.where(community_mask)[0]
+    if len(cut.partition[0]) < len(cut.partition[1]):
+        small_partition = 0
+    else:
+        small_partition = 1
 
-    if min_cut_seed_cells is not None:
-        if len(cut.partition[0]) < len(cut.partition[1]):
-            small_partition = 0
-        else:
-            small_partition = 1
-
-        if len(cut.partition[small_partition]) < min_cut_seed_cells:
-            if must_complete_cover:
-                return (False, False)
-            small_community_indices = community_indices[cut.partition[small_partition]]
-            community_of_nodes[small_community_indices] = -2
-            ut.logger().debug("give up on small cut: %s", len(cut.partition[small_partition]))
-            return (True, False)
-
-    second_partition_indices = community_indices[cut.partition[1]]
-    community_of_nodes[second_partition_indices] = new_community_index
-    return (True, True)
+    if len(cut.partition[small_partition]) >= min_cut_seed_cells:
+        second_partition_indices = community_indices[cut.partition[1]]
+        community_of_nodes[second_partition_indices] = new_community_index
+        return "split"
+
+    if must_complete_cover and cut_strength > 0:
+        ut.logger().debug("give up on small cut: %s", len(cut.partition[small_partition]))
+        return "unchanged"
+
+    small_community_indices = community_indices[cut.partition[small_partition]]
+    community_of_nodes[small_community_indices] = -1
+    return "cut"
 
 
 def _find_small_communities(
     *,
     community_of_nodes: ut.NumpyVector,
     node_sizes: ut.NumpyVector,
     min_metacell_size: Optional[float],
     min_metacell_cells: Optional[int],
 ) -> Tuple[Set[int], int]:
     communities_count = np.max(community_of_nodes) + 1
     assert communities_count > 0
 
     if min_metacell_size is None and min_metacell_cells is None:
-        ut.logger().debug("all communities are not too small")
+        ut.logger().debug("no communities are too small")
         return (set(), communities_count)
 
     small_communities: Set[int] = set()
     small_nodes_count = 0
 
     for community_index in range(communities_count):
         community_mask = community_of_nodes == community_index
         community_nodes_count = np.sum(community_mask)
-        community_size = np.sum(node_sizes[community_mask])
+        community_node_sizes = node_sizes[community_mask]
+        community_size = np.sum(community_node_sizes)
 
         if min_metacell_cells is not None and community_nodes_count < min_metacell_cells:
             ut.logger().debug("community: %s nodes: %s is too few", community_index, community_nodes_count)
         elif min_metacell_size is not None and community_size < min_metacell_size:
             ut.logger().debug(
                 "community: %s nodes: %s size: %s is too small", community_index, community_nodes_count, community_size
             )
@@ -590,60 +581,95 @@
     if seed_of_cells is None:
         seed_of_cells = np.full(size, -1, dtype="int32")
     else:
         assert seed_of_cells.dtype == "int32"
 
     assert outgoing_edge_weights.shape == incoming_edge_weights.shape == (len(seed_of_cells), len(seed_of_cells))
 
-    return _choose_seeds(
+    _choose_seeds(
         outgoing_edge_weights=outgoing_edge_weights,
         incoming_edge_weights=incoming_edge_weights,
         seed_of_cells=seed_of_cells,
         max_seeds_count=max_seeds_count,
         min_seed_size_quantile=min_seed_size_quantile,
         max_seed_size_quantile=max_seed_size_quantile,
         random_seed=random_seed,
     )
 
+    return seed_of_cells
+
 
+@ut.logged()
 @ut.timed_call()
 def _choose_seeds(
     *,
     outgoing_edge_weights: ut.CompressedMatrix,
     incoming_edge_weights: ut.CompressedMatrix,
     seed_of_cells: ut.NumpyVector,
     max_seeds_count: int,
     min_seed_size_quantile: float,
     max_seed_size_quantile: float,
     random_seed: int,
-) -> ut.NumpyVector:
+) -> None:
+    ut.log_calc("partial seeds", seed_of_cells, formatter=ut.groups_description)
+
     xt.choose_seeds(
         outgoing_edge_weights.data,
         outgoing_edge_weights.indices,
         outgoing_edge_weights.indptr,
         incoming_edge_weights.data,
         incoming_edge_weights.indices,
         incoming_edge_weights.indptr,
         random_seed,
         max_seeds_count,
         min_seed_size_quantile,
         max_seed_size_quantile,
         seed_of_cells,
     )
 
-    ut.log_calc("seeds", seed_of_cells, formatter=ut.groups_description)
-    return seed_of_cells
+    ut.log_calc("chosen seeds", seed_of_cells, formatter=ut.groups_description)
+    assert np.min(seed_of_cells) == 0
+
+
+@ut.logged()
+@ut.timed_call()
+def _complete_seeds(
+    *,
+    outgoing_edge_weights: ut.CompressedMatrix,
+    incoming_edge_weights: ut.CompressedMatrix,
+    seed_of_cells: ut.NumpyVector,
+    seeds_count: int,
+) -> None:
+    ut.log_calc("incomplete seeds", seed_of_cells, formatter=ut.groups_description)
+
+    xt.complete_seeds(
+        outgoing_edge_weights.data,
+        outgoing_edge_weights.indices,
+        outgoing_edge_weights.indptr,
+        incoming_edge_weights.data,
+        incoming_edge_weights.indices,
+        incoming_edge_weights.indptr,
+        seeds_count,
+        seed_of_cells,
+    )
+
+    ut.log_calc("completed seeds", seed_of_cells, formatter=ut.groups_description)
+    assert np.min(seed_of_cells) == 0
 
 
 @ut.logged()
 @ut.timed_call()
 def optimize_partitions(
     *,
     edge_weights: ut.CompressedMatrix,
     community_of_nodes: ut.NumpyVector,
+    low_partition_size: float,
+    target_partition_size: float,
+    high_partition_size: float,
+    node_sizes: ut.NumpyVector,
     cooldown_pass: float = pr.cooldown_pass,
     cooldown_node: float = pr.cooldown_node,
     random_seed: int,
 ) -> float:
     """
     Optimize partition to candidate metacells (communities) using the ``edge_weights``.
 
@@ -674,64 +700,85 @@
     to perform a final hill-climbing phase.
 
     This simulated-annealing-like behavior helps the algorithm to escape local maximums, although of
     course no claim is made of achieving the global maximum of the goal function.
     """
     outgoing_edge_weights = ut.mustbe_compressed_matrix(edge_weights)
     assert ut.is_layout(outgoing_edge_weights, "row_major")
+    assert 0 < low_partition_size < target_partition_size < high_partition_size
 
     incoming_edge_weights = ut.mustbe_compressed_matrix(ut.to_layout(outgoing_edge_weights, layout="column_major"))
     assert ut.is_layout(incoming_edge_weights, "column_major")
     return _optimize_partitions(
         outgoing_edge_weights=outgoing_edge_weights,
         incoming_edge_weights=incoming_edge_weights,
         random_seed=random_seed,
+        low_partition_size=low_partition_size,
+        target_partition_size=target_partition_size,
+        high_partition_size=high_partition_size,
+        node_sizes=node_sizes,
         cooldown_pass=cooldown_pass,
         cooldown_node=cooldown_node,
         community_of_nodes=community_of_nodes,
         cold_communities_count=0,
         cold_temperature=cooldown_pass,
     )
 
 
+@ut.logged()
 @ut.timed_call()
 def _optimize_partitions(
     *,
     outgoing_edge_weights: ut.CompressedMatrix,
     incoming_edge_weights: ut.CompressedMatrix,
     community_of_nodes: ut.NumpyVector,
+    low_partition_size: float,
+    target_partition_size: float,
+    high_partition_size: float,
+    node_sizes: ut.NumpyVector,
     cooldown_pass: float,
     cooldown_node: float,
     cold_communities_count: int,
     cold_temperature: float,
     random_seed: int,
 ) -> float:
     assert community_of_nodes.dtype == "int32"
+    assert node_sizes.dtype == "float32"
     score = xt.optimize_partitions(
         outgoing_edge_weights.data,
         outgoing_edge_weights.indices,
         outgoing_edge_weights.indptr,
         incoming_edge_weights.data,
         incoming_edge_weights.indices,
         incoming_edge_weights.indptr,
         random_seed,
+        low_partition_size,
+        target_partition_size,
+        high_partition_size,
+        node_sizes,
         cooldown_pass,
         cooldown_node,
         community_of_nodes,
         cold_communities_count,
         cold_temperature,
     )
     ut.log_calc("score", score)
+    ut.log_calc("partitions", community_of_nodes, formatter=ut.groups_description)
+    assert np.min(community_of_nodes) == 0
     return score
 
 
 @ut.logged()
 @ut.timed_call()
 def score_partitions(
     *,
+    low_partition_size: float,
+    target_partition_size: float,
+    high_partition_size: float,
+    node_sizes: ut.NumpyVector,
     edge_weights: ut.CompressedMatrix,
     partition_of_nodes: ut.NumpyVector,
     with_orphans: bool = True,
 ) -> None:
     """
     Compute the "stability" the "stability" goal function which is defined to be the ratio between
     (1) the probability that, selecting a random node and either a random outgoing edge or a random
@@ -740,15 +787,16 @@
     community (the fraction of its number of nodes out of the total).
 
     If ``with_orphans`` is True (the default), outlier nodes are included in the computation. In
     general we add 1e-6 to the product of the incoming and outgoing weights so we can safely log it
     for efficient computation; thus orphans are given a very small (non-zero) weight so the overall
     score is not zeroed even when including them.
     """
-    assert str(partition_of_nodes.dtype) == "int32"
+    assert partition_of_nodes.dtype == "int32"
+    assert node_sizes.dtype == "float32"
     outgoing_edge_weights = ut.mustbe_compressed_matrix(edge_weights)
     assert ut.is_layout(outgoing_edge_weights, "row_major")
 
     incoming_edge_weights = ut.mustbe_compressed_matrix(ut.to_layout(outgoing_edge_weights, layout="column_major"))
     assert ut.is_layout(incoming_edge_weights, "column_major")
 
     with ut.unfrozen(partition_of_nodes):
@@ -756,13 +804,17 @@
             score = xt.score_partitions(
                 outgoing_edge_weights.data,
                 outgoing_edge_weights.indices,
                 outgoing_edge_weights.indptr,
                 incoming_edge_weights.data,
                 incoming_edge_weights.indices,
                 incoming_edge_weights.indptr,
+                low_partition_size,
+                target_partition_size,
+                high_partition_size,
+                node_sizes,
                 partition_of_nodes,
                 with_orphans,
             )
 
     ut.log_calc("score", score)
     return score
```

### Comparing `metacells-0.8.0/metacells/tools/convey.py` & `metacells-0.9.0/metacells/tools/convey.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,25 +12,26 @@
 
 import metacells.utilities as ut
 
 __all__ = [
     "convey_group_to_obs",
     "convey_obs_to_obs",
     "convey_obs_to_group",
+    "convey_obs_fractions_to_group",
     "convey_obs_obs_to_group_group",
 ]
 
 
 @ut.logged()
 @ut.timed_call()
 def convey_group_to_obs(
     *,
     adata: AnnData,
     gdata: AnnData,
-    group: str,
+    group: str = "metacell",
     property_name: str,
     formatter: Optional[Callable[[Any], Any]] = None,
     to_property_name: Optional[str] = None,
     default: Any = None,
 ) -> None:
     """
     Project the value of a property from per-group data to per-observation data.
@@ -87,15 +88,15 @@
 
 @ut.logged()
 @ut.timed_call()
 def convey_obs_to_group(
     *,
     adata: AnnData,
     gdata: AnnData,
-    group: str,
+    group: str = "metacell",
     property_name: str,
     formatter: Optional[Callable[[Any], Any]] = None,
     to_property_name: Optional[str] = None,
     method: Callable[[ut.Vector], Any] = ut.most_frequent,
 ) -> None:
     """
     Project the value of a property from per-observation data to per-group data.
@@ -119,19 +120,58 @@
     assert gdata.n_obs == (np.max(group_of_obs) + 1)
     property_of_group = np.array([method(property_of_obs[group_of_obs == group]) for group in range(gdata.n_obs)])
     ut.set_o_data(gdata, to_property_name, property_of_group)
 
 
 @ut.logged()
 @ut.timed_call()
+def convey_obs_fractions_to_group(
+    *,
+    adata: AnnData,
+    gdata: AnnData,
+    group: str = "metacell",
+    property_name: str,
+    formatter: Optional[Callable[[Any], Any]] = None,
+    to_property_name: Optional[str] = None,
+) -> None:
+    """
+    Similar to ``convey_obs_to_group``, but create a per-metacell property for each value of the
+    per-cell property, storing the fraction of cells of the metacell that had that value.
+
+    The input annotated ``adata`` is expected to contain a per-observation (cell) annotation named
+    ``property_name`` and also a per-observation annotation named ``group`` which identifies the
+    group each observation (cell) belongs to, which must be an integer.
+
+    This will generate multiple new per-observation (group) annotation in ``gdata``, named
+    ``<to_property_name>_fraction_of_<value>`` (by default, the ``to_property_name`` is the same as ``property_name``),
+    containing the fraction of the metacell cells containing the specific property value.
+    """
+    if to_property_name is None:
+        to_property_name = property_name
+
+    property_of_obs = ut.get_o_numpy(adata, property_name, formatter=formatter)
+    unique_values = sorted(np.unique(property_of_obs))
+    for value in unique_values:
+        convey_obs_to_group(
+            adata=adata,
+            gdata=gdata,
+            group=group,
+            property_name=property_name,
+            to_property_name=f"{to_property_name}_fraction_of_{value}",
+            method=ut.fraction_of_grouped(value),
+        )
+
+
+@ut.logged()
+@ut.timed_call()
 def convey_obs_obs_to_group_group(
     *,
     adata: AnnData,
     gdata: AnnData,
-    group: str,
+    group: str = "metacell",
     property_name: str,
     formatter: Optional[Callable[[Any], Any]] = None,
     to_property_name: Optional[str] = None,
     method: Callable[[ut.Matrix], Any] = ut.nanmean_matrix,
 ) -> None:
     """
     Project the value of a property from per-observation-per-observation data to per-group-per-group
```

### Comparing `metacells-0.8.0/metacells/tools/dissolve.py` & `metacells-0.9.0/metacells/tools/dissolve.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,52 +21,48 @@
 @ut.expand_doc()
 @ut.timed_call()
 def dissolve_metacells(
     adata: AnnData,
     what: Union[str, ut.Matrix] = "__x__",
     *,
     candidates: Union[str, ut.Vector] = "candidate",
-    deviants: Optional[Union[str, ut.Vector]] = "cell_deviant_votes",
+    deviants: ut.Vector,
     target_metacell_size: float = pr.target_metacell_size,
     cell_sizes: Optional[Union[str, ut.Vector]] = pr.dissolve_cell_sizes,
     min_metacell_cells: int = pr.dissolve_min_metacell_cells,
     min_robust_size_factor: Optional[float] = pr.dissolve_min_robust_size_factor,
     min_convincing_size_factor: Optional[float] = pr.dissolve_min_convincing_size_factor,
     min_convincing_gene_fold_factor: float = pr.dissolve_min_convincing_gene_fold_factor,
-    abs_folds: bool = pr.dissolve_abs_folds,
-    inplace: bool = True,
-) -> Optional[ut.PandasFrame]:
+) -> None:
     """
     Dissolve too-small metacells based on ``what`` (default: {what}) data.
 
     **Input**
 
     Annotated ``adata``, where the observations are cells and the variables are genes, where
     ``what`` is a per-variable-per-observation matrix or the name of a per-variable-per-observation
     annotation containing such a matrix.
 
     **Returns**
 
+    Sets the following in ``adata``:
+
     Observation (Cell) Annotations
         ``metacell``
             The integer index of the metacell each cell belongs to. The metacells are in no
             particular order. Cells with no metacell assignment are given a metacell index of
             ``-1``.
 
         ``dissolved``
-            A boolean mask of the cells which were in a dissolved metacell.
-
-    If ``inplace`` (default: {inplace}), this is written to the data, and the function returns
-    ``None``. Otherwise this is returned as a pandas data frame (indexed by the observation names).
+           A boolean mask of the cells which were in a dissolved metacell.
 
     **Computation Parameters**
 
-    1. Mark all cells with non-zero ``deviants`` (default: {deviants}) as "outliers". This can be
-       the name of a per-observation (cell) annotation, or an explicit boolean mask of cells, or a
-       or ``None`` if there are no deviant cells to mark.
+    1. Mark all ``deviants`` cells "outliers". This can be the name of a per-observation (cell) annotation, or an
+       explicit boolean mask of cells, or a or ``None`` if there are no deviant cells to mark.
 
     2. Any metacell which has less cells than the ``min_metacell_cells`` is dissolved.
 
     3. We are trying to create metacells of size ``target_metacell_size``. Compute the sizes of the
        resulting metacells by summing the ``cell_sizes`` (default: {cell_sizes}). If it is ``None``,
        each has a size of one. These parameters are typically identical to these passed to
        :py:func:`metacells.tools.candidates.compute_candidate_metacells`.
@@ -74,29 +70,32 @@
     4. If ``min_robust_size_factor`` (default: {min_robust_size_factor}) is specified, then any
        metacell whose total size is at least ``target_metacell_size * min_robust_size_factor`` is
        preserved.
 
     5. If ``min_convincing_size_factor`` (default: {min_convincing_size_factor}) is specified, then any remaining
        metacells whose size is at least ``target_metacell_size * min_convincing_size_factor`` are preserved, given they
        contain at least one gene whose fold factor (log2((actual + 1) / (expected + 1))) is at least
-       ``min_convincing_gene_fold_factor`` (default: {min_convincing_gene_fold_factor}). If ``abs_folds``, consider the
-       absolute fold factors. That is, we only preserve these smaller metacells if there is at least one gene whose
-       expression is significantly different from the mean of the population.
+       ``min_convincing_gene_fold_factor`` (default: {min_convincing_gene_fold_factor}). Consider the absolute fold
+       factors. That is, we only preserve these smaller metacells if there is at least one gene whose expression is
+       significantly different from the mean of the population.
 
     6 . Any remaining metacell is dissolved into "outlier" cells.
     """
     dissolved_of_cells = np.zeros(adata.n_obs, dtype="bool")
 
     candidate_of_cells = ut.get_o_numpy(adata, candidates, formatter=ut.groups_description)
     candidate_of_cells = np.copy(candidate_of_cells)
 
     deviant_of_cells = ut.maybe_o_numpy(adata, deviants, formatter=ut.mask_description)
     if deviant_of_cells is not None:
         deviant_of_cells = deviant_of_cells > 0
-    cell_sizes = ut.maybe_o_numpy(adata, cell_sizes, formatter=ut.sizes_description)
+
+    if cell_sizes is not None:
+        cell_sizes = ut.get_o_numpy(adata, cell_sizes, formatter=ut.sizes_description)
+        ut.log_calc("cell_sizes", cell_sizes, formatter=ut.sizes_description)
 
     if deviant_of_cells is not None:
         candidate_of_cells[deviant_of_cells > 0] = -1
     candidate_of_cells = ut.compress_indices(candidate_of_cells)
     candidates_count = np.max(candidate_of_cells) + 1
 
     data = ut.get_vo_proper(adata, what, layout="column_major")
@@ -114,63 +113,48 @@
         min_convincing_size = target_metacell_size * min_convincing_size_factor
     ut.log_calc("min_convincing_size", min_convincing_size)
 
     did_dissolve = False
     for candidate_index in range(candidates_count):
         candidate_cell_indices = np.where(candidate_of_cells == candidate_index)[0]
         if not _keep_candidate(
-            adata,
             candidate_index,
             data=data,
             cell_sizes=cell_sizes,
             fraction_of_genes=fraction_of_genes,
             min_metacell_cells=min_metacell_cells,
             min_robust_size=min_robust_size,
             min_convincing_size=min_convincing_size,
             min_convincing_gene_fold_factor=min_convincing_gene_fold_factor,
-            abs_folds=abs_folds,
             candidates_count=candidates_count,
             candidate_cell_indices=candidate_cell_indices,
         ):
             dissolved_of_cells[candidate_cell_indices] = True
             candidate_of_cells[candidate_cell_indices] = -1
             did_dissolve = True
 
     if did_dissolve:
         metacell_of_cells = ut.compress_indices(candidate_of_cells)
     else:
         metacell_of_cells = candidate_of_cells
 
-    if inplace:
-        ut.set_o_data(adata, "dissolved", dissolved_of_cells, formatter=ut.mask_description)
-
-        ut.set_o_data(adata, "metacell", metacell_of_cells, formatter=ut.groups_description)
-        return None
-
-    ut.log_return("dissolved", dissolved_of_cells)
-    ut.log_return("metacell", metacell_of_cells, formatter=ut.groups_description)
-
-    obs_frame = ut.to_pandas_frame(index=adata.obs_names)
-    obs_frame["dissolved"] = dissolved_of_cells
-    obs_frame["metacell"] = metacell_of_cells
-    return obs_frame
+    ut.set_o_data(adata, "dissolved", dissolved_of_cells)
+    ut.set_o_data(adata, "metacell", metacell_of_cells, formatter=ut.groups_description)
 
 
 def _keep_candidate(  # pylint: disable=too-many-branches
-    adata: AnnData,
     candidate_index: int,
     *,
     data: ut.ProperMatrix,
     cell_sizes: Optional[ut.NumpyVector],
     fraction_of_genes: ut.NumpyVector,
     min_metacell_cells: int,
     min_robust_size: Optional[float],
     min_convincing_size: Optional[float],
     min_convincing_gene_fold_factor: float,
-    abs_folds: bool,
     candidates_count: int,
     candidate_cell_indices: ut.NumpyVector,
 ) -> bool:
     genes_count = data.shape[1]
 
     if cell_sizes is None:
         candidate_total_size = candidate_cell_indices.size
@@ -222,33 +206,25 @@
     assert candidate_data_of_genes.size == genes_count
     candidate_total = np.sum(candidate_data_of_genes)
     candidate_expected_of_genes = fraction_of_genes * candidate_total
     candidate_expected_of_genes += 1
     candidate_data_of_genes += 1
     candidate_data_of_genes /= candidate_expected_of_genes
     np.log2(candidate_data_of_genes, out=candidate_data_of_genes)
-    if abs_folds:
-        convincing_genes_mask = np.abs(candidate_data_of_genes) >= min_convincing_gene_fold_factor
-    else:
-        convincing_genes_mask = candidate_data_of_genes >= min_convincing_gene_fold_factor
+    convincing_genes_mask = np.abs(candidate_data_of_genes) >= min_convincing_gene_fold_factor
     keep_candidate = bool(np.any(convincing_genes_mask))
 
     if ut.logging_calc():
-        convincing_gene_indices = np.where(convincing_genes_mask)[0]
         if keep_candidate:
             ut.log_calc(
                 f'- candidate: {ut.progress_description(candidates_count, candidate_index, "candidate")} '
                 f"cells: {candidate_cell_indices.size} "
                 f"size: {candidate_total_size:g} "
-                f"is: convincing because:"
+                f"is: convincing"
             )
-            for fold_factor, name in reversed(
-                sorted(zip(candidate_data_of_genes[convincing_gene_indices], adata.var_names[convincing_gene_indices]))
-            ):
-                ut.log_calc(f"    {name}: {ut.fold_description(fold_factor)}")
         else:
             ut.log_calc(
                 f'- candidate: {ut.progress_description(candidates_count, candidate_index, "candidate")} '
                 f"cells: {candidate_cell_indices.size} "
                 f"size: {candidate_total_size:g} "
                 f"is: not convincing"
             )
```

### Comparing `metacells-0.8.0/metacells/tools/distinct.py` & `metacells-0.9.0/metacells/tools/distinct.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """,
-abs_folds
 Distincts
 ---------
 """
 
 import sys
 from typing import Optional
 from typing import Tuple
@@ -102,15 +101,14 @@
 @ut.timed_call()
 @ut.expand_doc()
 def find_distinct_genes(
     adata: AnnData,
     what: Union[str, ut.Matrix] = "distinct_fold",
     *,
     distinct_genes_count: int = pr.distinct_genes_count,
-    distinct_abs_folds: bool = pr.distinct_abs_folds,
     inplace: bool = True,
 ) -> Optional[Tuple[ut.PandasFrame, ut.PandasFrame]]:
     """
     Find for each observation (cell) the genes in which its ``what`` (default: {what}) value is most
     distinct from the general population. This is typically applied to the metacells data rather
     than to the cells data.
 
@@ -132,26 +130,25 @@
     ``None``. Otherwise this is returned as two pandas frames (indexed by the observation and
     distinct gene rank).
 
     **Computation Parameters**
 
     1. Fetch the previously computed per-observation-per-variable ``what`` data.
 
-    2. Keep the ``distinct_genes_count`` (default: {distinct_genes_count}) top fold factors. If ``distinct_abs_folds``
-       (default: ``distinct_abs_folds``), keep the top absolute fold factors.
+    2. Keep the ``distinct_genes_count`` (default: {distinct_genes_count}) top absolute fold factors.
     """
     assert 0 < distinct_genes_count < adata.n_vars
 
     distinct_gene_indices = np.empty((adata.n_obs, distinct_genes_count), dtype="int32")
     distinct_gene_folds = np.empty((adata.n_obs, distinct_genes_count), dtype="float32")
 
     fold_in_cells = ut.mustbe_numpy_matrix(ut.get_vo_proper(adata, what, layout="row_major"))
     extension_name = f"top_distinct_{fold_in_cells.dtype}_t"
     extension = getattr(xt, extension_name)
-    extension(distinct_gene_indices, distinct_gene_folds, fold_in_cells, distinct_abs_folds)
+    extension(distinct_gene_indices, distinct_gene_folds, fold_in_cells)
 
     if inplace:
         ut.set_oa_data(adata, "cell_distinct_gene_indices", distinct_gene_indices)
         ut.set_oa_data(adata, "cell_distinct_gene_folds", distinct_gene_folds)
         return None
 
     return (
```

### Comparing `metacells-0.8.0/metacells/tools/downsample.py` & `metacells-0.9.0/metacells/tools/downsample.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 def downsample_cells(
     adata: AnnData,
     what: Union[str, ut.Matrix] = "__x__",
     *,
     downsample_min_cell_quantile: float = pr.downsample_min_cell_quantile,
     downsample_min_samples: float = pr.downsample_min_samples,
     downsample_max_cell_quantile: float = pr.downsample_max_cell_quantile,
-    random_seed: int = pr.random_seed,
     inplace: bool = True,
+    random_seed: int,
 ) -> Optional[Tuple[int, ut.PandasFrame]]:
     """
     Downsample the values of ``what`` (default: {what}) data.
 
     Downsampling is an effective way to get the same number of samples in multiple cells
     (that is, the same number of total UMIs in multiple cells), and serves as an alternative to
     normalization (e.g., working with UMI fractions instead of raw UMI counts).
@@ -73,16 +73,16 @@
        reasonable downsampled total number of samples, so if possible we increase the number of
        samples, as long as at most ``downsample_min_cell_quantile`` (default:
        {downsample_min_cell_quantile}) cells will have lower number of samples. We'd also like all
        (most) cells to end up with the same downsampled total number of samples, so if we have to we
        decrease the number of samples to ensure at most ``downsample_max_cell_quantile`` (default:
        {downsample_max_cell_quantile}) cells will have a lower number of samples.
 
-    3. Downsample each cell so that it has at most the selected number of samples. Use the
-       ``random_seed`` to allow making this replicable.
+    3. Downsample each cell so that it has at most the selected number of samples. Specify a non-zero
+       ``random_seed`` to make this reproducible.
     """
     total_per_cell = ut.get_o_numpy(adata, what, sum=True)
 
     samples = int(
         round(
             min(
                 max(downsample_min_samples, np.quantile(total_per_cell, downsample_min_cell_quantile)),
```

### Comparing `metacells-0.8.0/metacells/tools/filter.py` & `metacells-0.9.0/metacells/tools/filter.py`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/metacells/tools/group.py` & `metacells-0.9.0/metacells/tools/group.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Group
 -----
 """
 
+from hashlib import shake_128
 from typing import Any
 from typing import Callable
+from typing import List
 from typing import Optional
 from typing import Union
 
 import numpy as np
 from anndata import AnnData  # type: ignore
 
 import metacells.utilities as ut
@@ -23,14 +25,15 @@
 @ut.timed_call()
 def group_obs_data(
     adata: AnnData,
     what: Union[str, ut.Matrix] = "__x__",
     *,
     groups: Union[str, ut.Vector],
     name: Optional[str] = None,
+    prefix: Optional[str] = None,
 ) -> Optional[AnnData]:
     """
     Compute new data which has the ``what`` (default: {what}) sum of the observations (cells) for
     each group.
 
     For example, having computed a metacell index for each cell, compute the per-metacell data
     for further analysis.
@@ -50,14 +53,18 @@
 
     An annotated data where each observation is the sum of the group of original observations
     (cells). Observations with a negative group index are discarded. If all observations are
     discarded, return ``None``.
 
     The new data will contain only:
 
+    * A single observation for each group. The name of each observation will be the optional ``prefix``
+      (default: {prefix}), followed by the group's index, followed by ``.`` and a 2-digit checksum of
+      the grouped members.
+
     * An ``X`` member holding the summed-per-group data.
 
     * A new ``grouped`` per-observation data which counts, for each group, the number
       of grouped observations summed into it.
 
     If ``name`` is not specified, the data will be unnamed. Otherwise, if it starts with a ``.``, it
     will be appended to the current name (if any). Otherwise, ``name`` is the new name.
@@ -68,23 +75,40 @@
     results = ut.sum_groups(data, group_of_cells, per="row")
     if results is None:
         return None
     summed_data, cell_counts = results
 
     gdata = AnnData(summed_data)
     gdata.var_names = adata.var_names
+    gdata.obs_names = _obs_names(prefix or "", ut.to_numpy_vector(adata.obs_names), group_of_cells)
 
     ut.set_name(gdata, ut.get_name(adata))
     ut.set_name(gdata, name)
 
     ut.set_o_data(gdata, "grouped", cell_counts, formatter=ut.sizes_description)
 
     return gdata
 
 
+# TODO: Replicated in metacells.pipeline.collect
+def _obs_names(prefix: str, name_of_members: ut.NumpyVector, group_of_members: ut.NumpyVector) -> List[str]:
+    groups_count = np.max(group_of_members) + 1
+    name_of_groups: List[str] = []
+    prefix = prefix or ""
+    for group_index in range(groups_count):
+        groups_mask = group_of_members == group_index
+        assert np.any(groups_mask)
+        hasher = shake_128()
+        for member_name in name_of_members[groups_mask]:
+            hasher.update(member_name.encode("utf8"))
+        checksum = int(hasher.hexdigest(16), 16) % 10
+        name_of_groups.append(f"{prefix}{group_index}.{checksum:02d}")
+    return name_of_groups
+
+
 @ut.logged()
 @ut.timed_call()
 @ut.expand_doc()
 def group_obs_annotation(
     adata: AnnData,
     gdata: AnnData,
     *,
@@ -141,15 +165,16 @@
 
     value_of_groups = np.empty(gdata.n_obs, dtype=values_of_cells.dtype)
 
     assert method in ("unique", "majority")
 
     if method == "unique":
         with ut.timed_step(".unique"):
-            value_of_groups[group_of_cells] = values_of_cells
+            grouped_mask = group_of_cells >= 0
+            value_of_groups[group_of_cells[grouped_mask]] = values_of_cells[grouped_mask]
 
     else:
         assert method == "majority"
         with ut.timed_step(".majority"):
             for group_index in range(gdata.n_obs):
                 cells_mask = group_of_cells == group_index
                 cells_count = np.sum(cells_mask)
```

### Comparing `metacells-0.8.0/metacells/tools/high.py` & `metacells-0.9.0/metacells/tools/high.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,87 +9,26 @@
 import numpy as np
 from anndata import AnnData  # type: ignore
 
 import metacells.parameters as pr
 import metacells.utilities as ut
 
 __all__ = [
-    "find_top_feature_genes",
     "find_high_total_genes",
     "find_high_topN_genes",
     "find_high_fraction_genes",
     "find_high_normalized_variance_genes",
     "find_high_relative_variance_genes",
-    "find_metacells_significant_genes",
+    "find_metacells_marker_genes",
 ]
 
 
 @ut.logged()
 @ut.timed_call()
 @ut.expand_doc()
-def find_top_feature_genes(
-    adata: AnnData,
-    *,
-    max_genes: int = pr.max_top_feature_genes,
-    inplace: bool = True,
-) -> Optional[ut.PandasSeries]:
-    """
-    Find genes which have high ``feature_gene`` value.
-
-    This is applied after computing metacells to pick the "strongest" feature genes. If using the
-    direct algorithm (:py:func:`metacells.pipeline.direct.compute_direct_metacells`) then all
-    feature genes are equally "strong"; however, if using the divide-and-conquer algorithm
-    (:py:func:`metacells.pipeline.divide_and_conquer.divide_and_conquer_pipeline`,
-    :py:func:`metacells.pipeline.divide_and_conquer.compute_divide_and_conquer_metacells`) then this
-    will pick the genes which were most commonly used as features across all the piles.
-
-    **Input**
-
-    Annotated ``adata``, where the observations are cells and the variables are genes, where
-    ``feature_gene`` is a per-variable (gene) annotation counting how many times each gene was used
-    as a feature.
-
-    **Returns**
-
-    Variable (Gene) Annotations
-        ``top_feature_gene``
-            A boolean mask indicating whether each gene was found to be a top feature gene.
-
-    If ``inplace`` (default: {inplace}), this is written to the data, and the function returns
-    ``None``. Otherwise this is returned as a pandas series (indexed by the variable names).
-
-    **Computation Parameters**
-
-    1. Look for the lowest positive ``feature_gene`` threshold such that at most ``max_genes`` are
-       picked as top feature genes. Note we may still pick more than ``max_genes``, for example when
-       using the direct algorithm, we always return all feature genes as there's no way to
-       distinguish between them using the ``feature_gene`` data.
-    """
-    feature_of_gene = ut.get_v_numpy(adata, "feature_gene", formatter=ut.mask_description)
-    max_threshold = np.max(feature_of_gene)
-    assert max_threshold > 0
-    threshold = 0
-    selected_count = max_genes + 1
-    while selected_count > max_genes and threshold < max_threshold:
-        threshold = threshold + 1
-        genes_mask = feature_of_gene >= threshold
-        selected_count = np.sum(genes_mask)
-        ut.log_calc(f"threshold: {threshold} selected: {selected_count}")
-
-    if inplace:
-        ut.set_v_data(adata, "top_feature_gene", genes_mask)
-        return None
-
-    ut.log_return("top_feature_gene", genes_mask)
-    return ut.to_pandas_series(genes_mask, index=adata.var_names)
-
-
-@ut.logged()
-@ut.timed_call()
-@ut.expand_doc()
 def find_high_total_genes(
     adata: AnnData,
     what: Union[str, ut.Matrix] = "__x__",
     *,
     min_gene_total: int,
     inplace: bool = True,
 ) -> Optional[ut.PandasSeries]:
@@ -139,16 +78,16 @@
 @ut.logged()
 @ut.timed_call()
 @ut.expand_doc()
 def find_high_topN_genes(  # pylint: disable=invalid-name
     adata: AnnData,
     what: Union[str, ut.Matrix] = "__x__",
     *,
-    topN: int,  # pylint: disable=invalid-name
-    min_gene_topN: int,  # pylint: disable=invalid-name
+    topN: int,
+    min_gene_topN: int,
     inplace: bool = True,
 ) -> Optional[ut.PandasSeries]:
     """
     Find genes which have high total top-Nth value of ``what`` (default: {what}) data.
 
     This should typically only be applied to downsampled data to ensure that variance in sampling
     depth does not affect the result.
@@ -256,15 +195,15 @@
 ) -> Optional[ut.PandasSeries]:
     """
     Find genes which have high normalized variance of ``what`` (default: {what}) data.
 
     The normalized variance measures the variance / mean of each gene. See
     :py:func:`metacells.utilities.computation.normalized_variance_per` for details.
 
-    Genes with a high normalized variance are "noisy", that is, have significantly different
+    Genes with a high normalized variance are "bursty", that is, have significantly different
     expression level in different cells.
 
     **Input**
 
     Annotated ``adata``, where the observations are cells and the variables are genes, where
     ``what`` is a per-variable-per-observation matrix or the name of a per-variable-per-observation
     annotation containing such a matrix.
@@ -314,15 +253,15 @@
     """
     Find genes which have high relative variance of ``what`` (default: {what}) data.
 
     The relative variance measures the variance / mean of each gene relative to the other genes with
     a similar level of expression. See
     :py:func:`metacells.utilities.computation.relative_variance_per` for details.
 
-    Genes with a high relative variance are good candidates for being selected as "feature genes",
+    Genes with a high relative variance are good candidates for being selected as "marker genes",
     that is, be used to compute the similarity between cells. Using the relative variance
     compensates for the bias for selecting higher-expression genes, whose normalized variance can to
     be larger due to random noise alone.
 
     **Input**
 
     Annotated ``adata``, where the observations are cells and the variables are genes, where
@@ -359,76 +298,77 @@
     ut.log_return("high_relative_variance_genes", genes_mask)
     return ut.to_pandas_series(genes_mask, index=adata.var_names)
 
 
 @ut.logged()
 @ut.timed_call()
 @ut.expand_doc()
-def find_metacells_significant_genes(
+def find_metacells_marker_genes(
     adata: AnnData,
     what: Union[str, ut.Matrix] = "__x__",
     *,
-    min_gene_range_fold: float = pr.min_significant_metacells_gene_range_fold_factor,
-    normalization: float = pr.metacells_gene_range_normalization,
-    min_gene_fraction: float = pr.min_significant_metacells_gene_fraction,
+    min_gene_range_fold: float = pr.min_marker_metacells_gene_range_fold_factor,
+    regularization: float = pr.metacells_gene_range_regularization,
+    min_max_gene_fraction: float = pr.min_marker_max_metacells_gene_fraction,
     inplace: bool = True,
 ) -> Optional[ut.PandasSeries]:
     """
-    Find genes which have a significant signal in metacells data. This computation is too unreliable to be used on
-    cells.
+    Find "marker" genes which have a significant signal in metacells data. This computation is too unreliable to be
+    used on cells.
 
     Find genes which have a high maximal expression in at least one metacell, and a wide range of expression across the
     metacells. Such genes are good candidates for being used as marker genes and/or to compute distances between
     metacells.
 
     **Input**
 
     Annotated ``adata``, where the observations are cells and the variables are genes, where
     ``what`` is a per-variable-per-observation matrix or the name of a per-variable-per-observation
     annotation containing such a matrix.
 
     **Returns**
 
     Variable (Gene) Annotations
-        ``significant_gene``
-            A boolean mask indicating whether each gene was found to be significant.
+        ``marker_gene``
+            A boolean mask indicating whether each gene is a "marker".
 
     If ``inplace`` (default: {inplace}), this is written to the data, and the function returns
     ``None``. Otherwise this is returned as a pandas series (indexed by the variable names).
 
     **Computation Parameters**
 
     1. Compute the minimal and maximal expression level of each gene.
 
-    2. Select the genes whose fold factor (log2 of maximal over minimal value, using the ``normalization``
-       (default: {normalization}) is at least ``min_gene_range_fold`` (default: {min_gene_range_fold}).
+    2. Select the genes whose fold factor (log2 of maximal over minimal value, using the ``regularization``
+       (default: {regularization}) is at least ``min_gene_range_fold`` (default: {min_gene_range_fold}).
 
-    3. Select the genes whose maximal expression is at least ``min_gene_fraction`` (default: {min_gene_fraction}).
+    3. Select the genes whose maximal expression is at least ``min_max_gene_fraction`` (default:
+       {min_max_gene_fraction}).
     """
-    assert normalization >= 0
+    assert regularization >= 0
 
     data = ut.get_vo_proper(adata, what, layout="row_major")
     fractions_of_genes = ut.to_layout(ut.fraction_by(data, by="row"), layout="column_major")
 
     min_fraction_of_genes = ut.min_per(fractions_of_genes, per="column")
     max_fraction_of_genes = ut.max_per(fractions_of_genes, per="column")
 
-    high_max_fraction_genes_mask = max_fraction_of_genes >= min_gene_fraction
+    high_max_fraction_genes_mask = max_fraction_of_genes >= min_max_gene_fraction
     ut.log_calc("high max fraction genes", high_max_fraction_genes_mask)
 
-    min_fraction_of_genes += normalization
-    max_fraction_of_genes += normalization
+    min_fraction_of_genes += regularization
+    max_fraction_of_genes += regularization
 
     max_fraction_of_genes /= min_fraction_of_genes
     range_fold_of_genes = np.log2(max_fraction_of_genes, out=max_fraction_of_genes)
 
     high_range_genes_mask = range_fold_of_genes >= min_gene_range_fold
     ut.log_calc("high range genes", high_range_genes_mask)
 
-    significant_genes_mask = high_max_fraction_genes_mask & high_range_genes_mask
+    marker_genes_mask = high_max_fraction_genes_mask & high_range_genes_mask
 
     if inplace:
-        ut.set_v_data(adata, "significant_gene", significant_genes_mask)
+        ut.set_v_data(adata, "marker_gene", marker_genes_mask)
         return None
 
-    ut.log_return("significant_genes", significant_genes_mask)
-    return ut.to_pandas_series(significant_genes_mask, index=adata.var_names)
+    ut.log_return("marker_genes", marker_genes_mask)
+    return ut.to_pandas_series(marker_genes_mask, index=adata.var_names)
```

### Comparing `metacells-0.8.0/metacells/tools/knn_graph.py` & `metacells-0.9.0/metacells/tools/knn_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,20 +147,14 @@
        This gives us a dense asymmetric ``<elements>_outgoing_ranks`` matrix.
 
     2. Convert the asymmetric outgoing ranks matrix into a symmetric ``var_balanced_ranks`` matrix
        by element-wise multiplying it with its transpose and taking the square root. That is, for
        each edge to be high-balanced-rank, the geomean of its outgoing rank has to be high in both
        nodes it connects.
 
-       .. note::
-
-            This can drastically reduce the degree of the nodes, since to survive an edge needs to
-            have been in the top ranks for both its nodes (as multiplying with zero drops the edge).
-            This is why the ``balanced_ranks_factor`` needs to be large-ish.
-
     3. Keeping only balanced ranks of up to ``k * k * balanced_ranks_factor`` (default:
        {balanced_ranks_factor}). This does a preliminary pruning of low-quality edges.
 
     4. Prune the edges, keeping only the ``k * incoming_degree_factor`` (default: k * {incoming_degree_factor})
        highest-ranked incoming edges for each node, and then only the ``k * outgoing_degree_factor`` (default:
        {outgoing_degree_factor}) highest-ranked outgoing edges for each node, while ensuring that the
        highest-balanced-ranked outgoing edge of each node is preserved. This gives us an asymmetric ``var_pruned_ranks``
@@ -292,21 +286,21 @@
     with ut.timed_step(".sqrt"):
         np.sqrt(dense_balanced_ranks, out=dense_balanced_ranks)
 
     max_rank = k * balanced_ranks_factor
     ut.log_calc("max_rank", max_rank)
 
     dense_balanced_ranks *= -1
-    dense_balanced_ranks += 2 ** 21
+    dense_balanced_ranks += 2**21
 
     with ut.timed_step("numpy.argmax"):
         ut.timed_parameters(size=size)
         max_index_of_each = ut.to_numpy_vector(dense_balanced_ranks.argmax(axis=1))  #
 
-    dense_balanced_ranks += max_rank + 1 - 2 ** 21
+    dense_balanced_ranks += max_rank + 1 - 2**21
 
     preserved_row_indices = np.arange(size)
     preserved_column_indices = max_index_of_each
     preserved_balanced_ranks = ut.to_numpy_vector(dense_balanced_ranks[preserved_row_indices, preserved_column_indices])
 
     preserved_balanced_ranks[preserved_balanced_ranks < 1] = 1
```

### Comparing `metacells-0.8.0/metacells/tools/layout.py` & `metacells-0.9.0/metacells/tools/layout.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Layout
 ------
 """
 
+import warnings
 from typing import Optional
 from typing import Union
 
 import numpy as np
 import scipy.sparse as sp  # type: ignore
 import umap  # type: ignore
 from anndata import AnnData  # type: ignore
@@ -23,20 +24,20 @@
 @ut.logged()
 @ut.timed_call()
 @ut.expand_doc()
 def umap_by_distances(
     adata: AnnData,
     distances: Union[str, ut.ProperMatrix] = "umap_distances",
     *,
-    prefix: str = "umap",
+    prefix: str = "",
     k: int = pr.umap_k,
     dimensions: int = 2,
     min_dist: float = pr.umap_min_dist,
     spread: float = pr.umap_spread,
-    random_seed: int = pr.random_seed,
+    random_seed: int,
 ) -> None:
     """
     Compute layout for the observations using UMAP, based on a distances matrix.
 
     **Input**
 
     The input annotated ``adata`` is expected to contain a per-observation-per-observation property
@@ -45,25 +46,25 @@
     diagonal).
 
     **Returns**
 
     Sets the following annotations in ``adata``:
 
     Observation (Cell) Annotations
-        ``<prefix>_x``, ``<prefix>_y``
+        ``<prefix>x``, ``<prefix>y``
             Coordinates for UMAP 2D projection of the observations (if ``dimensions`` is 2).
-        ``<prefix>_u``, ``<prefix>_v``, ``<prefix>_3``
+        ``<prefix>u``, ``<prefix>v``, ``<prefix>w``
             Coordinates for UMAP 3D projection of the observations (if ``dimensions`` is 3).
 
     **Computation Parameters**
 
     1. Invoke UMAP to compute a layout of some ``dimensions`` (default: {dimensions}D) using
        ``min_dist`` (default: {min_dist}), ``spread`` (default: {spread}) and ``k`` (default: {k}).
-       If the spread is lower than the minimal distance, it is raised. If ``random_seed`` (default:
-       {random_seed}) is not zero, then it is passed to UMAP to force the computation to be
+       If the spread is lower than the minimal distance, it is raised. If ``random_seed``
+       is not zero, then it is passed to UMAP to force the computation to be
        reproducible. However, this means UMAP will use a single-threaded implementation that will be
        slower.
     """
     assert dimensions in (2, 3)
     if isinstance(distances, str):
         distances_matrix = ut.get_oo_proper(adata, distances)
     else:
@@ -77,26 +78,29 @@
     n_neighbors = min(k, adata.n_obs - 2)
 
     random_state: Optional[int] = None
     if random_seed != 0:
         random_state = random_seed
 
     try:
-        coordinates = umap.UMAP(
-            metric="precomputed",
-            n_neighbors=n_neighbors,
-            spread=spread,
-            min_dist=min_dist,
-            n_components=dimensions,
-            random_state=random_state,
-        ).fit_transform(distances_csr)
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            coordinates = umap.UMAP(
+                metric="precomputed",
+                n_neighbors=n_neighbors,
+                spread=spread,
+                min_dist=min_dist,
+                n_components=dimensions,
+                random_state=random_state,
+            ).fit_transform(distances_csr)
     except ValueError:
         # UMAP implementation doesn't know how to handle too few edges.
         # However, it considers structural zeros as real edges.
-        distances_matrix = distances_matrix + 1.0  # type: ignore
+        distances_matrix = ut.to_numpy_matrix(distances_matrix, copy=True)
+        distances_matrix += 1.0
         np.fill_diagonal(distances_matrix, 0.0)
         distances_csr = sp.csr_matrix(distances_matrix)
         distances_csr.data -= 1.0
         coordinates = umap.UMAP(
             metric="precomputed", n_neighbors=n_neighbors, spread=spread, min_dist=min_dist, random_state=random_state
         ).fit_transform(distances_csr)
 
@@ -116,62 +120,61 @@
     elif dimensions == 3:
         all_names = ["u", "v", "w"]
     else:
         assert False
 
     order = np.argsort(all_sizes)
     for axis, name in zip(order, all_names):
-        ut.set_o_data(adata, f"{prefix}_{name}", all_coordinates[axis])
+        ut.set_o_data(adata, f"{prefix}{name}", all_coordinates[axis])
 
 
 @ut.logged()
 @ut.timed_call()
 @ut.expand_doc()
 def spread_coordinates(
     adata: AnnData,
     *,
-    prefix: str = "umap",
-    suffix: str = "spread",
-    cover_fraction: float = pr.cover_fraction,
-    noise_fraction: float = pr.noise_fraction,
-    random_seed: int = pr.random_seed,
+    prefix: str = "",
+    suffix: str = "_spread",
+    cover_fraction: float = pr.spread_cover_fraction,
+    noise_fraction: float = pr.spread_noise_fraction,
+    random_seed: int,
 ) -> None:
     """
     Move UMAP points so they cover some fraction of the plot area without overlapping.
 
     **Input**
 
     The input annotated ``adata`` is expected to contain the per-observation properties
-    ``<prefix>_x`` and ``<prefix>_y`` (default prefix: {prefix}) which contain the UMAP coordinates.
+    ``<prefix>x`` and ``<prefix>y`` (default prefix: {prefix}) which contain the UMAP coordinates.
 
     **Returns**
 
     Sets the following annotations in ``adata``:
 
     Observation (Cell) Annotations
-        ``<prefix>_x_<suffix>``, ``<prefix>_y_<suffix>`` (default suffix: {suffix})
+        ``<prefix>x<suffix>``, ``<prefix>y<suffix>`` (default suffix: {suffix})
             The new coordinates which will be spread out so the points do not overlap and
             cover some fraction of the total plot area.
 
     **Computation Parameters**
 
     1. Move the points so they cover ``cover_fraction`` (default: {cover_fraction}) of the total
        plot area. Also add a noise of the ``noise_fraction`` (default: {noise_fraction}) of the
-       minimal distance between the
-       points, using the ``random_seed`` (default: {random_seed}).
+       minimal distance between the points. A non-zero ``random_seed`` will make this reproducible.
     """
     assert 0 < cover_fraction < 1
     assert noise_fraction >= 0
 
-    x_coordinates = ut.get_o_numpy(adata, f"{prefix}_x")
-    y_coordinates = ut.get_o_numpy(adata, f"{prefix}_y")
+    x_coordinates = ut.get_o_numpy(adata, f"{prefix}x")
+    y_coordinates = ut.get_o_numpy(adata, f"{prefix}y")
 
     x_coordinates, y_coordinates = ut.cover_coordinates(
         x_coordinates,
         y_coordinates,
         cover_fraction=cover_fraction,
         noise_fraction=noise_fraction,
         random_seed=random_seed,
     )
 
-    ut.set_o_data(adata, f"{prefix}_x_{suffix}", x_coordinates)
-    ut.set_o_data(adata, f"{prefix}_y_{suffix}", y_coordinates)
+    ut.set_o_data(adata, f"{prefix}x{suffix}", x_coordinates)
+    ut.set_o_data(adata, f"{prefix}y{suffix}", y_coordinates)
```

### Comparing `metacells-0.8.0/metacells/tools/mask.py` & `metacells-0.9.0/metacells/tools/mask.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Mask
 ----
 """
 
-from typing import List
+from typing import Collection
 from typing import Optional
 
 from anndata import AnnData  # type: ignore
 
 import metacells.utilities as ut
 
 __all__ = [
@@ -16,15 +16,15 @@
 
 
 @ut.logged()
 @ut.timed_call()
 @ut.expand_doc()
 def combine_masks(  # pylint: disable=too-many-branches,too-many-statements
     adata: AnnData,
-    masks: List[str],
+    masks: Collection[str],
     *,
     invert: bool = False,
     to: Optional[str] = None,
 ) -> Optional[ut.PandasSeries]:
     """
     Combine different pre-computed masks into a final overall mask.
 
@@ -35,40 +35,38 @@
     **Returns**
 
     If ``to`` (default: {to}) is ``None``, returns the computed mask. Otherwise, sets the
     mask as an annotation (per-variable or per-observation depending on the type of the combined masks).
 
     **Computation Parameters**
 
-    1. For each of the mask in ``masks``, fetch it. Silently ignore missing masks if the name has a
-       ``?`` suffix. Invert the mask if the name has a ``~`` prefix. If the name has a ``|`` prefix
-       (before the ``~`` prefix, if any), then bitwise-OR the mask into the OR mask, otherwise (or if
-       it has a ``&`` prefix), bitwise-AND the mask into the AND mask.
+    1. For each of the mask in ``masks``, in order (left to right), fetch it. Silently ignore missing masks if the name
+       has a ``?`` suffix. If the first character of the mask name is ``&``, restrict the current mask, otherwise the
+       first character must be ``|`` and we'll expand the mask (for the 1st mask, the mask becomes the current mask
+       regardless of the 1st character). If the following character is ``~``, first invert the mask before applying it.
 
-    2. Combine (bitwise-AND) the AND mask and the OR mask into a single mask.
-
-    3. If ``invert`` (default: {invert}), invert the result combined mask.
+    3. If ``invert`` (default: {invert}), invert the final result mask.
     """
     assert len(masks) > 0
 
     per: Optional[str] = None
 
-    and_mask: Optional[ut.NumpyVector] = None
-    or_mask: Optional[ut.NumpyVector] = None
+    result_mask: Optional[ut.NumpyVector] = None
 
     for mask_name in masks:
         log_mask_name = mask_name
 
         if mask_name[0] == "|":
             is_or = True
             mask_name = mask_name[1:]
-        else:
+        elif mask_name[0] == "&":
             is_or = False
-            if mask_name[0] == "&":
-                mask_name = mask_name[1:]
+            mask_name = mask_name[1:]
+        else:
+            raise ValueError(f"invalid mask name: {mask_name} (does not start with & or |)")
 
         if mask_name[0] == "~":
             invert_mask = True
             mask_name = mask_name[1:]
         else:
             invert_mask = False
 
@@ -100,45 +98,33 @@
 
         if per is None:
             per = mask_per
         else:
             if mask_per != per:
                 raise ValueError("mixing per-observation and per-variable masks")
 
-        if is_or:
-            if or_mask is None:
-                or_mask = mask
-            else:
-                or_mask = or_mask | mask
-        else:
-            if and_mask is None:
-                and_mask = mask
-            else:
-                and_mask = and_mask & mask
-
-    if and_mask is not None:
-        if or_mask is not None:
-            combined_mask = and_mask & or_mask
+        if result_mask is None:
+            result_mask = mask
+        elif is_or:
+            result_mask = result_mask | mask
         else:
-            combined_mask = and_mask
-    else:
-        if or_mask is not None:
-            combined_mask = or_mask
-        else:
-            raise ValueError("no masks to combine")
+            result_mask = result_mask & mask
+
+    if result_mask is None:
+        raise ValueError("no masks to combine")
 
     if invert:
-        combined_mask = ~combined_mask
+        result_mask = ~result_mask
 
     if to is None:
-        ut.log_return("combined", combined_mask)
+        ut.log_return("result", result_mask)
         if per == "o":
-            return ut.to_pandas_series(combined_mask, index=adata.obs_names)
+            return ut.to_pandas_series(result_mask, index=adata.obs_names)
         assert per == "v"
-        return ut.to_pandas_series(combined_mask, index=adata.var_names)
+        return ut.to_pandas_series(result_mask, index=adata.var_names)
 
     if per == "o":
-        ut.set_o_data(adata, to, combined_mask)
+        ut.set_o_data(adata, to, result_mask)
     else:
-        ut.set_v_data(adata, to, combined_mask)
+        ut.set_v_data(adata, to, result_mask)
 
     return None
```

### Comparing `metacells-0.8.0/metacells/tools/named.py` & `metacells-0.9.0/metacells/tools/named.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,50 +17,77 @@
     "find_named_genes",
 ]
 
 
 @ut.logged()
 @ut.timed_call()
 @ut.expand_doc()
-def find_named_genes(
+def find_named_genes(  # pylint: disable=too-many-branches
     adata: AnnData,
     *,
+    name_property: Optional[str] = None,
     names: Optional[Collection[str]] = None,
     patterns: Optional[Collection[Union[str, Pattern]]] = None,
     to: Optional[str] = None,
     invert: bool = False,
+    op: str = "set",
 ) -> Optional[ut.PandasSeries]:
     """
     Find genes by their (case-insensitive) name.
 
-    This creates a mask of all the genes whose name appears in ``names`` or matches any of the
-    ``patterns``. If ``invert`` (default: {invert}), invert the resulting mask.
+    This computes a mask of all the genes whose name appears in ``names`` or matches any of the ``patterns``. If
+    ``invert`` (default: {invert}), invert the resulting mask.
 
-    If ``to`` (default: {to}) is specified, this is stored as a per-variable (gene) annotation with
-    that name, and returns ``None``. This is useful to fill gene masks such as ``excluded_genes``
-    (genes which should be excluded from the rest of the processing) and ``forbidden_genes`` (genes
-    which must not be chosen as feature genes).
+    Depending on ``op``, this will ``set`` a (compute a brand new) mask, ``add`` the result to a mask (which must
+    exist), or ``remove`` genes from a mask (which must exist).
+
+    If ``name_property`` is specified the mask will be based on this per-variable (gene) property.
+
+    If ``to`` (default: {to}) is specified, this is stored as a per-variable (gene) annotation with that name, and
+    returns ``None``. This is useful to fill gene masks such as ``excluded_genes`` (genes which should be excluded from
+    the rest of the processing), ``lateral_genes`` (genes which must not be selected for metacell computation) and
+    ``noisy_genes`` (genes which are given more leeway when computing deviant cells).
 
     Otherwise, it returns it as a pandas series (indexed by the variable, that is gene, names).
     """
-    if names is None:
+    assert op in ("set", "add", "remove")
+    if op in ("add", "remove"):
+        assert to is not None
+        base_mask = ut.get_v_numpy(adata, to)
+    else:
+        base_mask = np.zeros(adata.n_vars, dtype="bool")
+
+    if name_property is None:
+        var_names = adata.var_names
+    else:
+        var_names = ut.get_v_numpy(adata, name_property)
+
+    if names is None or len(names) == 0:
         names_mask = np.zeros(adata.n_vars, dtype="bool")
     else:
         lower_names_set = {name.lower() for name in names}
-        names_mask = np.array([name.lower() in lower_names_set for name in adata.var_names])  #
+        names_mask = np.array([name.lower() in lower_names_set for name in var_names])  #
 
-    if patterns is None:
+    if patterns is None or len(patterns) == 0:
         patterns_mask = np.zeros(adata.n_vars, dtype="bool")
     else:
-        patterns_mask = ut.patterns_matches(patterns, adata.var_names)
+        patterns_mask = ut.patterns_matches(patterns, var_names)
 
     genes_mask = names_mask | patterns_mask
 
     if invert:
         genes_mask = ~genes_mask
 
+    if op == "add":
+        result_mask = base_mask | genes_mask
+    elif op == "remove":
+        result_mask = base_mask & ~genes_mask
+    else:
+        assert op == "set"
+        result_mask = genes_mask
+
     if to is not None:
-        ut.set_v_data(adata, to, genes_mask)
+        ut.set_v_data(adata, to, result_mask)
         return None
 
-    ut.log_return("named_genes", genes_mask)
-    return ut.to_pandas_series(genes_mask, index=adata.var_names)
+    ut.log_return("named_genes", result_mask)
+    return ut.to_pandas_series(result_mask, index=adata.var_names)
```

### Comparing `metacells-0.8.0/metacells/tools/noisy_lonely.py` & `metacells-0.9.0/metacells/tools/bursty_lonely.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,48 +14,47 @@
 from metacells.tools.downsample import downsample_cells
 from metacells.tools.filter import filter_data
 from metacells.tools.high import find_high_normalized_variance_genes
 from metacells.tools.high import find_high_total_genes
 from metacells.tools.similarity import compute_var_var_similarity
 
 __all__ = [
-    "find_noisy_lonely_genes",
+    "find_bursty_lonely_genes",
 ]
 
 
 @ut.logged()
 @ut.timed_call()
 @ut.expand_doc()
-def find_noisy_lonely_genes(  # pylint: disable=too-many-statements
+def find_bursty_lonely_genes(  # pylint: disable=too-many-statements
     adata: AnnData,
     what: Union[str, ut.Matrix] = "__x__",
     *,
-    excluded_genes_mask: Optional[str] = None,
-    max_sampled_cells: int = pr.noisy_lonely_max_sampled_cells,
-    downsample_min_samples: int = pr.noisy_lonely_downsample_min_samples,
-    downsample_min_cell_quantile: float = pr.noisy_lonely_downsample_max_cell_quantile,
-    downsample_max_cell_quantile: float = pr.noisy_lonely_downsample_min_cell_quantile,
-    min_gene_total: int = pr.noisy_lonely_min_gene_total,
-    min_gene_normalized_variance: float = pr.noisy_lonely_min_gene_normalized_variance,
-    max_gene_similarity: float = pr.noisy_lonely_max_gene_similarity,
-    random_seed: int = pr.random_seed,
+    max_sampled_cells: int = pr.bursty_lonely_max_sampled_cells,
+    downsample_min_samples: int = pr.bursty_lonely_downsample_min_samples,
+    downsample_min_cell_quantile: float = pr.bursty_lonely_downsample_max_cell_quantile,
+    downsample_max_cell_quantile: float = pr.bursty_lonely_downsample_min_cell_quantile,
+    min_gene_total: int = pr.bursty_lonely_min_gene_total,
+    min_gene_normalized_variance: float = pr.bursty_lonely_min_gene_normalized_variance,
+    max_gene_similarity: float = pr.bursty_lonely_max_gene_similarity,
     inplace: bool = True,
+    random_seed: int,
 ) -> Optional[ut.PandasSeries]:
     """
-    Detect "noisy lonely" genes based on ``what`` (default: {what}) data.
+    Detect "bursty lonely" genes based on ``what`` (default: {what}) data.
 
-    Return the indices of genes which are "noisy" (have high variance compared to their mean) and
+    Return the indices of genes which are "bursty" (have high variance compared to their mean) and
     also "lonely" (have low correlation with all other genes). Such genes should be excluded since
     they will never meaningfully help us compute groups, and will actively cause profiles to be
     considered "deviants".
 
     Noisy genes have high expression and variance. Lonely genes have no (or low) correlations with
     any other gene. Noisy lonely genes tend to throw off clustering algorithms. In general, such
     algorithms try to group together cells with the same overall biological state. Since the genes
-    are lonely, they don't contribute towards this goal. Since they are noisy, they actively hamper
+    are lonely, they don't contribute towards this goal. Since they are bursty, they actively hamper
     this, because they make cells which are otherwise similar appear different (just for this lonely
     gene).
 
     It is therefore useful to explicitly identify, in a pre-processing step, the (few) such genes,
     and exclude them from the rest of the analysis.
 
     **Input**
@@ -63,82 +62,68 @@
     Annotated ``adata``, where the observations are cells and the variables are genes, where
     ``what`` is a per-variable-per-observation matrix or the name of a per-variable-per-observation
     annotation containing such a matrix.
 
     **Returns**
 
     Variable (Gene) Annotations
-        ``noisy_lonely_genes``
-            A boolean mask indicating whether each gene was found to be a "noisy lonely" gene.
+        ``bursty_lonely_genes``
+            A boolean mask indicating whether each gene was found to be a "bursty lonely" gene.
 
     If ``inplace`` (default: {inplace}), this is written to the data, and the function returns
     ``None``. Otherwise this is returned as a pandas series (indexed by the variable names).
 
     **Computation Parameters**
 
     1. If we have more than ``max_sampled_cells`` (default: {max_sampled_cells}), pick this number
-       of random cells from the data using the ``random_seed``.
+       of random cells. Specify a non-zero random seed to make this reproducible.
 
-    2. If we were specified an ``excluded_genes_mask``, this is the name of a per-variable (gene)
-       annotation containing a mask of excluded genes. Get rid of all these excluded genes.
-
-    3. Invoke :py:func:`metacells.tools.downsample.downsample_cells` to downsample the cells to the
+    2. Invoke :py:func:`metacells.tools.downsample.downsample_cells` to downsample the cells to the
        same total number of UMIs, using the ``downsample_min_samples`` (default:
        {downsample_min_samples}), ``downsample_min_cell_quantile`` (default:
        {downsample_min_cell_quantile}), ``downsample_max_cell_quantile`` (default:
-       {downsample_max_cell_quantile}) and the ``random_seed`` (default: {random_seed}).
+       {downsample_max_cell_quantile}) and the ``random_seed``.
 
-    4. Find "noisy" genes which have a total number of UMIs of at least ``min_gene_total`` (default:
+    3. Find "bursty" genes which have a total number of UMIs of at least ``min_gene_total`` (default:
        {min_gene_total}) and a normalized variance of at least ``min_gene_normalized_variance``
        (default: ``min_gene_normalized_variance``).
 
-    5. Cross-correlate the noisy genes.
+    4. Cross-correlate the bursty genes.
 
-    6. Find the noisy "lonely" genes whose maximal correlation is at most
+    5. Find the bursty "lonely" genes whose maximal correlation is at most
        ``max_gene_similarity`` (default: {max_gene_similarity}) with all other genes.
     """
     if max_sampled_cells < adata.n_obs:
         np.random.seed(random_seed)
         cell_indices = np.random.choice(np.arange(adata.n_obs), size=max_sampled_cells, replace=False)
-        s_data = ut.slice(adata, obs=cell_indices, name=".sampled", top_level=False)
+        sdata = ut.slice(adata, obs=cell_indices, name=".sampled", top_level=False)
     else:
-        s_data = ut.copy_adata(adata, top_level=False)
+        sdata = ut.copy_adata(adata, top_level=False)
 
     track_var: Optional[str] = "sampled_gene_index"
 
-    if excluded_genes_mask is not None:
-        results = filter_data(
-            s_data, name="included", top_level=False, track_var=track_var, var_masks=[f"~{excluded_genes_mask}"]
-        )
-        track_var = None
-        assert results is not None
-        i_data = results[0]
-        assert i_data is not None
-    else:
-        i_data = s_data
-
     downsample_cells(
-        i_data,
+        sdata,
         what,
         downsample_min_samples=downsample_min_samples,
         downsample_min_cell_quantile=downsample_min_cell_quantile,
         downsample_max_cell_quantile=downsample_max_cell_quantile,
         random_seed=random_seed,
     )
 
-    find_high_total_genes(i_data, "downsampled", min_gene_total=min_gene_total)
+    find_high_total_genes(sdata, "downsampled", min_gene_total=min_gene_total)
 
     results = filter_data(
-        i_data, name="high_total", top_level=False, track_var=track_var, var_masks=["high_total_gene"]
+        sdata, name="high_total", top_level=False, track_var=track_var, var_masks=["&high_total_gene"]
     )
     track_var = None
     assert results is not None
     ht_data = results[0]
 
-    noisy_lonely_genes_mask = np.full(adata.n_vars, False)
+    bursty_lonely_genes_mask = np.full(adata.n_vars, False)
 
     if ht_data is not None:
         ht_genes_count = ht_data.shape[1]
 
         ht_gene_ht_gene_similarity_frame = compute_var_var_similarity(
             ht_data, "downsampled", inplace=False, reproducible=(random_seed != 0)
         )
@@ -163,32 +148,32 @@
             htv_gene_ht_gene_similarity_matrix = ht_gene_ht_gene_similarity_matrix[htv_mask, :]
             assert ut.is_layout(htv_gene_ht_gene_similarity_matrix, "row_major")
             assert htv_gene_ht_gene_similarity_matrix.shape == (htv_genes_count, ht_genes_count)
 
             max_similarity_of_htv_genes = ut.max_per(htv_gene_ht_gene_similarity_matrix, per="row")
             htvl_mask = max_similarity_of_htv_genes <= max_gene_similarity
             htvl_genes_count = np.sum(htvl_mask)
-            ut.log_calc("noisy_lonely_genes_count", htvl_genes_count)
+            ut.log_calc("bursty_lonely_genes_count", htvl_genes_count)
 
             if htvl_genes_count > 0:
                 base_index_of_ht_genes = ut.get_v_numpy(ht_data, "sampled_gene_index")
                 base_index_of_htv_genes = base_index_of_ht_genes[htv_mask]
                 base_index_of_htvl_genes = base_index_of_htv_genes[htvl_mask]
 
-                noisy_lonely_genes_mask[base_index_of_htvl_genes] = True
+                bursty_lonely_genes_mask[base_index_of_htvl_genes] = True
 
                 htvl_gene_ht_gene_similarity_matrix = htv_gene_ht_gene_similarity_matrix[htvl_mask, :]
                 htvl_gene_ht_gene_similarity_matrix = ut.to_layout(
                     htvl_gene_ht_gene_similarity_matrix, layout="row_major"
                 )
                 assert htvl_gene_ht_gene_similarity_matrix.shape == (htvl_genes_count, ht_genes_count)
 
                 if ut.logging_calc():
-                    i_gene_totals = ut.get_v_numpy(i_data, "downsampled", sum=True)
-                    ht_mask = ut.get_v_numpy(i_data, "high_total_gene")
+                    i_gene_totals = ut.get_v_numpy(sdata, "downsampled", sum=True)
+                    ht_mask = ut.get_v_numpy(sdata, "high_total_gene")
                     i_total = np.sum(i_gene_totals)
                     htvl_gene_totals = i_gene_totals[ht_mask][htv_mask][htvl_mask]
                     top_similarity_of_htvl_genes = ut.top_per(htvl_gene_ht_gene_similarity_matrix, 10, per="row")
                     for htvl_index, gene_index in enumerate(base_index_of_htvl_genes):
                         gene_name = adata.var_names[gene_index]
                         gene_total = htvl_gene_totals[htvl_index]
                         gene_percent = 100 * gene_total / i_total
@@ -209,15 +194,15 @@
                                         sorted(zip(top_similar_ht_values, top_similar_ht_names))
                                     )
                                 ]
                             ),
                         )
 
     if ut.logging_calc():
-        ut.log_calc("noisy_lonely_gene_names", sorted(list(adata.var_names[noisy_lonely_genes_mask])))
+        ut.log_calc("bursty_lonely_gene_names", sorted(list(adata.var_names[bursty_lonely_genes_mask])))
 
     if inplace:
-        ut.set_v_data(adata, "noisy_lonely_gene", noisy_lonely_genes_mask)
+        ut.set_v_data(adata, "bursty_lonely_gene", bursty_lonely_genes_mask)
         return None
 
-    ut.log_return("noisy_lonely_genes", noisy_lonely_genes_mask)
-    return ut.to_pandas_series(noisy_lonely_genes_mask, index=adata.var_names)
+    ut.log_return("bursty_lonely_genes", bursty_lonely_genes_mask)
+    return ut.to_pandas_series(bursty_lonely_genes_mask, index=adata.var_names)
```

### Comparing `metacells-0.8.0/metacells/tools/properly_sampled.py` & `metacells-0.9.0/metacells/tools/properly_sampled.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,29 +9,44 @@
 import numpy as np
 from anndata import AnnData  # type: ignore
 
 import metacells.parameters as pr
 import metacells.utilities as ut
 
 __all__ = [
+    "compute_excluded_gene_umis",
     "find_properly_sampled_cells",
     "find_properly_sampled_genes",
 ]
 
 
+def compute_excluded_gene_umis(
+    adata: AnnData,
+    what: Union[str, ut.Matrix] = "__x__",
+) -> None:
+    """
+    Given an ``excluded_gene`` mask, compute the total ``excluded_umis`` of each cell.
+    """
+    umis_per_gene_per_cell = ut.get_vo_proper(adata, what, layout="column_major")
+    excluded_genes_mask = ut.get_v_numpy(adata, "excluded_gene")
+    umis_per_excluded_gene_per_cell = umis_per_gene_per_cell[:, excluded_genes_mask]
+    umis_per_excluded_gene_per_cell = ut.to_layout(umis_per_excluded_gene_per_cell, layout="row_major")
+    excluded_umis_per_cell = ut.sum_per(umis_per_excluded_gene_per_cell, per="row")
+    ut.set_o_data(adata, "excluded_umis", excluded_umis_per_cell)
+
+
 @ut.logged()
 @ut.timed_call()
 @ut.expand_doc()
 def find_properly_sampled_cells(
     adata: AnnData,
     what: Union[str, ut.Matrix] = "__x__",
     *,
     min_cell_total: Optional[int],
     max_cell_total: Optional[int],
-    excluded_adata: Optional[AnnData] = None,
     max_excluded_genes_fraction: Optional[float],
     inplace: bool = True,
 ) -> Optional[ut.PandasSeries]:
     """
     Detect cells with a "proper" amount of ``what`` (default: {what}) data.
 
     Due to both technical effects and natural variance between cells, the total number of UMIs
@@ -58,40 +73,33 @@
 
     1. Exclude all cells whose total data is less than the ``min_cell_total`` (no default), unless
        it is ``None``.
 
     2. Exclude all cells whose total data is more than the ``max_cell_total`` (no default), unless
        it is ``None``.
 
-    3. If ``max_excluded_genes_fraction`` (no default) is not ``None``, then ``excluded_adata`` must
-       not be ``None`` and should contain just the excluded genes data for each cell. Exclude all
-       cells whose sum of the excluded data divided by the total data is more than the specified
-       threshold.
+    3. If ``max_excluded_genes_fraction`` (no default) is not ``None``, then exclude all cells whose sum of the excluded
+       data (as defined by the ``excluded_gene`` mask) divided by the total data is more than the specified threshold.
     """
-    assert (max_excluded_genes_fraction is None) == (excluded_adata is None)
-
-    total_of_cells = ut.get_o_numpy(adata, what, sum=True)
+    total_umis_per_cell = ut.get_o_numpy(adata, what, sum=True)
 
     cells_mask = np.full(adata.n_obs, True, dtype="bool")
 
     if min_cell_total is not None:
-        cells_mask = cells_mask & (total_of_cells >= min_cell_total)
+        cells_mask = cells_mask & (total_umis_per_cell >= min_cell_total)
 
     if max_cell_total is not None:
-        cells_mask = cells_mask & (total_of_cells <= max_cell_total)
+        cells_mask = cells_mask & (total_umis_per_cell <= max_cell_total)
 
-    if excluded_adata is not None:
-        assert max_excluded_genes_fraction is not None
-        excluded_data = ut.get_vo_proper(excluded_adata, layout="row_major")
-        excluded_of_cells = ut.sum_per(excluded_data, per="row")
-        if np.min(total_of_cells) == 0:
-            total_of_cells = np.copy(total_of_cells)
-            total_of_cells[total_of_cells == 0] = 1
-        excluded_fraction = excluded_of_cells / total_of_cells
-        cells_mask = cells_mask & (excluded_fraction <= max_excluded_genes_fraction)
+    if max_excluded_genes_fraction is not None:
+        if not ut.has_data(adata, "excluded_umis"):
+            compute_excluded_gene_umis(adata, what)
+        excluded_umis_per_cell = ut.get_o_numpy(adata, "excluded_umis")
+        excluded_umis_fraction_per_cell = excluded_umis_per_cell / total_umis_per_cell
+        cells_mask = cells_mask & (excluded_umis_fraction_per_cell <= max_excluded_genes_fraction)
 
     if inplace:
         ut.set_o_data(adata, "properly_sampled_cell", cells_mask)
         return None
 
     ut.log_return("properly_sampled_cell", cells_mask)
     return ut.to_pandas_series(cells_mask, index=adata.obs_names)
```

### Comparing `metacells-0.8.0/metacells/tools/quality.py` & `metacells-0.9.0/metacells/tools/quality.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,637 +1,355 @@
 """
 Quality
 -------
 """
 
-from typing import Any
-from typing import List
+from typing import Collection
 from typing import Optional
-from typing import Set
 from typing import Tuple
 from typing import TypeVar
 from typing import Union
 
 import numpy as np
+import scipy.sparse as sp  # type: ignore
 from anndata import AnnData  # type: ignore
-from scipy import sparse  # type: ignore
 
 import metacells.parameters as pr
 import metacells.utilities as ut
 
 __all__ = [
-    "compute_type_compatible_sizes",
-    "compute_inner_normalized_variance",
-    "compute_inner_fold_factors",
-    "compute_significant_projected_fold_factors",
+    "compute_stdev_logs",
+    "compute_projected_folds",
     "compute_similar_query_metacells",
     "compute_outliers_matches",
-    "compute_deviant_fold_factors",
-    "compute_outliers_fold_factors",
+    "compute_deviant_folds",
+    "compute_inner_folds",
     "compute_type_genes_normalized_variances",
+    "compute_outliers_fold_factors",
+    "count_significant_inner_folds",
 ]
 
 
 T = TypeVar("T")
 
 
 @ut.logged()
 @ut.timed_call()
-@ut.expand_doc()
-def compute_type_compatible_sizes(
-    adatas: List[AnnData],
-    *,
-    size: str = "grouped",
-    kind: str = "type",
-) -> None:
-    """
-    Given multiple annotated data of groups, compute a "compatible" size for each one to allow for
-    consistent inner normalized variance comparison.
-
-    Since the inner normalized variance quality measure is sensitive to the group (metacell) sizes,
-    it is useful to artificially shrink the groups so the sizes will be similar between the compared
-    data sets. Assuming each group (metacell) has a type annotation, for each such type, we give
-    each one a "compatible" size (less than or equal to its actual size) so that using this reduced
-    size will give us comparable measures between all the data sets.
-
-    The "compatible" sizes are chosen such that the density distributions of the sizes in all data
-    sets would be as similar to each other as possible.
-
-    .. note::
-
-        This is only effective if the groups are "similar" in size. Using this to compare very coarse
-        grouping (few thousands of cells) with fine-grained ones (few dozens of cells) will still
-        result in very different results.
-
-    **Input**
-
-    Several annotated ``adatas`` where each observation is a group. Should contain per-observation
-    ``size`` annotation (default: {size}) and ``kind`` annotation (default: {kind}).
-
-    **Returns**
-
-    Sets the following in each ``adata``:
-
-    Per-Observation (group) Annotations:
-
-        ``compatible_size``
-            The number of grouped cells in the group to use for computing excess R^2 and inner
-            normalized variance.
-
-    **Computation**
-
-    1. For each type, sort the groups (metacells) in increasing number of grouped observations (cells).
-
-    2. Consider the maximal quantile (rank) of the next smallest group (metacell) in each data set.
-
-    3. Compute the minimal number of grouped observations in all the metacells whose quantile is up
-       to this maximal quantile.
-
-    4. Use this as the "compatible" size for all these groups, and remove them from consideration.
-
-    5. Loop until all groups are assigned a "compatible" size.
-    """
-    assert len(adatas) > 0
-    if len(adatas) == 1:
-        ut.set_o_data(adatas[0], "compatible_size", ut.get_o_numpy(adatas[0], size, formatter=ut.sizes_description))
-        return
-
-    group_sizes_of_data = [ut.get_o_numpy(adata, size, formatter=ut.sizes_description) for adata in adatas]
-    group_types_of_data = [ut.get_o_numpy(adata, kind) for adata in adatas]
-
-    unique_types: Set[Any] = set()
-    for group_types in group_types_of_data:
-        unique_types.update(group_types)
-
-    compatible_size_of_data = [np.full(adata.n_obs, -1) for adata in adatas]
-
-    groups_count_of_data: List[int] = []
-    for type_index, group_type in enumerate(sorted(unique_types)):
-        with ut.log_step(f"- {group_type}", ut.progress_description(len(unique_types), type_index, "type")):
-            sorted_group_indices_of_data = [
-                np.argsort(group_sizes)[group_types == group_type]
-                for group_sizes, group_types in zip(group_sizes_of_data, group_types_of_data)
-            ]
-
-            groups_count_of_data = [len(sorted_group_indices) for sorted_group_indices in sorted_group_indices_of_data]
-
-            ut.log_calc("group_counts", groups_count_of_data)
-
-            def _for_each(value_of_data: List[T]) -> List[T]:
-                return [value for groups_count, value in zip(groups_count_of_data, value_of_data) if groups_count > 0]
-
-            groups_count_of_each = _for_each(groups_count_of_data)
-
-            if len(groups_count_of_each) == 0:
-                continue
-
-            sorted_group_indices_of_each = _for_each(sorted_group_indices_of_data)
-            group_sizes_of_each = _for_each(group_sizes_of_data)
-            compatible_size_of_each = _for_each(compatible_size_of_data)
-
-            if len(groups_count_of_each) == 1:
-                compatible_size_of_each[0][sorted_group_indices_of_each[0]] = group_sizes_of_each[0][
-                    sorted_group_indices_of_each[0]
-                ]
-
-            group_quantile_of_each = [
-                (np.arange(len(sorted_group_indices)) + 1) / len(sorted_group_indices)
-                for sorted_group_indices in sorted_group_indices_of_each
-            ]
-
-            next_position_of_each = np.full(len(group_quantile_of_each), 0)
-
-            while True:
-                next_quantile_of_each = [
-                    group_quantile[next_position]
-                    for group_quantile, next_position in zip(group_quantile_of_each, next_position_of_each)
-                ]
-                next_quantile = max(next_quantile_of_each)
-
-                last_position_of_each = next_position_of_each.copy()
-                next_position_of_each[:] = [
-                    np.sum(group_quantile <= next_quantile) for group_quantile in group_quantile_of_each
-                ]
-
-                positions_of_each = [
-                    range(last_position, next_position)
-                    for last_position, next_position in zip(last_position_of_each, next_position_of_each)
-                ]
-
-                sizes_of_each = [
-                    group_sizes[sorted_group_indices[positions]]
-                    for group_sizes, sorted_group_indices, positions in zip(
-                        group_sizes_of_each, sorted_group_indices_of_each, positions_of_each
-                    )
-                ]
-
-                min_size_of_each = [np.min(sizes) for sizes, positions in zip(sizes_of_each, positions_of_each)]
-                min_size = min(min_size_of_each)
-
-                for sorted_group_indices, positions, compatible_size in zip(
-                    sorted_group_indices_of_each, positions_of_each, compatible_size_of_each
-                ):
-                    compatible_size[sorted_group_indices[positions]] = min_size
-
-                is_done_of_each = [
-                    next_position == groups_count
-                    for next_position, groups_count in zip(next_position_of_each, groups_count_of_each)
-                ]
-                if all(is_done_of_each):
-                    break
-
-                assert not any(is_done_of_each)
-
-    for adata, compatible_size in zip(adatas, compatible_size_of_data):
-        assert np.min(compatible_size) > 0
-        ut.set_o_data(adata, "compatible_size", compatible_size)
-
-
-@ut.logged()
-@ut.timed_call()
-@ut.expand_doc()
-def compute_inner_normalized_variance(
+def compute_stdev_logs(
     what: Union[str, ut.Matrix] = "__x__",
     *,
-    compatible_size: Optional[str] = None,
-    downsample_min_samples: int = pr.downsample_min_samples,
-    downsample_min_cell_quantile: float = pr.downsample_min_cell_quantile,
-    downsample_max_cell_quantile: float = pr.downsample_max_cell_quantile,
     min_gene_total: int = pr.quality_min_gene_total,
     adata: AnnData,
     gdata: AnnData,
     group: Union[str, ut.Vector] = "metacell",
-    random_seed: int = pr.random_seed,
 ) -> None:
     """
-    Compute the inner normalized variance (variance / mean) for each gene in each group.
+    Compute the standard deviation of the log (base 2) of the fraction of each gene in the cells of the metacell.
 
-    This is also known as the "index of dispersion" and can serve as a quality measure for
-    the groups. An ideal group would contain only cells with "the same" biological state
-    and all remaining inner variance would be due to technical sampling noise.
+    Ideally, the standard deviation should be ~1/3rd of the ``deviants_min_gene_fold_factor`` (which is ``3`` by
+    default), indicating that (all)most cells are within that maximal fold factor. In practice we may see higher values.
 
     **Input**
 
-    Annotated ``adata``, where the observations are cells and the variables are genes, where
-    ``what`` is a per-variable-per-observation matrix or the name of a per-variable-per-observation
-    annotation containing such a matrix.
+    Annotated ``adata``, where the observations are cells and the variables are genes, where ``what`` is a
+    per-variable-per-observation (UMIs) matrix or the name of a per-variable-per-observation annotation containing such
+    a matrix.
 
-    In addition, ``gdata`` is assumed to have one observation for each group, and use the same
-    genes as ``adata``.
+    In addition, ``gdata`` is assumed to have one (fraction) observation for each metacell, a ``total_umis`` per
+    metacell, and use the same genes as ``adata``.
 
     **Returns**
 
     Sets the following in ``gdata``:
 
     Per-Variable Per-Observation (Gene-Cell) Annotations
 
-        ``inner_variance``
-            For each gene and group, the variance of the gene in the group.
-
-        ``inner_normalized_variance``
-            For each gene and group, the normalized variance (variance over mean) of the
-            gene in the group.
+        ``inner_stdev_log``
+            For each gene and metacell, the normalized variance (variance over mean) of the gene in the metacell,
+            if it has a sufficient number of UMIs to make this meaningful (otherwise, is 0).
 
     **Computation Parameters**
 
-    For each group (metacell):
-
-    1. If ``compatible_size`` (default: {compatible_size}) is specified, it should be an
-       integer per-observation annotation of the groups, whose value is at most the
-       number of grouped cells in the group. Pick a random subset of the cells of
-       this size. If ``compatible_size`` is ``None``, use all the cells of the group.
-
-    2. Invoke :py:func:`metacells.tools.downsample.downsample_cells` to downsample the surviving
-       cells to the same total number of UMIs, using the ``downsample_min_samples`` (default:
-       {downsample_min_samples}), ``downsample_min_cell_quantile`` (default:
-       {downsample_min_cell_quantile}), ``downsample_max_cell_quantile`` (default:
-       {downsample_max_cell_quantile}) and the ``random_seed`` (default: {random_seed}).
-
-    3. Compute the normalized variance of each gene based on the downsampled data. Set the
-       result to ``nan`` for genes with less than ``min_gene_total`` (default: {min_gene_total}).
-    """
-    cells_data = ut.get_vo_proper(adata, what, layout="row_major")
-
-    if compatible_size is not None:
-        compatible_size_of_groups: Optional[ut.NumpyVector] = ut.get_o_numpy(
-            gdata, compatible_size, formatter=ut.sizes_description
-        )
-    else:
-        compatible_size_of_groups = None
-
-    group_of_cells = ut.get_o_numpy(adata, group, formatter=ut.groups_description)
-
-    groups_count = np.max(group_of_cells) + 1
-    assert groups_count > 0
+    For each metacell:
 
-    assert gdata.n_obs == groups_count
-    variance_per_gene_per_group = np.full(gdata.shape, None, dtype="float32")
-    normalized_variance_per_gene_per_group = np.full(gdata.shape, None, dtype="float32")
-
-    for group_index in range(groups_count):
-        with ut.log_step(
-            "- group",
-            group_index,
-            formatter=lambda group_index: ut.progress_description(groups_count, group_index, "group"),
-        ):
-            if compatible_size_of_groups is not None:
-                compatible_size_of_group = compatible_size_of_groups[group_index]
-            else:
-                compatible_size_of_group = None
-
-            _collect_group_data(
-                group_index,
-                group_of_cells=group_of_cells,
-                cells_data=cells_data,
-                compatible_size=compatible_size_of_group,
-                downsample_min_samples=downsample_min_samples,
-                downsample_min_cell_quantile=downsample_min_cell_quantile,
-                downsample_max_cell_quantile=downsample_max_cell_quantile,
-                min_gene_total=min_gene_total,
-                random_seed=random_seed,
-                variance_per_gene_per_group=variance_per_gene_per_group,
-                normalized_variance_per_gene_per_group=normalized_variance_per_gene_per_group,
-            )
+    1. Compute the log (base 2) of the fractions of the UMIs of each gene in each cell, regularized by 1 UMI.
 
-    ut.set_vo_data(gdata, "inner_variance", variance_per_gene_per_group)
-    ut.set_vo_data(gdata, "inner_normalized_variance", normalized_variance_per_gene_per_group)
+    2. Compute the standard deviation of these logs for each gene across all cells of each metacell.
+    """
+    assert list(adata.var_names) == list(gdata.var_names)
 
+    metacell_of_cells = ut.get_o_numpy(adata, group, formatter=ut.groups_description)
+    assert gdata.n_obs == np.max(metacell_of_cells) + 1
 
-def _collect_group_data(
-    group_index: int,
-    *,
-    group_of_cells: ut.NumpyVector,
-    cells_data: ut.ProperMatrix,
-    compatible_size: Optional[int],
-    downsample_min_samples: int,
-    downsample_min_cell_quantile: float,
-    downsample_max_cell_quantile: float,
-    min_gene_total: int,
-    random_seed: int,
-    variance_per_gene_per_group: ut.NumpyMatrix,
-    normalized_variance_per_gene_per_group: ut.NumpyMatrix,
-) -> None:
-    cell_indices = np.where(group_of_cells == group_index)[0]
-    cells_count = len(cell_indices)
-    if cells_count < 2:
-        return
+    umis_per_gene_per_cell = ut.get_vo_proper(adata, what, layout="row_major")
 
-    if compatible_size is None:
-        ut.log_calc("  cells", cells_count)
-    else:
-        assert 0 < compatible_size <= cells_count
-        if compatible_size < cells_count:
-            np.random.seed(random_seed)
-            if ut.logging_calc():
-                ut.log_calc(
-                    "  cells: " + ut.ratio_description(len(cell_indices), "cell", compatible_size, "compatible")
-                )
-            cell_indices = np.random.choice(cell_indices, size=compatible_size, replace=False)
-            assert len(cell_indices) == compatible_size
-
-    assert ut.is_layout(cells_data, "row_major")
-    group_data = cells_data[cell_indices, :]
-
-    total_per_cell = ut.sum_per(group_data, per="row")
-    samples = int(
-        round(
-            min(
-                max(downsample_min_samples, np.quantile(total_per_cell, downsample_min_cell_quantile)),
-                np.quantile(total_per_cell, downsample_max_cell_quantile),
-            )
+    @ut.timed_call()
+    def _single_metacell_stdev_log(metacell_index: int) -> Tuple[ut.NumpyVector, ut.NumpyVector]:
+        return _compute_metacell_stdev_log(
+            metacell_index=metacell_index,
+            metacell_of_cells=metacell_of_cells,
+            umis_per_gene_per_cell=umis_per_gene_per_cell,
+            min_gene_total=min_gene_total,
         )
-    )
-    if ut.logging_calc():
-        ut.log_calc(f"  samples: {samples}")
-    downsampled_data = ut.downsample_matrix(group_data, per="row", samples=samples, random_seed=random_seed)
-
-    downsampled_data = ut.to_layout(downsampled_data, layout="column_major")
-    total_per_gene = ut.sum_per(downsampled_data, per="column")
-    too_small_genes = total_per_gene < min_gene_total
-    if ut.logging_calc():
-        included_genes_count = len(too_small_genes) - np.sum(too_small_genes)
-        ut.log_calc(f"  included genes: {included_genes_count}")
 
-    variance_per_gene = ut.variance_per(downsampled_data, per="column")
-    normalized_variance_per_gene = ut.normalized_variance_per(downsampled_data, per="column")
+    results = list(ut.parallel_map(_single_metacell_stdev_log, gdata.n_obs))
+    data = np.concatenate([metacell_fold_factors for _metacell_gene_indices, metacell_fold_factors in results])
+    indices = np.concatenate([metacell_gene_indices for metacell_gene_indices, _metacell_fold_factors in results])
+    indptr = np.array(
+        [0] + [len(metacell_gene_indices) for metacell_gene_indices, _metacell_fold_factors in results], dtype="int64"
+    )
+    np.cumsum(indptr, out=indptr)
 
-    variance_per_gene[too_small_genes] = None
-    normalized_variance_per_gene[too_small_genes] = None
+    assert data.dtype == "float32"
+    assert indices.dtype == "int32"
+    assert indptr.dtype == "int64"
 
-    variance_per_gene_per_group[group_index, :] = variance_per_gene
-    normalized_variance_per_gene_per_group[group_index, :] = normalized_variance_per_gene
+    inner_stdev_log_per_gene_per_metacell = sp.csr_matrix((data, indices, indptr), shape=gdata.shape)
+    inner_stdev_log_per_gene_per_metacell.has_sorted_indices = True
+    inner_stdev_log_per_gene_per_metacell.has_canonical_format = True
+    ut.set_vo_data(gdata, "inner_stdev_log", inner_stdev_log_per_gene_per_metacell)
 
 
 @ut.logged()
-@ut.timed_call()
-@ut.expand_doc()
-def compute_inner_fold_factors(
-    what: Union[str, ut.Matrix] = "__x__",
+def _compute_metacell_stdev_log(
     *,
-    adata: AnnData,
-    gdata: AnnData,
-    group: Union[str, ut.Vector] = "metacell",
-    min_gene_inner_fold_factor: float = pr.min_gene_inner_fold_factor,
-    min_entry_inner_fold_factor: float = pr.min_entry_inner_fold_factor,
-    inner_abs_folds: bool = pr.inner_abs_folds,
-) -> None:
-    """
-    Compute the inner fold factors of genes within in each metacell.
-
-    This computes, for each cell of the metacell, the same fold factors that are used to detect deviant cells (see
-    :py:func:`metacells.tools.deviants.find_deviant_cells`), and keeps the maximal fold for each gene in the metacell.
-    The result per-metacell-per-gene matrix is then made sparse by discarding too-low values (setting them to zero).
-    Ideally, this matrix should be "very" sparse. If it contains "too many" non-zero values, this indicates the
-    metacells contains "too much" variability. This may be due to actual biology (e.g. immune cells or olfactory nerves
-    which are all similar except for each one expressing one different gene), due to batch effects (similar cells in
-    distinct batches differing in some genes due to technical issues), due to low data quality (the overall noise level
-    is so high that this is simply the best the algorithm can do), or worse - a combination of the above.
-
-    **Input**
-
-    Annotated ``adata``, where the observations are cells and the variables are genes, where ``what`` is a
-    per-variable-per-observation matrix or the name of a per-variable-per-observation annotation containing such a
-    matrix.
-
-    In addition, ``gdata`` is assumed to have one observation for each group, and use the same
-    genes as ``adata``.
-
-    **Returns**
-
-    Sets the following in ``gdata``:
-
-    Per-Variable Per-Observation (Gene-Cell) Annotations
-
-        ``inner_fold``
-            For each gene and group, the maximal fold factor of this gene in any cell contained in the group (unless the
-            value is too low to be of interest, in which case it will be zero).
-
-    **Computation Parameters**
-
-    1. For each group (metacell), for each gene, compute the gene's maximal (in all the cells of the group) fold factor
-       log2((actual UMIs + 1) / (expected UMIs + 1)), similarly to
-       :py:func:`metacells.tools.deviants.find_deviant_cells`.
-
-    2. If the maximal fold factor for a gene (across all metacells) is below ``min_gene_inner_fold_factor`` (default:
-       {min_gene_inner_fold_factor}), then set all the gene's fold factors to zero (too low to be of interest). If
-       ``inner_abs_folds`` (default: {inner_abs_folds}), consider the absolute fold factors.
-
-    3. Otherwise, for any metacell whose fold factor for the gene is less than ``min_entry_inner_fold_factor`` (default:
-       {min_entry_inner_fold_factor}), set the fold factor to zero (too low to be of interest).
-    """
-    assert 0 <= min_entry_inner_fold_factor <= min_gene_inner_fold_factor
-
-    cells_data = ut.get_vo_proper(adata, what, layout="row_major")
-    metacells_data = ut.get_vo_proper(gdata, what, layout="row_major")
-    group_of_cells = ut.get_o_numpy(adata, group, formatter=ut.groups_description)
-    total_umis_per_cell = ut.sum_per(cells_data, per="row")
-    total_umis_per_metacell = ut.sum_per(metacells_data, per="row")
-
-    @ut.timed_call("compute_metacell_inner_folds")
-    def _compute_single_metacell_inner_folds(metacell_index: int) -> ut.NumpyVector:
-        return _compute_metacell_inner_folds(
-            metacell_index=metacell_index,
-            cells_data=cells_data,
-            metacells_data=metacells_data,
-            group_of_cells=group_of_cells,
-            total_umis_per_cell=total_umis_per_cell,
-            total_umis_per_metacell=total_umis_per_metacell,
-        )
+    metacell_index: int,
+    metacell_of_cells: ut.NumpyVector,
+    umis_per_gene_per_cell: ut.ProperMatrix,
+    min_gene_total: int,
+) -> Tuple[ut.NumpyVector, ut.NumpyVector]:
+    ut.log_calc("metacell_index", metacell_index)
+    cell_indices = np.where(metacell_of_cells == metacell_index)[0]
+    umis_per_gene_per_cell_by_rows = ut.to_numpy_matrix(umis_per_gene_per_cell[cell_indices, :])
+    umis_per_gene_per_cell_by_columns = ut.to_layout(umis_per_gene_per_cell_by_rows, layout="column_major")
+    umis_per_gene = ut.sum_per(umis_per_gene_per_cell_by_columns, per="column")
+    genes_mask = umis_per_gene > min_gene_total
+    ut.log_calc("genes_mask", genes_mask)
+    genes_indices = np.where(genes_mask)[0].astype("int32")
+    if len(genes_indices) == 0:
+        return (genes_indices, genes_indices.astype("float32"))
 
-    results = list(ut.parallel_map(_compute_single_metacell_inner_folds, gdata.n_obs))
-    dense_inner_folds_by_row = np.array(results)
-    dense_inner_folds_by_column = ut.to_layout(dense_inner_folds_by_row, "column_major")
-    sparse_inner_folds = ut.sparsify_matrix(
-        dense_inner_folds_by_column,
-        min_column_max_value=min_gene_inner_fold_factor,
-        min_entry_value=min_entry_inner_fold_factor,
-        abs_values=inner_abs_folds,
+    regularized_umis_per_gene_per_cell = ut.to_layout(
+        umis_per_gene_per_cell_by_rows[:, genes_indices] + 1, layout="row_major"
     )
-    ut.set_vo_data(gdata, "inner_fold", sparse_inner_folds)
+    fraction_per_gene_per_cell = ut.fraction_by(regularized_umis_per_gene_per_cell, by="row")
+    log_fraction_per_gene_per_cell = np.log2(fraction_per_gene_per_cell, out=fraction_per_gene_per_cell)  # type: ignore
+    log_fraction_per_gene_per_cell = ut.to_layout(log_fraction_per_gene_per_cell, layout="column_major")
+    stdev_per_gene = ut.stdev_per(log_fraction_per_gene_per_cell, per="column").astype("float32")
+    ut.log_calc("stdev_per_gene", stdev_per_gene, formatter=ut.sizes_description)
 
-
-@ut.logged()
-def _compute_metacell_inner_folds(
-    *,
-    metacell_index: int,
-    cells_data: ut.Matrix,
-    metacells_data: ut.Matrix,
-    group_of_cells: ut.NumpyVector,
-    total_umis_per_cell: ut.NumpyVector,
-    total_umis_per_metacell: ut.NumpyVector,
-) -> ut.NumpyVector:
-    grouped_cells_mask = group_of_cells == metacell_index
-    assert np.sum(grouped_cells_mask) > 0
-    grouped_cells_data = ut.to_numpy_matrix(cells_data[grouped_cells_mask, :])
-    total_umis_per_grouped_cell = total_umis_per_cell[grouped_cells_mask]
-    metacell_data = metacells_data[metacell_index, :]
-    total_umis_of_metacell = total_umis_per_metacell[metacell_index]
-    expected_scale_per_grouped_cell = total_umis_per_grouped_cell / total_umis_of_metacell
-    expected_cells_data = expected_scale_per_grouped_cell[:, np.newaxis] * metacell_data[np.newaxis, :]
-    assert expected_cells_data.shape == grouped_cells_data.shape
-    fold_factors_per_grouped_cell = np.log2((expected_cells_data + 1) / (grouped_cells_data + 1))
-    fold_factors = ut.max_per(ut.to_layout(fold_factors_per_grouped_cell, "column_major"), per="column")
-    max_fold_factor = np.max(fold_factors)
-    ut.log_calc("max_fold_factor", max_fold_factor)
-    return fold_factors
+    gene_indices = np.where(genes_mask)[0].astype("int32")
+    return (gene_indices, stdev_per_gene)
 
 
 @ut.logged()
 @ut.timed_call()
 @ut.expand_doc()
-def compute_significant_projected_fold_factors(
-    adata: AnnData,
-    what: Union[str, ut.Matrix] = "__x__",
-    *,
-    total_umis: Optional[ut.Vector] = None,
-    projected: Union[str, ut.Matrix] = "projected",
-    fold_normalization: float = pr.project_fold_normalization,
-    min_significant_gene_value: float = pr.project_min_significant_gene_value,
-    min_gene_fold_factor: float = pr.project_max_projection_fold_factor,
-    min_entry_fold_factor: float = pr.min_entry_project_fold_factor,
-    abs_folds: bool = pr.project_abs_folds,
+def compute_projected_folds(
+    qdata: AnnData,
+    from_query_layer: str = "corrected_fraction",
+    to_query_layer: str = "projected_fraction",
+    fold_regularization: float = pr.project_fold_regularization,
+    min_significant_gene_umis: float = pr.project_min_significant_gene_umis,
 ) -> None:
     """
-    Compute the significant projected fold factors of genes for each query metacell.
+    Compute the projected fold factors of genes for each query metacell.
 
-    This computes, for each metacell of the query, the fold factors between the actual query UMIs and the UMIs of the
-    projection of the metacell onto the atlas (see :py:func:`metacells.tools.project.project_query_onto_atlas`). The
-    result per-metacell-per-gene matrix is then made sparse by discarding too-low values (setting them to zero).
-    Ideally, this matrix should be "very" sparse. If it contains "too many" non-zero values, more genes need to
-    be ignored by the projection, or somehow corrected for batch effects prior to computing the projection.
+    This computes, for each metacell of the query, the fold factors between the corrected and projected gene fractions
+    projection of the metacell onto the atlas (see :py:func:`metacells.tools.project.compute_projection_weights`).
 
     **Input**
 
-    Annotated ``adata``, where the observations are query metacells and the variables are genes, where ``what`` is a
-    per-variable-per-observation matrix or the name of a per-variable-per-observation annotation containing such a
+    Annotated query ``qdata``, where the observations are query metacells and the variables are genes, where ``what`` is
+    a per-variable-per-observation matrix or the name of a per-variable-per-observation annotation containing such a
     matrix.
 
     In addition, the ``projected`` UMIs of each query metacells onto the atlas.
 
     **Returns**
 
-    Sets the following in ``gdata``:
+    Sets the following in ``qdata``:
 
     Per-Variable Per-Observation (Gene-Cell) Annotations
         ``projected_fold``
-            For each gene and query metacell, the fold factor of this gene between the query and its projection (unless
-            the value is too low to be of interest, in which case it will be zero).
+            For each gene and query metacell, the fold factor of this gene between the query and its projection.
 
     **Computation Parameters**
 
-    1. For each group (metacell), for each gene, compute the gene's fold factor
-       log2((actual UMIs + ``fold_normalization``) / (expected UMIs + ``fold_normalization``)), similarly to
-       :py:func:`metacells.tools.project.project_query_onto_atlas` (the default ``fold_normalization`` is
-       {fold_normalization}).
-
-    2. Set the fold factor to zero for every case where the total UMIs in the query metacell and the projected image is
-       not at least ``min_significant_gene_value`` (default: {min_significant_gene_value}).
+    1. For each group (metacell), for each gene, compute the gene's fold factor log2((``from_query_layer`` (default:
+       {from_query_layer}) + ``fold_regularization``) / (``to_query_layer`` (default: {to_query_layer}) fractions +
+       ``fold_regularization``)), similarly to :py:func:`metacells.tools.project.compute_projection_weights` (the
+       default ``fold_regularization`` is {fold_regularization}).
 
-    3. If the maximal fold factor for a gene (across all metacells) is below ``min_gene_fold_factor`` (default:
-       {min_gene_fold_factor}), then set all the gene's fold factors to zero (too low to be of interest).
-
-    4. Otherwise, for any metacell whose fold factor for the gene is less than ``min_entry_fold_factor`` (default:
-       {min_entry_fold_factor}), set the fold factor to zero (too low to be of interest). If ``abs_folds`` (default:
-       {abs_folds}), consider the absolute fold factors.
+    2. Set the fold factor to zero for every case where the total UMIs of the gene in the query metacell are not at
+       least ``min_significant_gene_umis`` (default: {min_significant_gene_umis}).
     """
-    assert 0 <= min_entry_fold_factor <= min_gene_fold_factor
-    assert fold_normalization >= 0
+    assert fold_regularization >= 0
 
-    metacells_data = ut.get_vo_proper(adata, what, layout="row_major")
-    projected_data = ut.get_vo_proper(adata, projected, layout="row_major")
+    corrected_fractions = ut.get_vo_proper(qdata, from_query_layer, layout="row_major")
+    projected_fractions = ut.get_vo_proper(qdata, to_query_layer, layout="row_major")
 
-    metacells_fractions = ut.fraction_by(metacells_data, by="row", sums=total_umis)
-    projected_fractions = ut.fraction_by(projected_data, by="row", sums=total_umis)
+    corrected_fractions = ut.to_numpy_matrix(corrected_fractions, copy=True)
+    projected_fractions = ut.to_numpy_matrix(projected_fractions, copy=True)
 
-    metacells_fractions += fold_normalization  # type: ignore
-    projected_fractions += fold_normalization  # type: ignore
+    corrected_fractions += fold_regularization
+    projected_fractions += fold_regularization
 
-    dense_folds = metacells_fractions / projected_fractions  # type: ignore
-    dense_folds = np.log2(dense_folds, out=dense_folds)
+    dense_folds = np.log2(corrected_fractions) - np.log2(projected_fractions)
 
-    total_umis = ut.to_numpy_matrix(metacells_data + projected_data)  # type: ignore
-    insignificant_folds_mask = total_umis < min_significant_gene_value
-    ut.log_calc("insignificant entries", insignificant_folds_mask)
-    dense_folds[insignificant_folds_mask] = 0.0
-    dense_folds_by_column = ut.to_layout(dense_folds, layout="column_major")
-    sparse_folds = ut.sparsify_matrix(
-        dense_folds_by_column,
-        min_column_max_value=min_gene_fold_factor,
-        min_entry_value=min_entry_fold_factor,
-        abs_values=abs_folds,
-    )
+    total_umis = ut.to_numpy_matrix(ut.get_vo_proper(qdata, "total_umis", layout="row_major"))
+    insignificant_folds_mask = total_umis < min_significant_gene_umis
+    ut.log_calc("insignificant folds mask", insignificant_folds_mask)
 
-    ut.set_vo_data(adata, "projected_fold", sparse_folds)
+    dense_folds[insignificant_folds_mask] = 0.0
+    sparse_folds = sp.csr_matrix(dense_folds)
+    sparse_folds.has_sorted_indices = True
+    sparse_folds.has_canonical_format = True
+    ut.set_vo_data(qdata, "projected_fold", sparse_folds)
 
 
 @ut.logged()
 @ut.timed_call()
-def compute_similar_query_metacells(
-    adata: AnnData,
+def compute_similar_query_metacells(  # pylint: disable=too-many-statements
+    qdata: AnnData,
     max_projection_fold_factor: float = pr.project_max_projection_fold_factor,
-    max_dissimilar_genes: int = pr.project_max_dissimilar_genes,
-    abs_folds: bool = pr.project_abs_folds,
+    max_projection_noisy_fold_factor: float = pr.project_max_projection_noisy_fold_factor,
+    min_fitted_query_marker_genes: float = 0,
+    max_misfit_genes: int = pr.project_max_misfit_genes,
+    essential_genes_property: Union[None, str, Collection[str]] = None,
+    min_essential_genes: Optional[int] = None,
+    fitted_genes_mask: Optional[ut.NumpyVector] = None,
 ) -> None:
     """
-    Mark query metacells that are similar to their projection on the atlas.
+    Mark query metacells that are "similar" to their projection on the atlas.
 
     This does not guarantee the query metacell is "the same as" its projection on the atlas; rather, it means the two
-    are sufficiently similar that one can be "reasonably confident" in applying atlas metadata to the query metacell
-    based on the projection, which is a much lower bar.
+    are "sufficiently similar" that one can be reasonably confident in applying atlas metadata to the query metacell
+    based on the projection.
 
     **Input**
 
-    Annotated query ``adata``, where the observations are cells and the variables are genes, where ``what`` is a
-    per-variable-per-observation matrix or the name of a per-variable-per-observation annotation containing such a
-    matrix.
+    Annotated query ``qdata``, where the observations are metacells and the variables are genes.
 
     The data should contain per-observation-per-variable annotations ``projected_fold`` with the significant projection
-    folds factors, as computed by :py:func:`compute_significant_projected_fold_factors`.
+    folds factors, as computed by :py:func:`compute_projected_folds`. If ``min_essential_significant_genes_fraction``,
+    and ``essential_genes_property`` are specified, then the data may contain additional per-observation (gene) mask(s)
+    denoting the essential genes.
+
+    If a ``projected_noisy_gene`` mask exists, then the genes in it allow for a higher fold factor than normal genes.
 
     **Returns**
 
-    Sets the following in ``adata``:
+    Sets the following in ``qdata``:
 
     Per-Observation (Cell) Annotations
 
         ``similar``
             A boolean mask indicating the query metacell is similar to its projection in the atlas.
-        ``dissimilar_genes_count``
-            The number of genes whose fold factor is above the threshold.
+
+    Per-Variable Per-Observation (Gene-Cell) Annotations
+        ``misfit``
+            Whether the gene has a too-high fold factor between the query and its projection in the atlas.
 
     **Computation Parameters**
 
-    1. Mark as dissimilar any query metacells which have more than ``max_dissimilar_genes`` (default:
-       {max_dissimilar_genes}) genes whose projection fold is above ``max_projection_fold_factor``.
+    1. If ``fitted_genes_mask`` is not ``None``, restrict the analysis to the genes listed in it.
+
+    2. Mark as dissimilar any query metacells which have more than ``max_misfit_genes`` (default:
+       {max_misfit_genes}) genes whose projection fold is above ``max_projection_fold_factor``,
+       or, for genes in ``projected_noisy_gene``, above an additional ``max_projection_noisy_fold_factor``.
+
+    3. Mark as dissimilar any query metacells which did not fit at least ``min_fitted_query_marker_genes`` of the
+       query marker genes.
+
+    4. If ``essential_genes_property`` and ``min_essential_genes`` are specified, the former should be the name(s) of
+       boolean per-gene property/ies, and we will mark as dissimilar any query metacells which have at least this number
+       of essential genes with a low projection fold factor.
     """
     assert max_projection_fold_factor >= 0
-    assert max_dissimilar_genes >= 0
+    assert max_projection_noisy_fold_factor >= 0
+    assert max_misfit_genes >= 0
+
+    projected_fold_per_gene_per_metacell = ut.get_vo_proper(qdata, "projected_fold", layout="row_major")
+    projected_fold_per_gene_per_metacell = np.abs(projected_fold_per_gene_per_metacell)  # type: ignore
+
+    if ut.has_data(qdata, "projected_noisy_gene"):
+        max_projection_fold_factor_per_gene = np.full(qdata.n_vars, max_projection_fold_factor, dtype="float32")
+        noisy_per_gene = ut.get_v_numpy(qdata, "projected_noisy_gene")
+        max_projection_fold_factor_per_gene[noisy_per_gene] += max_projection_noisy_fold_factor
+        misfit_per_gene_per_metacell_proper = (
+            projected_fold_per_gene_per_metacell > max_projection_fold_factor_per_gene[np.newaxis, :]
+        )
+    else:
+        misfit_per_gene_per_metacell_proper = projected_fold_per_gene_per_metacell > max_projection_fold_factor
+    misfit_per_gene_per_metacell = sp.csr_matrix(misfit_per_gene_per_metacell_proper)
+    misfit_per_gene_per_metacell.has_sorted_indices = True
+    misfit_per_gene_per_metacell.has_canonical_format = True
+    ut.set_vo_data(qdata, "misfit", misfit_per_gene_per_metacell)
 
-    projected_folds = ut.get_vo_proper(adata, "projected_fold", layout="row_major")
-    if abs_folds:
-        projected_folds = np.abs(projected_folds)  # type: ignore
-    high_folds = projected_folds > max_projection_fold_factor  # type: ignore
-    high_folds_per_metacell = ut.sum_per(high_folds, per="row")  # type: ignore
-    similar_mask = high_folds_per_metacell <= max_dissimilar_genes
-    ut.log_calc("max dissimilar_genes_count", np.max(high_folds_per_metacell))
-    ut.set_o_data(adata, "dissimilar_genes_count", high_folds_per_metacell, formatter=ut.mask_description)
-    ut.set_o_data(adata, "similar", similar_mask)
+    if fitted_genes_mask is None:
+        misfit_per_fitted_gene_per_metacell = misfit_per_gene_per_metacell
+    else:
+        misfit_per_fitted_gene_per_metacell = misfit_per_gene_per_metacell[:, fitted_genes_mask]
+
+    misfit_per_metacell = ut.sum_per(misfit_per_fitted_gene_per_metacell, per="row")
+    ut.log_calc("misfit_per_metacell", misfit_per_metacell, formatter=ut.sizes_description)
+
+    similar_mask = misfit_per_metacell <= max_misfit_genes
+    ut.log_calc("similar_mask", similar_mask)
+
+    query_marker_genes_mask = ut.get_v_numpy(qdata, "marker_gene")
+    if fitted_genes_mask is not None:
+        fitted_query_marker_genes_mask = query_marker_genes_mask & fitted_genes_mask
+        ut.log_calc("fitted_query_marker_genes_mask", fitted_query_marker_genes_mask)
+    else:
+        fitted_query_marker_genes_mask = query_marker_genes_mask
+    fitted_query_marker_genes = np.sum(fitted_query_marker_genes_mask)
+    ut.log_calc("fitted_query_marker_genes", fitted_query_marker_genes)
+    if fitted_query_marker_genes < min_fitted_query_marker_genes:
+        similar_mask[:] = False
+        ut.log_calc("similar_mask", similar_mask)
+
+    if essential_genes_property is not None and min_essential_genes is not None:
+        essential_genes_mask = np.zeros(qdata.n_vars, dtype="bool")
+        if isinstance(essential_genes_property, str):
+            essential_genes_property = [essential_genes_property]
+        for property_name in essential_genes_property:
+            essential_genes_mask |= ut.get_v_numpy(qdata, property_name)
+
+        ut.log_calc("essential_genes_mask", essential_genes_mask)
+        essential_genes_count = np.sum(essential_genes_mask)
+        if essential_genes_count > 0:
+            ut.log_calc("essential_gene_names", qdata.var_names[essential_genes_mask])
+            misfit_per_essential_gene_per_metacell = misfit_per_gene_per_metacell[:, essential_genes_mask]
+            misfit_essential_per_metacell = ut.sum_per(misfit_per_essential_gene_per_metacell, per="row")
+            fitted_essential_per_metacell = essential_genes_count - misfit_essential_per_metacell
+        else:
+            fitted_essential_per_metacell = np.zeros(len(misfit_per_metacell), dtype="bool")
+
+        ut.log_calc("fitted_essential_per_metacell", fitted_essential_per_metacell, formatter=ut.sizes_description)
+        essential_similar_mask = fitted_essential_per_metacell >= min_essential_genes
+        ut.log_calc("essential_similar_mask", essential_similar_mask)
+
+        similar_mask &= essential_similar_mask
+
+    ut.set_o_data(qdata, "similar", similar_mask)
 
 
 @ut.logged()
 @ut.timed_call()
 @ut.expand_doc()
 def compute_outliers_matches(
     what: Union[str, ut.Matrix] = "__x__",
     *,
     adata: AnnData,
     gdata: AnnData,
     group: Union[str, ut.Vector] = "metacell",
     most_similar: str = "most_similar",
-    value_normalization: float = pr.outliers_fold_normalization,
+    value_regularization: float = pr.outliers_fold_regularization,
     reproducible: bool,
 ) -> None:
     """
     Given an assignment of observations (cells) to groups (metacells), compute for each outlier the "most similar"
     group.
 
     **Input**
@@ -653,61 +371,65 @@
 
         ``most_similar`` (default: {most_similar})
             For each observation (cell), the index of the "most similar" group.
 
     **Computation Parameters**
 
     1. Compute the log2 of the fraction of each gene in each of the outlier cells and the group metacells using
-       the ``value_normalization`` (default: {value_normalization}).
+       the ``value_regularization`` (default: {value_regularization}).
 
     2. Cross-correlate each of the outlier cells with each of the group metacells, in a ``reproducible`` manner.
     """
     assert list(adata.var_names) == list(gdata.var_names)
+    cells_similar_metacell_indices = np.full(adata.n_obs, -1, dtype="int32")
+
+    metacell_per_cell = ut.get_o_numpy(adata, group)
+    outliers_mask = metacell_per_cell < 0
+    if not np.any(outliers_mask):
+        ut.set_o_data(adata, most_similar, cells_similar_metacell_indices)
+        return
 
-    group_of_cells = ut.get_o_numpy(adata, group)
-    outliers_mask = group_of_cells < 0
     odata = ut.slice(adata, obs=outliers_mask)
 
     outliers_data = ut.get_vo_proper(odata, what, layout="row_major")
-    groups_data = ut.get_vo_proper(gdata, what, layout="row_major")
+    metacells_data = ut.get_vo_proper(gdata, what, layout="row_major")
 
     outliers_fractions = ut.fraction_by(outliers_data, by="row")
-    groups_fractions = ut.fraction_by(groups_data, by="row")
+    metacells_fractions = ut.fraction_by(metacells_data, by="row")
 
     outliers_fractions = ut.to_numpy_matrix(outliers_fractions)
-    groups_fractions = ut.to_numpy_matrix(groups_fractions)
+    metacells_fractions = ut.to_numpy_matrix(metacells_fractions)
 
-    outliers_fractions += value_normalization
-    groups_fractions += value_normalization
+    outliers_fractions += value_regularization
+    metacells_fractions += value_regularization
 
     outliers_log_fractions = np.log2(outliers_fractions, out=outliers_fractions)
-    groups_log_fractions = np.log2(groups_fractions, out=groups_fractions)
+    metacells_log_fractions = np.log2(metacells_fractions, out=metacells_fractions)
 
-    outliers_groups_correlation = ut.cross_corrcoef_rows(
-        outliers_log_fractions, groups_log_fractions, reproducible=reproducible
+    outliers_metacells_correlation = ut.cross_corrcoef_rows(
+        outliers_log_fractions, metacells_log_fractions, reproducible=reproducible
     )
-    outliers_similar_group_indices = np.argmax(outliers_groups_correlation, axis=1)
-    assert len(outliers_similar_group_indices) == odata.n_obs
+    outliers_similar_metacell_indices = np.argmax(outliers_metacells_correlation, axis=1)
+    assert len(outliers_similar_metacell_indices) == odata.n_obs
 
-    cells_similar_group_indices = np.full(adata.n_obs, -1, dtype="int32")
-    cells_similar_group_indices[outliers_mask] = outliers_similar_group_indices
-    ut.set_o_data(adata, most_similar, cells_similar_group_indices)
+    cells_similar_metacell_indices[outliers_mask] = outliers_similar_metacell_indices
+    ut.set_o_data(adata, most_similar, cells_similar_metacell_indices)
 
 
 @ut.logged()
 @ut.timed_call()
 @ut.expand_doc()
-def compute_deviant_fold_factors(
+def compute_deviant_folds(
     what: Union[str, ut.Matrix] = "__x__",
     *,
     adata: AnnData,
     gdata: AnnData,
     group: Union[str, ut.Vector] = "metacell",
-    most_similar: Union[str, ut.Vector] = "most_similar",
-    significant_gene_fold_factor: float = pr.significant_gene_fold_factor,
+    most_similar: Union[str, ut.Vector, None] = "most_similar",
+    min_gene_total: int = pr.quality_min_gene_total,
 ) -> None:
     """
     Given an assignment of observations (cells) to groups (metacells) or, if an outlier, to the most similar groups,
     compute for each observation and gene the fold factor relative to its group for the purpose of detecting deviant
     cells.
 
     Ideally, all grouped cells would have no genes with high enough fold factors to be considered deviants, and all
@@ -734,170 +456,171 @@
         ``deviant_fold``
             The fold factor between the cell's UMIs and the expected number of UMIs for the purpose of computing
             deviant cells.
 
     **Computation Parameters**
 
     1. For each cell, compute the expected UMIs for each gene given the fraction of the gene in the metacells associated
-       with the cell (the one it is belongs to, or the most similar one for outliers). If this is less than
-       ``significant_gene_fold_factor`` (default: {significant_gene_fold_factor}), set it to zero so the result will be
-       sparse.
-    """
-    cells_data = ut.get_vo_proper(adata, what, layout="row_major")
-    metacells_data = ut.get_vo_proper(gdata, what, layout="row_major")
-    total_umis_per_cell = ut.sum_per(cells_data, per="row")
-    total_umis_per_metacell = ut.sum_per(metacells_data, per="row")
+       with the cell (the one it is belongs to, or the most similar one for outliers).
 
-    group_of_cells = ut.get_o_numpy(adata, group, formatter=ut.groups_description)
-    most_similar_of_cells = ut.get_o_numpy(adata, most_similar, formatter=ut.groups_description)
+    2. If the number of UMIs in the metacell (for grouped cells), or sum of the UMIs of the gene in an outlier cell and
+       the metacell, is less than ``min_gene_total`` (default: {min_gene_total}), set the fold factor to 0 as we do not
+       have sufficient data to robustly estimate it.
+    """
+    umis_per_gene_per_cell = ut.get_vo_proper(adata, what, layout="row_major")
+    fraction_per_gene_per_metacell = ut.get_vo_proper(gdata, what, layout="row_major")
+    umis_per_gene_per_metacell = ut.get_vo_proper(gdata, "total_umis", layout="row_major")
+
+    metacell_per_cell = ut.get_o_numpy(adata, group, formatter=ut.groups_description)
+    combined_per_cell = metacell_per_cell.copy()
+    outliers_mask: Optional[ut.NumpyVector] = None
+    if most_similar is not None:
+        most_similar_per_cell = ut.get_o_numpy(adata, most_similar, formatter=ut.groups_description)
+        outliers_mask = metacell_per_cell < 0
+        assert outliers_mask is not None
+        assert np.all(most_similar_per_cell[outliers_mask] >= 0)
+        assert np.all(most_similar_per_cell[~outliers_mask] < 0)
+        combined_per_cell[outliers_mask] = most_similar_per_cell[outliers_mask]
 
-    @ut.timed_call("compute_cell_deviant_certificates")
-    def _compute_cell_deviant_certificates(cell_index: int) -> Tuple[ut.NumpyVector, ut.NumpyVector]:
-        return _compute_cell_certificates(
+    @ut.timed_call()
+    def _single_cell_deviant_folds(cell_index: int) -> Tuple[ut.NumpyVector, ut.NumpyVector]:
+        return _compute_cell_deviant_folds(
             cell_index=cell_index,
-            cells_data=cells_data,
-            metacells_data=metacells_data,
-            group_of_cells=group_of_cells,
-            most_similar_of_cells=most_similar_of_cells,
-            total_umis_per_cell=total_umis_per_cell,
-            total_umis_per_metacell=total_umis_per_metacell,
-            significant_gene_fold_factor=significant_gene_fold_factor,
+            umis_per_gene_per_cell=umis_per_gene_per_cell,
+            fraction_per_gene_per_metacell=fraction_per_gene_per_metacell,
+            umis_per_gene_per_metacell=umis_per_gene_per_metacell,
+            outliers_mask=outliers_mask,
+            metacell_per_cell=combined_per_cell,
+            min_gene_total=min_gene_total,
         )
 
-    results = list(ut.parallel_map(_compute_cell_deviant_certificates, adata.n_obs))
-
-    cell_indices = np.concatenate(
-        [np.full(len(result[0]), cell_index, dtype="int32") for cell_index, result in enumerate(results)]
+    results = list(ut.parallel_map(_single_cell_deviant_folds, adata.n_obs))
+    data = np.concatenate([cell_fold_factors for _cell_gene_indices, cell_fold_factors in results])
+    indices = np.concatenate([cell_gene_indices for cell_gene_indices, _cell_fold_factors in results])
+    indptr = np.array(
+        [0] + [len(cell_gene_indices) for cell_gene_indices, _cell_fold_factors in results], dtype="int64"
     )
-    gene_indices = np.concatenate([result[0] for result in results])
-    fold_factors = np.concatenate([result[1] for result in results])
+    np.cumsum(indptr, out=indptr)
+
+    assert data.dtype == "float32"
+    assert indices.dtype == "int32"
+    assert indptr.dtype == "int64"
 
-    deviant_folds = sparse.csr_matrix((fold_factors, (cell_indices, gene_indices)), shape=adata.shape)
-    ut.set_vo_data(adata, "deviant_folds", deviant_folds)
+    fold_factors_per_gene_per_cell = sp.csr_matrix((data, indices, indptr), shape=adata.shape)
+    fold_factors_per_gene_per_cell.has_sorted_indices = True
+    fold_factors_per_gene_per_cell.has_canonical_format = True
+    ut.set_vo_data(adata, "deviant_fold", fold_factors_per_gene_per_cell)
 
 
 @ut.logged()
-def _compute_cell_certificates(
+def _compute_cell_deviant_folds(
     *,
     cell_index: int,
-    cells_data: ut.Matrix,
-    metacells_data: ut.Matrix,
-    group_of_cells: ut.NumpyVector,
-    most_similar_of_cells: ut.NumpyVector,
-    total_umis_per_cell: ut.NumpyVector,
-    total_umis_per_metacell: ut.NumpyVector,
-    significant_gene_fold_factor: float,
+    umis_per_gene_per_cell: ut.Matrix,
+    fraction_per_gene_per_metacell: ut.Matrix,
+    umis_per_gene_per_metacell: ut.Matrix,
+    metacell_per_cell: ut.NumpyVector,
+    outliers_mask: Optional[ut.NumpyVector],
+    min_gene_total: int,
 ) -> Tuple[ut.NumpyVector, ut.NumpyVector]:
-    group_index = group_of_cells[cell_index]
-    most_similar_index = most_similar_of_cells[cell_index]
-    assert (group_index < 0) != (most_similar_index < 0)
-    metacell_index = max(group_index, most_similar_index)
-
-    expected_scale = total_umis_per_cell[cell_index] / total_umis_per_metacell[metacell_index]
-    expected_data = ut.to_numpy_vector(metacells_data[metacell_index, :], copy=True)
-    expected_data *= expected_scale
-
-    actual_data = ut.to_numpy_vector(cells_data[cell_index, :], copy=True)
-
-    expected_data += 1.0
-    actual_data += 1.0
-
-    fold_factors = actual_data
-    fold_factors /= expected_data
-    fold_factors = np.log2(fold_factors, out=fold_factors)
-    fold_factors = np.abs(fold_factors, out=fold_factors)
-
-    significant_folds_mask = fold_factors >= significant_gene_fold_factor
-    ut.log_calc("significant_folds_mask", significant_folds_mask)
-
-    significant_gene_indices = np.where(significant_folds_mask)[0].astype("int32")
-    significant_gene_folds = fold_factors[significant_folds_mask].astype("float32")
-    return (significant_gene_indices, significant_gene_folds)
+    actual_umis_per_gene = ut.to_numpy_vector(umis_per_gene_per_cell[cell_index, :], copy=True)
+    total_umis_of_cell = np.sum(actual_umis_per_gene)
+
+    metacell_index = metacell_per_cell[cell_index]
+    metacell_fraction_per_gene = ut.to_numpy_vector(fraction_per_gene_per_metacell[metacell_index, :])
+    expected_umis_per_gene = total_umis_of_cell * metacell_fraction_per_gene
+
+    actual_umis_per_gene += 1
+    expected_umis_per_gene += 1
+    fold_factors = np.log2(actual_umis_per_gene) - np.log2(expected_umis_per_gene)
+
+    metacell_umis_per_gene = ut.to_numpy_vector(umis_per_gene_per_metacell[metacell_index, :])
+    if outliers_mask is not None and outliers_mask[cell_index]:
+        total_umis_per_gene = actual_umis_per_gene + metacell_umis_per_gene
+    else:
+        total_umis_per_gene = metacell_umis_per_gene
+
+    gene_indices = np.where(total_umis_per_gene >= min_gene_total)[0].astype("int32")
+    ut.log_calc("nnz_fold_genes_count", len(gene_indices))
+    return (gene_indices.astype("int32"), fold_factors[gene_indices].astype("float32"))
 
 
 @ut.logged()
 @ut.timed_call()
-@ut.expand_doc()
-def compute_outliers_fold_factors(
-    what: Union[str, ut.Matrix] = "__x__",
+def compute_inner_folds(
     *,
     adata: AnnData,
     gdata: AnnData,
-    most_similar: Union[str, ut.Vector] = "most_similar",
-    fold_normalization: float = pr.outliers_fold_normalization,
-    min_gene_outliers_fold_factor: float = pr.min_gene_outliers_fold_factor,
-    min_entry_outliers_fold_factor: float = pr.min_entry_outliers_fold_factor,
-    abs_folds: bool = pr.outliers_abs_folds,
+    group: Union[str, ut.Vector] = "metacell",
 ) -> None:
     """
-    Given annotated data which is a slice containing just the outliers, where each has a "most similar" group, compute
-    for each observation and gene the fold factor relative to its group.
-
-    All outliers should have at least one (typically several) genes with high fold factors, which are the reason they
-    couldn't be merged into their most similar group.
-
-    **Input**
-
-    Annotated ``adata``, where the observations are outlier cells and the variables are genes, where ``what`` is a
-    per-variable-per-observation matrix or the name of a per-variable-per-observation annotation containing such a
-    matrix.
-
-    In addition, ``gdata`` is assumed to have one observation for each group, and use the same genes as ``adata``.
-    It should have a ``significant_gene`` mask.
-
-    **Returns**
-
-    Sets the following in ``adata``:
-
-    Per-Variable Per-Observation (Gene-Cell) Annotations
+    Given ``adata`` with computed ``deviant_fold`` for each gene for each cell, set in ``inner_fold`` in ``gdata``, for
+    each gene for each metacell the ``deviant_fold`` with the maximal absolute value.
+    """
+    group_per_cell = ut.get_o_numpy(adata, group)
+    deviant_fold_per_gene_per_cell = ut.get_vo_proper(adata, "deviant_fold")
 
-        ``<most_similar>_fold`` (default: {most_similar}_fold)
-            The fold factor between the outlier gene expression and their expression in the most similar group, (unless
-            the value is too low to be of interest, in which case it will be zero).
+    @ut.timed_call()
+    def _single_metacell_inner_folds(metacell_index: int) -> Tuple[ut.NumpyVector, ut.NumpyVector]:
+        return _compute_metacell_inner_folds(
+            metacell_index=metacell_index,
+            group_per_cell=group_per_cell,
+            deviant_fold_per_gene_per_cell=deviant_fold_per_gene_per_cell,
+        )
 
-    **Computation Parameters**
+    results = list(ut.parallel_map(_single_metacell_inner_folds, gdata.n_obs))
 
-    1. For each outlier, compute the expected UMIs for each gene given the fraction of the gene in the metacell
-       associated with the outlier by the ``most_similar`` (default: {most_similar}). If this is less than
-       ``min_entry_outliers_fold_factor`` (default: {min_entry_outliers_fold_factor}), or if the gene doesn't
-       have a fold factor of at least ``min_gene_outliers_fold_factor`` (default: {min_gene_outliers_fold_factor})
-       in any outlier, this is set to zero to make the matrix sparse. Also, all columns for genes not listed
-       in the ``significant_gene`` mask are also set to zero.
-    """
-    assert list(adata.var_names) == list(gdata.var_names)
+    data = np.concatenate([metacell_fold_factors for _metacell_gene_indices, metacell_fold_factors in results])
+    indices = np.concatenate([metacell_gene_indices for metacell_gene_indices, _metacell_fold_factors in results])
+    assert len(data) == len(indices)
+    indptr = np.array(
+        [0] + [len(metacell_gene_indices) for metacell_gene_indices, _metacell_fold_factors in results], dtype="int64"
+    )
+    np.cumsum(indptr, out=indptr)
 
-    most_similar_of_outliers = ut.get_o_numpy(adata, most_similar, formatter=ut.groups_description)
-    assert np.min(most_similar_of_outliers) >= 0
+    assert data.dtype == "float32"
+    assert indices.dtype == "int32"
+    assert indptr.dtype == "int64"
+
+    fold_factors_per_gene_per_metacell = sp.csr_matrix((data, indices, indptr), shape=gdata.shape)
+    fold_factors_per_gene_per_metacell.has_sorted_indices = True
+    fold_factors_per_gene_per_metacell.has_canonical_format = True
+    ut.set_vo_data(gdata, "inner_fold", fold_factors_per_gene_per_metacell)
 
-    outliers_data = ut.to_numpy_matrix(ut.get_vo_proper(adata, what, layout="row_major"))
-    groups_data = ut.to_numpy_matrix(ut.get_vo_proper(gdata, what, layout="row_major"))
-    most_similar_data = groups_data[most_similar_of_outliers, :]
 
-    outliers_fractions = ut.fraction_by(outliers_data, by="row")
-    most_similar_fractions = ut.fraction_by(most_similar_data, by="row")
+@ut.logged()
+def _compute_metacell_inner_folds(
+    *,
+    metacell_index: int,
+    group_per_cell: ut.NumpyVector,
+    deviant_fold_per_gene_per_cell: ut.ProperMatrix,
+) -> Tuple[ut.NumpyVector, ut.NumpyVector]:
+    cells_mask = group_per_cell == metacell_index
+    cells_count = np.sum(cells_mask)
+    assert cells_count > 0
+    genes_count = deviant_fold_per_gene_per_cell.shape[1]
 
-    outliers_fractions += fold_normalization  # type: ignore
-    most_similar_fractions += fold_normalization  # type: ignore
+    tmp_deviant_fold_per_gene_per_cell = ut.to_numpy_matrix(deviant_fold_per_gene_per_cell[cells_mask, :], copy=True)
+    tmp_deviant_fold_per_gene_per_cell = ut.to_layout(tmp_deviant_fold_per_gene_per_cell, layout="column_major")
+    assert tmp_deviant_fold_per_gene_per_cell.shape == (cells_count, genes_count)
 
-    outliers_log_fractions = np.log2(outliers_fractions, out=outliers_fractions)  # type: ignore
-    most_similar_log_fractions = np.log2(most_similar_fractions, out=most_similar_fractions)  # type: ignore
+    negative_folds_mask = tmp_deviant_fold_per_gene_per_cell < 0
+    tmp_deviant_fold_per_gene_per_cell[negative_folds_mask] *= -1
 
-    fold_factors = ut.to_layout(outliers_log_fractions - most_similar_log_fractions, layout="column_major")
+    max_index_per_gene = np.argmax(tmp_deviant_fold_per_gene_per_cell, axis=0)
+    assert len(max_index_per_gene) == genes_count
 
-    significant_gene_mask = ut.get_v_numpy(gdata, "significant_gene")
-    fold_factors[:, ~significant_gene_mask] = 0
+    tmp_deviant_fold_per_gene_per_cell[negative_folds_mask] *= -1
 
-    sparse_folds = ut.sparsify_matrix(
-        fold_factors,
-        min_column_max_value=min_gene_outliers_fold_factor,
-        min_entry_value=min_entry_outliers_fold_factor,
-        abs_values=abs_folds,
-    )
+    max_deviant_fold_per_gene = tmp_deviant_fold_per_gene_per_cell[max_index_per_gene, range(genes_count)]
+    assert len(max_deviant_fold_per_gene) == genes_count
 
-    ut.set_vo_data(adata, f"{most_similar}_fold", sparse_folds)
+    gene_indices = np.where(max_deviant_fold_per_gene != 0.0)[0].astype("int32")
+    ut.log_calc("nnz_fold_genes_count", len(gene_indices))
+    return (gene_indices.astype("int32"), max_deviant_fold_per_gene[gene_indices].astype("float32"))
 
 
 @ut.logged()
 @ut.timed_call()
 @ut.expand_doc()
 def compute_type_genes_normalized_variances(
     what: Union[str, ut.Matrix] = "__x__",
@@ -943,15 +666,15 @@
     """
     assert list(adata.var_names) == list(gdata.var_names)
 
     type_of_metacell = ut.get_o_numpy(gdata, type_property)
     unique_types = np.unique(type_of_metacell)
     ut.log_calc("types_count", len(unique_types))
 
-    metacell_of_cells = ut.get_o_numpy(adata, group_property)
+    metacell_per_cell = ut.get_o_numpy(adata, group_property)
     cells_umis = ut.get_vo_proper(adata, what, layout="row_major")
 
     @ut.logged()
     @ut.timed_call()
     def _compute_single_type_genes_normalized_variances(type_index: int) -> Tuple[str, ut.NumpyVector]:
         type_name = unique_types[type_index]
         ut.log_calc("type_name", type_name)
@@ -959,47 +682,155 @@
         ut.log_calc("type_metacells_count", len(type_metacells_indices))
         type_gene_normalized_variances_per_metacell = np.empty(
             (len(type_metacells_indices), adata.n_vars), dtype="float32"
         )
 
         for position, metacell_index in enumerate(type_metacells_indices):
             _compute_metacell_genes_normalized_variances(
-                metacell_of_cells=metacell_of_cells,
+                metacell_per_cell=metacell_per_cell,
                 cells_umis=cells_umis,
                 position=position,
                 metacell_index=metacell_index,
                 type_gene_normalized_variances_per_metacell=type_gene_normalized_variances_per_metacell,
             )
 
         type_gene_normalized_variances_per_metacell = ut.to_layout(
             type_gene_normalized_variances_per_metacell, layout="column_major"
         )
         return type_name, ut.quantile_per(
             type_gene_normalized_variances_per_metacell, quantile=type_gene_normalized_variance_quantile, per="column"
         )
 
-    for (type_name, type_gene_normalized_variances) in list(
+    for type_name, type_gene_normalized_variances in list(
         ut.parallel_map(_compute_single_type_genes_normalized_variances, len(unique_types))
     ):
         ut.set_v_data(gdata, f"normalized_variance_in_{type_name}", type_gene_normalized_variances)
 
 
 @ut.logged()
 @ut.timed_call()
 def _compute_metacell_genes_normalized_variances(
     *,
-    metacell_of_cells: ut.NumpyVector,
+    metacell_per_cell: ut.NumpyVector,
     cells_umis: ut.Matrix,
     position: int,
     metacell_index: int,
     type_gene_normalized_variances_per_metacell: ut.NumpyVector,
 ) -> None:
-    metacell_cells_mask = metacell_of_cells == metacell_index
+    metacell_cells_mask = metacell_per_cell == metacell_index
     metacell_umis = cells_umis[metacell_cells_mask, :]
     total_umis = ut.sum_per(metacell_umis, per="row")
     median_total_umis = np.median(total_umis)
     ut.log_calc("median_total_umis", median_total_umis)
     metacell_fractions = ut.fraction_by(metacell_umis, by="row")
     metacell_fractions = ut.to_layout(metacell_fractions, layout="column_major")
     metacell_fractions *= median_total_umis
     genes_normalized_variance = ut.normalized_variance_per(metacell_fractions, per="column")
     type_gene_normalized_variances_per_metacell[position, :] = genes_normalized_variance
+
+
+@ut.logged()
+@ut.timed_call()
+@ut.expand_doc()
+def compute_outliers_fold_factors(
+    what: Union[str, ut.Matrix] = "__x__",
+    *,
+    adata: AnnData,
+    gdata: AnnData,
+    most_similar: Union[str, ut.Vector] = "most_similar",
+    min_gene_total: int = pr.quality_min_gene_total,
+) -> None:
+    """
+    Given annotated data which is a slice containing just the outliers, where each has a "most similar" group, compute
+    for each observation and gene the fold factor relative to its group.
+
+    All outliers should have at least one (typically several) genes with high fold factors, which are the reason they
+    couldn't be merged into their most similar group.
+
+    **Input**
+
+    Annotated ``adata``, where the observations are outlier cells and the variables are genes, where ``what`` is a
+    per-variable-per-observation matrix or the name of a per-variable-per-observation annotation containing such a
+    matrix.
+
+    In addition, ``gdata`` is assumed to have one observation for each group, and use the same genes as ``adata``.
+    It should have a ``marker_gene`` mask.
+
+    **Returns**
+
+    Sets the following in ``adata``:
+
+    Per-Variable Per-Observation (Gene-Cell) Annotations
+
+        ``<most_similar>_fold`` (default: {most_similar}_fold)
+            The fold factor between the outlier gene expression and their expression in the most similar group, (unless
+            the value is too low to be of interest, in which case it will be zero).
+
+    **Computation Parameters**
+
+    1. For each outlier, compute the expected UMIs for each gene given the fraction of the gene in the metacell
+       associated with the outlier by the ``most_similar`` (default: {most_similar}).
+
+    2. If the sum of the UMIs of the gene in cell and the metacell are less than ``min_gene_total`` (default:
+       {min_gene_total}), set the fold factor to 0 as we do not have sufficient data to robustly estimate it.
+    """
+    assert list(adata.var_names) == list(gdata.var_names)
+
+    actual_umis_per_gene_per_outlier = ut.to_numpy_matrix(ut.get_vo_proper(adata, what, layout="row_major"), copy=True)
+    total_umis_per_outlier = ut.sum_per(actual_umis_per_gene_per_outlier, per="row")
+
+    most_similar_of_outliers = ut.get_o_numpy(adata, most_similar, formatter=ut.groups_description)
+    assert np.min(most_similar_of_outliers) >= 0
+
+    metacells_fractions = ut.to_numpy_matrix(ut.get_vo_proper(gdata, what, layout="row_major"))
+    metacells_umis = ut.to_numpy_matrix(ut.get_vo_proper(gdata, "total_umis", layout="row_major"))
+    fraction_per_gene_per_most_similar = ut.to_numpy_matrix(metacells_fractions[most_similar_of_outliers, :])
+    umis_per_gene_per_most_similar = ut.to_numpy_matrix(metacells_umis[most_similar_of_outliers, :])
+
+    expected_umis_per_gene_per_outlier = fraction_per_gene_per_most_similar * total_umis_per_outlier[:, np.newaxis]
+    assert actual_umis_per_gene_per_outlier.shape == expected_umis_per_gene_per_outlier.shape
+
+    actual_umis_per_gene_per_outlier += 1
+    expected_umis_per_gene_per_outlier += 1
+
+    fold_factor_per_gene_per_outlier = np.log2(actual_umis_per_gene_per_outlier) - np.log2(
+        expected_umis_per_gene_per_outlier
+    )
+
+    total_umis_per_gene_per_most_similar = umis_per_gene_per_most_similar[most_similar_of_outliers, :]
+    total_umis_per_gene_per_fold = actual_umis_per_gene_per_outlier + total_umis_per_gene_per_most_similar
+    fold_factor_per_gene_per_outlier[total_umis_per_gene_per_fold < min_gene_total] = 0.0
+
+    fold_factor_per_gene_per_outlier = sp.csr_matrix(fold_factor_per_gene_per_outlier)
+    fold_factor_per_gene_per_outlier.has_sorted_indices = True
+    fold_factor_per_gene_per_outlier.has_canonical_format = True
+    ut.set_vo_data(adata, f"{most_similar}_fold", fold_factor_per_gene_per_outlier)
+
+
+@ut.logged()
+@ut.timed_call()
+@ut.expand_doc()
+def count_significant_inner_folds(
+    adata: AnnData,
+    *,
+    min_gene_fold_factor: float = pr.significant_gene_fold_factor,
+) -> None:
+    """
+    Given grouped (metacells) data, count for each gene in how many metacells there is at least one cell
+    with a fold factor above some threshold.
+
+    **Input**
+
+    Annotated ``adata``, where the observations are metacells and the variables are genes, with an ``inner_fold``
+    layer (as computed by ``compute_inner_folds``).
+
+    **Returns**
+
+    Sets the ``significant_inner_folds_count`` annotation, counting for each gene the number of metacells
+    where the ``inner_fold`` is at least ``min_gene_fold_factor`` (default: {min_gene_fold_factor}), that is,
+    where at least one cell in the metacell has a high fold factor for the gene's expression compared to the
+    estimated overall gene expression in the metacell.
+    """
+    inner_fold_per_gene_per_metacell = ut.get_vo_proper(adata, "inner_fold", layout="column_major")
+    significant_per_gene_per_metacell = inner_fold_per_gene_per_metacell >= min_gene_fold_factor  # type: ignore
+    significant_per_gene = ut.sum_per(significant_per_gene_per_metacell, per="column")  # type: ignore
+    ut.set_v_data(adata, "significant_inner_folds_count", significant_per_gene, formatter=ut.sizes_description)
```

### Comparing `metacells-0.8.0/metacells/tools/rare.py` & `metacells-0.9.0/metacells/tools/rare.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,82 +1,79 @@
 """
 Rare
 ----
 """
 
-from re import Pattern
-from typing import Collection
 from typing import List
 from typing import Optional
 from typing import Set
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 import scipy.cluster.hierarchy as sch  # type: ignore
 import scipy.spatial.distance as scd  # type: ignore
 from anndata import AnnData  # type: ignore
 
 import metacells.parameters as pr
 import metacells.utilities as ut
 
-from .named import find_named_genes
 from .similarity import compute_var_var_similarity
 
 __all__ = [
     "find_rare_gene_modules",
 ]
 
 
 @ut.logged()
 @ut.timed_call()
 @ut.expand_doc()
 def find_rare_gene_modules(
     adata: AnnData,
     what: Union[str, ut.Matrix] = "__x__",
     *,
+    max_genes: int = pr.rare_max_genes,
     max_gene_cell_fraction: float = pr.rare_max_gene_cell_fraction,
     min_gene_maximum: int = pr.rare_min_gene_maximum,
     genes_similarity_method: str = pr.rare_genes_similarity_method,
     genes_cluster_method: str = pr.rare_genes_cluster_method,
-    forbidden_gene_names: Optional[Collection[str]] = None,
-    forbidden_gene_patterns: Optional[Collection[Union[str, Pattern]]] = None,
     min_genes_of_modules: int = pr.rare_min_genes_of_modules,
     min_cells_of_modules: int = pr.rare_min_cells_of_modules,
     target_pile_size: int = pr.min_target_pile_size,
     max_cells_factor_of_random_pile: float = pr.rare_max_cells_factor_of_random_pile,
     target_metacell_size: float = pr.target_metacell_size,
-    min_modules_size_factor: float = pr.rare_min_modules_size_factor,
     min_module_correlation: float = pr.rare_min_module_correlation,
     min_related_gene_fold_factor: float = pr.rare_min_related_gene_fold_factor,
     max_related_gene_increase_factor: float = pr.rare_max_related_gene_increase_factor,
     min_cell_module_total: int = pr.rare_min_cell_module_total,
-    reproducible: bool = pr.reproducible,
     inplace: bool = True,
+    reproducible: bool,
 ) -> Optional[Tuple[ut.PandasFrame, ut.PandasFrame]]:
     """
     Detect rare genes modules based on ``what`` (default: {what}) data.
 
     Rare gene modules include genes which are weakly and rarely expressed, yet are highly correlated
     with each other, allowing for robust detection. Global analysis algorithms (such as metacells)
     tend to ignore or at least discount such genes.
 
     It is therefore useful to explicitly identify, in a pre-processing step, the few cells which
     express such rare gene modules. Once identified, these cells can be exempt from the global
     algorithm, or the global algorithm can be tweaked in some way to pay extra attention to them.
 
-    If ``reproducible`` (default: {reproducible}) is ``True``, a slower (still parallel) but
-    reproducible algorithm will be used to compute pearson correlations.
+    If ``reproducible`` is ``True``, a slower (still parallel) but reproducible algorithm will be used to compute
+    pearson correlations.
 
     **Input**
 
     Annotated ``adata``, where the observations are cells and the variables are genes, where
     ``what`` is a per-variable-per-observation matrix or the name of a per-variable-per-observation
     annotation containing such a matrix.
 
+    Obeys (ignores the genes of) the ``lateral_gene`` per-gene (variable) annotation, if any.
+
     **Returns**
 
     Observation (Cell) Annotations
         ``cells_rare_gene_module``
             The index of the rare gene module each cell expresses the most, or ``-1`` in the common
             case it does not express any rare genes module.
 
@@ -91,18 +88,19 @@
             The index of the rare gene module a gene belongs to (-1 for non-rare genes).
 
     If ``inplace``, these are written to to the data, and the function returns ``None``. Otherwise
     they are returned as tuple containing two data frames.
 
     **Computation Parameters**
 
-    1. Pick as candidates all genes that are expressed in at most than ``max_gene_cell_fraction``
-       (default: {max_gene_cell_fraction}) of the cells, and whose maximal value in a cell is at
-       least ``min_gene_maximum`` (default: {min_gene_maximum}), as long as they do not match the
-       ``forbidden_gene_names`` or the ``forbidden_gene_patterns``.
+    1. Pick as candidates all genes that are expressed in at most ``max_gene_cell_fraction``
+       (default: {max_gene_cell_fraction}) of the cells, and whose maximal value in a cell is at least
+       ``min_gene_maximum`` (default: {min_gene_maximum}). If a ``lateral_gene`` masks exist, exclude them from the
+       candidates. Out of the candidates, pick at most ``max_genes`` (default {max_genes}) which are expressed in the
+       least cells.
 
     2. Compute the similarity between the genes using
        :py:func:`metacells.tools.similarity.compute_var_var_similarity` using the
        ``genes_similarity_method`` (default: {genes_similarity_method}).
 
     3. Create a hierarchical clustering of the candidate genes using the ``genes_cluster_method``
        (default: {genes_cluster_method}).
@@ -112,59 +110,55 @@
        cross-correlation of at least ``min_module_correlation`` (default:
        {min_module_correlation}).
 
     5. Consider cells expressing of any of the genes in the gene module. If the expected number of
        such cells in each random pile of size ``target_pile_size`` (default: {target_pile_size}), whose total number of
        UMIs of the rare gene module is at least ``min_cell_module_total`` (default: {min_cell_module_total}), is more
        than the ``max_cells_factor_of_random_pile`` (default: {max_cells_factor_of_random_pile}) as a fraction of the
-       mean metacells size, then discard the rare gene module as not that rare after all.
+       target metacells size, then discard the rare gene module as not that rare after all.
 
     6. Add to the gene module all genes whose fraction in cells expressing any of the genes in the
        rare gene module is at least 2^``min_related_gene_fold_factor`` (default:
        {min_related_gene_fold_factor}) times their fraction in the rest of the population, as long
        as their maximal value in one of the expressing cells is at least ``min_gene_maximum``,
        as long as this doesn't add more than ``max_related_gene_increase_factor`` times the original
-       number of cells to the rare gene module, and as long as they do not match the
-       ``forbidden_gene_names`` or the ``forbidden_gene_patterns``. If a gene is above the threshold
-       for multiple gene modules, associate it with the gene module for which its fold factor is
-       higher.
+       number of cells to the rare gene module, and as long as they are not listed in the ``lateral_gene`` masks. If a
+       gene is above the threshold for multiple gene modules, associate it with the gene module for which its fold
+       factor is higher.
 
     7. Associate cells with the rare gene module if they contain at least ``min_cell_module_total``
        (default: {min_cell_module_total}) UMIs of the expanded rare gene module. If a cell meets the
        above threshold for several rare gene modules, it is associated with the one for which it
        contains more UMIs.
-
-    8. Discard modules which have less than ``min_cells_of_modules`` (default:
-       {min_cells_of_modules}) cells or whose total UMIs are less than the ``target_metacell_size``
-       (default: {target_metacell_size}) times the ``min_modules_size_factor`` (default:
-       {min_modules_size_factor}).
     """
     assert min_cells_of_modules > 0
     assert min_genes_of_modules > 0
 
-    umis_per_gene = ut.get_v_numpy(adata, what, sum=True)
-    total_umis = np.sum(umis_per_gene)
-    mean_umis_per_cell = total_umis / adata.n_obs
-    mean_metacells_size = target_metacell_size / mean_umis_per_cell
-    ut.log_calc("mean_metacells_size", mean_metacells_size)
-    max_cells_of_random_pile = mean_metacells_size * max_cells_factor_of_random_pile
+    max_cells_of_random_pile = target_metacell_size * max_cells_factor_of_random_pile
     ut.log_calc("max_cells_of_random_pile", max_cells_of_random_pile)
 
-    forbidden_genes_mask = find_named_genes(adata, names=forbidden_gene_names, patterns=forbidden_gene_patterns)
-    assert forbidden_genes_mask is not None
+    allowed_genes_mask = np.full(adata.n_vars, True, dtype="bool")
+
+    if ut.has_data(adata, "lateral_gene"):
+        allowed_genes_mask &= ~ut.get_v_numpy(adata, "lateral_gene")
 
-    allowed_genes_mask = ~forbidden_genes_mask.values
     ut.log_calc("allowed_genes_mask", allowed_genes_mask)
 
     rare_module_of_cells = np.full(adata.n_obs, -1, dtype="int32")
     list_of_rare_gene_indices_of_modules: List[List[int]] = []
 
+    umis_per_gene_per_cell_by_rows = ut.get_vo_proper(adata, what, layout="row_major")
+    ut.log_calc("umis_per_gene_per_cell_by_rows", umis_per_gene_per_cell_by_rows)
+    umis_per_gene_per_cell_by_columns = ut.get_vo_proper(adata, what, layout="column_major")
+    ut.log_calc("umis_per_gene_per_cell_by_columns", umis_per_gene_per_cell_by_columns)
+
     candidates = _pick_candidates(
         adata_of_all_genes_of_all_cells=adata,
         what=what,
+        max_genes=max_genes,
         max_gene_cell_fraction=max_gene_cell_fraction,
         min_gene_maximum=min_gene_maximum,
         min_genes_of_modules=min_genes_of_modules,
         allowed_genes_mask=allowed_genes_mask,
     )
     if candidates is None:
         return _results(
@@ -192,43 +186,41 @@
     )
 
     max_cells_of_modules = int(max_cells_of_random_pile * adata.n_obs / target_pile_size)
     ut.log_calc("max_cells_of_modules", max_cells_of_modules)
 
     related_gene_indices_of_modules = _related_genes(
         adata_of_all_genes_of_all_cells=adata,
-        what=what,
+        umis_per_gene_per_cell_by_columns=umis_per_gene_per_cell_by_columns,
+        umis_per_gene_per_cell_by_rows=umis_per_gene_per_cell_by_rows,
         rare_gene_indices_of_modules=rare_gene_indices_of_modules,
         allowed_genes_mask=allowed_genes_mask,
         min_genes_of_modules=min_genes_of_modules,
         min_cells_of_modules=min_cells_of_modules,
         max_cells_of_modules=max_cells_of_modules,
         min_cell_module_total=min_cell_module_total,
         min_gene_maximum=min_gene_maximum,
         min_related_gene_fold_factor=min_related_gene_fold_factor,
         max_related_gene_increase_factor=max_related_gene_increase_factor,
     )
 
     _identify_cells(
         adata_of_all_genes_of_all_cells=adata,
-        what=what,
+        umis_per_gene_per_cell_by_columns=umis_per_gene_per_cell_by_columns,
         related_gene_indices_of_modules=related_gene_indices_of_modules,
         min_cells_of_modules=min_cells_of_modules,
         max_cells_of_modules=max_cells_of_modules,
         min_cell_module_total=min_cell_module_total,
         rare_module_of_cells=rare_module_of_cells,
     )
 
     list_of_rare_gene_indices_of_modules = _compress_modules(
         adata_of_all_genes_of_all_cells=adata,
-        what=what,
         min_cells_of_modules=min_cells_of_modules,
         max_cells_of_modules=max_cells_of_modules,
-        target_metacell_size=target_metacell_size,
-        min_modules_size_factor=min_modules_size_factor,
         related_gene_indices_of_modules=related_gene_indices_of_modules,
         rare_module_of_cells=rare_module_of_cells,
     )
 
     return _results(
         adata=adata,
         rare_module_of_cells=rare_module_of_cells,
@@ -238,14 +230,15 @@
 
 
 @ut.timed_call()
 def _pick_candidates(
     *,
     adata_of_all_genes_of_all_cells: AnnData,
     what: Union[str, ut.Matrix] = "__x__",
+    max_genes: int,
     max_gene_cell_fraction: float,
     min_gene_maximum: int,
     min_genes_of_modules: int,
     allowed_genes_mask: ut.NumpyVector,
 ) -> Optional[Tuple[AnnData, ut.NumpyVector]]:
     data = ut.get_vo_proper(adata_of_all_genes_of_all_cells, what, layout="column_major")
     nnz_cells_of_genes = ut.nnz_per(data, per="column")
@@ -257,14 +250,21 @@
     max_umis_mask_of_genes = max_umis_of_genes >= min_gene_maximum
 
     candidates_mask_of_genes = max_umis_mask_of_genes & nnz_cell_fraction_mask_of_genes & allowed_genes_mask
     ut.log_calc("candidate_genes", candidates_mask_of_genes)
 
     candidate_genes_indices = np.where(candidates_mask_of_genes)[0]
     candidate_genes_count = candidate_genes_indices.size
+
+    if candidate_genes_count > max_genes:
+        nnz_cell_fraction_of_candidates = nnz_cell_fraction_of_genes[candidate_genes_indices]
+        partitioned_genes_indices = np.argpartition(nnz_cell_fraction_of_candidates, max_genes)
+        candidate_genes_indices = candidate_genes_indices[partitioned_genes_indices[0:max_genes]]
+        candidate_genes_count = candidate_genes_indices.size
+
     if candidate_genes_count < min_genes_of_modules:
         return None
 
     candidate_data = ut.slice(
         adata_of_all_genes_of_all_cells, name=".candidate_genes", vars=candidate_genes_indices, top_level=False
     )
     return candidate_data, candidate_genes_indices
@@ -334,33 +334,37 @@
         if average_link_similarity < min_module_correlation:
             continue
 
         combined_candidate_indices[link_index] = link_combined_candidates
         del combined_candidate_indices[left_index]
         del combined_candidate_indices[right_index]
 
-    return [candidate_genes_indices[candidate_indices] for candidate_indices in combined_candidate_indices.values()]
+    return [
+        list(candidate_genes_indices[candidate_indices]) for candidate_indices in combined_candidate_indices.values()
+    ]
 
 
 @ut.timed_call()
 def _related_genes(  # pylint: disable=too-many-statements,too-many-branches
     *,
     adata_of_all_genes_of_all_cells: AnnData,
-    what: Union[str, ut.Matrix] = "__x__",
+    umis_per_gene_per_cell_by_rows: ut.ProperMatrix,
+    umis_per_gene_per_cell_by_columns: ut.ProperMatrix,
     rare_gene_indices_of_modules: List[List[int]],
     allowed_genes_mask: ut.NumpyVector,
     min_genes_of_modules: int,
     min_gene_maximum: int,
     min_cells_of_modules: int,
     max_cells_of_modules: int,
     min_cell_module_total: int,
     min_related_gene_fold_factor: float,
     max_related_gene_increase_factor: float,
 ) -> List[List[int]]:
-    total_all_cells_umis_of_all_genes = ut.get_v_numpy(adata_of_all_genes_of_all_cells, what, sum=True)
+    total_umis_per_gene = ut.sum_per(umis_per_gene_per_cell_by_columns, per="column")
+    ut.log_calc("total_umis_per_gene", total_umis_per_gene)
 
     ut.log_calc("genes for modules:")
     modules_count = 0
     related_gene_indices_of_modules: List[List[int]] = []
 
     rare_gene_indices_of_any: Set[int] = set()
     for rare_gene_indices_of_module in rare_gene_indices_of_modules:
@@ -375,124 +379,109 @@
         modules_count += 1
 
         with ut.log_step("- module", module_index):
             ut.log_calc(
                 "rare_gene_names", sorted(adata_of_all_genes_of_all_cells.var_names[rare_gene_indices_of_module])
             )
 
-            adata_of_module_genes_of_all_cells = ut.slice(
-                adata_of_all_genes_of_all_cells,
-                name=f".module{module_index}.rare_gene",
-                vars=rare_gene_indices_of_module,
-                top_level=False,
-            )
+            umis_per_module_gene_per_cell_by_columns = umis_per_gene_per_cell_by_columns[:, rare_gene_indices_of_module]
+            ut.log_calc("umis_per_module_gene_per_cell_by_columns", umis_per_module_gene_per_cell_by_columns)
+            assert ut.is_layout(umis_per_module_gene_per_cell_by_columns, "column_major")
 
-            total_module_genes_umis_of_all_cells = ut.get_o_numpy(adata_of_module_genes_of_all_cells, what, sum=True)
+            umis_per_module_gene_per_cell_by_rows = ut.to_layout(
+                umis_per_module_gene_per_cell_by_columns, layout="row_major"
+            )
+            ut.log_calc("umis_per_module_gene_per_cell_by_rows", umis_per_module_gene_per_cell_by_rows)
 
-            mask_of_expressed_cells = total_module_genes_umis_of_all_cells > 0
+            total_module_umis_per_cell = ut.sum_per(umis_per_module_gene_per_cell_by_rows, per="row")
+            ut.log_calc("total_module_umis_per_cell", total_module_umis_per_cell)
 
+            mask_of_expressed_cells = total_module_umis_per_cell > 0
             expressed_cells_count = np.sum(mask_of_expressed_cells)
 
             if expressed_cells_count > max_cells_of_modules:
                 if ut.logging_calc():
                     ut.log_calc("expressed_cells", ut.mask_description(mask_of_expressed_cells) + " (too many)")
                 continue
 
             if expressed_cells_count < min_cells_of_modules:
                 if ut.logging_calc():
                     ut.log_calc("expressed_cells", ut.mask_description(mask_of_expressed_cells) + " (too few)")
                 continue
 
             ut.log_calc("expressed_cells", mask_of_expressed_cells)
 
-            adata_of_all_genes_of_expressed_cells_of_module = ut.slice(
-                adata_of_all_genes_of_all_cells,
-                name=f".module{module_index}.rare_cell",
-                obs=mask_of_expressed_cells,
-                top_level=False,
-            )
+            umis_per_gene_per_expressed_cell_by_rows = umis_per_gene_per_cell_by_rows[mask_of_expressed_cells, :]
+            ut.log_calc("umis_per_gene_per_expressed_cell_by_rows", umis_per_gene_per_expressed_cell_by_rows)
+            assert ut.is_layout(umis_per_gene_per_expressed_cell_by_rows, "row_major")
 
-            total_expressed_cells_umis_of_all_genes = ut.get_v_numpy(
-                adata_of_all_genes_of_expressed_cells_of_module, what, sum=True
+            umis_per_gene_per_expressed_cell_by_columns = ut.to_layout(
+                umis_per_gene_per_expressed_cell_by_rows, layout="column_major"
             )
+            ut.log_calc("umis_per_module_gene_per_cell_by_columns", umis_per_module_gene_per_cell_by_columns)
 
-            data = ut.get_vo_proper(adata_of_all_genes_of_expressed_cells_of_module, what, layout="column_major")
-            max_expressed_cells_umis_of_all_genes = ut.max_per(data, per="column")
-
-            total_background_cells_umis_of_all_genes = (
-                total_all_cells_umis_of_all_genes - total_expressed_cells_umis_of_all_genes
-            )
+            max_expressed_umis_per_gene = ut.max_per(umis_per_gene_per_expressed_cell_by_columns, per="column")
+            ut.log_calc("max_expressed_umis_per_gene", max_expressed_umis_per_gene)
 
-            expressed_cells_fraction_of_all_genes = total_expressed_cells_umis_of_all_genes / sum(
-                total_expressed_cells_umis_of_all_genes
-            )
+            total_expressed_umis_per_gene = ut.sum_per(umis_per_gene_per_expressed_cell_by_columns, per="column")
+            expressed_fraction_per_gene = total_expressed_umis_per_gene / sum(total_expressed_umis_per_gene)
+            ut.log_calc("expressed_fraction_per_gene", expressed_fraction_per_gene)
 
-            background_cells_fraction_of_all_genes = total_background_cells_umis_of_all_genes / sum(
-                total_background_cells_umis_of_all_genes
-            )
+            total_background_umis_per_gene = total_umis_per_gene - total_expressed_umis_per_gene
+            background_fraction_per_gene = total_background_umis_per_gene / sum(total_background_umis_per_gene)
+            ut.log_calc("background_fraction_per_gene", background_fraction_per_gene)
 
             mask_of_related_genes = (
                 allowed_genes_mask
-                & (max_expressed_cells_umis_of_all_genes >= min_gene_maximum)
-                & (
-                    expressed_cells_fraction_of_all_genes
-                    >= background_cells_fraction_of_all_genes * (2 ** min_related_gene_fold_factor)
-                )
+                & (max_expressed_umis_per_gene >= min_gene_maximum)
+                & (expressed_fraction_per_gene >= background_fraction_per_gene * (2**min_related_gene_fold_factor))
             )
+            ut.log_calc("mask_of_related_genes", mask_of_related_genes)
 
             related_gene_indices = np.where(mask_of_related_genes)[0]
             assert np.all(mask_of_related_genes[rare_gene_indices_of_module])
 
-            base_genes_of_all_cells_adata = ut.slice(
-                adata_of_all_genes_of_all_cells, name=f".module{module_index}.base", vars=rare_gene_indices_of_module
-            )
-            total_base_genes_of_all_cells = ut.get_o_numpy(base_genes_of_all_cells_adata, what, sum=True)
-            mask_of_strong_base_cells = total_base_genes_of_all_cells >= min_cell_module_total
+            mask_of_strong_base_cells = total_module_umis_per_cell >= min_cell_module_total
             count_of_strong_base_cells = np.sum(mask_of_strong_base_cells)
 
             if ut.logging_calc():
                 ut.log_calc(
                     "candidate_gene_names", sorted(adata_of_all_genes_of_all_cells.var_names[related_gene_indices])
                 )
-                ut.log_calc("base_strong_genes", count_of_strong_base_cells)
+                ut.log_calc("mask_of_strong_base_cells", mask_of_strong_base_cells)
 
             related_gene_indices_of_module = list(rare_gene_indices_of_module)
             for gene_index in related_gene_indices:
                 if gene_index in rare_gene_indices_of_module:
                     continue
 
                 if gene_index in rare_gene_indices_of_any:
                     ut.log_calc(
                         f"- candidate gene {adata_of_all_genes_of_all_cells.var_names[gene_index]} "
                         f"belongs to another module"
                     )
                     continue
 
-                if gene_index not in rare_gene_indices_of_module:
-                    related_gene_of_all_cells_adata = ut.slice(
-                        adata_of_all_genes_of_all_cells,
-                        name=f".{adata_of_all_genes_of_all_cells.var_names[gene_index]}",
-                        vars=np.array([gene_index]),
-                    )
-                    assert related_gene_of_all_cells_adata.n_vars == 1
-                    total_related_genes_of_all_cells = ut.get_o_numpy(related_gene_of_all_cells_adata, what, sum=True)
-                    total_related_genes_of_all_cells += total_base_genes_of_all_cells
-                    mask_of_strong_related_cells = total_related_genes_of_all_cells >= min_cell_module_total
-                    count_of_strong_related_cells = np.sum(mask_of_strong_related_cells)
-                    ut.log_calc(
-                        f"- candidate gene {adata_of_all_genes_of_all_cells.var_names[gene_index]} "
-                        f"strong cells: {count_of_strong_related_cells} "
-                        f"factor: {count_of_strong_related_cells / count_of_strong_base_cells}"
-                    )
-                    if count_of_strong_related_cells > max_related_gene_increase_factor * count_of_strong_base_cells:
-                        continue
+                umis_of_related_gene_per_cell = ut.to_numpy_vector(
+                    umis_per_gene_per_cell_by_columns[:, gene_index], copy=True
+                )
+                umis_of_related_gene_per_cell += total_module_umis_per_cell
+                mask_of_strong_related_cells = umis_of_related_gene_per_cell >= min_cell_module_total
+                count_of_strong_related_cells = np.sum(mask_of_strong_related_cells)
+                ut.log_calc(
+                    f"- candidate gene {adata_of_all_genes_of_all_cells.var_names[gene_index]} "
+                    f"strong cells: {count_of_strong_related_cells} "
+                    f"factor: {count_of_strong_related_cells / count_of_strong_base_cells}"
+                )
+                if count_of_strong_related_cells > max_related_gene_increase_factor * count_of_strong_base_cells:
+                    continue
 
                 related_gene_indices_of_module.append(gene_index)
 
-            related_gene_indices_of_modules.append(related_gene_indices_of_module)  #
+            related_gene_indices_of_modules.append(related_gene_indices_of_module)
 
     if ut.logging_calc():
         ut.log_calc("related genes for modules:")
         for module_index, related_gene_indices_of_module in enumerate(related_gene_indices_of_modules):
             ut.log_calc(
                 f"- module {module_index} related_gene_names",
                 sorted(adata_of_all_genes_of_all_cells.var_names[related_gene_indices_of_module]),
@@ -501,15 +490,15 @@
     return related_gene_indices_of_modules
 
 
 @ut.timed_call()
 def _identify_cells(
     *,
     adata_of_all_genes_of_all_cells: AnnData,
-    what: Union[str, ut.Matrix] = "__x__",
+    umis_per_gene_per_cell_by_columns: ut.ProperMatrix,
     related_gene_indices_of_modules: List[List[int]],
     min_cell_module_total: int,
     min_cells_of_modules: int,
     max_cells_of_modules: int,
     rare_module_of_cells: ut.NumpyVector,
 ) -> None:
     max_strength_of_cells = np.zeros(adata_of_all_genes_of_all_cells.n_obs)
@@ -521,25 +510,29 @@
             continue
 
         with ut.log_step(
             "- module",
             module_index,
             formatter=lambda module_index: ut.progress_description(modules_count, module_index, "module"),
         ):
-            adata_of_related_genes_of_all_cells = ut.slice(
-                adata_of_all_genes_of_all_cells,
-                name=f".module{module_index}.related_genes",
-                vars=related_gene_indices_of_module,
-                top_level=False,
+            umis_per_related_gene_per_cell_by_columns = umis_per_gene_per_cell_by_columns[
+                :, related_gene_indices_of_module
+            ]
+            ut.log_calc("umis_per_related_gene_per_cell_by_columns", umis_per_related_gene_per_cell_by_columns)
+
+            umis_per_related_gene_per_cell_by_rows = ut.to_layout(
+                umis_per_related_gene_per_cell_by_columns, layout="row_major"
             )
-            total_related_genes_of_all_cells = ut.get_o_numpy(adata_of_related_genes_of_all_cells, what, sum=True)
+            ut.log_calc("umis_per_related_gene_per_cell_by_rows", umis_per_related_gene_per_cell_by_rows)
+
+            total_related_umis_per_cell = ut.sum_per(umis_per_related_gene_per_cell_by_rows, per="row")
 
-            mask_of_strong_cells_of_module = total_related_genes_of_all_cells >= min_cell_module_total
+            mask_of_strong_cells_of_module = total_related_umis_per_cell >= min_cell_module_total
 
-            median_strength_of_module = np.median(total_related_genes_of_all_cells[mask_of_strong_cells_of_module])  #
+            median_strength_of_module = np.median(total_related_umis_per_cell[mask_of_strong_cells_of_module])  #
             strong_cells_count = np.sum(mask_of_strong_cells_of_module)
 
             if strong_cells_count > max_cells_of_modules:
                 if ut.logging_calc():
                     ut.log_calc("strong_cells", ut.mask_description(mask_of_strong_cells_of_module) + " (too many)")  #
                 related_gene_indices_of_module.clear()
                 continue
@@ -548,43 +541,35 @@
                 if ut.logging_calc():
                     ut.log_calc("strong_cells", ut.mask_description(mask_of_strong_cells_of_module) + " (too few)")  #
                 related_gene_indices_of_module.clear()
                 continue
 
             ut.log_calc("strong_cells", mask_of_strong_cells_of_module)
 
-            strength_of_all_cells = total_related_genes_of_all_cells / median_strength_of_module
+            strength_of_all_cells = total_related_umis_per_cell / median_strength_of_module
             mask_of_strong_cells_of_module &= strength_of_all_cells >= max_strength_of_cells
             max_strength_of_cells[mask_of_strong_cells_of_module] = strength_of_all_cells[
                 mask_of_strong_cells_of_module
             ]
 
             rare_module_of_cells[mask_of_strong_cells_of_module] = module_index
 
 
 @ut.timed_call()
 def _compress_modules(
     *,
     adata_of_all_genes_of_all_cells: AnnData,
-    what: Union[str, ut.Matrix] = "__x__",
     min_cells_of_modules: int,
     max_cells_of_modules: int,
-    target_metacell_size: float,
-    min_modules_size_factor: float,
     related_gene_indices_of_modules: List[List[int]],
     rare_module_of_cells: ut.NumpyVector,
 ) -> List[List[int]]:
     list_of_rare_gene_indices_of_modules: List[List[int]] = []
     list_of_names_of_genes_of_modules: List[List[str]] = []
 
-    min_umis_of_modules = target_metacell_size * min_modules_size_factor
-    ut.log_calc("min_umis_of_modules", min_umis_of_modules)
-
-    total_all_genes_of_all_cells = ut.get_o_numpy(adata_of_all_genes_of_all_cells, what, sum=True)
-
     cell_counts_of_modules: List[int] = []
 
     ut.log_calc("compress modules:")
     modules_count = len(related_gene_indices_of_modules)
     for module_index, gene_indices_of_module in enumerate(related_gene_indices_of_modules):
         if len(gene_indices_of_module) == 0:
             continue
@@ -592,15 +577,14 @@
         with ut.log_step(
             "- module",
             module_index,
             formatter=lambda module_index: ut.progress_description(modules_count, module_index, "module"),
         ):
             module_cells_mask = rare_module_of_cells == module_index
             module_cells_count = np.sum(module_cells_mask)
-            module_umis_count = np.sum(total_all_genes_of_all_cells[module_cells_mask])
 
             if module_cells_count < min_cells_of_modules:
                 if ut.logging_calc():
                     ut.log_calc("cells", str(module_cells_count) + " (too few)")
                 rare_module_of_cells[module_cells_mask] = -1
                 continue
 
@@ -608,22 +592,14 @@
                 if ut.logging_calc():
                     ut.log_calc("cells", str(module_cells_count) + " (too many)")
                 rare_module_of_cells[module_cells_mask] = -1
                 continue
 
             ut.log_calc("cells", module_cells_count)
 
-            if module_umis_count < min_umis_of_modules:
-                if ut.logging_calc():
-                    ut.log_calc("UMIs", str(module_umis_count) + " (too few)")
-                rare_module_of_cells[module_cells_mask] = -1
-                continue
-
-            ut.log_calc("UMIs", module_umis_count)
-
             next_module_index = len(list_of_rare_gene_indices_of_modules)
             if module_index != next_module_index:
                 ut.log_calc("is reindexed to", next_module_index)
                 rare_module_of_cells[module_cells_mask] = next_module_index
                 module_index = next_module_index
 
             next_module_index += 1
```

### Comparing `metacells-0.8.0/metacells/tools/similarity.py` & `metacells-0.9.0/metacells/tools/similarity.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Cross-Similarity
 ----------------
 """
 
 from typing import Optional
 from typing import Union
 
+import numpy as np
 from anndata import AnnData  # type: ignore
 
 import metacells.parameters as pr
 import metacells.utilities as ut
 
 __all__ = [
     "compute_obs_obs_similarity",
@@ -21,32 +22,35 @@
 @ut.timed_call()
 @ut.expand_doc()
 def compute_obs_obs_similarity(
     adata: AnnData,
     what: Union[str, ut.Matrix] = "__x__",
     *,
     method: str = pr.similarity_method,
-    reproducible: bool = pr.reproducible,
     logistics_location: float = pr.logistics_location,
     logistics_slope: float = pr.logistics_slope,
     top: Optional[int] = None,
     bottom: Optional[int] = None,
     inplace: bool = True,
+    reproducible: bool,
 ) -> Optional[ut.PandasFrame]:
     """
     Compute a measure of the similarity between the observations (cells) of ``what`` (default: {what}).
 
-    If ``reproducible`` (default: {reproducible}) is ``True``, a slower (still parallel) but
+    If ``reproducible`` is ``True``, a slower (still parallel) but
     reproducible algorithm will be used to compute Pearson correlations.
 
     The ``method`` (default: {method}) can be one of:
     * ``pearson`` for computing Pearson correlation.
+    * ``abs_pearson`` for computing the absolute Pearson correlation.
     * ``repeated_pearson`` for computing correlations-of-correlations.
+    * ``repeated_abs_pearson`` for computing absolute correlations-of-correlations.
     * ``logistics`` for computing the logistics function.
     * ``logistics_pearson`` for computing correlations-of-logistics.
+    * ``logistics_abs_pearson`` for computing absolute correlations-of-logistics.
 
     If using the logistics function, use the ``logistics_slope`` (default: {logistics_slope}) and
     ``logistics_location`` (default: {logistics_location}).
 
     **Input**
 
     Annotated ``adata``, where the observations are cells and the variables are genes, where
@@ -96,38 +100,41 @@
 @ut.timed_call()
 @ut.expand_doc()
 def compute_var_var_similarity(
     adata: AnnData,
     what: Union[str, ut.Matrix] = "__x__",
     *,
     method: str = pr.similarity_method,
-    reproducible: bool = pr.reproducible,
     logistics_location: float = pr.logistics_location,
     logistics_slope: float = pr.logistics_slope,
     top: Optional[int] = None,
     bottom: Optional[int] = None,
     inplace: bool = True,
+    reproducible: bool,
 ) -> Optional[ut.PandasFrame]:
     """
     Compute a measure of the similarity between the variables (genes) of ``what`` (default: {what}).
 
-    If ``reproducible`` (default: {reproducible}) is ``True``, a slower (still parallel) but
-    reproducible algorithm will be used to compute pearson correlations.
+    If ``reproducible`` is ``True``, a slower (still parallel) but
+    reproducible algorithm will be used to compute Pearson correlations.
 
     **Input**
 
     Annotated ``adata``, where the observations are cells and the variables are genes, where
     ``what`` is a per-variable-per-observation matrix or the name of a per-variable-per-observation
     annotation containing such a matrix.
 
     The ``method`` (default: {method}) can be one of:
     * ``pearson`` for computing Pearson correlation.
+    * ``abs_pearson`` for computing the absolute Pearson correlation.
     * ``repeated_pearson`` for computing correlations-of-correlations.
+    * ``repeated_abs_pearson`` for computing absolute correlations-of-correlations.
     * ``logistics`` for computing the logistics function.
     * ``logistics_pearson`` for computing correlations-of-logistics.
+    * ``logistics_abs_pearson`` for computing absolute correlations-of-logistics.
 
     If using the logistics function, use the ``logistics_slope`` (default: {logistics_slope}) and
     ``logistics_location`` (default: {logistics_location}).
 
     **Returns**
 
     Variable-Pair (genes) Annotations
@@ -179,40 +186,53 @@
     logistics_slope: float,
     top: Optional[int],
     bottom: Optional[int],
     inplace: bool,
 ) -> Optional[ut.PandasFrame]:
     assert elements in ("obs", "var")
 
-    assert method in ("pearson", "repeated_pearson", "logistics", "logistics_pearson")
+    assert method in (
+        "logistics",
+        "logistics_pearson",
+        "logistics_abs_pearson",
+        "pearson",
+        "abs_pearson",
+        "repeated_pearson",
+        "repeated_abs_pearson",
+    ), f"invalid similarity method: {method}"
 
     data = ut.get_vo_proper(adata, what, layout=f"{per}_major")
     dense = ut.to_numpy_matrix(data)
 
     similarity: ut.ProperMatrix
-    if method.startswith("logistics"):
+    if method in ("logistics", "logistics_pearson", "logistics_abs_pearson"):
         similarity = ut.logistics(dense, location=logistics_location, slope=logistics_slope, per=per)
         similarity *= -1
         similarity += 1
     else:
         similarity = ut.corrcoef(dense, per=per, reproducible=reproducible)
+        if method in ("abs_pearson", "repeated_abs_pearson"):
+            np.absolute(similarity, out=similarity)
 
-    if method.endswith("_pearson"):
+    if method in ("repeated_pearson", "repeated_abs_pearson", "logistics_pearson", "logistics_abs_pearson"):
         similarity = ut.corrcoef(similarity, per=None, reproducible=reproducible)
+        if method in ("repeated_abs_pearson", "logistics_abs_pearson"):
+            np.absolute(similarity, out=similarity)
 
     if top is not None:
         top_similarity = ut.top_per(similarity, top, per="row")
 
     if bottom is not None:
         similarity *= -1
         bottom_similarity = ut.top_per(similarity, bottom, per="row")
         bottom_similarity *= -1  # type: ignore
 
     if top is not None:
         if bottom is not None:
+            assert top + bottom <= similarity.shape[0]
             similarity = top_similarity + bottom_similarity  # type: ignore
         else:
             similarity = top_similarity
     else:
         if bottom is not None:
             similarity = bottom_similarity
```

### Comparing `metacells-0.8.0/metacells/top_per.cpp` & `metacells-0.9.0/metacells/top_per.cpp`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/metacells/utilities/annotation.py` & `metacells-0.9.0/metacells/utilities/annotation.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,16 +121,16 @@
 
 
 @utm.timed_call()
 def slice(  # pylint: disable=redefined-builtin,too-many-branches,too-many-statements
     adata: AnnData,
     *,
     name: Optional[str] = None,
-    obs: utt.Vector = None,
-    vars: utt.Vector = None,
+    obs: Optional[utt.Vector] = None,
+    vars: Optional[utt.Vector] = None,
     track_obs: Optional[str] = None,
     track_var: Optional[str] = None,
     share_derived: bool = True,
     top_level: bool = True,
 ) -> AnnData:
     """
     Return new annotated data which includes a subset of the full ``adata``.
@@ -203,15 +203,14 @@
 
         if hasattr(bdata, "__is_top_level__"):
             delattr(bdata, "__is_top_level__")
         if hasattr(bdata, "__derived__"):
             delattr(bdata, "__derived__")
 
         if share_derived and (is_same_obs or is_same_obs is None) and (is_same_vars or is_same_vars is None):
-
             if is_same_obs is None:
                 is_same_obs = bdata.n_obs == adata.n_obs and bool(np.all(bdata.obs_names == adata.obs_names))
 
             if is_same_vars is None:
                 is_same_vars = bdata.n_vars == adata.n_vars and bool(np.all(bdata.var_names == adata.var_names))
 
             if is_same_obs and is_same_vars:
@@ -222,18 +221,18 @@
         if top_level:
             utl.top_level(bdata)
 
     if utl.logging_calc():
         utl.log_calc(f'slice {get_name(adata, "unnamed")} into {get_name(bdata, "unnamed")} shape {bdata.shape}')  #
 
     if track_obs is not None:
-        set_o_data(bdata, track_obs, np.arange(adata.n_obs)[obs])
+        set_o_data(bdata, track_obs, np.arange(adata.n_obs, dtype="int32")[obs])
 
     if track_var is not None:
-        set_v_data(bdata, track_var, np.arange(adata.n_vars)[vars])
+        set_v_data(bdata, track_var, np.arange(adata.n_vars, dtype="int32")[vars])
 
     return bdata
 
 
 @utm.timed_call()
 def _replace_with_layout(adata: AnnData, layout: str) -> Dict[str, utt.Matrix]:
     replaced: Dict[str, utt.Matrix] = {}
@@ -572,19 +571,24 @@
 
     If ``name`` is a string, it is the name of a per-variable annotation to fetch.
     Otherwise, it should be some matrix of data of the appropriate size.
 
     If ``layout`` (default: {layout}) is specified, it must be one of ``row_major`` or
     ``column_major``. If this requires relayout of the data, the result is cached in a hidden data
     member for future reuse.
+
+    .. note::
+
+        Since Pandas frames do not play well with sparse representations, this will **always** return the
+        data as a dense matrix. For very large data, this may consume much more memory, so use with care.
     """
     data = _get_oo_data(adata, name, layout=layout, formatter=formatter)
     frame = utt.maybe_pandas_frame(data)
     if frame is None:
-        frame = utt.to_pandas_frame(utt.to_proper_matrix(data), index=adata.obs_names, columns=adata.obs_names)
+        frame = utt.to_pandas_frame(utt.to_numpy_matrix(data), index=adata.obs_names, columns=adata.obs_names)
     return frame
 
 
 def get_oo_proper(
     adata: AnnData,
     name: Union[str, utt.Matrix],
     *,
@@ -622,19 +626,24 @@
 
     If ``name`` is a string, it is the name of a per-variable annotation to fetch.
     Otherwise, it should be some matrix of data of the appropriate size.
 
     If ``layout`` (default: {layout}) is specified, it must be one of ``row_major`` or
     ``column_major``. If this requires relayout of the data, the result is cached in a hidden data
     member for future reuse.
+
+    .. note::
+
+        Since Pandas frames do not play well with sparse representations, this will **always** return the
+        data as a dense matrix. For very large data, this may consume much more memory, so use with care.
     """
     data = _get_vv_data(adata, name, layout=layout, formatter=formatter)
     frame = utt.maybe_pandas_frame(data)
     if frame is None:
-        frame = utt.to_pandas_frame(utt.to_proper_matrix(data), index=adata.var_names, columns=adata.var_names)
+        frame = utt.to_pandas_frame(utt.to_numpy_matrix(data), index=adata.var_names, columns=adata.var_names)
     return frame
 
 
 def get_vv_proper(
     adata: AnnData,
     name: Union[str, utt.Matrix],
     *,
@@ -676,19 +685,24 @@
 
     If ``name`` is a string, it is the name of a per-variable annotation to fetch.
     Otherwise, it should be some matrix of data of the appropriate size.
 
     If ``layout`` (default: {layout}) is specified, it must be one of ``row_major`` or
     ``column_major``. If this requires relayout of the data, the result is cached in a hidden data
     member for future reuse.
+
+    .. note::
+
+        Since Pandas frames do not play well with sparse representations, this will **always** return the
+        data as a dense matrix. For very large data, this may consume much more memory, so use with care.
     """
     data = _get_oa_data(adata, name, layout=layout, formatter=formatter)
     frame = utt.maybe_pandas_frame(data)
     if frame is None:
-        frame = utt.to_pandas_frame(utt.to_proper_matrix(data), index=adata.obs_names, columns=columns)
+        frame = utt.to_pandas_frame(utt.to_numpy_matrix(data), index=adata.obs_names, columns=columns)
     return frame
 
 
 def get_oa_proper(
     adata: AnnData,
     name: Union[str, utt.Matrix],
     *,
@@ -730,19 +744,24 @@
 
     If ``name`` is a string, it is the name of a per-variable annotation to fetch.
     Otherwise, it should be some matrix of data of the appropriate size.
 
     If ``layout`` (default: {layout}) is specified, it must be one of ``row_major`` or
     ``column_major``. If this requires relayout of the data, the result is cached in a hidden data
     member for future reuse.
+
+    .. note::
+
+        Since Pandas frames do not play well with sparse representations, this will **always** return the
+        data as a dense matrix. For very large data, this may consume much more memory, so use with care.
     """
     data = _get_va_data(adata, name, layout=layout, formatter=formatter)
     frame = utt.maybe_pandas_frame(data)
     if frame is None:
-        frame = utt.to_pandas_frame(utt.to_proper_matrix(data), index=adata.var_names, columns=columns)
+        frame = utt.to_pandas_frame(utt.to_numpy_matrix(data), index=adata.var_names, columns=columns)
     return frame
 
 
 def get_va_proper(
     adata: AnnData,
     name: Union[str, utt.Matrix],
     *,
@@ -786,19 +805,24 @@
 
     If ``name`` is a string, it is the name of a per-variable annotation to fetch.
     Otherwise, it should be some matrix of data of the appropriate size.
 
     If ``layout`` (default: {layout}) is specified, it must be one of ``row_major`` or
     ``column_major``. If this requires relayout of the data, the result is cached in a hidden data
     member for future reuse.
+
+    .. note::
+
+        Since Pandas frames do not play well with sparse representations, this will **always** return the
+        data as a dense matrix. For very large data, this may consume much more memory, so use with care.
     """
     data = _get_vo_data(adata, name, layout=layout, formatter=formatter)
     frame = utt.maybe_pandas_frame(data)
     if frame is None:
-        frame = utt.to_pandas_frame(utt.to_proper_matrix(data), index=adata.obs_names, columns=adata.var_names)
+        frame = utt.to_pandas_frame(utt.to_numpy_matrix(data), index=adata.obs_names, columns=adata.var_names)
     return frame
 
 
 def get_vo_proper(
     adata: AnnData,
     name: Union[str, utt.Matrix] = "__x__",
     *,
@@ -1107,18 +1131,21 @@
     if name == "__x__":
         adata.X = data
     else:
         adata.layers[name] = data
 
     if hasattr(adata, "__derived__"):
         derived = getattr(adata, "__derived__")
-        for layout in ["column_major", "row_major"]:
-            layout_name = f"vo:{name}:{layout}"
-            if layout_name in derived:
-                del derived[layout_name]
+        marker_name = f":{name}:"
+        deleted_names: List[str] = []
+        for derived_name in derived.keys():
+            if marker_name in derived_name:
+                deleted_names.append(derived_name)
+        for deleted_name in deleted_names:
+            del derived[deleted_name]
 
 
 def _unknown_data(adata: AnnData, name: str, per: Optional[str] = None) -> KeyError:
     texts = ["unknown"]
 
     if per is not None:
         texts.append(" ")
```

### Comparing `metacells-0.8.0/metacells/utilities/computation.py` & `metacells-0.9.0/metacells/utilities/computation.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,19 @@
 from warnings import warn
 
 import cvxpy
 import igraph as ig  # type: ignore
 import numpy as np
 import pandas as pd  # type: ignore
 import scipy.sparse as sp  # type: ignore
+import scipy.stats as ss  # type: ignore
 
 import metacells.utilities.documentation as utd
+import metacells.utilities.logging as utl
+import metacells.utilities.parallel as utp
 import metacells.utilities.timing as utm
 import metacells.utilities.typing as utt
 
 if "sphinx" not in sys.argv[0]:
     import metacells.extensions as xt  # type: ignore
 
 __all__ = [
@@ -56,16 +59,18 @@
     "corrcoef",
     "cross_corrcoef_rows",
     "pairs_corrcoef_rows",
     "logistics",
     "cross_logistics_rows",
     "pairs_logistics_rows",
     "log_data",
+    "median_per",
     "mean_per",
     "nanmean_per",
+    "geomean_per",
     "max_per",
     "nanmax_per",
     "min_per",
     "nanmin_per",
     "nnz_per",
     "sum_per",
     "sum_squared_per",
@@ -73,44 +78,46 @@
     "top_per",
     "prune_per",
     "quantile_per",
     "nanquantile_per",
     "scale_by",
     "fraction_by",
     "fraction_per",
+    "stdev_per",
     "variance_per",
     "normalized_variance_per",
     "relative_variance_per",
     "sum_matrix",
     "nnz_matrix",
     "mean_matrix",
     "max_matrix",
     "min_matrix",
     "nanmean_matrix",
     "nanmax_matrix",
     "nanmin_matrix",
     "rank_matrix_by_layout",
     "bincount_vector",
     "most_frequent",
+    "strongest",
     "highest_weight",
+    "weighted_mean",
     "fraction_of_grouped",
     "downsample_matrix",
     "downsample_vector",
     "matrix_rows_folds_and_aurocs",
     "sliding_window_function",
     "patterns_matches",
     "compress_indices",
     "bin_pack",
     "bin_fill",
     "sum_groups",
     "shuffle_matrix",
     "cover_diameter",
     "cover_coordinates",
     "random_piles",
-    "group_piles",
     "represent",
     "min_cut",
     "sparsify_matrix",
 ]
 
 
 ALLOW_INEFFICIENT_LAYOUT: bool = True
@@ -188,19 +195,20 @@
         utm.timed_parameters(method="transpose")
         return proper
 
     is_frozen = utt.frozen(proper)
     result: utt.ProperMatrix
 
     if dense is not None:
-        utm.timed_parameters(method="reshape")
-        order = utt.DENSE_FAST_FLAG[layout][0]
-        with utm.timed_step("numpy.ravel"):
-            utm.timed_parameters(rows=dense.shape[0], columns=dense.shape[1])
-            result = np.reshape(np.ravel(dense, order=order), dense.shape, order=order)  # type: ignore
+        #       utm.timed_parameters(method="reshape")
+        #       order = utt.DENSE_FAST_FLAG[layout][0]
+        #       with utm.timed_step("numpy.ravel"):
+        #           utm.timed_parameters(rows=dense.shape[0], columns=dense.shape[1])
+        #           result = np.reshape(np.ravel(dense, order=order), dense.shape, order=order)  # type: ignore
+        result = _relayout_dense(dense, layout, 1024 * 1024)
 
     else:
         utm.timed_parameters(method="compressed")
         assert compressed is not None
         to_format = utt.SPARSE_FAST_FORMAT[layout]
         from_format = utt.SPARSE_SLOW_FORMAT[layout]
         assert compressed.getformat() == from_format
@@ -212,14 +220,41 @@
         utt.freeze(result)
 
     assert result.shape == matrix.shape
     return result
 
 
 @utm.timed_call()
+def _relayout_dense(dense: utt.NumpyMatrix, layout: str, block_size: int) -> utt.NumpyMatrix:
+    """
+    Efficient serial layout conversion of a ``dense`` matrix.
+    """
+    block_elements = int(sqrt(block_size / dense.dtype.itemsize))
+
+    row_elements = dense.shape[0]
+    column_elements = dense.shape[1]
+
+    row_blocks = int(ceil(row_elements / block_elements))
+    column_blocks = int(ceil(column_elements / block_elements))
+
+    numpy_order = utt.DENSE_FAST_FLAG[layout][0]
+    result = np.empty(dense.shape, dtype=dense.dtype, order=numpy_order)  # type: ignore
+
+    for row_block in range(row_blocks):
+        start_row = int(round(row_block * row_elements / row_blocks))
+        stop_row = int(round((row_block + 1) * row_elements / row_blocks))
+        for column_block in range(column_blocks):
+            start_column = int(round(column_block * column_elements / column_blocks))
+            stop_column = int(round((column_block + 1) * column_elements / column_blocks))
+            result[start_row:stop_row, start_column:stop_column] = dense[start_row:stop_row, start_column:stop_column]
+
+    return result
+
+
+@utm.timed_call()
 def _relayout_compressed(compressed: utt.CompressedMatrix) -> utt.CompressedMatrix:
     """
     Efficient parallel conversion of a CSR/CSC ``matrix`` to a CSC/CSR matrix.
     """
     axis = ("csr", "csc").index(compressed.getformat())
 
     if compressed.nnz < 2:
@@ -426,14 +461,16 @@
     if per == "column":
         dense = dense.T
     utm.timed_parameters(results=dense.shape[0], elements=dense.shape[1])
     extension_name = f"correlate_dense_{dense.dtype}_t"
     result = np.empty((dense.shape[0], dense.shape[0]), dtype="float32")
     extension = getattr(xt, extension_name)
     extension(dense, result)
+    result[np.isnan(result)] = 0.0
+    np.fill_diagonal(result, 1.0)
     return result
 
 
 @utm.timed_call()
 def cross_corrcoef_rows(
     first_matrix: utt.NumpyMatrix,
     second_matrix: utt.NumpyMatrix,
@@ -465,26 +502,33 @@
     first_matrix = utt.mustbe_numpy_matrix(first_matrix)
     second_matrix = utt.mustbe_numpy_matrix(second_matrix)
     assert utt.is_layout(first_matrix, "row_major")
     assert utt.is_layout(second_matrix, "row_major")
     assert first_matrix.shape[1] == second_matrix.shape[1]
     assert first_matrix.dtype == second_matrix.dtype
 
-    workaround = first_matrix.shape[0] == 1
-    if workaround:
+    first_workaround = first_matrix.shape[0] == 1
+    if first_workaround:
         first_matrix = np.concatenate([first_matrix, first_matrix])
 
+    second_workaround = second_matrix.shape[0] == 1
+    if second_workaround:
+        second_matrix = np.concatenate([second_matrix, second_matrix])
+
     extension_name = f"cross_correlate_dense_{first_matrix.dtype}_t"
     result = np.empty((first_matrix.shape[0], second_matrix.shape[0]), dtype="float32")
     extension = getattr(xt, extension_name)
     extension(first_matrix, second_matrix, result)
 
-    if workaround:
+    if first_workaround:
         result = result[0:1, :]
 
+    if second_workaround:
+        result = result[:, 0:1]
+
     return result
 
 
 @utm.timed_call()
 def pairs_corrcoef_rows(
     first_matrix: utt.NumpyMatrix,
     second_matrix: utt.NumpyMatrix,
@@ -514,18 +558,27 @@
     first_matrix = utt.mustbe_numpy_matrix(first_matrix)
     second_matrix = utt.mustbe_numpy_matrix(second_matrix)
     assert utt.is_layout(first_matrix, "row_major")
     assert utt.is_layout(second_matrix, "row_major")
     assert first_matrix.shape == second_matrix.shape
     assert first_matrix.dtype == second_matrix.dtype
 
+    is_single_row = first_matrix.shape[0] == 1
+    if is_single_row:
+        first_matrix = np.vstack([first_matrix, first_matrix])
+        second_matrix = np.vstack([second_matrix, second_matrix])
+
     extension_name = f"pairs_correlate_dense_{first_matrix.dtype}_t"
     result = np.empty(first_matrix.shape[0], dtype="float32")
     extension = getattr(xt, extension_name)
     extension(first_matrix, second_matrix, result)
+
+    if is_single_row:
+        result = result[[0]]
+
     return result
 
 
 @utm.timed_call()
 def logistics(matrix: utt.NumpyMatrix, *, location: float, slope: float, per: Optional[str]) -> utt.NumpyMatrix:
     """
     Compute a matrix of distances between each pair of rows in a dense (float or double) matrix
@@ -648,33 +701,33 @@
       that is, the zeros will be given a value this much smaller than the minimal "real" log value.
 
     .. note::
 
         The result is always dense, as even for sparse data, the log is rarely zero.
     """
     dense: np.ndarray
-    if shaped.ndim == 1:
+    if shaped.ndim == 1:  # type: ignore
         dense = utt.to_numpy_vector(shaped, copy=True)
     else:
         dense = utt.to_numpy_matrix(shaped, copy=True)  # type: ignore
 
     if normalization > 0:
         dense += normalization
     else:
         where = dense > 0
         if normalization < 0:
             dense[~where] = np.min(dense[where])
 
     if base is None:
         log_function = np.log
     elif base == 2:
-        log_function = np.log2
+        log_function = np.log2  # type: ignore
         base = None
     elif base == 10:
-        log_function = np.log10
+        log_function = np.log10  # type: ignore
         base = None
     else:
         assert base > 0
         log_function = np.log
 
     if normalization == 0:
         log_function(dense, out=dense, where=where)
@@ -693,47 +746,51 @@
 
 @utm.timed_call()
 @utd.expand_doc()
 def downsample_matrix(
     matrix: utt.Matrix,
     *,
     per: str,
-    samples: int,
+    samples: Union[int, utt.Vector],
     eliminate_zeros: bool = True,
     inplace: bool = False,
-    random_seed: int = 0,
+    random_seed: int,
 ) -> utt.ProperMatrix:
     """
     Downsample the data ``per`` (one of ``row`` and ``column``) such that the sum of each one
     becomes ``samples``.
 
     If the matrix is sparse, and ``eliminate_zeros`` (default: {eliminate_zeros}), then perform a
     final phase of eliminating leftover zero values from the compressed format. This means the
     result will be in "canonical format" so further ``scipy`` sparse operations on it will be
     faster.
 
     If ``inplace`` (default: {inplace}), modify the matrix in-place, otherwise, return a modified
     copy.
 
-    A non-zero ``random_seed`` (default: {random_seed}) will make the operation replicable.
+    A non-zero ``random_seed`` will make the operation replicable.
     """
     assert per in ("row", "column")
-    assert samples > 0
+    if isinstance(samples, (int, float)):
+        samples = np.full(matrix.shape[0], samples, dtype="int32")
+    else:
+        assert len(samples) == matrix.shape[0]
+        samples = utt.to_numpy_vector(samples).astype("int32")
 
     _, dense, compressed = utt.to_proper_matrices(matrix)
 
     if dense is not None:
         return _downsample_dense_matrix(dense, per, samples, inplace, random_seed)
 
     assert compressed is not None
     return _downsample_compressed_matrix(compressed, per, samples, eliminate_zeros, inplace, random_seed)
 
 
 def _downsample_dense_matrix(
-    matrix: utt.NumpyMatrix, per: str, samples: int, inplace: bool, random_seed: int
+    matrix: utt.NumpyMatrix, per: str, samples: utt.NumpyVector, inplace: bool, random_seed: int
 ) -> utt.NumpyMatrix:
     if inplace:
         output = matrix
     elif per == "row":
         output = np.empty(matrix.shape, dtype=matrix.dtype, order="C")
     else:
         output = np.empty(matrix.shape, dtype=matrix.dtype, order="F")
@@ -772,32 +829,37 @@
 
     if results_count == 1:
         input_array = utt.to_numpy_vector(matrix)
         output_array = utt.to_numpy_vector(output)
         extension_name = f"downsample_array_{input_array.dtype}_t_{output_array.dtype}_t"
         extension = getattr(xt, extension_name)
         with utm.timed_step("extensions.downsample_array"):
-            utm.timed_parameters(elements=input_array.size, samples=samples)
+            utm.timed_parameters(elements=input_array.size, samples=np.mean(samples))
             extension(input_array, output_array, samples, random_seed)
     else:
         extension_name = f"downsample_dense_{matrix.dtype}_t_{output.dtype}_t"
         extension = getattr(xt, extension_name)
         with utm.timed_step("extensions.downsample_dense_matrix"):
-            utm.timed_parameters(results=results_count, elements=elements_count, samples=samples)
+            utm.timed_parameters(results=results_count, elements=elements_count, samples=np.mean(samples))
             extension(matrix, output, samples, random_seed)
 
     if per == "column":
         output = np.transpose(output)
 
     assert output.shape == matrix.shape
     return output
 
 
 def _downsample_compressed_matrix(
-    matrix: utt.CompressedMatrix, per: str, samples: int, eliminate_zeros: bool, inplace: bool, random_seed: int
+    matrix: utt.CompressedMatrix,
+    per: str,
+    samples: utt.NumpyVector,
+    eliminate_zeros: bool,
+    inplace: bool,
+    random_seed: int,
 ) -> utt.CompressedMatrix:
     axis = utt.PER_OF_AXIS.index(per)
     results_count = matrix.shape[axis]
     elements_count = matrix.shape[1 - axis]
 
     axis_format = ("csr", "csc")[axis]
     if matrix.getformat() != axis_format:
@@ -823,41 +885,44 @@
         output.data.dtype,
     )
     extension = getattr(xt, extension_name)
 
     assert results_count == matrix.indptr.size - 1
 
     with utm.timed_step("extensions.downsample_sparse_matrix"):
-        utm.timed_parameters(results=results_count, elements=elements_count, samples=samples)
+        utm.timed_parameters(results=results_count, elements=elements_count, samples=np.mean(samples))
         extension(matrix.data, matrix.indptr, output.data, samples, random_seed)
 
     if eliminate_zeros:
         utt.eliminate_zeros(output)
 
     return output
 
 
 @utm.timed_call()
 @utd.expand_doc(data_types=",".join([f"``{data_type}``" for data_type in utt.CPP_DATA_TYPES]))
 def downsample_vector(
-    vector: utt.Vector, samples: int, *, output: Optional[utt.NumpyVector] = None, random_seed: int = 0
+    vector: utt.Vector,
+    samples: int,
+    *,
+    output: Optional[utt.NumpyVector] = None,
+    random_seed: int,
 ) -> None:
     """
     Downsample a vector of sample counters.
 
     **Input**
 
     * A numpy ``vector`` containing non-negative integer sample counts.
 
     * A desired total number of ``samples``.
 
     * An optional numpy array ``output`` to hold the results (otherwise, the input is overwritten).
 
-    * A ``random_seed`` (default: {random_seed}) which, if non-zero, will make the operation
-      replicable.
+    * A ``random_seed`` (non-zero for reproducible results).
 
     The arrays may have any of the data types: {data_types}.
 
     **Operation**
 
     If the total number of samples (sum of the array) is not higher than the required number of
     samples, the output is identical to the input.
@@ -944,14 +1009,56 @@
             rows_auroc,
         )
 
     return (rows_folds, rows_auroc)
 
 
 @utm.timed_call()
+def median_per(matrix: utt.Matrix, *, per: Optional[str]) -> utt.NumpyVector:
+    """
+    Compute the mean value ``per`` (``row`` or ``column``) of some ``matrix``.
+
+    If ``per`` is ``None``, the matrix must be square and is assumed to be symmetric, so the most
+    efficient direction is used based on the matrix layout. Otherwise it must be one of ``row`` or
+    ``column``, and the matrix must be in the appropriate layout (``row_major`` operating on rows,
+    ``column_major`` for operating on columns).
+    """
+    per = _ensure_per_for("median", matrix, per)
+    axis = 1 - utt.PER_OF_AXIS.index(per)
+
+    sparse = utt.maybe_sparse_matrix(matrix)
+    if sparse is not None:
+        return _reduce_matrix("median", sparse, per, lambda sparse: _median_sparse(sparse, per))  # type: ignore
+
+    dense = utt.to_numpy_matrix(matrix, only_extract=True)
+    return _reduce_matrix("median", dense, per, lambda dense: np.median(dense, axis=axis))
+
+
+@utm.timed_call()
+def _median_sparse(sparse: utt.SparseMatrix, per: str) -> utt.NumpyVector:
+    """
+    Compute the median for each row or column of a sparse matrix.
+    """
+    if per == "row":
+        assert sparse.getformat() == "csr"
+    else:
+        assert sparse.getformat() == "csc"
+    axis = utt.PER_OF_AXIS.index(per)
+    output = np.empty(sparse.shape[axis], dtype=sparse.dtype)  # type: ignore
+    extension_name = "median_compressed_%s_t_%s_t_%s_t" % (  # pylint: disable=consider-using-f-string
+        sparse.data.dtype,  # type: ignore
+        sparse.indices.dtype,  # type: ignore
+        sparse.indptr.dtype,  # type: ignore
+    )
+    extension = getattr(xt, extension_name)
+    extension(sparse.data, sparse.indices, sparse.indptr, sparse.shape[1 - axis], output)  # type: ignore
+    return output
+
+
+@utm.timed_call()
 def mean_per(matrix: utt.Matrix, *, per: Optional[str]) -> utt.NumpyVector:
     """
     Compute the mean value ``per`` (``row`` or ``column``) of some ``matrix``.
 
     If ``per`` is ``None``, the matrix must be square and is assumed to be symmetric, so the most
     efficient direction is used based on the matrix layout. Otherwise it must be one of ``row`` or
     ``column``, and the matrix must be in the appropriate layout (``row_major`` operating on rows,
@@ -978,14 +1085,33 @@
 
     with catch_warnings():
         filterwarnings("ignore", r"All-NaN (slice|axis) encountered")
         return _reduce_matrix("nanmean", dense, per, lambda dense: np.nanmean(dense, axis=1 - axis))
 
 
 @utm.timed_call()
+def geomean_per(matrix: utt.NumpyMatrix, *, per: Optional[str]) -> utt.NumpyVector:
+    """
+    Compute the geometric mean value ``per`` (``row`` or ``column``) of some (dense) ``matrix`` (of non-zero values).
+
+    If ``per`` is ``None``, the matrix must be square and is assumed to be symmetric, so the most efficient direction is
+    used based on the matrix layout. Otherwise it must be one of ``row`` or ``column``, and the matrix must be in the
+    appropriate layout (``row_major`` operating on rows, ``column_major`` for operating on columns).
+    """
+    per = _ensure_per_for("geomean", matrix, per)
+    axis = utt.PER_OF_AXIS.index(per)
+
+    sparse = utt.maybe_sparse_matrix(matrix)
+    assert sparse is None
+
+    dense = utt.to_numpy_matrix(matrix, only_extract=True)
+    return _reduce_matrix("geomean", dense, per, lambda dense: ss.mstats.gmean(dense, axis=1 - axis))
+
+
+@utm.timed_call()
 def max_per(matrix: utt.Matrix, *, per: Optional[str]) -> utt.NumpyVector:
     """
     Compute the maximal value ``per`` (``row`` or ``column``) of some ``matrix``.
 
     If ``per`` is ``None``, the matrix must be square and is assumed to be symmetric, so the most
     efficient direction is used based on the matrix layout. Otherwise it must be one of ``row`` or
     ``column``, and the matrix must be in the appropriate layout (``row_major`` operating on rows,
@@ -1374,14 +1500,30 @@
     ``column_major`` for operating on columns).
     """
     total_per_element = sum_per(matrix, per=per)
     return total_per_element / total_per_element.sum()
 
 
 @utm.timed_call()
+def stdev_per(matrix: utt.Matrix, *, per: Optional[str]) -> utt.NumpyVector:
+    """
+    Get the standard deviantion ``per`` (``row`` or ``column``) of some ``matrix``.
+
+    If ``per`` is ``None``, the matrix must be square and is assumed to be symmetric, so the most
+    efficient direction is used based on the matrix layout. Otherwise it must be one of ``row`` or
+    ``column``, and the matrix must be in the appropriate layout (``row_major`` operating on rows,
+    ``column_major`` for operating on columns).
+    """
+    per = _ensure_per_for("stdev", matrix, per)
+    result = variance_per(matrix, per=per)
+    np.sqrt(result, out=result)
+    return result
+
+
+@utm.timed_call()
 def variance_per(matrix: utt.Matrix, *, per: Optional[str]) -> utt.NumpyVector:
     """
     Get the variance ``per`` (``row`` or ``column``) of some ``matrix``.
 
     If ``per`` is ``None``, the matrix must be square and is assumed to be symmetric, so the most
     efficient direction is used based on the matrix layout. Otherwise it must be one of ``row`` or
     ``column``, and the matrix must be in the appropriate layout (``row_major`` operating on rows,
@@ -1392,14 +1534,15 @@
     sum_squared_per_element = sum_squared_per(matrix, per=per)
     axis = 1 - utt.PER_OF_AXIS.index(per)
     size = matrix.shape[axis]
     result = np.square(sum_per_element).astype(float)
     result /= -size
     result += sum_squared_per_element
     result /= size
+    result[result < 0] = 0
     return result
 
 
 @utm.timed_call()
 def normalized_variance_per(matrix: utt.Matrix, *, per: Optional[str], zero_value: float = 1.0) -> utt.NumpyVector:
     """
     Get the normalized variance (variance / mean) ``per`` (``row`` or ``column``) of some ``matrix``.
@@ -1481,23 +1624,23 @@
 
 
 @utm.timed_call()
 def max_matrix(matrix: utt.Matrix) -> Any:
     """
     Compute the maximum of all the values in a ``matrix``.
     """
-    return np.max(matrix)
+    return np.max(matrix)  # type: ignore
 
 
 @utm.timed_call()
 def min_matrix(matrix: utt.Matrix) -> Any:
     """
     Compute the minimum of all the values in a ``matrix``.
     """
-    return np.min(matrix)
+    return np.min(matrix)  # type: ignore
 
 
 @utm.timed_call()
 def nanmean_matrix(matrix: utt.Matrix) -> Any:
     """
     Compute the mean of all the non-NaN values in a ``matrix``.
     """
@@ -1517,30 +1660,30 @@
     Compute the maximum of all the non-NaN values in a ``matrix``.
     """
     with catch_warnings():
         filterwarnings("ignore", r"All-NaN (slice|axis) encountered")
 
         _, dense, compressed = utt.to_proper_matrices(matrix)
         if compressed is not None:
-            return np.nanmax(dense)
+            return np.nanmax(dense)  # type: ignore
         assert dense is not None
         return np.nanmax(dense)
 
 
 @utm.timed_call()
 def nanmin_matrix(matrix: utt.Matrix) -> Any:
     """
     Compute the minimum of all the non-NaN values in a ``matrix``.
     """
     with catch_warnings():
         filterwarnings("ignore", r"All-NaN (slice|axis) encountered")
 
         _, dense, compressed = utt.to_proper_matrices(matrix)
         if compressed is not None:
-            return np.nanmin(dense)
+            return np.nanmin(dense)  # type: ignore
         assert dense is not None
         return np.nanmin(dense)
 
 
 @utm.timed_call()
 def rank_matrix_by_layout(matrix: utt.NumpyMatrix, ascending: bool) -> Any:
     """
@@ -1566,37 +1709,33 @@
     per: str,
     reducer: Callable[[M], utt.NumpyVector],
 ) -> utt.NumpyVector:
     assert matrix.ndim == 2
     axis = utt.PER_OF_AXIS.index(per)
     results_count = matrix.shape[1 - axis]
 
-    compressed = utt.maybe_compressed_matrix(matrix)
-    if compressed is None:
-        timed_step = ".sparse"
-        elements_count: float = matrix.shape[axis]
-    else:
-        _, dense, compressed = utt.to_proper_matrices(matrix, default_layout=utt.LAYOUT_OF_AXIS[axis])
-
-        if dense is not None:
-            elements_count = dense.shape[axis]
-            axis_flag = (dense.flags.c_contiguous, dense.flags.f_contiguous)[axis]
-            if axis_flag:
-                timed_step = ".dense-efficient"
-            else:
-                timed_step = ".dense-inefficient"
+    _, dense, compressed = utt.to_proper_matrices(matrix, default_layout=utt.LAYOUT_OF_AXIS[axis])
 
+    elements_count: float
+    if dense is not None:
+        elements_count = dense.shape[axis]
+        axis_flag = (dense.flags.c_contiguous, dense.flags.f_contiguous)[axis]
+        if axis_flag:
+            timed_step = ".dense-efficient"
         else:
-            assert compressed is not None
-            elements_count = compressed.nnz / results_count
-            axis_format = ("csr", "csc")[axis]
-            if compressed.getformat() == axis_format:
-                timed_step = ".compressed-efficient"
-            else:
-                timed_step = ".compressed-inefficient"
+            timed_step = ".dense-inefficient"
+
+    else:
+        assert compressed is not None
+        elements_count = compressed.nnz / results_count
+        axis_format = ("csr", "csc")[axis]
+        if compressed.getformat() == axis_format:
+            timed_step = ".compressed-efficient"
+        else:
+            timed_step = ".compressed-inefficient"
 
     with utm.timed_step(timed_step):
         utm.timed_parameters(results=results_count, elements=elements_count)
         return utt.to_numpy_vector(reducer(matrix))
 
 
 @utm.timed_call()
@@ -1614,33 +1753,58 @@
     return result
 
 
 @utm.timed_call()
 def most_frequent(vector: utt.Vector) -> Any:
     """
     Return the most frequent value in a ``vector``.
+
+    This is useful for :py:func:`metacells.tools.convey.convey_obs_to_group`.
     """
     unique, positions = np.unique(utt.to_numpy_vector(vector), return_inverse=True)
     counts = np.bincount(positions)
     maxpos = np.argmax(counts)
     return unique[maxpos]
 
 
 @utm.timed_call()
+def strongest(vector: utt.Vector) -> Any:
+    """
+    Return the strongest (maximal absolute) value in a ``vector``.
+
+    This is useful for :py:func:`metacells.tools.convey.convey_obs_to_group`.
+    """
+    vector = utt.to_numpy_vector(vector)
+    return vector[np.argmax(np.abs(vector))]
+
+
+@utm.timed_call()
 def highest_weight(weights: utt.Vector, vector: utt.Vector) -> Any:
     """
-    Return the value with the highest total ``weight`` in a ``vector``.
+    Return the value with the highest total ``weights`` in a ``vector``.
+
+    This is useful for :py:func:`metacells.tools.project.convey_atlas_to_query`.
     """
     unique, positions = np.unique(utt.to_numpy_vector(vector), return_inverse=True)
-    counts = np.bincount(positions, weights=weights)
+    counts = np.bincount(positions, weights=weights)  # type: ignore
     maxpos = np.argmax(counts)
     return unique[maxpos]
 
 
 @utm.timed_call()
+def weighted_mean(weights: utt.Vector, vector: utt.Vector) -> Any:
+    """
+    Return the weighted mean (using the ``weights`` and the values in the ``vector``).
+
+    This is useful for :py:func:`metacells.tools.project.convey_atlas_to_query`.
+    """
+    return np.average(vector, weights=weights)  # type: ignore
+
+
+@utm.timed_call()
 def fraction_of_grouped(value: Any) -> Callable[[utt.Vector], Any]:
     """
     Return a function, that takes a vector and returns the fraction of elements of the vector which
     are equal to a specific ``value``.
     """
 
     def compute(vector: utt.Vector) -> Any:
@@ -1693,15 +1857,15 @@
     if window_size % 2 == 0:
         window_size += 1
     half_window_size = (window_size - 1) // 2
 
     utm.timed_parameters(function=function, size=dense.size, window=window_size)
 
     if window_size >= len(vector):
-        value = FULL_FUNCTIONS[function](vector)
+        value = FULL_FUNCTIONS[function](vector)  # type: ignore
         return np.full(len(vector), value)
 
     if order_by is not None:
         assert dense.size == order_by.size
         order_indices = np.argsort(order_by)
         reverse_order_indices = np.argsort(order_indices)
     else:
@@ -1742,22 +1906,26 @@
     If ``invert`` (default: {invert}), invert the mask.
     """
     if isinstance(patterns, (str, Pattern)):
         patterns = [patterns]
 
     utm.timed_parameters(patterns=len(patterns), strings=len(strings))
 
-    unified_pattern = (
-        "("
-        + ")|(".join([alternative if isinstance(alternative, str) else alternative.pattern for alternative in patterns])
-        + ")"
-    )
-    pattern: Pattern = re.compile(unified_pattern, re.IGNORECASE)
-
-    mask = np.array([bool(pattern.match(string)) for string in strings])
+    if len(patterns) == 0:
+        mask = np.full(len(strings), False, dtype="bool")
+    else:
+        unified_pattern = (
+            "("
+            + ")|(".join(
+                [alternative if isinstance(alternative, str) else alternative.pattern for alternative in patterns]
+            )
+            + ")"
+        )
+        pattern: Pattern = re.compile(unified_pattern, re.IGNORECASE)
+        mask = np.array([bool(pattern.fullmatch(string)) for string in strings])
 
     if invert:
         mask = ~mask
 
     return mask
 
 
@@ -1765,17 +1933,18 @@
 def compress_indices(indices: utt.Vector) -> utt.NumpyVector:
     """
     Given a vector of group ``indices`` per element, return a vector where the group indices are
     consecutive.
 
     If the group indices contain ``-1`` ("outliers"), then it is preserved as ``-1`` in the result.
     """
+    indices = utt.to_numpy_vector(indices)
     unique, consecutive = np.unique(indices, return_inverse=True)
     consecutive += min(unique[0], 0)
-    return consecutive
+    return consecutive.astype(indices.dtype)
 
 
 @utm.timed_call()
 def bin_pack(element_sizes: utt.Vector, max_bin_size: float) -> utt.NumpyVector:
     """
     Given a vector of ``element_sizes`` return a vector containing the bin number for each element,
     such that the total size of each bin is at most, and as close to as possible, to the
@@ -1812,23 +1981,23 @@
             if element_size > max_bin_size:
                 continue
 
             current_bin_index = bin_of_elements[element_index]
 
             current_bin_space = max_bin_size - size_of_bins[current_bin_index]
             assert current_bin_space >= 0
-            remove_loss = (element_size + current_bin_space) ** 2 - current_bin_space ** 2
+            remove_loss = (element_size + current_bin_space) ** 2 - current_bin_space**2
 
             for bin_index in range(len(size_of_bins)):  # pylint: disable=consider-using-enumerate
                 if bin_index == current_bin_index:
                     continue
                 bin_space = max_bin_size - size_of_bins[bin_index]
                 if bin_space < element_size:
                     continue
-                insert_gain = bin_space ** 2 - (bin_space - element_size) ** 2
+                insert_gain = bin_space**2 - (bin_space - element_size) ** 2
                 if insert_gain > remove_loss:
                     size_of_bins[current_bin_index] -= element_size
                     current_bin_index = bin_of_elements[element_index] = bin_index
                     size_of_bins[bin_index] += element_size
                     remove_loss = insert_gain
                     did_improve = True
 
@@ -1904,48 +2073,54 @@
             current_bin_index = bin_of_elements[element_index]
             current_bin_waste = size_of_bins[current_bin_index] - min_bin_size
             assert current_bin_waste >= 0
 
             if current_bin_waste < element_size:
                 continue
 
-            remove_gain = current_bin_waste ** 2 - (current_bin_waste - element_size) ** 2
+            remove_gain = current_bin_waste**2 - (current_bin_waste - element_size) ** 2
 
             for bin_index in range(len(size_of_bins)):  # pylint: disable=consider-using-enumerate
                 if bin_index == current_bin_index:
                     continue
                 bin_waste = size_of_bins[bin_index] - min_bin_size
-                insert_loss = (bin_waste + element_size) ** 2 - bin_waste ** 2
+                insert_loss = (bin_waste + element_size) ** 2 - bin_waste**2
                 if insert_loss < remove_gain:
                     size_of_bins[current_bin_index] -= element_size
                     current_bin_index = bin_of_elements[element_index] = bin_index
                     size_of_bins[bin_index] += element_size
                     remove_gain = insert_loss
                     did_improve = True
 
     utm.timed_parameters(elements=element_sizes.size, bins=len(size_of_bins))
     return bin_of_elements
 
 
 @utm.timed_call()
 def sum_groups(
-    matrix: utt.ProperMatrix, groups: utt.Vector, *, per: Optional[str]
-) -> Optional[Tuple[utt.Matrix, utt.NumpyVector]]:
+    matrix: utt.ProperMatrix,
+    groups: utt.Vector,
+    *,
+    per: Optional[str],
+    transform: Optional[Callable[[utt.Matrix], utt.Matrix]] = None,
+) -> Optional[Tuple[utt.NumpyMatrix, utt.NumpyVector]]:
     """
     Given a ``matrix``, and a vector of ``groups`` ``per`` column or row, return a matrix with a
     column or row ``per`` group, containing the sum of the groups columns or rows, and a vector of
     sizes (the number of summed columns or rows) ``per`` group.
 
     Negative group indices ("outliers") are ignored and their data is not included in the result. If
     there are no non-negative group indices, returns ``None``.
 
     If ``per`` is ``None``, the matrix must be square and is assumed to be symmetric, so the most
     efficient direction is used based on the matrix layout. Otherwise it must be one of ``row`` or
     ``column``, and the matrix must be in the appropriate layout (``row_major`` operating on rows,
     ``column_major`` for operating on columns).
+
+    If ``transform`` is not ``None``, it is applied to the data before summing it.
     """
     per = _ensure_per_for("sum_groups", matrix, per)
 
     groups = utt.to_numpy_vector(groups)
     groups_count = np.max(groups) + 1
 
     if groups_count == 0:
@@ -1965,47 +2140,58 @@
             timed_step = ".dense-efficient"
         else:
             timed_step = ".dense-inefficient"
 
     if per == "column":
         matrix = matrix.transpose()
 
-    group_sizes = np.zeros(groups_count, dtype="int32")
-
     with utm.timed_step(timed_step):
         utm.timed_parameters(groups=groups_count, entities=matrix.shape[0], elements=matrix.shape[1])
-        results = np.empty((groups_count, matrix.shape[1]), dtype=utt.shaped_dtype(matrix))
 
-        for group_index in range(groups_count):
-            group_mask = groups == group_index
-            group_size = np.sum(group_mask)
-            assert group_size > 0
-            group_sizes[group_index] = group_size
-            group_matrix = matrix[group_mask, :]
-            results[group_index, :] = utt.to_numpy_vector(group_matrix.sum(axis=0))
+        @utm.timed_call()
+        def _sum_group(group_index: int) -> Tuple[utt.NumpyVector, int]:
+            with utl.log_step(
+                "- group",
+                group_index,
+                formatter=lambda group_index: utl.progress_description(groups_count, group_index, "group"),
+            ):
+                group_mask = groups == group_index
+                utl.log_calc("group_mask", group_mask)
+                group_matrix = matrix[group_mask, :]
+                if transform is not None:
+                    group_matrix = transform(group_matrix)
+                group_size = group_matrix.shape[0]
+                assert group_size > 0
+                group_sum = utt.to_numpy_vector(group_matrix.sum(axis=0))
+                utl.log_calc("group_sum", group_sum, formatter=utl.sizes_description)
+                return (group_sum, group_size)
+
+        results = utp.parallel_map(_sum_group, groups_count)
+        size_per_group = np.array([size_of_group for _, size_of_group in results])
+        sum_per_group = np.vstack([sum_of_group for sum_of_group, _ in results])
 
     if per == "column":
-        results = results.transpose()
-    return results, group_sizes
+        sum_per_group = sum_per_group.transpose()
+    return sum_per_group, size_per_group
 
 
 @utm.timed_call()
 def shuffle_matrix(
     matrix: utt.Matrix,
     *,
     per: str,
-    random_seed: int = 0,
+    random_seed: int,
 ) -> None:
     """
     Shuffle (in-place) the ``matrix`` data ``per`` column or row.
 
     The matrix must be in the appropriate layout (``row_major`` for shuffling data in each row,
     ``column_major`` for shuffling data in each column).
 
-    A non-zero ``random_seed`` (default: {random_seed}) will make the operation replicable.
+    A non-zero ``random_seed`` (non-zero for reproducible results) will make the operation replicable.
     """
     _ensure_layout_for("shuffle", matrix, per, allow_inefficient=False)
     axis = utt.PER_OF_AXIS.index(per)
 
     _, dense, compressed = utt.to_proper_matrices(matrix)
 
     if compressed is not None:
@@ -2039,21 +2225,22 @@
 @utd.expand_doc()
 def cover_coordinates(
     x_coordinates: utt.Vector,
     y_coordinates: utt.Vector,
     *,
     cover_fraction: float = 1 / 3,
     noise_fraction: float = 1.0,
-    random_seed: int = 0,
+    random_seed: int,
 ) -> Tuple[utt.NumpyVector, utt.NumpyVector]:
     """
     Given x/y coordinates of points, move them so that the total area covered by them is
     ``cover_fraction`` (default: {cover_fraction}) of the total area of their bounding box, assuming
     each has the diameter of their minimal distance. The points are jiggled around by the
-    ``noise_fraction`` of their minimal distance using the ``random_seed`` (default: {random_seed}).
+    ``noise_fraction`` of their minimal distance using the ``random_seed`` (non-zero for reproducible
+    results).
 
     Returns new x/y coordinates vectors.
     """
     x_coordinates = utt.to_numpy_vector(x_coordinates)
     y_coordinates = utt.to_numpy_vector(y_coordinates)
 
     points_count = len(x_coordinates)
@@ -2079,23 +2266,24 @@
 
 
 @utm.timed_call()
 def random_piles(
     elements_count: int,
     target_pile_size: int,
     *,
-    random_seed: int = 0,
+    random_seed: int,
 ) -> utt.NumpyVector:
     """
     Split ``elements_count`` elements into piles of a size roughly equal to ``target_pile_size``.
 
     Return a vector specifying the pile index of each element.
 
     Specify a non-zero ``random_seed`` to make this replicable.
     """
+    assert elements_count > 0
     assert target_pile_size > 0
     piles_count = elements_count / target_pile_size
 
     few_piles_count = max(floor(piles_count), 1)
     many_piles_count = ceil(piles_count)
 
     if few_piles_count == many_piles_count:
@@ -2131,37 +2319,14 @@
     assert pile_of_elements.size == elements_count
 
     np.random.seed(random_seed)
     return np.random.permutation(pile_of_elements)
 
 
 @utm.timed_call()
-def group_piles(
-    group_of_elements: utt.NumpyVector,
-    group_of_groups: utt.NumpyVector,
-) -> utt.NumpyVector:
-    """
-    Group some elements into piles after first grouping them, and then grouping the groups.
-
-    Given the ``group_of_elements`` and for each such group, its larger ``group_of_groups``, compute
-    the pile index of each element to be the group of the group it belongs to, and return a vector
-    of the pile index of each element.
-
-    .. note::
-
-        Neither the ``group_of_elements`` nor the ``group_of_groups`` may contain "iutliers", that
-        is, they must assign an valid group index to each element and group.
-    """
-    assert np.min(group_of_elements) == 0
-    assert np.min(group_of_groups) == 0
-    group_of_group_of_elements = group_of_groups[group_of_elements]
-    return group_of_group_of_elements
-
-
-@utm.timed_call()
 def represent(
     goal: utt.NumpyVector,
     basis: utt.NumpyMatrix,
 ) -> Optional[Tuple[float, utt.NumpyVector]]:
     """
     Represent a ``goal`` vector as a weighted average of the row vectors of some ``basis`` matrix.
 
@@ -2239,15 +2404,15 @@
     first_size = len(cut.partition[0])
     second_size = len(cut.partition[1])
     assert first_size + second_size == nodes_count
 
     cut_total_weight = 0.0
     first_total_weight = 0.0
     second_total_weight = 0.0
-    for ((source, target), weight) in zip(edges, weight_of_edges):
+    for (source, target), weight in zip(edges, weight_of_edges):
         if is_second[source]:
             if is_second[target]:
                 second_total_weight += weight
             else:
                 cut_total_weight += weight
         else:
             if is_second[target]:
@@ -2290,15 +2455,15 @@
     absolute values when comparing to the thresholds.
     """
     assert 0 <= min_entry_value <= min_column_max_value
 
     if abs_values:
         comparable = np.abs(full)  # type: ignore
     else:
-        comparable = full
+        comparable = full  # type: ignore
 
     max_per_column = max_per(comparable, per="column")
     low_columns = max_per_column < min_column_max_value
 
     sparse_comparable = utt.maybe_compressed_matrix(comparable)
     if sparse_comparable is None:
         low_entries = comparable < min_entry_value
```

### Comparing `metacells-0.8.0/metacells/utilities/documentation.py` & `metacells-0.9.0/metacells/utilities/documentation.py`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/metacells/utilities/logging.py` & `metacells-0.9.0/metacells/utilities/logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,21 +34,22 @@
 Accessing top-level data and invoking top-level operations is logged at the coarse logging levels,
 anything else is logged at the ``DEBUG`` level.
 
 To improve the log messages, we allow each ``AnnData`` object to have an optional name for logging
 (see :py:func:`metacells.utilities.annotation.set_name` and
 :py:func:`metacells.utilities.annotation.get_name`). Whenever a temporary ``AnnData`` data is
 created, its name is extended by some descriptive suffix, so we get names like
-``full.clean.feature`` to describe the feature data extracted out of the clean data extracted out of
+``full.clean.select`` to describe the data selected from the clean data extracted out of
 the full data.
 """
 
 import importlib
 import logging
 import sys
+import warnings
 from contextlib import contextmanager
 from datetime import datetime
 from functools import wraps
 from inspect import Parameter
 from inspect import signature
 from logging import DEBUG
 from logging import INFO
@@ -104,14 +105,24 @@
     "ratio_description",
     "progress_description",
     "fraction_description",
     "fold_description",
 ]
 
 
+warnings.filterwarnings(
+    "ignore", category=FutureWarning, message=r".*Reordering categories will always return a new Categorical object.*"
+)
+warnings.filterwarnings(
+    "ignore",
+    category=FutureWarning,
+    message=r".*is_categorical is deprecated and will be removed in a future version.*",
+)
+
+
 class SynchronizedLogger(Logger):
     """
     A logger that synchronizes between the sub-processes.
 
     This ensures logging does not get garbled when when using multi-processing
     (e.g., using :py:func:`metacells.utilities.parallel.parallel_map`).
     """
@@ -158,36 +169,36 @@
 
 class ShortLoggingFormatter(LoggingFormatter):
     """
     Provide short level names.
     """
 
     #: Map the long level names to the fixed-width short level names.
-    SHORT_LEVEL_NAMES = dict(
-        CRITICAL="CRT",
-        CRT="CRT",
-        ERROR="ERR",
-        ERR="ERR",
-        WARNING="WRN",
-        WRN="WRN",
-        INFO="INF",
-        INF="INF",
-        STEP="STP",
-        STP="STP",
-        PARAM="PRM",
-        PRM="PRM",
-        HINT="PRM",
-        HNT="PRM",
-        CALC="CLC",
-        CLC="CLC",
-        DEBUG="DBG",
-        DBG="DBG",
-        NOTSET="NOT",
-        NOT="NOT",
-    )
+    SHORT_LEVEL_NAMES = {
+        "CRITICAL": "CRT",
+        "CRT": "CRT",
+        "ERROR": "ERR",
+        "ERR": "ERR",
+        "WARNING": "WRN",
+        "WRN": "WRN",
+        "INFO": "INF",
+        "INF": "INF",
+        "STEP": "STP",
+        "STP": "STP",
+        "PARAM": "PRM",
+        "PRM": "PRM",
+        "HINT": "PRM",
+        "HNT": "PRM",
+        "CALC": "CLC",
+        "CLC": "CLC",
+        "DEBUG": "DBG",
+        "DBG": "DBG",
+        "NOTSET": "NOT",
+        "NOT": "NOT",
+    }
 
     def format(self, record: LogRecord) -> Any:
         record.levelname = self.SHORT_LEVEL_NAMES[record.levelname]
         return LoggingFormatter.format(self, record)
 
 
 # Global logger object.
@@ -330,18 +341,18 @@
         def wrapper(*args: Any, **kwargs: Any) -> Any:  # pylint: disable=too-many-branches
             global CALL_LEVEL
             global INDENT_LEVEL
             names, values = _collect_parameters(ordered_parameters, *args, **kwargs)
             adatas = _collect_adatas(values)
             new_adatas: List[AnnData] = []
 
-            try:
-                global IS_TOP_LEVEL
-                old_is_top_level = IS_TOP_LEVEL
+            global IS_TOP_LEVEL
+            old_is_top_level = IS_TOP_LEVEL
 
+            try:
                 for adata in adatas:
                     IS_TOP_LEVEL = False
                     if hasattr(adata, "__is_top_level__"):
                         IS_TOP_LEVEL = IS_TOP_LEVEL or getattr(adata, "__is_top_level__")
                     else:
                         IS_TOP_LEVEL = IS_TOP_LEVEL or CALL_LEVEL == 0
                         setattr(adata, "__is_top_level__", CALL_LEVEL == 0)
@@ -409,37 +420,45 @@
             adatas += _collect_adatas(value)
     return adatas
 
 
 def _format_value(  # pylint: disable=too-many-return-statements,too-many-branches
     value: Any, name: str, formatter: Optional[Callable[[Any], Any]] = None
 ) -> Optional[str]:
-    if isinstance(value, Parameter.empty.__class__):
+    if isinstance(value, Parameter.empty.__class__):  # type: ignore
         return None
 
     checksum = ""
     # if utt.is_1d(value) and 'U' not in str(value.dtype) and 'o' not in str(value.dtype):
     #    checksum = ' checksum: %.20e' % utt.shaped_checksum(value)
     # elif utt.is_2d(value):
     #    checksum = ' checksum: %.20e' % utt.shaped_checksum(value)
 
+    # import psutil
+    # vm = psutil.virtual_memory()
+    # used = int(round(vm.used / (1024 * 1024 * 1024)))
+    # avail = int(round(vm.available / (1024 * 1024 * 1024)))
+    # free = int(round(vm.free / (1024 * 1024 * 1024)))
+    # avail -= free
+    # checksum += f" (M: {used}U {avail}A {free}F)"
+
     if formatter is not None:
         value = formatter(value)
         if value is None:
             return None
 
     if isinstance(value, AnnData):
-        name = value.uns.get("__name__", "unnamed")
+        aname = value.uns.get("__name__", "unnamed")
 
         if hasattr(value.X, "dtype"):
             dtype = getattr(value.X, "dtype")
         else:
             dtype = "unknown"
 
-        return f"{name} annotated data with {value.shape[0]} X {value.shape[1]} {dtype}s" + checksum
+        return f"{aname} annotated data with {value.shape[0]} X {value.shape[1]} {dtype}s" + checksum
 
     if isinstance(value, (np.bool_, bool, str, None.__class__)):
         return str(value) + checksum
 
     if isinstance(value, (int, float, np.float32, np.float64, np.int32, np.int64)):
         value = float(value)
         if "random_seed" in name:
@@ -466,37 +485,42 @@
     ):
         return mask_description(value) + checksum
 
     if hasattr(value, "ndim"):
         if value.ndim == 2:
             text = f"{value.__class__.__name__} {value.shape[0]} X {value.shape[1]} {utt.shaped_dtype(value)}s"
             if hasattr(value, "nnz"):
-                text += f" ({value.nnz} > 0)"
+                percent = 100 * value.nnz / (value.shape[0] * value.shape[1])
+                text += f" ({value.nnz} > 0, {percent:.4g}%)"
             return text + checksum
 
         if value.ndim == 1:
             value = utt.to_numpy_vector(value)
-            if len(value) > 100:
+            if len(value) > 20:
                 text = f"{len(value)} {value.dtype}s"
                 return text + checksum
             value = list(value)
 
     if isinstance(value, list):
-        if len(value) > 100:
+        if len(value) > 20 or (len(value) > 0 and hasattr(value[0], "__len__") and not isinstance(value[0], str)):
             return f"{len(value)} {value[0].__class__.__name__}s" + checksum
         texts = [
             element.uns.get("__name__", "unnamed") if isinstance(element, AnnData) else str(element)
             for element in value
         ]
         return f'[ {", ".join(texts)} ]' + checksum
 
     if isinstance(value, dict):
+        values = list(value.values())
+        if len(values) > 20 or (len(values) > 0 and hasattr(values[0], "__len__") and not isinstance(values[0], str)):
+            keys = list(value.keys())
+            return f"dict {_format_value(keys, 'keys')} => {_format_value(values, 'values')}"
         return str(value) + checksum
 
-    raise RuntimeError(f"unknown parameter type: {value.__class__} value: {value}")  #
+    return f"{value.__class__.__module__}.{value.__class__.__qualname__}#{id(value)}"
 
 
 def top_level(adata: AnnData) -> None:
     """
     Indicate that the annotated data will be returned to the top-level caller, increasing its
     logging level.
     """
@@ -550,36 +574,45 @@
     try:
         yield
     finally:
         INDENT_LEVEL -= delta
 
 
 #: Convert ``per`` to the name of the ``AnnData`` data member holding it.
-MEMBER_OF_PER = dict(m="uns", o="obs", v="var", oo="obsp", vv="varp", oa="obsm", va="varm", vo="layers")
+MEMBER_OF_PER = {
+    "m": "uns",
+    "o": "obs",
+    "v": "var",
+    "oo": "obsp",
+    "vv": "varp",
+    "oa": "obsm",
+    "va": "varm",
+    "vo": "layers",
+}
 
 
 def incremental(adata: AnnData, per: str, name: str, formatter: Optional[Callable[[Any], Any]] = None) -> None:
     """
     Declare that the named annotation will be built incrementally - set and then repeatedly modified.
     """
     assert per in ("m", "v", "o", "vv", "oo", "vo", "va", "oa")
     if not hasattr(adata, "__incremental__"):
         setattr(adata, "__incremental__", {})
     by_name: Dict[str, Tuple[str, Optional[Callable[[Any], Any]]]] = getattr(adata, "__incremental__")
-    assert name not in by_name
+    # assert name not in by_name
     by_name[name] = (per, formatter)
 
 
 def done_incrementals(adata: AnnData) -> None:
     """
     Declare that all the incremental values have been fully computed.
     """
     assert hasattr(adata, "__incremental__")
     by_name: Dict[str, Tuple[str, Optional[Callable[[Any], Any]]]] = getattr(adata, "__incremental__")
-    setattr(adata, "__incremental__", [])
+    setattr(adata, "__incremental__", {})
 
     for name, (per, formatter) in by_name.items():
         if name == "__x__":
             value = adata.X
         else:
             annotation = getattr(adata, MEMBER_OF_PER[per])
             if name not in annotation:
@@ -626,15 +659,18 @@
     Log getting some annotated data.
     """
     assert per in ("m", "v", "o", "vv", "oo", "vo", "va", "oa")
 
     is_top_level = (
         hasattr(adata, "__is_top_level__")
         and getattr(adata, "__is_top_level__")
-        and (not hasattr(adata, "__incremental__") or name not in getattr(adata, "__incremental__"))
+        and (
+            not hasattr(adata, "__incremental__")
+            or (isinstance(name, str) and name not in getattr(adata, "__incremental__"))
+        )
     )
 
     adata_name = adata.uns.get("__name__", "unnamed")
     if isinstance(name, str) and name == "__x__":
         name = f"{adata_name}.X"
     else:
         member_name = MEMBER_OF_PER[per]
@@ -716,17 +752,20 @@
     groups_count = np.max(groups) + 1
     outliers_count = np.sum(groups < 0)
 
     if groups_count == 0:
         assert outliers_count == len(groups)
         return f"{len(groups)} {groups.dtype} elements with all outliers (100%)"
 
-    mean = (len(groups) - outliers_count) / groups_count
+    grouped_count = len(groups) - outliers_count
+    mean = grouped_count / groups_count
     return (
-        ratio_description(len(groups), f"{groups.dtype} element", outliers_count, "outliers")
+        ratio_description(len(groups), f"{groups.dtype} element", outliers_count, "outliers", base=False)
+        + " and "
+        + ratio_description(len(groups), f"{groups.dtype} element", grouped_count, "grouped")
         + f" with {groups_count} groups with mean size {mean:.4g}"
     )
 
 
 def mask_description(mask: Union[str, utt.Vector, utt.Matrix]) -> str:
     """
     Return a string for logging a boolean mask.
@@ -743,28 +782,30 @@
         return f"{mask.shape[0]} X {mask.shape[1]} " + ratio_description(
             mask.size, str(mask.dtype), np.sum(mask > 0), value
         )
 
     return ratio_description(mask.size, str(mask.dtype), np.sum(mask > 0), value)
 
 
-def ratio_description(denominator: float, element: str, numerator: float, condition: str) -> str:
+def ratio_description(denominator: float, element: str, numerator: float, condition: str, *, base: bool = True) -> str:
     """
     Return a string for describing a ratio (including a percent representation).
     """
     assert numerator >= 0
     assert denominator > 0
 
     if int(numerator) == numerator:
         numerator = int(numerator)
     if int(denominator) == denominator:
         denominator = int(denominator)
 
     percent = (numerator * 100) / denominator
-    return f"{numerator} {condition} ({percent:.4g}%) out of {denominator} {element}s"
+    if base:
+        return f"{numerator} {condition} ({percent:.4g}%) out of {denominator} {element}s"
+    return f"{numerator} {condition} ({percent:.4g}%)"
 
 
 def progress_description(amount: int, index: int, element: str) -> str:
     """
     Return a string for describing progress in a loop.
     """
     assert amount > 0
@@ -788,14 +829,14 @@
     """
     Return a string for describing a fraction (including a percent representation).
     """
     if fold is None:
         return "None"
 
     if fold >= 0:
-        value = 2 ** fold
+        value = 2**fold
         char = "X"
     else:
-        value = 2 ** -fold
+        value = 2**-fold
         char = "/"
 
     return f"{fold:.4g} ({char} {value:.4g})"
```

### Comparing `metacells-0.8.0/metacells/utilities/parallel.py` & `metacells-0.9.0/metacells/utilities/parallel.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
     Re-implement all the package in a single language more suitable for scientific computing. Julia
     is looking like a good combination of convenience and performance...
 """
 import ctypes
 import os
 import sys
+from math import ceil
 from multiprocessing import Value
 from multiprocessing import get_context
 from threading import current_thread
 from typing import Any
 from typing import Callable
 from typing import List
 from typing import Optional
@@ -123,14 +124,16 @@
     assert processors > 0
 
     global PROCESSORS_COUNT
     PROCESSORS_COUNT = processors
 
     threadpool_limits(limits=PROCESSORS_COUNT)
     xt.set_threads_count(PROCESSORS_COUNT)
+    os.environ["OMP_NUM_THREADS"] = str(PROCESSORS_COUNT)
+    os.environ["MKL_NUM_THREADS"] = str(PROCESSORS_COUNT)
 
 
 if "sphinx" not in sys.argv[0]:
     set_processors_count(int(os.environ.get("METACELLS_PROCESSORS_COUNT", "0")))
 
 
 def get_processors_count() -> int:
@@ -174,14 +177,17 @@
     it in increments of ``1/invocations``.
 
     .. todo::
 
         It is currently only possible to invoke :py:func:`parallel_map` from the main application thread (that is, it
         does not nest).
     """
+    if invocations == 0:
+        return []
+
     assert function.__is_timed__  # type: ignore
 
     global IS_MAIN_PROCESS
     assert IS_MAIN_PROCESS
 
     global PROCESSES_COUNT
     PROCESSES_COUNT = min(PROCESSORS_COUNT, invocations)
@@ -196,14 +202,18 @@
 
     global PARALLEL_FUNCTION
     assert PARALLEL_FUNCTION is None
 
     global MAP_INDEX
     MAP_INDEX += 1
 
+    num_threads = str(ceil(PROCESSES_COUNT / invocations))
+    os.environ["OMP_NUM_THREADS"] = num_threads
+    os.environ["MKL_NUM_THREADS"] = num_threads
+
     PARALLEL_FUNCTION = function
     IS_MAIN_PROCESS = None
     try:
         results: List[Optional[T]] = [None] * invocations
         utm.flush_timing()
         with utm.timed_step("parallel_map"):
             utm.timed_parameters(index=MAP_INDEX, processes=PROCESSES_COUNT)
@@ -212,14 +222,16 @@
                     if utp.has_progress_bar() and not hide_from_progress_bar:
                         utp.did_progress(1 / invocations)
                     results[index] = result
         return results  # type: ignore
     finally:
         IS_MAIN_PROCESS = True
         PARALLEL_FUNCTION = None
+        os.environ["OMP_NUM_THREADS"] = str(PROCESSES_COUNT)
+        os.environ["MKL_NUM_THREADS"] = str(PROCESSES_COUNT)
 
 
 def _invocation(index: int) -> Tuple[int, Any]:
     global IS_MAIN_PROCESS
     if IS_MAIN_PROCESS is None:
         IS_MAIN_PROCESS = os.getpid() == MAIN_PROCESS_PID
         assert not IS_MAIN_PROCESS
@@ -237,10 +249,13 @@
         stop_processor_index = int(round(PROCESSORS_COUNT * (PROCESS_INDEX + 1) / PROCESSES_COUNT))
         PROCESSORS_COUNT = stop_processor_index - start_processor_index
 
         assert PROCESSORS_COUNT > 0
         utl.logger().debug("PROCESSORS: %s", PROCESSORS_COUNT)
         threadpool_limits(limits=PROCESSORS_COUNT)
         xt.set_threads_count(PROCESSORS_COUNT)
+        os.environ["OMP_NUM_THREADS"] = str(PROCESSORS_COUNT)
+        os.environ["MKL_NUM_THREADS"] = str(PROCESSORS_COUNT)
 
     assert PARALLEL_FUNCTION is not None
-    return index, PARALLEL_FUNCTION(index)
+    result = PARALLEL_FUNCTION(index)
+    return index, result
```

### Comparing `metacells-0.8.0/metacells/utilities/progress.py` & `metacells-0.9.0/metacells/utilities/progress.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,18 +110,17 @@
 def progress_bar_slice(fraction: Optional[float]) -> Any:
     """
     Run some code which will use a slice of the current progress bar.
 
     This can be nested to split the overall progress bar into smaller and smaller parts to represent a tree of
     computations.
 
-    If ``fraction`` is None and there is no active progress bar, simply runs the code.
+    If ``fraction`` is None, or there is no active progress bar, simply runs the code.
     """
     _show_progress_bar()
-    assert (fraction is not None) == has_progress_bar()
     if fraction is None:
         result = yield None
         return result
 
     old_state = start_progress_bar_slice(fraction)
     try:
         result = yield None
@@ -134,26 +133,32 @@
     """
     Start a nested slice of the overall progress bar.
 
     Returned the captured state that needs to be passed to ``end_progress_bar_slice``.
     """
     assert PROGRESS_BAR is not None
     assert TQDM_KWARGS is None
-    assert 0.0 < fraction < 1.0
+    assert 0.0 < fraction <= 1.0, f"invalid progress fraction: {fraction} (1 + {fraction - 1})"
 
     global PROGRESS_END
     global PROGRESS_SIZE
 
     old_progress_size = PROGRESS_SIZE
-    PROGRESS_SIZE = int(round(PROGRESS_SIZE * fraction))
-    assert 0 < PROGRESS_SIZE < old_progress_size
-
     old_progress_end = PROGRESS_END
+
+    PROGRESS_SIZE = int(PROGRESS_SIZE * fraction)
     PROGRESS_END = PROGRESS_POSITION + PROGRESS_SIZE
-    assert PROGRESS_END <= old_progress_end
+
+    assert (
+        0 < PROGRESS_SIZE <= old_progress_size
+    ), f"invalid progress size: {PROGRESS_SIZE} ({old_progress_size} + {PROGRESS_SIZE - old_progress_size})"
+
+    assert (
+        PROGRESS_END <= old_progress_end
+    ), f"invalid progress end: {PROGRESS_END} ({old_progress_end} + {PROGRESS_END - old_progress_end})"
 
     return old_progress_size, old_progress_end
 
 
 def end_progress_bar_slice(old_state: Tuple[int, int]) -> None:
     """
     End a nested slice of the overall progress bar.
@@ -179,21 +184,21 @@
 
 
 def did_progress(fraction: float) -> Any:
     """
     Report progress of some fraction of the current (slice of) progress bar.
     """
     _show_progress_bar()
-    assert 0 < fraction <= 1.0
+    assert 0.0 < fraction <= 1.0, f"invalid progress fraction: {fraction} (1 + {fraction - 1})"
     assert PROGRESS_BAR is not None
     assert TQDM_KWARGS is None
 
     global PROGRESS_POSITION
 
-    step = int(round(PROGRESS_SIZE * fraction))
+    step = int(PROGRESS_SIZE * fraction)
     step = min(step, PROGRESS_END - PROGRESS_POSITION)
 
     if step > 0:
         PROGRESS_BAR.update(step)
         PROGRESS_POSITION += step
```

### Comparing `metacells-0.8.0/metacells/utilities/timing.py` & `metacells-0.9.0/metacells/utilities/timing.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,19 +322,19 @@
         name = f".{name[1:]}"
     if name[0] == ".":
         assert parent_timing is not None
 
     step_timing = StepTiming(name, parent_timing)
     steps_stack.append(step_timing)
 
-    try:
-        if LOG_ALL_STEPS:
-            utl.logger().debug(f"{{[( {step_timing.context}")  # pylint: disable=logging-fstring-interpolation
+    if LOG_ALL_STEPS:
+        utl.logger().debug(f"{{[( {step_timing.context}")  # pylint: disable=logging-fstring-interpolation
 
-        yield_point = Counters.now()
+    yield_point = Counters.now()
+    try:
         yield None
 
     finally:
         back_point = Counters.now()
         total_times = back_point - yield_point
 
         global GC_STEPS
```

### Comparing `metacells-0.8.0/metacells/utilities/typing.py` & `metacells-0.9.0/metacells/utilities/typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,15 +264,15 @@
     def eliminate_zeros(self) -> None:
         ...
 
     def sort_indices(self) -> None:
         ...
 
 
-class PandasIndex(ShapedProtocol, Collection, Sized, Protocol):  # pylint: disable=abstract-method
+class PandasIndex(ShapedProtocol, Collection, Sized, Protocol):
     """
     A ``mypy`` type for a pandas index.
     """
 
     values: NumpyVector
 
 
@@ -759,36 +759,36 @@
     elif is_1d(shaped):
         if isinstance(shaped, (pd.DataFrame, pd.Series, pd.core.indexes.base.Index)):
             shaped = shaped.values
 
         if isinstance(shaped, pd.core.arrays.categorical.Categorical):
             shaped = np.array(shaped)
 
-        dense = shaped  # type: ignore
+        dense = shaped
 
     else:
         assert is_2d(shaped)
         assert shaped.shape[0] == 1 or shaped.shape[1] == 1  # type: ignore
         dense = to_numpy_matrix(shaped, copy=copy, only_extract=only_extract)  # type: ignore
         dense = np.reshape(dense, -1)
 
     if copy and id(dense) == id(shaped):
         dense = np.copy(dense)
 
     return mustbe_numpy_vector(dense)
 
 
 #: Which flag indicates efficient 2D dense matrix layout.
-DENSE_FAST_FLAG = dict(column_major="F_CONTIGUOUS", row_major="C_CONTIGUOUS")
+DENSE_FAST_FLAG = {"column_major": "F_CONTIGUOUS", "row_major": "C_CONTIGUOUS"}
 
 #: Which format indicates efficient 2D sparse matrix layout.
-SPARSE_FAST_FORMAT = dict(column_major="csc", row_major="csr")
+SPARSE_FAST_FORMAT = {"column_major": "csc", "row_major": "csr"}
 
 #: Which format indicates inefficient 2D sparse matrix layout.
-SPARSE_SLOW_FORMAT = dict(column_major="csr", row_major="csc")
+SPARSE_SLOW_FORMAT = {"column_major": "csr", "row_major": "csc"}
 
 #: The layout by the ``axis`` parameter.
 LAYOUT_OF_AXIS = ("row_major", "column_major")
 
 #: When reducing data, get results ``per`` row or column (by the ``axis`` parameter).
 PER_OF_AXIS = ("row", "column")
 
@@ -806,15 +806,15 @@
         return True
 
     sparse = maybe_sparse_matrix(matrix)
     if sparse is not None:
         return sparse.getformat() == SPARSE_FAST_FORMAT[layout]
 
     dense = to_numpy_matrix(matrix, only_extract=True)
-    return dense.flags[DENSE_FAST_FLAG[layout]]
+    return dense.flags[DENSE_FAST_FLAG[layout]]  # type: ignore
 
 
 def shaped_dtype(shaped: Shaped) -> str:
     """
     Return the data type of the element of shaped data.
     """
     frame = maybe_pandas_frame(shaped)
@@ -849,15 +849,15 @@
         for layout, sparse_format in SPARSE_FAST_FORMAT.items():
             if sparse.getformat() == sparse_format:
                 return layout
         return None
 
     dense = to_numpy_matrix(matrix, only_extract=True)
     for layout, flag in DENSE_FAST_FLAG.items():
-        if dense.flags[flag]:
+        if dense.flags[flag]:  # type: ignore
             return layout
 
     return None
 
 
 def is_contiguous(vector: Vector) -> bool:
     """
```

### Comparing `metacells-0.8.0/metacells.egg-info/SOURCES.txt` & `metacells-0.9.0/metacells.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 metacells/choose_seeds.cpp
 metacells/correlate.cpp
 metacells/cover.cpp
 metacells/downsample.cpp
 metacells/extensions.cpp
 metacells/extensions.h
 metacells/folds.cpp
+metacells/gaps.cpp
 metacells/logistics.cpp
 metacells/parameters.py
 metacells/partitions.cpp
 metacells/prune_per.cpp
 metacells/py.typed
 metacells/rank.cpp
 metacells/relayout.cpp
@@ -30,42 +31,43 @@
 metacells.egg-info/PKG-INFO
 metacells.egg-info/SOURCES.txt
 metacells.egg-info/dependency_links.txt
 metacells.egg-info/entry_points.txt
 metacells.egg-info/requires.txt
 metacells.egg-info/top_level.txt
 metacells/pipeline/__init__.py
-metacells/pipeline/clean.py
 metacells/pipeline/collect.py
 metacells/pipeline/consistency.py
 metacells/pipeline/direct.py
 metacells/pipeline/divide_and_conquer.py
-metacells/pipeline/feature.py
+metacells/pipeline/exclude.py
+metacells/pipeline/mark.py
 metacells/pipeline/mcview.py
 metacells/pipeline/projection.py
 metacells/pipeline/related_genes.py
+metacells/pipeline/select.py
 metacells/pipeline/umap.py
 metacells/scripts/__init__.py
 metacells/scripts/timing.py
 metacells/tools/__init__.py
 metacells/tools/apply.py
+metacells/tools/bursty_lonely.py
 metacells/tools/candidates.py
 metacells/tools/convey.py
 metacells/tools/deviants.py
 metacells/tools/dissolve.py
 metacells/tools/distinct.py
 metacells/tools/downsample.py
 metacells/tools/filter.py
 metacells/tools/group.py
 metacells/tools/high.py
 metacells/tools/knn_graph.py
 metacells/tools/layout.py
 metacells/tools/mask.py
 metacells/tools/named.py
-metacells/tools/noisy_lonely.py
 metacells/tools/project.py
 metacells/tools/properly_sampled.py
 metacells/tools/quality.py
 metacells/tools/rare.py
 metacells/tools/similarity.py
 metacells/utilities/__init__.py
 metacells/utilities/annotation.py
```

### Comparing `metacells-0.8.0/pybind11/include/pybind11/attr.h` & `metacells-0.9.0/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/pybind11/include/pybind11/buffer_info.h` & `metacells-0.9.0/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/pybind11/include/pybind11/cast.h` & `metacells-0.9.0/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/pybind11/include/pybind11/chrono.h` & `metacells-0.9.0/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/pybind11/include/pybind11/complex.h` & `metacells-0.9.0/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/pybind11/include/pybind11/detail/class.h` & `metacells-0.9.0/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/pybind11/include/pybind11/detail/common.h` & `metacells-0.9.0/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/pybind11/include/pybind11/detail/descr.h` & `metacells-0.9.0/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/pybind11/include/pybind11/detail/init.h` & `metacells-0.9.0/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/pybind11/include/pybind11/detail/internals.h` & `metacells-0.9.0/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/pybind11/include/pybind11/detail/typeid.h` & `metacells-0.9.0/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/pybind11/include/pybind11/eigen.h` & `metacells-0.9.0/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/pybind11/include/pybind11/embed.h` & `metacells-0.9.0/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/pybind11/include/pybind11/eval.h` & `metacells-0.9.0/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/pybind11/include/pybind11/functional.h` & `metacells-0.9.0/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/pybind11/include/pybind11/iostream.h` & `metacells-0.9.0/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/pybind11/include/pybind11/numpy.h` & `metacells-0.9.0/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/pybind11/include/pybind11/operators.h` & `metacells-0.9.0/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/pybind11/include/pybind11/options.h` & `metacells-0.9.0/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/pybind11/include/pybind11/pybind11.h` & `metacells-0.9.0/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/pybind11/include/pybind11/pytypes.h` & `metacells-0.9.0/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/pybind11/include/pybind11/stl.h` & `metacells-0.9.0/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/pybind11/include/pybind11/stl_bind.h` & `metacells-0.9.0/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `metacells-0.8.0/setup.cfg` & `metacells-0.9.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.8.0
+current_version = 0.9.0-dev.1
 commit = True
 tag = True
 parse = 
 	(?P<major>\d+)
 	\.
 	(?P<minor>\d+)
 	\.
```

### Comparing `metacells-0.8.0/setup.py` & `metacells-0.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #!/usr/bin/env python
 
 import os
 import platform
 from setuptools import Extension, setup, find_packages
+from glob import glob
 
 if os.name == "nt":
     raise NotImplementedError(
         "Python metacells does not support native windows.\nInstead, "
         "install Windows Subsystem for Linux, and metacells within it."
     )
 
 DEFINE_MACROS = [("ASSERT_LEVEL", 1)]  # 0 for none, 1 for fast, 2 for slow.
 COMPILE_ARGS = [f"-I{os.getcwd()}", "-std=c++14"]
+# COMPILE_ARGS += ["-fsanitize=address", "-fno-omit-frame-pointer"]
 # COMPILE_ARGS += ["-fopt-info-vec-all", "-fopt-info-loop-optimized"]
 
 with open("metacells/should_check_avx2.py", "w") as file:
     file.write("# file generated by setup\n")
     file.write("# don't change, don't track in version control\n")
     if str(os.getenv("WHEEL", "")) == "":
         COMPILE_ARGS += ["-march=native", "-mtune=native"]
@@ -33,14 +35,16 @@
 with open("HISTORY.rst") as history_file:
     history = history_file.read()
 
 requirements = open("requirements.txt").read().split()
 test_requirements = open("requirements_test.txt").read().split()
 dev_requirements = open("requirements_dev.txt").read().split()
 
+packages = ['metacells'] + [sub_dir for sub_dir in glob('metacells/*') if '.' not in sub_dir and '__' not in sub_dir]
+
 setup(
     author="Oren Ben-Kiki",
     author_email="oren@ben-kiki.org",
     python_requires=">=3.7",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
@@ -64,14 +68,15 @@
                 "metacells/auroc.cpp",
                 "metacells/choose_seeds.cpp",
                 "metacells/correlate.cpp",
                 "metacells/cover.cpp",
                 "metacells/downsample.cpp",
                 "metacells/extensions.cpp",
                 "metacells/folds.cpp",
+                "metacells/gaps.cpp",
                 "metacells/logistics.cpp",
                 "metacells/partitions.cpp",
                 "metacells/prune_per.cpp",
                 "metacells/rank.cpp",
                 "metacells/relayout.cpp",
                 "metacells/shuffle.cpp",
                 "metacells/top_per.cpp",
@@ -88,14 +93,14 @@
     install_requires=requirements,
     license="MIT license",
     long_description=readme + "\n\n" + history,
     long_description_content_type="text/x-rst",
     include_package_data=True,
     keywords="metacells",
     name="metacells",
-    packages=find_packages(include=["metacells"]),
+    packages=packages,
     test_suite="tests",
     tests_require=test_requirements,
     extras_require={"dev": dev_requirements},
     url="https://github.com/tanaylab/metacells.git",
-    version="0.8.0",
+    version="0.9.0",
 )
```

### Comparing `metacells-0.8.0/tests/test_data.py` & `metacells-0.9.0/tests/test_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,52 +39,54 @@
     return adata, expected
 
 
 def test_find_rare_gene_modules() -> None:
     for path in glob("../metacells-test-data/*.h5ad"):
         adata, expected = _load(path)
 
+        mc.pl.mark_lateral_genes(adata, **expected.get("mark_lateral_genes", {}))
         mc.tl.find_rare_gene_modules(  #
             adata,
-            forbidden_gene_names=expected["compute_direct_metacells"]["forbidden_gene_names"],
+            reproducible=True,
             **expected.get("find_rare_gene_modules", {}),
         )
 
         actual_rare_gene_modules = []
         rare_gene_modules = mc.ut.get_v_numpy(adata, "rare_gene_module")
         max_gene_module = np.max(rare_gene_modules)
         for module_index in range(max_gene_module + 1):
             actual_rare_gene_modules.append(sorted(adata.var_names[rare_gene_modules == module_index]))
 
         expected_rare_gene_modules = expected["rare_gene_modules"]
-
         assert actual_rare_gene_modules == expected_rare_gene_modules
 
 
 def test_direct_pipeline() -> None:
     for path in glob("../metacells-test-data/*.h5ad"):
         adata, expected = _load(path)
 
         mc.ut.log_calc("path", path)
         pdata = adata[range(6000), :].copy()
 
-        mc.pl.analyze_clean_genes(pdata, random_seed=123456, **expected.get("analyze_clean_genes", {}))
-        mc.pl.pick_clean_genes(pdata)
-        mc.pl.analyze_clean_cells(pdata, **expected.get("analyze_clean_cells", {}))
-        mc.pl.pick_clean_cells(pdata)
+        mc.pl.exclude_genes(pdata, random_seed=123456, **expected.get("exclude_genes", {}))
+        mc.pl.exclude_cells(pdata, **expected.get("exclude_cells", {}))
         cdata = mc.pl.extract_clean_data(pdata)
         assert cdata is not None
 
+        mc.pl.mark_lateral_genes(pdata, **expected.get("mark_lateral_genes", {}))
+
         mc.pl.compute_direct_metacells(cdata, random_seed=123456, **expected.get("compute_direct_metacells", {}))
 
-        mdata = mc.pl.collect_metacells(cdata)
+        mdata = mc.pl.collect_metacells(cdata, random_seed=123456)
 
-        mc.tl.compute_inner_normalized_variance(adata=cdata, gdata=mdata, random_seed=123456)
+        mc.pl.compute_for_mcview(adata=cdata, gdata=mdata, random_seed=123456)
 
-        expected_results = expected["inner_normalized_variance"]
+        expected_results = expected["inner_stdev_log"]
 
-        actual_results = np.nanmean(mc.ut.get_vo_proper(mdata, "inner_normalized_variance", layout="column_major"))
+        actual_results = np.mean(
+            mc.ut.to_numpy_matrix(mc.ut.get_vo_proper(mdata, "inner_stdev_log", layout="column_major"))
+        )
 
         # mc.ut.log_calc('PATH', path)
         # mc.ut.log_calc('EXPECT', expected_results)
         # mc.ut.log_calc('ACTUAL', actual_results)
         assert np.allclose([expected_results], [actual_results])
```

### Comparing `metacells-0.8.0/tests/test_utilities.py` & `metacells-0.9.0/tests/test_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,21 +206,21 @@
 
 def test_downsample_matrix() -> None:
     rvs = stats.poisson(10, loc=10).rvs
     matrix = sparse.random(1000, 10000, format="csr", dtype="int32", random_state=123456, data_rvs=rvs)
     assert matrix.nnz == matrix.shape[0] * matrix.shape[1] * 0.01
     old_row_sums = ut.sum_per(matrix, per="row")
     min_sum = np.min(old_row_sums)
-    result = ut.downsample_matrix(matrix, per="row", samples=int(min_sum))
+    result = ut.downsample_matrix(matrix, per="row", samples=int(min_sum), random_seed=123456)
     assert result.shape == matrix.shape
     new_row_sums = ut.sum_per(result, per="row")
     assert np.all(new_row_sums == min_sum)
 
     matrix = matrix.toarray()
-    result = ut.downsample_matrix(matrix, per="row", samples=int(min_sum))
+    result = ut.downsample_matrix(matrix, per="row", samples=int(min_sum), random_seed=123456)
     assert result.shape == matrix.shape
     new_row_sums = ut.sum_per(result, per="row")
     assert np.all(new_row_sums == min_sum)
 
 
 def test_matrix_rows_folds_and_aurocs() -> None:
     np.random.seed(123456)
@@ -342,15 +342,15 @@
 
     expected_result = np.array([1, 2, 1, 8 / 3, 8 / 3])
     assert np.allclose(actual_result, expected_result)
 
 
 def test_patterns_matches() -> None:
     strings = ["foo", "bar", "baz"]
-    actual = ut.patterns_matches("ba?", strings)
+    actual = ut.patterns_matches("ba[a-z]?", strings)
     expected = np.array([False, True, True])
     assert np.allclose(actual, expected)
 
 
 def test_bin_pack() -> None:
     size_of_elements = np.arange(10) * 8 + 1
     bin_of_elements = ut.bin_pack(size_of_elements, 106)
@@ -470,22 +470,14 @@
 
 def test_random_piles() -> None:
     result = ut.random_piles(10, target_pile_size=3, random_seed=123456)
     expected = np.array([2, 2, 1, 1, 1, 0, 0, 2, 0, 0])
     assert np.allclose(result, expected)
 
 
-def test_group_piles() -> None:
-    group_of_elements = np.array([0, 1, 2, 3, 0, 1, 2, 3, 0, 1])
-    group_of_groups = np.array([0, 1, 1, 0])
-    expected = np.array([0, 1, 1, 0, 0, 1, 1, 0, 0, 1])
-    result = ut.group_piles(group_of_elements, group_of_groups)
-    assert np.allclose(result, expected)
-
-
 def test_dense_per() -> None:
     matrix = np.array([[0, 1, 2], [3, 4, 5]], dtype="float")
     _test_per(matrix)
 
 
 def test_sparse_per() -> None:
     matrix = np.array([[0, 1, 2], [3, 4, 5]], dtype="float")
@@ -513,14 +505,17 @@
 
     assert np.allclose(ut.fraction_per(rows_matrix, per="row"), np.array([3 / 15, 12 / 15]))
     assert np.allclose(ut.fraction_per(columns_matrix, per="column"), np.array([3 / 15, 5 / 15, 7 / 15]))
 
     assert np.allclose(ut.mean_per(rows_matrix, per="row"), np.array([3 / 3, 12 / 3]))
     assert np.allclose(ut.mean_per(columns_matrix, per="column"), np.array([3 / 2, 5 / 2, 7 / 2]))
 
+    assert np.allclose(ut.median_per(rows_matrix, per="row"), np.array([3 / 3, 12 / 3]))
+    assert np.allclose(ut.median_per(columns_matrix, per="column"), np.array([3 / 2, 5 / 2, 7 / 2]))
+
     assert np.allclose(
         ut.variance_per(rows_matrix, per="row"), np.array([5 / 3 - (3 / 3) ** 2, 50 / 3 - (12 / 3) ** 2])
     )
 
     assert np.allclose(
         ut.variance_per(columns_matrix, per="column"),
         np.array([9 / 2 - (3 / 2) ** 2, 17 / 2 - (5 / 2) ** 2, 29 / 2 - (7 / 2) ** 2]),
```

