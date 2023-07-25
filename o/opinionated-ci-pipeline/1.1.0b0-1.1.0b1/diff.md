# Comparing `tmp/opinionated-ci-pipeline-1.1.0b0.tar.gz` & `tmp/opinionated-ci-pipeline-1.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opinionated-ci-pipeline-1.1.0b0.tar", last modified: Tue Apr  4 10:59:29 2023, max compression
+gzip compressed data, was "opinionated-ci-pipeline-1.1.0b1.tar", last modified: Tue Jul 25 14:10:04 2023, max compression
```

## Comparing `opinionated-ci-pipeline-1.1.0b0.tar` & `opinionated-ci-pipeline-1.1.0b1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:59:29.911831 opinionated-ci-pipeline-1.1.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-04 10:59:14.000000 opinionated-ci-pipeline-1.1.0b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-04 10:59:14.000000 opinionated-ci-pipeline-1.1.0b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11098 2023-04-04 10:59:29.911831 opinionated-ci-pipeline-1.1.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-04-04 10:59:14.000000 opinionated-ci-pipeline-1.1.0b0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-04 10:59:14.000000 opinionated-ci-pipeline-1.1.0b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 10:59:29.911831 opinionated-ci-pipeline-1.1.0b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-04 10:59:14.000000 opinionated-ci-pipeline-1.1.0b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:59:29.907831 opinionated-ci-pipeline-1.1.0b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:59:29.907831 opinionated-ci-pipeline-1.1.0b0/src/opinionated_ci_pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)    86493 2023-04-04 10:59:14.000000 opinionated-ci-pipeline-1.1.0b0/src/opinionated_ci_pipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:59:29.911831 opinionated-ci-pipeline-1.1.0b0/src/opinionated_ci_pipeline/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-04 10:59:14.000000 opinionated-ci-pipeline-1.1.0b0/src/opinionated_ci_pipeline/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   378330 2023-04-04 10:59:14.000000 opinionated-ci-pipeline-1.1.0b0/src/opinionated_ci_pipeline/_jsii/opinionated-ci-pipeline@1.1.0-beta.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 10:59:14.000000 opinionated-ci-pipeline-1.1.0b0/src/opinionated_ci_pipeline/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:59:29.911831 opinionated-ci-pipeline-1.1.0b0/src/opinionated_ci_pipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11098 2023-04-04 10:59:29.000000 opinionated-ci-pipeline-1.1.0b0/src/opinionated_ci_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-04 10:59:29.000000 opinionated-ci-pipeline-1.1.0b0/src/opinionated_ci_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 10:59:29.000000 opinionated-ci-pipeline-1.1.0b0/src/opinionated_ci_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-04 10:59:29.000000 opinionated-ci-pipeline-1.1.0b0/src/opinionated_ci_pipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-04 10:59:29.000000 opinionated-ci-pipeline-1.1.0b0/src/opinionated_ci_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:10:04.698379 opinionated-ci-pipeline-1.1.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-25 14:09:52.000000 opinionated-ci-pipeline-1.1.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 14:09:52.000000 opinionated-ci-pipeline-1.1.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11106 2023-07-25 14:10:04.698379 opinionated-ci-pipeline-1.1.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-07-25 14:09:52.000000 opinionated-ci-pipeline-1.1.0b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-25 14:09:52.000000 opinionated-ci-pipeline-1.1.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 14:10:04.698379 opinionated-ci-pipeline-1.1.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-25 14:09:52.000000 opinionated-ci-pipeline-1.1.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:10:04.698379 opinionated-ci-pipeline-1.1.0b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:10:04.698379 opinionated-ci-pipeline-1.1.0b1/src/opinionated_ci_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)    86501 2023-07-25 14:09:52.000000 opinionated-ci-pipeline-1.1.0b1/src/opinionated_ci_pipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:10:04.698379 opinionated-ci-pipeline-1.1.0b1/src/opinionated_ci_pipeline/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-25 14:09:52.000000 opinionated-ci-pipeline-1.1.0b1/src/opinionated_ci_pipeline/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   378056 2023-07-25 14:09:52.000000 opinionated-ci-pipeline-1.1.0b1/src/opinionated_ci_pipeline/_jsii/opinionated-ci-pipeline@1.1.0-beta.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 14:09:52.000000 opinionated-ci-pipeline-1.1.0b1/src/opinionated_ci_pipeline/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:10:04.698379 opinionated-ci-pipeline-1.1.0b1/src/opinionated_ci_pipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11106 2023-07-25 14:10:04.000000 opinionated-ci-pipeline-1.1.0b1/src/opinionated_ci_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-25 14:10:04.000000 opinionated-ci-pipeline-1.1.0b1/src/opinionated_ci_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 14:10:04.000000 opinionated-ci-pipeline-1.1.0b1/src/opinionated_ci_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-25 14:10:04.000000 opinionated-ci-pipeline-1.1.0b1/src/opinionated_ci_pipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-25 14:10:04.000000 opinionated-ci-pipeline-1.1.0b1/src/opinionated_ci_pipeline.egg-info/top_level.txt
```

### Comparing `opinionated-ci-pipeline-1.1.0b0/LICENSE` & `opinionated-ci-pipeline-1.1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `opinionated-ci-pipeline-1.1.0b0/PKG-INFO` & `opinionated-ci-pipeline-1.1.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opinionated-ci-pipeline
-Version: 1.1.0b0
+Version: 1.1.0b1
 Summary: CI/CD on AWS with feature-branch builds, developer-environment deployments, and build status notifications.
 Home-page: https://github.com/merapar/opinionated-ci-pipeline.git
 Author: Maciej Radzikowski<maciej.radzikowski@merapar.com>
 License: MIT
 Project-URL: Source, https://github.com/merapar/opinionated-ci-pipeline.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -24,15 +24,15 @@
 # Opinionated CDK CI Pipeline
 
 [![NPM](https://img.shields.io/npm/v/opinionated-ci-pipeline?color=blue)](https://www.npmjs.com/package/opinionated-ci-pipeline)
 [![PyPI](https://img.shields.io/pypi/v/opinionated-ci-pipeline?color=blue)](https://pypi.org/project/opinionated-ci-pipeline/)
 
 CI/CD utilizing [CDK Pipelines](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.pipelines-readme.html).
 
-See the [announcement blog post](https://merapar.com/finally-the-cdk-ci-pipeline-that-serverless-deserves/) for examples and architecture diagrams.
+See the [announcement blog post](https://articles.merapar.com/finally-the-cdk-ci-pipeline-that-serverless-deserves) for examples and architecture diagrams.
 
 Features:
 
 * pipeline deploying application from the default branch
   to multiple environments on multiple accounts,
 * feature branch deployments to ephemeral environments,
 * development environments deployments from the local CLI,
```

### Comparing `opinionated-ci-pipeline-1.1.0b0/README.md` & `opinionated-ci-pipeline-1.1.0b1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Opinionated CDK CI Pipeline
 
 [![NPM](https://img.shields.io/npm/v/opinionated-ci-pipeline?color=blue)](https://www.npmjs.com/package/opinionated-ci-pipeline)
 [![PyPI](https://img.shields.io/pypi/v/opinionated-ci-pipeline?color=blue)](https://pypi.org/project/opinionated-ci-pipeline/)
 
 CI/CD utilizing [CDK Pipelines](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.pipelines-readme.html).
 
-See the [announcement blog post](https://merapar.com/finally-the-cdk-ci-pipeline-that-serverless-deserves/) for examples and architecture diagrams.
+See the [announcement blog post](https://articles.merapar.com/finally-the-cdk-ci-pipeline-that-serverless-deserves) for examples and architecture diagrams.
 
 Features:
 
 * pipeline deploying application from the default branch
   to multiple environments on multiple accounts,
 * feature branch deployments to ephemeral environments,
 * development environments deployments from the local CLI,
```

### Comparing `opinionated-ci-pipeline-1.1.0b0/setup.py` & `opinionated-ci-pipeline-1.1.0b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "opinionated-ci-pipeline",
-    "version": "1.1.0.b0",
+    "version": "1.1.0.b1",
     "description": "CI/CD on AWS with feature-branch builds, developer-environment deployments, and build status notifications.",
     "license": "MIT",
     "url": "https://github.com/merapar/opinionated-ci-pipeline.git",
     "long_description_content_type": "text/markdown",
     "author": "Maciej Radzikowski<maciej.radzikowski@merapar.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "opinionated_ci_pipeline",
         "opinionated_ci_pipeline._jsii"
     ],
     "package_data": {
         "opinionated_ci_pipeline._jsii": [
-            "opinionated-ci-pipeline@1.1.0-beta.0.jsii.tgz"
+            "opinionated-ci-pipeline@1.1.0-beta.1.jsii.tgz"
         ],
         "opinionated_ci_pipeline": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `opinionated-ci-pipeline-1.1.0b0/src/opinionated_ci_pipeline/__init__.py` & `opinionated-ci-pipeline-1.1.0b1/src/opinionated_ci_pipeline/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Opinionated CDK CI Pipeline
 
 [![NPM](https://img.shields.io/npm/v/opinionated-ci-pipeline?color=blue)](https://www.npmjs.com/package/opinionated-ci-pipeline)
 [![PyPI](https://img.shields.io/pypi/v/opinionated-ci-pipeline?color=blue)](https://pypi.org/project/opinionated-ci-pipeline/)
 
 CI/CD utilizing [CDK Pipelines](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.pipelines-readme.html).
 
-See the [announcement blog post](https://merapar.com/finally-the-cdk-ci-pipeline-that-serverless-deserves/) for examples and architecture diagrams.
+See the [announcement blog post](https://articles.merapar.com/finally-the-cdk-ci-pipeline-that-serverless-deserves) for examples and architecture diagrams.
 
 Features:
 
 * pipeline deploying application from the default branch
   to multiple environments on multiple accounts,
 * feature branch deployments to ephemeral environments,
 * development environments deployments from the local CLI,
```

### Comparing `opinionated-ci-pipeline-1.1.0b0/src/opinionated_ci_pipeline.egg-info/PKG-INFO` & `opinionated-ci-pipeline-1.1.0b1/src/opinionated_ci_pipeline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opinionated-ci-pipeline
-Version: 1.1.0b0
+Version: 1.1.0b1
 Summary: CI/CD on AWS with feature-branch builds, developer-environment deployments, and build status notifications.
 Home-page: https://github.com/merapar/opinionated-ci-pipeline.git
 Author: Maciej Radzikowski<maciej.radzikowski@merapar.com>
 License: MIT
 Project-URL: Source, https://github.com/merapar/opinionated-ci-pipeline.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -24,15 +24,15 @@
 # Opinionated CDK CI Pipeline
 
 [![NPM](https://img.shields.io/npm/v/opinionated-ci-pipeline?color=blue)](https://www.npmjs.com/package/opinionated-ci-pipeline)
 [![PyPI](https://img.shields.io/pypi/v/opinionated-ci-pipeline?color=blue)](https://pypi.org/project/opinionated-ci-pipeline/)
 
 CI/CD utilizing [CDK Pipelines](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.pipelines-readme.html).
 
-See the [announcement blog post](https://merapar.com/finally-the-cdk-ci-pipeline-that-serverless-deserves/) for examples and architecture diagrams.
+See the [announcement blog post](https://articles.merapar.com/finally-the-cdk-ci-pipeline-that-serverless-deserves) for examples and architecture diagrams.
 
 Features:
 
 * pipeline deploying application from the default branch
   to multiple environments on multiple accounts,
 * feature branch deployments to ephemeral environments,
 * development environments deployments from the local CLI,
```

