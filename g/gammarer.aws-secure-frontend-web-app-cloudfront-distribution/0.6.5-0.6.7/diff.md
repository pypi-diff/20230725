# Comparing `tmp/gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5.tar.gz` & `tmp/gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5.tar", last modified: Sun Jul 23 18:27:31 2023, max compression
+gzip compressed data, was "gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7.tar", last modified: Tue Jul 25 18:27:42 2023, max compression
```

## Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5.tar` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 18:27:31.528262 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-23 18:27:17.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-23 18:27:17.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-23 18:27:31.528262 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-23 18:27:17.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-23 18:27:17.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 18:27:31.528262 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-23 18:27:17.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 18:27:31.524262 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 18:27:31.524262 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 18:27:31.524262 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-07-23 18:27:17.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 18:27:31.528262 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-23 18:27:17.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20673 2023-07-23 18:27:17.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@0.6.5.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 18:27:17.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 18:27:31.524262 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-23 18:27:31.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-23 18:27:31.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 18:27:31.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-23 18:27:31.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-23 18:27:31.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:27:42.627440 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-25 18:27:27.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 18:27:27.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-25 18:27:42.627440 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-25 18:27:27.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-25 18:27:27.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 18:27:42.627440 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-25 18:27:27.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:27:42.623440 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:27:42.623440 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:27:42.627440 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-07-25 18:27:27.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:27:42.627440 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-25 18:27:27.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20670 2023-07-25 18:27:27.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@0.6.7.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:27:27.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:27:42.627440 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-25 18:27:42.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-25 18:27:42.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:27:42.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-25 18:27:42.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 18:27:42.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/top_level.txt
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5/LICENSE` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5/PKG-INFO` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-frontend-web-app-cloudfront-distribution
-Version: 0.6.5
+Version: 0.6.7
 Summary: AWS CloudFront distribution for frontend web app (spa) optimized.
 Home-page: https://github.com/yicr/aws-secure-frontend-web-app-cloudfront-distribution.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-secure-frontend-web-app-cloudfront-distribution.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5/README.md` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5/setup.py` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-secure-frontend-web-app-cloudfront-distribution",
-    "version": "0.6.5",
+    "version": "0.6.7",
     "description": "AWS CloudFront distribution for frontend web app (spa) optimized.",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-secure-frontend-web-app-cloudfront-distribution.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_secure_frontend_web_app_cloudfront_distribution",
         "gammarer.aws_secure_frontend_web_app_cloudfront_distribution._jsii"
     ],
     "package_data": {
         "gammarer.aws_secure_frontend_web_app_cloudfront_distribution._jsii": [
-            "aws-secure-frontend-web-app-cloudfront-distribution@0.6.5.jsii.tgz"
+            "aws-secure-frontend-web-app-cloudfront-distribution@0.6.7.jsii.tgz"
         ],
         "gammarer.aws_secure_frontend_web_app_cloudfront_distribution": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/PKG-INFO` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-frontend-web-app-cloudfront-distribution
-Version: 0.6.5
+Version: 0.6.7
 Summary: AWS CloudFront distribution for frontend web app (spa) optimized.
 Home-page: https://github.com/yicr/aws-secure-frontend-web-app-cloudfront-distribution.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-secure-frontend-web-app-cloudfront-distribution.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.5/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-0.6.7/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt
 src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/dependency_links.txt
 src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/requires.txt
 src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/top_level.txt
 src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py
 src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/py.typed
 src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py
-src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@0.6.5.jsii.tgz
+src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@0.6.7.jsii.tgz
```

