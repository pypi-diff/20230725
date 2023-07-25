# Comparing `tmp/arthub_api-1.8.0.tar.gz` & `tmp/arthub_api-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arthub_api-1.8.0.tar", last modified: Tue Jul 25 13:49:18 2023, max compression
+gzip compressed data, was "arthub_api-1.8.1.tar", last modified: Tue Jul 25 14:03:06 2023, max compression
```

## Comparing `arthub_api-1.8.0.tar` & `arthub_api-1.8.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 13:49:18.336596 arthub_api-1.8.0/
--rw-rw-rw-   0        0        0     1077 2022-09-05 10:15:53.000000 arthub_api-1.8.0/LICENSE
--rw-rw-rw-   0        0        0      107 2022-09-05 10:15:53.000000 arthub_api-1.8.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1412 2023-07-25 13:49:18.335605 arthub_api-1.8.0/PKG-INFO
--rw-rw-rw-   0        0        0      864 2023-05-19 06:20:15.000000 arthub_api-1.8.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 13:49:18.313408 arthub_api-1.8.0/arthub_api/
--rw-rw-rw-   0        0        0      675 2023-07-25 13:45:45.000000 arthub_api-1.8.0/arthub_api/__init__.py
--rw-rw-rw-   0        0        0     3730 2023-07-25 13:45:45.000000 arthub_api-1.8.0/arthub_api/__main__.py
--rw-rw-rw-   0        0        0      241 2023-07-25 13:47:27.000000 arthub_api-1.8.0/arthub_api/__version__.py
--rw-rw-rw-   0        0        0    13661 2023-05-11 11:13:51.000000 arthub_api-1.8.0/arthub_api/_internal_utils.py
--rw-rw-rw-   0        0        0      104 2023-07-25 13:45:45.000000 arthub_api-1.8.0/arthub_api/arthub_api_config.py
--rw-rw-rw-   0        0        0      501 2023-07-25 13:45:45.000000 arthub_api-1.8.0/arthub_api/asset_matrix.py
--rw-rw-rw-   0        0        0    43536 2023-07-25 13:45:45.000000 arthub_api-1.8.0/arthub_api/blade_api.py
--rw-rw-rw-   0        0        0     2072 2023-07-25 13:45:45.000000 arthub_api-1.8.0/arthub_api/blade_api_instance.py
--rw-rw-rw-   0        0        0    28990 2023-07-25 13:45:45.000000 arthub_api-1.8.0/arthub_api/blade_storage.py
--rw-rw-rw-   0        0        0       22 2023-02-08 16:32:42.000000 arthub_api-1.8.0/arthub_api/cli.py
--rw-rw-rw-   0        0        0     1443 2023-07-25 13:45:45.000000 arthub_api-1.8.0/arthub_api/config.py
--rw-rw-rw-   0        0        0      523 2023-02-08 16:32:42.000000 arthub_api-1.8.0/arthub_api/exception.py
--rw-rw-rw-   0        0        0     1258 2023-03-14 10:50:34.000000 arthub_api-1.8.0/arthub_api/models.py
--rw-rw-rw-   0        0        0    44124 2023-07-25 13:45:45.000000 arthub_api-1.8.0/arthub_api/open_api.py
--rw-rw-rw-   0        0        0    41836 2023-07-25 13:45:45.000000 arthub_api-1.8.0/arthub_api/storage.py
--rw-rw-rw-   0        0        0     9102 2023-07-25 13:45:45.000000 arthub_api-1.8.0/arthub_api/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-25 13:49:18.324935 arthub_api-1.8.0/arthub_api.egg-info/
--rw-rw-rw-   0        0        0     1412 2023-07-25 13:49:17.000000 arthub_api-1.8.0/arthub_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      790 2023-07-25 13:49:17.000000 arthub_api-1.8.0/arthub_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 13:49:17.000000 arthub_api-1.8.0/arthub_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-07-25 13:49:17.000000 arthub_api-1.8.0/arthub_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-02-09 14:04:12.000000 arthub_api-1.8.0/arthub_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      116 2023-07-25 13:49:17.000000 arthub_api-1.8.0/arthub_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-25 13:49:17.000000 arthub_api-1.8.0/arthub_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       63 2022-09-26 03:28:18.000000 arthub_api-1.8.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 13:49:18.336596 arthub_api-1.8.0/setup.cfg
--rw-rw-rw-   0        0        0     3087 2023-07-25 13:45:45.000000 arthub_api-1.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 13:49:18.332912 arthub_api-1.8.0/tests/
--rw-rw-rw-   0        0        0      176 2023-07-25 13:45:45.000000 arthub_api-1.8.0/tests/__init__.py
--rw-rw-rw-   0        0        0      108 2023-05-19 06:20:15.000000 arthub_api-1.8.0/tests/_utils.py
--rw-rw-rw-   0        0        0      735 2023-07-25 13:45:45.000000 arthub_api-1.8.0/tests/conftest.py
--rw-rw-rw-   0        0        0     6646 2023-07-25 13:45:45.000000 arthub_api-1.8.0/tests/test_open_api.py
--rw-rw-rw-   0        0        0     2979 2023-07-25 13:45:45.000000 arthub_api-1.8.0/tests/test_storage.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:03:06.274170 arthub_api-1.8.1/
+-rw-rw-rw-   0        0        0     1077 2022-09-05 10:15:53.000000 arthub_api-1.8.1/LICENSE
+-rw-rw-rw-   0        0        0      107 2022-09-05 10:15:53.000000 arthub_api-1.8.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1412 2023-07-25 14:03:06.273209 arthub_api-1.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0      864 2023-05-19 06:20:15.000000 arthub_api-1.8.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 14:03:06.189377 arthub_api-1.8.1/arthub_api/
+-rw-rw-rw-   0        0        0      675 2023-07-25 13:45:45.000000 arthub_api-1.8.1/arthub_api/__init__.py
+-rw-rw-rw-   0        0        0     3730 2023-07-25 13:45:45.000000 arthub_api-1.8.1/arthub_api/__main__.py
+-rw-rw-rw-   0        0        0      241 2023-07-25 14:01:13.000000 arthub_api-1.8.1/arthub_api/__version__.py
+-rw-rw-rw-   0        0        0    13661 2023-05-11 11:13:51.000000 arthub_api-1.8.1/arthub_api/_internal_utils.py
+-rw-rw-rw-   0        0        0      104 2023-07-25 13:45:45.000000 arthub_api-1.8.1/arthub_api/arthub_api_config.py
+-rw-rw-rw-   0        0        0      501 2023-07-25 13:45:45.000000 arthub_api-1.8.1/arthub_api/asset_matrix.py
+-rw-rw-rw-   0        0        0    43536 2023-07-25 13:45:45.000000 arthub_api-1.8.1/arthub_api/blade_api.py
+-rw-rw-rw-   0        0        0     2072 2023-07-25 13:45:45.000000 arthub_api-1.8.1/arthub_api/blade_api_instance.py
+-rw-rw-rw-   0        0        0    28990 2023-07-25 13:45:45.000000 arthub_api-1.8.1/arthub_api/blade_storage.py
+-rw-rw-rw-   0        0        0       22 2023-02-08 16:32:42.000000 arthub_api-1.8.1/arthub_api/cli.py
+-rw-rw-rw-   0        0        0     1443 2023-07-25 13:45:45.000000 arthub_api-1.8.1/arthub_api/config.py
+-rw-rw-rw-   0        0        0      523 2023-02-08 16:32:42.000000 arthub_api-1.8.1/arthub_api/exception.py
+-rw-rw-rw-   0        0        0     1258 2023-03-14 10:50:34.000000 arthub_api-1.8.1/arthub_api/models.py
+-rw-rw-rw-   0        0        0    44124 2023-07-25 13:45:45.000000 arthub_api-1.8.1/arthub_api/open_api.py
+-rw-rw-rw-   0        0        0    41836 2023-07-25 13:45:45.000000 arthub_api-1.8.1/arthub_api/storage.py
+-rw-rw-rw-   0        0        0     9102 2023-07-25 13:45:45.000000 arthub_api-1.8.1/arthub_api/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:03:06.199350 arthub_api-1.8.1/arthub_api.egg-info/
+-rw-rw-rw-   0        0        0     1412 2023-07-25 14:03:06.000000 arthub_api-1.8.1/arthub_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      790 2023-07-25 14:03:06.000000 arthub_api-1.8.1/arthub_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 14:03:06.000000 arthub_api-1.8.1/arthub_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-07-25 14:03:06.000000 arthub_api-1.8.1/arthub_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-02-09 14:04:12.000000 arthub_api-1.8.1/arthub_api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      181 2023-07-25 14:03:06.000000 arthub_api-1.8.1/arthub_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-25 14:03:06.000000 arthub_api-1.8.1/arthub_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       63 2022-09-26 03:28:18.000000 arthub_api-1.8.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 14:03:06.274170 arthub_api-1.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     3154 2023-07-25 14:01:13.000000 arthub_api-1.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:03:06.271177 arthub_api-1.8.1/tests/
+-rw-rw-rw-   0        0        0      176 2023-07-25 13:45:45.000000 arthub_api-1.8.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      108 2023-05-19 06:20:15.000000 arthub_api-1.8.1/tests/_utils.py
+-rw-rw-rw-   0        0        0      735 2023-07-25 13:45:45.000000 arthub_api-1.8.1/tests/conftest.py
+-rw-rw-rw-   0        0        0     6646 2023-07-25 13:45:45.000000 arthub_api-1.8.1/tests/test_open_api.py
+-rw-rw-rw-   0        0        0     2979 2023-07-25 13:45:45.000000 arthub_api-1.8.1/tests/test_storage.py
```

### Comparing `arthub_api-1.8.0/LICENSE` & `arthub_api-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.0/PKG-INFO` & `arthub_api-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arthub_api
-Version: 1.8.0
+Version: 1.8.1
 Summary: ArHhub Python SDK
 Home-page: UNKNOWN
 Author: Joey Ding
 Author-email: joeyding@tencent.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arthub_api-1.8.0/README.md` & `arthub_api-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.0/arthub_api/__init__.py` & `arthub_api-1.8.1/arthub_api/__init__.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.0/arthub_api/__main__.py` & `arthub_api-1.8.1/arthub_api/__main__.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.0/arthub_api/_internal_utils.py` & `arthub_api-1.8.1/arthub_api/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.0/arthub_api/blade_api.py` & `arthub_api-1.8.1/arthub_api/blade_api.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.0/arthub_api/blade_api_instance.py` & `arthub_api-1.8.1/arthub_api/blade_api_instance.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.0/arthub_api/blade_storage.py` & `arthub_api-1.8.1/arthub_api/blade_storage.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.0/arthub_api/config.py` & `arthub_api-1.8.1/arthub_api/config.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.0/arthub_api/exception.py` & `arthub_api-1.8.1/arthub_api/exception.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.0/arthub_api/models.py` & `arthub_api-1.8.1/arthub_api/models.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.0/arthub_api/open_api.py` & `arthub_api-1.8.1/arthub_api/open_api.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.0/arthub_api/storage.py` & `arthub_api-1.8.1/arthub_api/storage.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.0/arthub_api/utils.py` & `arthub_api-1.8.1/arthub_api/utils.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.0/arthub_api.egg-info/PKG-INFO` & `arthub_api-1.8.1/arthub_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arthub-api
-Version: 1.8.0
+Version: 1.8.1
 Summary: ArHhub Python SDK
 Home-page: UNKNOWN
 Author: Joey Ding
 Author-email: joeyding@tencent.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arthub_api-1.8.0/arthub_api.egg-info/SOURCES.txt` & `arthub_api-1.8.1/arthub_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.0/setup.py` & `arthub_api-1.8.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,19 +49,20 @@
 # 'setup.py publish' shortcut.
 if sys.argv[-1] == "publish":
     os.system("python setup.py sdist bdist_wheel")
     os.system("twine upload dist/*")
     sys.exit()
 
 requires = [
-    "requests==2.25.1",
-    "platformdirs==2.0.2",
-    "tenacity>=5.0",
-    "six==1.16",
-    "environ_config>=21",
+    'requests==2.25.1',
+    'platformdirs==2.0.2',
+    'tenacity==5.0; python_version < "3"',
+    'tenacity==8; python_version >= "3"',
+    'six==1.16',
+    'environ_config==21.1',
 ]
 
 test_requirements = [
     "pytest",
 ]
 
 about = {}
```

### Comparing `arthub_api-1.8.0/tests/conftest.py` & `arthub_api-1.8.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.0/tests/test_open_api.py` & `arthub_api-1.8.1/tests/test_open_api.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.8.0/tests/test_storage.py` & `arthub_api-1.8.1/tests/test_storage.py`

 * *Files identical despite different names*

