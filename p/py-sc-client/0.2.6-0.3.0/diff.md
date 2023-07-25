# Comparing `tmp/py-sc-client-0.2.6.tar.gz` & `tmp/py-sc-client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-sc-client-0.2.6.tar", last modified: Mon Mar 27 14:40:15 2023, max compression
+gzip compressed data, was "py-sc-client-0.3.0.tar", last modified: Tue Jul 25 08:07:36 2023, max compression
```

## Comparing `py-sc-client-0.2.6.tar` & `py-sc-client-0.3.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:40:15.469774 py-sc-client-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-27 14:40:04.000000 py-sc-client-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23161 2023-03-27 14:40:15.469774 py-sc-client-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22314 2023-03-27 14:40:04.000000 py-sc-client-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-27 14:40:15.469774 py-sc-client-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-03-27 14:40:04.000000 py-sc-client-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:40:15.461774 py-sc-client-0.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:40:15.465774 py-sc-client-0.2.6/src/py_sc_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23161 2023-03-27 14:40:15.000000 py-sc-client-0.2.6/src/py_sc_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-03-27 14:40:15.000000 py-sc-client-0.2.6/src/py_sc_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 14:40:15.000000 py-sc-client-0.2.6/src/py_sc_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-27 14:40:15.000000 py-sc-client-0.2.6/src/py_sc_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-27 14:40:15.000000 py-sc-client-0.2.6/src/py_sc_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:40:15.465774 py-sc-client-0.2.6/src/sc_client/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-27 14:40:04.000000 py-sc-client-0.2.6/src/sc_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-03-27 14:40:04.000000 py-sc-client-0.2.6/src/sc_client/_internal_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:40:15.465774 py-sc-client-0.2.6/src/sc_client/client/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-27 14:40:04.000000 py-sc-client-0.2.6/src/sc_client/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-03-27 14:40:04.000000 py-sc-client-0.2.6/src/sc_client/client/_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-03-27 14:40:04.000000 py-sc-client-0.2.6/src/sc_client/client/_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-03-27 14:40:04.000000 py-sc-client-0.2.6/src/sc_client/client/_payload_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-03-27 14:40:04.000000 py-sc-client-0.2.6/src/sc_client/client/_response_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:40:15.465774 py-sc-client-0.2.6/src/sc_client/constants/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-27 14:40:04.000000 py-sc-client-0.2.6/src/sc_client/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-03-27 14:40:04.000000 py-sc-client-0.2.6/src/sc_client/constants/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-03-27 14:40:04.000000 py-sc-client-0.2.6/src/sc_client/constants/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-03-27 14:40:04.000000 py-sc-client-0.2.6/src/sc_client/constants/numeric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:40:15.469774 py-sc-client-0.2.6/src/sc_client/constants/sc_types/
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-03-27 14:40:04.000000 py-sc-client-0.2.6/src/sc_client/constants/sc_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-27 14:40:04.000000 py-sc-client-0.2.6/src/sc_client/constants/sc_types/bitmasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-03-27 14:40:04.000000 py-sc-client-0.2.6/src/sc_client/constants/sc_types/sc_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:40:15.469774 py-sc-client-0.2.6/src/sc_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-03-27 14:40:04.000000 py-sc-client-0.2.6/src/sc_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-27 14:40:04.000000 py-sc-client-0.2.6/src/sc_client/models/sc_addr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-03-27 14:40:04.000000 py-sc-client-0.2.6/src/sc_client/models/sc_construction.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-27 14:40:04.000000 py-sc-client-0.2.6/src/sc_client/models/sc_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-03-27 14:40:04.000000 py-sc-client-0.2.6/src/sc_client/models/sc_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-27 14:40:04.000000 py-sc-client-0.2.6/src/sc_client/models/scs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-03-27 14:40:04.000000 py-sc-client-0.2.6/src/sc_client/sc_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-03-27 14:40:04.000000 py-sc-client-0.2.6/src/sc_client/sc_keynodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-03-27 14:40:04.000000 py-sc-client-0.2.6/src/sc_client/sc_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-03-27 14:40:04.000000 py-sc-client-0.2.6/src/sc_client/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:07:36.793294 py-sc-client-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-25 08:07:20.000000 py-sc-client-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24714 2023-07-25 08:07:36.793294 py-sc-client-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23867 2023-07-25 08:07:20.000000 py-sc-client-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-25 08:07:36.793294 py-sc-client-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-25 08:07:20.000000 py-sc-client-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:07:36.781294 py-sc-client-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:07:36.785294 py-sc-client-0.3.0/src/py_sc_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24714 2023-07-25 08:07:36.000000 py-sc-client-0.3.0/src/py_sc_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-25 08:07:36.000000 py-sc-client-0.3.0/src/py_sc_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 08:07:36.000000 py-sc-client-0.3.0/src/py_sc_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-25 08:07:36.000000 py-sc-client-0.3.0/src/py_sc_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 08:07:36.000000 py-sc-client-0.3.0/src/py_sc_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:07:36.789294 py-sc-client-0.3.0/src/sc_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-25 08:07:20.000000 py-sc-client-0.3.0/src/sc_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-25 08:07:20.000000 py-sc-client-0.3.0/src/sc_client/_internal_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:07:36.789294 py-sc-client-0.3.0/src/sc_client/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-25 08:07:20.000000 py-sc-client-0.3.0/src/sc_client/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-07-25 08:07:20.000000 py-sc-client-0.3.0/src/sc_client/client/_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-25 08:07:20.000000 py-sc-client-0.3.0/src/sc_client/client/_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-07-25 08:07:20.000000 py-sc-client-0.3.0/src/sc_client/client/_payload_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-07-25 08:07:20.000000 py-sc-client-0.3.0/src/sc_client/client/_response_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:07:36.789294 py-sc-client-0.3.0/src/sc_client/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-25 08:07:20.000000 py-sc-client-0.3.0/src/sc_client/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-25 08:07:20.000000 py-sc-client-0.3.0/src/sc_client/constants/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-25 08:07:20.000000 py-sc-client-0.3.0/src/sc_client/constants/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-25 08:07:20.000000 py-sc-client-0.3.0/src/sc_client/constants/numeric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:07:36.789294 py-sc-client-0.3.0/src/sc_client/constants/sc_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-07-25 08:07:20.000000 py-sc-client-0.3.0/src/sc_client/constants/sc_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-25 08:07:20.000000 py-sc-client-0.3.0/src/sc_client/constants/sc_types/bitmasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-25 08:07:20.000000 py-sc-client-0.3.0/src/sc_client/constants/sc_types/sc_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:07:36.793294 py-sc-client-0.3.0/src/sc_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-25 08:07:20.000000 py-sc-client-0.3.0/src/sc_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-25 08:07:20.000000 py-sc-client-0.3.0/src/sc_client/models/sc_addr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-25 08:07:20.000000 py-sc-client-0.3.0/src/sc_client/models/sc_construction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-25 08:07:20.000000 py-sc-client-0.3.0/src/sc_client/models/sc_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-07-25 08:07:20.000000 py-sc-client-0.3.0/src/sc_client/models/sc_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-25 08:07:20.000000 py-sc-client-0.3.0/src/sc_client/models/scs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-25 08:07:20.000000 py-sc-client-0.3.0/src/sc_client/sc_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-25 08:07:20.000000 py-sc-client-0.3.0/src/sc_client/sc_keynodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-25 08:07:20.000000 py-sc-client-0.3.0/src/sc_client/sc_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-07-25 08:07:20.000000 py-sc-client-0.3.0/src/sc_client/session.py
```

### Comparing `py-sc-client-0.2.6/LICENSE` & `py-sc-client-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-sc-client-0.2.6/PKG-INFO` & `py-sc-client-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-sc-client
-Version: 0.2.6
+Version: 0.3.0
 Summary: The Python implementation of the client for communication with the sc-server
 Home-page: https://github.com/ostis-ai/py-sc-client
 Author: ostis-ai
 License: MIT
 Project-URL: Bug Reports, https://github.com/ostis-ai/py-sc-client/issues
 Project-URL: Source, https://github.com/ostis-ai/py-sc-client
 Keywords: sc-client,sc client
@@ -88,14 +88,59 @@
 ```python
 from sc_client.client import is_connected
 
 if is_connected():
     ...
 ```
 
+- *sc_client.client*.**set_error_handler**(callback)
+
+Sets a handler callback to manage client and server errors. Callback must take one argument - an exception object.
+
+```python
+from sc_client.client import set_error_handler
+
+def on_error(e):
+    if isinstance(e, AttributeError):
+        print(e)
+
+set_error_handler(on_error)        
+...
+```
+
+- *sc_client.client*.**set_reconnect_handler**(**reconnect_kwargs)
+
+Sets handler callback to reconnect on sc-server connection failure. Method takes the following arguments:
+ 
+- `_reconnect_handler_` - handler callback function. Default value: `_session.default_reconnect_handler_`.
+- `_post_reconnect_callback_` - handler callback invoked after `_reconnect_handler_` has finished successfully.
+- `_reconnect_retries_` - amount of call tries of `_reconnect_handler_`. Default value: `5`.
+- `_reconnect_retry_delay_` - period between call tries of `_reconnect_handler_` (in seconds). Default value: `2`.
+
+If the sc-server did not respond to one of the resent messages, after a requested `_reconnect_retry_delay_`
+the `_reconnect_handler_` is called, and the same message is sent again. This procedure is repeated for
+`_reconnect_retries_` times, until the message is sent and a response is received.
+
+```python
+from sc_client.client import set_reconnect_handler
+
+url = "ws://localhost:8090/ws_json"
+
+def on_reconnect():
+    connect(url)
+
+set_reconnect_handler(
+    reconnect_handler=connect,
+    post_reconnect_handler=None,
+    reconnect_retries=5,
+    reconnect_retry_delay=1.0 #seconds
+)        
+...
+```
+
 ## Base classes
 
 ### ScAddr
 
 Minimum element of sc is ScAddr.
 It contains address of some element in sc-memory.
 Knowing it, you can find related elements, connect edges, check the type, and so on:
```

### Comparing `py-sc-client-0.2.6/README.md` & `py-sc-client-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -67,14 +67,59 @@
 ```python
 from sc_client.client import is_connected
 
 if is_connected():
     ...
 ```
 
+- *sc_client.client*.**set_error_handler**(callback)
+
+Sets a handler callback to manage client and server errors. Callback must take one argument - an exception object.
+
+```python
+from sc_client.client import set_error_handler
+
+def on_error(e):
+    if isinstance(e, AttributeError):
+        print(e)
+
+set_error_handler(on_error)        
+...
+```
+
+- *sc_client.client*.**set_reconnect_handler**(**reconnect_kwargs)
+
+Sets handler callback to reconnect on sc-server connection failure. Method takes the following arguments:
+ 
+- `_reconnect_handler_` - handler callback function. Default value: `_session.default_reconnect_handler_`.
+- `_post_reconnect_callback_` - handler callback invoked after `_reconnect_handler_` has finished successfully.
+- `_reconnect_retries_` - amount of call tries of `_reconnect_handler_`. Default value: `5`.
+- `_reconnect_retry_delay_` - period between call tries of `_reconnect_handler_` (in seconds). Default value: `2`.
+
+If the sc-server did not respond to one of the resent messages, after a requested `_reconnect_retry_delay_`
+the `_reconnect_handler_` is called, and the same message is sent again. This procedure is repeated for
+`_reconnect_retries_` times, until the message is sent and a response is received.
+
+```python
+from sc_client.client import set_reconnect_handler
+
+url = "ws://localhost:8090/ws_json"
+
+def on_reconnect():
+    connect(url)
+
+set_reconnect_handler(
+    reconnect_handler=connect,
+    post_reconnect_handler=None,
+    reconnect_retries=5,
+    reconnect_retry_delay=1.0 #seconds
+)        
+...
+```
+
 ## Base classes
 
 ### ScAddr
 
 Minimum element of sc is ScAddr.
 It contains address of some element in sc-memory.
 Knowing it, you can find related elements, connect edges, check the type, and so on:
```

### Comparing `py-sc-client-0.2.6/setup.py` & `py-sc-client-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 DIRECTORY_PATH = Path(__file__).parent
 README = (DIRECTORY_PATH / "README.md").read_text()
 
-VERSION = "0.2.6"
+VERSION = "0.3.0"
 INSTALL_REQUIRES = ["websocket-client>=1.0.1"]
 CURRENT_PYTHON = sys.version_info[:2]
 REQUIRED_PYTHON = (3, 8)
 
 
 if CURRENT_PYTHON < REQUIRED_PYTHON:
     sys.stderr.write(
```

### Comparing `py-sc-client-0.2.6/src/py_sc_client.egg-info/PKG-INFO` & `py-sc-client-0.3.0/src/py_sc_client.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-sc-client
-Version: 0.2.6
+Version: 0.3.0
 Summary: The Python implementation of the client for communication with the sc-server
 Home-page: https://github.com/ostis-ai/py-sc-client
 Author: ostis-ai
 License: MIT
 Project-URL: Bug Reports, https://github.com/ostis-ai/py-sc-client/issues
 Project-URL: Source, https://github.com/ostis-ai/py-sc-client
 Keywords: sc-client,sc client
@@ -88,14 +88,59 @@
 ```python
 from sc_client.client import is_connected
 
 if is_connected():
     ...
 ```
 
+- *sc_client.client*.**set_error_handler**(callback)
+
+Sets a handler callback to manage client and server errors. Callback must take one argument - an exception object.
+
+```python
+from sc_client.client import set_error_handler
+
+def on_error(e):
+    if isinstance(e, AttributeError):
+        print(e)
+
+set_error_handler(on_error)        
+...
+```
+
+- *sc_client.client*.**set_reconnect_handler**(**reconnect_kwargs)
+
+Sets handler callback to reconnect on sc-server connection failure. Method takes the following arguments:
+ 
+- `_reconnect_handler_` - handler callback function. Default value: `_session.default_reconnect_handler_`.
+- `_post_reconnect_callback_` - handler callback invoked after `_reconnect_handler_` has finished successfully.
+- `_reconnect_retries_` - amount of call tries of `_reconnect_handler_`. Default value: `5`.
+- `_reconnect_retry_delay_` - period between call tries of `_reconnect_handler_` (in seconds). Default value: `2`.
+
+If the sc-server did not respond to one of the resent messages, after a requested `_reconnect_retry_delay_`
+the `_reconnect_handler_` is called, and the same message is sent again. This procedure is repeated for
+`_reconnect_retries_` times, until the message is sent and a response is received.
+
+```python
+from sc_client.client import set_reconnect_handler
+
+url = "ws://localhost:8090/ws_json"
+
+def on_reconnect():
+    connect(url)
+
+set_reconnect_handler(
+    reconnect_handler=connect,
+    post_reconnect_handler=None,
+    reconnect_retries=5,
+    reconnect_retry_delay=1.0 #seconds
+)        
+...
+```
+
 ## Base classes
 
 ### ScAddr
 
 Minimum element of sc is ScAddr.
 It contains address of some element in sc-memory.
 Knowing it, you can find related elements, connect edges, check the type, and so on:
```

### Comparing `py-sc-client-0.2.6/src/py_sc_client.egg-info/SOURCES.txt` & `py-sc-client-0.3.0/src/py_sc_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-sc-client-0.2.6/src/sc_client/_internal_utils.py` & `py-sc-client-0.3.0/src/sc_client/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `py-sc-client-0.2.6/src/sc_client/client/__init__.py` & `py-sc-client-0.3.0/src/sc_client/client/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,11 +16,13 @@
     get_link_content,
     get_links_by_content,
     get_links_by_content_substring,
     get_links_contents_by_content_substring,
     is_connected,
     is_event_valid,
     resolve_keynodes,
+    set_error_handler,
     set_link_contents,
+    set_reconnect_handler,
     template_generate,
     template_search,
 )
```

### Comparing `py-sc-client-0.2.6/src/sc_client/client/_api.py` & `py-sc-client-0.3.0/src/sc_client/client/_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 (See an accompanying file LICENSE or a copy at http://opensource.org/licenses/MIT)
 """
 
 from __future__ import annotations
 
 from sc_client import session
 from sc_client.constants import common, exceptions
-from sc_client.constants.numeric import SERVER_RECONNECTION_TIME
+from sc_client.constants.numeric import SERVER_RECONNECT_RETRIES, SERVER_RECONNECT_RETRY_DELAY
 from sc_client.constants.sc_types import ScType
 from sc_client.models import (
     ScAddr,
     ScConstruction,
     ScEvent,
     ScEventParams,
     ScIdtfResolveParams,
@@ -22,27 +22,39 @@
     ScTemplateIdtf,
     ScTemplateParams,
     ScTemplateResult,
 )
 from sc_client.models.sc_construction import ScLinkContentData
 
 
-def connect(url: str, do_reconnect=False, reconnection_time=SERVER_RECONNECTION_TIME) -> None:
-    session.set_connection(url, do_reconnect, reconnection_time)
+def connect(url: str) -> None:
+    session.set_connection(url)
 
 
 def is_connected() -> bool:
-    return session.is_connection_established()
+    return session.is_connected()
 
 
 def disconnect() -> None:
-    session.disable_reconnection()
     session.close_connection()
 
 
+def set_error_handler(callback) -> None:
+    session.set_error_handler(callback)
+
+
+def set_reconnect_handler(**reconnect_kwargs) -> None:
+    session.set_reconnect_handler(
+        reconnect_kwargs.get("reconnect_handler", session.default_reconnect_handler),
+        reconnect_kwargs.get("post_reconnect_handler"),
+        reconnect_kwargs.get("reconnect_retries", SERVER_RECONNECT_RETRIES),
+        reconnect_kwargs.get("reconnect_retry_delay", SERVER_RECONNECT_RETRY_DELAY),
+    )
+
+
 def check_elements(*addrs: ScAddr) -> list[ScType]:
     return session.execute(common.ClientCommand.CHECK_ELEMENTS, *addrs)
 
 
 def create_elements(constr: ScConstruction) -> list[ScAddr]:
     return session.execute(common.ClientCommand.CREATE_ELEMENTS, constr)
```

### Comparing `py-sc-client-0.2.6/src/sc_client/client/_executor.py` & `py-sc-client-0.3.0/src/sc_client/client/_executor.py`

 * *Files identical despite different names*

### Comparing `py-sc-client-0.2.6/src/sc_client/client/_payload_factory.py` & `py-sc-client-0.3.0/src/sc_client/client/_payload_factory.py`

 * *Files identical despite different names*

### Comparing `py-sc-client-0.2.6/src/sc_client/client/_response_processor.py` & `py-sc-client-0.3.0/src/sc_client/client/_response_processor.py`

 * *Files identical despite different names*

### Comparing `py-sc-client-0.2.6/src/sc_client/constants/common.py` & `py-sc-client-0.3.0/src/sc_client/constants/common.py`

 * *Files identical despite different names*

### Comparing `py-sc-client-0.2.6/src/sc_client/constants/exceptions.py` & `py-sc-client-0.3.0/src/sc_client/constants/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-sc-client-0.2.6/src/sc_client/constants/sc_types/__init__.py` & `py-sc-client-0.3.0/src/sc_client/constants/sc_types/__init__.py`

 * *Files identical despite different names*

### Comparing `py-sc-client-0.2.6/src/sc_client/constants/sc_types/bitmasks.py` & `py-sc-client-0.3.0/src/sc_client/constants/sc_types/bitmasks.py`

 * *Files identical despite different names*

### Comparing `py-sc-client-0.2.6/src/sc_client/constants/sc_types/sc_type.py` & `py-sc-client-0.3.0/src/sc_client/constants/sc_types/sc_type.py`

 * *Files identical despite different names*

### Comparing `py-sc-client-0.2.6/src/sc_client/models/sc_addr.py` & `py-sc-client-0.3.0/src/sc_client/models/sc_addr.py`

 * *Files identical despite different names*

### Comparing `py-sc-client-0.2.6/src/sc_client/models/sc_construction.py` & `py-sc-client-0.3.0/src/sc_client/models/sc_construction.py`

 * *Files identical despite different names*

### Comparing `py-sc-client-0.2.6/src/sc_client/models/sc_template.py` & `py-sc-client-0.3.0/src/sc_client/models/sc_template.py`

 * *Files identical despite different names*

### Comparing `py-sc-client-0.2.6/src/sc_client/sc_agent.py` & `py-sc-client-0.3.0/src/sc_client/sc_agent.py`

 * *Files identical despite different names*

### Comparing `py-sc-client-0.2.6/src/sc_client/sc_keynodes.py` & `py-sc-client-0.3.0/src/sc_client/sc_keynodes.py`

 * *Files identical despite different names*

### Comparing `py-sc-client-0.2.6/src/sc_client/sc_module.py` & `py-sc-client-0.3.0/src/sc_client/sc_module.py`

 * *Files identical despite different names*

### Comparing `py-sc-client-0.2.6/src/sc_client/session.py` & `py-sc-client-0.3.0/src/sc_client/session.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,50 +6,70 @@
 
 from __future__ import annotations
 
 import json
 import logging
 import threading
 import time
-from typing import Any
+from typing import Any, Callable
 
 import websocket
 
 from sc_client.client._executor import Executor
 from sc_client.constants import common
 from sc_client.constants.common import ClientCommand
 from sc_client.constants.exceptions import PayloadMaxSizeError
 from sc_client.constants.numeric import (
     LOGGING_MAX_SIZE,
     MAX_PAYLOAD_SIZE,
     SERVER_ANSWER_CHECK_TIME,
     SERVER_ESTABLISH_CONNECTION_TIME,
-    SERVER_RECONNECTION_TIME,
+    SERVER_RECONNECT_RETRIES,
+    SERVER_RECONNECT_RETRY_DELAY,
 )
 from sc_client.models import Response, ScAddr, ScEvent
 
 logger = logging.getLogger(__name__)
 
 
+def default_reconnect_handler() -> None:
+    establish_connection(_ScClientSession.ws_app.url)
+
+
+def default_error_handler(error: Exception) -> None:
+    raise error
+
+
 class _ScClientSession:
+    is_open = False
     lock_instance = threading.Lock()
     responses_dict = {}
     events_dict = {}
     command_id = 0
     executor = Executor()
     ws_app: websocket.WebSocketApp | None = None
-    do_reconnect = False
-    reconnecion_time = SERVER_RECONNECTION_TIME
+    error_handler: Callable[[Exception], None] = default_error_handler
+    reconnect_callback: Callable[[], None] = default_reconnect_handler
+    post_reconnect_callback: Callable[[], None] = lambda *args: None
+    reconnect_retries: int = SERVER_RECONNECT_RETRIES
+    reconnect_retry_delay: float = SERVER_RECONNECT_RETRY_DELAY
+    last_healthcheck_answer: str = None
 
     @classmethod
     def clear(cls):
+        cls.is_open = False
         cls.responses_dict = {}
         cls.events_dict = {}
         cls.command_id = 0
         cls.ws_app = None
+        cls.error_handler = default_error_handler
+        cls.reconnect_callback = default_reconnect_handler
+        cls.post_reconnect_callback = lambda *args: None
+        cls.reconnect_retries = SERVER_RECONNECT_RETRIES
+        cls.reconnect_retry_delay = SERVER_RECONNECT_RETRY_DELAY
 
 
 def _on_message(_, response: str) -> None:
     logger.debug(f"Receive: {str(response)[:LOGGING_MAX_SIZE]}")
     response = json.loads(response, object_hook=Response)
     if response.get(common.EVENT):
         threading.Thread(
@@ -62,114 +82,132 @@
 
 def _emit_callback(event_id: int, elems: list[int]) -> None:
     event = _ScClientSession.events_dict.get(event_id)
     if event:
         event.callback(*[ScAddr(addr) for addr in elems])
 
 
+def _on_open(_) -> None:
+    logger.info("New connection opened")
+    _ScClientSession.is_open = True
+
+
 def _on_error(_, error: Exception) -> None:
-    close_connection()
-    logger.error(f"{error}")
+    _ScClientSession.error_handler(error)
+
 
+def _on_close(_, _close_status_code, _close_msg) -> None:
+    logger.info("Connection closed")
+    _ScClientSession.is_open = False
 
-def _on_close(_, close_status_code, close_msg) -> None:
-    close_connection()
-    logger.info(f"{close_status_code}: {close_msg}")
 
+def set_error_handler(callback) -> None:
+    _ScClientSession.error_handler = callback
 
-def is_connection_established() -> bool:
-    return bool(_ScClientSession.ws_app)
 
+def set_reconnect_handler(
+    reconnect_callback, post_reconnect_callback, reconnect_retries: int, reconnect_retry_delay: float
+) -> None:
+    _ScClientSession.reconnect_callback = reconnect_callback
+    _ScClientSession.post_reconnect_callback = post_reconnect_callback
+    _ScClientSession.reconnect_retries = reconnect_retries
+    _ScClientSession.reconnect_retry_delay = reconnect_retry_delay
 
-def set_connection(url: str, do_reconnect, reconnection_time) -> None:
-    _ScClientSession.do_reconnect = do_reconnect
-    _ScClientSession.reconnecion_time = reconnection_time
 
-    if not is_connection_established():
-        establish_connection(url)
+def set_connection(url: str) -> None:
+    establish_connection(url)
 
-    if _ScClientSession.do_reconnect:
-        set_reconnection(url)
+
+def is_connected() -> bool:
+    return _ScClientSession.is_open
 
 
 def establish_connection(url) -> None:
     def run_in_thread():
         _ScClientSession.ws_app = websocket.WebSocketApp(
             url,
+            on_open=_on_open,
             on_message=_on_message,
             on_error=_on_error,
             on_close=_on_close,
         )
-        _ScClientSession.ws_app.run_forever()
+        logger.info(f"Sc-server socket: {_ScClientSession.ws_app.url}")
+        try:
+            _ScClientSession.ws_app.run_forever()
+        except websocket.WebSocketException as e:
+            _on_error(_ScClientSession.ws_app, e)
 
     client_thread = threading.Thread(target=run_in_thread, name="sc-client-session-thread")
     client_thread.start()
     time.sleep(SERVER_ESTABLISH_CONNECTION_TIME)
-    logger.debug("Trying to establish connection: %s", "successful" if is_connection_established() else "unsuccessful")
-
-
-def set_reconnection(url: str) -> None:
-    def run_in_thread():
-        while _ScClientSession.do_reconnect:
-            time.sleep(SERVER_ESTABLISH_CONNECTION_TIME)
-            if not is_connection_established():
-                logger.debug("No connection, trying to reconnect")
-                establish_connection(url)
-                if not is_connection_established():
-                    logger.debug("Still no connection, waiting")
-                    time.sleep(_ScClientSession.reconnecion_time)
-
-    reconnection_thread = threading.Thread(target=run_in_thread, name="reconnection-thread")
-    reconnection_thread.start()
 
-
-def disable_reconnection() -> None:
-    _ScClientSession.do_reconnect = False
+    if _ScClientSession.is_open:
+        _ScClientSession.post_reconnect_callback()
 
 
 def close_connection() -> None:
     try:
         _ScClientSession.ws_app.close()
-    except AttributeError:
-        pass
-    _ScClientSession.ws_app = None
-    logger.debug("Disconnected")
+        _ScClientSession.is_open = False
+    except AttributeError as e:
+        _on_error(_ScClientSession.ws_app, e)
 
 
 def receive_message(command_id: int) -> Response:
     response = None
-    while not response:
+    while not response and _ScClientSession.is_open:
         response = _ScClientSession.responses_dict.get(command_id)
         time.sleep(SERVER_ANSWER_CHECK_TIME)
     return response
 
 
-def _send_message(data: str) -> None:
-    _ScClientSession.ws_app.send(data)
-    logger.debug(f"Send: {data[:LOGGING_MAX_SIZE]}")
+def _send_message(data: str, retries: int, retry: int = 0) -> None:
+    try:
+        logger.debug(f"Send: {data[:LOGGING_MAX_SIZE]}")
+        _ScClientSession.ws_app.send(data)
+    except websocket.WebSocketConnectionClosedException:
+        if _ScClientSession.reconnect_callback and retry < retries:
+            logger.warning(
+                f"Connection to sc-server has failed. "
+                f"Trying to reconnect to sc-server socket in {_ScClientSession.reconnect_retry_delay} seconds"
+            )
+            if retry > 0:
+                time.sleep(_ScClientSession.reconnect_retry_delay)
+            _ScClientSession.reconnect_callback()
+            _send_message(data, retries, retry + 1)
+        else:
+            _on_error(_ScClientSession.ws_app, ConnectionAbortedError("Sc-server takes a long time to respond"))
 
 
 def send_message(request_type: common.ClientCommand, payload: Any) -> Response:
-    if not is_connection_established():
-        raise BrokenPipeError
     with _ScClientSession.lock_instance:
         _ScClientSession.command_id += 1
         command_id = _ScClientSession.command_id
     data = json.dumps(
         {
             common.ID: command_id,
             common.TYPE: request_type.value,
             common.PAYLOAD: payload,
         }
     )
+
     len_data = len(bytes(data, "utf-8"))
     if len_data > MAX_PAYLOAD_SIZE:
-        raise PayloadMaxSizeError(f"Data is too large: {len_data} > {MAX_PAYLOAD_SIZE} bytes")
-    _send_message(data)
-    response = receive_message(command_id)
+        _on_error(
+            _ScClientSession.ws_app, PayloadMaxSizeError(f"Data is too large: {len_data} > {MAX_PAYLOAD_SIZE} bytes")
+        )
+
+    def _handle_message() -> Response:
+        _send_message(data, _ScClientSession.reconnect_retries)
+        return receive_message(command_id)
+
+    response = _handle_message()
+    if not response:
+        _on_error(_ScClientSession.ws_app, ConnectionAbortedError("Sc-server takes a long time to respond"))
+
     return response
 
 
 def get_event(event_id: int) -> ScEvent | None:
     return _ScClientSession.events_dict.get(event_id)
```

