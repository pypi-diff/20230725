# Comparing `tmp/mypy-boto3-emr-serverless-1.28.0.tar.gz` & `tmp/mypy-boto3-emr-serverless-1.28.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-emr-serverless-1.28.0.tar", last modified: Thu Jul  6 20:59:33 2023, max compression
+gzip compressed data, was "mypy-boto3-emr-serverless-1.28.11.tar", last modified: Tue Jul 25 19:49:13 2023, max compression
```

## Comparing `mypy-boto3-emr-serverless-1.28.0.tar` & `mypy-boto3-emr-serverless-1.28.11.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:33.738299 mypy-boto3-emr-serverless-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:40:41.000000 mypy-boto3-emr-serverless-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14975 2023-07-06 20:59:33.734300 mypy-boto3-emr-serverless-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13463 2023-07-06 20:40:41.000000 mypy-boto3-emr-serverless-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:33.726299 mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-06 20:40:41.000000 mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-06 20:40:41.000000 mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-06 20:40:41.000000 mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14177 2023-07-06 20:40:41.000000 mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14153 2023-07-06 20:40:41.000000 mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-07-06 20:40:42.000000 mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-07-06 20:40:42.000000 mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-06 20:40:41.000000 mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-06 20:40:41.000000 mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:40:41.000000 mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19961 2023-07-06 20:40:42.000000 mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-07-06 20:40:42.000000 mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:40:41.000000 mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:33.734300 mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14975 2023-07-06 20:59:33.000000 mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-06 20:59:33.000000 mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:33.000000 mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:33.000000 mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:33.000000 mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 20:59:33.000000 mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:33.738299 mypy-boto3-emr-serverless-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-06 20:40:41.000000 mypy-boto3-emr-serverless-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:13.821034 mypy-boto3-emr-serverless-1.28.11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-25 19:47:55.000000 mypy-boto3-emr-serverless-1.28.11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15597 2023-07-25 19:49:13.821034 mypy-boto3-emr-serverless-1.28.11/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14083 2023-07-25 19:47:55.000000 mypy-boto3-emr-serverless-1.28.11/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:13.821034 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-25 19:47:55.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-25 19:47:55.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-25 19:47:55.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14226 2023-07-25 19:47:55.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-07-25 19:47:55.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-07-25 19:47:56.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-07-25 19:47:55.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-25 19:47:55.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-25 19:47:55.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:47:55.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23139 2023-07-25 19:47:56.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23114 2023-07-25 19:47:56.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-25 19:47:55.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:13.821034 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15597 2023-07-25 19:49:13.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-25 19:49:13.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:49:13.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:49:13.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-25 19:49:13.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-25 19:49:13.000000 mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:49:13.821034 mypy-boto3-emr-serverless-1.28.11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-25 19:47:55.000000 mypy-boto3-emr-serverless-1.28.11/setup.py
```

### Comparing `mypy-boto3-emr-serverless-1.28.0/LICENSE` & `mypy-boto3-emr-serverless-1.28.11/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.0/PKG-INFO` & `mypy-boto3-emr-serverless-1.28.11/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-serverless
-Version: 1.28.0
-Summary: Type annotations for boto3.EMRServerless 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.11
+Summary: Type annotations for boto3.EMRServerless 1.28.11 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr-serverless?color=blue)](https://pypistats.org/packages/mypy-boto3-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRServerless 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
+[boto3.EMRServerless 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-emr-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -326,60 +326,76 @@
 
 `mypy_boto3_emr_serverless.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_emr_serverless.type_defs import (
     ApplicationSummaryTypeDef,
+    AutoStartConfigOutputTypeDef,
+    AutoStopConfigOutputTypeDef,
+    ImageConfigurationTypeDef,
+    MaximumAllowedResourcesOutputTypeDef,
+    NetworkConfigurationOutputTypeDef,
     AutoStartConfigTypeDef,
     AutoStopConfigTypeDef,
-    ImageConfigurationTypeDef,
-    MaximumAllowedResourcesTypeDef,
-    NetworkConfigurationTypeDef,
     CancelJobRunRequestRequestTypeDef,
-    CancelJobRunResponseTypeDef,
+    ResponseMetadataTypeDef,
+    CloudWatchLoggingConfigurationOutputTypeDef,
+    CloudWatchLoggingConfigurationTypeDef,
+    ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     ImageConfigurationInputTypeDef,
-    CreateApplicationResponseTypeDef,
+    MaximumAllowedResourcesTypeDef,
+    NetworkConfigurationTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetDashboardForJobRunRequestRequestTypeDef,
-    GetDashboardForJobRunResponseTypeDef,
     GetJobRunRequestRequestTypeDef,
+    HiveOutputTypeDef,
     HiveTypeDef,
+    WorkerResourceConfigOutputTypeDef,
     WorkerResourceConfigTypeDef,
+    SparkSubmitOutputTypeDef,
     SparkSubmitTypeDef,
     JobRunSummaryTypeDef,
     ResourceUtilizationTypeDef,
     TotalResourceUtilizationTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationsRequestRequestTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
     ListJobRunsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    ManagedPersistenceMonitoringConfigurationOutputTypeDef,
     ManagedPersistenceMonitoringConfigurationTypeDef,
+    S3MonitoringConfigurationOutputTypeDef,
     S3MonitoringConfigurationTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     StartApplicationRequestRequestTypeDef,
-    StartJobRunResponseTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ListApplicationsResponseTypeDef,
     WorkerTypeSpecificationTypeDef,
+    CancelJobRunResponseTypeDef,
+    CreateApplicationResponseTypeDef,
+    GetDashboardForJobRunResponseTypeDef,
+    ListApplicationsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartJobRunResponseTypeDef,
     WorkerTypeSpecificationInputTypeDef,
+    InitialCapacityConfigOutputTypeDef,
     InitialCapacityConfigTypeDef,
+    JobDriverOutputTypeDef,
     JobDriverTypeDef,
     ListJobRunsResponseTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    ListJobRunsRequestListJobRunsPaginateTypeDef,
+    MonitoringConfigurationOutputTypeDef,
     MonitoringConfigurationTypeDef,
     ApplicationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
+    ConfigurationOverridesOutputTypeDef,
     ConfigurationOverridesTypeDef,
     GetApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     JobRunTypeDef,
     StartJobRunRequestRequestTypeDef,
     GetJobRunResponseTypeDef,
 )
```

### Comparing `mypy-boto3-emr-serverless-1.28.0/README.md` & `mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-emr-serverless
+Version: 1.28.11
+Summary: Type annotations for boto3.EMRServerless 1.28.11 service generated with mypy-boto3-builder 7.15.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 emr-serverless type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-emr-serverless"></a>
 
 # mypy-boto3-emr-serverless
 
 [![PyPI - mypy-boto3-emr-serverless](https://img.shields.io/pypi/v/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr-serverless?color=blue)](https://pypistats.org/packages/mypy-boto3-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRServerless 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
+[boto3.EMRServerless 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-emr-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -294,60 +326,76 @@
 
 `mypy_boto3_emr_serverless.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_emr_serverless.type_defs import (
     ApplicationSummaryTypeDef,
+    AutoStartConfigOutputTypeDef,
+    AutoStopConfigOutputTypeDef,
+    ImageConfigurationTypeDef,
+    MaximumAllowedResourcesOutputTypeDef,
+    NetworkConfigurationOutputTypeDef,
     AutoStartConfigTypeDef,
     AutoStopConfigTypeDef,
-    ImageConfigurationTypeDef,
-    MaximumAllowedResourcesTypeDef,
-    NetworkConfigurationTypeDef,
     CancelJobRunRequestRequestTypeDef,
-    CancelJobRunResponseTypeDef,
+    ResponseMetadataTypeDef,
+    CloudWatchLoggingConfigurationOutputTypeDef,
+    CloudWatchLoggingConfigurationTypeDef,
+    ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     ImageConfigurationInputTypeDef,
-    CreateApplicationResponseTypeDef,
+    MaximumAllowedResourcesTypeDef,
+    NetworkConfigurationTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetDashboardForJobRunRequestRequestTypeDef,
-    GetDashboardForJobRunResponseTypeDef,
     GetJobRunRequestRequestTypeDef,
+    HiveOutputTypeDef,
     HiveTypeDef,
+    WorkerResourceConfigOutputTypeDef,
     WorkerResourceConfigTypeDef,
+    SparkSubmitOutputTypeDef,
     SparkSubmitTypeDef,
     JobRunSummaryTypeDef,
     ResourceUtilizationTypeDef,
     TotalResourceUtilizationTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationsRequestRequestTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
     ListJobRunsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    ManagedPersistenceMonitoringConfigurationOutputTypeDef,
     ManagedPersistenceMonitoringConfigurationTypeDef,
+    S3MonitoringConfigurationOutputTypeDef,
     S3MonitoringConfigurationTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     StartApplicationRequestRequestTypeDef,
-    StartJobRunResponseTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ListApplicationsResponseTypeDef,
     WorkerTypeSpecificationTypeDef,
+    CancelJobRunResponseTypeDef,
+    CreateApplicationResponseTypeDef,
+    GetDashboardForJobRunResponseTypeDef,
+    ListApplicationsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartJobRunResponseTypeDef,
     WorkerTypeSpecificationInputTypeDef,
+    InitialCapacityConfigOutputTypeDef,
     InitialCapacityConfigTypeDef,
+    JobDriverOutputTypeDef,
     JobDriverTypeDef,
     ListJobRunsResponseTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    ListJobRunsRequestListJobRunsPaginateTypeDef,
+    MonitoringConfigurationOutputTypeDef,
     MonitoringConfigurationTypeDef,
     ApplicationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
+    ConfigurationOverridesOutputTypeDef,
     ConfigurationOverridesTypeDef,
     GetApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     JobRunTypeDef,
     StartJobRunRequestRequestTypeDef,
     GetJobRunResponseTypeDef,
 )
```

### Comparing `mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless/__init__.py` & `mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless/__init__.pyi` & `mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless/__main__.py` & `mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EMRServerless 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.EMRServerless 1.28.11\nVersion:         1.28.11\nBuilder"
+        " version: 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.0")
+    print("1.28.11")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless/client.py` & `mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#get_application)
         """
 
     def get_dashboard_for_job_run(
         self, *, applicationId: str, jobRunId: str
     ) -> GetDashboardForJobRunResponseTypeDef:
         """
-        Returns a URL to access the job run dashboard.
+        Creates and returns a URL that you can use to access the application UIs for a
+        job run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.get_dashboard_for_job_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#get_dashboard_for_job_run)
         """
 
     def get_job_run(self, *, applicationId: str, jobRunId: str) -> GetJobRunResponseTypeDef:
         """
```

### Comparing `mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless/client.pyi` & `mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.get_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#get_application)
         """
     def get_dashboard_for_job_run(
         self, *, applicationId: str, jobRunId: str
     ) -> GetDashboardForJobRunResponseTypeDef:
         """
-        Returns a URL to access the job run dashboard.
+        Creates and returns a URL that you can use to access the application UIs for a
+        job run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Client.get_dashboard_for_job_run)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/client/#get_dashboard_for_job_run)
         """
     def get_job_run(self, *, applicationId: str, jobRunId: str) -> GetJobRunResponseTypeDef:
         """
         Displays detailed information about a job run.
```

### Comparing `mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless/literals.py` & `mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,14 +256,15 @@
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless/literals.pyi` & `mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -254,14 +254,15 @@
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless/paginator.py` & `mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listapplicationspaginator)
     """
 
     def paginate(
         self,
         *,
         states: Sequence[ApplicationStateType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listapplicationspaginator)
         """
 
 
@@ -73,13 +73,13 @@
     def paginate(
         self,
         *,
         applicationId: str,
         createdAtAfter: Union[datetime, str] = ...,
         createdAtBefore: Union[datetime, str] = ...,
         states: Sequence[JobRunStateType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Paginator.ListJobRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listjobrunspaginator)
         """
```

### Comparing `mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless/paginator.pyi` & `mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listapplicationspaginator)
     """
 
     def paginate(
         self,
         *,
         states: Sequence[ApplicationStateType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listapplicationspaginator)
         """
 
 class ListJobRunsPaginator(Paginator):
@@ -69,13 +69,13 @@
     def paginate(
         self,
         *,
         applicationId: str,
         createdAtAfter: Union[datetime, str] = ...,
         createdAtBefore: Union[datetime, str] = ...,
         states: Sequence[JobRunStateType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless.Paginator.ListJobRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/paginators/#listjobrunspaginator)
         """
```

### Comparing `mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless/type_defs.py` & `mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/type_defs.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -18,99 +18,141 @@
 from .literals import ApplicationStateType, ArchitectureType, JobRunStateType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ApplicationSummaryTypeDef",
+    "AutoStartConfigOutputTypeDef",
+    "AutoStopConfigOutputTypeDef",
+    "ImageConfigurationTypeDef",
+    "MaximumAllowedResourcesOutputTypeDef",
+    "NetworkConfigurationOutputTypeDef",
     "AutoStartConfigTypeDef",
     "AutoStopConfigTypeDef",
-    "ImageConfigurationTypeDef",
-    "MaximumAllowedResourcesTypeDef",
-    "NetworkConfigurationTypeDef",
     "CancelJobRunRequestRequestTypeDef",
-    "CancelJobRunResponseTypeDef",
+    "ResponseMetadataTypeDef",
+    "CloudWatchLoggingConfigurationOutputTypeDef",
+    "CloudWatchLoggingConfigurationTypeDef",
+    "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
     "ImageConfigurationInputTypeDef",
-    "CreateApplicationResponseTypeDef",
+    "MaximumAllowedResourcesTypeDef",
+    "NetworkConfigurationTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetDashboardForJobRunRequestRequestTypeDef",
-    "GetDashboardForJobRunResponseTypeDef",
     "GetJobRunRequestRequestTypeDef",
+    "HiveOutputTypeDef",
     "HiveTypeDef",
+    "WorkerResourceConfigOutputTypeDef",
     "WorkerResourceConfigTypeDef",
+    "SparkSubmitOutputTypeDef",
     "SparkSubmitTypeDef",
     "JobRunSummaryTypeDef",
     "ResourceUtilizationTypeDef",
     "TotalResourceUtilizationTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationsRequestRequestTypeDef",
-    "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "ListJobRunsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "ManagedPersistenceMonitoringConfigurationOutputTypeDef",
     "ManagedPersistenceMonitoringConfigurationTypeDef",
+    "S3MonitoringConfigurationOutputTypeDef",
     "S3MonitoringConfigurationTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "StartApplicationRequestRequestTypeDef",
-    "StartJobRunResponseTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ListApplicationsResponseTypeDef",
     "WorkerTypeSpecificationTypeDef",
+    "CancelJobRunResponseTypeDef",
+    "CreateApplicationResponseTypeDef",
+    "GetDashboardForJobRunResponseTypeDef",
+    "ListApplicationsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartJobRunResponseTypeDef",
     "WorkerTypeSpecificationInputTypeDef",
+    "InitialCapacityConfigOutputTypeDef",
     "InitialCapacityConfigTypeDef",
+    "JobDriverOutputTypeDef",
     "JobDriverTypeDef",
     "ListJobRunsResponseTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    "ListJobRunsRequestListJobRunsPaginateTypeDef",
+    "MonitoringConfigurationOutputTypeDef",
     "MonitoringConfigurationTypeDef",
     "ApplicationTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
+    "ConfigurationOverridesOutputTypeDef",
     "ConfigurationOverridesTypeDef",
     "GetApplicationResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "JobRunTypeDef",
     "StartJobRunRequestRequestTypeDef",
     "GetJobRunResponseTypeDef",
 )
 
-_RequiredApplicationSummaryTypeDef = TypedDict(
-    "_RequiredApplicationSummaryTypeDef",
+ApplicationSummaryTypeDef = TypedDict(
+    "ApplicationSummaryTypeDef",
     {
         "id": str,
+        "name": str,
         "arn": str,
         "releaseLabel": str,
         "type": str,
         "state": ApplicationStateType,
+        "stateDetails": str,
         "createdAt": datetime,
         "updatedAt": datetime,
+        "architecture": ArchitectureType,
     },
 )
-_OptionalApplicationSummaryTypeDef = TypedDict(
-    "_OptionalApplicationSummaryTypeDef",
+
+AutoStartConfigOutputTypeDef = TypedDict(
+    "AutoStartConfigOutputTypeDef",
     {
-        "name": str,
-        "stateDetails": str,
-        "architecture": ArchitectureType,
+        "enabled": bool,
     },
-    total=False,
 )
 
+AutoStopConfigOutputTypeDef = TypedDict(
+    "AutoStopConfigOutputTypeDef",
+    {
+        "enabled": bool,
+        "idleTimeoutMinutes": int,
+    },
+)
 
-class ApplicationSummaryTypeDef(
-    _RequiredApplicationSummaryTypeDef, _OptionalApplicationSummaryTypeDef
-):
-    pass
+ImageConfigurationTypeDef = TypedDict(
+    "ImageConfigurationTypeDef",
+    {
+        "imageUri": str,
+        "resolvedImageDigest": str,
+    },
+)
 
+MaximumAllowedResourcesOutputTypeDef = TypedDict(
+    "MaximumAllowedResourcesOutputTypeDef",
+    {
+        "cpu": str,
+        "memory": str,
+        "disk": str,
+    },
+)
+
+NetworkConfigurationOutputTypeDef = TypedDict(
+    "NetworkConfigurationOutputTypeDef",
+    {
+        "subnetIds": List[str],
+        "securityGroupIds": List[str],
+    },
+)
 
 AutoStartConfigTypeDef = TypedDict(
     "AutoStartConfigTypeDef",
     {
         "enabled": bool,
     },
     total=False,
@@ -121,119 +163,128 @@
     {
         "enabled": bool,
         "idleTimeoutMinutes": int,
     },
     total=False,
 )
 
-_RequiredImageConfigurationTypeDef = TypedDict(
-    "_RequiredImageConfigurationTypeDef",
+CancelJobRunRequestRequestTypeDef = TypedDict(
+    "CancelJobRunRequestRequestTypeDef",
     {
-        "imageUri": str,
+        "applicationId": str,
+        "jobRunId": str,
     },
 )
-_OptionalImageConfigurationTypeDef = TypedDict(
-    "_OptionalImageConfigurationTypeDef",
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "resolvedImageDigest": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-
-class ImageConfigurationTypeDef(
-    _RequiredImageConfigurationTypeDef, _OptionalImageConfigurationTypeDef
-):
-    pass
-
-
-_RequiredMaximumAllowedResourcesTypeDef = TypedDict(
-    "_RequiredMaximumAllowedResourcesTypeDef",
+CloudWatchLoggingConfigurationOutputTypeDef = TypedDict(
+    "CloudWatchLoggingConfigurationOutputTypeDef",
     {
-        "cpu": str,
-        "memory": str,
+        "enabled": bool,
+        "logGroupName": str,
+        "logStreamNamePrefix": str,
+        "encryptionKeyArn": str,
+        "logTypes": Dict[str, List[str]],
     },
 )
-_OptionalMaximumAllowedResourcesTypeDef = TypedDict(
-    "_OptionalMaximumAllowedResourcesTypeDef",
+
+_RequiredCloudWatchLoggingConfigurationTypeDef = TypedDict(
+    "_RequiredCloudWatchLoggingConfigurationTypeDef",
     {
-        "disk": str,
+        "enabled": bool,
     },
-    total=False,
 )
-
-
-class MaximumAllowedResourcesTypeDef(
-    _RequiredMaximumAllowedResourcesTypeDef, _OptionalMaximumAllowedResourcesTypeDef
-):
-    pass
-
-
-NetworkConfigurationTypeDef = TypedDict(
-    "NetworkConfigurationTypeDef",
+_OptionalCloudWatchLoggingConfigurationTypeDef = TypedDict(
+    "_OptionalCloudWatchLoggingConfigurationTypeDef",
     {
-        "subnetIds": Sequence[str],
-        "securityGroupIds": Sequence[str],
+        "logGroupName": str,
+        "logStreamNamePrefix": str,
+        "encryptionKeyArn": str,
+        "logTypes": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
-CancelJobRunRequestRequestTypeDef = TypedDict(
-    "CancelJobRunRequestRequestTypeDef",
-    {
-        "applicationId": str,
-        "jobRunId": str,
-    },
-)
+class CloudWatchLoggingConfigurationTypeDef(
+    _RequiredCloudWatchLoggingConfigurationTypeDef, _OptionalCloudWatchLoggingConfigurationTypeDef
+):
+    pass
 
-CancelJobRunResponseTypeDef = TypedDict(
-    "CancelJobRunResponseTypeDef",
+ConfigurationOutputTypeDef = TypedDict(
+    "ConfigurationOutputTypeDef",
     {
-        "applicationId": str,
-        "jobRunId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "classification": str,
+        "properties": Dict[str, str],
+        "configurations": List[Dict[str, Any]],
     },
 )
 
 _RequiredConfigurationTypeDef = TypedDict(
     "_RequiredConfigurationTypeDef",
     {
         "classification": str,
     },
 )
 _OptionalConfigurationTypeDef = TypedDict(
     "_OptionalConfigurationTypeDef",
     {
-        "properties": Dict[str, str],
-        "configurations": List[Dict[str, Any]],
+        "properties": Mapping[str, str],
+        "configurations": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
-
 class ConfigurationTypeDef(_RequiredConfigurationTypeDef, _OptionalConfigurationTypeDef):
     pass
 
-
 ImageConfigurationInputTypeDef = TypedDict(
     "ImageConfigurationInputTypeDef",
     {
         "imageUri": str,
     },
     total=False,
 )
 
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
+_RequiredMaximumAllowedResourcesTypeDef = TypedDict(
+    "_RequiredMaximumAllowedResourcesTypeDef",
     {
-        "applicationId": str,
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "cpu": str,
+        "memory": str,
+    },
+)
+_OptionalMaximumAllowedResourcesTypeDef = TypedDict(
+    "_OptionalMaximumAllowedResourcesTypeDef",
+    {
+        "disk": str,
+    },
+    total=False,
+)
+
+class MaximumAllowedResourcesTypeDef(
+    _RequiredMaximumAllowedResourcesTypeDef, _OptionalMaximumAllowedResourcesTypeDef
+):
+    pass
+
+NetworkConfigurationTypeDef = TypedDict(
+    "NetworkConfigurationTypeDef",
+    {
+        "subnetIds": Sequence[str],
+        "securityGroupIds": Sequence[str],
     },
+    total=False,
 )
 
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
@@ -250,30 +301,31 @@
     "GetDashboardForJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
     },
 )
 
-GetDashboardForJobRunResponseTypeDef = TypedDict(
-    "GetDashboardForJobRunResponseTypeDef",
-    {
-        "url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetJobRunRequestRequestTypeDef = TypedDict(
     "GetJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
     },
 )
 
+HiveOutputTypeDef = TypedDict(
+    "HiveOutputTypeDef",
+    {
+        "query": str,
+        "initQueryFile": str,
+        "parameters": str,
+    },
+)
+
 _RequiredHiveTypeDef = TypedDict(
     "_RequiredHiveTypeDef",
     {
         "query": str,
     },
 )
 _OptionalHiveTypeDef = TypedDict(
@@ -281,18 +333,25 @@
     {
         "initQueryFile": str,
         "parameters": str,
     },
     total=False,
 )
 
-
 class HiveTypeDef(_RequiredHiveTypeDef, _OptionalHiveTypeDef):
     pass
 
+WorkerResourceConfigOutputTypeDef = TypedDict(
+    "WorkerResourceConfigOutputTypeDef",
+    {
+        "cpu": str,
+        "memory": str,
+        "disk": str,
+    },
+)
 
 _RequiredWorkerResourceConfigTypeDef = TypedDict(
     "_RequiredWorkerResourceConfigTypeDef",
     {
         "cpu": str,
         "memory": str,
     },
@@ -301,134 +360,102 @@
     "_OptionalWorkerResourceConfigTypeDef",
     {
         "disk": str,
     },
     total=False,
 )
 
-
 class WorkerResourceConfigTypeDef(
     _RequiredWorkerResourceConfigTypeDef, _OptionalWorkerResourceConfigTypeDef
 ):
     pass
 
+SparkSubmitOutputTypeDef = TypedDict(
+    "SparkSubmitOutputTypeDef",
+    {
+        "entryPoint": str,
+        "entryPointArguments": List[str],
+        "sparkSubmitParameters": str,
+    },
+)
 
 _RequiredSparkSubmitTypeDef = TypedDict(
     "_RequiredSparkSubmitTypeDef",
     {
         "entryPoint": str,
     },
 )
 _OptionalSparkSubmitTypeDef = TypedDict(
     "_OptionalSparkSubmitTypeDef",
     {
-        "entryPointArguments": List[str],
+        "entryPointArguments": Sequence[str],
         "sparkSubmitParameters": str,
     },
     total=False,
 )
 
-
 class SparkSubmitTypeDef(_RequiredSparkSubmitTypeDef, _OptionalSparkSubmitTypeDef):
     pass
 
-
-_RequiredJobRunSummaryTypeDef = TypedDict(
-    "_RequiredJobRunSummaryTypeDef",
+JobRunSummaryTypeDef = TypedDict(
+    "JobRunSummaryTypeDef",
     {
         "applicationId": str,
         "id": str,
+        "name": str,
         "arn": str,
         "createdBy": str,
         "createdAt": datetime,
         "updatedAt": datetime,
         "executionRole": str,
         "state": JobRunStateType,
         "stateDetails": str,
         "releaseLabel": str,
-    },
-)
-_OptionalJobRunSummaryTypeDef = TypedDict(
-    "_OptionalJobRunSummaryTypeDef",
-    {
-        "name": str,
         "type": str,
     },
-    total=False,
 )
 
-
-class JobRunSummaryTypeDef(_RequiredJobRunSummaryTypeDef, _OptionalJobRunSummaryTypeDef):
-    pass
-
-
 ResourceUtilizationTypeDef = TypedDict(
     "ResourceUtilizationTypeDef",
     {
         "vCPUHour": float,
         "memoryGBHour": float,
         "storageGBHour": float,
     },
-    total=False,
 )
 
 TotalResourceUtilizationTypeDef = TypedDict(
     "TotalResourceUtilizationTypeDef",
     {
         "vCPUHour": float,
         "memoryGBHour": float,
         "storageGBHour": float,
     },
-    total=False,
 )
 
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "states": Sequence[ApplicationStateType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "states": Sequence[ApplicationStateType],
     },
     total=False,
 )
 
-_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "createdAtAfter": Union[datetime, str],
-        "createdAtBefore": Union[datetime, str],
-        "states": Sequence[JobRunStateType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListJobRunsRequestListJobRunsPaginateTypeDef(
-    _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
-    _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListJobRunsRequestRequestTypeDef = TypedDict(
     "_RequiredListJobRunsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListJobRunsRequestRequestTypeDef = TypedDict(
@@ -439,92 +466,67 @@
         "createdAtAfter": Union[datetime, str],
         "createdAtBefore": Union[datetime, str],
         "states": Sequence[JobRunStateType],
     },
     total=False,
 )
 
-
 class ListJobRunsRequestRequestTypeDef(
     _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
 ):
     pass
 
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+ManagedPersistenceMonitoringConfigurationOutputTypeDef = TypedDict(
+    "ManagedPersistenceMonitoringConfigurationOutputTypeDef",
     {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "enabled": bool,
+        "encryptionKeyArn": str,
     },
 )
 
 ManagedPersistenceMonitoringConfigurationTypeDef = TypedDict(
     "ManagedPersistenceMonitoringConfigurationTypeDef",
     {
         "enabled": bool,
         "encryptionKeyArn": str,
     },
     total=False,
 )
 
-S3MonitoringConfigurationTypeDef = TypedDict(
-    "S3MonitoringConfigurationTypeDef",
+S3MonitoringConfigurationOutputTypeDef = TypedDict(
+    "S3MonitoringConfigurationOutputTypeDef",
     {
         "logUri": str,
         "encryptionKeyArn": str,
     },
-    total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+S3MonitoringConfigurationTypeDef = TypedDict(
+    "S3MonitoringConfigurationTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "logUri": str,
+        "encryptionKeyArn": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 StartApplicationRequestRequestTypeDef = TypedDict(
     "StartApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
-StartJobRunResponseTypeDef = TypedDict(
-    "StartJobRunResponseTypeDef",
-    {
-        "applicationId": str,
-        "jobRunId": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopApplicationRequestRequestTypeDef = TypedDict(
     "StopApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
@@ -540,59 +542,117 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+WorkerTypeSpecificationTypeDef = TypedDict(
+    "WorkerTypeSpecificationTypeDef",
+    {
+        "imageConfiguration": ImageConfigurationTypeDef,
+    },
+)
+
+CancelJobRunResponseTypeDef = TypedDict(
+    "CancelJobRunResponseTypeDef",
+    {
+        "applicationId": str,
+        "jobRunId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
+    {
+        "applicationId": str,
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDashboardForJobRunResponseTypeDef = TypedDict(
+    "GetDashboardForJobRunResponseTypeDef",
+    {
+        "url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "applications": List[ApplicationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-WorkerTypeSpecificationTypeDef = TypedDict(
-    "WorkerTypeSpecificationTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "imageConfiguration": ImageConfigurationTypeDef,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartJobRunResponseTypeDef = TypedDict(
+    "StartJobRunResponseTypeDef",
+    {
+        "applicationId": str,
+        "jobRunId": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 WorkerTypeSpecificationInputTypeDef = TypedDict(
     "WorkerTypeSpecificationInputTypeDef",
     {
         "imageConfiguration": ImageConfigurationInputTypeDef,
     },
     total=False,
 )
 
+InitialCapacityConfigOutputTypeDef = TypedDict(
+    "InitialCapacityConfigOutputTypeDef",
+    {
+        "workerCount": int,
+        "workerConfiguration": WorkerResourceConfigOutputTypeDef,
+    },
+)
+
 _RequiredInitialCapacityConfigTypeDef = TypedDict(
     "_RequiredInitialCapacityConfigTypeDef",
     {
         "workerCount": int,
     },
 )
 _OptionalInitialCapacityConfigTypeDef = TypedDict(
     "_OptionalInitialCapacityConfigTypeDef",
     {
         "workerConfiguration": WorkerResourceConfigTypeDef,
     },
     total=False,
 )
 
-
 class InitialCapacityConfigTypeDef(
     _RequiredInitialCapacityConfigTypeDef, _OptionalInitialCapacityConfigTypeDef
 ):
     pass
 
+JobDriverOutputTypeDef = TypedDict(
+    "JobDriverOutputTypeDef",
+    {
+        "sparkSubmit": SparkSubmitOutputTypeDef,
+        "hive": HiveOutputTypeDef,
+    },
+)
 
 JobDriverTypeDef = TypedDict(
     "JobDriverTypeDef",
     {
         "sparkSubmit": SparkSubmitTypeDef,
         "hive": HiveTypeDef,
     },
@@ -600,64 +660,97 @@
 )
 
 ListJobRunsResponseTypeDef = TypedDict(
     "ListJobRunsResponseTypeDef",
     {
         "jobRuns": List[JobRunSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "states": Sequence[ApplicationStateType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
+    {
+        "createdAtAfter": Union[datetime, str],
+        "createdAtBefore": Union[datetime, str],
+        "states": Sequence[JobRunStateType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListJobRunsRequestListJobRunsPaginateTypeDef(
+    _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
+    _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
+):
+    pass
+
+MonitoringConfigurationOutputTypeDef = TypedDict(
+    "MonitoringConfigurationOutputTypeDef",
+    {
+        "s3MonitoringConfiguration": S3MonitoringConfigurationOutputTypeDef,
+        "managedPersistenceMonitoringConfiguration": (
+            ManagedPersistenceMonitoringConfigurationOutputTypeDef
+        ),
+        "cloudWatchLoggingConfiguration": CloudWatchLoggingConfigurationOutputTypeDef,
     },
 )
 
 MonitoringConfigurationTypeDef = TypedDict(
     "MonitoringConfigurationTypeDef",
     {
         "s3MonitoringConfiguration": S3MonitoringConfigurationTypeDef,
         "managedPersistenceMonitoringConfiguration": (
             ManagedPersistenceMonitoringConfigurationTypeDef
         ),
+        "cloudWatchLoggingConfiguration": CloudWatchLoggingConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredApplicationTypeDef = TypedDict(
-    "_RequiredApplicationTypeDef",
+ApplicationTypeDef = TypedDict(
+    "ApplicationTypeDef",
     {
         "applicationId": str,
+        "name": str,
         "arn": str,
         "releaseLabel": str,
         "type": str,
         "state": ApplicationStateType,
+        "stateDetails": str,
+        "initialCapacity": Dict[str, InitialCapacityConfigOutputTypeDef],
+        "maximumCapacity": MaximumAllowedResourcesOutputTypeDef,
         "createdAt": datetime,
         "updatedAt": datetime,
-    },
-)
-_OptionalApplicationTypeDef = TypedDict(
-    "_OptionalApplicationTypeDef",
-    {
-        "name": str,
-        "stateDetails": str,
-        "initialCapacity": Dict[str, InitialCapacityConfigTypeDef],
-        "maximumCapacity": MaximumAllowedResourcesTypeDef,
         "tags": Dict[str, str],
-        "autoStartConfiguration": AutoStartConfigTypeDef,
-        "autoStopConfiguration": AutoStopConfigTypeDef,
-        "networkConfiguration": NetworkConfigurationTypeDef,
+        "autoStartConfiguration": AutoStartConfigOutputTypeDef,
+        "autoStopConfiguration": AutoStopConfigOutputTypeDef,
+        "networkConfiguration": NetworkConfigurationOutputTypeDef,
         "architecture": ArchitectureType,
         "imageConfiguration": ImageConfigurationTypeDef,
         "workerTypeSpecifications": Dict[str, WorkerTypeSpecificationTypeDef],
     },
-    total=False,
 )
 
-
-class ApplicationTypeDef(_RequiredApplicationTypeDef, _OptionalApplicationTypeDef):
-    pass
-
-
 _RequiredCreateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationRequestRequestTypeDef",
     {
         "releaseLabel": str,
         "type": str,
         "clientToken": str,
     },
@@ -675,21 +768,19 @@
         "architecture": ArchitectureType,
         "imageConfiguration": ImageConfigurationInputTypeDef,
         "workerTypeSpecifications": Mapping[str, WorkerTypeSpecificationInputTypeDef],
     },
     total=False,
 )
 
-
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
         "clientToken": str,
     },
 )
@@ -705,82 +796,77 @@
         "imageConfiguration": ImageConfigurationInputTypeDef,
         "workerTypeSpecifications": Mapping[str, WorkerTypeSpecificationInputTypeDef],
         "releaseLabel": str,
     },
     total=False,
 )
 
-
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
+ConfigurationOverridesOutputTypeDef = TypedDict(
+    "ConfigurationOverridesOutputTypeDef",
+    {
+        "applicationConfiguration": List["ConfigurationOutputTypeDef"],
+        "monitoringConfiguration": MonitoringConfigurationOutputTypeDef,
+    },
+)
 
 ConfigurationOverridesTypeDef = TypedDict(
     "ConfigurationOverridesTypeDef",
     {
-        "applicationConfiguration": List["ConfigurationTypeDef"],
+        "applicationConfiguration": Sequence["ConfigurationTypeDef"],
         "monitoringConfiguration": MonitoringConfigurationTypeDef,
     },
     total=False,
 )
 
 GetApplicationResponseTypeDef = TypedDict(
     "GetApplicationResponseTypeDef",
     {
         "application": ApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationResponseTypeDef = TypedDict(
     "UpdateApplicationResponseTypeDef",
     {
         "application": ApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredJobRunTypeDef = TypedDict(
-    "_RequiredJobRunTypeDef",
+JobRunTypeDef = TypedDict(
+    "JobRunTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
+        "name": str,
         "arn": str,
         "createdBy": str,
         "createdAt": datetime,
         "updatedAt": datetime,
         "executionRole": str,
         "state": JobRunStateType,
         "stateDetails": str,
         "releaseLabel": str,
-        "jobDriver": JobDriverTypeDef,
-    },
-)
-_OptionalJobRunTypeDef = TypedDict(
-    "_OptionalJobRunTypeDef",
-    {
-        "name": str,
-        "configurationOverrides": ConfigurationOverridesTypeDef,
+        "configurationOverrides": ConfigurationOverridesOutputTypeDef,
+        "jobDriver": JobDriverOutputTypeDef,
         "tags": Dict[str, str],
         "totalResourceUtilization": TotalResourceUtilizationTypeDef,
-        "networkConfiguration": NetworkConfigurationTypeDef,
+        "networkConfiguration": NetworkConfigurationOutputTypeDef,
         "totalExecutionDurationSeconds": int,
         "executionTimeoutMinutes": int,
         "billedResourceUtilization": ResourceUtilizationTypeDef,
     },
-    total=False,
 )
 
-
-class JobRunTypeDef(_RequiredJobRunTypeDef, _OptionalJobRunTypeDef):
-    pass
-
-
 _RequiredStartJobRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "clientToken": str,
         "executionRoleArn": str,
     },
@@ -793,21 +879,19 @@
         "tags": Mapping[str, str],
         "executionTimeoutMinutes": int,
         "name": str,
     },
     total=False,
 )
 
-
 class StartJobRunRequestRequestTypeDef(
     _RequiredStartJobRunRequestRequestTypeDef, _OptionalStartJobRunRequestRequestTypeDef
 ):
     pass
 
-
 GetJobRunResponseTypeDef = TypedDict(
     "GetJobRunResponseTypeDef",
     {
         "jobRun": JobRunTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless/type_defs.pyi` & `mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless/type_defs.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,214 +18,281 @@
 from .literals import ApplicationStateType, ArchitectureType, JobRunStateType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ApplicationSummaryTypeDef",
+    "AutoStartConfigOutputTypeDef",
+    "AutoStopConfigOutputTypeDef",
+    "ImageConfigurationTypeDef",
+    "MaximumAllowedResourcesOutputTypeDef",
+    "NetworkConfigurationOutputTypeDef",
     "AutoStartConfigTypeDef",
     "AutoStopConfigTypeDef",
-    "ImageConfigurationTypeDef",
-    "MaximumAllowedResourcesTypeDef",
-    "NetworkConfigurationTypeDef",
     "CancelJobRunRequestRequestTypeDef",
-    "CancelJobRunResponseTypeDef",
+    "ResponseMetadataTypeDef",
+    "CloudWatchLoggingConfigurationOutputTypeDef",
+    "CloudWatchLoggingConfigurationTypeDef",
+    "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
     "ImageConfigurationInputTypeDef",
-    "CreateApplicationResponseTypeDef",
+    "MaximumAllowedResourcesTypeDef",
+    "NetworkConfigurationTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetDashboardForJobRunRequestRequestTypeDef",
-    "GetDashboardForJobRunResponseTypeDef",
     "GetJobRunRequestRequestTypeDef",
+    "HiveOutputTypeDef",
     "HiveTypeDef",
+    "WorkerResourceConfigOutputTypeDef",
     "WorkerResourceConfigTypeDef",
+    "SparkSubmitOutputTypeDef",
     "SparkSubmitTypeDef",
     "JobRunSummaryTypeDef",
     "ResourceUtilizationTypeDef",
     "TotalResourceUtilizationTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationsRequestRequestTypeDef",
-    "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "ListJobRunsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "ManagedPersistenceMonitoringConfigurationOutputTypeDef",
     "ManagedPersistenceMonitoringConfigurationTypeDef",
+    "S3MonitoringConfigurationOutputTypeDef",
     "S3MonitoringConfigurationTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "StartApplicationRequestRequestTypeDef",
-    "StartJobRunResponseTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ListApplicationsResponseTypeDef",
     "WorkerTypeSpecificationTypeDef",
+    "CancelJobRunResponseTypeDef",
+    "CreateApplicationResponseTypeDef",
+    "GetDashboardForJobRunResponseTypeDef",
+    "ListApplicationsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartJobRunResponseTypeDef",
     "WorkerTypeSpecificationInputTypeDef",
+    "InitialCapacityConfigOutputTypeDef",
     "InitialCapacityConfigTypeDef",
+    "JobDriverOutputTypeDef",
     "JobDriverTypeDef",
     "ListJobRunsResponseTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    "ListJobRunsRequestListJobRunsPaginateTypeDef",
+    "MonitoringConfigurationOutputTypeDef",
     "MonitoringConfigurationTypeDef",
     "ApplicationTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
+    "ConfigurationOverridesOutputTypeDef",
     "ConfigurationOverridesTypeDef",
     "GetApplicationResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "JobRunTypeDef",
     "StartJobRunRequestRequestTypeDef",
     "GetJobRunResponseTypeDef",
 )
 
-_RequiredApplicationSummaryTypeDef = TypedDict(
-    "_RequiredApplicationSummaryTypeDef",
+ApplicationSummaryTypeDef = TypedDict(
+    "ApplicationSummaryTypeDef",
     {
         "id": str,
+        "name": str,
         "arn": str,
         "releaseLabel": str,
         "type": str,
         "state": ApplicationStateType,
+        "stateDetails": str,
         "createdAt": datetime,
         "updatedAt": datetime,
-    },
-)
-_OptionalApplicationSummaryTypeDef = TypedDict(
-    "_OptionalApplicationSummaryTypeDef",
-    {
-        "name": str,
-        "stateDetails": str,
         "architecture": ArchitectureType,
     },
-    total=False,
 )
 
-class ApplicationSummaryTypeDef(
-    _RequiredApplicationSummaryTypeDef, _OptionalApplicationSummaryTypeDef
-):
-    pass
-
-AutoStartConfigTypeDef = TypedDict(
-    "AutoStartConfigTypeDef",
+AutoStartConfigOutputTypeDef = TypedDict(
+    "AutoStartConfigOutputTypeDef",
     {
         "enabled": bool,
     },
-    total=False,
 )
 
-AutoStopConfigTypeDef = TypedDict(
-    "AutoStopConfigTypeDef",
+AutoStopConfigOutputTypeDef = TypedDict(
+    "AutoStopConfigOutputTypeDef",
     {
         "enabled": bool,
         "idleTimeoutMinutes": int,
     },
-    total=False,
 )
 
-_RequiredImageConfigurationTypeDef = TypedDict(
-    "_RequiredImageConfigurationTypeDef",
+ImageConfigurationTypeDef = TypedDict(
+    "ImageConfigurationTypeDef",
     {
         "imageUri": str,
-    },
-)
-_OptionalImageConfigurationTypeDef = TypedDict(
-    "_OptionalImageConfigurationTypeDef",
-    {
         "resolvedImageDigest": str,
     },
-    total=False,
 )
 
-class ImageConfigurationTypeDef(
-    _RequiredImageConfigurationTypeDef, _OptionalImageConfigurationTypeDef
-):
-    pass
-
-_RequiredMaximumAllowedResourcesTypeDef = TypedDict(
-    "_RequiredMaximumAllowedResourcesTypeDef",
+MaximumAllowedResourcesOutputTypeDef = TypedDict(
+    "MaximumAllowedResourcesOutputTypeDef",
     {
         "cpu": str,
         "memory": str,
+        "disk": str,
     },
 )
-_OptionalMaximumAllowedResourcesTypeDef = TypedDict(
-    "_OptionalMaximumAllowedResourcesTypeDef",
+
+NetworkConfigurationOutputTypeDef = TypedDict(
+    "NetworkConfigurationOutputTypeDef",
     {
-        "disk": str,
+        "subnetIds": List[str],
+        "securityGroupIds": List[str],
     },
-    total=False,
 )
 
-class MaximumAllowedResourcesTypeDef(
-    _RequiredMaximumAllowedResourcesTypeDef, _OptionalMaximumAllowedResourcesTypeDef
-):
-    pass
+AutoStartConfigTypeDef = TypedDict(
+    "AutoStartConfigTypeDef",
+    {
+        "enabled": bool,
+    },
+    total=False,
+)
 
-NetworkConfigurationTypeDef = TypedDict(
-    "NetworkConfigurationTypeDef",
+AutoStopConfigTypeDef = TypedDict(
+    "AutoStopConfigTypeDef",
     {
-        "subnetIds": Sequence[str],
-        "securityGroupIds": Sequence[str],
+        "enabled": bool,
+        "idleTimeoutMinutes": int,
     },
     total=False,
 )
 
 CancelJobRunRequestRequestTypeDef = TypedDict(
     "CancelJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
     },
 )
 
-CancelJobRunResponseTypeDef = TypedDict(
-    "CancelJobRunResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "applicationId": str,
-        "jobRunId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
+CloudWatchLoggingConfigurationOutputTypeDef = TypedDict(
+    "CloudWatchLoggingConfigurationOutputTypeDef",
+    {
+        "enabled": bool,
+        "logGroupName": str,
+        "logStreamNamePrefix": str,
+        "encryptionKeyArn": str,
+        "logTypes": Dict[str, List[str]],
+    },
+)
+
+_RequiredCloudWatchLoggingConfigurationTypeDef = TypedDict(
+    "_RequiredCloudWatchLoggingConfigurationTypeDef",
+    {
+        "enabled": bool,
+    },
+)
+_OptionalCloudWatchLoggingConfigurationTypeDef = TypedDict(
+    "_OptionalCloudWatchLoggingConfigurationTypeDef",
+    {
+        "logGroupName": str,
+        "logStreamNamePrefix": str,
+        "encryptionKeyArn": str,
+        "logTypes": Mapping[str, Sequence[str]],
+    },
+    total=False,
+)
+
+
+class CloudWatchLoggingConfigurationTypeDef(
+    _RequiredCloudWatchLoggingConfigurationTypeDef, _OptionalCloudWatchLoggingConfigurationTypeDef
+):
+    pass
+
+
+ConfigurationOutputTypeDef = TypedDict(
+    "ConfigurationOutputTypeDef",
+    {
+        "classification": str,
+        "properties": Dict[str, str],
+        "configurations": List[Dict[str, Any]],
     },
 )
 
 _RequiredConfigurationTypeDef = TypedDict(
     "_RequiredConfigurationTypeDef",
     {
         "classification": str,
     },
 )
 _OptionalConfigurationTypeDef = TypedDict(
     "_OptionalConfigurationTypeDef",
     {
-        "properties": Dict[str, str],
-        "configurations": List[Dict[str, Any]],
+        "properties": Mapping[str, str],
+        "configurations": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
+
 class ConfigurationTypeDef(_RequiredConfigurationTypeDef, _OptionalConfigurationTypeDef):
     pass
 
+
 ImageConfigurationInputTypeDef = TypedDict(
     "ImageConfigurationInputTypeDef",
     {
         "imageUri": str,
     },
     total=False,
 )
 
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
+_RequiredMaximumAllowedResourcesTypeDef = TypedDict(
+    "_RequiredMaximumAllowedResourcesTypeDef",
     {
-        "applicationId": str,
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "cpu": str,
+        "memory": str,
     },
 )
+_OptionalMaximumAllowedResourcesTypeDef = TypedDict(
+    "_OptionalMaximumAllowedResourcesTypeDef",
+    {
+        "disk": str,
+    },
+    total=False,
+)
+
+
+class MaximumAllowedResourcesTypeDef(
+    _RequiredMaximumAllowedResourcesTypeDef, _OptionalMaximumAllowedResourcesTypeDef
+):
+    pass
+
+
+NetworkConfigurationTypeDef = TypedDict(
+    "NetworkConfigurationTypeDef",
+    {
+        "subnetIds": Sequence[str],
+        "securityGroupIds": Sequence[str],
+    },
+    total=False,
+)
 
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
@@ -241,30 +308,31 @@
     "GetDashboardForJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
     },
 )
 
-GetDashboardForJobRunResponseTypeDef = TypedDict(
-    "GetDashboardForJobRunResponseTypeDef",
-    {
-        "url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetJobRunRequestRequestTypeDef = TypedDict(
     "GetJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
     },
 )
 
+HiveOutputTypeDef = TypedDict(
+    "HiveOutputTypeDef",
+    {
+        "query": str,
+        "initQueryFile": str,
+        "parameters": str,
+    },
+)
+
 _RequiredHiveTypeDef = TypedDict(
     "_RequiredHiveTypeDef",
     {
         "query": str,
     },
 )
 _OptionalHiveTypeDef = TypedDict(
@@ -272,17 +340,28 @@
     {
         "initQueryFile": str,
         "parameters": str,
     },
     total=False,
 )
 
+
 class HiveTypeDef(_RequiredHiveTypeDef, _OptionalHiveTypeDef):
     pass
 
+
+WorkerResourceConfigOutputTypeDef = TypedDict(
+    "WorkerResourceConfigOutputTypeDef",
+    {
+        "cpu": str,
+        "memory": str,
+        "disk": str,
+    },
+)
+
 _RequiredWorkerResourceConfigTypeDef = TypedDict(
     "_RequiredWorkerResourceConfigTypeDef",
     {
         "cpu": str,
         "memory": str,
     },
 )
@@ -290,126 +369,106 @@
     "_OptionalWorkerResourceConfigTypeDef",
     {
         "disk": str,
     },
     total=False,
 )
 
+
 class WorkerResourceConfigTypeDef(
     _RequiredWorkerResourceConfigTypeDef, _OptionalWorkerResourceConfigTypeDef
 ):
     pass
 
+
+SparkSubmitOutputTypeDef = TypedDict(
+    "SparkSubmitOutputTypeDef",
+    {
+        "entryPoint": str,
+        "entryPointArguments": List[str],
+        "sparkSubmitParameters": str,
+    },
+)
+
 _RequiredSparkSubmitTypeDef = TypedDict(
     "_RequiredSparkSubmitTypeDef",
     {
         "entryPoint": str,
     },
 )
 _OptionalSparkSubmitTypeDef = TypedDict(
     "_OptionalSparkSubmitTypeDef",
     {
-        "entryPointArguments": List[str],
+        "entryPointArguments": Sequence[str],
         "sparkSubmitParameters": str,
     },
     total=False,
 )
 
+
 class SparkSubmitTypeDef(_RequiredSparkSubmitTypeDef, _OptionalSparkSubmitTypeDef):
     pass
 
-_RequiredJobRunSummaryTypeDef = TypedDict(
-    "_RequiredJobRunSummaryTypeDef",
+
+JobRunSummaryTypeDef = TypedDict(
+    "JobRunSummaryTypeDef",
     {
         "applicationId": str,
         "id": str,
+        "name": str,
         "arn": str,
         "createdBy": str,
         "createdAt": datetime,
         "updatedAt": datetime,
         "executionRole": str,
         "state": JobRunStateType,
         "stateDetails": str,
         "releaseLabel": str,
-    },
-)
-_OptionalJobRunSummaryTypeDef = TypedDict(
-    "_OptionalJobRunSummaryTypeDef",
-    {
-        "name": str,
         "type": str,
     },
-    total=False,
 )
 
-class JobRunSummaryTypeDef(_RequiredJobRunSummaryTypeDef, _OptionalJobRunSummaryTypeDef):
-    pass
-
 ResourceUtilizationTypeDef = TypedDict(
     "ResourceUtilizationTypeDef",
     {
         "vCPUHour": float,
         "memoryGBHour": float,
         "storageGBHour": float,
     },
-    total=False,
 )
 
 TotalResourceUtilizationTypeDef = TypedDict(
     "TotalResourceUtilizationTypeDef",
     {
         "vCPUHour": float,
         "memoryGBHour": float,
         "storageGBHour": float,
     },
-    total=False,
 )
 
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "states": Sequence[ApplicationStateType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "states": Sequence[ApplicationStateType],
     },
     total=False,
 )
 
-_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "createdAtAfter": Union[datetime, str],
-        "createdAtBefore": Union[datetime, str],
-        "states": Sequence[JobRunStateType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListJobRunsRequestListJobRunsPaginateTypeDef(
-    _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
-    _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
-):
-    pass
-
 _RequiredListJobRunsRequestRequestTypeDef = TypedDict(
     "_RequiredListJobRunsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListJobRunsRequestRequestTypeDef = TypedDict(
@@ -420,90 +479,69 @@
         "createdAtAfter": Union[datetime, str],
         "createdAtBefore": Union[datetime, str],
         "states": Sequence[JobRunStateType],
     },
     total=False,
 )
 
+
 class ListJobRunsRequestRequestTypeDef(
     _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
 ):
     pass
 
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+ManagedPersistenceMonitoringConfigurationOutputTypeDef = TypedDict(
+    "ManagedPersistenceMonitoringConfigurationOutputTypeDef",
     {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "enabled": bool,
+        "encryptionKeyArn": str,
     },
 )
 
 ManagedPersistenceMonitoringConfigurationTypeDef = TypedDict(
     "ManagedPersistenceMonitoringConfigurationTypeDef",
     {
         "enabled": bool,
         "encryptionKeyArn": str,
     },
     total=False,
 )
 
-S3MonitoringConfigurationTypeDef = TypedDict(
-    "S3MonitoringConfigurationTypeDef",
+S3MonitoringConfigurationOutputTypeDef = TypedDict(
+    "S3MonitoringConfigurationOutputTypeDef",
     {
         "logUri": str,
         "encryptionKeyArn": str,
     },
-    total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+S3MonitoringConfigurationTypeDef = TypedDict(
+    "S3MonitoringConfigurationTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "logUri": str,
+        "encryptionKeyArn": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 StartApplicationRequestRequestTypeDef = TypedDict(
     "StartApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
-StartJobRunResponseTypeDef = TypedDict(
-    "StartJobRunResponseTypeDef",
-    {
-        "applicationId": str,
-        "jobRunId": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopApplicationRequestRequestTypeDef = TypedDict(
     "StopApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
@@ -519,120 +557,219 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+WorkerTypeSpecificationTypeDef = TypedDict(
+    "WorkerTypeSpecificationTypeDef",
+    {
+        "imageConfiguration": ImageConfigurationTypeDef,
+    },
+)
+
+CancelJobRunResponseTypeDef = TypedDict(
+    "CancelJobRunResponseTypeDef",
+    {
+        "applicationId": str,
+        "jobRunId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
+    {
+        "applicationId": str,
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDashboardForJobRunResponseTypeDef = TypedDict(
+    "GetDashboardForJobRunResponseTypeDef",
+    {
+        "url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "applications": List[ApplicationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-WorkerTypeSpecificationTypeDef = TypedDict(
-    "WorkerTypeSpecificationTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "imageConfiguration": ImageConfigurationTypeDef,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartJobRunResponseTypeDef = TypedDict(
+    "StartJobRunResponseTypeDef",
+    {
+        "applicationId": str,
+        "jobRunId": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 WorkerTypeSpecificationInputTypeDef = TypedDict(
     "WorkerTypeSpecificationInputTypeDef",
     {
         "imageConfiguration": ImageConfigurationInputTypeDef,
     },
     total=False,
 )
 
+InitialCapacityConfigOutputTypeDef = TypedDict(
+    "InitialCapacityConfigOutputTypeDef",
+    {
+        "workerCount": int,
+        "workerConfiguration": WorkerResourceConfigOutputTypeDef,
+    },
+)
+
 _RequiredInitialCapacityConfigTypeDef = TypedDict(
     "_RequiredInitialCapacityConfigTypeDef",
     {
         "workerCount": int,
     },
 )
 _OptionalInitialCapacityConfigTypeDef = TypedDict(
     "_OptionalInitialCapacityConfigTypeDef",
     {
         "workerConfiguration": WorkerResourceConfigTypeDef,
     },
     total=False,
 )
 
+
 class InitialCapacityConfigTypeDef(
     _RequiredInitialCapacityConfigTypeDef, _OptionalInitialCapacityConfigTypeDef
 ):
     pass
 
+
+JobDriverOutputTypeDef = TypedDict(
+    "JobDriverOutputTypeDef",
+    {
+        "sparkSubmit": SparkSubmitOutputTypeDef,
+        "hive": HiveOutputTypeDef,
+    },
+)
+
 JobDriverTypeDef = TypedDict(
     "JobDriverTypeDef",
     {
         "sparkSubmit": SparkSubmitTypeDef,
         "hive": HiveTypeDef,
     },
     total=False,
 )
 
 ListJobRunsResponseTypeDef = TypedDict(
     "ListJobRunsResponseTypeDef",
     {
         "jobRuns": List[JobRunSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "states": Sequence[ApplicationStateType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
+    {
+        "createdAtAfter": Union[datetime, str],
+        "createdAtBefore": Union[datetime, str],
+        "states": Sequence[JobRunStateType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListJobRunsRequestListJobRunsPaginateTypeDef(
+    _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
+    _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
+):
+    pass
+
+
+MonitoringConfigurationOutputTypeDef = TypedDict(
+    "MonitoringConfigurationOutputTypeDef",
+    {
+        "s3MonitoringConfiguration": S3MonitoringConfigurationOutputTypeDef,
+        "managedPersistenceMonitoringConfiguration": (
+            ManagedPersistenceMonitoringConfigurationOutputTypeDef
+        ),
+        "cloudWatchLoggingConfiguration": CloudWatchLoggingConfigurationOutputTypeDef,
     },
 )
 
 MonitoringConfigurationTypeDef = TypedDict(
     "MonitoringConfigurationTypeDef",
     {
         "s3MonitoringConfiguration": S3MonitoringConfigurationTypeDef,
         "managedPersistenceMonitoringConfiguration": (
             ManagedPersistenceMonitoringConfigurationTypeDef
         ),
+        "cloudWatchLoggingConfiguration": CloudWatchLoggingConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredApplicationTypeDef = TypedDict(
-    "_RequiredApplicationTypeDef",
+ApplicationTypeDef = TypedDict(
+    "ApplicationTypeDef",
     {
         "applicationId": str,
+        "name": str,
         "arn": str,
         "releaseLabel": str,
         "type": str,
         "state": ApplicationStateType,
+        "stateDetails": str,
+        "initialCapacity": Dict[str, InitialCapacityConfigOutputTypeDef],
+        "maximumCapacity": MaximumAllowedResourcesOutputTypeDef,
         "createdAt": datetime,
         "updatedAt": datetime,
-    },
-)
-_OptionalApplicationTypeDef = TypedDict(
-    "_OptionalApplicationTypeDef",
-    {
-        "name": str,
-        "stateDetails": str,
-        "initialCapacity": Dict[str, InitialCapacityConfigTypeDef],
-        "maximumCapacity": MaximumAllowedResourcesTypeDef,
         "tags": Dict[str, str],
-        "autoStartConfiguration": AutoStartConfigTypeDef,
-        "autoStopConfiguration": AutoStopConfigTypeDef,
-        "networkConfiguration": NetworkConfigurationTypeDef,
+        "autoStartConfiguration": AutoStartConfigOutputTypeDef,
+        "autoStopConfiguration": AutoStopConfigOutputTypeDef,
+        "networkConfiguration": NetworkConfigurationOutputTypeDef,
         "architecture": ArchitectureType,
         "imageConfiguration": ImageConfigurationTypeDef,
         "workerTypeSpecifications": Dict[str, WorkerTypeSpecificationTypeDef],
     },
-    total=False,
 )
 
-class ApplicationTypeDef(_RequiredApplicationTypeDef, _OptionalApplicationTypeDef):
-    pass
-
 _RequiredCreateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationRequestRequestTypeDef",
     {
         "releaseLabel": str,
         "type": str,
         "clientToken": str,
     },
@@ -650,19 +787,21 @@
         "architecture": ArchitectureType,
         "imageConfiguration": ImageConfigurationInputTypeDef,
         "workerTypeSpecifications": Mapping[str, WorkerTypeSpecificationInputTypeDef],
     },
     total=False,
 )
 
+
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
         "clientToken": str,
     },
 )
@@ -678,78 +817,79 @@
         "imageConfiguration": ImageConfigurationInputTypeDef,
         "workerTypeSpecifications": Mapping[str, WorkerTypeSpecificationInputTypeDef],
         "releaseLabel": str,
     },
     total=False,
 )
 
+
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
+
+ConfigurationOverridesOutputTypeDef = TypedDict(
+    "ConfigurationOverridesOutputTypeDef",
+    {
+        "applicationConfiguration": List["ConfigurationOutputTypeDef"],
+        "monitoringConfiguration": MonitoringConfigurationOutputTypeDef,
+    },
+)
+
 ConfigurationOverridesTypeDef = TypedDict(
     "ConfigurationOverridesTypeDef",
     {
-        "applicationConfiguration": List["ConfigurationTypeDef"],
+        "applicationConfiguration": Sequence["ConfigurationTypeDef"],
         "monitoringConfiguration": MonitoringConfigurationTypeDef,
     },
     total=False,
 )
 
 GetApplicationResponseTypeDef = TypedDict(
     "GetApplicationResponseTypeDef",
     {
         "application": ApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationResponseTypeDef = TypedDict(
     "UpdateApplicationResponseTypeDef",
     {
         "application": ApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredJobRunTypeDef = TypedDict(
-    "_RequiredJobRunTypeDef",
+JobRunTypeDef = TypedDict(
+    "JobRunTypeDef",
     {
         "applicationId": str,
         "jobRunId": str,
+        "name": str,
         "arn": str,
         "createdBy": str,
         "createdAt": datetime,
         "updatedAt": datetime,
         "executionRole": str,
         "state": JobRunStateType,
         "stateDetails": str,
         "releaseLabel": str,
-        "jobDriver": JobDriverTypeDef,
-    },
-)
-_OptionalJobRunTypeDef = TypedDict(
-    "_OptionalJobRunTypeDef",
-    {
-        "name": str,
-        "configurationOverrides": ConfigurationOverridesTypeDef,
+        "configurationOverrides": ConfigurationOverridesOutputTypeDef,
+        "jobDriver": JobDriverOutputTypeDef,
         "tags": Dict[str, str],
         "totalResourceUtilization": TotalResourceUtilizationTypeDef,
-        "networkConfiguration": NetworkConfigurationTypeDef,
+        "networkConfiguration": NetworkConfigurationOutputTypeDef,
         "totalExecutionDurationSeconds": int,
         "executionTimeoutMinutes": int,
         "billedResourceUtilization": ResourceUtilizationTypeDef,
     },
-    total=False,
 )
 
-class JobRunTypeDef(_RequiredJobRunTypeDef, _OptionalJobRunTypeDef):
-    pass
-
 _RequiredStartJobRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartJobRunRequestRequestTypeDef",
     {
         "applicationId": str,
         "clientToken": str,
         "executionRoleArn": str,
     },
@@ -762,19 +902,21 @@
         "tags": Mapping[str, str],
         "executionTimeoutMinutes": int,
         "name": str,
     },
     total=False,
 )
 
+
 class StartJobRunRequestRequestTypeDef(
     _RequiredStartJobRunRequestRequestTypeDef, _OptionalStartJobRunRequestRequestTypeDef
 ):
     pass
 
+
 GetJobRunResponseTypeDef = TypedDict(
     "GetJobRunResponseTypeDef",
     {
         "jobRun": JobRunTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless.egg-info/PKG-INFO` & `mypy-boto3-emr-serverless-1.28.11/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-emr-serverless
-Version: 1.28.0
-Summary: Type annotations for boto3.EMRServerless 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 emr-serverless type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-emr-serverless"></a>
 
 # mypy-boto3-emr-serverless
 
 [![PyPI - mypy-boto3-emr-serverless](https://img.shields.io/pypi/v/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-serverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr-serverless?color=blue)](https://pypistats.org/packages/mypy-boto3-emr-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRServerless 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
+[boto3.EMRServerless 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#EMRServerless)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-emr-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_serverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -326,60 +294,76 @@
 
 `mypy_boto3_emr_serverless.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_emr_serverless.type_defs import (
     ApplicationSummaryTypeDef,
+    AutoStartConfigOutputTypeDef,
+    AutoStopConfigOutputTypeDef,
+    ImageConfigurationTypeDef,
+    MaximumAllowedResourcesOutputTypeDef,
+    NetworkConfigurationOutputTypeDef,
     AutoStartConfigTypeDef,
     AutoStopConfigTypeDef,
-    ImageConfigurationTypeDef,
-    MaximumAllowedResourcesTypeDef,
-    NetworkConfigurationTypeDef,
     CancelJobRunRequestRequestTypeDef,
-    CancelJobRunResponseTypeDef,
+    ResponseMetadataTypeDef,
+    CloudWatchLoggingConfigurationOutputTypeDef,
+    CloudWatchLoggingConfigurationTypeDef,
+    ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     ImageConfigurationInputTypeDef,
-    CreateApplicationResponseTypeDef,
+    MaximumAllowedResourcesTypeDef,
+    NetworkConfigurationTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetDashboardForJobRunRequestRequestTypeDef,
-    GetDashboardForJobRunResponseTypeDef,
     GetJobRunRequestRequestTypeDef,
+    HiveOutputTypeDef,
     HiveTypeDef,
+    WorkerResourceConfigOutputTypeDef,
     WorkerResourceConfigTypeDef,
+    SparkSubmitOutputTypeDef,
     SparkSubmitTypeDef,
     JobRunSummaryTypeDef,
     ResourceUtilizationTypeDef,
     TotalResourceUtilizationTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationsRequestRequestTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
     ListJobRunsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    ManagedPersistenceMonitoringConfigurationOutputTypeDef,
     ManagedPersistenceMonitoringConfigurationTypeDef,
+    S3MonitoringConfigurationOutputTypeDef,
     S3MonitoringConfigurationTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     StartApplicationRequestRequestTypeDef,
-    StartJobRunResponseTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ListApplicationsResponseTypeDef,
     WorkerTypeSpecificationTypeDef,
+    CancelJobRunResponseTypeDef,
+    CreateApplicationResponseTypeDef,
+    GetDashboardForJobRunResponseTypeDef,
+    ListApplicationsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartJobRunResponseTypeDef,
     WorkerTypeSpecificationInputTypeDef,
+    InitialCapacityConfigOutputTypeDef,
     InitialCapacityConfigTypeDef,
+    JobDriverOutputTypeDef,
     JobDriverTypeDef,
     ListJobRunsResponseTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    ListJobRunsRequestListJobRunsPaginateTypeDef,
+    MonitoringConfigurationOutputTypeDef,
     MonitoringConfigurationTypeDef,
     ApplicationTypeDef,
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
+    ConfigurationOverridesOutputTypeDef,
     ConfigurationOverridesTypeDef,
     GetApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     JobRunTypeDef,
     StartJobRunRequestRequestTypeDef,
     GetJobRunResponseTypeDef,
 )
```

### Comparing `mypy-boto3-emr-serverless-1.28.0/mypy_boto3_emr_serverless.egg-info/SOURCES.txt` & `mypy-boto3-emr-serverless-1.28.11/mypy_boto3_emr_serverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-serverless-1.28.0/setup.py` & `mypy-boto3-emr-serverless-1.28.11/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-emr-serverless",
-    version="1.28.0",
+    version="1.28.11",
     packages=["mypy_boto3_emr_serverless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EMRServerless 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.EMRServerless 1.28.11 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

