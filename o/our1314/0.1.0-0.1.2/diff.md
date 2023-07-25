# Comparing `tmp/our1314-0.1.0.tar.gz` & `tmp/our1314-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "our1314-0.1.0.tar", last modified: Tue Jul 25 02:31:10 2023, max compression
+gzip compressed data, was "our1314-0.1.2.tar", last modified: Tue Jul 25 02:58:50 2023, max compression
```

## Comparing `our1314-0.1.0.tar` & `our1314-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 02:31:10.672092 our1314-0.1.0/
--rw-rw-rw-   0        0        0      240 2023-07-25 02:31:10.672092 our1314-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       39 2023-07-25 01:35:24.000000 our1314-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 02:31:10.665093 our1314-0.1.0/myutils/
--rw-rw-rw-   0        0        0        0 2023-07-25 02:10:04.000000 our1314-0.1.0/myutils/__init__.py
--rw-rw-rw-   0        0        0     1430 2023-07-10 10:51:17.000000 our1314-0.1.0/myutils/exportsd.py
--rw-rw-rw-   0        0        0     2370 2023-07-10 10:51:17.000000 our1314-0.1.0/myutils/importsd.py
--rw-rw-rw-   0        0        0     5665 2023-07-25 01:36:14.000000 our1314-0.1.0/myutils/myutils.py
-drwxrwxrwx   0        0        0        0 2023-07-25 02:31:10.671094 our1314-0.1.0/our1314.egg-info/
--rw-rw-rw-   0        0        0      240 2023-07-25 02:31:10.000000 our1314-0.1.0/our1314.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-07-25 02:31:10.000000 our1314-0.1.0/our1314.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 02:31:10.000000 our1314-0.1.0/our1314.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-25 02:31:10.000000 our1314-0.1.0/our1314.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 02:31:10.673092 our1314-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      417 2023-07-25 02:31:05.000000 our1314-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:58:50.757015 our1314-0.1.2/
+-rw-rw-rw-   0        0        0     1082 2023-07-25 01:35:24.000000 our1314-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      263 2023-07-25 02:58:50.756016 our1314-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       39 2023-07-25 01:35:24.000000 our1314-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 02:58:50.750015 our1314-0.1.2/myutils/
+-rw-rw-rw-   0        0        0        0 2023-07-25 02:10:04.000000 our1314-0.1.2/myutils/__init__.py
+-rw-rw-rw-   0        0        0     1430 2023-07-10 10:51:17.000000 our1314-0.1.2/myutils/exportsd.py
+-rw-rw-rw-   0        0        0     2370 2023-07-10 10:51:17.000000 our1314-0.1.2/myutils/importsd.py
+-rw-rw-rw-   0        0        0     5665 2023-07-25 01:36:14.000000 our1314-0.1.2/myutils/myutils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:58:50.756016 our1314-0.1.2/our1314.egg-info/
+-rw-rw-rw-   0        0        0      263 2023-07-25 02:58:50.000000 our1314-0.1.2/our1314.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-07-25 02:58:50.000000 our1314-0.1.2/our1314.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 02:58:50.000000 our1314-0.1.2/our1314.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-25 02:58:50.000000 our1314-0.1.2/our1314.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 02:58:50.757015 our1314-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      417 2023-07-25 02:56:58.000000 our1314-0.1.2/setup.py
```

### Comparing `our1314-0.1.0/myutils/exportsd.py` & `our1314-0.1.2/myutils/exportsd.py`

 * *Files identical despite different names*

### Comparing `our1314-0.1.0/myutils/importsd.py` & `our1314-0.1.2/myutils/importsd.py`

 * *Files identical despite different names*

### Comparing `our1314-0.1.0/myutils/myutils.py` & `our1314-0.1.2/myutils/myutils.py`

 * *Files identical despite different names*

