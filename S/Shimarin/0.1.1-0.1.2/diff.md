# Comparing `tmp/Shimarin-0.1.1.tar.gz` & `tmp/Shimarin-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Shimarin-0.1.1.tar", last modified: Mon Jul 24 21:33:47 2023, max compression
+gzip compressed data, was "Shimarin-0.1.2.tar", last modified: Tue Jul 25 12:48:11 2023, max compression
```

## Comparing `Shimarin-0.1.1.tar` & `Shimarin-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:33:47.585679 Shimarin-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-24 21:33:47.585679 Shimarin-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-24 21:33:36.000000 Shimarin-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:33:47.581679 Shimarin-0.1.1/Shimarin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:33:36.000000 Shimarin-0.1.1/Shimarin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:33:47.581679 Shimarin-0.1.1/Shimarin/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:33:36.000000 Shimarin-0.1.1/Shimarin/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-24 21:33:36.000000 Shimarin-0.1.1/Shimarin/client/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-07-24 21:33:36.000000 Shimarin-0.1.1/Shimarin/client/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-24 21:33:36.000000 Shimarin-0.1.1/Shimarin/client/networking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:33:47.581679 Shimarin-0.1.1/Shimarin/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:33:47.585679 Shimarin-0.1.1/Shimarin/plugins/flask_api/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-24 21:33:36.000000 Shimarin-0.1.1/Shimarin/plugins/flask_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-24 21:33:36.000000 Shimarin-0.1.1/Shimarin/plugins/flask_api/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:33:47.585679 Shimarin-0.1.1/Shimarin/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:33:36.000000 Shimarin-0.1.1/Shimarin/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-24 21:33:36.000000 Shimarin-0.1.1/Shimarin/server/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-24 21:33:36.000000 Shimarin-0.1.1/Shimarin/server/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:33:47.581679 Shimarin-0.1.1/Shimarin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-24 21:33:47.000000 Shimarin-0.1.1/Shimarin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-24 21:33:47.000000 Shimarin-0.1.1/Shimarin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 21:33:47.000000 Shimarin-0.1.1/Shimarin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 21:33:47.000000 Shimarin-0.1.1/Shimarin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-24 21:33:47.000000 Shimarin-0.1.1/Shimarin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 21:33:47.000000 Shimarin-0.1.1/Shimarin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-24 21:33:36.000000 Shimarin-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-24 21:33:47.585679 Shimarin-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:48:11.690329 Shimarin-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-25 12:48:11.690329 Shimarin-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-25 12:47:58.000000 Shimarin-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:48:11.686329 Shimarin-0.1.2/Shimarin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 12:47:58.000000 Shimarin-0.1.2/Shimarin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:48:11.690329 Shimarin-0.1.2/Shimarin/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 12:47:58.000000 Shimarin-0.1.2/Shimarin/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-25 12:47:58.000000 Shimarin-0.1.2/Shimarin/client/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-07-25 12:47:58.000000 Shimarin-0.1.2/Shimarin/client/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-25 12:47:58.000000 Shimarin-0.1.2/Shimarin/client/networking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:48:11.686329 Shimarin-0.1.2/Shimarin/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:48:11.690329 Shimarin-0.1.2/Shimarin/plugins/flask_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-25 12:47:58.000000 Shimarin-0.1.2/Shimarin/plugins/flask_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-25 12:47:58.000000 Shimarin-0.1.2/Shimarin/plugins/flask_api/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:48:11.690329 Shimarin-0.1.2/Shimarin/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 12:47:58.000000 Shimarin-0.1.2/Shimarin/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-25 12:47:58.000000 Shimarin-0.1.2/Shimarin/server/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-25 12:47:58.000000 Shimarin-0.1.2/Shimarin/server/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:48:11.690329 Shimarin-0.1.2/Shimarin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-25 12:48:11.000000 Shimarin-0.1.2/Shimarin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-25 12:48:11.000000 Shimarin-0.1.2/Shimarin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 12:48:11.000000 Shimarin-0.1.2/Shimarin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 12:48:11.000000 Shimarin-0.1.2/Shimarin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-25 12:48:11.000000 Shimarin-0.1.2/Shimarin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 12:48:11.000000 Shimarin-0.1.2/Shimarin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-25 12:47:58.000000 Shimarin-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-25 12:48:11.694329 Shimarin-0.1.2/setup.cfg
```

### Comparing `Shimarin-0.1.1/PKG-INFO` & `Shimarin-0.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shimarin
-Version: 0.1.1
+Version: 0.1.2
 Summary: asynchronous event-based communication between client and server
 Home-page: https://github.com/kamuridesu/Shimarin
 Author: Kamuri Amorim
 Author-email: myk.gata14@gmail.com
 License: MIT
 Keywords: python events client server asynchronous
 Description-Content-Type: text/markdown
```

### Comparing `Shimarin-0.1.1/Shimarin/client/events.py` & `Shimarin-0.1.2/Shimarin/client/events.py`

 * *Files identical despite different names*

### Comparing `Shimarin-0.1.1/Shimarin/client/networking.py` & `Shimarin-0.1.2/Shimarin/client/networking.py`

 * *Files identical despite different names*

### Comparing `Shimarin-0.1.1/Shimarin/plugins/flask_api/server.py` & `Shimarin-0.1.2/Shimarin/plugins/flask_api/server.py`

 * *Files identical despite different names*

### Comparing `Shimarin-0.1.1/Shimarin/server/events.py` & `Shimarin-0.1.2/Shimarin/server/events.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,14 +78,20 @@
 
 class EventEmitter:
     def __init__(self, max_age_seconds: float = 0):
         self.events: list[Event] = []
         self.handlers = CallbacksHandlers()
         self.max_age_seconds = max_age_seconds
 
+    async def get(self, event_id: str, default: Any | None = None) -> Event:
+        for event in self.events:
+            if event.identifier == event_id:
+                return event
+        return default
+
     async def clean_old_items(self):
         for event in self.events.copy():
             if event.done or ((event.age >= self.max_age_seconds) if (self.max_age_seconds > 0) else False):
                 self.events.remove(event)
         for event in self.handlers.events.copy():
             if event.done or ((event.age >= self.max_age_seconds) if (self.max_age_seconds > 0) else False):
                 self.handlers.events.remove(event)
```

### Comparing `Shimarin-0.1.1/Shimarin.egg-info/PKG-INFO` & `Shimarin-0.1.2/Shimarin.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shimarin
-Version: 0.1.1
+Version: 0.1.2
 Summary: asynchronous event-based communication between client and server
 Home-page: https://github.com/kamuridesu/Shimarin
 Author: Kamuri Amorim
 Author-email: myk.gata14@gmail.com
 License: MIT
 Keywords: python events client server asynchronous
 Description-Content-Type: text/markdown
```

### Comparing `Shimarin-0.1.1/Shimarin.egg-info/SOURCES.txt` & `Shimarin-0.1.2/Shimarin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Shimarin-0.1.1/setup.cfg` & `Shimarin-0.1.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = Shimarin
-version = 0.1.1
+version = 0.1.2
 description = asynchronous event-based communication between client and server
 author = Kamuri Amorim
 author_email = myk.gata14@gmail.com
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/kamuridesu/Shimarin
 keywords = python events client server asynchronous
```

