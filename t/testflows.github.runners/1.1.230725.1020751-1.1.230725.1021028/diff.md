# Comparing `tmp/testflows.github.runners-1.1.230725.1020751.tar.gz` & `tmp/testflows.github.runners-1.1.230725.1021028.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.1.230725.1020751.tar", last modified: Tue Jul 25 02:07:52 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.1.230725.1021028.tar", last modified: Tue Jul 25 02:10:28 2023, max compression
```

## Comparing `testflows.github.runners-1.1.230725.1020751.tar` & `testflows.github.runners-1.1.230725.1021028.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 02:07:52.014989 testflows.github.runners-1.1.230725.1020751/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.1.230725.1020751/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    22139 2023-07-25 02:07:52.010989 testflows.github.runners-1.1.230725.1020751/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    21547 2023-07-25 01:47:16.000000 testflows.github.runners-1.1.230725.1020751/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-25 02:07:52.014989 testflows.github.runners-1.1.230725.1020751/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-25 02:07:51.000000 testflows.github.runners-1.1.230725.1020751/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 02:07:52.010989 testflows.github.runners-1.1.230725.1020751/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 02:07:52.010989 testflows.github.runners-1.1.230725.1020751/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 02:07:52.010989 testflows.github.runners-1.1.230725.1020751/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-25 02:07:51.000000 testflows.github.runners-1.1.230725.1020751/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.1.230725.1020751/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1121 2023-07-25 02:04:51.000000 testflows.github.runners-1.1.230725.1020751/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 02:07:52.010989 testflows.github.runners-1.1.230725.1020751/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    14693 2023-07-25 02:07:25.000000 testflows.github.runners-1.1.230725.1020751/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)     4106 2023-07-25 02:06:43.000000 testflows.github.runners-1.1.230725.1020751/testflows/github/runners/deploy.py
--rw-rw-r--   0 user      (1000) user      (1000)     1266 2023-07-24 15:25:53.000000 testflows.github.runners-1.1.230725.1020751/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     8571 2023-07-25 01:13:14.000000 testflows.github.runners-1.1.230725.1020751/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)     8184 2023-07-25 02:00:02.000000 testflows.github.runners-1.1.230725.1020751/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 02:07:52.010989 testflows.github.runners-1.1.230725.1020751/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.1.230725.1020751/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 02:07:52.010989 testflows.github.runners-1.1.230725.1020751/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.1.230725.1020751/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      390 2023-07-25 01:34:03.000000 testflows.github.runners-1.1.230725.1020751/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-24 22:14:55.000000 testflows.github.runners-1.1.230725.1020751/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-24 01:28:32.000000 testflows.github.runners-1.1.230725.1020751/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      714 2023-07-24 01:27:59.000000 testflows.github.runners-1.1.230725.1020751/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.1.230725.1020751/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     4426 2023-07-25 02:03:48.000000 testflows.github.runners-1.1.230725.1020751/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1392 2023-07-24 23:28:45.000000 testflows.github.runners-1.1.230725.1020751/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 02:07:52.010989 testflows.github.runners-1.1.230725.1020751/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    22139 2023-07-25 02:07:51.000000 testflows.github.runners-1.1.230725.1020751/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1001 2023-07-25 02:07:51.000000 testflows.github.runners-1.1.230725.1020751/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-25 02:07:51.000000 testflows.github.runners-1.1.230725.1020751/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.1.230725.1020751/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-25 02:07:51.000000 testflows.github.runners-1.1.230725.1020751/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-25 02:07:51.000000 testflows.github.runners-1.1.230725.1020751/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 02:10:28.930267 testflows.github.runners-1.1.230725.1021028/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.1.230725.1021028/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    22139 2023-07-25 02:10:28.930267 testflows.github.runners-1.1.230725.1021028/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    21547 2023-07-25 01:47:16.000000 testflows.github.runners-1.1.230725.1021028/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-25 02:10:28.930267 testflows.github.runners-1.1.230725.1021028/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-25 02:10:28.000000 testflows.github.runners-1.1.230725.1021028/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 02:10:28.926267 testflows.github.runners-1.1.230725.1021028/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 02:10:28.926267 testflows.github.runners-1.1.230725.1021028/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 02:10:28.926267 testflows.github.runners-1.1.230725.1021028/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-25 02:10:28.000000 testflows.github.runners-1.1.230725.1021028/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.1.230725.1021028/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1121 2023-07-25 02:04:51.000000 testflows.github.runners-1.1.230725.1021028/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 02:10:28.926267 testflows.github.runners-1.1.230725.1021028/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    14693 2023-07-25 02:07:25.000000 testflows.github.runners-1.1.230725.1021028/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)     4533 2023-07-25 02:10:10.000000 testflows.github.runners-1.1.230725.1021028/testflows/github/runners/deploy.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1266 2023-07-24 15:25:53.000000 testflows.github.runners-1.1.230725.1021028/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8571 2023-07-25 01:13:14.000000 testflows.github.runners-1.1.230725.1021028/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8184 2023-07-25 02:00:02.000000 testflows.github.runners-1.1.230725.1021028/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 02:10:28.926267 testflows.github.runners-1.1.230725.1021028/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.1.230725.1021028/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 02:10:28.926267 testflows.github.runners-1.1.230725.1021028/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.1.230725.1021028/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      390 2023-07-25 01:34:03.000000 testflows.github.runners-1.1.230725.1021028/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-24 22:14:55.000000 testflows.github.runners-1.1.230725.1021028/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-24 01:28:32.000000 testflows.github.runners-1.1.230725.1021028/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      714 2023-07-24 01:27:59.000000 testflows.github.runners-1.1.230725.1021028/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.1.230725.1021028/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4426 2023-07-25 02:03:48.000000 testflows.github.runners-1.1.230725.1021028/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1392 2023-07-24 23:28:45.000000 testflows.github.runners-1.1.230725.1021028/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 02:10:28.926267 testflows.github.runners-1.1.230725.1021028/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    22139 2023-07-25 02:10:28.000000 testflows.github.runners-1.1.230725.1021028/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1001 2023-07-25 02:10:28.000000 testflows.github.runners-1.1.230725.1021028/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-25 02:10:28.000000 testflows.github.runners-1.1.230725.1021028/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.1.230725.1021028/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-25 02:10:28.000000 testflows.github.runners-1.1.230725.1021028/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-25 02:10:28.000000 testflows.github.runners-1.1.230725.1021028/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.1.230725.1020751/LICENSE` & `testflows.github.runners-1.1.230725.1021028/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1020751/PKG-INFO` & `testflows.github.runners-1.1.230725.1021028/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.1.230725.1020751
+Version: 1.1.230725.1021028
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.1.230725.1020751/README.rst` & `testflows.github.runners-1.1.230725.1021028/README.rst`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1020751/setup.py` & `testflows.github.runners-1.1.230725.1021028/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.1.230725.1020751",
+    version="1.1.230725.1021028",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.1.230725.1020751/testflows/github/runners/__init__.py` & `testflows.github.runners-1.1.230725.1021028/testflows/github/runners/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.1.230725.1020751"
+__version__ = "1.1.230725.1021028"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.1.230725.1020751/testflows/github/runners/actions.py` & `testflows.github.runners-1.1.230725.1021028/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1020751/testflows/github/runners/args.py` & `testflows.github.runners-1.1.230725.1021028/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1020751/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.1.230725.1021028/testflows/github/runners/bin/github-runners`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1020751/testflows/github/runners/deploy.py` & `testflows.github.runners-1.1.230725.1021028/testflows/github/runners/deploy.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
+import hashlib
 
 from hcloud import Client
 from hcloud.ssh_keys.domain import SSHKey
 from hcloud.server_types.domain import ServerType
 from hcloud.servers.client import BoundServer
 from hcloud.images.domain import Image
 from hcloud.locations.domain import Location
@@ -42,21 +43,30 @@
 
     if args.force:
         with Action(f"Checking if server {name} already exists", ignore_fail=True):
             server: BoundServer = client.servers.get_by_name(name)
             with Action(f"Deleting server {name}"):
                 server.delete()
 
+    with Action(f"Checking if SSH key exists"):
+        public_key = args.ssh_key.read()
+        key_name = hashlib.md5(public_key.encode("utf-8")).hexdigest()
+        ssh_key = SSHKey(name=key_name, public_key=public_key)
+
+        if not client.ssh_keys.get_by_name(name=ssh_key.name):
+            with Action(f"Creating SSH key {ssh_key.name}"):
+                client.ssh_keys.create(name=ssh_key.name, public_key=ssh_key.public_key)
+
     with Action(f"Creating new server"):
         response = client.servers.create(
             name=name,
             server_type=ServerType(name=args.type),
             image=Image(name=args.image),
             location=Location(name=args.location),
-            ssh_keys=[SSHKey(name=args.hetzner_ssh_key)],
+            ssh_keys=[ssh_key],
         )
         server: BoundServer = response.server
 
     with Action(f"Waiting for server to be ready") as action:
         wait_ready(server=server, timeout=timeout, action=action)
 
     with Action("Wait for SSH connection to be ready"):
```

### Comparing `testflows.github.runners-1.1.230725.1020751/testflows/github/runners/request.py` & `testflows.github.runners-1.1.230725.1021028/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1020751/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.1.230725.1021028/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1020751/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.1.230725.1021028/testflows/github/runners/scale_up.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1020751/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.1.230725.1021028/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1020751/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.1.230725.1021028/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1020751/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.1.230725.1021028/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1020751/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.1.230725.1021028/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1020751/testflows/github/runners/server.py` & `testflows.github.runners-1.1.230725.1021028/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1020751/testflows/github/runners/service.py` & `testflows.github.runners-1.1.230725.1021028/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1020751/testflows/github/runners/shell.py` & `testflows.github.runners-1.1.230725.1021028/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1020751/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.1.230725.1021028/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.1.230725.1020751
+Version: 1.1.230725.1021028
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.1.230725.1020751/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.1.230725.1021028/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

