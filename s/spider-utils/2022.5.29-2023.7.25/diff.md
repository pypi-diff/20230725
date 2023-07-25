# Comparing `tmp/spider-utils-2022.5.29.tar.gz` & `tmp/spider-utils-2023.7.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\spider-utils-2022.5.29.tar", last modified: Sun May 29 04:43:10 2022, max compression
+gzip compressed data, was "dist\spider-utils-2023.7.25.tar", last modified: Tue Jul 25 08:40:02 2023, max compression
```

## Comparing `spider-utils-2022.5.29.tar` & `spider-utils-2023.7.25.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-05-29 04:43:10.000000 spider-utils-2022.5.29/
--rw-rw-rw-   0        0        0       38 2019-11-30 15:34:22.000000 spider-utils-2022.5.29/MANIFEST.in
--rw-rw-rw-   0        0        0     1170 2022-05-29 04:43:10.000000 spider-utils-2022.5.29/PKG-INFO
--rw-rw-rw-   0        0        0      257 2019-11-30 09:17:23.000000 spider-utils-2022.5.29/README.md
--rw-rw-rw-   0        0        0       42 2022-05-29 04:43:10.000000 spider-utils-2022.5.29/setup.cfg
--rw-rw-rw-   0        0        0     2960 2022-05-29 04:43:09.000000 spider-utils-2022.5.29/setup.py
-drwxrwxrwx   0        0        0        0 2022-05-29 04:43:10.000000 spider-utils-2022.5.29/spider_utils/
--rw-rw-rw-   0        0        0     8100 2020-08-15 16:29:36.000000 spider-utils-2022.5.29/spider_utils/client.py
-drwxrwxrwx   0        0        0        0 2022-05-29 04:43:10.000000 spider-utils-2022.5.29/spider_utils/data/
--rw-rw-rw-   0        0        0    42686 2019-11-03 14:44:29.000000 spider-utils-2022.5.29/spider_utils/data/fake_useragent_0.1.11.json
--rw-rw-rw-   0        0        0   130849 2019-07-20 12:32:08.000000 spider-utils-2022.5.29/spider_utils/data/mobile_user_agents.txt
--rw-rw-rw-   0        0        0     2714 2020-05-24 15:14:09.000000 spider-utils-2022.5.29/spider_utils/download.py
--rw-rw-rw-   0        0        0     7261 2021-06-15 11:07:01.000000 spider-utils-2022.5.29/spider_utils/spider.py
--rw-rw-rw-   0        0        0      600 2019-11-30 16:02:24.000000 spider-utils-2022.5.29/spider_utils/useragent.py
--rw-rw-rw-   0        0        0     1020 2019-11-30 10:14:27.000000 spider-utils-2022.5.29/spider_utils/utils.py
--rw-rw-rw-   0        0        0      580 2019-11-30 15:53:53.000000 spider-utils-2022.5.29/spider_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-29 04:43:10.000000 spider-utils-2022.5.29/spider_utils.egg-info/
--rw-rw-rw-   0        0        0        1 2022-05-29 04:43:10.000000 spider-utils-2022.5.29/spider_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2019-11-30 10:23:41.000000 spider-utils-2022.5.29/spider_utils.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     1170 2022-05-29 04:43:10.000000 spider-utils-2022.5.29/spider_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      130 2022-05-29 04:43:10.000000 spider-utils-2022.5.29/spider_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0      474 2022-05-29 04:43:10.000000 spider-utils-2022.5.29/spider_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       13 2022-05-29 04:43:10.000000 spider-utils-2022.5.29/spider_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 08:40:02.000000 spider-utils-2023.7.25/
+-rw-rw-rw-   0        0        0       38 2019-11-30 15:34:22.000000 spider-utils-2023.7.25/MANIFEST.in
+-rw-rw-rw-   0        0        0     1170 2023-07-25 08:40:02.000000 spider-utils-2023.7.25/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2019-11-30 09:17:23.000000 spider-utils-2023.7.25/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-25 08:40:02.000000 spider-utils-2023.7.25/setup.cfg
+-rw-rw-rw-   0        0        0     2959 2023-07-25 08:39:00.000000 spider-utils-2023.7.25/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:40:02.000000 spider-utils-2023.7.25/spider_utils/
+-rw-rw-rw-   0        0        0     8100 2020-08-15 16:29:36.000000 spider-utils-2023.7.25/spider_utils/client.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:40:02.000000 spider-utils-2023.7.25/spider_utils/data/
+-rw-rw-rw-   0        0        0    42686 2019-11-03 14:44:29.000000 spider-utils-2023.7.25/spider_utils/data/fake_useragent_0.1.11.json
+-rw-rw-rw-   0        0        0   130849 2019-07-20 12:32:08.000000 spider-utils-2023.7.25/spider_utils/data/mobile_user_agents.txt
+-rw-rw-rw-   0        0        0     2714 2020-05-24 15:14:09.000000 spider-utils-2023.7.25/spider_utils/download.py
+-rw-rw-rw-   0        0        0     7261 2021-06-15 11:07:01.000000 spider-utils-2023.7.25/spider_utils/spider.py
+-rw-rw-rw-   0        0        0      606 2023-07-25 08:39:00.000000 spider-utils-2023.7.25/spider_utils/useragent.py
+-rw-rw-rw-   0        0        0     1020 2019-11-30 10:14:27.000000 spider-utils-2023.7.25/spider_utils/utils.py
+-rw-rw-rw-   0        0        0      580 2019-11-30 15:53:53.000000 spider-utils-2023.7.25/spider_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:40:02.000000 spider-utils-2023.7.25/spider_utils.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-25 08:40:02.000000 spider-utils-2023.7.25/spider_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2019-11-30 10:23:41.000000 spider-utils-2023.7.25/spider_utils.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     1170 2023-07-25 08:40:02.000000 spider-utils-2023.7.25/spider_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      129 2023-07-25 08:40:02.000000 spider-utils-2023.7.25/spider_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      474 2023-07-25 08:40:02.000000 spider-utils-2023.7.25/spider_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       13 2023-07-25 08:40:02.000000 spider-utils-2023.7.25/spider_utils.egg-info/top_level.txt
```

### Comparing `spider-utils-2022.5.29/PKG-INFO` & `spider-utils-2023.7.25/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spider-utils
-Version: 2022.5.29
+Version: 2023.7.25
 Summary: 常用爬虫模块的集合，为了多平台，多电脑调用方便!
 Home-page: https://github.com/ldsxp/spider-utils
 Author: lds
 Author-email: 85176878@qq.com
 License: GNU GPL 3
 Download-URL: https://pypi.org/project/spider-utils
 Description: # spider-utils
```

### Comparing `spider-utils-2022.5.29/setup.py` & `spider-utils-2023.7.25/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ﻿import os
 import sys
 
 # from pypandoc import convert
 from setuptools import setup, find_packages
 
-version = '2022.5.29'
+version = '2023.7.25'
 
 """
 pip install -U spider-utils
 pip --no-cache-dir install -U spider-utils
 
 # 检查错误
 # twine check dist/*
@@ -77,15 +77,15 @@
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.6',
     ],
     # 需要安装的依赖包
     install_requires=[
         'requests>=2.27.1',
-        'fake_useragent==0.1.11',
+        'fake_useragent>=1.1.3',
         'tqdm>=4.64.0',
         'loguru>=0.6.0',
         'beautifulsoup4>=4.11.1',
         'html2text>=2020.1.16',
     ],
     # data_files=[('', ['spider_utils/data/fake_useragent_0.1.11.json', 'spider_utils/data/mobile_user_agents.txt', ])],
     include_package_data=True,
```

### Comparing `spider-utils-2022.5.29/spider_utils/client.py` & `spider-utils-2023.7.25/spider_utils/client.py`

 * *Files identical despite different names*

### Comparing `spider-utils-2022.5.29/spider_utils/data/fake_useragent_0.1.11.json` & `spider-utils-2023.7.25/spider_utils/data/fake_useragent_0.1.11.json`

 * *Files identical despite different names*

### Comparing `spider-utils-2022.5.29/spider_utils/data/mobile_user_agents.txt` & `spider-utils-2023.7.25/spider_utils/data/mobile_user_agents.txt`

 * *Files identical despite different names*

### Comparing `spider-utils-2022.5.29/spider_utils/download.py` & `spider-utils-2023.7.25/spider_utils/download.py`

 * *Files identical despite different names*

### Comparing `spider-utils-2022.5.29/spider_utils/spider.py` & `spider-utils-2023.7.25/spider_utils/spider.py`

 * *Files identical despite different names*

### Comparing `spider-utils-2022.5.29/spider_utils/useragent.py` & `spider-utils-2023.7.25/spider_utils/useragent.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import random
 
 from . import BASE_DIR
 
 from fake_useragent import UserAgent
 
 # fake-useragent fake_useragent.json 下载： https://fake-useragent.herokuapp.com/browsers/0.1.11
-ua = UserAgent(path=os.path.join(BASE_DIR, 'data', 'fake_useragent_0.1.11.json'))
+ua = UserAgent(cache_path=os.path.join(BASE_DIR, 'data', 'fake_useragent_0.1.11.json'))
 
 with open(os.path.join(BASE_DIR, 'data', 'mobile_user_agents.txt')) as f:
     mobile_user_agents = [i.strip() for i in f.readlines()]
 
 
 def get_user_agent(is_mobile=False):
     """
```

### Comparing `spider-utils-2022.5.29/spider_utils/utils.py` & `spider-utils-2023.7.25/spider_utils/utils.py`

 * *Files identical despite different names*

### Comparing `spider-utils-2022.5.29/spider_utils/__init__.py` & `spider-utils-2023.7.25/spider_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `spider-utils-2022.5.29/spider_utils.egg-info/PKG-INFO` & `spider-utils-2023.7.25/spider_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spider-utils
-Version: 2022.5.29
+Version: 2023.7.25
 Summary: 常用爬虫模块的集合，为了多平台，多电脑调用方便!
 Home-page: https://github.com/ldsxp/spider-utils
 Author: lds
 Author-email: 85176878@qq.com
 License: GNU GPL 3
 Download-URL: https://pypi.org/project/spider-utils
 Description: # spider-utils
```

