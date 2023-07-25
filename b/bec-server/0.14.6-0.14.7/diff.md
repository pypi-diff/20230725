# Comparing `tmp/bec-server-0.14.6.tar.gz` & `tmp/bec-server-0.14.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec-server-0.14.6.tar", last modified: Tue Jul 25 08:55:07 2023, max compression
+gzip compressed data, was "bec-server-0.14.7.tar", last modified: Tue Jul 25 12:06:43 2023, max compression
```

## Comparing `bec-server-0.14.6.tar` & `bec-server-0.14.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:55:07.353039 bec-server-0.14.6/
--rw-r--r--   0 root         (0) root         (0)      443 2023-07-25 08:55:07.354039 bec-server-0.14.6/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:55:07.352039 bec-server-0.14.6/bec_server/
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-08 15:33:35.000000 bec-server-0.14.6/bec_server/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1391 2023-07-21 18:30:48.000000 bec-server-0.14.6/bec_server/launch.py
--rw-r--r--   0 root         (0) root         (0)     3075 2023-07-08 15:33:35.000000 bec-server-0.14.6/bec_server/service_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     2716 2023-07-21 18:30:48.000000 bec-server-0.14.6/bec_server/tmux_launch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:55:07.353039 bec-server-0.14.6/bec_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)      443 2023-07-25 08:55:07.000000 bec-server-0.14.6/bec_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      332 2023-07-25 08:55:07.000000 bec-server-0.14.6/bec_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 08:55:07.000000 bec-server-0.14.6/bec_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-07-25 08:55:07.000000 bec-server-0.14.6/bec_server.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-07-25 08:55:07.000000 bec-server-0.14.6/bec_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-25 08:55:07.000000 bec-server-0.14.6/bec_server.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      503 2023-07-25 08:55:07.354039 bec-server-0.14.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2073 2023-07-25 08:54:39.000000 bec-server-0.14.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:06:43.599296 bec-server-0.14.7/
+-rw-r--r--   0 root         (0) root         (0)      443 2023-07-25 12:06:43.599296 bec-server-0.14.7/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:06:43.598296 bec-server-0.14.7/bec_server/
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-08 15:33:35.000000 bec-server-0.14.7/bec_server/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1391 2023-07-21 18:30:48.000000 bec-server-0.14.7/bec_server/launch.py
+-rw-r--r--   0 root         (0) root         (0)     3075 2023-07-08 15:33:35.000000 bec-server-0.14.7/bec_server/service_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     2716 2023-07-21 18:30:48.000000 bec-server-0.14.7/bec_server/tmux_launch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:06:43.599296 bec-server-0.14.7/bec_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      443 2023-07-25 12:06:43.000000 bec-server-0.14.7/bec_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      332 2023-07-25 12:06:43.000000 bec-server-0.14.7/bec_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 12:06:43.000000 bec-server-0.14.7/bec_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-07-25 12:06:43.000000 bec-server-0.14.7/bec_server.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      192 2023-07-25 12:06:43.000000 bec-server-0.14.7/bec_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-25 12:06:43.000000 bec-server-0.14.7/bec_server.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      503 2023-07-25 12:06:43.599296 bec-server-0.14.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2167 2023-07-25 12:06:37.000000 bec-server-0.14.7/setup.py
```

### Comparing `bec-server-0.14.6/bec_server/launch.py` & `bec-server-0.14.7/bec_server/launch.py`

 * *Files identical despite different names*

### Comparing `bec-server-0.14.6/bec_server/service_handler.py` & `bec-server-0.14.7/bec_server/service_handler.py`

 * *Files identical despite different names*

### Comparing `bec-server-0.14.6/bec_server/tmux_launch.py` & `bec-server-0.14.7/bec_server/tmux_launch.py`

 * *Files identical despite different names*

### Comparing `bec-server-0.14.6/setup.py` & `bec-server-0.14.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os
 import pathlib
 import subprocess
+import sys
 
 from setuptools import setup
 
 current_path = pathlib.Path(__file__).parent.resolve()
 
-__version__ = "0.14.6"
+__version__ = "0.14.7"
 
 
 def run_install(setup_args: dict, bec_deps: list, editable=False):
     """
     Run the setup function with the given arguments.
 
     Args:
@@ -60,9 +61,12 @@
                 "coverage",
                 "black",
                 "pylint",
             ]
         },
     }
 
-    editable = os.path.dirname(os.path.abspath(__file__)).split("/")[-1] == "bec_server"
+    is_local = os.path.dirname(os.path.abspath(__file__)).split("/")[-1] == "bec_server"
+    is_build = "bdist_wheel" in sys.argv
+
+    editable = is_local and not is_build
     run_install(setup_args, bec_deps, editable=editable)
```

