# Comparing `tmp/kiki_utils_api-1.4.9-py3-none-any.whl.zip` & `tmp/kiki_utils_api-1.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 10921 bytes, number of entries: 18
+Zip file size: 10811 bytes, number of entries: 18
 -rw-rw-r--  2.0 unx        0 b- defN 22-Nov-28 10:23 kikiutils_api/__init__.py
 -rw-rw-r--  2.0 unx     4641 b- defN 23-Jun-21 10:31 kikiutils_api/classes/__init__.py
 -rw-rw-r--  2.0 unx      796 b- defN 23-Jan-06 04:19 kikiutils_api/classes/blacksheep.py
 -rw-rw-r--  2.0 unx      701 b- defN 23-Jun-21 10:32 kikiutils_api/classes/sanic.py
 -rw-rw-r--  2.0 unx     2356 b- defN 23-Jun-21 10:32 kikiutils_api/classes/transmission.py
--rw-rw-r--  2.0 unx     4098 b- defN 23-Jul-21 11:06 kikiutils_api/classes/websocket.py
+-rw-rw-r--  2.0 unx     3552 b- defN 23-Jul-25 00:06 kikiutils_api/classes/websocket.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Nov-28 10:23 kikiutils_api/decorators/__init__.py
 -rw-rw-r--  2.0 unx     1563 b- defN 23-Jul-20 10:59 kikiutils_api/decorators/blacksheep.py
 -rw-rw-r--  2.0 unx     3433 b- defN 23-Jan-06 05:44 kikiutils_api/decorators/sanic.py
 -rw-rw-r--  2.0 unx     1626 b- defN 23-Jun-21 10:36 kikiutils_api/utils/__init__.py
 -rw-rw-r--  2.0 unx      989 b- defN 22-Dec-30 18:34 kikiutils_api/utils/blacksheep.py
 -rw-rw-r--  2.0 unx      569 b- defN 22-Dec-21 05:28 kikiutils_api/utils/sanic.py
--rwxr-xr-x  2.0 unx     1066 b- defN 23-Jul-21 11:07 kiki_utils_api-1.4.9.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx      352 b- defN 23-Jul-21 11:07 kiki_utils_api-1.4.9.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-21 11:07 kiki_utils_api-1.4.9.dist-info/WHEEL
--rwxr-xr-x  2.0 unx       14 b- defN 23-Jul-21 11:07 kiki_utils_api-1.4.9.dist-info/top_level.txt
--rwxr-xr-x  2.0 unx        1 b- defN 23-Jun-21 10:38 kiki_utils_api-1.4.9.dist-info/zip-safe
--rw-rw-r--  2.0 unx     1584 b- defN 23-Jul-21 11:07 kiki_utils_api-1.4.9.dist-info/RECORD
-18 files, 23881 bytes uncompressed, 8271 bytes compressed:  65.4%
+-rwxr-xr-x  2.0 unx     1066 b- defN 23-Jul-25 00:07 kiki_utils_api-1.5.0.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx      352 b- defN 23-Jul-25 00:07 kiki_utils_api-1.5.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-25 00:07 kiki_utils_api-1.5.0.dist-info/WHEEL
+-rwxr-xr-x  2.0 unx       14 b- defN 23-Jul-25 00:07 kiki_utils_api-1.5.0.dist-info/top_level.txt
+-rwxr-xr-x  2.0 unx        1 b- defN 23-Jun-21 10:38 kiki_utils_api-1.5.0.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     1584 b- defN 23-Jul-25 00:07 kiki_utils_api-1.5.0.dist-info/RECORD
+18 files, 23335 bytes uncompressed, 8161 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -30,26 +30,26 @@
 
 Filename: kikiutils_api/utils/blacksheep.py
 Comment: 
 
 Filename: kikiutils_api/utils/sanic.py
 Comment: 
 
-Filename: kiki_utils_api-1.4.9.dist-info/LICENSE.txt
+Filename: kiki_utils_api-1.5.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: kiki_utils_api-1.4.9.dist-info/METADATA
+Filename: kiki_utils_api-1.5.0.dist-info/METADATA
 Comment: 
 
-Filename: kiki_utils_api-1.4.9.dist-info/WHEEL
+Filename: kiki_utils_api-1.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: kiki_utils_api-1.4.9.dist-info/top_level.txt
+Filename: kiki_utils_api-1.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: kiki_utils_api-1.4.9.dist-info/zip-safe
+Filename: kiki_utils_api-1.5.0.dist-info/zip-safe
 Comment: 
 
-Filename: kiki_utils_api-1.4.9.dist-info/RECORD
+Filename: kiki_utils_api-1.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kikiutils_api/classes/websocket.py

```diff
@@ -1,13 +1,13 @@
-from asyncio import AbstractEventLoop, Future, get_event_loop, sleep, Task
+from asyncio import AbstractEventLoop, CancelledError, get_event_loop, sleep, Task
 from kikiutils.aes import AesCrypt
 from kikiutils.log import logger
 from kikiutils.string import random_str
-from typing import Callable, Coroutine, Optional
-from uuid import uuid1
+from kikiutils.typehint import P, T
+from typing import Any, Callable, Coroutine
 from websockets.legacy.client import Connect
 
 
 class WebsocketClient:
     _check_task: Task
     _emit_raise_exception: bool
     _listen_task: Task
@@ -19,58 +19,58 @@
         aes: AesCrypt,
         name: str,
         url: str,
         check_interval: int = 3,
         headers: dict = {},
         emit_raise_exception: bool = False
     ):
-        self.aes = aes
+        self._aes = aes
         self.check_interval = check_interval
         self.code = random_str()
         self.connect_kwargs = {
             'extra_headers': {
                 'extra-info': aes.encrypt(headers)
             },
             'ping_interval': None,
             'uri': url
         }
 
         self.disconnecting = False
         self._emit_raise_exception = emit_raise_exception
         self.event_handlers: dict[str, Callable[..., Coroutine]] = {}
         self.name = name
-        self.waiting_events: dict[str, dict[str, Future]] = {}
 
     async def _check(self):
-        try:
-            await sleep(self.check_interval)
-            await self.ws.ping()
-            self._check_task = self._create_task(self._check())
-        except:
-            self._listen_task.cancel()
-            await self.wait_connect_success()
+        while True:
+            try:
+                await sleep(self.check_interval)
+                await self.ws.ping()
+            except CancelledError:
+                break
+            except:
+                self._listen_task.cancel()
+
+                try:
+                    await self.ws.close()
+                except:
+                    pass
+
+                return self._create_task(self.wait_connect_success())
 
-    def _create_task(self, coro: Coroutine):
+    def _create_task(self, coro: Coroutine[Any, Any, T]):
         if self.loop is None:
             self.loop = get_event_loop()
         return self.loop.create_task(coro)
 
     async def _listen(self):
         while True:
-            event, args, kwargs = self.aes.decrypt(await self.ws.recv())
+            event, args, kwargs = self._aes.decrypt(await self.ws.recv())
 
-            if event in self.event_handlers:
-                self._create_task(self.event_handlers[event](*args, **kwargs))
-
-            if event in self.waiting_events:
-                uuid: Optional[str] = kwargs.get('__wait_event_uuid')
-
-                if uuid and uuid in self.waiting_events[event]:
-                    self.waiting_events[event][uuid].set_result((args, kwargs))
-                    self.waiting_events[event].pop(uuid, None)
+            if handler := self.event_handlers.get(event):
+                self._create_task(handler(*args, **kwargs))
 
     async def connect(self):
         if self.disconnecting:
             return
 
         self.ws = await Connect(**self.connect_kwargs)
         await self.emit('init', code=self.code)
@@ -83,47 +83,36 @@
         self._check_task.cancel()
         self._listen_task.cancel()
         await self.ws.close()
         self.disconnecting = False
 
     async def emit(self, event: str, *args, **kwargs):
         if self._emit_raise_exception:
-            await self.ws.send(self.aes.encrypt([event, args, kwargs]))
+            await self.ws.send(self._aes.encrypt([event, args, kwargs]))
         else:
             try:
-                await self.ws.send(self.aes.encrypt([event, args, kwargs]))
+                await self.ws.send(self._aes.encrypt([event, args, kwargs]))
             except:
                 return False
 
         return True
 
-    async def emit_and_wait_event(self, event: str, wait_event: str, *args, **kwargs):
-        uuid = uuid1().hex
-        kwargs['__wait_event_uuid'] = uuid
-
-        if wait_event in self.waiting_events:
-            self.waiting_events[wait_event][uuid] = Future()
-        else:
-            self.waiting_events[wait_event] = {uuid: Future()}
-
-        await self.emit(event, *args, **kwargs)
-        return await self.waiting_events[wait_event][uuid]
-
     def on(self, event: str):
         """Register event handler."""
 
-        def decorator(view_func):
+        def decorator(view_func: Callable[P, Coroutine[Any, Any, T]]):
             self.event_handlers[event] = view_func
             return view_func
         return decorator
 
     async def wait_connect_success(self):
         """Wait for connect success."""
 
         while not self.disconnecting:
             try:
                 await self.connect()
                 break
             except KeyboardInterrupt:
                 exit()
             except:
+                logger.error('Websocket connect error!')
                 await sleep(1)
```

## Comparing `kiki_utils_api-1.4.9.dist-info/LICENSE.txt` & `kiki_utils_api-1.5.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `kiki_utils_api-1.4.9.dist-info/RECORD` & `kiki_utils_api-1.5.0.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 kikiutils_api/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kikiutils_api/classes/__init__.py,sha256=6yU2CrwyJr6BRHKX8Xa8_0ZVeYBNErJs1BBDsHueXD8,4641
 kikiutils_api/classes/blacksheep.py,sha256=pKlJenvk_UjW6we5H-iOYsRvIozW3tEDcGN1W_-odpk,796
 kikiutils_api/classes/sanic.py,sha256=N8Z9zlD1pKct1mWk7po0el3qkCGVJGKZpkJzXlkcKe0,701
 kikiutils_api/classes/transmission.py,sha256=w8InlUTgVoigiMTZc1cGw3pxR1G34cXGlK_0_tF-5tQ,2356
-kikiutils_api/classes/websocket.py,sha256=_B5QozY7sk9N1CyaGh2LeEcMUcWox19Sv4iYL71Rka8,4098
+kikiutils_api/classes/websocket.py,sha256=_-T0kvQi4G6GD_Vx1Qt2XJG0HOCB-BKarUjPhYlrWDs,3552
 kikiutils_api/decorators/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kikiutils_api/decorators/blacksheep.py,sha256=rQVsYUh9XCrowYylAXH4eMs8utknBMltvEKKlqzHOOE,1563
 kikiutils_api/decorators/sanic.py,sha256=zO6eWfMg_XdotAI1zrVnBBKAU0Y-hKw4_5z2V4E16-8,3433
 kikiutils_api/utils/__init__.py,sha256=rXwGW0d09QZm5hTdNZtm2H8KC7VM7UHO9PKDZz54AOg,1626
 kikiutils_api/utils/blacksheep.py,sha256=Z-6xf1KrE5CY7_v4z_fAh-UvG_CU3VZz_TxCTBManMo,989
 kikiutils_api/utils/sanic.py,sha256=-O9y1BBD2r2sGnPeq8XuZxeCLetk7kxj-4b4BA6qOgk,569
-kiki_utils_api-1.4.9.dist-info/LICENSE.txt,sha256=44b-vTY24N3ceU0dOUgyn24TtON5bW0tO0uRpSrTD3M,1066
-kiki_utils_api-1.4.9.dist-info/METADATA,sha256=QV7No1Xudu-l11wYfABKRwSohoUMJCMXrZA401RUM38,352
-kiki_utils_api-1.4.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-kiki_utils_api-1.4.9.dist-info/top_level.txt,sha256=v3xAK1Wovf8ap8KcQo8pUJnhNAo8aZ8Fcss0VNj92EY,14
-kiki_utils_api-1.4.9.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-kiki_utils_api-1.4.9.dist-info/RECORD,,
+kiki_utils_api-1.5.0.dist-info/LICENSE.txt,sha256=44b-vTY24N3ceU0dOUgyn24TtON5bW0tO0uRpSrTD3M,1066
+kiki_utils_api-1.5.0.dist-info/METADATA,sha256=mOhFs7UiQwdeCQDKFToknfGc5x5vwPQwY4pjJALcFOU,352
+kiki_utils_api-1.5.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+kiki_utils_api-1.5.0.dist-info/top_level.txt,sha256=v3xAK1Wovf8ap8KcQo8pUJnhNAo8aZ8Fcss0VNj92EY,14
+kiki_utils_api-1.5.0.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+kiki_utils_api-1.5.0.dist-info/RECORD,,
```

