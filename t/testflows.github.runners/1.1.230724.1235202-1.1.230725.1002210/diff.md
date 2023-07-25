# Comparing `tmp/testflows.github.runners-1.1.230724.1235202.tar.gz` & `tmp/testflows.github.runners-1.1.230725.1002210.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.1.230724.1235202.tar", last modified: Mon Jul 24 23:52:02 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.1.230725.1002210.tar", last modified: Tue Jul 25 00:22:10 2023, max compression
```

## Comparing `testflows.github.runners-1.1.230724.1235202.tar` & `testflows.github.runners-1.1.230725.1002210.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 23:52:02.319094 testflows.github.runners-1.1.230724.1235202/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.1.230724.1235202/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    21124 2023-07-24 23:52:02.319094 testflows.github.runners-1.1.230724.1235202/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    20532 2023-07-24 22:41:19.000000 testflows.github.runners-1.1.230724.1235202/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-24 23:52:02.319094 testflows.github.runners-1.1.230724.1235202/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-24 23:52:02.000000 testflows.github.runners-1.1.230724.1235202/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 23:52:02.315094 testflows.github.runners-1.1.230724.1235202/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 23:52:02.315094 testflows.github.runners-1.1.230724.1235202/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 23:52:02.319094 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-24 23:52:02.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      979 2023-07-24 20:59:02.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1173 2023-07-24 19:41:30.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 23:52:02.319094 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    12980 2023-07-24 22:29:17.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)     3759 2023-07-24 23:51:42.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/deploy.py
--rw-rw-r--   0 user      (1000) user      (1000)     1266 2023-07-24 15:25:53.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     8365 2023-07-24 14:06:05.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)     7972 2023-07-24 23:49:06.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 23:52:02.319094 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 23:52:02.319094 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      266 2023-07-24 22:16:12.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-24 22:14:55.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-24 01:28:32.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      714 2023-07-24 01:27:59.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     4443 2023-07-24 22:01:20.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1392 2023-07-24 23:28:45.000000 testflows.github.runners-1.1.230724.1235202/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-24 23:52:02.319094 testflows.github.runners-1.1.230724.1235202/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    21124 2023-07-24 23:52:02.000000 testflows.github.runners-1.1.230724.1235202/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1001 2023-07-24 23:52:02.000000 testflows.github.runners-1.1.230724.1235202/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 23:52:02.000000 testflows.github.runners-1.1.230724.1235202/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.1.230724.1235202/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-24 23:52:02.000000 testflows.github.runners-1.1.230724.1235202/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-24 23:52:02.000000 testflows.github.runners-1.1.230724.1235202/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 00:22:10.480706 testflows.github.runners-1.1.230725.1002210/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.1.230725.1002210/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    21124 2023-07-25 00:22:10.476706 testflows.github.runners-1.1.230725.1002210/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    20532 2023-07-24 22:41:19.000000 testflows.github.runners-1.1.230725.1002210/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-25 00:22:10.480706 testflows.github.runners-1.1.230725.1002210/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-25 00:22:10.000000 testflows.github.runners-1.1.230725.1002210/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 00:22:10.476706 testflows.github.runners-1.1.230725.1002210/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 00:22:10.476706 testflows.github.runners-1.1.230725.1002210/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 00:22:10.476706 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-25 00:22:10.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1173 2023-07-24 19:41:30.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 00:22:10.476706 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    13212 2023-07-25 00:21:34.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)     3759 2023-07-25 00:21:48.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/deploy.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1266 2023-07-24 15:25:53.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8365 2023-07-24 14:06:05.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7972 2023-07-24 23:49:06.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 00:22:10.476706 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 00:22:10.476706 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      266 2023-07-24 22:16:12.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-24 22:14:55.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-24 01:28:32.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      714 2023-07-24 01:27:59.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4443 2023-07-24 22:01:20.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1392 2023-07-24 23:28:45.000000 testflows.github.runners-1.1.230725.1002210/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 00:22:10.476706 testflows.github.runners-1.1.230725.1002210/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    21124 2023-07-25 00:22:10.000000 testflows.github.runners-1.1.230725.1002210/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1001 2023-07-25 00:22:10.000000 testflows.github.runners-1.1.230725.1002210/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-25 00:22:10.000000 testflows.github.runners-1.1.230725.1002210/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.1.230725.1002210/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-25 00:22:10.000000 testflows.github.runners-1.1.230725.1002210/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-25 00:22:10.000000 testflows.github.runners-1.1.230725.1002210/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.1.230724.1235202/LICENSE` & `testflows.github.runners-1.1.230725.1002210/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1235202/PKG-INFO` & `testflows.github.runners-1.1.230725.1002210/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.1.230724.1235202
+Version: 1.1.230725.1002210
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.1.230724.1235202/README.rst` & `testflows.github.runners-1.1.230725.1002210/README.rst`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1235202/setup.py` & `testflows.github.runners-1.1.230725.1002210/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.1.230724.1235202",
+    version="1.1.230725.1002210",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.1.230724.1235202/testflows/github/runners/__init__.py` & `testflows.github.runners-1.1.230725.1002210/testflows/github/runners/__init__.py`

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
-__version__ = "1.1.230724.1235202"
+__version__ = "1.1.230725.1002210"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.1.230724.1235202/testflows/github/runners/actions.py` & `testflows.github.runners-1.1.230725.1002210/testflows/github/runners/actions.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         return self
 
     def note(self, message):
         logger.log(msg=f"   {message}", stacklevel=2, level=self.level)
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
         if exc_value is not None:
-            msg = f"❌ Error: {exc_value}"
+            msg = f"❌ Error: {exc_type.__name__} {exc_value}"
             if not self.debug:
                 logger.log(msg=msg, stacklevel=2, level=logging.ERROR)
             else:
                 logger.exception(msg=msg, stacklevel=3)
             if self.ignore_fail:
                 return True
             raise
```

### Comparing `testflows.github.runners-1.1.230724.1235202/testflows/github/runners/args.py` & `testflows.github.runners-1.1.230725.1002210/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1235202/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.1.230725.1002210/testflows/github/runners/bin/github-runners`

 * *Files 2% similar despite different names*

```diff
@@ -404,15 +404,15 @@
 
     if args.logger_config:
         logging.config.fileConfig(args.logger_config)
     else:
         logger.setLevel(logging_level)
         handler = logging.StreamHandler(sys.stdout)
         formatter = logging.Formatter(
-            "%(asctime)s %(levelname)6s %(threadName)10s %(funcName)15s %(message)s",
+            "%(asctime)s %(levelname)8s %(threadName)10s %(funcName)15s %(message)s",
             datefmt="%m/%d/%Y %I:%M:%S %p",
         )
         handler.setFormatter(formatter)
         logger.addHandler(handler)
 
     if args.setup_script:
         scripts.setup = args.setup_script
@@ -420,15 +420,23 @@
     if args.startup_x64_script:
         scripts.startup_x64 = args.startup_x64_script
 
     if args.startup_arm64_script:
         scripts.startup_arm64 = args.startup_arm64_script
 
     if hasattr(args, "func"):
-        args.func(args=args)
+        try:
+            args.func(args=args)
+        except KeyboardInterrupt:
+            if args.debug:
+                raise
+        except BaseException as exc:
+            if args.debug:
+                raise
+            logger.fatal(f"❗ Error: {exc}")
 
     else:
         check(args)
 
         with ThreadPoolExecutor(
             max_workers=args.workers + 2, thread_name_prefix="worker"
         ) as worker_pool:
```

### Comparing `testflows.github.runners-1.1.230724.1235202/testflows/github/runners/deploy.py` & `testflows.github.runners-1.1.230725.1002210/testflows/github/runners/deploy.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1235202/testflows/github/runners/request.py` & `testflows.github.runners-1.1.230725.1002210/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scale_up.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1235202/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.1.230725.1002210/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1235202/testflows/github/runners/server.py` & `testflows.github.runners-1.1.230725.1002210/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1235202/testflows/github/runners/service.py` & `testflows.github.runners-1.1.230725.1002210/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1235202/testflows/github/runners/shell.py` & `testflows.github.runners-1.1.230725.1002210/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230724.1235202/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.1.230725.1002210/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.1.230724.1235202
+Version: 1.1.230725.1002210
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.1.230724.1235202/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.1.230725.1002210/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

