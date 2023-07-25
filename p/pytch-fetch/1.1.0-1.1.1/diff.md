# Comparing `tmp/pytch-fetch-1.1.0.tar.gz` & `tmp/pytch-fetch-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytch-fetch-1.1.0.tar", last modified: Tue Jul 25 16:15:23 2023, max compression
+gzip compressed data, was "pytch-fetch-1.1.1.tar", last modified: Tue Jul 25 16:37:38 2023, max compression
```

## Comparing `pytch-fetch-1.1.0.tar` & `pytch-fetch-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-25 16:15:23.363761 pytch-fetch-1.1.0/
--rw-r--r--   0 krit      (1000) krit      (1001)     1066 2023-07-24 09:11:38.000000 pytch-fetch-1.1.0/LICENSE
--rw-r--r--   0 krit      (1000) krit      (1001)     4220 2023-07-25 16:15:23.363761 pytch-fetch-1.1.0/PKG-INFO
--rw-r--r--   0 krit      (1000) krit      (1001)     1779 2023-07-25 16:13:59.000000 pytch-fetch-1.1.0/README.md
--rw-r--r--   0 krit      (1000) krit      (1001)     1298 2023-07-25 16:13:59.000000 pytch-fetch-1.1.0/pyproject.toml
--rw-r--r--   0 krit      (1000) krit      (1001)       38 2023-07-25 16:15:23.363761 pytch-fetch-1.1.0/setup.cfg
-drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-25 16:15:23.361761 pytch-fetch-1.1.0/src/
-drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-25 16:15:23.363761 pytch-fetch-1.1.0/src/pytch/
--rw-r--r--   0 krit      (1000) krit      (1001)        0 2023-07-24 09:11:38.000000 pytch-fetch-1.1.0/src/pytch/__init__.py
--rwxr-xr-x   0 krit      (1000) krit      (1001)     3505 2023-07-25 16:13:59.000000 pytch-fetch-1.1.0/src/pytch/__main__.py
--rw-r--r--   0 krit      (1000) krit      (1001)    21003 2023-07-25 16:13:59.000000 pytch-fetch-1.1.0/src/pytch/art.py
--rw-r--r--   0 krit      (1000) krit      (1001)     6373 2023-07-25 16:13:59.000000 pytch-fetch-1.1.0/src/pytch/funcs.py
-drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-25 16:15:23.363761 pytch-fetch-1.1.0/src/pytch_fetch.egg-info/
--rw-r--r--   0 krit      (1000) krit      (1001)     4220 2023-07-25 16:15:23.000000 pytch-fetch-1.1.0/src/pytch_fetch.egg-info/PKG-INFO
--rw-r--r--   0 krit      (1000) krit      (1001)      310 2023-07-25 16:15:23.000000 pytch-fetch-1.1.0/src/pytch_fetch.egg-info/SOURCES.txt
--rw-r--r--   0 krit      (1000) krit      (1001)        1 2023-07-25 16:15:23.000000 pytch-fetch-1.1.0/src/pytch_fetch.egg-info/dependency_links.txt
--rw-r--r--   0 krit      (1000) krit      (1001)       46 2023-07-25 16:15:23.000000 pytch-fetch-1.1.0/src/pytch_fetch.egg-info/entry_points.txt
--rw-r--r--   0 krit      (1000) krit      (1001)        6 2023-07-25 16:15:23.000000 pytch-fetch-1.1.0/src/pytch_fetch.egg-info/top_level.txt
+drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-25 16:37:38.639725 pytch-fetch-1.1.1/
+-rw-r--r--   0 krit      (1000) krit      (1001)     1066 2023-07-24 09:11:38.000000 pytch-fetch-1.1.1/LICENSE
+-rw-r--r--   0 krit      (1000) krit      (1001)     4258 2023-07-25 16:37:38.638725 pytch-fetch-1.1.1/PKG-INFO
+-rw-r--r--   0 krit      (1000) krit      (1001)     1779 2023-07-25 16:13:59.000000 pytch-fetch-1.1.1/README.md
+-rw-r--r--   0 krit      (1000) krit      (1001)     1329 2023-07-25 16:37:25.000000 pytch-fetch-1.1.1/pyproject.toml
+-rw-r--r--   0 krit      (1000) krit      (1001)       38 2023-07-25 16:37:38.639725 pytch-fetch-1.1.1/setup.cfg
+drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-25 16:37:38.637725 pytch-fetch-1.1.1/src/
+drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-25 16:37:38.638725 pytch-fetch-1.1.1/src/pytch/
+-rw-r--r--   0 krit      (1000) krit      (1001)        0 2023-07-24 09:11:38.000000 pytch-fetch-1.1.1/src/pytch/__init__.py
+-rwxr-xr-x   0 krit      (1000) krit      (1001)     3505 2023-07-25 16:36:56.000000 pytch-fetch-1.1.1/src/pytch/__main__.py
+-rw-r--r--   0 krit      (1000) krit      (1001)    21003 2023-07-25 16:13:59.000000 pytch-fetch-1.1.1/src/pytch/art.py
+-rw-r--r--   0 krit      (1000) krit      (1001)     6373 2023-07-25 16:13:59.000000 pytch-fetch-1.1.1/src/pytch/funcs.py
+drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-25 16:37:38.638725 pytch-fetch-1.1.1/src/pytch_fetch.egg-info/
+-rw-r--r--   0 krit      (1000) krit      (1001)     4258 2023-07-25 16:37:38.000000 pytch-fetch-1.1.1/src/pytch_fetch.egg-info/PKG-INFO
+-rw-r--r--   0 krit      (1000) krit      (1001)      310 2023-07-25 16:37:38.000000 pytch-fetch-1.1.1/src/pytch_fetch.egg-info/SOURCES.txt
+-rw-r--r--   0 krit      (1000) krit      (1001)        1 2023-07-25 16:37:38.000000 pytch-fetch-1.1.1/src/pytch_fetch.egg-info/dependency_links.txt
+-rw-r--r--   0 krit      (1000) krit      (1001)       46 2023-07-25 16:37:38.000000 pytch-fetch-1.1.1/src/pytch_fetch.egg-info/entry_points.txt
+-rw-r--r--   0 krit      (1000) krit      (1001)        6 2023-07-25 16:37:38.000000 pytch-fetch-1.1.1/src/pytch_fetch.egg-info/top_level.txt
```

### Comparing `pytch-fetch-1.1.0/LICENSE` & `pytch-fetch-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytch-fetch-1.1.0/PKG-INFO` & `pytch-fetch-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytch-fetch
-Version: 1.1.0
+Version: 1.1.1
 Summary: Pytch Yields Technical Characteristics Hastily
 Author-email: Krit Dass <dasskrit@gmail.com>
 Maintainer-email: Krit Dass <dasskrit@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Krit Dass
         
@@ -29,14 +29,15 @@
 Project-URL: Homepage, https://github.com/kritdass/pytch
 Project-URL: Repository, https://github.com/kritdass/pytch
 Keywords: linux,fetch,terminal
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `pytch-fetch-1.1.0/README.md` & `pytch-fetch-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pytch-fetch-1.1.0/pyproject.toml` & `pytch-fetch-1.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [build-system]
 requires = ["setuptools >= 61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytch-fetch"
-version = "1.1.0"
+version = "1.1.1"
 description="Pytch Yields Technical Characteristics Hastily"
 readme = "README.md"
 authors = [{ name = "Krit Dass", email = "dasskrit@gmail.com" }]
 maintainers = [{ name = "Krit Dass", email = "dasskrit@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
   "Development Status :: 1 - Planning",
   "License :: OSI Approved :: MIT License",
   "Natural Language :: English",
   "Operating System :: POSIX :: Linux",
+  "Operating System :: MacOS",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
```

### Comparing `pytch-fetch-1.1.0/src/pytch/__main__.py` & `pytch-fetch-1.1.1/src/pytch/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         "-l",
         "--logo",
         metavar="DISTRO",
         dest="logo",
         help="use an alternate distribution's logo",
     )
 
-    parser.add_argument("-v", "--version", action="version", version="1.1.0")
+    parser.add_argument("-v", "--version", action="version", version="1.1.1")
 
     args = parser.parse_args()
 
     attrs = [
         {"name": "user", "value": getlogin(), "icon": "", "color": "red"},
         {
             "name": "os",
```

### Comparing `pytch-fetch-1.1.0/src/pytch/art.py` & `pytch-fetch-1.1.1/src/pytch/art.py`

 * *Files identical despite different names*

### Comparing `pytch-fetch-1.1.0/src/pytch/funcs.py` & `pytch-fetch-1.1.1/src/pytch/funcs.py`

 * *Files identical despite different names*

### Comparing `pytch-fetch-1.1.0/src/pytch_fetch.egg-info/PKG-INFO` & `pytch-fetch-1.1.1/src/pytch_fetch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytch-fetch
-Version: 1.1.0
+Version: 1.1.1
 Summary: Pytch Yields Technical Characteristics Hastily
 Author-email: Krit Dass <dasskrit@gmail.com>
 Maintainer-email: Krit Dass <dasskrit@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Krit Dass
         
@@ -29,14 +29,15 @@
 Project-URL: Homepage, https://github.com/kritdass/pytch
 Project-URL: Repository, https://github.com/kritdass/pytch
 Keywords: linux,fetch,terminal
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

