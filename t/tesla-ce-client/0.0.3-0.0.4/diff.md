# Comparing `tmp/tesla-ce-client-0.0.3.tar.gz` & `tmp/tesla-ce-client-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tesla-ce-client-0.0.3.tar", last modified: Tue Jul 25 09:56:03 2023, max compression
+gzip compressed data, was "tesla-ce-client-0.0.4.tar", last modified: Tue Jul 25 10:40:42 2023, max compression
```

## Comparing `tesla-ce-client-0.0.3.tar` & `tesla-ce-client-0.0.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:56:03.548936 tesla-ce-client-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-25 09:56:03.548936 tesla-ce-client-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 09:56:03.548936 tesla-ce-client-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:56:03.544935 tesla-ce-client-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:56:03.544935 tesla-ce-client-0.0.3/src/tesla_ce_client/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9219 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:56:03.544935 tesla-ce-client-0.0.3/src/tesla_ce_client/data/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 09:56:03.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/data/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:56:03.544935 tesla-ce-client-0.0.3/src/tesla_ce_client/institution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/institution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:56:03.544935 tesla-ce-client-0.0.3/src/tesla_ce_client/provider/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/provider/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11185 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/provider/enrolment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/provider/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/provider/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:56:03.544935 tesla-ce-client-0.0.3/src/tesla_ce_client/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/v1/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/v1/rt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/v1/tep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/v1/tip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/v1/v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:56:03.548936 tesla-ce-client-0.0.3/src/tesla_ce_client/vle/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/vle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/vle/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:56:03.548936 tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:56:03.548936 tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/activity/
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/activity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14344 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/activity/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:56:03.548936 tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/activity/results/
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/activity/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/activity/results/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:56:03.548936 tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/learner/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/learner/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:56:03.544935 tesla-ce-client-0.0.3/src/tesla_ce_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-25 09:56:03.000000 tesla-ce-client-0.0.3/src/tesla_ce_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-25 09:56:03.000000 tesla-ce-client-0.0.3/src/tesla_ce_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 09:56:03.000000 tesla-ce-client-0.0.3/src/tesla_ce_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-25 09:56:03.000000 tesla-ce-client-0.0.3/src/tesla_ce_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 09:56:03.000000 tesla-ce-client-0.0.3/src/tesla_ce_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:56:03.548936 tesla-ce-client-0.0.3/src/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:56:03.548936 tesla-ce-client-0.0.3/src/tests/learners/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tests/learners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-07-25 09:55:54.000000 tesla-ce-client-0.0.3/src/tests/learners/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.631433 tesla-ce-client-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-25 10:40:42.631433 tesla-ce-client-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 10:40:42.631433 tesla-ce-client-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.627433 tesla-ce-client-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.631433 tesla-ce-client-0.0.4/src/tesla_ce_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/src/tesla_ce_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/src/tesla_ce_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9219 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/src/tesla_ce_client/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.631433 tesla-ce-client-0.0.4/src/tesla_ce_client/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 10:40:42.000000 tesla-ce-client-0.0.4/src/tesla_ce_client/data/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/src/tesla_ce_client/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.631433 tesla-ce-client-0.0.4/src/tesla_ce_client/institution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/src/tesla_ce_client/institution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.631433 tesla-ce-client-0.0.4/src/tesla_ce_client/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/src/tesla_ce_client/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/src/tesla_ce_client/provider/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/src/tesla_ce_client/provider/enrolment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/src/tesla_ce_client/provider/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/src/tesla_ce_client/provider/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.631433 tesla-ce-client-0.0.4/src/tesla_ce_client/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/src/tesla_ce_client/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/src/tesla_ce_client/v1/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/src/tesla_ce_client/v1/rt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/src/tesla_ce_client/v1/tep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/src/tesla_ce_client/v1/tip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/src/tesla_ce_client/v1/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.631433 tesla-ce-client-0.0.4/src/tesla_ce_client/vle/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/src/tesla_ce_client/vle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/src/tesla_ce_client/vle/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.631433 tesla-ce-client-0.0.4/src/tesla_ce_client/vle/course/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/src/tesla_ce_client/vle/course/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.631433 tesla-ce-client-0.0.4/src/tesla_ce_client/vle/course/activity/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/src/tesla_ce_client/vle/course/activity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14344 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/src/tesla_ce_client/vle/course/activity/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.631433 tesla-ce-client-0.0.4/src/tesla_ce_client/vle/course/activity/results/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/src/tesla_ce_client/vle/course/activity/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/src/tesla_ce_client/vle/course/activity/results/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/src/tesla_ce_client/vle/course/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.631433 tesla-ce-client-0.0.4/src/tesla_ce_client/vle/course/learner/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/src/tesla_ce_client/vle/course/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/src/tesla_ce_client/vle/course/learner/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.631433 tesla-ce-client-0.0.4/src/tesla_ce_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-25 10:40:42.000000 tesla-ce-client-0.0.4/src/tesla_ce_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-25 10:40:42.000000 tesla-ce-client-0.0.4/src/tesla_ce_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 10:40:42.000000 tesla-ce-client-0.0.4/src/tesla_ce_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-25 10:40:42.000000 tesla-ce-client-0.0.4/src/tesla_ce_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 10:40:42.000000 tesla-ce-client-0.0.4/src/tesla_ce_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.631433 tesla-ce-client-0.0.4/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/src/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.631433 tesla-ce-client-0.0.4/src/tests/learners/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/src/tests/learners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-07-25 10:40:36.000000 tesla-ce-client-0.0.4/src/tests/learners/test_client.py
```

### Comparing `tesla-ce-client-0.0.3/LICENSE` & `tesla-ce-client-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.3/PKG-INFO` & `tesla-ce-client-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tesla-ce-client
-Version: 0.0.3
+Version: 0.0.4
 Summary: TeSLA CE Client for Python
 Home-page: https://tesla-ce.github.io
 Author: Xavier Baro
 Author-email: xbaro@uoc.edu
 License: UNKNOWN
 Project-URL: Documentation, https://tesla-ce.github.io/python-client/
 Project-URL: Source, https://github.com/tesla-ce/python-client
```

### Comparing `tesla-ce-client-0.0.3/README.md` & `tesla-ce-client-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.3/setup.py` & `tesla-ce-client-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.3/src/tesla_ce_client/__init__.py` & `tesla-ce-client-0.0.4/src/tesla_ce_client/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.3/src/tesla_ce_client/client.py` & `tesla-ce-client-0.0.4/src/tesla_ce_client/client.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.3/src/tesla_ce_client/connector.py` & `tesla-ce-client-0.0.4/src/tesla_ce_client/connector.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.3/src/tesla_ce_client/exception.py` & `tesla-ce-client-0.0.4/src/tesla_ce_client/exception.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.3/src/tesla_ce_client/provider/__init__.py` & `tesla-ce-client-0.0.4/src/tesla_ce_client/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.3/src/tesla_ce_client/provider/client.py` & `tesla-ce-client-0.0.4/src/tesla_ce_client/provider/client.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.3/src/tesla_ce_client/provider/enrolment.py` & `tesla-ce-client-0.0.4/src/tesla_ce_client/provider/enrolment.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
                                      files={'file': io.StringIO(simplejson.dumps(model['model']))})
 
             # Check given response
             self._connector._check_response_status(resp.status_code, resp.content)
 
             return self._connector.put('/api/v2/provider/{}/enrolment/{}/'.format(provider_id, str(learner_id)),
                                         body={
-                                            'learner_id': learner_id,
+                                            'learner_id': str(learner_id),
                                             'task_id': task_id,
                                             'percentage': model['percentage'],
                                             'can_analyse': model['can_analyse'],
                                             'used_samples': model['used_samples']
                                         })
         except exception.BadRequestException as exc:
             if 'Model is locked' in exc.value:
```

### Comparing `tesla-ce-client-0.0.3/src/tesla_ce_client/provider/notification.py` & `tesla-ce-client-0.0.4/src/tesla_ce_client/provider/notification.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.3/src/tesla_ce_client/provider/verification.py` & `tesla-ce-client-0.0.4/src/tesla_ce_client/provider/verification.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.3/src/tesla_ce_client/v1/__init__.py` & `tesla-ce-client-0.0.4/src/tesla_ce_client/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.3/src/tesla_ce_client/v1/api.py` & `tesla-ce-client-0.0.4/src/tesla_ce_client/v1/api.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.3/src/tesla_ce_client/v1/rt.py` & `tesla-ce-client-0.0.4/src/tesla_ce_client/v1/rt.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.3/src/tesla_ce_client/v1/tep.py` & `tesla-ce-client-0.0.4/src/tesla_ce_client/v1/tep.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.3/src/tesla_ce_client/v1/tip.py` & `tesla-ce-client-0.0.4/src/tesla_ce_client/v1/tip.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.3/src/tesla_ce_client/v1/v1.py` & `tesla-ce-client-0.0.4/src/tesla_ce_client/v1/v1.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.3/src/tesla_ce_client/vle/__init__.py` & `tesla-ce-client-0.0.4/src/tesla_ce_client/vle/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.3/src/tesla_ce_client/vle/client.py` & `tesla-ce-client-0.0.4/src/tesla_ce_client/vle/client.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/__init__.py` & `tesla-ce-client-0.0.4/src/tesla_ce_client/vle/course/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/activity/__init__.py` & `tesla-ce-client-0.0.4/src/tesla_ce_client/vle/course/activity/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/activity/client.py` & `tesla-ce-client-0.0.4/src/tesla_ce_client/vle/course/activity/client.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/activity/results/__init__.py` & `tesla-ce-client-0.0.4/src/tesla_ce_client/vle/course/activity/results/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/activity/results/client.py` & `tesla-ce-client-0.0.4/src/tesla_ce_client/vle/course/activity/results/client.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/client.py` & `tesla-ce-client-0.0.4/src/tesla_ce_client/vle/course/client.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/learner/__init__.py` & `tesla-ce-client-0.0.4/src/tesla_ce_client/vle/course/learner/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.3/src/tesla_ce_client/vle/course/learner/client.py` & `tesla-ce-client-0.0.4/src/tesla_ce_client/vle/course/learner/client.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.3/src/tesla_ce_client.egg-info/PKG-INFO` & `tesla-ce-client-0.0.4/src/tesla_ce_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tesla-ce-client
-Version: 0.0.3
+Version: 0.0.4
 Summary: TeSLA CE Client for Python
 Home-page: https://tesla-ce.github.io
 Author: Xavier Baro
 Author-email: xbaro@uoc.edu
 License: UNKNOWN
 Project-URL: Documentation, https://tesla-ce.github.io/python-client/
 Project-URL: Source, https://github.com/tesla-ce/python-client
```

### Comparing `tesla-ce-client-0.0.3/src/tesla_ce_client.egg-info/SOURCES.txt` & `tesla-ce-client-0.0.4/src/tesla_ce_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.3/src/tests/__init__.py` & `tesla-ce-client-0.0.4/src/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.3/src/tests/learners/__init__.py` & `tesla-ce-client-0.0.4/src/tests/learners/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-client-0.0.3/src/tests/learners/test_client.py` & `tesla-ce-client-0.0.4/src/tests/learners/test_client.py`

 * *Files identical despite different names*

