# Comparing `tmp/easyID3-0.0.9.tar.gz` & `tmp/easyID3-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyID3-0.0.9.tar", last modified: Sun May 15 15:37:17 2022, max compression
+gzip compressed data, was "easyID3-0.1.1.tar", last modified: Tue Jul 25 03:24:13 2023, max compression
```

## Comparing `easyID3-0.0.9.tar` & `easyID3-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxrwxrwx   0        0        0        0 2022-05-15 15:37:17.596164 easyID3-0.0.9/
--rw-rw-rw-   0        0        0     1091 2022-05-12 20:31:52.000000 easyID3-0.0.9/LICENSE.txt
--rw-rw-rw-   0        0        0      899 2022-05-15 15:37:17.596164 easyID3-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      461 2022-05-13 22:44:43.000000 easyID3-0.0.9/README.md
--rw-rw-rw-   0        0        0       86 2022-05-12 20:38:07.000000 easyID3-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0      570 2022-05-15 15:37:17.613599 easyID3-0.0.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-05-15 15:37:17.496377 easyID3-0.0.9/src/
-drwxrwxrwx   0        0        0        0 2022-05-15 15:37:17.543249 easyID3-0.0.9/src/easyID3/
--rw-rw-rw-   0        0        0     4255 2022-05-15 15:34:25.000000 easyID3-0.0.9/src/easyID3/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-15 15:37:17.594128 easyID3-0.0.9/src/easyID3.egg-info/
--rw-rw-rw-   0        0        0      899 2022-05-15 15:37:16.000000 easyID3-0.0.9/src/easyID3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2022-05-15 15:37:17.000000 easyID3-0.0.9/src/easyID3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-15 15:37:16.000000 easyID3-0.0.9/src/easyID3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-05-15 15:37:17.000000 easyID3-0.0.9/src/easyID3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 03:24:13.740043 easyID3-0.1.1/
+-rw-rw-rw-   0        0        0     1090 2023-07-24 20:54:59.000000 easyID3-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      214 2023-07-25 03:24:13.740043 easyID3-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-07-25 03:09:08.000000 easyID3-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 03:24:13.739042 easyID3-0.1.1/easyID3.egg-info/
+-rw-rw-rw-   0        0        0      214 2023-07-25 03:24:13.000000 easyID3-0.1.1/easyID3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2023-07-25 03:24:13.000000 easyID3-0.1.1/easyID3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 03:24:13.000000 easyID3-0.1.1/easyID3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-25 03:24:13.000000 easyID3-0.1.1/easyID3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 03:24:13.000000 easyID3-0.1.1/easyID3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 03:24:13.740043 easyID3-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      352 2023-07-25 03:23:03.000000 easyID3-0.1.1/setup.py
```

### Comparing `easyID3-0.0.9/LICENSE.txt` & `easyID3-0.1.1/LICENSE`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-Copyright (c) 2018 The Python Packaging Authority
+MIT License
+
+Copyright (c) 2022 jonathanoren
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -12,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

