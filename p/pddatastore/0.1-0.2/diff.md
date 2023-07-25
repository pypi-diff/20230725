# Comparing `tmp/pddatastore-0.1.tar.gz` & `tmp/pddatastore-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pddatastore-0.1.tar", last modified: Wed Jul 12 23:23:34 2023, max compression
+gzip compressed data, was "pddatastore-0.2.tar", last modified: Tue Jul 25 14:40:23 2023, max compression
```

## Comparing `pddatastore-0.1.tar` & `pddatastore-0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 23:23:34.022092 pddatastore-0.1/
--rw-rw-rw-   0        0        0      166 2023-07-12 23:23:34.021085 pddatastore-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-12 23:23:34.021085 pddatastore-0.1/pddatastore.egg-info/
--rw-rw-rw-   0        0        0      166 2023-07-12 23:23:33.000000 pddatastore-0.1/pddatastore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      148 2023-07-12 23:23:33.000000 pddatastore-0.1/pddatastore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 23:23:33.000000 pddatastore-0.1/pddatastore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 23:23:33.000000 pddatastore-0.1/pddatastore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 23:23:34.023090 pddatastore-0.1/setup.cfg
--rw-rw-rw-   0        0        0      256 2023-07-12 23:22:55.000000 pddatastore-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:40:23.097220 pddatastore-0.2/
+-rw-rw-rw-   0        0        0      166 2023-07-25 14:40:23.096221 pddatastore-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-25 14:40:23.096221 pddatastore-0.2/pddatastore.egg-info/
+-rw-rw-rw-   0        0        0      166 2023-07-25 14:40:22.000000 pddatastore-0.2/pddatastore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      148 2023-07-25 14:40:23.000000 pddatastore-0.2/pddatastore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 14:40:22.000000 pddatastore-0.2/pddatastore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 14:40:22.000000 pddatastore-0.2/pddatastore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 14:40:23.097220 pddatastore-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      256 2023-07-25 14:39:53.000000 pddatastore-0.2/setup.py
```

