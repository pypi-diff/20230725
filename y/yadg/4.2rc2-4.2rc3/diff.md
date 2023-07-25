# Comparing `tmp/yadg-4.2rc2.tar.gz` & `tmp/yadg-4.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yadg-4.2rc2.tar", last modified: Thu Aug 18 06:30:22 2022, max compression
+gzip compressed data, was "yadg-4.2rc3.tar", last modified: Mon Aug 22 07:17:52 2022, max compression
```

## Comparing `yadg-4.2rc2.tar` & `yadg-4.2rc3.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxrwxrwx   0        0        0        0 2022-08-18 06:30:22.134787 yadg-4.2rc2/
--rw-rw-rw-   0        0        0    35823 2022-05-13 19:10:00.000000 yadg-4.2rc2/LICENSE
--rw-rw-rw-   0        0        0       53 2022-05-13 19:10:00.000000 yadg-4.2rc2/MANIFEST.in
--rw-rw-rw-   0        0        0     3843 2022-08-18 06:30:22.135667 yadg-4.2rc2/PKG-INFO
--rw-rw-rw-   0        0        0     3172 2022-05-13 19:10:00.000000 yadg-4.2rc2/README.md
--rw-rw-rw-   0        0        0      211 2022-08-18 06:30:22.145128 yadg-4.2rc2/setup.cfg
--rw-rw-rw-   0        0        0     1825 2022-08-18 06:29:02.000000 yadg-4.2rc2/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-18 06:30:21.423708 yadg-4.2rc2/src/
-drwxrwxrwx   0        0        0        0 2022-08-18 06:30:22.147013 yadg-4.2rc2/src/yadg/
--rw-rw-rw-   0        0        0      172 2022-05-13 19:10:00.000000 yadg-4.2rc2/src/yadg/__init__.py
--rw-rw-rw-   0        0        0      519 2022-08-18 06:30:22.147013 yadg-4.2rc2/src/yadg/_version.py
-drwxrwxrwx   0        0        0        0 2022-08-18 06:30:21.571371 yadg-4.2rc2/src/yadg/core/
--rw-rw-rw-   0        0        0      135 2022-05-13 19:10:00.000000 yadg-4.2rc2/src/yadg/core/__init__.py
--rw-rw-rw-   0        0        0     4272 2022-05-13 19:10:00.000000 yadg-4.2rc2/src/yadg/core/process.py
--rw-rw-rw-   0        0        0     1120 2022-07-26 11:17:46.000000 yadg-4.2rc2/src/yadg/core/spec_datagram.py
--rw-rw-rw-   0        0        0     8169 2022-05-13 19:10:00.000000 yadg-4.2rc2/src/yadg/core/validators.py
-drwxrwxrwx   0        0        0        0 2022-08-18 06:30:21.618277 yadg-4.2rc2/src/yadg/dgutils/
--rw-rw-rw-   0        0        0      288 2022-05-13 19:10:00.000000 yadg-4.2rc2/src/yadg/dgutils/__init__.py
--rw-rw-rw-   0        0        0     1666 2022-05-13 19:10:00.000000 yadg-4.2rc2/src/yadg/dgutils/btools.py
--rw-rw-rw-   0        0        0     2813 2022-05-13 19:10:00.000000 yadg-4.2rc2/src/yadg/dgutils/calib.py
--rw-rw-rw-   0        0        0    13445 2022-05-13 19:10:00.000000 yadg-4.2rc2/src/yadg/dgutils/dateutils.py
--rw-rw-rw-   0        0        0      640 2022-08-09 10:41:35.000000 yadg-4.2rc2/src/yadg/dgutils/helpers.py
--rw-rw-rw-   0        0        0     2299 2022-05-13 19:10:00.000000 yadg-4.2rc2/src/yadg/dgutils/pintutils.py
--rw-rw-rw-   0        0        0     9181 2022-05-13 19:10:00.000000 yadg-4.2rc2/src/yadg/dgutils/utils.py
--rw-rw-rw-   0        0        0     4377 2022-05-13 19:10:00.000000 yadg-4.2rc2/src/yadg/main.py
-drwxrwxrwx   0        0        0        0 2022-08-18 06:30:21.620267 yadg-4.2rc2/src/yadg/parsers/
--rw-rw-rw-   0        0        0        0 2022-05-13 19:10:00.000000 yadg-4.2rc2/src/yadg/parsers/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-18 06:30:21.626309 yadg-4.2rc2/src/yadg/parsers/basiccsv/
--rw-rw-rw-   0        0        0     1403 2022-08-18 06:29:02.000000 yadg-4.2rc2/src/yadg/parsers/basiccsv/__init__.py
--rw-rw-rw-   0        0        0     7666 2022-08-17 14:38:19.000000 yadg-4.2rc2/src/yadg/parsers/basiccsv/main.py
-drwxrwxrwx   0        0        0        0 2022-08-18 06:30:21.696480 yadg-4.2rc2/src/yadg/parsers/chromdata/
--rw-rw-rw-   0        0        0     2517 2022-08-16 11:37:52.000000 yadg-4.2rc2/src/yadg/parsers/chromdata/__init__.py
--rw-rw-rw-   0        0        0     7338 2022-08-10 07:35:21.000000 yadg-4.2rc2/src/yadg/parsers/chromdata/empalccsv.py
--rw-rw-rw-   0        0        0     7155 2022-08-16 11:37:52.000000 yadg-4.2rc2/src/yadg/parsers/chromdata/empalcxlsx.py
--rw-rw-rw-   0        0        0     3635 2022-08-10 07:35:21.000000 yadg-4.2rc2/src/yadg/parsers/chromdata/fusioncsv.py
--rw-rw-rw-   0        0        0     4636 2022-08-10 07:35:21.000000 yadg-4.2rc2/src/yadg/parsers/chromdata/fusionjson.py
--rw-rw-rw-   0        0        0     1985 2022-08-10 07:35:21.000000 yadg-4.2rc2/src/yadg/parsers/chromdata/fusionzip.py
--rw-rw-rw-   0        0        0     1636 2022-08-10 07:35:21.000000 yadg-4.2rc2/src/yadg/parsers/chromdata/main.py
-drwxrwxrwx   0        0        0        0 2022-08-18 06:30:21.813481 yadg-4.2rc2/src/yadg/parsers/chromtrace/
--rw-rw-rw-   0        0        0     5082 2022-08-16 11:37:52.000000 yadg-4.2rc2/src/yadg/parsers/chromtrace/__init__.py
--rw-rw-rw-   0        0        0     4235 2022-08-09 06:33:35.000000 yadg-4.2rc2/src/yadg/parsers/chromtrace/agilentch.py
--rw-rw-rw-   0        0        0     4586 2022-08-09 06:33:35.000000 yadg-4.2rc2/src/yadg/parsers/chromtrace/agilentcsv.py
--rw-rw-rw-   0        0        0     2384 2022-08-09 06:33:35.000000 yadg-4.2rc2/src/yadg/parsers/chromtrace/agilentdx.py
--rw-rw-rw-   0        0        0     5149 2022-08-09 06:33:35.000000 yadg-4.2rc2/src/yadg/parsers/chromtrace/ezchromasc.py
--rw-rw-rw-   0        0        0     3447 2022-08-09 10:41:35.000000 yadg-4.2rc2/src/yadg/parsers/chromtrace/fusionjson.py
--rw-rw-rw-   0        0        0     1948 2022-08-09 06:33:35.000000 yadg-4.2rc2/src/yadg/parsers/chromtrace/fusionzip.py
--rw-rw-rw-   0        0        0    12484 2022-05-13 19:10:01.000000 yadg-4.2rc2/src/yadg/parsers/chromtrace/integration.py
--rw-rw-rw-   0        0        0     7278 2022-08-09 10:41:35.000000 yadg-4.2rc2/src/yadg/parsers/chromtrace/main.py
-drwxrwxrwx   0        0        0        0 2022-08-18 06:30:21.832432 yadg-4.2rc2/src/yadg/parsers/dummy/
--rw-rw-rw-   0        0        0      126 2022-08-11 12:15:24.000000 yadg-4.2rc2/src/yadg/parsers/dummy/__init__.py
--rw-rw-rw-   0        0        0     1800 2022-08-16 11:37:52.000000 yadg-4.2rc2/src/yadg/parsers/dummy/main.py
-drwxrwxrwx   0        0        0        0 2022-08-18 06:30:21.872424 yadg-4.2rc2/src/yadg/parsers/electrochem/
--rw-rw-rw-   0        0        0     3021 2022-08-16 11:37:52.000000 yadg-4.2rc2/src/yadg/parsers/electrochem/__init__.py
--rw-rw-rw-   0        0        0    32569 2022-08-16 11:37:52.000000 yadg-4.2rc2/src/yadg/parsers/electrochem/eclabmpr.py
--rw-rw-rw-   0        0        0    13553 2022-08-16 11:37:52.000000 yadg-4.2rc2/src/yadg/parsers/electrochem/eclabmpt.py
--rw-rw-rw-   0        0        0    31461 2022-08-16 11:37:52.000000 yadg-4.2rc2/src/yadg/parsers/electrochem/eclabtechniques.py
--rw-rw-rw-   0        0        0     1584 2022-08-10 09:47:45.000000 yadg-4.2rc2/src/yadg/parsers/electrochem/main.py
--rw-rw-rw-   0        0        0     3405 2022-08-10 09:47:45.000000 yadg-4.2rc2/src/yadg/parsers/electrochem/tomatojson.py
-drwxrwxrwx   0        0        0        0 2022-08-18 06:30:21.905793 yadg-4.2rc2/src/yadg/parsers/flowdata/
--rw-rw-rw-   0        0        0     1170 2022-08-16 11:37:52.000000 yadg-4.2rc2/src/yadg/parsers/flowdata/__init__.py
--rw-rw-rw-   0        0        0     6698 2022-05-13 19:10:01.000000 yadg-4.2rc2/src/yadg/parsers/flowdata/drycal.py
--rw-rw-rw-   0        0        0     2453 2022-08-09 10:41:35.000000 yadg-4.2rc2/src/yadg/parsers/flowdata/main.py
-drwxrwxrwx   0        0        0        0 2022-08-18 06:30:21.933165 yadg-4.2rc2/src/yadg/parsers/masstrace/
--rw-rw-rw-   0        0        0     2342 2022-08-16 11:37:52.000000 yadg-4.2rc2/src/yadg/parsers/masstrace/__init__.py
--rw-rw-rw-   0        0        0     1007 2022-08-09 10:41:35.000000 yadg-4.2rc2/src/yadg/parsers/masstrace/main.py
--rw-rw-rw-   0        0        0    10825 2022-05-13 19:10:01.000000 yadg-4.2rc2/src/yadg/parsers/masstrace/quadstarsac.py
-drwxrwxrwx   0        0        0        0 2022-08-18 06:30:21.949518 yadg-4.2rc2/src/yadg/parsers/meascsv/
--rw-rw-rw-   0        0        0     1099 2022-08-16 11:37:52.000000 yadg-4.2rc2/src/yadg/parsers/meascsv/__init__.py
--rw-rw-rw-   0        0        0     3088 2022-08-17 11:10:22.000000 yadg-4.2rc2/src/yadg/parsers/meascsv/main.py
-drwxrwxrwx   0        0        0        0 2022-08-18 06:30:22.018319 yadg-4.2rc2/src/yadg/parsers/qftrace/
--rw-rw-rw-   0        0        0     2532 2022-08-16 11:37:52.000000 yadg-4.2rc2/src/yadg/parsers/qftrace/__init__.py
--rw-rw-rw-   0        0        0     8442 2022-05-13 19:10:01.000000 yadg-4.2rc2/src/yadg/parsers/qftrace/fit.py
--rw-rw-rw-   0        0        0     3183 2022-05-13 19:10:01.000000 yadg-4.2rc2/src/yadg/parsers/qftrace/labviewcsv.py
--rw-rw-rw-   0        0        0     3473 2022-08-09 10:41:35.000000 yadg-4.2rc2/src/yadg/parsers/qftrace/main.py
--rw-rw-rw-   0        0        0     2227 2022-05-13 19:10:01.000000 yadg-4.2rc2/src/yadg/parsers/qftrace/prune.py
-drwxrwxrwx   0        0        0        0 2022-08-18 06:30:22.055227 yadg-4.2rc2/src/yadg/parsers/xpstrace/
--rw-rw-rw-   0        0        0     1947 2022-08-16 11:37:52.000000 yadg-4.2rc2/src/yadg/parsers/xpstrace/__init__.py
--rw-rw-rw-   0        0        0     1000 2022-08-09 10:41:35.000000 yadg-4.2rc2/src/yadg/parsers/xpstrace/main.py
--rw-rw-rw-   0        0        0    13806 2022-05-13 19:10:01.000000 yadg-4.2rc2/src/yadg/parsers/xpstrace/phispe.py
-drwxrwxrwx   0        0        0        0 2022-08-18 06:30:22.131698 yadg-4.2rc2/src/yadg/parsers/xrdtrace/
--rw-rw-rw-   0        0        0     1694 2022-08-16 11:37:52.000000 yadg-4.2rc2/src/yadg/parsers/xrdtrace/__init__.py
--rw-rw-rw-   0        0        0     1962 2022-05-13 19:10:01.000000 yadg-4.2rc2/src/yadg/parsers/xrdtrace/common.py
--rw-rw-rw-   0        0        0     1308 2022-08-09 10:41:35.000000 yadg-4.2rc2/src/yadg/parsers/xrdtrace/main.py
--rw-rw-rw-   0        0        0     4675 2022-05-13 19:10:01.000000 yadg-4.2rc2/src/yadg/parsers/xrdtrace/panalyticalcsv.py
--rw-rw-rw-   0        0        0     7555 2022-05-13 19:10:01.000000 yadg-4.2rc2/src/yadg/parsers/xrdtrace/panalyticalxrdml.py
--rw-rw-rw-   0        0        0     2198 2022-05-13 19:10:01.000000 yadg-4.2rc2/src/yadg/parsers/xrdtrace/panalyticalxy.py
--rw-rw-rw-   0        0        0     6909 2022-08-09 06:33:35.000000 yadg-4.2rc2/src/yadg/subcommands.py
-drwxrwxrwx   0        0        0        0 2022-08-18 06:30:21.547437 yadg-4.2rc2/src/yadg.egg-info/
--rw-rw-rw-   0        0        0     3843 2022-08-18 06:30:21.000000 yadg-4.2rc2/src/yadg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2525 2022-08-18 06:30:21.000000 yadg-4.2rc2/src/yadg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-18 06:30:21.000000 yadg-4.2rc2/src/yadg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2022-08-18 06:30:21.000000 yadg-4.2rc2/src/yadg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      216 2022-08-18 06:30:21.000000 yadg-4.2rc2/src/yadg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2022-08-18 06:30:21.000000 yadg-4.2rc2/src/yadg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    83320 2022-05-13 19:10:03.000000 yadg-4.2rc2/versioneer.py
+drwxrwxrwx   0        0        0        0 2022-08-22 07:17:52.676196 yadg-4.2rc3/
+-rw-rw-rw-   0        0        0    35823 2022-05-13 19:10:00.000000 yadg-4.2rc3/LICENSE
+-rw-rw-rw-   0        0        0       53 2022-05-13 19:10:00.000000 yadg-4.2rc3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3843 2022-08-22 07:17:52.676196 yadg-4.2rc3/PKG-INFO
+-rw-rw-rw-   0        0        0     3172 2022-05-13 19:10:00.000000 yadg-4.2rc3/README.md
+-rw-rw-rw-   0        0        0      211 2022-08-22 07:17:52.689251 yadg-4.2rc3/setup.cfg
+-rw-rw-rw-   0        0        0     1825 2022-08-18 06:29:02.000000 yadg-4.2rc3/setup.py
+drwxrwxrwx   0        0        0        0 2022-08-22 07:17:52.383645 yadg-4.2rc3/src/
+drwxrwxrwx   0        0        0        0 2022-08-22 07:17:52.691246 yadg-4.2rc3/src/yadg/
+-rw-rw-rw-   0        0        0      172 2022-05-13 19:10:00.000000 yadg-4.2rc3/src/yadg/__init__.py
+-rw-rw-rw-   0        0        0      519 2022-08-22 07:17:52.691246 yadg-4.2rc3/src/yadg/_version.py
+drwxrwxrwx   0        0        0        0 2022-08-22 07:17:52.492008 yadg-4.2rc3/src/yadg/core/
+-rw-rw-rw-   0        0        0      135 2022-05-13 19:10:00.000000 yadg-4.2rc3/src/yadg/core/__init__.py
+-rw-rw-rw-   0        0        0     4272 2022-05-13 19:10:00.000000 yadg-4.2rc3/src/yadg/core/process.py
+-rw-rw-rw-   0        0        0     1120 2022-07-26 11:17:46.000000 yadg-4.2rc3/src/yadg/core/spec_datagram.py
+-rw-rw-rw-   0        0        0     8169 2022-05-13 19:10:00.000000 yadg-4.2rc3/src/yadg/core/validators.py
+drwxrwxrwx   0        0        0        0 2022-08-22 07:17:52.514798 yadg-4.2rc3/src/yadg/dgutils/
+-rw-rw-rw-   0        0        0      288 2022-05-13 19:10:00.000000 yadg-4.2rc3/src/yadg/dgutils/__init__.py
+-rw-rw-rw-   0        0        0     1666 2022-05-13 19:10:00.000000 yadg-4.2rc3/src/yadg/dgutils/btools.py
+-rw-rw-rw-   0        0        0     2813 2022-05-13 19:10:00.000000 yadg-4.2rc3/src/yadg/dgutils/calib.py
+-rw-rw-rw-   0        0        0    13445 2022-05-13 19:10:00.000000 yadg-4.2rc3/src/yadg/dgutils/dateutils.py
+-rw-rw-rw-   0        0        0      640 2022-08-09 10:41:35.000000 yadg-4.2rc3/src/yadg/dgutils/helpers.py
+-rw-rw-rw-   0        0        0     2299 2022-05-13 19:10:00.000000 yadg-4.2rc3/src/yadg/dgutils/pintutils.py
+-rw-rw-rw-   0        0        0     9181 2022-05-13 19:10:00.000000 yadg-4.2rc3/src/yadg/dgutils/utils.py
+-rw-rw-rw-   0        0        0     4377 2022-05-13 19:10:00.000000 yadg-4.2rc3/src/yadg/main.py
+drwxrwxrwx   0        0        0        0 2022-08-22 07:17:52.518656 yadg-4.2rc3/src/yadg/parsers/
+-rw-rw-rw-   0        0        0        0 2022-05-13 19:10:00.000000 yadg-4.2rc3/src/yadg/parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2022-08-22 07:17:52.523642 yadg-4.2rc3/src/yadg/parsers/basiccsv/
+-rw-rw-rw-   0        0        0     1636 2022-08-18 09:10:48.000000 yadg-4.2rc3/src/yadg/parsers/basiccsv/__init__.py
+-rw-rw-rw-   0        0        0     7700 2022-08-18 09:10:48.000000 yadg-4.2rc3/src/yadg/parsers/basiccsv/main.py
+drwxrwxrwx   0        0        0        0 2022-08-22 07:17:52.546755 yadg-4.2rc3/src/yadg/parsers/chromdata/
+-rw-rw-rw-   0        0        0     2517 2022-08-16 11:37:52.000000 yadg-4.2rc3/src/yadg/parsers/chromdata/__init__.py
+-rw-rw-rw-   0        0        0     7338 2022-08-10 07:35:21.000000 yadg-4.2rc3/src/yadg/parsers/chromdata/empalccsv.py
+-rw-rw-rw-   0        0        0     7155 2022-08-16 11:37:52.000000 yadg-4.2rc3/src/yadg/parsers/chromdata/empalcxlsx.py
+-rw-rw-rw-   0        0        0     3635 2022-08-10 07:35:21.000000 yadg-4.2rc3/src/yadg/parsers/chromdata/fusioncsv.py
+-rw-rw-rw-   0        0        0     4636 2022-08-10 07:35:21.000000 yadg-4.2rc3/src/yadg/parsers/chromdata/fusionjson.py
+-rw-rw-rw-   0        0        0     1985 2022-08-10 07:35:21.000000 yadg-4.2rc3/src/yadg/parsers/chromdata/fusionzip.py
+-rw-rw-rw-   0        0        0     1636 2022-08-10 07:35:21.000000 yadg-4.2rc3/src/yadg/parsers/chromdata/main.py
+drwxrwxrwx   0        0        0        0 2022-08-22 07:17:52.575419 yadg-4.2rc3/src/yadg/parsers/chromtrace/
+-rw-rw-rw-   0        0        0     5082 2022-08-16 11:37:52.000000 yadg-4.2rc3/src/yadg/parsers/chromtrace/__init__.py
+-rw-rw-rw-   0        0        0     4235 2022-08-09 06:33:35.000000 yadg-4.2rc3/src/yadg/parsers/chromtrace/agilentch.py
+-rw-rw-rw-   0        0        0     4586 2022-08-09 06:33:35.000000 yadg-4.2rc3/src/yadg/parsers/chromtrace/agilentcsv.py
+-rw-rw-rw-   0        0        0     2384 2022-08-09 06:33:35.000000 yadg-4.2rc3/src/yadg/parsers/chromtrace/agilentdx.py
+-rw-rw-rw-   0        0        0     5149 2022-08-09 06:33:35.000000 yadg-4.2rc3/src/yadg/parsers/chromtrace/ezchromasc.py
+-rw-rw-rw-   0        0        0     3447 2022-08-09 10:41:35.000000 yadg-4.2rc3/src/yadg/parsers/chromtrace/fusionjson.py
+-rw-rw-rw-   0        0        0     1948 2022-08-09 06:33:35.000000 yadg-4.2rc3/src/yadg/parsers/chromtrace/fusionzip.py
+-rw-rw-rw-   0        0        0    12484 2022-05-13 19:10:01.000000 yadg-4.2rc3/src/yadg/parsers/chromtrace/integration.py
+-rw-rw-rw-   0        0        0     7278 2022-08-09 10:41:35.000000 yadg-4.2rc3/src/yadg/parsers/chromtrace/main.py
+drwxrwxrwx   0        0        0        0 2022-08-22 07:17:52.582404 yadg-4.2rc3/src/yadg/parsers/dummy/
+-rw-rw-rw-   0        0        0      126 2022-08-11 12:15:24.000000 yadg-4.2rc3/src/yadg/parsers/dummy/__init__.py
+-rw-rw-rw-   0        0        0     1800 2022-08-16 11:37:52.000000 yadg-4.2rc3/src/yadg/parsers/dummy/main.py
+drwxrwxrwx   0        0        0        0 2022-08-22 07:17:52.606901 yadg-4.2rc3/src/yadg/parsers/electrochem/
+-rw-rw-rw-   0        0        0     3021 2022-08-16 11:37:52.000000 yadg-4.2rc3/src/yadg/parsers/electrochem/__init__.py
+-rw-rw-rw-   0        0        0    32569 2022-08-16 11:37:52.000000 yadg-4.2rc3/src/yadg/parsers/electrochem/eclabmpr.py
+-rw-rw-rw-   0        0        0    13553 2022-08-16 11:37:52.000000 yadg-4.2rc3/src/yadg/parsers/electrochem/eclabmpt.py
+-rw-rw-rw-   0        0        0    31461 2022-08-16 11:37:52.000000 yadg-4.2rc3/src/yadg/parsers/electrochem/eclabtechniques.py
+-rw-rw-rw-   0        0        0     1584 2022-08-10 09:47:45.000000 yadg-4.2rc3/src/yadg/parsers/electrochem/main.py
+-rw-rw-rw-   0        0        0     3405 2022-08-10 09:47:45.000000 yadg-4.2rc3/src/yadg/parsers/electrochem/tomatojson.py
+drwxrwxrwx   0        0        0        0 2022-08-22 07:17:52.616889 yadg-4.2rc3/src/yadg/parsers/flowdata/
+-rw-rw-rw-   0        0        0     1170 2022-08-16 11:37:52.000000 yadg-4.2rc3/src/yadg/parsers/flowdata/__init__.py
+-rw-rw-rw-   0        0        0     6698 2022-05-13 19:10:01.000000 yadg-4.2rc3/src/yadg/parsers/flowdata/drycal.py
+-rw-rw-rw-   0        0        0     2453 2022-08-09 10:41:35.000000 yadg-4.2rc3/src/yadg/parsers/flowdata/main.py
+drwxrwxrwx   0        0        0        0 2022-08-22 07:17:52.623872 yadg-4.2rc3/src/yadg/parsers/masstrace/
+-rw-rw-rw-   0        0        0     2342 2022-08-16 11:37:52.000000 yadg-4.2rc3/src/yadg/parsers/masstrace/__init__.py
+-rw-rw-rw-   0        0        0     1007 2022-08-09 10:41:35.000000 yadg-4.2rc3/src/yadg/parsers/masstrace/main.py
+-rw-rw-rw-   0        0        0    10825 2022-05-13 19:10:01.000000 yadg-4.2rc3/src/yadg/parsers/masstrace/quadstarsac.py
+drwxrwxrwx   0        0        0        0 2022-08-22 07:17:52.627863 yadg-4.2rc3/src/yadg/parsers/meascsv/
+-rw-rw-rw-   0        0        0     1099 2022-08-16 11:37:52.000000 yadg-4.2rc3/src/yadg/parsers/meascsv/__init__.py
+-rw-rw-rw-   0        0        0     3088 2022-08-17 11:10:22.000000 yadg-4.2rc3/src/yadg/parsers/meascsv/main.py
+drwxrwxrwx   0        0        0        0 2022-08-22 07:17:52.642709 yadg-4.2rc3/src/yadg/parsers/qftrace/
+-rw-rw-rw-   0        0        0     2532 2022-08-16 11:37:52.000000 yadg-4.2rc3/src/yadg/parsers/qftrace/__init__.py
+-rw-rw-rw-   0        0        0     8442 2022-05-13 19:10:01.000000 yadg-4.2rc3/src/yadg/parsers/qftrace/fit.py
+-rw-rw-rw-   0        0        0     3183 2022-05-13 19:10:01.000000 yadg-4.2rc3/src/yadg/parsers/qftrace/labviewcsv.py
+-rw-rw-rw-   0        0        0     3473 2022-08-09 10:41:35.000000 yadg-4.2rc3/src/yadg/parsers/qftrace/main.py
+-rw-rw-rw-   0        0        0     2227 2022-05-13 19:10:01.000000 yadg-4.2rc3/src/yadg/parsers/qftrace/prune.py
+drwxrwxrwx   0        0        0        0 2022-08-22 07:17:52.653257 yadg-4.2rc3/src/yadg/parsers/xpstrace/
+-rw-rw-rw-   0        0        0     1947 2022-08-16 11:37:52.000000 yadg-4.2rc3/src/yadg/parsers/xpstrace/__init__.py
+-rw-rw-rw-   0        0        0     1000 2022-08-09 10:41:35.000000 yadg-4.2rc3/src/yadg/parsers/xpstrace/main.py
+-rw-rw-rw-   0        0        0    13806 2022-05-13 19:10:01.000000 yadg-4.2rc3/src/yadg/parsers/xpstrace/phispe.py
+drwxrwxrwx   0        0        0        0 2022-08-22 07:17:52.672207 yadg-4.2rc3/src/yadg/parsers/xrdtrace/
+-rw-rw-rw-   0        0        0     1694 2022-08-16 11:37:52.000000 yadg-4.2rc3/src/yadg/parsers/xrdtrace/__init__.py
+-rw-rw-rw-   0        0        0     1962 2022-05-13 19:10:01.000000 yadg-4.2rc3/src/yadg/parsers/xrdtrace/common.py
+-rw-rw-rw-   0        0        0     1308 2022-08-09 10:41:35.000000 yadg-4.2rc3/src/yadg/parsers/xrdtrace/main.py
+-rw-rw-rw-   0        0        0     4675 2022-05-13 19:10:01.000000 yadg-4.2rc3/src/yadg/parsers/xrdtrace/panalyticalcsv.py
+-rw-rw-rw-   0        0        0     7555 2022-05-13 19:10:01.000000 yadg-4.2rc3/src/yadg/parsers/xrdtrace/panalyticalxrdml.py
+-rw-rw-rw-   0        0        0     2198 2022-05-13 19:10:01.000000 yadg-4.2rc3/src/yadg/parsers/xrdtrace/panalyticalxy.py
+-rw-rw-rw-   0        0        0     6909 2022-08-09 06:33:35.000000 yadg-4.2rc3/src/yadg/subcommands.py
+drwxrwxrwx   0        0        0        0 2022-08-22 07:17:52.479954 yadg-4.2rc3/src/yadg.egg-info/
+-rw-rw-rw-   0        0        0     3843 2022-08-22 07:17:52.000000 yadg-4.2rc3/src/yadg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2525 2022-08-22 07:17:52.000000 yadg-4.2rc3/src/yadg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-08-22 07:17:52.000000 yadg-4.2rc3/src/yadg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2022-08-22 07:17:52.000000 yadg-4.2rc3/src/yadg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      216 2022-08-22 07:17:52.000000 yadg-4.2rc3/src/yadg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2022-08-22 07:17:52.000000 yadg-4.2rc3/src/yadg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    83320 2022-05-13 19:10:03.000000 yadg-4.2rc3/versioneer.py
```

### Comparing `yadg-4.2rc2/LICENSE` & `yadg-4.2rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/PKG-INFO` & `yadg-4.2rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yadg
-Version: 4.2rc2
+Version: 4.2rc3
 Summary: yet another datagram
 Home-page: https://github.com/dgbowl/yadg
 Author: Peter Kraus
 Author-email: peter@tondon.de
 Project-URL: Bug Tracker, https://github.com/dgbowl/yadg/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `yadg-4.2rc2/README.md` & `yadg-4.2rc3/README.md`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/setup.py` & `yadg-4.2rc3/setup.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/_version.py` & `yadg-4.2rc3/src/yadg/_version.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2022-08-18T08:28:49+0200",
+ "date": "2022-08-22T09:14:34+0200",
  "dirty": false,
  "error": null,
- "full-revisionid": "6b768acf3a5e273ea2b81d30cc4d5cbd16f999d6",
- "version": "4.2rc2"
+ "full-revisionid": "2712ced892c06e1f9aedacdf28e8447cd18dc675",
+ "version": "4.2rc3"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

### Comparing `yadg-4.2rc2/src/yadg/core/process.py` & `yadg-4.2rc3/src/yadg/core/process.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/core/spec_datagram.py` & `yadg-4.2rc3/src/yadg/core/spec_datagram.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/core/validators.py` & `yadg-4.2rc3/src/yadg/core/validators.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/dgutils/btools.py` & `yadg-4.2rc3/src/yadg/dgutils/btools.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/dgutils/calib.py` & `yadg-4.2rc3/src/yadg/dgutils/calib.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/dgutils/dateutils.py` & `yadg-4.2rc3/src/yadg/dgutils/dateutils.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/dgutils/helpers.py` & `yadg-4.2rc3/src/yadg/dgutils/helpers.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/dgutils/pintutils.py` & `yadg-4.2rc3/src/yadg/dgutils/pintutils.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/dgutils/utils.py` & `yadg-4.2rc3/src/yadg/dgutils/utils.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/main.py` & `yadg-4.2rc3/src/yadg/main.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/basiccsv/__init__.py` & `yadg-4.2rc3/src/yadg/parsers/basiccsv/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 """
 This parser handles the reading and processing of any tabular files, as long as 
 the first line contains the column headers. By default, the second should contain
 the units. The columns of the table must be separated using a separator such as 
 ``,``, ``;``, or ``\\t``. 
 
+.. warning::
+
+  Since ``yadg-4.2``, the parser handles sparse tables (i.e. tables with missing 
+  data) by creating sparse `datagrams`, which means that the each element of the 
+  header might not be present in each timestep.
+
 .. note::
 
   :mod:`~yadg.parsers.basiccsv` attempts to deduce the timestamp from the column 
   headers, using :func:`yadg.dgutils.dateutils.infer_timestamp_from`. Alternatively, 
   the column(s) containing the timestamp data and their format can be provided using 
   parameters.
```

### Comparing `yadg-4.2rc2/src/yadg/parsers/basiccsv/main.py` & `yadg-4.2rc3/src/yadg/parsers/basiccsv/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,18 +82,19 @@
     raw = dict()
     der = dict()
     element = {"raw": dict()}
     columns = [column.strip() for column in items]
 
     # Process raw data, assign sigma and units
     element["uts"] = datefunc(*[columns[i] for i in datecolumns])
-    for header in headers:
-        ci = headers.index(header)
+    for ci, header in enumerate(headers):
         if ci in datecolumns:
             continue
+        elif columns[ci] == "":
+            continue
         try:
             val, sig = tuple_fromstr(columns[ci])
             unit = units[header]
             element["raw"][header] = {"n": val, "s": sig, "u": unit}
             raw[header] = (val, sig)
         except ValueError:
             element["raw"][header] = columns[ci]
```

### Comparing `yadg-4.2rc2/src/yadg/parsers/chromdata/__init__.py` & `yadg-4.2rc3/src/yadg/parsers/chromdata/__init__.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/chromdata/empalccsv.py` & `yadg-4.2rc3/src/yadg/parsers/chromdata/empalccsv.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/chromdata/empalcxlsx.py` & `yadg-4.2rc3/src/yadg/parsers/chromdata/empalcxlsx.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/chromdata/fusioncsv.py` & `yadg-4.2rc3/src/yadg/parsers/chromdata/fusioncsv.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/chromdata/fusionjson.py` & `yadg-4.2rc3/src/yadg/parsers/chromdata/fusionjson.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/chromdata/fusionzip.py` & `yadg-4.2rc3/src/yadg/parsers/chromdata/fusionzip.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/chromdata/main.py` & `yadg-4.2rc3/src/yadg/parsers/chromdata/main.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/chromtrace/__init__.py` & `yadg-4.2rc3/src/yadg/parsers/chromtrace/__init__.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/chromtrace/agilentch.py` & `yadg-4.2rc3/src/yadg/parsers/chromtrace/agilentch.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/chromtrace/agilentcsv.py` & `yadg-4.2rc3/src/yadg/parsers/chromtrace/agilentcsv.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/chromtrace/agilentdx.py` & `yadg-4.2rc3/src/yadg/parsers/chromtrace/agilentdx.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/chromtrace/ezchromasc.py` & `yadg-4.2rc3/src/yadg/parsers/chromtrace/ezchromasc.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/chromtrace/fusionjson.py` & `yadg-4.2rc3/src/yadg/parsers/chromtrace/fusionjson.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/chromtrace/fusionzip.py` & `yadg-4.2rc3/src/yadg/parsers/chromtrace/fusionzip.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/chromtrace/integration.py` & `yadg-4.2rc3/src/yadg/parsers/chromtrace/integration.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/chromtrace/main.py` & `yadg-4.2rc3/src/yadg/parsers/chromtrace/main.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/dummy/main.py` & `yadg-4.2rc3/src/yadg/parsers/dummy/main.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/electrochem/__init__.py` & `yadg-4.2rc3/src/yadg/parsers/electrochem/__init__.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/electrochem/eclabmpr.py` & `yadg-4.2rc3/src/yadg/parsers/electrochem/eclabmpr.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/electrochem/eclabmpt.py` & `yadg-4.2rc3/src/yadg/parsers/electrochem/eclabmpt.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/electrochem/eclabtechniques.py` & `yadg-4.2rc3/src/yadg/parsers/electrochem/eclabtechniques.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/electrochem/main.py` & `yadg-4.2rc3/src/yadg/parsers/electrochem/main.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/electrochem/tomatojson.py` & `yadg-4.2rc3/src/yadg/parsers/electrochem/tomatojson.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/flowdata/__init__.py` & `yadg-4.2rc3/src/yadg/parsers/flowdata/__init__.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/flowdata/drycal.py` & `yadg-4.2rc3/src/yadg/parsers/flowdata/drycal.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/flowdata/main.py` & `yadg-4.2rc3/src/yadg/parsers/flowdata/main.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/masstrace/__init__.py` & `yadg-4.2rc3/src/yadg/parsers/masstrace/__init__.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/masstrace/main.py` & `yadg-4.2rc3/src/yadg/parsers/masstrace/main.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/masstrace/quadstarsac.py` & `yadg-4.2rc3/src/yadg/parsers/masstrace/quadstarsac.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/meascsv/__init__.py` & `yadg-4.2rc3/src/yadg/parsers/meascsv/__init__.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/meascsv/main.py` & `yadg-4.2rc3/src/yadg/parsers/meascsv/main.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/qftrace/__init__.py` & `yadg-4.2rc3/src/yadg/parsers/qftrace/__init__.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/qftrace/fit.py` & `yadg-4.2rc3/src/yadg/parsers/qftrace/fit.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/qftrace/labviewcsv.py` & `yadg-4.2rc3/src/yadg/parsers/qftrace/labviewcsv.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/qftrace/main.py` & `yadg-4.2rc3/src/yadg/parsers/qftrace/main.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/qftrace/prune.py` & `yadg-4.2rc3/src/yadg/parsers/qftrace/prune.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/xpstrace/__init__.py` & `yadg-4.2rc3/src/yadg/parsers/xpstrace/__init__.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/xpstrace/main.py` & `yadg-4.2rc3/src/yadg/parsers/xpstrace/main.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/xpstrace/phispe.py` & `yadg-4.2rc3/src/yadg/parsers/xpstrace/phispe.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/xrdtrace/__init__.py` & `yadg-4.2rc3/src/yadg/parsers/xrdtrace/__init__.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/xrdtrace/common.py` & `yadg-4.2rc3/src/yadg/parsers/xrdtrace/common.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/xrdtrace/main.py` & `yadg-4.2rc3/src/yadg/parsers/xrdtrace/main.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/xrdtrace/panalyticalcsv.py` & `yadg-4.2rc3/src/yadg/parsers/xrdtrace/panalyticalcsv.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/xrdtrace/panalyticalxrdml.py` & `yadg-4.2rc3/src/yadg/parsers/xrdtrace/panalyticalxrdml.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/parsers/xrdtrace/panalyticalxy.py` & `yadg-4.2rc3/src/yadg/parsers/xrdtrace/panalyticalxy.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg/subcommands.py` & `yadg-4.2rc3/src/yadg/subcommands.py`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/src/yadg.egg-info/PKG-INFO` & `yadg-4.2rc3/src/yadg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yadg
-Version: 4.2rc2
+Version: 4.2rc3
 Summary: yet another datagram
 Home-page: https://github.com/dgbowl/yadg
 Author: Peter Kraus
 Author-email: peter@tondon.de
 Project-URL: Bug Tracker, https://github.com/dgbowl/yadg/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `yadg-4.2rc2/src/yadg.egg-info/SOURCES.txt` & `yadg-4.2rc3/src/yadg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yadg-4.2rc2/versioneer.py` & `yadg-4.2rc3/versioneer.py`

 * *Files identical despite different names*

