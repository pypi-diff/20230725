# Comparing `tmp/status_ok-0.0.2.tar.gz` & `tmp/status_ok-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "status_ok-0.0.2.tar", last modified: Tue Jul 25 09:22:52 2023, max compression
+gzip compressed data, was "status_ok-0.0.3.tar", last modified: Tue Jul 25 11:06:47 2023, max compression
```

## Comparing `status_ok-0.0.2.tar` & `status_ok-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 YuvrajSynapses   (502) staff       (20)        0 2023-07-25 09:22:52.068388 status_ok-0.0.2/
--rw-r--r--   0 YuvrajSynapses   (502) staff       (20)      490 2023-07-25 09:22:52.068226 status_ok-0.0.2/PKG-INFO
--rw-r--r--   0 YuvrajSynapses   (502) staff       (20)       38 2023-07-25 09:22:52.068444 status_ok-0.0.2/setup.cfg
--rw-r--r--   0 YuvrajSynapses   (502) staff       (20)      728 2023-07-25 09:22:48.000000 status_ok-0.0.2/setup.py
-drwxr-xr-x   0 YuvrajSynapses   (502) staff       (20)        0 2023-07-25 09:22:52.067361 status_ok-0.0.2/status_ok/
--rw-r--r--   0 YuvrajSynapses   (502) staff       (20)        0 2023-07-20 08:56:59.000000 status_ok-0.0.2/status_ok/__init__.py
--rw-r--r--   0 YuvrajSynapses   (502) staff       (20)     2796 2023-07-25 07:20:48.000000 status_ok-0.0.2/status_ok/handle_error.py
-drwxr-xr-x   0 YuvrajSynapses   (502) staff       (20)        0 2023-07-25 09:22:52.068055 status_ok-0.0.2/status_ok.egg-info/
--rw-r--r--   0 YuvrajSynapses   (502) staff       (20)      490 2023-07-25 09:22:52.000000 status_ok-0.0.2/status_ok.egg-info/PKG-INFO
--rw-r--r--   0 YuvrajSynapses   (502) staff       (20)      220 2023-07-25 09:22:52.000000 status_ok-0.0.2/status_ok.egg-info/SOURCES.txt
--rw-r--r--   0 YuvrajSynapses   (502) staff       (20)        1 2023-07-25 09:22:52.000000 status_ok-0.0.2/status_ok.egg-info/dependency_links.txt
--rw-r--r--   0 YuvrajSynapses   (502) staff       (20)        9 2023-07-25 09:22:52.000000 status_ok-0.0.2/status_ok.egg-info/requires.txt
--rw-r--r--   0 YuvrajSynapses   (502) staff       (20)       10 2023-07-25 09:22:52.000000 status_ok-0.0.2/status_ok.egg-info/top_level.txt
+drwxr-xr-x   0 YuvrajSynapses   (502) staff       (20)        0 2023-07-25 11:06:47.173451 status_ok-0.0.3/
+-rw-r--r--   0 YuvrajSynapses   (502) staff       (20)      490 2023-07-25 11:06:47.173338 status_ok-0.0.3/PKG-INFO
+-rw-r--r--   0 YuvrajSynapses   (502) staff       (20)       38 2023-07-25 11:06:47.173490 status_ok-0.0.3/setup.cfg
+-rw-r--r--   0 YuvrajSynapses   (502) staff       (20)      728 2023-07-25 11:06:16.000000 status_ok-0.0.3/setup.py
+drwxr-xr-x   0 YuvrajSynapses   (502) staff       (20)        0 2023-07-25 11:06:47.172457 status_ok-0.0.3/status_ok/
+-rw-r--r--   0 YuvrajSynapses   (502) staff       (20)        0 2023-07-20 08:56:59.000000 status_ok-0.0.3/status_ok/__init__.py
+-rw-r--r--   0 YuvrajSynapses   (502) staff       (20)      837 2023-07-25 11:03:43.000000 status_ok-0.0.3/status_ok/handle_error.py
+-rw-r--r--   0 YuvrajSynapses   (502) staff       (20)      420 2023-07-25 11:05:50.000000 status_ok-0.0.3/status_ok/status.py
+-rw-r--r--   0 YuvrajSynapses   (502) staff       (20)     2006 2023-07-25 11:00:07.000000 status_ok-0.0.3/status_ok/status_codex.py
+drwxr-xr-x   0 YuvrajSynapses   (502) staff       (20)        0 2023-07-25 11:06:47.173160 status_ok-0.0.3/status_ok.egg-info/
+-rw-r--r--   0 YuvrajSynapses   (502) staff       (20)      490 2023-07-25 11:06:47.000000 status_ok-0.0.3/status_ok.egg-info/PKG-INFO
+-rw-r--r--   0 YuvrajSynapses   (502) staff       (20)      266 2023-07-25 11:06:47.000000 status_ok-0.0.3/status_ok.egg-info/SOURCES.txt
+-rw-r--r--   0 YuvrajSynapses   (502) staff       (20)        1 2023-07-25 11:06:47.000000 status_ok-0.0.3/status_ok.egg-info/dependency_links.txt
+-rw-r--r--   0 YuvrajSynapses   (502) staff       (20)        9 2023-07-25 11:06:47.000000 status_ok-0.0.3/status_ok.egg-info/requires.txt
+-rw-r--r--   0 YuvrajSynapses   (502) staff       (20)       10 2023-07-25 11:06:47.000000 status_ok-0.0.3/status_ok.egg-info/top_level.txt
```

### Comparing `status_ok-0.0.2/setup.py` & `status_ok-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 LICENSE = 'MIT'
 REQUIRES = [
     'requests',
 ]
 
 setup(
     name="status_ok",
-    version="0.0.2",
+    version="0.0.3",
     description="This library is used to handle http responses.",
     long_description="This library is used to handle http responses in python.",
     long_description_content_type='text/markdown',
     author="yuvraj jaiswal",
     author_email="y.jaiswal@thesynapses.com",
     url="https://github.com/iLS-yuvrajj/statusOk/tree/main",
     license=LICENSE,
```

