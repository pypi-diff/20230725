# Comparing `tmp/influxdb3-python-0.2.0.tar.gz` & `tmp/influxdb3-python-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "influxdb3-python-0.2.0.tar", last modified: Tue Jul 18 14:10:15 2023, max compression
+gzip compressed data, was "influxdb3-python-0.2.1.tar", last modified: Tue Jul 25 12:08:45 2023, max compression
```

## Comparing `influxdb3-python-0.2.0.tar` & `influxdb3-python-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:10:15.302862 influxdb3-python-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-18 14:10:03.000000 influxdb3-python-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-07-18 14:10:15.302862 influxdb3-python-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-07-18 14:10:03.000000 influxdb3-python-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:10:15.302862 influxdb3-python-0.2.0/influxdb3_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-07-18 14:10:15.000000 influxdb3-python-0.2.0/influxdb3_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-18 14:10:15.000000 influxdb3-python-0.2.0/influxdb3_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:10:15.000000 influxdb3-python-0.2.0/influxdb3_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-18 14:10:15.000000 influxdb3-python-0.2.0/influxdb3_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-18 14:10:15.000000 influxdb3-python-0.2.0/influxdb3_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:10:15.302862 influxdb3-python-0.2.0/influxdb_client_3/
--rw-r--r--   0 runner    (1001) docker     (123)     8788 2023-07-18 14:10:03.000000 influxdb3-python-0.2.0/influxdb_client_3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-18 14:10:03.000000 influxdb3-python-0.2.0/influxdb_client_3/read_file.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:10:15.302862 influxdb3-python-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-18 14:10:03.000000 influxdb3-python-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:10:15.302862 influxdb3-python-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-18 14:10:03.000000 influxdb3-python-0.2.0/tests/test_influxdb_client_3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:08:45.554245 influxdb3-python-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 12:08:27.000000 influxdb3-python-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-07-25 12:08:45.554245 influxdb3-python-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-07-25 12:08:27.000000 influxdb3-python-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:08:45.554245 influxdb3-python-0.2.1/influxdb3_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-07-25 12:08:45.000000 influxdb3-python-0.2.1/influxdb3_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-25 12:08:45.000000 influxdb3-python-0.2.1/influxdb3_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 12:08:45.000000 influxdb3-python-0.2.1/influxdb3_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-25 12:08:45.000000 influxdb3-python-0.2.1/influxdb3_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-25 12:08:45.000000 influxdb3-python-0.2.1/influxdb3_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:08:45.554245 influxdb3-python-0.2.1/influxdb_client_3/
+-rw-r--r--   0 runner    (1001) docker     (123)     8788 2023-07-25 12:08:27.000000 influxdb3-python-0.2.1/influxdb_client_3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-25 12:08:27.000000 influxdb3-python-0.2.1/influxdb_client_3/read_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 12:08:45.554245 influxdb3-python-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-25 12:08:27.000000 influxdb3-python-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:08:45.554245 influxdb3-python-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-25 12:08:27.000000 influxdb3-python-0.2.1/tests/test_influxdb_client_3.py
```

### Comparing `influxdb3-python-0.2.0/LICENSE` & `influxdb3-python-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.2.0/PKG-INFO` & `influxdb3-python-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: influxdb3-python
-Version: 0.2.0
+Version: 0.2.1
 Summary: Community Python client for InfluxDB 3.0
 Home-page: https://github.com/InfluxCommunity/influxdb3-python
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+Provides-Extra: pandas
 License-File: LICENSE
 
 <p align="center">
     <img src="https://github.com/InfluxCommunity/influxdb3-python/blob/main/python-logo.png?raw=true" alt="Your Image" width="150px">
 </p>
 
 <p align="center">
@@ -42,30 +43,42 @@
 # InfluxDB 3.0 Python Client
 ## Introduction
 
 `influxdb_client_3` is a Python module that provides a simple and convenient way to interact with InfluxDB 3.0. This module supports both writing data to InfluxDB and querying data using the Flight client, which allows you to execute SQL and InfluxQL queries on InfluxDB 3.0.
 
 ## Dependencies
 
-- `pyarrow`
-- `influxdb-client`
+- `pyarrow` (automatically installed)
+- `influxdb-client` (automatically installed)
+- `pandas` (optional)
   
-*These are installed as part of the package*
 
 ## Installation
 
 You can install 'influxdb3-python' using `pip`:
 
 ```bash
 pip install influxdb3-python
 ```
 
+Note: This does not include Pandas support. If you would like to use key features such as `to_pandas()`  and `write_file()` you will need to install `pandas` separately.
+
+```bash
+pip install influxdb3-python[pandas]
+```
+or
+```bash
+pip install pandas
+```
+
 *Note: Please make sure you are using 3.6 or above. For the best performance use 3.11+*
 
 # Usage
+One of the easiest ways to get started is to checkout the ["Pokemon-Trainer cookbook"](Examples/pokemon-trainer/cookbook.ipynb). This scenario takes you through the basics of both the client library and Pyarrow.
+
 ## Importing the Module
 ```python
 from influxdb_client_3 import InfluxDBClient3, Point
 ```
 
 ## Initialization
 If you are using InfluxDB Cloud, then you should note that:
```

### Comparing `influxdb3-python-0.2.0/README.md` & `influxdb3-python-0.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -23,30 +23,42 @@
 # InfluxDB 3.0 Python Client
 ## Introduction
 
 `influxdb_client_3` is a Python module that provides a simple and convenient way to interact with InfluxDB 3.0. This module supports both writing data to InfluxDB and querying data using the Flight client, which allows you to execute SQL and InfluxQL queries on InfluxDB 3.0.
 
 ## Dependencies
 
-- `pyarrow`
-- `influxdb-client`
+- `pyarrow` (automatically installed)
+- `influxdb-client` (automatically installed)
+- `pandas` (optional)
   
-*These are installed as part of the package*
 
 ## Installation
 
 You can install 'influxdb3-python' using `pip`:
 
 ```bash
 pip install influxdb3-python
 ```
 
+Note: This does not include Pandas support. If you would like to use key features such as `to_pandas()`  and `write_file()` you will need to install `pandas` separately.
+
+```bash
+pip install influxdb3-python[pandas]
+```
+or
+```bash
+pip install pandas
+```
+
 *Note: Please make sure you are using 3.6 or above. For the best performance use 3.11+*
 
 # Usage
+One of the easiest ways to get started is to checkout the ["Pokemon-Trainer cookbook"](Examples/pokemon-trainer/cookbook.ipynb). This scenario takes you through the basics of both the client library and Pyarrow.
+
 ## Importing the Module
 ```python
 from influxdb_client_3 import InfluxDBClient3, Point
 ```
 
 ## Initialization
 If you are using InfluxDB Cloud, then you should note that:
```

### Comparing `influxdb3-python-0.2.0/influxdb3_python.egg-info/PKG-INFO` & `influxdb3-python-0.2.1/influxdb3_python.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: influxdb3-python
-Version: 0.2.0
+Version: 0.2.1
 Summary: Community Python client for InfluxDB 3.0
 Home-page: https://github.com/InfluxCommunity/influxdb3-python
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+Provides-Extra: pandas
 License-File: LICENSE
 
 <p align="center">
     <img src="https://github.com/InfluxCommunity/influxdb3-python/blob/main/python-logo.png?raw=true" alt="Your Image" width="150px">
 </p>
 
 <p align="center">
@@ -42,30 +43,42 @@
 # InfluxDB 3.0 Python Client
 ## Introduction
 
 `influxdb_client_3` is a Python module that provides a simple and convenient way to interact with InfluxDB 3.0. This module supports both writing data to InfluxDB and querying data using the Flight client, which allows you to execute SQL and InfluxQL queries on InfluxDB 3.0.
 
 ## Dependencies
 
-- `pyarrow`
-- `influxdb-client`
+- `pyarrow` (automatically installed)
+- `influxdb-client` (automatically installed)
+- `pandas` (optional)
   
-*These are installed as part of the package*
 
 ## Installation
 
 You can install 'influxdb3-python' using `pip`:
 
 ```bash
 pip install influxdb3-python
 ```
 
+Note: This does not include Pandas support. If you would like to use key features such as `to_pandas()`  and `write_file()` you will need to install `pandas` separately.
+
+```bash
+pip install influxdb3-python[pandas]
+```
+or
+```bash
+pip install pandas
+```
+
 *Note: Please make sure you are using 3.6 or above. For the best performance use 3.11+*
 
 # Usage
+One of the easiest ways to get started is to checkout the ["Pokemon-Trainer cookbook"](Examples/pokemon-trainer/cookbook.ipynb). This scenario takes you through the basics of both the client library and Pyarrow.
+
 ## Importing the Module
 ```python
 from influxdb_client_3 import InfluxDBClient3, Point
 ```
 
 ## Initialization
 If you are using InfluxDB Cloud, then you should note that:
```

### Comparing `influxdb3-python-0.2.0/influxdb_client_3/__init__.py` & `influxdb3-python-0.2.1/influxdb_client_3/__init__.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.2.0/influxdb_client_3/read_file.py` & `influxdb3-python-0.2.1/influxdb_client_3/read_file.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import pyarrow.csv as csv
 import pyarrow.feather as feather
 import pyarrow.parquet as parquet
-import pandas as pd
+
+
+
 
 # Check if the OS is not Windows
 if os.name != 'nt':
     import pyarrow.orc as orc
 
 
 class UploadFile:
@@ -17,14 +19,19 @@
         """
         Initialize an UploadFile instance.
 
         :param file: The file to upload.
         :type file: str
         :param kwargs: Additional arguments for file loading functions.
         """
+        try:
+            import pandas as pd
+        except ImportError:
+            raise ImportError("Pandas is required for write_file(). Please install it using 'pip install pandas' or 'pip install influxdb3-python[pandas]'")
+
         self._file = file
         self._kwargs = file_parser_options if file_parser_options is not None else {}
 
     def load_file(self):
         """
         Load a file based on its extension.
```

### Comparing `influxdb3-python-0.2.0/setup.py` & `influxdb3-python-0.2.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     description='Community Python client for InfluxDB 3.0',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='InfluxData',
     author_email='contact@influxdata.com',
     url='https://github.com/InfluxCommunity/influxdb3-python',
     packages=['influxdb_client_3'],
+    extras_require={'pandas': ['pandas']},
     install_requires=['pyarrow','influxdb-client'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
```

### Comparing `influxdb3-python-0.2.0/tests/test_influxdb_client_3.py` & `influxdb3-python-0.2.1/tests/test_influxdb_client_3.py`

 * *Files identical despite different names*

