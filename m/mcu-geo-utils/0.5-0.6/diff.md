# Comparing `tmp/mcu-geo-utils-0.5.tar.gz` & `tmp/mcu-geo-utils-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcu-geo-utils-0.5.tar", last modified: Fri Jul 21 19:31:45 2023, max compression
+gzip compressed data, was "mcu-geo-utils-0.6.tar", last modified: Tue Jul 25 13:25:51 2023, max compression
```

## Comparing `mcu-geo-utils-0.5.tar` & `mcu-geo-utils-0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 martincontreras   (501) staff       (20)        0 2023-07-21 19:31:45.906801 mcu-geo-utils-0.5/
--rw-r--r--   0 martincontreras   (501) staff       (20)     1075 2023-07-20 16:07:16.000000 mcu-geo-utils-0.5/LICENSE
--rw-r--r--   0 martincontreras   (501) staff       (20)       32 2023-07-19 20:10:43.000000 mcu-geo-utils-0.5/MANIFEST.in
--rw-r--r--   0 martincontreras   (501) staff       (20)      427 2023-07-21 19:31:45.906673 mcu-geo-utils-0.5/PKG-INFO
--rw-r--r--   0 martincontreras   (501) staff       (20)      144 2023-07-20 20:03:40.000000 mcu-geo-utils-0.5/README.md
-drwxr-xr-x   0 martincontreras   (501) staff       (20)        0 2023-07-21 19:31:45.905922 mcu-geo-utils-0.5/mcu_geo_utils/
--rw-r--r--   0 martincontreras   (501) staff       (20)     2045 2023-07-20 19:24:45.000000 mcu-geo-utils-0.5/mcu_geo_utils/OSM.py
--rw-r--r--   0 martincontreras   (501) staff       (20)      191 2023-07-19 19:51:00.000000 mcu-geo-utils-0.5/mcu_geo_utils/__init__.py
--rw-r--r--   0 martincontreras   (501) staff       (20)     3637 2023-07-21 19:25:05.000000 mcu-geo-utils-0.5/mcu_geo_utils/census.py
-drwxr-xr-x   0 martincontreras   (501) staff       (20)        0 2023-07-21 19:31:45.906516 mcu-geo-utils-0.5/mcu_geo_utils.egg-info/
--rw-r--r--   0 martincontreras   (501) staff       (20)      427 2023-07-21 19:31:45.000000 mcu-geo-utils-0.5/mcu_geo_utils.egg-info/PKG-INFO
--rw-r--r--   0 martincontreras   (501) staff       (20)      293 2023-07-21 19:31:45.000000 mcu-geo-utils-0.5/mcu_geo_utils.egg-info/SOURCES.txt
--rw-r--r--   0 martincontreras   (501) staff       (20)        1 2023-07-21 19:31:45.000000 mcu-geo-utils-0.5/mcu_geo_utils.egg-info/dependency_links.txt
--rw-r--r--   0 martincontreras   (501) staff       (20)       58 2023-07-21 19:31:45.000000 mcu-geo-utils-0.5/mcu_geo_utils.egg-info/requires.txt
--rw-r--r--   0 martincontreras   (501) staff       (20)       14 2023-07-21 19:31:45.000000 mcu-geo-utils-0.5/mcu_geo_utils.egg-info/top_level.txt
--rw-r--r--   0 martincontreras   (501) staff       (20)       38 2023-07-21 19:31:45.906844 mcu-geo-utils-0.5/setup.cfg
--rw-r--r--   0 martincontreras   (501) staff       (20)      562 2023-07-21 19:31:31.000000 mcu-geo-utils-0.5/setup.py
+drwxr-xr-x   0 martincontreras   (501) staff       (20)        0 2023-07-25 13:25:51.097618 mcu-geo-utils-0.6/
+-rw-r--r--   0 martincontreras   (501) staff       (20)     1075 2023-07-20 16:07:16.000000 mcu-geo-utils-0.6/LICENSE
+-rw-r--r--   0 martincontreras   (501) staff       (20)       32 2023-07-19 20:10:43.000000 mcu-geo-utils-0.6/MANIFEST.in
+-rw-r--r--   0 martincontreras   (501) staff       (20)      427 2023-07-25 13:25:51.097424 mcu-geo-utils-0.6/PKG-INFO
+-rw-r--r--   0 martincontreras   (501) staff       (20)      144 2023-07-20 20:03:40.000000 mcu-geo-utils-0.6/README.md
+drwxr-xr-x   0 martincontreras   (501) staff       (20)        0 2023-07-25 13:25:51.096300 mcu-geo-utils-0.6/mcu_geo_utils/
+-rw-r--r--   0 martincontreras   (501) staff       (20)     2045 2023-07-20 19:24:45.000000 mcu-geo-utils-0.6/mcu_geo_utils/OSM.py
+-rw-r--r--   0 martincontreras   (501) staff       (20)      191 2023-07-19 19:51:00.000000 mcu-geo-utils-0.6/mcu_geo_utils/__init__.py
+-rw-r--r--   0 martincontreras   (501) staff       (20)     3785 2023-07-25 13:21:45.000000 mcu-geo-utils-0.6/mcu_geo_utils/census.py
+drwxr-xr-x   0 martincontreras   (501) staff       (20)        0 2023-07-25 13:25:51.097171 mcu-geo-utils-0.6/mcu_geo_utils.egg-info/
+-rw-r--r--   0 martincontreras   (501) staff       (20)      427 2023-07-25 13:25:51.000000 mcu-geo-utils-0.6/mcu_geo_utils.egg-info/PKG-INFO
+-rw-r--r--   0 martincontreras   (501) staff       (20)      293 2023-07-25 13:25:51.000000 mcu-geo-utils-0.6/mcu_geo_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 martincontreras   (501) staff       (20)        1 2023-07-25 13:25:51.000000 mcu-geo-utils-0.6/mcu_geo_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 martincontreras   (501) staff       (20)       58 2023-07-25 13:25:51.000000 mcu-geo-utils-0.6/mcu_geo_utils.egg-info/requires.txt
+-rw-r--r--   0 martincontreras   (501) staff       (20)       14 2023-07-25 13:25:51.000000 mcu-geo-utils-0.6/mcu_geo_utils.egg-info/top_level.txt
+-rw-r--r--   0 martincontreras   (501) staff       (20)       38 2023-07-25 13:25:51.097728 mcu-geo-utils-0.6/setup.cfg
+-rw-r--r--   0 martincontreras   (501) staff       (20)      562 2023-07-25 13:23:06.000000 mcu-geo-utils-0.6/setup.py
```

### Comparing `mcu-geo-utils-0.5/LICENSE` & `mcu-geo-utils-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mcu-geo-utils-0.5/mcu_geo_utils/OSM.py` & `mcu-geo-utils-0.6/mcu_geo_utils/OSM.py`

 * *Files identical despite different names*

### Comparing `mcu-geo-utils-0.5/mcu_geo_utils/census.py` & `mcu-geo-utils-0.6/mcu_geo_utils/census.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 import pandas as pd
 import geopandas as gpd
 from shapely.geometry import Point
 import wget
 import os
+import warnings
+
+def fxn():
+    warnings.warn("user", UserWarning)
+
+with warnings.catch_warnings():
+    warnings.simplefilter("ignore")
+    fxn()
 
 # TODO:
 # 1: CHECK IF 18S OR 19S SHOULD APPLY
 
 
 def get_census_dataset() -> gpd.GeoDataFrame:
     os.makedirs("data", exist_ok=True)
@@ -33,15 +41,15 @@
                                lon: float,
                                census_df: gpd.GeoDataFrame,
                                radio: int = 1000) -> pd.DataFrame:
     # defining the geoseries point from 'lat' and 'lon'
     point = (
         gpd.GeoSeries(Point(lon, lat), crs=4326)
         .to_crs(9155)  # TODO 1
-        .buffer(1000)
+        .buffer(radio)
         .to_crs(4326)
     )
 
     # Creating the filtered dataframe
     def weighted_sum_censo(df):
         coverture = df.pop("coverture")
         return df.mul(coverture, axis=0).sum()
@@ -68,15 +76,15 @@
                              ismt_df: gpd.GeoDataFrame,
                              radio: int = 1000) -> pd.DataFrame:
 
     # defining the geoseries point from 'lat' and 'lon'
     point = (
         gpd.GeoSeries(Point(lon, lat), crs=4326)
         .to_crs(9155)  # TODO 1
-        .buffer(1000)
+        .buffer(radio)
         .to_crs(4326)
     )
     # Creating the filtered dataframe
     ismt_intersection = ismt_df.intersects(point.geometry.iloc[0])
     columns = [
         'Alto',
         'Medio',
```

### Comparing `mcu-geo-utils-0.5/setup.py` & `mcu-geo-utils-0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='mcu-geo-utils',
-    version='0.5',
+    version='0.6',
     author='Martin Conur',
     author_email='martincontrerasur@gmail.com',
     packages=['mcu_geo_utils'],
     scripts=[],
     url='https://pypi.org/project/mcu-geo-utils/',
     license='MIT',
     description='variaty of geo-related tools',
```

