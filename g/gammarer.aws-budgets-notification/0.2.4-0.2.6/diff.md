# Comparing `tmp/gammarer.aws-budgets-notification-0.2.4.tar.gz` & `tmp/gammarer.aws-budgets-notification-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-budgets-notification-0.2.4.tar", last modified: Sun Jul 23 19:20:10 2023, max compression
+gzip compressed data, was "gammarer.aws-budgets-notification-0.2.6.tar", last modified: Tue Jul 25 19:17:23 2023, max compression
```

## Comparing `gammarer.aws-budgets-notification-0.2.4.tar` & `gammarer.aws-budgets-notification-0.2.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:20:10.662702 gammarer.aws-budgets-notification-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-23 19:19:56.000000 gammarer.aws-budgets-notification-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-23 19:19:56.000000 gammarer.aws-budgets-notification-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-23 19:20:10.662702 gammarer.aws-budgets-notification-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-23 19:19:56.000000 gammarer.aws-budgets-notification-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-23 19:19:56.000000 gammarer.aws-budgets-notification-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 19:20:10.662702 gammarer.aws-budgets-notification-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-23 19:19:56.000000 gammarer.aws-budgets-notification-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:20:10.658702 gammarer.aws-budgets-notification-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:20:10.658702 gammarer.aws-budgets-notification-0.2.4/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:20:10.662702 gammarer.aws-budgets-notification-0.2.4/src/gammarer/aws_budgets_notification/
--rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-07-23 19:19:56.000000 gammarer.aws-budgets-notification-0.2.4/src/gammarer/aws_budgets_notification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:20:10.662702 gammarer.aws-budgets-notification-0.2.4/src/gammarer/aws_budgets_notification/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-23 19:19:56.000000 gammarer.aws-budgets-notification-0.2.4/src/gammarer/aws_budgets_notification/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    73875 2023-07-23 19:19:56.000000 gammarer.aws-budgets-notification-0.2.4/src/gammarer/aws_budgets_notification/_jsii/aws-budgets-notification@0.2.4.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 19:19:56.000000 gammarer.aws-budgets-notification-0.2.4/src/gammarer/aws_budgets_notification/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:20:10.662702 gammarer.aws-budgets-notification-0.2.4/src/gammarer.aws_budgets_notification.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-23 19:20:10.000000 gammarer.aws-budgets-notification-0.2.4/src/gammarer.aws_budgets_notification.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-23 19:20:10.000000 gammarer.aws-budgets-notification-0.2.4/src/gammarer.aws_budgets_notification.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 19:20:10.000000 gammarer.aws-budgets-notification-0.2.4/src/gammarer.aws_budgets_notification.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-23 19:20:10.000000 gammarer.aws-budgets-notification-0.2.4/src/gammarer.aws_budgets_notification.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-23 19:20:10.000000 gammarer.aws-budgets-notification-0.2.4/src/gammarer.aws_budgets_notification.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:17:23.375666 gammarer.aws-budgets-notification-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-25 19:17:12.000000 gammarer.aws-budgets-notification-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 19:17:12.000000 gammarer.aws-budgets-notification-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-25 19:17:23.375666 gammarer.aws-budgets-notification-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-25 19:17:12.000000 gammarer.aws-budgets-notification-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-25 19:17:12.000000 gammarer.aws-budgets-notification-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:17:23.375666 gammarer.aws-budgets-notification-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-25 19:17:12.000000 gammarer.aws-budgets-notification-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:17:23.375666 gammarer.aws-budgets-notification-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:17:23.375666 gammarer.aws-budgets-notification-0.2.6/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:17:23.375666 gammarer.aws-budgets-notification-0.2.6/src/gammarer/aws_budgets_notification/
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-07-25 19:17:12.000000 gammarer.aws-budgets-notification-0.2.6/src/gammarer/aws_budgets_notification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:17:23.375666 gammarer.aws-budgets-notification-0.2.6/src/gammarer/aws_budgets_notification/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-25 19:17:12.000000 gammarer.aws-budgets-notification-0.2.6/src/gammarer/aws_budgets_notification/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73873 2023-07-25 19:17:12.000000 gammarer.aws-budgets-notification-0.2.6/src/gammarer/aws_budgets_notification/_jsii/aws-budgets-notification@0.2.6.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:17:12.000000 gammarer.aws-budgets-notification-0.2.6/src/gammarer/aws_budgets_notification/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:17:23.375666 gammarer.aws-budgets-notification-0.2.6/src/gammarer.aws_budgets_notification.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-25 19:17:23.000000 gammarer.aws-budgets-notification-0.2.6/src/gammarer.aws_budgets_notification.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-25 19:17:23.000000 gammarer.aws-budgets-notification-0.2.6/src/gammarer.aws_budgets_notification.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:17:23.000000 gammarer.aws-budgets-notification-0.2.6/src/gammarer.aws_budgets_notification.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-25 19:17:23.000000 gammarer.aws-budgets-notification-0.2.6/src/gammarer.aws_budgets_notification.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 19:17:23.000000 gammarer.aws-budgets-notification-0.2.6/src/gammarer.aws_budgets_notification.egg-info/top_level.txt
```

### Comparing `gammarer.aws-budgets-notification-0.2.4/LICENSE` & `gammarer.aws-budgets-notification-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-budgets-notification-0.2.4/PKG-INFO` & `gammarer.aws-budgets-notification-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-budgets-notification
-Version: 0.2.4
+Version: 0.2.6
 Summary: AWS Budgets Notification
 Home-page: https://github.com/yicr/aws-budgets-notification.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-budgets-notification.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-budgets-notification-0.2.4/README.md` & `gammarer.aws-budgets-notification-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-budgets-notification-0.2.4/setup.py` & `gammarer.aws-budgets-notification-0.2.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-budgets-notification",
-    "version": "0.2.4",
+    "version": "0.2.6",
     "description": "AWS Budgets Notification",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-budgets-notification.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_budgets_notification",
         "gammarer.aws_budgets_notification._jsii"
     ],
     "package_data": {
         "gammarer.aws_budgets_notification._jsii": [
-            "aws-budgets-notification@0.2.4.jsii.tgz"
+            "aws-budgets-notification@0.2.6.jsii.tgz"
         ],
         "gammarer.aws_budgets_notification": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `gammarer.aws-budgets-notification-0.2.4/src/gammarer/aws_budgets_notification/__init__.py` & `gammarer.aws-budgets-notification-0.2.6/src/gammarer/aws_budgets_notification/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-budgets-notification-0.2.4/src/gammarer.aws_budgets_notification.egg-info/PKG-INFO` & `gammarer.aws-budgets-notification-0.2.6/src/gammarer.aws_budgets_notification.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-budgets-notification
-Version: 0.2.4
+Version: 0.2.6
 Summary: AWS Budgets Notification
 Home-page: https://github.com/yicr/aws-budgets-notification.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-budgets-notification.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-budgets-notification-0.2.4/src/gammarer.aws_budgets_notification.egg-info/SOURCES.txt` & `gammarer.aws-budgets-notification-0.2.6/src/gammarer.aws_budgets_notification.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_budgets_notification.egg-info/SOURCES.txt
 src/gammarer.aws_budgets_notification.egg-info/dependency_links.txt
 src/gammarer.aws_budgets_notification.egg-info/requires.txt
 src/gammarer.aws_budgets_notification.egg-info/top_level.txt
 src/gammarer/aws_budgets_notification/__init__.py
 src/gammarer/aws_budgets_notification/py.typed
 src/gammarer/aws_budgets_notification/_jsii/__init__.py
-src/gammarer/aws_budgets_notification/_jsii/aws-budgets-notification@0.2.4.jsii.tgz
+src/gammarer/aws_budgets_notification/_jsii/aws-budgets-notification@0.2.6.jsii.tgz
```

