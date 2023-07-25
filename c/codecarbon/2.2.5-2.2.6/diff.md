# Comparing `tmp/codecarbon-2.2.5.tar.gz` & `tmp/codecarbon-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codecarbon-2.2.5.tar", last modified: Wed Jul 12 17:40:00 2023, max compression
+gzip compressed data, was "codecarbon-2.2.6.tar", last modified: Tue Jul 25 06:29:22 2023, max compression
```

## Comparing `codecarbon-2.2.5.tar` & `codecarbon-2.2.6.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.708821 codecarbon-2.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-12 17:39:42.000000 codecarbon-2.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-12 17:40:00.708821 codecarbon-2.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-07-12 17:39:42.000000 codecarbon-2.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.688821 codecarbon-2.2.5/carbonserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.688821 codecarbon-2.2.5/carbonserver/carbonserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.688821 codecarbon-2.2.5/carbonserver/carbonserver/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.692821 codecarbon-2.2.5/carbonserver/carbonserver/api/domain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/domain/emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/domain/experiments.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/domain/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/domain/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/domain/runs.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/domain/teams.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/domain/users.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.692821 codecarbon-2.2.5/carbonserver/carbonserver/api/routers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/routers/authenticate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/routers/emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/routers/experiments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/routers/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/routers/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/routers/runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/routers/teams.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/routers/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/api/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.692821 codecarbon-2.2.5/carbonserver/carbonserver/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/database/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/carbonserver/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-12 17:39:42.000000 codecarbon-2.2.5/carbonserver/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.696821 codecarbon-2.2.5/codecarbon/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.696821 codecarbon-2.2.5/codecarbon/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/cli/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.700821 codecarbon-2.2.5/codecarbon/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/core/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/core/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/core/co2_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13758 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/core/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/core/emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/core/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/core/rapl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/core/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/core/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/core/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.684821 codecarbon-2.2.5/codecarbon/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.700821 codecarbon-2.2.5/codecarbon/data/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/data/cloud/impact.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.700821 codecarbon-2.2.5/codecarbon/data/hardware/
--rw-r--r--   0 runner    (1001) docker     (123)    49563 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/data/hardware/cpu_power.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.700821 codecarbon-2.2.5/codecarbon/data/private_infra/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.700821 codecarbon-2.2.5/codecarbon/data/private_infra/2016/
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/data/private_infra/2016/canada_energy_mix.json
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/data/private_infra/2016/usa_emissions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/data/private_infra/carbon_intensity_per_source.json
--rw-r--r--   0 runner    (1001) docker     (123)   124501 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/data/private_infra/global_energy_mix.json
--rw-r--r--   0 runner    (1001) docker     (123)    39720 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/emissions_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.700821 codecarbon-2.2.5/codecarbon/external/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/external/geography.py
--rw-r--r--   0 runner    (1001) docker     (123)    11030 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/external/hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/external/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/external/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.700821 codecarbon-2.2.5/codecarbon/prometheus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/prometheus/metric_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/prometheus/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.704821 codecarbon-2.2.5/codecarbon/viz/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/viz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.704821 codecarbon-2.2.5/codecarbon/viz/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/viz/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25442 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/viz/assets/car_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    29734 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/viz/assets/house_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    29874 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/viz/assets/tv_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/viz/carbonboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/viz/carbonboard_on_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27905 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/viz/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-07-12 17:39:42.000000 codecarbon-2.2.5/codecarbon/viz/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.696821 codecarbon-2.2.5/codecarbon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-12 17:40:00.000000 codecarbon-2.2.5/codecarbon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-07-12 17:40:00.000000 codecarbon-2.2.5/codecarbon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:40:00.000000 codecarbon-2.2.5/codecarbon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-12 17:40:00.000000 codecarbon-2.2.5/codecarbon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-12 17:40:00.000000 codecarbon-2.2.5/codecarbon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-12 17:40:00.000000 codecarbon-2.2.5/codecarbon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 17:40:00.708821 codecarbon-2.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-12 17:39:43.000000 codecarbon-2.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:40:00.708821 codecarbon-2.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_api_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_co2_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_core_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10298 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_emissions_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_emissions_tracker_constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_emissions_tracker_flush.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_geography.py
--rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_logging_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/test_ram.py
--rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/testdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-12 17:39:43.000000 codecarbon-2.2.5/tests/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:22.044973 codecarbon-2.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-25 06:29:09.000000 codecarbon-2.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-25 06:29:22.044973 codecarbon-2.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-07-25 06:29:09.000000 codecarbon-2.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:22.032972 codecarbon-2.2.6/carbonserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:09.000000 codecarbon-2.2.6/carbonserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:22.032972 codecarbon-2.2.6/carbonserver/carbonserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:09.000000 codecarbon-2.2.6/carbonserver/carbonserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:22.032972 codecarbon-2.2.6/carbonserver/carbonserver/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:09.000000 codecarbon-2.2.6/carbonserver/carbonserver/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-25 06:29:09.000000 codecarbon-2.2.6/carbonserver/carbonserver/api/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:22.032972 codecarbon-2.2.6/carbonserver/carbonserver/api/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:09.000000 codecarbon-2.2.6/carbonserver/carbonserver/api/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-25 06:29:09.000000 codecarbon-2.2.6/carbonserver/carbonserver/api/domain/emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-25 06:29:09.000000 codecarbon-2.2.6/carbonserver/carbonserver/api/domain/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-25 06:29:09.000000 codecarbon-2.2.6/carbonserver/carbonserver/api/domain/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-25 06:29:09.000000 codecarbon-2.2.6/carbonserver/carbonserver/api/domain/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-25 06:29:09.000000 codecarbon-2.2.6/carbonserver/carbonserver/api/domain/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-25 06:29:09.000000 codecarbon-2.2.6/carbonserver/carbonserver/api/domain/teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-25 06:29:09.000000 codecarbon-2.2.6/carbonserver/carbonserver/api/domain/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-25 06:29:09.000000 codecarbon-2.2.6/carbonserver/carbonserver/api/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:22.036972 codecarbon-2.2.6/carbonserver/carbonserver/api/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:09.000000 codecarbon-2.2.6/carbonserver/carbonserver/api/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-25 06:29:09.000000 codecarbon-2.2.6/carbonserver/carbonserver/api/routers/authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-25 06:29:09.000000 codecarbon-2.2.6/carbonserver/carbonserver/api/routers/emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-25 06:29:09.000000 codecarbon-2.2.6/carbonserver/carbonserver/api/routers/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-07-25 06:29:09.000000 codecarbon-2.2.6/carbonserver/carbonserver/api/routers/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-25 06:29:09.000000 codecarbon-2.2.6/carbonserver/carbonserver/api/routers/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-07-25 06:29:09.000000 codecarbon-2.2.6/carbonserver/carbonserver/api/routers/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-25 06:29:09.000000 codecarbon-2.2.6/carbonserver/carbonserver/api/routers/teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-25 06:29:09.000000 codecarbon-2.2.6/carbonserver/carbonserver/api/routers/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-07-25 06:29:09.000000 codecarbon-2.2.6/carbonserver/carbonserver/api/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-25 06:29:09.000000 codecarbon-2.2.6/carbonserver/carbonserver/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:22.036972 codecarbon-2.2.6/carbonserver/carbonserver/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:09.000000 codecarbon-2.2.6/carbonserver/carbonserver/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-25 06:29:09.000000 codecarbon-2.2.6/carbonserver/carbonserver/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-25 06:29:09.000000 codecarbon-2.2.6/carbonserver/carbonserver/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-07-25 06:29:09.000000 codecarbon-2.2.6/carbonserver/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-25 06:29:09.000000 codecarbon-2.2.6/carbonserver/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-25 06:29:09.000000 codecarbon-2.2.6/carbonserver/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:22.036972 codecarbon-2.2.6/codecarbon/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:22.036972 codecarbon-2.2.6/codecarbon/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/cli/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:22.040973 codecarbon-2.2.6/codecarbon/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/core/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/core/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/core/co2_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13758 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/core/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/core/emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7976 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/core/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/core/rapl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/core/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/core/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/core/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:22.028972 codecarbon-2.2.6/codecarbon/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:22.040973 codecarbon-2.2.6/codecarbon/data/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/data/cloud/impact.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:22.040973 codecarbon-2.2.6/codecarbon/data/hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)    49563 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/data/hardware/cpu_power.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:22.040973 codecarbon-2.2.6/codecarbon/data/private_infra/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:22.040973 codecarbon-2.2.6/codecarbon/data/private_infra/2016/
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/data/private_infra/2016/canada_energy_mix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/data/private_infra/2016/usa_emissions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/data/private_infra/carbon_intensity_per_source.json
+-rw-r--r--   0 runner    (1001) docker     (123)   124501 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/data/private_infra/global_energy_mix.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39720 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/emissions_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:22.040973 codecarbon-2.2.6/codecarbon/external/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/external/geography.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11030 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/external/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/external/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/external/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:22.040973 codecarbon-2.2.6/codecarbon/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/prometheus/metric_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/prometheus/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:22.040973 codecarbon-2.2.6/codecarbon/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/viz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:22.040973 codecarbon-2.2.6/codecarbon/viz/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/viz/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25442 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/viz/assets/car_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29734 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/viz/assets/house_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29874 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/viz/assets/tv_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/viz/carbonboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/viz/carbonboard_on_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27905 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/viz/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-07-25 06:29:09.000000 codecarbon-2.2.6/codecarbon/viz/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:22.036972 codecarbon-2.2.6/codecarbon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-25 06:29:22.000000 codecarbon-2.2.6/codecarbon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-07-25 06:29:22.000000 codecarbon-2.2.6/codecarbon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:29:22.000000 codecarbon-2.2.6/codecarbon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-25 06:29:22.000000 codecarbon-2.2.6/codecarbon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-25 06:29:22.000000 codecarbon-2.2.6/codecarbon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-25 06:29:22.000000 codecarbon-2.2.6/codecarbon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 06:29:22.044973 codecarbon-2.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-25 06:29:09.000000 codecarbon-2.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:29:22.044973 codecarbon-2.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-25 06:29:09.000000 codecarbon-2.2.6/tests/test_api_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-25 06:29:09.000000 codecarbon-2.2.6/tests/test_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-25 06:29:09.000000 codecarbon-2.2.6/tests/test_co2_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-07-25 06:29:09.000000 codecarbon-2.2.6/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-25 06:29:09.000000 codecarbon-2.2.6/tests/test_core_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10298 2023-07-25 06:29:09.000000 codecarbon-2.2.6/tests/test_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-07-25 06:29:09.000000 codecarbon-2.2.6/tests/test_emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-07-25 06:29:09.000000 codecarbon-2.2.6/tests/test_emissions_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-07-25 06:29:09.000000 codecarbon-2.2.6/tests/test_emissions_tracker_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-25 06:29:09.000000 codecarbon-2.2.6/tests/test_emissions_tracker_flush.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-25 06:29:09.000000 codecarbon-2.2.6/tests/test_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-07-25 06:29:09.000000 codecarbon-2.2.6/tests/test_geography.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-07-25 06:29:09.000000 codecarbon-2.2.6/tests/test_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-25 06:29:09.000000 codecarbon-2.2.6/tests/test_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-25 06:29:09.000000 codecarbon-2.2.6/tests/test_logging_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-25 06:29:09.000000 codecarbon-2.2.6/tests/test_ram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-07-25 06:29:09.000000 codecarbon-2.2.6/tests/testdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-25 06:29:09.000000 codecarbon-2.2.6/tests/testutils.py
```

### Comparing `codecarbon-2.2.5/LICENSE` & `codecarbon-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/PKG-INFO` & `codecarbon-2.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codecarbon
-Version: 2.2.5
+Version: 2.2.6
 Author: Mila, DataForGood, BCG GAMMA, Comet.ml, Haverford College
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `codecarbon-2.2.5/README.md` & `codecarbon-2.2.6/README.md`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/carbonserver/carbonserver/api/dependencies.py` & `codecarbon-2.2.6/carbonserver/carbonserver/api/dependencies.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/carbonserver/carbonserver/api/domain/experiments.py` & `codecarbon-2.2.6/carbonserver/carbonserver/api/domain/experiments.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/carbonserver/carbonserver/api/errors.py` & `codecarbon-2.2.6/carbonserver/carbonserver/api/errors.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/carbonserver/carbonserver/api/routers/authenticate.py` & `codecarbon-2.2.6/carbonserver/carbonserver/api/routers/authenticate.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/carbonserver/carbonserver/api/routers/emissions.py` & `codecarbon-2.2.6/carbonserver/carbonserver/api/routers/emissions.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/carbonserver/carbonserver/api/routers/experiments.py` & `codecarbon-2.2.6/carbonserver/carbonserver/api/routers/experiments.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/carbonserver/carbonserver/api/routers/organizations.py` & `codecarbon-2.2.6/carbonserver/carbonserver/api/routers/organizations.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/carbonserver/carbonserver/api/routers/projects.py` & `codecarbon-2.2.6/carbonserver/carbonserver/api/routers/projects.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/carbonserver/carbonserver/api/routers/runs.py` & `codecarbon-2.2.6/carbonserver/carbonserver/api/routers/runs.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/carbonserver/carbonserver/api/routers/teams.py` & `codecarbon-2.2.6/carbonserver/carbonserver/api/routers/teams.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/carbonserver/carbonserver/api/routers/users.py` & `codecarbon-2.2.6/carbonserver/carbonserver/api/routers/users.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/carbonserver/carbonserver/api/schemas.py` & `codecarbon-2.2.6/carbonserver/carbonserver/api/schemas.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/carbonserver/carbonserver/database/database.py` & `codecarbon-2.2.6/carbonserver/carbonserver/database/database.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/carbonserver/container.py` & `codecarbon-2.2.6/carbonserver/container.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/carbonserver/main.py` & `codecarbon-2.2.6/carbonserver/main.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/carbonserver/setup.py` & `codecarbon-2.2.6/carbonserver/setup.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/cli/cli_utils.py` & `codecarbon-2.2.6/codecarbon/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/cli/main.py` & `codecarbon-2.2.6/codecarbon/cli/main.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/core/api_client.py` & `codecarbon-2.2.6/codecarbon/core/api_client.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/core/cloud.py` & `codecarbon-2.2.6/codecarbon/core/cloud.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/core/co2_signal.py` & `codecarbon-2.2.6/codecarbon/core/co2_signal.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/core/config.py` & `codecarbon-2.2.6/codecarbon/core/config.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/core/cpu.py` & `codecarbon-2.2.6/codecarbon/core/cpu.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/core/emissions.py` & `codecarbon-2.2.6/codecarbon/core/emissions.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/core/gpu.py` & `codecarbon-2.2.6/codecarbon/core/gpu.py`

 * *Files 8% similar despite different names*

```diff
@@ -126,31 +126,36 @@
     ]
     """
     try:
         pynvml.nvmlInit()
         deviceCount = pynvml.nvmlDeviceGetCount()
         devices = []
         for i in range(deviceCount):
-            handle = pynvml.nvmlDeviceGetHandleByIndex(i)
+            try:
+                handle = pynvml.nvmlDeviceGetHandleByIndex(i)
 
-            # Memory
-            memory = get_memory_info(handle)
+                # Memory
+                memory = get_memory_info(handle)
 
-            device_details = {
-                "name": get_gpu_name(handle),
-                "uuid": get_uuid(handle),
-                "total_memory": memory.total,
-                "power_limit": get_power_limit(handle),
-                "gpu_index": i,
-            }
-            devices.append(device_details)
+                device_details = {
+                    "name": get_gpu_name(handle),
+                    "uuid": get_uuid(handle),
+                    "total_memory": memory.total,
+                    "power_limit": get_power_limit(handle),
+                    "gpu_index": i,
+                }
+                devices.append(device_details)
+            except Exception as e:
+                logger.warning(
+                    f"Failed to retrieve info for GPU number {i} : {e}", exc_info=True
+                )
         return devices
 
     except pynvml.NVMLError:
-        logger.debug("Failed to retrieve gpu static info", exc_info=True)
+        logger.warning("Failed to retrieve gpu static info", exc_info=True)
         return []
 
 
 def get_gpu_details():
     """Get all GPUs instantaneous metrics
     >>> get_gpu_details()
     [
@@ -171,38 +176,43 @@
     ]
     """
     try:
         pynvml.nvmlInit()
         deviceCount = pynvml.nvmlDeviceGetCount()
         devices = []
         for i in range(deviceCount):
-            handle = pynvml.nvmlDeviceGetHandleByIndex(i)
+            try:
+                handle = pynvml.nvmlDeviceGetHandleByIndex(i)
 
-            # Memory
-            memory = get_memory_info(handle)
+                # Memory
+                memory = get_memory_info(handle)
 
-            device_details = {
-                "name": get_gpu_name(handle),
-                "uuid": get_uuid(handle),
-                "free_memory": memory.free,
-                "total_memory": memory.total,
-                "used_memory": memory.used,
-                "temperature": get_temperature(handle),
-                "power_usage": get_power_usage(handle),
-                "power_limit": get_power_limit(handle),
-                "gpu_utilization": get_gpu_utilization(handle),
-                "compute_mode": get_compute_mode(handle),
-                "compute_processes": get_compute_processes(handle),
-                "graphics_processes": get_graphics_processes(handle),
-            }
-            devices.append(device_details)
+                device_details = {
+                    "name": get_gpu_name(handle),
+                    "uuid": get_uuid(handle),
+                    "free_memory": memory.free,
+                    "total_memory": memory.total,
+                    "used_memory": memory.used,
+                    "temperature": get_temperature(handle),
+                    "power_usage": get_power_usage(handle),
+                    "power_limit": get_power_limit(handle),
+                    "gpu_utilization": get_gpu_utilization(handle),
+                    "compute_mode": get_compute_mode(handle),
+                    "compute_processes": get_compute_processes(handle),
+                    "graphics_processes": get_graphics_processes(handle),
+                }
+                devices.append(device_details)
+            except Exception as e:
+                logger.warning(
+                    f"Failed to retrieve info for GPU number {i} : {e}", exc_info=True
+                )
         return devices
 
     except pynvml.NVMLError:
-        logger.debug("Failed to retrieve gpu information", exc_info=True)
+        logger.warning("Failed to retrieve gpu information", exc_info=True)
         return []
 
 
 def is_gpu_details_available():
     """Returns True if the GPU details are available."""
     try:
         pynvml.nvmlInit()
```

### Comparing `codecarbon-2.2.5/codecarbon/core/rapl.py` & `codecarbon-2.2.6/codecarbon/core/rapl.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/core/schemas.py` & `codecarbon-2.2.6/codecarbon/core/schemas.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/core/units.py` & `codecarbon-2.2.6/codecarbon/core/units.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/core/util.py` & `codecarbon-2.2.6/codecarbon/core/util.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/data/cloud/impact.csv` & `codecarbon-2.2.6/codecarbon/data/cloud/impact.csv`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/data/hardware/cpu_power.csv` & `codecarbon-2.2.6/codecarbon/data/hardware/cpu_power.csv`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/data/private_infra/2016/canada_energy_mix.json` & `codecarbon-2.2.6/codecarbon/data/private_infra/2016/canada_energy_mix.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/data/private_infra/2016/usa_emissions.json` & `codecarbon-2.2.6/codecarbon/data/private_infra/2016/usa_emissions.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/data/private_infra/carbon_intensity_per_source.json` & `codecarbon-2.2.6/codecarbon/data/private_infra/carbon_intensity_per_source.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/data/private_infra/global_energy_mix.json` & `codecarbon-2.2.6/codecarbon/data/private_infra/global_energy_mix.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/emissions_tracker.py` & `codecarbon-2.2.6/codecarbon/emissions_tracker.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/external/geography.py` & `codecarbon-2.2.6/codecarbon/external/geography.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/external/hardware.py` & `codecarbon-2.2.6/codecarbon/external/hardware.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/external/logger.py` & `codecarbon-2.2.6/codecarbon/external/logger.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/external/scheduler.py` & `codecarbon-2.2.6/codecarbon/external/scheduler.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/input.py` & `codecarbon-2.2.6/codecarbon/input.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/output.py` & `codecarbon-2.2.6/codecarbon/output.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/prometheus/metric_definitions.py` & `codecarbon-2.2.6/codecarbon/prometheus/metric_definitions.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/prometheus/prometheus.py` & `codecarbon-2.2.6/codecarbon/prometheus/prometheus.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/viz/assets/car_icon.png` & `codecarbon-2.2.6/codecarbon/viz/assets/car_icon.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/viz/assets/house_icon.png` & `codecarbon-2.2.6/codecarbon/viz/assets/house_icon.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/viz/assets/tv_icon.png` & `codecarbon-2.2.6/codecarbon/viz/assets/tv_icon.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/viz/carbonboard.py` & `codecarbon-2.2.6/codecarbon/viz/carbonboard.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/viz/carbonboard_on_api.py` & `codecarbon-2.2.6/codecarbon/viz/carbonboard_on_api.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/viz/components.py` & `codecarbon-2.2.6/codecarbon/viz/components.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon/viz/data.py` & `codecarbon-2.2.6/codecarbon/viz/data.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/codecarbon.egg-info/PKG-INFO` & `codecarbon-2.2.6/codecarbon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codecarbon
-Version: 2.2.5
+Version: 2.2.6
 Author: Mila, DataForGood, BCG GAMMA, Comet.ml, Haverford College
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `codecarbon-2.2.5/codecarbon.egg-info/SOURCES.txt` & `codecarbon-2.2.6/codecarbon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/setup.py` & `codecarbon-2.2.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ]
 
 TEST_DEPENDENCIES = ["mock", "pytest", "responses", "tox", "numpy", "requests-mock"]
 
 
 setuptools.setup(
     name="codecarbon",
-    version="2.2.5",
+    version="2.2.6",
     author="Mila, DataForGood, BCG GAMMA, Comet.ml, Haverford College",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license_files=("LICENSE",),
     packages=setuptools.find_packages(
         exclude=["*.tests", "*.tests.*", "tests.*", "tests"]
     ),
```

### Comparing `codecarbon-2.2.5/tests/test_api_call.py` & `codecarbon-2.2.6/tests/test_api_call.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/tests/test_cloud.py` & `codecarbon-2.2.6/tests/test_cloud.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/tests/test_co2_signal.py` & `codecarbon-2.2.6/tests/test_co2_signal.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/tests/test_config.py` & `codecarbon-2.2.6/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/tests/test_core_util.py` & `codecarbon-2.2.6/tests/test_core_util.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/tests/test_cpu.py` & `codecarbon-2.2.6/tests/test_cpu.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/tests/test_emissions.py` & `codecarbon-2.2.6/tests/test_emissions.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/tests/test_emissions_tracker.py` & `codecarbon-2.2.6/tests/test_emissions_tracker.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/tests/test_emissions_tracker_constant.py` & `codecarbon-2.2.6/tests/test_emissions_tracker_constant.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/tests/test_emissions_tracker_flush.py` & `codecarbon-2.2.6/tests/test_emissions_tracker_flush.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/tests/test_energy.py` & `codecarbon-2.2.6/tests/test_energy.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/tests/test_geography.py` & `codecarbon-2.2.6/tests/test_geography.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/tests/test_gpu.py` & `codecarbon-2.2.6/tests/test_gpu.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/tests/test_hardware.py` & `codecarbon-2.2.6/tests/test_hardware.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/tests/test_logging_output.py` & `codecarbon-2.2.6/tests/test_logging_output.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/tests/test_ram.py` & `codecarbon-2.2.6/tests/test_ram.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/tests/testdata.py` & `codecarbon-2.2.6/tests/testdata.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.5/tests/testutils.py` & `codecarbon-2.2.6/tests/testutils.py`

 * *Files identical despite different names*

