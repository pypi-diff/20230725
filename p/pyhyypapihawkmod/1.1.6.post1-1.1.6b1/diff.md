# Comparing `tmp/pyhyypapihawkmod-1.1.6.post1.tar.gz` & `tmp/pyhyypapihawkmod-1.1.6b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-1.1.6.post1.tar", last modified: Tue Jul 25 16:42:20 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-1.1.6b1.tar", last modified: Tue Jul 25 16:46:42 2023, max compression
```

## Comparing `pyhyypapihawkmod-1.1.6.post1.tar` & `pyhyypapihawkmod-1.1.6b1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 16:42:20.846032 pyhyypapihawkmod-1.1.6.post1/
--rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6.post1/LICENSE.md
--rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6.post1/MANIFEST.in
--rw-rw-rw-   0        0        0      523 2023-07-25 16:42:20.845024 pyhyypapihawkmod-1.1.6.post1/PKG-INFO
--rw-rw-rw-   0        0        0     1940 2023-07-25 16:40:14.000000 pyhyypapihawkmod-1.1.6.post1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 16:42:20.833899 pyhyypapihawkmod-1.1.6.post1/pyhyypapihawkmod/
--rw-rw-rw-   0        0        0      429 2023-06-19 07:52:00.000000 pyhyypapihawkmod-1.1.6.post1/pyhyypapihawkmod/__init__.py
--rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.1.6.post1/pyhyypapihawkmod/__main__.py
--rw-rw-rw-   0        0        0     8446 2023-07-25 16:39:11.000000 pyhyypapihawkmod-1.1.6.post1/pyhyypapihawkmod/alarm_info.py
--rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6.post1/pyhyypapihawkmod/android_checkin_pb2.py
--rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6.post1/pyhyypapihawkmod/checkin_pb2.py
--rw-rw-rw-   0        0        0    27868 2023-07-25 16:40:24.000000 pyhyypapihawkmod-1.1.6.post1/pyhyypapihawkmod/client.py
--rw-rw-rw-   0        0        0     4005 2023-05-28 09:35:32.000000 pyhyypapihawkmod-1.1.6.post1/pyhyypapihawkmod/constants.py
--rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6.post1/pyhyypapihawkmod/exceptions.py
--rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6.post1/pyhyypapihawkmod/mcs_pb2.py
--rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.1.6.post1/pyhyypapihawkmod/push_receiver.py
-drwxrwxrwx   0        0        0        0 2023-07-25 16:42:20.843005 pyhyypapihawkmod-1.1.6.post1/pyhyypapihawkmod.egg-info/
--rw-rw-rw-   0        0        0      523 2023-07-25 16:42:20.000000 pyhyypapihawkmod-1.1.6.post1/pyhyypapihawkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2023-07-25 16:42:20.000000 pyhyypapihawkmod-1.1.6.post1/pyhyypapihawkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 16:42:20.000000 pyhyypapihawkmod-1.1.6.post1/pyhyypapihawkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-25 16:42:20.000000 pyhyypapihawkmod-1.1.6.post1/pyhyypapihawkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-25 16:42:20.000000 pyhyypapihawkmod-1.1.6.post1/pyhyypapihawkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 16:42:20.846032 pyhyypapihawkmod-1.1.6.post1/setup.cfg
--rw-rw-rw-   0        0        0      923 2023-07-25 15:37:31.000000 pyhyypapihawkmod-1.1.6.post1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 16:46:42.540065 pyhyypapihawkmod-1.1.6b1/
+-rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b1/LICENSE.md
+-rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b1/MANIFEST.in
+-rw-rw-rw-   0        0        0      519 2023-07-25 16:46:42.539557 pyhyypapihawkmod-1.1.6b1/PKG-INFO
+-rw-rw-rw-   0        0        0     1940 2023-07-25 16:40:14.000000 pyhyypapihawkmod-1.1.6b1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 16:46:42.527890 pyhyypapihawkmod-1.1.6b1/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      429 2023-06-19 07:52:00.000000 pyhyypapihawkmod-1.1.6b1/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.1.6b1/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0     8446 2023-07-25 16:39:11.000000 pyhyypapihawkmod-1.1.6b1/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b1/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b1/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    27868 2023-07-25 16:40:24.000000 pyhyypapihawkmod-1.1.6b1/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     4005 2023-05-28 09:35:32.000000 pyhyypapihawkmod-1.1.6b1/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b1/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b1/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.1.6b1/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-07-25 16:46:42.537535 pyhyypapihawkmod-1.1.6b1/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      519 2023-07-25 16:46:42.000000 pyhyypapihawkmod-1.1.6b1/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-07-25 16:46:42.000000 pyhyypapihawkmod-1.1.6b1/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 16:46:42.000000 pyhyypapihawkmod-1.1.6b1/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-25 16:46:42.000000 pyhyypapihawkmod-1.1.6b1/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-25 16:46:42.000000 pyhyypapihawkmod-1.1.6b1/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 16:46:42.540571 pyhyypapihawkmod-1.1.6b1/setup.cfg
+-rw-rw-rw-   0        0        0      923 2023-07-25 16:45:55.000000 pyhyypapihawkmod-1.1.6b1/setup.py
```

### Comparing `pyhyypapihawkmod-1.1.6.post1/LICENSE.md` & `pyhyypapihawkmod-1.1.6b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6.post1/PKG-INFO` & `pyhyypapihawkmod-1.1.6b1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.1.6.post1
+Version: 1.1.6b1
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.1.6.post1/README.md` & `pyhyypapihawkmod-1.1.6b1/README.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6.post1/pyhyypapihawkmod/alarm_info.py` & `pyhyypapihawkmod-1.1.6b1/pyhyypapihawkmod/alarm_info.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6.post1/pyhyypapihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-1.1.6b1/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6.post1/pyhyypapihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-1.1.6b1/pyhyypapihawkmod/checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6.post1/pyhyypapihawkmod/client.py` & `pyhyypapihawkmod-1.1.6b1/pyhyypapihawkmod/client.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6.post1/pyhyypapihawkmod/constants.py` & `pyhyypapihawkmod-1.1.6b1/pyhyypapihawkmod/constants.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6.post1/pyhyypapihawkmod/mcs_pb2.py` & `pyhyypapihawkmod-1.1.6b1/pyhyypapihawkmod/mcs_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6.post1/pyhyypapihawkmod/push_receiver.py` & `pyhyypapihawkmod-1.1.6b1/pyhyypapihawkmod/push_receiver.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6.post1/pyhyypapihawkmod.egg-info/PKG-INFO` & `pyhyypapihawkmod-1.1.6b1/pyhyypapihawkmod.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.1.6.post1
+Version: 1.1.6b1
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.1.6.post1/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-1.1.6b1/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6.post1/setup.py` & `pyhyypapihawkmod-1.1.6b1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhyypapihawkmod',
-    version="1.1.6-1",
+    version="1.1.6b1",
     license='Apache Software License 2.0',
     author='hawky358 (Original code by Renier Moorcroft)',
     author_email='hawky358@users.github.com',
     description='IDS Hyyp/ADT Secure Home API',
     long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others. Please view readme on github (Based on 0.0.0.8 by Renier Moorcroft with updated protobuf files) ",
     url='https://github.com/hawky358/pyHyypApi',
     packages=setuptools.find_packages(),
```

