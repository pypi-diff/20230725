# Comparing `tmp/clover-energy-5.1.0.post1.tar.gz` & `tmp/clover-energy-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/bewinche/modelling/CLOVER/dist/.tmp-fbxeilbo/clover-energy-5.1.0.post1.tar", last modified: Tue Jul 18 10:30:49 2023, max compression
+gzip compressed data, was "/home/bewinche/modelling/CLOVER/dist/.tmp-uu0k8rq_/clover-energy-5.1.1.tar", last modified: Tue Jul 25 13:19:21 2023, max compression
```

## Comparing `clover-energy-5.1.0.post1.tar` & `clover-energy-5.1.1.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:49.000000 clover-energy-5.1.0.post1/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1080 2023-06-30 07:49:00.000000 clover-energy-5.1.0.post1/LICENSE
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)       47 2023-06-30 07:49:00.000000 clover-energy-5.1.0.post1/MANIFEST.in
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    16579 2023-07-18 10:30:49.000000 clover-energy-5.1.0.post1/PKG-INFO
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    15933 2023-07-17 10:28:59.000000 clover-energy-5.1.0.post1/README.md
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      103 2023-06-30 07:49:00.000000 clover-energy-5.1.0.post1/pyproject.toml
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1302 2023-07-18 10:30:49.000000 clover-energy-5.1.0.post1/setup.cfg
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     2049 2023-07-17 10:09:36.000000 clover-energy-5.1.0.post1/src/clover/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    51541 2023-07-18 10:23:54.000000 clover-energy-5.1.0.post1/src/clover/__main__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    97316 2023-07-18 09:54:23.000000 clover-energy-5.1.0.post1/src/clover/__utils__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    36718 2023-07-18 09:54:23.000000 clover-energy-5.1.0.post1/src/clover/analysis.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     8512 2023-07-18 09:54:23.000000 clover-energy-5.1.0.post1/src/clover/argparser.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover/conversion/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      710 2023-07-17 10:09:36.000000 clover-energy-5.1.0.post1/src/clover/conversion/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    26993 2023-07-17 10:28:59.000000 clover-energy-5.1.0.post1/src/clover/conversion/conversion.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover/conversion/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/conversion/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover/conversion/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/conversion/tests/unit/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)   107239 2023-07-18 09:54:23.000000 clover-energy-5.1.0.post1/src/clover/fileparser.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover/generation/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/generation/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    20730 2023-07-18 09:54:23.000000 clover-energy-5.1.0.post1/src/clover/generation/__utils__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    27727 2023-07-18 09:54:23.000000 clover-energy-5.1.0.post1/src/clover/generation/solar.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover/generation/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/generation/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover/generation/tests/component/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/generation/tests/component/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover/generation/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/generation/tests/unit/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4554 2023-07-18 09:54:23.000000 clover-energy-5.1.0.post1/src/clover/generation/weather.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     3563 2023-07-18 09:54:23.000000 clover-energy-5.1.0.post1/src/clover/generation/wind.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover/impact/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1141 2023-07-17 10:09:36.000000 clover-energy-5.1.0.post1/src/clover/impact/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4199 2023-07-17 10:28:59.000000 clover-energy-5.1.0.post1/src/clover/impact/__utils__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    44572 2023-07-18 09:54:23.000000 clover-energy-5.1.0.post1/src/clover/impact/finance.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    31219 2023-07-18 09:54:23.000000 clover-energy-5.1.0.post1/src/clover/impact/ghgs.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover/impact/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/impact/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover/impact/tests/component/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/impact/tests/component/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover/impact/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/impact/tests/unit/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover/load/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      931 2023-07-17 10:09:36.000000 clover-energy-5.1.0.post1/src/clover/load/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    39767 2023-07-17 10:28:59.000000 clover-energy-5.1.0.post1/src/clover/load/load.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover/load/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/load/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover/load/tests/component/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/load/tests/component/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover/mains_supply/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      774 2023-07-17 10:09:36.000000 clover-energy-5.1.0.post1/src/clover/mains_supply/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4473 2023-07-11 16:32:53.000000 clover-energy-5.1.0.post1/src/clover/mains_supply/__utils__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4578 2023-07-11 16:32:53.000000 clover-energy-5.1.0.post1/src/clover/mains_supply/grid.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover/mains_supply/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/mains_supply/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover/mains_supply/tests/component/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/mains_supply/tests/component/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover/mains_supply/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/mains_supply/tests/unit/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    11741 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/mains_supply/water_source.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover/optimisation/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1069 2023-07-17 10:09:36.000000 clover-energy-5.1.0.post1/src/clover/optimisation/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    43348 2023-07-18 10:01:36.000000 clover-energy-5.1.0.post1/src/clover/optimisation/__utils__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    29385 2023-07-18 09:54:23.000000 clover-energy-5.1.0.post1/src/clover/optimisation/appraisal.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    64706 2023-07-18 09:54:23.000000 clover-energy-5.1.0.post1/src/clover/optimisation/optimisation.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    43556 2023-07-18 09:54:23.000000 clover-energy-5.1.0.post1/src/clover/optimisation/single_line_simulation.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover/optimisation/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/optimisation/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover/optimisation/tests/component/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/optimisation/tests/component/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover/optimisation/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/optimisation/tests/unit/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     8754 2023-07-18 09:54:23.000000 clover-energy-5.1.0.post1/src/clover/printer.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover/scripts/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/scripts/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1309 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/scripts/clover.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1202 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/scripts/clover_hpc_clover.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1298 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/scripts/clover_hpc_outbox_assembly.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1138 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/scripts/clover_new_location.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1360 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/scripts/clover_update_api_token.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     6682 2023-07-17 10:09:36.000000 clover-energy-5.1.0.post1/src/clover/scripts/hpc.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    10191 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/scripts/hpc_clover.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4894 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/scripts/hpc_outbox_assembly.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    22944 2023-07-17 10:09:36.000000 clover-energy-5.1.0.post1/src/clover/scripts/hpc_utils.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    11904 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/scripts/new_location.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover/scripts/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/scripts/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover/scripts/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/scripts/tests/unit/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     3638 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/scripts/update_api_token.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:49.000000 clover-energy-5.1.0.post1/src/clover/simulation/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1199 2023-07-17 10:09:36.000000 clover-energy-5.1.0.post1/src/clover/simulation/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    21928 2023-07-18 09:54:23.000000 clover-energy-5.1.0.post1/src/clover/simulation/__utils__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    12992 2023-07-17 10:28:59.000000 clover-energy-5.1.0.post1/src/clover/simulation/diesel.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    88978 2023-07-18 09:54:23.000000 clover-energy-5.1.0.post1/src/clover/simulation/energy_system.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     2450 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/simulation/exchanger.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    24234 2023-07-17 10:28:59.000000 clover-energy-5.1.0.post1/src/clover/simulation/solar.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    31852 2023-07-18 09:54:23.000000 clover-energy-5.1.0.post1/src/clover/simulation/storage.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    19002 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/simulation/storage_utils.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:49.000000 clover-energy-5.1.0.post1/src/clover/simulation/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/simulation/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:49.000000 clover-energy-5.1.0.post1/src/clover/simulation/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/simulation/tests/unit/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     5411 2023-07-11 16:48:20.000000 clover-energy-5.1.0.post1/src/clover/simulation/transmission.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:49.000000 clover-energy-5.1.0.post1/src/clover/src/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/src/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    56900 2023-07-17 10:28:59.000000 clover-energy-5.1.0.post1/src/clover/src/new_location.yaml
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:49.000000 clover-energy-5.1.0.post1/src/clover/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:49.000000 clover-energy-5.1.0.post1/src/clover/tests/integration/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.0.post1/src/clover/tests/integration/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:49.000000 clover-energy-5.1.0.post1/src/clover/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:49:00.000000 clover-energy-5.1.0.post1/src/clover/tests/unit/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-18 10:30:49.000000 clover-energy-5.1.0.post1/src/clover_energy.egg-info/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    16579 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover_energy.egg-info/PKG-INFO
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     3003 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover_energy.egg-info/SOURCES.txt
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)        1 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover_energy.egg-info/dependency_links.txt
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      299 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover_energy.egg-info/entry_points.txt
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      119 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover_energy.egg-info/requires.txt
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)        7 2023-07-18 10:30:48.000000 clover-energy-5.1.0.post1/src/clover_energy.egg-info/top_level.txt
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1080 2023-06-30 07:49:00.000000 clover-energy-5.1.1/LICENSE
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)       47 2023-06-30 07:49:00.000000 clover-energy-5.1.1/MANIFEST.in
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    16573 2023-07-25 13:19:21.000000 clover-energy-5.1.1/PKG-INFO
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    15933 2023-07-17 10:28:59.000000 clover-energy-5.1.1/README.md
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      103 2023-06-30 07:49:00.000000 clover-energy-5.1.1/pyproject.toml
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1296 2023-07-25 13:19:21.000000 clover-energy-5.1.1/setup.cfg
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     2049 2023-07-17 10:09:36.000000 clover-energy-5.1.1/src/clover/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    51535 2023-07-25 12:11:04.000000 clover-energy-5.1.1/src/clover/__main__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    97316 2023-07-18 09:54:23.000000 clover-energy-5.1.1/src/clover/__utils__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    36718 2023-07-18 09:54:23.000000 clover-energy-5.1.1/src/clover/analysis.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     8512 2023-07-18 09:54:23.000000 clover-energy-5.1.1/src/clover/argparser.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/conversion/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      710 2023-07-17 10:09:36.000000 clover-energy-5.1.1/src/clover/conversion/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    26993 2023-07-17 10:28:59.000000 clover-energy-5.1.1/src/clover/conversion/conversion.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/conversion/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/conversion/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/conversion/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/conversion/tests/unit/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)   107239 2023-07-18 09:54:23.000000 clover-energy-5.1.1/src/clover/fileparser.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/generation/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/generation/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    20730 2023-07-18 09:54:23.000000 clover-energy-5.1.1/src/clover/generation/__utils__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    27727 2023-07-18 09:54:23.000000 clover-energy-5.1.1/src/clover/generation/solar.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/generation/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/generation/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/generation/tests/component/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/generation/tests/component/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/generation/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/generation/tests/unit/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4554 2023-07-18 09:54:23.000000 clover-energy-5.1.1/src/clover/generation/weather.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     3563 2023-07-18 09:54:23.000000 clover-energy-5.1.1/src/clover/generation/wind.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/impact/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1141 2023-07-17 10:09:36.000000 clover-energy-5.1.1/src/clover/impact/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4199 2023-07-17 10:28:59.000000 clover-energy-5.1.1/src/clover/impact/__utils__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    44572 2023-07-18 09:54:23.000000 clover-energy-5.1.1/src/clover/impact/finance.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    31219 2023-07-18 09:54:23.000000 clover-energy-5.1.1/src/clover/impact/ghgs.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/impact/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/impact/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/impact/tests/component/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/impact/tests/component/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/impact/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/impact/tests/unit/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/load/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      931 2023-07-17 10:09:36.000000 clover-energy-5.1.1/src/clover/load/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    39767 2023-07-17 10:28:59.000000 clover-energy-5.1.1/src/clover/load/load.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/load/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/load/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/load/tests/component/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/load/tests/component/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/mains_supply/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      774 2023-07-17 10:09:36.000000 clover-energy-5.1.1/src/clover/mains_supply/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4473 2023-07-11 16:32:53.000000 clover-energy-5.1.1/src/clover/mains_supply/__utils__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4578 2023-07-11 16:32:53.000000 clover-energy-5.1.1/src/clover/mains_supply/grid.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/mains_supply/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/mains_supply/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/mains_supply/tests/component/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/mains_supply/tests/component/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/mains_supply/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/mains_supply/tests/unit/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    11741 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/mains_supply/water_source.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/src/clover/optimisation/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1069 2023-07-17 10:09:36.000000 clover-energy-5.1.1/src/clover/optimisation/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    43348 2023-07-18 10:01:36.000000 clover-energy-5.1.1/src/clover/optimisation/__utils__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    29385 2023-07-18 09:54:23.000000 clover-energy-5.1.1/src/clover/optimisation/appraisal.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    64706 2023-07-18 09:54:23.000000 clover-energy-5.1.1/src/clover/optimisation/optimisation.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    43556 2023-07-18 09:54:23.000000 clover-energy-5.1.1/src/clover/optimisation/single_line_simulation.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/src/clover/optimisation/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/optimisation/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/src/clover/optimisation/tests/component/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/optimisation/tests/component/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/src/clover/optimisation/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/optimisation/tests/unit/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     8754 2023-07-18 09:54:23.000000 clover-energy-5.1.1/src/clover/printer.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/src/clover/scripts/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/scripts/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1309 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/scripts/clover.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1202 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/scripts/clover_hpc_clover.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1298 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/scripts/clover_hpc_outbox_assembly.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1138 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/scripts/clover_new_location.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1360 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/scripts/clover_update_api_token.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     6682 2023-07-17 10:09:36.000000 clover-energy-5.1.1/src/clover/scripts/hpc.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    10191 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/scripts/hpc_clover.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4894 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/scripts/hpc_outbox_assembly.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    22944 2023-07-17 10:09:36.000000 clover-energy-5.1.1/src/clover/scripts/hpc_utils.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    11904 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/scripts/new_location.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/src/clover/scripts/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/scripts/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/src/clover/scripts/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/scripts/tests/unit/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     3638 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/scripts/update_api_token.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/src/clover/simulation/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1199 2023-07-17 10:09:36.000000 clover-energy-5.1.1/src/clover/simulation/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    21928 2023-07-18 09:54:23.000000 clover-energy-5.1.1/src/clover/simulation/__utils__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    12992 2023-07-17 10:28:59.000000 clover-energy-5.1.1/src/clover/simulation/diesel.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    88978 2023-07-25 10:34:01.000000 clover-energy-5.1.1/src/clover/simulation/energy_system.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     2450 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/simulation/exchanger.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    24234 2023-07-17 10:28:59.000000 clover-energy-5.1.1/src/clover/simulation/solar.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    31896 2023-07-25 12:19:28.000000 clover-energy-5.1.1/src/clover/simulation/storage.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    19002 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/simulation/storage_utils.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/src/clover/simulation/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/simulation/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/src/clover/simulation/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/simulation/tests/unit/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     5411 2023-07-11 16:48:20.000000 clover-energy-5.1.1/src/clover/simulation/transmission.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/src/clover/src/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/src/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    56900 2023-07-25 10:16:42.000000 clover-energy-5.1.1/src/clover/src/new_location.yaml
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/src/clover/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/src/clover/tests/integration/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/tests/integration/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/src/clover/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:49:00.000000 clover-energy-5.1.1/src/clover/tests/unit/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/src/clover_energy.egg-info/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    16573 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover_energy.egg-info/PKG-INFO
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     3003 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover_energy.egg-info/SOURCES.txt
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)        1 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover_energy.egg-info/dependency_links.txt
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      299 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover_energy.egg-info/entry_points.txt
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      119 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover_energy.egg-info/requires.txt
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)        7 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover_energy.egg-info/top_level.txt
```

### Comparing `clover-energy-5.1.0.post1/LICENSE` & `clover-energy-5.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/PKG-INFO` & `clover-energy-5.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clover-energy
-Version: 5.1.0.post1
+Version: 5.1.1
 Summary: Continuous Lifetime Optimisation of Variable Electricity Resources
 Home-page: https://github.com/CLOVER-energy/CLOVER
 Author: Phil Sandwell, Ben Winchester and Hamish Beath
 Author-email: philip.sandwell@gmail.com,benedict.winchester@gmail.com,hamishbeath@outlook.com
 Project-URL: Bug Tracker, https://github.com/CLOVER-energy/CLOVER/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `clover-energy-5.1.0.post1/README.md` & `clover-energy-5.1.1/README.md`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/setup.cfg` & `clover-energy-5.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = clover-energy
-version = 5.1.0.post1
+version = 5.1.1
 author = Phil Sandwell, Ben Winchester and Hamish Beath
 author_email = philip.sandwell@gmail.com,benedict.winchester@gmail.com,hamishbeath@outlook.com
 description = Continuous Lifetime Optimisation of Variable Electricity Resources
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CLOVER-energy/CLOVER
 project_urls =
```

### Comparing `clover-energy-5.1.0.post1/src/clover/__init__.py` & `clover-energy-5.1.1/src/clover/__init__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/__main__.py` & `clover-energy-5.1.1/src/clover/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 CLOVER (Continuous Lifetime Optimisation of Variable Electricity Resources) can evaluate
 and optimise minigrid systems, determining whether a demand is met whilst minimising
 environmental and economic impacts. The main flow of CLOVER can be executed by running
 the clover module from the command-line interface.
 
 """
 
-__version__ = "5.1.0.post1"
+__version__ = "5.1.1"
 
 import collections
 import datetime
 import logging
 import math
 import os
 import re
```

### Comparing `clover-energy-5.1.0.post1/src/clover/__utils__.py` & `clover-energy-5.1.1/src/clover/__utils__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/analysis.py` & `clover-energy-5.1.1/src/clover/analysis.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/argparser.py` & `clover-energy-5.1.1/src/clover/argparser.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/conversion/__init__.py` & `clover-energy-5.1.1/src/clover/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/conversion/conversion.py` & `clover-energy-5.1.1/src/clover/conversion/conversion.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/fileparser.py` & `clover-energy-5.1.1/src/clover/fileparser.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/generation/__utils__.py` & `clover-energy-5.1.1/src/clover/generation/__utils__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/generation/solar.py` & `clover-energy-5.1.1/src/clover/generation/solar.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/generation/weather.py` & `clover-energy-5.1.1/src/clover/generation/weather.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/generation/wind.py` & `clover-energy-5.1.1/src/clover/generation/wind.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/impact/__init__.py` & `clover-energy-5.1.1/src/clover/impact/__init__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/impact/__utils__.py` & `clover-energy-5.1.1/src/clover/impact/__utils__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/impact/finance.py` & `clover-energy-5.1.1/src/clover/impact/finance.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/impact/ghgs.py` & `clover-energy-5.1.1/src/clover/impact/ghgs.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/load/__init__.py` & `clover-energy-5.1.1/src/clover/load/__init__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/load/load.py` & `clover-energy-5.1.1/src/clover/load/load.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/mains_supply/__init__.py` & `clover-energy-5.1.1/src/clover/mains_supply/__init__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/mains_supply/__utils__.py` & `clover-energy-5.1.1/src/clover/mains_supply/__utils__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/mains_supply/grid.py` & `clover-energy-5.1.1/src/clover/mains_supply/grid.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/mains_supply/water_source.py` & `clover-energy-5.1.1/src/clover/mains_supply/water_source.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/optimisation/__init__.py` & `clover-energy-5.1.1/src/clover/optimisation/__init__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/optimisation/__utils__.py` & `clover-energy-5.1.1/src/clover/optimisation/__utils__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/optimisation/appraisal.py` & `clover-energy-5.1.1/src/clover/optimisation/appraisal.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/optimisation/optimisation.py` & `clover-energy-5.1.1/src/clover/optimisation/optimisation.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/optimisation/single_line_simulation.py` & `clover-energy-5.1.1/src/clover/optimisation/single_line_simulation.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/printer.py` & `clover-energy-5.1.1/src/clover/printer.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/scripts/clover.py` & `clover-energy-5.1.1/src/clover/scripts/clover.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/scripts/clover_hpc_clover.py` & `clover-energy-5.1.1/src/clover/scripts/clover_hpc_clover.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/scripts/clover_hpc_outbox_assembly.py` & `clover-energy-5.1.1/src/clover/scripts/clover_hpc_outbox_assembly.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/scripts/clover_new_location.py` & `clover-energy-5.1.1/src/clover/scripts/clover_new_location.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/scripts/clover_update_api_token.py` & `clover-energy-5.1.1/src/clover/scripts/clover_update_api_token.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/scripts/hpc.py` & `clover-energy-5.1.1/src/clover/scripts/hpc.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/scripts/hpc_clover.py` & `clover-energy-5.1.1/src/clover/scripts/hpc_clover.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/scripts/hpc_outbox_assembly.py` & `clover-energy-5.1.1/src/clover/scripts/hpc_outbox_assembly.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/scripts/hpc_utils.py` & `clover-energy-5.1.1/src/clover/scripts/hpc_utils.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/scripts/new_location.py` & `clover-energy-5.1.1/src/clover/scripts/new_location.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/scripts/update_api_token.py` & `clover-energy-5.1.1/src/clover/scripts/update_api_token.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/simulation/__init__.py` & `clover-energy-5.1.1/src/clover/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/simulation/__utils__.py` & `clover-energy-5.1.1/src/clover/simulation/__utils__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/simulation/diesel.py` & `clover-energy-5.1.1/src/clover/simulation/diesel.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/simulation/energy_system.py` & `clover-energy-5.1.1/src/clover/simulation/energy_system.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/simulation/exchanger.py` & `clover-energy-5.1.1/src/clover/simulation/exchanger.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/simulation/solar.py` & `clover-energy-5.1.1/src/clover/simulation/solar.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/simulation/storage.py` & `clover-energy-5.1.1/src/clover/simulation/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -652,15 +652,17 @@
         battery_storage_profile: pd.DataFrame = pd.DataFrame(
             remaining_profile.values + grid_energy.values
         )
 
     else:
         # Take energy from grid first if available
         if scenario.grid:
-            grid_energy = pd.DataFrame(grid_profile.mul(load_energy[0]))  # type: ignore
+            grid_energy = pd.DataFrame(  # type: ignore
+                grid_profile.mul(load_energy[0].values).values
+            )
         else:
             grid_energy = pd.DataFrame([0] * (end_hour - start_hour))
         # as needed for load
         remaining_profile = (grid_energy[0] <= 0).mul(load_energy[0])  # type: ignore
         logger.debug(
             "Remainig profile: %s kWh",
             round(float(np.sum(remaining_profile)), 2),  # type: ignore [arg-type]
```

### Comparing `clover-energy-5.1.0.post1/src/clover/simulation/storage_utils.py` & `clover-energy-5.1.1/src/clover/simulation/storage_utils.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/simulation/transmission.py` & `clover-energy-5.1.1/src/clover/simulation/transmission.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover/src/new_location.yaml` & `clover-energy-5.1.1/src/clover/src/new_location.yaml`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.0.post1/src/clover_energy.egg-info/PKG-INFO` & `clover-energy-5.1.1/src/clover_energy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clover-energy
-Version: 5.1.0.post1
+Version: 5.1.1
 Summary: Continuous Lifetime Optimisation of Variable Electricity Resources
 Home-page: https://github.com/CLOVER-energy/CLOVER
 Author: Phil Sandwell, Ben Winchester and Hamish Beath
 Author-email: philip.sandwell@gmail.com,benedict.winchester@gmail.com,hamishbeath@outlook.com
 Project-URL: Bug Tracker, https://github.com/CLOVER-energy/CLOVER/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `clover-energy-5.1.0.post1/src/clover_energy.egg-info/SOURCES.txt` & `clover-energy-5.1.1/src/clover_energy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

