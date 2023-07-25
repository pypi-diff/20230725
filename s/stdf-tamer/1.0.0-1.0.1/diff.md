# Comparing `tmp/stdf_tamer-1.0.0.tar.gz` & `tmp/stdf_tamer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stdf_tamer-1.0.0.tar", last modified: Tue Jul 25 14:59:46 2023, max compression
+gzip compressed data, was "stdf_tamer-1.0.1.tar", last modified: Tue Jul 25 15:05:21 2023, max compression
```

## Comparing `stdf_tamer-1.0.0.tar` & `stdf_tamer-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    11558 2023-07-06 13:14:13.436374 stdf_tamer-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0      915 2023-07-25 14:59:46.378608 stdf_tamer-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      151 2022-12-19 08:36:15.991971 stdf_tamer-1.0.0/src/_ams_rw_stdf_writer_state.py
--rw-r--r--   0        0        0    24533 2023-07-23 10:26:23.075896 stdf_tamer-1.0.0/src/ams_rw_stdf.py
--rw-r--r--   0        0        0    16086 2023-07-22 10:05:33.495555 stdf_tamer-1.0.0/src/ams_rw_stdf_writer.py
--rw-r--r--   0        0        0     4332 2023-07-25 13:49:56.954726 stdf_tamer-1.0.0/src/converter.py
--rw-r--r--   0        0        0     1549 2023-03-09 16:19:36.796549 stdf_tamer-1.0.0/src/create_index_at_dropzone.py
--rw-r--r--   0        0        0      488 2022-12-19 08:36:10.856733 stdf_tamer-1.0.0/src/example.py
--rw-r--r--   0        0        0     2148 2023-07-06 13:14:13.461501 stdf_tamer-1.0.0/src/simulator.py
--rw-r--r--   0        0        0      731 2023-07-23 10:24:08.230092 stdf_tamer-1.0.0/src/stdfanalyser.py
--rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 stdf_tamer-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-07-06 13:14:13.436374 stdf_tamer-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0      422 2023-07-25 14:39:05.133046 stdf_tamer-1.0.1/README.md
+-rw-r--r--   0        0        0     1140 2023-07-25 15:05:21.933876 stdf_tamer-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      151 2022-12-19 08:36:15.991971 stdf_tamer-1.0.1/src/_ams_rw_stdf_writer_state.py
+-rw-r--r--   0        0        0    24533 2023-07-23 10:26:23.075896 stdf_tamer-1.0.1/src/ams_rw_stdf.py
+-rw-r--r--   0        0        0    16086 2023-07-22 10:05:33.495555 stdf_tamer-1.0.1/src/ams_rw_stdf_writer.py
+-rw-r--r--   0        0        0     4332 2023-07-25 13:49:56.954726 stdf_tamer-1.0.1/src/converter.py
+-rw-r--r--   0        0        0     1549 2023-03-09 16:19:36.796549 stdf_tamer-1.0.1/src/create_index_at_dropzone.py
+-rw-r--r--   0        0        0      488 2022-12-19 08:36:10.856733 stdf_tamer-1.0.1/src/example.py
+-rw-r--r--   0        0        0     2148 2023-07-06 13:14:13.461501 stdf_tamer-1.0.1/src/simulator.py
+-rw-r--r--   0        0        0      731 2023-07-23 10:24:08.230092 stdf_tamer-1.0.1/src/stdfanalyser.py
+-rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 stdf_tamer-1.0.1/PKG-INFO
```

### Comparing `stdf_tamer-1.0.0/LICENSE.txt` & `stdf_tamer-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stdf_tamer-1.0.0/src/ams_rw_stdf.py` & `stdf_tamer-1.0.1/src/ams_rw_stdf.py`

 * *Files identical despite different names*

### Comparing `stdf_tamer-1.0.0/src/ams_rw_stdf_writer.py` & `stdf_tamer-1.0.1/src/ams_rw_stdf_writer.py`

 * *Files identical despite different names*

### Comparing `stdf_tamer-1.0.0/src/converter.py` & `stdf_tamer-1.0.1/src/converter.py`

 * *Files identical despite different names*

### Comparing `stdf_tamer-1.0.0/src/create_index_at_dropzone.py` & `stdf_tamer-1.0.1/src/create_index_at_dropzone.py`

 * *Files identical despite different names*

### Comparing `stdf_tamer-1.0.0/src/simulator.py` & `stdf_tamer-1.0.1/src/simulator.py`

 * *Files identical despite different names*

### Comparing `stdf_tamer-1.0.0/src/stdfanalyser.py` & `stdf_tamer-1.0.1/src/stdfanalyser.py`

 * *Files identical despite different names*

