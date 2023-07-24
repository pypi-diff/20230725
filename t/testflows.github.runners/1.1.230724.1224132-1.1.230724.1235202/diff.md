# Comparing `tmp/testflows.github.runners-1.1.230724.1224132.tar.gz` & `tmp/testflows.github.runners-1.1.230724.1235202.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.1.230724.1224132.tar", last modified: Mon Jul 24 22:41:32 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.1.230724.1235202.tar", last modified: Mon Jul 24 23:52:02 2023, max compression
```

## Comparing `testflows.github.runners-1.1.230724.1224132.tar` & `testflows.github.runners-1.1.230724.1235202.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 22:41:32.820220 testflows.github.runners-1.1.230724.1224132/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.1.230724.1224132/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    21124 2023-07-24 22:41:32.820220 testflows.github.runners-1.1.230724.1224132/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    20532 2023-07-24 22:41:19.000000 testflows.github.runners-1.1.230724.1224132/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-24 22:41:32.820220 testflows.github.runners-1.1.230724.1224132/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-24 22:41:32.000000 testflows.github.runners-1.1.230724.1224132/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 22:41:32.816220 testflows.github.runners-1.1.230724.1224132/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 22:41:32.816220 testflows.github.runners-1.1.230724.1224132/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 22:41:32.820220 testflows.github.runners-1.1.230724.1224132/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-24 22:41:32.000000 testflows.github.runners-1.1.230724.1224132/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      979 2023-07-24 20:59:02.000000 testflows.github.runners-1.1.230724.1224132/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1173 2023-07-24 19:41:30.000000 testflows.github.runners-1.1.230724.1224132/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 22:41:32.820220 testflows.github.runners-1.1.230724.1224132/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    12980 2023-07-24 22:29:17.000000 testflows.github.runners-1.1.230724.1224132/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)     4510 2023-07-24 22:39:23.000000 testflows.github.runners-1.1.230724.1224132/testflows/github/runners/deploy.py
--rw-rw-r--   0 user      (1000) user      (1000)     1266 2023-07-24 15:25:53.000000 testflows.github.runners-1.1.230724.1224132/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     8365 2023-07-24 14:06:05.000000 testflows.github.runners-1.1.230724.1224132/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)     8767 2023-07-24 22:25:34.000000 testflows.github.runners-1.1.230724.1224132/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 22:41:32.820220 testflows.github.runners-1.1.230724.1224132/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.1.230724.1224132/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 22:41:32.820220 testflows.github.runners-1.1.230724.1224132/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.1.230724.1224132/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      266 2023-07-24 22:16:12.000000 testflows.github.runners-1.1.230724.1224132/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-24 22:14:55.000000 testflows.github.runners-1.1.230724.1224132/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-24 01:28:32.000000 testflows.github.runners-1.1.230724.1224132/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      714 2023-07-24 01:27:59.000000 testflows.github.runners-1.1.230724.1224132/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     4443 2023-07-24 22:01:20.000000 testflows.github.runners-1.1.230724.1224132/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1151 2023-07-24 12:06:14.000000 testflows.github.runners-1.1.230724.1224132/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 22:41:32.816220 testflows.github.runners-1.1.230724.1224132/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    21124 2023-07-24 22:41:32.000000 testflows.github.runners-1.1.230724.1224132/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      966 2023-07-24 22:41:32.000000 testflows.github.runners-1.1.230724.1224132/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 22:41:32.000000 testflows.github.runners-1.1.230724.1224132/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.1.230724.1224132/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-24 22:41:32.000000 testflows.github.runners-1.1.230724.1224132/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-24 22:41:32.000000 testflows.github.runners-1.1.230724.1224132/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 23:52:02.319094 testflows.github.runners-1.1.230724.1235202/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.1.230724.1235202/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    21124 2023-07-24 23:52:02.319094 testflows.github.runners-1.1.230724.1235202/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    20532 2023-07-24 22:41:19.000000 testflows.github.runners-1.1.230724.1235202/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-24 23:52:02.319094 testflows.github.runners-1.1.230724.1235202/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-24 23:52:02.000000 testflows.github.runners-1.1.230724.1235202/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 23:52:02.315094 testflows.github.runners-1.1.230724.1235202/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 23:52:02.315094 testflows.github.runners-1.1.230724.1235202/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 23:52:02.319094 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-24 23:52:02.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      979 2023-07-24 20:59:02.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1173 2023-07-24 19:41:30.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 23:52:02.319094 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    12980 2023-07-24 22:29:17.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)     3759 2023-07-24 23:51:42.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/deploy.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1266 2023-07-24 15:25:53.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8365 2023-07-24 14:06:05.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7972 2023-07-24 23:49:06.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 23:52:02.319094 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 23:52:02.319094 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      266 2023-07-24 22:16:12.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-24 22:14:55.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-24 01:28:32.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      714 2023-07-24 01:27:59.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4443 2023-07-24 22:01:20.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1392 2023-07-24 23:28:45.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 23:52:02.319094 testflows.github.runners-1.1.230724.1235202/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    21124 2023-07-24 23:52:02.000000 testflows.github.runners-1.1.230724.1235202/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1001 2023-07-24 23:52:02.000000 testflows.github.runners-1.1.230724.1235202/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 23:52:02.000000 testflows.github.runners-1.1.230724.1235202/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.1.230724.1235202/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-24 23:52:02.000000 testflows.github.runners-1.1.230724.1235202/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-24 23:52:02.000000 testflows.github.runners-1.1.230724.1235202/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.1.230724.1224132/LICENSE` & `testflows.github.runners-1.1.230724.1235202/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1224132/PKG-INFO` & `testflows.github.runners-1.1.230724.1235202/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.1.230724.1224132
+Version: 1.1.230724.1235202
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.1.230724.1224132/README.rst` & `testflows.github.runners-1.1.230724.1235202/README.rst`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1224132/setup.py` & `testflows.github.runners-1.1.230724.1235202/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.1.230724.1224132",
+    version="1.1.230724.1235202",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.1.230724.1224132/testflows/github/runners/__init__.py` & `testflows.github.runners-1.1.230724.1235202/testflows/github/runners/__init__.py`

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
-__version__ = "1.1.230724.1224132"
+__version__ = "1.1.230724.1235202"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.1.230724.1224132/testflows/github/runners/actions.py` & `testflows.github.runners-1.1.230724.1235202/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1224132/testflows/github/runners/args.py` & `testflows.github.runners-1.1.230724.1235202/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1224132/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.1.230724.1235202/testflows/github/runners/bin/github-runners`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1224132/testflows/github/runners/deploy.py` & `testflows.github.runners-1.1.230724.1235202/testflows/github/runners/deploy.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,94 +18,67 @@
 from hcloud import Client
 from hcloud.ssh_keys.domain import SSHKey
 from hcloud.server_types.domain import ServerType
 from hcloud.servers.client import BoundServer
 from hcloud.images.domain import Image
 
 from .actions import Action
-from .shell import shell
 from .args import check
 from . import __version__
 
+from .server import wait_ready, wait_ssh, ssh
+
 current_dir = os.path.dirname(__file__)
 
 
 def deploy(args, timeout=60):
     """Deploy github-runners as a service to a
     new Hetzner server instance."""
     check(args)
 
     with Action("Logging in to Hetzner Cloud"):
         client = Client(token=args.hetzner_token)
 
     with Action(f"Creating new server"):
         response = client.servers.create(
             name="github-runners",
-            server_type=ServerType("cx11"),
-            image=Image(args.hetzner_image),
+            server_type=ServerType("cpx11"),
+            image=Image("ubuntu-20.04"),
             ssh_keys=[SSHKey(name=args.hetzner_ssh_key)],
         )
         server: BoundServer = response.server
 
-    with Action(f"Waiting for server {server.name}") as action:
-        start_time = time.time()
+    with Action(f"Waiting for server {server.name} to be ready") as action:
+        wait_ready(server=server, timeout=timeout, action=action)
 
-        while True:
-            status = server.status
-            action.note(f"{server.name} {status}")
-            if status == server.STATUS_RUNNING:
-                break
-            if time.time() - start_time >= timeout:
-                raise TimeoutError("waiting for server to start running")
-            time.sleep(1)
-            server.reload()
-
-    ip = server.public_net.primary_ipv4.ip
-    ssh = f'ssh -q -o "StrictHostKeyChecking no" root@{ip}'
-
-    with Action("SSH to server"):
-        attempt = -1
-        start_time = time.time()
-
-        while True:
-            attempt += 1
-
-            with Action(
-                f"Trying to connect to {server.name}@{ip}...{attempt}", ignore_fail=True
-            ):
-                returncode = shell(f"{ssh} hostname")
-                if returncode == 0:
-                    break
-
-            if time.time() - start_time >= timeout:
-                shell(f"{ssh} hostname")
-            else:
-                time.sleep(5)
+    with Action("Wait for SSH connection to be ready"):
+        wait_ssh(server=server, timeout=timeout)
 
     with Action("Executing setup.sh script"):
-        shell(
-            f"{ssh} bash -s  < {os.path.join(current_dir, 'scripts', 'deploy', 'setup.sh')}"
+        ssh(
+            server,
+            f"bash -s  < {os.path.join(current_dir, 'scripts', 'deploy', 'setup.sh')}",
         )
 
     with Action("Installing github-runners"):
-        shell(f"{ssh} 'sudo -u runner pip3 install testflows.github.runners'")
+        ssh(
+            server,
+            f"'sudo -u runner pip3 install testflows.github.runners=={__version__}'",
+        )
 
     with Action("Installing service"):
-        command = f"{ssh} 'sudo -u runner "
-
+        command = f"su - runner -c '"
         command += f"GITHUB_TOKEN={args.github_token} "
         command += f"GITHUB_REPOSITORY={args.github_repository} "
         command += f"HETZNER_TOKEN={args.hetzner_token} "
         command += f"HETZNER_SSH_KEY={args.hetzner_ssh_key} "
         command += f"HETZNER_IMAGE={args.hetzner_image} "
 
         command += "github-runners"
-
         command += f" --workers {args.workers}"
-
         command += f" --max-runners {args.max_runners}" if args.max_runners else ""
         command += (
             f" --logger-config {args.logger_config}" if args.logger_config else ""
         )
         command += f" --setup-script {args.setup_script}" if args.setup_script else ""
         command += (
             f" --startup-x64-script {args.startup_x64_script}"
@@ -121,10 +94,10 @@
             f" --max-powered-off-time {args.max_powered_off_time}"
             f" --max-idle-runner-time {args.max_idle_runner_time}"
             f" --max-runner-registration-time {args.max_runner_registration_time}"
             f" --scale-up-interval {args.scale_up_interval}"
             f" --scale-down-interval {args.scale_down_interval}"
         )
         command += f" --debug" if args.debug else ""
-        command += " service install'"
+        command += " service install -f'"
 
-        shell(command)
+        ssh(server, command)
```

### Comparing `testflows.github.runners-1.1.230724.1224132/testflows/github/runners/request.py` & `testflows.github.runners-1.1.230724.1235202/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1224132/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1224132/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scale_up.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,18 +14,19 @@
 # limitations under the License.
 import os
 import time
 import logging
 import threading
 
 from .actions import Action
-from .shell import shell
 from .scripts import Scripts
 from .request import request
 
+from .server import wait_ssh, ssh, wait_ready
+
 from hcloud import Client
 from hcloud.ssh_keys.domain import SSHKey
 from hcloud.server_types.domain import ServerType
 from hcloud.servers.client import BoundServer
 from hcloud.images.domain import Image
 
 from github.Repository import Repository
@@ -40,64 +41,45 @@
     startup_script: str,
     github_token: str,
     github_repository: str,
     runner_labels: str,
     timeout: float = 60,
 ):
     """Setup new server instance."""
-
-    ip = server.public_net.primary_ipv4.ip
-    ssh = f'ssh -q -o "StrictHostKeyChecking no" root@{ip}'
-
-    with Action("SSH to server"):
-        attempt = -1
-        start_time = time.time()
-
-        while True:
-            attempt += 1
-
-            with Action(
-                f"Trying to connect to {server.name}@{ip}...{attempt}", ignore_fail=True
-            ):
-                returncode = shell(f"{ssh} hostname")
-                if returncode == 0:
-                    break
-
-            if time.time() - start_time >= timeout:
-                shell(f"{ssh} hostname")
-            else:
-                time.sleep(5)
+    with Action("Wait for SSH connection to be ready"):
+        wait_ssh(server=server, timeout=timeout)
 
     with Action("Getting registration token for the runner"):
         content, resp = request(
             f"https://api.github.com/repos/{github_repository}/actions/runners/registration-token",
             headers={
                 "Accept": "application/vnd.github+json",
                 "Authorization": f"Bearer {github_token}",
                 "X-GitHub-Api-Version": "2022-11-28",
             },
             data={},
             format="json",
         )
         GITHUB_RUNNER_TOKEN = content["token"]
 
-    with Action("Get current directory"):
+    with Action("Getting current directory"):
         current_dir = os.path.dirname(__file__)
 
     with Action("Executing setup.sh script"):
-        shell(f"{ssh} bash -s  < {setup_script}")
+        ssh(server, f"bash -s  < {setup_script}")
 
     with Action("Executing startup.sh script"):
-        shell(
-            f"{ssh} 'sudo -u runner "
+        ssh(
+            server,
+            f"'sudo -u runner "
             f"GITHUB_REPOSITORY=\"{os.getenv('GITHUB_REPOSITORY')}\" "
             f'GITHUB_RUNNER_TOKEN="{GITHUB_RUNNER_TOKEN}" '
             f"GITHUB_RUNNER_GROUP=Default "
             f'GITHUB_RUNNER_LABELS="{runner_labels}" '
-            f"bash -s' < {startup_script}"
+            f"bash -s' < {startup_script}",
         )
 
 
 def create_server(
     client: Client,
     job: WorkflowJob,
     name: str,
@@ -118,26 +100,16 @@
             name=name,
             server_type=server_type,
             image=image,
             ssh_keys=[ssh_key],
         )
         server: BoundServer = response.server
 
-    with Action(f"Waiting for server {server.name}") as action:
-        start_time = time.time()
-
-        while True:
-            status = server.status
-            action.note(f"{server.name} {status}")
-            if status == server.STATUS_RUNNING:
-                break
-            if time.time() - start_time >= timeout:
-                raise TimeoutError("waiting for server to start running")
-            time.sleep(1)
-            server.reload()
+    with Action(f"Waiting for server {server.name} to be ready") as action:
+        wait_ready(server=server, timeout=timeout, action=action)
 
     server_setup(
         server=response.server,
         setup_script=setup_script,
         startup_script=startup_script,
         github_token=github_token,
         github_repository=github_repository,
```

### Comparing `testflows.github.runners-1.1.230724.1224132/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1224132/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1224132/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1224132/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1224132/testflows/github/runners/service.py` & `testflows.github.runners-1.1.230724.1235202/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1224132/testflows/github/runners/shell.py` & `testflows.github.runners-1.1.230724.1235202/testflows/github/runners/shell.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,28 +8,39 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import time
 import logging
 import subprocess
 
 logger = logging.getLogger("testflows.github.runners")
 
 
 def shell(cmd: str, shell: bool = True, check: bool = True):
     """Execute command."""
-    p = subprocess.run(
+    p = subprocess.Popen(
         cmd,
         shell=shell,
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
-        check=check,
         bufsize=1,
         universal_newlines=True,
+        text=True,
+        encoding="utf-8",
     )
-    for line in p.stdout.splitlines():
-        logger.info(f"   > {line}", stacklevel=2)
+
+    for line in iter(p.stdout.readline, ""):
+        if line == "":
+            time.sleep(0.1)
+            continue
+        logger.info(f"   > {line.rstrip()}", stacklevel=2)
+
+    p.wait()
+
+    if check:
+        assert p.returncode == 0, f"{cmd} returned non-zero exit code {p.returncode}"
 
     return p.returncode
```

### Comparing `testflows.github.runners-1.1.230724.1224132/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.1.230724.1235202/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.1.230724.1224132
+Version: 1.1.230724.1235202
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.1.230724.1224132/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.1.230724.1235202/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 testflows/github/runners/__init__.py
 testflows/github/runners/actions.py
 testflows/github/runners/args.py
 testflows/github/runners/deploy.py
 testflows/github/runners/request.py
 testflows/github/runners/scale_down.py
 testflows/github/runners/scale_up.py
+testflows/github/runners/server.py
 testflows/github/runners/service.py
 testflows/github/runners/shell.py
 testflows/github/runners/bin/github-runners
 testflows/github/runners/scripts/__init__.py
 testflows/github/runners/scripts/setup.sh
 testflows/github/runners/scripts/startup_arm64.sh
 testflows/github/runners/scripts/startup_x64.sh
```

