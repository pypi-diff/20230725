# Comparing `tmp/sddp_discovery_protocol-1.0.0.tar.gz` & `tmp/sddp_discovery_protocol-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sddp_discovery_protocol-1.0.0.tar", max compression
+gzip compressed data, was "sddp_discovery_protocol-1.1.0.tar", max compression
```

## Comparing `sddp_discovery_protocol-1.0.0.tar` & `sddp_discovery_protocol-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1075 2023-07-24 16:07:34.987872 sddp_discovery_protocol-1.0.0/LICENSE
--rw-r--r--   0        0        0    10723 2023-07-24 16:07:34.987872 sddp_discovery_protocol-1.0.0/README.md
--rw-r--r--   0        0        0     1330 2023-07-24 16:07:34.987872 sddp_discovery_protocol-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1793 2023-07-24 16:07:34.987872 sddp_discovery_protocol-1.0.0/sddp_discovery_protocol/__init__.py
--rwxr-xr-x   0        0        0    11602 2023-07-24 16:07:34.987872 sddp_discovery_protocol-1.0.0/sddp_discovery_protocol/__main__.py
--rwxr-xr-x   0        0        0     9444 2023-07-24 16:07:34.987872 sddp_discovery_protocol-1.0.0/sddp_discovery_protocol/client.py
--rw-r--r--   0        0        0      319 2023-07-24 16:07:34.987872 sddp_discovery_protocol-1.0.0/sddp_discovery_protocol/constants.py
--rw-r--r--   0        0        0      253 2023-07-24 16:07:34.987872 sddp_discovery_protocol-1.0.0/sddp_discovery_protocol/exceptions.py
--rw-r--r--   0        0        0     1431 2023-07-24 16:07:34.987872 sddp_discovery_protocol-1.0.0/sddp_discovery_protocol/internal_types.py
--rwxr-xr-x   0        0        0      269 2023-07-24 16:07:34.987872 sddp_discovery_protocol-1.0.0/sddp_discovery_protocol/pkg_logging.py
--rw-r--r--   0        0        0        0 2023-07-24 16:07:34.987872 sddp_discovery_protocol-1.0.0/sddp_discovery_protocol/py.typed
--rwxr-xr-x   0        0        0    19088 2023-07-24 16:07:34.987872 sddp_discovery_protocol-1.0.0/sddp_discovery_protocol/sddp_datagram.py
--rwxr-xr-x   0        0        0    20245 2023-07-24 16:07:34.987872 sddp_discovery_protocol-1.0.0/sddp_discovery_protocol/sddp_socket.py
--rwxr-xr-x   0        0        0    17429 2023-07-24 16:07:34.987872 sddp_discovery_protocol-1.0.0/sddp_discovery_protocol/server.py
--rwxr-xr-x   0        0        0     8360 2023-07-24 16:07:34.987872 sddp_discovery_protocol-1.0.0/sddp_discovery_protocol/util.py
--rw-r--r--   0        0        0      454 2023-07-24 16:07:34.987872 sddp_discovery_protocol-1.0.0/sddp_discovery_protocol/version.py
--rw-r--r--   0        0        0    11716 1970-01-01 00:00:00.000000 sddp_discovery_protocol-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/LICENSE
+-rw-r--r--   0        0        0    13789 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/README.md
+-rw-r--r--   0        0        0     1330 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1812 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/__init__.py
+-rwxr-xr-x   0        0        0    12686 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/__main__.py
+-rwxr-xr-x   0        0        0    17332 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/client.py
+-rw-r--r--   0        0        0      319 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/constants.py
+-rw-r--r--   0        0        0      253 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/exceptions.py
+-rw-r--r--   0        0        0     1466 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/internal_types.py
+-rwxr-xr-x   0        0        0      269 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/pkg_logging.py
+-rw-r--r--   0        0        0        0 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/py.typed
+-rwxr-xr-x   0        0        0    19088 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/sddp_datagram.py
+-rwxr-xr-x   0        0        0    20519 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/sddp_socket.py
+-rwxr-xr-x   0        0        0    17429 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/server.py
+-rwxr-xr-x   0        0        0     8360 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/util.py
+-rw-r--r--   0        0        0      454 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/version.py
+-rw-r--r--   0        0        0    14782 1970-01-01 00:00:00.000000 sddp_discovery_protocol-1.1.0/PKG-INFO
```

### Comparing `sddp_discovery_protocol-1.0.0/LICENSE` & `sddp_discovery_protocol-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sddp_discovery_protocol-1.0.0/README.md` & `sddp_discovery_protocol-1.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -177,17 +177,17 @@
 
 
 #### Getting the package version
 ```bash
 $ sddp version
 0.1.0
 $
-``````
+```
 
-#### Discovering all devices on the local subnet
+#### Discovering devices on the local subnet
 
 ```bash
 $ sddp search --help
 usage: sddp search [-h] [--pattern PATTERN] [--wait-time WAIT_TIME] [-b BIND_ADDRESSES] [--include-error-responses]
 
 Search for SDDP devices
 
@@ -241,14 +241,42 @@
     "status": "OK",
     "status_code": 200,
     "utc_time": "2023-07-24T00:13:30.850138"
   }
 ]
 ```
 
+If you know the expected value of one or more response headers and are looking for a specific response, you
+can speed up the search in the successful case by applying a header filter and limiting the responses
+to 1; in this case the search will terminate as soon as the relevant response is received:
+
+```bash
+$ sddp search --max-responses 1 -F Type=JVCKENWOOD:Projector
+{
+  "headers": {
+    "Driver": "projector_JVCKENWOOD_DLA-RS3100_NZ8.c4i",
+    "From": "192.168.4.237:1902",
+    "Host": "JVC_PROJECTOR-E0DADC152802",
+    "Manufacturer": "JVCKENWOOD",
+    "Max-Age": 1800,
+    "Model": "DLA-RS3100_NZ8",
+    "Primary-Proxy": "projector",
+    "Proxies": "projector",
+    "Type": "JVCKENWOOD:Projector"
+  },
+  "local_addr": "192.168.4.198:58941",
+  "monotonic_time": 0.093766125,
+  "sddp_version": "1.0",
+  "src_addr": "192.168.4.237:1902",
+  "status": "OK",
+  "status_code": 200,
+  "utc_time": "2023-07-24T22:23:54.175783"
+}
+```
+
 #### Running an SDDP server
 ```bash
 $ sddp server --help
 usage: sddp server [-h] [--advertise-interval ADVERTISE_INTERVAL] [-H HEADERS] [-b BIND_ADDRESSES]
 
 Run an SDDP server
 
@@ -268,15 +296,75 @@
 $ sddp --log-level=debug server
 ...
 ```
 
 API
 ---
 
-TBD
+#### Discovering devices on the local subnet
+
+```python
+import logging
+import asyncio
+import sddp_discovery_protocol as sddp
+
+#logging.basicConfig(level=logging.DEBUG)
+
+async def amain():
+    # all parameters to SddpClient are optional; they allow you to set the IP addresses to bind to, etc.
+    async with sddp.SddpClient() as client:
+        # Entering the client.search() context manager sends the search multicast request and reliably collects responses.
+        # Parameters are optional; they allow you to set search filters, max wait time, max returned responses, etc.
+        async with client.search() as search_request:
+            # search_request.iter_responses() is an async generator that yields SddpResponseInfo objects
+            # as they come in until the max wait time has elapsed or the max number of responses has been received.
+            async for response_info in search_request.iter_responses():
+                print(response_info.datagram)
+                # It is possible to exit the loop early here if you found what you're looking for
+
+loop = asyncio.new_event_loop()
+try:
+    asyncio.set_event_loop(loop)
+    loop.run_until_complete(amain())
+finally:
+    loop.close()
+```
+
+#### Running an SDDP server
+
+```python
+import logging
+import asyncio
+import sddp_discovery_protocol as sddp
+
+logging.basicConfig(level=logging.DEBUG)
+
+device_headers = {
+    "Type": "Acme:TestDevice",
+    "Primary-Proxy": "test-device",
+    "Proxies": "test-device",
+    "Manufacturer": "Acme",
+    "Model": "TestDevPlus",
+    "Driver": "test-device_Acme_TestDevPlus.c4i",
+}
+
+async def amain():
+    # The SddpServerContext manager starts the server listening on the multicast port, sending out advertisements,
+    # and responding to search requests.  When the context manager exits, the server will be stopped.
+    async with sddp.SddpServer(device_headers=device_headers) as server:
+        # This will wait forever unless another task stops the server
+        await server.wait_for_done()        
+
+loop = asyncio.new_event_loop()
+try:
+    asyncio.set_event_loop(loop)
+    loop.run_until_complete(amain())
+finally:
+    loop.close()
+```
 
 Known issues and limitations
 ----------------------------
 
 * SDDP is a proprietary protocol defined by [Control4](https://www.control4.com/) with responders implemented by its
   smart-home business partners. The protocol is not standard and is not publicly documented. This
   package is a best effort to provide an open implementation of the protocol based on limited observation of
```

### Comparing `sddp_discovery_protocol-1.0.0/pyproject.toml` & `sddp_discovery_protocol-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sddp-discovery-protocol"
-version = "1.0.0"
+version = "1.1.0"
 description = "Implementation of Control4's Simple Device Discovery Protocol (SDDP)"
 authors = [ "Sam McKelvie <dev@mckelvie.org>" ]
 license = "MIT"
 keywords = [ "Control4", "SDDP", "SSDP", "UPnP", "protocol", "multicast", "UDP",
              "discovery", "network", "automation", "smart-home" ]
 readme = "README.md"
 homepage = "https://github.com/sammck/sddp-discovery-protocol"
```

### Comparing `sddp_discovery_protocol-1.0.0/sddp_discovery_protocol/__init__.py` & `sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from .internal_types import Jsonable, JsonableDict
 
 from .exceptions import SddpError
 
 from .sddp_datagram import SddpDatagram
 from .sddp_socket import SddpSocket, SddpSocketBinding, SddpDatagramSubscriber
 from .server import SddpServer, SddpAdvertisementInfo
-from .client import SddpClient, SddpResponseInfo, DEFAULT_RESPONSE_WAIT_TIME
+from .client import SddpClient, SddpSearchRequest, SddpResponseInfo, DEFAULT_RESPONSE_WAIT_TIME
 from .util import CaseInsensitiveDict
 from .constants import SDDP_MULTICAST_ADDRESS, SDDP_PORT
 
 __all__ = [
     '__version__',
     'Jsonable', 'JsonableDict',
     'SddpError',
```

### Comparing `sddp_discovery_protocol-1.0.0/sddp_discovery_protocol/__main__.py` & `sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 from sddp_discovery_protocol.internal_types import *
 
 from sddp_discovery_protocol import (
     __version__ as pkg_version,
     SddpServer,
     SddpClient,
+    SddpSearchRequest,
     SddpDatagramSubscriber,
     SddpDatagram,
     SddpSocketBinding,
     CaseInsensitiveDict,
     SddpAdvertisementInfo,
     DEFAULT_RESPONSE_WAIT_TIME,
   )
@@ -56,14 +57,24 @@
 
     def __init__(self, argv: Optional[Sequence[str]]=None):
         self._argv = argv
 
     async def cmd_bare(self) -> int:
         print("A command is required", file=sys.stderr)
         return 1
+    
+    def _parse_arg_headers(self, arg_headers: List[str]) -> CaseInsensitiveDict:
+        headers = CaseInsensitiveDict()
+        for header_assignment in arg_headers:
+            name, value = header_assignment.split('=', 1)
+            if name.lower() in [x.lower() for x in integer_sddp_headers]:
+                value = int(value)
+            headers[name] = value
+        return headers
+        
 
     async def cmd_server(self) -> int:
         async def notify_handler(info: SddpAdvertisementInfo) -> None:
             results: List[JsonableDict] = []
             datagram = info.datagram
             header_dict: Dict[str, str] = dict(datagram.headers)
             summary: JsonableDict = {
@@ -76,21 +87,15 @@
             }
             if datagram.body is not None and len(datagram.body) > 0:
                 summary["body"] = base64.b64encode(datagram.body).decode('ascii')
 
             print(json.dumps(summary, indent=2, sort_keys=True))
 
         advertise_interval: float = self._args.advertise_interval
-        headers = CaseInsensitiveDict()
-        arg_headers: List[str] = self._args.headers
-        for header_assignment in arg_headers:
-            name, value = header_assignment.split('=', 1)
-            if name.lower() in [x.lower() for x in integer_sddp_headers]:
-                value = int(value)
-            headers[name] = value
+        headers = self._parse_arg_headers(self._args.headers)
         bind_addresses: Optional[List[str]] = self._args.bind_addresses
         if not bind_addresses is None and len(bind_addresses) == 0:
             bind_addresses = None
         server = SddpServer(advertise_interval=advertise_interval, device_headers=headers, bind_addresses=bind_addresses)
         server.add_notify_handler(notify_handler)
         if not self._provide_traceback:
             async def sigint_cleanup() -> None:
@@ -120,40 +125,45 @@
                     pass
         return 0
 
     async def cmd_search(self) -> int:
         response_wait_time: float = self._args.wait_time
         search_pattern: str = self._args.pattern
         include_error_responses: bool = self._args.include_error_responses
+        max_responses: int = self._args.max_responses
         bind_addresses: Optional[List[str]] = self._args.bind_addresses
         if not bind_addresses is None and len(bind_addresses) == 0:
             bind_addresses = None
+        filter_headers = self._parse_arg_headers(self._args.filter_headers)
         async with SddpClient(response_wait_time=response_wait_time, bind_addresses=bind_addresses) as client:
-            responses = await client.search(search_pattern=search_pattern, include_error_responses=include_error_responses)
-
-        results: List[JsonableDict] = []
-
-        for info in responses:
-            datagram = info.datagram
-            header_dict: Dict[str, str] = dict(datagram.headers)
-            summary: JsonableDict = {
-                "sddp_version": info.sddp_version,
-                "status_code": info.status_code,
-                "status": info.status,
-                "src_addr": f"{info.src_addr[0]}:{info.src_addr[1]}",
-                "local_addr": f"{info.socket_binding.unicast_addr[0]}:{info.socket_binding.unicast_addr[1]}",
-                "headers": header_dict,
-                "monotonic_time": info.monotonic_time,
-                "utc_time": info.utc_time.isoformat(),
-            }
-            if datagram.body is not None and len(datagram.body) > 0:
-                summary["body"] = base64.b64encode(datagram.body).decode('ascii')
-            results.append(summary)
-
-        print(json.dumps(results, indent=2, sort_keys=True))
+            async with SddpSearchRequest(
+                    client,
+                    search_pattern=search_pattern,
+                    response_wait_time=response_wait_time,
+                    max_responses=max_responses,
+                    include_error_responses=include_error_responses,
+                    filter_headers=filter_headers,
+                ) as search_request:
+                async for info in search_request.iter_responses():
+                    datagram = info.datagram
+                    header_dict: Dict[str, str] = dict(datagram.headers)
+                    summary: JsonableDict = {
+                        "sddp_version": info.sddp_version,
+                        "status_code": info.status_code,
+                        "status": info.status,
+                        "src_addr": f"{info.src_addr[0]}:{info.src_addr[1]}",
+                        "local_addr": f"{info.socket_binding.unicast_addr[0]}:{info.socket_binding.unicast_addr[1]}",
+                        "headers": header_dict,
+                        "monotonic_time": info.monotonic_time,
+                        "utc_time": info.utc_time.isoformat(),
+                    }
+                    if datagram.body is not None and len(datagram.body) > 0:
+                        summary["body"] = base64.b64encode(datagram.body).decode('ascii')
+                    print(json.dumps(summary, indent=2, sort_keys=True))
+                    sys.stdout.flush()
 
         return 0
 
     async def cmd_version(self) -> int:
         print(pkg_version)
         return 0
 
@@ -207,14 +217,18 @@
                             help='''The device pattern to search for. Default: "*"''')
         parser_search.add_argument('--wait-time', type=float, default=DEFAULT_RESPONSE_WAIT_TIME,
                             help=f'''The amount of time to wait for responses, in seconds. Default: {DEFAULT_RESPONSE_WAIT_TIME}''')
         parser_search.add_argument('-b', '--bind', dest="bind_addresses", action='append', default=[],
                             help='''The local unicast IP address to bind to. May be repeated. Default: all local non-loopback unicast addresses.''')
         parser_search.add_argument('--include-error-responses', dest="include_error_responses", action='store_true', default=False,
                             help='Include error responses in the output. Default: False')
+        parser_search.add_argument('--max-responses', type=int, default=0,
+                            help='The maximum number of responses to return. Default: 0 (no limit)')
+        parser_search.add_argument('-F', '--filter', dest="filter_headers", action='append', default=[],
+                            help='''A <name>=<value> header that must match a response for the response to be included. May be repeated.''')
         parser_search.set_defaults(func=self.cmd_search)
 
         # ======================= version
 
         parser_version = subparsers.add_parser('version',
                                 description='''Display version information.''')
         parser_version.set_defaults(func=self.cmd_version)
```

### Comparing `sddp_discovery_protocol-1.0.0/sddp_discovery_protocol/internal_types.py` & `sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/internal_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,17 +28,20 @@
     Coroutine,
     Generator,
     Iterable,
     Iterable,
     Mapping,
     MutableMapping,
     Sequence,
-    AsyncIterator
+    AsyncIterator,
   )
 
+from types import TracebackType
+
+
 from typing_extensions import Self
 
 JsonableTypes = ( str, int, float, bool, dict, list )
 # A tuple of types to use for isinstance checking of JSON-serializable types. Excludes None. Useful for isinstance.
 
 if TYPE_CHECKING:
   Jsonable = Union[str, int, float, bool, None, Dict[str, Any], List[Any]]
```

### Comparing `sddp_discovery_protocol-1.0.0/sddp_discovery_protocol/sddp_datagram.py` & `sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/sddp_datagram.py`

 * *Files identical despite different names*

### Comparing `sddp_discovery_protocol-1.0.0/sddp_discovery_protocol/sddp_socket.py` & `sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/sddp_socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,15 +204,20 @@
         self.queue = asyncio.Queue(max_queue_size)
         self.final_result = Future()
 
     async def __aenter__(self) -> SddpDatagramSubscriber:
         await self.sddp_socket.add_subscriber(self)
         return self
 
-    async def __aexit__(self, exc_type, exc, tb) -> bool:
+    async def __aexit__(
+            self,
+            exc_type: Optional[type[BaseException]],
+            exc: Optional[BaseException],
+            tb: Optional[TracebackType]
+      ) -> bool:
         await self.sddp_socket.remove_subscriber(self)
         self.set_final_result()
         try:
             # ensure that final_result has been awaited
             await self.final_result
         except BaseException as e:
             pass
@@ -489,15 +494,20 @@
             self._close_all_transports()
             self._close_all_socks()
 
     async def __aenter__(self) -> Self:
         await self.start()
         return self
 
-    async def __aexit__(self, exc_type, exc, tb) -> bool:
+    async def __aexit__(
+            self,
+            exc_type: Optional[type[BaseException]],
+            exc: Optional[BaseException],
+            tb: Optional[TracebackType]
+      ) -> bool:
         if exc is None:
             self.set_final_result()
         else:
             self.set_final_exception(exc)
         try:
             # ensure that final_result has been awaited
             await self.wait_for_done()
```

### Comparing `sddp_discovery_protocol-1.0.0/sddp_discovery_protocol/server.py` & `sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/server.py`

 * *Files identical despite different names*

### Comparing `sddp_discovery_protocol-1.0.0/sddp_discovery_protocol/util.py` & `sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/util.py`

 * *Files identical despite different names*

### Comparing `sddp_discovery_protocol-1.0.0/PKG-INFO` & `sddp_discovery_protocol-1.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sddp-discovery-protocol
-Version: 1.0.0
+Version: 1.1.0
 Summary: Implementation of Control4's Simple Device Discovery Protocol (SDDP)
 Home-page: https://github.com/sammck/sddp-discovery-protocol
 License: MIT
 Keywords: Control4,SDDP,SSDP,UPnP,protocol,multicast,UDP,discovery,network,automation,smart-home
 Author: Sam McKelvie
 Author-email: dev@mckelvie.org
 Requires-Python: >=3.8,<4.0
@@ -200,17 +200,17 @@
 
 
 #### Getting the package version
 ```bash
 $ sddp version
 0.1.0
 $
-``````
+```
 
-#### Discovering all devices on the local subnet
+#### Discovering devices on the local subnet
 
 ```bash
 $ sddp search --help
 usage: sddp search [-h] [--pattern PATTERN] [--wait-time WAIT_TIME] [-b BIND_ADDRESSES] [--include-error-responses]
 
 Search for SDDP devices
 
@@ -264,14 +264,42 @@
     "status": "OK",
     "status_code": 200,
     "utc_time": "2023-07-24T00:13:30.850138"
   }
 ]
 ```
 
+If you know the expected value of one or more response headers and are looking for a specific response, you
+can speed up the search in the successful case by applying a header filter and limiting the responses
+to 1; in this case the search will terminate as soon as the relevant response is received:
+
+```bash
+$ sddp search --max-responses 1 -F Type=JVCKENWOOD:Projector
+{
+  "headers": {
+    "Driver": "projector_JVCKENWOOD_DLA-RS3100_NZ8.c4i",
+    "From": "192.168.4.237:1902",
+    "Host": "JVC_PROJECTOR-E0DADC152802",
+    "Manufacturer": "JVCKENWOOD",
+    "Max-Age": 1800,
+    "Model": "DLA-RS3100_NZ8",
+    "Primary-Proxy": "projector",
+    "Proxies": "projector",
+    "Type": "JVCKENWOOD:Projector"
+  },
+  "local_addr": "192.168.4.198:58941",
+  "monotonic_time": 0.093766125,
+  "sddp_version": "1.0",
+  "src_addr": "192.168.4.237:1902",
+  "status": "OK",
+  "status_code": 200,
+  "utc_time": "2023-07-24T22:23:54.175783"
+}
+```
+
 #### Running an SDDP server
 ```bash
 $ sddp server --help
 usage: sddp server [-h] [--advertise-interval ADVERTISE_INTERVAL] [-H HEADERS] [-b BIND_ADDRESSES]
 
 Run an SDDP server
 
@@ -291,15 +319,75 @@
 $ sddp --log-level=debug server
 ...
 ```
 
 API
 ---
 
-TBD
+#### Discovering devices on the local subnet
+
+```python
+import logging
+import asyncio
+import sddp_discovery_protocol as sddp
+
+#logging.basicConfig(level=logging.DEBUG)
+
+async def amain():
+    # all parameters to SddpClient are optional; they allow you to set the IP addresses to bind to, etc.
+    async with sddp.SddpClient() as client:
+        # Entering the client.search() context manager sends the search multicast request and reliably collects responses.
+        # Parameters are optional; they allow you to set search filters, max wait time, max returned responses, etc.
+        async with client.search() as search_request:
+            # search_request.iter_responses() is an async generator that yields SddpResponseInfo objects
+            # as they come in until the max wait time has elapsed or the max number of responses has been received.
+            async for response_info in search_request.iter_responses():
+                print(response_info.datagram)
+                # It is possible to exit the loop early here if you found what you're looking for
+
+loop = asyncio.new_event_loop()
+try:
+    asyncio.set_event_loop(loop)
+    loop.run_until_complete(amain())
+finally:
+    loop.close()
+```
+
+#### Running an SDDP server
+
+```python
+import logging
+import asyncio
+import sddp_discovery_protocol as sddp
+
+logging.basicConfig(level=logging.DEBUG)
+
+device_headers = {
+    "Type": "Acme:TestDevice",
+    "Primary-Proxy": "test-device",
+    "Proxies": "test-device",
+    "Manufacturer": "Acme",
+    "Model": "TestDevPlus",
+    "Driver": "test-device_Acme_TestDevPlus.c4i",
+}
+
+async def amain():
+    # The SddpServerContext manager starts the server listening on the multicast port, sending out advertisements,
+    # and responding to search requests.  When the context manager exits, the server will be stopped.
+    async with sddp.SddpServer(device_headers=device_headers) as server:
+        # This will wait forever unless another task stops the server
+        await server.wait_for_done()        
+
+loop = asyncio.new_event_loop()
+try:
+    asyncio.set_event_loop(loop)
+    loop.run_until_complete(amain())
+finally:
+    loop.close()
+```
 
 Known issues and limitations
 ----------------------------
 
 * SDDP is a proprietary protocol defined by [Control4](https://www.control4.com/) with responders implemented by its
   smart-home business partners. The protocol is not standard and is not publicly documented. This
   package is a best effort to provide an open implementation of the protocol based on limited observation of
```

