# Comparing `tmp/cwtune-0.1.8.tar.gz` & `tmp/cwtune-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cwtune-0.1.8.tar", last modified: Tue Jul 25 12:38:55 2023, max compression
+gzip compressed data, was "cwtune-0.1.9.tar", last modified: Tue Jul 25 12:45:48 2023, max compression
```

## Comparing `cwtune-0.1.8.tar` & `cwtune-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-07-25 12:38:55.149937 cwtune-0.1.8/
--rw-r--r--   0 arran      (501) staff       (20)     1204 2023-07-25 11:17:40.000000 cwtune-0.1.8/.gitignore
--rw-r--r--   0 arran      (501) staff       (20)     1070 2023-07-25 11:24:31.000000 cwtune-0.1.8/LICENSE
--rw-r--r--   0 arran      (501) staff       (20)     1531 2023-07-25 12:38:55.150380 cwtune-0.1.8/PKG-INFO
--rw-r--r--   0 arran      (501) staff       (20)      860 2023-07-11 11:02:07.000000 cwtune-0.1.8/README.rst
-drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-07-25 12:38:55.133182 cwtune-0.1.8/cwtune/
--rw-r--r--   0 arran      (501) staff       (20)      123 2023-07-11 11:02:07.000000 cwtune-0.1.8/cwtune/__init__.py
--rw-r--r--   0 arran      (501) staff       (20)     5599 2023-07-25 10:25:39.000000 cwtune-0.1.8/cwtune/aws.py
--rw-r--r--   0 arran      (501) staff       (20)     1247 2023-07-25 12:37:56.000000 cwtune-0.1.8/cwtune/cli.py
--rw-r--r--   0 arran      (501) staff       (20)     9126 2023-07-25 10:19:06.000000 cwtune-0.1.8/cwtune/cwtune.py
--rw-r--r--   0 arran      (501) staff       (20)     2400 2023-07-24 12:37:41.000000 cwtune-0.1.8/cwtune/timeseries.py
--rw-r--r--   0 arran      (501) staff       (20)     2760 2023-07-24 10:43:29.000000 cwtune-0.1.8/cwtune/utils.py
-drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-07-25 12:38:55.141467 cwtune-0.1.8/cwtune.egg-info/
--rw-r--r--   0 arran      (501) staff       (20)     1531 2023-07-25 12:38:54.000000 cwtune-0.1.8/cwtune.egg-info/PKG-INFO
--rw-r--r--   0 arran      (501) staff       (20)      564 2023-07-25 12:38:55.000000 cwtune-0.1.8/cwtune.egg-info/SOURCES.txt
--rw-r--r--   0 arran      (501) staff       (20)        1 2023-07-25 12:38:54.000000 cwtune-0.1.8/cwtune.egg-info/dependency_links.txt
--rw-r--r--   0 arran      (501) staff       (20)       43 2023-07-25 12:38:54.000000 cwtune-0.1.8/cwtune.egg-info/entry_points.txt
--rw-r--r--   0 arran      (501) staff       (20)        1 2023-07-25 11:33:06.000000 cwtune-0.1.8/cwtune.egg-info/not-zip-safe
--rw-r--r--   0 arran      (501) staff       (20)       65 2023-07-25 12:38:54.000000 cwtune-0.1.8/cwtune.egg-info/requires.txt
--rw-r--r--   0 arran      (501) staff       (20)        7 2023-07-25 12:38:54.000000 cwtune-0.1.8/cwtune.egg-info/top_level.txt
--rw-r--r--   0 arran      (501) staff       (20)       66 2023-07-25 12:31:11.000000 cwtune-0.1.8/requirements.txt
--rw-r--r--   0 arran      (501) staff       (20)      423 2023-07-25 12:38:55.153175 cwtune-0.1.8/setup.cfg
--rw-r--r--   0 arran      (501) staff       (20)     1337 2023-07-25 12:38:47.000000 cwtune-0.1.8/setup.py
-drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-07-25 12:38:55.142677 cwtune-0.1.8/tests/
--rw-r--r--   0 arran      (501) staff       (20)       36 2023-07-11 11:02:07.000000 cwtune-0.1.8/tests/__init__.py
-drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-07-25 12:38:55.145911 cwtune-0.1.8/tests/__pycache__/
--rw-r--r--   0 arran      (501) staff       (20)      208 2023-07-11 11:10:33.000000 cwtune-0.1.8/tests/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 arran      (501) staff       (20)     4029 2023-07-11 11:10:33.000000 cwtune-0.1.8/tests/__pycache__/test_cwtune.cpython-311-pytest-6.2.4.pyc
--rw-r--r--   0 arran      (501) staff       (20)     7071 2023-07-17 14:03:14.000000 cwtune-0.1.8/tests/__pycache__/test_cwtune.cpython-311.pyc
--rw-r--r--   0 arran      (501) staff       (20)     3754 2023-07-17 14:03:13.000000 cwtune-0.1.8/tests/test_cwtune.py
+drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-07-25 12:45:48.428566 cwtune-0.1.9/
+-rw-r--r--   0 arran      (501) staff       (20)     1204 2023-07-25 11:17:40.000000 cwtune-0.1.9/.gitignore
+-rw-r--r--   0 arran      (501) staff       (20)     1070 2023-07-25 11:24:31.000000 cwtune-0.1.9/LICENSE
+-rw-r--r--   0 arran      (501) staff       (20)     1531 2023-07-25 12:45:48.430439 cwtune-0.1.9/PKG-INFO
+-rw-r--r--   0 arran      (501) staff       (20)      860 2023-07-11 11:02:07.000000 cwtune-0.1.9/README.rst
+drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-07-25 12:45:48.327695 cwtune-0.1.9/cwtune/
+-rw-r--r--   0 arran      (501) staff       (20)      123 2023-07-11 11:02:07.000000 cwtune-0.1.9/cwtune/__init__.py
+-rw-r--r--   0 arran      (501) staff       (20)     5599 2023-07-25 10:25:39.000000 cwtune-0.1.9/cwtune/aws.py
+-rw-r--r--   0 arran      (501) staff       (20)     1247 2023-07-25 12:37:56.000000 cwtune-0.1.9/cwtune/cli.py
+-rw-r--r--   0 arran      (501) staff       (20)     9126 2023-07-25 10:19:06.000000 cwtune-0.1.9/cwtune/cwtune.py
+-rw-r--r--   0 arran      (501) staff       (20)     2400 2023-07-24 12:37:41.000000 cwtune-0.1.9/cwtune/timeseries.py
+-rw-r--r--   0 arran      (501) staff       (20)     2760 2023-07-25 12:45:29.000000 cwtune-0.1.9/cwtune/utils.py
+drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-07-25 12:45:48.367193 cwtune-0.1.9/cwtune.egg-info/
+-rw-r--r--   0 arran      (501) staff       (20)     1531 2023-07-25 12:45:47.000000 cwtune-0.1.9/cwtune.egg-info/PKG-INFO
+-rw-r--r--   0 arran      (501) staff       (20)      564 2023-07-25 12:45:48.000000 cwtune-0.1.9/cwtune.egg-info/SOURCES.txt
+-rw-r--r--   0 arran      (501) staff       (20)        1 2023-07-25 12:45:47.000000 cwtune-0.1.9/cwtune.egg-info/dependency_links.txt
+-rw-r--r--   0 arran      (501) staff       (20)       43 2023-07-25 12:45:47.000000 cwtune-0.1.9/cwtune.egg-info/entry_points.txt
+-rw-r--r--   0 arran      (501) staff       (20)        1 2023-07-25 11:33:06.000000 cwtune-0.1.9/cwtune.egg-info/not-zip-safe
+-rw-r--r--   0 arran      (501) staff       (20)       65 2023-07-25 12:45:47.000000 cwtune-0.1.9/cwtune.egg-info/requires.txt
+-rw-r--r--   0 arran      (501) staff       (20)        7 2023-07-25 12:45:47.000000 cwtune-0.1.9/cwtune.egg-info/top_level.txt
+-rw-r--r--   0 arran      (501) staff       (20)       66 2023-07-25 12:31:11.000000 cwtune-0.1.9/requirements.txt
+-rw-r--r--   0 arran      (501) staff       (20)      423 2023-07-25 12:45:48.444829 cwtune-0.1.9/setup.cfg
+-rw-r--r--   0 arran      (501) staff       (20)     1337 2023-07-25 12:45:37.000000 cwtune-0.1.9/setup.py
+drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-07-25 12:45:48.390258 cwtune-0.1.9/tests/
+-rw-r--r--   0 arran      (501) staff       (20)       36 2023-07-11 11:02:07.000000 cwtune-0.1.9/tests/__init__.py
+drwxr-xr-x   0 arran      (501) staff       (20)        0 2023-07-25 12:45:48.423237 cwtune-0.1.9/tests/__pycache__/
+-rw-r--r--   0 arran      (501) staff       (20)      208 2023-07-11 11:10:33.000000 cwtune-0.1.9/tests/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 arran      (501) staff       (20)     4029 2023-07-11 11:10:33.000000 cwtune-0.1.9/tests/__pycache__/test_cwtune.cpython-311-pytest-6.2.4.pyc
+-rw-r--r--   0 arran      (501) staff       (20)     7071 2023-07-17 14:03:14.000000 cwtune-0.1.9/tests/__pycache__/test_cwtune.cpython-311.pyc
+-rw-r--r--   0 arran      (501) staff       (20)     3754 2023-07-17 14:03:13.000000 cwtune-0.1.9/tests/test_cwtune.py
```

### Comparing `cwtune-0.1.8/.gitignore` & `cwtune-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.8/LICENSE` & `cwtune-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.8/PKG-INFO` & `cwtune-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwtune
-Version: 0.1.8
+Version: 0.1.9
 Summary: CLI for AWS CLoudWatch Alarm Tuning/Creation
 Home-page: https://github.com/availabl-co/cwtune
 Author: Arran McCabe
 Author-email: arran@availabl.ai
 License: MIT license
 Keywords: cwtune
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `cwtune-0.1.8/README.rst` & `cwtune-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.8/cwtune/aws.py` & `cwtune-0.1.9/cwtune/aws.py`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.8/cwtune/cli.py` & `cwtune-0.1.9/cwtune/cli.py`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.8/cwtune/cwtune.py` & `cwtune-0.1.9/cwtune/cwtune.py`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.8/cwtune/timeseries.py` & `cwtune-0.1.9/cwtune/timeseries.py`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.8/cwtune/utils.py` & `cwtune-0.1.9/cwtune/utils.py`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.8/cwtune.egg-info/PKG-INFO` & `cwtune-0.1.9/cwtune.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwtune
-Version: 0.1.8
+Version: 0.1.9
 Summary: CLI for AWS CLoudWatch Alarm Tuning/Creation
 Home-page: https://github.com/availabl-co/cwtune
 Author: Arran McCabe
 Author-email: arran@availabl.ai
 License: MIT license
 Keywords: cwtune
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `cwtune-0.1.8/cwtune.egg-info/SOURCES.txt` & `cwtune-0.1.9/cwtune.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.8/setup.py` & `cwtune-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords='cwtune',
     name='cwtune',
     packages=find_packages(include=['cwtune', 'cwtune.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/availabl-co/cwtune',
-    version='0.1.8',
+    version='0.1.9',
     zip_safe=False,
 )
```

### Comparing `cwtune-0.1.8/tests/__pycache__/test_cwtune.cpython-311-pytest-6.2.4.pyc` & `cwtune-0.1.9/tests/__pycache__/test_cwtune.cpython-311-pytest-6.2.4.pyc`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.8/tests/__pycache__/test_cwtune.cpython-311.pyc` & `cwtune-0.1.9/tests/__pycache__/test_cwtune.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cwtune-0.1.8/tests/test_cwtune.py` & `cwtune-0.1.9/tests/test_cwtune.py`

 * *Files identical despite different names*

