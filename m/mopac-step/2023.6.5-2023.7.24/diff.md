# Comparing `tmp/mopac_step-2023.6.5.tar.gz` & `tmp/mopac_step-2023.7.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mopac_step-2023.6.5.tar", last modified: Mon Jun  5 16:48:24 2023, max compression
+gzip compressed data, was "mopac_step-2023.7.24.tar", last modified: Tue Jul 25 20:14:13 2023, max compression
```

## Comparing `mopac_step-2023.6.5.tar` & `mopac_step-2023.7.24.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:48:24.362433 mopac_step-2023.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-06-05 16:48:24.362433 mopac_step-2023.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:48:24.350433 mopac_step-2023.6.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:48:24.354433 mopac_step-2023.6.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/docs/_static/SEAMM inverted.png
--rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:48:24.354433 mopac_step-2023.6.5/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9525 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:48:24.354433 mopac_step-2023.6.5/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:48:24.354433 mopac_step-2023.6.5/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:48:24.354433 mopac_step-2023.6.5/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/docs/user_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:48:24.362433 mopac_step-2023.6.5/mopac_step/
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-05 16:48:24.362433 mopac_step-2023.6.5/mopac_step/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:48:24.362433 mopac_step-2023.6.5/mopac_step/data/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/data/configuration.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/data/properties.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24413 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/data/references.bib
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/data/seamm-mopac.yml
--rw-r--r--   0 runner    (1001) docker     (123)    37841 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/energy_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/energy_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    19662 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/forceconstants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/forceconstants_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/forceconstants_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/installer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9835 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/ir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/ir_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/ir_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    17652 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/lewis_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/lewis_structure_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/lewis_structure_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    62194 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    14081 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/mopac.py
--rw-r--r--   0 runner    (1001) docker     (123)    10627 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/mopac_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/mopac_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/optimization_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/optimization_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    11972 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/thermodynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/thermodynamics_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/thermodynamics_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/tk_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/tk_forceconstants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/tk_ir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/tk_lewis_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/tk_mopac.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/tk_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/mopac_step/tk_thermodynamics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:48:24.362433 mopac_step-2023.6.5/mopac_step.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-06-05 16:48:24.000000 mopac_step-2023.6.5/mopac_step.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-05 16:48:24.000000 mopac_step-2023.6.5/mopac_step.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:48:24.000000 mopac_step-2023.6.5/mopac_step.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-05 16:48:24.000000 mopac_step-2023.6.5/mopac_step.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-05 16:48:24.000000 mopac_step-2023.6.5/mopac_step.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-05 16:48:24.000000 mopac_step-2023.6.5/mopac_step.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:48:09.000000 mopac_step-2023.6.5/mopac_step.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-05 16:48:24.362433 mopac_step-2023.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:48:24.362433 mopac_step-2023.6.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/tests/test_mopac_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-05 16:48:05.000000 mopac_step-2023.6.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:14:13.569137 mopac_step-2023.7.24/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-07-25 20:14:13.569137 mopac_step-2023.7.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:14:13.561137 mopac_step-2023.7.24/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:14:13.561137 mopac_step-2023.7.24/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/_static/SEAMM inverted.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:14:13.561137 mopac_step-2023.7.24/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9525 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:14:13.561137 mopac_step-2023.7.24/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:14:13.561137 mopac_step-2023.7.24/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:14:13.561137 mopac_step-2023.7.24/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/docs/user_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:14:13.569137 mopac_step-2023.7.24/mopac_step/
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-25 20:14:13.569137 mopac_step-2023.7.24/mopac_step/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:14:13.569137 mopac_step-2023.7.24/mopac_step/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/data/configuration.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/data/properties.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24413 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/data/references.bib
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/data/seamm-mopac.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    37841 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/energy_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/energy_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19662 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/forceconstants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/forceconstants_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/forceconstants_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9835 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/ir_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/ir_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17652 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/lewis_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/lewis_structure_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/lewis_structure_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62194 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14081 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/mopac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10627 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/mopac_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/mopac_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/optimization_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/optimization_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11972 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/thermodynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/thermodynamics_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/thermodynamics_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/tk_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/tk_forceconstants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/tk_ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/tk_lewis_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/tk_mopac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/tk_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/mopac_step/tk_thermodynamics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:14:13.565137 mopac_step-2023.7.24/mopac_step.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-07-25 20:14:13.000000 mopac_step-2023.7.24/mopac_step.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-25 20:14:13.000000 mopac_step-2023.7.24/mopac_step.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 20:14:13.000000 mopac_step-2023.7.24/mopac_step.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-25 20:14:13.000000 mopac_step-2023.7.24/mopac_step.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-25 20:14:13.000000 mopac_step-2023.7.24/mopac_step.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-25 20:14:13.000000 mopac_step-2023.7.24/mopac_step.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 20:13:57.000000 mopac_step-2023.7.24/mopac_step.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-25 20:14:13.569137 mopac_step-2023.7.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:14:13.569137 mopac_step-2023.7.24/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/tests/test_mopac_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-25 20:13:52.000000 mopac_step-2023.7.24/versioneer.py
```

### Comparing `mopac_step-2023.6.5/CONTRIBUTING.rst` & `mopac_step-2023.7.24/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/HISTORY.rst` & `mopac_step-2023.7.24/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 =======
 History
 =======
+2023.7.24 -- Bugfix in Lewis structure with bond orders
+  * Major issue in getting the bonds from the Lewis structure where the atoms and bond
+    orders were mixed up.
+    
 2023.6.5 -- Bugfix working around MOPAC problem
   * MOPAC is not consistent about putting end of file and end of program markers in the
     AUX file. This caused carashed in SEAMM, which this fixes until MOPAC can be
     corrected.
     
 2023.4.24 -- Bugfixes for Lewis structure
   * Correctly handle periodic systems in Lewis structure.
```

### Comparing `mopac_step-2023.6.5/LICENSE` & `mopac_step-2023.7.24/LICENSE`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/PKG-INFO` & `mopac_step-2023.7.24/mopac_step.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mopac_step
-Version: 2023.6.5
+Name: mopac-step
+Version: 2023.7.24
 Summary: A SEAMM plug-in to setup, run and analyze semiempirical calculations with MOPAC
 Home-page: https://github.com/molssi-seam/mopac_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,forcefield,MOPAC,semiempirical,orbitals
 Platform: Linux
@@ -89,14 +89,18 @@
 .. _MolSSI: https://www.molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2023.7.24 -- Bugfix in Lewis structure with bond orders
+  * Major issue in getting the bonds from the Lewis structure where the atoms and bond
+    orders were mixed up.
+    
 2023.6.5 -- Bugfix working around MOPAC problem
   * MOPAC is not consistent about putting end of file and end of program markers in the
     AUX file. This caused carashed in SEAMM, which this fixes until MOPAC can be
     corrected.
     
 2023.4.24 -- Bugfixes for Lewis structure
   * Correctly handle periodic systems in Lewis structure.
```

### Comparing `mopac_step-2023.6.5/README.rst` & `mopac_step-2023.7.24/README.rst`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/docs/Makefile` & `mopac_step-2023.7.24/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/docs/_static/SEAMM inverted.png` & `mopac_step-2023.7.24/docs/_static/SEAMM inverted.png`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/docs/_static/SEAMM logo.png` & `mopac_step-2023.7.24/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/docs/_static/molssi_main_logo.png` & `mopac_step-2023.7.24/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/docs/_static/molssi_main_logo_inverted_white.png` & `mopac_step-2023.7.24/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/docs/_static/molssi_square.png` & `mopac_step-2023.7.24/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/docs/_static/nsf.png` & `mopac_step-2023.7.24/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/docs/conf.py` & `mopac_step-2023.7.24/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/docs/developer_guide/installation.rst` & `mopac_step-2023.7.24/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/docs/getting_started/index.rst` & `mopac_step-2023.7.24/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/docs/index.rst` & `mopac_step-2023.7.24/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/docs/make.bat` & `mopac_step-2023.7.24/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/__init__.py` & `mopac_step-2023.7.24/mopac_step/__init__.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/data/configuration.txt` & `mopac_step-2023.7.24/mopac_step/data/configuration.txt`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/data/properties.csv` & `mopac_step-2023.7.24/mopac_step/data/properties.csv`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/data/references.bib` & `mopac_step-2023.7.24/mopac_step/data/references.bib`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/energy.py` & `mopac_step-2023.7.24/mopac_step/energy.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/energy_parameters.py` & `mopac_step-2023.7.24/mopac_step/energy_parameters.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/energy_step.py` & `mopac_step-2023.7.24/mopac_step/energy_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/forceconstants.py` & `mopac_step-2023.7.24/mopac_step/forceconstants.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/forceconstants_parameters.py` & `mopac_step-2023.7.24/mopac_step/forceconstants_parameters.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/forceconstants_step.py` & `mopac_step-2023.7.24/mopac_step/forceconstants_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/installer.py` & `mopac_step-2023.7.24/mopac_step/installer.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/ir.py` & `mopac_step-2023.7.24/mopac_step/ir.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/ir_parameters.py` & `mopac_step-2023.7.24/mopac_step/ir_parameters.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/ir_step.py` & `mopac_step-2023.7.24/mopac_step/ir_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/lewis_structure.py` & `mopac_step-2023.7.24/mopac_step/lewis_structure.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -440,37 +440,37 @@
             text += tmp
             text += "\n"
 
         # If requested, overwrite the bonding information in the system
         if P["use bonds"]:
             ids = configuration.atoms.ids
             if same:
+                iatoms = [ids[i] for i in bonds["i"]]
+                jatoms = [ids[j] for j in bonds["j"]]
+                configuration.bonds.delete()
+                configuration.bonds.append(
+                    i=iatoms, j=jatoms, bondorder=bonds["bondorder"]
+                )
+                text += "\nReplaced the bonds in the configuration with those from the "
+                text += "Lewis structure.\n"
+            else:
                 iatoms = []
                 jatoms = []
                 bondorders = []
                 for i in range(n_atoms):
                     for j in lneighbors[i]:
                         if j > i:
                             iatoms.append(ids[i])
                             jatoms.append(ids[j])
                             bondorders.append(1)
                 configuration.bonds.delete()
                 configuration.bonds.append(
                     i=iatoms, j=jatoms, bondorder=bonds["bondorder"]
                 )
                 text += "\nReplaced the bonds in the configuration with those from the "
-                text += "Lewis structure.\n"
-            else:
-                iatoms = [ids[i] for i in bonds["i"]]
-                jatoms = [ids[j] for j in bonds["j"]]
-                configuration.bonds.delete()
-                configuration.bonds.append(
-                    i=iatoms, j=jatoms, bondorder=bonds["bondorder"]
-                )
-                text += "\nReplaced the bonds in the configuration with those from the "
                 text += "simple connectivity structure.\n"
 
         # Put any requested results into variables or tables
         self.store_results(
             configuration=configuration,
             data=data,
         )
```

### Comparing `mopac_step-2023.6.5/mopac_step/lewis_structure_parameters.py` & `mopac_step-2023.7.24/mopac_step/lewis_structure_parameters.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/lewis_structure_step.py` & `mopac_step-2023.7.24/mopac_step/lewis_structure_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/metadata.py` & `mopac_step-2023.7.24/mopac_step/metadata.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/mopac.py` & `mopac_step-2023.7.24/mopac_step/mopac.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/mopac_base.py` & `mopac_step-2023.7.24/mopac_step/mopac_base.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/mopac_step.py` & `mopac_step-2023.7.24/mopac_step/mopac_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/optimization.py` & `mopac_step-2023.7.24/mopac_step/optimization.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/optimization_parameters.py` & `mopac_step-2023.7.24/mopac_step/optimization_parameters.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/optimization_step.py` & `mopac_step-2023.7.24/mopac_step/optimization_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/thermodynamics.py` & `mopac_step-2023.7.24/mopac_step/thermodynamics.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/thermodynamics_parameters.py` & `mopac_step-2023.7.24/mopac_step/thermodynamics_parameters.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/thermodynamics_step.py` & `mopac_step-2023.7.24/mopac_step/thermodynamics_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/tk_energy.py` & `mopac_step-2023.7.24/mopac_step/tk_energy.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/tk_forceconstants.py` & `mopac_step-2023.7.24/mopac_step/tk_forceconstants.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/tk_ir.py` & `mopac_step-2023.7.24/mopac_step/tk_ir.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/tk_lewis_structure.py` & `mopac_step-2023.7.24/mopac_step/tk_lewis_structure.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/tk_mopac.py` & `mopac_step-2023.7.24/mopac_step/tk_mopac.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/tk_optimization.py` & `mopac_step-2023.7.24/mopac_step/tk_optimization.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step/tk_thermodynamics.py` & `mopac_step-2023.7.24/mopac_step/tk_thermodynamics.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step.egg-info/PKG-INFO` & `mopac_step-2023.7.24/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mopac-step
-Version: 2023.6.5
+Name: mopac_step
+Version: 2023.7.24
 Summary: A SEAMM plug-in to setup, run and analyze semiempirical calculations with MOPAC
 Home-page: https://github.com/molssi-seam/mopac_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,forcefield,MOPAC,semiempirical,orbitals
 Platform: Linux
@@ -89,14 +89,18 @@
 .. _MolSSI: https://www.molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2023.7.24 -- Bugfix in Lewis structure with bond orders
+  * Major issue in getting the bonds from the Lewis structure where the atoms and bond
+    orders were mixed up.
+    
 2023.6.5 -- Bugfix working around MOPAC problem
   * MOPAC is not consistent about putting end of file and end of program markers in the
     AUX file. This caused carashed in SEAMM, which this fixes until MOPAC can be
     corrected.
     
 2023.4.24 -- Bugfixes for Lewis structure
   * Correctly handle periodic systems in Lewis structure.
```

### Comparing `mopac_step-2023.6.5/mopac_step.egg-info/SOURCES.txt` & `mopac_step-2023.7.24/mopac_step.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/mopac_step.egg-info/entry_points.txt` & `mopac_step-2023.7.24/mopac_step.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/setup.py` & `mopac_step-2023.7.24/setup.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/tests/test_mopac_step.py` & `mopac_step-2023.7.24/tests/test_mopac_step.py`

 * *Files identical despite different names*

### Comparing `mopac_step-2023.6.5/versioneer.py` & `mopac_step-2023.7.24/versioneer.py`

 * *Files identical despite different names*

