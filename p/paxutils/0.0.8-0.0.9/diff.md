# Comparing `tmp/paxutils-0.0.8.tar.gz` & `tmp/paxutils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paxutils-0.0.8.tar", last modified: Tue Apr 19 19:19:22 2022, max compression
+gzip compressed data, was "paxutils-0.0.9.tar", last modified: Tue Apr 19 19:23:48 2022, max compression
```

## Comparing `paxutils-0.0.8.tar` & `paxutils-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 parizeau   (502) staff       (20)        0 2022-04-19 19:19:22.998019 paxutils-0.0.8/
--rw-r--r--   0 parizeau   (502) staff       (20)     1071 2022-04-08 13:37:32.000000 paxutils-0.0.8/LICENSE
--rw-r--r--   0 parizeau   (502) staff       (20)      595 2022-04-19 19:19:22.998089 paxutils-0.0.8/PKG-INFO
--rw-r--r--   0 parizeau   (502) staff       (20)       55 2022-04-08 13:37:32.000000 paxutils-0.0.8/README.md
--rw-r--r--   0 parizeau   (502) staff       (20)       85 2022-04-08 14:01:49.000000 paxutils-0.0.8/pyproject.toml
--rw-r--r--   0 parizeau   (502) staff       (20)      649 2022-04-19 19:19:22.998369 paxutils-0.0.8/setup.cfg
-drwxr-xr-x   0 parizeau   (502) staff       (20)        0 2022-04-19 19:19:22.996338 paxutils-0.0.8/src/
-drwxr-xr-x   0 parizeau   (502) staff       (20)        0 2022-04-19 19:19:22.997363 paxutils-0.0.8/src/paxutils/
--rw-r--r--   0 parizeau   (502) staff       (20)       22 2022-04-19 19:17:57.000000 paxutils-0.0.8/src/paxutils/__init__.py
--rw-r--r--   0 parizeau   (502) staff       (20)     2893 2022-04-19 19:00:56.000000 paxutils-0.0.8/src/paxutils/path.py
-drwxr-xr-x   0 parizeau   (502) staff       (20)        0 2022-04-19 19:19:22.997904 paxutils-0.0.8/src/paxutils.egg-info/
--rw-r--r--   0 parizeau   (502) staff       (20)      595 2022-04-19 19:19:22.000000 paxutils-0.0.8/src/paxutils.egg-info/PKG-INFO
--rw-r--r--   0 parizeau   (502) staff       (20)      232 2022-04-19 19:19:22.000000 paxutils-0.0.8/src/paxutils.egg-info/SOURCES.txt
--rw-r--r--   0 parizeau   (502) staff       (20)        1 2022-04-19 19:19:22.000000 paxutils-0.0.8/src/paxutils.egg-info/dependency_links.txt
--rw-r--r--   0 parizeau   (502) staff       (20)        9 2022-04-19 19:19:22.000000 paxutils-0.0.8/src/paxutils.egg-info/top_level.txt
+drwxr-xr-x   0 parizeau   (502) staff       (20)        0 2022-04-19 19:23:48.893968 paxutils-0.0.9/
+-rw-r--r--   0 parizeau   (502) staff       (20)     1071 2022-04-08 13:37:32.000000 paxutils-0.0.9/LICENSE
+-rw-r--r--   0 parizeau   (502) staff       (20)      595 2022-04-19 19:23:48.894038 paxutils-0.0.9/PKG-INFO
+-rw-r--r--   0 parizeau   (502) staff       (20)       55 2022-04-08 13:37:32.000000 paxutils-0.0.9/README.md
+-rw-r--r--   0 parizeau   (502) staff       (20)       85 2022-04-08 14:01:49.000000 paxutils-0.0.9/pyproject.toml
+-rw-r--r--   0 parizeau   (502) staff       (20)      649 2022-04-19 19:23:48.894322 paxutils-0.0.9/setup.cfg
+drwxr-xr-x   0 parizeau   (502) staff       (20)        0 2022-04-19 19:23:48.892640 paxutils-0.0.9/src/
+drwxr-xr-x   0 parizeau   (502) staff       (20)        0 2022-04-19 19:23:48.893367 paxutils-0.0.9/src/paxutils/
+-rw-r--r--   0 parizeau   (502) staff       (20)       22 2022-04-19 19:23:35.000000 paxutils-0.0.9/src/paxutils/__init__.py
+-rw-r--r--   0 parizeau   (502) staff       (20)     2894 2022-04-19 19:23:23.000000 paxutils-0.0.9/src/paxutils/path.py
+drwxr-xr-x   0 parizeau   (502) staff       (20)        0 2022-04-19 19:23:48.893869 paxutils-0.0.9/src/paxutils.egg-info/
+-rw-r--r--   0 parizeau   (502) staff       (20)      595 2022-04-19 19:23:48.000000 paxutils-0.0.9/src/paxutils.egg-info/PKG-INFO
+-rw-r--r--   0 parizeau   (502) staff       (20)      232 2022-04-19 19:23:48.000000 paxutils-0.0.9/src/paxutils.egg-info/SOURCES.txt
+-rw-r--r--   0 parizeau   (502) staff       (20)        1 2022-04-19 19:23:48.000000 paxutils-0.0.9/src/paxutils.egg-info/dependency_links.txt
+-rw-r--r--   0 parizeau   (502) staff       (20)        9 2022-04-19 19:23:48.000000 paxutils-0.0.9/src/paxutils.egg-info/top_level.txt
```

### Comparing `paxutils-0.0.8/LICENSE` & `paxutils-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `paxutils-0.0.8/PKG-INFO` & `paxutils-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paxutils
-Version: 0.0.8
+Version: 0.0.9
 Summary: Miscellaneous utilities for PAX notebooks
 Home-page: https://github.com/pax-ul/paxutils
 Author: Marc Parizeau
 Author-email: marc@parizeau.org
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pax-ul/paxutils/issues
 Platform: UNKNOWN
```

### Comparing `paxutils-0.0.8/setup.cfg` & `paxutils-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `paxutils-0.0.8/src/paxutils/path.py` & `paxutils-0.0.9/src/paxutils/path.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             if pathlib.Path('../fichiers').is_dir():
                 # use local relative file path prefix
                 self = super(Path, cls).__new__(cls, '../fichiers', *paths)
                 self._path_index = 2
 
             elif pathlib.Path('/pax/shared', course, *paths).exists():
                 # use local absolute shared prefix
-                self = super(Path, cls).__new__(cls, '/pax/shared', course, *path)
+                self = super(Path, cls).__new__(cls, '/pax/shared', course, *paths)
                 self._path_index = 4
 
             else:
                 # use local writeable temp prefix
                 self = super(Path, cls).__new__(cls, '/tmp/pax', course, *paths)
                 self._path_index = 4
```

### Comparing `paxutils-0.0.8/src/paxutils.egg-info/PKG-INFO` & `paxutils-0.0.9/src/paxutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paxutils
-Version: 0.0.8
+Version: 0.0.9
 Summary: Miscellaneous utilities for PAX notebooks
 Home-page: https://github.com/pax-ul/paxutils
 Author: Marc Parizeau
 Author-email: marc@parizeau.org
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pax-ul/paxutils/issues
 Platform: UNKNOWN
```

