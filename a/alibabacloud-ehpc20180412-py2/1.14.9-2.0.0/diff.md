# Comparing `tmp/alibabacloud_ehpc20180412_py2-1.14.9.tar.gz` & `tmp/alibabacloud_ehpc20180412_py2-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_ehpc20180412_py2-1.14.9.tar", last modified: Mon Oct 25 06:34:56 2021, max compression
+gzip compressed data, was "dist/alibabacloud_ehpc20180412_py2-2.0.0.tar", last modified: Tue Jul 25 10:36:22 2023, max compression
```

## Comparing `alibabacloud_ehpc20180412_py2-1.14.9.tar` & `alibabacloud_ehpc20180412_py2-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 06:34:56.000000 alibabacloud_ehpc20180412_py2-1.14.9/
--rw-r--r--   0 root         (0) root         (0)      588 2021-10-25 06:34:56.000000 alibabacloud_ehpc20180412_py2-1.14.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1119 2021-10-25 06:34:56.000000 alibabacloud_ehpc20180412_py2-1.14.9/README.md
--rw-r--r--   0 root         (0) root         (0)     2469 2021-10-25 06:34:56.000000 alibabacloud_ehpc20180412_py2-1.14.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       28 2021-10-25 06:34:56.000000 alibabacloud_ehpc20180412_py2-1.14.9/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 06:34:56.000000 alibabacloud_ehpc20180412_py2-1.14.9/alibabacloud_ehpc20180412_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)       26 2021-10-25 06:34:56.000000 alibabacloud_ehpc20180412_py2-1.14.9/alibabacloud_ehpc20180412_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2469 2021-10-25 06:34:56.000000 alibabacloud_ehpc20180412_py2-1.14.9/alibabacloud_ehpc20180412_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      448 2021-10-25 06:34:56.000000 alibabacloud_ehpc20180412_py2-1.14.9/alibabacloud_ehpc20180412_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-10-25 06:34:56.000000 alibabacloud_ehpc20180412_py2-1.14.9/alibabacloud_ehpc20180412_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      175 2021-10-25 06:34:56.000000 alibabacloud_ehpc20180412_py2-1.14.9/alibabacloud_ehpc20180412_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1036 2021-10-25 06:34:56.000000 alibabacloud_ehpc20180412_py2-1.14.9/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     2938 2021-10-25 06:34:56.000000 alibabacloud_ehpc20180412_py2-1.14.9/setup.py
--rw-r--r--   0 root         (0) root         (0)       94 2021-10-25 06:34:56.000000 alibabacloud_ehpc20180412_py2-1.14.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       61 2021-10-25 06:34:56.000000 alibabacloud_ehpc20180412_py2-1.14.9/ChangeLog.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-25 06:34:56.000000 alibabacloud_ehpc20180412_py2-1.14.9/alibabacloud_ehpc20180412/
--rw-r--r--   0 root         (0) root         (0)    75152 2021-10-25 06:34:56.000000 alibabacloud_ehpc20180412_py2-1.14.9/alibabacloud_ehpc20180412/client.py
--rw-r--r--   0 root         (0) root         (0)   743993 2021-10-25 06:34:56.000000 alibabacloud_ehpc20180412_py2-1.14.9/alibabacloud_ehpc20180412/models.py
--rw-r--r--   0 root         (0) root         (0)       22 2021-10-25 06:34:56.000000 alibabacloud_ehpc20180412_py2-1.14.9/alibabacloud_ehpc20180412/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:36:22.000000 alibabacloud_ehpc20180412_py2-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1425 2023-07-25 10:36:22.000000 alibabacloud_ehpc20180412_py2-2.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-25 10:36:22.000000 alibabacloud_ehpc20180412_py2-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-25 10:36:22.000000 alibabacloud_ehpc20180412_py2-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-07-25 10:36:22.000000 alibabacloud_ehpc20180412_py2-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1036 2023-07-25 10:36:22.000000 alibabacloud_ehpc20180412_py2-2.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-07-25 10:36:22.000000 alibabacloud_ehpc20180412_py2-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:36:22.000000 alibabacloud_ehpc20180412_py2-2.0.0/alibabacloud_ehpc20180412/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-25 10:36:22.000000 alibabacloud_ehpc20180412_py2-2.0.0/alibabacloud_ehpc20180412/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   146120 2023-07-25 10:36:22.000000 alibabacloud_ehpc20180412_py2-2.0.0/alibabacloud_ehpc20180412/client.py
+-rw-r--r--   0 root         (0) root         (0)  1231563 2023-07-25 10:36:22.000000 alibabacloud_ehpc20180412_py2-2.0.0/alibabacloud_ehpc20180412/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:36:22.000000 alibabacloud_ehpc20180412_py2-2.0.0/alibabacloud_ehpc20180412_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-07-25 10:36:22.000000 alibabacloud_ehpc20180412_py2-2.0.0/alibabacloud_ehpc20180412_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      448 2023-07-25 10:36:22.000000 alibabacloud_ehpc20180412_py2-2.0.0/alibabacloud_ehpc20180412_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 10:36:22.000000 alibabacloud_ehpc20180412_py2-2.0.0/alibabacloud_ehpc20180412_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-25 10:36:22.000000 alibabacloud_ehpc20180412_py2-2.0.0/alibabacloud_ehpc20180412_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-25 10:36:22.000000 alibabacloud_ehpc20180412_py2-2.0.0/alibabacloud_ehpc20180412_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-25 10:36:22.000000 alibabacloud_ehpc20180412_py2-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2938 2023-07-25 10:36:22.000000 alibabacloud_ehpc20180412_py2-2.0.0/setup.py
```

### Comparing `alibabacloud_ehpc20180412_py2-1.14.9/LICENSE` & `alibabacloud_ehpc20180412_py2-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_ehpc20180412_py2-1.14.9/README.md` & `alibabacloud_ehpc20180412_py2-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ehpc20180412_py2-1.14.9/PKG-INFO` & `alibabacloud_ehpc20180412_py2-2.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: alibabacloud_ehpc20180412_py2
-Version: 1.14.9
+Version: 2.0.0
 Summary: Alibaba Cloud Elastic High Performance Computing (20180412) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -59,7 +59,8 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development
+Description-Content-Type: text/markdown
```

### Comparing `alibabacloud_ehpc20180412_py2-1.14.9/alibabacloud_ehpc20180412_py2.egg-info/PKG-INFO` & `alibabacloud_ehpc20180412_py2-2.0.0/alibabacloud_ehpc20180412_py2.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: alibabacloud-ehpc20180412-py2
-Version: 1.14.9
+Version: 2.0.0
 Summary: Alibaba Cloud Elastic High Performance Computing (20180412) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -59,7 +59,8 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development
+Description-Content-Type: text/markdown
```

### Comparing `alibabacloud_ehpc20180412_py2-1.14.9/README-CN.md` & `alibabacloud_ehpc20180412_py2-2.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ehpc20180412_py2-1.14.9/setup.py` & `alibabacloud_ehpc20180412_py2-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_ehpc20180412_py2.
 
-Created on 25/10/2021
+Created on 25/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_ehpc20180412"
 NAME = "alibabacloud_ehpc20180412_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Elastic High Performance Computing (20180412) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.5, <1.0.0",
-    "alibabacloud_tea_openapi_py2>=0.0.6, <1.0.0",
-    "alibabacloud_openapi_util_py2>=0.0.7, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.9, <1.0.0",
+    "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
+    "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
```

