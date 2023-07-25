# Comparing `tmp/aioevents-0.1.tar.gz` & `tmp/aioevents-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aioevents-0.1.tar", last modified: Sun Feb 23 03:59:21 2014, max compression
+gzip compressed data, was "aioevents-0.2.tar", max compression
```

## Comparing `aioevents-0.1.tar` & `aioevents-0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
-drwxr-xr-x   0 astronouth7303  (1000) astronouth7303  (1000)        0 2014-02-23 03:59:21.000000 aioevents-0.1/
--rw-r--r--   0 astronouth7303  (1000) astronouth7303  (1000)      767 2014-02-23 03:59:21.000000 aioevents-0.1/PKG-INFO
-drwxr-xr-x   0 astronouth7303  (1000) astronouth7303  (1000)        0 2014-02-23 03:59:21.000000 aioevents-0.1/aioevents/
--rw-r--r--   0 astronouth7303  (1000) astronouth7303  (1000)     3502 2014-02-22 04:56:33.000000 aioevents-0.1/aioevents/__init__.py
--rw-r--r--   0 astronouth7303  (1000) astronouth7303  (1000)     1125 2014-02-23 03:55:21.000000 aioevents-0.1/setup.py
+-rw-r--r--   0        0        0     1078 2023-07-25 18:00:32.755667 aioevents-0.2/LICENSE
+-rw-r--r--   0        0        0      377 2023-07-25 18:00:32.755667 aioevents-0.2/README.md
+-rw-r--r--   0        0        0     4239 2023-07-25 18:00:32.755667 aioevents-0.2/aioevents/__init__.py
+-rw-r--r--   0        0        0      923 2023-07-25 18:00:32.755667 aioevents-0.2/pyproject.toml
+-rw-r--r--   0        0        0      917 1970-01-01 00:00:00.000000 aioevents-0.2/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

