# Comparing `tmp/libservice-0.1.8.tar.gz` & `tmp/libservice-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libservice-0.1.8.tar", last modified: Fri Apr 21 09:48:35 2023, max compression
+gzip compressed data, was "libservice-0.1.9.tar", last modified: Fri Apr 21 10:45:35 2023, max compression
```

## Comparing `libservice-0.1.8.tar` & `libservice-0.1.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-21 09:48:35.756358 libservice-0.1.8/
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-21 09:48:35.752358 libservice-0.1.8/.github/
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-21 09:48:35.756358 libservice-0.1.8/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 joente    (1000) joente    (1000)      535 2022-02-17 12:20:07.000000 libservice-0.1.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 joente    (1000) joente    (1000)      595 2022-02-17 12:20:07.000000 libservice-0.1.8/.github/ISSUE_TEMPLATE/feature_request.md
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-21 09:48:35.756358 libservice-0.1.8/.github/workflows/
--rw-rw-r--   0 joente    (1000) joente    (1000)      685 2022-11-30 08:37:20.000000 libservice-0.1.8/.github/workflows/ci.yml
--rw-rw-r--   0 joente    (1000) joente    (1000)     1799 2022-02-17 09:45:16.000000 libservice-0.1.8/.gitignore
--rw-rw-r--   0 joente    (1000) joente    (1000)    35149 2022-07-05 11:43:02.000000 libservice-0.1.8/LICENSE
--rw-rw-r--   0 joente    (1000) joente    (1000)     4440 2023-04-21 09:48:35.756358 libservice-0.1.8/PKG-INFO
--rw-rw-r--   0 joente    (1000) joente    (1000)     3543 2023-04-20 08:27:55.000000 libservice-0.1.8/README.md
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-21 09:48:35.756358 libservice-0.1.8/libservice/
--rw-rw-r--   0 joente    (1000) joente    (1000)      134 2023-02-20 10:29:20.000000 libservice-0.1.8/libservice/__init__.py
--rw-rw-r--   0 joente    (1000) joente    (1000)      919 2023-04-20 18:05:54.000000 libservice-0.1.8/libservice/asset.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     1125 2023-02-17 14:23:33.000000 libservice-0.1.8/libservice/check.py
--rw-rw-r--   0 joente    (1000) joente    (1000)      849 2023-04-21 09:47:05.000000 libservice-0.1.8/libservice/exceptions.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-21 09:48:35.756358 libservice-0.1.8/libservice/hub/
--rw-rw-r--   0 joente    (1000) joente    (1000)       50 2022-11-25 07:18:03.000000 libservice-0.1.8/libservice/hub/__init__.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     4459 2023-02-20 09:45:11.000000 libservice-0.1.8/libservice/hub/client.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-21 09:48:35.756358 libservice-0.1.8/libservice/hub/net/
--rw-rw-r--   0 joente    (1000) joente    (1000)        0 2022-10-18 13:35:23.000000 libservice-0.1.8/libservice/hub/net/__init__.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     2205 2022-12-27 19:39:41.000000 libservice-0.1.8/libservice/hub/net/package.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     3128 2022-10-18 13:35:23.000000 libservice-0.1.8/libservice/hub/net/protocol.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     1214 2023-02-20 09:46:36.000000 libservice-0.1.8/libservice/hub/protocol.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     1666 2023-02-17 16:03:47.000000 libservice-0.1.8/libservice/logger.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     7659 2023-04-21 09:44:25.000000 libservice-0.1.8/libservice/serviceroom.py
--rw-rw-r--   0 joente    (1000) joente    (1000)       86 2023-02-17 12:31:27.000000 libservice-0.1.8/libservice/severity.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     2666 2023-02-20 13:20:33.000000 libservice-0.1.8/libservice/start.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-21 09:48:35.756358 libservice-0.1.8/libservice/ticonn/
--rw-rw-r--   0 joente    (1000) joente    (1000)       27 2022-10-21 06:25:36.000000 libservice-0.1.8/libservice/ticonn/__init__.py
--rw-rw-r--   0 joente    (1000) joente    (1000)       55 2022-10-21 06:25:36.000000 libservice-0.1.8/libservice/ticonn/ticonn.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-21 09:48:35.756358 libservice-0.1.8/libservice.egg-info/
--rw-rw-r--   0 joente    (1000) joente    (1000)     4440 2023-04-21 09:48:35.000000 libservice-0.1.8/libservice.egg-info/PKG-INFO
--rw-rw-r--   0 joente    (1000) joente    (1000)      745 2023-04-21 09:48:35.000000 libservice-0.1.8/libservice.egg-info/SOURCES.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)        1 2023-04-21 09:48:35.000000 libservice-0.1.8/libservice.egg-info/dependency_links.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       46 2023-04-21 09:48:35.000000 libservice-0.1.8/libservice.egg-info/requires.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       11 2023-04-21 09:48:35.000000 libservice-0.1.8/libservice.egg-info/top_level.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       75 2023-04-20 08:15:18.000000 libservice-0.1.8/requirements.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       38 2023-04-21 09:48:35.756358 libservice-0.1.8/setup.cfg
--rw-rw-r--   0 joente    (1000) joente    (1000)     1555 2023-02-20 09:28:37.000000 libservice-0.1.8/setup.py
--rw-rw-r--   0 joente    (1000) joente    (1000)       22 2023-04-21 09:45:06.000000 libservice-0.1.8/version.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-21 10:45:35.501492 libservice-0.1.9/
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-21 10:45:35.497492 libservice-0.1.9/.github/
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-21 10:45:35.497492 libservice-0.1.9/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 joente    (1000) joente    (1000)      535 2022-02-17 12:20:07.000000 libservice-0.1.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 joente    (1000) joente    (1000)      595 2022-02-17 12:20:07.000000 libservice-0.1.9/.github/ISSUE_TEMPLATE/feature_request.md
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-21 10:45:35.497492 libservice-0.1.9/.github/workflows/
+-rw-rw-r--   0 joente    (1000) joente    (1000)      685 2022-11-30 08:37:20.000000 libservice-0.1.9/.github/workflows/ci.yml
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1799 2022-02-17 09:45:16.000000 libservice-0.1.9/.gitignore
+-rw-rw-r--   0 joente    (1000) joente    (1000)    35149 2022-07-05 11:43:02.000000 libservice-0.1.9/LICENSE
+-rw-rw-r--   0 joente    (1000) joente    (1000)     4440 2023-04-21 10:45:35.501492 libservice-0.1.9/PKG-INFO
+-rw-rw-r--   0 joente    (1000) joente    (1000)     3543 2023-04-20 08:27:55.000000 libservice-0.1.9/README.md
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-21 10:45:35.501492 libservice-0.1.9/libservice/
+-rw-rw-r--   0 joente    (1000) joente    (1000)      152 2023-04-21 09:53:01.000000 libservice-0.1.9/libservice/__init__.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)      995 2023-04-21 10:39:57.000000 libservice-0.1.9/libservice/asset.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1125 2023-04-21 10:39:19.000000 libservice-0.1.9/libservice/check.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)      849 2023-04-21 09:47:05.000000 libservice-0.1.9/libservice/exceptions.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-21 10:45:35.501492 libservice-0.1.9/libservice/hub/
+-rw-rw-r--   0 joente    (1000) joente    (1000)       50 2022-11-25 07:18:03.000000 libservice-0.1.9/libservice/hub/__init__.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     4459 2023-02-20 09:45:11.000000 libservice-0.1.9/libservice/hub/client.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-21 10:45:35.501492 libservice-0.1.9/libservice/hub/net/
+-rw-rw-r--   0 joente    (1000) joente    (1000)        0 2022-10-18 13:35:23.000000 libservice-0.1.9/libservice/hub/net/__init__.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     2205 2022-12-27 19:39:41.000000 libservice-0.1.9/libservice/hub/net/package.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     3128 2022-10-18 13:35:23.000000 libservice-0.1.9/libservice/hub/net/protocol.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1214 2023-02-20 09:46:36.000000 libservice-0.1.9/libservice/hub/protocol.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1666 2023-02-17 16:03:47.000000 libservice-0.1.9/libservice/logger.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     8211 2023-04-21 10:41:48.000000 libservice-0.1.9/libservice/serviceroom.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)       86 2023-02-17 12:31:27.000000 libservice-0.1.9/libservice/severity.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     2666 2023-02-20 13:20:33.000000 libservice-0.1.9/libservice/start.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-21 10:45:35.501492 libservice-0.1.9/libservice/ticonn/
+-rw-rw-r--   0 joente    (1000) joente    (1000)       27 2022-10-21 06:25:36.000000 libservice-0.1.9/libservice/ticonn/__init__.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)       55 2022-10-21 06:25:36.000000 libservice-0.1.9/libservice/ticonn/ticonn.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-21 10:45:35.501492 libservice-0.1.9/libservice.egg-info/
+-rw-rw-r--   0 joente    (1000) joente    (1000)     4440 2023-04-21 10:45:35.000000 libservice-0.1.9/libservice.egg-info/PKG-INFO
+-rw-rw-r--   0 joente    (1000) joente    (1000)      745 2023-04-21 10:45:35.000000 libservice-0.1.9/libservice.egg-info/SOURCES.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)        1 2023-04-21 10:45:35.000000 libservice-0.1.9/libservice.egg-info/dependency_links.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       46 2023-04-21 10:45:35.000000 libservice-0.1.9/libservice.egg-info/requires.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       11 2023-04-21 10:45:35.000000 libservice-0.1.9/libservice.egg-info/top_level.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       75 2023-04-20 08:15:18.000000 libservice-0.1.9/requirements.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       38 2023-04-21 10:45:35.501492 libservice-0.1.9/setup.cfg
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1555 2023-02-20 09:28:37.000000 libservice-0.1.9/setup.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)       22 2023-04-21 09:53:29.000000 libservice-0.1.9/version.py
```

### Comparing `libservice-0.1.8/.github/ISSUE_TEMPLATE/bug_report.md` & `libservice-0.1.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `libservice-0.1.8/.github/ISSUE_TEMPLATE/feature_request.md` & `libservice-0.1.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `libservice-0.1.8/.github/workflows/ci.yml` & `libservice-0.1.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `libservice-0.1.8/.gitignore` & `libservice-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `libservice-0.1.8/LICENSE` & `libservice-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `libservice-0.1.8/PKG-INFO` & `libservice-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: libservice
-Version: 0.1.8
+Version: 0.1.9
 Summary: Library for building InfraSonar services
 Home-page: https://github.com/infrasonar/python-libservice
-Download-URL: https://github.com/infrasonar/python-libservice/tarball/v0.1.8
+Download-URL: https://github.com/infrasonar/python-libservice/tarball/v0.1.9
 Author: Cesbit
 Author-email: info@cesbit.com
 License: UNKNOWN
 Keywords: monitoring,infrasonar,service
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `libservice-0.1.8/README.md` & `libservice-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `libservice-0.1.8/libservice/asset.py` & `libservice-0.1.9/libservice/asset.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,14 +20,17 @@
         self.check_id = check_id
         self.config = config
         self.key = None
 
     def __repr__(self) -> str:
         return f"asset: {self.asset_id} check: {self.check_id}"
 
+    def get_interval(self) -> int:
+        return self.config['_interval']
+
     async def decrypt(self, secret: str):
         if self.key is None:
             self.key = await ticonn.run(
                 'get_encryption_key',
                 self.container_id)
 
         return Fernet(self.key).decrypt(base64.b64decode(secret)).decode()
```

### Comparing `libservice-0.1.8/libservice/check.py` & `libservice-0.1.9/libservice/check.py`

 * *Files identical despite different names*

### Comparing `libservice-0.1.8/libservice/exceptions.py` & `libservice-0.1.9/libservice/exceptions.py`

 * *Files identical despite different names*

### Comparing `libservice-0.1.8/libservice/hub/client.py` & `libservice-0.1.9/libservice/hub/client.py`

 * *Files identical despite different names*

### Comparing `libservice-0.1.8/libservice/hub/net/package.py` & `libservice-0.1.9/libservice/hub/net/package.py`

 * *Files identical despite different names*

### Comparing `libservice-0.1.8/libservice/hub/net/protocol.py` & `libservice-0.1.9/libservice/hub/net/protocol.py`

 * *Files identical despite different names*

### Comparing `libservice-0.1.8/libservice/hub/protocol.py` & `libservice-0.1.9/libservice/hub/protocol.py`

 * *Files identical despite different names*

### Comparing `libservice-0.1.8/libservice/logger.py` & `libservice-0.1.9/libservice/logger.py`

 * *Files identical despite different names*

### Comparing `libservice-0.1.8/libservice/serviceroom.py` & `libservice-0.1.9/libservice/serviceroom.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,21 +21,23 @@
 assert 60 >= SLEEP_TIME > 0
 
 
 class ServiceRoom(Room):
 
     def init(self, collector_key: str,
              checks: Tuple[Union[CheckBase, CheckBaseMulti]],
-             on_log_level: Callable[[int], None], no_count: bool = False):
+             on_log_level: Callable[[int], None], no_count: bool = False,
+             max_timeout: float = 300.0):
         self.collector_key = collector_key
         self._checks = {check.key: check for check in checks}
         self._last = int(time.time())-1
         self._scheduled: Dict[int, Dict[int, dict]] = defaultdict(dict)
         self._on_log_level = on_log_level
         self._no_count = no_count
+        self._max_timeout = max_timeout
 
     async def load_all(self):
         self._query = functools.partial(self.client.query, scope=self.scope)
         assert self.collector_key, 'run init before load_all()'
         root_id, root = await self._query("""//ti
             [.root.id(), .root.wrap("_ContainerSvc")];
         """)
@@ -117,15 +119,20 @@
             logging.error(f'Failed to send data to hub: {msg}; {asset}')
         else:
             logging.debug(f'successfully send data to hub; {asset}')
 
     async def _run_multi(self, check: CheckBaseMulti, assets: List[Asset]):
         ts = time.time()
         try:
-            results = await check.run(ts, assets)
+            results = await asyncio.wait_for(
+                check.run(ts, assets),
+                timeout=self._max_timeout)
+        except asyncio.TimeoutError:
+            error = CheckException('timed out').to_dict()
+            results = [(None, error)] * len(assets)
         except CheckException as e:
             error = e.to_dict()
             results = [(None, error)] * len(assets)
         except Exception as e:
             msg = str(e) or type(e).__name__
             error = CheckException(msg).to_dict()
             results = [(None, error)] * len(assets)
@@ -133,16 +140,21 @@
         for asset, (result, error) in zip(assets, results):
             await self._send_to_hub(asset, result, error, ts, self._no_count)
             await asyncio.sleep(HUB_REQ_SLEEP)
 
     async def _run(self, check: CheckBase, asset: Asset):
         ts = time.time()
         no_count = self._no_count
+        timeout = min(0.8 * asset.get_interval(), self._max_timeout)
         try:
-            result, error = await check.run(ts, asset)
+            result, error = await asyncio.wait_for(
+                check.run(ts, asset),
+                timeout=timeout)
+        except asyncio.TimeoutError:
+            result, error = None, CheckException('timed out').to_dict()
         except NoCountException as e:
             result, error, no_count = e.result, None, True  # Force True
         except CheckException as e:
             result, error = None, e.to_dict()
         except Exception as e:
             msg = str(e) or type(e).__name__
             result, error = None, CheckException(msg).to_dict()
```

### Comparing `libservice-0.1.8/libservice/start.py` & `libservice-0.1.9/libservice/start.py`

 * *Files identical despite different names*

### Comparing `libservice-0.1.8/libservice.egg-info/PKG-INFO` & `libservice-0.1.9/libservice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: libservice
-Version: 0.1.8
+Version: 0.1.9
 Summary: Library for building InfraSonar services
 Home-page: https://github.com/infrasonar/python-libservice
-Download-URL: https://github.com/infrasonar/python-libservice/tarball/v0.1.8
+Download-URL: https://github.com/infrasonar/python-libservice/tarball/v0.1.9
 Author: Cesbit
 Author-email: info@cesbit.com
 License: UNKNOWN
 Keywords: monitoring,infrasonar,service
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `libservice-0.1.8/libservice.egg-info/SOURCES.txt` & `libservice-0.1.9/libservice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libservice-0.1.8/setup.py` & `libservice-0.1.9/setup.py`

 * *Files identical despite different names*

