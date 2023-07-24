# Comparing `tmp/cachier-client-0.2.0.tar.gz` & `tmp/cachier-client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cachier-client-0.2.0.tar", last modified: Mon Jul 24 22:23:38 2023, max compression
+gzip compressed data, was "cachier-client-0.3.0.tar", last modified: Mon Jul 24 22:24:32 2023, max compression
```

## Comparing `cachier-client-0.2.0.tar` & `cachier-client-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 apinanyogaratnam   (501) staff       (20)        0 2023-07-24 22:23:38.678191 cachier-client-0.2.0/
--rw-r--r--   0 apinanyogaratnam   (501) staff       (20)     1057 2023-07-24 21:14:56.000000 cachier-client-0.2.0/LICENSE
--rw-r--r--   0 apinanyogaratnam   (501) staff       (20)     1883 2023-07-24 22:23:38.678058 cachier-client-0.2.0/PKG-INFO
--rw-r--r--   0 apinanyogaratnam   (501) staff       (20)     1423 2023-07-24 22:22:58.000000 cachier-client-0.2.0/README.md
-drwxr-xr-x   0 apinanyogaratnam   (501) staff       (20)        0 2023-07-24 22:23:38.677333 cachier-client-0.2.0/cachier_client/
--rw-r--r--   0 apinanyogaratnam   (501) staff       (20)      106 2023-07-24 22:13:57.000000 cachier-client-0.2.0/cachier_client/__init__.py
--rw-r--r--   0 apinanyogaratnam   (501) staff       (20)     3334 2023-07-24 22:11:42.000000 cachier-client-0.2.0/cachier_client/main.py
-drwxr-xr-x   0 apinanyogaratnam   (501) staff       (20)        0 2023-07-24 22:23:38.677870 cachier-client-0.2.0/cachier_client.egg-info/
--rw-r--r--   0 apinanyogaratnam   (501) staff       (20)     1883 2023-07-24 22:23:38.000000 cachier-client-0.2.0/cachier_client.egg-info/PKG-INFO
--rw-r--r--   0 apinanyogaratnam   (501) staff       (20)      243 2023-07-24 22:23:38.000000 cachier-client-0.2.0/cachier_client.egg-info/SOURCES.txt
--rw-r--r--   0 apinanyogaratnam   (501) staff       (20)        1 2023-07-24 22:23:38.000000 cachier-client-0.2.0/cachier_client.egg-info/dependency_links.txt
--rw-r--r--   0 apinanyogaratnam   (501) staff       (20)       15 2023-07-24 22:23:38.000000 cachier-client-0.2.0/cachier_client.egg-info/top_level.txt
--rw-r--r--   0 apinanyogaratnam   (501) staff       (20)      131 2023-07-24 21:14:56.000000 cachier-client-0.2.0/pyproject.toml
--rw-r--r--   0 apinanyogaratnam   (501) staff       (20)       38 2023-07-24 22:23:38.678236 cachier-client-0.2.0/setup.cfg
--rw-r--r--   0 apinanyogaratnam   (501) staff       (20)      699 2023-07-24 22:23:29.000000 cachier-client-0.2.0/setup.py
+drwxr-xr-x   0 apinanyogaratnam   (501) staff       (20)        0 2023-07-24 22:24:32.117514 cachier-client-0.3.0/
+-rw-r--r--   0 apinanyogaratnam   (501) staff       (20)     1057 2023-07-24 21:14:56.000000 cachier-client-0.3.0/LICENSE
+-rw-r--r--   0 apinanyogaratnam   (501) staff       (20)     1893 2023-07-24 22:24:32.117362 cachier-client-0.3.0/PKG-INFO
+-rw-r--r--   0 apinanyogaratnam   (501) staff       (20)     1433 2023-07-24 22:24:05.000000 cachier-client-0.3.0/README.md
+drwxr-xr-x   0 apinanyogaratnam   (501) staff       (20)        0 2023-07-24 22:24:32.116421 cachier-client-0.3.0/cachier_client/
+-rw-r--r--   0 apinanyogaratnam   (501) staff       (20)      106 2023-07-24 22:13:57.000000 cachier-client-0.3.0/cachier_client/__init__.py
+-rw-r--r--   0 apinanyogaratnam   (501) staff       (20)     3334 2023-07-24 22:11:42.000000 cachier-client-0.3.0/cachier_client/main.py
+drwxr-xr-x   0 apinanyogaratnam   (501) staff       (20)        0 2023-07-24 22:24:32.117162 cachier-client-0.3.0/cachier_client.egg-info/
+-rw-r--r--   0 apinanyogaratnam   (501) staff       (20)     1893 2023-07-24 22:24:32.000000 cachier-client-0.3.0/cachier_client.egg-info/PKG-INFO
+-rw-r--r--   0 apinanyogaratnam   (501) staff       (20)      243 2023-07-24 22:24:32.000000 cachier-client-0.3.0/cachier_client.egg-info/SOURCES.txt
+-rw-r--r--   0 apinanyogaratnam   (501) staff       (20)        1 2023-07-24 22:24:32.000000 cachier-client-0.3.0/cachier_client.egg-info/dependency_links.txt
+-rw-r--r--   0 apinanyogaratnam   (501) staff       (20)       15 2023-07-24 22:24:32.000000 cachier-client-0.3.0/cachier_client.egg-info/top_level.txt
+-rw-r--r--   0 apinanyogaratnam   (501) staff       (20)      131 2023-07-24 21:14:56.000000 cachier-client-0.3.0/pyproject.toml
+-rw-r--r--   0 apinanyogaratnam   (501) staff       (20)       38 2023-07-24 22:24:32.117560 cachier-client-0.3.0/setup.cfg
+-rw-r--r--   0 apinanyogaratnam   (501) staff       (20)      699 2023-07-24 22:24:23.000000 cachier-client-0.3.0/setup.py
```

### Comparing `cachier-client-0.2.0/LICENSE` & `cachier-client-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cachier-client-0.2.0/PKG-INFO` & `cachier-client-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cachier-client
-Version: 0.2.0
+Version: 0.3.0
 Summary: A cachier python client package
 Home-page: https://github.com/cachier-cache/cachier-python-client
 Author: apinanyogaratnam
 Author-email: apinanapinan@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,15 +27,15 @@
 - [Contributing](#contributing)
 
 ## Installation
 
 Install the package using pip:
 
 ```sh
-pip install base
+pip install cachier_client
 ```
 
 ## Usage
 
 ```python
 from cachier_client import CachierClient
```

### Comparing `cachier-client-0.2.0/README.md` & `cachier-client-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 - [Contributing](#contributing)
 
 ## Installation
 
 Install the package using pip:
 
 ```sh
-pip install base
+pip install cachier_client
 ```
 
 ## Usage
 
 ```python
 from cachier_client import CachierClient
```

### Comparing `cachier-client-0.2.0/cachier_client/main.py` & `cachier-client-0.3.0/cachier_client/main.py`

 * *Files identical despite different names*

### Comparing `cachier-client-0.2.0/cachier_client.egg-info/PKG-INFO` & `cachier-client-0.3.0/cachier_client.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cachier-client
-Version: 0.2.0
+Version: 0.3.0
 Summary: A cachier python client package
 Home-page: https://github.com/cachier-cache/cachier-python-client
 Author: apinanyogaratnam
 Author-email: apinanapinan@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,15 +27,15 @@
 - [Contributing](#contributing)
 
 ## Installation
 
 Install the package using pip:
 
 ```sh
-pip install base
+pip install cachier_client
 ```
 
 ## Usage
 
 ```python
 from cachier_client import CachierClient
```

### Comparing `cachier-client-0.2.0/setup.py` & `cachier-client-0.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="cachier-client",
-    version="0.2.0",
+    version="0.3.0",
     author="apinanyogaratnam",
     author_email="apinanapinan@icloud.com",
     description="A cachier python client package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cachier-cache/cachier-python-client",
     packages=setuptools.find_packages(),
```

