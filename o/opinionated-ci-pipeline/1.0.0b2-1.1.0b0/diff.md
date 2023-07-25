# Comparing `tmp/opinionated-ci-pipeline-1.0.0b2.tar.gz` & `tmp/opinionated-ci-pipeline-1.1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opinionated-ci-pipeline-1.0.0b2.tar", last modified: Thu Mar  9 10:12:39 2023, max compression
+gzip compressed data, was "opinionated-ci-pipeline-1.1.0b0.tar", last modified: Tue Apr  4 10:59:29 2023, max compression
```

## Comparing `opinionated-ci-pipeline-1.0.0b2.tar` & `opinionated-ci-pipeline-1.1.0b0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 10:12:39.396549 opinionated-ci-pipeline-1.0.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-03-09 10:12:23.000000 opinionated-ci-pipeline-1.0.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-09 10:12:23.000000 opinionated-ci-pipeline-1.0.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-03-09 10:12:39.396549 opinionated-ci-pipeline-1.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-03-09 10:12:23.000000 opinionated-ci-pipeline-1.0.0b2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-09 10:12:23.000000 opinionated-ci-pipeline-1.0.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 10:12:39.396549 opinionated-ci-pipeline-1.0.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-03-09 10:12:23.000000 opinionated-ci-pipeline-1.0.0b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 10:12:39.396549 opinionated-ci-pipeline-1.0.0b2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 10:12:39.396549 opinionated-ci-pipeline-1.0.0b2/src/opinionated_ci_pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)    89626 2023-03-09 10:12:23.000000 opinionated-ci-pipeline-1.0.0b2/src/opinionated_ci_pipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 10:12:39.396549 opinionated-ci-pipeline-1.0.0b2/src/opinionated_ci_pipeline/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-03-09 10:12:23.000000 opinionated-ci-pipeline-1.0.0b2/src/opinionated_ci_pipeline/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   377041 2023-03-09 10:12:23.000000 opinionated-ci-pipeline-1.0.0b2/src/opinionated_ci_pipeline/_jsii/opinionated-ci-pipeline@1.0.0-beta.2.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 10:12:23.000000 opinionated-ci-pipeline-1.0.0b2/src/opinionated_ci_pipeline/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 10:12:39.396549 opinionated-ci-pipeline-1.0.0b2/src/opinionated_ci_pipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-03-09 10:12:39.000000 opinionated-ci-pipeline-1.0.0b2/src/opinionated_ci_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-03-09 10:12:39.000000 opinionated-ci-pipeline-1.0.0b2/src/opinionated_ci_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 10:12:39.000000 opinionated-ci-pipeline-1.0.0b2/src/opinionated_ci_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-09 10:12:39.000000 opinionated-ci-pipeline-1.0.0b2/src/opinionated_ci_pipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-09 10:12:39.000000 opinionated-ci-pipeline-1.0.0b2/src/opinionated_ci_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:59:29.911831 opinionated-ci-pipeline-1.1.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-04 10:59:14.000000 opinionated-ci-pipeline-1.1.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-04 10:59:14.000000 opinionated-ci-pipeline-1.1.0b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11098 2023-04-04 10:59:29.911831 opinionated-ci-pipeline-1.1.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-04-04 10:59:14.000000 opinionated-ci-pipeline-1.1.0b0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-04 10:59:14.000000 opinionated-ci-pipeline-1.1.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 10:59:29.911831 opinionated-ci-pipeline-1.1.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-04 10:59:14.000000 opinionated-ci-pipeline-1.1.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:59:29.907831 opinionated-ci-pipeline-1.1.0b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:59:29.907831 opinionated-ci-pipeline-1.1.0b0/src/opinionated_ci_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)    86493 2023-04-04 10:59:14.000000 opinionated-ci-pipeline-1.1.0b0/src/opinionated_ci_pipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:59:29.911831 opinionated-ci-pipeline-1.1.0b0/src/opinionated_ci_pipeline/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-04 10:59:14.000000 opinionated-ci-pipeline-1.1.0b0/src/opinionated_ci_pipeline/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   378330 2023-04-04 10:59:14.000000 opinionated-ci-pipeline-1.1.0b0/src/opinionated_ci_pipeline/_jsii/opinionated-ci-pipeline@1.1.0-beta.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 10:59:14.000000 opinionated-ci-pipeline-1.1.0b0/src/opinionated_ci_pipeline/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 10:59:29.911831 opinionated-ci-pipeline-1.1.0b0/src/opinionated_ci_pipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11098 2023-04-04 10:59:29.000000 opinionated-ci-pipeline-1.1.0b0/src/opinionated_ci_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-04 10:59:29.000000 opinionated-ci-pipeline-1.1.0b0/src/opinionated_ci_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 10:59:29.000000 opinionated-ci-pipeline-1.1.0b0/src/opinionated_ci_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-04 10:59:29.000000 opinionated-ci-pipeline-1.1.0b0/src/opinionated_ci_pipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-04 10:59:29.000000 opinionated-ci-pipeline-1.1.0b0/src/opinionated_ci_pipeline.egg-info/top_level.txt
```

### Comparing `opinionated-ci-pipeline-1.0.0b2/LICENSE` & `opinionated-ci-pipeline-1.1.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opinionated-ci-pipeline-1.0.0b2/PKG-INFO` & `opinionated-ci-pipeline-1.1.0b0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,16 @@
-Metadata-Version: 2.1
-Name: opinionated-ci-pipeline
-Version: 1.0.0b2
-Summary: CI/CD on AWS with feature-branch builds, developer-environment deployments, and build status notifications.
-Home-page: https://github.com/merapar/opinionated-ci-pipeline.git
-Author: Maciej Radzikowski<maciej.radzikowski@merapar.com>
-License: MIT
-Project-URL: Source, https://github.com/merapar/opinionated-ci-pipeline.git
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: JavaScript
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Typing :: Typed
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved
-Requires-Python: ~=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Opinionated CDK CI Pipeline
 
 [![NPM](https://img.shields.io/npm/v/opinionated-ci-pipeline?color=blue)](https://www.npmjs.com/package/opinionated-ci-pipeline)
 [![PyPI](https://img.shields.io/pypi/v/opinionated-ci-pipeline?color=blue)](https://pypi.org/project/opinionated-ci-pipeline/)
 
 CI/CD utilizing [CDK Pipelines](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.pipelines-readme.html).
 
+See the [announcement blog post](https://merapar.com/finally-the-cdk-ci-pipeline-that-serverless-deserves/) for examples and architecture diagrams.
+
 Features:
 
 * pipeline deploying application from the default branch
   to multiple environments on multiple accounts,
 * feature branch deployments to ephemeral environments,
 * development environments deployments from the local CLI,
 * build status notifications to repository commits,
@@ -52,14 +31,18 @@
     * [GitHub](#github)
     * [Bitbucket](#bitbucket)
   * [5. Bootstrap the CDK](#5-bootstrap-the-cdk)
   * [6. Deploy the CI Stack](#6-deploy-the-ci-stack)
   * [Deploy development environment](#deploy-development-environment)
 * [Parameters](#parameters)
 * [Notifications and alarms](#notifications-and-alarms)
+* [How to](#how-to)
+
+  * [Run unit tests during build](#run-unit-tests-during-build)
+  * [Enable Docker](#enable-docker)
 * [Library development](#library-development)
 
 ## Usage
 
 To set up, you need to complete the following steps:
 
 1. Install the library in your project.
@@ -238,23 +221,37 @@
     </tr>
     <tr>
         <td>packageManager</td>
         <td>npm | pnpm</td>
         <td>
 Package manager used in the repository.
 <br/>
-If provided, the install commands will be set to install dependencies using given package manager.
-        </td>
+
+If provided, the `install` command will be set to install dependencies using given package manager.
+
+</td>
     </tr>
     <tr>
         <td>commands</td>
         <td>object</td>
         <td>
+
 Commands executed to build and deploy the application.
 <br/>
+The following commands are set by default:
+
+* `install`
+* `synthPipeline`
+* `deployEnvironment`
+* `destroyEnvironment`
+
+If you override the `install` command,
+either install the `aws-cdk@2` globally
+or modify the other 3 commands to use the local `cdk` binary.
+<br/>
 Commands executed on particular builds:
 
 * main pipeline:
 
   * `preInstall`
   * `install`
   * `buildAndTest`
@@ -341,14 +338,45 @@
 an additional SNS Topic will be created
 to which you can send CloudWatch Alarms.
 It's ARN is provided:
 
 * SSM: `/{projectName}/ci/slackAlarmsTopicArn`
 * Stack exported output: `{projectName}-ci-slackAlarmsTopicArn`
 
+## How to
+
+### Run unit tests during build
+
+Set commands in the `commands.buildAndTest`:
+
+```python
+{
+    commands: {
+        buildAndTest: [
+            'npm run lint',
+            'npm run test',
+        ]
+    }
+}
+```
+
+### Enable Docker
+
+Set `codeBuild.buildEnvironment.privileged` to `true`:
+
+```python
+{
+    codeBuild: {
+        buildEnvironment: {
+            privileged: true
+        }
+    }
+}
+```
+
 ## Library development
 
 Project uses [jsii](https://aws.github.io/jsii/)
 to generate packages for different languages.
 
 Install dependencies:
```

### Comparing `opinionated-ci-pipeline-1.0.0b2/README.md` & `opinionated-ci-pipeline-1.1.0b0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,39 @@
+Metadata-Version: 2.1
+Name: opinionated-ci-pipeline
+Version: 1.1.0b0
+Summary: CI/CD on AWS with feature-branch builds, developer-environment deployments, and build status notifications.
+Home-page: https://github.com/merapar/opinionated-ci-pipeline.git
+Author: Maciej Radzikowski<maciej.radzikowski@merapar.com>
+License: MIT
+Project-URL: Source, https://github.com/merapar/opinionated-ci-pipeline.git
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: JavaScript
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Typing :: Typed
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved
+Requires-Python: ~=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Opinionated CDK CI Pipeline
 
 [![NPM](https://img.shields.io/npm/v/opinionated-ci-pipeline?color=blue)](https://www.npmjs.com/package/opinionated-ci-pipeline)
 [![PyPI](https://img.shields.io/pypi/v/opinionated-ci-pipeline?color=blue)](https://pypi.org/project/opinionated-ci-pipeline/)
 
 CI/CD utilizing [CDK Pipelines](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.pipelines-readme.html).
 
+See the [announcement blog post](https://merapar.com/finally-the-cdk-ci-pipeline-that-serverless-deserves/) for examples and architecture diagrams.
+
 Features:
 
 * pipeline deploying application from the default branch
   to multiple environments on multiple accounts,
 * feature branch deployments to ephemeral environments,
 * development environments deployments from the local CLI,
 * build status notifications to repository commits,
@@ -29,14 +54,18 @@
     * [GitHub](#github)
     * [Bitbucket](#bitbucket)
   * [5. Bootstrap the CDK](#5-bootstrap-the-cdk)
   * [6. Deploy the CI Stack](#6-deploy-the-ci-stack)
   * [Deploy development environment](#deploy-development-environment)
 * [Parameters](#parameters)
 * [Notifications and alarms](#notifications-and-alarms)
+* [How to](#how-to)
+
+  * [Run unit tests during build](#run-unit-tests-during-build)
+  * [Enable Docker](#enable-docker)
 * [Library development](#library-development)
 
 ## Usage
 
 To set up, you need to complete the following steps:
 
 1. Install the library in your project.
@@ -215,23 +244,37 @@
     </tr>
     <tr>
         <td>packageManager</td>
         <td>npm | pnpm</td>
         <td>
 Package manager used in the repository.
 <br/>
-If provided, the install commands will be set to install dependencies using given package manager.
-        </td>
+
+If provided, the `install` command will be set to install dependencies using given package manager.
+
+</td>
     </tr>
     <tr>
         <td>commands</td>
         <td>object</td>
         <td>
+
 Commands executed to build and deploy the application.
 <br/>
+The following commands are set by default:
+
+* `install`
+* `synthPipeline`
+* `deployEnvironment`
+* `destroyEnvironment`
+
+If you override the `install` command,
+either install the `aws-cdk@2` globally
+or modify the other 3 commands to use the local `cdk` binary.
+<br/>
 Commands executed on particular builds:
 
 * main pipeline:
 
   * `preInstall`
   * `install`
   * `buildAndTest`
@@ -318,14 +361,45 @@
 an additional SNS Topic will be created
 to which you can send CloudWatch Alarms.
 It's ARN is provided:
 
 * SSM: `/{projectName}/ci/slackAlarmsTopicArn`
 * Stack exported output: `{projectName}-ci-slackAlarmsTopicArn`
 
+## How to
+
+### Run unit tests during build
+
+Set commands in the `commands.buildAndTest`:
+
+```python
+{
+    commands: {
+        buildAndTest: [
+            'npm run lint',
+            'npm run test',
+        ]
+    }
+}
+```
+
+### Enable Docker
+
+Set `codeBuild.buildEnvironment.privileged` to `true`:
+
+```python
+{
+    codeBuild: {
+        buildEnvironment: {
+            privileged: true
+        }
+    }
+}
+```
+
 ## Library development
 
 Project uses [jsii](https://aws.github.io/jsii/)
 to generate packages for different languages.
 
 Install dependencies:
```

### Comparing `opinionated-ci-pipeline-1.0.0b2/setup.py` & `opinionated-ci-pipeline-1.1.0b0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "opinionated-ci-pipeline",
-    "version": "1.0.0.b2",
+    "version": "1.1.0.b0",
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
-            "opinionated-ci-pipeline@1.0.0-beta.2.jsii.tgz"
+            "opinionated-ci-pipeline@1.1.0-beta.0.jsii.tgz"
         ],
         "opinionated_ci_pipeline": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
@@ -46,15 +46,15 @@
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Typing :: Typed",
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
 )
```

### Comparing `opinionated-ci-pipeline-1.0.0b2/src/opinionated_ci_pipeline/__init__.py` & `opinionated-ci-pipeline-1.1.0b0/src/opinionated_ci_pipeline/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 # Opinionated CDK CI Pipeline
 
 [![NPM](https://img.shields.io/npm/v/opinionated-ci-pipeline?color=blue)](https://www.npmjs.com/package/opinionated-ci-pipeline)
 [![PyPI](https://img.shields.io/pypi/v/opinionated-ci-pipeline?color=blue)](https://pypi.org/project/opinionated-ci-pipeline/)
 
 CI/CD utilizing [CDK Pipelines](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.pipelines-readme.html).
 
+See the [announcement blog post](https://merapar.com/finally-the-cdk-ci-pipeline-that-serverless-deserves/) for examples and architecture diagrams.
+
 Features:
 
 * pipeline deploying application from the default branch
   to multiple environments on multiple accounts,
 * feature branch deployments to ephemeral environments,
 * development environments deployments from the local CLI,
 * build status notifications to repository commits,
@@ -30,14 +32,18 @@
     * [GitHub](#github)
     * [Bitbucket](#bitbucket)
   * [5. Bootstrap the CDK](#5-bootstrap-the-cdk)
   * [6. Deploy the CI Stack](#6-deploy-the-ci-stack)
   * [Deploy development environment](#deploy-development-environment)
 * [Parameters](#parameters)
 * [Notifications and alarms](#notifications-and-alarms)
+* [How to](#how-to)
+
+  * [Run unit tests during build](#run-unit-tests-during-build)
+  * [Enable Docker](#enable-docker)
 * [Library development](#library-development)
 
 ## Usage
 
 To set up, you need to complete the following steps:
 
 1. Install the library in your project.
@@ -216,23 +222,37 @@
     </tr>
     <tr>
         <td>packageManager</td>
         <td>npm | pnpm</td>
         <td>
 Package manager used in the repository.
 <br/>
-If provided, the install commands will be set to install dependencies using given package manager.
-        </td>
+
+If provided, the `install` command will be set to install dependencies using given package manager.
+
+</td>
     </tr>
     <tr>
         <td>commands</td>
         <td>object</td>
         <td>
+
 Commands executed to build and deploy the application.
 <br/>
+The following commands are set by default:
+
+* `install`
+* `synthPipeline`
+* `deployEnvironment`
+* `destroyEnvironment`
+
+If you override the `install` command,
+either install the `aws-cdk@2` globally
+or modify the other 3 commands to use the local `cdk` binary.
+<br/>
 Commands executed on particular builds:
 
 * main pipeline:
 
   * `preInstall`
   * `install`
   * `buildAndTest`
@@ -319,14 +339,45 @@
 an additional SNS Topic will be created
 to which you can send CloudWatch Alarms.
 It's ARN is provided:
 
 * SSM: `/{projectName}/ci/slackAlarmsTopicArn`
 * Stack exported output: `{projectName}-ci-slackAlarmsTopicArn`
 
+## How to
+
+### Run unit tests during build
+
+Set commands in the `commands.buildAndTest`:
+
+```python
+{
+    commands: {
+        buildAndTest: [
+            'npm run lint',
+            'npm run test',
+        ]
+    }
+}
+```
+
+### Enable Docker
+
+Set `codeBuild.buildEnvironment.privileged` to `true`:
+
+```python
+{
+    codeBuild: {
+        buildEnvironment: {
+            privileged: true
+        }
+    }
+}
+```
+
 ## Library development
 
 Project uses [jsii](https://aws.github.io/jsii/)
 to generate packages for different languages.
 
 Install dependencies:
 
@@ -394,25 +445,23 @@
         code_build: typing.Optional[typing.Union[_aws_cdk_pipelines_ceddda9d.CodeBuildOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         code_pipeline: typing.Optional[typing.Union["CodePipelineOverrides", typing.Dict[builtins.str, typing.Any]]] = None,
         commands: typing.Optional[typing.Union["BuildCommands", typing.Dict[builtins.str, typing.Any]]] = None,
         package_manager: typing.Optional[builtins.str] = None,
         slack_notifications: typing.Optional[typing.Union["SlackNotifications", typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''
-        :param pipeline: (experimental) CodePipeline deployment pipeline for the main repository branch. Can contain environments to deploy and waves that deploy multiple environments in parallel. Each environment and wave can have pre and post commands that will be executed before and after the environment or wave deployment.
+        :param pipeline: CodePipeline deployment pipeline for the main repository branch. Can contain environments to deploy and waves that deploy multiple environments in parallel. Each environment and wave can have pre and post commands that will be executed before and after the environment or wave deployment.
         :param repository: 
-        :param stacks: (experimental) An object with a create() method to create Stacks for the application. The same Stacks will be deployed with main pipeline, feature-branch builds, and local deployments.
-        :param cdk_output_directory: (experimental) The location where CDK outputs synthetized files. Corresponds to the CDK Pipelines ShellStepProps#primaryOutputDirectory. Default: cdk.out
-        :param code_build: (experimental) Override CodeBuild properties, used for the main pipeline as well as feature branch ephemeral environments deploys and destroys. Default: 30 minutes timeout, compute type MEDIUM with Linux build image Standard 6.0
-        :param code_pipeline: (experimental) Override CodePipeline properties.
-        :param commands: (experimental) Commands executed to build and deploy the application.
-        :param package_manager: (experimental) Package manager used in the repository. If provided, the install commands will be set to install dependencies using given package manager.
-        :param slack_notifications: (experimental) Configuration for Slack notifications. Requires configuring AWS Chatbot client manually first.
-
-        :stability: experimental
+        :param stacks: An object with a create() method to create Stacks for the application. The same Stacks will be deployed with main pipeline, feature-branch builds, and local deployments.
+        :param cdk_output_directory: The location where CDK outputs synthetized files. Corresponds to the CDK Pipelines ShellStepProps#primaryOutputDirectory. Default: cdk.out
+        :param code_build: Override CodeBuild properties, used for the main pipeline as well as feature branch ephemeral environments deploys and destroys. Default: 30 minutes timeout, compute type MEDIUM with Linux build image Standard 6.0
+        :param code_pipeline: Override CodePipeline properties.
+        :param commands: Commands executed to build and deploy the application.
+        :param package_manager: Package manager used in the repository. If provided, the install commands will be set to install dependencies using given package manager.
+        :param slack_notifications: Configuration for Slack notifications. Requires configuring AWS Chatbot client manually first.
         '''
         if isinstance(repository, dict):
             repository = RepositoryProps(**repository)
         if isinstance(code_build, dict):
             code_build = _aws_cdk_pipelines_ceddda9d.CodeBuildOptions(**code_build)
         if isinstance(code_pipeline, dict):
             code_pipeline = CodePipelineOverrides(**code_pipeline)
@@ -449,111 +498,90 @@
         if slack_notifications is not None:
             self._values["slack_notifications"] = slack_notifications
 
     @builtins.property
     def pipeline(
         self,
     ) -> typing.List[typing.Union["WaveDeployment", "EnvironmentDeployment"]]:
-        '''(experimental) CodePipeline deployment pipeline for the main repository branch.
+        '''CodePipeline deployment pipeline for the main repository branch.
 
         Can contain environments to deploy
         and waves that deploy multiple environments in parallel.
 
         Each environment and wave can have pre and post commands
         that will be executed before and after the environment or wave deployment.
-
-        :stability: experimental
         '''
         result = self._values.get("pipeline")
         assert result is not None, "Required property 'pipeline' is missing"
         return typing.cast(typing.List[typing.Union["WaveDeployment", "EnvironmentDeployment"]], result)
 
     @builtins.property
     def repository(self) -> "RepositoryProps":
-        '''
-        :stability: experimental
-        '''
         result = self._values.get("repository")
         assert result is not None, "Required property 'repository' is missing"
         return typing.cast("RepositoryProps", result)
 
     @builtins.property
     def stacks(self) -> "IStacksCreation":
-        '''(experimental) An object with a create() method to create Stacks for the application.
+        '''An object with a create() method to create Stacks for the application.
 
         The same Stacks will be deployed with main pipeline, feature-branch builds, and local deployments.
-
-        :stability: experimental
         '''
         result = self._values.get("stacks")
         assert result is not None, "Required property 'stacks' is missing"
         return typing.cast("IStacksCreation", result)
 
     @builtins.property
     def cdk_output_directory(self) -> typing.Optional[builtins.str]:
-        '''(experimental) The location where CDK outputs synthetized files.
+        '''The location where CDK outputs synthetized files.
 
         Corresponds to the CDK Pipelines ShellStepProps#primaryOutputDirectory.
 
         :default: cdk.out
-
-        :stability: experimental
         '''
         result = self._values.get("cdk_output_directory")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def code_build(
         self,
     ) -> typing.Optional[_aws_cdk_pipelines_ceddda9d.CodeBuildOptions]:
-        '''(experimental) Override CodeBuild properties, used for the main pipeline as well as feature branch ephemeral environments deploys and destroys.
+        '''Override CodeBuild properties, used for the main pipeline as well as feature branch ephemeral environments deploys and destroys.
 
         :default: 30 minutes timeout, compute type MEDIUM with Linux build image Standard 6.0
-
-        :stability: experimental
         '''
         result = self._values.get("code_build")
         return typing.cast(typing.Optional[_aws_cdk_pipelines_ceddda9d.CodeBuildOptions], result)
 
     @builtins.property
     def code_pipeline(self) -> typing.Optional["CodePipelineOverrides"]:
-        '''(experimental) Override CodePipeline properties.
-
-        :stability: experimental
-        '''
+        '''Override CodePipeline properties.'''
         result = self._values.get("code_pipeline")
         return typing.cast(typing.Optional["CodePipelineOverrides"], result)
 
     @builtins.property
     def commands(self) -> typing.Optional["BuildCommands"]:
-        '''(experimental) Commands executed to build and deploy the application.
-
-        :stability: experimental
-        '''
+        '''Commands executed to build and deploy the application.'''
         result = self._values.get("commands")
         return typing.cast(typing.Optional["BuildCommands"], result)
 
     @builtins.property
     def package_manager(self) -> typing.Optional[builtins.str]:
-        '''(experimental) Package manager used in the repository.
+        '''Package manager used in the repository.
 
         If provided, the install commands will be set to install dependencies using given package manager.
-
-        :stability: experimental
         '''
         result = self._values.get("package_manager")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def slack_notifications(self) -> typing.Optional["SlackNotifications"]:
-        '''(experimental) Configuration for Slack notifications.
+        '''Configuration for Slack notifications.
 
         Requires configuring AWS Chatbot client manually first.
-
-        :stability: experimental
         '''
         result = self._values.get("slack_notifications")
         return typing.cast(typing.Optional["SlackNotifications"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -592,16 +620,14 @@
         '''
         :param build_and_test: 
         :param deploy_environment: 
         :param destroy_environment: 
         :param install: 
         :param pre_install: 
         :param synth_pipeline: 
-
-        :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__784009b669b30e314c38fdf9a7262dc95229d2370f3ae7a3bda7d6cf264f0c25)
             check_type(argname="argument build_and_test", value=build_and_test, expected_type=type_hints["build_and_test"])
             check_type(argname="argument deploy_environment", value=deploy_environment, expected_type=type_hints["deploy_environment"])
             check_type(argname="argument destroy_environment", value=destroy_environment, expected_type=type_hints["destroy_environment"])
             check_type(argname="argument install", value=install, expected_type=type_hints["install"])
@@ -619,57 +645,39 @@
         if pre_install is not None:
             self._values["pre_install"] = pre_install
         if synth_pipeline is not None:
             self._values["synth_pipeline"] = synth_pipeline
 
     @builtins.property
     def build_and_test(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''
-        :stability: experimental
-        '''
         result = self._values.get("build_and_test")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def deploy_environment(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''
-        :stability: experimental
-        '''
         result = self._values.get("deploy_environment")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def destroy_environment(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''
-        :stability: experimental
-        '''
         result = self._values.get("destroy_environment")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def install(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''
-        :stability: experimental
-        '''
         result = self._values.get("install")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def pre_install(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''
-        :stability: experimental
-        '''
         result = self._values.get("pre_install")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def synth_pipeline(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''
-        :stability: experimental
-        '''
         result = self._values.get("synth_pipeline")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -682,18 +690,14 @@
 
 
 class CDKApplication(
     _aws_cdk_ceddda9d.App,
     metaclass=jsii.JSIIMeta,
     jsii_type="opinionated-ci-pipeline.CDKApplication",
 ):
-    '''
-    :stability: experimental
-    '''
-
     def __init__(
         self,
         *,
         analytics_reporting: typing.Optional[builtins.bool] = None,
         auto_synth: typing.Optional[builtins.bool] = None,
         context: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         default_stack_synthesizer: typing.Optional[_aws_cdk_ceddda9d.IReusableStackSynthesizer] = None,
@@ -716,25 +720,23 @@
         :param auto_synth: Automatically call ``synth()`` before the program exits. If you set this, you don't have to call ``synth()`` explicitly. Note that this feature is only available for certain programming languages, and calling ``synth()`` is still recommended. Default: true if running via CDK CLI (``CDK_OUTDIR`` is set), ``false`` otherwise
         :param context: Additional context values for the application. Context set by the CLI or the ``context`` key in ``cdk.json`` has precedence. Context can be read from any construct using ``node.getContext(key)``. Default: - no additional context
         :param default_stack_synthesizer: The stack synthesizer to use by default for all Stacks in the App. The Stack Synthesizer controls aspects of synthesis and deployment, like how assets are referenced and what IAM roles to use. For more information, see the README of the main CDK package. Default: - A ``DefaultStackSynthesizer`` with default settings
         :param outdir: The output directory into which to emit synthesized artifacts. You should never need to set this value. By default, the value you pass to the CLI's ``--output`` flag will be used, and if you change it to a different directory the CLI will fail to pick up the generated Cloud Assembly. This property is intended for internal and testing use. Default: - If this value is *not* set, considers the environment variable ``CDK_OUTDIR``. If ``CDK_OUTDIR`` is not defined, uses a temp directory.
         :param post_cli_context: Additional context values for the application. Context provided here has precedence over context set by: - The CLI via --context - The ``context`` key in ``cdk.json`` - The ``AppProps.context`` property This property is recommended over the ``AppProps.context`` property since you can make final decision over which context value to take in your app. Context can be read from any construct using ``node.getContext(key)``. Default: - no additional context
         :param stack_traces: Include construct creation stack trace in the ``aws:cdk:trace`` metadata key of all constructs. Default: true stack traces are included unless ``aws:cdk:disable-stack-trace`` is set in the context.
         :param tree_metadata: Include construct tree metadata as part of the Cloud Assembly. Default: true
-        :param pipeline: (experimental) CodePipeline deployment pipeline for the main repository branch. Can contain environments to deploy and waves that deploy multiple environments in parallel. Each environment and wave can have pre and post commands that will be executed before and after the environment or wave deployment.
+        :param pipeline: CodePipeline deployment pipeline for the main repository branch. Can contain environments to deploy and waves that deploy multiple environments in parallel. Each environment and wave can have pre and post commands that will be executed before and after the environment or wave deployment.
         :param repository: 
-        :param stacks: (experimental) An object with a create() method to create Stacks for the application. The same Stacks will be deployed with main pipeline, feature-branch builds, and local deployments.
-        :param cdk_output_directory: (experimental) The location where CDK outputs synthetized files. Corresponds to the CDK Pipelines ShellStepProps#primaryOutputDirectory. Default: cdk.out
-        :param code_build: (experimental) Override CodeBuild properties, used for the main pipeline as well as feature branch ephemeral environments deploys and destroys. Default: 30 minutes timeout, compute type MEDIUM with Linux build image Standard 6.0
-        :param code_pipeline: (experimental) Override CodePipeline properties.
-        :param commands: (experimental) Commands executed to build and deploy the application.
-        :param package_manager: (experimental) Package manager used in the repository. If provided, the install commands will be set to install dependencies using given package manager.
-        :param slack_notifications: (experimental) Configuration for Slack notifications. Requires configuring AWS Chatbot client manually first.
-
-        :stability: experimental
+        :param stacks: An object with a create() method to create Stacks for the application. The same Stacks will be deployed with main pipeline, feature-branch builds, and local deployments.
+        :param cdk_output_directory: The location where CDK outputs synthetized files. Corresponds to the CDK Pipelines ShellStepProps#primaryOutputDirectory. Default: cdk.out
+        :param code_build: Override CodeBuild properties, used for the main pipeline as well as feature branch ephemeral environments deploys and destroys. Default: 30 minutes timeout, compute type MEDIUM with Linux build image Standard 6.0
+        :param code_pipeline: Override CodePipeline properties.
+        :param commands: Commands executed to build and deploy the application.
+        :param package_manager: Package manager used in the repository. If provided, the install commands will be set to install dependencies using given package manager.
+        :param slack_notifications: Configuration for Slack notifications. Requires configuring AWS Chatbot client manually first.
         '''
         props = CDKApplicationProps(
             analytics_reporting=analytics_reporting,
             auto_synth=auto_synth,
             context=context,
             default_stack_synthesizer=default_stack_synthesizer,
             outdir=outdir,
@@ -805,25 +807,23 @@
         :param auto_synth: Automatically call ``synth()`` before the program exits. If you set this, you don't have to call ``synth()`` explicitly. Note that this feature is only available for certain programming languages, and calling ``synth()`` is still recommended. Default: true if running via CDK CLI (``CDK_OUTDIR`` is set), ``false`` otherwise
         :param context: Additional context values for the application. Context set by the CLI or the ``context`` key in ``cdk.json`` has precedence. Context can be read from any construct using ``node.getContext(key)``. Default: - no additional context
         :param default_stack_synthesizer: The stack synthesizer to use by default for all Stacks in the App. The Stack Synthesizer controls aspects of synthesis and deployment, like how assets are referenced and what IAM roles to use. For more information, see the README of the main CDK package. Default: - A ``DefaultStackSynthesizer`` with default settings
         :param outdir: The output directory into which to emit synthesized artifacts. You should never need to set this value. By default, the value you pass to the CLI's ``--output`` flag will be used, and if you change it to a different directory the CLI will fail to pick up the generated Cloud Assembly. This property is intended for internal and testing use. Default: - If this value is *not* set, considers the environment variable ``CDK_OUTDIR``. If ``CDK_OUTDIR`` is not defined, uses a temp directory.
         :param post_cli_context: Additional context values for the application. Context provided here has precedence over context set by: - The CLI via --context - The ``context`` key in ``cdk.json`` - The ``AppProps.context`` property This property is recommended over the ``AppProps.context`` property since you can make final decision over which context value to take in your app. Context can be read from any construct using ``node.getContext(key)``. Default: - no additional context
         :param stack_traces: Include construct creation stack trace in the ``aws:cdk:trace`` metadata key of all constructs. Default: true stack traces are included unless ``aws:cdk:disable-stack-trace`` is set in the context.
         :param tree_metadata: Include construct tree metadata as part of the Cloud Assembly. Default: true
-        :param pipeline: (experimental) CodePipeline deployment pipeline for the main repository branch. Can contain environments to deploy and waves that deploy multiple environments in parallel. Each environment and wave can have pre and post commands that will be executed before and after the environment or wave deployment.
+        :param pipeline: CodePipeline deployment pipeline for the main repository branch. Can contain environments to deploy and waves that deploy multiple environments in parallel. Each environment and wave can have pre and post commands that will be executed before and after the environment or wave deployment.
         :param repository: 
-        :param stacks: (experimental) An object with a create() method to create Stacks for the application. The same Stacks will be deployed with main pipeline, feature-branch builds, and local deployments.
-        :param cdk_output_directory: (experimental) The location where CDK outputs synthetized files. Corresponds to the CDK Pipelines ShellStepProps#primaryOutputDirectory. Default: cdk.out
-        :param code_build: (experimental) Override CodeBuild properties, used for the main pipeline as well as feature branch ephemeral environments deploys and destroys. Default: 30 minutes timeout, compute type MEDIUM with Linux build image Standard 6.0
-        :param code_pipeline: (experimental) Override CodePipeline properties.
-        :param commands: (experimental) Commands executed to build and deploy the application.
-        :param package_manager: (experimental) Package manager used in the repository. If provided, the install commands will be set to install dependencies using given package manager.
-        :param slack_notifications: (experimental) Configuration for Slack notifications. Requires configuring AWS Chatbot client manually first.
-
-        :stability: experimental
+        :param stacks: An object with a create() method to create Stacks for the application. The same Stacks will be deployed with main pipeline, feature-branch builds, and local deployments.
+        :param cdk_output_directory: The location where CDK outputs synthetized files. Corresponds to the CDK Pipelines ShellStepProps#primaryOutputDirectory. Default: cdk.out
+        :param code_build: Override CodeBuild properties, used for the main pipeline as well as feature branch ephemeral environments deploys and destroys. Default: 30 minutes timeout, compute type MEDIUM with Linux build image Standard 6.0
+        :param code_pipeline: Override CodePipeline properties.
+        :param commands: Commands executed to build and deploy the application.
+        :param package_manager: Package manager used in the repository. If provided, the install commands will be set to install dependencies using given package manager.
+        :param slack_notifications: Configuration for Slack notifications. Requires configuring AWS Chatbot client manually first.
         '''
         if isinstance(repository, dict):
             repository = RepositoryProps(**repository)
         if isinstance(code_build, dict):
             code_build = _aws_cdk_pipelines_ceddda9d.CodeBuildOptions(**code_build)
         if isinstance(code_pipeline, dict):
             code_pipeline = CodePipelineOverrides(**code_pipeline)
@@ -1009,111 +1009,90 @@
         result = self._values.get("tree_metadata")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def pipeline(
         self,
     ) -> typing.List[typing.Union["WaveDeployment", "EnvironmentDeployment"]]:
-        '''(experimental) CodePipeline deployment pipeline for the main repository branch.
+        '''CodePipeline deployment pipeline for the main repository branch.
 
         Can contain environments to deploy
         and waves that deploy multiple environments in parallel.
 
         Each environment and wave can have pre and post commands
         that will be executed before and after the environment or wave deployment.
-
-        :stability: experimental
         '''
         result = self._values.get("pipeline")
         assert result is not None, "Required property 'pipeline' is missing"
         return typing.cast(typing.List[typing.Union["WaveDeployment", "EnvironmentDeployment"]], result)
 
     @builtins.property
     def repository(self) -> "RepositoryProps":
-        '''
-        :stability: experimental
-        '''
         result = self._values.get("repository")
         assert result is not None, "Required property 'repository' is missing"
         return typing.cast("RepositoryProps", result)
 
     @builtins.property
     def stacks(self) -> "IStacksCreation":
-        '''(experimental) An object with a create() method to create Stacks for the application.
+        '''An object with a create() method to create Stacks for the application.
 
         The same Stacks will be deployed with main pipeline, feature-branch builds, and local deployments.
-
-        :stability: experimental
         '''
         result = self._values.get("stacks")
         assert result is not None, "Required property 'stacks' is missing"
         return typing.cast("IStacksCreation", result)
 
     @builtins.property
     def cdk_output_directory(self) -> typing.Optional[builtins.str]:
-        '''(experimental) The location where CDK outputs synthetized files.
+        '''The location where CDK outputs synthetized files.
 
         Corresponds to the CDK Pipelines ShellStepProps#primaryOutputDirectory.
 
         :default: cdk.out
-
-        :stability: experimental
         '''
         result = self._values.get("cdk_output_directory")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def code_build(
         self,
     ) -> typing.Optional[_aws_cdk_pipelines_ceddda9d.CodeBuildOptions]:
-        '''(experimental) Override CodeBuild properties, used for the main pipeline as well as feature branch ephemeral environments deploys and destroys.
+        '''Override CodeBuild properties, used for the main pipeline as well as feature branch ephemeral environments deploys and destroys.
 
         :default: 30 minutes timeout, compute type MEDIUM with Linux build image Standard 6.0
-
-        :stability: experimental
         '''
         result = self._values.get("code_build")
         return typing.cast(typing.Optional[_aws_cdk_pipelines_ceddda9d.CodeBuildOptions], result)
 
     @builtins.property
     def code_pipeline(self) -> typing.Optional["CodePipelineOverrides"]:
-        '''(experimental) Override CodePipeline properties.
-
-        :stability: experimental
-        '''
+        '''Override CodePipeline properties.'''
         result = self._values.get("code_pipeline")
         return typing.cast(typing.Optional["CodePipelineOverrides"], result)
 
     @builtins.property
     def commands(self) -> typing.Optional[BuildCommands]:
-        '''(experimental) Commands executed to build and deploy the application.
-
-        :stability: experimental
-        '''
+        '''Commands executed to build and deploy the application.'''
         result = self._values.get("commands")
         return typing.cast(typing.Optional[BuildCommands], result)
 
     @builtins.property
     def package_manager(self) -> typing.Optional[builtins.str]:
-        '''(experimental) Package manager used in the repository.
+        '''Package manager used in the repository.
 
         If provided, the install commands will be set to install dependencies using given package manager.
-
-        :stability: experimental
         '''
         result = self._values.get("package_manager")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def slack_notifications(self) -> typing.Optional["SlackNotifications"]:
-        '''(experimental) Configuration for Slack notifications.
+        '''Configuration for Slack notifications.
 
         Requires configuring AWS Chatbot client manually first.
-
-        :stability: experimental
         '''
         result = self._values.get("slack_notifications")
         return typing.cast(typing.Optional["SlackNotifications"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1161,15 +1140,15 @@
         reuse_cross_region_support_stacks: typing.Optional[builtins.bool] = None,
         role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
         self_mutation: typing.Optional[builtins.bool] = None,
         self_mutation_code_build_defaults: typing.Optional[typing.Union[_aws_cdk_pipelines_ceddda9d.CodeBuildOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         synth_code_build_defaults: typing.Optional[typing.Union[_aws_cdk_pipelines_ceddda9d.CodeBuildOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         use_change_sets: typing.Optional[builtins.bool] = None,
     ) -> None:
-        '''(experimental) Since jsii does not support Partial or Omit, we have to define all properties from CodePipelineProps that may be overriden manually.
+        '''Since jsii does not support Partial or Omit, we have to define all properties from CodePipelineProps that may be overriden manually.
 
         :param asset_publishing_code_build_defaults: 
         :param code_build_defaults: 
         :param docker_credentials: 
         :param docker_enabled_for_self_mutation: 
         :param docker_enabled_for_synth: 
         :param enable_key_rotation: 
@@ -1177,16 +1156,14 @@
         :param publish_assets_in_parallel: 
         :param reuse_cross_region_support_stacks: 
         :param role: 
         :param self_mutation: 
         :param self_mutation_code_build_defaults: 
         :param synth_code_build_defaults: 
         :param use_change_sets: 
-
-        :stability: experimental
         '''
         if isinstance(asset_publishing_code_build_defaults, dict):
             asset_publishing_code_build_defaults = _aws_cdk_pipelines_ceddda9d.CodeBuildOptions(**asset_publishing_code_build_defaults)
         if isinstance(code_build_defaults, dict):
             code_build_defaults = _aws_cdk_pipelines_ceddda9d.CodeBuildOptions(**code_build_defaults)
         if isinstance(self_mutation_code_build_defaults, dict):
             self_mutation_code_build_defaults = _aws_cdk_pipelines_ceddda9d.CodeBuildOptions(**self_mutation_code_build_defaults)
@@ -1238,129 +1215,87 @@
         if use_change_sets is not None:
             self._values["use_change_sets"] = use_change_sets
 
     @builtins.property
     def asset_publishing_code_build_defaults(
         self,
     ) -> typing.Optional[_aws_cdk_pipelines_ceddda9d.CodeBuildOptions]:
-        '''
-        :stability: experimental
-        '''
         result = self._values.get("asset_publishing_code_build_defaults")
         return typing.cast(typing.Optional[_aws_cdk_pipelines_ceddda9d.CodeBuildOptions], result)
 
     @builtins.property
     def code_build_defaults(
         self,
     ) -> typing.Optional[_aws_cdk_pipelines_ceddda9d.CodeBuildOptions]:
-        '''
-        :stability: experimental
-        '''
         result = self._values.get("code_build_defaults")
         return typing.cast(typing.Optional[_aws_cdk_pipelines_ceddda9d.CodeBuildOptions], result)
 
     @builtins.property
     def docker_credentials(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_pipelines_ceddda9d.DockerCredential]]:
-        '''
-        :stability: experimental
-        '''
         result = self._values.get("docker_credentials")
         return typing.cast(typing.Optional[typing.List[_aws_cdk_pipelines_ceddda9d.DockerCredential]], result)
 
     @builtins.property
     def docker_enabled_for_self_mutation(self) -> typing.Optional[builtins.bool]:
-        '''
-        :stability: experimental
-        '''
         result = self._values.get("docker_enabled_for_self_mutation")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def docker_enabled_for_synth(self) -> typing.Optional[builtins.bool]:
-        '''
-        :stability: experimental
-        '''
         result = self._values.get("docker_enabled_for_synth")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def enable_key_rotation(self) -> typing.Optional[builtins.bool]:
-        '''
-        :stability: experimental
-        '''
         result = self._values.get("enable_key_rotation")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def pipeline_name(self) -> typing.Optional[builtins.str]:
-        '''
-        :stability: experimental
-        '''
         result = self._values.get("pipeline_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def publish_assets_in_parallel(self) -> typing.Optional[builtins.bool]:
-        '''
-        :stability: experimental
-        '''
         result = self._values.get("publish_assets_in_parallel")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def reuse_cross_region_support_stacks(self) -> typing.Optional[builtins.bool]:
-        '''
-        :stability: experimental
-        '''
         result = self._values.get("reuse_cross_region_support_stacks")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def role(self) -> typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole]:
-        '''
-        :stability: experimental
-        '''
         result = self._values.get("role")
         return typing.cast(typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole], result)
 
     @builtins.property
     def self_mutation(self) -> typing.Optional[builtins.bool]:
-        '''
-        :stability: experimental
-        '''
         result = self._values.get("self_mutation")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def self_mutation_code_build_defaults(
         self,
     ) -> typing.Optional[_aws_cdk_pipelines_ceddda9d.CodeBuildOptions]:
-        '''
-        :stability: experimental
-        '''
         result = self._values.get("self_mutation_code_build_defaults")
         return typing.cast(typing.Optional[_aws_cdk_pipelines_ceddda9d.CodeBuildOptions], result)
 
     @builtins.property
     def synth_code_build_defaults(
         self,
     ) -> typing.Optional[_aws_cdk_pipelines_ceddda9d.CodeBuildOptions]:
-        '''
-        :stability: experimental
-        '''
         result = self._values.get("synth_code_build_defaults")
         return typing.cast(typing.Optional[_aws_cdk_pipelines_ceddda9d.CodeBuildOptions], result)
 
     @builtins.property
     def use_change_sets(self) -> typing.Optional[builtins.bool]:
-        '''
-        :stability: experimental
-        '''
         result = self._values.get("use_change_sets")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -1382,19 +1317,17 @@
         self,
         *,
         environment: builtins.str,
         post: typing.Optional[typing.Sequence[builtins.str]] = None,
         pre: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param environment: (experimental) Environment name. Environment will be deployed to AWS account and region defined in cdk.json file ``context/environments`` properties, falling back to the ``default`` environment settings if given environment configuration is not found.
-        :param post: (experimental) Commands to execute after the environment deployment.
-        :param pre: (experimental) Commands to execute before the environment deployment.
-
-        :stability: experimental
+        :param environment: Environment name. Environment will be deployed to AWS account and region defined in cdk.json file ``context/environments`` properties, falling back to the ``default`` environment settings if given environment configuration is not found.
+        :param post: Commands to execute after the environment deployment.
+        :param pre: Commands to execute before the environment deployment.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__8a56d8f8652385a6beef9373eed0946aec4a1e2ca901b17252542af97a91c99a)
             check_type(argname="argument environment", value=environment, expected_type=type_hints["environment"])
             check_type(argname="argument post", value=post, expected_type=type_hints["post"])
             check_type(argname="argument pre", value=pre, expected_type=type_hints["pre"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
@@ -1403,41 +1336,33 @@
         if post is not None:
             self._values["post"] = post
         if pre is not None:
             self._values["pre"] = pre
 
     @builtins.property
     def environment(self) -> builtins.str:
-        '''(experimental) Environment name.
+        '''Environment name.
 
         Environment will be deployed to AWS account and region
         defined in cdk.json file ``context/environments`` properties,
         falling back to the ``default`` environment settings if given environment configuration is not found.
-
-        :stability: experimental
         '''
         result = self._values.get("environment")
         assert result is not None, "Required property 'environment' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def post(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''(experimental) Commands to execute after the environment deployment.
-
-        :stability: experimental
-        '''
+        '''Commands to execute after the environment deployment.'''
         result = self._values.get("post")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def pre(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''(experimental) Commands to execute before the environment deployment.
-
-        :stability: experimental
-        '''
+        '''Commands to execute before the environment deployment.'''
         result = self._values.get("pre")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -1447,77 +1372,69 @@
         return "EnvironmentDeployment(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.interface(jsii_type="opinionated-ci-pipeline.IStacksCreation")
 class IStacksCreation(typing_extensions.Protocol):
-    '''(experimental) To provide a method as parameter, jsii requires creating a behavioral interface, prefixed with "I".
+    '''To provide a method as parameter, jsii requires creating a behavioral interface, prefixed with "I".
 
     Mixing structural and behavioral interfaces is not always possible, hence we extract stacks creation
     to a separate object described by this behavioral interface.
-
-    :stability: experimental
     '''
 
     @jsii.member(jsii_name="create")
     def create(
         self,
         scope: _constructs_77d1e7e8.Construct,
         project_name: builtins.str,
         env_name: builtins.str,
     ) -> None:
-        '''(experimental) Create Stacks for the application.
+        '''Create Stacks for the application.
 
         Use provided scope as stacks' parent (first constructor argument).
 
         Stacks must include provided environment name in their names
         to distinguish them when deploying multiple environments
         (like feature-branch environments) to the same account.
 
         :param scope: -
         :param project_name: -
         :param env_name: -
-
-        :stability: experimental
         '''
         ...
 
 
 class _IStacksCreationProxy:
-    '''(experimental) To provide a method as parameter, jsii requires creating a behavioral interface, prefixed with "I".
+    '''To provide a method as parameter, jsii requires creating a behavioral interface, prefixed with "I".
 
     Mixing structural and behavioral interfaces is not always possible, hence we extract stacks creation
     to a separate object described by this behavioral interface.
-
-    :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "opinionated-ci-pipeline.IStacksCreation"
 
     @jsii.member(jsii_name="create")
     def create(
         self,
         scope: _constructs_77d1e7e8.Construct,
         project_name: builtins.str,
         env_name: builtins.str,
     ) -> None:
-        '''(experimental) Create Stacks for the application.
+        '''Create Stacks for the application.
 
         Use provided scope as stacks' parent (first constructor argument).
 
         Stacks must include provided environment name in their names
         to distinguish them when deploying multiple environments
         (like feature-branch environments) to the same account.
 
         :param scope: -
         :param project_name: -
         :param env_name: -
-
-        :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__6f94daa933ae3ad6d5e4b09fd8274268c1c6c4ce67db84eea5360a505e3c5d56)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument project_name", value=project_name, expected_type=type_hints["project_name"])
             check_type(argname="argument env_name", value=env_name, expected_type=type_hints["env_name"])
         return typing.cast(None, jsii.invoke(self, "create", [scope, project_name, env_name]))
@@ -1536,19 +1453,17 @@
         self,
         *,
         host: builtins.str,
         name: builtins.str,
         default_branch: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param host: (experimental) Repository hosting.
-        :param name: (experimental) Like "my-comapny/my-repo".
-        :param default_branch: (experimental) Branch to deploy the environments from in the main pipeline. Default: main
-
-        :stability: experimental
+        :param host: Repository hosting.
+        :param name: Like "my-comapny/my-repo".
+        :param default_branch: Branch to deploy the environments from in the main pipeline. Default: main
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f6f830ab1d423354edc601071d8aae1b0849f4eb33644f06838e41508d8ba714)
             check_type(argname="argument host", value=host, expected_type=type_hints["host"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument default_branch", value=default_branch, expected_type=type_hints["default_branch"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
@@ -1556,39 +1471,31 @@
             "name": name,
         }
         if default_branch is not None:
             self._values["default_branch"] = default_branch
 
     @builtins.property
     def host(self) -> builtins.str:
-        '''(experimental) Repository hosting.
-
-        :stability: experimental
-        '''
+        '''Repository hosting.'''
         result = self._values.get("host")
         assert result is not None, "Required property 'host' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''(experimental) Like "my-comapny/my-repo".
-
-        :stability: experimental
-        '''
+        '''Like "my-comapny/my-repo".'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def default_branch(self) -> typing.Optional[builtins.str]:
-        '''(experimental) Branch to deploy the environments from in the main pipeline.
+        '''Branch to deploy the environments from in the main pipeline.
 
         :default: main
-
-        :stability: experimental
         '''
         result = self._values.get("default_branch")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1619,18 +1526,16 @@
         workspace_id: builtins.str,
         feature_branch_failures: typing.Optional[builtins.bool] = None,
         main_pipeline_failures: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''
         :param channel_id: 
         :param workspace_id: 
-        :param feature_branch_failures: (experimental) Whether to notify about feature branch deployment failures. Default: false
-        :param main_pipeline_failures: (experimental) Whether to notify about main pipeline failures. Default: true
-
-        :stability: experimental
+        :param feature_branch_failures: Whether to notify about feature branch deployment failures. Default: false
+        :param main_pipeline_failures: Whether to notify about main pipeline failures. Default: true
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__62e47fdb1eef2b0738fcc2152a329dd258aee175431814841e5687481f56c87b)
             check_type(argname="argument channel_id", value=channel_id, expected_type=type_hints["channel_id"])
             check_type(argname="argument workspace_id", value=workspace_id, expected_type=type_hints["workspace_id"])
             check_type(argname="argument feature_branch_failures", value=feature_branch_failures, expected_type=type_hints["feature_branch_failures"])
             check_type(argname="argument main_pipeline_failures", value=main_pipeline_failures, expected_type=type_hints["main_pipeline_failures"])
@@ -1641,48 +1546,38 @@
         if feature_branch_failures is not None:
             self._values["feature_branch_failures"] = feature_branch_failures
         if main_pipeline_failures is not None:
             self._values["main_pipeline_failures"] = main_pipeline_failures
 
     @builtins.property
     def channel_id(self) -> builtins.str:
-        '''
-        :stability: experimental
-        '''
         result = self._values.get("channel_id")
         assert result is not None, "Required property 'channel_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def workspace_id(self) -> builtins.str:
-        '''
-        :stability: experimental
-        '''
         result = self._values.get("workspace_id")
         assert result is not None, "Required property 'workspace_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def feature_branch_failures(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Whether to notify about feature branch deployment failures.
+        '''Whether to notify about feature branch deployment failures.
 
         :default: false
-
-        :stability: experimental
         '''
         result = self._values.get("feature_branch_failures")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def main_pipeline_failures(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Whether to notify about main pipeline failures.
+        '''Whether to notify about main pipeline failures.
 
         :default: true
-
-        :stability: experimental
         '''
         result = self._values.get("main_pipeline_failures")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1715,22 +1610,20 @@
         wave: builtins.str,
         post: typing.Optional[typing.Sequence[builtins.str]] = None,
         post_each_environment: typing.Optional[typing.Sequence[builtins.str]] = None,
         pre: typing.Optional[typing.Sequence[builtins.str]] = None,
         pre_each_environment: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param environments: (experimental) List of environments to deploy in parallel.
-        :param wave: (experimental) Wave name.
-        :param post: (experimental) Commands to execute after the wave deployment.
-        :param post_each_environment: (experimental) Commands to execute after environment deployment. If environment configuration also contains commands to execute post-deployment, they will be executed before the commands defined here.
-        :param pre: (experimental) Commands to execute before the wave deployment.
-        :param pre_each_environment: (experimental) Commands to execute before each environment deployment. If environment configuration also contains commands to execute pre-deployment, they will be executed after the commands defined here.
-
-        :stability: experimental
+        :param environments: List of environments to deploy in parallel.
+        :param wave: Wave name.
+        :param post: Commands to execute after the wave deployment.
+        :param post_each_environment: Commands to execute after environment deployment. If environment configuration also contains commands to execute post-deployment, they will be executed before the commands defined here.
+        :param pre: Commands to execute before the wave deployment.
+        :param pre_each_environment: Commands to execute before each environment deployment. If environment configuration also contains commands to execute pre-deployment, they will be executed after the commands defined here.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__3e2f9daf95ae58e92db6a6c5f2f46d1d02b4f767b770eaf9116fc04ca2c5158e)
             check_type(argname="argument environments", value=environments, expected_type=type_hints["environments"])
             check_type(argname="argument wave", value=wave, expected_type=type_hints["wave"])
             check_type(argname="argument post", value=post, expected_type=type_hints["post"])
             check_type(argname="argument post_each_environment", value=post_each_environment, expected_type=type_hints["post_each_environment"])
@@ -1747,70 +1640,54 @@
         if pre is not None:
             self._values["pre"] = pre
         if pre_each_environment is not None:
             self._values["pre_each_environment"] = pre_each_environment
 
     @builtins.property
     def environments(self) -> typing.List[EnvironmentDeployment]:
-        '''(experimental) List of environments to deploy in parallel.
-
-        :stability: experimental
-        '''
+        '''List of environments to deploy in parallel.'''
         result = self._values.get("environments")
         assert result is not None, "Required property 'environments' is missing"
         return typing.cast(typing.List[EnvironmentDeployment], result)
 
     @builtins.property
     def wave(self) -> builtins.str:
-        '''(experimental) Wave name.
-
-        :stability: experimental
-        '''
+        '''Wave name.'''
         result = self._values.get("wave")
         assert result is not None, "Required property 'wave' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def post(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''(experimental) Commands to execute after the wave deployment.
-
-        :stability: experimental
-        '''
+        '''Commands to execute after the wave deployment.'''
         result = self._values.get("post")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def post_each_environment(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''(experimental) Commands to execute after environment deployment.
+        '''Commands to execute after environment deployment.
 
         If environment configuration also contains commands to execute post-deployment,
         they will be executed before the commands defined here.
-
-        :stability: experimental
         '''
         result = self._values.get("post_each_environment")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def pre(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''(experimental) Commands to execute before the wave deployment.
-
-        :stability: experimental
-        '''
+        '''Commands to execute before the wave deployment.'''
         result = self._values.get("pre")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def pre_each_environment(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''(experimental) Commands to execute before each environment deployment.
+        '''Commands to execute before each environment deployment.
 
         If environment configuration also contains commands to execute pre-deployment,
         they will be executed after the commands defined here.
-
-        :stability: experimental
         '''
         result = self._values.get("pre_each_environment")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `opinionated-ci-pipeline-1.0.0b2/src/opinionated_ci_pipeline.egg-info/PKG-INFO` & `opinionated-ci-pipeline-1.1.0b0/src/opinionated_ci_pipeline.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 Metadata-Version: 2.1
 Name: opinionated-ci-pipeline
-Version: 1.0.0b2
+Version: 1.1.0b0
 Summary: CI/CD on AWS with feature-branch builds, developer-environment deployments, and build status notifications.
 Home-page: https://github.com/merapar/opinionated-ci-pipeline.git
 Author: Maciej Radzikowski<maciej.radzikowski@merapar.com>
 License: MIT
 Project-URL: Source, https://github.com/merapar/opinionated-ci-pipeline.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Typing :: Typed
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Opinionated CDK CI Pipeline
 
 [![NPM](https://img.shields.io/npm/v/opinionated-ci-pipeline?color=blue)](https://www.npmjs.com/package/opinionated-ci-pipeline)
 [![PyPI](https://img.shields.io/pypi/v/opinionated-ci-pipeline?color=blue)](https://pypi.org/project/opinionated-ci-pipeline/)
 
 CI/CD utilizing [CDK Pipelines](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.pipelines-readme.html).
 
+See the [announcement blog post](https://merapar.com/finally-the-cdk-ci-pipeline-that-serverless-deserves/) for examples and architecture diagrams.
+
 Features:
 
 * pipeline deploying application from the default branch
   to multiple environments on multiple accounts,
 * feature branch deployments to ephemeral environments,
 * development environments deployments from the local CLI,
 * build status notifications to repository commits,
@@ -52,14 +54,18 @@
     * [GitHub](#github)
     * [Bitbucket](#bitbucket)
   * [5. Bootstrap the CDK](#5-bootstrap-the-cdk)
   * [6. Deploy the CI Stack](#6-deploy-the-ci-stack)
   * [Deploy development environment](#deploy-development-environment)
 * [Parameters](#parameters)
 * [Notifications and alarms](#notifications-and-alarms)
+* [How to](#how-to)
+
+  * [Run unit tests during build](#run-unit-tests-during-build)
+  * [Enable Docker](#enable-docker)
 * [Library development](#library-development)
 
 ## Usage
 
 To set up, you need to complete the following steps:
 
 1. Install the library in your project.
@@ -238,23 +244,37 @@
     </tr>
     <tr>
         <td>packageManager</td>
         <td>npm | pnpm</td>
         <td>
 Package manager used in the repository.
 <br/>
-If provided, the install commands will be set to install dependencies using given package manager.
-        </td>
+
+If provided, the `install` command will be set to install dependencies using given package manager.
+
+</td>
     </tr>
     <tr>
         <td>commands</td>
         <td>object</td>
         <td>
+
 Commands executed to build and deploy the application.
 <br/>
+The following commands are set by default:
+
+* `install`
+* `synthPipeline`
+* `deployEnvironment`
+* `destroyEnvironment`
+
+If you override the `install` command,
+either install the `aws-cdk@2` globally
+or modify the other 3 commands to use the local `cdk` binary.
+<br/>
 Commands executed on particular builds:
 
 * main pipeline:
 
   * `preInstall`
   * `install`
   * `buildAndTest`
@@ -341,14 +361,45 @@
 an additional SNS Topic will be created
 to which you can send CloudWatch Alarms.
 It's ARN is provided:
 
 * SSM: `/{projectName}/ci/slackAlarmsTopicArn`
 * Stack exported output: `{projectName}-ci-slackAlarmsTopicArn`
 
+## How to
+
+### Run unit tests during build
+
+Set commands in the `commands.buildAndTest`:
+
+```python
+{
+    commands: {
+        buildAndTest: [
+            'npm run lint',
+            'npm run test',
+        ]
+    }
+}
+```
+
+### Enable Docker
+
+Set `codeBuild.buildEnvironment.privileged` to `true`:
+
+```python
+{
+    codeBuild: {
+        buildEnvironment: {
+            privileged: true
+        }
+    }
+}
+```
+
 ## Library development
 
 Project uses [jsii](https://aws.github.io/jsii/)
 to generate packages for different languages.
 
 Install dependencies:
```

