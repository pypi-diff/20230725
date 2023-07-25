# Comparing `tmp/sfrmaker-0.9.3.tar.gz` & `tmp/sfrmaker-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sfrmaker-0.9.3.tar", last modified: Mon Dec 19 16:06:26 2022, max compression
+gzip compressed data, was "sfrmaker-0.9.4.tar", last modified: Thu Jan 19 20:22:38 2023, max compression
```

## Comparing `sfrmaker-0.9.3.tar` & `sfrmaker-0.9.4.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 16:06:26.106350 sfrmaker-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/AUTHORS.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      299 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2022-12-19 16:06:26.106350 sfrmaker-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 16:06:26.102349 sfrmaker-0.9.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      797 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 16:06:26.102349 sfrmaker-0.9.3/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 16:06:26.102349 sfrmaker-0.9.3/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/docs/source/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      135 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/docs/source/api/sfrmaker.flows.rst
--rw-r--r--   0 runner    (1001) docker     (123)      133 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/docs/source/api/sfrmaker.grid.rst
--rw-r--r--   0 runner    (1001) docker     (123)      136 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/docs/source/api/sfrmaker.lines.rst
--rw-r--r--   0 runner    (1001) docker     (123)      148 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/docs/source/api/sfrmaker.mf5to6.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/docs/source/api/sfrmaker.observations.rst
--rw-r--r--   0 runner    (1001) docker     (123)      151 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/docs/source/api/sfrmaker.preprocessing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      139 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/docs/source/api/sfrmaker.sfrdata.rst
--rw-r--r--   0 runner    (1001) docker     (123)      139 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/docs/source/api/sfrmaker.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      239 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/docs/source/concepts.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/docs/source/config-summary.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15536 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/docs/source/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 16:06:26.102349 sfrmaker-0.9.3/docs/source/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5952 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/docs/source/examples/meras.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/docs/source/examples/tf.rst
--rw-r--r--   0 runner    (1001) docker     (123)      941 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/docs/source/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/docs/source/inputs.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15515 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/docs/source/philosophy.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/docs/source/references.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10009 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/docs/source/release-history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/docs/source/troubleshooting.rst
--rw-r--r--   0 runner    (1001) docker     (123)      198 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      287 2022-12-19 16:06:26.106350 sfrmaker-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 16:06:26.110350 sfrmaker-0.9.3/sfrmaker/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/sfrmaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2022-12-19 16:06:26.110350 sfrmaker-0.9.3/sfrmaker/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/sfrmaker/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8778 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/sfrmaker/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/sfrmaker/elevations.py
--rw-r--r--   0 runner    (1001) docker     (123)    11555 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/sfrmaker/fileio.py
--rw-r--r--   0 runner    (1001) docker     (123)    27112 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/sfrmaker/flows.py
--rw-r--r--   0 runner    (1001) docker     (123)     9587 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/sfrmaker/gis.py
--rw-r--r--   0 runner    (1001) docker     (123)    22971 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/sfrmaker/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    51718 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/sfrmaker/lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/sfrmaker/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    21814 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/sfrmaker/mf5to6.py
--rw-r--r--   0 runner    (1001) docker     (123)    15562 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/sfrmaker/nhdplus_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22377 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/sfrmaker/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)    74549 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/sfrmaker/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11332 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/sfrmaker/reaches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/sfrmaker/rivdata.py
--rw-r--r--   0 runner    (1001) docker     (123)    11065 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/sfrmaker/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)    83265 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/sfrmaker/sfrdata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 16:06:26.106350 sfrmaker-0.9.3/sfrmaker/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/sfrmaker/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10446 2022-12-19 16:06:12.000000 sfrmaker-0.9.3/sfrmaker/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2022-12-19 16:06:13.000000 sfrmaker-0.9.3/sfrmaker/test/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)        2 2022-12-19 16:06:13.000000 sfrmaker-0.9.3/sfrmaker/test/test_elevations.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2022-12-19 16:06:13.000000 sfrmaker-0.9.3/sfrmaker/test/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2022-12-19 16:06:13.000000 sfrmaker-0.9.3/sfrmaker/test/test_fileio.py
--rw-r--r--   0 runner    (1001) docker     (123)     9248 2022-12-19 16:06:13.000000 sfrmaker-0.9.3/sfrmaker/test/test_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2022-12-19 16:06:13.000000 sfrmaker-0.9.3/sfrmaker/test/test_from_nhdplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     7382 2022-12-19 16:06:13.000000 sfrmaker-0.9.3/sfrmaker/test/test_from_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2022-12-19 16:06:13.000000 sfrmaker-0.9.3/sfrmaker/test/test_gis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2022-12-19 16:06:13.000000 sfrmaker-0.9.3/sfrmaker/test/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2022-12-19 16:06:13.000000 sfrmaker-0.9.3/sfrmaker/test/test_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2022-12-19 16:06:13.000000 sfrmaker-0.9.3/sfrmaker/test/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2022-12-19 16:06:13.000000 sfrmaker-0.9.3/sfrmaker/test/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2022-12-19 16:06:13.000000 sfrmaker-0.9.3/sfrmaker/test/test_mf5to6.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2022-12-19 16:06:13.000000 sfrmaker-0.9.3/sfrmaker/test/test_nhdplus_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2022-12-19 16:06:13.000000 sfrmaker-0.9.3/sfrmaker/test/test_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    10966 2022-12-19 16:06:13.000000 sfrmaker-0.9.3/sfrmaker/test/test_observations.py
--rw-r--r--   0 runner    (1001) docker     (123)    15028 2022-12-19 16:06:13.000000 sfrmaker-0.9.3/sfrmaker/test/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2022-12-19 16:06:13.000000 sfrmaker-0.9.3/sfrmaker/test/test_routing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13151 2022-12-19 16:06:13.000000 sfrmaker-0.9.3/sfrmaker/test/test_sfr_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2022-12-19 16:06:13.000000 sfrmaker-0.9.3/sfrmaker/test/test_units.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2022-12-19 16:06:13.000000 sfrmaker-0.9.3/sfrmaker/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2022-12-19 16:06:13.000000 sfrmaker-0.9.3/sfrmaker/test/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10035 2022-12-19 16:06:13.000000 sfrmaker-0.9.3/sfrmaker/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    18196 2022-12-19 16:06:13.000000 sfrmaker-0.9.3/sfrmaker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 16:06:26.106350 sfrmaker-0.9.3/sfrmaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2022-12-19 16:06:26.000000 sfrmaker-0.9.3/sfrmaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2022-12-19 16:06:26.000000 sfrmaker-0.9.3/sfrmaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 16:06:26.000000 sfrmaker-0.9.3/sfrmaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2022-12-19 16:06:26.000000 sfrmaker-0.9.3/sfrmaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-19 16:06:26.000000 sfrmaker-0.9.3/sfrmaker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    68619 2022-12-19 16:06:13.000000 sfrmaker-0.9.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 20:22:38.094841 sfrmaker-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/AUTHORS.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-01-19 20:22:38.094841 sfrmaker-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 20:22:38.086841 sfrmaker-0.9.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 20:22:38.086841 sfrmaker-0.9.4/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 20:22:38.086841 sfrmaker-0.9.4/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/docs/source/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/docs/source/api/sfrmaker.flows.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/docs/source/api/sfrmaker.grid.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/docs/source/api/sfrmaker.lines.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/docs/source/api/sfrmaker.mf5to6.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/docs/source/api/sfrmaker.observations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/docs/source/api/sfrmaker.preprocessing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/docs/source/api/sfrmaker.sfrdata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/docs/source/api/sfrmaker.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/docs/source/concepts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/docs/source/config-summary.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16595 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/docs/source/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 20:22:38.086841 sfrmaker-0.9.4/docs/source/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/docs/source/examples/meras.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/docs/source/examples/tf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/docs/source/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/docs/source/inputs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18588 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/docs/source/philosophy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/docs/source/references.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/docs/source/release-history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/docs/source/troubleshooting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-01-19 20:22:38.094841 sfrmaker-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 20:22:38.094841 sfrmaker-0.9.4/sfrmaker/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/sfrmaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-01-19 20:22:38.094841 sfrmaker-0.9.4/sfrmaker/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/sfrmaker/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8778 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/sfrmaker/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/sfrmaker/elevations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/sfrmaker/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27112 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/sfrmaker/flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/sfrmaker/gis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23126 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/sfrmaker/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52140 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/sfrmaker/lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/sfrmaker/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21814 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/sfrmaker/mf5to6.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16024 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/sfrmaker/nhdplus_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22377 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/sfrmaker/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74549 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/sfrmaker/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/sfrmaker/reaches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/sfrmaker/rivdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/sfrmaker/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83265 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/sfrmaker/sfrdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 20:22:38.094841 sfrmaker-0.9.4/sfrmaker/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/sfrmaker/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10446 2023-01-19 20:22:26.000000 sfrmaker-0.9.4/sfrmaker/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-01-19 20:22:27.000000 sfrmaker-0.9.4/sfrmaker/test/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-01-19 20:22:27.000000 sfrmaker-0.9.4/sfrmaker/test/test_elevations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-01-19 20:22:27.000000 sfrmaker-0.9.4/sfrmaker/test/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-01-19 20:22:27.000000 sfrmaker-0.9.4/sfrmaker/test/test_fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9248 2023-01-19 20:22:27.000000 sfrmaker-0.9.4/sfrmaker/test/test_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-01-19 20:22:27.000000 sfrmaker-0.9.4/sfrmaker/test/test_from_nhdplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-01-19 20:22:27.000000 sfrmaker-0.9.4/sfrmaker/test/test_from_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-01-19 20:22:27.000000 sfrmaker-0.9.4/sfrmaker/test/test_gis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-01-19 20:22:27.000000 sfrmaker-0.9.4/sfrmaker/test/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-01-19 20:22:27.000000 sfrmaker-0.9.4/sfrmaker/test/test_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-01-19 20:22:27.000000 sfrmaker-0.9.4/sfrmaker/test/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-01-19 20:22:27.000000 sfrmaker-0.9.4/sfrmaker/test/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-01-19 20:22:27.000000 sfrmaker-0.9.4/sfrmaker/test/test_mf5to6.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-19 20:22:27.000000 sfrmaker-0.9.4/sfrmaker/test/test_nhdplus_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-01-19 20:22:27.000000 sfrmaker-0.9.4/sfrmaker/test/test_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-01-19 20:22:27.000000 sfrmaker-0.9.4/sfrmaker/test/test_observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15028 2023-01-19 20:22:27.000000 sfrmaker-0.9.4/sfrmaker/test/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-01-19 20:22:27.000000 sfrmaker-0.9.4/sfrmaker/test/test_routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13151 2023-01-19 20:22:27.000000 sfrmaker-0.9.4/sfrmaker/test/test_sfr_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-01-19 20:22:27.000000 sfrmaker-0.9.4/sfrmaker/test/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-01-19 20:22:27.000000 sfrmaker-0.9.4/sfrmaker/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-01-19 20:22:27.000000 sfrmaker-0.9.4/sfrmaker/test/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10035 2023-01-19 20:22:27.000000 sfrmaker-0.9.4/sfrmaker/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18196 2023-01-19 20:22:27.000000 sfrmaker-0.9.4/sfrmaker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 20:22:38.090841 sfrmaker-0.9.4/sfrmaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-01-19 20:22:38.000000 sfrmaker-0.9.4/sfrmaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-01-19 20:22:38.000000 sfrmaker-0.9.4/sfrmaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 20:22:38.000000 sfrmaker-0.9.4/sfrmaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-01-19 20:22:38.000000 sfrmaker-0.9.4/sfrmaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-19 20:22:38.000000 sfrmaker-0.9.4/sfrmaker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    68619 2023-01-19 20:22:27.000000 sfrmaker-0.9.4/versioneer.py
```

### Comparing `sfrmaker-0.9.3/LICENSE.md` & `sfrmaker-0.9.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/PKG-INFO` & `sfrmaker-0.9.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfrmaker
-Version: 0.9.3
+Version: 0.9.4
 Summary: Python package for rapid creation of streamflow routing networks.
 Home-page: https://github.com/aleaf/sfrmaker
 Author: USGS
 Author-email: aleaf@usgs.gov
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `sfrmaker-0.9.3/Readme.md` & `sfrmaker-0.9.4/Readme.md`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/docs/Makefile` & `sfrmaker-0.9.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/docs/make.bat` & `sfrmaker-0.9.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/docs/source/conf.py` & `sfrmaker-0.9.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/docs/source/config-summary.rst` & `sfrmaker-0.9.4/docs/source/config-summary.rst`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/docs/source/contributing.rst` & `sfrmaker-0.9.4/docs/source/contributing.rst`

 * *Files 6% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
 - Imports should be grouped with standard library imports first,
   3rd-party libraries next, and SFRmaker imports third.  Within each
   grouping, imports should be alphabetized.  Always use absolute
   imports when possible, and explicit relative imports for local
   imports when necessary in tests. Imports can be sorted automatically using the isort package with a pre-commit hook. For more details see :ref:`below <contributing_style>`.
 
-- SFRmaker supports Python 3.7+ only.
+- SFRmaker supports Python 3.9+ only.
 
 
 Seven Steps for Contributing
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 There are seven basic steps to contributing to *SFRmaker*:
 
@@ -296,14 +296,28 @@
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Once you've made changes and pushed them to your forked repository, you then
 submit a pull request to have them integrated into the *SFRmaker* code base.
 
 You can find a pull request (or PR) tutorial in the `GitHub's Help Docs <https://help.github.com/articles/using-pull-requests/>`_.
 
+.. note::
+   Please make pull requests to the develop branch; the master branch is typically only updated when releases are made to PyPI.
+
+.. note::
+   If you haven't already, it's also good practice to rebase the feature branch that your are working on (e.g. ``shiny-new-feature`` above) to the develop branch on the main repository. This brings your branch into sync with the main develop branch, and places the commits you are adding (the new feature or bug fix, etc) on top of it. If you see a message in the pull request dialog on GitHub such as "This branch cannot be rebased due to conflicts", rebasing your feature branch to the develop branch on the main repository should fix it. Note that you may have to use the ``-f`` flag to force push to your fork after rebasing. For example:
+
+   .. code-block:: 
+
+     git fetch upstream
+     git rebase upstream/develop
+     git push origin shiny-new-feature
+
+   (this assumes that your remote pointing to the main repository is called *upstream*, and your remote pointing to your fork is called *origin*) 
+
 .. _contributing_style:
 
 Style Guide & Linting
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 SFRmaker tries to follow the `PEP8 <http://www.python.org/dev/peps/pep-0008/>`_ standard. At this point, there's no enforcement of this, but I am considering implementing `Black <https://black.readthedocs.io/en/stable/>`_, which automates a code style that is PEP8-complient. Many editors perform automatic linting that makes following PEP8 easy.
```

### Comparing `sfrmaker-0.9.3/docs/source/examples/meras.rst` & `sfrmaker-0.9.4/docs/source/examples/meras.rst`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/docs/source/examples/tf.rst` & `sfrmaker-0.9.4/docs/source/examples/tf.rst`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/docs/source/examples.rst` & `sfrmaker-0.9.4/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/docs/source/index.rst` & `sfrmaker-0.9.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/docs/source/inputs.rst` & `sfrmaker-0.9.4/docs/source/inputs.rst`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/docs/source/installation.rst` & `sfrmaker-0.9.4/docs/source/installation.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,66 +1,85 @@
 ============
 Installation
 ============
 
 Installing python dependencies with Conda
 -----------------------------------------
-``sfrmaker`` depends on a number of python packages, many of which have external C library dependencies. The easiest way to install most of these is with `conda`_. A few packages are not available via conda, and must be installed with `pip`_. If you are on the USGS internal network, see the `Considerations for USGS Users`_ section below first.
+SFRmaker depends on a number of python packages, many of which have external C library dependencies. The easiest way to install most of these is with a package installer like `Conda`_. A few packages are not available via conda, and must be installed with `pip`_. If you are on the USGS internal network, see the `Considerations for USGS Users`_ section below first.
 
-Download and install the 64-bit `Anaconda python distribution`_ or `Miniconda <https://docs.conda.io/en/latest/miniconda.html>`_
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+Download and install a python distribution and Conda-like package installer 
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+There are many ways to do this:
 
-  * Anaconda comes with a larger selection of popular data science and scientific packages, making it ideal for those who use python frequently for scientific computing.
-  * Miniconda is a minimal installer with a much smaller footprint, making it ideal for those who only want to use ``SFRmaker``.
-  * **Make sure to install Anaconda or Miniconda to your username** (not at the system level). More often than not, installing at the system level (for all users) seems to result in issues with library dependencies (for example, import of ``fiona`` or ``rasterio`` failing because gdal isn't found). It is also good practice to periodically do a `clean uninstall`_ of Anaconda, which at the system level requires admin. privileges.
+    * The `Anaconda python distribution`_ comes with a large selection of popular data science and scientific packages pre-installed.
 
-    * In the installer, at the “Destination Select” step, select “Install for me only.” It should say something about how the software will be installed to your home folder.
-    * If your installer skips the “Destination Select” step, when you get to "Installation Type", click “Change Install Location” and then “Install for me only.”
+    * `Miniconda <https://docs.conda.io/en/latest/miniconda.html>`_ is a minimal installer with a much smaller footprint, making it ideal for creating python environments dedicated to specific tasks (a recommended practice).
+
+    * `Mambaforge <https://github.com/conda-forge/miniforge#mambaforge>`_ is like Miniconda, but pre-configured to use the `Mamba`_ installer, and only the `conda-forge <https://conda-forge.org/docs/user/introduction.html>`_ channel for getting packages (more below). If the above two options don't work (for example, the Conda installer fails or gets stuck on the "solve" step), this may be your best option.
+
+**Make sure to install Anaconda or Miniconda to your username** (not at the system level). More often than not, installing at the system level (for all users) seems to result in issues with library dependencies (for example, import of ``fiona`` or ``rasterio`` failing because gdal isn't found). It is also good practice to periodically do a `clean uninstall`_ of Anaconda, which at the system level requires admin. privileges.
+
+  * In the installer, at the “Destination Select” step, select “Install for me only.” It should say something about how the software will be installed to your home folder.
+
+  * If your installer skips the “Destination Select” step, when you get to "Installation Type", click “Change Install Location” and then “Install for me only.”
 
 Download an environment file
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
   * `requirements.yml`_ for a `conda environment`_ with the minimum packages required to run SFRmaker, or
+
   * `gis.yml`_ for a more full set of packages in the python geospatial stack, including Jupyter Notebooks and packages needed for testing, documentation and packaging. Note that the environment described by ``requirements.yml`` is called `sfrmaker`, while the environment in ``gis.yml`` is called `gis`.
 
     .. note::
         To download the above YAML files, simply follow the links to get the raw text and then go to File > Save within your web browser, and save the text as a YAML file (with the `.yaml` or `.yml` extension).
 
-  * Alternatively, clone (`using git`_) or `download`_ the ``sfrmaker`` repository, which includes the two environment files at the root level.
-  * Note that both of these environment files contain a ``pip`` section of packages that will be installed with pip, after the ``conda`` packages are installed.
+  * Alternatively, clone (`using git`_) or `download`_ the SFRmaker repository, which includes the two environment files at the root level.
+
+  * Note that both of these environment files contain a ``pip`` section of packages that will be installed with pip, after the Conda packages are installed.
 
 Creating a `Conda environment`_ using `Mamba`_
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 If you are on the USGS internal network, see the `Considerations for USGS Users`_ section below first.
 
 While Conda can of course be used to create a Conda environment, the Mamba package solver is generally faster and more robust, especially for larger, more complex environments like the included ``requirements.yml``. Mamba is a reimplementation of the conda package manager in C++.
 
-To get started, open an Anaconda Command Prompt on Windows or a terminal window on OSX and point it to the location of ``requirements.yml`` or ``gis.yml`` and enter:
+Before using Mamba, you will need to `install it first <https://mamba.readthedocs.io/en/latest/installation.html>`_.
+
+Python packages are available from conda via channels. Conda comes preconfigured to install packages from the default channel, which is maintained by Anaconda, Inc. In general, you may have better luck exclusively using the `conda-forge <https://conda-forge.org/docs/user/introduction.html>`_ channel instead, which is community-based and intended to provide a single location to get any package, with a minimum of hassle. In general, it is bad practice to mix package channels within a single environment. You can read more `here <https://conda-forge.org/docs/user/introduction.html>`__, but to set conda-forge as the default:
+
+.. code-block:: bash
+
+    conda config --add channels conda-forge
+
+.. note::
+    If you are having trouble installing Mamba (for example, the conda package solver fails when you try to install it, or takes an excessively long time), you may have better luck uninstalling `Anaconda completely <clean uninstall>`_ and installing `Mambaforge <https://github.com/conda-forge/miniforge#mambaforge>`_ instead, as directed in the Mamba install instructions. Mambaforge solves both of the above problems by providing a minimal python distribution and conda-style package installer that is preconfigured to use both `conda-forge <https://conda-forge.org/docs/user/introduction.html>`_ and `Mamba`_.
+
+Once you have a python distribution and mamba installed, to create the conda environment, open a new Anaconda Command Prompt on Windows or a new terminal window on OSX and point it to the location of ``requirements.yml`` or ``gis.yml`` and enter:
 
 .. code-block:: bash
 
     mamba env create -f requirements.yml
 
 Building the environment will probably take a while. If the build fails because of an SSL error, fix the problem (see `Considerations for USGS Users`_ below) and either:
 
     .. note::
         Creating the ``requirements.yml`` environment (or any environment with ``git+https: ...`` installs) requires Git to be installed and visible in the system path where ``env create`` is being run. If Git is installed and somehow not in the system path, it can be added to the system path on Windows 10 without admin. rights via the "environment variables" editor under User Accounts in the Control Panel (Google it).
 
     a) 	Update the environment
 
         .. code-block:: bash
 
-            conda env update -f requirements.yml
+            mamba env update -f requirements.yml
 
     b) 	or remove and reinstall it:
 
         .. code-block:: bash
 
             conda env remove -n sfrmaker
-            conda env create -f requirements.yml
+            mamba env create -f requirements.yml
 
 Keeping the Conda environment up to date
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 The python packages and other open source software libraries that SFRmaker depends on are continually changing. SFRmaker aims to mostly follow the `Numpy guidelines for package support <https://numpy.org/neps/nep-0029-deprecation_policy.html>`_, which effectively means that the two latest minor versions of Python (e.g. 3.9 and 3.8) and their associated Numpy versions will be supported. However, occasionally backwards compatability with a particular package may be broken in a shorter timeframe, in which case the minimum required version of that package will be specified in the ``requirements.yml`` file. All of this to say that your Conda environment will eventually get out of date. The `Conda documentation <https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html>`_ has instructions for updating packages within a Conda environment, but at some point (perhaps a few times a year) it is good practice to simply delete the environment and rebuild it from the `.yml` file. Every so often, you may also want to reinstall Anaconda after a `clean uninstall`_.
 
 Installing SFRmaker
 ------------------------
@@ -137,32 +156,44 @@
 .. note::
     If you are making local changes to SFRmaker that you want to contribute, the workflow is slightly different. See the :ref:`Contributing to SFRmaker` page for more details.
 
 
 The advantage of installing the source code in-place is that any changes you make are automatically incorporated into your python environment, without any additional install commands. When debugging in an interactive development environment (IDE) such as Pycharm or VS Code, error tracebacks and inspection features go to the actual source code, not the version installed in the ``site-packages`` folder. Additionally, since this install is done through pip, ``pip uninstall``
 will work to remove the package, and the current version of the package (including the latest commit information) will be visible with ``conda list``.
 
+Installing the IPython kernel to use SFRmaker in Jupyter Notebooks
+------------------------------------------------------------------------------------------------
+This step may not be needed if you already have an existing Python environment with the packages required by SFRmaker *and* Jupyter Notebook installed. However, if you'd like to use SFRmaker in a Jupyter Notebook with the included ``sfrmaker`` environment (specified in ``requirements.yml``), you'll most likely need to install the IPython kernel in that environment. You can do this at the command line or terminal window (with ``sfrmaker`` activated):
+
+.. code-block:: bash
+
+    python -m ipykernel install --user --name sfrmaker --display-name "sfrmaker"
+
+
+The first instance of ``sfrmaker`` in this command is the environment to install the kernel to, and the second instance (in quotes) is the name that will appear in the ``Kernel`` menu within Jupyter Notebook. To use the kernel, simply select it from the ``Kernel > Change kernel`` menu within  Jupyter Notebook.
+
 Best practices
 ------------------------
 
-* Install the \*conda distribution of your choice to your user account, NOT at the system level. Installing to your user means you have rights to delete and reinstall Anaconda as-needed, as well as to edit any configuration files for ``pip``, ``conda``, etc. Installing at the system level also just seems to lead to more confusing problems with dependencies, at least in the USGS.
+* Install the \*conda distribution of your choice to your user account, NOT at the system level. Installing to your user means you have rights to delete and reinstall Anaconda as-needed, as well as to edit any configuration files for pip, Conda, etc. Installing at the system level also just seems to lead to more confusing problems with dependencies, at least in the USGS.
 * Periodically (maybe a few times a year?) fully remove your \*conda distribution and reinstall it. If you just can't get things to work (packages won't import or produce DLL errors on import, adding or upgrading a package takes a very long time or results in excessive upgrades or downgrades of other packages, etc.), fully removing and reinstalling \*conda just may resolve your issues.
 * Don't use your base environment; create and delete environments as needed. Conda is generally pretty good about managing packages between environments without wasting a lot of disk space.
 * Use an environment file (as above) to create a conda environment, instead of installing packages ad-hoc.
-* Use ``mamba`` instead of ``conda``; it just works better for environments with a lot of packages.
-* After setting up the above conda environment, scan the screen output to make sure that everything installed correctly, especially the packages installed through ``pip``.
+* Use Mamba instead of Conda; it just works better for environments with a lot of packages.
+* After setting up the above conda environment, scan the screen output to make sure that everything installed correctly, especially the packages installed through pip.
+* Avoid mixing package channels within a Conda environment. Strictly sticking to conda-forge may yield the best results.
 * Use `conda-pack`_, rather than an overly-detailed environment file, to guarantee reproducibility.
 
 
 _`Considerations for USGS Users`
 --------------------------------
 Using conda or pip on the USGS network requires SSL verification, which can cause a number of issues.
 If you are encountering persistant issues with creating the conda environment,
 you may have better luck trying the install off of the USGS network (e.g. at home).
-See `here <https://tst.usgs.gov/applications/application-and-script-signing/>`_ for more information
+See `here <https://tst.usgs.gov/applications/application-and-script-signing/>`__ for more information
 about SSL verification on the USGS network, and to download the DOI SSL certificate.
 
 _`Installing the DOI SSL certificate for use with pip`
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 1) `Download the DOI SSL certificate (internal DOI network only) <https://tst.usgs.gov/applications/application-and-script-signing/>`_
 2) On Windows, create the file ``C:\Users\<your username>\AppData\Roaming\pip\pip.ini``.
    On OSX, create ``/Users/<your username>/Library/Application Support/pip/pip.conf``.
@@ -204,15 +235,15 @@
 Troubleshooting issues with the USGS network
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 SSL-related error messages when using conda
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 (with ``SSL`` mentioned in the message and possibly ``bad handshake``)
 
-Make sure that the ``conda`` package installer is configured to use the USGS certificate
+Make sure that the ``Conda`` package installer is configured to use the USGS certificate
 (see :ref:`Installing the DOI SSL certificate for use with conda` above).
 
 
 SSL-related error messages when using pip
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 (something similar to ``SSL: CERTIFICATE_VERIFY_FAILED``).
 
@@ -238,15 +269,15 @@
 
 This tells conda to fetch ``m2w64-gettext`` from the ``msys2`` channel instead. Note that this is only a dependency on Windows,
 so it needs to be commented out on other operating systems (normally it wouldn't need to be listed, but the above HTTP 500 error indicates that installation from the default source location failed.)
 
 
 .. _Anaconda python distribution: https://www.anaconda.com/distribution/
 .. _clean uninstall: https://docs.anaconda.com/anaconda/install/uninstall/
-.. _conda: https://docs.conda.io/en/latest/
+.. _Conda: https://docs.conda.io/en/latest/
 .. _Mamba: https://mamba.readthedocs.io/en/latest/
 .. _conda environment: https://docs.conda.io/projects/conda/en/latest/user-guide/concepts/environments.html
 .. _conda-pack: https://conda.github.io/conda-pack/
 .. _condarc: https://docs.conda.io/projects/conda/en/latest/user-guide/configuration/use-condarc.html
 .. _download: https://github.com/aleaf/sfrmaker/archive/master.zip
 .. _gis.yml: https://raw.githubusercontent.com/aleaf/sfrmaker/master/gis.yml
 .. _pip: https://packaging.python.org/tutorials/installing-packages/#use-pip-for-installing
```

### Comparing `sfrmaker-0.9.3/docs/source/philosophy.rst` & `sfrmaker-0.9.4/docs/source/philosophy.rst`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/docs/source/references.rst` & `sfrmaker-0.9.4/docs/source/references.rst`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/docs/source/release-history.rst` & `sfrmaker-0.9.4/docs/source/release-history.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 ===============
 Release History
 ===============
 
+Version 0.9.4 (2023-01-19)
+--------------------------
+* add ability drop NHDPlus High Resolution segments by ftype (e.g., 428) and NHDPlusID, similar to the "drop_fcodes" option in the ``from_nhdplus_hr()`` method.
+* fix issue where the crs argument for pyproj CRS-style coordinate references wasn't being passed to the base grid class; get the crs from a Flopy-style grid if it exists.
+* updates to the install instructions, concerning Mamba and IPython kernels
+
 Version 0.9.3 (2022-12-19)
 --------------------------
 * fixes to ``SFRdata.assign_layers``:
     * only compare new cell bottoms to old cell bottoms if a new bottom array is returned
     * when using idomain/ibound to set reach layers, recast array to boolean array of inactive/active cells, otherwise the ``np.argmax`` approach for finding the lowest active layer might identify the wrong layer (if ibound or idomain has values > 1). 
     * bug in file naming for revised bottom arrays (all arrays were previously named using the bottom layer).
 * fixes to ``Lines`` class:
```

### Comparing `sfrmaker-0.9.3/docs/source/troubleshooting.rst` & `sfrmaker-0.9.4/docs/source/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/setup.py` & `sfrmaker-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/base.py` & `sfrmaker-0.9.4/sfrmaker/base.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/checks.py` & `sfrmaker-0.9.4/sfrmaker/checks.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/elevations.py` & `sfrmaker-0.9.4/sfrmaker/elevations.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/fileio.py` & `sfrmaker-0.9.4/sfrmaker/fileio.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/flows.py` & `sfrmaker-0.9.4/sfrmaker/flows.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/gis.py` & `sfrmaker-0.9.4/sfrmaker/gis.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/grid.py` & `sfrmaker-0.9.4/sfrmaker/grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,19 +278,19 @@
     _structured = True
 
     def __init__(self, df,
                  xul=None, yul=None, dx=None, dy=None, rotation=0.,
                  uniform=None,
                  model_units='undefined', crs_units=None,
                  bounds=None, active_area=None,
-                 epsg=None, proj_str=None, prjfile=None, **kwargs):
+                 crs=None, epsg=None, proj_str=None, prjfile=None, **kwargs):
 
         Grid.__init__(self, df, model_units=model_units, crs_units=crs_units,
                       bounds=bounds, active_area=active_area,
-                      epsg=epsg, proj_str=proj_str, prjfile=prjfile, **kwargs)
+                      crs=crs, epsg=epsg, proj_str=proj_str, prjfile=prjfile, **kwargs)
 
         # structured grid parameters
         self.xul = xul
         self.yul = yul
         self.rotation = rotation
         self.nrow = self.df.i.max() + 1
         self.ncol = self.df.j.max() + 1
@@ -376,14 +376,17 @@
                            'i': sorted(list(range(mg.nrow)) * mg.ncol),
                            'j': list(range(mg.ncol)) * mg.nrow,
                            'geometry': polygons
                            }, columns=['node', 'i', 'j', 'geometry'])
         if epsg is None:
             epsg = mg.epsg
         crs = get_crs(prjfile=prjfile, epsg=epsg, proj_str=mg.proj4, crs=crs)
+        # get the crs from the model grid if it wasn't supplied
+        if crs is None and hasattr(mg, 'crs'):
+            crs = mg.crs
 
         if isfr is not None:
             # if a 3D array is supplied for isfr, convert to 2D
             # (retain all i, j locations with at least one active layer;
             # assuming that top of each highest-active cell represents the land surface)
             if len(isfr.shape) == 3:
                 isfr = np.any(isfr == 1, axis=0).astype(int)
```

### Comparing `sfrmaker-0.9.3/sfrmaker/lines.py` & `sfrmaker-0.9.4/sfrmaker/lines.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,22 +90,21 @@
 
     @property
     def geometry_length_units(self):
         """Length units of reach LineString geometries.
         """
         valid_units = {'feet': 'feet',
                        'foot': 'feet',
-                       'us-ft': 'feet',
                        'meters': 'meters',
-                       'meter': 'meters'}
+                       'metre': 'meters'}
         self._geometry_length_units = valid_units.get(self.crs.axis_info[0].unit_name)
         if self._geometry_length_units is None:
             print("Warning: No length units specified in CRS for input LineStrings "
-                  "or length units not recognized. "
-                  "Defaulting to meters.")
+                  "or length units not recognized"
+                  "defaulting to meters.")
             self._geometry_length_units = 'meters'
         return self._geometry_length_units
 
     @property
     def routing(self):
         """Dictionary of routing connections from ids (keys)
         to to_ids (values).
@@ -667,15 +666,15 @@
                                   name_column='GNIS_NAME',
                                   attr_length_units='meters',
                                   attr_height_units='meters',
                                   epsg=epsg, proj_str=proj_str, prjfile=prjfile)
 
     @classmethod
     def from_nhdplus_hr(cls, NHDPlusHR_paths, filter=None, 
-                        drop_fcodes=None, crs=None, 
+                        drop_fcodes=None, drop_ftypes=None, drop_NHDPlusIDs=None, crs=None,
                         epsg=None, proj_str=None):
         """
         Parameters
         ==========
         NHDPlusHR_paths : str or list of strings
             path (or list of paths) to the NHDPlus High Resolution HU-4 Subregion 
             file geodatabase (.gdb) to include, assuming the file structure is 
@@ -690,15 +689,21 @@
             Bounding box (tuple) or shapefile of model stream network area.
         drop_fcodes : int or list of ints, optional
             fcode or list of NHDFlowline FCodes to drop from network. 
             For example, to remove underground aqueducts and general case
             water pipelines from line network::
                 
                 drop_fcodes = [42803, 42814]
-                
+        drop_ftypes : int or list of ints, optional
+            List of NHDFlowline FTypes to drop from network.
+            For example, to remove all pipelines from line network::
+
+                drop_fcodes = [428]
+        drop_NHDPlusIDs : int or list of ints, optional
+            List of NHDFlowlines (as NHDPlusIDs) to drop from network.
         crs : obj, optional
             Coordinate reference object to reproject NHDPlus High Resolution 
             flowlines. A Python int, dict, str, or :class:`pyproj.crs.CRS` 
             instance passed to :meth:`pyproj.crs.CRS.from_user_input`
             Can be any of:
             - PROJ string
             - Dictionary of PROJ parameters
@@ -718,15 +723,16 @@
             proj_str string to to reproject NHDPlus High Resolution flowlines.
             By default, None, will use NHDPlus HR fileGDB CRS 
 
         Returns
         ==========
         lines : :class:`Lines` instance
         """
-        df, gdb_crs = load_nhdplus_hr(NHDPlusHR_paths, filter = filter, drop_fcodes=drop_fcodes)
+        df, gdb_crs = load_nhdplus_hr(NHDPlusHR_paths, filter=filter, drop_fcodes=drop_fcodes, 
+                                      drop_ftypes=drop_ftypes, drop_NHDPlusIDs=drop_NHDPlusIDs)
 
         #  check to see if flowline geodataframe needs to be reprojected, and get new CRS
         if crs is not None or epsg is not None or proj_str is not None:
             if crs is not None:
                 crs = get_authority_crs(crs)
             if epsg is not None:
                 if crs is None:
@@ -847,15 +853,15 @@
         print("\nCreating sfr dataset...")
         totim = time.time()
 
         if flopy and active_area is None and isfr is None and model is not None:
             if model.version == 'mf6':
                 isfr = np.sum(model.dis.idomain.array > 0, axis=0) > 0
             else:
-                isfr = np.sum(model.bas6.ibound.array > 0, axis=0) > 0
+                isfr = np.sum(model.bas6.ibound.array == 1, axis=0) > 0
         if flopy and isinstance(grid, flopy.discretization.StructuredGrid):
             print('\nCreating grid class instance from flopy Grid instance...')
             ta = time.time()
             grid = StructuredGrid.from_modelgrid(grid, active_area=active_area, isfr=isfr)
             print("grid class created in {:.2f}s\n".format(time.time() - ta))
         elif flopy and model is not None:
             grid = StructuredGrid.from_modelgrid(model.modelgrid, active_area=active_area, isfr=isfr)
```

### Comparing `sfrmaker-0.9.3/sfrmaker/logger.py` & `sfrmaker-0.9.4/sfrmaker/logger.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/mf5to6.py` & `sfrmaker-0.9.4/sfrmaker/mf5to6.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/nhdplus_utils.py` & `sfrmaker-0.9.4/sfrmaker/nhdplus_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -276,28 +276,32 @@
                                pf.loc[pf.Divergence_ToNHDPID != 2, 'ToNHDPID']))
     
     print("finished in {:.2f}s\n".format(time.time() - ta))
     return pf_routing_dict
 
 
 def load_nhdplus_hr(NHDPlusHR_paths, filter=None, 
-                    drop_fcodes=None):
+                    drop_fcodes=None, drop_ftypes=None, drop_NHDPlusIDs=None):
     """
     Parameters
     ==========
     NHDPlusHR_paths : path (or list of paths) to the NHDPlus High Resolution HU-4 
         Subregion  file geodatabase (.gdb) to include, assuming the file structure 
         is the same as when downloaded from the USGS National Map Downloader tool 
         (v2.0) website (https://apps.nationalmap.gov/downloader/#/).
     filter : tuple, str (filepath), shapely Polygon or GeoJSON polygon
         Bounding box (tuple) or polygon feature of model stream network area.
         Shapefiles will be reprojected to the CRS of the flowlines; all other
         feature types must be supplied in same CRS as flowlines.
     drop_fcodes: int or list of ints, optional
             fcode or list of NHDFlowline FCodes to drop from network. 
+    drop_ftypes: int or list of ints, optional
+            ftype or list of NHDFlowline Ftypes to drop from network. 
+    drop_NHDPlusIDs: int or list of ints, optional
+            NHDPlusID or list of NHDFlowline NHDPlusIDs to drop from network. 
     crs : obj
         Coordinate reference system of the NHDPlus data. Only needed if
         the data do not have a valid ESRI projection (.prj) file.
         A Python int, dict, str, or :class:`pyproj.crs.CRS` instance
         passed to :meth:`pyproj.crs.CRS.from_user_input`
 
         Can be any of:
@@ -345,14 +349,18 @@
         df = read_nhdplus_hr(NHDPlusHR_paths, filter = filter)
         #  get OpenFileGDB crs
         crs = df.crs
    
     #  Option to drop specified FCodes
     if drop_fcodes is not None:    
         df = df.loc[~df.FCode.isin(drop_fcodes)]
+    if drop_ftypes is not None:
+        df = df.loc[~df.FType.isin(drop_ftypes)]
+    if drop_NHDPlusIDs is not None:
+        df = df.loc[~df.NHDPlusID.isin(drop_NHDPlusIDs)]
         
     keep_cols = ['NHDPlusID', 'ToNHDPID', 'ArbolateSu',
                'geometry', 'StreamOrde',
                'MaxElevSmo', 'MinElevSmo', 'GNIS_Name']
     
     #  Make final dataframe with only the info needed for lines
     df = df[keep_cols].copy()
```

### Comparing `sfrmaker-0.9.3/sfrmaker/observations.py` & `sfrmaker-0.9.4/sfrmaker/observations.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/preprocessing.py` & `sfrmaker-0.9.4/sfrmaker/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/reaches.py` & `sfrmaker-0.9.4/sfrmaker/reaches.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/rivdata.py` & `sfrmaker-0.9.4/sfrmaker/rivdata.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/routing.py` & `sfrmaker-0.9.4/sfrmaker/routing.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/sfrdata.py` & `sfrmaker-0.9.4/sfrmaker/sfrdata.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/test/conftest.py` & `sfrmaker-0.9.4/sfrmaker/test/conftest.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/test/test_data.py` & `sfrmaker-0.9.4/sfrmaker/test/test_data.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/test/test_examples.py` & `sfrmaker-0.9.4/sfrmaker/test/test_examples.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/test/test_flows.py` & `sfrmaker-0.9.4/sfrmaker/test/test_flows.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/test/test_from_nhdplus.py` & `sfrmaker-0.9.4/sfrmaker/test/test_from_nhdplus.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/test/test_from_yaml.py` & `sfrmaker-0.9.4/sfrmaker/test/test_from_yaml.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/test/test_gis.py` & `sfrmaker-0.9.4/sfrmaker/test/test_gis.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/test/test_grid.py` & `sfrmaker-0.9.4/sfrmaker/test/test_grid.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/test/test_lines.py` & `sfrmaker-0.9.4/sfrmaker/test/test_lines.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,10 +54,28 @@
     outshp = test_data_path / 'lines.shp'
     lines.write_shapefile(outshp)
     assert outshp.exists()
 
 
 @pytest.mark.skipif(platform.system() == 'Linux', reason="Fiona FileGDB driver error")
 def test_load_nhdplus_hr(neversink_lines_from_nhdplus_hr):
+    
     lines = neversink_lines_from_nhdplus_hr
     assert isinstance(lines, sfrmaker.lines.Lines)
-    assert is_to_one(lines._original_routing)
+    assert is_to_one(lines._original_routing)
+
+
+@pytest.mark.skipif(platform.system() == 'Linux', reason="Fiona FileGDB driver error")
+@pytest.mark.parametrize('kwargs', (
+    {'drop_ftypes': [428], 'drop_NHDPlusIDs': [10000200240966]},
+))
+def test_load_nhdplus_hr_options(datapath, kwargs):
+    NHDPlusHR_paths = [f'{datapath}/neversink_rondout/NHDPLUS_HR_1.gdb', 
+                       f'{datapath}/neversink_rondout/NHDPLUS_HR_2.gdb']
+    boundary_file = f'{datapath}/neversink_rondout/Model_Extent.shp'
+
+    lns = sfrmaker.Lines.from_nhdplus_hr(NHDPlusHR_paths,
+                                        filter=boundary_file,
+                                        **kwargs)
+    assert not any(set(lns.df.id).intersection(kwargs['drop_NHDPlusIDs']))
+    # these two NHDPlusIDs have FType == 428
+    assert not any(set(lns.df.id).intersection([10000700047982, 10000200046339]))
```

### Comparing `sfrmaker-0.9.3/sfrmaker/test/test_logger.py` & `sfrmaker-0.9.4/sfrmaker/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/test/test_map.py` & `sfrmaker-0.9.4/sfrmaker/test/test_map.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/test/test_mf5to6.py` & `sfrmaker-0.9.4/sfrmaker/test/test_mf5to6.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/test/test_notebooks.py` & `sfrmaker-0.9.4/sfrmaker/test/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/test/test_observations.py` & `sfrmaker-0.9.4/sfrmaker/test/test_observations.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/test/test_preprocessing.py` & `sfrmaker-0.9.4/sfrmaker/test/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/test/test_routing.py` & `sfrmaker-0.9.4/sfrmaker/test/test_routing.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/test/test_sfr_data.py` & `sfrmaker-0.9.4/sfrmaker/test/test_sfr_data.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/test/test_units.py` & `sfrmaker-0.9.4/sfrmaker/test/test_units.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/test/test_utils.py` & `sfrmaker-0.9.4/sfrmaker/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/test/test_version.py` & `sfrmaker-0.9.4/sfrmaker/test/test_version.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/units.py` & `sfrmaker-0.9.4/sfrmaker/units.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker/utils.py` & `sfrmaker-0.9.4/sfrmaker/utils.py`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/sfrmaker.egg-info/PKG-INFO` & `sfrmaker-0.9.4/sfrmaker.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfrmaker
-Version: 0.9.3
+Version: 0.9.4
 Summary: Python package for rapid creation of streamflow routing networks.
 Home-page: https://github.com/aleaf/sfrmaker
 Author: USGS
 Author-email: aleaf@usgs.gov
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `sfrmaker-0.9.3/sfrmaker.egg-info/SOURCES.txt` & `sfrmaker-0.9.4/sfrmaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sfrmaker-0.9.3/versioneer.py` & `sfrmaker-0.9.4/versioneer.py`

 * *Files identical despite different names*

