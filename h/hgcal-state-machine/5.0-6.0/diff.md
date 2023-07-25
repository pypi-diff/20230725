# Comparing `tmp/hgcal_state_machine-5.0.tar.gz` & `tmp/hgcal_state_machine-6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hgcal_state_machine-5.0.tar", last modified: Tue Jul 25 15:06:19 2023, max compression
+gzip compressed data, was "hgcal_state_machine-6.0.tar", last modified: Tue Jul 25 15:20:19 2023, max compression
```

## Comparing `hgcal_state_machine-5.0.tar` & `hgcal_state_machine-6.0.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-07-25 15:06:19.106737 hgcal_state_machine-5.0/
--rw-r--r--   0 simondejean   (501) staff       (20)      142 2023-07-25 15:06:19.106635 hgcal_state_machine-5.0/PKG-INFO
-drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-07-25 15:06:19.106477 hgcal_state_machine-5.0/hgcal_state_machine.egg-info/
--rw-r--r--   0 simondejean   (501) staff       (20)      142 2023-07-25 15:06:19.000000 hgcal_state_machine-5.0/hgcal_state_machine.egg-info/PKG-INFO
--rw-r--r--   0 simondejean   (501) staff       (20)      222 2023-07-25 15:06:19.000000 hgcal_state_machine-5.0/hgcal_state_machine.egg-info/SOURCES.txt
--rw-r--r--   0 simondejean   (501) staff       (20)        1 2023-07-25 15:06:19.000000 hgcal_state_machine-5.0/hgcal_state_machine.egg-info/dependency_links.txt
--rw-r--r--   0 simondejean   (501) staff       (20)       12 2023-07-25 15:06:19.000000 hgcal_state_machine-5.0/hgcal_state_machine.egg-info/requires.txt
--rw-r--r--   0 simondejean   (501) staff       (20)        1 2023-07-25 15:06:19.000000 hgcal_state_machine-5.0/hgcal_state_machine.egg-info/top_level.txt
--rw-r--r--   0 simondejean   (501) staff       (20)       38 2023-07-25 15:06:19.106774 hgcal_state_machine-5.0/setup.cfg
--rw-r--r--   0 simondejean   (501) staff       (20)      217 2023-07-25 15:06:14.000000 hgcal_state_machine-5.0/setup.py
+drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-07-25 15:20:19.384990 hgcal_state_machine-6.0/
+-rw-r--r--   0 simondejean   (501) staff       (20)      142 2023-07-25 15:20:19.384882 hgcal_state_machine-6.0/PKG-INFO
+drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-07-25 15:20:19.383935 hgcal_state_machine-6.0/hgcal_state_machine/
+-rw-r--r--   0 simondejean   (501) staff       (20)        1 2023-07-25 15:19:45.000000 hgcal_state_machine-6.0/hgcal_state_machine/__init__.py
+-rw-r--r--   0 simondejean   (501) staff       (20)     3980 2023-07-24 13:46:44.000000 hgcal_state_machine-6.0/hgcal_state_machine/hgcal_state_machine.py
+drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-07-25 15:20:19.384715 hgcal_state_machine-6.0/hgcal_state_machine.egg-info/
+-rw-r--r--   0 simondejean   (501) staff       (20)      142 2023-07-25 15:20:19.000000 hgcal_state_machine-6.0/hgcal_state_machine.egg-info/PKG-INFO
+-rw-r--r--   0 simondejean   (501) staff       (20)      297 2023-07-25 15:20:19.000000 hgcal_state_machine-6.0/hgcal_state_machine.egg-info/SOURCES.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)        1 2023-07-25 15:20:19.000000 hgcal_state_machine-6.0/hgcal_state_machine.egg-info/dependency_links.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)       12 2023-07-25 15:20:19.000000 hgcal_state_machine-6.0/hgcal_state_machine.egg-info/requires.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)       20 2023-07-25 15:20:19.000000 hgcal_state_machine-6.0/hgcal_state_machine.egg-info/top_level.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)       38 2023-07-25 15:20:19.385036 hgcal_state_machine-6.0/setup.cfg
+-rw-r--r--   0 simondejean   (501) staff       (20)      240 2023-07-25 15:18:59.000000 hgcal_state_machine-6.0/setup.py
```

