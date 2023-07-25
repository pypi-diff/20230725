# Comparing `tmp/hgcal_state_machine-0.5.0.tar.gz` & `tmp/hgcal_state_machine-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hgcal_state_machine-0.5.0.tar", last modified: Tue Jul 25 13:20:10 2023, max compression
+gzip compressed data, was "hgcal_state_machine-0.6.0.tar", last modified: Tue Jul 25 14:03:09 2023, max compression
```

## Comparing `hgcal_state_machine-0.5.0.tar` & `hgcal_state_machine-0.6.0.tar`

### file list

```diff
@@ -1,10 +1,14 @@
-drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-07-25 13:20:10.300755 hgcal_state_machine-0.5.0/
--rw-r--r--   0 simondejean   (501) staff       (20)      144 2023-07-25 13:20:10.300651 hgcal_state_machine-0.5.0/PKG-INFO
-drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-07-25 13:20:10.300475 hgcal_state_machine-0.5.0/hgcal_state_machine.egg-info/
--rw-r--r--   0 simondejean   (501) staff       (20)      144 2023-07-25 13:20:10.000000 hgcal_state_machine-0.5.0/hgcal_state_machine.egg-info/PKG-INFO
--rw-r--r--   0 simondejean   (501) staff       (20)      222 2023-07-25 13:20:10.000000 hgcal_state_machine-0.5.0/hgcal_state_machine.egg-info/SOURCES.txt
--rw-r--r--   0 simondejean   (501) staff       (20)        1 2023-07-25 13:20:10.000000 hgcal_state_machine-0.5.0/hgcal_state_machine.egg-info/dependency_links.txt
--rw-r--r--   0 simondejean   (501) staff       (20)       12 2023-07-25 13:20:10.000000 hgcal_state_machine-0.5.0/hgcal_state_machine.egg-info/requires.txt
--rw-r--r--   0 simondejean   (501) staff       (20)        1 2023-07-25 13:20:10.000000 hgcal_state_machine-0.5.0/hgcal_state_machine.egg-info/top_level.txt
--rw-r--r--   0 simondejean   (501) staff       (20)       38 2023-07-25 13:20:10.300790 hgcal_state_machine-0.5.0/setup.cfg
--rw-r--r--   0 simondejean   (501) staff       (20)      189 2023-07-25 13:20:05.000000 hgcal_state_machine-0.5.0/setup.py
+drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-07-25 14:03:09.727002 hgcal_state_machine-0.6.0/
+-rw-r--r--   0 simondejean   (501) staff       (20)      144 2023-07-25 14:03:09.726899 hgcal_state_machine-0.6.0/PKG-INFO
+-rw-r--r--   0 simondejean   (501) staff       (20)      891 2023-07-25 13:21:51.000000 hgcal_state_machine-0.6.0/README.txt
+drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-07-25 14:03:09.726489 hgcal_state_machine-0.6.0/hgcal_state_machine.egg-info/
+-rw-r--r--   0 simondejean   (501) staff       (20)      144 2023-07-25 14:03:09.000000 hgcal_state_machine-0.6.0/hgcal_state_machine.egg-info/PKG-INFO
+-rw-r--r--   0 simondejean   (501) staff       (20)      300 2023-07-25 14:03:09.000000 hgcal_state_machine-0.6.0/hgcal_state_machine.egg-info/SOURCES.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)        1 2023-07-25 14:03:09.000000 hgcal_state_machine-0.6.0/hgcal_state_machine.egg-info/dependency_links.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)       12 2023-07-25 14:03:09.000000 hgcal_state_machine-0.6.0/hgcal_state_machine.egg-info/requires.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)       14 2023-07-25 14:03:09.000000 hgcal_state_machine-0.6.0/hgcal_state_machine.egg-info/top_level.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)       38 2023-07-25 14:03:09.727046 hgcal_state_machine-0.6.0/setup.cfg
+-rw-r--r--   0 simondejean   (501) staff       (20)      191 2023-07-25 14:02:59.000000 hgcal_state_machine-0.6.0/setup_s_m.py
+drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-07-25 14:03:09.726730 hgcal_state_machine-0.6.0/state_machine/
+-rw-r--r--   0 simondejean   (501) staff       (20)        0 2023-07-24 13:26:39.000000 hgcal_state_machine-0.6.0/state_machine/__init__.py
+-rw-r--r--   0 simondejean   (501) staff       (20)     3980 2023-07-25 13:03:27.000000 hgcal_state_machine-0.6.0/state_machine/hgcal_state_machine.py
```

