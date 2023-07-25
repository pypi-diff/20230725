# Comparing `tmp/hgcal_state_machine-4.0.tar.gz` & `tmp/hgcal_state_machine-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hgcal_state_machine-4.0.tar", last modified: Tue Jul 25 15:01:50 2023, max compression
+gzip compressed data, was "hgcal_state_machine-5.0.tar", last modified: Tue Jul 25 15:06:19 2023, max compression
```

## Comparing `hgcal_state_machine-4.0.tar` & `hgcal_state_machine-5.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-07-25 15:01:50.734268 hgcal_state_machine-4.0/
--rw-r--r--   0 simondejean   (501) staff       (20)      142 2023-07-25 15:01:50.734160 hgcal_state_machine-4.0/PKG-INFO
-drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-07-25 15:01:50.733973 hgcal_state_machine-4.0/hgcal_state_machine.egg-info/
--rw-r--r--   0 simondejean   (501) staff       (20)      142 2023-07-25 15:01:50.000000 hgcal_state_machine-4.0/hgcal_state_machine.egg-info/PKG-INFO
--rw-r--r--   0 simondejean   (501) staff       (20)      222 2023-07-25 15:01:50.000000 hgcal_state_machine-4.0/hgcal_state_machine.egg-info/SOURCES.txt
--rw-r--r--   0 simondejean   (501) staff       (20)        1 2023-07-25 15:01:50.000000 hgcal_state_machine-4.0/hgcal_state_machine.egg-info/dependency_links.txt
--rw-r--r--   0 simondejean   (501) staff       (20)       12 2023-07-25 15:01:50.000000 hgcal_state_machine-4.0/hgcal_state_machine.egg-info/requires.txt
--rw-r--r--   0 simondejean   (501) staff       (20)        1 2023-07-25 15:01:50.000000 hgcal_state_machine-4.0/hgcal_state_machine.egg-info/top_level.txt
--rw-r--r--   0 simondejean   (501) staff       (20)       38 2023-07-25 15:01:50.734308 hgcal_state_machine-4.0/setup.cfg
--rw-r--r--   0 simondejean   (501) staff       (20)      217 2023-07-25 15:01:30.000000 hgcal_state_machine-4.0/setup.py
+drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-07-25 15:06:19.106737 hgcal_state_machine-5.0/
+-rw-r--r--   0 simondejean   (501) staff       (20)      142 2023-07-25 15:06:19.106635 hgcal_state_machine-5.0/PKG-INFO
+drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-07-25 15:06:19.106477 hgcal_state_machine-5.0/hgcal_state_machine.egg-info/
+-rw-r--r--   0 simondejean   (501) staff       (20)      142 2023-07-25 15:06:19.000000 hgcal_state_machine-5.0/hgcal_state_machine.egg-info/PKG-INFO
+-rw-r--r--   0 simondejean   (501) staff       (20)      222 2023-07-25 15:06:19.000000 hgcal_state_machine-5.0/hgcal_state_machine.egg-info/SOURCES.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)        1 2023-07-25 15:06:19.000000 hgcal_state_machine-5.0/hgcal_state_machine.egg-info/dependency_links.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)       12 2023-07-25 15:06:19.000000 hgcal_state_machine-5.0/hgcal_state_machine.egg-info/requires.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)        1 2023-07-25 15:06:19.000000 hgcal_state_machine-5.0/hgcal_state_machine.egg-info/top_level.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)       38 2023-07-25 15:06:19.106774 hgcal_state_machine-5.0/setup.cfg
+-rw-r--r--   0 simondejean   (501) staff       (20)      217 2023-07-25 15:06:14.000000 hgcal_state_machine-5.0/setup.py
```

