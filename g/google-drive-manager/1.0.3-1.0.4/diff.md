# Comparing `tmp/google-drive-manager-1.0.3.tar.gz` & `tmp/google-drive-manager-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-drive-manager-1.0.3.tar", last modified: Tue Jul 25 13:38:55 2023, max compression
+gzip compressed data, was "google-drive-manager-1.0.4.tar", last modified: Tue Jul 25 13:41:36 2023, max compression
```

## Comparing `google-drive-manager-1.0.3.tar` & `google-drive-manager-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 guillaume  (1000) guillaume  (1000)        0 2023-07-25 13:38:55.580016 google-drive-manager-1.0.3/
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)     1293 2023-07-25 13:38:55.580016 google-drive-manager-1.0.3/PKG-INFO
-drwxrwxr-x   0 guillaume  (1000) guillaume  (1000)        0 2023-07-25 13:38:55.572016 google-drive-manager-1.0.3/google_drive_manager/
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)        0 2023-07-24 15:14:53.000000 google-drive-manager-1.0.3/google_drive_manager/__init__.py
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)    11129 2023-07-25 09:27:53.000000 google-drive-manager-1.0.3/google_drive_manager/google_drive_manager.py
-drwxrwxr-x   0 guillaume  (1000) guillaume  (1000)        0 2023-07-25 13:38:55.580016 google-drive-manager-1.0.3/google_drive_manager.egg-info/
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)     1293 2023-07-25 13:38:55.000000 google-drive-manager-1.0.3/google_drive_manager.egg-info/PKG-INFO
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)      305 2023-07-25 13:38:55.000000 google-drive-manager-1.0.3/google_drive_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)        1 2023-07-25 13:38:55.000000 google-drive-manager-1.0.3/google_drive_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)       61 2023-07-25 13:38:55.000000 google-drive-manager-1.0.3/google_drive_manager.egg-info/requires.txt
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)       21 2023-07-25 13:38:55.000000 google-drive-manager-1.0.3/google_drive_manager.egg-info/top_level.txt
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)       38 2023-07-25 13:38:55.580016 google-drive-manager-1.0.3/setup.cfg
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)     1371 2023-07-25 13:38:52.000000 google-drive-manager-1.0.3/setup.py
+drwxrwxr-x   0 guillaume  (1000) guillaume  (1000)        0 2023-07-25 13:41:36.391736 google-drive-manager-1.0.4/
+-rw-rw-r--   0 guillaume  (1000) guillaume  (1000)     1006 2023-07-25 13:41:36.391736 google-drive-manager-1.0.4/PKG-INFO
+drwxrwxr-x   0 guillaume  (1000) guillaume  (1000)        0 2023-07-25 13:41:36.387736 google-drive-manager-1.0.4/google_drive_manager/
+-rw-rw-r--   0 guillaume  (1000) guillaume  (1000)        0 2023-07-24 15:14:53.000000 google-drive-manager-1.0.4/google_drive_manager/__init__.py
+-rw-rw-r--   0 guillaume  (1000) guillaume  (1000)    11129 2023-07-25 09:27:53.000000 google-drive-manager-1.0.4/google_drive_manager/google_drive_manager.py
+drwxrwxr-x   0 guillaume  (1000) guillaume  (1000)        0 2023-07-25 13:41:36.391736 google-drive-manager-1.0.4/google_drive_manager.egg-info/
+-rw-rw-r--   0 guillaume  (1000) guillaume  (1000)     1006 2023-07-25 13:41:36.000000 google-drive-manager-1.0.4/google_drive_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 guillaume  (1000) guillaume  (1000)      305 2023-07-25 13:41:36.000000 google-drive-manager-1.0.4/google_drive_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 guillaume  (1000) guillaume  (1000)        1 2023-07-25 13:41:36.000000 google-drive-manager-1.0.4/google_drive_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 guillaume  (1000) guillaume  (1000)       61 2023-07-25 13:41:36.000000 google-drive-manager-1.0.4/google_drive_manager.egg-info/requires.txt
+-rw-rw-r--   0 guillaume  (1000) guillaume  (1000)       21 2023-07-25 13:41:36.000000 google-drive-manager-1.0.4/google_drive_manager.egg-info/top_level.txt
+-rw-rw-r--   0 guillaume  (1000) guillaume  (1000)       38 2023-07-25 13:41:36.391736 google-drive-manager-1.0.4/setup.cfg
+-rw-rw-r--   0 guillaume  (1000) guillaume  (1000)     1068 2023-07-25 13:41:17.000000 google-drive-manager-1.0.4/setup.py
```

### Comparing `google-drive-manager-1.0.3/google_drive_manager/google_drive_manager.py` & `google-drive-manager-1.0.4/google_drive_manager/google_drive_manager.py`

 * *Files identical despite different names*

