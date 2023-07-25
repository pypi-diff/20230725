# Comparing `tmp/easyID3-0.1.3.tar.gz` & `tmp/easyID3-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyID3-0.1.3.tar", last modified: Tue Jul 25 04:15:08 2023, max compression
+gzip compressed data, was "easyID3-0.1.4.tar", last modified: Tue Jul 25 04:29:18 2023, max compression
```

## Comparing `easyID3-0.1.3.tar` & `easyID3-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 04:15:08.955784 easyID3-0.1.3/
--rw-rw-rw-   0        0        0     1090 2023-07-24 20:54:59.000000 easyID3-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      214 2023-07-25 04:15:08.955784 easyID3-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-07-25 03:09:08.000000 easyID3-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 04:15:08.953789 easyID3-0.1.3/easyID3.egg-info/
--rw-rw-rw-   0        0        0      214 2023-07-25 04:15:08.000000 easyID3-0.1.3/easyID3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-07-25 04:15:08.000000 easyID3-0.1.3/easyID3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 04:15:08.000000 easyID3-0.1.3/easyID3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-25 04:15:08.000000 easyID3-0.1.3/easyID3.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 04:15:08.000000 easyID3-0.1.3/easyID3.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 04:15:08.955784 easyID3-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      352 2023-07-25 04:14:52.000000 easyID3-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 04:29:18.752512 easyID3-0.1.4/
+-rw-rw-rw-   0        0        0     1090 2023-07-24 20:54:59.000000 easyID3-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      214 2023-07-25 04:29:18.751509 easyID3-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-07-25 03:09:08.000000 easyID3-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 04:29:18.750008 easyID3-0.1.4/easyID3.egg-info/
+-rw-rw-rw-   0        0        0      214 2023-07-25 04:29:18.000000 easyID3-0.1.4/easyID3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2023-07-25 04:29:18.000000 easyID3-0.1.4/easyID3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 04:29:18.000000 easyID3-0.1.4/easyID3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-25 04:29:18.000000 easyID3-0.1.4/easyID3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 04:29:18.000000 easyID3-0.1.4/easyID3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 04:29:18.753507 easyID3-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      352 2023-07-25 04:29:15.000000 easyID3-0.1.4/setup.py
```

### Comparing `easyID3-0.1.3/LICENSE` & `easyID3-0.1.4/LICENSE`

 * *Files identical despite different names*

