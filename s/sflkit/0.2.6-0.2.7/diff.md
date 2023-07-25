# Comparing `tmp/sflkit-0.2.6.tar.gz` & `tmp/sflkit-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sflkit-0.2.6.tar", last modified: Thu Jul 20 14:45:55 2023, max compression
+gzip compressed data, was "sflkit-0.2.7.tar", last modified: Tue Jul 25 09:16:40 2023, max compression
```

## Comparing `sflkit-0.2.6.tar` & `sflkit-0.2.7.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 14:45:55.061460 sflkit-0.2.6/
--rw-r--r--   0 marius     (501) staff       (20)     1112 2023-03-23 09:55:10.000000 sflkit-0.2.6/LICENSE
--rw-r--r--   0 marius     (501) staff       (20)     4805 2023-07-20 14:45:55.061619 sflkit-0.2.6/PKG-INFO
--rw-r--r--   0 marius     (501) staff       (20)     4050 2023-07-19 14:43:48.000000 sflkit-0.2.6/README.md
--rw-r--r--   0 marius     (501) staff       (20)      809 2023-07-20 14:40:30.000000 sflkit-0.2.6/pyproject.toml
--rw-r--r--   0 marius     (501) staff       (20)     1278 2023-07-20 14:45:55.062301 sflkit-0.2.6/setup.cfg
--rw-r--r--   0 marius     (501) staff       (20)       39 2023-03-23 09:55:13.000000 sflkit-0.2.6/setup.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 14:45:55.033739 sflkit-0.2.6/src/
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 14:45:55.039142 sflkit-0.2.6/src/SFLKit.egg-info/
--rw-r--r--   0 marius     (501) staff       (20)     4805 2023-07-20 14:45:55.000000 sflkit-0.2.6/src/SFLKit.egg-info/PKG-INFO
--rw-r--r--   0 marius     (501) staff       (20)     1848 2023-07-20 14:45:55.000000 sflkit-0.2.6/src/SFLKit.egg-info/SOURCES.txt
--rw-r--r--   0 marius     (501) staff       (20)        1 2023-07-20 14:45:55.000000 sflkit-0.2.6/src/SFLKit.egg-info/dependency_links.txt
--rw-r--r--   0 marius     (501) staff       (20)       43 2023-07-20 14:45:55.000000 sflkit-0.2.6/src/SFLKit.egg-info/entry_points.txt
--rw-r--r--   0 marius     (501) staff       (20)      311 2023-07-20 14:45:55.000000 sflkit-0.2.6/src/SFLKit.egg-info/requires.txt
--rw-r--r--   0 marius     (501) staff       (20)        7 2023-07-20 14:45:55.000000 sflkit-0.2.6/src/SFLKit.egg-info/top_level.txt
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 14:45:55.040287 sflkit-0.2.6/src/sflkit/
--rw-r--r--   0 marius     (501) staff       (20)     2330 2023-07-20 14:40:30.000000 sflkit-0.2.6/src/sflkit/__init__.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 14:45:55.044592 sflkit-0.2.6/src/sflkit/analysis/
--rw-r--r--   0 marius     (501) staff       (20)      161 2023-03-23 09:55:13.000000 sflkit-0.2.6/src/sflkit/analysis/__init__.py
--rw-r--r--   0 marius     (501) staff       (20)     3707 2023-07-20 08:38:14.000000 sflkit-0.2.6/src/sflkit/analysis/analysis_type.py
--rw-r--r--   0 marius     (501) staff       (20)     2228 2023-03-23 17:28:40.000000 sflkit-0.2.6/src/sflkit/analysis/analyzer.py
--rw-r--r--   0 marius     (501) staff       (20)    15380 2023-07-20 14:39:25.000000 sflkit-0.2.6/src/sflkit/analysis/factory.py
--rw-r--r--   0 marius     (501) staff       (20)     1511 2023-03-23 09:55:13.000000 sflkit-0.2.6/src/sflkit/analysis/mapping.py
--rw-r--r--   0 marius     (501) staff       (20)    12806 2023-07-20 07:34:00.000000 sflkit-0.2.6/src/sflkit/analysis/predicate.py
--rw-r--r--   0 marius     (501) staff       (20)     1045 2023-03-24 10:29:08.000000 sflkit-0.2.6/src/sflkit/analysis/similarity.py
--rw-r--r--   0 marius     (501) staff       (20)    18236 2023-07-20 08:39:14.000000 sflkit-0.2.6/src/sflkit/analysis/spectra.py
--rw-r--r--   0 marius     (501) staff       (20)     1224 2023-03-23 15:58:48.000000 sflkit-0.2.6/src/sflkit/analysis/suggestion.py
--rw-r--r--   0 marius     (501) staff       (20)     3643 2023-07-18 08:52:29.000000 sflkit-0.2.6/src/sflkit/cli.py
--rw-r--r--   0 marius     (501) staff       (20)     3432 2023-03-23 09:55:13.000000 sflkit-0.2.6/src/sflkit/color.py
--rw-r--r--   0 marius     (501) staff       (20)    10920 2023-07-18 09:25:52.000000 sflkit-0.2.6/src/sflkit/config.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 14:45:55.046098 sflkit-0.2.6/src/sflkit/instrumentation/
--rw-r--r--   0 marius     (501) staff       (20)      661 2023-07-18 09:22:46.000000 sflkit-0.2.6/src/sflkit/instrumentation/__init__.py
--rw-r--r--   0 marius     (501) staff       (20)     3382 2023-07-18 09:23:43.000000 sflkit-0.2.6/src/sflkit/instrumentation/dir_instrumentation.py
--rw-r--r--   0 marius     (501) staff       (20)      446 2023-03-23 09:55:13.000000 sflkit-0.2.6/src/sflkit/instrumentation/file_instrumentation.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 14:45:55.048777 sflkit-0.2.6/src/sflkit/language/
--rw-r--r--   0 marius     (501) staff       (20)      151 2023-03-23 09:55:13.000000 sflkit-0.2.6/src/sflkit/language/__init__.py
--rw-r--r--   0 marius     (501) staff       (20)      353 2023-03-24 09:13:32.000000 sflkit-0.2.6/src/sflkit/language/extract.py
--rw-r--r--   0 marius     (501) staff       (20)      654 2023-03-23 15:08:14.000000 sflkit-0.2.6/src/sflkit/language/finder.py
--rw-r--r--   0 marius     (501) staff       (20)     3798 2023-07-18 09:25:18.000000 sflkit-0.2.6/src/sflkit/language/language.py
--rw-r--r--   0 marius     (501) staff       (20)     4066 2023-07-18 09:24:46.000000 sflkit-0.2.6/src/sflkit/language/meta.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 14:45:55.052273 sflkit-0.2.6/src/sflkit/language/python/
--rw-r--r--   0 marius     (501) staff       (20)        0 2023-03-23 09:55:13.000000 sflkit-0.2.6/src/sflkit/language/python/__init__.py
--rw-r--r--   0 marius     (501) staff       (20)     8602 2023-07-18 09:24:46.000000 sflkit-0.2.6/src/sflkit/language/python/extract.py
--rw-r--r--   0 marius     (501) staff       (20)    26800 2023-07-18 09:31:57.000000 sflkit-0.2.6/src/sflkit/language/python/factory.py
--rw-r--r--   0 marius     (501) staff       (20)     2990 2023-03-23 09:55:13.000000 sflkit-0.2.6/src/sflkit/language/python/finder.py
--rw-r--r--   0 marius     (501) staff       (20)     6119 2023-03-23 09:55:13.000000 sflkit-0.2.6/src/sflkit/language/python/visitor.py
--rw-r--r--   0 marius     (501) staff       (20)     1085 2023-07-18 08:52:29.000000 sflkit-0.2.6/src/sflkit/language/visitor.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 14:45:55.054152 sflkit-0.2.6/src/sflkit/model/
--rw-r--r--   0 marius     (501) staff       (20)      163 2023-03-23 09:55:13.000000 sflkit-0.2.6/src/sflkit/model/__init__.py
--rw-r--r--   0 marius     (501) staff       (20)      806 2023-07-18 09:25:18.000000 sflkit-0.2.6/src/sflkit/model/event_file.py
--rw-r--r--   0 marius     (501) staff       (20)     2073 2023-03-23 09:55:13.000000 sflkit-0.2.6/src/sflkit/model/model.py
--rw-r--r--   0 marius     (501) staff       (20)     1007 2023-03-23 09:55:13.000000 sflkit-0.2.6/src/sflkit/model/scope.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 14:45:55.054779 sflkit-0.2.6/src/sflkit/runners/
--rw-r--r--   0 marius     (501) staff       (20)      362 2023-07-19 11:34:17.000000 sflkit-0.2.6/src/sflkit/runners/__init__.py
--rw-r--r--   0 marius     (501) staff       (20)     8895 2023-07-19 14:43:48.000000 sflkit-0.2.6/src/sflkit/runners/run.py
-drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-20 14:45:55.061143 sflkit-0.2.6/tests/
--rw-r--r--   0 marius     (501) staff       (20)     7993 2023-07-18 09:27:16.000000 sflkit-0.2.6/tests/test_analysis_objects.py
--rw-r--r--   0 marius     (501) staff       (20)     2057 2023-03-23 18:03:53.000000 sflkit-0.2.6/tests/test_cli.py
--rw-r--r--   0 marius     (501) staff       (20)     1025 2023-03-24 09:19:40.000000 sflkit-0.2.6/tests/test_color.py
--rw-r--r--   0 marius     (501) staff       (20)     6194 2023-07-18 09:28:33.000000 sflkit-0.2.6/tests/test_config.py
--rw-r--r--   0 marius     (501) staff       (20)    14215 2023-07-18 09:30:53.000000 sflkit-0.2.6/tests/test_events.py
--rw-r--r--   0 marius     (501) staff       (20)     1318 2023-03-23 17:37:40.000000 sflkit-0.2.6/tests/test_execution.py
--rw-r--r--   0 marius     (501) staff       (20)     5090 2023-07-18 09:32:50.000000 sflkit-0.2.6/tests/test_instrumentation.py
--rw-r--r--   0 marius     (501) staff       (20)     8856 2023-07-18 09:28:00.000000 sflkit-0.2.6/tests/test_language.py
--rw-r--r--   0 marius     (501) staff       (20)     2773 2023-03-23 09:55:13.000000 sflkit-0.2.6/tests/test_predicates.py
--rw-r--r--   0 marius     (501) staff       (20)     7727 2023-07-19 11:35:28.000000 sflkit-0.2.6/tests/test_runner.py
--rw-r--r--   0 marius     (501) staff       (20)      615 2023-03-23 15:20:53.000000 sflkit-0.2.6/tests/test_scope.py
--rw-r--r--   0 marius     (501) staff       (20)     4279 2023-07-18 09:27:50.000000 sflkit-0.2.6/tests/test_spectra.py
--rw-r--r--   0 marius     (501) staff       (20)    11301 2023-03-24 12:11:43.000000 sflkit-0.2.6/tests/test_suggestions.py
--rw-r--r--   0 marius     (501) staff       (20)     1912 2023-03-23 09:55:13.000000 sflkit-0.2.6/tests/test_visitors.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-25 09:16:40.745813 sflkit-0.2.7/
+-rw-r--r--   0 marius     (501) staff       (20)     1112 2023-03-23 09:55:10.000000 sflkit-0.2.7/LICENSE
+-rw-r--r--   0 marius     (501) staff       (20)     4805 2023-07-25 09:16:40.745956 sflkit-0.2.7/PKG-INFO
+-rw-r--r--   0 marius     (501) staff       (20)     4050 2023-07-19 14:43:48.000000 sflkit-0.2.7/README.md
+-rw-r--r--   0 marius     (501) staff       (20)      809 2023-07-25 09:15:29.000000 sflkit-0.2.7/pyproject.toml
+-rw-r--r--   0 marius     (501) staff       (20)     1278 2023-07-25 09:16:40.747025 sflkit-0.2.7/setup.cfg
+-rw-r--r--   0 marius     (501) staff       (20)       39 2023-03-23 09:55:13.000000 sflkit-0.2.7/setup.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-25 09:16:40.721393 sflkit-0.2.7/src/
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-25 09:16:40.727196 sflkit-0.2.7/src/SFLKit.egg-info/
+-rw-r--r--   0 marius     (501) staff       (20)     4805 2023-07-25 09:16:40.000000 sflkit-0.2.7/src/SFLKit.egg-info/PKG-INFO
+-rw-r--r--   0 marius     (501) staff       (20)     1848 2023-07-25 09:16:40.000000 sflkit-0.2.7/src/SFLKit.egg-info/SOURCES.txt
+-rw-r--r--   0 marius     (501) staff       (20)        1 2023-07-25 09:16:40.000000 sflkit-0.2.7/src/SFLKit.egg-info/dependency_links.txt
+-rw-r--r--   0 marius     (501) staff       (20)       43 2023-07-25 09:16:40.000000 sflkit-0.2.7/src/SFLKit.egg-info/entry_points.txt
+-rw-r--r--   0 marius     (501) staff       (20)      311 2023-07-25 09:16:40.000000 sflkit-0.2.7/src/SFLKit.egg-info/requires.txt
+-rw-r--r--   0 marius     (501) staff       (20)        7 2023-07-25 09:16:40.000000 sflkit-0.2.7/src/SFLKit.egg-info/top_level.txt
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-25 09:16:40.728559 sflkit-0.2.7/src/sflkit/
+-rw-r--r--   0 marius     (501) staff       (20)     2330 2023-07-25 09:15:29.000000 sflkit-0.2.7/src/sflkit/__init__.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-25 09:16:40.732227 sflkit-0.2.7/src/sflkit/analysis/
+-rw-r--r--   0 marius     (501) staff       (20)      161 2023-03-23 09:55:13.000000 sflkit-0.2.7/src/sflkit/analysis/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)     3707 2023-07-24 12:42:27.000000 sflkit-0.2.7/src/sflkit/analysis/analysis_type.py
+-rw-r--r--   0 marius     (501) staff       (20)     2228 2023-03-23 17:28:40.000000 sflkit-0.2.7/src/sflkit/analysis/analyzer.py
+-rw-r--r--   0 marius     (501) staff       (20)    15380 2023-07-20 14:39:25.000000 sflkit-0.2.7/src/sflkit/analysis/factory.py
+-rw-r--r--   0 marius     (501) staff       (20)     1511 2023-03-23 09:55:13.000000 sflkit-0.2.7/src/sflkit/analysis/mapping.py
+-rw-r--r--   0 marius     (501) staff       (20)    12806 2023-07-20 07:34:00.000000 sflkit-0.2.7/src/sflkit/analysis/predicate.py
+-rw-r--r--   0 marius     (501) staff       (20)     1045 2023-03-24 10:29:08.000000 sflkit-0.2.7/src/sflkit/analysis/similarity.py
+-rw-r--r--   0 marius     (501) staff       (20)    18236 2023-07-20 08:39:14.000000 sflkit-0.2.7/src/sflkit/analysis/spectra.py
+-rw-r--r--   0 marius     (501) staff       (20)     1224 2023-03-23 15:58:48.000000 sflkit-0.2.7/src/sflkit/analysis/suggestion.py
+-rw-r--r--   0 marius     (501) staff       (20)     3643 2023-07-18 08:52:29.000000 sflkit-0.2.7/src/sflkit/cli.py
+-rw-r--r--   0 marius     (501) staff       (20)     3432 2023-03-23 09:55:13.000000 sflkit-0.2.7/src/sflkit/color.py
+-rw-r--r--   0 marius     (501) staff       (20)    10920 2023-07-18 09:25:52.000000 sflkit-0.2.7/src/sflkit/config.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-25 09:16:40.733553 sflkit-0.2.7/src/sflkit/instrumentation/
+-rw-r--r--   0 marius     (501) staff       (20)      661 2023-07-18 09:22:46.000000 sflkit-0.2.7/src/sflkit/instrumentation/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)     3382 2023-07-18 09:23:43.000000 sflkit-0.2.7/src/sflkit/instrumentation/dir_instrumentation.py
+-rw-r--r--   0 marius     (501) staff       (20)      446 2023-03-23 09:55:13.000000 sflkit-0.2.7/src/sflkit/instrumentation/file_instrumentation.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-25 09:16:40.735893 sflkit-0.2.7/src/sflkit/language/
+-rw-r--r--   0 marius     (501) staff       (20)      151 2023-03-23 09:55:13.000000 sflkit-0.2.7/src/sflkit/language/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)      353 2023-03-24 09:13:32.000000 sflkit-0.2.7/src/sflkit/language/extract.py
+-rw-r--r--   0 marius     (501) staff       (20)      654 2023-03-23 15:08:14.000000 sflkit-0.2.7/src/sflkit/language/finder.py
+-rw-r--r--   0 marius     (501) staff       (20)     3798 2023-07-18 09:25:18.000000 sflkit-0.2.7/src/sflkit/language/language.py
+-rw-r--r--   0 marius     (501) staff       (20)     4066 2023-07-18 09:24:46.000000 sflkit-0.2.7/src/sflkit/language/meta.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-25 09:16:40.737743 sflkit-0.2.7/src/sflkit/language/python/
+-rw-r--r--   0 marius     (501) staff       (20)        0 2023-03-23 09:55:13.000000 sflkit-0.2.7/src/sflkit/language/python/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)     8602 2023-07-18 09:24:46.000000 sflkit-0.2.7/src/sflkit/language/python/extract.py
+-rw-r--r--   0 marius     (501) staff       (20)    26977 2023-07-24 12:44:53.000000 sflkit-0.2.7/src/sflkit/language/python/factory.py
+-rw-r--r--   0 marius     (501) staff       (20)     2990 2023-03-23 09:55:13.000000 sflkit-0.2.7/src/sflkit/language/python/finder.py
+-rw-r--r--   0 marius     (501) staff       (20)     6303 2023-07-25 08:57:54.000000 sflkit-0.2.7/src/sflkit/language/python/visitor.py
+-rw-r--r--   0 marius     (501) staff       (20)     1085 2023-07-18 08:52:29.000000 sflkit-0.2.7/src/sflkit/language/visitor.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-25 09:16:40.739217 sflkit-0.2.7/src/sflkit/model/
+-rw-r--r--   0 marius     (501) staff       (20)      163 2023-03-23 09:55:13.000000 sflkit-0.2.7/src/sflkit/model/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)      806 2023-07-18 09:25:18.000000 sflkit-0.2.7/src/sflkit/model/event_file.py
+-rw-r--r--   0 marius     (501) staff       (20)     2073 2023-03-23 09:55:13.000000 sflkit-0.2.7/src/sflkit/model/model.py
+-rw-r--r--   0 marius     (501) staff       (20)     1007 2023-03-23 09:55:13.000000 sflkit-0.2.7/src/sflkit/model/scope.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-25 09:16:40.740187 sflkit-0.2.7/src/sflkit/runners/
+-rw-r--r--   0 marius     (501) staff       (20)      362 2023-07-19 11:34:17.000000 sflkit-0.2.7/src/sflkit/runners/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)     9291 2023-07-24 13:53:59.000000 sflkit-0.2.7/src/sflkit/runners/run.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-07-25 09:16:40.745557 sflkit-0.2.7/tests/
+-rw-r--r--   0 marius     (501) staff       (20)     7993 2023-07-18 09:27:16.000000 sflkit-0.2.7/tests/test_analysis_objects.py
+-rw-r--r--   0 marius     (501) staff       (20)     2057 2023-03-23 18:03:53.000000 sflkit-0.2.7/tests/test_cli.py
+-rw-r--r--   0 marius     (501) staff       (20)     1025 2023-03-24 09:19:40.000000 sflkit-0.2.7/tests/test_color.py
+-rw-r--r--   0 marius     (501) staff       (20)     6194 2023-07-18 09:28:33.000000 sflkit-0.2.7/tests/test_config.py
+-rw-r--r--   0 marius     (501) staff       (20)    14215 2023-07-18 09:30:53.000000 sflkit-0.2.7/tests/test_events.py
+-rw-r--r--   0 marius     (501) staff       (20)     1318 2023-03-23 17:37:40.000000 sflkit-0.2.7/tests/test_execution.py
+-rw-r--r--   0 marius     (501) staff       (20)     5090 2023-07-18 09:32:50.000000 sflkit-0.2.7/tests/test_instrumentation.py
+-rw-r--r--   0 marius     (501) staff       (20)     8856 2023-07-18 09:28:00.000000 sflkit-0.2.7/tests/test_language.py
+-rw-r--r--   0 marius     (501) staff       (20)     2773 2023-03-23 09:55:13.000000 sflkit-0.2.7/tests/test_predicates.py
+-rw-r--r--   0 marius     (501) staff       (20)     7727 2023-07-19 11:35:28.000000 sflkit-0.2.7/tests/test_runner.py
+-rw-r--r--   0 marius     (501) staff       (20)      615 2023-03-23 15:20:53.000000 sflkit-0.2.7/tests/test_scope.py
+-rw-r--r--   0 marius     (501) staff       (20)     4279 2023-07-18 09:27:50.000000 sflkit-0.2.7/tests/test_spectra.py
+-rw-r--r--   0 marius     (501) staff       (20)    11301 2023-03-24 12:11:43.000000 sflkit-0.2.7/tests/test_suggestions.py
+-rw-r--r--   0 marius     (501) staff       (20)     1912 2023-03-23 09:55:13.000000 sflkit-0.2.7/tests/test_visitors.py
```

### Comparing `sflkit-0.2.6/LICENSE` & `sflkit-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/PKG-INFO` & `sflkit-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sflkit
-Version: 0.2.6
+Version: 0.2.7
 Summary: SFLKit: : A Workbench for Statistical Fault Localization
 Home-page: https://github.com/uds-se/sflkit
 Author: Marius Smytzek & Andreas Zeller
 Author-email: Marius Smytzek <marius.smytzek@cispa.de>
 Project-URL: Homepage, https://github.com/uds-se/sflkit/
 Project-URL: Bug Tracker, https://github.com/uds-se/sflkit/issues
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sflkit-0.2.6/README.md` & `sflkit-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/pyproject.toml` & `sflkit-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=67.6.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sflkit"
-version = "0.2.6"
+version = "0.2.7"
 authors = [
     { name = "Marius Smytzek", email = "marius.smytzek@cispa.de" },
 ]
 description = "SFLKit: : A Workbench for Statistical Fault Localization"
 readme = "README.md"
 license = { file = "COPYING" }
 requires-python = ">=3.10"
```

### Comparing `sflkit-0.2.6/setup.cfg` & `sflkit-0.2.7/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -22,28 +22,28 @@
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.10
 install_requires = 
 	sflkitlib>=0.0.1
 	astor>=0.8.1
-	numpy==1.25.1
-	matplotlib==3.7.2
+	numpy>=1.25.1
+	matplotlib>=3.7.2
 	sortedcollections>=2.1.0
 	parameterized>=0.8.1
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 test = 
 	sflkitlib>=0.0.1
 	astor>=0.8.1
-	numpy==1.25.1
-	matplotlib==3.7.2
+	numpy>=1.25.1
+	matplotlib>=3.7.2
 	sortedcollections>=2.1.0
 	pytest>=7.2.2
 	pytest-cov>=4.1.0
 	pytest-html>=3.2.0
 	pytest-rerunfailures>=11.1.2
 	parameterized>=0.8.1
 dev =
```

### Comparing `sflkit-0.2.6/src/SFLKit.egg-info/PKG-INFO` & `sflkit-0.2.7/src/SFLKit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sflkit
-Version: 0.2.6
+Version: 0.2.7
 Summary: SFLKit: : A Workbench for Statistical Fault Localization
 Home-page: https://github.com/uds-se/sflkit
 Author: Marius Smytzek & Andreas Zeller
 Author-email: Marius Smytzek <marius.smytzek@cispa.de>
 Project-URL: Homepage, https://github.com/uds-se/sflkit/
 Project-URL: Bug Tracker, https://github.com/uds-se/sflkit/issues
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sflkit-0.2.6/src/SFLKit.egg-info/SOURCES.txt` & `sflkit-0.2.7/src/SFLKit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/src/sflkit/__init__.py` & `sflkit-0.2.7/src/sflkit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 from sflkit.analysis.analyzer import Analyzer
 from sflkit.analysis.predicate import Predicate
 from sflkit.config import Config, parse_config
 from sflkit.instrumentation.dir_instrumentation import DirInstrumentation
 
-__version__ = "0.2.6"
+__version__ = "0.2.7"
 
 
 def instrument_config(conf: Config, event_dump: str = None):
     instrumentation = DirInstrumentation(conf.visitor)
     instrumentation.instrument(
         conf.target_path,
         conf.instrument_working,
```

### Comparing `sflkit-0.2.6/src/sflkit/analysis/analysis_type.py` & `sflkit-0.2.7/src/sflkit/analysis/analysis_type.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/src/sflkit/analysis/analyzer.py` & `sflkit-0.2.7/src/sflkit/analysis/analyzer.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/src/sflkit/analysis/factory.py` & `sflkit-0.2.7/src/sflkit/analysis/factory.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/src/sflkit/analysis/mapping.py` & `sflkit-0.2.7/src/sflkit/analysis/mapping.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/src/sflkit/analysis/predicate.py` & `sflkit-0.2.7/src/sflkit/analysis/predicate.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/src/sflkit/analysis/similarity.py` & `sflkit-0.2.7/src/sflkit/analysis/similarity.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/src/sflkit/analysis/spectra.py` & `sflkit-0.2.7/src/sflkit/analysis/spectra.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/src/sflkit/analysis/suggestion.py` & `sflkit-0.2.7/src/sflkit/analysis/suggestion.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/src/sflkit/cli.py` & `sflkit-0.2.7/src/sflkit/cli.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/src/sflkit/color.py` & `sflkit-0.2.7/src/sflkit/color.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/src/sflkit/config.py` & `sflkit-0.2.7/src/sflkit/config.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/src/sflkit/instrumentation/__init__.py` & `sflkit-0.2.7/src/sflkit/instrumentation/__init__.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/src/sflkit/instrumentation/dir_instrumentation.py` & `sflkit-0.2.7/src/sflkit/instrumentation/dir_instrumentation.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/src/sflkit/language/finder.py` & `sflkit-0.2.7/src/sflkit/language/finder.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/src/sflkit/language/language.py` & `sflkit-0.2.7/src/sflkit/language/language.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/src/sflkit/language/meta.py` & `sflkit-0.2.7/src/sflkit/language/meta.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/src/sflkit/language/python/extract.py` & `sflkit-0.2.7/src/sflkit/language/python/extract.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/src/sflkit/language/python/factory.py` & `sflkit-0.2.7/src/sflkit/language/python/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,20 +199,28 @@
             self.file, node.lineno, self.id_generator.get_next_id(), self.branch_id, -1
         )
         return Injection(
             body=[self.get_event_call(branch_event)], events=[branch_event]
         )
 
     def visit_Try(self, node: Try) -> Injection:
-        else_branch_event = BranchEvent(
-            self.file, node.lineno, self.id_generator.get_next_id(), self.branch_id, -1
-        )
-        return Injection(
-            orelse=[self.get_event_call(else_branch_event)], events=[else_branch_event]
-        )
+        if node.handlers:
+            else_branch_event = BranchEvent(
+                self.file,
+                node.lineno,
+                self.id_generator.get_next_id(),
+                self.branch_id,
+                -1,
+            )
+            return Injection(
+                orelse=[self.get_event_call(else_branch_event)],
+                events=[else_branch_event],
+            )
+        else:
+            return Injection()
 
 
 class DefEventFactory(PythonEventFactory):
     def get_function(self):
         return "add_def_event"
 
     def get_event_call(self, event: DefEvent):
```

### Comparing `sflkit-0.2.6/src/sflkit/language/python/finder.py` & `sflkit-0.2.7/src/sflkit/language/python/finder.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/src/sflkit/language/python/visitor.py` & `sflkit-0.2.7/src/sflkit/language/python/visitor.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,25 +70,31 @@
                         body=[node],
                         handlers=[],
                         orelse=[],
                         finalbody=injection.finalbody,
                     )
         if injection.error:
             error_var = self.meta_visitor.tmp_generator.get_var_name()
+            raise_stmt = [
+                Raise(
+                    exc=Name(id=error_var),
+                    cause=None,
+                )
+            ]
             if body:
                 node.body = (
                     Try(
                         body=node.body,
                         handlers=[
                             ExceptHandler(
                                 type=Name(
                                     id="BaseException",
                                 ),
                                 name=error_var,
-                                body=injection.error,
+                                body=injection.error + raise_stmt,
                             )
                         ],
                         orelse=[],
                         finalbody=[],
                     ),
                 )
             else:
@@ -97,15 +103,15 @@
                         body=[node],
                         handlers=[
                             ExceptHandler(
                                 type=Name(
                                     id="BaseException",
                                 ),
                                 name=error_var,
-                                body=injection.error,
+                                body=injection.error + raise_stmt,
                             )
                         ],
                         orelse=[],
                         finalbody=[],
                     ),
                 )
         if injection.pre or injection.post:
```

### Comparing `sflkit-0.2.6/src/sflkit/language/visitor.py` & `sflkit-0.2.7/src/sflkit/language/visitor.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/src/sflkit/model/event_file.py` & `sflkit-0.2.7/src/sflkit/model/event_file.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/src/sflkit/model/model.py` & `sflkit-0.2.7/src/sflkit/model/model.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/src/sflkit/model/scope.py` & `sflkit-0.2.7/src/sflkit/model/scope.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/src/sflkit/runners/run.py` & `sflkit-0.2.7/src/sflkit/runners/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 PYTEST_COLLECT_PATTERN = re.compile(
     '<(?P<kind>Package|Module|Class|Function|UnitTestCase|TestCaseFunction) (?P<name>[^>]+|"([^"]|\\")+")>'
 )
 PYTEST_RESULT_PATTERN = re.compile(
     rb"= ((((?P<f>\d+) failed)|((?P<p>\d+) passed)|(\d+ warnings?))(, )?)+ in "
 )
 
+DEFAULT_TIMEOUT = 10
+
 
 class PytestNode(abc.ABC):
     def __init__(self, name: str, parent=None):
         self.name = name
         self.parent: Optional[PytestNode] = parent
         self.children: List[PytestNode] = []
 
@@ -137,15 +139,16 @@
     UNDEFINED = "UNDEFINED"
 
     def get_dir(self):
         return self.value.lower()
 
 
 class Runner(abc.ABC):
-    def __init__(self, re_filter: str = r".*"):
+    def __init__(self, re_filter: str = r".*", timeout=DEFAULT_TIMEOUT):
+        self.timeout = timeout
         self.re_filter = re.compile(re_filter)
 
     def get_tests(self, directory: Path, environ: Environment = None) -> List[str]:
         return []
 
     def run_test(
         self, directory: Path, test: str, environ: Environment = None
@@ -214,20 +217,24 @@
                 passing = 0
             return True, passing, failing
         return False, None, None
 
     def run_test(
         self, directory: Path, test: str, environ: Environment = None
     ) -> TestResult:
-        output = subprocess.run(
-            ["python", "-m", "pytest", test],
-            stdout=subprocess.PIPE,
-            env=environ,
-            cwd=directory,
-        ).stdout
+        try:
+            output = subprocess.run(
+                ["python", "-m", "pytest", test],
+                stdout=subprocess.PIPE,
+                env=environ,
+                cwd=directory,
+                timeout=self.timeout,
+            ).stdout
+        except subprocess.TimeoutExpired:
+            return TestResult.UNDEFINED
         successful, passing, failing = self.__get_pytest_result__(output)
         if successful:
             if passing > 0 and failing == 0:
                 return TestResult.PASSING
             elif failing > 0 and passing == 0:
                 return TestResult.FAILING
             else:
@@ -268,19 +275,23 @@
     ) -> TestResult:
         if "passing" in test_name:
             test = self.passing[test_name]
             result = TestResult.PASSING
         else:
             test = self.failing[test_name]
             result = TestResult.FAILING
-        process = subprocess.run(
-            ["python", self.access] + test,
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
-            env=environ,
-            cwd=directory,
-        )
+        try:
+            process = subprocess.run(
+                ["python", self.access] + test,
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+                env=environ,
+                cwd=directory,
+                timeout=self.timeout,
+            )
+        except subprocess.TimeoutExpired:
+            return TestResult.UNDEFINED
         self.output[test_name] = (
             process.stdout.decode("utf8"),
             process.stderr.decode("utf8"),
         )
         return result
```

### Comparing `sflkit-0.2.6/tests/test_analysis_objects.py` & `sflkit-0.2.7/tests/test_analysis_objects.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/tests/test_cli.py` & `sflkit-0.2.7/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/tests/test_color.py` & `sflkit-0.2.7/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/tests/test_config.py` & `sflkit-0.2.7/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/tests/test_events.py` & `sflkit-0.2.7/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/tests/test_execution.py` & `sflkit-0.2.7/tests/test_execution.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/tests/test_instrumentation.py` & `sflkit-0.2.7/tests/test_instrumentation.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/tests/test_language.py` & `sflkit-0.2.7/tests/test_language.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/tests/test_predicates.py` & `sflkit-0.2.7/tests/test_predicates.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/tests/test_runner.py` & `sflkit-0.2.7/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/tests/test_scope.py` & `sflkit-0.2.7/tests/test_scope.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/tests/test_spectra.py` & `sflkit-0.2.7/tests/test_spectra.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/tests/test_suggestions.py` & `sflkit-0.2.7/tests/test_suggestions.py`

 * *Files identical despite different names*

### Comparing `sflkit-0.2.6/tests/test_visitors.py` & `sflkit-0.2.7/tests/test_visitors.py`

 * *Files identical despite different names*

