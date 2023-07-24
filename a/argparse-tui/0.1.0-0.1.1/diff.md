# Comparing `tmp/argparse-tui-0.1.0.tar.gz` & `tmp/argparse-tui-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argparse-tui-0.1.0.tar", last modified: Sun Jul 23 04:29:37 2023, max compression
+gzip compressed data, was "argparse-tui-0.1.1.tar", last modified: Mon Jul 24 04:02:16 2023, max compression
```

## Comparing `argparse-tui-0.1.0.tar` & `argparse-tui-0.1.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 04:29:37.125522 argparse-tui-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     1058 2023-07-23 04:25:40.000000 argparse-tui-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5565 2023-07-23 04:29:37.125522 argparse-tui-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3901 2023-07-23 04:25:40.000000 argparse-tui-0.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)     4714 2023-07-23 04:25:40.000000 argparse-tui-0.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-23 04:29:37.125522 argparse-tui-0.1.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 04:29:37.117522 argparse-tui-0.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 04:29:37.121522 argparse-tui-0.1.0/src/argparse_tui/
--rw-r--r--   0 root         (0) root         (0)      159 2023-07-23 04:25:40.000000 argparse-tui-0.1.0/src/argparse_tui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 04:29:37.121522 argparse-tui-0.1.0/src/argparse_tui/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      299 2023-07-23 04:26:27.000000 argparse-tui-0.1.0/src/argparse_tui/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      156 2023-07-23 04:29:16.000000 argparse-tui-0.1.0/src/argparse_tui/__pycache__/__version__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     7277 2023-07-23 04:26:27.000000 argparse-tui-0.1.0/src/argparse_tui/__pycache__/argparse.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      312 2023-07-23 04:26:27.000000 argparse-tui-0.1.0/src/argparse_tui/__pycache__/constants.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     1303 2023-07-23 04:26:27.000000 argparse-tui-0.1.0/src/argparse_tui/__pycache__/detect_run_string.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     7006 2023-07-23 04:26:27.000000 argparse-tui-0.1.0/src/argparse_tui/__pycache__/run_command.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     4197 2023-07-23 04:26:27.000000 argparse-tui-0.1.0/src/argparse_tui/__pycache__/schemas.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)    11772 2023-07-23 04:26:27.000000 argparse-tui-0.1.0/src/argparse_tui/__pycache__/tui.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-23 04:29:16.000000 argparse-tui-0.1.0/src/argparse_tui/__version__.py
--rw-r--r--   0 root         (0) root         (0)    10637 2023-07-23 04:25:40.000000 argparse-tui-0.1.0/src/argparse_tui/argparse.py
--rw-r--r--   0 root         (0) root         (0)      164 2023-07-23 04:25:40.000000 argparse-tui-0.1.0/src/argparse_tui/constants.py
--rw-r--r--   0 root         (0) root         (0)     1740 2023-07-23 04:25:40.000000 argparse-tui-0.1.0/src/argparse_tui/detect_run_string.py
--rw-r--r--   0 root         (0) root         (0)    10938 2023-07-23 04:25:40.000000 argparse-tui-0.1.0/src/argparse_tui/run_command.py
--rw-r--r--   0 root         (0) root         (0)     3736 2023-07-23 04:25:40.000000 argparse-tui-0.1.0/src/argparse_tui/schemas.py
--rw-r--r--   0 root         (0) root         (0)    12743 2023-07-23 04:25:40.000000 argparse-tui-0.1.0/src/argparse_tui/tui.py
--rw-r--r--   0 root         (0) root         (0)     3859 2023-07-23 04:25:40.000000 argparse-tui-0.1.0/src/argparse_tui/tui.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 04:29:37.125522 argparse-tui-0.1.0/src/argparse_tui/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-23 04:25:40.000000 argparse-tui-0.1.0/src/argparse_tui/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 04:29:37.125522 argparse-tui-0.1.0/src/argparse_tui/widgets/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      140 2023-07-23 04:26:27.000000 argparse-tui-0.1.0/src/argparse_tui/widgets/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     3449 2023-07-23 04:26:28.000000 argparse-tui-0.1.0/src/argparse_tui/widgets/__pycache__/about.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     4146 2023-07-23 04:26:27.000000 argparse-tui-0.1.0/src/argparse_tui/widgets/__pycache__/command_info.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     2573 2023-07-23 04:26:27.000000 argparse-tui-0.1.0/src/argparse_tui/widgets/__pycache__/command_tree.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     6957 2023-07-23 04:26:27.000000 argparse-tui-0.1.0/src/argparse_tui/widgets/__pycache__/form.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     3854 2023-07-23 04:26:27.000000 argparse-tui-0.1.0/src/argparse_tui/widgets/__pycache__/multiple_choice.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)    11469 2023-07-23 04:26:27.000000 argparse-tui-0.1.0/src/argparse_tui/widgets/__pycache__/parameter_controls.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     2647 2023-07-23 04:25:40.000000 argparse-tui-0.1.0/src/argparse_tui/widgets/about.py
--rw-r--r--   0 root         (0) root         (0)     4010 2023-07-23 04:25:40.000000 argparse-tui-0.1.0/src/argparse_tui/widgets/command_info.py
--rw-r--r--   0 root         (0) root         (0)     2246 2023-07-23 04:25:40.000000 argparse-tui-0.1.0/src/argparse_tui/widgets/command_tree.py
--rw-r--r--   0 root         (0) root         (0)     8067 2023-07-23 04:25:40.000000 argparse-tui-0.1.0/src/argparse_tui/widgets/form.py
--rw-r--r--   0 root         (0) root         (0)     2857 2023-07-23 04:25:40.000000 argparse-tui-0.1.0/src/argparse_tui/widgets/multiple_choice.py
--rw-r--r--   0 root         (0) root         (0)    16529 2023-07-23 04:25:40.000000 argparse-tui-0.1.0/src/argparse_tui/widgets/parameter_controls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 04:29:37.121522 argparse-tui-0.1.0/src/argparse_tui.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5565 2023-07-23 04:29:37.000000 argparse-tui-0.1.0/src/argparse_tui.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1724 2023-07-23 04:29:37.000000 argparse-tui-0.1.0/src/argparse_tui.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-23 04:29:37.000000 argparse-tui-0.1.0/src/argparse_tui.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      556 2023-07-23 04:29:37.000000 argparse-tui-0.1.0/src/argparse_tui.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-23 04:29:37.000000 argparse-tui-0.1.0/src/argparse_tui.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 04:29:37.125522 argparse-tui-0.1.0/tests/
--rw-r--r--   0 root         (0) root         (0)     1611 2023-07-23 04:25:40.000000 argparse-tui-0.1.0/tests/test_help_argparse.py
--rw-r--r--   0 root         (0) root         (0)     3897 2023-07-23 04:25:40.000000 argparse-tui-0.1.0/tests/test_run_command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 04:02:16.445725 argparse-tui-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-07-24 03:58:21.000000 argparse-tui-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5565 2023-07-24 04:02:16.445725 argparse-tui-0.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3901 2023-07-24 03:58:21.000000 argparse-tui-0.1.1/README.md
+-rw-r--r--   0 root         (0) root         (0)     4714 2023-07-24 03:58:21.000000 argparse-tui-0.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 04:02:16.445725 argparse-tui-0.1.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 04:02:16.437725 argparse-tui-0.1.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 04:02:16.437725 argparse-tui-0.1.1/src/argparse_tui/
+-rw-r--r--   0 root         (0) root         (0)      159 2023-07-24 03:58:21.000000 argparse-tui-0.1.1/src/argparse_tui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 04:02:16.441725 argparse-tui-0.1.1/src/argparse_tui/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      299 2023-07-24 03:59:06.000000 argparse-tui-0.1.1/src/argparse_tui/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-24 04:01:55.000000 argparse-tui-0.1.1/src/argparse_tui/__pycache__/__version__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     6956 2023-07-24 03:59:06.000000 argparse-tui-0.1.1/src/argparse_tui/__pycache__/argparse.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      312 2023-07-24 03:59:06.000000 argparse-tui-0.1.1/src/argparse_tui/__pycache__/constants.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     1303 2023-07-24 03:59:06.000000 argparse-tui-0.1.1/src/argparse_tui/__pycache__/detect_run_string.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     7006 2023-07-24 03:59:06.000000 argparse-tui-0.1.1/src/argparse_tui/__pycache__/run_command.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     4197 2023-07-24 03:59:06.000000 argparse-tui-0.1.1/src/argparse_tui/__pycache__/schemas.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)    11772 2023-07-24 03:59:06.000000 argparse-tui-0.1.1/src/argparse_tui/__pycache__/tui.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-24 04:01:55.000000 argparse-tui-0.1.1/src/argparse_tui/__version__.py
+-rw-r--r--   0 root         (0) root         (0)    10247 2023-07-24 03:58:21.000000 argparse-tui-0.1.1/src/argparse_tui/argparse.py
+-rw-r--r--   0 root         (0) root         (0)      164 2023-07-24 03:58:21.000000 argparse-tui-0.1.1/src/argparse_tui/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-07-24 03:58:21.000000 argparse-tui-0.1.1/src/argparse_tui/detect_run_string.py
+-rw-r--r--   0 root         (0) root         (0)    10938 2023-07-24 03:58:21.000000 argparse-tui-0.1.1/src/argparse_tui/run_command.py
+-rw-r--r--   0 root         (0) root         (0)     3736 2023-07-24 03:58:21.000000 argparse-tui-0.1.1/src/argparse_tui/schemas.py
+-rw-r--r--   0 root         (0) root         (0)    12743 2023-07-24 03:58:21.000000 argparse-tui-0.1.1/src/argparse_tui/tui.py
+-rw-r--r--   0 root         (0) root         (0)     3859 2023-07-24 03:58:21.000000 argparse-tui-0.1.1/src/argparse_tui/tui.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 04:02:16.445725 argparse-tui-0.1.1/src/argparse_tui/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 03:58:21.000000 argparse-tui-0.1.1/src/argparse_tui/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 04:02:16.445725 argparse-tui-0.1.1/src/argparse_tui/widgets/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-24 03:59:06.000000 argparse-tui-0.1.1/src/argparse_tui/widgets/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     3449 2023-07-24 03:59:07.000000 argparse-tui-0.1.1/src/argparse_tui/widgets/__pycache__/about.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     4146 2023-07-24 03:59:06.000000 argparse-tui-0.1.1/src/argparse_tui/widgets/__pycache__/command_info.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     2573 2023-07-24 03:59:06.000000 argparse-tui-0.1.1/src/argparse_tui/widgets/__pycache__/command_tree.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     6957 2023-07-24 03:59:06.000000 argparse-tui-0.1.1/src/argparse_tui/widgets/__pycache__/form.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     3854 2023-07-24 03:59:06.000000 argparse-tui-0.1.1/src/argparse_tui/widgets/__pycache__/multiple_choice.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)    11469 2023-07-24 03:59:06.000000 argparse-tui-0.1.1/src/argparse_tui/widgets/__pycache__/parameter_controls.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     2647 2023-07-24 03:58:21.000000 argparse-tui-0.1.1/src/argparse_tui/widgets/about.py
+-rw-r--r--   0 root         (0) root         (0)     4010 2023-07-24 03:58:21.000000 argparse-tui-0.1.1/src/argparse_tui/widgets/command_info.py
+-rw-r--r--   0 root         (0) root         (0)     2246 2023-07-24 03:58:21.000000 argparse-tui-0.1.1/src/argparse_tui/widgets/command_tree.py
+-rw-r--r--   0 root         (0) root         (0)     8067 2023-07-24 03:58:21.000000 argparse-tui-0.1.1/src/argparse_tui/widgets/form.py
+-rw-r--r--   0 root         (0) root         (0)     2857 2023-07-24 03:58:21.000000 argparse-tui-0.1.1/src/argparse_tui/widgets/multiple_choice.py
+-rw-r--r--   0 root         (0) root         (0)    16529 2023-07-24 03:58:21.000000 argparse-tui-0.1.1/src/argparse_tui/widgets/parameter_controls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 04:02:16.441725 argparse-tui-0.1.1/src/argparse_tui.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5565 2023-07-24 04:02:16.000000 argparse-tui-0.1.1/src/argparse_tui.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1724 2023-07-24 04:02:16.000000 argparse-tui-0.1.1/src/argparse_tui.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 04:02:16.000000 argparse-tui-0.1.1/src/argparse_tui.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      556 2023-07-24 04:02:16.000000 argparse-tui-0.1.1/src/argparse_tui.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-24 04:02:16.000000 argparse-tui-0.1.1/src/argparse_tui.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 04:02:16.445725 argparse-tui-0.1.1/tests/
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-07-24 03:58:21.000000 argparse-tui-0.1.1/tests/test_help_argparse.py
+-rw-r--r--   0 root         (0) root         (0)     3897 2023-07-24 03:58:21.000000 argparse-tui-0.1.1/tests/test_run_command.py
```

### Comparing `argparse-tui-0.1.0/LICENSE` & `argparse-tui-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.0/PKG-INFO` & `argparse-tui-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argparse-tui
-Version: 0.1.0
+Version: 0.1.1
 Summary: Display your Python argparse CLI as a TUI.
 Author-email: Donald Mellenbruch <hello@f2dv.com>
 License: Copyright 2023 Donald Mellenbruch
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `argparse-tui-0.1.0/README.md` & `argparse-tui-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.0/pyproject.toml` & `argparse-tui-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.0/src/argparse_tui/__pycache__/argparse.cpython-310.pyc` & `argparse-tui-0.1.1/src/argparse_tui/__pycache__/argparse.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jul 23 04:25:40 2023 UTC, .py size: 10637 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-00000000: 6f0d 0d0a 0000 0000 c4ab bc64 8d29 0000  o..........d.)..
+00000000: 6f0d 0d0a 0000 0000 ddf6 bd64 0728 0000  o..........d.(..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 a400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 6400 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 6d06 5a06 0100 6404 6405 6c07  m.Z.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6404 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 0100 6404  m.Z.m.Z.m.Z...d.
-00000080: 6407 6c0e 6d0f 5a0f 0100 0902 641e 641f  d.l.m.Z.....d.d.
+00000080: 6407 6c0e 6d0f 5a0f 0100 0902 641d 641e  d.l.m.Z.....d.d.
 00000090: 640e 640f 8405 5a10 4700 6410 6411 8400  d.d...Z.G.d.d...
 000000a0: 6411 6502 6a11 8303 5a12 6402 6412 6502  d.e.j...Z.d.d.e.
-000000b0: 6a13 6603 6420 6418 6419 8405 5a14 6508  j.f.d d.d...Z.e.
-000000c0: 6412 6602 6421 641c 641d 8405 5a15 6402  d.f.d!d.d...Z.d.
-000000d0: 5300 2922 e900 0000 0029 01da 0b61 6e6e  S.)".....)...ann
+000000b0: 6a13 6603 641f 6418 6419 8405 5a14 6508  j.f.d.d.d...Z.e.
+000000c0: 6412 6602 6420 641b 641c 8405 5a15 6402  d.f.d d.d...Z.d.
+000000d0: 5300 2921 e900 0000 0029 01da 0b61 6e6e  S.)!.....)...ann
 000000e0: 6f74 6174 696f 6e73 4e29 02da 0341 6e79  otationsN)...Any
 000000f0: da04 5479 7065 e901 0000 0029 01da 1444  ..Type.....)...D
 00000100: 4546 4155 4c54 5f43 4f4d 4d41 4e44 5f4e  EFAULT_COMMAND_N
 00000110: 414d 4529 04da 0e41 7267 756d 656e 7453  AME)...ArgumentS
 00000120: 6368 656d 61da 0b43 6f6d 6d61 6e64 4e61  chema..CommandNa
 00000130: 6d65 da0d 436f 6d6d 616e 6453 6368 656d  me..CommandSchem
 00000140: 61da 0c4f 7074 696f 6e53 6368 656d 6129  a..OptionSchema)
@@ -308,15 +308,15 @@
 00001330: 044e 6f6e 6563 0400 0000 0000 0000 0000  .Nonec..........
 00001340: 0000 0500 0000 0700 0000 4b00 0001 734e  ..........K...sN
 00001350: 0000 007c 0173 1064 0174 00a0 0164 0264  ...|.s.d.t...d.d
 00001360: 03a1 02a0 0264 03a1 019b 009d 0267 017d  .....d.......g.}
 00001370: 016e 0874 037c 0174 0483 0272 187c 0167  .n.t.|.t...r.|.g
 00001380: 017d 017c 006a 057c 0164 0474 067c 037c  .}.|.j.|.d.t.|.|
 00001390: 0264 059c 047c 04a4 018e 0101 0064 0653  .d...|.......d.S
-000013a0: 0029 0761 d101 0000 0a0a 2020 2020 4172  .).a......    Ar
+000013a0: 0029 0761 dd01 0000 0a0a 2020 2020 4172  .).a......    Ar
 000013b0: 6773 3a0a 2020 2020 2020 2020 7061 7273  gs:.        pars
 000013c0: 6572 3a20 7468 6520 6172 6770 6172 7365  er: the argparse
 000013d0: 2070 6172 7365 720a 2020 2020 2020 2020   parser.        
 000013e0: 6f70 7469 6f6e 5f73 7472 696e 6773 3a20  option_strings: 
 000013f0: 6c69 7374 206f 6620 434c 4920 666c 6167  list of CLI flag
 00001400: 7320 7468 6174 2077 696c 6c20 696e 766f  s that will invo
 00001410: 6b65 2074 6865 2054 5549 2028 6465 6661  ke the TUI (defa
@@ -329,127 +329,107 @@
 00001480: 7273 650a 2020 2020 2020 2020 3e3e 3e20  rse.        >>> 
 00001490: 6672 6f6d 2061 7267 7061 7273 655f 7475  from argparse_tu
 000014a0: 6920 696d 706f 7274 2061 6464 5f74 7569  i import add_tui
 000014b0: 5f61 7267 756d 656e 740a 2020 2020 2020  _argument.      
 000014c0: 2020 2e2e 2e0a 2020 2020 2020 2020 3e3e    ....        >>
 000014d0: 3e20 7061 7273 6572 203d 2061 7267 7061  > parser = argpa
 000014e0: 7273 652e 4172 6775 6d65 6e74 5061 7273  rse.ArgumentPars
-000014f0: 6572 2829 0a20 2020 2020 2020 203e 3e3e  er().        >>>
-00001500: 2061 6464 5f74 7569 5f61 7267 756d 656e   add_tui_argumen
-00001510: 7428 7061 7273 6572 290a 2020 2020 2020  t(parser).      
-00001520: 2020 2e2e 2e0a 2020 2020 2020 2020 3e3e    ....        >>
-00001530: 3e20 7061 7273 6572 2e70 7269 6e74 5f75  > parser.print_u
-00001540: 7361 6765 2829 0a20 2020 2020 2020 2075  sage().        u
-00001550: 7361 6765 3a20 5f5f 6d61 696e 5f5f 2e70  sage: __main__.p
-00001560: 7920 5b2d 685d 205b 2d2d 7475 6920 5b43  y [-h] [--tui [C
-00001570: 4d44 5d5d 0a20 2020 207a 022d 2dda 015f  MD]].    z.--.._
-00001580: da01 2d5a 0343 4d44 2904 7266 0000 00da  ..-Z.CMD).rf....
-00001590: 0661 6374 696f 6e72 3700 0000 7238 0000  .actionr7...r8..
-000015a0: 004e 2907 7206 0000 0072 5300 0000 da06  .N).r....rS.....
-000015b0: 6c73 7472 6970 7242 0000 0072 5400 0000  lstriprB...rT...
-000015c0: da0c 6164 645f 6172 6775 6d65 6e74 7243  ..add_argumentrC
-000015d0: 0000 0029 0572 0c00 0000 724a 0000 0072  ...).r....rJ...r
-000015e0: 3800 0000 7237 0000 00da 066b 7761 7267  8...r7.....kwarg
-000015f0: 7372 1e00 0000 721e 0000 0072 2300 0000  sr....r....r#...
-00001600: da10 6164 645f 7475 695f 6172 6775 6d65  ..add_tui_argume
-00001610: 6e74 e100 0000 731a 0000 0004 181c 010a  nt....s.........
-00001620: 0106 0104 0202 0102 0102 0102 0102 0104  ................
-00001630: fb02 060a fa72 8200 0000 fa34 6172 6770  .....r.....4argp
-00001640: 6172 7365 2e41 7267 756d 656e 7450 6172  arse.ArgumentPar
-00001650: 7365 7220 7c20 6172 6770 6172 7365 2e5f  ser | argparse._
-00001660: 5375 6250 6172 7365 7273 4163 7469 6f6e  SubParsersAction
-00001670: da07 636f 6d6d 616e 6463 0300 0000 0000  ..commandc......
-00001680: 0000 0000 0000 0600 0000 0600 0000 4300  ..............C.
-00001690: 0001 736e 0000 0074 007c 0074 016a 0283  ..sn...t.|.t.j..
-000016a0: 0272 097c 007d 036e 147c 006a 0344 005d  .r.|.}.n.|.j.D.]
-000016b0: 0c7d 0474 007c 0474 016a 0283 0272 187c  .}.t.|.t.j...r.|
-000016c0: 047d 0301 006e 0571 0c7c 00a0 04a1 007d  .}...n.q.|.....}
-000016d0: 037c 036a 057c 0174 016a 067c 0264 018d  .|.j.|.t.j.|.d..
-000016e0: 037d 057c 056a 077c 0064 028d 0101 0074  .}.|.j.|.d.....t
-000016f0: 087c 0564 0367 0164 0464 0564 068d 0401  .|.d.g.d.d.d....
-00001700: 0064 0453 0029 0761 0703 0000 0a0a 2020  .d.S.).a......  
-00001710: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00001720: 7061 7273 6572 3a20 7468 6520 6172 6770  parser: the argp
-00001730: 6172 7365 2070 6172 7365 720a 2020 2020  arse parser.    
-00001740: 2020 2020 636f 6d6d 616e 643a 206e 616d      command: nam
-00001750: 6520 6f66 2074 6865 2043 4c49 2063 6f6d  e of the CLI com
-00001760: 6d61 6e64 2074 6861 7420 7769 6c6c 2069  mand that will i
-00001770: 6e76 6f6b 6520 7468 6520 5455 4920 2864  nvoke the TUI (d
-00001780: 6566 6175 6c74 3d60 7475 6960 290a 2020  efault=`tui`).  
-00001790: 2020 2020 2020 6865 6c70 3a20 6865 6c70        help: help
-000017a0: 206d 6573 7361 6765 2066 6f72 2074 6865   message for the
-000017b0: 2061 7267 756d 656e 740a 0a20 2020 2045   argument..    E
-000017c0: 7861 6d70 6c65 733a 0a20 2020 2020 2020  xamples:.       
-000017d0: 203e 3e3e 2069 6d70 6f72 7420 6172 6770   >>> import argp
-000017e0: 6172 7365 0a20 2020 2020 2020 203e 3e3e  arse.        >>>
-000017f0: 2066 726f 6d20 6172 6770 6172 7365 5f74   from argparse_t
-00001800: 7569 2069 6d70 6f72 7420 6164 645f 7475  ui import add_tu
-00001810: 695f 6172 6775 6d65 6e74 0a20 2020 2020  i_argument.     
-00001820: 2020 202e 2e2e 0a20 2020 2020 2020 203e     ....        >
-00001830: 3e3e 2070 6172 7365 7220 3d20 6172 6770  >> parser = argp
-00001840: 6172 7365 2e41 7267 756d 656e 7450 6172  arse.ArgumentPar
-00001850: 7365 7228 290a 2020 2020 2020 2020 3e3e  ser().        >>
-00001860: 3e20 6164 645f 7475 695f 636f 6d6d 616e  > add_tui_comman
-00001870: 6428 7061 7273 6572 290a 2020 2020 2020  d(parser).      
-00001880: 2020 2e2e 2e0a 2020 2020 2020 2020 3e3e    ....        >>
-00001890: 3e20 7061 7273 6572 2e70 7269 6e74 5f75  > parser.print_u
-000018a0: 7361 6765 2829 0a20 2020 2020 2020 2075  sage().        u
-000018b0: 7361 6765 3a20 5f5f 6d61 696e 5f5f 2e70  sage: __main__.p
-000018c0: 7920 5b2d 685d 207b 7475 697d 202e 2e2e  y [-h] {tui} ...
-000018d0: 0a0a 2020 2020 2020 2020 3e3e 3e20 696d  ..        >>> im
-000018e0: 706f 7274 2061 7267 7061 7273 650a 2020  port argparse.  
-000018f0: 2020 2020 2020 3e3e 3e20 6672 6f6d 2061        >>> from a
-00001900: 7267 7061 7273 655f 7475 6920 696d 706f  rgparse_tui impo
-00001910: 7274 2061 6464 5f74 7569 5f61 7267 756d  rt add_tui_argum
-00001920: 656e 740a 2020 2020 2020 2020 2e2e 2e0a  ent.        ....
-00001930: 2020 2020 2020 2020 3e3e 3e20 7061 7273          >>> pars
-00001940: 6572 203d 2061 7267 7061 7273 652e 4172  er = argparse.Ar
-00001950: 6775 6d65 6e74 5061 7273 6572 2829 0a20  gumentParser(). 
-00001960: 2020 2020 2020 203e 3e3e 2073 7562 7061         >>> subpa
-00001970: 7273 6572 7320 3d20 7061 7273 6572 2e61  rsers = parser.a
-00001980: 6464 5f73 7562 7061 7273 6572 7328 290a  dd_subparsers().
-00001990: 2020 2020 2020 2020 3e3e 3e20 6164 645f          >>> add_
-000019a0: 7475 695f 636f 6d6d 616e 6428 7375 6270  tui_command(subp
-000019b0: 6172 7365 7273 290a 2020 2020 2020 2020  arsers).        
-000019c0: 2e2e 2e0a 2020 2020 2020 2020 3e3e 3e20  ....        >>> 
-000019d0: 7061 7273 6572 2e70 7269 6e74 5f75 7361  parser.print_usa
-000019e0: 6765 2829 0a20 2020 2020 2020 2075 7361  ge().        usa
-000019f0: 6765 3a20 5f5f 6d61 696e 5f5f 2e70 7920  ge: __main__.py 
-00001a00: 5b2d 685d 207b 7475 697d 202e 2e2e 0a20  [-h] {tui} .... 
-00001a10: 2020 2029 0272 3f00 0000 7238 0000 0029     ).r?...r8...)
-00001a20: 0172 6e00 0000 5a0a 636d 645f 6669 6c74  .rn...Z.cmd_filt
-00001a30: 6572 4e7a 0e43 6f6d 6d61 6e64 2066 696c  erNz.Command fil
-00001a40: 7465 7229 0372 4a00 0000 7237 0000 0072  ter).rJ...r7...r
-00001a50: 3800 0000 2909 7242 0000 0072 4400 0000  8...).rB...rD...
-00001a60: 7246 0000 0072 4100 0000 da0e 6164 645f  rF...rA.....add_
-00001a70: 7375 6270 6172 7365 7273 da0a 6164 645f  subparsers..add_
-00001a80: 7061 7273 6572 7245 0000 00da 0c73 6574  parserrE.....set
-00001a90: 5f64 6566 6175 6c74 7372 8200 0000 2906  _defaultsr....).
-00001aa0: 720c 0000 0072 8400 0000 7238 0000 005a  r....r....r8...Z
-00001ab0: 0a73 7562 7061 7273 6572 7372 7e00 0000  .subparsersr~...
-00001ac0: 5a0a 7475 695f 7061 7273 6572 721e 0000  Z.tui_parserr...
-00001ad0: 0072 1e00 0000 7223 0000 00da 0f61 6464  .r....r#.....add
-00001ae0: 5f74 7569 5f63 6f6d 6d61 6e64 0801 0000  _tui_command....
-00001af0: 7328 0000 000c 2106 010a 020c 0104 0104  s(....!.........
-00001b00: 0102 fe08 0404 0202 0104 0102 0106 fd0c  ................
-00001b10: 0502 0202 0104 0102 0102 010a fc72 8800  .............r..
-00001b20: 0000 725f 0000 0029 0672 0c00 0000 720d  ..r_...).r....r.
-00001b30: 0000 0072 0e00 0000 720f 0000 0072 1000  ...r....r....r..
-00001b40: 0000 7211 0000 0029 0872 0c00 0000 720d  ..r....).r....r.
-00001b50: 0000 0072 4a00 0000 727a 0000 0072 3800  ...rJ...rz...r8.
-00001b60: 0000 7254 0000 0072 1000 0000 727b 0000  ..rT...r....r{..
-00001b70: 0029 0872 0c00 0000 7283 0000 0072 8400  .).r....r....r..
-00001b80: 0000 7254 0000 0072 3800 0000 7254 0000  ..rT...r8...rT..
-00001b90: 0072 1000 0000 727b 0000 0029 16da 0a5f  .r....r{...)..._
-00001ba0: 5f66 7574 7572 655f 5f72 0200 0000 7244  _future__r....rD
-00001bb0: 0000 0072 4e00 0000 da06 7479 7069 6e67  ...rN.....typing
-00001bc0: 7203 0000 0072 0400 0000 da09 636f 6e73  r....r......cons
-00001bd0: 7461 6e74 7372 0600 0000 5a07 7363 6865  tantsr....Z.sche
-00001be0: 6d61 7372 0700 0000 7208 0000 0072 0900  masr....r....r..
-00001bf0: 0000 720a 0000 00da 0374 7569 720b 0000  ..r......tuir...
-00001c00: 0072 6100 0000 da06 4163 7469 6f6e 7243  .ra.....ActionrC
-00001c10: 0000 0072 4500 0000 7282 0000 0072 8800  ...rE...r....r..
-00001c20: 0000 721e 0000 0072 1e00 0000 721e 0000  ..r....r....r...
-00001c30: 0072 2300 0000 da08 3c6d 6f64 756c 653e  .r#.....<module>
-00001c40: 0100 0000 7324 0000 000c 0008 0208 0110  ....s$..........
-00001c50: 010c 0218 010c 0102 050c fe00 7f12 2302  ..............#.
-00001c60: 3502 0104 010c fc02 2902 0110 fd         5.......)....
+000014f0: 6572 2829 0a20 2020 2020 2020 202e 2e2e  er().        ...
+00001500: 0a20 2020 2020 2020 203e 3e3e 2061 6464  .        >>> add
+00001510: 5f74 7569 5f61 7267 756d 656e 7428 7061  _tui_argument(pa
+00001520: 7273 6572 290a 2020 2020 2020 2020 2e2e  rser).        ..
+00001530: 2e0a 2020 2020 2020 2020 3e3e 3e20 7061  ..        >>> pa
+00001540: 7273 6572 2e70 7269 6e74 5f75 7361 6765  rser.print_usage
+00001550: 2829 0a20 2020 2020 2020 2075 7361 6765  ().        usage
+00001560: 3a20 5f5f 6d61 696e 5f5f 2e70 7920 5b2d  : __main__.py [-
+00001570: 685d 205b 2d2d 7475 6920 5b43 4d44 5d5d  h] [--tui [CMD]]
+00001580: 0a20 2020 207a 022d 2dda 015f da01 2d5a  .    z.--.._..-Z
+00001590: 0343 4d44 2904 7266 0000 00da 0661 6374  .CMD).rf.....act
+000015a0: 696f 6e72 3700 0000 7238 0000 004e 2907  ionr7...r8...N).
+000015b0: 7206 0000 0072 5300 0000 da06 6c73 7472  r....rS.....lstr
+000015c0: 6970 7242 0000 0072 5400 0000 da0c 6164  iprB...rT.....ad
+000015d0: 645f 6172 6775 6d65 6e74 7243 0000 0029  d_argumentrC...)
+000015e0: 0572 0c00 0000 724a 0000 0072 3800 0000  .r....rJ...r8...
+000015f0: 7237 0000 00da 066b 7761 7267 7372 1e00  r7.....kwargsr..
+00001600: 0000 721e 0000 0072 2300 0000 da10 6164  ..r....r#.....ad
+00001610: 645f 7475 695f 6172 6775 6d65 6e74 e100  d_tui_argument..
+00001620: 0000 731a 0000 0004 191c 010a 0106 0104  ..s.............
+00001630: 0202 0102 0102 0102 0102 0104 fb02 060a  ................
+00001640: fa72 8200 0000 da07 636f 6d6d 616e 6463  .r......commandc
+00001650: 0300 0000 0000 0000 0000 0000 0600 0000  ................
+00001660: 0600 0000 4300 0001 735c 0000 007c 006a  ....C...s\...|.j
+00001670: 0044 005d 0c7d 0374 017c 0374 026a 0383  .D.].}.t.|.t.j..
+00001680: 0272 0f7c 037d 0401 006e 0571 037c 00a0  .r.|.}...n.q.|..
+00001690: 04a1 007d 047c 046a 057c 0174 026a 067c  ...}.|.j.|.t.j.|
+000016a0: 0264 018d 037d 057c 056a 077c 0064 028d  .d...}.|.j.|.d..
+000016b0: 0101 0074 087c 0564 0367 0164 0464 0564  ...t.|.d.g.d.d.d
+000016c0: 068d 0401 0064 0453 0029 0761 0602 0000  .....d.S.).a....
+000016d0: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+000016e0: 2020 2020 7061 7273 6572 3a20 7468 6520      parser: the 
+000016f0: 6172 6770 6172 7365 2070 6172 7365 720a  argparse parser.
+00001700: 2020 2020 2020 2020 636f 6d6d 616e 643a          command:
+00001710: 206e 616d 6520 6f66 2074 6865 2043 4c49   name of the CLI
+00001720: 2063 6f6d 6d61 6e64 2074 6861 7420 7769   command that wi
+00001730: 6c6c 2069 6e76 6f6b 6520 7468 6520 5455  ll invoke the TU
+00001740: 4920 2864 6566 6175 6c74 3d60 7475 6960  I (default=`tui`
+00001750: 290a 2020 2020 2020 2020 6865 6c70 3a20  ).        help: 
+00001760: 6865 6c70 206d 6573 7361 6765 2066 6f72  help message for
+00001770: 2074 6865 2061 7267 756d 656e 740a 0a20   the argument.. 
+00001780: 2020 2045 7861 6d70 6c65 733a 0a20 2020     Examples:.   
+00001790: 2020 2020 203e 3e3e 2069 6d70 6f72 7420       >>> import 
+000017a0: 6172 6770 6172 7365 0a20 2020 2020 2020  argparse.       
+000017b0: 203e 3e3e 2066 726f 6d20 6172 6770 6172   >>> from argpar
+000017c0: 7365 5f74 7569 2069 6d70 6f72 7420 6164  se_tui import ad
+000017d0: 645f 7475 695f 6172 6775 6d65 6e74 0a20  d_tui_argument. 
+000017e0: 2020 2020 2020 202e 2e2e 0a20 2020 2020         ....     
+000017f0: 2020 203e 3e3e 2070 6172 7365 7220 3d20     >>> parser = 
+00001800: 6172 6770 6172 7365 2e41 7267 756d 656e  argparse.Argumen
+00001810: 7450 6172 7365 7228 290a 2020 2020 2020  tParser().      
+00001820: 2020 3e3e 3e20 7375 6270 6172 7365 7273    >>> subparsers
+00001830: 203d 2070 6172 7365 722e 6164 645f 7375   = parser.add_su
+00001840: 6270 6172 7365 7273 2829 0a20 2020 2020  bparsers().     
+00001850: 2020 202e 2e2e 0a20 2020 2020 2020 203e     ....        >
+00001860: 3e3e 2061 6464 5f74 7569 5f63 6f6d 6d61  >> add_tui_comma
+00001870: 6e64 2870 6172 7365 7229 0a20 2020 2020  nd(parser).     
+00001880: 2020 202e 2e2e 0a20 2020 2020 2020 203e     ....        >
+00001890: 3e3e 2070 6172 7365 722e 7072 696e 745f  >> parser.print_
+000018a0: 7573 6167 6528 290a 2020 2020 2020 2020  usage().        
+000018b0: 7573 6167 653a 205f 5f6d 6169 6e5f 5f2e  usage: __main__.
+000018c0: 7079 205b 2d68 5d20 7b74 7569 7d20 2e2e  py [-h] {tui} ..
+000018d0: 2e0a 2020 2020 2902 723f 0000 0072 3800  ..    ).r?...r8.
+000018e0: 0000 2901 726e 0000 005a 0a63 6d64 5f66  ..).rn...Z.cmd_f
+000018f0: 696c 7465 724e 7a0e 436f 6d6d 616e 6420  ilterNz.Command 
+00001900: 6669 6c74 6572 2903 724a 0000 0072 3700  filter).rJ...r7.
+00001910: 0000 7238 0000 0029 0972 4100 0000 7242  ..r8...).rA...rB
+00001920: 0000 0072 4400 0000 7246 0000 00da 0e61  ...rD...rF.....a
+00001930: 6464 5f73 7562 7061 7273 6572 73da 0a61  dd_subparsers..a
+00001940: 6464 5f70 6172 7365 7272 4500 0000 da0c  dd_parserrE.....
+00001950: 7365 745f 6465 6661 756c 7473 7282 0000  set_defaultsr...
+00001960: 0029 0672 0c00 0000 7283 0000 0072 3800  .).r....r....r8.
+00001970: 0000 727e 0000 005a 0a73 7562 7061 7273  ..r~...Z.subpars
+00001980: 6572 735a 0a74 7569 5f70 6172 7365 7272  ersZ.tui_parserr
+00001990: 1e00 0000 721e 0000 0072 2300 0000 da0f  ....r....r#.....
+000019a0: 6164 645f 7475 695f 636f 6d6d 616e 6409  add_tui_command.
+000019b0: 0100 0073 2400 0000 0a1a 0c01 0401 0401  ...s$...........
+000019c0: 02fe 0804 0402 0201 0401 0201 06fd 0c05  ................
+000019d0: 0202 0201 0401 0201 0201 0afc 7287 0000  ............r...
+000019e0: 0072 5f00 0000 2906 720c 0000 0072 0d00  .r_...).r....r..
+000019f0: 0000 720e 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+00001a00: 0072 1100 0000 2908 720c 0000 0072 0d00  .r....).r....r..
+00001a10: 0000 724a 0000 0072 7a00 0000 7238 0000  ..rJ...rz...r8..
+00001a20: 0072 5400 0000 7210 0000 0072 7b00 0000  .rT...r....r{...
+00001a30: 2908 720c 0000 0072 0d00 0000 7283 0000  ).r....r....r...
+00001a40: 0072 5400 0000 7238 0000 0072 5400 0000  .rT...r8...rT...
+00001a50: 7210 0000 0072 7b00 0000 2916 da0a 5f5f  r....r{...)...__
+00001a60: 6675 7475 7265 5f5f 7202 0000 0072 4400  future__r....rD.
+00001a70: 0000 724e 0000 00da 0674 7970 696e 6772  ..rN.....typingr
+00001a80: 0300 0000 7204 0000 00da 0963 6f6e 7374  ....r......const
+00001a90: 616e 7473 7206 0000 005a 0773 6368 656d  antsr....Z.schem
+00001aa0: 6173 7207 0000 0072 0800 0000 7209 0000  asr....r....r...
+00001ab0: 0072 0a00 0000 da03 7475 6972 0b00 0000  .r......tuir....
+00001ac0: 7261 0000 00da 0641 6374 696f 6e72 4300  ra.....ActionrC.
+00001ad0: 0000 7245 0000 0072 8200 0000 7287 0000  ..rE...r....r...
+00001ae0: 0072 1e00 0000 721e 0000 0072 1e00 0000  .r....r....r....
+00001af0: 7223 0000 00da 083c 6d6f 6475 6c65 3e01  r#.....<module>.
+00001b00: 0000 0073 2400 0000 0c00 0802 0801 1001  ...s$...........
+00001b10: 0c02 1801 0c01 0205 0cfe 007f 1223 0235  .............#.5
+00001b20: 0201 0401 0cfc 022a 0201 10fd            .......*....
```

### Comparing `argparse-tui-0.1.0/src/argparse_tui/__pycache__/detect_run_string.cpython-310.pyc` & `argparse-tui-0.1.1/src/argparse_tui/__pycache__/detect_run_string.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jul 23 04:25:40 2023 UTC, .py size: 1740 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c4ab bc64 cc06 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 ddf6 bd64 cc06 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 4800 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 6400 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 640b 6405 6406 8404 5a05 6402 6504  Z.d.d.d...Z.d.e.
 00000060: 6a06 6407 1900 6602 640c 6409 640a 8405  j.d...f.d.d.d...
 00000070: 5a07 6402 5300 290d e900 0000 0029 01da  Z.d.S.)......)..
```

### Comparing `argparse-tui-0.1.0/src/argparse_tui/__pycache__/run_command.cpython-310.pyc` & `argparse-tui-0.1.1/src/argparse_tui/__pycache__/run_command.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jul 23 04:25:40 2023 UTC, .py size: 10938 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c4ab bc64 ba2a 0000  o..........d.*..
+00000000: 6f0d 0d0a 0000 0000 ddf6 bd64 ba2a 0000  o..........d.*..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 c400 0000 5500  .....@...s....U.
 00000030: 6400 6401 6c00 6d01 5a01 0100 6400 6402  d.d.l.m.Z...d.d.
 00000040: 6c02 5a02 6400 6402 6c03 5a03 6400 6403  l.Z.d.d.l.Z.d.d.
 00000050: 6c04 6d05 5a05 0100 6400 6404 6c06 6d07  l.m.Z...d.d.l.m.
 00000060: 5a07 0100 6400 6405 6c08 6d09 5a09 6d0a  Z...d.d.l.m.Z.m.
 00000070: 5a0a 6d0b 5a0b 0100 6400 6406 6c0c 6d0d  Z.m.Z...d.d.l.m.
```

### Comparing `argparse-tui-0.1.0/src/argparse_tui/__pycache__/schemas.cpython-310.pyc` & `argparse-tui-0.1.1/src/argparse_tui/__pycache__/schemas.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jul 23 04:25:40 2023 UTC, .py size: 3736 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c4ab bc64 980e 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 ddf6 bd64 980e 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0173 ba00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 0100 6406 6407 8400 5a0d 6504  m.Z...d.d...Z.e.
```

### Comparing `argparse-tui-0.1.0/src/argparse_tui/__pycache__/tui.cpython-310.pyc` & `argparse-tui-0.1.1/src/argparse_tui/__pycache__/tui.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jul 23 04:25:40 2023 UTC, .py size: 12743 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c4ab bc64 c731 0000  o..........d.1..
+00000000: 6f0d 0d0a 0000 0000 ddf6 bd64 c731 0000  o..........d.1..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 a401 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 6400 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6400 6403 6c05 6d06 5a06 0100 6400  Z.d.d.l.m.Z...d.
 00000060: 6404 6c07 6d07 5a07 0100 6400 6405 6c08  d.l.m.Z...d.d.l.
 00000070: 6d09 5a09 0100 6400 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
@@ -72,18 +72,18 @@
 00000470: 0b64 5164 3664 3784 045a 0c64 5264 5364  .dQd6d7..Z.dRdSd
 00000480: 3a64 3b84 055a 0d65 0e65 0f6a 1083 0164  :d;..Z.e.e.j...d
 00000490: 5464 3d64 3e84 0483 015a 1165 0e65 126a  Td=d>....Z.e.e.j
 000004a0: 1383 0164 5564 4064 4184 0483 015a 1464  ...dUd@dA....Z.d
 000004b0: 5664 4364 4484 045a 1564 5764 4964 4a84  VdCdD..Z.dWdIdJ.
 000004c0: 045a 1664 5664 4b64 4c84 045a 1787 0004  .Z.dVdKdL..Z....
 000004d0: 005a 1853 0029 58da 0e43 6f6d 6d61 6e64  .Z.S.)X..Command
-000004e0: 4275 696c 6465 723e 0300 0000 fa13 636f  Builder>......co
-000004f0: 6d6d 616e 642d 6e61 6d65 2d73 796e 7461  mmand-name-synta
-00000500: 78fa 0e76 6572 7369 6f6e 2d73 7472 696e  x..version-strin
-00000510: 67da 0670 726f 6d70 747a 0663 7472 6c2b  g..promptz.ctrl+
+000004e0: 4275 696c 6465 723e 0300 0000 fa0e 7665  Builder>......ve
+000004f0: 7273 696f 6e2d 7374 7269 6e67 da06 7072  rsion-string..pr
+00000500: 6f6d 7074 fa13 636f 6d6d 616e 642d 6e61  ompt..command-na
+00000510: 6d65 2d73 796e 7461 787a 0663 7472 6c2b  me-syntaxz.ctrl+
 00000520: 725a 0d63 6c6f 7365 5f61 6e64 5f72 756e  rZ.close_and_run
 00000530: 7a0b 5275 6e20 436f 6d6d 616e 6429 03da  z.Run Command)..
 00000540: 036b 6579 da06 6163 7469 6f6e da0b 6465  .key..action..de
 00000550: 7363 7269 7074 696f 6e7a 0663 7472 6c2b  scriptionz.ctrl+
 00000560: 795a 1363 6f70 795f 636f 6d6d 616e 645f  yZ.copy_command_
 00000570: 7374 7269 6e67 7a0c 436f 7079 2043 6f6d  stringz.Copy Com
 00000580: 6d61 6e64 7a0d 6374 726c 2b74 2c65 7363  mandz.ctrl+t,esc
@@ -144,15 +144,15 @@
 000008f0: 640d 8301 640f 6408 8d02 7d07 640a 7c07  d...d.d...}.d.|.
 00000900: 5f0e 7c07 5600 0100 740d 7411 740f 640d  _.|.V...t.t.t.d.
 00000910: 6410 6408 8d02 6411 6408 8d02 6412 6408  d.d...d.d...d.d.
 00000920: 8d02 5600 0100 5700 6400 0400 0400 8303  ..V...W.d.......
 00000930: 0100 6e08 3100 7391 7701 0100 0100 0100  ..n.1.s.w.......
 00000940: 5900 0100 7412 8300 5600 0100 6400 5300  Y...t...V...d.S.
 00000950: 2913 4e5a 0843 6f6d 6d61 6e64 73da 0162  ).NZ.Commands..b
-00000960: 2901 da05 7374 796c 6572 2b00 0000 da01  )...styler+.....
+00000960: 2901 da05 7374 796c 6572 2a00 0000 da01  )...styler*.....
 00000970: 0ada 0176 7a13 686f 6d65 2d63 6f6d 6d61  ...vz.home-comma
 00000980: 6e64 732d 6c61 6265 6c29 0172 3d00 0000  nds-label).r=...
 00000990: 7a0c 686f 6d65 2d73 6964 6562 6172 467a  z.home-sidebarFz
 000009a0: 0968 6f6d 652d 626f 6479 7a22 686f 6d65  .home-bodyz"home
 000009b0: 2d63 6f6d 6d61 6e64 2d64 6573 6372 6970  -command-descrip
 000009c0: 7469 6f6e 2d63 6f6e 7461 696e 6572 da00  tion-container..
 000009d0: 7a18 686f 6d65 2d63 6f6d 6d61 6e64 2d64  z.home-command-d
@@ -379,15 +379,15 @@
 000017a0: 017d 0774 02a0 0564 057c 0766 027c 06a1  .}.t...d.|.f.|..
 000017b0: 027d 087c 00a0 0764 0674 08a1 02a0 097c  .}.|...d.t.....|
 000017c0: 08a1 0101 0064 0153 0064 0153 0029 077a  .....d.S.d.S.).z
 000017d0: 4055 7064 6174 6520 7468 6520 7072 6576  @Update the prev
 000017e0: 6965 7720 626f 7820 7368 6f77 696e 6720  iew box showing 
 000017f0: 7468 6520 636f 6d6d 616e 6420 7374 7269  the command stri
 00001800: 6e67 2074 6f20 6265 2065 7865 6375 7465  ng to be execute
-00001810: 644e 722a 0000 0072 6500 0000 722c 0000  dNr*...re...r,..
+00001810: 644e 722c 0000 0072 6500 0000 722b 0000  dNr,...re...r+..
 00001820: 007a 0224 207a 1923 686f 6d65 2d65 7865  .z.$ z.#home-exe
 00001830: 632d 7072 6576 6965 772d 7374 6174 6963  c-preview-static
 00001840: 290a 7242 0000 0072 5000 0000 720b 0000  ).rB...rP...r...
 00001850: 0072 3600 0000 725a 0000 0072 5200 0000  .r6...rZ...rR...
 00001860: 7244 0000 0072 7f00 0000 721a 0000 0072  rD...r....r....r
 00001870: 8e00 0000 2909 7245 0000 0072 8f00 0000  ....).rE...r....
 00001880: 7242 0000 005a 1963 6f6d 6d61 6e64 5f6e  rB...Z.command_n
```

### Comparing `argparse-tui-0.1.0/src/argparse_tui/argparse.py` & `argparse-tui-0.1.1/src/argparse_tui/argparse.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,14 +237,15 @@
         help: help message for the argument
 
     Examples:
         >>> import argparse
         >>> from argparse_tui import add_tui_argument
         ...
         >>> parser = argparse.ArgumentParser()
+        ...
         >>> add_tui_argument(parser)
         ...
         >>> parser.print_usage()
         usage: __main__.py [-h] [--tui [CMD]]
     """
     if not option_strings:
         option_strings = [f"--{DEFAULT_COMMAND_NAME.replace('_', '-').lstrip('-')}"]
@@ -258,15 +259,15 @@
         default=default,
         help=help,
         **kwargs,
     )
 
 
 def add_tui_command(
-    parser: argparse.ArgumentParser | argparse._SubParsersAction,
+    parser: argparse.ArgumentParser,
     command: str = DEFAULT_COMMAND_NAME,
     help: str = "Open Textual UI.",
 ) -> None:
     """
 
     Args:
         parser: the argparse parser
@@ -274,39 +275,29 @@
         help: help message for the argument
 
     Examples:
         >>> import argparse
         >>> from argparse_tui import add_tui_argument
         ...
         >>> parser = argparse.ArgumentParser()
-        >>> add_tui_command(parser)
-        ...
-        >>> parser.print_usage()
-        usage: __main__.py [-h] {tui} ...
-
-        >>> import argparse
-        >>> from argparse_tui import add_tui_argument
-        ...
-        >>> parser = argparse.ArgumentParser()
         >>> subparsers = parser.add_subparsers()
-        >>> add_tui_command(subparsers)
+        ...
+        >>> add_tui_command(parser)
         ...
         >>> parser.print_usage()
         usage: __main__.py [-h] {tui} ...
     """
+
     subparsers: argparse._SubParsersAction
-    if isinstance(parser, argparse._SubParsersAction):
-        subparsers = parser
+    for action in parser._actions:
+        if isinstance(action, argparse._SubParsersAction):
+            subparsers = action
+            break
     else:
-        for action in parser._actions:
-            if isinstance(action, argparse._SubParsersAction):
-                subparsers = action
-                break
-        else:
-            subparsers = parser.add_subparsers()
+        subparsers = parser.add_subparsers()
 
     tui_parser = subparsers.add_parser(
         command,
         description=argparse.SUPPRESS,
         help=help,
     )
     tui_parser.set_defaults(_parent_parser=parser)
```

### Comparing `argparse-tui-0.1.0/src/argparse_tui/detect_run_string.py` & `argparse-tui-0.1.1/src/argparse_tui/detect_run_string.py`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.0/src/argparse_tui/run_command.py` & `argparse-tui-0.1.1/src/argparse_tui/run_command.py`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.0/src/argparse_tui/schemas.py` & `argparse-tui-0.1.1/src/argparse_tui/schemas.py`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.0/src/argparse_tui/tui.py` & `argparse-tui-0.1.1/src/argparse_tui/tui.py`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.0/src/argparse_tui/tui.scss` & `argparse-tui-0.1.1/src/argparse_tui/tui.scss`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.0/src/argparse_tui/widgets/__pycache__/about.cpython-310.pyc` & `argparse-tui-0.1.1/src/argparse_tui/widgets/__pycache__/about.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jul 23 04:25:40 2023 UTC, .py size: 2647 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c4ab bc64 570a 0000  o..........dW...
+00000000: 6f0d 0d0a 0000 0000 ddf6 bd64 570a 0000  o..........dW...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 9800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 0100 6401  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6401 6406 6c0b  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6401 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `argparse-tui-0.1.0/src/argparse_tui/widgets/__pycache__/command_info.cpython-310.pyc` & `argparse-tui-0.1.1/src/argparse_tui/widgets/__pycache__/command_info.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jul 23 04:25:40 2023 UTC, .py size: 4010 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c4ab bc64 aa0f 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 ddf6 bd64 aa0f 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 ac00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6400 6406 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6400 6407 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `argparse-tui-0.1.0/src/argparse_tui/widgets/__pycache__/command_tree.cpython-310.pyc` & `argparse-tui-0.1.1/src/argparse_tui/widgets/__pycache__/command_tree.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jul 23 04:25:40 2023 UTC, .py size: 2246 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c4ab bc64 c608 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 ddf6 bd64 c608 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0173 7800 0000 6400  .....@...sx...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 6d0d 5a0d 0100 6407  d.l.m.Z.m.Z...d.
```

### Comparing `argparse-tui-0.1.0/src/argparse_tui/widgets/__pycache__/form.cpython-310.pyc` & `argparse-tui-0.1.1/src/argparse_tui/widgets/__pycache__/form.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jul 23 04:25:40 2023 UTC, .py size: 8067 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c4ab bc64 831f 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 ddf6 bd64 831f 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 c400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c03 6d04 5a04 0100 6400  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 0100 6400 6406 6c0a  m.Z.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6400 6407 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `argparse-tui-0.1.0/src/argparse_tui/widgets/__pycache__/multiple_choice.cpython-310.pyc` & `argparse-tui-0.1.1/src/argparse_tui/widgets/__pycache__/multiple_choice.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jul 23 04:25:40 2023 UTC, .py size: 2857 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c4ab bc64 290b 0000  o..........d)...
+00000000: 6f0d 0d0a 0000 0000 ddf6 bd64 290b 0000  o..........d)...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0173 a800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 6d0d 5a0d 0100 6400  d.l.m.Z.m.Z...d.
```

### Comparing `argparse-tui-0.1.0/src/argparse_tui/widgets/__pycache__/parameter_controls.cpython-310.pyc` & `argparse-tui-0.1.1/src/argparse_tui/widgets/__pycache__/parameter_controls.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jul 23 04:25:40 2023 UTC, .py size: 16529 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c4ab bc64 9140 0000  o..........d.@..
+00000000: 6f0d 0d0a 0000 0000 ddf6 bd64 9140 0000  o..........d.@..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0173 3601 0000 5500  .....@...s6...U.
 00000030: 6400 6401 6c00 6d01 5a01 0100 6400 6402  d.d.l.m.Z...d.d.
 00000040: 6c02 5a02 6400 6403 6c02 6d03 5a03 0100  l.Z.d.d.l.m.Z...
 00000050: 6400 6404 6c04 6d05 5a05 6d06 5a06 6d07  d.d.l.m.Z.m.Z.m.
 00000060: 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b  Z.m.Z.m.Z.m.Z.m.
 00000070: 5a0b 0100 6400 6405 6c0c 6d0d 5a0d 0100  Z...d.d.l.m.Z...
```

### Comparing `argparse-tui-0.1.0/src/argparse_tui/widgets/about.py` & `argparse-tui-0.1.1/src/argparse_tui/widgets/about.py`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.0/src/argparse_tui/widgets/command_info.py` & `argparse-tui-0.1.1/src/argparse_tui/widgets/command_info.py`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.0/src/argparse_tui/widgets/command_tree.py` & `argparse-tui-0.1.1/src/argparse_tui/widgets/command_tree.py`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.0/src/argparse_tui/widgets/form.py` & `argparse-tui-0.1.1/src/argparse_tui/widgets/form.py`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.0/src/argparse_tui/widgets/multiple_choice.py` & `argparse-tui-0.1.1/src/argparse_tui/widgets/multiple_choice.py`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.0/src/argparse_tui/widgets/parameter_controls.py` & `argparse-tui-0.1.1/src/argparse_tui/widgets/parameter_controls.py`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.0/src/argparse_tui.egg-info/PKG-INFO` & `argparse-tui-0.1.1/src/argparse_tui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argparse-tui
-Version: 0.1.0
+Version: 0.1.1
 Summary: Display your Python argparse CLI as a TUI.
 Author-email: Donald Mellenbruch <hello@f2dv.com>
 License: Copyright 2023 Donald Mellenbruch
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `argparse-tui-0.1.0/src/argparse_tui.egg-info/SOURCES.txt` & `argparse-tui-0.1.1/src/argparse_tui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.0/src/argparse_tui.egg-info/requires.txt` & `argparse-tui-0.1.1/src/argparse_tui.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.0/tests/test_help_argparse.py` & `argparse-tui-0.1.1/tests/test_help_argparse.py`

 * *Files identical despite different names*

### Comparing `argparse-tui-0.1.0/tests/test_run_command.py` & `argparse-tui-0.1.1/tests/test_run_command.py`

 * *Files identical despite different names*

