# Comparing `tmp/mypyllant-0.3.2.tar.gz` & `tmp/mypyllant-0.3.3.tar.gz`

## Comparing `mypyllant-0.3.2.tar` & `mypyllant-0.3.3.tar`

### file list

```diff
@@ -1,36 +1,43 @@
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 mypyllant-0.3.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0    45426 2020-02-02 00:00:00.000000 mypyllant-0.3.2/logo.png
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 mypyllant-0.3.2/requirements-dev.txt
--rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 mypyllant-0.3.2/run_pytest.sh
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 mypyllant-0.3.2/.github/workflows/build-test.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/__init__.py
--rw-r--r--   0        0        0    17950 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/api.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/const.py
--rwxr-xr-x   0        0        0     2782 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/export.py
--rw-r--r--   0        0        0     8358 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/py.typed
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/sample.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/__init__.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/conftest.py
--rwxr-xr-x   0        0        0      934 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/find_countries.py
--rw-r--r--   0        0        0     6824 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/generate_test_data.py
--rw-r--r--   0        0        0     7710 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/test_api.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/test_countries.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/test_export.py
--rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/test_generate_test_data.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/test_sample.py
--rwxr-xr-x   0        0        0      655 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/update_sample.py
--rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/utils.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/claims.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/connection_status.json
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/control_identifier.json
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/current_system.json
--rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/device_buckets.json
--rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/system.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mypyllant-0.3.2/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/time_zone.json
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 mypyllant-0.3.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mypyllant-0.3.2/LICENSE
--rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 mypyllant-0.3.2/README.md
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 mypyllant-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 mypyllant-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 mypyllant-0.3.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    45426 2020-02-02 00:00:00.000000 mypyllant-0.3.3/logo.png
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 mypyllant-0.3.3/requirements-dev.txt
+-rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 mypyllant-0.3.3/run_pytest.sh
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 mypyllant-0.3.3/.github/workflows/build-test.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/__init__.py
+-rw-r--r--   0        0        0    17950 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/api.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/const.py
+-rwxr-xr-x   0        0        0     2782 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/export.py
+-rw-r--r--   0        0        0     8610 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/py.typed
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/sample.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/__init__.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/conftest.py
+-rwxr-xr-x   0        0        0      934 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/find_countries.py
+-rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/generate_test_data.py
+-rw-r--r--   0        0        0     7808 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/test_api.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/test_countries.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/test_export.py
+-rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/test_generate_test_data.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/test_sample.py
+-rwxr-xr-x   0        0        0      655 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/update_sample.py
+-rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/utils.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/json/030f109526faf40c523f7ac79f8a0d7e368b2938/claims.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/json/030f109526faf40c523f7ac79f8a0d7e368b2938/connection_status.json
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/json/030f109526faf40c523f7ac79f8a0d7e368b2938/control_identifier.json
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/json/030f109526faf40c523f7ac79f8a0d7e368b2938/current_system.json
+-rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/json/030f109526faf40c523f7ac79f8a0d7e368b2938/device_buckets.json
+-rw-r--r--   0        0        0     9669 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/json/030f109526faf40c523f7ac79f8a0d7e368b2938/system.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/json/030f109526faf40c523f7ac79f8a0d7e368b2938/time_zone.json
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/claims.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/connection_status.json
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/control_identifier.json
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/current_system.json
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/device_buckets.json
+-rw-r--r--   0        0        0     5539 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/system.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/time_zone.json
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 mypyllant-0.3.3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mypyllant-0.3.3/LICENSE
+-rw-r--r--   0        0        0     4971 2020-02-02 00:00:00.000000 mypyllant-0.3.3/README.md
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 mypyllant-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 mypyllant-0.3.3/PKG-INFO
```

### Comparing `mypyllant-0.3.2/.pre-commit-config.yaml` & `mypyllant-0.3.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.2/logo.png` & `mypyllant-0.3.3/logo.png`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.2/.github/workflows/build-test.yaml` & `mypyllant-0.3.3/.github/workflows/build-test.yaml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.2/src/myPyllant/api.py` & `mypyllant-0.3.3/src/myPyllant/api.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.2/src/myPyllant/const.py` & `mypyllant-0.3.3/src/myPyllant/const.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.2/src/myPyllant/export.py` & `mypyllant-0.3.3/src/myPyllant/export.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.2/src/myPyllant/models.py` & `mypyllant-0.3.3/src/myPyllant/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import datetime
-import json
 import logging
 from collections.abc import Iterator
 from enum import Enum
 from typing import Any, Optional
 
 from pydantic import BaseModel
 
@@ -156,19 +155,20 @@
     connected: bool | None
 
     def __init__(self, **data: Any) -> None:
         if "claim" in data and "id" not in data:
             data["id"] = data["claim"].system_id
         super().__init__(**data)
         logger.debug(f"Creating related models from state: {data}")
-        self.zones = [Zone(system_id=self.id, **z) for z in self._merged_zones]
-        self.circuits = [Circuit(system_id=self.id, **c) for c in self._merged_circuits]
+        self.zones = [Zone(system_id=self.id, **z) for z in self._merge_object("zones")]
+        self.circuits = [
+            Circuit(system_id=self.id, **c) for c in self._merge_object("circuits")
+        ]
         self.domestic_hot_water = [
-            DomesticHotWater(system_id=self.id, **d)
-            for d in self._merged_domestic_hot_water
+            DomesticHotWater(system_id=self.id, **d) for d in self._merge_object("dhw")
         ]
         self.devices = [
             Device(system_id=self.id, type=k, **v) for k, v in self._raw_devices
         ]
 
     class Config:
         arbitrary_types_allowed = True  # Necessary for timezone
@@ -183,44 +183,44 @@
     def primary_heat_generator(self) -> Optional["Device"]:
         devices = [d for d in self.devices if d.type == "primary_heat_generator"]
         if len(devices) > 0:
             return devices[0]
         return None
 
     def _merge_object(self, obj_name) -> Iterator[dict]:
+        """
+        The Vaillant API returns information about zones, circuits, and dhw separately as
+        configuration, state, and properties.
+
+        This function merges everything together into one big dict for a given object (i.e. zones)
+        """
         indexes = [o["index"] for o in self.configuration.get(obj_name, [])]
         for idx in indexes:
-            configuration = [
+            # deepcopy() avoids unintentional changes to the referenced objects
+            configuration = next(
                 c for c in self.configuration.get(obj_name, []) if c["index"] == idx
-            ][0]
-            state = [c for c in self.state.get(obj_name, []) if c["index"] == idx][0]
-            properties = [
-                c for c in self.properties.get(obj_name, []) if c["index"] == idx
-            ][0]
-            del state["index"]
-            del properties["index"]
-            logger.debug(
-                f"Merging {obj_name} into results: {json.dumps(configuration, indent=2)}"
             )
-            logger.debug(json.dumps(state, indent=2))
-            logger.debug(json.dumps(properties, indent=2))
-            merged = dict(**state, **properties, **configuration)
-            yield merged
-
-    @property
-    def _merged_zones(self) -> Iterator[dict]:
-        return self._merge_object("zones")
-
-    @property
-    def _merged_circuits(self) -> Iterator[dict]:
-        return self._merge_object("circuits")
-
-    @property
-    def _merged_domestic_hot_water(self) -> Iterator[dict]:
-        return self._merge_object("dhw")
+            try:
+                state = next(
+                    c for c in self.state.get(obj_name, []) if c["index"] == idx
+                )
+            except (StopIteration, KeyError) as e:
+                logger.warning("Error when merging state", exc_info=e)
+                state = {}
+            try:
+                properties = next(
+                    c for c in self.properties.get(obj_name, []) if c["index"] == idx
+                )
+            except (StopIteration, KeyError) as e:
+                logger.warning("Error when merging properties", exc_info=e)
+                properties = {}
+            # index is part of all three fields, delete from two to avoid multiple keyword argument error in dict init
+            configuration.update(state)
+            configuration.update(properties)
+            yield configuration
 
     @property
     def outdoor_temperature(self) -> float | None:
         try:
             return self.state["system"]["outdoor_temperature"]
         except KeyError:
             logger.info(
```

### Comparing `mypyllant-0.3.2/src/myPyllant/sample.py` & `mypyllant-0.3.3/src/myPyllant/sample.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.2/src/myPyllant/utils.py` & `mypyllant-0.3.3/src/myPyllant/utils.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.2/src/myPyllant/tests/find_countries.py` & `mypyllant-0.3.3/src/myPyllant/tests/find_countries.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.2/src/myPyllant/tests/generate_test_data.py` & `mypyllant-0.3.3/src/myPyllant/tests/generate_test_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,17 @@
             claims_url, headers=api.get_authorized_headers()
         ) as claims_resp:
             claims = await claims_resp.json()
             with open(json_dir / "claims.json", "w") as fh:
                 anonymized_system = _recursive_data_anonymize(
                     copy.deepcopy(claims), SALT
                 )
+                for system in anonymized_system:
+                    if "address" in system:
+                        system.pop("address")
                 fh.write(json.dumps(anonymized_system, indent=2))
 
         control_identifier_url = f"{API_URL_BASE}/systems/{claims[0]['systemId']}/meta-info/control-identifier"
         async with api.aiohttp_session.get(
             control_identifier_url, headers=api.get_authorized_headers()
         ) as ci_response:
             with open(json_dir / "control_identifier.json", "w") as fh:
```

### Comparing `mypyllant-0.3.2/src/myPyllant/tests/test_api.py` & `mypyllant-0.3.3/src/myPyllant/tests/test_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,30 +86,30 @@
         await mocked_api.aiohttp_session.close()
 
 
 @pytest.mark.parametrize("test_data", get_test_data())
 async def test_devices(mypyllant_aioresponses, mocked_api, test_data) -> None:
     with mypyllant_aioresponses(test_data) as _:
         system = await anext(mocked_api.get_systems())
-        device = system.devices[0]
-
-        assert isinstance(device, Device)
-        assert isinstance(device.name_display, str)
+        if len(system.devices) > 0:
+            device = system.devices[0]
+            assert isinstance(device, Device)
+            assert isinstance(device.name_display, str)
         await mocked_api.aiohttp_session.close()
 
 
 @pytest.mark.parametrize("test_data", get_test_data())
 async def test_device_data(mypyllant_aioresponses, mocked_api, test_data) -> None:
     with mypyllant_aioresponses(test_data) as _:
         system = await anext(mocked_api.get_systems())
-        device = system.devices[0]
-        device_data = await anext(mocked_api.get_data_by_device(device))
-
-        assert isinstance(device_data, DeviceData)
-        assert isinstance(device_data.data[0], DeviceDataBucket)
+        if len(system.devices) > 0:
+            device = system.devices[0]
+            device_data = await anext(mocked_api.get_data_by_device(device))
+            assert isinstance(device_data, DeviceData)
+            assert isinstance(device_data.data[0], DeviceDataBucket)
         await mocked_api.aiohttp_session.close()
 
 
 @pytest.mark.parametrize("test_data", get_test_data())
 async def test_quick_veto(mypyllant_aioresponses, mocked_api, test_data) -> None:
     with mypyllant_aioresponses(test_data) as aio:
         system = await anext(mocked_api.get_systems())
```

### Comparing `mypyllant-0.3.2/src/myPyllant/tests/test_countries.py` & `mypyllant-0.3.3/src/myPyllant/tests/test_countries.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.2/src/myPyllant/tests/test_export.py` & `mypyllant-0.3.3/src/myPyllant/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.2/src/myPyllant/tests/test_generate_test_data.py` & `mypyllant-0.3.3/src/myPyllant/tests/test_generate_test_data.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.2/src/myPyllant/tests/update_sample.py` & `mypyllant-0.3.3/src/myPyllant/tests/update_sample.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.2/src/myPyllant/tests/utils.py` & `mypyllant-0.3.3/src/myPyllant/tests/utils.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.2/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/current_system.json` & `mypyllant-0.3.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/current_system.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9815476190476191%*

 * *Differences: {"'electric_backup_heater'": "{'device_uuid': 'c6b85542bb0658a49e653bce4d9fba4032a3b27e', "*

 * *                             "'device_serial_number': '99ec5f0d620e5cafa83dd67680ee01ad2561309d', "*

 * *                             "'last_data': '2023-07-25T20:42:12Z', 'data': {0: {'to': "*

 * *                             "'2023-07-25T20:42:12Z'}, 1: {'to': '2023-07-25T20:42:11Z'}}}",*

 * * "'primary_heat_generator'": "{'device_uuid': '975c511300d878cbd350beaca74cb90e54b444ed', "*

 * *                             "'device_serial_nu […]*

```diff
@@ -3,90 +3,90 @@
         "article_number": "0010023609",
         "bus_coupler_address": 0,
         "data": [
             {
                 "calculated": false,
                 "from": "2022-10-11T16:16:40Z",
                 "operation_mode": "DOMESTIC_HOT_WATER",
-                "to": "2023-04-24T09:51:54Z",
+                "to": "2023-07-25T20:42:12Z",
                 "value_type": "CONSUMED_ELECTRICAL_ENERGY"
             },
             {
                 "calculated": false,
                 "from": "2022-10-11T16:16:40Z",
                 "operation_mode": "HEATING",
-                "to": "2023-04-24T09:51:54Z",
+                "to": "2023-07-25T20:42:11Z",
                 "value_type": "CONSUMED_ELECTRICAL_ENERGY"
             }
         ],
-        "device_serial_number": "dac5856554b37f1755cc28f041d32417e17c2b46",
+        "device_serial_number": "99ec5f0d620e5cafa83dd67680ee01ad2561309d",
         "device_type": "ELECTRIC_AUXILIARY_HEATER",
-        "device_uuid": "51e8d5f067005d0731e0a347eae3d881ff492b05",
+        "device_uuid": "c6b85542bb0658a49e653bce4d9fba4032a3b27e",
         "ebus_id": "VWZ02",
         "emfValid": true,
         "first_data": "2022-10-11T16:16:40Z",
-        "last_data": "2023-04-24T09:51:54Z",
+        "last_data": "2023-07-25T20:42:12Z",
         "product_name": "hydraulic station",
         "spn": 351
     },
     "has_emf_capable_devices": true,
     "primary_heat_generator": {
         "article_number": "0010021118",
         "bus_coupler_address": 0,
         "data": [
             {
                 "calculated": false,
                 "from": "2022-10-11T16:16:40Z",
                 "operation_mode": "DOMESTIC_HOT_WATER",
-                "to": "2023-04-24T09:51:52Z",
+                "to": "2023-07-25T20:42:09Z",
                 "value_type": "CONSUMED_ELECTRICAL_ENERGY"
             },
             {
                 "calculated": false,
                 "from": "2022-10-11T16:16:40Z",
                 "operation_mode": "HEATING",
-                "to": "2023-04-24T09:51:52Z",
+                "to": "2023-07-25T20:42:09Z",
                 "value_type": "CONSUMED_ELECTRICAL_ENERGY"
             },
             {
                 "calculated": false,
                 "from": "2022-10-11T16:16:40Z",
                 "operation_mode": "DOMESTIC_HOT_WATER",
-                "to": "2023-04-24T09:51:51Z",
+                "to": "2023-07-25T20:42:10Z",
                 "value_type": "EARNED_ENVIRONMENT_ENERGY"
             },
             {
                 "calculated": false,
                 "from": "2022-10-11T16:16:40Z",
                 "operation_mode": "HEATING",
-                "to": "2023-04-24T09:51:52Z",
+                "to": "2023-07-25T20:42:10Z",
                 "value_type": "EARNED_ENVIRONMENT_ENERGY"
             },
             {
                 "calculated": true,
                 "from": "2022-10-11T16:16:40Z",
                 "operation_mode": "HEATING",
-                "to": "2023-04-24T09:51:52Z",
+                "to": "2023-07-25T20:42:09Z",
                 "value_type": "HEAT_GENERATED"
             },
             {
                 "calculated": true,
                 "from": "2022-10-11T16:16:40Z",
                 "operation_mode": "DOMESTIC_HOT_WATER",
-                "to": "2023-04-24T09:51:51Z",
+                "to": "2023-07-25T20:42:09Z",
                 "value_type": "HEAT_GENERATED"
             }
         ],
-        "device_serial_number": "761cc85068c3cb2fb11c490a81ce537dc99425d4",
+        "device_serial_number": "ae71310aab0ba75989ee63aebb7f43bc379c912a",
         "device_type": "HEATPUMP",
-        "device_uuid": "baf4a5d5cc9d4277c54316a1dfcd9f3cbf1970de",
+        "device_uuid": "975c511300d878cbd350beaca74cb90e54b444ed",
         "ebus_id": "HMU03",
         "emfValid": true,
         "first_data": "2022-10-11T16:16:40Z",
-        "last_data": "2023-04-24T09:51:52Z",
+        "last_data": "2023-07-25T20:42:10Z",
         "product_name": "aroTHERM plus",
         "spn": 351
     },
     "secondary_heat_generators": [],
     "solar_station": null,
     "system_type": "HEATPUMP",
     "ventilation": null
```

### Comparing `mypyllant-0.3.2/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/device_buckets.json` & `mypyllant-0.3.3/src/myPyllant/tests/json/030f109526faf40c523f7ac79f8a0d7e368b2938/device_buckets.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.2/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/system.json` & `mypyllant-0.3.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/system.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9565972222222222%*

 * *Differences: {"'configuration'": "{'zones': {0: {'heating': {'manualModeSetpointHeating': 19.0}}}, 'circuits': "*

 * *                    "{0: {'heatingCurve': 0.6842696}}}",*

 * * "'state'": "{'system': {'outdoorTemperature': 15.65625, 'systemWaterPressure': 1.3, "*

 * *            "'outdoorTemperatureAverage24h': 19.300781}, 'zones': {0: "*

 * *            "{'desiredRoomTemperatureSetpointHeating': 0.0, 'desiredRoomTemperatureSetpoint': 0.0, "*

 * *            "'currentRoomTemperature': 23.1625, 'currentRoomHumidity': 62.0, "*

 * *            "'cu […]*

```diff
@@ -1,12 +1,12 @@
 {
     "configuration": {
         "circuits": [
             {
-                "heatingCurve": 0.5549309,
+                "heatingCurve": 0.6842696,
                 "heatingFlowTemperatureMinimumSetpoint": 35.0,
                 "index": 0,
                 "setBackModeEnabled": false
             }
         ],
         "dhw": [
             {
@@ -115,15 +115,15 @@
         ],
         "zones": [
             {
                 "general": {
                     "name": "Zone 1"
                 },
                 "heating": {
-                    "manualModeSetpointHeating": 21.0,
+                    "manualModeSetpointHeating": 19.0,
                     "operationModeHeating": "TIME_CONTROLLED",
                     "setBackTemperature": 15.5,
                     "timeProgramHeating": {
                         "friday": [
                             {
                                 "endTime": 1290,
                                 "setpoint": 19.5,
@@ -210,38 +210,38 @@
                 "zoneBinding": "CENTRAL_CONTROL"
             }
         ]
     },
     "state": {
         "circuits": [
             {
-                "circuitState": "HEATING",
-                "currentCircuitFlowTemperature": 52.5,
+                "calculatedEnergyManagerState": "HEATING_STANDBY",
+                "circuitState": "STANDBY",
+                "currentCircuitFlowTemperature": 30.0,
                 "index": 0
             }
         ],
         "dhw": [
             {
-                "currentDhwTemperature": 45.5,
+                "currentDhwTemperature": 44.0,
                 "currentSpecialFunction": "REGULAR",
                 "index": 255
             }
         ],
         "system": {
-            "outdoorTemperature": 15.199219,
-            "systemWaterPressure": 1.1
+            "outdoorTemperature": 15.65625,
+            "outdoorTemperatureAverage24h": 19.300781,
+            "systemWaterPressure": 1.3
         },
         "zones": [
             {
-                "currentRoomHumidity": 60.0,
-                "currentRoomTemperature": 20.35,
-                "currentSpecialFunction": "QUICK_VETO",
-                "desiredRoomTemperatureSetpoint": 20.5,
-                "desiredRoomTemperatureSetpointHeating": 20.5,
-                "heatingState": "HEATING_UP",
-                "index": 0,
-                "quickVetoEndDateTime": "2023-04-24T12:35:00Z",
-                "quickVetoStartDateTime": "2023-04-24T09:35:28Z"
+                "currentRoomHumidity": 62.0,
+                "currentRoomTemperature": 23.1625,
+                "currentSpecialFunction": "NONE",
+                "desiredRoomTemperatureSetpoint": 0.0,
+                "desiredRoomTemperatureSetpointHeating": 0.0,
+                "heatingState": "IDLE",
+                "index": 0
             }
         ]
     }
 }
```

### Comparing `mypyllant-0.3.2/.gitignore` & `mypyllant-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.2/LICENSE` & `mypyllant-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.2/README.md` & `mypyllant-0.3.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -97,14 +97,16 @@
 > **Warning**
 > 
 > You need at least Python 3.10
 
 I'm happy to accept PRs, if you run the pre-commit checks and test your changes:
 
 ```shell
+git clone https://github.com/signalkraft/myPyllant.git
+cd myPyllant
 python3 -m venv .venv
 source .venv/bin/activate
 pip install -r requirements-dev.txt
 pip install -e .
 pre-commit install
 pytest
 ```
```

### Comparing `mypyllant-0.3.2/pyproject.toml` & `mypyllant-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.2/PKG-INFO` & `mypyllant-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myPyllant
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Python library to interact with the API behind the myVAILLANT app
 Project-URL: Homepage, https://github.com/signalkraft/myPyllant
 Project-URL: Bug Tracker, https://github.com/signalkraft/myPyllant/issues
 Author-email: Philipp <pd@signalkraft.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -113,14 +113,16 @@
 > **Warning**
 > 
 > You need at least Python 3.10
 
 I'm happy to accept PRs, if you run the pre-commit checks and test your changes:
 
 ```shell
+git clone https://github.com/signalkraft/myPyllant.git
+cd myPyllant
 python3 -m venv .venv
 source .venv/bin/activate
 pip install -r requirements-dev.txt
 pip install -e .
 pre-commit install
 pytest
 ```
```

