# Comparing `tmp/qtaf-5.6.7.tar.gz` & `tmp/qtaf-5.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtaf-5.6.7.tar", last modified: Mon Jul 24 03:56:17 2023, max compression
+gzip compressed data, was "qtaf-5.6.8.tar", last modified: Tue Jul 25 10:52:07 2023, max compression
```

## Comparing `qtaf-5.6.7.tar` & `qtaf-5.6.8.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:56:17.767449 qtaf-5.6.7/
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-24 03:56:06.000000 qtaf-5.6.7/LICENSE.TXT
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-24 03:56:06.000000 qtaf-5.6.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-07-24 03:56:17.767449 qtaf-5.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-24 03:56:06.000000 qtaf-5.6.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-24 03:56:06.000000 qtaf-5.6.7/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:56:17.759449 qtaf-5.6.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-24 03:56:06.000000 qtaf-5.6.7/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-24 03:56:06.000000 qtaf-5.6.7/qta-manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:56:17.759449 qtaf-5.6.7/qta_statics/
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-24 03:56:06.000000 qtaf-5.6.7/qta_statics/TestReport.xsl
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-24 03:56:06.000000 qtaf-5.6.7/qta_statics/TestResult.xsl
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 03:56:06.000000 qtaf-5.6.7/qta_statics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1968182 2023-07-24 03:56:06.000000 qtaf-5.6.7/qta_statics/qta-report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:56:17.763449 qtaf-5.6.7/qtaf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-07-24 03:56:17.000000 qtaf-5.6.7/qtaf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-24 03:56:17.000000 qtaf-5.6.7/qtaf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 03:56:17.000000 qtaf-5.6.7/qtaf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 03:56:17.000000 qtaf-5.6.7/qtaf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 03:56:17.000000 qtaf-5.6.7/qtaf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-24 03:56:17.000000 qtaf-5.6.7/qtaf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-24 03:56:06.000000 qtaf-5.6.7/qtaf_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-24 03:56:06.000000 qtaf-5.6.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 03:56:17.767449 qtaf-5.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-24 03:56:06.000000 qtaf-5.6.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:56:17.767449 qtaf-5.6.7/testbase/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27311 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/datadrive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/exlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    15550 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    34147 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/management.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    35792 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/report.py
--rw-r--r--   0 runner    (1001) docker     (123)    24595 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    44877 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    45863 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/testcase.py
--rw-r--r--   0 runner    (1001) docker     (123)    29712 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/testresult.py
--rw-r--r--   0 runner    (1001) docker     (123)    16556 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/testsuite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    26680 2023-07-24 03:56:06.000000 qtaf-5.6.7/testbase/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 03:56:17.000000 qtaf-5.6.7/testbase/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:56:17.767449 qtaf-5.6.7/tuia/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/_tif.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/accessible.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/filedialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/gfcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/mouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/qpath.py
--rw-r--r--   0 runner    (1001) docker     (123)    16430 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/qpathparser.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/remoteprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/testcase.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/uiacontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/webcontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/wincontrols.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-24 03:56:06.000000 qtaf-5.6.7/tuia/wintypes.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 03:56:16.000000 qtaf-5.6.7/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:52:07.970141 qtaf-5.6.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-25 10:51:56.000000 qtaf-5.6.8/LICENSE.TXT
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-25 10:51:56.000000 qtaf-5.6.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-07-25 10:52:07.970141 qtaf-5.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-25 10:51:56.000000 qtaf-5.6.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-25 10:51:56.000000 qtaf-5.6.8/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:52:07.962141 qtaf-5.6.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-25 10:51:56.000000 qtaf-5.6.8/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-25 10:51:56.000000 qtaf-5.6.8/qta-manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:52:07.962141 qtaf-5.6.8/qta_statics/
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-25 10:51:56.000000 qtaf-5.6.8/qta_statics/TestReport.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-25 10:51:56.000000 qtaf-5.6.8/qta_statics/TestResult.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 10:51:56.000000 qtaf-5.6.8/qta_statics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1968182 2023-07-25 10:51:56.000000 qtaf-5.6.8/qta_statics/qta-report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:52:07.966141 qtaf-5.6.8/qtaf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-07-25 10:52:07.000000 qtaf-5.6.8/qtaf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-25 10:52:07.000000 qtaf-5.6.8/qtaf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 10:52:07.000000 qtaf-5.6.8/qtaf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-25 10:52:07.000000 qtaf-5.6.8/qtaf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 10:52:07.000000 qtaf-5.6.8/qtaf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-25 10:52:07.000000 qtaf-5.6.8/qtaf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-25 10:51:56.000000 qtaf-5.6.8/qtaf_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-25 10:51:56.000000 qtaf-5.6.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 10:52:07.970141 qtaf-5.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-25 10:51:56.000000 qtaf-5.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:52:07.966141 qtaf-5.6.8/testbase/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-25 10:51:56.000000 qtaf-5.6.8/testbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27697 2023-07-25 10:51:56.000000 qtaf-5.6.8/testbase/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-07-25 10:51:56.000000 qtaf-5.6.8/testbase/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-25 10:51:56.000000 qtaf-5.6.8/testbase/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-25 10:51:56.000000 qtaf-5.6.8/testbase/datadrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-07-25 10:51:56.000000 qtaf-5.6.8/testbase/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-07-25 10:51:56.000000 qtaf-5.6.8/testbase/exlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15730 2023-07-25 10:51:56.000000 qtaf-5.6.8/testbase/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-07-25 10:51:56.000000 qtaf-5.6.8/testbase/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34147 2023-07-25 10:51:56.000000 qtaf-5.6.8/testbase/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-25 10:51:56.000000 qtaf-5.6.8/testbase/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-07-25 10:51:56.000000 qtaf-5.6.8/testbase/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35792 2023-07-25 10:51:56.000000 qtaf-5.6.8/testbase/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24595 2023-07-25 10:51:56.000000 qtaf-5.6.8/testbase/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-25 10:51:56.000000 qtaf-5.6.8/testbase/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44877 2023-07-25 10:51:56.000000 qtaf-5.6.8/testbase/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-25 10:51:56.000000 qtaf-5.6.8/testbase/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-25 10:51:56.000000 qtaf-5.6.8/testbase/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45863 2023-07-25 10:51:56.000000 qtaf-5.6.8/testbase/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29712 2023-07-25 10:51:56.000000 qtaf-5.6.8/testbase/testresult.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16556 2023-07-25 10:51:56.000000 qtaf-5.6.8/testbase/testsuite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-25 10:51:56.000000 qtaf-5.6.8/testbase/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26680 2023-07-25 10:51:56.000000 qtaf-5.6.8/testbase/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-25 10:52:07.000000 qtaf-5.6.8/testbase/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:52:07.970141 qtaf-5.6.8/tuia/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-25 10:51:56.000000 qtaf-5.6.8/tuia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-25 10:51:56.000000 qtaf-5.6.8/tuia/_tif.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-25 10:51:56.000000 qtaf-5.6.8/tuia/accessible.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-25 10:51:56.000000 qtaf-5.6.8/tuia/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-25 10:51:56.000000 qtaf-5.6.8/tuia/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-25 10:51:56.000000 qtaf-5.6.8/tuia/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-25 10:51:56.000000 qtaf-5.6.8/tuia/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-25 10:51:56.000000 qtaf-5.6.8/tuia/filedialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-25 10:51:56.000000 qtaf-5.6.8/tuia/gfcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-25 10:51:56.000000 qtaf-5.6.8/tuia/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-25 10:51:56.000000 qtaf-5.6.8/tuia/mouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-25 10:51:56.000000 qtaf-5.6.8/tuia/qpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16430 2023-07-25 10:51:56.000000 qtaf-5.6.8/tuia/qpathparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-25 10:51:56.000000 qtaf-5.6.8/tuia/remoteprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-25 10:51:56.000000 qtaf-5.6.8/tuia/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-25 10:51:56.000000 qtaf-5.6.8/tuia/uiacontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-25 10:51:56.000000 qtaf-5.6.8/tuia/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-25 10:51:56.000000 qtaf-5.6.8/tuia/webcontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-25 10:51:56.000000 qtaf-5.6.8/tuia/wincontrols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-25 10:51:56.000000 qtaf-5.6.8/tuia/wintypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 10:52:06.000000 qtaf-5.6.8/version.txt
```

### Comparing `qtaf-5.6.7/LICENSE.TXT` & `qtaf-5.6.8/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/PKG-INFO` & `qtaf-5.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtaf
-Version: 5.6.7
+Version: 5.6.8
 Summary: Basic test automation framework for QTA
 Home-page: https://github.com/Tencent/QTAF
 Author: Tencent
 License: Copyright(c)2010-2018 Tencent All Rights Reserved. 
 Project-URL: TestBase Documentation, https://qta-testbase.readthedocs.io/zh/latest/
 Project-URL: TUIA Documentation, https://qta-tuia.readthedocs.io/zh/latest/
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `qtaf-5.6.7/README.md` & `qtaf-5.6.8/README.md`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/__main__.py` & `qtaf-5.6.8/__main__.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/qta-manage.py` & `qtaf-5.6.8/qta-manage.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/qta_statics/TestReport.xsl` & `qtaf-5.6.8/qta_statics/TestReport.xsl`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/qta_statics/TestResult.xsl` & `qtaf-5.6.8/qta_statics/TestResult.xsl`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/qta_statics/qta-report.html` & `qtaf-5.6.8/qta_statics/qta-report.html`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/qtaf.egg-info/PKG-INFO` & `qtaf-5.6.8/qtaf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtaf
-Version: 5.6.7
+Version: 5.6.8
 Summary: Basic test automation framework for QTA
 Home-page: https://github.com/Tencent/QTAF
 Author: Tencent
 License: Copyright(c)2010-2018 Tencent All Rights Reserved. 
 Project-URL: TestBase Documentation, https://qta-testbase.readthedocs.io/zh/latest/
 Project-URL: TUIA Documentation, https://qta-tuia.readthedocs.io/zh/latest/
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `qtaf-5.6.7/qtaf.egg-info/SOURCES.txt` & `qtaf-5.6.8/qtaf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/qtaf_settings.py` & `qtaf-5.6.8/qtaf_settings.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/setup.py` & `qtaf-5.6.8/setup.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/testbase/__init__.py` & `qtaf-5.6.8/testbase/__init__.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/testbase/assertion.py` & `qtaf-5.6.8/testbase/assertion.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,16 +227,23 @@
         self.variable_counter = itertools.count()
         self.stack = []
         self.on_failure = []
         self.push_format_context()
 
         # Rewrite assert into a bunch of statements.
         if isinstance(elem, ast.Expr):
-            top_condition, explanation = self.visit(elem.value.args[1])
-            msg_arg = elem.value.args[0]
+            if len(elem.value.args) < 2 and getattr(elem.value, "keywords", None):
+                for keyword in elem.value.keywords:
+                    if keyword.arg == "message":
+                        msg_arg = keyword.value
+                    elif keyword.arg == "value":
+                        top_condition, explanation = self.visit(keyword.value)
+            else:
+                top_condition, explanation = self.visit(elem.value.args[1])
+                msg_arg = elem.value.args[0]
             caller_id = "self"
         elif isinstance(elem, ast.Call):
             top_condition, explanation = self.visit(elem.args[1])
             msg_arg = elem.args[0]
             caller_id = "_qtaf_assert_"
 
         # Create failure message.
```

### Comparing `qtaf-5.6.7/testbase/conf.py` & `qtaf-5.6.8/testbase/conf.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/testbase/context.py` & `qtaf-5.6.8/testbase/context.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/testbase/datadrive.py` & `qtaf-5.6.8/testbase/datadrive.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/testbase/dist.py` & `qtaf-5.6.8/testbase/dist.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/testbase/exlib.py` & `qtaf-5.6.8/testbase/exlib.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/testbase/loader.py` & `qtaf-5.6.8/testbase/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,17 @@
         i = 0
         while i < len(parts):
             i += 1
             modulename = ".".join(parts[:i])
             try:
                 module = __import__(modulename)  # __import__得到的是最外层模块的object
             except Exception as ex:  # pylint: disable=broad-except
+                if i == len(parts) and hasattr(module, parts[-1]):  # 类写在__init__.py的场景下module需返回文件夹
+                    i -= 1
+                    break
                 self._module_errs[modulename] = traceback.format_exc()
                 return
             else:
                 for name in parts[1:i]:
                     module = getattr(module, name)
                 if not hasattr(module, "__path__"):
                     # file module
```

### Comparing `qtaf-5.6.7/testbase/logger.py` & `qtaf-5.6.8/testbase/logger.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #
 """log模块
 """
 
 import logging
 import sys
 import traceback
+import inspect
 from testbase import context
 from testbase.util import ensure_binary_stream, smart_binary
 
 _stream, _encoding = ensure_binary_stream(sys.stdout)
 
 class _Formatter(logging.Formatter):
     def format(self, record):
@@ -36,29 +37,31 @@
 
 class TestResultBridge(logging.Handler):
     """中转log信息到TestResult"""
 
     def emit(self, log_record):
         """Log Handle 必须实现此函数"""
         testresult = context.current_testresult()
+        formatted_msg = self.format(log_record)
         if testresult is None:
             _stream_handler.emit(log_record)
             return
         record = {}
         if log_record.exc_info:
             record["traceback"] = "".join(
                 traceback.format_tb(log_record.exc_info[2])
             ) + "%s: %s" % (log_record.exc_info[0].__name__, log_record.exc_info[1])
-        testresult.log_record(log_record.levelno, log_record.msg, record)
+        testresult.log_record(log_record.levelno, formatted_msg, record)
 
 
 _LOGGER_NAME = "QTA_LOGGER"
 _logger = logging.getLogger(_LOGGER_NAME)
 _logger.setLevel(logging.DEBUG)
-_logger.addHandler(TestResultBridge())
+_testresult_bridge = TestResultBridge()
+_logger.addHandler(_testresult_bridge)
 
 
 def critical(msg, *args, **kwargs):
     _logger.error(msg, *args, **kwargs)
 
 
 fatal = critical
@@ -105,17 +108,34 @@
 def removeHandler(hdlr):  # pylint: disable=invalid-name
     """Remove the specified handler from this logger."""
     _logger.removeHandler(hdlr)
 
 def set_formatter(fmt):
     """Set the specified formatter to this logger.
     """
-    class __formatter(_Formatter):
+    class __Formatter(_Formatter):
         def __init__(self, fmt):
             super(_Formatter, self).__init__(fmt)
 
-    _stream_handler.setFormatter(__formatter(fmt))
+    class _CustomFormatter(logging.Formatter):
+        def format(self, record):
+            # Get the code line number and file name of the call logger function.
+            logger_module = "logger"
+            for frame_info in inspect.stack():
+                frame = frame_info[0]
+                module_name = inspect.getmodulename(frame.f_code.co_filename)
+                if module_name != "__init__" and module_name != logger_module:
+                    caller = inspect.getframeinfo(frame)
+                    break
+            else:
+                return super(_CustomFormatter, self).format(record)
+            record.filename = caller.filename.split('/')[-1]
+            record.lineno = caller.lineno
+            return super(_CustomFormatter, self).format(record)
+
+    _stream_handler.setFormatter(__Formatter(fmt))
+    _testresult_bridge.setFormatter(_CustomFormatter(fmt))
 
 def set_level(level):
     """Set the specified log level to this logger.
     """
     _logger.setLevel(level)
```

### Comparing `qtaf-5.6.7/testbase/management.py` & `qtaf-5.6.8/testbase/management.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/testbase/plan.py` & `qtaf-5.6.8/testbase/plan.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/testbase/project.py` & `qtaf-5.6.8/testbase/project.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/testbase/report.py` & `qtaf-5.6.8/testbase/report.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/testbase/resource.py` & `qtaf-5.6.8/testbase/resource.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/testbase/retry.py` & `qtaf-5.6.8/testbase/retry.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/testbase/runner.py` & `qtaf-5.6.8/testbase/runner.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/testbase/serialization.py` & `qtaf-5.6.8/testbase/serialization.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/testbase/test.py` & `qtaf-5.6.8/testbase/test.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/testbase/testcase.py` & `qtaf-5.6.8/testbase/testcase.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/testbase/testresult.py` & `qtaf-5.6.8/testbase/testresult.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/testbase/testsuite.py` & `qtaf-5.6.8/testbase/testsuite.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/testbase/types.py` & `qtaf-5.6.8/testbase/types.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/testbase/util.py` & `qtaf-5.6.8/testbase/util.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/tuia/__init__.py` & `qtaf-5.6.8/tuia/__init__.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/tuia/_tif.py` & `qtaf-5.6.8/tuia/_tif.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/tuia/accessible.py` & `qtaf-5.6.8/tuia/accessible.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/tuia/app.py` & `qtaf-5.6.8/tuia/app.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/tuia/control.py` & `qtaf-5.6.8/tuia/control.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/tuia/env.py` & `qtaf-5.6.8/tuia/env.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/tuia/exceptions.py` & `qtaf-5.6.8/tuia/exceptions.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/tuia/filedialog.py` & `qtaf-5.6.8/tuia/filedialog.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/tuia/gfcontrols.py` & `qtaf-5.6.8/tuia/gfcontrols.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/tuia/keyboard.py` & `qtaf-5.6.8/tuia/keyboard.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/tuia/mouse.py` & `qtaf-5.6.8/tuia/mouse.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/tuia/qpath.py` & `qtaf-5.6.8/tuia/qpath.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/tuia/qpathparser.py` & `qtaf-5.6.8/tuia/qpathparser.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/tuia/remoteprocessing.py` & `qtaf-5.6.8/tuia/remoteprocessing.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/tuia/testcase.py` & `qtaf-5.6.8/tuia/testcase.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/tuia/uiacontrols.py` & `qtaf-5.6.8/tuia/uiacontrols.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/tuia/util.py` & `qtaf-5.6.8/tuia/util.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/tuia/webcontrols.py` & `qtaf-5.6.8/tuia/webcontrols.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/tuia/wincontrols.py` & `qtaf-5.6.8/tuia/wincontrols.py`

 * *Files identical despite different names*

### Comparing `qtaf-5.6.7/tuia/wintypes.py` & `qtaf-5.6.8/tuia/wintypes.py`

 * *Files identical despite different names*

