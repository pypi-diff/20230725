# Comparing `tmp/tme_api-2023.7.25.tar.gz` & `tmp/tme_api-2023.7.25.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\tme_api-2023.7.25.tar", last modified: Tue Jul 25 08:58:15 2023, max compression
+gzip compressed data, was "dist\tme_api-2023.7.25.post2.tar", last modified: Tue Jul 25 09:26:46 2023, max compression
```

## Comparing `tme_api-2023.7.25.tar` & `tme_api-2023.7.25.post2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 08:58:15.000000 tme_api-2023.7.25/
--rw-rw-rw-   0        0        0      609 2023-07-25 08:58:15.000000 tme_api-2023.7.25/PKG-INFO
--rw-rw-rw-   0        0        0       44 2022-01-26 09:14:36.000000 tme_api-2023.7.25/README.md
--rw-rw-rw-   0        0        0       42 2023-07-25 08:58:15.000000 tme_api-2023.7.25/setup.cfg
--rw-rw-rw-   0        0        0     5334 2023-07-25 08:57:15.000000 tme_api-2023.7.25/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:58:15.000000 tme_api-2023.7.25/tme_api/
-drwxrwxrwx   0        0        0        0 2023-07-25 08:58:15.000000 tme_api-2023.7.25/tme_api/cms/
--rw-rw-rw-   0        0        0    26444 2022-10-20 08:36:17.000000 tme_api-2023.7.25/tme_api/cms/api.py
--rw-rw-rw-   0        0        0     7533 2023-03-20 11:00:57.000000 tme_api-2023.7.25/tme_api/cms/enums.py
--rw-rw-rw-   0        0        0      656 2020-09-28 03:45:55.000000 tme_api-2023.7.25/tme_api/cms/exception.py
--rw-rw-rw-   0        0        0    16771 2023-07-25 08:55:55.000000 tme_api-2023.7.25/tme_api/cms/model.py
--rw-rw-rw-   0        0        0    20739 2023-07-25 08:55:55.000000 tme_api-2023.7.25/tme_api/cms/requests.py
--rw-rw-rw-   0        0        0    28480 2023-07-25 08:55:55.000000 tme_api-2023.7.25/tme_api/cms/responses.py
--rw-rw-rw-   0        0        0     1566 2021-11-08 10:41:13.000000 tme_api-2023.7.25/tme_api/cms/utils.py
--rw-rw-rw-   0        0        0        0 2020-09-01 10:18:32.000000 tme_api-2023.7.25/tme_api/cms/__init__.py
--rw-rw-rw-   0        0        0        0 2020-09-01 10:18:32.000000 tme_api-2023.7.25/tme_api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:58:15.000000 tme_api-2023.7.25/tme_api.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-25 08:58:14.000000 tme_api-2023.7.25/tme_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      609 2023-07-25 08:58:14.000000 tme_api-2023.7.25/tme_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       56 2023-07-25 08:58:14.000000 tme_api-2023.7.25/tme_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0      372 2023-07-25 08:58:14.000000 tme_api-2023.7.25/tme_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-07-25 08:58:14.000000 tme_api-2023.7.25/tme_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 09:26:46.000000 tme_api-2023.7.25.post2/
+-rw-rw-rw-   0        0        0      615 2023-07-25 09:26:46.000000 tme_api-2023.7.25.post2/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2022-01-26 09:14:36.000000 tme_api-2023.7.25.post2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-25 09:26:46.000000 tme_api-2023.7.25.post2/setup.cfg
+-rw-rw-rw-   0        0        0     5339 2023-07-25 09:24:21.000000 tme_api-2023.7.25.post2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:26:46.000000 tme_api-2023.7.25.post2/tme_api/
+drwxrwxrwx   0        0        0        0 2023-07-25 09:26:46.000000 tme_api-2023.7.25.post2/tme_api/cms/
+-rw-rw-rw-   0        0        0    26444 2022-10-20 08:36:17.000000 tme_api-2023.7.25.post2/tme_api/cms/api.py
+-rw-rw-rw-   0        0        0     7533 2023-03-20 11:00:57.000000 tme_api-2023.7.25.post2/tme_api/cms/enums.py
+-rw-rw-rw-   0        0        0      656 2020-09-28 03:45:55.000000 tme_api-2023.7.25.post2/tme_api/cms/exception.py
+-rw-rw-rw-   0        0        0    16771 2023-07-25 08:55:55.000000 tme_api-2023.7.25.post2/tme_api/cms/model.py
+-rw-rw-rw-   0        0        0    20739 2023-07-25 08:55:55.000000 tme_api-2023.7.25.post2/tme_api/cms/requests.py
+-rw-rw-rw-   0        0        0    28480 2023-07-25 08:55:55.000000 tme_api-2023.7.25.post2/tme_api/cms/responses.py
+-rw-rw-rw-   0        0        0     1566 2021-11-08 10:41:13.000000 tme_api-2023.7.25.post2/tme_api/cms/utils.py
+-rw-rw-rw-   0        0        0        0 2020-09-01 10:18:32.000000 tme_api-2023.7.25.post2/tme_api/cms/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-09-01 10:18:32.000000 tme_api-2023.7.25.post2/tme_api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:26:46.000000 tme_api-2023.7.25.post2/tme_api.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-25 09:26:46.000000 tme_api-2023.7.25.post2/tme_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      615 2023-07-25 09:26:46.000000 tme_api-2023.7.25.post2/tme_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       59 2023-07-25 09:26:46.000000 tme_api-2023.7.25.post2/tme_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      372 2023-07-25 09:26:46.000000 tme_api-2023.7.25.post2/tme_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-07-25 09:26:46.000000 tme_api-2023.7.25.post2/tme_api.egg-info/top_level.txt
```

### Comparing `tme_api-2023.7.25/PKG-INFO` & `tme_api-2023.7.25.post2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tme_api
-Version: 2023.7.25
+Version: 2023.7.25.post2
 Summary: tme_api
 Home-page: https://github.com/ldsxp/tme_api
 Author: lds
 Author-email: 85176878@qq.com
 License: GNU GPL 3
 Download-URL: https://pypi.org/project/tme_api
 Description: 访问 icms.tmeoa.com 的api
```

### Comparing `tme_api-2023.7.25/setup.py` & `tme_api-2023.7.25.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ﻿import os
 import sys
 from setuptools import setup, find_packages
 
-version = '2023.7.25'
+version = '2023.7.25-2'
 
 # 创建一个源码包
 # python setup.py sdist
 # 对于 Windows，可以执行python setup.py bdist_wininst 生成一个exe文件；
 # 若要生成 RPM 包，执行 python setup.py bdist_rpm，但系统必须有 rpm 命令的支持。
 # 可以运行下面的命令查看所有格式的支持：
 # python setup.py bdist --help-formats
@@ -124,15 +124,15 @@
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.6',
     ],
     # 需要安装的依赖包
     install_requires=[
         'requests_toolbelt',
         'requests',
-        'pydantic>=1.9.2',
+        'pydantic>=1.9.2,<2',
         'spider-utils',
         # 'xlrd>=1.1.0',
         # 'colorama',
         # 'chardet',
         # 'pyperclip',
         # 'requests',
         # 'html2text',
```

### Comparing `tme_api-2023.7.25/tme_api/cms/api.py` & `tme_api-2023.7.25.post2/tme_api/cms/api.py`

 * *Files identical despite different names*

### Comparing `tme_api-2023.7.25/tme_api/cms/enums.py` & `tme_api-2023.7.25.post2/tme_api/cms/enums.py`

 * *Files identical despite different names*

### Comparing `tme_api-2023.7.25/tme_api/cms/exception.py` & `tme_api-2023.7.25.post2/tme_api/cms/exception.py`

 * *Files identical despite different names*

### Comparing `tme_api-2023.7.25/tme_api/cms/model.py` & `tme_api-2023.7.25.post2/tme_api/cms/model.py`

 * *Files identical despite different names*

### Comparing `tme_api-2023.7.25/tme_api/cms/requests.py` & `tme_api-2023.7.25.post2/tme_api/cms/requests.py`

 * *Files identical despite different names*

### Comparing `tme_api-2023.7.25/tme_api/cms/responses.py` & `tme_api-2023.7.25.post2/tme_api/cms/responses.py`

 * *Files identical despite different names*

### Comparing `tme_api-2023.7.25/tme_api/cms/utils.py` & `tme_api-2023.7.25.post2/tme_api/cms/utils.py`

 * *Files identical despite different names*

### Comparing `tme_api-2023.7.25/tme_api.egg-info/PKG-INFO` & `tme_api-2023.7.25.post2/tme_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tme-api
-Version: 2023.7.25
+Version: 2023.7.25.post2
 Summary: tme_api
 Home-page: https://github.com/ldsxp/tme_api
 Author: lds
 Author-email: 85176878@qq.com
 License: GNU GPL 3
 Download-URL: https://pypi.org/project/tme_api
 Description: 访问 icms.tmeoa.com 的api
```

