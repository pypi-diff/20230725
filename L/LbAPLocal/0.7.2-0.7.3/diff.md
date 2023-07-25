# Comparing `tmp/LbAPLocal-0.7.2.tar.gz` & `tmp/LbAPLocal-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LbAPLocal-0.7.2.tar", last modified: Tue Jul 25 13:12:05 2023, max compression
+gzip compressed data, was "LbAPLocal-0.7.3.tar", last modified: Tue Jul 25 19:09:17 2023, max compression
```

## Comparing `LbAPLocal-0.7.2.tar` & `LbAPLocal-0.7.3.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:12:05.448000 LbAPLocal-0.7.2/
--rw-r--r--   0 root         (0) root         (0)       36 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/.coveragerc
--rw-r--r--   0 root         (0) root         (0)     2083 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/.gitignore
--rw-r--r--   0 root         (0) root         (0)     2416 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)      866 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)     3027 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)    32472 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7375 2023-07-25 13:12:05.448000 LbAPLocal-0.7.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6552 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/README.md
--rw-r--r--   0 root         (0) root         (0)      393 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/environment.yaml
--rw-r--r--   0 root         (0) root         (0)     1590 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/example.json
--rw-r--r--   0 root         (0) root         (0)     1863 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 13:12:05.448000 LbAPLocal-0.7.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:12:05.424000 LbAPLocal-0.7.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:12:05.428000 LbAPLocal-0.7.2/src/LbAPLocal/
--rw-r--r--   0 root         (0) root         (0)      800 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/src/LbAPLocal/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5997 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/src/LbAPLocal/checks.py
--rw-r--r--   0 root         (0) root         (0)    23965 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/src/LbAPLocal/cli.py
--rw-r--r--   0 root         (0) root         (0)     3292 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/src/LbAPLocal/log_parsing.py
--rw-r--r--   0 root         (0) root         (0)    10999 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/src/LbAPLocal/testing.py
--rw-r--r--   0 root         (0) root         (0)    10025 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/src/LbAPLocal/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:12:05.428000 LbAPLocal-0.7.2/src/LbAPLocal.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7375 2023-07-25 13:12:05.000000 LbAPLocal-0.7.2/src/LbAPLocal.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5877 2023-07-25 13:12:05.000000 LbAPLocal-0.7.2/src/LbAPLocal.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 13:12:05.000000 LbAPLocal-0.7.2/src/LbAPLocal.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-07-25 13:12:05.000000 LbAPLocal-0.7.2/src/LbAPLocal.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      183 2023-07-25 13:12:05.000000 LbAPLocal-0.7.2/src/LbAPLocal.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-25 13:12:05.000000 LbAPLocal-0.7.2/src/LbAPLocal.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:12:05.428000 LbAPLocal-0.7.2/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:12:05.424000 LbAPLocal-0.7.2/tests/cassettes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:12:05.432000 LbAPLocal-0.7.2/tests/cassettes/test_execute/
--rw-r--r--   0 root         (0) root         (0)     2775 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/cassettes/test_execute/test_run_test[2016_MagDown_PromptMC_D02KK-2444].yaml
--rw-r--r--   0 root         (0) root         (0)     1015 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/cassettes/test_execute/test_run_test[2016_MagDown_PromptMC_D02KK_noautoconf-2444].yaml
--rw-r--r--   0 root         (0) root         (0)     2536 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/cassettes/test_execute/test_run_test[2016_MagUp_PromptMC_D02KK-2393].yaml
--rw-r--r--   0 root         (0) root         (0)      908 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/cassettes/test_execute/test_run_test[2016_MagUp_PromptMC_D02KK_noautoconf-2393].yaml
--rw-r--r--   0 root         (0) root         (0)     5430 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:12:05.424000 LbAPLocal-0.7.2/tests/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:12:05.432000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/
--rw-r--r--   0 root         (0) root         (0)      622 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/.gitignore
--rw-r--r--   0 root         (0) root         (0)      837 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)      405 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/AnalysisProductions.xenv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:12:05.432000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/
--rw-r--r--   0 root         (0) root         (0)     4485 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bc2Bspi2JpsiPhi.py
--rw-r--r--   0 root         (0) root         (0)     4320 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bd2JpsiKstar.py
--rw-r--r--   0 root         (0) root         (0)      341 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bd2JpsiKstar_stripping.py
--rw-r--r--   0 root         (0) root         (0)     5996 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2DsPi.py
--rw-r--r--   0 root         (0) root         (0)     3988 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi.py
--rw-r--r--   0 root         (0) root         (0)     4315 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi_Prompt.py
--rw-r--r--   0 root         (0) root         (0)     4905 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi_Prompt_PVMixer.py
--rw-r--r--   0 root         (0) root         (0)     3597 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi_Swave.py
--rw-r--r--   0 root         (0) root         (0)     2563 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bu2JpsiKplus.py
--rw-r--r--   0 root         (0) root         (0)      337 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bu2JpsiKplus_stripping.py
--rw-r--r--   0 root         (0) root         (0)      178 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/LbJpsipK.py
--rw-r--r--   0 root         (0) root         (0)     1081 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:12:05.432000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/helpers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3770 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/helpers/stripping.py
--rw-r--r--   0 root         (0) root         (0)     8845 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/helpers/tuple_maker.py
--rw-r--r--   0 root         (0) root         (0)    20265 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/info.yaml
--rw-r--r--   0 root         (0) root         (0)     1013 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/sequence_setup.py
--rw-r--r--   0 root         (0) root         (0)    35149 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/COPYING
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:12:05.436000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/RDs/
--rw-r--r--   0 root         (0) root         (0)      212 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/RDs/README.md
--rw-r--r--   0 root         (0) root         (0)      831 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/RDs/Run1_Signal.py
--rw-r--r--   0 root         (0) root         (0)      865 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/RDs/Run2_Signal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:12:05.436000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/RDs/helpers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/RDs/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8972 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/RDs/helpers/signal_tuple_maker.py
--rw-r--r--   0 root         (0) root         (0)     1910 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/RDs/info.yaml
--rw-r--r--   0 root         (0) root         (0)     6380 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/README.md
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:12:05.440000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/
--rw-r--r--   0 root         (0) root         (0)       63 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/2011_datatype.py
--rw-r--r--   0 root         (0) root         (0)       63 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/2012_datatype.py
--rw-r--r--   0 root         (0) root         (0)       63 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/2015_datatype.py
--rw-r--r--   0 root         (0) root         (0)       63 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/2016_datatype.py
--rw-r--r--   0 root         (0) root         (0)       63 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/2017_datatype.py
--rw-r--r--   0 root         (0) root         (0)       63 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/2018_datatype.py
--rw-r--r--   0 root         (0) root         (0)      233 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/B0ToK0ee.py
--rw-r--r--   0 root         (0) root         (0)      235 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/B0ToK0mumu.py
--rw-r--r--   0 root         (0) root         (0)      240 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/BpToKee.py
--rw-r--r--   0 root         (0) root         (0)      233 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/BpToKmumu.py
--rw-r--r--   0 root         (0) root         (0)      228 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/LbToL0ee.py
--rw-r--r--   0 root         (0) root         (0)      231 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/LbToL0eeSS.py
--rw-r--r--   0 root         (0) root         (0)      230 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/LbToL0emu.py
--rw-r--r--   0 root         (0) root         (0)      233 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/LbToL0emuSS.py
--rw-r--r--   0 root         (0) root         (0)      234 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/LbToL0mumu.py
--rw-r--r--   0 root         (0) root         (0)      232 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/LbToL0mumuSS.py
--rw-r--r--   0 root         (0) root         (0)     1447 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/README.md
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/__init__.py
--rw-r--r--   0 root         (0) root         (0)      150 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/general_options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:12:05.440000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/helpers/
--rw-r--r--   0 root         (0) root         (0)     1660 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/helpers/MC_tuple_maker.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7993 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/helpers/decay_descriptors.py
--rw-r--r--   0 root         (0) root         (0)     1937 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/helpers/locations.py
--rw-r--r--   0 root         (0) root         (0)     2985 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/helpers/related_info.py
--rw-r--r--   0 root         (0) root         (0)     3733 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/helpers/stripping.py
--rw-r--r--   0 root         (0) root         (0)    56910 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/helpers/tags.py
--rw-r--r--   0 root         (0) root         (0)    20824 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/helpers/tuple_maker.py
--rw-r--r--   0 root         (0) root         (0)     2093 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/info.yaml
--rw-r--r--   0 root         (0) root         (0)      149 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/mc_general_options_DST.py
--rw-r--r--   0 root         (0) root         (0)      149 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/mc_general_options_FDST.py
--rw-r--r--   0 root         (0) root         (0)      150 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/mc_general_options_FMDST.py
--rw-r--r--   0 root         (0) root         (0)      150 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/mc_general_options_MDST.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:12:05.444000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/mc_samples/
--rw-r--r--   0 root         (0) root         (0)      121 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bd2JpsiKs_ee.py
--rw-r--r--   0 root         (0) root         (0)      122 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bd2JpsiKs_mm.py
--rw-r--r--   0 root         (0) root         (0)      118 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bd2Ksee.py
--rw-r--r--   0 root         (0) root         (0)      118 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bd2Ksmm.py
--rw-r--r--   0 root         (0) root         (0)      121 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bd2PsiKs_ee.py
--rw-r--r--   0 root         (0) root         (0)      122 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bd2PsiKs_mm.py
--rw-r--r--   0 root         (0) root         (0)      122 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bu2JpsiK_ee.py
--rw-r--r--   0 root         (0) root         (0)      122 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bu2JpsiK_mm.py
--rw-r--r--   0 root         (0) root         (0)      120 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Lb2JpsiL_ee.py
--rw-r--r--   0 root         (0) root         (0)      120 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Lb2JpsiL_mm.py
--rw-r--r--   0 root         (0) root         (0)      117 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Lb2Lee.py
--rw-r--r--   0 root         (0) root         (0)      117 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Lb2Lem.py
--rw-r--r--   0 root         (0) root         (0)      117 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Lb2Lmm.py
--rw-r--r--   0 root         (0) root         (0)      120 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Lb2PsiL_ee.py
--rw-r--r--   0 root         (0) root         (0)      120 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Lb2PsiL_mm.py
--rw-r--r--   0 root         (0) root         (0)     1068 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/sequence_setup.py
--rw-r--r--   0 root         (0) root         (0)      621 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/stripping_seq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:12:05.444000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/executabletests/
--rw-r--r--   0 root         (0) root         (0)      348 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/executabletests/2016_MagDown_PromptMC_D02KK_autoconf.py
--rw-r--r--   0 root         (0) root         (0)      348 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/executabletests/2016_MagUp_PromptMC_D02KK_autoconf.py
--rw-r--r--   0 root         (0) root         (0)     1182 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/executabletests/info.yaml
--rw-r--r--   0 root         (0) root         (0)     1393 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/data-pkg-repo/executabletests/ntuple_options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:12:05.448000 LbAPLocal-0.7.2/tests/data/example-logs/
--rw-r--r--   0 root         (0) root         (0)   516613 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/example-logs/error-failed-to-read-file.log
--rw-r--r--   0 root         (0) root         (0)   344567 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/example-logs/error-illegal-instruction.log
--rw-r--r--   0 root         (0) root         (0)     3373 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/example-logs/error-missing-shared-library.log
--rw-r--r--   0 root         (0) root         (0)     2723 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/example-logs/error-platform-unsupported.log
--rw-r--r--   0 root         (0) root         (0)   584650 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/example-logs/error-related-info-missing.log
--rw-r--r--   0 root         (0) root         (0)   135940 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/example-logs/good-DaVinci_00110296_00000038_1.log
--rw-r--r--   0 root         (0) root         (0)   139869 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/example-logs/good-DaVinci_00110296_00000194_1.log
--rw-r--r--   0 root         (0) root         (0)   751141 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/data/example-logs/good-Gauss_00104988_00000011_1.log
--rw-r--r--   0 root         (0) root         (0)     4057 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     4758 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/test_execute.py
--rw-r--r--   0 root         (0) root         (0)     2724 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/test_local_datapkg.py
--rw-r--r--   0 root         (0) root         (0)     1471 2023-07-25 13:11:50.000000 LbAPLocal-0.7.2/tests/test_log_parse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:09:17.720000 LbAPLocal-0.7.3/
+-rw-r--r--   0 root         (0) root         (0)       36 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)     2083 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     2416 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)      866 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)     3027 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    32472 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7375 2023-07-25 19:09:17.720000 LbAPLocal-0.7.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6552 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/README.md
+-rw-r--r--   0 root         (0) root         (0)      393 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/environment.yaml
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/example.json
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 19:09:17.720000 LbAPLocal-0.7.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:09:17.692000 LbAPLocal-0.7.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:09:17.700000 LbAPLocal-0.7.3/src/LbAPLocal/
+-rw-r--r--   0 root         (0) root         (0)      800 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/src/LbAPLocal/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5997 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/src/LbAPLocal/checks.py
+-rw-r--r--   0 root         (0) root         (0)    23965 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/src/LbAPLocal/cli.py
+-rw-r--r--   0 root         (0) root         (0)     3292 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/src/LbAPLocal/log_parsing.py
+-rw-r--r--   0 root         (0) root         (0)    10999 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/src/LbAPLocal/testing.py
+-rw-r--r--   0 root         (0) root         (0)    10025 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/src/LbAPLocal/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:09:17.700000 LbAPLocal-0.7.3/src/LbAPLocal.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7375 2023-07-25 19:09:17.000000 LbAPLocal-0.7.3/src/LbAPLocal.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5877 2023-07-25 19:09:17.000000 LbAPLocal-0.7.3/src/LbAPLocal.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 19:09:17.000000 LbAPLocal-0.7.3/src/LbAPLocal.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-07-25 19:09:17.000000 LbAPLocal-0.7.3/src/LbAPLocal.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      183 2023-07-25 19:09:17.000000 LbAPLocal-0.7.3/src/LbAPLocal.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-25 19:09:17.000000 LbAPLocal-0.7.3/src/LbAPLocal.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:09:17.700000 LbAPLocal-0.7.3/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:09:17.692000 LbAPLocal-0.7.3/tests/cassettes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:09:17.700000 LbAPLocal-0.7.3/tests/cassettes/test_execute/
+-rw-r--r--   0 root         (0) root         (0)     2775 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/cassettes/test_execute/test_run_test[2016_MagDown_PromptMC_D02KK-2444].yaml
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/cassettes/test_execute/test_run_test[2016_MagDown_PromptMC_D02KK_noautoconf-2444].yaml
+-rw-r--r--   0 root         (0) root         (0)     2536 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/cassettes/test_execute/test_run_test[2016_MagUp_PromptMC_D02KK-2393].yaml
+-rw-r--r--   0 root         (0) root         (0)      908 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/cassettes/test_execute/test_run_test[2016_MagUp_PromptMC_D02KK_noautoconf-2393].yaml
+-rw-r--r--   0 root         (0) root         (0)     5430 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:09:17.696000 LbAPLocal-0.7.3/tests/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:09:17.704000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/
+-rw-r--r--   0 root         (0) root         (0)      622 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      837 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)      405 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/AnalysisProductions.xenv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:09:17.704000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/
+-rw-r--r--   0 root         (0) root         (0)     4485 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bc2Bspi2JpsiPhi.py
+-rw-r--r--   0 root         (0) root         (0)     4320 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bd2JpsiKstar.py
+-rw-r--r--   0 root         (0) root         (0)      341 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bd2JpsiKstar_stripping.py
+-rw-r--r--   0 root         (0) root         (0)     5996 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2DsPi.py
+-rw-r--r--   0 root         (0) root         (0)     3988 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi.py
+-rw-r--r--   0 root         (0) root         (0)     4315 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi_Prompt.py
+-rw-r--r--   0 root         (0) root         (0)     4905 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi_Prompt_PVMixer.py
+-rw-r--r--   0 root         (0) root         (0)     3597 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi_Swave.py
+-rw-r--r--   0 root         (0) root         (0)     2563 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bu2JpsiKplus.py
+-rw-r--r--   0 root         (0) root         (0)      337 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bu2JpsiKplus_stripping.py
+-rw-r--r--   0 root         (0) root         (0)      178 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/LbJpsipK.py
+-rw-r--r--   0 root         (0) root         (0)     1081 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:09:17.708000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/helpers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 19:09:03.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3770 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/helpers/stripping.py
+-rw-r--r--   0 root         (0) root         (0)     8845 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/helpers/tuple_maker.py
+-rw-r--r--   0 root         (0) root         (0)    20265 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/info.yaml
+-rw-r--r--   0 root         (0) root         (0)     1013 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/sequence_setup.py
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/COPYING
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:09:17.708000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/RDs/
+-rw-r--r--   0 root         (0) root         (0)      212 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/RDs/README.md
+-rw-r--r--   0 root         (0) root         (0)      831 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/RDs/Run1_Signal.py
+-rw-r--r--   0 root         (0) root         (0)      865 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/RDs/Run2_Signal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:09:17.708000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/RDs/helpers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 19:09:03.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/RDs/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8972 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/RDs/helpers/signal_tuple_maker.py
+-rw-r--r--   0 root         (0) root         (0)     1910 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/RDs/info.yaml
+-rw-r--r--   0 root         (0) root         (0)     6380 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/README.md
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 19:09:03.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:09:17.712000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/
+-rw-r--r--   0 root         (0) root         (0)       63 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/2011_datatype.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/2012_datatype.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/2015_datatype.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/2016_datatype.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/2017_datatype.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/2018_datatype.py
+-rw-r--r--   0 root         (0) root         (0)      233 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/B0ToK0ee.py
+-rw-r--r--   0 root         (0) root         (0)      235 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/B0ToK0mumu.py
+-rw-r--r--   0 root         (0) root         (0)      240 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/BpToKee.py
+-rw-r--r--   0 root         (0) root         (0)      233 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/BpToKmumu.py
+-rw-r--r--   0 root         (0) root         (0)      228 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/LbToL0ee.py
+-rw-r--r--   0 root         (0) root         (0)      231 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/LbToL0eeSS.py
+-rw-r--r--   0 root         (0) root         (0)      230 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/LbToL0emu.py
+-rw-r--r--   0 root         (0) root         (0)      233 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/LbToL0emuSS.py
+-rw-r--r--   0 root         (0) root         (0)      234 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/LbToL0mumu.py
+-rw-r--r--   0 root         (0) root         (0)      232 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/LbToL0mumuSS.py
+-rw-r--r--   0 root         (0) root         (0)     1447 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/README.md
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 19:09:03.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      150 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/general_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:09:17.712000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/helpers/
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/helpers/MC_tuple_maker.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 19:09:03.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7993 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/helpers/decay_descriptors.py
+-rw-r--r--   0 root         (0) root         (0)     1937 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/helpers/locations.py
+-rw-r--r--   0 root         (0) root         (0)     2985 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/helpers/related_info.py
+-rw-r--r--   0 root         (0) root         (0)     3733 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/helpers/stripping.py
+-rw-r--r--   0 root         (0) root         (0)    56910 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/helpers/tags.py
+-rw-r--r--   0 root         (0) root         (0)    20824 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/helpers/tuple_maker.py
+-rw-r--r--   0 root         (0) root         (0)     2093 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/info.yaml
+-rw-r--r--   0 root         (0) root         (0)      149 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/mc_general_options_DST.py
+-rw-r--r--   0 root         (0) root         (0)      149 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/mc_general_options_FDST.py
+-rw-r--r--   0 root         (0) root         (0)      150 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/mc_general_options_FMDST.py
+-rw-r--r--   0 root         (0) root         (0)      150 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/mc_general_options_MDST.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:09:17.716000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/mc_samples/
+-rw-r--r--   0 root         (0) root         (0)      121 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bd2JpsiKs_ee.py
+-rw-r--r--   0 root         (0) root         (0)      122 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bd2JpsiKs_mm.py
+-rw-r--r--   0 root         (0) root         (0)      118 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bd2Ksee.py
+-rw-r--r--   0 root         (0) root         (0)      118 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bd2Ksmm.py
+-rw-r--r--   0 root         (0) root         (0)      121 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bd2PsiKs_ee.py
+-rw-r--r--   0 root         (0) root         (0)      122 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bd2PsiKs_mm.py
+-rw-r--r--   0 root         (0) root         (0)      122 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bu2JpsiK_ee.py
+-rw-r--r--   0 root         (0) root         (0)      122 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bu2JpsiK_mm.py
+-rw-r--r--   0 root         (0) root         (0)      120 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Lb2JpsiL_ee.py
+-rw-r--r--   0 root         (0) root         (0)      120 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Lb2JpsiL_mm.py
+-rw-r--r--   0 root         (0) root         (0)      117 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Lb2Lee.py
+-rw-r--r--   0 root         (0) root         (0)      117 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Lb2Lem.py
+-rw-r--r--   0 root         (0) root         (0)      117 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Lb2Lmm.py
+-rw-r--r--   0 root         (0) root         (0)      120 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Lb2PsiL_ee.py
+-rw-r--r--   0 root         (0) root         (0)      120 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Lb2PsiL_mm.py
+-rw-r--r--   0 root         (0) root         (0)     1068 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/sequence_setup.py
+-rw-r--r--   0 root         (0) root         (0)      621 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/stripping_seq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:09:17.716000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/executabletests/
+-rw-r--r--   0 root         (0) root         (0)      348 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/executabletests/2016_MagDown_PromptMC_D02KK_autoconf.py
+-rw-r--r--   0 root         (0) root         (0)      348 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/executabletests/2016_MagUp_PromptMC_D02KK_autoconf.py
+-rw-r--r--   0 root         (0) root         (0)     1182 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/executabletests/info.yaml
+-rw-r--r--   0 root         (0) root         (0)     1393 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/data-pkg-repo/executabletests/ntuple_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:09:17.720000 LbAPLocal-0.7.3/tests/data/example-logs/
+-rw-r--r--   0 root         (0) root         (0)   516613 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/example-logs/error-failed-to-read-file.log
+-rw-r--r--   0 root         (0) root         (0)   344567 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/example-logs/error-illegal-instruction.log
+-rw-r--r--   0 root         (0) root         (0)     3373 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/example-logs/error-missing-shared-library.log
+-rw-r--r--   0 root         (0) root         (0)     2723 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/example-logs/error-platform-unsupported.log
+-rw-r--r--   0 root         (0) root         (0)   584650 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/example-logs/error-related-info-missing.log
+-rw-r--r--   0 root         (0) root         (0)   135940 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/example-logs/good-DaVinci_00110296_00000038_1.log
+-rw-r--r--   0 root         (0) root         (0)   139869 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/example-logs/good-DaVinci_00110296_00000194_1.log
+-rw-r--r--   0 root         (0) root         (0)   751141 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/data/example-logs/good-Gauss_00104988_00000011_1.log
+-rw-r--r--   0 root         (0) root         (0)     4057 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     4758 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/test_execute.py
+-rw-r--r--   0 root         (0) root         (0)     2724 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/test_local_datapkg.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-07-25 19:09:02.000000 LbAPLocal-0.7.3/tests/test_log_parse.py
```

### Comparing `LbAPLocal-0.7.2/.gitignore` & `LbAPLocal-0.7.3/.gitignore`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/.gitlab-ci.yml` & `LbAPLocal-0.7.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/.pre-commit-config.yaml` & `LbAPLocal-0.7.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/CONTRIBUTING.md` & `LbAPLocal-0.7.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/LICENSE` & `LbAPLocal-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/PKG-INFO` & `LbAPLocal-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LbAPLocal
-Version: 0.7.2
+Version: 0.7.3
 Summary: Tool to locally run tests for AnalysisProductions
 Author: LHCb
 Project-URL: Homepage, https://gitlab.cern.ch/lhcb-dpa/analysis-productions/lbaplocal
 Project-URL: Bug Reports, https://gitlab.cern.ch/lhcb-dpa/analysis-productions/lbaplocal/-/issues
 Project-URL: Source, https://gitlab.cern.ch/lhcb-dpa/analysis-productions/lbaplocal
 Keywords: LHCb AnalysisProductions DIRAC
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LbAPLocal-0.7.2/README.md` & `LbAPLocal-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/example.json` & `LbAPLocal-0.7.3/example.json`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/pyproject.toml` & `LbAPLocal-0.7.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.9",
 ]
 requires-python = ">=3.9"
 dependencies = [
-    "LbAPCommon>=0.10.2",
+    "LbAPCommon>=0.10.3",
     "LbDiracWrappers",
     "LbEnv",
     "LbProdRun~=1.3",
     "apd>=0.6.0",
     "click",
     "consolemd",
     "mplhep",
```

### Comparing `LbAPLocal-0.7.2/src/LbAPLocal/__init__.py` & `LbAPLocal-0.7.3/src/LbAPLocal/__init__.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/src/LbAPLocal/checks.py` & `LbAPLocal-0.7.3/src/LbAPLocal/checks.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/src/LbAPLocal/cli.py` & `LbAPLocal-0.7.3/src/LbAPLocal/cli.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/src/LbAPLocal/log_parsing.py` & `LbAPLocal-0.7.3/src/LbAPLocal/log_parsing.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/src/LbAPLocal/testing.py` & `LbAPLocal-0.7.3/src/LbAPLocal/testing.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/src/LbAPLocal/utils.py` & `LbAPLocal-0.7.3/src/LbAPLocal/utils.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/src/LbAPLocal.egg-info/PKG-INFO` & `LbAPLocal-0.7.3/src/LbAPLocal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LbAPLocal
-Version: 0.7.2
+Version: 0.7.3
 Summary: Tool to locally run tests for AnalysisProductions
 Author: LHCb
 Project-URL: Homepage, https://gitlab.cern.ch/lhcb-dpa/analysis-productions/lbaplocal
 Project-URL: Bug Reports, https://gitlab.cern.ch/lhcb-dpa/analysis-productions/lbaplocal/-/issues
 Project-URL: Source, https://gitlab.cern.ch/lhcb-dpa/analysis-productions/lbaplocal
 Keywords: LHCb AnalysisProductions DIRAC
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LbAPLocal-0.7.2/src/LbAPLocal.egg-info/SOURCES.txt` & `LbAPLocal-0.7.3/src/LbAPLocal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/cassettes/test_execute/test_run_test[2016_MagDown_PromptMC_D02KK-2444].yaml` & `LbAPLocal-0.7.3/tests/cassettes/test_execute/test_run_test[2016_MagDown_PromptMC_D02KK-2444].yaml`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/cassettes/test_execute/test_run_test[2016_MagDown_PromptMC_D02KK_noautoconf-2444].yaml` & `LbAPLocal-0.7.3/tests/cassettes/test_execute/test_run_test[2016_MagDown_PromptMC_D02KK_noautoconf-2444].yaml`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/cassettes/test_execute/test_run_test[2016_MagUp_PromptMC_D02KK-2393].yaml` & `LbAPLocal-0.7.3/tests/cassettes/test_execute/test_run_test[2016_MagUp_PromptMC_D02KK-2393].yaml`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/cassettes/test_execute/test_run_test[2016_MagUp_PromptMC_D02KK_noautoconf-2393].yaml` & `LbAPLocal-0.7.3/tests/cassettes/test_execute/test_run_test[2016_MagUp_PromptMC_D02KK_noautoconf-2393].yaml`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/conftest.py` & `LbAPLocal-0.7.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/.gitignore` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/.gitignore`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/.gitlab-ci.yml` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bc2Bspi2JpsiPhi.py` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bc2Bspi2JpsiPhi.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bd2JpsiKstar.py` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bd2JpsiKstar.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2DsPi.py` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2DsPi.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi.py` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi_Prompt.py` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi_Prompt.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi_Prompt_PVMixer.py` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi_Prompt_PVMixer.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi_Swave.py` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi_Swave.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bu2JpsiKplus.py` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bu2JpsiKplus.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/README.md` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/README.md`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/helpers/stripping.py` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/helpers/stripping.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/helpers/tuple_maker.py` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/helpers/tuple_maker.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/info.yaml` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/info.yaml`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/BsToJpsiPhi/sequence_setup.py` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/BsToJpsiPhi/sequence_setup.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/COPYING` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/COPYING`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/RDs/Run1_Signal.py` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/RDs/Run1_Signal.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/RDs/Run2_Signal.py` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/RDs/Run2_Signal.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/RDs/helpers/signal_tuple_maker.py` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/RDs/helpers/signal_tuple_maker.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/RDs/info.yaml` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/RDs/info.yaml`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/README.md` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/README.md`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/README.md` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/README.md`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/helpers/MC_tuple_maker.py` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/helpers/MC_tuple_maker.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/helpers/decay_descriptors.py` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/helpers/decay_descriptors.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/helpers/locations.py` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/helpers/locations.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/helpers/related_info.py` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/helpers/related_info.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/helpers/stripping.py` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/helpers/stripping.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/helpers/tags.py` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/helpers/tags.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/helpers/tuple_maker.py` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/helpers/tuple_maker.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/info.yaml` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/info.yaml`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/sequence_setup.py` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/sequence_setup.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/cbtesting/stripping_seq.py` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/cbtesting/stripping_seq.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/executabletests/info.yaml` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/executabletests/info.yaml`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/data-pkg-repo/executabletests/ntuple_options.py` & `LbAPLocal-0.7.3/tests/data/data-pkg-repo/executabletests/ntuple_options.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/example-logs/error-failed-to-read-file.log` & `LbAPLocal-0.7.3/tests/data/example-logs/error-failed-to-read-file.log`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/example-logs/error-illegal-instruction.log` & `LbAPLocal-0.7.3/tests/data/example-logs/error-illegal-instruction.log`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/example-logs/error-missing-shared-library.log` & `LbAPLocal-0.7.3/tests/data/example-logs/error-missing-shared-library.log`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/example-logs/error-platform-unsupported.log` & `LbAPLocal-0.7.3/tests/data/example-logs/error-platform-unsupported.log`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/example-logs/error-related-info-missing.log` & `LbAPLocal-0.7.3/tests/data/example-logs/error-related-info-missing.log`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/example-logs/good-DaVinci_00110296_00000038_1.log` & `LbAPLocal-0.7.3/tests/data/example-logs/good-DaVinci_00110296_00000038_1.log`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/example-logs/good-DaVinci_00110296_00000194_1.log` & `LbAPLocal-0.7.3/tests/data/example-logs/good-DaVinci_00110296_00000194_1.log`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/data/example-logs/good-Gauss_00104988_00000011_1.log` & `LbAPLocal-0.7.3/tests/data/example-logs/good-Gauss_00104988_00000011_1.log`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/test_cli.py` & `LbAPLocal-0.7.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/test_execute.py` & `LbAPLocal-0.7.3/tests/test_execute.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/test_local_datapkg.py` & `LbAPLocal-0.7.3/tests/test_local_datapkg.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.7.2/tests/test_log_parse.py` & `LbAPLocal-0.7.3/tests/test_log_parse.py`

 * *Files identical despite different names*

