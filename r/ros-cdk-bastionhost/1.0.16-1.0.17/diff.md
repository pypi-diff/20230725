# Comparing `tmp/ros-cdk-bastionhost-1.0.16.tar.gz` & `tmp/ros-cdk-bastionhost-1.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-bastionhost-1.0.16.tar", last modified: Wed Jul 19 02:05:15 2023, max compression
+gzip compressed data, was "dist/ros-cdk-bastionhost-1.0.17.tar", last modified: Tue Jul 25 08:05:17 2023, max compression
```

## Comparing `ros-cdk-bastionhost-1.0.16.tar` & `ros-cdk-bastionhost-1.0.17.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:05:15.000000 ros-cdk-bastionhost-1.0.16/
--rw-r--r--   0 root         (0) root         (0)    10279 2023-07-19 02:05:15.000000 ros-cdk-bastionhost-1.0.16/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-19 02:05:15.000000 ros-cdk-bastionhost-1.0.16/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2023-07-19 02:05:15.000000 ros-cdk-bastionhost-1.0.16/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1324 2023-07-19 02:05:15.000000 ros-cdk-bastionhost-1.0.16/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      203 2023-07-19 02:05:15.000000 ros-cdk-bastionhost-1.0.16/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-07-19 02:05:15.000000 ros-cdk-bastionhost-1.0.16/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-19 02:05:15.000000 ros-cdk-bastionhost-1.0.16/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1923 2023-07-19 02:05:15.000000 ros-cdk-bastionhost-1.0.16/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:05:15.000000 ros-cdk-bastionhost-1.0.16/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:05:15.000000 ros-cdk-bastionhost-1.0.16/src/ros_cdk_bastionhost/
--rw-r--r--   0 root         (0) root         (0)    43509 2023-07-19 02:05:15.000000 ros-cdk-bastionhost-1.0.16/src/ros_cdk_bastionhost/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:05:15.000000 ros-cdk-bastionhost-1.0.16/src/ros_cdk_bastionhost/_jsii/
--rw-r--r--   0 root         (0) root         (0)      435 2023-07-19 02:05:15.000000 ros-cdk-bastionhost-1.0.16/src/ros_cdk_bastionhost/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34036 2023-07-19 02:05:15.000000 ros-cdk-bastionhost-1.0.16/src/ros_cdk_bastionhost/_jsii/ros-cdk-bastionhost@1.0.16.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 02:05:15.000000 ros-cdk-bastionhost-1.0.16/src/ros_cdk_bastionhost/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:05:15.000000 ros-cdk-bastionhost-1.0.16/src/ros_cdk_bastionhost.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1324 2023-07-19 02:05:15.000000 ros-cdk-bastionhost-1.0.16/src/ros_cdk_bastionhost.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      481 2023-07-19 02:05:15.000000 ros-cdk-bastionhost-1.0.16/src/ros_cdk_bastionhost.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 02:05:15.000000 ros-cdk-bastionhost-1.0.16/src/ros_cdk_bastionhost.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-07-19 02:05:15.000000 ros-cdk-bastionhost-1.0.16/src/ros_cdk_bastionhost.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-19 02:05:15.000000 ros-cdk-bastionhost-1.0.16/src/ros_cdk_bastionhost.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:05:17.000000 ros-cdk-bastionhost-1.0.17/
+-rw-r--r--   0 root         (0) root         (0)    10279 2023-07-25 08:05:17.000000 ros-cdk-bastionhost-1.0.17/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-25 08:05:17.000000 ros-cdk-bastionhost-1.0.17/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2023-07-25 08:05:17.000000 ros-cdk-bastionhost-1.0.17/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1324 2023-07-25 08:05:17.000000 ros-cdk-bastionhost-1.0.17/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      203 2023-07-25 08:05:17.000000 ros-cdk-bastionhost-1.0.17/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-07-25 08:05:17.000000 ros-cdk-bastionhost-1.0.17/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 08:05:17.000000 ros-cdk-bastionhost-1.0.17/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1923 2023-07-25 08:05:17.000000 ros-cdk-bastionhost-1.0.17/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:05:17.000000 ros-cdk-bastionhost-1.0.17/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:05:17.000000 ros-cdk-bastionhost-1.0.17/src/ros_cdk_bastionhost/
+-rw-r--r--   0 root         (0) root         (0)    43509 2023-07-25 08:05:17.000000 ros-cdk-bastionhost-1.0.17/src/ros_cdk_bastionhost/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:05:17.000000 ros-cdk-bastionhost-1.0.17/src/ros_cdk_bastionhost/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      435 2023-07-25 08:05:17.000000 ros-cdk-bastionhost-1.0.17/src/ros_cdk_bastionhost/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34037 2023-07-25 08:05:17.000000 ros-cdk-bastionhost-1.0.17/src/ros_cdk_bastionhost/_jsii/ros-cdk-bastionhost@1.0.17.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 08:05:17.000000 ros-cdk-bastionhost-1.0.17/src/ros_cdk_bastionhost/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:05:17.000000 ros-cdk-bastionhost-1.0.17/src/ros_cdk_bastionhost.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1324 2023-07-25 08:05:17.000000 ros-cdk-bastionhost-1.0.17/src/ros_cdk_bastionhost.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      481 2023-07-25 08:05:17.000000 ros-cdk-bastionhost-1.0.17/src/ros_cdk_bastionhost.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 08:05:17.000000 ros-cdk-bastionhost-1.0.17/src/ros_cdk_bastionhost.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-07-25 08:05:17.000000 ros-cdk-bastionhost-1.0.17/src/ros_cdk_bastionhost.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-25 08:05:17.000000 ros-cdk-bastionhost-1.0.17/src/ros_cdk_bastionhost.egg-info/top_level.txt
```

### Comparing `ros-cdk-bastionhost-1.0.16/LICENSE` & `ros-cdk-bastionhost-1.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-bastionhost-1.0.16/PKG-INFO` & `ros-cdk-bastionhost-1.0.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-bastionhost
-Version: 1.0.16
+Version: 1.0.17
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS BASTIONHOST Construct Library
```

### Comparing `ros-cdk-bastionhost-1.0.16/setup.py` & `ros-cdk-bastionhost-1.0.17/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-bastionhost",
-    "version": "1.0.16",
+    "version": "1.0.17",
     "description": "Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com",
     "license": "Apache-2.0",
     "url": "https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git",
     "long_description_content_type": "text/markdown",
     "author": "ROS Development Team",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "ros_cdk_bastionhost",
         "ros_cdk_bastionhost._jsii"
     ],
     "package_data": {
         "ros_cdk_bastionhost._jsii": [
-            "ros-cdk-bastionhost@1.0.16.jsii.tgz"
+            "ros-cdk-bastionhost@1.0.17.jsii.tgz"
         ],
         "ros_cdk_bastionhost": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `ros-cdk-bastionhost-1.0.16/src/ros_cdk_bastionhost/__init__.py` & `ros-cdk-bastionhost-1.0.17/src/ros_cdk_bastionhost/__init__.py`

 * *Files identical despite different names*

### Comparing `ros-cdk-bastionhost-1.0.16/src/ros_cdk_bastionhost.egg-info/PKG-INFO` & `ros-cdk-bastionhost-1.0.17/src/ros_cdk_bastionhost.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-bastionhost
-Version: 1.0.16
+Version: 1.0.17
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS BASTIONHOST Construct Library
```

