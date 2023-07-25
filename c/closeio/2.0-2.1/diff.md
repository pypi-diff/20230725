# Comparing `tmp/closeio-2.0.tar.gz` & `tmp/closeio-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "closeio-2.0.tar", last modified: Thu Apr  7 13:44:11 2022, max compression
+gzip compressed data, was "closeio-2.1.tar", last modified: Tue Jul 25 17:51:37 2023, max compression
```

## Comparing `closeio-2.0.tar` & `closeio-2.1.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 alec       (501) staff       (20)        0 2022-04-07 13:44:11.551277 closeio-2.0/
--rw-r--r--   0 alec       (501) staff       (20)      585 2022-04-07 13:44:11.551389 closeio-2.0/PKG-INFO
--rw-r--r--   0 alec       (501) staff       (20)     2202 2022-04-06 12:56:39.000000 closeio-2.0/README.md
-drwxr-xr-x   0 alec       (501) staff       (20)        0 2022-04-07 13:44:11.550137 closeio-2.0/closeio.egg-info/
--rw-r--r--   0 alec       (501) staff       (20)      585 2022-04-07 13:44:11.000000 closeio-2.0/closeio.egg-info/PKG-INFO
--rw-r--r--   0 alec       (501) staff       (20)      227 2022-04-07 13:44:11.000000 closeio-2.0/closeio.egg-info/SOURCES.txt
--rw-r--r--   0 alec       (501) staff       (20)        1 2022-04-07 13:44:11.000000 closeio-2.0/closeio.egg-info/dependency_links.txt
--rw-r--r--   0 alec       (501) staff       (20)       17 2022-04-07 13:44:11.000000 closeio-2.0/closeio.egg-info/requires.txt
--rw-r--r--   0 alec       (501) staff       (20)       12 2022-04-07 13:44:11.000000 closeio-2.0/closeio.egg-info/top_level.txt
-drwxr-xr-x   0 alec       (501) staff       (20)        0 2022-04-07 13:44:11.550927 closeio-2.0/closeio_api/
--rw-r--r--   0 alec       (501) staff       (20)     8510 2022-04-06 20:21:19.000000 closeio-2.0/closeio_api/__init__.py
--rw-r--r--   0 alec       (501) staff       (20)      251 2022-04-06 12:56:39.000000 closeio-2.0/closeio_api/utils.py
--rw-r--r--   0 alec       (501) staff       (20)       71 2022-04-07 13:44:11.551755 closeio-2.0/setup.cfg
--rw-r--r--   0 alec       (501) staff       (20)      886 2022-04-06 20:21:19.000000 closeio-2.0/setup.py
+drwxr-xr-x   0 alec       (501) staff       (20)        0 2023-07-25 17:51:37.163015 closeio-2.1/
+-rw-r--r--   0 alec       (501) staff       (20)     1086 2023-07-20 13:56:58.000000 closeio-2.1/LICENSE
+-rw-r--r--   0 alec       (501) staff       (20)      538 2023-07-25 17:51:37.163067 closeio-2.1/PKG-INFO
+-rw-r--r--   0 alec       (501) staff       (20)     2202 2023-07-20 13:56:58.000000 closeio-2.1/README.md
+drwxr-xr-x   0 alec       (501) staff       (20)        0 2023-07-25 17:51:37.162372 closeio-2.1/closeio.egg-info/
+-rw-r--r--   0 alec       (501) staff       (20)      538 2023-07-25 17:51:37.000000 closeio-2.1/closeio.egg-info/PKG-INFO
+-rw-r--r--   0 alec       (501) staff       (20)      253 2023-07-25 17:51:37.000000 closeio-2.1/closeio.egg-info/SOURCES.txt
+-rw-r--r--   0 alec       (501) staff       (20)        1 2023-07-25 17:51:37.000000 closeio-2.1/closeio.egg-info/dependency_links.txt
+-rw-r--r--   0 alec       (501) staff       (20)       17 2023-07-25 17:51:37.000000 closeio-2.1/closeio.egg-info/requires.txt
+-rw-r--r--   0 alec       (501) staff       (20)       12 2023-07-25 17:51:37.000000 closeio-2.1/closeio.egg-info/top_level.txt
+drwxr-xr-x   0 alec       (501) staff       (20)        0 2023-07-25 17:51:37.162603 closeio-2.1/closeio_api/
+-rw-r--r--   0 alec       (501) staff       (20)     8992 2023-07-25 17:45:55.000000 closeio-2.1/closeio_api/__init__.py
+-rw-r--r--   0 alec       (501) staff       (20)      251 2023-07-20 13:56:58.000000 closeio-2.1/closeio_api/utils.py
+-rw-r--r--   0 alec       (501) staff       (20)       71 2023-07-25 17:51:37.163272 closeio-2.1/setup.cfg
+-rw-r--r--   0 alec       (501) staff       (20)      886 2023-07-20 13:56:58.000000 closeio-2.1/setup.py
+drwxr-xr-x   0 alec       (501) staff       (20)        0 2023-07-25 17:51:37.162796 closeio-2.1/tests/
+-rw-r--r--   0 alec       (501) staff       (20)     5056 2023-07-25 17:45:55.000000 closeio-2.1/tests/test_api.py
```

### Comparing `closeio-2.0/PKG-INFO` & `closeio-2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: closeio
-Version: 2.0
+Version: 2.1
 Summary: Close API Python Client
 Home-page: https://github.com/closeio/closeio-api/
 Author: Close Team
-Author-email: UNKNOWN
-License: UNKNOWN
-Description: Close API Python Client
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
+License-File: LICENSE
+
+Close API Python Client
```

### Comparing `closeio-2.0/README.md` & `closeio-2.1/README.md`

 * *Files identical despite different names*

### Comparing `closeio-2.0/closeio.egg-info/PKG-INFO` & `closeio-2.1/closeio.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: closeio
-Version: 2.0
+Version: 2.1
 Summary: Close API Python Client
 Home-page: https://github.com/closeio/closeio-api/
 Author: Close Team
-Author-email: UNKNOWN
-License: UNKNOWN
-Description: Close API Python Client
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
+License-File: LICENSE
+
+Close API Python Client
```

### Comparing `closeio-2.0/closeio_api/__init__.py` & `closeio-2.1/closeio_api/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import contextlib
 import logging
+import re
 import time
 
 from random import uniform
 
 import requests
 
 from closeio_api.utils import local_tz_offset
 
 DEFAULT_RATE_LIMIT_DELAY = 2   # Seconds
 
 # To update the package version, change this variable. This variable is also
 # read by setup.py when installing the package.
-__version__ = '2.0'
+__version__ = '2.1'
 
 class APIError(Exception):
     """Raised when sending a request to the API failed."""
 
     def __init__(self, response):
         # For compatibility purposes we can access the original string through
         # the args property.
@@ -143,15 +144,27 @@
             raise APIError(response)
 
     def _get_rate_limit_sleep_time(self, response):
         """Get rate limit window expiration time from response if the response
         status code is 429. 
         """
         with contextlib.suppress(KeyError):
+            rate_limit = response.headers["RateLimit"]
+            # we don't actually need all these values, but per the RFC:
+            # "Malformed RateLimit header fields MUST be ignored."
+            match = re.match(
+                r"limit=(\d+), remaining=(\d+), reset=(\d+)", rate_limit
+            )
+            if match:
+                limit, remaining, reset = match.groups()
+                return float(reset)
+
+        with contextlib.suppress(KeyError):
             return float(response.headers["Retry-After"])
+
         with contextlib.suppress(KeyError):
             return float(response.headers["RateLimit-Reset"])
 
         logging.exception('Error parsing rate limiting response')
         return DEFAULT_RATE_LIMIT_DELAY
 
     def _get_randomized_sleep_time_for_error(self, status_code, retries):
```

### Comparing `closeio-2.0/setup.py` & `closeio-2.1/setup.py`

 * *Files identical despite different names*

