# Comparing `tmp/testflows.github.runners-1.1.230725.1010307.tar.gz` & `tmp/testflows.github.runners-1.1.230725.1010623.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.1.230725.1010307.tar", last modified: Tue Jul 25 01:03:07 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.1.230725.1010623.tar", last modified: Tue Jul 25 01:06:23 2023, max compression
```

## Comparing `testflows.github.runners-1.1.230725.1010307.tar` & `testflows.github.runners-1.1.230725.1010623.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:03:07.573266 testflows.github.runners-1.1.230725.1010307/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.1.230725.1010307/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    22488 2023-07-25 01:03:07.573266 testflows.github.runners-1.1.230725.1010307/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    21896 2023-07-25 00:55:47.000000 testflows.github.runners-1.1.230725.1010307/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-25 01:03:07.573266 testflows.github.runners-1.1.230725.1010307/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-25 01:03:07.000000 testflows.github.runners-1.1.230725.1010307/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:03:07.569266 testflows.github.runners-1.1.230725.1010307/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:03:07.569266 testflows.github.runners-1.1.230725.1010307/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:03:07.573266 testflows.github.runners-1.1.230725.1010307/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-25 01:03:07.000000 testflows.github.runners-1.1.230725.1010307/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.1.230725.1010307/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1173 2023-07-24 19:41:30.000000 testflows.github.runners-1.1.230725.1010307/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:03:07.573266 testflows.github.runners-1.1.230725.1010307/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    14128 2023-07-25 00:50:26.000000 testflows.github.runners-1.1.230725.1010307/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)     4106 2023-07-25 01:02:35.000000 testflows.github.runners-1.1.230725.1010307/testflows/github/runners/deploy.py
--rw-rw-r--   0 user      (1000) user      (1000)     1266 2023-07-24 15:25:53.000000 testflows.github.runners-1.1.230725.1010307/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     8365 2023-07-24 14:06:05.000000 testflows.github.runners-1.1.230725.1010307/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)     7972 2023-07-24 23:49:06.000000 testflows.github.runners-1.1.230725.1010307/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:03:07.573266 testflows.github.runners-1.1.230725.1010307/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.1.230725.1010307/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:03:07.573266 testflows.github.runners-1.1.230725.1010307/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.1.230725.1010307/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      266 2023-07-24 22:16:12.000000 testflows.github.runners-1.1.230725.1010307/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-24 22:14:55.000000 testflows.github.runners-1.1.230725.1010307/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-24 01:28:32.000000 testflows.github.runners-1.1.230725.1010307/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      714 2023-07-24 01:27:59.000000 testflows.github.runners-1.1.230725.1010307/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.1.230725.1010307/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     4443 2023-07-24 22:01:20.000000 testflows.github.runners-1.1.230725.1010307/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1392 2023-07-24 23:28:45.000000 testflows.github.runners-1.1.230725.1010307/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:03:07.569266 testflows.github.runners-1.1.230725.1010307/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    22488 2023-07-25 01:03:07.000000 testflows.github.runners-1.1.230725.1010307/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1001 2023-07-25 01:03:07.000000 testflows.github.runners-1.1.230725.1010307/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-25 01:03:07.000000 testflows.github.runners-1.1.230725.1010307/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.1.230725.1010307/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-25 01:03:07.000000 testflows.github.runners-1.1.230725.1010307/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-25 01:03:07.000000 testflows.github.runners-1.1.230725.1010307/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:06:23.908331 testflows.github.runners-1.1.230725.1010623/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.1.230725.1010623/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    22494 2023-07-25 01:06:23.908331 testflows.github.runners-1.1.230725.1010623/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    21902 2023-07-25 01:05:56.000000 testflows.github.runners-1.1.230725.1010623/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-25 01:06:23.908331 testflows.github.runners-1.1.230725.1010623/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-25 01:06:23.000000 testflows.github.runners-1.1.230725.1010623/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:06:23.904331 testflows.github.runners-1.1.230725.1010623/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:06:23.904331 testflows.github.runners-1.1.230725.1010623/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:06:23.908331 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-25 01:06:23.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1173 2023-07-24 19:41:30.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:06:23.908331 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    14128 2023-07-25 01:05:24.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)     4106 2023-07-25 01:02:35.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/deploy.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1266 2023-07-24 15:25:53.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8365 2023-07-24 14:06:05.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7972 2023-07-24 23:49:06.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:06:23.908331 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:06:23.908331 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      266 2023-07-24 22:16:12.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-24 22:14:55.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-24 01:28:32.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      714 2023-07-24 01:27:59.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4443 2023-07-24 22:01:20.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1392 2023-07-24 23:28:45.000000 testflows.github.runners-1.1.230725.1010623/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 01:06:23.908331 testflows.github.runners-1.1.230725.1010623/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    22494 2023-07-25 01:06:23.000000 testflows.github.runners-1.1.230725.1010623/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1001 2023-07-25 01:06:23.000000 testflows.github.runners-1.1.230725.1010623/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-25 01:06:23.000000 testflows.github.runners-1.1.230725.1010623/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.1.230725.1010623/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-25 01:06:23.000000 testflows.github.runners-1.1.230725.1010623/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-25 01:06:23.000000 testflows.github.runners-1.1.230725.1010623/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.1.230725.1010307/LICENSE` & `testflows.github.runners-1.1.230725.1010623/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1010307/PKG-INFO` & `testflows.github.runners-1.1.230725.1010623/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.1.230725.1010307
+Version: 1.1.230725.1010623
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -175,15 +175,15 @@
       Group=1000
       Type=simple
       Restart=always
       Environment=GITHUB_TOKEN=ghp_...
       Environment=GITHUB_REPOSITORY=testflows/github-runners
       Environment=HETZNER_TOKEN=GJ..
       Environment=HETZNER_SSH_KEY=user@user-node
-      Environment=HETZNER_IMAGE=ubuntu-20.04
+      Environment=HETZNER_IMAGE=ubuntu-22.04
       ExecStart=/home/user/.local/lib/python3.10/site-packages/testflows/github/runners/bin/github-runners --workers 10 --max-powered-off-time 20 --max-idle-runner-time 120 --max-runner-registration-time 60 --scale-up-interval 10 --scale-down-interval 10
       [Install]
       WantedBy=multi-user.target
 
 Modifying Program Options
 =========================
 
@@ -325,15 +325,15 @@
 The **deploy** command will use the following default values:
 
 :location:
    *ash*
 :type:
    *cpx11*
 :image:
-   *ubuntu-20.04*
+   *ubuntu-22.04*
 
 You can customize deployment server location, type, and image using the *--location*, *--type*, and *--image* options.
 
 .. code-block:: bash
 
    github-runners deploy --location nbg1 --type cx11 --image ubuntu-22.04
 
@@ -549,21 +549,21 @@
 * **--hetzner-token HETZNER_TOKEN**
   Hetzner Cloud token, default: *$HETZNER_TOKEN* environment variable
 
 * **--ssh-key HETZNER_SSH_KEY**
   Hetzner Cloud SSH key name, default: *$HETZNER_SSH_KEY* environment variable
 
 * **--image HETZNER_IMAGE**
-  Hetzner Cloud server image name, default: ubuntu-20.04
+  Hetzner Cloud server image name, default: *ubuntu-22.04*
 
 * **-m count, --max-runners count**
-  maximum number of active runners, default: unlimited
+  maximum number of active runners, default: *unlimited*
 
 * **-w count, --workers count**
-  number of concurrent workers, default: 10
+  number of concurrent workers, default: *10*
 
 * **--logger-config path**
   custom logger configuration file
 
 * **--setup-script path**
   path to custom server setup script
 
@@ -607,15 +607,15 @@
       * **-l name, --location name**
         deployment server location, default: *ash*
 
       * **-t name, --type name**
         deployment server type, default: *cpx11*
 
       * **-i name, --image name**
-        deployment server image, default: *ubuntu-20.04*
+        deployment server image, default: *ubuntu-22.04*
 
     * **service**
       service commands
 
       * **install**
         install service
```

### Comparing `testflows.github.runners-1.1.230725.1010307/README.rst` & `testflows.github.runners-1.1.230725.1010623/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
       Group=1000
       Type=simple
       Restart=always
       Environment=GITHUB_TOKEN=ghp_...
       Environment=GITHUB_REPOSITORY=testflows/github-runners
       Environment=HETZNER_TOKEN=GJ..
       Environment=HETZNER_SSH_KEY=user@user-node
-      Environment=HETZNER_IMAGE=ubuntu-20.04
+      Environment=HETZNER_IMAGE=ubuntu-22.04
       ExecStart=/home/user/.local/lib/python3.10/site-packages/testflows/github/runners/bin/github-runners --workers 10 --max-powered-off-time 20 --max-idle-runner-time 120 --max-runner-registration-time 60 --scale-up-interval 10 --scale-down-interval 10
       [Install]
       WantedBy=multi-user.target
 
 Modifying Program Options
 =========================
 
@@ -308,15 +308,15 @@
 The **deploy** command will use the following default values:
 
 :location:
    *ash*
 :type:
    *cpx11*
 :image:
-   *ubuntu-20.04*
+   *ubuntu-22.04*
 
 You can customize deployment server location, type, and image using the *--location*, *--type*, and *--image* options.
 
 .. code-block:: bash
 
    github-runners deploy --location nbg1 --type cx11 --image ubuntu-22.04
 
@@ -532,21 +532,21 @@
 * **--hetzner-token HETZNER_TOKEN**
   Hetzner Cloud token, default: *$HETZNER_TOKEN* environment variable
 
 * **--ssh-key HETZNER_SSH_KEY**
   Hetzner Cloud SSH key name, default: *$HETZNER_SSH_KEY* environment variable
 
 * **--image HETZNER_IMAGE**
-  Hetzner Cloud server image name, default: ubuntu-20.04
+  Hetzner Cloud server image name, default: *ubuntu-22.04*
 
 * **-m count, --max-runners count**
-  maximum number of active runners, default: unlimited
+  maximum number of active runners, default: *unlimited*
 
 * **-w count, --workers count**
-  number of concurrent workers, default: 10
+  number of concurrent workers, default: *10*
 
 * **--logger-config path**
   custom logger configuration file
 
 * **--setup-script path**
   path to custom server setup script
 
@@ -590,15 +590,15 @@
       * **-l name, --location name**
         deployment server location, default: *ash*
 
       * **-t name, --type name**
         deployment server type, default: *cpx11*
 
       * **-i name, --image name**
-        deployment server image, default: *ubuntu-20.04*
+        deployment server image, default: *ubuntu-22.04*
 
     * **service**
       service commands
 
       * **install**
         install service
```

### Comparing `testflows.github.runners-1.1.230725.1010307/setup.py` & `testflows.github.runners-1.1.230725.1010623/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.1.230725.1010307",
+    version="1.1.230725.1010623",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.1.230725.1010307/testflows/github/runners/__init__.py` & `testflows.github.runners-1.1.230725.1010623/testflows/github/runners/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.1.230725.1010307"
+__version__ = "1.1.230725.1010623"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.1.230725.1010307/testflows/github/runners/actions.py` & `testflows.github.runners-1.1.230725.1010623/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1010307/testflows/github/runners/args.py` & `testflows.github.runners-1.1.230725.1010623/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1010307/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.1.230725.1010623/testflows/github/runners/bin/github-runners`

 * *Files 0% similar despite different names*

```diff
@@ -128,18 +128,18 @@
     )
 
     parser.add_argument(
         "--hetzner-image",
         metavar="HETZNER_IMAGE",
         type=env_var("HETZNER_IMAGE"),
         help=(
-            "Hetzner Cloud server image name, default: ubuntu-20.04, "
+            "Hetzner Cloud server image name, default: ubuntu-22.04, "
             "or if specified, $HETZNER_IMAGE environment variable value"
         ),
-        default="ubuntu-20.04",
+        default="ubuntu-22.04",
     )
 
     parser.add_argument(
         "-w",
         "--workers",
         metavar="count",
         type=count,
@@ -258,16 +258,16 @@
         help="deployment server type, default: cpx11",
         default="cpx11",
     )
     deploy_parser.add_argument(
         "-i", "--image",
         metavar="name",
         type=str,
-        help="deployment server image, default: ubuntu-20.04",
-        default="ubuntu-20.04",
+        help="deployment server image, default: ubuntu-22.04",
+        default="ubuntu-22.04",
     )
     deploy_parser.set_defaults(func=deploy)
 
     service_parser = commands.add_parser(
         "service",
         help="service commands",
         description="Service commands.",
```

### Comparing `testflows.github.runners-1.1.230725.1010307/testflows/github/runners/deploy.py` & `testflows.github.runners-1.1.230725.1010623/testflows/github/runners/deploy.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1010307/testflows/github/runners/request.py` & `testflows.github.runners-1.1.230725.1010623/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1010307/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1010307/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scale_up.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1010307/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1010307/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1010307/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1010307/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.1.230725.1010623/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1010307/testflows/github/runners/server.py` & `testflows.github.runners-1.1.230725.1010623/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1010307/testflows/github/runners/service.py` & `testflows.github.runners-1.1.230725.1010623/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1010307/testflows/github/runners/shell.py` & `testflows.github.runners-1.1.230725.1010623/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1010307/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.1.230725.1010623/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.1.230725.1010307
+Version: 1.1.230725.1010623
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -175,15 +175,15 @@
       Group=1000
       Type=simple
       Restart=always
       Environment=GITHUB_TOKEN=ghp_...
       Environment=GITHUB_REPOSITORY=testflows/github-runners
       Environment=HETZNER_TOKEN=GJ..
       Environment=HETZNER_SSH_KEY=user@user-node
-      Environment=HETZNER_IMAGE=ubuntu-20.04
+      Environment=HETZNER_IMAGE=ubuntu-22.04
       ExecStart=/home/user/.local/lib/python3.10/site-packages/testflows/github/runners/bin/github-runners --workers 10 --max-powered-off-time 20 --max-idle-runner-time 120 --max-runner-registration-time 60 --scale-up-interval 10 --scale-down-interval 10
       [Install]
       WantedBy=multi-user.target
 
 Modifying Program Options
 =========================
 
@@ -325,15 +325,15 @@
 The **deploy** command will use the following default values:
 
 :location:
    *ash*
 :type:
    *cpx11*
 :image:
-   *ubuntu-20.04*
+   *ubuntu-22.04*
 
 You can customize deployment server location, type, and image using the *--location*, *--type*, and *--image* options.
 
 .. code-block:: bash
 
    github-runners deploy --location nbg1 --type cx11 --image ubuntu-22.04
 
@@ -549,21 +549,21 @@
 * **--hetzner-token HETZNER_TOKEN**
   Hetzner Cloud token, default: *$HETZNER_TOKEN* environment variable
 
 * **--ssh-key HETZNER_SSH_KEY**
   Hetzner Cloud SSH key name, default: *$HETZNER_SSH_KEY* environment variable
 
 * **--image HETZNER_IMAGE**
-  Hetzner Cloud server image name, default: ubuntu-20.04
+  Hetzner Cloud server image name, default: *ubuntu-22.04*
 
 * **-m count, --max-runners count**
-  maximum number of active runners, default: unlimited
+  maximum number of active runners, default: *unlimited*
 
 * **-w count, --workers count**
-  number of concurrent workers, default: 10
+  number of concurrent workers, default: *10*
 
 * **--logger-config path**
   custom logger configuration file
 
 * **--setup-script path**
   path to custom server setup script
 
@@ -607,15 +607,15 @@
       * **-l name, --location name**
         deployment server location, default: *ash*
 
       * **-t name, --type name**
         deployment server type, default: *cpx11*
 
       * **-i name, --image name**
-        deployment server image, default: *ubuntu-20.04*
+        deployment server image, default: *ubuntu-22.04*
 
     * **service**
       service commands
 
       * **install**
         install service
```

### Comparing `testflows.github.runners-1.1.230725.1010307/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.1.230725.1010623/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

