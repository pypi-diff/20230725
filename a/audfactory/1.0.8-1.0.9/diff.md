# Comparing `tmp/audfactory-1.0.8.tar.gz` & `tmp/audfactory-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audfactory-1.0.8.tar", last modified: Mon Jan  3 14:53:42 2022, max compression
+gzip compressed data, was "audfactory-1.0.9.tar", last modified: Fri Dec 23 11:30:11 2022, max compression
```

## Comparing `audfactory-1.0.8.tar` & `audfactory-1.0.9.tar`

### file list

```diff
@@ -1,41 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 14:53:42.490729 audfactory-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 14:53:42.486729 audfactory-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 14:53:42.486729 audfactory-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2035 2022-01-03 14:53:32.000000 audfactory-1.0.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1455 2022-01-03 14:53:32.000000 audfactory-1.0.8/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-01-03 14:53:32.000000 audfactory-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     7498 2022-01-03 14:53:32.000000 audfactory-1.0.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2367 2022-01-03 14:53:32.000000 audfactory-1.0.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1143 2022-01-03 14:53:32.000000 audfactory-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    12745 2022-01-03 14:53:42.490729 audfactory-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1559 2022-01-03 14:53:32.000000 audfactory-1.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 14:53:42.486729 audfactory-1.0.8/audfactory/
--rw-r--r--   0 runner    (1001) docker     (121)      557 2022-01-03 14:53:32.000000 audfactory-1.0.8/audfactory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 14:53:42.490729 audfactory-1.0.8/audfactory/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-03 14:53:32.000000 audfactory-1.0.8/audfactory/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12055 2022-01-03 14:53:32.000000 audfactory-1.0.8/audfactory/core/api.py
--rw-r--r--   0 runner    (1001) docker     (121)    21968 2022-01-03 14:53:32.000000 audfactory-1.0.8/audfactory/core/lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 14:53:42.486729 audfactory-1.0.8/audfactory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12745 2022-01-03 14:53:42.000000 audfactory-1.0.8/audfactory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      672 2022-01-03 14:53:42.000000 audfactory-1.0.8/audfactory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-03 14:53:42.000000 audfactory-1.0.8/audfactory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-01-03 14:53:42.000000 audfactory-1.0.8/audfactory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-01-03 14:53:42.000000 audfactory-1.0.8/audfactory.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 14:53:42.490729 audfactory-1.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-01-03 14:53:32.000000 audfactory-1.0.8/docs/api-audfactory.rst
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-01-03 14:53:32.000000 audfactory-1.0.8/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1607 2022-01-03 14:53:32.000000 audfactory-1.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-01-03 14:53:32.000000 audfactory-1.0.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-01-03 14:53:32.000000 audfactory-1.0.8/docs/genindex.rst
--rw-r--r--   0 runner    (1001) docker     (121)      577 2022-01-03 14:53:32.000000 audfactory-1.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-01-03 14:53:32.000000 audfactory-1.0.8/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-01-03 14:53:32.000000 audfactory-1.0.8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3069 2022-01-03 14:53:32.000000 audfactory-1.0.8/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-01-03 14:53:32.000000 audfactory-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1298 2022-01-03 14:53:42.490729 audfactory-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-01-03 14:53:32.000000 audfactory-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 14:53:42.490729 audfactory-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-01-03 14:53:32.000000 audfactory-1.0.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-01-03 14:53:32.000000 audfactory-1.0.8/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     9441 2022-01-03 14:53:32.000000 audfactory-1.0.8/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    11447 2022-01-03 14:53:32.000000 audfactory-1.0.8/tests/test_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 11:30:11.820442 audfactory-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 11:30:11.812442 audfactory-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 11:30:11.816442 audfactory-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2022-12-23 11:29:57.000000 audfactory-1.0.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2022-12-23 11:29:57.000000 audfactory-1.0.9/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2022-12-23 11:29:57.000000 audfactory-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     7658 2022-12-23 11:29:57.000000 audfactory-1.0.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2022-12-23 11:29:57.000000 audfactory-1.0.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2022-12-23 11:29:57.000000 audfactory-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13020 2022-12-23 11:30:11.820442 audfactory-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2022-12-23 11:29:57.000000 audfactory-1.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 11:30:11.816442 audfactory-1.0.9/audfactory/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2022-12-23 11:29:57.000000 audfactory-1.0.9/audfactory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 11:30:11.816442 audfactory-1.0.9/audfactory/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 11:29:57.000000 audfactory-1.0.9/audfactory/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12062 2022-12-23 11:29:57.000000 audfactory-1.0.9/audfactory/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21973 2022-12-23 11:29:57.000000 audfactory-1.0.9/audfactory/core/lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 11:30:11.816442 audfactory-1.0.9/audfactory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13020 2022-12-23 11:30:11.000000 audfactory-1.0.9/audfactory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2022-12-23 11:30:11.000000 audfactory-1.0.9/audfactory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-23 11:30:11.000000 audfactory-1.0.9/audfactory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-23 11:30:11.000000 audfactory-1.0.9/audfactory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-23 11:30:11.000000 audfactory-1.0.9/audfactory.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 11:30:11.816442 audfactory-1.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 11:30:11.812442 audfactory-1.0.9/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 11:30:11.816442 audfactory-1.0.9/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-23 11:29:57.000000 audfactory-1.0.9/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2022-12-23 11:29:57.000000 audfactory-1.0.9/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2022-12-23 11:29:57.000000 audfactory-1.0.9/docs/_templates/autosummary/function.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 11:30:11.816442 audfactory-1.0.9/docs/api-src/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2022-12-23 11:29:57.000000 audfactory-1.0.9/docs/api-src/audfactory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-23 11:29:57.000000 audfactory-1.0.9/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2022-12-23 11:29:57.000000 audfactory-1.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-23 11:29:57.000000 audfactory-1.0.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2022-12-23 11:29:57.000000 audfactory-1.0.9/docs/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2022-12-23 11:29:57.000000 audfactory-1.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2022-12-23 11:29:57.000000 audfactory-1.0.9/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2022-12-23 11:29:57.000000 audfactory-1.0.9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2022-12-23 11:29:57.000000 audfactory-1.0.9/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2022-12-23 11:29:57.000000 audfactory-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2022-12-23 11:30:11.820442 audfactory-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2022-12-23 11:29:57.000000 audfactory-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 11:30:11.820442 audfactory-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2022-12-23 11:29:57.000000 audfactory-1.0.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2022-12-23 11:29:57.000000 audfactory-1.0.9/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9441 2022-12-23 11:29:57.000000 audfactory-1.0.9/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2022-12-23 11:29:57.000000 audfactory-1.0.9/tests/test_lookup.py
```

### Comparing `audfactory-1.0.8/.github/workflows/publish.yml` & `audfactory-1.0.9/.github/workflows/publish.yml`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,20 @@
     tags:
       - 'v*' # Push events to matching v*, i.e. v1.0, v20.15.10
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
       with:
         fetch-depth: 2
 
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: '3.8'
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install setuptools wheel twine
@@ -60,14 +60,14 @@
         CHANGELOG="${CHANGELOG//$'\n'/'%0A'}"
         CHANGELOG="${CHANGELOG//$'\r'/'%0D'}"
         echo "Got changelog: $CHANGELOG"
         echo "::set-output name=body::$CHANGELOG"
 
     - name: Create release on Github
       id: create_release
-      uses: actions/create-release@v1
+      uses: softprops/action-gh-release@v1
       env:
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
       with:
         tag_name: ${{ github.ref }}
-        release_name: Release ${{ github.ref }}
+        release_name: Release ${{ github.ref_name }}
         body: ${{ steps.changelog.outputs.body }}
```

### Comparing `audfactory-1.0.8/.github/workflows/test.yml` & `audfactory-1.0.9/.github/workflows/test.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 name: Test
 
 on:
   push:
-    branches: [ master ]
+    branches: [ main ]
   pull_request:
-    branches: [ master ]
+    branches: [ main ]
 
 jobs:
   build:
 
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ ubuntu-20.04, windows-latest, macOS-latest ]
-        python-version: [3.8]
+        python-version: [ '3.8' ]
         include:
           - os: ubuntu-latest
-            python-version: 3.7
+            python-version: '3.7'
           - os: ubuntu-latest
-            python-version: 3.9
+            python-version: '3.9'
+          - os: ubuntu-latest
+            python-version: '3.10'
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
 
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Install dependencies
       run: |
         python -V
         python -m pip install --upgrade pip
@@ -40,15 +42,15 @@
       env:
         ARTIFACTORY_USERNAME: ${{ secrets.ARTIFACTORY_USERNAME }}
         ARTIFACTORY_API_KEY: ${{ secrets.ARTIFACTORY_API_KEY }}
       run: |
         python -m pytest
 
     - name: Upload coverage to Codecov
-      uses: codecov/codecov-action@v1
+      uses: codecov/codecov-action@v3
       with:
         token: ${{ secrets.CODECOV_TOKEN }}
         file: ./coverage.xml
       if: matrix.os == 'ubuntu-20.04'
 
     - name: Test building documentation
       run: |
```

### Comparing `audfactory-1.0.8/CHANGELOG.rst` & `audfactory-1.0.9/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 1.0.9 (2022-12-23)
+--------------------------
+
+* Added: support for Python 3.10
+* Changed: split API documentation into sub-pages
+  for each function
+
+
 Version 1.0.8 (2022-01-03)
 --------------------------
 
 * Added: Python 3.9 support
 * Removed: Python 3.6 support
```

### Comparing `audfactory-1.0.8/CONTRIBUTING.rst` & `audfactory-1.0.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `audfactory-1.0.8/LICENSE` & `audfactory-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `audfactory-1.0.8/PKG-INFO` & `audfactory-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: audfactory
-Version: 1.0.8
+Version: 1.0.9
 Summary: Communicate with Artifactory
 Home-page: https://github.com/audeering/audfactory/
 Author: Johannes Wagner, Hagen Wierstorf
 Author-email: jwagner@audeering.com, hwierstorf@audeering.com
 License: MIT
 Project-URL: Documentation, https://audeering.github.io/audfactory/
 Description: ==========
@@ -49,14 +49,22 @@
         
         All notable changes to this project will be documented in this file.
         
         The format is based on `Keep a Changelog`_,
         and this project adheres to `Semantic Versioning`_.
         
         
+        Version 1.0.9 (2022-12-23)
+        --------------------------
+        
+        * Added: support for Python 3.10
+        * Changed: split API documentation into sub-pages
+          for each function
+        
+        
         Version 1.0.8 (2022-01-03)
         --------------------------
         
         * Added: Python 3.9 support
         * Removed: Python 3.6 support
         
         
@@ -363,8 +371,9 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `audfactory-1.0.8/README.rst` & `audfactory-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `audfactory-1.0.8/audfactory/__init__.py` & `audfactory-1.0.9/audfactory/__init__.py`

 * *Files identical despite different names*

### Comparing `audfactory-1.0.8/audfactory/core/api.py` & `audfactory-1.0.9/audfactory/core/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             or URL to file path on Artifactory
         type: checksum type to calculate,
             one of ``'md5'``, ``'sha1'``, ``'sha256'``
 
     Returns:
         checksum
 
-    Example:
+    Examples:
         >>> checksum(
         ...     'https://audeering.jfrog.io/artifactory/'
         ...     'data-public/emodb/db/1.1.0/db-1.1.0.zip'
         ... )
         'f4cfdbc821a070e1163d225b72b241a7'
 
     """
@@ -195,15 +195,15 @@
     Returns:
         path to local artifact
 
     Raises:
         RuntimeError: if artifact cannot be found,
             or you don't have access rights to the artifact
 
-    Example:
+    Examples:
         >>> file = download(
         ...     (
         ...         'https://audeering.jfrog.io/artifactory/'
         ...         'data-public/emodb/db/1.1.0/db-1.1.0.yaml'
         ...     ),
         ... )
         >>> os.path.basename(file)
@@ -256,15 +256,15 @@
 
     Args:
         group_id: group ID
 
     Returns:
         group ID path
 
-    Example:
+    Examples:
         >>> group_id_to_path('com.audeering.data.emodb')
         'com/audeering/data/emodb'
 
     """
     return '/'.join(group_id.split('.'))
 
 
@@ -287,15 +287,15 @@
 
     Args:
         url: URL to path on Artifactory
 
     Returns:
         Artifactory path object similar to pathlib.Path
 
-    Example:
+    Examples:
         >>> artifactory_path = path(
         ...     'https://audeering.jfrog.io/artifactory/data-public/emodb/'
         ... )
         >>> for content in artifactory_path:
         ...     print(os.path.basename(str(content)))
         ...
         db
@@ -314,15 +314,15 @@
 
     Args:
         path: group ID path
 
     Returns:
         group ID
 
-    Example:
+    Examples:
         >>> path_to_group_id('com/audeering/data/emodb')
         'com.audeering.data.emodb'
 
     """
     return '.'.join(path.split('/'))
 
 
@@ -336,15 +336,15 @@
 
     Args:
         url: REST API request URl
 
     Returns:
         server response
 
-    Example:
+    Examples:
         >>> r = rest_api_get(
         ...     'https://audeering.jfrog.io/artifactory/'
         ...     'data-public/emodb/meta/files/1.1.0/'
         ...     'files-1.1.0.zip!/db.files.csv'
         ... )
         >>> print(r.text[:35])
         file,duration,speaker,transcription
@@ -371,15 +371,15 @@
         group_id: group ID
         name: name of artifact
         version: version of artifact
 
     Returns:
         URL to location on server
 
-    Example:
+    Examples:
         >>> url(
         ...     'https://audeering.jfrog.io/artifactory',
         ...     repository='data-public',
         ...     name='emodb',
         ... )
         'https://audeering.jfrog.io/artifactory/data-public/emodb'
```

### Comparing `audfactory-1.0.8/audfactory/core/lookup.py` & `audfactory-1.0.9/audfactory/core/lookup.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         name: name of lookup table
         version: version of lookup table
 
     Raises:
         RuntimeError: if no lookup tables or no lookup
             table with the specified version can be found
 
-    Example:
+    Examples:
         >>> lookup = Lookup(
         ...     'https://artifactory.audeering.com/artifactory',
         ...     'models-public-local',
         ...     'com.audeering.models.gender.voxcnn',
         ...     version='0.2.0',
         ... )
         >>> lookup
@@ -462,15 +462,15 @@
             group_id: group ID of lookup table
             version: version of lookup table
             name: name of lookup table
 
         Returns:
             ``True`` if lookup table exists
 
-        Example:
+        Examples:
             >>> Lookup.exists(
             ...     'https://artifactory.audeering.com/artifactory',
             ...     'models-public-local',
             ...     'com.audeering.models.gender.voxcnn',
             ...     '0.1.0',
             ... )
             True
@@ -497,15 +497,15 @@
             group_id: group ID of lookup table
             params: lookup table entry in the form of ``{column: parameter}``
             name: name of lookup table
 
         Returns:
             latest version of lookup table
 
-        Example:
+        Examples:
             >>> Lookup.latest_version(
             ...     'https://artifactory.audeering.com/artifactory',
             ...     'models-public-local',
             ...     'com.audeering.models.gender.voxcnn',
             ... )
             '0.2.0'
 
@@ -538,15 +538,15 @@
             name: name of lookup table
             version: version of lookup table
             repository: repository of lookup table
 
         Returns:
             unique identifier of length 36
 
-        Example:
+        Examples:
             >>> Lookup.generate_uid(
             ...     params={0: None},
             ...     name='name',
             ...     group_id='group.id',
             ...     version='1.0.0',
             ...     repository='models-public-local',
             ... )
@@ -581,15 +581,15 @@
             group_id: group ID of lookup table
             params: lookup table entry in the form of ``{column: parameter}``
             name: name of lookup table
 
         Returns:
             available versions of lookup table
 
-        Example:
+        Examples:
             >>> Lookup.versions(
             ...     'https://artifactory.audeering.com/artifactory',
             ...     'models-public-local',
             ...     'com.audeering.models.gender.voxcnn',
             ... )
             ['0.1.0', '0.2.0']
```

### Comparing `audfactory-1.0.8/audfactory.egg-info/PKG-INFO` & `audfactory-1.0.9/audfactory.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: audfactory
-Version: 1.0.8
+Version: 1.0.9
 Summary: Communicate with Artifactory
 Home-page: https://github.com/audeering/audfactory/
 Author: Johannes Wagner, Hagen Wierstorf
 Author-email: jwagner@audeering.com, hwierstorf@audeering.com
 License: MIT
 Project-URL: Documentation, https://audeering.github.io/audfactory/
 Description: ==========
@@ -49,14 +49,22 @@
         
         All notable changes to this project will be documented in this file.
         
         The format is based on `Keep a Changelog`_,
         and this project adheres to `Semantic Versioning`_.
         
         
+        Version 1.0.9 (2022-12-23)
+        --------------------------
+        
+        * Added: support for Python 3.10
+        * Changed: split API documentation into sub-pages
+          for each function
+        
+        
         Version 1.0.8 (2022-01-03)
         --------------------------
         
         * Added: Python 3.9 support
         * Removed: Python 3.6 support
         
         
@@ -363,8 +371,9 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `audfactory-1.0.8/audfactory.egg-info/SOURCES.txt` & `audfactory-1.0.9/audfactory.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,20 +13,23 @@
 audfactory.egg-info/SOURCES.txt
 audfactory.egg-info/dependency_links.txt
 audfactory.egg-info/requires.txt
 audfactory.egg-info/top_level.txt
 audfactory/core/__init__.py
 audfactory/core/api.py
 audfactory/core/lookup.py
-docs/api-audfactory.rst
 docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
 docs/genindex.rst
 docs/index.rst
 docs/installation.rst
 docs/requirements.txt
 docs/usage.rst
+docs/_templates/autosummary/base.rst
+docs/_templates/autosummary/class.rst
+docs/_templates/autosummary/function.rst
+docs/api-src/audfactory.rst
 tests/conftest.py
 tests/requirements.txt
 tests/test_api.py
 tests/test_lookup.py
```

### Comparing `audfactory-1.0.8/docs/conf.py` & `audfactory-1.0.9/docs/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,83 @@
+import configparser
 from datetime import date
 import os
-from subprocess import check_output
+import shutil
 import sys
 
 import audeer
 
 
+config = configparser.ConfigParser()
+config.read(os.path.join('..', 'setup.cfg'))
+
+
 # Project -----------------------------------------------------------------
-project = 'audfactory'
+author = config['metadata']['author']
 copyright = f'2019-{date.today().year} audEERING GmbH'
-author = 'Hagen Wierstorf'
-# The x.y.z version read from tags
-try:
-    version = check_output(['git', 'describe', '--tags', '--always'])
-    version = version.decode().strip()
-except Exception:
-    version = '<unknown>'
-title = '{} Documentation'.format(project)
+project = config['metadata']['name']
+version = audeer.git_repo_version()
+title = 'Documentation'
 
 
 # General -----------------------------------------------------------------
 master_doc = 'index'
 extensions = []
 source_suffix = '.rst'
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+exclude_patterns = [
+    'build',
+    'tests',
+    'Thumbs.db',
+    '.DS_Store',
+    'api-src',
+]
+templates_path = ['_templates']
 pygments_style = None
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.napoleon',  # support for Google-style docstrings
+    'sphinx.ext.autosummary',
     'sphinx_autodoc_typehints',
     'sphinx.ext.viewcode',
     'sphinx.ext.intersphinx',
     'sphinx_copybutton',
     'jupyter_sphinx',
 ]
 intersphinx_mapping = {
     'audeer': ('https://audeering.github.io/audeer/', None),
+    'pandas': ('https://pandas.pydata.org/pandas-docs/stable/', None),
     'python': ('https://docs.python.org/3/', None),
-    'pandas': ('https://pandas-docs.github.io/pandas-docs-travis/', None),
 }
 # Disable Gitlab as we need to sign in
 linkcheck_ignore = [
     'https://gitlab.audeering.com',
     'http://sphinx-doc.org/',
 ]
 
+# Disable auto-generation of TOC entries in the API
+# https://github.com/sphinx-doc/sphinx/issues/6316
+toc_object_entries = False
+
 
 # HTML --------------------------------------------------------------------
 html_theme = 'sphinx_audeering_theme'
 html_theme_options = {
     'display_version': True,
     'logo_only': False,
     'footer_links': False,
 }
 html_context = {
     'display_github': True,
 }
 html_title = title
+
+
+# Copy API (sub-)module RST files to docs/api/ folder ---------------------
+audeer.rmdir('api')
+audeer.mkdir('api')
+api_src_files = audeer.list_file_names('api-src')
+api_dst_files = [
+    audeer.path('api', os.path.basename(src_file))
+    for src_file in api_src_files
+]
+for src_file, dst_file in zip(api_src_files, api_dst_files):
+    shutil.copyfile(src_file, dst_file)
```

### Comparing `audfactory-1.0.8/docs/index.rst` & `audfactory-1.0.9/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 .. Warning: the usage of genindex is a hack to get a TOC entry, see
 .. https://stackoverflow.com/a/42310803. This might break the usage of sphinx if
 .. you want to create something different than HTML output.
 .. toctree::
     :caption: API Documentation
     :hidden:
 
-    api-audfactory
+    api/audfactory
     genindex
 
 .. toctree::
     :caption: Development
     :maxdepth: 2
     :hidden:
```

### Comparing `audfactory-1.0.8/docs/usage.rst` & `audfactory-1.0.9/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `audfactory-1.0.8/setup.cfg` & `audfactory-1.0.9/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 	Topic :: Scientific/Engineering
 
 [options]
 packages = find:
 install_requires = 
 	audeer>=1.11.0
 	dohq-artifactory>=0.7.377
```

### Comparing `audfactory-1.0.8/tests/conftest.py` & `audfactory-1.0.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `audfactory-1.0.8/tests/test_api.py` & `audfactory-1.0.9/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `audfactory-1.0.8/tests/test_lookup.py` & `audfactory-1.0.9/tests/test_lookup.py`

 * *Files identical despite different names*

