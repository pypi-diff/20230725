# Comparing `tmp/moesifdjango-2.3.3.tar.gz` & `tmp/moesifdjango-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moesifdjango-2.3.3.tar", last modified: Wed Jul 12 22:37:49 2023, max compression
+gzip compressed data, was "moesifdjango-2.3.4.tar", last modified: Tue Jul 25 17:50:17 2023, max compression
```

## Comparing `moesifdjango-2.3.3.tar` & `moesifdjango-2.3.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 brian     (1000) brian     (1001)        0 2023-07-12 22:37:49.656316 moesifdjango-2.3.3/
--rwxr-xr-x   0 brian     (1000) brian     (1001)    11918 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/LICENSE
--rw-r--r--   0 brian     (1000) brian     (1001)       61 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/MANIFEST.in
--rw-r--r--   0 brian     (1000) brian     (1001)    19503 2023-07-12 22:37:49.656316 moesifdjango-2.3.3/PKG-INFO
--rwxr-xr-x   0 brian     (1000) brian     (1001)    18400 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/README.md
-drwxr-xr-x   0 brian     (1000) brian     (1001)        0 2023-07-12 22:37:49.656316 moesifdjango-2.3.3/moesifdjango/
--rw-r--r--   0 brian     (1000) brian     (1001)       63 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/moesifdjango/__init__.py
--rw-r--r--   0 brian     (1000) brian     (1001)      666 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/moesifdjango/block_response_buffer.py
--rw-r--r--   0 brian     (1000) brian     (1001)     4855 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/moesifdjango/client_ip.py
--rw-r--r--   0 brian     (1000) brian     (1001)     1570 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/moesifdjango/event_mapper.py
--rw-r--r--   0 brian     (1000) brian     (1001)      555 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/moesifdjango/governance_rule_response.py
--rw-r--r--   0 brian     (1000) brian     (1001)     2152 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/moesifdjango/governance_rules.py
--rw-r--r--   0 brian     (1000) brian     (1001)      616 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/moesifdjango/http_response_catcher.py
--rw-r--r--   0 brian     (1000) brian     (1001)     3699 2023-07-12 22:28:28.000000 moesifdjango-2.3.3/moesifdjango/job_scheduler.py
--rw-r--r--   0 brian     (1000) brian     (1001)    14517 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/moesifdjango/logger_helper.py
--rw-r--r--   0 brian     (1000) brian     (1001)     1403 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/moesifdjango/masks.py
--rw-r--r--   0 brian     (1000) brian     (1001)    17343 2023-07-12 22:37:26.000000 moesifdjango-2.3.3/moesifdjango/middleware.py
--rw-r--r--   0 brian     (1000) brian     (1001)    14371 2023-07-12 20:54:27.000000 moesifdjango-2.3.3/moesifdjango/middleware_pre19.py
--rw-r--r--   0 brian     (1000) brian     (1001)    25617 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/moesifdjango/moesif_gov.py
--rw-r--r--   0 brian     (1000) brian     (1001)     2471 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/moesifdjango/parse_body.py
--rw-r--r--   0 brian     (1000) brian     (1001)     6657 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/moesifdjango/update_companies.py
--rw-r--r--   0 brian     (1000) brian     (1001)     6381 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/moesifdjango/update_users.py
-drwxr-xr-x   0 brian     (1000) brian     (1001)        0 2023-07-12 22:37:49.656316 moesifdjango-2.3.3/moesifdjango.egg-info/
--rw-r--r--   0 brian     (1000) brian     (1001)    19503 2023-07-12 22:37:49.000000 moesifdjango-2.3.3/moesifdjango.egg-info/PKG-INFO
--rw-r--r--   0 brian     (1000) brian     (1001)      861 2023-07-12 22:37:49.000000 moesifdjango-2.3.3/moesifdjango.egg-info/SOURCES.txt
--rw-r--r--   0 brian     (1000) brian     (1001)        1 2023-07-12 22:37:49.000000 moesifdjango-2.3.3/moesifdjango.egg-info/dependency_links.txt
--rw-r--r--   0 brian     (1000) brian     (1001)      136 2023-07-12 22:37:49.000000 moesifdjango-2.3.3/moesifdjango.egg-info/requires.txt
--rw-r--r--   0 brian     (1000) brian     (1001)       19 2023-07-12 22:37:49.000000 moesifdjango-2.3.3/moesifdjango.egg-info/top_level.txt
--rw-r--r--   0 brian     (1000) brian     (1001)       67 2023-07-12 22:37:49.656316 moesifdjango-2.3.3/setup.cfg
--rw-r--r--   0 brian     (1000) brian     (1001)     3363 2023-07-12 21:19:51.000000 moesifdjango-2.3.3/setup.py
-drwxr-xr-x   0 brian     (1000) brian     (1001)        0 2023-07-12 22:37:49.656316 moesifdjango-2.3.3/tests/
-drwxr-xr-x   0 brian     (1000) brian     (1001)        0 2023-07-12 22:37:49.656316 moesifdjango-2.3.3/tests/middleware_pre19_tests/
--rw-r--r--   0 brian     (1000) brian     (1001)        0 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/tests/middleware_pre19_tests/__init__.py
--rw-r--r--   0 brian     (1000) brian     (1001)     4990 2023-07-12 21:17:50.000000 moesifdjango-2.3.3/tests/middleware_pre19_tests/tests.py
-drwxr-xr-x   0 brian     (1000) brian     (1001)        0 2023-07-12 22:37:49.656316 moesifdjango-2.3.3/tests/middleware_tests/
--rw-r--r--   0 brian     (1000) brian     (1001)        0 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/tests/middleware_tests/__init__.py
--rw-r--r--   0 brian     (1000) brian     (1001)     5266 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/tests/middleware_tests/tests.py
+drwxr-xr-x   0 brian     (1000) brian     (1001)        0 2023-07-25 17:50:17.116302 moesifdjango-2.3.4/
+-rwxr-xr-x   0 brian     (1000) brian     (1001)    11918 2023-07-12 20:42:10.000000 moesifdjango-2.3.4/LICENSE
+-rw-r--r--   0 brian     (1000) brian     (1001)       61 2023-07-12 20:42:10.000000 moesifdjango-2.3.4/MANIFEST.in
+-rw-r--r--   0 brian     (1000) brian     (1001)    19503 2023-07-25 17:50:17.116302 moesifdjango-2.3.4/PKG-INFO
+-rwxr-xr-x   0 brian     (1000) brian     (1001)    18400 2023-07-12 20:42:10.000000 moesifdjango-2.3.4/README.md
+drwxr-xr-x   0 brian     (1000) brian     (1001)        0 2023-07-25 17:50:17.116302 moesifdjango-2.3.4/moesifdjango/
+-rw-r--r--   0 brian     (1000) brian     (1001)       63 2023-07-12 20:42:10.000000 moesifdjango-2.3.4/moesifdjango/__init__.py
+-rw-r--r--   0 brian     (1000) brian     (1001)      666 2023-07-12 20:42:10.000000 moesifdjango-2.3.4/moesifdjango/block_response_buffer.py
+-rw-r--r--   0 brian     (1000) brian     (1001)     4855 2023-07-12 20:42:10.000000 moesifdjango-2.3.4/moesifdjango/client_ip.py
+-rw-r--r--   0 brian     (1000) brian     (1001)     1570 2023-07-12 20:42:10.000000 moesifdjango-2.3.4/moesifdjango/event_mapper.py
+-rw-r--r--   0 brian     (1000) brian     (1001)      555 2023-07-12 20:42:10.000000 moesifdjango-2.3.4/moesifdjango/governance_rule_response.py
+-rw-r--r--   0 brian     (1000) brian     (1001)     2152 2023-07-12 20:42:10.000000 moesifdjango-2.3.4/moesifdjango/governance_rules.py
+-rw-r--r--   0 brian     (1000) brian     (1001)      616 2023-07-12 20:42:10.000000 moesifdjango-2.3.4/moesifdjango/http_response_catcher.py
+-rw-r--r--   0 brian     (1000) brian     (1001)     3584 2023-07-25 17:32:38.000000 moesifdjango-2.3.4/moesifdjango/job_scheduler.py
+-rw-r--r--   0 brian     (1000) brian     (1001)    14517 2023-07-12 20:42:10.000000 moesifdjango-2.3.4/moesifdjango/logger_helper.py
+-rw-r--r--   0 brian     (1000) brian     (1001)     1403 2023-07-12 20:42:10.000000 moesifdjango-2.3.4/moesifdjango/masks.py
+-rw-r--r--   0 brian     (1000) brian     (1001)    17394 2023-07-25 17:32:38.000000 moesifdjango-2.3.4/moesifdjango/middleware.py
+-rw-r--r--   0 brian     (1000) brian     (1001)    14371 2023-07-12 20:54:27.000000 moesifdjango-2.3.4/moesifdjango/middleware_pre19.py
+-rw-r--r--   0 brian     (1000) brian     (1001)    25617 2023-07-12 20:42:10.000000 moesifdjango-2.3.4/moesifdjango/moesif_gov.py
+-rw-r--r--   0 brian     (1000) brian     (1001)     2471 2023-07-12 20:42:10.000000 moesifdjango-2.3.4/moesifdjango/parse_body.py
+-rw-r--r--   0 brian     (1000) brian     (1001)     6657 2023-07-12 20:42:10.000000 moesifdjango-2.3.4/moesifdjango/update_companies.py
+-rw-r--r--   0 brian     (1000) brian     (1001)     6381 2023-07-12 20:42:10.000000 moesifdjango-2.3.4/moesifdjango/update_users.py
+drwxr-xr-x   0 brian     (1000) brian     (1001)        0 2023-07-25 17:50:17.116302 moesifdjango-2.3.4/moesifdjango.egg-info/
+-rw-r--r--   0 brian     (1000) brian     (1001)    19503 2023-07-25 17:50:17.000000 moesifdjango-2.3.4/moesifdjango.egg-info/PKG-INFO
+-rw-r--r--   0 brian     (1000) brian     (1001)      861 2023-07-25 17:50:17.000000 moesifdjango-2.3.4/moesifdjango.egg-info/SOURCES.txt
+-rw-r--r--   0 brian     (1000) brian     (1001)        1 2023-07-25 17:50:17.000000 moesifdjango-2.3.4/moesifdjango.egg-info/dependency_links.txt
+-rw-r--r--   0 brian     (1000) brian     (1001)      136 2023-07-25 17:50:17.000000 moesifdjango-2.3.4/moesifdjango.egg-info/requires.txt
+-rw-r--r--   0 brian     (1000) brian     (1001)       19 2023-07-25 17:50:17.000000 moesifdjango-2.3.4/moesifdjango.egg-info/top_level.txt
+-rw-r--r--   0 brian     (1000) brian     (1001)       67 2023-07-25 17:50:17.116302 moesifdjango-2.3.4/setup.cfg
+-rw-r--r--   0 brian     (1000) brian     (1001)     3363 2023-07-25 17:50:03.000000 moesifdjango-2.3.4/setup.py
+drwxr-xr-x   0 brian     (1000) brian     (1001)        0 2023-07-25 17:50:17.112969 moesifdjango-2.3.4/tests/
+drwxr-xr-x   0 brian     (1000) brian     (1001)        0 2023-07-25 17:50:17.116302 moesifdjango-2.3.4/tests/middleware_pre19_tests/
+-rw-r--r--   0 brian     (1000) brian     (1001)        0 2023-07-12 20:42:10.000000 moesifdjango-2.3.4/tests/middleware_pre19_tests/__init__.py
+-rw-r--r--   0 brian     (1000) brian     (1001)     4990 2023-07-12 21:17:50.000000 moesifdjango-2.3.4/tests/middleware_pre19_tests/tests.py
+drwxr-xr-x   0 brian     (1000) brian     (1001)        0 2023-07-25 17:50:17.116302 moesifdjango-2.3.4/tests/middleware_tests/
+-rw-r--r--   0 brian     (1000) brian     (1001)        0 2023-07-12 20:42:10.000000 moesifdjango-2.3.4/tests/middleware_tests/__init__.py
+-rw-r--r--   0 brian     (1000) brian     (1001)     5266 2023-07-12 20:42:10.000000 moesifdjango-2.3.4/tests/middleware_tests/tests.py
```

### Comparing `moesifdjango-2.3.3/LICENSE` & `moesifdjango-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.3/PKG-INFO` & `moesifdjango-2.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moesifdjango
-Version: 2.3.3
+Version: 2.3.4
 Summary: Moesif Middleware for Python Django
 Home-page: https://www.moesif.com/docs/server-integration/django/
 Author: Moesif, Inc
 Author-email: derric@moesif.com
 License: Apache Software License
 Keywords: log analysis restful api development debug
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moesifdjango-2.3.3/README.md` & `moesifdjango-2.3.4/README.md`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.3/moesifdjango/block_response_buffer.py` & `moesifdjango-2.3.4/moesifdjango/block_response_buffer.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.3/moesifdjango/client_ip.py` & `moesifdjango-2.3.4/moesifdjango/client_ip.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.3/moesifdjango/event_mapper.py` & `moesifdjango-2.3.4/moesifdjango/event_mapper.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.3/moesifdjango/governance_rule_response.py` & `moesifdjango-2.3.4/moesifdjango/governance_rule_response.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.3/moesifdjango/governance_rules.py` & `moesifdjango-2.3.4/moesifdjango/governance_rules.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.3/moesifdjango/http_response_catcher.py` & `moesifdjango-2.3.4/moesifdjango/http_response_catcher.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.3/moesifdjango/job_scheduler.py` & `moesifdjango-2.3.4/moesifdjango/job_scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,14 @@
             if debug:
                 print('Error while fetching the application configuration')
                 print(str(e))
         return config, config_etag, sampling_percentage, last_updated_time
 
 
     def batch_events(self, api_client, moesif_events_queue, debug, batch_size):
-        print("Starting batch events job")
         batch_events = []
         try:
             while not moesif_events_queue.empty():
                 batch_events.append(moesif_events_queue.get_nowait())
                 if len(batch_events) == batch_size:
                     break
 
@@ -61,20 +60,18 @@
                 req_time = batch_events[0].request.time
                 req_time = datetime.strptime(req_time, '%Y-%m-%dT%H:%M:%S.%f')
                 batch_response_config_etag, batch_response_rules_etag = self.send_events(api_client, batch_events, debug)
                 batch_events[:] = []
                 # Set the last time event job ran after sending events
                 batch_send_time = datetime.utcnow()
                 delta = batch_send_time - req_time
-                if debug and delta.total_seconds() > 0:
+                if debug and delta.total_seconds() > 60:
                     print("Warning: It took %s seconds to send events to Moesif. req.time=%s now=%s"%(delta.total_seconds(), req_time, batch_send_time))
                 return batch_response_config_etag, batch_response_rules_etag, batch_send_time
             else:
-                if debug:
-                    print("No events to send")
                 # Set the last time event job ran but no message to read from the queue
                 return None, None, datetime.utcnow()
         except Exception as e:
             if debug:
                 print("No message to read from the queue")
                 print(str(e))
             # Set the last time event job ran when exception occurred while sending event
```

### Comparing `moesifdjango-2.3.3/moesifdjango/logger_helper.py` & `moesifdjango-2.3.4/moesifdjango/logger_helper.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.3/moesifdjango/masks.py` & `moesifdjango-2.3.4/moesifdjango/masks.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.3/moesifdjango/middleware.py` & `moesifdjango-2.3.4/moesifdjango/middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,15 @@
     def schedule_event_background_job(self):
         try:
             if not self.scheduler:
                 self.scheduler = BackgroundScheduler(daemon=True)
             if not self.scheduler.get_jobs():
                 self.scheduler.add_listener(self.event_listener, EVENT_JOB_EXECUTED | EVENT_JOB_ERROR)
                 self.scheduler.start()
+                print("Starting batch events job")
                 self.scheduler.add_job(
                     func=lambda: self.job_scheduler.batch_events(self.api_client, self.mo_events_queue, self.DEBUG,
                                                                  self.event_batch_size),
                     trigger=IntervalTrigger(seconds=2),
                     id='moesif_events_batch_job',
                     name='Schedule events batch job every 2 second',
                     replace_existing=True)
```

### Comparing `moesifdjango-2.3.3/moesifdjango/middleware_pre19.py` & `moesifdjango-2.3.4/moesifdjango/middleware_pre19.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.3/moesifdjango/moesif_gov.py` & `moesifdjango-2.3.4/moesifdjango/moesif_gov.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.3/moesifdjango/parse_body.py` & `moesifdjango-2.3.4/moesifdjango/parse_body.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.3/moesifdjango/update_companies.py` & `moesifdjango-2.3.4/moesifdjango/update_companies.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.3/moesifdjango/update_users.py` & `moesifdjango-2.3.4/moesifdjango/update_users.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.3/moesifdjango.egg-info/PKG-INFO` & `moesifdjango-2.3.4/moesifdjango.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moesifdjango
-Version: 2.3.3
+Version: 2.3.4
 Summary: Moesif Middleware for Python Django
 Home-page: https://www.moesif.com/docs/server-integration/django/
 Author: Moesif, Inc
 Author-email: derric@moesif.com
 License: Apache Software License
 Keywords: log analysis restful api development debug
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moesifdjango-2.3.3/moesifdjango.egg-info/SOURCES.txt` & `moesifdjango-2.3.4/moesifdjango.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.3/setup.py` & `moesifdjango-2.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 setup(
     name='moesifdjango',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='2.3.3',
+    version='2.3.4',
 
     description='Moesif Middleware for Python Django',
     long_description=long_description,
     long_description_content_type="text/markdown",
     
     # The project's main homepage.
     url='https://www.moesif.com/docs/server-integration/django/',
```

### Comparing `moesifdjango-2.3.3/tests/middleware_pre19_tests/tests.py` & `moesifdjango-2.3.4/tests/middleware_pre19_tests/tests.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.3/tests/middleware_tests/tests.py` & `moesifdjango-2.3.4/tests/middleware_tests/tests.py`

 * *Files identical despite different names*

