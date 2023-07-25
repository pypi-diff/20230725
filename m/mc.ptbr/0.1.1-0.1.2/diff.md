# Comparing `tmp/mc.ptbr-0.1.1.tar.gz` & `tmp/mc.ptbr-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mc.ptbr-0.1.1.tar", last modified: Tue Jul 25 13:41:46 2023, max compression
+gzip compressed data, was "mc.ptbr-0.1.2.tar", last modified: Tue Jul 25 13:45:42 2023, max compression
```

## Comparing `mc.ptbr-0.1.1.tar` & `mc.ptbr-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 13:41:46.892613 mc.ptbr-0.1.1/
--rw-rw-rw-   0        0        0      177 2023-07-25 13:41:46.892613 mc.ptbr-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-25 13:41:46.876978 mc.ptbr-0.1.1/mc.ptbr.egg-info/
--rw-rw-rw-   0        0        0      177 2023-07-25 13:41:46.000000 mc.ptbr-0.1.1/mc.ptbr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-07-25 13:41:46.000000 mc.ptbr-0.1.1/mc.ptbr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 13:41:46.000000 mc.ptbr-0.1.1/mc.ptbr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-25 13:41:46.000000 mc.ptbr-0.1.1/mc.ptbr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 13:41:46.000000 mc.ptbr-0.1.1/mc.ptbr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 13:41:46.892613 mc.ptbr-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      492 2023-07-25 13:40:56.000000 mc.ptbr-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 13:45:42.836065 mc.ptbr-0.1.2/
+-rw-rw-rw-   0        0        0      177 2023-07-25 13:45:42.836065 mc.ptbr-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-25 13:45:42.836065 mc.ptbr-0.1.2/mc.ptbr.egg-info/
+-rw-rw-rw-   0        0        0      177 2023-07-25 13:45:42.000000 mc.ptbr-0.1.2/mc.ptbr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2023-07-25 13:45:42.000000 mc.ptbr-0.1.2/mc.ptbr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 13:45:42.000000 mc.ptbr-0.1.2/mc.ptbr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-25 13:45:42.000000 mc.ptbr-0.1.2/mc.ptbr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 13:45:42.000000 mc.ptbr-0.1.2/mc.ptbr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 13:45:42.836065 mc.ptbr-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      492 2023-07-25 13:44:13.000000 mc.ptbr-0.1.2/setup.py
```

