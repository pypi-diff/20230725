# Comparing `tmp/gammarer.aws-daily-cost-usage-reporter-0.9.3.tar.gz` & `tmp/gammarer.aws-daily-cost-usage-reporter-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-daily-cost-usage-reporter-0.9.3.tar", last modified: Sun Jul 23 19:18:41 2023, max compression
+gzip compressed data, was "gammarer.aws-daily-cost-usage-reporter-0.9.5.tar", last modified: Tue Jul 25 19:18:39 2023, max compression
```

## Comparing `gammarer.aws-daily-cost-usage-reporter-0.9.3.tar` & `gammarer.aws-daily-cost-usage-reporter-0.9.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:18:41.796911 gammarer.aws-daily-cost-usage-reporter-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-23 19:18:25.000000 gammarer.aws-daily-cost-usage-reporter-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-23 19:18:25.000000 gammarer.aws-daily-cost-usage-reporter-0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-23 19:18:41.796911 gammarer.aws-daily-cost-usage-reporter-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-23 19:18:25.000000 gammarer.aws-daily-cost-usage-reporter-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-23 19:18:25.000000 gammarer.aws-daily-cost-usage-reporter-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 19:18:41.796911 gammarer.aws-daily-cost-usage-reporter-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-23 19:18:25.000000 gammarer.aws-daily-cost-usage-reporter-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:18:41.792911 gammarer.aws-daily-cost-usage-reporter-0.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:18:41.792911 gammarer.aws-daily-cost-usage-reporter-0.9.3/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:18:41.796911 gammarer.aws-daily-cost-usage-reporter-0.9.3/src/gammarer/aws_daily_cost_usage_reporter/
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-07-23 19:18:25.000000 gammarer.aws-daily-cost-usage-reporter-0.9.3/src/gammarer/aws_daily_cost_usage_reporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:18:41.796911 gammarer.aws-daily-cost-usage-reporter-0.9.3/src/gammarer/aws_daily_cost_usage_reporter/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-23 19:18:25.000000 gammarer.aws-daily-cost-usage-reporter-0.9.3/src/gammarer/aws_daily_cost_usage_reporter/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   233517 2023-07-23 19:18:25.000000 gammarer.aws-daily-cost-usage-reporter-0.9.3/src/gammarer/aws_daily_cost_usage_reporter/_jsii/aws-daily-cost-usage-reporter@0.9.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 19:18:25.000000 gammarer.aws-daily-cost-usage-reporter-0.9.3/src/gammarer/aws_daily_cost_usage_reporter/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:18:41.796911 gammarer.aws-daily-cost-usage-reporter-0.9.3/src/gammarer.aws_daily_cost_usage_reporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-23 19:18:41.000000 gammarer.aws-daily-cost-usage-reporter-0.9.3/src/gammarer.aws_daily_cost_usage_reporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-23 19:18:41.000000 gammarer.aws-daily-cost-usage-reporter-0.9.3/src/gammarer.aws_daily_cost_usage_reporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 19:18:41.000000 gammarer.aws-daily-cost-usage-reporter-0.9.3/src/gammarer.aws_daily_cost_usage_reporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-23 19:18:41.000000 gammarer.aws-daily-cost-usage-reporter-0.9.3/src/gammarer.aws_daily_cost_usage_reporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-23 19:18:41.000000 gammarer.aws-daily-cost-usage-reporter-0.9.3/src/gammarer.aws_daily_cost_usage_reporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:18:39.001282 gammarer.aws-daily-cost-usage-reporter-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-25 19:18:22.000000 gammarer.aws-daily-cost-usage-reporter-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 19:18:22.000000 gammarer.aws-daily-cost-usage-reporter-0.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-25 19:18:39.001282 gammarer.aws-daily-cost-usage-reporter-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-25 19:18:22.000000 gammarer.aws-daily-cost-usage-reporter-0.9.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-25 19:18:22.000000 gammarer.aws-daily-cost-usage-reporter-0.9.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:18:39.001282 gammarer.aws-daily-cost-usage-reporter-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-25 19:18:22.000000 gammarer.aws-daily-cost-usage-reporter-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:18:39.001282 gammarer.aws-daily-cost-usage-reporter-0.9.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:18:39.001282 gammarer.aws-daily-cost-usage-reporter-0.9.5/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:18:39.001282 gammarer.aws-daily-cost-usage-reporter-0.9.5/src/gammarer/aws_daily_cost_usage_reporter/
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-07-25 19:18:22.000000 gammarer.aws-daily-cost-usage-reporter-0.9.5/src/gammarer/aws_daily_cost_usage_reporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:18:39.001282 gammarer.aws-daily-cost-usage-reporter-0.9.5/src/gammarer/aws_daily_cost_usage_reporter/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-25 19:18:22.000000 gammarer.aws-daily-cost-usage-reporter-0.9.5/src/gammarer/aws_daily_cost_usage_reporter/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   233518 2023-07-25 19:18:22.000000 gammarer.aws-daily-cost-usage-reporter-0.9.5/src/gammarer/aws_daily_cost_usage_reporter/_jsii/aws-daily-cost-usage-reporter@0.9.5.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:18:22.000000 gammarer.aws-daily-cost-usage-reporter-0.9.5/src/gammarer/aws_daily_cost_usage_reporter/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:18:39.001282 gammarer.aws-daily-cost-usage-reporter-0.9.5/src/gammarer.aws_daily_cost_usage_reporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-25 19:18:38.000000 gammarer.aws-daily-cost-usage-reporter-0.9.5/src/gammarer.aws_daily_cost_usage_reporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-25 19:18:38.000000 gammarer.aws-daily-cost-usage-reporter-0.9.5/src/gammarer.aws_daily_cost_usage_reporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:18:38.000000 gammarer.aws-daily-cost-usage-reporter-0.9.5/src/gammarer.aws_daily_cost_usage_reporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-25 19:18:38.000000 gammarer.aws-daily-cost-usage-reporter-0.9.5/src/gammarer.aws_daily_cost_usage_reporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 19:18:38.000000 gammarer.aws-daily-cost-usage-reporter-0.9.5/src/gammarer.aws_daily_cost_usage_reporter.egg-info/top_level.txt
```

### Comparing `gammarer.aws-daily-cost-usage-reporter-0.9.3/LICENSE` & `gammarer.aws-daily-cost-usage-reporter-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-daily-cost-usage-reporter-0.9.3/PKG-INFO` & `gammarer.aws-daily-cost-usage-reporter-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-daily-cost-usage-reporter
-Version: 0.9.3
+Version: 0.9.5
 Summary: Cost & Usage Reports
 Home-page: https://github.com/yicr/aws-daily-cost-usage-reporter.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-daily-cost-usage-reporter.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-daily-cost-usage-reporter-0.9.3/README.md` & `gammarer.aws-daily-cost-usage-reporter-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-daily-cost-usage-reporter-0.9.3/setup.py` & `gammarer.aws-daily-cost-usage-reporter-0.9.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-daily-cost-usage-reporter",
-    "version": "0.9.3",
+    "version": "0.9.5",
     "description": "Cost & Usage Reports",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-daily-cost-usage-reporter.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_daily_cost_usage_reporter",
         "gammarer.aws_daily_cost_usage_reporter._jsii"
     ],
     "package_data": {
         "gammarer.aws_daily_cost_usage_reporter._jsii": [
-            "aws-daily-cost-usage-reporter@0.9.3.jsii.tgz"
+            "aws-daily-cost-usage-reporter@0.9.5.jsii.tgz"
         ],
         "gammarer.aws_daily_cost_usage_reporter": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `gammarer.aws-daily-cost-usage-reporter-0.9.3/src/gammarer/aws_daily_cost_usage_reporter/__init__.py` & `gammarer.aws-daily-cost-usage-reporter-0.9.5/src/gammarer/aws_daily_cost_usage_reporter/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-daily-cost-usage-reporter-0.9.3/src/gammarer.aws_daily_cost_usage_reporter.egg-info/PKG-INFO` & `gammarer.aws-daily-cost-usage-reporter-0.9.5/src/gammarer.aws_daily_cost_usage_reporter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-daily-cost-usage-reporter
-Version: 0.9.3
+Version: 0.9.5
 Summary: Cost & Usage Reports
 Home-page: https://github.com/yicr/aws-daily-cost-usage-reporter.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-daily-cost-usage-reporter.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-daily-cost-usage-reporter-0.9.3/src/gammarer.aws_daily_cost_usage_reporter.egg-info/SOURCES.txt` & `gammarer.aws-daily-cost-usage-reporter-0.9.5/src/gammarer.aws_daily_cost_usage_reporter.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_daily_cost_usage_reporter.egg-info/SOURCES.txt
 src/gammarer.aws_daily_cost_usage_reporter.egg-info/dependency_links.txt
 src/gammarer.aws_daily_cost_usage_reporter.egg-info/requires.txt
 src/gammarer.aws_daily_cost_usage_reporter.egg-info/top_level.txt
 src/gammarer/aws_daily_cost_usage_reporter/__init__.py
 src/gammarer/aws_daily_cost_usage_reporter/py.typed
 src/gammarer/aws_daily_cost_usage_reporter/_jsii/__init__.py
-src/gammarer/aws_daily_cost_usage_reporter/_jsii/aws-daily-cost-usage-reporter@0.9.3.jsii.tgz
+src/gammarer/aws_daily_cost_usage_reporter/_jsii/aws-daily-cost-usage-reporter@0.9.5.jsii.tgz
```

