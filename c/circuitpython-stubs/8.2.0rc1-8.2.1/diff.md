# Comparing `tmp/circuitpython-stubs-8.2.0rc1.tar.gz` & `tmp/circuitpython-stubs-8.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-stubs-8.2.0rc1.tar", last modified: Tue Jun 27 17:31:04 2023, max compression
+gzip compressed data, was "circuitpython-stubs-8.2.1.tar", last modified: Tue Jul 25 16:37:31 2023, max compression
```

## Comparing `circuitpython-stubs-8.2.0rc1.tar` & `circuitpython-stubs-8.2.1.tar`

### file list

```diff
@@ -1,232 +1,232 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.766423 circuitpython-stubs-8.2.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-27 17:30:56.000000 circuitpython-stubs-8.2.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-27 17:31:04.766423 circuitpython-stubs-8.2.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-27 17:30:56.000000 circuitpython-stubs-8.2.0rc1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/_bleio/
--rw-r--r--   0 runner    (1001) docker     (123)    31094 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/_bleio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/_eve/
--rw-r--r--   0 runner    (1001) docker     (123)    20379 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/_eve/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/_pew/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/_pew/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/_pixelmap/
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/_pixelmap/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/_stage/
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/_stage/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/adafruit_bus_device/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/adafruit_bus_device/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/adafruit_bus_device/i2c_device/
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/adafruit_bus_device/i2c_device/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/adafruit_bus_device/spi_device/
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/adafruit_bus_device/spi_device/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/adafruit_pixelbuf/
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/adafruit_pixelbuf/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/aesio/
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/aesio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/alarm/
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/alarm/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/alarm/pin/
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/alarm/pin/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/alarm/time/
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/alarm/time/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/alarm/touch/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/alarm/touch/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/analogbufio/
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/analogbufio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/analogio/
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/analogio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/atexit/
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/atexit/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.750423 circuitpython-stubs-8.2.0rc1/audiobusio/
--rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-06-27 17:30:53.000000 circuitpython-stubs-8.2.0rc1/audiobusio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/audiocore/
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/audiocore/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/audioio/
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/audioio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/audiomixer/
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/audiomixer/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/audiomp3/
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/audiomp3/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/audiopwmio/
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/audiopwmio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/bitbangio/
--rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/bitbangio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/bitmaptools/
--rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/bitmaptools/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/bitops/
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/bitops/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/board/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/board/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/busio/
--rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/busio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/camera/
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/camera/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/canio/
--rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/canio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/circuitpython_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-27 17:31:04.000000 circuitpython-stubs-8.2.0rc1/circuitpython_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-06-27 17:31:04.000000 circuitpython-stubs-8.2.0rc1/circuitpython_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:31:04.000000 circuitpython-stubs-8.2.0rc1/circuitpython_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:31:04.000000 circuitpython-stubs-8.2.0rc1/circuitpython_stubs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-27 17:31:04.000000 circuitpython-stubs-8.2.0rc1/circuitpython_stubs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/countio/
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/countio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/cyw43/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-27 17:30:56.000000 circuitpython-stubs-8.2.0rc1/cyw43/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/digitalio/
--rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/digitalio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/displayio/
--rw-r--r--   0 runner    (1001) docker     (123)    40379 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/displayio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/dualbank/
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/dualbank/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/espcamera/
--rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-06-27 17:30:56.000000 circuitpython-stubs-8.2.0rc1/espcamera/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/espidf/
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-27 17:30:56.000000 circuitpython-stubs-8.2.0rc1/espidf/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/espnow/
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-06-27 17:30:56.000000 circuitpython-stubs-8.2.0rc1/espnow/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/espulp/
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-27 17:30:56.000000 circuitpython-stubs-8.2.0rc1/espulp/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/floppyio/
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/floppyio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/fontio/
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/fontio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/framebufferio/
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/framebufferio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/frequencyio/
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/frequencyio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/getpass/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/getpass/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/gifio/
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/gifio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/gnss/
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/gnss/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/hashlib/
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/hashlib/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/i2ctarget/
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/i2ctarget/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/imagecapture/
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/imagecapture/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/ipaddress/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/ipaddress/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/is31fl3741/
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/is31fl3741/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/keypad/
--rw-r--r--   0 runner    (1001) docker     (123)    13080 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/keypad/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/math/
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/math/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/mdns/
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/mdns/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.754423 circuitpython-stubs-8.2.0rc1/memorymap/
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/memorymap/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/memorymonitor/
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/memorymonitor/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/microcontroller/
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/microcontroller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/msgpack/
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/msgpack/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/neopixel_write/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/neopixel_write/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/nvm/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/nvm/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/onewireio/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/onewireio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/os/
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/os/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/paralleldisplay/
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/paralleldisplay/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/picodvi/
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-27 17:30:56.000000 circuitpython-stubs-8.2.0rc1/picodvi/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/ps2io/
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/ps2io/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/pulseio/
--rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/pulseio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/pwmio/
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/pwmio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/qrio/
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/qrio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/rainbowio/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/rainbowio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/random/
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/random/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/rgbmatrix/
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/rgbmatrix/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/rotaryio/
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/rotaryio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/rp2pio/
--rw-r--r--   0 runner    (1001) docker     (123)    16742 2023-06-27 17:30:56.000000 circuitpython-stubs-8.2.0rc1/rp2pio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/rtc/
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/rtc/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/samd/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/samd/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/sdcardio/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/sdcardio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/sdioio/
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/sdioio/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 17:31:04.766423 circuitpython-stubs-8.2.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-27 17:30:56.000000 circuitpython-stubs-8.2.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/sharpdisplay/
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/sharpdisplay/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/socketpool/
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/socketpool/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/ssl/
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/ssl/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-06-27 17:30:54.000000 circuitpython-stubs-8.2.0rc1/storage/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/struct/
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/struct/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/supervisor/
--rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/supervisor/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/synthio/
--rw-r--r--   0 runner    (1001) docker     (123)    22728 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/synthio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/terminalio/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/terminalio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/time/
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/time/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/touchio/
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/touchio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/traceback/
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/traceback/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/uheap/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/uheap/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/ulab/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/ulab/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/ulab/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)    15556 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/ulab/numpy/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/ulab/numpy/carray/
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/ulab/numpy/carray/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.758423 circuitpython-stubs-8.2.0rc1/ulab/numpy/fft/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/ulab/numpy/fft/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/ulab/numpy/linalg/
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/ulab/numpy/linalg/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/ulab/scipy/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/ulab/scipy/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/ulab/scipy/linalg/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/ulab/scipy/linalg/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/ulab/scipy/optimize/
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/ulab/scipy/optimize/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/ulab/user/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/ulab/user/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/ulab/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/ulab/utils/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/usb/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/usb/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/usb/core/
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/usb/core/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/usb_cdc/
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/usb_cdc/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/usb_hid/
--rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/usb_hid/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/usb_host/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/usb_host/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/usb_midi/
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/usb_midi/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/ustack/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/ustack/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/vectorio/
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/vectorio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/watchdog/
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/watchdog/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/wifi/
--rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/wifi/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:04.762423 circuitpython-stubs-8.2.0rc1/zlib/
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-27 17:30:55.000000 circuitpython-stubs-8.2.0rc1/zlib/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.534528 circuitpython-stubs-8.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-25 16:37:21.000000 circuitpython-stubs-8.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-25 16:37:31.530528 circuitpython-stubs-8.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-25 16:37:21.000000 circuitpython-stubs-8.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/_bleio/
+-rw-r--r--   0 runner    (1001) docker     (123)    31094 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/_bleio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/_eve/
+-rw-r--r--   0 runner    (1001) docker     (123)    20379 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/_eve/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/_pew/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/_pew/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/_pixelmap/
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/_pixelmap/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/_stage/
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/_stage/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/adafruit_bus_device/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/adafruit_bus_device/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/adafruit_bus_device/i2c_device/
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/adafruit_bus_device/i2c_device/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/adafruit_bus_device/spi_device/
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/adafruit_bus_device/spi_device/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/adafruit_pixelbuf/
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/adafruit_pixelbuf/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/aesio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/aesio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/alarm/
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/alarm/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/alarm/pin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/alarm/pin/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/alarm/time/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/alarm/time/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/alarm/touch/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/alarm/touch/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/analogbufio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/analogbufio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/analogio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/analogio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/atexit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/atexit/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/audiobusio/
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/audiobusio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/audiocore/
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/audiocore/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.510528 circuitpython-stubs-8.2.1/audioio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/audioio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/audiomixer/
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/audiomixer/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/audiomp3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/audiomp3/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/audiopwmio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/audiopwmio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/bitbangio/
+-rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/bitbangio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/bitmaptools/
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/bitmaptools/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/bitops/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/bitops/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/board/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/board/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/busio/
+-rw-r--r--   0 runner    (1001) docker     (123)    20590 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/busio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/camera/
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/camera/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/canio/
+-rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/canio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.530528 circuitpython-stubs-8.2.1/circuitpython_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-25 16:37:30.000000 circuitpython-stubs-8.2.1/circuitpython_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-07-25 16:37:31.000000 circuitpython-stubs-8.2.1/circuitpython_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 16:37:30.000000 circuitpython-stubs-8.2.1/circuitpython_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 16:37:30.000000 circuitpython-stubs-8.2.1/circuitpython_stubs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-25 16:37:30.000000 circuitpython-stubs-8.2.1/circuitpython_stubs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/countio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/countio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/cyw43/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-25 16:37:21.000000 circuitpython-stubs-8.2.1/cyw43/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/digitalio/
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-07-25 16:37:18.000000 circuitpython-stubs-8.2.1/digitalio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/displayio/
+-rw-r--r--   0 runner    (1001) docker     (123)    40379 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/displayio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/dualbank/
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/dualbank/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/espcamera/
+-rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-07-25 16:37:21.000000 circuitpython-stubs-8.2.1/espcamera/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/espidf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-25 16:37:21.000000 circuitpython-stubs-8.2.1/espidf/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/espnow/
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-07-25 16:37:21.000000 circuitpython-stubs-8.2.1/espnow/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/espulp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-25 16:37:21.000000 circuitpython-stubs-8.2.1/espulp/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/floppyio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/floppyio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.514528 circuitpython-stubs-8.2.1/fontio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/fontio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/framebufferio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/framebufferio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/frequencyio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/frequencyio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/getpass/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/getpass/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/gifio/
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/gifio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/gnss/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/gnss/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/hashlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/hashlib/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/i2ctarget/
+-rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/i2ctarget/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/imagecapture/
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/imagecapture/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/ipaddress/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/ipaddress/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/is31fl3741/
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/is31fl3741/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/keypad/
+-rw-r--r--   0 runner    (1001) docker     (123)    13945 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/keypad/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/math/
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/math/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/mdns/
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/mdns/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/memorymap/
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/memorymap/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/memorymonitor/
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/memorymonitor/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/microcontroller/
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/microcontroller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/msgpack/
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/msgpack/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/neopixel_write/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/neopixel_write/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/nvm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/nvm/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/onewireio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/onewireio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/os/
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/os/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/paralleldisplay/
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/paralleldisplay/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.518528 circuitpython-stubs-8.2.1/picodvi/
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-07-25 16:37:21.000000 circuitpython-stubs-8.2.1/picodvi/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/ps2io/
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/ps2io/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/pulseio/
+-rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/pulseio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/pwmio/
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/pwmio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/qrio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/qrio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/rainbowio/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/rainbowio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/random/
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/random/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/rgbmatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/rgbmatrix/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/rotaryio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/rotaryio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/rp2pio/
+-rw-r--r--   0 runner    (1001) docker     (123)    16742 2023-07-25 16:37:21.000000 circuitpython-stubs-8.2.1/rp2pio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/rtc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/rtc/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/samd/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/samd/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/sdcardio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/sdcardio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/sdioio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/sdioio/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 16:37:31.534528 circuitpython-stubs-8.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-25 16:37:21.000000 circuitpython-stubs-8.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/sharpdisplay/
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/sharpdisplay/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/socketpool/
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/socketpool/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/ssl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/ssl/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/storage/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/struct/
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/struct/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/supervisor/
+-rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/supervisor/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/synthio/
+-rw-r--r--   0 runner    (1001) docker     (123)    22728 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/synthio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.522528 circuitpython-stubs-8.2.1/terminalio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/terminalio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/time/
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/time/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/touchio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-25 16:37:19.000000 circuitpython-stubs-8.2.1/touchio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/traceback/
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/traceback/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/uheap/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/uheap/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/ulab/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/ulab/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/ulab/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)    15556 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/ulab/numpy/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/ulab/numpy/carray/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/ulab/numpy/carray/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/ulab/numpy/fft/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/ulab/numpy/fft/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/ulab/numpy/linalg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/ulab/numpy/linalg/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/ulab/scipy/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/ulab/scipy/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/ulab/scipy/linalg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/ulab/scipy/linalg/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/ulab/scipy/optimize/
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/ulab/scipy/optimize/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/ulab/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/ulab/user/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/ulab/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/ulab/utils/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/usb/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/usb/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/usb/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/usb/core/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/usb_cdc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/usb_cdc/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/usb_hid/
+-rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/usb_hid/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/usb_host/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/usb_host/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/usb_midi/
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/usb_midi/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/ustack/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/ustack/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.526528 circuitpython-stubs-8.2.1/vectorio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/vectorio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.530528 circuitpython-stubs-8.2.1/watchdog/
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/watchdog/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.530528 circuitpython-stubs-8.2.1/wifi/
+-rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/wifi/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:37:31.530528 circuitpython-stubs-8.2.1/zlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-25 16:37:20.000000 circuitpython-stubs-8.2.1/zlib/__init__.pyi
```

### Comparing `circuitpython-stubs-8.2.0rc1/README.rst` & `circuitpython-stubs-8.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/_bleio/__init__.pyi` & `circuitpython-stubs-8.2.1/_bleio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/_eve/__init__.pyi` & `circuitpython-stubs-8.2.1/_eve/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/_pew/__init__.pyi` & `circuitpython-stubs-8.2.1/_pew/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/_pixelmap/__init__.pyi` & `circuitpython-stubs-8.2.1/_pixelmap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/_stage/__init__.pyi` & `circuitpython-stubs-8.2.1/_stage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/adafruit_bus_device/i2c_device/__init__.pyi` & `circuitpython-stubs-8.2.1/adafruit_bus_device/i2c_device/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/adafruit_bus_device/spi_device/__init__.pyi` & `circuitpython-stubs-8.2.1/adafruit_bus_device/spi_device/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/adafruit_pixelbuf/__init__.pyi` & `circuitpython-stubs-8.2.1/adafruit_pixelbuf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/aesio/__init__.pyi` & `circuitpython-stubs-8.2.1/aesio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/alarm/__init__.pyi` & `circuitpython-stubs-8.2.1/alarm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/alarm/pin/__init__.pyi` & `circuitpython-stubs-8.2.1/alarm/pin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/alarm/time/__init__.pyi` & `circuitpython-stubs-8.2.1/alarm/time/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/alarm/touch/__init__.pyi` & `circuitpython-stubs-8.2.1/alarm/touch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/analogbufio/__init__.pyi` & `circuitpython-stubs-8.2.1/analogbufio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/analogio/__init__.pyi` & `circuitpython-stubs-8.2.1/analogio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/atexit/__init__.pyi` & `circuitpython-stubs-8.2.1/atexit/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/audiobusio/__init__.pyi` & `circuitpython-stubs-8.2.1/audiobusio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/audiocore/__init__.pyi` & `circuitpython-stubs-8.2.1/audiocore/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/audioio/__init__.pyi` & `circuitpython-stubs-8.2.1/audioio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/audiomixer/__init__.pyi` & `circuitpython-stubs-8.2.1/audiomixer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/audiomp3/__init__.pyi` & `circuitpython-stubs-8.2.1/audiomp3/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/audiopwmio/__init__.pyi` & `circuitpython-stubs-8.2.1/audiopwmio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/bitbangio/__init__.pyi` & `circuitpython-stubs-8.2.1/bitbangio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/bitmaptools/__init__.pyi` & `circuitpython-stubs-8.2.1/bitmaptools/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/bitops/__init__.pyi` & `circuitpython-stubs-8.2.1/bitops/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/board/__init__.pyi` & `circuitpython-stubs-8.2.1/board/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/busio/__init__.pyi` & `circuitpython-stubs-8.2.1/busio/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 for working with custom drivers.
 
 Tutorial for I2C and SPI:
 https://learn.adafruit.com/circuitpython-basics-i2c-and-spi
 
 Tutorial for UART:
 https://learn.adafruit.com/circuitpython-essentials/circuitpython-uart-serial
+
+.. jinja
 """
 
 from __future__ import annotations
 
 from typing import List, Optional
 
 import microcontroller
@@ -189,15 +191,30 @@
     SPI is a serial protocol that has exclusive pins for data in and out of the
     main device.  It is typically faster than :py:class:`~bitbangio.I2C` because a
     separate pin is used to select a device rather than a transmitted
     address. This class only manages three of the four SPI lines: `!clock`,
     `!MOSI`, `!MISO`. Its up to the client to manage the appropriate
     select line, often abbreviated `!CS` or `!SS`. (This is common because
     multiple secondaries can share the `!clock`, `!MOSI` and `!MISO` lines
-    and therefore the hardware.)"""
+    and therefore the hardware.)
+
+    .. raw:: html
+
+        <p>
+        <details>
+        <summary>Available on these boards</summary>
+        <ul>
+        {% for board in support_matrix_reverse["busio.SPI"] %}
+        <li> {{ board }}
+        {% endfor %}
+        </ul>
+        </details>
+        </p>
+
+    """
 
     def __init__(
         self,
         clock: microcontroller.Pin,
         MOSI: Optional[microcontroller.Pin] = None,
         MISO: Optional[microcontroller.Pin] = None,
         half_duplex: bool = False,
@@ -352,15 +369,30 @@
         """
         ...
     frequency: int
     """The actual SPI bus frequency. This may not match the frequency requested
     due to internal limitations."""
 
 class UART:
-    """A bidirectional serial protocol"""
+    """A bidirectional serial protocol
+
+    .. raw:: html
+
+        <p>
+        <details>
+        <summary>Available on these boards</summary>
+        <ul>
+        {% for board in support_matrix_reverse["busio.UART"] %}
+        <li> {{ board }}
+        {% endfor %}
+        </ul>
+        </details>
+        </p>
+
+    """
 
     def __init__(
         self,
         tx: Optional[microcontroller.Pin] = None,
         rx: Optional[microcontroller.Pin] = None,
         *,
         rts: Optional[microcontroller.Pin] = None,
```

### Comparing `circuitpython-stubs-8.2.0rc1/camera/__init__.pyi` & `circuitpython-stubs-8.2.1/camera/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/canio/__init__.pyi` & `circuitpython-stubs-8.2.1/canio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/circuitpython_stubs.egg-info/SOURCES.txt` & `circuitpython-stubs-8.2.1/circuitpython_stubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/circuitpython_stubs.egg-info/top_level.txt` & `circuitpython-stubs-8.2.1/circuitpython_stubs.egg-info/top_level.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/countio/__init__.pyi` & `circuitpython-stubs-8.2.1/countio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/cyw43/__init__.pyi` & `circuitpython-stubs-8.2.1/cyw43/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/digitalio/__init__.pyi` & `circuitpython-stubs-8.2.1/digitalio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/displayio/__init__.pyi` & `circuitpython-stubs-8.2.1/displayio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/dualbank/__init__.pyi` & `circuitpython-stubs-8.2.1/dualbank/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/espcamera/__init__.pyi` & `circuitpython-stubs-8.2.1/espcamera/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/espidf/__init__.pyi` & `circuitpython-stubs-8.2.1/espidf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/espnow/__init__.pyi` & `circuitpython-stubs-8.2.1/espnow/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/espulp/__init__.pyi` & `circuitpython-stubs-8.2.1/espulp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/floppyio/__init__.pyi` & `circuitpython-stubs-8.2.1/floppyio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/fontio/__init__.pyi` & `circuitpython-stubs-8.2.1/fontio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/framebufferio/__init__.pyi` & `circuitpython-stubs-8.2.1/framebufferio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/frequencyio/__init__.pyi` & `circuitpython-stubs-8.2.1/frequencyio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/getpass/__init__.pyi` & `circuitpython-stubs-8.2.1/getpass/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/gifio/__init__.pyi` & `circuitpython-stubs-8.2.1/gifio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/gnss/__init__.pyi` & `circuitpython-stubs-8.2.1/gnss/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/hashlib/__init__.pyi` & `circuitpython-stubs-8.2.1/hashlib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/i2ctarget/__init__.pyi` & `circuitpython-stubs-8.2.1/i2ctarget/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/imagecapture/__init__.pyi` & `circuitpython-stubs-8.2.1/imagecapture/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/ipaddress/__init__.pyi` & `circuitpython-stubs-8.2.1/ipaddress/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/is31fl3741/__init__.pyi` & `circuitpython-stubs-8.2.1/is31fl3741/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/keypad/__init__.pyi` & `circuitpython-stubs-8.2.1/keypad/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 The `keypad` module provides native support to scan sets of keys or buttons,
 connected independently to individual pins,
 connected to a shift register,
 or connected in a row-and-column matrix.
 
 For more information about working with the `keypad` module in CircuitPython,
 see `this Learn guide <https://learn.adafruit.com/key-pad-matrix-scanning-in-circuitpython>`_.
+
+.. jinja
 """
 
 from __future__ import annotations
 
 from typing import Optional, Sequence, Tuple
 
 import microcontroller
@@ -101,15 +103,30 @@
         ...
     overflowed: bool
     """``True`` if an event could not be added to the event queue because it was full. (read-only)
     Set to ``False`` by  `clear()`.
     """
 
 class KeyMatrix:
-    """Manage a 2D matrix of keys with row and column pins."""
+    """Manage a 2D matrix of keys with row and column pins.
+
+    .. raw:: html
+
+        <p>
+        <details>
+        <summary>Available on these boards</summary>
+        <ul>
+        {% for board in support_matrix_reverse["keypad.KeyMatrix"] %}
+        <li> {{ board }}
+        {% endfor %}
+        </ul>
+        </details>
+        </p>
+
+    """
 
     def __init__(
         self,
         row_pins: Sequence[microcontroller.Pin],
         column_pins: Sequence[microcontroller.Pin],
         columns_to_anodes: bool = True,
         interval: float = 0.020,
@@ -173,15 +190,30 @@
         """
         ...
     events: EventQueue
     """The `EventQueue` associated with this `Keys` object. (read-only)
     """
 
 class Keys:
-    """Manage a set of independent keys."""
+    """Manage a set of independent keys.
+
+    .. raw:: html
+
+        <p>
+        <details>
+        <summary>Available on these boards</summary>
+        <ul>
+        {% for board in support_matrix_reverse["keypad.Keys"] %}
+        <li> {{ board }}
+        {% endfor %}
+        </ul>
+        </details>
+        </p>
+
+    """
 
     def __init__(
         self,
         pins: Sequence[microcontroller.Pin],
         *,
         value_when_pressed: bool,
         pull: bool = True,
@@ -233,15 +265,30 @@
     """The number of keys that are being scanned. (read-only)
     """
     events: EventQueue
     """The `EventQueue` associated with this `Keys` object. (read-only)
     """
 
 class ShiftRegisterKeys:
-    """Manage a set of keys attached to an incoming shift register."""
+    """Manage a set of keys attached to an incoming shift register.
+
+    .. raw:: html
+
+        <p>
+        <details>
+        <summary>Available on these boards</summary>
+        <ul>
+        {% for board in support_matrix_reverse["keypad.ShiftRegisterKeys"] %}
+        <li> {{ board }}
+        {% endfor %}
+        </ul>
+        </details>
+        </p>
+
+    """
 
     def __init__(
         self,
         *,
         clock: microcontroller.Pin,
         data: microcontroller.Pin,
         latch: microcontroller.Pin,
```

### Comparing `circuitpython-stubs-8.2.0rc1/math/__init__.pyi` & `circuitpython-stubs-8.2.1/math/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/mdns/__init__.pyi` & `circuitpython-stubs-8.2.1/mdns/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -69,11 +69,13 @@
         ...
     def advertise_service(self, *, service_type: str, protocol: str, port: int) -> None:
         """Respond to queries for the given service with the given port.
 
         ``service_type`` and ``protocol`` can only occur on one port. Any call after the first
         will update the entry's port.
 
+        If web workflow is active, the port it uses can't also be used to advertise a service.
+
         :param str service_type: The service type such as "_http"
         :param str protocol: The service protocol such as "_tcp"
         :param int port: The port used by the service"""
         ...
```

### Comparing `circuitpython-stubs-8.2.0rc1/memorymap/__init__.pyi` & `circuitpython-stubs-8.2.1/memorymap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/memorymonitor/__init__.pyi` & `circuitpython-stubs-8.2.1/memorymonitor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/microcontroller/__init__.pyi` & `circuitpython-stubs-8.2.1/microcontroller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/msgpack/__init__.pyi` & `circuitpython-stubs-8.2.1/msgpack/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/neopixel_write/__init__.pyi` & `circuitpython-stubs-8.2.1/neopixel_write/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/nvm/__init__.pyi` & `circuitpython-stubs-8.2.1/nvm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/onewireio/__init__.pyi` & `circuitpython-stubs-8.2.1/onewireio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/os/__init__.pyi` & `circuitpython-stubs-8.2.1/os/__init__.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """functions that an OS normally provides
 
 |see_cpython_module| :mod:`cpython:os`.
+
+.. jinja
 """
 
 from __future__ import annotations
 
 import typing
 from typing import Optional, Tuple
 
@@ -29,15 +31,32 @@
 def getcwd() -> str:
     """Get the current directory."""
     ...
 
 def getenv(key: str, default: Optional[str] = None) -> Optional[str]:
     """Get the environment variable value for the given key or return ``default``.
 
-    This may load values from disk so cache the result instead of calling this often."""
+    This may load values from disk so cache the result instead of calling this often.
+
+    On boards that do not support ``settings.toml`` reading in the core, this function will raise NotImplementedError.
+
+    .. raw:: html
+
+        <p>
+        <details>
+        <summary>Available on these boards</summary>
+        <ul>
+        {% for board in support_matrix_reverse["os.getenv"] %}
+        <li> {{ board }}
+        {% endfor %}
+        </ul>
+        </details>
+        </p>
+
+    """
     ...
 
 def listdir(dir: str) -> str:
     """With no argument, list the current directory.  Otherwise list the given directory."""
     ...
 
 def mkdir(path: str) -> None:
```

### Comparing `circuitpython-stubs-8.2.0rc1/paralleldisplay/__init__.pyi` & `circuitpython-stubs-8.2.1/paralleldisplay/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/picodvi/__init__.pyi` & `circuitpython-stubs-8.2.1/picodvi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/ps2io/__init__.pyi` & `circuitpython-stubs-8.2.1/ps2io/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/pulseio/__init__.pyi` & `circuitpython-stubs-8.2.1/pulseio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/pwmio/__init__.pyi` & `circuitpython-stubs-8.2.1/pwmio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/qrio/__init__.pyi` & `circuitpython-stubs-8.2.1/qrio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/random/__init__.pyi` & `circuitpython-stubs-8.2.1/random/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/rgbmatrix/__init__.pyi` & `circuitpython-stubs-8.2.1/rgbmatrix/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/rotaryio/__init__.pyi` & `circuitpython-stubs-8.2.1/rotaryio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/rp2pio/__init__.pyi` & `circuitpython-stubs-8.2.1/rp2pio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/rtc/__init__.pyi` & `circuitpython-stubs-8.2.1/rtc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/samd/__init__.pyi` & `circuitpython-stubs-8.2.1/samd/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/sdcardio/__init__.pyi` & `circuitpython-stubs-8.2.1/sdcardio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/sdioio/__init__.pyi` & `circuitpython-stubs-8.2.1/sdioio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/setup.py` & `circuitpython-stubs-8.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/sharpdisplay/__init__.pyi` & `circuitpython-stubs-8.2.1/sharpdisplay/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/socketpool/__init__.pyi` & `circuitpython-stubs-8.2.1/socketpool/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/ssl/__init__.pyi` & `circuitpython-stubs-8.2.1/ssl/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/storage/__init__.pyi` & `circuitpython-stubs-8.2.1/storage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/struct/__init__.pyi` & `circuitpython-stubs-8.2.1/struct/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/supervisor/__init__.pyi` & `circuitpython-stubs-8.2.1/supervisor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/synthio/__init__.pyi` & `circuitpython-stubs-8.2.1/synthio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/terminalio/__init__.pyi` & `circuitpython-stubs-8.2.1/terminalio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/time/__init__.pyi` & `circuitpython-stubs-8.2.1/time/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/touchio/__init__.pyi` & `circuitpython-stubs-8.2.1/touchio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/traceback/__init__.pyi` & `circuitpython-stubs-8.2.1/traceback/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/ulab/__init__.pyi` & `circuitpython-stubs-8.2.1/ulab/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/ulab/numpy/__init__.pyi` & `circuitpython-stubs-8.2.1/ulab/numpy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/ulab/numpy/carray/__init__.pyi` & `circuitpython-stubs-8.2.1/ulab/numpy/carray/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/ulab/numpy/fft/__init__.pyi` & `circuitpython-stubs-8.2.1/ulab/numpy/fft/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/ulab/numpy/linalg/__init__.pyi` & `circuitpython-stubs-8.2.1/ulab/numpy/linalg/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/ulab/scipy/linalg/__init__.pyi` & `circuitpython-stubs-8.2.1/ulab/scipy/linalg/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/ulab/scipy/optimize/__init__.pyi` & `circuitpython-stubs-8.2.1/ulab/scipy/optimize/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/usb/core/__init__.pyi` & `circuitpython-stubs-8.2.1/usb/core/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/usb_cdc/__init__.pyi` & `circuitpython-stubs-8.2.1/usb_cdc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/usb_hid/__init__.pyi` & `circuitpython-stubs-8.2.1/usb_hid/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/usb_host/__init__.pyi` & `circuitpython-stubs-8.2.1/usb_host/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/usb_midi/__init__.pyi` & `circuitpython-stubs-8.2.1/usb_midi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/vectorio/__init__.pyi` & `circuitpython-stubs-8.2.1/vectorio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/watchdog/__init__.pyi` & `circuitpython-stubs-8.2.1/watchdog/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0rc1/wifi/__init__.pyi` & `circuitpython-stubs-8.2.1/wifi/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -227,29 +227,34 @@
         *,
         ipv4: ipaddress.IPv4Address,
         netmask: ipaddress.IPv4Address,
         gateway: ipaddress.IPv4Address,
         ipv4_dns: Optional[ipaddress.IPv4Address],
     ) -> None:
         """Sets the IP v4 address of the station. Must include the netmask and gateway. DNS address is optional.
-        Setting the address manually will stop the DHCP client."""
+        Setting the address manually will stop the DHCP client.
+
+        .. note::
+
+            In the raspberrypi port (RP2040 CYW43), the access point needs to be started before the IP v4 address can be set.
+        """
         ...
     def set_ipv4_address_ap(
         self,
         *,
         ipv4: ipaddress.IPv4Address,
         netmask: ipaddress.IPv4Address,
         gateway: ipaddress.IPv4Address,
     ) -> None:
         """Sets the IP v4 address of the access point. Must include the netmask and gateway."""
         ...
     ipv4_address: Optional[ipaddress.IPv4Address]
     """IP v4 Address of the station when connected to an access point. None otherwise. (read-only)"""
     ipv4_address_ap: Optional[ipaddress.IPv4Address]
-    """IP v4 Address of the access point, when enabled. None otherwise."""
+    """IP v4 Address of the access point, when enabled. None otherwise. (read-only)"""
     ipv4_dns: ipaddress.IPv4Address
     """IP v4 Address of the DNS server to be used."""
     ap_info: Optional[Network]
     """Network object containing BSSID, SSID, authmode, channel, country and RSSI when connected to an access point. None otherwise."""
     def start_dhcp(self) -> None:
         """Starts the station DHCP client."""
         ...
```

### Comparing `circuitpython-stubs-8.2.0rc1/zlib/__init__.pyi` & `circuitpython-stubs-8.2.1/zlib/__init__.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 This module allows to decompress binary data compressed with DEFLATE algorithm
 (commonly used in zlib library and gzip archiver). Compression is not yet implemented."""
 
 from __future__ import annotations
 
 from typing import Optional
 
-def zlib_decompress(
+def decompress(
     data: bytes, wbits: Optional[int] = 0, bufsize: Optional[int] = 0
 ) -> bytes:
     """Return decompressed *data* as bytes. *wbits* is DEFLATE dictionary window
     size used during compression (8-15, the dictionary size is power of 2 of
     that value). Additionally, if value is positive, *data* is assumed to be
     zlib stream (with zlib header). Otherwise, if it's negative, it's assumed
     to be raw DEFLATE stream.
```

