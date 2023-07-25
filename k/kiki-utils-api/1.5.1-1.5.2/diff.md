# Comparing `tmp/kiki_utils_api-1.5.1-py3-none-any.whl.zip` & `tmp/kiki_utils_api-1.5.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 10607 bytes, number of entries: 18
+Zip file size: 10609 bytes, number of entries: 18
 -rw-rw-r--  2.0 unx        0 b- defN 22-Nov-28 10:23 kikiutils_api/__init__.py
 -rw-rw-r--  2.0 unx     3634 b- defN 23-Jul-25 02:47 kikiutils_api/classes/__init__.py
--rw-rw-r--  2.0 unx      796 b- defN 23-Jan-06 04:19 kikiutils_api/classes/blacksheep.py
--rw-rw-r--  2.0 unx      701 b- defN 23-Jun-21 10:32 kikiutils_api/classes/sanic.py
+-rw-rw-r--  2.0 unx      797 b- defN 23-Jul-25 05:03 kikiutils_api/classes/blacksheep.py
+-rw-rw-r--  2.0 unx      702 b- defN 23-Jul-25 05:03 kikiutils_api/classes/sanic.py
 -rw-rw-r--  2.0 unx     2356 b- defN 23-Jun-21 10:32 kikiutils_api/classes/transmission.py
 -rw-rw-r--  2.0 unx     3552 b- defN 23-Jul-25 00:06 kikiutils_api/classes/websocket.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Nov-28 10:23 kikiutils_api/decorators/__init__.py
 -rw-rw-r--  2.0 unx     1563 b- defN 23-Jul-20 10:59 kikiutils_api/decorators/blacksheep.py
 -rw-rw-r--  2.0 unx     3433 b- defN 23-Jan-06 05:44 kikiutils_api/decorators/sanic.py
 -rw-rw-r--  2.0 unx     1626 b- defN 23-Jun-21 10:36 kikiutils_api/utils/__init__.py
 -rw-rw-r--  2.0 unx      989 b- defN 22-Dec-30 18:34 kikiutils_api/utils/blacksheep.py
 -rw-rw-r--  2.0 unx      569 b- defN 22-Dec-21 05:28 kikiutils_api/utils/sanic.py
--rwxr-xr-x  2.0 unx     1066 b- defN 23-Jul-25 02:47 kiki_utils_api-1.5.1.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx      352 b- defN 23-Jul-25 02:47 kiki_utils_api-1.5.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-25 02:47 kiki_utils_api-1.5.1.dist-info/WHEEL
--rwxr-xr-x  2.0 unx       14 b- defN 23-Jul-25 02:47 kiki_utils_api-1.5.1.dist-info/top_level.txt
--rwxr-xr-x  2.0 unx        1 b- defN 23-Jun-21 10:38 kiki_utils_api-1.5.1.dist-info/zip-safe
--rw-rw-r--  2.0 unx     1584 b- defN 23-Jul-25 02:47 kiki_utils_api-1.5.1.dist-info/RECORD
-18 files, 22328 bytes uncompressed, 7957 bytes compressed:  64.4%
+-rwxr-xr-x  2.0 unx     1066 b- defN 23-Jul-25 05:04 kiki_utils_api-1.5.2.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx      352 b- defN 23-Jul-25 05:04 kiki_utils_api-1.5.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-25 05:04 kiki_utils_api-1.5.2.dist-info/WHEEL
+-rwxr-xr-x  2.0 unx       14 b- defN 23-Jul-25 05:04 kiki_utils_api-1.5.2.dist-info/top_level.txt
+-rwxr-xr-x  2.0 unx        1 b- defN 23-Jun-21 10:38 kiki_utils_api-1.5.2.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     1584 b- defN 23-Jul-25 05:04 kiki_utils_api-1.5.2.dist-info/RECORD
+18 files, 22330 bytes uncompressed, 7959 bytes compressed:  64.4%
```

## zipnote {}

```diff
@@ -30,26 +30,26 @@
 
 Filename: kikiutils_api/utils/blacksheep.py
 Comment: 
 
 Filename: kikiutils_api/utils/sanic.py
 Comment: 
 
-Filename: kiki_utils_api-1.5.1.dist-info/LICENSE.txt
+Filename: kiki_utils_api-1.5.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: kiki_utils_api-1.5.1.dist-info/METADATA
+Filename: kiki_utils_api-1.5.2.dist-info/METADATA
 Comment: 
 
-Filename: kiki_utils_api-1.5.1.dist-info/WHEEL
+Filename: kiki_utils_api-1.5.2.dist-info/WHEEL
 Comment: 
 
-Filename: kiki_utils_api-1.5.1.dist-info/top_level.txt
+Filename: kiki_utils_api-1.5.2.dist-info/top_level.txt
 Comment: 
 
-Filename: kiki_utils_api-1.5.1.dist-info/zip-safe
+Filename: kiki_utils_api-1.5.2.dist-info/zip-safe
 Comment: 
 
-Filename: kiki_utils_api-1.5.1.dist-info/RECORD
+Filename: kiki_utils_api-1.5.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kikiutils_api/classes/blacksheep.py

```diff
@@ -14,14 +14,14 @@
 
     async def send(self, data: Union[bytes, str]):
         if isinstance(data, bytes):
             return await self.ws.send_bytes(data)
         await self.ws.send_text(data)
 
     async def recv_data(self) -> list:
-        return self.aes.decrypt(await self.ws.receive_text())
+        return self._aes.decrypt(await self.ws.receive_text())
 
 
 class ServiceWebsockets(BaseServiceWebsockets):
     _connection_class = ServiceWebsocketConnection
     connections: dict[str, ServiceWebsocketConnection]
     need_accept = True
```

## kikiutils_api/classes/sanic.py

```diff
@@ -12,13 +12,13 @@
     def _get_ip(self, rq: Request):
         return rq.remote_addr
 
     async def send(self, data: Union[bytes, str]):
         await self.ws.send(data)
 
     async def recv_data(self) -> list:
-        return self.aes.decrypt(await self.ws.recv())
+        return self._aes.decrypt(await self.ws.recv())
 
 
 class ServiceWebsockets(BaseServiceWebsockets):
     _connection_class = ServiceWebsocketConnection
     connections: dict[str, ServiceWebsocketConnection]
```

## Comparing `kiki_utils_api-1.5.1.dist-info/LICENSE.txt` & `kiki_utils_api-1.5.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `kiki_utils_api-1.5.1.dist-info/RECORD` & `kiki_utils_api-1.5.2.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 kikiutils_api/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kikiutils_api/classes/__init__.py,sha256=c4jsjf9UK08GtpimsWAJm5SYkHv3XzMsPZHnKpUIcug,3634
-kikiutils_api/classes/blacksheep.py,sha256=pKlJenvk_UjW6we5H-iOYsRvIozW3tEDcGN1W_-odpk,796
-kikiutils_api/classes/sanic.py,sha256=N8Z9zlD1pKct1mWk7po0el3qkCGVJGKZpkJzXlkcKe0,701
+kikiutils_api/classes/blacksheep.py,sha256=9yT5bzwFivLKWE9oRICeLppJiH0WC0u3UvOIIz68aco,797
+kikiutils_api/classes/sanic.py,sha256=ig5JmmaKRctLNNwFZKOf2W-1V-Zf7C985tRsqtPV-cA,702
 kikiutils_api/classes/transmission.py,sha256=w8InlUTgVoigiMTZc1cGw3pxR1G34cXGlK_0_tF-5tQ,2356
 kikiutils_api/classes/websocket.py,sha256=_-T0kvQi4G6GD_Vx1Qt2XJG0HOCB-BKarUjPhYlrWDs,3552
 kikiutils_api/decorators/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kikiutils_api/decorators/blacksheep.py,sha256=rQVsYUh9XCrowYylAXH4eMs8utknBMltvEKKlqzHOOE,1563
 kikiutils_api/decorators/sanic.py,sha256=zO6eWfMg_XdotAI1zrVnBBKAU0Y-hKw4_5z2V4E16-8,3433
 kikiutils_api/utils/__init__.py,sha256=rXwGW0d09QZm5hTdNZtm2H8KC7VM7UHO9PKDZz54AOg,1626
 kikiutils_api/utils/blacksheep.py,sha256=Z-6xf1KrE5CY7_v4z_fAh-UvG_CU3VZz_TxCTBManMo,989
 kikiutils_api/utils/sanic.py,sha256=-O9y1BBD2r2sGnPeq8XuZxeCLetk7kxj-4b4BA6qOgk,569
-kiki_utils_api-1.5.1.dist-info/LICENSE.txt,sha256=44b-vTY24N3ceU0dOUgyn24TtON5bW0tO0uRpSrTD3M,1066
-kiki_utils_api-1.5.1.dist-info/METADATA,sha256=0NI1W77W51DSqJdCE8uCUsb2kJTWiaS8lzuqkPqrwBE,352
-kiki_utils_api-1.5.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-kiki_utils_api-1.5.1.dist-info/top_level.txt,sha256=v3xAK1Wovf8ap8KcQo8pUJnhNAo8aZ8Fcss0VNj92EY,14
-kiki_utils_api-1.5.1.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-kiki_utils_api-1.5.1.dist-info/RECORD,,
+kiki_utils_api-1.5.2.dist-info/LICENSE.txt,sha256=44b-vTY24N3ceU0dOUgyn24TtON5bW0tO0uRpSrTD3M,1066
+kiki_utils_api-1.5.2.dist-info/METADATA,sha256=1rXQ5nNgI7ln7CsO7eKEqs6ob7eOANgHTZcew0O8oYM,352
+kiki_utils_api-1.5.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+kiki_utils_api-1.5.2.dist-info/top_level.txt,sha256=v3xAK1Wovf8ap8KcQo8pUJnhNAo8aZ8Fcss0VNj92EY,14
+kiki_utils_api-1.5.2.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+kiki_utils_api-1.5.2.dist-info/RECORD,,
```

