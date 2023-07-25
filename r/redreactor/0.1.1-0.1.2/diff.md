# Comparing `tmp/redreactor-0.1.1.tar.gz` & `tmp/redreactor-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redreactor-0.1.1.tar", max compression
+gzip compressed data, was "redreactor-0.1.2.tar", max compression
```

## Comparing `redreactor-0.1.1.tar` & `redreactor-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1067 2023-06-01 08:17:19.223168 redreactor-0.1.1/LICENSE
--rw-r--r--   0        0        0     3409 2023-06-01 08:17:19.223168 redreactor-0.1.1/README.md
--rw-r--r--   0        0        0     3199 2023-06-01 08:17:33.679257 redreactor-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       60 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/__init__.py
--rw-r--r--   0        0        0     3997 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/__main__.py
--rw-r--r--   0        0        0       97 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/components/commander/__init__.py
--rw-r--r--   0        0        0     6734 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/components/commander/commander.py
--rw-r--r--   0        0        0      121 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/components/homeassistant/__init__.py
--rw-r--r--   0        0        0      526 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/components/homeassistant/binary_sensor.py
--rw-r--r--   0        0        0      646 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/components/homeassistant/button.py
--rw-r--r--   0        0        0     4954 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/components/homeassistant/common.py
--rw-r--r--   0        0        0     7744 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/components/homeassistant/homeassistant.py
--rw-r--r--   0        0        0     1224 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/components/homeassistant/number.py
--rw-r--r--   0        0        0      707 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/components/homeassistant/sensor.py
--rw-r--r--   0        0        0       99 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/components/monitor/__init__.py
--rw-r--r--   0        0        0     1601 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/components/monitor/data.py
--rw-r--r--   0        0        0    12761 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/components/monitor/monitor.py
--rw-r--r--   0        0        0       84 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/components/mqtt/__init__.py
--rw-r--r--   0        0        0     6086 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/components/mqtt/mqtt.py
--rw-r--r--   0        0        0     8497 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/configuration.py
--rw-r--r--   0        0        0      708 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/const.py
--rw-r--r--   0        0        0       37 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/helpers/__init__.py
--rw-r--r--   0        0        0      902 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/helpers/emitter.py
--rw-r--r--   0        0        0     1116 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/helpers/repeater.py
--rw-r--r--   0        0        0      685 2023-06-01 08:17:19.223168 redreactor-0.1.1/src/redreactor/helpers/utils.py
--rw-r--r--   0        0        0     4342 1970-01-01 00:00:00.000000 redreactor-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-25 19:51:52.729909 redreactor-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3409 2023-07-25 19:51:52.729909 redreactor-0.1.2/README.md
+-rw-r--r--   0        0        0     3252 2023-07-25 19:52:08.442261 redreactor-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       60 2023-07-25 19:51:52.729909 redreactor-0.1.2/src/redreactor/__init__.py
+-rw-r--r--   0        0        0     3997 2023-07-25 19:51:52.729909 redreactor-0.1.2/src/redreactor/__main__.py
+-rw-r--r--   0        0        0       97 2023-07-25 19:51:52.729909 redreactor-0.1.2/src/redreactor/components/commander/__init__.py
+-rw-r--r--   0        0        0     6734 2023-07-25 19:51:52.729909 redreactor-0.1.2/src/redreactor/components/commander/commander.py
+-rw-r--r--   0        0        0      121 2023-07-25 19:51:52.729909 redreactor-0.1.2/src/redreactor/components/homeassistant/__init__.py
+-rw-r--r--   0        0        0      526 2023-07-25 19:51:52.729909 redreactor-0.1.2/src/redreactor/components/homeassistant/binary_sensor.py
+-rw-r--r--   0        0        0      646 2023-07-25 19:51:52.729909 redreactor-0.1.2/src/redreactor/components/homeassistant/button.py
+-rw-r--r--   0        0        0     4954 2023-07-25 19:51:52.729909 redreactor-0.1.2/src/redreactor/components/homeassistant/common.py
+-rw-r--r--   0        0        0     7744 2023-07-25 19:51:52.729909 redreactor-0.1.2/src/redreactor/components/homeassistant/homeassistant.py
+-rw-r--r--   0        0        0     1224 2023-07-25 19:51:52.733909 redreactor-0.1.2/src/redreactor/components/homeassistant/number.py
+-rw-r--r--   0        0        0      707 2023-07-25 19:51:52.733909 redreactor-0.1.2/src/redreactor/components/homeassistant/sensor.py
+-rw-r--r--   0        0        0       99 2023-07-25 19:51:52.733909 redreactor-0.1.2/src/redreactor/components/monitor/__init__.py
+-rw-r--r--   0        0        0     1601 2023-07-25 19:51:52.733909 redreactor-0.1.2/src/redreactor/components/monitor/data.py
+-rw-r--r--   0        0        0    12751 2023-07-25 19:51:52.733909 redreactor-0.1.2/src/redreactor/components/monitor/monitor.py
+-rw-r--r--   0        0        0       84 2023-07-25 19:51:52.733909 redreactor-0.1.2/src/redreactor/components/mqtt/__init__.py
+-rw-r--r--   0        0        0     6086 2023-07-25 19:51:52.733909 redreactor-0.1.2/src/redreactor/components/mqtt/mqtt.py
+-rw-r--r--   0        0        0     8497 2023-07-25 19:51:52.733909 redreactor-0.1.2/src/redreactor/configuration.py
+-rw-r--r--   0        0        0      794 2023-07-25 19:51:52.733909 redreactor-0.1.2/src/redreactor/const.py
+-rw-r--r--   0        0        0       37 2023-07-25 19:51:52.733909 redreactor-0.1.2/src/redreactor/helpers/__init__.py
+-rw-r--r--   0        0        0      902 2023-07-25 19:51:52.733909 redreactor-0.1.2/src/redreactor/helpers/emitter.py
+-rw-r--r--   0        0        0     1116 2023-07-25 19:51:52.733909 redreactor-0.1.2/src/redreactor/helpers/repeater.py
+-rw-r--r--   0        0        0      673 2023-07-25 19:51:52.733909 redreactor-0.1.2/src/redreactor/helpers/utils.py
+-rw-r--r--   0        0        0     4342 1970-01-01 00:00:00.000000 redreactor-0.1.2/PKG-INFO
```

### Comparing `redreactor-0.1.1/LICENSE` & `redreactor-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.1/README.md` & `redreactor-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.1/pyproject.toml` & `redreactor-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redreactor"
-version = "0.1.1"
+version = "0.1.2"
 description = "Red Reactor Battery Monitoring service with MQTT, and Home Assistant support"
 documentation = "https://github.com/mreditor97/redreactor"
 repository = "https://github.com/mreditor97/redreactor"
 homepage = "https://github.com/mreditor97/redreactor"
 authors = ["MrEditor97 <dev@mreditor97.co.uk>"]
 license = "MIT"
 readme = "README.md"
@@ -20,27 +20,27 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/mreditor97/redreactor/issues"
 Changelog = "https://github.com/mreditor97/redreactor/releases"
 
 [tool.poetry.dev-dependencies]
 aresponses = "2.1.6"
-black = "23.3.0"
-blacken-docs = "1.13.0"
-codespell = "2.2.4"
+black = "23.7.0"
+blacken-docs = "1.15.0"
+codespell = "2.2.5"
 covdefaults = "2.3.0"
 coverage = {version = "7.2.7", extras = ["toml"]}
-mypy = "1.3.0"
-pre-commit = "3.3.2"
+mypy = "1.4.1"
+pre-commit = "3.3.3"
 pre-commit-hooks = "4.4.0"
 pylint = "2.17.4"
-pytest = "7.3.1"
-pytest-asyncio = "0.21.0"
+pytest = "7.4.0"
+pytest-asyncio = "0.21.1"
 pytest-cov = "4.1.0"
-ruff = "0.0.270"
+ruff = "0.0.280"
 safety = "2.4.0b1"
 types-cachetools = "^5.3.0"
 yamllint = "1.32.0"
 types-pyyaml = "^6.0.12.10"
 
 [tool.coverage.run]
 plugins = ["covdefaults"]
@@ -126,14 +126,15 @@
 ignore = [
   "ANN101", # Self... explanatory
   "ANN401", # Opinioated warning on disallowing dynamically typed expressions
   "D203", # Conflicts with other rules
   "D213", # Conflicts with other rules
   "D417", # False positives in some occasions
   "PLR2004", # Just annoying, not really useful
+  "RUF012", # Disabled until it is Ruff finalises it
 ]
 select = ["ALL"]
 
 [tool.ruff.flake8-pytest-style]
 fixture-parentheses = false
 mark-parentheses = false
```

### Comparing `redreactor-0.1.1/src/redreactor/__main__.py` & `redreactor-0.1.2/src/redreactor/__main__.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.1/src/redreactor/components/commander/commander.py` & `redreactor-0.1.2/src/redreactor/components/commander/commander.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.1/src/redreactor/components/homeassistant/binary_sensor.py` & `redreactor-0.1.2/src/redreactor/components/homeassistant/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.1/src/redreactor/components/homeassistant/button.py` & `redreactor-0.1.2/src/redreactor/components/homeassistant/button.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.1/src/redreactor/components/homeassistant/common.py` & `redreactor-0.1.2/src/redreactor/components/homeassistant/common.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.1/src/redreactor/components/homeassistant/homeassistant.py` & `redreactor-0.1.2/src/redreactor/components/homeassistant/homeassistant.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.1/src/redreactor/components/homeassistant/number.py` & `redreactor-0.1.2/src/redreactor/components/homeassistant/number.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.1/src/redreactor/components/homeassistant/sensor.py` & `redreactor-0.1.2/src/redreactor/components/homeassistant/sensor.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.1/src/redreactor/components/monitor/data.py` & `redreactor-0.1.2/src/redreactor/components/monitor/data.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.1/src/redreactor/components/monitor/monitor.py` & `redreactor-0.1.2/src/redreactor/components/monitor/monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from ina219 import INA219, DeviceRangeError
 from paho.mqtt.client import Client
 
 from redreactor.components.mqtt import MQTT
 from redreactor.configuration import DynamicConfiguration
 from redreactor.const import (
     DEFAULT_BATTERY_VOLTAGE_MAXIMUM,
+    DEFAULT_BATTERY_VOLTAGE_MAXIMUM_DROP,
     DEFAULT_BATTERY_VOLTAGE_MINIMUM,
     DEFAULT_BATTERY_WARNING_THRESHOLD,
     DEFAULT_REPORT_INTERVAL,
 )
 from redreactor.helpers.emitter import EventEmitter
 from redreactor.helpers.repeater import RepeatTimer
 
@@ -148,20 +149,18 @@
                     if self.data.external_power:
                         # Power removed
                         self.data.external_power = False
                         self._update()
                 elif self.data.current >= 0:
                     # Battery now Full
                     self.data.external_power = True
-                else:
-                    # Charging
-                    if not self.data.external_power:  # noqa: PLR5501
-                        # Power restored
-                        self.data.external_power = True
-                        self._update()
+                elif not self.data.external_power:
+                    # Power restored
+                    self.data.external_power = True
+                    self._update()
 
         if (
             self.data.battery_level <= float(self.data.battery_warning_threshold)
             and not self.data.external_power
         ):
             # Force immediate publish update at warning level
             self._update()
@@ -189,15 +188,15 @@
         return int(
             max(
                 min(
                     100,
                     (voltage - self.data.battery_voltage_minimum)
                     / (
                         self.data.battery_voltage_maximum
-                        - 0.05
+                        - DEFAULT_BATTERY_VOLTAGE_MAXIMUM_DROP
                         - self.data.battery_voltage_minimum
                     )
                     * 100,
                 ),
                 0,
             ),
         )
```

### Comparing `redreactor-0.1.1/src/redreactor/components/mqtt/mqtt.py` & `redreactor-0.1.2/src/redreactor/components/mqtt/mqtt.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.1/src/redreactor/configuration.py` & `redreactor-0.1.2/src/redreactor/configuration.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.1/src/redreactor/const.py` & `redreactor-0.1.2/src/redreactor/const.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Constants used by Red Reactor components."""
 
 DEFAULT_REPORT_INTERVAL = 30  # Seconds between data reporting
 DEFAULT_EXPIRE_INTERVAL = 120  # Seconds before Home Assistant invalidates received data
 DEFAULT_BATTERY_WARNING_THRESHOLD = 10  # Percentage of charge remaining
-DEFAULT_BATTERY_VOLTAGE_MINIMUM = 2.7  # Minimum battery voltage before shutting down
+DEFAULT_BATTERY_VOLTAGE_MINIMUM = 2.9  # Minimum battery voltage before shutting down
 DEFAULT_BATTERY_VOLTAGE_MAXIMUM = 4.2  # Maximum battery voltage
+DEFAULT_BATTERY_VOLTAGE_MAXIMUM_DROP = 0.03  # Maximum battery voltage allowable drop
 DEFAULT_BATTERY_VOLTAGE_ERROR = DEFAULT_BATTERY_VOLTAGE_MAXIMUM + 0.05
 
 DEFAULT_INA_I2C_ADDRESS = 0x40  # Red Reactor Default I2C Address
 DEFAULT_INA_SHUNT_OHMS = 0.05  # Red Reactor Shunt Ohms
 DEFAULT_INA_MAX_EXPECTED_AMPS = 5.5
 DEFAULT_INA_MONITOR_INTERVAL = 5  # Second read time
```

### Comparing `redreactor-0.1.1/src/redreactor/helpers/emitter.py` & `redreactor-0.1.2/src/redreactor/helpers/emitter.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.1/src/redreactor/helpers/repeater.py` & `redreactor-0.1.2/src/redreactor/helpers/repeater.py`

 * *Files identical despite different names*

### Comparing `redreactor-0.1.1/src/redreactor/helpers/utils.py` & `redreactor-0.1.2/src/redreactor/helpers/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,12 +11,12 @@
     updating only top-level keys, dict_merge recurses down into dicts nested
     to an arbitrary depth, updating keys. The ``merge_dct`` is merged into
     ``dct``.
     :param dct: dict onto which the merge is executed
     :param merge_dct: dct merged into dct
     :return: None.
     """
-    for k, _v in merge_dct.items():
+    for k in merge_dct:
         if k in dct and isinstance(dct[k], dict) and isinstance(merge_dct[k], dict):
             dict_merge(dct[k], merge_dct[k])
         else:
             dct[k] = merge_dct[k]
```

### Comparing `redreactor-0.1.1/PKG-INFO` & `redreactor-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redreactor
-Version: 0.1.1
+Version: 0.1.2
 Summary: Red Reactor Battery Monitoring service with MQTT, and Home Assistant support
 Home-page: https://github.com/mreditor97/redreactor
 License: MIT
 Author: MrEditor97
 Author-email: dev@mreditor97.co.uk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

