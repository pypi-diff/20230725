# Comparing `tmp/our1314-0.1.4.tar.gz` & `tmp/our1314-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "our1314-0.1.4.tar", last modified: Tue Jul 25 06:03:52 2023, max compression
+gzip compressed data, was "our1314-0.1.5.tar", last modified: Tue Jul 25 06:06:31 2023, max compression
```

## Comparing `our1314-0.1.4.tar` & `our1314-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 06:03:52.151418 our1314-0.1.4/
--rw-rw-rw-   0        0        0     1082 2023-07-25 01:35:24.000000 our1314-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      263 2023-07-25 06:03:52.150417 our1314-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       39 2023-07-25 01:35:24.000000 our1314-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 06:03:52.124415 our1314-0.1.4/our1314/
--rw-rw-rw-   0        0        0        0 2023-07-25 02:10:04.000000 our1314-0.1.4/our1314/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 06:03:52.149416 our1314-0.1.4/our1314/myutils/
--rw-rw-rw-   0        0        0        0 2023-07-25 02:10:04.000000 our1314-0.1.4/our1314/myutils/__init__.py
--rw-rw-rw-   0        0        0     1430 2023-07-10 10:51:17.000000 our1314-0.1.4/our1314/myutils/exportsd.py
--rw-rw-rw-   0        0        0     2370 2023-07-10 10:51:17.000000 our1314-0.1.4/our1314/myutils/importsd.py
--rw-rw-rw-   0        0        0     5426 2023-07-25 05:56:11.000000 our1314-0.1.4/our1314/myutils/myutils.py
-drwxrwxrwx   0        0        0        0 2023-07-25 06:03:52.137415 our1314-0.1.4/our1314.egg-info/
--rw-rw-rw-   0        0        0      263 2023-07-25 06:03:52.000000 our1314-0.1.4/our1314.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2023-07-25 06:03:52.000000 our1314-0.1.4/our1314.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 06:03:52.000000 our1314-0.1.4/our1314.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-25 06:03:52.000000 our1314-0.1.4/our1314.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 06:03:52.151418 our1314-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      417 2023-07-25 06:02:46.000000 our1314-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:06:31.380876 our1314-0.1.5/
+-rw-rw-rw-   0        0        0     1082 2023-07-25 01:35:24.000000 our1314-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      263 2023-07-25 06:06:31.380876 our1314-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       39 2023-07-25 01:35:24.000000 our1314-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 06:06:31.371874 our1314-0.1.5/our1314/
+-rw-rw-rw-   0        0        0        0 2023-07-25 02:10:04.000000 our1314-0.1.5/our1314/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:06:31.377874 our1314-0.1.5/our1314/cv/
+-rw-rw-rw-   0        0        0        0 2023-07-25 06:04:58.000000 our1314-0.1.5/our1314/cv/__init__.py
+-rw-rw-rw-   0        0        0     1240 2023-07-25 05:55:44.000000 our1314-0.1.5/our1314/cv/mouseselect.py
+-rw-rw-rw-   0        0        0      960 2023-07-25 06:04:38.000000 our1314-0.1.5/our1314/cv/templatematch.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:06:31.379874 our1314-0.1.5/our1314/myutils/
+-rw-rw-rw-   0        0        0        0 2023-07-25 02:10:04.000000 our1314-0.1.5/our1314/myutils/__init__.py
+-rw-rw-rw-   0        0        0     1430 2023-07-10 10:51:17.000000 our1314-0.1.5/our1314/myutils/exportsd.py
+-rw-rw-rw-   0        0        0     2370 2023-07-10 10:51:17.000000 our1314-0.1.5/our1314/myutils/importsd.py
+-rw-rw-rw-   0        0        0     5426 2023-07-25 05:56:11.000000 our1314-0.1.5/our1314/myutils/myutils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:06:31.375873 our1314-0.1.5/our1314.egg-info/
+-rw-rw-rw-   0        0        0      263 2023-07-25 06:06:31.000000 our1314-0.1.5/our1314.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-07-25 06:06:31.000000 our1314-0.1.5/our1314.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 06:06:31.000000 our1314-0.1.5/our1314.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-25 06:06:31.000000 our1314-0.1.5/our1314.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 06:06:31.380876 our1314-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      417 2023-07-25 06:05:36.000000 our1314-0.1.5/setup.py
```

### Comparing `our1314-0.1.4/LICENSE` & `our1314-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `our1314-0.1.4/our1314/myutils/exportsd.py` & `our1314-0.1.5/our1314/myutils/exportsd.py`

 * *Files identical despite different names*

### Comparing `our1314-0.1.4/our1314/myutils/importsd.py` & `our1314-0.1.5/our1314/myutils/importsd.py`

 * *Files identical despite different names*

### Comparing `our1314-0.1.4/our1314/myutils/myutils.py` & `our1314-0.1.5/our1314/myutils/myutils.py`

 * *Files identical despite different names*

