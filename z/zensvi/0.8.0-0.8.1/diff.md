# Comparing `tmp/zensvi-0.8.0.tar.gz` & `tmp/zensvi-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zensvi-0.8.0.tar", max compression
+gzip compressed data, was "zensvi-0.8.1.tar", max compression
```

## Comparing `zensvi-0.8.0.tar` & `zensvi-0.8.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.8.0/LICENSE
--rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.8.0/README.md
--rwxr-xr-x   0        0        0     1401 2023-07-25 03:33:27.972186 zensvi-0.8.0/pyproject.toml
--rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.8.0/src/zensvi/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.8.0/src/zensvi/cv/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.8.0/src/zensvi/cv/segmentation/__init__.py
--rwxr-xr-x   0        0        0    45608 2023-07-13 09:34:43.004230 zensvi-0.8.0/src/zensvi/cv/segmentation/segmentation.py
--rwxr-xr-x   0        0        0       63 2023-05-30 03:03:24.804064 zensvi-0.8.0/src/zensvi/download/__init__.py
--rw-r--r--   0        0        0      629 2023-07-11 07:03:47.656454 zensvi-0.8.0/src/zensvi/download/mapillary/__init__.py
--rw-r--r--   0        0        0        0 2023-07-11 07:03:47.656489 zensvi-0.8.0/src/zensvi/download/mapillary/config/.gitkeep
--rw-r--r--   0        0        0     1110 2023-07-11 07:03:47.656962 zensvi-0.8.0/src/zensvi/download/mapillary/config/__init__.py
--rw-r--r--   0        0        0      398 2023-07-11 07:03:47.657311 zensvi-0.8.0/src/zensvi/download/mapillary/config/api/__init__.py
--rw-r--r--   0        0        0    25264 2023-07-11 07:03:47.657833 zensvi-0.8.0/src/zensvi/download/mapillary/config/api/entities.py
--rw-r--r--   0        0        0     1917 2023-07-11 07:03:47.658201 zensvi-0.8.0/src/zensvi/download/mapillary/config/api/general.py
--rw-r--r--   0        0        0     8163 2023-07-11 07:03:47.658519 zensvi-0.8.0/src/zensvi/download/mapillary/config/api/vector_tiles.py
--rw-r--r--   0        0        0      481 2023-07-11 07:03:47.658811 zensvi-0.8.0/src/zensvi/download/mapillary/controller/__init__.py
--rw-r--r--   0        0        0     2297 2023-07-11 08:21:16.088478 zensvi-0.8.0/src/zensvi/download/mapillary/controller/detection.py
--rw-r--r--   0        0        0     4775 2023-07-11 08:21:17.279629 zensvi-0.8.0/src/zensvi/download/mapillary/controller/feature.py
--rw-r--r--   0        0        0    31634 2023-07-11 08:20:22.811895 zensvi-0.8.0/src/zensvi/download/mapillary/controller/image.py
--rw-r--r--   0        0        0     4904 2023-07-11 08:20:39.797301 zensvi-0.8.0/src/zensvi/download/mapillary/controller/save.py
--rw-r--r--   0        0        0    34865 2023-07-11 07:03:47.660533 zensvi-0.8.0/src/zensvi/download/mapillary/interface.py
--rw-r--r--   0        0        0        0 2023-07-11 07:03:47.660579 zensvi-0.8.0/src/zensvi/download/mapillary/models/.gitkeep
--rw-r--r--   0        0        0      520 2023-07-11 07:03:47.660843 zensvi-0.8.0/src/zensvi/download/mapillary/models/__init__.py
--rw-r--r--   0        0        0      396 2023-07-11 07:03:47.660998 zensvi-0.8.0/src/zensvi/download/mapillary/models/api/__init__.py
--rw-r--r--   0        0        0     8168 2023-07-11 08:21:35.171162 zensvi-0.8.0/src/zensvi/download/mapillary/models/api/entities.py
--rw-r--r--   0        0        0    14403 2023-07-11 08:23:11.396978 zensvi-0.8.0/src/zensvi/download/mapillary/models/api/general.py
--rw-r--r--   0        0        0    19294 2023-07-11 08:22:13.318683 zensvi-0.8.0/src/zensvi/download/mapillary/models/api/vector_tiles.py
--rw-r--r--   0        0        0     8273 2023-07-11 08:26:45.376434 zensvi-0.8.0/src/zensvi/download/mapillary/models/client.py
--rw-r--r--   0        0        0     1398 2023-07-11 07:03:47.662813 zensvi-0.8.0/src/zensvi/download/mapillary/models/config.py
--rw-r--r--   0        0        0    10328 2023-07-11 07:03:47.663102 zensvi-0.8.0/src/zensvi/download/mapillary/models/exceptions.py
--rw-r--r--   0        0        0    14602 2023-07-11 08:21:05.329571 zensvi-0.8.0/src/zensvi/download/mapillary/models/geojson.py
--rw-r--r--   0        0        0     2496 2023-07-11 07:03:47.663608 zensvi-0.8.0/src/zensvi/download/mapillary/models/logger.py
--rw-r--r--   0        0        0        0 2023-07-11 07:03:47.663642 zensvi-0.8.0/src/zensvi/download/mapillary/utils/.gitkeep
--rw-r--r--   0        0        0      511 2023-07-11 07:03:47.663779 zensvi-0.8.0/src/zensvi/download/mapillary/utils/__init__.py
--rw-r--r--   0        0        0     1774 2023-07-11 08:22:50.091875 zensvi-0.8.0/src/zensvi/download/mapillary/utils/auth.py
--rw-r--r--   0        0        0     1750 2023-07-11 07:03:47.664341 zensvi-0.8.0/src/zensvi/download/mapillary/utils/extract.py
--rw-r--r--   0        0        0    16350 2023-07-14 08:34:10.134073 zensvi-0.8.0/src/zensvi/download/mapillary/utils/filter.py
--rw-r--r--   0        0        0    26693 2023-07-11 08:26:13.918807 zensvi-0.8.0/src/zensvi/download/mapillary/utils/format.py
--rw-r--r--   0        0        0     1723 2023-07-11 07:03:47.665237 zensvi-0.8.0/src/zensvi/download/mapillary/utils/time.py
--rw-r--r--   0        0        0     9976 2023-07-11 08:22:46.586975 zensvi-0.8.0/src/zensvi/download/mapillary/utils/verify.py
--rwxr-xr-x   0        0        0    46819 2023-07-14 08:34:10.134403 zensvi-0.8.0/src/zensvi/download/streetview_downloader.py
--rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.8.0/src/zensvi/download/utils/UserAgent.csv
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.8.0/src/zensvi/download/utils/__init__.py
--rwxr-xr-x   0        0        0     8651 2023-06-05 08:53:58.000000 zensvi-0.8.0/src/zensvi/download/utils/geoprocess.py
--rwxr-xr-x   0        0        0     1810 2023-06-05 08:53:58.000000 zensvi-0.8.0/src/zensvi/download/utils/get_pids.py
--rwxr-xr-x   0        0        0      956 2023-05-14 09:11:59.596085 zensvi-0.8.0/src/zensvi/download/utils/helpers.py
--rwxr-xr-x   0        0        0     7273 2023-07-14 08:34:10.134616 zensvi-0.8.0/src/zensvi/download/utils/imtool.py
--rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.8.0/src/zensvi/download/utils/proxies.csv
--rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.8.0/src/zensvi/transform/__init__.py
--rwxr-xr-x   0        0        0    10503 2023-07-25 03:33:12.884662 zensvi-0.8.0/src/zensvi/transform/transform_image.py
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.8.0/src/zensvi/zensvi.py
--rw-r--r--   0        0        0     3158 1970-01-01 00:00:00.000000 zensvi-0.8.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.8.1/LICENSE
+-rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.8.1/README.md
+-rwxr-xr-x   0        0        0     1401 2023-07-25 04:01:27.582422 zensvi-0.8.1/pyproject.toml
+-rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.8.1/src/zensvi/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.8.1/src/zensvi/cv/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.8.1/src/zensvi/cv/segmentation/__init__.py
+-rwxr-xr-x   0        0        0    45608 2023-07-13 09:34:43.004230 zensvi-0.8.1/src/zensvi/cv/segmentation/segmentation.py
+-rwxr-xr-x   0        0        0       63 2023-05-30 03:03:24.804064 zensvi-0.8.1/src/zensvi/download/__init__.py
+-rw-r--r--   0        0        0      629 2023-07-11 07:03:47.656454 zensvi-0.8.1/src/zensvi/download/mapillary/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 07:03:47.656489 zensvi-0.8.1/src/zensvi/download/mapillary/config/.gitkeep
+-rw-r--r--   0        0        0     1110 2023-07-11 07:03:47.656962 zensvi-0.8.1/src/zensvi/download/mapillary/config/__init__.py
+-rw-r--r--   0        0        0      398 2023-07-11 07:03:47.657311 zensvi-0.8.1/src/zensvi/download/mapillary/config/api/__init__.py
+-rw-r--r--   0        0        0    25264 2023-07-11 07:03:47.657833 zensvi-0.8.1/src/zensvi/download/mapillary/config/api/entities.py
+-rw-r--r--   0        0        0     1917 2023-07-11 07:03:47.658201 zensvi-0.8.1/src/zensvi/download/mapillary/config/api/general.py
+-rw-r--r--   0        0        0     8163 2023-07-11 07:03:47.658519 zensvi-0.8.1/src/zensvi/download/mapillary/config/api/vector_tiles.py
+-rw-r--r--   0        0        0      481 2023-07-11 07:03:47.658811 zensvi-0.8.1/src/zensvi/download/mapillary/controller/__init__.py
+-rw-r--r--   0        0        0     2297 2023-07-11 08:21:16.088478 zensvi-0.8.1/src/zensvi/download/mapillary/controller/detection.py
+-rw-r--r--   0        0        0     4775 2023-07-11 08:21:17.279629 zensvi-0.8.1/src/zensvi/download/mapillary/controller/feature.py
+-rw-r--r--   0        0        0    31634 2023-07-11 08:20:22.811895 zensvi-0.8.1/src/zensvi/download/mapillary/controller/image.py
+-rw-r--r--   0        0        0     4904 2023-07-11 08:20:39.797301 zensvi-0.8.1/src/zensvi/download/mapillary/controller/save.py
+-rw-r--r--   0        0        0    34865 2023-07-11 07:03:47.660533 zensvi-0.8.1/src/zensvi/download/mapillary/interface.py
+-rw-r--r--   0        0        0        0 2023-07-11 07:03:47.660579 zensvi-0.8.1/src/zensvi/download/mapillary/models/.gitkeep
+-rw-r--r--   0        0        0      520 2023-07-11 07:03:47.660843 zensvi-0.8.1/src/zensvi/download/mapillary/models/__init__.py
+-rw-r--r--   0        0        0      396 2023-07-11 07:03:47.660998 zensvi-0.8.1/src/zensvi/download/mapillary/models/api/__init__.py
+-rw-r--r--   0        0        0     8168 2023-07-11 08:21:35.171162 zensvi-0.8.1/src/zensvi/download/mapillary/models/api/entities.py
+-rw-r--r--   0        0        0    14403 2023-07-11 08:23:11.396978 zensvi-0.8.1/src/zensvi/download/mapillary/models/api/general.py
+-rw-r--r--   0        0        0    19294 2023-07-11 08:22:13.318683 zensvi-0.8.1/src/zensvi/download/mapillary/models/api/vector_tiles.py
+-rw-r--r--   0        0        0     8273 2023-07-11 08:26:45.376434 zensvi-0.8.1/src/zensvi/download/mapillary/models/client.py
+-rw-r--r--   0        0        0     1398 2023-07-11 07:03:47.662813 zensvi-0.8.1/src/zensvi/download/mapillary/models/config.py
+-rw-r--r--   0        0        0    10328 2023-07-11 07:03:47.663102 zensvi-0.8.1/src/zensvi/download/mapillary/models/exceptions.py
+-rw-r--r--   0        0        0    14602 2023-07-11 08:21:05.329571 zensvi-0.8.1/src/zensvi/download/mapillary/models/geojson.py
+-rw-r--r--   0        0        0     2496 2023-07-11 07:03:47.663608 zensvi-0.8.1/src/zensvi/download/mapillary/models/logger.py
+-rw-r--r--   0        0        0        0 2023-07-11 07:03:47.663642 zensvi-0.8.1/src/zensvi/download/mapillary/utils/.gitkeep
+-rw-r--r--   0        0        0      511 2023-07-11 07:03:47.663779 zensvi-0.8.1/src/zensvi/download/mapillary/utils/__init__.py
+-rw-r--r--   0        0        0     1774 2023-07-11 08:22:50.091875 zensvi-0.8.1/src/zensvi/download/mapillary/utils/auth.py
+-rw-r--r--   0        0        0     1750 2023-07-11 07:03:47.664341 zensvi-0.8.1/src/zensvi/download/mapillary/utils/extract.py
+-rw-r--r--   0        0        0    16350 2023-07-14 08:34:10.134073 zensvi-0.8.1/src/zensvi/download/mapillary/utils/filter.py
+-rw-r--r--   0        0        0    26693 2023-07-11 08:26:13.918807 zensvi-0.8.1/src/zensvi/download/mapillary/utils/format.py
+-rw-r--r--   0        0        0     1723 2023-07-11 07:03:47.665237 zensvi-0.8.1/src/zensvi/download/mapillary/utils/time.py
+-rw-r--r--   0        0        0     9976 2023-07-11 08:22:46.586975 zensvi-0.8.1/src/zensvi/download/mapillary/utils/verify.py
+-rwxr-xr-x   0        0        0    46819 2023-07-14 08:34:10.134403 zensvi-0.8.1/src/zensvi/download/streetview_downloader.py
+-rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.8.1/src/zensvi/download/utils/UserAgent.csv
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.8.1/src/zensvi/download/utils/__init__.py
+-rwxr-xr-x   0        0        0     8651 2023-06-05 08:53:58.000000 zensvi-0.8.1/src/zensvi/download/utils/geoprocess.py
+-rwxr-xr-x   0        0        0     1810 2023-06-05 08:53:58.000000 zensvi-0.8.1/src/zensvi/download/utils/get_pids.py
+-rwxr-xr-x   0        0        0      956 2023-05-14 09:11:59.596085 zensvi-0.8.1/src/zensvi/download/utils/helpers.py
+-rwxr-xr-x   0        0        0     7273 2023-07-14 08:34:10.134616 zensvi-0.8.1/src/zensvi/download/utils/imtool.py
+-rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.8.1/src/zensvi/download/utils/proxies.csv
+-rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.8.1/src/zensvi/transform/__init__.py
+-rwxr-xr-x   0        0        0    10587 2023-07-25 03:34:33.869476 zensvi-0.8.1/src/zensvi/transform/transform_image.py
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.8.1/src/zensvi/zensvi.py
+-rw-r--r--   0        0        0     3158 1970-01-01 00:00:00.000000 zensvi-0.8.1/PKG-INFO
```

### Comparing `zensvi-0.8.0/LICENSE` & `zensvi-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/README.md` & `zensvi-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/pyproject.toml` & `zensvi-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zensvi"
-version = "0.8.0"
+version = "0.8.1"
 description = "This package handles downloading, cleaning, analyzing street view imagery in a one-stop and zen manner."
 authors = ["koito19960406"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
```

### Comparing `zensvi-0.8.0/src/zensvi/cv/segmentation/segmentation.py` & `zensvi-0.8.1/src/zensvi/cv/segmentation/segmentation.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/mapillary/__init__.py` & `zensvi-0.8.1/src/zensvi/download/mapillary/__init__.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/mapillary/config/__init__.py` & `zensvi-0.8.1/src/zensvi/download/mapillary/config/__init__.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/mapillary/config/api/entities.py` & `zensvi-0.8.1/src/zensvi/download/mapillary/config/api/entities.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/mapillary/config/api/general.py` & `zensvi-0.8.1/src/zensvi/download/mapillary/config/api/general.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/mapillary/config/api/vector_tiles.py` & `zensvi-0.8.1/src/zensvi/download/mapillary/config/api/vector_tiles.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/mapillary/controller/detection.py` & `zensvi-0.8.1/src/zensvi/download/mapillary/controller/detection.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/mapillary/controller/feature.py` & `zensvi-0.8.1/src/zensvi/download/mapillary/controller/feature.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/mapillary/controller/image.py` & `zensvi-0.8.1/src/zensvi/download/mapillary/controller/image.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/mapillary/controller/save.py` & `zensvi-0.8.1/src/zensvi/download/mapillary/controller/save.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/mapillary/interface.py` & `zensvi-0.8.1/src/zensvi/download/mapillary/interface.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/mapillary/models/__init__.py` & `zensvi-0.8.1/src/zensvi/download/mapillary/models/__init__.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/mapillary/models/api/entities.py` & `zensvi-0.8.1/src/zensvi/download/mapillary/models/api/entities.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/mapillary/models/api/general.py` & `zensvi-0.8.1/src/zensvi/download/mapillary/models/api/general.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/mapillary/models/api/vector_tiles.py` & `zensvi-0.8.1/src/zensvi/download/mapillary/models/api/vector_tiles.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/mapillary/models/client.py` & `zensvi-0.8.1/src/zensvi/download/mapillary/models/client.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/mapillary/models/config.py` & `zensvi-0.8.1/src/zensvi/download/mapillary/models/config.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/mapillary/models/exceptions.py` & `zensvi-0.8.1/src/zensvi/download/mapillary/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/mapillary/models/geojson.py` & `zensvi-0.8.1/src/zensvi/download/mapillary/models/geojson.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/mapillary/models/logger.py` & `zensvi-0.8.1/src/zensvi/download/mapillary/models/logger.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/mapillary/utils/auth.py` & `zensvi-0.8.1/src/zensvi/download/mapillary/utils/auth.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/mapillary/utils/extract.py` & `zensvi-0.8.1/src/zensvi/download/mapillary/utils/extract.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/mapillary/utils/filter.py` & `zensvi-0.8.1/src/zensvi/download/mapillary/utils/filter.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/mapillary/utils/format.py` & `zensvi-0.8.1/src/zensvi/download/mapillary/utils/format.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/mapillary/utils/time.py` & `zensvi-0.8.1/src/zensvi/download/mapillary/utils/time.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/mapillary/utils/verify.py` & `zensvi-0.8.1/src/zensvi/download/mapillary/utils/verify.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/streetview_downloader.py` & `zensvi-0.8.1/src/zensvi/download/streetview_downloader.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/utils/UserAgent.csv` & `zensvi-0.8.1/src/zensvi/download/utils/UserAgent.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/utils/geoprocess.py` & `zensvi-0.8.1/src/zensvi/download/utils/geoprocess.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/utils/get_pids.py` & `zensvi-0.8.1/src/zensvi/download/utils/get_pids.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/utils/helpers.py` & `zensvi-0.8.1/src/zensvi/download/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/utils/imtool.py` & `zensvi-0.8.1/src/zensvi/download/utils/imtool.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/download/utils/proxies.csv` & `zensvi-0.8.1/src/zensvi/download/utils/proxies.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.8.0/src/zensvi/transform/transform_image.py` & `zensvi-0.8.1/src/zensvi/transform/transform_image.py`

 * *Files 4% similar despite different names*

```diff
@@ -221,27 +221,23 @@
 
         # Copy pixels from original image to new image
         new_img[y[mask], x[mask]] = img[yp, xp]
 
         return new_img
 
     def transform_images(self, style_list=["perspective", "equidistant_fisheye", "orthographic_fisheye", "stereographic_fisheye", "equisolid_fisheye"], 
-                        FOV = 90, aspects = (9, 16), show_size=100):
-        # FOV validation
-        if 360 % FOV != 0:
-            raise ValueError("FOV must be a divisor of 360.")
-
+                    FOV = 90, theta = 90, aspects = (9, 16), show_size=100):
         # check if there's anything other than "perspective" and "fisheye"
         if not all(style in ["perspective", "equidistant_fisheye", "orthographic_fisheye", "stereographic_fisheye", "equisolid_fisheye"] for style in style_list):
-            raise ValueError("Please input the correct image style. The correct image style should be 'perspective' or 'fisheye'.")
+            raise ValueError("Please input the correct image style. The correct image style should be 'perspective', 'equidistant_fisheye', 'orthographic_fisheye', 'stereographic_fisheye', or 'equisolid_fisheye'")
 
         # set image file extensions
         image_extensions = ['.jpg', '.jpeg', '.png', '.bmp', '.gif', '.tiff', '.tif', '.webp', '.ico', '.jfif', '.heic', '.heif']
 
-        def run(path_input, path_output, show_size, style):
+        def run(path_input, path_output, show_size, style, theta, aspects, FOV):
             img_raw = cv2.imread(str(path_input), cv2.IMREAD_COLOR)
             if style == "equidistant_fisheye":
                 if not path_output.exists():
                     img_new = self.equidistant_fisheye(img_raw)
                     cv2.imwrite(str(path_output), img_new)
             
             elif style == "orthographic_fisheye":
@@ -256,34 +252,34 @@
             
             elif style == "equisolid_fisheye":
                 if not path_output.exists():
                     img_new = self.equisolid_fisheye(img_raw)
                     cv2.imwrite(str(path_output), img_new)
 
             elif style == "perspective":
-                num_images = 360 // FOV  # Calculate the number of images
-                thetas = [FOV * i for i in range(num_images)]  # Calculate thetas based on FOV
+                num_images = 360 // theta  # Calculate the number of images based on theta
+                thetas = [theta * i for i in range(num_images)]  # Calculate thetas based on step size
                 aspects_v = (aspects[0], aspects[1] / num_images)  # Set aspects_v based on the number of images
 
                 for theta in thetas:
                     height = int(aspects_v[0] * show_size)
                     width = int(aspects_v[1] * show_size)
                     aspect_name = '%s--%s' % (aspects[0], aspects[1])
                     path_output_raw = path_output.with_name(f'{path_output.stem}_Direction_{theta}_FOV_{FOV}_aspect_{aspect_name}_raw.png')
                     if not path_output_raw.exists(): 
                         img_new = self.get_perspective(img_raw, FOV, theta, 0, height, width)
                         cv2.imwrite(str(path_output_raw), img_new)
 
-        def process_image(dir_input, dir_output, name, show_size, style):
+        def process_image(dir_input, dir_output, name, show_size, style, theta, aspects, FOV):
             path_input = dir_input / name.name
             path_output = dir_output / (name.stem + ".png")
-            return path_input, path_output, show_size, style
+            return path_input, path_output, show_size, style, theta, aspects, FOV
 
         for current_style in style_list:
             dir_output = Path(self.dir_output) / current_style
             dir_output.mkdir(parents=True, exist_ok=True)
 
             with ThreadPoolExecutor() as executor:
-                futures = [executor.submit(run, *process_image(self.dir_input, dir_output, name, show_size, current_style)) \
+                futures = [executor.submit(run, *process_image(self.dir_input, dir_output, name, show_size, current_style, theta, aspects, FOV)) \
                     for name in self.dir_input.rglob('*') if name.suffix.lower() in image_extensions]
                 for future in tqdm(as_completed(futures), total=len(futures), desc=f"Converting to {current_style}"):
                     future.result()
```

### Comparing `zensvi-0.8.0/PKG-INFO` & `zensvi-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zensvi
-Version: 0.8.0
+Version: 0.8.1
 Summary: This package handles downloading, cleaning, analyzing street view imagery in a one-stop and zen manner.
 License: MIT
 Author: koito19960406
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

