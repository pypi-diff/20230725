# Comparing `tmp/commonroad-openscenario-converter-0.0.4.tar.gz` & `tmp/commonroad-openscenario-converter-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commonroad-openscenario-converter-0.0.4.tar", last modified: Thu Jun 29 07:11:18 2023, max compression
+gzip compressed data, was "commonroad-openscenario-converter-0.1.0.tar", last modified: Tue Jul 25 11:27:15 2023, max compression
```

## Comparing `commonroad-openscenario-converter-0.0.4.tar` & `commonroad-openscenario-converter-0.1.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-06-29 07:11:18.879254 commonroad-openscenario-converter-0.0.4/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1570 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/LICENSE
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      575 2023-06-29 07:11:18.879254 commonroad-openscenario-converter-0.0.4/PKG-INFO
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4250 2023-06-29 07:07:14.000000 commonroad-openscenario-converter-0.0.4/README.md
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-06-29 07:11:18.875254 commonroad-openscenario-converter-0.0.4/commonroad_openscenario_converter.egg-info/
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      575 2023-06-29 07:11:18.000000 commonroad-openscenario-converter-0.0.4/commonroad_openscenario_converter.egg-info/PKG-INFO
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)     1794 2023-06-29 07:11:18.000000 commonroad-openscenario-converter-0.0.4/commonroad_openscenario_converter.egg-info/SOURCES.txt
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)        1 2023-06-29 07:11:18.000000 commonroad-openscenario-converter-0.0.4/commonroad_openscenario_converter.egg-info/dependency_links.txt
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      181 2023-06-29 07:11:18.000000 commonroad-openscenario-converter-0.0.4/commonroad_openscenario_converter.egg-info/requires.txt
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)       23 2023-06-29 07:11:18.000000 commonroad-openscenario-converter-0.0.4/commonroad_openscenario_converter.egg-info/top_level.txt
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-06-29 07:11:18.875254 commonroad-openscenario-converter-0.0.4/osc_cr_converter/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/__init__.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-06-29 07:11:18.875254 commonroad-openscenario-converter-0.0.4/osc_cr_converter/analyzer/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/analyzer/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4190 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/analyzer/base.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      756 2023-05-30 08:29:14.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/analyzer/enum_analyzer.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1242 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/analyzer/error.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      482 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/analyzer/result.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-06-29 07:11:18.875254 commonroad-openscenario-converter-0.0.4/osc_cr_converter/batch/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 16:13:42.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/batch/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    18497 2023-05-09 11:24:57.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/batch/analysis.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5792 2023-05-30 08:36:11.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/batch/converter.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-06-29 07:11:18.879254 commonroad-openscenario-converter-0.0.4/osc_cr_converter/converter/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/converter/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1921 2023-05-30 09:16:52.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/converter/base.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    21898 2023-06-15 13:14:23.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/converter/osc2cr.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3075 2023-05-30 08:36:55.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/converter/result.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1872 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/converter/serializable.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-06-29 07:11:18.879254 commonroad-openscenario-converter-0.0.4/osc_cr_converter/udp_driver/
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/udp_driver/__init__.py
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)     4494 2023-05-17 07:35:27.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/udp_driver/common.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-06-29 07:11:18.879254 commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2836 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/abs_rel.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     7617 2023-06-15 13:24:49.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/configuration.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1876 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/general.py
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)     1820 2023-06-29 06:45:10.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/logger.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3952 2023-06-15 13:20:59.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/obstacle_info.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3610 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/pps_builder.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      984 2023-05-09 08:11:46.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/statistics.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3455 2023-05-08 16:13:42.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/visualization.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-06-29 07:11:18.879254 commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/__init__.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-06-29 07:11:18.879254 commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/base/
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/base/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      483 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/base/ending_cause.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5956 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/base/scenario_object.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3570 2023-05-30 10:40:12.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/base/sim_wrapper.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-06-29 07:11:18.879254 commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/esmini/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/esmini/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    10620 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/esmini/esmini_scenario_object.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    13375 2023-06-15 13:01:18.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/esmini/esmini_wrapper.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4868 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/esmini/esmini_wrapper_provider.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      995 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/esmini/storyboard_element.py
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)       38 2023-06-29 07:11:18.879254 commonroad-openscenario-converter-0.0.4/setup.cfg
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1086 2023-06-29 07:09:38.000000 commonroad-openscenario-converter-0.0.4/setup.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-06-29 07:11:18.879254 commonroad-openscenario-converter-0.0.4/tests/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.0.4/tests/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1937 2023-05-09 12:06:26.000000 commonroad-openscenario-converter-0.0.4/tests/test_conversion.py
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      194 2023-05-16 14:12:02.000000 commonroad-openscenario-converter-0.0.4/tests/test_udp.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-07-25 11:27:15.703149 commonroad-openscenario-converter-0.1.0/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1570 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.1.0/LICENSE
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)     5839 2023-07-25 11:27:15.703149 commonroad-openscenario-converter-0.1.0/PKG-INFO
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4880 2023-07-25 11:24:42.000000 commonroad-openscenario-converter-0.1.0/README.md
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-07-25 11:27:15.699149 commonroad-openscenario-converter-0.1.0/commonroad_openscenario_converter.egg-info/
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)     5839 2023-07-25 11:27:15.000000 commonroad-openscenario-converter-0.1.0/commonroad_openscenario_converter.egg-info/PKG-INFO
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)     1794 2023-07-25 11:27:15.000000 commonroad-openscenario-converter-0.1.0/commonroad_openscenario_converter.egg-info/SOURCES.txt
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)        1 2023-07-25 11:27:15.000000 commonroad-openscenario-converter-0.1.0/commonroad_openscenario_converter.egg-info/dependency_links.txt
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      181 2023-07-25 11:27:15.000000 commonroad-openscenario-converter-0.1.0/commonroad_openscenario_converter.egg-info/requires.txt
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)       23 2023-07-25 11:27:15.000000 commonroad-openscenario-converter-0.1.0/commonroad_openscenario_converter.egg-info/top_level.txt
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-07-25 11:27:15.699149 commonroad-openscenario-converter-0.1.0/osc_cr_converter/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/__init__.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-07-25 11:27:15.699149 commonroad-openscenario-converter-0.1.0/osc_cr_converter/analyzer/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/analyzer/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4303 2023-07-25 11:09:57.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/analyzer/base.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      750 2023-07-25 11:09:57.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/analyzer/enum_analyzer.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1248 2023-07-25 11:09:57.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/analyzer/error.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      478 2023-07-25 11:09:57.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/analyzer/result.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-07-25 11:27:15.703149 commonroad-openscenario-converter-0.1.0/osc_cr_converter/batch/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 16:13:42.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/batch/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    18896 2023-07-25 11:09:57.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/batch/analysis.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5790 2023-07-25 11:09:57.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/batch/converter.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-07-25 11:27:15.703149 commonroad-openscenario-converter-0.1.0/osc_cr_converter/converter/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/converter/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1955 2023-07-25 11:09:57.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/converter/base.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    22822 2023-07-25 11:09:57.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/converter/osc2cr.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3187 2023-07-25 11:09:57.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/converter/result.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1868 2023-07-25 11:09:57.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/converter/serializable.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-07-25 11:27:15.703149 commonroad-openscenario-converter-0.1.0/osc_cr_converter/udp_driver/
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/udp_driver/__init__.py
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)     4549 2023-07-25 11:09:57.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/udp_driver/common.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-07-25 11:27:15.703149 commonroad-openscenario-converter-0.1.0/osc_cr_converter/utility/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/utility/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2906 2023-07-25 11:09:57.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/utility/abs_rel.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     7774 2023-07-25 11:09:57.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/utility/configuration.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1976 2023-07-25 11:09:57.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/utility/general.py
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)     1790 2023-07-25 11:09:57.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/utility/logger.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4493 2023-07-25 11:01:53.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/utility/obstacle_info.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3529 2023-07-25 11:01:53.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/utility/pps_builder.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      979 2023-07-25 11:09:57.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/utility/statistics.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3559 2023-07-25 11:09:57.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/utility/visualization.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-07-25 11:27:15.703149 commonroad-openscenario-converter-0.1.0/osc_cr_converter/wrapper/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/wrapper/__init__.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-07-25 11:27:15.703149 commonroad-openscenario-converter-0.1.0/osc_cr_converter/wrapper/base/
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/wrapper/base/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      479 2023-07-25 11:09:57.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/wrapper/base/ending_cause.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     6303 2023-07-25 11:09:57.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/wrapper/base/scenario_object.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3611 2023-07-25 11:09:57.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/wrapper/base/sim_wrapper.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-07-25 11:27:15.703149 commonroad-openscenario-converter-0.1.0/osc_cr_converter/wrapper/esmini/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/wrapper/esmini/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    10661 2023-07-25 11:09:57.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/wrapper/esmini/esmini_scenario_object.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    14360 2023-07-25 11:09:57.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/wrapper/esmini/esmini_wrapper.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5317 2023-07-25 11:09:57.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/wrapper/esmini/esmini_wrapper_provider.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1041 2023-07-25 11:09:57.000000 commonroad-openscenario-converter-0.1.0/osc_cr_converter/wrapper/esmini/storyboard_element.py
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)       38 2023-07-25 11:27:15.703149 commonroad-openscenario-converter-0.1.0/setup.cfg
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1671 2023-07-25 11:20:58.000000 commonroad-openscenario-converter-0.1.0/setup.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-07-25 11:27:15.703149 commonroad-openscenario-converter-0.1.0/tests/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:25:03.000000 commonroad-openscenario-converter-0.1.0/tests/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1960 2023-07-25 11:01:54.000000 commonroad-openscenario-converter-0.1.0/tests/test_conversion.py
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      192 2023-07-25 11:01:54.000000 commonroad-openscenario-converter-0.1.0/tests/test_udp.py
```

### Comparing `commonroad-openscenario-converter-0.0.4/LICENSE` & `commonroad-openscenario-converter-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.4/README.md` & `commonroad-openscenario-converter-0.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # CommonROAD-OpenSCENARIO Converter
-![image info](./docs/figures/converter-banner.png)
+![image info](https://gitlab.lrz.de/tum-cps/commonroad-openscenario-converter/-/raw/master/docs/figures/converter-banner.png)
 
 Automatic Traffic Scenario Conversion between [OpenSCENARIO](https://www.asam.net/standards/detail/openscenario/)
 and [CommonRoad](commonroad.in.tum.de/). Currently, only the conversion from **O**pen**SC**ENARIO to **C**ommon**R**OAD (osc2cr) is developed.<br>
-[![Linux](https://svgshare.com/i/Zhy.svg?style=plastic)](https://svgshare.com/i/Zhy.svg)
+[![Linux](https://img.shields.io/badge/os-linux?&logo=Linux&logoColor=white&labelColor=gray)](https://pypi.python.org/pypi/commonroad-openscenario-converter/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/commonroad-openscenario-converter.svg)](https://pypi.python.org/pypi/commonroad-openscenario-converter/)
 [![PyPI license](https://img.shields.io/pypi/l/commonroad-openscenario-converter.svg)](https://pypi.python.org/pypi/commonroad-openscenario-converter/)
 [![PyPI version fury.io](https://badge.fury.io/py/commonroad-openscenario-converter.svg)](https://pypi.python.org/pypi/commonroad-openscenario-converter/)<br>
 [![PyPI download month](https://img.shields.io/pypi/dm/commonroad-openscenario-converter.svg?style=plastic&label=PyPI%20downloads)](https://pypi.python.org/pypi/commonroad-openscenario-converter/) 
 [![PyPI download week](https://img.shields.io/pypi/dw/commonroad-openscenario-converter.svg?style=plastic&label=PyPI%20downloads)](https://pypi.python.org/pypi/commonroad-openscenario-converter/)<br>
 
 ### Using the Converter
@@ -48,32 +48,44 @@
 external driver models or vehicle simulators, you need to install OSI manually, 
 see [here](https://github.com/OpenSimulationInterface/open-simulation-interface).
 
 ### Contributors (in alphabetical order by last name)
 - Yuanfei Lin
 - Michael Ratzel
 
+### Documentation
+
+The documentation of our toolbox is available on our website: https://cps.pages.gitlab.lrz.de/commonroad-openscenario-converter/.
+
+In order to generate the documentation via Sphinx locally, run the following commands in the root directory:
+
+```bash
+$ pip install -r ./docs/requirements_doc.txt
+$ cd docs/sphinx
+$ make html
+```
+The documentation can then be launched by browsing ``./docs/sphinx/build/html/index.html/``.
 ### Acknowledgments
 We would like to extend our heartfelt gratitude to the team behind [esmini](https://github.com/esmini/esmini) for 
 their remarkable effort in developing the simulation tool. Specifically, we would like to express our sincere 
 appreciation to [Emil Knabe](https://www.linkedin.com/in/emil-knabe-216a1a11/?originalSubdomain=se)
 for his invaluable contribution in reviewing and accepting the proposed changes to the esmini interface, 
 and to [Sebastian Maierhofer](https://www.ce.cit.tum.de/air/people/sebastian-maierhofer-msc/)
 for maintaining the converter from OpenDRIVE to lanelets.
 We gratefully acknowledge partial financial support by the German Federal Ministry for Digital and Transport (BMDV) 
 within the project _Cooperative Autonomous Driving with Safety Guarantees_
 ([KoSi](https://www.ce.cit.tum.de/air/research/kosi/)).
 
 ### Citation
-If you use `commonroad-openscenario-converter` for academic work, we highly encourage you to cite our [paper](https://arxiv.org/pdf/2305.10080.pdf):
+If you use `commonroad-openscenario-converter` for academic work, we highly encourage you to cite our [paper](https://mediatum.ub.tum.de/doc/1716501/1716501.pdf):
 ```text
-@article{osc2cr,
-  title={Automatic Traffic Scenario Conversion from OpenSCENARIO to CommonRoad},
-  author={Yuanfei Lin, Michael Ratzel, and Matthias Althoff},
-  archivePrefix={arXiv},
-  journal={arXiv preprint arXiv:2305.10080},
-  year={2023}}
+@inproceedings{Lin2023Osc2Cr,
+	author = {Yuanfei Lin, Michael Ratzel, and Matthias Althoff},
+	title = {Automatic Traffic Scenario Conversion from {OpenSCENARIO} to {CommonRoad}},
+	booktitle = {Proc. of the IEEE Int. Conf. on Intell. Transp. Syst.},
+	year = {2023},
+	pages= {},
 }
 ```
 If you use this project's code in industry, we'd love to hear from you as well; 
 feel free to reach out to [Yuanfei Lin](mailto:yuanfei.lin@tum.de) directly.
```

### Comparing `commonroad-openscenario-converter-0.0.4/commonroad_openscenario_converter.egg-info/SOURCES.txt` & `commonroad-openscenario-converter-0.1.0/commonroad_openscenario_converter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `commonroad-openscenario-converter-0.0.4/osc_cr_converter/analyzer/base.py` & `commonroad-openscenario-converter-0.1.0/osc_cr_converter/analyzer/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __author__ = "Michael Ratzel, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.0.1"
+__version__ = "0.1.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
-__status__ = "Pre-alpha"
+__status__ = "beta"
 
 import time
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from multiprocessing import Manager, Process
 from typing import Optional, Dict, Tuple
 
@@ -26,18 +26,23 @@
 class Analyzer(ABC):
     """
     The base interface for all post conversion analyzer.
 
     To implement your own analyzer, implement the _run method and make sure it is safe that the analyzer will be killed
     after the timeout happened
     """
+
     timeout: float = 120
 
-    def run(self, scenario: Scenario, obstacles: Dict[str, Optional[DynamicObstacle]],
-            obstacles_extra_info: Dict[str, Optional[Vehicle]]) -> Tuple[float, Dict[str, AnalyzerResult]]:
+    def run(
+        self,
+        scenario: Scenario,
+        obstacles: Dict[str, Optional[DynamicObstacle]],
+        obstacles_extra_info: Dict[str, Optional[Vehicle]],
+    ) -> Tuple[float, Dict[str, AnalyzerResult]]:
         """
         The run method is the main entry point for your analyzer. It is called by the
         scenario runner and expects to receive three arguments:
 
             * A Scenario object, which contains all information about the scenario that was converted.
             * A dictionary of DynamicObstacle objects, keyed by obstacle name, which represents all dynamic obstacles in
               this scenario
@@ -53,41 +58,53 @@
         :return: A tuple containing the dictionary of analyzer results per obstacle name and the calculation time
         """
         assert dataclass_is_complete(self)
 
         time_start = time.time()
 
         result_dict = Manager().dict()
-        process = Process(target=self.__run, args=(scenario, obstacles, obstacles_extra_info, result_dict), daemon=True)
+        process = Process(
+            target=self.__run,
+            args=(scenario, obstacles, obstacles_extra_info, result_dict),
+            daemon=True,
+        )
         process.start()
         process.join(self.timeout)
         exec_time = time.time() - time_start
         if process.exitcode is None:
             process.terminate()
             process.join(self.timeout / 2)
             exception_text = "Timed out"
             if process.exitcode is None:
                 process.kill()
                 exception_text = "Timed out - NEEDED SIGKILL"
             result = AnalyzerErrorResult(
-                exception_text=exception_text,
-                traceback_text=""
+                exception_text=exception_text, traceback_text=""
             )
             results = {o_name: result for o_name in obstacles.keys()}
         else:
             results = dict(result_dict)
         return exec_time, results
 
-    def __run(self, scenario: Scenario, obstacles: Dict[str, Optional[DynamicObstacle]],
-              obstacles_extra_info: Dict[str, Optional[Vehicle]], result_dict: Dict[str, AnalyzerResult]):
+    def __run(
+        self,
+        scenario: Scenario,
+        obstacles: Dict[str, Optional[DynamicObstacle]],
+        obstacles_extra_info: Dict[str, Optional[Vehicle]],
+        result_dict: Dict[str, AnalyzerResult],
+    ):
         result_dict.update(self._run(scenario, obstacles, obstacles_extra_info))
 
     @abstractmethod
-    def _run(self, scenario: Scenario, obstacles: Dict[str, Optional[DynamicObstacle]],
-             obstacles_extra_info: Dict[str, Optional[Vehicle]]) -> Dict[str, AnalyzerResult]:
+    def _run(
+        self,
+        scenario: Scenario,
+        obstacles: Dict[str, Optional[DynamicObstacle]],
+        obstacles_extra_info: Dict[str, Optional[Vehicle]],
+    ) -> Dict[str, AnalyzerResult]:
         """
         The _run method is the method where the actual work of the analyzer happens
 
         :param scenario:Scenario: Get the current scenario
         :param obstacles:Dict[str, Optional[DynamicObstacle]]: Obstacles per name
         :param obstacles_extra_info:Dict[str, Optional[Vehicle]]: Extra obstacle info per name
         :return: A dictionary of analyzer results per obstacle name
```

### Comparing `commonroad-openscenario-converter-0.0.4/osc_cr_converter/analyzer/enum_analyzer.py` & `commonroad-openscenario-converter-0.1.0/osc_cr_converter/analyzer/enum_analyzer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __author__ = "Michael Ratzel, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.0.4"
+__version__ = "0.1.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
-__status__ = "Pre-alpha"
+__status__ = "beta"
 
 from enum import Enum
 from typing import Type
 
 from osc_cr_converter.analyzer.base import Analyzer
 from osc_cr_converter.analyzer.result import AnalyzerResult
 
@@ -19,8 +19,7 @@
 
     def __new__(cls, analyzer_type: Type[Analyzer], result_type: Type[AnalyzerResult]):
         obj = object.__new__(cls)
         obj._value_ = len(cls.__members__)
         obj.analyzer_type = analyzer_type
         obj.result_type = result_type
         return obj
-
```

### Comparing `commonroad-openscenario-converter-0.0.4/osc_cr_converter/analyzer/error.py` & `commonroad-openscenario-converter-0.1.0/osc_cr_converter/analyzer/error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 __author__ = "Michael Ratzel, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.0.1"
+__version__ = "0.1.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
-__status__ = "Pre-alpha"
+__status__ = "beta"
 
 import traceback
 from dataclasses import dataclass, fields
 from typing import Dict
 
 from osc_cr_converter.analyzer.result import AnalyzerResult
 
 
 @dataclass(frozen=True)
 class AnalyzerErrorResult(AnalyzerResult):
     """
     A result containing a exception text and traceback
     """
+
     exception_text: str
     traceback_text: str
 
     def __getstate__(self) -> Dict:
         return self.__dict__.copy()
 
     def __setstate__(self, data: Dict):
@@ -29,15 +30,16 @@
 
     def __str__(self):
         return f"{self.exception_text}\n{self.traceback_text}"
 
     @staticmethod
     def is_error(data: Dict) -> bool:
         expected_fields = fields(AnalyzerErrorResult)
-        return len(data) == len(expected_fields) and all([field.name in data for field in expected_fields])
+        return len(data) == len(expected_fields) and all(
+            [field.name in data for field in expected_fields]
+        )
 
     @staticmethod
     def from_exception(e: Exception) -> "AnalyzerErrorResult":
         return AnalyzerErrorResult(
-            exception_text=str(e),
-            traceback_text=traceback.format_exc(limit=50)
+            exception_text=str(e), traceback_text=traceback.format_exc(limit=50)
         )
```

### Comparing `commonroad-openscenario-converter-0.0.4/osc_cr_converter/batch/analysis.py` & `commonroad-openscenario-converter-0.1.0/osc_cr_converter/batch/analysis.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __author__ = "Michael Ratzel, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.0.1"
+__version__ = "0.1.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
-__status__ = "Pre-alpha"
+__status__ = "beta"
 
 from enum import Enum
 from typing import Union, Dict, List, Optional, Type
 
 import numpy as np
 from commonroad.visualization.mp_renderer import MPRenderer
 from matplotlib import pyplot as plt
@@ -64,18 +64,18 @@
     def count(name: str, amount: int = 1):
         if name in counts:
             counts[name] += amount
         else:
             counts[name] = amount
 
     def perc(
-            description: str,
-            part_str: Union[str, List[str]],
-            total_str: Union[str, List[str]],
-            invert: bool = False
+        description: str,
+        part_str: Union[str, List[str]],
+        total_str: Union[str, List[str]],
+        invert: bool = False,
     ):
         if isinstance(part_str, str):
             part = counts.get(part_str, 0)
         else:
             part = sum([counts.get(single_part, 0) for single_part in part_str])
         if isinstance(total_str, str):
             total = counts.get(total_str, 0)
@@ -119,15 +119,18 @@
 
                 for t_analyzer, analysis in result.analysis.items():
                     exec_time, analysis = analysis
                     if t_analyzer not in analyzer_times:
                         analyzer_times[t_analyzer] = []
                     analyzer_times[t_analyzer].append(exec_time)
                     count(f"{t_analyzer.__name__} scenario total")
-                    count(f"{t_analyzer.__name__} vehicle total", stats.num_obstacle_conversions)
+                    count(
+                        f"{t_analyzer.__name__} vehicle total",
+                        stats.num_obstacle_conversions,
+                    )
                     scenario_run = True
                     scenario_success = True
                     for vehicle_name, analyzer_result in analysis.items():
                         vehicle_run = True
                         vehicle_success = True
                         if isinstance(analyzer_result, AnalyzerErrorResult):
                             scenario_run = False
@@ -154,49 +157,77 @@
     print("-" * 80)
     perc("OpenDRIVE Conversion run rate", "odr conversions run", "success")
     perc("OpenDRIVE Conversion success rate", "odr conversions success", "success")
     perc("", "odr conversions success", "odr conversions run")
     print("-" * 80)
     print("Sim Ending causes:")
     for e_ending_cause in ESimEndingCause:
-        perc(f" | {e_ending_cause.name}", f"sim ending cause {e_ending_cause.name}", "success")
+        perc(
+            f" | {e_ending_cause.name}",
+            f"sim ending cause {e_ending_cause.name}",
+            "success",
+        )
     print("\n" + "#" * 80)
     print("Granularity SCENARIO")
     print("-" * 80)
     perc("Conversion success rate", "success", "total")
     perc("Conversion failure rate", "failed", "total")
     for reason in EFailureReason:
         perc(f" | {reason.name}", f"failed {reason.name}", "failed")
     perc("Conversion exception rate", "exception", "total")
     print("-" * 80)
     for path, reason in failed_scenarios.items():
-        print(reason, ':', path)
+        print(reason, ":", path)
     for t_analyzer in analyzer_times.keys():
         print("-" * 80)
         print(f"{t_analyzer.__name__}")
         print(f"{'Average time':<50s} {np.mean(analyzer_times[t_analyzer]):}")
-        perc("run rate", f"{t_analyzer.__name__} scenario run", f"{t_analyzer.__name__} scenario total")
-        perc("success rate", f"{t_analyzer.__name__} scenario success", f"{t_analyzer.__name__} scenario total")
-        perc("", f"{t_analyzer.__name__} scenario success", f"{t_analyzer.__name__} scenario run")
+        perc(
+            "run rate",
+            f"{t_analyzer.__name__} scenario run",
+            f"{t_analyzer.__name__} scenario total",
+        )
+        perc(
+            "success rate",
+            f"{t_analyzer.__name__} scenario success",
+            f"{t_analyzer.__name__} scenario total",
+        )
+        perc(
+            "",
+            f"{t_analyzer.__name__} scenario success",
+            f"{t_analyzer.__name__} scenario run",
+        )
     print("\n" + "#" * 80)
     print("Granularity VEHICLE")
     print("-" * 80)
     perc("Conversion success rate", "vehicle failed", "vehicle total", invert=True)
     print("-" * 80)
     for t_analyzer in analyzer_times.keys():
         print("-" * 80)
         print(f"{t_analyzer.__name__}")
-        perc("run rate", f"{t_analyzer.__name__} vehicle run", f"{t_analyzer.__name__} vehicle total")
-        perc("success rate", f"{t_analyzer.__name__} vehicle success", f"{t_analyzer.__name__} vehicle total")
-        perc("", f"{t_analyzer.__name__} vehicle success", f"{t_analyzer.__name__} vehicle run")
+        perc(
+            "run rate",
+            f"{t_analyzer.__name__} vehicle run",
+            f"{t_analyzer.__name__} vehicle total",
+        )
+        perc(
+            "success rate",
+            f"{t_analyzer.__name__} vehicle success",
+            f"{t_analyzer.__name__} vehicle total",
+        )
+        perc(
+            "",
+            f"{t_analyzer.__name__} vehicle success",
+            f"{t_analyzer.__name__} vehicle run",
+        )
 
 
 def print_exception_tracebacks(
-        results: Dict[str, BatchConversionResult],
-        compressed=True,
+    results: Dict[str, BatchConversionResult],
+    compressed=True,
 ):
     """
     Print the exception tracebacks, that raised inside the Converter and caught by the BatchConverter.
 
     :param results: The result dict returned by the BatchConverter
     :param compressed:bool: If true print only unique errors and a count how often they were raised.
     """
@@ -210,31 +241,34 @@
 
     for error, count in errors.items():
         print(f"{count}\n{error.traceback_text}")
         print("\n" * 3)
 
 
 def print_exception_tracebacks_for_analyzer(
-        results: Dict[str, BatchConversionResult], analyzer: Type[Analyzer],
-        granularity: EGranularity = EGranularity.SCENARIO,
-        compressed=True,
+    results: Dict[str, BatchConversionResult],
+    analyzer: Type[Analyzer],
+    granularity: EGranularity = EGranularity.SCENARIO,
+    compressed=True,
 ):
     """
     Print the exception tracebacks, that were raised inside an Analyzer implementation.
 
     :param results: The result dict returned by the BatchConverter
     :param analyzer:EAnalyzer: Specify of which analyzer the tracebacks shall be printed
     :param granularity: Specify the granularity this shall work on
     :param compressed:bool: If true print only unique errors and a count how often they were raised.
     """
     errors: Dict[AnalyzerErrorResult, int] = {}
 
     def handle_error(source_file, found_error: AnalyzerErrorResult):
         if not compressed:
-            print(f"{source_file}: {found_error.exception_text}\n{found_error.traceback_text}")
+            print(
+                f"{source_file}: {found_error.exception_text}\n{found_error.traceback_text}"
+            )
         else:
             errors[found_error] = 1 + errors.get(found_error, 0)
 
     for scenario_path, result in results.items():
         if not result.without_exception:
             continue
         result = result.get_result()
@@ -251,15 +285,22 @@
                 if granularity == EGranularity.SCENARIO and error is not None:
                     handle_error(result.xosc_file, error)
 
     for error, count in errors.items():
         print(f"{count}\n{error.exception_text}\n{error.traceback_text}")
         print("\n" * 3)
 
-def _plot_times(times, n_bins: int, low_pass_filter: Optional[float], path: Optional[str], label=None):
+
+def _plot_times(
+    times,
+    n_bins: int,
+    low_pass_filter: Optional[float],
+    path: Optional[str],
+    label=None,
+):
     if low_pass_filter is None:
         fig = plt.figure(figsize=(5, 2.5), tight_layout=True)
         plt.hist(times, bins=n_bins, color=_get_colors(times))
         if label is not None:
             plt.legend(label)
         plt.xlabel("t [s]")
         plt.ylabel("# scenarios")
@@ -290,19 +331,21 @@
         fig.show()
 
     if path is not None:
         fig.savefig(path)
 
 
 def plot_sim_times(
-        results: Union[Dict[str, BatchConversionResult], List[Dict[str, BatchConversionResult]]],
-        n_bins: int = 25,
-        low_pass_filter: Optional[float] = None,
-        path: Optional[str] = None,
-        label: Optional[List[str]] = None
+    results: Union[
+        Dict[str, BatchConversionResult], List[Dict[str, BatchConversionResult]]
+    ],
+    n_bins: int = 25,
+    low_pass_filter: Optional[float] = None,
+    path: Optional[str] = None,
+    label: Optional[List[str]] = None,
 ):
     """
     Plot the simulation times in a histogram, it can also combine multiple results in one dict, if those are passed as a
     list in the results parameter, resulting in a more colorful dict. See the label param if you want to do this
 
     :param results: The result dict returned by the BatchConverter or a list of such dicts
     :param n_bins:int: The number of bins used for the histogram
@@ -327,20 +370,23 @@
                 continue
             result = result.get_result()
             if isinstance(result, Osc2CrConverterResult):
                 times.append(result.statistics.sim_time)
 
     _plot_times(times, n_bins, low_pass_filter, path, label)
 
+
 def plot_runtimes(
-        results: Union[Dict[str, BatchConversionResult], List[Dict[str, BatchConversionResult]]],
-        n_bins: int = 25,
-        low_pass_filter: Optional[float] = None,
-        path: Optional[str] = None,
-        label: Optional[List[str]] = None
+    results: Union[
+        Dict[str, BatchConversionResult], List[Dict[str, BatchConversionResult]]
+    ],
+    n_bins: int = 25,
+    low_pass_filter: Optional[float] = None,
+    path: Optional[str] = None,
+    label: Optional[List[str]] = None,
 ):
     """
     Plot the simulation times in a histogram, it can also combine multiple results in one dict, if those are passed as a
     list in the results parameter, resulting in a more colorful dict. See the label param if you want to do this
 
     :param results: The result dict returned by the BatchConverter or a list of such dicts
     :param n_bins:int: The number of bins used for the histogram
@@ -365,18 +411,19 @@
                 continue
             result = result.get_result()
             if isinstance(result, Osc2CrConverterResult):
                 times.append(result.statistics.runtime)
 
     _plot_times(times, n_bins, low_pass_filter, path, label)
 
+
 def plot_num_obstacles(
-        results: Dict[str, BatchConversionResult],
-        low_pass_filter: Optional[int] = None,
-        path: Optional[str] = None
+    results: Dict[str, BatchConversionResult],
+    low_pass_filter: Optional[int] = None,
+    path: Optional[str] = None,
 ):
     """
     Plot how many scenarios have a num of obstacles in them
 
     :param results: The result dict returned by the BatchConverter
     :param low_pass_filter:float: If present a second plot with only obstacles counts times leq than this will be added
     :param path:float: If present the plot will be stored here
```

### Comparing `commonroad-openscenario-converter-0.0.4/osc_cr_converter/batch/converter.py` & `commonroad-openscenario-converter-0.1.0/osc_cr_converter/batch/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __author__ = "Michael Ratzel, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.0.4"
+__version__ = "0.1.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
-__status__ = "Pre-alpha"
+__status__ = "beta"
 
 import os
 import pickle
 import re
 from concurrent.futures import ProcessPoolExecutor, Future
 from dataclasses import dataclass
 from typing import Optional, Dict, List
@@ -22,42 +22,44 @@
 
 @dataclass(frozen=True)
 class BatchConversionResult(Serializable):
     """
     Contains either an AnalyzerErrorResult, or the path to an file, where the pickled result of the converter run is
     stored
     """
+
     exception: Optional[AnalyzerErrorResult]
     result_file: Optional[str]
 
     def __post_init__(self):
         """
         Enforcing that exactly one of the two parameters is set
         """
-        assert self.exception is not None or self.result_file is not None and \
-               (self.exception is None or self.result_file is None)
+        assert (
+            self.exception is not None
+            or self.result_file is not None
+            and (self.exception is None or self.result_file is None)
+        )
 
     def __getstate__(self) -> Dict:
         return self.__dict__.copy()
 
     def __setstate__(self, data: Dict):
         self.__dict__.update(data)
 
     @staticmethod
     def from_result_file(result_file: str) -> "BatchConversionResult":
         return BatchConversionResult(
-            exception=None,
-            result_file=os.path.abspath(result_file)
+            exception=None, result_file=os.path.abspath(result_file)
         )
 
     @staticmethod
     def from_exception(e: Exception) -> "BatchConversionResult":
         return BatchConversionResult(
-            exception=AnalyzerErrorResult.from_exception(e),
-            result_file=None
+            exception=AnalyzerErrorResult.from_exception(e), result_file=None
         )
 
     def get_result(self) -> Serializable:
         """
         Load the result of the conversion run from disk
         Use this to actually access the data, but it might take a bit of time depending on the conversion run
         """
@@ -98,19 +100,19 @@
         return self._converter
 
     @converter.setter
     def converter(self, new_converter: Converter):
         self._converter = new_converter
 
     def discover_files(
-            self,
-            directory: str,
-            file_matcher: re.Pattern,
-            reset_file_list: bool = True,
-            recursively: bool = True
+        self,
+        directory: str,
+        file_matcher: re.Pattern,
+        reset_file_list: bool = True,
+        recursively: bool = True,
     ):
         """
         Utility method to search a repository and discover files, that can be run in the batch conversion.
 
         The results will be added to the file_list attribute of the object
 
         :param directory:str: The directory where to start the search
@@ -124,15 +126,17 @@
         for dir_path, dirs, files in os.walk(directory):
             if not recursively and os.path.abspath(dir_path) != abs_directory:
                 continue
             for file in files:
                 if file_matcher.match(file) is not None:
                     self.file_list.append(os.path.join(dir_path, file))
 
-    def run_batch_conversion(self, num_worker: Optional[int] = None, timeout: Optional[int] = None):
+    def run_batch_conversion(
+        self, num_worker: Optional[int] = None, timeout: Optional[int] = None
+    ):
         """
         Run the batch conversion
 
         :param num_worker:int: If None or leq than 0, it will default to all available processors
         :timeout:int: If present a single conversion run will time out if this amount of seconds passed
         """
         assert Serializable.storage_dir is not None
```

### Comparing `commonroad-openscenario-converter-0.0.4/osc_cr_converter/converter/base.py` & `commonroad-openscenario-converter-0.1.0/osc_cr_converter/converter/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,57 @@
 __author__ = "Michael Ratzel, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.0.4"
+__version__ = "0.1.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
-__status__ = "Pre-alpha"
+__status__ = "beta"
 
 import pickle
 from abc import ABC, abstractmethod
 from enum import Enum, auto
 from multiprocessing import Lock
 from os import path
-from typing import Union, ClassVar, Optional
+from typing import Union, ClassVar
 
 from commonroad.scenario.scenario import Scenario
 
 from osc_cr_converter.converter.serializable import Serializable
 from osc_cr_converter.converter.result import Osc2CrConverterResult
 
 
 class EFailureReason(Enum):
     """
     The enum of reasons why the conversion failed
     """
+
     SCENARIO_FILE_INVALID_PATH = auto()
     SCENARIO_FILE_IS_CATALOG = auto()
     SCENARIO_FILE_IS_PARAMETER_VALUE_DISTRIBUTION = auto()
     SCENARIO_FILE_CONTAINS_NO_STORYBOARD = auto()
     SIMULATION_FAILED_CREATING_OUTPUT = auto()
     NO_DYNAMIC_BEHAVIOR_FOUND = auto()
 
 
 class Converter(ABC):
     """
     The Base class for a converter
 
     It only needs to implement the run_conversion function
     """
+
     __lock: ClassVar[Lock] = Lock()
     conversion_result: Union[Osc2CrConverterResult, EFailureReason] = None
 
     def run_in_batch_conversion(self, source_file: str) -> str:
         with self.__lock:
-            file_path_base = path.join(Serializable.storage_dir, "Res_" + path.splitext(path.basename(source_file))[0])
+            file_path_base = path.join(
+                Serializable.storage_dir,
+                "Res_" + path.splitext(path.basename(source_file))[0],
+            )
             i = 1
             while path.exists(result_file := file_path_base + f"{i}.pickle"):
                 i += 1
         self.run_conversion(source_file)
         with open(result_file, "wb") as file:
             pickle.dump(self.conversion_result, file)
         return result_file
```

### Comparing `commonroad-openscenario-converter-0.0.4/osc_cr_converter/converter/osc2cr.py` & `commonroad-openscenario-converter-0.1.0/osc_cr_converter/converter/osc2cr.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __author__ = "Michael Ratzel, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.0.4"
+__version__ = "0.1.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
-__status__ = "Pre-alpha"
+__status__ = "beta"
 
 import math
 import os
 import re
 import time
 import warnings
 import logging
@@ -30,16 +30,21 @@
 
 from osc_cr_converter.converter.base import Converter, EFailureReason
 from osc_cr_converter.analyzer.base import Analyzer
 from osc_cr_converter.analyzer.error import AnalyzerErrorResult
 from osc_cr_converter.analyzer.result import AnalyzerResult
 from osc_cr_converter.analyzer.enum_analyzer import EAnalyzer
 from osc_cr_converter.wrapper.base.ending_cause import ESimEndingCause
-from osc_cr_converter.wrapper.esmini.esmini_wrapper_provider import EsminiWrapperProvider
-from osc_cr_converter.wrapper.base.scenario_object import ScenarioObjectState, SimScenarioObjectState
+from osc_cr_converter.wrapper.esmini.esmini_wrapper_provider import (
+    EsminiWrapperProvider,
+)
+from osc_cr_converter.wrapper.base.scenario_object import (
+    ScenarioObjectState,
+    SimScenarioObjectState,
+)
 from osc_cr_converter.wrapper.base.sim_wrapper import SimWrapper, WrapperSimResult
 from osc_cr_converter.converter.result import Osc2CrConverterResult
 from osc_cr_converter.utility.statistics import ConversionStatistics
 from osc_cr_converter.utility.obstacle_info import ObstacleExtraInfoFinder
 from osc_cr_converter.utility.pps_builder import PPSBuilder
 from osc_cr_converter.utility.general import trim_scenario, dataclass_is_complete
 from osc_cr_converter.utility.configuration import ConverterParams
@@ -50,27 +55,33 @@
 
 
 @dataclass
 class Osc2CrConverter(Converter):
     """
     The main class of the OpenSCENARIO to CommonRoad conversion
     """
-    def __init__(self, config: ConverterParams):
-
-        self.author: str = config.scenario.author              # Author of the scenario
-        self.affiliation: str = config.scenario.affiliation    # Affiliation of the author of the scenario
-        self.source: str = config.scenario.source              # Source of the scenario
-        self.tags: Set[Tag] = config.scenario.tags             # Tags of the scenario
 
-        self.dt_cr: float = config.scenario.dt_cr              # Time step size of the CommonRoad scenario
+    def __init__(self, config: ConverterParams):
+        self.author: str = config.scenario.author  # Author of the scenario
+        self.affiliation: str = (
+            config.scenario.affiliation
+        )  # Affiliation of the author of the scenario
+        self.source: str = config.scenario.source  # Source of the scenario
+        self.tags: Set[Tag] = config.scenario.tags  # Tags of the scenario
+
+        self.dt_cr: float = (
+            config.scenario.dt_cr
+        )  # Time step size of the CommonRoad scenario
 
-        self.config: ConverterParams = config                  # Configurations
+        self.config: ConverterParams = config  # Configurations
 
         # The used SimWrapper implementation
-        self.sim_wrapper: SimWrapper = EsminiWrapperProvider(config).provide_esmini_wrapper()
+        self.sim_wrapper: SimWrapper = EsminiWrapperProvider(
+            config
+        ).provide_esmini_wrapper()
         # The used PPSBuilder instance
         self.pps_builder: PPSBuilder = config.initialize_planning_problem_set()
 
         # indicating whether the openDRIVE map defined in the openSCENARIO is used
         self.use_implicit_odr_file: bool = config.esmini.use_implicit_odr_file
         # indicating whether the huge mag contained in the scenario is trimmed
         self.trim_scenario: bool = config.scenario.trim_scenario
@@ -79,134 +90,172 @@
         # indicating whether the scenario needs to be visualized with esmini
         self.view_scenario: bool = config.debug.run_viewer
         self.render_to_gif: bool = config.debug.render_to_gif
 
         # analyzers of the scenario with CommonRoad tools
         self.analyzers: Union[Dict[EAnalyzer, Optional[Analyzer]], List[EAnalyzer]] = {}
 
-        self.dt_sim: Optional[float] = config.esmini.dt_sim  # User-defined time step size for esmini simulation
-        self.odr_file_override: Optional[str] = config.esmini.odr_file_override  # User-defined OpenDRIVE map to be used
-        self.ego_filter: Optional[re.Pattern, str] = config.esmini.ego_filter  # Pattern of recognizing the ego vehicle
+        self.dt_sim: Optional[
+            float
+        ] = config.esmini.dt_sim  # User-defined time step size for esmini simulation
+        self.odr_file_override: Optional[
+            str
+        ] = config.esmini.odr_file_override  # User-defined OpenDRIVE map to be used
+        self.ego_filter: Optional[
+            re.Pattern, str
+        ] = config.esmini.ego_filter  # Pattern of recognizing the ego vehicle
 
     def get_analyzer_objects(self) -> Dict[EAnalyzer, Analyzer]:
         if self.analyzers is None:
             return {}
         elif isinstance(self.analyzers, list):
-            return {e_analyzer: e_analyzer.analyzer_type() for e_analyzer in self.analyzers}
+            return {
+                e_analyzer: e_analyzer.analyzer_type() for e_analyzer in self.analyzers
+            }
         elif isinstance(self.analyzers, dict):
             ret = {}
             for e_analyzer, analyzer in self.analyzers.items():
                 if analyzer is not None:
                     ret[e_analyzer] = analyzer
                 else:
                     ret[e_analyzer] = e_analyzer.analyzer_type()
             return ret
 
-    def run_conversion(self, source_file: str) \
-            -> Union[Scenario, EFailureReason]:
+    def run_conversion(self, source_file: str) -> Union[Scenario, EFailureReason]:
         """
         The main function, that runs the simulation wrapper (SimWrapper) and converts its results.
         :param source_file: the given openSCENARIO source file
         :return converted results if converted successfully. Otherwise, the reason for the failure.
         """
-        self.config.general.name_xosc = os.path.basename(source_file).split('.')[0]
-        util_logger.print_and_log_info(logger,
-                                       f"* Converting the OpenSCENARIO file: {self.config.general.name_xosc}.xosc")
+        self.config.general.name_xosc = os.path.basename(source_file).split(".")[0]
+        util_logger.print_and_log_info(
+            logger,
+            f"* Converting the OpenSCENARIO file: {self.config.general.name_xosc}.xosc",
+        )
 
         assert dataclass_is_complete(self)
 
         xosc_file = path.abspath(source_file)
 
         implicit_opendrive_path = self._pre_parse_scenario(xosc_file)
 
         if isinstance(implicit_opendrive_path, EFailureReason):
             self.conversion_result = implicit_opendrive_path
-            util_logger.print_and_log_error(logger, f"*\t Failed since : {self.conversion_result.name}")
+            util_logger.print_and_log_error(
+                logger, f"*\t Failed since : {self.conversion_result.name}"
+            )
             return self.conversion_result
 
         start_time = time.time()
-        scenario, xodr_file, xodr_conversion_error = self._create_basic_scenario(implicit_opendrive_path)
+        scenario, xodr_file, xodr_conversion_error = self._create_basic_scenario(
+            implicit_opendrive_path
+        )
         runtime = time.time() - start_time
-        util_logger.print_and_log_info(logger, f"*\t Map conversion takes {runtime:.2f} s")
+        util_logger.print_and_log_info(
+            logger, f"*\t Map conversion takes {runtime:.2f} s"
+        )
 
         if isinstance(scenario, EFailureReason):
             self.conversion_result = scenario
-            util_logger.print_and_log_error(logger, f"*\t Failed since : {self.conversion_result.name}")
+            util_logger.print_and_log_error(
+                logger, f"*\t Failed since : {self.conversion_result.name}"
+            )
             return self.conversion_result
 
         if self.view_scenario:
             self.sim_wrapper.view_scenario(source_file, self.config.esmini.window_size)
         if self.render_to_gif:
-            self.sim_wrapper.render_scenario_to_gif(source_file,
-                                                    self.config.general.path_output + self.config.general.name_xosc
-                                                    + ".gif")
+            self.sim_wrapper.render_scenario_to_gif(
+                source_file,
+                self.config.general.path_output
+                + self.config.general.name_xosc
+                + ".gif",
+            )
 
         dt_sim = self.dt_sim if self.dt_sim is not None else self.dt_cr / 10
         res: WrapperSimResult = self.sim_wrapper.simulate_scenario(xosc_file, dt_sim)
         if res.ending_cause is ESimEndingCause.FAILURE:
             self.conversion_result = EFailureReason.SIMULATION_FAILED_CREATING_OUTPUT
-            util_logger.print_and_log_error(logger, f"*\t Failed since : {self.conversion_result.name}")
+            util_logger.print_and_log_error(
+                logger, f"*\t Failed since : {self.conversion_result.name}"
+            )
             return self.conversion_result
         if len(res.states) == 0:
             self.conversion_result = EFailureReason.NO_DYNAMIC_BEHAVIOR_FOUND
-            util_logger.print_and_log_error(logger, f"*\t Failed since : {self.conversion_result.name}")
+            util_logger.print_and_log_error(
+                logger, f"*\t Failed since : {self.conversion_result.name}"
+            )
             return self.conversion_result
         sim_time = res.sim_time
         runtime += res.runtime
         ending_cause = res.ending_cause
-        util_logger.print_and_log_info(logger, f"*\t Esmini simulation takes {res.runtime:.2f} s")
+        util_logger.print_and_log_info(
+            logger, f"*\t Esmini simulation takes {res.runtime:.2f} s"
+        )
 
         start_time = time.time()
 
-        ego_vehicle, ego_vehicle_found_with_filter = self._find_ego_vehicle(list(res.states.keys()))
+        ego_vehicle, ego_vehicle_found_with_filter = self._find_ego_vehicle(
+            list(res.states.keys())
+        )
         keep_ego_vehicle = self.keep_ego_vehicle
 
-        obstacles_extra_info = ObstacleExtraInfoFinder(xosc_file, set(res.states.keys())).run()
+        obstacles_extra_info = ObstacleExtraInfoFinder(
+            xosc_file, set(res.states.keys())
+        ).run()
         obstacles_extra_info_finder_error = None
         if isinstance(obstacles_extra_info, AnalyzerErrorResult):
             obstacles_extra_info_finder_error = obstacles_extra_info
             obstacles_extra_info = {o_name: None for o_name in res.states.keys()}
 
         obstacles = self._create_obstacles_from_state_lists(
             scenario, ego_vehicle, res.states, res.sim_time, obstacles_extra_info
         )
 
-        scenario.add_objects([
-            obstacle for obstacle_name, obstacle in obstacles.items()
-            if obstacle is not None and (self.keep_ego_vehicle or ego_vehicle != obstacle_name)
-        ])
+        scenario.add_objects(
+            [
+                obstacle
+                for obstacle_name, obstacle in obstacles.items()
+                if obstacle is not None
+                and (self.keep_ego_vehicle or ego_vehicle != obstacle_name)
+            ]
+        )
         if len(scenario.lanelet_network.lanelets) > 0:
             scenario.assign_obstacles_to_lanelets()
 
         if self.trim_scenario:
             scenario = trim_scenario(scenario, deep_copy=False)
         pps = self.pps_builder.build(obstacles[ego_vehicle])
         runtime += time.time() - start_time
-        util_logger.print_and_log_info(logger, f"*\t Other conversion tasks take {time.time() - start_time:.2f} s")
-        util_logger.print_and_log_info(logger, f"* {self.config.general.name_xosc} is successfully converted 🏆!")
+        util_logger.print_and_log_info(
+            logger, f"*\t Other conversion tasks take {time.time() - start_time:.2f} s"
+        )
+        util_logger.print_and_log_info(
+            logger, f"* {self.config.general.name_xosc} is successfully converted 🏆!"
+        )
 
         if self.config.debug.write_to_xml:
             self.write_to_xml(scenario, pps)
 
         self.conversion_result = Osc2CrConverterResult(
             statistics=self.build_statistics(
                 obstacles=obstacles,
                 ego_vehicle=ego_vehicle,
                 ego_vehicle_found_with_filter=ego_vehicle_found_with_filter,
                 keep_ego_vehicle=keep_ego_vehicle,
                 ending_cause=ending_cause,
                 sim_time=sim_time,
-                runtime=runtime
+                runtime=runtime,
             ),
             analysis=self.run_analysis(
                 scenario=scenario,
                 obstacles=obstacles,
                 ego_vehicle=ego_vehicle,
                 keep_ego_vehicle=keep_ego_vehicle,
-                obstacles_extra_info=obstacles_extra_info
+                obstacles_extra_info=obstacles_extra_info,
             ),
             xosc_file=xosc_file,
             xodr_file=xodr_file,
             xodr_conversion_error=xodr_conversion_error,
             obstacles_extra_info_finder_error=obstacles_extra_info_finder_error,
             scenario=scenario,
             planning_problem_set=pps,
@@ -223,47 +272,56 @@
         if not path.exists(source_file):
             return EFailureReason.SCENARIO_FILE_INVALID_PATH
         root = ElementTree.parse(source_file).getroot()
         if root.find("Storyboard") is None:
             if root.find("Catalog") is not None:
                 return EFailureReason.SCENARIO_FILE_IS_CATALOG
             elif (pvd := root.find("ParameterValueDistribution")) is not None:
-                if (alternative_file := pvd.find("ScenarioFile[@filepath]")) is not None:
+                if (
+                    alternative_file := pvd.find("ScenarioFile[@filepath]")
+                ) is not None:
                     warnings.warn(
-                        f'<Osc2CrConverter/_pre_parse_scenario> {path.basename(source_file)} contains no source file, '
-                        f'but references another OpenSCENARIO file: \"'
-                        f'{path.join(path.dirname(source_file), alternative_file.attrib["filepath"])}\"'
+                        f"<Osc2CrConverter/_pre_parse_scenario> {path.basename(source_file)} contains no source file, "
+                        f'but references another OpenSCENARIO file: "'
+                        f'{path.join(path.dirname(source_file), alternative_file.attrib["filepath"])}"'
                     )
                 return EFailureReason.SCENARIO_FILE_IS_PARAMETER_VALUE_DISTRIBUTION
             return EFailureReason.SCENARIO_FILE_CONTAINS_NO_STORYBOARD
 
-        if (implicit_odr_file := root.find("RoadNetwork/LogicFile[@filepath]")) is not None:
-            return path.join(path.dirname(source_file), implicit_odr_file.attrib["filepath"])
+        if (
+            implicit_odr_file := root.find("RoadNetwork/LogicFile[@filepath]")
+        ) is not None:
+            return path.join(
+                path.dirname(source_file), implicit_odr_file.attrib["filepath"]
+            )
         return None
 
-    def _create_basic_scenario(self, implicit_odr_file: Optional[str]) \
-            -> Tuple[Scenario, Optional[str], Optional[AnalyzerErrorResult]]:
+    def _create_basic_scenario(
+        self, implicit_odr_file: Optional[str]
+    ) -> Tuple[Scenario, Optional[str], Optional[AnalyzerErrorResult]]:
         """
         Creating the scenario with basic information and road networks (map)
         :param implicit_odr_file: the source file of openDRIVE map
         :return: the scenario with/without map, path of the openDRIVE, the reason of the failure if applicable
         """
         odr_file: Optional[str] = None
         if self.odr_file_override is not None:
             if path.exists(self.odr_file_override):
                 odr_file = self.odr_file_override
             else:
                 warnings.warn(
-                    f"<OpenSCENARIO2CRConverter/_create_scenario> File {self.odr_file_override} does not exist")
+                    f"<OpenSCENARIO2CRConverter/_create_scenario> File {self.odr_file_override} does not exist"
+                )
         elif implicit_odr_file is not None and self.use_implicit_odr_file:
             if path.exists(implicit_odr_file):
                 odr_file = implicit_odr_file
             else:
                 warnings.warn(
-                    f"<OpenSCENARIO2CRConverter/_create_scenario> File {implicit_odr_file} does not exist")
+                    f"<OpenSCENARIO2CRConverter/_create_scenario> File {implicit_odr_file} does not exist"
+                )
 
         odr_conversion_error = None
         if odr_file is not None:
             try:
                 scenario = opendrive_to_commonroad(odr_file)
                 scenario.dt = self.dt_cr
             except Exception as e:
@@ -282,173 +340,214 @@
     def _find_ego_vehicle(self, vehicle_name_list: List[str]) -> Tuple[str, bool]:
         """
         Finding the ego vehicle based on the given pattern if applicable.
         :param vehicle_name_list: the list of vehicle names
         :return: ego vehicle found/first vehicle in the list, indication of which situation
         """
         if self.ego_filter is not None:
-            found_ego_vehicles = [name for name in vehicle_name_list if self.ego_filter.match(name) is not None]
+            found_ego_vehicles = [
+                name
+                for name in vehicle_name_list
+                if self.ego_filter.match(name) is not None
+            ]
             if len(found_ego_vehicles) > 0:
                 return sorted(found_ego_vehicles)[0], True
 
         return sorted(vehicle_name_list)[0], False
 
     def _create_obstacles_from_state_lists(
-            self,
-            scenario: Scenario,
-            ego_vehicle: str,
-            states: Dict[str, List[SimScenarioObjectState]],
-            sim_time: float,
-            obstacles_extra_info: Dict[str, Optional[Vehicle]]
+        self,
+        scenario: Scenario,
+        ego_vehicle: str,
+        states: Dict[str, List[SimScenarioObjectState]],
+        sim_time: float,
+        obstacles_extra_info: Dict[str, Optional[Vehicle]],
     ) -> Dict[str, Optional[DynamicObstacle]]:
         """
         Creating obstacles based on the given vehicle state lists.
         :param scenario: basic scenario
         :param ego_vehicle: name of the ego vehicle
         :param states: state list
         :param sim_time: total simulation time (in esmini)
         :param obstacles_extra_info: extra information about the Vehicle
         :return: created CommonRoad obstacles
         """
-        final_timestamps = [step * self.dt_cr for step in range(math.floor(sim_time / self.dt_cr) + 1)]
+        final_timestamps = [
+            step * self.dt_cr for step in range(math.floor(sim_time / self.dt_cr) + 1)
+        ]
 
         def create_obstacle(obstacle_name: str) -> Optional[DynamicObstacle]:
             return self._osc_states_to_dynamic_obstacle(
                 obstacle_id=scenario.generate_object_id(),
                 states=states[obstacle_name],
                 timestamps=final_timestamps,
-                obstacle_extra_info=obstacles_extra_info[obstacle_name]
+                obstacle_extra_info=obstacles_extra_info[obstacle_name],
             )
 
         # Make sure ego vehicle is always the obstacle with the lowest obstacle_id
         obstacles = {ego_vehicle: create_obstacle(ego_vehicle)}
         for object_name in sorted(states.keys()):
             if object_name != ego_vehicle:
                 obstacles[object_name] = create_obstacle(object_name)
         return obstacles
 
     def _osc_states_to_dynamic_obstacle(
-            self,
-            obstacle_id: int,
-            states: List[SimScenarioObjectState],
-            timestamps: List[float],
-            obstacle_extra_info: Optional[Vehicle],
+        self,
+        obstacle_id: int,
+        states: List[SimScenarioObjectState],
+        timestamps: List[float],
+        obstacle_extra_info: Optional[Vehicle],
     ) -> Optional[DynamicObstacle]:
         if len(states) == 0:
             return None
         first_occurred_timestamp = min([state.get_timestamp() for state in states])
         last_occurred_timestamp = max([state.get_timestamp() for state in states])
-        first_used_timestamp = min([t for t in timestamps], key=lambda t: math.fabs(first_occurred_timestamp - t))
-        last_used_timestamp = min([t for t in timestamps], key=lambda t: math.fabs(last_occurred_timestamp - t))
+        first_used_timestamp = min(
+            [t for t in timestamps],
+            key=lambda t: math.fabs(first_occurred_timestamp - t),
+        )
+        last_used_timestamp = min(
+            [t for t in timestamps],
+            key=lambda t: math.fabs(last_occurred_timestamp - t),
+        )
         first_used_time_step = round(first_used_timestamp / self.dt_cr)
         last_used_time_step = round(last_used_timestamp / self.dt_cr)
-        used_timestamps = sorted([t for t in timestamps if first_used_timestamp <= t <= last_used_timestamp])
-        used_states = [ScenarioObjectState.build_interpolated(states, t, obstacle_extra_info) for t in used_timestamps]
+        used_timestamps = sorted(
+            [t for t in timestamps if first_used_timestamp <= t <= last_used_timestamp]
+        )
+        used_states = [
+            ScenarioObjectState.build_interpolated(states, t, obstacle_extra_info)
+            for t in used_timestamps
+        ]
 
         obstacle_type = states[0].get_obstacle_type()
         if obstacle_type == ObstacleType.PEDESTRIAN:
             # for pedestrian, we consider an overapproximated circular area.
             # see: Koschi, Markus, et al. "Set-based prediction of pedestrians in urban environments considering
             # formalized traffic rules." IEEE ITSC, 2018
-            shape = Circle(max(states[0].get_object_length()/2., states[0].get_object_width())/2.)
+            shape = Circle(
+                max(states[0].get_object_length() / 2.0, states[0].get_object_width())
+                / 2.0
+            )
         else:
-            shape = Rectangle(states[0].get_object_length(), states[0].get_object_width())
+            shape = Rectangle(
+                states[0].get_object_length(), states[0].get_object_width()
+            )
 
         trajectory = Trajectory(
             first_used_time_step,
-            [state.to_cr_state(i + first_used_time_step) for i, state in enumerate(used_states)]
+            [
+                state.to_cr_state(i + first_used_time_step)
+                for i, state in enumerate(used_states)
+            ],
         )
         prediction = TrajectoryPrediction(trajectory, shape)
         prediction.final_time_step = last_used_time_step
         prediction.initial_time_step = first_used_time_step
 
         return DynamicObstacle(
             obstacle_id=obstacle_id,
             obstacle_type=obstacle_type,
             obstacle_shape=shape,
             initial_state=trajectory.state_list[0],
-            prediction=prediction
+            prediction=prediction,
         )
 
     def write_to_xml(
-            self,
-            scenario: Scenario,
-            pps: PlanningProblemSet,
+        self,
+        scenario: Scenario,
+        pps: PlanningProblemSet,
     ) -> None:
         """
         Writing the CommonRoad scenario to xml file together with the planning problem set
         :param scenario: CommonRoad scenario
         :param pps: planning problem set
         """
-        COUNTRY = 'OSC'  # OpenSCENARIO
+        COUNTRY = "OSC"  # OpenSCENARIO
         SCENE = self.config.general.name_xosc
         CONFIG = self.config.scenario.config
         # T: single trajectories
         PRED = self.config.scenario.pred
-        file_name = COUNTRY + '_' + SCENE + '_' + CONFIG + '_' + 'T-' + PRED + '.xml'
-        fw = CommonRoadFileWriter(scenario, pps, self.author, self.affiliation, self.source, self.tags)
-        fw.write_to_file(self.config.general.path_output + file_name, OverwriteExistingFile.ALWAYS)
+        file_name = COUNTRY + "_" + SCENE + "_" + CONFIG + "_" + "T-" + PRED + ".xml"
+        fw = CommonRoadFileWriter(
+            scenario, pps, self.author, self.affiliation, self.source, self.tags
+        )
+        fw.write_to_file(
+            self.config.general.path_output + file_name, OverwriteExistingFile.ALWAYS
+        )
 
     @staticmethod
     def build_statistics(
-            obstacles: Dict[str, Optional[DynamicObstacle]],
-            ego_vehicle: str,
-            ego_vehicle_found_with_filter: bool,
-            keep_ego_vehicle: bool,
-            ending_cause: ESimEndingCause,
-            sim_time: float,
-            runtime: float
+        obstacles: Dict[str, Optional[DynamicObstacle]],
+        ego_vehicle: str,
+        ego_vehicle_found_with_filter: bool,
+        keep_ego_vehicle: bool,
+        ending_cause: ESimEndingCause,
+        sim_time: float,
+        runtime: float,
     ) -> ConversionStatistics:
         """
         Building the statistics of the conversion.
         :param obstacles: created obstacles
         :param ego_vehicle: name of the ego vehicle
         :param ego_vehicle_found_with_filter: the way of ego creation
         :param keep_ego_vehicle: whether the ego vehicle is kept
         :param ending_cause: why simulation is finished
         :param sim_time: simulation time in total
         :param runtime: runtime of converting the scenario
         :return: statistics
         """
-        util_logger.print_and_log_info(logger, "# ===========  Conversion Statistics  ========== #")
+        util_logger.print_and_log_info(
+            logger, "# ===========  Conversion Statistics  ========== #"
+        )
         util_logger.print_and_log_info(logger, f"#\t Nr of obstacles: {len(obstacles)}")
-        util_logger.print_and_log_info(logger, f"#\t Scenario duration: {sim_time:.2f} s")
-        util_logger.print_and_log_info(logger, f"#\t The ego vehicle is removed"
-                                               f"" if not keep_ego_vehicle else "#\t the ego vehicle is kept")
-        util_logger.print_and_log_info(logger, f"#\t The ending cause {ending_cause.name}")
-        util_logger.print_and_log_info(logger, "# ============================================== #")
+        util_logger.print_and_log_info(
+            logger, f"#\t Scenario duration: {sim_time:.2f} s"
+        )
+        util_logger.print_and_log_info(
+            logger,
+            f"#\t The ego vehicle is removed" f""
+            if not keep_ego_vehicle
+            else "#\t the ego vehicle is kept",
+        )
+        util_logger.print_and_log_info(
+            logger, f"#\t The ending cause {ending_cause.name}"
+        )
+        util_logger.print_and_log_info(
+            logger, "# ============================================== #"
+        )
         return ConversionStatistics(
             num_obstacle_conversions=len(obstacles),
-            failed_obstacle_conversions=[o_name for o_name, o in obstacles.items() if o is None],
+            failed_obstacle_conversions=[
+                o_name for o_name, o in obstacles.items() if o is None
+            ],
             ego_vehicle=ego_vehicle,
             ego_vehicle_found_with_filter=ego_vehicle_found_with_filter,
             ego_vehicle_removed=not keep_ego_vehicle,
             sim_ending_cause=ending_cause,
             sim_time=sim_time,
-            runtime=runtime
+            runtime=runtime,
         )
 
     def run_analysis(
-            self,
-            scenario: Scenario,
-            obstacles: Dict[str, Optional[DynamicObstacle]],
-            ego_vehicle: str,
-            keep_ego_vehicle: bool,
-            obstacles_extra_info: Dict[str, Optional[Vehicle]],
+        self,
+        scenario: Scenario,
+        obstacles: Dict[str, Optional[DynamicObstacle]],
+        ego_vehicle: str,
+        keep_ego_vehicle: bool,
+        obstacles_extra_info: Dict[str, Optional[Vehicle]],
     ) -> Dict[EAnalyzer, Tuple[float, Dict[str, AnalyzerResult]]]:
         analyzers = self.get_analyzer_objects()
         if len(analyzers) == 0:
             return {}
         else:
             trimmed_scenario = trim_scenario(scenario)
             if not keep_ego_vehicle:
                 trimmed_scenario.add_objects(obstacles[ego_vehicle])
                 if len(scenario.lanelet_network.lanelets) > 0:
                     scenario.assign_obstacles_to_lanelets()
             return {
                 e_analyzer: analyzer.run(
-                    trimmed_scenario,
-                    obstacles,
-                    obstacles_extra_info
-                ) for e_analyzer, analyzer in analyzers.items()
+                    trimmed_scenario, obstacles, obstacles_extra_info
+                )
+                for e_analyzer, analyzer in analyzers.items()
             }
-
```

### Comparing `commonroad-openscenario-converter-0.0.4/osc_cr_converter/converter/result.py` & `commonroad-openscenario-converter-0.1.0/osc_cr_converter/converter/result.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __author__ = "Michael Ratzel, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.0.4"
+__version__ = "0.1.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
-__status__ = "Pre-alpha"
+__status__ = "beta"
 
 from dataclasses import dataclass
 from multiprocessing import Lock
 from os import path
 from typing import Dict, Optional, Tuple, ClassVar
 
 from commonroad.common.file_reader import CommonRoadFileReader
@@ -28,48 +28,57 @@
     """
     The result of the Osc2CrConverter it contains the converted scenario and planning problem set as well as general
     statistics and other useful information.
 
     For faster import of the results the loading of the scenario and planning problem set can be deactivated using
     the Serializable interface
     """
+
     __lock: ClassVar[Lock] = Lock()
     statistics: ConversionStatistics
     analysis: Dict[EAnalyzer, Tuple[float, Dict[str, AnalyzerResult]]]
     xosc_file: str
     xodr_file: Optional[str]
     xodr_conversion_error: Optional[AnalyzerErrorResult]
     obstacles_extra_info_finder_error: Optional[AnalyzerErrorResult]
 
     scenario: Optional[Scenario]
     planning_problem_set: Optional[PlanningProblemSet]
 
     def __getstate__(self) -> Dict:
         data = self.__dict__.copy()
-        if self.scenario is not None and self.planning_problem_set is not None \
-                and Serializable.storage_dir is not None:
+        if (
+            self.scenario is not None
+            and self.planning_problem_set is not None
+            and Serializable.storage_dir is not None
+        ):
             del data["scenario"]
             del data["planning_problem_set"]
-            file_path_base = path.join(Serializable.storage_dir, path.splitext(path.basename(self.xosc_file))[0])
+            file_path_base = path.join(
+                Serializable.storage_dir,
+                path.splitext(path.basename(self.xosc_file))[0],
+            )
             with self.__lock:
                 i = 1
                 while path.exists(file_path := file_path_base + f"{i}.xml"):
                     i += 1
                 CommonRoadFileWriter(
                     scenario=self.scenario,
-                    planning_problem_set=self.planning_problem_set
+                    planning_problem_set=self.planning_problem_set,
                 ).write_to_file(file_path, OverwriteExistingFile.SKIP)
                 data["file_path"] = file_path
 
         return data
 
     def __setstate__(self, data: Dict):
         if "file_path" in data:
             scenario = None
             pps = None
             if path.exists(data["file_path"]) and Serializable.import_extra_files:
-                scenario, pps = CommonRoadFileReader(data["file_path"]).open(lanelet_assignment=True)
+                scenario, pps = CommonRoadFileReader(data["file_path"]).open(
+                    lanelet_assignment=True
+                )
             del data["file_path"]
             data["scenario"] = scenario
             data["planning_problem_set"] = pps
 
         self.__dict__.update(data)
```

### Comparing `commonroad-openscenario-converter-0.0.4/osc_cr_converter/converter/serializable.py` & `commonroad-openscenario-converter-0.1.0/osc_cr_converter/converter/serializable.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __author__ = "Michael Ratzel, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.0.1"
+__version__ = "0.1.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
-__status__ = "Pre-alpha"
+__status__ = "beta"
 
 import base64
 import pickle
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Dict, Optional, ClassVar
 
@@ -17,14 +17,15 @@
 class Serializable(ABC):
     """
     The main interface to enforce that classes can be pickled.
 
     Also when unpickle any file implementing is assumed to contain a small amount of data, unless the
     import_extra_files field is set to True here
     """
+
     storage_dir: ClassVar[Optional[str]] = None
     import_extra_files: ClassVar[bool] = True
 
     @abstractmethod
     def __getstate__(self) -> Dict:
         raise NotImplementedError
```

### Comparing `commonroad-openscenario-converter-0.0.4/osc_cr_converter/udp_driver/common.py` & `commonroad-openscenario-converter-0.1.0/osc_cr_converter/udp_driver/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __author__ = "Michael Ratzel, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.0.2"
+__version__ = "0.1.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
-__status__ = "Pre-alpha"
+__status__ = "beta"
 
 
 """
 Code is original from
  https://github.com/esmini/esmini/blob/2e438be3b3a176dafd296fa5e41742f886868e6f/scripts/udp_driver/udp_osi_common.py.
  Exemplary usage please also refer to the esmini repository. 
  
@@ -46,39 +46,41 @@
 from socket import *
 import struct
 
 from osi3.osi_groundtruth_pb2 import GroundTruth
 
 
 input_modes = {
-  'driverInput': 1,
-  'stateXYZHPR': 2,
-  'stateXYH': 3,
-  'stateH': 4,
+    "driverInput": 1,
+    "stateXYZHPR": 2,
+    "stateXYH": 3,
+    "stateH": 4,
 }
 
 base_port = 53995
 
 
-class UdpSender():
-    def __init__(self, ip='127.0.0.1', port=base_port):
+class UdpSender:
+    def __init__(self, ip="127.0.0.1", port=base_port):
         # Create a UDP socket
         self.sock = socket(AF_INET, SOCK_DGRAM)
         self.addr = (ip, port)
 
     def send(self, msg):
         self.sock.sendto(msg, self.addr)
 
     def close(self):
         self.sock.close()
 
 
-class UdpReceiver():
-    def __init__(self, ip='127.0.0.1', port=base_port, timeout=-1):
-        self.buffersize = 8208  # MAX OSI data size (contract with esmini) + header (two ints)
+class UdpReceiver:
+    def __init__(self, ip="127.0.0.1", port=base_port, timeout=-1):
+        self.buffersize = (
+            8208  # MAX OSI data size (contract with esmini) + header (two ints)
+        )
         # Create a UDP socket
         self.sock = socket(AF_INET, SOCK_DGRAM)
         if timeout >= 0:
             self.sock.settimeout(timeout)
         # Bind to address and ip
         self.sock.bind((ip, port))
 
@@ -87,52 +89,54 @@
         message = bytesAddressPair[0]
         return message
 
     def close(self):
         self.sock.close()
 
 
-class OSIReceiver():
+class OSIReceiver:
     def __init__(self):
         self.udp_receiver = UdpReceiver(port=48198)
         self.osi_msg = GroundTruth()
 
     def receive(self):
         done = False
         next_index = 1
-        complete_msg = b''
+        complete_msg = b""
 
         # Large nessages might be split in multiple parts
         # esmini will add a counter to indicate sequence number 0, 1, 2...
         # negative counter means last part and message is now complete
         while not done:
             # receive header
             msg = self.udp_receiver.receive()
 
             # extract message parts
             header_size = 4 + 4  # counter(int) + size(unsigned int)
-            counter, size, frame = struct.unpack('iI{}s'.format(len(msg)-header_size), msg)
+            counter, size, frame = struct.unpack(
+                "iI{}s".format(len(msg) - header_size), msg
+            )
             # print('counter {} size {}'.format(counter, size))
 
-            if not (len(frame) == size == len(msg)-8):
-                print('Error: Unexpected invalid lengths')
+            if not (len(frame) == size == len(msg) - 8):
+                print("Error: Unexpected invalid lengths")
                 return
 
             if counter == 1:  # new message
-                complete_msg = b''
+                complete_msg = b""
                 next_index = 1
 
             # Compose complete message
             if counter == 1 or abs(counter) == next_index:
                 complete_msg += frame
                 next_index += 1
                 if counter < 0:  # negative counter number indicates end of message
                     done = True
             else:
-                next_index = 1   # out of sync, reset
+                next_index = 1  # out of sync, reset
 
         # Parse and return message
         self.osi_msg.ParseFromString(complete_msg)
         return self.osi_msg
 
     def close(self):
-        self.udp_receiver.close()
+        self.udp_receiver.close()
```

### Comparing `commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/abs_rel.py` & `commonroad-openscenario-converter-0.1.0/osc_cr_converter/utility/abs_rel.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __author__ = "Michael Ratzel, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.0.1"
+__version__ = "0.1.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
-__status__ = "Pre-alpha"
+__status__ = "beta"
 
 from dataclasses import dataclass
 from enum import Enum
 from typing import Generic, TypeVar, ClassVar, Callable, Union
 
 from commonroad.common.util import Interval, AngleInterval
 
@@ -19,14 +19,15 @@
 class AbsRel(Generic[T]):
     """
     A class used for configuration parameters storing absolute or relative values.
     If _value is used as a relative configuration value, one of the four elementary arithmetic operations is applied to
     it
     If _value is used as an absolute configuration value, it is returned without modification
     """
+
     __create_key: ClassVar[object] = object()
     _value: T
     _usage: "AbsRel.EUsage"
 
     def __init__(self, value: T, usage: "AbsRel.EUsage"):
         object.__setattr__(self, "_value", value)
         object.__setattr__(self, "_usage", usage)
@@ -50,25 +51,29 @@
             obj = object.__new__(cls)
             obj._value_ = len(cls.__members__)
             obj.formula = apply_to_reference_value
             return obj
 
         ABS = (lambda v, _: v,)
         REL_ADD = (lambda v, r: v + r,)
-        REL_SUB = (lambda v, r: v - r)
+        REL_SUB = lambda v, r: v - r
         REL_MUL = (lambda v, r: v * r,)
         REL_DIV = (lambda v, r: v / r,)
 
     def get(self, reference_value: float) -> T:
         """
         Applying the applicable usage formula and returning the reference value
 
         :param reference_value:float: The reference value this is relative to (if it is not an absolute AbsRel)
         :return: The modified _value if relative or _value if absolute
         """
         if isinstance(self._value, (Interval, AngleInterval)):
             return type(self._value)(
-                start=self._usage.apply_value_to_reference(self._value.start, reference_value),
-                end=self._usage.apply_value_to_reference(self._value.end, reference_value),
+                start=self._usage.apply_value_to_reference(
+                    self._value.start, reference_value
+                ),
+                end=self._usage.apply_value_to_reference(
+                    self._value.end, reference_value
+                ),
             )
         elif isinstance(self._value, (float, int)):
             return self._usage.apply_value_to_reference(self._value, reference_value)
```

### Comparing `commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/configuration.py` & `commonroad-openscenario-converter-0.1.0/osc_cr_converter/utility/configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __author__ = "Michael Ratzel, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.0.4"
+__version__ = "0.1.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
-__status__ = "Pre-alpha"
+__status__ = "beta"
 
 import dataclasses
 import inspect
 from dataclasses import dataclass, field
 from typing import Union, Any, Dict, List, Optional
 from datetime import datetime
 import pathlib
@@ -67,68 +67,78 @@
 
         :param: Item for which content should be returned.
         :return: Item value.
         """
         try:
             value = self.__getattribute__(item)
         except AttributeError as e:
-            raise KeyError(f"{item} is not a parameter of {self.__class__.__name__}") from e
+            raise KeyError(
+                f"{item} is not a parameter of {self.__class__.__name__}"
+            ) from e
         return value
 
     def __setitem__(self, key: str, value: Any):
         """
         Setter for item.
 
         :param key: Name of item.
         :param value: Value of item.
         """
         try:
             self.__setattr__(key, value)
         except AttributeError as e:
-            raise KeyError(f"{key} is not a parameter of {self.__class__.__name__}") from e
+            raise KeyError(
+                f"{key} is not a parameter of {self.__class__.__name__}"
+            ) from e
 
     @classmethod
-    def load(cls, file_path: Union[pathlib.Path, str], validate_types: bool = True) -> 'ConverterParams':
+    def load(
+        cls, file_path: Union[pathlib.Path, str], validate_types: bool = True
+    ) -> "ConverterParams":
         """
         Loads config file and creates parameter class.
 
         :param file_path: Path to yaml file containing config parameters.
         :param validate_types: overwrite the default params
         :return: Base parameter class.
         """
         file_path = pathlib.Path(file_path)
-        assert file_path.suffix == ".yaml", f"File type {file_path.suffix} is unsupported! Please use .yaml!"
+        assert (
+            file_path.suffix == ".yaml"
+        ), f"File type {file_path.suffix} is unsupported! Please use .yaml!"
         loaded_yaml = OmegaConf.load(file_path)
         if validate_types:
             OmegaConf.merge(OmegaConf.structured(ConverterParams), loaded_yaml)
         params = _dict_to_params(OmegaConf.to_object(loaded_yaml), cls)
         return params
 
 
 @dataclass
 class GeneralParams(BaseParam):
     """Parameters specifying the general setup"""
 
     # path of the root
     # name of the OpenSCENARIO file and its path
-    name_xosc: str = ''
+    name_xosc: str = ""
 
     # path for the output files
-    path_output_abs: str = os.path.normpath(os.path.join(os.path.dirname(__file__), "../..")) + "/output/"
+    path_output_abs: str = (
+        os.path.normpath(os.path.join(os.path.dirname(__file__), "../..")) + "/output/"
+    )
     # path for logging information
-    path_output_log: str = path_output_abs + 'log/'
+    path_output_log: str = path_output_abs + "log/"
     string_date_time = datetime.now().strftime("%Y_%m_%d_%H-%M-%S")
 
     def __init__(self):
         super().__init__()
         os.makedirs(self.path_output_abs, exist_ok=True)
 
     @property
     def path_output(self):
-        path_output = self.path_output_abs + self.name_xosc + '/'
+        path_output = self.path_output_abs + self.name_xosc + "/"
         os.makedirs(path_output, exist_ok=True)
         return path_output
 
 
 @dataclass
 class DebugParams(BaseParam):
     """Parameters specifying debug-related information"""
@@ -154,25 +164,26 @@
     """Parameters specifying the esmini settings"""
 
     @dataclass(frozen=True)
     class WindowSize:
         """
         Utility class storing information about the size and position of a window
         """
+
         x: int = 0
         y: int = 0
         width: int = 640
         height: int = 480
 
     # version
     version: str = "default"  # we use v2.29.3 as default version
 
     # lower and upper time limits for the simulation duration
-    min_time: float = 5.
-    max_time: float = 60.
+    min_time: float = 5.0
+    max_time: float = 60.0
 
     # logging information
     log_to_console: bool = False
     log_to_file: bool = True
 
     # run the simulation using this random seed
     random_seed: int = 0
@@ -203,31 +214,36 @@
     # scenario information
     # CommonRoad time step size
     dt_cr: float = 0.1
     keep_ego_vehicle: bool = True
     # trim the map based on the vehicle information
     trim_scenario: bool = False
     # default config & pred for specifying the scenario name:
-    config: str = '1'  # 1-9
-    pred: str = '1'
+    config: str = "1"  # 1-9
+    pred: str = "1"
 
 
 @dataclass
 class ConverterParams(BaseParam):
     """Configuration parameters for OpenSCENARIO2CommonRoad converter."""
+
     general: GeneralParams = field(default_factory=GeneralParams)
     debug: DebugParams = field(default_factory=DebugParams)
     esmini: EsminiParams = field(default_factory=EsminiParams)
     scenario: ScenarioParams = field(default_factory=ScenarioParams)
 
     @staticmethod
     def initialize_planning_problem_set():
         planning_problem_set = PPSBuilder()
-        planning_problem_set.time_interval = AbsRel(Interval(-10, 0), AbsRel.EUsage.REL_ADD)
+        planning_problem_set.time_interval = AbsRel(
+            Interval(-10, 0), AbsRel.EUsage.REL_ADD
+        )
         planning_problem_set.pos_length = AbsRel(50, AbsRel.EUsage.ABS)
         planning_problem_set.pos_width = AbsRel(10, AbsRel.EUsage.ABS)
         planning_problem_set.pos_rotation = AbsRel(0, AbsRel.EUsage.REL_ADD)
         planning_problem_set.pos_center_x = AbsRel(0, AbsRel.EUsage.REL_ADD)
         planning_problem_set.pos_center_y = AbsRel(0, AbsRel.EUsage.REL_ADD)
-        planning_problem_set.velocity_interval = AbsRel(Interval(-5, 5), AbsRel.EUsage.REL_ADD)
+        planning_problem_set.velocity_interval = AbsRel(
+            Interval(-5, 5), AbsRel.EUsage.REL_ADD
+        )
         planning_problem_set.orientation_interval = None
         return planning_problem_set
```

### Comparing `commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/general.py` & `commonroad-openscenario-converter-0.1.0/osc_cr_converter/utility/general.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __author__ = "Michael Ratzel, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.0.1"
+__version__ = "0.1.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
-__status__ = "Pre-alpha"
+__status__ = "beta"
 
 import copy
 from dataclasses import fields
 from typing import get_origin, Union, get_args
 
 from commonroad.scenario.scenario import Scenario
 
@@ -16,35 +16,44 @@
 def trim_scenario(scenario: Scenario, deep_copy: bool = True) -> Scenario:
     trimmed_scenario = copy.deepcopy(scenario) if deep_copy else scenario
 
     if len(trimmed_scenario.lanelet_network.lanelets) == 0:
         return trimmed_scenario
     trimmed_scenario.assign_obstacles_to_lanelets()
 
-    if any(obstacle.prediction.shape_lanelet_assignment is None for obstacle in trimmed_scenario.dynamic_obstacles):
+    if any(
+        obstacle.prediction.shape_lanelet_assignment is None
+        for obstacle in trimmed_scenario.dynamic_obstacles
+    ):
         return trimmed_scenario
 
     used_lanelets = set()
     for obstacle in trimmed_scenario.dynamic_obstacles:
         for lanelet_set in obstacle.prediction.shape_lanelet_assignment.values():
             for lanelet in lanelet_set:
                 used_lanelets.add(lanelet)
 
     removable_lanelets = []
-    all_ids = {lanelet.lanelet_id for lanelet in trimmed_scenario.lanelet_network.lanelets}
+    all_ids = {
+        lanelet.lanelet_id for lanelet in trimmed_scenario.lanelet_network.lanelets
+    }
     for lanelet_id in all_ids - used_lanelets:
         lanelet = trimmed_scenario.lanelet_network.find_lanelet_by_id(lanelet_id)
         if lanelet is not None:
             removable_lanelets.append(lanelet)
     trimmed_scenario.remove_lanelet(removable_lanelets)
     trimmed_scenario.assign_obstacles_to_lanelets()
 
     return trimmed_scenario
 
 
 def dataclass_is_complete(dataclass_object) -> bool:
     for field in fields(dataclass_object):
-        if get_origin(field.type) is not Union or type(None) not in get_args(field.type):
-            if not hasattr(dataclass_object, field.name) or getattr(dataclass_object, field.name) is None:
+        if get_origin(field.type) is not Union or type(None) not in get_args(
+            field.type
+        ):
+            if (
+                not hasattr(dataclass_object, field.name)
+                or getattr(dataclass_object, field.name) is None
+            ):
                 return False
     return True
-
```

### Comparing `commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/logger.py` & `commonroad-openscenario-converter-0.1.0/osc_cr_converter/utility/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 __author__ = "Michael Ratzel, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.0.4"
+__version__ = "0.1.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
-__status__ = "Pre-alpha"
+__status__ = "beta"
 
 import logging
 import os
 from osc_cr_converter.utility.configuration import ConverterParams
 
 
 def initialize_logger(config: ConverterParams) -> logging.Logger:
     # create log directory
     os.makedirs(config.general.path_output_log, exist_ok=True)
 
     # create logger
     logger = logging.getLogger()
 
     # create file handler (outputs to file)
-    path_log = os.path.join(config.general.path_output_log,
-                            f"convert_{config.general.string_date_time}.log")
+    path_log = os.path.join(
+        config.general.path_output_log, f"convert_{config.general.string_date_time}.log"
+    )
     file_handler = logging.FileHandler(path_log)
 
     # set logging levels
     logger.setLevel(config.debug.logging_level)
     file_handler.setLevel(config.debug.logging_level)
 
     # create log formatter
-    formatter = logging.Formatter("%(levelname)-8s [%(asctime)s] --- %(message)s (%(filename)s:%(lineno)s)",
-                                  "%Y-%m-%d %H:%M:%S")
+    formatter = logging.Formatter(
+        "%(levelname)-8s [%(asctime)s] --- %(message)s (%(filename)s:%(lineno)s)",
+        "%Y-%m-%d %H:%M:%S",
+    )
     file_handler.setFormatter(formatter)
 
     # add handlers
     logger.addHandler(file_handler)
 
     return logger
```

### Comparing `commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/obstacle_info.py` & `commonroad-openscenario-converter-0.1.0/osc_cr_converter/utility/obstacle_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,21 @@
 import os
 import warnings
 import xml.etree.ElementTree as Et
 from dataclasses import dataclass
 from os import path
 from typing import Dict, Optional, Set, Union
 
-from scenariogeneration.xosc import Vehicle, ParseOpenScenario, Scenario, CatalogReference, Catalog
+from scenariogeneration.xosc import (
+    Vehicle,
+    ParseOpenScenario,
+    Scenario,
+    CatalogReference,
+    Catalog,
+)
 
 from osc_cr_converter.analyzer.error import AnalyzerErrorResult
 from osc_cr_converter.utility.general import dataclass_is_complete
 
 
 @dataclass
 class ObstacleExtraInfoFinder:
@@ -25,62 +31,86 @@
     obstacle_names: Set[str] = None
 
     def run(self) -> Union[AnalyzerErrorResult, Dict[str, Optional[Vehicle]]]:
         assert dataclass_is_complete(self)
         try:
             scenario: Scenario = ParseOpenScenario(self.scenario_path)
 
-            matched_obstacles: Dict[str, Vehicle] = {o_name: None for o_name in self.obstacle_names}
+            matched_obstacles: Dict[str, Vehicle] = {
+                o_name: None for o_name in self.obstacle_names
+            }
             for scenario_object in scenario.entities.scenario_objects:
                 if scenario_object.name not in matched_obstacles.keys():
                     continue
-                if scenario_object.name in self.obstacle_names and isinstance(scenario_object.entityobject, Vehicle):
-                    matched_obstacles[scenario_object.name] = scenario_object.entityobject
+                if scenario_object.name in self.obstacle_names and isinstance(
+                    scenario_object.entityobject, Vehicle
+                ):
+                    matched_obstacles[
+                        scenario_object.name
+                    ] = scenario_object.entityobject
 
             if all([obstacle is not None for obstacle in matched_obstacles.values()]):
                 return matched_obstacles
 
             catalogs = self._parse_catalogs(scenario)
             for scenario_object in scenario.entities.scenario_objects:
                 if scenario_object.name not in matched_obstacles.keys():
                     continue
-                if scenario_object.name in matched_obstacles and matched_obstacles[scenario_object.name] is not None:
+                if (
+                    scenario_object.name in matched_obstacles
+                    and matched_obstacles[scenario_object.name] is not None
+                ):
                     continue
                 if isinstance(scenario_object.entityobject, CatalogReference):
                     if scenario_object.entityobject.catalogname in catalogs:
                         for obj in catalogs[scenario_object.entityobject.catalogname]:
-                            if obj.tag == "Vehicle" and obj.attrib["name"] == scenario_object.entityobject.entryname:
-                                matched_obstacles[scenario_object.name] = Vehicle.parse(obj)
+                            if (
+                                obj.tag == "Vehicle"
+                                and obj.attrib["name"]
+                                == scenario_object.entityobject.entryname
+                            ):
+                                matched_obstacles[scenario_object.name] = Vehicle.parse(
+                                    obj
+                                )
 
             return matched_obstacles
         except Exception as e:
-            warnings.warn(f"<ObstacleExtraInfoFinder/run> {path.basename(self.scenario_path)} failed with {str(e)}")
+            warnings.warn(
+                f"<ObstacleExtraInfoFinder/run> {path.basename(self.scenario_path)} failed with {str(e)}"
+            )
             return AnalyzerErrorResult.from_exception(e)
 
     def _parse_catalogs(self, scenario: Scenario) -> Dict[str, Et.Element]:
-        assert "VehicleCatalog" in Catalog._CATALOGS, "Probably the OpenSCENARIO standard changed"
+        assert (
+            "VehicleCatalog" in Catalog._CATALOGS
+        ), "Probably the OpenSCENARIO standard changed"
         if "VehicleCatalog" in scenario.catalog.catalogs:
             # Prefer the VehicleCatalog by inserting it at first
             catalog_locations = [scenario.catalog.catalogs["VehicleCatalog"]]
-            catalog_locations.extend([
-                location for l_name, location in scenario.catalog.catalogs.items() if l_name != "VehicleCatalog"
-            ])
+            catalog_locations.extend(
+                [
+                    location
+                    for l_name, location in scenario.catalog.catalogs.items()
+                    if l_name != "VehicleCatalog"
+                ]
+            )
         else:
             catalog_locations = scenario.catalog.catalogs.values()
 
         catalog_files = []
         for catalog_path in catalog_locations:
             catalog_path = path.join(path.dirname(self.scenario_path), catalog_path)
             for file in os.listdir(catalog_path):
                 file = path.join(catalog_path, file)
                 if path.isfile(file):
                     catalog_files.append(file)
 
         return {
-            catalog.attrib["name"]: catalog for catalog_file in catalog_files if
-            (catalog := self._parse_single_catalog(catalog_file)) is not None
+            catalog.attrib["name"]: catalog
+            for catalog_file in catalog_files
+            if (catalog := self._parse_single_catalog(catalog_file)) is not None
         }
 
     @staticmethod
     def _parse_single_catalog(catalog_file) -> Optional[Et.Element]:
         root = Et.parse(catalog_file)
         return root.find("Catalog")
```

### Comparing `commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/pps_builder.py` & `commonroad-openscenario-converter-0.1.0/osc_cr_converter/utility/pps_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 
 @dataclass
 class PPSBuilder:
     """
     Planning Problem Set builder
     """
+
     # Required
     time_interval: AbsRel[Interval] = AbsRel(Interval(-10, 0), AbsRel.EUsage.REL_ADD)
 
     pos_length: AbsRel[float] = AbsRel(50, AbsRel.EUsage.ABS)
     pos_width: AbsRel[float] = AbsRel(10, AbsRel.EUsage.ABS)
     pos_rotation: AbsRel[float] = AbsRel(0, AbsRel.EUsage.REL_ADD)
     pos_center_x: AbsRel[float] = AbsRel(0, AbsRel.EUsage.REL_ADD)
@@ -41,51 +42,55 @@
     orientation_interval: Optional[AbsRel[AngleInterval]] = None
 
     def build(self, obstacle: DynamicObstacle) -> PlanningProblemSet:
         assert dataclass_is_complete(self)
 
         first_state = obstacle.prediction.trajectory.state_list[0]
         final_state = obstacle.prediction.trajectory.final_state
-        initial_state = InitialState(position=first_state.position,
-                                     velocity=first_state.velocity,
-                                     orientation=first_state.orientation,
-                                     yaw_rate=first_state.yaw_rate,
-                                     slip_angle=first_state.slip_angle,
-                                     time_step=first_state.time_step)
+        initial_state = InitialState(
+            position=first_state.position,
+            velocity=first_state.velocity,
+            orientation=first_state.orientation,
+            yaw_rate=first_state.yaw_rate,
+            slip_angle=first_state.slip_angle,
+            time_step=first_state.time_step,
+        )
 
         goal_state = CustomState()
 
         position_rotation = self.pos_rotation.get(final_state.orientation)
         while not is_valid_orientation(position_rotation):
             if position_rotation > 0:
                 position_rotation -= 2 * np.pi
             else:
                 position_rotation += 2 * np.pi
-        center = np.array((
-            self.pos_center_x.get(final_state.position[0]),
-            self.pos_center_y.get(final_state.position[1]),
-        ))
+        center = np.array(
+            (
+                self.pos_center_x.get(final_state.position[0]),
+                self.pos_center_y.get(final_state.position[1]),
+            )
+        )
         goal_state.position = Rectangle(
             length=self.pos_length.get(obstacle.obstacle_shape.length),
             width=self.pos_width.get(obstacle.obstacle_shape.width),
             center=center,
-            orientation=position_rotation
+            orientation=position_rotation,
         )
 
         goal_state.time_step = self.time_interval.get(final_state.time_step)
 
         if self.velocity_interval is not None:
             goal_state.velocity = self.velocity_interval.get(final_state.velocity)
         if self.orientation_interval is not None:
-            goal_state.orientation = self.orientation_interval.get(final_state.orientation)
+            goal_state.orientation = self.orientation_interval.get(
+                final_state.orientation
+            )
 
         return PlanningProblemSet(
             [
                 PlanningProblem(
                     planning_problem_id=obstacle.obstacle_id,
                     initial_state=initial_state,
-                    goal_region=GoalRegion(
-                        state_list=[goal_state]
-                    )
+                    goal_region=GoalRegion(state_list=[goal_state]),
                 )
             ]
         )
```

### Comparing `commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/statistics.py` & `commonroad-openscenario-converter-0.1.0/osc_cr_converter/utility/statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __author__ = "Michael Ratzel, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
 __version__ = "0.0.1"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
-__status__ = "Pre-alpha"
+__status__ = "beta"
 
 from dataclasses import dataclass
 from typing import Optional, List, Dict
 
 from osc_cr_converter.wrapper.esmini.esmini_wrapper import ESimEndingCause
 from osc_cr_converter.converter.serializable import Serializable
```

### Comparing `commonroad-openscenario-converter-0.0.4/osc_cr_converter/utility/visualization.py` & `commonroad-openscenario-converter-0.1.0/osc_cr_converter/utility/visualization.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __author__ = "Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.0.1"
+__version__ = "0.1.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
-__status__ = "Pre-alpha"
+__status__ = "beta"
 
 from enum import Enum
 import numpy as np
 from typing import List, Union
 import matplotlib.pyplot as plt
 
 from commonroad.visualization.mp_renderer import MPRenderer
@@ -32,36 +32,52 @@
     TUMblack = (0, 0, 0)
     TUMlightgray = (217 / 255, 218 / 255, 219 / 255)
 
 
 zorder = 22
 
 
-def draw_state_list(rnd: MPRenderer, state_list: List[Union[PMState, CustomState]],
-                    start_time_step: Union[None, int] = None,
-                    color: TUMcolor = TUMcolor.TUMdarkblue,
-                    linewidth: float = 0.75) -> None:
+def draw_state_list(
+    rnd: MPRenderer,
+    state_list: List[Union[PMState, CustomState]],
+    start_time_step: Union[None, int] = None,
+    color: TUMcolor = TUMcolor.TUMdarkblue,
+    linewidth: float = 0.75,
+) -> None:
     """
     Visualizing the state list as a connecting trajectory. The transparency is based on the starting
     time step.
     """
     global zorder
     # visualize optimal trajectory
     pos = np.asarray([state.position for state in state_list])
     if start_time_step:
         opacity = 0.5 * (start_time_step / len(state_list) + 1)
     else:
         opacity = 1
-    rnd.ax.plot(pos[:, 0], pos[:, 1], linestyle='-', marker='o', color=color, markersize=5,
-                zorder=zorder, linewidth=linewidth, alpha=opacity)
+    rnd.ax.plot(
+        pos[:, 0],
+        pos[:, 1],
+        linestyle="-",
+        marker="o",
+        color=color,
+        markersize=5,
+        zorder=zorder,
+        linewidth=linewidth,
+        alpha=opacity,
+    )
     zorder += 1
 
 
-def draw_dyn_vehicle_shape(rnd: MPRenderer, obstacle: DynamicObstacle, time_step: int,
-                           color: TUMcolor = TUMcolor.TUMblue):
+def draw_dyn_vehicle_shape(
+    rnd: MPRenderer,
+    obstacle: DynamicObstacle,
+    time_step: int,
+    color: TUMcolor = TUMcolor.TUMblue,
+):
     global zorder
     obs_shape = obstacle.occupancy_at_time(time_step).shape
     if isinstance(obs_shape, ShapeGroup):
         for shape_element in obs_shape.shapes:
             x, y = shape_element.shapely_object.exterior.xy
             rnd.ax.fill(x, y, alpha=0.5, fc=color, ec=None, zorder=zorder)
     else:
@@ -81,12 +97,18 @@
     rnd.draw_params.time_end = time_steps[-1]
     rnd.draw_params.trajectory.draw_trajectory = False
     rnd.draw_params.dynamic_obstacle.draw_icon = True
     scenario.draw(rnd)
     rnd.render()
     for obs in scenario.obstacles:
         if obs.prediction.final_time_step >= time_steps[-1]:
-            draw_state_list(rnd, obs.prediction.trajectory.state_list[time_steps[0]:time_steps[-1] + 1],
-                            color=TUMcolor.TUMblue, linewidth=5)
+            draw_state_list(
+                rnd,
+                obs.prediction.trajectory.state_list[
+                    time_steps[0] : time_steps[-1] + 1
+                ],
+                color=TUMcolor.TUMblue,
+                linewidth=5,
+            )
             for ts in time_steps[1:]:
                 draw_dyn_vehicle_shape(rnd, obs, ts, color=TUMcolor.TUMblue)
     plt.show()
```

### Comparing `commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/base/scenario_object.py` & `commonroad-openscenario-converter-0.1.0/osc_cr_converter/wrapper/base/scenario_object.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __author__ = "Michael Ratzel, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.0.1"
+__version__ = "0.1.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
-__status__ = "Pre-alpha"
+__status__ = "beta"
 
 from abc import abstractmethod
 from typing import Tuple, List, Type, Optional
 
 from commonroad.scenario.obstacle import ObstacleType
 from commonroad.scenario.trajectory import State
 from scenariogeneration.xosc import Vehicle
@@ -47,23 +47,30 @@
     """
     The baseclass for the scenario object states.
 
     For each time step in the final scenario one of these objects is created with the two closest
     SimScenarioObjectStates stored in _closest. Implementations of this class take care of interpolating the two
     SimScenarioObjectStates and creating a CommonRoad state out of it.
     """
+
     _closest: Tuple[SimScenarioObjectState, SimScenarioObjectState]
     _timestamp: float
     _dt1: float
     _dt2: float
     _obstacle_extra_info: Optional[Vehicle]
 
-    def __init__(self, timestamp: float, closest_states: Tuple[SimScenarioObjectState, SimScenarioObjectState],
-                 obstacle_extra_info: Optional[Vehicle]):
-        if abs(timestamp - closest_states[0].get_timestamp()) <= abs(timestamp - closest_states[1].get_timestamp()):
+    def __init__(
+        self,
+        timestamp: float,
+        closest_states: Tuple[SimScenarioObjectState, SimScenarioObjectState],
+        obstacle_extra_info: Optional[Vehicle],
+    ):
+        if abs(timestamp - closest_states[0].get_timestamp()) <= abs(
+            timestamp - closest_states[1].get_timestamp()
+        ):
             self._closest = (closest_states[0], closest_states[1])
         else:
             self._closest = (closest_states[1], closest_states[0])
 
         self._timestamp = timestamp
         self._dt1 = self._closest[1].get_timestamp() - self._closest[0].get_timestamp()
         self._dt2 = self.timestamp - self._closest[0].get_timestamp()
@@ -85,30 +92,37 @@
         return self._width
 
     @property
     def obstacle_type(self) -> ObstacleType:
         return self._obstacle_type
 
     @staticmethod
-    def build_interpolated(states: List[SimScenarioObjectState], timestamp: float,
-                           obstacle_extra_info: Optional[Vehicle]) -> "ScenarioObjectState":
+    def build_interpolated(
+        states: List[SimScenarioObjectState],
+        timestamp: float,
+        obstacle_extra_info: Optional[Vehicle],
+    ) -> "ScenarioObjectState":
         """
         Convenience function around _build_interpolated which utilizes
         SimScenarioObjectState.get_scenario_object_state_type() to enable inheritance
 
 
         :param states:List[SimScenarioObjectState]: All states as input
         :param timestamp:float: Specify the time at which the interpolated state should be created
         :param obstacle_extra_info:Optional[Vehicle]: Extra information about the Vehicle
         :return: The interpolated state of the object at a given timestamp
         """
         assert len(states) > 0
         if len(states) == 1:
-            return ScenarioObjectState.build_interpolated([states[0], states[0]], timestamp, obstacle_extra_info)
-        sorted_states = sorted(states, key=lambda state: abs(timestamp - state.timestamp))[:2]
+            return ScenarioObjectState.build_interpolated(
+                [states[0], states[0]], timestamp, obstacle_extra_info
+            )
+        sorted_states = sorted(
+            states, key=lambda state: abs(timestamp - state.timestamp)
+        )[:2]
         return states[0].get_scenario_object_state_type()(
             timestamp=timestamp,
             closest_states=(sorted_states[0], sorted_states[1]),
             obstacle_extra_info=obstacle_extra_info,
         )
 
     @abstractmethod
@@ -123,34 +137,55 @@
         """
         raise NotImplementedError
 
     def _get_interpolated(self, field_name: str):
         """
         Interpolate the value of field_name between the two closest states
         """
-        val0, val1, = (getattr(self._closest[0], field_name), getattr(self._closest[1], field_name))
+        (
+            val0,
+            val1,
+        ) = (
+            getattr(self._closest[0], field_name),
+            getattr(self._closest[1], field_name),
+        )
         gradient = (val1 - val0) / self._dt1
         return val0 + gradient * self._dt2
 
     def _get_equal(self, field_name: str):
         """
         Assert that the values of field_name match in both closest states and return the value
         """
-        val0, val1, = (getattr(self._closest[0], field_name), getattr(self._closest[1], field_name))
+        (
+            val0,
+            val1,
+        ) = (
+            getattr(self._closest[0], field_name),
+            getattr(self._closest[1], field_name),
+        )
         if val0 != val1:
-            raise ValueError("Failed interpolating new state, expected {}s to be equal: {}!={}"
-                             .format(field_name, val0, val1))
+            raise ValueError(
+                "Failed interpolating new state, expected {}s to be equal: {}!={}".format(
+                    field_name, val0, val1
+                )
+            )
         else:
             return val0
 
     def _get_closest(self, field_name: str):
         """
         Get the value of field_name of the closer of the two closest states
         """
         return getattr(self._closest[0], field_name)
 
     def _get_differentiate(self, field_name: str):
         """
         Get the rate of change of field_name between the two closest states
         """
-        val0, val1, = (getattr(self._closest[0], field_name), getattr(self._closest[1], field_name))
+        (
+            val0,
+            val1,
+        ) = (
+            getattr(self._closest[0], field_name),
+            getattr(self._closest[1], field_name),
+        )
         return (val1 - val0) / self._dt1
```

### Comparing `commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/base/sim_wrapper.py` & `commonroad-openscenario-converter-0.1.0/osc_cr_converter/wrapper/base/sim_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 __author__ = "Michael Ratzel, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.0.1"
+__version__ = "0.1.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
-__status__ = "Pre-alpha"
+__status__ = "beta"
 
 import warnings
-from typing import Optional,  Dict, List
+from typing import Optional, Dict, List
 from dataclasses import dataclass
 
 from commonroad.common.validity import is_real_number
 
 from osc_cr_converter.wrapper.base.ending_cause import ESimEndingCause
 from osc_cr_converter.wrapper.base.scenario_object import SimScenarioObjectState
 from osc_cr_converter.utility.configuration import ConverterParams, EsminiParams
@@ -23,38 +23,37 @@
     Dataclass to store the results of a wrapper simulation run
 
     Attributes
         ending_cause cause why the simulation ended
         states_per_vehicle List of simulation states per vehicle
         total_simulation_time total time simulated (Not execution time)
     """
+
     states: Dict[str, List[SimScenarioObjectState]]
     sim_time: float
     runtime: float
     ending_cause: ESimEndingCause
 
     @staticmethod
     def failure() -> "WrapperSimResult":
         """
         The failure function returns a WrapperSimResult with the ending cause set to FAILURE.
 
         :return: A wrappersimresult object
         """
         return WrapperSimResult(
-            ending_cause=ESimEndingCause.FAILURE,
-            states={},
-            sim_time=0.0,
-            runtime=0.0
+            ending_cause=ESimEndingCause.FAILURE, states={}, sim_time=0.0, runtime=0.0
         )
 
 
 class SimWrapper:
     """
     The base class of a ScenarioWrapper.
     """
+
     def __init__(self, config: ConverterParams):
         self.config = config
         self.max_time = config.esmini.max_time
 
     @property
     def max_time(self) -> float:
         """
@@ -65,42 +64,52 @@
     @max_time.setter
     def max_time(self, new_max_time: Optional[float]):
         if new_max_time is None:
             self._max_time = self.config.esmini.max_time
         elif is_real_number(new_max_time):
             self._max_time = new_max_time
         else:
-            warnings.warn(f"<EsminiWrapper/max_time> Tried to set to non real number value {new_max_time}.")
+            warnings.warn(
+                f"<EsminiWrapper/max_time> Tried to set to non real number value {new_max_time}."
+            )
 
     def simulate_scenario(self, scenario_path: str, sim_dt: float) -> WrapperSimResult:
         """
         Simulate a scenario and return its results
 
         :param scenario_path Path to the .xosc scenario file
         :param sim_dt delta time used for the simulation
         :return The WrapperSimResult
         """
         raise NotImplementedError
 
-    def view_scenario(self, scenario_path: str, window_size: Optional[EsminiParams.WindowSize] = None):
+    def view_scenario(
+        self, scenario_path: str, window_size: Optional[EsminiParams.WindowSize] = None
+    ):
         """
         Render a XOSC file
 
         :param scenario_path Path to the .xosc scenario file
         :param window_size Wanted size of the rendering window
         """
         warnings.warn(f"{self.__class__} did not implement to view scenario")
 
-    def render_scenario_to_gif(self, scenario_path: str, gif_file_path: str, fps: int = 30,
-                               gif_size: Optional[EsminiParams.WindowSize] = None) -> bool:
+    def render_scenario_to_gif(
+        self,
+        scenario_path: str,
+        gif_file_path: str,
+        fps: int = 30,
+        gif_size: Optional[EsminiParams.WindowSize] = None,
+    ) -> bool:
         """
         Create a gif of an XOSC file.
 
         :param scenario_path Path to the .xosc scenario file
         :param gif_file_path Path to the .gif product
         :param fps Frames per second of the gif
         :param gif_size Size of the gif
         :return Returns if gif creation was successful
         """
-        warnings.warn(f"{self.__class__} did not implement to render a scenario to a gif")
+        warnings.warn(
+            f"{self.__class__} did not implement to render a scenario to a gif"
+        )
         return False
-
```

### Comparing `commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/esmini/esmini_scenario_object.py` & `commonroad-openscenario-converter-0.1.0/osc_cr_converter/wrapper/esmini/esmini_scenario_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 __author__ = "Michael Ratzel, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.0.1"
+__version__ = "0.1.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
-__status__ = "Pre-alpha"
+__status__ = "beta"
 
 import ctypes as ct
 from typing import Type
 
 import numpy as np
 from commonroad.scenario.obstacle import ObstacleType
 from commonroad.scenario.state import CustomState
 
-from osc_cr_converter.wrapper.base.scenario_object import ScenarioObjectState, SimScenarioObjectState
+from osc_cr_converter.wrapper.base.scenario_object import (
+    ScenarioObjectState,
+    SimScenarioObjectState,
+)
 
 
 class SEStruct(ct.Structure, SimScenarioObjectState):
     """
     Implementation of the SimScenarioObjectState ABC. Objects of this will be recorded while running the simulation
     """
+
     _fields_ = [
         ("id", ct.c_int),
         ("model_id", ct.c_int),
         ("control", ct.c_int),
         ("timestamp", ct.c_float),
         ("x", ct.c_float),
         ("y", ct.c_float),
@@ -43,15 +47,15 @@
         ("centerOffsetZ", ct.c_float),
         ("width", ct.c_float),
         ("length", ct.c_float),
         ("height", ct.c_float),
         ("objectType", ct.c_int),
         ("objectCategory", ct.c_int),
         ("wheel_angle", ct.c_float),
-        ("wheel_rotation", ct.c_float)
+        ("wheel_rotation", ct.c_float),
     ]
 
     def get_scenario_object_state_type(self) -> "Type[ScenarioObjectState]":
         return EsminiScenarioObjectState
 
     def get_timestamp(self) -> float:
         return self.timestamp
@@ -108,14 +112,15 @@
             return ObstacleType.UNKNOWN
 
 
 class EsminiScenarioObjectState(ScenarioObjectState):
     """
     Class that converts from SEStructs to CommonRoad states
     """
+
     @property
     def id(self) -> int:
         if not hasattr(self, "_id"):
             self._id = self._get_equal("id")
         return self._id
 
     @property
@@ -285,29 +290,29 @@
         return self._height
 
     def to_cr_state(self, time_step: int) -> CustomState:
         c_h, s_h = np.cos(self.h), np.sin(self.h)  # heading
         c_p, s_p = np.cos(self.p), np.sin(self.p)  # pitch
         c_r, s_r = np.cos(self.r), np.sin(self.r)  # roll
 
-        center = np.array((
-            self.x,
-            self.y,
-            self.z
-        ))
-        rotation_matrix = np.array((
-            (c_h * c_p, c_h * s_p * s_r - s_h * c_r, c_h * s_p * c_r + s_h * s_r),
-            (s_h * c_p, s_h * s_p * s_r + c_h * c_r, s_h * s_p * s_r - c_h * s_r),
-            (-s_p, c_p * s_r, c_p * c_r),
-        ))
-        offset = np.array((
-            self.center_offset_x,
-            self.center_offset_y,
-            self.center_offset_z,
-        ))
+        center = np.array((self.x, self.y, self.z))
+        rotation_matrix = np.array(
+            (
+                (c_h * c_p, c_h * s_p * s_r - s_h * c_r, c_h * s_p * c_r + s_h * s_r),
+                (s_h * c_p, s_h * s_p * s_r + c_h * c_r, s_h * s_p * s_r - c_h * s_r),
+                (-s_p, c_p * s_r, c_p * c_r),
+            )
+        )
+        offset = np.array(
+            (
+                self.center_offset_x,
+                self.center_offset_y,
+                self.center_offset_z,
+            )
+        )
         position_3d = center + np.matmul(rotation_matrix, offset)
         return CustomState(
             time_step=time_step,
             position=position_3d[0:2],
             orientation=self.h,
             velocity=self.speed,
             steering_angle=self.steering_angle,
```

### Comparing `commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/esmini/esmini_wrapper.py` & `commonroad-openscenario-converter-0.1.0/osc_cr_converter/wrapper/esmini/esmini_wrapper.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 __author__ = "Michael Ratzel, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.0.4"
+__version__ = "0.1.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
-__status__ = "Pre-alpha"
+__status__ = "beta"
 
 import ctypes as ct
 import logging
 import math
 import os.path
 import re
 import time
-from datetime import datetime
 import warnings
 from multiprocessing import Lock
 from os import path
 from sys import platform
 from typing import Optional, List, Dict, Union
 
 import imageio
 
 from osc_cr_converter.wrapper.base.ending_cause import ESimEndingCause
 from osc_cr_converter.wrapper.esmini.esmini_scenario_object import SEStruct
-from osc_cr_converter.wrapper.esmini.storyboard_element import EStoryBoardElementState, \
-    EStoryBoardElementLevel, StoryBoardElement
+from osc_cr_converter.wrapper.esmini.storyboard_element import (
+    EStoryBoardElementState,
+    EStoryBoardElementLevel,
+    StoryBoardElement,
+)
 from osc_cr_converter.wrapper.base.sim_wrapper import SimWrapper, WrapperSimResult
 from osc_cr_converter.utility.configuration import ConverterParams, EsminiParams
 
 
 class EsminiWrapper(SimWrapper):
     """
     The implementation of the SimWrapper to simulate, render to gif, and view scenarios in a window based in the
     Environment Simulator Minimalistic (esmini).
 
     Due to the possible usage of udp sockets this wrapper will only run sequential which is enforced by the __lock.
     """
+
     __lock: Lock = Lock()
 
     _all_sim_elements: Dict[StoryBoardElement, EStoryBoardElementState]
 
     _scenario_engine_initialized: bool
     _first_frame_run: bool
 
@@ -86,34 +89,46 @@
         Path to the esmini lib bin directory path: "path/to/esmini/bin"
         """
         return self._esmini_lib_bin_path_
 
     @_esmini_lib_bin_path.setter
     def _esmini_lib_bin_path(self, new_esmini_lib_bin_path: str):
         if hasattr(self, "_esmini_lib"):
-            warnings.warn("<EsminiWrapper/esmini_lib> EsminiLib ctypes object is immutable")
+            warnings.warn(
+                "<EsminiWrapper/esmini_lib> EsminiLib ctypes object is immutable"
+            )
         elif path.exists(new_esmini_lib_bin_path):
             self._esmini_lib_bin_path_ = new_esmini_lib_bin_path
             if platform.startswith("linux"):
-                self._esmini_lib = ct.CDLL(path.join(new_esmini_lib_bin_path, "libesminiLib.so"))
+                self._esmini_lib = ct.CDLL(
+                    path.join(new_esmini_lib_bin_path, "libesminiLib.so")
+                )
             elif platform.startswith("darwin"):
-                self._esmini_lib = ct.CDLL(path.join(new_esmini_lib_bin_path, "libesminiLib.dylib"))
+                self._esmini_lib = ct.CDLL(
+                    path.join(new_esmini_lib_bin_path, "libesminiLib.dylib")
+                )
             elif platform.startswith("win32"):
-                self._esmini_lib = ct.CDLL(path.join(new_esmini_lib_bin_path, "esminiLib.dll"))
+                self._esmini_lib = ct.CDLL(
+                    path.join(new_esmini_lib_bin_path, "esminiLib.dll")
+                )
             else:
-                warnings.warn(f"<EsminiWrapper/esmini_lib> Unsupported platform: {platform}")
+                warnings.warn(
+                    f"<EsminiWrapper/esmini_lib> Unsupported platform: {platform}"
+                )
                 return
 
             self._esmini_lib.SE_StepDT.argtypes = [ct.c_float]
             self._esmini_lib.SE_GetSimulationTime.restype = ct.c_float
             self._esmini_lib.SE_SetSeed.argtypes = [ct.c_uint]
             self._esmini_lib.SE_GetObjectName.restype = ct.c_char_p
 
         else:
-            warnings.warn(f"<EsminiWrapper/esmini_lib> Path {new_esmini_lib_bin_path} does not exist")
+            warnings.warn(
+                f"<EsminiWrapper/esmini_lib> Path {new_esmini_lib_bin_path} does not exist"
+            )
 
     @property
     def random_seed(self) -> int:
         """
         Run the simulation using this random seed, default is 0
         """
         return self._random_seed
@@ -148,18 +163,24 @@
 
     @log_to_file.setter
     def log_to_file(self, new_log_to_file: Union[None, bool, str]):
         if new_log_to_file is None:
             self._log_to_file = None
         elif isinstance(new_log_to_file, bool):
             if new_log_to_file:
-                log_dir = os.path.dirname(os.path.realpath(__file__)) + "/../../../output/log"
-                os.makedirs(log_dir, exist_ok=True)  # create directory if it doesn't exist
-                self._log_to_file = os.path.join(self.config.general.path_output_log,
-                                                 f"esmini_{self.config.general.string_date_time}.log")
+                log_dir = (
+                    os.path.dirname(os.path.realpath(__file__)) + "/../../../output/log"
+                )
+                os.makedirs(
+                    log_dir, exist_ok=True
+                )  # create directory if it doesn't exist
+                self._log_to_file = os.path.join(
+                    self.config.general.path_output_log,
+                    f"esmini_{self.config.general.string_date_time}.log",
+                )
             else:
                 self._log_to_file = None
 
     def __getstate__(self):
         state = self.__dict__.copy()
         del state["_esmini_lib"]
 
@@ -173,119 +194,161 @@
     def __setstate__(self, state):
         self.__dict__.update(state)
         self._esmini_lib_bin_path = state["_esmini_lib_bin_path_"]
         self._reset()
 
     def simulate_scenario(self, scenario_path: str, sim_dt: float) -> WrapperSimResult:
         with EsminiWrapper.__lock:
-            if not self._initialize_scenario_engine(scenario_path, viewer_mode=0, use_threading=False):
-                warnings.warn("<EsminiWrapper/simulate_scenario> Failed to initialize scenario engine")
+            if not self._initialize_scenario_engine(
+                scenario_path, viewer_mode=0, use_threading=False
+            ):
+                warnings.warn(
+                    "<EsminiWrapper/simulate_scenario> Failed to initialize scenario engine"
+                )
                 return WrapperSimResult.failure()
             sim_time = 0.0
             runtime_start = time.time()
             all_states: Dict[int, List[SEStruct]]
-            all_states = {object_id: [state] for object_id, state in self._get_scenario_object_states().items()}
+            all_states = {
+                object_id: [state]
+                for object_id, state in self._get_scenario_object_states().items()
+            }
             while (cause := self._sim_finished()) is None:
                 self._sim_step(sim_dt)
                 sim_time += sim_dt
                 for object_id, new_state in self._get_scenario_object_states().items():
                     if object_id not in all_states:
                         all_states[object_id] = [new_state]
-                    elif math.isclose(new_state.timestamp, all_states[object_id][-1].timestamp):
+                    elif math.isclose(
+                        new_state.timestamp, all_states[object_id][-1].timestamp
+                    ):
                         all_states[object_id][-1] = new_state
                     else:
                         all_states[object_id].append(new_state)
             runtime = time.time() - runtime_start
             return WrapperSimResult(
-                states={self._get_scenario_object_name(object_id): states for object_id, states in
-                        all_states.items()},
+                states={
+                    self._get_scenario_object_name(object_id): states
+                    for object_id, states in all_states.items()
+                },
                 sim_time=sim_time,
                 runtime=runtime,
-                ending_cause=cause
+                ending_cause=cause,
             )
 
-    def view_scenario(self, scenario_path: str, window_size: Optional[EsminiParams.WindowSize] = None):
+    def view_scenario(
+        self, scenario_path: str, window_size: Optional[EsminiParams.WindowSize] = None
+    ):
         with EsminiWrapper.__lock:
-            if not self._initialize_scenario_engine(scenario_path, viewer_mode=1, use_threading=True):
-                warnings.warn("<EsminiWrapper/view_scenario> Failed to initialize scenario engine")
+            if not self._initialize_scenario_engine(
+                scenario_path, viewer_mode=1, use_threading=True
+            ):
+                warnings.warn(
+                    "<EsminiWrapper/view_scenario> Failed to initialize scenario engine"
+                )
                 return
             if window_size is not None:
                 self._set_set_window_size(window_size)
             while self._sim_finished() is None:
                 self._sim_step(None)
             self._close_scenario_engine()
 
-    def render_scenario_to_gif(self, scenario_path: str, gif_file_path: str, fps: int = 30,
-                               window_size: Optional[EsminiParams.WindowSize] = None) -> bool:
+    def render_scenario_to_gif(
+        self,
+        scenario_path: str,
+        gif_file_path: str,
+        fps: int = 30,
+        window_size: Optional[EsminiParams.WindowSize] = None,
+    ) -> bool:
         with EsminiWrapper.__lock:
-            if not self._initialize_scenario_engine(scenario_path, viewer_mode=7, use_threading=False):
-                warnings.warn("<EsminiWrapper/render_scenario_to_gif> Failed to initialize scenario engine")
+            if not self._initialize_scenario_engine(
+                scenario_path, viewer_mode=7, use_threading=False
+            ):
+                warnings.warn(
+                    "<EsminiWrapper/render_scenario_to_gif> Failed to initialize scenario engine"
+                )
                 return False
             if window_size is not None:
                 self._set_set_window_size(window_size)
             image_regex = re.compile(r"screen_shot_\d{5,}\.tga")
-            ignored_images = set([p for p in os.listdir(".") if image_regex.match(p) is not None])
+            ignored_images = set(
+                [p for p in os.listdir(".") if image_regex.match(p) is not None]
+            )
             while self._sim_finished() is None:
                 self._sim_step(1 / fps)
             self._close_scenario_engine()
             images = sorted(
-                [p for p in os.listdir(".") if image_regex.match(p) is not None and p not in ignored_images])
+                [
+                    p
+                    for p in os.listdir(".")
+                    if image_regex.match(p) is not None and p not in ignored_images
+                ]
+            )
             with imageio.get_writer(gif_file_path, mode="I", fps=fps) as writer:
                 for image in images:
                     writer.append_data(imageio.v3.imread(image))
                     os.remove(image)
             return True
 
     def _reset(self):
         self._all_sim_elements = {}
         self._scenario_engine_initialized = False
         self._first_frame_run = False
         self._callback_functor = None
         self._sim_end_detected_time = None
 
-    def _initialize_scenario_engine(self, scenario_path: str, viewer_mode: int, use_threading: bool) -> bool:
+    def _initialize_scenario_engine(
+        self, scenario_path: str, viewer_mode: int, use_threading: bool
+    ) -> bool:
         self._reset()
 
         self.esmini_lib.SE_LogToConsole(self.log_to_console)
         if self.log_to_file is None:
             self.esmini_lib.SE_SetLogFilePath("".encode("ASCII"))
         else:
             self.esmini_lib.SE_SetLogFilePath(self.log_to_file.encode("ASCII"))
 
         ret = self.esmini_lib.SE_Init(
             scenario_path.encode("ASCII"),
             int(0),
             int(viewer_mode),
             int(use_threading),
-            int(0)
+            int(0),
         )
         if ret != 0:
             return False
 
         self.esmini_lib.SE_SetSeed(self.random_seed)
 
         self.esmini_lib.SE_OpenOSISocket("127.0.0.1")
 
-        self._callback_functor = ct.CFUNCTYPE(None, ct.c_char_p, ct.c_int, ct.c_int)(self.__state_change_callback)
-        self.esmini_lib.SE_RegisterStoryBoardElementStateChangeCallback(self._callback_functor)
+        self._callback_functor = ct.CFUNCTYPE(None, ct.c_char_p, ct.c_int, ct.c_int)(
+            self.__state_change_callback
+        )
+        self.esmini_lib.SE_RegisterStoryBoardElementStateChangeCallback(
+            self._callback_functor
+        )
         self._scenario_engine_initialized = True
         return True
 
     def _set_set_window_size(self, window_size: EsminiParams.WindowSize):
-        self.esmini_lib.SE_SetWindowPosAndSize(window_size.x, window_size.y, window_size.width, window_size.height)
+        self.esmini_lib.SE_SetWindowPosAndSize(
+            window_size.x, window_size.y, window_size.width, window_size.height
+        )
 
     def _close_scenario_engine(self):
         if not self._scenario_engine_initialized:
             raise RuntimeError("Scenario Engine not initialized")
         self.esmini_lib.SE_Close()
         self._scenario_engine_initialized = False
 
     def __state_change_callback(self, name: bytes, element_type: int, state: int):
-        self._all_sim_elements[StoryBoardElement(name, EStoryBoardElementLevel(element_type))] = EStoryBoardElementState(
-            state)
+        self._all_sim_elements[
+            StoryBoardElement(name, EStoryBoardElementLevel(element_type))
+        ] = EStoryBoardElementState(state)
 
     def _sim_step(self, dt: Optional[float]):
         if not self._scenario_engine_initialized:
             raise RuntimeError("Scenario Engine not initialized")
         self._first_frame_run = True
 
         if dt is not None:
@@ -296,34 +359,42 @@
     def _sim_finished(self) -> Optional[ESimEndingCause]:
         if not self._scenario_engine_initialized:
             return None
         if not self._first_frame_run:
             return None
         now = self.esmini_lib.SE_GetSimulationTime()
         if self.esmini_lib.SE_GetQuitFlag() == 1:
-            self._log("{:.3f}: esmini requested quitting -> Scenario finished completely ".format(now))
+            self._log(
+                "{:.3f}: esmini requested quitting -> Scenario finished completely ".format(
+                    now
+                )
+            )
             return ESimEndingCause.SCENARIO_FINISHED_BY_SIMULATOR
         if now >= self.max_time:
             self._log("{:.3f}: Max Execution time reached ".format(now))
             return ESimEndingCause.MAX_TIME_REACHED
         return None
 
     def _get_scenario_object_states(self) -> Optional[Dict[int, SEStruct]]:
         if not self._scenario_engine_initialized:
             raise RuntimeError("Scenario Engine not initialized")
         try:
             objects = {}
             for j in range(self.esmini_lib.SE_GetNumberOfObjects()):
                 object_id = self.esmini_lib.SE_GetId(j)
                 objects[object_id] = SEStruct()
-                self.esmini_lib.SE_GetObjectState(object_id, ct.byref(objects[object_id]))
+                self.esmini_lib.SE_GetObjectState(
+                    object_id, ct.byref(objects[object_id])
+                )
 
             return objects
         except Exception as e:
-            logging.warning("Unexpected exception during scenario object extraction: {}".format(e))
+            logging.warning(
+                "Unexpected exception during scenario object extraction: {}".format(e)
+            )
             return None
 
     def _get_scenario_object_name(self, object_id: int) -> Optional[str]:
         raw_name: bytes = self.esmini_lib.SE_GetObjectName(object_id)
         return f"no-name-{object_id}" if raw_name is None else raw_name.decode("utf-8")
 
     def _log(self, text: str):
```

### Comparing `commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/esmini/esmini_wrapper_provider.py` & `commonroad-openscenario-converter-0.1.0/osc_cr_converter/wrapper/esmini/esmini_wrapper_provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __author__ = "Michael Ratzel, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.0.1"
+__version__ = "0.1.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
-__status__ = "Pre-alpha"
+__status__ = "beta"
 
 import os
 import re
 import sys
 import warnings
 from io import BytesIO
 from os import path
@@ -24,14 +24,15 @@
 class EsminiWrapperProvider:
 
     """
     This class downloads the wanted esmini version from GitHub and creates an EsminiWrapper from it.
 
     It works on Mac Windows and Linux
     """
+
     def __init__(self, config: ConverterParams):
         self.storage_prefix = None
         self.preferred_version = config.esmini.version
         self.config = config
 
     @property
     def storage_prefix(self) -> str:
@@ -43,15 +44,17 @@
     @storage_prefix.setter
     def storage_prefix(self, new_path_prefix: Optional[str]):
         if new_path_prefix is None:
             self._path_prefix = path.abspath(path.dirname(__file__))
         elif path.exists(new_path_prefix):
             self._path_prefix = new_path_prefix
         else:
-            warnings.warn(f"<EsminiWrapperProvider/storage_prefix> Path not found {new_path_prefix}")
+            warnings.warn(
+                f"<EsminiWrapperProvider/storage_prefix> Path not found {new_path_prefix}"
+            )
 
     @property
     def preferred_version(self) -> Optional[str]:
         """
         The Preferred version of esmini with v2.29.3 being the default, as this is the latest tested version
         """
         return self._preferred_version
@@ -63,36 +66,50 @@
             self._preferred_version = None
         elif new_preferred_version.lower() == "default":
             self._preferred_version = "v2.29.3"
         elif r.fullmatch(new_preferred_version) is not None:
             self._preferred_version = new_preferred_version
         else:
             warnings.warn(
-                f"<EsminiWrapperProvider/preferred_version> New version {new_preferred_version} not match {r.pattern}")
+                f"<EsminiWrapperProvider/preferred_version> New version {new_preferred_version} not match {r.pattern}"
+            )
 
     def provide_esmini_wrapper(self) -> Optional[EsminiWrapper]:
         if self.preferred_version is not None:
             if self._try_loading_version(self.preferred_version):
-                return EsminiWrapper(self._bin_path(self._esmini_path(self.preferred_version)), self.config)
+                return EsminiWrapper(
+                    self._bin_path(self._esmini_path(self.preferred_version)),
+                    self.config,
+                )
             else:
-                print("Failed loading specified esmini version: {}".format(self.preferred_version))
+                print(
+                    "Failed loading specified esmini version: {}".format(
+                        self.preferred_version
+                    )
+                )
                 quit()
 
         try:
-            r = requests.get('https://github.com/esmini/esmini/releases/latest')
+            r = requests.get("https://github.com/esmini/esmini/releases/latest")
             version = r.url.split("/")[-1]
             if self._try_loading_version(version):
-                return EsminiWrapper(self._bin_path(self._esmini_path(version)), self.config)
+                return EsminiWrapper(
+                    self._bin_path(self._esmini_path(version)), self.config
+                )
         except requests.exceptions.ConnectionError:
             pass
 
-        available_versions = sorted([
-            dir_path for dir_path in os.listdir(self.storage_prefix)
-            if re.match(self._esmini_path(""), dir_path) and os.path.exists(self._bin_path(dir_path))
-        ])
+        available_versions = sorted(
+            [
+                dir_path
+                for dir_path in os.listdir(self.storage_prefix)
+                if re.match(self._esmini_path(""), dir_path)
+                and os.path.exists(self._bin_path(dir_path))
+            ]
+        )
 
         if len(available_versions) > 0:
             return EsminiWrapper(self._bin_path(available_versions[-1]), self.config)
 
         return None
 
     def _try_loading_version(self, version: str) -> bool:
@@ -118,13 +135,21 @@
             archive_name = "esmini-bin_mac_catalina.zip"
         elif sys.platform.startswith("win32"):
             archive_name = "esmini-bin_win_x64.zip"
         else:
             print("Unsupported platform: {}".format(sys.platform))
             quit()
         try:
-            r = requests.get("/".join(["https://github.com/esmini/esmini/releases/download", version, archive_name]))
+            r = requests.get(
+                "/".join(
+                    [
+                        "https://github.com/esmini/esmini/releases/download",
+                        version,
+                        archive_name,
+                    ]
+                )
+            )
             with ZipFile(BytesIO(r.content), "r") as zipObj:
                 zipObj.extractall(self._abs_path(self._esmini_path(version)))
         except requests.exceptions.ConnectionError:
             return False
         return True
```

### Comparing `commonroad-openscenario-converter-0.0.4/osc_cr_converter/wrapper/esmini/storyboard_element.py` & `commonroad-openscenario-converter-0.1.0/osc_cr_converter/wrapper/esmini/storyboard_element.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,52 @@
 __author__ = "Michael Ratzel, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.0.1"
+__version__ = "0.1.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
-__status__ = "Pre-alpha"
+__status__ = "beta"
 
 from dataclasses import dataclass
 from enum import IntEnum
 
 
 class EStoryBoardElementLevel(IntEnum):
     """
     Levels of the storyboard elements
     """
+
     STORY = 1
     ACT = 2
     MANEUVER_GROUP = 3
     MANEUVER = 4
     EVENT = 5
     ACTION = 6
     UNDEFINED_ELEMENT_TYPE = 0
 
 
 class EStoryBoardElementState(IntEnum):
     """
     State of the storyboard elements
     """
+
     STANDBY = 1
     RUNNING = 2
     COMPLETE = 3
     UNDEFINED_ELEMENT_STATE = 0
 
 
 @dataclass(frozen=True)
 class StoryBoardElement:
     """
     A storyboard element
     """
+
     name: bytes
     element_type: EStoryBoardElementLevel
 
     def __eq__(self, o: object) -> bool:
-        return isinstance(o, StoryBoardElement) and self.name == o.name and self.element_type == o.element_type
+        return (
+            isinstance(o, StoryBoardElement)
+            and self.name == o.name
+            and self.element_type == o.element_type
+        )
```

### Comparing `commonroad-openscenario-converter-0.0.4/tests/test_conversion.py` & `commonroad-openscenario-converter-0.1.0/tests/test_conversion.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 
     def setUp(self) -> None:
         super().setUp()
         config = ConverterParams()
         self.converter = Osc2CrConverter(config)
 
     def load_and_convert_openscenario(self, file_name: str) -> Scenario:
-        source_file = os.path.dirname(os.path.realpath(__file__)) + "/../scenarios/" + file_name
+        source_file = (
+            os.path.dirname(os.path.realpath(__file__)) + "/../scenarios/" + file_name
+        )
         return self.converter.run_conversion(source_file)
 
     def test_pedestrian_collision(self):
         name = "from_esmini/xosc/pedestrian_collision.xosc"
         scenario = self.load_and_convert_openscenario(name)
 
         # check whether the conversion is successfully done or not
@@ -44,8 +46,7 @@
 
         # test map conversion
         self.assertIsInstance(scenario.lanelet_network, LaneletNetwork)
 
         # test nr of obstacles
         self.assertEqual(len(scenario.dynamic_obstacles), 2)
         self.assertEqual(len(scenario.static_obstacles), 0)
-
```

