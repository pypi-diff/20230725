# Comparing `tmp/hirmeos_access_logs_local_driver-0.0.2.tar.gz` & `tmp/hirmeos_access_logs_local_driver-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hirmeos_access_logs_local_driver-0.0.2.tar", last modified: Tue Jul 25 09:59:43 2023, max compression
+gzip compressed data, was "hirmeos_access_logs_local_driver-0.0.3.tar", last modified: Tue Jul 25 16:03:42 2023, max compression
```

## Comparing `hirmeos_access_logs_local_driver-0.0.2.tar` & `hirmeos_access_logs_local_driver-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 cristiangarcia  (1000) cristiangarcia  (1000)        0 2023-07-25 09:59:43.588839 hirmeos_access_logs_local_driver-0.0.2/
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     1074 2023-07-24 14:23:34.000000 hirmeos_access_logs_local_driver-0.0.2/LICENSE
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     1454 2023-07-25 09:59:43.584839 hirmeos_access_logs_local_driver-0.0.2/PKG-INFO
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)      950 2023-07-12 11:39:02.000000 hirmeos_access_logs_local_driver-0.0.2/README.rst
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)      600 2023-07-25 09:59:12.000000 hirmeos_access_logs_local_driver-0.0.2/pyproject.toml
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)       38 2023-07-25 09:59:43.588839 hirmeos_access_logs_local_driver-0.0.2/setup.cfg
-drwxrwxr-x   0 cristiangarcia  (1000) cristiangarcia  (1000)        0 2023-07-25 09:59:43.576839 hirmeos_access_logs_local_driver-0.0.2/src/
-drwxrwxr-x   0 cristiangarcia  (1000) cristiangarcia  (1000)        0 2023-07-25 09:59:43.580839 hirmeos_access_logs_local_driver-0.0.2/src/hirmeos_access_logs_local_driver/
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)       78 2023-07-25 09:10:45.000000 hirmeos_access_logs_local_driver-0.0.2/src/hirmeos_access_logs_local_driver/__init__.py
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     1280 2023-07-23 16:32:43.000000 hirmeos_access_logs_local_driver-0.0.2/src/hirmeos_access_logs_local_driver/geolookup.py
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     9513 2023-07-24 15:19:47.000000 hirmeos_access_logs_local_driver-0.0.2/src/hirmeos_access_logs_local_driver/logdata.py
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)      996 2023-07-24 15:18:59.000000 hirmeos_access_logs_local_driver-0.0.2/src/hirmeos_access_logs_local_driver/process_download_logs.py
-drwxrwxr-x   0 cristiangarcia  (1000) cristiangarcia  (1000)        0 2023-07-25 09:59:43.584839 hirmeos_access_logs_local_driver-0.0.2/src/hirmeos_access_logs_local_driver.egg-info/
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     1454 2023-07-25 09:59:43.000000 hirmeos_access_logs_local_driver-0.0.2/src/hirmeos_access_logs_local_driver.egg-info/PKG-INFO
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)      540 2023-07-25 09:59:43.000000 hirmeos_access_logs_local_driver-0.0.2/src/hirmeos_access_logs_local_driver.egg-info/SOURCES.txt
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)        1 2023-07-25 09:59:43.000000 hirmeos_access_logs_local_driver-0.0.2/src/hirmeos_access_logs_local_driver.egg-info/dependency_links.txt
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)       33 2023-07-25 09:59:43.000000 hirmeos_access_logs_local_driver-0.0.2/src/hirmeos_access_logs_local_driver.egg-info/top_level.txt
-drwxrwxr-x   0 cristiangarcia  (1000) cristiangarcia  (1000)        0 2023-07-25 09:59:43.584839 hirmeos_access_logs_local_driver-0.0.2/tests/
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)    29554 2023-07-25 09:33:31.000000 hirmeos_access_logs_local_driver-0.0.2/tests/test_logdata.py
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     4323 2023-07-25 09:10:45.000000 hirmeos_access_logs_local_driver-0.0.2/tests/test_process_download_logs.py
+drwxrwxr-x   0 cristiangarcia  (1000) cristiangarcia  (1000)        0 2023-07-25 16:03:42.124421 hirmeos_access_logs_local_driver-0.0.3/
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     1184 2023-07-25 15:41:05.000000 hirmeos_access_logs_local_driver-0.0.3/LICENSE
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     1473 2023-07-25 16:03:42.124421 hirmeos_access_logs_local_driver-0.0.3/PKG-INFO
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)      972 2023-07-25 15:43:15.000000 hirmeos_access_logs_local_driver-0.0.3/README.rst
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)      647 2023-07-25 15:54:46.000000 hirmeos_access_logs_local_driver-0.0.3/pyproject.toml
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)       38 2023-07-25 16:03:42.124421 hirmeos_access_logs_local_driver-0.0.3/setup.cfg
+drwxrwxr-x   0 cristiangarcia  (1000) cristiangarcia  (1000)        0 2023-07-25 16:03:42.120421 hirmeos_access_logs_local_driver-0.0.3/src/
+drwxrwxr-x   0 cristiangarcia  (1000) cristiangarcia  (1000)        0 2023-07-25 16:03:42.120421 hirmeos_access_logs_local_driver-0.0.3/src/hirmeos_access_logs_local_driver/
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)       79 2023-07-25 14:15:55.000000 hirmeos_access_logs_local_driver-0.0.3/src/hirmeos_access_logs_local_driver/__init__.py
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     1280 2023-07-23 16:32:43.000000 hirmeos_access_logs_local_driver-0.0.3/src/hirmeos_access_logs_local_driver/geolookup.py
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     9513 2023-07-24 15:19:47.000000 hirmeos_access_logs_local_driver-0.0.3/src/hirmeos_access_logs_local_driver/logdata.py
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)      996 2023-07-24 15:18:59.000000 hirmeos_access_logs_local_driver-0.0.3/src/hirmeos_access_logs_local_driver/process_download_logs.py
+drwxrwxr-x   0 cristiangarcia  (1000) cristiangarcia  (1000)        0 2023-07-25 16:03:42.120421 hirmeos_access_logs_local_driver-0.0.3/src/hirmeos_access_logs_local_driver.egg-info/
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     1473 2023-07-25 16:03:42.000000 hirmeos_access_logs_local_driver-0.0.3/src/hirmeos_access_logs_local_driver.egg-info/PKG-INFO
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)      599 2023-07-25 16:03:42.000000 hirmeos_access_logs_local_driver-0.0.3/src/hirmeos_access_logs_local_driver.egg-info/SOURCES.txt
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)        1 2023-07-25 16:03:42.000000 hirmeos_access_logs_local_driver-0.0.3/src/hirmeos_access_logs_local_driver.egg-info/dependency_links.txt
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)       23 2023-07-25 16:03:42.000000 hirmeos_access_logs_local_driver-0.0.3/src/hirmeos_access_logs_local_driver.egg-info/requires.txt
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)       33 2023-07-25 16:03:42.000000 hirmeos_access_logs_local_driver-0.0.3/src/hirmeos_access_logs_local_driver.egg-info/top_level.txt
+drwxrwxr-x   0 cristiangarcia  (1000) cristiangarcia  (1000)        0 2023-07-25 16:03:42.124421 hirmeos_access_logs_local_driver-0.0.3/tests/
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)    29554 2023-07-25 09:33:31.000000 hirmeos_access_logs_local_driver-0.0.3/tests/test_logdata.py
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     4280 2023-07-25 10:47:58.000000 hirmeos_access_logs_local_driver-0.0.3/tests/test_process_download_logs.py
```

### Comparing `hirmeos_access_logs_local_driver-0.0.2/LICENSE` & `hirmeos_access_logs_local_driver-0.0.3/LICENSE`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,11 @@
-Copyright (c) 2018 The Python Packaging Authority
+MIT License
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
+Copyright (c) 2018, Open Book Publishers.
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
+This code builds upon previous effort by Open Book Publishers, and is used under the following license:
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `hirmeos_access_logs_local_driver-0.0.2/PKG-INFO` & `hirmeos_access_logs_local_driver-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: hirmeos_access_logs_local_driver
-Version: 0.0.2
+Version: 0.0.3
 Summary: Functions required by the access-logs-local-driver
 Author-email: Cristian Garcia <cristian.garcia@ubiquitypress.com>
 Project-URL: Homepage, https://github.com/hirmeos/access_logs_driver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10.6
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 # Access Logs Driver
 [![Build Status](https://travis-ci.org/hirmeos/access_logs_driver.svg?branch=master)](https://travis-ci.org/hirmeos/access_logs_driver)
 
 
@@ -25,14 +25,15 @@
 a URL within the last `SESSION_TIMEOUT` (e.g. half-hour)
 
 Additionally, we convert the URLs to ISBNs and collate request data by date,
 outputting a CSV for ingest via the stats system.
 
 Release Notes:
 [0.0.2] - 2023-07-11
+[0.0.3] - 2023-07-25
 
 Added:
     * Unittests
 
 Changed:
     * Moved the files out of the package and get the file's data as parameters and return the filtered data.
     * renamed the plugin to access-logs-local
```

### Comparing `hirmeos_access_logs_local_driver-0.0.2/README.rst` & `hirmeos_access_logs_local_driver-0.0.3/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 a URL within the last `SESSION_TIMEOUT` (e.g. half-hour)
 
 Additionally, we convert the URLs to ISBNs and collate request data by date,
 outputting a CSV for ingest via the stats system.
 
 Release Notes:
 [0.0.2] - 2023-07-11
+[0.0.3] - 2023-07-25
 
 Added:
     * Unittests
 
 Changed:
     * Moved the files out of the package and get the file's data as parameters and return the filtered data.
-    * renamed the plugin to access-logs-local
+    * renamed the plugin to access-logs-local
```

### Comparing `hirmeos_access_logs_local_driver-0.0.2/pyproject.toml` & `hirmeos_access_logs_local_driver-0.0.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hirmeos_access_logs_local_driver"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Cristian Garcia", email="cristian.garcia@ubiquitypress.com" },
 ]
 description = "Functions required by the access-logs-local-driver"
 readme = "README.rst" 
-requires-python = ">=3.10.6"
+requires-python = ">=3.10"
+dependencies = [
+  "hirmeos-clients >= 0.1.6",
+]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `hirmeos_access_logs_local_driver-0.0.2/src/hirmeos_access_logs_local_driver/geolookup.py` & `hirmeos_access_logs_local_driver-0.0.3/src/hirmeos_access_logs_local_driver/geolookup.py`

 * *Files identical despite different names*

### Comparing `hirmeos_access_logs_local_driver-0.0.2/src/hirmeos_access_logs_local_driver/logdata.py` & `hirmeos_access_logs_local_driver-0.0.3/src/hirmeos_access_logs_local_driver/logdata.py`

 * *Files identical despite different names*

### Comparing `hirmeos_access_logs_local_driver-0.0.2/src/hirmeos_access_logs_local_driver/process_download_logs.py` & `hirmeos_access_logs_local_driver-0.0.3/src/hirmeos_access_logs_local_driver/process_download_logs.py`

 * *Files identical despite different names*

### Comparing `hirmeos_access_logs_local_driver-0.0.2/src/hirmeos_access_logs_local_driver.egg-info/PKG-INFO` & `hirmeos_access_logs_local_driver-0.0.3/src/hirmeos_access_logs_local_driver.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: hirmeos-access-logs-local-driver
-Version: 0.0.2
+Version: 0.0.3
 Summary: Functions required by the access-logs-local-driver
 Author-email: Cristian Garcia <cristian.garcia@ubiquitypress.com>
 Project-URL: Homepage, https://github.com/hirmeos/access_logs_driver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10.6
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 # Access Logs Driver
 [![Build Status](https://travis-ci.org/hirmeos/access_logs_driver.svg?branch=master)](https://travis-ci.org/hirmeos/access_logs_driver)
 
 
@@ -25,14 +25,15 @@
 a URL within the last `SESSION_TIMEOUT` (e.g. half-hour)
 
 Additionally, we convert the URLs to ISBNs and collate request data by date,
 outputting a CSV for ingest via the stats system.
 
 Release Notes:
 [0.0.2] - 2023-07-11
+[0.0.3] - 2023-07-25
 
 Added:
     * Unittests
 
 Changed:
     * Moved the files out of the package and get the file's data as parameters and return the filtered data.
     * renamed the plugin to access-logs-local
```

### Comparing `hirmeos_access_logs_local_driver-0.0.2/src/hirmeos_access_logs_local_driver.egg-info/SOURCES.txt` & `hirmeos_access_logs_local_driver-0.0.3/src/hirmeos_access_logs_local_driver.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,10 +4,11 @@
 src/hirmeos_access_logs_local_driver/__init__.py
 src/hirmeos_access_logs_local_driver/geolookup.py
 src/hirmeos_access_logs_local_driver/logdata.py
 src/hirmeos_access_logs_local_driver/process_download_logs.py
 src/hirmeos_access_logs_local_driver.egg-info/PKG-INFO
 src/hirmeos_access_logs_local_driver.egg-info/SOURCES.txt
 src/hirmeos_access_logs_local_driver.egg-info/dependency_links.txt
+src/hirmeos_access_logs_local_driver.egg-info/requires.txt
 src/hirmeos_access_logs_local_driver.egg-info/top_level.txt
 tests/test_logdata.py
 tests/test_process_download_logs.py
```

### Comparing `hirmeos_access_logs_local_driver-0.0.2/tests/test_logdata.py` & `hirmeos_access_logs_local_driver-0.0.3/tests/test_logdata.py`

 * *Files identical despite different names*

### Comparing `hirmeos_access_logs_local_driver-0.0.2/tests/test_process_download_logs.py` & `hirmeos_access_logs_local_driver-0.0.3/tests/test_process_download_logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from unittest import TestCase
 from requests.models import Response
-from drivers.access_logs_local.access_logs_local_driver.src.access_logs_local_driver.process_download_logs import (
+from src.hirmeos_access_logs_local_driver.process_download_logs import (
     make_filters,
     method_ok,
     no_plus_http,
     no_star,
     only_successful,
 )
```

