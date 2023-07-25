# Comparing `tmp/dashio-3.3.7.tar.gz` & `tmp/dashio-3.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dashio-3.3.7.tar", last modified: Tue Jul 11 22:05:24 2023, max compression
+gzip compressed data, was "dashio-3.3.9.tar", last modified: Tue Jul 25 06:05:07 2023, max compression
```

## Comparing `dashio-3.3.7.tar` & `dashio-3.3.9.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:05:24.647575 dashio-3.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-11 22:05:15.000000 dashio-3.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-07-11 22:05:24.647575 dashio-3.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9743 2023-07-11 22:05:15.000000 dashio-3.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:05:24.639575 dashio-3.3.7/dashio/
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21460 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/action_station.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:05:24.639575 dashio-3.3.7/dashio/action_station_services/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/action_station_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/action_station_services/action_station_service_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/action_station_services/as_servicel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/action_station_services/clock_servicel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/action_station_services/modbus_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/action_station_services/task_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/action_station_services/timer_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/bleconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12853 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/dashconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)    22685 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:05:24.643575 dashio-3.3.7/dashio/iotcontrol/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/audio_visual_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/button_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/color_picker.py
--rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/device_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     8762 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/dial.py
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/event_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/knob.py
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/label.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/ring_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/slider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/textbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    12106 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/time_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/mqttconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/serialconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13036 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/tcpconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/zeroconf_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/zmqconnection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:05:24.639575 dashio-3.3.7/dashio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-07-11 22:05:24.000000 dashio-3.3.7/dashio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-11 22:05:24.000000 dashio-3.3.7/dashio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 22:05:24.000000 dashio-3.3.7/dashio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 22:05:24.000000 dashio-3.3.7/dashio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-11 22:05:24.000000 dashio-3.3.7/dashio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-11 22:05:24.000000 dashio-3.3.7/dashio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-11 22:05:15.000000 dashio-3.3.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-11 22:05:24.647575 dashio-3.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-11 22:05:15.000000 dashio-3.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:05:24.647575 dashio-3.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_button.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_button_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_control.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_dashconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_dashdevice.py
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_device_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_dial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_event_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_knob.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_mqttconntection.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_slider.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_tcpconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_textbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_time_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_zqmconnection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:05:24.647575 dashio-3.3.7/utilities/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1313 2023-07-11 22:05:15.000000 dashio-3.3.7/utilities/c64_decode
--rwxr-xr-x   0 runner    (1001) docker     (123)     1726 2023-07-11 22:05:15.000000 dashio-3.3.7/utilities/c64_encode
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:07.595159 dashio-3.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-25 06:04:55.000000 dashio-3.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-07-25 06:05:07.595159 dashio-3.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9743 2023-07-25 06:04:55.000000 dashio-3.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:07.579159 dashio-3.3.9/dashio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21460 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/action_station.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:07.583159 dashio-3.3.9/dashio/action_station_services/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/action_station_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/action_station_services/action_station_service_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/action_station_services/as_servicel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/action_station_services/clock_servicel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/action_station_services/modbus_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/action_station_services/task_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/action_station_services/timer_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/bleconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12853 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/dashconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22685 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:07.591159 dashio-3.3.9/dashio/iotcontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/audio_visual_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/button_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14604 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/device_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8788 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/dial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7880 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/event_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/knob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/ring_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/textbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12106 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/iotcontrol/time_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/mqttconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/serialconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13036 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/tcpconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/zeroconf_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-25 06:04:55.000000 dashio-3.3.9/dashio/zmqconnection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:07.583159 dashio-3.3.9/dashio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-07-25 06:05:07.000000 dashio-3.3.9/dashio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-25 06:05:07.000000 dashio-3.3.9/dashio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:05:07.000000 dashio-3.3.9/dashio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:05:07.000000 dashio-3.3.9/dashio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-25 06:05:07.000000 dashio-3.3.9/dashio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 06:05:07.000000 dashio-3.3.9/dashio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-25 06:04:55.000000 dashio-3.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-25 06:05:07.599159 dashio-3.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-25 06:04:55.000000 dashio-3.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:07.595159 dashio-3.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_button_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_dashconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_dashdevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_device_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_dial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_event_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_knob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_mqttconntection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_tcpconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_textbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_time_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 06:04:55.000000 dashio-3.3.9/tests/test_zqmconnection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:05:07.595159 dashio-3.3.9/utilities/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1313 2023-07-25 06:04:55.000000 dashio-3.3.9/utilities/c64_decode
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1726 2023-07-25 06:04:55.000000 dashio-3.3.9/utilities/c64_encode
```

### Comparing `dashio-3.3.7/LICENSE` & `dashio-3.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/PKG-INFO` & `dashio-3.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dashio
-Version: 3.3.7
+Version: 3.3.9
 Summary: DashIO interface library
 Home-page: https://dashio.io
 Download-URL: https://github.com/dashio-connect/python-dashio
 Author: James Boulton
 Author-email: james@dashio.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `dashio-3.3.7/README.md` & `dashio-3.3.9/README.md`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/__init__.py` & `dashio-3.3.9/dashio/__init__.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/action_station.py` & `dashio-3.3.9/dashio/action_station.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/action_station_services/action_station_service_config.py` & `dashio-3.3.9/dashio/action_station_services/action_station_service_config.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/action_station_services/as_servicel.py` & `dashio-3.3.9/dashio/action_station_services/as_servicel.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/action_station_services/clock_servicel.py` & `dashio-3.3.9/dashio/action_station_services/clock_servicel.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/action_station_services/modbus_service.py` & `dashio-3.3.9/dashio/action_station_services/modbus_service.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/action_station_services/task_service.py` & `dashio-3.3.9/dashio/action_station_services/task_service.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/action_station_services/timer_service.py` & `dashio-3.3.9/dashio/action_station_services/timer_service.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/bleconnection.py` & `dashio-3.3.9/dashio/bleconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/constants.py` & `dashio-3.3.9/dashio/constants.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/dashconnection.py` & `dashio-3.3.9/dashio/dashconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/device.py` & `dashio-3.3.9/dashio/device.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/iotcontrol/__init__.py` & `dashio-3.3.9/dashio/iotcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/iotcontrol/alarm.py` & `dashio-3.3.9/dashio/iotcontrol/alarm.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/iotcontrol/audio_visual_display.py` & `dashio-3.3.9/dashio/iotcontrol/audio_visual_display.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/iotcontrol/button.py` & `dashio-3.3.9/dashio/iotcontrol/button.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 from ..constants import BAD_CHARS
-from .control import Control, ControlPosition, ControlConfig, _get_color, _get_icon, _get_title_position, _get_button_style
+from .control import Control, ControlPosition, ControlConfig, _get_color, _get_icon, _get_title_position, _get_button_style, _get_color_str
 from .enums import ButtonState, Color, Icon, TitlePosition, ButtonStyle
 
 
 class ButtonConfig(ControlConfig):
     """ButtonGroupConfig"""
     def __init__(
         self,
@@ -42,16 +42,16 @@
         control_position: ControlPosition
     ) -> None:
         super().__init__(control_id, title, control_position, title_position)
         self.cfg["text"] = text.translate(BAD_CHARS)
         self.cfg["iconName"] = icon_name.value
         self.cfg["buttonEnabled"] = button_enabled
         self.cfg["style"] = str(style.value)
-        self.cfg["onColor"] = str(on_color.value)
-        self.cfg["offColor"] = str(off_color.value)
+        self.cfg["onColor"] = _get_color_str(on_color)
+        self.cfg["offColor"] = _get_color_str(off_color)
 
     @classmethod
     def from_dict(cls, cfg_dict: dict):
         """Instantiates ButtonGroupConfig from cfg dictionary
 
         Parameters
         ----------
```

### Comparing `dashio-3.3.7/dashio/iotcontrol/button_group.py` & `dashio-3.3.9/dashio/iotcontrol/button_group.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/iotcontrol/chart.py` & `dashio-3.3.9/dashio/iotcontrol/chart.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/iotcontrol/color_picker.py` & `dashio-3.3.9/dashio/iotcontrol/color_picker.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/iotcontrol/control.py` & `dashio-3.3.9/dashio/iotcontrol/control.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,23 @@
 
 
 def _get_icon(icon_str: str) -> Icon:
     icon_name = icon_str.upper().replace(" ", "")
     return Icon[icon_name]
 
 
+def _get_color_str(color) -> str:
+    if isinstance(color, str):
+        if color[0] == '#':
+            return color
+    return str(color.value)
+
 def _get_color(color_str: str) -> Color:
+    if color_str[0] == '#':
+        return color_str
     color_name = color_str.upper().replace(" ", "_")
     return Color[color_name]
 
 
 def _get_title_position(position_str: str) -> TitlePosition:
     t_pos_name = position_str.upper().replace(" ", "")
     return TitlePosition[t_pos_name]
```

### Comparing `dashio-3.3.7/dashio/iotcontrol/device_view.py` & `dashio-3.3.9/dashio/iotcontrol/device_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
-from .control import Control, ControlConfig, _get_color, _get_icon, _get_device_view_style
+from .control import Control, ControlConfig, _get_color, _get_icon, _get_device_view_style, _get_color_str
 from .enums import Color, Icon, DeviceViewStyle
 
 
 class DeviceViewConfig(ControlConfig):
     """DeviceViewConfig"""
     def __init__(
         self,
@@ -46,28 +46,28 @@
         control_background_transparency: int,
         num_grid_columns: int,
         num_grid_rows: int,
     ) -> None:
         super().__init__(control_id, title, control_position=None, title_position=None)
         self.cfg["iconName"] = icon_name.value
         self.cfg["style"] = str(style.value)
-        self.cfg["color"] = str(color.value)
+        self.cfg["color"] = _get_color_str(color)
         self.cfg["shareColumn"] = share_column
         if 1 <= num_columns <= 10:
             self.cfg["numColumns"] = num_columns
         else:
             raise ValueError("num_columns must be in the range 1 to 10")
-        self.cfg["ctrlTitleBoxColor"] = str(control_title_box_color.value)
+        self.cfg["ctrlTitleBoxColor"] = _get_color_str(control_title_box_color)
         if 0 <= control_title_box_transparency <= 100:
             self.cfg["ctrlTitleBoxTransparency"] = control_title_box_transparency
         else:
             raise ValueError("Value must be in the range 0 to 100")
-        self.cfg["ctrlColor"] = str(control_color.value)
-        self.cfg["ctrlBorderColor"] = str(control_border_color.value)
-        self.cfg["ctrlBkgndColor"] = str(control_background_color.value)
+        self.cfg["ctrlColor"] = _get_color_str(control_color)
+        self.cfg["ctrlBorderColor"] = _get_color_str(control_border_color)
+        self.cfg["ctrlBkgndColor"] = _get_color_str(control_background_color)
         self.cfg["ctrlTitleFontSize"] = control_title_font_size
         self.cfg["ctrlMaxFontSize"] = control_max_font_size
         if 0 <= control_background_transparency <= 100:
             self.cfg["ctrlBkgndTransparency"] = control_background_transparency
         else:
             raise ValueError("Value must be in the range 0 to 100")
         self.cfg["gridColumns"] = num_grid_columns
```

### Comparing `dashio-3.3.7/dashio/iotcontrol/dial.py` & `dashio-3.3.9/dashio/iotcontrol/dial.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
-from .control import Control, ControlPosition, ControlConfig, _get_color, _get_title_position, _get_dial_number_position, _get_dial_style, _get_precision
+from .control import Control, ControlPosition, ControlConfig, _get_color, _get_title_position, _get_dial_number_position, _get_dial_style, _get_precision, _get_color_str
 from .enums import (Color, DialNumberPosition, DialStyle, Precision,
                     TitlePosition)
 
 
 class DialConfig(ControlConfig):
     """DialConfig"""
     def __init__(
@@ -45,16 +45,16 @@
         units: str,
         control_position: ControlPosition
     ) -> None:
         super().__init__(control_id, title, control_position, title_position)
         self.cfg["min"] = dial_min
         self.cfg["max"] = dial_max
         self.cfg["redValue"] = red_value
-        self.cfg["dialFillColor"] = str(dial_fill_color.value)
-        self.cfg["pointerColor"] = str(pointer_color.value)
+        self.cfg["dialFillColor"] = _get_color_str(dial_fill_color)
+        self.cfg["pointerColor"] = _get_color_str(pointer_color)
         self.cfg["numberPosition"] = number_position.value
         self.cfg["showMinMax"] = show_min_max
         self.cfg["style"] = style.value
         self.cfg["precision"] = precision.value
         self.cfg["units"] = units
 
     @classmethod
```

### Comparing `dashio-3.3.7/dashio/iotcontrol/direction.py` & `dashio-3.3.9/dashio/iotcontrol/direction.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 from ..constants import BAD_CHARS
-from .control import Control, ControlPosition, ControlConfig, _get_color, _get_title_position, _get_direction_style, _get_precision
+from .control import Control, ControlPosition, ControlConfig, _get_color, _get_title_position, _get_direction_style, _get_precision, _get_color_str
 from .enums import Color, DirectionStyle, Precision, TitlePosition
 
 
 class DirectionConfig(ControlConfig):
     """DirectionConfig"""
     def __init__(
         self,
@@ -38,15 +38,15 @@
         units: str,
         precision: Precision,
         calibration_angle: float,
         control_position: ControlPosition
     ) -> None:
         super().__init__(control_id, title, control_position, title_position)
         self.cfg["style"] = str(style.value)
-        self.cfg["pointerColor"] = str(pointer_color.value)
+        self.cfg["pointerColor"] = _get_color_str(pointer_color)
         self.cfg["units"] = units
         self.cfg["precision"] = precision.value
         self.cfg["calAngle"] = calibration_angle
 
     @classmethod
     def from_dict(cls, cfg_dict: dict):
         """Instantiates DirectionConfig from cfg dictionary
```

### Comparing `dashio-3.3.7/dashio/iotcontrol/enums.py` & `dashio-3.3.9/dashio/iotcontrol/enums.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/iotcontrol/event.py` & `dashio-3.3.9/dashio/iotcontrol/event.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/iotcontrol/event_log.py` & `dashio-3.3.9/dashio/iotcontrol/event_log.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/iotcontrol/knob.py` & `dashio-3.3.9/dashio/iotcontrol/knob.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
-from .control import Control, ControlPosition, ControlConfig, _get_color, _get_title_position, _get_knob_style
+from .control import Control, ControlPosition, ControlConfig, _get_color, _get_title_position, _get_knob_style, _get_color_str
 from .enums import Color, KnobStyle, TitlePosition
 
 
 class KnobConfig(ControlConfig):
     """KnobConfig"""
     def __init__(
         self,
@@ -47,16 +47,16 @@
         self.cfg["style"] = str(knob_style.value)
         self.cfg["min"] = dial_min
         self.cfg["max"] = dial_max
         self.cfg["redValue"] = red_value
         self.cfg["showMinMax"] = show_min_max
         self.cfg["sendOnlyOnRelease"] = send_only_on_release
         self.cfg["dialFollowsKnob"] = dial_follows_knob
-        self.cfg["dialColor"] = str(dial_color.value)
-        self.cfg["knobColor"] = str(knob_color.value)
+        self.cfg["dialColor"] = _get_color_str(dial_color)
+        self.cfg["knobColor"] = _get_color_str(knob_color)
 
     @classmethod
     def from_dict(cls, cfg_dict: dict):
         """Instantiates KnobConfig from cfg dictionary
 
         Parameters
         ----------
```

### Comparing `dashio-3.3.7/dashio/iotcontrol/label.py` & `dashio-3.3.9/dashio/iotcontrol/label.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
-from .control import Control, ControlPosition, ControlConfig, _get_color, _get_title_position, _get_label_style
+from .control import Control, ControlPosition, ControlConfig, _get_color, _get_title_position, _get_label_style, _get_color_str
 from .enums import Color, LabelStyle, TitlePosition
 
 
 class LabelConfig(ControlConfig):
     """LabelConfig"""
     def __init__(
         self,
@@ -34,15 +34,15 @@
         title_position: TitlePosition,
         color: Color,
         style: LabelStyle,
         control_position: ControlPosition
     ) -> None:
         super().__init__(control_id, title, control_position, title_position)
         self.cfg["style"] = style.value
-        self.cfg["color"] = str(color.value)
+        self.cfg["color"] = _get_color_str(color)
 
     @classmethod
     def from_dict(cls, cfg_dict: dict):
         """Instantiates LabelConfig from cfg dictionary
 
         Parameters
         ----------
```

### Comparing `dashio-3.3.7/dashio/iotcontrol/map.py` & `dashio-3.3.9/dashio/iotcontrol/map.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/iotcontrol/menu.py` & `dashio-3.3.9/dashio/iotcontrol/menu.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/iotcontrol/ring_buffer.py` & `dashio-3.3.9/dashio/iotcontrol/ring_buffer.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/iotcontrol/selector.py` & `dashio-3.3.9/dashio/iotcontrol/selector.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/iotcontrol/slider.py` & `dashio-3.3.9/dashio/iotcontrol/slider.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
-from .control import Control, ControlPosition, ControlConfig, _get_title_position, _get_color, _get_bar_style
+from .control import Control, ControlPosition, ControlConfig, _get_title_position, _get_color, _get_bar_style, _get_color_str
 from .enums import Color, SliderBarStyle, TitlePosition
 
 
 class SliderConfig(ControlConfig):
     """SliderConfig"""
     def __init__(
         self,
@@ -48,16 +48,16 @@
         self.cfg["redValue"] = red_value
         self.cfg["min"] = bar_min
         self.cfg["max"] = bar_max
         self.cfg["showMinMax"] = show_min_max
         self.cfg["sliderEnabled"] = slider_enabled
         self.cfg["sendOnlyOnRelease"] = send_only_on_release
         self.cfg["barFollowsSlider"] = bar_follows_slider
-        self.cfg["barColor"] = str(bar_color.value)
-        self.cfg["knobColor"] = str(knob_color.value)
+        self.cfg["barColor"] = _get_color_str(bar_color)
+        self.cfg["knobColor"] = _get_color_str(knob_color)
         self.cfg["barStyle"] = bar_style.value
 
     @classmethod
     def from_dict(cls, cfg_dict: dict):
         """Instantiates SliderConfig from cfg dictionary
 
         Parameters
```

### Comparing `dashio-3.3.7/dashio/iotcontrol/textbox.py` & `dashio-3.3.9/dashio/iotcontrol/textbox.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/iotcontrol/time_graph.py` & `dashio-3.3.9/dashio/iotcontrol/time_graph.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/ip.py` & `dashio-3.3.9/dashio/ip.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/load_config.py` & `dashio-3.3.9/dashio/load_config.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/mqttconnection.py` & `dashio-3.3.9/dashio/mqttconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/serialconnection.py` & `dashio-3.3.9/dashio/serialconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/tcpconnection.py` & `dashio-3.3.9/dashio/tcpconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/zeroconf_service.py` & `dashio-3.3.9/dashio/zeroconf_service.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio/zmqconnection.py` & `dashio-3.3.9/dashio/zmqconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/dashio.egg-info/PKG-INFO` & `dashio-3.3.9/dashio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dashio
-Version: 3.3.7
+Version: 3.3.9
 Summary: DashIO interface library
 Home-page: https://dashio.io
 Download-URL: https://github.com/dashio-connect/python-dashio
 Author: James Boulton
 Author-email: james@dashio.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `dashio-3.3.7/dashio.egg-info/SOURCES.txt` & `dashio-3.3.9/dashio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/setup.cfg` & `dashio-3.3.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/setup.py` & `dashio-3.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="dashio",
-    version="3.3.7",
+    version="3.3.9",
     description="DashIO interface library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="James Boulton",
     author_email="james@dashio.com",
     url="https://dashio.io",
     download_url="https://github.com/dashio-connect/python-dashio",
```

### Comparing `dashio-3.3.7/tests/test_button.py` & `dashio-3.3.9/tests/test_button.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/tests/test_button_group.py` & `dashio-3.3.9/tests/test_button_group.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/tests/test_chart.py` & `dashio-3.3.9/tests/test_chart.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/tests/test_dashdevice.py` & `dashio-3.3.9/tests/test_dashdevice.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/tests/test_device_view.py` & `dashio-3.3.9/tests/test_device_view.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/tests/test_dial.py` & `dashio-3.3.9/tests/test_dial.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/tests/test_direction.py` & `dashio-3.3.9/tests/test_direction.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/tests/test_event_log.py` & `dashio-3.3.9/tests/test_event_log.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/tests/test_knob.py` & `dashio-3.3.9/tests/test_knob.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/tests/test_label.py` & `dashio-3.3.9/tests/test_label.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/tests/test_map.py` & `dashio-3.3.9/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/tests/test_menu.py` & `dashio-3.3.9/tests/test_menu.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/tests/test_selector.py` & `dashio-3.3.9/tests/test_selector.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/tests/test_slider.py` & `dashio-3.3.9/tests/test_slider.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/tests/test_textbox.py` & `dashio-3.3.9/tests/test_textbox.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/tests/test_time_graph.py` & `dashio-3.3.9/tests/test_time_graph.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/utilities/c64_decode` & `dashio-3.3.9/utilities/c64_decode`

 * *Files identical despite different names*

### Comparing `dashio-3.3.7/utilities/c64_encode` & `dashio-3.3.9/utilities/c64_encode`

 * *Files identical despite different names*

