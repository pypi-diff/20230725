# Comparing `tmp/tesla-ce-provider-0.0.7.tar.gz` & `tmp/tesla-ce-provider-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tesla-ce-provider-0.0.7.tar", last modified: Mon Nov 29 08:18:33 2021, max compression
+gzip compressed data, was "tesla-ce-provider-0.0.8.tar", last modified: Tue Jul 25 10:28:18 2023, max compression
```

## Comparing `tesla-ce-provider-0.0.7.tar` & `tesla-ce-provider-0.0.8.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-29 08:18:33.337004 tesla-ce-provider-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       88 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2910 2021-11-29 08:18:33.337004 tesla-ce-provider-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2036 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       77 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-29 08:18:33.337004 tesla-ce-provider-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1944 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-29 08:18:33.333004 tesla-ce-provider-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-29 08:18:33.333004 tesla-ce-provider-0.0.7/src/tesla_ce_provider/
--rw-r--r--   0 runner    (1001) docker     (121)     1044 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2599 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider/celery_app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-29 08:18:33.337004 tesla-ce-provider-0.0.7/src/tesla_ce_provider/data/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-11-29 08:18:32.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider/data/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)      487 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider/data/options.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-29 08:18:33.337004 tesla-ce-provider-0.0.7/src/tesla_ce_provider/message/
--rw-r--r--   0 runner    (1001) docker     (121)      971 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      934 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider/message/integrity.py
--rw-r--r--   0 runner    (1001) docker     (121)     1446 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider/message/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     1401 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider/message/sensor.py
--rw-r--r--   0 runner    (1001) docker     (121)      949 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider/message/status.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-29 08:18:33.337004 tesla-ce-provider-0.0.7/src/tesla_ce_provider/models/
--rw-r--r--   0 runner    (1001) docker     (121)      980 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10050 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider/models/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3051 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider/models/fr.py
--rw-r--r--   0 runner    (1001) docker     (121)     6572 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider/models/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     1721 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider/models/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-29 08:18:33.337004 tesla-ce-provider-0.0.7/src/tesla_ce_provider/provider/
--rw-r--r--   0 runner    (1001) docker     (121)      915 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider/provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-29 08:18:33.337004 tesla-ce-provider-0.0.7/src/tesla_ce_provider/provider/audit/
--rw-r--r--   0 runner    (1001) docker     (121)      960 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider/provider/audit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1412 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider/provider/audit/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3221 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider/provider/audit/fr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1515 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider/provider/audit/ks.py
--rw-r--r--   0 runner    (1001) docker     (121)     3693 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider/provider/audit/tp.py
--rw-r--r--   0 runner    (1001) docker     (121)     6344 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider/provider/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     9517 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider/provider/result.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-29 08:18:33.337004 tesla-ce-provider-0.0.7/src/tesla_ce_provider/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)     1028 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12571 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider/tasks/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     8556 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider/tasks/enrolment.py
--rw-r--r--   0 runner    (1001) docker     (121)     2110 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider/tasks/notification.py
--rw-r--r--   0 runner    (1001) docker     (121)     4658 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider/tasks/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-29 08:18:33.337004 tesla-ce-provider-0.0.7/src/tesla_ce_provider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2910 2021-11-29 08:18:33.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1636 2021-11-29 08:18:33.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-29 08:18:33.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       77 2021-11-29 08:18:33.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       59 2021-11-29 08:18:33.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2021-11-29 08:18:33.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-29 08:18:33.337004 tesla-ce-provider-0.0.7/src/tesla_ce_provider_fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)      820 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider_fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7565 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tesla_ce_provider_fixtures/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-29 08:18:33.337004 tesla-ce-provider-0.0.7/src/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      788 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-29 08:18:33.337004 tesla-ce-provider-0.0.7/src/tests/base_fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)      791 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tests/base_fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tests/base_fixtures/test_provider_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (121)     1883 2021-11-29 08:18:26.000000 tesla-ce-provider-0.0.7/src/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:28:18.692268 tesla-ce-provider-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-25 10:28:18.692268 tesla-ce-provider-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 10:28:18.692268 tesla-ce-provider-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:28:18.688267 tesla-ce-provider-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:28:18.692268 tesla-ce-provider-0.0.8/src/tesla_ce_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider/celery_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:28:18.692268 tesla-ce-provider-0.0.8/src/tesla_ce_provider/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 10:28:18.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider/data/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider/data/options.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:28:18.692268 tesla-ce-provider-0.0.8/src/tesla_ce_provider/message/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider/message/integrity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider/message/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider/message/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider/message/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:28:18.692268 tesla-ce-provider-0.0.8/src/tesla_ce_provider/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider/models/fr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider/models/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:28:18.692268 tesla-ce-provider-0.0.8/src/tesla_ce_provider/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider/provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:28:18.692268 tesla-ce-provider-0.0.8/src/tesla_ce_provider/provider/audit/
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider/provider/audit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider/provider/audit/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider/provider/audit/fr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider/provider/audit/ks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider/provider/audit/tp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider/provider/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9517 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider/provider/result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:28:18.692268 tesla-ce-provider-0.0.8/src/tesla_ce_provider/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider/tasks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider/tasks/enrolment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider/tasks/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider/tasks/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:28:18.692268 tesla-ce-provider-0.0.8/src/tesla_ce_provider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-25 10:28:18.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-25 10:28:18.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 10:28:18.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-25 10:28:18.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-25 10:28:18.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-25 10:28:18.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:28:18.692268 tesla-ce-provider-0.0.8/src/tesla_ce_provider_fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider_fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tesla_ce_provider_fixtures/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:28:18.692268 tesla-ce-provider-0.0.8/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:28:18.692268 tesla-ce-provider-0.0.8/src/tests/base_fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tests/base_fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tests/base_fixtures/test_provider_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-25 10:28:09.000000 tesla-ce-provider-0.0.8/src/tests/conftest.py
```

### Comparing `tesla-ce-provider-0.0.7/LICENSE` & `tesla-ce-provider-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/PKG-INFO` & `tesla-ce-provider-0.0.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 Metadata-Version: 2.1
 Name: tesla-ce-provider
-Version: 0.0.7
+Version: 0.0.8
 Summary: TeSLA Python SDK for providers
 Home-page: https://tesla-ce.github.io
 Author: Xavier Baro
 Author-email: xbaro@uoc.edu
 License: UNKNOWN
 Project-URL: Documentation, https://tesla-ce.github.io/python-provider-sdk/
 Project-URL: Source, https://github.com/tesla-ce/python-provider-sdk
-Description: [![PyPi Version](https://img.shields.io/pypi/v/tesla-ce-provider.svg)](https://pypi.python.org/pypi/tesla-ce-provider/)
-        [![codecov](https://codecov.io/gh/tesla-ce/python-provider-sdk/branch/main/graph/badge.svg?token=PJJQMW981P)](https://codecov.io/gh/tesla-ce/python-provider-sdk)
-        [![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)  
-        [![Quality gate](https://sonar.sunai.uoc.edu/api/project_badges/quality_gate?project=tesla-ce_python-provider-sdk)](https://sonar.sunai.uoc.edu/dashboard?id=tesla-ce_python-provider-sdk)
-        # TeSLA CE Providers Python SDK
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
 Classifier: Framework :: Pytest
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPi Version](https://img.shields.io/pypi/v/tesla-ce-provider.svg)](https://pypi.python.org/pypi/tesla-ce-provider/)
+[![codecov](https://codecov.io/gh/tesla-ce/python-provider-sdk/branch/main/graph/badge.svg?token=PJJQMW981P)](https://codecov.io/gh/tesla-ce/python-provider-sdk)
+[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)  
+[![Quality gate](https://sonar.sunai.uoc.edu/api/project_badges/quality_gate?project=tesla-ce_python-provider-sdk)](https://sonar.sunai.uoc.edu/dashboard?id=tesla-ce_python-provider-sdk)
+# TeSLA CE Providers Python SDK
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

### Comparing `tesla-ce-provider-0.0.7/README.md` & `tesla-ce-provider-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/setup.py` & `tesla-ce-provider-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/src/tesla_ce_provider/__init__.py` & `tesla-ce-provider-0.0.8/src/tesla_ce_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/src/tesla_ce_provider/celery_app.py` & `tesla-ce-provider-0.0.8/src/tesla_ce_provider/celery_app.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/src/tesla_ce_provider/message/__init__.py` & `tesla-ce-provider-0.0.8/src/tesla_ce_provider/message/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/src/tesla_ce_provider/message/integrity.py` & `tesla-ce-provider-0.0.8/src/tesla_ce_provider/message/integrity.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/src/tesla_ce_provider/message/provider.py` & `tesla-ce-provider-0.0.8/src/tesla_ce_provider/message/provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,10 +20,11 @@
     """ Message codes related to Providers """
     PROVIDER_MULTIPLE_PEOPLE = 'PROVIDER_MULTIPLE_PEOPLE'
     PROVIDER_INCOMPLETE_ENROLMENT = 'PROVIDER_INCOMPLETE_ENROLMENT'
     PROVIDER_NO_FACE_DETECTED = 'PROVIDER_NO_FACE_DETECTED'
     PROVIDER_INVALID_MIMETYPE = 'PROVIDER_INVALID_MIMETYPE'
     PROVIDER_MISSING_MIMETYPE = 'PROVIDER_MISSING_MIMETYPE'
     PROVIDER_INVALID_SAMPLE_DATA = 'PROVIDER_INVALID_SAMPLE_DATA'
+    PROVIDER_INVALID_PARTIAL_SAMPLE_DATA = 'PROVIDER_INVALID_PARTIAL_SAMPLE_DATA'
     PROVIDER_BLACK_IMAGE = 'PROVIDER_BLACK_IMAGE'
     PROVIDER_EXTERNAL_SERVICE_DOWN = 'PROVIDER_EXTERNAL_SERVICE_DOWN'
     PROVIDER_EXTERNAL_SERVICE_TIMEOUT = 'PROVIDER_EXTERNAL_SERVICE_TIMEOUT'
```

### Comparing `tesla-ce-provider-0.0.7/src/tesla_ce_provider/message/sensor.py` & `tesla-ce-provider-0.0.8/src/tesla_ce_provider/message/sensor.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/src/tesla_ce_provider/message/status.py` & `tesla-ce-provider-0.0.8/src/tesla_ce_provider/message/status.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/src/tesla_ce_provider/models/__init__.py` & `tesla-ce-provider-0.0.8/src/tesla_ce_provider/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/src/tesla_ce_provider/models/base.py` & `tesla-ce-provider-0.0.8/src/tesla_ce_provider/models/base.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/src/tesla_ce_provider/models/fr.py` & `tesla-ce-provider-0.0.8/src/tesla_ce_provider/models/fr.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/src/tesla_ce_provider/models/model.py` & `tesla-ce-provider-0.0.8/src/tesla_ce_provider/models/model.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/src/tesla_ce_provider/models/parser.py` & `tesla-ce-provider-0.0.8/src/tesla_ce_provider/models/parser.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/src/tesla_ce_provider/provider/__init__.py` & `tesla-ce-provider-0.0.8/src/tesla_ce_provider/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/src/tesla_ce_provider/provider/audit/__init__.py` & `tesla-ce-provider-0.0.8/src/tesla_ce_provider/provider/audit/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/src/tesla_ce_provider/provider/audit/base.py` & `tesla-ce-provider-0.0.8/src/tesla_ce_provider/provider/audit/base.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/src/tesla_ce_provider/provider/audit/fr.py` & `tesla-ce-provider-0.0.8/src/tesla_ce_provider/provider/audit/fr.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/src/tesla_ce_provider/provider/audit/ks.py` & `tesla-ce-provider-0.0.8/src/tesla_ce_provider/provider/audit/ks.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/src/tesla_ce_provider/provider/audit/tp.py` & `tesla-ce-provider-0.0.8/src/tesla_ce_provider/provider/audit/tp.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/src/tesla_ce_provider/provider/base.py` & `tesla-ce-provider-0.0.8/src/tesla_ce_provider/provider/base.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/src/tesla_ce_provider/provider/result.py` & `tesla-ce-provider-0.0.8/src/tesla_ce_provider/provider/result.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/src/tesla_ce_provider/tasks/__init__.py` & `tesla-ce-provider-0.0.8/src/tesla_ce_provider/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/src/tesla_ce_provider/tasks/base.py` & `tesla-ce-provider-0.0.8/src/tesla_ce_provider/tasks/base.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/src/tesla_ce_provider/tasks/enrolment.py` & `tesla-ce-provider-0.0.8/src/tesla_ce_provider/tasks/enrolment.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/src/tesla_ce_provider/tasks/notification.py` & `tesla-ce-provider-0.0.8/src/tesla_ce_provider/tasks/notification.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/src/tesla_ce_provider/tasks/verification.py` & `tesla-ce-provider-0.0.8/src/tesla_ce_provider/tasks/verification.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/src/tesla_ce_provider.egg-info/PKG-INFO` & `tesla-ce-provider-0.0.8/src/tesla_ce_provider.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 Metadata-Version: 2.1
 Name: tesla-ce-provider
-Version: 0.0.7
+Version: 0.0.8
 Summary: TeSLA Python SDK for providers
 Home-page: https://tesla-ce.github.io
 Author: Xavier Baro
 Author-email: xbaro@uoc.edu
 License: UNKNOWN
 Project-URL: Documentation, https://tesla-ce.github.io/python-provider-sdk/
 Project-URL: Source, https://github.com/tesla-ce/python-provider-sdk
-Description: [![PyPi Version](https://img.shields.io/pypi/v/tesla-ce-provider.svg)](https://pypi.python.org/pypi/tesla-ce-provider/)
-        [![codecov](https://codecov.io/gh/tesla-ce/python-provider-sdk/branch/main/graph/badge.svg?token=PJJQMW981P)](https://codecov.io/gh/tesla-ce/python-provider-sdk)
-        [![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)  
-        [![Quality gate](https://sonar.sunai.uoc.edu/api/project_badges/quality_gate?project=tesla-ce_python-provider-sdk)](https://sonar.sunai.uoc.edu/dashboard?id=tesla-ce_python-provider-sdk)
-        # TeSLA CE Providers Python SDK
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
 Classifier: Framework :: Pytest
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPi Version](https://img.shields.io/pypi/v/tesla-ce-provider.svg)](https://pypi.python.org/pypi/tesla-ce-provider/)
+[![codecov](https://codecov.io/gh/tesla-ce/python-provider-sdk/branch/main/graph/badge.svg?token=PJJQMW981P)](https://codecov.io/gh/tesla-ce/python-provider-sdk)
+[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)  
+[![Quality gate](https://sonar.sunai.uoc.edu/api/project_badges/quality_gate?project=tesla-ce_python-provider-sdk)](https://sonar.sunai.uoc.edu/dashboard?id=tesla-ce_python-provider-sdk)
+# TeSLA CE Providers Python SDK
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

### Comparing `tesla-ce-provider-0.0.7/src/tesla_ce_provider.egg-info/SOURCES.txt` & `tesla-ce-provider-0.0.8/src/tesla_ce_provider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/src/tesla_ce_provider_fixtures/__init__.py` & `tesla-ce-provider-0.0.8/src/tesla_ce_provider_fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/src/tesla_ce_provider_fixtures/fixtures.py` & `tesla-ce-provider-0.0.8/src/tesla_ce_provider_fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/src/tests/__init__.py` & `tesla-ce-provider-0.0.8/src/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/src/tests/base_fixtures/__init__.py` & `tesla-ce-provider-0.0.8/src/tests/base_fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/src/tests/base_fixtures/test_provider_fixtures.py` & `tesla-ce-provider-0.0.8/src/tests/base_fixtures/test_provider_fixtures.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-0.0.7/src/tests/conftest.py` & `tesla-ce-provider-0.0.8/src/tests/conftest.py`

 * *Files identical despite different names*

