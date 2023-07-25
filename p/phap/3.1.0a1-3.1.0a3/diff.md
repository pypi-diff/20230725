# Comparing `tmp/phap-3.1.0a1.tar.gz` & `tmp/phap-3.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phap-3.1.0a1.tar", last modified: Mon Jul 24 11:44:11 2023, max compression
+gzip compressed data, was "phap-3.1.0a3.tar", last modified: Tue Jul 25 03:57:52 2023, max compression
```

## Comparing `phap-3.1.0a1.tar` & `phap-3.1.0a3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 11:44:11.340023 phap-3.1.0a1/
--rw-rw-rw-   0        0        0     1069 2023-05-25 04:31:47.000000 phap-3.1.0a1/LICENSE
--rw-rw-rw-   0        0        0     2504 2023-07-24 11:44:11.332014 phap-3.1.0a1/PKG-INFO
--rw-rw-rw-   0        0        0     1705 2023-07-24 11:38:22.000000 phap-3.1.0a1/README.md
--rw-rw-rw-   0        0        0       86 2022-03-12 07:02:40.000000 phap-3.1.0a1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-24 11:44:11.340023 phap-3.1.0a1/setup.cfg
--rw-rw-rw-   0        0        0     1685 2023-07-24 11:38:28.000000 phap-3.1.0a1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:44:11.212351 phap-3.1.0a1/src/
-drwxrwxrwx   0        0        0        0 2023-07-24 11:44:11.268380 phap-3.1.0a1/src/algo/
--rw-rw-rw-   0        0        0      210 2023-07-23 04:55:40.000000 phap-3.1.0a1/src/algo/__init__.py
--rw-rw-rw-   0        0        0      600 2023-07-24 11:42:41.000000 phap-3.1.0a1/src/algo/arraylib.py
--rw-rw-rw-   0        0        0     2356 2023-07-24 11:41:55.000000 phap-3.1.0a1/src/algo/treelib.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:44:11.276394 phap-3.1.0a1/src/pba/
--rw-rw-rw-   0        0        0     1013 2023-07-24 11:41:34.000000 phap-3.1.0a1/src/pba/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:44:11.276394 phap-3.1.0a1/src/phap/
--rw-rw-rw-   0        0        0       72 2023-07-24 11:39:49.000000 phap-3.1.0a1/src/phap/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:44:11.291984 phap-3.1.0a1/src/phap.egg-info/
--rw-rw-rw-   0        0        0     2504 2023-07-24 11:44:11.000000 phap-3.1.0a1/src/phap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2023-07-24 11:44:11.000000 phap-3.1.0a1/src/phap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 11:44:11.000000 phap-3.1.0a1/src/phap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-24 11:44:11.000000 phap-3.1.0a1/src/phap.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-24 11:44:11.324013 phap-3.1.0a1/src/stralgo/
--rw-rw-rw-   0        0        0      718 2023-07-23 04:55:41.000000 phap-3.1.0a1/src/stralgo/__init__.py
--rw-rw-rw-   0        0        0     1021 2023-07-23 04:55:41.000000 phap-3.1.0a1/src/stralgo/base.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:44:11.324013 phap-3.1.0a1/src/stralgo/hash/
--rw-rw-rw-   0        0        0      354 2023-07-23 04:55:41.000000 phap-3.1.0a1/src/stralgo/hash/__init__.py
--rw-rw-rw-   0        0        0      508 2023-07-23 04:55:41.000000 phap-3.1.0a1/src/stralgo/hash/sha.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:44:11.332014 phap-3.1.0a1/src/stralgo/hash/sm/
--rw-rw-rw-   0        0        0      148 2023-07-23 04:55:41.000000 phap-3.1.0a1/src/stralgo/hash/sm/__init__.py
--rw-rw-rw-   0        0        0     6943 2023-07-24 11:35:14.000000 phap-3.1.0a1/src/stralgo/hash/sm/sm3libs.py
--rw-rw-rw-   0        0        0      233 2023-07-23 04:55:41.000000 phap-3.1.0a1/src/stralgo/json.py
+drwxrwxrwx   0        0        0        0 2023-07-25 03:57:52.428018 phap-3.1.0a3/
+-rw-rw-rw-   0        0        0     1069 2023-05-25 04:31:47.000000 phap-3.1.0a3/LICENSE
+-rw-rw-rw-   0        0        0     2504 2023-07-25 03:57:52.427019 phap-3.1.0a3/PKG-INFO
+-rw-rw-rw-   0        0        0     1705 2023-07-25 03:54:14.000000 phap-3.1.0a3/README.md
+-rw-rw-rw-   0        0        0       86 2022-03-12 07:02:40.000000 phap-3.1.0a3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-25 03:57:52.429020 phap-3.1.0a3/setup.cfg
+-rw-rw-rw-   0        0        0     1685 2023-07-25 03:50:00.000000 phap-3.1.0a3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 03:57:52.269934 phap-3.1.0a3/src/
+drwxrwxrwx   0        0        0        0 2023-07-25 03:57:52.324286 phap-3.1.0a3/src/algo/
+-rw-rw-rw-   0        0        0      210 2023-07-23 04:55:40.000000 phap-3.1.0a3/src/algo/__init__.py
+-rw-rw-rw-   0        0        0      603 2023-07-25 03:55:42.000000 phap-3.1.0a3/src/algo/arraylib.py
+-rw-rw-rw-   0        0        0     2359 2023-07-25 03:55:39.000000 phap-3.1.0a3/src/algo/treelib.py
+drwxrwxrwx   0        0        0        0 2023-07-25 03:57:52.326290 phap-3.1.0a3/src/phap/
+-rw-rw-rw-   0        0        0       72 2023-07-24 11:39:49.000000 phap-3.1.0a3/src/phap/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 03:57:52.355296 phap-3.1.0a3/src/phap.egg-info/
+-rw-rw-rw-   0        0        0     2504 2023-07-25 03:57:52.000000 phap-3.1.0a3/src/phap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      455 2023-07-25 03:57:52.000000 phap-3.1.0a3/src/phap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 03:57:52.000000 phap-3.1.0a3/src/phap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-25 03:57:52.000000 phap-3.1.0a3/src/phap.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 03:57:52.356302 phap-3.1.0a3/src/phapbm/
+-rw-rw-rw-   0        0        0     1013 2023-07-24 11:41:34.000000 phap-3.1.0a3/src/phapbm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 03:57:52.396177 phap-3.1.0a3/src/stralgo/
+-rw-rw-rw-   0        0        0      718 2023-07-23 04:55:41.000000 phap-3.1.0a3/src/stralgo/__init__.py
+-rw-rw-rw-   0        0        0     1021 2023-07-23 04:55:41.000000 phap-3.1.0a3/src/stralgo/base.py
+drwxrwxrwx   0        0        0        0 2023-07-25 03:57:52.399177 phap-3.1.0a3/src/stralgo/hash/
+-rw-rw-rw-   0        0        0      354 2023-07-23 04:55:41.000000 phap-3.1.0a3/src/stralgo/hash/__init__.py
+-rw-rw-rw-   0        0        0      508 2023-07-23 04:55:41.000000 phap-3.1.0a3/src/stralgo/hash/sha.py
+drwxrwxrwx   0        0        0        0 2023-07-25 03:57:52.402694 phap-3.1.0a3/src/stralgo/hash/sm/
+-rw-rw-rw-   0        0        0      148 2023-07-23 04:55:41.000000 phap-3.1.0a3/src/stralgo/hash/sm/__init__.py
+-rw-rw-rw-   0        0        0     6943 2023-07-24 11:35:14.000000 phap-3.1.0a3/src/stralgo/hash/sm/sm3libs.py
+-rw-rw-rw-   0        0        0      233 2023-07-23 04:55:41.000000 phap-3.1.0a3/src/stralgo/json.py
```

### Comparing `phap-3.1.0a1/LICENSE` & `phap-3.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `phap-3.1.0a1/PKG-INFO` & `phap-3.1.0a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phap
-Version: 3.1.0a1
+Version: 3.1.0a3
 Summary: Programing Helpful Algorithm Package
 Home-page: https://github.com/DashBing/phap/
 Author: DashBing
 Author-email: mcbbkf@outlook.com
 Project-URL: Github, https://github.com/DashBing/phap/
 Project-URL: Old Project Version(stralgo), https://pypi.org/project/stralgo/
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,20 +14,20 @@
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Natural Language :: Chinese (Simplified)
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# phap
+# PHAP
 ### *Programing Helpful Algorithm Package*
 ### Powered by Python 3.11
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
 
-### English  | [简体中文](README-zh-CN.md)
+### English  | [简体中文](README_zh-CN.md)
 #### *如果你不是在Github上阅读本说明，你可能无法打开非英语版本的说明文档*
 #### *请前往[Github](https://github.com/DashBing/phap/ "Github")网站，确保你能够成功地切换语言*
 
 # Links
 [Github](https://github.com/DashBing/phap/ "Github") | [Pypi](https://pypi.org/project/phap/ "Pypi") | [Pypi (stralgo)](https://pypi.org/project/stralgo/ "Pypi (stralgo)")
 
 # Versions
@@ -38,15 +38,15 @@
 + v2.2.1
 
 ## Latest Available Version
 + v3.0.0
 
 ## Latest Version
 ### *(The data under the master branch is inaccurate. Please refer to the dev branch for details)*
-+ v3.1.0-alpha1
++ v3.1.0-alpha3
 
 # To Use
 ## Read our development document
 ### *(Click the [Github](https://github.com/DashBing/phap/ "Github") link to read this document，or you may can not to open the link)*
 + [Development Document](doc/README.md)
 
 # Build
```

### Comparing `phap-3.1.0a1/README.md` & `phap-3.1.0a3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# phap
+# PHAP
 ### *Programing Helpful Algorithm Package*
 ### Powered by Python 3.11
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
 
-### English  | [简体中文](README-zh-CN.md)
+### English  | [简体中文](README_zh-CN.md)
 #### *如果你不是在Github上阅读本说明，你可能无法打开非英语版本的说明文档*
 #### *请前往[Github](https://github.com/DashBing/phap/ "Github")网站，确保你能够成功地切换语言*
 
 # Links
 [Github](https://github.com/DashBing/phap/ "Github") | [Pypi](https://pypi.org/project/phap/ "Pypi") | [Pypi (stralgo)](https://pypi.org/project/stralgo/ "Pypi (stralgo)")
 
 # Versions
@@ -18,15 +18,15 @@
 + v2.2.1
 
 ## Latest Available Version
 + v3.0.0
 
 ## Latest Version
 ### *(The data under the master branch is inaccurate. Please refer to the dev branch for details)*
-+ v3.1.0-alpha1
++ v3.1.0-alpha3
 
 # To Use
 ## Read our development document
 ### *(Click the [Github](https://github.com/DashBing/phap/ "Github") link to read this document，or you may can not to open the link)*
 + [Development Document](doc/README.md)
 
 # Build
```

### Comparing `phap-3.1.0a1/setup.py` & `phap-3.1.0a3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="phap",
-    version="3.1.0a1",  #版本
+    version="3.1.0a3",  #版本
     author="DashBing",
     author_email="mcbbkf@outlook.com",
     description="Programing Helpful Algorithm Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     #scripts=[],
     url="https://github.com/DashBing/phap/",
```

### Comparing `phap-3.1.0a1/src/algo/arraylib.py` & `phap-3.1.0a3/src/algo/arraylib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pba import ErrorTemplate
+from phapbm import ErrorTemplate
 
 class phap_numalgo_deskcheck_DataNotTrueError(ErrorTemplate):  # 从phap包导入错误类模板，具体可见phap/__init__.py
     message = "The value is not true."
     info_list = ["Try to change a new value."]
 
 def deskcheck(
         array : list = None,
```

### Comparing `phap-3.1.0a1/src/algo/treelib.py` & `phap-3.1.0a3/src/algo/treelib.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pba import ErrorTemplate
+from phapbm import ErrorTemplate
 
 class ValueTypeError(ErrorTemplate):  # 从phap包继承错误类模板，具体可见phap/__init__.py
     message = "The value's type must not be treenode."
     info_list = ['Try to change the type to "str" or "int".']
 
 class treenode:  # 二叉树类
     def __init__(self, val = 0, left = 0, right = 0):  # 参数分别是，初始节点参数，初始节点左边和右边的值
```

### Comparing `phap-3.1.0a1/src/pba/__init__.py` & `phap-3.1.0a3/src/phapbm/__init__.py`

 * *Files identical despite different names*

### Comparing `phap-3.1.0a1/src/phap.egg-info/PKG-INFO` & `phap-3.1.0a3/src/phap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phap
-Version: 3.1.0a1
+Version: 3.1.0a3
 Summary: Programing Helpful Algorithm Package
 Home-page: https://github.com/DashBing/phap/
 Author: DashBing
 Author-email: mcbbkf@outlook.com
 Project-URL: Github, https://github.com/DashBing/phap/
 Project-URL: Old Project Version(stralgo), https://pypi.org/project/stralgo/
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,20 +14,20 @@
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Natural Language :: Chinese (Simplified)
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# phap
+# PHAP
 ### *Programing Helpful Algorithm Package*
 ### Powered by Python 3.11
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
 
-### English  | [简体中文](README-zh-CN.md)
+### English  | [简体中文](README_zh-CN.md)
 #### *如果你不是在Github上阅读本说明，你可能无法打开非英语版本的说明文档*
 #### *请前往[Github](https://github.com/DashBing/phap/ "Github")网站，确保你能够成功地切换语言*
 
 # Links
 [Github](https://github.com/DashBing/phap/ "Github") | [Pypi](https://pypi.org/project/phap/ "Pypi") | [Pypi (stralgo)](https://pypi.org/project/stralgo/ "Pypi (stralgo)")
 
 # Versions
@@ -38,15 +38,15 @@
 + v2.2.1
 
 ## Latest Available Version
 + v3.0.0
 
 ## Latest Version
 ### *(The data under the master branch is inaccurate. Please refer to the dev branch for details)*
-+ v3.1.0-alpha1
++ v3.1.0-alpha3
 
 # To Use
 ## Read our development document
 ### *(Click the [Github](https://github.com/DashBing/phap/ "Github") link to read this document，or you may can not to open the link)*
 + [Development Document](doc/README.md)
 
 # Build
```

### Comparing `phap-3.1.0a1/src/stralgo/__init__.py` & `phap-3.1.0a3/src/stralgo/__init__.py`

 * *Files identical despite different names*

### Comparing `phap-3.1.0a1/src/stralgo/base.py` & `phap-3.1.0a3/src/stralgo/base.py`

 * *Files identical despite different names*

### Comparing `phap-3.1.0a1/src/stralgo/hash/sm/sm3libs.py` & `phap-3.1.0a3/src/stralgo/hash/sm/sm3libs.py`

 * *Files identical despite different names*

