# Comparing `tmp/python-otbr-api-2.2.0.tar.gz` & `tmp/python-otbr-api-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-otbr-api-2.2.0.tar", last modified: Wed Jun  7 12:40:18 2023, max compression
+gzip compressed data, was "python-otbr-api-2.3.0.tar", last modified: Tue Jul 25 06:19:39 2023, max compression
```

## Comparing `python-otbr-api-2.2.0.tar` & `python-otbr-api-2.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:40:18.849282 python-otbr-api-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-07 12:39:59.000000 python-otbr-api-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-07 12:40:18.849282 python-otbr-api-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-07 12:39:59.000000 python-otbr-api-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-07 12:39:59.000000 python-otbr-api-2.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:40:18.845282 python-otbr-api-2.2.0/python_otbr_api/
--rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-06-07 12:39:59.000000 python-otbr-api-2.2.0/python_otbr_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-07 12:39:59.000000 python-otbr-api-2.2.0/python_otbr_api/mdns.py
--rw-r--r--   0 runner    (1001) docker     (123)     8565 2023-06-07 12:39:59.000000 python-otbr-api-2.2.0/python_otbr_api/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-07 12:39:59.000000 python-otbr-api-2.2.0/python_otbr_api/pskc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 12:39:59.000000 python-otbr-api-2.2.0/python_otbr_api/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-06-07 12:39:59.000000 python-otbr-api-2.2.0/python_otbr_api/tlv_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:40:18.849282 python-otbr-api-2.2.0/python_otbr_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-07 12:40:18.000000 python-otbr-api-2.2.0/python_otbr_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-07 12:40:18.000000 python-otbr-api-2.2.0/python_otbr_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 12:40:18.000000 python-otbr-api-2.2.0/python_otbr_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-07 12:40:18.000000 python-otbr-api-2.2.0/python_otbr_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-07 12:40:18.000000 python-otbr-api-2.2.0/python_otbr_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 12:40:18.000000 python-otbr-api-2.2.0/python_otbr_api.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-07 12:40:18.849282 python-otbr-api-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:19:39.529856 python-otbr-api-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-25 06:19:16.000000 python-otbr-api-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-25 06:19:39.529856 python-otbr-api-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-25 06:19:16.000000 python-otbr-api-2.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-25 06:19:16.000000 python-otbr-api-2.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:19:39.525856 python-otbr-api-2.3.0/python_otbr_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-07-25 06:19:16.000000 python-otbr-api-2.3.0/python_otbr_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-25 06:19:16.000000 python-otbr-api-2.3.0/python_otbr_api/mdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8565 2023-07-25 06:19:16.000000 python-otbr-api-2.3.0/python_otbr_api/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-25 06:19:16.000000 python-otbr-api-2.3.0/python_otbr_api/pskc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 06:19:16.000000 python-otbr-api-2.3.0/python_otbr_api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-07-25 06:19:16.000000 python-otbr-api-2.3.0/python_otbr_api/tlv_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:19:39.529856 python-otbr-api-2.3.0/python_otbr_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-25 06:19:39.000000 python-otbr-api-2.3.0/python_otbr_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-25 06:19:39.000000 python-otbr-api-2.3.0/python_otbr_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:19:39.000000 python-otbr-api-2.3.0/python_otbr_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-25 06:19:39.000000 python-otbr-api-2.3.0/python_otbr_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 06:19:39.000000 python-otbr-api-2.3.0/python_otbr_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:19:39.000000 python-otbr-api-2.3.0/python_otbr_api.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-25 06:19:39.529856 python-otbr-api-2.3.0/setup.cfg
```

### Comparing `python-otbr-api-2.2.0/LICENSE` & `python-otbr-api-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-otbr-api-2.2.0/pyproject.toml` & `python-otbr-api-2.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=65.6", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name         = "python-otbr-api"
-version      = "2.2.0"
+version      = "2.3.0"
 license      = {text = "MIT"}
 description  = "API to interact with an OTBR via its REST API"
 readme       = "README.md"
 authors      = [
     {name = "The Home Assistant Authors", email = "hello@home-assistant.io"}
 ]
 requires-python = ">=3.9.0"
```

### Comparing `python-otbr-api-2.2.0/python_otbr_api/__init__.py` & `python-otbr-api-2.3.0/python_otbr_api/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 PENDING_DATASET_DELAY_TIMER = 5 * 60 * 1000
 
 
 class OTBRError(Exception):
     """Raised on error."""
 
 
+class FactoryResetNotSupportedError(OTBRError):
+    """Raised when attempting to factory reset a router which does not support it."""
+
+
 class ThreadNetworkActiveError(OTBRError):
     """Raised on attempts to modify the active dataset when thread network is active."""
 
 
 class OTBR:  # pylint: disable=too-few-public-methods
     """Class to interact with the Open Thread Border Router REST API."""
 
@@ -28,14 +32,28 @@
         self, url: str, session: aiohttp.ClientSession, timeout: int = 10
     ) -> None:
         """Initialize."""
         self._session = session
         self._url = url
         self._timeout = timeout
 
+    async def factory_reset(self) -> None:
+        """Factory reset the router."""
+
+        response = await self._session.delete(
+            f"{self._url}/node",
+            timeout=aiohttp.ClientTimeout(total=10),
+        )
+
+        if response.status == HTTPStatus.METHOD_NOT_ALLOWED:
+            raise FactoryResetNotSupportedError
+
+        if response.status != HTTPStatus.OK:
+            raise OTBRError(f"unexpected http status {response.status}")
+
     async def set_enabled(self, enabled: bool) -> None:
         """Enable or disable the router."""
 
         response = await self._session.put(
             f"{self._url}/node/state",
             json="enable" if enabled else "disable",
             timeout=aiohttp.ClientTimeout(total=10),
```

### Comparing `python-otbr-api-2.2.0/python_otbr_api/mdns.py` & `python-otbr-api-2.3.0/python_otbr_api/mdns.py`

 * *Files identical despite different names*

### Comparing `python-otbr-api-2.2.0/python_otbr_api/models.py` & `python-otbr-api-2.3.0/python_otbr_api/models.py`

 * *Files identical despite different names*

### Comparing `python-otbr-api-2.2.0/python_otbr_api/pskc.py` & `python-otbr-api-2.3.0/python_otbr_api/pskc.py`

 * *Files identical despite different names*

### Comparing `python-otbr-api-2.2.0/python_otbr_api/tlv_parser.py` & `python-otbr-api-2.3.0/python_otbr_api/tlv_parser.py`

 * *Files identical despite different names*

