# Comparing `tmp/SMAGrader-0.1.4.tar.gz` & `tmp/SMAGrader-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SMAGrader-0.1.4.tar", last modified: Tue Jul 25 21:36:17 2023, max compression
+gzip compressed data, was "SMAGrader-0.1.5.tar", last modified: Tue Jul 25 21:38:14 2023, max compression
```

## Comparing `SMAGrader-0.1.4.tar` & `SMAGrader-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 21:36:17.119447 SMAGrader-0.1.4/
--rw-rw-rw-   0        0        0       19 2023-07-25 21:29:41.000000 SMAGrader-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      151 2023-07-25 21:36:17.103443 SMAGrader-0.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-25 21:36:17.080438 SMAGrader-0.1.4/SMAGrader/
--rw-rw-rw-   0        0        0        0 2023-07-25 19:17:05.000000 SMAGrader-0.1.4/SMAGrader/__init__.py
--rw-rw-rw-   0        0        0    18856 2023-07-25 21:33:10.000000 SMAGrader-0.1.4/SMAGrader/checker.py
-drwxrwxrwx   0        0        0        0 2023-07-25 21:36:17.100443 SMAGrader-0.1.4/SMAGrader.egg-info/
--rw-rw-rw-   0        0        0      151 2023-07-25 21:36:16.000000 SMAGrader-0.1.4/SMAGrader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-07-25 21:36:16.000000 SMAGrader-0.1.4/SMAGrader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 21:36:16.000000 SMAGrader-0.1.4/SMAGrader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-25 21:36:16.000000 SMAGrader-0.1.4/SMAGrader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-25 21:36:16.000000 SMAGrader-0.1.4/SMAGrader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 21:36:17.119447 SMAGrader-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      426 2023-07-25 21:35:43.000000 SMAGrader-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 21:38:14.101031 SMAGrader-0.1.5/
+-rw-rw-rw-   0        0        0      151 2023-07-25 21:38:14.100031 SMAGrader-0.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-25 21:38:14.079026 SMAGrader-0.1.5/SMAGrader/
+-rw-rw-rw-   0        0        0        0 2023-07-25 19:17:05.000000 SMAGrader-0.1.5/SMAGrader/__init__.py
+-rw-rw-rw-   0        0        0    18856 2023-07-25 21:33:10.000000 SMAGrader-0.1.5/SMAGrader/checker.py
+drwxrwxrwx   0        0        0        0 2023-07-25 21:38:14.097030 SMAGrader-0.1.5/SMAGrader.egg-info/
+-rw-rw-rw-   0        0        0      151 2023-07-25 21:38:13.000000 SMAGrader-0.1.5/SMAGrader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-07-25 21:38:13.000000 SMAGrader-0.1.5/SMAGrader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 21:38:13.000000 SMAGrader-0.1.5/SMAGrader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-25 21:38:13.000000 SMAGrader-0.1.5/SMAGrader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-25 21:38:13.000000 SMAGrader-0.1.5/SMAGrader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 21:38:14.101031 SMAGrader-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      426 2023-07-25 21:38:11.000000 SMAGrader-0.1.5/setup.py
```

### Comparing `SMAGrader-0.1.4/SMAGrader/checker.py` & `SMAGrader-0.1.5/SMAGrader/checker.py`

 * *Files identical despite different names*

