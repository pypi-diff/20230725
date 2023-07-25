# Comparing `tmp/demo_rowan08-0.0.2.tar.gz` & `tmp/demo_rowan08-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "demo_rowan08-0.0.2.tar", last modified: Tue Jul 25 12:51:38 2023, max compression
+gzip compressed data, was "demo_rowan08-0.0.3.tar", last modified: Tue Jul 25 12:57:13 2023, max compression
```

## Comparing `demo_rowan08-0.0.2.tar` & `demo_rowan08-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2023-07-25 12:51:38.323371 demo_rowan08-0.0.2/
--rw-r--r--   0 rowan     (1000) rowan     (1000)        0 2023-07-25 08:44:28.000000 demo_rowan08-0.0.2/LICENSE
--rw-r--r--   0 rowan     (1000) rowan     (1000)      489 2023-07-25 12:51:38.323371 demo_rowan08-0.0.2/PKG-INFO
--rw-r--r--   0 rowan     (1000) rowan     (1000)        0 2023-07-25 08:44:28.000000 demo_rowan08-0.0.2/README.md
--rw-r--r--   0 rowan     (1000) rowan     (1000)      680 2023-07-25 12:51:26.000000 demo_rowan08-0.0.2/pyproject.toml
--rw-r--r--   0 rowan     (1000) rowan     (1000)       38 2023-07-25 12:51:38.323371 demo_rowan08-0.0.2/setup.cfg
-drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2023-07-25 12:51:38.320038 demo_rowan08-0.0.2/src/
-drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2023-07-25 12:51:38.320038 demo_rowan08-0.0.2/src/demo_rowan08/
--rw-r--r--   0 rowan     (1000) rowan     (1000)        0 2023-07-25 08:46:59.000000 demo_rowan08-0.0.2/src/demo_rowan08/__init__.py
--rw-r--r--   0 rowan     (1000) rowan     (1000)      112 2023-07-25 08:50:48.000000 demo_rowan08-0.0.2/src/demo_rowan08/demo_mod.py
--rw-r--r--   0 rowan     (1000) rowan     (1000)      213 2023-07-25 08:53:18.000000 demo_rowan08-0.0.2/src/demo_rowan08/extra.py
--rw-r--r--   0 rowan     (1000) rowan     (1000)      170 2023-07-25 12:40:29.000000 demo_rowan08-0.0.2/src/demo_rowan08/maths_stuff.py
-drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2023-07-25 12:51:38.323371 demo_rowan08-0.0.2/src/demo_rowan08.egg-info/
--rw-r--r--   0 rowan     (1000) rowan     (1000)      489 2023-07-25 12:51:38.000000 demo_rowan08-0.0.2/src/demo_rowan08.egg-info/PKG-INFO
--rw-r--r--   0 rowan     (1000) rowan     (1000)      347 2023-07-25 12:51:38.000000 demo_rowan08-0.0.2/src/demo_rowan08.egg-info/SOURCES.txt
--rw-r--r--   0 rowan     (1000) rowan     (1000)        1 2023-07-25 12:51:38.000000 demo_rowan08-0.0.2/src/demo_rowan08.egg-info/dependency_links.txt
--rw-r--r--   0 rowan     (1000) rowan     (1000)       14 2023-07-25 12:51:38.000000 demo_rowan08-0.0.2/src/demo_rowan08.egg-info/requires.txt
--rw-r--r--   0 rowan     (1000) rowan     (1000)       13 2023-07-25 12:51:38.000000 demo_rowan08-0.0.2/src/demo_rowan08.egg-info/top_level.txt
+drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2023-07-25 12:57:13.665298 demo_rowan08-0.0.3/
+-rw-r--r--   0 rowan     (1000) rowan     (1000)        0 2023-07-25 08:44:28.000000 demo_rowan08-0.0.3/LICENSE
+-rw-r--r--   0 rowan     (1000) rowan     (1000)      489 2023-07-25 12:57:13.665298 demo_rowan08-0.0.3/PKG-INFO
+-rw-r--r--   0 rowan     (1000) rowan     (1000)        0 2023-07-25 08:44:28.000000 demo_rowan08-0.0.3/README.md
+-rw-r--r--   0 rowan     (1000) rowan     (1000)      741 2023-07-25 12:57:04.000000 demo_rowan08-0.0.3/pyproject.toml
+-rw-r--r--   0 rowan     (1000) rowan     (1000)       14 2023-07-25 12:55:44.000000 demo_rowan08-0.0.3/requirements.txt
+-rw-r--r--   0 rowan     (1000) rowan     (1000)       38 2023-07-25 12:57:13.665298 demo_rowan08-0.0.3/setup.cfg
+drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2023-07-25 12:57:13.661965 demo_rowan08-0.0.3/src/
+drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2023-07-25 12:57:13.665298 demo_rowan08-0.0.3/src/demo_rowan08/
+-rw-r--r--   0 rowan     (1000) rowan     (1000)        0 2023-07-25 08:46:59.000000 demo_rowan08-0.0.3/src/demo_rowan08/__init__.py
+-rw-r--r--   0 rowan     (1000) rowan     (1000)      112 2023-07-25 08:50:48.000000 demo_rowan08-0.0.3/src/demo_rowan08/demo_mod.py
+-rw-r--r--   0 rowan     (1000) rowan     (1000)      213 2023-07-25 08:53:18.000000 demo_rowan08-0.0.3/src/demo_rowan08/extra.py
+-rw-r--r--   0 rowan     (1000) rowan     (1000)      170 2023-07-25 12:40:29.000000 demo_rowan08-0.0.3/src/demo_rowan08/maths_stuff.py
+drwxr-xr-x   0 rowan     (1000) rowan     (1000)        0 2023-07-25 12:57:13.665298 demo_rowan08-0.0.3/src/demo_rowan08.egg-info/
+-rw-r--r--   0 rowan     (1000) rowan     (1000)      489 2023-07-25 12:57:13.000000 demo_rowan08-0.0.3/src/demo_rowan08.egg-info/PKG-INFO
+-rw-r--r--   0 rowan     (1000) rowan     (1000)      364 2023-07-25 12:57:13.000000 demo_rowan08-0.0.3/src/demo_rowan08.egg-info/SOURCES.txt
+-rw-r--r--   0 rowan     (1000) rowan     (1000)        1 2023-07-25 12:57:13.000000 demo_rowan08-0.0.3/src/demo_rowan08.egg-info/dependency_links.txt
+-rw-r--r--   0 rowan     (1000) rowan     (1000)       14 2023-07-25 12:57:13.000000 demo_rowan08-0.0.3/src/demo_rowan08.egg-info/requires.txt
+-rw-r--r--   0 rowan     (1000) rowan     (1000)       13 2023-07-25 12:57:13.000000 demo_rowan08-0.0.3/src/demo_rowan08.egg-info/top_level.txt
```

