# Comparing `tmp/vulcan-sql-0.5.3.tar.gz` & `tmp/vulcan-sql-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vulcan-sql-0.5.3.tar", last modified: Tue Jul  4 05:01:56 2023, max compression
+gzip compressed data, was "vulcan-sql-0.6.0.tar", last modified: Tue Jul 25 07:40:05 2023, max compression
```

## Comparing `vulcan-sql-0.5.3.tar` & `vulcan-sql-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 canner     (501) staff       (20)        0 2023-07-04 05:01:56.789948 vulcan-sql-0.5.3/
--rw-r--r--   0 canner     (501) staff       (20)      397 2023-07-04 02:18:20.000000 vulcan-sql-0.5.3/MANIFEST.in
--rw-r--r--   0 canner     (501) staff       (20)     1112 2023-07-04 05:01:56.789089 vulcan-sql-0.5.3/PKG-INFO
--rw-r--r--   0 canner     (501) staff       (20)      542 2023-07-04 02:03:53.000000 vulcan-sql-0.5.3/PUBLIC_README.md
--rw-r--r--   0 canner     (501) staff       (20)     4197 2023-07-04 02:20:38.000000 vulcan-sql-0.5.3/README.md
--rw-r--r--   0 canner     (501) staff       (20)       38 2023-07-04 05:01:56.790202 vulcan-sql-0.5.3/setup.cfg
--rw-r--r--   0 canner     (501) staff       (20)     1143 2023-07-04 05:01:47.000000 vulcan-sql-0.5.3/setup.py
-drwxr-xr-x   0 canner     (501) staff       (20)        0 2023-07-04 05:01:56.786702 vulcan-sql-0.5.3/vulcan_sql.egg-info/
--rw-r--r--   0 canner     (501) staff       (20)     1112 2023-07-04 05:01:56.000000 vulcan-sql-0.5.3/vulcan_sql.egg-info/PKG-INFO
--rw-r--r--   0 canner     (501) staff       (20)      259 2023-07-04 05:01:56.000000 vulcan-sql-0.5.3/vulcan_sql.egg-info/SOURCES.txt
--rw-r--r--   0 canner     (501) staff       (20)        1 2023-07-04 05:01:56.000000 vulcan-sql-0.5.3/vulcan_sql.egg-info/dependency_links.txt
--rw-r--r--   0 canner     (501) staff       (20)       53 2023-07-04 05:01:56.000000 vulcan-sql-0.5.3/vulcan_sql.egg-info/entry_points.txt
--rw-r--r--   0 canner     (501) staff       (20)       10 2023-07-04 05:01:56.000000 vulcan-sql-0.5.3/vulcan_sql.egg-info/top_level.txt
-drwxr-xr-x   0 canner     (501) staff       (20)        0 2023-07-04 05:01:56.788220 vulcan-sql-0.5.3/vulcansql/
--rw-r--r--   0 canner     (501) staff       (20)      170 2023-07-04 02:03:53.000000 vulcan-sql-0.5.3/vulcansql/__init__.py
--rw-r--r--   0 canner     (501) staff       (20)     2145 2023-07-04 03:10:48.000000 vulcan-sql-0.5.3/vulcansql/cli.py
+drwxr-xr-x   0 canner     (501) staff       (20)        0 2023-07-25 07:40:05.606351 vulcan-sql-0.6.0/
+-rw-r--r--   0 canner     (501) staff       (20)      397 2023-07-04 06:26:29.000000 vulcan-sql-0.6.0/MANIFEST.in
+-rw-r--r--   0 canner     (501) staff       (20)      937 2023-07-25 07:40:05.605981 vulcan-sql-0.6.0/PKG-INFO
+-rw-r--r--   0 canner     (501) staff       (20)      542 2023-07-04 02:03:53.000000 vulcan-sql-0.6.0/PUBLIC_README.md
+-rw-r--r--   0 canner     (501) staff       (20)     4197 2023-07-04 06:26:29.000000 vulcan-sql-0.6.0/README.md
+-rw-r--r--   0 canner     (501) staff       (20)       38 2023-07-25 07:40:05.606460 vulcan-sql-0.6.0/setup.cfg
+-rw-r--r--   0 canner     (501) staff       (20)     1143 2023-07-25 07:40:03.000000 vulcan-sql-0.6.0/setup.py
+drwxr-xr-x   0 canner     (501) staff       (20)        0 2023-07-25 07:40:05.604076 vulcan-sql-0.6.0/vulcan_sql.egg-info/
+-rw-r--r--   0 canner     (501) staff       (20)      937 2023-07-25 07:40:05.000000 vulcan-sql-0.6.0/vulcan_sql.egg-info/PKG-INFO
+-rw-r--r--   0 canner     (501) staff       (20)      259 2023-07-25 07:40:05.000000 vulcan-sql-0.6.0/vulcan_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 canner     (501) staff       (20)        1 2023-07-25 07:40:05.000000 vulcan-sql-0.6.0/vulcan_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 canner     (501) staff       (20)       52 2023-07-25 07:40:05.000000 vulcan-sql-0.6.0/vulcan_sql.egg-info/entry_points.txt
+-rw-r--r--   0 canner     (501) staff       (20)       10 2023-07-25 07:40:05.000000 vulcan-sql-0.6.0/vulcan_sql.egg-info/top_level.txt
+drwxr-xr-x   0 canner     (501) staff       (20)        0 2023-07-25 07:40:05.605342 vulcan-sql-0.6.0/vulcansql/
+-rw-r--r--   0 canner     (501) staff       (20)      170 2023-07-04 02:03:53.000000 vulcan-sql-0.6.0/vulcansql/__init__.py
+-rw-r--r--   0 canner     (501) staff       (20)     2165 2023-07-25 07:37:13.000000 vulcan-sql-0.6.0/vulcansql/cli.py
```

### Comparing `vulcan-sql-0.5.3/PKG-INFO` & `vulcan-sql-0.6.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: vulcan-sql
-Version: 0.5.3
+Version: 0.6.0
 Summary: VulcanSQL turns your SQL templates into data APIs for efficient data sharing. No backend skills required. Empower your data sharing, faster.
 Home-page: https://github.com/Canner/vulcan-sql
 Author: Canner Team
 Author-email: contact@cannerdata.com
 License: Apache 2.0
-Description: # Introduction
-        
-        The package provide the python `pip install` method to install VulcanSQL. currently support Python version from `3.3.x` to `3.11.x`.
-        
-        # What is VulcanSQL
-        
-        VulcanSQL turns your SQL templates into data APIs for efficient data sharing. No backend skills required. Empower your data sharing, faster.
-        
-        For more introduction please see [VulcanSQL Official Website](https://vulcansql.com/).
-        
-        # Installation
-        
-        Install VulcanSQL by pip and then you could use VulcanSQL by `vulcan`.
-        
-        ```bash
-        $ pip install vulcan-sql
-        $ vulcan --help
-        ```
-        
-Platform: UNKNOWN
 Requires-Python: >=3.0.0
 Description-Content-Type: text/markdown
+
+# Introduction
+
+The package provide the python `pip install` method to install VulcanSQL. currently support Python version from `3.3.x` to `3.11.x`.
+
+# What is VulcanSQL
+
+VulcanSQL turns your SQL templates into data APIs for efficient data sharing. No backend skills required. Empower your data sharing, faster.
+
+For more introduction please see [VulcanSQL Official Website](https://vulcansql.com/).
+
+# Installation
+
+Install VulcanSQL by pip and then you could use VulcanSQL by `vulcan`.
+
+```bash
+$ pip install vulcan-sql
+$ vulcan --help
+```
```

### Comparing `vulcan-sql-0.5.3/PUBLIC_README.md` & `vulcan-sql-0.6.0/PUBLIC_README.md`

 * *Files identical despite different names*

### Comparing `vulcan-sql-0.5.3/README.md` & `vulcan-sql-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `vulcan-sql-0.5.3/setup.py` & `vulcan-sql-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # read the contents of your README file
 directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(directory, "PUBLIC_README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup_kwargs = {
     'name': 'vulcan-sql',
-    'version': '0.5.3',
+    'version': '0.6.0',
     'description': 'VulcanSQL turns your SQL templates into data APIs for efficient data sharing. No backend skills required. Empower your data sharing, faster.',
     'long_description': long_description,
     'long_description_content_type': "text/markdown",
     'author': 'Canner Team',
     'author_email': 'contact@cannerdata.com',
     'license': "Apache 2.0",
     'url': 'https://github.com/Canner/vulcan-sql',
```

### Comparing `vulcan-sql-0.5.3/vulcan_sql.egg-info/PKG-INFO` & `vulcan-sql-0.6.0/vulcan_sql.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: vulcan-sql
-Version: 0.5.3
+Version: 0.6.0
 Summary: VulcanSQL turns your SQL templates into data APIs for efficient data sharing. No backend skills required. Empower your data sharing, faster.
 Home-page: https://github.com/Canner/vulcan-sql
 Author: Canner Team
 Author-email: contact@cannerdata.com
 License: Apache 2.0
-Description: # Introduction
-        
-        The package provide the python `pip install` method to install VulcanSQL. currently support Python version from `3.3.x` to `3.11.x`.
-        
-        # What is VulcanSQL
-        
-        VulcanSQL turns your SQL templates into data APIs for efficient data sharing. No backend skills required. Empower your data sharing, faster.
-        
-        For more introduction please see [VulcanSQL Official Website](https://vulcansql.com/).
-        
-        # Installation
-        
-        Install VulcanSQL by pip and then you could use VulcanSQL by `vulcan`.
-        
-        ```bash
-        $ pip install vulcan-sql
-        $ vulcan --help
-        ```
-        
-Platform: UNKNOWN
 Requires-Python: >=3.0.0
 Description-Content-Type: text/markdown
+
+# Introduction
+
+The package provide the python `pip install` method to install VulcanSQL. currently support Python version from `3.3.x` to `3.11.x`.
+
+# What is VulcanSQL
+
+VulcanSQL turns your SQL templates into data APIs for efficient data sharing. No backend skills required. Empower your data sharing, faster.
+
+For more introduction please see [VulcanSQL Official Website](https://vulcansql.com/).
+
+# Installation
+
+Install VulcanSQL by pip and then you could use VulcanSQL by `vulcan`.
+
+```bash
+$ pip install vulcan-sql
+$ vulcan --help
+```
```

### Comparing `vulcan-sql-0.5.3/vulcansql/cli.py` & `vulcan-sql-0.6.0/vulcansql/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 import tarfile
 import logging
 from urllib import request 
 # Set the log level by environment variable, default is INFO.
 LOGLEVEL = os.environ.get('PY_VULCAN_LOGLEVEL', 'INFO').upper()
 logging.basicConfig(level=LOGLEVEL)
 
-EXECUTABLE_SOURCE_URL = 'https://d3jr9lxbk67t5c.cloudfront.net/bin/'
+EXECUTABLE_SOURCE_URL = 'https://github.com/Canner/vulcan-sql/releases/download/v0.6.0/'
 
 # The executable file name for different system.
 EXECUTABLE_FILES = {
-    "Windows": "vulcan.win.0.5.3.zip",
-    "Linux": "vulcan.linux.0.5.3.tar.gz",
-    "Darwin": "vulcan.osx.0.5.3.tar.gz",
+    "Windows": "vulcan.win.0.6.0.zip",
+    "Linux": "vulcan.linux.0.6.0.tar.gz",
+    "Darwin": "vulcan.osx.0.6.0.tar.gz",
 }
 
 
 def run_vulcan():
     system = platform.system()
     supported_systems = ["Linux", "Darwin", "Windows"]
```

