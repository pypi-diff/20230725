# Comparing `tmp/hxrsnd-0.2.9.tar.gz` & `tmp/hxrsnd-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hxrsnd-0.2.9.tar", last modified: Thu Oct 20 20:42:57 2022, max compression
+gzip compressed data, was "hxrsnd-0.3.0.tar", last modified: Tue Jul 25 21:09:45 2023, max compression
```

## Comparing `hxrsnd-0.2.9.tar` & `hxrsnd-0.3.0.tar`

### file list

```diff
@@ -1,61 +1,115 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-10-20 20:42:57.179074 hxrsnd-0.2.9/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2468 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/LICENSE.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       93 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      175 2022-10-20 20:42:57.179074 hxrsnd-0.2.9/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1796 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-10-20 20:42:57.179074 hxrsnd-0.2.9/hxrsnd/
--rw-rw-r--   0 travis    (2000) travis    (2000)      203 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      497 2022-10-20 20:42:57.179074 hxrsnd-0.2.9/hxrsnd/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25352 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/aerotech.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17884 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/attocube.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9806 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/bragg.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8062 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/diode.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1248 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    49560 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/macromotor.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-10-20 20:42:57.175072 hxrsnd-0.2.9/hxrsnd/plans/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/plans/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8872 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/plans/alignment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17579 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/plans/calibration.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2066 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/plans/plan_stubs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1148 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/plans/preprocessors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6306 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/plans/scans.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8249 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/pneumatic.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      262 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/rtd.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-10-20 20:42:57.175072 hxrsnd-0.2.9/hxrsnd/screens/
--rw-rw-r--   0 travis    (2000) travis    (2000)    34405 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/screens/diode.ui
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1349 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/screens/motor_expert_screens.sh
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1368 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/screens/snd_main
--rw-rw-r--   0 travis    (2000) travis    (2000)      719 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/sequencer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2478 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/snddevice.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15924 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/sndmotor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6411 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/sndsystem.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-10-20 20:42:57.179074 hxrsnd-0.2.9/hxrsnd/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)       69 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8317 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1680 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/tests/test_aerotech.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1572 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/tests/test_attocube.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1637 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/tests/test_plans_alignment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9467 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/tests/test_plans_calibration.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      750 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/tests/test_plans_plan_stubs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1232 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/tests/test_plans_preprocessors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3835 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/tests/test_plans_scans.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1700 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/tests/test_pneumatic.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      543 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/tests/test_rtd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      473 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/tests/test_scripts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      561 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/tests/test_sequencer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      587 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/tests/test_snd_devices.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      560 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/tests/test_snddevice.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7317 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/tests/test_sndmotor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      423 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/tests/test_sndsystem.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1819 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/tests/test_tower.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2205 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/tests/test_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16139 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/tower.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4891 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/hxrsnd/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-10-20 20:42:57.175072 hxrsnd-0.2.9/hxrsnd.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      175 2022-10-20 20:42:57.000000 hxrsnd-0.2.9/hxrsnd.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1319 2022-10-20 20:42:57.000000 hxrsnd-0.2.9/hxrsnd.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-10-20 20:42:57.000000 hxrsnd-0.2.9/hxrsnd.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2022-10-20 20:42:57.000000 hxrsnd-0.2.9/hxrsnd.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      171 2022-10-20 20:42:57.179074 hxrsnd-0.2.9/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      368 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68552 2022-10-20 20:42:40.000000 hxrsnd-0.2.9/versioneer.py
+drwxr-xr-x   0 klauer   (1318172782) SLAC\Domain Users (1704612529)        0 2023-07-25 21:09:45.918804 hxrsnd-0.3.0/
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      132 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/.coveragerc
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      974 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/.flake8
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      125 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/.git_archival.txt
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)       32 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/.gitattributes
+drwxr-xr-x   0 klauer   (1318172782) SLAC\Domain Users (1704612529)        0 2023-07-25 21:09:45.792904 hxrsnd-0.3.0/.github/
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1068 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      751 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 klauer   (1318172782) SLAC\Domain Users (1704612529)        0 2023-07-25 21:09:45.794434 hxrsnd-0.3.0/.github/workflows/
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      750 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/.github/workflows/standard.yml
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1193 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/.gitignore
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      317 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/.landscape.yml
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      785 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      174 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/AUTHORS.rst
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     2987 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     2468 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/LICENSE.md
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)       93 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/MANIFEST.in
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     5012 2023-07-25 21:09:45.917712 hxrsnd-0.3.0/PKG-INFO
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1796 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/README.rst
+drwxr-xr-x   0 klauer   (1318172782) SLAC\Domain Users (1704612529)        0 2023-07-25 21:09:45.795405 hxrsnd-0.3.0/conda-recipe/
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      875 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/conda-recipe/meta.yaml
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)       33 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/dev-requirements.txt
+drwxr-xr-x   0 klauer   (1318172782) SLAC\Domain Users (1704612529)        0 2023-07-25 21:09:45.796360 hxrsnd-0.3.0/docs/
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      611 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/Makefile
+drwxr-xr-x   0 klauer   (1318172782) SLAC\Domain Users (1704612529)        0 2023-07-25 21:09:45.833592 hxrsnd-0.3.0/docs/source/
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      453 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/aerotech.rst
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1608 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/alignment.rst
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      343 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/attocube.rst
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     5821 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/basic_usage.rst
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      789 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/bragg.rst
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     7025 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/calibrating_delay_scans.rst
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      376 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/calibration.rst
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     2941 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/docs/source/conf.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)       42 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/diode.rst
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      268 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/exceptions.rst
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1286 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/index.rst
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1172 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/installation.rst
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1368 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/macromotor.rst
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      104 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/misc_plans.rst
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)       84 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/pneumatic.rst
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)       60 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/rtd.rst
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     2001 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/running_daq_scans.rst
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1195 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/running_scans.rst
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      144 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/scans.rst
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      460 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/screens.rst
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      911 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/scripting.rst
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      207 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/sndsystem.rst
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      413 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/tower.rst
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      274 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/docs/source/utils.rst
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)       67 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/docs-requirements.txt
+drwxr-xr-x   0 klauer   (1318172782) SLAC\Domain Users (1704612529)        0 2023-07-25 21:09:45.858818 hxrsnd-0.3.0/hxrsnd/
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      157 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/__init__.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      160 2023-07-25 21:09:45.000000 hxrsnd-0.3.0/hxrsnd/_version.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)    25036 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/aerotech.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)    17755 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/attocube.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     9792 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/bragg.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     8060 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/diode.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1224 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/exceptions.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)    49469 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/macromotor.py
+drwxr-xr-x   0 klauer   (1318172782) SLAC\Domain Users (1704612529)        0 2023-07-25 21:09:45.875357 hxrsnd-0.3.0/hxrsnd/plans/
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)        0 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/plans/__init__.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     8872 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/plans/alignment.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)    17557 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/plans/calibration.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     2064 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/plans/plan_stubs.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1148 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/plans/preprocessors.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     6284 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/plans/scans.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     8223 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/pneumatic.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      262 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/rtd.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     2392 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/run_snd.py
+drwxr-xr-x   0 klauer   (1318172782) SLAC\Domain Users (1704612529)        0 2023-07-25 21:09:45.878952 hxrsnd-0.3.0/hxrsnd/screens/
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)    34405 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/screens/diode.ui
+-rwxr-xr-x   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1349 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/screens/motor_expert_screens.sh
+-rwxr-xr-x   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1368 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/screens/snd_main
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      719 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/sequencer.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     2478 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/snddevice.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)    15921 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/sndmotor.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     6401 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/sndsystem.py
+drwxr-xr-x   0 klauer   (1318172782) SLAC\Domain Users (1704612529)        0 2023-07-25 21:09:45.911610 hxrsnd-0.3.0/hxrsnd/tests/
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)       69 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/tests/__init__.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     8309 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/tests/conftest.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1654 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/tests/test_aerotech.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1546 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/tests/test_attocube.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1637 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/tests/test_plans_alignment.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     9467 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/tests/test_plans_calibration.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      750 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/tests/test_plans_plan_stubs.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1232 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/tests/test_plans_preprocessors.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     3835 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/tests/test_plans_scans.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1674 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/tests/test_pneumatic.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      517 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/tests/test_rtd.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      473 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/tests/test_scripts.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      535 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/tests/test_sequencer.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      587 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/hxrsnd/tests/test_snd_devices.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      534 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/tests/test_snddevice.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     7291 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/tests/test_sndmotor.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      397 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/tests/test_sndsystem.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1793 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/tests/test_tower.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     2196 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/tests/test_utils.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)    16093 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/tower.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     4860 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/utils.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1898 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/hxrsnd/version.py
+drwxr-xr-x   0 klauer   (1318172782) SLAC\Domain Users (1704612529)        0 2023-07-25 21:09:45.867239 hxrsnd-0.3.0/hxrsnd.egg-info/
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     5012 2023-07-25 21:09:45.000000 hxrsnd-0.3.0/hxrsnd.egg-info/PKG-INFO
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     2406 2023-07-25 21:09:45.000000 hxrsnd-0.3.0/hxrsnd.egg-info/SOURCES.txt
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)        1 2023-07-25 21:09:45.000000 hxrsnd-0.3.0/hxrsnd.egg-info/dependency_links.txt
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)       48 2023-07-25 21:09:45.000000 hxrsnd-0.3.0/hxrsnd.egg-info/entry_points.txt
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      211 2023-07-25 21:09:45.000000 hxrsnd-0.3.0/hxrsnd.egg-info/requires.txt
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)        7 2023-07-25 21:09:45.000000 hxrsnd-0.3.0/hxrsnd.egg-info/top_level.txt
+drwxr-xr-x   0 klauer   (1318172782) SLAC\Domain Users (1704612529)        0 2023-07-25 21:09:45.913635 hxrsnd-0.3.0/notebooks/
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)    76846 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/notebooks/maximize_diode.ipynb
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1156 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/pyproject.toml
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)       96 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/requirements.txt
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     5548 2023-07-25 21:09:03.000000 hxrsnd-0.3.0/scripts.py
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)       38 2023-07-25 21:09:45.919238 hxrsnd-0.3.0/setup.cfg
+-rw-r--r--   0 klauer   (1318172782) SLAC\Domain Users (1704612529)      570 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/snd_devices.py
+-rwxr-xr-x   0 klauer   (1318172782) SLAC\Domain Users (1704612529)     1663 2022-06-03 18:46:07.000000 hxrsnd-0.3.0/snd_env.sh
```

### Comparing `hxrsnd-0.2.9/LICENSE.md` & `hxrsnd-0.3.0/LICENSE.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2016, The Board of Trustees of the Leland Stanford Junior
+Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
 University, through SLAC National Accelerator Laboratory (subject to receipt
 of any required approvals from the U.S. Dept. of Energy). All rights reserved.
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 (1) Redistributions of source code must retain the above copyright notice,
     this list of conditions and the following disclaimer.
```

### Comparing `hxrsnd-0.2.9/README.rst` & `hxrsnd-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.2.9/hxrsnd/aerotech.py` & `hxrsnd-0.3.0/hxrsnd/aerotech.py`

 * *Files 9% similar despite different names*

```diff
@@ -150,15 +150,15 @@
         Status : StatusObject
             Status of the set.
         """
         # Check the motor status
         if check_status:
             self.check_status()
         status = self.home_forward.set(1, timeout=self.set_timeout)
-        return self._status_print(status, "Homing '{0}' forward.".format(
+        return self._status_print(status, "Homing '{}' forward.".format(
             self.desc), print_set=print_set, ret_status=ret_status)
 
     @stop_on_keyboardinterrupt
     def homr(self, ret_status=False, print_set=True, check_status=True):
         """
         Home the motor in reverse.
 
@@ -178,15 +178,15 @@
         Status : StatusObject
             Status of the set.
         """
         # Check the motor status
         if check_status:
             self.check_status()
         status = self.home_reverse.set(1, timeout=self.set_timeout)
-        return self._status_print(status, "Homing '{0}' in reverse.".format(
+        return self._status_print(status, "Homing '{}' in reverse.".format(
             self.desc), print_set=print_set, ret_status=ret_status)
 
     def move(self, position, wait=False, check_status=True, timeout=None, *args,
              **kwargs):
         """
         Move to a specified position, optionally waiting for motion to
         complete.
@@ -226,15 +226,15 @@
 
         RuntimeError
             If motion fails other than timing out
         """
         # Check the motor status
         if check_status:
             self.check_status(position)
-        logger.debug("Moving {0} to {1}".format(self.name, position))
+        logger.debug(f"Moving {self.name} to {position}")
         return super().move(position, wait=wait, timeout=timeout, *args,
                             **kwargs)
 
     def mv(self, position, wait=True, print_move=True, *args, **kwargs):
         """
         Move to a specified position, optionally waiting for motion to
         complete. mv() is different from move() by catching all the common
@@ -278,34 +278,40 @@
         """
         try:
             status = super().mv(position, wait=wait, *args, **kwargs)
 
             # Notify the user that a motor has completed or the command is sent
             if print_move:
                 if wait:
-                    logger.info("Move completed for '{0}'.".format(self.desc))
+                    logger.info(f"Move completed for '{self.desc}'.")
                 else:
-                    logger.info(
-                        "Move command sent to '{0}'.".format(self.desc))
+                    logger.info(f"Move command sent to '{self.desc}'.")
             return status
 
         # Catch all the common motor exceptions
         except LimitError:
-            logger.warning("Requested move '{0}' is outside the soft limits "
-                           "{1} for motor {2}".format(position, self.limits,
-                                                      self.desc))
+            logger.warning(
+                "Requested move '{}' is outside the soft limits "
+                "{} for motor {}".format(position, self.limits, self.desc)
+            )
         except MotorDisabled:
-            logger.warning("Cannot move - motor {0} is currently disabled. Try "
-                           "running 'motor.enable()'.".format(self.desc))
+            logger.warning(
+                "Cannot move - motor {} is currently disabled. Try "
+                "running 'motor.enable()'.".format(self.desc)
+            )
         except MotorFaulted:
-            logger.warning("Cannot move - motor {0} is currently faulted. Try "
-                           "running 'motor.clear()'.".format(self.desc))
+            logger.warning(
+                "Cannot move - motor {} is currently faulted. Try "
+                "running 'motor.clear()'.".format(self.desc)
+            )
         except MotorStopped:
-            logger.warning("Cannot move - motor {0} is currently stopped. Try "
-                           "running 'motor.state=\"Go\"'.".format(self.desc))
+            logger.warning(
+                "Cannot move - motor {} is currently stopped. Try "
+                "running 'motor.state=\"Go\"'.".format(self.desc)
+            )
 
     def check_status(self, position=None):
         """
         Checks the status of the motor to make sure it is ready to move. Checks
         the current position of the motor, and if a position is provided it also
         checks that position.
 
@@ -322,25 +328,25 @@
         MotorFaulted
             If the motor is faulted.
 
         MotorStopped
             If the motor is stopped.
         """
         if not self.enabled:
-            err = "Motor '{0}' is currently disabled".format(self.desc)
+            err = f"Motor '{self.desc}' is currently disabled"
             logger.error(err)
             raise MotorDisabled(err)
 
         if self.faulted:
-            err = "Motor '{0}' is currently faulted.".format(self.desc)
+            err = f"Motor '{self.desc}' is currently faulted."
             logger.error(err)
             raise MotorFaulted(err)
 
         if self.state == "Stop":
-            err = "Motor '{0}' is currently stopped.".format(self.desc)
+            err = f"Motor '{self.desc}' is currently stopped."
             logger.error(err)
             raise MotorStopped(err)
 
         # Check if the current position is valid
         self.check_value(self.position)
         # Check if the move position is valid
         if position:
@@ -382,15 +388,15 @@
 
         Returns
         -------
         Status
             The status object for setting the power signal.
         """
         status = self.power.set(1, timeout=self.set_timeout)
-        return self._status_print(status, "Enabled motor '{0}'.".format(
+        return self._status_print(status, "Enabled motor '{}'.".format(
             self.desc), print_set=print_set, ret_status=ret_status)
 
     def disable(self, ret_status=False, print_set=True):
         """
         Disables the motor power.
 
         Parameters
@@ -403,15 +409,15 @@
 
         Returns
         -------
         Status
             The status object for setting the power signal.
         """
         status = self.power.set(0, timeout=self.set_timeout)
-        return self._status_print(status, "Disabled motor '{0}'.".format(
+        return self._status_print(status, "Disabled motor '{}'.".format(
             self.desc), print_set=print_set, ret_status=ret_status)
 
     @property
     def enabled(self):
         """
         Returns if the motor is curently enabled.
 
@@ -436,15 +442,15 @@
 
         Returns
         -------
         Status
             The status object for setting the clear_error signal.
         """
         status = self.clear_error.set(1, timeout=self.set_timeout)
-        return self._status_print(status, "Cleared motor '{0}'.".format(
+        return self._status_print(status, "Cleared motor '{}'.".format(
             self.desc), print_set=print_set, ret_status=ret_status)
 
     def reconfig(self, ret_status=False, print_set=True):
         """
         Re-configures the motor.
 
         Parameters
@@ -457,15 +463,15 @@
 
         Returns
         -------
         Status
             The status object for setting the config signal.
         """
         status = self.config.set(1, timeout=self.set_timeout)
-        return self._status_print(status, "Reconfigured motor '{0}'.".format(
+        return self._status_print(status, "Reconfigured motor '{}'.".format(
             self.desc), print_set=print_set, ret_status=ret_status)
 
     @property
     def faulted(self):
         """
         Returns the current fault with the motor.
 
@@ -493,15 +499,15 @@
 
         Returns
         -------
         status : StatusObject
             Status object for the set.
         """
         status = self.zero_all_proc.set(1, timeout=self.set_timeout)
-        return self._status_print(status, "Zeroed motor '{0}'.".format(
+        return self._status_print(status, "Zeroed motor '{}'.".format(
             self.desc), print_set=print_set, ret_status=ret_status)
 
     @property
     def state(self):
         """
         Returns the state of the motor. State can be one of the following:
             'Stop', 'Pause', 'Move', 'Go'
@@ -535,15 +541,15 @@
         -------
         Status
             The status object for setting the state signal.
         """
         try:
             return self.set_state(val, ret_status, print_set)
         except ValueError:
-            logger.info("State must be one of the following: {0}".format(
+            logger.info("State must be one of the following: {}".format(
                 self._state_list))
 
     def set_state(self, state, ret_status=True, print_set=False):
         """
         Sets the state of the motor. Inputted state can be one of the following
         states or the index of the desired state:
             'Stop', 'Pause', 'Move', 'Go'
@@ -566,23 +572,23 @@
         # Make sure it is in title case if it's a string
         val = state
         if isinstance(state, str):
             val = state.title()
 
         # Make sure it is a valid state or enum
         if val not in self._state_list + list(range(len(self._state_list))):
-            error = "Invalid state inputted: '{0}'.".format(val)
+            error = f"Invalid state inputted: '{val}'."
             logger.error(error)
             raise ValueError(error)
 
         # Lets enforce it's a string or value
         status = self.state_component.set(val, timeout=self.set_timeout)
 
         return self._status_print(
-            status, "Changed state of '{0} to '{1}'.".format(self.desc, val),
+            status, f"Changed state of '{self.desc} to '{val}'.",
             print_set=print_set, ret_status=ret_status)
 
     def ready_motor(self, ret_status=False, print_set=True):
         """
         Sets the motor to the ready state by clearing any errors, enabling it,
         and setting the state to be 'Go'.
 
@@ -599,15 +605,15 @@
         Status
             The status object for all the sets.
         """
         status = [self.clear(ret_status=True, print_set=False)]
         status.append(self.enable(ret_status=True, print_set=False))
         status.append(self.set_state("Go", ret_status=True, print_set=False))
         return self._status_print(
-            status, "Motor '{0}' is now ready to move.".format(self.desc),
+            status, f"Motor '{self.desc}' is now ready to move.",
             print_set=print_set, ret_status=ret_status)
 
     def expert_screen(self, print_msg=True):
         """
         Launches the expert screen for the motor.
 
         Parameters
@@ -615,15 +621,15 @@
         print_msg : bool, optional
             Prints that the screen is being launched.
         """
         path = absolute_submodule_path(
             "hxrsnd/screens/motor_expert_screens.sh")
         if print_msg:
             logger.info("Launching expert screen.")
-        os.system("{0} {1} {2} &".format(path, self.prefix, "aerotech"))
+        os.system("{} {} {} &".format(path, self.prefix, "aerotech"))
 
     def status(self, status="", offset=0, print_status=True, newline=False,
                short=False):
         """
         Returns the status of the device.
 
         Parameters
@@ -642,33 +648,36 @@
 
         Returns
         -------
         status : str
             Status string.
         """
         if short:
-            status += "\n{0}{1:<16}|{2:^16.3f}|{3:^16.3f}".format(
-                " "*offset, self.desc, self.position, self.dial.get())
+            status += "\n{}{:<16}|{:^16.3f}|{:^16.3f}".format(
+                " " * offset, self.desc, self.position, self.dial.get()
+            )
         else:
-            status += "{0}{1}\n".format(" "*offset, self.desc)
-            status += "{0}PV: {1:>25}\n".format(" "*(offset+2), self.prefix)
-            status += "{0}Enabled: {1:>20}\n".format(" "*(offset+2),
-                                                     str(self.enabled))
-            status += "{0}Faulted: {1:>20}\n".format(" "*(offset+2),
-                                                     str(self.faulted))
-            status += "{0}State: {1:>22}\n".format(" "*(offset+2),
-                                                   str(self.state))
-            status += "{0}Position: {1:>19}\n".format(" "*(offset+2),
-                                                      np.round(self.wm(), 6))
-            status += "{0}Dial: {1:>23}\n".format(" "*(offset+2),
-                                                  np.round(self.dial.get(),
-                                                           6))
-            status += "{0}Limits: {1:>21}\n".format(
-                " "*(offset+2), str((int(self.low_limit),
-                                     int(self.high_limit))))
+            status += "{}{}\n".format(" " * offset, self.desc)
+            status += "{}PV: {:>25}\n".format(" " * (offset + 2), self.prefix)
+            status += "{}Enabled: {:>20}\n".format(
+                " " * (offset + 2), str(self.enabled)
+            )
+            status += "{}Faulted: {:>20}\n".format(
+                " " * (offset + 2), str(self.faulted)
+            )
+            status += "{}State: {:>22}\n".format(" " * (offset + 2), str(self.state))
+            status += "{}Position: {:>19}\n".format(
+                " " * (offset + 2), np.round(self.wm(), 6)
+            )
+            status += "{}Dial: {:>23}\n".format(
+                " " * (offset + 2), np.round(self.dial.get(), 6)
+            )
+            status += "{}Limits: {:>21}\n".format(
+                " " * (offset + 2), str((int(self.low_limit), int(self.high_limit)))
+            )
 
         if newline:
             status += "\n"
         if print_status is True:
             logger.info(status)
         else:
             return status
@@ -708,15 +717,15 @@
         MotorStopped
             If the motor is stopped.
 
         BadN2Pressure
             If the pressure in the tower is bad.
         """
         if self._pressure.bad:
-            err = "Cannot move - Pressure in {0} is bad.".format(self._tower)
+            err = f"Cannot move - Pressure in {self._tower} is bad."
             logger.error(err)
             raise BadN2Pressure(err)
         super().check_status(*args, **kwargs)
 
     def mv(self, position, *args, **kwargs):
         """
         Move to a specified position, optionally waiting for motion to
@@ -766,15 +775,15 @@
         status : MoveStatus
             Status object for the move.
         """
         try:
             return self.move(position, *args, **kwargs)
         # Catch a bad pressure setting.
         except BadN2Pressure:
-            logger.warning("Cannot move - pressure in tower {0} is bad.".format(
+            logger.warning("Cannot move - pressure in tower {} is bad.".format(
                 self._tower))
 
 
 class LinearAero(AeroBase):
     """
     Class for the aerotech linear stage.
     """
```

### Comparing `hxrsnd-0.2.9/hxrsnd/attocube.py` & `hxrsnd-0.3.0/hxrsnd/attocube.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     _flash = Cmp(EpicsSignal, ":RDB:FLASH", write_pv=":CMD:FLASH")
 
     @property
     def firmware(self):
         """
         Returns the firmware in the same date format as the EDM screen.
         """
-        return "{0}/{1}/{2}".format(
+        return "{}/{}/{}".format(
             self._firm_day.get(), self._firm_month.get(), self._firm_year.get())
 
     @property
     def flash(self):
         """
         Saves the current configuration of the controller.
         """
@@ -207,15 +207,15 @@
 
         Returns
         -------
         Status
             The status object for setting the power signal.
         """
         status = self.motor_enable.set(1, timeout=self.set_timeout)
-        return self._status_print(status, "Enabled motor '{0}'".format(
+        return self._status_print(status, "Enabled motor '{}'".format(
             self.desc), ret_status=ret_status, print_set=print_set)
 
     def disable(self, ret_status=False, print_set=True):
         """
         Disables the motor power.
 
         Parameters
@@ -228,15 +228,15 @@
 
         Returns
         -------
         Status
             The status object for setting the power signal.
         """
         status = self.motor_enable.set(0, timeout=self.set_timeout)
-        return self._status_print(status, "Disabled motor '{0}'".format(
+        return self._status_print(status, "Disabled motor '{}'".format(
             self.desc), ret_status=ret_status, print_set=print_set)
 
     @property
     def enabled(self):
         """
         Returns if the motor is curently enabled.
 
@@ -289,15 +289,15 @@
 
         Returns
         -------
         status : StatusObject
             Status object for the set.
         """
         status = self.motor_reset.set(1, timeout=self.set_timeout)
-        return self._status_print(status, "Reset motor '{0}'".format(
+        return self._status_print(status, "Reset motor '{}'".format(
             self.desc), ret_status=ret_status, print_set=print_set)
 
     def move(self, position, check_status=True, timeout=None, *args, **kwargs):
         """
         Move to a specified position.
 
         Parameters
@@ -323,15 +323,15 @@
 
         RuntimeError
             If motion fails other than timing out
         """
         # Check the motor status
         if check_status:
             self.check_status(position)
-        logger.debug("Moving {0} to {1}".format(self.name, position))
+        logger.debug(f"Moving {self.name} to {position}")
         # Begin the move process
         return self.user_setpoint.set(position, timeout=timeout)
 
     def mv(self, position, print_move=True, wait=None,
            *args, **kwargs):
         """
         Move to a specified position, optionally waiting for motion to
@@ -366,29 +366,34 @@
             Status object for the move.
         """
         try:
             status = super().mv(position, *args, **kwargs)
 
             # Notify the user that a motor has completed or the command is sent
             if print_move:
-                logger.info("Move command sent to '{0}'.".format(self.desc))
+                logger.info(f"Move command sent to '{self.desc}'.")
             # Check if a status object is desired
             return status
 
         # Catch all the common motor exceptions
         except LimitError:
-            logger.warning("Requested move '{0}' is outside the soft limits "
-                           "{1} for motor {2}".format(position, self.limits,
-                                                      self.desc))
+            logger.warning(
+                "Requested move '{}' is outside the soft limits "
+                "{} for motor {}".format(position, self.limits, self.desc)
+            )
         except MotorDisabled:
-            logger.warning("Cannot move - motor {0} is currently disabled. Try "
-                           "running 'motor.enable()'.".format(self.desc))
+            logger.warning(
+                "Cannot move - motor {} is currently disabled. Try "
+                "running 'motor.enable()'.".format(self.desc)
+            )
         except MotorFaulted:
-            logger.warning("Cannot move - motor {0} is currently faulted. Try "
-                           "running 'motor.clear()'.".format(self.desc))
+            logger.warning(
+                "Cannot move - motor {} is currently faulted. Try "
+                "running 'motor.clear()'.".format(self.desc)
+            )
 
     def check_status(self, position=None):
         """
         Checks the status of the motor to make sure it is ready to move. Checks
         the current position of the motor, and if a position is provided it also
         checks that position.
 
@@ -402,20 +407,20 @@
         MotorDisabled
             If the motor is disabled.
 
         MotorError
             If the motor has an error.
         """
         if not self.enabled:
-            err = "Motor '{0}' is currently disabled.".format(self.desc)
+            err = f"Motor '{self.desc}' is currently disabled."
             logger.error(err)
             raise MotorDisabled(err)
 
         if self.error:
-            err = "Motor '{0}' currently has an error.".format(self.desc)
+            err = f"Motor '{self.desc}' currently has an error."
             logger.error(err)
             raise MotorError(err)
 
         # Check if the current position is valid
         self.check_value(self.position)
         # Check if the move position is valid
         if position:
@@ -435,20 +440,20 @@
         ValueError
             If position is None, NaN or Inf
         LimitError
             If the position is outside the soft limits.
         """
         # Check for invalid positions
         if position is None or np.isnan(position) or np.isinf(position):
-            raise ValueError("Invalid value inputted: '{0}'".format(position))
+            raise ValueError(f"Invalid value inputted: '{position}'")
 
         # Check if it is within the soft limits
         if not (self.low_limit <= position <= self.high_limit):
             err_str = (
-                "Requested value {0} outside of range: [{1}, {2}]"
+                "Requested value {} outside of range: [{}, {}]"
                 "".format(position, self.low_limit, self.high_limit)
             )
             logger.warn(err_str)
             raise LimitError(err_str)
 
     def stop(self, success=False, ret_status=False, print_set=True):
         """
@@ -465,15 +470,15 @@
         Returns
         -------
         Status : StatusObject
             Status of the set.
         """
         status = self.motor_stop.set(1, wait=False, timeout=self.set_timeout)
         super().stop(success=success)
-        return self._status_print(status, "Stopped motor '{0}'".format(
+        return self._status_print(status, "Stopped motor '{}'".format(
             self.desc), ret_status=ret_status, print_set=print_set)
 
     def expert_screen(self, print_msg=True):
         """
         Launches the expert screen for the motor.
 
         Parameters
@@ -482,15 +487,15 @@
             Prints that the screen is being launched.
         """
         # Get the absolute path to the screen
         path = absolute_submodule_path(
             "hxrsnd/screens/motor_expert_screens.sh")
         if print_msg:
             logger.info("Launching expert screen.")
-        os.system("{0} {1} {2} &".format(path, self.prefix, "attocube"))
+        os.system("{} {} {} &".format(path, self.prefix, "attocube"))
 
     def set_limits(self, llm, hlm):
         """
         Sets the limits of the motor. Alias for limits = (llm, hlm).
 
         Parameters
         ----------
@@ -578,27 +583,30 @@
 
         Returns
         -------
         status : str
             Status string.
         """
         if short:
-            status += "\n{0}{1:<16}|{2:^16.3f}|{3:^16.3f}".format(
-                " "*offset, self.desc, self.position, self.reference)
+            status += "\n{}{:<16}|{:^16.3f}|{:^16.3f}".format(
+                " " * offset, self.desc, self.position, self.reference
+            )
         else:
-            status += "{0}{1}\n".format(" "*offset, self.desc)
-            status += "{0}PV: {1:>25}\n".format(" "*(offset+2), self.prefix)
-            status += "{0}Enabled: {1:>20}\n".format(" "*(offset+2),
-                                                     str(self.enabled))
-            status += "{0}Faulted: {1:>20}\n".format(" "*(offset+2),
-                                                     str(self.error))
-            status += "{0}Position: {1:>19}\n".format(" "*(offset+2),
-                                                      np.round(self.wm(), 6))
-            status += "{0}Limits: {1:>21}\n".format(
-                " "*(offset+2), str((int(self.low_limit), int(self.high_limit))))
+            status += "{}{}\n".format(" " * offset, self.desc)
+            status += "{}PV: {:>25}\n".format(" " * (offset + 2), self.prefix)
+            status += "{}Enabled: {:>20}\n".format(
+                " " * (offset + 2), str(self.enabled)
+            )
+            status += "{}Faulted: {:>20}\n".format(" " * (offset + 2), str(self.error))
+            status += "{}Position: {:>19}\n".format(
+                " " * (offset + 2), np.round(self.wm(), 6)
+            )
+            status += "{}Limits: {:>21}\n".format(
+                " " * (offset + 2), str((int(self.low_limit), int(self.high_limit)))
+            )
         if newline:
             status += "\n"
         if print_status is True:
             logger.info(status)
         else:
             return status
```

### Comparing `hxrsnd-0.2.9/hxrsnd/bragg.py` & `hxrsnd-0.3.0/hxrsnd/bragg.py`

 * *Files 4% similar despite different names*

```diff
@@ -173,15 +173,15 @@
         E = E
     else:
         E = eV(E)
     lam = (12398.4/E)/u['ang']
     return lam
 
 
-def lam2E(l):
+def lam2E(l):  # noqa: E741
     """
     Computes photon energy in eV
 
     Parameters
     ----------
     l : float
         Photon wavelength in m
@@ -191,15 +191,15 @@
     E : float
         Energy in eV
     """
     E = 12398.4/(l*u['ang'])
     return E
 
 
-def lam2f(l):
+def lam2f(l):  # noqa: E741
     """
     Computes the photon frequency in Hz
 
     Parameters
     ----------
     l : float
         Photon wavelength in m
@@ -298,15 +298,15 @@
     -------
     d : float
         The d-spacing of the crystal using the inputted reflection.
     """
     ID = check_id(ID)
     h = hkl[0]
     k = hkl[1]
-    l = hkl[2]
+    l_ = hkl[2]
 
     lp = lattice_parameters[ID]
     a = lp[0]/u['ang']
     b = lp[1]/u['ang']
     c = lp[2]/u['ang']
     alpha = lp[3]
     beta = lp[4]
@@ -316,16 +316,16 @@
     cb = cosd(beta)
     cg = cosd(gamma)
     sa = sind(alpha)
     sb = sind(beta)
     sg = sind(gamma)
 
     invdsqr = 1 / (1.+2.*ca*cb*cg-ca**2.-cb**2.-cg**2.) * \
-        (h**2.*sa**2./a**2. + k**2.*sb**2./b**2. + l**2.*sg**2./c**2. +
-         2.*h*k*(ca*cb-cg)/a/b+2.*k*l*(cb*cg-ca)/b/c+2.*h*l*(ca*cg-cb)/a/c)
+        (h**2.*sa**2./a**2. + k**2.*sb**2./b**2. + l_**2.*sg**2./c**2. +
+         2.*h*k*(ca*cb-cg)/a/b+2.*k*l_*(cb*cg-ca)/b/c+2.*h*l_*(ca*cg-cb)/a/c)
 
     d = invdsqr**-0.5
     return d
 
 
 def bragg_angle(E=None, ID="Si", hkl=(2, 2, 0)):
     """
@@ -374,16 +374,16 @@
     Returns
     -------
     E : float, optional
         Photon energy in eV
     """
     ID = check_id(ID)
     d = d_space(ID, hkl)
-    l = 2*d*sind(theta)
-    E = lam2E(l)
+    l_ = 2*d*sind(theta)
+    E = lam2E(l_)
     return E
 
 
 def snd_L(E1, E2, delay, gap=55):
     """
     Calculates the theta angles of the towers and the delay length based on the
     desired energy and delay.
@@ -415,18 +415,18 @@
     """
     cl = 0.3
     theta_L = bragg_angle('Si', (2, 2, 0), E1)
     theta_cc = bragg_angle('Si', (2, 2, 0), E2)
     # gap is the distance between the two faces of the channel cut crystal
     L = (delay*cl/2.+gap*(1-cosd(2*theta_cc))/sind(theta_cc))/(1-cosd(
         2*theta_L))
-    logger.info("t1.L = t4.L = {} mm".format(L))
-    logger.info("t1.tth = t4.tth = {} degree".format(2*theta_L))
-    logger.info("t1.th1=t1.th2=t4.th1=t4.th2 = {} degree".format(theta_L))
-    logger.info("t2.th=t3.th = {} degree".format(theta_cc))
+    logger.info(f"t1.L = t4.L = {L} mm")
+    logger.info(f"t1.tth = t4.tth = {2*theta_L} degree")
+    logger.info(f"t1.th1=t1.th2=t4.th1=t4.th2 = {theta_L} degree")
+    logger.info(f"t2.th=t3.th = {theta_cc} degree")
     return theta_L, theta_cc, L
 
 
 def snd_diag(E1, E2, delay, gap=55):
     """
     Calculates the positions of the middle diagnostics of the system based on
     the inputted energy and delay.
@@ -457,16 +457,16 @@
     # speed of light
     theta_L = bragg_angle('Si', (2, 2, 0), E1)
     theta_cc = bragg_angle('Si', (2, 2, 0), E2)
     dcc_x = 2*cosd(theta_cc)*gap
     L = (delay*cl/2.+gap*(1-cosd(2*theta_cc))/sind(theta_cc))/(1-cosd(
         2*theta_L))
     dd_x = -L*sind(2*theta_L)
-    logger.info("dd.x = {}".format(dd_x))
-    logger.info("dcc.x = {}".format(dcc_x))
+    logger.info(f"dd.x = {dd_x}")
+    logger.info(f"dcc.x = {dcc_x}")
     return dd_x, dcc_x
 
 
 def snd_delay(E1, E2, L, gap=55):
     """
     Calculates the delay of the system based on the inputted energies and the
     delay length.
```

### Comparing `hxrsnd-0.2.9/hxrsnd/diode.py` & `hxrsnd-0.3.0/hxrsnd/diode.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
         -------
         status : MoveStatus
             Status object for the move.
         """
         # Move to the blocked position if we aren't already there
         if self.blocked is True:
             # We are already in the blocked position
-            logger.info("Motor '{0}' is currently in the blocked position"
+            logger.info("Motor '{}' is currently in the blocked position"
                         "".format(self.x.desc))
         else:
             return self.x.mv(self.pos_func() + self.block_pos, *args, **kwargs)
 
     def unblock(self, *args, **kwargs):
         """
         Moves the diode by the nonblocking position defined by the position
@@ -205,15 +205,15 @@
         -------
         status : MoveStatus
             Status object for the move.
         """
         # Move to the blocked position if we aren't already there
         if self.blocked is False:
             # We are already in the blocked position
-            logger.info("Motor '{0}' is currently in the unblocked position"
+            logger.info("Motor '{}' is currently in the unblocked position"
                         "".format(self.x.desc))
         else:
             return self.x.mv(self.pos_func(), *args, **kwargs)
 
 
 class DiodeIO(SndDevice):
     """
```

### Comparing `hxrsnd-0.2.9/hxrsnd/exceptions.py` & `hxrsnd-0.3.0/hxrsnd/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 """
 Exceptions for the SnD system.
 """
 
 import logging
 
 logger = logging.getLogger(__name__)
```

### Comparing `hxrsnd-0.2.9/hxrsnd/macromotor.py` & `hxrsnd-0.3.0/hxrsnd/macromotor.py`

 * *Files 2% similar despite different names*

```diff
@@ -312,24 +312,24 @@
                 self.verify_move = verify_move
 
             return super().mv(position, wait=wait, *args, **kwargs)
         # Catch all the common motor exceptions
         except LimitError:
             logger.warning("Requested move is outside the soft limits")
         except MotorDisabled:
-            logger.warning("Cannot move '{0}' - a motor is currently disabled. "
+            logger.warning("Cannot move '{}' - a motor is currently disabled. "
                            "Try running 'motor.enable()'.".format(self.desc))
         except MotorFaulted:
-            logger.warning("Cannot move '{0}' - a motor is currently faulted. "
+            logger.warning("Cannot move '{}' - a motor is currently faulted. "
                            "Try running 'motor.clear()'.".format(self.desc))
         except MotorStopped:
-            logger.warning("Cannot move '{0}' - a motor is currently stopped. "
+            logger.warning("Cannot move '{}' - a motor is currently stopped. "
                            "Try running 'motor.state='Go''.".format(self.desc))
         except BadN2Pressure:
-            logger.warning("Cannot move '{0}' - pressure in a tower is bad."
+            logger.warning("Cannot move '{}' - pressure in a tower is bad."
                            "".format(self.desc))
         finally:
             if use_diag is not _UNSET:
                 self.use_diag = old_use_diag
             if verify_move is not _UNSET:
                 self.verify_move = old_verify_move
 
@@ -358,15 +358,15 @@
         string : str
             Message to be printed to user.
         """
         logger.info(string)
         try:
             response = input("\nConfirm Move [y/n]: ")
         except Exception as e:
-            logger.info("Exception raised: {0}".format(e))
+            logger.info(f"Exception raised: {e}")
             response = "n"
 
         if response.lower() != "y":
             logger.info("\nMove cancelled.")
             return True
         else:
             logger.debug("\nMove confirmed.")
@@ -384,20 +384,20 @@
         offset : int, optional
             Amount to offset each line of the status.
 
         print_status : bool, optional
             Determines whether the string is printed or returned.
         """
         try:
-            status += "\n{0}{1:<16} {2:^16}".format(
+            status += "\n{}{:<16} {:^16}".format(
                 " "*offset,
                 self.desc+":",
                 self.position)
         except TypeError:
-            status += "\n{0}{1:<16} {2:^}".format(
+            status += "\n{}{:<16} {:^}".format(
                 " "*offset,
                 self.desc+":",
                 str(self.position))
 
         if newline:
             status += "\n"
         if print_status:
@@ -687,15 +687,15 @@
         # Get the desired length for the delay stage
         length = self._delay_to_length(delay)
 
         # Move the delay stages
         status = [tower.set_length(length, wait=False, check_status=False)
                   for tower in self._delay_towers]
         # Log the delay change
-        logger.debug("Setting delay to {0}.".format(delay))
+        logger.debug(f"Setting delay to {delay}.")
 
         if use_diag:
             # Move the delay diagnostic to the inputted position
             status += [self.parent.dd.x.move(position_dd, wait=False)]
 
         # Perform the compensation
         if self.has_calib and self.use_calib:
@@ -751,15 +751,15 @@
 
         # Diagnostic
         if use_diag:
             position_dd = self._get_delay_diagnostic_position(delay=delay)
             self.parent.dd.x.set_position(position_dd, print_set=False)
 
         if print_set:
-            logger.info("Setting positions for delay to {0}.".format(delay))
+            logger.info(f"Setting positions for delay to {delay}.")
 
 
 class Energy1Macro(DelayTowerMacro):
     """
     Macro-motor for the energy 1 macro-motor.
     """
     # @property
@@ -942,15 +942,15 @@
         """
         use_diag = use_diag if use_diag is not _UNSET else self.use_diag
 
         # Move the towers to the specified energy
         status = [tower.set_energy(E1, wait=False, check_status=False) for
                   tower in self._delay_towers]
         # Log the energy change
-        logger.debug("Setting E1 to {0}.".format(E1))
+        logger.debug(f"Setting E1 to {E1}.")
 
         # Move the delay diagnostic to the inputted position
         if use_diag:
             status += [self.parent.dd.x.move(position_dd, wait=False)]
 
         return status
 
@@ -1026,15 +1026,15 @@
         # Set the diagnostic
         if use_diag:
             position_dd = self._get_delay_diagnostic_position(E1=E1)
             self.parent.dd.x.set_position(position_dd, print_set=False)
 
         # Log the set
         if print_set is True:
-            logger.info("Setting positions for E1 to {0}.".format(E1))
+            logger.info(f"Setting positions for E1 to {E1}.")
 
 
 class Energy1CCMacro(Energy1Macro):
     """
     Macro-motor for the energy 1 channel cut macro-motor.
     """
 
@@ -1157,15 +1157,15 @@
         """
         use_diag = use_diag if use_diag is not _UNSET else self.use_diag
         # Move the towers to the specified energy
         status = [tower.tth.move(2*bragg_angle(E1), wait=False,
                                  check_status=False)
                   for tower in self._delay_towers]
         # Log the energy change
-        logger.debug("Setting E1_cc to {0}.".format(E1))
+        logger.debug(f"Setting E1_cc to {E1}.")
 
         # Move the delay diagnostic to the inputted position
         if use_diag:
             status += [self.parent.dd.x.move(position_dd, wait=False)]
 
         return status
 
@@ -1205,15 +1205,15 @@
         # Set the diagnostic
         if use_diag:
             position_dd = self._get_delay_diagnostic_position(E1=E1)
             self.parent.dd.x.set_position(position_dd, print_set=False)
 
         # Log the set
         if print_set is True:
-            logger.info("Setting positions for E1 to {0}.".format(E1))
+            logger.info(f"Setting positions for E1 to {E1}.")
 
 
 class Energy2Macro(MacroBase):
     """
     Macro-motor for the energy 2 macro-motor.
     """
 
@@ -1398,15 +1398,15 @@
         # Move the channel cut towers
         status += [tower.set_energy(E2, wait=False, check_status=False) for
                    tower in self._channelcut_towers]
         # Move the channel cut diagnostics
         if use_diag:
             status += [self.parent.dcc.x.move(position_dcc, wait=False)]
         # Log the energy change
-        logger.debug("Setting E2 to {0}.".format(E2))
+        logger.debug(f"Setting E2 to {E2}.")
 
         return status
 
     @property
     @nan_if_no_parent
     def position(self):
         """
@@ -1456,8 +1456,8 @@
 
         # Move the cc diagnostic as well
         position_dcc = self._get_channelcut_diagnostic_position(E2)
         self.parent.dcc.x.set_position(position_dcc, print_set=False)
 
         # Log the set
         if print_set is True:
-            logger.info("Setting positions for E2 to {0}.".format(E2))
+            logger.info(f"Setting positions for E2 to {E2}.")
```

### Comparing `hxrsnd-0.2.9/hxrsnd/plans/alignment.py` & `hxrsnd-0.3.0/hxrsnd/plans/alignment.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.2.9/hxrsnd/plans/calibration.py` & `hxrsnd-0.3.0/hxrsnd/plans/calibration.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                        "existing calibration.")
         # If a calibration is loaded, prompt the user for verification
         if confirm_overwrite:
             # Prompt the user about the move before making it
             try:
                 response = input("\nConfirm Overwrite [y/n]: ")
             except Exception as e:
-                logger.warning("Exception raised: {0}".format(e))
+                logger.warning(f"Exception raised: {e}")
                 response = "n"
             if response.lower() != "y":
                 logger.info("\nCalibration cancelled.")
                 return
             logger.debug("\nOverwrite confirmed.")
 
     # Perform the calibration scan
@@ -262,15 +262,15 @@
         length as the number of calibration fields.
     """
     calib_fields = as_list(calib_fields or [m.name for m in calib_motors])
 
     # Make sure the same number of calibration fields as motors are passed
     if len(calib_motors) != len(calib_fields):
         raise ValueError("Must one calibration field for every calibration "
-                         "motor, but got {0} fields for {1} motors.".format(
+                         "motor, but got {} fields for {} motors.".format(
                              len(calib_fields), len(calib_motors)))
 
     # Perform the main scan, correctly passing the calibration parameters
     df = yield from centroid_scan(
         detector, motor, start, stop, steps, *args, system=calib_motors,
         system_fields=calib_fields, return_to_start=False, **kwargs
     )
@@ -338,15 +338,15 @@
     start_positions : list
         List of the initial positions of the motors before the walk
     """
     detector_fields = [col for col in df_scan.columns if detector.name in col]
     calib_fields = [col[:-4] for col in df_scan.columns if col.endswith("_pre")]
     if len(detector_fields) != len(calib_fields):
         raise ValueError("Must have same number of calibration fields as "
-                         "detector fields, but got {0} and {1}.".format(
+                         "detector fields, but got {} and {}.".format(
                              len(calib_fields), len(detector_fields)))
 
     # Perform all the initial necessities
     num = len(detector_fields)
     average = average or 1
     calib_motors = as_list(calib_motors)
     first_step = as_list(first_step, num, float)
@@ -375,32 +375,32 @@
 
         # Get the farthest detector value we know we can move to from the
         # current position
         idx_max = abs(df_scan[dfld] - dfld_start).values.argmax()
 
         # Walk the cmotor to the first pre-correction detector entry
         try:
-            logger.debug("Beginning walk to {0} on {1} using {2}".format(
+            logger.debug("Beginning walk to {} on {} using {}".format(
                 df_scan.iloc[idx_max][dfld], detector.name, cmotor.name))
             yield from walk_to_pixel(
                 detector, cmotor, df_scan.iloc[idx_max][dfld], *args,
                 filters=filters, gradient=gradients[i],
                 target_fields=[dfld, cfld],
                 first_step=first_step[i], tolerance=tolerance[i],
                 system=inp_system, average=average, max_steps=max_steps[i],
                 **kwargs
             )
 
         except RuntimeError:
-            logger.warning("walk_to_pixel raised a RuntimeError for motor '{0}'"
-                           ". Using its current position {1} for scale "
+            logger.warning("walk_to_pixel raised a RuntimeError for motor '{}'"
+                           ". Using its current position {} for scale "
                            "calulation.".format(cmotor.desc, cmotor.position))
         except LimitError:
             logger.warning("walk_to_pixel tried to exceed the limits of motor "
-                           "'{0}'. Using current position '{1}' for scale "
+                           "'{}'. Using current position '{}' for scale "
                            "calculation.".format(cmotor.desc, cmotor.position))
 
         # Get the positions and values we moved to
         reads = (yield from measure_average([detector]+system,
                                             num=average,
                                             filters=filters))
         motor_end = reads[cfld]
@@ -450,15 +450,15 @@
     calib_fields = [col[:-4] for col in df_scan.columns if col.endswith("_pre")]
     motor_fields = [col for col in df_scan.columns
                     if col not in detector_fields and not col.endswith("_pre")]
 
     # Ensure these two are equal
     if len(detector_fields) != len(calib_fields):
         raise ValueError("Must have same number of calibration fields as "
-                         "detector fields, but got {0} and {1}.".format(
+                         "detector fields, but got {} and {}.".format(
                              len(calib_fields), len(detector_fields)))
 
     df_corrections = pd.DataFrame(index=df_scan.index)
 
     # Use the conversion to create an expected correction table
     for scale, start, cfld, dfld in zip(scaling, start_positions, calib_fields,
                                         detector_fields):
```

### Comparing `hxrsnd-0.2.9/hxrsnd/plans/plan_stubs.py` & `hxrsnd-0.3.0/hxrsnd/plans/plan_stubs.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     # Get the full detector fields
     prep_dev_fields = [field_prepend(fld, device) for fld in device_fields]
 
     # Make sure the number of device fields and targets is the same
     if len(device_fields) != len(targets):
         raise ValueError(
             "Number of device fields and targets must be the same."
-            "Got {0} and {1}".format(len(device_fields), len(targets))
+            "Got {} and {}".format(len(device_fields), len(targets))
         )
     # Measure the average
     read = (yield from measure_average([device], num=average, filters=filters))
     # Get the squared differences between the centroids
     squared_differences = [(read[fld]-target)**2 for fld, target in zip(
         prep_dev_fields, targets)]
     # Combine into euclidean distance
```

### Comparing `hxrsnd-0.2.9/hxrsnd/plans/preprocessors.py` & `hxrsnd-0.3.0/hxrsnd/plans/preprocessors.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.2.9/hxrsnd/plans/scans.py` & `hxrsnd-0.3.0/hxrsnd/plans/scans.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,24 +73,24 @@
 
     # Define the inner scan
     # @stage_decorator([motor])
     @run_decorator(md=_md)
     def inner_scan():
 
         for i, step in enumerate(steps):
-            logger.info("\nStep {0}: Moving to {1}".format(i+1, step))
+            logger.info(f"\nStep {i+1}: Moving to {step}")
             grp = _short_uid('set')
             yield Msg('checkpoint')
             # Set wait to be false in set once the status object is implemented
             yield Msg('set', motor, step, group=grp, *args, **kwargs)
             yield Msg('wait', None, group=grp)
             yield from trigger_and_read([motor])
 
         if return_to_start:
-            logger.info("\nScan complete. Moving back to starting position: {0}"
+            logger.info("\nScan complete. Moving back to starting position: {}"
                         "\n".format(start))
             yield Msg('set', motor, start, group=grp, *args, **kwargs)
             yield Msg('wait', None, group=grp)
 
     return (yield from inner_scan())
 
 
@@ -168,15 +168,15 @@
     # Build the dataframe with the centroids
     df = pd.DataFrame(columns=all_fields, index=np.linspace(start, stop, steps))
 
     # Create a basic measuring plan
     def per_step(detectors, motor, step):
         # Perform step
         yield from checkpoint()
-        logger.debug("Measuring average at step {0} ...".format(step))
+        logger.debug(f"Measuring average at step {step} ...")
         yield from abs_set(motor, step, wait=True)
         # Measure the average
         reads = (yield from measure_average(all_devices, num=average,
                                             filters=filters, *args, **kwargs))
         # Fill the dataframe at this step with the centroid difference
         for fld in all_fields:
             df.loc[step, fld] = reads[fld]
```

### Comparing `hxrsnd-0.2.9/hxrsnd/pneumatic.py` & `hxrsnd-0.3.0/hxrsnd/pneumatic.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,16 +37,17 @@
             Adds a new line to the end of the string.
 
         Returns
         -------
         status : str
             Status string.
         """
-        status += "{0}{1:<16}|{2:^16}\n".format(" "*offset, self.desc+"",
-                                                self.position)
+        status += "{}{:<16}|{:^16}\n".format(
+            " " * offset, self.desc + "", self.position
+        )
         if newline:
             status += "\n"
         if print_status is True:
             logger.info(status)
         else:
             return status
 
@@ -249,15 +250,15 @@
             Adds a new line to the end of the string.
 
         Returns
         -------
         status : str
             Status string.
         """
-        status += "\n{0}Pneumatics".format(" "*offset)
+        status += "\n{}Pneumatics".format(" "*offset)
         status += "\n{0}{1}\n{0}{2:^16}|{3:^16}\n{0}{4}\n".format(
             " "*(offset+2), "-"*34, "Device", "State", "-"*34)
         for valve in self._valves:
             status += valve.status(offset=offset+2, print_status=False)
         for pressure in self._pressure_switches:
             status += pressure.status(offset=offset+2, print_status=False)
```

### Comparing `hxrsnd-0.2.9/hxrsnd/screens/diode.ui` & `hxrsnd-0.3.0/hxrsnd/screens/diode.ui`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.2.9/hxrsnd/screens/motor_expert_screens.sh` & `hxrsnd-0.3.0/hxrsnd/screens/motor_expert_screens.sh`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.2.9/hxrsnd/screens/snd_main` & `hxrsnd-0.3.0/hxrsnd/screens/snd_main`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.2.9/hxrsnd/sequencer.py` & `hxrsnd-0.3.0/hxrsnd/sequencer.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.2.9/hxrsnd/snddevice.py` & `hxrsnd-0.3.0/hxrsnd/snddevice.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.2.9/hxrsnd/sndmotor.py` & `hxrsnd-0.3.0/hxrsnd/sndmotor.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,26 +290,26 @@
         if calib is None:
             pass
 
         # We have a correction table but it isnt a Dataframe
         elif not isinstance(calib, pd.DataFrame):
             raise TypeError("Only Dataframes are supported for calibrations "
                             "tables at this time. Got a calibration of type "
-                            "{0}.".format(type(calib)))
+                            "{}.".format(type(calib)))
 
         # We have a correction table but no motors to correct with
         elif not motors:
             raise InputError("Inputted a correction table with no calibration "
                              "motors.")
 
         # We have a correction table and calibration motors, but they arent the
         # same length, so we cannot actually use it
         elif len(calib.columns) != len(motors):
             raise InputError("Mismatched calibration size and number of "
-                             "motors. Got {0} columns for {1} motors.".format(
+                             "motors. Got {} columns for {} motors.".format(
                                  len(calib.columns), len(motors)))
 
         # We have the correct correction table and motors but one of the of the
         # extra parameters were not passed, which is critical for corrected
         # motions but warn the user
         elif scan is None or not scale or not start:
             logger.warning("Inputted correction table and calibration motors "
```

### Comparing `hxrsnd-0.2.9/hxrsnd/sndsystem.py` & `hxrsnd-0.3.0/hxrsnd/sndsystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,18 +117,18 @@
             self.E2._get_channelcut_diagnostic_position()
 
     def diag_status(self):
         """
         Prints a string containing the blocking status and the position of the
         motor.
         """
-        status = "\n{0}{1:<14}|{2:^16}|{3:^16}\n{4}{5}".format(
+        status = "\n{}{:<14}|{:^16}|{:^16}\n{}{}".format(
             " "*2, "Diagnostic", "Blocking", "Position", " "*2, "-"*50)
         for diag in self._diagnostics:
-            status += "\n{0}{1:<14}|{2:^16}|{3:^16.3f}".format(
+            status += "\n{}{:<14}|{:^16}|{:^16.3f}".format(
                 " "*2, diag.desc, str(diag.blocked), diag.x.position)
         logger.info(status)
 
     @property
     def theta1(self):
         """
         Returns the bragg angle the the delay line is currently set to
```

### Comparing `hxrsnd-0.2.9/hxrsnd/tests/conftest.py` & `hxrsnd-0.3.0/hxrsnd/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
 @pytest.fixture(scope='session', autouse=True)
 def set_level(pytestconfig):
     # Read user input logging level
     log_level = getattr(logging, pytestconfig.getoption('--log'), None)
 
     # Report invalid logging level
     if not isinstance(log_level, int):
-        raise ValueError("Invalid log level : {}".format(log_level))
+        raise ValueError(f"Invalid log level : {log_level}")
 
     # Create basic configuration
     logging.basicConfig(level=log_level,
                         filename=pytestconfig.getoption('--logfile'))
 
 
 @pytest.fixture(scope='function')
```

### Comparing `hxrsnd-0.2.9/hxrsnd/tests/test_aerotech.py` & `hxrsnd-0.3.0/hxrsnd/tests/test_aerotech.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 import logging
 from collections import OrderedDict
 
 import pytest
 from ophyd.device import Device
 
 from hxrsnd import aerotech
@@ -13,16 +12,16 @@
 
 logger = logging.getLogger(__name__)
 
 
 @pytest.mark.parametrize("dev", get_classes_in_module(aerotech, Device))
 def test_aerotech_devices_instantiate_and_run_ophyd_functions(dev):
     motor = fake_device(dev, "TEST:SND:T1")
-    assert(isinstance(motor.read(), OrderedDict))
-    assert(isinstance(motor.read_configuration(), OrderedDict))
+    assert isinstance(motor.read(), OrderedDict)
+    assert isinstance(motor.read_configuration(), OrderedDict)
 
 
 def test_AeroBase_raises_MotorDisabled_if_moved_while_disabled():
     motor = fake_device(AeroBase, "TEST:SND:T1")
     motor.axis_fault.sim_put(0)
     assert not motor.faulted
     motor.disable()
```

### Comparing `hxrsnd-0.2.9/hxrsnd/tests/test_attocube.py` & `hxrsnd-0.3.0/hxrsnd/tests/test_attocube.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 import logging
 import time
 from collections import OrderedDict
 
 import pytest
 from ophyd.device import Device
 
@@ -14,16 +13,16 @@
 
 logger = logging.getLogger(__name__)
 
 
 @pytest.mark.parametrize("dev", get_classes_in_module(attocube, Device))
 def test_attocube_devices_instantiate_and_run_ophyd_functions(dev):
     motor = fake_device(dev)
-    assert(isinstance(motor.read(), OrderedDict))
-    assert(isinstance(motor.read_configuration(), OrderedDict))
+    assert isinstance(motor.read(), OrderedDict)
+    assert isinstance(motor.read_configuration(), OrderedDict)
 
 
 def test_EccBase_raises_MotorDisabled_if_moved_while_disabled():
     motor = fake_device(EccBase)
     motor.motor_error.sim_put(0)
     assert not motor.error
     motor.disable()
```

### Comparing `hxrsnd-0.2.9/hxrsnd/tests/test_plans_alignment.py` & `hxrsnd-0.3.0/hxrsnd/tests/test_plans_alignment.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.2.9/hxrsnd/tests/test_plans_calibration.py` & `hxrsnd-0.3.0/hxrsnd/tests/test_plans_calibration.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.2.9/hxrsnd/tests/test_plans_plan_stubs.py` & `hxrsnd-0.3.0/hxrsnd/tests/test_plans_plan_stubs.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.2.9/hxrsnd/tests/test_plans_preprocessors.py` & `hxrsnd-0.3.0/hxrsnd/tests/test_plans_preprocessors.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.2.9/hxrsnd/tests/test_plans_scans.py` & `hxrsnd-0.3.0/hxrsnd/tests/test_plans_scans.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.2.9/hxrsnd/tests/test_pneumatic.py` & `hxrsnd-0.3.0/hxrsnd/tests/test_pneumatic.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 import logging
 import time
 from collections import OrderedDict
 
 import pytest
 from ophyd.device import Device
 
@@ -14,16 +13,16 @@
 
 logger = logging.getLogger(__name__)
 
 
 @pytest.mark.parametrize("dev", get_classes_in_module(pneumatic, Device))
 def test_devices_instantiate_and_run_ophyd_functions(dev):
     device = fake_device(dev)
-    assert(isinstance(device.read(), OrderedDict))
-    assert(isinstance(device.read_configuration(), OrderedDict))
+    assert isinstance(device.read(), OrderedDict)
+    assert isinstance(device.read_configuration(), OrderedDict)
 
 
 def test_ProportionalValve_opens_and_closes_correctly():
     valve = fake_device(ProportionalValve)
     valve.open()
     time.sleep(.1)
     assert valve.position == "OPEN"
```

### Comparing `hxrsnd-0.2.9/hxrsnd/tests/test_rtd.py` & `hxrsnd-0.3.0/hxrsnd/tests/test_rtd.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 import logging
 from collections import OrderedDict
 
 import pytest
 from ophyd.device import Device
 
 from hxrsnd import rtd
@@ -12,9 +11,9 @@
 
 logger = logging.getLogger(__name__)
 
 
 @pytest.mark.parametrize("dev", get_classes_in_module(rtd, Device))
 def test_rtd_devices_instantiate_and_run_ophyd_functions(dev):
     device = fake_device(dev)
-    assert(isinstance(device.read(), OrderedDict))
-    assert(isinstance(device.read_configuration(), OrderedDict))
+    assert isinstance(device.read(), OrderedDict)
+    assert isinstance(device.read_configuration(), OrderedDict)
```

### Comparing `hxrsnd-0.2.9/hxrsnd/tests/test_sequencer.py` & `hxrsnd-0.3.0/hxrsnd/tests/test_sequencer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 import logging
 from collections import OrderedDict
 
 import pytest
 from ophyd.device import Device
 
 from hxrsnd import sequencer
@@ -12,9 +11,9 @@
 
 logger = logging.getLogger(__name__)
 
 
 @pytest.mark.parametrize("dev", get_classes_in_module(sequencer, Device))
 def test_sequencer_devices_instantiate_and_run_ophyd_functions(dev):
     device = fake_device(dev)
-    assert(isinstance(device.read(), OrderedDict))
-    assert(isinstance(device.read_configuration(), OrderedDict))
+    assert isinstance(device.read(), OrderedDict)
+    assert isinstance(device.read_configuration(), OrderedDict)
```

### Comparing `hxrsnd-0.2.9/hxrsnd/tests/test_snd_devices.py` & `hxrsnd-0.3.0/hxrsnd/tests/test_snd_devices.py`

 * *Files identical despite different names*

### Comparing `hxrsnd-0.2.9/hxrsnd/tests/test_sndmotor.py` & `hxrsnd-0.3.0/hxrsnd/tests/test_sndmotor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 import logging
 from collections import OrderedDict
 from copy import deepcopy
 
 import numpy as np
 import pandas as pd
 import pytest
@@ -21,16 +20,16 @@
 logger = logging.getLogger(__name__)
 rtol = 1e-6                             # Numpy relative tolerance
 
 
 @pytest.mark.parametrize("dev", get_classes_in_module(sndmotor, Device))
 def test_sndmotor_devices_instantiate_and_run_ophyd_functions(dev):
     device = fake_device(dev)
-    assert(isinstance(device.read(), OrderedDict))
-    assert(isinstance(device.read_configuration(), OrderedDict))
+    assert isinstance(device.read(), OrderedDict)
+    assert isinstance(device.read_configuration(), OrderedDict)
 
 
 def test_CalibMotor_configure_raises_errors_on_bad_inputs():
     dev = CalibMotor("TST", name="test")
     config = deepcopy(dev.read_configuration())
 
     # Define a quick function to test value equivalence
```

### Comparing `hxrsnd-0.2.9/hxrsnd/tests/test_tower.py` & `hxrsnd-0.3.0/hxrsnd/tests/test_tower.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 import logging
 import time
 from collections import OrderedDict
 
 import pytest
 from ophyd.device import Device
 
@@ -15,16 +14,16 @@
 
 logger = logging.getLogger(__name__)
 
 
 @pytest.mark.parametrize("dev", get_classes_in_module(tower, Device))
 def test_devices_instantiate_and_run_ophyd_functions(dev):
     device = fake_device(dev, "TEST:SND:T1")
-    assert(isinstance(device.read(), OrderedDict))
-    assert(isinstance(device.read_configuration(), OrderedDict))
+    assert isinstance(device.read(), OrderedDict)
+    assert isinstance(device.read_configuration(), OrderedDict)
 
 
 def test_DelayTower_does_not_move_if_motors_not_ready():
     tower = fake_device(DelayTower, "TEST:SND:T1")
     tower.disable()
     time.sleep(.5)
     tower.tth.user_setpoint.sim_set_limits((-100, 100))
```

### Comparing `hxrsnd-0.2.9/hxrsnd/tests/test_utils.py` & `hxrsnd-0.3.0/hxrsnd/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,82 +57,82 @@
 00000380: 6d65 7472 697a 6528 2273 6372 6565 6e22  metrize("screen"
 00000390: 2c20 5b22 6d6f 746f 725f 6578 7065 7274  , ["motor_expert
 000003a0: 5f73 6372 6565 6e2e 7368 222c 2022 736e  _screen.sh", "sn
 000003b0: 645f 6d61 696e 225d 290a 6465 6620 7465  d_main"]).def te
 000003c0: 7374 5f61 6273 6f6c 7574 655f 7375 626d  st_absolute_subm
 000003d0: 6f64 756c 655f 7061 7468 5f77 6f72 6b73  odule_path_works
 000003e0: 5f63 6f72 7265 6374 6c79 2873 6372 6565  _correctly(scree
-000003f0: 6e29 3a0a 2020 2020 7061 7468 203d 2022  n):.    path = "
-00000400: 4858 5253 6e44 2f73 6372 6565 6e73 2f7b  HXRSnD/screens/{
-00000410: 307d 222e 666f 726d 6174 2873 6372 6565  0}".format(scree
-00000420: 6e29 0a20 2020 2074 656d 706c 6174 6520  n).    template 
-00000430: 3d20 222f 7265 672f 6e65 682f 6f70 6572  = "/reg/neh/oper
-00000440: 6174 6f72 2f78 6373 6f70 722f 6269 6e2f  ator/xcsopr/bin/
-00000450: 736e 642f 4858 5253 6e44 2f68 7872 736e  snd/HXRSnD/hxrsn
-00000460: 642f 7574 696c 732e 7079 220a 2020 2020  d/utils.py".    
-00000470: 6162 735f 7061 7468 203d 2050 6174 6828  abs_path = Path(
-00000480: 7574 696c 732e 6162 736f 6c75 7465 5f73  utils.absolute_s
-00000490: 7562 6d6f 6475 6c65 5f70 6174 6828 7061  ubmodule_path(pa
-000004a0: 7468 2c20 7465 6d70 6c61 7465 2929 0a20  th, template)). 
-000004b0: 2020 2061 7373 6572 7420 6162 735f 7061     assert abs_pa
-000004c0: 7468 203d 3d20 5061 7468 2822 2f22 2e6a  th == Path("/".j
-000004d0: 6f69 6e28 7465 6d70 6c61 7465 2e73 706c  oin(template.spl
-000004e0: 6974 2822 2f22 295b 3a2d 335d 2920 2b20  it("/")[:-3]) + 
-000004f0: 222f 2220 2b20 7061 7468 290a 0a0a 6465  "/" + path)...de
-00000500: 6620 7465 7374 5f73 746f 705f 6f6e 5f6b  f test_stop_on_k
-00000510: 6579 626f 6172 6469 6e74 6572 7275 7074  eyboardinterrupt
-00000520: 5f72 756e 735f 7374 6f70 5f6d 6574 686f  _runs_stop_metho
-00000530: 6428 293a 0a20 2020 2063 6c61 7373 2054  d():.    class T
-00000540: 6573 7443 6c61 7373 3a0a 2020 2020 2020  estClass:.      
-00000550: 2020 6e61 6d65 203d 2022 7465 7374 220a    name = "test".
-00000560: 2020 2020 2020 2020 7374 6f70 7065 6420          stopped 
-00000570: 3d20 4661 6c73 650a 0a20 2020 2020 2020  = False..       
-00000580: 2040 7574 696c 732e 7374 6f70 5f6f 6e5f   @utils.stop_on_
-00000590: 6b65 7962 6f61 7264 696e 7465 7272 7570  keyboardinterrup
-000005a0: 740a 2020 2020 2020 2020 6465 6620 736f  t.        def so
-000005b0: 6d65 7468 696e 675f 7468 6174 5f72 6169  mething_that_rai
-000005c0: 7365 735f 6b65 7962 6f61 7264 696e 7465  ses_keyboardinte
-000005d0: 7272 7570 7428 7365 6c66 293a 0a20 2020  rrupt(self):.   
-000005e0: 2020 2020 2020 2020 2072 6169 7365 204b           raise K
-000005f0: 6579 626f 6172 6449 6e74 6572 7275 7074  eyboardInterrupt
-00000600: 0a0a 2020 2020 2020 2020 6465 6620 7374  ..        def st
-00000610: 6f70 2873 656c 6629 3a0a 2020 2020 2020  op(self):.      
-00000620: 2020 2020 2020 7365 6c66 2e73 746f 7070        self.stopp
-00000630: 6564 203d 2054 7275 650a 2020 2020 7473  ed = True.    ts
-00000640: 7420 3d20 5465 7374 436c 6173 7328 290a  t = TestClass().
-00000650: 2020 2020 6173 7365 7274 2074 7374 2e73      assert tst.s
-00000660: 746f 7070 6564 2069 7320 4661 6c73 650a  topped is False.
-00000670: 2020 2020 7473 742e 736f 6d65 7468 696e      tst.somethin
-00000680: 675f 7468 6174 5f72 6169 7365 735f 6b65  g_that_raises_ke
-00000690: 7962 6f61 7264 696e 7465 7272 7570 7428  yboardinterrupt(
-000006a0: 290a 2020 2020 6173 7365 7274 2074 7374  ).    assert tst
-000006b0: 2e73 746f 7070 6564 2069 7320 5472 7565  .stopped is True
-000006c0: 0a0a 0a64 6566 2074 6573 745f 6e61 6e5f  ...def test_nan_
-000006d0: 6966 5f6e 6f5f 7061 7265 6e74 5f77 6f72  if_no_parent_wor
-000006e0: 6b73 5f66 6f72 5f6d 6574 686f 6473 5f61  ks_for_methods_a
-000006f0: 6e64 5f70 726f 7065 7274 6965 7328 293a  nd_properties():
-00000700: 0a20 2020 2063 6c61 7373 2054 6573 743a  .    class Test:
-00000710: 0a20 2020 2020 2020 2040 7072 6f70 6572  .        @proper
-00000720: 7479 0a20 2020 2020 2020 2040 7574 696c  ty.        @util
-00000730: 732e 6e61 6e5f 6966 5f6e 6f5f 7061 7265  s.nan_if_no_pare
-00000740: 6e74 0a20 2020 2020 2020 2064 6566 2074  nt.        def t
-00000750: 7374 5f70 726f 7065 7274 7928 7365 6c66  st_property(self
-00000760: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-00000770: 6574 7572 6e20 5472 7565 0a0a 2020 2020  eturn True..    
-00000780: 2020 2020 4075 7469 6c73 2e6e 616e 5f69      @utils.nan_i
-00000790: 665f 6e6f 5f70 6172 656e 740a 2020 2020  f_no_parent.    
-000007a0: 2020 2020 6465 6620 7473 745f 6d65 7468      def tst_meth
-000007b0: 6f64 2873 656c 6629 3a0a 2020 2020 2020  od(self):.      
-000007c0: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-000007d0: 650a 2020 2020 7473 7420 3d20 5465 7374  e.    tst = Test
-000007e0: 2829 0a20 2020 2074 7374 2e70 6172 656e  ().    tst.paren
-000007f0: 7420 3d20 4e6f 6e65 0a20 2020 2061 7373  t = None.    ass
-00000800: 6572 7420 6973 6e61 6e28 7473 742e 7473  ert isnan(tst.ts
-00000810: 745f 7072 6f70 6572 7479 290a 2020 2020  t_property).    
-00000820: 6173 7365 7274 2069 736e 616e 2874 7374  assert isnan(tst
-00000830: 2e74 7374 5f6d 6574 686f 6428 2929 0a20  .tst_method()). 
-00000840: 2020 2074 7374 2e70 6172 656e 7420 3d20     tst.parent = 
-00000850: 5472 7565 0a20 2020 2061 7373 6572 7420  True.    assert 
-00000860: 7473 742e 7473 745f 7072 6f70 6572 7479  tst.tst_property
-00000870: 2069 7320 5472 7565 0a20 2020 2061 7373   is True.    ass
-00000880: 6572 7420 7473 742e 7473 745f 6d65 7468  ert tst.tst_meth
-00000890: 6f64 2829 2069 7320 5472 7565 0a         od() is True.
+000003f0: 6e29 3a0a 2020 2020 7061 7468 203d 2066  n):.    path = f
+00000400: 2248 5852 536e 442f 7363 7265 656e 732f  "HXRSnD/screens/
+00000410: 7b73 6372 6565 6e7d 220a 2020 2020 7465  {screen}".    te
+00000420: 6d70 6c61 7465 203d 2022 2f72 6567 2f6e  mplate = "/reg/n
+00000430: 6568 2f6f 7065 7261 746f 722f 7863 736f  eh/operator/xcso
+00000440: 7072 2f62 696e 2f73 6e64 2f48 5852 536e  pr/bin/snd/HXRSn
+00000450: 442f 6878 7273 6e64 2f75 7469 6c73 2e70  D/hxrsnd/utils.p
+00000460: 7922 0a20 2020 2061 6273 5f70 6174 6820  y".    abs_path 
+00000470: 3d20 5061 7468 2875 7469 6c73 2e61 6273  = Path(utils.abs
+00000480: 6f6c 7574 655f 7375 626d 6f64 756c 655f  olute_submodule_
+00000490: 7061 7468 2870 6174 682c 2074 656d 706c  path(path, templ
+000004a0: 6174 6529 290a 2020 2020 6173 7365 7274  ate)).    assert
+000004b0: 2061 6273 5f70 6174 6820 3d3d 2050 6174   abs_path == Pat
+000004c0: 6828 222f 222e 6a6f 696e 2874 656d 706c  h("/".join(templ
+000004d0: 6174 652e 7370 6c69 7428 222f 2229 5b3a  ate.split("/")[:
+000004e0: 2d33 5d29 202b 2022 2f22 202b 2070 6174  -3]) + "/" + pat
+000004f0: 6829 0a0a 0a64 6566 2074 6573 745f 7374  h)...def test_st
+00000500: 6f70 5f6f 6e5f 6b65 7962 6f61 7264 696e  op_on_keyboardin
+00000510: 7465 7272 7570 745f 7275 6e73 5f73 746f  terrupt_runs_sto
+00000520: 705f 6d65 7468 6f64 2829 3a0a 2020 2020  p_method():.    
+00000530: 636c 6173 7320 5465 7374 436c 6173 733a  class TestClass:
+00000540: 0a20 2020 2020 2020 206e 616d 6520 3d20  .        name = 
+00000550: 2274 6573 7422 0a20 2020 2020 2020 2073  "test".        s
+00000560: 746f 7070 6564 203d 2046 616c 7365 0a0a  topped = False..
+00000570: 2020 2020 2020 2020 4075 7469 6c73 2e73          @utils.s
+00000580: 746f 705f 6f6e 5f6b 6579 626f 6172 6469  top_on_keyboardi
+00000590: 6e74 6572 7275 7074 0a20 2020 2020 2020  nterrupt.       
+000005a0: 2064 6566 2073 6f6d 6574 6869 6e67 5f74   def something_t
+000005b0: 6861 745f 7261 6973 6573 5f6b 6579 626f  hat_raises_keybo
+000005c0: 6172 6469 6e74 6572 7275 7074 2873 656c  ardinterrupt(sel
+000005d0: 6629 3a0a 2020 2020 2020 2020 2020 2020  f):.            
+000005e0: 7261 6973 6520 4b65 7962 6f61 7264 496e  raise KeyboardIn
+000005f0: 7465 7272 7570 740a 0a20 2020 2020 2020  terrupt..       
+00000600: 2064 6566 2073 746f 7028 7365 6c66 293a   def stop(self):
+00000610: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00000620: 662e 7374 6f70 7065 6420 3d20 5472 7565  f.stopped = True
+00000630: 0a20 2020 2074 7374 203d 2054 6573 7443  .    tst = TestC
+00000640: 6c61 7373 2829 0a20 2020 2061 7373 6572  lass().    asser
+00000650: 7420 7473 742e 7374 6f70 7065 6420 6973  t tst.stopped is
+00000660: 2046 616c 7365 0a20 2020 2074 7374 2e73   False.    tst.s
+00000670: 6f6d 6574 6869 6e67 5f74 6861 745f 7261  omething_that_ra
+00000680: 6973 6573 5f6b 6579 626f 6172 6469 6e74  ises_keyboardint
+00000690: 6572 7275 7074 2829 0a20 2020 2061 7373  errupt().    ass
+000006a0: 6572 7420 7473 742e 7374 6f70 7065 6420  ert tst.stopped 
+000006b0: 6973 2054 7275 650a 0a0a 6465 6620 7465  is True...def te
+000006c0: 7374 5f6e 616e 5f69 665f 6e6f 5f70 6172  st_nan_if_no_par
+000006d0: 656e 745f 776f 726b 735f 666f 725f 6d65  ent_works_for_me
+000006e0: 7468 6f64 735f 616e 645f 7072 6f70 6572  thods_and_proper
+000006f0: 7469 6573 2829 3a0a 2020 2020 636c 6173  ties():.    clas
+00000700: 7320 5465 7374 3a0a 2020 2020 2020 2020  s Test:.        
+00000710: 4070 726f 7065 7274 790a 2020 2020 2020  @property.      
+00000720: 2020 4075 7469 6c73 2e6e 616e 5f69 665f    @utils.nan_if_
+00000730: 6e6f 5f70 6172 656e 740a 2020 2020 2020  no_parent.      
+00000740: 2020 6465 6620 7473 745f 7072 6f70 6572    def tst_proper
+00000750: 7479 2873 656c 6629 3a0a 2020 2020 2020  ty(self):.      
+00000760: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+00000770: 650a 0a20 2020 2020 2020 2040 7574 696c  e..        @util
+00000780: 732e 6e61 6e5f 6966 5f6e 6f5f 7061 7265  s.nan_if_no_pare
+00000790: 6e74 0a20 2020 2020 2020 2064 6566 2074  nt.        def t
+000007a0: 7374 5f6d 6574 686f 6428 7365 6c66 293a  st_method(self):
+000007b0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000007c0: 7572 6e20 5472 7565 0a20 2020 2074 7374  urn True.    tst
+000007d0: 203d 2054 6573 7428 290a 2020 2020 7473   = Test().    ts
+000007e0: 742e 7061 7265 6e74 203d 204e 6f6e 650a  t.parent = None.
+000007f0: 2020 2020 6173 7365 7274 2069 736e 616e      assert isnan
+00000800: 2874 7374 2e74 7374 5f70 726f 7065 7274  (tst.tst_propert
+00000810: 7929 0a20 2020 2061 7373 6572 7420 6973  y).    assert is
+00000820: 6e61 6e28 7473 742e 7473 745f 6d65 7468  nan(tst.tst_meth
+00000830: 6f64 2829 290a 2020 2020 7473 742e 7061  od()).    tst.pa
+00000840: 7265 6e74 203d 2054 7275 650a 2020 2020  rent = True.    
+00000850: 6173 7365 7274 2074 7374 2e74 7374 5f70  assert tst.tst_p
+00000860: 726f 7065 7274 7920 6973 2054 7275 650a  roperty is True.
+00000870: 2020 2020 6173 7365 7274 2074 7374 2e74      assert tst.t
+00000880: 7374 5f6d 6574 686f 6428 2920 6973 2054  st_method() is T
+00000890: 7275 650a                                rue.
```

### Comparing `hxrsnd-0.2.9/hxrsnd/tower.py` & `hxrsnd-0.3.0/hxrsnd/tower.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         self.pos_removed = pos_removed
         self.desc_short = "".join([s[0] for s in self.desc.split(" ")])
 
         # Add Tower short name to desc
         for sig_name in self.component_names:
             signal = getattr(self, sig_name)
             if hasattr(signal, "desc"):
-                signal.desc = "{0} {1}".format(self.desc_short, signal.desc)
+                signal.desc = f"{self.desc_short} {signal.desc}"
 
     def set_energy(self, E, *args, **kwargs):
         """
         Placeholder for the energy setter. Implement for each TowerBase
         subclass.
         """
         pass
@@ -200,15 +200,15 @@
                 raise
 
         # Check that we can move all the motors
         for motor, position in zip(motors, positions):
             try:
                 motor.check_status(position)
             except Exception as e:
-                err = "Motor {0} got an exception: {1}".format(motor.desc, e)
+                err = f"Motor {motor.desc} got an exception: {e}"
                 logger.error(err)
                 raise e
 
     def stop(self):
         """
         Stops the motions of all the motors.
         """
@@ -254,45 +254,45 @@
         Returns
         -------
         status : str
             Status string.
         """
         if short:
             # Header
-            status += "\n{0}{1}\n{2}{3}".format(
+            status += "\n{}{}\n{}{}".format(
                 " "*offset, self.desc, " "*(offset+2), "-"*50)
 
             # Aerotech body
             status_list_aero = self._apply_all(
                 "status", AeroBase, offset=offset+2, print_status=False,
                 short=True)
             if status_list_aero:
                 # Aerotech header
                 status += (
-                    "\n{0}{1:<16}|{2:^16}|{3:^16}\n{4}{5}".format(
+                    "\n{}{:<16}|{:^16}|{:^16}\n{}{}".format(
                         " "*(offset+2), "Motor", "Position", "Dial", " "*(offset+2), "-"*50
                     )
                 )
                 status += "".join(status_list_aero)
 
             # Attocube body
             status_list_atto = self._apply_all(
                 "status", EccBase, offset=offset+2, print_status=False,
                 short=True)
             if status_list_atto:
                 # Attocube Header
                 status += (
-                    "\n{0}{1}\n{2}{3:<16}|{4:^16}|{5:^16}\n{6}{7}".format(
+                    "\n{}{}\n{}{:<16}|{:^16}|{:^16}\n{}{}".format(
                         " "*(offset+2), "-"*50, " " * (offset+2),
                         "Motor", "Position", "Reference", " "*(offset+2), "-"*50)
                 )
                 status += "".join(status_list_atto)
 
         else:
-            status += "{0}{1}:\n{2}{3}\n".format(
+            status += "{}{}:\n{}{}\n".format(
                 " "*offset, self.desc, " "*offset, "-"*(len(self.desc)+1)
             )
             status_list = self._apply_all("status", (AeroBase, EccBase),
                                           offset=offset+2, print_status=False)
             status += "".join(status_list)
 
         if newline:
```

### Comparing `hxrsnd-0.2.9/hxrsnd/utils.py` & `hxrsnd-0.3.0/hxrsnd/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -124,16 +124,15 @@
     Returns
     -------
     value : object
         The contents of the iterable
     """
     for val in inp_iter:
         if isiterable(val):
-            for ival in _flatten(val):
-                yield ival
+            yield from _flatten(val)
         else:
             yield val
 
 
 def flatten(inp_iter):
     """
     Returns a flattened list of the inputted iterable.
@@ -160,18 +159,18 @@
     @wraps(func)
     def stop_dev_on_keyboardinterrupt(obj, *args, **kwargs):
         if hasattr(obj, "stop") and callable(obj.stop):
             try:
                 return func(obj, *args, **kwargs)
             except KeyboardInterrupt:
                 obj.stop()
-                logger.info("Motor '{0}' stopped by keyboard interrupt".format(
+                logger.info("Motor '{}' stopped by keyboard interrupt".format(
                     obj.name))
         else:
-            raise AttributeError("Object '{0}' needs a stop method to use the "
+            raise AttributeError("Object '{}' needs a stop method to use the "
                                  "stop_on_keyboardinterrupt decorator.".format(
                                      obj))
     return stop_dev_on_keyboardinterrupt
 
 
 def nan_if_no_parent(method):
     """
```

