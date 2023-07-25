# Comparing `tmp/testflows.github.runners-1.1.230725.1002210.tar.gz` & `tmp/testflows.github.runners-1.1.230725.1005626.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.1.230725.1002210.tar", last modified: Tue Jul 25 00:22:10 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.1.230725.1005626.tar", last modified: Tue Jul 25 00:56:26 2023, max compression
```

## Comparing `testflows.github.runners-1.1.230725.1002210.tar` & `testflows.github.runners-1.1.230725.1005626.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 00:22:10.480706 testflows.github.runners-1.1.230725.1002210/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.1.230725.1002210/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    21124 2023-07-25 00:22:10.476706 testflows.github.runners-1.1.230725.1002210/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    20532 2023-07-24 22:41:19.000000 testflows.github.runners-1.1.230725.1002210/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-25 00:22:10.480706 testflows.github.runners-1.1.230725.1002210/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-25 00:22:10.000000 testflows.github.runners-1.1.230725.1002210/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 00:22:10.476706 testflows.github.runners-1.1.230725.1002210/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 00:22:10.476706 testflows.github.runners-1.1.230725.1002210/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 00:22:10.476706 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-25 00:22:10.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1173 2023-07-24 19:41:30.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 00:22:10.476706 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    13212 2023-07-25 00:21:34.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)     3759 2023-07-25 00:21:48.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/deploy.py
--rw-rw-r--   0 user      (1000) user      (1000)     1266 2023-07-24 15:25:53.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     8365 2023-07-24 14:06:05.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)     7972 2023-07-24 23:49:06.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 00:22:10.476706 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 00:22:10.476706 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      266 2023-07-24 22:16:12.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-24 22:14:55.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-24 01:28:32.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      714 2023-07-24 01:27:59.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     4443 2023-07-24 22:01:20.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1392 2023-07-24 23:28:45.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 00:22:10.476706 testflows.github.runners-1.1.230725.1002210/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    21124 2023-07-25 00:22:10.000000 testflows.github.runners-1.1.230725.1002210/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1001 2023-07-25 00:22:10.000000 testflows.github.runners-1.1.230725.1002210/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-25 00:22:10.000000 testflows.github.runners-1.1.230725.1002210/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.1.230725.1002210/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-25 00:22:10.000000 testflows.github.runners-1.1.230725.1002210/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-25 00:22:10.000000 testflows.github.runners-1.1.230725.1002210/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 00:56:26.759602 testflows.github.runners-1.1.230725.1005626/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.1.230725.1005626/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    22488 2023-07-25 00:56:26.759602 testflows.github.runners-1.1.230725.1005626/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    21896 2023-07-25 00:55:47.000000 testflows.github.runners-1.1.230725.1005626/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-25 00:56:26.759602 testflows.github.runners-1.1.230725.1005626/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-25 00:56:26.000000 testflows.github.runners-1.1.230725.1005626/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 00:56:26.755602 testflows.github.runners-1.1.230725.1005626/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 00:56:26.755602 testflows.github.runners-1.1.230725.1005626/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 00:56:26.759602 testflows.github.runners-1.1.230725.1005626/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-25 00:56:26.000000 testflows.github.runners-1.1.230725.1005626/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.1.230725.1005626/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1173 2023-07-24 19:41:30.000000 testflows.github.runners-1.1.230725.1005626/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 00:56:26.759602 testflows.github.runners-1.1.230725.1005626/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    14128 2023-07-25 00:50:26.000000 testflows.github.runners-1.1.230725.1005626/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)     4102 2023-07-25 00:51:22.000000 testflows.github.runners-1.1.230725.1005626/testflows/github/runners/deploy.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1266 2023-07-24 15:25:53.000000 testflows.github.runners-1.1.230725.1005626/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8365 2023-07-24 14:06:05.000000 testflows.github.runners-1.1.230725.1005626/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7972 2023-07-24 23:49:06.000000 testflows.github.runners-1.1.230725.1005626/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 00:56:26.759602 testflows.github.runners-1.1.230725.1005626/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.1.230725.1005626/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 00:56:26.759602 testflows.github.runners-1.1.230725.1005626/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.1.230725.1005626/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      266 2023-07-24 22:16:12.000000 testflows.github.runners-1.1.230725.1005626/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-24 22:14:55.000000 testflows.github.runners-1.1.230725.1005626/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-24 01:28:32.000000 testflows.github.runners-1.1.230725.1005626/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      714 2023-07-24 01:27:59.000000 testflows.github.runners-1.1.230725.1005626/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.1.230725.1005626/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4443 2023-07-24 22:01:20.000000 testflows.github.runners-1.1.230725.1005626/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1392 2023-07-24 23:28:45.000000 testflows.github.runners-1.1.230725.1005626/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 00:56:26.759602 testflows.github.runners-1.1.230725.1005626/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    22488 2023-07-25 00:56:26.000000 testflows.github.runners-1.1.230725.1005626/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1001 2023-07-25 00:56:26.000000 testflows.github.runners-1.1.230725.1005626/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-25 00:56:26.000000 testflows.github.runners-1.1.230725.1005626/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.1.230725.1005626/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-25 00:56:26.000000 testflows.github.runners-1.1.230725.1005626/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-25 00:56:26.000000 testflows.github.runners-1.1.230725.1005626/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.1.230725.1002210/LICENSE` & `testflows.github.runners-1.1.230725.1005626/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1002210/PKG-INFO` & `testflows.github.runners-1.1.230725.1005626/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: testflows.github.runners
-Version: 1.1.230725.1002210
-Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
-Home-page: https://github.com/testflows/github-runners
-Author: Vitaliy Zakaznikov
-Author-email: vzakaznikov@testflows.com
-License: Apache-2.0
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
-License-File: LICENSE
-
 .. image:: https://raw.githubusercontent.com/testflows/TestFlows-ArtWork/master/images/logo.png
    :width: 20%
    :target: https://testflows.com
    :alt: test bug
 
 ======================================================
 Autoscaling GitHub Actions Runners Using Hetzner Cloud
@@ -298,14 +281,49 @@
       Jul 24 14:24:42 user-node env[62771]: LANGUAGE=en_CA:en
       Jul 24 14:24:42 user-node env[62771]: PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/snap/bin
       Jul 24 14:24:42 user-node env[62771]: INVOCATION_ID=dc7b778f95fa4ccf95e4a4592b50d9e1
       Jul 24 14:24:42 user-node env[62771]: JOURNAL_STREAM=8:328542
       Jul 24 14:24:42 user-node env[62771]: SYSTEMD_EXEC_PID=62771
       ...
 
+-----------------------
+Deploying Application
+-----------------------
+
+You can deploy **github-runners** as a service to a new Hetzner Cloud server instance
+using the **deploy** command.
+
+:✋ Note:
+   The options that are passed to the **github-runners <options> deploy** command
+   will be the same options with which the service will be executed.
+
+.. code-block:: bash
+
+   export GITHUB_TOKEN=ghp_...
+   export GITHUB_REPOSITORY=testflows/github-runners
+   export HETZNER_TOKEN=GJzdc...
+   export HETZNER_SSH_KEY_NAME=user@user-node
+
+   github-runners deploy
+
+The **deploy** command will use the following default values:
+
+:location:
+   *ash*
+:type:
+   *cpx11*
+:image:
+   *ubuntu-20.04*
+
+You can customize deployment server location, type, and image using the *--location*, *--type*, and *--image* options.
+
+.. code-block:: bash
+
+   github-runners deploy --location nbg1 --type cx11 --image ubuntu-22.04
+
 
 ------------------
 Scaling Up Runners
 ------------------
 
 The program scale up runners by looking for any jobs that have **queued** status.
 For each such job, a corresponding Hetzner Cloud server instance is created with the following name:
@@ -556,14 +574,32 @@
 * **--debug**
   enable debugging mode, default: *False*
 
 * **commands:**
 
   * *command*
 
+    * **deploy**
+      deploy application
+
+      * **-n, --name**
+        deployment server name, default: *github-runners*
+
+      * **-f, --force**
+        force deployment if already exist
+
+      * **-l name, --location name**
+        deployment server location, default: *ash*
+
+      * **-t name, --type name**
+        deployment server type, default: *cpx11*
+
+      * **-i name, --image name**
+        deployment server image, default: *ubuntu-20.04*
+
     * **service**
       service commands
 
       * **install**
         install service
 
         * **-f, --force**
```

### Comparing `testflows.github.runners-1.1.230725.1002210/README.rst` & `testflows.github.runners-1.1.230725.1005626/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: testflows.github.runners
+Version: 1.1.230725.1005626
+Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
+Home-page: https://github.com/testflows/github-runners
+Author: Vitaliy Zakaznikov
+Author-email: vzakaznikov@testflows.com
+License: Apache-2.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
+License-File: LICENSE
+
 .. image:: https://raw.githubusercontent.com/testflows/TestFlows-ArtWork/master/images/logo.png
    :width: 20%
    :target: https://testflows.com
    :alt: test bug
 
 ======================================================
 Autoscaling GitHub Actions Runners Using Hetzner Cloud
@@ -281,14 +298,49 @@
       Jul 24 14:24:42 user-node env[62771]: LANGUAGE=en_CA:en
       Jul 24 14:24:42 user-node env[62771]: PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/snap/bin
       Jul 24 14:24:42 user-node env[62771]: INVOCATION_ID=dc7b778f95fa4ccf95e4a4592b50d9e1
       Jul 24 14:24:42 user-node env[62771]: JOURNAL_STREAM=8:328542
       Jul 24 14:24:42 user-node env[62771]: SYSTEMD_EXEC_PID=62771
       ...
 
+-----------------------
+Deploying Application
+-----------------------
+
+You can deploy **github-runners** as a service to a new Hetzner Cloud server instance
+using the **deploy** command.
+
+:✋ Note:
+   The options that are passed to the **github-runners <options> deploy** command
+   will be the same options with which the service will be executed.
+
+.. code-block:: bash
+
+   export GITHUB_TOKEN=ghp_...
+   export GITHUB_REPOSITORY=testflows/github-runners
+   export HETZNER_TOKEN=GJzdc...
+   export HETZNER_SSH_KEY_NAME=user@user-node
+
+   github-runners deploy
+
+The **deploy** command will use the following default values:
+
+:location:
+   *ash*
+:type:
+   *cpx11*
+:image:
+   *ubuntu-20.04*
+
+You can customize deployment server location, type, and image using the *--location*, *--type*, and *--image* options.
+
+.. code-block:: bash
+
+   github-runners deploy --location nbg1 --type cx11 --image ubuntu-22.04
+
 
 ------------------
 Scaling Up Runners
 ------------------
 
 The program scale up runners by looking for any jobs that have **queued** status.
 For each such job, a corresponding Hetzner Cloud server instance is created with the following name:
@@ -539,14 +591,32 @@
 * **--debug**
   enable debugging mode, default: *False*
 
 * **commands:**
 
   * *command*
 
+    * **deploy**
+      deploy application
+
+      * **-n, --name**
+        deployment server name, default: *github-runners*
+
+      * **-f, --force**
+        force deployment if already exist
+
+      * **-l name, --location name**
+        deployment server location, default: *ash*
+
+      * **-t name, --type name**
+        deployment server type, default: *cpx11*
+
+      * **-i name, --image name**
+        deployment server image, default: *ubuntu-20.04*
+
     * **service**
       service commands
 
       * **install**
         install service
 
         * **-f, --force**
```

### Comparing `testflows.github.runners-1.1.230725.1002210/setup.py` & `testflows.github.runners-1.1.230725.1005626/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.1.230725.1002210",
+    version="1.1.230725.1005626",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.1.230725.1002210/testflows/github/runners/__init__.py` & `testflows.github.runners-1.1.230725.1005626/testflows/github/runners/__init__.py`

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
-__version__ = "1.1.230725.1002210"
+__version__ = "1.1.230725.1005626"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.1.230725.1002210/testflows/github/runners/actions.py` & `testflows.github.runners-1.1.230725.1005626/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1002210/testflows/github/runners/args.py` & `testflows.github.runners-1.1.230725.1005626/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1002210/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.1.230725.1005626/testflows/github/runners/bin/github-runners`

 * *Files 2% similar despite different names*

```diff
@@ -228,14 +228,47 @@
 
     deploy_parser = commands.add_parser(
         "deploy",
         help="deploy application",
         description="Deploy application as a service to a cloud instance.",
         formatter_class=RawTextHelpFormatter
     )
+    deploy_parser.add_argument(
+        "-n", "--name",
+        metavar="name",
+        type=str,
+        help="deployment server name, default: github-runners",
+        default="github-runners",
+    )
+    deploy_parser.add_argument(
+        "-f", "--force",
+        action="store_true",
+        help="force deployment if already exist",
+    )
+    deploy_parser.add_argument(
+        "-l", "--location",
+        metavar="name",
+        type=str,
+        help="deployment server location, default: ash",
+        default="ash",
+    )
+    deploy_parser.add_argument(
+        "-t", "--type",
+        metavar="name",
+        type=str,
+        help="deployment server type, default: cpx11",
+        default="cpx11",
+    )
+    deploy_parser.add_argument(
+        "-i", "--image",
+        metavar="name",
+        type=str,
+        help="deployment server image, default: ubuntu-20.04",
+        default="ubuntu-20.04",
+    )
     deploy_parser.set_defaults(func=deploy)
 
     service_parser = commands.add_parser(
         "service",
         help="service commands",
         description="Service commands.",
         formatter_class=RawTextHelpFormatter
```

### Comparing `testflows.github.runners-1.1.230725.1002210/testflows/github/runners/deploy.py` & `testflows.github.runners-1.1.230725.1005626/testflows/github/runners/deploy.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
-import time
 
 from hcloud import Client
 from hcloud.ssh_keys.domain import SSHKey
 from hcloud.server_types.domain import ServerType
 from hcloud.servers.client import BoundServer
 from hcloud.images.domain import Image
+from hcloud.locations.domain import Location
 
 from .actions import Action
 from .args import check
 from . import __version__
 
 from .server import wait_ready, wait_ssh, ssh
 
@@ -31,27 +31,36 @@
 
 
 def deploy(args, timeout=60):
     """Deploy github-runners as a service to a
     new Hetzner server instance."""
     check(args)
 
+    name = args.name
+
     with Action("Logging in to Hetzner Cloud"):
         client = Client(token=args.hetzner_token)
 
+    if args.force:
+        with Action(f"Checking if server {name} already exists", ignore_fail=True):
+            server: BoundServer = client.servers.get_by_name(name)
+            with Action(f"Deleting server {name}"):
+                server.delete()
+
     with Action(f"Creating new server"):
         response = client.servers.create(
-            name="github-runners",
-            server_type=ServerType("cpx11"),
-            image=Image("ubuntu-20.04"),
+            name=name,
+            server_type=ServerType(name=args.type),
+            image=Image(name=args.image),
+            location=Location(name=args.location),
             ssh_keys=[SSHKey(name=args.hetzner_ssh_key)],
         )
         server: BoundServer = response.server
 
-    with Action(f"Waiting for server {server.name} to be ready") as action:
+    with Action(f"Waiting for server to be ready") as action:
         wait_ready(server=server, timeout=timeout, action=action)
 
     with Action("Wait for SSH connection to be ready"):
         wait_ssh(server=server, timeout=timeout)
 
     with Action("Executing setup.sh script"):
         ssh(
```

### Comparing `testflows.github.runners-1.1.230725.1002210/testflows/github/runners/request.py` & `testflows.github.runners-1.1.230725.1005626/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.1.230725.1005626/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.1.230725.1005626/testflows/github/runners/scale_up.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.1.230725.1005626/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.1.230725.1005626/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.1.230725.1005626/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.1.230725.1005626/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1002210/testflows/github/runners/server.py` & `testflows.github.runners-1.1.230725.1005626/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1002210/testflows/github/runners/service.py` & `testflows.github.runners-1.1.230725.1005626/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1002210/testflows/github/runners/shell.py` & `testflows.github.runners-1.1.230725.1005626/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1002210/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.1.230725.1005626/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.1.230725.1002210
+Version: 1.1.230725.1005626
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -298,14 +298,49 @@
       Jul 24 14:24:42 user-node env[62771]: LANGUAGE=en_CA:en
       Jul 24 14:24:42 user-node env[62771]: PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/snap/bin
       Jul 24 14:24:42 user-node env[62771]: INVOCATION_ID=dc7b778f95fa4ccf95e4a4592b50d9e1
       Jul 24 14:24:42 user-node env[62771]: JOURNAL_STREAM=8:328542
       Jul 24 14:24:42 user-node env[62771]: SYSTEMD_EXEC_PID=62771
       ...
 
+-----------------------
+Deploying Application
+-----------------------
+
+You can deploy **github-runners** as a service to a new Hetzner Cloud server instance
+using the **deploy** command.
+
+:✋ Note:
+   The options that are passed to the **github-runners <options> deploy** command
+   will be the same options with which the service will be executed.
+
+.. code-block:: bash
+
+   export GITHUB_TOKEN=ghp_...
+   export GITHUB_REPOSITORY=testflows/github-runners
+   export HETZNER_TOKEN=GJzdc...
+   export HETZNER_SSH_KEY_NAME=user@user-node
+
+   github-runners deploy
+
+The **deploy** command will use the following default values:
+
+:location:
+   *ash*
+:type:
+   *cpx11*
+:image:
+   *ubuntu-20.04*
+
+You can customize deployment server location, type, and image using the *--location*, *--type*, and *--image* options.
+
+.. code-block:: bash
+
+   github-runners deploy --location nbg1 --type cx11 --image ubuntu-22.04
+
 
 ------------------
 Scaling Up Runners
 ------------------
 
 The program scale up runners by looking for any jobs that have **queued** status.
 For each such job, a corresponding Hetzner Cloud server instance is created with the following name:
@@ -556,14 +591,32 @@
 * **--debug**
   enable debugging mode, default: *False*
 
 * **commands:**
 
   * *command*
 
+    * **deploy**
+      deploy application
+
+      * **-n, --name**
+        deployment server name, default: *github-runners*
+
+      * **-f, --force**
+        force deployment if already exist
+
+      * **-l name, --location name**
+        deployment server location, default: *ash*
+
+      * **-t name, --type name**
+        deployment server type, default: *cpx11*
+
+      * **-i name, --image name**
+        deployment server image, default: *ubuntu-20.04*
+
     * **service**
       service commands
 
       * **install**
         install service
 
         * **-f, --force**
```

### Comparing `testflows.github.runners-1.1.230725.1002210/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.1.230725.1005626/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

