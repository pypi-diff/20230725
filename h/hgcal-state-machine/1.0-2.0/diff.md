# Comparing `tmp/hgcal_state_machine-1.0.tar.gz` & `tmp/hgcal_state_machine-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hgcal_state_machine-1.0.tar", last modified: Tue Jul 25 14:39:43 2023, max compression
+gzip compressed data, was "hgcal_state_machine-2.0.tar", last modified: Tue Jul 25 14:50:38 2023, max compression
```

## Comparing `hgcal_state_machine-1.0.tar` & `hgcal_state_machine-2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-07-25 14:39:43.139547 hgcal_state_machine-1.0/
--rw-r--r--   0 simondejean   (501) staff       (20)      142 2023-07-25 14:39:43.139450 hgcal_state_machine-1.0/PKG-INFO
-drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-07-25 14:39:43.139294 hgcal_state_machine-1.0/hgcal_state_machine.egg-info/
--rw-r--r--   0 simondejean   (501) staff       (20)      142 2023-07-25 14:39:43.000000 hgcal_state_machine-1.0/hgcal_state_machine.egg-info/PKG-INFO
--rw-r--r--   0 simondejean   (501) staff       (20)      222 2023-07-25 14:39:43.000000 hgcal_state_machine-1.0/hgcal_state_machine.egg-info/SOURCES.txt
--rw-r--r--   0 simondejean   (501) staff       (20)        1 2023-07-25 14:39:43.000000 hgcal_state_machine-1.0/hgcal_state_machine.egg-info/dependency_links.txt
--rw-r--r--   0 simondejean   (501) staff       (20)       12 2023-07-25 14:39:43.000000 hgcal_state_machine-1.0/hgcal_state_machine.egg-info/requires.txt
--rw-r--r--   0 simondejean   (501) staff       (20)        1 2023-07-25 14:39:43.000000 hgcal_state_machine-1.0/hgcal_state_machine.egg-info/top_level.txt
--rw-r--r--   0 simondejean   (501) staff       (20)       38 2023-07-25 14:39:43.139582 hgcal_state_machine-1.0/setup.cfg
--rw-r--r--   0 simondejean   (501) staff       (20)      187 2023-07-25 14:39:22.000000 hgcal_state_machine-1.0/setup.py
+drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-07-25 14:50:38.723203 hgcal_state_machine-2.0/
+-rw-r--r--   0 simondejean   (501) staff       (20)      142 2023-07-25 14:50:38.723098 hgcal_state_machine-2.0/PKG-INFO
+drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-07-25 14:50:38.722934 hgcal_state_machine-2.0/hgcal_state_machine.egg-info/
+-rw-r--r--   0 simondejean   (501) staff       (20)      142 2023-07-25 14:50:38.000000 hgcal_state_machine-2.0/hgcal_state_machine.egg-info/PKG-INFO
+-rw-r--r--   0 simondejean   (501) staff       (20)      222 2023-07-25 14:50:38.000000 hgcal_state_machine-2.0/hgcal_state_machine.egg-info/SOURCES.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)        1 2023-07-25 14:50:38.000000 hgcal_state_machine-2.0/hgcal_state_machine.egg-info/dependency_links.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)       12 2023-07-25 14:50:38.000000 hgcal_state_machine-2.0/hgcal_state_machine.egg-info/requires.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)        1 2023-07-25 14:50:38.000000 hgcal_state_machine-2.0/hgcal_state_machine.egg-info/top_level.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)       38 2023-07-25 14:50:38.723240 hgcal_state_machine-2.0/setup.cfg
+-rw-r--r--   0 simondejean   (501) staff       (20)      217 2023-07-25 14:50:26.000000 hgcal_state_machine-2.0/setup.py
```

