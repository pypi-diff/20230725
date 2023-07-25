# Comparing `tmp/dummy_url_wrapper-0.0.8.tar.gz` & `tmp/dummy_url_wrapper-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dummy_url_wrapper-0.0.8.tar", last modified: Mon Jul 17 10:26:47 2023, max compression
+gzip compressed data, was "dummy_url_wrapper-0.0.9.tar", last modified: Tue Jul 25 10:23:11 2023, max compression
```

## Comparing `dummy_url_wrapper-0.0.8.tar` & `dummy_url_wrapper-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-17 10:26:47.078899 dummy_url_wrapper-0.0.8/
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      714 2023-07-17 10:26:47.078899 dummy_url_wrapper-0.0.8/PKG-INFO
-drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-17 10:26:47.078899 dummy_url_wrapper-0.0.8/dummy_url_wrapper/
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       71 2023-07-17 09:13:05.000000 dummy_url_wrapper-0.0.8/dummy_url_wrapper/__init__.py
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)     5320 2023-07-17 09:16:16.000000 dummy_url_wrapper-0.0.8/dummy_url_wrapper/mysdk.py
-drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-17 10:26:47.078899 dummy_url_wrapper-0.0.8/dummy_url_wrapper.egg-info/
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      714 2023-07-17 10:26:47.000000 dummy_url_wrapper-0.0.8/dummy_url_wrapper.egg-info/PKG-INFO
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      269 2023-07-17 10:26:47.000000 dummy_url_wrapper-0.0.8/dummy_url_wrapper.egg-info/SOURCES.txt
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)        1 2023-07-17 10:26:47.000000 dummy_url_wrapper-0.0.8/dummy_url_wrapper.egg-info/dependency_links.txt
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       23 2023-07-17 10:26:47.000000 dummy_url_wrapper-0.0.8/dummy_url_wrapper.egg-info/requires.txt
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       18 2023-07-17 10:26:47.000000 dummy_url_wrapper-0.0.8/dummy_url_wrapper.egg-info/top_level.txt
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       38 2023-07-17 10:26:47.078899 dummy_url_wrapper-0.0.8/setup.cfg
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      886 2023-07-17 10:26:42.000000 dummy_url_wrapper-0.0.8/setup.py
+drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-25 10:23:11.569468 dummy_url_wrapper-0.0.9/
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      416 2023-07-25 10:23:11.569468 dummy_url_wrapper-0.0.9/PKG-INFO
+drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-25 10:23:11.565468 dummy_url_wrapper-0.0.9/dummy_url_wrapper/
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       71 2023-07-17 09:13:05.000000 dummy_url_wrapper-0.0.9/dummy_url_wrapper/__init__.py
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)     9544 2023-07-25 10:19:18.000000 dummy_url_wrapper-0.0.9/dummy_url_wrapper/mysdk.py
+drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-25 10:23:11.569468 dummy_url_wrapper-0.0.9/dummy_url_wrapper.egg-info/
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      416 2023-07-25 10:23:11.000000 dummy_url_wrapper-0.0.9/dummy_url_wrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      269 2023-07-25 10:23:11.000000 dummy_url_wrapper-0.0.9/dummy_url_wrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)        1 2023-07-25 10:23:11.000000 dummy_url_wrapper-0.0.9/dummy_url_wrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       23 2023-07-25 10:23:11.000000 dummy_url_wrapper-0.0.9/dummy_url_wrapper.egg-info/requires.txt
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       18 2023-07-25 10:23:11.000000 dummy_url_wrapper-0.0.9/dummy_url_wrapper.egg-info/top_level.txt
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       38 2023-07-25 10:23:11.569468 dummy_url_wrapper-0.0.9/setup.cfg
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      594 2023-07-25 10:22:56.000000 dummy_url_wrapper-0.0.9/setup.py
```

