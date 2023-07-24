# Comparing `tmp/sddp_discovery_protocol-1.1.0.tar.gz` & `tmp/sddp_discovery_protocol-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sddp_discovery_protocol-1.1.0.tar", max compression
+gzip compressed data, was "sddp_discovery_protocol-1.2.0.tar", max compression
```

## Comparing `sddp_discovery_protocol-1.1.0.tar` & `sddp_discovery_protocol-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1075 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/LICENSE
--rw-r--r--   0        0        0    13789 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/README.md
--rw-r--r--   0        0        0     1330 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1812 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/__init__.py
--rwxr-xr-x   0        0        0    12686 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/__main__.py
--rwxr-xr-x   0        0        0    17332 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/client.py
--rw-r--r--   0        0        0      319 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/constants.py
--rw-r--r--   0        0        0      253 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/exceptions.py
--rw-r--r--   0        0        0     1466 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/internal_types.py
--rwxr-xr-x   0        0        0      269 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/pkg_logging.py
--rw-r--r--   0        0        0        0 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/py.typed
--rwxr-xr-x   0        0        0    19088 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/sddp_datagram.py
--rwxr-xr-x   0        0        0    20519 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/sddp_socket.py
--rwxr-xr-x   0        0        0    17429 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/server.py
--rwxr-xr-x   0        0        0     8360 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/util.py
--rw-r--r--   0        0        0      454 2023-07-24 23:25:57.064393 sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/version.py
--rw-r--r--   0        0        0    14782 1970-01-01 00:00:00.000000 sddp_discovery_protocol-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-24 23:34:25.750936 sddp_discovery_protocol-1.2.0/LICENSE
+-rw-r--r--   0        0        0    13789 2023-07-24 23:34:25.750936 sddp_discovery_protocol-1.2.0/README.md
+-rw-r--r--   0        0        0     1353 2023-07-24 23:34:25.750936 sddp_discovery_protocol-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1812 2023-07-24 23:34:25.750936 sddp_discovery_protocol-1.2.0/sddp_discovery_protocol/__init__.py
+-rwxr-xr-x   0        0        0    12686 2023-07-24 23:34:25.750936 sddp_discovery_protocol-1.2.0/sddp_discovery_protocol/__main__.py
+-rwxr-xr-x   0        0        0    17332 2023-07-24 23:34:25.750936 sddp_discovery_protocol-1.2.0/sddp_discovery_protocol/client.py
+-rw-r--r--   0        0        0      319 2023-07-24 23:34:25.750936 sddp_discovery_protocol-1.2.0/sddp_discovery_protocol/constants.py
+-rw-r--r--   0        0        0      253 2023-07-24 23:34:25.750936 sddp_discovery_protocol-1.2.0/sddp_discovery_protocol/exceptions.py
+-rw-r--r--   0        0        0     1466 2023-07-24 23:34:25.750936 sddp_discovery_protocol-1.2.0/sddp_discovery_protocol/internal_types.py
+-rwxr-xr-x   0        0        0      269 2023-07-24 23:34:25.750936 sddp_discovery_protocol-1.2.0/sddp_discovery_protocol/pkg_logging.py
+-rw-r--r--   0        0        0        0 2023-07-24 23:34:25.750936 sddp_discovery_protocol-1.2.0/sddp_discovery_protocol/py.typed
+-rwxr-xr-x   0        0        0    19088 2023-07-24 23:34:25.750936 sddp_discovery_protocol-1.2.0/sddp_discovery_protocol/sddp_datagram.py
+-rwxr-xr-x   0        0        0    20519 2023-07-24 23:34:25.750936 sddp_discovery_protocol-1.2.0/sddp_discovery_protocol/sddp_socket.py
+-rwxr-xr-x   0        0        0    17429 2023-07-24 23:34:25.750936 sddp_discovery_protocol-1.2.0/sddp_discovery_protocol/server.py
+-rwxr-xr-x   0        0        0     8360 2023-07-24 23:34:25.754936 sddp_discovery_protocol-1.2.0/sddp_discovery_protocol/util.py
+-rw-r--r--   0        0        0      454 2023-07-24 23:34:25.754936 sddp_discovery_protocol-1.2.0/sddp_discovery_protocol/version.py
+-rw-r--r--   0        0        0    14748 1970-01-01 00:00:00.000000 sddp_discovery_protocol-1.2.0/PKG-INFO
```

### Comparing `sddp_discovery_protocol-1.1.0/LICENSE` & `sddp_discovery_protocol-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sddp_discovery_protocol-1.1.0/README.md` & `sddp_discovery_protocol-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sddp_discovery_protocol-1.1.0/pyproject.toml` & `sddp_discovery_protocol-1.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [tool.poetry]
 name = "sddp-discovery-protocol"
-version = "1.1.0"
+version = "1.2.0"
 description = "Implementation of Control4's Simple Device Discovery Protocol (SDDP)"
 authors = [ "Sam McKelvie <dev@mckelvie.org>" ]
 license = "MIT"
 keywords = [ "Control4", "SDDP", "SSDP", "UPnP", "protocol", "multicast", "UDP",
              "discovery", "network", "automation", "smart-home" ]
 readme = "README.md"
 homepage = "https://github.com/sammck/sddp-discovery-protocol"
 repository = "https://github.com/sammck/sddp-discovery-protocol.git"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 #argcomplete = "^2.0.0"
-jq = "^1.2.2"
-colorama = "^0.4.4"
+#jq = "^1.2.2"
+#colorama = "^0.4.4"
 typing-extensions = "^4.7.1"
 netifaces-plus = "^0.12.0"
+requests = "^2.31.0"
 
 [tool.poetry.dev-dependencies]
 mypy = "^0.931"
 #dunamai = "^1.9.0"
 python-semantic-release = "^7.25.2"
 #pydoc-markdown = "^4.6.0"
 #doc2md = "^0.1.0"
```

### Comparing `sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/__init__.py` & `sddp_discovery_protocol-1.2.0/sddp_discovery_protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/__main__.py` & `sddp_discovery_protocol-1.2.0/sddp_discovery_protocol/__main__.py`

 * *Files identical despite different names*

### Comparing `sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/client.py` & `sddp_discovery_protocol-1.2.0/sddp_discovery_protocol/client.py`

 * *Files identical despite different names*

### Comparing `sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/internal_types.py` & `sddp_discovery_protocol-1.2.0/sddp_discovery_protocol/internal_types.py`

 * *Files identical despite different names*

### Comparing `sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/sddp_datagram.py` & `sddp_discovery_protocol-1.2.0/sddp_discovery_protocol/sddp_datagram.py`

 * *Files identical despite different names*

### Comparing `sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/sddp_socket.py` & `sddp_discovery_protocol-1.2.0/sddp_discovery_protocol/sddp_socket.py`

 * *Files identical despite different names*

### Comparing `sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/server.py` & `sddp_discovery_protocol-1.2.0/sddp_discovery_protocol/server.py`

 * *Files identical despite different names*

### Comparing `sddp_discovery_protocol-1.1.0/sddp_discovery_protocol/util.py` & `sddp_discovery_protocol-1.2.0/sddp_discovery_protocol/util.py`

 * *Files identical despite different names*

### Comparing `sddp_discovery_protocol-1.1.0/PKG-INFO` & `sddp_discovery_protocol-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: sddp-discovery-protocol
-Version: 1.1.0
+Version: 1.2.0
 Summary: Implementation of Control4's Simple Device Discovery Protocol (SDDP)
 Home-page: https://github.com/sammck/sddp-discovery-protocol
 License: MIT
 Keywords: Control4,SDDP,SSDP,UPnP,protocol,multicast,UDP,discovery,network,automation,smart-home
 Author: Sam McKelvie
 Author-email: dev@mckelvie.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: colorama (>=0.4.4,<0.5.0)
-Requires-Dist: jq (>=1.2.2,<2.0.0)
 Requires-Dist: netifaces-plus (>=0.12.0,<0.13.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: typing-extensions (>=4.7.1,<5.0.0)
 Project-URL: Repository, https://github.com/sammck/sddp-discovery-protocol.git
 Description-Content-Type: text/markdown
 
 sddp-discovery-protocol: Protocol library for Control4's Simple Device Discovery Protocol (SDDP)
 =================================================
```

