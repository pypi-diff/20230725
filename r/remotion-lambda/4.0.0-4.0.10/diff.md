# Comparing `tmp/remotion_lambda-4.0.0.tar.gz` & `tmp/remotion_lambda-4.0.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotion_lambda-4.0.0.tar", last modified: Tue Jul 25 00:57:47 2023, max compression
+gzip compressed data, was "remotion_lambda-4.0.10.tar", last modified: Tue Jul 25 00:58:21 2023, max compression
```

## Comparing `remotion_lambda-4.0.0.tar` & `remotion_lambda-4.0.10.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 codedev    (503) staff       (20)        0 2023-07-25 00:57:47.760849 remotion_lambda-4.0.0/
--rw-r--r--   0 codedev    (503) staff       (20)     2512 2023-07-21 08:40:48.000000 remotion_lambda-4.0.0/LICENSE
--rw-r--r--   0 codedev    (503) staff       (20)      315 2023-07-25 00:57:47.760697 remotion_lambda-4.0.0/PKG-INFO
--rw-r--r--   0 codedev    (503) staff       (20)       26 2023-07-21 08:40:48.000000 remotion_lambda-4.0.0/README.md
-drwxr-xr-x   0 codedev    (503) staff       (20)        0 2023-07-25 00:57:47.758638 remotion_lambda-4.0.0/remotion_lambda/
--rw-r--r--   0 codedev    (503) staff       (20)      202 2023-07-21 08:40:48.000000 remotion_lambda-4.0.0/remotion_lambda/__init__.py
--rw-r--r--   0 codedev    (503) staff       (20)     5252 2023-07-21 08:40:48.000000 remotion_lambda-4.0.0/remotion_lambda/models.py
--rw-r--r--   0 codedev    (503) staff       (20)     6182 2023-07-23 00:48:40.000000 remotion_lambda-4.0.0/remotion_lambda/remotionclient.py
--rw-r--r--   0 codedev    (503) staff       (20)       84 2023-07-23 00:21:34.000000 remotion_lambda-4.0.0/remotion_lambda/version.py
-drwxr-xr-x   0 codedev    (503) staff       (20)        0 2023-07-25 00:57:47.759537 remotion_lambda-4.0.0/remotion_lambda.egg-info/
--rw-r--r--   0 codedev    (503) staff       (20)      315 2023-07-25 00:57:47.000000 remotion_lambda-4.0.0/remotion_lambda.egg-info/PKG-INFO
--rw-r--r--   0 codedev    (503) staff       (20)      384 2023-07-25 00:57:47.000000 remotion_lambda-4.0.0/remotion_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 codedev    (503) staff       (20)        1 2023-07-25 00:57:47.000000 remotion_lambda-4.0.0/remotion_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 codedev    (503) staff       (20)       42 2023-07-25 00:57:47.000000 remotion_lambda-4.0.0/remotion_lambda.egg-info/top_level.txt
--rw-r--r--   0 codedev    (503) staff       (20)       38 2023-07-25 00:57:47.760891 remotion_lambda-4.0.0/setup.cfg
--rw-r--r--   0 codedev    (503) staff       (20)      684 2023-07-21 08:40:48.000000 remotion_lambda-4.0.0/setup.py
-drwxr-xr-x   0 codedev    (503) staff       (20)        0 2023-07-25 00:57:47.760293 remotion_lambda-4.0.0/tests/
--rw-r--r--   0 codedev    (503) staff       (20)      131 2023-07-21 08:40:48.000000 remotion_lambda-4.0.0/tests/__init__.py
--rw-r--r--   0 codedev    (503) staff       (20)      474 2023-07-21 22:55:58.000000 remotion_lambda-4.0.0/tests/test_get_render_progress_client.py
--rw-r--r--   0 codedev    (503) staff       (20)      764 2023-07-21 22:55:55.000000 remotion_lambda-4.0.0/tests/test_render_client.py
+drwxr-xr-x   0 codedev    (503) staff       (20)        0 2023-07-25 00:58:21.787713 remotion_lambda-4.0.10/
+-rw-r--r--   0 codedev    (503) staff       (20)     2512 2023-07-21 08:40:48.000000 remotion_lambda-4.0.10/LICENSE
+-rw-r--r--   0 codedev    (503) staff       (20)      316 2023-07-25 00:58:21.787545 remotion_lambda-4.0.10/PKG-INFO
+-rw-r--r--   0 codedev    (503) staff       (20)       26 2023-07-21 08:40:48.000000 remotion_lambda-4.0.10/README.md
+drwxr-xr-x   0 codedev    (503) staff       (20)        0 2023-07-25 00:58:21.786093 remotion_lambda-4.0.10/remotion_lambda/
+-rw-r--r--   0 codedev    (503) staff       (20)      202 2023-07-21 08:40:48.000000 remotion_lambda-4.0.10/remotion_lambda/__init__.py
+-rw-r--r--   0 codedev    (503) staff       (20)     5252 2023-07-21 08:40:48.000000 remotion_lambda-4.0.10/remotion_lambda/models.py
+-rw-r--r--   0 codedev    (503) staff       (20)     6182 2023-07-23 00:48:40.000000 remotion_lambda-4.0.10/remotion_lambda/remotionclient.py
+-rw-r--r--   0 codedev    (503) staff       (20)       85 2023-07-25 00:58:16.000000 remotion_lambda-4.0.10/remotion_lambda/version.py
+drwxr-xr-x   0 codedev    (503) staff       (20)        0 2023-07-25 00:58:21.786610 remotion_lambda-4.0.10/remotion_lambda.egg-info/
+-rw-r--r--   0 codedev    (503) staff       (20)      316 2023-07-25 00:58:21.000000 remotion_lambda-4.0.10/remotion_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 codedev    (503) staff       (20)      384 2023-07-25 00:58:21.000000 remotion_lambda-4.0.10/remotion_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 codedev    (503) staff       (20)        1 2023-07-25 00:58:21.000000 remotion_lambda-4.0.10/remotion_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 codedev    (503) staff       (20)       42 2023-07-25 00:58:21.000000 remotion_lambda-4.0.10/remotion_lambda.egg-info/top_level.txt
+-rw-r--r--   0 codedev    (503) staff       (20)       38 2023-07-25 00:58:21.787756 remotion_lambda-4.0.10/setup.cfg
+-rw-r--r--   0 codedev    (503) staff       (20)      684 2023-07-21 08:40:48.000000 remotion_lambda-4.0.10/setup.py
+drwxr-xr-x   0 codedev    (503) staff       (20)        0 2023-07-25 00:58:21.787180 remotion_lambda-4.0.10/tests/
+-rw-r--r--   0 codedev    (503) staff       (20)      131 2023-07-21 08:40:48.000000 remotion_lambda-4.0.10/tests/__init__.py
+-rw-r--r--   0 codedev    (503) staff       (20)      474 2023-07-21 22:55:58.000000 remotion_lambda-4.0.10/tests/test_get_render_progress_client.py
+-rw-r--r--   0 codedev    (503) staff       (20)      764 2023-07-21 22:55:55.000000 remotion_lambda-4.0.10/tests/test_render_client.py
```

### Comparing `remotion_lambda-4.0.0/LICENSE` & `remotion_lambda-4.0.10/LICENSE`

 * *Files identical despite different names*

### Comparing `remotion_lambda-4.0.0/remotion_lambda/models.py` & `remotion_lambda-4.0.10/remotion_lambda/models.py`

 * *Files identical despite different names*

### Comparing `remotion_lambda-4.0.0/remotion_lambda/remotionclient.py` & `remotion_lambda-4.0.10/remotion_lambda/remotionclient.py`

 * *Files identical despite different names*

### Comparing `remotion_lambda-4.0.0/setup.py` & `remotion_lambda-4.0.10/setup.py`

 * *Files identical despite different names*

### Comparing `remotion_lambda-4.0.0/tests/test_render_client.py` & `remotion_lambda-4.0.10/tests/test_render_client.py`

 * *Files identical despite different names*

