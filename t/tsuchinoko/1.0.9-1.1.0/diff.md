# Comparing `tmp/tsuchinoko-1.0.9.tar.gz` & `tmp/tsuchinoko-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsuchinoko-1.0.9.tar", last modified: Thu Mar 16 18:22:25 2023, max compression
+gzip compressed data, was "tsuchinoko-1.1.0.tar", last modified: Tue Jul 25 20:48:31 2023, max compression
```

## Comparing `tsuchinoko-1.0.9.tar` & `tsuchinoko-1.1.0.tar`

### file list

```diff
@@ -1,95 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.905186 tsuchinoko-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-16 18:22:25.905186 tsuchinoko-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.897186 tsuchinoko-1.0.9/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.897186 tsuchinoko-1.0.9/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/legal.txt
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-16 18:22:25.905186 tsuchinoko-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.897186 tsuchinoko-1.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tests/test_graphics_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tests/test_gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.905186 tsuchinoko-1.0.9/tsuchinoko/
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-16 18:22:25.905186 tsuchinoko-1.0.9/tsuchinoko/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.897186 tsuchinoko-1.0.9/tsuchinoko/adaptive/
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/adaptive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/adaptive/_adaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/adaptive/acquisition_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/adaptive/adaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/adaptive/fvgp_gpCAM_in_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/adaptive/gpCAM_in_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/adaptive/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    17537 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/adaptive/quadtree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/adaptive/random_in_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.897186 tsuchinoko-1.0.9/tsuchinoko/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.901186 tsuchinoko-1.0.9/tsuchinoko/core/
--rw-r--r--   0 runner    (1001) docker     (123)    11271 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/core/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.901186 tsuchinoko-1.0.9/tsuchinoko/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/examples/IRBL_server_demo_LC.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/examples/_launch_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/examples/adaptive_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/examples/client_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/examples/grid_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/examples/headless_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/examples/high_dimensionality_server_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/examples/ir_server_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/examples/multi_task_server_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/examples/quadtree_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/examples/server_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/examples/server_demo_bluesky.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/examples/vector_metric_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.901186 tsuchinoko-1.0.9/tsuchinoko/execution/
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/execution/bluesky_in_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/execution/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/execution/threaded_in_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.901186 tsuchinoko-1.0.9/tsuchinoko/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.901186 tsuchinoko-1.0.9/tsuchinoko/graphics_items/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/graphics_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24019 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/graphics_items/clouditem.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/graphics_items/indicatoritem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/graphics_items/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.901186 tsuchinoko-1.0.9/tsuchinoko/graphs/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/graphs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/graphs/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.901186 tsuchinoko-1.0.9/tsuchinoko/parameters/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/parameters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.901186 tsuchinoko-1.0.9/tsuchinoko/plan_stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/plan_stubs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.905186 tsuchinoko-1.0.9/tsuchinoko/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/utils/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/utils/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/utils/mutex.py
--rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/utils/runengine.py
--rw-r--r--   0 runner    (1001) docker     (123)    13395 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/utils/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.905186 tsuchinoko-1.0.9/tsuchinoko/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/widgets/debugmenubar.py
--rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/widgets/displays.py
--rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/widgets/graph_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    17741 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/tsuchinoko/widgets/mainwindow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:22:25.897186 tsuchinoko-1.0.9/tsuchinoko.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-16 18:22:25.000000 tsuchinoko-1.0.9/tsuchinoko.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-03-16 18:22:25.000000 tsuchinoko-1.0.9/tsuchinoko.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 18:22:25.000000 tsuchinoko-1.0.9/tsuchinoko.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-16 18:22:25.000000 tsuchinoko-1.0.9/tsuchinoko.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-03-16 18:22:25.000000 tsuchinoko-1.0.9/tsuchinoko.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-16 18:22:25.000000 tsuchinoko-1.0.9/tsuchinoko.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-03-16 18:22:17.000000 tsuchinoko-1.0.9/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.555759 tsuchinoko-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-07-25 20:48:31.555759 tsuchinoko-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.547758 tsuchinoko-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.547758 tsuchinoko-1.1.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/legal.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-25 20:48:31.555759 tsuchinoko-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.547758 tsuchinoko-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tests/test_graphics_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tests/test_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.555759 tsuchinoko-1.1.0/tsuchinoko/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-25 20:48:31.555759 tsuchinoko-1.1.0/tsuchinoko/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.551759 tsuchinoko-1.1.0/tsuchinoko/adaptive/
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/adaptive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/adaptive/_adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/adaptive/acquisition_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/adaptive/adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/adaptive/fvgp_gpCAM_in_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/adaptive/gpCAM_in_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/adaptive/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17537 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/adaptive/quadtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/adaptive/random_in_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.551759 tsuchinoko-1.1.0/tsuchinoko/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.551759 tsuchinoko-1.1.0/tsuchinoko/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    12841 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/core/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.551759 tsuchinoko-1.1.0/tsuchinoko/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/examples/IRBL_server_demo_LC.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/examples/_launch_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/examples/adaptive_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/examples/bluesky_adaptive_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/examples/client_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/examples/grid_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/examples/headless_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/examples/high_dimensionality_server_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/examples/ir_server_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/examples/multi_task_server_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/examples/quadtree_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/examples/server_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/examples/server_demo_bluesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/examples/vector_metric_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.551759 tsuchinoko-1.1.0/tsuchinoko/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/execution/bluesky_adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/execution/bluesky_in_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/execution/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/execution/threaded_in_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.551759 tsuchinoko-1.1.0/tsuchinoko/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.551759 tsuchinoko-1.1.0/tsuchinoko/graphics_items/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/graphics_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24019 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/graphics_items/clouditem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/graphics_items/indicatoritem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13024 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/graphics_items/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.551759 tsuchinoko-1.1.0/tsuchinoko/graphs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/graphs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19804 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/graphs/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.551759 tsuchinoko-1.1.0/tsuchinoko/parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/parameters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.555759 tsuchinoko-1.1.0/tsuchinoko/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/patches/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/patches/pyqode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/patches/pyqtgraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.555759 tsuchinoko-1.1.0/tsuchinoko/plan_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/plan_stubs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.555759 tsuchinoko-1.1.0/tsuchinoko/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/utils/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/utils/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/utils/mutex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/utils/runengine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13395 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/utils/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.555759 tsuchinoko-1.1.0/tsuchinoko/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/widgets/debugmenubar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/widgets/displays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/widgets/graph_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19662 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/widgets/mainwindow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/widgets/server_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/tsuchinoko/widgets/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:48:31.547758 tsuchinoko-1.1.0/tsuchinoko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-07-25 20:48:31.000000 tsuchinoko-1.1.0/tsuchinoko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-25 20:48:31.000000 tsuchinoko-1.1.0/tsuchinoko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 20:48:31.000000 tsuchinoko-1.1.0/tsuchinoko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-25 20:48:31.000000 tsuchinoko-1.1.0/tsuchinoko.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-25 20:48:31.000000 tsuchinoko-1.1.0/tsuchinoko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-25 20:48:31.000000 tsuchinoko-1.1.0/tsuchinoko.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-25 20:48:22.000000 tsuchinoko-1.1.0/versioneer.py
```

### Comparing `tsuchinoko-1.0.9/CONTRIBUTING.rst` & `tsuchinoko-1.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/LICENSE` & `tsuchinoko-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/PKG-INFO` & `tsuchinoko-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: tsuchinoko
-Version: 1.0.9
-Summary: An adaptive optics alignment tool for ALS beamlines utilizing gpCAM.
-Home-page: https://github.com/lbl-camera/tsuchinoko
-Author: Ronald J Pandolfi
-Author-email: ronpandolfi@lbl.gov
-License: GPLv3+
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
-Provides-Extra: tests
-License-File: LICENSE
-License-File: AUTHORS.rst
-
 # Tsuchinoko
 [![PyPI](https://badgen.net/pypi/v/tsuchinoko)](https://pypi.org/project/tsuchinoko/)
 [![License](https://badgen.net/pypi/license/tsuchinoko)](https://github.com/lbl-camera/tsuchinoko)
 [![Build Status](https://github.com/lbl-camera/tsuchinoko/actions/workflows/main.yml/badge.svg)](https://github.com/lbl-camera/tsuchinoko/actions/workflows/main.yml)
 [![Documentation Status](https://readthedocs.org/projects/tsuchinoko/badge/?version=latest)](https://tsuchinoko.readthedocs.io/en/latest/?badge=latest)
 [![Test Coverage](https://img.shields.io/codecov/c/github/lbl-camera/tsuchinoko/master.svg)](https://codecov.io/github/lbl-camera/tsuchinoko?branch=master)
 [![Slack Status](https://img.shields.io/badge/slack-gpCAM-yellow.svg?logo=slack)](https://nikea.slack.com/messages/U7Q1N42F6)
@@ -35,24 +15,32 @@
 powerful Gaussian process regression at the core.
 
 A Tsuchinoko system includes 4 distinct components: the GUI client, an adaptive engine, and execution engine, and a
 core service. These components are separable to allow flexibility with a variety of distributed designs.
 
 ![Tsuchinoko running simulated measurements](docs/source/_static/running-score.PNG)
 
-## Installation
+## Standard Installation
 
-The latest stable Tsuchinoko version is available on PyPI, and is installable with `pip`.
+The latest stable Tsuchinoko version is available on PyPI, and is installable with `pip`. It is recommended that you
+use Python 3.9 for this installation.
 
 ```bash
 pip install tsuchinoko
 ```
 
 For more information, see the [installation documentation](https://tsuchinoko.readthedocs.io/en/latest/quickstart.html).
 
+## Easy Installation
+
+For Mac OSX and Windows, pre-packaged installers are available. These do not require a base Python installation. See the [installation documentation](https://tsuchinoko.readthedocs.io/en/latest/installers.html) for more details.
+
+- [Latest Windows Installer](https://github.com/lbl-camera/tsuchinoko/releases/latest/download/Tsuchinoko-amd64.exe)
+- [Latest Mac OSX Installer](https://github.com/lbl-camera/tsuchinoko/releases/latest/download/Tsuchinoko.app.tgz)
+
 ## Resources
 
 * Documentation: https://tsuchinoko.readthedocs.io/en/latest
 * Report an issue in Tsuchinoko: [New Bug Report](https://github.com/lbl-camera/tsuchinoko/issues/new?labels=bug)
 
 ## About the name
```

### Comparing `tsuchinoko-1.0.9/docs/Makefile` & `tsuchinoko-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/docs/make.bat` & `tsuchinoko-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/docs/source/conf.py` & `tsuchinoko-1.1.0/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,23 +110,22 @@
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 html_theme = "sphinx_rtd_theme"
 html_theme_path = [sphinx_rtd_theme.get_html_theme_path()]
-
+html_logo = "_static/tsuchinoko-real.png"
 html_style = 'custom.css'
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 html_theme_options = dict(
-    logo_only=True,
     display_version=True,
     collapse_navigation=False,
     titles_only=False
 )
 
 # user starts in dark mode
 default_dark_mode = True
@@ -201,7 +200,9 @@
     'python': ('https://docs.python.org/3/', None),
     'numpy': ('https://numpy.org/doc/stable/', None),
     'scipy': ('https://docs.scipy.org/doc/scipy/reference/', None),
     'pandas': ('https://pandas.pydata.org/pandas-docs/stable', None),
     'matplotlib': ('https://matplotlib.org/stable', None),
     'pyqtgraph': ("https://pyqtgraph.readthedocs.io/en/latest/", None),
 }
+
+autoclass_content = 'both'
```

### Comparing `tsuchinoko-1.0.9/legal.txt` & `tsuchinoko-1.1.0/legal.txt`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/setup.py` & `tsuchinoko-1.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     packages=find_packages(exclude=['docs', 'tests', 'examples']),
     entry_points={
         "gui_scripts": [
             'tsuchinoko = tsuchinoko:launch_client',
         ],
         "console_scripts": [
             'tsuchinoko_demo = tsuchinoko:launch_server',
+            'tsuchinoko_bootstrap = tsuchinoko:bootstrap'
         ],
     },
     include_package_data=True,
     package_data={
         'tsuchinoko': [
             # When adding files here, remember to update MANIFEST.in as well,
             # or else they will not be included in the distribution on PyPI!
```

### Comparing `tsuchinoko-1.0.9/tests/test_core.py` & `tsuchinoko-1.1.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/tests/test_graphics_items.py` & `tsuchinoko-1.1.0/tests/test_graphics_items.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,20 @@
+import os
+
 import numpy as np
 import pyqtgraph as pg
+import pytest
 import scipy.misc
 
 from tsuchinoko.graphics_items.clouditem import CloudItem
 
+IN_GITHUB_ACTIONS = os.getenv("GITHUB_ACTIONS") == "true"
+
 
+@pytest.mark.skipif(IN_GITHUB_ACTIONS, reason="Test doesn't work in Github Actions.")
 def test_cloud(qtbot, monkeypatch):
     pg.setConfigOption('useOpenGL', True)
     pg.setConfigOption('enableExperimental', True)
 
     # Create window with GraphicsView widget
     win = pg.GraphicsLayoutWidget()
     win.show()  # show widget alone in its own window
```

### Comparing `tsuchinoko-1.0.9/tests/test_gui.py` & `tsuchinoko-1.1.0/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/tsuchinoko/__init__.py` & `tsuchinoko-1.1.0/tsuchinoko/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 from qtpy.QtCore import QEventLoop
 from pyqtgraph import mkQApp
 import ctypes
 import os
 import asyncio
 import importlib
 import sys
+import runpy
 
 from ._version import get_versions
 
 __version__ = get_versions()['version']
 
+from . import patches
 from .utils import runengine
 from . import parameters  # registers parameter types
 
 del get_versions
 
 
 @click.command()
@@ -35,8 +37,18 @@
     sys.exit(qapp.exec_())
 
 
 @click.command()
 @click.argument('demo_name', required=False, default='server_demo')
 def launch_server(demo_name='server_demo'):
     demo_module = importlib.import_module(f'tsuchinoko.examples.{demo_name}')
-    demo_module.core.main()
+    demo_module.core.main()
+
+
+@click.command(context_settings=dict(ignore_unknown_options=True))
+@click.argument('path', required=True)
+@click.argument("args", nargs=-1, type=click.UNPROCESSED)
+def bootstrap(path, args):
+    """A pyinstaller trick to allow launch of python scripts from built exes"""
+    print(path)
+    sys.argv.pop(0)
+    runpy.run_path(path, {}, "__main__")
```

### Comparing `tsuchinoko-1.0.9/tsuchinoko/adaptive/__init__.py` & `tsuchinoko-1.1.0/tsuchinoko/adaptive/__init__.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/tsuchinoko/adaptive/acquisition_functions.py` & `tsuchinoko-1.1.0/tsuchinoko/adaptive/acquisition_functions.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/tsuchinoko/adaptive/adaptive.py` & `tsuchinoko-1.1.0/tsuchinoko/adaptive/adaptive.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/tsuchinoko/adaptive/fvgp_gpCAM_in_process.py` & `tsuchinoko-1.1.0/tsuchinoko/adaptive/fvgp_gpCAM_in_process.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,15 @@
+import sys
+
 import numpy as np
 
 from gpcam.gp_optimizer import  fvGPOptimizer
-from .acquisition_functions import explore_target_100, radical_gradient
 from .gpCAM_in_process import GPCAMInProcessEngine
 from ..graphs.common import GPCamPosteriorCovariance, GPCamAcquisitionFunction, GPCamPosteriorMean, Table
 
-acquisition_functions = {s: s for s in ['variance', 'shannon_ig', 'ucb', 'maximum', 'minimum', 'covariance', 'gradient', 'explore_target_100']}
-acquisition_functions['explore_target_100'] = explore_target_100
-acquisition_functions['radical_gradient'] = radical_gradient
 
 
 class FvgpGPCAMInProcessEngine(GPCAMInProcessEngine):
     """
     A multi-task adaptive engine powered by gpCAM: https://gpcam.readthedocs.io/en/latest/
     """
 
@@ -26,22 +24,34 @@
                            GPCamAcquisitionFunction(),
                            GPCamPosteriorMean(),
                            Table()]
         elif dimensionality > 2:
             self.graphs = [GPCamPosteriorCovariance(),
                            Table()]
 
+    # TODO: refactor this into base
     def init_optimizer(self):
         parameter_bounds = np.asarray([[self.parameters[('bounds', f'axis_{i}_{edge}')]
                                         for edge in ['min', 'max']]
                                        for i in range(self.dimensionality)])
         hyperparameters = np.asarray([self.parameters[('hyperparameters', f'hyperparameter_{i}')]
-                                      for i in range(self.dimensionality + 1)])
+                                      for i in range(self.num_hyperparameters)])
 
         self.optimizer = fvGPOptimizer(self.dimensionality, self.output_dim, self.output_number, parameter_bounds)
-        self.optimizer.tell(np.empty((1, self.dimensionality)), np.empty((1, self.output_number)))  # we'll wipe this out later; required for initialization
-        self.optimizer.init_fvgp(hyperparameters)
+
+        if self.initial_x_data is not None and self.initial_y_data is not None:
+            variance_kwargs = {}
+            if self.initial_v_data is not None:
+                variance_kwargs['variances'] = self.initial_v_data
+            self.optimizer.tell(self.initial_x_data, self.initial_y_data, **variance_kwargs)
+
+        opts = self.gp_opts.copy()
+        # TODO: only fallback to numpy when packaged as an app
+        if sys.platform == 'darwin':
+            opts['compute_device'] = 'numpy'
+
+        self.optimizer.init_fvgp(hyperparameters, **opts)
 
     def _set_hyperparameter(self, parameter, value):
         self.optimizer.gp_initialized = False  # Force re-initialization
         self.optimizer.init_fvgp(np.asarray([self.parameters[('hyperparameters', f'hyperparameter_{i}')]
-                                           for i in range(self.dimensionality + 1)]))
+                                           for i in range(self.num_hyperparameters)]))
```

### Comparing `tsuchinoko-1.0.9/tsuchinoko/adaptive/gpCAM_in_process.py` & `tsuchinoko-1.1.0/tsuchinoko/adaptive/gpCAM_in_process.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,56 @@
+import sys
 import uuid
 from functools import cached_property
+from typing import Callable
 
 import numpy as np
 from pyqtgraph.parametertree.parameterTypes import SimpleParameter, GroupParameter, ListParameter
+from loguru import logger
 
 from gpcam.gp_optimizer import GPOptimizer
 from . import Engine, Data
 from .acquisition_functions import explore_target_100, radical_gradient
-from ..graphs.common import Variance, GPCamPosteriorCovariance, Score, GPCamAcquisitionFunction, GPCamPosteriorMean, Table
+from ..graphs.common import Variance, GPCamPosteriorCovariance, Score, GPCamAcquisitionFunction, GPCamPosteriorMean, Table, HighDimensionalityGPCamPosteriorMean
 from ..parameters import TrainingParameter
 
-acquisition_functions = {s: s for s in ['variance', 'shannon_ig', 'ucb', 'maximum', 'minimum', 'covariance', 'gradient', 'explore_target_100']}
-acquisition_functions['explore_target_100'] = explore_target_100
-acquisition_functions['radical_gradient'] = radical_gradient
+gpcam_acquisition_functions = {s: s for s in ['variance', 'shannon_ig', 'ucb', 'maximum', 'minimum', 'covariance', 'gradient', 'explore_target_100']}
+gpcam_acquisition_functions['explore_target_100'] = explore_target_100
+gpcam_acquisition_functions['radical_gradient'] = radical_gradient
+
+
+def prepend_update_acquisition_functions(acquisition_functions:dict):
+    cpy = gpcam_acquisition_functions.copy()
+    gpcam_acquisition_functions.clear()
+    gpcam_acquisition_functions.update(acquisition_functions)
+    gpcam_acquisition_functions.update(cpy)
 
 
 class GPCAMInProcessEngine(Engine):
     """
     An adaptive engine powered by gpCAM: https://gpcam.readthedocs.io/en/latest/
     """
     default_retrain_globally_at = (20, 50, 100, 400, 1000)
     default_retrain_locally_at = (20, 40, 60, 80, 100, 200, 400, 1000)
 
-    def __init__(self, dimensionality, parameter_bounds, hyperparameters, hyperparameter_bounds, **kwargs):
-        self.kwargs = kwargs
+    def __init__(self, dimensionality, parameter_bounds, hyperparameters, hyperparameter_bounds,
+                 x_data=None, y_data=None, v_data = None, acquisition_functions:dict[str, Callable]=None, gp_opts: dict = None):
         self.dimensionality = dimensionality
+        self.gp_opts = gp_opts or {}
+        self.initial_x_data = x_data
+        self.initial_y_data = y_data
+        self.initial_v_data = v_data
+        self.num_hyperparameters = len(hyperparameters)
+        if acquisition_functions:
+            prepend_update_acquisition_functions(acquisition_functions)
 
         for i in range(dimensionality):
             for j, edge in enumerate(['min', 'max']):
                 self.parameters[('bounds', f'axis_{i}_{edge}')] = parameter_bounds[i][j]
-        for i in range(dimensionality + 1):
+        for i in range(self.num_hyperparameters):
             for j, edge in enumerate(['min', 'max']):
                 self.parameters[('hyperparameters', f'hyperparameter_{i}_{edge}')] = hyperparameter_bounds[i][j]
             self.parameters.child('hyperparameters', f'hyperparameter_{i}').setValue(hyperparameters[i], blockSignal=self._set_hyperparameter)
 
         self.reset()
 
         if dimensionality == 2:
@@ -42,47 +59,58 @@
                            GPCamPosteriorMean(),
                            # GPCamAverageCovariance(),
                            Table(),
                            Variance(),
                            Score()]
         elif dimensionality > 2:
             self.graphs = [GPCamPosteriorCovariance(),
+                           HighDimensionalityGPCamPosteriorMean(dimensions=dimensionality, bounds=parameter_bounds),
                            # GPCamAverageCovariance(),
                            Table()]
 
     def init_optimizer(self):
         parameter_bounds = np.asarray([[self.parameters[('bounds', f'axis_{i}_{edge}')]
                                         for edge in ['min', 'max']]
                                        for i in range(self.dimensionality)])
         hyperparameters = np.asarray([self.parameters[('hyperparameters', f'hyperparameter_{i}')]
-                                      for i in range(self.dimensionality + 1)])
+                                      for i in range(self.num_hyperparameters)])
 
         self.optimizer = GPOptimizer(self.dimensionality, parameter_bounds)
-        self.optimizer.tell(np.empty((1, self.dimensionality)), np.empty((1,)), np.empty((1,)))  # we'll wipe this out later; required for initialization
-        self.optimizer.init_gp(hyperparameters)
+
+        if self.initial_x_data is not None and self.initial_y_data is not None:
+            variance_kwargs = {}
+            if self.initial_v_data is not None:
+                variance_kwargs['variances'] = self.initial_v_data
+            self.optimizer.tell(self.initial_x_data, self.initial_y_data, **variance_kwargs)
+
+        opts = self.gp_opts.copy()
+        # TODO: only fallback to numpy when packaged as an app
+        if sys.platform == 'darwin':
+            opts['compute_device'] = 'numpy'
+        self.optimizer.init_gp(hyperparameters, **opts)
 
     def reset(self):
         self._completed_training = {'global': set(),
                                     'local': set()}
         self.init_optimizer()
 
         self.optimizer.points = np.array([])
         self.optimizer.values = np.array([])
         self.optimizer.variances = np.array([])
 
     @cached_property
     def parameters(self):
         hyper_parameters = [SimpleParameter(title=f'Hyperparameter #{i + 1}', name=f'hyperparameter_{i}', type='float')
-                            for i in range(1 + self.dimensionality)]
+                            for i in range(self.num_hyperparameters)]
         hyper_parameters_bounds = [SimpleParameter(title=f'Hyperparameter #{i + 1} {edge}', name=f'hyperparameter_{i}_{edge}', type='float')
-                                   for i in range(1 + self.dimensionality) for edge in ['min', 'max']]
+                                   for i in range(self.num_hyperparameters) for edge in ['min', 'max']]
         bounds_parameters = [SimpleParameter(title=f'Axis #{i + 1} {edge}', name=f'axis_{i}_{edge}', type='float')
                              for i in range(self.dimensionality) for edge in ['min', 'max']]
         func_parameters = [ListParameter(title='Method', name='method', limits=['global', 'local', 'hgdl']),
-                           ListParameter(title='Acquisition Function', name='acquisition_function', limits=list(acquisition_functions.keys())),
+                           ListParameter(title='Acquisition Function', name='acquisition_function', limits=list(gpcam_acquisition_functions.keys())),
                            SimpleParameter(title='Queue Length', name='n', value=1, type='int'),
                            SimpleParameter(title='Population Size (global only)', name='pop_size', value=20, type='int'),
                            SimpleParameter(title='Tolerance', name='tol', value=1e-6, type='float')]
 
         global_train_parameter = TrainingParameter(title='Train globally at...', name='global_training', addText='Add', children=[
             SimpleParameter(title='N=', name=str(uuid.uuid4()), value=N, type='int') for N in self.default_retrain_globally_at
         ])
@@ -98,43 +126,50 @@
                                         GroupParameter(name='hyperparameters', title='Hyperparameter Bounds', children=hyper_parameters + hyper_parameters_bounds),
                                         global_train_parameter,
                                         local_train_parameter, ]
         return GroupParameter(name='top', children=parameters)
 
     def _set_hyperparameter(self, parameter, value):
         self.optimizer.gp_initialized = False  # Force re-initialization
+        opts = dict()
+        # TODO: only fallback to numpy when packaged as an app
+        if sys.platform == 'darwin':
+            opts['compute_device'] = 'numpy'
         self.optimizer.init_gp(np.asarray([self.parameters[('hyperparameters', f'hyperparameter_{i}')]
-                                           for i in range(self.dimensionality + 1)]))
+                                           for i in range(self.num_hyperparameters)]), **opts)
 
     def update_measurements(self, data: Data):
         with data.r_lock():  # quickly grab values within lock before passing to optimizer
             positions = data.positions.copy()
             scores = data.scores.copy()
             variances = data.variances.copy()
-        self.optimizer.tell(positions, scores, variances)
+        self.optimizer.tell(np.asarray(positions), scores, variances)
 
     def update_metrics(self, data: Data):
         for graph in self.graphs:
-            graph.compute(data, self)
+            try:
+                graph.compute(data, self)
+            except Exception as ex:
+                logger.exception(ex)
 
     def request_targets(self, position):
         kwargs = {key: self.parameters[key] for key in ['acquisition_function', 'method', 'pop_size', 'tol']}
         kwargs.update({'bounds': np.asarray([[self.parameters[('bounds', f'axis_{i}_{edge}')]
                                               for edge in ['min', 'max']]
                                              for i in range(self.dimensionality)])})
         n = self.parameters['n']
-        return self.optimizer.ask(position, n, acquisition_function=acquisition_functions[kwargs.pop('acquisition_function')], **kwargs)['x']
+        return self.optimizer.ask(position, n, acquisition_function=gpcam_acquisition_functions[kwargs.pop('acquisition_function')], **kwargs)['x']
 
     def train(self):
         for method in ['global', 'local']:
             train_at = set(child.value() for child in self.parameters.child(f'{method}_training').children())
 
             for N in train_at:
                 if len(self.optimizer.values) > N and N not in self._completed_training[method]:
                     self.optimizer.train(np.asarray([[self.parameters[('hyperparameters', f'hyperparameter_{i}_{edge}')]
                                                       for edge in ['min', 'max']]
-                                                     for i in range(self.dimensionality + 1)]),
+                                                     for i in range(self.num_hyperparameters)]),
                                          np.asarray([self.parameters[('hyperparameters', f'hyperparameter_{i}')]
-                                                     for i in range(self.dimensionality + 1)]), method=method)
+                                                     for i in range(self.num_hyperparameters)]), method=method)
                     self._completed_training[method].add(N)
                     # return  # only does global training if specified for both
-        return True
+        return True
```

### Comparing `tsuchinoko-1.0.9/tsuchinoko/adaptive/grid.py` & `tsuchinoko-1.1.0/tsuchinoko/adaptive/grid.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/tsuchinoko/adaptive/quadtree.py` & `tsuchinoko-1.1.0/tsuchinoko/adaptive/quadtree.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/tsuchinoko/adaptive/random_in_process.py` & `tsuchinoko-1.1.0/tsuchinoko/adaptive/random_in_process.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/tsuchinoko/core/__init__.py` & `tsuchinoko-1.1.0/tsuchinoko/core/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,27 +25,31 @@
     Paused = auto()
     Resuming = auto()
     Stopping = auto()
     Restarting = auto()
     Exiting = auto()
 
 
+SLEEP_FOR_FRESH_DATA_TIME = .1
+
+
 class Core:
     def __init__(self,
                  execution_engine: ExecutionEngine = None,
                  adaptive_engine: AdaptiveEngine = None):
         self.execution_engine = execution_engine
         self.adaptive_engine = adaptive_engine
 
         self.iteration = 0
 
         self._state = CoreState.Inactive
         self._exception_queue = Queue()
         self._forced_position_queue = Queue()
         self._forced_measurement_queue = Queue()
+        self._has_fresh_data = True
 
         self.data = Data()
         self._graphs = []
 
         self.experiment_thread = None
 
     @property
@@ -112,65 +116,93 @@
 
             if self.state not in [CoreState.Stopping, CoreState.Exiting, CoreState.Resuming, CoreState.Restarting]:
                 await self.notify_clients()
 
     def experiment_loop(self):
         while True:
             if self.state == CoreState.Running:
-                logger.info(f'Iteration: {len(self.data)}')
+                logger.info(f'Iteration: {self.data._completed_iterations}, Data count: {len(self.data)}')
                 try:
                     self.experiment_iteration()
                 except Exception as ex:
                     self._exception_queue.put(ex)
                     self.state = CoreState.Pausing
                     logger.exception(ex)
             elif self.state in [CoreState.Stopping, CoreState.Inactive, CoreState.Exiting]:
                 return
             else:
                 time.sleep(.1)
 
     def experiment_iteration(self):
         with self.data.iteration():
-            with log_time('getting position', cumulative_key='getting position'):
-                position = tuple(self.execution_engine.get_position() or [0] * self.data.dimensionality)
-            if self._forced_position_queue.empty():
-                with log_time('getting targets', cumulative_key='getting targets'):
-                    targets = self.adaptive_engine.request_targets(position)
-            else:
-                targets = [self._forced_position_queue.get()]
-            with log_time('updating targets', cumulative_key='updating targets'):
-                if self._forced_measurement_queue.empty():
-                    self.execution_engine.update_targets(targets)
-                    with log_time('getting measurements', cumulative_key='getting measurements'):
-                        new_measurements = self.execution_engine.get_measurements()
+            if self._has_fresh_data:
+                with log_time('getting position', cumulative_key='getting position'):
+                    position = self.execution_engine.get_position()
+                    if position is None:
+                        position = [0] * self.data.dimensionality
+                    position = tuple(position)
+                if self._forced_position_queue.empty():
+                    with log_time('getting targets', cumulative_key='getting targets'):
+                        targets = self.adaptive_engine.request_targets(position)
                 else:
-                    new_measurements = [self._forced_measurement_queue.get()]
+                    targets = [self._forced_position_queue.get()]
+
+            if self._forced_measurement_queue.empty():
+                if self._has_fresh_data:
+                    with log_time('updating targets', cumulative_key='updating targets'):
+                        self.execution_engine.update_targets(targets)
+                    self._has_fresh_data = False
+                with log_time('getting measurements', cumulative_key='getting measurements'):
+                    new_measurements = self.execution_engine.get_measurements()
+            else:
+                new_measurements = [self._forced_measurement_queue.get()]
             if len(new_measurements):
+                self._has_fresh_data = True
                 with log_time('stashing new measurements', cumulative_key='injecting new measurements'):
                     self.data.inject_new(new_measurements)
                 with log_time('updating engine with new measurements', cumulative_key='updating engine with new measurements'):
                     self.adaptive_engine.update_measurements(self.data)
                 with log_time('updating metrics', cumulative_key='updating metrics'):
                     self.adaptive_engine.update_metrics(self.data)
-            with log_time('training', cumulative_key='training'):
-                self.adaptive_engine.train()
+            else:
+                time.sleep(SLEEP_FOR_FRESH_DATA_TIME)
+            if self._has_fresh_data:
+                with log_time('training', cumulative_key='training'):
+                    self.adaptive_engine.train()
+            else:
+                logger.info('Current data is stale. Waiting for an update with fresh data.')
 
     async def notify_clients(self):
         ...
 
     @property
     def graphs(self):
         execution_graphs = getattr(self.execution_engine, 'graphs', []) or []
         adaptive_graphs = getattr(self.adaptive_engine, 'graphs', []) or []
         return execution_graphs + adaptive_graphs + self._graphs
 
     @graphs.setter
     def graphs(self, graphs):
         raise NotImplementedError('Updating graphs on server not supported yet.')
 
+    def update_graph(self, new_graph):
+        execution_graphs = getattr(self.execution_engine, 'graphs', []) or []
+        adaptive_graphs = getattr(self.adaptive_engine, 'graphs', []) or []
+        self_graphs = self._graphs
+
+        for graph_list in [execution_graphs, adaptive_graphs, self_graphs]:
+            for i, old_graph in enumerate(graph_list):
+                if old_graph.id == new_graph.id:
+                    graph_list[i] = new_graph
+                    return
+        else:
+            raise ValueError('Graph not found in graphs lists.')
+
+
+
 
 class ZMQCore(Core):
     def __init__(self, *args, **kwargs):
         super(ZMQCore, self).__init__(*args, **kwargs)
         # self.start_server()
         self.context = None
         self.poller = None
@@ -240,16 +272,21 @@
     def respond_ConnectRequest(self, request):
         return ConnectResponse(self.state)
 
     def respond_PullGraphsRequest(self, request):
         return GraphsResponse(self.graphs)
 
     def respond_PushGraphsRequest(self, request):
-        self.graphs = request.graphs
-        return GraphsResponse(self.graphs)
+        for graph in request.graphs:
+            try:
+                self.update_graph(graph)
+            except ValueError as ex:
+                return ExceptionResponse("Graph ID not found in server's graphs.")
+        # self.graphs = request.graphs
+        return StateResponse(self.state)
 
     def respond_ReplayRequest(self, request):
         self._forced_measurement_queue.queue.clear()
         self._forced_position_queue.queue.clear()
 
         for position in request.positions:
             self._forced_position_queue.put(position)
@@ -274,15 +311,18 @@
                     time.sleep(.1)
                     continue
 
                 logger.info(f"Received request: {request}")
                 with log_time('preparing response', cumulative_key='preparing response'):
                     responder = getattr(self, f'respond_{request.__class__.__name__}', None)
                     if responder:
-                        response = responder(request)
+                        try:
+                            response = responder(request)
+                        except Exception as ex:
+                            response = ExceptionResponse(ex)
                     else:
                         response = UnknownResponse()
 
                 logger.info(f'Sending response: {response}')
                 await socket.send_pyobj(response)
 
                 if isinstance(response, UnknownResponse):
```

### Comparing `tsuchinoko-1.0.9/tsuchinoko/core/messages.py` & `tsuchinoko-1.1.0/tsuchinoko/core/messages.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/tsuchinoko/examples/IRBL_server_demo_LC.py` & `tsuchinoko-1.1.0/tsuchinoko/examples/IRBL_server_demo_LC.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/tsuchinoko/examples/adaptive_demo.py` & `tsuchinoko-1.1.0/tsuchinoko/examples/adaptive_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/tsuchinoko/examples/grid_demo.py` & `tsuchinoko-1.1.0/tsuchinoko/examples/grid_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/tsuchinoko/examples/headless_demo.py` & `tsuchinoko-1.1.0/tsuchinoko/examples/headless_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/tsuchinoko/examples/high_dimensionality_server_demo.py` & `tsuchinoko-1.1.0/tsuchinoko/examples/high_dimensionality_server_demo.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,36 +24,32 @@
         sys.exit(1)
     subprocess.check_call([sys.executable, "-m", "pip", "install", 'perlin-noise'])
     from perlin_noise import PerlinNoise
 
 
 
 # More useful for display purposes; PerlinNoise interpolates internally and accepts float positions in range [0,1)
-noise = PerlinNoise(octaves=3)
+noise = PerlinNoise(octaves=8)
 # size = 10
 # shape = (size, size, size)
 # indices = np.transpose(np.indices(shape)/size,(3,2,1,0)).reshape((np.prod(shape), 3))
 # noise_map = map(noise, indices)
 
 
 
 
 execution = SimpleEngine(measure_func=lambda position: (position, noise(position), 1, {}))
 
 
+dimensionality = 5
 # Define a gpCAM adaptive engine with initial parameters
-adaptive = GPCAMInProcessEngine(dimensionality=3,
-                                parameter_bounds=[(0, 1),
-                                                  (0, 1),
-                                                  (0, 1)],
-                                hyperparameters=[255, 100, 100, 100],
-                                hyperparameter_bounds=[(0, 1e5),
-                                                       (0, 1e5),
-                                                       (0, 1e5),
-                                                       (0, 1e5)])
+adaptive = GPCAMInProcessEngine(dimensionality=dimensionality,
+                                parameter_bounds=[(0, 10)] * dimensionality,
+                                hyperparameters=[255] + [100] * dimensionality,
+                                hyperparameter_bounds=[(0, 1e5)] * (dimensionality+1))
 
 # Construct a core server
 core = ZMQCore()
 core.set_adaptive_engine(adaptive)
 core.set_execution_engine(execution)
 
 if __name__ == '__main__':
```

### Comparing `tsuchinoko-1.0.9/tsuchinoko/examples/ir_server_demo.py` & `tsuchinoko-1.1.0/tsuchinoko/examples/ir_server_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/tsuchinoko/examples/multi_task_server_demo.py` & `tsuchinoko-1.1.0/tsuchinoko/examples/multi_task_server_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/tsuchinoko/examples/quadtree_demo.py` & `tsuchinoko-1.1.0/tsuchinoko/examples/quadtree_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/tsuchinoko/examples/server_demo.py` & `tsuchinoko-1.1.0/tsuchinoko/examples/server_demo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from pathlib import Path
 import numpy as np
 from PIL import Image
 from scipy import ndimage
 
+from tsuchinoko import examples
 from tsuchinoko.adaptive.gpCAM_in_process import GPCAMInProcessEngine
 from tsuchinoko.core import ZMQCore
 from tsuchinoko.execution.simple import SimpleEngine
 
 # Load data from a jpg image to be used as a luminosity map
-image = np.flipud(np.asarray(Image.open(Path(__file__).parent/'sombrero_pug.jpg')))
+image = np.flipud(np.asarray(Image.open(Path(examples.__file__).parent/'sombrero_pug.jpg')))
 luminosity = np.average(image, axis=2)
 
 
 # Bilinear sampling will be used to effectively smooth pixel edges in source data
 def bilinear_sample(pos):
     return pos, ndimage.map_coordinates(luminosity, [[pos[1]], [pos[0]]], order=1)[0], 1, {}
```

### Comparing `tsuchinoko-1.0.9/tsuchinoko/examples/server_demo_bluesky.py` & `tsuchinoko-1.1.0/tsuchinoko/examples/server_demo_bluesky.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/tsuchinoko/examples/vector_metric_demo.py` & `tsuchinoko-1.1.0/tsuchinoko/examples/vector_metric_demo.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/tsuchinoko/execution/__init__.py` & `tsuchinoko-1.1.0/tsuchinoko/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/tsuchinoko/execution/bluesky_in_process.py` & `tsuchinoko-1.1.0/tsuchinoko/execution/bluesky_in_process.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/tsuchinoko/execution/simple.py` & `tsuchinoko-1.1.0/tsuchinoko/execution/simple.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/tsuchinoko/execution/threaded_in_process.py` & `tsuchinoko-1.1.0/tsuchinoko/execution/threaded_in_process.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/tsuchinoko/graphics_items/clouditem.py` & `tsuchinoko-1.1.0/tsuchinoko/graphics_items/clouditem.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/tsuchinoko/graphs/__init__.py` & `tsuchinoko-1.1.0/tsuchinoko/graphs/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from enum import Enum, auto
+from typing import ClassVar
+from uuid import uuid4
 
 from qtpy.QtWidgets import QWidget
+from qtpy.QtCore import Signal, QObject
 
 
 class Location(Enum):
     Client = auto()
     Core = auto()
     ExecutionEngine = auto()
     AdaptiveEngine = auto()
@@ -17,30 +20,41 @@
 
 
 class RenderMode(Enum):
     Blocking = auto()
     Background = auto()
 
 
+class GraphSignalRelay(QObject):
+    sigPush = Signal(object)
+
+
+graph_signal_relay = GraphSignalRelay()
+
+
 @dataclass(eq=False)
 class Graph:
-    name: str
+    name: ClassVar[str] = ''
     compute_with: Location = Location.Client
     compute_mode: ComputeMode = ComputeMode.Blocking
     render_mode: RenderMode = RenderMode.Blocking
-    widget: QWidget = None
+    widget_class: ClassVar[type[QWidget]] = None
+    widget_args: tuple = field(default_factory=tuple)
+    widget_kwargs: dict = field(default_factory=dict)
+    id: str = field(default_factory=lambda: str(uuid4()))
+
 
     def compute(self, data: 'Data', *args):
         ...
 
     def update(self, data: 'Data', *args):
         ...
 
     def make_widget(self):
-        ...
+        return self.widget_class(*self.widget_args, **self.widget_kwargs)
 
     # @property
     # def widget(self):
     #     return
     #
     # @widget.setter
     # def widget(self, value):
```

### Comparing `tsuchinoko-1.0.9/tsuchinoko/plan_stubs/__init__.py` & `tsuchinoko-1.1.0/tsuchinoko/plan_stubs/__init__.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/tsuchinoko/utils/__init__.py` & `tsuchinoko-1.1.0/tsuchinoko/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/tsuchinoko/utils/coverage.py` & `tsuchinoko-1.1.0/tsuchinoko/utils/coverage.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/tsuchinoko/utils/dependencies.py` & `tsuchinoko-1.1.0/tsuchinoko/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/tsuchinoko/utils/logging.py` & `tsuchinoko-1.1.0/tsuchinoko/utils/logging.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/tsuchinoko/utils/mutex.py` & `tsuchinoko-1.1.0/tsuchinoko/utils/mutex.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/tsuchinoko/utils/runengine.py` & `tsuchinoko-1.1.0/tsuchinoko/utils/runengine.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/tsuchinoko/utils/threads.py` & `tsuchinoko-1.1.0/tsuchinoko/utils/threads.py`

 * *Files identical despite different names*

### Comparing `tsuchinoko-1.0.9/tsuchinoko/widgets/debugmenubar.py` & `tsuchinoko-1.1.0/tsuchinoko/widgets/debugmenubar.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,55 @@
 import sys
-
-from qtpy.QtWidgets import QMenuBar, QShortcut, QMenu, QPushButton, QApplication, QWidget
-from qtpy.QtGui import QKeySequence
-from qtpy.QtCore import Qt, QObject, QEvent
+from functools import partial
 
 # Hack to work around PySide being imported from nowhere:
 import qtpy
+from loguru import logger
+from qtpy.QtCore import Qt, QObject, QEvent
+from qtpy.QtGui import QKeySequence
+from qtpy.QtWidgets import QMenuBar, QShortcut, QMenu, QWidget, QAction, QActionGroup
 
 if "PySide.QtCore" in sys.modules and qtpy.API != "pyside":
     del sys.modules["PySide.QtCore"]
 
 from qtconsole.rich_jupyter_widget import RichJupyterWidget
 from qtconsole.inprocess import QtInProcessKernelManager
 
 
 class DebuggableMenuBar(QMenuBar):
     def __init__(self, *args, **kwargs):
         super(DebuggableMenuBar, self).__init__(*args, **kwargs)
 
-        self.debugshortcut = QShortcut(QKeySequence("Ctrl+Return"), self, self.showDebugMenu, context=Qt.ApplicationShortcut)
+        self.debugshortcut = QShortcut(QKeySequence("Ctrl+Return"),
+                                       self,
+                                       self.showDebugMenu,
+                                       context=Qt.ApplicationShortcut)
 
         self._debugmenu = QMenu("Debugging")
         self._debugmenu.addAction("Debug widget", self.startDebugging)
+        self._loggingmenu = QMenu("Logging level")
+        self._debugmenu.addMenu(self._loggingmenu)
+        self._levels_group = QActionGroup(self)
+        self._levels_group.setExclusive(True)
+        for level in ['Critical', 'Error', 'Warning', 'Info', 'Debug']:
+            action = QAction(level)
+            action.triggered.connect(partial(self.set_level, level))
+            action.setCheckable(True)
+            self._levels_group.addAction(action)
+            self._loggingmenu.addAction(action)
+        self._loggingmenu.actions()[2].setChecked(True)
 
         self.mousedebugger = MouseDebugger()
 
+    def set_level(self, level: str):
+        from . import displays
+        logger.remove(displays.log_handler_id)
+        displays.log_handler_id = logger.add(displays.LogHandler(), level=level.upper())
+        logger.critical(f'Log level set to {level.upper()}')
+
     def showDebugMenu(self):
         self.addMenu(self._debugmenu)
 
     def startDebugging(self):
         QApplication.instance().installEventFilter(self.mousedebugger)
```

### Comparing `tsuchinoko-1.0.9/tsuchinoko/widgets/displays.py` & `tsuchinoko-1.1.0/tsuchinoko/widgets/displays.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,41 +6,46 @@
 from pyqtgraph.dockarea import Dock, DockArea
 from pyqtgraph.parametertree import ParameterTree, Parameter
 from pyqtgraph.parametertree.parameterTypes import GroupParameter
 from qtpy.QtWidgets import QFormLayout, QWidget, QListWidget, QListWidgetItem, QPushButton, QLabel, QSpacerItem, QSizePolicy, QStyle, QToolButton, QHBoxLayout, QVBoxLayout
 from loguru import logger
 
 from tsuchinoko.core import CoreState, ExceptionResponse
+from tsuchinoko.graphs import graph_signal_relay
 from tsuchinoko.utils import runengine
 from tsuchinoko.utils.threads import invoke_as_event, invoke_in_main_thread
 
 
+log_handler_id = None
+
+
 class Singleton(type(QObject)):
     _instances = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
             cls._instances[cls] = super(Singleton, cls).__call__(*args, **kwargs)
         return cls._instances[cls]
 
 
 class Display(Dock):
     ...
 
 
-class LogHandler(logging.Handler):
+class LogHandler(logging.Handler, metaclass=Singleton):
     colors = {logging.DEBUG: Qt.gray, logging.ERROR: Qt.darkRed, logging.CRITICAL: Qt.red,
               logging.INFO: Qt.white, logging.WARNING: Qt.yellow}
 
     def __init__(self, log_widget, level=logging.WARNING):
+        global log_handler_id
         super(LogHandler, self).__init__(level=level)
         logging.getLogger().addHandler(self)
         self.log_widget = log_widget
 
-        logger.add(logging.getLogger().handlers[-1], level=level)
+        log_handler_id = logger.add(logging.getLogger().handlers[-1], level=level)
 
     # follows same design as vanilla logger emissions
     def emit(self, record, level=logging.INFO, timestamp=None, icon=None, *args):  # We can have icons!
         item = QListWidgetItem(record.getMessage())
         item.setForeground(QBrush(self.colors[record.levelno]))
         item.setToolTip(timestamp)
         self.log_widget.insertItem(0, item)
@@ -179,46 +184,49 @@
         if self.start_pause_button.text() == 'Pause':
             self.sigPause.emit()
         elif self.start_pause_button.text() in ['Start', 'Resume']:
             self.sigStart.emit()
 
 
 class GraphManager(Display, metaclass=Singleton):
+    sigPush = Signal(object)
+
     def __init__(self):
         self.dock_area = DockArea()
 
         super(GraphManager, self).__init__('Graphs', hideTitle=True, size=(500, 500), widget=self.dock_area)
 
-        self.graphs = list()
+        self.graphs = dict()  # graph: widget
+        graph_signal_relay.sigPush.connect(self.sigPush)
 
     def set_graphs(self, graphs, data=None):
         self.clear()
         self.graphs.clear()
         for graph in graphs:
             self.register_graph(graph)
         if data:
             self.update_graphs(data, 0)
 
     def register_graph(self, graph):
-        graph.widget = graph.make_widget()
-        display = Dock(graph.name, area=self.dock_area, widget=graph.widget)
-        graph.display = display
+        widget = graph.make_widget()
+        display = Dock(graph.name, area=self.dock_area, widget=widget)
+        # graph.display = display
         self.dock_area.addDock(display, position='below')
-        self.graphs.append(graph)
+        self.graphs[graph] = widget
 
     def update_graphs(self, data, last_data_size):
-        for graph in self.graphs:
+        for graph, widget in self.graphs.items():
             try:
-                graph.update(data, slice(last_data_size, None))
+                graph.update(widget, data, slice(last_data_size, None))
             except Exception as ex:
                 logger.exception(ex)
 
     def clear(self):
         for graph in self.graphs:
             # NOTE: the parent's parent is always a Display instance containing only that graph
-            graph.widget.parent().parent().setParent(None)
-            graph.widget.parent().parent().close()
-            graph.widget.parent().parent().deleteLater()
+            self.graphs[graph].parent().parent().setParent(None)
+            self.graphs[graph].parent().parent().close()
+            self.graphs[graph].parent().parent().deleteLater()
 
     def reset(self):
         self.clear()
         self.set_graphs(self.graphs)
```

### Comparing `tsuchinoko-1.0.9/tsuchinoko/widgets/graph_widgets.py` & `tsuchinoko-1.1.0/tsuchinoko/widgets/graph_widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,18 +26,18 @@
         Qt.Key.Key_Up,
         Qt.Key.Key_Down,
         Qt.Key.Key_PageUp,
         Qt.Key.Key_PageDown,
     ]
 
     def __init__(self, data_key:str, accumulates:bool):
+        self.graph = ClickRequesterPlot()
         super().__init__()
         self.data_key = data_key
         self.accumulates = accumulates
-        graph = ClickRequesterPlot()
         # scatter = ScatterPlotItem(name='scatter', x=[0], y=[0], size=10, pen=mkPen(None), brush=mkBrush(255, 255, 255, 120))
         self.timeline = InfiniteLine(0, pen=mkPen(width=3), movable=True)
         self.timeline.sigPositionChanged.connect(self.timeline_changed)
         self.timeline_plot = PlotWidget()
         self.timeline_plot.hideAxis('left')
         self.timeline_plot.setMouseEnabled(False, False)
         self.timeline_plot.addItem(self.timeline)
@@ -47,18 +47,18 @@
         histlut.setImageItem(self.cloud)
 
         self.setLayout(QVBoxLayout())
         hlayout = QHBoxLayout()
         self.layout().addLayout(hlayout)
         self.layout().addWidget(self.timeline_plot)
 
-        hlayout.addWidget(graph)
+        hlayout.addWidget(self.graph)
         hlayout.addWidget(histlut)
 
-        graph.addItem(self.cloud)
+        self.graph.addItem(self.cloud)
 
         # Hard-coded to show max
         self.max_arrow = BetterCurveArrow(self.cloud.scatter, brush=mkBrush('r'))
         self.last_arrow = BetterCurveArrow(self.cloud.scatter, brush=mkBrush('w'))
         # text = TextItem()
 
         self.cache = dict()
@@ -260,7 +260,10 @@
         self.timeline.setBounds([0, min_length-1])
         if timeline_at_end:
             with fn.SignalBlock(self.timeline.sigPositionChanged, self.timeline_changed):
                 self.timeline.setPos(min_length-1)
 
         # text.setText(f'Max: {v[max_index]:.2f} ({x[max_index]:.2f}, {y[max_index]:.2f})')
         # text.setPos(x[max_index], y[max_index])
+
+    def getView(self):
+        return self.graph
```

### Comparing `tsuchinoko-1.0.9/tsuchinoko/widgets/mainwindow.py` & `tsuchinoko-1.1.0/tsuchinoko/widgets/mainwindow.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from signal import SIGINT
 from typing import Any, Type, Union
 import sys
 from pathlib import Path
 
 from tsuchinoko.utils.dependencies import check_dependencies
 from tsuchinoko.widgets.debugmenubar import DebuggableMenuBar
+from tsuchinoko.widgets.server_editor import ServerEditor
 
 try:
     from yaml import CLoader as Loader, CDumper as Dumper, dump, load
 except ImportError:
     from yaml import Loader, Dumper
 
 import zmq
@@ -29,15 +30,15 @@
 from tsuchinoko.assets import path
 from tsuchinoko.adaptive import Data
 from tsuchinoko.core import CoreState
 from tsuchinoko.core.messages import PauseRequest, StartRequest, GetParametersRequest, SetParameterRequest, \
     PartialDataRequest, FullDataRequest, StopRequest, Message, StateRequest, StateResponse, GetParametersResponse, \
     FullDataResponse, PartialDataResponse, MeasureRequest, \
     ConnectRequest, ConnectResponse, PushDataRequest, ExceptionResponse, PullGraphsRequest, GraphsResponse, \
-    ReplayRequest, ExitRequest
+    ReplayRequest, ExitRequest, PushGraphsRequest
 from tsuchinoko.graphics_items.clouditem import CloudItem
 from tsuchinoko.graphics_items.indicatoritem import BetterCurveArrow
 from tsuchinoko.graphics_items.mixins import ClickRequester, request_relay, ClickRequesterPlot
 from tsuchinoko.utils.threads import QThreadFutureIterator, invoke_as_event
 from tsuchinoko.widgets.displays import Log, Configuration, GraphManager, StateManager
 
 
@@ -52,18 +53,20 @@
         menubar = DebuggableMenuBar()
         file_menu = menubar.addMenu("&File")
         file_menu.addAction('&New...', self.new_data)
         open_data_action = QAction(self.style().standardIcon(QStyle.SP_DirOpenIcon), 'Open data...', parent=file_menu)
         open_parameters_action = QAction(self.style().standardIcon(QStyle.SP_DirOpenIcon), 'Open parameters...', parent=file_menu)
         save_data_action = QAction(self.style().standardIcon(QStyle.SP_DialogSaveButton), 'Save data as...', parent=file_menu)
         save_parameters_action = QAction(self.style().standardIcon(QStyle.SP_DialogSaveButton), 'Save parameters as...', parent=file_menu)
+        open_server_editor = QAction(self.style().standardIcon(QStyle.SP_DirOpenIcon), 'Open Server Editor', parent=file_menu)
         file_menu.addAction(open_data_action)
         file_menu.addAction(open_parameters_action)
         file_menu.addAction(save_data_action)
         file_menu.addAction(save_parameters_action)
+        file_menu.addAction(open_server_editor)
         file_menu.addAction('E&xit', self.close)
         self.setMenuBar(menubar)
 
         demo_menu = menubar.addMenu("&Demo")
         demo_menu.addAction('Start &Simple Demo', partial(self.start_demo, 'server_demo'))
         demo_menu.addAction('Start &Adaptive Demo', partial(self.start_demo, 'adaptive_demo')).setEnabled(check_dependencies(['adaptive']))
         demo_menu.addAction('Start &Grid Scan Demo', partial(self.start_demo, 'grid_demo'))
@@ -72,14 +75,15 @@
         demo_menu.addAction('Start &Quad Tree Demo',  partial(self.start_demo, 'quadtree_demo'))
         demo_menu.addAction('Start &Bluesky Demo',  partial(self.start_demo, 'server_demo_bluesky'))
 
         save_data_action.triggered.connect(self.save_data)
         open_data_action.triggered.connect(self.open_data)
         save_parameters_action.triggered.connect(self.save_parameters)
         open_parameters_action.triggered.connect(self.open_parameters)
+        open_server_editor.triggered.connect(self.open_server_editor)
 
         self.setWindowTitle('Tsuchinoko')
         self.setWindowIcon(QIcon(path('tsuchinoko.png')))
         self.resize(1700, 1000)
 
         self.log_widget = Log()
         self.configuration_widget = Configuration()
@@ -105,14 +109,15 @@
 
         self.state_manager_widget.sigPause.connect(self.pause)
         self.state_manager_widget.sigStart.connect(self.start)
         self.state_manager_widget.sigStop.connect(self.stop)
         self.state_manager_widget.sigReplay.connect(self.replay)
         self.configuration_widget.sigPushParameter.connect(self.set_parameter)
         self.configuration_widget.sigRequestParameters.connect(self.request_parameters)
+        self.graph_manager_widget.sigPush.connect(self.push_graph)
         request_relay.sigRequestMeasure.connect(self.request_measure)
 
         self.update_thread = QThreadFutureIterator(self.update, finished_slot=self.close_zmq, name='tsuchinoko-update')
         self.update_thread.start()
 
         self.data: Data = Data()
         self.last_data_size = None
@@ -165,14 +170,17 @@
 
     def request_measure(self, pos):
         self.message_queue.put(MeasureRequest(pos))
 
     def request_parameters(self):
         self.message_queue.put(GetParametersRequest())
 
+    def push_graph(self, graph):
+        self.message_queue.put(PushGraphsRequest([graph]))
+
     def set_parameter(self, child_path: str, value: Any):
         if child_path:
             self.message_queue.put(SetParameterRequest(child_path, value))
 
     def update(self):
         self.data = Data()
         self.last_data_size = 0
@@ -219,14 +227,16 @@
                 self.last_data_size = 0
                 self.state_manager_widget.update_state(CoreState.Connecting)
             else:
                 logger.info(f'response: {response}')
                 if not response:
                     self.get_state()
                 else:
+                    if self.state_manager_widget.state == CoreState.Connecting:
+                        logger.critical(f'Successfully connected to server at {self.core_address}.')
                     for callback, as_event in self.callbacks[type(response)]:
                         if as_event:
                             invoke_as_event(callback, *response.payload)
                         else:
                             callback(*response.payload)
 
     def _data_callback(self, data_payload, last_data_size=None):
@@ -234,16 +244,17 @@
             return
 
         if last_data_size is not None and last_data_size < len(self.data):
             raise IndexError('Overwriting of previous data prevented.')
 
         self.data.extend(Data(**data_payload))
         if len(data_payload['positions']):
-            invoke_as_event(self.update_graphs, self.data, self.last_data_size)
-        self.last_data_size = len(self.data)
+            # stash the length of new data early to avoid events getting confused when pausing this thread
+            old_last_data_size, self.last_data_size = self.last_data_size, len(self.data)
+            invoke_as_event(self.update_graphs, self.data, old_last_data_size)
 
     def refresh_state(self, _):
         self.message_queue.queue.clear()
         self.message_queue.put(GetParametersRequest())
         self.message_queue.put(PullGraphsRequest())
 
     def update_graphs(self, data, last_data_size):
@@ -340,15 +351,15 @@
             self.socket = None
         if self.context:
             logger.debug('Closing context')
             self.context.term()
             self.context = None
 
     def closeEvent(self, event):
-        if not self.close_demo():
+        if not self.close_demo(confirm=True):
             event.ignore()
             return
         if self.data and len(self.data):
             result = QMessageBox.question(self,
                                       'Save data?',
                                       "You have unsaved data in the active experiment. Do you want to save the data?",
                                       buttons=QMessageBox.StandardButtons(QMessageBox.Yes | QMessageBox.No | QMessageBox.Cancel),
@@ -360,32 +371,46 @@
                 self.close_zmq()
             else:
                 event.ignore()
         else:
             event.accept()
             self.close_zmq()
 
-
     def start_demo(self, demo_key):
         # If not communicating with localhost, dump connection to server
         if self.core_address != 'localhost':
             self.core_address = 'localhost'
             self.init_socket()
 
         # if there's a child process server, exit it
-        if not self.close_demo():
+        if not self.close_demo(confirm=True):
             return
 
         suffix = Path(sys.executable).suffix 
         demo_exe = (Path(sys.executable).parent/'tsuchinoko_demo').with_suffix(suffix if suffix=='.exe' else '')
-        print(demo_exe)
+        # print(demo_exe)
         self._server = subprocess.Popen([demo_exe, demo_key])
 
-    def close_demo(self):
+    def start_server(self, path):
+        suffix = Path(sys.executable).suffix
+        bootstrap_exe = (Path(sys.executable).parent / 'tsuchinoko_bootstrap').with_suffix(suffix if suffix == '.exe' else '')
+        # print(bootstrap_exe)
+        self._server = subprocess.Popen([bootstrap_exe, path])
+
+    def close_demo(self, confirm=False):
         if self._server:
+            if confirm:
+                result = QMessageBox.question(self,
+                                              'Shutdown server?',
+                                              "A Tsuchinoko experiment server is currently running. Would you like to stop the server?",
+                                              buttons=QMessageBox.StandardButtons(
+                                                  QMessageBox.Yes | QMessageBox.Cancel),
+                                              defaultButton=QMessageBox.Yes)
+                if result != QMessageBox.Yes:
+                    return False
             self.message_queue.put(ExitRequest())
             try:
                 self._server.wait(3)
 
             except subprocess.TimeoutExpired:
                 result = QMessageBox.question(self,
                                               'Server not responding.',
@@ -395,7 +420,13 @@
                                               defaultButton=QMessageBox.Yes)
                 if result == QMessageBox.Yes:
                     self._server.kill()
                     return True
                 elif result == QMessageBox.Cancel:
                     return False
         return True
+
+    stop_server = close_demo
+
+    def open_server_editor(self):
+        self.editor_window = ServerEditor(main_window=self)
+        self.editor_window.show()
```

### Comparing `tsuchinoko-1.0.9/tsuchinoko.egg-info/PKG-INFO` & `tsuchinoko-1.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsuchinoko
-Version: 1.0.9
+Version: 1.1.0
 Summary: An adaptive optics alignment tool for ALS beamlines utilizing gpCAM.
 Home-page: https://github.com/lbl-camera/tsuchinoko
 Author: Ronald J Pandolfi
 Author-email: ronpandolfi@lbl.gov
 License: GPLv3+
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -35,24 +35,32 @@
 powerful Gaussian process regression at the core.
 
 A Tsuchinoko system includes 4 distinct components: the GUI client, an adaptive engine, and execution engine, and a
 core service. These components are separable to allow flexibility with a variety of distributed designs.
 
 ![Tsuchinoko running simulated measurements](docs/source/_static/running-score.PNG)
 
-## Installation
+## Standard Installation
 
-The latest stable Tsuchinoko version is available on PyPI, and is installable with `pip`.
+The latest stable Tsuchinoko version is available on PyPI, and is installable with `pip`. It is recommended that you
+use Python 3.9 for this installation.
 
 ```bash
 pip install tsuchinoko
 ```
 
 For more information, see the [installation documentation](https://tsuchinoko.readthedocs.io/en/latest/quickstart.html).
 
+## Easy Installation
+
+For Mac OSX and Windows, pre-packaged installers are available. These do not require a base Python installation. See the [installation documentation](https://tsuchinoko.readthedocs.io/en/latest/installers.html) for more details.
+
+- [Latest Windows Installer](https://github.com/lbl-camera/tsuchinoko/releases/latest/download/Tsuchinoko-amd64.exe)
+- [Latest Mac OSX Installer](https://github.com/lbl-camera/tsuchinoko/releases/latest/download/Tsuchinoko.app.tgz)
+
 ## Resources
 
 * Documentation: https://tsuchinoko.readthedocs.io/en/latest
 * Report an issue in Tsuchinoko: [New Bug Report](https://github.com/lbl-camera/tsuchinoko/issues/new?labels=bug)
 
 ## About the name
```

### Comparing `tsuchinoko-1.0.9/tsuchinoko.egg-info/SOURCES.txt` & `tsuchinoko-1.1.0/tsuchinoko.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 docs/Makefile
 docs/make.bat
 docs/source/conf.py
 tests/test_core.py
 tests/test_graphics_items.py
 tests/test_gui.py
 tsuchinoko/__init__.py
+tsuchinoko/_bootstrap.py
 tsuchinoko/_version.py
 tsuchinoko.egg-info/PKG-INFO
 tsuchinoko.egg-info/SOURCES.txt
 tsuchinoko.egg-info/dependency_links.txt
 tsuchinoko.egg-info/entry_points.txt
 tsuchinoko.egg-info/requires.txt
 tsuchinoko.egg-info/top_level.txt
@@ -35,42 +36,50 @@
 tsuchinoko/assets/__init__.py
 tsuchinoko/core/__init__.py
 tsuchinoko/core/messages.py
 tsuchinoko/examples/IRBL_server_demo_LC.py
 tsuchinoko/examples/__init__.py
 tsuchinoko/examples/_launch_demo.py
 tsuchinoko/examples/adaptive_demo.py
+tsuchinoko/examples/bluesky_adaptive_demo.py
 tsuchinoko/examples/client_demo.py
 tsuchinoko/examples/grid_demo.py
 tsuchinoko/examples/headless_demo.py
 tsuchinoko/examples/high_dimensionality_server_demo.py
 tsuchinoko/examples/ir_server_demo.py
 tsuchinoko/examples/multi_task_server_demo.py
 tsuchinoko/examples/quadtree_demo.py
 tsuchinoko/examples/server_demo.py
 tsuchinoko/examples/server_demo_bluesky.py
 tsuchinoko/examples/vector_metric_demo.py
 tsuchinoko/execution/__init__.py
+tsuchinoko/execution/bluesky_adaptive.py
 tsuchinoko/execution/bluesky_in_process.py
 tsuchinoko/execution/simple.py
 tsuchinoko/execution/threaded_in_process.py
 tsuchinoko/extensions/__init__.py
 tsuchinoko/graphics_items/__init__.py
 tsuchinoko/graphics_items/clouditem.py
 tsuchinoko/graphics_items/indicatoritem.py
 tsuchinoko/graphics_items/mixins.py
 tsuchinoko/graphs/__init__.py
 tsuchinoko/graphs/common.py
 tsuchinoko/parameters/__init__.py
+tsuchinoko/patches/__init__.py
+tsuchinoko/patches/jupyter.py
+tsuchinoko/patches/pyqode.py
+tsuchinoko/patches/pyqtgraph.py
 tsuchinoko/plan_stubs/__init__.py
 tsuchinoko/utils/__init__.py
 tsuchinoko/utils/coverage.py
 tsuchinoko/utils/dependencies.py
 tsuchinoko/utils/logging.py
 tsuchinoko/utils/mutex.py
 tsuchinoko/utils/runengine.py
 tsuchinoko/utils/threads.py
 tsuchinoko/widgets/__init__.py
 tsuchinoko/widgets/debugmenubar.py
 tsuchinoko/widgets/displays.py
 tsuchinoko/widgets/graph_widgets.py
-tsuchinoko/widgets/mainwindow.py
+tsuchinoko/widgets/mainwindow.py
+tsuchinoko/widgets/server_editor.py
+tsuchinoko/widgets/simple.py
```

### Comparing `tsuchinoko-1.0.9/versioneer.py` & `tsuchinoko-1.1.0/versioneer.py`

 * *Files identical despite different names*

