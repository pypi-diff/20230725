# Comparing `tmp/SMAGrader-0.1.2.tar.gz` & `tmp/SMAGrader-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SMAGrader-0.1.2.tar", last modified: Tue Jul 25 19:17:38 2023, max compression
+gzip compressed data, was "SMAGrader-0.1.3.tar", last modified: Tue Jul 25 19:31:57 2023, max compression
```

## Comparing `SMAGrader-0.1.2.tar` & `SMAGrader-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 19:17:38.126816 SMAGrader-0.1.2/
--rw-rw-rw-   0        0        0      151 2023-07-25 19:17:38.125816 SMAGrader-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-25 19:17:38.104812 SMAGrader-0.1.2/SMAGrader/
--rw-rw-rw-   0        0        0        0 2023-07-25 19:17:05.000000 SMAGrader-0.1.2/SMAGrader/__init__.py
--rw-rw-rw-   0        0        0    18791 2023-07-25 19:16:39.000000 SMAGrader-0.1.2/SMAGrader/checker.py
--rw-rw-rw-   0        0        0      112 2023-07-11 20:15:42.000000 SMAGrader-0.1.2/SMAGrader/constants.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:17:38.123817 SMAGrader-0.1.2/SMAGrader.egg-info/
--rw-rw-rw-   0        0        0      151 2023-07-25 19:17:37.000000 SMAGrader-0.1.2/SMAGrader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-07-25 19:17:38.000000 SMAGrader-0.1.2/SMAGrader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 19:17:37.000000 SMAGrader-0.1.2/SMAGrader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-25 19:17:37.000000 SMAGrader-0.1.2/SMAGrader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-25 19:17:37.000000 SMAGrader-0.1.2/SMAGrader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 19:17:38.126816 SMAGrader-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      426 2023-07-25 19:17:30.000000 SMAGrader-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:31:57.066880 SMAGrader-0.1.3/
+-rw-rw-rw-   0        0        0      151 2023-07-25 19:31:57.065879 SMAGrader-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-25 19:31:57.042874 SMAGrader-0.1.3/SMAGrader/
+-rw-rw-rw-   0        0        0        0 2023-07-25 19:17:05.000000 SMAGrader-0.1.3/SMAGrader/__init__.py
+-rw-rw-rw-   0        0        0    18791 2023-07-25 19:30:35.000000 SMAGrader-0.1.3/SMAGrader/checker.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:31:57.063880 SMAGrader-0.1.3/SMAGrader.egg-info/
+-rw-rw-rw-   0        0        0      151 2023-07-25 19:31:56.000000 SMAGrader-0.1.3/SMAGrader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-07-25 19:31:56.000000 SMAGrader-0.1.3/SMAGrader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 19:31:56.000000 SMAGrader-0.1.3/SMAGrader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-25 19:31:56.000000 SMAGrader-0.1.3/SMAGrader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-25 19:31:56.000000 SMAGrader-0.1.3/SMAGrader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 19:31:57.066880 SMAGrader-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      426 2023-07-25 19:31:47.000000 SMAGrader-0.1.3/setup.py
```

### Comparing `SMAGrader-0.1.2/SMAGrader/checker.py` & `SMAGrader-0.1.3/SMAGrader/checker.py`

 * *Files identical despite different names*

