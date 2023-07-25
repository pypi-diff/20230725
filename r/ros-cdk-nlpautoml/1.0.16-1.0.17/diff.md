# Comparing `tmp/ros-cdk-nlpautoml-1.0.16.tar.gz` & `tmp/ros-cdk-nlpautoml-1.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-nlpautoml-1.0.16.tar", last modified: Wed Jul 19 02:02:37 2023, max compression
+gzip compressed data, was "dist/ros-cdk-nlpautoml-1.0.17.tar", last modified: Tue Jul 25 07:14:57 2023, max compression
```

## Comparing `ros-cdk-nlpautoml-1.0.16.tar` & `ros-cdk-nlpautoml-1.0.17.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:02:37.000000 ros-cdk-nlpautoml-1.0.16/
--rw-r--r--   0 root         (0) root         (0)    10279 2023-07-19 02:02:36.000000 ros-cdk-nlpautoml-1.0.16/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-19 02:02:36.000000 ros-cdk-nlpautoml-1.0.16/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2023-07-19 02:02:36.000000 ros-cdk-nlpautoml-1.0.16/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1316 2023-07-19 02:02:37.000000 ros-cdk-nlpautoml-1.0.16/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      197 2023-07-19 02:02:36.000000 ros-cdk-nlpautoml-1.0.16/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-07-19 02:02:36.000000 ros-cdk-nlpautoml-1.0.16/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-19 02:02:37.000000 ros-cdk-nlpautoml-1.0.16/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1911 2023-07-19 02:02:36.000000 ros-cdk-nlpautoml-1.0.16/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:02:37.000000 ros-cdk-nlpautoml-1.0.16/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:02:37.000000 ros-cdk-nlpautoml-1.0.16/src/ros_cdk_nlpautoml/
--rw-r--r--   0 root         (0) root         (0)    69727 2023-07-19 02:02:36.000000 ros-cdk-nlpautoml-1.0.16/src/ros_cdk_nlpautoml/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:02:37.000000 ros-cdk-nlpautoml-1.0.16/src/ros_cdk_nlpautoml/_jsii/
--rw-r--r--   0 root         (0) root         (0)      431 2023-07-19 02:02:36.000000 ros-cdk-nlpautoml-1.0.16/src/ros_cdk_nlpautoml/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41604 2023-07-19 02:02:36.000000 ros-cdk-nlpautoml-1.0.16/src/ros_cdk_nlpautoml/_jsii/ros-cdk-nlpautoml@1.0.16.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 02:02:36.000000 ros-cdk-nlpautoml-1.0.16/src/ros_cdk_nlpautoml/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:02:37.000000 ros-cdk-nlpautoml-1.0.16/src/ros_cdk_nlpautoml.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1316 2023-07-19 02:02:37.000000 ros-cdk-nlpautoml-1.0.16/src/ros_cdk_nlpautoml.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      461 2023-07-19 02:02:37.000000 ros-cdk-nlpautoml-1.0.16/src/ros_cdk_nlpautoml.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 02:02:37.000000 ros-cdk-nlpautoml-1.0.16/src/ros_cdk_nlpautoml.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-07-19 02:02:37.000000 ros-cdk-nlpautoml-1.0.16/src/ros_cdk_nlpautoml.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-19 02:02:37.000000 ros-cdk-nlpautoml-1.0.16/src/ros_cdk_nlpautoml.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 07:14:57.000000 ros-cdk-nlpautoml-1.0.17/
+-rw-r--r--   0 root         (0) root         (0)    10279 2023-07-25 07:14:56.000000 ros-cdk-nlpautoml-1.0.17/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-25 07:14:56.000000 ros-cdk-nlpautoml-1.0.17/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2023-07-25 07:14:56.000000 ros-cdk-nlpautoml-1.0.17/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1316 2023-07-25 07:14:57.000000 ros-cdk-nlpautoml-1.0.17/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      197 2023-07-25 07:14:56.000000 ros-cdk-nlpautoml-1.0.17/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-07-25 07:14:56.000000 ros-cdk-nlpautoml-1.0.17/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 07:14:57.000000 ros-cdk-nlpautoml-1.0.17/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1911 2023-07-25 07:14:56.000000 ros-cdk-nlpautoml-1.0.17/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 07:14:57.000000 ros-cdk-nlpautoml-1.0.17/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 07:14:57.000000 ros-cdk-nlpautoml-1.0.17/src/ros_cdk_nlpautoml/
+-rw-r--r--   0 root         (0) root         (0)    69727 2023-07-25 07:14:56.000000 ros-cdk-nlpautoml-1.0.17/src/ros_cdk_nlpautoml/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 07:14:57.000000 ros-cdk-nlpautoml-1.0.17/src/ros_cdk_nlpautoml/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      431 2023-07-25 07:14:56.000000 ros-cdk-nlpautoml-1.0.17/src/ros_cdk_nlpautoml/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41604 2023-07-25 07:14:56.000000 ros-cdk-nlpautoml-1.0.17/src/ros_cdk_nlpautoml/_jsii/ros-cdk-nlpautoml@1.0.17.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 07:14:56.000000 ros-cdk-nlpautoml-1.0.17/src/ros_cdk_nlpautoml/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 07:14:57.000000 ros-cdk-nlpautoml-1.0.17/src/ros_cdk_nlpautoml.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1316 2023-07-25 07:14:56.000000 ros-cdk-nlpautoml-1.0.17/src/ros_cdk_nlpautoml.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      461 2023-07-25 07:14:57.000000 ros-cdk-nlpautoml-1.0.17/src/ros_cdk_nlpautoml.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 07:14:56.000000 ros-cdk-nlpautoml-1.0.17/src/ros_cdk_nlpautoml.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-07-25 07:14:56.000000 ros-cdk-nlpautoml-1.0.17/src/ros_cdk_nlpautoml.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-25 07:14:56.000000 ros-cdk-nlpautoml-1.0.17/src/ros_cdk_nlpautoml.egg-info/top_level.txt
```

### Comparing `ros-cdk-nlpautoml-1.0.16/LICENSE` & `ros-cdk-nlpautoml-1.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-nlpautoml-1.0.16/PKG-INFO` & `ros-cdk-nlpautoml-1.0.17/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-nlpautoml
-Version: 1.0.16
+Version: 1.0.17
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS NLPAUTOML Construct Library
```

### Comparing `ros-cdk-nlpautoml-1.0.16/setup.py` & `ros-cdk-nlpautoml-1.0.17/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-nlpautoml",
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
         "ros_cdk_nlpautoml",
         "ros_cdk_nlpautoml._jsii"
     ],
     "package_data": {
         "ros_cdk_nlpautoml._jsii": [
-            "ros-cdk-nlpautoml@1.0.16.jsii.tgz"
+            "ros-cdk-nlpautoml@1.0.17.jsii.tgz"
         ],
         "ros_cdk_nlpautoml": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `ros-cdk-nlpautoml-1.0.16/src/ros_cdk_nlpautoml/__init__.py` & `ros-cdk-nlpautoml-1.0.17/src/ros_cdk_nlpautoml/__init__.py`

 * *Files identical despite different names*

### Comparing `ros-cdk-nlpautoml-1.0.16/src/ros_cdk_nlpautoml.egg-info/PKG-INFO` & `ros-cdk-nlpautoml-1.0.17/src/ros_cdk_nlpautoml.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-nlpautoml
-Version: 1.0.16
+Version: 1.0.17
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS NLPAUTOML Construct Library
```

