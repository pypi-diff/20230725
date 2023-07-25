# Comparing `tmp/readDataFile-0.0.3.tar.gz` & `tmp/readDataFile-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\readDataFile-0.0.3.tar", last modified: Tue Jul 25 05:33:20 2023, max compression
+gzip compressed data, was "dist\readDataFile-0.0.4.tar", last modified: Tue Jul 25 06:25:09 2023, max compression
```

## Comparing `readDataFile-0.0.3.tar` & `readDataFile-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 05:33:20.000000 readDataFile-0.0.3/
--rw-rw-rw-   0        0        0       22 2023-07-25 03:15:54.000000 readDataFile-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0      577 2023-07-25 05:33:20.000000 readDataFile-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       68 2023-07-25 03:15:25.000000 readDataFile-0.0.3/README.md
--rw-rw-rw-   0        0        0      108 2023-07-25 03:12:12.000000 readDataFile-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-25 05:33:20.000000 readDataFile-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      816 2023-07-25 05:28:16.000000 readDataFile-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 05:33:19.000000 readDataFile-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-25 05:33:20.000000 readDataFile-0.0.3/src/readDataFile/
--rw-rw-rw-   0        0        0     8423 2023-07-25 03:10:43.000000 readDataFile-0.0.3/src/readDataFile/ReadDataFile.py
--rw-rw-rw-   0        0        0     2349 2022-07-26 06:54:15.000000 readDataFile-0.0.3/src/readDataFile/_ListDelimiter_.py
--rw-rw-rw-   0        0        0        0 2023-07-25 02:59:37.000000 readDataFile-0.0.3/src/readDataFile/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 05:33:20.000000 readDataFile-0.0.3/src/readDataFile.egg-info/
--rw-rw-rw-   0        0        0      577 2023-07-25 05:33:19.000000 readDataFile-0.0.3/src/readDataFile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-07-25 05:33:19.000000 readDataFile-0.0.3/src/readDataFile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 05:33:19.000000 readDataFile-0.0.3/src/readDataFile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-25 05:33:19.000000 readDataFile-0.0.3/src/readDataFile.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 06:25:09.000000 readDataFile-0.0.4/
+-rw-rw-rw-   0        0        0       22 2023-07-25 03:15:54.000000 readDataFile-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      577 2023-07-25 06:25:09.000000 readDataFile-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       68 2023-07-25 03:15:25.000000 readDataFile-0.0.4/README.md
+-rw-rw-rw-   0        0        0      108 2023-07-25 03:12:12.000000 readDataFile-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-25 06:25:09.000000 readDataFile-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      816 2023-07-25 06:23:05.000000 readDataFile-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:25:09.000000 readDataFile-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-25 06:25:09.000000 readDataFile-0.0.4/src/readDataFile/
+-rw-rw-rw-   0        0        0     8423 2023-07-25 03:10:43.000000 readDataFile-0.0.4/src/readDataFile/ReadDataFile.py
+-rw-rw-rw-   0        0        0     2349 2022-07-26 06:54:15.000000 readDataFile-0.0.4/src/readDataFile/_ListDelimiter_.py
+-rw-rw-rw-   0        0        0       43 2023-07-25 06:24:45.000000 readDataFile-0.0.4/src/readDataFile/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:25:09.000000 readDataFile-0.0.4/src/readDataFile.egg-info/
+-rw-rw-rw-   0        0        0      577 2023-07-25 06:25:09.000000 readDataFile-0.0.4/src/readDataFile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-07-25 06:25:09.000000 readDataFile-0.0.4/src/readDataFile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 06:25:09.000000 readDataFile-0.0.4/src/readDataFile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-25 06:25:09.000000 readDataFile-0.0.4/src/readDataFile.egg-info/top_level.txt
```

### Comparing `readDataFile-0.0.3/PKG-INFO` & `readDataFile-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readDataFile
-Version: 0.0.3
+Version: 0.0.4
 Summary: uno test data file read
 Home-page: https://github.com/uunnooo/readUnoDataFile
 Author: Uno
 Author-email: uno0522@gmail.com
 Project-URL: Bug Tracker, https://github.com/uunnooo/readUnoDataFile
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `readDataFile-0.0.3/setup.py` & `readDataFile-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="readDataFile",
-    version="0.0.3",
+    version="0.0.4",
     author="Uno",
     author_email="uno0522@gmail.com",
     description="uno test data file read",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/uunnooo/readUnoDataFile",
     project_urls={
```

### Comparing `readDataFile-0.0.3/src/readDataFile/ReadDataFile.py` & `readDataFile-0.0.4/src/readDataFile/ReadDataFile.py`

 * *Files identical despite different names*

### Comparing `readDataFile-0.0.3/src/readDataFile/_ListDelimiter_.py` & `readDataFile-0.0.4/src/readDataFile/_ListDelimiter_.py`

 * *Files identical despite different names*

### Comparing `readDataFile-0.0.3/src/readDataFile.egg-info/PKG-INFO` & `readDataFile-0.0.4/src/readDataFile.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readDataFile
-Version: 0.0.3
+Version: 0.0.4
 Summary: uno test data file read
 Home-page: https://github.com/uunnooo/readUnoDataFile
 Author: Uno
 Author-email: uno0522@gmail.com
 Project-URL: Bug Tracker, https://github.com/uunnooo/readUnoDataFile
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

