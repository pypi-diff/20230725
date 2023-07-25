# Comparing `tmp/Akatosh-2.1.7.tar.gz` & `tmp/Akatosh-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Akatosh-2.1.7.tar", last modified: Fri Jul 21 05:28:57 2023, max compression
+gzip compressed data, was "Akatosh-2.1.8.tar", last modified: Tue Jul 25 01:26:07 2023, max compression
```

## Comparing `Akatosh-2.1.7.tar` & `Akatosh-2.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 05:28:57.560065 Akatosh-2.1.7/
-drwxrwxrwx   0        0        0        0 2023-07-21 05:28:57.502698 Akatosh-2.1.7/Akatosh/
--rw-rw-rw-   0        0        0      242 2023-07-12 05:21:53.000000 Akatosh-2.1.7/Akatosh/__init__.py
--rw-rw-rw-   0        0        0    14879 2023-07-20 01:56:56.000000 Akatosh-2.1.7/Akatosh/entity.py
--rw-rw-rw-   0        0        0    13484 2023-07-21 05:26:19.000000 Akatosh-2.1.7/Akatosh/event.py
--rw-rw-rw-   0        0        0      384 2023-07-12 04:33:32.000000 Akatosh-2.1.7/Akatosh/logger.py
--rw-rw-rw-   0        0        0     9111 2023-07-20 06:14:59.000000 Akatosh-2.1.7/Akatosh/resource.py
--rw-rw-rw-   0        0        0      201 2023-07-12 04:33:32.000000 Akatosh-2.1.7/Akatosh/states.py
--rw-rw-rw-   0        0        0     6365 2023-07-20 01:43:52.000000 Akatosh-2.1.7/Akatosh/universe.py
-drwxrwxrwx   0        0        0        0 2023-07-21 05:28:57.547165 Akatosh-2.1.7/Akatosh.egg-info/
--rw-rw-rw-   0        0        0     2830 2023-07-21 05:28:57.000000 Akatosh-2.1.7/Akatosh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-07-21 05:28:57.000000 Akatosh-2.1.7/Akatosh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 05:28:57.000000 Akatosh-2.1.7/Akatosh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-21 05:28:57.000000 Akatosh-2.1.7/Akatosh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2830 2023-07-21 05:28:57.551339 Akatosh-2.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2238 2023-07-12 04:33:32.000000 Akatosh-2.1.7/README.md
--rw-rw-rw-   0        0        0      635 2023-07-21 05:27:30.000000 Akatosh-2.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-21 05:28:57.561031 Akatosh-2.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-25 01:26:07.656094 Akatosh-2.1.8/
+drwxrwxrwx   0        0        0        0 2023-07-25 01:26:07.574087 Akatosh-2.1.8/Akatosh/
+-rw-rw-rw-   0        0        0      242 2023-07-12 05:21:53.000000 Akatosh-2.1.8/Akatosh/__init__.py
+-rw-rw-rw-   0        0        0    14990 2023-07-25 01:00:44.000000 Akatosh-2.1.8/Akatosh/entity.py
+-rw-rw-rw-   0        0        0    14704 2023-07-25 01:21:42.000000 Akatosh-2.1.8/Akatosh/event.py
+-rw-rw-rw-   0        0        0      384 2023-07-12 04:33:32.000000 Akatosh-2.1.8/Akatosh/logger.py
+-rw-rw-rw-   0        0        0     9111 2023-07-20 06:14:59.000000 Akatosh-2.1.8/Akatosh/resource.py
+-rw-rw-rw-   0        0        0      201 2023-07-12 04:33:32.000000 Akatosh-2.1.8/Akatosh/states.py
+-rw-rw-rw-   0        0        0     6365 2023-07-20 01:43:52.000000 Akatosh-2.1.8/Akatosh/universe.py
+drwxrwxrwx   0        0        0        0 2023-07-25 01:26:07.633136 Akatosh-2.1.8/Akatosh.egg-info/
+-rw-rw-rw-   0        0        0     2830 2023-07-25 01:26:07.000000 Akatosh-2.1.8/Akatosh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-07-25 01:26:07.000000 Akatosh-2.1.8/Akatosh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 01:26:07.000000 Akatosh-2.1.8/Akatosh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-25 01:26:07.000000 Akatosh-2.1.8/Akatosh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2830 2023-07-25 01:26:07.647087 Akatosh-2.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2238 2023-07-12 04:33:32.000000 Akatosh-2.1.8/README.md
+-rw-rw-rw-   0        0        0      635 2023-07-25 01:24:17.000000 Akatosh-2.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-25 01:26:07.656094 Akatosh-2.1.8/setup.cfg
```

### Comparing `Akatosh-2.1.7/Akatosh/entity.py` & `Akatosh-2.1.8/Akatosh/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,16 @@
 
     def create(self, at: int | float) -> None:
         """The creation of the entity."""
 
         def _create():
             if self.terminated:
                 raise RuntimeError(f"Entity {self.label} is already terminated.")
+            if self.created:
+                return
             self._state.append(State.CREATED)
             self._created_at = Mundus.now
             self.on_creation()
             logger.debug(f"Entity {self.label} created at {Mundus.now}")
 
         if self.precursor is None:
             self._creation = InstantEvent(
@@ -92,14 +94,16 @@
 
     def terminate(self, at: int | float) -> None:
         """The termination of the entity. This will release all occupied resource, remove the entity from all entity lists, and cancel all unfinished events."""
 
         def _terminate():
             if not self.created:
                 raise RuntimeError(f"Entity {self.label} is not created yet.")
+            if self.terminated:
+                return
             self._state.append(State.TERMINATED)
             self._terminated_at = Mundus.now
             self.release_resources()
             self.unregister_from_lists()
             self.cancel_unfinished_events()
             self.on_termination()
             logger.debug(f"Entity {self.label} terminated at {Mundus.now}")
```

### Comparing `Akatosh-2.1.7/Akatosh/event.py` & `Akatosh-2.1.8/Akatosh/event.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import inspect
 from abc import abstractmethod
 from typing import Any, Callable, List
 from uuid import uuid4
+import warnings
 
 from .logger import logger
 from .states import State
 from .universe import Mundus
 
 
 class Event:
@@ -54,78 +55,113 @@
         if callable(priority):
             self._priority = priority()
         else:
             self._priority = priority
         # assign label
         self._label = label
         # add to the universe
-        if Mundus.now<self.at:
+        if Mundus.now < self.at:
             Mundus.future_events.append(self)
-        elif Mundus.now>self.at:
+        elif Mundus.now > self.at:
             raise RuntimeError(f"Event {self.label} tries to later the past.")
         else:
             Mundus.current_events.append(self)
 
     def end(self):
         """End the event and activate the follower events if there is any."""
+        if self.ended:
+            return
+
         self.state = State.ENDED
         if self in Mundus.future_events:
             Mundus.future_events.remove(self)
         if self in Mundus.current_events:
             Mundus.current_events.remove(self)
         Mundus.past_events.append(self)
         for event in self.follower:
             try:
                 event.activate()
             except RuntimeError:
                 logger.debug(f"Event {event.label} passed due time.")
         logger.debug(f"Event {self.label} is ended.")
 
     def activate(self, force: bool = False):
+        """Activate the event."""
+        
+        # raise error if the event has already ended
         if self.ended:
             raise RuntimeError(f"Event {self.label} has already ended.")
 
+        # raise warning if the event is cancelled
+        if self.cancelled:
+            warnings.warn(f"Event {self.label} is cancelled.")
+            return
+        
+        # return if the event is already active
+        if self.active:
+            return
+
         if force:
             self.state = State.ACTIVE
+            self._at = Mundus.now
             logger.debug(f"Event {self.label} is set to active.")
         else:
             if all(e.state == State.ENDED for e in self.precursor):
                 self.state = State.ACTIVE
+                self._at = Mundus.now
                 logger.debug(f"Event {self.label} is set to active.")
             else:
-                raise RuntimeError(
-                    f"Event {self.label} is waiting for other events to end."
-                )
+                warnings.warn(f"Event {self.label} is waiting for other events to end.")
+                return
 
     def deactivate(self):
         """Deactivate the event.
 
         Raises:
             RuntimeError: raise if the event has already ended.
         """
+        
+        # raise error if the event has already ended
         if self.ended:
             raise RuntimeError(f"Event {self.label} has already ended.")
+        
+        # raise warning if the event is cancelled
+        if self.cancelled:
+            warnings.warn(f"Event {self.label} is cancelled.")
+            return
+
+        # return if the event is already inactive
+        if self.inactive:
+            return
+
         self.state = State.INACTIVE
 
     def cancel(self):
         """Cancel the event. Will not set the follower events to active.
 
         Raises:
             RuntimeError: raise if the event has already ended.
         """
+        
+        # raise error if the event has already ended
         if self.ended:
             raise RuntimeError(f"Event {self.label} has already ended.")
+
+        # return if the event is already cancelled
+        if self.cancelled:
+            return
+
         self.state = State.CANCELED
         if self in Mundus.future_events:
             Mundus.future_events.remove(self)
         if self in Mundus.current_events:
             Mundus.current_events.remove(self)
         Mundus.past_events.append(self)
         logger.debug(f"Event {self.label} is cancelled.")
-        
+
     @abstractmethod
     async def _perform(self):
         """Abstract method for the event to perform its action."""
         pass
 
     def __eq__(self, _o: Event) -> bool:
         """Determine if two events are the same."""
@@ -312,14 +348,21 @@
                 self._at = round(self.interval + Mundus.now, Mundus.resolution)
             if self.at <= self.till:
                 logger.debug(f"Event {self.label} next step is at {self.at}.")
                 Mundus.future_events.append(self)
                 Mundus.current_events.remove(self)
             else:
                 self.end()
+                
+    def activate(self, force: bool = False):
+        
+        if Mundus.now > self.till:
+            warnings.warn(f"Event {self.label} has passed due time.")
+        else:
+            super().activate(force)
 
     @property
     def interval(self) -> int | float | Callable[..., Any]:
         """Return the interval between each action repeat."""
         return self._interval
 
     @property
```

### Comparing `Akatosh-2.1.7/Akatosh/resource.py` & `Akatosh-2.1.8/Akatosh/resource.py`

 * *Files identical despite different names*

### Comparing `Akatosh-2.1.7/Akatosh/universe.py` & `Akatosh-2.1.8/Akatosh/universe.py`

 * *Files identical despite different names*

### Comparing `Akatosh-2.1.7/Akatosh.egg-info/PKG-INFO` & `Akatosh-2.1.8/Akatosh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 2.1.7
+Version: 2.1.8
 Summary: A simple implement for discrete events simulation.
 Author-email: Yifei Ren <ryf0510@live.com>
 Project-URL: Homepage, https://github.com/ulfaric/Akatosh
 Project-URL: Documentation, https://ulfaric.github.io/Akatosh
 Project-URL: Bug Tracker, https://github.com/ulfaric/Akatosh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Akatosh-2.1.7/PKG-INFO` & `Akatosh-2.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 2.1.7
+Version: 2.1.8
 Summary: A simple implement for discrete events simulation.
 Author-email: Yifei Ren <ryf0510@live.com>
 Project-URL: Homepage, https://github.com/ulfaric/Akatosh
 Project-URL: Documentation, https://ulfaric.github.io/Akatosh
 Project-URL: Bug Tracker, https://github.com/ulfaric/Akatosh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Akatosh-2.1.7/README.md` & `Akatosh-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `Akatosh-2.1.7/pyproject.toml` & `Akatosh-2.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Akatosh"
-version = "2.1.7"
+version = "2.1.8"
 authors = [{ name = "Yifei Ren", email = "ryf0510@live.com" }]
 description = "A simple implement for discrete events simulation."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

