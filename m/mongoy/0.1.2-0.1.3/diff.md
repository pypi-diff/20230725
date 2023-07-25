# Comparing `tmp/mongoy-0.1.2.tar.gz` & `tmp/mongoy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongoy-0.1.2.tar", last modified: Tue Jul 25 16:44:04 2023, max compression
+gzip compressed data, was "mongoy-0.1.3.tar", last modified: Tue Jul 25 16:44:54 2023, max compression
```

## Comparing `mongoy-0.1.2.tar` & `mongoy-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 16:44:04.933522 mongoy-0.1.2/
--rw-rw-rw-   0        0        0     1067 2023-07-25 16:42:49.000000 mongoy-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     2052 2023-07-25 16:44:04.933522 mongoy-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1701 2023-07-25 16:42:49.000000 mongoy-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 16:44:04.909441 mongoy-0.1.2/mongoy/
--rw-rw-rw-   0        0        0        0 2023-07-25 16:43:10.000000 mongoy-0.1.2/mongoy/__init__.py
--rw-rw-rw-   0        0        0     4084 2023-07-25 16:42:49.000000 mongoy-0.1.2/mongoy/mongo.py
-drwxrwxrwx   0        0        0        0 2023-07-25 16:44:04.933522 mongoy-0.1.2/mongoy.egg-info/
--rw-rw-rw-   0        0        0     2052 2023-07-25 16:44:04.000000 mongoy-0.1.2/mongoy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-07-25 16:44:04.000000 mongoy-0.1.2/mongoy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 16:44:04.000000 mongoy-0.1.2/mongoy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-25 16:44:04.000000 mongoy-0.1.2/mongoy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-25 16:44:04.000000 mongoy-0.1.2/mongoy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 16:44:04.933522 mongoy-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1212 2023-07-25 16:43:59.000000 mongoy-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 16:44:54.285753 mongoy-0.1.3/
+-rw-rw-rw-   0        0        0     1067 2023-07-25 16:42:49.000000 mongoy-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     2052 2023-07-25 16:44:54.285753 mongoy-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1701 2023-07-25 16:42:49.000000 mongoy-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 16:44:54.261745 mongoy-0.1.3/mongoy/
+-rw-rw-rw-   0        0        0        0 2023-07-25 16:43:10.000000 mongoy-0.1.3/mongoy/__init__.py
+-rw-rw-rw-   0        0        0     4084 2023-07-25 16:42:49.000000 mongoy-0.1.3/mongoy/mongo.py
+drwxrwxrwx   0        0        0        0 2023-07-25 16:44:54.277749 mongoy-0.1.3/mongoy.egg-info/
+-rw-rw-rw-   0        0        0     2052 2023-07-25 16:44:53.000000 mongoy-0.1.3/mongoy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-07-25 16:44:54.000000 mongoy-0.1.3/mongoy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 16:44:53.000000 mongoy-0.1.3/mongoy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-25 16:44:53.000000 mongoy-0.1.3/mongoy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-25 16:44:53.000000 mongoy-0.1.3/mongoy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 16:44:54.285753 mongoy-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1212 2023-07-25 16:44:48.000000 mongoy-0.1.3/setup.py
```

### Comparing `mongoy-0.1.2/LICENSE` & `mongoy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mongoy-0.1.2/PKG-INFO` & `mongoy-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongoy
-Version: 0.1.2
+Version: 0.1.3
 Summary: wrapper utility for mongodb
 Author: pavittarx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `mongoy-0.1.2/README.md` & `mongoy-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `mongoy-0.1.2/mongoy/mongo.py` & `mongoy-0.1.3/mongoy/mongo.py`

 * *Files identical despite different names*

### Comparing `mongoy-0.1.2/mongoy.egg-info/PKG-INFO` & `mongoy-0.1.3/mongoy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongoy
-Version: 0.1.2
+Version: 0.1.3
 Summary: wrapper utility for mongodb
 Author: pavittarx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `mongoy-0.1.2/setup.py` & `mongoy-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mongoy",                     # This is the name of the package
-    version="0.1.2",                        # The initial release version
+    version="0.1.3",                        # The initial release version
     author="pavittarx",                     # Full name of the author
     description="wrapper utility for mongodb",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

