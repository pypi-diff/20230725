# Comparing `tmp/remotemanager-0.9.3.tar.gz` & `tmp/remotemanager-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotemanager-0.9.3.tar", last modified: Fri Jul 21 11:14:30 2023, max compression
+gzip compressed data, was "remotemanager-0.9.4.tar", last modified: Tue Jul 25 13:05:14 2023, max compression
```

## Comparing `remotemanager-0.9.3.tar` & `remotemanager-0.9.4.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:14:30.742383 remotemanager-0.9.3/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.9.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1278 2023-07-21 11:14:30.742383 remotemanager-0.9.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:45:06.000000 remotemanager-0.9.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1367 2023-07-21 09:25:26.000000 remotemanager-0.9.3/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:14:30.734383 remotemanager-0.9.3/remotemanager/
--rw-rw-rw-   0 root         (0) root         (0)      481 2023-07-21 09:25:26.000000 remotemanager-0.9.3/remotemanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:14:30.738383 remotemanager-0.9.3/remotemanager/connection/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/connection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-14 09:06:03.000000 remotemanager-0.9.3/remotemanager/connection/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:14:30.738383 remotemanager-0.9.3/remotemanager/connection/computers/
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/connection/computers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12849 2023-07-11 12:50:11.000000 remotemanager-0.9.3/remotemanager/connection/computers/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:29:09.000000 remotemanager-0.9.3/remotemanager/connection/computers/example.py
--rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:29:09.000000 remotemanager-0.9.3/remotemanager/connection/computers/options.py
--rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 09:38:01.000000 remotemanager-0.9.3/remotemanager/connection/computers/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:29:09.000000 remotemanager-0.9.3/remotemanager/connection/detect_locale_error.py
--rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/connection/testing_object.py
--rw-rw-rw-   0 root         (0) root         (0)    26008 2023-07-19 14:27:58.000000 remotemanager-0.9.3/remotemanager/connection/url.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:14:30.738383 remotemanager-0.9.3/remotemanager/dataset/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    53942 2023-07-21 09:25:26.000000 remotemanager-0.9.3/remotemanager/dataset/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     9729 2023-07-20 13:52:59.000000 remotemanager-0.9.3/remotemanager/dataset/dependency.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2023-07-12 13:38:06.000000 remotemanager-0.9.3/remotemanager/dataset/lazy_append.py
--rw-rw-rw-   0 root         (0) root         (0)    22294 2023-07-21 09:25:26.000000 remotemanager-0.9.3/remotemanager/dataset/runner.py
--rw-rw-rw-   0 root         (0) root         (0)     2065 2023-07-18 13:45:10.000000 remotemanager-0.9.3/remotemanager/dataset/runnerstates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:14:30.738383 remotemanager-0.9.3/remotemanager/jupyter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.9.3/remotemanager/jupyter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5186 2023-07-18 09:05:28.000000 remotemanager-0.9.3/remotemanager/jupyter/magic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:14:30.742383 remotemanager-0.9.3/remotemanager/logging/
--rw-rw-rw-   0 root         (0) root         (0)     4341 2023-06-14 09:06:03.000000 remotemanager-0.9.3/remotemanager/logging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:38.000000 remotemanager-0.9.3/remotemanager/logging/log.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.9.3/remotemanager/logging/quiet.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.9.3/remotemanager/logging/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/logging/verbosity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:14:30.742383 remotemanager-0.9.3/remotemanager/serialisation/
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-14 07:47:50.000000 remotemanager-0.9.3/remotemanager/serialisation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/serialisation/serial.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.9.3/remotemanager/serialisation/serialdill.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.9.3/remotemanager/serialisation/serialjson.py
--rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/serialisation/serialjsonpickle.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/serialisation/serialyaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:14:30.742383 remotemanager-0.9.3/remotemanager/storage/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/storage/database.py
--rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.9.3/remotemanager/storage/function.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/storage/remotefunction.py
--rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:31.000000 remotemanager-0.9.3/remotemanager/storage/sendablemixin.py
--rw-rw-rw-   0 root         (0) root         (0)     3696 2023-07-18 13:45:10.000000 remotemanager-0.9.3/remotemanager/storage/trackedfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:14:30.742383 remotemanager-0.9.3/remotemanager/transport/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/transport/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/transport/cp.py
--rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.9.3/remotemanager/transport/rsync.py
--rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:35.000000 remotemanager-0.9.3/remotemanager/transport/scp.py
--rw-rw-rw-   0 root         (0) root         (0)    10027 2023-07-18 09:05:28.000000 remotemanager-0.9.3/remotemanager/transport/transport.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:14:30.742383 remotemanager-0.9.3/remotemanager/utils/
--rw-rw-rw-   0 root         (0) root         (0)     5390 2023-07-18 13:45:10.000000 remotemanager-0.9.3/remotemanager/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/utils/flags.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/utils/uuid.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 12:56:19.000000 remotemanager-0.9.3/remotemanager/utils/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 11:14:30.738383 remotemanager-0.9.3/remotemanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1278 2023-07-21 11:14:30.000000 remotemanager-0.9.3/remotemanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1863 2023-07-21 11:14:30.000000 remotemanager-0.9.3/remotemanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 11:14:30.000000 remotemanager-0.9.3/remotemanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      163 2023-07-21 11:14:30.000000 remotemanager-0.9.3/remotemanager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-21 11:14:30.000000 remotemanager-0.9.3/remotemanager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 11:14:30.742383 remotemanager-0.9.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.9.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:05:14.306562 remotemanager-0.9.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.9.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-07-25 13:05:14.306562 remotemanager-0.9.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:45:06.000000 remotemanager-0.9.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1367 2023-07-25 12:11:06.000000 remotemanager-0.9.4/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:05:14.298562 remotemanager-0.9.4/remotemanager/
+-rw-rw-rw-   0 root         (0) root         (0)      481 2023-07-25 12:11:06.000000 remotemanager-0.9.4/remotemanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:05:14.298562 remotemanager-0.9.4/remotemanager/connection/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/connection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15806 2023-06-14 09:06:03.000000 remotemanager-0.9.4/remotemanager/connection/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:05:14.298562 remotemanager-0.9.4/remotemanager/connection/computers/
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/connection/computers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12849 2023-07-11 12:50:11.000000 remotemanager-0.9.4/remotemanager/connection/computers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:29:09.000000 remotemanager-0.9.4/remotemanager/connection/computers/example.py
+-rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:29:09.000000 remotemanager-0.9.4/remotemanager/connection/computers/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 09:38:01.000000 remotemanager-0.9.4/remotemanager/connection/computers/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:29:09.000000 remotemanager-0.9.4/remotemanager/connection/detect_locale_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/connection/testing_object.py
+-rw-rw-rw-   0 root         (0) root         (0)    26008 2023-07-19 14:27:58.000000 remotemanager-0.9.4/remotemanager/connection/url.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:05:14.302562 remotemanager-0.9.4/remotemanager/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    54208 2023-07-25 12:11:06.000000 remotemanager-0.9.4/remotemanager/dataset/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)    10077 2023-07-25 12:11:06.000000 remotemanager-0.9.4/remotemanager/dataset/dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2023-07-12 13:38:06.000000 remotemanager-0.9.4/remotemanager/dataset/lazy_append.py
+-rw-rw-rw-   0 root         (0) root         (0)    22571 2023-07-25 12:11:06.000000 remotemanager-0.9.4/remotemanager/dataset/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     2609 2023-07-24 14:12:05.000000 remotemanager-0.9.4/remotemanager/dataset/runnerstates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:05:14.302562 remotemanager-0.9.4/remotemanager/jupyter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.9.4/remotemanager/jupyter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5186 2023-07-18 09:05:28.000000 remotemanager-0.9.4/remotemanager/jupyter/magic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:05:14.302562 remotemanager-0.9.4/remotemanager/logging/
+-rw-rw-rw-   0 root         (0) root         (0)     4341 2023-06-14 09:06:03.000000 remotemanager-0.9.4/remotemanager/logging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:38.000000 remotemanager-0.9.4/remotemanager/logging/log.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.9.4/remotemanager/logging/quiet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.9.4/remotemanager/logging/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/logging/verbosity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:05:14.302562 remotemanager-0.9.4/remotemanager/serialisation/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-14 07:47:50.000000 remotemanager-0.9.4/remotemanager/serialisation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/serialisation/serial.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.9.4/remotemanager/serialisation/serialdill.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.9.4/remotemanager/serialisation/serialjson.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/serialisation/serialjsonpickle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/serialisation/serialyaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:05:14.302562 remotemanager-0.9.4/remotemanager/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/storage/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.9.4/remotemanager/storage/function.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/storage/remotefunction.py
+-rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:31.000000 remotemanager-0.9.4/remotemanager/storage/sendablemixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3696 2023-07-18 13:45:10.000000 remotemanager-0.9.4/remotemanager/storage/trackedfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:05:14.306562 remotemanager-0.9.4/remotemanager/transport/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/transport/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/transport/cp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.9.4/remotemanager/transport/rsync.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:35.000000 remotemanager-0.9.4/remotemanager/transport/scp.py
+-rw-rw-rw-   0 root         (0) root         (0)    10027 2023-07-18 09:05:28.000000 remotemanager-0.9.4/remotemanager/transport/transport.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:05:14.306562 remotemanager-0.9.4/remotemanager/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     5390 2023-07-18 13:45:10.000000 remotemanager-0.9.4/remotemanager/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/utils/flags.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/utils/uuid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 12:56:19.000000 remotemanager-0.9.4/remotemanager/utils/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:05:14.298562 remotemanager-0.9.4/remotemanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-07-25 13:05:14.000000 remotemanager-0.9.4/remotemanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-07-25 13:05:14.000000 remotemanager-0.9.4/remotemanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 13:05:14.000000 remotemanager-0.9.4/remotemanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      163 2023-07-25 13:05:14.000000 remotemanager-0.9.4/remotemanager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-25 13:05:14.000000 remotemanager-0.9.4/remotemanager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 13:05:14.306562 remotemanager-0.9.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.9.4/setup.py
```

### Comparing `remotemanager-0.9.3/LICENSE` & `remotemanager-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.3/PKG-INFO` & `remotemanager-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.9.3
+Version: 0.9.4
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.9.3/README.md` & `remotemanager-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.3/pyproject.toml` & `remotemanager-0.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 [tool.pytest.ini_options]
 addopts = "--nbval --cov=remotemanager --cov-report term-missing --cov-append --nbval-sanitize-with ./tests/uuid_sanitise.cfg"
 
 [tool.coverage.report]
 omit = ["remotemanager/connection/computers/*"]
 
 [tool.bumpver]
-current_version = "0.9.3"
+current_version = "0.9.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "[clean] bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `remotemanager-0.9.3/remotemanager/connection/cmd.py` & `remotemanager-0.9.4/remotemanager/connection/cmd.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.3/remotemanager/connection/computers/base.py` & `remotemanager-0.9.4/remotemanager/connection/computers/base.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.3/remotemanager/connection/computers/example.py` & `remotemanager-0.9.4/remotemanager/connection/computers/example.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.3/remotemanager/connection/computers/options.py` & `remotemanager-0.9.4/remotemanager/connection/computers/options.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.3/remotemanager/connection/computers/parsers.py` & `remotemanager-0.9.4/remotemanager/connection/computers/parsers.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.3/remotemanager/connection/testing_object.py` & `remotemanager-0.9.4/remotemanager/connection/testing_object.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.3/remotemanager/connection/url.py` & `remotemanager-0.9.4/remotemanager/connection/url.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.3/remotemanager/dataset/dataset.py` & `remotemanager-0.9.4/remotemanager/dataset/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1269,15 +1269,15 @@
 
         if uuids is not None:
             self._logger.runtime(f"running only runners {format_iterable(uuids)}")
 
         # first step is to handle the writing of the scripts to the local dir
         # the runners take care of this
         runners_to_update = []
-        master_content = [f"export {self.main_dir_env}=$PWD\n"]
+        master_content = ["sourcedir=$PWD"]
         goahead = False
         asynchronous = True  # should always be updated in the loop
         for runner in self.runners:
             if uuids is not None and runner.uuid not in uuids:
                 self._logger.runtime(f"skipping {runner} (uuid {runner.short_uuid})")
                 continue
 
@@ -1309,14 +1309,16 @@
             runline.append(f"{submitter} {jobfile} " f"2>> {errorpath}")
 
             # get relative path to jobscript, but we must cd into it to stop any
             # run_dirs being created in the wrong remote
             if self.remote_dir != runner.remote_dir:
                 runline.insert(0, f"cd {jobpath} && ")
 
+            runline.append(f"$sourcedir/{self.repofile.name}")
+
             asynchronous = runner._run_args_temp["asynchronous"]
             if asynchronous and submitter == "bash":
                 self._logger.debug('appending "&" for async run')
                 runline.append("&")
 
             for file in runner.extra_files["send"]:
                 self.transport.queue_for_push(
@@ -1642,14 +1644,24 @@
 
         Returns (list):
             runner.result for each runner
         """
         self._logger.runtime("#### Dataset errors called")
         return [r.error for r in self.runners]
 
+    @property
+    def failed(self) -> list:
+        """
+        Returns a list of failed runners
+
+        Returns:
+            list of failed runners
+        """
+        return [r for r in self.runners if r.state.failed]
+
     def avoid_runtime(self) -> None:
         """
         Call for last_runtime sensitive operations such as is_finished and fetch_results
 
         Waits for 1s if we're too close to the saved _last_run time
 
         Returns:
```

### Comparing `remotemanager-0.9.3/remotemanager/dataset/dependency.py` & `remotemanager-0.9.4/remotemanager/dataset/dependency.py`

 * *Files 3% similar despite different names*

```diff
@@ -155,15 +155,16 @@
                 ds.runners[-1]._dependency_info["parent_import"] = lstr
 
             tmp = []
             for child in self.get_children(ds):
                 runner = child.runners[-1]
                 tmp.append(
                     f"{child.url.submitter} {runner.jobscript.name} "
-                    f"2>> {runner.errorfile.name}"
+                    f"2>> {runner.errorfile.name} "
+                    f"$PWD/{datasets[0].repofile.name}"
                 )
 
             ds.runners[-1]._dependency_info["child_submit"] = tmp
 
             if not lazy:
                 ds.database.update(ds.pack())
 
@@ -211,15 +212,15 @@
             o.write("\n")
             o.write(first.serialiser.loadfunc())
 
         first.transport.queue_for_push(first.repofile)
 
         # and now a master script to kick off the chains
         # we need the export for ALL datasets
-        master_content = [f"export {first.main_dir_env}=$PWD\n"]
+        master_content = []
 
         for ds in ds_store:
             # reuse the store as a list of runner uuids for runners_to_update
             ds_store[ds] = []
             for runner in ds.runners:
                 ready = runner.stage(
                     python=ds.url.python,
@@ -233,26 +234,32 @@
                 # is handled by the jobscripts
                 if ds == first:
                     submitter = ds.url.submitter
                     jobscript = runner.jobscript.relative_remote_path(
                         ds.master_script.remote_dir
                     )
                     jobpath, jobfile = os.path.split(jobscript)
+                    errorpath = runner.errorfile.relative_remote_path(runner.remote_dir)
+                    runline = []
+                    if runner.remote_dir != runner.run_path:
+                        runline.append(f"mkdir -p {runner.run_dir} &&")
 
-                    runline = f"{submitter} {jobfile} " f"2>> {runner.errorfile.name}"
+                    runline.append(f"{submitter} {jobfile} " f"2>> {errorpath}")
 
                     if ds.remote_dir != runner.remote_dir:
-                        runline = f"cd {jobpath} && " + runline
+                        runline.insert(0, f"cd {jobpath} && ")
+
+                    runline.append(f"$PWD/{first.repofile.name}")
 
                     asynchronous = runner.run_args["asynchronous"]
                     if asynchronous and submitter == "bash":
                         ds._logger.debug('appending "&" for async run')
-                        runline += f" &"
+                        runline.append("&")
 
-                    master_content.append(runline)
+                    master_content.append(" ".join(runline))
 
                 first.transport.queue_for_push(runner.jobscript)
                 first.transport.queue_for_push(runner.runfile)
 
                 for file in runner.extra_files["send"]:
                     first.transport.queue_for_push(
                         os.path.split(file)[1],
```

### Comparing `remotemanager-0.9.3/remotemanager/dataset/lazy_append.py` & `remotemanager-0.9.4/remotemanager/dataset/lazy_append.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.3/remotemanager/dataset/runner.py` & `remotemanager-0.9.4/remotemanager/dataset/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -504,18 +504,19 @@
 
         # python file writing
         # if repo is not overidden by a dependency, generate the import path here
         if repo is None:
             repo = f"${self.parent.main_dir_env}/{self.parent.repofile.name}"
 
         errorpath = self.errorfile.relative_remote_path(self.run_path)
+        dir_env_name = f"DIR_{self.short_uuid}"
         # script proper
         runscript = [
             f"import importlib.util, os",
-            f"path = os.path.expandvars('{repo}')",
+            f"path = os.path.expandvars('${dir_env_name}')",
             f"runtime = os.path.getmtime(path)",
             f"spec = importlib.util.spec_from_file_location('repo', path)",
             f"repo = importlib.util.module_from_spec(spec)",
             f"spec.loader.exec_module(repo)\n",
             argline,
             f"result = repo.{self.parent.function.name}(**kwargs)",
             f"# if the error file mtime (created at run) has changed, don't output",
@@ -532,20 +533,24 @@
         # initialise script with whatever the parent url needs
         tmp = []
         if not avoid_nodes:
             tmp.append(self.parent._script_sub(**self._run_args_temp))
         if self.run_path != self.remote_dir:
             self._logger.debug("run dir is separate to remote dir, appending extras")
             submit = (
+                f"export {dir_env_name}=$1\n"
                 f"pydir=$PWD\n"
                 f"cd {self.run_dir} && "
                 f"{python} ${{pydir}}/{self.runfile.name} 2>> {errorpath}"
             )
         else:
-            submit = f"{python} {self.runfile.name} 2>> {errorpath}"
+            submit = (
+                f"export {dir_env_name}=$1\n"
+                f"{python} {self.runfile.name} 2>> {errorpath}"
+            )
             self._logger.debug(f"directly using script {submit}")
         # append the submission lines
         tmp.append(submit)
         # if this runner has children, append the lines to submit them
         for line in self._dependency_info.get("child_submit", []):
             tmp.append(line)
         self.jobscript.write("\n".join(tmp))
@@ -596,23 +601,25 @@
             return True
 
         self._logger.runtime("Not marked completed, returning False")
         return False
 
     def read_local_files(self):
         satisfied = False
+        success = False
         if self.state == "reset":
             self._logger.runtime("runner is in a reset state, ignoring file read")
             return
 
         if os.path.isfile(self.resultfile.local):
             if os.path.getmtime(self.resultfile.local) > self.last_submitted:
                 self._logger.runtime("reading recent results file")
                 self.result = self.parent.serialiser.load(self.resultfile.local)
                 satisfied = True
+                success = True
             else:
                 self._logger.runtime("local results file is outdated")
                 satisfied = False
 
         if os.path.isfile(self.errorfile.local):
             if os.path.getmtime(self.errorfile.local) > self.last_submitted:
                 self._logger.runtime("reading recent error file")
@@ -620,14 +627,15 @@
                 satisfied = True
             else:
                 self._logger.runtime("local error file is outdated")
                 satisfied = False
 
         if satisfied and not self.state == "satisfied":
             self.state = "satisfied"
+            self.state.success = success
 
     @property
     def result(self):
         self.read_local_files()
         if hasattr(self, "_result"):
             try:
                 if SERIALISED_STORAGE_KEY in self._result:
```

### Comparing `remotemanager-0.9.3/remotemanager/dataset/runnerstates.py` & `remotemanager-0.9.4/remotemanager/dataset/runnerstates.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,20 +16,32 @@
         "submitted": 4,  # confirmed running/queued by presence of an empty error file
         "completed": 5,  # valid result file exists
         "failed": 5,  # valid error file exists
         "satisfied": 6,  # files have been retrieved
     }
 
     def __init__(self, state: str = None):
+        self._state = None
+        self._success = None
+
         self.state = state
 
+        if self.state == "completed":
+            self.success = True
+        elif self.state == "failed":
+            self.success = False
+
     def __str__(self):
         if self.state is None:
             return "None"
-        return self.state
+        append = ""
+        if self.value > 5:
+            append = f" (failed)" if self.failed else f" (success)"
+
+        return self.state + append
 
     def __repr__(self):
         return f"RunnerState({self.state})"
 
     @property
     def state(self):
         return self._state
@@ -38,14 +50,26 @@
     def state(self, state):
         if state not in RunnerState._states:
             raise ValueError(f"invalid state; {state}")
 
         self._state = state
 
     @property
+    def success(self):
+        return self._success
+
+    @success.setter
+    def success(self, success):
+        self._success = success
+
+    @property
+    def failed(self):
+        return not self.success
+
+    @property
     def value(self):
         return RunnerState._states[self.state]
 
     def _prepare_compare(self, other):
         if not isinstance(other, RunnerState):
             other = RunnerState(other)
```

### Comparing `remotemanager-0.9.3/remotemanager/jupyter/magic.py` & `remotemanager-0.9.4/remotemanager/jupyter/magic.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.3/remotemanager/logging/__init__.py` & `remotemanager-0.9.4/remotemanager/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.3/remotemanager/logging/log.py` & `remotemanager-0.9.4/remotemanager/logging/log.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.3/remotemanager/logging/utils.py` & `remotemanager-0.9.4/remotemanager/logging/utils.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.3/remotemanager/logging/verbosity.py` & `remotemanager-0.9.4/remotemanager/logging/verbosity.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.3/remotemanager/serialisation/__init__.py` & `remotemanager-0.9.4/remotemanager/serialisation/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.3/remotemanager/serialisation/serial.py` & `remotemanager-0.9.4/remotemanager/serialisation/serial.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.3/remotemanager/serialisation/serialjsonpickle.py` & `remotemanager-0.9.4/remotemanager/serialisation/serialjsonpickle.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.3/remotemanager/serialisation/serialyaml.py` & `remotemanager-0.9.4/remotemanager/serialisation/serialyaml.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.3/remotemanager/storage/database.py` & `remotemanager-0.9.4/remotemanager/storage/database.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.3/remotemanager/storage/function.py` & `remotemanager-0.9.4/remotemanager/storage/function.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.3/remotemanager/storage/remotefunction.py` & `remotemanager-0.9.4/remotemanager/storage/remotefunction.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.3/remotemanager/storage/sendablemixin.py` & `remotemanager-0.9.4/remotemanager/storage/sendablemixin.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.3/remotemanager/storage/trackedfile.py` & `remotemanager-0.9.4/remotemanager/storage/trackedfile.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.3/remotemanager/transport/cp.py` & `remotemanager-0.9.4/remotemanager/transport/cp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.3/remotemanager/transport/rsync.py` & `remotemanager-0.9.4/remotemanager/transport/rsync.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.3/remotemanager/transport/scp.py` & `remotemanager-0.9.4/remotemanager/transport/scp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.3/remotemanager/transport/transport.py` & `remotemanager-0.9.4/remotemanager/transport/transport.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.3/remotemanager/utils/__init__.py` & `remotemanager-0.9.4/remotemanager/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.3/remotemanager/utils/flags.py` & `remotemanager-0.9.4/remotemanager/utils/flags.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.3/remotemanager/utils/version.py` & `remotemanager-0.9.4/remotemanager/utils/version.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.9.3/remotemanager.egg-info/PKG-INFO` & `remotemanager-0.9.4/remotemanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.9.3
+Version: 0.9.4
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.9.3/remotemanager.egg-info/SOURCES.txt` & `remotemanager-0.9.4/remotemanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

