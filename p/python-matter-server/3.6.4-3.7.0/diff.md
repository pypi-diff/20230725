# Comparing `tmp/python-matter-server-3.6.4.tar.gz` & `tmp/python-matter-server-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-matter-server-3.6.4.tar", last modified: Wed Jul 12 18:46:49 2023, max compression
+gzip compressed data, was "python-matter-server-3.7.0.tar", last modified: Tue Jul 25 16:26:55 2023, max compression
```

## Comparing `python-matter-server-3.6.4.tar` & `python-matter-server-3.7.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:46:49.973142 python-matter-server-3.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-07-12 18:46:49.973142 python-matter-server-3.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:46:49.969142 python-matter-server-3.6.4/matter_server/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:46:49.969142 python-matter-server-3.6.4/matter_server/client/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19354 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:46:49.969142 python-matter-server-3.6.4/matter_server/client/models/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14062 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/client/models/device_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/client/models/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:46:49.969142 python-matter-server-3.6.4/matter_server/common/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/common/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/common/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:46:49.969142 python-matter-server-3.6.4/matter_server/common/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/common/helpers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/common/helpers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/common/helpers/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/common/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:46:49.973142 python-matter-server-3.6.4/matter_server/server/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/server/client_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/server/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    37306 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/server/device_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:46:49.973142 python-matter-server-3.6.4/matter_server/server/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/server/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/server/helpers/paa_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/server/stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/server/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/server/vendor_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-12 18:46:38.000000 python-matter-server-3.6.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:46:49.973142 python-matter-server-3.6.4/python_matter_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-07-12 18:46:49.000000 python-matter-server-3.6.4/python_matter_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-12 18:46:49.000000 python-matter-server-3.6.4/python_matter_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:46:49.000000 python-matter-server-3.6.4/python_matter_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-12 18:46:49.000000 python-matter-server-3.6.4/python_matter_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:46:47.000000 python-matter-server-3.6.4/python_matter_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-12 18:46:49.000000 python-matter-server-3.6.4/python_matter_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-12 18:46:49.000000 python-matter-server-3.6.4/python_matter_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-12 18:46:49.973142 python-matter-server-3.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:26:55.122351 python-matter-server-3.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-07-25 16:26:43.000000 python-matter-server-3.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-07-25 16:26:55.122351 python-matter-server-3.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-07-25 16:26:43.000000 python-matter-server-3.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:26:55.118351 python-matter-server-3.7.0/matter_server/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-25 16:26:43.000000 python-matter-server-3.7.0/matter_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:26:55.118351 python-matter-server-3.7.0/matter_server/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-25 16:26:43.000000 python-matter-server-3.7.0/matter_server/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19850 2023-07-25 16:26:43.000000 python-matter-server-3.7.0/matter_server/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-07-25 16:26:43.000000 python-matter-server-3.7.0/matter_server/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-25 16:26:43.000000 python-matter-server-3.7.0/matter_server/client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:26:55.118351 python-matter-server-3.7.0/matter_server/client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-25 16:26:43.000000 python-matter-server-3.7.0/matter_server/client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14062 2023-07-25 16:26:43.000000 python-matter-server-3.7.0/matter_server/client/models/device_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-07-25 16:26:43.000000 python-matter-server-3.7.0/matter_server/client/models/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:26:55.118351 python-matter-server-3.7.0/matter_server/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-25 16:26:43.000000 python-matter-server-3.7.0/matter_server/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-25 16:26:43.000000 python-matter-server-3.7.0/matter_server/common/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-25 16:26:43.000000 python-matter-server-3.7.0/matter_server/common/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:26:55.118351 python-matter-server-3.7.0/matter_server/common/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-25 16:26:43.000000 python-matter-server-3.7.0/matter_server/common/helpers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-25 16:26:43.000000 python-matter-server-3.7.0/matter_server/common/helpers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-07-25 16:26:43.000000 python-matter-server-3.7.0/matter_server/common/helpers/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-25 16:26:43.000000 python-matter-server-3.7.0/matter_server/common/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 16:26:43.000000 python-matter-server-3.7.0/matter_server/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:26:55.122351 python-matter-server-3.7.0/matter_server/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-25 16:26:43.000000 python-matter-server-3.7.0/matter_server/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-25 16:26:43.000000 python-matter-server-3.7.0/matter_server/server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-07-25 16:26:43.000000 python-matter-server-3.7.0/matter_server/server/client_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-25 16:26:43.000000 python-matter-server-3.7.0/matter_server/server/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38431 2023-07-25 16:26:43.000000 python-matter-server-3.7.0/matter_server/server/device_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:26:55.122351 python-matter-server-3.7.0/matter_server/server/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-25 16:26:43.000000 python-matter-server-3.7.0/matter_server/server/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-25 16:26:43.000000 python-matter-server-3.7.0/matter_server/server/helpers/paa_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-07-25 16:26:43.000000 python-matter-server-3.7.0/matter_server/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-25 16:26:43.000000 python-matter-server-3.7.0/matter_server/server/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-07-25 16:26:43.000000 python-matter-server-3.7.0/matter_server/server/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-07-25 16:26:43.000000 python-matter-server-3.7.0/matter_server/server/vendor_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-25 16:26:45.000000 python-matter-server-3.7.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:26:55.122351 python-matter-server-3.7.0/python_matter_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-07-25 16:26:54.000000 python-matter-server-3.7.0/python_matter_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-25 16:26:55.000000 python-matter-server-3.7.0/python_matter_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 16:26:54.000000 python-matter-server-3.7.0/python_matter_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-25 16:26:54.000000 python-matter-server-3.7.0/python_matter_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 16:26:53.000000 python-matter-server-3.7.0/python_matter_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-25 16:26:54.000000 python-matter-server-3.7.0/python_matter_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 16:26:54.000000 python-matter-server-3.7.0/python_matter_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-25 16:26:55.122351 python-matter-server-3.7.0/setup.cfg
```

### Comparing `python-matter-server-3.6.4/LICENSE` & `python-matter-server-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.4/PKG-INFO` & `python-matter-server-3.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-matter-server
-Version: 3.6.4
+Version: 3.7.0
 Summary: Python Matter WebSocket Server
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
```

### Comparing `python-matter-server-3.6.4/README.md` & `python-matter-server-3.7.0/README.md`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.4/matter_server/client/client.py` & `python-matter-server-3.7.0/matter_server/client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from ..common.models import (
     APICommand,
     CommandMessage,
     ErrorResultMessage,
     EventMessage,
     EventType,
     MatterNodeData,
+    MatterNodeEvent,
     MessageType,
     ResultMessageBase,
     ServerDiagnostics,
     ServerInfoMessage,
     SuccessResultMessage,
 )
 from .connection import MatterClientConnection
@@ -482,14 +483,27 @@
                 attribute_path=attribute_path,
             )
             return
         if msg.event == EventType.ENDPOINT_ADDED:
             node_id = msg.data["node_id"]
             endpoint_id = msg.data["endpoint_id"]
             self.logger.debug("Endpoint added: %s/%s", node_id, endpoint_id)
+        if msg.event == EventType.NODE_EVENT:
+            if self.logger.isEnabledFor(logging.DEBUG):
+                self.logger.debug(
+                    "Node event: %s",
+                    msg.data,
+                )
+            node_event = dataclass_from_dict(MatterNodeEvent, msg.data)
+            self._signal_event(
+                EventType.NODE_EVENT,
+                data=node_event,
+                node_id=node_event.node_id,
+            )
+            return
         # simply forward all other events as-is
         if self.logger.isEnabledFor(logging.DEBUG):
             self.logger.debug("Received event: %s", msg)
         self._signal_event(msg.event, msg.data)
 
     def _signal_event(
         self,
```

### Comparing `python-matter-server-3.6.4/matter_server/client/connection.py` & `python-matter-server-3.7.0/matter_server/client/connection.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.4/matter_server/client/exceptions.py` & `python-matter-server-3.7.0/matter_server/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.4/matter_server/client/models/device_types.py` & `python-matter-server-3.7.0/matter_server/client/models/device_types.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.4/matter_server/client/models/node.py` & `python-matter-server-3.7.0/matter_server/client/models/node.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.4/matter_server/common/errors.py` & `python-matter-server-3.7.0/matter_server/common/errors.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.4/matter_server/common/helpers/api.py` & `python-matter-server-3.7.0/matter_server/common/helpers/api.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.4/matter_server/common/helpers/json.py` & `python-matter-server-3.7.0/matter_server/common/helpers/json.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.4/matter_server/common/helpers/util.py` & `python-matter-server-3.7.0/matter_server/common/helpers/util.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.4/matter_server/common/models.py` & `python-matter-server-3.7.0/matter_server/common/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,14 +79,29 @@
     # where each value can also be a '*' for wildcard
     attribute_subscriptions: set[tuple[int | str, int | str, int | str]] = field(
         default_factory=set
     )
 
 
 @dataclass
+class MatterNodeEvent:
+    """Representation of a NodeEvent for a Matter node."""
+
+    node_id: int
+    endpoint_id: int
+    cluster_id: int
+    event_id: int
+    event_number: int
+    priority: int
+    timestamp: int
+    timestamp_type: int
+    data: dict[str, Any] | None
+
+
+@dataclass
 class ServerDiagnostics:
     """Full dump of the server information and data."""
 
     info: ServerInfoMessage
     nodes: list[MatterNodeData]
     events: list[dict]
```

### Comparing `python-matter-server-3.6.4/matter_server/server/__main__.py` & `python-matter-server-3.7.0/matter_server/server/__main__.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.4/matter_server/server/client_handler.py` & `python-matter-server-3.7.0/matter_server/server/client_handler.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.4/matter_server/server/const.py` & `python-matter-server-3.7.0/matter_server/server/const.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.4/matter_server/server/device_controller.py` & `python-matter-server-3.7.0/matter_server/server/device_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,30 +31,29 @@
 from ..common.helpers.json import json_dumps
 from ..common.helpers.util import (
     create_attribute_path,
     create_attribute_path_from_attribute,
     dataclass_from_dict,
     parse_attribute_path,
 )
-from ..common.models import APICommand, EventType, MatterNodeData
+from ..common.models import APICommand, EventType, MatterNodeData, MatterNodeEvent
 from .const import PAA_ROOT_CERTS_DIR
 from .helpers.paa_certificates import fetch_certificates
 
 if TYPE_CHECKING:
     from chip.ChipDeviceCtrl import ChipDeviceController
 
     from .server import MatterServer
 
 _T = TypeVar("_T")
 
 DATA_KEY_NODES = "nodes"
 DATA_KEY_LAST_NODE_ID = "last_node_id"
 
 LOGGER = logging.getLogger(__name__)
-INTERVIEW_TASK_LIMIT = 5
 MAX_POLL_INTERVAL = 600
 
 # a list of attributes we should always watch on all nodes
 DEFAULT_SUBSCRIBE_ATTRIBUTES: set[tuple[int | str, int | str, int | str]] = {
     ("*", 0x001D, 0x00000000),  # all endpoints, descriptor cluster, deviceTypeList
     ("*", 0x001D, 0x00000003),  # all endpoints, descriptor cluster, partsList
     (0, 0x0028, "*"),  # endpoint 0, BasicInformation cluster, all attributes
@@ -73,22 +72,20 @@
     ):
         """Initialize the device controller."""
         self.server = server
         # we keep the last events in memory so we can include them in the diagnostics dump
         self.event_history: Deque[Attribute.EventReadResult] = deque(maxlen=25)
         self._subscriptions: dict[int, Attribute.SubscriptionTransaction] = {}
         self._attr_subscriptions: dict[int, list[tuple[Any, ...]] | str] = {}
-        self._resub_timer: dict[int, asyncio.TimerHandle] = {}
+        self._resub_debounce_timer: dict[int, asyncio.TimerHandle] = {}
+        self._sub_retry_timer: dict[int, asyncio.TimerHandle] = {}
         self._nodes: dict[int, MatterNodeData | None] = {}
         self.wifi_credentials_set: bool = False
         self.thread_credentials_set: bool = False
         self.compressed_fabric_id: int | None = None
-        self._interview_limit: asyncio.Semaphore = asyncio.Semaphore(
-            INTERVIEW_TASK_LIMIT
-        )
         self._resolve_lock: asyncio.Lock = asyncio.Lock()
         self._node_lock: dict[int, asyncio.Lock] = {}
 
     async def initialize(self) -> None:
         """Async initialize of controller."""
         # (re)fetch all PAA certificates once at startup
         # NOTE: this must be done before initializing the controller
@@ -301,24 +298,22 @@
         """Interview a node."""
         if self.chip_controller is None:
             raise RuntimeError("Device Controller not initialized.")
 
         LOGGER.debug("Interviewing node: %s", node_id)
         try:
             await self._resolve_node(node_id=node_id)
-            async with self._interview_limit:
-                async with self._get_node_lock(node_id):
-                    read_response: Attribute.AsyncReadTransaction.ReadResponse = (
-                        await self.chip_controller.Read(
-                            nodeid=node_id,
-                            attributes="*",
-                            events="*",
-                            fabricFiltered=False,
-                        )
+            async with self._get_node_lock(node_id):
+                read_response: Attribute.AsyncReadTransaction.ReadResponse = (
+                    await self.chip_controller.Read(
+                        nodeid=node_id,
+                        attributes="*",
+                        fabricFiltered=False,
                     )
+                )
         except (ChipStackError, NodeNotResolving) as err:
             raise NodeInterviewFailed(f"Failed to interview node {node_id}") from err
 
         is_new_node = node_id not in self._nodes
         existing_info = self._nodes.get(node_id)
         node = MatterNodeData(
             node_id=node_id,
@@ -405,15 +400,15 @@
                 await self.chip_controller.Read(
                     nodeid=node_id,
                     attributes=[(endpoint_id, attribute)],
                     fabricFiltered=False,
                 )
             )
             read_atributes = self._parse_attributes_from_read_result(result.attributes)
-            return read_atributes[attribute_path]
+            return read_atributes.get(attribute_path, None)
 
     @api_command(APICommand.WRITE_ATTRIBUTE)
     async def write_attribute(
         self,
         node_id: int,
         attribute_path: str,
         value: Any,
@@ -436,14 +431,17 @@
             raise RuntimeError("Device Controller not initialized.")
 
         if node_id not in self._nodes:
             raise NodeNotExists(
                 f"Node {node_id} does not exist or has not been interviewed."
             )
 
+        # pop any existing interview/subscription reschedule timer
+        self._sub_retry_timer.pop(node_id, None)
+
         node = self._nodes.pop(node_id)
         self.server.storage.remove(
             DATA_KEY_NODES,
             subkey=str(node_id),
         )
 
         assert node is not None
@@ -501,21 +499,23 @@
             value=node,
         )
 
         # (re)setup node subscription
         # this could potentially be called multiple times within a short timeframe
         # so debounce it a bit
         def resubscribe() -> None:
-            self._resub_timer.pop(node_id, None)
+            self._resub_debounce_timer.pop(node_id, None)
             asyncio.create_task(self._subscribe_node(node_id))
 
-        if existing_timer := self._resub_timer.pop(node_id, None):
+        if existing_timer := self._resub_debounce_timer.pop(node_id, None):
             existing_timer.cancel()
         assert self.server.loop is not None
-        self._resub_timer[node_id] = self.server.loop.call_later(5, resubscribe)
+        self._resub_debounce_timer[node_id] = self.server.loop.call_later(
+            5, resubscribe
+        )
 
     async def _subscribe_node(self, node_id: int) -> None:
         """
         Subscribe to all node state changes/events for an individual node.
 
         Note that by using the listen command at server level,
         you will receive all (subscribed) node events and attribute updates.
@@ -589,16 +589,17 @@
         async with node_lock:
             node_logger.debug("Setting up attributes and events subscription.")
             sub: Attribute.SubscriptionTransaction = await self.chip_controller.Read(
                 nodeid=node_id,
                 # In order to prevent network congestion due to wildcard subscriptions on all nodes,
                 # we keep a list of attributes we are explicitly interested in.
                 attributes=attr_subscriptions,
-                # simply subscribe to all (urgent and non urgent) device events
-                events=[("*", 1), ("*", 0)],
+                # simply subscribe to urgent device events only (e.g. button press etc.)
+                # non urgent events are disagnostic reports etc. for which we have no usecase (yet).
+                events=[("*", 1)],
                 # Use a report interval of 0, 300 which means we want to receive state changes
                 # as soon as possible (the 0 as floor) but we want to receive a report
                 # at least once every 5 minutes (300 as ceiling).
                 # This is also used to detect the node is still alive.
                 # A resubscription will be initiated automatically by the sdk
                 # if there was no report within the interval.
                 reportInterval=(0, 300),
@@ -669,17 +670,28 @@
             transaction: Attribute.SubscriptionTransaction,
         ) -> None:
             # pylint: disable=unused-argument
             assert self.server.loop is not None
             node_logger.debug(
                 "Received node event: %s - transaction: %s", data, transaction
             )
-            self.event_history.append(data)
+            node_event = MatterNodeEvent(
+                node_id=node_id,
+                endpoint_id=data.Header.EndpointId,
+                cluster_id=data.Header.ClusterId,
+                event_id=data.Header.EventId,
+                event_number=data.Header.EventNumber,
+                priority=data.Header.Priority,
+                timestamp=data.Header.Timestamp,
+                timestamp_type=data.Header.TimestampType,
+                data=data.Data,
+            )
+            self.event_history.append(node_event)
             self.server.loop.call_soon_threadsafe(
-                self.server.signal_event, EventType.NODE_EVENT, data
+                self.server.signal_event, EventType.NODE_EVENT, node_event
             )
 
         def error_callback(
             chipError: int, transaction: Attribute.SubscriptionTransaction
         ) -> None:
             # pylint: disable=unused-argument, invalid-name
             node_logger.error("Got error from node: %s", chipError)
@@ -758,18 +770,24 @@
         )
 
     async def _check_interview_and_subscription(
         self, node_id: int, reschedule_interval: int = 30
     ) -> None:
         """Handle interview (if needed) and subscription for known node."""
 
+        if node_id not in self._nodes:
+            raise NodeNotExists(f"Node {node_id} does not exist.")
+
+        # pop any existing reschedule timer
+        self._sub_retry_timer.pop(node_id, None)
+
         def reschedule() -> None:
             """(Re)Schedule interview and/or initial subscription for a node."""
             assert self.server.loop is not None
-            self.server.loop.call_later(
+            self._sub_retry_timer[node_id] = self.server.loop.call_later(
                 reschedule_interval,
                 asyncio.create_task,
                 self._check_interview_and_subscription(
                     node_id,
                     # increase interval at each attempt with maximum of
                     # MAX_POLL_INTERVAL seconds (= 10 minutes)
                     min(reschedule_interval + 10, MAX_POLL_INTERVAL),
@@ -852,18 +870,24 @@
                         )
                         continue
                     result[attribute_path] = attr_value
         return result
 
     async def _resolve_node(self, node_id: int, retries: int = 3) -> None:
         """Resolve a Node on the network."""
+        if (node := self._nodes.get(node_id)) and node.available:
+            # no need to resolve, the node is already available/connected
+            return
+
         node_lock = self._get_node_lock(node_id)
         if self.chip_controller is None:
             raise RuntimeError("Device Controller not initialized.")
         try:
+            # the sdk crashes when multiple resolves happen at the same time
+            # guard simultane resolves with a lock.
             async with node_lock, self._resolve_lock:
                 LOGGER.debug("Attempting to resolve node %s...", node_id)
                 await self._call_sdk(
                     self.chip_controller.ResolveNode,
                     nodeid=node_id,
                 )
         except (ChipStackError, TimeoutError) as err:
```

### Comparing `python-matter-server-3.6.4/matter_server/server/helpers/paa_certificates.py` & `python-matter-server-3.7.0/matter_server/server/helpers/paa_certificates.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.4/matter_server/server/server.py` & `python-matter-server-3.7.0/matter_server/server/server.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.4/matter_server/server/stack.py` & `python-matter-server-3.7.0/matter_server/server/stack.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.4/matter_server/server/storage.py` & `python-matter-server-3.7.0/matter_server/server/storage.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.4/matter_server/server/vendor_info.py` & `python-matter-server-3.7.0/matter_server/server/vendor_info.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.4/pyproject.toml` & `python-matter-server-3.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools~=62.3",
     "wheel~=0.37.1",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-matter-server"
-version = "3.6.4"
+version = "3.7.0"
 description = "Python Matter WebSocket Server"
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [
     { name = "The Home Assistant Authors", email = "hello@home-assistant.io" },
 ]
 classifiers = [
@@ -33,18 +33,18 @@
 
 [project.license]
 text = "Apache-2.0"
 
 [project.optional-dependencies]
 server = [
     "home-assistant-chip-core==2023.6.0",
-    "cryptography==41.0.1",
+    "cryptography==41.0.2",
 ]
 test = [
-    "black==23.3.0",
+    "black==23.7.0",
     "flake8==6.0.0",
     "flake8-docstrings==1.7.0",
     "isort==5.12.0",
     "mypy==1.4.1",
     "pylint==2.17.4",
     "pytest==7.4.0",
     "pytest-aiohttp==1.0.4",
```

### Comparing `python-matter-server-3.6.4/python_matter_server.egg-info/PKG-INFO` & `python-matter-server-3.7.0/python_matter_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-matter-server
-Version: 3.6.4
+Version: 3.7.0
 Summary: Python Matter WebSocket Server
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
```

### Comparing `python-matter-server-3.6.4/python_matter_server.egg-info/SOURCES.txt` & `python-matter-server-3.7.0/python_matter_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

