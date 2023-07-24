# Comparing `tmp/flardl-0.0.4.tar.gz` & `tmp/flardl-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flardl-0.0.4.tar", max compression
+gzip compressed data, was "flardl-0.0.5.tar", max compression
```

## Comparing `flardl-0.0.4.tar` & `flardl-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1958 2023-07-17 23:01:11.854476 flardl-0.0.4/LICENSE
--rw-r--r--   0        0        0      243 2023-07-17 23:01:11.854476 flardl-0.0.4/LICENSE.logo.txt
--rw-r--r--   0        0        0     5376 2023-07-17 23:01:11.854476 flardl-0.0.4/README.md
--rw-r--r--   0        0        0     2762 2023-07-17 23:01:24.174634 flardl-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      673 2023-07-17 23:01:24.174634 flardl-0.0.4/src/flardl/__init__.py
--rw-r--r--   0        0        0     3380 2023-07-17 23:01:11.858476 flardl-0.0.4/src/flardl/common.py
--rw-r--r--   0        0        0     1581 2023-07-17 23:01:11.858476 flardl-0.0.4/src/flardl/dict_to_indexed_list.py
--rwxr-xr-x   0        0        0     8195 2023-07-17 23:01:24.174634 flardl-0.0.4/src/flardl/downloader.py
--rwxr-xr-x   0        0        0     4225 2023-07-17 23:01:11.858476 flardl-0.0.4/src/flardl/instrumented_streams.py
--rwxr-xr-x   0        0        0     7304 2023-07-17 23:01:24.174634 flardl-0.0.4/src/flardl/multidispatcher.py
--rw-r--r--   0        0        0        0 2023-07-17 23:01:11.858476 flardl-0.0.4/src/flardl/py.typed
--rw-r--r--   0        0        0      613 2023-07-17 23:01:24.174634 flardl-0.0.4/src/flardl/server_defs.py
--rwxr-xr-x   0        0        0    11622 2023-07-17 23:01:11.858476 flardl-0.0.4/src/flardl/stream_stats.py
--rw-r--r--   0        0        0     6716 1970-01-01 00:00:00.000000 flardl-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1958 2023-07-24 22:21:35.793575 flardl-0.0.5/LICENSE
+-rw-r--r--   0        0        0      243 2023-07-24 22:21:35.793575 flardl-0.0.5/LICENSE.logo.txt
+-rw-r--r--   0        0        0     7841 2023-07-24 22:21:48.441846 flardl-0.0.5/README.md
+-rw-r--r--   0        0        0     2781 2023-07-24 22:21:48.441846 flardl-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      673 2023-07-24 22:21:35.797575 flardl-0.0.5/src/flardl/__init__.py
+-rw-r--r--   0        0        0     3380 2023-07-24 22:21:35.797575 flardl-0.0.5/src/flardl/common.py
+-rw-r--r--   0        0        0     1581 2023-07-24 22:21:35.797575 flardl-0.0.5/src/flardl/dict_to_indexed_list.py
+-rwxr-xr-x   0        0        0     8265 2023-07-24 22:21:35.797575 flardl-0.0.5/src/flardl/downloader.py
+-rwxr-xr-x   0        0        0     4225 2023-07-24 22:21:35.797575 flardl-0.0.5/src/flardl/instrumented_streams.py
+-rwxr-xr-x   0        0        0     7304 2023-07-24 22:21:35.797575 flardl-0.0.5/src/flardl/multidispatcher.py
+-rw-r--r--   0        0        0        0 2023-07-24 22:21:35.797575 flardl-0.0.5/src/flardl/py.typed
+-rw-r--r--   0        0        0      651 2023-07-24 22:21:35.797575 flardl-0.0.5/src/flardl/server_defs.py
+-rwxr-xr-x   0        0        0    11622 2023-07-24 22:21:35.797575 flardl-0.0.5/src/flardl/stream_stats.py
+-rw-r--r--   0        0        0     9181 1970-01-01 00:00:00.000000 flardl-0.0.5/PKG-INFO
```

### Comparing `flardl-0.0.4/LICENSE` & `flardl-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flardl-0.0.4/pyproject.toml` & `flardl-0.0.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flardl"
-version = "0.0.4"
+version = "0.0.5"
 description = "Flardl"
 authors = ["Joel Berendzen <joel@generisbio.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/hydrationdynamics/flardl"
 repository = "https://github.com/hydrationdynamics/flardl"
 documentation = "https://flardl.readthedocs.io"
@@ -68,14 +68,15 @@
 myst-parser = {version = ">=0.16.1"}
 # test deps for this package
 loguru-mypy = ">=0.0.4"
 pandas = ">=1.4.0"
 pandas-stubs = ">=1.5.2.221124"
 pytest-datadir-mgr = ">1.3.1"
 pytest-trio = ">=0.8.0"
+numpy = ">=1.25.1"
 
 [tool.bandit]
 exclude_dirs = ["tests/", "noxfile.py"]
 skips = ["B101", "B311"]
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
```

### Comparing `flardl-0.0.4/src/flardl/__init__.py` & `flardl-0.0.5/src/flardl/__init__.py`

 * *Files identical despite different names*

### Comparing `flardl-0.0.4/src/flardl/common.py` & `flardl-0.0.5/src/flardl/common.py`

 * *Files identical despite different names*

### Comparing `flardl-0.0.4/src/flardl/dict_to_indexed_list.py` & `flardl-0.0.5/src/flardl/dict_to_indexed_list.py`

 * *Files identical despite different names*

### Comparing `flardl-0.0.4/src/flardl/downloader.py` & `flardl-0.0.5/src/flardl/downloader.py`

 * *Files 6% similar despite different names*

```diff
@@ -210,32 +210,36 @@
         *args,
         server: str,
         dir: str,
         transport: str,
         transport_ver: str,
         bw_limit_mbps: float,
         queue_depth: int,
-        timeout_ms: float,
+        timeout_s: float,
         **super_kwargs,
     ):
         """Init with id number."""
         super().__init__(*args, **super_kwargs)
-        self.hard_exceptions: tuple[()] | tuple[type[BaseException]] = (ValueError,)
+        self.hard_exceptions: tuple[()] | tuple[type[BaseException]] = (
+            httpx.ConnectError,
+        )
         self.soft_exceptions: tuple[()] | tuple[type[BaseException]] = (
             ConnectionError,
         )
         self.launch_rate = self.LAUNCH_RATE_MAX
         self.base_url = transport + "://" + server + "/"
         if dir != "":
             self.base_url += dir + "/"
         if transport_ver == "2":
             self.http2 = True
         else:
             self.http2 = False
-        self.client = httpx.AsyncClient(base_url=self.base_url, http2=self.http2)
+        self.client = httpx.AsyncClient(
+            base_url=self.base_url, http2=self.http2, timeout=timeout_s
+        )
 
     async def worker(
         self,
         result_q: ResultStream,
         worker_count: int,
         /,
         idx: int,
```

### Comparing `flardl-0.0.4/src/flardl/instrumented_streams.py` & `flardl-0.0.5/src/flardl/instrumented_streams.py`

 * *Files identical despite different names*

### Comparing `flardl-0.0.4/src/flardl/multidispatcher.py` & `flardl-0.0.5/src/flardl/multidispatcher.py`

 * *Files identical despite different names*

### Comparing `flardl-0.0.4/src/flardl/server_defs.py` & `flardl-0.0.5/src/flardl/server_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define server attributes."""
+from typing import Optional
 
 from attrs import asdict
 from attrs import define
 
 from .common import SIMPLE_TYPES
 
 
@@ -16,12 +17,12 @@
     name: str
     server: str
     dir: str = ""
     transport: str = "https"
     transport_ver: str = "1"
     bw_limit_mbps: float = 0.0
     queue_depth: int = 0
-    timeout_ms: float = 0.0
+    timeout_s: Optional[float] = None
 
     def get_all(self) -> dict[str, SIMPLE_TYPES]:
         """Return dictionary of non-private attributes."""
         return asdict(self, filter=lambda attr, value: not attr.name.startswith("_"))
```

### Comparing `flardl-0.0.4/src/flardl/stream_stats.py` & `flardl-0.0.5/src/flardl/stream_stats.py`

 * *Files identical despite different names*

