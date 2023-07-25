# Comparing `tmp/fsapi-tools-1.0.0rc0.tar.gz` & `tmp/fsapi-tools-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsapi-tools-1.0.0rc0.tar", last modified: Mon Jul 17 09:52:49 2023, max compression
+gzip compressed data, was "fsapi-tools-2.0.0.tar", last modified: Tue Jul 25 15:08:13 2023, max compression
```

## Comparing `fsapi-tools-1.0.0rc0.tar` & `fsapi-tools-2.0.0.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 09:52:49.023280 fsapi-tools-1.0.0rc0/
--rw-rw-rw-   0        0        0     1090 2023-07-16 17:34:26.000000 fsapi-tools-1.0.0rc0/LICENSE
--rw-rw-rw-   0        0        0    10789 2023-07-17 09:52:49.032733 fsapi-tools-1.0.0rc0/PKG-INFO
--rw-rw-rw-   0        0        0     9982 2023-07-17 09:33:01.000000 fsapi-tools-1.0.0rc0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 09:52:48.060670 fsapi-tools-1.0.0rc0/fsapi/
--rw-rw-rw-   0        0        0     1311 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/__init__.py
--rw-rw-rw-   0        0        0     1202 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:52:48.208990 fsapi-tools-1.0.0rc0/fsapi/ecmascript/
--rw-rw-rw-   0        0        0     2169 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/ecmascript/__init__.py
--rw-rw-rw-   0        0        0     1193 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/ecmascript/__main__.py
--rw-rw-rw-   0        0        0     3180 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/ecmascript/cli.py
--rw-rw-rw-   0        0        0     4611 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/ecmascript/esbin.py
--rw-rw-rw-   0        0        0     9035 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/ecmascript/opcode.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:52:48.483648 fsapi-tools-1.0.0rc0/fsapi/isu/
--rw-rw-rw-   0        0        0     2820 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/isu/__init__.py
--rw-rw-rw-   0        0        0     1187 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/isu/__main__.py
--rw-rw-rw-   0        0        0     9012 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/isu/cli.py
--rw-rw-rw-   0        0        0    12597 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/isu/format.py
--rw-rw-rw-   0        0        0     6965 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/isu/product.py
--rw-rw-rw-   0        0        0    11934 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/isu/update.py
--rw-rw-rw-   0        0        0     4126 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/isu/util.py
--rw-rw-rw-   0        0        0     2619 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/netconfig.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:52:48.802739 fsapi-tools-1.0.0rc0/fsapi/netremote/
--rw-rw-rw-   0        0        0     5190 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/netremote/__init__.py
--rw-rw-rw-   0        0        0     9939 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/netremote/basenode.py
--rw-rw-rw-   0        0        0    11710 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/netremote/cli.py
--rw-rw-rw-   0        0        0   162959 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/netremote/nodes.py
--rw-rw-rw-   0        0        0     8638 2023-07-17 09:09:48.000000 fsapi-tools-1.0.0rc0/fsapi/netremote/radiohttp.py
-drwxrwxrwx   0        0        0        0 2023-07-17 09:52:48.936612 fsapi-tools-1.0.0rc0/fsapi_tools.egg-info/
--rw-rw-rw-   0        0        0    10789 2023-07-17 09:52:47.000000 fsapi-tools-1.0.0rc0/fsapi_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      673 2023-07-17 09:52:47.000000 fsapi-tools-1.0.0rc0/fsapi_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 09:52:47.000000 fsapi-tools-1.0.0rc0/fsapi_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-07-17 09:52:47.000000 fsapi-tools-1.0.0rc0/fsapi_tools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-07-17 09:52:47.000000 fsapi-tools-1.0.0rc0/fsapi_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      973 2023-07-17 09:09:49.000000 fsapi-tools-1.0.0rc0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-17 09:52:49.134566 fsapi-tools-1.0.0rc0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-25 15:08:13.083565 fsapi-tools-2.0.0/
+-rw-rw-rw-   0        0        0     1090 2023-07-16 17:34:26.000000 fsapi-tools-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0    11680 2023-07-25 15:08:13.054562 fsapi-tools-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10876 2023-07-25 15:04:14.000000 fsapi-tools-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 15:08:11.996760 fsapi-tools-2.0.0/fsapi/
+-rw-rw-rw-   0        0        0     1308 2023-07-25 15:06:23.000000 fsapi-tools-2.0.0/fsapi/__init__.py
+-rw-rw-rw-   0        0        0     1202 2023-07-17 09:09:48.000000 fsapi-tools-2.0.0/fsapi/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 15:08:12.147764 fsapi-tools-2.0.0/fsapi/ecmascript/
+-rw-rw-rw-   0        0        0     2169 2023-07-17 09:09:48.000000 fsapi-tools-2.0.0/fsapi/ecmascript/__init__.py
+-rw-rw-rw-   0        0        0     1193 2023-07-17 09:09:48.000000 fsapi-tools-2.0.0/fsapi/ecmascript/__main__.py
+-rw-rw-rw-   0        0        0     3180 2023-07-17 09:09:48.000000 fsapi-tools-2.0.0/fsapi/ecmascript/cli.py
+-rw-rw-rw-   0        0        0     4611 2023-07-17 09:09:48.000000 fsapi-tools-2.0.0/fsapi/ecmascript/esbin.py
+-rw-rw-rw-   0        0        0     9035 2023-07-17 09:09:48.000000 fsapi-tools-2.0.0/fsapi/ecmascript/opcode.py
+drwxrwxrwx   0        0        0        0 2023-07-25 15:08:12.413901 fsapi-tools-2.0.0/fsapi/isu/
+-rw-rw-rw-   0        0        0     2894 2023-07-25 15:04:15.000000 fsapi-tools-2.0.0/fsapi/isu/__init__.py
+-rw-rw-rw-   0        0        0     1187 2023-07-17 09:09:48.000000 fsapi-tools-2.0.0/fsapi/isu/__main__.py
+-rw-rw-rw-   0        0        0     9606 2023-07-20 20:12:20.000000 fsapi-tools-2.0.0/fsapi/isu/cli.py
+-rw-rw-rw-   0        0        0    18383 2023-07-20 20:12:20.000000 fsapi-tools-2.0.0/fsapi/isu/format.py
+-rw-rw-rw-   0        0        0     6965 2023-07-17 09:09:48.000000 fsapi-tools-2.0.0/fsapi/isu/product.py
+-rw-rw-rw-   0        0        0    13082 2023-07-25 15:04:15.000000 fsapi-tools-2.0.0/fsapi/isu/update.py
+-rw-rw-rw-   0        0        0     4253 2023-07-25 15:04:15.000000 fsapi-tools-2.0.0/fsapi/isu/util.py
+drwxrwxrwx   0        0        0        0 2023-07-25 15:08:12.761560 fsapi-tools-2.0.0/fsapi/net/
+-rw-rw-rw-   0        0        0     4300 2023-07-25 15:04:15.000000 fsapi-tools-2.0.0/fsapi/net/__init__.py
+-rw-rw-rw-   0        0        0     1187 2023-07-25 15:04:15.000000 fsapi-tools-2.0.0/fsapi/net/__main__.py
+-rw-rw-rw-   0        0        0     3865 2023-07-25 15:04:15.000000 fsapi-tools-2.0.0/fsapi/net/_enum.py
+-rw-rw-rw-   0        0        0   173833 2023-07-25 15:04:15.000000 fsapi-tools-2.0.0/fsapi/net/_nodes.py
+-rw-rw-rw-   0        0        0    11535 2023-07-25 15:04:15.000000 fsapi-tools-2.0.0/fsapi/net/_wrap.py
+-rw-rw-rw-   0        0        0    27881 2023-07-25 15:04:15.000000 fsapi-tools-2.0.0/fsapi/net/base.py
+-rw-rw-rw-   0        0        0    19805 2023-07-25 15:04:15.000000 fsapi-tools-2.0.0/fsapi/net/cli.py
+-rw-rw-rw-   0        0        0    15726 2023-07-25 15:04:15.000000 fsapi-tools-2.0.0/fsapi/net/device.py
+-rw-rw-rw-   0        0        0     2619 2023-07-17 09:09:48.000000 fsapi-tools-2.0.0/fsapi/netconfig.py
+drwxrwxrwx   0        0        0        0 2023-07-25 15:08:13.037568 fsapi-tools-2.0.0/fsapi_tools.egg-info/
+-rw-rw-rw-   0        0        0    11680 2023-07-25 15:08:11.000000 fsapi-tools-2.0.0/fsapi_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2023-07-25 15:08:11.000000 fsapi-tools-2.0.0/fsapi_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 15:08:11.000000 fsapi-tools-2.0.0/fsapi_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-07-25 15:08:11.000000 fsapi-tools-2.0.0/fsapi_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-07-25 15:08:11.000000 fsapi-tools-2.0.0/fsapi_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      964 2023-07-25 15:06:23.000000 fsapi-tools-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-25 15:08:13.085560 fsapi-tools-2.0.0/setup.cfg
```

### Comparing `fsapi-tools-1.0.0rc0/LICENSE` & `fsapi-tools-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fsapi-tools-1.0.0rc0/PKG-INFO` & `fsapi-tools-2.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsapi-tools
-Version: 1.0.0rc0
+Version: 2.0.0
 Summary: Frontier Smart Firmware Tools and FSAPI Implementation.
 Author-email: MatrixEditor <not@supported.com>
 Project-URL: Homepage, https://github.com/MatrixEditor/frontier-smart-api
 Project-URL: API-Docs, https://matrixeditor.github.io/frontier-smart-api/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div id="top"></div>
 <div align="center">
 
-![logo](docs/graphics/company_logo.png)
+![Company logo would be displayed here.](docs/graphics/company_logo.png)
 
 </div>
 
 # Frontier Smart API and Firmware Tools
 
 [![python](https://img.shields.io/badge/python-3.7+-blue.svg?logo=python&labelColor=grey)](https://www.python.org/downloads/)
 ![Codestyle](https://img.shields.io:/static/v1?label=Codestyle&message=black&color=black)
@@ -165,28 +165,41 @@
 ```
 
 ### NET - FSAPI
 
 This small tool can be utilized to interact with Frontier Smart devices via CLI.
 
 ```bash
-$ fsapi-net set -n sys.info.friendlyName --args value:MedionIR $IP_ADDRESS
-[+] fsapiResponse of netRemote.sys.info.friendlyName:
-    - status: FS_OK
-
-$ fsapi-net get -n sys.info.friendlyName $IP_ADDRESS
-[+] fsapiResponse of netRemote.sys.info.friendlyName:
-    - status: FS_OK
-    - value: MedionIR
-    - readonly: False
-    - notifying: True
+$ fsapi-ctl set netremote.sys.info.friendlyName "MedionIR" 127.0.0.1
+> FSResponse('netRemote.sys.info.friendlyName', <Method.SET: 'SET'>)
+    - status: <Status.FS_OK: 'FS_OK'>
+
+$ fsapi-ctl get netremote.sys.info.friendlyName 127.0.0.1
+> FSResponse('netRemote.sys.info.friendlyName', <Method.GET: 'GET'>)
+    - status: <Status.FS_OK: 'FS_OK'>
+    - value: 'Hello World'
 
-$ fsapi-net isu --find $IP_ADDRESS
+$ fsapi-ctl -X update fetch 127.0.0.1 .
 [+] Generating current URL...
-    - url: https://update.wifiradiofrontier.com/Update.aspx?f=/updates/ir-mmi-FS2026-0500-0549.2.12.25c.EX72088-1A12.isu.bin
+    > URL: 'https://update.wifiradiofrontier.com/Update.aspx?f=/updates/ir-mmi-FS2026-0500-0549.2.12.25c.EX72088-1A12.isu.bin'
+
+$ fsapi-ctl view netremote.sys.power
+> SYS: Power (netRemote_sys_power_nt):
+    - path: 'netRemote.sys.power'
+    - readonly: False
+    - cacheable: True
+    - notifying: True
+    - type: <class 'fsapi.net.base.NodeE8'>
+    - prototype:
+        [0] => 'value'
+            - length: 1
+            - type: <ArgType.ARG_TYPE_E8: 17>
+    - enum values:
+        [0] => 'OFF'
+        [1] => 'ON'
 ```
 
 ## Usage Examples
 
 ### ISU API
 
 ```python
@@ -198,42 +211,59 @@
 pp = DataclassPrinter()
 pp.print_object(isu.header)
 ```
 
 ## FSAPI
 
 ```python
-from fsapi.netremote import Set, Get, ListGetNext, nodes, FSDevice
-from fsapi.netconfig import FSNetConfiguration
-from fsapi.isu import isu_find_update, isu_new_url, isu_get_update
+from fsapi.net import FSDevice, wrap, nodes
+
+# First, create the radio object
+device = FSDevice("127.0.0.1")
+
+# Create a new session id (only one at a time)
+device.new_session()
+
+# In order to simplify the usage of the FSDevice class
+api = wrap(device)
+friendly_name = api.friendly_name
+# or manually
+response = device.get(nodes / "netRemote.sys.info.friendlyName")
+if response.status == FS_OK:
+    #_ Again, type(content) = nodes.BaseSysInfoFriendlyName
+    friendly_name = response.content.value
+
+    # Apply a new name via wrapper
+    api.friendly_name = "FooBar"
+    # or manually
+    device.put(nodes / "netRemote.sys.info.friendlyName", value="FooBar")
+
+# get all elements of a list
+valid_modes = api.ls_valid_modes()
+# get a certain amount of elements beginning at index 3
+valid_mpdes = api.ls_valid_modes(_pos=3, max_items=10)
+```
+
+## Software Update
+
+```python
+from fsapi.isu import find_update, url_get_update, get_update
 
 # 1.Find and download updates
 # without custom netconfig -> HTTPS traffic
-response = isu_find_update('$MAC', '$CUSTOM', '$VERSION')
+request = find_update('$MAC', '$CUSTOM', '$VERSION')
 
 # with custom config -> force HTTP traffic
 config = FSNetConfiguration(http_pool=urllib3.HTTPConnectionPool('$HOST'))
-response = isu_find_update('$MAC', '$CUSTOM', '$VERSION', netconfig=config)
+request = find_update('$MAC', '$CUSTOM', '$VERSION', netconfig=config)
 
 # without custom netconfig -> HTTPS traffic
-response = isu_find_update('$MAC', '$CUSTOM', '$VERSION')
-for _software in response['updates']:
-   isu_get_update('$FILE_PATH', software=_software)
-
-# First, create the device:
-device = FSDevice("127.0.0.1")
-
-# SET request
-result = Set(nodes.BaseSysInfoFriendlyName, device, value="Hello World")
-
-# GET request
-result = Get(nodes.BaseSysInfoFriendlyName, device)
-
-# LIST_GET_NEXT request
-result = ListGetNext(nodes.NODECLASS, device, maxItems=100)
+if request.has_update:
+    for _software in request.updates:
+        get_update('$FILE_PATH', software=_software)
 ```
 
 ## Contributing
 
 Contributions are highly appreciated as they contribute to the growth and improvement of the open-source community. If you have any suggestions that could enhance this project, please feel free to fork the repository and create a pull request. Alternatively, you can also open an issue with the "enhancement" tag.
 
 To contribute, follow these steps:
```

### Comparing `fsapi-tools-1.0.0rc0/README.md` & `fsapi-tools-2.0.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <div id="top"></div>
 <div align="center">
 
-![logo](docs/graphics/company_logo.png)
+![Company logo would be displayed here.](docs/graphics/company_logo.png)
 
 </div>
 
 # Frontier Smart API and Firmware Tools
 
 [![python](https://img.shields.io/badge/python-3.7+-blue.svg?logo=python&labelColor=grey)](https://www.python.org/downloads/)
 ![Codestyle](https://img.shields.io:/static/v1?label=Codestyle&message=black&color=black)
@@ -147,28 +147,41 @@
 ```
 
 ### NET - FSAPI
 
 This small tool can be utilized to interact with Frontier Smart devices via CLI.
 
 ```bash
-$ fsapi-net set -n sys.info.friendlyName --args value:MedionIR $IP_ADDRESS
-[+] fsapiResponse of netRemote.sys.info.friendlyName:
-    - status: FS_OK
-
-$ fsapi-net get -n sys.info.friendlyName $IP_ADDRESS
-[+] fsapiResponse of netRemote.sys.info.friendlyName:
-    - status: FS_OK
-    - value: MedionIR
-    - readonly: False
-    - notifying: True
+$ fsapi-ctl set netremote.sys.info.friendlyName "MedionIR" 127.0.0.1
+> FSResponse('netRemote.sys.info.friendlyName', <Method.SET: 'SET'>)
+    - status: <Status.FS_OK: 'FS_OK'>
+
+$ fsapi-ctl get netremote.sys.info.friendlyName 127.0.0.1
+> FSResponse('netRemote.sys.info.friendlyName', <Method.GET: 'GET'>)
+    - status: <Status.FS_OK: 'FS_OK'>
+    - value: 'Hello World'
 
-$ fsapi-net isu --find $IP_ADDRESS
+$ fsapi-ctl -X update fetch 127.0.0.1 .
 [+] Generating current URL...
-    - url: https://update.wifiradiofrontier.com/Update.aspx?f=/updates/ir-mmi-FS2026-0500-0549.2.12.25c.EX72088-1A12.isu.bin
+    > URL: 'https://update.wifiradiofrontier.com/Update.aspx?f=/updates/ir-mmi-FS2026-0500-0549.2.12.25c.EX72088-1A12.isu.bin'
+
+$ fsapi-ctl view netremote.sys.power
+> SYS: Power (netRemote_sys_power_nt):
+    - path: 'netRemote.sys.power'
+    - readonly: False
+    - cacheable: True
+    - notifying: True
+    - type: <class 'fsapi.net.base.NodeE8'>
+    - prototype:
+        [0] => 'value'
+            - length: 1
+            - type: <ArgType.ARG_TYPE_E8: 17>
+    - enum values:
+        [0] => 'OFF'
+        [1] => 'ON'
 ```
 
 ## Usage Examples
 
 ### ISU API
 
 ```python
@@ -180,42 +193,59 @@
 pp = DataclassPrinter()
 pp.print_object(isu.header)
 ```
 
 ## FSAPI
 
 ```python
-from fsapi.netremote import Set, Get, ListGetNext, nodes, FSDevice
-from fsapi.netconfig import FSNetConfiguration
-from fsapi.isu import isu_find_update, isu_new_url, isu_get_update
+from fsapi.net import FSDevice, wrap, nodes
+
+# First, create the radio object
+device = FSDevice("127.0.0.1")
+
+# Create a new session id (only one at a time)
+device.new_session()
+
+# In order to simplify the usage of the FSDevice class
+api = wrap(device)
+friendly_name = api.friendly_name
+# or manually
+response = device.get(nodes / "netRemote.sys.info.friendlyName")
+if response.status == FS_OK:
+    #_ Again, type(content) = nodes.BaseSysInfoFriendlyName
+    friendly_name = response.content.value
+
+    # Apply a new name via wrapper
+    api.friendly_name = "FooBar"
+    # or manually
+    device.put(nodes / "netRemote.sys.info.friendlyName", value="FooBar")
+
+# get all elements of a list
+valid_modes = api.ls_valid_modes()
+# get a certain amount of elements beginning at index 3
+valid_mpdes = api.ls_valid_modes(_pos=3, max_items=10)
+```
+
+## Software Update
+
+```python
+from fsapi.isu import find_update, url_get_update, get_update
 
 # 1.Find and download updates
 # without custom netconfig -> HTTPS traffic
-response = isu_find_update('$MAC', '$CUSTOM', '$VERSION')
+request = find_update('$MAC', '$CUSTOM', '$VERSION')
 
 # with custom config -> force HTTP traffic
 config = FSNetConfiguration(http_pool=urllib3.HTTPConnectionPool('$HOST'))
-response = isu_find_update('$MAC', '$CUSTOM', '$VERSION', netconfig=config)
+request = find_update('$MAC', '$CUSTOM', '$VERSION', netconfig=config)
 
 # without custom netconfig -> HTTPS traffic
-response = isu_find_update('$MAC', '$CUSTOM', '$VERSION')
-for _software in response['updates']:
-   isu_get_update('$FILE_PATH', software=_software)
-
-# First, create the device:
-device = FSDevice("127.0.0.1")
-
-# SET request
-result = Set(nodes.BaseSysInfoFriendlyName, device, value="Hello World")
-
-# GET request
-result = Get(nodes.BaseSysInfoFriendlyName, device)
-
-# LIST_GET_NEXT request
-result = ListGetNext(nodes.NODECLASS, device, maxItems=100)
+if request.has_update:
+    for _software in request.updates:
+        get_update('$FILE_PATH', software=_software)
 ```
 
 ## Contributing
 
 Contributions are highly appreciated as they contribute to the growth and improvement of the open-source community. If you have any suggestions that could enhance this project, please feel free to fork the repository and create a pull request. Alternatively, you can also open an issue with the "enhancement" tag.
 
 To contribute, follow these steps:
```

### Comparing `fsapi-tools-1.0.0rc0/fsapi/__init__.py` & `fsapi-tools-2.0.0/fsapi/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,9 +22,9 @@
 """
 A python implementation of the FSAPI with all possible nodes. To run this
 module type:
 
 >>> python3 -m fsapi --help
 """
 
-__version__ = "1.0.0-rc"
+__version__ = "2.0.0"
 __author__ = 'MatrixEditor'
```

### Comparing `fsapi-tools-1.0.0rc0/fsapi/__main__.py` & `fsapi-tools-2.0.0/fsapi/__main__.py`

 * *Files identical despite different names*

### Comparing `fsapi-tools-1.0.0rc0/fsapi/ecmascript/__init__.py` & `fsapi-tools-2.0.0/fsapi/ecmascript/__init__.py`

 * *Files identical despite different names*

### Comparing `fsapi-tools-1.0.0rc0/fsapi/ecmascript/__main__.py` & `fsapi-tools-2.0.0/fsapi/ecmascript/__main__.py`

 * *Files identical despite different names*

### Comparing `fsapi-tools-1.0.0rc0/fsapi/ecmascript/cli.py` & `fsapi-tools-2.0.0/fsapi/ecmascript/cli.py`

 * *Files identical despite different names*

### Comparing `fsapi-tools-1.0.0rc0/fsapi/ecmascript/esbin.py` & `fsapi-tools-2.0.0/fsapi/ecmascript/esbin.py`

 * *Files identical despite different names*

### Comparing `fsapi-tools-1.0.0rc0/fsapi/ecmascript/opcode.py` & `fsapi-tools-2.0.0/fsapi/ecmascript/opcode.py`

 * *Files identical despite different names*

### Comparing `fsapi-tools-1.0.0rc0/fsapi/isu/__init__.py` & `fsapi-tools-2.0.0/fsapi/isu/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,17 +38,21 @@
     FSCustomisation,
     FSVersion,
     RE_CUSTOMISATION,
     RE_VERSION,
     FSVERSION_MODULE_TYPES
 )
 from .update import (
-    isu_find_update,
-    isu_get_update,
-    isu_new_url,
+    find_update,
+    url_find_update,
+    UpdateError,
+    UpdateRequest,
+    UpdateStatus,
+    get_update,
+    url_get_update,
     ISU_EDGE_PROVIDER_HOST,
     ISU_FILE_PROVIDER_HOST,
     ISUSoftwareElement
 )
 from .format import (
     ISU,
     ISUHeader,
```

### Comparing `fsapi-tools-1.0.0rc0/fsapi/isu/__main__.py` & `fsapi-tools-2.0.0/fsapi/isu/__main__.py`

 * *Files identical despite different names*

### Comparing `fsapi-tools-1.0.0rc0/fsapi/isu/cli.py` & `fsapi-tools-2.0.0/fsapi/isu/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -96,24 +96,30 @@
     e_group.add_argument(
         "-eC",
         "--extract-core",
         default=None,
         metavar="PATH",
         help="Saves the compressed/encrypted core to the provided path.",
     )
+    e_group.add_argument(
+        "-dC",
+        "--decompress-core",
+        action="store_true",
+        help="Decompresses the firmware core (onlay applicable with -eC).",
+    )
 
     argv = parser.parse_args(cmd)
     pp = DataclassPrinter(colorized=not argv.disable_color)
 
     # some sanity checks before we can start
     if not argv.dump_all and (
         not (argv.header or argv.archive or argv.fields)
         and not (argv.extract_core or argv.extract_archive, argv.json)
     ):
-        print(pp.get_msg(Fore.RED, "[!] -> Invalid options: nothing selected!"))
+        pp.print_msg(Fore.RED, "[!] -> Invalid options: nothing selected!")
         sys.exit(1)
 
     target_path = pathlib.Path(argv.path)
 
     if not target_path.is_dir():
         _run(argv, target_path, pp)
     else:
@@ -127,31 +133,31 @@
                 if out_archive_base:
                     new_path = pathlib.Path(out_archive_base) / path.stem
                     argv.extract_archive = new_path
                 try:
                     _run(argv, path, pp)
                     print()  # just for prettier output
                 except Exception as err:
-                    print(pp.get_msg(Fore.RED, f"[!] {type(err).__name__}:", str(err)))
+                    pp.print_msg(Fore.RED, f"[!] {type(err).__name__}:", str(err))
 
 
 def _run(argv, target: pathlib.Path, pp: DataclassPrinter):
-    print(pp.get_msg(Fore.LIGHTBLACK_EX, f"[in] {target}"))
+    pp.print_msg(Fore.LIGHTBLACK_EX, f"[in] {target}")
 
     isu = ISU.parse_file(str(target))
     header = isu.header
     if argv.header or argv.dump_all:
         pp.print_object(header, indent=3)
 
     fields = isu.data_fields
     if argv.fields or argv.dump_all:
         if len(fields) == 0:
-            print(pp.get_msg(Fore.YELLOW, " " * 3, "> No Data Fields"))
+            pp.print_msg(Fore.YELLOW, " " * 3, "> No Data Fields")
         else:
-            print(pp.get_msg(Fore.LIGHTBLACK_EX, " " * 3, "> Data Fields:"))
+            pp.print_msg(Fore.LIGHTBLACK_EX, " " * 3, "> Data Fields:")
             for i, data_field in enumerate(fields):
                 msg = " " * 7 + pp.get_array_format(i)
                 print(msg + pp.get_msg(Fore.LIGHTCYAN_EX, str(type(data_field))))
 
                 pp.print_object(data_field, indent=11)
 
     archive = isu.archive
@@ -172,42 +178,53 @@
             }
             if not argv.json_full:
                 # Don't include the data section if no explicitly activated
                 values["archive"].pop("data")
 
             with open(str(out_path), "w") as fp:
                 json.dump(values, fp, cls=BytesJSONEncoder)
-            print(pp.get_msg(Fore.LIGHTBLACK_EX, "[out] JSON saved to", str(out_path)))
+            pp.print_msg(Fore.LIGHTBLACK_EX, "[out] JSON saved to", str(out_path))
         else:
-            print(pp.get_msg(Fore.RED, "[!] Invalid JSON output path (is a dir)"))
+            pp.print_msg(Fore.RED, "[!] Invalid JSON output path (is a dir)")
 
     if argv.extract_core:
         field = fields["CompSize"]
         out_path = pathlib.Path(argv.extract_core)
         if out_path.is_dir():
             out_path = out_path / f"{header.customisation}_{header.version}.core.bin"
 
-        # we use this as identifier for now
-        index = isu.stream.find(b"\x1B\x00\x55\xAA", 0)
-        if index == -1:
-            print(pp.get_msg(Fore.RED, "[!] Could not find any compressed core data!"))
+        decomp_size = fields["DecompSize"]
+        core = isu.get_core(field.value)
+        if core.has_errors:
+            pp.print_msg(Fore.RED, "[!] Could not find any compressed core data!")
         else:
             with open(str(out_path), "wb") as fp:
-                fp.write(isu.stream[index : index + field.value])
+                if argv.decompress_core:
+                    msg = "[out] Saved decompressed core to"
+                    data = core.decompress(decomp_size.value)
+                    if core.has_errors:
+                        pp_msg = pp.get_msg(
+                            Fore.RED, "[!] Could not decompress core:", str(core.errors)
+                        )
+                        print(pp_msg)
+                    fp.write(data)
+                else:
+                    msg = "[out] Saved core to"
+                    fp.write(core.data)
 
-            print(pp.get_msg(Fore.LIGHTBLACK_EX, "[out] Saved core to", str(out_path)))
+            pp.print_msg(Fore.LIGHTBLACK_EX, msg, str(out_path))
 
     if argv.extract_archive and archive is not None:
         out_dir = pathlib.Path(argv.extract_archive)
         if not out_dir.exists():
             out_dir.mkdir(parents=True, exist_ok=True)
 
         if not out_dir.is_dir():
             out_dir = out_dir.parent
-        print(pp.get_msg(Fore.LIGHTBLACK_EX, "[out] Directory Archive:", str(out_dir)))
+        pp.print_msg(Fore.LIGHTBLACK_EX, "[out] Directory Archive:", str(out_dir))
         for entry in archive.index.entries:
             save_entry(entry, out_dir, isu, archive, pp, indent=3)
 
     isu.stream.close()
 
 
 def save_entry(
@@ -224,15 +241,15 @@
         content = entry.content
         with open(str(path / entry.name), "wb") as fp:
             data = isu.get_archive_file(content, archive)
             if content.is_compressed():
                 try:
                     fp.write(zlib.decompress(data))
                 except zlib.error as err:
-                    print(pp.get_msg(Fore.RED, " " * indent, f"! zlib.error: {err}"))
+                    pp.print_msg(Fore.RED, " " * indent, f"! zlib.error: {err}")
             else:
                 fp.write(data)
 
     else:
         msg = pp.get_msg(
             Fore.LIGHTBLACK_EX,
             " " * indent,
```

### Comparing `fsapi-tools-1.0.0rc0/fsapi/isu/product.py` & `fsapi-tools-2.0.0/fsapi/isu/product.py`

 * *Files identical despite different names*

### Comparing `fsapi-tools-1.0.0rc0/fsapi/isu/update.py` & `fsapi-tools-2.0.0/fsapi/isu/update.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,292 +17,341 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 __doc__ = """
 The backend used to find and download updates is located at ``update.wifiradiofrontier.com.``
-To interact with the underlaying API, the isudata-module comes with two main-methods:
+To interact with the underlaying API, the isudata-module comes with three main-methods:
 
-* ``isu_new_url``,
-* ``isu_find_update`` and
-* ``isu_get_update``.
+* ``url_get_update``,
+* ``find_update`` and
+* ``get_update``.
 
 """
 
 import urllib3
 import re
+import dataclasses
+import enum
 import xml.etree.ElementTree as xmltree
 
 from fsapi.netconfig import FSNetConfiguration
 from .product import RE_CUSTOMISATION, RE_VERSION
 
 __all__ = [
     "ISU_FILE_PROVIDER_HOST",
     "ISUSoftwareElement",
-    "isu_find_update",
-    "isu_get_update",
-    "isu_new_url",
+    "UpdateError",
+    "MalformedMACError",
+    "CustomisationError",
+    "VersionError",
+    "UpdateStatus",
+    "UpdateRequest",
+    "url_find_update",
+    "find_update",
+    "get_update",
+    "url_get_update",
 ]
 
 ###############################################################################
 # Constants
 ###############################################################################
 ISU_FILE_PROVIDER_HOST = "update.wifiradiofrontier.com"
 ISU_EDGE_PROVIDER_HOST = "nuv-isu-cdn.azureedge.net"
 ISU_REQUEST_HEADERS = {"User-Agent": "FSL IR/0.1", "Connection": "Close"}
 
 # MAC-Address structure for internet radios:
 # '002261' + 6 characters from hex-alphabet
 RE_FSIR_MAC_ADDR = r"^(002261)[\w]{6}$"
 
 
-
 ###############################################################################
 # Classes
 ###############################################################################
+@dataclasses.dataclass
 class ISUSoftwareElement:
     """This class contains all information needed to distinguish an update entry.
 
     Use the ``loadxml`` function to import data from an XML-Element.
 
     :param customisaton: The customisation string for this element.
     :param version: The version string for this element.
     :param download_url: The URL where the firmware binary is located
     :param mandatory: Indicates whether this update is mandatory
     :param md5hash: The calculated md5Hash for the firmware binary
     :param product: The product's name
-    :param vendor: usually Frontier Smart
+    :param vendor: usually Frontier Silicon
     :param size: the file's size
     """
 
-    def __init__(
-        self,
-        customisation: str = None,
-        version: str = None,
-        download_url: str = None,
-        mandatory: bool = False,
-        md5hash: str = None,
-        product: str = None,
-        size: int = 0,
-        vendor: str = "Frontier Silicon",
-        summary: str = None,
-    ) -> None:
-        self.customisation = customisation
-        self.version = version
-        self.download_url = download_url
-        self.mandatory = mandatory
-        self.md5hash = md5hash
-        self.product = product
-        self.vendor = vendor
-        self.summary = summary
-        self.size = size
-
-    def __str__(self) -> str:
-        return "Software(c='%s', v='%s', mandatory=%s, size=%d, path='%s')" % (
-            self.customisation,
-            self.version,
-            self.mandatory,
-            self.size,
-            self.download_url,
-        )
+    customisation: str | None = None
+    version: str | None = None
+    download_url: str | None = None
+    mandatory: bool = False
+    md5hash: str | None = None
+    product: str | None = None
+    size: int = 0
+    vendor: str = "Frontier Silicon"
+    summary: str | None = None
 
     def loadxml(self, element: xmltree.Element):
         """Imports data from the given XML-Element."""
-        if not element:
+        if element is None:
             return
         self.customisation = element.get("customisation")
         self.version = element.get("version")
         self.download_url = element.find("download").text
         self.mandatory = element.find("mandatory").text == "True"
         self.product = element.find("product").text
         self.size = int(element.find("size").text)
         self.md5hash = element.find("md5").text
         self.summary = element.find("summary").text
         self.vendor = element.find("vendor").text
 
 
+class UpdateError(Exception):
+    """Base class for general update related errors."""
+    pass
+
+
+class MalformedMACError(UpdateError):
+    """Raised if an invalid MAC address is passed."""
+
+
+class CustomisationError(UpdateError):
+    """Raised if an invalid customisation is passed."""
+    pass
+
+
+class VersionError(UpdateError):
+    """Raised if an invalid version is passed."""
+    pass
+
+
+class UpdateStatus(enum.IntEnum):
+    """Update status of an UpdateRequest."""
+
+    NOT_FOUND = 404
+    NOT_AVAILABLE = 304
+    FOUND = 200
+    ERROR = -1
+
+
+@dataclasses.dataclass
+class UpdateRequest:
+    """Small storage class for update requests.
+
+    Objects of this class can be utilized as follows:
+
+    >>> request = find_update(...)
+    >>> if request.has_update:
+    ...     updates = request.updates
+    ...
+    """
+
+    status: UpdateStatus | int = UpdateStatus.ERROR
+    updates: list[ISUSoftwareElement] = dataclasses.field(default_factory=list)
+    error: Exception | None = None
+
+    @property
+    def has_update(self) -> bool:
+        """Returns whether the request stores an actual :class:`ISUSoftwareElement`.
+
+        :return: whether the status is set to ``FOUND`` and there is no error
+        :rtype: bool
+        """
+        return self.status == UpdateStatus.FOUND and self.error is None
+
+
 ###############################################################################
 # Functions
 ###############################################################################
 def _url_find_update_add_parameters(url: str, parameters: dict) -> str:
     uri = "/FindUpdate.aspx?"
     return (
         url + uri + "&".join(["%s=%s" % (key, parameters[key]) for key in parameters])
     )
 
 
-def isu_find_update(
+def url_find_update(mac, customisation, version) -> str:
+    """Generates a new URL that can be used to query for newer software packages.
+
+    :param mac: the MAC address
+    :type mac: str
+    :param customisation: the device's customisation
+    :type customisation: str
+    :param version: the current firmware version
+    :type version: str
+    :return: the created URL
+    :rtype: str
+    """
+    return _url_find_update_add_parameters(
+        "https://" + ISU_FILE_PROVIDER_HOST,
+        {"mac": mac, "customisation": customisation, "version": version},
+    )
+
+
+def find_update(
     mac: str,
     customisation: str,
     version: str,
-    verbose: bool = False,
     netconfig: FSNetConfiguration = None,
-) -> dict:
+) -> UpdateRequest:
     """Tries to find updates for the given version and customisation.
 
     :param mac: The MAC-Address string of a frontier silicon device in the following
                 format: ``002261xxxxxx``. This string must start with ``002261``.
     :param customisation: Information about the used interface, module and version
                             number.
     :param version: As the name already states, the full version string.
-    :param verbose: if enabled/True, error messages will be printed to stdout
     :param netconfig: if a custom configuration like a proxy should be used, this
                         object can be passed as a parameter
 
-    :returns: ``None`` if an error occurred or a dictionary with the following structure
-                if one ore more updates are present::
-
-                    return {
-                        'update_present': bool,
-                        'headers': dict,
-                        'updates': list[ISUSoftwareElement]
-                    }
+    :returns: a new instance of an :class:`UpdateRequest` that stores any occurred errors.
     """
 
-    result = {"update_present": False, "headers": None, "updates": []}
+    result = UpdateRequest()
     if not re.match(RE_FSIR_MAC_ADDR, mac):
-        if verbose:
-            print("[-] Failed to find an update: malformed MAC-Address")
+        result.error = MalformedMACError(f"'{mac}' is not a valid FS MAC address.")
         return result
 
     if not re.match(RE_CUSTOMISATION, customisation):
-        if verbose:
-            print("[-] Failed to find an update: malformed customisation string")
+        result.error = CustomisationError(
+            f"Malformed customisation: '{customisation}' does not match r'{RE_CUSTOMISATION}'"
+        )
         return result
 
     if not re.match(RE_VERSION, version):
-        if verbose:
-            print("[-] Failed to find an update: malformed version string")
+        result.error = VersionError(
+            f"Malformed version string: '{version}' does not match r'{RE_VERSION}'"
+        )
         return result
 
-    url = _url_find_update_add_parameters(
-        "https://" + ISU_FILE_PROVIDER_HOST,
-        {"mac": mac, "customisation": customisation, "version": version},
-    )
-
-    if netconfig:
-        response = netconfig.delegate_request("GET", url, ISU_REQUEST_HEADERS)
-    else:
-        pool = urllib3.HTTPSConnectionPool(
-            host=ISU_FILE_PROVIDER_HOST, headers=ISU_REQUEST_HEADERS
-        )
-        response = pool.request("GET", url)
-        pool.close()
+    url = url_find_update(mac, customisation, version)
+    try:
+        if netconfig:
+            response = netconfig.delegate_request("GET", url, ISU_REQUEST_HEADERS)
+        else:
+            pool = urllib3.HTTPSConnectionPool(
+                host=ISU_FILE_PROVIDER_HOST, headers=ISU_REQUEST_HEADERS
+            )
+            response = pool.request("GET", url)
+            pool.close()
+    except urllib3.exceptions.PoolError as err:
+        result.error = err
+        return result
 
     if response.status == 404:
-        if verbose:
-            print("[-] Update not found: invalid version or customisation")
+        result.status = UpdateStatus.NOT_FOUND
         return result
     elif response.status == 304:
-        if verbose:
-            print("[-] No Update available for: ", customisation)
+        result.status = UpdateStatus.NOT_AVAILABLE
         return result
 
     if response.status != 200:
-        if verbose:
-            print("[-] Unexpected result code:", response.status)
+        result.status = UpdateStatus.ERROR
         return result
     else:
+        result.status = UpdateStatus.FOUND
         try:
-            result["headers"] = response.headers
             content = str(response.data, "utf-8")
-
+            # NOTE: The returned content is a HTML page with embedded
+            # XML data.
             pos = content.find("<?xml")
             if pos == -1:
-                if verbose:
-                    print("[-] Unexpected result: XML-Content missing")
+                result.status = UpdateStatus.ERROR
+                result.error = UpdateError("Could not find XML document!")
                 return result
             else:
                 content = content[pos : pos + content.find("</updates>", pos) + 9]
                 root = xmltree.fromstring(content)
                 updates = []
                 for software in root:
                     s = ISUSoftwareElement()
                     s.loadxml(software)
                     updates.append(s)
 
-                result["updates"] = updates
-                result["update_present"] = True
-                return result
-        except Exception as e:
-            if verbose:
-                print("[-] Error while parsing response: %s" % e)
-            return result
+                result.updates.extend(updates)
+        except Exception as err:
+            result.error = err
+
+        return result
 
 
-def isu_get_update(
+def get_update(
     path: str,
     url: str = None,
     software: ISUSoftwareElement = None,
-    verbose: bool = False,
     netconfig: FSNetConfiguration = None,
 ):
     """Tries to download and save the firmware binary located at the given URL.
 
     :param path: an absolute or relative path to the output file
     :param url: optional the direct download link - if not set, the software parameter
                 must be defined
     :param software: the software object containing the relevant data for downloading
                     the update file
-    :param verbose: if enabled/True, error messages will be printed to stdout
     :param netconfig: if a custom configuration like a proxy should be used, this object
                         can be passed as a parameter
     """
     if not url and (not software or not software.download_url):
-        if verbose:
-            print(
-                "[-] Invalid choice of parameters: either url or software has to be nonnull"
-            )
-        return
+        raise UpdateError(
+            "Invalid choice of parameters: either url or software has to be non null"
+        )
 
     url = url if url else software.download_url
-    if netconfig:
-        response = netconfig.delegate_request(
-            "GET", url, ISU_REQUEST_HEADERS, preload_content=False
-        )
-    else:
-        if "https" not in url:
-            url = url.replace("http", "https")
-        pool = urllib3.HTTPSConnectionPool(
-            host=url.split("/")[2], headers=ISU_REQUEST_HEADERS, timeout=5
-        )
-        response = pool.request("GET", url, preload_content=False)
+    try:
+        if netconfig:
+            response = netconfig.delegate_request(
+                "GET", url, ISU_REQUEST_HEADERS, preload_content=False
+            )
+        else:
+            if "https" not in url:
+                url = url.replace("http", "https")
+            pool = urllib3.HTTPSConnectionPool(
+                host=url.split("/")[2], headers=ISU_REQUEST_HEADERS, timeout=5
+            )
+            response = pool.request("GET", url, preload_content=False)
+    except urllib3.exceptions.PoolError as err:
+        raise UpdateError from err
 
     if response.status != 200:
-        if verbose:
-            print("[-] Unexpected result code:", response.status)
+        raise UpdateError(f"Unexpected result code: {response.status}")
     else:
         try:
             with open(path, "wb") as _res:
                 for chunk in response.stream(4096 * 16):
                     if chunk:
                         _res.write(chunk)
-        except TimeoutError:
-            print("[-] Timeout Error...")
+        except urllib3.exceptions.PoolError as err:
+            raise UpdateError from err
     response.release_conn()
 
 
-def isu_new_url(name: str) -> str:
+def url_get_update(name: str) -> str:
     """An URL generator for the given product descriptor.
 
-    :param name: the customisation and version put toghether wither with
-                a '`_V`'.
+    :param name: the customisation and version put toghether wither with a '`_V`'.
     :returns: the newly generated url where the firmware can be downloaded
     """
     parts = name.split("-")
     fs_part = None
     url = None
 
     # NOTE: Some firmware binaries contain different sub-interfaces, so
     # the FSXXXX module definition will be shifted to the right.
     for f in filter(lambda x: "FS" in x, parts):
         fs_part = f
         break
 
+    if fs_part is None:
+        # Venice 6 module will be inferred
+        fs_part = "FS2026"
+
     if fs_part is not None:
         if fs_part == "FS2340":
             customisation = name.split("_V")[0]
             url = "https://%s/srupdates/srupdates/%s/%s.isu.bin" % (
                 ISU_EDGE_PROVIDER_HOST,
                 customisation,
                 name,
```

### Comparing `fsapi-tools-1.0.0rc0/fsapi/isu/util.py` & `fsapi-tools-2.0.0/fsapi/isu/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,29 +74,32 @@
 
     def get_msg(self, style, *msg, end="") -> str:
         if self.colorized:
             return style + " ".join(list(msg)) + end
 
         return " ".join(list(msg))
 
+    def print_msg(self, style, *msg, end="") -> None:
+        print(self.get_msg(style, *msg, end=end))
+
     def get_format(self, name: str, value) -> str:
         result = value
         result_c = value
         indent = len(name) + self.indent
         if name in self.handlers:
             return self.handlers[name](value, colorized=self.colorized, indent=indent)
 
+        elif isinstance(value, (enum.Enum, enum.IntEnum, type)):
+            result = repr(value)
+            result_c = Fore.LIGHTCYAN_EX + result
+
         elif isinstance(value, (int, float)):
             result = str(value)
             result_c = Fore.LIGHTMAGENTA_EX + str(value)
 
-        elif isinstance(value, enum.IntEnum):
-            result = repr(value)
-            result_c = Fore.LIGHTCYAN_EX + result
-
         elif isinstance(value, str):
             result = pprint.pformat(value, indent=indent, width=125)
             result_c = Fore.YELLOW + result
 
         elif isinstance(value, bytes):
             try:
                 result = pprint.pformat(value.decode(), indent=indent, width=125)
```

### Comparing `fsapi-tools-1.0.0rc0/fsapi/netconfig.py` & `fsapi-tools-2.0.0/fsapi/netconfig.py`

 * *Files identical despite different names*

### Comparing `fsapi-tools-1.0.0rc0/fsapi/netremote/basenode.py` & `fsapi-tools-2.0.0/fsapi/net/_wrap.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,305 +15,276 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-__doc__ = """
-The first two classes, "NodePrototype" and "NodeArg", are used to add a prototype
-template to each node. By adding a "NodeArg" to a "NodePrototype" object, the same
-parameter has to be specified when calling the ``netremote_request('SET', ...)`` method.
-
-Here's a small example to illustrate its importance:
-
-.. code-block:: python
-    :linenos:
-
-    # <in specific Node class> -> do not change this code
-    # Creating a prototype for the default parameter 'value' of type ui16.
-    prototype = NodePrototype(arg=NodeArg(data_Type=ARG_TYPE_U16))
-
-    # <custom code>
-    # If calling the SET method, the parameter has to be given
-    result = fsapi.netremote_request('SET', node_class, radio, parameters={'value': 1})
-
-
-There are only a few ``ARG_TYPE`` values implemented and available for use. They are:
-
-- ``ARG_TYPE_C``:   int = ``0x10``, C8-Array (char array)
-- ``ARG_TYPE_E8``:  int = ``0x11``, Type defined by an Enum
-- ``ARG_TYPE_U8``:  int = ``0x12``, unsigned char
-- ``ARG_TYPE_U16``: int = ``0x13``, unsigned short
-- ``ARG_TYPE_U32``: int = ``0x14``, unsigned int
-- ``ARG_TYPE_S8``:  int = ``0x15``, signed char
-- ``ARG_TYPE_S16``: int = ``0x16``, signed short
-- ``ARG_TYPE_S32``: int = ``0x17``, signed int
-- ``ARG_TYPE_U``:   int = ``0x18``, array of data
-
-The node classes represent the foundation of all possible functionalities provided by
-this API. The package name of each node class can be obtained by calling the static method
-``node_class.get_name()``. You can use *fsapi.get_all_node_names()* to retrieve all
-implemented nodes.
-
-Each node provides the following attributes:
-
-- `cacheable` [bool],
-- `notifying` [bool],
-- `readonly` [bool],
-- <static> `package_name` [str],
-- `prototype` [NodePrototype],
-
-and the stored value in case the node is not a :class:`NodeList`. The node list classes simply
-contain a list of :class:`NodeListItem`, which can have one or more fields. These fields are
-packed into a dictionary named ``attr``.
-
-To simplify the import of NodeLists and NodeListItems, these classes come with an inbuilt
-function called `loadxml()`. Please note that the XMLElement always needs to be the root element.
-"""
-
-from xml.etree import ElementTree as xmltree
-
-__all__ = [
-    "ARG_TYPE_C",
-    "ARG_TYPE_E8",
-    "ARG_TYPE_U8",
-    "ARG_TYPE_U16",
-    "ARG_TYPE_U32",
-    "ARG_TYPE_S8",
-    "ARG_TYPE_S16",
-    "ARG_TYPE_S32",
-    "ARG_TYPE_U",
-    "NodeArg",
-    "NodePrototype",
-    "NodeInfo",
-    "NodeInteger",
-    "NodeS8",
-    "NodeS16",
-    "NodeS32",
-    "NodeU8",
-    "NodeU16",
-    "NodeU32",
-    "NodeE8",
-    "NodeC",
-    "NodeU",
-    "NodeListItem",
-    "NodeList",
-]
-
-ARG_TYPE_C: int = 0x10
-"""C8-Array (char array)"""
-ARG_TYPE_E8: int = 0x11
-"""Type defined by an Enum"""
-ARG_TYPE_U8: int = 0x12
-"""unsigned char"""
-ARG_TYPE_U16: int = 0x13
-"""unsigned short"""
-ARG_TYPE_U32: int = 0x14
-"""unsigned int"""
-ARG_TYPE_S8: int = 0x15
-"""signed char"""
-ARG_TYPE_S16: int = 0x16
-"""signed short"""
-ARG_TYPE_S32: int = 0x17
-"""signed int"""
-ARG_TYPE_U: int = 0x18
-"""array of data"""
-
-
-class NodeArg:
-    """A simple Node-Argument.
-
-    This class has to be added to the ``NodePrototype`` if the node can be altered. The
-    default name for an argument is "`value`".
-
-    :param name: the argument's name (default "`value`")
-    :param length: the maximum data length
-    :param data_type: one of the previous declared data types
-    """
-
-    def __init__(self, name: str = None, length: int = 0, data_type: int = 0) -> None:
-        self.name = name
-        self.length = length
-        self.data_type = data_type
-
-
-class NodePrototype:
-    """The prototype for a node definition.
-
-    This class stores the arguments that are necessary when reading from or writing to
-    a node.
-
-    :param arg: a single ``NodeArg``
-    :param args: a list of ``NodeArg``
-    """
-
-    def __init__(self, arg: NodeArg = None, args: list = None) -> None:
-        if arg:
-            self.arguments = [arg]
-        elif args:
-            self.arguments = args if args else []
-        else:
-            self.arguments = []
-
-    def get_args(self) -> list:
-        """Returns the stored node's arguments."""
-        return self.arguments
-
-    def __iter__(self):
-        return iter(self.arguments)
-
-
-class NodeInfo:
-    """The base class for all nodes.
-
-    As defined above, each node provides the following attributes:
-
-    - ``cacheable`` [bool],
-    - ``notifying`` [bool],
-    - ``readonly`` [bool],
-    - <static> ``package_name`` [str],
-    - ``prototype``[NodePrototype]
-
-    and the stored value in case the node is not a ``NodeList``.
-    """
+from __future__ import annotations
 
-    def is_cacheable(self) -> bool:
-        """Returns whether this node can be cached (on the device)."""
-        return False
+import typing as t
 
-    def is_notifying(self) -> bool:
-        """Returns whether this node is notifying."""
-        return False
+from .base import NodePath, NodeListItem, IntEnumValue
+from .device import FSDevice, Status
 
-    def is_readonly(self) -> bool:
-        """Returns whether this node can't be altered."""
-        return False
 
-    def get_name(self) -> str:
-        """Returns the name of this node."""
-        pass
+def wrap(device: FSDevice) -> _Wrapper:
+    """Creates a new API wrapper for the given device.
 
-    def get_prototype(self) -> NodePrototype:
-        """Returns the prototype for this node."""
-        pass
+    With the returned wrapper object, the most important nodes can be accessed
+    using simple attribute syntax:
 
-    def update(self):
-        """@Deprecated"""
-        pass
+    >>> device = FSDevice("127.0.0.1")
+    >>> api = wrap(device)
+    >>> name: str = api.friendly_name
 
+    Note that every access will fire an HTTP request to the desired target device.
+    It is also possible to use this method as a decorator (property is optionall):
 
-class NodeInteger(NodeInfo):
-    def __init__(self, value: int, min_value: int = 0, max_value: int = 0) -> None:
-        self.value = value
-        self.minimum = min_value
-        self.maximum = max_value
-
-    def get_value(self) -> int:
-        return self.value
-
-    def update(self):
-        if type(self.value) == str:
-            self.value = int(self.value)
-
-    def __str__(self) -> str:
-        return "NodeInt(v=%s)" % str(self.get_value())
-
-    def __eq__(self, __o: object) -> bool:
-        if isinstance(__o, self.__class__):
-            return __o.get_value() == self.get_value()
+    >>> class Foo:
+    ...    @wrap
+    ...    @property
+    ...    def api(self):
+    ...        return self.device
+    ...
 
+    :param device: the controller implementing the FSAPI
+    :type device: FSDevice
+    :return: a new API wrapper
+    :rtype: _Wrapper
+    """
+    return _Wrapper(device)
 
-class NodeS8(NodeInteger):
-    def __init__(self, value: int, max_size: int = 0) -> None:
-        super().__init__(value, 127, -127)
 
+# Internal type variable to enable static type checking
+_T = t.TypeVar("_T")
 
-class NodeS16(NodeInteger):
-    def __init__(self, value: int, max_size: int = 0) -> None:
-        super().__init__(value, 0x7FFF, -0x7FFF)
 
+class APICall(t.Generic[_T]):
+    """Generic API call using simple node definitions.
 
-class NodeS32(NodeInteger):
-    def __init__(self, value: int, max_size: int = 0) -> None:
-        super().__init__(value, 0x7FFFFFFF, -0x7FFFFFFF)
+    This class will enable checks during runtime that prevents changing immutable
+    values.
 
+    **Important:** This class is strongly typed. In order to enable static type checking
+    this class is annotated with a type variable.
 
-class NodeU8(NodeInteger):
-    def __init__(self, value: int, max_size: int = 0) -> None:
-        super().__init__(value, 0xFF, 0)
+    >>> class Foo:
+    ...     value: APICall[int] = APICall("foo.bar")
+    ...
+    >>> foo = Foo()
+    >>> foo.value
+    5
 
+    :param node_path: the node's path
+    :type node_path: str
+    """
 
-class NodeU16(NodeInteger):
-    def __init__(self, value: int, max_size: int = 0) -> None:
-        super().__init__(value, 0xFFFF, 0)
+    def __init__(self, node_path: str) -> None:
+        self.node_path = NodePath(node_path)
 
+    def __get__(self, __instance: t.Any, __owner: type | None = None) -> _T:
+        return self.get(__instance)
 
-class NodeU32(NodeInteger):
-    def __init__(self, value: int, max_size: int = 0) -> None:
-        super().__init__(value, 0xFFFFFFFF, 0)
+    def __set__(self, __instance: t.Any, __value: _T) -> None:
+        self.put(__instance, __value)
 
+    def get(self, wrapper: _Wrapper) -> _T | None:
+        """Returns the value for the linked node.
+
+        :param wrapper: the API wrapper instance
+        :type wrapper: _Wrapper
+        :return: the fetched value or None if an error occurred
+        :rtype: _T | None
+        """
+        response = wrapper.device.get(self.node_path)
+        if response.status == Status.FS_OK:
+            return response.node.value
+        # REVISIT: maybe raise an exception
+        return None
+
+    def put(self, wrapper: _Wrapper, value: _T) -> None:
+        """Sets a new value for the linked node.
+
+        :param wrapper: the API wrapper instance
+        :type wrapper: _Wrapper
+        :param value: the new value to be applied
+        :type value: _T
+        :raises AttributeError: if the linked node is readonly
+        """
+        cls = self.node_path.get_node_type()
+        if cls.readonly:
+            # REVISIT: maybe don't throw an exception here
+            raise AttributeError(f"Node '{cls.path}' is immutable!")
+
+        wrapper.device.put(self.node_path, value=value)
+
+
+class ListAPICall(APICall[list[NodeListItem]]):
+    """Representation for a list API call.
+
+    This class behaves differently compared to standard API call variables
+    as it fetches more than one item and can take query arguments.
+
+    >>> api = wrap(device)
+    >>> api.ls_eqpresets(_pos=2, max_items=3)
+    [...]
 
-class NodeE8(NodeInfo):
-    def __init__(self, value: int = 0, mapping: dict = None) -> None:
-        self.value = value
-        self.mapping = mapping
+    - ``_pos``: the starting index position within the list (-1 for all items)
+    - ``max_items``: the number of items that should be returned
+    """
 
-    def get_enum_value(self) -> object:
-        if not self.mapping or self.value not in self.mapping:
+    def __init__(self, node_path: str) -> None:
+        super().__init__(node_path)
+        self.__instance = None
+
+    def __get__(self, __instance: t.Any, __owner: type | None = None) -> ListAPICall:
+        self.__instance = __instance
+        return self
+
+    def __call__(self, _pos=-1, max_items=0xFFFF, **argv) -> list[NodeListItem] | None:
+        argv["_pos"] = _pos
+        argv["maxItems"] = max_items
+        return self.get(self.__instance, **argv)
+
+    def get(self, wrapper: _Wrapper, **argv) -> list[NodeListItem] | None:
+        """Returns a list of items.
+
+        :param wrapper: the api wrapper instance
+        :type wrapper: _Wrapper
+        :return: the list returned by the device
+        :rtype: list[NodeListItem] | None
+        """
+        response = wrapper.device.list_get_next(self.node_path, **argv)
+        if response.status != Status.FS_OK:
             return None
-        return self.mapping[self.value]
 
-    def get_value(self) -> int:
-        return self.value
+        return list(response.node)
 
-    def __str__(self) -> str:
-        return f"NodeE8<{self.get_enum_value()}>"
+    def put(self, wrapper: _Wrapper, value: int) -> None:
+        """Selects an item within the context of this list node.
 
+        :param wrapper: the API wrapper instance
+        :type wrapper: _Wrapper
+        :param value: the key of an item (index position)
+        :type value: int
+        :raises TypeError: if the provided value is not an integer
+        """
+        if not isinstance(value, int):
+            raise TypeError(f"Expected int value - got {type(value)}")
 
-class NodeC(NodeInfo):
-    def __init__(self, value: str = None, max_size: int = 0) -> None:
-        super().__init__()
-        self.value = value
-        self.max_size = max_size
+        return super().put(wrapper, value)
 
-    def get_maximum_length(self) -> int:
-        return self.max_size
 
+# Internal wrapper fro api call classes
+_ac = APICall
+_lac = ListAPICall
 
-class NodeU(NodeC):
-    def __init__(self, value: str = None, max_size: int = 0) -> None:
-        super().__init__(value, max_size)
+# TODO: add multiroom and spotify support
+class _Wrapper:
+    """Web FSAPI wrapper class.
 
+    This class stores the most common nodes to control devices using the
+    FSAPI. Standard nodes can be accessed via attribute access and list
+    nodes should be handled differently. List nodes start with ``ls_``.
 
-class NodeListItem:
-    def __init__(self, attributes: dict = None) -> None:
-        self.attr = attributes if attributes else {}
+    Instances of this class can be retrieved by calling the exported ``wrap()``
+    method:
 
-    def loadxml(self, element: xmltree.Element):
-        key = element.get("key", None)
-        self.attr["key"] = key
-        for field_node in element.findall("field"):
-            self.attr[field_node.attrib["name"]] = field_node[0].text
+    >>> device = FSDevice("127.0.0.1")
+    >>> api = wrap(device)
 
-    def get_attr_by_name(self, field: str) -> object:
-        if not field or field not in self.attr:
-            return None
-        return self.attr[field]
+    Standard nodes can be accessed and controlled with ease:
 
+    >>> api.friendly_name
+    'MEDION'
+    >>> api.volume
+    3
+    >>> api.friendly_name = "MEDION2"
+    >>> api.friendly_name
+    'MEDION2'
 
-class NodeList(NodeInfo):
-    def __init__(self, items: list = None) -> None:
-        super().__init__()
-        self.items = items if items else []
+    Inaccessable nodes or blocked nodes will return a ``None`` value and immutable
+    nodes will raise an AttributeError on modification. List nodes behave special:
 
-    def loadxml(self, element: xmltree.Element):
-        for item in element.findall("item"):
-            node_item = NodeListItem()
-            node_item.loadxml(item)
-            self.get_items().append(node_item)
+    >>> api.ls_eqpresets(_pos=4)
+    [...]
+    >>> api.ls_eqpresets = 1
+
+    Use the assignment to select an item and the function call operator to query
+    a range of items.
+    """
 
-    def size(self) -> int:
-        return len(self.items)
+    def __init__(self, device: FSDevice) -> None:
+        self.__device = device
 
-    def get_items(self) -> list:
-        return self.items
+    @property
+    def device(self) -> FSDevice:
+        """The linked device"""
+        if isinstance(self.__device, property):
+            return self.__device.fget()
+        elif isinstance(self.__device, t.Callable):
+            return self.__device()
+        return self.__device
+
+    def get_field(self, name: str) -> APICall | ListAPICall:
+        """Returns a field of this instance named by the provided string.
+
+        :param name: the field's name
+        :type name: str
+        :return: the api call wrapper instance
+        :rtype: APICall | ListAPICall
+        """
+        return getattr(self, name)
+
+    # Standard API nodes
+    friendly_name: _ac[str]     = APICall("netRemote.sys.info.friendlyName")
+    dmr_uuid: _ac[str]          = APICall("netRemote.sys.info.dmruuid")
+    radio_id: _ac[str]          = APICall("netRemote.sys.info.radioId")
+    radio_pin: _ac[str]         = APICall("netRemote.sys.info.radioPin")
+    serial_number: _ac[str]     = APICall("netRemote.sys.info.serialNumber")
+    version: _ac[str]           = APICall("netRemote.sys.info.version")
+    build_version: _ac[str]     = APICall("netRemote.sys.info.buildVersion")
+    model_name: _ac[str]        = APICall("netRemote.sys.info.modelName")
+    mode: _ac[int]              = APICall("netRemote.sys.mode")
+    commit_changes: _ac[int]    = APICall("netRemote.sys.net.commitChanges")
+    lang: _ac[int]              = APICall("netRemote.sys.lang")
+    volume: _ac[int]            = APICall("netRemote.sys.audio.volume")
+    mute: _ac[int]              = APICall("netRemote.sys.audio.mute")
+    eq_preset: _ac[int]         = APICall("netRemote.sys.audio.eqPreset")
+    eq_loudness: _ac[int]       = APICall("netRemote.sys.audio.eqLoudness")
+    eq_custom_bass: _ac[int]    = APICall("netRemote.sys.audio.eqCustom.param0")
+    eq_custom_trible: _ac[int]  = APICall("netRemote.sys.audio.eqCustom.param1")
+    nav_num_items: _ac[int]     = APICall("netRemote.nav.numItems")
+    play_rate: _ac[int]         = APICall("netRemote.play.rate")
+    play_position: _ac[int]     = APICall("netRemote.play.position")
+    frequency: _ac[int]         = APICall("netRemote.play.frequency")
+    freq_upper_bound: _ac[int]  = APICall("netRemote.sys.caps.fmFreqRange.upper")
+    freq_lower_bound: _ac[int]  = APICall("netRemote.sys.caps.fmFreqRange.lower")
+    active_session: _ac[int]    = APICall("netRemote.sys.info.activeSession")
+    trace_level: _ac[int]       = APICall("netRemote.misc.debug.traceLevel")
+
+    delete_incident_report: _ac[int] = APICall("netRemote.debug.incidentReport.delete")
+    create_incident_report: _ac[int] = APICall("netRemote.debug.incidentReport.create")
+    last_incident_report: _ac[int]   = APICall("netRemote.debug.incidentReport.lastCreatedKey")
+
+    power: _ac[IntEnumValue] = APICall("netRemote.sys.power")
+    factory_reset: _ac[IntEnumValue] = APICall("netRemote.sys.factoryReset")
+    nav_state: _ac[IntEnumValue] = APICall("netRemote.nav.state")
+    nav_status: _ac[IntEnumValue] = APICall("netRemote.nav.status")
+    play_control: _ac[IntEnumValue] = APICall("netRemote.play.control")
+    play_repeat: _ac[IntEnumValue] = APICall("netRemote.play.repeat")
+    play_shuffle: _ac[IntEnumValue] = APICall("netRemote.play.shuffle")
+    shuffle_status: _ac[IntEnumValue] = APICall("netRemote.play.shuffleStatus")
+    play_status: _ac[IntEnumValue] = APICall("netRemote.play.status")
+
+    # List API nodes
+    ls_eqpresets: _lac = ListAPICall("netRemote.sys.caps.eqPresets")
+    ls_valid_modes: _lac = ListAPICall("netRemote.sys.caps.validModes")
+    ls_nav_list: _lac = ListAPICall("netRemote.nav.list")
+    ls_presets: _lac = ListAPICall("netRemote.nav.presets")
+    ls_dab_freqs: _lac = ListAPICall("netRemote.sys.caps.dabFreqList")
+    ls_eqbands: _lac = ListAPICall("netRemote.sys.caps.eqBands")
+    ls_incident_reports: _lac = ListAPICall("netRemote.debug.incidentReport.list")
+    ls_clock_sources: _lac = ListAPICall("netRemote.sys.caps.clockSourceList")
+    ls_languages: _lac = ListAPICall("netRemote.sys.caps.validLang")
+    ls_: _lac = ListAPICall("netRemote.sys.caps.clockSourceList")
```

### Comparing `fsapi-tools-1.0.0rc0/fsapi_tools.egg-info/PKG-INFO` & `fsapi-tools-2.0.0/fsapi_tools.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsapi-tools
-Version: 1.0.0rc0
+Version: 2.0.0
 Summary: Frontier Smart Firmware Tools and FSAPI Implementation.
 Author-email: MatrixEditor <not@supported.com>
 Project-URL: Homepage, https://github.com/MatrixEditor/frontier-smart-api
 Project-URL: API-Docs, https://matrixeditor.github.io/frontier-smart-api/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div id="top"></div>
 <div align="center">
 
-![logo](docs/graphics/company_logo.png)
+![Company logo would be displayed here.](docs/graphics/company_logo.png)
 
 </div>
 
 # Frontier Smart API and Firmware Tools
 
 [![python](https://img.shields.io/badge/python-3.7+-blue.svg?logo=python&labelColor=grey)](https://www.python.org/downloads/)
 ![Codestyle](https://img.shields.io:/static/v1?label=Codestyle&message=black&color=black)
@@ -165,28 +165,41 @@
 ```
 
 ### NET - FSAPI
 
 This small tool can be utilized to interact with Frontier Smart devices via CLI.
 
 ```bash
-$ fsapi-net set -n sys.info.friendlyName --args value:MedionIR $IP_ADDRESS
-[+] fsapiResponse of netRemote.sys.info.friendlyName:
-    - status: FS_OK
-
-$ fsapi-net get -n sys.info.friendlyName $IP_ADDRESS
-[+] fsapiResponse of netRemote.sys.info.friendlyName:
-    - status: FS_OK
-    - value: MedionIR
-    - readonly: False
-    - notifying: True
+$ fsapi-ctl set netremote.sys.info.friendlyName "MedionIR" 127.0.0.1
+> FSResponse('netRemote.sys.info.friendlyName', <Method.SET: 'SET'>)
+    - status: <Status.FS_OK: 'FS_OK'>
+
+$ fsapi-ctl get netremote.sys.info.friendlyName 127.0.0.1
+> FSResponse('netRemote.sys.info.friendlyName', <Method.GET: 'GET'>)
+    - status: <Status.FS_OK: 'FS_OK'>
+    - value: 'Hello World'
 
-$ fsapi-net isu --find $IP_ADDRESS
+$ fsapi-ctl -X update fetch 127.0.0.1 .
 [+] Generating current URL...
-    - url: https://update.wifiradiofrontier.com/Update.aspx?f=/updates/ir-mmi-FS2026-0500-0549.2.12.25c.EX72088-1A12.isu.bin
+    > URL: 'https://update.wifiradiofrontier.com/Update.aspx?f=/updates/ir-mmi-FS2026-0500-0549.2.12.25c.EX72088-1A12.isu.bin'
+
+$ fsapi-ctl view netremote.sys.power
+> SYS: Power (netRemote_sys_power_nt):
+    - path: 'netRemote.sys.power'
+    - readonly: False
+    - cacheable: True
+    - notifying: True
+    - type: <class 'fsapi.net.base.NodeE8'>
+    - prototype:
+        [0] => 'value'
+            - length: 1
+            - type: <ArgType.ARG_TYPE_E8: 17>
+    - enum values:
+        [0] => 'OFF'
+        [1] => 'ON'
 ```
 
 ## Usage Examples
 
 ### ISU API
 
 ```python
@@ -198,42 +211,59 @@
 pp = DataclassPrinter()
 pp.print_object(isu.header)
 ```
 
 ## FSAPI
 
 ```python
-from fsapi.netremote import Set, Get, ListGetNext, nodes, FSDevice
-from fsapi.netconfig import FSNetConfiguration
-from fsapi.isu import isu_find_update, isu_new_url, isu_get_update
+from fsapi.net import FSDevice, wrap, nodes
+
+# First, create the radio object
+device = FSDevice("127.0.0.1")
+
+# Create a new session id (only one at a time)
+device.new_session()
+
+# In order to simplify the usage of the FSDevice class
+api = wrap(device)
+friendly_name = api.friendly_name
+# or manually
+response = device.get(nodes / "netRemote.sys.info.friendlyName")
+if response.status == FS_OK:
+    #_ Again, type(content) = nodes.BaseSysInfoFriendlyName
+    friendly_name = response.content.value
+
+    # Apply a new name via wrapper
+    api.friendly_name = "FooBar"
+    # or manually
+    device.put(nodes / "netRemote.sys.info.friendlyName", value="FooBar")
+
+# get all elements of a list
+valid_modes = api.ls_valid_modes()
+# get a certain amount of elements beginning at index 3
+valid_mpdes = api.ls_valid_modes(_pos=3, max_items=10)
+```
+
+## Software Update
+
+```python
+from fsapi.isu import find_update, url_get_update, get_update
 
 # 1.Find and download updates
 # without custom netconfig -> HTTPS traffic
-response = isu_find_update('$MAC', '$CUSTOM', '$VERSION')
+request = find_update('$MAC', '$CUSTOM', '$VERSION')
 
 # with custom config -> force HTTP traffic
 config = FSNetConfiguration(http_pool=urllib3.HTTPConnectionPool('$HOST'))
-response = isu_find_update('$MAC', '$CUSTOM', '$VERSION', netconfig=config)
+request = find_update('$MAC', '$CUSTOM', '$VERSION', netconfig=config)
 
 # without custom netconfig -> HTTPS traffic
-response = isu_find_update('$MAC', '$CUSTOM', '$VERSION')
-for _software in response['updates']:
-   isu_get_update('$FILE_PATH', software=_software)
-
-# First, create the device:
-device = FSDevice("127.0.0.1")
-
-# SET request
-result = Set(nodes.BaseSysInfoFriendlyName, device, value="Hello World")
-
-# GET request
-result = Get(nodes.BaseSysInfoFriendlyName, device)
-
-# LIST_GET_NEXT request
-result = ListGetNext(nodes.NODECLASS, device, maxItems=100)
+if request.has_update:
+    for _software in request.updates:
+        get_update('$FILE_PATH', software=_software)
 ```
 
 ## Contributing
 
 Contributions are highly appreciated as they contribute to the growth and improvement of the open-source community. If you have any suggestions that could enhance this project, please feel free to fork the repository and create a pull request. Alternatively, you can also open an issue with the "enhancement" tag.
 
 To contribute, follow these steps:
```

### Comparing `fsapi-tools-1.0.0rc0/pyproject.toml` & `fsapi-tools-2.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 00000000: 5b70 726f 6a65 6374 5d0d 0a6e 616d 6520  [project]..name 
 00000010: 3d20 2266 7361 7069 2d74 6f6f 6c73 220d  = "fsapi-tools".
-00000020: 0a76 6572 7369 6f6e 203d 2022 312e 302e  .version = "1.0.
-00000030: 302d 7263 220d 0a64 6573 6372 6970 7469  0-rc"..descripti
-00000040: 6f6e 3d22 4672 6f6e 7469 6572 2053 6d61  on="Frontier Sma
-00000050: 7274 2046 6972 6d77 6172 6520 546f 6f6c  rt Firmware Tool
-00000060: 7320 616e 6420 4653 4150 4920 496d 706c  s and FSAPI Impl
-00000070: 656d 656e 7461 7469 6f6e 2e22 0d0a 6175  ementation."..au
-00000080: 7468 6f72 7320 3d20 5b0d 0a20 207b 206e  thors = [..  { n
-00000090: 616d 653d 224d 6174 7269 7845 6469 746f  ame="MatrixEdito
-000000a0: 7222 2c20 656d 6169 6c3d 226e 6f74 4073  r", email="not@s
-000000b0: 7570 706f 7274 6564 2e63 6f6d 2220 7d2c  upported.com" },
-000000c0: 0d0a 5d0d 0a72 6561 646d 6520 3d20 2252  ..]..readme = "R
-000000d0: 4541 444d 452e 6d64 220d 0a63 6c61 7373  EADME.md"..class
-000000e0: 6966 6965 7273 203d 205b 0d0a 2020 2020  ifiers = [..    
-000000f0: 2744 6576 656c 6f70 6d65 6e74 2053 7461  'Development Sta
-00000100: 7475 7320 3a3a 2035 202d 2050 726f 6475  tus :: 5 - Produ
-00000110: 6374 696f 6e2f 5374 6162 6c65 272c 0d0a  ction/Stable',..
-00000120: 2020 2020 2749 6e74 656e 6465 6420 4175      'Intended Au
-00000130: 6469 656e 6365 203a 3a20 5363 6965 6e63  dience :: Scienc
-00000140: 652f 5265 7365 6172 6368 272c 0d0a 2020  e/Research',..  
-00000150: 2020 274c 6963 656e 7365 203a 3a20 4f53    'License :: OS
-00000160: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
-00000170: 5420 4c69 6365 6e73 6527 2c0d 0a20 2020  T License',..   
-00000180: 2027 5072 6f67 7261 6d6d 696e 6720 4c61   'Programming La
-00000190: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000001a0: 203a 3a20 332e 3627 2c0d 0a20 2020 2027   :: 3.6',..    '
-000001b0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000001c0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000001d0: 3a20 332e 3727 2c0d 0a20 2020 2027 5072  : 3.7',..    'Pr
-000001e0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000001f0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000200: 332e 3827 2c0d 0a20 2020 2027 5072 6f67  3.8',..    'Prog
-00000210: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000220: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000230: 3927 2c0d 0a20 2020 2027 5072 6f67 7261  9',..    'Progra
-00000240: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000250: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
-00000260: 272c 0d0a 2020 5d0d 0a0d 0a5b 7072 6f6a  ',..  ]....[proj
-00000270: 6563 742e 7572 6c73 5d0d 0a22 486f 6d65  ect.urls].."Home
-00000280: 7061 6765 2220 3d20 2268 7474 7073 3a2f  page" = "https:/
-00000290: 2f67 6974 6875 622e 636f 6d2f 4d61 7472  /github.com/Matr
-000002a0: 6978 4564 6974 6f72 2f66 726f 6e74 6965  ixEditor/frontie
-000002b0: 722d 736d 6172 742d 6170 6922 0d0a 2241  r-smart-api".."A
-000002c0: 5049 2d44 6f63 7322 203d 2022 6874 7470  PI-Docs" = "http
-000002d0: 733a 2f2f 6d61 7472 6978 6564 6974 6f72  s://matrixeditor
-000002e0: 2e67 6974 6875 622e 696f 2f66 726f 6e74  .github.io/front
-000002f0: 6965 722d 736d 6172 742d 6170 692f 220d  ier-smart-api/".
-00000300: 0a0d 0a5b 7072 6f6a 6563 742e 7363 7269  ...[project.scri
-00000310: 7074 735d 0d0a 6973 7574 6f6f 6c20 3d20  pts]..isutool = 
-00000320: 2266 7361 7069 2e69 7375 2e63 6c69 3a6d  "fsapi.isu.cli:m
-00000330: 6169 6e22 0d0a 6673 6170 692d 7864 7220  ain"..fsapi-xdr 
-00000340: 3d20 2266 7361 7069 2e65 636d 6173 6372  = "fsapi.ecmascr
-00000350: 6970 742e 636c 693a 6d61 696e 220d 0a66  ipt.cli:main"..f
-00000360: 7361 7069 2d6e 6574 203d 2022 6673 6170  sapi-net = "fsap
-00000370: 692e 6e65 7472 656d 6f74 652e 636c 693a  i.netremote.cli:
-00000380: 6d61 696e 220d 0a0d 0a5b 746f 6f6c 2e73  main"....[tool.s
-00000390: 6574 7570 746f 6f6c 732e 7061 636b 6167  etuptools.packag
-000003a0: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
-000003b0: 3d20 5b22 2e22 5d0d 0a69 6e63 6c75 6465  = ["."]..include
-000003c0: 203d 205b 2266 7361 7069 2a22 5d          = ["fsapi*"]
+00000020: 0a76 6572 7369 6f6e 203d 2022 322e 302e  .version = "2.0.
+00000030: 3022 0d0a 6465 7363 7269 7074 696f 6e3d  0"..description=
+00000040: 2246 726f 6e74 6965 7220 536d 6172 7420  "Frontier Smart 
+00000050: 4669 726d 7761 7265 2054 6f6f 6c73 2061  Firmware Tools a
+00000060: 6e64 2046 5341 5049 2049 6d70 6c65 6d65  nd FSAPI Impleme
+00000070: 6e74 6174 696f 6e2e 220d 0a61 7574 686f  ntation."..autho
+00000080: 7273 203d 205b 0d0a 2020 7b20 6e61 6d65  rs = [..  { name
+00000090: 3d22 4d61 7472 6978 4564 6974 6f72 222c  ="MatrixEditor",
+000000a0: 2065 6d61 696c 3d22 6e6f 7440 7375 7070   email="not@supp
+000000b0: 6f72 7465 642e 636f 6d22 207d 2c0d 0a5d  orted.com" },..]
+000000c0: 0d0a 7265 6164 6d65 203d 2022 5245 4144  ..readme = "READ
+000000d0: 4d45 2e6d 6422 0d0a 636c 6173 7369 6669  ME.md"..classifi
+000000e0: 6572 7320 3d20 5b0d 0a20 2020 2027 4465  ers = [..    'De
+000000f0: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
+00000100: 203a 3a20 3520 2d20 5072 6f64 7563 7469   :: 5 - Producti
+00000110: 6f6e 2f53 7461 626c 6527 2c0d 0a20 2020  on/Stable',..   
+00000120: 2027 496e 7465 6e64 6564 2041 7564 6965   'Intended Audie
+00000130: 6e63 6520 3a3a 2053 6369 656e 6365 2f52  nce :: Science/R
+00000140: 6573 6561 7263 6827 2c0d 0a20 2020 2027  esearch',..    '
+00000150: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+00000160: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
+00000170: 6963 656e 7365 272c 0d0a 2020 2020 2750  icense',..    'P
+00000180: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000190: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000001a0: 2033 2e36 272c 0d0a 2020 2020 2750 726f   3.6',..    'Pro
+000001b0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000001c0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000001d0: 2e37 272c 0d0a 2020 2020 2750 726f 6772  .7',..    'Progr
+000001e0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000001f0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
+00000200: 272c 0d0a 2020 2020 2750 726f 6772 616d  ',..    'Program
+00000210: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000220: 2050 7974 686f 6e20 3a3a 2033 2e39 272c   Python :: 3.9',
+00000230: 0d0a 2020 2020 2750 726f 6772 616d 6d69  ..    'Programmi
+00000240: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000250: 7974 686f 6e20 3a3a 2033 2e31 3027 2c0d  ython :: 3.10',.
+00000260: 0a20 205d 0d0a 0d0a 5b70 726f 6a65 6374  .  ]....[project
+00000270: 2e75 726c 735d 0d0a 2248 6f6d 6570 6167  .urls].."Homepag
+00000280: 6522 203d 2022 6874 7470 733a 2f2f 6769  e" = "https://gi
+00000290: 7468 7562 2e63 6f6d 2f4d 6174 7269 7845  thub.com/MatrixE
+000002a0: 6469 746f 722f 6672 6f6e 7469 6572 2d73  ditor/frontier-s
+000002b0: 6d61 7274 2d61 7069 220d 0a22 4150 492d  mart-api".."API-
+000002c0: 446f 6373 2220 3d20 2268 7474 7073 3a2f  Docs" = "https:/
+000002d0: 2f6d 6174 7269 7865 6469 746f 722e 6769  /matrixeditor.gi
+000002e0: 7468 7562 2e69 6f2f 6672 6f6e 7469 6572  thub.io/frontier
+000002f0: 2d73 6d61 7274 2d61 7069 2f22 0d0a 0d0a  -smart-api/"....
+00000300: 5b70 726f 6a65 6374 2e73 6372 6970 7473  [project.scripts
+00000310: 5d0d 0a69 7375 746f 6f6c 203d 2022 6673  ]..isutool = "fs
+00000320: 6170 692e 6973 752e 636c 693a 6d61 696e  api.isu.cli:main
+00000330: 220d 0a66 7361 7069 2d78 6472 203d 2022  "..fsapi-xdr = "
+00000340: 6673 6170 692e 6563 6d61 7363 7269 7074  fsapi.ecmascript
+00000350: 2e63 6c69 3a6d 6169 6e22 0d0a 6673 6170  .cli:main"..fsap
+00000360: 692d 6374 6c20 3d20 2266 7361 7069 2e6e  i-ctl = "fsapi.n
+00000370: 6574 2e63 6c69 3a6d 6169 6e22 0d0a 0d0a  et.cli:main"....
+00000380: 5b74 6f6f 6c2e 7365 7475 7074 6f6f 6c73  [tool.setuptools
+00000390: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
+000003a0: 0a77 6865 7265 203d 205b 222e 225d 0d0a  .where = ["."]..
+000003b0: 696e 636c 7564 6520 3d20 5b22 6673 6170  include = ["fsap
+000003c0: 692a 225d                                i*"]
```

