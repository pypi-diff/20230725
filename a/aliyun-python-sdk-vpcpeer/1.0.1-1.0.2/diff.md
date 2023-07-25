# Comparing `tmp/aliyun-python-sdk-vpcpeer-1.0.1.tar.gz` & `tmp/aliyun-python-sdk-vpcpeer-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-vpcpeer-1.0.1.tar", last modified: Tue May 30 07:59:54 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-vpcpeer-1.0.2.tar", last modified: Tue Jul 25 09:37:38 2023, max compression
```

## Comparing `aliyun-python-sdk-vpcpeer-1.0.1.tar` & `aliyun-python-sdk-vpcpeer-1.0.2.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 07:59:54.000000 aliyun-python-sdk-vpcpeer-1.0.1/
--rw-r--r--   0 root         (0) root         (0)      575 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1557 2023-05-30 07:59:54.000000 aliyun-python-sdk-vpcpeer-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      535 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 07:59:54.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyun_python_sdk_vpcpeer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1557 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyun_python_sdk_vpcpeer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1103 2023-05-30 07:59:54.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyun_python_sdk_vpcpeer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyun_python_sdk_vpcpeer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyun_python_sdk_vpcpeer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyun_python_sdk_vpcpeer.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 07:59:54.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1087 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 07:59:54.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 07:59:54.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/
--rw-r--r--   0 root         (0) root         (0)     2324 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/AcceptVpcPeerConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     3056 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/CreateVpcPeerConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2016 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/DeleteVpcPeerConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1752 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/GetVpcPeerConnectionAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2556 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/ListTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2891 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/ListVpcPeerConnectionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2390 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/ModifyVpcPeerConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2104 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/RejectVpcPeerConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2367 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/TagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2345 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/UnTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-05-30 07:59:54.000000 aliyun-python-sdk-vpcpeer-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2472 2023-05-30 07:59:53.000000 aliyun-python-sdk-vpcpeer-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:37:38.000000 aliyun-python-sdk-vpcpeer-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-07-25 09:37:38.000000 aliyun-python-sdk-vpcpeer-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-07-25 09:37:38.000000 aliyun-python-sdk-vpcpeer-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-07-25 09:37:38.000000 aliyun-python-sdk-vpcpeer-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      535 2023-07-25 09:37:38.000000 aliyun-python-sdk-vpcpeer-1.0.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:37:38.000000 aliyun-python-sdk-vpcpeer-1.0.2/aliyun_python_sdk_vpcpeer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-07-25 09:37:38.000000 aliyun-python-sdk-vpcpeer-1.0.2/aliyun_python_sdk_vpcpeer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1166 2023-07-25 09:37:38.000000 aliyun-python-sdk-vpcpeer-1.0.2/aliyun_python_sdk_vpcpeer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 09:37:38.000000 aliyun-python-sdk-vpcpeer-1.0.2/aliyun_python_sdk_vpcpeer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-25 09:37:38.000000 aliyun-python-sdk-vpcpeer-1.0.2/aliyun_python_sdk_vpcpeer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-25 09:37:38.000000 aliyun-python-sdk-vpcpeer-1.0.2/aliyun_python_sdk_vpcpeer.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:37:38.000000 aliyun-python-sdk-vpcpeer-1.0.2/aliyunsdkvpcpeer/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-25 09:37:38.000000 aliyun-python-sdk-vpcpeer-1.0.2/aliyunsdkvpcpeer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2023-07-25 09:37:38.000000 aliyun-python-sdk-vpcpeer-1.0.2/aliyunsdkvpcpeer/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:37:38.000000 aliyun-python-sdk-vpcpeer-1.0.2/aliyunsdkvpcpeer/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 09:37:38.000000 aliyun-python-sdk-vpcpeer-1.0.2/aliyunsdkvpcpeer/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:37:38.000000 aliyun-python-sdk-vpcpeer-1.0.2/aliyunsdkvpcpeer/request/v20220101/
+-rw-r--r--   0 root         (0) root         (0)     2324 2023-07-25 09:37:38.000000 aliyun-python-sdk-vpcpeer-1.0.2/aliyunsdkvpcpeer/request/v20220101/AcceptVpcPeerConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3056 2023-07-25 09:37:38.000000 aliyun-python-sdk-vpcpeer-1.0.2/aliyunsdkvpcpeer/request/v20220101/CreateVpcPeerConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2016 2023-07-25 09:37:38.000000 aliyun-python-sdk-vpcpeer-1.0.2/aliyunsdkvpcpeer/request/v20220101/DeleteVpcPeerConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1752 2023-07-25 09:37:38.000000 aliyun-python-sdk-vpcpeer-1.0.2/aliyunsdkvpcpeer/request/v20220101/GetVpcPeerConnectionAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2556 2023-07-25 09:37:38.000000 aliyun-python-sdk-vpcpeer-1.0.2/aliyunsdkvpcpeer/request/v20220101/ListTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2891 2023-07-25 09:37:38.000000 aliyun-python-sdk-vpcpeer-1.0.2/aliyunsdkvpcpeer/request/v20220101/ListVpcPeerConnectionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2023-07-25 09:37:38.000000 aliyun-python-sdk-vpcpeer-1.0.2/aliyunsdkvpcpeer/request/v20220101/ModifyVpcPeerConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1921 2023-07-25 09:37:38.000000 aliyun-python-sdk-vpcpeer-1.0.2/aliyunsdkvpcpeer/request/v20220101/MoveResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2104 2023-07-25 09:37:38.000000 aliyun-python-sdk-vpcpeer-1.0.2/aliyunsdkvpcpeer/request/v20220101/RejectVpcPeerConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-07-25 09:37:38.000000 aliyun-python-sdk-vpcpeer-1.0.2/aliyunsdkvpcpeer/request/v20220101/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2345 2023-07-25 09:37:38.000000 aliyun-python-sdk-vpcpeer-1.0.2/aliyunsdkvpcpeer/request/v20220101/UnTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 09:37:38.000000 aliyun-python-sdk-vpcpeer-1.0.2/aliyunsdkvpcpeer/request/v20220101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-07-25 09:37:38.000000 aliyun-python-sdk-vpcpeer-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-07-25 09:37:38.000000 aliyun-python-sdk-vpcpeer-1.0.2/setup.py
```

### Comparing `aliyun-python-sdk-vpcpeer-1.0.1/LICENSE` & `aliyun-python-sdk-vpcpeer-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-vpcpeer-1.0.1/PKG-INFO` & `aliyun-python-sdk-vpcpeer-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-vpcpeer
-Version: 1.0.1
+Version: 1.0.2
 Summary: The vpcpeer module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-vpcpeer
```

### Comparing `aliyun-python-sdk-vpcpeer-1.0.1/README.rst` & `aliyun-python-sdk-vpcpeer-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-vpcpeer-1.0.1/aliyun_python_sdk_vpcpeer.egg-info/PKG-INFO` & `aliyun-python-sdk-vpcpeer-1.0.2/aliyun_python_sdk_vpcpeer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-vpcpeer
-Version: 1.0.1
+Version: 1.0.2
 Summary: The vpcpeer module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-vpcpeer
```

### Comparing `aliyun-python-sdk-vpcpeer-1.0.1/aliyun_python_sdk_vpcpeer.egg-info/SOURCES.txt` & `aliyun-python-sdk-vpcpeer-1.0.2/aliyun_python_sdk_vpcpeer.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -14,11 +14,12 @@
 aliyunsdkvpcpeer/request/v20220101/AcceptVpcPeerConnectionRequest.py
 aliyunsdkvpcpeer/request/v20220101/CreateVpcPeerConnectionRequest.py
 aliyunsdkvpcpeer/request/v20220101/DeleteVpcPeerConnectionRequest.py
 aliyunsdkvpcpeer/request/v20220101/GetVpcPeerConnectionAttributeRequest.py
 aliyunsdkvpcpeer/request/v20220101/ListTagResourcesRequest.py
 aliyunsdkvpcpeer/request/v20220101/ListVpcPeerConnectionsRequest.py
 aliyunsdkvpcpeer/request/v20220101/ModifyVpcPeerConnectionRequest.py
+aliyunsdkvpcpeer/request/v20220101/MoveResourceGroupRequest.py
 aliyunsdkvpcpeer/request/v20220101/RejectVpcPeerConnectionRequest.py
 aliyunsdkvpcpeer/request/v20220101/TagResourcesRequest.py
 aliyunsdkvpcpeer/request/v20220101/UnTagResourcesRequest.py
 aliyunsdkvpcpeer/request/v20220101/__init__.py
```

### Comparing `aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/endpoint.py` & `aliyun-python-sdk-vpcpeer-1.0.2/aliyunsdkvpcpeer/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/AcceptVpcPeerConnectionRequest.py` & `aliyun-python-sdk-vpcpeer-1.0.2/aliyunsdkvpcpeer/request/v20220101/AcceptVpcPeerConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/CreateVpcPeerConnectionRequest.py` & `aliyun-python-sdk-vpcpeer-1.0.2/aliyunsdkvpcpeer/request/v20220101/CreateVpcPeerConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/DeleteVpcPeerConnectionRequest.py` & `aliyun-python-sdk-vpcpeer-1.0.2/aliyunsdkvpcpeer/request/v20220101/DeleteVpcPeerConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/GetVpcPeerConnectionAttributeRequest.py` & `aliyun-python-sdk-vpcpeer-1.0.2/aliyunsdkvpcpeer/request/v20220101/GetVpcPeerConnectionAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/ListTagResourcesRequest.py` & `aliyun-python-sdk-vpcpeer-1.0.2/aliyunsdkvpcpeer/request/v20220101/ListTagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/ListVpcPeerConnectionsRequest.py` & `aliyun-python-sdk-vpcpeer-1.0.2/aliyunsdkvpcpeer/request/v20220101/ListVpcPeerConnectionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/ModifyVpcPeerConnectionRequest.py` & `aliyun-python-sdk-vpcpeer-1.0.2/aliyunsdkvpcpeer/request/v20220101/ModifyVpcPeerConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/RejectVpcPeerConnectionRequest.py` & `aliyun-python-sdk-vpcpeer-1.0.2/aliyunsdkvpcpeer/request/v20220101/RejectVpcPeerConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/TagResourcesRequest.py` & `aliyun-python-sdk-vpcpeer-1.0.2/aliyunsdkvpcpeer/request/v20220101/TagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-vpcpeer-1.0.1/aliyunsdkvpcpeer/request/v20220101/UnTagResourcesRequest.py` & `aliyun-python-sdk-vpcpeer-1.0.2/aliyunsdkvpcpeer/request/v20220101/UnTagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-vpcpeer-1.0.1/setup.py` & `aliyun-python-sdk-vpcpeer-1.0.2/setup.py`

 * *Files identical despite different names*

