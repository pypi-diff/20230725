# Comparing `tmp/ros-cdk-directmail-1.0.16.tar.gz` & `tmp/ros-cdk-directmail-1.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-directmail-1.0.16.tar", last modified: Wed Jul 19 02:43:28 2023, max compression
+gzip compressed data, was "dist/ros-cdk-directmail-1.0.17.tar", last modified: Tue Jul 25 07:55:49 2023, max compression
```

## Comparing `ros-cdk-directmail-1.0.16.tar` & `ros-cdk-directmail-1.0.17.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:43:28.000000 ros-cdk-directmail-1.0.16/
--rw-r--r--   0 root         (0) root         (0)    10279 2023-07-19 02:43:28.000000 ros-cdk-directmail-1.0.16/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-19 02:43:28.000000 ros-cdk-directmail-1.0.16/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2023-07-19 02:43:28.000000 ros-cdk-directmail-1.0.16/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1320 2023-07-19 02:43:28.000000 ros-cdk-directmail-1.0.16/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      200 2023-07-19 02:43:28.000000 ros-cdk-directmail-1.0.16/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-07-19 02:43:28.000000 ros-cdk-directmail-1.0.16/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-19 02:43:28.000000 ros-cdk-directmail-1.0.16/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1917 2023-07-19 02:43:28.000000 ros-cdk-directmail-1.0.16/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:43:28.000000 ros-cdk-directmail-1.0.16/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:43:28.000000 ros-cdk-directmail-1.0.16/src/ros_cdk_directmail/
--rw-r--r--   0 root         (0) root         (0)    34716 2023-07-19 02:43:28.000000 ros-cdk-directmail-1.0.16/src/ros_cdk_directmail/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:43:28.000000 ros-cdk-directmail-1.0.16/src/ros_cdk_directmail/_jsii/
--rw-r--r--   0 root         (0) root         (0)      433 2023-07-19 02:43:28.000000 ros-cdk-directmail-1.0.16/src/ros_cdk_directmail/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37772 2023-07-19 02:43:28.000000 ros-cdk-directmail-1.0.16/src/ros_cdk_directmail/_jsii/ros-cdk-directmail@1.0.16.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 02:43:28.000000 ros-cdk-directmail-1.0.16/src/ros_cdk_directmail/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:43:28.000000 ros-cdk-directmail-1.0.16/src/ros_cdk_directmail.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1320 2023-07-19 02:43:28.000000 ros-cdk-directmail-1.0.16/src/ros_cdk_directmail.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      471 2023-07-19 02:43:28.000000 ros-cdk-directmail-1.0.16/src/ros_cdk_directmail.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 02:43:28.000000 ros-cdk-directmail-1.0.16/src/ros_cdk_directmail.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-07-19 02:43:28.000000 ros-cdk-directmail-1.0.16/src/ros_cdk_directmail.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-19 02:43:28.000000 ros-cdk-directmail-1.0.16/src/ros_cdk_directmail.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 07:55:49.000000 ros-cdk-directmail-1.0.17/
+-rw-r--r--   0 root         (0) root         (0)    10279 2023-07-25 07:55:49.000000 ros-cdk-directmail-1.0.17/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-25 07:55:49.000000 ros-cdk-directmail-1.0.17/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2023-07-25 07:55:49.000000 ros-cdk-directmail-1.0.17/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-07-25 07:55:49.000000 ros-cdk-directmail-1.0.17/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      200 2023-07-25 07:55:49.000000 ros-cdk-directmail-1.0.17/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-07-25 07:55:49.000000 ros-cdk-directmail-1.0.17/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 07:55:49.000000 ros-cdk-directmail-1.0.17/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1958 2023-07-25 07:55:49.000000 ros-cdk-directmail-1.0.17/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 07:55:49.000000 ros-cdk-directmail-1.0.17/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 07:55:49.000000 ros-cdk-directmail-1.0.17/src/ros_cdk_directmail/
+-rw-r--r--   0 root         (0) root         (0)    34845 2023-07-25 07:55:49.000000 ros-cdk-directmail-1.0.17/src/ros_cdk_directmail/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 07:55:49.000000 ros-cdk-directmail-1.0.17/src/ros_cdk_directmail/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      433 2023-07-25 07:55:49.000000 ros-cdk-directmail-1.0.17/src/ros_cdk_directmail/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38322 2023-07-25 07:55:49.000000 ros-cdk-directmail-1.0.17/src/ros_cdk_directmail/_jsii/ros-cdk-directmail@1.0.17.jsii.tgz
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 07:55:49.000000 ros-cdk-directmail-1.0.17/src/ros_cdk_directmail/datasource/
+-rw-r--r--   0 root         (0) root         (0)    17827 2023-07-25 07:55:49.000000 ros-cdk-directmail-1.0.17/src/ros_cdk_directmail/datasource/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 07:55:49.000000 ros-cdk-directmail-1.0.17/src/ros_cdk_directmail/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 07:55:49.000000 ros-cdk-directmail-1.0.17/src/ros_cdk_directmail.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-07-25 07:55:49.000000 ros-cdk-directmail-1.0.17/src/ros_cdk_directmail.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      517 2023-07-25 07:55:49.000000 ros-cdk-directmail-1.0.17/src/ros_cdk_directmail.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 07:55:49.000000 ros-cdk-directmail-1.0.17/src/ros_cdk_directmail.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-07-25 07:55:49.000000 ros-cdk-directmail-1.0.17/src/ros_cdk_directmail.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-25 07:55:49.000000 ros-cdk-directmail-1.0.17/src/ros_cdk_directmail.egg-info/top_level.txt
```

### Comparing `ros-cdk-directmail-1.0.16/LICENSE` & `ros-cdk-directmail-1.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-directmail-1.0.16/PKG-INFO` & `ros-cdk-directmail-1.0.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-directmail
-Version: 1.0.16
+Version: 1.0.17
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS DIRECTMAIL Construct Library
```

### Comparing `ros-cdk-directmail-1.0.16/setup.py` & `ros-cdk-directmail-1.0.17/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-directmail",
-    "version": "1.0.16",
+    "version": "1.0.17",
     "description": "Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com",
     "license": "Apache-2.0",
     "url": "https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git",
     "long_description_content_type": "text/markdown",
     "author": "ROS Development Team",
     "bdist_wheel": {
         "universal": true
@@ -18,19 +18,20 @@
         "Source": "https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git"
     },
     "package_dir": {
         "": "src"
     },
     "packages": [
         "ros_cdk_directmail",
-        "ros_cdk_directmail._jsii"
+        "ros_cdk_directmail._jsii",
+        "ros_cdk_directmail.datasource"
     ],
     "package_data": {
         "ros_cdk_directmail._jsii": [
-            "ros-cdk-directmail@1.0.16.jsii.tgz"
+            "ros-cdk-directmail@1.0.17.jsii.tgz"
         ],
         "ros_cdk_directmail": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `ros-cdk-directmail-1.0.16/src/ros_cdk_directmail/__init__.py` & `ros-cdk-directmail-1.0.17/src/ros_cdk_directmail/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -739,18 +739,22 @@
     "DomainProps",
     "Ipfilter",
     "IpfilterProps",
     "RosDomain",
     "RosDomainProps",
     "RosIpfilter",
     "RosIpfilterProps",
+    "datasource",
 ]
 
 publication.publish()
 
+# Loading modules to ensure their types are registered with the jsii runtime library
+from . import datasource
+
 def _typecheckingstub__07e5535889367ac5fbb0bf92c6ee0efd0891e4db565c682913ac3810dd49c5aa(
     scope: _ros_cdk_core_7adfd82f.Construct,
     id: builtins.str,
     props: typing.Union[DomainProps, typing.Dict[builtins.str, typing.Any]],
     enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
```

### Comparing `ros-cdk-directmail-1.0.16/src/ros_cdk_directmail.egg-info/PKG-INFO` & `ros-cdk-directmail-1.0.17/src/ros_cdk_directmail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-directmail
-Version: 1.0.16
+Version: 1.0.17
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS DIRECTMAIL Construct Library
```

