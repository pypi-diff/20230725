# Comparing `tmp/baam-0.0.1.tar.gz` & `tmp/baam-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baam-0.0.1.tar", last modified: Tue Jul 25 15:08:25 2023, max compression
+gzip compressed data, was "baam-0.0.2.tar", last modified: Tue Jul 25 15:16:54 2023, max compression
```

## Comparing `baam-0.0.1.tar` & `baam-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-07-25 15:08:25.340044 baam-0.0.1/
--rw-r--r--   0 pedro      (503) staff       (20)      911 2023-07-25 15:08:25.339886 baam-0.0.1/PKG-INFO
--rw-r--r--   0 pedro      (503) staff       (20)      331 2023-07-25 15:03:15.000000 baam-0.0.1/README.md
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-07-25 15:08:25.338575 baam-0.0.1/baam/
--rw-r--r--   0 pedro      (503) staff       (20)       18 2023-07-25 14:18:40.000000 baam-0.0.1/baam/__init__.py
--rw-r--r--   0 pedro      (503) staff       (20)      101 2023-07-25 15:00:06.000000 baam-0.0.1/baam/cli.py
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-07-25 15:08:25.339415 baam-0.0.1/baam.egg-info/
--rw-r--r--   0 pedro      (503) staff       (20)      911 2023-07-25 15:08:25.000000 baam-0.0.1/baam.egg-info/PKG-INFO
--rw-r--r--   0 pedro      (503) staff       (20)      234 2023-07-25 15:08:25.000000 baam-0.0.1/baam.egg-info/SOURCES.txt
--rw-r--r--   0 pedro      (503) staff       (20)        1 2023-07-25 15:08:25.000000 baam-0.0.1/baam.egg-info/dependency_links.txt
--rw-r--r--   0 pedro      (503) staff       (20)       39 2023-07-25 15:08:25.000000 baam-0.0.1/baam.egg-info/entry_points.txt
--rw-r--r--   0 pedro      (503) staff       (20)        7 2023-07-25 15:08:25.000000 baam-0.0.1/baam.egg-info/requires.txt
--rw-r--r--   0 pedro      (503) staff       (20)        5 2023-07-25 15:08:25.000000 baam-0.0.1/baam.egg-info/top_level.txt
--rw-r--r--   0 pedro      (503) staff       (20)       38 2023-07-25 15:08:25.340095 baam-0.0.1/setup.cfg
--rw-r--r--   0 pedro      (503) staff       (20)      998 2023-07-25 15:03:22.000000 baam-0.0.1/setup.py
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-07-25 15:08:25.339642 baam-0.0.1/test/
--rw-r--r--   0 pedro      (503) staff       (20)       73 2023-07-25 15:00:02.000000 baam-0.0.1/test/test_cli.py
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-07-25 15:16:54.195754 baam-0.0.2/
+-rw-r--r--   0 pedro      (503) staff       (20)      906 2023-07-25 15:16:54.195645 baam-0.0.2/PKG-INFO
+-rw-r--r--   0 pedro      (503) staff       (20)      325 2023-07-25 15:15:02.000000 baam-0.0.2/README.md
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-07-25 15:16:54.194436 baam-0.0.2/baam/
+-rw-r--r--   0 pedro      (503) staff       (20)       18 2023-07-25 15:15:59.000000 baam-0.0.2/baam/__init__.py
+-rw-r--r--   0 pedro      (503) staff       (20)      101 2023-07-25 15:00:06.000000 baam-0.0.2/baam/cli.py
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-07-25 15:16:54.195332 baam-0.0.2/baam.egg-info/
+-rw-r--r--   0 pedro      (503) staff       (20)      906 2023-07-25 15:16:54.000000 baam-0.0.2/baam.egg-info/PKG-INFO
+-rw-r--r--   0 pedro      (503) staff       (20)      234 2023-07-25 15:16:54.000000 baam-0.0.2/baam.egg-info/SOURCES.txt
+-rw-r--r--   0 pedro      (503) staff       (20)        1 2023-07-25 15:16:54.000000 baam-0.0.2/baam.egg-info/dependency_links.txt
+-rw-r--r--   0 pedro      (503) staff       (20)       39 2023-07-25 15:16:54.000000 baam-0.0.2/baam.egg-info/entry_points.txt
+-rw-r--r--   0 pedro      (503) staff       (20)        7 2023-07-25 15:16:54.000000 baam-0.0.2/baam.egg-info/requires.txt
+-rw-r--r--   0 pedro      (503) staff       (20)        5 2023-07-25 15:16:54.000000 baam-0.0.2/baam.egg-info/top_level.txt
+-rw-r--r--   0 pedro      (503) staff       (20)       38 2023-07-25 15:16:54.195796 baam-0.0.2/setup.cfg
+-rw-r--r--   0 pedro      (503) staff       (20)      999 2023-07-25 15:16:15.000000 baam-0.0.2/setup.py
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-07-25 15:16:54.195466 baam-0.0.2/test/
+-rw-r--r--   0 pedro      (503) staff       (20)       73 2023-07-25 15:00:02.000000 baam-0.0.2/test/test_cli.py
```

### Comparing `baam-0.0.1/setup.py` & `baam-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setup(
     name="baam",
     version=VERSION,
-    description="Deploy docker apps",
+    description="Deploys docker apps",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="jpedro",
     author_email="jpedro.barbosa@gmail.com",
     url="https://github.com/jpedro/baam",
     download_url="https://github.com/jpedro/baam/tarball/master",
     keywords="deploy docker apps",
```

