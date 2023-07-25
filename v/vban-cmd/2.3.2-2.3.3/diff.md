# Comparing `tmp/vban_cmd-2.3.2.tar.gz` & `tmp/vban_cmd-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vban_cmd-2.3.2.tar", max compression
+gzip compressed data, was "vban_cmd-2.3.3.tar", max compression
```

## Comparing `vban_cmd-2.3.2.tar` & `vban_cmd-2.3.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1091 2022-03-24 12:30:28.474287 vban_cmd-2.3.2/LICENSE
--rw-r--r--   0        0        0      951 2023-07-12 08:49:24.959188 vban_cmd-2.3.2/pyproject.toml
--rw-r--r--   0        0        0    12527 2023-07-11 18:49:38.369576 vban_cmd-2.3.2/README.md
--rw-r--r--   0        0        0       70 2022-07-12 16:30:51.963399 vban_cmd-2.3.2/vban_cmd/__init__.py
--rw-r--r--   0        0        0     5276 2023-06-25 10:36:16.654167 vban_cmd-2.3.2/vban_cmd/bus.py
--rw-r--r--   0        0        0     1127 2023-06-25 10:36:19.263212 vban_cmd-2.3.2/vban_cmd/command.py
--rw-r--r--   0        0        0     5855 2023-07-11 17:23:11.340063 vban_cmd-2.3.2/vban_cmd/config.py
--rw-r--r--   0        0        0      197 2023-06-25 10:36:23.500662 vban_cmd-2.3.2/vban_cmd/error.py
--rw-r--r--   0        0        0     1621 2023-06-22 09:26:30.424951 vban_cmd-2.3.2/vban_cmd/event.py
--rw-r--r--   0        0        0     6902 2023-07-08 06:42:16.984039 vban_cmd-2.3.2/vban_cmd/factory.py
--rw-r--r--   0        0        0     4115 2023-07-05 18:08:51.113607 vban_cmd-2.3.2/vban_cmd/iremote.py
--rw-r--r--   0        0        0     2202 2023-07-12 04:34:54.220984 vban_cmd-2.3.2/vban_cmd/kinds.py
--rw-r--r--   0        0        0     1150 2023-07-08 06:13:52.713834 vban_cmd-2.3.2/vban_cmd/macrobutton.py
--rw-r--r--   0        0        0     2992 2023-06-25 10:36:33.230612 vban_cmd-2.3.2/vban_cmd/meta.py
--rw-r--r--   0        0        0     9644 2023-06-25 14:59:01.896621 vban_cmd-2.3.2/vban_cmd/packet.py
--rw-r--r--   0        0        0    10137 2023-06-25 12:32:36.307607 vban_cmd-2.3.2/vban_cmd/strip.py
--rw-r--r--   0        0        0     2277 2023-06-25 10:36:40.287522 vban_cmd-2.3.2/vban_cmd/subject.py
--rw-r--r--   0        0        0     2525 2023-07-12 03:46:12.026345 vban_cmd-2.3.2/vban_cmd/util.py
--rw-r--r--   0        0        0     5996 2023-07-12 09:23:28.333915 vban_cmd-2.3.2/vban_cmd/vban.py
--rw-r--r--   0        0        0     7391 2023-07-12 03:47:07.637840 vban_cmd-2.3.2/vban_cmd/vbancmd.py
--rw-r--r--   0        0        0     6905 2023-06-25 14:54:55.684238 vban_cmd-2.3.2/vban_cmd/worker.py
--rw-r--r--   0        0        0    12664 1970-01-01 00:00:00.000000 vban_cmd-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-03-24 12:30:28.474287 vban_cmd-2.3.3/LICENSE
+-rw-r--r--   0        0        0      951 2023-07-25 15:22:56.363154 vban_cmd-2.3.3/pyproject.toml
+-rw-r--r--   0        0        0    12875 2023-07-15 07:15:00.451610 vban_cmd-2.3.3/README.md
+-rw-r--r--   0        0        0       70 2022-07-12 16:30:51.963399 vban_cmd-2.3.3/vban_cmd/__init__.py
+-rw-r--r--   0        0        0     5276 2023-06-25 10:36:16.654167 vban_cmd-2.3.3/vban_cmd/bus.py
+-rw-r--r--   0        0        0     1127 2023-06-25 10:36:19.263212 vban_cmd-2.3.3/vban_cmd/command.py
+-rw-r--r--   0        0        0     5855 2023-07-11 17:23:11.340063 vban_cmd-2.3.3/vban_cmd/config.py
+-rw-r--r--   0        0        0      197 2023-06-25 10:36:23.500662 vban_cmd-2.3.3/vban_cmd/error.py
+-rw-r--r--   0        0        0     1621 2023-06-22 09:26:30.424951 vban_cmd-2.3.3/vban_cmd/event.py
+-rw-r--r--   0        0        0     6902 2023-07-08 06:42:16.984039 vban_cmd-2.3.3/vban_cmd/factory.py
+-rw-r--r--   0        0        0     4130 2023-07-25 14:58:38.295129 vban_cmd-2.3.3/vban_cmd/iremote.py
+-rw-r--r--   0        0        0     2418 2023-07-25 14:54:48.277200 vban_cmd-2.3.3/vban_cmd/kinds.py
+-rw-r--r--   0        0        0     1158 2023-07-25 15:00:05.263943 vban_cmd-2.3.3/vban_cmd/macrobutton.py
+-rw-r--r--   0        0        0     2992 2023-06-25 10:36:33.230612 vban_cmd-2.3.3/vban_cmd/meta.py
+-rw-r--r--   0        0        0     9625 2023-07-25 14:57:29.669770 vban_cmd-2.3.3/vban_cmd/packet.py
+-rw-r--r--   0        0        0    10137 2023-06-25 12:32:36.307607 vban_cmd-2.3.3/vban_cmd/strip.py
+-rw-r--r--   0        0        0     2277 2023-06-25 10:36:40.287522 vban_cmd-2.3.3/vban_cmd/subject.py
+-rw-r--r--   0        0        0     2525 2023-07-12 03:46:12.026345 vban_cmd-2.3.3/vban_cmd/util.py
+-rw-r--r--   0        0        0     5996 2023-07-12 09:23:28.333915 vban_cmd-2.3.3/vban_cmd/vban.py
+-rw-r--r--   0        0        0     7391 2023-07-12 03:47:07.637840 vban_cmd-2.3.3/vban_cmd/vbancmd.py
+-rw-r--r--   0        0        0     6879 2023-07-25 14:56:03.314782 vban_cmd-2.3.3/vban_cmd/worker.py
+-rw-r--r--   0        0        0    12994 1970-01-01 00:00:00.000000 vban_cmd-2.3.3/PKG-INFO
```

### Comparing `vban_cmd-2.3.2/LICENSE` & `vban_cmd-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.2/pyproject.toml` & `vban_cmd-2.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vban-cmd"
-version = "2.3.2"
+version = "2.3.3"
 description = "Python interface for the VBAN RT Packet Service (Sendtext)"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/vban-cmd-python"
 
 [tool.poetry.dependencies]
```

### Comparing `vban_cmd-2.3.2/README.md` & `vban_cmd-2.3.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 ![Tests Status](./tests/basic.svg?dummy=8484744)
 ![Tests Status](./tests/banana.svg?dummy=8484744)
 ![Tests Status](./tests/potato.svg?dummy=8484744)
 
 # VBAN CMD
 
-This python interface allows you to get and set Voicemeeter parameter values over a network.
+This python interface allows you to transmit Voicemeeter parameters over a network.
 
 It may be used standalone or to extend the [Voicemeeter Remote Python API](https://github.com/onyx-and-iris/voicemeeter-api-python)
 
 There is no support for audio transfer in this package, only parameters.
 
 For an outline of past/future changes refer to: [CHANGELOG](CHANGELOG.md)
 
@@ -247,25 +247,28 @@
 -   `mute`: boolean
 -   `label`: string
 -   `gain`: float, -60 to 12
 
 example:
 
 ```python
-vban.bus[4].eq = true
 print(vban.bus[0].label)
 ```
 
 ##### Bus.EQ
 
 The following properties are available.
 
 -   `on`: boolean
 -   `ab`: boolean
 
+```python
+vban.bus[4].eq.on = true
+```
+
 ##### Modes
 
 The following properties are available.
 
 -   `normal`: boolean
 -   `amix`: boolean
 -   `bmix`: boolean
@@ -502,20 +505,35 @@
 
 #### `vban.public_packet`
 
 Returns a `VbanRtPacket`. Designed to be used internally by the interface but available for parsing through this read only property object. 
 
 States not guaranteed to be current (requires use of dirty parameters to confirm).
 
-### `Errors`
+## Errors
 
 -   `errors.VBANCMDError`: Exception raised when general errors occur.
 -   `errors.VBANCMDConnectionError`: Exception raised when connection/timeout errors occur.
 
-### `Tests`
+## Logging
+
+It's possible to see the messages sent by the interface's setters and getters, may be useful for debugging.
+
+example:
+```python
+import vban_cmd
+
+logging.basicConfig(level=logging.DEBUG)
+
+opts = {"ip": "ip.local", "port": 6980, "streamname": "Command1"}
+with vban_cmd.api('banana', **opts) as vban:
+        ...
+```
+
+## Tests
 
 First make sure you installed the [development dependencies](https://github.com/onyx-and-iris/vban-cmd-python#installation)
 
 Then from tests directory:
 
 `pytest -v`
```

### Comparing `vban_cmd-2.3.2/vban_cmd/bus.py` & `vban_cmd-2.3.3/vban_cmd/bus.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.2/vban_cmd/command.py` & `vban_cmd-2.3.3/vban_cmd/command.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.2/vban_cmd/config.py` & `vban_cmd-2.3.3/vban_cmd/config.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.2/vban_cmd/event.py` & `vban_cmd-2.3.3/vban_cmd/event.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.2/vban_cmd/factory.py` & `vban_cmd-2.3.3/vban_cmd/factory.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.2/vban_cmd/iremote.py` & `vban_cmd-2.3.3/vban_cmd/iremote.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,14 +106,15 @@
 
     def _cmd(self, param):
         cmd = (self.identifier,)
         if param:
             cmd += (f".{param}",)
         return "".join(cmd)
 
+    @property
     @abstractmethod
     def identifier(self):
         pass
 
     @property
     def public_packet(self):
         """Returns an RT data packet."""
```

### Comparing `vban_cmd-2.3.2/vban_cmd/kinds.py` & `vban_cmd-2.3.3/vban_cmd/kinds.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,14 +49,22 @@
     def num_strip(self):
         return sum(self.ins)
 
     @property
     def num_bus(self):
         return sum(self.outs)
 
+    @property
+    def num_strip_levels(self) -> int:
+        return 2 * self.phys_in + 8 * self.virt_in
+
+    @property
+    def num_bus_levels(self) -> int:
+        return 8 * (self.phys_out + self.virt_out)
+
     def __str__(self) -> str:
         return self.name.capitalize()
 
 
 @dataclass
 class BasicMap(KindMapClass):
     name: str
```

### Comparing `vban_cmd-2.3.2/vban_cmd/macrobutton.py` & `vban_cmd-2.3.3/vban_cmd/macrobutton.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     """A placeholder class in case this interface is being used interchangeably with the Remote API"""
 
     def __str__(self):
         return f"{type(self).__name__}{self._remote.kind}{self.index}"
 
     @property
     def identifier(self):
-        return f"button[{self.index}]"
+        return f"command.button[{self.index}]"
 
     @property
     def state(self) -> bool:
         self.logger.warning("button.state commands are not supported over VBAN")
 
     @state.setter
     def state(self, _):
```

### Comparing `vban_cmd-2.3.2/vban_cmd/meta.py` & `vban_cmd-2.3.3/vban_cmd/meta.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.2/vban_cmd/packet.py` & `vban_cmd-2.3.3/vban_cmd/packet.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,20 +99,20 @@
     def samplerate(self) -> int:
         """returns samplerate as an int"""
         return int.from_bytes(self._samplerate, "little")
 
     @property
     def inputlevels(self) -> tuple:
         """returns the entire level array across all inputs for a kind"""
-        return self.strip_levels[0 : (2 * self._kind.phys_in + 8 * self._kind.virt_in)]
+        return self.strip_levels[0 : self._kind.num_strip_levels]
 
     @property
     def outputlevels(self) -> tuple:
         """returns the entire level array across all outputs for a kind"""
-        return self.bus_levels[0 : 8 * self._kind.num_bus]
+        return self.bus_levels[0 : self._kind.num_bus_levels]
 
     @property
     def stripstate(self) -> tuple:
         """returns tuple of strip states accessable through bit modes"""
         return tuple(self._stripState[i : i + 4] for i in range(0, 32, 4))
 
     @property
```

### Comparing `vban_cmd-2.3.2/vban_cmd/strip.py` & `vban_cmd-2.3.3/vban_cmd/strip.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.2/vban_cmd/subject.py` & `vban_cmd-2.3.3/vban_cmd/subject.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.2/vban_cmd/util.py` & `vban_cmd-2.3.3/vban_cmd/util.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.2/vban_cmd/vban.py` & `vban_cmd-2.3.3/vban_cmd/vban.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.2/vban_cmd/vbancmd.py` & `vban_cmd-2.3.3/vban_cmd/vbancmd.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.2/vban_cmd/worker.py` & `vban_cmd-2.3.3/vban_cmd/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,17 +137,16 @@
         self._remote = remote
         self.queue = queue
         self.logger = logger.getChild(self.__class__.__name__)
         self._remote.socks[Socket.response].settimeout(self._remote.timeout)
         self._remote.socks[Socket.response].bind(
             (socket.gethostbyname(socket.gethostname()), self._remote.port)
         )
-        p_in, v_in = self._remote.kind.ins
-        self._remote._strip_comp = [False] * (2 * p_in + 8 * v_in)
-        self._remote._bus_comp = [False] * (self._remote.kind.num_bus * 8)
+        self._remote._strip_comp = [False] * (self._remote.kind.num_strip_levels)
+        self._remote._bus_comp = [False] * (self._remote.kind.num_bus_levels)
 
     def run(self):
         """
         Continously update observers of dirty states.
 
         Generate _strip_comp, _bus_comp and update level cache if ldirty.
         """
```

### Comparing `vban_cmd-2.3.2/PKG-INFO` & `vban_cmd-2.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vban-cmd
-Version: 2.3.2
+Version: 2.3.3
 Summary: Python interface for the VBAN RT Packet Service (Sendtext)
 Home-page: https://github.com/onyx-and-iris/vban-cmd-python
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -21,15 +21,15 @@
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 ![Tests Status](./tests/basic.svg?dummy=8484744)
 ![Tests Status](./tests/banana.svg?dummy=8484744)
 ![Tests Status](./tests/potato.svg?dummy=8484744)
 
 # VBAN CMD
 
-This python interface allows you to get and set Voicemeeter parameter values over a network.
+This python interface allows you to transmit Voicemeeter parameters over a network.
 
 It may be used standalone or to extend the [Voicemeeter Remote Python API](https://github.com/onyx-and-iris/voicemeeter-api-python)
 
 There is no support for audio transfer in this package, only parameters.
 
 For an outline of past/future changes refer to: [CHANGELOG](CHANGELOG.md)
 
@@ -264,25 +264,28 @@
 -   `mute`: boolean
 -   `label`: string
 -   `gain`: float, -60 to 12
 
 example:
 
 ```python
-vban.bus[4].eq = true
 print(vban.bus[0].label)
 ```
 
 ##### Bus.EQ
 
 The following properties are available.
 
 -   `on`: boolean
 -   `ab`: boolean
 
+```python
+vban.bus[4].eq.on = true
+```
+
 ##### Modes
 
 The following properties are available.
 
 -   `normal`: boolean
 -   `amix`: boolean
 -   `bmix`: boolean
@@ -519,20 +522,35 @@
 
 #### `vban.public_packet`
 
 Returns a `VbanRtPacket`. Designed to be used internally by the interface but available for parsing through this read only property object. 
 
 States not guaranteed to be current (requires use of dirty parameters to confirm).
 
-### `Errors`
+## Errors
 
 -   `errors.VBANCMDError`: Exception raised when general errors occur.
 -   `errors.VBANCMDConnectionError`: Exception raised when connection/timeout errors occur.
 
-### `Tests`
+## Logging
+
+It's possible to see the messages sent by the interface's setters and getters, may be useful for debugging.
+
+example:
+```python
+import vban_cmd
+
+logging.basicConfig(level=logging.DEBUG)
+
+opts = {"ip": "ip.local", "port": 6980, "streamname": "Command1"}
+with vban_cmd.api('banana', **opts) as vban:
+        ...
+```
+
+## Tests
 
 First make sure you installed the [development dependencies](https://github.com/onyx-and-iris/vban-cmd-python#installation)
 
 Then from tests directory:
 
 `pytest -v`
```

