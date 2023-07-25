# Comparing `tmp/promptz-0.0.2.tar.gz` & `tmp/promptz-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptz-0.0.2.tar", last modified: Tue Jul 25 16:10:19 2023, max compression
+gzip compressed data, was "promptz-0.0.3.tar", last modified: Tue Jul 25 16:15:07 2023, max compression
```

## Comparing `promptz-0.0.2.tar` & `promptz-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-25 16:10:19.205643 promptz-0.0.2/
--rw-r--r--   0 rjl       (1000) rjl       (1000)      165 2023-07-25 16:10:19.205643 promptz-0.0.2/PKG-INFO
--rw-r--r--   0 rjl       (1000) rjl       (1000)    14608 2023-07-25 15:57:54.000000 promptz-0.0.2/README.md
-drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-25 16:10:19.205643 promptz-0.0.2/promptz/
--rw-r--r--   0 rjl       (1000) rjl       (1000)    43438 2023-07-25 16:05:27.000000 promptz-0.0.2/promptz/__init__.py
--rw-r--r--   0 rjl       (1000) rjl       (1000)      151 2023-05-17 11:33:35.000000 promptz-0.0.2/promptz/main.py
-drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-25 16:10:19.205643 promptz-0.0.2/promptz.egg-info/
--rw-r--r--   0 rjl       (1000) rjl       (1000)      165 2023-07-25 16:10:19.000000 promptz-0.0.2/promptz.egg-info/PKG-INFO
--rw-r--r--   0 rjl       (1000) rjl       (1000)      178 2023-07-25 16:10:19.000000 promptz-0.0.2/promptz.egg-info/SOURCES.txt
--rw-r--r--   0 rjl       (1000) rjl       (1000)        1 2023-07-25 16:10:19.000000 promptz-0.0.2/promptz.egg-info/dependency_links.txt
--rw-r--r--   0 rjl       (1000) rjl       (1000)        8 2023-07-25 16:10:19.000000 promptz-0.0.2/promptz.egg-info/top_level.txt
--rw-r--r--   0 rjl       (1000) rjl       (1000)       38 2023-07-25 16:10:19.205643 promptz-0.0.2/setup.cfg
--rw-r--r--   0 rjl       (1000) rjl       (1000)      165 2023-07-25 16:09:55.000000 promptz-0.0.2/setup.py
+drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-25 16:15:07.398233 promptz-0.0.3/
+-rw-r--r--   0 rjl       (1000) rjl       (1000)      165 2023-07-25 16:15:07.398233 promptz-0.0.3/PKG-INFO
+-rw-r--r--   0 rjl       (1000) rjl       (1000)    14608 2023-07-25 15:57:54.000000 promptz-0.0.3/README.md
+drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-25 16:15:07.398233 promptz-0.0.3/promptz/
+-rw-r--r--   0 rjl       (1000) rjl       (1000)    43438 2023-07-25 16:05:27.000000 promptz-0.0.3/promptz/__init__.py
+-rw-r--r--   0 rjl       (1000) rjl       (1000)      151 2023-05-17 11:33:35.000000 promptz-0.0.3/promptz/main.py
+drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-25 16:15:07.398233 promptz-0.0.3/promptz.egg-info/
+-rw-r--r--   0 rjl       (1000) rjl       (1000)      165 2023-07-25 16:15:07.000000 promptz-0.0.3/promptz.egg-info/PKG-INFO
+-rw-r--r--   0 rjl       (1000) rjl       (1000)      178 2023-07-25 16:15:07.000000 promptz-0.0.3/promptz.egg-info/SOURCES.txt
+-rw-r--r--   0 rjl       (1000) rjl       (1000)        1 2023-07-25 16:15:07.000000 promptz-0.0.3/promptz.egg-info/dependency_links.txt
+-rw-r--r--   0 rjl       (1000) rjl       (1000)        8 2023-07-25 16:15:07.000000 promptz-0.0.3/promptz.egg-info/top_level.txt
+-rw-r--r--   0 rjl       (1000) rjl       (1000)       38 2023-07-25 16:15:07.398233 promptz-0.0.3/setup.cfg
+-rw-r--r--   0 rjl       (1000) rjl       (1000)      165 2023-07-25 16:14:54.000000 promptz-0.0.3/setup.py
```

### Comparing `promptz-0.0.2/README.md` & `promptz-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `promptz-0.0.2/promptz/__init__.py` & `promptz-0.0.3/promptz/__init__.py`

 * *Files identical despite different names*

