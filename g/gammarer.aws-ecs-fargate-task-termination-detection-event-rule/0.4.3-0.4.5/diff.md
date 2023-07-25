# Comparing `tmp/gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3.tar.gz` & `tmp/gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3.tar", last modified: Sun Jul 23 18:23:10 2023, max compression
+gzip compressed data, was "gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5.tar", last modified: Tue Jul 25 18:24:35 2023, max compression
```

## Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3.tar` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 18:23:10.854287 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-23 18:22:58.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-23 18:22:58.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-23 18:23:10.854287 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-23 18:22:58.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-23 18:22:58.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 18:23:10.854287 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-23 18:22:58.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 18:23:10.854287 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 18:23:10.854287 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 18:23:10.854287 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-07-23 18:22:58.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 18:23:10.854287 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-23 18:22:58.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17502 2023-07-23 18:22:58.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/aws-ecs-fargate-task-termination-detection-event-rule@0.4.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 18:22:58.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 18:23:10.854287 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-23 18:23:10.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-23 18:23:10.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 18:23:10.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-23 18:23:10.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-23 18:23:10.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:24:35.432511 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-25 18:24:23.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 18:24:23.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-25 18:24:35.432511 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-25 18:24:23.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-25 18:24:23.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 18:24:35.432511 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-25 18:24:23.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:24:35.428511 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:24:35.428511 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:24:35.432511 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-07-25 18:24:23.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:24:35.432511 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-25 18:24:23.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17501 2023-07-25 18:24:23.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/aws-ecs-fargate-task-termination-detection-event-rule@0.4.5.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:24:23.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:24:35.432511 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-25 18:24:35.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-25 18:24:35.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:24:35.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-25 18:24:35.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 18:24:35.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/top_level.txt
```

### Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3/LICENSE` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3/PKG-INFO` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-ecs-fargate-task-termination-detection-event-rule
-Version: 0.4.3
+Version: 0.4.5
 Summary: This an AWS ECS Fargate task termination detection Event Rule.
 Home-page: https://github.com/yicr/aws-ecs-fargate-task-termination-detection-event-rule.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-ecs-fargate-task-termination-detection-event-rule.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3/README.md` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3/setup.py` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-ecs-fargate-task-termination-detection-event-rule",
-    "version": "0.4.3",
+    "version": "0.4.5",
     "description": "This an AWS ECS Fargate task termination detection Event Rule.",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-ecs-fargate-task-termination-detection-event-rule.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_ecs_fargate_task_termination_detection_event_rule",
         "gammarer.aws_ecs_fargate_task_termination_detection_event_rule._jsii"
     ],
     "package_data": {
         "gammarer.aws_ecs_fargate_task_termination_detection_event_rule._jsii": [
-            "aws-ecs-fargate-task-termination-detection-event-rule@0.4.3.jsii.tgz"
+            "aws-ecs-fargate-task-termination-detection-event-rule@0.4.5.jsii.tgz"
         ],
         "gammarer.aws_ecs_fargate_task_termination_detection_event_rule": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/__init__.py` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/aws-ecs-fargate-task-termination-detection-event-rule@0.4.3.jsii.tgz` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/aws-ecs-fargate-task-termination-detection-event-rule@0.4.5.jsii.tgz`

 * *Files 24% similar despite different names*

#### Comparing `aws-ecs-fargate-task-termination-detection-event-rule@0.4.3.jsii.tgz-content` & `aws-ecs-fargate-task-termination-detection-event-rule@0.4.5.jsii.tgz-content`

##### package/.jsii

###### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'fingerprint'": "'XBXBeyb0KdqUd2lCUrLzwTLdgBcuLBItcGr1v6YEKt0='", "'version'": "'0.4.5'"}*

```diff
@@ -3304,15 +3304,15 @@
             }
         }
     },
     "description": "This an AWS ECS Fargate task termination detection Event Rule.",
     "docs": {
         "stability": "stable"
     },
-    "fingerprint": "yAm/C8AkqiE6wu7teiyvra2u2w5QvDZuKSr0TMHd/uo=",
+    "fingerprint": "XBXBeyb0KdqUd2lCUrLzwTLdgBcuLBItcGr1v6YEKt0=",
     "homepage": "https://github.com/yicr/aws-ecs-fargate-task-termination-detection-event-rule.git",
     "jsiiVersion": "1.85.0 (build 08ee592)",
     "keywords": [
         "aws",
         "aws-cdk",
         "cdk",
         "ecs",
@@ -3453,9 +3453,9 @@
                         "primitive": "string"
                     }
                 }
             ],
             "symbolId": "src/index:EcsFargateTaskTerminationDetectionEventRuleProps"
         }
     },
-    "version": "0.4.3"
+    "version": "0.4.5"
 }
```

##### package/lib/index.js

###### js-beautify {}

```diff
@@ -32,10 +32,10 @@
         });
     }
 }
 exports.EcsFargateTaskTerminationDetectionEventRule = EcsFargateTaskTerminationDetectionEventRule;
 _a = JSII_RTTI_SYMBOL_1;
 EcsFargateTaskTerminationDetectionEventRule[_a] = {
     fqn: "@gammarer/aws-ecs-fargate-task-termination-detection-event-rule.EcsFargateTaskTerminationDetectionEventRule",
-    version: "0.4.3"
+    version: "0.4.5"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiaW5kZXguanMiLCJzb3VyY2VSb290IjoiIiwic291cmNlcyI6WyIuLi9zcmMvaW5kZXgudHMiXSwibmFtZXMiOltdLCJtYXBwaW5ncyI6Ijs7Ozs7QUFBQSxpREFBaUQ7QUFTakQsTUFBYSwyQ0FBNEMsU0FBUSxNQUFNLENBQUMsSUFBSTtJQUUxRSxZQUFZLEtBQWdCLEVBQUUsRUFBVSxFQUFFLEtBQXVEO1FBQy9GLEtBQUssQ0FBQyxLQUFLLEVBQUUsRUFBRSxFQUFFO1lBQ2YsUUFBUSxFQUFFLEtBQUssQ0FBQyxRQUFRO1lBQ3hCLFdBQVcsRUFBRSxLQUFLLENBQUMsV0FBVztZQUM5QixZQUFZLEVBQUU7Z0JBQ1osTUFBTSxFQUFFLENBQUMsU0FBUyxDQUFDO2dCQUNuQixVQUFVLEVBQUUsQ0FBQyx1QkFBdUIsQ0FBQztnQkFDckMsTUFBTSxFQUFFO29CQUNOLFVBQVUsRUFBRSxLQUFLLENBQUMsVUFBVTtvQkFDNUIsVUFBVSxFQUFFO3dCQUNWLFFBQVEsRUFBRTs0QkFDUixFQUFFLGNBQWMsRUFBRSxDQUFDLEVBQUU7eUJBQ3RCO3FCQUNGO29CQUNELFVBQVUsRUFBRSxDQUFDLFNBQVMsQ0FBQztvQkFDdkIsYUFBYSxFQUFFO3dCQUNiOzRCQUNFLGNBQWMsRUFBRSxFQUFFLE1BQU0sRUFBRSwrQkFBK0IsRUFBRTt5QkFDNUQ7cUJBQ0Y7aUJBQ0Y7YUFDRjtTQUNGLENBQUMsQ0FBQztJQUNMLENBQUM7O0FBekJILGtHQTBCQyIsInNvdXJjZXNDb250ZW50IjpbImltcG9ydCAqIGFzIGV2ZW50cyBmcm9tICdhd3MtY2RrLWxpYi9hd3MtZXZlbnRzJztcbmltcG9ydCB7IENvbnN0cnVjdCB9IGZyb20gJ2NvbnN0cnVjdHMnO1xuXG5leHBvcnQgaW50ZXJmYWNlIEVjc0ZhcmdhdGVUYXNrVGVybWluYXRpb25EZXRlY3Rpb25FdmVudFJ1bGVQcm9wcyB7XG4gIHJlYWRvbmx5IHJ1bGVOYW1lPzogc3RyaW5nO1xuICByZWFkb25seSBkZXNjcmlwdGlvbj86IHN0cmluZztcbiAgcmVhZG9ubHkgY2x1c3RlckFybjogc3RyaW5nO1xufVxuXG5leHBvcnQgY2xhc3MgRWNzRmFyZ2F0ZVRhc2tUZXJtaW5hdGlvbkRldGVjdGlvbkV2ZW50UnVsZSBleHRlbmRzIGV2ZW50cy5SdWxlIHtcblxuICBjb25zdHJ1Y3RvcihzY29wZTogQ29uc3RydWN0LCBpZDogc3RyaW5nLCBwcm9wczogRWNzRmFyZ2F0ZVRhc2tUZXJtaW5hdGlvbkRldGVjdGlvbkV2ZW50UnVsZVByb3BzKSB7XG4gICAgc3VwZXIoc2NvcGUsIGlkLCB7XG4gICAgICBydWxlTmFtZTogcHJvcHMucnVsZU5hbWUsXG4gICAgICBkZXNjcmlwdGlvbjogcHJvcHMuZGVzY3JpcHRpb24sXG4gICAgICBldmVudFBhdHRlcm46IHtcbiAgICAgICAgc291cmNlOiBbJ2F3cy5lY3MnXSxcbiAgICAgICAgZGV0YWlsVHlwZTogWydFQ1MgVGFzayBTdGF0ZSBDaGFuZ2UnXSxcbiAgICAgICAgZGV0YWlsOiB7XG4gICAgICAgICAgY2x1c3RlckFybjogcHJvcHMuY2x1c3RlckFybixcbiAgICAgICAgICBjb250YWluZXJzOiB7XG4gICAgICAgICAgICBleGl0Q29kZTogW1xuICAgICAgICAgICAgICB7ICdhbnl0aGluZy1idXQnOiAwIH0sXG4gICAgICAgICAgICBdLFxuICAgICAgICAgIH0sXG4gICAgICAgICAgbGFzdFN0YXR1czogWydTVE9QUEVEJ10sXG4gICAgICAgICAgc3RvcHBlZFJlYXNvbjogW1xuICAgICAgICAgICAge1xuICAgICAgICAgICAgICAnYW55dGhpbmctYnV0JzogeyBwcmVmaXg6ICdTY2FsaW5nIGFjdGl2aXR5IGluaXRpYXRlZCBieScgfSxcbiAgICAgICAgICAgIH0sXG4gICAgICAgICAgXSxcbiAgICAgICAgfSxcbiAgICAgIH0sXG4gICAgfSk7XG4gIH1cbn0iXX0=
```

##### package/package.json

###### Pretty-printed

 * *Similarity: 0.9731121281464531%*

 * *Differences: {"'devDependencies'": "{'projen': '^0.71.150'}", "'version'": "'0.4.5'"}*

```diff
@@ -21,15 +21,15 @@
         "jest-junit": "^15",
         "jsii": "1.x",
         "jsii-diff": "^1.85.0",
         "jsii-docgen": "^7.2.9",
         "jsii-pacmak": "^1.85.0",
         "jsii-rosetta": "1.x",
         "npm-check-updates": "^16",
-        "projen": "^0.71.148",
+        "projen": "^0.71.150",
         "standard-version": "^9",
         "ts-jest": "^27",
         "ts-node": "^10.9.1",
         "typescript": "^4.9.5"
     },
     "engines": {
         "node": ">= 16.0.0"
@@ -137,9 +137,9 @@
         "test:watch": "npx projen test:watch",
         "unbump": "npx projen unbump",
         "upgrade": "npx projen upgrade",
         "watch": "npx projen watch"
     },
     "stability": "stable",
     "types": "lib/index.d.ts",
-    "version": "0.4.3"
+    "version": "0.4.5"
 }
```

### Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/PKG-INFO` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-ecs-fargate-task-termination-detection-event-rule
-Version: 0.4.3
+Version: 0.4.5
 Summary: This an AWS ECS Fargate task termination detection Event Rule.
 Home-page: https://github.com/yicr/aws-ecs-fargate-task-termination-detection-event-rule.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-ecs-fargate-task-termination-detection-event-rule.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.3/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/SOURCES.txt` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/SOURCES.txt
 src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/dependency_links.txt
 src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/requires.txt
 src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/top_level.txt
 src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/__init__.py
 src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/py.typed
 src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/__init__.py
-src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/aws-ecs-fargate-task-termination-detection-event-rule@0.4.3.jsii.tgz
+src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/aws-ecs-fargate-task-termination-detection-event-rule@0.4.5.jsii.tgz
```

