# Comparing `tmp/dingtalk-stream-0.7.5.tar.gz` & `tmp/dingtalk-stream-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dingtalk-stream-0.7.5.tar", last modified: Fri Jul 21 11:31:28 2023, max compression
+gzip compressed data, was "dingtalk-stream-0.8.0.tar", last modified: Tue Jul 25 11:43:05 2023, max compression
```

## Comparing `dingtalk-stream-0.7.5.tar` & `dingtalk-stream-0.8.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:31:28.153699 dingtalk-stream-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-21 11:31:27.000000 dingtalk-stream-0.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-21 11:31:28.153699 dingtalk-stream-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-21 11:31:27.000000 dingtalk-stream-0.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:31:28.153699 dingtalk-stream-0.7.5/dingtalk_stream/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-21 11:31:27.000000 dingtalk-stream-0.7.5/dingtalk_stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-21 11:31:27.000000 dingtalk-stream-0.7.5/dingtalk_stream/card_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-07-21 11:31:27.000000 dingtalk-stream-0.7.5/dingtalk_stream/card_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-07-21 11:31:27.000000 dingtalk-stream-0.7.5/dingtalk_stream/card_replier.py
--rw-r--r--   0 runner    (1001) docker     (123)    25657 2023-07-21 11:31:27.000000 dingtalk-stream-0.7.5/dingtalk_stream/chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-21 11:31:27.000000 dingtalk-stream-0.7.5/dingtalk_stream/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-07-21 11:31:27.000000 dingtalk-stream-0.7.5/dingtalk_stream/frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-21 11:31:27.000000 dingtalk-stream-0.7.5/dingtalk_stream/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-07-21 11:31:27.000000 dingtalk-stream-0.7.5/dingtalk_stream/interactive_card.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-21 11:31:27.000000 dingtalk-stream-0.7.5/dingtalk_stream/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-07-21 11:31:27.000000 dingtalk-stream-0.7.5/dingtalk_stream/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 11:31:27.000000 dingtalk-stream-0.7.5/dingtalk_stream/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:31:28.153699 dingtalk-stream-0.7.5/dingtalk_stream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-21 11:31:28.000000 dingtalk-stream-0.7.5/dingtalk_stream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-21 11:31:28.000000 dingtalk-stream-0.7.5/dingtalk_stream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 11:31:28.000000 dingtalk-stream-0.7.5/dingtalk_stream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-21 11:31:28.000000 dingtalk-stream-0.7.5/dingtalk_stream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 11:31:28.000000 dingtalk-stream-0.7.5/dingtalk_stream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 11:31:28.153699 dingtalk-stream-0.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-21 11:31:27.000000 dingtalk-stream-0.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:43:05.211190 dingtalk-stream-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-25 11:43:05.211190 dingtalk-stream-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:43:05.211190 dingtalk-stream-0.8.0/dingtalk_stream/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/dingtalk_stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/dingtalk_stream/card_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/dingtalk_stream/card_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/dingtalk_stream/card_replier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25657 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/dingtalk_stream/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/dingtalk_stream/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/dingtalk_stream/frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/dingtalk_stream/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/dingtalk_stream/interactive_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/dingtalk_stream/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/dingtalk_stream/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/dingtalk_stream/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/dingtalk_stream/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:43:05.211190 dingtalk-stream-0.8.0/dingtalk_stream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-25 11:43:05.000000 dingtalk-stream-0.8.0/dingtalk_stream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-25 11:43:05.000000 dingtalk-stream-0.8.0/dingtalk_stream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 11:43:05.000000 dingtalk-stream-0.8.0/dingtalk_stream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-25 11:43:05.000000 dingtalk-stream-0.8.0/dingtalk_stream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 11:43:05.000000 dingtalk-stream-0.8.0/dingtalk_stream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 11:43:05.211190 dingtalk-stream-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-25 11:43:03.000000 dingtalk-stream-0.8.0/setup.py
```

### Comparing `dingtalk-stream-0.7.5/LICENSE` & `dingtalk-stream-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.5/PKG-INFO` & `dingtalk-stream-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.7.5
+Version: 0.8.0
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dingtalk-stream-0.7.5/README.md` & `dingtalk-stream-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.5/dingtalk_stream/__init__.py` & `dingtalk-stream-0.8.0/dingtalk_stream/__init__.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.5/dingtalk_stream/card_callback.py` & `dingtalk-stream-0.8.0/dingtalk_stream/card_callback.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.5/dingtalk_stream/card_instance.py` & `dingtalk-stream-0.8.0/dingtalk_stream/card_instance.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.5/dingtalk_stream/card_replier.py` & `dingtalk-stream-0.8.0/dingtalk_stream/card_replier.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.5/dingtalk_stream/chatbot.py` & `dingtalk-stream-0.8.0/dingtalk_stream/chatbot.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.5/dingtalk_stream/frames.py` & `dingtalk-stream-0.8.0/dingtalk_stream/frames.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.5/dingtalk_stream/handlers.py` & `dingtalk-stream-0.8.0/dingtalk_stream/handlers.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.5/dingtalk_stream/interactive_card.py` & `dingtalk-stream-0.8.0/dingtalk_stream/interactive_card.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.7.5/dingtalk_stream/stream.py` & `dingtalk-stream-0.8.0/dingtalk_stream/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from .handlers import EventHandler
 from .handlers import SystemHandler
 from .frames import SystemMessage
 from .frames import EventMessage
 from .frames import CallbackMessage
 from .log import setup_default_logger
 from .utils import DINGTALK_OPENAPI_ENDPOINT
+from .version import VERSION_STRING
 
 
 class DingTalkStreamClient(object):
     OPEN_CONNECTION_API = DINGTALK_OPENAPI_ENDPOINT + '/v1.0/gateway/connections/open'
     TAG_DISCONNECT = 'disconnect'
 
     def __init__(self, credential: Credential, logger: logging.Logger = None):
@@ -128,27 +129,28 @@
                 continue
 
     def open_connection(self):
         self.logger.info('open connection, url=%s' % DingTalkStreamClient.OPEN_CONNECTION_API)
         request_headers = {
             'Content-Type': 'application/json',
             'Accept': 'application/json',
-            'User-Agent': ('DingTalkStream/1.0 SDK/0.1.0 Python/%s '
+            'User-Agent': ('DingTalkStream/1.0 SDK/%s Python/%s '
                            '(+https://github.com/open-dingtalk/dingtalk-stream-sdk-python)'
-                           ) % platform.python_version(),
+                           ) % (VERSION_STRING, platform.python_version()),
         }
         topics = []
         if self._is_event_required:
             topics.append({'type': 'EVENT', 'topic': '*'})
         for topic in self.callback_handler_map.keys():
             topics.append({'type': 'CALLBACK', 'topic': topic})
         request_body = json.dumps({
             'clientId': self.credential.client_id,
             'clientSecret': self.credential.client_secret,
             'subscriptions': topics,
+            'ua': 'dingtalk-sdk-python/v%s' % VERSION_STRING,
             'localIp': self.get_host_ip()
         }).encode('utf-8')
 
         try:
             response = requests.post(DingTalkStreamClient.OPEN_CONNECTION_API,
                                      headers=request_headers,
                                      data=request_body)
```

### Comparing `dingtalk-stream-0.7.5/dingtalk_stream.egg-info/PKG-INFO` & `dingtalk-stream-0.8.0/dingtalk_stream.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.7.5
+Version: 0.8.0
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dingtalk-stream-0.7.5/dingtalk_stream.egg-info/SOURCES.txt` & `dingtalk-stream-0.8.0/dingtalk_stream.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,12 +9,13 @@
 dingtalk_stream/credential.py
 dingtalk_stream/frames.py
 dingtalk_stream/handlers.py
 dingtalk_stream/interactive_card.py
 dingtalk_stream/log.py
 dingtalk_stream/stream.py
 dingtalk_stream/utils.py
+dingtalk_stream/version.py
 dingtalk_stream.egg-info/PKG-INFO
 dingtalk_stream.egg-info/SOURCES.txt
 dingtalk_stream.egg-info/dependency_links.txt
 dingtalk_stream.egg-info/requires.txt
 dingtalk_stream.egg-info/top_level.txt
```

