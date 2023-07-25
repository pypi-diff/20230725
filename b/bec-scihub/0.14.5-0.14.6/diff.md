# Comparing `tmp/bec_scihub-0.14.5.tar.gz` & `tmp/bec_scihub-0.14.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_scihub-0.14.5.tar", last modified: Mon Jul 24 17:00:34 2023, max compression
+gzip compressed data, was "bec_scihub-0.14.6.tar", last modified: Tue Jul 25 08:55:04 2023, max compression
```

## Comparing `bec_scihub-0.14.5.tar` & `bec_scihub-0.14.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 17:00:34.949677 bec_scihub-0.14.5/
--rw-r--r--   0 root         (0) root         (0)      478 2023-07-24 17:00:34.949677 bec_scihub-0.14.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 17:00:34.948677 bec_scihub-0.14.5/bec_scihub.egg-info/
--rw-r--r--   0 root         (0) root         (0)      478 2023-07-24 17:00:34.000000 bec_scihub-0.14.5/bec_scihub.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      569 2023-07-24 17:00:34.000000 bec_scihub-0.14.5/bec_scihub.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 17:00:34.000000 bec_scihub-0.14.5/bec_scihub.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-24 17:00:34.000000 bec_scihub-0.14.5/bec_scihub.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-07-24 17:00:34.000000 bec_scihub-0.14.5/bec_scihub.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-24 17:00:34.000000 bec_scihub-0.14.5/bec_scihub.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 17:00:34.945677 bec_scihub-0.14.5/scihub/
--rw-r--r--   0 root         (0) root         (0)       56 2023-07-08 15:33:35.000000 bec_scihub-0.14.5/scihub/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 17:00:34.945677 bec_scihub-0.14.5/scihub/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 15:01:50.000000 bec_scihub-0.14.5/scihub/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      782 2023-07-08 15:33:35.000000 bec_scihub-0.14.5/scihub/cli/launch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 17:00:34.947677 bec_scihub-0.14.5/scihub/scibec/
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-06-19 08:14:59.000000 bec_scihub-0.14.5/scihub/scibec/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7654 2023-06-28 10:41:58.000000 bec_scihub-0.14.5/scihub/scibec/config_handler.py
--rw-r--r--   0 root         (0) root         (0)    15033 2023-06-28 10:41:58.000000 bec_scihub-0.14.5/scihub/scibec/scibec.py
--rw-r--r--   0 root         (0) root         (0)     4428 2023-06-28 10:41:58.000000 bec_scihub-0.14.5/scihub/scibec/scibec_connector.py
--rw-r--r--   0 root         (0) root         (0)     4126 2023-06-28 10:41:58.000000 bec_scihub-0.14.5/scihub/scibec/scibec_metadata_handler.py
--rw-rw-rw-   0 root         (0) root         (0)      880 2023-06-19 08:14:59.000000 bec_scihub-0.14.5/scihub/scibec/scibec_validator.py
--rw-r--r--   0 root         (0) root         (0)      902 2023-06-28 10:41:58.000000 bec_scihub-0.14.5/scihub/scihub.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 17:00:34.947677 bec_scihub-0.14.5/scihub/scilog/
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-19 08:14:59.000000 bec_scihub-0.14.5/scihub/scilog/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3330 2023-06-28 10:41:58.000000 bec_scihub-0.14.5/scihub/scilog/scilog.py
--rw-r--r--   0 root         (0) root         (0)      538 2023-07-24 17:00:34.949677 bec_scihub-0.14.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-24 17:00:09.000000 bec_scihub-0.14.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:55:04.760120 bec_scihub-0.14.6/
+-rw-r--r--   0 root         (0) root         (0)      478 2023-07-25 08:55:04.760120 bec_scihub-0.14.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:55:04.760120 bec_scihub-0.14.6/bec_scihub.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      478 2023-07-25 08:55:04.000000 bec_scihub-0.14.6/bec_scihub.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      569 2023-07-25 08:55:04.000000 bec_scihub-0.14.6/bec_scihub.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 08:55:04.000000 bec_scihub-0.14.6/bec_scihub.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-25 08:55:04.000000 bec_scihub-0.14.6/bec_scihub.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-07-25 08:55:04.000000 bec_scihub-0.14.6/bec_scihub.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-25 08:55:04.000000 bec_scihub-0.14.6/bec_scihub.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:55:04.757120 bec_scihub-0.14.6/scihub/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-08 15:33:35.000000 bec_scihub-0.14.6/scihub/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:55:04.758120 bec_scihub-0.14.6/scihub/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 15:01:50.000000 bec_scihub-0.14.6/scihub/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      782 2023-07-08 15:33:35.000000 bec_scihub-0.14.6/scihub/cli/launch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:55:04.759120 bec_scihub-0.14.6/scihub/scibec/
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-06-19 08:14:59.000000 bec_scihub-0.14.6/scihub/scibec/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7654 2023-06-28 10:41:58.000000 bec_scihub-0.14.6/scihub/scibec/config_handler.py
+-rw-r--r--   0 root         (0) root         (0)    15033 2023-06-28 10:41:58.000000 bec_scihub-0.14.6/scihub/scibec/scibec.py
+-rw-r--r--   0 root         (0) root         (0)     4428 2023-06-28 10:41:58.000000 bec_scihub-0.14.6/scihub/scibec/scibec_connector.py
+-rw-r--r--   0 root         (0) root         (0)     4126 2023-06-28 10:41:58.000000 bec_scihub-0.14.6/scihub/scibec/scibec_metadata_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)      880 2023-06-19 08:14:59.000000 bec_scihub-0.14.6/scihub/scibec/scibec_validator.py
+-rw-r--r--   0 root         (0) root         (0)      902 2023-06-28 10:41:58.000000 bec_scihub-0.14.6/scihub/scihub.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:55:04.759120 bec_scihub-0.14.6/scihub/scilog/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-19 08:14:59.000000 bec_scihub-0.14.6/scihub/scilog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3330 2023-06-28 10:41:58.000000 bec_scihub-0.14.6/scihub/scilog/scilog.py
+-rw-r--r--   0 root         (0) root         (0)      538 2023-07-25 08:55:04.761120 bec_scihub-0.14.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1664 2023-07-25 08:54:39.000000 bec_scihub-0.14.6/setup.py
```

### Comparing `bec_scihub-0.14.5/bec_scihub.egg-info/SOURCES.txt` & `bec_scihub-0.14.6/bec_scihub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.14.5/scihub/cli/launch.py` & `bec_scihub-0.14.6/scihub/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.14.5/scihub/scibec/config_handler.py` & `bec_scihub-0.14.6/scihub/scibec/config_handler.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.14.5/scihub/scibec/scibec.py` & `bec_scihub-0.14.6/scihub/scibec/scibec.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.14.5/scihub/scibec/scibec_connector.py` & `bec_scihub-0.14.6/scihub/scibec/scibec_connector.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.14.5/scihub/scibec/scibec_metadata_handler.py` & `bec_scihub-0.14.6/scihub/scibec/scibec_metadata_handler.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.14.5/scihub/scibec/scibec_validator.py` & `bec_scihub-0.14.6/scihub/scibec/scibec_validator.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.14.5/scihub/scihub.py` & `bec_scihub-0.14.6/scihub/scihub.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.14.5/scihub/scilog/scilog.py` & `bec_scihub-0.14.6/scihub/scilog/scilog.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.14.5/setup.cfg` & `bec_scihub-0.14.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `bec_scihub-0.14.5/setup.py` & `bec_scihub-0.14.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup
 
 current_path = pathlib.Path(__file__).parent.resolve()
 
 bec_lib = f"{current_path}/../bec_lib/"
 
 
-__version__ = "0.14.5"
+__version__ = "0.14.6"
 
 
 def run_install(setup_args: dict, bec_deps: list, editable=False):
     """
     Run the setup function with the given arguments.
 
     Args:
```

