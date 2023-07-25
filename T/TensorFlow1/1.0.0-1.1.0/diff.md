# Comparing `tmp/TensorFlow1-1.0.0.tar.gz` & `tmp/TensorFlow1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TensorFlow1-1.0.0.tar", last modified: Tue Jul 25 14:41:22 2023, max compression
+gzip compressed data, was "TensorFlow1-1.1.0.tar", last modified: Tue Jul 25 14:54:24 2023, max compression
```

## Comparing `TensorFlow1-1.0.0.tar` & `TensorFlow1-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 14:41:22.596226 TensorFlow1-1.0.0/
--rw-rw-rw-   0        0        0      186 2023-07-25 14:41:22.596226 TensorFlow1-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-25 12:12:58.000000 TensorFlow1-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 14:41:22.563251 TensorFlow1-1.0.0/TensorFlow1/
--rw-rw-rw-   0        0        0    17833 2023-07-25 14:37:39.000000 TensorFlow1-1.0.0/TensorFlow1/TensorFlow.py
--rw-rw-rw-   0        0        0       28 2023-07-25 14:37:45.000000 TensorFlow1-1.0.0/TensorFlow1/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 14:41:22.593235 TensorFlow1-1.0.0/TensorFlow1.egg-info/
--rw-rw-rw-   0        0        0      186 2023-07-25 14:41:22.000000 TensorFlow1-1.0.0/TensorFlow1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-07-25 14:41:22.000000 TensorFlow1-1.0.0/TensorFlow1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 14:41:22.000000 TensorFlow1-1.0.0/TensorFlow1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-25 14:41:22.000000 TensorFlow1-1.0.0/TensorFlow1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-07-25 12:13:11.000000 TensorFlow1-1.0.0/license.txt
--rw-rw-rw-   0        0        0      158 2023-07-25 14:41:22.599786 TensorFlow1-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      297 2023-07-25 14:39:46.000000 TensorFlow1-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:54:24.943781 TensorFlow1-1.1.0/
+-rw-rw-rw-   0        0        0      193 2023-07-25 14:54:24.943781 TensorFlow1-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-25 12:12:58.000000 TensorFlow1-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 14:54:24.923442 TensorFlow1-1.1.0/TensorFlow1/
+-rw-rw-rw-   0        0        0    17833 2023-07-25 14:37:39.000000 TensorFlow1-1.1.0/TensorFlow1/TensorFlow.py
+-rw-rw-rw-   0        0        0       40 2023-07-25 14:53:10.000000 TensorFlow1-1.1.0/TensorFlow1/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:54:24.942777 TensorFlow1-1.1.0/TensorFlow1.egg-info/
+-rw-rw-rw-   0        0        0      193 2023-07-25 14:54:24.000000 TensorFlow1-1.1.0/TensorFlow1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-07-25 14:54:24.000000 TensorFlow1-1.1.0/TensorFlow1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 14:54:24.000000 TensorFlow1-1.1.0/TensorFlow1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-25 14:54:24.000000 TensorFlow1-1.1.0/TensorFlow1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-07-25 12:13:11.000000 TensorFlow1-1.1.0/license.txt
+-rw-rw-rw-   0        0        0      158 2023-07-25 14:54:24.952251 TensorFlow1-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      304 2023-07-25 14:53:56.000000 TensorFlow1-1.1.0/setup.py
```

### Comparing `TensorFlow1-1.0.0/TensorFlow1/TensorFlow.py` & `TensorFlow1-1.1.0/TensorFlow1/TensorFlow.py`

 * *Files identical despite different names*

