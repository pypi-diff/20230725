# Comparing `tmp/gogo_cli-0.1.2.tar.gz` & `tmp/gogo_cli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gogo_cli-0.1.2.tar", max compression
+gzip compressed data, was "gogo_cli-0.1.3.tar", max compression
```

## Comparing `gogo_cli-0.1.2.tar` & `gogo_cli-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-07-25 08:28:43.940696 gogo_cli-0.1.2/LICENSE
--rw-r--r--   0        0        0        0 2023-07-25 08:28:43.940696 gogo_cli-0.1.2/gogo_cli/__init__.py
--rw-r--r--   0        0        0      114 2023-07-25 08:28:43.940696 gogo_cli-0.1.2/gogo_cli/__main__.py
--rw-r--r--   0        0        0     2805 2023-07-25 08:28:43.940696 gogo_cli-0.1.2/gogo_cli/core/__gogo_cli__.py
--rw-r--r--   0        0        0        0 2023-07-25 08:28:43.940696 gogo_cli-0.1.2/gogo_cli/core/__init__.py
--rw-r--r--   0        0        0       19 2023-07-25 08:28:43.940696 gogo_cli-0.1.2/gogo_cli/core/__version__.py
--rw-r--r--   0        0        0      251 2023-07-25 08:28:43.940696 gogo_cli-0.1.2/gogo_cli/core/utils/__cast__.py
--rw-r--r--   0        0        0      743 2023-07-25 08:28:43.940696 gogo_cli-0.1.2/gogo_cli/core/utils/__downloader__.py
--rw-r--r--   0        0        0        0 2023-07-25 08:28:43.940696 gogo_cli-0.1.2/gogo_cli/core/utils/__init__.py
--rw-r--r--   0        0        0     1445 2023-07-25 08:28:43.940696 gogo_cli-0.1.2/gogo_cli/core/utils/__menu__.py
--rw-r--r--   0        0        0     1342 2023-07-25 08:28:43.940696 gogo_cli-0.1.2/gogo_cli/core/utils/__player__.py
--rw-r--r--   0        0        0      459 2023-07-25 08:28:43.940696 gogo_cli-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-25 08:28:43.940696 gogo_cli-0.1.2/readme.txt
--rw-r--r--   0        0        0      504 1970-01-01 00:00:00.000000 gogo_cli-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-25 12:30:20.783442 gogo_cli-0.1.3/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-25 12:30:20.783442 gogo_cli-0.1.3/gogo_cli/__init__.py
+-rw-r--r--   0        0        0      114 2023-07-25 12:30:20.783442 gogo_cli-0.1.3/gogo_cli/__main__.py
+-rw-r--r--   0        0        0     2805 2023-07-25 12:30:20.783442 gogo_cli-0.1.3/gogo_cli/core/__gogo_cli__.py
+-rw-r--r--   0        0        0        0 2023-07-25 12:30:20.783442 gogo_cli-0.1.3/gogo_cli/core/__init__.py
+-rw-r--r--   0        0        0       19 2023-07-25 12:30:20.783442 gogo_cli-0.1.3/gogo_cli/core/__version__.py
+-rw-r--r--   0        0        0      251 2023-07-25 12:30:20.783442 gogo_cli-0.1.3/gogo_cli/core/utils/__cast__.py
+-rw-r--r--   0        0        0      743 2023-07-25 12:30:20.783442 gogo_cli-0.1.3/gogo_cli/core/utils/__downloader__.py
+-rw-r--r--   0        0        0        0 2023-07-25 12:30:20.783442 gogo_cli-0.1.3/gogo_cli/core/utils/__init__.py
+-rw-r--r--   0        0        0     1445 2023-07-25 12:30:20.783442 gogo_cli-0.1.3/gogo_cli/core/utils/__menu__.py
+-rw-r--r--   0        0        0     1634 2023-07-25 12:30:20.783442 gogo_cli-0.1.3/gogo_cli/core/utils/__player__.py
+-rw-r--r--   0        0        0      459 2023-07-25 12:30:20.783442 gogo_cli-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-25 12:30:20.783442 gogo_cli-0.1.3/readme.txt
+-rw-r--r--   0        0        0      504 1970-01-01 00:00:00.000000 gogo_cli-0.1.3/PKG-INFO
```

### Comparing `gogo_cli-0.1.2/LICENSE` & `gogo_cli-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gogo_cli-0.1.2/gogo_cli/core/__gogo_cli__.py` & `gogo_cli-0.1.3/gogo_cli/core/__gogo_cli__.py`

 * *Files identical despite different names*

### Comparing `gogo_cli-0.1.2/gogo_cli/core/utils/__downloader__.py` & `gogo_cli-0.1.3/gogo_cli/core/utils/__downloader__.py`

 * *Files identical despite different names*

### Comparing `gogo_cli-0.1.2/gogo_cli/core/utils/__menu__.py` & `gogo_cli-0.1.3/gogo_cli/core/utils/__menu__.py`

 * *Files identical despite different names*

