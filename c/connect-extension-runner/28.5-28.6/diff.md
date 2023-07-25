# Comparing `tmp/connect_extension_runner-28.5.tar.gz` & `tmp/connect_extension_runner-28.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connect_extension_runner-28.5.tar", max compression
+gzip compressed data, was "connect_extension_runner-28.6.tar", max compression
```

## Comparing `connect_extension_runner-28.5.tar` & `connect_extension_runner-28.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    11357 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/LICENSE
--rw-r--r--   0        0        0     1422 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/README.md
--rw-r--r--   0        0        0       55 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/dataclasses.py
--rw-r--r--   0        0        0      405 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/extension.py
--rw-r--r--   0        0        0      143 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/artworks/__init__.py
--rw-r--r--   0        0        0     9409 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/artworks/ansi_regular.flf
--rw-r--r--   0        0        0      950 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/artworks/banner.py
--rw-r--r--   0        0        0    11425 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/artworks/bloody.flf
--rw-r--r--   0        0        0     6483 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/config.py
--rw-r--r--   0        0        0     5708 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/constants.py
--rw-r--r--   0        0        0      320 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/handlers/__init__.py
--rw-r--r--   0        0        0     2692 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/handlers/anvil.py
--rw-r--r--   0        0        0     4391 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/handlers/base.py
--rw-r--r--   0        0        0     3751 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/handlers/events.py
--rw-r--r--   0        0        0     2444 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/handlers/transformations.py
--rw-r--r--   0        0        0     7133 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/handlers/web.py
--rw-r--r--   0        0        0    18982 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/helpers.py
--rw-r--r--   0        0        0     1989 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/main.py
--rw-r--r--   0        0        0      340 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/managers/__init__.py
--rw-r--r--   0        0        0     3190 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/managers/background.py
--rw-r--r--   0        0        0     8100 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/managers/base.py
--rw-r--r--   0        0        0     2225 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/managers/interactive.py
--rw-r--r--   0        0        0     1931 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/managers/scheduled.py
--rw-r--r--   0        0        0    20665 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/managers/transformation.py
--rw-r--r--   0        0        0      533 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/managers/utils.py
--rw-r--r--   0        0        0     7917 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/master.py
--rw-r--r--   0        0        0        0 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/workers/__init__.py
--rw-r--r--   0        0        0     2549 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/workers/anvil.py
--rw-r--r--   0        0        0    11320 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/workers/base.py
--rw-r--r--   0        0        0     8834 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/workers/events.py
--rw-r--r--   0        0        0     6545 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/workers/transformations.py
--rw-r--r--   0        0        0     7038 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/workers/web.py
--rw-r--r--   0        0        0     2870 2023-07-12 11:07:21.439286 connect_extension_runner-28.5/pyproject.toml
--rw-r--r--   0        0        0     2909 1970-01-01 00:00:00.000000 connect_extension_runner-28.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-25 10:26:32.627653 connect_extension_runner-28.6/LICENSE
+-rw-r--r--   0        0        0     1422 2023-07-25 10:26:32.627653 connect_extension_runner-28.6/README.md
+-rw-r--r--   0        0        0       55 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/dataclasses.py
+-rw-r--r--   0        0        0      405 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/extension.py
+-rw-r--r--   0        0        0      143 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/runner/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/runner/artworks/__init__.py
+-rw-r--r--   0        0        0     9409 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/runner/artworks/ansi_regular.flf
+-rw-r--r--   0        0        0      950 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/runner/artworks/banner.py
+-rw-r--r--   0        0        0    11425 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/runner/artworks/bloody.flf
+-rw-r--r--   0        0        0     6764 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/runner/config.py
+-rw-r--r--   0        0        0     5708 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/runner/constants.py
+-rw-r--r--   0        0        0      320 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/runner/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/runner/handlers/__init__.py
+-rw-r--r--   0        0        0     2692 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/runner/handlers/anvil.py
+-rw-r--r--   0        0        0     4391 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/runner/handlers/base.py
+-rw-r--r--   0        0        0     3751 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/runner/handlers/events.py
+-rw-r--r--   0        0        0     2444 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/runner/handlers/transformations.py
+-rw-r--r--   0        0        0     7133 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/runner/handlers/web.py
+-rw-r--r--   0        0        0    19074 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/runner/helpers.py
+-rw-r--r--   0        0        0     1989 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/runner/main.py
+-rw-r--r--   0        0        0      340 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/runner/managers/__init__.py
+-rw-r--r--   0        0        0     3190 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/runner/managers/background.py
+-rw-r--r--   0        0        0     8100 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/runner/managers/base.py
+-rw-r--r--   0        0        0     2225 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/runner/managers/interactive.py
+-rw-r--r--   0        0        0     1931 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/runner/managers/scheduled.py
+-rw-r--r--   0        0        0    20665 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/runner/managers/transformation.py
+-rw-r--r--   0        0        0      533 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/runner/managers/utils.py
+-rw-r--r--   0        0        0     7917 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/runner/master.py
+-rw-r--r--   0        0        0        0 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/runner/workers/__init__.py
+-rw-r--r--   0        0        0     2549 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/runner/workers/anvil.py
+-rw-r--r--   0        0        0    11824 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/runner/workers/base.py
+-rw-r--r--   0        0        0     8834 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/runner/workers/events.py
+-rw-r--r--   0        0        0     6545 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/runner/workers/transformations.py
+-rw-r--r--   0        0        0     7038 2023-07-25 10:26:32.631653 connect_extension_runner-28.6/connect/eaas/runner/workers/web.py
+-rw-r--r--   0        0        0     2928 2023-07-25 10:28:02.772670 connect_extension_runner-28.6/pyproject.toml
+-rw-r--r--   0        0        0     2963 1970-01-01 00:00:00.000000 connect_extension_runner-28.6/PKG-INFO
```

### Comparing `connect_extension_runner-28.5/LICENSE` & `connect_extension_runner-28.6/LICENSE`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.5/README.md` & `connect_extension_runner-28.6/README.md`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.5/connect/eaas/runner/artworks/ansi_regular.flf` & `connect_extension_runner-28.6/connect/eaas/runner/artworks/ansi_regular.flf`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.5/connect/eaas/runner/artworks/banner.py` & `connect_extension_runner-28.6/connect/eaas/runner/artworks/banner.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.5/connect/eaas/runner/artworks/bloody.flf` & `connect_extension_runner-28.6/connect/eaas/runner/artworks/bloody.flf`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.5/connect/eaas/runner/config.py` & `connect_extension_runner-28.6/connect/eaas/runner/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -95,14 +95,26 @@
     @property
     def event_definitions(self):
         return {
             definition.event_type: definition
             for definition in (self.dyn_config.event_definitions or [])
         }
 
+    @property
+    def proxy(self):
+        return self.env.get('wss_proxy') if self.secure else self.env.get('ws_proxy')
+
+    @property
+    def ws_address(self):
+        return self.env["ws_address"]
+
+    @property
+    def ws_port(self):
+        return 443 if self.secure else 80
+
     def get_events_ws_url(self):
         proto = 'wss' if self.secure else 'ws'
         return (
             f'{proto}://{self.env["ws_address"]}/public/v1/devops/ws'
             f'/{self.env["environment_id"]}/{self.env["instance_id"]}'
         )
```

### Comparing `connect_extension_runner-28.5/connect/eaas/runner/constants.py` & `connect_extension_runner-28.6/connect/eaas/runner/constants.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.5/connect/eaas/runner/handlers/anvil.py` & `connect_extension_runner-28.6/connect/eaas/runner/handlers/anvil.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.5/connect/eaas/runner/handlers/base.py` & `connect_extension_runner-28.6/connect/eaas/runner/handlers/base.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.5/connect/eaas/runner/handlers/events.py` & `connect_extension_runner-28.6/connect/eaas/runner/handlers/events.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.5/connect/eaas/runner/handlers/transformations.py` & `connect_extension_runner-28.6/connect/eaas/runner/handlers/transformations.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.5/connect/eaas/runner/handlers/web.py` & `connect_extension_runner-28.6/connect/eaas/runner/handlers/web.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.5/connect/eaas/runner/helpers.py` & `connect_extension_runner-28.6/connect/eaas/runner/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,14 +100,16 @@
 def get_environment():
     return {
         'api_key': os.getenv('API_KEY'),
         'environment_id': os.getenv('ENVIRONMENT_ID'),
         'instance_id': os.getenv('INSTANCE_ID', get_container_id()),
         'ws_address': os.getenv('SERVER_ADDRESS', 'api.cnct.info'),
         'api_address': os.getenv('API_ADDRESS', os.getenv('SERVER_ADDRESS', 'api.cnct.info')),
+        'ws_proxy': os.getenv('HTTP_PROXY'),
+        'wss_proxy': os.getenv('HTTPS_PROXY'),
         'background_task_max_execution_time': int(os.getenv(
             'BACKGROUND_TASK_MAX_EXECUTION_TIME', BACKGROUND_TASK_MAX_EXECUTION_TIME,
         )),
         'interactive_task_max_execution_time': int(os.getenv(
             'INTERACTIVE_TASK_MAX_EXECUTION_TIME', INTERACTIVE_TASK_MAX_EXECUTION_TIME,
         )),
         'scheduled_task_max_execution_time': int(os.getenv(
```

### Comparing `connect_extension_runner-28.5/connect/eaas/runner/main.py` & `connect_extension_runner-28.6/connect/eaas/runner/main.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.5/connect/eaas/runner/managers/background.py` & `connect_extension_runner-28.6/connect/eaas/runner/managers/background.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.5/connect/eaas/runner/managers/base.py` & `connect_extension_runner-28.6/connect/eaas/runner/managers/base.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.5/connect/eaas/runner/managers/interactive.py` & `connect_extension_runner-28.6/connect/eaas/runner/managers/interactive.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.5/connect/eaas/runner/managers/scheduled.py` & `connect_extension_runner-28.6/connect/eaas/runner/managers/scheduled.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.5/connect/eaas/runner/managers/transformation.py` & `connect_extension_runner-28.6/connect/eaas/runner/managers/transformation.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.5/connect/eaas/runner/managers/utils.py` & `connect_extension_runner-28.6/connect/eaas/runner/managers/utils.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.5/connect/eaas/runner/master.py` & `connect_extension_runner-28.6/connect/eaas/runner/master.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.5/connect/eaas/runner/workers/anvil.py` & `connect_extension_runner-28.6/connect/eaas/runner/workers/anvil.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.5/connect/eaas/runner/workers/base.py` & `connect_extension_runner-28.6/connect/eaas/runner/workers/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 )
 
 import backoff
 import websockets
 from devtools import (
     pformat,
 )
+from python_socks.async_.asyncio import (
+    Proxy,
+)
 from websockets.exceptions import (
     ConnectionClosedError,
     ConnectionClosedOK,
     InvalidStatusCode,
 )
 
 from connect.eaas.core.proto import (
@@ -110,14 +113,15 @@
                         url = self.get_url()
                         self.ws = await websockets.connect(
                             url,
                             extra_headers=self.config.get_headers(),
                             ping_interval=60,
                             ping_timeout=60,
                             max_queue=128,
+                            **await self.get_proxy_config(),
                         )
                         await (await self.ws.ping())
                         await self.do_handshake()
                         logger.info(f'{self} connected to {url}')
                     except InvalidStatusCode as ic:
                         if ic.status_code == 502:
                             logger.warning(f'{self}: maintenance in progress...')
@@ -135,14 +139,27 @@
                         raise CommunicationError()
                     except Exception as e:
                         logger.exception(f'{self}: received an unexpected exception: {e}...')
                         raise CommunicationError()
 
         await _connect()
 
+    async def get_proxy_config(self):
+        if not self.config.proxy:
+            return {}
+        proxy = Proxy.from_url(self.config.proxy)
+        sock = await proxy.connect(
+            dest_host=self.config.ws_address,
+            dest_port=self.config.ws_port,
+        )
+        return {
+            'sock': sock,
+            'server_hostname': self.config.ws_address,
+        }
+
     async def do_handshake(self):
         setup_request = self.get_setup_request()
         await self.send(setup_request)
         message = await asyncio.wait_for(self.ws.recv(), timeout=5)
         await self.process_message(json.loads(message))
 
     async def send(self, message):
```

### Comparing `connect_extension_runner-28.5/connect/eaas/runner/workers/events.py` & `connect_extension_runner-28.6/connect/eaas/runner/workers/events.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.5/connect/eaas/runner/workers/transformations.py` & `connect_extension_runner-28.6/connect/eaas/runner/workers/transformations.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.5/connect/eaas/runner/workers/web.py` & `connect_extension_runner-28.6/connect/eaas/runner/workers/web.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.5/pyproject.toml` & `connect_extension_runner-28.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "connect-extension-runner"
-version = "28.5"
+version = "28.6"
 description = "CloudBlue Connect EaaS Extension Runner"
 authors = ["CloudBlue LLC"]
 license = "Apache-2.0"
 packages = [
     { include = "connect" },
 ]
 readme = "./README.md"
@@ -37,14 +37,15 @@
 pyfiglet = "^0.8.post1"
 devtools = "^0.10.0"
 watchfiles = "^0.19.0"
 openpyxl = ">=3.0.0,<4"
 lxml = "^4.9.2"
 uvloop = "^0.17.0"
 urllib3 = "<2"
+python-socks = {extras = ["asyncio"], version = "^2.3.0"}
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.3.1"
 pytest-randomly = "^3.12.0"
 coverage = {extras = ["toml"], version = "^5.3"}
```

### Comparing `connect_extension_runner-28.5/PKG-INFO` & `connect_extension_runner-28.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connect-extension-runner
-Version: 28.5
+Version: 28.6
 Summary: CloudBlue Connect EaaS Extension Runner
 Home-page: https://connect.cloudblue.com
 License: Apache-2.0
 Author: CloudBlue LLC
 Requires-Python: >=3.8,<4
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -23,14 +23,15 @@
 Requires-Dist: connect-openapi-client (>=25.16)
 Requires-Dist: devtools (>=0.10.0,<0.11.0)
 Requires-Dist: httpx (>=0.23,<0.25)
 Requires-Dist: logzio-python-handler (>=3.1.1,<4.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: openpyxl (>=3.0.0,<4)
 Requires-Dist: pyfiglet (>=0.8.post1,<0.9)
+Requires-Dist: python-socks[asyncio] (>=2.3.0,<3.0.0)
 Requires-Dist: rich (>=12)
 Requires-Dist: urllib3 (<2)
 Requires-Dist: uvloop (>=0.17.0,<0.18.0)
 Requires-Dist: watchfiles (>=0.19.0,<0.20.0)
 Requires-Dist: websockets (==10.*)
 Project-URL: Repository, https://github.com/cloudblue/connect-extension-runner
 Description-Content-Type: text/markdown
```

