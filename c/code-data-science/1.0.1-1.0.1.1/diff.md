# Comparing `tmp/code_data_science-1.0.1.tar.gz` & `tmp/code_data_science-1.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_data_science-1.0.1.tar", last modified: Thu Feb  9 19:28:29 2023, max compression
+gzip compressed data, was "code_data_science-1.0.1.1.tar", last modified: Tue Jul 25 01:56:28 2023, max compression
```

## Comparing `code_data_science-1.0.1.tar` & `code_data_science-1.0.1.1.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 19:28:29.950823 code_data_science-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-02-09 19:28:29.950823 code_data_science-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-02-09 19:28:13.000000 code_data_science-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 19:28:29.950823 code_data_science-1.0.1/code_data_science/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 19:28:13.000000 code_data_science-1.0.1/code_data_science/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-02-09 19:28:13.000000 code_data_science-1.0.1/code_data_science/index_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-02-09 19:28:13.000000 code_data_science-1.0.1/code_data_science/sort_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 19:28:29.950823 code_data_science-1.0.1/code_data_science.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-02-09 19:28:29.000000 code_data_science-1.0.1/code_data_science.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-02-09 19:28:29.000000 code_data_science-1.0.1/code_data_science.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 19:28:29.000000 code_data_science-1.0.1/code_data_science.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-09 19:28:29.000000 code_data_science-1.0.1/code_data_science.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 19:28:29.950823 code_data_science-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-02-09 19:28:13.000000 code_data_science-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:56:28.420926 code_data_science-1.0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-25 01:56:28.420926 code_data_science-1.0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-25 01:56:08.000000 code_data_science-1.0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:56:28.416926 code_data_science-1.0.1.1/code_data_science/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 01:56:08.000000 code_data_science-1.0.1.1/code_data_science/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-25 01:56:08.000000 code_data_science-1.0.1.1/code_data_science/index_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-25 01:56:08.000000 code_data_science-1.0.1.1/code_data_science/moderne_data_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-25 01:56:08.000000 code_data_science-1.0.1.1/code_data_science/moderne_palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-25 01:56:08.000000 code_data_science-1.0.1.1/code_data_science/scm_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-07-25 01:56:08.000000 code_data_science-1.0.1.1/code_data_science/sort_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:56:28.420926 code_data_science-1.0.1.1/code_data_science.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-25 01:56:28.000000 code_data_science-1.0.1.1/code_data_science.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-25 01:56:28.000000 code_data_science-1.0.1.1/code_data_science.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 01:56:28.000000 code_data_science-1.0.1.1/code_data_science.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-25 01:56:28.000000 code_data_science-1.0.1.1/code_data_science.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-25 01:56:28.000000 code_data_science-1.0.1.1/code_data_science.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-25 01:56:08.000000 code_data_science-1.0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 01:56:28.420926 code_data_science-1.0.1.1/setup.cfg
```

### Comparing `code_data_science-1.0.1/code_data_science/sort_versions.py` & `code_data_science-1.0.1.1/code_data_science/sort_versions.py`

 * *Files identical despite different names*

