# Comparing `tmp/odin_cyble-0.0.3.tar.gz` & `tmp/odin_cyble-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odin_cyble-0.0.3.tar", max compression
+gzip compressed data, was "odin_cyble-0.0.4.tar", max compression
```

## Comparing `odin_cyble-0.0.3.tar` & `odin_cyble-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1073 2023-07-25 06:36:49.084746 odin_cyble-0.0.3/LICENSE
--rw-r--r--   0        0        0     1492 2023-07-25 08:13:29.982778 odin_cyble-0.0.3/README.md
--rw-r--r--   0        0        0      977 2023-07-25 10:55:28.436097 odin_cyble-0.0.3/odin/__init__.py
--rw-r--r--   0        0        0     3169 2023-07-25 06:16:06.492192 odin_cyble-0.0.3/odin/example.py
--rw-r--r--   0        0        0      483 2023-07-24 13:30:01.718847 odin_cyble-0.0.3/odin/exceptions.py
--rw-r--r--   0        0        0      805 2023-07-25 10:55:44.171344 odin_cyble-0.0.3/odin/models/__init__.py
--rw-r--r--   0        0        0     2823 2023-07-14 03:25:54.374435 odin_cyble-0.0.3/odin/models/certificate_search_response_model.py
--rw-r--r--   0        0        0      434 2023-07-12 05:06:57.147103 odin_cyble-0.0.3/odin/models/get_certificate_count.py
--rw-r--r--   0        0        0     7214 2023-07-12 05:30:11.746441 odin_cyble-0.0.3/odin/models/get_certificate_hash_details.py
--rw-r--r--   0        0        0      960 2023-07-12 05:30:16.127850 odin_cyble-0.0.3/odin/models/get_certificates_summary.py
--rw-r--r--   0        0        0      429 2023-07-12 04:48:26.964336 odin_cyble-0.0.3/odin/models/get_host_count.py
--rw-r--r--   0        0        0     6693 2023-07-12 04:49:22.181362 odin_cyble-0.0.3/odin/models/get_hosts_ip_details_response.py
--rw-r--r--   0        0        0      941 2023-07-12 05:04:30.079384 odin_cyble-0.0.3/odin/models/get_hosts_summary_response.py
--rw-r--r--   0        0        0     7419 2023-07-14 03:05:42.334035 odin_cyble-0.0.3/odin/models/search_hosts_response_model.py
--rw-r--r--   0        0        0     5900 2023-07-25 07:31:34.549646 odin_cyble-0.0.3/odin/odin_client.py
--rw-r--r--   0        0        0      327 2023-07-25 10:56:38.064733 odin_cyble-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1926 1970-01-01 00:00:00.000000 odin_cyble-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-25 06:36:49.084746 odin_cyble-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1492 2023-07-25 08:13:29.982778 odin_cyble-0.0.4/README.md
+-rw-r--r--   0        0        0      977 2023-07-25 10:55:28.436097 odin_cyble-0.0.4/odin/__init__.py
+-rw-r--r--   0        0        0     3169 2023-07-25 06:16:06.492192 odin_cyble-0.0.4/odin/example.py
+-rw-r--r--   0        0        0      483 2023-07-24 13:30:01.718847 odin_cyble-0.0.4/odin/exceptions.py
+-rw-r--r--   0        0        0      805 2023-07-25 10:55:44.171344 odin_cyble-0.0.4/odin/models/__init__.py
+-rw-r--r--   0        0        0     2823 2023-07-14 03:25:54.374435 odin_cyble-0.0.4/odin/models/certificate_search_response_model.py
+-rw-r--r--   0        0        0      434 2023-07-12 05:06:57.147103 odin_cyble-0.0.4/odin/models/get_certificate_count.py
+-rw-r--r--   0        0        0     7214 2023-07-12 05:30:11.746441 odin_cyble-0.0.4/odin/models/get_certificate_hash_details.py
+-rw-r--r--   0        0        0      960 2023-07-12 05:30:16.127850 odin_cyble-0.0.4/odin/models/get_certificates_summary.py
+-rw-r--r--   0        0        0      429 2023-07-12 04:48:26.964336 odin_cyble-0.0.4/odin/models/get_host_count.py
+-rw-r--r--   0        0        0     6693 2023-07-12 04:49:22.181362 odin_cyble-0.0.4/odin/models/get_hosts_ip_details_response.py
+-rw-r--r--   0        0        0      941 2023-07-12 05:04:30.079384 odin_cyble-0.0.4/odin/models/get_hosts_summary_response.py
+-rw-r--r--   0        0        0     7419 2023-07-14 03:05:42.334035 odin_cyble-0.0.4/odin/models/search_hosts_response_model.py
+-rw-r--r--   0        0        0     5940 2023-07-25 10:58:32.925297 odin_cyble-0.0.4/odin/odin_client.py
+-rw-r--r--   0        0        0      327 2023-07-25 10:58:46.898096 odin_cyble-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1926 1970-01-01 00:00:00.000000 odin_cyble-0.0.4/PKG-INFO
```

### Comparing `odin_cyble-0.0.3/LICENSE` & `odin_cyble-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.3/README.md` & `odin_cyble-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.3/odin/__init__.py` & `odin_cyble-0.0.4/odin/__init__.py`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.3/odin/example.py` & `odin_cyble-0.0.4/odin/example.py`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.3/odin/models/__init__.py` & `odin_cyble-0.0.4/odin/models/__init__.py`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.3/odin/models/certificate_search_response_model.py` & `odin_cyble-0.0.4/odin/models/certificate_search_response_model.py`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.3/odin/models/get_certificate_hash_details.py` & `odin_cyble-0.0.4/odin/models/get_certificate_hash_details.py`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.3/odin/models/get_certificates_summary.py` & `odin_cyble-0.0.4/odin/models/get_certificates_summary.py`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.3/odin/models/get_hosts_ip_details_response.py` & `odin_cyble-0.0.4/odin/models/get_hosts_ip_details_response.py`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.3/odin/models/get_hosts_summary_response.py` & `odin_cyble-0.0.4/odin/models/get_hosts_summary_response.py`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.3/odin/models/search_hosts_response_model.py` & `odin_cyble-0.0.4/odin/models/search_hosts_response_model.py`

 * *Files identical despite different names*

### Comparing `odin_cyble-0.0.3/odin/odin_client.py` & `odin_cyble-0.0.4/odin/odin_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import requests
-from models.certificate_search_response_model import CertificateSearchResponse
-from models.get_host_count import GetHostsCountResponse
-from models.get_hosts_ip_details_response import GetHostsIpDetailsResponse
-from models.search_hosts_response_model import SearchHostsResponse
-from models.get_hosts_summary_response import GetHostSummaryResponse
-from models.get_certificate_count import GetCertificatesCountResponse
-from models.get_certificate_hash_details import GetCertificateHashDetails
-from models.get_certificates_summary import GetCertificatesSummaryResponse
+from odin.models.certificate_search_response_model import CertificateSearchResponse
+from odin.models.get_host_count import GetHostsCountResponse
+from odin.models.get_hosts_ip_details_response import GetHostsIpDetailsResponse
+from odin.models.search_hosts_response_model import SearchHostsResponse
+from odin.models.get_hosts_summary_response import GetHostSummaryResponse
+from odin.models.get_certificate_count import GetCertificatesCountResponse
+from odin.models.get_certificate_hash_details import GetCertificateHashDetails
+from odin.models.get_certificates_summary import GetCertificatesSummaryResponse
 from exceptions import APIException
 import json
 
 class OdinClient:
     
     def __init__(self, base_url, api_key, timeout=None):
         """
```

### Comparing `odin_cyble-0.0.3/PKG-INFO` & `odin_cyble-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odin-cyble
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
 Author: Anukul Kumar
 Author-email: anukul.kumar@cyble.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

