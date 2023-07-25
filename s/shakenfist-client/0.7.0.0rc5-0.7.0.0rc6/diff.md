# Comparing `tmp/shakenfist-client-0.7.0.0rc5.tar.gz` & `tmp/shakenfist-client-0.7.0.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shakenfist-client-0.7.0.0rc5.tar", last modified: Sun Jul 16 08:19:27 2023, max compression
+gzip compressed data, was "shakenfist-client-0.7.0.0rc6.tar", last modified: Tue Jul 25 06:57:47 2023, max compression
```

## Comparing `shakenfist-client-0.7.0.0rc5.tar` & `shakenfist-client-0.7.0.0rc6.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-07-16 08:19:27.831839 shakenfist-client-0.7.0.0rc5/
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-07-16 08:19:27.823839 shakenfist-client-0.7.0.0rc5/.github/
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-07-16 08:19:27.827839 shakenfist-client-0.7.0.0rc5/.github/workflows/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1048 2022-12-27 01:53:29.000000 shakenfist-client-0.7.0.0rc5/.github/workflows/configure-tests.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8937 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/.github/workflows/functional-tests-debian-10-localhost.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8946 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/.github/workflows/functional-tests-debian-11-slim-primary.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8952 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/.github/workflows/functional-tests-ubuntu-2004-slim-primary.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     9302 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/.github/workflows/functional-tests.tmpl
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1306 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/.github/workflows/python-unit-tests.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       56 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc5/.stestr.conf
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      131 2023-07-16 08:19:27.000000 shakenfist-client-0.7.0.0rc5/AUTHORS
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    11357 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc5/LICENSE
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1006 2023-07-16 08:19:27.831839 shakenfist-client-0.7.0.0rc5/PKG-INFO
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      280 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc5/README.md
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-07-16 08:19:27.827839 shakenfist-client-0.7.0.0rc5/ansible/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    10729 2022-11-20 01:06:18.000000 shakenfist-client-0.7.0.0rc5/ansible/sf_instance.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     3994 2021-11-04 05:09:57.000000 shakenfist-client-0.7.0.0rc5/ansible/sf_network.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     3484 2021-11-04 05:09:57.000000 shakenfist-client-0.7.0.0rc5/ansible/sf_snapshot.py
--rwxrwxr-x   0 parallels  (1000) parallels  (1000)      845 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc5/release.sh
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      398 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/requirements.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      720 2023-07-16 08:19:27.835839 shakenfist-client-0.7.0.0rc5/setup.cfg
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1372 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc5/setup.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-07-16 08:19:27.827839 shakenfist-client-0.7.0.0rc5/shakenfist_client/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/__init__.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    37569 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/apiclient.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-07-16 08:19:27.831839 shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1012 2022-08-09 10:00:30.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/admin.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    13862 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/artifact.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     2492 2022-08-09 10:00:30.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/backup.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     7843 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/blob.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    28703 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/instance.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     3249 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/interface.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      512 2022-01-08 00:34:31.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/label.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8896 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/namespace.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8294 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/network.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     7475 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/node.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     4222 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/main.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-07-16 08:19:27.831839 shakenfist-client-0.7.0.0rc5/shakenfist_client/tests/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/tests/__init__.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    15322 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/tests/test_client_apiclient.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     5829 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/util.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-07-16 08:19:27.827839 shakenfist-client-0.7.0.0rc5/shakenfist_client.egg-info/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1006 2023-07-16 08:19:27.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client.egg-info/PKG-INFO
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1476 2023-07-16 08:19:27.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client.egg-info/SOURCES.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-07-16 08:19:27.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client.egg-info/dependency_links.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       58 2023-07-16 08:19:27.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client.egg-info/entry_points.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-07-16 08:19:27.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client.egg-info/not-zip-safe
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       47 2023-07-16 08:19:27.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client.egg-info/pbr.json
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      129 2023-07-16 08:19:27.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client.egg-info/requires.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       18 2023-07-16 08:19:27.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client.egg-info/top_level.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      164 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/test-requirements.txt
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-07-16 08:19:27.831839 shakenfist-client-0.7.0.0rc5/tools/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      402 2022-12-27 01:53:29.000000 shakenfist-client-0.7.0.0rc5/tools/buffer.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     4017 2022-12-27 01:53:29.000000 shakenfist-client-0.7.0.0rc5/tools/clone_with_depends.py
--rwxrwxr-x   0 parallels  (1000) parallels  (1000)      573 2022-12-27 01:53:29.000000 shakenfist-client-0.7.0.0rc5/tools/flake8wrap.sh
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      899 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/tox.ini
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-07-25 06:57:47.050907 shakenfist-client-0.7.0.0rc6/
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-07-25 06:57:47.038905 shakenfist-client-0.7.0.0rc6/.github/
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-07-25 06:57:47.042906 shakenfist-client-0.7.0.0rc6/.github/workflows/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1048 2022-12-27 01:53:29.000000 shakenfist-client-0.7.0.0rc6/.github/workflows/configure-tests.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8972 2023-07-25 06:57:19.000000 shakenfist-client-0.7.0.0rc6/.github/workflows/functional-tests-debian-10-localhost.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8981 2023-07-25 06:57:19.000000 shakenfist-client-0.7.0.0rc6/.github/workflows/functional-tests-debian-11-slim-primary.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8987 2023-07-25 06:57:19.000000 shakenfist-client-0.7.0.0rc6/.github/workflows/functional-tests-ubuntu-2004-slim-primary.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     9337 2023-07-25 06:57:19.000000 shakenfist-client-0.7.0.0rc6/.github/workflows/functional-tests.tmpl
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1306 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc6/.github/workflows/python-unit-tests.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       56 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc6/.stestr.conf
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      131 2023-07-25 06:57:46.000000 shakenfist-client-0.7.0.0rc6/AUTHORS
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    11357 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc6/LICENSE
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1006 2023-07-25 06:57:47.050907 shakenfist-client-0.7.0.0rc6/PKG-INFO
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      280 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc6/README.md
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-07-25 06:57:47.042906 shakenfist-client-0.7.0.0rc6/ansible/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    10729 2022-11-20 01:06:18.000000 shakenfist-client-0.7.0.0rc6/ansible/sf_instance.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     3994 2021-11-04 05:09:57.000000 shakenfist-client-0.7.0.0rc6/ansible/sf_network.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     3484 2021-11-04 05:09:57.000000 shakenfist-client-0.7.0.0rc6/ansible/sf_snapshot.py
+-rwxrwxr-x   0 parallels  (1000) parallels  (1000)      845 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc6/release.sh
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      398 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc6/requirements.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      720 2023-07-25 06:57:47.054908 shakenfist-client-0.7.0.0rc6/setup.cfg
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1372 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc6/setup.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-07-25 06:57:47.046907 shakenfist-client-0.7.0.0rc6/shakenfist_client/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc6/shakenfist_client/__init__.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    37914 2023-07-25 06:57:19.000000 shakenfist-client-0.7.0.0rc6/shakenfist_client/apiclient.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-07-25 06:57:47.050907 shakenfist-client-0.7.0.0rc6/shakenfist_client/commandline/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1012 2022-08-09 10:00:30.000000 shakenfist-client-0.7.0.0rc6/shakenfist_client/commandline/admin.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    13862 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc6/shakenfist_client/commandline/artifact.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     2492 2022-08-09 10:00:30.000000 shakenfist-client-0.7.0.0rc6/shakenfist_client/commandline/backup.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     7843 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc6/shakenfist_client/commandline/blob.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    28703 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc6/shakenfist_client/commandline/instance.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     3249 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc6/shakenfist_client/commandline/interface.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      512 2022-01-08 00:34:31.000000 shakenfist-client-0.7.0.0rc6/shakenfist_client/commandline/label.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8896 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc6/shakenfist_client/commandline/namespace.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8294 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc6/shakenfist_client/commandline/network.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     7475 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc6/shakenfist_client/commandline/node.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     4222 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc6/shakenfist_client/main.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-07-25 06:57:47.050907 shakenfist-client-0.7.0.0rc6/shakenfist_client/tests/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc6/shakenfist_client/tests/__init__.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    15322 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc6/shakenfist_client/tests/test_client_apiclient.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     5829 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc6/shakenfist_client/util.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-07-25 06:57:47.046907 shakenfist-client-0.7.0.0rc6/shakenfist_client.egg-info/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1006 2023-07-25 06:57:46.000000 shakenfist-client-0.7.0.0rc6/shakenfist_client.egg-info/PKG-INFO
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1476 2023-07-25 06:57:46.000000 shakenfist-client-0.7.0.0rc6/shakenfist_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-07-25 06:57:46.000000 shakenfist-client-0.7.0.0rc6/shakenfist_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       58 2023-07-25 06:57:46.000000 shakenfist-client-0.7.0.0rc6/shakenfist_client.egg-info/entry_points.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-07-25 06:57:46.000000 shakenfist-client-0.7.0.0rc6/shakenfist_client.egg-info/not-zip-safe
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       47 2023-07-25 06:57:46.000000 shakenfist-client-0.7.0.0rc6/shakenfist_client.egg-info/pbr.json
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      129 2023-07-25 06:57:46.000000 shakenfist-client-0.7.0.0rc6/shakenfist_client.egg-info/requires.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       18 2023-07-25 06:57:46.000000 shakenfist-client-0.7.0.0rc6/shakenfist_client.egg-info/top_level.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      164 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc6/test-requirements.txt
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-07-25 06:57:47.050907 shakenfist-client-0.7.0.0rc6/tools/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      402 2022-12-27 01:53:29.000000 shakenfist-client-0.7.0.0rc6/tools/buffer.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     4017 2022-12-27 01:53:29.000000 shakenfist-client-0.7.0.0rc6/tools/clone_with_depends.py
+-rwxrwxr-x   0 parallels  (1000) parallels  (1000)      573 2022-12-27 01:53:29.000000 shakenfist-client-0.7.0.0rc6/tools/flake8wrap.sh
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      899 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc6/tox.ini
```

### Comparing `shakenfist-client-0.7.0.0rc5/.github/workflows/configure-tests.py` & `shakenfist-client-0.7.0.0rc6/.github/workflows/configure-tests.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc5/.github/workflows/functional-tests-debian-10-localhost.yml` & `shakenfist-client-0.7.0.0rc6/.github/workflows/functional-tests-debian-10-localhost.yml`

 * *Files 1% similar despite different names*

```diff
@@ -214,9 +214,10 @@
 
           zip -rq artifacts/bundle.zip bundle/*
 
       - uses: actions/upload-artifact@v3
         if: ${{ ! cancelled() }}
         with:
           name: bundle.zip
-          retention-days: 14
+          retention-days: 90
+          if-no-files-found: error
           path: ${{ github.workspace }}/artifacts/bundle.zip
```

### Comparing `shakenfist-client-0.7.0.0rc5/.github/workflows/functional-tests-debian-11-slim-primary.yml` & `shakenfist-client-0.7.0.0rc6/.github/workflows/functional-tests-debian-11-slim-primary.yml`

 * *Files 1% similar despite different names*

```diff
@@ -214,9 +214,10 @@
 
           zip -rq artifacts/bundle.zip bundle/*
 
       - uses: actions/upload-artifact@v3
         if: ${{ ! cancelled() }}
         with:
           name: bundle.zip
-          retention-days: 14
+          retention-days: 90
+          if-no-files-found: error
           path: ${{ github.workspace }}/artifacts/bundle.zip
```

### Comparing `shakenfist-client-0.7.0.0rc5/.github/workflows/functional-tests-ubuntu-2004-slim-primary.yml` & `shakenfist-client-0.7.0.0rc6/.github/workflows/functional-tests-ubuntu-2004-slim-primary.yml`

 * *Files 1% similar despite different names*

```diff
@@ -214,9 +214,10 @@
 
           zip -rq artifacts/bundle.zip bundle/*
 
       - uses: actions/upload-artifact@v3
         if: ${{ ! cancelled() }}
         with:
           name: bundle.zip
-          retention-days: 14
+          retention-days: 90
+          if-no-files-found: error
           path: ${{ github.workspace }}/artifacts/bundle.zip
```

### Comparing `shakenfist-client-0.7.0.0rc5/.github/workflows/functional-tests.tmpl` & `shakenfist-client-0.7.0.0rc6/.github/workflows/functional-tests.tmpl`

 * *Files 1% similar despite different names*

```diff
@@ -214,9 +214,10 @@
 
           zip -rq artifacts/bundle.zip bundle/*
 
       - uses: actions/upload-artifact@v3
         if: {% raw %}${{{% endraw %} ! cancelled() {% raw %}}}{% endraw %}
         with:
           name: bundle.zip
-          retention-days: 14
+          retention-days: 90
+          if-no-files-found: error
           path: {% raw %}${{{% endraw %} github.workspace {% raw %}}}{% endraw %}/artifacts/bundle.zip
```

### Comparing `shakenfist-client-0.7.0.0rc5/.github/workflows/python-unit-tests.yml` & `shakenfist-client-0.7.0.0rc6/.github/workflows/python-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc5/LICENSE` & `shakenfist-client-0.7.0.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc5/PKG-INFO` & `shakenfist-client-0.7.0.0rc6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shakenfist-client
-Version: 0.7.0.0rc5
+Version: 0.7.0.0rc6
 Summary: Shaken Fist: an opinionated minimal cloud
 Home-page: https://madebymikal.com/shakenfist
 Author: Michael Still
 Author-email: mikal@stillhq.com
 License: Apache2
 Description: Python REST API client for Shaken Fist
         ======================================
```

### Comparing `shakenfist-client-0.7.0.0rc5/ansible/sf_instance.py` & `shakenfist-client-0.7.0.0rc6/ansible/sf_instance.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc5/ansible/sf_network.py` & `shakenfist-client-0.7.0.0rc6/ansible/sf_network.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc5/ansible/sf_snapshot.py` & `shakenfist-client-0.7.0.0rc6/ansible/sf_snapshot.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc5/release.sh` & `shakenfist-client-0.7.0.0rc6/release.sh`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc5/setup.cfg` & `shakenfist-client-0.7.0.0rc6/setup.cfg`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc5/setup.py` & `shakenfist-client-0.7.0.0rc6/setup.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc5/shakenfist_client/apiclient.py` & `shakenfist-client-0.7.0.0rc6/shakenfist_client/apiclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -980,11 +980,19 @@
         if not self.check_capability('agentoperations-crud'):
             raise IncapableException(
                 'The API server version you are talking to does not support '
                 'agent operations.')
 
         self._request_url('DELETE', '/agentoperations/' + operation_uuid)
 
+    def get_cluster_cacert(self):
+        if not self.check_capability('cluster-cacert'):
+            raise IncapableException(
+                'The API server version you are talking to does not support '
+                'fetching a CA certificate for the cluster.')
+        r = self._request_url('GET', '/admin/cacert')
+        return r.text
+
 
 def get_user_agent():
     sf_version = VersionInfo('shakenfist_client').version_string()
     return 'Mozilla/5.0 (Ubuntu; Linux x86_64) Shaken Fist/%s' % sf_version
```

### Comparing `shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/admin.py` & `shakenfist-client-0.7.0.0rc6/shakenfist_client/commandline/admin.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/artifact.py` & `shakenfist-client-0.7.0.0rc6/shakenfist_client/commandline/artifact.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/backup.py` & `shakenfist-client-0.7.0.0rc6/shakenfist_client/commandline/backup.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/blob.py` & `shakenfist-client-0.7.0.0rc6/shakenfist_client/commandline/blob.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/instance.py` & `shakenfist-client-0.7.0.0rc6/shakenfist_client/commandline/instance.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/interface.py` & `shakenfist-client-0.7.0.0rc6/shakenfist_client/commandline/interface.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/label.py` & `shakenfist-client-0.7.0.0rc6/shakenfist_client/commandline/label.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/namespace.py` & `shakenfist-client-0.7.0.0rc6/shakenfist_client/commandline/namespace.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/network.py` & `shakenfist-client-0.7.0.0rc6/shakenfist_client/commandline/network.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/node.py` & `shakenfist-client-0.7.0.0rc6/shakenfist_client/commandline/node.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc5/shakenfist_client/main.py` & `shakenfist-client-0.7.0.0rc6/shakenfist_client/main.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc5/shakenfist_client/tests/test_client_apiclient.py` & `shakenfist-client-0.7.0.0rc6/shakenfist_client/tests/test_client_apiclient.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc5/shakenfist_client/util.py` & `shakenfist-client-0.7.0.0rc6/shakenfist_client/util.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc5/shakenfist_client.egg-info/PKG-INFO` & `shakenfist-client-0.7.0.0rc6/shakenfist_client.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shakenfist-client
-Version: 0.7.0.0rc5
+Version: 0.7.0.0rc6
 Summary: Shaken Fist: an opinionated minimal cloud
 Home-page: https://madebymikal.com/shakenfist
 Author: Michael Still
 Author-email: mikal@stillhq.com
 License: Apache2
 Description: Python REST API client for Shaken Fist
         ======================================
```

### Comparing `shakenfist-client-0.7.0.0rc5/shakenfist_client.egg-info/SOURCES.txt` & `shakenfist-client-0.7.0.0rc6/shakenfist_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc5/tools/clone_with_depends.py` & `shakenfist-client-0.7.0.0rc6/tools/clone_with_depends.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc5/tools/flake8wrap.sh` & `shakenfist-client-0.7.0.0rc6/tools/flake8wrap.sh`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc5/tox.ini` & `shakenfist-client-0.7.0.0rc6/tox.ini`

 * *Files identical despite different names*

