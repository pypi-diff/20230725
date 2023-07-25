# Comparing `tmp/hishel-0.0.1.tar.gz` & `tmp/hishel-0.0.2.tar.gz`

## Comparing `hishel-0.0.1.tar` & `hishel-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hishel-0.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 hishel-0.0.1/README.md
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 hishel-0.0.1/hishel/__about__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 hishel-0.0.1/hishel/__init__.py
--rw-r--r--   0        0        0     8033 2020-02-02 00:00:00.000000 hishel-0.0.1/hishel/_controller.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 hishel-0.0.1/hishel/_exceptions.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 hishel-0.0.1/hishel/_files.py
--rw-r--r--   0        0        0     7719 2020-02-02 00:00:00.000000 hishel-0.0.1/hishel/_headers.py
--rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 hishel-0.0.1/hishel/_serializers.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 hishel-0.0.1/hishel/_utils.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 hishel-0.0.1/hishel/_async/__init__.py
--rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 hishel-0.0.1/hishel/_async/_client.py
--rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 hishel-0.0.1/hishel/_async/_pool.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 hishel-0.0.1/hishel/_async/_storages.py
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 hishel-0.0.1/hishel/_async/_transports.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 hishel-0.0.1/hishel/_sync/__init__.py
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 hishel-0.0.1/hishel/_sync/_client.py
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 hishel-0.0.1/hishel/_sync/_pool.py
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 hishel-0.0.1/hishel/_sync/_storages.py
--rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 hishel-0.0.1/hishel/_sync/_transports.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 hishel-0.0.1/.gitignore
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 hishel-0.0.1/LICENSE
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 hishel-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 hishel-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hishel-0.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0     4004 2020-02-02 00:00:00.000000 hishel-0.0.2/README.md
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/__about__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/__init__.py
+-rw-r--r--   0        0        0     8040 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_controller.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_exceptions.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_files.py
+-rw-r--r--   0        0        0     7921 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_headers.py
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_serializers.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_synchronization.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/py.typed
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_async/__init__.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_async/_client.py
+-rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_async/_pool.py
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_async/_storages.py
+-rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_async/_transports.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_sync/__init__.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_sync/_client.py
+-rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_sync/_pool.py
+-rw-r--r--   0        0        0     3558 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_sync/_storages.py
+-rw-r--r--   0        0        0     5337 2020-02-02 00:00:00.000000 hishel-0.0.2/hishel/_sync/_transports.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 hishel-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 hishel-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 hishel-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 hishel-0.0.2/PKG-INFO
```

### Comparing `hishel-0.0.1/hishel/_controller.py` & `hishel-0.0.2/hishel/_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,108 +1,107 @@
-import time
 import typing as tp
 
 from httpcore import Request, Response
 
 from hishel._headers import parse_cache_control
 
 from ._utils import (
+    BaseClock,
+    Clock,
     extract_header_values,
     extract_header_values_decoded,
     header_presents,
     parse_date,
 )
 
 HEURISTICALLY_CACHABLE = (200, 203, 204, 206, 300, 301, 308, 404, 405, 410, 414, 501)
 
+__all__ = ("Controller",)
+
+
 def get_updated_headers(
-        stored_response_headers: tp.List[tp.Tuple[bytes, bytes]],
-        new_response_headers: tp.List[tp.Tuple[bytes, bytes]]
-    ) -> tp.List[tp.Tuple[bytes, bytes]]:
-        updated_headers = []
-
-        checked = set()
-
-        for key, value in stored_response_headers:
-            if key not in checked and key.lower() != b'content-length':
-                checked.add(key)
-                values = extract_header_values(new_response_headers, key)
-
-                if values:
-                    updated_headers.extend([(key, value) for value in values])
-                else:
-                    values = extract_header_values(stored_response_headers, key)
-                    updated_headers.extend([(key, value) for value in values])
-
-        for key, value in new_response_headers:
-            if key not in checked and key.lower() != b'content-length':
-                values = extract_header_values(new_response_headers, key)
+    stored_response_headers: tp.List[tp.Tuple[bytes, bytes]],
+    new_response_headers: tp.List[tp.Tuple[bytes, bytes]],
+) -> tp.List[tp.Tuple[bytes, bytes]]:
+    updated_headers = []
+
+    checked = set()
+
+    for key, value in stored_response_headers:
+        if key not in checked and key.lower() != b"content-length":
+            checked.add(key)
+            values = extract_header_values(new_response_headers, key)
+
+            if values:
+                updated_headers.extend([(key, value) for value in values])
+            else:
+                values = extract_header_values(stored_response_headers, key)
                 updated_headers.extend([(key, value) for value in values])
 
-        return updated_headers
+    for key, value in new_response_headers:
+        if key not in checked and key.lower() != b"content-length":
+            values = extract_header_values(new_response_headers, key)
+            updated_headers.extend([(key, value) for value in values])
 
+    return updated_headers
 
-def get_freshness_lifetime(response: Response) -> tp.Optional[int]:
 
+def get_freshness_lifetime(response: Response) -> tp.Optional[int]:
     response_cache_control = parse_cache_control(
-        extract_header_values_decoded(response.headers, b'Cache-Control'))
+        extract_header_values_decoded(response.headers, b"Cache-Control")
+    )
 
     if response_cache_control.max_age is not None:
         return response_cache_control.max_age
 
-    if header_presents(response.headers, b'expires'):
-        expires = extract_header_values_decoded(response.headers, b'expires', single=True)[0]
+    if header_presents(response.headers, b"expires"):
+        expires = extract_header_values_decoded(
+            response.headers, b"expires", single=True
+        )[0]
         expires_timestamp = parse_date(expires)
-        date = extract_header_values_decoded(response.headers, b'date', single=True)[0]
+        date = extract_header_values_decoded(response.headers, b"date", single=True)[0]
         date_timestamp = parse_date(date)
 
         return expires_timestamp - date_timestamp
     return None
 
-def get_age(response: Response, clock: "BaseClock") -> tp.Optional[int]:
 
-    date = parse_date(extract_header_values_decoded(response.headers, b'date')[0])
+def get_age(response: Response, clock: "BaseClock") -> tp.Optional[int]:
+    date = parse_date(extract_header_values_decoded(response.headers, b"date")[0])
 
     now = clock.now()
 
     apparent_age = max(0, now - date)
     return int(apparent_age)
 
+
 def allowed_stale(response: Response) -> bool:
     response_cache_control = parse_cache_control(
-        extract_header_values_decoded(response.headers, b'Cache-Control'))
+        extract_header_values_decoded(response.headers, b"Cache-Control")
+    )
 
     if response_cache_control.no_cache:
         return False
 
     if response_cache_control.must_revalidate:
         return False
 
     return True
 
-class BaseClock:
-
-    def now(self) -> int:
-        raise NotImplementedError()
-
-class Clock(BaseClock):
-
-    def now(self) -> int:
-        return int(time.time())
 
 class Controller:
-
-
-    def __init__(self,
-                 cacheable_methods: tp.Optional[tp.List[str]] = None,
-                 cacheable_status_codes: tp.Optional[tp.List[int]] = None,
-                 cache_heuristically: bool = False,
-                 clock: tp.Optional[BaseClock] = None,
-                 allow_stale: bool = False):
-
+    def __init__(
+        self,
+        cacheable_methods: tp.Optional[tp.List[str]] = None,
+        cacheable_status_codes: tp.Optional[tp.List[int]] = None,
+        cache_heuristically: bool = False,
+        clock: tp.Optional[BaseClock] = None,
+        allow_stale: bool = False,
+        always_revalidate: bool = False,
+    ):
         if cacheable_methods:
             self._cacheable_methods = cacheable_methods
         else:
             self._cacheable_methods = ["GET"]
 
         if cacheable_status_codes:
             self._cacheable_status_codes = cacheable_status_codes
@@ -111,45 +110,46 @@
 
         if clock:  # pragma: no cover
             self._clock = clock
         else:
             self._clock = Clock()
         self._cache_heuristically = cache_heuristically
         self._allow_stale = allow_stale
+        self._always_revalidate = always_revalidate
 
     def is_cachable(self, request: Request, response: Response) -> bool:
         """
-            According to https://www.rfc-editor.org/rfc/rfc9111.html#section-3
+        According to https://www.rfc-editor.org/rfc/rfc9111.html#section-3
         """
 
-        method = request.method.decode('ascii')
+        method = request.method.decode("ascii")
 
         if response.status not in self._cacheable_status_codes:
             return False
 
         if response.status in (301, 308):
             return True
 
         # the request method is understood by the cache
         if method not in self._cacheable_methods:
             return False
 
         response_cache_control = parse_cache_control(
-            extract_header_values_decoded(response.headers, b'cache-control')
+            extract_header_values_decoded(response.headers, b"cache-control")
         )
 
         # the response status code is final
         if response.status // 100 == 1:
             return False
 
         # the no-store cache directive is not present in the response (see Section 5.2.2.5)
         if response_cache_control.no_store:
             return False
 
-        expires_presents = header_presents(response.headers, b'expires')
+        expires_presents = header_presents(response.headers, b"expires")
         # the response contains at least one of the following:
         # - a public response directive (see Section 5.2.2.9);
         # - a private response directive, if the cache is not shared (see Section 5.2.2.7);
         # - an Expires header field (see Section 5.3);
         # - a max-age response directive (see Section 5.2.2.1);
         # - if the cache is shared: an s-maxage response directive (see Section 5.2.2.10);
         # - a cache extension that allows it to be cached (see Section 5.2.3); or
@@ -161,53 +161,55 @@
             [
                 response_cache_control.public,
                 response_cache_control.private,
                 expires_presents,
                 response_cache_control.max_age is not None,
             ]
         ):
-
             return False
 
         # response is a cachable!
         return True
 
-
     def _make_request_conditional(self, request: Request, response: Response) -> None:
-
-        if header_presents(response.headers, b'last-modified'):
-            last_modified = extract_header_values(response.headers, b'last-modified', single=True)[0]
+        if header_presents(response.headers, b"last-modified"):
+            last_modified = extract_header_values(
+                response.headers, b"last-modified", single=True
+            )[0]
         else:
             last_modified = None
 
-        if header_presents(response.headers, b'etag'):
-            etag = extract_header_values(response.headers, b'etag', single=True)[0]
+        if header_presents(response.headers, b"etag"):
+            etag = extract_header_values(response.headers, b"etag", single=True)[0]
         else:
             etag = None
 
         precondition_headers: tp.List[tp.Tuple[bytes, bytes]] = []
         if last_modified:
-            precondition_headers.append((b'If-Unmodified-Since', last_modified))
+            precondition_headers.append((b"If-Unmodified-Since", last_modified))
         if etag:
-            precondition_headers.append((b'If-None-Match', etag))
+            precondition_headers.append((b"If-None-Match", etag))
 
         request.headers.extend(precondition_headers)
 
-
-    def construct_response_from_cache(self,
-                                      request: Request,
-                                      response: Response) -> tp.Union[Response, Request]:
-
+    def construct_response_from_cache(
+        self, request: Request, response: Response
+    ) -> tp.Union[Response, Request]:
         if response.status in (301, 308):
             return response
 
         response_cache_control = parse_cache_control(
-            extract_header_values_decoded(response.headers, b'Cache-Control'))
+            extract_header_values_decoded(response.headers, b"Cache-Control")
+        )
 
-        if response_cache_control.no_cache:
+        if (
+            self._always_revalidate
+            or response_cache_control.no_cache
+            or response_cache_control.must_revalidate
+        ):
             self._make_request_conditional(request=request, response=response)
             return request
 
         freshness_lifetime = get_freshness_lifetime(response)
         age = get_age(response, self._clock)
 
         if freshness_lifetime is None or age is None:  # pragma: no cover
@@ -217,17 +219,19 @@
         if is_fresh or (self._allow_stale and allowed_stale(response)):
             return response
 
         else:
             self._make_request_conditional(request=request, response=response)
             return request
 
-    def handle_validation_response(self, old_response: Response, new_response: Response) -> Response:
-
+    def handle_validation_response(
+        self, old_response: Response, new_response: Response
+    ) -> Response:
         if new_response.status == 304:
             headers = get_updated_headers(
                 stored_response_headers=old_response.headers,
-                new_response_headers=new_response.headers)
+                new_response_headers=new_response.headers,
+            )
             old_response.headers = headers
         else:
             return new_response
         return old_response
```

### Comparing `hishel-0.0.1/hishel/_files.py` & `hishel-0.0.2/hishel/_files.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,64 +1,70 @@
 import typing as tp
 
 import anyio
 
 
 class AsyncBaseFileManager:
-
-    def __init__(self,
-                 is_binary: bool) -> None:
+    def __init__(self, is_binary: bool) -> None:
         self.is_binary = is_binary
 
-    async def write_to(self, path: str, data: tp.Union[bytes, str], is_binary: tp.Optional[bool] = None) -> None:
+    async def write_to(
+        self, path: str, data: tp.Union[bytes, str], is_binary: tp.Optional[bool] = None
+    ) -> None:
         raise NotImplementedError()
 
-    async def read_from(self, path: str, is_binary: tp.Optional[bool] = None) -> tp.Union[bytes, str]:
+    async def read_from(
+        self, path: str, is_binary: tp.Optional[bool] = None
+    ) -> tp.Union[bytes, str]:
         raise NotImplementedError()
 
-class AsyncFileManager(AsyncBaseFileManager):
 
-    async def write_to(self,
-                       path: str,
-                       data: tp.Union[bytes, str],
-                       is_binary: tp.Optional[bool] = None) -> None:
+class AsyncFileManager(AsyncBaseFileManager):
+    async def write_to(
+        self, path: str, data: tp.Union[bytes, str], is_binary: tp.Optional[bool] = None
+    ) -> None:
         is_binary = self.is_binary if is_binary is None else is_binary
-        mode = 'wb' if is_binary else 'wt'
+        mode = "wb" if is_binary else "wt"
         async with await anyio.open_file(path, mode) as f:  # type: ignore[call-overload]
             await f.write(data)
 
-    async def read_from(self, path: str, is_binary: tp.Optional[bool] = None) -> tp.Union[bytes, str]:
+    async def read_from(
+        self, path: str, is_binary: tp.Optional[bool] = None
+    ) -> tp.Union[bytes, str]:
         is_binary = self.is_binary if is_binary is None else is_binary
-        mode = 'rb' if is_binary else 'rt'
+        mode = "rb" if is_binary else "rt"
 
         async with await anyio.open_file(path, mode) as f:  # type: ignore[call-overload]
             return tp.cast(tp.Union[bytes, str], await f.read())
 
-class BaseFileManager:
 
-    def __init__(self,
-                 is_binary: bool) -> None:
+class BaseFileManager:
+    def __init__(self, is_binary: bool) -> None:
         self.is_binary = is_binary
 
-    def write_to(self, path: str, data: tp.Union[bytes, str], is_binary: tp.Optional[bool] = None) -> None:
+    def write_to(
+        self, path: str, data: tp.Union[bytes, str], is_binary: tp.Optional[bool] = None
+    ) -> None:
         raise NotImplementedError()
 
-    def read_from(self, path: str, is_binary: tp.Optional[bool] = None) -> tp.Union[bytes, str]:
+    def read_from(
+        self, path: str, is_binary: tp.Optional[bool] = None
+    ) -> tp.Union[bytes, str]:
         raise NotImplementedError()
 
-class FileManager(BaseFileManager):
 
-    def write_to(self, path: str, data: tp.Union[bytes, str], is_binary: tp.Optional[bool] = None) -> None:
+class FileManager(BaseFileManager):
+    def write_to(
+        self, path: str, data: tp.Union[bytes, str], is_binary: tp.Optional[bool] = None
+    ) -> None:
         is_binary = self.is_binary if is_binary is None else is_binary
-        mode = 'wb' if is_binary else 'wt'
+        mode = "wb" if is_binary else "wt"
         with open(path, mode) as f:
             f.write(data)
 
-    def read_from(self, path: str, is_binary: tp.Optional[bool] = None) -> tp.Union[bytes, str]:
+    def read_from(
+        self, path: str, is_binary: tp.Optional[bool] = None
+    ) -> tp.Union[bytes, str]:
         is_binary = self.is_binary if is_binary is None else is_binary
-        mode = 'rb' if is_binary else 'rt'
+        mode = "rb" if is_binary else "rt"
         with open(path, mode) as f:
             return tp.cast(tp.Union[bytes, str], f.read())
-
-
-
-
```

### Comparing `hishel-0.0.1/hishel/_headers.py` & `hishel-0.0.2/hishel/_headers.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 from typing import Any, Dict, List, Optional, Union
 
 from ._exceptions import ParseError, ValidationError
 
 ## Grammar
 
 
-HTAB = '\t'
-SP = ' '
-obs_text = ''.join(chr(i) for i in range(0x80, 0xFF+1))  # 0x80-0xFF
+HTAB = "\t"
+SP = " "
+obs_text = "".join(chr(i) for i in range(0x80, 0xFF + 1))  # 0x80-0xFF
 
 tchar = "!#$%&'*+-.^_`|~0123456789" + string.ascii_letters
-qdtext = ''.join([
-    HTAB,
-    SP,
-    "\x21",
-    ''.join(chr(i) for i in range(0x23, 0x5b+1)),  # 0x23-0x5b
-    ''.join(chr(i) for i in range(0x5D, 0x7E+1)),  # 0x5D-0x7E
-    obs_text
-])
+qdtext = "".join(
+    [
+        HTAB,
+        SP,
+        "\x21",
+        "".join(chr(i) for i in range(0x23, 0x5B + 1)),  # 0x23-0x5b
+        "".join(chr(i) for i in range(0x5D, 0x7E + 1)),  # 0x5D-0x7E
+        obs_text,
+    ]
+)
 
 TIME_FIELDS = [
     "max_age",
     "max_stale",
     "min_fresh",
     "s_maxage",
 ]
@@ -36,39 +38,38 @@
     "only_if_cached",
     "public",
     "proxy_revalidate",
     "stale_if_error",
     "stale_while_revalidate",
 ]
 
-LIST_FIELDS = [
-    "no_cache",
-    "private"
-]
+LIST_FIELDS = ["no_cache", "private"]
 
 __all__ = (
-    'CacheControl',
-    'Vary',
+    "CacheControl",
+    "Vary",
 )
 
+
 def strip_ows_around(text: str) -> str:
     return text.strip(" ").strip("\t")
 
+
 def normalize_directive(text: str) -> str:
-    return text.replace('-', '_')
+    return text.replace("-", "_")
 
-def parse_cache_control(cache_control_values: List[str]) -> "CacheControl":
 
+def parse_cache_control(cache_control_values: List[str]) -> "CacheControl":
     directives = {}
 
     for cache_control_value in cache_control_values:
-        if 'no-cache=' in cache_control_value or "private=" in cache_control_value:
+        if "no-cache=" in cache_control_value or "private=" in cache_control_value:
             cache_control_splited = [cache_control_value]
         else:
-            cache_control_splited = cache_control_value.split(',')
+            cache_control_splited = cache_control_value.split(",")
 
         for directive in cache_control_splited:
             key: str = ""
             value: Optional[str] = None
             dquote = False
 
             if not directive:
@@ -76,81 +77,86 @@
 
             directive = strip_ows_around(directive)
 
             if not directive:
                 raise ParseError("The directive should not contain only whitespaces.")
 
             for i, key_char in enumerate(directive):
-                if key_char == '=':
-                    value = directive[i+1:]
+                if key_char == "=":
+                    value = directive[i + 1 :]
 
                     if not value:
                         raise ParseError("The directive value cannot be left blank.")
 
                     if value[0] == '"':
                         dquote = True
                     if dquote and value[-1] != '"':
                         raise ParseError("Invalid quotes around the value.")
 
                     if not dquote:
                         for value_char in value:
                             if value_char not in tchar:
-                                raise ParseError(f"The character '{value_char!r}' "
-                                                    "is not permitted for the unquoted values.")
+                                raise ParseError(
+                                    f"The character '{value_char!r}' "
+                                    "is not permitted for the unquoted values."
+                                )
                     else:
                         for value_char in value[1:-1]:
                             if value_char not in qdtext:
-                                raise ParseError(f"The character '{value_char!r}' "
-                                                    "is not permitted for the quoted values.")
+                                raise ParseError(
+                                    f"The character '{value_char!r}' "
+                                    "is not permitted for the quoted values."
+                                )
                     break
 
                 if key_char not in tchar:
-                    raise ParseError(f"The character '{key_char!r}' is not permitted in the directive name.")
+                    raise ParseError(
+                        f"The character '{key_char!r}' is not permitted in the directive name."
+                    )
                 key += key_char
             directives[key] = value
     validated_data = CacheControl.validate(directives)
     return CacheControl(**validated_data)
 
 
 class Vary:
-
     def __init__(self, values: List[str]) -> None:
         self._values = values
 
-
     @classmethod
     def from_value(cls, vary_values: List[str]) -> "Vary":
         values = []
 
         for vary_value in vary_values:
-            for field_name in vary_value.split(','):
+            for field_name in vary_value.split(","):
                 field_name = field_name.strip()
                 values.append(field_name)
         return Vary(values)
 
-class CacheControl:
 
-    def __init__(self,
-                 immutable: bool = False,        # [RFC8246]
-                 max_age: Optional[int] = None,  # [RFC9111, Section 5.2.1.1, 5.2.2.1]
-                 max_stale: Optional[int] = None,        # [RFC9111, Section 5.2.1.2]
-                 min_fresh: Optional[int] = None,        # [RFC9111, Section 5.2.1.3]
-                 must_revalidate: bool = False,  # [RFC9111, Section 5.2.2.2]
-                 must_understand: bool = False,  # [RFC9111, Section 5.2.2.3]
-                 no_cache: Union[bool, List[str]] = False,  # [RFC9111, Section 5.2.1.4, 5.2.2.4]
-                 no_store: bool = False,  # [RFC9111, Section 5.2.1.5, 5.2.2.5]
-                 no_transform: bool = False,  # [RFC9111, Section 5.2.1.6, 5.2.2.6]
-                 only_if_cached: bool = False,  # [RFC9111, Section 5.2.1.7]
-                 private: Union[bool, List[str]] = False,  # [RFC9111, Section 5.2.2.7]
-                 proxy_revalidate: bool = False,  # [RFC9111, Section 5.2.2.8]
-                 public: bool = False,  # [RFC9111, Section 5.2.2.9]
-                 s_maxage: Optional[int] = None,  # [RFC9111, Section 5.2.2.10]
-                 stale_if_error: bool = False,  # [RFC5861, Section 4]
-                 stale_while_revalidate: bool = False,  # [RFC5861, Section 3]
-                 ) -> None:
+class CacheControl:
+    def __init__(
+        self,
+        immutable: bool = False,  # [RFC8246]
+        max_age: Optional[int] = None,  # [RFC9111, Section 5.2.1.1, 5.2.2.1]
+        max_stale: Optional[int] = None,  # [RFC9111, Section 5.2.1.2]
+        min_fresh: Optional[int] = None,  # [RFC9111, Section 5.2.1.3]
+        must_revalidate: bool = False,  # [RFC9111, Section 5.2.2.2]
+        must_understand: bool = False,  # [RFC9111, Section 5.2.2.3]
+        no_cache: Union[bool, List[str]] = False,  # [RFC9111, Section 5.2.1.4, 5.2.2.4]
+        no_store: bool = False,  # [RFC9111, Section 5.2.1.5, 5.2.2.5]
+        no_transform: bool = False,  # [RFC9111, Section 5.2.1.6, 5.2.2.6]
+        only_if_cached: bool = False,  # [RFC9111, Section 5.2.1.7]
+        private: Union[bool, List[str]] = False,  # [RFC9111, Section 5.2.2.7]
+        proxy_revalidate: bool = False,  # [RFC9111, Section 5.2.2.8]
+        public: bool = False,  # [RFC9111, Section 5.2.2.9]
+        s_maxage: Optional[int] = None,  # [RFC9111, Section 5.2.2.10]
+        stale_if_error: bool = False,  # [RFC5861, Section 4]
+        stale_while_revalidate: bool = False,  # [RFC5861, Section 3]
+    ) -> None:
         self.immutable = immutable
         self.max_age = max_age
         self.max_stale = max_stale
         self.min_fresh = min_fresh
         self.must_revalidate = must_revalidate
         self.must_understand = must_understand
         self.no_cache = no_cache
@@ -160,62 +166,68 @@
         self.private = private
         self.proxy_revalidate = proxy_revalidate
         self.public = public
         self.s_maxage = s_maxage
         self.stale_if_error = stale_if_error
         self.stale_while_revalidate = stale_while_revalidate
 
-
     @classmethod
     def validate(cls, directives: Dict[str, Any]) -> Dict[str, Any]:
         validated_data: Dict[str, Any] = {}
 
         for key, value in directives.items():
             key = normalize_directive(key)
             if key in TIME_FIELDS:
-
                 if value is None:
-                    raise ValidationError(f"The directive '{key}' necessitates a value.")
-
-                if value[0] == "\"" or value[-1] == "\"":
-                    raise ValidationError(f"The argument '{key}' should be an integer, but a quote was found.")
+                    raise ValidationError(
+                        f"The directive '{key}' necessitates a value."
+                    )
+
+                if value[0] == '"' or value[-1] == '"':
+                    raise ValidationError(
+                        f"The argument '{key}' should be an integer, but a quote was found."
+                    )
 
                 try:
                     validated_data[key] = int(value)
                 except Exception:
-                    raise ValidationError(f"The argument '{key}' should be an integer, but got '{value!r}'.")
+                    raise ValidationError(
+                        f"The argument '{key}' should be an integer, but got '{value!r}'."
+                    )
             elif key in BOOLEAN_FIELDS:
                 if value is not None:
-                    raise ValidationError(f"The directive '{key}' should have no value, but it does.")
+                    raise ValidationError(
+                        f"The directive '{key}' should have no value, but it does."
+                    )
                 validated_data[key] = True
             elif key in LIST_FIELDS:
                 if value is None:
                     validated_data[key] = True
                 else:
                     values = []
-                    for list_value in value[1:-1].split(','):
+                    for list_value in value[1:-1].split(","):
                         if not list_value:
                             raise ValidationError("The list value must not be empty.")
                         list_value = strip_ows_around(list_value)
                         values.append(list_value)
                     validated_data[key] = values
 
         return validated_data
 
     def __repr__(self) -> str:
         fields = ""
 
         for key in TIME_FIELDS:
-            key = key.replace('-', '_')
+            key = key.replace("-", "_")
             value = getattr(self, key)
             if value:
                 fields += f"{key}={value}, "
 
         for key in BOOLEAN_FIELDS:
-            key = key.replace('-', '_')
+            key = key.replace("-", "_")
             value = getattr(self, key)
             if value:
                 fields += f"{key}, "
 
         fields = fields[:-2]
 
         return f"<{type(self).__name__} {fields}>"
```

### Comparing `hishel-0.0.1/hishel/_serializers.py` & `hishel-0.0.2/hishel/_serializers.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,117 +2,123 @@
 import json
 import pickle
 import typing as tp
 
 import yaml
 from httpcore import Response
 
-HEADERS_ENCODING = 'iso-8859-1'
-KNOWN_RESPONSE_EXTENSIONS = ('http_version', 'reason_phrase')
+HEADERS_ENCODING = "iso-8859-1"
+KNOWN_RESPONSE_EXTENSIONS = ("http_version", "reason_phrase")
 
-class BaseSerializer:
 
+class BaseSerializer:
     def dumps(self, response: Response) -> tp.Union[str, bytes]:
         raise NotImplementedError()
 
     def loads(self, data: tp.Union[str, bytes]) -> Response:
         raise NotImplementedError()
 
     @property
     def is_binary(self) -> bool:
         raise NotImplementedError()
 
 
 class PickleSerializer(BaseSerializer):
-
     def dumps(self, response: Response) -> tp.Union[str, bytes]:
         clone_response = Response(
             status=response.status,
             headers=response.headers,
             content=response.content,
-            extensions={key: value for key, value in response.extensions.items() if key in KNOWN_RESPONSE_EXTENSIONS}
+            extensions={
+                key: value
+                for key, value in response.extensions.items()
+                if key in KNOWN_RESPONSE_EXTENSIONS
+            },
         )
         return pickle.dumps(clone_response)
 
     def loads(self, data: tp.Union[str, bytes]) -> Response:
         assert isinstance(data, bytes)
         return tp.cast(Response, pickle.loads(data))
 
     @property
     def is_binary(self) -> bool:  # pragma: no cover
         return True
 
-class DictSerializer(BaseSerializer):
 
+class DictSerializer(BaseSerializer):
     def dumps(self, response: Response) -> tp.Union[str, bytes]:
         response_dict = {
             "status": response.status,
             "headers": [
-                (
-                    key.decode(HEADERS_ENCODING),
-                    value.decode(HEADERS_ENCODING)
-                ) for key, value in response.headers],
-            "content": base64.b64encode(response.content).decode('ascii'),
+                (key.decode(HEADERS_ENCODING), value.decode(HEADERS_ENCODING))
+                for key, value in response.headers
+            ],
+            "content": base64.b64encode(response.content).decode("ascii"),
             "extensions": {
-                key: value.decode('ascii') for key, value in response.extensions.items()
-                if key in KNOWN_RESPONSE_EXTENSIONS}
+                key: value.decode("ascii")
+                for key, value in response.extensions.items()
+                if key in KNOWN_RESPONSE_EXTENSIONS
+            },
         }
 
         return json.dumps(response_dict, indent=4)
 
     def loads(self, data: tp.Union[str, bytes]) -> Response:
         response_dict = json.loads(data)
 
         return Response(
             status=response_dict["status"],
             headers=[
-                (
-                    key.encode(HEADERS_ENCODING),
-                    value.encode(HEADERS_ENCODING)
-                ) for key, value in response_dict["headers"]],
-            content=base64.b64decode(response_dict["content"].encode('ascii')),
+                (key.encode(HEADERS_ENCODING), value.encode(HEADERS_ENCODING))
+                for key, value in response_dict["headers"]
+            ],
+            content=base64.b64decode(response_dict["content"].encode("ascii")),
             extensions={
-                key: value.encode('ascii') for key, value in response_dict["extensions"].items()
-                if key in KNOWN_RESPONSE_EXTENSIONS}
+                key: value.encode("ascii")
+                for key, value in response_dict["extensions"].items()
+                if key in KNOWN_RESPONSE_EXTENSIONS
+            },
         )
 
     @property
     def is_binary(self) -> bool:
         return False
 
-class YamlSerializer(BaseSerializer):
-
 
+class YamlSerializer(BaseSerializer):
     def dumps(self, response: Response) -> tp.Union[str, bytes]:
         response_dict = {
             "status": response.status,
             "headers": [
-                (
-                    key.decode(HEADERS_ENCODING),
-                    value.decode(HEADERS_ENCODING)
-                ) for key, value in response.headers],
-            "content": base64.b64encode(response.content).decode('ascii'),
+                (key.decode(HEADERS_ENCODING), value.decode(HEADERS_ENCODING))
+                for key, value in response.headers
+            ],
+            "content": base64.b64encode(response.content).decode("ascii"),
             "extensions": {
-                key: value.decode('ascii') for key, value in response.extensions.items()
-                if key in KNOWN_RESPONSE_EXTENSIONS}
+                key: value.decode("ascii")
+                for key, value in response.extensions.items()
+                if key in KNOWN_RESPONSE_EXTENSIONS
+            },
         }
         return yaml.safe_dump(response_dict, sort_keys=False)
 
     def loads(self, data: tp.Union[str, bytes]) -> Response:
         response_dict = yaml.safe_load(data)
 
         return Response(
             status=response_dict["status"],
             headers=[
-                (
-                    key.encode(HEADERS_ENCODING),
-                    value.encode(HEADERS_ENCODING)
-                ) for key, value in response_dict["headers"]],
-            content=base64.b64decode(response_dict["content"].encode('ascii')),
+                (key.encode(HEADERS_ENCODING), value.encode(HEADERS_ENCODING))
+                for key, value in response_dict["headers"]
+            ],
+            content=base64.b64decode(response_dict["content"].encode("ascii")),
             extensions={
-                key: value.encode('ascii') for key, value in response_dict["extensions"].items()
-                if key in KNOWN_RESPONSE_EXTENSIONS}
+                key: value.encode("ascii")
+                for key, value in response_dict["extensions"].items()
+                if key in KNOWN_RESPONSE_EXTENSIONS
+            },
         )
 
     @property
     def is_binary(self) -> bool:  # pragma: no cover
         return False
```

### Comparing `hishel-0.0.1/hishel/_utils.py` & `hishel-0.0.2/hishel/_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,86 +1,105 @@
 import calendar
+import time
 import typing as tp
 from email.utils import parsedate_tz
 from hashlib import blake2b
 
+import anyio
 import httpcore
 from httpcore import URL
 
 from ._headers import Vary
 
 
-def normalized_url(url: tp.Union[httpcore.URL, str, bytes]) -> str:
+class BaseClock:
+    def now(self) -> int:
+        raise NotImplementedError()
+
+
+class Clock(BaseClock):
+    def now(self) -> int:
+        return int(time.time())
 
+
+def normalized_url(url: tp.Union[httpcore.URL, str, bytes]) -> str:
     if isinstance(url, str):  # pragma: no cover
         return url
 
     if isinstance(url, bytes):  # pragma: no cover
-        return url.decode('ascii')
+        return url.decode("ascii")
 
     if isinstance(url, httpcore.URL):
         port = f":{url.port}" if url.port is not None else ""
         return f'{url.scheme.decode("ascii")}://{url.host.decode("ascii")}{port}{url.target.decode("ascii")}'
     assert False, "Invalid type for `normalized_url`"  # pragma: no cover
 
 
-def generate_key(method: bytes,
-                 url: URL,
-                 headers: tp.List[tp.Tuple[bytes, bytes]]) -> str:
-
+def generate_key(
+    method: bytes, url: URL, headers: tp.List[tp.Tuple[bytes, bytes]]
+) -> str:
     # TODO: sort vary headers
-    vary_values = [val.decode('ascii') for val in extract_header_values(headers, b'vary')]
+    vary_values = [
+        val.decode("ascii") for val in extract_header_values(headers, b"vary")
+    ]
     vary = Vary.from_value(vary_values=vary_values)
     vary_headers_suffix = b""
     for vary_value in vary._values:
-        vary_headers_suffix += vary_value.encode('ascii') + b'='
-        vary_headers_suffix += b', '.join(extract_header_values(headers, vary_value.encode('ascii')))
+        vary_headers_suffix += vary_value.encode("ascii") + b"="
+        vary_headers_suffix += b", ".join(
+            extract_header_values(headers, vary_value.encode("ascii"))
+        )
 
-    encoded_url = normalized_url(url).encode('ascii')
+    encoded_url = normalized_url(url).encode("ascii")
 
     key_parts = [
-            method,
-            encoded_url,
-            vary_headers_suffix,
-         ]
-
+        method,
+        encoded_url,
+        vary_headers_suffix,
+    ]
 
     key = blake2b(digest_size=16)
     for part in key_parts:
         key.update(part)
     return key.hexdigest()
 
 
 def extract_header_values(
-    headers: tp.List[tp.Tuple[bytes, bytes]],
-    header_key: bytes,
-    single: bool = False
+    headers: tp.List[tp.Tuple[bytes, bytes]], header_key: bytes, single: bool = False
 ) -> tp.List[bytes]:
     extracted_headers = []
 
     for key, value in headers:
         if key.lower() == header_key.lower():
             extracted_headers.append(value)
             if single:
                 break
     return extracted_headers
 
+
 def extract_header_values_decoded(
-    headers: tp.List[tp.Tuple[bytes, bytes]],
-    header_key: bytes,
-    single: bool = False
+    headers: tp.List[tp.Tuple[bytes, bytes]], header_key: bytes, single: bool = False
 ) -> tp.List[str]:
-    values = extract_header_values(headers=headers, header_key=header_key, single=single)
+    values = extract_header_values(
+        headers=headers, header_key=header_key, single=single
+    )
     return [value.decode() for value in values]
 
 
 def header_presents(
-    headers: tp.List[tp.Tuple[bytes, bytes]],
-    header_key: bytes
+    headers: tp.List[tp.Tuple[bytes, bytes]], header_key: bytes
 ) -> bool:
     return bool(extract_header_values(headers, header_key, single=True))
 
 
 def parse_date(date: str) -> int:
     expires = parsedate_tz(date)
     timestamp = calendar.timegm(expires[:6])  # type: ignore
     return timestamp
+
+
+async def asleep(seconds: int) -> None:
+    await anyio.sleep(seconds)
+
+
+def sleep(seconds: int) -> None:
+    time.sleep(seconds)
```

### Comparing `hishel-0.0.1/hishel/_async/_pool.py` & `hishel-0.0.2/hishel/_async/_pool.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,75 +1,93 @@
 import logging
+import types
 import typing as tp
 
 from httpcore._async.interfaces import AsyncRequestInterface
 from httpcore._models import Request, Response
 
 from .._controller import Controller
 from .._serializers import DictSerializer
 from .._utils import generate_key, normalized_url
 from ._storages import AsyncBaseStorage, AsyncFileStorage
 
-logger = logging.getLogger('hishel.pool')
+logger = logging.getLogger("hishel.pool")
 
-__all__ = (
-    "AsyncCacheConnectionPool",
-)
+T = tp.TypeVar("T")
+
+__all__ = ("AsyncCacheConnectionPool",)
 
-class AsyncCacheConnectionPool(AsyncRequestInterface):
 
-    def __init__(self,
-                 pool: AsyncRequestInterface,
-                 storage: tp.Optional[AsyncBaseStorage] = None,
-                 cache_controller: tp.Optional[Controller] = None) -> None:
+class AsyncCacheConnectionPool(AsyncRequestInterface):
+    def __init__(
+        self,
+        pool: AsyncRequestInterface,
+        storage: tp.Optional[AsyncBaseStorage] = None,
+        cache_controller: tp.Optional[Controller] = None,
+    ) -> None:
         self._pool = pool
 
         if storage is not None:  # pragma: no cover
             self._storage = storage
         else:
             self._storage = AsyncFileStorage(serializer=DictSerializer())
 
         if cache_controller is not None:  # pragma: no cover
             self._controller = cache_controller
         else:
             self._controller = Controller()
 
     async def handle_async_request(self, request: Request) -> Response:
-
-        key = generate_key(
-            request.method,
-            request.url,
-            request.headers
-        )
+        key = generate_key(request.method, request.url, request.headers)
         stored_resposne = await self._storage.retreive(key)
 
         url = normalized_url(request.url)
 
         if stored_resposne:
             await stored_resposne.aread()
             logger.debug(f"The cached response for the `{url}` url was found.")
-            res = self._controller.construct_response_from_cache(request=request, response=stored_resposne)
+            res = self._controller.construct_response_from_cache(
+                request=request, response=stored_resposne
+            )
 
             if isinstance(res, Response):
                 logger.debug(f"For the `{url}` url, the cached response was used.")
                 return res
-            elif isinstance(res, Request):
-                logger.debug(f"Validating the response associated with the `{url}` url.")
+            elif isinstance(res, Request):  # pragma: no cover
+                logger.debug(
+                    f"Validating the response associated with the `{url}` url."
+                )
                 response = await self._pool.handle_async_request(res)
                 await response.aread()
                 updated_response = self._controller.handle_validation_response(
                     old_response=stored_resposne, new_response=response
                 )
                 await self._storage.store(key, updated_response)
                 return updated_response
 
-            assert False, "invalid return value for `construct_response_from_cache`"
+            assert (
+                False
+            ), "invalid return value for `construct_response_from_cache`"  # pragma: no cover
         logger.debug(f"A cached response to the url `{url}` was not found.")
         response = await self._pool.handle_async_request(request)
         await response.aread()
 
         if self._controller.is_cachable(request=request, response=response):
             await self._storage.store(key, response)
         else:  # pragma: no cover
             logger.debug(f"The response to the `{url}` url is not cacheable.")
 
         return response
+
+    async def aclose(self) -> None:
+        await self._storage.aclose()
+
+    async def __aenter__(self: T) -> T:
+        return self
+
+    async def __aexit__(
+        self,
+        exc_type: tp.Optional[tp.Type[BaseException]] = None,
+        exc_value: tp.Optional[BaseException] = None,
+        traceback: tp.Optional[types.TracebackType] = None,
+    ) -> None:
+        await self.aclose()
```

### Comparing `hishel-0.0.1/hishel/_async/_storages.py` & `hishel-0.0.2/hishel/_sync/_storages.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,74 +1,120 @@
 import logging
+import time
 import typing as tp
 from pathlib import Path
 
+import redis
 from httpcore import Response
 
 from hishel._serializers import BaseSerializer
 
-from .._files import AsyncFileManager
+from .._files import FileManager
 from .._serializers import DictSerializer
+from .._synchronization import Lock
 
-logger = logging.getLogger('hishel.storages')
+logger = logging.getLogger("hishel.storages")
 
-__all__ = (
-    'AsyncFileStorage',
-)
+__all__ = ("FileStorage", "RedisStorage")
 
-class AsyncBaseStorage:
 
-    def __init__(self,
-                 serializer: tp.Optional[BaseSerializer] = None) -> None:
+class BaseStorage:
+    def __init__(self, serializer: tp.Optional[BaseSerializer] = None) -> None:
         if serializer:  # pragma: no cover
             self._serializer = serializer
         else:
             self._serializer = DictSerializer()
 
-    async def store(self, key: str, response: Response) -> None:
+    def store(self, key: str, response: Response) -> None:
         raise NotImplementedError()
 
-    async def retreive(self, key: str) -> tp.Optional[Response]:
+    def retreive(self, key: str) -> tp.Optional[Response]:
         raise NotImplementedError()
 
+    def close(self) -> None:
+        raise NotImplementedError()
 
-class AsyncFileStorage(AsyncBaseStorage):
 
-    def __init__(self,
-                 serializer: tp.Optional[BaseSerializer] = None,
-                 base_path: tp.Optional[Path] = None) -> None:
+class FileStorage(BaseStorage):
+    def __init__(
+        self,
+        serializer: tp.Optional[BaseSerializer] = None,
+        base_path: tp.Optional[Path] = None,
+        max_cache_age: tp.Optional[int] = None,
+    ) -> None:
         super().__init__(serializer)
         if base_path:  # pragma: no cover
             self._base_path = base_path
         else:
-            self._base_path = Path('./.cache/hishel')
+            self._base_path = Path("./.cache/hishel")
 
         if not self._base_path.is_dir():
             self._base_path.mkdir(parents=True)
 
-        self._file_manager = AsyncFileManager(is_binary=self._serializer.is_binary)
-
-    async def store(self, key: str, response: Response) -> None:
+        self._file_manager = FileManager(is_binary=self._serializer.is_binary)
+        self._max_cache_age = max_cache_age
+        self._lock = Lock()
 
+    def store(self, key: str, response: Response) -> None:
         response_path = self._base_path / key
-        await self._file_manager.write_to(
-            str(response_path),
-            self._serializer.dumps(response)
-        )
 
-    async def retreive(self, key: str) -> tp.Optional[Response]:
+        with self._lock:
+            self._file_manager.write_to(
+                str(response_path), self._serializer.dumps(response)
+            )
+        self._remove_expired_caches()
 
+    def retreive(self, key: str) -> tp.Optional[Response]:
         response_path = self._base_path / key
 
-        if response_path.exists():
-            return self._serializer.loads(
-                await self._file_manager.read_from(str(response_path))
-            )
+        with self._lock:
+            if response_path.exists():
+                return self._serializer.loads(
+                    self._file_manager.read_from(str(response_path))
+                )
+        self._remove_expired_caches()
         return None
 
-    async def delete(self, key: str) -> bool:
-        response_path = self._base_path / key
+    def close(self) -> None:
+        return
+
+    def _remove_expired_caches(self) -> None:
+        if self._max_cache_age is None:
+            return
+
+        with self._lock:
+            for file in self._base_path.iterdir():
+                if file.is_file():
+                    age = time.time() - file.stat().st_mtime
+                    if age > self._max_cache_age:
+                        file.unlink()
+
+
+class RedisStorage(BaseStorage):
+    def __init__(
+        self,
+        serializer: tp.Optional[BaseSerializer] = None,
+        client: tp.Optional[redis.Redis] = None,  # type: ignore
+        max_cache_age: tp.Optional[int] = None,
+    ) -> None:
+        super().__init__(serializer)
+
+        if client is None:
+            self._client = redis.Redis()  # type: ignore
+        else:  # pragma: no cover
+            self._client = client
+        self._max_cache_age = max_cache_age
+
+    def store(self, key: str, response: Response) -> None:
+        self._client.set(
+            key, self._serializer.dumps(response), ex=self._max_cache_age
+        )
+
+    def retreive(self, key: str) -> tp.Optional[Response]:
+        cached_response = self._client.get(key)
+        if cached_response is None:
+            return None
+
+        return self._serializer.loads(cached_response)
 
-        if response_path.exists():
-            response_path.unlink()
-            return True
-        return False
+    def close(self) -> None:  # pragma: no cover
+        self._client.close()
```

### Comparing `hishel-0.0.1/hishel/_async/_transports.py` & `hishel-0.0.2/hishel/_sync/_transports.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,130 +1,163 @@
 import logging
+import types
 import typing as tp
-from typing import AsyncIterator
+from typing import Iterator
 
 import httpcore
 import httpx
-from httpx._types import AsyncByteStream
+from httpx._types import SyncByteStream
 
 from hishel._utils import (
     generate_key,
     normalized_url,
 )
 
 from .._controller import Controller
 from .._serializers import DictSerializer
-from ._storages import AsyncBaseStorage, AsyncFileStorage
+from ._storages import BaseStorage, FileStorage
 
-logger = logging.getLogger('hishel.transports')
+logger = logging.getLogger("hishel.transports")
 
-__all__ = (
-    "AsyncCacheTransport",
-)
+__all__ = ("CacheTransport",)
+T = tp.TypeVar("T")
 
-async def to_httpx_response(httpcore_response: httpcore.Response) -> httpx.Response:
 
+def to_httpx_response(httpcore_response: httpcore.Response) -> httpx.Response:
     response = httpx.Response(
         status_code=httpcore_response.status,
         headers=httpcore_response.headers,
         stream=MockStream(httpcore_response.content),
-        extensions=httpcore_response.extensions
+        extensions=httpcore_response.extensions,
     )
     return response
 
-async def to_httpcore_response(httpx_response: httpx.Response) -> httpcore.Response:
 
-    raw_bytes = b''.join([raw_bytes async for raw_bytes in httpx_response.aiter_raw()])
+def to_httpcore_response(httpx_response: httpx.Response) -> httpcore.Response:
+    raw_bytes = b"".join([raw_bytes for raw_bytes in httpx_response.iter_raw()])
     response = httpcore.Response(
         status=httpx_response.status_code,
         headers=httpx_response.headers.raw,
         content=raw_bytes,
-        extensions=httpx_response.extensions
+        extensions=httpx_response.extensions,
     )
-    await response.aread()
+    response.read()
     return response
 
-async def to_httpx_request(httpcore_request: httpcore.Request) -> httpx.Request:
-    raw_bytes = b''.join([raw_bytes async for raw_bytes in httpcore_request.stream]) #  type: ignore
+
+def to_httpx_request(
+    httpcore_request: httpcore.Request,
+) -> httpx.Request:  # pragma: no cover
+    raw_bytes = b"".join(
+        [raw_bytes for raw_bytes in httpcore_request.stream]  #  type: ignore
+    )
     return httpx.Request(
         httpcore_request.method,
         normalized_url(httpcore_request.url),
         headers=httpcore_request.headers,
         extensions=httpcore_request.extensions,
-        stream=MockStream(raw_bytes)
+        stream=MockStream(raw_bytes),
     )
 
+
 def to_httpcore_request(httpx_request: httpx.Request) -> httpcore.Request:
     return httpcore.Request(
         httpx_request.method,
         str(httpx_request.url),
         headers=httpx_request.headers.raw,
         content=httpx_request.content,
-        extensions=httpx_request.extensions
+        extensions=httpx_request.extensions,
     )
 
-class MockStream(AsyncByteStream):
 
+class MockStream(SyncByteStream):
     def __init__(self, content: bytes) -> None:
         self.content = content
 
-    async def __aiter__(self) -> AsyncIterator[bytes]:
+    def __iter__(self) -> Iterator[bytes]:
         yield self.content
 
-class AsyncCacheTransport(httpx.AsyncBaseTransport):
 
-    def __init__(self,
-                 transport: httpx.AsyncBaseTransport,
-                 storage: tp.Optional[AsyncBaseStorage] = None,
-                 cache_controller: tp.Optional[Controller] = None) -> None:
+class CacheTransport(httpx.BaseTransport):
+    def __init__(
+        self,
+        transport: httpx.BaseTransport,
+        storage: tp.Optional[BaseStorage] = None,
+        cache_controller: tp.Optional[Controller] = None,
+    ) -> None:
         self._transport = transport
 
-        if storage is not None:
+        if storage is not None:  # pragma: no cover
             self._storage = storage
         else:
-            self._storage = AsyncFileStorage(serializer=DictSerializer())
+            self._storage = FileStorage(serializer=DictSerializer())
 
-        if cache_controller is not None:
+        if cache_controller is not None:  # pragma: no cover
             self._controller = cache_controller
         else:
             self._controller = Controller()
 
-    async def handle_async_request(self, request: httpx.Request) -> httpx.Response:
+    def handle_request(self, request: httpx.Request) -> httpx.Response:
         httpcore_request = to_httpcore_request(httpx_request=request)
         key = generate_key(
-            httpcore_request.method,
-            httpcore_request.url,
-            httpcore_request.headers
+            httpcore_request.method, httpcore_request.url, httpcore_request.headers
         )
         url = normalized_url(httpcore_request.url)
 
-        stored_resposne = await self._storage.retreive(key)
+        stored_resposne = self._storage.retreive(key)
 
         if stored_resposne:
-            await stored_resposne.aread()
+            stored_resposne.read()
             logger.debug(f"The cached response for the `{url}` url was found.")
-            res = self._controller.construct_response_from_cache(request=httpcore_request, response=stored_resposne)
+            res = self._controller.construct_response_from_cache(
+                request=httpcore_request, response=stored_resposne
+            )
 
             if isinstance(res, httpcore.Response):
                 logger.debug(f"For the `{url}` url, the cached response was used.")
-                return await to_httpx_response(res)
-            elif isinstance(res, httpcore.Request):
-                logger.debug(f"Validating the response associated with the `{url}` url.")
-                response = await self._transport.handle_async_request(await to_httpx_request(res))
+                return to_httpx_response(res)
+            elif isinstance(res, httpcore.Request):  # pragma: no cover
+                logger.debug(
+                    f"Validating the response associated with the `{url}` url."
+                )
+                response = self._transport.handle_request(
+                    to_httpx_request(res)
+                )
                 updated_response = self._controller.handle_validation_response(
                     old_response=stored_resposne,
-                    new_response=await to_httpcore_response(response)
+                    new_response=to_httpcore_response(response),
                 )
-                await self._storage.store(key, updated_response)
-                return await to_httpx_response(updated_response)
+                self._storage.store(key, updated_response)
+                return to_httpx_response(updated_response)
 
-            assert False, "invalid return value for `construct_response_from_cache`"
+            assert (
+                False
+            ), "invalid return value for `construct_response_from_cache`"  # pragma: no cover
         logger.debug(f"A cached response to the url `{url}` was not found.")
-        response = await self._transport.handle_async_request(request)
+        response = self._transport.handle_request(request)
 
-        httpcore_response = await to_httpcore_response(response)
-        if self._controller.is_cachable(request=httpcore_request, response=httpcore_response):
-            await self._storage.store(key, httpcore_response)
+        httpcore_response = to_httpcore_response(response)
+        if self._controller.is_cachable(
+            request=httpcore_request, response=httpcore_response
+        ):
+            self._storage.store(key, httpcore_response)
         else:
-            logger.debug(f"The response to the `{url}` url is not cacheable.")
-
-        return await to_httpx_response(httpcore_response=httpcore_response)
+            logger.debug(
+                f"The response to the `{url}` url is not cacheable."
+            )  # pragma: no cover
+
+        return to_httpx_response(httpcore_response=httpcore_response)
+
+    def close(self) -> None:
+        self._transport.close()
+        self._storage.close()
+
+    def __enter__(self: T) -> T:
+        return self
+
+    def __exit__(
+        self,
+        exc_type: tp.Optional[tp.Type[BaseException]] = None,
+        exc_value: tp.Optional[BaseException] = None,
+        traceback: tp.Optional[types.TracebackType] = None,
+    ) -> None:
+        self.close()
```

### Comparing `hishel-0.0.1/hishel/_sync/_pool.py` & `hishel-0.0.2/hishel/_sync/_pool.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,75 +1,93 @@
 import logging
+import types
 import typing as tp
 
 from httpcore._sync.interfaces import RequestInterface
 from httpcore._models import Request, Response
 
 from .._controller import Controller
 from .._serializers import DictSerializer
 from .._utils import generate_key, normalized_url
 from ._storages import BaseStorage, FileStorage
 
-logger = logging.getLogger('hishel.pool')
+logger = logging.getLogger("hishel.pool")
 
-__all__ = (
-    "CacheConnectionPool",
-)
+T = tp.TypeVar("T")
+
+__all__ = ("CacheConnectionPool",)
 
-class CacheConnectionPool(RequestInterface):
 
-    def __init__(self,
-                 pool: RequestInterface,
-                 storage: tp.Optional[BaseStorage] = None,
-                 cache_controller: tp.Optional[Controller] = None) -> None:
+class CacheConnectionPool(RequestInterface):
+    def __init__(
+        self,
+        pool: RequestInterface,
+        storage: tp.Optional[BaseStorage] = None,
+        cache_controller: tp.Optional[Controller] = None,
+    ) -> None:
         self._pool = pool
 
         if storage is not None:  # pragma: no cover
             self._storage = storage
         else:
             self._storage = FileStorage(serializer=DictSerializer())
 
         if cache_controller is not None:  # pragma: no cover
             self._controller = cache_controller
         else:
             self._controller = Controller()
 
     def handle_request(self, request: Request) -> Response:
-
-        key = generate_key(
-            request.method,
-            request.url,
-            request.headers
-        )
+        key = generate_key(request.method, request.url, request.headers)
         stored_resposne = self._storage.retreive(key)
 
         url = normalized_url(request.url)
 
         if stored_resposne:
             stored_resposne.read()
             logger.debug(f"The cached response for the `{url}` url was found.")
-            res = self._controller.construct_response_from_cache(request=request, response=stored_resposne)
+            res = self._controller.construct_response_from_cache(
+                request=request, response=stored_resposne
+            )
 
             if isinstance(res, Response):
                 logger.debug(f"For the `{url}` url, the cached response was used.")
                 return res
-            elif isinstance(res, Request):
-                logger.debug(f"Validating the response associated with the `{url}` url.")
+            elif isinstance(res, Request):  # pragma: no cover
+                logger.debug(
+                    f"Validating the response associated with the `{url}` url."
+                )
                 response = self._pool.handle_request(res)
                 response.read()
                 updated_response = self._controller.handle_validation_response(
                     old_response=stored_resposne, new_response=response
                 )
                 self._storage.store(key, updated_response)
                 return updated_response
 
-            assert False, "invalid return value for `construct_response_from_cache`"
+            assert (
+                False
+            ), "invalid return value for `construct_response_from_cache`"  # pragma: no cover
         logger.debug(f"A cached response to the url `{url}` was not found.")
         response = self._pool.handle_request(request)
         response.read()
 
         if self._controller.is_cachable(request=request, response=response):
             self._storage.store(key, response)
         else:  # pragma: no cover
             logger.debug(f"The response to the `{url}` url is not cacheable.")
 
         return response
+
+    def close(self) -> None:
+        self._storage.close()
+
+    def __enter__(self: T) -> T:
+        return self
+
+    def __exit__(
+        self,
+        exc_type: tp.Optional[tp.Type[BaseException]] = None,
+        exc_value: tp.Optional[BaseException] = None,
+        traceback: tp.Optional[types.TracebackType] = None,
+    ) -> None:
+        self.close()
```

### Comparing `hishel-0.0.1/LICENSE` & `hishel-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hishel-0.0.1/pyproject.toml` & `hishel-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,29 +3,28 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "hishel"
 dynamic = ["readme", "version"]
 description = "Persistant cache implementation for httpx and httpcore"
 license = "BSD-3-Clause"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 authors = [
     { name = "Kar Petrosyan", email = "kar.petrosyanpy@gmail.com" },
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Web Environment",
     "Framework :: AsyncIO",
     "Framework :: Trio",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP",
 ]
 dependencies = [
@@ -34,14 +33,18 @@
 
 [project.optional-dependencies]
 
 yaml = [
     "pyyaml==6.0.1",
 ]
 
+redis = [
+    "redis==4.6.0"
+]
+
 [project.urls]
 Homepage = "https://github.com/karosis88/hishel"
 Source = "https://github.com/karosis88/hishel"
 
 [tool.hatch.version]
 path = "hishel/__init__.py"
 
@@ -60,24 +63,25 @@
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 path = "CHANGELOG.md"
 
 [tool.mypy]
 strict = true
 show_error_codes = true
+warn_unused_ignores = false
+
 
 [[tool.mypy.overrides]]
 module = "tests.*"
 disallow_untyped_defs = false
 check_untyped_defs = true
 
 
 [tool.pytest.ini_options]
 addopts = ["-rxXs", "--strict-config", "--strict-markers"]
-markers = ["copied_from(source, changes=None): mark test as copied from somewhere else, along with a description of changes made to accodomate e.g. our test setup"]
 filterwarnings = []
 
 [tool.coverage.run]
 omit = [
     "venv/*", 
     "hishel/_sync/*"
 ]
```

### Comparing `hishel-0.0.1/PKG-INFO` & `hishel-0.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,275 +1,251 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 6869 7368  : 2.1.Name: hish
-00000020: 656c 0a56 6572 7369 6f6e 3a20 302e 302e  el.Version: 0.0.
-00000030: 310a 5375 6d6d 6172 793a 2050 6572 7369  1.Summary: Persi
-00000040: 7374 616e 7420 6361 6368 6520 696d 706c  stant cache impl
-00000050: 656d 656e 7461 7469 6f6e 2066 6f72 2068  ementation for h
-00000060: 7474 7078 2061 6e64 2068 7474 7063 6f72  ttpx and httpcor
-00000070: 650a 5072 6f6a 6563 742d 5552 4c3a 2048  e.Project-URL: H
-00000080: 6f6d 6570 6167 652c 2068 7474 7073 3a2f  omepage, https:/
-00000090: 2f67 6974 6875 622e 636f 6d2f 6b61 726f  /github.com/karo
-000000a0: 7369 7338 382f 6869 7368 656c 0a50 726f  sis88/hishel.Pro
-000000b0: 6a65 6374 2d55 524c 3a20 536f 7572 6365  ject-URL: Source
-000000c0: 2c20 6874 7470 733a 2f2f 6769 7468 7562  , https://github
-000000d0: 2e63 6f6d 2f6b 6172 6f73 6973 3838 2f68  .com/karosis88/h
-000000e0: 6973 6865 6c0a 4175 7468 6f72 2d65 6d61  ishel.Author-ema
-000000f0: 696c 3a20 4b61 7220 5065 7472 6f73 7961  il: Kar Petrosya
-00000100: 6e20 3c6b 6172 2e70 6574 726f 7379 616e  n <kar.petrosyan
-00000110: 7079 4067 6d61 696c 2e63 6f6d 3e0a 4c69  py@gmail.com>.Li
-00000120: 6365 6e73 652d 4578 7072 6573 7369 6f6e  cense-Expression
-00000130: 3a20 4253 442d 332d 436c 6175 7365 0a4c  : BSD-3-Clause.L
-00000140: 6963 656e 7365 2d46 696c 653a 204c 4943  icense-File: LIC
-00000150: 454e 5345 0a43 6c61 7373 6966 6965 723a  ENSE.Classifier:
-00000160: 2044 6576 656c 6f70 6d65 6e74 2053 7461   Development Sta
-00000170: 7475 7320 3a3a 2033 202d 2041 6c70 6861  tus :: 3 - Alpha
-00000180: 0a43 6c61 7373 6966 6965 723a 2045 6e76  .Classifier: Env
-00000190: 6972 6f6e 6d65 6e74 203a 3a20 5765 6220  ironment :: Web 
-000001a0: 456e 7669 726f 6e6d 656e 740a 436c 6173  Environment.Clas
-000001b0: 7369 6669 6572 3a20 4672 616d 6577 6f72  sifier: Framewor
-000001c0: 6b20 3a3a 2041 7379 6e63 494f 0a43 6c61  k :: AsyncIO.Cla
-000001d0: 7373 6966 6965 723a 2046 7261 6d65 776f  ssifier: Framewo
-000001e0: 726b 203a 3a20 5472 696f 0a43 6c61 7373  rk :: Trio.Class
-000001f0: 6966 6965 723a 2049 6e74 656e 6465 6420  ifier: Intended 
-00000200: 4175 6469 656e 6365 203a 3a20 4465 7665  Audience :: Deve
-00000210: 6c6f 7065 7273 0a43 6c61 7373 6966 6965  lopers.Classifie
-00000220: 723a 204c 6963 656e 7365 203a 3a20 4f53  r: License :: OS
-00000230: 4920 4170 7072 6f76 6564 203a 3a20 4253  I Approved :: BS
-00000240: 4420 4c69 6365 6e73 650a 436c 6173 7369  D License.Classi
-00000250: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
-00000260: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
-00000270: 6570 656e 6465 6e74 0a43 6c61 7373 6966  ependent.Classif
-00000280: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000290: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000002a0: 686f 6e20 3a3a 2033 0a43 6c61 7373 6966  hon :: 3.Classif
-000002b0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-000002c0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000002d0: 686f 6e20 3a3a 2033 203a 3a20 4f6e 6c79  hon :: 3 :: Only
-000002e0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-000002f0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000300: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000310: 2e37 0a43 6c61 7373 6966 6965 723a 2050  .7.Classifier: P
-00000320: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000330: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000340: 2033 2e38 0a43 6c61 7373 6966 6965 723a   3.8.Classifier:
-00000350: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-00000360: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000370: 3a3a 2033 2e39 0a43 6c61 7373 6966 6965  :: 3.9.Classifie
-00000380: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000390: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000003a0: 6e20 3a3a 2033 2e31 300a 436c 6173 7369  n :: 3.10.Classi
-000003b0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-000003c0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000003d0: 7468 6f6e 203a 3a20 332e 3131 0a43 6c61  thon :: 3.11.Cla
-000003e0: 7373 6966 6965 723a 2054 6f70 6963 203a  ssifier: Topic :
-000003f0: 3a20 496e 7465 726e 6574 203a 3a20 5757  : Internet :: WW
-00000400: 572f 4854 5450 0a52 6571 7569 7265 732d  W/HTTP.Requires-
-00000410: 5079 7468 6f6e 3a20 3e3d 332e 370a 5265  Python: >=3.7.Re
-00000420: 7175 6972 6573 2d44 6973 743a 2068 7474  quires-Dist: htt
-00000430: 7063 6f72 650a 5072 6f76 6964 6573 2d45  pcore.Provides-E
-00000440: 7874 7261 3a20 7961 6d6c 0a52 6571 7569  xtra: yaml.Requi
-00000450: 7265 732d 4469 7374 3a20 7079 7961 6d6c  res-Dist: pyyaml
-00000460: 3d3d 362e 302e 313b 2065 7874 7261 203d  ==6.0.1; extra =
-00000470: 3d20 2779 616d 6c27 0a44 6573 6372 6970  = 'yaml'.Descrip
-00000480: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
-00000490: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
-000004a0: 0a0a 2320 6869 7368 656c 0a0a 5b21 5b50  ..# hishel..[![P
-000004b0: 7950 4920 2d20 5665 7273 696f 6e5d 2868  yPI - Version](h
-000004c0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-000004d0: 6473 2e69 6f2f 7079 7069 2f76 2f68 6973  ds.io/pypi/v/his
-000004e0: 6865 6c2e 7376 6729 5d28 6874 7470 733a  hel.svg)](https:
-000004f0: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-00000500: 6374 2f68 6973 6865 6c29 0a5b 215b 5079  ct/hishel).[![Py
-00000510: 5049 202d 2050 7974 686f 6e20 5665 7273  PI - Python Vers
-00000520: 696f 6e5d 2868 7474 7073 3a2f 2f69 6d67  ion](https://img
-00000530: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
-00000540: 2f70 7976 6572 7369 6f6e 732f 6869 7368  /pyversions/hish
-00000550: 656c 2e73 7667 295d 2868 7474 7073 3a2f  el.svg)](https:/
-00000560: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-00000570: 742f 6869 7368 656c 290a 0a2d 2d2d 2d2d  t/hishel)..-----
-00000580: 0a0a 2a2a 4869 7368 656c 2028 d5b0 d5ab  ..**Hishel (....
-00000590: d5b7 d5a5 d5ac 2c20 7265 6d65 6d62 6572  ......, remember
-000005a0: 292a 2a20 6973 2061 206c 6962 7261 7279  )** is a library
-000005b0: 2074 6861 7420 696d 706c 656d 656e 7473   that implements
-000005c0: 2048 5454 5020 4361 6368 696e 6720 666f   HTTP Caching fo
-000005d0: 7220 5b48 5454 5058 5d28 6874 7470 733a  r [HTTPX](https:
-000005e0: 2f2f 6769 7468 7562 2e63 6f6d 2f65 6e63  //github.com/enc
-000005f0: 6f64 652f 6874 7470 7829 2061 6e64 205b  ode/httpx) and [
-00000600: 4854 5450 2043 6f72 655d 2868 7474 7073  HTTP Core](https
-00000610: 3a2f 2f67 6974 6875 622e 636f 6d2f 656e  ://github.com/en
-00000620: 636f 6465 2f68 7474 7063 6f72 6529 206c  code/httpcore) l
-00000630: 6962 7261 7269 6573 2069 6e20 6163 636f  ibraries in acco
-00000640: 7264 616e 6365 2077 6974 6820 2a2a 5246  rdance with **RF
-00000650: 4320 3931 3131 2a2a 2c20 7468 6520 6d6f  C 9111**, the mo
-00000660: 7374 2072 6563 656e 7420 6361 6368 696e  st recent cachin
-00000670: 6720 7370 6563 6966 6963 6174 696f 6e2e  g specification.
-00000680: 0a0a 2323 2046 6561 7475 7265 730a 0a2d  ..## Features..-
-00000690: 20f0 9f92 be20 5065 7273 6973 7465 6e63   .... Persistenc
-000006a0: 653a 2052 6573 706f 6e73 6573 2061 7265  e: Responses are
-000006b0: 2063 6163 6865 6420 696e 2074 6865 202a   cached in the *
-000006c0: 2a70 6572 7369 7374 656e 7420 6d65 6d6f  *persistent memo
-000006d0: 7279 2a2a 2066 6f72 206c 6174 6572 2075  ry** for later u
-000006e0: 7365 2e0a 2d20 f09f a4b2 2043 6f6d 7061  se..- .... Compa
-000006f0: 7469 6269 6c69 7479 3a20 4974 2069 7320  tibility: It is 
-00000700: 7665 7279 2073 696d 706c 6520 746f 2069  very simple to i
-00000710: 6e74 6567 7261 7465 2077 6974 6820 796f  ntegrate with yo
-00000720: 7572 202a 2a65 7869 7374 696e 6720 6874  ur **existing ht
-00000730: 7470 7820 636c 6965 6e74 2c20 7472 616e  tpx client, tran
-00000740: 7370 6f72 742c 206f 7220 6874 7470 636f  sport, or httpco
-00000750: 7265 2070 6f6f 6c2e 2a2a 0a2d 20f0 9fa4  re pool.**.- ...
-00000760: 9720 4561 7379 2074 6f20 7573 653a 2059  . Easy to use: Y
-00000770: 6f75 2063 6f6e 7469 6e75 6520 746f 2075  ou continue to u
-00000780: 7365 2074 6865 2068 7474 7078 2061 6e64  se the httpx and
-00000790: 2068 7474 7063 6f72 6520 696e 7465 7266   httpcore interf
-000007a0: 6163 6573 2e20 2a2a 4361 6e20 6265 2069  aces. **Can be i
-000007b0: 6e74 6567 7261 7465 6420 7769 7468 206e  ntegrated with n
-000007c0: 6f20 6368 616e 6765 7320 746f 2074 6865  o changes to the
-000007d0: 2063 6f64 652e 2a2a 0a2d 20f0 9fa7 a020   code.**.- .... 
-000007e0: 536d 6172 743a 2041 7474 656d 7074 7320  Smart: Attempts 
-000007f0: 746f 2063 6c65 6172 6c79 2069 6d70 6c65  to clearly imple
-00000800: 6d65 6e74 2052 4643 2039 3131 312c 2075  ment RFC 9111, u
-00000810: 6e64 6572 7374 616e 6473 2060 5661 7279  nderstands `Vary
-00000820: 602c 2060 4574 6167 602c 2060 4c61 7374  `, `Etag`, `Last
-00000830: 2d4d 6f64 6966 6965 6460 2c20 2060 4361  -Modified`,  `Ca
-00000840: 6368 652d 436f 6e74 726f 6c60 2c20 616e  che-Control`, an
-00000850: 6420 6045 7870 6972 6573 6020 6865 6164  d `Expires` head
-00000860: 6572 732c 2061 6e64 202a 2a68 616e 646c  ers, and **handl
-00000870: 6573 2072 6573 706f 6e73 6520 7265 2d76  es response re-v
-00000880: 616c 6964 6174 696f 6e20 6175 746f 6d61  alidation automa
-00000890: 7469 6361 6c6c 792a 2a2e 0a0a 2323 2051  tically**...## Q
-000008a0: 7569 636b 5374 6172 740a 0a49 6e73 7461  uickStart..Insta
-000008b0: 6c6c 2060 4869 7368 656c 6020 7573 696e  ll `Hishel` usin
-000008c0: 6720 7069 703a 0a60 6060 2073 6865 6c6c  g pip:.``` shell
-000008d0: 0a24 2070 6970 2069 6e73 7461 6c6c 2068  .$ pip install h
-000008e0: 6973 6865 6c0a 6060 600a 0a4c 6574 2773  ishel.```..Let's
-000008f0: 2062 6567 696e 2077 6974 6820 616e 2065   begin with an e
-00000900: 7861 6d70 6c65 206f 6620 6120 6874 7470  xample of a http
-00000910: 7820 636c 6965 6e74 2e0a 0a60 6060 7079  x client...```py
-00000920: 7468 6f6e 0a69 6d70 6f72 7420 6869 7368  thon.import hish
-00000930: 656c 0a0a 636c 6965 6e74 203d 2068 6973  el..client = his
-00000940: 6865 6c2e 4361 6368 6543 6c69 656e 7428  hel.CacheClient(
-00000950: 290a 636c 6965 6e74 2e67 6574 2822 6874  ).client.get("ht
-00000960: 7470 733a 2f2f 7777 772e 6769 7468 7562  tps://www.github
-00000970: 2e63 6f6d 2229 0a63 6c69 656e 742e 6765  .com").client.ge
-00000980: 7428 2268 7474 7073 3a2f 2f77 7777 2e67  t("https://www.g
-00000990: 6974 6875 622e 636f 6d22 2920 2023 2074  ithub.com")  # t
-000009a0: 616b 6573 2066 726f 6d20 7468 6520 6361  akes from the ca
-000009b0: 6368 6520 2876 6572 7920 6661 7374 2129  che (very fast!)
-000009c0: 0a60 6060 0a0a 4966 2074 6865 2072 6573  .```..If the res
-000009d0: 706f 6e73 6520 6973 2063 6163 6865 6162  ponse is cacheab
-000009e0: 6c65 2061 6363 6f72 6469 6e67 2074 6f20  le according to 
-000009f0: 2a2a 5246 4320 3931 3131 2a2a 2c20 6869  **RFC 9111**, hi
-00000a00: 7368 656c 2077 696c 6c20 7361 7665 2069  shel will save i
-00000a10: 7420 666f 7220 6c61 7465 7220 7573 652c  t for later use,
-00000a20: 2073 6f20 7468 6520 7573 6572 206f 6e6c   so the user onl
-00000a30: 7920 6e65 6564 7320 746f 2063 6861 6e67  y needs to chang
-00000a40: 6520 7468 6520 636c 6965 6e74 2061 6e64  e the client and
-00000a50: 2074 6865 2072 6573 7420 6f66 2074 6865   the rest of the
-00000a60: 2073 7461 6666 2077 696c 6c20 6265 2064   staff will be d
-00000a70: 6f6e 6520 6175 746f 6d61 7469 6361 6c6c  one automaticall
-00000a80: 792e 0a0a 4279 2064 6566 6175 6c74 2c20  y...By default, 
-00000a90: 4869 7368 656c 2073 746f 7265 7320 7265  Hishel stores re
-00000aa0: 7370 6f6e 7365 7320 696e 2074 6865 202a  sponses in the *
-00000ab0: 2a2e 2f63 6163 6865 2f68 6973 6865 6c2a  *./cache/hishel*
-00000ac0: 2a20 6469 7265 6374 6f72 792c 2062 7574  * directory, but
-00000ad0: 2074 6869 7320 6265 6861 7669 6f72 2063   this behavior c
-00000ae0: 616e 2062 6520 6f76 6572 7269 6464 656e  an be overridden
-00000af0: 2062 7920 6578 706c 6963 6974 6c79 2073   by explicitly s
-00000b00: 7065 6369 6679 696e 6720 7374 6f72 6167  pecifying storag
-00000b10: 652e 0a0a 4966 2077 6520 6c6f 6f6b 2c20  e...If we look, 
-00000b20: 7765 2063 616e 2073 6565 2074 6861 7420  we can see that 
-00000b30: 6120 6e65 7720 6669 6c65 2077 6173 2063  a new file was c
-00000b40: 7265 6174 6564 2069 6e20 7468 6174 2064  reated in that d
-00000b50: 6972 6563 746f 7279 2e20 5468 6973 2069  irectory. This i
-00000b60: 7320 6f75 7220 7365 7269 616c 697a 6564  s our serialized
-00000b70: 2072 6573 706f 6e73 652e 2048 6973 6865   response. Hishe
-00000b80: 6c20 7573 6573 2074 6865 206a 736f 6e20  l uses the json 
-00000b90: 7365 7269 616c 697a 6572 2062 7920 6465  serializer by de
-00000ba0: 6661 756c 742c 2062 7574 2077 6520 6361  fault, but we ca
-00000bb0: 6e20 6578 706c 6963 6974 6c79 2073 6574  n explicitly set
-00000bc0: 2074 6865 206f 7468 6572 2073 7570 706f   the other suppo
-00000bd0: 7274 6564 2073 6572 6961 6c69 7a65 7273  rted serializers
-00000be0: 2c20 7375 6368 2061 7320 2a2a 5941 4d4c  , such as **YAML
-00000bf0: 2a2a 2061 6e64 202a 2a50 6963 6b6c 652a  ** and **Pickle*
-00000c00: 2a20 7365 7269 616c 697a 6572 732e 0a0a  * serializers...
-00000c10: 5468 6973 2069 7320 686f 7720 7468 6520  This is how the 
-00000c20: 6669 6c65 206c 6f6f 6b73 2e0a 0a60 6060  file looks...```
-00000c30: 206a 736f 6e0a 7b0a 2020 2020 2273 7461   json.{.    "sta
-00000c40: 7475 7322 3a20 3330 312c 0a20 2020 2022  tus": 301,.    "
-00000c50: 6865 6164 6572 7322 3a20 5b0a 2020 2020  headers": [.    
-00000c60: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
-00000c70: 2020 2253 6572 7665 7222 2c0a 2020 2020    "Server",.    
-00000c80: 2020 2020 2020 2020 226e 6769 6e78 220a          "nginx".
-00000c90: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
-00000ca0: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
-00000cb0: 2022 4461 7465 222c 0a20 2020 2020 2020   "Date",.       
-00000cc0: 2020 2020 2022 4672 692c 2032 3120 4a75       "Fri, 21 Ju
-00000cd0: 6c20 3230 3233 2031 343a 3233 3a35 3020  l 2023 14:23:50 
-00000ce0: 474d 5422 0a20 2020 2020 2020 205d 2c0a  GMT".        ],.
-00000cf0: 2020 2020 2020 2020 5b0a 2020 2020 2020          [.      
-00000d00: 2020 2020 2020 2243 6f6e 7465 6e74 2d4c        "Content-L
-00000d10: 656e 6774 6822 2c0a 2020 2020 2020 2020  ength",.        
-00000d20: 2020 2020 2230 220a 2020 2020 2020 2020      "0".        
-00000d30: 5d2c 0a20 2020 2020 2020 205b 0a20 2020  ],.        [.   
-00000d40: 2020 2020 2020 2020 2022 436f 6e6e 6563           "Connec
-00000d50: 7469 6f6e 222c 0a20 2020 2020 2020 2020  tion",.         
-00000d60: 2020 2022 6b65 6570 2d61 6c69 7665 220a     "keep-alive".
-00000d70: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
-00000d80: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
-00000d90: 2022 4c6f 6361 7469 6f6e 222c 0a20 2020   "Location",.   
-00000da0: 2020 2020 2020 2020 2022 6874 7470 733a           "https:
-00000db0: 2f2f 6874 7470 6275 6e2e 6f72 6722 0a20  //httpbun.org". 
-00000dc0: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
-00000dd0: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
-00000de0: 2258 2d50 6f77 6572 6564 2d42 7922 2c0a  "X-Powered-By",.
-00000df0: 2020 2020 2020 2020 2020 2020 2268 7474              "htt
-00000e00: 7062 756e 2f33 6330 6463 3035 3838 3364  pbun/3c0dc05883d
-00000e10: 6439 3231 3261 6333 3862 3034 3730 3530  d9212ac38b047050
-00000e20: 3337 6435 3062 3032 6632 3539 3622 0a20  37d50b02f2596". 
-00000e30: 2020 2020 2020 205d 0a20 2020 205d 2c0a         ].    ],.
-00000e40: 2020 2020 2263 6f6e 7465 6e74 223a 2022      "content": "
-00000e50: 222c 0a20 2020 2022 6578 7465 6e73 696f  ",.    "extensio
-00000e60: 6e73 223a 207b 0a20 2020 2020 2020 2022  ns": {.        "
-00000e70: 6874 7470 5f76 6572 7369 6f6e 223a 2022  http_version": "
-00000e80: 4854 5450 2f31 2e31 222c 0a20 2020 2020  HTTP/1.1",.     
-00000e90: 2020 2022 7265 6173 6f6e 5f70 6872 6173     "reason_phras
-00000ea0: 6522 3a20 224d 6f76 6564 2050 6572 6d61  e": "Moved Perma
-00000eb0: 6e65 6e74 6c79 220a 2020 2020 7d0a 7d0a  nently".    }.}.
-00000ec0: 6060 600a 0a54 6865 7265 2069 7320 616c  ```..There is al
-00000ed0: 6c20 7468 6520 696e 666f 726d 6174 696f  l the informatio
-00000ee0: 6e20 7265 7175 6972 6564 2074 6f20 7265  n required to re
-00000ef0: 6275 696c 6420 7468 6520 7265 7370 6f6e  build the respon
-00000f00: 7365 2c20 696e 636c 7564 696e 6720 7468  se, including th
-00000f10: 6520 636f 6e74 656e 7420 7661 6c75 6520  e content value 
-00000f20: 656e 636f 6465 6420 696e 2062 6173 6536  encoded in base6
-00000f30: 342e 0a0a 4869 7368 656c 2061 6c73 6f20  4...Hishel also 
-00000f40: 776f 726b 7320 7765 6c6c 2077 6974 6820  works well with 
-00000f50: 6874 7470 636f 7265 2c20 616e 6420 796f  httpcore, and yo
-00000f60: 7520 6361 6e20 6d61 6b65 2079 6f75 7220  u can make your 
-00000f70: 6874 7470 636f 7265 2063 6f6e 6e65 6374  httpcore connect
-00000f80: 696f 6e20 706f 6f6c 7320 6361 6368 6561  ion pools cachea
-00000f90: 626c 6520 7769 7468 2061 2073 696e 676c  ble with a singl
-00000fa0: 6520 6c69 6e65 206f 6620 636f 6465 2e0a  e line of code..
-00000fb0: 0a59 6f75 7220 6578 6973 7469 6e67 2063  .Your existing c
-00000fc0: 6f64 650a 6060 6020 7079 7468 6f6e 0a66  ode.``` python.f
-00000fd0: 726f 6d20 6874 7470 636f 7265 2069 6d70  rom httpcore imp
-00000fe0: 6f72 7420 436f 6e6e 6563 7469 6f6e 506f  ort ConnectionPo
-00000ff0: 6f6c 0a0a 706f 6f6c 203d 2043 6f6e 6e65  ol..pool = Conne
-00001000: 6374 696f 6e50 6f6f 6c28 290a 0a2e 2e2e  ctionPool().....
-00001010: 0a60 6060 0a0a 4164 6469 6e67 2048 5454  .```..Adding HTT
-00001020: 5020 6361 6368 696e 6720 746f 2079 6f75  P caching to you
-00001030: 7220 7072 6f67 7261 6d20 7769 6c6c 206d  r program will m
-00001040: 616b 6520 6974 206d 7563 6820 6661 7374  ake it much fast
-00001050: 6572 2061 6e64 206d 6f72 6520 6566 6669  er and more effi
-00001060: 6369 656e 742e 0a60 6060 2070 7974 686f  cient..``` pytho
-00001070: 6e0a 696d 706f 7274 2068 6973 6865 6c0a  n.import hishel.
-00001080: 6672 6f6d 2068 7474 7063 6f72 6520 696d  from httpcore im
-00001090: 706f 7274 2043 6f6e 6e65 6374 696f 6e50  port ConnectionP
-000010a0: 6f6f 6c0a 0a70 6f6f 6c20 3d20 436f 6e6e  ool..pool = Conn
-000010b0: 6563 7469 6f6e 506f 6f6c 2829 0a70 6f6f  ectionPool().poo
-000010c0: 6c20 3d20 6869 7368 656c 2e43 6163 6865  l = hishel.Cache
-000010d0: 436f 6e6e 6563 7469 6f6e 506f 6f6c 2870  ConnectionPool(p
-000010e0: 6f6f 6c3d 706f 6f6c 290a 2e2e 2e0a 6060  ool=pool).....``
-000010f0: 600a 0a41 7320 796f 7520 6361 6e20 7365  `..As you can se
-00001100: 652c 2069 7420 6973 202a 2a65 7874 7265  e, it is **extre
-00001110: 6d65 6c79 2073 696d 706c 6520 746f 2069  mely simple to i
-00001120: 6e74 6567 7261 7465 2a2a 2e20 0a0a       ntegrate**. ..
+00000000: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00000010: 223e 0a20 203c 6120 6872 6566 3d22 223e  ">.  <a href="">
+00000020: 3c69 6d67 2077 6964 7468 3d22 3335 3022  <img width="350"
+00000030: 2068 6569 6768 743d 2232 3530 2220 7372   height="250" sr
+00000040: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
+00000050: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00000060: 2e63 6f6d 2f6b 6172 6f73 6973 3838 2f68  .com/karosis88/h
+00000070: 6973 6865 6c2f 6d61 7374 6572 2f2e 6769  ishel/master/.gi
+00000080: 7468 7562 2f6c 6f67 6f2e 6a70 6722 2061  thub/logo.jpg" a
+00000090: 6c74 3d27 4854 5450 5827 3e3c 2f61 3e0a  lt='HTTPX'></a>.
+000000a0: 3c2f 703e 0a0a 0a3c 7020 616c 6967 6e3d  </p>...<p align=
+000000b0: 2263 656e 7465 7222 3e3c 7374 726f 6e67  "center"><strong
+000000c0: 3e48 6973 6865 6c3c 2f73 7472 6f6e 673e  >Hishel</strong>
+000000d0: 203c 656d 3e2d 2041 6e20 656c 6567 616e   <em>- An elegan
+000000e0: 7420 4854 5450 2043 6163 6865 2069 6d70  t HTTP Cache imp
+000000f0: 6c65 6d65 6e74 6174 696f 6e20 666f 7220  lementation for 
+00000100: 6874 7470 7820 616e 6420 6874 7470 636f  httpx and httpco
+00000110: 7265 2e3c 2f65 6d3e 3c2f 703e 0a0a 0a5b  re.</em></p>...[
+00000120: 215b 5079 5049 202d 2056 6572 7369 6f6e  ![PyPI - Version
+00000130: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000140: 6965 6c64 732e 696f 2f70 7970 692f 762f  ields.io/pypi/v/
+00000150: 6869 7368 656c 2e73 7667 295d 2868 7474  hishel.svg)](htt
+00000160: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
+00000170: 6f6a 6563 742f 6869 7368 656c 290a 5b21  oject/hishel).[!
+00000180: 5b50 7950 4920 2d20 5079 7468 6f6e 2056  [PyPI - Python V
+00000190: 6572 7369 6f6e 5d28 6874 7470 733a 2f2f  ersion](https://
+000001a0: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+000001b0: 7970 692f 7079 7665 7273 696f 6e73 2f68  ypi/pyversions/h
+000001c0: 6973 6865 6c2e 7376 6729 5d28 6874 7470  ishel.svg)](http
+000001d0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+000001e0: 6a65 6374 2f68 6973 6865 6c29 0a21 5b50  ject/hishel).![P
+000001f0: 7950 4920 2d20 4c69 6365 6e73 655d 2868  yPI - License](h
+00000200: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000210: 6473 2e69 6f2f 7079 7069 2f6c 2f68 6973  ds.io/pypi/l/his
+00000220: 6865 6c29 0a21 5b43 6f64 6563 6f76 5d28  hel).![Codecov](
+00000230: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000240: 6c64 732e 696f 2f63 6f64 6563 6f76 2f63  lds.io/codecov/c
+00000250: 2f67 6974 6875 622f 6b61 726f 7369 7338  /github/karosis8
+00000260: 382f 6869 7368 656c 290a 0a0a 2d2d 2d2d  8/hishel)...----
+00000270: 2d0a 0a2a 2a48 6973 6865 6c20 28d5 b0d5  -..**Hishel (...
+00000280: abd5 b7d5 a5d5 ac2c 2072 656d 656d 6265  ......., remembe
+00000290: 7229 2a2a 2069 7320 6120 6c69 6272 6172  r)** is a librar
+000002a0: 7920 7468 6174 2069 6d70 6c65 6d65 6e74  y that implement
+000002b0: 7320 4854 5450 2043 6163 6869 6e67 2066  s HTTP Caching f
+000002c0: 6f72 205b 4854 5450 585d 2868 7474 7073  or [HTTPX](https
+000002d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 656e  ://github.com/en
+000002e0: 636f 6465 2f68 7474 7078 2920 616e 6420  code/httpx) and 
+000002f0: 5b48 5454 5020 436f 7265 5d28 6874 7470  [HTTP Core](http
+00000300: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f65  s://github.com/e
+00000310: 6e63 6f64 652f 6874 7470 636f 7265 2920  ncode/httpcore) 
+00000320: 6c69 6272 6172 6965 7320 696e 2061 6363  libraries in acc
+00000330: 6f72 6461 6e63 6520 7769 7468 202a 2a52  ordance with **R
+00000340: 4643 2039 3131 312a 2a2c 2074 6865 206d  FC 9111**, the m
+00000350: 6f73 7420 7265 6365 6e74 2063 6163 6869  ost recent cachi
+00000360: 6e67 2073 7065 6369 6669 6361 7469 6f6e  ng specification
+00000370: 2e0a 0a23 2320 4665 6174 7572 6573 0a0a  ...## Features..
+00000380: 2d20 f09f 92be 2050 6572 7369 7374 656e  - .... Persisten
+00000390: 6365 3a20 5265 7370 6f6e 7365 7320 6172  ce: Responses ar
+000003a0: 6520 6361 6368 6564 2069 6e20 7468 6520  e cached in the 
+000003b0: 5b2a 2a70 6572 7369 7374 656e 7420 6d65  [**persistent me
+000003c0: 6d6f 7279 2a2a 5d28 6874 7470 733a 2f2f  mory**](https://
+000003d0: 656e 2e6d 2e77 696b 6970 6564 6961 2e6f  en.m.wikipedia.o
+000003e0: 7267 2f77 696b 692f 5065 7273 6973 7465  rg/wiki/Persiste
+000003f0: 6e74 5f6d 656d 6f72 7929 2066 6f72 206c  nt_memory) for l
+00000400: 6174 6572 2075 7365 2e0a 2d20 f09f a4b2  ater use..- ....
+00000410: 2043 6f6d 7061 7469 6269 6c69 7479 3a20   Compatibility: 
+00000420: 4974 2069 7320 636f 6d70 6c65 7465 6c79  It is completely
+00000430: 2063 6f6d 7061 7469 626c 6520 7769 7468   compatible with
+00000440: 2079 6f75 7220 6578 6973 7469 6e67 2074   your existing t
+00000450: 7261 6e73 706f 7274 7320 6f72 2063 6f6e  ransports or con
+00000460: 6e65 6374 696f 6e20 706f 6f6c 732c 202a  nection pools, *
+00000470: 2a77 6865 7468 6572 2074 6865 7920 6172  *whether they ar
+00000480: 6520 6465 6661 756c 742c 2063 7573 746f  e default, custo
+00000490: 6d2c 206f 7220 7072 6f76 6964 6564 2062  m, or provided b
+000004a0: 7920 7468 6972 642d 7061 7274 7920 6c69  y third-party li
+000004b0: 6272 6172 6965 732e 2a2a 0a2d 20f0 9fa4  braries.**.- ...
+000004c0: 9720 4561 7379 2074 6f20 7573 653a 2059  . Easy to use: Y
+000004d0: 6f75 2063 6f6e 7469 6e75 6520 746f 2075  ou continue to u
+000004e0: 7365 2074 6865 2068 7474 7078 2061 6e64  se the httpx and
+000004f0: 2068 7474 7063 6f72 6520 696e 7465 7266   httpcore interf
+00000500: 6163 6573 2e20 2a2a 4361 6e20 6265 2069  aces. **Can be i
+00000510: 6e74 6567 7261 7465 6420 7769 7468 206e  ntegrated with n
+00000520: 6f20 6368 616e 6765 7320 746f 2074 6865  o changes to the
+00000530: 2063 6f64 652e 2a2a 0a2d 20f0 9fa7 a020   code.**.- .... 
+00000540: 536d 6172 743a 2041 7474 656d 7074 7320  Smart: Attempts 
+00000550: 746f 2063 6c65 6172 6c79 2069 6d70 6c65  to clearly imple
+00000560: 6d65 6e74 2052 4643 2039 3131 312c 2075  ment RFC 9111, u
+00000570: 6e64 6572 7374 616e 6473 2060 5661 7279  nderstands `Vary
+00000580: 602c 2060 4574 6167 602c 2060 4c61 7374  `, `Etag`, `Last
+00000590: 2d4d 6f64 6966 6965 6460 2c20 2060 4361  -Modified`,  `Ca
+000005a0: 6368 652d 436f 6e74 726f 6c60 2c20 616e  che-Control`, an
+000005b0: 6420 6045 7870 6972 6573 6020 6865 6164  d `Expires` head
+000005c0: 6572 732c 2061 6e64 202a 2a68 616e 646c  ers, and **handl
+000005d0: 6573 2072 6573 706f 6e73 6520 7265 2d76  es response re-v
+000005e0: 616c 6964 6174 696f 6e20 6175 746f 6d61  alidation automa
+000005f0: 7469 6361 6c6c 792a 2a2e 0a2d 20e2 9a99  tically**..- ...
+00000600: efb8 8f20 436f 6e66 6967 7572 6162 6c65  ... Configurable
+00000610: 3a20 596f 7520 6361 6e20 7370 6563 6966  : You can specif
+00000620: 7920 7468 6520 2a2a 6261 636b 656e 642a  y the **backend*
+00000630: 2a20 7768 6572 6520 7468 6520 7265 7370  * where the resp
+00000640: 6f6e 7365 7320 7368 6f75 6c64 2062 6520  onses should be 
+00000650: 7374 6f72 6564 2c20 7468 6520 2a2a 7365  stored, the **se
+00000660: 7269 616c 697a 6572 2a2a 2c20 616e 6420  rializer**, and 
+00000670: 796f 7520 6361 6e20 7772 6974 6520 796f  you can write yo
+00000680: 7572 206f 776e 202a 2a62 6163 6b65 6e64  ur own **backend
+00000690: 7320 616e 6420 7365 7269 616c 697a 6572  s and serializer
+000006a0: 732a 2a2e 2059 6f75 2063 616e 2061 6c73  s**. You can als
+000006b0: 6f20 7370 6563 6966 7920 7768 6963 6820  o specify which 
+000006c0: 7061 7274 7320 6f66 2052 4643 2039 3131  parts of RFC 911
+000006d0: 3120 2a2a 7368 6f75 6c64 2062 6520 6967  1 **should be ig
+000006e0: 6e6f 7265 6420 616e 6420 7768 6963 6820  nored and which 
+000006f0: 7368 6f75 6c64 206e 6f74 2a2a 2c20 666f  should not**, fo
+00000700: 7220 6578 616d 706c 652c 2079 6f75 2063  r example, you c
+00000710: 616e 2065 7870 6c69 6369 746c 7920 6469  an explicitly di
+00000720: 7361 626c 6520 7374 616c 6520 7265 7370  sable stale resp
+00000730: 6f6e 7365 7320 666f 7220 796f 7572 2073  onses for your s
+00000740: 6166 6574 7920 6f72 2065 6e61 626c 6520  afety or enable 
+00000750: 7265 2d76 616c 6964 6174 696f 6e20 666f  re-validation fo
+00000760: 7220 6561 6368 2072 6573 706f 6e73 6520  r each response 
+00000770: 6265 666f 7265 2075 7369 6e67 2069 742e  before using it.
+00000780: 200a 2d20 f09f 9a80 2056 6572 7920 6661   .- .... Very fa
+00000790: 7374 3a20 5768 656e 202a 2a49 4f20 6973  st: When **IO is
+000007a0: 206e 6f74 2072 6571 7569 7265 642a 2a2c   not required**,
+000007b0: 2079 6f75 7220 7265 7175 6573 7473 2061   your requests a
+000007c0: 7265 2065 7665 6e20 6661 7374 6572 2e0a  re even faster..
+000007d0: 0a0a 2323 2051 7569 636b 5374 6172 740a  ..## QuickStart.
+000007e0: 0a49 6e73 7461 6c6c 2060 4869 7368 656c  .Install `Hishel
+000007f0: 6020 7573 696e 6720 7069 703a 0a60 6060  ` using pip:.```
+00000800: 2073 6865 6c6c 0a24 2070 6970 2069 6e73   shell.$ pip ins
+00000810: 7461 6c6c 2068 6973 6865 6c0a 6060 600a  tall hishel.```.
+00000820: 0a4c 6574 2773 2062 6567 696e 2077 6974  .Let's begin wit
+00000830: 6820 616e 2065 7861 6d70 6c65 206f 6620  h an example of 
+00000840: 6120 6874 7470 7820 636c 6965 6e74 2e0a  a httpx client..
+00000850: 0a60 6060 7079 7468 6f6e 0a69 6d70 6f72  .```python.impor
+00000860: 7420 6869 7368 656c 0a0a 7769 7468 2068  t hishel..with h
+00000870: 6973 6865 6c2e 4361 6368 6543 6c69 656e  ishel.CacheClien
+00000880: 7428 2920 6173 2063 6c69 656e 743a 0a20  t() as client:. 
+00000890: 2020 2063 6c69 656e 742e 6765 7428 2268     client.get("h
+000008a0: 7474 7073 3a2f 2f77 7777 2e67 6974 6875  ttps://www.githu
+000008b0: 622e 636f 6d22 290a 2020 2020 636c 6965  b.com").    clie
+000008c0: 6e74 2e67 6574 2822 6874 7470 733a 2f2f  nt.get("https://
+000008d0: 7777 772e 6769 7468 7562 2e63 6f6d 2229  www.github.com")
+000008e0: 2020 2320 7461 6b65 7320 6672 6f6d 2074    # takes from t
+000008f0: 6865 2063 6163 6865 2028 7665 7279 2066  he cache (very f
+00000900: 6173 7421 290a 6060 600a 0a49 6620 7468  ast!).```..If th
+00000910: 6520 7265 7370 6f6e 7365 2069 7320 6361  e response is ca
+00000920: 6368 6561 626c 6520 6163 636f 7264 696e  cheable accordin
+00000930: 6720 746f 202a 2a52 4643 2039 3131 312a  g to **RFC 9111*
+00000940: 2a2c 2068 6973 6865 6c20 7769 6c6c 2073  *, hishel will s
+00000950: 6176 6520 6974 2066 6f72 206c 6174 6572  ave it for later
+00000960: 2075 7365 2c20 736f 2074 6865 2075 7365   use, so the use
+00000970: 7220 6f6e 6c79 206e 6565 6473 2074 6f20  r only needs to 
+00000980: 6368 616e 6765 2074 6865 202a 2a63 6c69  change the **cli
+00000990: 656e 7420 616e 6420 7468 6520 7265 7374  ent and the rest
+000009a0: 206f 6620 7468 6520 7374 6166 6620 7769   of the staff wi
+000009b0: 6c6c 2062 6520 646f 6e65 2061 7574 6f6d  ll be done autom
+000009c0: 6174 6963 616c 6c79 2e2a 2a0a 0a48 6973  atically.**..His
+000009d0: 6865 6c20 616c 736f 2077 6f72 6b73 2077  hel also works w
+000009e0: 656c 6c20 7769 7468 2068 7474 7063 6f72  ell with httpcor
+000009f0: 652c 2061 6e64 2079 6f75 2063 616e 202a  e, and you can *
+00000a00: 2a6d 616b 6520 796f 7572 2068 7474 7063  *make your httpc
+00000a10: 6f72 6520 636f 6e6e 6563 7469 6f6e 2070  ore connection p
+00000a20: 6f6f 6c73 2063 6163 6865 6162 6c65 2077  ools cacheable w
+00000a30: 6974 6820 6120 7369 6e67 6c65 206c 696e  ith a single lin
+00000a40: 6520 6f66 2063 6f64 652e 2a2a 0a0a 596f  e of code.**..Yo
+00000a50: 7572 2065 7869 7374 696e 6720 636f 6465  ur existing code
+00000a60: 0a60 6060 2070 7974 686f 6e0a 6672 6f6d  .``` python.from
+00000a70: 2068 7474 7063 6f72 6520 696d 706f 7274   httpcore import
+00000a80: 2043 6f6e 6e65 6374 696f 6e50 6f6f 6c0a   ConnectionPool.
+00000a90: 0a70 6f6f 6c20 3d20 436f 6e6e 6563 7469  .pool = Connecti
+00000aa0: 6f6e 506f 6f6c 2829 0a0a 2e2e 2e0a 6060  onPool()......``
+00000ab0: 600a 0a41 6464 696e 6720 4854 5450 2063  `..Adding HTTP c
+00000ac0: 6163 6869 6e67 2074 6f20 796f 7572 2070  aching to your p
+00000ad0: 726f 6772 616d 2077 696c 6c20 6d61 6b65  rogram will make
+00000ae0: 2069 7420 6d75 6368 2066 6173 7465 7220   it much faster 
+00000af0: 616e 6420 6d6f 7265 2065 6666 6963 6965  and more efficie
+00000b00: 6e74 2e0a 6060 6020 7079 7468 6f6e 0a69  nt..``` python.i
+00000b10: 6d70 6f72 7420 6869 7368 656c 0a66 726f  mport hishel.fro
+00000b20: 6d20 6874 7470 636f 7265 2069 6d70 6f72  m httpcore impor
+00000b30: 7420 436f 6e6e 6563 7469 6f6e 506f 6f6c  t ConnectionPool
+00000b40: 0a0a 706f 6f6c 203d 2043 6f6e 6e65 6374  ..pool = Connect
+00000b50: 696f 6e50 6f6f 6c28 290a 706f 6f6c 203d  ionPool().pool =
+00000b60: 2068 6973 6865 6c2e 4361 6368 6543 6f6e   hishel.CacheCon
+00000b70: 6e65 6374 696f 6e50 6f6f 6c28 706f 6f6c  nectionPool(pool
+00000b80: 3d70 6f6f 6c29 0a2e 2e2e 0a60 6060 0a0a  =pool).....```..
+00000b90: 4173 2079 6f75 2063 616e 2073 6565 2c20  As you can see, 
+00000ba0: 6974 2069 7320 2a2a 6578 7472 656d 656c  it is **extremel
+00000bb0: 7920 7369 6d70 6c65 2074 6f20 696e 7465  y simple to inte
+00000bc0: 6772 6174 652a 2a2e 200a 0a42 6563 6175  grate**. ..Becau
+00000bd0: 7365 2060 4869 7368 656c 6020 7265 7370  se `Hishel` resp
+00000be0: 6563 7473 2079 6f75 7220 6375 7374 6f6d  ects your custom
+00000bf0: 2074 7261 6e73 706f 7274 7320 616e 6420   transports and 
+00000c00: 636f 6e6e 6563 7469 6f6e 2070 6f6f 6c73  connection pools
+00000c10: 2c20 6974 2072 6571 7569 7265 7320 7468  , it requires th
+00000c20: 6520 7265 616c 202a 2a43 6f6e 6e65 6374  e real **Connect
+00000c30: 696f 6e50 6f6f 6c2a 2a20 616e 6420 7468  ionPool** and th
+00000c40: 6520 7265 616c 202a 2a48 5454 5054 7261  e real **HTTPTra
+00000c50: 6e73 706f 7274 2a2a 2074 6f20 776f 726b  nsport** to work
+00000c60: 206f 6e20 746f 7020 6f66 2069 742e 0a0a   on top of it...
+00000c70: 2a2a 5472 616e 7370 6f72 7473 2a2a 2065  **Transports** e
+00000c80: 7861 6d70 6c65 3a0a 0a60 6060 2070 7974  xample:..``` pyt
+00000c90: 686f 6e0a 696d 706f 7274 2068 7474 7078  hon.import httpx
+00000ca0: 0a69 6d70 6f72 7420 6869 7368 656c 0a0a  .import hishel..
+00000cb0: 7472 616e 7370 6f72 7420 3d20 6874 7470  transport = http
+00000cc0: 782e 4854 5450 5472 616e 7370 6f72 7428  x.HTTPTransport(
+00000cd0: 290a 6361 6368 655f 7472 616e 7370 6f72  ).cache_transpor
+00000ce0: 7420 3d20 6869 7368 656c 2e43 6163 6865  t = hishel.Cache
+00000cf0: 5472 616e 7370 6f72 7428 7472 616e 7370  Transport(transp
+00000d00: 6f72 743d 7472 616e 7370 6f72 7429 0a0a  ort=transport)..
+00000d10: 7265 7120 3d20 6874 7470 782e 5265 7175  req = httpx.Requ
+00000d20: 6573 7428 2247 4554 222c 0a20 2020 2020  est("GET",.     
+00000d30: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000d40: 6874 7470 733a 2f2f 676f 6f67 6c65 2e63  https://google.c
+00000d50: 6f6d 2229 0a0a 6361 6368 655f 7472 616e  om")..cache_tran
+00000d60: 7370 6f72 742e 6861 6e64 6c65 5f72 6571  sport.handle_req
+00000d70: 7565 7374 2872 6571 290a 6361 6368 655f  uest(req).cache_
+00000d80: 7472 616e 7370 6f72 742e 6861 6e64 6c65  transport.handle
+00000d90: 5f72 6571 7565 7374 2872 6571 290a 6060  _request(req).``
+00000da0: 600a 0a23 2320 486f 7720 616e 6420 7768  `..## How and wh
+00000db0: 6572 6520 6172 6520 7468 6520 7265 7370  ere are the resp
+00000dc0: 6f6e 7365 7320 7361 7665 643f 0a0a 4869  onses saved?..Hi
+00000dd0: 7368 656c 2073 7570 706f 7274 7320 6120  shel supports a 
+00000de0: 7661 7269 6574 7920 6f66 2062 6163 6b65  variety of backe
+00000df0: 6e64 7320 666f 7220 7374 6f72 696e 6720  nds for storing 
+00000e00: 7265 7370 6f6e 7365 732c 2062 7574 2074  responses, but t
+00000e10: 6865 202a 2a66 696c 6573 7973 7465 6d20  he **filesystem 
+00000e20: 6973 2074 6865 2064 6566 6175 6c74 2a2a  is the default**
+00000e30: 2e0a 0a59 6f75 2063 616e 2061 6c73 6f20  ...You can also 
+00000e40: 7573 6520 616e 6f74 6865 7220 6261 636b  use another back
+00000e50: 656e 642c 2073 7563 6820 6173 202a 2a72  end, such as **r
+00000e60: 6564 6973 2a2a 2c20 746f 2073 746f 7265  edis**, to store
+00000e70: 2079 6f75 7220 7265 7370 6f6e 7365 732c   your responses,
+00000e80: 206f 7220 6576 656e 202a 2a77 7269 7465   or even **write
+00000e90: 2079 6f75 7220 6f77 6e2a 2a20 6966 206e   your own** if n
+00000ea0: 6563 6573 7361 7279 2e0a 0a0a 2323 2043  ecessary....## C
+00000eb0: 6f6e 7472 6962 7574 696e 670a 0a48 6973  ontributing..His
+00000ec0: 6865 6c20 6973 2061 2070 6f77 6572 6675  hel is a powerfu
+00000ed0: 6c20 746f 6f6c 2c20 6275 7420 6974 2069  l tool, but it i
+00000ee0: 7320 616c 736f 2061 206e 6577 2070 726f  s also a new pro
+00000ef0: 6a65 6374 2077 6974 6820 706f 7465 6e74  ject with potent
+00000f00: 6961 6c20 666c 6177 732c 2073 6f20 7765  ial flaws, so we
+00000f10: 2077 656c 636f 6d65 2063 6f6e 7472 6962   welcome contrib
+00000f20: 7574 696f 6e73 210a 0a54 6865 206d 6f73  utions!..The mos
+00000f30: 7420 636f 6d6d 6f6e 2073 7472 6174 6567  t common strateg
+00000f40: 7920 666f 7220 636f 6e74 7269 6275 7469  y for contributi
+00000f50: 6e67 2060 4869 7368 656c 6020 6170 7065  ng `Hishel` appe
+00000f60: 6172 7320 746f 2062 653a 0a0a 2d20 466f  ars to be:..- Fo
+00000f70: 726b 2074 6865 2070 726f 6a65 6374 0a2d  rk the project.-
+00000f80: 204d 616b 6520 6368 616e 6765 0a2d 204f   Make change.- O
+00000f90: 7065 6e20 7468 6520 7075 6c6c 2072 6571  pen the pull req
+00000fa0: 7565 7374                                uest
```

