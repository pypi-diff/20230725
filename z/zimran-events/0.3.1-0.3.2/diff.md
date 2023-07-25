# Comparing `tmp/zimran-events-0.3.1.tar.gz` & `tmp/zimran-events-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zimran-events-0.3.1.tar", last modified: Wed Jul 19 08:30:34 2023, max compression
+gzip compressed data, was "zimran-events-0.3.2.tar", last modified: Tue Jul 25 09:59:52 2023, max compression
```

## Comparing `zimran-events-0.3.1.tar` & `zimran-events-0.3.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:30:34.700029 zimran-events-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-19 08:30:21.000000 zimran-events-0.3.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-19 08:30:21.000000 zimran-events-0.3.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-19 08:30:21.000000 zimran-events-0.3.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:30:34.696029 zimran-events-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:30:34.700029 zimran-events-0.3.1/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-07-19 08:30:21.000000 zimran-events-0.3.1/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:30:34.700029 zimran-events-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-19 08:30:21.000000 zimran-events-0.3.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-19 08:30:21.000000 zimran-events-0.3.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-07-19 08:30:21.000000 zimran-events-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-19 08:30:21.000000 zimran-events-0.3.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-19 08:30:21.000000 zimran-events-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-19 08:30:21.000000 zimran-events-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-19 08:30:34.700029 zimran-events-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-19 08:30:21.000000 zimran-events-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-19 08:30:21.000000 zimran-events-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-19 08:30:21.000000 zimran-events-0.3.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 08:30:34.700029 zimran-events-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:30:34.700029 zimran-events-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-19 08:30:21.000000 zimran-events-0.3.1/tests/test_legacy_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-19 08:30:21.000000 zimran-events-0.3.1/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:30:34.696029 zimran-events-0.3.1/zimran/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:30:34.700029 zimran-events-0.3.1/zimran/events/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-19 08:30:21.000000 zimran-events-0.3.1/zimran/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-07-19 08:30:21.000000 zimran-events-0.3.1/zimran/events/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-19 08:30:21.000000 zimran-events-0.3.1/zimran/events/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-07-19 08:30:21.000000 zimran-events-0.3.1/zimran/events/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-19 08:30:21.000000 zimran-events-0.3.1/zimran/events/dto.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-19 08:30:21.000000 zimran-events-0.3.1/zimran/events/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-19 08:30:21.000000 zimran-events-0.3.1/zimran/events/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-19 08:30:21.000000 zimran-events-0.3.1/zimran/events/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-19 08:30:21.000000 zimran-events-0.3.1/zimran/events/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-19 08:30:21.000000 zimran-events-0.3.1/zimran/events/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 08:30:34.700029 zimran-events-0.3.1/zimran_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-19 08:30:34.000000 zimran-events-0.3.1/zimran_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-19 08:30:34.000000 zimran-events-0.3.1/zimran_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 08:30:34.000000 zimran-events-0.3.1/zimran_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-19 08:30:34.000000 zimran-events-0.3.1/zimran_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-19 08:30:34.000000 zimran-events-0.3.1/zimran_events.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:59:52.244856 zimran-events-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-25 09:59:44.000000 zimran-events-0.3.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-25 09:59:44.000000 zimran-events-0.3.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-25 09:59:44.000000 zimran-events-0.3.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:59:52.240856 zimran-events-0.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:59:52.240856 zimran-events-0.3.2/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-07-25 09:59:44.000000 zimran-events-0.3.2/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:59:52.240856 zimran-events-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-25 09:59:44.000000 zimran-events-0.3.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-25 09:59:44.000000 zimran-events-0.3.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-07-25 09:59:44.000000 zimran-events-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-25 09:59:44.000000 zimran-events-0.3.2/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-25 09:59:44.000000 zimran-events-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-25 09:59:44.000000 zimran-events-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-25 09:59:52.244856 zimran-events-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-25 09:59:44.000000 zimran-events-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-25 09:59:44.000000 zimran-events-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-25 09:59:44.000000 zimran-events-0.3.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 09:59:52.244856 zimran-events-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:59:52.240856 zimran-events-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-25 09:59:44.000000 zimran-events-0.3.2/tests/test_legacy_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-25 09:59:44.000000 zimran-events-0.3.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:59:52.240856 zimran-events-0.3.2/zimran/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:59:52.244856 zimran-events-0.3.2/zimran/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-25 09:59:44.000000 zimran-events-0.3.2/zimran/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-07-25 09:59:44.000000 zimran-events-0.3.2/zimran/events/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-25 09:59:44.000000 zimran-events-0.3.2/zimran/events/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-07-25 09:59:44.000000 zimran-events-0.3.2/zimran/events/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-25 09:59:44.000000 zimran-events-0.3.2/zimran/events/dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-25 09:59:44.000000 zimran-events-0.3.2/zimran/events/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-25 09:59:44.000000 zimran-events-0.3.2/zimran/events/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-07-25 09:59:44.000000 zimran-events-0.3.2/zimran/events/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-25 09:59:44.000000 zimran-events-0.3.2/zimran/events/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-25 09:59:44.000000 zimran-events-0.3.2/zimran/events/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:59:52.244856 zimran-events-0.3.2/zimran_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-25 09:59:52.000000 zimran-events-0.3.2/zimran_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-25 09:59:52.000000 zimran-events-0.3.2/zimran_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 09:59:52.000000 zimran-events-0.3.2/zimran_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-25 09:59:52.000000 zimran-events-0.3.2/zimran_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 09:59:52.000000 zimran-events-0.3.2/zimran_events.egg-info/top_level.txt
```

### Comparing `zimran-events-0.3.1/.github/scripts/release.py` & `zimran-events-0.3.2/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.3.1/.github/workflows/publish.yml` & `zimran-events-0.3.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `zimran-events-0.3.1/.gitignore` & `zimran-events-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `zimran-events-0.3.1/.pre-commit-config.yaml` & `zimran-events-0.3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `zimran-events-0.3.1/LICENSE` & `zimran-events-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zimran-events-0.3.1/PKG-INFO` & `zimran-events-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zimran-events
-Version: 0.3.1
+Version: 0.3.2
 Summary: The zimran-events provides amqp interface
 Author-email: Talgat Abdraimov <abdraimov.talga@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Talgat Abdraimov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `zimran-events-0.3.1/README.md` & `zimran-events-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `zimran-events-0.3.1/pyproject.toml` & `zimran-events-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zimran-events"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
   { name="Talgat Abdraimov", email="abdraimov.talga@gmail.com" },
 ]
 description = "The zimran-events provides amqp interface"
 readme = "README.md"
 requires-python = ">=3.10"
 license = { file = "LICENSE" }
```

### Comparing `zimran-events-0.3.1/tests/test_utils.py` & `zimran-events-0.3.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.3.1/zimran/events/connection.py` & `zimran-events-0.3.2/zimran/events/connection.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.3.1/zimran/events/consumer.py` & `zimran-events-0.3.2/zimran/events/consumer.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.3.1/zimran/events/dto.py` & `zimran-events-0.3.2/zimran/events/dto.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.3.1/zimran/events/patterns.py` & `zimran-events-0.3.2/zimran/events/patterns.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.3.1/zimran/events/producer.py` & `zimran-events-0.3.2/zimran/events/producer.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,32 +11,32 @@
 except ImportError:
     import logging
 
     logger = logging.getLogger(__name__)
 
 
 from .connection import AsyncConnection, Connection
-from .schemas import ChannelPropertiesScheme, ExchangeScheme
+from .dto import ChannelProperties, Exchange
 from .utils import retry_policy, validate_channel_properties, validate_exchange
 
 
 class Producer(Connection):
     def __init__(self, *, broker_url: str, channel_number: int = 1):
         super().__init__(broker_url=broker_url, channel_number=channel_number)
 
     def publish(
         self,
         routing_key: str,
         *,
         payload: dict,
-        exchange: ExchangeScheme | None = None,
-        properties: ChannelPropertiesScheme | None = None,
+        exchange: Exchange | None = None,
+        properties: ChannelProperties | None = None,
     ):
         if properties is None:
-            properties = ChannelPropertiesScheme()
+            properties = ChannelProperties()
         else:
             validate_channel_properties(properties)
 
         basic_properties = pika.BasicProperties(**properties.as_dict(exclude_none=True))
         body = json.dumps(payload, default=str)
         if exchange is None:
             self.channel.basic_publish(exchange='', routing_key=routing_key, body=body, properties=basic_properties)
@@ -68,19 +68,19 @@
 
     @retry(retry_policy)
     async def publish(
         self,
         routing_key: str,
         *,
         payload: dict,
-        exchange: ExchangeScheme | None = None,
-        properties: ChannelPropertiesScheme | None = None,
+        exchange: Exchange | None = None,
+        properties: ChannelProperties | None = None,
     ):
         if properties is None:
-            properties = ChannelPropertiesScheme()
+            properties = ChannelProperties()
         else:
             validate_channel_properties(properties)
 
         message = self._get_message(properties=properties, payload=payload)
 
         channel = await self.channel
         if exchange is None:
@@ -96,9 +96,9 @@
             return_exceptions=True,
         )
 
         await declared_exchange.publish(message=message, routing_key=routing_key)
         logger.info(f'Message published to {exchange.name} exchange | routing_key: {routing_key}')
 
     @staticmethod
-    def _get_message(properties: ChannelPropertiesScheme, payload: dict):
+    def _get_message(properties: ChannelProperties, payload: dict):
         return aio_pika.Message(body=json.dumps(payload, default=str).encode(), **properties.as_dict(exclude_none=True))
```

### Comparing `zimran-events-0.3.1/zimran/events/utils.py` & `zimran-events-0.3.2/zimran/events/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
+import aioretry
 from aiormq.exceptions import AMQPChannelError, AMQPConnectionError
 
 
 try:
     from loguru import logger
 except ImportError:
     import logging
 
     logger = logging.getLogger(__name__)
 
+from .dto import ChannelProperties, Exchange
 from .exceptions import ChannelPropertiesTypeError, ExchangeTypeError
-from .schemas import ChannelPropertiesScheme, ExchangeScheme
 
 
-def validate_exchange(exchange: ExchangeScheme):
-    if not isinstance(exchange, ExchangeScheme):
-        raise ExchangeTypeError('ExchangeTypeError: <exchange> must be instance of <ExchangeScheme>')
+def validate_exchange(exchange: Exchange):
+    if not isinstance(exchange, Exchange):
+        raise ExchangeTypeError('ExchangeTypeError: <exchange> must be instance of <Exchange>')
 
 
-def validate_channel_properties(properties: ChannelPropertiesScheme):
-    if not isinstance(properties, ChannelPropertiesScheme):
+def validate_channel_properties(properties: ChannelProperties):
+    if not isinstance(properties, ChannelProperties):
         raise ChannelPropertiesTypeError(
-            'ChannelPropertiesTypeError: <properties> must be instance of <ChannelPropertiesScheme>',
+            'ChannelPropertiesTypeError: <properties> must be instance of <ChannelProperties>',
         )
 
 
 def cleanup_and_normalize_queue_name(queue_name: str):
     if '*' in queue_name:
         queue_name = queue_name.replace('*', '')
 
@@ -36,13 +37,13 @@
 
     if queue_name.endswith('.'):
         queue_name = queue_name[:-1]
 
     return f'{queue_name}_q'
 
 
-def retry_policy(info):
+def retry_policy(info: aioretry.RetryInfo):
     if isinstance(info.exception, (AMQPConnectionError, AMQPChannelError)):
         logger.warning(f'Retrying connection... | attempt amount: {info.fails}')
         return info.fails > 3, (info.fails - 1) * 2
 
     return True, 0
```

### Comparing `zimran-events-0.3.1/zimran_events.egg-info/PKG-INFO` & `zimran-events-0.3.2/zimran_events.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zimran-events
-Version: 0.3.1
+Version: 0.3.2
 Summary: The zimran-events provides amqp interface
 Author-email: Talgat Abdraimov <abdraimov.talga@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Talgat Abdraimov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `zimran-events-0.3.1/zimran_events.egg-info/SOURCES.txt` & `zimran-events-0.3.2/zimran_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

