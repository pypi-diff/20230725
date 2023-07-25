# Comparing `tmp/py3dtiles-5.0.0.tar.gz` & `tmp/py3dtiles-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3dtiles-5.0.0.tar", last modified: Fri Feb  3 14:02:22 2023, max compression
+gzip compressed data, was "py3dtiles-6.0.0.tar", last modified: Tue Jul 25 15:44:34 2023, max compression
```

## Comparing `py3dtiles-5.0.0.tar` & `py3dtiles-6.0.0.tar`

### file list

```diff
@@ -1,81 +1,87 @@
-drwxrwx---   0 augustin  (1000) augustin  (1000)        0 2023-02-03 14:02:22.887074 py3dtiles-5.0.0/
--rw-rw----   0 augustin  (1000) augustin  (1000)      690 2023-01-24 09:50:57.000000 py3dtiles-5.0.0/LICENSE
--rw-rw----   0 augustin  (1000) augustin  (1000)       83 2022-10-24 09:30:31.000000 py3dtiles-5.0.0/MANIFEST.in
--rw-rw----   0 augustin  (1000) augustin  (1000)     1446 2023-02-03 14:02:22.887074 py3dtiles-5.0.0/PKG-INFO
--rw-rw----   0 augustin  (1000) augustin  (1000)      931 2023-01-17 13:18:34.000000 py3dtiles-5.0.0/README.rst
-drwxrwx---   0 augustin  (1000) augustin  (1000)        0 2023-02-03 14:02:22.875074 py3dtiles-5.0.0/py3dtiles/
--rw-rw----   0 augustin  (1000) augustin  (1000)       22 2023-02-03 13:56:49.000000 py3dtiles-5.0.0/py3dtiles/__init__.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     1063 2023-01-24 09:50:57.000000 py3dtiles-5.0.0/py3dtiles/command_line.py
--rw-rw----   0 augustin  (1000) augustin  (1000)    38363 2023-02-02 17:14:07.000000 py3dtiles-5.0.0/py3dtiles/convert.py
--rw-rw----   0 augustin  (1000) augustin  (1000)      680 2023-01-09 09:03:23.000000 py3dtiles-5.0.0/py3dtiles/exceptions.py
--rw-rw----   0 augustin  (1000) augustin  (1000)    11348 2023-01-24 09:50:57.000000 py3dtiles-5.0.0/py3dtiles/export.py
--rwxrwx---   0 augustin  (1000) augustin  (1000)     2556 2023-02-02 17:14:07.000000 py3dtiles-5.0.0/py3dtiles/info.py
--rw-rw----   0 augustin  (1000) augustin  (1000)    10188 2023-02-02 17:14:07.000000 py3dtiles-5.0.0/py3dtiles/merger.py
-drwxrwx---   0 augustin  (1000) augustin  (1000)        0 2023-02-03 14:02:22.875074 py3dtiles-5.0.0/py3dtiles/reader/
--rw-rw----   0 augustin  (1000) augustin  (1000)        0 2023-01-24 09:50:57.000000 py3dtiles-5.0.0/py3dtiles/reader/__init__.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     4359 2023-01-24 09:50:57.000000 py3dtiles-5.0.0/py3dtiles/reader/las_reader.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     4014 2023-01-24 09:50:57.000000 py3dtiles-5.0.0/py3dtiles/reader/ply_reader.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     5036 2023-02-02 17:14:07.000000 py3dtiles-5.0.0/py3dtiles/reader/xyz_reader.py
-drwxrwx---   0 augustin  (1000) augustin  (1000)        0 2023-02-03 14:02:22.875074 py3dtiles-5.0.0/py3dtiles/tilers/
--rw-rw----   0 augustin  (1000) augustin  (1000)        0 2023-01-24 09:50:57.000000 py3dtiles-5.0.0/py3dtiles/tilers/__init__.py
-drwxrwx---   0 augustin  (1000) augustin  (1000)        0 2023-02-03 14:02:22.879074 py3dtiles-5.0.0/py3dtiles/tilers/b3dm/
--rw-rw----   0 augustin  (1000) augustin  (1000)       24 2023-01-24 09:50:57.000000 py3dtiles-5.0.0/py3dtiles/tilers/b3dm/__init__.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     9053 2023-01-24 09:50:57.000000 py3dtiles-5.0.0/py3dtiles/tilers/b3dm/wkb_utils.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     1201 2023-01-24 09:50:57.000000 py3dtiles-5.0.0/py3dtiles/tilers/matrix_manipulation.py
-drwxrwx---   0 augustin  (1000) augustin  (1000)        0 2023-02-03 14:02:22.879074 py3dtiles-5.0.0/py3dtiles/tilers/node/
--rw-rw----   0 augustin  (1000) augustin  (1000)      138 2023-01-24 09:50:57.000000 py3dtiles-5.0.0/py3dtiles/tilers/node/__init__.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     1168 2023-02-02 17:14:07.000000 py3dtiles-5.0.0/py3dtiles/tilers/node/distance.py
--rw-rw----   0 augustin  (1000) augustin  (1000)    12810 2023-02-02 17:14:07.000000 py3dtiles-5.0.0/py3dtiles/tilers/node/node.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     2510 2023-02-02 17:14:07.000000 py3dtiles-5.0.0/py3dtiles/tilers/node/node_catalog.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     5227 2023-01-24 09:50:57.000000 py3dtiles-5.0.0/py3dtiles/tilers/node/node_process.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     4942 2023-02-02 17:14:07.000000 py3dtiles-5.0.0/py3dtiles/tilers/node/points_grid.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     4596 2023-02-02 17:14:07.000000 py3dtiles-5.0.0/py3dtiles/tilers/node/shared_node_store.py
-drwxrwx---   0 augustin  (1000) augustin  (1000)        0 2023-02-03 14:02:22.879074 py3dtiles-5.0.0/py3dtiles/tilers/pnts/
--rw-rw----   0 augustin  (1000) augustin  (1000)       64 2023-01-24 09:50:57.000000 py3dtiles-5.0.0/py3dtiles/tilers/pnts/__init__.py
--rw-rw----   0 augustin  (1000) augustin  (1000)      237 2023-01-24 09:50:57.000000 py3dtiles-5.0.0/py3dtiles/tilers/pnts/constants.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     2014 2023-01-24 09:50:57.000000 py3dtiles-5.0.0/py3dtiles/tilers/pnts/pnts_writer.py
-drwxrwx---   0 augustin  (1000) augustin  (1000)        0 2023-02-03 14:02:22.883074 py3dtiles-5.0.0/py3dtiles/tileset/
--rw-rw----   0 augustin  (1000) augustin  (1000)        0 2023-01-24 09:50:57.000000 py3dtiles-5.0.0/py3dtiles/tileset/__init__.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     1749 2023-02-02 17:14:07.000000 py3dtiles-5.0.0/py3dtiles/tileset/batch_table.py
--rw-rw----   0 augustin  (1000) augustin  (1000)      968 2023-02-02 17:14:07.000000 py3dtiles-5.0.0/py3dtiles/tileset/bounding_volume.py
--rw-rw----   0 augustin  (1000) augustin  (1000)    10193 2023-02-02 17:14:07.000000 py3dtiles-5.0.0/py3dtiles/tileset/bounding_volume_box.py
-drwxrwx---   0 augustin  (1000) augustin  (1000)        0 2023-02-03 14:02:22.883074 py3dtiles-5.0.0/py3dtiles/tileset/content/
--rw-rw----   0 augustin  (1000) augustin  (1000)       63 2023-01-24 09:50:57.000000 py3dtiles-5.0.0/py3dtiles/tileset/content/__init__.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     5197 2023-02-02 17:14:07.000000 py3dtiles-5.0.0/py3dtiles/tileset/content/b3dm.py
--rw-rw----   0 augustin  (1000) augustin  (1000)    10084 2023-01-24 09:50:57.000000 py3dtiles-5.0.0/py3dtiles/tileset/content/gltf.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     5437 2023-02-02 17:14:07.000000 py3dtiles-5.0.0/py3dtiles/tileset/content/pnts.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     1189 2023-02-02 17:14:07.000000 py3dtiles-5.0.0/py3dtiles/tileset/extendable.py
-drwxrwx---   0 augustin  (1000) augustin  (1000)        0 2023-02-03 14:02:22.883074 py3dtiles-5.0.0/py3dtiles/tileset/extension/
--rw-rw----   0 augustin  (1000) augustin  (1000)       42 2023-01-24 09:50:57.000000 py3dtiles-5.0.0/py3dtiles/tileset/extension/__init__.py
--rw-rw----   0 augustin  (1000) augustin  (1000)      276 2023-02-02 17:14:07.000000 py3dtiles-5.0.0/py3dtiles/tileset/extension/base_extension.py
--rw-rw----   0 augustin  (1000) augustin  (1000)    12472 2023-02-02 17:14:07.000000 py3dtiles-5.0.0/py3dtiles/tileset/feature_table.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     5975 2023-02-02 17:14:07.000000 py3dtiles-5.0.0/py3dtiles/tileset/tile.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     1561 2023-02-02 17:14:07.000000 py3dtiles-5.0.0/py3dtiles/tileset/tile_content.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     3032 2023-02-02 17:14:07.000000 py3dtiles-5.0.0/py3dtiles/tileset/tileset.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     1022 2023-01-24 09:50:57.000000 py3dtiles-5.0.0/py3dtiles/tileset/utils.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     1687 2023-02-02 17:14:07.000000 py3dtiles-5.0.0/py3dtiles/typing.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     3570 2023-02-02 17:14:07.000000 py3dtiles-5.0.0/py3dtiles/utils.py
-drwxrwx---   0 augustin  (1000) augustin  (1000)        0 2023-02-03 14:02:22.875074 py3dtiles-5.0.0/py3dtiles.egg-info/
--rw-rw-r--   0 augustin  (1000) augustin  (1000)     1446 2023-02-03 14:02:22.000000 py3dtiles-5.0.0/py3dtiles.egg-info/PKG-INFO
--rw-rw-r--   0 augustin  (1000) augustin  (1000)     1940 2023-02-03 14:02:22.000000 py3dtiles-5.0.0/py3dtiles.egg-info/SOURCES.txt
--rw-rw-r--   0 augustin  (1000) augustin  (1000)        1 2023-02-03 14:02:22.000000 py3dtiles-5.0.0/py3dtiles.egg-info/dependency_links.txt
--rw-rw-r--   0 augustin  (1000) augustin  (1000)       58 2023-02-03 14:02:22.000000 py3dtiles-5.0.0/py3dtiles.egg-info/entry_points.txt
--rw-rw-r--   0 augustin  (1000) augustin  (1000)        1 2019-05-24 16:00:22.000000 py3dtiles-5.0.0/py3dtiles.egg-info/not-zip-safe
--rw-rw-r--   0 augustin  (1000) augustin  (1000)      383 2023-02-03 14:02:22.000000 py3dtiles-5.0.0/py3dtiles.egg-info/requires.txt
--rw-rw-r--   0 augustin  (1000) augustin  (1000)       16 2023-02-03 14:02:22.000000 py3dtiles-5.0.0/py3dtiles.egg-info/top_level.txt
--rw-rw----   0 augustin  (1000) augustin  (1000)      582 2023-02-03 14:02:22.891074 py3dtiles-5.0.0/setup.cfg
--rw-rw----   0 augustin  (1000) augustin  (1000)     2377 2023-02-03 14:02:09.000000 py3dtiles-5.0.0/setup.py
-drwxrwx---   0 augustin  (1000) augustin  (1000)        0 2023-02-03 14:02:22.887074 py3dtiles-5.0.0/tests/
--rw-rw----   0 augustin  (1000) augustin  (1000)        0 2021-03-05 17:00:58.000000 py3dtiles-5.0.0/tests/__init__.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     4731 2023-01-24 09:50:58.000000 py3dtiles-5.0.0/tests/test_b3dm.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     1831 2023-02-02 17:14:07.000000 py3dtiles-5.0.0/tests/test_batch_table.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     6463 2023-02-02 17:14:07.000000 py3dtiles-5.0.0/tests/test_bounding_volume_box.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     8901 2023-02-02 17:14:07.000000 py3dtiles-5.0.0/tests/test_convert.py
--rw-rw----   0 augustin  (1000) augustin  (1000)      429 2023-01-24 09:50:58.000000 py3dtiles-5.0.0/tests/test_extension.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     4333 2023-01-24 09:50:58.000000 py3dtiles-5.0.0/tests/test_pc.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     3011 2023-01-24 09:50:58.000000 py3dtiles-5.0.0/tests/test_points.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     2697 2023-01-24 09:50:58.000000 py3dtiles-5.0.0/tests/test_reader.py
--rw-rw----   0 augustin  (1000) augustin  (1000)      787 2023-02-02 17:14:07.000000 py3dtiles-5.0.0/tests/test_shared_node_store.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     5380 2023-02-02 17:14:07.000000 py3dtiles-5.0.0/tests/test_tile.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     2055 2023-02-02 17:14:07.000000 py3dtiles-5.0.0/tests/test_tileset.py
--rw-rw----   0 augustin  (1000) augustin  (1000)     7635 2023-01-24 09:50:58.000000 py3dtiles-5.0.0/tests/test_wkb_utils.py
+drwxrwx---   0 augustin  (1000) augustin  (1000)        0 2023-07-25 15:44:34.841438 py3dtiles-6.0.0/
+-rw-rw----   0 augustin  (1000) augustin  (1000)      690 2023-03-14 14:40:39.000000 py3dtiles-6.0.0/LICENSE
+-rw-rw----   0 augustin  (1000) augustin  (1000)       83 2022-10-24 09:30:31.000000 py3dtiles-6.0.0/MANIFEST.in
+-rw-rw----   0 augustin  (1000) augustin  (1000)     5735 2023-07-25 15:44:34.841438 py3dtiles-6.0.0/PKG-INFO
+-rw-rw----   0 augustin  (1000) augustin  (1000)     5113 2023-07-21 14:19:46.000000 py3dtiles-6.0.0/README.rst
+drwxrwx---   0 augustin  (1000) augustin  (1000)        0 2023-07-25 15:44:34.813437 py3dtiles-6.0.0/py3dtiles/
+-rw-rw----   0 augustin  (1000) augustin  (1000)       22 2023-07-24 15:34:44.000000 py3dtiles-6.0.0/py3dtiles/__init__.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     1078 2023-07-11 14:41:40.000000 py3dtiles-6.0.0/py3dtiles/command_line.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)    48066 2023-07-24 15:34:44.000000 py3dtiles-6.0.0/py3dtiles/convert.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     1545 2023-07-11 14:41:40.000000 py3dtiles-6.0.0/py3dtiles/exceptions.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)    11952 2023-07-11 14:41:40.000000 py3dtiles-6.0.0/py3dtiles/export.py
+-rwxrwx---   0 augustin  (1000) augustin  (1000)      682 2023-07-11 14:41:40.000000 py3dtiles-6.0.0/py3dtiles/info.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)    11064 2023-07-11 14:41:40.000000 py3dtiles-6.0.0/py3dtiles/merger.py
+drwxrwx---   0 augustin  (1000) augustin  (1000)        0 2023-07-25 15:44:34.817437 py3dtiles-6.0.0/py3dtiles/reader/
+-rw-rw----   0 augustin  (1000) augustin  (1000)        0 2023-03-14 14:40:39.000000 py3dtiles-6.0.0/py3dtiles/reader/__init__.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     3648 2023-07-11 14:41:40.000000 py3dtiles-6.0.0/py3dtiles/reader/las_reader.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     5517 2023-07-11 14:41:40.000000 py3dtiles-6.0.0/py3dtiles/reader/ply_reader.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     4961 2023-07-11 14:41:40.000000 py3dtiles-6.0.0/py3dtiles/reader/xyz_reader.py
+drwxrwx---   0 augustin  (1000) augustin  (1000)        0 2023-07-25 15:44:34.817437 py3dtiles-6.0.0/py3dtiles/tilers/
+-rw-rw----   0 augustin  (1000) augustin  (1000)        0 2023-03-14 14:40:39.000000 py3dtiles-6.0.0/py3dtiles/tilers/__init__.py
+drwxrwx---   0 augustin  (1000) augustin  (1000)        0 2023-07-25 15:44:34.817437 py3dtiles-6.0.0/py3dtiles/tilers/b3dm/
+-rw-rw----   0 augustin  (1000) augustin  (1000)       49 2023-07-11 14:41:40.000000 py3dtiles-6.0.0/py3dtiles/tilers/b3dm/__init__.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     9871 2023-07-21 13:20:20.000000 py3dtiles-6.0.0/py3dtiles/tilers/b3dm/wkb_utils.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     1495 2023-07-11 14:41:40.000000 py3dtiles-6.0.0/py3dtiles/tilers/matrix_manipulation.py
+drwxrwx---   0 augustin  (1000) augustin  (1000)        0 2023-07-25 15:44:34.821437 py3dtiles-6.0.0/py3dtiles/tilers/node/
+-rw-rw----   0 augustin  (1000) augustin  (1000)      277 2023-07-11 14:41:40.000000 py3dtiles-6.0.0/py3dtiles/tilers/node/__init__.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     1208 2023-07-21 13:20:20.000000 py3dtiles-6.0.0/py3dtiles/tilers/node/distance.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)    18706 2023-07-21 13:20:20.000000 py3dtiles-6.0.0/py3dtiles/tilers/node/node.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     2522 2023-07-20 10:24:19.000000 py3dtiles-6.0.0/py3dtiles/tilers/node/node_catalog.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     4773 2023-07-11 14:41:40.000000 py3dtiles-6.0.0/py3dtiles/tilers/node/node_process.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     7138 2023-07-21 13:20:20.000000 py3dtiles-6.0.0/py3dtiles/tilers/node/points_grid.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     4853 2023-07-21 13:20:20.000000 py3dtiles-6.0.0/py3dtiles/tilers/node/shared_node_store.py
+drwxrwx---   0 augustin  (1000) augustin  (1000)        0 2023-07-25 15:44:34.821437 py3dtiles-6.0.0/py3dtiles/tilers/pnts/
+-rw-rw----   0 augustin  (1000) augustin  (1000)      109 2023-07-11 14:41:40.000000 py3dtiles-6.0.0/py3dtiles/tilers/pnts/__init__.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)      237 2023-03-14 14:40:39.000000 py3dtiles-6.0.0/py3dtiles/tilers/pnts/constants.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     1975 2023-07-21 13:20:20.000000 py3dtiles-6.0.0/py3dtiles/tilers/pnts/pnts_writer.py
+drwxrwx---   0 augustin  (1000) augustin  (1000)        0 2023-07-25 15:44:34.825437 py3dtiles-6.0.0/py3dtiles/tileset/
+-rw-rw----   0 augustin  (1000) augustin  (1000)      410 2023-07-11 14:41:40.000000 py3dtiles-6.0.0/py3dtiles/tileset/__init__.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     1694 2023-07-21 13:20:20.000000 py3dtiles-6.0.0/py3dtiles/tileset/bounding_volume.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)    10508 2023-07-21 13:20:20.000000 py3dtiles-6.0.0/py3dtiles/tileset/bounding_volume_box.py
+drwxrwx---   0 augustin  (1000) augustin  (1000)        0 2023-07-25 15:44:34.825437 py3dtiles-6.0.0/py3dtiles/tileset/content/
+-rw-rw----   0 augustin  (1000) augustin  (1000)      503 2023-07-11 14:41:40.000000 py3dtiles-6.0.0/py3dtiles/tileset/content/__init__.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     6366 2023-07-21 13:20:20.000000 py3dtiles-6.0.0/py3dtiles/tileset/content/b3dm.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     6659 2023-07-21 13:20:20.000000 py3dtiles-6.0.0/py3dtiles/tileset/content/batch_table.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)    19148 2023-07-21 13:20:20.000000 py3dtiles-6.0.0/py3dtiles/tileset/content/feature_table.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)    10727 2023-07-11 14:41:40.000000 py3dtiles-6.0.0/py3dtiles/tileset/content/gltf.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)    10148 2023-07-21 13:20:20.000000 py3dtiles-6.0.0/py3dtiles/tileset/content/pnts.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     1851 2023-07-11 14:41:40.000000 py3dtiles-6.0.0/py3dtiles/tileset/content/tile_content.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     1077 2023-07-21 13:20:20.000000 py3dtiles-6.0.0/py3dtiles/tileset/content/tile_content_reader.py
+drwxrwx---   0 augustin  (1000) augustin  (1000)        0 2023-07-25 15:44:34.829437 py3dtiles-6.0.0/py3dtiles/tileset/extension/
+-rw-rw----   0 augustin  (1000) augustin  (1000)      159 2023-07-11 14:41:40.000000 py3dtiles-6.0.0/py3dtiles/tileset/extension/__init__.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)      803 2023-07-11 14:41:40.000000 py3dtiles-6.0.0/py3dtiles/tileset/extension/base_extension.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     3757 2023-07-11 14:41:40.000000 py3dtiles-6.0.0/py3dtiles/tileset/extension/batch_table_hierarchy_extension.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     1524 2023-07-21 13:20:20.000000 py3dtiles-6.0.0/py3dtiles/tileset/root_property.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)    10985 2023-07-21 13:20:20.000000 py3dtiles-6.0.0/py3dtiles/tileset/tile.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     5885 2023-07-21 13:20:20.000000 py3dtiles-6.0.0/py3dtiles/tileset/tileset.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     1368 2023-07-11 14:41:40.000000 py3dtiles-6.0.0/py3dtiles/tileset/utils.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     2908 2023-07-21 13:20:20.000000 py3dtiles-6.0.0/py3dtiles/typing.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     4570 2023-07-24 15:34:44.000000 py3dtiles-6.0.0/py3dtiles/utils.py
+drwxrwx---   0 augustin  (1000) augustin  (1000)        0 2023-07-25 15:44:34.817437 py3dtiles-6.0.0/py3dtiles.egg-info/
+-rw-rw-r--   0 augustin  (1000) augustin  (1000)     5735 2023-07-25 15:44:34.000000 py3dtiles-6.0.0/py3dtiles.egg-info/PKG-INFO
+-rw-rw-r--   0 augustin  (1000) augustin  (1000)     2195 2023-07-25 15:44:34.000000 py3dtiles-6.0.0/py3dtiles.egg-info/SOURCES.txt
+-rw-rw-r--   0 augustin  (1000) augustin  (1000)        1 2023-07-25 15:44:34.000000 py3dtiles-6.0.0/py3dtiles.egg-info/dependency_links.txt
+-rw-rw-r--   0 augustin  (1000) augustin  (1000)       58 2023-07-25 15:44:34.000000 py3dtiles-6.0.0/py3dtiles.egg-info/entry_points.txt
+-rw-rw-r--   0 augustin  (1000) augustin  (1000)        1 2019-05-24 16:00:22.000000 py3dtiles-6.0.0/py3dtiles.egg-info/not-zip-safe
+-rw-rw-r--   0 augustin  (1000) augustin  (1000)      439 2023-07-25 15:44:34.000000 py3dtiles-6.0.0/py3dtiles.egg-info/requires.txt
+-rw-rw-r--   0 augustin  (1000) augustin  (1000)       16 2023-07-25 15:44:34.000000 py3dtiles-6.0.0/py3dtiles.egg-info/top_level.txt
+-rw-rw----   0 augustin  (1000) augustin  (1000)      644 2023-07-25 15:44:34.845438 py3dtiles-6.0.0/setup.cfg
+-rw-rw----   0 augustin  (1000) augustin  (1000)     2441 2023-07-11 14:41:40.000000 py3dtiles-6.0.0/setup.py
+drwxrwx---   0 augustin  (1000) augustin  (1000)        0 2023-07-25 15:44:34.841438 py3dtiles-6.0.0/tests/
+-rw-rw----   0 augustin  (1000) augustin  (1000)        0 2021-03-05 17:00:58.000000 py3dtiles-6.0.0/tests/__init__.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     6459 2023-07-21 13:20:20.000000 py3dtiles-6.0.0/tests/test_b3dm.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     9615 2023-07-11 14:41:40.000000 py3dtiles-6.0.0/tests/test_batch_table.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     4192 2023-07-11 14:41:40.000000 py3dtiles-6.0.0/tests/test_batch_table_hierachy_extension.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     5721 2023-07-21 13:20:20.000000 py3dtiles-6.0.0/tests/test_bounding_volume_box.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)      899 2023-07-21 13:20:20.000000 py3dtiles-6.0.0/tests/test_code_examples.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)    24268 2023-07-24 15:34:44.000000 py3dtiles-6.0.0/tests/test_convert.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)      314 2023-07-11 14:41:40.000000 py3dtiles-6.0.0/tests/test_extension.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     9653 2023-07-21 13:20:20.000000 py3dtiles-6.0.0/tests/test_merger.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     5421 2023-07-21 13:20:20.000000 py3dtiles-6.0.0/tests/test_pnts.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     3621 2023-07-21 13:20:20.000000 py3dtiles-6.0.0/tests/test_points.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     3427 2023-07-21 13:20:20.000000 py3dtiles-6.0.0/tests/test_reader.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)      796 2023-07-21 13:20:20.000000 py3dtiles-6.0.0/tests/test_shared_node_store.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     7352 2023-07-21 13:20:20.000000 py3dtiles-6.0.0/tests/test_tile.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     4843 2023-07-21 13:20:20.000000 py3dtiles-6.0.0/tests/test_tileset.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)      672 2023-07-24 15:34:44.000000 py3dtiles-6.0.0/tests/test_utils.py
+-rw-rw----   0 augustin  (1000) augustin  (1000)     8172 2023-07-11 14:41:40.000000 py3dtiles-6.0.0/tests/test_wkb_utils.py
```

### Comparing `py3dtiles-5.0.0/LICENSE` & `py3dtiles-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py3dtiles-5.0.0/py3dtiles/command_line.py` & `py3dtiles-6.0.0/py3dtiles/command_line.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import argparse
 
 from py3dtiles import convert, export, info, merger
 
 
-def main():
+def main() -> None:
     parser = argparse.ArgumentParser(
-        description='Read/write 3dtiles files',
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-    sub_parsers = parser.add_subparsers(dest='command')
+        description="Read/write 3dtiles files",
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+    )
+    sub_parsers = parser.add_subparsers(dest="command")
 
     # init subparsers
     command_parsers = [
         convert.init_parser(sub_parsers),
         info.init_parser(sub_parsers),
         merger.init_parser(sub_parsers),
-        export.init_parser(sub_parsers)
+        export.init_parser(sub_parsers),
     ]
     # add the verbose argument for all sub-parsers so that it is after the command.
     for command_parser in command_parsers:
-        command_parser.add_argument('--verbose', '-v', action='count', default=0)
+        command_parser.add_argument("--verbose", "-v", action="count", default=0)
 
     args = parser.parse_args()
 
-    if args.command == 'convert':
+    if args.command == "convert":
         convert.main(args)
-    elif args.command == 'info':
+    elif args.command == "info":
         info.main(args)
-    elif args.command == 'merge':
+    elif args.command == "merge":
         merger.main(args)
-    elif args.command == 'export':
+    elif args.command == "export":
         export.main(args)
     else:
         parser.print_help()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `py3dtiles-5.0.0/py3dtiles/convert.py` & `py3dtiles-6.0.0/py3dtiles/convert.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,86 +1,140 @@
 import argparse
-from collections import namedtuple
 import concurrent.futures
 import json
 from multiprocessing import cpu_count, Process
 import os
 from pathlib import Path, PurePath
 import pickle
 import shutil
 import struct
 import sys
+import tempfile
 import time
 import traceback
-from typing import Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
+import numpy.typing as npt
 import psutil
 from pyproj import CRS, Transformer
 import zmq
 
-from py3dtiles.exceptions import SrsInMissingException, SrsInMixinException, WorkerException
+from py3dtiles.exceptions import (
+    SrsInMissingException,
+    SrsInMixinException,
+    TilerException,
+    WorkerException,
+)
 from py3dtiles.reader import las_reader, ply_reader, xyz_reader
-from py3dtiles.tilers.matrix_manipulation import make_rotation_matrix, make_scale_matrix, make_translation_matrix
-from py3dtiles.tilers.node import Node
-from py3dtiles.tilers.node import node_process
-from py3dtiles.tilers.node import SharedNodeStore
+from py3dtiles.tilers.matrix_manipulation import (
+    make_rotation_matrix,
+    make_scale_matrix,
+    make_translation_matrix,
+)
+from py3dtiles.tilers.node import Node, NodeCatalog, NodeProcess, SharedNodeStore
 from py3dtiles.tilers.pnts import pnts_writer
 from py3dtiles.tilers.pnts.constants import MIN_POINT_SIZE
-from py3dtiles.tileset.utils import TileContentReader
-from py3dtiles.utils import CommandType, compute_spacing, node_name_to_path, ResponseType, str_to_CRS
+from py3dtiles.tileset.content import read_binary_tile_content
+from py3dtiles.typing import PortionsType
+from py3dtiles.utils import (
+    CommandType,
+    compute_spacing,
+    make_aabb_valid,
+    node_from_name,
+    node_name_to_path,
+    OctreeMetadata,
+    ResponseType,
+    str_to_CRS,
+)
 
 TOTAL_MEMORY_MB = int(psutil.virtual_memory().total / (1024 * 1024))
 DEFAULT_CACHE_SIZE = int(TOTAL_MEMORY_MB / 10)
 CPU_COUNT = cpu_count()
 
 # IPC protocol is not supported on Windows
-if os.name == 'nt':
-    URI = 'tcp://127.0.0.1:0'
+if os.name == "nt":
+    URI = "tcp://127.0.0.1:0"
 else:
-    URI = "ipc:///tmp/py3dtiles1"
-
-OctreeMetadata = namedtuple('OctreeMetadata', ['aabb', 'spacing', 'scale'])
+    # Generate a unique name for this socket
+    tmpdir = tempfile.TemporaryDirectory()
+    URI = f"ipc://{tmpdir.name}/py3dtiles.sock"
 
 READER_MAP = {
-    '.xyz': xyz_reader,
-    '.las': las_reader,
-    '.laz': las_reader,
-    '.ply': ply_reader,
+    ".xyz": xyz_reader,
+    ".las": las_reader,
+    ".laz": las_reader,
+    ".ply": ply_reader,
 }
 
 
-class Worker(Process):
+def worker_target(
+    activity_graph: bool,
+    transformer: Optional[Transformer],
+    octree_metadata: OctreeMetadata,
+    folder: Path,
+    write_rgb: bool,
+    color_scale: Optional[float],
+    write_classification: bool,
+    verbosity: int,
+    uri: bytes,
+) -> None:
+    return Worker(
+        activity_graph,
+        transformer,
+        octree_metadata,
+        folder,
+        write_rgb,
+        color_scale,
+        write_classification,
+        verbosity,
+        uri,
+    ).run()
+
+
+class Worker:
     """
     This class waits from jobs commands from the Zmq socket.
     """
-    def __init__(self, activity_graph, transformer, octree_metadata, folder: Path, write_rgb, verbosity, uri):
-        super().__init__()
+
+    def __init__(
+        self,
+        activity_graph: bool,
+        transformer: Optional[Transformer],
+        octree_metadata: OctreeMetadata,
+        folder: Path,
+        write_rgb: bool,
+        color_scale: Optional[float],
+        write_classification: bool,
+        verbosity: int,
+        uri: bytes,
+    ) -> None:
         self.activity_graph = activity_graph
         self.transformer = transformer
         self.octree_metadata = octree_metadata
         self.folder = folder
         self.write_rgb = write_rgb
+        self.color_scale = color_scale
+        self.write_classification = write_classification
         self.verbosity = verbosity
         self.uri = uri
 
         # Socket to receive messages on
         self.context = zmq.Context()
-        self.skt = None
 
-    def run(self):
-        self.skt = self.context.socket(zmq.DEALER)
+    def run(self) -> None:
+        self.skt: zmq.Socket[bytes] = self.context.socket(zmq.DEALER)
 
-        self.skt.connect(self.uri)
+        self.skt.connect(self.uri)  # type: ignore [arg-type]
 
         startup_time = time.time()
-        idle_time = 0
+        idle_time = 0.0
 
         if self.activity_graph:
-            activity = open(f'activity.{os.getpid()}.csv', 'w')
+            activity = open(f"activity.{os.getpid()}.csv", "w")
 
         # notify we're ready
         self.skt.send_multipart([ResponseType.IDLE.value])
 
         while True:
             try:
                 before = time.time() - startup_time
@@ -91,183 +145,306 @@
 
                 message = self.skt.recv_multipart()
                 content = message[1:]
                 command = content[0]
 
                 delta = time.time() - pickle.loads(message[0])
                 if delta > 0.01 and self.verbosity >= 1:
-                    print(f'{os.getpid()} / {round(after, 2)} : Delta time: {round(delta, 3)}')
+                    print(
+                        f"{os.getpid()} / {round(after, 2)} : Delta time: {round(delta, 3)}"
+                    )
 
                 if command == CommandType.READ_FILE.value:
                     self.execute_read_file(content)
                     command_type = 1
                 elif command == CommandType.PROCESS_JOBS.value:
                     self.execute_process_jobs(content)
                     command_type = 2
                 elif command == CommandType.WRITE_PNTS.value:
-                    self.execute_write_pnts(content)
+                    self.execute_write_pnts(content[2], content[1])
                     command_type = 3
                 elif command == CommandType.SHUTDOWN.value:
                     break  # ack
                 else:
-                    raise NotImplementedError(f'Unknown command {command}')
+                    raise NotImplementedError(f"Unknown command {command!r}")
 
                 # notify we're idle
                 self.skt.send_multipart([ResponseType.IDLE.value])
 
                 if self.activity_graph:
-                    print(f'{before}, {command_type}', file=activity)
-                    print(f'{before}, 0', file=activity)
-                    print(f'{after}, 0', file=activity)
-                    print(f'{after}, {command_type}', file=activity)
+                    print(f"{before}, {command_type}", file=activity)
+                    print(f"{before}, 0", file=activity)
+                    print(f"{after}, 0", file=activity)
+                    print(f"{after}, {command_type}", file=activity)
             except Exception as e:
                 traceback.print_exc()
                 # usually first arg is the explaining string.
                 # let's assume it is always in our context
                 self.skt.send_multipart([ResponseType.ERROR.value, e.args[0].encode()])
                 # we still print it for stacktraces
 
         if self.activity_graph:
             activity.close()
 
         if self.verbosity >= 1:
-            print('total: {} sec, idle: {}'.format(
-                round(time.time() - startup_time, 1),
-                round(idle_time, 1))
+            print(
+                "total: {} sec, idle: {}".format(
+                    round(time.time() - startup_time, 1), round(idle_time, 1)
+                )
             )
 
         self.skt.send_multipart([ResponseType.HALTED.value])
 
-    def execute_read_file(self, content):
+    def execute_read_file(self, content: List[bytes]) -> None:
         parameters = pickle.loads(content[1])
 
-        extension = PurePath(parameters['filename']).suffix
+        extension = PurePath(parameters["filename"]).suffix
         if extension in READER_MAP:
             reader = READER_MAP[extension]
         else:
-            raise ValueError(f"The file with {extension} extension can't be read, "
-                             f"the available extensions are: {READER_MAP.keys()}")
+            raise ValueError(
+                f"The file with {extension} extension can't be read, "
+                f"the available extensions are: {READER_MAP.keys()}"
+            )
 
-        reader.run(
-            parameters['filename'],
-            parameters['offset_scale'],
-            parameters['portion'],
-            self.skt,
-            self.transformer
-        )
-
-    def execute_write_pnts(self, content):
-        pnts_writer.run(self.skt, content[2], content[1], self.folder, self.write_rgb)
-
-    def execute_process_jobs(self, content):
-        node_process.run(
-            content[1:],
-            self.octree_metadata,
-            self.skt,
-            self.verbosity
+        reader_gen = reader.run(
+            parameters["filename"],
+            parameters["offset_scale"],
+            parameters["portion"],
+            self.transformer,
+            self.color_scale,
         )
+        for coords, colors, classification in reader_gen:
+            self.skt.send_multipart(
+                [
+                    ResponseType.NEW_TASK.value,
+                    b"",
+                    pickle.dumps(
+                        {"xyz": coords, "rgb": colors, "classification": classification}
+                    ),
+                    struct.pack(">I", len(coords)),
+                ],
+                copy=False,
+            )
+
+        self.skt.send_multipart([ResponseType.READ.value])
+
+    def execute_write_pnts(self, data: bytes, node_name: bytes) -> None:
+        pnts_writer_gen = pnts_writer.run(
+            data, self.folder, self.write_rgb, self.write_classification
+        )
+        for total in pnts_writer_gen:
+            self.skt.send_multipart(
+                [ResponseType.PNTS_WRITTEN.value, struct.pack(">I", total), node_name]
+            )
+
+    def execute_process_jobs(self, content: List[bytes]) -> None:
+        begin = time.time()
+        log_enabled = self.verbosity >= 2
+        if log_enabled:
+            log_filename = f"py3dtiles-{os.getpid()}.log"
+            log_file = open(log_filename, "a")
+        else:
+            log_file = None
+
+        work = content[1:]
+        i = 0
+        while i < len(work):
+            name = work[i]
+            node = work[i + 1]
+            count = struct.unpack(">I", work[i + 2])[0]
+            tasks = work[i + 3 : i + 3 + count]
+            i += 3 + count
+
+            node_catalog = NodeCatalog(node, name, self.octree_metadata)
+
+            node_process = NodeProcess(
+                node_catalog,
+                self.octree_metadata,
+                name,
+                tasks,
+                begin,
+                log_file,
+            )
+            for proc_name, proc_data, proc_point_count in node_process.run():
+                self.skt.send_multipart(
+                    [
+                        ResponseType.NEW_TASK.value,
+                        proc_name,
+                        proc_data,
+                        struct.pack(">I", proc_point_count),
+                    ],
+                    copy=False,
+                    block=False,
+                )
+
+            if log_enabled:
+                print(f"save on disk {name!r} [{time.time() - begin}]", file=log_file)
+
+            # save node state on disk
+            if len(name) > 0:
+                data = node_catalog.dump(name, node_process.infer_depth_from_name() - 1)
+            else:
+                data = b""
+
+            if log_enabled:
+                print(f"saved on disk [{time.time() - begin}]", file=log_file)
+
+            self.skt.send_multipart(
+                [
+                    ResponseType.PROCESSED.value,
+                    pickle.dumps(
+                        {
+                            "name": name,
+                            "total": node_process.total_point_count,
+                            "data": data,
+                        }
+                    ),
+                ],
+                copy=False,
+            )
+
+        if log_enabled:
+            print(
+                "[<] return result [{} sec] [{}]".format(
+                    round(time.time() - begin, 2), time.time() - begin
+                ),
+                file=log_file,
+                flush=True,
+            )
+            if log_file is not None:
+                log_file.close()
 
 
 # Manager
 class ZmqManager:
     """
     This class sends messages to the workers.
     We can also request general status.
     """
-    def __init__(self, number_of_jobs: int, process_args: tuple):
+
+    def __init__(
+        self,
+        number_of_jobs: int,
+        process_args: Tuple[
+            bool,
+            Optional[Transformer],
+            OctreeMetadata,
+            Path,
+            bool,
+            Optional[float],
+            bool,
+            int,
+        ],
+    ) -> None:
         """
         For the process_args argument, see the init method of Worker
         to get the list of needed parameters.
         """
         self.context = zmq.Context()
 
         self.number_of_jobs = number_of_jobs
 
         self.socket = self.context.socket(zmq.ROUTER)
         self.socket.bind(URI)
         # Useful only when TCP is used to get the URI with the opened port
         self.uri = self.socket.getsockopt(zmq.LAST_ENDPOINT)
+        if not isinstance(self.uri, bytes):
+            raise RuntimeError(
+                "The uri returned by self.socket.getsockopt should be bytes."
+            )
 
         self.processes = [
-            Worker(*process_args, self.uri) # type: ignore
+            Process(target=worker_target, args=(*process_args, self.uri))
             for _ in range(number_of_jobs)
         ]
         for p in self.processes:
             p.start()
 
         self.activities = [p.pid for p in self.processes]
         self.idle_clients: List[bytes] = []
 
         self.killing_processes = False
         self.number_processes_killed = 0
-        self.time_waiting_an_idle_process = 0
+        self.time_waiting_an_idle_process = 0.0
 
-    def send_to_process(self, message):
+    def send_to_process(self, message: List[bytes]) -> None:
         if not self.idle_clients:
             raise ValueError("idle_clients is empty")
-        self.socket.send_multipart([self.idle_clients.pop(), pickle.dumps(time.time())] + message)
+        self.socket.send_multipart(
+            [self.idle_clients.pop(), pickle.dumps(time.time())] + message
+        )
 
-    def send_to_all_idle_processes(self, message):
+    def send_to_all_idle_processes(self, message: List[bytes]) -> None:
         if not self.idle_clients:
             raise ValueError("idle_clients is empty")
         for client in self.idle_clients:
             self.socket.send_multipart([client, pickle.dumps(time.time())] + message)
         self.idle_clients.clear()
 
-    def can_queue_more_jobs(self):
+    def can_queue_more_jobs(self) -> bool:
         return len(self.idle_clients) != 0
 
-    def add_idle_client(self, client_id):
+    def add_idle_client(self, client_id: bytes) -> None:
         if client_id in self.idle_clients:
-            raise ValueError(f"The client id {client_id} is already in idle_clients")
+            raise ValueError(f"The client id {client_id!r} is already in idle_clients")
         self.idle_clients.append(client_id)
 
-    def are_all_processes_idle(self):
+    def are_all_processes_idle(self) -> bool:
         return len(self.idle_clients) == self.number_of_jobs
 
-    def are_all_processes_killed(self):
+    def are_all_processes_killed(self) -> bool:
         return self.number_processes_killed == self.number_of_jobs
 
-    def kill_all_processes(self):
+    def kill_all_processes(self) -> None:
         self.send_to_all_idle_processes([CommandType.SHUTDOWN.value])
         self.killing_processes = True
 
-    def join_all_processes(self):
+    def join_all_processes(self) -> None:
         for p in self.processes:
             p.join()
 
-    def terminate_all_processes(self):
+    def terminate_all_processes(self) -> None:
         for p in self.processes:
             p.terminate()
 
 
-def is_ancestor(node_name, ancestor):
+def is_ancestor(node_name: bytes, ancestor: bytes) -> bool:
     """
     Example, the tile 22 is ancestor of 22458
     Particular case, the tile 22 is ancestor of 22
     """
-    return len(ancestor) <= len(node_name) and node_name[0:len(ancestor)] == ancestor
-
-
-def is_ancestor_in_list(node_name, ancestors):
-    for ancestor in ancestors:
-        if not ancestor or is_ancestor(node_name, ancestor):
-            return True
-    return False
+    return len(ancestor) <= len(node_name) and node_name[0 : len(ancestor)] == ancestor
 
 
-def can_pnts_be_written(node_name, finished_node, input_nodes, active_nodes):
+def is_ancestor_in_list(
+    node_name: bytes, ancestors: Union[List[bytes], Dict[bytes, Any]]
+) -> bool:
+    return any(
+        not ancestor or is_ancestor(node_name, ancestor) for ancestor in ancestors
+    )
+
+
+def can_pnts_be_written(
+    node_name: bytes,
+    finished_node: bytes,
+    input_nodes: Union[List[bytes], Dict[bytes, Any]],
+    active_nodes: Union[List[bytes], Dict[bytes, Any]],
+) -> bool:
     return (
         is_ancestor(node_name, finished_node)
         and not is_ancestor_in_list(node_name, active_nodes)
-        and not is_ancestor_in_list(node_name, input_nodes))
+        and not is_ancestor_in_list(node_name, input_nodes)
+    )
 
 
 class State:
-    def __init__(self, pointcloud_file_portions, max_reading_jobs: int):
+    def __init__(
+        self, pointcloud_file_portions: PortionsType, max_reading_jobs: int
+    ) -> None:
         self.processed_points = 0
         self.max_point_in_progress = 60_000_000
         self.points_in_progress = 0
         self.points_in_pnts = 0
 
         # pointcloud_file_portions is a list of tuple (filename, (start offset, end offset))
         self.point_cloud_file_parts = pointcloud_file_portions
@@ -291,319 +468,406 @@
         # just keep the name of the node.
         # This list will be filled until the writing could be started.
         self.waiting_writing_nodes: List[bytes] = []
         # when the node is writing, its name is moved from waiting_writing_nodes to pnts_to_writing
         # the data to write are stored in a node object.
         self.pnts_to_writing: List[bytes] = []
 
-    def is_reading_finish(self):
+    def is_reading_finish(self) -> bool:
         return not self.point_cloud_file_parts and self.number_of_reading_jobs == 0
 
-    def add_tasks_to_process(self, node_name, data, point_count):
+    def add_tasks_to_process(
+        self, node_name: bytes, data: bytes, point_count: int
+    ) -> None:
         if point_count <= 0:
-            raise ValueError("point_count should be strictly positive, currently", point_count)
+            raise ValueError(
+                "point_count should be strictly positive, currently", point_count
+            )
 
         if node_name not in self.node_to_process:
             self.node_to_process[node_name] = ([data], point_count)
         else:
             tasks, count = self.node_to_process[node_name]
             tasks.append(data)
             self.node_to_process[node_name] = (tasks, count + point_count)
 
-    def can_add_reading_jobs(self):
-        return (
+    def can_add_reading_jobs(self) -> bool:
+        return bool(
             self.point_cloud_file_parts
             and self.points_in_progress < self.max_point_in_progress
             and self.number_of_reading_jobs < self.max_reading_jobs
         )
 
-    def print_debug(self):
-        print('{:^16}|{:^8}|{:^8}|{:^8}'.format('Step', 'Input', 'Active', 'Inactive'))
-        print('{:^16}|{:^8}|{:^8}|{:^8}'.format(
-            'Reader',
-            len(self.point_cloud_file_parts),
-            self.number_of_reading_jobs,
-            ''))
-        print('{:^16}|{:^8}|{:^8}|{:^8}'.format(
-            'Node process',
-            len(self.node_to_process),
-            len(self.processing_nodes),
-            len(self.waiting_writing_nodes)))
-        print('{:^16}|{:^8}|{:^8}|{:^8}'.format(
-            'Pnts writer',
-            len(self.pnts_to_writing),
-            self.number_of_writing_jobs,
-            ''))
+    def print_debug(self) -> None:
+        print("{:^16}|{:^8}|{:^8}|{:^8}".format("Step", "Input", "Active", "Inactive"))
+        print(
+            "{:^16}|{:^8}|{:^8}|{:^8}".format(
+                "Reader",
+                len(self.point_cloud_file_parts),
+                self.number_of_reading_jobs,
+                "",
+            )
+        )
+        print(
+            "{:^16}|{:^8}|{:^8}|{:^8}".format(
+                "Node process",
+                len(self.node_to_process),
+                len(self.processing_nodes),
+                len(self.waiting_writing_nodes),
+            )
+        )
+        print(
+            "{:^16}|{:^8}|{:^8}|{:^8}".format(
+                "Pnts writer",
+                len(self.pnts_to_writing),
+                self.number_of_writing_jobs,
+                "",
+            )
+        )
+
 
-def convert(*args, **kwargs):
+def convert(*args, **kwargs) -> None:  # type: ignore [no-untyped-def] # todo use directly the _Convert class
     converter = _Convert(*args, **kwargs)
     return converter.convert()
 
 
 class _Convert:
-    def __init__(self,
-                 files: Union[List[Union[str, Path]], str, Path],
-                 outfolder: Union[str, Path] = './3dtiles',
-                 overwrite: bool = False,
-                 jobs: int = CPU_COUNT,
-                 cache_size: int = DEFAULT_CACHE_SIZE,
-                 crs_out: Optional[CRS] = None,
-                 crs_in: Optional[CRS] = None,
-                 force_crs_in: bool = False,
-                 fraction: int = 100,
-                 benchmark: Optional[str] = None,
-                 rgb: bool = True,
-                 graph: bool = False,
-                 color_scale: Optional[float] = None,
-                 verbose: bool = False):
+    def __init__(
+        self,
+        files: Union[List[Union[str, Path]], str, Path],
+        outfolder: Union[str, Path] = "./3dtiles",
+        overwrite: bool = False,
+        jobs: int = CPU_COUNT,
+        cache_size: int = DEFAULT_CACHE_SIZE,
+        crs_out: Optional[CRS] = None,
+        crs_in: Optional[CRS] = None,
+        force_crs_in: bool = False,
+        fraction: int = 100,
+        benchmark: Optional[str] = None,
+        rgb: bool = True,
+        classification: bool = True,
+        graph: bool = False,
+        color_scale: Optional[float] = None,
+        verbose: int = False,
+    ) -> None:
         """
         :param files: Filenames to process. The file must use the .las, .laz, .xyz or .ply format.
         :param outfolder: The folder where the resulting tileset will be written.
         :param overwrite: Overwrite the ouput folder if it already exists.
         :param jobs: The number of parallel jobs to start. Default to the number of cpu.
         :param cache_size: Cache size in MB. Default to available memory / 10.
         :param crs_out: CRS to convert the output with
         :param crs_in: Set a default input CRS
         :param force_crs_in: Force every input CRS to be `crs_in`, even if not null
         :param fraction: Percentage of the pointcloud to process, between 0 and 100.
         :param benchmark: Print summary at the end of the process
         :param rgb: Export rgb attributes.
+        :param classification: Export classification attribute.
         :param graph: Produce debug graphs (requires pygal).
-        :param color_scale: Force color scale
+        :param color_scale: Scale the color with the specified amount. Useful to lighten or darken black pointclouds with only intensity.
 
         :raises SrsInMissingException: if py3dtiles couldn't find srs informations in input files and srs_in is not specified
         :raises SrsInMixinException: if the input files have different CRS
 
         """
         self.jobs = jobs
         self.cache_size = cache_size
         self.rgb = rgb
+        self.classification = classification
 
         # allow str directly if only one input
-        files = [files] if isinstance(files, str) or isinstance(files, Path) else files
+        files = [files] if isinstance(files, (str, Path)) else files
         self.files = [Path(file) for file in files]
 
         self.verbose = verbose
         self.graph = graph
         self.benchmark = benchmark
-        self.startup = None
 
-        self.file_info = self.get_file_info(color_scale, crs_in, force_crs_in)
+        self.color_scale = color_scale
+
+        self.file_info = self.get_file_info(crs_in, force_crs_in)
 
         transformer = self.get_transformer(crs_out)
-        self.rotation_matrix, self.original_aabb, self.avg_min = self.get_rotation_matrix(crs_out, transformer)
-        self.root_aabb, self.root_scale, self.root_spacing = self.get_root_aabb(self.original_aabb)
-        octree_metadata = OctreeMetadata(aabb=self.root_aabb, spacing=self.root_spacing, scale=self.root_scale[0])
+        (
+            self.rotation_matrix,
+            self.original_aabb,
+            self.avg_min,
+        ) = self.get_rotation_matrix(crs_out, transformer)
+        self.root_aabb, self.root_scale, self.root_spacing = self.get_root_aabb(
+            self.original_aabb
+        )
+        octree_metadata = OctreeMetadata(
+            aabb=self.root_aabb, spacing=self.root_spacing, scale=self.root_scale[0]
+        )
 
         if self.verbose >= 1:
             self.print_summary()
         if self.graph:
-            self.progression_log = open('progression.csv', 'w')
+            self.progression_log = open("progression.csv", "w")
 
         # create folder
         self.out_folder = Path(outfolder)
         if self.out_folder.is_dir():
             if overwrite:
                 shutil.rmtree(self.out_folder, ignore_errors=True)
             else:
                 raise FileExistsError(f"Folder '{self.out_folder}' already exists")
 
         self.out_folder.mkdir()
         self.working_dir = self.out_folder / "tmp"
         self.working_dir.mkdir(parents=True)
 
-        self.zmq_manager = ZmqManager(self.jobs, (self.graph, transformer, octree_metadata, self.out_folder, self.rgb, self.verbose))
+        self.zmq_manager = ZmqManager(
+            self.jobs,
+            (
+                self.graph,
+                transformer,
+                octree_metadata,
+                self.out_folder,
+                self.rgb,
+                self.color_scale,
+                self.classification,
+                self.verbose,
+            ),
+        )
         self.node_store = SharedNodeStore(self.working_dir)
-        self.state = State(self.file_info['portions'], max(1, self.jobs // 2))
+        self.state = State(self.file_info["portions"], max(1, self.jobs // 2))
 
-    def get_file_info(self, color_scale, crs_in: Optional[CRS], force_crs_in: bool = False) -> dict:
+    def get_file_info(
+        self,
+        crs_in: Optional[CRS],
+        force_crs_in: bool = False,
+    ) -> Dict[str, Any]:
 
         pointcloud_file_portions = []
         aabb = None
-        color_scale_by_file = {}
         total_point_count = 0
-        avg_min = np.array([0., 0., 0.])
+        avg_min = np.array([0.0, 0.0, 0.0])
 
         # read all input files headers and determine the aabb/spacing
         for file in self.files:
             extension = file.suffix
             if extension in READER_MAP:
                 reader = READER_MAP[extension]
             else:
-                raise ValueError(f"The file with {extension} extension can't be read, "
-                                 f"the available extensions are: {READER_MAP.keys()}")
+                raise ValueError(
+                    f"The file with {extension} extension can't be read, "
+                    f"the available extensions are: {READER_MAP.keys()}"
+                )
 
-            file_info = reader.get_metadata(file, color_scale=color_scale)
+            file_info = reader.get_metadata(file)
 
-            pointcloud_file_portions += file_info['portions']
+            pointcloud_file_portions += file_info["portions"]
             if aabb is None:
-                aabb = file_info['aabb']
+                aabb = file_info["aabb"]
             else:
-                aabb[0] = np.minimum(aabb[0], file_info['aabb'][0])
-                aabb[1] = np.maximum(aabb[1], file_info['aabb'][1])
-            color_scale_by_file[str(file)] = file_info['color_scale']
+                aabb[0] = np.minimum(aabb[0], file_info["aabb"][0])
+                aabb[1] = np.maximum(aabb[1], file_info["aabb"][1])
 
-            file_crs_in = str_to_CRS(file_info['srs_in'])
+            file_crs_in = file_info["crs_in"]
             if file_crs_in is not None:
                 if crs_in is None:
                     crs_in = file_crs_in
                 elif crs_in != file_crs_in and not force_crs_in:
-                    raise SrsInMixinException("All input files should have the same srs in, currently there are a mix of"
-                                     f" {crs_in} and {file_crs_in}")
-            total_point_count += file_info['point_count']
-            avg_min += file_info['avg_min'] / len(self.files)
-
+                    raise SrsInMixinException(
+                        "All input files should have the same srs in, currently there are a mix of"
+                        f" {crs_in} and {file_crs_in}"
+                    )
+            total_point_count += file_info["point_count"]
+            avg_min += file_info["avg_min"] / len(self.files)
+
+        # The fact self.files is not empty have been checked before, so this shouldn't happen
+        # but this keeps mypy happy and also serve as "defensive programming"
+        if aabb is None:
+            raise RuntimeError("No aabb could be computed!")
+        # correct aabb, so that we don't have null sized box
+        # we add 10^-5, supposing it's reasonable for most use case
+        make_aabb_valid(aabb)
         return {
-            'portions': pointcloud_file_portions,
-            'aabb': aabb,
-            'color_scale': color_scale_by_file,
-            'crs_in': crs_in,
-            'point_count': total_point_count,
-            'avg_min': avg_min
+            "portions": pointcloud_file_portions,
+            "aabb": aabb,
+            "crs_in": crs_in,
+            "point_count": total_point_count,
+            "avg_min": avg_min,
         }
 
-    def get_transformer(self, crs_out: Optional[CRS]) -> Union[Transformer, None]:
+    def get_transformer(self, crs_out: Optional[CRS]) -> Optional[Transformer]:
         if crs_out:
-            if self.file_info['crs_in'] is None:
-                raise SrsInMissingException("None file has a input srs specified. Should be provided.")
+            if self.file_info["crs_in"] is None:
+                raise SrsInMissingException(
+                    "None file has a input srs specified. Should be provided."
+                )
 
-            transformer = Transformer.from_crs(self.file_info['crs_in'], crs_out)
+            transformer = Transformer.from_crs(self.file_info["crs_in"], crs_out)
         else:
             transformer = None
 
         return transformer
 
-    def get_rotation_matrix(self, crs_out, transformer):
-        avg_min = self.file_info['avg_min']
-        aabb = self.file_info['aabb']
+    def get_rotation_matrix(
+        self, crs_out: Optional[CRS], transformer: Optional[Transformer]
+    ) -> Tuple[
+        npt.NDArray[np.float64], npt.NDArray[np.float64], npt.NDArray[np.float64]
+    ]:
+        avg_min: npt.NDArray[np.float64] = self.file_info["avg_min"]
+        aabb: npt.NDArray[np.float64] = self.file_info["aabb"]
 
-        rotation_matrix = None
-        if crs_out:
+        rotation_matrix: npt.NDArray[np.float64] = np.identity(4)
+        if crs_out is not None and transformer is not None:
 
-            bl = np.array(list(transformer.transform(
-                aabb[0][0], aabb[0][1], aabb[0][2])))
-            tr = np.array(list(transformer.transform(
-                aabb[1][0], aabb[1][1], aabb[1][2])))
-            br = np.array(list(transformer.transform(
-                aabb[1][0], aabb[0][1], aabb[0][2])))
+            bl: npt.NDArray[np.float64] = np.array(
+                list(transformer.transform(aabb[0][0], aabb[0][1], aabb[0][2]))
+            )
+            tr: npt.NDArray[np.float64] = np.array(
+                list(transformer.transform(aabb[1][0], aabb[1][1], aabb[1][2]))
+            )
+            br: npt.NDArray[np.float64] = np.array(
+                list(transformer.transform(aabb[1][0], aabb[0][1], aabb[0][2]))
+            )
 
-            avg_min = np.array(list(transformer.transform(
-                avg_min[0], avg_min[1], avg_min[2])))
+            avg_min = np.array(
+                list(transformer.transform(avg_min[0], avg_min[1], avg_min[2]))
+            )
 
             x_axis = br - bl
 
             bl = bl - avg_min
             tr = tr - avg_min
 
             if crs_out.to_epsg() == 4978:
                 # Transform geocentric normal => (0, 0, 1)
                 # and 4978-bbox x axis => (1, 0, 0),
                 # to have a bbox in local coordinates that's nicely aligned with the data
                 rotation_matrix = make_rotation_matrix(avg_min, np.array([0, 0, 1]))
                 rotation_matrix = np.dot(
-                    make_rotation_matrix(x_axis, np.array([1, 0, 0])),
-                    rotation_matrix)
+                    make_rotation_matrix(x_axis, np.array([1, 0, 0])), rotation_matrix
+                )
 
-                bl = np.dot(bl, rotation_matrix[:3, :3].T)
-                tr = np.dot(tr, rotation_matrix[:3, :3].T)
+                rotation_matrix_part = rotation_matrix[:3, :3].T
 
-            root_aabb = np.array([
-                np.minimum(bl, tr),
-                np.maximum(bl, tr)
-            ])
+                bl = np.dot(bl, rotation_matrix_part)
+                tr = np.dot(tr, rotation_matrix_part)
+
+            root_aabb = np.array([np.minimum(bl, tr), np.maximum(bl, tr)])
         else:
             # offset
             root_aabb = aabb - avg_min
 
         return rotation_matrix, root_aabb, avg_min
 
-    def get_root_aabb(self, original_aabb):
+    def get_root_aabb(
+        self, original_aabb: npt.NDArray[np.float64]
+    ) -> Tuple[npt.NDArray[np.float64], npt.NDArray[np.float32], float]:
         base_spacing = compute_spacing(original_aabb)
         if base_spacing > 10:
             root_scale = np.array([0.01, 0.01, 0.01])
         elif base_spacing > 1:
             root_scale = np.array([0.1, 0.1, 0.1])
         else:
             root_scale = np.array([1, 1, 1])
 
         root_aabb = original_aabb * root_scale
         root_spacing = compute_spacing(root_aabb)
         return root_aabb, root_scale, root_spacing
 
-    def convert(self):
+    def convert(self) -> None:
         """convert
 
         Convert pointclouds (xyz, las or laz) to 3dtiles tileset containing pnts node
         """
-        self.startup = time.time()
+        startup: float = time.time()
 
         try:
             while not self.zmq_manager.killing_processes:
-                now = time.time() - self.startup
+                now = time.time() - startup
 
                 at_least_one_job_ended = False
-                if not self.zmq_manager.can_queue_more_jobs() or self.zmq_manager.socket.poll(timeout=0, flags=zmq.POLLIN):
+                if (
+                    not self.zmq_manager.can_queue_more_jobs()
+                    or self.zmq_manager.socket.poll(timeout=0, flags=zmq.POLLIN)
+                ):
                     at_least_one_job_ended = self.process_message()
 
-                while self.state.pnts_to_writing and self.zmq_manager.can_queue_more_jobs():
+                while (
+                    self.state.pnts_to_writing
+                    and self.zmq_manager.can_queue_more_jobs()
+                ):
                     self.send_pnts_to_write()
 
                 if self.zmq_manager.can_queue_more_jobs():
                     self.send_points_to_process(now)
 
-                while self.state.can_add_reading_jobs() and self.zmq_manager.can_queue_more_jobs():
+                while (
+                    self.state.can_add_reading_jobs()
+                    and self.zmq_manager.can_queue_more_jobs()
+                ):
                     self.send_file_to_read()
 
                 # if at this point we have no work in progress => we're done
                 if self.zmq_manager.are_all_processes_idle():
                     self.zmq_manager.kill_all_processes()
 
                 if at_least_one_job_ended:
                     self.print_debug(now)
                     if self.graph:
-                        percent = round(100 * self.state.processed_points / self.file_info['point_count'], 3)
-                        print(f'{time.time() - self.startup}, {percent}', file=self.progression_log)
+                        percent = round(
+                            100
+                            * self.state.processed_points
+                            / self.file_info["point_count"],
+                            3,
+                        )
+                        print(
+                            f"{time.time() - startup}, {percent}",
+                            file=self.progression_log,
+                        )
 
                 self.node_store.control_memory_usage(self.cache_size, self.verbose)
 
             self.zmq_manager.join_all_processes()
 
-            if self.state.points_in_pnts != self.file_info['point_count']:
-                raise ValueError("!!! Invalid point count in the written .pnts"
-                                 + f"(expected: {self.file_info['point_count']}, was: {self.state.points_in_pnts})")
+            if self.state.points_in_pnts != self.file_info["point_count"]:
+                raise ValueError(
+                    "!!! Invalid point count in the written .pnts"
+                    + f"(expected: {self.file_info['point_count']}, was: {self.state.points_in_pnts})"
+                )
 
             if self.verbose >= 1:
-                print('Writing 3dtiles {}'.format(self.file_info['avg_min']))
+                print("Writing 3dtiles {}".format(self.file_info["avg_min"]))
 
             self.write_tileset()
             shutil.rmtree(self.working_dir)
 
             if self.verbose >= 1:
-                print('Done')
+                print("Done")
 
             if self.benchmark:
-                print('{},{},{},{}'.format(
-                    self.benchmark,
-                    ','.join([f.name for f in self.files]),
-                    self.state.points_in_pnts,
-                    round(time.time() - self.startup, 1)))
+                print(
+                    "{},{},{},{}".format(
+                        self.benchmark,
+                        ",".join([f.name for f in self.files]),
+                        self.state.points_in_pnts,
+                        round(time.time() - startup, 1),
+                    )
+                )
         finally:
             self.zmq_manager.terminate_all_processes()
 
             if self.verbose >= 1:
-                print('destroy', round(self.zmq_manager.time_waiting_an_idle_process, 2))
+                print(
+                    "destroy", round(self.zmq_manager.time_waiting_an_idle_process, 2)
+                )
 
             # pygal chart
             if self.graph:
                 self.progression_log.close()
                 self.draw_graph()
 
             self.zmq_manager.context.destroy()
 
-    def process_message(self):
+    def process_message(self) -> bool:
         one_job_ended = False
 
         # Blocking read but it's fine because either all our child processes are busy
         # or we know that there's something to read (zmq.POLLIN)
         start = time.time()
         message = self.zmq_manager.socket.recv_multipart()
 
@@ -622,349 +886,457 @@
 
         elif return_type == ResponseType.READ.value:
             self.state.number_of_reading_jobs -= 1
             one_job_ended = True
 
         elif return_type == ResponseType.PROCESSED.value:
             content = pickle.loads(result[-1])
-            self.state.processed_points += content['total']
-            self.state.points_in_progress -= content['total']
+            self.state.processed_points += content["total"]
+            self.state.points_in_progress -= content["total"]
 
-            del self.state.processing_nodes[content['name']]
+            del self.state.processing_nodes[content["name"]]
 
             self.dispatch_processed_nodes(content)
 
             one_job_ended = True
 
         elif return_type == ResponseType.PNTS_WRITTEN.value:
-            self.state.points_in_pnts += struct.unpack('>I', result[1])[0]
+            self.state.points_in_pnts += struct.unpack(">I", result[1])[0]
             self.state.number_of_writing_jobs -= 1
 
         elif return_type == ResponseType.NEW_TASK.value:
             self.state.add_tasks_to_process(
-                node_name=result[1], data=result[2], point_count=struct.unpack('>I', result[3])[0]
+                node_name=result[1],
+                data=result[2],
+                point_count=struct.unpack(">I", result[3])[0],
             )
 
         elif return_type == ResponseType.ERROR.value:
-            raise WorkerException(f'An exception occurred in a worker: {result[1].decode()}')
+            raise WorkerException(
+                f"An exception occurred in a worker: {result[1].decode()}"
+            )
 
         else:
-            raise NotImplementedError(f"The command {return_type} is not implemented")
+            raise NotImplementedError(f"The command {return_type!r} is not implemented")
 
         return one_job_ended
 
-    def dispatch_processed_nodes(self, content):
-        if not content['name']:
+    def dispatch_processed_nodes(self, content: Dict[str, bytes]) -> None:
+        if not content["name"]:
             return
 
-        self.node_store.put(content['name'], content['save'])
-        self.state.waiting_writing_nodes.append(content['name'])
+        self.node_store.put(content["name"], content["data"])
+        self.state.waiting_writing_nodes.append(content["name"])
 
         if not self.state.is_reading_finish():
             return
 
         # if all nodes aren't processed yet,
         # we should check if linked ancestors are processed
         if self.state.processing_nodes or self.state.node_to_process:
-            finished_node = content['name']
+            finished_node = content["name"]
             if can_pnts_be_written(
-                finished_node, finished_node,
-                self.state.node_to_process, self.state.processing_nodes
+                finished_node,
+                finished_node,
+                self.state.node_to_process,
+                self.state.processing_nodes,
             ):
                 self.state.waiting_writing_nodes.pop(-1)
                 self.state.pnts_to_writing.append(finished_node)
 
                 for i in range(len(self.state.waiting_writing_nodes) - 1, -1, -1):
                     candidate = self.state.waiting_writing_nodes[i]
 
                     if can_pnts_be_written(
-                        candidate, finished_node,
-                        self.state.node_to_process, self.state.processing_nodes
+                        candidate,
+                        finished_node,
+                        self.state.node_to_process,
+                        self.state.processing_nodes,
                     ):
                         self.state.waiting_writing_nodes.pop(i)
                         self.state.pnts_to_writing.append(candidate)
 
         else:
             for c in self.state.waiting_writing_nodes:
                 self.state.pnts_to_writing.append(c)
             self.state.waiting_writing_nodes.clear()
 
-    def send_pnts_to_write(self):
+    def send_pnts_to_write(self) -> None:
         node_name = self.state.pnts_to_writing.pop()
         data = self.node_store.get(node_name)
         if not data:
-            raise ValueError(f'{node_name} has no data')
+            raise ValueError(f"{node_name!r} has no data")
 
-        self.zmq_manager.send_to_process([CommandType.WRITE_PNTS.value, node_name, data])
+        self.zmq_manager.send_to_process(
+            [CommandType.WRITE_PNTS.value, node_name, data]
+        )
         self.node_store.remove(node_name)
         self.state.number_of_writing_jobs += 1
 
-    def send_points_to_process(self, now):
+    def send_points_to_process(self, now: float) -> None:
         potentials = sorted(
             # a key (=task) can be in node_to_process and processing_nodes if the node isn't completely processed
             [
-                (node, task) for node, task in self.state.node_to_process.items()  # task: [data...], point_count
+                (node, task)
+                for node, task in self.state.node_to_process.items()  # task: [data...], point_count
                 if node not in self.state.processing_nodes
             ],
-            key=lambda task: -len(task[0]))  # sort by node name size, the root nodes first
+            key=lambda task: -len(task[0]),
+        )  # sort by node name size, the root nodes first
 
         while self.zmq_manager.can_queue_more_jobs() and potentials:
             target_count = 100_000
             job_list = []
             count = 0
             idx = len(potentials) - 1
             while count < target_count and idx >= 0:
                 name, (tasks, point_count) = potentials[idx]
                 count += point_count
                 job_list += [
                     name,
                     self.node_store.get(name),
-                    struct.pack('>I', len(tasks)),
+                    struct.pack(">I", len(tasks)),
                 ] + tasks
                 del potentials[idx]
 
                 del self.state.node_to_process[name]
                 self.state.processing_nodes[name] = (len(tasks), point_count, now)
 
                 if name in self.state.waiting_writing_nodes:
-                    self.state.waiting_writing_nodes.pop(self.state.waiting_writing_nodes.index(name))
+                    self.state.waiting_writing_nodes.pop(
+                        self.state.waiting_writing_nodes.index(name)
+                    )
                 idx -= 1
 
             if job_list:
-                self.zmq_manager.send_to_process([CommandType.PROCESS_JOBS.value] + job_list)
+                self.zmq_manager.send_to_process(
+                    [CommandType.PROCESS_JOBS.value] + job_list
+                )
 
-    def send_file_to_read(self):
+    def send_file_to_read(self) -> None:
         if self.verbose >= 1:
-            print(f'Submit next portion {self.state.point_cloud_file_parts[-1]}')
+            print(f"Submit next portion {self.state.point_cloud_file_parts[-1]}")
         file, portion = self.state.point_cloud_file_parts.pop()
         self.state.points_in_progress += portion[1] - portion[0]
 
-        self.zmq_manager.send_to_process([CommandType.READ_FILE.value, pickle.dumps({
-            'filename': file,
-            'offset_scale': (
-                -self.avg_min,
-                self.root_scale,
-                self.rotation_matrix[:3, :3].T if self.rotation_matrix is not None else None,
-                self.file_info['color_scale'].get(file) if self.file_info['color_scale'] is not None else None,
-            ),
-            'portion': portion,
-        })])
+        self.zmq_manager.send_to_process(
+            [
+                CommandType.READ_FILE.value,
+                pickle.dumps(
+                    {
+                        "filename": file,
+                        "offset_scale": (
+                            -self.avg_min,
+                            self.root_scale,
+                            self.rotation_matrix[:3, :3].T,
+                        ),
+                        "portion": portion,
+                    }
+                ),
+            ]
+        )
 
         self.state.number_of_reading_jobs += 1
 
-    def write_tileset(self):
+    def write_tileset(self) -> None:
         # compute tile transform matrix
-        if self.rotation_matrix is None:
-            transform = np.identity(4)
-        else:
-            transform = np.linalg.inv(self.rotation_matrix)
+        transform = np.linalg.inv(self.rotation_matrix)
         transform = np.dot(transform, make_scale_matrix(1.0 / self.root_scale[0]))
         transform = np.dot(make_translation_matrix(self.avg_min), transform)
 
         # Create the root tile by sampling (or taking all points?) of child nodes
-        root_node = Node(b'', self.root_aabb, self.root_spacing * 2)
+        root_node = Node(b"", self.root_aabb, self.root_spacing * 2)
         root_node.children = []
-        inv_aabb_size = (1.0 / np.maximum(MIN_POINT_SIZE, self.root_aabb[1] - self.root_aabb[0])).astype(
-            np.float32)
-        for child in range(8):
-            tile_path = node_name_to_path(self.out_folder, str(child).encode('ascii'), '.pnts')
+        inv_aabb_size = (
+            1.0 / np.maximum(MIN_POINT_SIZE, self.root_aabb[1] - self.root_aabb[0])
+        ).astype(np.float32)
+        for child_num in range(8):
+            tile_path = node_name_to_path(
+                self.out_folder, str(child_num).encode("ascii"), ".pnts"
+            )
             if tile_path.exists():
-                tile_content = TileContentReader.read_file(tile_path)
+                tile_content = read_binary_tile_content(tile_path)
 
                 fth = tile_content.body.feature_table.header
-                xyz = tile_content.body.feature_table.body.positions_arr.view(np.float32).reshape(
-                    (fth.points_length, 3))
+                xyz = tile_content.body.feature_table.body.position.view(
+                    np.float32
+                ).reshape((fth.points_length, 3))
                 if self.rgb:
-                    rgb = tile_content.body.feature_table.body.colors_arr.reshape((fth.points_length, 3))
+                    tile_color = tile_content.body.feature_table.body.color
+                    if tile_color is None:
+                        raise TilerException(
+                            "tile_content.body.feature_table.body.color shouldn't be None here. Seems to be a py3dtiles issue."
+                        )
+                    if tile_color.dtype != np.uint8:
+                        raise TilerException(
+                            "The data type of tile_content.body.feature_table.body.color must be np.uint8. Seems to be a py3dtiles issue."
+                        )
+                    rgb = tile_color.reshape((fth.points_length, 3)).astype(
+                        np.uint8, copy=False
+                    )  # the astype is used for typing
                 else:
                     rgb = np.zeros(xyz.shape, dtype=np.uint8)
-
+                if self.classification:
+                    classification = (
+                        tile_content.body.batch_table.get_binary_property(
+                            "Classification"
+                        )
+                        .astype(np.uint8)
+                        .reshape(-1, 1)
+                    )
+                else:
+                    classification = np.zeros((fth.points_length, 1), dtype=np.uint8)
                 root_node.grid.insert(
                     self.root_aabb[0].astype(np.float32),
                     inv_aabb_size,
                     xyz.copy(),
-                    rgb)
+                    rgb,
+                    classification,
+                )
 
-        pnts_writer.node_to_pnts(b'', root_node, self.out_folder, self.rgb)
+        pnts_writer.node_to_pnts(
+            b"", root_node, self.out_folder, self.rgb, self.classification
+        )
 
-        executor = concurrent.futures.ProcessPoolExecutor()
-        root_tileset = Node.to_tileset(executor, b'', self.root_aabb, self.root_spacing,
-                                       self.out_folder, self.root_scale, prune=False)
-        executor.shutdown()
+        pool_executor = concurrent.futures.ProcessPoolExecutor()
+        root_tileset = node_from_name(
+            b"", self.root_aabb, self.root_spacing
+        ).to_tileset(self.out_folder, self.root_scale, None, 0, pool_executor)
+        pool_executor.shutdown()
+
+        if root_tileset is None:
+            raise RuntimeError(
+                "root_tileset cannot be None here. This is likely a tiler bug."
+            )
 
-        root_tileset['transform'] = transform.T.reshape(16).tolist()
-        root_tileset['refine'] = 'REPLACE'  # The root tile is in the "REPLACE" refine mode
+        root_tileset["transform"] = transform.T.reshape(16).tolist()
+        root_tileset[
+            "refine"
+        ] = "REPLACE"  # The root tile is in the "REPLACE" refine mode
         if "children" in root_tileset:
             # And children with the "ADD" refine mode
             # No need to set this property in their children, they will take the parent value if it is not present
-            for child in root_tileset['children']:
-                child['refine'] = 'ADD'  # type: ignore
+            for child in root_tileset["children"]:
+                child["refine"] = "ADD"
 
+        geometric_error = (
+            np.linalg.norm(self.root_aabb[1] - self.root_aabb[0]) / self.root_scale[0]
+        )
         tileset = {
-            'asset': {
-                'version': '1.0',
+            "asset": {
+                "version": "1.0",
             },
-            'geometricError': np.linalg.norm(
-                self.root_aabb[1] - self.root_aabb[0]) / self.root_scale[0],
-            'root': root_tileset,
+            "geometricError": geometric_error,
+            "root": root_tileset,
         }
 
         tileset_path = self.out_folder / "tileset.json"
-        with tileset_path.open('w') as f:
+        with tileset_path.open("w") as f:
             f.write(json.dumps(tileset))
 
-    def print_summary(self):
-        print('Summary:')
-        print('  - points to process: {}'.format(self.file_info['point_count']))
-        print(f'  - offset to use: {self.avg_min}')
-        print(f'  - root spacing: {self.root_spacing / self.root_scale[0]}')
-        print(f'  - root aabb: {self.root_aabb}')
-        print(f'  - original aabb: {self.original_aabb}')
-        print(f'  - scale: {self.root_scale}')
+    def print_summary(self) -> None:
+        print("Summary:")
+        print("  - points to process: {}".format(self.file_info["point_count"]))
+        print(f"  - offset to use: {self.avg_min}")
+        print(f"  - root spacing: {self.root_spacing / self.root_scale[0]}")
+        print(f"  - root aabb: {self.root_aabb}")
+        print(f"  - original aabb: {self.original_aabb}")
+        print(f"  - scale: {self.root_scale}")
 
-    def draw_graph(self):
-        import pygal  # type: ignore
+    def draw_graph(self) -> None:
+        import pygal
 
         dateline = pygal.XY(x_label_rotation=25, secondary_range=(0, 100))
         for pid in self.zmq_manager.activities:
             activity = []
-            activity_csv_path = Path(f'activity.{pid}.csv')
-            i = len(self.zmq_manager.activities) - self.zmq_manager.activities.index(pid) - 1
+            activity_csv_path = Path(f"activity.{pid}.csv")
+            i = (
+                len(self.zmq_manager.activities)
+                - self.zmq_manager.activities.index(pid)
+                - 1
+            )
             # activities.index(pid) =
             with activity_csv_path.open() as f:
-                content = f.read().split('\n')
+                content = f.read().split("\n")
                 for line in content[1:]:
-                    line = line.split(',')
-                    if line[0]:
-                        ts = float(line[0])
-                        value = int(line[1]) / 3.0
+                    line_item = line.split(",")
+                    if line_item[0]:
+                        ts = float(line_item[0])
+                        value = int(line_item[1]) / 3.0
                         activity.append((ts, i + value * 0.9))
 
             activity_csv_path.unlink()
             if activity:
                 activity.append((activity[-1][0], activity[0][1]))
                 activity.append(activity[0])
                 dateline.add(str(pid), activity, show_dots=False, fill=True)
 
-        progression_csv_path = Path('progression.csv')
+        progression_csv_path = Path("progression.csv")
         with progression_csv_path.open() as f:
             values = []
-            for line in f.read().split('\n'):
+            for line in f.read().split("\n"):
                 if line:
-                    line = line.split(',')
-                    values += [(float(line[0]), float(line[1]))]
+                    line_item = line.split(",")
+                    values += [(float(line_item[0]), float(line_item[1]))]
         progression_csv_path.unlink()
-        dateline.add('progression', values, show_dots=False, secondary=True,
-                     stroke_style={'width': 2, 'color': 'black'})
+        dateline.add(
+            "progression",
+            values,
+            show_dots=False,
+            secondary=True,
+            stroke_style={"width": 2, "color": "black"},
+        )
 
-        dateline.render_to_file('activity.svg')
+        dateline.render_to_file("activity.svg")
 
-    def print_debug(self, now):
+    def print_debug(self, now: float) -> None:
         if self.verbose >= 3:
-            print('{:^16}|{:^8}|{:^8}'.format('Name', 'Points', 'Seconds'))
+            print("{:^16}|{:^8}|{:^8}".format("Name", "Points", "Seconds"))
             for name, v in self.state.processing_nodes.items():
-                print('{:^16}|{:^8}|{:^8}'.format(
-                    '{} ({})'.format(name.decode('ascii'), v[0]),
-                    v[1],
-                    round(now - v[2], 1)))
-            print('')
-            print('Pending:')
-            print('  - root: {} / {}'.format(
-                len(self.state.point_cloud_file_parts),
-                self.state.initial_portion_count))
-            print('  - other: {} files for {} nodes'.format(
-                sum([len(f[0]) for f in self.state.node_to_process.values()]),
-                len(self.state.node_to_process)))
-            print('')
+                print(
+                    "{:^16}|{:^8}|{:^8}".format(
+                        "{} ({})".format(name.decode("ascii"), v[0]),
+                        v[1],
+                        round(now - v[2], 1),
+                    )
+                )
+            print("")
+            print("Pending:")
+            print(
+                "  - root: {} / {}".format(
+                    len(self.state.point_cloud_file_parts),
+                    self.state.initial_portion_count,
+                )
+            )
+            print(
+                "  - other: {} files for {} nodes".format(
+                    sum([len(f[0]) for f in self.state.node_to_process.values()]),
+                    len(self.state.node_to_process),
+                )
+            )
+            print("")
 
         elif self.verbose >= 2:
             self.state.print_debug()
 
         if self.verbose >= 1:
-            print('{} % points in {} sec [{} tasks, {} nodes, {} wip]'.format(
-                round(100 * self.state.processed_points / self.file_info['point_count'], 2),
-                round(now, 1),
-                self.jobs - len(self.zmq_manager.idle_clients),
-                len(self.state.processing_nodes),
-                self.state.points_in_progress))
+            print(
+                "{} % points in {} sec [{} tasks, {} nodes, {} wip]".format(
+                    round(
+                        100
+                        * self.state.processed_points
+                        / self.file_info["point_count"],
+                        2,
+                    ),
+                    round(now, 1),
+                    self.jobs - len(self.zmq_manager.idle_clients),
+                    len(self.state.processing_nodes),
+                    self.state.points_in_progress,
+                )
+            )
 
         elif self.verbose >= 0:
-            percent = round(100 * self.state.processed_points / self.file_info['point_count'], 2)
+            percent = round(
+                100 * self.state.processed_points / self.file_info["point_count"], 2
+            )
             time_left = (100 - percent) * now / (percent + 0.001)
-            print(f'\r{percent:>6} % in {round(now)} sec [est. time left: {round(time_left)} sec]', end='',
-                  flush=True)
+            print(
+                f"\r{percent:>6} % in {round(now)} sec [est. time left: {round(time_left)} sec]      ",
+                end="",
+                flush=True,
+            )
 
 
-def init_parser(subparser):
-    parser = subparser.add_parser(
-        'convert',
-        help='Convert input 3D data to a 3dtiles tileset.',
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+def init_parser(
+    subparser: "argparse._SubParsersAction[Any]",
+) -> argparse.ArgumentParser:
+    parser: argparse.ArgumentParser = subparser.add_parser(
+        "convert",
+        help="Convert input 3D data to a 3dtiles tileset.",
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+    )
     parser.add_argument(
-        'files',
-        nargs='+',
-        help='Filenames to process. The file must use the .las, .laz (lastools must be installed), .xyz or .ply format.')
+        "files",
+        nargs="+",
+        help="Filenames to process. The file must use the .las, .laz (lastools must be installed), .xyz or .ply format.",
+    )
     parser.add_argument(
-        '--out',
+        "--out",
         type=str,
-        help='The folder where the resulting tileset will be written.',
-        default='./3dtiles')
+        help="The folder where the resulting tileset will be written.",
+        default="./3dtiles",
+    )
     parser.add_argument(
-        '--overwrite',
-        help='Delete and recreate the ouput folder if it already exists. WARNING: be careful, there will be no confirmation!',
-        action='store_true')
+        "--overwrite",
+        help="Delete and recreate the ouput folder if it already exists. WARNING: be careful, there will be no confirmation!",
+        action="store_true",
+    )
     parser.add_argument(
-        '--jobs',
-        help='The number of parallel jobs to start. Default to the number of cpu.',
+        "--jobs",
+        help="The number of parallel jobs to start. Default to the number of cpu.",
         default=cpu_count(),
-        type=int)
+        type=int,
+    )
     parser.add_argument(
-        '--cache_size',
-        help='Cache size in MB. Default to available memory / 10.',
+        "--cache_size",
+        help="Cache size in MB. Default to available memory / 10.",
         default=int(TOTAL_MEMORY_MB / 10),
-        type=int)
+        type=int,
+    )
     parser.add_argument(
-        '--srs_out', help='SRS to convert the output with (numeric part of the EPSG code)', type=str)
+        "--srs_out",
+        help="SRS to convert the output with (numeric part of the EPSG code)",
+        type=str,
+    )
     parser.add_argument(
-        '--srs_in', help='Override input SRS (numeric part of the EPSG code)', type=str)
+        "--srs_in", help="Override input SRS (numeric part of the EPSG code)", type=str
+    )
     parser.add_argument(
-        '--fraction',
-        help='Percentage of the pointcloud to process.',
-        default=100, type=int)
+        "--fraction",
+        help="Percentage of the pointcloud to process.",
+        default=100,
+        type=int,
+    )
     parser.add_argument(
-        '--benchmark',
-        help='Print summary at the end of the process', type=str)
+        "--benchmark", help="Print summary at the end of the process", type=str
+    )
     parser.add_argument(
-        '--no-rgb',
-        help="Don't export rgb attributes", action='store_true')
+        "--no-rgb", help="Don't export rgb attributes", action="store_true"
+    )
     parser.add_argument(
-        '--graph',
-        help='Produce debug graphes (requires pygal)', action='store_true')
+        "--classification", help="Export classification attributes", action="store_true"
+    )
     parser.add_argument(
-        '--color_scale',
-        help='Force color scale', type=float)
+        "--graph", help="Produce debug graphes (requires pygal)", action="store_true"
+    )
+    parser.add_argument("--color_scale", help="Force color scale", type=float)
     parser.add_argument(
-        '--force-srs-in',
-        help='Force the input srs even if the srs in the input files are different. CAUTION, use only if you know what you are doing.', action='store_true')
+        "--force-srs-in",
+        help="Force the input srs even if the srs in the input files are different. CAUTION, use only if you know what you are doing.",
+        action="store_true",
+    )
 
     return parser
 
 
-def main(args):
+def main(args: argparse.Namespace) -> None:
     try:
-        return convert(args.files,
-                       outfolder=args.out,
-                       overwrite=args.overwrite,
-                       jobs=args.jobs,
-                       cache_size=args.cache_size,
-                       crs_out=str_to_CRS(args.srs_out),
-                       crs_in=str_to_CRS(args.srs_in),
-                       force_crs_in=args.force_srs_in,
-                       fraction=args.fraction,
-                       benchmark=args.benchmark,
-                       rgb=not args.no_rgb,
-                       graph=args.graph,
-                       color_scale=args.color_scale,
-                       verbose=args.verbose)
+        return convert(
+            args.files,
+            outfolder=args.out,
+            overwrite=args.overwrite,
+            jobs=args.jobs,
+            cache_size=args.cache_size,
+            crs_out=str_to_CRS(args.srs_out),
+            crs_in=str_to_CRS(args.srs_in),
+            force_crs_in=args.force_srs_in,
+            fraction=args.fraction,
+            benchmark=args.benchmark,
+            rgb=not args.no_rgb,
+            classification=args.classification,
+            graph=args.graph,
+            color_scale=args.color_scale,
+            verbose=args.verbose,
+        )
     except SrsInMissingException:
-        print('No SRS information in input files, you should specify it with --srs_in')
+        print("No SRS information in input files, you should specify it with --srs_in")
         sys.exit(1)
```

### Comparing `py3dtiles-5.0.0/py3dtiles/exceptions.py` & `py3dtiles-6.0.0/py3dtiles/exceptions.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,15 +2,21 @@
     """
     All exceptions thrown by py3dtiles code derives this class.
 
     Client code that wishes to catch all py3dtiles exception can use `except Py3dtilesException`.
     """
 
 
-class WorkerException(Py3dtilesException):
+class TilerException(Py3dtilesException):
+    """
+    This exception will be thrown when there is an issue during a tiling task.
+    """
+
+
+class WorkerException(TilerException):
     """
     This exception will be thrown by the conversion code if one exception occurs inside a worker.
     """
 
 
 class SrsInMissingException(Py3dtilesException):
     """
@@ -18,7 +24,37 @@
     """
 
 
 class SrsInMixinException(Py3dtilesException):
     """
     This exception will be thrown when among all input files, there is a mix of input srs.
     """
+
+
+class Invalid3dtilesError(Py3dtilesException):
+    """
+    This exception will be thrown if the 3d tile specification isn't respected.
+    """
+
+
+class InvalidPntsError(Invalid3dtilesError):
+    """
+    This exception will be thrown if the point cloud format isn't respected.
+    """
+
+
+class InvalidB3dmError(Invalid3dtilesError):
+    """
+    This exception will be thrown if the batched 3D model format isn't respected.
+    """
+
+
+class InvalidTilesetError(Invalid3dtilesError):
+    """
+    This exception will be thrown if the tileset format isn't respected.
+    """
+
+
+class BoundingVolumeMissingException(InvalidTilesetError):
+    """
+    This exception will be thrown when a bounding volume is needed but not present.
+    """
```

### Comparing `py3dtiles-5.0.0/py3dtiles/export.py` & `py3dtiles-6.0.0/py3dtiles/export.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,40 @@
+import argparse
 import errno
 import getpass
 import json
 import math
 import os
+from typing import Any
 
 import numpy as np
 import psycopg2
 
 from py3dtiles.tilers.b3dm.wkb_utils import TriangleSoup
-from py3dtiles.tileset.batch_table import BatchTable
 from py3dtiles.tileset.content import B3dm, GlTF
+from py3dtiles.tileset.content.batch_table import BatchTable
 
 
 class BoundingBox:
     def __init__(self, minimum, maximum):
         self.min = [float(i) for i in minimum]
         self.max = [float(i) for i in maximum]
 
     def inside(self, point):
-        return ((self.min[0] <= point[0] < self.max[0])
-                and (self.min[1] <= point[1] < self.max[1]))
+        return all(self.min[idx] <= point[idx] < self.max[idx] for idx in (0, 1))
 
     def center(self):
         return [(i + j) / 2 for (i, j) in zip(self.min, self.max)]
 
     def add(self, box):
         self.min = [min(i, j) for (i, j) in zip(self.min, box.min)]
         self.max = [max(i, j) for (i, j) in zip(self.max, box.max)]
 
 
-class Feature():
+class Feature:
     def __init__(self, index, box):
         self.index = index
         self.box = box
 
 
 class Node:
     counter = 0
@@ -47,105 +48,102 @@
 
     def add(self, node):
         self.children.append(node)
 
     def compute_bbox(self):
         self.box = BoundingBox(
             [float("inf"), float("inf"), float("inf")],
-            [-float("inf"), -float("inf"), -float("inf")])
+            [-float("inf"), -float("inf"), -float("inf")],
+        )
         for c in self.children:
             c.compute_bbox()
             self.box.add(c.box)
         for g in self.features:
             self.box.add(g.box)
 
     def to_tileset(self, transform):
         self.compute_bbox()
         tiles = {
             "asset": {"version": "1.0"},
             "geometricError": 500,  # TODO
-            "root": self.to_tileset_r(500)
+            "root": self.to_tileset_r(500),
         }
         tiles["root"]["transform"] = [round(float(e), 3) for e in transform]
         return tiles
 
     def to_tileset_r(self, error):
+        if self.box is None:
+            raise RuntimeError(
+                "The attribute box cannot be None. Use the method to_tileset."
+            )
         (c1, c2) = (self.box.min, self.box.max)
-        center = [(c1[i] + c2[i]) / 2 for i in range(0, 3)]
+        center = [(c1[i] + c2[i]) / 2 for i in range(3)]
         x_axis = [(c2[0] - c1[0]) / 2, 0, 0]
         y_axis = [0, (c2[1] - c1[1]) / 2, 0]
         z_axis = [0, 0, (c2[2] - c1[2]) / 2]
         box = [round(x, 3) for x in center + x_axis + y_axis + z_axis]
         tile = {
-            "boundingVolume": {
-                "box": box
-            },
+            "boundingVolume": {"box": box},
             "geometricError": error,  # TODO
-            "children": [n.to_tileset_r(error / 2.) for n in self.children],
-            "refine": "add"
+            "children": [n.to_tileset_r(error / 2.0) for n in self.children],
+            "refine": "add",
         }
         if len(self.features) != 0:
-            tile["content"] = {
-                "uri": f"tiles/{self.id}.b3dm"
-            }
+            tile["content"] = {"uri": f"tiles/{self.id}.b3dm"}
 
         return tile
 
     def all_nodes(self):
         nodes = [self]
         for c in self.children:
             nodes.extend(c.all_nodes())
         return nodes
 
 
 def tile_extent(extent, size, i, j):
-    min_extent = [
-        extent.min[0] + i * size,
-        extent.min[1] + j * size]
-    max_extent = [
-        extent.min[0] + (i + 1) * size,
-        extent.min[1] + (j + 1) * size]
+    min_extent = [extent.min[0] + i * size, extent.min[1] + j * size]
+    max_extent = [extent.min[0] + (i + 1) * size, extent.min[1] + (j + 1) * size]
     return BoundingBox(min_extent, max_extent)
 
 
 # TODO: transform
 def arrays2tileset(positions, normals, bboxes, transform, ids=None):
     print("Creating tileset...")
     max_tile_size = 2000
     features_per_tile = 20
-    indices = [i for i in range(len(positions))]
+    indices = list(range(len(positions)))
 
     # glTF is Y-up, so to get the bounding boxes in the 3D tiles
     # coordinate system, we have to apply a Y-to-Z transform to the
     # glTF bounding boxes
     z_up_bboxes = []
     for bbox in bboxes:
         tmp = m = bbox[0]
         M = bbox[1]
         m = [m[0], -m[2], m[1]]
         M = [M[0], -tmp[2], M[1]]
         z_up_bboxes.append([m, M])
 
     # Compute extent
-    x_min = y_min = float('inf')
-    x_max = y_max = - float('inf')
+    x_min = y_min = float("inf")
+    x_max = y_max = -float("inf")
 
     for bbox in z_up_bboxes:
         x_min = min(x_min, bbox[0][0])
         y_min = min(y_min, bbox[0][1])
         x_max = max(x_max, bbox[1][0])
         y_max = max(y_max, bbox[1][1])
     extent = BoundingBox([x_min, y_min], [x_max, y_max])
     extent_x = x_max - x_min
     extent_y = y_max - y_min
 
     # Create quadtree
     tree = Node()
-    for i in range(0, int(math.ceil(extent_x / max_tile_size))):
-        for j in range(0, int(math.ceil(extent_y / max_tile_size))):
+    for i in range(int(math.ceil(extent_x / max_tile_size))):
+        for j in range(int(math.ceil(extent_y / max_tile_size))):
             tile = tile_extent(extent, max_tile_size, i, j)
 
             geoms = []
             for idx, box in zip(indices, z_up_bboxes):
                 bbox = BoundingBox(box[0], box[1])
 
                 if tile.inside(bbox.center()):
@@ -153,74 +151,91 @@
 
             if len(geoms) == 0:
                 continue
 
             if len(geoms) > features_per_tile:
                 node = Node(geoms[0:features_per_tile])
                 tree.add(node)
-                divide(tile, geoms[features_per_tile:len(geoms)], i * 2,
-                       j * 2, max_tile_size / 2., features_per_tile, node)
+                divide(
+                    tile,
+                    geoms[features_per_tile : len(geoms)],
+                    i * 2,
+                    j * 2,
+                    max_tile_size / 2.0,
+                    features_per_tile,
+                    node,
+                )
             else:
                 node = Node(geoms)
                 tree.add(node)
 
     # Export b3dm & tileset
     tileset = tree.to_tileset(transform)
-    f = open("tileset.json", 'w')
-    f.write(json.dumps(tileset))
+    with open("tileset.json", "w") as f:
+        f.write(json.dumps(tileset))
     print("Creating tiles...")
     nodes = tree.all_nodes()
-    identity = np.identity(4).flatten('F')
+    identity = np.identity(4).flatten("F")
     try:
         os.makedirs("tiles")
     except OSError as e:
         if e.errno != errno.EEXIST:
             raise
     for node in nodes:
         if len(node.features) != 0:
             bin_arrays = []
             gids = []
             for feature in node.features:
                 pos = feature.index
-                bin_arrays.append({
-                    'position': positions[pos],
-                    'normal': normals[pos],
-                    'bbox': [[float(i) for i in j] for j in bboxes[pos]],
-                })
+                bin_arrays.append(
+                    {
+                        "position": positions[pos],
+                        "normal": normals[pos],
+                        "bbox": [[float(i) for i in j] for j in bboxes[pos]],
+                    }
+                )
                 if ids is not None:
                     gids.append(ids[pos])
             gltf = GlTF.from_binary_arrays(bin_arrays, identity)
             bt = None
             if ids is not None:
                 bt = BatchTable()
-                bt.add_property_from_array("id", gids)
-            b3dm = B3dm.from_glTF(gltf, bt).to_array()
-            f = open(f"tiles/{node.id}.b3dm", 'wb')
-            f.write(b3dm)
+                bt.add_property_as_json("id", gids)
+            b3dm = B3dm.from_gltf(gltf, bt).to_array()
 
+            with open(f"tiles/{node.id}.b3dm", "wb") as f:
+                f.write(b3dm.tobytes())
 
-def divide(extent, geometries, x_offset, y_offset, tile_size,
-           features_per_tile, parent):
-    for i in range(0, 2):
-        for j in range(0, 2):
+
+def divide(
+    extent, geometries, x_offset, y_offset, tile_size, features_per_tile, parent
+):
+    for i in range(2):
+        for j in range(2):
             tile = tile_extent(extent, tile_size, i, j)
 
             geoms = []
             for g in geometries:
                 if tile.inside(g.box.center()):
                     geoms.append(g)
             if len(geoms) == 0:
                 continue
 
             if len(geoms) > features_per_tile:
                 node = Node(geoms[0:features_per_tile])
                 parent.add(node)
-                divide(tile, geoms[features_per_tile:len(geoms)],
-                       (x_offset + i) * 2, (y_offset + j) * 2,
-                       tile_size / 2., features_per_tile, node)
+                divide(
+                    tile,
+                    geoms[features_per_tile : len(geoms)],
+                    (x_offset + i) * 2,
+                    (y_offset + j) * 2,
+                    tile_size / 2.0,
+                    features_per_tile,
+                    node,
+                )
             else:
                 node = Node(geoms)
                 parent.add(node)
 
 
 def wkbs_to_tileset(wkbs, ids, transform):
     geoms = [TriangleSoup.from_wkb_multipolygon(wkb) for wkb in wkbs]
@@ -254,96 +269,110 @@
     connection = build_secure_conn(db_conn_info)
     cur = connection.cursor()
 
     print("Loading data from database...")
     cur.execute(f"SELECT ST_3DExtent({column_name}) FROM {table_name}")
     extent = cur.fetchall()[0][0]
     extent = [m.split(" ") for m in extent[6:-1].split(",")]
-    offset = [(float(extent[1][0]) + float(extent[0][0])) / 2,
-              (float(extent[1][1]) + float(extent[0][1])) / 2,
-              (float(extent[1][2]) + float(extent[0][2])) / 2]
+    offset = [
+        (float(extent[1][0]) + float(extent[0][0])) / 2,
+        (float(extent[1][1]) + float(extent[0][1])) / 2,
+        (float(extent[1][2]) + float(extent[0][2])) / 2,
+    ]
 
     id_statement = ""
     if id_column_name is not None:
         id_statement = "," + id_column_name
-    cur.execute("SELECT ST_AsBinary(ST_RotateX(ST_Translate({0}, {1}, {2}, {3}), -pi() / 2)),"
-                "ST_Area(ST_Force2D({0})) AS weight{5} FROM {4} ORDER BY weight DESC"
-                .format(column_name, -offset[0], -offset[1], -offset[2],
-                        table_name, id_statement))
+    cur.execute(
+        "SELECT ST_AsBinary(ST_RotateX(ST_Translate({0}, {1}, {2}, {3}), -pi() / 2)),"
+        "ST_Area(ST_Force2D({0})) AS weight{5} FROM {4} ORDER BY weight DESC".format(
+            column_name, -offset[0], -offset[1], -offset[2], table_name, id_statement
+        )
+    )
     res = cur.fetchall()
     wkbs = [t[0] for t in res]
     ids = None
     if id_column_name is not None:
         ids = [t[2] for t in res]
-    transform = np.array([
-        [1, 0, 0, offset[0]],
-        [0, 1, 0, offset[1]],
-        [0, 0, 1, offset[2]],
-        [0, 0, 0, 1]], dtype=float)
-    transform = transform.flatten('F')
+    transform = np.array(
+        [
+            [1, 0, 0, offset[0]],
+            [0, 1, 0, offset[1]],
+            [0, 0, 1, offset[2]],
+            [0, 0, 0, 1],
+        ],
+        dtype=float,
+    )
+    transform = transform.flatten("F")
 
     wkbs_to_tileset(wkbs, ids, transform)
 
 
 def from_directory(directory, offset):
     # TODO: improvement -> order wkbs by geometry size, similarly to database mode
     offset = (0, 0, 0) if offset is None else offset
     # open all wkbs from directory
     files = os.listdir(directory)
     files = [os.path.join(directory, f) for f in os.listdir(directory)]
-    files = [f for f in files if os.path.isfile(f) and os.path.splitext(f)[1] == '.wkb']
+    files = [f for f in files if os.path.isfile(f) and os.path.splitext(f)[1] == ".wkb"]
     wkbs = []
     for f in files:
-        of = open(f, 'rb')
+        of = open(f, "rb")
         wkbs.append(of.read())
         of.close()
 
-    transform = np.array([
-        [1, 0, 0, offset[0]],
-        [0, 1, 0, offset[1]],
-        [0, 0, 1, offset[2]],
-        [0, 0, 0, 1]], dtype=float)
-    transform = transform.flatten('F')
+    transform = np.array(
+        [
+            [1, 0, 0, offset[0]],
+            [0, 1, 0, offset[1]],
+            [0, 0, 1, offset[2]],
+            [0, 0, 0, 1],
+        ],
+        dtype=float,
+    )
+    transform = transform.flatten("F")
     wkbs_to_tileset(wkbs, None, transform)
 
 
-def init_parser(subparser):
+def init_parser(
+    subparser: "argparse._SubParsersAction[Any]",
+) -> argparse.ArgumentParser:
     descr = "Generate a tileset from a set of geometries"
-    parser = subparser.add_parser('export', help=descr)
+    parser: argparse.ArgumentParser = subparser.add_parser("export", help=descr)
 
     group = parser.add_mutually_exclusive_group()
 
     d_help = "Name of the directory containing the geometries"
-    group.add_argument('-d', metavar='DIRECTORY', type=str, help=d_help)
+    group.add_argument("-d", metavar="DIRECTORY", type=str, help=d_help)
 
     o_help = "Offset of the geometries (only with '-d')"
-    parser.add_argument('-o', nargs=3, metavar=('X', 'Y', 'Z'), type=float, help=o_help)
+    parser.add_argument("-o", nargs=3, metavar=("X", "Y", "Z"), type=float, help=o_help)
 
     D_help = """
     Database connexion info (e.g. 'service=py3dtiles' or \
     'dbname=py3dtiles host=localhost port=5432 user=yourname password=yourpwd')
     """
-    group.add_argument('-D', metavar='DB_CONNINFO', type=str, help=D_help)
+    group.add_argument("-D", metavar="DB_CONNINFO", type=str, help=D_help)
 
     t_help = "Table name (required if '-D' option is activated)"
-    parser.add_argument('-t', metavar='TABLE', type=str, help=t_help)
+    parser.add_argument("-t", metavar="TABLE", type=str, help=t_help)
 
     c_help = "Geometry column name (required if '-D' option is activated)"
-    parser.add_argument('-c', metavar='COLUMN', type=str, help=c_help)
+    parser.add_argument("-c", metavar="COLUMN", type=str, help=c_help)
 
     i_help = "Id column name (only with '-D')"
-    parser.add_argument('-i', metavar='IDCOLUMN', type=str, help=i_help)
+    parser.add_argument("-i", metavar="IDCOLUMN", type=str, help=i_help)
 
     return parser
 
 
-def main(args):
+def main(args: argparse.Namespace) -> None:
     if args.D is not None:
         if args.t is None or args.c is None:
-            print('Error: please define a table (-t) and column (-c)')
+            print("Error: please define a table (-t) and column (-c)")
             exit()
 
         from_db(args.D, args.t, args.c, args.i)
     elif args.d is not None:
         from_directory(args.d, args.o)
     else:
-        raise NameError('Error: database or directory must be set')
+        raise NameError("Error: database or directory must be set")
```

### Comparing `py3dtiles-5.0.0/py3dtiles/reader/las_reader.py` & `py3dtiles-6.0.0/py3dtiles/reader/xyz_reader.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,128 +1,152 @@
-import json
 import math
 from pathlib import Path
-import pickle
-import struct
-import subprocess
+from typing import Generator, List, Optional, Tuple
 
-import laspy
 import numpy as np
+import numpy.typing as npt
+from pyproj import Transformer
 
-from py3dtiles.utils import ResponseType
+from py3dtiles.typing import MetadataReaderType, OffsetScaleType, PortionItemType
 
 
-def get_metadata(path: Path, color_scale=None, fraction: int = 100) -> dict:
-    pointcloud_file_portions = []
-    srs_in = None
-
-    filename = str(path)
-    with laspy.open(filename) as f:
-        point_count = f.header.point_count * fraction // 100
-
-        # read the first points red channel
-        if not color_scale:
-            if 'red' in f.header.point_format.dimension_names:
-                points = next(f.chunk_iterator(10_000))['red']
-                if np.max(points) > 255:
-                    color_scale = 1.0 / 255
+def get_metadata(path: Path, fraction: int = 100) -> MetadataReaderType:
+    aabb = None
+    count = 0
+    seek_values = []
+
+    with path.open() as f:
+        while True:
+            batch = 10_000
+            points = np.zeros((batch, 3))
+
+            offset = f.tell()
+            for i in range(batch):
+                line = f.readline()
+                if not line:
+                    points = np.resize(points, (i, 3))
+                    break
+                points[i] = [float(s) for s in line.split(" ")][:3]
+
+            if points.shape[0] == 0:
+                break
+
+            if not count % 1_000_000:
+                seek_values += [offset]
+
+            count += points.shape[0]
+            batch_aabb = np.array([np.min(points, axis=0), np.max(points, axis=0)])
+
+            # Update aabb
+            if aabb is None:
+                aabb = batch_aabb
             else:
-                # the intensity is then used as color
-                color_scale = 1.0 / 255
+                aabb[0] = np.minimum(aabb[0], batch_aabb[0])
+                aabb[1] = np.maximum(aabb[1], batch_aabb[1])
 
-        _1M = min(point_count, 1_000_000)
-        steps = math.ceil(point_count / _1M)
-        portions = [(i * _1M, min(point_count, (i + 1) * _1M)) for i in range(steps)]
-        for p in portions:
-            pointcloud_file_portions += [(filename, p)]
-
-        output = subprocess.check_output(['pdal', 'info', '--summary', filename])
-        summary = json.loads(output)['summary']
-        if 'srs' in summary:
-            srs_in = summary['srs'].get('proj4')
+        # We need an exact point count
+        point_count = count * fraction // 100
+
+        _1M = min(count, 1_000_000)
+        steps = math.ceil(count / _1M)
+        if steps != len(seek_values):
+            raise ValueError(
+                "the size of seek_values should be equal to steps,"
+                f"currently steps = {steps} and len(seek_values) = {len(seek_values)}"
+            )
+        portions: List[PortionItemType] = [
+            (i * _1M, min(count, (i + 1) * _1M), seek_values[i]) for i in range(steps)
+        ]
+
+        pointcloud_file_portions = [(str(path), p) for p in portions]
+
+    if aabb is None:
+        raise ValueError(f"There is no point in the file {path}")
 
     return {
-        'portions': pointcloud_file_portions,
-        'aabb': np.array([f.header.mins, f.header.maxs]),
-        'color_scale': color_scale,
-        'srs_in': srs_in,
-        'point_count': point_count,
-        'avg_min': np.array(f.header.mins)
+        "portions": pointcloud_file_portions,
+        "aabb": aabb,
+        "crs_in": None,
+        "point_count": point_count,
+        "avg_min": aabb[0],
     }
 
 
-def run(filename: str, offset_scale, portion, queue, transformer):
+def run(
+    filename: str,
+    offset_scale: OffsetScaleType,
+    portion: PortionItemType,
+    transformer: Optional[Transformer],
+    color_scale: Optional[float],
+) -> Generator[
+    Tuple[npt.NDArray[np.float32], npt.NDArray[np.uint8], npt.NDArray[np.uint8]],
+    None,
+    None,
+]:
     """
-    Reads points from a las file
+    Reads points from a xyz file
+
+    Consider XYZIRGB format following FME documentation(*). If the number of
+    features does not correspond (i.e. does not equal to 7), we do the
+    following hypothesis:
+    - 3 features mean XYZ
+    - 4 features mean XYZI
+    - 6 features mean XYZRGB
+
+    NOTE: we assume RGB are 8 bits components.
+
+    (*) See: https://docs.safe.com/fme/html/FME_Desktop_Documentation/FME_ReadersWriters/pointcloudxyz/pointcloudxyz.htm
     """
-    try:
-        with laspy.open(filename) as f:
+    with open(filename) as f:
+
+        point_count = portion[1] - portion[0]
+
+        step = min(point_count, max((point_count) // 10, 100000))
+
+        f.seek(portion[2])
 
-            point_count = portion[1] - portion[0]
+        feature_nb = 7
 
-            step = min(point_count, max(point_count // 10, 100_000))
+        for _ in range(0, point_count, step):
+            points = np.zeros((step, feature_nb), dtype=np.float32)
+
+            for j in range(step):
+                line = f.readline()
+                if not line:
+                    points = np.resize(points, (j, feature_nb))
+                    break
+                line_features: List[float | None] = [float(s) for s in line.split(" ")]
+                if len(line_features) == 3:
+                    line_features += [None] * 4  # Insert intensity and RGB
+                elif len(line_features) == 4:
+                    line_features += [None] * 3  # Insert RGB
+                elif len(line_features) == 6:
+                    line_features.insert(3, None)  # Insert intensity
+                points[j] = line_features
+
+            x, y, z = (points[:, c] for c in [0, 1, 2])
+
+            if transformer:
+                x, y, z = transformer.transform(x, y, z)
+
+            x = (x + offset_scale[0][0]) * offset_scale[1][0]
+            y = (y + offset_scale[0][1]) * offset_scale[1][1]
+            z = (z + offset_scale[0][2]) * offset_scale[1][2]
+
+            coords = np.vstack((x, y, z)).transpose()
+
+            if offset_scale[2] is not None:
+                # Apply transformation matrix (because the tile's transform will contain
+                # the inverse of this matrix)
+                coords = np.dot(coords, offset_scale[2])
+
+            coords = np.ascontiguousarray(coords.astype(np.float32))
+
+            # Read colors: 3 last columns of the point cloud
+            if color_scale is None:
+                colors = points[:, -3:].astype(np.uint8)
+            else:
+                colors = np.clip(points[:, -3:] * color_scale, 0, 255).astype(np.uint8)
 
-            indices = [i for i in range(math.ceil(point_count / step))]
+            classification = np.zeros((points.shape[0], 1), dtype=np.uint8)
 
-            color_scale = offset_scale[3]
-
-            for index in indices:
-                start_offset = portion[0] + index * step
-                num = min(step, portion[1] - start_offset)
-
-                # read scaled values and apply offset
-                f.seek(start_offset)
-                points = next(f.chunk_iterator(num))
-
-                x, y, z = points.x, points.y, points.z
-                if transformer:
-                    x, y, z = transformer.transform(x, y, z)
-
-                x = (x + offset_scale[0][0]) * offset_scale[1][0]
-                y = (y + offset_scale[0][1]) * offset_scale[1][1]
-                z = (z + offset_scale[0][2]) * offset_scale[1][2]
-
-                coords = np.vstack((x, y, z)).transpose()
-
-                if offset_scale[2] is not None:
-                    # Apply transformation matrix (because the tile's transform will contain
-                    # the inverse of this matrix)
-                    coords = np.dot(coords, offset_scale[2])
-
-                coords = np.ascontiguousarray(coords.astype(np.float32))
-
-                # Read colors
-
-                # todo: attributes
-                if 'red' in f.header.point_format.dimension_names:
-                    red = points['red']
-                    green = points['green']
-                    blue = points['blue']
-                else:
-                    red = points['intensity']
-                    green = points['intensity']
-                    blue = points['intensity']
-
-                if not color_scale:
-                    red = red.astype(np.uint8)
-                    green = green.astype(np.uint8)
-                    blue = blue.astype(np.uint8)
-                else:
-                    red = (red * color_scale).astype(np.uint8)
-                    green = (green * color_scale).astype(np.uint8)
-                    blue = (blue * color_scale).astype(np.uint8)
-
-                colors = np.vstack((red, green, blue)).transpose()
-
-                queue.send_multipart(
-                    [
-                        ResponseType.NEW_TASK.value,
-                        b'',
-                        pickle.dumps({'xyz': coords, 'rgb': colors}),
-                        struct.pack('>I', len(coords))
-                    ], copy=False)
-
-            queue.send_multipart([ResponseType.READ.value])
-
-    except Exception as e:
-        print(f'Exception while reading points from las file {filename}')
-        raise e
+            yield coords, colors, classification
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `py3dtiles-5.0.0/py3dtiles/tilers/b3dm/wkb_utils.py` & `py3dtiles-6.0.0/py3dtiles/tilers/b3dm/wkb_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,175 +1,163 @@
+from __future__ import annotations
+
 import math
 import struct
+from typing import List
 
 from earcut.earcut import earcut
 import numpy as np
+import numpy.typing as npt
+
+CoordinateType = npt.NDArray[np.float32]
+LineType = List[CoordinateType]
+PolygonType = List[LineType]
+MultiPolygonsType = List[PolygonType]
+
+PolygonAsTriangleType = List[npt.NDArray[np.float32]]  # the array shape is 3, 3
+
 
 class TriangleSoup:
-    def __init__(self):
-        self.triangles = []
+    def __init__(self) -> None:
+        self.triangles: list[PolygonAsTriangleType] = []
 
     @staticmethod
-    def from_wkb_multipolygon(wkb, associated_data=None):
+    def from_wkb_multipolygon(
+        wkb: bytes, associated_data: list[bytes] | None = None
+    ) -> TriangleSoup:
         """
-        Parameters
-        ----------
-        wkb : string
-            Well-Known Binary binary string describing a multipolygon
+        :param wkb: Well-Known Binary binary string describing a multipolygon
 
-        associated_data : array
-            array of multipolygons containing data attached to the wkb
+        :param associated_data: array of multipolygons containing data attached to the wkb
             parameter multipolygon. Must be the same size as wkb.
-
-        Returns
-        -------
-        ts : TriangleSoup
         """
-        multipolygons = [parse(bytes(wkb))]
+        multipolygons: list[MultiPolygonsType] = [parse(bytes(wkb))]
 
         if associated_data is None:
             associated_data = []
 
         for additional_wkb in associated_data:
             multipolygons.append(parse(bytes(additional_wkb)))
 
-        triangles_array = [[] for _ in range(len(multipolygons))]
-        for i in range(0, len(multipolygons[0])):
-            polygon = multipolygons[0][i]
+        triangles_array: list[PolygonAsTriangleType] = [
+            [] for _ in range(len(multipolygons))
+        ]
+        for i in range(len(multipolygons[0])):
+            polygon: PolygonType = multipolygons[0][i]
             additional_polygons = [mp[i] for mp in multipolygons[1:]]
             triangles = triangulate(polygon, additional_polygons)
             for array, tri in zip(triangles_array, triangles):
                 array += tri
 
         ts = TriangleSoup()
         ts.triangles = triangles_array
 
         return ts
 
-    def get_position_array(self):
+    def get_position_array(self) -> bytes:
         """
-        Parameters
-        ----------
-
-        Returns
-        -------
-        Binary array of vertex positions
+        Returns a binary array of vertex positions
         """
 
         vertex_triangles = self.triangles[0]
         vertex_array = vertex_attribute_to_array(vertex_triangles)
-        return b''.join(vertex_array)
+        return b"".join([vertex.tobytes() for vertex in vertex_array])
 
-    def get_data_array(self, index):
+    def get_data_array(self, index: int) -> bytes:
         """
-        Parameters
-        ----------
-        index: int
-            The index of the associated data
-
-        Returns
-        -------
-        Binary array of vertex data
+        Returns a binary array of vertex data
         """
 
         vertex_triangles = self.triangles[1 + index]
         vertex_array = vertex_attribute_to_array(vertex_triangles)
-        return b''.join(vertex_array)
+        return b"".join([vertex.tobytes() for vertex in vertex_array])
 
-    def get_normal_array(self):
+    def get_normal_array(self) -> bytes:
         """
-        Parameters
-        ----------
-
-        Returns
-        -------
-        Binary array of vertice normals
+        Returns a binary array of vertex normals
         """
-        normals = []
+        normals: list[CoordinateType] = []
         for t in self.triangles[0]:
             U = t[1] - t[0]
             V = t[2] - t[0]
             N = np.cross(U, V)
             norm = np.linalg.norm(N)
             if norm == 0:
                 normals.append(np.array([0, 0, 1], dtype=np.float32))
             else:
                 normals.append(N / norm)
 
         vertex_array = face_attribute_to_array(normals)
-        return b''.join(vertex_array)
+        return b"".join([vertex.tobytes() for vertex in vertex_array])
 
-    def get_bbox(self):
+    def get_bbox(self) -> list[npt.NDArray[np.float32]]:
         """
-        Parameters
-        ----------
-
-        Returns
-        -------
-        Array [[minX, minY, minZ],[maxX, maxY, maxZ]]
+        Returns the bbox in this format: [[minX, minY, minZ],[maxX, maxY, maxZ]]
         """
         mins = np.array([np.min(t, 0) for t in self.triangles[0]])
         maxs = np.array([np.max(t, 0) for t in self.triangles[0]])
         return [np.min(mins, 0), np.max(maxs, 0)]
 
 
-def face_attribute_to_array(triangles):
+def face_attribute_to_array(triangles: list[CoordinateType]) -> list[CoordinateType]:
     array = []
     for face in triangles:
         array += [face, face, face]
     return array
 
 
-def vertex_attribute_to_array(triangles):
+def vertex_attribute_to_array(triangles: PolygonAsTriangleType) -> list[CoordinateType]:
     array = []
     for face in triangles:
         for vertex in face:
             array.append(vertex)
     return array
 
 
-def parse(wkb):
-    multipolygon = []
-    byteorder = struct.unpack('b', wkb[0:1])
-    bo = '<' if byteorder[0] else '>'
-    geomtype = struct.unpack(bo + 'I', wkb[1:5])[0]
+def parse(wkb: bytes) -> MultiPolygonsType:
+    multipolygon: MultiPolygonsType = []
+    byteorder = struct.unpack("b", wkb[0:1])
+    bo = "<" if byteorder[0] else ">"
+    geomtype = struct.unpack(bo + "I", wkb[1:5])[0]
     has_z = (geomtype == 1006) or (geomtype == 1015)
     # MultipolygonZ or polyhedralSurface
     pnt_offset = 24 if has_z else 16
-    pnt_unpack = 'ddd' if has_z else 'dd'
-    geom_nb = struct.unpack(bo + 'I', wkb[5:9])[0]
+    pnt_unpack = "ddd" if has_z else "dd"
+    geom_nb = struct.unpack(bo + "I", wkb[5:9])[0]
     # print(struct.unpack('b', wkb[9:10])[0])
     # print(struct.unpack('I', wkb[10:14])[0])   # 1003 (Polygon)
     # print(struct.unpack('I', wkb[14:18])[0])   # num lines
     # print(struct.unpack('I', wkb[18:22])[0])   # num points
     offset = 9
-    for _ in range(0, geom_nb):
+    for _ in range(geom_nb):
         offset += 5  # struct.unpack('bI', wkb[offset:offset + 5])[0]
         # 1 (byteorder), 1003 (Polygon)
-        line_nb = struct.unpack(bo + 'I', wkb[offset:offset + 4])[0]
+        line_nb = struct.unpack(bo + "I", wkb[offset : offset + 4])[0]
         offset += 4
         polygon = []
-        for _ in range(0, line_nb):
-            point_nb = struct.unpack(bo + 'I', wkb[offset:offset + 4])[0]
+        for _ in range(line_nb):
+            point_nb = struct.unpack(bo + "I", wkb[offset : offset + 4])[0]
             offset += 4
             line = []
-            for _ in range(0, point_nb - 1):
+            for _ in range(point_nb - 1):
                 pt = np.array(
-                    struct.unpack(bo + pnt_unpack, wkb[offset:offset + pnt_offset]),
-                    dtype=np.float32
+                    struct.unpack(bo + pnt_unpack, wkb[offset : offset + pnt_offset]),
+                    dtype=np.float32,
                 )
                 offset += pnt_offset
                 line.append(pt)
             offset += pnt_offset  # skip redundant point
             polygon.append(line)
         multipolygon.append(polygon)
     return multipolygon
 
 
-def triangulate(polygon, additional_polygons=None):
+def triangulate(
+    polygon: PolygonType, additional_polygons: list[PolygonType] | None = None
+) -> list[PolygonAsTriangleType]:
     """
     Triangulates 3D polygons
     """
     # let's find out if the polygon is *mostly* clockwise or counter-clockwise
     # and triangulate accordingly
     # for 2D explanations:
     # https://stackoverflow.com/a/1165943/1528985
@@ -191,35 +179,39 @@
     # - comparing these 3 results actually give us the most interesting plane
     # to triangulate in (the plane were the projected area is the biggest)
     # - we drop the 1/2 factor because we are only interesting in the sign and relative comparison
     vect_prod = np.array([0, 0, 0], dtype=np.float32)
     for i in range(len(polygon[0])):
         curr_edge = polygon[0][i]
         next_edge = polygon[0][(i + 1) % len(polygon[0])]
-        vect_prod += np.array([
-            # yz plane, seen from negative x
-            (curr_edge[1] - next_edge[1]) * (next_edge[2] + curr_edge[2]),
-            # zx plane, seen from negative y
-            (curr_edge[2] - next_edge[2]) * (next_edge[0] + curr_edge[0]),
-            # xy plane, seen from negative z
-            (curr_edge[0] - next_edge[0]) * (next_edge[1] + curr_edge[1]),
-        ], dtype=np.float32)
+        vect_prod += np.array(
+            [
+                # yz plane, seen from negative x
+                (curr_edge[1] - next_edge[1]) * (next_edge[2] + curr_edge[2]),
+                # zx plane, seen from negative y
+                (curr_edge[2] - next_edge[2]) * (next_edge[0] + curr_edge[0]),
+                # xy plane, seen from negative z
+                (curr_edge[0] - next_edge[0]) * (next_edge[1] + curr_edge[1]),
+            ],
+            dtype=np.float32,
+        )
 
     if additional_polygons is None:
         additional_polygons = []
 
     polygon_2d = []
     holes = []
     delta = 0
     for p in polygon[:-1]:
         holes.append(delta + len(p))
         delta += len(p)
     # triangulation of the polygon projected on planes (xy) (zx) or (yz)
-    if (math.fabs(vect_prod[0]) > math.fabs(vect_prod[1])
-       and math.fabs(vect_prod[0]) > math.fabs(vect_prod[2])):
+    if math.fabs(vect_prod[0]) > math.fabs(vect_prod[1]) and math.fabs(
+        vect_prod[0]
+    ) > math.fabs(vect_prod[2]):
         # (yz) projection
         for linestring in polygon:
             for point in linestring:
                 polygon_2d.extend([point[1], point[2]])
     elif math.fabs(vect_prod[1]) > math.fabs(vect_prod[2]):
         # (zx) projection
         for linestring in polygon:
@@ -229,40 +221,42 @@
         # (xy) projection
         for linestring in polygon:
             for point in linestring:
                 polygon_2d.extend([point[0], point[1]])
 
     triangles_idx = earcut(polygon_2d, holes, 2)
 
-    arrays = [[] for _ in range(len(additional_polygons) + 1)]
+    arrays: list[PolygonAsTriangleType] = [
+        [] for _ in range(len(additional_polygons) + 1)
+    ]
     for i in range(0, len(triangles_idx), 3):
-        t = triangles_idx[i:i + 3]
+        t = triangles_idx[i : i + 3]
         p0 = unflatten(polygon, holes, t[0])
         p1 = unflatten(polygon, holes, t[1])
         p2 = unflatten(polygon, holes, t[2])
         # triangulation may break triangle orientation, test it before
         # adding triangles
         # FIXME fix / change the triangulation code instead?
         cross_product = np.cross(p1 - p0, p2 - p0)
         invert = np.dot(vect_prod, cross_product) < 0
         if invert:
-            arrays[0].append([p1, p0, p2])
+            arrays[0].append(np.array([p1, p0, p2], dtype=np.float32))
         else:
-            arrays[0].append([p0, p1, p2])
-        for array, p in zip(arrays[1:], additional_polygons):
-            pp0 = unflatten(p, holes, t[0])
-            pp1 = unflatten(p, holes, t[1])
-            pp2 = unflatten(p, holes, t[2])
+            arrays[0].append(np.array([p0, p1, p2], dtype=np.float32))
+        for array, additional_polygon in zip(arrays[1:], additional_polygons):
+            pp0 = unflatten(additional_polygon, holes, t[0])
+            pp1 = unflatten(additional_polygon, holes, t[1])
+            pp2 = unflatten(additional_polygon, holes, t[2])
             if invert:
-                array.append([pp1, pp0, pp2])
+                array.append(np.array([pp1, pp0, pp2], dtype=np.float32))
             else:
-                array.append([pp0, pp1, pp2])
+                array.append(np.array([pp0, pp1, pp2], dtype=np.float32))
 
     return arrays
 
 
-def unflatten(array, lengths, index):
-    for i in reversed(range(0, len(lengths))):
+def unflatten(array: PolygonType, lengths: list[int], index: int) -> CoordinateType:
+    for i in reversed(range(len(lengths))):
         lgth = lengths[i]
         if index >= lgth:
             return array[i + 1][index - lgth]
     return array[0][index]
```

### Comparing `py3dtiles-5.0.0/py3dtiles/tilers/matrix_manipulation.py` & `py3dtiles-6.0.0/py3dtiles/tilers/matrix_manipulation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,20 @@
+from typing import TypeVar
+
 import numpy as np
+import numpy.typing as npt
+
+_T = TypeVar("_T", bound=npt.NBitBase)
 
 
-def make_rotation_matrix(z1: np.ndarray, z2: np.ndarray) -> np.ndarray:
-    v0 = z1 / np.linalg.norm(z1)
-    v1 = z2 / np.linalg.norm(z2)
+def make_rotation_matrix(
+    z1: "npt.NDArray[np.floating[_T]]", z2: "npt.NDArray[np.floating[_T]]"
+) -> "npt.NDArray[np.floating[_T]]":
+    v0: "npt.NDArray[np.floating[_T]]" = z1 / np.linalg.norm(z1)
+    v1: "npt.NDArray[np.floating[_T]]" = z2 / np.linalg.norm(z2)
 
     angle = np.arccos(np.clip(np.dot(v0, v1), -1.0, 1.0))
     direction = np.cross(v0, v1)
 
     sina = np.sin(angle)
     cosa = np.cos(angle)
     direction[:3] /= np.sqrt(np.dot(direction[:3], direction[:3]))
@@ -18,20 +25,23 @@
     rotation_matrix += np.array(
         [
             [0.0, -direction[2], direction[1]],
             [direction[2], 0.0, -direction[0]],
             [-direction[1], direction[0], 0.0],
         ]
     )
-    final_rotation_matrix = np.identity(4)
+    final_rotation_matrix = np.identity(4, dtype=z1.dtype)
     final_rotation_matrix[:3, :3] = rotation_matrix
 
     return final_rotation_matrix
 
-def make_scale_matrix(factor: float) -> np.ndarray:
-    scale_matrix = np.diag([factor, factor, factor, 1.0])
-    return scale_matrix
 
-def make_translation_matrix(direction: np.ndarray) -> np.ndarray:
-    translation_matrix = np.identity(4)
+def make_scale_matrix(factor: float) -> npt.NDArray[np.float32]:
+    return np.diag([factor, factor, factor, 1.0])
+
+
+def make_translation_matrix(
+    direction: "npt.NDArray[np.floating[_T]]",
+) -> "npt.NDArray[np.floating[_T]]":
+    translation_matrix = np.identity(4, dtype=direction.dtype)
     translation_matrix[:3, 3] = direction[:3]
     return translation_matrix
```

### Comparing `py3dtiles-5.0.0/py3dtiles/tilers/node/distance.py` & `py3dtiles-6.0.0/py3dtiles/tilers/node/distance.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,38 @@
-from numba import jit, njit # type: ignore
+from numba import jit, njit  # type: ignore [attr-defined]
 import numpy as np
 
 
-@njit("boolean(float32[:,:], float32[:], float32)", fastmath=True, nogil=True, cache=True)
+@njit(
+    "boolean(float32[:,:], float32[:], float32)", fastmath=True, nogil=True, cache=True
+)
 def is_point_far_enough(points, tested_point, squared_min_distance):
     nbp = points.shape[0]
     farenough = True
     for i in range(nbp - 1, -1, -1):
-        if (tested_point[0] - points[i][0]) ** 2 + \
-           (tested_point[1] - points[i][1]) ** 2 + \
-           (tested_point[2] - points[i][2]) ** 2 < squared_min_distance:
+        if (
+            (tested_point[0] - points[i][0]) ** 2
+            + (tested_point[1] - points[i][1]) ** 2
+            + (tested_point[2] - points[i][2]) ** 2
+        ) < squared_min_distance:
             farenough = False
             break
     return farenough
 
 
 @jit(cache=True, nogil=True)
 def xyz_to_child_index(xyz, aabb_center):
     test = np.greater_equal(xyz - aabb_center, 0).astype(np.int8)
     return np.sum(np.left_shift(test, np.array([2, 1, 0])), axis=1)
 
 
-@njit("int32[:](float32[:,:], int32[:], float32[:], float32[:], int32)", cache=True, nogil=True)
+@njit(
+    "int32[:](float32[:,:], int32[:], float32[:], float32[:], int32)",
+    cache=True,
+    nogil=True,
+)
 def xyz_to_key(xyz, cell_count, aabb_min, inv_aabb_size, shift):
     a = ((cell_count * inv_aabb_size) * (xyz - aabb_min)).astype(np.int64)
-    a = np.minimum(
-        np.maximum(a, 0),
-        cell_count - 1)
+    a = np.minimum(np.maximum(a, 0), cell_count - 1)
     a[:, 1] <<= shift
-    a[:, 2] <<= (2 * shift)
+    a[:, 2] <<= 2 * shift
     return np.sum(a, axis=1).astype(np.int32)
```

### Comparing `py3dtiles-5.0.0/py3dtiles/tilers/node/node.py` & `py3dtiles-6.0.0/py3dtiles/tilers/node/node.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,328 +1,529 @@
 from __future__ import annotations
 
-import concurrent.futures
+from concurrent.futures import ProcessPoolExecutor
 import json
 from pathlib import Path
 import pickle
-from typing import Any, Iterator, TYPE_CHECKING
+from typing import Any, Generator, Iterator, TYPE_CHECKING, TypedDict
 
 import numpy as np
 import numpy.typing as npt
 
+from py3dtiles.exceptions import TilerException
 from py3dtiles.tilers.pnts import MIN_POINT_SIZE
-from py3dtiles.tilers.pnts.pnts_writer import points_to_pnts
-from py3dtiles.tileset.feature_table import SemanticPoint
-from py3dtiles.tileset.utils import TileContentReader
-from py3dtiles.utils import aabb_size_to_subdivision_type, node_from_name, node_name_to_path, SubdivisionType
+from py3dtiles.tilers.pnts.pnts_writer import points_to_pnts_file
+from py3dtiles.tileset.content import read_binary_tile_content
+from py3dtiles.tileset.content.feature_table import SemanticPoint
+from py3dtiles.typing import BoundingVolumeBoxDictType, ContentType, TileDictType
+from py3dtiles.utils import (
+    aabb_size_to_subdivision_type,
+    node_from_name,
+    node_name_to_path,
+    SubdivisionType,
+)
 from .distance import xyz_to_child_index
 from .points_grid import Grid
 
 if TYPE_CHECKING:
     from .node_catalog import NodeCatalog
+    from typing_extensions import NotRequired
 
 
-def node_to_tileset(args):
-    return Node.to_tileset(None, args[0], args[1], args[2], args[3], args[4])
+def node_to_tileset(
+    args: tuple[Node, Path, npt.NDArray[np.float32], Node | None, int]
+) -> TileDictType | None:
+    return args[0].to_tileset(args[1], args[2], args[3], args[4], None)
+
+
+class _DummyNodeDictType(TypedDict):
+    children: NotRequired[list[bytes]]
+    grid: NotRequired[Grid]
+    points: NotRequired[
+        list[
+            tuple[npt.NDArray[np.float32], npt.NDArray[np.uint8], npt.NDArray[np.uint8]]
+        ]
+    ]
 
 
 class DummyNode:
-    def __init__(self, _bytes):
-        if 'children' in _bytes:
-            self.children = _bytes['children']
-            self.grid = _bytes['grid']
+    def __init__(self, _bytes: _DummyNodeDictType) -> None:
+        if "children" in _bytes:
+            self.children: list[bytes] | None = _bytes["children"]
+            self.grid = _bytes["grid"]
         else:
             self.children = None
-            self.points = _bytes['points']
+            self.points = _bytes["points"]
 
 
 class Node:
     """docstring for Node"""
-    __slots__ = (
-        'name', 'aabb', 'aabb_size', 'inv_aabb_size', 'aabb_center',
-        'spacing', 'pending_xyz', 'pending_rgb', 'children', 'grid',
-        'points', 'dirty')
 
-    def __init__(self, name: bytes, aabb: np.ndarray, spacing: float) -> None:
+    __slots__ = (
+        "name",
+        "aabb",
+        "aabb_size",
+        "inv_aabb_size",
+        "aabb_center",
+        "spacing",
+        "pending_xyz",
+        "pending_rgb",
+        "pending_classification",
+        "children",
+        "grid",
+        "points",
+        "dirty",
+    )
+
+    def __init__(
+        self, name: bytes, aabb: npt.NDArray[np.float64 | np.float32], spacing: float
+    ) -> None:
         super().__init__()
         self.name = name
-        self.aabb = aabb.astype(np.float32)
-        self.aabb_size = np.maximum(aabb[1] - aabb[0], MIN_POINT_SIZE).astype(np.float32)
-        self.inv_aabb_size = (1.0 / self.aabb_size).astype(np.float32)
-        self.aabb_center = ((aabb[0] + aabb[1]) * 0.5).astype(np.float32)
+        self.aabb = aabb.astype(
+            np.float32
+        )  # TODO remove astype once the whole typing is done (and once data type issues on numpy arrays are fixed).
+        self.aabb_size = np.maximum(self.aabb[1] - self.aabb[0], MIN_POINT_SIZE)
+        self.inv_aabb_size = 1.0 / self.aabb_size
+        self.aabb_center = (self.aabb[0] + self.aabb[1]) * 0.5
         self.spacing = spacing
-        self.pending_xyz: list[npt.NDArray] = []
-        self.pending_rgb: list[npt.NDArray] = []
+        self.pending_xyz: list[npt.NDArray[np.float32]] = []
+        self.pending_rgb: list[npt.NDArray[np.uint8]] = []
+        self.pending_classification: list[npt.NDArray[np.uint8]] = []
         self.children: list[bytes] | None = None
         self.grid = Grid(self)
-        self.points: list[tuple[npt.NDArray, npt.NDArray]] = []
+        self.points: list[
+            tuple[npt.NDArray[np.float32], npt.NDArray[np.uint8], npt.NDArray[np.uint8]]
+        ] = []
         self.dirty = False
 
     def save_to_bytes(self) -> bytes:
-        sub_pickle = {}
+        sub_pickle: dict[str, Any] = {}
         if self.children is not None:
-            sub_pickle['children'] = self.children # type: ignore # TODO fix
-            sub_pickle['grid'] = self.grid # type: ignore # TODO fix
+            sub_pickle["children"] = self.children
+            sub_pickle["grid"] = self.grid
         else:
-            sub_pickle['points'] = self.points # type: ignore # TODO fix
+            sub_pickle["points"] = self.points
 
-        d = pickle.dumps(sub_pickle)
-        return d
+        return pickle.dumps(sub_pickle)
 
     def load_from_bytes(self, byt: bytes) -> None:
         sub_pickle = pickle.loads(byt)
-        if 'children' in sub_pickle:
-            self.children = sub_pickle['children']
-            self.grid = sub_pickle['grid']
+        if "children" in sub_pickle:
+            self.children = sub_pickle["children"]
+            self.grid = sub_pickle["grid"]
         else:
-            self.points = sub_pickle['points']
+            self.points = sub_pickle["points"]
 
-    def insert(self, node_catalog: NodeCatalog, scale: float, xyz: npt.NDArray, rgb: npt.NDArray, make_empty_node: bool = False):
+    def insert(
+        self,
+        scale: float,
+        xyz: npt.NDArray[np.float32],
+        rgb: npt.NDArray[np.uint8],
+        classification: npt.NDArray[np.uint8],
+        make_empty_node: bool = False,
+    ) -> None:
         if make_empty_node:
             self.children = []
             self.pending_xyz += [xyz]
             self.pending_rgb += [rgb]
+            self.pending_classification += [classification]
             return
 
         # fastpath
         if self.children is None:
-            self.points.append((xyz, rgb))
-            count = sum([xyz.shape[0] for xyz, rgb in self.points])
+            self.points.append((xyz, rgb, classification))
+            count = sum([xyz.shape[0] for xyz, rgb, classification in self.points])
             # stop subdividing if spacing is 1mm
             if count >= 20000 and self.spacing > 0.001 * scale:
-                self._split(node_catalog, scale)
+                self._split(scale)
             self.dirty = True
 
-            return True
+            return
 
         # grid based insertion
-        reminder_xyz, reminder_rgb, needs_balance = self.grid.insert(
-            self.aabb[0], self.inv_aabb_size, xyz, rgb)
+        (
+            remainder_xyz,
+            remainder_rgb,
+            remainder_classification,
+            needs_balance,
+        ) = self.grid.insert(self.aabb[0], self.inv_aabb_size, xyz, rgb, classification)
 
         if needs_balance:
             self.grid.balance(self.aabb_size, self.aabb[0], self.inv_aabb_size)
             self.dirty = True
 
-        self.dirty = self.dirty or (len(reminder_xyz) != len(xyz))
+        self.dirty = self.dirty or (len(remainder_xyz) != len(xyz))
 
-        if len(reminder_xyz) > 0:
-            self.pending_xyz += [reminder_xyz]
-            self.pending_rgb += [reminder_rgb]
+        if len(remainder_xyz) > 0:
+            self.pending_xyz += [remainder_xyz]
+            self.pending_rgb += [remainder_rgb]
+            self.pending_classification += [remainder_classification]
 
     def needs_balance(self) -> bool:
         if self.children is not None:
             return self.grid.needs_balance()
         return False
 
     def flush_pending_points(self, catalog: NodeCatalog, scale: float) -> None:
-        for name, xyz, rgb in self._get_pending_points():
-            catalog.get_node(name).insert(catalog, scale, xyz, rgb)
+        for name, xyz, rgb, classification in self._get_pending_points():
+            catalog.get_node(name).insert(scale, xyz, rgb, classification)
         self.pending_xyz = []
         self.pending_rgb = []
+        self.pending_classification = []
 
     def dump_pending_points(self) -> list[tuple[bytes, bytes, int]]:
         result = [
-            (name, pickle.dumps({'xyz': xyz, 'rgb': rgb}), len(xyz))
-            for name, xyz, rgb in self._get_pending_points()
+            (
+                name,
+                pickle.dumps(
+                    {"xyz": xyz, "rgb": rgb, "classification": classification}
+                ),
+                len(xyz),
+            )
+            for name, xyz, rgb, classification in self._get_pending_points()
         ]
 
         self.pending_xyz = []
         self.pending_rgb = []
+        self.pending_classification = []
         return result
 
     def get_pending_points_count(self) -> int:
         return sum([xyz.shape[0] for xyz in self.pending_xyz])
 
-    def _get_pending_points(self) -> Iterator[tuple[bytes, np.ndarray, np.ndarray]]:
+    def _get_pending_points(
+        self,
+    ) -> Iterator[
+        tuple[
+            bytes, npt.NDArray[np.float32], npt.NDArray[np.uint8], npt.NDArray[np.uint8]
+        ]
+    ]:
         if not self.pending_xyz:
             return
 
         pending_xyz_arr = np.concatenate(self.pending_xyz)
         pending_rgb_arr = np.concatenate(self.pending_rgb)
+        pending_classification_arr = np.concatenate(self.pending_classification)
         t = aabb_size_to_subdivision_type(self.aabb_size)
         if t == SubdivisionType.QUADTREE:
             indices = xyz_to_child_index(
                 pending_xyz_arr,
                 np.array(
                     [self.aabb_center[0], self.aabb_center[1], self.aabb[1][2]],
-                    dtype=np.float32)
+                    dtype=np.float32,
+                ),
             )
         else:
             indices = xyz_to_child_index(pending_xyz_arr, self.aabb_center)
 
         # unique children list
         childs = np.unique(indices)
 
         # make sure all children nodes exist
         for child in childs:
-            name = '{}{}'.format(self.name.decode('ascii'), child).encode('ascii')
+            name = "{}{}".format(self.name.decode("ascii"), child).encode("ascii")
             # create missing nodes, only for remembering they exist.
             # We don't want to serialize them
             # probably not needed...
-            if self.children is not None and name not in self.children :
+            if self.children is not None and name not in self.children:
                 self.children += [name]
                 self.dirty = True
                 # print('Added node {}'.format(name))
 
             mask = np.where(indices - child == 0)
             xyz = pending_xyz_arr[mask]
             if len(xyz) > 0:
-                yield name, xyz, pending_rgb_arr[mask]
+                yield name, xyz, pending_rgb_arr[mask], pending_classification_arr[mask]
 
-    def _split(self, node_catalog: NodeCatalog, scale: float) -> None:
+    def _split(self, scale: float) -> None:
         self.children = []
-        for xyz, rgb in self.points:
-            self.insert(node_catalog, scale, xyz, rgb)
+        for xyz, rgb, classification in self.points:
+            self.insert(scale, xyz, rgb, classification)
         self.points = []
 
-    def get_point_count(self, node_catalog: NodeCatalog, max_depth: int, depth: int = 0) -> int:
+    def get_point_count(
+        self, node_catalog: NodeCatalog, max_depth: int, depth: int = 0
+    ) -> int:
         if self.children is None:
-            return sum([xyz.shape[0] for xyz, rgb in self.points])
+            return sum([xyz.shape[0] for xyz, rgb, classification in self.points])
         else:
             count = self.grid.get_point_count()
             if depth < max_depth:
                 for n in self.children:
                     count += node_catalog.get_node(n).get_point_count(
-                        node_catalog, max_depth, depth + 1)
+                        node_catalog, max_depth, depth + 1
+                    )
             return count
 
     @staticmethod
-    def get_points(data: Node | DummyNode, include_rgb: bool) -> np.ndarray:  # todo remove staticmethod
+    def get_points(
+        data: Node | DummyNode, include_rgb: bool, include_classification: bool
+    ) -> npt.NDArray[np.uint8]:  # todo remove staticmethod
         if data.children is None:
             points = data.points
-            xyz = np.concatenate(tuple([xyz for xyz, rgb in points])).view(np.uint8).ravel()
+            xyz = (
+                np.concatenate(tuple([xyz for xyz, rgb, classification in points]))
+                .view(np.uint8)
+                .ravel()
+            )
+
             if include_rgb:
-                rgb = np.concatenate(tuple([rgb for xyz, rgb in points])).ravel()
-                result = np.concatenate((xyz, rgb))
-                return result
+                rgb = np.concatenate(
+                    tuple([rgb for xyz, rgb, classification in points])
+                ).ravel()
             else:
-                return xyz
+                rgb = np.array([], dtype=np.uint8)
+
+            if include_classification:
+                classification = np.concatenate(
+                    tuple([classification for xyz, rgb, classification in points])
+                ).ravel()
+            else:
+                classification = np.array([], dtype=np.uint8)
+
+            return np.concatenate((xyz, rgb, classification))
         else:
-            return data.grid.get_points(include_rgb)
+            return data.grid.get_points(include_rgb, include_classification)
 
-    @staticmethod
-    def to_tileset(executor: concurrent.futures.ProcessPoolExecutor | None,
-                   name: bytes,
-                   parent_aabb: np.ndarray,
-                   parent_spacing: float,
-                   folder: Path,
-                   scale: np.ndarray,
-                   prune: bool = True) -> dict:
-        node = node_from_name(name, parent_aabb, parent_spacing)
-        aabb = node.aabb
-        tile_path = node_name_to_path(folder, name, '.pnts')
-        xyz = np.array(0)
-        rgb = np.array(0)
-
-        # Read tile's pnts file, if existing, we'll need it for:
-        #   - computing the real AABB (instead of the one based on the octree)
-        #   - merging this tile's small (<100 points) children
-        if tile_path.exists():
-            tile = TileContentReader.read_file(tile_path)
+    def get_child_names(self) -> Generator[bytes, None, None]:
+        for number_child in range(8):
+            yield f"{self.name.decode('ascii')}{number_child}".encode("ascii")
+
+    def to_tileset(
+        self,
+        folder: Path,
+        scale: npt.NDArray[np.float32],
+        parent_node: Node | None = None,
+        depth: int = 0,
+        pool_executor: ProcessPoolExecutor | None = None,
+    ) -> TileDictType | None:
+        # create child tileset parts
+        # if their size is below of 100 points, they will be merged in this node.
+        children_tileset_parts: list[TileDictType] = []
+        parameter_to_compute: list[
+            tuple[Node, Path, npt.NDArray[np.float32], Node, int]
+        ] = []
+        for child_name in self.get_child_names():
+            child_node = node_from_name(child_name, self.aabb, self.spacing)
+            child_pnts_path = node_name_to_path(folder, child_name, ".pnts")
+
+            if child_pnts_path.exists():
+                # multi thread is only allowed on nodes where there are no prune
+                # a simple rule is: only is there is not a parent node
+                if pool_executor and parent_node is None:
+                    parameter_to_compute.append(
+                        (child_node, folder, scale, self, depth + 1)
+                    )
+                else:
+                    children_tileset_part = child_node.to_tileset(
+                        folder, scale, self, depth + 1
+                    )
+                    if (
+                        children_tileset_part is not None
+                    ):  # return None if the child has been merged
+                        children_tileset_parts.append(children_tileset_part)
+
+        if pool_executor and parent_node is None:
+            children_tileset_parts = [
+                t
+                for t in pool_executor.map(node_to_tileset, parameter_to_compute)
+                if t is not None
+            ]
+
+        pnts_path = node_name_to_path(folder, self.name, ".pnts")
+        tile = read_binary_tile_content(pnts_path)
+        fth = tile.body.feature_table.header
+        xyz = tile.body.feature_table.body.position
+
+        # check if this node should be merged in the parent.
+        prune = False  # prune only if the node is a leaf
+
+        # If this child is small enough, merge in the current tile
+        if parent_node is not None and depth > 1 and fth.points_length < 100:
+            parent_pnts_path = node_name_to_path(folder, parent_node.name, ".pnts")
+            parent_tile = read_binary_tile_content(parent_pnts_path)
+            parent_fth = parent_tile.body.feature_table.header
+
+            parent_xyz = parent_tile.body.feature_table.body.position
+
+            if (
+                parent_fth.colors != SemanticPoint.NONE
+                and parent_tile.body.feature_table.body.color is not None
+            ):
+                parent_rgb = parent_tile.body.feature_table.body.color
+            else:
+                parent_rgb = np.array([], dtype=np.uint8)
+
+            if "Classification" in parent_tile.body.batch_table.header.data:
+                parent_classification = (
+                    parent_tile.body.batch_table.get_binary_property("Classification")
+                )
+            else:
+                parent_classification = np.array([], dtype=np.uint8)
+
+            parent_xyz_float = parent_xyz.reshape((parent_fth.points_length, 3))
+            # update aabb based on real values
+            parent_aabb = np.array(
+                [
+                    np.amin(parent_xyz_float, axis=0),
+                    np.amax(parent_xyz_float, axis=0),
+                ]
+            )
+
+            parent_xyz = np.concatenate((parent_xyz, xyz))
 
-            fth = tile.body.feature_table.header
-            xyz = tile.body.feature_table.body.positions_arr
             if fth.colors != SemanticPoint.NONE:
-                rgb = tile.body.feature_table.body.colors_arr
+                if tile.body.feature_table.body.color is None:
+                    raise TilerException(
+                        "If the parent has color data, the children must also have color data."
+                    )
+                parent_rgb = np.concatenate(
+                    (parent_rgb, tile.body.feature_table.body.color)
+                )
+
+            if "Classification" in tile.body.batch_table.header.data:
+                parent_classification = np.concatenate(
+                    (
+                        parent_classification,
+                        tile.body.batch_table.get_binary_property("Classification"),
+                    )
+                )
+
+            # update aabb
+            xyz_float = xyz.view(np.float32).reshape((fth.points_length, 3))
+
+            parent_aabb[0] = np.amin(
+                [parent_aabb[0], np.min(xyz_float, axis=0)], axis=0
+            )
+            parent_aabb[1] = np.amax(
+                [parent_aabb[1], np.max(xyz_float, axis=0)], axis=0
+            )
+
+            parent_pnts_path.unlink()
+            points_to_pnts_file(
+                parent_node.name,
+                np.concatenate(
+                    (parent_xyz.view(np.uint8), parent_rgb, parent_classification)
+                ),
+                folder,
+                len(parent_rgb) != 0,
+                len(parent_classification) != 0,
+            )
+            pnts_path.unlink()
+            prune = True
+
+        content: ContentType | None = None
+        if not prune:
+            content = {"uri": str(pnts_path.relative_to(folder))}
             xyz_float = xyz.view(np.float32).reshape((fth.points_length, 3))
+
             # update aabb based on real values
-            aabb = np.array([
-                np.amin(xyz_float, axis=0),
-                np.amax(xyz_float, axis=0)])
-
-        # geometricError is in meters, so we divide it by the scale
-        tileset = {'geometricError': 10 * node.spacing / scale[0]}
-
-        children: list[Any] = [] # todo at the next refacto, fix it
-        tile_needs_rewrite = False
-        if tile_path.exists():
-            tileset['content'] = {'uri': str(tile_path.relative_to(folder))}
-        for child in ['0', '1', '2', '3', '4', '5', '6', '7']:
-            child_name = '{}{}'.format(
-                name.decode('ascii'),
-                child
-            ).encode('ascii')
-            child_tile_path = node_name_to_path(folder, child_name, '.pnts')
-
-            if child_tile_path.exists():
-                # See if we should merge this child in tile
-                if len(xyz):
-                    # Read pnts content
-                    tile = TileContentReader.read_file(child_tile_path)
-
-                    fth = tile.body.feature_table.header
-
-                    # If this child is small enough, merge in the current tile.
-                    # prune should be set at False is the refine mode is REPLACE.
-                    # In some cases, we cannot know which point in the parent tile should be deleted
-                    # (for example when 2 points are at the same location)
-                    if prune and fth.points_length < 100:
-                        xyz = np.concatenate(
-                            (xyz,
-                             tile.body.feature_table.body.positions_arr))
-
-                        if fth.colors != SemanticPoint.NONE:
-                            rgb = np.concatenate(
-                                (rgb,
-                                 tile.body.feature_table.body.colors_arr))
-
-                        # update aabb
-                        xyz_float = tile.body.feature_table.body.positions_arr.view(
-                            np.float32).reshape((fth.points_length, 3))
-
-                        aabb[0] = np.amin(
-                            [aabb[0], np.min(xyz_float, axis=0)], axis=0)
-                        aabb[1] = np.amax(
-                            [aabb[1], np.max(xyz_float, axis=0)], axis=0)
-
-                        tile_needs_rewrite = True
-                        child_tile_path.unlink()
-                        continue
-
-                # Add child to the to-be-processed list if it hasn't been merged
-                if executor is not None:
-                    children += [(child_name, node.aabb, node.spacing, folder, scale)]
+            aabb = np.array([np.amin(xyz_float, axis=0), np.amax(xyz_float, axis=0)])
+
+            center = ((aabb[0] + aabb[1]) * 0.5).tolist()
+            half_size = ((aabb[1] - aabb[0]) * 0.5).tolist()
+            bounding_volume: BoundingVolumeBoxDictType = {
+                "box": [
+                    center[0],
+                    center[1],
+                    center[2],
+                    half_size[0],
+                    0,
+                    0,
+                    0,
+                    half_size[1],
+                    0,
+                    0,
+                    0,
+                    half_size[2],
+                ]
+            }
+        else:
+            # if it is a leaf that should be pruned
+            if not children_tileset_parts:
+                return None
+
+            # recompute the aabb in function of children
+            aabb = None
+            for child_tileset_part in children_tileset_parts:
+                bounding_box = child_tileset_part["boundingVolume"].get("box")
+                if not isinstance(bounding_box, list):
+                    raise ValueError("bounding_box must be a list")
+                if bounding_box is None:
+                    raise NotImplementedError(
+                        "bounding_box can only be a bounding volume box"
+                    )
+
+                center = np.array(bounding_box[:3])
+                half_size = np.array(bounding_box[3::4])
+
+                child_aabb = np.array([center + half_size, center - half_size])
+
+                if aabb is None:
+                    aabb = child_aabb
                 else:
-                    children += [Node.to_tileset(None, child_name, node.aabb, node.spacing, folder, scale)]
+                    aabb[0] = np.amin([aabb[0], child_aabb[0]], axis=0)
+                    aabb[1] = np.amax([aabb[1], child_aabb[1]], axis=0)
 
-        # If we merged at least one child tile in the current tile
-        # the pnts file needs to be rewritten.
-        if tile_needs_rewrite:
-            tile_path.unlink()
-            points_to_pnts(name, np.concatenate((xyz, rgb)), folder, len(rgb) != 0)
-
-        center = ((aabb[0] + aabb[1]) * 0.5).tolist()
-        half_size = ((aabb[1] - aabb[0]) * 0.5).tolist()
-        tileset['boundingVolume'] = {
-            'box': [
-                center[0], center[1], center[2],
-                half_size[0], 0, 0,
-                0, half_size[1], 0,
-                0, 0, half_size[2]]
-        }
+            if aabb is None:
+                raise TilerException("aabb shouldn't be None")
 
-        if executor is not None:
-            children = [t for t in executor.map(node_to_tileset, children)]
+            center = ((aabb[0] + aabb[1]) * 0.5).tolist()
+            half_size = ((aabb[1] - aabb[0]) * 0.5).tolist()
+            bounding_volume = {
+                "box": [
+                    center[0],
+                    center[1],
+                    center[2],
+                    half_size[0],
+                    0,
+                    0,
+                    0,
+                    half_size[1],
+                    0,
+                    0,
+                    0,
+                    half_size[2],
+                ]
+            }
+
+        tileset: TileDictType = {
+            "boundingVolume": bounding_volume,
+            "geometricError": 10 * self.spacing / scale[0],
+        }
+        if content is not None:
+            tileset["content"] = content
 
-        if children:
-            tileset['children'] = children
+        if children_tileset_parts:
+            tileset["children"] = children_tileset_parts
         else:
-            tileset['geometricError'] = 0.0
+            tileset["geometricError"] = 0.0
 
-        if len(name) > 0 and children:
-            if len(json.dumps(tileset)) > 100000:
-                tile_root = {
-                    'asset': {
-                        'version': '1.0',
-                    },
-                    'refine': 'ADD',
-                    'geometricError': tileset['geometricError'],
-                    'root': tileset
-                }
-                tileset_name = f"tileset.{name.decode('ascii')}.json"
-                tileset_path = folder / tileset_name
-                with tileset_path.open('w') as f:
-                    json.dump(tile_root, f)
-                tileset['content'] = {'uri': tileset_name}
-                del tileset['children']
+        if (
+            len(self.name) > 0
+            and children_tileset_parts
+            and len(json.dumps(tileset)) > 100000
+        ):
+            tileset = split_tileset(tileset, self.name.decode(), folder)
 
         return tileset
+
+
+def split_tileset(
+    tile_dict: TileDictType, split_name: str, folder: Path
+) -> TileDictType:
+    tileset = {
+        "asset": {
+            "version": "1.0",
+        },
+        "refine": "ADD",
+        "geometricError": tile_dict["geometricError"],
+        "root": tile_dict,
+    }
+    tileset_name = f"tileset.{split_name}.json"
+    with (folder / tileset_name).open("w") as f:
+        f.write(json.dumps(tileset))
+    tile_dict["content"] = {"uri": tileset_name}
+    del tile_dict["children"]
+
+    return tile_dict
```

### Comparing `py3dtiles-5.0.0/py3dtiles/tilers/node/node_catalog.py` & `py3dtiles-6.0.0/py3dtiles/tilers/node/node_catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,27 @@
 
 import lz4.frame as gzip
 
 from py3dtiles.tilers.node.node import Node
 from py3dtiles.utils import split_aabb
 
 if TYPE_CHECKING:
-    from py3dtiles.convert import OctreeMetadata
+    from py3dtiles.utils import OctreeMetadata
 
 
 class NodeCatalog:
     """NodeCatalog is a store of Node objects.py3dtiles
 
     Using a NodeCatalog allows to only store a children names
     in nodes, instead of storing a full recursive structure.
     """
 
-    def __init__(self, nodes: bytes, name: bytes, octree_metadata: OctreeMetadata) -> None:
+    def __init__(
+        self, nodes: bytes, name: bytes, octree_metadata: OctreeMetadata
+    ) -> None:
         self.nodes: dict[bytes, Node] = {}
         self.root_aabb = octree_metadata.aabb
         self.root_spacing = octree_metadata.spacing
         self.node_bytes: dict[bytes, bytes] = {}
         self._load_from_store(name, nodes)
 
     def get_node(self, name: bytes) -> Node:
```

### Comparing `py3dtiles-5.0.0/py3dtiles/tilers/node/shared_node_store.py` & `py3dtiles-6.0.0/py3dtiles/tilers/node/shared_node_store.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,89 +2,99 @@
 from pathlib import Path
 from sys import getsizeof
 import time
 from typing import Dict, List, Tuple
 
 import lz4.frame as gzip
 
+from py3dtiles.exceptions import TilerException
 from py3dtiles.utils import node_name_to_path
 
 
 class SharedNodeStore:
     def __init__(self, folder: Path) -> None:
         self.metadata: Dict[bytes, Tuple[float, int] | None] = {}
         self.data: List[bytes | None] = []
         self.folder = folder
         self.stats = {
-            'hit': 0,
-            'miss': 0,
-            'new': 0,
+            "hit": 0,
+            "miss": 0,
+            "new": 0,
         }
         self.memory_size = {
-            'content': 0,
-            'container': getsizeof(self.data) + getsizeof(self.metadata),
+            "content": 0,
+            "container": getsizeof(self.data) + getsizeof(self.metadata),
         }
 
     def control_memory_usage(self, max_size_mb: int, verbose: int) -> None:
         bytes_to_mb = 1.0 / (1024 * 1024)
         max_size_mb = max(max_size_mb, 200)
 
         if verbose >= 3:
             self.print_statistics()
 
         # guess cache size
-        cache_size = (self.memory_size['container'] + self.memory_size['content']) * bytes_to_mb
+        cache_size = (
+            self.memory_size["container"] + self.memory_size["content"]
+        ) * bytes_to_mb
 
         before = cache_size
         if before < max_size_mb:
             return
 
         if verbose >= 2:
-            print(f'>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>> CACHE CLEANING [{before}]')
+            print(f">>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>> CACHE CLEANING [{before}]")
         self.remove_oldest_nodes(1 - max_size_mb / before)
         gc.collect()
 
         if verbose >= 2:
-            print('<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<< CACHE CLEANING')
+            print("<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<< CACHE CLEANING")
 
     def get(self, name: bytes, stat_inc: int = 1) -> bytes:
         metadata = self.metadata.get(name, None)
-        data = b''
+        data = b""
         if metadata is not None:
             tmp_data = self.data[metadata[1]]
             if tmp_data is None:
-                raise RuntimeError("tmp_data shouldn't be None if metadata is not None.")
+                raise TilerException(
+                    "tmp_data shouldn't be None if metadata is not None."
+                )
             else:
                 data = tmp_data
-            self.stats['hit'] += stat_inc
+            self.stats["hit"] += stat_inc
         else:
             node_path = node_name_to_path(self.folder, name)
             if node_path.exists():
-                self.stats['miss'] += stat_inc
-                with node_path.open('rb') as f:
+                self.stats["miss"] += stat_inc
+                with node_path.open("rb") as f:
                     data = f.read()
             else:
-                self.stats['new'] += stat_inc
+                self.stats["new"] += stat_inc
             #  should we cache this node?
 
         return data
 
     def remove(self, name: bytes) -> None:
         meta = self.metadata.pop(name, None)
 
         node_path = node_name_to_path(self.folder, name)
         if meta is None:
             if not node_path.exists():
                 raise FileNotFoundError(f"{node_path} should exist")
         else:
-            self.memory_size['content'] -= getsizeof(meta)
-            if self.data[meta[1]] is None:
-                raise ValueError(f"{name!r} is present in self.metadata but not in self.data.")
-            self.memory_size['content'] -= len(self.data[meta[1]]) # type: ignore
-            self.memory_size['container'] = getsizeof(self.data) + getsizeof(self.metadata)
+            self.memory_size["content"] -= getsizeof(meta)
+            content = self.data[meta[1]]
+            if content is None:
+                raise TilerException(
+                    f"{name!r} is present in self.metadata but not in self.data."
+                )
+            self.memory_size["content"] -= len(content)
+            self.memory_size["container"] = getsizeof(self.data) + getsizeof(
+                self.metadata
+            )
             self.data[meta[1]] = None
 
         if node_path.exists():
             node_path.unlink()
 
     def put(self, name: bytes, data: bytes) -> None:
         compressed_data = gzip.compress(data)
@@ -94,43 +104,48 @@
             metadata = (time.time(), len(self.data))
             self.data.append(compressed_data)
         else:
             metadata = (time.time(), metadata[1])
             self.data[metadata[1]] = compressed_data
         self.metadata.update([(name, metadata)])
 
-        self.memory_size['content'] += len(compressed_data) + getsizeof((name, metadata))
-        self.memory_size['container'] = getsizeof(self.data) + getsizeof(self.metadata)
+        self.memory_size["content"] += len(compressed_data) + getsizeof(
+            (name, metadata)
+        )
+        self.memory_size["container"] = getsizeof(self.data) + getsizeof(self.metadata)
 
     def remove_oldest_nodes(self, percent: float = 100) -> Tuple[int, int]:
         count = _remove_all(self)
 
-        self.memory_size['content'] = 0
-        self.memory_size['container'] = getsizeof(self.data) + getsizeof(self.metadata)
+        self.memory_size["content"] = 0
+        self.memory_size["container"] = getsizeof(self.data) + getsizeof(self.metadata)
 
         return count
 
     def print_statistics(self) -> None:
-        print('Stats: Hits = {}, Miss = {}, New = {}'.format(
-            self.stats['hit'],
-            self.stats['miss'],
-            self.stats['new']))
+        print(
+            "Stats: Hits = {}, Miss = {}, New = {}".format(
+                self.stats["hit"], self.stats["miss"], self.stats["new"]
+            )
+        )
 
 
 def _remove_all(store: SharedNodeStore) -> Tuple[int, int]:
     # delete the entries
     count = len(store.metadata)
     bytes_written = 0
     for name, meta in store.metadata.items():
         if meta is None:
             continue
         data = store.data[meta[1]]
         if data is None:
-            raise ValueError(f"{name!r} is present in self.metadata but not in self.data.")
+            raise TilerException(
+                f"{name!r} is present in self.metadata but not in self.data."
+            )
         node_path = node_name_to_path(store.folder, name)
-        with node_path.open('wb') as f:
+        with node_path.open("wb") as f:
             bytes_written += f.write(data)
 
     store.metadata = {}
     store.data = []
 
     return count, bytes_written
```

### Comparing `py3dtiles-5.0.0/py3dtiles/tileset/bounding_volume_box.py` & `py3dtiles-6.0.0/py3dtiles/tileset/bounding_volume_box.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from __future__ import annotations
 
 import copy
-from typing import TYPE_CHECKING
+from typing import Any, TYPE_CHECKING
 
 import numpy as np
 import numpy.typing as npt
 
+from py3dtiles.exceptions import TilerException
 from py3dtiles.typing import BoundingVolumeBoxDictType
 from .bounding_volume import BoundingVolume
 
 if TYPE_CHECKING:
     from .tile import Tile
+    from typing_extensions import Self
 
 # In order to prevent the appearance of ghost newline characters ("\n")
 # when printing a numpy.array (mainly self._box in this file):
 np.set_printoptions(linewidth=500)
 
 
-class BoundingVolumeBox(BoundingVolume):
+class BoundingVolumeBox(BoundingVolume[BoundingVolumeBoxDictType]):
     """
     A box bounding volume as defined in the 3DTiles specifications i.e. an
     array of 12 numbers that define an oriented bounding box:
     - The first three elements define the x, y, and z values for the
     center of the box.
     - The next three elements (with indices 3, 4, and 5) define the x axis
     direction and half-length.
@@ -41,59 +43,67 @@
     box i.e. a box that is parallel to the coordinate axis.
     """
 
     def __init__(self) -> None:
         super().__init__()
         self._box: npt.NDArray[np.float64] | None = None
 
+    @classmethod
+    def from_dict(cls, bounding_volume_box_dict: BoundingVolumeBoxDictType) -> Self:
+        bounding_volume_box = cls()
+        bounding_volume_box.set_from_list(bounding_volume_box_dict["box"])
+
+        bounding_volume_box.set_properties_from_dict(bounding_volume_box_dict)
+
+        return bounding_volume_box
+
     def get_center(self) -> npt.NDArray[np.float64]:
         if self._box is None:
-            raise AttributeError('Bounding Volume Box is not defined.')
+            raise AttributeError("Bounding Volume Box is not defined.")
 
-        return self._box[0: 3]
+        return self._box[0:3]
 
     def translate(self, offset: npt.NDArray[np.float64]) -> None:
         """
         Translate the box center with the given offset "vector"
         :param offset: the 3D vector by which the box should be translated
         """
         if self._box is None:
-            raise AttributeError('Bounding Volume Box is not defined.')
+            raise AttributeError("Bounding Volume Box is not defined.")
 
         self._box[:3] += offset[:3]
 
     def transform(self, transform: npt.NDArray[np.float64]) -> None:
         """
         Apply the provided transformation matrix (4x4) to the box
         :param transform: transformation matrix (4x4) to be applied
         """
         if self._box is None:
-            raise AttributeError('Bounding Volume Box is not defined.')
+            raise AttributeError("Bounding Volume Box is not defined.")
+
+        transform = transform.flatten()
 
         # FIXME: the following code only uses the first three coordinates
         # of the transformation matrix (and basically ignores the fourth
         # column of transform). This looks like some kind of mistake...
-        rotation = np.array([transform[0:3],
-                             transform[4:7],
-                             transform[8:11]])
-
-        center = self._box[0: 3]
-        x_half_axis = self._box[3: 6]
-        y_half_axis = self._box[6: 9]
+        rotation = np.array([transform[0:3], transform[4:7], transform[8:11]])
+
+        center = self._box[0:3]
+        x_half_axis = self._box[3:6]
+        y_half_axis = self._box[6:9]
         z_half_axis = self._box[9:12]
 
         # Apply the rotation part to each element
         new_center = rotation.dot(center)
         new_x_half_axis = rotation.dot(x_half_axis)
         new_y_half_axis = rotation.dot(y_half_axis)
         new_z_half_axis = rotation.dot(z_half_axis)
-        self._box = np.concatenate((new_center,
-                                    new_x_half_axis,
-                                    new_y_half_axis,
-                                    new_z_half_axis))
+        self._box = np.concatenate(
+            (new_center, new_x_half_axis, new_y_half_axis, new_z_half_axis)
+        )
         offset = transform[12:15]
         self.translate(offset)
 
     def is_box(self) -> bool:
         return True
 
     def set_from_list(self, box_list: npt.ArrayLike) -> None:
@@ -121,134 +131,141 @@
         self._box = BoundingVolumeBox.get_box_array_from_mins_maxs(mins_maxs)
 
     def get_corners(self) -> list[npt.NDArray[np.float64]]:
         """
         :return: the corners (3D points) of the box as a list
         """
         if self._box is None:
-            raise AttributeError('Bounding Volume Box is not defined.')
+            raise AttributeError("Bounding Volume Box is not defined.")
 
-        center = self._box[0: 3: 1]
-        x_half_axis = self._box[3: 6: 1]
-        y_half_axis = self._box[6: 9: 1]
-        z_half_axis = self._box[9:12: 1]
+        center, x_half_axis, y_half_axis, z_half_axis = self._box.reshape([-1, 3])
 
         x_axis = x_half_axis * 2
         y_axis = y_half_axis * 2
         z_axis = z_half_axis * 2
 
         # The eight cornering points of the box
-        tmp = np.subtract(center, x_half_axis)
-        tmp = np.subtract(tmp, y_half_axis)
+        origin = center - x_half_axis - y_half_axis - z_half_axis
 
-        o = np.subtract(tmp, z_half_axis)
-        ox = np.add(o, x_axis)
-        oy = np.add(o, y_axis)
-        oxy = np.add(o, np.add(x_axis, y_axis))
-
-        oz = np.add(o, z_axis)
-        oxz = np.add(oz, x_axis)
-        oyz = np.add(oz, y_axis)
-        oxyz = np.add(oz, np.add(x_axis, y_axis))
+        ox = origin + x_axis
+        oy = origin + y_axis
+        oz = origin + z_axis
+        oxy = ox + y_axis
+        oxz = ox + z_axis
+        oyz = oy + z_axis
+        oxyz = oxy + z_axis
 
-        return [o, ox, oy, oxy, oz, oxz, oyz, oxyz]
+        return [origin, ox, oy, oxy, oz, oxz, oyz, oxyz]
 
     def get_canonical_as_array(self) -> npt.NDArray[np.float64]:
         """
         :return: the smallest enclosing box (as an array) that is parallel
                  to the coordinate axis
         """
         return BoundingVolumeBox.get_box_array_from_point(self.get_corners())
 
-    def add(self, other: BoundingVolume) -> None:
+    def add(self, other: BoundingVolume[Any]) -> None:
         """
         Compute the 'canonical' bounding volume fitting this bounding volume
         together with the added bounding volume. Again (refer above to the
         class definition) the computed fitting bounding volume is generically
         not the smallest one (due to its alignment with the coordinate axis).
         :param other: another box bounding volume to be added with this one
         """
         if not isinstance(other, BoundingVolumeBox):
-            raise NotImplementedError("The add method works only with BoundingVolumeBox")
+            raise NotImplementedError(
+                "The add method works only with BoundingVolumeBox"
+            )
 
         if self._box is None:
             # Then it is safe to overwrite
-            self._box = other._box
+            self._box = copy.deepcopy(other._box)
             return
 
         corners = self.get_corners() + other.get_corners()
         self.set_from_points(corners)
 
     def sync_with_children(self, owner: Tile) -> None:
         # We reset to some dummy state of this Bounding Volume Box so we
         # can add up in place the boxes of the owner's children
         # If there is no child, no modifications are done.
-        for child in owner.get_direct_children():
+        for child in owner.children:
             if child.bounding_volume is None:
-                raise ValueError("Child should have a bounding volume.")
+                raise TilerException("Child should have a bounding volume.")
 
             bounding_volume = copy.deepcopy(child.bounding_volume)
             bounding_volume.transform(child.transform)
             if not bounding_volume.is_box():
-                raise AttributeError("All children should also have a box as bounding volume"
-                                     "if the parent has a bounding box")
+                raise TilerException(
+                    "All children must also have a box as bounding volume "
+                    "if the parent has a bounding box"
+                )
             self.add(bounding_volume)
 
     def to_dict(self) -> BoundingVolumeBoxDictType:
         if self._box is None:
-            raise AttributeError('Bounding Volume Box is not defined.')
+            raise AttributeError("Bounding Volume Box is not defined.")
 
-        return {'box': list(self._box)}
+        dict_data: BoundingVolumeBoxDictType = {"box": list(self._box)}
+        return self.add_root_properties_to_dict(dict_data)
 
     @staticmethod
-    def get_box_array_from_mins_maxs(mins_maxs: npt.NDArray[np.float64]) -> npt.NDArray[np.float64]:
+    def get_box_array_from_mins_maxs(
+        mins_maxs: npt.NDArray[np.float64],
+    ) -> npt.NDArray[np.float64]:
         """
         :param mins_maxs: the list [x_min, y_min, z_min, x_max, y_max, z_max]
                           that is the boundaries of the box along each
                           coordinate axis
         :return: the smallest box (as an array, as opposed to a
                 BoundingVolumeBox instance) that encloses the given list of
                 (3D) points and that is parallel to the coordinate axis.
         """
         x_min = mins_maxs[0]
         x_max = mins_maxs[3]
         y_min = mins_maxs[1]
         y_max = mins_maxs[4]
         z_min = mins_maxs[2]
         z_max = mins_maxs[5]
-        new_center = np.array([(x_min + x_max) / 2,
-                               (y_min + y_max) / 2,
-                               (z_min + z_max) / 2])
+        new_center = np.array(
+            [(x_min + x_max) / 2, (y_min + y_max) / 2, (z_min + z_max) / 2]
+        )
         new_x_half_axis = np.array([(x_max - x_min) / 2, 0, 0])
         new_y_half_axis = np.array([0, (y_max - y_min) / 2, 0])
         new_z_half_axis = np.array([0, 0, (z_max - z_min) / 2])
 
-        return np.concatenate((new_center,
-                               new_x_half_axis,
-                               new_y_half_axis,
-                               new_z_half_axis))
+        return np.concatenate(
+            (new_center, new_x_half_axis, new_y_half_axis, new_z_half_axis)
+        )
 
     @staticmethod
-    def get_box_array_from_point(points: list[npt.NDArray[np.float64]]) -> npt.NDArray[np.float64]:
+    def get_box_array_from_point(
+        points: list[npt.NDArray[np.float64]],
+    ) -> npt.NDArray[np.float64]:
         """
         :param points: a list of 3D points
         :return: the smallest box (as an array, as opposed to a
                 BoundingVolumeBox instance) that encloses the given list of
                 (3D) points and that is parallel to the coordinate axis.
         """
         return BoundingVolumeBox.get_box_array_from_mins_maxs(
-            np.array([min(c[0] for c in points),
-             min(c[1] for c in points),
-             min(c[2] for c in points),
-             max(c[0] for c in points),
-             max(c[1] for c in points),
-             max(c[2] for c in points)]))
+            np.array(
+                [
+                    min(c[0] for c in points),
+                    min(c[1] for c in points),
+                    min(c[2] for c in points),
+                    max(c[0] for c in points),
+                    max(c[1] for c in points),
+                    max(c[2] for c in points),
+                ]
+            )
+        )
 
     @staticmethod
     def is_valid(box: npt.NDArray[np.float64]) -> tuple[bool, str]:
         if box is None:
-            return False, 'Bounding Volume Box is not defined.'
-        if not box.ndim == 1:
-            return False, 'Bounding Volume Box has wrong dimensions.'
-        if not box.shape[0] == 12:
-            return False, 'Warning: Bounding Volume Box must have 12 elements.'
+            return False, "Bounding Volume Box is not defined."
+        if box.ndim != 1:
+            return False, "Bounding Volume Box has wrong dimensions."
+        if box.shape[0] != 12:
+            return False, "Warning: Bounding Volume Box must have 12 elements."
         return True, ""
```

### Comparing `py3dtiles-5.0.0/py3dtiles/tileset/content/b3dm.py` & `py3dtiles-6.0.0/py3dtiles/tileset/content/b3dm.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,206 +1,196 @@
-import json
+from __future__ import annotations
+
 import struct
 
 import numpy as np
+import numpy.typing as npt
 
-from py3dtiles.tileset.batch_table import BatchTable
-from py3dtiles.tileset.tile_content import TileContent, TileContentBody, TileContentHeader, TileContentType
+from py3dtiles.exceptions import InvalidB3dmError
+from .batch_table import BatchTable
 from .gltf import GlTF
+from .tile_content import (
+    TileContent,
+    TileContentBody,
+    TileContentHeader,
+)
 
 
 class B3dm(TileContent):
+    def __init__(self, header: B3dmHeader, body: B3dmBody) -> None:
+        super().__init__()
 
-    @staticmethod
-    def from_glTF(gltf, bt=None):
+        self.header: B3dmHeader = header
+        self.body: B3dmBody = body
+
+    def sync(self) -> None:
         """
-        Parameters
-        ----------
-        gltf : GlTF
-            glTF object representing a set of objects
-
-        bt : Batch Table (optional)
-            BatchTable object containing per-feature metadata
-
-        Returns
-        -------
-        tile : TileContent
+        Allow to synchronize headers with contents.
         """
 
-        tb = B3dmBody()
-        tb.glTF = gltf
-        tb.batch_table = bt
-
-        th = B3dmHeader()
-        th.sync(tb)
-
-        t = TileContent()
-        t.body = tb
-        t.header = th
+        # extract array
+        gltf_arr = self.body.gltf.to_array()
 
-        return t
+        # sync the tile header with feature table contents
+        self.header.tile_byte_length = len(gltf_arr) + B3dmHeader.BYTE_LENGTH
+        self.header.bt_json_byte_length = 0
+        self.header.bt_bin_byte_length = 0
+        self.header.ft_json_byte_length = 0
+        self.header.ft_bin_byte_length = 0
+
+        if self.body.batch_table is not None:
+            bth_arr = self.body.batch_table.to_array()
+
+            self.header.tile_byte_length += len(bth_arr)
+            self.header.bt_json_byte_length = len(bth_arr)
+
+    def print_info(self) -> None:
+        if self.header:
+            th = self.header
+            print("Tile Header")
+            print("-----------")
+            print("Magic Value: ", th.magic_value)
+            print("Version: ", th.version)
+            print("Tile byte length: ", th.tile_byte_length)
+            print("Feature table json byte length: ", th.ft_json_byte_length)
+            print("Feature table bin byte length: ", th.ft_bin_byte_length)
+            print("Batch table json byte length: ", th.bt_json_byte_length)
+            print("Batch table bin byte length: ", th.bt_bin_byte_length)
+        else:
+            print("Tile with no header")
+
+        if self.body:
+            gltf_header = self.body.gltf.header
+            print("")
+            print("glTF Header")
+            print("-----------")
+            print(gltf_header)
+        else:
+            print("Tile with no body")
 
     @staticmethod
-    def from_array(array):
-        """
-        Parameters
-        ----------
-        array : numpy.array
-
-        Returns
-        -------
-        t : TileContent
-        """
+    def from_gltf(gltf: GlTF, batch_table: BatchTable | None = None) -> B3dm:
+        b3dm_body = B3dmBody()
+        b3dm_body.gltf = gltf
+        if batch_table is not None:
+            b3dm_body.batch_table = batch_table
+
+        b3dm_header = B3dmHeader()
+        b3dm = B3dm(b3dm_header, b3dm_body)
+        b3dm.sync()
 
+        return b3dm
+
+    @staticmethod
+    def from_array(array: npt.NDArray[np.uint8]) -> B3dm:
         # build tile header
-        h_arr = array[0:B3dmHeader.BYTE_LENGTH]
-        h = B3dmHeader.from_array(h_arr)
+        h_arr = array[0 : B3dmHeader.BYTE_LENGTH]
+        b3dm_header = B3dmHeader.from_array(h_arr)
 
-        if h.tile_byte_length != len(array):
-            raise RuntimeError("Invalid byte length in header")
+        if b3dm_header.tile_byte_length != len(array):
+            raise InvalidB3dmError(
+                f"Invalid byte length in header, the size of array is {len(array)}, "
+                f"the tile_byte_length for header is {b3dm_header.tile_byte_length}"
+            )
 
         # build tile body
-        b_arr = array[B3dmHeader.BYTE_LENGTH:h.tile_byte_length]
-        b = B3dmBody.from_array(h, b_arr)
+        b_arr = array[B3dmHeader.BYTE_LENGTH : b3dm_header.tile_byte_length]
+        b3dm_body = B3dmBody.from_array(b3dm_header, b_arr)
 
-        # build TileContent with header and body
-        t = TileContent()
-        t.header = h
-        t.body = b
-
-        return t
+        # build tile with header and body
+        return B3dm(b3dm_header, b3dm_body)
 
 
 class B3dmHeader(TileContentHeader):
     BYTE_LENGTH = 28
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
-        self.type = TileContentType.BATCHED_3D_MODEL
         self.magic_value = b"b3dm"
         self.version = 1
 
-    def to_array(self):
+    def to_array(self) -> npt.NDArray[np.uint8]:
         header_arr = np.frombuffer(self.magic_value, np.uint8)
 
-        header_arr2 = np.array([self.version,
-                                self.tile_byte_length,
-                                self.ft_json_byte_length,
-                                self.ft_bin_byte_length,
-                                self.bt_json_byte_length,
-                                self.bt_bin_byte_length], dtype=np.uint32)
+        header_arr2 = np.array(
+            [
+                self.version,
+                self.tile_byte_length,
+                self.ft_json_byte_length,
+                self.ft_bin_byte_length,
+                self.bt_json_byte_length,
+                self.bt_bin_byte_length,
+            ],
+            dtype=np.uint32,
+        )
 
         return np.concatenate((header_arr, header_arr2.view(np.uint8)))
 
-    def sync(self, body):
-        """
-        Allow to synchronize headers with contents.
-        """
-
-        # extract array
-        glTF_arr = body.glTF.to_array()
-
-        # sync the tile header with feature table contents
-        self.tile_byte_length = len(glTF_arr) + B3dmHeader.BYTE_LENGTH
-        self.bt_json_byte_length = 0
-        self.bt_bin_byte_length = 0
-        self.ft_json_byte_length = 0
-        self.ft_bin_byte_length = 0
-
-        if body.batch_table is not None:
-            bth_arr = body.batch_table.to_array()
-
-            self.tile_byte_length += len(bth_arr)
-            self.bt_json_byte_length = len(bth_arr)
-
     @staticmethod
-    def from_array(array):
-        """
-        Parameters
-        ----------
-        array : numpy.array
-
-        Returns
-        -------
-        h : TileContentHeader
-        """
-
+    def from_array(array: npt.NDArray[np.uint8]) -> B3dmHeader:
         h = B3dmHeader()
 
         if len(array) != B3dmHeader.BYTE_LENGTH:
-            raise RuntimeError("Invalid header length")
-
-        h.version = struct.unpack("i", array[4:8])[0]
-        h.tile_byte_length = struct.unpack("i", array[8:12])[0]
-        h.ft_json_byte_length = struct.unpack("i", array[12:16])[0]
-        h.ft_bin_byte_length = struct.unpack("i", array[16:20])[0]
-        h.bt_json_byte_length = struct.unpack("i", array[20:24])[0]
-        h.bt_bin_byte_length = struct.unpack("i", array[24:28])[0]
+            raise InvalidB3dmError(
+                f"Invalid header byte length, the size of array is {len(array)}, "
+                f"the header must have a size of {B3dmHeader.BYTE_LENGTH}"
+            )
+
+        h.version = struct.unpack("i", array[4:8].tobytes())[0]
+        h.tile_byte_length = struct.unpack("i", array[8:12].tobytes())[0]
+        h.ft_json_byte_length = struct.unpack("i", array[12:16].tobytes())[0]
+        h.ft_bin_byte_length = struct.unpack("i", array[16:20].tobytes())[0]
+        h.bt_json_byte_length = struct.unpack("i", array[20:24].tobytes())[0]
+        h.bt_bin_byte_length = struct.unpack("i", array[24:28].tobytes())[0]
 
         return h
 
 
 class B3dmBody(TileContentBody):
-    def __init__(self):
+    def __init__(self) -> None:
         self.batch_table = BatchTable()
-        self.glTF = GlTF()
+        self.gltf = GlTF()
 
-    def to_array(self):
-        # TODO : export feature table
-        array = self.glTF.to_array()
-        if self.batch_table is not None:
-            array = np.concatenate((self.batch_table.to_array(), array))
-        return array
+    def to_array(self) -> npt.NDArray[np.uint8]:
+        # TODO : export feature table, reminder, the glTF part must start on an 8-byte boundary.
+        if self.batch_table:
+            batch_table = self.batch_table.to_array()
+        else:
+            batch_table = np.array([], dtype=np.uint8)
 
-    @staticmethod
-    def from_glTF(glTF):
-        """
-        Parameters
-        ----------
-        th : TileContentHeader
-
-        glTF : GlTF
-
-        Returns
-        -------
-        b : TileContentBody
-        """
+        # The glTF part must start and end on an 8-byte boundary
+        gltf_array = self.gltf.to_array()
+
+        return np.concatenate((batch_table, gltf_array))
 
+    @staticmethod
+    def from_gltf(gltf: GlTF) -> B3dmBody:
         # build tile body
         b = B3dmBody()
-        b.glTF = glTF
+        b.gltf = gltf
 
         return b
 
     @staticmethod
-    def from_array(th, array):
-        """
-        Parameters
-        ----------
-        th : TileContentHeader
-
-        array : numpy.array
-
-        Returns
-        -------
-        b : TileContentBody
-        """
-
+    def from_array(b3dm_header: B3dmHeader, array: npt.NDArray[np.uint8]) -> B3dmBody:
         # build feature table
-        ft_len = th.ft_json_byte_length + th.ft_bin_byte_length
+        ft_len = b3dm_header.ft_json_byte_length + b3dm_header.ft_bin_byte_length
 
         # build batch table
-        bt_len = th.bt_json_byte_length + th.bt_bin_byte_length
+        bt_len = b3dm_header.bt_json_byte_length + b3dm_header.bt_bin_byte_length
 
         # build glTF
-        glTF_len = (th.tile_byte_length - ft_len - bt_len
-                    - B3dmHeader.BYTE_LENGTH)
-        glTF_arr = array[ft_len + bt_len:ft_len + bt_len + glTF_len]
-        glTF = GlTF.from_array(glTF_arr)
+        gltf_len = (
+            b3dm_header.tile_byte_length - ft_len - bt_len - B3dmHeader.BYTE_LENGTH
+        )
+        gltf_arr = array[ft_len + bt_len : ft_len + bt_len + gltf_len]
+        gltf = GlTF.from_array(gltf_arr)
 
         # build tile body with batch table
         b = B3dmBody()
-        b.glTF = glTF
-        if th.bt_json_byte_length > 0:
-            b.batch_table.header = json.loads(array[0:th.bt_json_byte_length].tobytes().decode('utf-8'))
+        b.gltf = gltf
+        if b3dm_header.bt_json_byte_length > 0:
+            b.batch_table = BatchTable.from_array(
+                b3dm_header, array[0 : b3dm_header.bt_json_byte_length]
+            )
 
         return b
```

### Comparing `py3dtiles-5.0.0/py3dtiles/tileset/content/gltf.py` & `py3dtiles-6.0.0/py3dtiles/tileset/content/gltf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,70 @@
+from __future__ import annotations
+
 import json
 import struct
+from typing import Any, Sequence
 
 import numpy as np
+import numpy.typing as npt
 
 
 class GlTF:
     HEADER_LENGTH = 12
     CHUNK_HEADER_LENGTH = 8
 
-    def __init__(self):
+    def __init__(self) -> None:
         self.header = {}
         self.body = None
 
-    def to_array(self):  # glb
-        scene = json.dumps(self.header, separators=(',', ':'))
-
-        # body must be 4-byte aligned
-        scene += ' ' * ((4 - len(scene) % 4) % 4)
+    def to_array(self) -> npt.NDArray[np.uint8]:  # glb
+        scene = json.dumps(self.header, separators=(",", ":"))
 
-        padding = np.array([0 for i in range(0, (4 - len(self.body) % 4) % 4)],
-                           dtype=np.uint8)
+        # body must start with 4-byte boundary
+        scene += " " * ((4 - len(scene) % 4) % 4)
 
         length = GlTF.HEADER_LENGTH + (2 * GlTF.CHUNK_HEADER_LENGTH)
-        length += len(self.body) + len(scene) + len(padding)
-        binary_header = np.array([0x46546C67,  # "glTF" magic
-                                  2,  # version
-                                  length], dtype=np.uint32)
-        json_chunk_header = np.array([len(scene),  # JSON chunck length
-                                      0x4E4F534A], dtype=np.uint32)  # "JSON"
-
-        bin_chunk_header = np.array([len(self.body) + len(padding),
-                                     # BIN chunck length
-                                     0x004E4942], dtype=np.uint32)  # "BIN"
-
-        return np.concatenate((binary_header.view(np.uint8),
-                               json_chunk_header.view(np.uint8),
-                               np.frombuffer(scene.encode('utf-8'), dtype=np.uint8),
-                               bin_chunk_header.view(np.uint8),
-                               self.body,
-                               padding))
-
-    @staticmethod
-    def from_array(array):
-        """
-        Parameters
-        ----------
-        array : numpy.array
+        length += len(self.body) + len(scene)
 
-        Returns
-        -------
-        glTF : GlTf
-        """
+        # gltf must end with an 8-byte boundary
+        # the padding is added inside the gltf body
+        # https://github.com/CesiumGS/3d-tiles/tree/main/specification/TileFormats/Batched3DModel#padding
+        body_padding = np.zeros((8 - length % 8) % 8, dtype=np.uint8)
+        length += len(body_padding)
+
+        binary_header = np.array(
+            [0x46546C67, 2, length], dtype=np.uint32  # "glTF" magic  # version
+        )
+        json_chunk_header = np.array(
+            [len(scene), 0x4E4F534A], dtype=np.uint32  # JSON chunck length
+        )  # "JSON"
+
+        bin_chunk_header = np.array(
+            [
+                len(self.body) + len(body_padding),
+                # BIN chunck length
+                0x004E4942,
+            ],
+            dtype=np.uint32,
+        )  # "BIN"
+
+        return np.concatenate(
+            (
+                binary_header.view(np.uint8),
+                json_chunk_header.view(np.uint8),
+                np.frombuffer(scene.encode("utf-8"), dtype=np.uint8),
+                bin_chunk_header.view(np.uint8),
+                self.body,
+                body_padding,
+            )
+        )
 
-        glTF = GlTF()
+    @staticmethod
+    def from_array(array: npt.NDArray[np.uint8]) -> GlTF:
+        gltf = GlTF()
 
         if struct.unpack("4s", array[0:4])[0] != b"glTF":
             raise RuntimeError("Array does not contain a binary glTF")
 
         version = struct.unpack("i", array[4:8])[0]
         if version != 1 and version != 2:
             raise RuntimeError("Unsupported glTF version")
@@ -64,26 +72,37 @@
         length = struct.unpack("i", array[8:12])[0]
         json_chunk_length = struct.unpack("i", array[12:16])[0]
 
         chunk_type = struct.unpack("i", array[16:20])[0]
         if chunk_type != 0 and chunk_type != 1313821514:  # 1313821514 => 'JSON'
             raise RuntimeError("Unsupported binary glTF content type")
 
-        index = GlTF.HEADER_LENGTH + GlTF.CHUNK_HEADER_LENGTH  # Skip the header and the JSON chunk header
-        header = struct.unpack(str(json_chunk_length) + "s",
-                               array[index:index + json_chunk_length])[0]
-        glTF.header = json.loads(header.decode("ascii"))
-
-        index += json_chunk_length + GlTF.CHUNK_HEADER_LENGTH  # Skip the JSON chunk data and the binary chunk header
-        glTF.body = array[index:length]
+        index = (
+            GlTF.HEADER_LENGTH + GlTF.CHUNK_HEADER_LENGTH
+        )  # Skip the header and the JSON chunk header
+        header = struct.unpack(
+            str(json_chunk_length) + "s", array[index : index + json_chunk_length]
+        )[0]
+        gltf.header = json.loads(header.decode("ascii"))
+
+        index += (
+            json_chunk_length + GlTF.CHUNK_HEADER_LENGTH
+        )  # Skip the JSON chunk data and the binary chunk header
+        gltf.body = array[index:length]
 
-        return glTF
+        return gltf
 
     @staticmethod
-    def from_binary_arrays(arrays, transform, batched=True, uri=None, texture_uri=None):
+    def from_binary_arrays(
+        arrays: list[dict[str, Sequence[Any]]],
+        transform: npt.NDArray[np.float64],
+        batched: bool = True,
+        uri: str | None = None,
+        texture_uri: str | None = None,
+    ) -> GlTF:
         """
         Parameters
         ----------
         arrays : array of dictionaries
             Each dictionary has the data for one geometry
             arrays['position']: binary array of vertex positions
             arrays['normal']: binary array of vertex normals
@@ -92,232 +111,248 @@
             arrays['bbox']: geometry bounding box (numpy.array)
 
         transform : numpy.array
             World coordinates transformation flattend matrix
 
         Returns
         -------
-        glTF : GlTF
+        gltf : GlTF
         """
 
-        glTF = GlTF()
+        gltf = GlTF()
 
-        textured = 'uv' in arrays[0]
+        textured = "uv" in arrays[0]
         bin_vertices = []
         bin_normals = []
         bin_ids = []
         bin_uvs = []
         n_vertices = []
         bb = []
         batch_length = 0
         for i, geometry in enumerate(arrays):
-            bin_vertices.append(geometry['position'])
-            bin_normals.append(geometry['normal'])
-            n = round(len(geometry['position']) / 12)
+            bin_vertices.append(geometry["position"])
+            bin_normals.append(geometry["normal"])
+            n = round(len(geometry["position"]) / 12)
             n_vertices.append(n)
-            bb.append(geometry['bbox'])
+            bb.append(geometry["bbox"])
             if batched:
                 bin_ids.append(np.full(n, i, dtype=np.float32))
             if textured:
-                bin_uvs.append(geometry['uv'])
+                bin_uvs.append(geometry["uv"])
 
         if batched:
-            bin_vertices = [b''.join(bin_vertices)]
-            bin_normals = [b''.join(bin_normals)]
-            bin_uvs = [b''.join(bin_uvs)]
-            bin_ids = [b''.join(bin_ids)]
+            bin_vertices = [b"".join(bin_vertices)]
+            bin_normals = [b"".join(bin_normals)]
+            bin_uvs = [b"".join(bin_uvs)]
+            bin_ids = [b"".join(bin_ids)]
             n_vertices = [sum(n_vertices)]
             batch_length = len(arrays)
             [minx, miny, minz] = bb[0][0]
             [maxx, maxy, maxz] = bb[0][1]
             for box in bb[1:]:
                 minx = min(minx, box[0][0])
                 miny = min(miny, box[0][1])
                 minz = min(minz, box[0][2])
                 maxx = max(maxx, box[1][0])
                 maxy = max(maxy, box[1][1])
                 maxz = max(maxz, box[1][2])
             bb = [[[minx, miny, minz], [maxx, maxy, maxz]]]
 
-        glTF.header = compute_header(bin_vertices, n_vertices, bb, transform,
-                                     textured, batched, batch_length, uri,
-                                     texture_uri)
-        glTF.body = np.frombuffer(compute_binary(bin_vertices, bin_normals,
-                                                 bin_ids, bin_uvs), dtype=np.uint8)
+        gltf.header = compute_header(
+            bin_vertices,
+            n_vertices,
+            bb,
+            transform,
+            textured,
+            batched,
+            batch_length,
+            uri,
+            texture_uri,
+        )
+        gltf.body = np.frombuffer(
+            compute_binary(bin_vertices, bin_normals, bin_ids, bin_uvs), dtype=np.uint8
+        )
 
-        return glTF
+        return gltf
 
 
 def compute_binary(bin_vertices, bin_normals, bin_ids, bin_uvs):
-    bv = b''.join(bin_vertices)
-    bn = b''.join(bin_normals)
-    bid = b''.join(bin_ids)
-    buv = b''.join(bin_uvs)
+    bv = b"".join(bin_vertices)
+    bn = b"".join(bin_normals)
+    bid = b"".join(bin_ids)
+    buv = b"".join(bin_uvs)
     return bv + bn + buv + bid
 
 
-def compute_header(bin_vertices, n_vertices, bb, transform,
-                   textured, batched, batch_length, uri, texture_uri):
+def compute_header(
+    bin_vertices,
+    n_vertices,
+    bb,
+    transform,
+    textured,
+    batched,
+    batch_length,
+    uri,
+    texture_uri,
+):
     # Buffer
     mesh_nb = len(bin_vertices)
     size_vce = []
-    for i in range(0, mesh_nb):
+    for i in range(mesh_nb):
         size_vce.append(len(bin_vertices[i]))
 
     byte_length = 2 * sum(size_vce)
     if textured:
         byte_length += int(round(2 * sum(size_vce) / 3))
     if batched:
         byte_length += int(round(sum(size_vce) / 3))
-    buffers = [{
-        'byteLength': byte_length
-    }]
+    buffers = [{"byteLength": byte_length}]
     if uri is not None:
         buffers.append({"binary_glTF": {"uri": uri}})
 
     # Buffer view
-    buffer_views = [{
-        'buffer': 0,
-        'byteLength': sum(size_vce),
-        'byteOffset': 0,
-        'target': 34962
-    }, {
-        'buffer': 0,
-        'byteLength': sum(size_vce),
-        'byteOffset': sum(size_vce),
-        'target': 34962
-    }]
+    buffer_views = [
+        {"buffer": 0, "byteLength": sum(size_vce), "byteOffset": 0, "target": 34962},
+        {
+            "buffer": 0,
+            "byteLength": sum(size_vce),
+            "byteOffset": sum(size_vce),
+            "target": 34962,
+        },
+    ]
     # vertices
     if textured:
-        buffer_views.append({
-            'buffer': 0,
-            'byteLength': int(round(2 * sum(size_vce) / 3)),
-            'byteOffset': 2 * sum(size_vce),
-            'target': 34962
-        })
+        buffer_views.append(
+            {
+                "buffer": 0,
+                "byteLength": int(round(2 * sum(size_vce) / 3)),
+                "byteOffset": 2 * sum(size_vce),
+                "target": 34962,
+            }
+        )
     if batched:
-        buffer_views.append({
-            'buffer': 0,
-            'byteLength': int(round(sum(size_vce) / 3)),
-            'byteOffset': int(round(8 / 3 * sum(size_vce))) if textured
-            else 2 * sum(size_vce),
-            'target': 34962
-        })
+        buffer_views.append(
+            {
+                "buffer": 0,
+                "byteLength": int(round(sum(size_vce) / 3)),
+                "byteOffset": int(round(8 / 3 * sum(size_vce)))
+                if textured
+                else 2 * sum(size_vce),
+                "target": 34962,
+            }
+        )
 
     # Accessor
     accessors = []
-    for i in range(0, mesh_nb):
+    for i in range(mesh_nb):
         # vertices
-        accessors.append({
-            'bufferView': 0,
-            'byteOffset': sum(size_vce[0:i]),
-            'componentType': 5126,
-            'count': n_vertices[i],
-            'min': [bb[i][0][0], bb[i][0][1], bb[i][0][2]],
-            'max': [bb[i][1][0], bb[i][1][1], bb[i][1][2]],
-            'type': "VEC3"
-        })
+        accessors.append(
+            {
+                "bufferView": 0,
+                "byteOffset": sum(size_vce[0:i]),
+                "componentType": 5126,
+                "count": n_vertices[i],
+                "min": [bb[i][0][0], bb[i][0][1], bb[i][0][2]],
+                "max": [bb[i][1][0], bb[i][1][1], bb[i][1][2]],
+                "type": "VEC3",
+            }
+        )
         # normals
-        accessors.append({
-            'bufferView': 1,
-            'byteOffset': sum(size_vce[0:i]),
-            'componentType': 5126,
-            'count': n_vertices[i],
-            'max': [1, 1, 1],
-            'min': [-1, -1, -1],
-            'type': "VEC3"
-        })
+        accessors.append(
+            {
+                "bufferView": 1,
+                "byteOffset": sum(size_vce[0:i]),
+                "componentType": 5126,
+                "count": n_vertices[i],
+                "max": [1, 1, 1],
+                "min": [-1, -1, -1],
+                "type": "VEC3",
+            }
+        )
         if textured:
-            accessors.append({
-                'bufferView': 2,
-                'byteOffset': int(round(2 / 3 * sum(size_vce[0:i]))),
-                'componentType': 5126,
-                'count': sum(n_vertices),
-                'max': [1, 1],
-                'min': [0, 0],
-                'type': "VEC2"
-            })
+            accessors.append(
+                {
+                    "bufferView": 2,
+                    "byteOffset": int(round(2 / 3 * sum(size_vce[0:i]))),
+                    "componentType": 5126,
+                    "count": sum(n_vertices),
+                    "max": [1, 1],
+                    "min": [0, 0],
+                    "type": "VEC2",
+                }
+            )
     if batched:
-        accessors.append({
-            'bufferView': 3 if textured else 2,
-            'byteOffset': 0,
-            'componentType': 5126,
-            'count': n_vertices[0],
-            'max': [batch_length],
-            'min': [0],
-            'type': "SCALAR"
-        })
+        accessors.append(
+            {
+                "bufferView": 3 if textured else 2,
+                "byteOffset": 0,
+                "componentType": 5126,
+                "count": n_vertices[0],
+                "max": [batch_length],
+                "min": [0],
+                "type": "SCALAR",
+            }
+        )
 
     # Meshes
     meshes = []
     n_attributes = 3 if textured else 2
-    for i in range(0, mesh_nb):
-        meshes.append({
-            'primitives': [{
-                'attributes': {
-                    "POSITION": n_attributes * i,
-                    "NORMAL": n_attributes * i + 1
-                },
-                "material": 0,
-                "mode": 4
-            }]
-        })
+    for i in range(mesh_nb):
+        meshes.append(
+            {
+                "primitives": [
+                    {
+                        "attributes": {
+                            "POSITION": n_attributes * i,
+                            "NORMAL": n_attributes * i + 1,
+                        },
+                        "material": 0,
+                        "mode": 4,
+                    }
+                ]
+            }
+        )
         if textured:
-            meshes[i]['primitives'][0]['attributes']['TEXCOORD_0'] = (
-                n_attributes * i + 2)
+            meshes[i]["primitives"][0]["attributes"]["TEXCOORD_0"] = (
+                n_attributes * i + 2
+            )
     if batched:
-        meshes[0]['primitives'][0]['attributes']['_BATCHID'] = n_attributes
+        meshes[0]["primitives"][0]["attributes"]["_BATCHID"] = n_attributes
 
     # Nodes
     nodes = []
-    for i in range(0, mesh_nb):
-        nodes.append({
-            'matrix': [float(e) for e in transform],
-            'mesh': i
-        })
+    for i in range(mesh_nb):
+        nodes.append({"matrix": [float(e) for e in transform], "mesh": i})
 
     # Materials
-    materials = [{
-        'pbrMetallicRoughness': {
-            'metallicFactor': 0
-        },
-        'name': 'Material',
-    }]
+    materials = [
+        {
+            "pbrMetallicRoughness": {"metallicFactor": 0},
+            "name": "Material",
+        }
+    ]
 
     # Final glTF
     header = {
-        'asset': {
-            "generator": "py3dtiles",
-            "version": "2.0"
-        },
-        'scene': 0,
-        'scenes': [{
-            'nodes': [i for i in range(0, len(nodes))]
-        }],
-        'nodes': nodes,
-        'meshes': meshes,
-        'materials': materials,
-        'accessors': accessors,
-        'bufferViews': buffer_views,
-        'buffers': buffers
+        "asset": {"generator": "py3dtiles", "version": "2.0"},
+        "scene": 0,
+        "scenes": [{"nodes": list(range(len(nodes)))}],
+        "nodes": nodes,
+        "meshes": meshes,
+        "materials": materials,
+        "accessors": accessors,
+        "bufferViews": buffer_views,
+        "buffers": buffers,
     }
 
     # Texture data
     if textured:
-        header['textures'] = [{
-            'sampler': 0,
-            'source': 0
-        }]
-        header['images'] = [{
-            'uri': texture_uri
-        }]
-        header['samplers'] = [{
-            "magFilter": 9729,
-            "minFilter": 9987,
-            "wrapS": 10497,
-            "wrapT": 10497
-        }]
-        header['materials'][0]['pbrMetallicRoughness']['baseColorTexture'] = {
-            'index': 0
+        header["textures"] = [{"sampler": 0, "source": 0}]
+        header["images"] = [{"uri": texture_uri}]
+        header["samplers"] = [
+            {"magFilter": 9729, "minFilter": 9987, "wrapS": 10497, "wrapT": 10497}
+        ]
+        header["materials"][0]["pbrMetallicRoughness"]["baseColorTexture"] = {
+            "index": 0
         }
 
     return header
```

### Comparing `py3dtiles-5.0.0/py3dtiles/tileset/tile_content.py` & `py3dtiles-6.0.0/py3dtiles/tileset/content/tile_content.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,77 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from enum import Enum
 from pathlib import Path
+from typing import Literal
 
 import numpy as np
 import numpy.typing as npt
 
+from .batch_table import BatchTable
+from .feature_table import FeatureTable
 
-class TileContent:
-    def __init__(self):
-        self.header = None
-        self.body = None
+
+class TileContent(ABC):
+    header: TileContentHeader
+    body: TileContentBody
 
     def to_array(self) -> npt.NDArray[np.uint8]:
         self.sync()
         header_arr = self.header.to_array()
         body_arr = self.body.to_array()
         return np.concatenate((header_arr, body_arr))
 
-    def to_hex_str(self):
+    def to_hex_str(self) -> str:
         arr = self.to_array()
         return " ".join(f"{x:02X}" for x in arr)
 
-    def save_as(self, path: Path):
+    def save_as(self, path: Path) -> None:
         tile_arr = self.to_array()
-        with path.open('bw') as f:
+        with path.open("bw") as f:
             f.write(bytes(tile_arr))
 
-    def sync(self):
+    @abstractmethod
+    def print_info(self) -> None:
+        ...
+
+    @abstractmethod
+    def sync(self) -> None:
         """
         Allow to synchronize headers with contents.
         """
-        self.header.sync(self.body)
 
-
-class TileContentType(Enum):
-    UNKNOWN = 0
-    POINT_CLOUD = 1
-    BATCHED_3D_MODEL = 2
+    @staticmethod
+    @abstractmethod
+    def from_array(array: npt.NDArray[np.uint8]) -> TileContent:
+        ...
 
 
 class TileContentHeader(ABC):
-    def __init__(self):
+    magic_value: Literal[b"b3dm", b"pnts"]
+    version: int
+
+    def __init__(self) -> None:
         self.tile_byte_length = 0
         self.ft_json_byte_length = 0
         self.ft_bin_byte_length = 0
         self.bt_json_byte_length = 0
         self.bt_bin_byte_length = 0
         self.bt_length = 0  # number of models in the batch
 
     @staticmethod
     @abstractmethod
-    def from_array(array: npt.NDArray) -> TileContentHeader: ...
-
-    @abstractmethod
-    def to_array(self) -> npt.NDArray: ...
+    def from_array(array: npt.NDArray[np.uint8]) -> TileContentHeader:
+        ...
 
     @abstractmethod
-    def sync(self, body) -> None: ...
+    def to_array(self) -> npt.NDArray[np.uint8]:
+        ...
 
 
 class TileContentBody(ABC):
+    batch_table: BatchTable
+    feature_table: FeatureTable
+
     @abstractmethod
-    def to_array(self) -> npt.NDArray: ...
+    def to_array(self) -> npt.NDArray[np.uint8]:
+        ...
```

### Comparing `py3dtiles-5.0.0/py3dtiles/tileset/utils.py` & `py3dtiles-6.0.0/py3dtiles/tileset/content/tile_content_reader.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 from __future__ import annotations
 
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 import numpy as np
+import numpy.typing as npt
 
-from py3dtiles.tileset.content import B3dm, Pnts
+from py3dtiles.exceptions import Invalid3dtilesError
+from .b3dm import B3dm
+from .pnts import Pnts
 
 if TYPE_CHECKING:
-    from .tile_content import TileContent
+    from py3dtiles.tileset.content import TileContent
 
+__all__ = ["read_binary_tile_content"]
 
-class TileContentReader:
 
-    @staticmethod
-    def read_file(tile_path: Path) -> TileContent:
-        with tile_path.open('rb') as f:
-            data = f.read()
-            arr = np.frombuffer(data, dtype=np.uint8)
-
-            tile_content = TileContentReader.read_array(arr)
-            if tile_content is None or tile_content.header is None:
-                raise ValueError(f"The file {tile_path} doesn't contain a valid TileContent data.")
-
-            return tile_content
-
-    @staticmethod
-    def read_array(array: np.ndarray) -> TileContent | None:
-        magic = ''.join([c.decode('UTF-8') for c in array[0:4].view('c')])
-        if magic == 'pnts':
-            return Pnts.from_array(array)
-        if magic == 'b3dm':
-            return B3dm.from_array(array)
-        return None
+def read_binary_tile_content(tile_path: Path) -> TileContent:
+    with tile_path.open("rb") as f:
+        data = f.read()
+        arr = np.frombuffer(data, dtype=np.uint8)
+
+        tile_content = read_array(arr)
+        if tile_content is None or tile_content.header is None:
+            raise Invalid3dtilesError(
+                f"The file {tile_path} doesn't contain a valid TileContent data."
+            )
+
+        return tile_content
+
+
+def read_array(array: npt.NDArray[np.uint8]) -> TileContent | None:
+    magic = "".join([c.decode("UTF-8") for c in array[0:4].view("c")])
+    if magic == "pnts":
+        return Pnts.from_array(array)
+    if magic == "b3dm":
+        return B3dm.from_array(array)
+    return None
```

### Comparing `py3dtiles-5.0.0/py3dtiles/utils.py` & `py3dtiles-6.0.0/py3dtiles/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,103 +1,133 @@
 from __future__ import annotations
 
 from enum import Enum
 from io import StringIO
 from pathlib import Path, PurePath
-from typing import Callable
+from typing import Callable, NamedTuple, TYPE_CHECKING, TypeVar
 
 import numpy as np
+import numpy.typing as npt
 from pyproj import CRS
 
+if TYPE_CHECKING:
+    from py3dtiles.tilers.node import Node
+    from typing_extensions import ParamSpec
+
+_T = TypeVar("_T", bound=npt.NBitBase)
+
+MIN_AABB_SIZE = 0.00001
+
 
 def str_to_CRS(srs: str | CRS | None) -> CRS | None:
     """
     Convert a string in a pyproj CRS object. The string could be an epsg code or a Proj4 string. If srs is already
     a CRS object, the function returns the same CRS definition.
     """
     if srs is None:
         return None
 
     try:
-        return CRS.from_epsg(int(srs)) # type: ignore
+        return CRS.from_epsg(int(srs))  # type: ignore [arg-type]
     except ValueError:
         return CRS(srs)
 
 
 class CommandType(Enum):
-    READ_FILE = b'read_file'
-    WRITE_PNTS = b'write_pnts'
-    PROCESS_JOBS = b'process_jobs'
-    SHUTDOWN = b'shutdown'
+    READ_FILE = b"read_file"
+    WRITE_PNTS = b"write_pnts"
+    PROCESS_JOBS = b"process_jobs"
+    SHUTDOWN = b"shutdown"
 
 
 class ResponseType(Enum):
-    IDLE = b'idle'
-    HALTED = b'halted'
-    READ = b'read'
-    PROCESSED = b'processed'
-    PNTS_WRITTEN = b'pnts_written'
-    NEW_TASK = b'new_task'
-    ERROR = b'error'
+    IDLE = b"idle"
+    HALTED = b"halted"
+    READ = b"read"
+    PROCESSED = b"processed"
+    PNTS_WRITTEN = b"pnts_written"
+    NEW_TASK = b"new_task"
+    ERROR = b"error"
+
+
+class OctreeMetadata(NamedTuple):
+    aabb: npt.NDArray[np.float64]
+    spacing: float
+    scale: float
+
+
+if TYPE_CHECKING:
+    Param = ParamSpec("Param")
+    RetType = TypeVar("RetType")
 
 
-def profile(func: Callable) -> Callable:
+def profile(func: Callable[Param, RetType]) -> Callable[Param, RetType]:
     from line_profiler import LineProfiler
 
-    def wrapper(*args, **kwargs):
+    def wrapper(*args, **kwargs):  # type: ignore [no-untyped-def]
         lp = LineProfiler()
         deco = lp(func)
         res = deco(*args, **kwargs)
         s = StringIO()
         lp.print_stats(stream=s)
         print(s.getvalue())
         return res
+
     return wrapper
 
 
 class SubdivisionType(Enum):
     OCTREE = 1
     QUADTREE = 2
 
-def node_name_to_path(working_dir: Path, name: bytes, suffix: str = '', split_len: int = 8) -> Path:
+
+def node_name_to_path(
+    working_dir: Path, name: bytes, suffix: str = "", split_len: int = 8
+) -> Path:
     """
     Get the path of a tile from its name and the working directory.
     If the name is '222262175' with the suffix '.pnts', the result is 'working_dir/22226217/r5.pnts'
     """
-    str_name = name.decode('ascii')
+    str_name = name.decode("ascii")
     if len(str_name) <= split_len:
         filename = PurePath("r" + str_name + suffix)
     else:
         # the name is split on every 'split_len' char to avoid to have too many tiles on the same folder.
-        sub_folders = [str_name[i:i + split_len] for i in range(0, len(str_name), split_len)]
+        sub_folders = [
+            str_name[i : i + split_len] for i in range(0, len(str_name), split_len)
+        ]
         working_dir = working_dir.joinpath(*sub_folders[:-1])
         filename = PurePath("r" + sub_folders[-1] + suffix)
 
     full_path = working_dir / filename
     working_dir.mkdir(parents=True, exist_ok=True)
 
     return full_path
 
 
-def compute_spacing(aabb: np.ndarray) -> float:
+def compute_spacing(aabb: npt.NDArray[np.floating[_T]]) -> float:
     return float(np.linalg.norm(aabb[1] - aabb[0]) / 125)
 
 
-def aabb_size_to_subdivision_type(size: np.ndarray) -> SubdivisionType:
+def aabb_size_to_subdivision_type(
+    size: npt.NDArray[np.floating[_T]],
+) -> SubdivisionType:
     if size[2] / min(size[0], size[1]) < 0.5:
         return SubdivisionType.QUADTREE
     else:
         return SubdivisionType.OCTREE
 
 
-def split_aabb(aabb: np.ndarray, index: int, force_quadtree: bool = False) -> np.ndarray:
+def split_aabb(
+    aabb: npt.NDArray[np.floating[_T]], index: int, force_quadtree: bool = False
+) -> npt.NDArray[np.floating[_T]]:
     half = (aabb[1] - aabb[0]) * 0.5
     t = aabb_size_to_subdivision_type(half)
 
-    new_aabb = np.array([np.copy(aabb[0]), aabb[0] + half])
+    new_aabb = np.array([aabb[0], aabb[0] + half])
     if index & 4:
         new_aabb[0][0] += half[0]
         new_aabb[1][0] += half[0]
     if index & 2:
         new_aabb[0][1] += half[1]
         new_aabb[1][1] += half[1]
 
@@ -106,21 +136,35 @@
     elif index & 1:
         new_aabb[0][2] += half[2]
         new_aabb[1][2] += half[2]
 
     return new_aabb
 
 
-def make_aabb_cubic(aabb):
+def make_aabb_cubic(aabb: npt.NDArray[np.floating[_T]]) -> npt.NDArray[np.floating[_T]]:
     s = max(aabb[1] - aabb[0])
     aabb[1][0] = aabb[0][0] + s
     aabb[1][1] = aabb[0][1] + s
     aabb[1][2] = aabb[0][2] + s
     return aabb
 
 
-def node_from_name(name, parent_aabb, parent_spacing):
+def make_aabb_valid(aabb: list[list[float]]) -> None:
+    """
+    Modify inplace the aabb so that no dimension is 0-sized
+    """
+    for i in range(3):
+        if aabb[0][i] == aabb[1][i]:
+            aabb[1][i] = aabb[1][i] + MIN_AABB_SIZE
+
+
+def node_from_name(
+    name: bytes,
+    parent_aabb: npt.NDArray[np.floating[_T]],
+    parent_spacing: float,
+) -> Node:
     from py3dtiles.tilers.node import Node
+
     spacing = parent_spacing * 0.5
     aabb = split_aabb(parent_aabb, int(name[-1])) if len(name) > 0 else parent_aabb
-    #  let's build a new Node
-    return Node(name, aabb, spacing)
+    # let's build a new Node
+    return Node(name, aabb.astype(np.float64), spacing)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `py3dtiles-5.0.0/py3dtiles.egg-info/SOURCES.txt` & `py3dtiles-6.0.0/py3dtiles.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -34,35 +34,41 @@
 py3dtiles/tilers/node/node_process.py
 py3dtiles/tilers/node/points_grid.py
 py3dtiles/tilers/node/shared_node_store.py
 py3dtiles/tilers/pnts/__init__.py
 py3dtiles/tilers/pnts/constants.py
 py3dtiles/tilers/pnts/pnts_writer.py
 py3dtiles/tileset/__init__.py
-py3dtiles/tileset/batch_table.py
 py3dtiles/tileset/bounding_volume.py
 py3dtiles/tileset/bounding_volume_box.py
-py3dtiles/tileset/extendable.py
-py3dtiles/tileset/feature_table.py
+py3dtiles/tileset/root_property.py
 py3dtiles/tileset/tile.py
-py3dtiles/tileset/tile_content.py
 py3dtiles/tileset/tileset.py
 py3dtiles/tileset/utils.py
 py3dtiles/tileset/content/__init__.py
 py3dtiles/tileset/content/b3dm.py
+py3dtiles/tileset/content/batch_table.py
+py3dtiles/tileset/content/feature_table.py
 py3dtiles/tileset/content/gltf.py
 py3dtiles/tileset/content/pnts.py
+py3dtiles/tileset/content/tile_content.py
+py3dtiles/tileset/content/tile_content_reader.py
 py3dtiles/tileset/extension/__init__.py
 py3dtiles/tileset/extension/base_extension.py
+py3dtiles/tileset/extension/batch_table_hierarchy_extension.py
 tests/__init__.py
 tests/test_b3dm.py
 tests/test_batch_table.py
+tests/test_batch_table_hierachy_extension.py
 tests/test_bounding_volume_box.py
+tests/test_code_examples.py
 tests/test_convert.py
 tests/test_extension.py
-tests/test_pc.py
+tests/test_merger.py
+tests/test_pnts.py
 tests/test_points.py
 tests/test_reader.py
 tests/test_shared_node_store.py
 tests/test_tile.py
 tests/test_tileset.py
+tests/test_utils.py
 tests/test_wkb_utils.py
```

### Comparing `py3dtiles-5.0.0/setup.py` & `py3dtiles-6.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,54 +2,52 @@
 import re
 
 from setuptools import find_packages, setup
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 requirements = (
-    'cython',
-    'earcut==1.1.5',
-    'laspy>=2.0,<3.0',
-    'lz4',
-    'numba',
-    'numpy>=1.20.0,<1.23',
-    'plyfile',
-    'psutil',
-    'psycopg2-binary',
-    'pyproj',
-    'pyzmq',
+    "cython",
+    "earcut==1.1.5",
+    "laspy>=2.0,<3.0",
+    "lz4",
+    "numba",
+    "numpy>=1.20.0,<1.23",
+    "plyfile",
+    "psutil",
+    "psycopg2-binary",
+    "pyproj",
+    "pyzmq",
 )
 
 dev_requirements = (
-    'commitizen',
-    'line_profiler',
-    'pre-commit',
-    'pytest',
-    'pytest-benchmark',
-    'pytest-cov',
-    'mypy',
-    'typing_extensions',
+    "commitizen",
+    "line_profiler",
+    "pre-commit",
+    "pytest",
+    "pytest-benchmark",
+    "pytest-cov",
+    "mypy",
+    "typing_extensions",
+    "types_psutil",
+    "types_psycopg2",
 )
 
 doc_requirements = (
-    'sphinx',
-    'sphinx-multiversion',
-    'sphinx_rtd_theme',
+    "sphinx",
+    "sphinx-multiversion",
+    "sphinx_rtd_theme",
 )
 
 packaging_requirements = sum(
     (
         dev_requirements,
-        (
-            'build',
-            'twine',
-            'wheel'
-        ),
+        ("build", "twine", "wheel"),
     ),
-    ()
+    (),
 )
 
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
@@ -59,44 +57,46 @@
     """
 
     with open(os.path.join(here, *file_paths)) as f:
         version_file = f.read()
 
     # The version line must have the form
     # __version__ = 'ver'
-    version_match = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]",
-                              version_file, re.M)
+    version_match = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]", version_file, re.M)
     if version_match:
         return version_match.group(1)
-    raise RuntimeError("Unable to find version string. "
-                       "Should be at the first line of __init__.py.")
+    raise RuntimeError(
+        "Unable to find version string. " "Should be at the first line of __init__.py."
+    )
 
 
 setup(
-    name='py3dtiles',
-    version=find_version('py3dtiles', '__init__.py'),
+    name="py3dtiles",
+    version=find_version("py3dtiles", "__init__.py"),
     description="Python module for 3D tiles format",
-    long_description=read('README.rst'),
-    long_description_content_type='text/x-rst',
-    url='https://gitlab.com/Oslandia/py3dtiles',
-    author='Oslandia',
-    author_email='contact@oslandia.com',
-    license='Apache License Version 2.0',
-    python_requires='>=3.8',
+    long_description=read("README.rst"),
+    long_description_content_type="text/x-rst",
+    url="https://gitlab.com/Oslandia/py3dtiles",
+    author="Oslandia",
+    author_email="contact@oslandia.com",
+    license="Apache License Version 2.0",
+    python_requires=">=3.8,<3.11",
     classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'Programming Language :: Python :: 3.8',
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ],
     packages=find_packages(),
     install_requires=requirements,
     test_suite="tests",
     extras_require={
-        'dev': dev_requirements,
-        'doc': doc_requirements,
-        'pack': packaging_requirements,
+        "dev": dev_requirements,
+        "doc": doc_requirements,
+        "pack": packaging_requirements,
     },
     entry_points={
-        'console_scripts': ['py3dtiles=py3dtiles.command_line:main'],
+        "console_scripts": ["py3dtiles=py3dtiles.command_line:main"],
     },
-    zip_safe=False  # zip packaging conflicts with Numba cache (#25)
+    zip_safe=False,  # zip packaging conflicts with Numba cache (#25)
 )
```

### Comparing `py3dtiles-5.0.0/tests/test_bounding_volume_box.py` & `py3dtiles-6.0.0/tests/test_bounding_volume_box.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,207 +1,172 @@
+from typing import List
 import unittest
 
 import numpy as np
 from numpy.testing import assert_array_equal
 
-from py3dtiles.tileset.bounding_volume_box import BoundingVolumeBox
+from py3dtiles.tileset import BoundingVolumeBox
 
 
-class TestBoundingVolumeBox(unittest.TestCase):
+# fmt: off
+DUMMY_MATRIX = [
+    1, 2, 3, 4,
+    5, 6, 7, 8,
+    9, 10, 11, 12,
+]
+# fmt: on
+
 
+class TestBoundingVolumeBox(unittest.TestCase):
     @classmethod
-    def build_box_sample(cls):
+    def build_box_sample(cls) -> BoundingVolumeBox:
         bounding_volume_box = BoundingVolumeBox()
-        bounding_volume_box.set_from_list([
-            1, 2, 3, 4,
-            5, 6, 7, 8,
-            9, 10, 11, 12
-        ])
+        bounding_volume_box.set_from_list(DUMMY_MATRIX)
         return bounding_volume_box
 
-    def test_constructor(self):
+    def test_constructor(self) -> None:
         bounding_volume_box = BoundingVolumeBox()
         self.assertIs(bounding_volume_box._box, None)
 
-    def test_set_from_list(self):
+    def test_set_from_list(self) -> None:
         bounding_volume_box = BoundingVolumeBox()
-        bounding_volume_list = [
-            1, 2, 3, 4,
-            5, 6, 7, 8,
-            9, 10, 11, 12
-        ]
-        bounding_volume_box.set_from_list(bounding_volume_list)
-        assert_array_equal(bounding_volume_box._box, np.array(bounding_volume_list))
+        bounding_volume_box.set_from_list(DUMMY_MATRIX)
+        box = bounding_volume_box._box
+        assert_array_equal(box, np.array(DUMMY_MATRIX))  # type: ignore [arg-type]
 
-    def test_set_from_invalid_list(self):
+    def test_set_from_invalid_list(self) -> None:
         bounding_volume_box = BoundingVolumeBox()
 
         # Empty list
-        bounding_volume_list = []
+        bounding_volume_list: List[float] = []
         with self.assertRaises(ValueError):
             bounding_volume_box.set_from_list(bounding_volume_list)
         self.assertIs(bounding_volume_box._box, None)
 
         # Too small list
-        bounding_volume_list = [
-            1, 2, 3, 4,
-            5, 6, 7, 8,
-            9, 10, 11
-        ]
         with self.assertRaises(ValueError):
-            bounding_volume_box.set_from_list(bounding_volume_list)
+            bounding_volume_box.set_from_list(DUMMY_MATRIX[:-1])
         self.assertIs(bounding_volume_box._box, None)
 
         # Too long list
-        bounding_volume_list = [
-            1, 2, 3, 4,
-            5, 6, 7, 8,
-            9, 10, 11, 12, 13
-        ]
         with self.assertRaises(ValueError):
-            bounding_volume_box.set_from_list(bounding_volume_list)
+            bounding_volume_box.set_from_list(DUMMY_MATRIX + [13])
         self.assertIs(bounding_volume_box._box, None)
 
         # Not only number
-        bounding_volume_list = [
-            1, 2, 3, 4,
-            5, 6, 7, 8,
-            9, 10, 11, 'a'
-        ]
         with self.assertRaises(ValueError):
-            bounding_volume_box.set_from_list(bounding_volume_list)
+            bounding_volume_box.set_from_list(DUMMY_MATRIX[:-1] + ["a"])
         self.assertIs(bounding_volume_box._box, None)
 
-        bounding_volume_list = [
-            1, 2, 3, 4,
-            5, 6, 7, 8,
-            9, 10, 11, [1]
-        ]
         with self.assertRaises(ValueError):
-            bounding_volume_box.set_from_list(bounding_volume_list)
+            bounding_volume_box.set_from_list(DUMMY_MATRIX[:-1] + [[1]])
         self.assertIs(bounding_volume_box._box, None)
 
-    def test_set_from_points(self):
+    def test_set_from_points(self) -> None:
         pass
 
-    def test_set_from_invalid_points(self):
+    def test_set_from_invalid_points(self) -> None:
         # what if I give only one point ?
         pass
 
-    def test_is_only_box(self):
+    def test_is_only_box(self) -> None:
         bounding_volume_box = BoundingVolumeBox()
         self.assertTrue(bounding_volume_box.is_box())
         self.assertFalse(bounding_volume_box.is_region())
         self.assertFalse(bounding_volume_box.is_sphere())
 
-    def test_get_center(self):
+    def test_get_center(self) -> None:
         bounding_volume_box = BoundingVolumeBox()
         with self.assertRaises(AttributeError):
             bounding_volume_box.get_center()
 
         bounding_volume_box = TestBoundingVolumeBox.build_box_sample()
         assert_array_equal(bounding_volume_box.get_center(), [1, 2, 3])
 
-    def test_translate(self):
+    def test_translate(self) -> None:
         bounding_volume_box = BoundingVolumeBox()
         with self.assertRaises(AttributeError):
             bounding_volume_box.translate(np.array([-1, -2, -3]))
 
         bounding_volume_box = TestBoundingVolumeBox.build_box_sample()
         assert_array_equal(bounding_volume_box.get_center(), [1, 2, 3])
 
         bounding_volume_box.translate(np.array([-1, -2, -3]))
         # Should move only the center
-        assert_array_equal(
-            bounding_volume_box._box,
-            [
-                0, 0, 0, 4,
-                5, 6, 7, 8,
-                9, 10, 11, 12
-            ]
-        )
+        # fmt: off
+        expected_result = [
+            0, 0, 0, 4,
+            5, 6, 7, 8,
+            9, 10, 11, 12,
+        ]
+        # fmt: on
+        box = bounding_volume_box._box
+        assert_array_equal(box, expected_result)  # type: ignore [arg-type]
 
-    def test_transform(self):
+    def test_transform(self) -> None:
         bounding_volume_box = TestBoundingVolumeBox.build_box_sample()
 
         # Assert box hasn't change after transformation with identity matrix
-        bounding_volume_box.transform(np.array([1, 0, 0, 0,
-                                       0, 1, 0, 0,
-                                       0, 0, 1, 0,
-                                       0, 0, 0, 1]))
-        assert_array_equal(
-            bounding_volume_box._box,
-            [
-                1, 2, 3,
-                4, 5, 6,
-                7, 8, 9,
-                10, 11, 12
-            ]
-        )
+        transformer = np.identity(4).reshape(-1)
+        bounding_volume_box.transform(transformer)
+        assert_array_equal(bounding_volume_box._box, DUMMY_MATRIX)  # type: ignore [arg-type]
 
         # Assert box is translated by [10, 10, 10] on X,Y, Z axis
-        bounding_volume_box.transform(np.array([1, 0, 0, 0,
-                                       0, 1, 0, 0,
-                                       0, 0, 1, 0,
-                                       10, 10, 10, 1]))
-        assert_array_equal(
-            bounding_volume_box._box,
-            [
-                11, 12, 13,
-                4, 5, 6,
-                7, 8, 9,
-                10, 11, 12
-            ]
-        )
+        transformer[12:15] = 10
+        bounding_volume_box.transform(transformer)
+        # fmt: off
+        expected_result = [
+            11, 12, 13, 4,
+            5, 6, 7, 8,
+            9, 10, 11, 12,
+        ]
+        # fmt: on
+        assert_array_equal(bounding_volume_box._box, expected_result)  # type: ignore [arg-type]
 
         # Assert box is reversed
-        bounding_volume_box.transform(np.array([-1, 0, 0, 0,
-                                       0, -1, 0, 0,
-                                       0, 0, -1, 0,
-                                       0, 0, 0, -1]))
-        assert_array_equal(
-            bounding_volume_box._box,
-            [
-                -11, -12, -13,
-                -4, -5, -6,
-                -7, -8, -9,
-                -10, -11, -12
-            ]
-        )
+        transformer = -np.identity(4).reshape(-1)
+        bounding_volume_box.transform(transformer)
+        # fmt: off
+        expected_result = [
+            -11, -12, -13, -4,
+            -5, -6, -7, -8,
+            -9, -10, -11, -12,
+        ]
+        # fmt: on
+        assert_array_equal(bounding_volume_box._box, expected_result)  # type: ignore [arg-type]
 
-    def test_get_corners(self):
+    def test_get_corners(self) -> None:
         bounding_volume_box = BoundingVolumeBox()
         with self.assertRaises(AttributeError):
             bounding_volume_box.get_corners()
 
         bounding_volume_box = TestBoundingVolumeBox.build_box_sample()
-        assert_array_equal(bounding_volume_box.get_corners(), [  # almost a kindness test
-            [-20, -22, -24],
-            [-12, -12, -12],
-            [-6, -6, -6],
-            [2, 4, 6],
-            [0, 0, 0],
-            [8, 10, 12],
-            [14, 16, 18],
-            [22, 26, 30]])
+        assert_array_equal(
+            bounding_volume_box.get_corners(),
+            [  # almost a kindness test
+                [-20, -22, -24],
+                [-12, -12, -12],
+                [-6, -6, -6],
+                [2, 4, 6],
+                [0, 0, 0],
+                [8, 10, 12],
+                [14, 16, 18],
+                [22, 26, 30],
+            ],
+        )
 
-    def test_get_canonical_as_array(self):
+    def test_get_canonical_as_array(self) -> None:
         pass
 
-    def test_to_dict(self):
+    def test_to_dict(self) -> None:
         bounding_volume_box = BoundingVolumeBox()
         with self.assertRaises(AttributeError):
             bounding_volume_box.to_dict()
 
         self.assertDictEqual(
             TestBoundingVolumeBox.build_box_sample().to_dict(),
-            {'box': [
-                1, 2, 3, 4,
-                5, 6, 7, 8,
-                9, 10, 11, 12
-            ]
-            }
+            {"box": DUMMY_MATRIX},
         )
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `py3dtiles-5.0.0/tests/test_pc.py` & `py3dtiles-6.0.0/tests/test_pnts.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,112 +1,139 @@
 from pathlib import Path
 import unittest
 
 import numpy as np
+from numpy.testing import assert_array_equal
 
-from py3dtiles.tileset.content import Pnts
-from py3dtiles.tileset.feature_table import Feature
-from py3dtiles.tileset.utils import TileContentReader
+from py3dtiles.tileset.content import Pnts, PntsHeader, read_binary_tile_content
+from py3dtiles.tileset.content.feature_table import FeatureTableHeader, SemanticPoint
 
 
 class TestTileContentReader(unittest.TestCase):
-
-    def test_read(self):
-        tile = TileContentReader().read_file(Path('tests/fixtures/pointCloudRGB.pnts'))
+    def test_read(self) -> None:
+        tile = read_binary_tile_content(Path("tests/fixtures/pointCloudRGB.pnts"))
 
         self.assertEqual(tile.header.version, 1.0)
         self.assertEqual(tile.header.tile_byte_length, 15176)
         self.assertEqual(tile.header.ft_json_byte_length, 148)
         self.assertEqual(tile.header.ft_bin_byte_length, 15000)
         self.assertEqual(tile.header.bt_json_byte_length, 0)
         self.assertEqual(tile.header.bt_bin_byte_length, 0)
 
         feature_table = tile.body.feature_table
-        feature = feature_table.feature(0)
-        dcol_res = {'Red': 44, 'Blue': 209, 'Green': 243}
-        self.assertDictEqual(dcol_res, feature.colors)
+        pt_color = feature_table.get_feature_color_at(0)
+        if pt_color is None:
+            raise RuntimeError("pt_color should not be None")
+        assert_array_equal(
+            np.array([44, 243, 209], dtype=np.uint8),
+            pt_color,
+        )
 
 
 class TestTileBuilder(unittest.TestCase):
-
-    def test_build_without_colors(self):
-        tread = TileContentReader().read_file(Path('tests/fixtures/pointCloudRGB.pnts'))
-        f0_ref = tread.body.feature_table.feature(0).positions
-
-        # numpy dtype for positions and colors
-        pdt = np.dtype([('X', '<f4'), ('Y', '<f4'), ('Z', '<f4')])
+    def test_build_without_colors(self) -> None:
+        tread = read_binary_tile_content(Path("tests/fixtures/pointCloudRGB.pnts"))
+        feature_0_position = tread.body.feature_table.get_feature_position_at(0)
 
         # create features
-        features = []
-        for i in range(0, tread.body.feature_table.header.points_length):
-            f = tread.body.feature_table.feature(i)
-            p = f.positions
-            pos = np.array([(p['X'], p['Y'], p['Z'])], dtype=pdt).view('uint8')
-            newf = Feature.from_array(pdt, pos)
-            features.append(newf)
+        positions = []
+        for i in range(tread.body.feature_table.header.points_length):
+            feature_position = tread.body.feature_table.get_feature_position_at(i)
+            positions.append(feature_position)
+        position_array = np.array(positions).flatten()
 
         # create a tile
-        t = Pnts.from_features(pdt, None, features)
+        feature_table_header = FeatureTableHeader.from_semantic(
+            SemanticPoint.POSITION,
+            None,
+            None,
+            len(positions),
+        )
+        t = Pnts.from_features(feature_table_header, position_array)
 
         # configure the tile
-        rtc = [1215012.8828876738, -4736313.051199594, 4081605.22126042]
+        rtc = (1215012.8828876738, -4736313.051199594, 4081605.22126042)
         t.body.feature_table.header.rtc = rtc
 
         # get an array
         tile_arr = t.to_array()
         t2 = Pnts.from_array(tile_arr)
         self.assertEqual(t2.header.version, 1.0)
+
+        # Test the tile byte length
         self.assertEqual(t2.header.tile_byte_length, 12152)
+        self.assertEqual(
+            t2.header.tile_byte_length % 8, 0
+        )  # tile bytes must be 8-byte aligned
+
+        # Test the feature table byte lengths
+        json_feature_table_end = PntsHeader.BYTE_LENGTH + t2.header.ft_json_byte_length
+        self.assertEqual(json_feature_table_end % 8, 0)
         self.assertEqual(t2.header.ft_json_byte_length, 124)
+        bin_feature_table_end = json_feature_table_end + t2.header.ft_bin_byte_length
+        self.assertEqual(bin_feature_table_end % 8, 0)
         self.assertEqual(t2.header.ft_bin_byte_length, 12000)
+
         self.assertEqual(t2.header.bt_json_byte_length, 0)
         self.assertEqual(t2.header.bt_bin_byte_length, 0)
 
         feature_table = t.body.feature_table
-        f0 = feature_table.feature(0).positions
 
-        self.assertAlmostEqual(f0_ref['X'], f0['X'])
-        self.assertAlmostEqual(f0_ref['Y'], f0['Y'])
-        self.assertAlmostEqual(f0_ref['Z'], f0['Z'])
-
-    def test_build(self):
-        tread = TileContentReader().read_file(Path('tests/fixtures/pointCloudRGB.pnts'))
-
-        # numpy dtype for positions and colors
-        pdt = np.dtype([('X', '<f4'), ('Y', '<f4'), ('Z', '<f4')])
-        cdt = np.dtype([('Red', 'u1'), ('Green', 'u1'), ('Blue', 'u1')])
+        assert_array_equal(feature_0_position, feature_table.get_feature_position_at(0))
+
+    def test_build(self) -> None:
+        tread = read_binary_tile_content(Path("tests/fixtures/pointCloudRGB.pnts"))
 
         # create features
-        features = []
-        for i in range(0, tread.body.feature_table.header.points_length):
-            f = tread.body.feature_table.feature(i)
-            p = f.positions
-            c = f.colors
-            pos = np.array([(p['X'], p['Y'], p['Z'])], dtype=pdt).view('uint8')
-            col = np.array([(c['Red'], c['Green'], c['Blue'])],
-                           dtype=cdt).view('uint8')
-            newf = Feature.from_array(pdt, pos, cdt, col)
-            features.append(newf)
+        positions = []
+        colors = []
+        for i in range(tread.body.feature_table.header.points_length):
+            (
+                feature_position,
+                feature_color,
+                _,
+            ) = tread.body.feature_table.get_feature_at(i)
+            positions.append(feature_position)
+            colors.append(feature_color)
+        position_array = np.array(positions).flatten()
+        color_array = np.array(colors).flatten()
 
         # create a tile
-        t = Pnts.from_features(pdt, cdt, features)
+        feature_table_header = FeatureTableHeader.from_semantic(
+            SemanticPoint.POSITION, SemanticPoint.RGB, None, len(positions)
+        )
+        t = Pnts.from_features(feature_table_header, position_array, color_array)
 
         # configure the tile
-        rtc = [1215012.8828876738, -4736313.051199594, 4081605.22126042]
+        rtc = (1215012.8828876738, -4736313.051199594, 4081605.22126042)
         t.body.feature_table.header.rtc = rtc
 
         # get an array
         tile_arr = t.to_array()
         t2 = Pnts.from_array(tile_arr)
         self.assertEqual(t2.header.version, 1.0)
+
+        # Test the tile byte length
         self.assertEqual(t2.header.tile_byte_length, 15176)
+        self.assertEqual(
+            t2.header.tile_byte_length % 8, 0
+        )  # tile bytes must be 8-byte aligned
+
+        # Test the feature table byte lengths
+        json_feature_table_end = PntsHeader.BYTE_LENGTH + t2.header.ft_json_byte_length
+        self.assertEqual(json_feature_table_end % 8, 0)
         self.assertEqual(t2.header.ft_json_byte_length, 148)
+        bin_feature_table_end = json_feature_table_end + t2.header.ft_bin_byte_length
+        self.assertEqual(bin_feature_table_end % 8, 0)
         self.assertEqual(t2.header.ft_bin_byte_length, 15000)
+
         self.assertEqual(t2.header.bt_json_byte_length, 0)
         self.assertEqual(t2.header.bt_bin_byte_length, 0)
 
         feature_table = t.body.feature_table
-        feature = feature_table.feature(0)
-        dcol_res = {'Red': 44, 'Blue': 209, 'Green': 243}
-        self.assertDictEqual(dcol_res, feature.colors)
-
-        # t2.save_as("/tmp/py3dtiles_test_build_1.pnts")
+        pt_color = feature_table.get_feature_color_at(0)
+        if pt_color is None:
+            raise RuntimeError("pt_color should not be None")
+        assert_array_equal(
+            np.array([44, 243, 209], dtype=np.uint8),
+            pt_color,
+        )
```

### Comparing `py3dtiles-5.0.0/tests/test_reader.py` & `py3dtiles-6.0.0/tests/test_reader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,75 +1,93 @@
 """Test the point cloud readers.
 
 The example that is run in the test (`simple.ply`) comes from the [CGAL repository](https://github.com/CGAL/cgal/blob/master/Data/data/points_3/b9_training.ply). Thanks to their maintainers (for more details, please refer to CGAL, Computational Geometry Algorithms Library, https://www.cgal.org):
 
 """
 
 from pathlib import Path
+from typing import Any, Dict, Generator
 
 import numpy as np
-import numpy.typing as npt
 import plyfile
 from pytest import fixture, raises
-import zmq
 
-from py3dtiles.convert import URI
 from py3dtiles.reader import ply_reader
-from py3dtiles.utils import compute_spacing
 
 
-DATA_DIRECTORY = Path(__file__).parent / 'fixtures'
+DATA_DIRECTORY = Path(__file__).parent / "fixtures"
 
 
 @fixture
-def ply_filepath():
+def ply_filepath() -> Generator[Path, None, None]:
     yield DATA_DIRECTORY / "simple.ply"
 
 
 @fixture
-def buggy_ply_filepath():
+def buggy_ply_filepath() -> Generator[Path, None, None]:
     yield DATA_DIRECTORY / "buggy.ply"
 
 
 @fixture(params=["wrongname", "vertex"])
-def buggy_ply_data(request):
+def buggy_ply_data(request) -> Generator[Dict[str, Any], None, None]:  # type: ignore [no-untyped-def]
     """This ply data does not contain any 'vertex' element!"""
-    types = [('x', np.float32, (5,)), ('y', np.float32, (5,)), ('z', np.float32, (5,))]
+    types = [("x", np.float32, (5,)), ("y", np.float32, (5,)), ("z", np.float32, (5,))]
     data = [(np.random.sample(5), np.random.sample(5), np.random.sample(5))]
-    arr = np.array(
-        data if request.param == "wrongname" else [data[0][:2]],
-        dtype=np.dtype(types) if request.param == "wrongname" else np.dtype(types[:2]),
-    )
+    if request.param == "wrongname":
+        arr = np.array(data, dtype=np.dtype(types))
+    else:
+        arr = np.array([data[0][:2]], np.dtype(types[:2]))
     ply_item = plyfile.PlyElement.describe(data=arr, name=request.param)
     ply_data = plyfile.PlyData(elements=[ply_item])
     yield {
         "data": ply_data,
-        "msg": "vertex" if request.param == "wrongname" else "x, y, z"
+        "msg": "vertex" if request.param == "wrongname" else "x, y, z",
     }
 
 
-def test_ply_get_metadata(ply_filepath):
+def test_ply_get_metadata(ply_filepath: Path) -> None:
     ply_metadata = ply_reader.get_metadata(path=ply_filepath)
     expected_point_count = 22300
     expected_aabb = (
-        np.array([5.966480625e+05, 2.43620015625e+05, 7.350153350830078e+01]),
-        np.array([5.967389375e+05, 2.43731984375e+05, 9.718580627441406e+01]),
+        np.array([5.966480625e05, 2.43620015625e05, 7.350153350830078e01]),
+        np.array([5.967389375e05, 2.43731984375e05, 9.718580627441406e01]),
     )
     assert list(ply_metadata.keys()) == [
-        "portions", "aabb", "color_scale", "srs_in", "point_count", "avg_min"
-    ]
-    assert ply_metadata["portions"] == [
-        (str(ply_filepath), (0, expected_point_count, expected_point_count))
+        "portions",
+        "aabb",
+        "crs_in",
+        "point_count",
+        "avg_min",
     ]
+    assert ply_metadata["portions"] == [(str(ply_filepath), (0, expected_point_count))]
     assert np.all(ply_metadata["aabb"][0] == expected_aabb[0])
     assert np.all(ply_metadata["aabb"][1] == expected_aabb[1])
-    assert ply_metadata["color_scale"] is None
-    assert ply_metadata["srs_in"] is None
+    assert ply_metadata["crs_in"] is None
     assert ply_metadata["point_count"] == expected_point_count
     assert np.all(ply_metadata["avg_min"] == expected_aabb[0])
 
 
-def test_ply_get_metadata_buggy(buggy_ply_data, buggy_ply_filepath):
+def test_ply_get_metadata_buggy(
+    buggy_ply_data: Dict[str, Any], buggy_ply_filepath: Path
+) -> None:
     buggy_ply_data["data"].write(buggy_ply_filepath)
     with raises(KeyError, match=buggy_ply_data["msg"]):
         _ = ply_reader.get_metadata(path=buggy_ply_filepath)
     buggy_ply_filepath.unlink()
+
+
+def test_create_plydata_with_renamed_property(ply_filepath: Path) -> None:
+    ply_data = plyfile.PlyData.read(ply_filepath)
+    modified_ply_data = ply_reader.create_plydata_with_renamed_property(
+        ply_data, "label", "classification"
+    )
+    for prop1, prop2 in zip(
+        ply_data["vertex"].properties, modified_ply_data["vertex"].properties
+    ):
+        assert prop1.name == prop2.name or (
+            prop1.name == "label" and prop2.name == "classification"
+        )
+    for dtype1, dtype2 in zip(
+        ply_data["vertex"].data.dtype.names,
+        modified_ply_data["vertex"].data.dtype.names,
+    ):
+        assert dtype1 == dtype2 or (dtype1 == "label" and dtype2 == "classification")
```

### Comparing `py3dtiles-5.0.0/tests/test_shared_node_store.py` & `py3dtiles-6.0.0/tests/test_shared_node_store.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 import shutil
 import unittest
 
 from py3dtiles.tilers.node import SharedNodeStore
 
 
 class TestSharedNodeStore(unittest.TestCase):
-    TMP_DIR = Path('tmp/')
-    def test_remove_oldest_nodes(self):
+    TMP_DIR = Path("tmp/")
+
+    def test_remove_oldest_nodes(self) -> None:
         shared_node_store = SharedNodeStore(TestSharedNodeStore.TMP_DIR)
 
         self.assertEqual(len(shared_node_store.data), 0)
         self.assertEqual(len(shared_node_store.metadata), 0)
 
-        shared_node_store.put(b'0', b"11111111")
+        shared_node_store.put(b"0", b"11111111")
 
         self.assertEqual(len(shared_node_store.data), 1)
         self.assertEqual(len(shared_node_store.metadata), 1)
 
         shared_node_store.remove_oldest_nodes()
 
         self.assertEqual(len(shared_node_store.data), 0)
```

### Comparing `py3dtiles-5.0.0/tests/test_wkb_utils.py` & `py3dtiles-6.0.0/tests/test_wkb_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,73 +1,75 @@
 import json
 
 import numpy as np
 import pytest
+from pytest_benchmark.fixture import BenchmarkFixture
 
 from py3dtiles.tilers.b3dm import wkb_utils
+from py3dtiles.tilers.b3dm.wkb_utils import PolygonType
 
 
 @pytest.fixture
-def clockwise_star():
-    with open('tests/fixtures/star_clockwise.geojson') as f:
+def clockwise_star() -> PolygonType:
+    with open("tests/fixtures/star_clockwise.geojson") as f:
         star_geo = json.load(f)
-        coords = star_geo['features'][0]['geometry']['coordinates']
+        coords: PolygonType = star_geo["features"][0]["geometry"]["coordinates"]
         # triangulate expects the coordinates to be numpy array
         polygon = coords[0]
         for i in range(len(polygon)):
             polygon[i] = np.array(polygon[i], dtype=np.float32)
         # triangulate implicitly use wkb format, which is not self-closing
         del polygon[-1]
         return coords
 
 
 @pytest.fixture
-def counterclockwise_star():
-    with open('tests/fixtures/star_counterclockwise.geojson') as f:
+def counterclockwise_star() -> PolygonType:
+    with open("tests/fixtures/star_counterclockwise.geojson") as f:
         star_geo = json.load(f)
-        coords = star_geo['features'][0]['geometry']['coordinates']
+        coords: PolygonType = star_geo["features"][0]["geometry"]["coordinates"]
         # triangulate expects the coordinates to be numpy array
         polygon = coords[0]
         for i in range(len(polygon)):
             polygon[i] = np.array(polygon[i], dtype=np.float32)
         # triangulate implicitly use wkb format, which is not self-closing
         del polygon[-1]
         return coords
 
 
 @pytest.fixture
-def counterclockwise_zx_star():
-    with open('tests/fixtures/star_zx_counter_clockwise.geojson') as f:
+def counterclockwise_zx_star() -> PolygonType:
+    with open("tests/fixtures/star_zx_counter_clockwise.geojson") as f:
         star_geo = json.load(f)
-        coords = star_geo['features'][0]['geometry']['coordinates']
+        coords: PolygonType = star_geo["features"][0]["geometry"]["coordinates"]
         # triangulate expects the coordinates to be numpy array
         polygon = coords[0]
         for i in range(len(polygon)):
             polygon[i] = np.array(polygon[i], dtype=np.float32)
         # triangulate implicitly use wkb format, which is not self-closing
         del polygon[-1]
         return coords
 
 
 @pytest.fixture
-def big_poly():
-    with open('tests/fixtures/big_polygon_counter_clockwise.geojson') as f:
+def big_poly() -> PolygonType:
+    with open("tests/fixtures/big_polygon_counter_clockwise.geojson") as f:
         big_poly = json.load(f)
-        coords = big_poly['features'][0]['geometry']['coordinates']
+        coords: PolygonType = big_poly["features"][0]["geometry"]["coordinates"]
         # triangulate expects the coordinates to be numpy array
         polygon = coords[0]
         for i in range(len(polygon)):
             polygon[i] = np.array(polygon[i], dtype=np.float32)
         # triangulate implicitly use wkb format, which is not self-closing
         del polygon[-1]
         return coords
 
 
 @pytest.fixture
-def complex_polygon():
+def complex_polygon() -> PolygonType:
     # tricky polygon 1:
     # 0x---------x 4
     #   \        |
     #    \       |
     #   1 x      |
     #    /       |
     #   /        |
@@ -75,126 +77,145 @@
     # the first few vertices seems to indicate an inverse winding order
     return [
         [
             np.array([0, 1, 0], dtype=np.float32),
             np.array([0.5, 0.5, 0], dtype=np.float32),
             np.array([0, 0, 0], dtype=np.float32),
             np.array([1, 0, 0], dtype=np.float32),
-            np.array([1, 1, 0], dtype=np.float32)
+            np.array([1, 1, 0], dtype=np.float32),
         ]
     ]
 
 
-def test_triangulate_winding_order_simple():
+def test_triangulate_winding_order_simple() -> None:
     # simple case: a square on xy plane, counter-clockwise
     polygon = [
         [
             np.array([0, 0, 0], dtype=np.float32),
             np.array([1, 0, 0], dtype=np.float32),
             np.array([1, 1, 0], dtype=np.float32),
-            np.array([0, 1, 0], dtype=np.float32)
+            np.array([0, 1, 0], dtype=np.float32),
         ]
     ]
 
     triangles = wkb_utils.triangulate(polygon)
-    assert len(triangles[0]) == 2, 'Should generate 2 triangles'
-    assert \
-        all(np.cross(
+    assert len(triangles[0]) == 2, "Should generate 2 triangles"
+    assert all(
+        np.cross(
             triangles[0][0][1] - triangles[0][0][0],
-            triangles[0][0][2] - triangles[0][0][0]) == np.array([0, 0, 1], dtype=np.float32)), \
-        'Check winding order is coherent with vertex order: counter-clockwise (triangle 1)'
-    assert \
-        all(np.cross(
+            triangles[0][0][2] - triangles[0][0][0],
+        )
+        == np.array([0, 0, 1], dtype=np.float32)
+    ), "Check winding order is coherent with vertex order: counter-clockwise (triangle 1)"
+    assert all(
+        np.cross(
             triangles[0][1][1] - triangles[0][1][0],
-            triangles[0][1][2] - triangles[0][1][0]) == np.array([0, 0, 1], dtype=np.float32)), \
-        'Check winding order is coherent with vertex order: counter-clockwise (triangle 2)'
+            triangles[0][1][2] - triangles[0][1][0],
+        )
+        == np.array([0, 0, 1], dtype=np.float32)
+    ), "Check winding order is coherent with vertex order: counter-clockwise (triangle 2)"
 
     # simple case 2: a square on xy plane, clockwise
     polygon = [
         [
             np.array([0, 0, 0], dtype=np.float32),
             np.array([0, 1, 0], dtype=np.float32),
             np.array([1, 1, 0], dtype=np.float32),
-            np.array([1, 0, 0], dtype=np.float32)
+            np.array([1, 0, 0], dtype=np.float32),
         ]
     ]
     triangles = wkb_utils.triangulate(polygon)
-    assert len(triangles[0]) == 2, 'Should generate 2 triangles'
-    assert \
-        all(np.cross(
+    assert len(triangles[0]) == 2, "Should generate 2 triangles"
+    assert all(
+        np.cross(
             triangles[0][0][1] - triangles[0][0][0],
-            triangles[0][0][2] - triangles[0][0][0]) == np.array([0, 0, -1], dtype=np.float32)), \
-        'Check winding order is coherent with vertex order: clockwise (triangle1)'
-    assert \
-        all(np.cross(
+            triangles[0][0][2] - triangles[0][0][0],
+        )
+        == np.array([0, 0, -1], dtype=np.float32)
+    ), "Check winding order is coherent with vertex order: clockwise (triangle1)"
+    assert all(
+        np.cross(
             triangles[0][1][1] - triangles[0][1][0],
-            triangles[0][1][2] - triangles[0][1][0]) == np.array([0, 0, -1], dtype=np.float32)), \
-        'Check winding order is coherent with vertex order: clockwise (triangle2)'
+            triangles[0][1][2] - triangles[0][1][0],
+        )
+        == np.array([0, 0, -1], dtype=np.float32)
+    ), "Check winding order is coherent with vertex order: clockwise (triangle2)"
 
 
-def test_triangulate_winding_order_complex(complex_polygon):
+def test_triangulate_winding_order_complex(complex_polygon: PolygonType) -> None:
     triangles = wkb_utils.triangulate(complex_polygon)
-    assert len(triangles[0]) == 3, 'Should generate 2 triangles'
+    assert len(triangles[0]) == 3, "Should generate 2 triangles"
     crossprod_triangle1 = np.cross(
-        triangles[0][0][1] - triangles[0][0][0],
-        triangles[0][0][2] - triangles[0][0][0]
+        triangles[0][0][1] - triangles[0][0][0], triangles[0][0][2] - triangles[0][0][0]
     )
     crossprod_triangle1 /= np.linalg.norm(crossprod_triangle1)
-    assert \
-        all(crossprod_triangle1 == np.array([0, 0, 1], dtype=np.float32)), \
-        'Check winding order is coherent with vertex order: counter-clockwise'
+    assert all(
+        crossprod_triangle1 == np.array([0, 0, 1], dtype=np.float32)
+    ), "Check winding order is coherent with vertex order: counter-clockwise"
 
 
-def test_triangulate_winding_order_stars(clockwise_star):
+def test_triangulate_winding_order_stars(clockwise_star: PolygonType) -> None:
     triangles = wkb_utils.triangulate(clockwise_star)
     crossprod_triangle1 = np.cross(
-        triangles[0][0][1] - triangles[0][0][0],
-        triangles[0][0][2] - triangles[0][0][0])
+        triangles[0][0][1] - triangles[0][0][0], triangles[0][0][2] - triangles[0][0][0]
+    )
     crossprod_triangle1 /= np.linalg.norm(crossprod_triangle1)
-    assert all(crossprod_triangle1 == np.array([0, 0, -1], dtype=np.float32)), \
-        'Check winding order is coherent with vertex order: clockwise'
+    assert all(
+        crossprod_triangle1 == np.array([0, 0, -1], dtype=np.float32)
+    ), "Check winding order is coherent with vertex order: clockwise"
 
 
-def test_triangulate_winding_order_counter_clockwise_stars(counterclockwise_star):
+def test_triangulate_winding_order_counter_clockwise_stars(
+    counterclockwise_star: PolygonType,
+) -> None:
     triangles = wkb_utils.triangulate(counterclockwise_star)
     crossprod_triangle1 = np.cross(
-        triangles[0][0][1] - triangles[0][0][0],
-        triangles[0][0][2] - triangles[0][0][0])
+        triangles[0][0][1] - triangles[0][0][0], triangles[0][0][2] - triangles[0][0][0]
+    )
     crossprod_triangle1 /= np.linalg.norm(crossprod_triangle1)
-    assert all(crossprod_triangle1 == np.array([0, 0, 1], dtype=np.float32)), \
-        'Check winding order is coherent with vertex order: counter-clockwise'
+    assert all(
+        crossprod_triangle1 == np.array([0, 0, 1], dtype=np.float32)
+    ), "Check winding order is coherent with vertex order: counter-clockwise"
 
 
-def test_triangulate_winding_order_counter_clockwise_zx_stars(counterclockwise_zx_star):
+def test_triangulate_winding_order_counter_clockwise_zx_stars(
+    counterclockwise_zx_star: PolygonType,
+) -> None:
     triangles = wkb_utils.triangulate(counterclockwise_zx_star)
     crossprod_triangle1 = np.cross(
-        triangles[0][0][1] - triangles[0][0][0],
-        triangles[0][0][2] - triangles[0][0][0])
+        triangles[0][0][1] - triangles[0][0][0], triangles[0][0][2] - triangles[0][0][0]
+    )
     crossprod_triangle1 /= np.linalg.norm(crossprod_triangle1)
     # check the 2nd dimension is the largest by far and is positive
-    assert crossprod_triangle1[1] > 0.8,\
-        'Check winding order is coherent with vertex order: counter-clockwise in zx plane'
+    assert (
+        crossprod_triangle1[1] > 0.8
+    ), "Check winding order is coherent with vertex order: counter-clockwise in zx plane"
 
 
-def test_big_poly_winding_order(big_poly):
+def test_big_poly_winding_order(big_poly: PolygonType) -> None:
     triangles = wkb_utils.triangulate(big_poly)
     crossprod_triangle1 = np.cross(
-        triangles[0][0][1] - triangles[0][0][0],
-        triangles[0][0][2] - triangles[0][0][0])
+        triangles[0][0][1] - triangles[0][0][0], triangles[0][0][2] - triangles[0][0][0]
+    )
     crossprod_triangle1 /= np.linalg.norm(crossprod_triangle1)
-    assert all(crossprod_triangle1 == np.array([0, 0, 1], dtype=np.float32)), \
-        'Check winding order is coherent with vertex order: counter-clockwise'
+    assert all(
+        crossprod_triangle1 == np.array([0, 0, 1], dtype=np.float32)
+    ), "Check winding order is coherent with vertex order: counter-clockwise"
 
 
 ################
 # benchmarking #
 ################
-def test_benchmark_triangulate(complex_polygon, benchmark):
+def test_benchmark_triangulate(
+    complex_polygon: PolygonType, benchmark: BenchmarkFixture
+) -> None:
     benchmark(wkb_utils.triangulate, complex_polygon)
 
 
-def test_benchmark_star(clockwise_star, benchmark):
+def test_benchmark_star(
+    clockwise_star: PolygonType, benchmark: BenchmarkFixture
+) -> None:
     benchmark(wkb_utils.triangulate, clockwise_star)
 
 
-def test_benchmark_big_poly(big_poly, benchmark):
+def test_benchmark_big_poly(big_poly: PolygonType, benchmark: BenchmarkFixture) -> None:
     benchmark(wkb_utils.triangulate, big_poly)
```

