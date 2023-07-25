# Comparing `tmp/nctoolkit-0.9.4.tar.gz` & `tmp/nctoolkit-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nctoolkit-0.9.4.tar", last modified: Tue Jun 27 15:13:22 2023, max compression
+gzip compressed data, was "nctoolkit-1.0.0.tar", last modified: Tue Jul 25 13:06:56 2023, max compression
```

## Comparing `nctoolkit-0.9.4.tar` & `nctoolkit-1.0.0.tar`

### file list

```diff
@@ -1,98 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:13:22.031390 nctoolkit-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-06-27 15:13:09.000000 nctoolkit-0.9.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-27 15:13:09.000000 nctoolkit-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-27 15:13:09.000000 nctoolkit-0.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-27 15:13:22.027390 nctoolkit-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-27 15:13:09.000000 nctoolkit-0.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:13:22.019390 nctoolkit-0.9.4/cheatsheet/
--rw-r--r--   0 runner    (1001) docker     (123)   144398 2023-06-27 15:13:09.000000 nctoolkit-0.9.4/cheatsheet/nctoolkit_cheatsheet.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   383483 2023-06-27 15:13:09.000000 nctoolkit-0.9.4/cheatsheet/nctoolkit_cheatsheet.pptx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:13:22.019390 nctoolkit-0.9.4/checklists/
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-27 15:13:09.000000 nctoolkit-0.9.4/checklists/api_checker.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:13:22.019390 nctoolkit-0.9.4/data/
--rw-r--r--   0 runner    (1001) docker     (123)   802316 2023-06-27 15:13:09.000000 nctoolkit-0.9.4/data/geotiff.tif
--rw-r--r--   0 runner    (1001) docker     (123)   163943 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/data/pubplot_test.png
--rw-r--r--   0 runner    (1001) docker     (123)   488867 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/data/test1.html
--rw-r--r--   0 runner    (1001) docker     (123)    18976 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/data/test2.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:13:22.027390 nctoolkit-0.9.4/nctoolkit/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23048 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/add_etc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/anomaly.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    58984 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1902 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/append.py
--rw-r--r--   0 runner    (1001) docker     (123)    24608 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/cdo_command.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2166 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/cellareas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/centres.py
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6789 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/cleanup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/clear.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7789 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/compare.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7515 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/compare_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/corr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1393 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/create_ensemble.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5262 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/crop.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/distgrid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3667 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/ensembles.py
--rw-r--r--   0 runner    (1001) docker     (123)    11668 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/esoteric.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/fill.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       88 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)     7880 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/fldstat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      882 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/format.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2560 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/generate_grid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2183 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/inttime.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1557 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/masking.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      649 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/matchpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     9019 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/mergers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/meridonials.py
--rw-r--r--   0 runner    (1001) docker     (123)    10450 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/mp_adders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/mp_matchers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16851 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/mp_matchups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/nco_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/phenology.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3112 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/plot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      785 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/reduce.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1034 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/reduce_grid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6401 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/regrid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1952 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/remove.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2228 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/rename.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      856 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/resample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/rollstat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1290 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    45968 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/runthis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/session.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      767 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/set.py
--rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/setters.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/split.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23194 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/static_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/strip_vars.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16127 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/subset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1179 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/sumall.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/temp_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    17640 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/temporal_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/temporals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/thresholds.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4415 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/to_lonlat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5192 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/to_nc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3592 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/toxarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/tozlev.py
--rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/unify.py
--rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      578 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/validator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22712 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/validator_funs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19509 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/verticals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      480 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/nctoolkit/zonals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:13:22.027390 nctoolkit-0.9.4/nctoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-27 15:13:21.000000 nctoolkit-0.9.4/nctoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 15:13:22.031390 nctoolkit-0.9.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3245 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:13:22.027390 nctoolkit-0.9.4/testing/
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/testing/test_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-27 15:13:10.000000 nctoolkit-0.9.4/testing/test_scripting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:06:56.841851 nctoolkit-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-07-25 13:06:42.000000 nctoolkit-1.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 13:06:42.000000 nctoolkit-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-25 13:06:42.000000 nctoolkit-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-25 13:06:56.841851 nctoolkit-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-07-25 13:06:42.000000 nctoolkit-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:06:56.825849 nctoolkit-1.0.0/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)  2588969 2023-07-25 13:06:42.000000 nctoolkit-1.0.0/benchmarks/benchmark_nctoolkit_versus_xarray.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:06:56.829850 nctoolkit-1.0.0/cheatsheet/
+-rw-r--r--   0 runner    (1001) docker     (123)   141095 2023-07-25 13:06:42.000000 nctoolkit-1.0.0/cheatsheet/nctoolkit_cheatsheet.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   383483 2023-07-25 13:06:42.000000 nctoolkit-1.0.0/cheatsheet/nctoolkit_cheatsheet.pptx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:06:56.829850 nctoolkit-1.0.0/checklists/
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-25 13:06:42.000000 nctoolkit-1.0.0/checklists/api_checker.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:06:56.833850 nctoolkit-1.0.0/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   802316 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/data/geotiff.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   163943 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/data/pubplot_test.png
+-rw-r--r--   0 runner    (1001) docker     (123)   488867 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/data/test1.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18976 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/data/test2.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:06:56.841851 nctoolkit-1.0.0/nctoolkit/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22916 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/add_etc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/anomaly.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    55956 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1902 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/append.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24571 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/cdo_command.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2155 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/cellareas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/centres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6789 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/cleanup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/clear.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7748 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/compare.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7515 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/compare_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/corr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1393 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/create_ensemble.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5251 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/distgrid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3624 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11636 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/esoteric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/fill.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       88 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/fldstat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      882 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/format.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2560 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/generate_grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2056 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/inttime.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1517 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/masking.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      649 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/matchpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/mergers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/meridonials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10502 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/mp_adders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/mp_matchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16852 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/mp_matchups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/nco_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/phenology.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3112 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      744 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/reduce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      994 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/reduce_grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6462 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/regrid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1952 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/remove.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2188 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/rename.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      815 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/rollstat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1290 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45968 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/runthis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/session.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      767 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/setters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/split.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23806 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/static_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/strip_vars.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16096 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/subset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1179 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/sumall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/temp_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17629 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/temporal_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/temporals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/thresholds.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4415 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/to_lonlat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5192 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/to_nc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3592 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/toxarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/tozlev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/unify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      578 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/validator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22712 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/validator_funs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20044 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/verticals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      480 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/nctoolkit/zonals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:06:56.841851 nctoolkit-1.0.0/nctoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-25 13:06:56.000000 nctoolkit-1.0.0/nctoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 13:06:56.841851 nctoolkit-1.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3247 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:06:56.841851 nctoolkit-1.0.0/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/testing/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-25 13:06:43.000000 nctoolkit-1.0.0/testing/test_scripting.py
```

### Comparing `nctoolkit-0.9.4/CODE_OF_CONDUCT.md` & `nctoolkit-1.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/LICENSE` & `nctoolkit-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/MANIFEST.in` & `nctoolkit-1.0.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/PKG-INFO` & `nctoolkit-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: nctoolkit
-Version: 0.9.4
+Version: 1.0.0
 Summary: Fast and easy analysis of netCDF data in Python
 Home-page: https://github.com/pmlmodelling/nctoolkit
 Author: Robert Wilson
 Author-email: rwi@pml.ac.uk
 Maintainer: Robert Wilson
 Project-URL: Bug Tracker, https://github.com/pmlmodelling/nctoolkit/issues
 Project-URL: Documentation, https://nctoolkit.readthedocs.io/en/stable
 Project-URL: Source Code, https://github.com/pmlmodelling/nctoolkit
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6.1
 Provides-Extra: complete
 License-File: LICENSE
 
 
 
 **nctoolkit** is a comprehensive Python (3.6 and above) package for analyzing netCDF data on Linux and macOS.
```

### Comparing `nctoolkit-0.9.4/README.md` & `nctoolkit-1.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -77,16 +77,24 @@
 
 ## Reference and tutorials
 
 A full API reference, in depth tutorials and a how-to guide are available at [readthedocs](https://nctoolkit.readthedocs.io/en/latest/).
 
 
 
+## Contributing
 
+If you are interesting in contributing to nctoolkit feel free to read the [Contributing page](https://nctoolkit.readthedocs.io/en/latest/contributing.html).
 
+## Got questions about nctoolkit? 
+
+- If you have a question about how to use nctoolkit, please ask on 
+    [GitHub Discussions](https://github.com/pmlmodelling/nctoolkit/discussions).
+- Report any bugs, suggest new features or view the source code [on
+    GitHub](https://github.com/pmlmodelling/nctoolkit).
```

### Comparing `nctoolkit-0.9.4/cheatsheet/nctoolkit_cheatsheet.pdf` & `nctoolkit-1.0.0/cheatsheet/nctoolkit_cheatsheet.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 8% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,10 +1,10 @@
 Exporting datasets
 
-nctoolkit v0.9.3
+nctoolkit v0.9.4
 Cheat Sheet
 
 Creating datasets
 ds = nc.open_data(foo.nc)
 Open a local file as a dataset.
 ds = nc.open_url(‘https://foo.foo.nc’)
 Open/download a file as a dataset.
@@ -94,15 +94,15 @@
 ds.tmax()
 Calculate the temporal maximum.
 ds.tmedian()
 Calculate the temporal median.
 ds.trange()
 Calculate the temporal range.
 ds.tpercentile(95)
-Calculate the 95th percentile.
+Calculate the 95 th percentile.
 ds.tvariance()
 Calculate the temporal variance.
 ds.shift(hours = -1)
 Shift time back 1 hour. Other valid arguments:‘d
 ays’, ‘months’, ‘years’.
 ds.tcumsum()
 Temporal cumulative sum.
```

### Comparing `nctoolkit-0.9.4/cheatsheet/nctoolkit_cheatsheet.pptx` & `nctoolkit-1.0.0/cheatsheet/nctoolkit_cheatsheet.pptx`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/checklists/api_checker.ipynb` & `nctoolkit-1.0.0/checklists/api_checker.ipynb`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/data/geotiff.tif` & `nctoolkit-1.0.0/data/geotiff.tif`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/data/pubplot_test.png` & `nctoolkit-1.0.0/data/pubplot_test.png`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/data/test1.html` & `nctoolkit-1.0.0/data/test1.html`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/data/test2.html` & `nctoolkit-1.0.0/data/test2.html`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/__init__.py` & `nctoolkit-1.0.0/nctoolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/add_etc.py` & `nctoolkit-1.0.0/nctoolkit/add_etc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import copy
 import os
 import warnings
 import pandas as pd
 
 
 from nctoolkit.cleanup import cleanup
-from nctoolkit.runthis import run_this, run_cdo, tidy_command
+from nctoolkit.runthis import run_cdo, tidy_command
 from nctoolkit.session import session_info, append_safe, remove_safe
 from nctoolkit.show import nc_variables, nc_times
 from nctoolkit.temp_file import temp_file
 from nctoolkit.utils import version_above
 from nctoolkit.api import open_data
 import nctoolkit.api as api
 
@@ -35,15 +35,15 @@
         x = x.current
         if len(x) > 1:
             raise ValueError("requires single file")
         else:
             x = x[0]
 
     # create the system command and run it
-    cdo_command = f"cdo -yday{stat} {self[0]} {x}"
+    cdo_command = f"cdo yday{stat} {self[0]} {x}"
     target = temp_file(".nc")
 
     the_command = cdo_command + " " + target
 
     the_command = tidy_command(the_command)
 
     target = run_cdo(the_command, target, precision=self._precision)
@@ -63,17 +63,17 @@
     This is used by add etc.
     """
 
     if len(self) == 0:
         raise ValueError("This does not work on empty datasets!")
 
     # create the system command and run it
-    cdo_command = f"cdo -{stat},{x}"
+    cdo_command = f"cdo {stat},{x}"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command)
 
 
 def operation(self, method="mul", ff=None, var=None):
     """
     Method to add, subtract etc. a netCDF file from another one
     This is used by add etc.
     """
@@ -674,15 +674,15 @@
     If you wanted to get the absolute value of each variable, you just need do this:
 
     >>> ds.abs()
 
     """
     cdo_command = f"cdo -abs"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
 def power(self, x=None):
     """
     Powers of variables in dataset
 
     Parameters
@@ -700,15 +700,15 @@
     """
 
     if not isinstance(x, (int, float)):
         raise TypeError("x is not a float or int")
 
     cdo_command = f"cdo -pow,{x}"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command)
 
 
 __pow__ = power
 
 
 def exp(self):
     """
@@ -720,15 +720,15 @@
     If you wanted to calculate the exponential of a variable, you just need to do this:
 
     >>> ds.exp(0.5)
 
     """
     cdo_command = f"cdo -exp"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command)
 
 
 def log(self):
     """
     Method to get the natural log of variables
 
     Examples
@@ -737,15 +737,15 @@
     If you wanted to calculate the natural log of each variable, you just need to do this:
 
     >>> ds.log()
 
     """
     cdo_command = f"cdo -ln"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command)
 
 
 def log10(self):
     """
     Method to get the base 10 log of variables
 
     Examples
@@ -754,15 +754,15 @@
     If you wanted to calculate the base 10 log of each variable, you just need to do this:
 
     >>> ds.log10()
 
     """
     cdo_command = f"cdo -log10"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command)
 
 
 def square(self):
     """
     Method to get the square of variables
 
     Examples
@@ -771,15 +771,15 @@
     If you wanted to calculate the square of each variable, you just need to do this:
 
     >>> ds.power()
 
     """
     cdo_command = f"cdo -sqr"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command)
 
 
 def sqrt(self):
     """
     Method to get the square root of variables
 
     Examples
@@ -788,8 +788,8 @@
     If you wanted to calculate the square root of each variable, you just need to do this:
 
     >>> ds.sqrt()
 
     """
     cdo_command = f"cdo -sqrt"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command)
```

### Comparing `nctoolkit-0.9.4/nctoolkit/anomaly.py` & `nctoolkit-1.0.0/nctoolkit/anomaly.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/api.py` & `nctoolkit-1.0.0/nctoolkit/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -115,14 +115,28 @@
 session_info["lazy"] = True
 session_info["precision"] = None
 session_info["parallel"] = False
 session_info["progress"] = "on"
 session_info["checks"] = True
 session_info["user"] = ""
 
+# get the cdo methods
+
+read = subprocess.run(
+    "cdo --operators", shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE
+).stdout
+
+cdo_methods = [x.split(" ")[0].replace("b'", "") for x in str(read).split("\\n")]
+
+cdo_methods = [mm for mm in cdo_methods if len(mm) > 0]
+
+cdo_methods.append("L")
+cdo_methods.append("reduce_dim")
+session_info["cdo_methods"] = cdo_methods
+
 
 def coast_check():
     try:
         import geoviews
         import cartopy
         from cartopy import crs
         import cartopy.crs as ccrs
@@ -327,109 +341,28 @@
         "checks",
         "progress",
     ]
 
     update_options(kwargs)
     return None
 
-    for key in kwargs:
-        if key not in valid_keys:
-            raise AttributeError(key + " is not a valid option")
-
-        if key == "parallel" or key == "lazy" or key == "thread_safe":
-            if isinstance(kwargs[key], bool):
-                raise TypeError(f"{key} should be boolean")
-
-        if key == "checks":
-            if isinstance(kwargs[key], bool):
-                raise TypeError(f"{key} should be boolean")
-
-        if isinstance(kwargs[key], bool):
-            if key == "temp_dir":
-                if isinstance(kwargs[key], str):
-                    if os.path.exists(kwargs[key]) is False:
-                        raise ValueError("The temp_dir specified does not exist!")
-                    session_info[key] = os.path.abspath(kwargs[key])
-                    session_info["user_dir"] = True
-                return None
-            if key == "progress":
-                if kwargs[key] not in ["on", "off", "auto", "of"]:
-                    raise ValueError("progress must be one of 'on', 'off', 'auto'")
-
-                if kwargs[key] == "of":
-                    session_info[key] = "off"
-                else:
-                    session_info[key] = kwargs[key]
-                return None
-
-            if key == "cores":
-                if isinstance(kwargs[key], int):
-                    if kwargs[key] > mp.cpu_count():
-                        raise ValueError(
-                            str(kwargs[key])
-                            + " is greater than the number of system cores ("
-                            + str(mp.cpu_count())
-                            + ")"
-                        )
-                    session_info[key] = kwargs[key]
-                else:
-                    raise TypeError("cores must be an int")
-            else:
-                if key == "precision":
-                    if kwargs[key] not in ["I8", "I16", "I32", "F32", "F64"]:
-                        raise ValueError("precision supplied is not valid!")
-                    session_info[key] = kwargs[key]
-                else:
-                    raise ValueError(kwargs[key] + " is not valid session info!")
-        else:
-            session_info[key] = kwargs[key]
-
-            # update safe-lists etc. if running in parallel
-            if kwargs[key] and key == "parallel":
-                if len(temp_dirs) > 0:
-                    for ff in temp_dirs:
-                        append_tempdirs(ff)
-
-                if len(nc_safe) > 0:
-                    for ff in nc_safe:
-                        nc_safe_par.append(ff)
-
-                if len(nc_protected) > 0:
-                    for ff in nc_protected:
-                        nc_protected_par.append(ff)
-                        nc_protected.remove(ff)
-
-            if (kwargs[key] is False) and key == "parallel":
-                if len(temp_dirs_par) > 0:
-                    for ff in temp_dirs_par:
-                        append_tempdirs(ff)
-
-                if len(nc_safe_par) > 0:
-                    for ff in nc_safe_par:
-                        nc_safe.append(ff)
-                        nc_safe_par.remove(ff)
-
-                if len(nc_protected_par) > 0:
-                    for ff in nc_protected_par:
-                        nc_protected.append(ff)
-                        nc_protected_par.remove(ff)
 
 
 # if nctoolkitrc exists, we need to read the possible options from there...
 
 
 def find_config():
     # first look in the working directory
     for ff in [".nctoolkitrc", "nctoolkitrc"]:
         if os.path.exists(ff):
             return ff
 
     # now look in the home directory....
     from os.path import expanduser
-
+ 
     home = expanduser("~")
     for ff in [".nctoolkitrc", "nctoolkitrc"]:
         if os.path.exists(home + "/" + ff):
             return home + "/" + ff
 
     return None
 
@@ -1194,45 +1127,38 @@
 
     def __iter__(self):
         for ff in self.current:
             yield ff
         return
 
     def __repr__(self):
+        self.run()
         if len(self) == 0:
             return "Empty dataset"
         current = str(len(self))
 
         output = "<nctoolkit.DataSet>:\nNumber of files: " + current
         output = output + "\n" + "File contents:"
         # repr_params = fmt.get_dataframe_repr_params()
         output += "\n"
         output += self.show_contents(min(12, len(self))).to_string()
         output += "\n"
         if len(self) > 12:
             output += "......"
         return output
 
-        # return(self.show_contents(min(12, len(self))))
-        #''    print(".......")
-
-        # return (
-        #    "<nctoolkit.DataSet>:\nFiles: "
-        #    + current
-        #    + "\n"
-        #    + "Variables: "
-        #    + str_flatten(variables)
-        # )
 
     @property
     def size(self):
+
         """The size of an object
         This will print the number of files, total size, and smallest and largest files
         in an DataSet object.
         """
+        self.run()
         all_sizes = []
 
         smallest_file = ""
         largest_file = ""
         min_size = 1e15
         max_size = -1
 
@@ -1261,15 +1187,15 @@
 
     @property
     def calendar(self):
         """
         List calendars of dataset files
         """
 
-        # return None
+        self.run()
 
         cals = []
         for ff in self:
             ds = Dataset(ff)
             for x in [x for x in ds.variables.keys() if "time" in x]:
                 y = ds.variables[x]
                 try:
@@ -1291,14 +1217,16 @@
 
     @property
     def variables(self):
         """
         List variables contained in a dataset
         """
 
+        self.run()
+
         all_variables = []
         for ff in self:
             all_variables += nc_variables(ff)
 
         all_variables = list(set(all_variables))
 
         all_variables.sort()
@@ -1307,14 +1235,16 @@
 
     @property
     def months(self):
         """
         List months contained in a dataset
         """
 
+        self.run()
+
         all_months = []
         for ff in self:
             all_months += nc_months(ff)
 
         all_months = list(set(all_months))
 
         all_months.sort()
@@ -1323,14 +1253,16 @@
 
     @property
     def levels(self):
         """
         List levels contained in a dataset
         """
 
+        self.run()
+
         all_levels = []
         for ff in self:
             all_levels += nc_levels(ff)
 
         all_levels = list(set(all_levels))
 
         all_levels.sort()
@@ -1339,14 +1271,16 @@
 
     @property
     def times(self):
         """
         List times contained in a dataset
         """
 
+        self.run()
+
         all_times = []
         for ff in self:
             all_times += nc_times(ff)
 
         all_times = list(set(all_times))
 
         all_times.sort()
@@ -1355,14 +1289,16 @@
 
     @property
     def ncformat(self):
         """
         List formats of files contained in a dataset
         """
 
+        self.run()
+
         all_formats = []
         for ff in self:
             all_formats += nc_format(ff)
 
         all_formats = list(set(all_formats))
 
         all_formats.sort()
@@ -1371,14 +1307,16 @@
 
     @property
     def years(self):
         """
         List years contained in a dataset
         """
 
+        self.run()
+
         all_years = []
         for ff in self:
             all_years += nc_years(ff)
 
         all_years = list(set(all_years))
 
         all_years.sort()
@@ -1606,14 +1544,16 @@
     @property
     def contents(self):
         """
         Detailed list of variables contained in a dataset.
         This will only display the variables in the first file of an ensemble.
         """
 
+        self.run()
+
         return self.show_contents()
 
     @property
     def start(self):
         """
         The starting file or files of the DataSet object
         """
```

### Comparing `nctoolkit-0.9.4/nctoolkit/append.py` & `nctoolkit-1.0.0/nctoolkit/append.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/assign.py` & `nctoolkit-1.0.0/nctoolkit/assign.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import re
 import dill
 import inspect
 import numpy as np
 
-from nctoolkit.runthis import run_this
 from nctoolkit.session import session_info
 from nctoolkit.utils import version_below
 
 
 def split_equation(mystr):
     return re.split("[-+^!=*/(&|)\[\]]", mystr)
 
@@ -753,8 +752,8 @@
 
     # create the cdo call and run it
     if drop is False:
         cdo_command = f"cdo -aexpr,'{command}'"
     else:
         cdo_command = f"cdo -expr,'{command}'"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble = False)
```

### Comparing `nctoolkit-0.9.4/nctoolkit/cellareas.py` & `nctoolkit-1.0.0/nctoolkit/cellareas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import copy
 
 from nctoolkit.cleanup import cleanup
 from nctoolkit.session import remove_safe
-from nctoolkit.runthis import run_this, tidy_command, run_cdo
+from nctoolkit.runthis import tidy_command, run_cdo
 from nctoolkit.show import nc_variables
 from nctoolkit.temp_file import temp_file
 
 
 def cell_area(self, join=True):
     """
     Calculate the area of grid cells.
@@ -69,15 +69,15 @@
 
         self._hold_history = copy.deepcopy(self.history)
 
         cleanup()
 
     else:
         cdo_command = "cdo -gridarea"
-        run_this(cdo_command, self, output="ensemble")
+        self.cdo_command(cdo_command, ensemble=False)
 
     # add units
 
     self.set_units({"cell_area": "m^2"})
 
     if join:
         self.run()
```

### Comparing `nctoolkit-0.9.4/nctoolkit/centres.py` & `nctoolkit-1.0.0/nctoolkit/centres.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/checks.py` & `nctoolkit-1.0.0/nctoolkit/checks.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/cleanup.py` & `nctoolkit-1.0.0/nctoolkit/cleanup.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/clear.py` & `nctoolkit-1.0.0/nctoolkit/clear.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/compare.py` & `nctoolkit-1.0.0/nctoolkit/compare.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from nctoolkit.runthis import run_this
-
 
 def is_integer(x):
     try:
         y = int(str(x))
         return True
     except:
         return False
@@ -175,15 +173,15 @@
         raise ValueError("No expression supplied")
 
     if not isinstance(expression, str):
         raise TypeError("Expression supplied is not str")
 
     expression = fix_expr(expression)
     cdo_command = f"cdo -{expression}"
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
 def __eq__(self, x):
     if not isinstance(x, str):
         try:
             test = float(x)
             x_new = x
```

### Comparing `nctoolkit-0.9.4/nctoolkit/compare_data.py` & `nctoolkit-1.0.0/nctoolkit/compare_data.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/corr.py` & `nctoolkit-1.0.0/nctoolkit/corr.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/create_ensemble.py` & `nctoolkit-1.0.0/nctoolkit/create_ensemble.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/crop.py` & `nctoolkit-1.0.0/nctoolkit/crop.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import copy
 import xarray as xr
 import subprocess
 import numbers
 
 from nctoolkit.cleanup import cleanup
 from nctoolkit.flatten import str_flatten
-from nctoolkit.runthis import run_this, run_nco, tidy_command
+from nctoolkit.runthis import run_nco, tidy_command
 from nctoolkit.temp_file import temp_file
 from nctoolkit.session import remove_safe
 
 
 def crop(self, lon=[-180, 180], lat=[-90, 90], nco=False, nco_vars=None):
     """
     Crop to a rectangular longitude and latitude box
@@ -84,15 +84,15 @@
 
     if nco is False:
         if (lon[0] >= -180) and (lon[1] <= 180) and (lat[0] >= -90) and (lat[1] <= 90):
             lat_box = str_flatten(lon + lat)
             cdo_command = "cdo -sellonlatbox," + lat_box
             cdo_command = tidy_command(cdo_command)
 
-            run_this(cdo_command, self, output="ensemble")
+            self.cdo_command(cdo_command, ensemble=False)
             return None
         else:
             raise ValueError("The lonlat box supplied is not valid!")
 
     new_files = []
     new_commands = []
```

### Comparing `nctoolkit-0.9.4/nctoolkit/distgrid.py` & `nctoolkit-1.0.0/nctoolkit/distgrid.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/drop.py` & `nctoolkit-1.0.0/nctoolkit/drop.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 from nctoolkit.flatten import str_flatten
-from nctoolkit.runthis import run_this
-
 
 def fix_ind(x):
     if x < 0:
         return x
     else:
         return x + 1
 
@@ -80,15 +78,15 @@
                     raise TypeError(f"{vv} is not an int")
 
             vars = [fix_ind(x) for x in vars]
             vars = str_flatten(vars, ",")
 
             # create the cdo command and run it
             cdo_command = f"cdo -delete,timestep={vars}"
-            run_this(cdo_command, self, output="ensemble")
+            self.cdo_command(cdo_command, ensemble=False)
 
         if "var" in key:
             vars = kwargs[key]
 
             if not isinstance(vars, list):
                 vars = [vars]
 
@@ -96,15 +94,15 @@
                 if not isinstance(vv, str):
                     raise TypeError(f"{vv} is not a str")
 
             vars = str_flatten(vars, ",")
 
             # create the cdo command and run it
             cdo_command = f"cdo -delete,name={vars}"
-            run_this(cdo_command, self, output="ensemble")
+            self.cdo_command(cdo_command, ensemble=False)
 
         if ("mon" in key) or ("day" in key) or ("year" in key):
             vars = kwargs[key]
 
             if isinstance(vars, range):
                 vars = list(vars)
 
@@ -122,8 +120,8 @@
                 temporal_command = temporal_command + f",day={vars}"
             if "mon" in key:
                 temporal_command = temporal_command + f",month={vars}"
             if "year" in key:
                 temporal_command = temporal_command + f",year={vars}"
 
     if len(temporal_command) > len("cdo -delete"):
-        run_this(temporal_command, self, output="ensemble")
+        self.cdo_command(temporal_command, ensemble=False)
```

### Comparing `nctoolkit-0.9.4/nctoolkit/ensembles.py` & `nctoolkit-1.0.0/nctoolkit/ensembles.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import copy
 import warnings
 
 from nctoolkit.cleanup import cleanup
 from nctoolkit.flatten import str_flatten
-from nctoolkit.runthis import run_this, run_nco
+from nctoolkit.runthis import  run_nco
 from nctoolkit.temp_file import temp_file
 from nctoolkit.session import get_safe, remove_safe
 
 
 def ensemble_percentile(self, p=None):
     """
     Calculate an ensemble percentile
@@ -38,15 +38,15 @@
 
     # Throw an error if there is only a single file in the tracker
     if len(self) == 1:
         warnings.warn(message="There is only one file in the dataset")
 
     # create the cdo command and run it
     cdo_command = f"cdo --sortname -enspctl,{p}"
-    run_this(cdo_command, self, output="one")
+    self.cdo_command(cdo_command, ensemble=True)
 
     # set the _merged attribute to True
     self._merged = True
 
 
 def ensemble_nco(self, method, ignore_time=False):
     """
@@ -99,17 +99,15 @@
     self.run()
 
     if len(self) == 1:
         warnings.warn(message="There is only one file in the dataset")
 
     cdo_command = "cdo --sortname -ensstd"
 
-    run_this(cdo_command, self)
-
-    self._merged = True
+    self.cdo_command(cdo_command, ensemble=True)
 
 
 def ensemble_var(self):
     """
     Calculate an ensemble variance
 
     The ensemble variance is calculated for each time steps; for example, if the ensemble is made up of
@@ -119,17 +117,15 @@
     self.run()
 
     if len(self) == 1:
         warnings.warn(message="There is only one file in the dataset")
 
     cdo_command = "cdo --sortname -ensvar"
 
-    run_this(cdo_command, self)
-
-    self._merged = True
+    self.cdo_command(cdo_command, ensemble=True)
 
 
 def ensemble_max(self, nco=False, ignore_time=False):
     """
     Calculate an ensemble maximum
 
     Parameters
@@ -150,17 +146,15 @@
             warnings.warn(message="There is only one file in the dataset")
 
         if ignore_time is False:
             cdo_command = "cdo --sortname -ensmax"
         else:
             cdo_command = "cdo -timmax --sortname -ensmax"
 
-        run_this(cdo_command, self)
-
-        self._merged = True
+        self.cdo_command(cdo_command, ensemble=True)
 
         return None
 
     ensemble_nco(self, "max", ignore_time=ignore_time)
 
 
 def ensemble_min(self, nco=False, ignore_time=False):
@@ -184,17 +178,15 @@
         self.run()
 
         if ignore_time is False:
             cdo_command = "cdo --sortname -ensmin"
         else:
             cdo_command = "cdo -timmin --sortname -ensmin"
 
-        run_this(cdo_command, self)
-
-        self._merged = True
+        self.cdo_command(cdo_command, ensemble=True)
 
         return None
 
     ensemble_nco(self, "min", ignore_time=ignore_time)
 
 
 def ensemble_mean(self, nco=False, ignore_time=False):
@@ -219,17 +211,15 @@
             warnings.warn(message="There is only one file in the dataset")
 
         if ignore_time is False:
             cdo_command = "cdo --sortname -ensmean"
         else:
             cdo_command = "cdo -timmean --sortname -ensmean"
 
-        run_this(cdo_command, self)
-
-        self._merged = True
+        self.cdo_command(cdo_command, ensemble=True)
 
         return None
 
     ensemble_nco(self, "mean", ignore_time=ignore_time)
 
 
 def ensemble_range(self):
@@ -241,17 +231,15 @@
     self.run()
 
     if len(self) == 1:
         warnings.warn(message="There is only one file in the dataset")
 
     cdo_command = "cdo --sortname -ensrange"
 
-    run_this(cdo_command, self)
-
-    self._merged = True
+    self.cdo_command(cdo_command, ensemble=True)
 
 
 def ensemble_sum(self):
     """
     Calculate an ensemble sum
     The sum is calculated for each time step; for example, if each file in the
     ensemble has 12 months of data the statistic will be calculated for each month.
@@ -259,10 +247,9 @@
     self.run()
 
     if len(self) == 1:
         warnings.warn(message="There is only one file in the dataset")
 
     cdo_command = "cdo --sortname -enssum"
 
-    run_this(cdo_command, self)
+    self.cdo_command(cdo_command, ensemble=True)
 
-    self._merged = True
```

### Comparing `nctoolkit-0.9.4/nctoolkit/esoteric.py` & `nctoolkit-1.0.0/nctoolkit/esoteric.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import copy
 import pandas as pd
 import numpy as np
 import xarray as xr
 
 from .temp_file import temp_file
 from .cleanup import cleanup
-from .runthis import run_this
 from .runthis import run_nco
 from .api import open_data
 import warnings
 
 def fix_amm7_grid(self):
     """
     A quick hack to change the grid file in AMM7 North West European shelf Nemo grids.
@@ -150,15 +149,15 @@
     Remove leap years.
     This uses an undocumented CDO feature to remove Feb 29 and sets the calendar to leap year free
 
     """
 
     cdo_command = f"cdo -del29feb"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
 def set_gridtype(self, grid):
     """
     Set the grid type. Only use this if, for example, the grid is "generic" when it should be lonlat.
 
     Parameters
@@ -179,15 +178,15 @@
         "regularnn",
         "lonlat",
     ]:
         raise ValueError("Grid type supplies is not supported")
 
     cdo_command = f"cdo -setgridtype,{grid}"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
 def assign_coords(self, lon_name=None, lat_name=None, time_name=None):
     """
     Assign coordinates to variables
 
     Parameters
```

### Comparing `nctoolkit-0.9.4/nctoolkit/fldstat.py` & `nctoolkit-1.0.0/nctoolkit/fldstat.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import copy
 
 from nctoolkit.cleanup import cleanup
-from nctoolkit.runthis import run_this, run_cdo, tidy_command
+from nctoolkit.runthis import run_cdo, run_this, tidy_command
 from nctoolkit.temp_file import temp_file
 from nctoolkit.session import remove_safe
 
 
 def boxstat(self, stat="mean", x=1, y=1):
     """Method to calculate the spatial stat from a dataset"""
 
@@ -20,15 +20,15 @@
         raise ValueError("y should be positive")
 
     if len(self) == 0:
         raise ValueError("Failure due to empty dataset!")
 
     cdo_command = f"cdo -gridbox{stat},{x},{y}"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
 def box_mean(self, x=1, y=1):
     """
     Calculate the grid box mean for all variables
     This is performed for each time step.
 
@@ -116,15 +116,15 @@
     """Method to calculate the spatial stat from a dataset"""
 
     if len(self) == 0:
         raise ValueError("Failure due to empty dataset!")
 
     cdo_command = f"cdo -fld{stat}"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
 def spatial_mean(self):
     """
     Calculate the area weighted spatial mean for all variables
     This is performed for each time step.
 
@@ -255,15 +255,17 @@
         if by_area:
             self.run()
 
             cdo_command = f"cdo -fldsum -mul {self.current[0]} -gridarea "
         else:
             cdo_command = "cdo -fldsum"
 
-        run_this(cdo_command, self, output="ensemble")
+        self.cdo_command(cdo_command, ensemble=False)
+
+        # run_this(cdo_command, self, output="ensemble")
 
         return None
 
     new_files = []
     new_commands = []
     for ff in self:
         target = temp_file("nc")
@@ -312,8 +314,8 @@
     if not isinstance(p, (int, float)):
         raise ValueError(f"{str(p)} is not a valid percentile")
     if (p < 0) or (p > 100):
         raise ValueError(f"p: {str(p)} is not between 0 and 100!")
 
     cdo_command = f"cdo -fldpctl,{str(p)}"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
```

### Comparing `nctoolkit-0.9.4/nctoolkit/format.py` & `nctoolkit-1.0.0/nctoolkit/format.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/generate_grid.py` & `nctoolkit-1.0.0/nctoolkit/generate_grid.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/inttime.py` & `nctoolkit-1.0.0/nctoolkit/inttime.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-from nctoolkit.runthis import run_this
-
-# to do. Some padding needs to be added in case something like 2000/1/1 is provided.
 
 
 def time_interp(self, start=None, end=None, resolution="monthly"):
     """
     Temporally interpolate variables based on date range and time resolution
 
     Parameters
@@ -44,15 +41,15 @@
 
     if end is None:
         cdo_command = f"cdo {cdo_command}"
     else:
         end = end.replace("/", "-")
         cdo_command = f"cdo -seldate,{start},{end} {cdo_command}"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
 def timestep_interp(self, steps=None):
     """
     Temporally interpolate a dataset to given number of time steps
     between existing time steps
 
@@ -67,8 +64,8 @@
         raise TypeError(f"{steps} is not an int!")
 
     if steps < 2:
         raise ValueError(f"{steps} is not greater than 1")
 
     cdo_command = f"cdo -intntime,{steps}"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
```

### Comparing `nctoolkit-0.9.4/nctoolkit/masking.py` & `nctoolkit-1.0.0/nctoolkit/masking.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from nctoolkit.flatten import str_flatten
-from nctoolkit.runthis import run_this
 
 
 def mask_box(self, lon=[-180, 180], lat=[-90, 90]):
     """
     Mask a lon/lat box
 
     Parameters
@@ -43,10 +42,10 @@
         raise ValueError("Check lon order")
 
     # now, clip to the lonlat box we need
 
     if (lon[0] >= -180) and (lon[1] <= 180) and (lat[0] >= -90) and (lat[1] <= 90):
         lat_box = str_flatten(lon + lat)
         cdo_command = f"cdo -masklonlatbox,{lat_box}"
-        run_this(cdo_command, self, output="ensemble")
+        self.cdo_command(cdo_command, ensemble=False)
     else:
         raise ValueError("The lonlat box supplied is not valid!")
```

### Comparing `nctoolkit-0.9.4/nctoolkit/matchpoint.py` & `nctoolkit-1.0.0/nctoolkit/matchpoint.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/mergers.py` & `nctoolkit-1.0.0/nctoolkit/mergers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import pandas as pd
 import subprocess
 import warnings
 
-from nctoolkit.runthis import run_this
 from nctoolkit.session import session_info
 from nctoolkit.show import nc_variables, nc_times
 from nctoolkit.utils import version_below
 from nctoolkit.api import open_data
 
 
 def chunks(l, n):
@@ -117,24 +116,23 @@
                 raise ValueError(
                     "You are trying to merge files with different variables!"
                 )
 
         cdo_command = "cdo --sortname -mergetime"
 
         if len(self) < 400:
-            run_this(cdo_command, self, output="one")
+            self.cdo_command(cdo_command, ensemble=True)
         else:
             new_ds = open_data()
             files = chunks(self, 365)
             ii = 0
             for ff in files:
                 ii += 1
                 ds = open_data(ff, checks=False)
                 ds.merge("time", check=check)
-                # run_this(cdo_command, ds, output="one")
                 ds.run()
                 new_ds.append(ds)
 
             new_ds.merge("time", check=check)
             new_ds.run()
             self.current = new_ds.current
 
@@ -179,16 +177,14 @@
         cdo_result = subprocess.run(
             f"cdo ntime {ff}",
             shell=True,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         )
         cdo_result = cdo_result.stdout.decode("utf-8")
-        # .stdout
-        #''cdo_result = str(cdo_result).replace("b'", "").strip()
         cdo_result = str(cdo_result)
         ntime = int(cdo_result.split("\n")[0])
         all_times.append(ntime)
     if len(set(all_times)) > 1:
         warnings.warn(
             message="The files to merge do not have the same number of time steps!"
         )
@@ -210,22 +206,14 @@
             "Consider using regrid!"
         )
 
     # check the file times are compatible
     all_times = []
     for ff in self:
         cdo_result = nc_times(ff)
-        #    f"cdo showtimestamp {ff}",
-        #    shell=True,
-        #    stdout=subprocess.PIPE,
-        #    stderr=subprocess.PIPE,
-        # ).stdout
-        # cdo_result = str(cdo_result).replace("b'", "").strip()
-        # cdo_result = cdo_result.split()
-        # cdo_result = pd.Series((v for v in cdo_result))
         all_times.append(cdo_result)
 
     for i in range(1, len(all_times)):
         if (len(all_times[i]) != len(all_times[0])) and (len(all_times[i]) > 1):
             raise ValueError(
                 "You are trying to merge data sets with an incompatible number "
                 "of time steps"
@@ -245,15 +233,15 @@
             all_df.append(i_data)
 
     for i in range(1, len(all_df)):
         if all_df[0].equals(all_df[i]) is False:
             raise ValueError("Dates of data sets do not satisfy matching criteria!")
 
     cdo_command = "cdo -merge"
-    run_this(cdo_command, self, output="one")
+    self.cdo_command(cdo_command, ensemble=False)
 
     if session_info["lazy"]:
         self._merged = True
 
 
 def collect(self):
     """
@@ -264,13 +252,13 @@
 
     if len(self) == 1:
         warnings.warn(message="There is only file in the dataset. No need to merge!")
         return None
 
     cdo_command = "cdo -collgrid"
 
-    run_this(cdo_command, self, output="one")
+    self.cdo_command(cdo_command, ensemble=True)
 
     if session_info["lazy"]:
         self._merged = True
 
     self.run()
```

### Comparing `nctoolkit-0.9.4/nctoolkit/meridonials.py` & `nctoolkit-1.0.0/nctoolkit/meridonials.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from nctoolkit.runthis import run_this
 from nctoolkit.utils import is_curvilinear
 
 
 def zonstat(self, stat="mean"):
     """Method to calculate the meridonial statistic from a netCDF file"""
     for ff in self:
         if is_curvilinear(ff):
             raise TypeError(
                 f"meridonal_{stat} cannot be calculated for curvilinear grids."
             )
     cdo_command = f"cdo -mer{stat}"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
 def meridonial_mean(self):
     """
     Calculate the meridonial mean for each year/month combination in files.
     This applies to each file in an ensemble.
```

### Comparing `nctoolkit-0.9.4/nctoolkit/mp_adders.py` & `nctoolkit-1.0.0/nctoolkit/mp_adders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pandas as pd
 from nctoolkit.api import open_data, open_thredds
 from nctoolkit.matchpoint import open_matchpoint
 import nctoolkit.api as api
+import os
 
 
 def match_points(
     ds=None,
     df=None,
     variables=None,
     depths=None,
@@ -256,15 +257,16 @@
         self.depths = [y for y in x]
 
     if not isinstance(x, list):
         if len(x.variables) > 1:
             raise ValueError("Depths file should only have one variable")
 
         self.depths = x.copy()
-        self.depths.rename({x.variables[0]: "depth"})
+        if x.variables[0] != "depth":
+            self.depths.rename({x.variables[0]: "depth"})
         self.depths.run()
 
 
 def add_points(self, df=None):
     """
     Add point data
```

### Comparing `nctoolkit-0.9.4/nctoolkit/mp_matchers.py` & `nctoolkit-1.0.0/nctoolkit/mp_matchers.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/mp_matchups.py` & `nctoolkit-1.0.0/nctoolkit/mp_matchups.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,14 +222,15 @@
                 ds.subset(variables=self.variables)
             ds.regrid(points.loc[:, ["lon", "lat"]], method=regrid)
             df_merged = [ds.to_dataframe().reset_index()]
             points_merged = True
 
     n_missing = 0
 
+
     if (len(df_times)) == 0:
         raise ValueError("There are no matching times")
 
     if points_merged is False:
         df_times = df_times.sample(frac=1)
 
         print("Looping through times in ds and df to matchup")
```

### Comparing `nctoolkit-0.9.4/nctoolkit/nco_command.py` & `nctoolkit-1.0.0/nctoolkit/nco_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,38 +64,41 @@
         if cores > 1:
             for ff in self:
                 target = temp_file(".nc")
 
                 append_safe(target)
 
                 the_command = f"{command} {ff} {target}"
+                the_command = the_command.replace("  ", " ")
 
                 temp = pool.apply_async(run_nco, [the_command, target])
                 results[ff] = temp
                 new_commands.append(the_command)
 
         else:
             for ff in self:
                 target = temp_file(".nc")
                 append_safe(target)
 
                 the_command = f"{command} {ff} {target}"
+                the_command = the_command.replace("  ", " ")
 
                 target = run_nco(the_command, target=target)
 
                 new_files.append(target)
                 new_commands.append(the_command)
 
     else:
         target = temp_file(".nc")
         append_safe(target)
 
         files = str_flatten(self.current, " ")
 
         the_command = f"{command} {files} {target}"
+        the_command = the_command.replace("  ", " ")
 
         target = run_nco(the_command, target=target)
 
         new_files.append(target)
         new_commands.append(the_command)
 
     if cores == 1 or ensemble:
@@ -106,15 +109,17 @@
             for ff in new_files:
                 if len([x for x in get_safe() if x == ff]) > 1:
                     remove_safe(ff)
                     removed += 1
             if removed == 0:
                 break
 
-        self.history.append(command)
+        for cc in new_commands:
+            self.history.append(cc)
+        #self.history.append(command)
         self._hold_history = copy.deepcopy(self.history)
 
     if cores > 1:
         pool.close()
         pool.close()
         for k, v in results.items():
             target_list.append(v.get())
```

### Comparing `nctoolkit-0.9.4/nctoolkit/phenology.py` & `nctoolkit-1.0.0/nctoolkit/phenology.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/plot.py` & `nctoolkit-1.0.0/nctoolkit/plot.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/reduce.py` & `nctoolkit-1.0.0/nctoolkit/reduce.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from nctoolkit.runthis import run_this
-
 
 def reduce_dims(self):
     """
     Reduce dimensions of data
     This will remove any dimensions with only one value. For example, if only selecting
     one vertical level, the vertical dimension will be removed.
 
@@ -20,8 +18,8 @@
     """
 
     if len(self.history) == len(self._hold_history):
         cdo_command = "cdo --reduce_dim copy"
     else:
         cdo_command = "cdo --reduce_dim"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
```

### Comparing `nctoolkit-0.9.4/nctoolkit/reduce_grid.py` & `nctoolkit-1.0.0/nctoolkit/reduce_grid.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 
 from nctoolkit.api import open_data
-from nctoolkit.runthis import run_this
 import nctoolkit.api as api
 
 
 def reduce_grid(self, mask=None):
     """
     Reduce the dataset to non-zero locations in a mask
 
@@ -33,9 +32,9 @@
     # Set missing values to zero in the mask, just in case
     targeted_mask = open_data(target)
     targeted_mask.cdo_command("-setmisstoc,0")
     targeted_mask.run()
 
     cdo_command = f"cdo -reducegrid,{targeted_mask.current[0]}"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
     self.run()
```

### Comparing `nctoolkit-0.9.4/nctoolkit/regrid.py` & `nctoolkit-1.0.0/nctoolkit/regrid.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pandas as pd
 import subprocess
 import warnings
 
 from nctoolkit.api import open_data
 from nctoolkit.cleanup import cleanup
 from nctoolkit.generate_grid import generate_grid
-from nctoolkit.runthis import run_this, run_cdo
+from nctoolkit.runthis import run_cdo, run_this
 from nctoolkit.session import append_safe, remove_safe, get_safe
 from nctoolkit.temp_file import temp_file
 import nctoolkit.api as api
 
 
 def is_iterable(x):
     try:
@@ -76,15 +76,16 @@
     valid_methods = ["bil", "nn", "bic", "dis", "con", "con2", "laf"]
 
     if isinstance(grid, api.DataSet):
         if grid._weights is not None and grid._grid is not None:
             target_grid = grid._grid
             weights_nc = grid._weights
             cdo_command = f"cdo -remap,{target_grid},{weights_nc}"
-            run_this(cdo_command, self, output="ensemble")
+            self.cdo_command(cdo_command, ensemble=False)
+            # run_this(cdo_command, self, output="ensemble")
 
             return None
 
     del_grid = None
     if grid is None:
         raise ValueError("No grid was supplied")
 
@@ -189,14 +190,15 @@
             self._weights = weights_nc
             self._grid = target_grid
 
         cdo_command = f"cdo -remap,{target_grid},{weights_nc}"
 
         tracker._execute = True
 
+
         run_this(cdo_command, tracker, output="ensemble", suppress=suppress)
 
         if recycle is False:
             remove_safe(weights_nc)
 
         for ff in tracker:
             append_safe(ff)
```

### Comparing `nctoolkit-0.9.4/nctoolkit/remove.py` & `nctoolkit-1.0.0/nctoolkit/remove.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/rename.py` & `nctoolkit-1.0.0/nctoolkit/rename.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from nctoolkit.runthis import run_this
 from nctoolkit.show import nc_variables
 from nctoolkit.utils import name_check
 import warnings
 
 
 # A custom format for warnings.
 def custom_formatwarning(msg, *args, **kwargs):
@@ -68,8 +67,8 @@
         if not isinstance(value, str):
             raise TypeError(f"{value} is not a str")
         cdo_rename += "," + key
         cdo_rename += "," + value
 
     # create the cdo call and run it
     cdo_command = "cdo -chname" + cdo_rename
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
```

### Comparing `nctoolkit-0.9.4/nctoolkit/resample.py` & `nctoolkit-1.0.0/nctoolkit/resample.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from nctoolkit.runthis import run_this
-
 
 def resample_grid(self, factor=None):
     """
     Resample the horizontal grid of a dataset
 
     Parameters
     -------------
@@ -23,8 +21,8 @@
     if not isinstance(factor, int):
         raise TypeError(f"{factor} is not an integer")
 
     if factor < 1:
         raise ValueError(f"{factor} is not a postive integer greater than 1")
 
     cdo_command = f"cdo -samplegrid,{factor}"
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
```

### Comparing `nctoolkit-0.9.4/nctoolkit/rollstat.py` & `nctoolkit-1.0.0/nctoolkit/rollstat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from nctoolkit.runthis import run_this
-
 
 def align(self, align="right"):
     """
     Method to align output time in temporal methods.
 
     Parameters
     -------------
@@ -59,15 +57,15 @@
         raise TypeError("The window supplied is not numeric!")
 
     if window < 1:
         raise ValueError(f"{window} is not a valid window!")
 
     # create the cdo call and run it
     cdo_command = f"cdo -run{stat},{str(window)}"
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
 def rolling_mean(self, window=None, align="right"):
     """
     Calculate a rolling mean based on a window
 
     Parameters
```

### Comparing `nctoolkit-0.9.4/nctoolkit/run.py` & `nctoolkit-1.0.0/nctoolkit/run.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/runthis.py` & `nctoolkit-1.0.0/nctoolkit/runthis.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/session.py` & `nctoolkit-1.0.0/nctoolkit/session.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/set.py` & `nctoolkit-1.0.0/nctoolkit/set.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/setters.py` & `nctoolkit-1.0.0/nctoolkit/setters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import copy
 import warnings
 
 from nctoolkit.cleanup import cleanup
-from nctoolkit.runthis import run_this, run_nco
 from nctoolkit.temp_file import temp_file
 from nctoolkit.session import remove_safe
 from nctoolkit.show import nc_variables
 from nctoolkit.utils import name_check
 
 
 def set_year(self, x):
@@ -18,15 +17,15 @@
     x : int
         Year to set dataset to
     """
 
     if not isinstance(x, int):
         raise ValueError(f"{x} is not a int")
     cdo_command = f"cdo -setyear,{x}"
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
 def set_day(self, x):
     """
     Set the day for each time step in a dataset
 
     Parameters
@@ -34,15 +33,15 @@
     x : int
         Day to set dataset to
     """
 
     if not isinstance(x, int):
         raise ValueError(f"{x} is not a int")
     cdo_command = f"cdo -setday,{x}"
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
 def set_precision(self, x):
     """
     Set the precision in a dataset
 
     Parameters
@@ -112,15 +111,15 @@
         raise TypeError("day supplied is not an int")
 
     cdo_command = (
         f"cdo -setreftime,{str(base_year)}-01-01 "
         f"-setdate,{str(year)}-{str(month)}-{str(day)}"
     )
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
 def missing_as(self, value=None):
     """
     Convert missing values to a constant
 
     Parameters
@@ -132,15 +131,15 @@
     try:
         test = float(value)
     except:
         raise TypeError("value must be coercible to float")
 
     cdo_command = f"cdo -setmisstoc,{value}"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
 def set_fill(self, value=None):
     """
     Set the fill value
 
     Parameters
@@ -157,15 +156,15 @@
     try:
         test = float(value)
     except:
         raise TypeError("value cannot evaluate to a float")
 
     cdo_command = f"cdo -setmissval,{value} -setmissval,nan"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
 def as_missing(self, value=None):
     """
     Change a range or individual value to missing.
 
     Parameters
@@ -188,15 +187,15 @@
     for vv in value:
         if not isinstance(vv, (int, float)):
             raise TypeError(f"{vv} is not an int or float")
 
     if isinstance(value, list):
         cdo_command = f"cdo -setrtomiss,{str(value[0])},{str(value[1])}"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
 def set_units(self, unit_dict=None, **kwargs):
     """
     Set the units for variables
 
     Parameters
@@ -239,15 +238,15 @@
     for i in unit_dict:
         if not isinstance(i, str):
             raise TypeError("key,values in unit_dict are not strings")
         if not isinstance(unit_dict[i], str):
             raise TypeError("key,values in unit_dict are not strings")
 
         cdo_command = f'cdo -setattribute,{i}@units="{unit_dict[i]}"'
-        run_this(cdo_command, self, output="ensemble")
+        self.cdo_command(cdo_command, ensemble=False)
 
 
 def set_longnames(self, name_dict=None, **kwargs):
     """
     Set the long names of variables
 
     Parameters
@@ -272,19 +271,14 @@
         raise TypeError("Please supply a dictionary")
 
     self.run()
 
     if not isinstance(name_dict, dict):
         TypeError("A dictionary has not been supplied!")
 
-    # change the longnames in turn. This doesn't seem to be something you can chain?
-
-    new_commands = []
-    new_files = []
-
     if len(self.history) == len(self._hold_history):
         variables = nc_variables(self[0])
         for key in name_dict:
             if key not in variables:
                 if len(self) > 1:
                     warnings.warn(
                         message=f"{key} is not in the first file of the dataset"
@@ -292,38 +286,18 @@
                 else:
                     warnings.warn(message=f"{key} is not in the dataset")
 
     for key, value in name_dict.items():
         if name_check(key) is False:
             raise ValueError(f"{key} is not a valid netCDF variable name")
 
-    for ff in self:
-        nco_command = "ncatted "
-        for i in name_dict:
-            if not isinstance(i, str):
-                raise TypeError("key,values in name_dict are not strings")
-            if not isinstance(name_dict[i], str):
-                raise TypeError("key,values in name_dict are not strings")
-            i_dict = name_dict[i]
-            i_dict = i_dict.replace('"', "'")
-            nco_command += "-a long_name," + i + ',o,c,"' + i_dict + '" '
-
-        target = temp_file("nc")
-
-        nco_command += ff + " " + target
-
-        target = run_nco(nco_command, target)
-
-        new_files.append(target)
-        new_commands.append(nco_command)
-
-    self.history += new_commands
-    self._hold_history = copy.deepcopy(self.history)
-
-    self.current = new_files
-
-    for ff in new_files:
-        remove_safe(ff)
+    nco_command = "ncatted "
+    for i in name_dict:
+        if not isinstance(i, str):
+            raise TypeError("key,values in name_dict are not strings")
+        if not isinstance(name_dict[i], str):
+            raise TypeError("key,values in name_dict are not strings")
+        i_dict = name_dict[i]
+        i_dict = i_dict.replace('"', "'")
+        nco_command += "-a long_name," + i + ',o,c,"' + i_dict + '" '
 
-    # clean up the directory
-    cleanup()
-    self.disk_clean()
+    self.nco_command(nco_command)
```

### Comparing `nctoolkit-0.9.4/nctoolkit/shape.py` & `nctoolkit-1.0.0/nctoolkit/shape.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/shift.py` & `nctoolkit-1.0.0/nctoolkit/shift.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from nctoolkit.runthis import run_this
-
 
 def shift_hours(self, shift=None):
     """
     Shift times in dataset by a number of hours
 
     Parameters
     -------------
@@ -18,15 +16,15 @@
         shift = int(shift)
 
     if not isinstance(shift, int):
         raise TypeError("Please supply an int for shift")
 
     cdo_command = f"cdo -shifttime,{shift}hour"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
 def shift_days(self, shift=None):
     """
     Shift times in dataset by a number of days
 
     Parameters
@@ -42,15 +40,15 @@
         shift = int(shift)
 
     if not isinstance(shift, int):
         raise TypeError("Please supply an int for shift")
 
     cdo_command = f"cdo -shifttime,{shift}days"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
 def shift_months(self, shift=None):
     """
     Shift times in dataset by a number of months
 
     Parameters
@@ -66,15 +64,15 @@
         shift = int(shift)
 
     if not isinstance(shift, int):
         raise TypeError("Please supply an int for shift")
 
     cdo_command = f"cdo -shifttime,{shift}months"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
 def shift_years(self, shift=None):
     """
     Shift times in dataset by a number of years
 
     Parameters
@@ -90,15 +88,15 @@
         shift = int(shift)
 
     if not isinstance(shift, int):
         raise TypeError("Please supply an int for shift")
 
     cdo_command = f"cdo -shifttime,{shift}years"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
 def shift(self, **kwargs):
     """
     Shift method. A wrapper for shift_days, shift_hours
     Operations are applied in the order supplied.
```

### Comparing `nctoolkit-0.9.4/nctoolkit/show.py` & `nctoolkit-1.0.0/nctoolkit/show.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/split.py` & `nctoolkit-1.0.0/nctoolkit/split.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/static_plot.py` & `nctoolkit-1.0.0/nctoolkit/static_plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,20 +25,35 @@
     from cartopy.mpl.geoaxes import GeoAxes
 except:
     session_info["static_plot"] = False
 
 from textwrap import wrap
 
 
+def find_closest_grid(z):
+    x = np.ceil(np.sqrt(z))
+    y = x
+
+    if (x * y) - z == 0.0:
+        return x, y
+    while True:
+        x = x - 1
+        if (x * y) - z < 0.0:
+            x = x + 1
+            break
+    return int(y), int(x)
+
+
 from difflib import SequenceMatcher
 
 
 def similar(a, b):
     return SequenceMatcher(None, a, b).ratio()
 
+
 from math import radians, sin, cos, asin, sqrt
 
 
 def haversine(lon1, lat1, lon2, lat2):
     lon1, lat1, lon2, lat2 = map(radians, [lon1, lat1, lon2, lat2])
     dlon = lon2 - lon1
     dlat = lat2 - lat1
@@ -95,16 +110,16 @@
     mid_point=None,
     coast="auto",
     scale="auto",
     grid=True,
     grid_colour="auto",
     legend_position="auto",
     robust=False,
-    out = None,
-    breaks = None,
+    out=None,
+    breaks=None,
     **kwargs,
 ):
     """
     Static plotting. This requires datasets to have regular latlon grids.
     Plots a static map, and requires only one variable, time step and vertical level
 
     Parameters
@@ -149,15 +164,15 @@
 
     -------------
     """
 
     axis = None
 
     if legend_position not in ["auto", "right", "bottom"]:
-        if legend_position is not None: 
+        if legend_position is not None:
             raise ValueError("legend_position must be one of right/bottom or None")
 
     land_auto = land == "auto"
 
     if land is not None:
         if not isinstance(land, str):
             raise TypeError("land must be str")
@@ -196,33 +211,31 @@
     n_cols = 1
 
     if "fig" not in kwargs.keys():
         fig = None
     if "gs" not in kwargs.keys():
         gs = None
 
-
     if "quiver" in kwargs:
         quiver = True
         u = kwargs["u"]
         v = kwargs["v"]
         kwargs.pop("quiver")
         kwargs.pop("u")
         kwargs.pop("v")
     else:
         quiver = False
 
-
     for kk in kwargs:
         fixed = False
 
         if kk == "fig":
             fig = kwargs[kk]
             fixed = True
-        
+
         if kk == "gs":
             gs = kwargs[kk]
             fixed = True
 
         if var is None:
             if kk.lower().startswith("var"):
                 var = kwargs[kk]
@@ -274,15 +287,15 @@
             if len(possible) > 0:
                 part2 = ",".join(possible)
                 raise ValueError(
                     f"{kk} is not a valid argument. Did you mean one of these? {part2}"
                 )
             else:
                 raise ValueError(f"{kk} is not a valid argument")
-    
+
     if gs is not None:
         if fig is None:
             raise ValueError("If you specify gs, you must also specify fig")
 
     ds1 = ds.copy()
 
     if not quiver:
@@ -418,22 +431,25 @@
         u = input_file.variables[u][:].squeeze()
         v = input_file.variables[v][:].squeeze()
 
         # mask where the values is 0 == land points
         # values = np.ma.masked_where(values == 0, values)
         u = np.ma.masked_where(u == 0, u)
         v = np.ma.masked_where(v == 0, v)
+    
+    if limits is None:
+        limits = [None, None]
 
     if not quiver:
         values = input_file.variables[ds1.variables[0]][:].squeeze()
 
         # mask where the values is 0 == land points
         values = np.ma.masked_where(values == 0, values)
 
-        if limits != None:
+        if limits is not None:
             if limits[0] is None:
                 limits[0] = np.min(values)
             if limits[1] is None:
                 limits[1] = np.max(values)
 
         if grid_colour == "auto":
             value_10 = values.min() + (values.max() - values.min()) * 0.3
@@ -458,21 +474,27 @@
                 min_value = np.nanpercentile(np.ma.filled(values, np.nan), 2)
                 max_value = np.nanpercentile(np.ma.filled(values, np.nan), 98)
             if r_min is not None:
                 min_value = np.nanpercentile(np.ma.filled(values, np.nan), r_min)
             if r_max is not None:
                 max_value = np.nanpercentile(np.ma.filled(values, np.nan), r_max)
 
-            if min_value < 0 and max_value > 0:
-                mid_point = 0
-                if colours == "auto":
-                    colours = "coolwarm"
-                    if land_auto:
-                        if land != "auto":
-                            land = "grey"
+        if limits is not None:
+            try:
+                if limits[0] < 0 and limits[1] > 0:
+                    min_value = limits[0]
+                    max_value = limits[1]
+                    mid_point = 0
+                    if colours == "auto":
+                        colours = "coolwarm"
+                        if land_auto and land is not None:
+                            if land != "auto":
+                                land = "grey"
+            except:
+                pass
 
         if colours == "auto":
             colours = "viridis"
 
     # generate the figure and the axes where to plot the map. When the axes are generated (either with add_subplot or add_axes, or any other way), the projection to be used need to be specified
     # the axes generated show the entire globe up to the cutoff latitude
     if fig is None:
@@ -514,30 +536,37 @@
             vmin = np.nanpercentile(np.ma.filled(values, np.nan), 2)
             vmax = np.nanpercentile(np.ma.filled(values, np.nan), 98)
         if limits is None:
             if r_min is not None:
                 vmin = np.nanpercentile(np.ma.filled(values, np.nan), r_min)
             if r_max is not None:
                 vmax = np.nanpercentile(np.ma.filled(values, np.nan), r_max)
+        
 
         if mid_point is not None:
             val_min = values.min()
             val_max = values.max()
+
+
+
+            if mid_point == 0.0:
+                if limits is not None:
+                    val_min = limits[0]
+                    val_max = limits[1]
             if robust and limits is None:
                 val_min = np.nanpercentile(np.ma.filled(values, np.nan), 2)
                 val_max = np.nanpercentile(np.ma.filled(values, np.nan), 98)
             if mid_point < val_min:
                 raise ValueError("mid_point is outside value range")
             if mid_point > val_max:
                 raise ValueError("mid_point is outside value range")
             adjustment = max(val_max - mid_point, mid_point - val_min)
             vmin = mid_point - adjustment
             vmax = mid_point + adjustment
 
-
         norm_plot = False
         if norm in ["log", "log10"]:
             norm = mpl.colors.LogNorm(vmin=vmin, vmax=vmax)
             norm_plot = True
         if norm is not None:
             vmin = None
             vmax = None
@@ -561,15 +590,15 @@
     # first define the gridliner object
     # crs define the units of the values (here spehric coorindates)
     # the other options are for grpahics, more details can be found here
     # https://scitools.org.uk/cartopy/docs/v0.13/matplotlib/gridliner.html
     # note that if x_inline and y_inline are not set to False, the labels of the axis could be written inside the map
 
     if quiver:
-        im =  ax.quiver(lon, lat, u, v, units='width', transform = data_crs)
+        im = ax.quiver(lon, lat, u, v, units="width", transform=data_crs)
 
     if not quiver:
         if grid_colour == "auto" and norm_plot:
             grid_colour = "black"
 
     if grid:
         if grid_colour == "auto":
@@ -630,15 +659,15 @@
         else:
             fraction = 0.046 * size[1] / size[0]
 
         if l_location == "bottom":
             cb = plt.colorbar(im, fraction=fraction, pad=0.04, location=l_location)
         else:
             cb = plt.colorbar(im, fraction=fraction, pad=0.04)
-    
+
         # add breaks to colorbar cb
         if breaks is not None:
             cb.set_ticks(breaks)
             cb.set_ticklabels(breaks)
 
         cbax = cb.ax
     if land is not None:
@@ -672,20 +701,17 @@
 
     if not quiver:
         if legend is not None:
             cbax.set_ylabel(legend)
         else:
             ds_contents = ds1.contents
             try:
-                label = (
-                    fix_long(ds_contents.long_name.values[0])
-                    + " ("
-                    + fix_label(ds_contents.unit.values[0])
-                    + ")"
-                )
+                label = fix_long(ds_contents.long_name.values[0])
+                if ds_contents.unit.values[0] is not None:
+                    label = label + " (" + fix_label(ds_contents.unit.values[0]) + ")"
             except:
                 print(
                     "Unable to parse legend from dataset contents. Check long names and units"
                 )
                 label = ""
 
             if l_location == "bottom":
@@ -696,74 +722,68 @@
             if l_location == "bottom":
                 cbax.set_xlabel(label)
             else:
                 cbax.set_ylabel(label)
 
         if legend_position is None:
             cb.remove()
-    
+
     if out is not None:
         print("saving as file")
         plt.savefig(out)
 
 
-
-def quiver_plot(ds, u = None, v = None, **kwargs):
+def quiver_plot(ds, u=None, v=None, **kwargs):
     """
     Quiver plot using u and v velocities
 
     Parameters
     ----------
     ds : nctoolkit Dataset
         dataset containing u and v velocities
     u : str
-        u velocity  
+        u velocity
     v : str
         v velocity
     **kwargs : dict
         kwargs to pass to pub_plot
 
     Returns
     -------
-    fig : matplotlib figure 
+    fig : matplotlib figure
         figure object
-    
+
 
     """
 
     ds.run()
 
     # check only one time step in ds
 
     if len(ds.times) > 1:
         raise ValueError("ds must contain only one time step for quiver_plot")
 
     # some type checks for u and v
 
     if u is None:
         raise ValueError("u must be specified")
-    
+
     if v is None:
         raise ValueError("v must be specified")
-    
+
     # check u and v are str
 
     if not isinstance(u, str):
         raise TypeError("u must be a string")
-    
+
     if not isinstance(v, str):
         raise TypeError("v must be a string")
 
     vars = ds.variables
 
     if u not in vars:
         raise ValueError("u not in dataset")
-    
+
     if v not in vars:
         raise ValueError("v not in dataset")
 
-    
-
-    pub_plot(ds, quiver = True, u = u, v = v, **kwargs)
-
-
-
+    pub_plot(ds, quiver=True, u=u, v=v, **kwargs)
```

### Comparing `nctoolkit-0.9.4/nctoolkit/strip_vars.py` & `nctoolkit-1.0.0/nctoolkit/strip_vars.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/subset.py` & `nctoolkit-1.0.0/nctoolkit/subset.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import warnings
 import numpy as np
 from datetime import datetime, timedelta
 
 from nctoolkit.cleanup import cleanup
 from nctoolkit.flatten import str_flatten
-from nctoolkit.runthis import run_this
 from nctoolkit.show import nc_years
 from nctoolkit.utils import cdo_version, version_above, name_check
 
 
 def fix_ind(x):
     if int(x) < 0:
         return int(x)
@@ -61,15 +60,15 @@
             raise ValueError("levels provided are not valid!")
         if levels[0] > levels[1]:
             raise ValueError("levels have the wrong order")
         levels = f"{levels[0]}/{levels[1]}"
 
     cdo_command = f"cdo -sellevel,{levels}"
 
-    run_this(cdo_command, self, "ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
 def select_period(self, period=None):
     """
     Select season from a dataset
 
     Parameters
@@ -98,15 +97,15 @@
         raise ValueError("Range order is incorrect")
 
     start = str(period[0]).split(" ")[0]
     end = period[1] - timedelta(days=1)
     end = str(end).split(" ")[0]
     cdo_command = f"cdo -seldate,{start},{end}"
 
-    run_this(cdo_command, self, "ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
 def select_seasons(self, season=None):
     """
     Select season from a dataset
 
     Parameters
@@ -121,15 +120,15 @@
     if not isinstance(season, str):
         raise TypeError("Invalid season supplied")
 
     if season not in ["DJF", "MAM", "JJA", "SON"]:
         raise ValueError("Invalid season supplied")
 
     cdo_command = f"cdo -select,season={season}"
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
 def select_hours(self, hours=None):
     """
     Select hours from a dataset
     This method will subset the dataset to only contain hours within the list given.
     A warning message will be provided when there are missing hours.
@@ -160,15 +159,15 @@
             raise TypeError(f"{x} is not an int")
         if x not in list(range(1, 32)):
             raise ValueError(f"{x} is not a hour")
 
     hours = str_flatten(hours, ",")
 
     cdo_command = f"cdo -selhour,{hours}"
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
 def select_days(self, days=None):
     """
     Select days from a dataset
     This method will subset the dataset to only contain days within the list given.
     A warning message will be provided when there are missing days.
@@ -199,15 +198,15 @@
             raise TypeError(f"{x} is not an int")
         if x not in list(range(1, 32)):
             raise ValueError(f"{x} is not a day")
 
     days = str_flatten(days, ",")
 
     cdo_command = f"cdo -selday,{days}"
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
 def select_months(self, months=None):
     """
     Select months from a dataset
     This method will subset the dataset to only contain months within the list given.
     A warning message will be provided when there are missing months.
@@ -238,15 +237,15 @@
             raise TypeError(f"{x} is not an int")
         if x not in list(range(1, 13)):
             raise ValueError(f"{x} is not a month")
 
     months = str_flatten(months, ",")
 
     cdo_command = f"cdo -selmonth,{months}"
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
 def select_years(self, years=None):
     """
     Select years from a dataset
     This method will subset the dataset to only contain years within the list given.
     A warning message will be provided when there are missing years.
@@ -340,21 +339,21 @@
         self.current = new_current
 
         if missing_files > 0:
             years = str_flatten(years, ",")
 
             cdo_command = f"cdo -selyear,{years}"
 
-            run_this(cdo_command, self, output="ensemble")
+            self.cdo_command(cdo_command, ensemble=False)
     else:
         years = str_flatten(years, ",")
 
         cdo_command = f"cdo -selyear,{years}"
 
-        run_this(cdo_command, self, output="one")
+        self.cdo_command(cdo_command, ensemble=True)
 
     cleanup()
 
 
 def select_variables(self, vars=None):
     """
     Select variables from a dataset
@@ -382,15 +381,15 @@
             if ("*" not in x) and ("?" not in x):
                 raise ValueError(f"{x} is not a valid netCDF variable name")
 
     vars_list = str_flatten(vars_list, ",")
 
     cdo_command = f"cdo -selname,{vars_list}"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
 def select_timesteps(self, times=None):
     """
     Select timesteps from a dataset
 
     Parameters
@@ -423,15 +422,15 @@
 
     times = [fix_ind(x) for x in times]
     times = [str(x) for x in times]
     times = str_flatten(times)
 
     cdo_command = f"cdo -seltimestep,{times}"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
 def subset(self, **kwargs):
     """
     A method for subsetting datasets to specific variables, years, longitudes etc.
     Operations are applied in the order supplied.
```

### Comparing `nctoolkit-0.9.4/nctoolkit/sumall.py` & `nctoolkit-1.0.0/nctoolkit/sumall.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/temp_file.py` & `nctoolkit-1.0.0/nctoolkit/temp_file.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/temporal_stat.py` & `nctoolkit-1.0.0/nctoolkit/temporal_stat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import copy
 
 from nctoolkit.cleanup import cleanup
-from nctoolkit.runthis import run_this, run_cdo, tidy_command
+from nctoolkit.runthis import run_cdo, tidy_command
 from nctoolkit.temporals import *
 from nctoolkit.temp_file import temp_file
 from nctoolkit.session import remove_safe
 
 
 def time_stat(self, stat="mean", over="time"):
     """Method to calculate a stat over all time steps"""
     # create cdo command and run it
 
     if len(self) == 0:
         raise ValueError("Failure due to empty dataset!")
 
     if over == "time":
         cdo_command = f"cdo -tim{stat}"
-        run_this(cdo_command, self, output="ensemble")
+        self.cdo_command(cdo_command, ensemble=False)
         return None
 
     if stat not in ["mean", "sum", "min", "max", "range", "var", "cumsum", "std"]:
         raise ValueError(f"{stat} is not a valid CDO stat!")
 
     # some tidying of over
     if isinstance(over, str):
```

### Comparing `nctoolkit-0.9.4/nctoolkit/thresholds.py` & `nctoolkit-1.0.0/nctoolkit/thresholds.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/to_lonlat.py` & `nctoolkit-1.0.0/nctoolkit/to_lonlat.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/to_nc.py` & `nctoolkit-1.0.0/nctoolkit/to_nc.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/toxarray.py` & `nctoolkit-1.0.0/nctoolkit/toxarray.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/tozlev.py` & `nctoolkit-1.0.0/nctoolkit/tozlev.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,102 +2,131 @@
 from nctoolkit.runthis import run_cdo
 from nctoolkit.temp_file import temp_file
 from nctoolkit.session import append_safe
 from nctoolkit.session import remove_safe
 import nctoolkit.api as api
 
 
-def to_zlevels(self, levels=None, thickness=None):
+def to_zlevels(self, levels=None, thickness=None, depths = None):
     """
     Convert datasets with non z-level verticals to z-levels
     Experimental method: Use at your own risk.
 
 
     Parameters
     -------------
     levels: list
         List of new z-levels. Must be positive and in metres.
     thickness: str or Dataset
         One of: a variable, in the dataset, which contains the variable thicknesses; a .nc file which contains
         the thicknesses; or a Dataset that contains the thicknesses. Note: the .nc file or Dataset must only contain
         one variable. Thickness should be in metres. Vertical interpolation will take the value from the mid-point of the level.
+    depths: str or Dataset
+        This or thickness must be supplied if fixed is False, otherwise vertical thickness/depth cannot be known.
+        Option argument when vertical levels vary in space.
+        One of: a variable, in the dataset, which contains the variable depths; a .nc file which contains
+        the depths; or a Dataset that contains the depths. Note: the .nc file or Dataset must only contain
+        one variable. Depths should be in metres, and be the mid-point of the level.
     """
     self.run()
 
     if len(self) > 1:
         raise ValueError("This currently only works on single file datasets")
 
-    if thickness is None:
+    if thickness is None and depths is None:
         if "e3t" in self.variables:
             thickness = "e3t"
 
     drop_this = None
 
-    if not isinstance(thickness, api.DataSet):
-        if thickness is None or not isinstance(thickness, str):
-            raise ValueError("Please provide a valid thickness or depths variable")
+    if depths is None:
+        if not isinstance(thickness, api.DataSet):
+            if thickness is None or not isinstance(thickness, str):
+                raise ValueError("Please provide a valid thickness or depths variable")
 
-    if thickness is None:
+    if thickness is None and depths is None:
         if not isinstance(depths, api.DataSet):
             if depths is None or not isinstance(depths, str):
                 raise ValueError("Please provide a valid thickness or depths variable")
 
     # Set up the thickness
 
     ds = self.copy()
 
     ds.subset(variables=ds.contents.query("nlevels > 1").variable)
     ds.run()
     vars = ds.variables
 
     sorted = False
 
-    if isinstance(thickness, api.DataSet):
-        ds_depths = thickness.copy()
-        ds_depths.run()
-        if len(ds_depths.variables) != 1:
-            raise ValueError("Please provide a thickness dataset with 1 variable!")
-        sorted = True
-
-    if sorted is False:
-        if thickness in self.variables:
-            ds_depths = open_data(self[0])
-            ds_depths.subset(variable=thickness)
+    if depths is None:
+        if isinstance(thickness, api.DataSet):
+            ds_depths = thickness.copy()
+            ds_depths.run()
+            if len(ds_depths.variables) != 1:
+                raise ValueError("Please provide a thickness dataset with 1 variable!")
+            sorted = True
+    else:
+        if isinstance(depths, api.DataSet):
+            ds_depths = depths.copy()
             ds_depths.run()
-            drop_this = thickness
-        else:
-            ds_depths = open_data(thickness)
             if len(ds_depths.variables) != 1:
-                raise ValueError("Please provide a thickness file with 1 variable!")
+                raise ValueError("Please provide a thickness or depths dataset with 1 variable!")
+            sorted = True
 
-    thick_var = ds_depths.variables[0]
+    if depths is None:
+        if sorted is False:
+            if thickness in self.variables:
+                ds_depths = open_data(self[0])
+                ds_depths.subset(variable=thickness)
+                ds_depths.run()
+                drop_this = thickness
+            else:
+                ds_depths = open_data(thickness)
+                if len(ds_depths.variables) != 1:
+                    raise ValueError("Please provide a thickness file with 1 variable!")
 
-    ds_depths.rename({thick_var: "thickness"})
-    ds_depths.cdo_command("setmisstoc,1.0")
-    ds_depths.run()
-    ds_thick = ds_depths.copy()
-    ds_thick.divide(2)
-    ds_depths.vertical_cumsum()
-    ds_depths.rename({"thickness": "depth"})
-    ds_depths.subtract(ds_thick)
-    ds_depths.assign( depth=lambda x: x.depth * (vertical_min(x.depth) < x.depth) * (isnan(x.depth) == False), drop=True,)
-    ds_depths.subset(times=0)
-    ds_depths.cdo_command("setmisstoc,-9999999")
-    ds_depths.run()
+        thick_var = ds_depths.variables[0]
 
-    zaxis = temp_file().replace(".", "")
-    append_safe(zaxis)
+        ds_depths.rename({thick_var: "thickness"})
+        ds_depths.cdo_command("setmisstoc,1.0")
+        ds_depths.run()
+        ds_thick = ds_depths.copy()
+        ds_thick.divide(2)
+        ds_depths.vertical_cumsum()
+        ds_depths.rename({"thickness": "depth"})
+        ds_depths.subtract(ds_thick)
+        ds_depths.assign( depth=lambda x: x.depth * (vertical_min(x.depth) < x.depth) * (isnan(x.depth) == False), drop=True,)
+        ds_depths.subset(times=0)
+        ds_depths.cdo_command("setmisstoc,-9999999")
+        ds_depths.run()
+
+
+    if isinstance(depths, str):
+        ds_depths = open_data(depths) 
 
     if not isinstance(levels, list):
         raise TypeError("levels must be a list")
 
     for ll in levels:
         if ll < 0:
             raise ValueError("levels must not have negative values")
 
+    # check the name if depths are supplied
+
+    if depths is not None:
+        if len(ds_depths.variables) > 1:
+            raise ValueError("Please provide a thickness or depths dataset with 1 variable!")
+        
+        if "depth" not in ds_depths.variables:
+            ds_depths.rename({ds_depths.variables[0]: "depth"})
+            ds_depths.run()
+
+    zaxis = temp_file().replace(".", "")
+    append_safe(zaxis)
     line3 = "levels = " + " ".join([str(x) for x in levels]) + " \n"
     with open(zaxis, "a") as the_file:
         x = the_file.write("zaxistype = depth_below_sea \n")
         x = the_file.write(f"size = {len(levels)} \n")
         x = the_file.write(line3)
 
     target = ds_depths.copy()
```

### Comparing `nctoolkit-0.9.4/nctoolkit/unify.py` & `nctoolkit-1.0.0/nctoolkit/unify.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/utils.py` & `nctoolkit-1.0.0/nctoolkit/utils.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/validator.py` & `nctoolkit-1.0.0/nctoolkit/validator.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/validator_funs.py` & `nctoolkit-1.0.0/nctoolkit/validator_funs.py`

 * *Files identical despite different names*

### Comparing `nctoolkit-0.9.4/nctoolkit/verticals.py` & `nctoolkit-1.0.0/nctoolkit/verticals.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import warnings
 import copy
 from nctoolkit.cleanup import cleanup
 from nctoolkit.api import open_data
 from nctoolkit.temp_file import temp_file
 from nctoolkit.utils import version_above, cdo_version
 from nctoolkit.flatten import str_flatten
-from nctoolkit.runthis import run_this 
 import nctoolkit.api as api
 
 
 def bottom(self):
     """
     Extract the bottom level from a dataset
     This extracts the bottom level from each netCDF file. Please note that for
@@ -44,17 +43,17 @@
     cdo_result = subprocess.run(
         "cdo nlevel " + ff, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE
     ).stdout
     n_levels = int(
         str(cdo_result).replace("b'", "").strip().replace("'", "").split("\\n")[0]
     )
 
-    cdo_command = f"cdo -sellevidx,{str(n_levels)}"
+    cdo_command = f"-sellevidx,{str(n_levels)}"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
 def top(self):
     """
     Extract the top/surface level from a dataset
     This extracts the first vertical level from each file in a dataset.
 
@@ -65,39 +64,46 @@
 
     >>> ds.top()
 
     This method is most useful for things like oceanic data, where this method will extract the sea surface.
     """
 
     cdo_command = "cdo -sellevidx,1"
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
-def vertical_interp(self, levels=None, fixed=None, thickness=None):
+def vertical_interp(self, levels=None, fixed=None, thickness=None, depths = None):
     """
     Verticaly interpolate a dataset based on given vertical levels
     This is calculated for each time step and grid cell
     Note: This requires consistent vertical levels in space. For the likes of sigma-coordinates,
     please use to_zlevels.
 
     Parameters
     -------------
     levels : list, int or str
         list of vertical levels, for example depths for an ocean model, to vertically
         interpolate to. These must be floats or ints.
     fixed : bool
         Define whether the vertical levels are the same in all spatial locations.
         Set to True if they are, e.g. you have z-levels. If you have the likes of sigma-coordinates,
-        set this to True.
+        set this to False.
     thickness: str or Dataset
-        This must be supplied if fixed is False, otherwise vertical thickness cannot be known.
+        This or depths must be supplied if fixed is False, otherwise vertical thickness/depth cannot be known.
         Option argument when vertical levels vary in space.
         One of: a variable, in the dataset, which contains the variable thicknesses; a .nc file which contains
         the thicknesses; or a Dataset that contains the thicknesses. Note: the .nc file or Dataset must only contain
         one variable. Thickness should be in metres. Vertical interpolation will take the value from the mid-point of the level.
+    depths: str or Dataset
+        This or thickness must be supplied if fixed is False, otherwise vertical thickness/depth cannot be known.
+        Option argument when vertical levels vary in space.
+        One of: a variable, in the dataset, which contains the variable depths; a .nc file which contains
+        the depths; or a Dataset that contains the depths. Note: the .nc file or Dataset must only contain
+        one variable. Depths should be in metres, and be the mid-point of the level.
+
 
     Examples
     ------------
 
     If you wanted to vertically interpolate a dataset with spatially consistent vertical levels to 5 and 10 metres, you would do the following:
 
     >>> ds.vertical_interp(levels = [5,10], fixed = True)
@@ -107,27 +113,28 @@
 
     """
 
     if fixed is None:
         if thickness is None:
             raise ValueError("You must provide the fixed arg")
 
-    if fixed is False:
-        if thickness is None:
-            raise ValueError("Please provide thickness")
+    if depths is None:
+        if fixed is False:
+            if thickness is None:
+                raise ValueError("Please provide thickness")
 
     if not isinstance(fixed, bool):
         if thickness is None:
             raise TypeError("fixed must be a bool")
 
     if thickness is not None:
         fixed = False
 
     if fixed is False:
-        self.to_zlevels(levels=levels, thickness=thickness)
+        self.to_zlevels(levels=levels, thickness=thickness, depths = depths)
         return None
 
     if levels is None:
         raise ValueError("Please supply vertical depths")
 
     # first a quick fix for the case when there is only one vertical depth
 
@@ -139,21 +146,21 @@
     for vv in levels:
         if not isinstance(vv, (int, float)):
             raise TypeError(f"{vv} is not a valid depth")
 
     levels = str_flatten(levels, ",")
     cdo_command = f"cdo -intlevel,{levels}"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
 def vertstat(self, stat="mean"):
     """Method to calculate the vertical mean from a function"""
     cdo_command = f"cdo -vert{stat}"
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
 def vertical_mean(self, thickness=None, depth_range=None, fixed=None):
     """
     Calculate the depth-averaged mean for each variable
     This is calculated for each time step and grid cell
 
@@ -521,15 +528,15 @@
     If you wanted to invert the vertical levels, you would do this:
 
     >>> ds.invert_levels()
 
     """
     cdo_command = "cdo -invertlev"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble=False)
 
 
 def bottom_mask(self):
     """
     Create a mask identifying the deepest cell without missing values.
     This converts a dataset to a mask identifying which cell represents the bottom,
     for example the seabed. 1 identifies the deepest cell with non-missing values.
```

### Comparing `nctoolkit-0.9.4/nctoolkit/zonals.py` & `nctoolkit-1.0.0/nctoolkit/zonals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-from nctoolkit.runthis import run_this
 from nctoolkit.utils import is_curvilinear
 from nctoolkit.api import open_data
 
 
 def zonstat(self, stat="mean"):
     """Method to calculate the zonal statistic from a netCDF file"""
 
     for ff in self:
         if is_curvilinear(ff):
             raise TypeError(f"zonal_{stat} cannot be calculated for curvilinear grids.")
 
     cdo_command = f"cdo -zon{stat}"
 
-    run_this(cdo_command, self, output="ensemble")
+    self.cdo_command(cdo_command, ensemble = False)
 
 
 def zonal_sum(self, by_area=False):
     """
     Calculate the zonal sum for each year/month combination in files.
     This applies to each file in an ensemble.
```

### Comparing `nctoolkit-0.9.4/nctoolkit.egg-info/SOURCES.txt` & `nctoolkit-1.0.0/nctoolkit.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 CODE_OF_CONDUCT.md
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
+benchmarks/benchmark_nctoolkit_versus_xarray.ipynb
 cheatsheet/nctoolkit_cheatsheet.pdf
 cheatsheet/nctoolkit_cheatsheet.pptx
 checklists/api_checker.ipynb
 data/geotiff.tif
 data/pubplot_test.png
 data/test1.html
 data/test2.html
```

### Comparing `nctoolkit-0.9.4/setup.py` & `nctoolkit-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,26 +43,26 @@
 
 
 extras_require["complete"] = ["geoviews", "rioxarray", "cfchecker", "geocube", "geopandas"]
 
 REQUIREMENTS = [i.strip() for i in open("requirements.txt").readlines()]
 
 setup(name='nctoolkit',
-      version='0.9.4',
+      version='1.0.0',
       description=DESCRIPTION,
       long_description=LONG_DESCRIPTION,
       python_requires='>=3.6.1',
       classifiers=[
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS",
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 
       project_urls=PROJECT_URLS,
       url = "https://github.com/pmlmodelling/nctoolkit",
       author='Robert Wilson',
       maintainer='Robert Wilson',
       author_email='rwi@pml.ac.uk',
```

### Comparing `nctoolkit-0.9.4/testing/test_parallel.py` & `nctoolkit-1.0.0/testing/test_parallel.py`

 * *Files identical despite different names*

