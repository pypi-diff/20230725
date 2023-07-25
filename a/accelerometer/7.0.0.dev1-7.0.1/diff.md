# Comparing `tmp/accelerometer-7.0.0.dev1.tar.gz` & `tmp/accelerometer-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelerometer-7.0.0.dev1.tar", last modified: Tue May  9 20:36:47 2023, max compression
+gzip compressed data, was "accelerometer-7.0.1.tar", last modified: Tue Jul 25 08:32:15 2023, max compression
```

## Comparing `accelerometer-7.0.0.dev1.tar` & `accelerometer-7.0.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:36:47.929013 accelerometer-7.0.0.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-05-09 20:36:47.929013 accelerometer-7.0.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 20:36:47.929013 accelerometer-7.0.0.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:36:47.921013 accelerometer-7.0.0.dev1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:36:47.929013 accelerometer-7.0.0.dev1/src/accelerometer/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-09 20:36:47.929013 accelerometer-7.0.0.dev1/src/accelerometer/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/accCollateSummary.py
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/accPlot.py
--rw-r--r--   0 runner    (1001) docker     (123)    20172 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/accProcess.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/accWriteCmds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:36:47.925013 accelerometer-7.0.0.dev1/src/accelerometer/activityModels/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/activityModels/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/circadian.py
--rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    22477 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:36:47.929013 accelerometer-7.0.0.dev1/src/accelerometer/java/
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-05-09 20:36:33.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/AccStats.class
--rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/AccStats.java
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-09 20:36:33.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/AccelerometerParser.class
--rw-r--r--   0 runner    (1001) docker     (123)    10305 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/AccelerometerParser.java
--rw-r--r--   0 runner    (1001) docker     (123)    11988 2023-05-09 20:36:33.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/ActigraphReader.class
--rw-r--r--   0 runner    (1001) docker     (123)    29730 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/ActigraphReader.java
--rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-05-09 20:36:33.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/AxivityReader.class
--rw-r--r--   0 runner    (1001) docker     (123)    16174 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/AxivityReader.java
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-09 20:36:33.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/BandpassFilter.class
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/BandpassFilter.java
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-09 20:36:33.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/CsvReader.class
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/CsvReader.java
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-05-09 20:36:33.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/DeviceReader.class
--rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/DeviceReader.java
--rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-05-09 20:36:33.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/EpochWriter.class
--rw-r--r--   0 runner    (1001) docker     (123)    15684 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/EpochWriter.java
--rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-05-09 20:36:33.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/Features.class
--rw-r--r--   0 runner    (1001) docker     (123)    24365 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/Features.java
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-09 20:36:33.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/Filter.class
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/Filter.java
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-09 20:36:33.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/GENEActivReader.class
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/GENEActivReader.java
--rw-r--r--   0 runner    (1001) docker     (123)  1501730 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/JTransforms-3.1-with-dependencies.jar
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-09 20:36:33.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/LowpassFilter.class
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/LowpassFilter.java
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-05-09 20:36:33.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/NpyWriter.class
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/NpyWriter.java
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-09 20:36:34.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/Resample.class
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/Resample.java
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/java/logging.properties
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/summarisation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15015 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/src/accelerometer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 20:36:47.925013 accelerometer-7.0.0.dev1/src/accelerometer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-05-09 20:36:47.000000 accelerometer-7.0.0.dev1/src/accelerometer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-09 20:36:47.000000 accelerometer-7.0.0.dev1/src/accelerometer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 20:36:47.000000 accelerometer-7.0.0.dev1/src/accelerometer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-09 20:36:47.000000 accelerometer-7.0.0.dev1/src/accelerometer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-09 20:36:47.000000 accelerometer-7.0.0.dev1/src/accelerometer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 20:36:47.000000 accelerometer-7.0.0.dev1/src/accelerometer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-05-09 20:36:28.000000 accelerometer-7.0.0.dev1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:15.490905 accelerometer-7.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-07-25 08:31:56.000000 accelerometer-7.0.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-25 08:31:56.000000 accelerometer-7.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-07-25 08:32:15.490905 accelerometer-7.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-25 08:31:56.000000 accelerometer-7.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-07-25 08:31:56.000000 accelerometer-7.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 08:32:15.490905 accelerometer-7.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-25 08:31:56.000000 accelerometer-7.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:15.482905 accelerometer-7.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:15.490905 accelerometer-7.0.1/src/accelerometer/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-25 08:31:56.000000 accelerometer-7.0.1/src/accelerometer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-25 08:32:15.490905 accelerometer-7.0.1/src/accelerometer/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-25 08:31:56.000000 accelerometer-7.0.1/src/accelerometer/accCollateSummary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-07-25 08:31:56.000000 accelerometer-7.0.1/src/accelerometer/accPlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20172 2023-07-25 08:31:56.000000 accelerometer-7.0.1/src/accelerometer/accProcess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-25 08:31:56.000000 accelerometer-7.0.1/src/accelerometer/accWriteCmds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:15.486905 accelerometer-7.0.1/src/accelerometer/activityModels/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-25 08:31:56.000000 accelerometer-7.0.1/src/accelerometer/activityModels/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-07-25 08:31:56.000000 accelerometer-7.0.1/src/accelerometer/circadian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-07-25 08:31:56.000000 accelerometer-7.0.1/src/accelerometer/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22477 2023-07-25 08:31:56.000000 accelerometer-7.0.1/src/accelerometer/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:15.490905 accelerometer-7.0.1/src/accelerometer/java/
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-25 08:32:01.000000 accelerometer-7.0.1/src/accelerometer/java/AccStats.class
+-rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-07-25 08:31:56.000000 accelerometer-7.0.1/src/accelerometer/java/AccStats.java
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-25 08:32:01.000000 accelerometer-7.0.1/src/accelerometer/java/AccelerometerParser.class
+-rw-r--r--   0 runner    (1001) docker     (123)    10305 2023-07-25 08:31:56.000000 accelerometer-7.0.1/src/accelerometer/java/AccelerometerParser.java
+-rw-r--r--   0 runner    (1001) docker     (123)    11988 2023-07-25 08:32:02.000000 accelerometer-7.0.1/src/accelerometer/java/ActigraphReader.class
+-rw-r--r--   0 runner    (1001) docker     (123)    29730 2023-07-25 08:31:56.000000 accelerometer-7.0.1/src/accelerometer/java/ActigraphReader.java
+-rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-07-25 08:32:02.000000 accelerometer-7.0.1/src/accelerometer/java/AxivityReader.class
+-rw-r--r--   0 runner    (1001) docker     (123)    16174 2023-07-25 08:31:56.000000 accelerometer-7.0.1/src/accelerometer/java/AxivityReader.java
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-25 08:32:02.000000 accelerometer-7.0.1/src/accelerometer/java/BandpassFilter.class
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-25 08:31:56.000000 accelerometer-7.0.1/src/accelerometer/java/BandpassFilter.java
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-25 08:32:02.000000 accelerometer-7.0.1/src/accelerometer/java/CsvReader.class
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-07-25 08:31:56.000000 accelerometer-7.0.1/src/accelerometer/java/CsvReader.java
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-07-25 08:32:02.000000 accelerometer-7.0.1/src/accelerometer/java/DeviceReader.class
+-rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-07-25 08:31:56.000000 accelerometer-7.0.1/src/accelerometer/java/DeviceReader.java
+-rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-07-25 08:32:02.000000 accelerometer-7.0.1/src/accelerometer/java/EpochWriter.class
+-rw-r--r--   0 runner    (1001) docker     (123)    15684 2023-07-25 08:31:56.000000 accelerometer-7.0.1/src/accelerometer/java/EpochWriter.java
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-07-25 08:32:02.000000 accelerometer-7.0.1/src/accelerometer/java/Features.class
+-rw-r--r--   0 runner    (1001) docker     (123)    24365 2023-07-25 08:31:56.000000 accelerometer-7.0.1/src/accelerometer/java/Features.java
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-25 08:32:01.000000 accelerometer-7.0.1/src/accelerometer/java/Filter.class
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-25 08:31:56.000000 accelerometer-7.0.1/src/accelerometer/java/Filter.java
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-25 08:32:02.000000 accelerometer-7.0.1/src/accelerometer/java/GENEActivReader.class
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-07-25 08:31:56.000000 accelerometer-7.0.1/src/accelerometer/java/GENEActivReader.java
+-rw-r--r--   0 runner    (1001) docker     (123)  1501730 2023-07-25 08:31:56.000000 accelerometer-7.0.1/src/accelerometer/java/JTransforms-3.1-with-dependencies.jar
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-07-25 08:32:02.000000 accelerometer-7.0.1/src/accelerometer/java/LowpassFilter.class
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-07-25 08:31:56.000000 accelerometer-7.0.1/src/accelerometer/java/LowpassFilter.java
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-07-25 08:32:02.000000 accelerometer-7.0.1/src/accelerometer/java/NpyWriter.class
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-07-25 08:31:56.000000 accelerometer-7.0.1/src/accelerometer/java/NpyWriter.java
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-25 08:31:56.000000 accelerometer-7.0.1/src/accelerometer/java/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-25 08:32:02.000000 accelerometer-7.0.1/src/accelerometer/java/Resample.class
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-07-25 08:31:56.000000 accelerometer-7.0.1/src/accelerometer/java/Resample.java
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-25 08:31:57.000000 accelerometer-7.0.1/src/accelerometer/java/logging.properties
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-25 08:31:57.000000 accelerometer-7.0.1/src/accelerometer/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-07-25 08:31:57.000000 accelerometer-7.0.1/src/accelerometer/summarisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15015 2023-07-25 08:31:57.000000 accelerometer-7.0.1/src/accelerometer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:15.486905 accelerometer-7.0.1/src/accelerometer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-07-25 08:32:15.000000 accelerometer-7.0.1/src/accelerometer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-25 08:32:15.000000 accelerometer-7.0.1/src/accelerometer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 08:32:15.000000 accelerometer-7.0.1/src/accelerometer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-25 08:32:15.000000 accelerometer-7.0.1/src/accelerometer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-25 08:32:15.000000 accelerometer-7.0.1/src/accelerometer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 08:32:15.000000 accelerometer-7.0.1/src/accelerometer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-07-25 08:31:57.000000 accelerometer-7.0.1/versioneer.py
```

### Comparing `accelerometer-7.0.0.dev1/LICENSE.md` & `accelerometer-7.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/PKG-INFO` & `accelerometer-7.0.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,70 +1,45 @@
-Metadata-Version: 2.1
-Name: accelerometer
-Version: 7.0.0.dev1
-Summary: A package to extract meaningful health information from large accelerometer datasets e.g. how much time individuals spend in sleep, sedentary behaviour, walking and moderate intensity physical activity
-Home-page: https://github.com/activityMonitoring/biobankAccelerometerAnalysis
-Download-URL: https://github.com/activityMonitoring/biobankAccelerometerAnalysis
-Author: Aiden Doherty, Shing Chan, Rosemary Walmsley, Hang Yuan
-Maintainer: Shing Chan
-Maintainer-email: shing.chan@ndph.ox.ac.uk
-License: See LICENSE.md
-Keywords: wearables,accelerometer,health data science,human activity recognition
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Requires-Python: >=3.7, <3.11
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
-License-File: LICENSE.md
-
 ![Accelerometer data processing overview](docs/source/accelerometerLogo.png)
 
 [![Github all releases](https://img.shields.io/github/release/activityMonitoring/biobankAccelerometerAnalysis.svg)](https://github.com/activityMonitoring/biobankAccelerometerAnalysis/releases/)
 ![install](https://github.com/activityMonitoring/biobankAccelerometerAnalysis/workflows/install/badge.svg)
 ![flake8](https://github.com/activityMonitoring/biobankAccelerometerAnalysis/workflows/flake8/badge.svg)
 ![junit](https://github.com/activityMonitoring/biobankAccelerometerAnalysis/workflows/junit/badge.svg)
 ![gt3x](https://github.com/activityMonitoring/biobankAccelerometerAnalysis/workflows/gt3x/badge.svg)
 ![cwa](https://github.com/activityMonitoring/biobankAccelerometerAnalysis/workflows/cwa/badge.svg)
 
 A tool to extract meaningful health information from large accelerometer datasets. The software generates time-series and summary metrics useful for answering key questions such as how much time is spent in sleep, sedentary behaviour, or doing physical activity.
 
-## Installation
-
-```bash
-pip install accelerometer
-```
+## Install
 
-You also need Java 8 (1.8.0) or greater. Check with the following:
+We recommend using **Anaconda**:
 
-```bash
-java -version
-```
+1. Download & install [Miniconda](https://docs.conda.io/en/latest/miniconda.html) (light-weight version of Anaconda).
+1. (Windows) Once installed, launch the **Anaconda Prompt**.
+1. Create a virtual environment:
+    ```console
+    $ conda create -n accelerometer python=3.9 openjdk pip
+    ```
+    This creates a virtual environment called `accelerometer` with Python version 3.9, OpenJDK, and Pip.
+1. Activate the environment:
+    ```console
+    $ conda activate accelerometer
+    ```
+    You should now see `(accelerometer)` written in front of your prompt.
+1. Install `accelerometer`:
+    ```console
+    $ pip install accelerometer
+    ```
 
-You can try the following to check that everything works properly:
-```bash
-# Create an isolated environment
-$ mkdir test_baa/ ; cd test_baa/
-$ python -m venv baa
-$ source baa/bin/activate
-
-# Install and test
-$ pip install accelerometer
-$ wget -P data/ http://gas.ndph.ox.ac.uk/aidend/accModels/sample.cwa.gz  # download a sample file
-$ accProcess data/sample.cwa.gz
-$ accPlot data/sample-timeSeries.csv.gz
-```
+You are all set! The next time that you want to use `accelerometer`, open the Anaconda Prompt and activate the environment (step 4). If you see `(accelerometer)` in front of your prompt, you are ready to go!
 
 ## Usage
 To extract summary movement statistics from an Axivity file (.cwa):
 
-```bash
+```console
 $ accProcess data/sample.cwa.gz
 
  <output written to data/sample-outputSummary.json>
  <time series output written to data/sample-timeSeries.csv.gz>
 ```
 
 Movement statistics will be stored in a JSON file:
@@ -80,21 +55,26 @@
 }
 ```
 
 See [Data Dictionary](https://biobankaccanalysis.readthedocs.io/en/latest/datadict.html) for the list of output variables.
 
 Actigraph and GENEActiv files are also supported, as well as custom CSV files. See [Usage](https://biobankaccanalysis.readthedocs.io/en/latest/usage.html#basic-usage) for more details.
 
-To visualise the activity profile:
-```bash
+To plot the activity profile:
+```console
 $ accPlot data/sample-timeSeries.csv.gz
  <output plot written to data/sample-timeSeries-plot.png>
 ```
 ![Time series plot](docs/source/samplePlot.png)
 
+### Troubleshooting 
+Some systems may face issues with Java when running the script. If this is your case, try fixing OpenJDK to version 8:
+```console
+$ conda install -n accelerometer openjdk=8
+```
 
 ## Under the hood
 Interpreted levels of physical activity can vary, as many approaches can be
 taken to extract summary physical activity information from raw accelerometer
 data. To minimise error and bias, our tool uses published methods to calibrate,
 resample, and summarise the accelerometer data.
```

### Comparing `accelerometer-7.0.0.dev1/pyproject.toml` & `accelerometer-7.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/setup.py` & `accelerometer-7.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         'scipy==1.7.*',
         'matplotlib==3.5.*',
         'pandas==1.3.*',
         'tqdm==4.65.*',
         'statsmodels==0.13.*',
         'joblib==1.1.*',
         'imbalanced-learn==0.8.1',
-        'scikit-learn==1.0.1',
+        'scikit-learn==1.0.2',
     ],
     extras_require={
         "dev": [
             "flake8",
             "autopep8",
             "ipython",
             "ipdb",
```

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/accPlot.py` & `accelerometer-7.0.1/src/accelerometer/accPlot.py`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/accProcess.py` & `accelerometer-7.0.1/src/accelerometer/accProcess.py`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/accWriteCmds.py` & `accelerometer-7.0.1/src/accelerometer/accWriteCmds.py`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/circadian.py` & `accelerometer-7.0.1/src/accelerometer/circadian.py`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/classification.py` & `accelerometer-7.0.1/src/accelerometer/classification.py`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/device.py` & `accelerometer-7.0.1/src/accelerometer/device.py`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/java/AccStats.class` & `accelerometer-7.0.1/src/accelerometer/java/AccStats.class`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/java/AccStats.java` & `accelerometer-7.0.1/src/accelerometer/java/AccStats.java`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/java/AccelerometerParser.class` & `accelerometer-7.0.1/src/accelerometer/java/AccelerometerParser.class`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/java/AccelerometerParser.java` & `accelerometer-7.0.1/src/accelerometer/java/AccelerometerParser.java`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/java/ActigraphReader.class` & `accelerometer-7.0.1/src/accelerometer/java/ActigraphReader.class`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/java/ActigraphReader.java` & `accelerometer-7.0.1/src/accelerometer/java/ActigraphReader.java`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/java/AxivityReader.class` & `accelerometer-7.0.1/src/accelerometer/java/AxivityReader.class`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/java/AxivityReader.java` & `accelerometer-7.0.1/src/accelerometer/java/AxivityReader.java`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/java/BandpassFilter.class` & `accelerometer-7.0.1/src/accelerometer/java/BandpassFilter.class`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/java/BandpassFilter.java` & `accelerometer-7.0.1/src/accelerometer/java/BandpassFilter.java`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/java/CsvReader.class` & `accelerometer-7.0.1/src/accelerometer/java/CsvReader.class`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/java/CsvReader.java` & `accelerometer-7.0.1/src/accelerometer/java/CsvReader.java`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/java/DeviceReader.class` & `accelerometer-7.0.1/src/accelerometer/java/DeviceReader.class`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/java/DeviceReader.java` & `accelerometer-7.0.1/src/accelerometer/java/DeviceReader.java`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/java/EpochWriter.class` & `accelerometer-7.0.1/src/accelerometer/java/EpochWriter.class`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/java/EpochWriter.java` & `accelerometer-7.0.1/src/accelerometer/java/EpochWriter.java`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/java/Features.class` & `accelerometer-7.0.1/src/accelerometer/java/Features.class`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/java/Features.java` & `accelerometer-7.0.1/src/accelerometer/java/Features.java`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/java/Filter.class` & `accelerometer-7.0.1/src/accelerometer/java/Filter.class`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/java/Filter.java` & `accelerometer-7.0.1/src/accelerometer/java/Filter.java`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/java/GENEActivReader.class` & `accelerometer-7.0.1/src/accelerometer/java/GENEActivReader.class`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/java/GENEActivReader.java` & `accelerometer-7.0.1/src/accelerometer/java/GENEActivReader.java`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/java/JTransforms-3.1-with-dependencies.jar` & `accelerometer-7.0.1/src/accelerometer/java/JTransforms-3.1-with-dependencies.jar`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/java/LowpassFilter.class` & `accelerometer-7.0.1/src/accelerometer/java/LowpassFilter.class`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/java/LowpassFilter.java` & `accelerometer-7.0.1/src/accelerometer/java/LowpassFilter.java`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/java/NpyWriter.class` & `accelerometer-7.0.1/src/accelerometer/java/NpyWriter.class`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/java/NpyWriter.java` & `accelerometer-7.0.1/src/accelerometer/java/NpyWriter.java`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/java/Resample.class` & `accelerometer-7.0.1/src/accelerometer/java/Resample.class`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/java/Resample.java` & `accelerometer-7.0.1/src/accelerometer/java/Resample.java`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/models.py` & `accelerometer-7.0.1/src/accelerometer/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,33 +3,32 @@
 MODEL_DIR = pathlib.Path(__file__).parent / "models"
 MODEL_ROOT_URL = "https://wearables-files.ndph.ox.ac.uk/files/models/biobankAccelerometerAnalysis"
 
 
 MODELS = {
 
     'willetts': {
-        "pth": MODEL_DIR / "willetts" / "20220210.tar",
-        "url": f"{MODEL_ROOT_URL}/willetts/20220210.tar",
+        "pth": MODEL_DIR / "willetts" / "20220210_sk_1_0_2.tar",
+        "url": f"{MODEL_ROOT_URL}/willetts/20220210_sk_1_0_2.tar",
     },
 
     'doherty': {
-        "pth": MODEL_DIR / "doherty" / "20220210.tar",
-        "url": f"{MODEL_ROOT_URL}/doherty/20220210.tar",
+        "pth": MODEL_DIR / "doherty" / "20220210_sk_1_0_2.tar",
+        "url": f"{MODEL_ROOT_URL}/doherty/20220210_sk_1_0_2.tar",
     },
 
     'walmsley': {
-        "pth": MODEL_DIR / "walmsley" / "20220210.tar",
-        "url": f"{MODEL_ROOT_URL}/walmsley/20220210.tar",
+        "pth": MODEL_DIR / "walmsley" / "20220210_sk_1_0_2.tar",
+        "url": f"{MODEL_ROOT_URL}/walmsley/20220210_sk_1_0_2.tar",
     },
 
     'chan': {
-        "pth": MODEL_DIR / "chan" / "20230103.tar",
-        "url": f"{MODEL_ROOT_URL}/chan/20230103.tar",
-
+        "pth": MODEL_DIR / "chan" / "20230103_sk_1_0_2.tar",
+        "url": f"{MODEL_ROOT_URL}/chan/20230103_sk_1_0_2.tar",
     },
 
     'chanw': {
-        "pth": MODEL_DIR / "chanw" / "20230106.tar",
-        "url": f"{MODEL_ROOT_URL}/chanw/20230106.tar"
+        "pth": MODEL_DIR / "chanw" / "20230106_sk_1_0_2.tar",
+        "url": f"{MODEL_ROOT_URL}/chanw/20230106_sk_1_0_2.tar"
     },
 
 }
```

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/summarisation.py` & `accelerometer-7.0.1/src/accelerometer/summarisation.py`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer/utils.py` & `accelerometer-7.0.1/src/accelerometer/utils.py`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer.egg-info/PKG-INFO` & `accelerometer-7.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accelerometer
-Version: 7.0.0.dev1
+Version: 7.0.1
 Summary: A package to extract meaningful health information from large accelerometer datasets e.g. how much time individuals spend in sleep, sedentary behaviour, walking and moderate intensity physical activity
 Home-page: https://github.com/activityMonitoring/biobankAccelerometerAnalysis
 Download-URL: https://github.com/activityMonitoring/biobankAccelerometerAnalysis
 Author: Aiden Doherty, Shing Chan, Rosemary Walmsley, Hang Yuan
 Maintainer: Shing Chan
 Maintainer-email: shing.chan@ndph.ox.ac.uk
 License: See LICENSE.md
@@ -27,44 +27,41 @@
 ![flake8](https://github.com/activityMonitoring/biobankAccelerometerAnalysis/workflows/flake8/badge.svg)
 ![junit](https://github.com/activityMonitoring/biobankAccelerometerAnalysis/workflows/junit/badge.svg)
 ![gt3x](https://github.com/activityMonitoring/biobankAccelerometerAnalysis/workflows/gt3x/badge.svg)
 ![cwa](https://github.com/activityMonitoring/biobankAccelerometerAnalysis/workflows/cwa/badge.svg)
 
 A tool to extract meaningful health information from large accelerometer datasets. The software generates time-series and summary metrics useful for answering key questions such as how much time is spent in sleep, sedentary behaviour, or doing physical activity.
 
-## Installation
+## Install
 
-```bash
-pip install accelerometer
-```
+We recommend using **Anaconda**:
 
-You also need Java 8 (1.8.0) or greater. Check with the following:
+1. Download & install [Miniconda](https://docs.conda.io/en/latest/miniconda.html) (light-weight version of Anaconda).
+1. (Windows) Once installed, launch the **Anaconda Prompt**.
+1. Create a virtual environment:
+    ```console
+    $ conda create -n accelerometer python=3.9 openjdk pip
+    ```
+    This creates a virtual environment called `accelerometer` with Python version 3.9, OpenJDK, and Pip.
+1. Activate the environment:
+    ```console
+    $ conda activate accelerometer
+    ```
+    You should now see `(accelerometer)` written in front of your prompt.
+1. Install `accelerometer`:
+    ```console
+    $ pip install accelerometer
+    ```
 
-```bash
-java -version
-```
-
-You can try the following to check that everything works properly:
-```bash
-# Create an isolated environment
-$ mkdir test_baa/ ; cd test_baa/
-$ python -m venv baa
-$ source baa/bin/activate
-
-# Install and test
-$ pip install accelerometer
-$ wget -P data/ http://gas.ndph.ox.ac.uk/aidend/accModels/sample.cwa.gz  # download a sample file
-$ accProcess data/sample.cwa.gz
-$ accPlot data/sample-timeSeries.csv.gz
-```
+You are all set! The next time that you want to use `accelerometer`, open the Anaconda Prompt and activate the environment (step 4). If you see `(accelerometer)` in front of your prompt, you are ready to go!
 
 ## Usage
 To extract summary movement statistics from an Axivity file (.cwa):
 
-```bash
+```console
 $ accProcess data/sample.cwa.gz
 
  <output written to data/sample-outputSummary.json>
  <time series output written to data/sample-timeSeries.csv.gz>
 ```
 
 Movement statistics will be stored in a JSON file:
@@ -80,21 +77,26 @@
 }
 ```
 
 See [Data Dictionary](https://biobankaccanalysis.readthedocs.io/en/latest/datadict.html) for the list of output variables.
 
 Actigraph and GENEActiv files are also supported, as well as custom CSV files. See [Usage](https://biobankaccanalysis.readthedocs.io/en/latest/usage.html#basic-usage) for more details.
 
-To visualise the activity profile:
-```bash
+To plot the activity profile:
+```console
 $ accPlot data/sample-timeSeries.csv.gz
  <output plot written to data/sample-timeSeries-plot.png>
 ```
 ![Time series plot](docs/source/samplePlot.png)
 
+### Troubleshooting 
+Some systems may face issues with Java when running the script. If this is your case, try fixing OpenJDK to version 8:
+```console
+$ conda install -n accelerometer openjdk=8
+```
 
 ## Under the hood
 Interpreted levels of physical activity can vary, as many approaches can be
 taken to extract summary physical activity information from raw accelerometer
 data. To minimise error and bias, our tool uses published methods to calibrate,
 resample, and summarise the accelerometer data.
```

### Comparing `accelerometer-7.0.0.dev1/src/accelerometer.egg-info/SOURCES.txt` & `accelerometer-7.0.1/src/accelerometer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `accelerometer-7.0.0.dev1/versioneer.py` & `accelerometer-7.0.1/versioneer.py`

 * *Files identical despite different names*

