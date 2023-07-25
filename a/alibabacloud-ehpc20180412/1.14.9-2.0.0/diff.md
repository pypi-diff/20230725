# Comparing `tmp/alibabacloud_ehpc20180412-1.14.9.tar.gz` & `tmp/alibabacloud_ehpc20180412-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_ehpc20180412-1.14.9.tar", last modified: Mon Oct 25 06:35:05 2021, max compression
+gzip compressed data, was "dist/alibabacloud_ehpc20180412-2.0.0.tar", last modified: Tue Jul 25 10:36:57 2023, max compression
```

## Comparing `alibabacloud_ehpc20180412-1.14.9.tar` & `alibabacloud_ehpc20180412-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/
--rw-r--r--   0 root         (0) root         (0)      226 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2365 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1025 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1110 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/alibabacloud_ehpc20180412/
--rw-r--r--   0 root         (0) root         (0)       22 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/alibabacloud_ehpc20180412/__init__.py
--rw-r--r--   0 root         (0) root         (0)   217305 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/alibabacloud_ehpc20180412/client.py
--rw-r--r--   0 root         (0) root         (0)   737630 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/alibabacloud_ehpc20180412/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/alibabacloud_ehpc20180412.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2365 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/alibabacloud_ehpc20180412.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      428 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/alibabacloud_ehpc20180412.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/alibabacloud_ehpc20180412.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/alibabacloud_ehpc20180412.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/alibabacloud_ehpc20180412.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2645 2021-10-25 06:35:05.000000 alibabacloud_ehpc20180412-1.14.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:36:57.000000 alibabacloud_ehpc20180412-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-07-25 10:36:57.000000 alibabacloud_ehpc20180412-2.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-25 10:36:57.000000 alibabacloud_ehpc20180412-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-25 10:36:57.000000 alibabacloud_ehpc20180412-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-07-25 10:36:57.000000 alibabacloud_ehpc20180412-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-07-25 10:36:57.000000 alibabacloud_ehpc20180412-2.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-07-25 10:36:57.000000 alibabacloud_ehpc20180412-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:36:57.000000 alibabacloud_ehpc20180412-2.0.0/alibabacloud_ehpc20180412/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-25 10:36:57.000000 alibabacloud_ehpc20180412-2.0.0/alibabacloud_ehpc20180412/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   370027 2023-07-25 10:36:57.000000 alibabacloud_ehpc20180412-2.0.0/alibabacloud_ehpc20180412/client.py
+-rw-r--r--   0 root         (0) root         (0)  1221987 2023-07-25 10:36:57.000000 alibabacloud_ehpc20180412-2.0.0/alibabacloud_ehpc20180412/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:36:57.000000 alibabacloud_ehpc20180412-2.0.0/alibabacloud_ehpc20180412.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-07-25 10:36:57.000000 alibabacloud_ehpc20180412-2.0.0/alibabacloud_ehpc20180412.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      428 2023-07-25 10:36:57.000000 alibabacloud_ehpc20180412-2.0.0/alibabacloud_ehpc20180412.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 10:36:57.000000 alibabacloud_ehpc20180412-2.0.0/alibabacloud_ehpc20180412.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-07-25 10:36:57.000000 alibabacloud_ehpc20180412-2.0.0/alibabacloud_ehpc20180412.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-25 10:36:57.000000 alibabacloud_ehpc20180412-2.0.0/alibabacloud_ehpc20180412.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-25 10:36:57.000000 alibabacloud_ehpc20180412-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2646 2023-07-25 10:36:57.000000 alibabacloud_ehpc20180412-2.0.0/setup.py
```

### Comparing `alibabacloud_ehpc20180412-1.14.9/LICENSE` & `alibabacloud_ehpc20180412-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_ehpc20180412-1.14.9/PKG-INFO` & `alibabacloud_ehpc20180412-2.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_ehpc20180412
-Version: 1.14.9
+Version: 2.0.0
 Summary: Alibaba Cloud Elastic High Performance Computing (20180412) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ehpc20180412-1.14.9/README-CN.md` & `alibabacloud_ehpc20180412-2.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ehpc20180412-1.14.9/README.md` & `alibabacloud_ehpc20180412-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ehpc20180412-1.14.9/alibabacloud_ehpc20180412.egg-info/PKG-INFO` & `alibabacloud_ehpc20180412-2.0.0/alibabacloud_ehpc20180412.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ehpc20180412
-Version: 1.14.9
+Version: 2.0.0
 Summary: Alibaba Cloud Elastic High Performance Computing (20180412) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ehpc20180412-1.14.9/setup.py` & `alibabacloud_ehpc20180412-2.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_ehpc20180412.
 
-Created on 25/10/2021
+Created on 25/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_ehpc20180412"
 NAME = "alibabacloud_ehpc20180412" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Elastic High Performance Computing (20180412) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.5, <1.0.0",
-    "alibabacloud_tea_openapi>=0.2.7, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.5, <1.0.0",
+    "alibabacloud_tea_util>=0.3.11, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

