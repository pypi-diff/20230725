# Comparing `tmp/hgcal_swamp-0.2.0.tar.gz` & `tmp/hgcal_swamp-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hgcal_swamp-0.2.0.tar", last modified: Tue Jul 25 14:23:07 2023, max compression
+gzip compressed data, was "hgcal_swamp-0.3.0.tar", last modified: Tue Jul 25 14:26:15 2023, max compression
```

## Comparing `hgcal_swamp-0.2.0.tar` & `hgcal_swamp-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-07-25 14:23:07.222673 hgcal_swamp-0.2.0/
--rw-r--r--   0 simondejean   (501) staff       (20)      136 2023-07-25 14:23:07.222526 hgcal_swamp-0.2.0/PKG-INFO
--rw-r--r--   0 simondejean   (501) staff       (20)      154 2023-07-25 13:32:51.000000 hgcal_swamp-0.2.0/README.md
-drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-07-25 14:23:07.222370 hgcal_swamp-0.2.0/hgcal_swamp.egg-info/
--rw-r--r--   0 simondejean   (501) staff       (20)      136 2023-07-25 14:23:07.000000 hgcal_swamp-0.2.0/hgcal_swamp.egg-info/PKG-INFO
--rw-r--r--   0 simondejean   (501) staff       (20)      192 2023-07-25 14:23:07.000000 hgcal_swamp-0.2.0/hgcal_swamp.egg-info/SOURCES.txt
--rw-r--r--   0 simondejean   (501) staff       (20)        1 2023-07-25 14:23:07.000000 hgcal_swamp-0.2.0/hgcal_swamp.egg-info/dependency_links.txt
--rw-r--r--   0 simondejean   (501) staff       (20)       69 2023-07-25 14:23:07.000000 hgcal_swamp-0.2.0/hgcal_swamp.egg-info/requires.txt
--rw-r--r--   0 simondejean   (501) staff       (20)        1 2023-07-25 14:23:07.000000 hgcal_swamp-0.2.0/hgcal_swamp.egg-info/top_level.txt
--rw-r--r--   0 simondejean   (501) staff       (20)       38 2023-07-25 14:23:07.222708 hgcal_swamp-0.2.0/setup.cfg
--rw-r--r--   0 simondejean   (501) staff       (20)      261 2023-07-25 14:23:04.000000 hgcal_swamp-0.2.0/setup.py
+drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-07-25 14:26:15.414922 hgcal_swamp-0.3.0/
+-rw-r--r--   0 simondejean   (501) staff       (20)      136 2023-07-25 14:26:15.414825 hgcal_swamp-0.3.0/PKG-INFO
+-rw-r--r--   0 simondejean   (501) staff       (20)      154 2023-07-25 13:32:51.000000 hgcal_swamp-0.3.0/README.md
+drwxr-xr-x   0 simondejean   (501) staff       (20)        0 2023-07-25 14:26:15.414667 hgcal_swamp-0.3.0/hgcal_swamp.egg-info/
+-rw-r--r--   0 simondejean   (501) staff       (20)      136 2023-07-25 14:26:15.000000 hgcal_swamp-0.3.0/hgcal_swamp.egg-info/PKG-INFO
+-rw-r--r--   0 simondejean   (501) staff       (20)      192 2023-07-25 14:26:15.000000 hgcal_swamp-0.3.0/hgcal_swamp.egg-info/SOURCES.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)        1 2023-07-25 14:26:15.000000 hgcal_swamp-0.3.0/hgcal_swamp.egg-info/dependency_links.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)       61 2023-07-25 14:26:15.000000 hgcal_swamp-0.3.0/hgcal_swamp.egg-info/requires.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)        1 2023-07-25 14:26:15.000000 hgcal_swamp-0.3.0/hgcal_swamp.egg-info/top_level.txt
+-rw-r--r--   0 simondejean   (501) staff       (20)       38 2023-07-25 14:26:15.414965 hgcal_swamp-0.3.0/setup.cfg
+-rw-r--r--   0 simondejean   (501) staff       (20)      250 2023-07-25 14:26:03.000000 hgcal_swamp-0.3.0/setup.py
```

