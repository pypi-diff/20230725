# Comparing `tmp/maxsmart-0.1.7.tar.gz` & `tmp/maxsmart-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxsmart-0.1.7.tar", last modified: Thu Jun 29 09:47:07 2023, max compression
+gzip compressed data, was "maxsmart-0.1.8.tar", last modified: Tue Jul 25 06:32:33 2023, max compression
```

## Comparing `maxsmart-0.1.7.tar` & `maxsmart-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-06-29 09:47:07.468305 maxsmart-0.1.7/
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)     1070 2023-05-20 20:48:25.000000 maxsmart-0.1.7/LICENSE
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)      846 2023-06-29 09:47:07.468305 maxsmart-0.1.7/PKG-INFO
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)     7581 2023-06-22 20:20:51.000000 maxsmart-0.1.7/README.md
-drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-06-29 09:47:07.464972 maxsmart-0.1.7/maxsmart/
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)       78 2023-06-22 19:33:26.000000 maxsmart-0.1.7/maxsmart/__init__.py
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)     5149 2023-06-29 09:36:05.000000 maxsmart-0.1.7/maxsmart/maxsmart.py
-drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-06-29 09:47:07.468305 maxsmart-0.1.7/maxsmart.egg-info/
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)      846 2023-06-29 09:47:07.000000 maxsmart-0.1.7/maxsmart.egg-info/PKG-INFO
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)      268 2023-06-29 09:47:07.000000 maxsmart-0.1.7/maxsmart.egg-info/SOURCES.txt
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)        1 2023-06-29 09:47:07.000000 maxsmart-0.1.7/maxsmart.egg-info/dependency_links.txt
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)        9 2023-06-29 09:47:07.000000 maxsmart-0.1.7/maxsmart.egg-info/requires.txt
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)       15 2023-06-29 09:47:07.000000 maxsmart-0.1.7/maxsmart.egg-info/top_level.txt
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)       38 2023-06-29 09:47:07.468305 maxsmart-0.1.7/setup.cfg
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)     1014 2023-06-29 09:21:45.000000 maxsmart-0.1.7/setup.py
-drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-06-29 09:47:07.468305 maxsmart-0.1.7/tests/
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)        0 2023-05-20 20:48:25.000000 maxsmart-0.1.7/tests/__init__.py
--rw-r--r--   0 superkikim  (1000) superkikim  (1001)     3533 2023-06-22 18:58:26.000000 maxsmart-0.1.7/tests/test_maxsmart.py
+drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-07-25 06:32:33.608309 maxsmart-0.1.8/
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)     1070 2023-05-20 20:48:25.000000 maxsmart-0.1.8/LICENSE
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)      846 2023-07-25 06:32:33.608309 maxsmart-0.1.8/PKG-INFO
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)     7581 2023-06-22 20:20:51.000000 maxsmart-0.1.8/README.md
+drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-07-25 06:32:33.608309 maxsmart-0.1.8/maxsmart/
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)       78 2023-06-22 19:33:26.000000 maxsmart-0.1.8/maxsmart/__init__.py
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)     5134 2023-07-25 06:30:30.000000 maxsmart-0.1.8/maxsmart/maxsmart.py
+drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-07-25 06:32:33.608309 maxsmart-0.1.8/maxsmart.egg-info/
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)      846 2023-07-25 06:32:33.000000 maxsmart-0.1.8/maxsmart.egg-info/PKG-INFO
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)      268 2023-07-25 06:32:33.000000 maxsmart-0.1.8/maxsmart.egg-info/SOURCES.txt
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)        1 2023-07-25 06:32:33.000000 maxsmart-0.1.8/maxsmart.egg-info/dependency_links.txt
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)        9 2023-07-25 06:32:33.000000 maxsmart-0.1.8/maxsmart.egg-info/requires.txt
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)       15 2023-07-25 06:32:33.000000 maxsmart-0.1.8/maxsmart.egg-info/top_level.txt
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)       38 2023-07-25 06:32:33.608309 maxsmart-0.1.8/setup.cfg
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)     1014 2023-07-25 06:19:57.000000 maxsmart-0.1.8/setup.py
+drwxr-xr-x   0 superkikim  (1000) superkikim  (1001)        0 2023-07-25 06:32:33.608309 maxsmart-0.1.8/tests/
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)        0 2023-05-20 20:48:25.000000 maxsmart-0.1.8/tests/__init__.py
+-rw-r--r--   0 superkikim  (1000) superkikim  (1001)     3533 2023-06-22 18:58:26.000000 maxsmart-0.1.8/tests/test_maxsmart.py
```

### Comparing `maxsmart-0.1.7/LICENSE` & `maxsmart-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `maxsmart-0.1.7/PKG-INFO` & `maxsmart-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxsmart
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python module for operating network connected power strips
 Home-page: https://github.com/superkikim/maxsmart
 Author: Akim Sissaoui
 Author-email: superkikim@sissaoui.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `maxsmart-0.1.7/README.md` & `maxsmart-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `maxsmart-0.1.7/maxsmart/maxsmart.py` & `maxsmart-0.1.8/maxsmart/maxsmart.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         return maxsmart_devices
 
     @staticmethod
     def _validate_firmware_versions(devices):
         for device in devices:
             firmware_version = device.get('ver')
             if firmware_version != '1.30':
-                raise IncompatibleFirmwareError(f"Device with IP {device['ip']} has firmware version {firmware_version}. This module has been tested with MaxSmart devices with firmware version 1.30.")
+                raise ValueError(f"Device with IP {device['ip']} has firmware version {firmware_version}. This module has been tested with MaxSmart devices with firmware version 1.30.")
 
 class MaxSmartDevice:
     def __init__(self, ip):
         self.ip = ip
 
     def _send_command(self, cmd, params=None):
         url = f"http://{self.ip}/?cmd={cmd}"
```

### Comparing `maxsmart-0.1.7/maxsmart.egg-info/PKG-INFO` & `maxsmart-0.1.8/maxsmart.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxsmart
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python module for operating network connected power strips
 Home-page: https://github.com/superkikim/maxsmart
 Author: Akim Sissaoui
 Author-email: superkikim@sissaoui.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `maxsmart-0.1.7/setup.py` & `maxsmart-0.1.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='maxsmart',
-    version='0.1.7',
+    version='0.1.8',
     author='Akim Sissaoui',
     author_email='superkikim@sissaoui.com',
     description='A Python module for operating network connected power strips',
     long_description='''A Python module for operating network connected power strips.
                         It provides functionality to turn on/off sockets, check their state, and retrieve power consumption data.''',
     url='https://github.com/superkikim/maxsmart',
     packages=find_packages(),
```

### Comparing `maxsmart-0.1.7/tests/test_maxsmart.py` & `maxsmart-0.1.8/tests/test_maxsmart.py`

 * *Files identical despite different names*

