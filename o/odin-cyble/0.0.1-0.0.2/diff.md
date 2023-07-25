# Comparing `tmp/odin_cyble-0.0.1.tar.gz` & `tmp/odin_cyble-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odin_cyble-0.0.1.tar", max compression
+gzip compressed data, was "odin_cyble-0.0.2.tar", max compression
```

## Comparing `odin_cyble-0.0.1.tar` & `odin_cyble-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1073 2023-07-25 06:36:49.084746 odin_cyble-0.0.1/LICENSE
--rw-r--r--   0        0        0     1492 2023-07-25 08:13:29.982778 odin_cyble-0.0.1/README.md
--rw-r--r--   0        0        0      937 2023-07-25 10:20:19.551618 odin_cyble-0.0.1/odin/__init__.py
--rw-r--r--   0        0        0     3169 2023-07-25 06:16:06.492192 odin_cyble-0.0.1/odin/example.py
--rw-r--r--   0        0        0      483 2023-07-24 13:30:01.718847 odin_cyble-0.0.1/odin/exceptions.py
--rw-r--r--   0        0        0      805 2023-07-12 13:19:55.965787 odin_cyble-0.0.1/odin/models/__init__.py
--rw-r--r--   0        0        0     2823 2023-07-14 03:25:54.374435 odin_cyble-0.0.1/odin/models/certificate_search_response_model.py
--rw-r--r--   0        0        0      434 2023-07-12 05:06:57.147103 odin_cyble-0.0.1/odin/models/get_certificate_count.py
--rw-r--r--   0        0        0     7214 2023-07-12 05:30:11.746441 odin_cyble-0.0.1/odin/models/get_certificate_hash_details.py
--rw-r--r--   0        0        0      960 2023-07-12 05:30:16.127850 odin_cyble-0.0.1/odin/models/get_certificates_summary.py
--rw-r--r--   0        0        0      429 2023-07-12 04:48:26.964336 odin_cyble-0.0.1/odin/models/get_host_count.py
--rw-r--r--   0        0        0     6693 2023-07-12 04:49:22.181362 odin_cyble-0.0.1/odin/models/get_hosts_ip_details_response.py
--rw-r--r--   0        0        0      941 2023-07-12 05:04:30.079384 odin_cyble-0.0.1/odin/models/get_hosts_summary_response.py
--rw-r--r--   0        0        0     7419 2023-07-14 03:05:42.334035 odin_cyble-0.0.1/odin/models/search_hosts_response_model.py
--rw-r--r--   0        0        0     5900 2023-07-25 07:31:34.549646 odin_cyble-0.0.1/odin/odin_client.py
--rw-r--r--   0        0        0      304 2023-07-25 10:20:06.791733 odin_cyble-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1884 1970-01-01 00:00:00.000000 odin_cyble-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-25 06:36:49.084746 odin_cyble-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1492 2023-07-25 08:13:29.982778 odin_cyble-0.0.2/README.md
+-rw-r--r--   0        0        0      937 2023-07-25 10:20:19.551618 odin_cyble-0.0.2/odin/__init__.py
+-rw-r--r--   0        0        0     3169 2023-07-25 06:16:06.492192 odin_cyble-0.0.2/odin/example.py
+-rw-r--r--   0        0        0      483 2023-07-24 13:30:01.718847 odin_cyble-0.0.2/odin/exceptions.py
+-rw-r--r--   0        0        0      805 2023-07-12 13:19:55.965787 odin_cyble-0.0.2/odin/models/__init__.py
+-rw-r--r--   0        0        0     2823 2023-07-14 03:25:54.374435 odin_cyble-0.0.2/odin/models/certificate_search_response_model.py
+-rw-r--r--   0        0        0      434 2023-07-12 05:06:57.147103 odin_cyble-0.0.2/odin/models/get_certificate_count.py
+-rw-r--r--   0        0        0     7214 2023-07-12 05:30:11.746441 odin_cyble-0.0.2/odin/models/get_certificate_hash_details.py
+-rw-r--r--   0        0        0      960 2023-07-12 05:30:16.127850 odin_cyble-0.0.2/odin/models/get_certificates_summary.py
+-rw-r--r--   0        0        0      429 2023-07-12 04:48:26.964336 odin_cyble-0.0.2/odin/models/get_host_count.py
+-rw-r--r--   0        0        0     6693 2023-07-12 04:49:22.181362 odin_cyble-0.0.2/odin/models/get_hosts_ip_details_response.py
+-rw-r--r--   0        0        0      941 2023-07-12 05:04:30.079384 odin_cyble-0.0.2/odin/models/get_hosts_summary_response.py
+-rw-r--r--   0        0        0     7419 2023-07-14 03:05:42.334035 odin_cyble-0.0.2/odin/models/search_hosts_response_model.py
+-rw-r--r--   0        0        0     5900 2023-07-25 07:31:34.549646 odin_cyble-0.0.2/odin/odin_client.py
+-rw-r--r--   0        0        0      327 2023-07-25 10:51:39.365968 odin_cyble-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1926 1970-01-01 00:00:00.000000 odin_cyble-0.0.2/PKG-INFO
```

### Comparing `odin_cyble-0.0.1/LICENSE` & `odin_cyble-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.1/README.md` & `odin_cyble-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.1/odin/__init__.py` & `odin_cyble-0.0.2/odin/__init__.py`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.1/odin/example.py` & `odin_cyble-0.0.2/odin/example.py`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.1/odin/models/__init__.py` & `odin_cyble-0.0.2/odin/models/__init__.py`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.1/odin/models/certificate_search_response_model.py` & `odin_cyble-0.0.2/odin/models/certificate_search_response_model.py`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.1/odin/models/get_certificate_hash_details.py` & `odin_cyble-0.0.2/odin/models/get_certificate_hash_details.py`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.1/odin/models/get_certificates_summary.py` & `odin_cyble-0.0.2/odin/models/get_certificates_summary.py`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.1/odin/models/get_hosts_ip_details_response.py` & `odin_cyble-0.0.2/odin/models/get_hosts_ip_details_response.py`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.1/odin/models/get_hosts_summary_response.py` & `odin_cyble-0.0.2/odin/models/get_hosts_summary_response.py`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.1/odin/models/search_hosts_response_model.py` & `odin_cyble-0.0.2/odin/models/search_hosts_response_model.py`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.1/odin/odin_client.py` & `odin_cyble-0.0.2/odin/odin_client.py`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.1/PKG-INFO` & `odin_cyble-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: odin-cyble
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Author: Anukul Kumar
 Author-email: anukul.kumar@cyble.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: requests (>=2.26.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Odin SDK for Python
 
 The Odin SDK for Python allows you to easily interact with the Odin API and access various cybersecurity services, certificate information, and more.
 
 ## Installation
```

