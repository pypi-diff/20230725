# Comparing `tmp/testflows.github.runners-1.1.230725.1010623.tar.gz` & `tmp/testflows.github.runners-1.1.230725.1011420.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.1.230725.1010623.tar", last modified: Tue Jul 25 01:06:23 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.1.230725.1011420.tar", last modified: Tue Jul 25 01:14:20 2023, max compression
```

## Comparing `testflows.github.runners-1.1.230725.1010623.tar` & `testflows.github.runners-1.1.230725.1011420.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:06:23.908331 testflows.github.runners-1.1.230725.1010623/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.1.230725.1010623/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    22494 2023-07-25 01:06:23.908331 testflows.github.runners-1.1.230725.1010623/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    21902 2023-07-25 01:05:56.000000 testflows.github.runners-1.1.230725.1010623/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-25 01:06:23.908331 testflows.github.runners-1.1.230725.1010623/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-25 01:06:23.000000 testflows.github.runners-1.1.230725.1010623/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:06:23.904331 testflows.github.runners-1.1.230725.1010623/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:06:23.904331 testflows.github.runners-1.1.230725.1010623/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:06:23.908331 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-25 01:06:23.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1173 2023-07-24 19:41:30.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:06:23.908331 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    14128 2023-07-25 01:05:24.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)     4106 2023-07-25 01:02:35.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/deploy.py
--rw-rw-r--   0 user      (1000) user      (1000)     1266 2023-07-24 15:25:53.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     8365 2023-07-24 14:06:05.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)     7972 2023-07-24 23:49:06.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:06:23.908331 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:06:23.908331 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      266 2023-07-24 22:16:12.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-24 22:14:55.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-24 01:28:32.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      714 2023-07-24 01:27:59.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     4443 2023-07-24 22:01:20.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1392 2023-07-24 23:28:45.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:06:23.908331 testflows.github.runners-1.1.230725.1010623/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    22494 2023-07-25 01:06:23.000000 testflows.github.runners-1.1.230725.1010623/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1001 2023-07-25 01:06:23.000000 testflows.github.runners-1.1.230725.1010623/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-25 01:06:23.000000 testflows.github.runners-1.1.230725.1010623/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.1.230725.1010623/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-25 01:06:23.000000 testflows.github.runners-1.1.230725.1010623/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-25 01:06:23.000000 testflows.github.runners-1.1.230725.1010623/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:14:20.295345 testflows.github.runners-1.1.230725.1011420/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.1.230725.1011420/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    22494 2023-07-25 01:14:20.295345 testflows.github.runners-1.1.230725.1011420/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    21902 2023-07-25 01:05:56.000000 testflows.github.runners-1.1.230725.1011420/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-25 01:14:20.295345 testflows.github.runners-1.1.230725.1011420/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-25 01:14:20.000000 testflows.github.runners-1.1.230725.1011420/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:14:20.291345 testflows.github.runners-1.1.230725.1011420/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:14:20.291345 testflows.github.runners-1.1.230725.1011420/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:14:20.295345 testflows.github.runners-1.1.230725.1011420/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-25 01:14:20.000000 testflows.github.runners-1.1.230725.1011420/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.1.230725.1011420/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1173 2023-07-24 19:41:30.000000 testflows.github.runners-1.1.230725.1011420/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:14:20.295345 testflows.github.runners-1.1.230725.1011420/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    14128 2023-07-25 01:05:24.000000 testflows.github.runners-1.1.230725.1011420/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)     4106 2023-07-25 01:02:35.000000 testflows.github.runners-1.1.230725.1011420/testflows/github/runners/deploy.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1266 2023-07-24 15:25:53.000000 testflows.github.runners-1.1.230725.1011420/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8571 2023-07-25 01:13:14.000000 testflows.github.runners-1.1.230725.1011420/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8184 2023-07-25 01:13:14.000000 testflows.github.runners-1.1.230725.1011420/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:14:20.295345 testflows.github.runners-1.1.230725.1011420/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.1.230725.1011420/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:14:20.295345 testflows.github.runners-1.1.230725.1011420/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.1.230725.1011420/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      266 2023-07-24 22:16:12.000000 testflows.github.runners-1.1.230725.1011420/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-24 22:14:55.000000 testflows.github.runners-1.1.230725.1011420/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-24 01:28:32.000000 testflows.github.runners-1.1.230725.1011420/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      714 2023-07-24 01:27:59.000000 testflows.github.runners-1.1.230725.1011420/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.1.230725.1011420/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4443 2023-07-24 22:01:20.000000 testflows.github.runners-1.1.230725.1011420/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1392 2023-07-24 23:28:45.000000 testflows.github.runners-1.1.230725.1011420/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:14:20.295345 testflows.github.runners-1.1.230725.1011420/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    22494 2023-07-25 01:14:20.000000 testflows.github.runners-1.1.230725.1011420/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1001 2023-07-25 01:14:20.000000 testflows.github.runners-1.1.230725.1011420/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-25 01:14:20.000000 testflows.github.runners-1.1.230725.1011420/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.1.230725.1011420/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-25 01:14:20.000000 testflows.github.runners-1.1.230725.1011420/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-25 01:14:20.000000 testflows.github.runners-1.1.230725.1011420/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.1.230725.1010623/LICENSE` & `testflows.github.runners-1.1.230725.1011420/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1010623/PKG-INFO` & `testflows.github.runners-1.1.230725.1011420/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.1.230725.1010623
+Version: 1.1.230725.1011420
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.1.230725.1010623/README.rst` & `testflows.github.runners-1.1.230725.1011420/README.rst`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1010623/setup.py` & `testflows.github.runners-1.1.230725.1011420/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.1.230725.1010623",
+    version="1.1.230725.1011420",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.1.230725.1010623/testflows/github/runners/__init__.py` & `testflows.github.runners-1.1.230725.1011420/testflows/github/runners/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.1.230725.1010623"
+__version__ = "1.1.230725.1011420"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.1.230725.1010623/testflows/github/runners/actions.py` & `testflows.github.runners-1.1.230725.1011420/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1010623/testflows/github/runners/args.py` & `testflows.github.runners-1.1.230725.1011420/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1010623/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.1.230725.1011420/testflows/github/runners/bin/github-runners`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1010623/testflows/github/runners/deploy.py` & `testflows.github.runners-1.1.230725.1011420/testflows/github/runners/deploy.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1010623/testflows/github/runners/request.py` & `testflows.github.runners-1.1.230725.1011420/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.1.230725.1011420/testflows/github/runners/scale_down.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import time
 import logging
 import threading
 
 from dataclasses import dataclass
 
 from .actions import Action
+from .scale_up import runner_server_prefix
 
 from github.Repository import Repository
 from github.SelfHostedActionsRunner import SelfHostedActionsRunner
 
 from hcloud import Client
 from hcloud.servers.client import BoundServer
 
@@ -76,14 +77,19 @@
 
         if terminate.is_set():
             with Action("Terminating scale down service"):
                 break
 
         with Action("Getting list of servers", level=logging.DEBUG):
             servers: list[BoundServer] = client.servers.get_all()
+            servers = [
+                server
+                for server in servers
+                if server.name.startswith(runner_server_prefix)
+            ]
 
         with Action("Getting list of self-hosted runners", level=logging.DEBUG):
             runners: list[SelfHostedActionsRunner] = repo.get_self_hosted_runners()
 
         with Action("Looking for powered off or zombie servers", level=logging.DEBUG):
             for server in servers:
                 if server.status == server.STATUS_OFF:
```

### Comparing `testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.1.230725.1011420/testflows/github/runners/scale_up.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 from hcloud.images.domain import Image
 
 from github.Repository import Repository
 from github.WorkflowJob import WorkflowJob
 
 from concurrent.futures import ThreadPoolExecutor, Future
 
+runner_server_prefix = "github-runner-"
+
 
 def server_setup(
     server: BoundServer,
     setup_script: str,
     startup_script: str,
     github_token: str,
     github_repository: str,
@@ -163,26 +165,31 @@
     while True:
         if terminate.is_set():
             with Action("Terminating scale up service"):
                 break
 
         with Action("Getting list of servers", level=logging.DEBUG):
             servers: list[BoundServer] = client.servers.get_all()
+            servers = [
+                server
+                for server in servers
+                if server.name.startswith(runner_server_prefix)
+            ]
 
         with Action("Getting workflow runs", level=logging.DEBUG):
             workflow_runs = repo.get_workflow_runs(branch="main", status="queued")
 
         futures: list[Future] = []
 
         with Action("Looking for queued jobs", level=logging.DEBUG) as action:
             for run in workflow_runs:
                 for job in run.jobs():
                     if job.status == "queued":
                         with Action(f"Found queued job {job}"):
-                            server_name = f"github-runner-{job.run_id}"
+                            server_name = f"{runner_server_prefix}{job.run_id}"
                             server_type = get_server_type(job=job)
                             startup_script = get_startup_script(
                                 server_type=server_type, scripts=scripts
                             )
 
                             if max_servers is not None:
                                 with Action(
```

### Comparing `testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.1.230725.1011420/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.1.230725.1011420/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.1.230725.1011420/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.1.230725.1011420/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1010623/testflows/github/runners/server.py` & `testflows.github.runners-1.1.230725.1011420/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1010623/testflows/github/runners/service.py` & `testflows.github.runners-1.1.230725.1011420/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1010623/testflows/github/runners/shell.py` & `testflows.github.runners-1.1.230725.1011420/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1010623/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.1.230725.1011420/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.1.230725.1010623
+Version: 1.1.230725.1011420
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.1.230725.1010623/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.1.230725.1011420/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

