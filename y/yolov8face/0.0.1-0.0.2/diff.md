# Comparing `tmp/yolov8face-0.0.1.tar.gz` & `tmp/yolov8face-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yolov8face-0.0.1.tar", last modified: Sun Jul 23 10:50:39 2023, max compression
+gzip compressed data, was "yolov8face-0.0.2.tar", last modified: Tue Jul 25 19:50:15 2023, max compression
```

## Comparing `yolov8face-0.0.1.tar` & `yolov8face-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-07-23 10:50:39.907153 yolov8face-0.0.1/
--rw-rw-r--   0 harsh     (1000) harsh     (1000)    35149 2023-07-22 13:32:13.000000 yolov8face-0.0.1/LICENSE
--rw-rw-r--   0 harsh     (1000) harsh     (1000)      120 2023-07-23 10:50:39.907153 yolov8face-0.0.1/PKG-INFO
--rw-rw-r--   0 harsh     (1000) harsh     (1000)      280 2023-07-22 13:32:13.000000 yolov8face-0.0.1/README.md
--rw-rw-r--   0 harsh     (1000) harsh     (1000)       38 2023-07-23 10:50:39.907153 yolov8face-0.0.1/setup.cfg
--rw-rw-r--   0 harsh     (1000) harsh     (1000)      253 2023-07-20 15:09:36.000000 yolov8face-0.0.1/setup.py
-drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-07-23 10:50:39.907153 yolov8face-0.0.1/yolov8face.egg-info/
--rw-rw-r--   0 harsh     (1000) harsh     (1000)      120 2023-07-23 10:50:39.000000 yolov8face-0.0.1/yolov8face.egg-info/PKG-INFO
--rw-rw-r--   0 harsh     (1000) harsh     (1000)      195 2023-07-23 10:50:39.000000 yolov8face-0.0.1/yolov8face.egg-info/SOURCES.txt
--rw-rw-r--   0 harsh     (1000) harsh     (1000)        1 2023-07-23 10:50:39.000000 yolov8face-0.0.1/yolov8face.egg-info/dependency_links.txt
--rw-rw-r--   0 harsh     (1000) harsh     (1000)       20 2023-07-23 10:50:39.000000 yolov8face-0.0.1/yolov8face.egg-info/requires.txt
--rw-rw-r--   0 harsh     (1000) harsh     (1000)        1 2023-07-23 10:50:39.000000 yolov8face-0.0.1/yolov8face.egg-info/top_level.txt
+drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-07-25 19:50:15.091105 yolov8face-0.0.2/
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)    35149 2023-07-22 13:32:13.000000 yolov8face-0.0.2/LICENSE
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)     1585 2023-07-25 19:50:15.091105 yolov8face-0.0.2/PKG-INFO
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)     1424 2023-07-25 19:45:20.000000 yolov8face-0.0.2/README.md
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)       38 2023-07-25 19:50:15.091105 yolov8face-0.0.2/setup.cfg
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)      563 2023-07-25 19:48:52.000000 yolov8face-0.0.2/setup.py
+drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-07-25 19:50:15.091105 yolov8face-0.0.2/yolov8face.egg-info/
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)     1585 2023-07-25 19:50:15.000000 yolov8face-0.0.2/yolov8face.egg-info/PKG-INFO
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)      195 2023-07-25 19:50:15.000000 yolov8face-0.0.2/yolov8face.egg-info/SOURCES.txt
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)        1 2023-07-25 19:50:15.000000 yolov8face-0.0.2/yolov8face.egg-info/dependency_links.txt
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)       20 2023-07-25 19:50:15.000000 yolov8face-0.0.2/yolov8face.egg-info/requires.txt
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)        1 2023-07-25 19:50:15.000000 yolov8face-0.0.2/yolov8face.egg-info/top_level.txt
```

### Comparing `yolov8face-0.0.1/LICENSE` & `yolov8face-0.0.2/LICENSE`

 * *Files identical despite different names*

