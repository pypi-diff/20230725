# Comparing `tmp/easyID3-0.1.4.tar.gz` & `tmp/easyID3-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyID3-0.1.4.tar", last modified: Tue Jul 25 04:29:18 2023, max compression
+gzip compressed data, was "easyID3-0.1.5.tar", last modified: Tue Jul 25 05:17:41 2023, max compression
```

## Comparing `easyID3-0.1.4.tar` & `easyID3-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 04:29:18.752512 easyID3-0.1.4/
--rw-rw-rw-   0        0        0     1090 2023-07-24 20:54:59.000000 easyID3-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      214 2023-07-25 04:29:18.751509 easyID3-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-07-25 03:09:08.000000 easyID3-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 04:29:18.750008 easyID3-0.1.4/easyID3.egg-info/
--rw-rw-rw-   0        0        0      214 2023-07-25 04:29:18.000000 easyID3-0.1.4/easyID3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-07-25 04:29:18.000000 easyID3-0.1.4/easyID3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 04:29:18.000000 easyID3-0.1.4/easyID3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-25 04:29:18.000000 easyID3-0.1.4/easyID3.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 04:29:18.000000 easyID3-0.1.4/easyID3.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 04:29:18.753507 easyID3-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      352 2023-07-25 04:29:15.000000 easyID3-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 05:17:41.089821 easyID3-0.1.5/
+-rw-rw-rw-   0        0        0     1090 2023-07-24 20:54:59.000000 easyID3-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      214 2023-07-25 05:17:41.089821 easyID3-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-07-25 03:09:08.000000 easyID3-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 05:17:41.068280 easyID3-0.1.5/easyID3/
+-rw-rw-rw-   0        0        0       43 2023-07-25 04:13:00.000000 easyID3-0.1.5/easyID3/__init__.py
+-rw-rw-rw-   0        0        0      279 2023-07-25 04:25:46.000000 easyID3-0.1.5/easyID3/node.py
+-rw-rw-rw-   0        0        0     8991 2023-07-25 04:24:56.000000 easyID3-0.1.5/easyID3/tree.py
+drwxrwxrwx   0        0        0        0 2023-07-25 05:17:41.088636 easyID3-0.1.5/easyID3.egg-info/
+-rw-rw-rw-   0        0        0      214 2023-07-25 05:17:40.000000 easyID3-0.1.5/easyID3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-07-25 05:17:40.000000 easyID3-0.1.5/easyID3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 05:17:40.000000 easyID3-0.1.5/easyID3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-25 05:17:40.000000 easyID3-0.1.5/easyID3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-25 05:17:40.000000 easyID3-0.1.5/easyID3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 05:17:41.089821 easyID3-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      352 2023-07-25 05:16:22.000000 easyID3-0.1.5/setup.py
```

### Comparing `easyID3-0.1.4/LICENSE` & `easyID3-0.1.5/LICENSE`

 * *Files identical despite different names*

