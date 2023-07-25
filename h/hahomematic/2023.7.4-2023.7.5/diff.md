# Comparing `tmp/hahomematic-2023.7.4.tar.gz` & `tmp/hahomematic-2023.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hahomematic-2023.7.4.tar", last modified: Sat Jul 22 21:30:00 2023, max compression
+gzip compressed data, was "hahomematic-2023.7.5.tar", last modified: Tue Jul 25 18:58:55 2023, max compression
```

## Comparing `hahomematic-2023.7.4.tar` & `hahomematic-2023.7.5.tar`

### file list

```diff
@@ -1,79 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:30:00.590215 hahomematic-2023.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-22 21:30:00.590215 hahomematic-2023.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:30:00.582215 hahomematic-2023.7.4/hahomematic/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/backport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:30:00.586215 hahomematic-2023.7.4/hahomematic/caches/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/caches/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)    16932 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/caches/persistent.py
--rw-r--r--   0 runner    (1001) docker     (123)    25139 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/caches/visibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    54098 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/central_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    46889 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14862 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/hmcli.py
--rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/json_rpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:30:00.586215 hahomematic-2023.7.4/hahomematic/platforms/
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:30:00.586215 hahomematic-2023.7.4/hahomematic/platforms/custom/
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/custom/climate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/custom/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    23747 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/custom/cover.py
--rw-r--r--   0 runner    (1001) docker     (123)    27916 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/custom/definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/custom/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    34405 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/custom/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/custom/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/custom/siren.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/custom/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/custom/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)    26742 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    20557 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:30:00.586215 hahomematic-2023.7.4/hahomematic/platforms/generic/
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/generic/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/generic/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/generic/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/generic/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/generic/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/generic/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/generic/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/generic/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:30:00.586215 hahomematic-2023.7.4/hahomematic/platforms/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/hub/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/hub/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/hub/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/hub/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/hub/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/hub/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/hub/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/hub/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    15792 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/update.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:30:00.590215 hahomematic-2023.7.4/hahomematic/rega_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/rega_scripts/fetch_all_device_data.fn
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/rega_scripts/get_serial.fn
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/rega_scripts/set_system_variable.fn
--rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/xml_rpc_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/xml_rpc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:30:00.586215 hahomematic-2023.7.4/hahomematic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-22 21:29:59.000000 hahomematic-2023.7.4/hahomematic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-22 21:30:00.000000 hahomematic-2023.7.4/hahomematic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 21:30:00.000000 hahomematic-2023.7.4/hahomematic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 21:29:58.000000 hahomematic-2023.7.4/hahomematic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-22 21:30:00.000000 hahomematic-2023.7.4/hahomematic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-22 21:30:00.000000 hahomematic-2023.7.4/hahomematic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17319 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-22 21:30:00.590215 hahomematic-2023.7.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:58:55.973132 hahomematic-2023.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-25 18:58:55.973132 hahomematic-2023.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:58:55.969132 hahomematic-2023.7.5/hahomematic/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:58:55.969132 hahomematic-2023.7.5/hahomematic/caches/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/caches/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16932 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/caches/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25139 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/caches/visibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54335 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/central_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47766 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14829 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/hmcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29672 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/json_rpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:58:55.969132 hahomematic-2023.7.5/hahomematic/platforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:58:55.969132 hahomematic-2023.7.5/hahomematic/platforms/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24865 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/custom/climate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/custom/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23747 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/custom/cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27916 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/custom/definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/custom/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34405 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/custom/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/custom/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/custom/siren.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/custom/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/custom/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26742 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20557 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:58:55.969132 hahomematic-2023.7.5/hahomematic/platforms/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/generic/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/generic/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/generic/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/generic/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/generic/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/generic/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/generic/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/generic/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:58:55.973132 hahomematic-2023.7.5/hahomematic/platforms/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/hub/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/hub/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/hub/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/hub/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/hub/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/hub/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/hub/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/hub/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15792 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/platforms/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:58:55.973132 hahomematic-2023.7.5/hahomematic/rega_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/rega_scripts/fetch_all_device_data.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/rega_scripts/get_serial.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/rega_scripts/set_system_variable.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     8669 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/xml_rpc_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/hahomematic/xml_rpc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:58:55.969132 hahomematic-2023.7.5/hahomematic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-25 18:58:55.000000 hahomematic-2023.7.5/hahomematic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-07-25 18:58:55.000000 hahomematic-2023.7.5/hahomematic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:58:55.000000 hahomematic-2023.7.5/hahomematic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:58:53.000000 hahomematic-2023.7.5/hahomematic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-25 18:58:55.000000 hahomematic-2023.7.5/hahomematic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 18:58:55.000000 hahomematic-2023.7.5/hahomematic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17264 2023-07-25 18:58:20.000000 hahomematic-2023.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-25 18:58:55.973132 hahomematic-2023.7.5/setup.cfg
```

### Comparing `hahomematic-2023.7.4/LICENSE` & `hahomematic-2023.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/PKG-INFO` & `hahomematic-2023.7.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.7.4
+Version: 2023.7.5
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
@@ -12,24 +12,23 @@
 Keywords: home,automation,homematic
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Home Automation
-Requires-Python: >=3.10.0
+Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hahomematic
 
-`hahomematic` is a Python 3 (>= 3.10) module for [Home Assistant](https://www.home-assistant.io/) to interact with [HomeMatic](https://www.eq-3.com/products/homematic.html) and [HomematicIP](https://www.homematic-ip.com/en/start.html) devices. Some other devices (f.ex. Bosch, Intertechno) might be supported as well.
+`hahomematic` is a Python 3 (>= 3.11) module for [Home Assistant](https://www.home-assistant.io/) to interact with [HomeMatic](https://www.eq-3.com/products/homematic.html) and [HomematicIP](https://www.homematic-ip.com/en/start.html) devices. Some other devices (f.ex. Bosch, Intertechno) might be supported as well.
 
 This is intended to become the successor of [pyhomematic](https://github.com/danielperna84/pyhomematic).
 
 It can be installed by using the [custom_component](https://github.com/danielperna84/custom_homematic).
 Necessary installation instructions can be found [here](https://github.com/danielperna84/custom_homematic/wiki/Installation).
 
 ## Project goal and features
```

### Comparing `hahomematic-2023.7.4/README.md` & `hahomematic-2023.7.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # hahomematic
 
-`hahomematic` is a Python 3 (>= 3.10) module for [Home Assistant](https://www.home-assistant.io/) to interact with [HomeMatic](https://www.eq-3.com/products/homematic.html) and [HomematicIP](https://www.homematic-ip.com/en/start.html) devices. Some other devices (f.ex. Bosch, Intertechno) might be supported as well.
+`hahomematic` is a Python 3 (>= 3.11) module for [Home Assistant](https://www.home-assistant.io/) to interact with [HomeMatic](https://www.eq-3.com/products/homematic.html) and [HomematicIP](https://www.homematic-ip.com/en/start.html) devices. Some other devices (f.ex. Bosch, Intertechno) might be supported as well.
 
 This is intended to become the successor of [pyhomematic](https://github.com/danielperna84/pyhomematic).
 
 It can be installed by using the [custom_component](https://github.com/danielperna84/custom_homematic).
 Necessary installation instructions can be found [here](https://github.com/danielperna84/custom_homematic/wiki/Installation).
 
 ## Project goal and features
```

### Comparing `hahomematic-2023.7.4/hahomematic/__init__.py` & `hahomematic-2023.7.5/hahomematic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/caches/dynamic.py` & `hahomematic-2023.7.5/hahomematic/caches/dynamic.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/caches/persistent.py` & `hahomematic-2023.7.5/hahomematic/caches/persistent.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/caches/visibility.py` & `hahomematic-2023.7.5/hahomematic/caches/visibility.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/central_unit.py` & `hahomematic-2023.7.5/hahomematic/central_unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 from hahomematic.platforms.generic.entity import GenericEntity
 from hahomematic.platforms.hub import HmHub
 from hahomematic.platforms.hub.button import HmProgramButton
 from hahomematic.platforms.hub.entity import GenericHubEntity, GenericSystemVariable
 from hahomematic.platforms.update import HmUpdate
 from hahomematic.support import (
     HM_INTERFACE_EVENT_SCHEMA,
+    SystemInformation,
     check_or_create_directory,
     check_password,
     get_device_address,
 )
 from hahomematic.xml_rpc_proxy import XmlRpcProxy
 
 _LOGGER = logging.getLogger(__name__)
@@ -213,19 +214,19 @@
 
     @property
     def name(self) -> str:
         """Return the name of the backend. #CC."""
         return self._attr_name
 
     @property
-    def serial(self) -> str | None:
-        """Return the serial of the backend."""
+    def system_information(self) -> SystemInformation:
+        """Return the system_information of the backend."""
         if client := self.get_primary_client():
-            return client.serial
-        return None
+            return client.system_information
+        return SystemInformation()
 
     @property
     def version(self) -> str | None:
         """Return the version of the backend. #CC."""
         if self._attr_version is None:
             versions: list[str] = []
             for client in self._clients.values():
@@ -359,15 +360,18 @@
 
         local_ip = await self._identify_callback_ip(list(self.config.interface_configs)[0].port)
         for interface_config in self.config.interface_configs:
             try:
                 if client := await hmcl.create_client(
                     central=self, interface_config=interface_config, local_ip=local_ip
                 ):
-                    if interface_config.interface not in await client.get_available_interfaces():
+                    if (
+                        interface_config.interface
+                        not in client.system_information.available_interfaces
+                    ):
                         _LOGGER.debug(
                             "CREATE_CLIENTS failed: Interface: %s is not available for backend",
                             interface_config.interface,
                         )
                         continue
                     _LOGGER.debug(
                         "CREATE_CLIENTS: Adding client %s to %s",
@@ -483,31 +487,31 @@
         """Start the connection checker."""
         self._connection_checker.stop()
         _LOGGER.debug(
             "STOP_CONNECTION_CHECKER: Stopped connection_checker for %s",
             self._attr_name,
         )
 
-    async def validate_config_and_get_serial(self) -> str | None:
+    async def validate_config_and_get_system_information(self) -> SystemInformation:
         """Validate the central configuration. #CC."""
         try:
             if len(self.config.interface_configs) == 0:
                 raise NoClients("validate_config: No clients defined.")
 
             local_ip = await self._identify_callback_ip(
                 list(self.config.interface_configs)[0].port
             )
-            serial: str | None = None
+            system_information = SystemInformation()
             for interface_config in self.config.interface_configs:
                 client = await hmcl.create_client(
                     central=self, interface_config=interface_config, local_ip=local_ip
                 )
-                if not serial:
-                    serial = await client.get_serial()
-            return serial
+                if not system_information.serial:
+                    system_information = client.system_information
+            return system_information
         except Exception as ex:
             _LOGGER.warning(ex)
             raise
 
     def get_client(self, interface_id: str) -> hmcl.Client:
         """Return a client by interface_id. #CC."""
         if not self.has_client(interface_id=interface_id):
```

### Comparing `hahomematic-2023.7.4/hahomematic/client.py` & `hahomematic-2023.7.5/hahomematic/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     HmInterfaceEventType,
     HmProductGroup,
 )
 from hahomematic.exceptions import AuthFailure, BaseHomematicException, NoConnection
 from hahomematic.platforms.device import HmDevice
 from hahomematic.support import (
     ProgramData,
+    SystemInformation,
     SystemVariableData,
     build_headers,
     build_xml_rpc_uri,
     get_channel_no,
 )
 from hahomematic.xml_rpc_proxy import XmlRpcProxy
 
@@ -68,26 +69,37 @@
 
     def __init__(self, client_config: _ClientConfig) -> None:
         """Initialize the Client."""
         self._config: Final = client_config
         self.central: Final[hmcu.CentralUnit] = client_config.central
 
         self._json_rpc_client: Final = client_config.central.json_rpc_client
-        self._proxy: Final = client_config.xml_rpc_proxy
-        self._proxy_read: Final = client_config.xml_rpc_proxy_read
+
         self.interface: Final = client_config.interface
         self.interface_id: Final = client_config.interface_id
-        self.serial: Final = client_config.serial
         self.version: Final = client_config.version
-
         self._attr_available: bool = True
         self._connection_error_count: int = 0
         self._is_callback_alive: bool = True
         self.last_updated: datetime = INIT_DATETIME
 
+        self._proxy: XmlRpcProxy
+        self._proxy_read: XmlRpcProxy
+        self.system_information: SystemInformation
+
+    async def init_client(self) -> None:
+        """Init the client."""
+        self.system_information = await self._get_system_information()
+        self._proxy = self._config.get_xml_rpc_proxy(
+            auth_enabled=self.system_information.auth_enabled
+        )
+        self._proxy_read = self._config.get_xml_rpc_proxy(
+            auth_enabled=self.system_information.auth_enabled
+        )
+
     @property
     def available(self) -> bool:
         """Return the availability of the client."""
         return self._attr_available
 
     @property
     @abstractmethod
@@ -268,32 +280,28 @@
         """Get single system variable from CCU / Homegear."""
 
     @abstractmethod
     async def get_all_system_variables(self, include_internal: bool) -> list[SystemVariableData]:
         """Get all system variables from CCU / Homegear."""
 
     @abstractmethod
-    async def get_available_interfaces(self) -> list[str]:
-        """Get all available interfaces from CCU / Homegear."""
-
-    @abstractmethod
     async def get_all_programs(self, include_internal: bool) -> list[ProgramData]:
         """Get all programs, if available."""
 
     @abstractmethod
     async def get_all_rooms(self) -> dict[str, set[str]]:
         """Get all rooms, if available."""
 
     @abstractmethod
     async def get_all_functions(self) -> dict[str, set[str]]:
         """Get all functions, if available."""
 
     @abstractmethod
-    async def get_serial(self) -> str:
-        """Get the serial of the backend."""
+    async def _get_system_information(self) -> SystemInformation:
+        """Get system information of the backend."""
 
     def get_virtual_remote(self) -> HmDevice | None:
         """Get the virtual remote for the Client."""
         for device_type in HM_VIRTUAL_REMOTE_TYPES:
             for device in self.central.devices:
                 if device.interface_id == self.interface_id and device.device_type == device_type:
                     return device
@@ -720,18 +728,14 @@
 
     async def get_all_system_variables(self, include_internal: bool) -> list[SystemVariableData]:
         """Get all system variables from CCU / Homegear."""
         return await self._json_rpc_client.get_all_system_variables(
             include_internal=include_internal
         )
 
-    async def get_available_interfaces(self) -> list[str]:
-        """Get all available interfaces from CCU / Homegear."""
-        return await self._json_rpc_client.get_available_interfaces()
-
     async def get_all_programs(self, include_internal: bool) -> list[ProgramData]:
         """Get all programs, if available."""
         return await self._json_rpc_client.get_all_programs(include_internal=include_internal)
 
     async def get_all_rooms(self) -> dict[str, set[str]]:
         """Get all rooms from CCU."""
         rooms: dict[str, set[str]] = {}
@@ -750,17 +754,22 @@
         for address, channel_id in self.central.device_details.device_channel_ids.items():
             if sections := channel_ids_function.get(channel_id):
                 if address not in functions:
                     functions[address] = set()
                 functions[address].update(sections)
         return functions
 
-    async def get_serial(self) -> str:
-        """Get the serial of the backend."""
-        return await self._json_rpc_client.get_serial()
+    async def _get_system_information(self) -> SystemInformation:
+        """Get system information of the backend."""
+        return SystemInformation(
+            available_interfaces=await self._json_rpc_client.get_available_interfaces(),
+            auth_enabled=await self._json_rpc_client.get_auth_enabled(),
+            https_redirect_enabled=await self._json_rpc_client.get_https_redirect_enabled(),
+            serial=await self._json_rpc_client.get_serial(),
+        )
 
 
 class ClientHomegear(Client):
     """Client implementation for Homegear backend."""
 
     @property
     def model(self) -> str:
@@ -844,33 +853,31 @@
             if hg_variables := await self._proxy.getAllSystemVariables():
                 for name, value in hg_variables.items():
                     variables.append(SystemVariableData(name=name, value=value))
         except BaseHomematicException as hhe:
             _LOGGER.warning("GET_ALL_SYSTEM_VARIABLES failed: %s [%s]", hhe.name, hhe.args)
         return variables
 
-    async def get_available_interfaces(self) -> list[str]:
-        """Get all available interfaces from CCU / Homegear."""
-        return [IF_BIDCOS_RF_NAME]
-
     async def get_all_programs(self, include_internal: bool) -> list[ProgramData]:
         """Get all programs, if available."""
         return []
 
     async def get_all_rooms(self) -> dict[str, set[str]]:
         """Get all rooms from Homegear."""
         return {}
 
     async def get_all_functions(self) -> dict[str, set[str]]:
         """Get all functions from Homegear."""
         return {}
 
-    async def get_serial(self) -> str:
-        """Get the serial of the backend."""
-        return "Homegear_SN0815"
+    async def _get_system_information(self) -> SystemInformation:
+        """Get system information of the backend."""
+        return SystemInformation(
+            available_interfaces=[IF_BIDCOS_RF_NAME], serial="Homegear_SN0815"
+        )
 
 
 class ClientLocal(Client):  # pragma: no cover
     """Local client object to provide access to locally stored files."""
 
     _paramset_descriptions_cache: dict[str, Any] = {}
 
@@ -934,33 +941,29 @@
         """Get single system variable from CCU / Homegear."""
         return "Empty"
 
     async def get_all_system_variables(self, include_internal: bool) -> list[SystemVariableData]:
         """Get all system variables from CCU / Homegear."""
         return []
 
-    async def get_available_interfaces(self) -> list[str]:
-        """Get all available interfaces from CCU / Homegear."""
-        return [LOCAL_INTERFACE]
-
     async def get_all_programs(self, include_internal: bool) -> list[ProgramData]:
         """Get all programs, if available."""
         return []
 
     async def get_all_rooms(self) -> dict[str, set[str]]:
         """Get all rooms, if available."""
         return {}
 
     async def get_all_functions(self) -> dict[str, set[str]]:
         """Get all functions, if available."""
         return {}
 
-    async def get_serial(self) -> str:
-        """Get the serial of the backend."""
-        return LOCAL_SERIAL
+    async def _get_system_information(self) -> SystemInformation:
+        """Get system information of the backend."""
+        return SystemInformation(available_interfaces=[LOCAL_INTERFACE], serial=LOCAL_SERIAL)
 
     async def get_all_device_descriptions(self) -> Any:
         """Get device descriptions from CCU / Homegear."""
         local_resources = self._config.interface_config.local_resources
         if not local_resources:
             _LOGGER.warning(
                 "GET_ALL_DEVICE_DESCRIPTIONS: missing local_resources in config for %s",
@@ -1114,14 +1117,16 @@
     def __init__(
         self,
         central: hmcu.CentralUnit,
         interface_config: InterfaceConfig,
         local_ip: str,
     ) -> None:
         self.central: Final = central
+        self.version: str = "0"
+        self.system_information = SystemInformation()
         self.interface_config: Final = interface_config
         self.interface: Final = interface_config.interface
         self.interface_id: Final = interface_config.interface_id
         self._callback_host: Final[str] = (
             central.config.callback_host if central.config.callback_host else local_ip
         )
         self._callback_port: Final[int] = (
@@ -1133,66 +1138,84 @@
         self.init_url: Final[str] = f"http://{self._callback_host}:{self._callback_port}"
         self.xml_rpc_uri: Final = build_xml_rpc_uri(
             host=central.config.host,
             port=interface_config.port,
             path=interface_config.remote_path,
             tls=central.config.tls,
         )
-        xml_rpc_headers: Final = build_headers(
-            username=central.config.username,
-            password=central.config.password,
-        )
-        self.xml_rpc_proxy: Final[XmlRpcProxy] = XmlRpcProxy(
-            max_workers=1,
-            interface_id=self.interface_id,
-            connection_state=central.config.connection_state,
-            uri=self.xml_rpc_uri,
-            headers=xml_rpc_headers,
-            tls=central.config.tls,
-            verify_tls=central.config.verify_tls,
-        )
-        self.xml_rpc_proxy_read: Final[XmlRpcProxy] = XmlRpcProxy(
-            max_workers=1,
-            interface_id=self.interface_id,
-            connection_state=central.config.connection_state,
-            uri=self.xml_rpc_uri,
-            headers=xml_rpc_headers,
-            tls=central.config.tls,
-            verify_tls=central.config.verify_tls,
-        )
-        self.version: str = "0"
-        self.serial: str = "0"
 
     async def get_client(self) -> Client:
         """Identify the used client."""
+        client: Client | None = None
+        if self.interface_config.local_resources:
+            client = ClientLocal(client_config=self)
+            await client.init_client()
+            return client
+        check_proxy = self._get_simple_xml_rpc_proxy()
         try:
-            client: Client | None = None
-            if self.interface_config.local_resources:
-                return ClientLocal(client_config=self)
-            methods = await self.xml_rpc_proxy.system.listMethods()
-            if methods and "getVersion" not in methods:
+            if methods := await check_proxy.system.listMethods():
                 # BidCos-Wired does not support getVersion()
-                client = ClientCCU(client_config=self)
-            elif version := await self.xml_rpc_proxy.getVersion():
-                self.version = cast(str, version)
-                if "Homegear" in version or "pydevccu" in version:
-                    client = ClientHomegear(client_config=self)
-            if not client:
-                client = ClientCCU(client_config=self)
-            if await client.check_connection_availability():
-                self.serial = await client.get_serial()
-                return client
+                self.version = (
+                    cast(str, await check_proxy.getVersion()) if "getVersion" in methods else "0"
+                )
+
+            if client := (
+                ClientHomegear(client_config=self)
+                if "Homegear" in self.version or "pydevccu" in self.version
+                else ClientCCU(client_config=self)
+            ):
+                await client.init_client()
+                if await client.check_connection_availability():
+                    return client
             raise NoConnection(f"No connection to {self.interface_id}")
         except AuthFailure as auf:
             raise AuthFailure(f"Unable to authenticate {auf.args}.") from auf
         except NoConnection as noc:
             raise noc
         except Exception as exc:
             raise NoConnection(f"Unable to connect {exc.args}.") from exc
 
+    def get_xml_rpc_proxy(self, auth_enabled: bool | None = None) -> XmlRpcProxy:
+        """Return a XmlRPC proxy for backend communication."""
+        central_config = self.central.config
+        xml_rpc_headers = (
+            build_headers(
+                username=central_config.username,
+                password=central_config.password,
+            )
+            if auth_enabled
+            else []
+        )
+        return XmlRpcProxy(
+            max_workers=1,
+            interface_id=self.interface_id,
+            connection_state=central_config.connection_state,
+            uri=self.xml_rpc_uri,
+            headers=xml_rpc_headers,
+            tls=central_config.tls,
+            verify_tls=central_config.verify_tls,
+        )
+
+    def _get_simple_xml_rpc_proxy(self) -> XmlRpcProxy:
+        """Return a XmlRPC proxy for backend communication."""
+        central_config = self.central.config
+        xml_rpc_headers = build_headers(
+            username=central_config.username,
+            password=central_config.password,
+        )
+        return XmlRpcProxy(
+            max_workers=0,
+            interface_id=self.interface_id,
+            connection_state=central_config.connection_state,
+            uri=self.xml_rpc_uri,
+            headers=xml_rpc_headers,
+            tls=central_config.tls,
+            verify_tls=central_config.verify_tls,
+        )
+
 
 class InterfaceConfig:
     """interface config for a Client."""
 
     def __init__(
         self,
         central_name: str,
```

### Comparing `hahomematic-2023.7.4/hahomematic/const.py` & `hahomematic-2023.7.5/hahomematic/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """Constants used by hahomematic."""
 from __future__ import annotations
 
 from datetime import datetime
-from enum import IntEnum
+from enum import IntEnum, StrEnum
 from typing import Final
 
-from hahomematic.backport import StrEnum
-
 DEFAULT_CONNECTION_CHECKER_INTERVAL: Final = (
     15  # check if connection is available via rpc ping every:
 )
 DEFAULT_ENCODING: Final = "UTF-8"
 DEFAULT_PING_PONG_MISMATCH_COUNT: Final = 10
 DEFAULT_RECONNECT_WAIT: Final = 120  # wait with reconnect after a first ping was successful
 DEFAULT_TIMEOUT: Final = 60  # default timeout for a connection
```

### Comparing `hahomematic-2023.7.4/hahomematic/decorators.py` & `hahomematic-2023.7.5/hahomematic/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/exceptions.py` & `hahomematic-2023.7.5/hahomematic/exceptions.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/exporter.py` & `hahomematic-2023.7.5/hahomematic/exporter.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/hmcli.py` & `hahomematic-2023.7.5/hahomematic/hmcli.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/json_rpc_client.py` & `hahomematic-2023.7.5/hahomematic/json_rpc_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -652,14 +652,42 @@
                     )
 
         except BaseHomematicException as hhe:
             _LOGGER.warning("GET_ALL_PROGRAMS failed: %s [%s]", hhe.name, hhe.args)
 
         return all_programs
 
+    async def get_auth_enabled(self) -> bool | None:
+        """Get the auth_enabled flag of the backend."""
+        auth_enabled: bool | None = None
+        _LOGGER.debug("GET_AUTH_ENABLED: Getting the flag auth_enabled via JSON-RPC")
+        try:
+            response = await self._post(method="CCU.getAuthEnabled")
+            if (json_result := response[ATTR_RESULT]) is not None:
+                auth_enabled = bool(json_result)
+        except BaseHomematicException as hhe:
+            _LOGGER.warning("GET_AUTH_ENABLED failed: %s [%s]", hhe.name, hhe.args)
+
+        return auth_enabled
+
+    async def get_https_redirect_enabled(self) -> bool | None:
+        """Get the auth_enabled flag of the backend."""
+        https_redirect_enabled: bool | None = None
+        _LOGGER.debug(
+            "GET_HTTPS_REDIRECT_ENABLED: Getting the flag https_redirect_enabled via JSON-RPC"
+        )
+        try:
+            response = await self._post(method="CCU.getHttpsRedirectEnabled")
+            if (json_result := response[ATTR_RESULT]) is not None:
+                https_redirect_enabled = bool(json_result)
+        except BaseHomematicException as hhe:
+            _LOGGER.warning("GET_HTTPS_REDIRECT_ENABLED failed: %s [%s]", hhe.name, hhe.args)
+
+        return https_redirect_enabled
+
     async def get_serial(self) -> str:
         """Get the serial of the backend."""
         serial = "unknown"
         _LOGGER.debug("GET_SERIAL: Getting the backend serial via JSON-RPC")
         try:
             response = await self._post_script(script_name=REGA_SCRIPT_GET_SERIAL)
             if json_result := response[ATTR_RESULT]:
```

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/__init__.py` & `hahomematic-2023.7.5/hahomematic/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/custom/__init__.py` & `hahomematic-2023.7.5/hahomematic/platforms/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/custom/climate.py` & `hahomematic-2023.7.5/hahomematic/platforms/custom/climate.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 Module for entities implemented using the climate platform.
 
 See https://www.home-assistant.io/integrations/climate/.
 """
 from __future__ import annotations
 
 from datetime import datetime, timedelta
+from enum import StrEnum
 import logging
 from typing import Any, Final
 
-from hahomematic.backport import StrEnum
 from hahomematic.const import HmPlatform
 from hahomematic.decorators import bind_collector
 from hahomematic.platforms import device as hmd
 from hahomematic.platforms.custom import definition as hmed
 from hahomematic.platforms.custom.const import (
     FIELD_ACTIVE_PROFILE,
     FIELD_AUTO_MODE,
```

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/custom/const.py` & `hahomematic-2023.7.5/hahomematic/platforms/custom/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Constants used by hahomematic custom entities."""
 from __future__ import annotations
 
+from enum import StrEnum
 from typing import Final
 
-from hahomematic.backport import StrEnum
-
 
 class HmEntityDefinition(StrEnum):
     """Enum for entity definitions."""
 
     IP_COVER = "IPCover"
     IP_DIMMER = "IPDimmer"
     IP_FIXED_COLOR_LIGHT = "IPFixedColorLight"
```

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/custom/cover.py` & `hahomematic-2023.7.5/hahomematic/platforms/custom/cover.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/custom/definition.py` & `hahomematic-2023.7.5/hahomematic/platforms/custom/definition.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/custom/entity.py` & `hahomematic-2023.7.5/hahomematic/platforms/custom/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/custom/light.py` & `hahomematic-2023.7.5/hahomematic/platforms/custom/light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/custom/lock.py` & `hahomematic-2023.7.5/hahomematic/platforms/custom/lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/custom/siren.py` & `hahomematic-2023.7.5/hahomematic/platforms/custom/siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/custom/support.py` & `hahomematic-2023.7.5/hahomematic/platforms/custom/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/custom/switch.py` & `hahomematic-2023.7.5/hahomematic/platforms/custom/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/device.py` & `hahomematic-2023.7.5/hahomematic/platforms/device.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/entity.py` & `hahomematic-2023.7.5/hahomematic/platforms/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/event.py` & `hahomematic-2023.7.5/hahomematic/platforms/event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/generic/__init__.py` & `hahomematic-2023.7.5/hahomematic/platforms/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/generic/action.py` & `hahomematic-2023.7.5/hahomematic/platforms/generic/action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/generic/binary_sensor.py` & `hahomematic-2023.7.5/hahomematic/platforms/generic/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/generic/button.py` & `hahomematic-2023.7.5/hahomematic/platforms/generic/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/generic/entity.py` & `hahomematic-2023.7.5/hahomematic/platforms/generic/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/generic/number.py` & `hahomematic-2023.7.5/hahomematic/platforms/generic/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/generic/select.py` & `hahomematic-2023.7.5/hahomematic/platforms/generic/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/generic/sensor.py` & `hahomematic-2023.7.5/hahomematic/platforms/generic/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/generic/switch.py` & `hahomematic-2023.7.5/hahomematic/platforms/generic/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/hub/__init__.py` & `hahomematic-2023.7.5/hahomematic/platforms/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/hub/binary_sensor.py` & `hahomematic-2023.7.5/hahomematic/platforms/hub/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/hub/button.py` & `hahomematic-2023.7.5/hahomematic/platforms/hub/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/hub/entity.py` & `hahomematic-2023.7.5/hahomematic/platforms/hub/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/hub/number.py` & `hahomematic-2023.7.5/hahomematic/platforms/hub/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/hub/select.py` & `hahomematic-2023.7.5/hahomematic/platforms/hub/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/hub/sensor.py` & `hahomematic-2023.7.5/hahomematic/platforms/hub/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/hub/text.py` & `hahomematic-2023.7.5/hahomematic/platforms/hub/text.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/support.py` & `hahomematic-2023.7.5/hahomematic/platforms/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/platforms/update.py` & `hahomematic-2023.7.5/hahomematic/platforms/update.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/rega_scripts/fetch_all_device_data.fn` & `hahomematic-2023.7.5/hahomematic/rega_scripts/fetch_all_device_data.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/rega_scripts/get_serial.fn` & `hahomematic-2023.7.5/hahomematic/rega_scripts/get_serial.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/rega_scripts/get_system_variables_ext_marker.fn` & `hahomematic-2023.7.5/hahomematic/rega_scripts/get_system_variables_ext_marker.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic/support.py` & `hahomematic-2023.7.5/hahomematic/support.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Helper functions used within hahomematic."""
 from __future__ import annotations
 
 import base64
 from collections.abc import Collection
 from contextlib import closing
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from datetime import datetime
 from functools import cache
 import logging
 import os
 import re
 import socket
 import ssl
@@ -261,14 +261,24 @@
     value: bool | float | int | str | None = None
     value_list: list[str] | None = None
     max_value: float | int | None = None
     min_value: float | int | None = None
     extended_sysvar: bool = False
 
 
+@dataclass
+class SystemInformation:
+    """System information of the backend."""
+
+    available_interfaces: list[str] = field(default_factory=list)
+    auth_enabled: bool | None = None
+    https_redirect_enabled: bool | None = None
+    serial: str | None = None
+
+
 def cleanup_cache_dirs(instance_name: str, storage_folder: str) -> None:
     """Clean up the used cached directories."""
     cache_dir = f"{storage_folder}/cache"
     files_to_delete = [FILE_DEVICES, FILE_PARAMSETS]
 
     def _delete_file(file_name: str) -> None:
         if os.path.exists(os.path.join(cache_dir, file_name)):
```

### Comparing `hahomematic-2023.7.4/hahomematic/xml_rpc_proxy.py` & `hahomematic-2023.7.5/hahomematic/xml_rpc_proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,16 +52,18 @@
         **kwargs: Any,
     ) -> None:
         """Initialize new proxy for server and get local ip."""
         self._tasks: Final[set[asyncio.Future[Any]]] = set()
         self.interface_id: Final = interface_id
         self._connection_state: Final = connection_state
         self._loop: Final = asyncio.get_running_loop()
-        self._proxy_executor: Final = ThreadPoolExecutor(
-            max_workers=max_workers, thread_name_prefix=interface_id
+        self._proxy_executor: Final = (
+            ThreadPoolExecutor(max_workers=max_workers, thread_name_prefix=interface_id)
+            if max_workers > 0
+            else None
         )
         self._tls: Final[bool] = kwargs.pop(ATTR_TLS, False)
         self._verify_tls: Final[bool] = kwargs.pop(ATTR_VERIFY_TLS, True)
         if self._tls:
             kwargs[ATTR_CONTEXT] = get_tls_context(self._verify_tls)
         xmlrpc.client.ServerProxy.__init__(  # type: ignore[misc]
             self, encoding=ATTR_ENCODING_ISO_8859_1, *args, **kwargs
@@ -119,8 +121,9 @@
 
     def __getattr__(self, *args, **kwargs):  # type: ignore[no-untyped-def]
         """Magic method dispatcher."""
         return xmlrpc.client._Method(self.__async_request, *args, **kwargs)
 
     def stop(self) -> None:
         """Stop depending services."""
-        self._proxy_executor.shutdown()
+        if self._proxy_executor:
+            self._proxy_executor.shutdown()
```

### Comparing `hahomematic-2023.7.4/hahomematic/xml_rpc_server.py` & `hahomematic-2023.7.5/hahomematic/xml_rpc_server.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.4/hahomematic.egg-info/PKG-INFO` & `hahomematic-2023.7.5/hahomematic.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.7.4
+Version: 2023.7.5
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
@@ -12,24 +12,23 @@
 Keywords: home,automation,homematic
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Home Automation
-Requires-Python: >=3.10.0
+Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hahomematic
 
-`hahomematic` is a Python 3 (>= 3.10) module for [Home Assistant](https://www.home-assistant.io/) to interact with [HomeMatic](https://www.eq-3.com/products/homematic.html) and [HomematicIP](https://www.homematic-ip.com/en/start.html) devices. Some other devices (f.ex. Bosch, Intertechno) might be supported as well.
+`hahomematic` is a Python 3 (>= 3.11) module for [Home Assistant](https://www.home-assistant.io/) to interact with [HomeMatic](https://www.eq-3.com/products/homematic.html) and [HomematicIP](https://www.homematic-ip.com/en/start.html) devices. Some other devices (f.ex. Bosch, Intertechno) might be supported as well.
 
 This is intended to become the successor of [pyhomematic](https://github.com/danielperna84/pyhomematic).
 
 It can be installed by using the [custom_component](https://github.com/danielperna84/custom_homematic).
 Necessary installation instructions can be found [here](https://github.com/danielperna84/custom_homematic/wiki/Installation).
 
 ## Project goal and features
```

### Comparing `hahomematic-2023.7.4/hahomematic.egg-info/SOURCES.txt` & `hahomematic-2023.7.5/hahomematic.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 hahomematic/__init__.py
-hahomematic/backport.py
 hahomematic/central_unit.py
 hahomematic/client.py
 hahomematic/config.py
 hahomematic/const.py
 hahomematic/decorators.py
 hahomematic/exceptions.py
 hahomematic/exporter.py
```

### Comparing `hahomematic-2023.7.4/pyproject.toml` & `hahomematic-2023.7.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "hahomematic"
-version     = "2023.7.4"
+version     = "2023.7.5"
 license     = {text = "MIT License"}
 description = "Homematic interface for Home Assistant running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Daniel Perna", email = "danielperna84@gmail.com"},
     {name = "SukramJ", email = "sukramj@icloud.com"},
 ]
 keywords    = ["home", "automation", "homematic"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: End Users/Desktop",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Home Automation",
 ]
-requires-python = ">=3.10.0"
+requires-python = ">=3.11.0"
 dependencies    = [
     "aiohttp>=3.8.4",
     "orjson>=3.9.1",
     "python-slugify>=4.0.1",
     "voluptuous>=0.13.1",
 ]
 
@@ -49,20 +48,20 @@
 include = ["hahomematic*"]
 exclude = ["tests", "tests.*", "dist", "build"]
 
 [tool.setuptools.package-data]
 hahomematic = ["py.typed", "rega_scripts/*.fn"]
 
 [tool.black]
-target-version = ["py310", "py311"]
+target-version = ["py311"]
 exclude = 'generated'
 line-length = 99
 
 [tool.pylint.MAIN]
-py-version = "3.10"
+py-version = "3.11"
 ignore = [
     "tests",
 ]
 extension-pkg-whitelist= ["orjson"]
 # Use a conservative default here; 2 should speed up most setups and not hurt
 # any too bad. Override on command line as appropriate.
 jobs = 2
@@ -394,15 +393,15 @@
 norecursedirs = [
     ".git",
     "testing_config",
 ]
 asyncio_mode = "auto"
 
 [tool.ruff]
-target-version = "py310"
+target-version = "py311"
 line-length = 99
 
 
 select = [
     "B002", # Python does not support the unary prefix increment
     "B007", # Loop control variable {name} not used within loop body
     "B014", # Exception handler with duplicate exception
```

