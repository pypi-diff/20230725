# Comparing `tmp/bs_admin_utils-1.1.4-py3-none-any.whl.zip` & `tmp/bs_admin_utils-1.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 209302 bytes, number of entries: 14
+Zip file size: 209359 bytes, number of entries: 14
 -rw-rw-r--  2.0 unx       13 b- defN 23-Apr-07 03:39 bs_admin_utils/__init__.py
 -rw-rw-r--  2.0 unx     4090 b- defN 23-Jun-21 08:15 bs_admin_utils/api.py
 -rw-rw-r--  2.0 unx      636 b- defN 23-Jul-20 10:44 bs_admin_utils/decorators.py
 -rw-rw-r--  2.0 unx     1098 b- defN 23-Jun-17 08:33 bs_admin_utils/model.py
 -rw-rw-r--  2.0 unx     2439 b- defN 23-Jun-14 10:58 bs_admin_utils/vercode.py
--rw-rw-r--  2.0 unx     2868 b- defN 23-Jul-20 10:50 bs_admin_utils/websocket.py
+-rw-rw-r--  2.0 unx     2926 b- defN 23-Jul-25 02:51 bs_admin_utils/websocket.py
 -rwxr-xr-x  2.0 unx   367112 b- defN 23-Apr-07 03:52 bs_admin_utils/static/arial.ttf
 -rwxr-xr-x  2.0 unx     6248 b- defN 23-Jun-14 10:45 bs_admin_utils/static/nstc.ttf
--rwxr-xr-x  2.0 unx     1067 b- defN 23-Jul-20 10:59 bs_admin_utils-1.1.4.dist-info/LICENSE
--rw-rw-r--  2.0 unx      380 b- defN 23-Jul-20 10:59 bs_admin_utils-1.1.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-20 10:59 bs_admin_utils-1.1.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       20 b- defN 23-Jul-20 10:59 bs_admin_utils-1.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Jul-20 10:59 bs_admin_utils-1.1.4.dist-info/zip-safe
--rw-rw-r--  2.0 unx     1179 b- defN 23-Jul-20 10:59 bs_admin_utils-1.1.4.dist-info/RECORD
-14 files, 387243 bytes uncompressed, 207328 bytes compressed:  46.5%
+-rwxr-xr-x  2.0 unx     1067 b- defN 23-Jul-25 02:52 bs_admin_utils-1.1.5.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      380 b- defN 23-Jul-25 02:52 bs_admin_utils-1.1.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-25 02:52 bs_admin_utils-1.1.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       20 b- defN 23-Jul-25 02:52 bs_admin_utils-1.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jul-25 02:52 bs_admin_utils-1.1.5.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     1179 b- defN 23-Jul-25 02:52 bs_admin_utils-1.1.5.dist-info/RECORD
+14 files, 387301 bytes uncompressed, 207385 bytes compressed:  46.5%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: bs_admin_utils/static/arial.ttf
 Comment: 
 
 Filename: bs_admin_utils/static/nstc.ttf
 Comment: 
 
-Filename: bs_admin_utils-1.1.4.dist-info/LICENSE
+Filename: bs_admin_utils-1.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: bs_admin_utils-1.1.4.dist-info/METADATA
+Filename: bs_admin_utils-1.1.5.dist-info/METADATA
 Comment: 
 
-Filename: bs_admin_utils-1.1.4.dist-info/WHEEL
+Filename: bs_admin_utils-1.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: bs_admin_utils-1.1.4.dist-info/top_level.txt
+Filename: bs_admin_utils-1.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: bs_admin_utils-1.1.4.dist-info/zip-safe
+Filename: bs_admin_utils-1.1.5.dist-info/zip-safe
 Comment: 
 
-Filename: bs_admin_utils-1.1.4.dist-info/RECORD
+Filename: bs_admin_utils-1.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bs_admin_utils/websocket.py

```diff
@@ -1,11 +1,12 @@
 from asyncio import create_task
 from blacksheep import WebSocket
 from kikiutils.json import odumps, oloads
-from typing import Callable, Coroutine
+from kikiutils.typehint import P, T
+from typing import Any, Callable, Coroutine
 
 
 class WebsocketConnection:
     code: str = ''
 
     def __init__(self, websocket: WebSocket):
         self.ws = websocket
@@ -33,25 +34,21 @@
             self.connections[user_code].pop(connection.code, None)
 
             if not len(self.connections[user_code]):
                 self.connections.pop(user_code, None)
 
     async def _listen(self, connection: WebsocketConnection):
         while True:
-            data = await connection.ws.receive_text()
-
-            if data == '':
+            if (data := await connection.ws.receive_text()) == '':
                 continue
 
             event, args, kwargs = oloads(data)
 
-            if event in self.event_handlers:
-                create_task(
-                    self.event_handlers[event](connection, *args, **kwargs)
-                )
+            if handler := self.event_handlers.get(event):
+                create_task(handler(connection, *args, **kwargs))
 
     async def accept_and_listen(self, user_code: str, websocket: WebSocket):
         await websocket.accept()
 
         try:
             connection = WebsocketConnection(websocket)
             data = await connection.recv_data()
@@ -78,11 +75,13 @@
         if user_code is self.connections:
             data = odumps([event, args, kwargs])
 
             for c in self.connections[user_code].values():
                 await c.ws.send_bytes(data)
 
     def on(self, event: str):
-        def decorator(view_func):
+        """Register event handler."""
+
+        def decorator(view_func: Callable[P, Coroutine[Any, Any, T]]):
             self.event_handlers[event] = view_func
             return view_func
         return decorator
```

## Comparing `bs_admin_utils-1.1.4.dist-info/LICENSE` & `bs_admin_utils-1.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bs_admin_utils-1.1.4.dist-info/RECORD` & `bs_admin_utils-1.1.5.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 bs_admin_utils/__init__.py,sha256=da1PTClDMl-IBkrSvq6JC1lnS-K_BASzCvxVhNxN5Ls,13
 bs_admin_utils/api.py,sha256=nQ15WdbjjKV8djnGZ7En3s6DctKit4ygpM_pHN84UrY,4090
 bs_admin_utils/decorators.py,sha256=H6x8ZU-f7ZrNngoyxANDhOyT9zwmeVRIonS089e1RGk,636
 bs_admin_utils/model.py,sha256=-b3qlE6tlobm6mq01j09DHY7Ig25sOfy5q9ogmZTdZU,1098
 bs_admin_utils/vercode.py,sha256=l08RRsQG_n4SzKNkwFBairOhqQ4nxrfpD1FVQm20Lhk,2439
-bs_admin_utils/websocket.py,sha256=3cZQWHM8wbWW2Wy8HIlnaE455naabyqYO0C7Gp7jrkE,2868
+bs_admin_utils/websocket.py,sha256=AqBndTbw1nSaJL2dwIUqZirxvd3RRdPT_1AR8INZF48,2926
 bs_admin_utils/static/arial.ttf,sha256=QTx4-RvTnhNPPAuyBLHVqQ8p35793I_SaVCheAWNXXQ,367112
 bs_admin_utils/static/nstc.ttf,sha256=2tSmFfCuO5olGT35eF2kq3QhyR0aiqRedv4WO4rpqlQ,6248
-bs_admin_utils-1.1.4.dist-info/LICENSE,sha256=qmE7pY48Ur85GJoQksvL5vuMovFb2P-4qcjHj6HF8Ag,1067
-bs_admin_utils-1.1.4.dist-info/METADATA,sha256=Kcy7Fqf98pVLv5cF20TriRo8LB_buOu79I_WEkJsnwg,380
-bs_admin_utils-1.1.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-bs_admin_utils-1.1.4.dist-info/top_level.txt,sha256=sUy6z6pEqYADWdTRh6stGJQfcgyhEiLBteEMm283pF8,20
-bs_admin_utils-1.1.4.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-bs_admin_utils-1.1.4.dist-info/RECORD,,
+bs_admin_utils-1.1.5.dist-info/LICENSE,sha256=qmE7pY48Ur85GJoQksvL5vuMovFb2P-4qcjHj6HF8Ag,1067
+bs_admin_utils-1.1.5.dist-info/METADATA,sha256=4DA3TcLgi9Qux8pXdzUMWK9gpqtXcnQR0NqyEh8jT24,380
+bs_admin_utils-1.1.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+bs_admin_utils-1.1.5.dist-info/top_level.txt,sha256=sUy6z6pEqYADWdTRh6stGJQfcgyhEiLBteEMm283pF8,20
+bs_admin_utils-1.1.5.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+bs_admin_utils-1.1.5.dist-info/RECORD,,
```

