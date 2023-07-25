# Comparing `tmp/odin_cyble-0.0.6.tar.gz` & `tmp/odin_cyble-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odin_cyble-0.0.6.tar", max compression
+gzip compressed data, was "odin_cyble-0.0.7.tar", max compression
```

## Comparing `odin_cyble-0.0.6.tar` & `odin_cyble-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,47 @@
--rw-r--r--   0        0        0     1073 2023-07-25 06:36:49.084746 odin_cyble-0.0.6/LICENSE
--rw-r--r--   0        0        0     1492 2023-07-25 08:13:29.982778 odin_cyble-0.0.6/README.md
--rw-r--r--   0        0        0      977 2023-07-25 11:02:14.876346 odin_cyble-0.0.6/odin/__init__.py
--rw-r--r--   0        0        0     3169 2023-07-25 06:16:06.492192 odin_cyble-0.0.6/odin/example.py
--rw-r--r--   0        0        0      483 2023-07-24 13:30:01.718847 odin_cyble-0.0.6/odin/exceptions.py
--rw-r--r--   0        0        0      845 2023-07-25 11:02:56.332833 odin_cyble-0.0.6/odin/models/__init__.py
--rw-r--r--   0        0        0     2823 2023-07-14 03:25:54.374435 odin_cyble-0.0.6/odin/models/certificate_search_response_model.py
--rw-r--r--   0        0        0      434 2023-07-12 05:06:57.147103 odin_cyble-0.0.6/odin/models/get_certificate_count.py
--rw-r--r--   0        0        0     7214 2023-07-12 05:30:11.746441 odin_cyble-0.0.6/odin/models/get_certificate_hash_details.py
--rw-r--r--   0        0        0      960 2023-07-12 05:30:16.127850 odin_cyble-0.0.6/odin/models/get_certificates_summary.py
--rw-r--r--   0        0        0      429 2023-07-12 04:48:26.964336 odin_cyble-0.0.6/odin/models/get_host_count.py
--rw-r--r--   0        0        0     6693 2023-07-12 04:49:22.181362 odin_cyble-0.0.6/odin/models/get_hosts_ip_details_response.py
--rw-r--r--   0        0        0      941 2023-07-12 05:04:30.079384 odin_cyble-0.0.6/odin/models/get_hosts_summary_response.py
--rw-r--r--   0        0        0     7419 2023-07-14 03:05:42.334035 odin_cyble-0.0.6/odin/models/search_hosts_response_model.py
--rw-r--r--   0        0        0     5945 2023-07-25 11:02:44.728376 odin_cyble-0.0.6/odin/odin_client.py
--rw-r--r--   0        0        0      327 2023-07-25 11:03:24.569140 odin_cyble-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1926 1970-01-01 00:00:00.000000 odin_cyble-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1490 2023-07-25 13:14:38.764176 odin_cyble-0.0.7/README.md
+-rw-r--r--   0        0        0      977 2023-07-25 11:02:14.876346 odin_cyble-0.0.7/odin/__init__.py
+-rw-r--r--   0        0        0      933 2023-07-12 13:16:47.000000 odin_cyble-0.0.7/odin/build/lib/models/__init__.py
+-rw-r--r--   0        0        0     2710 2023-07-12 05:31:11.000000 odin_cyble-0.0.7/odin/build/lib/models/certificate_search_response_model.py
+-rw-r--r--   0        0        0      434 2023-07-12 05:06:57.000000 odin_cyble-0.0.7/odin/build/lib/models/get_certificate_count.py
+-rw-r--r--   0        0        0     7214 2023-07-12 05:30:11.000000 odin_cyble-0.0.7/odin/build/lib/models/get_certificate_hash_details.py
+-rw-r--r--   0        0        0      960 2023-07-12 05:30:16.000000 odin_cyble-0.0.7/odin/build/lib/models/get_certificates_summary.py
+-rw-r--r--   0        0        0      429 2023-07-12 04:48:26.000000 odin_cyble-0.0.7/odin/build/lib/models/get_host_count.py
+-rw-r--r--   0        0        0     6693 2023-07-12 04:49:22.000000 odin_cyble-0.0.7/odin/build/lib/models/get_hosts_ip_details_response.py
+-rw-r--r--   0        0        0      941 2023-07-12 05:04:30.000000 odin_cyble-0.0.7/odin/build/lib/models/get_hosts_summary_response.py
+-rw-r--r--   0        0        0     7294 2023-07-12 04:57:14.000000 odin_cyble-0.0.7/odin/build/lib/models/search_hosts_response_model.py
+-rw-r--r--   0        0        0     3253 2023-07-25 12:33:22.352466 odin_cyble-0.0.7/odin/example.py
+-rw-r--r--   0        0        0      483 2023-07-24 13:30:01.718847 odin_cyble-0.0.7/odin/exceptions.py
+-rw-r--r--   0        0        0      845 2023-07-25 11:02:56.332833 odin_cyble-0.0.7/odin/models/__init__.py
+-rw-r--r--   0        0        0     1072 2023-07-25 11:43:04.241571 odin_cyble-0.0.7/odin/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6864 2023-07-12 05:31:17.693938 odin_cyble-0.0.7/odin/models/__pycache__/certificateSearchResponse.cpython-311.pyc
+-rw-r--r--   0        0        0     7148 2023-07-14 03:26:07.367970 odin_cyble-0.0.7/odin/models/__pycache__/certificate_search_response_model.cpython-311.pyc
+-rw-r--r--   0        0        0     1570 2023-07-12 05:17:26.235602 odin_cyble-0.0.7/odin/models/__pycache__/getCertificateCount.cpython-311.pyc
+-rw-r--r--   0        0        0    17993 2023-07-12 05:31:17.698223 odin_cyble-0.0.7/odin/models/__pycache__/getCertificateHashDetails.cpython-311.pyc
+-rw-r--r--   0        0        0     2858 2023-07-12 05:31:17.699481 odin_cyble-0.0.7/odin/models/__pycache__/getCertificatesSummary.cpython-311.pyc
+-rw-r--r--   0        0        0     1549 2023-07-12 04:48:51.890504 odin_cyble-0.0.7/odin/models/__pycache__/getHostCount.cpython-311.pyc
+-rw-r--r--   0        0        0    15185 2023-07-12 04:49:24.382971 odin_cyble-0.0.7/odin/models/__pycache__/getHostsIpDetailsResponse.cpython-311.pyc
+-rw-r--r--   0        0        0     2819 2023-07-12 05:04:32.249502 odin_cyble-0.0.7/odin/models/__pycache__/getHostsSummaryResponse.cpython-311.pyc
+-rw-r--r--   0        0        0     1576 2023-07-12 13:19:58.295803 odin_cyble-0.0.7/odin/models/__pycache__/get_certificate_count.cpython-311.pyc
+-rw-r--r--   0        0        0    18000 2023-07-12 13:19:58.297309 odin_cyble-0.0.7/odin/models/__pycache__/get_certificate_hash_details.cpython-311.pyc
+-rw-r--r--   0        0        0     2864 2023-07-12 13:19:58.298060 odin_cyble-0.0.7/odin/models/__pycache__/get_certificates_summary.cpython-311.pyc
+-rw-r--r--   0        0        0     1555 2023-07-12 13:19:58.298654 odin_cyble-0.0.7/odin/models/__pycache__/get_host_count.cpython-311.pyc
+-rw-r--r--   0        0        0    15193 2023-07-12 13:19:58.299839 odin_cyble-0.0.7/odin/models/__pycache__/get_hosts_ip_details_response.cpython-311.pyc
+-rw-r--r--   0        0        0     2826 2023-07-12 13:19:58.302638 odin_cyble-0.0.7/odin/models/__pycache__/get_hosts_summary_response.cpython-311.pyc
+-rw-r--r--   0        0        0    16425 2023-07-12 04:58:04.504493 odin_cyble-0.0.7/odin/models/__pycache__/searchHostsModel.cpython-311.pyc
+-rw-r--r--   0        0        0    16727 2023-07-14 03:05:45.593010 odin_cyble-0.0.7/odin/models/__pycache__/search_hosts_response_model.cpython-311.pyc
+-rw-r--r--   0        0        0     2823 2023-07-14 03:25:54.374435 odin_cyble-0.0.7/odin/models/certificate_search_response_model.py
+-rw-r--r--   0        0        0      434 2023-07-12 05:06:57.147103 odin_cyble-0.0.7/odin/models/get_certificate_count.py
+-rw-r--r--   0        0        0     7214 2023-07-12 05:30:11.746441 odin_cyble-0.0.7/odin/models/get_certificate_hash_details.py
+-rw-r--r--   0        0        0      960 2023-07-12 05:30:16.127850 odin_cyble-0.0.7/odin/models/get_certificates_summary.py
+-rw-r--r--   0        0        0      429 2023-07-12 04:48:26.964336 odin_cyble-0.0.7/odin/models/get_host_count.py
+-rw-r--r--   0        0        0     6693 2023-07-12 04:49:22.181362 odin_cyble-0.0.7/odin/models/get_hosts_ip_details_response.py
+-rw-r--r--   0        0        0      941 2023-07-12 05:04:30.079384 odin_cyble-0.0.7/odin/models/get_hosts_summary_response.py
+-rw-r--r--   0        0        0     7419 2023-07-14 03:05:42.334035 odin_cyble-0.0.7/odin/models/search_hosts_response_model.py
+-rw-r--r--   0        0        0      177 2023-07-12 13:17:48.671081 odin_cyble-0.0.7/odin/odin_client.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      491 2023-07-12 13:17:48.684965 odin_cyble-0.0.7/odin/odin_client.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2023-07-12 13:17:48.671422 odin_cyble-0.0.7/odin/odin_client.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       78 2023-07-12 13:17:48.671764 odin_cyble-0.0.7/odin/odin_client.egg-info/requires.txt
+-rw-r--r--   0        0        0        7 2023-07-12 13:17:48.672142 odin_cyble-0.0.7/odin/odin_client.egg-info/top_level.txt
+-rw-r--r--   0        0        0     5945 2023-07-25 11:02:44.728376 odin_cyble-0.0.7/odin/odin_client.py
+-rw-r--r--   0        0        0      448 2023-07-25 13:40:20.828864 odin_cyble-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2045 1970-01-01 00:00:00.000000 odin_cyble-0.0.7/PKG-INFO
```

### Comparing `odin_cyble-0.0.6/README.md` & `odin_cyble-0.0.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 ```bash
 pip install odin-cyble
 ```
 ## Usage
 
 Import the package into your Go code and create an instance of the `odin.APIClient` by providing the base API URL and your API key:
 ```python
-from odin_client import OdinClient
+from odin.odin_client import OdinClient
 
 client = OdinClient("https://api.getodin.com/v1", "<APIKey>")
 ```
 
 ## Examples
 
-In the "example.py", you can find various usage examples demonstrating how to interact with the Odin API using the `odin-sdk-python` package.
+In the "example.py", you can find various usage examples demonstrating how to interact with the Odin API using the `odin-sdk` package.
 
 Each example is a standalone Go program that showcases specific functionalities of the SDK.
 
 ```
 # Example for using get_certificate_count
 def ex_certificate_count():
     try:
```

### Comparing `odin_cyble-0.0.6/odin/__init__.py` & `odin_cyble-0.0.7/odin/__init__.py`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.6/odin/example.py` & `odin_cyble-0.0.7/odin/example.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from odin_client import OdinClient
+from odin.odin_client import OdinClient
 import json
 import requests
 from exceptions import APIException
 
 client = OdinClient("https://api.getodin.com/v1", "<APIKey>")
 
 # Example for using get_hosts_count
@@ -18,15 +18,15 @@
         
 # Example for using get_hosts_ip_details
 def ex_hosts_ip_details():
     try:
         response = client.get_hosts_ip_details("223.217.65.218")
         print(response.success)
         for svc in response.data.services:
-            print(svc.name)
+            print(f"Service Name: {svc.name}, Port: {svc.port}")
     except APIException as e:
         print(e.status_code)
         print(e.message)
 
 # Example for using search_host
 def ex_search_hosts():
     try:
@@ -43,16 +43,16 @@
         print(e.status_code)
         print(e.message)
 
 # Example for using get_hosts_summary
 def ex_hosts_summary():
     try:
         response = client.get_hosts_summary("services.port",9)
-        print(response.success)
-        print(len(response.data.buckets))
+        for bucket in response.data.buckets:
+            print(f"Service: {bucket.key}, Count: {bucket.doc_count}")
     except APIException as e:
         print(e.status_code)
         print(e.message)
     
 # Example for using get_certificate_count
 def ex_certificate_count():
     try:
```

### Comparing `odin_cyble-0.0.6/odin/models/__init__.py` & `odin_cyble-0.0.7/odin/models/__init__.py`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.6/odin/models/certificate_search_response_model.py` & `odin_cyble-0.0.7/odin/models/certificate_search_response_model.py`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.6/odin/models/get_certificate_hash_details.py` & `odin_cyble-0.0.7/odin/build/lib/models/get_certificate_hash_details.py`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.6/odin/models/get_certificates_summary.py` & `odin_cyble-0.0.7/odin/build/lib/models/get_certificates_summary.py`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.6/odin/models/get_hosts_ip_details_response.py` & `odin_cyble-0.0.7/odin/build/lib/models/get_hosts_ip_details_response.py`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.6/odin/models/get_hosts_summary_response.py` & `odin_cyble-0.0.7/odin/build/lib/models/get_hosts_summary_response.py`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.6/odin/models/search_hosts_response_model.py` & `odin_cyble-0.0.7/odin/models/search_hosts_response_model.py`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.6/odin/odin_client.py` & `odin_cyble-0.0.7/odin/odin_client.py`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.6/PKG-INFO` & `odin_cyble-0.0.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: odin-cyble
-Version: 0.0.6
-Summary: 
+Version: 0.0.7
+Summary: Allows to interact easily with the Odin API and access various cybersecurity services, certificate information, and more.
 Author: Anukul Kumar
 Author-email: anukul.kumar@cyble.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -23,22 +23,22 @@
 ```bash
 pip install odin-cyble
 ```
 ## Usage
 
 Import the package into your Go code and create an instance of the `odin.APIClient` by providing the base API URL and your API key:
 ```python
-from odin_client import OdinClient
+from odin.odin_client import OdinClient
 
 client = OdinClient("https://api.getodin.com/v1", "<APIKey>")
 ```
 
 ## Examples
 
-In the "example.py", you can find various usage examples demonstrating how to interact with the Odin API using the `odin-sdk-python` package.
+In the "example.py", you can find various usage examples demonstrating how to interact with the Odin API using the `odin-sdk` package.
 
 Each example is a standalone Go program that showcases specific functionalities of the SDK.
 
 ```
 # Example for using get_certificate_count
 def ex_certificate_count():
     try:
```

