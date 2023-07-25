# Comparing `tmp/landfall-0.3.1.tar.gz` & `tmp/landfall-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landfall-0.3.1.tar", last modified: Tue Jul 25 15:16:17 2023, max compression
+gzip compressed data, was "landfall-0.3.2.tar", last modified: Tue Jul 25 16:57:28 2023, max compression
```

## Comparing `landfall-0.3.1.tar` & `landfall-0.3.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-25 15:16:17.368546 landfall-0.3.1/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1068 2023-02-28 17:06:52.000000 landfall-0.3.1/LICENSE
--rw-r--r--   0 odosmatthews   (501) staff       (20)      570 2023-07-25 15:16:17.368728 landfall-0.3.1/PKG-INFO
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1348 2023-07-21 17:24:03.000000 landfall-0.3.1/README.md
--rw-r--r--   0 odosmatthews   (501) staff       (20)      499 2023-02-28 17:09:25.000000 landfall-0.3.1/pyproject.toml
--rw-r--r--   0 odosmatthews   (501) staff       (20)      871 2023-07-25 15:16:17.370042 landfall-0.3.1/setup.cfg
--rw-r--r--   0 odosmatthews   (501) staff       (20)       68 2023-02-28 17:08:57.000000 landfall-0.3.1/setup.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-25 15:16:17.354887 landfall-0.3.1/src/
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-25 15:16:17.362907 landfall-0.3.1/src/landfall/
--rw-r--r--   0 odosmatthews   (501) staff       (20)      216 2023-07-25 15:15:36.000000 landfall-0.3.1/src/landfall/__init__.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1848 2023-03-06 19:27:35.000000 landfall-0.3.1/src/landfall/color.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)      631 2023-03-06 17:06:44.000000 landfall-0.3.1/src/landfall/colorsys.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)      865 2023-07-24 18:54:39.000000 landfall-0.3.1/src/landfall/combos.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)      484 2023-07-25 14:24:09.000000 landfall-0.3.1/src/landfall/context.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)      271 2023-03-06 17:06:44.000000 landfall-0.3.1/src/landfall/distinctipy.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)     3526 2023-07-25 15:14:16.000000 landfall-0.3.1/src/landfall/points.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)     2213 2023-07-24 18:49:22.000000 landfall-0.3.1/src/landfall/polygons.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-25 15:16:17.368242 landfall-0.3.1/src/landfall.egg-info/
--rw-r--r--   0 odosmatthews   (501) staff       (20)      570 2023-07-25 15:16:17.000000 landfall-0.3.1/src/landfall.egg-info/PKG-INFO
--rw-r--r--   0 odosmatthews   (501) staff       (20)      460 2023-07-25 15:16:17.000000 landfall-0.3.1/src/landfall.egg-info/SOURCES.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-07-25 15:16:17.000000 landfall-0.3.1/src/landfall.egg-info/dependency_links.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-02-28 18:06:53.000000 landfall-0.3.1/src/landfall.egg-info/not-zip-safe
--rw-r--r--   0 odosmatthews   (501) staff       (20)      156 2023-07-25 15:16:17.000000 landfall-0.3.1/src/landfall.egg-info/requires.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        9 2023-07-25 15:16:17.000000 landfall-0.3.1/src/landfall.egg-info/top_level.txt
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-25 16:57:28.968345 landfall-0.3.2/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1068 2023-02-28 17:06:52.000000 landfall-0.3.2/LICENSE
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1822 2023-07-25 16:57:28.968497 landfall-0.3.2/PKG-INFO
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1195 2023-07-25 16:31:00.000000 landfall-0.3.2/README.md
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      499 2023-02-28 17:09:25.000000 landfall-0.3.2/pyproject.toml
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      926 2023-07-25 16:57:28.969753 landfall-0.3.2/setup.cfg
+-rw-r--r--   0 odosmatthews   (501) staff       (20)       68 2023-07-25 16:48:54.000000 landfall-0.3.2/setup.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-25 16:57:28.955928 landfall-0.3.2/src/
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-25 16:57:28.964081 landfall-0.3.2/src/landfall/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      216 2023-07-25 16:49:22.000000 landfall-0.3.2/src/landfall/__init__.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1848 2023-03-06 19:27:35.000000 landfall-0.3.2/src/landfall/color.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      631 2023-03-06 17:06:44.000000 landfall-0.3.2/src/landfall/colorsys.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      865 2023-07-24 18:54:39.000000 landfall-0.3.2/src/landfall/combos.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      484 2023-07-25 14:24:09.000000 landfall-0.3.2/src/landfall/context.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      271 2023-03-06 17:06:44.000000 landfall-0.3.2/src/landfall/distinctipy.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     3526 2023-07-25 15:14:16.000000 landfall-0.3.2/src/landfall/points.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     2213 2023-07-24 18:49:22.000000 landfall-0.3.2/src/landfall/polygons.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-25 16:57:28.968023 landfall-0.3.2/src/landfall.egg-info/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1822 2023-07-25 16:57:28.000000 landfall-0.3.2/src/landfall.egg-info/PKG-INFO
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      460 2023-07-25 16:57:28.000000 landfall-0.3.2/src/landfall.egg-info/SOURCES.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-07-25 16:57:28.000000 landfall-0.3.2/src/landfall.egg-info/dependency_links.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-02-28 18:06:53.000000 landfall-0.3.2/src/landfall.egg-info/not-zip-safe
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      118 2023-07-25 16:57:28.000000 landfall-0.3.2/src/landfall.egg-info/requires.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        9 2023-07-25 16:57:28.000000 landfall-0.3.2/src/landfall.egg-info/top_level.txt
```

### Comparing `landfall-0.3.1/LICENSE` & `landfall-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `landfall-0.3.1/README.md` & `landfall-0.3.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 ```sh
 # PyPI
 pip install landfall
 ```
 
 ## Dependencies
 - [py-staticmaps - A python module to create static map images (PNG, SVG) with markers, geodesic lines, etc.](https://github.com/flopp/py-staticmaps)
-- [PyGeodesy - A pure python implementation of geodesy tools used here for geographic calculations like geohashes](https://github.com/mrJean1/PyGeodesy)
 - [distinctipy - A lightweight package for generating visually distinct colours.](https://github.com/alan-turing-institute/distinctipy)
 
 
 ## Example
 ```sh
 import landfall
```

### Comparing `landfall-0.3.1/setup.cfg` & `landfall-0.3.2/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 [metadata]
 name = landfall
-version = 0.3.1
+version = 0.3.2
 description = Easy to use functions to plot geospatial data on maps using staticmaps.
+long_description = file: README.md
+long_description_content_type = text/markdown; charset=UTF-8
 author = Odos Matthews
 license = MIT
 license_file = LICENSE
 platforms = unix, linux, osx, cygwin, win32
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
@@ -14,17 +16,14 @@
 	Programming Language :: Python :: 3.10
 
 [options]
 packages = 
 	landfall
 install_requires = 
 	py-staticmaps
-	more-itertools
-	tinytim
-	range_key_dict
 	distinctipy
 	Pillow<=9.5.0
 python_requires = >=3.8
 package_dir = 
 	=src
 zip_safe = no
```

### Comparing `landfall-0.3.1/src/landfall/color.py` & `landfall-0.3.2/src/landfall/color.py`

 * *Files identical despite different names*

### Comparing `landfall-0.3.1/src/landfall/colorsys.py` & `landfall-0.3.2/src/landfall/colorsys.py`

 * *Files identical despite different names*

### Comparing `landfall-0.3.1/src/landfall/combos.py` & `landfall-0.3.2/src/landfall/combos.py`

 * *Files identical despite different names*

### Comparing `landfall-0.3.1/src/landfall/points.py` & `landfall-0.3.2/src/landfall/points.py`

 * *Files identical despite different names*

### Comparing `landfall-0.3.1/src/landfall/polygons.py` & `landfall-0.3.2/src/landfall/polygons.py`

 * *Files identical despite different names*

