# Comparing `tmp/autonomous-app-0.1.3.tar.gz` & `tmp/autonomous-app-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autonomous-app-0.1.3.tar", last modified: Thu Jul 20 15:48:56 2023, max compression
+gzip compressed data, was "autonomous-app-0.1.4.tar", last modified: Tue Jul 25 17:31:10 2023, max compression
```

## Comparing `autonomous-app-0.1.3.tar` & `autonomous-app-0.1.4.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-20 15:48:56.813320 autonomous-app-0.1.3/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1076 2023-03-07 12:36:40.000000 autonomous-app-0.1.3/LICENSE
--rw-r--r--   0 samoore   (1000) samoore   (1000)     3809 2023-07-20 15:48:56.813320 autonomous-app-0.1.3/PKG-INFO
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2011 2023-06-20 21:09:23.000000 autonomous-app-0.1.3/README.md
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1469 2023-07-20 14:57:42.000000 autonomous-app-0.1.3/pyproject.toml
--rw-r--r--   0 samoore   (1000) samoore   (1000)      510 2023-06-12 14:16:24.000000 autonomous-app-0.1.3/requirements.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-07-20 15:48:56.813320 autonomous-app-0.1.3/setup.cfg
--rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-04-04 14:14:59.000000 autonomous-app-0.1.3/setup.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-20 15:48:56.808320 autonomous-app-0.1.3/src/
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-20 15:48:56.809320 autonomous-app-0.1.3/src/autonomous/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       86 2023-07-20 15:47:41.000000 autonomous-app-0.1.3/src/autonomous/__init__.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-20 15:48:56.809320 autonomous-app-0.1.3/src/autonomous/apis/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       27 2023-06-20 19:34:19.000000 autonomous-app-0.1.3/src/autonomous/apis/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2149 2023-07-07 13:12:31.000000 autonomous-app-0.1.3/src/autonomous/apis/openai.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-20 15:48:56.810320 autonomous-app-0.1.3/src/autonomous/apis/version_control/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1069 2023-03-07 16:24:11.000000 autonomous-app-0.1.3/src/autonomous/apis/version_control/GHCallbacks.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1155 2023-03-07 21:09:26.000000 autonomous-app-0.1.3/src/autonomous/apis/version_control/GHOrganization.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     4622 2023-03-07 16:24:11.000000 autonomous-app-0.1.3/src/autonomous/apis/version_control/GHRepo.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      196 2023-03-07 16:24:11.000000 autonomous-app-0.1.3/src/autonomous/apis/version_control/GHVersionControl.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      117 2023-03-07 16:24:11.000000 autonomous-app-0.1.3/src/autonomous/apis/version_control/__init__.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-20 15:48:56.808320 autonomous-app-0.1.3/src/autonomous/app_template/
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-20 15:48:56.810320 autonomous-app-0.1.3/src/autonomous/app_template/app/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       29 2023-04-04 14:32:12.000000 autonomous-app-0.1.3/src/autonomous/app_template/app/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1495 2023-04-28 17:49:36.000000 autonomous-app-0.1.3/src/autonomous/app_template/app/app.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      574 2023-04-28 17:51:04.000000 autonomous-app-0.1.3/src/autonomous/app_template/app/config.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-20 15:48:56.810320 autonomous-app-0.1.3/src/autonomous/app_template/app/models/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-04-04 14:32:12.000000 autonomous-app-0.1.3/src/autonomous/app_template/app/models/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      203 2023-04-04 15:41:08.000000 autonomous-app-0.1.3/src/autonomous/app_template/app/models/model.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-20 15:48:56.810320 autonomous-app-0.1.3/src/autonomous/app_template/app/views/
--rwxr-xr-x   0 samoore   (1000) samoore   (1000)      589 2023-04-04 14:32:12.000000 autonomous-app-0.1.3/src/autonomous/app_template/app/views/admin.py
--rwxr-xr-x   0 samoore   (1000) samoore   (1000)      589 2023-04-28 17:48:57.000000 autonomous-app-0.1.3/src/autonomous/app_template/app/views/index.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-20 15:48:56.811319 autonomous-app-0.1.3/src/autonomous/app_template/tests/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-04-04 14:32:12.000000 autonomous-app-0.1.3/src/autonomous/app_template/tests/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      204 2023-04-04 18:40:47.000000 autonomous-app-0.1.3/src/autonomous/app_template/tests/test_app.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      558 2023-04-04 18:40:13.000000 autonomous-app-0.1.3/src/autonomous/app_template/tests/test_modules.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-20 15:48:56.811319 autonomous-app-0.1.3/src/autonomous/app_template/vendor/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1124 2023-04-13 17:57:17.000000 autonomous-app-0.1.3/src/autonomous/app_template/vendor/gunicorn.conf.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2252 2023-06-08 19:19:57.000000 autonomous-app-0.1.3/src/autonomous/assets.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)       42 2023-04-04 14:14:59.000000 autonomous-app-0.1.3/src/autonomous/cli.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-20 15:48:56.811319 autonomous-app-0.1.3/src/autonomous/db/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       94 2023-07-07 12:00:23.000000 autonomous-app-0.1.3/src/autonomous/db/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      812 2023-07-07 12:05:15.000000 autonomous-app-0.1.3/src/autonomous/db/autodb.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      531 2023-04-04 14:14:59.000000 autonomous-app-0.1.3/src/autonomous/db/storage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2521 2023-06-20 21:17:55.000000 autonomous-app-0.1.3/src/autonomous/db/table.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1245 2023-06-01 20:06:24.000000 autonomous-app-0.1.3/src/autonomous/logger.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-20 15:48:56.811319 autonomous-app-0.1.3/src/autonomous/model/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-04-02 18:01:05.000000 autonomous-app-0.1.3/src/autonomous/model/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     4035 2023-07-20 15:46:58.000000 autonomous-app-0.1.3/src/autonomous/model/automodel.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      650 2023-06-13 18:03:23.000000 autonomous-app-0.1.3/src/autonomous/model/orm.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-20 15:48:56.812320 autonomous-app-0.1.3/src/autonomous/storage/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       88 2023-06-13 18:11:53.000000 autonomous-app-0.1.3/src/autonomous/storage/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      447 2023-06-05 17:49:27.000000 autonomous-app-0.1.3/src/autonomous/storage/basestorage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1620 2023-07-07 13:13:20.000000 autonomous-app-0.1.3/src/autonomous/storage/cloudinarystorage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      156 2023-06-13 18:11:43.000000 autonomous-app-0.1.3/src/autonomous/storage/localstorage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1381 2023-06-13 18:12:16.000000 autonomous-app-0.1.3/src/autonomous/storage/s3storage.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-20 15:48:56.812320 autonomous-app-0.1.3/src/autonomous/tasks/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       23 2023-07-20 14:42:57.000000 autonomous-app-0.1.3/src/autonomous/tasks/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1319 2023-07-20 15:37:47.000000 autonomous-app-0.1.3/src/autonomous/tasks/task.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      529 2023-07-20 15:09:11.000000 autonomous-app-0.1.3/src/autonomous/tasks/taskqueue.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-20 15:48:56.813320 autonomous-app-0.1.3/src/autonomous_app.egg-info/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     3809 2023-07-20 15:48:56.000000 autonomous-app-0.1.3/src/autonomous_app.egg-info/PKG-INFO
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1737 2023-07-20 15:48:56.000000 autonomous-app-0.1.3/src/autonomous_app.egg-info/SOURCES.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-07-20 15:48:56.000000 autonomous-app-0.1.3/src/autonomous_app.egg-info/dependency_links.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)       53 2023-07-20 15:48:56.000000 autonomous-app-0.1.3/src/autonomous_app.egg-info/entry_points.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)      148 2023-07-20 15:48:56.000000 autonomous-app-0.1.3/src/autonomous_app.egg-info/requires.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)       11 2023-07-20 15:48:56.000000 autonomous-app-0.1.3/src/autonomous_app.egg-info/top_level.txt
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-25 17:31:10.138188 autonomous-app-0.1.4/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1076 2023-03-07 12:36:40.000000 autonomous-app-0.1.4/LICENSE
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     3809 2023-07-25 17:31:10.138188 autonomous-app-0.1.4/PKG-INFO
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     2011 2023-06-20 21:09:23.000000 autonomous-app-0.1.4/README.md
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1469 2023-07-20 14:57:42.000000 autonomous-app-0.1.4/pyproject.toml
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      510 2023-06-12 14:16:24.000000 autonomous-app-0.1.4/requirements.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-07-25 17:31:10.138188 autonomous-app-0.1.4/setup.cfg
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-04-04 14:14:59.000000 autonomous-app-0.1.4/setup.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-25 17:31:10.124188 autonomous-app-0.1.4/src/
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-25 17:31:10.127188 autonomous-app-0.1.4/src/autonomous/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       86 2023-07-25 17:30:54.000000 autonomous-app-0.1.4/src/autonomous/__init__.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-25 17:31:10.127188 autonomous-app-0.1.4/src/autonomous/apis/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       27 2023-06-20 19:34:19.000000 autonomous-app-0.1.4/src/autonomous/apis/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     2149 2023-07-07 13:12:31.000000 autonomous-app-0.1.4/src/autonomous/apis/openai.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-25 17:31:10.129187 autonomous-app-0.1.4/src/autonomous/apis/version_control/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1069 2023-03-07 16:24:11.000000 autonomous-app-0.1.4/src/autonomous/apis/version_control/GHCallbacks.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1155 2023-03-07 21:09:26.000000 autonomous-app-0.1.4/src/autonomous/apis/version_control/GHOrganization.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     4622 2023-03-07 16:24:11.000000 autonomous-app-0.1.4/src/autonomous/apis/version_control/GHRepo.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      196 2023-03-07 16:24:11.000000 autonomous-app-0.1.4/src/autonomous/apis/version_control/GHVersionControl.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      117 2023-03-07 16:24:11.000000 autonomous-app-0.1.4/src/autonomous/apis/version_control/__init__.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-25 17:31:10.124188 autonomous-app-0.1.4/src/autonomous/app_template/
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-25 17:31:10.130188 autonomous-app-0.1.4/src/autonomous/app_template/app/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       29 2023-04-04 14:32:12.000000 autonomous-app-0.1.4/src/autonomous/app_template/app/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1495 2023-04-28 17:49:36.000000 autonomous-app-0.1.4/src/autonomous/app_template/app/app.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      574 2023-04-28 17:51:04.000000 autonomous-app-0.1.4/src/autonomous/app_template/app/config.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-25 17:31:10.130188 autonomous-app-0.1.4/src/autonomous/app_template/app/models/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-04-04 14:32:12.000000 autonomous-app-0.1.4/src/autonomous/app_template/app/models/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      203 2023-04-04 15:41:08.000000 autonomous-app-0.1.4/src/autonomous/app_template/app/models/model.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-25 17:31:10.131188 autonomous-app-0.1.4/src/autonomous/app_template/app/views/
+-rwxr-xr-x   0 samoore   (1000) samoore   (1000)      589 2023-04-04 14:32:12.000000 autonomous-app-0.1.4/src/autonomous/app_template/app/views/admin.py
+-rwxr-xr-x   0 samoore   (1000) samoore   (1000)      589 2023-04-28 17:48:57.000000 autonomous-app-0.1.4/src/autonomous/app_template/app/views/index.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-25 17:31:10.131188 autonomous-app-0.1.4/src/autonomous/app_template/tests/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-04-04 14:32:12.000000 autonomous-app-0.1.4/src/autonomous/app_template/tests/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      204 2023-04-04 18:40:47.000000 autonomous-app-0.1.4/src/autonomous/app_template/tests/test_app.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      558 2023-04-04 18:40:13.000000 autonomous-app-0.1.4/src/autonomous/app_template/tests/test_modules.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-25 17:31:10.132187 autonomous-app-0.1.4/src/autonomous/app_template/vendor/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1124 2023-04-13 17:57:17.000000 autonomous-app-0.1.4/src/autonomous/app_template/vendor/gunicorn.conf.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     2252 2023-06-08 19:19:57.000000 autonomous-app-0.1.4/src/autonomous/assets.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       42 2023-04-04 14:14:59.000000 autonomous-app-0.1.4/src/autonomous/cli.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-25 17:31:10.134188 autonomous-app-0.1.4/src/autonomous/db/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       94 2023-07-07 12:00:23.000000 autonomous-app-0.1.4/src/autonomous/db/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      812 2023-07-07 12:05:15.000000 autonomous-app-0.1.4/src/autonomous/db/autodb.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      531 2023-04-04 14:14:59.000000 autonomous-app-0.1.4/src/autonomous/db/storage.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     2521 2023-06-20 21:17:55.000000 autonomous-app-0.1.4/src/autonomous/db/table.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1245 2023-06-01 20:06:24.000000 autonomous-app-0.1.4/src/autonomous/logger.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-25 17:31:10.135187 autonomous-app-0.1.4/src/autonomous/model/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-04-02 18:01:05.000000 autonomous-app-0.1.4/src/autonomous/model/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     4035 2023-07-20 15:46:58.000000 autonomous-app-0.1.4/src/autonomous/model/automodel.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      650 2023-06-13 18:03:23.000000 autonomous-app-0.1.4/src/autonomous/model/orm.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-25 17:31:10.136187 autonomous-app-0.1.4/src/autonomous/storage/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       88 2023-06-13 18:11:53.000000 autonomous-app-0.1.4/src/autonomous/storage/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      447 2023-06-05 17:49:27.000000 autonomous-app-0.1.4/src/autonomous/storage/basestorage.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1620 2023-07-07 13:13:20.000000 autonomous-app-0.1.4/src/autonomous/storage/cloudinarystorage.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      156 2023-06-13 18:11:43.000000 autonomous-app-0.1.4/src/autonomous/storage/localstorage.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1381 2023-06-13 18:12:16.000000 autonomous-app-0.1.4/src/autonomous/storage/s3storage.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-25 17:31:10.136187 autonomous-app-0.1.4/src/autonomous/tasks/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       23 2023-07-20 14:42:57.000000 autonomous-app-0.1.4/src/autonomous/tasks/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     2201 2023-07-25 17:16:13.000000 autonomous-app-0.1.4/src/autonomous/tasks/task.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      529 2023-07-20 15:09:11.000000 autonomous-app-0.1.4/src/autonomous/tasks/taskqueue.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-25 17:31:10.137188 autonomous-app-0.1.4/src/autonomous_app.egg-info/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     3809 2023-07-25 17:31:10.000000 autonomous-app-0.1.4/src/autonomous_app.egg-info/PKG-INFO
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1737 2023-07-25 17:31:10.000000 autonomous-app-0.1.4/src/autonomous_app.egg-info/SOURCES.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-07-25 17:31:10.000000 autonomous-app-0.1.4/src/autonomous_app.egg-info/dependency_links.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       53 2023-07-25 17:31:10.000000 autonomous-app-0.1.4/src/autonomous_app.egg-info/entry_points.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      148 2023-07-25 17:31:10.000000 autonomous-app-0.1.4/src/autonomous_app.egg-info/requires.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       11 2023-07-25 17:31:10.000000 autonomous-app-0.1.4/src/autonomous_app.egg-info/top_level.txt
```

### Comparing `autonomous-app-0.1.3/LICENSE` & `autonomous-app-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.3/PKG-INFO` & `autonomous-app-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomous-app
-Version: 0.1.3
+Version: 0.1.4
 Summary: Containerized application framework built on Flask with additional libraries and tools for rapid development of web applications.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autonomous-app-0.1.3/README.md` & `autonomous-app-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.3/pyproject.toml` & `autonomous-app-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.3/src/autonomous/apis/openai.py` & `autonomous-app-0.1.4/src/autonomous/apis/openai.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.3/src/autonomous/apis/version_control/GHCallbacks.py` & `autonomous-app-0.1.4/src/autonomous/apis/version_control/GHCallbacks.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.3/src/autonomous/apis/version_control/GHOrganization.py` & `autonomous-app-0.1.4/src/autonomous/apis/version_control/GHOrganization.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.3/src/autonomous/apis/version_control/GHRepo.py` & `autonomous-app-0.1.4/src/autonomous/apis/version_control/GHRepo.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.3/src/autonomous/app_template/app/app.py` & `autonomous-app-0.1.4/src/autonomous/app_template/app/app.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.3/src/autonomous/app_template/app/config.py` & `autonomous-app-0.1.4/src/autonomous/app_template/app/config.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.3/src/autonomous/app_template/app/views/admin.py` & `autonomous-app-0.1.4/src/autonomous/app_template/app/views/admin.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.3/src/autonomous/app_template/app/views/index.py` & `autonomous-app-0.1.4/src/autonomous/app_template/app/views/index.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.3/src/autonomous/app_template/tests/test_modules.py` & `autonomous-app-0.1.4/src/autonomous/app_template/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.3/src/autonomous/app_template/vendor/gunicorn.conf.py` & `autonomous-app-0.1.4/src/autonomous/app_template/vendor/gunicorn.conf.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.3/src/autonomous/assets.py` & `autonomous-app-0.1.4/src/autonomous/assets.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.3/src/autonomous/db/autodb.py` & `autonomous-app-0.1.4/src/autonomous/db/autodb.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.3/src/autonomous/db/storage.py` & `autonomous-app-0.1.4/src/autonomous/db/storage.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.3/src/autonomous/db/table.py` & `autonomous-app-0.1.4/src/autonomous/db/table.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.3/src/autonomous/logger.py` & `autonomous-app-0.1.4/src/autonomous/logger.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.3/src/autonomous/model/automodel.py` & `autonomous-app-0.1.4/src/autonomous/model/automodel.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.3/src/autonomous/model/orm.py` & `autonomous-app-0.1.4/src/autonomous/model/orm.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.3/src/autonomous/storage/cloudinarystorage.py` & `autonomous-app-0.1.4/src/autonomous/storage/cloudinarystorage.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.3/src/autonomous/storage/s3storage.py` & `autonomous-app-0.1.4/src/autonomous/storage/s3storage.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.3/src/autonomous/tasks/task.py` & `autonomous-app-0.1.4/src/autonomous/tasks/task.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,34 +13,66 @@
         # wait until thread is finished
         if self.task.is_alive():
             self.task.join()
         self.interrupt_handler(signum, frame)
 
 
 class Task(threading.Thread):
-    def __init__(self):
-        super().__init__()
+    """
+    Create a task to run in a seperate thread.
+
+    ### Usage
+
+    ```python
+    class MyTask(Task):
+        def startup(self):
+            '''optional: initialize resources for the task'''
+        def task(self):
+            '''implement the task'''
+        def shutdown(self):
+            '''optional: clean up resources for the task'''
+    ```
+    -----
+    ```
+    mytask = MyTask()
+    mytask.start()
+    print(Task.runningtasks[mytask.name])  # check status of task
+    mytask.join() # to wait for the task to complete
+    ```
+
+    """
+
+    runningtasks = {}
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
         self.handler = TaskInterruptHandler(self)
+        Task.runningtasks[self.name] = "initialized"
 
     def startup(self) -> None:
-        log("Task started: override `startup` method to intialize resouces for the task")
+        log("Task started: override `startup(self)` method to intialize resources for the task")
 
     def task(self) -> None:
-        log("Task executing: override `task` mwethod to implement the task")
+        log("Task executing: override `task` method to implement the task")
 
     def shutdown(self) -> None:
-        log("Task stopped: override `shutdown` method to clean up resources for the task")
+        log("Task complete: override `shutdown` method to clean up resources for the task")
 
     def run(self) -> None:
         """
         This method will be executed in a separate thread
         when start() method is called.
         :return: None
         """
+        Task.runningtasks[self.name] = "starting"
         self.startup()
         try:
+            Task.runningtasks[self.name] = "running"
             self.task()
         except Exception as e:
+            Task.runningtasks[self.name] = f"ERROR: {e}"
             log(f"Task raised an exception: {e}")
+            raise e
         else:
             log("Task was executed.")
         self.shutdown()
+        Task.runningtasks[self.name] = "complete"
```

### Comparing `autonomous-app-0.1.3/src/autonomous/tasks/taskqueue.py` & `autonomous-app-0.1.4/src/autonomous/tasks/taskqueue.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.3/src/autonomous_app.egg-info/PKG-INFO` & `autonomous-app-0.1.4/src/autonomous_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomous-app
-Version: 0.1.3
+Version: 0.1.4
 Summary: Containerized application framework built on Flask with additional libraries and tools for rapid development of web applications.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autonomous-app-0.1.3/src/autonomous_app.egg-info/SOURCES.txt` & `autonomous-app-0.1.4/src/autonomous_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

