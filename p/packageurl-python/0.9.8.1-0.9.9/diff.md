# Comparing `tmp/packageurl-python-0.9.8.1.tar.gz` & `tmp/packageurl-python-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/packageurl-python-0.9.8.1.tar", last modified: Sat Feb 12 03:58:13 2022, max compression
+gzip compressed data, was "dist/packageurl-python-0.9.9.tar", last modified: Tue Feb 15 19:08:08 2022, max compression
```

## Comparing `packageurl-python-0.9.8.1.tar` & `packageurl-python-0.9.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2022-02-12 03:58:13.000000 packageurl-python-0.9.8.1/
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2022-02-12 03:58:13.000000 packageurl-python-0.9.8.1/tests/
--rw-rw-r--   0 jono      (1000) jono      (1000)    10874 2022-02-07 19:35:06.000000 packageurl-python-0.9.8.1/tests/test_packageurl.py
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2022-02-12 03:58:13.000000 packageurl-python-0.9.8.1/tests/contrib/
--rw-rw-r--   0 jono      (1000) jono      (1000)     3298 2022-02-07 19:35:06.000000 packageurl-python-0.9.8.1/tests/contrib/test_purl2url.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     1785 2022-02-07 19:35:06.000000 packageurl-python-0.9.8.1/tests/contrib/test_get_path_segments.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     3361 2022-02-12 03:38:43.000000 packageurl-python-0.9.8.1/tests/contrib/test_url2purl.py
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2022-02-12 03:58:13.000000 packageurl-python-0.9.8.1/tests/contrib/data/
--rw-rw-r--   0 jono      (1000) jono      (1000)    32348 2022-02-12 03:56:56.000000 packageurl-python-0.9.8.1/tests/contrib/data/url2purl.json
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2022-02-12 03:58:13.000000 packageurl-python-0.9.8.1/tests/data/
--rw-rw-r--   0 jono      (1000) jono      (1000)     9916 2022-02-07 19:35:06.000000 packageurl-python-0.9.8.1/tests/data/test-suite-data.json
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2022-02-12 03:58:13.000000 packageurl-python-0.9.8.1/src/
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2022-02-12 03:58:13.000000 packageurl-python-0.9.8.1/src/packageurl_python.egg-info/
--rw-rw-r--   0 jono      (1000) jono      (1000)      831 2022-02-12 03:58:13.000000 packageurl-python-0.9.8.1/src/packageurl_python.egg-info/SOURCES.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)       11 2022-02-12 03:58:13.000000 packageurl-python-0.9.8.1/src/packageurl_python.egg-info/top_level.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)       21 2022-02-12 03:58:13.000000 packageurl-python-0.9.8.1/src/packageurl_python.egg-info/requires.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)     4308 2022-02-12 03:58:13.000000 packageurl-python-0.9.8.1/src/packageurl_python.egg-info/PKG-INFO
--rw-rw-r--   0 jono      (1000) jono      (1000)        1 2022-02-12 03:58:13.000000 packageurl-python-0.9.8.1/src/packageurl_python.egg-info/dependency_links.txt
--rw-rw-r--   0 jono      (1000) jono      (1000)        1 2022-02-07 19:50:13.000000 packageurl-python-0.9.8.1/src/packageurl_python.egg-info/not-zip-safe
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2022-02-12 03:58:13.000000 packageurl-python-0.9.8.1/src/packageurl/
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2022-02-12 03:58:13.000000 packageurl-python-0.9.8.1/src/packageurl/contrib/
-drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2022-02-12 03:58:13.000000 packageurl-python-0.9.8.1/src/packageurl/contrib/django/
--rw-rw-r--   0 jono      (1000) jono      (1000)     5564 2022-02-11 23:04:16.000000 packageurl-python-0.9.8.1/src/packageurl/contrib/django/models.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     1779 2022-02-07 19:35:06.000000 packageurl-python-0.9.8.1/src/packageurl/contrib/django/filters.py
--rw-rw-r--   0 jono      (1000) jono      (1000)        0 2022-02-07 19:35:06.000000 packageurl-python-0.9.8.1/src/packageurl/contrib/django/__init__.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     8012 2022-02-07 19:35:06.000000 packageurl-python-0.9.8.1/src/packageurl/contrib/route.py
--rw-rw-r--   0 jono      (1000) jono      (1000)     4411 2022-02-07 19:35:06.000000 packageurl-python-0.9.8.1/src/packageurl/contrib/purl2url.py
--rw-rw-r--   0 jono      (1000) jono      (1000)    20414 2022-02-12 03:56:56.000000 packageurl-python-0.9.8.1/src/packageurl/contrib/url2purl.py
--rw-rw-r--   0 jono      (1000) jono      (1000)        0 2022-02-07 19:35:06.000000 packageurl-python-0.9.8.1/src/packageurl/contrib/__init__.py
--rw-rw-r--   0 jono      (1000) jono      (1000)    12843 2022-02-07 19:35:06.000000 packageurl-python-0.9.8.1/src/packageurl/__init__.py
--rw-rw-r--   0 jono      (1000) jono      (1000)      232 2022-02-07 19:35:06.000000 packageurl-python-0.9.8.1/MANIFEST.in
--rw-rw-r--   0 jono      (1000) jono      (1000)     2671 2022-02-07 19:35:06.000000 packageurl-python-0.9.8.1/README.rst
--rw-rw-r--   0 jono      (1000) jono      (1000)      150 2022-02-07 19:35:06.000000 packageurl-python-0.9.8.1/setup.py
--rw-rw-r--   0 jono      (1000) jono      (1000)      670 2022-02-07 19:35:06.000000 packageurl-python-0.9.8.1/CONTRIBUTING.rst
--rw-rw-r--   0 jono      (1000) jono      (1000)     1054 2022-02-07 19:35:06.000000 packageurl-python-0.9.8.1/mit.LICENSE
--rw-rw-r--   0 jono      (1000) jono      (1000)     2334 2022-02-12 03:56:56.000000 packageurl-python-0.9.8.1/CHANGELOG.rst
--rw-rw-r--   0 jono      (1000) jono      (1000)     1589 2022-02-12 03:58:13.000000 packageurl-python-0.9.8.1/setup.cfg
--rw-rw-r--   0 jono      (1000) jono      (1000)     4308 2022-02-12 03:58:13.000000 packageurl-python-0.9.8.1/PKG-INFO
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2022-02-15 19:08:08.000000 packageurl-python-0.9.9/
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2022-02-15 19:08:08.000000 packageurl-python-0.9.9/tests/
+-rw-rw-r--   0 jono      (1000) jono      (1000)    10874 2022-02-07 19:35:06.000000 packageurl-python-0.9.9/tests/test_packageurl.py
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2022-02-15 19:08:08.000000 packageurl-python-0.9.9/tests/contrib/
+-rw-rw-r--   0 jono      (1000) jono      (1000)     3298 2022-02-07 19:35:06.000000 packageurl-python-0.9.9/tests/contrib/test_purl2url.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1785 2022-02-07 19:35:06.000000 packageurl-python-0.9.9/tests/contrib/test_get_path_segments.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     3361 2022-02-12 03:38:43.000000 packageurl-python-0.9.9/tests/contrib/test_url2purl.py
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2022-02-15 19:08:08.000000 packageurl-python-0.9.9/tests/contrib/data/
+-rw-rw-r--   0 jono      (1000) jono      (1000)    32348 2022-02-12 03:56:56.000000 packageurl-python-0.9.9/tests/contrib/data/url2purl.json
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2022-02-15 19:08:08.000000 packageurl-python-0.9.9/tests/data/
+-rw-rw-r--   0 jono      (1000) jono      (1000)     9916 2022-02-07 19:35:06.000000 packageurl-python-0.9.9/tests/data/test-suite-data.json
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2022-02-15 19:08:08.000000 packageurl-python-0.9.9/src/
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2022-02-15 19:08:08.000000 packageurl-python-0.9.9/src/packageurl_python.egg-info/
+-rw-rw-r--   0 jono      (1000) jono      (1000)      831 2022-02-15 19:08:07.000000 packageurl-python-0.9.9/src/packageurl_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)       11 2022-02-15 19:08:07.000000 packageurl-python-0.9.9/src/packageurl_python.egg-info/top_level.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)       21 2022-02-15 19:08:07.000000 packageurl-python-0.9.9/src/packageurl_python.egg-info/requires.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)     4306 2022-02-15 19:08:07.000000 packageurl-python-0.9.9/src/packageurl_python.egg-info/PKG-INFO
+-rw-rw-r--   0 jono      (1000) jono      (1000)        1 2022-02-15 19:08:07.000000 packageurl-python-0.9.9/src/packageurl_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 jono      (1000) jono      (1000)        1 2022-02-07 19:50:13.000000 packageurl-python-0.9.9/src/packageurl_python.egg-info/not-zip-safe
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2022-02-15 19:08:08.000000 packageurl-python-0.9.9/src/packageurl/
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2022-02-15 19:08:08.000000 packageurl-python-0.9.9/src/packageurl/contrib/
+drwxrwxr-x   0 jono      (1000) jono      (1000)        0 2022-02-15 19:08:08.000000 packageurl-python-0.9.9/src/packageurl/contrib/django/
+-rw-rw-r--   0 jono      (1000) jono      (1000)     5564 2022-02-11 23:04:16.000000 packageurl-python-0.9.9/src/packageurl/contrib/django/models.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1779 2022-02-07 19:35:06.000000 packageurl-python-0.9.9/src/packageurl/contrib/django/filters.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)        0 2022-02-07 19:35:06.000000 packageurl-python-0.9.9/src/packageurl/contrib/django/__init__.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     8012 2022-02-07 19:35:06.000000 packageurl-python-0.9.9/src/packageurl/contrib/route.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)     4411 2022-02-07 19:35:06.000000 packageurl-python-0.9.9/src/packageurl/contrib/purl2url.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)    20414 2022-02-12 03:56:56.000000 packageurl-python-0.9.9/src/packageurl/contrib/url2purl.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)        0 2022-02-07 19:35:06.000000 packageurl-python-0.9.9/src/packageurl/contrib/__init__.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)    12843 2022-02-07 19:35:06.000000 packageurl-python-0.9.9/src/packageurl/__init__.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)      232 2022-02-07 19:35:06.000000 packageurl-python-0.9.9/MANIFEST.in
+-rw-rw-r--   0 jono      (1000) jono      (1000)     2671 2022-02-07 19:35:06.000000 packageurl-python-0.9.9/README.rst
+-rw-rw-r--   0 jono      (1000) jono      (1000)      150 2022-02-07 19:35:06.000000 packageurl-python-0.9.9/setup.py
+-rw-rw-r--   0 jono      (1000) jono      (1000)      670 2022-02-07 19:35:06.000000 packageurl-python-0.9.9/CONTRIBUTING.rst
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1054 2022-02-07 19:35:06.000000 packageurl-python-0.9.9/mit.LICENSE
+-rw-rw-r--   0 jono      (1000) jono      (1000)     2456 2022-02-15 18:23:30.000000 packageurl-python-0.9.9/CHANGELOG.rst
+-rw-rw-r--   0 jono      (1000) jono      (1000)     1587 2022-02-15 19:08:08.000000 packageurl-python-0.9.9/setup.cfg
+-rw-rw-r--   0 jono      (1000) jono      (1000)     4306 2022-02-15 19:08:08.000000 packageurl-python-0.9.9/PKG-INFO
```

### Comparing `packageurl-python-0.9.8.1/tests/test_packageurl.py` & `packageurl-python-0.9.9/tests/test_packageurl.py`

 * *Files identical despite different names*

### Comparing `packageurl-python-0.9.8.1/tests/contrib/test_purl2url.py` & `packageurl-python-0.9.9/tests/contrib/test_purl2url.py`

 * *Files identical despite different names*

### Comparing `packageurl-python-0.9.8.1/tests/contrib/test_get_path_segments.py` & `packageurl-python-0.9.9/tests/contrib/test_get_path_segments.py`

 * *Files identical despite different names*

### Comparing `packageurl-python-0.9.8.1/tests/contrib/test_url2purl.py` & `packageurl-python-0.9.9/tests/contrib/test_url2purl.py`

 * *Files identical despite different names*

### Comparing `packageurl-python-0.9.8.1/tests/contrib/data/url2purl.json` & `packageurl-python-0.9.9/tests/contrib/data/url2purl.json`

 * *Files identical despite different names*

### Comparing `packageurl-python-0.9.8.1/tests/data/test-suite-data.json` & `packageurl-python-0.9.9/tests/data/test-suite-data.json`

 * *Files identical despite different names*

### Comparing `packageurl-python-0.9.8.1/src/packageurl_python.egg-info/SOURCES.txt` & `packageurl-python-0.9.9/src/packageurl_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `packageurl-python-0.9.8.1/src/packageurl_python.egg-info/PKG-INFO` & `packageurl-python-0.9.9/src/packageurl_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packageurl-python
-Version: 0.9.8.1
+Version: 0.9.9
 Summary: A purl aka. Package URL parser and builder
 Home-page: https://github.com/package-url/packageurl-python
 Author: the purl authors
 License: MIT
 Description: # packageurl-python
         
         Python library to parse and build "purl" aka. Package URLs.
```

### Comparing `packageurl-python-0.9.8.1/src/packageurl/contrib/django/models.py` & `packageurl-python-0.9.9/src/packageurl/contrib/django/models.py`

 * *Files identical despite different names*

### Comparing `packageurl-python-0.9.8.1/src/packageurl/contrib/django/filters.py` & `packageurl-python-0.9.9/src/packageurl/contrib/django/filters.py`

 * *Files identical despite different names*

### Comparing `packageurl-python-0.9.8.1/src/packageurl/contrib/route.py` & `packageurl-python-0.9.9/src/packageurl/contrib/route.py`

 * *Files identical despite different names*

### Comparing `packageurl-python-0.9.8.1/src/packageurl/contrib/purl2url.py` & `packageurl-python-0.9.9/src/packageurl/contrib/purl2url.py`

 * *Files identical despite different names*

### Comparing `packageurl-python-0.9.8.1/src/packageurl/contrib/url2purl.py` & `packageurl-python-0.9.9/src/packageurl/contrib/url2purl.py`

 * *Files identical despite different names*

### Comparing `packageurl-python-0.9.8.1/src/packageurl/__init__.py` & `packageurl-python-0.9.9/src/packageurl/__init__.py`

 * *Files identical despite different names*

### Comparing `packageurl-python-0.9.8.1/README.rst` & `packageurl-python-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `packageurl-python-0.9.8.1/CONTRIBUTING.rst` & `packageurl-python-0.9.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `packageurl-python-0.9.8.1/mit.LICENSE` & `packageurl-python-0.9.9/mit.LICENSE`

 * *Files identical despite different names*

### Comparing `packageurl-python-0.9.8.1/CHANGELOG.rst` & `packageurl-python-0.9.9/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 Changelog
 =========
 
-0.9.8.1 (2022-02-11)
+0.9.9 (2022-02-15)
 ------------------
 
+- Update version to be semver compliant. No changes to the code have been made.
+
+0.9.8.1 (2022-02-11)
+--------------------
+
 - Fix generic sourceforge PackageURL generation #79
 
 0.9.8 (2022-02-11)
 ------------------
 
 - Do not create a generic PackageURL for URLs without a path in url2purl #72
 - Use project name as the Package name when creating generic sourceforge PackageURLs #74
```

### Comparing `packageurl-python-0.9.8.1/setup.cfg` & `packageurl-python-0.9.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = packageurl-python
-version = 0.9.8.1
+version = 0.9.9
 license = MIT
 description = A purl aka. Package URL parser and builder
 long_description = file:README.rst
 author = the purl authors
 url = https://github.com/package-url/packageurl-python
 classifiers = 
 	Development Status :: 4 - Beta
```

### Comparing `packageurl-python-0.9.8.1/PKG-INFO` & `packageurl-python-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packageurl-python
-Version: 0.9.8.1
+Version: 0.9.9
 Summary: A purl aka. Package URL parser and builder
 Home-page: https://github.com/package-url/packageurl-python
 Author: the purl authors
 License: MIT
 Description: # packageurl-python
         
         Python library to parse and build "purl" aka. Package URLs.
```

