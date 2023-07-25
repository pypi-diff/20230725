# Comparing `tmp/readDataFile-0.0.5.tar.gz` & `tmp/readDataFile-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\readDataFile-0.0.5.tar", last modified: Tue Jul 25 06:33:26 2023, max compression
+gzip compressed data, was "dist\readDataFile-0.0.6.tar", last modified: Tue Jul 25 07:00:01 2023, max compression
```

## Comparing `readDataFile-0.0.5.tar` & `readDataFile-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 06:33:26.000000 readDataFile-0.0.5/
--rw-rw-rw-   0        0        0       22 2023-07-25 03:15:54.000000 readDataFile-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      577 2023-07-25 06:33:26.000000 readDataFile-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       68 2023-07-25 03:15:25.000000 readDataFile-0.0.5/README.md
--rw-rw-rw-   0        0        0      108 2023-07-25 03:12:12.000000 readDataFile-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-25 06:33:26.000000 readDataFile-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      816 2023-07-25 06:33:21.000000 readDataFile-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 06:33:26.000000 readDataFile-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-07-25 06:33:26.000000 readDataFile-0.0.5/src/readDataFile/
--rw-rw-rw-   0        0        0     8423 2023-07-25 03:10:43.000000 readDataFile-0.0.5/src/readDataFile/ReadDataFile.py
--rw-rw-rw-   0        0        0     2349 2022-07-26 06:54:15.000000 readDataFile-0.0.5/src/readDataFile/_ListDelimiter_.py
--rw-rw-rw-   0        0        0       57 2023-07-25 06:31:02.000000 readDataFile-0.0.5/src/readDataFile/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 06:33:26.000000 readDataFile-0.0.5/src/readDataFile.egg-info/
--rw-rw-rw-   0        0        0      577 2023-07-25 06:33:26.000000 readDataFile-0.0.5/src/readDataFile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-07-25 06:33:26.000000 readDataFile-0.0.5/src/readDataFile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 06:33:26.000000 readDataFile-0.0.5/src/readDataFile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-25 06:33:26.000000 readDataFile-0.0.5/src/readDataFile.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 07:00:01.000000 readDataFile-0.0.6/
+-rw-rw-rw-   0        0        0       22 2023-07-25 03:15:54.000000 readDataFile-0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      577 2023-07-25 07:00:01.000000 readDataFile-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       68 2023-07-25 03:15:25.000000 readDataFile-0.0.6/README.md
+-rw-rw-rw-   0        0        0      108 2023-07-25 03:12:12.000000 readDataFile-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-25 07:00:01.000000 readDataFile-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      816 2023-07-25 06:55:02.000000 readDataFile-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 07:00:01.000000 readDataFile-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-25 07:00:01.000000 readDataFile-0.0.6/src/readDataFile/
+-rw-rw-rw-   0        0        0     8424 2023-07-25 06:54:41.000000 readDataFile-0.0.6/src/readDataFile/ReadDataFile.py
+-rw-rw-rw-   0        0        0     2349 2022-07-26 06:54:15.000000 readDataFile-0.0.6/src/readDataFile/_ListDelimiter_.py
+-rw-rw-rw-   0        0        0       57 2023-07-25 06:31:02.000000 readDataFile-0.0.6/src/readDataFile/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 07:00:01.000000 readDataFile-0.0.6/src/readDataFile.egg-info/
+-rw-rw-rw-   0        0        0      577 2023-07-25 07:00:01.000000 readDataFile-0.0.6/src/readDataFile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-07-25 07:00:01.000000 readDataFile-0.0.6/src/readDataFile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 07:00:01.000000 readDataFile-0.0.6/src/readDataFile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-25 07:00:01.000000 readDataFile-0.0.6/src/readDataFile.egg-info/top_level.txt
```

### Comparing `readDataFile-0.0.5/PKG-INFO` & `readDataFile-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readDataFile
-Version: 0.0.5
+Version: 0.0.6
 Summary: uno test data file read
 Home-page: https://github.com/uunnooo/readUnoDataFile
 Author: Uno
 Author-email: uno0522@gmail.com
 Project-URL: Bug Tracker, https://github.com/uunnooo/readUnoDataFile
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `readDataFile-0.0.5/setup.py` & `readDataFile-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="readDataFile",
-    version="0.0.5",
+    version="0.0.6",
     author="Uno",
     author_email="uno0522@gmail.com",
     description="uno test data file read",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/uunnooo/readUnoDataFile",
     project_urls={
```

### Comparing `readDataFile-0.0.5/src/readDataFile/ReadDataFile.py` & `readDataFile-0.0.6/src/readDataFile/ReadDataFile.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     """
     :param RawData:
     :param lineNum:
     :return:
     """
 
     import pandas as pd
-    from _ListDelimiter_ import funcFindDelimiter
+    from ._ListDelimiter_ import funcFindDelimiter
 
     # 라인에 대한 넘버 정보 하나일때, 즉 데이터 정의나 단위 정보일때
     if len(lineNum) < 2 :
         listLineNum = [lineNum[0], lineNum[0] + 1]
         # 형을 맞춰주기 위함
         lineData = RawData.iloc[listLineNum[0]: listLineNum[1], 0].str.rstrip()
         separator = funcFindDelimiter(lineData)
```

### Comparing `readDataFile-0.0.5/src/readDataFile/_ListDelimiter_.py` & `readDataFile-0.0.6/src/readDataFile/_ListDelimiter_.py`

 * *Files identical despite different names*

### Comparing `readDataFile-0.0.5/src/readDataFile.egg-info/PKG-INFO` & `readDataFile-0.0.6/src/readDataFile.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readDataFile
-Version: 0.0.5
+Version: 0.0.6
 Summary: uno test data file read
 Home-page: https://github.com/uunnooo/readUnoDataFile
 Author: Uno
 Author-email: uno0522@gmail.com
 Project-URL: Bug Tracker, https://github.com/uunnooo/readUnoDataFile
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

