# Comparing `tmp/pc_mouseparty-0.0.1.tar.gz` & `tmp/pc_mouseparty-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pc_mouseparty-0.0.1.tar", last modified: Tue Jul 25 17:08:03 2023, max compression
+gzip compressed data, was "pc_mouseparty-0.1.1.tar", last modified: Tue Jul 25 19:59:21 2023, max compression
```

## Comparing `pc_mouseparty-0.0.1.tar` & `pc_mouseparty-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 17:08:03.995634 pc_mouseparty-0.0.1/
--rw-rw-rw-   0        0        0      184 2023-07-25 16:36:28.000000 pc_mouseparty-0.0.1/AUTHORS.rst
--rw-rw-rw-   0        0        0     1099 2023-07-25 16:36:28.000000 pc_mouseparty-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      129 2023-07-25 16:36:28.000000 pc_mouseparty-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1475 2023-07-25 17:08:03.995634 pc_mouseparty-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      637 2023-07-25 16:36:28.000000 pc_mouseparty-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 17:08:03.983090 pc_mouseparty-0.0.1/pc_mouseparty/
--rw-rw-rw-   0        0        0      151 2023-07-25 16:36:28.000000 pc_mouseparty-0.0.1/pc_mouseparty/__init__.py
--rw-rw-rw-   0        0        0      473 2023-07-25 16:36:28.000000 pc_mouseparty-0.0.1/pc_mouseparty/cli.py
--rw-rw-rw-   0        0        0      194 2023-07-25 16:36:28.000000 pc_mouseparty-0.0.1/pc_mouseparty/common.py
--rw-rw-rw-   0        0        0       18 2023-07-25 16:42:42.000000 pc_mouseparty-0.0.1/pc_mouseparty/pc_mouseparty.py
-drwxrwxrwx   0        0        0        0 2023-07-25 17:08:03.995634 pc_mouseparty-0.0.1/pc_mouseparty.egg-info/
--rw-rw-rw-   0        0        0     1475 2023-07-25 17:08:03.000000 pc_mouseparty-0.0.1/pc_mouseparty.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      403 2023-07-25 17:08:03.000000 pc_mouseparty-0.0.1/pc_mouseparty.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 17:08:03.000000 pc_mouseparty-0.0.1/pc_mouseparty.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-25 17:08:03.000000 pc_mouseparty-0.0.1/pc_mouseparty.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-07-25 17:08:03.000000 pc_mouseparty-0.0.1/pc_mouseparty.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2023-07-25 17:08:03.000000 pc_mouseparty-0.0.1/pc_mouseparty.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-07-25 16:36:28.000000 pc_mouseparty-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0      484 2023-07-25 17:08:03.996632 pc_mouseparty-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1989 2023-07-25 16:36:28.000000 pc_mouseparty-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:59:21.896717 pc_mouseparty-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-25 19:59:03.000000 pc_mouseparty-0.1.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-25 19:59:03.000000 pc_mouseparty-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-25 19:59:03.000000 pc_mouseparty-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-25 19:59:21.896717 pc_mouseparty-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-25 19:59:03.000000 pc_mouseparty-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:59:21.896717 pc_mouseparty-0.1.1/pc_mouseparty/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-25 19:59:03.000000 pc_mouseparty-0.1.1/pc_mouseparty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-25 19:59:03.000000 pc_mouseparty-0.1.1/pc_mouseparty/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-25 19:59:03.000000 pc_mouseparty-0.1.1/pc_mouseparty/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-25 19:59:03.000000 pc_mouseparty-0.1.1/pc_mouseparty/pc_mouseparty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:59:21.896717 pc_mouseparty-0.1.1/pc_mouseparty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-25 19:59:21.000000 pc_mouseparty-0.1.1/pc_mouseparty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-25 19:59:21.000000 pc_mouseparty-0.1.1/pc_mouseparty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:59:21.000000 pc_mouseparty-0.1.1/pc_mouseparty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-25 19:59:21.000000 pc_mouseparty-0.1.1/pc_mouseparty.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:59:21.000000 pc_mouseparty-0.1.1/pc_mouseparty.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 19:59:21.000000 pc_mouseparty-0.1.1/pc_mouseparty.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:59:03.000000 pc_mouseparty-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-25 19:59:21.896717 pc_mouseparty-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-25 19:59:03.000000 pc_mouseparty-0.1.1/setup.py
```

### Comparing `pc_mouseparty-0.0.1/LICENSE` & `pc_mouseparty-0.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-MIT License
-
-Copyright (c) 2023, Christopher Marais
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
+MIT License
+
+Copyright (c) 2023, Christopher Marais
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
```

