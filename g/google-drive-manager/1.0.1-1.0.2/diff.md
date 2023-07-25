# Comparing `tmp/google-drive-manager-1.0.1.tar.gz` & `tmp/google-drive-manager-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-drive-manager-1.0.1.tar", last modified: Mon Jul 24 15:32:31 2023, max compression
+gzip compressed data, was "google-drive-manager-1.0.2.tar", last modified: Tue Jul 25 13:29:29 2023, max compression
```

## Comparing `google-drive-manager-1.0.1.tar` & `google-drive-manager-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 guillaume  (1000) guillaume  (1000)        0 2023-07-24 15:32:31.429062 google-drive-manager-1.0.1/
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)      205 2023-07-24 15:32:31.429062 google-drive-manager-1.0.1/PKG-INFO
-drwxrwxr-x   0 guillaume  (1000) guillaume  (1000)        0 2023-07-24 15:32:31.421062 google-drive-manager-1.0.1/google_drive_manager/
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)        0 2023-07-24 15:14:53.000000 google-drive-manager-1.0.1/google_drive_manager/__init__.py
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)     6774 2023-07-18 13:43:05.000000 google-drive-manager-1.0.1/google_drive_manager/google_drive_manager.py
-drwxrwxr-x   0 guillaume  (1000) guillaume  (1000)        0 2023-07-24 15:32:31.429062 google-drive-manager-1.0.1/google_drive_manager.egg-info/
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)      205 2023-07-24 15:32:31.000000 google-drive-manager-1.0.1/google_drive_manager.egg-info/PKG-INFO
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)      305 2023-07-24 15:32:31.000000 google-drive-manager-1.0.1/google_drive_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)        1 2023-07-24 15:32:31.000000 google-drive-manager-1.0.1/google_drive_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)       61 2023-07-24 15:32:31.000000 google-drive-manager-1.0.1/google_drive_manager.egg-info/requires.txt
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)       21 2023-07-24 15:32:31.000000 google-drive-manager-1.0.1/google_drive_manager.egg-info/top_level.txt
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)       38 2023-07-24 15:32:31.429062 google-drive-manager-1.0.1/setup.cfg
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)      330 2023-07-24 15:31:56.000000 google-drive-manager-1.0.1/setup.py
+drwxrwxr-x   0 guillaume  (1000) guillaume  (1000)        0 2023-07-25 13:29:29.765081 google-drive-manager-1.0.2/
+-rw-rw-r--   0 guillaume  (1000) guillaume  (1000)      310 2023-07-25 13:29:29.765081 google-drive-manager-1.0.2/PKG-INFO
+drwxrwxr-x   0 guillaume  (1000) guillaume  (1000)        0 2023-07-25 13:29:29.753081 google-drive-manager-1.0.2/google_drive_manager/
+-rw-rw-r--   0 guillaume  (1000) guillaume  (1000)        0 2023-07-24 15:14:53.000000 google-drive-manager-1.0.2/google_drive_manager/__init__.py
+-rw-rw-r--   0 guillaume  (1000) guillaume  (1000)    11129 2023-07-25 09:27:53.000000 google-drive-manager-1.0.2/google_drive_manager/google_drive_manager.py
+drwxrwxr-x   0 guillaume  (1000) guillaume  (1000)        0 2023-07-25 13:29:29.761081 google-drive-manager-1.0.2/google_drive_manager.egg-info/
+-rw-rw-r--   0 guillaume  (1000) guillaume  (1000)      310 2023-07-25 13:29:29.000000 google-drive-manager-1.0.2/google_drive_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 guillaume  (1000) guillaume  (1000)      305 2023-07-25 13:29:29.000000 google-drive-manager-1.0.2/google_drive_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 guillaume  (1000) guillaume  (1000)        1 2023-07-25 13:29:29.000000 google-drive-manager-1.0.2/google_drive_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 guillaume  (1000) guillaume  (1000)       61 2023-07-25 13:29:29.000000 google-drive-manager-1.0.2/google_drive_manager.egg-info/requires.txt
+-rw-rw-r--   0 guillaume  (1000) guillaume  (1000)       21 2023-07-25 13:29:29.000000 google-drive-manager-1.0.2/google_drive_manager.egg-info/top_level.txt
+-rw-rw-r--   0 guillaume  (1000) guillaume  (1000)       38 2023-07-25 13:29:29.765081 google-drive-manager-1.0.2/setup.cfg
+-rw-rw-r--   0 guillaume  (1000) guillaume  (1000)      461 2023-07-25 13:28:52.000000 google-drive-manager-1.0.2/setup.py
```

