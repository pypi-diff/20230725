# Comparing `tmp/trolldaddy-1.0.0.tar.gz` & `tmp/trolldaddy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trolldaddy-1.0.0.tar", last modified: Mon Jul 24 05:20:55 2023, max compression
+gzip compressed data, was "trolldaddy-1.0.1.tar", last modified: Tue Jul 25 02:09:39 2023, max compression
```

## Comparing `trolldaddy-1.0.0.tar` & `trolldaddy-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 05:20:55.114286 trolldaddy-1.0.0/
--rw-rw-rw-   0        0        0        0 2023-07-17 05:21:13.000000 trolldaddy-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      370 2023-07-24 05:20:55.043281 trolldaddy-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-07-24 05:19:45.000000 trolldaddy-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-24 05:20:55.115285 trolldaddy-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      592 2023-07-24 05:20:23.000000 trolldaddy-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 05:20:54.920271 trolldaddy-1.0.0/trolldaddy/
--rw-rw-rw-   0        0        0        0 2023-07-17 05:21:50.000000 trolldaddy-1.0.0/trolldaddy/__init__.py
--rw-rw-rw-   0        0        0     5595 2023-07-24 05:17:24.000000 trolldaddy-1.0.0/trolldaddy/trolldaddy.py
-drwxrwxrwx   0        0        0        0 2023-07-24 05:20:55.039281 trolldaddy-1.0.0/trolldaddy.egg-info/
--rw-rw-rw-   0        0        0      370 2023-07-24 05:20:54.000000 trolldaddy-1.0.0/trolldaddy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-07-24 05:20:54.000000 trolldaddy-1.0.0/trolldaddy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 05:20:54.000000 trolldaddy-1.0.0/trolldaddy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-24 05:20:54.000000 trolldaddy-1.0.0/trolldaddy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 02:09:39.422362 trolldaddy-1.0.1/
+-rw-rw-rw-   0        0        0        0 2023-07-17 05:21:13.000000 trolldaddy-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      379 2023-07-25 02:09:39.415362 trolldaddy-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-07-24 05:19:45.000000 trolldaddy-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-25 02:09:39.422362 trolldaddy-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      748 2023-07-25 02:08:58.000000 trolldaddy-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:09:39.321790 trolldaddy-1.0.1/trolldaddy/
+-rw-rw-rw-   0        0        0        0 2023-07-17 05:21:50.000000 trolldaddy-1.0.1/trolldaddy/__init__.py
+-rw-rw-rw-   0        0        0     5595 2023-07-24 05:17:24.000000 trolldaddy-1.0.1/trolldaddy/trolldaddy.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:09:39.410362 trolldaddy-1.0.1/trolldaddy.egg-info/
+-rw-rw-rw-   0        0        0      379 2023-07-25 02:09:37.000000 trolldaddy-1.0.1/trolldaddy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-07-25 02:09:37.000000 trolldaddy-1.0.1/trolldaddy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 02:09:37.000000 trolldaddy-1.0.1/trolldaddy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-25 02:09:37.000000 trolldaddy-1.0.1/trolldaddy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-25 02:09:37.000000 trolldaddy-1.0.1/trolldaddy.egg-info/top_level.txt
```

### Comparing `trolldaddy-1.0.0/trolldaddy/trolldaddy.py` & `trolldaddy-1.0.1/trolldaddy/trolldaddy.py`

 * *Files identical despite different names*

