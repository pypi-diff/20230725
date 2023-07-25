# Comparing `tmp/denari-1.0.8.tar.gz` & `tmp/denari-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denari-1.0.8.tar", last modified: Wed Mar  1 23:34:40 2023, max compression
+gzip compressed data, was "denari-1.0.9.tar", last modified: Thu Mar  2 00:02:38 2023, max compression
```

## Comparing `denari-1.0.8.tar` & `denari-1.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-03-01 23:34:40.341082 denari-1.0.8/
--rw-rw-rw-   0        0        0        0 2023-03-01 23:30:35.000000 denari-1.0.8/LICENCE
--rw-rw-rw-   0        0        0      200 2023-03-01 23:34:40.340080 denari-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-03-01 23:30:08.000000 denari-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-01 23:34:40.339081 denari-1.0.8/denari.egg-info/
--rw-rw-rw-   0        0        0      200 2023-03-01 23:34:39.000000 denari-1.0.8/denari.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      175 2023-03-01 23:34:39.000000 denari-1.0.8/denari.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-01 23:34:39.000000 denari-1.0.8/denari.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-03-01 23:34:39.000000 denari-1.0.8/denari.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-03-01 23:34:39.000000 denari-1.0.8/denari.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-01 23:34:40.341082 denari-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      364 2023-03-01 23:29:56.000000 denari-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-02 00:02:38.583162 denari-1.0.9/
+-rw-rw-rw-   0        0        0        0 2023-03-01 23:30:35.000000 denari-1.0.9/LICENCE
+-rw-rw-rw-   0        0        0      200 2023-03-02 00:02:38.583162 denari-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-03-01 23:30:08.000000 denari-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-02 00:02:38.581163 denari-1.0.9/denari.egg-info/
+-rw-rw-rw-   0        0        0      200 2023-03-02 00:02:38.000000 denari-1.0.9/denari.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      175 2023-03-02 00:02:38.000000 denari-1.0.9/denari.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-02 00:02:38.000000 denari-1.0.9/denari.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-03-02 00:02:38.000000 denari-1.0.9/denari.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-03-02 00:02:38.000000 denari-1.0.9/denari.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-02 00:02:38.583162 denari-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      364 2023-03-01 23:45:25.000000 denari-1.0.9/setup.py
```

