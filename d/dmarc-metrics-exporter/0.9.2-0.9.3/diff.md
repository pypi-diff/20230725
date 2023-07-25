# Comparing `tmp/dmarc_metrics_exporter-0.9.2.tar.gz` & `tmp/dmarc_metrics_exporter-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmarc_metrics_exporter-0.9.2.tar", max compression
+gzip compressed data, was "dmarc_metrics_exporter-0.9.3.tar", max compression
```

## Comparing `dmarc_metrics_exporter-0.9.2.tar` & `dmarc_metrics_exporter-0.9.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1073 2023-06-30 17:31:40.186472 dmarc_metrics_exporter-0.9.2/LICENSE
--rw-r--r--   0        0        0    10258 2023-06-30 17:31:40.186472 dmarc_metrics_exporter-0.9.2/README.rst
--rw-r--r--   0        0        0       22 2023-06-30 17:31:40.190472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/__init__.py
--rw-r--r--   0        0        0      109 2023-06-30 17:31:40.190472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/__main__.py
--rw-r--r--   0        0        0     5096 2023-06-30 17:31:40.190472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/app.py
--rw-r--r--   0        0        0     4447 2023-06-30 17:31:40.190472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/deserialization.py
--rw-r--r--   0        0        0      703 2023-06-30 17:31:40.190472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/dmarc_event.py
--rw-r--r--   0        0        0     1716 2023-06-30 17:31:40.190472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/dmarc_metrics.py
--rw-r--r--   0        0        0     2104 2023-06-30 17:31:40.190472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/expiring_set.py
--rw-r--r--   0        0        0    13739 2023-06-30 17:31:40.190472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/imap_client.py
--rw-r--r--   0        0        0     5784 2023-06-30 17:31:40.190472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/imap_parser.py
--rwxr-xr-x   0        0        0     5172 2023-06-30 17:31:40.190472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/imap_queue.py
--rw-r--r--   0        0        0     1793 2023-06-30 17:31:40.190472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/metrics_persister.py
--rw-r--r--   0        0        0      461 2023-06-30 17:31:40.190472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/model/__init__.py
--rw-r--r--   0        0        0     9773 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/model/dmarc_aggregate_report.py
--rw-r--r--   0        0        0        0 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/model/tests/__init__.py
--rw-r--r--   0        0        0     2972 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/model/tests/sample_data.py
--rw-r--r--   0        0        0      403 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/model/tests/test_deserialization.py
--rw-r--r--   0        0        0     5093 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/prometheus_exporter.py
--rw-r--r--   0        0        0        0 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/__init__.py
--rw-r--r--   0        0        0     2976 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/conftest.py
--rw-r--r--   0        0        0     1769 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/sample_emails.py
--rw-r--r--   0        0        0     2983 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_app.py
--rw-r--r--   0        0        0     1357 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_deserialization.py
--rw-r--r--   0        0        0     1428 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_dmarc_metrics.py
--rw-r--r--   0        0        0     3499 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_e2e.py
--rw-r--r--   0        0        0      932 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_expiring_set.py
--rw-r--r--   0        0        0    16524 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_imap_client.py
--rw-r--r--   0        0        0    10834 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_imap_parser.py
--rw-r--r--   0        0        0     4757 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_imap_queue.py
--rw-r--r--   0        0        0     1192 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_metrics_persister.py
--rw-r--r--   0        0        0     3960 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_prometheus_exporter.py
--rwxr-xr-x   0        0        0     2133 2023-06-30 17:31:40.194472 dmarc_metrics_exporter-0.9.2/pyproject.toml
--rw-r--r--   0        0        0    11550 1970-01-01 00:00:00.000000 dmarc_metrics_exporter-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-25 19:54:38.442700 dmarc_metrics_exporter-0.9.3/LICENSE
+-rw-r--r--   0        0        0    10258 2023-07-25 19:54:38.442700 dmarc_metrics_exporter-0.9.3/README.rst
+-rw-r--r--   0        0        0       22 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/__init__.py
+-rw-r--r--   0        0        0      109 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/__main__.py
+-rw-r--r--   0        0        0     5096 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/app.py
+-rw-r--r--   0        0        0     4581 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/deserialization.py
+-rw-r--r--   0        0        0      703 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/dmarc_event.py
+-rw-r--r--   0        0        0     1716 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/dmarc_metrics.py
+-rw-r--r--   0        0        0     2104 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/expiring_set.py
+-rw-r--r--   0        0        0    13739 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/imap_client.py
+-rw-r--r--   0        0        0     5784 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/imap_parser.py
+-rwxr-xr-x   0        0        0     5172 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/imap_queue.py
+-rw-r--r--   0        0        0     1793 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/metrics_persister.py
+-rw-r--r--   0        0        0      461 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/model/__init__.py
+-rw-r--r--   0        0        0     9773 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/model/dmarc_aggregate_report.py
+-rw-r--r--   0        0        0        0 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/model/tests/__init__.py
+-rw-r--r--   0        0        0     2990 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/model/tests/sample_data.py
+-rw-r--r--   0        0        0      537 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/model/tests/test_deserialization.py
+-rw-r--r--   0        0        0     5093 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/prometheus_exporter.py
+-rw-r--r--   0        0        0        0 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/__init__.py
+-rw-r--r--   0        0        0     2976 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/conftest.py
+-rw-r--r--   0        0        0     1769 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/sample_emails.py
+-rw-r--r--   0        0        0     2983 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_app.py
+-rw-r--r--   0        0        0     1357 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_deserialization.py
+-rw-r--r--   0        0        0     1428 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_dmarc_metrics.py
+-rw-r--r--   0        0        0     3499 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_e2e.py
+-rw-r--r--   0        0        0      932 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_expiring_set.py
+-rw-r--r--   0        0        0    16524 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_imap_client.py
+-rw-r--r--   0        0        0    10834 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_imap_parser.py
+-rw-r--r--   0        0        0     4757 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_imap_queue.py
+-rw-r--r--   0        0        0     1192 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_metrics_persister.py
+-rw-r--r--   0        0        0     3960 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_prometheus_exporter.py
+-rwxr-xr-x   0        0        0     2133 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0    11550 1970-01-01 00:00:00.000000 dmarc_metrics_exporter-0.9.3/PKG-INFO
```

### Comparing `dmarc_metrics_exporter-0.9.2/LICENSE` & `dmarc_metrics_exporter-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.2/README.rst` & `dmarc_metrics_exporter-0.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/app.py` & `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/app.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/deserialization.py` & `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/deserialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import logging
 from email.contentmanager import raw_data_manager
 from email.message import EmailMessage
 from typing import Callable, Generator, Mapping, Optional
 from zipfile import ZipFile
 
 from xsdata.formats.dataclass.context import XmlContext
+from xsdata.formats.dataclass.parsers.config import ParserConfig
 from xsdata.formats.dataclass.parsers.xml import XmlParser
 
 from dmarc_metrics_exporter.dmarc_event import (
     Disposition,
     DmarcEvent,
     DmarcResult,
     Meta,
@@ -45,15 +46,17 @@
     "text/xml": handle_text_xml,
 }
 
 
 def get_aggregate_report_from_email(
     msg: EmailMessage,
 ) -> Generator[Feedback, None, None]:
-    parser = XmlParser(context=XmlContext())
+    parser = XmlParser(
+        context=XmlContext(), config=ParserConfig(fail_on_unknown_properties=False)
+    )
     has_found_a_report = False
     for part in msg.walk():
         if part.get_content_type() in content_type_handlers:
             handler = content_type_handlers[part.get_content_type()]
             content = raw_data_manager.get_content(part)
             has_found_a_report = True
             for payload in handler(content):
```

### Comparing `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/dmarc_event.py` & `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/dmarc_event.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/dmarc_metrics.py` & `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/dmarc_metrics.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/expiring_set.py` & `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/expiring_set.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/imap_client.py` & `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/imap_client.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/imap_parser.py` & `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/imap_parser.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/imap_queue.py` & `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/imap_queue.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/metrics_persister.py` & `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/metrics_persister.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/model/dmarc_aggregate_report.py` & `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/model/dmarc_aggregate_report.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/model/tests/sample_data.py` & `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/model/tests/sample_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
   <policy_published>
     <domain>mydomain.de</domain>
     <adkim>r</adkim>
     <aspf>r</aspf>
     <p>none</p>
     <sp>none</sp>
     <pct>100</pct>
+    <np>none</np>
   </policy_published>
   <record>
     <row>
       <source_ip>dead:beef:1:abc::</source_ip>
       <count>1</count>
       <policy_evaluated>
         <disposition>none</disposition>
```

### Comparing `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/prometheus_exporter.py` & `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/prometheus_exporter.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/conftest.py` & `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/sample_emails.py` & `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/sample_emails.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_app.py` & `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_deserialization.py` & `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_dmarc_metrics.py` & `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_dmarc_metrics.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_e2e.py` & `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_expiring_set.py` & `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_expiring_set.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_imap_client.py` & `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_imap_client.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_imap_parser.py` & `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_imap_parser.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_imap_queue.py` & `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_imap_queue.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_metrics_persister.py` & `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_metrics_persister.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.2/dmarc_metrics_exporter/tests/test_prometheus_exporter.py` & `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_prometheus_exporter.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.2/pyproject.toml` & `dmarc_metrics_exporter-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ]
 description = "Export Prometheus metrics from DMARC reports."
 keywords = ["DMARC", "DKIM", "SPF", "Prometheus"]
 license = "MIT"
 name = "dmarc-metrics-exporter"
 readme = "README.rst"
 repository = "https://github.com/jgosmann/dmarc-metrics-exporter/"
-version = "0.9.2" # Update also in __init__.py!
+version = "0.9.3" # Update also in __init__.py!
 
 [tool.poetry.scripts]
 dmarc-metrics-exporter = "dmarc_metrics_exporter.__main__:run"
 
 [tool.poetry.dependencies]
 bite-parser = "^0.2.2"
 dataclasses-serialization = "^1.3.1"
```

### Comparing `dmarc_metrics_exporter-0.9.2/PKG-INFO` & `dmarc_metrics_exporter-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmarc-metrics-exporter
-Version: 0.9.2
+Version: 0.9.3
 Summary: Export Prometheus metrics from DMARC reports.
 Home-page: https://github.com/jgosmann/dmarc-metrics-exporter/
 License: MIT
 Keywords: DMARC,DKIM,SPF,Prometheus
 Author: Jan Gosmann
 Author-email: jan@hyper-world.de
 Requires-Python: >=3.8,<4.0
```

