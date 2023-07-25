# Comparing `tmp/metar2bufr-0.0.2.24.tar.gz` & `tmp/metar2bufr-0.0.2.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metar2bufr-0.0.2.24.tar", last modified: Fri Jul 21 01:33:27 2023, max compression
+gzip compressed data, was "metar2bufr-0.0.2.25.tar", last modified: Tue Jul 25 01:43:32 2023, max compression
```

## Comparing `metar2bufr-0.0.2.24.tar` & `metar2bufr-0.0.2.25.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-21 01:33:27.352203 metar2bufr-0.0.2.24/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     1073 2023-07-13 16:23:37.000000 metar2bufr-0.0.2.24/LICENSE
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       39 2023-07-13 22:22:45.000000 metar2bufr-0.0.2.24/MANIFEST.in
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      623 2023-07-21 01:33:27.352203 metar2bufr-0.0.2.24/PKG-INFO
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       85 2023-07-13 16:24:38.000000 metar2bufr-0.0.2.24/README.md
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      764 2023-07-21 01:32:41.000000 metar2bufr-0.0.2.24/pyproject.toml
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       38 2023-07-21 01:33:27.352203 metar2bufr-0.0.2.24/setup.cfg
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-21 01:33:27.345203 metar2bufr-0.0.2.24/src/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-21 01:33:27.347203 metar2bufr-0.0.2.24/src/metar2bufr/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      164 2023-07-13 20:54:01.000000 metar2bufr-0.0.2.24/src/metar2bufr/__init__.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-21 01:33:27.348203 metar2bufr-0.0.2.24/src/metar2bufr/csv2bufr/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-21 01:33:27.345203 metar2bufr-0.0.2.24/src/metar2bufr/csv2bufr/build/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-21 01:33:27.345203 metar2bufr-0.0.2.24/src/metar2bufr/csv2bufr/build/lib/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-21 01:33:27.349202 metar2bufr-0.0.2.24/src/metar2bufr/csv2bufr/build/lib/csv2bufr/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    36767 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.24/src/metar2bufr/csv2bufr/build/lib/csv2bufr/__init__.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     4621 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.24/src/metar2bufr/csv2bufr/build/lib/csv2bufr/cli.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     7899 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.24/src/metar2bufr/csv2bufr/build/lib/csv2bufr/pygeoapi_plugin.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-21 01:33:27.349202 metar2bufr-0.0.2.24/src/metar2bufr/csv2bufr/csv2bufr/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    36767 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.24/src/metar2bufr/csv2bufr/csv2bufr/__init__.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     4621 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.24/src/metar2bufr/csv2bufr/csv2bufr/cli.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     7899 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.24/src/metar2bufr/csv2bufr/csv2bufr/pygeoapi_plugin.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-21 01:33:27.345203 metar2bufr-0.0.2.24/src/metar2bufr/csv2bufr/docs/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-21 01:33:27.350203 metar2bufr-0.0.2.24/src/metar2bufr/csv2bufr/docs/source/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3056 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.24/src/metar2bufr/csv2bufr/docs/source/conf.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3330 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.24/src/metar2bufr/csv2bufr/setup.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-21 01:33:27.350203 metar2bufr-0.0.2.24/src/metar2bufr/csv2bufr/tests/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     8502 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.24/src/metar2bufr/csv2bufr/tests/test_csv2bufr.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    25864 2023-07-21 01:32:07.000000 metar2bufr-0.0.2.24/src/metar2bufr/icao_bufr_encoder.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-21 01:33:27.351203 metar2bufr-0.0.2.24/src/metar2bufr/metarDecoder/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-13 17:15:28.000000 metar2bufr-0.0.2.24/src/metar2bufr/metarDecoder/__init__.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    59241 2023-07-13 20:20:04.000000 metar2bufr-0.0.2.24/src/metar2bufr/metarDecoder/metarDecoders.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    82209 2023-07-13 16:28:08.000000 metar2bufr-0.0.2.24/src/metar2bufr/metarDecoder/tpg.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     8261 2023-07-13 16:28:19.000000 metar2bufr-0.0.2.24/src/metar2bufr/metarDecoder/xmlConfig.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     6620 2023-07-13 20:39:39.000000 metar2bufr-0.0.2.24/src/metar2bufr/metarDecoder/xmlUtilities.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    23865 2023-07-17 23:02:50.000000 metar2bufr-0.0.2.24/src/metar2bufr/metar_bufr_encoder.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-21 01:33:27.351203 metar2bufr-0.0.2.24/src/metar2bufr/resources/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-13 22:08:27.000000 metar2bufr-0.0.2.24/src/metar2bufr/resources/__init__.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     2793 2023-07-20 23:18:14.000000 metar2bufr-0.0.2.24/src/metar2bufr/resources/icao-metar-mappings.json
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     2825 2023-07-13 16:29:37.000000 metar2bufr-0.0.2.24/src/metar2bufr/resources/metar-mappings.json
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3136 2023-07-13 16:29:37.000000 metar2bufr-0.0.2.24/src/metar2bufr/resources/metar-mappings2.json
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-21 01:33:27.348203 metar2bufr-0.0.2.24/src/metar2bufr.egg-info/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      623 2023-07-21 01:33:27.000000 metar2bufr-0.0.2.24/src/metar2bufr.egg-info/PKG-INFO
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     1107 2023-07-21 01:33:27.000000 metar2bufr-0.0.2.24/src/metar2bufr.egg-info/SOURCES.txt
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        1 2023-07-21 01:33:27.000000 metar2bufr-0.0.2.24/src/metar2bufr.egg-info/dependency_links.txt
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       11 2023-07-21 01:33:27.000000 metar2bufr-0.0.2.24/src/metar2bufr.egg-info/top_level.txt
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-25 01:43:32.557033 metar2bufr-0.0.2.25/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     1073 2023-07-13 16:23:37.000000 metar2bufr-0.0.2.25/LICENSE
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       39 2023-07-13 22:22:45.000000 metar2bufr-0.0.2.25/MANIFEST.in
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      623 2023-07-25 01:43:32.557033 metar2bufr-0.0.2.25/PKG-INFO
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       85 2023-07-13 16:24:38.000000 metar2bufr-0.0.2.25/README.md
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      764 2023-07-25 01:42:34.000000 metar2bufr-0.0.2.25/pyproject.toml
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       38 2023-07-25 01:43:32.558033 metar2bufr-0.0.2.25/setup.cfg
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-25 01:43:32.550033 metar2bufr-0.0.2.25/src/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-25 01:43:32.553033 metar2bufr-0.0.2.25/src/metar2bufr/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      164 2023-07-13 20:54:01.000000 metar2bufr-0.0.2.25/src/metar2bufr/__init__.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-25 01:43:32.554033 metar2bufr-0.0.2.25/src/metar2bufr/csv2bufr/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-25 01:43:32.551033 metar2bufr-0.0.2.25/src/metar2bufr/csv2bufr/build/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-25 01:43:32.551033 metar2bufr-0.0.2.25/src/metar2bufr/csv2bufr/build/lib/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-25 01:43:32.554033 metar2bufr-0.0.2.25/src/metar2bufr/csv2bufr/build/lib/csv2bufr/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    36767 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.25/src/metar2bufr/csv2bufr/build/lib/csv2bufr/__init__.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     4621 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.25/src/metar2bufr/csv2bufr/build/lib/csv2bufr/cli.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     7899 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.25/src/metar2bufr/csv2bufr/build/lib/csv2bufr/pygeoapi_plugin.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-25 01:43:32.555033 metar2bufr-0.0.2.25/src/metar2bufr/csv2bufr/csv2bufr/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    36767 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.25/src/metar2bufr/csv2bufr/csv2bufr/__init__.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     4621 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.25/src/metar2bufr/csv2bufr/csv2bufr/cli.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     7899 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.25/src/metar2bufr/csv2bufr/csv2bufr/pygeoapi_plugin.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-25 01:43:32.551033 metar2bufr-0.0.2.25/src/metar2bufr/csv2bufr/docs/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-25 01:43:32.555033 metar2bufr-0.0.2.25/src/metar2bufr/csv2bufr/docs/source/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3056 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.25/src/metar2bufr/csv2bufr/docs/source/conf.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3330 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.25/src/metar2bufr/csv2bufr/setup.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-25 01:43:32.555033 metar2bufr-0.0.2.25/src/metar2bufr/csv2bufr/tests/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     8502 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.25/src/metar2bufr/csv2bufr/tests/test_csv2bufr.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    26208 2023-07-25 01:42:00.000000 metar2bufr-0.0.2.25/src/metar2bufr/icao_bufr_encoder.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-25 01:43:32.556033 metar2bufr-0.0.2.25/src/metar2bufr/metarDecoder/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-13 17:15:28.000000 metar2bufr-0.0.2.25/src/metar2bufr/metarDecoder/__init__.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    59241 2023-07-13 20:20:04.000000 metar2bufr-0.0.2.25/src/metar2bufr/metarDecoder/metarDecoders.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    82209 2023-07-13 16:28:08.000000 metar2bufr-0.0.2.25/src/metar2bufr/metarDecoder/tpg.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     8261 2023-07-13 16:28:19.000000 metar2bufr-0.0.2.25/src/metar2bufr/metarDecoder/xmlConfig.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     6620 2023-07-13 20:39:39.000000 metar2bufr-0.0.2.25/src/metar2bufr/metarDecoder/xmlUtilities.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    23865 2023-07-17 23:02:50.000000 metar2bufr-0.0.2.25/src/metar2bufr/metar_bufr_encoder.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-25 01:43:32.557033 metar2bufr-0.0.2.25/src/metar2bufr/resources/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-13 22:08:27.000000 metar2bufr-0.0.2.25/src/metar2bufr/resources/__init__.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     2793 2023-07-20 23:18:14.000000 metar2bufr-0.0.2.25/src/metar2bufr/resources/icao-metar-mappings.json
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     2825 2023-07-13 16:29:37.000000 metar2bufr-0.0.2.25/src/metar2bufr/resources/metar-mappings.json
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3136 2023-07-13 16:29:37.000000 metar2bufr-0.0.2.25/src/metar2bufr/resources/metar-mappings2.json
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-25 01:43:32.553033 metar2bufr-0.0.2.25/src/metar2bufr.egg-info/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      623 2023-07-25 01:43:32.000000 metar2bufr-0.0.2.25/src/metar2bufr.egg-info/PKG-INFO
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     1107 2023-07-25 01:43:32.000000 metar2bufr-0.0.2.25/src/metar2bufr.egg-info/SOURCES.txt
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        1 2023-07-25 01:43:32.000000 metar2bufr-0.0.2.25/src/metar2bufr.egg-info/dependency_links.txt
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       11 2023-07-25 01:43:32.000000 metar2bufr-0.0.2.25/src/metar2bufr.egg-info/top_level.txt
```

### Comparing `metar2bufr-0.0.2.24/LICENSE` & `metar2bufr-0.0.2.25/LICENSE`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.24/PKG-INFO` & `metar2bufr-0.0.2.25/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metar2bufr
-Version: 0.0.2.24
+Version: 0.0.2.25
 Summary: Package for converting METAR TAC messages or an individual METAR message to BUFR4
 Author-email: Alexander Thompson <alexander.thompson@noaa.gov>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: WMO,METAR,FM-15,BUFR,decoding,weather,observations
 Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.7
```

### Comparing `metar2bufr-0.0.2.24/pyproject.toml` & `metar2bufr-0.0.2.25/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "metar2bufr"
-version = "0.0.2.24"
+version = "0.0.2.25"
 authors = [
   { name="Alexander Thompson", email="alexander.thompson@noaa.gov" },
 ]
 description = "Package for converting METAR TAC messages or an individual METAR message to BUFR4"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `metar2bufr-0.0.2.24/src/metar2bufr/csv2bufr/build/lib/csv2bufr/__init__.py` & `metar2bufr-0.0.2.25/src/metar2bufr/csv2bufr/build/lib/csv2bufr/__init__.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.24/src/metar2bufr/csv2bufr/build/lib/csv2bufr/cli.py` & `metar2bufr-0.0.2.25/src/metar2bufr/csv2bufr/build/lib/csv2bufr/cli.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.24/src/metar2bufr/csv2bufr/build/lib/csv2bufr/pygeoapi_plugin.py` & `metar2bufr-0.0.2.25/src/metar2bufr/csv2bufr/build/lib/csv2bufr/pygeoapi_plugin.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.24/src/metar2bufr/csv2bufr/csv2bufr/__init__.py` & `metar2bufr-0.0.2.25/src/metar2bufr/csv2bufr/csv2bufr/__init__.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.24/src/metar2bufr/csv2bufr/csv2bufr/cli.py` & `metar2bufr-0.0.2.25/src/metar2bufr/csv2bufr/csv2bufr/cli.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.24/src/metar2bufr/csv2bufr/csv2bufr/pygeoapi_plugin.py` & `metar2bufr-0.0.2.25/src/metar2bufr/csv2bufr/csv2bufr/pygeoapi_plugin.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.24/src/metar2bufr/csv2bufr/docs/source/conf.py` & `metar2bufr-0.0.2.25/src/metar2bufr/csv2bufr/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.24/src/metar2bufr/csv2bufr/setup.py` & `metar2bufr-0.0.2.25/src/metar2bufr/csv2bufr/setup.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.24/src/metar2bufr/csv2bufr/tests/test_csv2bufr.py` & `metar2bufr-0.0.2.25/src/metar2bufr/csv2bufr/tests/test_csv2bufr.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.24/src/metar2bufr/icao_bufr_encoder.py` & `metar2bufr-0.0.2.25/src/metar2bufr/icao_bufr_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,17 @@
 # metar = "METAR KAFF 121755Z AUTO 21016G24KT 180V240 1SM R11/6000FT R12/P6000 R01L/0600VP6000FT -RA VA PO BKN015 OVC025TCU 06/04 A2990="
 # metar = "METAR KABC 121755Z AUTO 21016G24KT 180V240 1000 2000 R11/P6000FT -RA BR BKN015 OVC025 06/04 A2990="
 # metar = "SPECI DNPO 180700Z 00000KT 5000 BR BKN008 24/24 Q1015 BECMG 7000="
 # metar = "METAR FNHU 171700Z AUTO 13004KT 9999 // NCD 20/03 Q1024="
 # metar = "METAR SABE 012200Z NIL="
 
 # metar = "SPECI DNPO 180700Z 21016G24MPS 3000 0500NW 1000E BR BKN008 24/24 Q1015 BECMG 7000="
-metar = "METAR K2C8 181955Z AUTO 13005KT 5SM HZ FEW038 SCT060 BKN120 21/16 A2992 RMK AO2="
-#K2C8
+# metar = "METAR K2C8 181955Z AUTO 13005KT 5SM HZ FEW038 SCT060 BKN120 21/16 A2992 RMK AO2="
+metar = "METAR K17J 250035Z AUTO 24003KT 10SM CLR 26/20 A3009 RMK AO2 T02580203="
+
 # metar = "SAUS11 KAWN 182000 RRA\
 # METAR K2C8 181955Z AUTO 13005KT 5SM HZ FEW038 SCT060 BKN120 21/16 A2992\
 #       RMK AO2=\
 # METAR K6L4 181955Z AUTO 21004KT 10SM SCT041 SCT049 SCT120 28/21 A3005\
 #       RMK AO2=\
 # METAR KANE 181946Z 21007KT 10SM SCT060 28/10 A2996=\
 # METAR KATW 181945Z 28005KT 10SM BKN050 27/12 A2998=\
@@ -139,16 +140,16 @@
 def parse_metar(message: str, year: int, month: int) -> dict:
     icaoID = re_ID.match(message).group('id')
     if deu.isUSIdentifier(icaoID):
         decoded = fmh(message)
     else:
         decoded = annex3(message)
 
-    # for key in decoded:
-    #     print(key, ': ', decoded[key])
+    for key in decoded:
+        print(key, ': ', decoded[key])
 
     output = deepcopy(metar_template)
 
     output['report_type'] = message[0:5]
     output['year'] = year
     output['month'] = month
 
@@ -157,21 +158,21 @@
         output['icao_location_identifier'] = icao
 
         #   find ICAO identifier in aviation list and pull out lat, long, and elevation
         response = request.urlopen(ICAOSTATIONSURL)
         html = response.read().decode('utf-8').split('\n')
         for line in html:
             if f' {icao} ' in line:
-                # print(line)
+                print(line)
                 # lat = re.search('\d{1,2} [0-9]{1,2}[N,S]', line).group()
                 # long = re.search('\d{1,2} [0-9]{1,2}[N,S]  \d{1,3} \d{1,2}[E,W]\s{1,4}\d{1,4}', line).group()
                 # info = re.search('\d{1,2} \d{1,2}[N,S] \d{1,3} \d{2}[E,W]\s{1,4}\d{1,4}').group()
 
                 info = re.search('\d{1,2} [0-9]{1,2}[N,S]  \d{1,3} \d{1,2}[E,W]\s{1,4}\d{1,4}', line).group().split()
-                # print(info)
+                print(info)
                 lat = int(info[0]) + int(info[1][:-1])/60   # degrees
                 long = int(info[2]) + int(info[3][:-1])/60  # degrees
                 elevation = info[4]                         # meters
                 output['_latitude'] = lat
                 output['_longitude'] = long
                 output['_station_height'] = elevation
                 break
@@ -297,14 +298,18 @@
                 # METAR reports vertical visibility in 100s of ft. Need to convert to meters for bufr
                 vertical_visibility_ft = float(decoded['sky']['str'][0][3:]) * 100
                 output['vertical_visibility'] = math.floor(vertical_visibility_ft*0.3048)
                 # output['vertical_visibility'] = decoded['sky']['str'][0][3:]
                 break
             #need to convert the recorded cloud amount to bufr using ecCode cloudAmount - table 020011
             cloud_amount = decoded['sky']['str'][i][:3]
+            if cloud_amount == 'SKC' or cloud_amount == 'CLR':
+                # table 020011 codes no cloud cover as 0. break out of the loops since this will be the only group with no other info
+                output[f'cloud_amount_{i+1}'] = 0
+                break
             if cloud_amount == 'FEW':
                 # table 020011 codes FEW clouds as 13
                 output[f'cloud_amount_{i+1}'] = 13
             elif cloud_amount == 'SCT':
                 # codes SCATTERED clouds as 11
                 output[f'cloud_amount_{i+1}'] = 11
             elif cloud_amount == 'BKN':
@@ -333,19 +338,19 @@
     #             output['sig_convec_'+str(i+1)] = decoded['sky']['str'][i][6:]
 
     #         #  TODO need to incorporate NSC and NCD values as described in section 15.9.1.3 of FM-15 manual
 
     if 'temps' in decoded:
         if 'air' in decoded['temps']:
             # metar records temperatures in Celsius. Need to convert to Kelvin for bufr
-            air_temp = int(decoded['temps']['air'])
+            air_temp = float(decoded['temps']['air'])
             output['air_temp'] = air_temp + 273.15
         if 'dewpoint' in decoded['temps']:
             # metar records temperatures in Celsius. Need to convert to Kelvin for bufr
-            dewpoint_temp = int(decoded['temps']['dewpoint'])
+            dewpoint_temp = float(decoded['temps']['dewpoint'])
             output['dew_point_temp'] = dewpoint_temp + 273.15
 
     if 'altimeter' in decoded:
         altimeter = float(decoded['altimeter']['value'])
         alt_uom = decoded['altimeter']['uom']
         if alt_uom == 'hPa':
             output['altimeter'] = altimeter*100
```

### Comparing `metar2bufr-0.0.2.24/src/metar2bufr/metarDecoder/metarDecoders.py` & `metar2bufr-0.0.2.25/src/metar2bufr/metarDecoder/metarDecoders.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.24/src/metar2bufr/metarDecoder/tpg.py` & `metar2bufr-0.0.2.25/src/metar2bufr/metarDecoder/tpg.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.24/src/metar2bufr/metarDecoder/xmlConfig.py` & `metar2bufr-0.0.2.25/src/metar2bufr/metarDecoder/xmlConfig.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.24/src/metar2bufr/metarDecoder/xmlUtilities.py` & `metar2bufr-0.0.2.25/src/metar2bufr/metarDecoder/xmlUtilities.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.24/src/metar2bufr/metar_bufr_encoder.py` & `metar2bufr-0.0.2.25/src/metar2bufr/metar_bufr_encoder.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.24/src/metar2bufr/resources/icao-metar-mappings.json` & `metar2bufr-0.0.2.25/src/metar2bufr/resources/icao-metar-mappings.json`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.24/src/metar2bufr/resources/metar-mappings.json` & `metar2bufr-0.0.2.25/src/metar2bufr/resources/metar-mappings.json`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.24/src/metar2bufr/resources/metar-mappings2.json` & `metar2bufr-0.0.2.25/src/metar2bufr/resources/metar-mappings2.json`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.24/src/metar2bufr.egg-info/PKG-INFO` & `metar2bufr-0.0.2.25/src/metar2bufr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metar2bufr
-Version: 0.0.2.24
+Version: 0.0.2.25
 Summary: Package for converting METAR TAC messages or an individual METAR message to BUFR4
 Author-email: Alexander Thompson <alexander.thompson@noaa.gov>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: WMO,METAR,FM-15,BUFR,decoding,weather,observations
 Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.7
```

### Comparing `metar2bufr-0.0.2.24/src/metar2bufr.egg-info/SOURCES.txt` & `metar2bufr-0.0.2.25/src/metar2bufr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

