# Comparing `tmp/promptz-0.0.5.tar.gz` & `tmp/promptz-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptz-0.0.5.tar", last modified: Tue Jul 25 16:20:55 2023, max compression
+gzip compressed data, was "promptz-0.0.6.tar", last modified: Tue Jul 25 16:23:18 2023, max compression
```

## Comparing `promptz-0.0.5.tar` & `promptz-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-25 16:20:55.601021 promptz-0.0.5/
--rw-r--r--   0 rjl       (1000) rjl       (1000)      165 2023-07-25 16:20:55.601021 promptz-0.0.5/PKG-INFO
--rw-r--r--   0 rjl       (1000) rjl       (1000)    14608 2023-07-25 15:57:54.000000 promptz-0.0.5/README.md
-drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-25 16:20:55.601021 promptz-0.0.5/promptz/
--rw-r--r--   0 rjl       (1000) rjl       (1000)    40171 2023-07-25 16:20:12.000000 promptz-0.0.5/promptz/__init__.py
--rw-r--r--   0 rjl       (1000) rjl       (1000)      151 2023-05-17 11:33:35.000000 promptz-0.0.5/promptz/main.py
-drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-25 16:20:55.601021 promptz-0.0.5/promptz.egg-info/
--rw-r--r--   0 rjl       (1000) rjl       (1000)      165 2023-07-25 16:20:55.000000 promptz-0.0.5/promptz.egg-info/PKG-INFO
--rw-r--r--   0 rjl       (1000) rjl       (1000)      178 2023-07-25 16:20:55.000000 promptz-0.0.5/promptz.egg-info/SOURCES.txt
--rw-r--r--   0 rjl       (1000) rjl       (1000)        1 2023-07-25 16:20:55.000000 promptz-0.0.5/promptz.egg-info/dependency_links.txt
--rw-r--r--   0 rjl       (1000) rjl       (1000)        8 2023-07-25 16:20:55.000000 promptz-0.0.5/promptz.egg-info/top_level.txt
--rw-r--r--   0 rjl       (1000) rjl       (1000)       38 2023-07-25 16:20:55.601021 promptz-0.0.5/setup.cfg
--rw-r--r--   0 rjl       (1000) rjl       (1000)      165 2023-07-25 16:20:37.000000 promptz-0.0.5/setup.py
+drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-25 16:23:18.126548 promptz-0.0.6/
+-rw-r--r--   0 rjl       (1000) rjl       (1000)      165 2023-07-25 16:23:18.126548 promptz-0.0.6/PKG-INFO
+-rw-r--r--   0 rjl       (1000) rjl       (1000)    14608 2023-07-25 15:57:54.000000 promptz-0.0.6/README.md
+drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-25 16:23:18.126548 promptz-0.0.6/promptz/
+-rw-r--r--   0 rjl       (1000) rjl       (1000)    40171 2023-07-25 16:20:12.000000 promptz-0.0.6/promptz/__init__.py
+-rw-r--r--   0 rjl       (1000) rjl       (1000)      151 2023-05-17 11:33:35.000000 promptz-0.0.6/promptz/main.py
+drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-25 16:23:18.126548 promptz-0.0.6/promptz.egg-info/
+-rw-r--r--   0 rjl       (1000) rjl       (1000)      165 2023-07-25 16:23:18.000000 promptz-0.0.6/promptz.egg-info/PKG-INFO
+-rw-r--r--   0 rjl       (1000) rjl       (1000)      208 2023-07-25 16:23:18.000000 promptz-0.0.6/promptz.egg-info/SOURCES.txt
+-rw-r--r--   0 rjl       (1000) rjl       (1000)        1 2023-07-25 16:23:18.000000 promptz-0.0.6/promptz.egg-info/dependency_links.txt
+-rw-r--r--   0 rjl       (1000) rjl       (1000)     2122 2023-07-25 16:23:18.000000 promptz-0.0.6/promptz.egg-info/requires.txt
+-rw-r--r--   0 rjl       (1000) rjl       (1000)        8 2023-07-25 16:23:18.000000 promptz-0.0.6/promptz.egg-info/top_level.txt
+-rw-r--r--   0 rjl       (1000) rjl       (1000)       38 2023-07-25 16:23:18.126548 promptz-0.0.6/setup.cfg
+-rw-r--r--   0 rjl       (1000) rjl       (1000)      278 2023-07-25 16:23:00.000000 promptz-0.0.6/setup.py
```

### Comparing `promptz-0.0.5/README.md` & `promptz-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `promptz-0.0.5/promptz/__init__.py` & `promptz-0.0.6/promptz/__init__.py`

 * *Files identical despite different names*

