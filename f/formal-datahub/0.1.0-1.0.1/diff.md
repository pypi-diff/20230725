# Comparing `tmp/formal-datahub-0.1.0.tar.gz` & `tmp/formal-datahub-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formal-datahub-0.1.0.tar", last modified: Tue Nov  8 00:02:51 2022, max compression
+gzip compressed data, was "formal-datahub-1.0.1.tar", last modified: Mon Jul 24 23:16:05 2023, max compression
```

## Comparing `formal-datahub-0.1.0.tar` & `formal-datahub-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 junyin     (501) staff       (20)        0 2022-11-08 00:02:51.232240 formal-datahub-0.1.0/
--rw-r--r--   0 junyin     (501) staff       (20)     1073 2022-07-09 20:24:59.000000 formal-datahub-0.1.0/LICENSE
--rw-r--r--   0 junyin     (501) staff       (20)     2341 2022-11-08 00:02:51.232094 formal-datahub-0.1.0/PKG-INFO
--rw-r--r--   0 junyin     (501) staff       (20)      683 2022-11-08 00:00:41.000000 formal-datahub-0.1.0/README.md
--rw-r--r--   0 junyin     (501) staff       (20)      542 2022-11-08 00:02:38.000000 formal-datahub-0.1.0/pyproject.toml
--rw-r--r--   0 junyin     (501) staff       (20)       38 2022-11-08 00:02:51.232288 formal-datahub-0.1.0/setup.cfg
-drwxr-xr-x   0 junyin     (501) staff       (20)        0 2022-11-08 00:02:51.230420 formal-datahub-0.1.0/src/
-drwxr-xr-x   0 junyin     (501) staff       (20)        0 2022-11-08 00:02:51.231416 formal-datahub-0.1.0/src/formal-datahub/
--rw-r--r--   0 junyin     (501) staff       (20)        0 2022-07-09 20:21:32.000000 formal-datahub-0.1.0/src/formal-datahub/__init__.py
--rw-r--r--   0 junyin     (501) staff       (20)     2265 2022-07-14 15:19:46.000000 formal-datahub-0.1.0/src/formal-datahub/action.py
--rw-r--r--   0 junyin     (501) staff       (20)     8666 2022-11-08 00:00:41.000000 formal-datahub-0.1.0/src/formal-datahub/formal.py
-drwxr-xr-x   0 junyin     (501) staff       (20)        0 2022-11-08 00:02:51.231892 formal-datahub-0.1.0/src/formal_datahub.egg-info/
--rw-r--r--   0 junyin     (501) staff       (20)     2341 2022-11-08 00:02:51.000000 formal-datahub-0.1.0/src/formal_datahub.egg-info/PKG-INFO
--rw-r--r--   0 junyin     (501) staff       (20)      289 2022-11-08 00:02:51.000000 formal-datahub-0.1.0/src/formal_datahub.egg-info/SOURCES.txt
--rw-r--r--   0 junyin     (501) staff       (20)        1 2022-11-08 00:02:51.000000 formal-datahub-0.1.0/src/formal_datahub.egg-info/dependency_links.txt
--rw-r--r--   0 junyin     (501) staff       (20)       15 2022-11-08 00:02:51.000000 formal-datahub-0.1.0/src/formal_datahub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 23:16:05.254939 formal-datahub-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-24 23:15:54.000000 formal-datahub-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-24 23:16:05.254939 formal-datahub-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-24 23:15:54.000000 formal-datahub-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-24 23:15:54.000000 formal-datahub-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 23:16:05.254939 formal-datahub-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 23:16:05.254939 formal-datahub-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 23:16:05.254939 formal-datahub-1.0.1/src/formal-datahub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 23:15:54.000000 formal-datahub-1.0.1/src/formal-datahub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-24 23:15:54.000000 formal-datahub-1.0.1/src/formal-datahub/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-07-24 23:15:54.000000 formal-datahub-1.0.1/src/formal-datahub/formal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 23:16:05.254939 formal-datahub-1.0.1/src/formal_datahub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-24 23:16:05.000000 formal-datahub-1.0.1/src/formal_datahub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-24 23:16:05.000000 formal-datahub-1.0.1/src/formal_datahub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 23:16:05.000000 formal-datahub-1.0.1/src/formal_datahub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-24 23:16:05.000000 formal-datahub-1.0.1/src/formal_datahub.egg-info/top_level.txt
```

### Comparing `formal-datahub-0.1.0/LICENSE` & `formal-datahub-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `formal-datahub-0.1.0/PKG-INFO` & `formal-datahub-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formal-datahub
-Version: 0.1.0
+Version: 1.0.1
 Summary: Formal Datahub Plugin
 Author-email: Formal <hello@joinformal.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `formal-datahub-0.1.0/README.md` & `formal-datahub-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `formal-datahub-0.1.0/pyproject.toml` & `formal-datahub-1.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "formal-datahub"
-version = "0.1.00"
+version = "1.0.1"
 authors = [
   { name="Formal", email="hello@joinformal.com" },
 ]
 description = "Formal Datahub Plugin"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `formal-datahub-0.1.0/src/formal-datahub/formal.py` & `formal-datahub-1.0.1/src/formal-datahub/formal.py`

 * *Files identical despite different names*

### Comparing `formal-datahub-0.1.0/src/formal_datahub.egg-info/PKG-INFO` & `formal-datahub-1.0.1/src/formal_datahub.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formal-datahub
-Version: 0.1.0
+Version: 1.0.1
 Summary: Formal Datahub Plugin
 Author-email: Formal <hello@joinformal.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

