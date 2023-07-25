# Comparing `tmp/ros-cdk-ebs-1.0.17.tar.gz` & `tmp/ros-cdk-ebs-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-ebs-1.0.17.tar", last modified: Tue Jul 25 07:18:17 2023, max compression
+gzip compressed data, was "dist/ros-cdk-ebs-1.0.9.tar", last modified: Fri Sep 23 12:33:30 2022, max compression
```

## Comparing `ros-cdk-ebs-1.0.17.tar` & `ros-cdk-ebs-1.0.9.tar`

### file list

```diff
@@ -1,24 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 07:18:17.000000 ros-cdk-ebs-1.0.17/
--rw-r--r--   0 root         (0) root         (0)    10279 2023-07-25 07:18:17.000000 ros-cdk-ebs-1.0.17/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-25 07:18:17.000000 ros-cdk-ebs-1.0.17/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2023-07-25 07:18:17.000000 ros-cdk-ebs-1.0.17/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1292 2023-07-25 07:18:17.000000 ros-cdk-ebs-1.0.17/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2023-07-25 07:18:17.000000 ros-cdk-ebs-1.0.17/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-07-25 07:18:17.000000 ros-cdk-ebs-1.0.17/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 07:18:17.000000 ros-cdk-ebs-1.0.17/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1909 2023-07-25 07:18:17.000000 ros-cdk-ebs-1.0.17/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 07:18:17.000000 ros-cdk-ebs-1.0.17/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 07:18:17.000000 ros-cdk-ebs-1.0.17/src/ros_cdk_ebs/
--rw-r--r--   0 root         (0) root         (0)   134122 2023-07-25 07:18:17.000000 ros-cdk-ebs-1.0.17/src/ros_cdk_ebs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 07:18:17.000000 ros-cdk-ebs-1.0.17/src/ros_cdk_ebs/_jsii/
--rw-r--r--   0 root         (0) root         (0)      406 2023-07-25 07:18:17.000000 ros-cdk-ebs-1.0.17/src/ros_cdk_ebs/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    61710 2023-07-25 07:18:17.000000 ros-cdk-ebs-1.0.17/src/ros_cdk_ebs/_jsii/ros-cdk-ebs@1.0.17.jsii.tgz
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 07:18:17.000000 ros-cdk-ebs-1.0.17/src/ros_cdk_ebs/datasource/
--rw-r--r--   0 root         (0) root         (0)    29172 2023-07-25 07:18:17.000000 ros-cdk-ebs-1.0.17/src/ros_cdk_ebs/datasource/__init__.py
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 07:18:17.000000 ros-cdk-ebs-1.0.17/src/ros_cdk_ebs/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 07:18:17.000000 ros-cdk-ebs-1.0.17/src/ros_cdk_ebs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1292 2023-07-25 07:18:17.000000 ros-cdk-ebs-1.0.17/src/ros_cdk_ebs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2023-07-25 07:18:17.000000 ros-cdk-ebs-1.0.17/src/ros_cdk_ebs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 07:18:17.000000 ros-cdk-ebs-1.0.17/src/ros_cdk_ebs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-07-25 07:18:17.000000 ros-cdk-ebs-1.0.17/src/ros_cdk_ebs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-25 07:18:17.000000 ros-cdk-ebs-1.0.17/src/ros_cdk_ebs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:33:30.000000 ros-cdk-ebs-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 12:33:30.000000 ros-cdk-ebs-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 12:33:30.000000 ros-cdk-ebs-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 12:33:30.000000 ros-cdk-ebs-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 12:33:30.000000 ros-cdk-ebs-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 12:33:30.000000 ros-cdk-ebs-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 12:33:30.000000 ros-cdk-ebs-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 12:33:30.000000 ros-cdk-ebs-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 12:33:30.000000 ros-cdk-ebs-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:33:30.000000 ros-cdk-ebs-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:33:30.000000 ros-cdk-ebs-1.0.9/src/ros_cdk_ebs/
+-rw-r--r--   0 root         (0) root         (0)    13641 2022-09-23 12:33:30.000000 ros-cdk-ebs-1.0.9/src/ros_cdk_ebs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:33:30.000000 ros-cdk-ebs-1.0.9/src/ros_cdk_ebs/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 12:33:30.000000 ros-cdk-ebs-1.0.9/src/ros_cdk_ebs/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28904 2022-09-23 12:33:30.000000 ros-cdk-ebs-1.0.9/src/ros_cdk_ebs/_jsii/ros-cdk-ebs@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:33:30.000000 ros-cdk-ebs-1.0.9/src/ros_cdk_ebs/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:33:30.000000 ros-cdk-ebs-1.0.9/src/ros_cdk_ebs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 12:33:30.000000 ros-cdk-ebs-1.0.9/src/ros_cdk_ebs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 12:33:30.000000 ros-cdk-ebs-1.0.9/src/ros_cdk_ebs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:33:30.000000 ros-cdk-ebs-1.0.9/src/ros_cdk_ebs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 12:33:30.000000 ros-cdk-ebs-1.0.9/src/ros_cdk_ebs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 12:33:30.000000 ros-cdk-ebs-1.0.9/src/ros_cdk_ebs.egg-info/top_level.txt
```

### Comparing `ros-cdk-ebs-1.0.17/LICENSE` & `ros-cdk-ebs-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-ebs-1.0.17/PKG-INFO` & `ros-cdk-ebs-1.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-ebs
-Version: 1.0.17
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS EBS Construct Library
         
@@ -19,13 +19,12 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ros-cdk-ebs-1.0.17/setup.py` & `ros-cdk-ebs-1.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-ebs",
-    "version": "1.0.17",
+    "version": "1.0.9",
     "description": "Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com",
     "license": "Apache-2.0",
     "url": "https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git",
     "long_description_content_type": "text/markdown",
     "author": "ROS Development Team",
     "bdist_wheel": {
         "universal": true
@@ -18,43 +18,41 @@
         "Source": "https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git"
     },
     "package_dir": {
         "": "src"
     },
     "packages": [
         "ros_cdk_ebs",
-        "ros_cdk_ebs._jsii",
-        "ros_cdk_ebs.datasource"
+        "ros_cdk_ebs._jsii"
     ],
     "package_data": {
         "ros_cdk_ebs._jsii": [
-            "ros-cdk-ebs@1.0.17.jsii.tgz"
+            "ros-cdk-ebs@1.0.9.jsii.tgz"
         ],
         "ros_cdk_ebs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "constructs>=3.0.4, <4.0.0",
-        "jsii>=1.85.0, <2.0.0",
+        "jsii>=1.68.0, <2.0.0",
         "publication>=0.0.3",
         "ros-cdk-core>=1.0.6, <2.0.0",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "License :: OSI Approved",
         "Programming Language :: Python :: 3"
     ],
     "scripts": []
 }
 """
```

### Comparing `ros-cdk-ebs-1.0.17/src/ros_cdk_ebs.egg-info/PKG-INFO` & `ros-cdk-ebs-1.0.9/src/ros_cdk_ebs.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-ebs
-Version: 1.0.17
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS EBS Construct Library
         
@@ -19,13 +19,12 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
```

