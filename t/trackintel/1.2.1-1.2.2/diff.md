# Comparing `tmp/trackintel-1.2.1.tar.gz` & `tmp/trackintel-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trackintel-1.2.1.tar", last modified: Thu Apr 20 14:25:16 2023, max compression
+gzip compressed data, was "trackintel-1.2.2.tar", last modified: Tue Jul 25 19:33:55 2023, max compression
```

## Comparing `trackintel-1.2.1.tar` & `trackintel-1.2.2.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.770783 trackintel-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-20 14:25:08.000000 trackintel-1.2.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-20 14:25:08.000000 trackintel-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-04-20 14:25:16.770783 trackintel-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-04-20 14:25:08.000000 trackintel-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.742782 trackintel-1.2.1/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:08.000000 trackintel-1.2.1/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-04-20 14:25:08.000000 trackintel-1.2.1/benchmarks/preprocessing_benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 14:25:16.770783 trackintel-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-20 14:25:08.000000 trackintel-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.742782 trackintel-1.2.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.746782 trackintel-1.2.1/tests/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/analysis/test_label.py
--rw-r--r--   0 runner    (1001) docker     (123)    20437 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/analysis/test_location_identification.py
--rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/analysis/test_modal_split.py
--rw-r--r--   0 runner    (1001) docker     (123)    19336 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/analysis/test_tracking_quality.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.746782 trackintel-1.2.1/tests/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/examples/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/examples/test_tutorial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.746782 trackintel-1.2.1/tests/geogr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/geogr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/geogr/test_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/geogr/test_point_distances.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.750782 trackintel-1.2.1/tests/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/io/test_dataset_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/io/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    15670 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/io/test_from_geopandas.py
--rw-r--r--   0 runner    (1001) docker     (123)    28897 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/io/test_postgis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.750782 trackintel-1.2.1/tests/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/model/test_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/model/test_positionfixes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/model/test_staypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/model/test_triplegs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/model/test_trips.py
--rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/model/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.754783 trackintel-1.2.1/tests/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/preprocessing/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    25185 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/preprocessing/test_positionfixes.py
--rw-r--r--   0 runner    (1001) docker     (123)    25722 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/preprocessing/test_staypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    31836 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/preprocessing/test_triplegs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/preprocessing/test_trips.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/preprocessing/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/test_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.754783 trackintel-1.2.1/tests/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/visualization/test_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/visualization/test_modal_split.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/visualization/test_positionfixes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/visualization/test_staypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/visualization/test_triplegs.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-20 14:25:08.000000 trackintel-1.2.1/tests/visualization/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.758782 trackintel-1.2.1/trackintel/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.758782 trackintel-1.2.1/trackintel/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/analysis/labelling.py
--rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/analysis/location_identification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/analysis/modal_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/analysis/tracking_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.762783 trackintel-1.2.1/trackintel/geogr/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/geogr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/geogr/distances.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/geogr/point_distances.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.762783 trackintel-1.2.1/trackintel/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27617 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/io/dataset_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    20115 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/io/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    13340 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/io/from_geopandas.py
--rw-r--r--   0 runner    (1001) docker     (123)    24080 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/io/postgis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.766783 trackintel-1.2.1/trackintel/model/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/model/locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/model/positionfixes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/model/staypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/model/tours.py
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/model/triplegs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/model/trips.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/model/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.766783 trackintel-1.2.1/trackintel/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/preprocessing/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21266 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/preprocessing/positionfixes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14528 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/preprocessing/staypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    14341 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/preprocessing/triplegs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17114 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/preprocessing/trips.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/preprocessing/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.770783 trackintel-1.2.1/trackintel/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/visualization/locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/visualization/modal_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/visualization/osm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/visualization/positionfixes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/visualization/staypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/visualization/triplegs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-20 14:25:08.000000 trackintel-1.2.1/trackintel/visualization/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:25:16.758782 trackintel-1.2.1/trackintel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-04-20 14:25:16.000000 trackintel-1.2.1/trackintel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-20 14:25:16.000000 trackintel-1.2.1/trackintel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:25:16.000000 trackintel-1.2.1/trackintel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-20 14:25:16.000000 trackintel-1.2.1/trackintel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-20 14:25:16.000000 trackintel-1.2.1/trackintel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:33:55.118948 trackintel-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-25 19:33:44.000000 trackintel-1.2.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-25 19:33:44.000000 trackintel-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-07-25 19:33:55.118948 trackintel-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-07-25 19:33:44.000000 trackintel-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:33:55.102948 trackintel-1.2.2/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:33:44.000000 trackintel-1.2.2/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-07-25 19:33:44.000000 trackintel-1.2.2/benchmarks/preprocessing_benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:33:55.118948 trackintel-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-25 19:33:44.000000 trackintel-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:33:55.102948 trackintel-1.2.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:33:55.102948 trackintel-1.2.2/tests/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/analysis/test_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20437 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/analysis/test_location_identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/analysis/test_modal_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19336 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/analysis/test_tracking_quality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:33:55.102948 trackintel-1.2.2/tests/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/examples/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/examples/test_tutorial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:33:55.102948 trackintel-1.2.2/tests/geogr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/geogr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/geogr/test_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/geogr/test_point_distances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:33:55.106948 trackintel-1.2.2/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/io/test_dataset_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/io/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15670 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/io/test_from_geopandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28897 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/io/test_postgis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:33:55.106948 trackintel-1.2.2/tests/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/model/test_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/model/test_positionfixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/model/test_staypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/model/test_triplegs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/model/test_trips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/model/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:33:55.106948 trackintel-1.2.2/tests/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/preprocessing/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26131 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/preprocessing/test_positionfixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25722 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/preprocessing/test_staypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31836 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/preprocessing/test_triplegs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/preprocessing/test_trips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/preprocessing/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:33:55.110948 trackintel-1.2.2/tests/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/visualization/test_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/visualization/test_modal_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/visualization/test_positionfixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/visualization/test_staypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/visualization/test_triplegs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-25 19:33:44.000000 trackintel-1.2.2/tests/visualization/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:33:55.110948 trackintel-1.2.2/trackintel/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:33:55.110948 trackintel-1.2.2/trackintel/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/analysis/labelling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13109 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/analysis/location_identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/analysis/modal_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/analysis/tracking_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:33:55.114948 trackintel-1.2.2/trackintel/geogr/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/geogr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/geogr/distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/geogr/point_distances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:33:55.114948 trackintel-1.2.2/trackintel/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27617 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/io/dataset_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20115 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/io/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13340 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/io/from_geopandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24080 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/io/postgis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:33:55.114948 trackintel-1.2.2/trackintel/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/model/locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/model/positionfixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/model/staypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/model/tours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/model/triplegs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/model/trips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/model/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:33:55.118948 trackintel-1.2.2/trackintel/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/preprocessing/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21589 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/preprocessing/positionfixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14312 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/preprocessing/staypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13893 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/preprocessing/triplegs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17114 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/preprocessing/trips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/preprocessing/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:33:55.118948 trackintel-1.2.2/trackintel/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/visualization/locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/visualization/modal_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/visualization/osm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/visualization/positionfixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/visualization/staypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/visualization/triplegs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-07-25 19:33:44.000000 trackintel-1.2.2/trackintel/visualization/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:33:55.110948 trackintel-1.2.2/trackintel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-07-25 19:33:55.000000 trackintel-1.2.2/trackintel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-25 19:33:55.000000 trackintel-1.2.2/trackintel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:33:55.000000 trackintel-1.2.2/trackintel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-25 19:33:55.000000 trackintel-1.2.2/trackintel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-25 19:33:55.000000 trackintel-1.2.2/trackintel.egg-info/top_level.txt
```

### Comparing `trackintel-1.2.1/AUTHORS.md` & `trackintel-1.2.2/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/LICENSE` & `trackintel-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/PKG-INFO` & `trackintel-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trackintel
-Version: 1.2.1
+Version: 1.2.2
 Summary: Human mobility and movement analysis framework.
 Home-page: https://github.com/mie-lab/trackintel
 Author: Dominik Bucher, Henry Martin, Ye Hong
 Author-email: dobucher@ethz.ch, martinhe@ethz.ch
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -23,15 +23,15 @@
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/trackintel.svg)](https://anaconda.org/conda-forge/trackintel)
 [![Actions Status](https://github.com/mie-lab/trackintel/workflows/Tests/badge.svg)](https://github.com/mie-lab/trackintel/actions?query=workflow%3ATests)
 [![Documentation Status](https://readthedocs.org/projects/trackintel/badge/?version=latest)](https://trackintel.readthedocs.io/en/latest/?badge=latest)
 [![codecov.io](https://codecov.io/gh/mie-lab/trackintel/coverage.svg?branch=master)](https://codecov.io/gh/mie-lab/trackintel)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![asv](http://img.shields.io/badge/benchmarked%20by-asv-green.svg?style=flat)](https://mie-lab.github.io/trackintel/)
 
-*trackintel* is a library for the analysis of spatio-temporal tracking data with a focus on human mobility. The core of *trackintel* is the hierachical data model for movement data that is used in GIS, transport planning and related fields. We provide functionalities for the full life-cycle of human mobility data analysis: import and export of tracking data of different types (e.g, trackpoints, check-ins, trajectories), preprocessing, data quality assessment, semantic enrichment, quantitative analysis and mining tasks, and visualization of data and results.
+*trackintel* is a library for the analysis of spatio-temporal tracking data with a focus on human mobility. The core of *trackintel* is the hierarchical data model for movement data that is used in GIS, transport planning and related fields. We provide functionalities for the full life-cycle of human mobility data analysis: import and export of tracking data of different types (e.g, trackpoints, check-ins, trajectories), preprocessing, data quality assessment, semantic enrichment, quantitative analysis and mining tasks, and visualization of data and results.
 Trackintel is based on [Pandas](https://pandas.pydata.org/) and [GeoPandas](https://geopandas.org/#). 
 
 You can find the documentation on the [trackintel documentation page](https://trackintel.readthedocs.io/en/latest). 
 
 Try *trackintel* online in a MyBinder notebook: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mie-lab/trackintel/HEAD?filepath=%2Fexamples%2Ftrackintel_basic_tutorial.ipynb)
 
 Please star this repo and [cite](#citelink) our paper if you find our work is helpful for you.
@@ -139,15 +139,14 @@
 * Pint
 * NetworkX
 * GeoAlchemy2
 * scikit-learn
 * tqdm
 * OSMnx
 * similaritymeasures
-* pygeos
 
 ## Development
 You can find the development roadmap under `ROADMAP.md` and further development guidelines under `CONTRIBUTING.md`.
 
 ## Contributors
 
 *trackintel* is primarily maintained by the Mobility Information Engineering Lab at ETH Zurich ([mie-lab.ethz.ch](http://mie-lab.ethz.ch)).
```

### Comparing `trackintel-1.2.1/README.md` & `trackintel-1.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/trackintel.svg)](https://anaconda.org/conda-forge/trackintel)
 [![Actions Status](https://github.com/mie-lab/trackintel/workflows/Tests/badge.svg)](https://github.com/mie-lab/trackintel/actions?query=workflow%3ATests)
 [![Documentation Status](https://readthedocs.org/projects/trackintel/badge/?version=latest)](https://trackintel.readthedocs.io/en/latest/?badge=latest)
 [![codecov.io](https://codecov.io/gh/mie-lab/trackintel/coverage.svg?branch=master)](https://codecov.io/gh/mie-lab/trackintel)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![asv](http://img.shields.io/badge/benchmarked%20by-asv-green.svg?style=flat)](https://mie-lab.github.io/trackintel/)
 
-*trackintel* is a library for the analysis of spatio-temporal tracking data with a focus on human mobility. The core of *trackintel* is the hierachical data model for movement data that is used in GIS, transport planning and related fields. We provide functionalities for the full life-cycle of human mobility data analysis: import and export of tracking data of different types (e.g, trackpoints, check-ins, trajectories), preprocessing, data quality assessment, semantic enrichment, quantitative analysis and mining tasks, and visualization of data and results.
+*trackintel* is a library for the analysis of spatio-temporal tracking data with a focus on human mobility. The core of *trackintel* is the hierarchical data model for movement data that is used in GIS, transport planning and related fields. We provide functionalities for the full life-cycle of human mobility data analysis: import and export of tracking data of different types (e.g, trackpoints, check-ins, trajectories), preprocessing, data quality assessment, semantic enrichment, quantitative analysis and mining tasks, and visualization of data and results.
 Trackintel is based on [Pandas](https://pandas.pydata.org/) and [GeoPandas](https://geopandas.org/#). 
 
 You can find the documentation on the [trackintel documentation page](https://trackintel.readthedocs.io/en/latest). 
 
 Try *trackintel* online in a MyBinder notebook: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mie-lab/trackintel/HEAD?filepath=%2Fexamples%2Ftrackintel_basic_tutorial.ipynb)
 
 Please star this repo and [cite](#citelink) our paper if you find our work is helpful for you.
@@ -121,15 +121,14 @@
 * Pint
 * NetworkX
 * GeoAlchemy2
 * scikit-learn
 * tqdm
 * OSMnx
 * similaritymeasures
-* pygeos
 
 ## Development
 You can find the development roadmap under `ROADMAP.md` and further development guidelines under `CONTRIBUTING.md`.
 
 ## Contributors
 
 *trackintel* is primarily maintained by the Mobility Information Engineering Lab at ETH Zurich ([mie-lab.ethz.ch](http://mie-lab.ethz.ch)).
```

### Comparing `trackintel-1.2.1/benchmarks/preprocessing_benchmarks.py` & `trackintel-1.2.2/benchmarks/preprocessing_benchmarks.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/setup.py` & `trackintel-1.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,42 +18,40 @@
 REQUIRES_PYTHON = ">=3.6.0"
 VERSION = None
 LICENSE = "MIT"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "pandas",
-    "geopandas>=0.9.0",
+    "geopandas>=0.12.0",
     "matplotlib",
     "numpy",
     "pint",
     "shapely",
     "networkx",
     "geoalchemy2",
     "osmnx",
     "scikit-learn",
     "tqdm",
     "similaritymeasures",
-    "pygeos>=0.10.0",
 ]
 
 install_requires = [
     "pandas",
     "matplotlib",
     "numpy",
     "pint",
-    "shapely<=1.8.5",
+    "shapely",
     "networkx",
     "geoalchemy2",
     "osmnx",
     "scikit-learn",
     "tqdm",
-    "geopandas>=0.10.0",
+    "geopandas>=0.12.0",
     "similaritymeasures",
-    "pygeos>=0.10.0",
 ]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
```

### Comparing `trackintel-1.2.1/tests/analysis/test_label.py` & `trackintel-1.2.2/tests/analysis/test_label.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/tests/analysis/test_location_identification.py` & `trackintel-1.2.2/tests/analysis/test_location_identification.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/tests/analysis/test_modal_split.py` & `trackintel-1.2.2/tests/analysis/test_modal_split.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/tests/analysis/test_tracking_quality.py` & `trackintel-1.2.2/tests/analysis/test_tracking_quality.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/tests/examples/test_tutorial.py` & `trackintel-1.2.2/tests/examples/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/tests/geogr/test_distances.py` & `trackintel-1.2.2/tests/geogr/test_distances.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/tests/geogr/test_point_distances.py` & `trackintel-1.2.2/tests/geogr/test_point_distances.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/tests/io/test_dataset_reader.py` & `trackintel-1.2.2/tests/io/test_dataset_reader.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/tests/io/test_file.py` & `trackintel-1.2.2/tests/io/test_file.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/tests/io/test_from_geopandas.py` & `trackintel-1.2.2/tests/io/test_from_geopandas.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/tests/io/test_postgis.py` & `trackintel-1.2.2/tests/io/test_postgis.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/tests/model/test_locations.py` & `trackintel-1.2.2/tests/model/test_locations.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/tests/model/test_positionfixes.py` & `trackintel-1.2.2/tests/model/test_positionfixes.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/tests/model/test_staypoints.py` & `trackintel-1.2.2/tests/model/test_staypoints.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/tests/model/test_triplegs.py` & `trackintel-1.2.2/tests/model/test_triplegs.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/tests/model/test_trips.py` & `trackintel-1.2.2/tests/model/test_trips.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/tests/model/test_util.py` & `trackintel-1.2.2/tests/model/test_util.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/tests/preprocessing/test_filter.py` & `trackintel-1.2.2/tests/preprocessing/test_filter.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/tests/preprocessing/test_positionfixes.py` & `trackintel-1.2.2/tests/preprocessing/test_positionfixes.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,14 +289,23 @@
             _, sp = pfs.as_positionfixes.generate_staypoints(include_last=True)
             assert len(sp) == 0
 
         # using large gap_threshold one sp will be generated
         _, sp = pfs.as_positionfixes.generate_staypoints(gap_threshold=1e8, include_last=True)
         assert len(sp) == 1
 
+    def test_str_userid(self, example_positionfixes):
+        """Staypoint generation should also run without error if the user_id is a string"""
+        # the pfs would not generate staypoints with the default parameters
+        pfs = example_positionfixes
+        pfs["user_id"] = pfs["user_id"].astype(str)
+        warn_string = "No staypoints can be generated, returning empty sp."
+        with pytest.warns(UserWarning, match=warn_string):
+            pfs, sp = pfs.as_positionfixes.generate_staypoints()
+
 
 class Test_Generate_staypoints_sliding_user:
     """Test for _generate_staypoints_sliding_user."""
 
     def test_unknown_distance_metric(self, example_positionfixes):
         """Test if the distance metric is unknown, an AttributeError will be raised."""
         with pytest.raises(AttributeError):
@@ -532,7 +541,16 @@
             sp_tpls_this = sp_tpls[sp_tpls["user_id"] == user_id_this]
             diff = sp_tpls_this["started_at"] - sp_tpls_this["finished_at"].shift(1)
             # transform to numpy array and drop first values (always nan due to shift operation)
             diff = diff.values[1:]
 
             # all values have to greater or equal to zero. Otherwise there is an overlap
             assert all(diff >= np.timedelta64(datetime.timedelta()))
+
+    def test_str_userid(self, example_positionfixes_isolated):
+        """Tripleg generation should also work if the user IDs are strings"""
+        pfs = example_positionfixes_isolated
+        # remove isolated - not needed for this test
+        pfs = pfs[~pfs.index.isin([1, 2])].copy()
+        # set user ID to string
+        pfs["user_id"] = pfs["user_id"].astype(str)
+        pfs, tpls = pfs.as_positionfixes.generate_triplegs()
```

### Comparing `trackintel-1.2.1/tests/preprocessing/test_staypoints.py` & `trackintel-1.2.2/tests/preprocessing/test_staypoints.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/tests/preprocessing/test_triplegs.py` & `trackintel-1.2.2/tests/preprocessing/test_triplegs.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/tests/preprocessing/test_trips.py` & `trackintel-1.2.2/tests/preprocessing/test_trips.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/tests/preprocessing/test_util.py` & `trackintel-1.2.2/tests/preprocessing/test_util.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/tests/visualization/test_locations.py` & `trackintel-1.2.2/tests/visualization/test_locations.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/tests/visualization/test_modal_split.py` & `trackintel-1.2.2/tests/visualization/test_modal_split.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/tests/visualization/test_positionfixes.py` & `trackintel-1.2.2/tests/visualization/test_positionfixes.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/tests/visualization/test_staypoints.py` & `trackintel-1.2.2/tests/visualization/test_staypoints.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/tests/visualization/test_triplegs.py` & `trackintel-1.2.2/tests/visualization/test_triplegs.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/tests/visualization/test_util.py` & `trackintel-1.2.2/tests/visualization/test_util.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/trackintel/analysis/__init__.py` & `trackintel-1.2.2/trackintel/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/trackintel/analysis/labelling.py` & `trackintel-1.2.2/trackintel/analysis/labelling.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/trackintel/analysis/location_identification.py` & `trackintel-1.2.2/trackintel/analysis/location_identification.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,17 +44,14 @@
     https://doi.org/10.1080/13658816.2021.1887489.
 
     Examples
     --------
     >>> from ti.analysis.location_identification import location_identifier
     >>> location_identifier(staypoints, pre_filter=True, method="FREQ")
     """
-    # assert validity of staypoints
-    staypoints.as_staypoints
-
     sp = staypoints.copy()
     if "location_id" not in sp.columns:
         raise KeyError(
             (
                 "To derive activity labels the GeoDataFrame (as trackintel staypoints) must have a column "
                 f"named 'location_id' but it has [{', '.join(sp.columns)}]"
             )
@@ -121,17 +118,14 @@
 
     Examples
     --------
     >>> from ti.analysis.location_identification import pre_filter_locations
     >>> mask = pre_filter_locations(staypoints)
     >>> staypoints = staypoints[mask]
     """
-    # assert validity of staypoints
-    staypoints.as_staypoints
-
     sp = staypoints.copy()
     if isinstance(thresh_loc_time, str):
         thresh_loc_time = pd.to_timedelta(thresh_loc_time)
     if isinstance(thresh_loc_period, str):
         thresh_loc_period = pd.to_timedelta(thresh_loc_period)
 
     # filtering users
```

### Comparing `trackintel-1.2.1/trackintel/analysis/modal_split.py` & `trackintel-1.2.2/trackintel/analysis/modal_split.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/trackintel/analysis/tracking_quality.py` & `trackintel-1.2.2/trackintel/analysis/tracking_quality.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/trackintel/geogr/distances.py` & `trackintel-1.2.2/trackintel/geogr/distances.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import multiprocessing
 import warnings
 from functools import partial
 from math import cos, pi
 
 import numpy as np
 import pandas as pd
-import pygeos
+import shapely
+import similaritymeasures
 from scipy.spatial.distance import cdist
 from sklearn.metrics import pairwise_distances
-import similaritymeasures
 
 from trackintel.geogr.point_distances import haversine_dist
 
 
 def calculate_distance_matrix(X, Y=None, dist_metric="haversine", n_jobs=0, **kwds):
     """
     Calculate a distance matrix based on a specific distance metric.
@@ -246,13 +246,13 @@
         The length of each linestring in meters
 
     Examples
     --------
     >>> from trackintel.geogr.distances import calculate_haversine_length
     >>> triplegs['length'] = calculate_haversine_length(triplegs)
     """
-    geom = pygeos.from_shapely(gdf.geometry)
-    assert np.any(pygeos.get_type_id(geom) == 1)  # 1 is LineStrings
-    geom, index = pygeos.get_coordinates(geom, return_index=True)
+    geom = gdf.geometry
+    assert np.any(shapely.get_type_id(geom) == 1)  # 1 is LineStrings
+    geom, index = shapely.get_coordinates(geom, return_index=True)
     no_mix = index[:-1] == index[1:]  # mask where LineStrings are not overlapping
     dist = haversine_dist(geom[:-1, 0], geom[:-1, 1], geom[1:, 0], geom[1:, 1])
     return np.bincount((index[:-1])[no_mix], weights=dist[no_mix])
```

### Comparing `trackintel-1.2.1/trackintel/geogr/point_distances.py` & `trackintel-1.2.2/trackintel/geogr/point_distances.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/trackintel/io/__init__.py` & `trackintel-1.2.2/trackintel/io/__init__.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/trackintel/io/dataset_reader.py` & `trackintel-1.2.2/trackintel/io/dataset_reader.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/trackintel/io/file.py` & `trackintel-1.2.2/trackintel/io/file.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/trackintel/io/from_geopandas.py` & `trackintel-1.2.2/trackintel/io/from_geopandas.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/trackintel/io/postgis.py` & `trackintel-1.2.2/trackintel/io/postgis.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/trackintel/model/locations.py` & `trackintel-1.2.2/trackintel/model/locations.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/trackintel/model/positionfixes.py` & `trackintel-1.2.2/trackintel/model/positionfixes.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/trackintel/model/staypoints.py` & `trackintel-1.2.2/trackintel/model/staypoints.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/trackintel/model/tours.py` & `trackintel-1.2.2/trackintel/model/tours.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/trackintel/model/triplegs.py` & `trackintel-1.2.2/trackintel/model/triplegs.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/trackintel/model/trips.py` & `trackintel-1.2.2/trackintel/model/trips.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/trackintel/model/util.py` & `trackintel-1.2.2/trackintel/model/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,15 @@
     """
     pfs = positionfixes.copy()
     is_planar_crs = ti.geogr.distances.check_gdf_planar(pfs)
 
     g = pfs.geometry
     # get distance and time difference
     if is_planar_crs:
-        with warnings.catch_warnings():
-            warnings.filterwarnings("ignore", message="CRS not set for some of the concatenation inputs.*")
-
-            dist = g.distance(g.shift(1)).to_numpy()
+        dist = g.distance(g.shift(1)).to_numpy()
     else:
         x = g.x.to_numpy()
         y = g.y.to_numpy()
         dist = np.zeros(len(pfs), dtype=np.float64)
         dist[1:] = haversine_dist(x[:-1], y[:-1], x[1:], y[1:])
 
     time_delta = (pfs["tracked_at"] - pfs["tracked_at"].shift(1)).dt.total_seconds().to_numpy()
```

### Comparing `trackintel-1.2.1/trackintel/preprocessing/filter.py` & `trackintel-1.2.2/trackintel/preprocessing/filter.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/trackintel/preprocessing/positionfixes.py` & `trackintel-1.2.2/trackintel/preprocessing/positionfixes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import datetime
 import warnings
 
 import geopandas as gpd
 import numpy as np
 import pandas as pd
+from tqdm import tqdm
 from shapely.geometry import LineString
 
 from trackintel.geogr.distances import check_gdf_planar, haversine_dist
 from trackintel.preprocessing.util import _explode_agg, angle_centroid_multipoints, applyParallel
 
 
 def generate_staypoints(
@@ -166,14 +167,15 @@
 
 
 def generate_triplegs(
     positionfixes,
     staypoints=None,
     method="between_staypoints",
     gap_threshold=15,
+    print_progress=False,
 ):
     """Generate triplegs from positionfixes.
 
     Parameters
     ----------
     positionfixes : GeoDataFrame (as trackintel positionfixes)
         The positionfixes have to follow the standard definition for positionfixes DataFrames.
@@ -188,14 +190,17 @@
         between two staypoints (no overlap). This method requires either a column 'staypoint_id' on
         the positionfixes or passing staypoints as an input.
 
     gap_threshold: float, default 15 (minutes)
         Maximum allowed temporal gap size in minutes. If tracking data is missing for more than
         `gap_threshold` minutes, a new tripleg will be generated.
 
+    print_progress: boolean, default False
+        Show the progress bar for assigning staypoints to positionfixes if set to True.
+
     Returns
     -------
     pfs: GeoDataFrame (as trackintel positionfixes)
         The original positionfixes with a new column ``[`tripleg_id`]``.
 
     tpls: GeoDataFrame (as trackintel triplegs)
         The generated triplegs.
@@ -240,15 +245,19 @@
         # - step 1: Assign staypoint ids to positionfixes by matching timestamps (per user)
         # - step 2: Find first positionfix after a staypoint
         # (relevant if the pfs of sp are not provided, and we can only infer the pfs after sp through time)
         if case == 2:
             # initialize the index list of pfs where a tpl will begin
             insert_index_ls = []
             pfs["staypoint_id"] = pd.NA
-            for user_id_this in pfs["user_id"].unique():
+
+            # initalize the variable 'disable' to control display of progress bar.
+            disable = not print_progress
+
+            for user_id_this in tqdm(pfs["user_id"].unique(), disable=disable):
                 sp_user = staypoints[staypoints["user_id"] == user_id_this]
                 pfs_user = pfs[pfs["user_id"] == user_id_this]
 
                 # step 1
                 # All positionfixes with timestamp between staypoints are assigned the value 0
                 # Intersect all positionfixes of a user with all staypoints of the same user
                 intervals = pd.IntervalIndex.from_arrays(sp_user["started_at"], sp_user["finished_at"], closed="left")
@@ -272,15 +281,15 @@
         # pd.NA will be replaced later with tripleg ids
         pfs["tripleg_id"] = pd.NA
         pfs.loc[~pd.isna(pfs["staypoint_id"]), "tripleg_id"] = -1
 
         # get all conditions that trigger a new tripleg.
         # condition 1: a positionfix belongs to a new tripleg if the user changes. For this we need to sort pfs.
         # The first positionfix of the new user is the start of a new tripleg (if it is no staypoint)
-        cond_new_user = ((pfs["user_id"] - pfs["user_id"].shift(1)) != 0) & pd.isna(pfs["staypoint_id"])
+        cond_new_user = (pfs["user_id"] != pfs["user_id"].shift(1)) & pd.isna(pfs["staypoint_id"])
 
         # condition 2: Temporal gaps
         # if there is a gap that is longer than gap_threshold minutes, we start a new tripleg
         cond_gap = pfs["tracked_at"] - pfs["tracked_at"].shift(1) > datetime.timedelta(minutes=gap_threshold)
 
         # condition 3: staypoint
         # By our definition the pf after a stp is the first pf of a tpl.
```

### Comparing `trackintel-1.2.1/trackintel/preprocessing/staypoints.py` & `trackintel-1.2.2/trackintel/preprocessing/staypoints.py`

 * *Files 3% similar despite different names*

```diff
@@ -266,20 +266,16 @@
     tpls_merge["type"] = "tripleg"
     sp_merge["type"] = "staypoint"
     # convert datatypes in order to preserve the datatypes (especially ints) despite of NaNs during concat
     sp_merge = sp_merge.convert_dtypes()
 
     # a joined dataframe sp_tpls is constructed to add the columns 'type' and 'next_type' to the 'sp_merge' table
     # concat and sort by time
-    with warnings.catch_warnings():
-        warnings.filterwarnings("ignore", message="CRS not set for some of the concatenation inputs.*")
-
-        # TODO: the warning relates to how we process when no triplegs is provided. In future versions,
-        # we want to seperate the two scenarios. See issue #463.
-        sp_tpls = pd.concat([sp_merge, tpls_merge]).sort_values(by=["user_id", "started_at"])
+    sp_tpls = pd.concat([sp_merge, tpls_merge]).sort_values(by=["user_id", "started_at"])
+    # TODO: we want to make tpls as argumtent optional and adapt this logic here. See issue #463.
     sp_tpls.index.rename(index_name, inplace=True)
     # get information whether the there is a tripleg after a staypoint
     sp_tpls["next_type"] = sp_tpls["type"].shift(-1)
     # get only staypoints, but with next type information
     sp_merge = sp_tpls[sp_tpls["type"] == "staypoint"]
 
     # reset index and make temporary index
```

### Comparing `trackintel-1.2.1/trackintel/preprocessing/triplegs.py` & `trackintel-1.2.2/trackintel/preprocessing/triplegs.py`

 * *Files 8% similar despite different names*

```diff
@@ -128,34 +128,26 @@
     user_change["started_at"] = sp_tpls.loc[condition_new_user, "started_at"] - gap_threshold / 2
     user_change[["type", "is_activity"]] = ["user_change", True]  # nicer for debugging
 
     # merge trips with (filler) activities
     trips.drop(columns=["type", "sp_tpls_id"], inplace=True)  # make space so no overlap with activity "sp_tpls_id"
     # Inserting `gaps` and `user_change` into the dataframe creates buffers that catch shifted
     # "staypoint_id" and "trip_id" from corrupting staypoints/trips.
-    with warnings.catch_warnings():
-        warnings.filterwarnings("ignore", message="CRS not set for some of the concatenation inputs.*")
-
-        # TODO: the warning might be caused from process within geopandas. Remember to check
-        # if the warning persists in later versions.
-        trips_with_act = pd.concat((trips, sp_tpls_only_act, gaps, user_change), axis=0, ignore_index=True)
+    trips_with_act = pd.concat((trips, sp_tpls_only_act, gaps, user_change), axis=0, ignore_index=True)
     trips_with_act.sort_values(["user_id", "started_at"], inplace=True)
 
     # ID assignment #
     # add origin/destination ids by shifting
     trips_with_act["origin_staypoint_id"] = trips_with_act["sp_tpls_id"].shift(1)
     trips_with_act["destination_staypoint_id"] = trips_with_act["sp_tpls_id"].shift(-1)
 
     # add geometry for start and end points
     if add_geometry:
-        with warnings.catch_warnings():
-            warnings.filterwarnings("ignore", message="CRS not set for some of the concatenation inputs.*")
-
-            trips_with_act["origin_geom"] = trips_with_act["geom"].shift(1)
-            trips_with_act["destination_geom"] = trips_with_act["geom"].shift(-1)
+        trips_with_act["origin_geom"] = trips_with_act["geom"].shift(1)
+        trips_with_act["destination_geom"] = trips_with_act["geom"].shift(-1)
 
     # add prev_trip_id and next_trip_id for is_activity staypoints
     trips_with_act["prev_trip_id"] = trips_with_act["trip_id"].shift(1)
     trips_with_act["next_trip_id"] = trips_with_act["trip_id"].shift(-1)
 
     # transform column to binary
     trips_with_act["is_activity"].fillna(False, inplace=True)
```

### Comparing `trackintel-1.2.1/trackintel/preprocessing/trips.py` & `trackintel-1.2.2/trackintel/preprocessing/trips.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/trackintel/preprocessing/util.py` & `trackintel-1.2.2/trackintel/preprocessing/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import timedelta
 
 import geopandas as gpd
 import numpy as np
 import pandas as pd
-import pygeos
+import shapely
 from joblib import Parallel, delayed
 from shapely.geometry.base import BaseGeometry
 from tqdm import tqdm
 
 
 def calc_temp_overlap(start_1, end_1, start_2, end_2):
     """
@@ -123,16 +123,15 @@
         Should contain only Points or MultiPoints any other lead to wrong results.
 
     Returns
     -------
     geopandas.GeometryArray
         Centroid of geometries (shapely.Point)
     """
-    g = pygeos.from_shapely(geometry)
-    g, index = pygeos.get_coordinates(g, return_index=True)
+    g, index = shapely.get_coordinates(geometry, return_index=True)
     # number of coordinate pairs per MultiPoint
     count = np.bincount(index)
     x, y = g[:, 0], g[:, 1]
     # calculate mean of y Coordinates -> no wrapping
     y = np.bincount(index, weights=y) / count
     # calculate mean of x Coordinates with wrapping
     x_rad = np.deg2rad(x)
```

### Comparing `trackintel-1.2.1/trackintel/visualization/locations.py` & `trackintel-1.2.2/trackintel/visualization/locations.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/trackintel/visualization/modal_split.py` & `trackintel-1.2.2/trackintel/visualization/modal_split.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/trackintel/visualization/osm.py` & `trackintel-1.2.2/trackintel/visualization/osm.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/trackintel/visualization/positionfixes.py` & `trackintel-1.2.2/trackintel/visualization/positionfixes.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/trackintel/visualization/staypoints.py` & `trackintel-1.2.2/trackintel/visualization/staypoints.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/trackintel/visualization/triplegs.py` & `trackintel-1.2.2/trackintel/visualization/triplegs.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/trackintel/visualization/util.py` & `trackintel-1.2.2/trackintel/visualization/util.py`

 * *Files identical despite different names*

### Comparing `trackintel-1.2.1/trackintel.egg-info/PKG-INFO` & `trackintel-1.2.2/trackintel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trackintel
-Version: 1.2.1
+Version: 1.2.2
 Summary: Human mobility and movement analysis framework.
 Home-page: https://github.com/mie-lab/trackintel
 Author: Dominik Bucher, Henry Martin, Ye Hong
 Author-email: dobucher@ethz.ch, martinhe@ethz.ch
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -23,15 +23,15 @@
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/trackintel.svg)](https://anaconda.org/conda-forge/trackintel)
 [![Actions Status](https://github.com/mie-lab/trackintel/workflows/Tests/badge.svg)](https://github.com/mie-lab/trackintel/actions?query=workflow%3ATests)
 [![Documentation Status](https://readthedocs.org/projects/trackintel/badge/?version=latest)](https://trackintel.readthedocs.io/en/latest/?badge=latest)
 [![codecov.io](https://codecov.io/gh/mie-lab/trackintel/coverage.svg?branch=master)](https://codecov.io/gh/mie-lab/trackintel)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![asv](http://img.shields.io/badge/benchmarked%20by-asv-green.svg?style=flat)](https://mie-lab.github.io/trackintel/)
 
-*trackintel* is a library for the analysis of spatio-temporal tracking data with a focus on human mobility. The core of *trackintel* is the hierachical data model for movement data that is used in GIS, transport planning and related fields. We provide functionalities for the full life-cycle of human mobility data analysis: import and export of tracking data of different types (e.g, trackpoints, check-ins, trajectories), preprocessing, data quality assessment, semantic enrichment, quantitative analysis and mining tasks, and visualization of data and results.
+*trackintel* is a library for the analysis of spatio-temporal tracking data with a focus on human mobility. The core of *trackintel* is the hierarchical data model for movement data that is used in GIS, transport planning and related fields. We provide functionalities for the full life-cycle of human mobility data analysis: import and export of tracking data of different types (e.g, trackpoints, check-ins, trajectories), preprocessing, data quality assessment, semantic enrichment, quantitative analysis and mining tasks, and visualization of data and results.
 Trackintel is based on [Pandas](https://pandas.pydata.org/) and [GeoPandas](https://geopandas.org/#). 
 
 You can find the documentation on the [trackintel documentation page](https://trackintel.readthedocs.io/en/latest). 
 
 Try *trackintel* online in a MyBinder notebook: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mie-lab/trackintel/HEAD?filepath=%2Fexamples%2Ftrackintel_basic_tutorial.ipynb)
 
 Please star this repo and [cite](#citelink) our paper if you find our work is helpful for you.
@@ -139,15 +139,14 @@
 * Pint
 * NetworkX
 * GeoAlchemy2
 * scikit-learn
 * tqdm
 * OSMnx
 * similaritymeasures
-* pygeos
 
 ## Development
 You can find the development roadmap under `ROADMAP.md` and further development guidelines under `CONTRIBUTING.md`.
 
 ## Contributors
 
 *trackintel* is primarily maintained by the Mobility Information Engineering Lab at ETH Zurich ([mie-lab.ethz.ch](http://mie-lab.ethz.ch)).
```

### Comparing `trackintel-1.2.1/trackintel.egg-info/SOURCES.txt` & `trackintel-1.2.2/trackintel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

