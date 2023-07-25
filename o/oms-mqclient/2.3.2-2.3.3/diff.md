# Comparing `tmp/oms-mqclient-2.3.2.tar.gz` & `tmp/oms-mqclient-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oms-mqclient-2.3.2.tar", last modified: Mon Jul 17 21:02:07 2023, max compression
+gzip compressed data, was "oms-mqclient-2.3.3.tar", last modified: Tue Jul 25 17:23:55 2023, max compression
```

## Comparing `oms-mqclient-2.3.2.tar` & `oms-mqclient-2.3.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:02:07.970305 oms-mqclient-2.3.2/
--rw-r--r--   0 root         (0) root         (0)     1103 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2651 2023-07-17 21:02:07.970305 oms-mqclient-2.3.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1354 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:02:07.962304 oms-mqclient-2.3.2/mqclient/
--rw-r--r--   0 root         (0) root         (0)      582 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/mqclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6458 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/mqclient/broker_client_interface.py
--rw-r--r--   0 root         (0) root         (0)     1423 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/mqclient/broker_client_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:02:07.966304 oms-mqclient-2.3.2/mqclient/broker_clients/
--rw-r--r--   0 root         (0) root         (0)      113 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/mqclient/broker_clients/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14434 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/mqclient/broker_clients/apachepulsar.py
--rw-r--r--   0 root         (0) root         (0)    14181 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/mqclient/broker_clients/nats.py
--rw-r--r--   0 root         (0) root         (0)    16642 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/mqclient/broker_clients/rabbitmq.py
--rw-r--r--   0 root         (0) root         (0)     1925 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/mqclient/broker_clients/utils.py
--rw-r--r--   0 root         (0) root         (0)      378 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/mqclient/config.py
--rw-r--r--   0 root         (0) root         (0)     2133 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/mqclient/log_msgs.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/mqclient/py.typed
--rw-r--r--   0 root         (0) root         (0)    23738 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/mqclient/queue.py
--rw-r--r--   0 root         (0) root         (0)     2820 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/mqclient/telemetry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:02:07.966304 oms-mqclient-2.3.2/oms_mqclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2651 2023-07-17 21:02:07.000000 oms-mqclient-2.3.2/oms_mqclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1151 2023-07-17 21:02:07.000000 oms-mqclient-2.3.2/oms_mqclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 21:02:07.000000 oms-mqclient-2.3.2/oms_mqclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      298 2023-07-17 21:02:07.000000 oms-mqclient-2.3.2/oms_mqclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-17 21:02:07.000000 oms-mqclient-2.3.2/oms_mqclient.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2708 2023-07-17 21:02:07.970305 oms-mqclient-2.3.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      103 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:02:07.962304 oms-mqclient-2.3.2/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:02:07.966304 oms-mqclient-2.3.2/tests/abstract_broker_client_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/tests/abstract_broker_client_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9038 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/tests/abstract_broker_client_tests/integrate_broker_client_interface.py
--rw-r--r--   0 root         (0) root         (0)    35347 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/tests/abstract_broker_client_tests/integrate_queue.py
--rw-r--r--   0 root         (0) root         (0)    20234 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/tests/abstract_broker_client_tests/unit_tests.py
--rw-r--r--   0 root         (0) root         (0)     2058 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/tests/abstract_broker_client_tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:02:07.966304 oms-mqclient-2.3.2/tests/integrate/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/tests/integrate/__init__.py
--rw-r--r--   0 root         (0) root         (0)      962 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/tests/integrate/conftest.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/tests/integrate/test_nats.py
--rw-r--r--   0 root         (0) root         (0)      859 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/tests/integrate/test_pulsar.py
--rw-r--r--   0 root         (0) root         (0)      925 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/tests/integrate/test_rabbitmq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:02:07.966304 oms-mqclient-2.3.2/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:02:07.966304 oms-mqclient-2.3.2/tests/unit/pulsar/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/tests/unit/pulsar/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5586 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/tests/unit/pulsar/test_pulsar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 21:02:07.966304 oms-mqclient-2.3.2/tests/unit/rabbitmq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/tests/unit/rabbitmq/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9196 2023-07-17 21:02:05.000000 oms-mqclient-2.3.2/tests/unit/rabbitmq/test_rabbitmq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 17:23:55.600529 oms-mqclient-2.3.3/
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2651 2023-07-25 17:23:55.600529 oms-mqclient-2.3.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1354 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 17:23:55.596529 oms-mqclient-2.3.3/mqclient/
+-rw-r--r--   0 root         (0) root         (0)      582 2023-07-25 17:23:52.000000 oms-mqclient-2.3.3/mqclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6667 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/mqclient/broker_client_interface.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/mqclient/broker_client_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 17:23:55.600529 oms-mqclient-2.3.3/mqclient/broker_clients/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/mqclient/broker_clients/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14402 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/mqclient/broker_clients/apachepulsar.py
+-rw-r--r--   0 root         (0) root         (0)    14188 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/mqclient/broker_clients/nats.py
+-rw-r--r--   0 root         (0) root         (0)    17161 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/mqclient/broker_clients/rabbitmq.py
+-rw-r--r--   0 root         (0) root         (0)     1925 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/mqclient/broker_clients/utils.py
+-rw-r--r--   0 root         (0) root         (0)      395 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/mqclient/config.py
+-rw-r--r--   0 root         (0) root         (0)     2133 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/mqclient/log_msgs.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/mqclient/py.typed
+-rw-r--r--   0 root         (0) root         (0)    23781 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/mqclient/queue.py
+-rw-r--r--   0 root         (0) root         (0)     2820 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/mqclient/telemetry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 17:23:55.600529 oms-mqclient-2.3.3/oms_mqclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2651 2023-07-25 17:23:55.000000 oms-mqclient-2.3.3/oms_mqclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1151 2023-07-25 17:23:55.000000 oms-mqclient-2.3.3/oms_mqclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 17:23:55.000000 oms-mqclient-2.3.3/oms_mqclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      311 2023-07-25 17:23:55.000000 oms-mqclient-2.3.3/oms_mqclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-25 17:23:55.000000 oms-mqclient-2.3.3/oms_mqclient.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2722 2023-07-25 17:23:55.604529 oms-mqclient-2.3.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 17:23:55.596529 oms-mqclient-2.3.3/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 17:23:55.600529 oms-mqclient-2.3.3/tests/abstract_broker_client_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/tests/abstract_broker_client_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9038 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/tests/abstract_broker_client_tests/integrate_broker_client_interface.py
+-rw-r--r--   0 root         (0) root         (0)    38854 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/tests/abstract_broker_client_tests/integrate_queue.py
+-rw-r--r--   0 root         (0) root         (0)    20234 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/tests/abstract_broker_client_tests/unit_tests.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/tests/abstract_broker_client_tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 17:23:55.600529 oms-mqclient-2.3.3/tests/integrate/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/tests/integrate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      962 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/tests/integrate/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/tests/integrate/test_nats.py
+-rw-r--r--   0 root         (0) root         (0)      859 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/tests/integrate/test_pulsar.py
+-rw-r--r--   0 root         (0) root         (0)      925 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/tests/integrate/test_rabbitmq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 17:23:55.600529 oms-mqclient-2.3.3/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 17:23:55.600529 oms-mqclient-2.3.3/tests/unit/pulsar/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/tests/unit/pulsar/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5586 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/tests/unit/pulsar/test_pulsar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 17:23:55.600529 oms-mqclient-2.3.3/tests/unit/rabbitmq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/tests/unit/rabbitmq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9196 2023-07-25 17:23:51.000000 oms-mqclient-2.3.3/tests/unit/rabbitmq/test_rabbitmq.py
```

### Comparing `oms-mqclient-2.3.2/LICENSE` & `oms-mqclient-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.2/PKG-INFO` & `oms-mqclient-2.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oms-mqclient
-Version: 2.3.2
+Version: 2.3.3
 Summary: A Message Queue Client API Supporting Apache Pulsar, RabbitMQ, and NATS.io
 Home-page: https://github.com/Observation-Management-Service/MQClient
 Download-URL: https://pypi.org/project/oms-mqclient/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/MQClient/issues
```

### Comparing `oms-mqclient-2.3.2/README.md` & `oms-mqclient-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.2/mqclient/__init__.py` & `oms-mqclient-2.3.3/mqclient/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "2.3.2"
+__version__ = "2.3.3"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `oms-mqclient-2.3.2/mqclient/broker_client_interface.py` & `oms-mqclient-2.3.3/mqclient/broker_client_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Define an interface that broker_clients will adhere to."""
 
 
 import pickle
 from enum import Enum, auto
 from typing import Any, AsyncGenerator, Dict, Optional, Union
 
+from .config import MIN_PREFETCH
+
 MessageID = Union[int, str, bytes]
 
 
 class ConnectingFailedException(Exception):
     """Raised when a `connect()` fails."""
 
 
@@ -136,15 +138,22 @@
 
 class Sub(RawQueue):
     """Subscriber queue."""
 
     @property
     def prefetch(self) -> int:
         """Get prefetch."""
-        return self._prefetch  # type: ignore[attr-defined, no-any-return]
+        return self._prefetch
+
+    @prefetch.setter
+    def prefetch(self, val: int) -> None:
+        """Set prefetch."""
+        if val < MIN_PREFETCH:
+            raise ValueError(f"prefetch must be >= {MIN_PREFETCH}")
+        self._prefetch = val
 
     @staticmethod
     def _to_message(*args: Any) -> Optional[Message]:
         """Convert broker_client-specific payload to standardized Message
         type."""
         raise NotImplementedError()
```

### Comparing `oms-mqclient-2.3.2/mqclient/broker_client_manager.py` & `oms-mqclient-2.3.3/mqclient/broker_client_manager.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.2/mqclient/broker_clients/apachepulsar.py` & `oms-mqclient-2.3.3/mqclient/broker_clients/apachepulsar.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         ack_timeout: Optional[int],
         prefetch: int,
     ) -> None:
         LOGGER.debug(f"{log_msgs.INIT_SUB} ({address}; {topic})")
         super().__init__(address, topic, auth_token, ack_timeout)
         self.consumer: pulsar.Consumer = None
         self.subscription_name = subscription_name
-        self._prefetch = prefetch  # see `Sub.prefetch` property
+        self.prefetch = prefetch
 
     async def connect(self) -> None:
         """Connect to subscriber."""
         LOGGER.debug(log_msgs.CONNECTING_SUB)
         await super().connect()
 
         self.consumer = self.client.subscribe(
```

### Comparing `oms-mqclient-2.3.2/mqclient/broker_clients/nats.py` & `oms-mqclient-2.3.3/mqclient/broker_clients/nats.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,19 +131,25 @@
     """Wrapper around queue with prefetch-queue, using JetStream.
 
     Extends:
         NATS
         Sub
     """
 
-    def __init__(self, endpoint: str, stream_id: str, subject: str, prefetch: int):
+    def __init__(
+        self,
+        endpoint: str,
+        stream_id: str,
+        subject: str,
+        prefetch: int,
+    ):
         LOGGER.debug(f"{log_msgs.INIT_SUB} ({endpoint}; {stream_id}; {subject})")
         super().__init__(endpoint, stream_id, subject)
         self._subscription: Optional[nats.js.JetStreamContext.PullSubscription] = None
-        self._prefetch = prefetch  # see `Sub.prefetch` property
+        self.prefetch = prefetch
 
     async def connect(self) -> None:
         """Set up sub (pull subscription)."""
         LOGGER.debug(log_msgs.CONNECTING_SUB)
         await super().connect()
         if not self.js:
             raise RuntimeError("JetStream is not connected.")
@@ -354,15 +360,15 @@
         if not self._subscription:
             raise RuntimeError("subscriber is not connected")
 
         msg = None
         try:
             gen = self._gen_messages(
                 timeout * 1000,
-                self.prefetch + 1,  # prefetch + 1 = # of msgs pulled
+                self.prefetch,  # prefetch = # of msgs pulled
                 retries,
                 retry_delay,
             )
             while True:
                 # get message
                 LOGGER.debug(log_msgs.MSGGEN_GET_NEW_MESSAGE)
                 msg = await _anext(gen, None)
```

### Comparing `oms-mqclient-2.3.2/mqclient/broker_clients/rabbitmq.py` & `oms-mqclient-2.3.3/mqclient/broker_clients/rabbitmq.py`

 * *Files 8% similar despite different names*

```diff
@@ -138,17 +138,23 @@
     """Wrapper around queue with delivery-confirm mode in the channel.
 
     Extends:
         RabbitMQ
         Pub
     """
 
-    def __init__(self, *args: Any, **kwargs: Any) -> None:
-        LOGGER.debug(f"{log_msgs.INIT_PUB} ({args}; {kwargs})")
-        super().__init__(*args, **kwargs)
+    def __init__(
+        self,
+        address: str,
+        name: str,
+        auth_token: str,
+        ack_timeout: Optional[int],
+    ) -> None:
+        LOGGER.debug(f"{log_msgs.INIT_PUB} ({address}; {name})")
+        super().__init__(address, name, auth_token, ack_timeout)
 
     async def connect(self) -> None:
         """Set up connection, channel, and queue.
 
         Turn on delivery confirmations.
         """
         LOGGER.debug(log_msgs.CONNECTING_PUB)
@@ -222,32 +228,43 @@
     """Wrapper around queue with prefetch-queue QoS.
 
     Extends:
         RabbitMQ
         Sub
     """
 
-    def __init__(self, *args: Any, prefetch: int, **kwargs: Any) -> None:
-        LOGGER.debug(f"{log_msgs.INIT_SUB} ({args}; {kwargs})")
-        super().__init__(*args, **kwargs)
+    def __init__(
+        self,
+        address: str,
+        name: str,
+        auth_token: str,
+        ack_timeout: Optional[int],
+        prefetch: int,
+    ) -> None:
+        LOGGER.debug(f"{log_msgs.INIT_SUB} ({address}; {name})")
+        super().__init__(address, name, auth_token, ack_timeout)
         self.consumer_id = None
-        self._prefetch = prefetch  # see `Sub.prefetch` property
+        self.prefetch = prefetch
 
     async def connect(self) -> None:
         """Set up connection, channel, and queue.
 
         Turn on prefetching.
         """
         LOGGER.debug(log_msgs.CONNECTING_SUB)
         await super().connect()
 
         if not self.channel:
             raise ConnectingFailedException("No channel to configure connection.")
 
-        self.channel.basic_qos(prefetch_count=self.prefetch)
+        self.channel.basic_qos(prefetch_count=max(self.prefetch, 1))
+        # Setting the value to 0 lets the consumer drain the entire queue.
+        # https://www.cloudamqp.com/blog/rabbitmq-basic-consume-vs-rabbitmq-basic-get.html#what-are-the-advantages-of-a-rabbitmq-consumer
+        # https://www.cloudamqp.com/blog/part1-rabbitmq-best-practice.html#prefetch
+        #
         # https://www.rabbitmq.com/consumer-prefetch.html
         #    Meaning of prefetch_count in RabbitMQ w/ global_qos=False:
         #    applied separately to each new consumer on the channel
         #
         # global_qos=False b/c using quorum queues
         # https://www.rabbitmq.com/quorum-queues.html#global-qos
```

### Comparing `oms-mqclient-2.3.2/mqclient/broker_clients/utils.py` & `oms-mqclient-2.3.3/mqclient/broker_clients/utils.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.2/mqclient/log_msgs.py` & `oms-mqclient-2.3.3/mqclient/log_msgs.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.2/mqclient/queue.py` & `oms-mqclient-2.3.3/mqclient/queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from .broker_client_interface import AckException, Message, NackException, Pub, Sub
 from .config import (
     DEFAULT_EXCEPT_ERRORS,
     DEFAULT_PREFETCH,
     DEFAULT_RETRIES,
     DEFAULT_RETRY_DELAY,
     DEFAULT_TIMEOUT,
+    MIN_PREFETCH,
 )
 
 LOGGER = logging.getLogger("mqclient")
 
 
 # deprecation check
 for envvar in ["RABBITMQ_HEARTBEAT", "PULSAR_UNACKED_MESSAGES_TIMEOUT_SEC"]:
@@ -39,15 +40,15 @@
 class Queue:
     """User-facing queue library.
 
     Args:
         broker_client: the broker_client to use
         address: address of queue
         name: name of queue
-        prefetch: size of prefetch buffer for receiving messages
+        prefetch: size of prefetch buffer for receiving messages (min 1)
         timeout: seconds to wait for a message to be delivered
         ack_timeout: max time (seconds) to acknowledge a message
                      before broker considers it lost (and re-queues)
         except_errors: whether to suppress interior context errors for
                         the consumer (when `True`, the context manager
                         will act like a `try-except` block)
         auth_token: the (jwt) authentication token
@@ -66,16 +67,16 @@
         except_errors: bool = DEFAULT_EXCEPT_ERRORS,
         auth_token: str = "",
     ) -> None:
         self._broker_client = broker_client_manager.get_broker_client(broker_client)
         self._address = address
         self._name = name if name else Queue.make_name()
 
-        if prefetch < 0:
-            raise ValueError("prefetch must be non-negative")
+        if prefetch < MIN_PREFETCH:
+            raise ValueError(f"prefetch must be >= {MIN_PREFETCH}")
         self._prefetch = prefetch
 
         self._auth_token = auth_token
 
         if ack_timeout is not None and ack_timeout <= 0:
             raise ValueError("timeout must be positive")
         self._ack_timeout = ack_timeout
```

### Comparing `oms-mqclient-2.3.2/mqclient/telemetry.py` & `oms-mqclient-2.3.3/mqclient/telemetry.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.2/oms_mqclient.egg-info/PKG-INFO` & `oms-mqclient-2.3.3/oms_mqclient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oms-mqclient
-Version: 2.3.2
+Version: 2.3.3
 Summary: A Message Queue Client API Supporting Apache Pulsar, RabbitMQ, and NATS.io
 Home-page: https://github.com/Observation-Management-Service/MQClient
 Download-URL: https://pypi.org/project/oms-mqclient/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/MQClient/issues
```

### Comparing `oms-mqclient-2.3.2/oms_mqclient.egg-info/SOURCES.txt` & `oms-mqclient-2.3.3/oms_mqclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.2/setup.cfg` & `oms-mqclient-2.3.3/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -82,14 +82,15 @@
 	pytest-asyncio
 	pytest-mock
 	mock
 	coloredlogs
 integration = 
 	wipac-keycloak-rest-services
 	wipac-rest-tools
+	pytest-xdist
 
 [options.package_data]
 * = py.typed
 
 [options.packages.find]
 exclude = 
 	test
```

### Comparing `oms-mqclient-2.3.2/tests/abstract_broker_client_tests/integrate_broker_client_interface.py` & `oms-mqclient-2.3.3/tests/abstract_broker_client_tests/integrate_broker_client_interface.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.2/tests/abstract_broker_client_tests/integrate_queue.py` & `oms-mqclient-2.3.3/tests/abstract_broker_client_tests/integrate_queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import random
 from multiprocessing.dummy import Pool as ThreadPool
 from typing import Any, List, Optional
 from unittest.mock import patch
 
 import asyncstdlib as asl
 import pytest
-from mqclient.queue import Queue
+from mqclient.queue import EmptyQueueException, Queue
 
 from .utils import (
     DATA_LIST,
     _log_recv,
     _log_recv_multiple,
     _log_send,
     all_were_received,
@@ -39,29 +39,32 @@
 
 
 #
 # tests
 #
 
 
+PREFETCH_TEST_VALUES = [None, 1, 2, len(DATA_LIST), 50]
+
+
 class PubSubQueue:
     """Integration test suite for Queue objects."""
 
     broker_client: str = ""
 
     ###########################################################################
     # tests 000 - 099:
     #
     # Testing scenarios with different numbers of sub and/or pubs
     # to see no data loss
     ###########################################################################
 
     @pytest.mark.asyncio
     @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
-    async def test_010(self, queue_name: str, auth_token: str) -> None:
+    async def test_000(self, queue_name: str, auth_token: str) -> None:
         """Test one pub, one sub."""
         all_recvd: List[Any] = []
 
         pub_sub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
         async with pub_sub.open_pub() as p:
             await p.send(DATA_LIST[0])
             _log_send(DATA_LIST[0])
@@ -82,15 +85,15 @@
                 all_recvd.append(_log_recv(d))
                 # assert d == DATA_LIST[i]  # we don't guarantee order
 
         assert all_were_received(all_recvd, [DATA_LIST[0]] + DATA_LIST)
 
     @pytest.mark.asyncio
     @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
-    async def test_011(self, queue_name: str, auth_token: str) -> None:
+    async def test_001(self, queue_name: str, auth_token: str) -> None:
         """Test an individual pub and an individual sub."""
         all_recvd: List[Any] = []
 
         pub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
         async with pub.open_pub() as p:
             await p.send(DATA_LIST[0])
             _log_send(DATA_LIST[0])
@@ -112,15 +115,15 @@
                 all_recvd.append(_log_recv(d))
                 # assert d == DATA_LIST[i]  # we don't guarantee order
 
         assert all_were_received(all_recvd, [DATA_LIST[0]] + DATA_LIST)
 
     @pytest.mark.asyncio
     @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
-    async def test_012(self, queue_name: str, auth_token: str) -> None:
+    async def test_002(self, queue_name: str, auth_token: str) -> None:
         """Failure-test one pub, two subs (one subscribed to wrong queue)."""
         all_recvd: List[Any] = []
 
         async with Queue(
             self.broker_client, name=queue_name, auth_token=auth_token
         ).open_pub() as p:
             await p.send(DATA_LIST[0])
@@ -137,15 +140,15 @@
             all_recvd.append(_log_recv(d))
             assert d == DATA_LIST[0]
 
         assert all_were_received(all_recvd, [DATA_LIST[0]])
 
     @pytest.mark.asyncio
     @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
-    async def test_020(self, queue_name: str, auth_token: str) -> None:
+    async def test_010(self, queue_name: str, auth_token: str) -> None:
         """Test one pub, multiple subs, ordered/alternatingly."""
         all_recvd: List[Any] = []
 
         # for each send, create and receive message via a new sub
         async with Queue(
             self.broker_client, name=queue_name, auth_token=auth_token
         ).open_pub() as p:
@@ -157,74 +160,196 @@
                     self.broker_client, name=queue_name, auth_token=auth_token
                 ).open_sub_one() as d:
                     all_recvd.append(_log_recv(d))
                     assert d == data
 
         assert all_were_received(all_recvd)
 
-    async def _test_021(self, queue_name: str, num_subs: int, auth_token: str) -> None:
-        """Test one pub, multiple subs, unordered (front-loaded sending)."""
+    @pytest.mark.asyncio
+    @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
+    @pytest.mark.parametrize(
+        "num_subs",
+        [
+            len(DATA_LIST) // 2,
+            len(DATA_LIST),
+            len(DATA_LIST) ** 2,
+        ],
+    )
+    async def test_020(self, queue_name: str, auth_token: str, num_subs: int) -> None:
+        """Test one pub, multiple subs, unordered (front-loaded sending).
+
+        Uses `open_sub()`
+        """
+        all_recvd: List[Any] = []
+
+        async with Queue(
+            self.broker_client, name=queue_name, auth_token=auth_token
+        ).open_pub() as p:
+            for data in DATA_LIST:
+                await p.send(data)
+                _log_send(data)
+
+        subs = []
+        for _ in range(num_subs):
+            subs.append(
+                Queue(
+                    self.broker_client,
+                    name=queue_name,
+                    auth_token=auth_token,
+                    timeout=1,
+                )
+            )
+            await asyncio.sleep(0.1)
+
+        for i, sub in enumerate(subs):
+            async with sub.open_sub() as gen:
+                recv_data_list = [_log_recv(m) async for m in gen]
+                if i < len(DATA_LIST):
+                    assert recv_data_list
+                else:
+                    assert not recv_data_list
+                all_recvd.extend(recv_data_list)
+
+        assert all_were_received(all_recvd)
+
+    @pytest.mark.asyncio
+    @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
+    @pytest.mark.parametrize(
+        "num_subs",
+        [
+            len(DATA_LIST) // 2,
+            len(DATA_LIST),
+            len(DATA_LIST) ** 2,
+        ],
+    )
+    async def test_021__threaded(
+        self, queue_name: str, auth_token: str, num_subs: int
+    ) -> None:
+        """Test one pub, multiple subs, unordered (front-loaded sending).
+
+        Uses `open_sub()`
+        """
         all_recvd: List[Any] = []
 
         async with Queue(
             self.broker_client, name=queue_name, auth_token=auth_token
         ).open_pub() as p:
             for data in DATA_LIST:
                 await p.send(data)
                 _log_send(data)
 
-        async def recv_thread(_: int) -> List[Any]:
+        async def recv_thread(i: int) -> List[Any]:
             sub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
             sub.timeout = 1
             async with sub.open_sub() as gen:
                 recv_data_list = [m async for m in gen]
             return _log_recv_multiple(recv_data_list)
 
         def start_recv_thread(num_id: int) -> Any:
             return asyncio.run(recv_thread(num_id))
 
         with ThreadPool(num_subs) as pool:
             received_data = pool.map(start_recv_thread, range(num_subs))
-        all_recvd.extend(item for sublist in received_data for item in sublist)
+
+        n_subs_that_got_msgs = 0
+        for sublist in received_data:
+            if sublist:
+                n_subs_that_got_msgs += 1
+                all_recvd.extend(sublist)
+        # since threads are mixed, can't test like test_020
+        if num_subs < len(DATA_LIST):
+            assert n_subs_that_got_msgs == num_subs
+        else:
+            logging.debug(f"{n_subs_that_got_msgs=}")
+            assert n_subs_that_got_msgs == len(DATA_LIST)
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
     @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
-    async def test_021_fewer(self, queue_name: str, auth_token: str) -> None:
+    async def test_030(self, queue_name: str, auth_token: str) -> None:
         """Test one pub, multiple subs, unordered (front-loaded sending).
 
-        Fewer subs than messages.
+        Use the same number of subs as number of messages.
+
+        Uses `open_sub_one()`
         """
-        await self._test_021(queue_name, len(DATA_LIST) // 2, auth_token)
+        all_recvd: List[Any] = []
 
-    @pytest.mark.asyncio
-    @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
-    async def test_021_same(self, queue_name: str, auth_token: str) -> None:
-        """Test one pub, multiple subs, unordered (front-loaded sending).
+        async with Queue(
+            self.broker_client, name=queue_name, auth_token=auth_token
+        ).open_pub() as p:
+            for data in DATA_LIST:
+                await p.send(data)
+                _log_send(data)
 
-        Same number of subs as messages.
-        """
-        await self._test_021(queue_name, len(DATA_LIST), auth_token)
+        subs = [
+            Queue(
+                self.broker_client,
+                name=queue_name,
+                auth_token=auth_token,
+                timeout=1,
+            )
+            for _ in range(len(DATA_LIST))
+        ]
+
+        for sub in subs:
+            async with sub.open_sub_one() as m:
+                all_recvd.append(_log_recv(m))
+
+        assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
     @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
-    async def test_021_more(self, queue_name: str, auth_token: str) -> None:
-        """Test one pub, multiple subs, unordered (front-loaded sending).
+    async def test_031(self, queue_name: str, auth_token: str) -> None:
+        """Failure-test one pub, and too many subs.
 
-        More subs than messages.
+        More subs than messages with `open_sub_one()` will raise an
+        exception.
+
+        Uses `open_sub_one()`
         """
-        await self._test_021(queue_name, len(DATA_LIST) ** 2, auth_token)
+        all_recvd: List[Any] = []
+
+        async with Queue(
+            self.broker_client, name=queue_name, auth_token=auth_token
+        ).open_pub() as p:
+            for data in DATA_LIST:
+                await p.send(data)
+                _log_send(data)
+
+        subs = [
+            Queue(
+                self.broker_client,
+                name=queue_name,
+                auth_token=auth_token,
+                timeout=1,
+            )
+            for _ in range(len(DATA_LIST) + 1)
+        ]
+
+        for i, sub in enumerate(subs):
+            if i == len(DATA_LIST):
+                with pytest.raises(EmptyQueueException):
+                    async with sub.open_sub_one() as m:
+                        all_recvd.append(_log_recv(m))
+            else:
+                async with sub.open_sub_one() as m:
+                    all_recvd.append(_log_recv(m))
+
+        assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
     @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
-    async def test_022(self, queue_name: str, auth_token: str) -> None:
+    async def test_032__threaded(self, queue_name: str, auth_token: str) -> None:
         """Test one pub, multiple subs, unordered (front-loaded sending).
 
         Use the same number of subs as number of messages.
+
+        Uses `open_sub_one()`
         """
         all_recvd: List[Any] = []
 
         async with Queue(
             self.broker_client, name=queue_name, auth_token=auth_token
         ).open_pub() as p:
             for data in DATA_LIST:
@@ -244,19 +369,21 @@
         with ThreadPool(len(DATA_LIST)) as pool:
             all_recvd = pool.map(start_recv_thread, range(len(DATA_LIST)))
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
     @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
-    async def test_023(self, queue_name: str, auth_token: str) -> None:
+    async def test_033__threaded(self, queue_name: str, auth_token: str) -> None:
         """Failure-test one pub, and too many subs.
 
         More subs than messages with `open_sub_one()` will raise an
         exception.
+
+        Uses `open_sub_one()`
         """
         all_recvd: List[Any] = []
 
         async with Queue(
             self.broker_client, name=queue_name, auth_token=auth_token
         ).open_pub() as p:
             for data in DATA_LIST:
@@ -273,22 +400,22 @@
         def start_recv_thread(num_id: int) -> Any:
             return asyncio.run(recv_thread(num_id))
 
         with ThreadPool(len(DATA_LIST)) as pool:
             all_recvd = pool.map(start_recv_thread, range(len(DATA_LIST)))
 
         # Extra Sub
-        with pytest.raises(Exception):
+        with pytest.raises(EmptyQueueException):
             await recv_thread(-1)
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
     @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
-    async def test_030(self, queue_name: str, auth_token: str) -> None:
+    async def test_060(self, queue_name: str, auth_token: str) -> None:
         """Test multiple pubs, one sub, ordered/alternatingly."""
         all_recvd: List[Any] = []
 
         sub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
 
         for data in DATA_LIST:
             async with Queue(
@@ -306,15 +433,15 @@
             assert len(received_data) == 1
             assert data == received_data[0]
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
     @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
-    async def test_031(self, queue_name: str, auth_token: str) -> None:
+    async def test_061(self, queue_name: str, auth_token: str) -> None:
         """Test multiple pubs, one sub, unordered (front-loaded sending)."""
         all_recvd: List[Any] = []
 
         for data in DATA_LIST:
             async with Queue(
                 self.broker_client, name=queue_name, auth_token=auth_token
             ).open_pub() as p:
@@ -327,15 +454,15 @@
             received_data = [m async for m in gen]
         all_recvd.extend(_log_recv_multiple(received_data))
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
     @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
-    async def test_040(self, queue_name: str, auth_token: str) -> None:
+    async def test_080(self, queue_name: str, auth_token: str) -> None:
         """Test multiple pubs, multiple subs, ordered/alternatingly.
 
         Use the same number of pubs as subs.
         """
         all_recvd: List[Any] = []
 
         for data in DATA_LIST:
@@ -345,24 +472,25 @@
                 await p.send(data)
                 _log_send(data)
 
             sub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
             sub.timeout = 1
             async with sub.open_sub() as gen:
                 received_data = [m async for m in gen]
+            assert received_data
             all_recvd.extend(_log_recv_multiple(received_data))
 
             assert len(received_data) == 1
             assert data == received_data[0]
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
     @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
-    async def test_041(self, queue_name: str, auth_token: str) -> None:
+    async def test_081(self, queue_name: str, auth_token: str) -> None:
         """Test multiple pubs, multiple subs, unordered (front-loaded sending).
 
         Use the same number of pubs as subs.
         """
         all_recvd: List[Any] = []
 
         for data in DATA_LIST:
@@ -378,15 +506,15 @@
             ).open_sub_one() as d:
                 all_recvd.append(_log_recv(d))
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
     @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
-    async def test_042(self, queue_name: str, auth_token: str) -> None:
+    async def test_082(self, queue_name: str, auth_token: str) -> None:
         """Test multiple pubs, multiple subs, unordered (front-loaded sending).
 
         Use the more pubs than subs.
         """
         all_recvd: List[Any] = []
 
         for data in DATA_LIST:
@@ -402,15 +530,15 @@
             async with sub.open_sub_one() as d:
                 all_recvd.append(_log_recv(d))
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
     @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
-    async def test_043(self, queue_name: str, auth_token: str) -> None:
+    async def test_083(self, queue_name: str, auth_token: str) -> None:
         """Test multiple pubs, multiple subs, unordered (front-loaded sending).
 
         Use the fewer pubs than subs.
         """
         all_recvd: List[Any] = []
 
         for data_pairs in [DATA_LIST[i : i + 2] for i in range(0, len(DATA_LIST), 2)]:
@@ -427,15 +555,15 @@
             ).open_sub_one() as d:
                 all_recvd.append(_log_recv(d))
 
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
     @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
-    async def test_050(self, queue_name: str, auth_token: str) -> None:
+    async def test_090(self, queue_name: str, auth_token: str) -> None:
         """Test_20 with variable prefetching.
 
         One pub, multiple subs.
         """
         all_recvd: List[Any] = []
 
         async with Queue(
@@ -457,15 +585,15 @@
                         all_recvd.append(_log_recv(d))
                         assert d == data
 
         assert all_were_received(all_recvd, DATA_LIST * ((len(DATA_LIST) * 2) - 1))
 
     @pytest.mark.asyncio
     @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
-    async def test_051(self, queue_name: str, auth_token: str) -> None:
+    async def test_091(self, queue_name: str, auth_token: str) -> None:
         """Test one pub, multiple subs, with prefetching.
 
         Prefetching should have no visible affect.
         """
         all_recvd: List[Any] = []
 
         for data in DATA_LIST:
@@ -650,15 +778,15 @@
     # tests 200 - 299:
     #
     # Tests for open_sub_manual_acking()
     ###########################################################################
 
     @pytest.mark.asyncio
     @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
-    @pytest.mark.parametrize("sub_queue_prefetch", [None, 0, 1, 2, 50])
+    @pytest.mark.parametrize("sub_queue_prefetch", PREFETCH_TEST_VALUES)
     async def test_200__ideal(
         self,
         queue_name: str,
         auth_token: str,
         sub_queue_prefetch: Optional[int],
     ) -> None:
         """Test open_sub_manual_acking() ideal scenario."""
@@ -693,15 +821,15 @@
                 await gen.ack(msg)
 
         print(all_recvd)
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
     @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
-    @pytest.mark.parametrize("sub_queue_prefetch", [None, 0, 1, 2, 50])
+    @pytest.mark.parametrize("sub_queue_prefetch", PREFETCH_TEST_VALUES)
     async def test_202__delayed_mixed_acking_nacking(
         self,
         queue_name: str,
         auth_token: str,
         sub_queue_prefetch: Optional[int],
     ) -> None:
         """Test open_sub_manual_acking() fail and immediate recovery with
@@ -755,15 +883,15 @@
                 await gen.ack(msg)
 
         print(all_recvd)
         assert all_were_received(all_recvd)
 
     @pytest.mark.asyncio
     @patch(CI_TEST_RETRY_TRIGGER, new=fail_first_try)
-    @pytest.mark.parametrize("sub_queue_prefetch", [None, 0, 1, 2, 50])
+    @pytest.mark.parametrize("sub_queue_prefetch", PREFETCH_TEST_VALUES)
     async def test_204__post_ack(
         self,
         queue_name: str,
         auth_token: str,
         sub_queue_prefetch: Optional[int],
     ) -> None:
         """Test open_sub_manual_acking() where messages aren't acked until
```

### Comparing `oms-mqclient-2.3.2/tests/abstract_broker_client_tests/unit_tests.py` & `oms-mqclient-2.3.3/tests/abstract_broker_client_tests/unit_tests.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.2/tests/abstract_broker_client_tests/utils.py` & `oms-mqclient-2.3.3/tests/abstract_broker_client_tests/utils.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.2/tests/integrate/conftest.py` & `oms-mqclient-2.3.3/tests/integrate/conftest.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.2/tests/integrate/test_nats.py` & `oms-mqclient-2.3.3/tests/integrate/test_nats.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.2/tests/integrate/test_pulsar.py` & `oms-mqclient-2.3.3/tests/integrate/test_pulsar.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.2/tests/integrate/test_rabbitmq.py` & `oms-mqclient-2.3.3/tests/integrate/test_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.2/tests/unit/pulsar/test_pulsar.py` & `oms-mqclient-2.3.3/tests/unit/pulsar/test_pulsar.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.3.2/tests/unit/rabbitmq/test_rabbitmq.py` & `oms-mqclient-2.3.3/tests/unit/rabbitmq/test_rabbitmq.py`

 * *Files identical despite different names*

