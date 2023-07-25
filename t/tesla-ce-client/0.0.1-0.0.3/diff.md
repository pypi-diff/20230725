# Comparing `tmp/tesla-ce-client-0.0.1.tar.gz` & `tmp/tesla-ce-client-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tesla-ce-client-0.0.1.tar", last modified: Fri May 28 18:26:11 2021, max compression
+gzip compressed data, was "tesla-ce-client-0.0.3.tar", last modified: Tue Jul 25 09:56:03 2023, max compression
```

## Comparing `tesla-ce-client-0.0.1.tar` & `tesla-ce-client-0.0.3.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-28 18:26:11.495721 tesla-ce-client-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       82 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2825 2021-05-28 18:26:11.495721 tesla-ce-client-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2001 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      159 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-28 18:26:11.495721 tesla-ce-client-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1504 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-28 18:26:11.487721 tesla-ce-client-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-28 18:26:11.487721 tesla-ce-client-0.0.1/src/tesla_ce_client/
--rw-r--r--   0 runner    (1001) docker     (121)      826 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/src/tesla_ce_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5914 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/src/tesla_ce_client/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     9219 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/src/tesla_ce_client/connector.py
--rw-r--r--   0 runner    (1001) docker     (121)     3461 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/src/tesla_ce_client/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-28 18:26:11.487721 tesla-ce-client-0.0.1/src/tesla_ce_client/institution/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/src/tesla_ce_client/institution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-28 18:26:11.491721 tesla-ce-client-0.0.1/src/tesla_ce_client/provider/
--rw-r--r--   0 runner    (1001) docker     (121)      869 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/src/tesla_ce_client/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2864 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/src/tesla_ce_client/provider/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    11130 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/src/tesla_ce_client/provider/enrolment.py
--rw-r--r--   0 runner    (1001) docker     (121)     2752 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/src/tesla_ce_client/provider/notification.py
--rw-r--r--   0 runner    (1001) docker     (121)     3291 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/src/tesla_ce_client/provider/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-28 18:26:11.491721 tesla-ce-client-0.0.1/src/tesla_ce_client/v1/
--rw-r--r--   0 runner    (1001) docker     (121)      794 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/src/tesla_ce_client/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      866 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/src/tesla_ce_client/v1/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      875 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/src/tesla_ce_client/v1/rt.py
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/src/tesla_ce_client/v1/tep.py
--rw-r--r--   0 runner    (1001) docker     (121)     1478 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/src/tesla_ce_client/v1/tip.py
--rw-r--r--   0 runner    (1001) docker     (121)     1277 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/src/tesla_ce_client/v1/v1.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-28 18:26:11.491721 tesla-ce-client-0.0.1/src/tesla_ce_client/vle/
--rw-r--r--   0 runner    (1001) docker     (121)      859 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/src/tesla_ce_client/vle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3680 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/src/tesla_ce_client/vle/client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-28 18:26:11.491721 tesla-ce-client-0.0.1/src/tesla_ce_client/vle/course/
--rw-r--r--   0 runner    (1001) docker     (121)      857 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/src/tesla_ce_client/vle/course/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-28 18:26:11.491721 tesla-ce-client-0.0.1/src/tesla_ce_client/vle/course/activity/
--rw-r--r--   0 runner    (1001) docker     (121)      888 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/src/tesla_ce_client/vle/course/activity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14344 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/src/tesla_ce_client/vle/course/activity/client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-28 18:26:11.491721 tesla-ce-client-0.0.1/src/tesla_ce_client/vle/course/activity/results/
--rw-r--r--   0 runner    (1001) docker     (121)      902 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/src/tesla_ce_client/vle/course/activity/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4767 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/src/tesla_ce_client/vle/course/activity/results/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     4235 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/src/tesla_ce_client/vle/course/client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-28 18:26:11.495721 tesla-ce-client-0.0.1/src/tesla_ce_client/vle/course/learner/
--rw-r--r--   0 runner    (1001) docker     (121)      886 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/src/tesla_ce_client/vle/course/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4704 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/src/tesla_ce_client/vle/course/learner/client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-28 18:26:11.487721 tesla-ce-client-0.0.1/src/tesla_ce_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2825 2021-05-28 18:26:11.000000 tesla-ce-client-0.0.1/src/tesla_ce_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1397 2021-05-28 18:26:11.000000 tesla-ce-client-0.0.1/src/tesla_ce_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-28 18:26:11.000000 tesla-ce-client-0.0.1/src/tesla_ce_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-05-28 18:26:11.000000 tesla-ce-client-0.0.1/src/tesla_ce_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-05-28 18:26:11.000000 tesla-ce-client-0.0.1/src/tesla_ce_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-28 18:26:11.495721 tesla-ce-client-0.0.1/src/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      744 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/src/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-28 18:26:11.495721 tesla-ce-client-0.0.1/src/tests/learners/
--rw-r--r--   0 runner    (1001) docker     (121)      784 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/src/tests/learners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3760 2021-05-28 18:26:05.000000 tesla-ce-client-0.0.1/src/tests/learners/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:56:03.548936 tesla-ce-client-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-25 09:56:03.548936 tesla-ce-client-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 09:56:03.548936 tesla-ce-client-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:56:03.544935 tesla-ce-client-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:56:03.544935 tesla-ce-client-0.0.3/src/tesla_ce_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9219 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:56:03.544935 tesla-ce-client-0.0.3/src/tesla_ce_client/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 09:56:03.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/data/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:56:03.544935 tesla-ce-client-0.0.3/src/tesla_ce_client/institution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/institution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:56:03.544935 tesla-ce-client-0.0.3/src/tesla_ce_client/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/provider/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11185 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/provider/enrolment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/provider/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/provider/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:56:03.544935 tesla-ce-client-0.0.3/src/tesla_ce_client/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/v1/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/v1/rt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/v1/tep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/v1/tip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/v1/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:56:03.548936 tesla-ce-client-0.0.3/src/tesla_ce_client/vle/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/vle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/vle/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:56:03.548936 tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:56:03.548936 tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/activity/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/activity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14344 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/activity/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:56:03.548936 tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/activity/results/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/activity/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/activity/results/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:56:03.548936 tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/learner/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/learner/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:56:03.544935 tesla-ce-client-0.0.3/src/tesla_ce_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-25 09:56:03.000000 tesla-ce-client-0.0.3/src/tesla_ce_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-25 09:56:03.000000 tesla-ce-client-0.0.3/src/tesla_ce_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 09:56:03.000000 tesla-ce-client-0.0.3/src/tesla_ce_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-25 09:56:03.000000 tesla-ce-client-0.0.3/src/tesla_ce_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 09:56:03.000000 tesla-ce-client-0.0.3/src/tesla_ce_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:56:03.548936 tesla-ce-client-0.0.3/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:56:03.548936 tesla-ce-client-0.0.3/src/tests/learners/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tests/learners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tests/learners/test_client.py
```

### Comparing `tesla-ce-client-0.0.1/LICENSE` & `tesla-ce-client-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.1/PKG-INFO` & `tesla-ce-client-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 Metadata-Version: 2.1
 Name: tesla-ce-client
-Version: 0.0.1
+Version: 0.0.3
 Summary: TeSLA CE Client for Python
-Home-page: https://github.com/tesla-ce/python-client
+Home-page: https://tesla-ce.github.io
 Author: Xavier Baro
 Author-email: xbaro@uoc.edu
 License: UNKNOWN
-Project-URL: Documentation, https://tesla-ce.github.io
+Project-URL: Documentation, https://tesla-ce.github.io/python-client/
 Project-URL: Source, https://github.com/tesla-ce/python-client
-Description: [![PyPi Version](https://img.shields.io/pypi/v/tesla-ce-client.svg)](https://pypi.python.org/pypi/tesla-ce-client/)
-        [![codecov](https://codecov.io/gh/tesla-ce/python-client/branch/main/graph/badge.svg?token=PJJQMW981P)](https://codecov.io/gh/tesla-ce/python-client)
-        [![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)  
-        [![Quality gate](https://sonar.sunai.uoc.edu/api/project_badges/quality_gate?project=tesla-ce_python-client)](https://sonar.sunai.uoc.edu/dashboard?id=tesla-ce_python-client)
-        # TeSLA CE Python Client
-        
-        | :warning: This repository is **under construction**. Final release of TeSLA Community Edition source code is expected by the **end of 2021** |
-        | --- |
-        
-        ## Description
-        Description: A description of your project follows. A good description is clear, short, and to the point. Describe the importance of your project, and what it does.
-        
-        ## Installation
-        Installation: Installation is the next section in an effective README. Tell other users how to install your project locally. Optionally, include a gif to make the process even more clear for other people.
-        
-        ## Usage
-        Usage: The next section is usage, in which you instruct other people on how to use your project after they’ve installed it. This would also be a good place to include screenshots of your project in action.
-        
-        ## Contributing
-        Contributing: Larger projects often have sections on contributing to their project, in which contribution instructions are outlined. Sometimes, this is a separate file. If you have specific contribution preferences, explain them so that other developers know how to best contribute to your work. To learn more about how to help others contribute, check out the guide for setting guidelines for repository contributors.
-        
-        ## Credits
-        Credits: Include a section for credits in order to highlight and link to the authors of your project.
-        
-        ## License
-        This project is licensed under [AGPL v3 licence](http://www.gnu.org/licenses/agpl-3.0).
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPi Version](https://img.shields.io/pypi/v/tesla-ce-client.svg)](https://pypi.python.org/pypi/tesla-ce-client/)
+[![codecov](https://codecov.io/gh/tesla-ce/python-client/branch/main/graph/badge.svg?token=PJJQMW981P)](https://codecov.io/gh/tesla-ce/python-client)
+[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)  
+[![Quality gate](https://sonar.sunai.uoc.edu/api/project_badges/quality_gate?project=tesla-ce_python-client)](https://sonar.sunai.uoc.edu/dashboard?id=tesla-ce_python-client)
+# TeSLA CE Python Client
+
+| :warning: This repository is **under construction**. Final release of TeSLA Community Edition source code is expected by the **end of 2021** |
+| --- |
+
+## Description
+Description: A description of your project follows. A good description is clear, short, and to the point. Describe the importance of your project, and what it does.
+
+## Installation
+Installation: Installation is the next section in an effective README. Tell other users how to install your project locally. Optionally, include a gif to make the process even more clear for other people.
+
+## Usage
+Usage: The next section is usage, in which you instruct other people on how to use your project after they’ve installed it. This would also be a good place to include screenshots of your project in action.
+
+## Contributing
+Contributing: Larger projects often have sections on contributing to their project, in which contribution instructions are outlined. Sometimes, this is a separate file. If you have specific contribution preferences, explain them so that other developers know how to best contribute to your work. To learn more about how to help others contribute, check out the guide for setting guidelines for repository contributors.
+
+## Credits
+Credits: Include a section for credits in order to highlight and link to the authors of your project.
+
+## License
+This project is licensed under [AGPL v3 licence](http://www.gnu.org/licenses/agpl-3.0).
+
+
```

### Comparing `tesla-ce-client-0.0.1/README.md` & `tesla-ce-client-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.1/setup.py` & `tesla-ce-client-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,17 @@
     name="tesla-ce-client",
     version=version,
     author="Xavier Baro",
     author_email="xbaro@uoc.edu",
     description="TeSLA CE Client for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/tesla-ce/python-client",
+    url="https://tesla-ce.github.io",
     project_urls={
-        'Documentation': 'https://tesla-ce.github.io',
+        'Documentation': 'https://tesla-ce.github.io/python-client/',
         'Source': 'https://github.com/tesla-ce/python-client',
     },
     packages=setuptools.find_packages('src', exclude='__pycache__'),
     package_dir={'': 'src'},  # tell distutils packages are under src
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
```

### Comparing `tesla-ce-client-0.0.1/src/tesla_ce_client/__init__.py` & `tesla-ce-client-0.0.3/src/tesla_ce_client/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,7 +11,9 @@
 #      GNU Affero General Public License for more details.
 #
 #      You should have received a copy of the GNU Affero General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """ TeSLA CE CLient package """
 from .client import Client
 from . import exception
+
+__all__ = ['Client', 'exception']
```

### Comparing `tesla-ce-client-0.0.1/src/tesla_ce_client/client.py` & `tesla-ce-client-0.0.3/src/tesla_ce_client/client.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.1/src/tesla_ce_client/connector.py` & `tesla-ce-client-0.0.3/src/tesla_ce_client/connector.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.1/src/tesla_ce_client/exception.py` & `tesla-ce-client-0.0.3/src/tesla_ce_client/exception.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.1/src/tesla_ce_client/provider/__init__.py` & `tesla-ce-client-0.0.3/src/tesla_ce_client/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.1/src/tesla_ce_client/provider/client.py` & `tesla-ce-client-0.0.3/src/tesla_ce_client/provider/client.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.1/src/tesla_ce_client/provider/enrolment.py` & `tesla-ce-client-0.0.3/src/tesla_ce_client/provider/enrolment.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             :type task_id: str
             :return: Learner model
             :rtype: dict
         """
         try:
             return self._connector.post('/api/v2/provider/{}/enrolment/'.format(provider_id),
                                         body={
-                                            'learner_id': learner_id,
+                                            'learner_id': str(learner_id),
                                             'task_id': task_id
                                         })
         except exception.BadRequestException as exc:
             if 'Model is locked' in exc.value:
                 raise exception.LockedResourceException("Model is locked")
 
     def get_model(self, provider_id, learner_id):
@@ -74,28 +74,28 @@
             :param provider_id: Provider ID
             :type provider_id: int
             :param learner_id: The learner UUID
             :type learner_id: str
             :return: Learner model
             :rtype: dict
         """
-        return self._connector.get('/api/v2/provider/{}/enrolment/{}/'.format(provider_id, learner_id))
+        return self._connector.get('/api/v2/provider/{}/enrolment/{}/'.format(provider_id, str(learner_id)))
 
     def unlock_model(self, provider_id, learner_id, task_id):
         """
             Unlock the learner model for a provider.
 
             :param provider_id: Provider ID
             :type provider_id: int
             :param learner_id: The learner UUID
             :type learner_id: str
             :param task_id: Task UUID value. It will allow to update the model.
             :type task_id: str
         """
-        self._connector.post('/api/v2/provider/{}/enrolment/{}/unlock/'.format(provider_id, learner_id),
+        self._connector.post('/api/v2/provider/{}/enrolment/{}/unlock/'.format(provider_id, str(learner_id)),
                              body={
                                  'token': task_id
                              })
 
     def save_model(self, provider_id, learner_id, task_id, model):
         """
             Get learner model for a provider ready to be modified.
@@ -117,15 +117,15 @@
             else:
                 resp = requests.post(model['model_upload_url']['url'], data=model['model_upload_url']['fields'],
                                      files={'file': io.StringIO(simplejson.dumps(model['model']))})
 
             # Check given response
             self._connector._check_response_status(resp.status_code, resp.content)
 
-            return self._connector.put('/api/v2/provider/{}/enrolment/{}/'.format(provider_id, learner_id),
+            return self._connector.put('/api/v2/provider/{}/enrolment/{}/'.format(provider_id, str(learner_id)),
                                         body={
                                             'learner_id': learner_id,
                                             'task_id': task_id,
                                             'percentage': model['percentage'],
                                             'can_analyse': model['can_analyse'],
                                             'used_samples': model['used_samples']
                                         })
@@ -143,15 +143,15 @@
             :type learner_id: str
             :param sample_id: Sample id
             :type sample_id: int
             :return: Enrolment sample
             :rtype: dict
         """
         return self._connector.get('/api/v2/provider/{}/enrolment/{}/sample/{}/'.format(provider_id,
-                                                                                        learner_id,
+                                                                                        str(learner_id),
                                                                                         sample_id))
 
     def get_sample_validation(self, provider_id, learner_id, sample_id, validation_id):
         """
             Get validation result for an enrolment sample
 
             :param provider_id: Provider ID
@@ -162,15 +162,15 @@
             :type sample_id: int
             :param validation_id: Sample validation id
             :type validation_id: int
             :param result: Validation result
             :type result: dict
         """
         return self._connector.get('/api/v2/provider/{}/enrolment/{}/sample/{}/validation/{}/'.format(
-            provider_id, learner_id, sample_id, validation_id))
+            provider_id, str(learner_id), sample_id, validation_id))
 
     def set_sample_validation(self, provider_id, learner_id, sample_id, validation_id, result):
         """
             Store validation result for an enrolment sample
 
             :param provider_id: Provider ID
             :type provider_id: int
@@ -180,15 +180,15 @@
             :type sample_id: int
             :param validation_id: Sample Validation id
             :type validation_id: int
             :param result: Validation result
             :type result: dict
         """
         return self._connector.put('/api/v2/provider/{}/enrolment/{}/sample/{}/validation/{}/'.format(
-            provider_id, learner_id, sample_id, validation_id), body=result)
+            provider_id, str(learner_id), sample_id, validation_id), body=result)
 
     def get_sample_validation_list(self, provider_id, learner_id, sample_id):
         """
             Get validation result for an enrolment sample
 
             :param provider_id: Provider ID
             :type provider_id: int
@@ -196,43 +196,43 @@
             :type learner_id: str
             :param sample_id: Sample id
             :type sample_id: int
             :param result: Validation results
             :type result: dict
         """
         return self._connector.get('/api/v2/provider/{}/enrolment/{}/sample/{}/validation/'.format(
-            provider_id, learner_id, sample_id))
+            provider_id, str(learner_id), sample_id))
 
     def get_model_samples(self, provider_id, learner_id):
         """
             Get the list of enrolment samples used in current model
 
             :param provider_id: Provider ID
             :type provider_id: int
             :param learner_id: The learner UUID
             :type learner_id: str
             :param result: Enrolment samples
             :type result: dict
         """
         return self._connector.get('/api/v2/provider/{}/enrolment/{}/used_samples/'.format(
-            provider_id, learner_id))
+            provider_id, str(learner_id)))
 
     def get_available_samples(self, provider_id, learner_id):
         """
             Get the list of available validated enrolment samples that are not used in current model
 
             :param provider_id: Provider ID
             :type provider_id: int
             :param learner_id: The learner UUID
             :type learner_id: str
             :param result: Enrolment samples
             :type result: dict
         """
         return self._connector.get('/api/v2/provider/{}/enrolment/{}/available_samples/'.format(
-            provider_id, learner_id))
+            provider_id, str(learner_id)))
 
     def set_sample_validation_status(self, provider_id, learner_id, sample_id, validation_id, status):
         """
             Change sample validation status
 
             :param provider_id: Provider ID
             :type provider_id: int
@@ -245,15 +245,15 @@
             :param status: Sample's status. Valid status: 0 validating, 1 valid, 2 error, 3 timeout, 4 waiting external
             service
             :type status: SampleValidationStatus
 
             :return:
         """
         return self._connector.post('/api/v2/provider/{}/enrolment/{}/sample/{}/validation/{}/status/'.format(
-            provider_id, learner_id, sample_id, validation_id), body={"status": status.value})
+            provider_id, str(learner_id), sample_id, validation_id), body={"status": status.value})
 
     def set_sample_status(self, provider_id, learner_id, sample_id, status):
         """
             Change sample status
 
             :param provider_id: Provider ID
             :type provider_id: int
```

### Comparing `tesla-ce-client-0.0.1/src/tesla_ce_client/provider/notification.py` & `tesla-ce-client-0.0.3/src/tesla_ce_client/provider/notification.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.1/src/tesla_ce_client/provider/verification.py` & `tesla-ce-client-0.0.3/src/tesla_ce_client/provider/verification.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.1/src/tesla_ce_client/v1/__init__.py` & `tesla-ce-client-0.0.3/src/tesla_ce_client/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.1/src/tesla_ce_client/v1/api.py` & `tesla-ce-client-0.0.3/src/tesla_ce_client/v1/api.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.1/src/tesla_ce_client/v1/rt.py` & `tesla-ce-client-0.0.3/src/tesla_ce_client/v1/rt.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.1/src/tesla_ce_client/v1/tep.py` & `tesla-ce-client-0.0.3/src/tesla_ce_client/v1/tep.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.1/src/tesla_ce_client/v1/tip.py` & `tesla-ce-client-0.0.3/src/tesla_ce_client/v1/tip.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.1/src/tesla_ce_client/v1/v1.py` & `tesla-ce-client-0.0.3/src/tesla_ce_client/v1/v1.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.1/src/tesla_ce_client/vle/__init__.py` & `tesla-ce-client-0.0.3/src/tesla_ce_client/vle/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.1/src/tesla_ce_client/vle/client.py` & `tesla-ce-client-0.0.3/src/tesla_ce_client/vle/client.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.1/src/tesla_ce_client/vle/course/__init__.py` & `tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.1/src/tesla_ce_client/vle/course/activity/__init__.py` & `tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/activity/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.1/src/tesla_ce_client/vle/course/activity/client.py` & `tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/activity/client.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.1/src/tesla_ce_client/vle/course/activity/results/__init__.py` & `tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/activity/results/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.1/src/tesla_ce_client/vle/course/activity/results/client.py` & `tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/activity/results/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,16 +89,16 @@
         """
         if vle_id is None:
             vle_id = self._connector.get_vle_id()
         if instrument is None:
             return self._connector.get('api/v2/vle/{}/course/{}/activity/{}/learner/{}/request/'.format(vle_id,
                                                                                                         course_id,
                                                                                                         activity_id,
-                                                                                                        learner_id)
+                                                                                                        str(learner_id))
                                        )
         return self._connector.get('api/v2/vle/{}/course/{}/activity/{}/learner/{}/request/?instruments={}'.format(
             vle_id,
             course_id,
             activity_id,
-            learner_id,
+            str(learner_id),
             instrument)
         )
```

### Comparing `tesla-ce-client-0.0.1/src/tesla_ce_client/vle/course/client.py` & `tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/client.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.1/src/tesla_ce_client/vle/course/learner/__init__.py` & `tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/learner/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.1/src/tesla_ce_client/vle/course/learner/client.py` & `tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/learner/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             :param vle_id: Identifier of the vle. If not provided take it from module configuration
             :type vle_id: int
             :return: List of activities
             :rtype: list
         """
         if vle_id is None:
             vle_id = self._connector.get_vle_id()
-        return self._connector.get('api/v2/vle/{}/course/{}/activity/{}/'.format(vle_id, course_id, learner_id))
+        return self._connector.get('api/v2/vle/{}/course/{}/activity/{}/'.format(vle_id, course_id, str(learner_id)))
 
     def find_by_uid(self, course_id, uid, vle_id=None):
         """
             Get a learner
 
             :param course_id: Identifier of the course
             :type course_id: int
@@ -121,15 +121,15 @@
             :type vle_id: int
             :return: Learner data
             :rtype: dict
         """
         if vle_id is None:
             vle_id = self._connector.get_vle_id()
         result = self._connector.get('api/v2/vle/{}/course/{}/learner/?lerner_id={}'.format(
-            vle_id, course_id, learner_id)
+            vle_id, course_id, str(learner_id))
         )
 
         if result['count'] == 1:
             return result['results'][0]
 
         return None
```

### Comparing `tesla-ce-client-0.0.1/src/tesla_ce_client.egg-info/PKG-INFO` & `tesla-ce-client-0.0.3/src/tesla_ce_client.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 Metadata-Version: 2.1
 Name: tesla-ce-client
-Version: 0.0.1
+Version: 0.0.3
 Summary: TeSLA CE Client for Python
-Home-page: https://github.com/tesla-ce/python-client
+Home-page: https://tesla-ce.github.io
 Author: Xavier Baro
 Author-email: xbaro@uoc.edu
 License: UNKNOWN
-Project-URL: Documentation, https://tesla-ce.github.io
+Project-URL: Documentation, https://tesla-ce.github.io/python-client/
 Project-URL: Source, https://github.com/tesla-ce/python-client
-Description: [![PyPi Version](https://img.shields.io/pypi/v/tesla-ce-client.svg)](https://pypi.python.org/pypi/tesla-ce-client/)
-        [![codecov](https://codecov.io/gh/tesla-ce/python-client/branch/main/graph/badge.svg?token=PJJQMW981P)](https://codecov.io/gh/tesla-ce/python-client)
-        [![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)  
-        [![Quality gate](https://sonar.sunai.uoc.edu/api/project_badges/quality_gate?project=tesla-ce_python-client)](https://sonar.sunai.uoc.edu/dashboard?id=tesla-ce_python-client)
-        # TeSLA CE Python Client
-        
-        | :warning: This repository is **under construction**. Final release of TeSLA Community Edition source code is expected by the **end of 2021** |
-        | --- |
-        
-        ## Description
-        Description: A description of your project follows. A good description is clear, short, and to the point. Describe the importance of your project, and what it does.
-        
-        ## Installation
-        Installation: Installation is the next section in an effective README. Tell other users how to install your project locally. Optionally, include a gif to make the process even more clear for other people.
-        
-        ## Usage
-        Usage: The next section is usage, in which you instruct other people on how to use your project after they’ve installed it. This would also be a good place to include screenshots of your project in action.
-        
-        ## Contributing
-        Contributing: Larger projects often have sections on contributing to their project, in which contribution instructions are outlined. Sometimes, this is a separate file. If you have specific contribution preferences, explain them so that other developers know how to best contribute to your work. To learn more about how to help others contribute, check out the guide for setting guidelines for repository contributors.
-        
-        ## Credits
-        Credits: Include a section for credits in order to highlight and link to the authors of your project.
-        
-        ## License
-        This project is licensed under [AGPL v3 licence](http://www.gnu.org/licenses/agpl-3.0).
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPi Version](https://img.shields.io/pypi/v/tesla-ce-client.svg)](https://pypi.python.org/pypi/tesla-ce-client/)
+[![codecov](https://codecov.io/gh/tesla-ce/python-client/branch/main/graph/badge.svg?token=PJJQMW981P)](https://codecov.io/gh/tesla-ce/python-client)
+[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)  
+[![Quality gate](https://sonar.sunai.uoc.edu/api/project_badges/quality_gate?project=tesla-ce_python-client)](https://sonar.sunai.uoc.edu/dashboard?id=tesla-ce_python-client)
+# TeSLA CE Python Client
+
+| :warning: This repository is **under construction**. Final release of TeSLA Community Edition source code is expected by the **end of 2021** |
+| --- |
+
+## Description
+Description: A description of your project follows. A good description is clear, short, and to the point. Describe the importance of your project, and what it does.
+
+## Installation
+Installation: Installation is the next section in an effective README. Tell other users how to install your project locally. Optionally, include a gif to make the process even more clear for other people.
+
+## Usage
+Usage: The next section is usage, in which you instruct other people on how to use your project after they’ve installed it. This would also be a good place to include screenshots of your project in action.
+
+## Contributing
+Contributing: Larger projects often have sections on contributing to their project, in which contribution instructions are outlined. Sometimes, this is a separate file. If you have specific contribution preferences, explain them so that other developers know how to best contribute to your work. To learn more about how to help others contribute, check out the guide for setting guidelines for repository contributors.
+
+## Credits
+Credits: Include a section for credits in order to highlight and link to the authors of your project.
+
+## License
+This project is licensed under [AGPL v3 licence](http://www.gnu.org/licenses/agpl-3.0).
+
+
```

### Comparing `tesla-ce-client-0.0.1/src/tesla_ce_client.egg-info/SOURCES.txt` & `tesla-ce-client-0.0.3/src/tesla_ce_client.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 src/tesla_ce_client/connector.py
 src/tesla_ce_client/exception.py
 src/tesla_ce_client.egg-info/PKG-INFO
 src/tesla_ce_client.egg-info/SOURCES.txt
 src/tesla_ce_client.egg-info/dependency_links.txt
 src/tesla_ce_client.egg-info/requires.txt
 src/tesla_ce_client.egg-info/top_level.txt
+src/tesla_ce_client/data/VERSION
 src/tesla_ce_client/institution/__init__.py
 src/tesla_ce_client/provider/__init__.py
 src/tesla_ce_client/provider/client.py
 src/tesla_ce_client/provider/enrolment.py
 src/tesla_ce_client/provider/notification.py
 src/tesla_ce_client/provider/verification.py
 src/tesla_ce_client/v1/__init__.py
```

### Comparing `tesla-ce-client-0.0.1/src/tests/__init__.py` & `tesla-ce-client-0.0.3/src/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.1/src/tests/learners/__init__.py` & `tesla-ce-client-0.0.3/src/tests/learners/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.1/src/tests/learners/test_client.py` & `tesla-ce-client-0.0.3/src/tests/learners/test_client.py`

 * *Files identical despite different names*

