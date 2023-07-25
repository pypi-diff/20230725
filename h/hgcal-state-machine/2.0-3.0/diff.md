# Comparing `tmp/hgcal_state_machine-2.0.tar.gz` & `tmp/hgcal_state_machine-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hgcal_state_machine-2.0.tar", last modified: Tue Jul 25 14:50:38 2023, max compression
+gzip compressed data, was "hgcal_state_machine-3.0.tar", last modified: Tue Jul 25 14:54:16 2023, max compression
```

## Comparing `hgcal_state_machine-2.0.tar` & `hgcal_state_machine-3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-07-25 14:50:38.723203 hgcal_state_machine-2.0/
--rw-r--r--   0 simondejean   (501) staff       (20)      142 2023-07-25 14:50:38.723098 hgcal_state_machine-2.0/PKG-INFO
-drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-07-25 14:50:38.722934 hgcal_state_machine-2.0/hgcal_state_machine.egg-info/
--rw-r--r--   0 simondejean   (501) staff       (20)      142 2023-07-25 14:50:38.000000 hgcal_state_machine-2.0/hgcal_state_machine.egg-info/PKG-INFO
--rw-r--r--   0 simondejean   (501) staff       (20)      222 2023-07-25 14:50:38.000000 hgcal_state_machine-2.0/hgcal_state_machine.egg-info/SOURCES.txt
--rw-r--r--   0 simondejean   (501) staff       (20)        1 2023-07-25 14:50:38.000000 hgcal_state_machine-2.0/hgcal_state_machine.egg-info/dependency_links.txt
--rw-r--r--   0 simondejean   (501) staff       (20)       12 2023-07-25 14:50:38.000000 hgcal_state_machine-2.0/hgcal_state_machine.egg-info/requires.txt
--rw-r--r--   0 simondejean   (501) staff       (20)        1 2023-07-25 14:50:38.000000 hgcal_state_machine-2.0/hgcal_state_machine.egg-info/top_level.txt
--rw-r--r--   0 simondejean   (501) staff       (20)       38 2023-07-25 14:50:38.723240 hgcal_state_machine-2.0/setup.cfg
--rw-r--r--   0 simondejean   (501) staff       (20)      217 2023-07-25 14:50:26.000000 hgcal_state_machine-2.0/setup.py
+drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-07-25 14:54:16.587062 hgcal_state_machine-3.0/
+-rw-r--r--   0 simondejean   (501) staff       (20)      142 2023-07-25 14:54:16.586945 hgcal_state_machine-3.0/PKG-INFO
+drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-07-25 14:54:16.586784 hgcal_state_machine-3.0/hgcal_state_machine.egg-info/
+-rw-r--r--   0 simondejean   (501) staff       (20)      142 2023-07-25 14:54:16.000000 hgcal_state_machine-3.0/hgcal_state_machine.egg-info/PKG-INFO
+-rw-r--r--   0 simondejean   (501) staff       (20)      222 2023-07-25 14:54:16.000000 hgcal_state_machine-3.0/hgcal_state_machine.egg-info/SOURCES.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)        1 2023-07-25 14:54:16.000000 hgcal_state_machine-3.0/hgcal_state_machine.egg-info/dependency_links.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)       12 2023-07-25 14:54:16.000000 hgcal_state_machine-3.0/hgcal_state_machine.egg-info/requires.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)        1 2023-07-25 14:54:16.000000 hgcal_state_machine-3.0/hgcal_state_machine.egg-info/top_level.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)       38 2023-07-25 14:54:16.587103 hgcal_state_machine-3.0/setup.cfg
+-rw-r--r--   0 simondejean   (501) staff       (20)      217 2023-07-25 14:53:54.000000 hgcal_state_machine-3.0/setup.py
```

