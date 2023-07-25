# Comparing `tmp/prismstudio-dev-1.1.7.tar.gz` & `tmp/prismstudio-dev-1.1.7a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prismstudio-dev-1.1.7.tar", last modified: Sat Jul 15 01:01:27 2023, max compression
+gzip compressed data, was "prismstudio-dev-1.1.7a0.tar", last modified: Tue Jul 25 13:58:11 2023, max compression
```

## Comparing `prismstudio-dev-1.1.7.tar` & `prismstudio-dev-1.1.7a0.tar`

### file list

```diff
@@ -1,89 +1,98 @@
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-15 01:01:27.633500 prismstudio-dev-1.1.7/
--rw-rw-r--   0 prism     (1000) prism     (1000)    23016 2023-07-09 08:09:32.000000 prismstudio-dev-1.1.7/LICENSE.txt
--rw-rw-r--   0 prism     (1000) prism     (1000)      444 2023-07-15 01:01:27.633500 prismstudio-dev-1.1.7/PKG-INFO
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-15 01:01:27.633500 prismstudio-dev-1.1.7/prism/
--rw-rw-r--   0 prism     (1000) prism     (1000)     1177 2023-07-07 08:39:02.000000 prismstudio-dev-1.1.7/prism/__init__.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-15 01:01:27.633500 prismstudio-dev-1.1.7/prism/_common/
--rw-rw-r--   0 prism     (1000) prism     (1000)       28 2023-07-15 01:01:24.000000 prismstudio-dev-1.1.7/prism/_common/.env
--rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_common/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     3472 2023-07-09 08:26:49.000000 prismstudio-dev-1.1.7/prism/_common/config.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    10482 2023-07-15 01:00:00.000000 prismstudio-dev-1.1.7/prism/_common/const.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-15 01:01:27.633500 prismstudio-dev-1.1.7/prism/_core/
--rw-rw-r--   0 prism     (1000) prism     (1000)      251 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_core/__init__.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-15 01:01:27.633500 prismstudio-dev-1.1.7/prism/_core/_data/
--rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_core/_data/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    41177 2023-06-16 00:01:45.000000 prismstudio-dev-1.1.7/prism/_core/_data/estimate.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     7950 2023-06-16 00:01:45.000000 prismstudio-dev-1.1.7/prism/_core/_data/event.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    70894 2023-07-09 08:09:32.000000 prismstudio-dev-1.1.7/prism/_core/_data/financial.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    12927 2023-07-15 00:59:57.000000 prismstudio-dev-1.1.7/prism/_core/_data/index.py
--rw-rw-r--   0 prism     (1000) prism     (1000)   121051 2023-06-16 00:01:45.000000 prismstudio-dev-1.1.7/prism/_core/_data/industry.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    36768 2023-07-07 02:42:51.000000 prismstudio-dev-1.1.7/prism/_core/_data/market.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     6446 2023-06-16 00:01:45.000000 prismstudio-dev-1.1.7/prism/_core/_data/precalculated.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     3840 2023-06-14 16:37:45.000000 prismstudio-dev-1.1.7/prism/_core/_data/securitymaster.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    15625 2023-06-15 23:39:09.000000 prismstudio-dev-1.1.7/prism/_core/_fn.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-15 01:01:27.633500 prismstudio-dev-1.1.7/prism/_core/_req_builder/
--rw-rw-r--   0 prism     (1000) prism     (1000)     1458 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_core/_req_builder/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1450 2023-07-13 01:40:27.000000 prismstudio-dev-1.1.7/prism/_core/_req_builder/_auth.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    22657 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_core/_req_builder/_dataquery.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2058 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_core/_req_builder/_dbinfo.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     7633 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_core/_req_builder/_exportdata.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     3633 2023-06-15 23:39:09.000000 prismstudio-dev-1.1.7/prism/_core/_req_builder/_gui.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    15003 2023-06-14 16:37:45.000000 prismstudio-dev-1.1.7/prism/_core/_req_builder/_job.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     4582 2023-06-14 16:37:45.000000 prismstudio-dev-1.1.7/prism/_core/_req_builder/_list.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    15321 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_core/_req_builder/_portfolio.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     4295 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_core/_req_builder/_securitymaster.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    25699 2023-06-15 23:39:09.000000 prismstudio-dev-1.1.7/prism/_core/_req_builder/_task.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    10877 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_core/_req_builder/_taskquery.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    24533 2023-06-14 16:37:45.000000 prismstudio-dev-1.1.7/prism/_core/_req_builder/_universe.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     8696 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_core/_req_builder/preference.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     9606 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_core/ols.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-15 01:01:27.633500 prismstudio-dev-1.1.7/prism/_prismcomponent/
--rw-rw-r--   0 prism     (1000) prism     (1000)      353 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_prismcomponent/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     7644 2023-07-15 01:00:00.000000 prismstudio-dev-1.1.7/prism/_prismcomponent/abstract_prismcomponent.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    11256 2023-07-15 01:00:00.000000 prismstudio-dev-1.1.7/prism/_prismcomponent/datacomponent.py
--rw-rw-r--   0 prism     (1000) prism     (1000)   185816 2023-07-15 01:00:00.000000 prismstudio-dev-1.1.7/prism/_prismcomponent/prismcomponent.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    21567 2023-07-07 02:42:51.000000 prismstudio-dev-1.1.7/prism/_prismcomponent/taskcomponent.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-15 01:01:27.633500 prismstudio-dev-1.1.7/prism/_utils/
--rw-rw-r--   0 prism     (1000) prism     (1000)      480 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_utils/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2248 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_utils/auth_utils.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     3629 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_utils/exceptions.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2028 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_utils/loader.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     3706 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_utils/prismcomponent_utils.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     5532 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_utils/req_builder_utils.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    14289 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_utils/validate_utils.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     7232 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_utils/validate_utils_refactored.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1438 2023-07-07 02:42:51.000000 prismstudio-dev-1.1.7/prism/_utils/version.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-15 01:01:27.633500 prismstudio-dev-1.1.7/prismstudio_dev.egg-info/
--rw-rw-r--   0 prism     (1000) prism     (1000)      444 2023-07-15 01:01:27.000000 prismstudio-dev-1.1.7/prismstudio_dev.egg-info/PKG-INFO
--rw-rw-r--   0 prism     (1000) prism     (1000)     3042 2023-07-15 01:01:27.000000 prismstudio-dev-1.1.7/prismstudio_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 prism     (1000) prism     (1000)        1 2023-07-15 01:01:27.000000 prismstudio-dev-1.1.7/prismstudio_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 prism     (1000) prism     (1000)      256 2023-07-15 01:01:27.000000 prismstudio-dev-1.1.7/prismstudio_dev.egg-info/requires.txt
--rw-rw-r--   0 prism     (1000) prism     (1000)       12 2023-07-15 01:01:27.000000 prismstudio-dev-1.1.7/prismstudio_dev.egg-info/top_level.txt
--rw-rw-r--   0 prism     (1000) prism     (1000)       91 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/pyproject.toml
--rw-rw-r--   0 prism     (1000) prism     (1000)       38 2023-07-15 01:01:27.633500 prismstudio-dev-1.1.7/setup.cfg
--rw-rw-r--   0 prism     (1000) prism     (1000)     1341 2023-07-09 08:09:32.000000 prismstudio-dev-1.1.7/setup.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-15 01:01:27.633500 prismstudio-dev-1.1.7/tests/
--rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/__init__.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-15 01:01:27.633500 prismstudio-dev-1.1.7/tests/test_util/
--rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/__init__.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-15 01:01:27.633500 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/
--rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2200 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_common_functions.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1539 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_fillna.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-15 01:01:27.633500 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/
--rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     5990 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_01_frequency.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2004 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_02_datetype.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2719 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_03_periodtype.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1615 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_04_adjustment.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2304 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_05_shownid.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1946 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_06_rank_method.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2302 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_07_method.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     6448 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_08_in_startdate_or_enddate.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     3854 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_09_contains_universename.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1717 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_10_contains_min_periods.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1118 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_11_base.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1792 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_12_preliminary.py
--rw-rw-r--   0 prism     (1000) prism     (1000)      889 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_13_setting.py
--rw-rw-r--   0 prism     (1000) prism     (1000)      956 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_14_settings.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1770 2023-07-07 02:42:51.000000 prismstudio-dev-1.1.7/tests/test_util/test_version.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-25 13:58:11.254202 prismstudio-dev-1.1.7a0/
+-rw-rw-r--   0 prism     (1000) prism     (1000)    23016 2023-07-09 08:09:32.000000 prismstudio-dev-1.1.7a0/LICENSE.txt
+-rw-rw-r--   0 prism     (1000) prism     (1000)      446 2023-07-25 13:58:11.254202 prismstudio-dev-1.1.7a0/PKG-INFO
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-25 13:58:11.250202 prismstudio-dev-1.1.7a0/prism/
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1177 2023-07-07 08:39:02.000000 prismstudio-dev-1.1.7a0/prism/__init__.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-25 13:58:11.250202 prismstudio-dev-1.1.7a0/prism/_common/
+-rw-rw-r--   0 prism     (1000) prism     (1000)       29 2023-07-25 13:58:08.000000 prismstudio-dev-1.1.7a0/prism/_common/.env
+-rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_common/__init__.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     3472 2023-07-09 08:26:49.000000 prismstudio-dev-1.1.7a0/prism/_common/config.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    11029 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/prism/_common/const.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-25 13:58:11.250202 prismstudio-dev-1.1.7a0/prism/_core/
+-rw-rw-r--   0 prism     (1000) prism     (1000)      288 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/prism/_core/__init__.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-25 13:58:11.254202 prismstudio-dev-1.1.7a0/prism/_core/_data/
+-rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_core/_data/__init__.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    10231 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/prism/_core/_data/esg.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    41180 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/prism/_core/_data/estimate.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     7950 2023-06-16 00:01:45.000000 prismstudio-dev-1.1.7a0/prism/_core/_data/event.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    70894 2023-07-09 08:09:32.000000 prismstudio-dev-1.1.7a0/prism/_core/_data/financial.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    12927 2023-07-15 00:59:57.000000 prismstudio-dev-1.1.7a0/prism/_core/_data/index.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)   121051 2023-06-16 00:01:45.000000 prismstudio-dev-1.1.7a0/prism/_core/_data/industry.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    37342 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/prism/_core/_data/market.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     6446 2023-06-16 00:01:45.000000 prismstudio-dev-1.1.7a0/prism/_core/_data/precalculated.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     3840 2023-06-14 16:37:45.000000 prismstudio-dev-1.1.7a0/prism/_core/_data/securitymaster.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    15625 2023-06-15 23:39:09.000000 prismstudio-dev-1.1.7a0/prism/_core/_fn.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-25 13:58:11.254202 prismstudio-dev-1.1.7a0/prism/_core/_req_builder/
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1458 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_core/_req_builder/__init__.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     2074 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_auth.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    22677 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_dataquery.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     2058 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_dbinfo.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     7633 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_exportdata.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     3633 2023-06-15 23:39:09.000000 prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_gui.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    15003 2023-06-14 16:37:45.000000 prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_job.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     4828 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_list.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    15321 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_portfolio.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     4295 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_securitymaster.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    25699 2023-06-15 23:39:09.000000 prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_task.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    10877 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_taskquery.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    24533 2023-06-14 16:37:45.000000 prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_universe.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     8696 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_core/_req_builder/preference.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     9606 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_core/ols.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-25 13:58:11.254202 prismstudio-dev-1.1.7a0/prism/_prismcomponent/
+-rw-rw-r--   0 prism     (1000) prism     (1000)      353 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_prismcomponent/__init__.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     7644 2023-07-15 01:00:00.000000 prismstudio-dev-1.1.7a0/prism/_prismcomponent/abstract_prismcomponent.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    12663 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/prism/_prismcomponent/datacomponent.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)   186982 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/prism/_prismcomponent/prismcomponent.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    21567 2023-07-07 02:42:51.000000 prismstudio-dev-1.1.7a0/prism/_prismcomponent/taskcomponent.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-25 13:58:11.254202 prismstudio-dev-1.1.7a0/prism/_utils/
+-rw-rw-r--   0 prism     (1000) prism     (1000)      480 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_utils/__init__.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     2248 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_utils/auth_utils.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     3629 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_utils/exceptions.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     2028 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_utils/loader.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     3706 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_utils/prismcomponent_utils.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     5532 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_utils/req_builder_utils.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    14289 2023-07-18 01:25:58.000000 prismstudio-dev-1.1.7a0/prism/_utils/validate_utils.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     7232 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_utils/validate_utils_refactored.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1438 2023-07-07 02:42:51.000000 prismstudio-dev-1.1.7a0/prism/_utils/version.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-25 13:58:11.254202 prismstudio-dev-1.1.7a0/prismstudio_dev.egg-info/
+-rw-rw-r--   0 prism     (1000) prism     (1000)      446 2023-07-25 13:58:11.000000 prismstudio-dev-1.1.7a0/prismstudio_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 prism     (1000) prism     (1000)     3097 2023-07-25 13:58:11.000000 prismstudio-dev-1.1.7a0/prismstudio_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 prism     (1000) prism     (1000)        1 2023-07-25 13:58:11.000000 prismstudio-dev-1.1.7a0/prismstudio_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 prism     (1000) prism     (1000)      242 2023-07-25 13:58:11.000000 prismstudio-dev-1.1.7a0/prismstudio_dev.egg-info/requires.txt
+-rw-rw-r--   0 prism     (1000) prism     (1000)       12 2023-07-25 13:58:11.000000 prismstudio-dev-1.1.7a0/prismstudio_dev.egg-info/top_level.txt
+-rw-rw-r--   0 prism     (1000) prism     (1000)      137 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/pyproject.toml
+-rw-rw-r--   0 prism     (1000) prism     (1000)       38 2023-07-25 13:58:11.254202 prismstudio-dev-1.1.7a0/setup.cfg
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1316 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/setup.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-25 13:58:11.254202 prismstudio-dev-1.1.7a0/tests/
+-rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/tests/__init__.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)       94 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/conftest.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-25 13:58:11.254202 prismstudio-dev-1.1.7a0/tests/test__validate_args/
+-rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/__init__.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     2200 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_common_functions.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1539 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_fillna.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-25 13:58:11.254202 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/
+-rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/__init__.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     5990 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_01_frequency.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     2004 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_02_datetype.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     2719 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_03_periodtype.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1615 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_04_adjustment.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     2304 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_05_shownid.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1946 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_06_rank_method.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     2302 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_07_method.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     6448 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_08_in_startdate_or_enddate.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     3854 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_09_contains_universename.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1717 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_10_contains_min_periods.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1118 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_11_base.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1792 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_12_preliminary.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)      889 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_13_setting.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)      956 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_14_settings.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     2441 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test_factors.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-25 13:58:11.254202 prismstudio-dev-1.1.7a0/tests/test_util/
+-rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/tests/test_util/__init__.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)      603 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test_util/db_fixtures.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1264 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test_util/dq_model.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1753 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test_util/dq_table.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    15617 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test_util/factor_fixtures.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     2738 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test_util/update_factor.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1259 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test_util/utils.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1770 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test_version.py
```

### Comparing `prismstudio-dev-1.1.7/LICENSE.txt` & `prismstudio-dev-1.1.7a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prism/__init__.py` & `prismstudio-dev-1.1.7a0/prism/__init__.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prism/_common/config.py` & `prismstudio-dev-1.1.7a0/prism/_common/config.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prism/_common/const.py` & `prismstudio-dev-1.1.7a0/prism/_common/const.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,20 @@
 ACTIVE_DATE = pd.to_datetime('2199-12-31')
 
 
 class PrismComponentType(str, Enum):
     FUNCTION_COMPONENT = 'functioncomponent'
     DATA_COMPONENT = 'datacomponent'
     TASK_COMPONENT = 'taskcomponent'
+    MODEL_COMPONENT = 'modelcomponent'
+
+
+class TCModelComponentType(str, Enum):
+    ALMGREN = "Almgren"
+    BIDASKSPREAD = "Bid-Ask Spread"
 
 
 SMValues = None
 PreferenceType = None
 
 
 class AdjustmentType(Enum):
@@ -129,24 +135,35 @@
 class TaskComponentType(str, Enum):
     SCREEN = 'screen'
     FACTOR_BACKTEST = 'factor_backtest'
     STRATEGY_BACKTEST = 'strategy_backtest'
     EXPORT_DATA = 'export_data'
 
 
+class PrismModelCategoryType(str, Enum):
+    TC = "Transaction Cost"
+
 class DataCategoryType(str, Enum):
     FINANCIAL = "Financial"
     PRECALCAULATED = "Precalculated"
     EVENT = "Event"
     SM = "Securitymaster"
     MARKET = "Market"
     ESTIMATE = "Estimate"
     INDEX = "Index"
     INDUSTRY_ESTIMATE = "Industry Estimate"
     INDUSTRY_FINANCIAL = "Industry"
+    ESG = "ESG"
+
+
+class ESGDataComponentType(str, Enum):
+    ENVIRONMENTAL = 'Environmental'
+    SOCIAL = 'Social'
+    GOVERNANCE = 'Governance'
+    SUMMARY = 'Summary'
 
 
 class FinancialDataComponentType(str, Enum):
     BALANCE_SHEET = 'Balance Sheet'
     CASH_FLOW = 'Cash Flow'
     DPS = 'DPS'
     EPS = 'EPS'
@@ -180,14 +197,17 @@
     VOLUME = 'Volume'
     DIVIDEND = 'Dividend'
     DIVIDEND_ADJ_FACTOR = 'Dividend Adjustment Factor'
     EXCHANGERATE = 'Exchange Rate'
     SHORT_INTEREST = 'Short Interest'
     SPLIT = 'Split'
     SPLIT_ADJ_FACTOR = 'Split Adjustment Factor'
+    SHARES_OUTSTANDING = 'Shares Outstanding'
+    TOTAL_ENTERPRISE_VALUE = 'Total Enterprise Value'
+    IMPLIED_MARKET_CAPITALIZATION = 'Implied Market Capitalization'
 
 
 class PrecalculatedDataComponentType(str, Enum):
     AFL = 'Alpha Factor Library'
 
 
 class IndexDataComponentType(str, Enum):
```

### Comparing `prismstudio-dev-1.1.7/prism/_core/_data/estimate.py` & `prismstudio-dev-1.1.7a0/prism/_core/_data/estimate.py`

 * *Files 0% similar despite different names*

```diff
@@ -563,15 +563,15 @@
     -------
         prism._PrismComponent
 
     Examples
     --------
         >>> di = prism.estimate.surprise_dataitems('revenue')
         >>> di[['dataitemid', 'dataitemname']]
-        dataitemid                   dataitemname
+           dataitemid                   dataitemname
         0      200618  Revenue - Surpise, Difference
         1      200619     Revenue - Surpise, Percent
 
         >>> rev = prism.estimate.surprise(dataitemid=200618, periodtype='Q')
         >>> rev_df = rev.get_data(universe='S&P 500', startdate='2010-01-01', enddate='2015-12-31', shownid=['ticker'])
         >>> rev_df
                listingid      period        date  EPS Normalized - Surpise, Difference  Ticker
```

### Comparing `prismstudio-dev-1.1.7/prism/_core/_data/event.py` & `prismstudio-dev-1.1.7a0/prism/_core/_data/event.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prism/_core/_data/financial.py` & `prismstudio-dev-1.1.7a0/prism/_core/_data/financial.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prism/_core/_data/index.py` & `prismstudio-dev-1.1.7a0/prism/_core/_data/index.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prism/_core/_data/industry.py` & `prismstudio-dev-1.1.7a0/prism/_core/_data/industry.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prism/_core/_data/market.py` & `prismstudio-dev-1.1.7a0/prism/_core/_data/market.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,17 @@
     _Volume,
     _Dividend,
     _DividendAdjustmentFactor,
     _Split,
     _SplitAdjustmentFactor,
     _ExchangeRate,
     _ShortInterest,
+    _SharesOutstanding,
+    _TotalEnterpriseValue,
+    _ImpliedMarketCapitalization
 )
 from ..._utils.validate_utils import _validate_args
 
 
 __all__ = [
     'open',
     'close',
@@ -36,14 +39,17 @@
     'exchange_rate',
     'short_interest',
     'split',
     'split_adjustment_factor',
     'dividend_adjustment_factor',
     'dataitems',
     'short_interest_dataitems',
+    'shares_outstanding',
+    'enterprise_value',
+    'implied_market_cap'
 ]
 
 
 @_validate_args
 def _build_price(
     datacomponentclass,
     adjustment: Union[str, bool] = None,
@@ -907,19 +913,34 @@
             - *datamodule : str*
             - *datacomponent : str*
             - *packagename : str*
 
     Examples
     --------
         >>> prism.market.short_interest_dataitems(search='short')
-           dataitemid                               dataitemname  ...  datamodule                packagename
+           dataitemid         ;                      dataitemname  ...  datamodule                packagename
         0     1100035                Broker Short Interest Value  ...        None  IHS Markit Short Interest
         1     1100055        Short Interest Ratio (Day to Cover)  ...        None  IHS Markit Short Interest
         2     1100056                      Short Interest Tenure  ...        None  IHS Markit Short Interest
         3     1100057                       Short Interest Value  ...        None  IHS Markit Short Interest
         4     1100058          Short Interest as % Of Free Float  ...        None  IHS Markit Short Interest
         5     1100059  Short Interest as % Of Shares Outstanding  ...        None  IHS Markit Short Interest
         6     1100060                                Short Score  ...        None  IHS Markit Short Interest
         7     1100063           Supply Side Short Interest Value  ...        None  IHS Markit Short Interest
     """
 
     return _list_dataitem_market(_MarketDataComponentType.SHORT_INTEREST, search, package)
+
+
+@_validate_args
+def shares_outstanding(adjustment: Union[str, bool] = True):
+    return _SharesOutstanding(adjustment=adjustment)
+
+
+@_validate_args
+def enterprise_value(currency: str = 'trade'):
+    return _TotalEnterpriseValue(currency=currency)
+
+
+@_validate_args
+def implied_market_cap(include: str = 'all', currency: str = 'trade'):
+    return _ImpliedMarketCapitalization(include=include, currency=currency)
```

### Comparing `prismstudio-dev-1.1.7/prism/_core/_data/precalculated.py` & `prismstudio-dev-1.1.7a0/prism/_core/_data/precalculated.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prism/_core/_data/securitymaster.py` & `prismstudio-dev-1.1.7a0/prism/_core/_data/securitymaster.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prism/_core/_fn.py` & `prismstudio-dev-1.1.7a0/prism/_core/_fn.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prism/_core/_req_builder/__init__.py` & `prismstudio-dev-1.1.7a0/prism/_core/_req_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prism/_core/_req_builder/_dataquery.py` & `prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_dataquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -403,15 +403,15 @@
     cmpts = set()
     if isinstance(name, list) & (name is not None):
         if any([not isinstance(n, str) for n in name]):
             raise PrismTypeError('Names shoud be string')
 
     def add_cmpts(o):
         cmpts = set()
-        if o["component_type"] == "datacomponent":
+        if o["component_type"] in ["datacomponent", "modelcomponent"]:
             cmpts.add(o["component_name"])
         else:
             for c in o["children"]:
                 cmpts = cmpts | add_cmpts(c)
         return cmpts
 
     if not isinstance(component, list):
```

### Comparing `prismstudio-dev-1.1.7/prism/_core/_req_builder/_dbinfo.py` & `prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_dbinfo.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prism/_core/_req_builder/_exportdata.py` & `prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_exportdata.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prism/_core/_req_builder/_gui.py` & `prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_gui.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prism/_core/_req_builder/_job.py` & `prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_job.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prism/_core/_req_builder/_list.py` & `prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,20 +92,26 @@
 @_validate_args
 def _list_dataitem_estimate(datacomponent, search : str = None, package : str = None):
     param = {'datacategory': 'Estimate', 'datacomponent': datacomponent, 'search': search, 'package': package}
     return get(URL_DATAITEMS, param)
 
 
 @_validate_args
-def _list_dataitem_market(datacomponent: str, search : str = None, package : str = None):
+def _list_dataitem_market(datacomponent: str, search : str = None, package: str = None):
     param = {'datacategory': 'Market', 'datacomponent': datacomponent, 'search': search, 'package': package}
     return get(URL_DATAITEMS, param)
 
 
 @_validate_args
+def _list_dataitems_esg(datacomponent: str, search: str = None, package: str = None):
+    param = {'datacategory': 'ESG', 'datacomponent': datacomponent, 'search': search, 'package': package}
+    return get(URL_DATAITEMS, param)
+
+
+@_validate_args
 def _list_dataitem_precalculated(datacomponent: str, search : str = None, package : str = None):
     param = {'datacategory': 'Precalculated', 'datacomponent': datacomponent, 'search': search, 'package': package}
     return get(URL_DATAITEMS, param)
 
 
 @_validate_args
 def _list_dataitem_index(datacomponent: str, search : str = None, package : str = None):
```

### Comparing `prismstudio-dev-1.1.7/prism/_core/_req_builder/_portfolio.py` & `prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_portfolio.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prism/_core/_req_builder/_securitymaster.py` & `prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_securitymaster.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prism/_core/_req_builder/_task.py` & `prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_task.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prism/_core/_req_builder/_taskquery.py` & `prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_taskquery.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prism/_core/_req_builder/_universe.py` & `prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_universe.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prism/_core/_req_builder/preference.py` & `prismstudio-dev-1.1.7a0/prism/_core/_req_builder/preference.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prism/_core/ols.py` & `prismstudio-dev-1.1.7a0/prism/_core/ols.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prism/_prismcomponent/abstract_prismcomponent.py` & `prismstudio-dev-1.1.7a0/prism/_prismcomponent/abstract_prismcomponent.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prism/_prismcomponent/datacomponent.py` & `prismstudio-dev-1.1.7a0/prism/_prismcomponent/datacomponent.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     MarketDataComponentType,
     PrecalculatedDataComponentType,
     IndexDataComponentType,
     EventDataComponentType,
     OtherDataComponentType,
     IndustryComponentType,
     DataCategoryType,
+    ESGDataComponentType
 )
 from .._core._req_builder import _dataquery
 from .._prismcomponent.prismcomponent import _PrismComponent, _PrismDataComponent, _PrismFinancialComponent
 from .._utils import _validate_args, _req_call
 
 
 # ------------------------------------------------------------------------------------------------------------------- #
@@ -84,14 +85,26 @@
 
     @_validate_args
     @_req_call(_dataquery)
     def get_data(self, startdate: str = None, enddate: str = None, name = None,) -> pd.DataFrame:
         pass
 
 
+class _SharesOutstanding(_PrismMarketComponent):
+    _component_name = MarketDataComponentType.SHARES_OUTSTANDING
+
+
+class _TotalEnterpriseValue(_PrismMarketComponent):
+    _component_name = MarketDataComponentType.TOTAL_ENTERPRISE_VALUE
+
+
+class _ImpliedMarketCapitalization(_PrismMarketComponent):
+    _component_name = MarketDataComponentType.IMPLIED_MARKET_CAPITALIZATION
+
+
 # ------------------------------------------------------------------------------------------------------------------- #
 #                                                      Financial                                                      #
 # ------------------------------------------------------------------------------------------------------------------- #
 class _BalanceSheet(_PrismDataComponent, _PrismFinancialComponent):
     _component_category = DataCategoryType.FINANCIAL
     _component_name = FinancialDataComponentType.BALANCE_SHEET
 
@@ -307,7 +320,34 @@
 
 class _Telecom(_PrismIndustryFinancialComponent):
     _component_name = IndustryComponentType.TELECOM
 
 
 class _Utility(_PrismIndustryFinancialComponent):
     _component_name = IndustryComponentType.UTILITY
+
+
+# ------------------------------------------------------------------------------------------------------------------- #
+#                                                       ESG                                                      #
+# ------------------------------------------------------------------------------------------------------------------- #
+class _PrismESGComponent(_PrismDataComponent, _PrismComponent):
+    _component_category = DataCategoryType.ESG
+    # @_validate_args
+    # @_req_call(_dataquery)
+    # def get_data(self, startdate: str = None, enddate: str = None, name = None,) -> pd.DataFrame:
+    #     pass
+
+
+class _Environmental(_PrismESGComponent):
+    _component_name = ESGDataComponentType.ENVIRONMENTAL
+
+
+class _Social(_PrismESGComponent):
+    _component_name = ESGDataComponentType.SOCIAL
+
+
+class _Governance(_PrismESGComponent):
+    _component_name = ESGDataComponentType.GOVERNANCE
+
+
+class _Summary(_PrismESGComponent):
+    _component_name = ESGDataComponentType.SUMMARY
```

### Comparing `prismstudio-dev-1.1.7/prism/_prismcomponent/prismcomponent.py` & `prismstudio-dev-1.1.7a0/prism/_prismcomponent/prismcomponent.py`

 * *Files 1% similar despite different names*

```diff
@@ -4548,7 +4548,36 @@
         Returns
         -------
             prism._PrismFinancialComponent
                 n fiscal quarters sum timeseries of the PrismFinancialComponent.
         """
         if (weights is not None) and (len(weights) != n):
             raise PrismValueError("Number of weights should equal to n")
+
+
+class _PrismModelComponent(_PrismComponent):
+    _component_type = PrismComponentType.MODEL_COMPONENT
+
+    def __init__(self, **kwargs):
+        component_args = dict(kwargs)
+        children = [] if "children" not in component_args else component_args.pop("children")
+        query = {
+            "component_type": self._component_type,
+            "component_category": self._component_category,
+            "component_name": self._component_name,
+            "component_args": component_args,
+            "children": children,
+            "nodeid": str(uuid.uuid4()),
+        }
+        val_res = requests.post(url=URL_DATAQUERIES + "/validate", json=query, headers=_authentication())
+        if val_res.status_code >= 400:
+            if val_res.status_code == 401:
+                raise PrismAuthError(f"Please Login First")
+            else:
+                try:
+                    err_msg = val_res.json()["message"]
+                except:
+                    err_msg = val_res.content
+                raise PrismResponseError(err_msg)
+        query = val_res.json()["rescontent"]["data"]
+        query.pop("query_name")
+        super().__init__(**query)
```

### Comparing `prismstudio-dev-1.1.7/prism/_prismcomponent/taskcomponent.py` & `prismstudio-dev-1.1.7a0/prism/_prismcomponent/taskcomponent.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prism/_utils/auth_utils.py` & `prismstudio-dev-1.1.7a0/prism/_utils/auth_utils.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prism/_utils/exceptions.py` & `prismstudio-dev-1.1.7a0/prism/_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prism/_utils/loader.py` & `prismstudio-dev-1.1.7a0/prism/_utils/loader.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prism/_utils/prismcomponent_utils.py` & `prismstudio-dev-1.1.7a0/prism/_utils/prismcomponent_utils.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prism/_utils/req_builder_utils.py` & `prismstudio-dev-1.1.7a0/prism/_utils/req_builder_utils.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prism/_utils/validate_utils.py` & `prismstudio-dev-1.1.7a0/prism/_utils/validate_utils.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prism/_utils/validate_utils_refactored.py` & `prismstudio-dev-1.1.7a0/prism/_utils/validate_utils_refactored.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prism/_utils/version.py` & `prismstudio-dev-1.1.7a0/prism/_utils/version.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/prismstudio_dev.egg-info/SOURCES.txt` & `prismstudio-dev-1.1.7a0/prismstudio_dev.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 prism/_common/__init__.py
 prism/_common/config.py
 prism/_common/const.py
 prism/_core/__init__.py
 prism/_core/_fn.py
 prism/_core/ols.py
 prism/_core/_data/__init__.py
+prism/_core/_data/esg.py
 prism/_core/_data/estimate.py
 prism/_core/_data/event.py
 prism/_core/_data/financial.py
 prism/_core/_data/index.py
 prism/_core/_data/industry.py
 prism/_core/_data/market.py
 prism/_core/_data/precalculated.py
@@ -48,27 +49,35 @@
 prism/_utils/version.py
 prismstudio_dev.egg-info/PKG-INFO
 prismstudio_dev.egg-info/SOURCES.txt
 prismstudio_dev.egg-info/dependency_links.txt
 prismstudio_dev.egg-info/requires.txt
 prismstudio_dev.egg-info/top_level.txt
 tests/__init__.py
+tests/conftest.py
+tests/test_factors.py
+tests/test_version.py
+tests/test__validate_args/__init__.py
+tests/test__validate_args/test_common_functions.py
+tests/test__validate_args/test_fillna.py
+tests/test__validate_args/test_params/__init__.py
+tests/test__validate_args/test_params/test_param_01_frequency.py
+tests/test__validate_args/test_params/test_param_02_datetype.py
+tests/test__validate_args/test_params/test_param_03_periodtype.py
+tests/test__validate_args/test_params/test_param_04_adjustment.py
+tests/test__validate_args/test_params/test_param_05_shownid.py
+tests/test__validate_args/test_params/test_param_06_rank_method.py
+tests/test__validate_args/test_params/test_param_07_method.py
+tests/test__validate_args/test_params/test_param_08_in_startdate_or_enddate.py
+tests/test__validate_args/test_params/test_param_09_contains_universename.py
+tests/test__validate_args/test_params/test_param_10_contains_min_periods.py
+tests/test__validate_args/test_params/test_param_11_base.py
+tests/test__validate_args/test_params/test_param_12_preliminary.py
+tests/test__validate_args/test_params/test_param_13_setting.py
+tests/test__validate_args/test_params/test_param_14_settings.py
 tests/test_util/__init__.py
-tests/test_util/test_version.py
-tests/test_util/test__validate_args/__init__.py
-tests/test_util/test__validate_args/test_common_functions.py
-tests/test_util/test__validate_args/test_fillna.py
-tests/test_util/test__validate_args/test_params/__init__.py
-tests/test_util/test__validate_args/test_params/test_param_01_frequency.py
-tests/test_util/test__validate_args/test_params/test_param_02_datetype.py
-tests/test_util/test__validate_args/test_params/test_param_03_periodtype.py
-tests/test_util/test__validate_args/test_params/test_param_04_adjustment.py
-tests/test_util/test__validate_args/test_params/test_param_05_shownid.py
-tests/test_util/test__validate_args/test_params/test_param_06_rank_method.py
-tests/test_util/test__validate_args/test_params/test_param_07_method.py
-tests/test_util/test__validate_args/test_params/test_param_08_in_startdate_or_enddate.py
-tests/test_util/test__validate_args/test_params/test_param_09_contains_universename.py
-tests/test_util/test__validate_args/test_params/test_param_10_contains_min_periods.py
-tests/test_util/test__validate_args/test_params/test_param_11_base.py
-tests/test_util/test__validate_args/test_params/test_param_12_preliminary.py
-tests/test_util/test__validate_args/test_params/test_param_13_setting.py
-tests/test_util/test__validate_args/test_params/test_param_14_settings.py
+tests/test_util/db_fixtures.py
+tests/test_util/dq_model.py
+tests/test_util/dq_table.py
+tests/test_util/factor_fixtures.py
+tests/test_util/update_factor.py
+tests/test_util/utils.py
```

### Comparing `prismstudio-dev-1.1.7/setup.py` & `prismstudio-dev-1.1.7a0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,16 +25,15 @@
     data_files=datafiles,
     classifiers=[
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
     install_requires=[
-        "pandas==1.4.1",
-        "pytest==7.1.1",
+        "pandas==2.0.3",
         "mypy==0.941",
         "pyarrow==8.0.0",
         "multivolumefile==0.2.3",
         "urllib3==1.26.9",
         "tqdm==4.64.0",
         "orjson==3.7.3",
         "ipywidgets==7.7.1",
```

### Comparing `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_common_functions.py` & `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_common_functions.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_fillna.py` & `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_fillna.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_01_frequency.py` & `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_01_frequency.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_02_datetype.py` & `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_02_datetype.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_03_periodtype.py` & `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_03_periodtype.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_04_adjustment.py` & `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_04_adjustment.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_05_shownid.py` & `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_05_shownid.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_06_rank_method.py` & `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_06_rank_method.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_07_method.py` & `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_07_method.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_08_in_startdate_or_enddate.py` & `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_08_in_startdate_or_enddate.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_09_contains_universename.py` & `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_09_contains_universename.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_10_contains_min_periods.py` & `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_10_contains_min_periods.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_11_base.py` & `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_11_base.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_12_preliminary.py` & `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_12_preliminary.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_13_setting.py` & `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_13_setting.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_14_settings.py` & `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_14_settings.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7/tests/test_util/test_version.py` & `prismstudio-dev-1.1.7a0/tests/test_version.py`

 * *Files identical despite different names*

