# Comparing `tmp/eagleeyev3-0.0.6.tar.gz` & `tmp/eagleeyev3-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eagleeyev3-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "eagleeyev3-0.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `eagleeyev3-0.0.6.tar` & `eagleeyev3-0.0.7.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0      162 2023-07-20 15:43:05.663721 eagleeyev3-0.0.6/.gitignore
--rw-r--r--   0        0        0     1049 2023-07-18 18:55:59.571391 eagleeyev3-0.0.6/LICENSE
--rw-r--r--   0        0        0      375 2023-07-20 04:33:54.569165 eagleeyev3-0.0.6/README.md
--rw-r--r--   0        0        0      380 2023-07-20 15:33:42.589081 eagleeyev3-0.0.6/pyproject.toml
--rw-r--r--   0        0        0    27527 2023-07-24 20:58:26.689982 eagleeyev3-0.0.6/src/EagleEyev3/__init__.py
--rw-r--r--   0        0        0      533 2023-07-11 02:17:41.899184 eagleeyev3-0.0.6/src/EagleEyev3/settings.py
--rw-r--r--   0        0        0      670 1970-01-01 00:00:00.000000 eagleeyev3-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      162 2023-07-24 21:05:15.503728 eagleeyev3-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1049 2023-07-18 18:55:59.571391 eagleeyev3-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1126 2023-07-25 16:21:45.463775 eagleeyev3-0.0.7/README.md
+-rw-r--r--   0        0        0      380 2023-07-20 15:33:42.589081 eagleeyev3-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0    27503 2023-07-25 16:25:06.684769 eagleeyev3-0.0.7/src/EagleEyev3/__init__.py
+-rw-r--r--   0        0        0     1421 1970-01-01 00:00:00.000000 eagleeyev3-0.0.7/PKG-INFO
```

### Comparing `eagleeyev3-0.0.6/LICENSE` & `eagleeyev3-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `eagleeyev3-0.0.6/src/EagleEyev3/__init__.py` & `eagleeyev3-0.0.7/src/EagleEyev3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """ Python client for Eagle Eye Networks APIv3 """
-version = "0.0.6"
+version = "0.0.7"
 __version__ = version
 
 
 import json
 import logging
 import requests
-from .settings import *
 
 from datetime import datetime, timedelta
 from pytz import timezone
 
 from io import BytesIO
 
 logging.basicConfig(level=logging.INFO)
```

