# Comparing `tmp/tess-atl-0.0.2.tar.gz` & `tmp/tess-atl-0.0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tess-atl-0.0.2.tar", last modified: Tue Jul 25 06:59:55 2023, max compression
+gzip compressed data, was "tess-atl-0.0.2.dev0.tar", last modified: Tue Jul 25 07:05:04 2023, max compression
```

## Comparing `tess-atl-0.0.2.tar` & `tess-atl-0.0.2.dev0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-25 06:59:55.804406 tess-atl-0.0.2/
--rw-r--r--   0 daniel     (501) staff       (20)      295 2023-07-25 06:59:55.804230 tess-atl-0.0.2/PKG-INFO
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-25 06:59:55.802944 tess-atl-0.0.2/atl/
--rw-r--r--   0 daniel     (501) staff       (20)        0 2023-07-25 01:50:22.000000 tess-atl-0.0.2/atl/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)     7076 2023-07-25 06:50:40.000000 tess-atl-0.0.2/atl/atl.py
--rw-r--r--   0 daniel     (501) staff       (20)     3246 2023-07-25 06:52:40.000000 tess-atl-0.0.2/atl/cli.py
--rw-r--r--   0 daniel     (501) staff       (20)      148 2023-07-25 02:17:54.000000 tess-atl-0.0.2/atl/constants.py
--rw-r--r--   0 daniel     (501) staff       (20)     4283 2023-07-25 05:32:29.000000 tess-atl-0.0.2/atl/noise.py
--rw-r--r--   0 daniel     (501) staff       (20)     1899 2023-07-25 03:19:42.000000 tess-atl-0.0.2/atl/query.py
--rw-r--r--   0 daniel     (501) staff       (20)     1066 2023-07-25 06:30:15.000000 tess-atl-0.0.2/atl/scaling.py
--rw-r--r--   0 daniel     (501) staff       (20)    70607 2023-07-25 02:01:10.000000 tess-atl-0.0.2/atl/tess_stars2px.py
--rw-r--r--   0 daniel     (501) staff       (20)       22 2023-07-25 06:58:59.000000 tess-atl-0.0.2/atl/version.py
--rw-r--r--   0 daniel     (501) staff       (20)       38 2023-07-25 06:59:55.804451 tess-atl-0.0.2/setup.cfg
--rw-r--r--   0 daniel     (501) staff       (20)      959 2023-07-25 06:42:18.000000 tess-atl-0.0.2/setup.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-25 06:59:55.804012 tess-atl-0.0.2/tess_atl.egg-info/
--rw-r--r--   0 daniel     (501) staff       (20)      295 2023-07-25 06:59:55.000000 tess-atl-0.0.2/tess_atl.egg-info/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)      334 2023-07-25 06:59:55.000000 tess-atl-0.0.2/tess_atl.egg-info/SOURCES.txt
--rw-r--r--   0 daniel     (501) staff       (20)        1 2023-07-25 06:59:55.000000 tess-atl-0.0.2/tess_atl.egg-info/dependency_links.txt
--rw-r--r--   0 daniel     (501) staff       (20)       37 2023-07-25 06:59:55.000000 tess-atl-0.0.2/tess_atl.egg-info/entry_points.txt
--rw-r--r--   0 daniel     (501) staff       (20)       38 2023-07-25 06:59:55.000000 tess-atl-0.0.2/tess_atl.egg-info/requires.txt
--rw-r--r--   0 daniel     (501) staff       (20)        4 2023-07-25 06:59:55.000000 tess-atl-0.0.2/tess_atl.egg-info/top_level.txt
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-25 07:05:04.260287 tess-atl-0.0.2.dev0/
+-rw-r--r--   0 daniel     (501) staff       (20)      300 2023-07-25 07:05:04.260068 tess-atl-0.0.2.dev0/PKG-INFO
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-25 07:05:04.258413 tess-atl-0.0.2.dev0/atl/
+-rw-r--r--   0 daniel     (501) staff       (20)        0 2023-07-25 01:50:22.000000 tess-atl-0.0.2.dev0/atl/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     7076 2023-07-25 06:50:40.000000 tess-atl-0.0.2.dev0/atl/atl.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3246 2023-07-25 06:52:40.000000 tess-atl-0.0.2.dev0/atl/cli.py
+-rw-r--r--   0 daniel     (501) staff       (20)      148 2023-07-25 02:17:54.000000 tess-atl-0.0.2.dev0/atl/constants.py
+-rw-r--r--   0 daniel     (501) staff       (20)     4283 2023-07-25 05:32:29.000000 tess-atl-0.0.2.dev0/atl/noise.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1899 2023-07-25 03:19:42.000000 tess-atl-0.0.2.dev0/atl/query.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1066 2023-07-25 06:30:15.000000 tess-atl-0.0.2.dev0/atl/scaling.py
+-rw-r--r--   0 daniel     (501) staff       (20)    70607 2023-07-25 02:01:10.000000 tess-atl-0.0.2.dev0/atl/tess_stars2px.py
+-rw-r--r--   0 daniel     (501) staff       (20)       27 2023-07-25 07:04:46.000000 tess-atl-0.0.2.dev0/atl/version.py
+-rw-r--r--   0 daniel     (501) staff       (20)       38 2023-07-25 07:05:04.260342 tess-atl-0.0.2.dev0/setup.cfg
+-rw-r--r--   0 daniel     (501) staff       (20)      959 2023-07-25 07:04:37.000000 tess-atl-0.0.2.dev0/setup.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-25 07:05:04.259727 tess-atl-0.0.2.dev0/tess_atl.egg-info/
+-rw-r--r--   0 daniel     (501) staff       (20)      300 2023-07-25 07:05:04.000000 tess-atl-0.0.2.dev0/tess_atl.egg-info/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)      334 2023-07-25 07:05:04.000000 tess-atl-0.0.2.dev0/tess_atl.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        1 2023-07-25 07:05:04.000000 tess-atl-0.0.2.dev0/tess_atl.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       37 2023-07-25 07:05:04.000000 tess-atl-0.0.2.dev0/tess_atl.egg-info/entry_points.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       38 2023-07-25 07:05:04.000000 tess-atl-0.0.2.dev0/tess_atl.egg-info/requires.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        4 2023-07-25 07:05:04.000000 tess-atl-0.0.2.dev0/tess_atl.egg-info/top_level.txt
```

### Comparing `tess-atl-0.0.2/atl/atl.py` & `tess-atl-0.0.2.dev0/atl/atl.py`

 * *Files identical despite different names*

### Comparing `tess-atl-0.0.2/atl/cli.py` & `tess-atl-0.0.2.dev0/atl/cli.py`

 * *Files identical despite different names*

### Comparing `tess-atl-0.0.2/atl/noise.py` & `tess-atl-0.0.2.dev0/atl/noise.py`

 * *Files identical despite different names*

### Comparing `tess-atl-0.0.2/atl/query.py` & `tess-atl-0.0.2.dev0/atl/query.py`

 * *Files identical despite different names*

### Comparing `tess-atl-0.0.2/atl/scaling.py` & `tess-atl-0.0.2.dev0/atl/scaling.py`

 * *Files identical despite different names*

### Comparing `tess-atl-0.0.2/atl/tess_stars2px.py` & `tess-atl-0.0.2.dev0/atl/tess_stars2px.py`

 * *Files identical despite different names*

### Comparing `tess-atl-0.0.2/setup.py` & `tess-atl-0.0.2.dev0/setup.py`

 * *Files identical despite different names*

