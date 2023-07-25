# Comparing `tmp/greetnow-1.0.0.tar.gz` & `tmp/greetnow-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greetnow-1.0.0.tar", last modified: Mon Jul 24 18:09:53 2023, max compression
+gzip compressed data, was "greetnow-1.0.1.tar", last modified: Tue Jul 25 04:52:16 2023, max compression
```

## Comparing `greetnow-1.0.0.tar` & `greetnow-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 fourofour   (501) staff       (20)        0 2023-07-24 18:09:53.407767 greetnow-1.0.0/
--rw-r--r--   0 fourofour   (501) staff       (20)      222 2023-07-24 18:09:53.407641 greetnow-1.0.0/PKG-INFO
-drwxr-xr-x   0 fourofour   (501) staff       (20)        0 2023-07-24 18:09:53.406160 greetnow-1.0.0/greetnow/
--rw-r--r--   0 fourofour   (501) staff       (20)       50 2023-07-24 17:59:41.000000 greetnow-1.0.0/greetnow/__init__.py
-drwxr-xr-x   0 fourofour   (501) staff       (20)        0 2023-07-24 18:09:53.406978 greetnow-1.0.0/greetnow/evening/
--rw-r--r--   0 fourofour   (501) staff       (20)       29 2023-07-24 18:01:02.000000 greetnow-1.0.0/greetnow/evening/__init__.py
--rw-r--r--   0 fourofour   (501) staff       (20)       69 2023-07-24 18:06:45.000000 greetnow-1.0.0/greetnow/evening/even_greet.py
--rw-r--r--   0 fourofour   (501) staff       (20)       50 2023-07-24 18:00:01.000000 greetnow-1.0.0/greetnow/generic.py
-drwxr-xr-x   0 fourofour   (501) staff       (20)        0 2023-07-24 18:09:53.407206 greetnow-1.0.0/greetnow/morning/
--rw-r--r--   0 fourofour   (501) staff       (20)       29 2023-07-24 18:00:52.000000 greetnow-1.0.0/greetnow/morning/__init__.py
--rw-r--r--   0 fourofour   (501) staff       (20)       61 2023-07-24 18:06:24.000000 greetnow-1.0.0/greetnow/morning/mng_greet.py
-drwxr-xr-x   0 fourofour   (501) staff       (20)        0 2023-07-24 18:09:53.407451 greetnow-1.0.0/greetnow/noon/
--rw-r--r--   0 fourofour   (501) staff       (20)       50 2023-07-24 18:00:41.000000 greetnow-1.0.0/greetnow/noon/__init__.py
--rw-r--r--   0 fourofour   (501) staff       (20)       55 2023-07-24 18:00:29.000000 greetnow-1.0.0/greetnow/noon/noon_greet.py
-drwxr-xr-x   0 fourofour   (501) staff       (20)        0 2023-07-24 18:09:53.406746 greetnow-1.0.0/greetnow.egg-info/
--rw-r--r--   0 fourofour   (501) staff       (20)      222 2023-07-24 18:09:53.000000 greetnow-1.0.0/greetnow.egg-info/PKG-INFO
--rw-r--r--   0 fourofour   (501) staff       (20)      350 2023-07-24 18:09:53.000000 greetnow-1.0.0/greetnow.egg-info/SOURCES.txt
--rw-r--r--   0 fourofour   (501) staff       (20)        1 2023-07-24 18:09:53.000000 greetnow-1.0.0/greetnow.egg-info/dependency_links.txt
--rw-r--r--   0 fourofour   (501) staff       (20)        9 2023-07-24 18:09:53.000000 greetnow-1.0.0/greetnow.egg-info/top_level.txt
--rw-r--r--   0 fourofour   (501) staff       (20)       38 2023-07-24 18:09:53.407811 greetnow-1.0.0/setup.cfg
--rw-r--r--   0 fourofour   (501) staff       (20)      373 2023-07-24 18:09:08.000000 greetnow-1.0.0/setup.py
+drwxr-xr-x   0 fourofour   (501) staff       (20)        0 2023-07-25 04:52:16.741394 greetnow-1.0.1/
+-rw-r--r--   0 fourofour   (501) staff       (20)      222 2023-07-25 04:52:16.741257 greetnow-1.0.1/PKG-INFO
+drwxr-xr-x   0 fourofour   (501) staff       (20)        0 2023-07-25 04:52:16.739334 greetnow-1.0.1/greetnow/
+-rw-r--r--   0 fourofour   (501) staff       (20)       50 2023-07-24 17:59:41.000000 greetnow-1.0.1/greetnow/__init__.py
+drwxr-xr-x   0 fourofour   (501) staff       (20)        0 2023-07-25 04:52:16.740506 greetnow-1.0.1/greetnow/evening/
+-rw-r--r--   0 fourofour   (501) staff       (20)       29 2023-07-24 18:01:02.000000 greetnow-1.0.1/greetnow/evening/__init__.py
+-rw-r--r--   0 fourofour   (501) staff       (20)       69 2023-07-24 18:06:45.000000 greetnow-1.0.1/greetnow/evening/even_greet.py
+-rw-r--r--   0 fourofour   (501) staff       (20)       50 2023-07-24 18:00:01.000000 greetnow-1.0.1/greetnow/generic.py
+drwxr-xr-x   0 fourofour   (501) staff       (20)        0 2023-07-25 04:52:16.740803 greetnow-1.0.1/greetnow/morning/
+-rw-r--r--   0 fourofour   (501) staff       (20)       29 2023-07-24 18:00:52.000000 greetnow-1.0.1/greetnow/morning/__init__.py
+-rw-r--r--   0 fourofour   (501) staff       (20)       61 2023-07-24 18:06:24.000000 greetnow-1.0.1/greetnow/morning/mng_greet.py
+drwxr-xr-x   0 fourofour   (501) staff       (20)        0 2023-07-25 04:52:16.741063 greetnow-1.0.1/greetnow/noon/
+-rw-r--r--   0 fourofour   (501) staff       (20)       50 2023-07-24 18:00:41.000000 greetnow-1.0.1/greetnow/noon/__init__.py
+-rw-r--r--   0 fourofour   (501) staff       (20)       55 2023-07-24 18:00:29.000000 greetnow-1.0.1/greetnow/noon/noon_greet.py
+drwxr-xr-x   0 fourofour   (501) staff       (20)        0 2023-07-25 04:52:16.740187 greetnow-1.0.1/greetnow.egg-info/
+-rw-r--r--   0 fourofour   (501) staff       (20)      222 2023-07-25 04:52:16.000000 greetnow-1.0.1/greetnow.egg-info/PKG-INFO
+-rw-r--r--   0 fourofour   (501) staff       (20)      350 2023-07-25 04:52:16.000000 greetnow-1.0.1/greetnow.egg-info/SOURCES.txt
+-rw-r--r--   0 fourofour   (501) staff       (20)        1 2023-07-25 04:52:16.000000 greetnow-1.0.1/greetnow.egg-info/dependency_links.txt
+-rw-r--r--   0 fourofour   (501) staff       (20)        9 2023-07-25 04:52:16.000000 greetnow-1.0.1/greetnow.egg-info/top_level.txt
+-rw-r--r--   0 fourofour   (501) staff       (20)       38 2023-07-25 04:52:16.741441 greetnow-1.0.1/setup.cfg
+-rw-r--r--   0 fourofour   (501) staff       (20)      373 2023-07-25 04:50:19.000000 greetnow-1.0.1/setup.py
```

