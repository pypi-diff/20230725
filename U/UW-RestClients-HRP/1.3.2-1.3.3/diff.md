# Comparing `tmp/UW-RestClients-HRP-1.3.2.tar.gz` & `tmp/UW-RestClients-HRP-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UW-RestClients-HRP-1.3.2.tar", last modified: Thu May  4 22:01:06 2023, max compression
+gzip compressed data, was "UW-RestClients-HRP-1.3.3.tar", last modified: Tue Jul 25 16:25:21 2023, max compression
```

## Comparing `UW-RestClients-HRP-1.3.2.tar` & `UW-RestClients-HRP-1.3.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:01:06.160029 UW-RestClients-HRP-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      652 2023-05-04 22:01:06.160029 UW-RestClients-HRP-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      895 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:01:06.160029 UW-RestClients-HRP-1.3.2/UW_RestClients_HRP.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      652 2023-05-04 22:01:05.000000 UW-RestClients-HRP-1.3.2/UW_RestClients_HRP.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-05-04 22:01:06.000000 UW-RestClients-HRP-1.3.2/UW_RestClients_HRP.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 22:01:05.000000 UW-RestClients-HRP-1.3.2/UW_RestClients_HRP.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-05-04 22:01:05.000000 UW-RestClients-HRP-1.3.2/UW_RestClients_HRP.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-04 22:01:05.000000 UW-RestClients-HRP-1.3.2/UW_RestClients_HRP.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-04 22:01:06.160029 UW-RestClients-HRP-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:01:06.160029 UW-RestClients-HRP-1.3.2/uw_hrp/
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-04 22:01:04.000000 UW-RestClients-HRP-1.3.2/uw_hrp/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)     3652 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      452 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/dao.py
--rw-r--r--   0 runner    (1001) docker     (122)    11430 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:01:06.156029 UW-RestClients-HRP-1.3.2/uw_hrp/resources/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:01:06.156029 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:01:06.156029 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:01:06.156029 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:01:06.156029 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v1/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:01:06.160029 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v1/appointee/
--rw-r--r--   0 runner    (1001) docker     (122)     4837 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v1/appointee/123456789.json
--rw-r--r--   0 runner    (1001) docker     (122)     4837 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v1/appointee/9136CCB8F66711D5BE060004AC494FFE.json
--rw-r--r--   0 runner    (1001) docker     (122)     4837 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v1/appointee/javerage.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:01:06.160029 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/
--rw-r--r--   0 runner    (1001) docker     (122)      358 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/Worker.json_changed_since_2019_page_size_200_page_start_2
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:01:06.160029 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker/
--rw-r--r--   0 runner    (1001) docker     (122)    10331 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker/10000000000000000000000000000015.json
--rw-r--r--   0 runner    (1001) docker     (122)    10331 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker/10000000000000000000000000000015.json_workerpositionstate_current_future
--rw-r--r--   0 runner    (1001) docker     (122)    10331 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker/100000015.json
--rw-r--r--   0 runner    (1001) docker     (122)    10331 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker/100000015.json_workerpositionstate_current_future
--rw-r--r--   0 runner    (1001) docker     (122)    10331 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker/chair.json
--rw-r--r--   0 runner    (1001) docker     (122)     8018 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker/faculty.json
--rw-r--r--   0 runner    (1001) docker     (122)     8018 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker/faculty.json_workerpositionstate_current_future
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker.json_changed_since_2019_page_size_200
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker.json_changed_since_2020_page_size_200
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:01:06.160029 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v3/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:01:06.160029 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v3/person/
--rw-r--r--   0 runner    (1001) docker     (122)    40857 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v3/person/000000005.json
--rw-r--r--   0 runner    (1001) docker     (122)    44463 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v3/person/9136CCB8F66711D5BE060004AC494FFE.json
--rw-r--r--   0 runner    (1001) docker     (122)    40857 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v3/person/faculty.json
--rw-r--r--   0 runner    (1001) docker     (122)    40857 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v3/person/faculty.json_future_worker_true
--rw-r--r--   0 runner    (1001) docker     (122)    27656 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v3/person.json_changed_since_date_2022-12-12_page_size_200
--rw-r--r--   0 runner    (1001) docker     (122)      463 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:01:06.160029 UW-RestClients-HRP-1.3.2/uw_hrp/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      388 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/tests/test_dao.py
--rw-r--r--   0 runner    (1001) docker     (122)     5019 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/tests/test_hrp.py
--rw-r--r--   0 runner    (1001) docker     (122)    14785 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/tests/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:01:06.160029 UW-RestClients-HRP-1.3.2/uw_hrp/util/
--rw-r--r--   0 runner    (1001) docker     (122)      215 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 16:25:21.876268 UW-RestClients-HRP-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-07-25 16:25:11.000000 UW-RestClients-HRP-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-07-25 16:25:11.000000 UW-RestClients-HRP-1.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      652 2023-07-25 16:25:21.876268 UW-RestClients-HRP-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      895 2023-07-25 16:25:11.000000 UW-RestClients-HRP-1.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 16:25:21.872268 UW-RestClients-HRP-1.3.3/UW_RestClients_HRP.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      652 2023-07-25 16:25:21.000000 UW-RestClients-HRP-1.3.3/UW_RestClients_HRP.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-07-25 16:25:21.000000 UW-RestClients-HRP-1.3.3/UW_RestClients_HRP.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-25 16:25:21.000000 UW-RestClients-HRP-1.3.3/UW_RestClients_HRP.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-07-25 16:25:21.000000 UW-RestClients-HRP-1.3.3/UW_RestClients_HRP.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-25 16:25:21.000000 UW-RestClients-HRP-1.3.3/UW_RestClients_HRP.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-25 16:25:21.876268 UW-RestClients-HRP-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-07-25 16:25:11.000000 UW-RestClients-HRP-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 16:25:21.872268 UW-RestClients-HRP-1.3.3/uw_hrp/
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-25 16:25:20.000000 UW-RestClients-HRP-1.3.3/uw_hrp/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)     3652 2023-07-25 16:25:11.000000 UW-RestClients-HRP-1.3.3/uw_hrp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      452 2023-07-25 16:25:11.000000 UW-RestClients-HRP-1.3.3/uw_hrp/dao.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11405 2023-07-25 16:25:11.000000 UW-RestClients-HRP-1.3.3/uw_hrp/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 16:25:21.872268 UW-RestClients-HRP-1.3.3/uw_hrp/resources/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 16:25:21.872268 UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 16:25:21.872268 UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 16:25:21.872268 UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 16:25:21.872268 UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v1/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 16:25:21.872268 UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v1/appointee/
+-rw-r--r--   0 runner    (1001) docker     (122)     4837 2023-07-25 16:25:11.000000 UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v1/appointee/123456789.json
+-rw-r--r--   0 runner    (1001) docker     (122)     4837 2023-07-25 16:25:11.000000 UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v1/appointee/9136CCB8F66711D5BE060004AC494FFE.json
+-rw-r--r--   0 runner    (1001) docker     (122)     4837 2023-07-25 16:25:11.000000 UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v1/appointee/javerage.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 16:25:21.876268 UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v2/
+-rw-r--r--   0 runner    (1001) docker     (122)      358 2023-07-25 16:25:11.000000 UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v2/Worker.json_changed_since_2019_page_size_200_page_start_2
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 16:25:21.876268 UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v2/worker/
+-rw-r--r--   0 runner    (1001) docker     (122)    10331 2023-07-25 16:25:11.000000 UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v2/worker/10000000000000000000000000000015.json
+-rw-r--r--   0 runner    (1001) docker     (122)    10331 2023-07-25 16:25:11.000000 UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v2/worker/10000000000000000000000000000015.json_workerpositionstate_current_future
+-rw-r--r--   0 runner    (1001) docker     (122)    10331 2023-07-25 16:25:11.000000 UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v2/worker/100000015.json
+-rw-r--r--   0 runner    (1001) docker     (122)    10331 2023-07-25 16:25:11.000000 UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v2/worker/100000015.json_workerpositionstate_current_future
+-rw-r--r--   0 runner    (1001) docker     (122)    10331 2023-07-25 16:25:11.000000 UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v2/worker/chair.json
+-rw-r--r--   0 runner    (1001) docker     (122)     8018 2023-07-25 16:25:11.000000 UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v2/worker/faculty.json
+-rw-r--r--   0 runner    (1001) docker     (122)     8018 2023-07-25 16:25:11.000000 UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v2/worker/faculty.json_workerpositionstate_current_future
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-07-25 16:25:11.000000 UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v2/worker.json_changed_since_2019_page_size_200
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-25 16:25:11.000000 UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v2/worker.json_changed_since_2020_page_size_200
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 16:25:21.876268 UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v3/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 16:25:21.876268 UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v3/person/
+-rw-r--r--   0 runner    (1001) docker     (122)    41954 2023-07-25 16:25:11.000000 UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v3/person/000000005.json
+-rw-r--r--   0 runner    (1001) docker     (122)    44463 2023-07-25 16:25:11.000000 UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v3/person/9136CCB8F66711D5BE060004AC494FFE.json
+-rw-r--r--   0 runner    (1001) docker     (122)    41954 2023-07-25 16:25:11.000000 UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v3/person/faculty.json
+-rw-r--r--   0 runner    (1001) docker     (122)    41954 2023-07-25 16:25:11.000000 UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v3/person/faculty.json_future_worker_true
+-rw-r--r--   0 runner    (1001) docker     (122)    27656 2023-07-25 16:25:11.000000 UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v3/person.json_changed_since_date_2022-12-12_page_size_200
+-rw-r--r--   0 runner    (1001) docker     (122)      463 2023-07-25 16:25:11.000000 UW-RestClients-HRP-1.3.3/uw_hrp/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 16:25:21.876268 UW-RestClients-HRP-1.3.3/uw_hrp/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-25 16:25:11.000000 UW-RestClients-HRP-1.3.3/uw_hrp/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      388 2023-07-25 16:25:11.000000 UW-RestClients-HRP-1.3.3/uw_hrp/tests/test_dao.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4972 2023-07-25 16:25:11.000000 UW-RestClients-HRP-1.3.3/uw_hrp/tests/test_hrp.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14345 2023-07-25 16:25:11.000000 UW-RestClients-HRP-1.3.3/uw_hrp/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 16:25:21.876268 UW-RestClients-HRP-1.3.3/uw_hrp/util/
+-rw-r--r--   0 runner    (1001) docker     (122)      215 2023-07-25 16:25:11.000000 UW-RestClients-HRP-1.3.3/uw_hrp/util/__init__.py
```

### Comparing `UW-RestClients-HRP-1.3.2/LICENSE` & `UW-RestClients-HRP-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.2/PKG-INFO` & `UW-RestClients-HRP-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: UW-RestClients-HRP
-Version: 1.3.2
+Version: 1.3.3
 Summary: A library for connecting to the UW Human Resources API
 Home-page: https://github.com/uw-it-aca/uw-restclients-hrp
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Description: 
         See the README on `GitHub
```

### Comparing `UW-RestClients-HRP-1.3.2/README.md` & `UW-RestClients-HRP-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.2/UW_RestClients_HRP.egg-info/PKG-INFO` & `UW-RestClients-HRP-1.3.3/UW_RestClients_HRP.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: UW-RestClients-HRP
-Version: 1.3.2
+Version: 1.3.3
 Summary: A library for connecting to the UW Human Resources API
 Home-page: https://github.com/uw-it-aca/uw-restclients-hrp
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Description: 
         See the README on `GitHub
```

### Comparing `UW-RestClients-HRP-1.3.2/UW_RestClients_HRP.egg-info/SOURCES.txt` & `UW-RestClients-HRP-1.3.3/UW_RestClients_HRP.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.2/setup.py` & `UW-RestClients-HRP-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.2/uw_hrp/__init__.py` & `UW-RestClients-HRP-1.3.3/uw_hrp/__init__.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.2/uw_hrp/models.py` & `UW-RestClients-HRP-1.3.3/uw_hrp/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,31 +103,31 @@
                     self.job_code = id_data.get("Value")
 
     def __str__(self):
         return json.dumps(self.to_json())
 
 
 class EmploymentDetails(models.Model):
-    budget_code = models.CharField(max_length=16, default="")
     start_date = models.DateTimeField(null=True, default=None)
     end_date = models.DateTimeField(null=True, default=None)
+    hr_org = models.CharField(max_length=96, default="")
     job_class = models.CharField(max_length=128, null=True, default=None)
     job_title = models.CharField(max_length=128, null=True, default=None)
     is_primary = models.BooleanField(default=False)
     location = models.CharField(max_length=96, null=True, default=None)
     org_code = models.CharField(max_length=16, default="")
     org_name = models.CharField(max_length=128, default="")
     org_unit_code = models.CharField(max_length=10, default="")
     pos_type = models.CharField(max_length=64, null=True, default=None)
     supervisor_eid = models.CharField(max_length=16,
                                       null=True, default=None)
 
     def to_json(self):
         data = {
-                'budget_code': self.budget_code,
+                'hr_org': self.hr_org,
                 'end_date': date_to_str(self.end_date),
                 'is_primary': self.is_primary,
                 'job_title': self.job_title,
                 'job_class': self.job_class,
                 'location': self.location,
                 'org_code': self.org_code,
                 'org_name': self.org_name,
@@ -169,16 +169,16 @@
 
         if (data.get("OrganizationDetails") is not None and
                 len(data["OrganizationDetails"])):
             for org_det in data["OrganizationDetails"]:
                 if (org_det.get("Organization") is not None and
                         org_det["Organization"].get("Name") is not None and
                         org_det.get("Type") is not None and
-                        org_det["Type"].get("Name") == "Cost Center"):
-                    self.budget_code = org_det["Organization"]["Name"]
+                        org_det["Type"].get("Name") == "HR Org"):
+                    self.hr_org = org_det["Organization"]["Name"]
 
         if data.get("PositionWorkerType") is not None:
             self.pos_type = data["PositionWorkerType"].get("Name")
 
         self.is_primary = data.get("PrimaryPosition")
         self.end_date = parse_date(data.get("PositionVacateDate"))
         self.start_date = parse_date(data.get("StartDate"))
```

### Comparing `UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v1/appointee/123456789.json` & `UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v1/appointee/123456789.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v1/appointee/9136CCB8F66711D5BE060004AC494FFE.json` & `UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v1/appointee/9136CCB8F66711D5BE060004AC494FFE.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v1/appointee/javerage.json` & `UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v1/appointee/javerage.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker/10000000000000000000000000000015.json` & `UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v2/worker/10000000000000000000000000000015.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker/10000000000000000000000000000015.json_workerpositionstate_current_future` & `UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v2/worker/10000000000000000000000000000015.json_workerpositionstate_current_future`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker/100000015.json` & `UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v2/worker/100000015.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker/100000015.json_workerpositionstate_current_future` & `UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v2/worker/100000015.json_workerpositionstate_current_future`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker/chair.json` & `UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v2/worker/chair.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker/faculty.json` & `UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v2/worker/faculty.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker/faculty.json_workerpositionstate_current_future` & `UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v2/worker/faculty.json_workerpositionstate_current_future`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v3/person/000000005.json` & `UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v3/person/000000005.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999957482993198%*

 * *Differences: {"'WorkerDetails'": "{0: {'EmploymentDetails': {0: {'OrganizationDetails': {insert: [(5, "*

 * *                    "OrderedDict([('Type', OrderedDict([('Name', 'HR Org'), ('WID', "*

 * *                    "'87c9ff9a8b111001721d949632ca0000'), ('IDs', [OrderedDict([('Type', 'WID'), "*

 * *                    "('Value', '87c9ff9a8b111001721d949632ca0000')]), OrderedDict([('Type', "*

 * *                    "'Organization_Type_ID'), ('Value', 'HR_ORG')])])])), ('Organization', "*

 * *                    "OrderedDict([('Name', 'Famil […]*

```diff
@@ -348,14 +348,48 @@
                                         "Type": "Organization_Type_ID",
                                         "Value": "SUPERVISORY"
                                     }
                                 ],
                                 "Name": "Supervisory",
                                 "WID": "afa35b88537f014fa5e2f8afb6572d00"
                             }
+                        },
+                        {
+                            "Organization": {
+                                "IDs": [
+                                    {
+                                        "Type": "WID",
+                                        "Value": "990283877b661001ba2b7654f95d0000"
+                                    },
+                                    {
+                                        "Type": "Organization_Reference_ID",
+                                        "Value": "HROrg000733"
+                                    },
+                                    {
+                                        "Type": "Custom_Organization_Reference_ID",
+                                        "Value": "HROrg000733"
+                                    }
+                                ],
+                                "Name": "Family Medicine",
+                                "WID": "990283877b661001ba2b7654f95d0000"
+                            },
+                            "Type": {
+                                "IDs": [
+                                    {
+                                        "Type": "WID",
+                                        "Value": "87c9ff9a8b111001721d949632ca0000"
+                                    },
+                                    {
+                                        "Type": "Organization_Type_ID",
+                                        "Value": "HR_ORG"
+                                    }
+                                ],
+                                "Name": "HR Org",
+                                "WID": "87c9ff9a8b111001721d949632ca0000"
+                            }
                         }
                     ],
                     "PayRateType": {
                         "IDs": [
                             {
                                 "Type": "WID",
                                 "Value": "d957207a306801e0ff0dbb026d5cda1d"
```

### Comparing `UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v3/person/9136CCB8F66711D5BE060004AC494FFE.json` & `UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v3/person/9136CCB8F66711D5BE060004AC494FFE.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v3/person/faculty.json` & `UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v3/person/faculty.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999957482993198%*

 * *Differences: {"'WorkerDetails'": "{0: {'EmploymentDetails': {0: {'OrganizationDetails': {insert: [(5, "*

 * *                    "OrderedDict([('Type', OrderedDict([('Name', 'HR Org'), ('WID', "*

 * *                    "'87c9ff9a8b111001721d949632ca0000'), ('IDs', [OrderedDict([('Type', 'WID'), "*

 * *                    "('Value', '87c9ff9a8b111001721d949632ca0000')]), OrderedDict([('Type', "*

 * *                    "'Organization_Type_ID'), ('Value', 'HR_ORG')])])])), ('Organization', "*

 * *                    "OrderedDict([('Name', 'Famil […]*

```diff
@@ -348,14 +348,48 @@
                                         "Type": "Organization_Type_ID",
                                         "Value": "SUPERVISORY"
                                     }
                                 ],
                                 "Name": "Supervisory",
                                 "WID": "afa35b88537f014fa5e2f8afb6572d00"
                             }
+                        },
+                        {
+                            "Organization": {
+                                "IDs": [
+                                    {
+                                        "Type": "WID",
+                                        "Value": "990283877b661001ba2b7654f95d0000"
+                                    },
+                                    {
+                                        "Type": "Organization_Reference_ID",
+                                        "Value": "HROrg000733"
+                                    },
+                                    {
+                                        "Type": "Custom_Organization_Reference_ID",
+                                        "Value": "HROrg000733"
+                                    }
+                                ],
+                                "Name": "Family Medicine",
+                                "WID": "990283877b661001ba2b7654f95d0000"
+                            },
+                            "Type": {
+                                "IDs": [
+                                    {
+                                        "Type": "WID",
+                                        "Value": "87c9ff9a8b111001721d949632ca0000"
+                                    },
+                                    {
+                                        "Type": "Organization_Type_ID",
+                                        "Value": "HR_ORG"
+                                    }
+                                ],
+                                "Name": "HR Org",
+                                "WID": "87c9ff9a8b111001721d949632ca0000"
+                            }
                         }
                     ],
                     "PayRateType": {
                         "IDs": [
                             {
                                 "Type": "WID",
                                 "Value": "d957207a306801e0ff0dbb026d5cda1d"
```

### Comparing `UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v3/person/faculty.json_future_worker_true` & `UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v3/person/faculty.json_future_worker_true`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999957482993198%*

 * *Differences: {"'WorkerDetails'": "{0: {'EmploymentDetails': {0: {'OrganizationDetails': {insert: [(5, "*

 * *                    "OrderedDict([('Type', OrderedDict([('Name', 'HR Org'), ('WID', "*

 * *                    "'87c9ff9a8b111001721d949632ca0000'), ('IDs', [OrderedDict([('Type', 'WID'), "*

 * *                    "('Value', '87c9ff9a8b111001721d949632ca0000')]), OrderedDict([('Type', "*

 * *                    "'Organization_Type_ID'), ('Value', 'HR_ORG')])])])), ('Organization', "*

 * *                    "OrderedDict([('Name', 'Famil […]*

```diff
@@ -348,14 +348,48 @@
                                         "Type": "Organization_Type_ID",
                                         "Value": "SUPERVISORY"
                                     }
                                 ],
                                 "Name": "Supervisory",
                                 "WID": "afa35b88537f014fa5e2f8afb6572d00"
                             }
+                        },
+                        {
+                            "Organization": {
+                                "IDs": [
+                                    {
+                                        "Type": "WID",
+                                        "Value": "990283877b661001ba2b7654f95d0000"
+                                    },
+                                    {
+                                        "Type": "Organization_Reference_ID",
+                                        "Value": "HROrg000733"
+                                    },
+                                    {
+                                        "Type": "Custom_Organization_Reference_ID",
+                                        "Value": "HROrg000733"
+                                    }
+                                ],
+                                "Name": "Family Medicine",
+                                "WID": "990283877b661001ba2b7654f95d0000"
+                            },
+                            "Type": {
+                                "IDs": [
+                                    {
+                                        "Type": "WID",
+                                        "Value": "87c9ff9a8b111001721d949632ca0000"
+                                    },
+                                    {
+                                        "Type": "Organization_Type_ID",
+                                        "Value": "HR_ORG"
+                                    }
+                                ],
+                                "Name": "HR Org",
+                                "WID": "87c9ff9a8b111001721d949632ca0000"
+                            }
                         }
                     ],
                     "PayRateType": {
                         "IDs": [
                             {
                                 "Type": "WID",
                                 "Value": "d957207a306801e0ff0dbb026d5cda1d"
```

### Comparing `UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v3/person.json_changed_since_date_2022-12-12_page_size_200` & `UW-RestClients-HRP-1.3.3/uw_hrp/resources/hrpws/file/hrp/v3/person.json_changed_since_date_2022-12-12_page_size_200`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.2/uw_hrp/tests/test_hrp.py` & `UW-RestClients-HRP-1.3.3/uw_hrp/tests/test_hrp.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
                 'retirement_date': None,
                 'status': 'Active',
                 'termination_date': None
             })
         self.assertEqual(
             position.primary_position.to_json(),
             {
-                'budget_code': '681925 WORKDAY DEFAULT DEPTBG',
+                'hr_org': 'Family Medicine',
                 'end_date': None,
                 'is_primary': True,
                 'job_class': 'Academic Personnel',
                 'job_profile': {
                     'description': 'Unpaid Academic',
                     'job_code': '21184'
                 },
@@ -95,15 +95,15 @@
         self.assertEqual(
             len(json_worker_details[0]['active_positions']), 2)
         position = person.worker_details[0]
         self.assertEqual(len(position.other_active_positions), 1)
         self.maxDiff = None
         self.assertEqual(
             position.other_active_positions[0].to_json(),
-            {'budget_code': '141614 UNIVERSITY PRESS',
+            {'hr_org': '',
              'end_date': None,
              'is_primary': False,
              'job_class': 'Undergraduate Student',
              'job_profile': {
                 'description': 'Student Assistant - Grad (NE H)',
                 'job_code': '10889'},
              'job_title': 'UW Press Marketing & Sales Student Associate',
```

### Comparing `UW-RestClients-HRP-1.3.2/uw_hrp/tests/test_models.py` & `UW-RestClients-HRP-1.3.3/uw_hrp/tests/test_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,41 +171,31 @@
                                     }
                                 ],
                     }
                 ],
                 "OrganizationDetails": [
                     {
                         "Type": {
-                            "Name": "Cost Center"
+                            "Name": "HR Org"
                         },
                         "Organization": {
-                            "Name": "141614 UNIVERSITY PRESS",
-                            "IDs": [
-                                {
-                                    "Type": "Organization_Reference_ID",
-                                    "Value": "141614"
-                                },
-                                {
-                                    "Type": "Cost_Center_Reference_ID",
-                                    "Value": "141614"
-                                }
-                            ]
+                            "Name": "University Libraries and UW Press (Dept)"
                         }
-                    },
+                    }
                 ],
                 "SupervisoryOrganization": {
                     "Name": "SOM: Family Medicine (... (Inherited))",
                 }
             }
         )
         self.maxDiff = None
         self.assertEqual(
             emp_details.to_json(),
             {
-                'budget_code': '141614 UNIVERSITY PRESS',
+                'hr_org': 'University Libraries and UW Press (Dept)',
                 'end_date': None,
                 'is_primary': True,
                 'job_class': 'Academic Personnel',
                 'job_title': 'Clinical Associate Professor',
                 'job_profile': {
                     'description': 'Unpaid Academic',
                     'job_code': None
@@ -351,15 +341,15 @@
                 'primary_manager_id': None,
                 'regid': '10000000000000000000000000000005',
                 'student_id': '1000005',
                 'worker_details': [
                     {
                         'active_positions': [
                             {
-                                'budget_code': '',
+                                'hr_org': '',
                                 'is_primary': True,
                                 'job_class': None,
                                 'job_profile': {'description': None,
                                                 'job_code': None},
                                 'job_title': 'Student Assistant (NE H)',
                                 'location': None,
                                 'org_code': 'CAS',
```

