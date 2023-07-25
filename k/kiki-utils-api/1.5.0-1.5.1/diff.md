# Comparing `tmp/kiki_utils_api-1.5.0-py3-none-any.whl.zip` & `tmp/kiki_utils_api-1.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 10811 bytes, number of entries: 18
+Zip file size: 10607 bytes, number of entries: 18
 -rw-rw-r--  2.0 unx        0 b- defN 22-Nov-28 10:23 kikiutils_api/__init__.py
--rw-rw-r--  2.0 unx     4641 b- defN 23-Jun-21 10:31 kikiutils_api/classes/__init__.py
+-rw-rw-r--  2.0 unx     3634 b- defN 23-Jul-25 02:47 kikiutils_api/classes/__init__.py
 -rw-rw-r--  2.0 unx      796 b- defN 23-Jan-06 04:19 kikiutils_api/classes/blacksheep.py
 -rw-rw-r--  2.0 unx      701 b- defN 23-Jun-21 10:32 kikiutils_api/classes/sanic.py
 -rw-rw-r--  2.0 unx     2356 b- defN 23-Jun-21 10:32 kikiutils_api/classes/transmission.py
 -rw-rw-r--  2.0 unx     3552 b- defN 23-Jul-25 00:06 kikiutils_api/classes/websocket.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Nov-28 10:23 kikiutils_api/decorators/__init__.py
 -rw-rw-r--  2.0 unx     1563 b- defN 23-Jul-20 10:59 kikiutils_api/decorators/blacksheep.py
 -rw-rw-r--  2.0 unx     3433 b- defN 23-Jan-06 05:44 kikiutils_api/decorators/sanic.py
 -rw-rw-r--  2.0 unx     1626 b- defN 23-Jun-21 10:36 kikiutils_api/utils/__init__.py
 -rw-rw-r--  2.0 unx      989 b- defN 22-Dec-30 18:34 kikiutils_api/utils/blacksheep.py
 -rw-rw-r--  2.0 unx      569 b- defN 22-Dec-21 05:28 kikiutils_api/utils/sanic.py
--rwxr-xr-x  2.0 unx     1066 b- defN 23-Jul-25 00:07 kiki_utils_api-1.5.0.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx      352 b- defN 23-Jul-25 00:07 kiki_utils_api-1.5.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-25 00:07 kiki_utils_api-1.5.0.dist-info/WHEEL
--rwxr-xr-x  2.0 unx       14 b- defN 23-Jul-25 00:07 kiki_utils_api-1.5.0.dist-info/top_level.txt
--rwxr-xr-x  2.0 unx        1 b- defN 23-Jun-21 10:38 kiki_utils_api-1.5.0.dist-info/zip-safe
--rw-rw-r--  2.0 unx     1584 b- defN 23-Jul-25 00:07 kiki_utils_api-1.5.0.dist-info/RECORD
-18 files, 23335 bytes uncompressed, 8161 bytes compressed:  65.0%
+-rwxr-xr-x  2.0 unx     1066 b- defN 23-Jul-25 02:47 kiki_utils_api-1.5.1.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx      352 b- defN 23-Jul-25 02:47 kiki_utils_api-1.5.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-25 02:47 kiki_utils_api-1.5.1.dist-info/WHEEL
+-rwxr-xr-x  2.0 unx       14 b- defN 23-Jul-25 02:47 kiki_utils_api-1.5.1.dist-info/top_level.txt
+-rwxr-xr-x  2.0 unx        1 b- defN 23-Jun-21 10:38 kiki_utils_api-1.5.1.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     1584 b- defN 23-Jul-25 02:47 kiki_utils_api-1.5.1.dist-info/RECORD
+18 files, 22328 bytes uncompressed, 7957 bytes compressed:  64.4%
```

## zipnote {}

```diff
@@ -30,26 +30,26 @@
 
 Filename: kikiutils_api/utils/blacksheep.py
 Comment: 
 
 Filename: kikiutils_api/utils/sanic.py
 Comment: 
 
-Filename: kiki_utils_api-1.5.0.dist-info/LICENSE.txt
+Filename: kiki_utils_api-1.5.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: kiki_utils_api-1.5.0.dist-info/METADATA
+Filename: kiki_utils_api-1.5.1.dist-info/METADATA
 Comment: 
 
-Filename: kiki_utils_api-1.5.0.dist-info/WHEEL
+Filename: kiki_utils_api-1.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: kiki_utils_api-1.5.0.dist-info/top_level.txt
+Filename: kiki_utils_api-1.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: kiki_utils_api-1.5.0.dist-info/zip-safe
+Filename: kiki_utils_api-1.5.1.dist-info/zip-safe
 Comment: 
 
-Filename: kiki_utils_api-1.5.0.dist-info/RECORD
+Filename: kiki_utils_api-1.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kikiutils_api/classes/__init__.py

```diff
@@ -1,87 +1,78 @@
 from abc import abstractmethod
-from asyncio import create_task, Future
-from functools import wraps
+from asyncio import create_task
 from kikiutils.aes import AesCrypt
 from kikiutils.time import now_time_utc
-from typing import Callable, Coroutine, Optional, Type
+from kikiutils.typehint import P, T
+from typing import Any, Callable, Coroutine, Type
 from uuid import uuid1
 
 
 class BaseServiceWebsocketConnection:
     code: str = ''
 
     def __init__(self, aes: AesCrypt, extra_headers: dict, name: str, request, websocket):
-        self.aes = aes
+        self._aes = aes
         self.extra_headers = extra_headers
         self.ip = self._get_ip(request)
         self.name = name
         self.request = request
         self.time: int = now_time_utc()
         self.uuid = uuid1()
         self.ws = websocket
 
+    @abstractmethod
     def _get_ip(self, rq):
         return ''
 
     @abstractmethod
     async def emit(self, event: str, *args, **kwargs):
-        await self.send(self.aes.encrypt([event, args, kwargs]))
+        await self.send(self._aes.encrypt([event, args, kwargs]))
 
     @abstractmethod
     async def recv_data(self) -> list:
         return []
 
 
 class BaseServiceWebsockets:
     _connection_class: Type[BaseServiceWebsocketConnection]
     need_accept = False
 
     def __init__(self, aes: AesCrypt, service_name: str):
-        self.aes = aes
+        self._aes = aes
         self.connections: dict[str, Type[BaseServiceWebsocketConnection]] = {}
         self.event_handlers: dict[str, Callable[..., Coroutine]] = {}
         self.service_name = service_name
-        self.waiting_events: dict[str, dict[str, Future]] = {}
 
     @abstractmethod
     def _add_connection(self, name: str, connection: Type[BaseServiceWebsocketConnection]):
         self.connections[name] = connection
 
     @abstractmethod
     def _del_connection(self, name: str):
         self.connections.pop(name, None)
 
     @abstractmethod
     async def _listen(self, connection: Type[BaseServiceWebsocketConnection]):
         while True:
             event, args, kwargs = await connection.recv_data()
 
-            if event in self.event_handlers:
-                create_task(
-                    self.event_handlers[event](connection, *args, **kwargs)
-                )
-
-            if event in self.waiting_events:
-                uuid: Optional[str] = kwargs.get('__wait_event_uuid')
-
-                if uuid and uuid in self.waiting_events[event]:
-                    self.waiting_events[event][uuid].set_result((args, kwargs))
-                    self.waiting_events[event].pop(uuid, None)
+            if handler := self.event_handlers.get(event):
+                create_task(handler(connection, *args, **kwargs))
 
     @abstractmethod
     async def accept_and_listen(self, name: str, request, websocket, extra_headers: dict = {}):
         if self.need_accept:
             await websocket.accept()
 
         connection = None
 
         try:
             connection = self._connection_class(
-                self.aes,
+                self._aes,
                 extra_headers,
                 name,
                 request,
                 websocket
             )
 
             data = await connection.recv_data()
@@ -95,47 +86,31 @@
         except:
             pass
 
         if connection and name in self.connections and connection.uuid == self.connections[name].uuid:
             self._del_connection(name)
 
     @abstractmethod
-    async def emit_and_wait_event(self, name: str, event: str, wait_event: str, *args, **kwargs):
-        uuid = uuid1().hex
-        kwargs['__wait_event_uuid'] = uuid
-
-        if wait_event in self.waiting_events:
-            self.waiting_events[wait_event][uuid] = Future()
-        else:
-            self.waiting_events[wait_event] = {uuid: Future()}
-
-        await self.emit_to_name(name, event, *args, **kwargs)
-        return await self.waiting_events[wait_event][uuid]
-
-    @abstractmethod
     async def emit_to_all(self, event: str, *args, **kwargs):
-        data = self.aes.encrypt([event, args, kwargs])
+        data = self._aes.encrypt([event, args, kwargs])
 
         for connection in self.connections.values():
             create_task(connection.send(data))
 
     @abstractmethod
     async def emit_to_name(self, name: str, event: str, *args, **kwargs):
         if connection := self.connections.get(name):
-            data = self.aes.encrypt([event, args, kwargs])
+            data = self._aes.encrypt([event, args, kwargs])
             await connection.send(data)
 
     @abstractmethod
     def get_connection(self, name):
         return self.connections.get(name)
 
     @abstractmethod
     def on(self, event: str):
         """Register event handler."""
 
-        def decorator(view_func):
-            @wraps(view_func)
-            async def wrapped_view(*args, **kwargs):
-                await view_func(*args, **kwargs)
-            self.event_handlers[event] = wrapped_view
-            return wrapped_view
+        def decorator(view_func: Callable[P, Coroutine[Any, Any, T]]):
+            self.event_handlers[event] = view_func
+            return view_func
         return decorator
```

## Comparing `kiki_utils_api-1.5.0.dist-info/LICENSE.txt` & `kiki_utils_api-1.5.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `kiki_utils_api-1.5.0.dist-info/RECORD` & `kiki_utils_api-1.5.1.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 kikiutils_api/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kikiutils_api/classes/__init__.py,sha256=6yU2CrwyJr6BRHKX8Xa8_0ZVeYBNErJs1BBDsHueXD8,4641
+kikiutils_api/classes/__init__.py,sha256=c4jsjf9UK08GtpimsWAJm5SYkHv3XzMsPZHnKpUIcug,3634
 kikiutils_api/classes/blacksheep.py,sha256=pKlJenvk_UjW6we5H-iOYsRvIozW3tEDcGN1W_-odpk,796
 kikiutils_api/classes/sanic.py,sha256=N8Z9zlD1pKct1mWk7po0el3qkCGVJGKZpkJzXlkcKe0,701
 kikiutils_api/classes/transmission.py,sha256=w8InlUTgVoigiMTZc1cGw3pxR1G34cXGlK_0_tF-5tQ,2356
 kikiutils_api/classes/websocket.py,sha256=_-T0kvQi4G6GD_Vx1Qt2XJG0HOCB-BKarUjPhYlrWDs,3552
 kikiutils_api/decorators/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kikiutils_api/decorators/blacksheep.py,sha256=rQVsYUh9XCrowYylAXH4eMs8utknBMltvEKKlqzHOOE,1563
 kikiutils_api/decorators/sanic.py,sha256=zO6eWfMg_XdotAI1zrVnBBKAU0Y-hKw4_5z2V4E16-8,3433
 kikiutils_api/utils/__init__.py,sha256=rXwGW0d09QZm5hTdNZtm2H8KC7VM7UHO9PKDZz54AOg,1626
 kikiutils_api/utils/blacksheep.py,sha256=Z-6xf1KrE5CY7_v4z_fAh-UvG_CU3VZz_TxCTBManMo,989
 kikiutils_api/utils/sanic.py,sha256=-O9y1BBD2r2sGnPeq8XuZxeCLetk7kxj-4b4BA6qOgk,569
-kiki_utils_api-1.5.0.dist-info/LICENSE.txt,sha256=44b-vTY24N3ceU0dOUgyn24TtON5bW0tO0uRpSrTD3M,1066
-kiki_utils_api-1.5.0.dist-info/METADATA,sha256=mOhFs7UiQwdeCQDKFToknfGc5x5vwPQwY4pjJALcFOU,352
-kiki_utils_api-1.5.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-kiki_utils_api-1.5.0.dist-info/top_level.txt,sha256=v3xAK1Wovf8ap8KcQo8pUJnhNAo8aZ8Fcss0VNj92EY,14
-kiki_utils_api-1.5.0.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-kiki_utils_api-1.5.0.dist-info/RECORD,,
+kiki_utils_api-1.5.1.dist-info/LICENSE.txt,sha256=44b-vTY24N3ceU0dOUgyn24TtON5bW0tO0uRpSrTD3M,1066
+kiki_utils_api-1.5.1.dist-info/METADATA,sha256=0NI1W77W51DSqJdCE8uCUsb2kJTWiaS8lzuqkPqrwBE,352
+kiki_utils_api-1.5.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+kiki_utils_api-1.5.1.dist-info/top_level.txt,sha256=v3xAK1Wovf8ap8KcQo8pUJnhNAo8aZ8Fcss0VNj92EY,14
+kiki_utils_api-1.5.1.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+kiki_utils_api-1.5.1.dist-info/RECORD,,
```

