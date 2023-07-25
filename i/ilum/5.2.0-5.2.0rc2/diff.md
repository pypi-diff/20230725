# Comparing `tmp/ilum-5.2.0.tar.gz` & `tmp/ilum-5.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilum-5.2.0.tar", last modified: Tue Jul 25 07:11:03 2023, max compression
+gzip compressed data, was "ilum-5.2.0rc2.tar", last modified: Tue Jul 25 07:16:27 2023, max compression
```

## Comparing `ilum-5.2.0.tar` & `ilum-5.2.0rc2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-07-25 07:11:03.982032 ilum-5.2.0/
--rw-r--r--   0 runner    (1001) runner    (1001)     2237 2023-07-25 07:11:03.981032 ilum-5.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)     1512 2023-07-25 07:08:41.000000 ilum-5.2.0/README.md
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-07-25 07:11:03.980032 ilum-5.2.0/ilum/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-07-25 07:08:41.000000 ilum-5.2.0/ilum/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      642 2023-07-25 07:08:41.000000 ilum-5.2.0/ilum/api.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-07-25 07:11:03.981032 ilum-5.2.0/ilum.egg-info/
--rw-r--r--   0 runner    (1001) runner    (1001)     2237 2023-07-25 07:11:03.000000 ilum-5.2.0/ilum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)      159 2023-07-25 07:11:03.000000 ilum-5.2.0/ilum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        1 2023-07-25 07:11:03.000000 ilum-5.2.0/ilum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        5 2023-07-25 07:11:03.000000 ilum-5.2.0/ilum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       38 2023-07-25 07:11:03.982032 ilum-5.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) runner    (1001)     1072 2023-07-25 07:08:41.000000 ilum-5.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-07-25 07:16:27.980725 ilum-5.2.0rc2/
+-rw-r--r--   0 runner    (1001) runner    (1001)     2240 2023-07-25 07:16:27.979725 ilum-5.2.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)     1512 2023-07-25 07:08:41.000000 ilum-5.2.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-07-25 07:16:27.978726 ilum-5.2.0rc2/ilum/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-07-25 07:08:41.000000 ilum-5.2.0rc2/ilum/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      642 2023-07-25 07:08:41.000000 ilum-5.2.0rc2/ilum/api.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-07-25 07:16:27.979725 ilum-5.2.0rc2/ilum.egg-info/
+-rw-r--r--   0 runner    (1001) runner    (1001)     2240 2023-07-25 07:16:27.000000 ilum-5.2.0rc2/ilum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)      159 2023-07-25 07:16:27.000000 ilum-5.2.0rc2/ilum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        1 2023-07-25 07:16:27.000000 ilum-5.2.0rc2/ilum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        5 2023-07-25 07:16:27.000000 ilum-5.2.0rc2/ilum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       38 2023-07-25 07:16:27.980725 ilum-5.2.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) runner    (1001)     1076 2023-07-25 07:15:36.000000 ilum-5.2.0rc2/setup.py
```

### Comparing `ilum-5.2.0/PKG-INFO` & `ilum-5.2.0rc2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilum
-Version: 5.2.0
+Version: 5.2.0rc2
 Summary: Ilum job python api
 Home-page: https://ilum.cloud
 Author: Ilum Labs LLC
 Author-email: info@ilum.cloud
 License: apache-2.0
 Project-URL: Documentation, https://ilum.cloud/docs/
 Project-URL: API Ref, https://ilum.cloud/docs/api/
```

### Comparing `ilum-5.2.0/README.md` & `ilum-5.2.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `ilum-5.2.0/ilum/api.py` & `ilum-5.2.0rc2/ilum/api.py`

 * *Files identical despite different names*

### Comparing `ilum-5.2.0/ilum.egg-info/PKG-INFO` & `ilum-5.2.0rc2/ilum.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilum
-Version: 5.2.0
+Version: 5.2.0rc2
 Summary: Ilum job python api
 Home-page: https://ilum.cloud
 Author: Ilum Labs LLC
 Author-email: info@ilum.cloud
 License: apache-2.0
 Project-URL: Documentation, https://ilum.cloud/docs/
 Project-URL: API Ref, https://ilum.cloud/docs/api/
```

### Comparing `ilum-5.2.0/setup.py` & `ilum-5.2.0rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="ilum",
-    version="5.2.0",
+    version="5.2.0-RC2",
     packages=find_packages(),
     package_data={"": ["ilum/*"]},
     url="https://ilum.cloud",
     author="Ilum Labs LLC",
     author_email="info@ilum.cloud",
     description="Ilum job python api",
     long_description=long_description,
```

