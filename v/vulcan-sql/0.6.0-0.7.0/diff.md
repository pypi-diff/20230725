# Comparing `tmp/vulcan-sql-0.6.0.tar.gz` & `tmp/vulcan-sql-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulcan-sql-0.6.0.tar", last modified: Tue Jul 25 07:40:05 2023, max compression
+gzip compressed data, was "vulcan-sql-0.7.0.tar", last modified: Tue Jul 25 08:01:44 2023, max compression
```

## Comparing `vulcan-sql-0.6.0.tar` & `vulcan-sql-0.7.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 canner     (501) staff       (20)        0 2023-07-25 07:40:05.606351 vulcan-sql-0.6.0/
--rw-r--r--   0 canner     (501) staff       (20)      397 2023-07-04 06:26:29.000000 vulcan-sql-0.6.0/MANIFEST.in
--rw-r--r--   0 canner     (501) staff       (20)      937 2023-07-25 07:40:05.605981 vulcan-sql-0.6.0/PKG-INFO
--rw-r--r--   0 canner     (501) staff       (20)      542 2023-07-04 02:03:53.000000 vulcan-sql-0.6.0/PUBLIC_README.md
--rw-r--r--   0 canner     (501) staff       (20)     4197 2023-07-04 06:26:29.000000 vulcan-sql-0.6.0/README.md
--rw-r--r--   0 canner     (501) staff       (20)       38 2023-07-25 07:40:05.606460 vulcan-sql-0.6.0/setup.cfg
--rw-r--r--   0 canner     (501) staff       (20)     1143 2023-07-25 07:40:03.000000 vulcan-sql-0.6.0/setup.py
-drwxr-xr-x   0 canner     (501) staff       (20)        0 2023-07-25 07:40:05.604076 vulcan-sql-0.6.0/vulcan_sql.egg-info/
--rw-r--r--   0 canner     (501) staff       (20)      937 2023-07-25 07:40:05.000000 vulcan-sql-0.6.0/vulcan_sql.egg-info/PKG-INFO
--rw-r--r--   0 canner     (501) staff       (20)      259 2023-07-25 07:40:05.000000 vulcan-sql-0.6.0/vulcan_sql.egg-info/SOURCES.txt
--rw-r--r--   0 canner     (501) staff       (20)        1 2023-07-25 07:40:05.000000 vulcan-sql-0.6.0/vulcan_sql.egg-info/dependency_links.txt
--rw-r--r--   0 canner     (501) staff       (20)       52 2023-07-25 07:40:05.000000 vulcan-sql-0.6.0/vulcan_sql.egg-info/entry_points.txt
--rw-r--r--   0 canner     (501) staff       (20)       10 2023-07-25 07:40:05.000000 vulcan-sql-0.6.0/vulcan_sql.egg-info/top_level.txt
-drwxr-xr-x   0 canner     (501) staff       (20)        0 2023-07-25 07:40:05.605342 vulcan-sql-0.6.0/vulcansql/
--rw-r--r--   0 canner     (501) staff       (20)      170 2023-07-04 02:03:53.000000 vulcan-sql-0.6.0/vulcansql/__init__.py
--rw-r--r--   0 canner     (501) staff       (20)     2165 2023-07-25 07:37:13.000000 vulcan-sql-0.6.0/vulcansql/cli.py
+drwxr-xr-x   0 canner     (501) staff       (20)        0 2023-07-25 08:01:44.713948 vulcan-sql-0.7.0/
+-rw-r--r--   0 canner     (501) staff       (20)      397 2023-07-04 06:26:29.000000 vulcan-sql-0.7.0/MANIFEST.in
+-rw-r--r--   0 canner     (501) staff       (20)      937 2023-07-25 08:01:44.713514 vulcan-sql-0.7.0/PKG-INFO
+-rw-r--r--   0 canner     (501) staff       (20)      542 2023-07-04 02:03:53.000000 vulcan-sql-0.7.0/PUBLIC_README.md
+-rw-r--r--   0 canner     (501) staff       (20)     4312 2023-07-25 07:55:01.000000 vulcan-sql-0.7.0/README.md
+-rw-r--r--   0 canner     (501) staff       (20)       38 2023-07-25 08:01:44.714083 vulcan-sql-0.7.0/setup.cfg
+-rw-r--r--   0 canner     (501) staff       (20)     1143 2023-07-25 08:00:46.000000 vulcan-sql-0.7.0/setup.py
+drwxr-xr-x   0 canner     (501) staff       (20)        0 2023-07-25 08:01:44.710866 vulcan-sql-0.7.0/vulcan_sql.egg-info/
+-rw-r--r--   0 canner     (501) staff       (20)      937 2023-07-25 08:01:44.000000 vulcan-sql-0.7.0/vulcan_sql.egg-info/PKG-INFO
+-rw-r--r--   0 canner     (501) staff       (20)      259 2023-07-25 08:01:44.000000 vulcan-sql-0.7.0/vulcan_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 canner     (501) staff       (20)        1 2023-07-25 08:01:44.000000 vulcan-sql-0.7.0/vulcan_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 canner     (501) staff       (20)       52 2023-07-25 08:01:44.000000 vulcan-sql-0.7.0/vulcan_sql.egg-info/entry_points.txt
+-rw-r--r--   0 canner     (501) staff       (20)       10 2023-07-25 08:01:44.000000 vulcan-sql-0.7.0/vulcan_sql.egg-info/top_level.txt
+drwxr-xr-x   0 canner     (501) staff       (20)        0 2023-07-25 08:01:44.712454 vulcan-sql-0.7.0/vulcansql/
+-rw-r--r--   0 canner     (501) staff       (20)      170 2023-07-04 02:03:53.000000 vulcan-sql-0.7.0/vulcansql/__init__.py
+-rw-r--r--   0 canner     (501) staff       (20)     2147 2023-07-25 07:59:55.000000 vulcan-sql-0.7.0/vulcansql/cli.py
```

### Comparing `vulcan-sql-0.6.0/PKG-INFO` & `vulcan-sql-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-sql
-Version: 0.6.0
+Version: 0.7.0
 Summary: VulcanSQL turns your SQL templates into data APIs for efficient data sharing. No backend skills required. Empower your data sharing, faster.
 Home-page: https://github.com/Canner/vulcan-sql
 Author: Canner Team
 Author-email: contact@cannerdata.com
 License: Apache 2.0
 Requires-Python: >=3.0.0
 Description-Content-Type: text/markdown
```

### Comparing `vulcan-sql-0.6.0/PUBLIC_README.md` & `vulcan-sql-0.7.0/PUBLIC_README.md`

 * *Files identical despite different names*

### Comparing `vulcan-sql-0.6.0/README.md` & `vulcan-sql-0.7.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
 Because supporting python versions from `3.4.x` to `3.11.x`, it not easy to manage multiple python versions and switch it to test `pip install vulcan-sql`.
 
 Therefore, suggest to use the [pyenv](https://github.com/pyenv/pyenv) to test your Python package by using `pip install` on your local environment, please make sure you have switch to the version we supported.
 
 # Build
 
-Before starting to build, remember to update `version` in the `setup.py` and `pyproject.toml`.
+Before starting to build, **remember to update `version` in the `setup.py` and `pyproject.toml`**.
 
 ```bash
 # Removed old distribution
 $> rm -rf dist
 # Build source distribution (please follow the more detail about setuptools document)
 $> python setup.py sdist
 ```
@@ -83,10 +83,12 @@
 # Build and Publish
 
 After you finished the development and test would like to publish to remote repository like [pypi](https://pypi.org/project/canner-python-client/).
 
 ```sh
 # Removed old distribution
 $> rm -rf dist
+# Build source distribution (please follow the more detail about setuptools document)
+$> python setup.py sdist
 # upload to pypi and type account & password
 $>  twine upload dist/*
 ```
```

### Comparing `vulcan-sql-0.6.0/setup.py` & `vulcan-sql-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # read the contents of your README file
 directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(directory, "PUBLIC_README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup_kwargs = {
     'name': 'vulcan-sql',
-    'version': '0.6.0',
+    'version': '0.7.0',
     'description': 'VulcanSQL turns your SQL templates into data APIs for efficient data sharing. No backend skills required. Empower your data sharing, faster.',
     'long_description': long_description,
     'long_description_content_type': "text/markdown",
     'author': 'Canner Team',
     'author_email': 'contact@cannerdata.com',
     'license': "Apache 2.0",
     'url': 'https://github.com/Canner/vulcan-sql',
```

### Comparing `vulcan-sql-0.6.0/vulcan_sql.egg-info/PKG-INFO` & `vulcan-sql-0.7.0/vulcan_sql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-sql
-Version: 0.6.0
+Version: 0.7.0
 Summary: VulcanSQL turns your SQL templates into data APIs for efficient data sharing. No backend skills required. Empower your data sharing, faster.
 Home-page: https://github.com/Canner/vulcan-sql
 Author: Canner Team
 Author-email: contact@cannerdata.com
 License: Apache 2.0
 Requires-Python: >=3.0.0
 Description-Content-Type: text/markdown
```

### Comparing `vulcan-sql-0.6.0/vulcansql/cli.py` & `vulcan-sql-0.7.0/vulcansql/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 import tarfile
 import logging
 from urllib import request 
 # Set the log level by environment variable, default is INFO.
 LOGLEVEL = os.environ.get('PY_VULCAN_LOGLEVEL', 'INFO').upper()
 logging.basicConfig(level=LOGLEVEL)
 
-EXECUTABLE_SOURCE_URL = 'https://github.com/Canner/vulcan-sql/releases/download/v0.6.0/'
+EXECUTABLE_SOURCE_URL = 'https://github.com/Canner/vulcan-sql/releases/latest/download/'
 
 # The executable file name for different system.
 EXECUTABLE_FILES = {
-    "Windows": "vulcan.win.0.6.0.zip",
-    "Linux": "vulcan.linux.0.6.0.tar.gz",
-    "Darwin": "vulcan.osx.0.6.0.tar.gz",
+    "Windows": "vulcan.win.zip",
+    "Linux": "vulcan.linux.tar.gz",
+    "Darwin": "vulcan.osx.tar.gz",
 }
 
 
 def run_vulcan():
     system = platform.system()
     supported_systems = ["Linux", "Darwin", "Windows"]
```

