# Comparing `tmp/michina-0.1.0.tar.gz` & `tmp/michina-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "michina-0.1.0.tar", max compression
+gzip compressed data, was "michina-0.1.1.tar", max compression
```

## Comparing `michina-0.1.0.tar` & `michina-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,12 @@
--rw-r--r--   0        0        0       94 2023-07-24 18:14:49.101187 michina-0.1.0/README.md
--rw-r--r--   0        0        0      931 2023-07-24 21:41:33.336097 michina-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       21 2023-07-24 21:02:36.705292 michina-0.1.0/src/michina/__init__.py
--rw-r--r--   0        0        0      310 2023-07-24 18:35:05.155781 michina-0.1.0/src/michina/exceptions.py
--rw-r--r--   0        0        0     3877 2023-07-24 18:58:44.955732 michina-0.1.0/src/michina/isConsistent.py
--rw-r--r--   0        0        0       51 2023-07-24 18:51:40.448708 michina-0.1.0/src/michina/michina.py
--rw-r--r--   0        0        0     3644 2023-07-24 18:52:43.865441 michina-0.1.0/src/michina/toneCheck.py
--rw-r--r--   0        0        0      686 1970-01-01 00:00:00.000000 michina-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      146 2023-07-25 08:16:01.149793 michina-0.1.1/README.md
+-rw-r--r--   0        0        0      122 2023-07-25 00:01:47.195488 michina-0.1.1/michina/checks/__init__.py
+-rw-r--r--   0        0        0      238 2023-07-24 23:36:58.809362 michina-0.1.1/michina/checks/base_check.py
+-rw-r--r--   0        0        0      175 2023-07-25 00:01:47.195444 michina-0.1.1/michina/checks/consistency/__init__.py
+-rw-r--r--   0        0        0     1786 2023-07-25 00:01:47.195414 michina-0.1.1/michina/checks/consistency/check.py
+-rw-r--r--   0        0        0     2611 2023-07-24 23:08:42.323294 michina-0.1.1/michina/checks/consistency/prompt.py
+-rw-r--r--   0        0        0      140 2023-07-25 00:01:47.195530 michina-0.1.1/michina/checks/tone/__init__.py
+-rw-r--r--   0        0        0     1587 2023-07-25 00:01:47.195581 michina-0.1.1/michina/checks/tone/check.py
+-rw-r--r--   0        0        0     2397 2023-07-24 23:13:10.018714 michina-0.1.1/michina/checks/tone/prompt.py
+-rw-r--r--   0        0        0      310 2023-07-24 18:35:05.155781 michina-0.1.1/michina/exceptions/exceptions.py
+-rw-r--r--   0        0        0      469 2023-07-25 08:39:09.246042 michina-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 michina-0.1.1/PKG-INFO
```

### Comparing `michina-0.1.0/PKG-INFO` & `michina-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
 Name: michina
-Version: 0.1.0
+Version: 0.1.1
 Summary: Integ test framework for LLMs.
 Home-page: https://github.com/michina-ai/michina
 Author: bkitano
 Author-email: briankitano@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: build (>=0.10.0,<0.11.0)
-Requires-Dist: bumpver (>=2023.1125,<2024.0)
+Requires-Dist: langchain (>=0.0.240,<0.0.241)
+Requires-Dist: openai (>=0.27.8,<0.28.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: twine (>=4.0.2,<5.0.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Project-URL: Repository, https://github.com/michina-ai/michina
 Description-Content-Type: text/markdown
 
 # Michina
 From the quechua word for "pasture".
 
 Unit testing and integration testing for LLMs.
+
+## Todo
+- make it run on github via github actions
```

