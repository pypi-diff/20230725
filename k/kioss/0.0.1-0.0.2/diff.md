# Comparing `tmp/kioss-0.0.1.tar.gz` & `tmp/kioss-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kioss-0.0.1.tar", last modified: Tue Jul 25 15:50:41 2023, max compression
+gzip compressed data, was "kioss-0.0.2.tar", last modified: Tue Jul 25 15:55:44 2023, max compression
```

## Comparing `kioss-0.0.1.tar` & `kioss-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:50:41.419477 kioss-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 15:50:29.000000 kioss-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-25 15:50:41.419477 kioss-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-25 15:50:29.000000 kioss-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:50:41.415477 kioss-0.0.1/kioss/
--rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-07-25 15:50:29.000000 kioss-0.0.1/kioss/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-25 15:50:29.000000 kioss-0.0.1/kioss/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:50:41.419477 kioss-0.0.1/kioss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-25 15:50:41.000000 kioss-0.0.1/kioss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-25 15:50:41.000000 kioss-0.0.1/kioss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 15:50:41.000000 kioss-0.0.1/kioss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 15:50:41.000000 kioss-0.0.1/kioss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 15:50:41.419477 kioss-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-25 15:50:29.000000 kioss-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:50:41.419477 kioss-0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-07-25 15:50:29.000000 kioss-0.0.1/test/test_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-25 15:50:29.000000 kioss-0.0.1/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:55:44.270475 kioss-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 15:55:29.000000 kioss-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-25 15:55:44.270475 kioss-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-25 15:55:29.000000 kioss-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:55:44.270475 kioss-0.0.2/kioss/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-25 15:55:29.000000 kioss-0.0.2/kioss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-07-25 15:55:29.000000 kioss-0.0.2/kioss/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-25 15:55:29.000000 kioss-0.0.2/kioss/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:55:44.270475 kioss-0.0.2/kioss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-25 15:55:44.000000 kioss-0.0.2/kioss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-25 15:55:44.000000 kioss-0.0.2/kioss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 15:55:44.000000 kioss-0.0.2/kioss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 15:55:44.000000 kioss-0.0.2/kioss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 15:55:44.270475 kioss-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-25 15:55:29.000000 kioss-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:55:44.270475 kioss-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-07-25 15:55:29.000000 kioss-0.0.2/test/test_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-25 15:55:29.000000 kioss-0.0.2/test/test_util.py
```

### Comparing `kioss-0.0.1/LICENSE` & `kioss-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kioss-0.0.1/README.md` & `kioss-0.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -18,23 +18,23 @@
     .explode()
     .map(lambda _: 1)
     .reduce(int.__add__)
 )
 ```
 
 ## Features
-- `.slow` a pipe to limit the iteration's speed over it to a given `freq`
+- `.slow` a pipe to limit the iteration's speed over it
 - `.catch` any pipe's error to treat it after iteration
 - `.batch` pipe's elements and yield them as lists of a given max size or spanning over a given max period.
 - `.map` over pipe's elements uing multiple threads
 - `.merge` several pipes to form a new one that yields elements using multiple threads
 - `.log` a pipe's iteration status
 - `.list` a pipe to collect its output into a list having an optional max size
-- `reduce` a pipe
-- `filter` a pipe
+- `.reduce` a pipe
+- `.filter` a pipe
 
 
 ## Setup
 
 ```bash
 python -m venv .venv
 source ./.venv/bin/activate
```

### Comparing `kioss-0.0.1/kioss/pipe.py` & `kioss-0.0.2/kioss/pipe.py`

 * *Files identical despite different names*

### Comparing `kioss-0.0.1/test/test_pipe.py` & `kioss-0.0.2/test/test_pipe.py`

 * *Files identical despite different names*

