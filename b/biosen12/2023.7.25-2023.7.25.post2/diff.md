# Comparing `tmp/biosen12-2023.7.25.tar.gz` & `tmp/biosen12-2023.7.25.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biosen12-2023.7.25.tar", max compression
+gzip compressed data, was "biosen12-2023.7.25.post2.tar", max compression
```

## Comparing `biosen12-2023.7.25.tar` & `biosen12-2023.7.25.post2.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0       10 2023-07-25 12:47:29.058887 biosen12-2023.7.25/README.md
--rw-r--r--   0        0        0       80 2023-07-25 12:47:30.438884 biosen12-2023.7.25/biosen12/main.py
--rw-r--r--   0        0        0      268 2023-07-25 12:47:30.434884 biosen12-2023.7.25/pyproject.toml
--rw-r--r--   0        0        0      510 1970-01-01 00:00:00.000000 biosen12-2023.7.25/setup.py
--rw-r--r--   0        0        0      396 1970-01-01 00:00:00.000000 biosen12-2023.7.25/PKG-INFO
+-rw-r--r--   0        0        0       10 2023-07-25 12:47:29.058887 biosen12-2023.7.25.post2/README.md
+-rw-r--r--   0        0        0       24 2023-07-25 12:48:44.806760 biosen12-2023.7.25.post2/biosen12/__init__.py
+-rw-r--r--   0        0        0       82 2023-07-25 12:49:21.094715 biosen12-2023.7.25.post2/biosen12/main.py
+-rw-r--r--   0        0        0      270 2023-07-25 12:49:21.090715 biosen12-2023.7.25.post2/pyproject.toml
+-rw-r--r--   0        0        0      516 1970-01-01 00:00:00.000000 biosen12-2023.7.25.post2/setup.py
+-rw-r--r--   0        0        0      402 1970-01-01 00:00:00.000000 biosen12-2023.7.25.post2/PKG-INFO
```

