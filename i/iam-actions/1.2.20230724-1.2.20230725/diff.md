# Comparing `tmp/iam_actions-1.2.20230724.tar.gz` & `tmp/iam_actions-1.2.20230725.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230724.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230725.tar", max compression
```

## Comparing `iam_actions-1.2.20230724.tar` & `iam_actions-1.2.20230725.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-07-24 02:29:51.142695 iam_actions-1.2.20230724/LICENSE
--rw-r--r--   0        0        0     2302 2023-07-24 02:29:51.142695 iam_actions-1.2.20230724/README.md
--rw-r--r--   0        0        0      228 2023-07-24 02:29:51.142695 iam_actions-1.2.20230724/iam_actions/__init__.py
--rw-r--r--   0        0        0  4374831 2023-07-24 02:31:30.946953 iam_actions-1.2.20230724/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-07-24 02:29:51.142695 iam_actions-1.2.20230724/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-07-24 02:29:51.142695 iam_actions-1.2.20230724/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-07-24 02:29:51.142695 iam_actions-1.2.20230724/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-07-24 02:29:51.142695 iam_actions-1.2.20230724/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-07-24 02:29:51.142695 iam_actions-1.2.20230724/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-07-24 02:29:51.142695 iam_actions-1.2.20230724/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-07-24 02:29:51.142695 iam_actions-1.2.20230724/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-07-24 02:29:51.142695 iam_actions-1.2.20230724/iam_actions/generate/services.py
--rw-r--r--   0        0        0   562970 2023-07-24 02:31:30.946953 iam_actions-1.2.20230724/iam_actions/policies.json
--rw-r--r--   0        0        0   197464 2023-07-24 02:31:30.946953 iam_actions-1.2.20230724/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   546046 2023-07-24 02:31:30.946953 iam_actions-1.2.20230724/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-07-24 02:31:31.722955 iam_actions-1.2.20230724/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230724/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230724/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-25 02:40:43.508074 iam_actions-1.2.20230725/LICENSE
+-rw-r--r--   0        0        0     2302 2023-07-25 02:40:43.508074 iam_actions-1.2.20230725/README.md
+-rw-r--r--   0        0        0      228 2023-07-25 02:40:43.508074 iam_actions-1.2.20230725/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4375008 2023-07-25 02:42:07.572322 iam_actions-1.2.20230725/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-07-25 02:40:43.508074 iam_actions-1.2.20230725/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-07-25 02:40:43.508074 iam_actions-1.2.20230725/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-07-25 02:40:43.508074 iam_actions-1.2.20230725/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-07-25 02:40:43.508074 iam_actions-1.2.20230725/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-07-25 02:40:43.508074 iam_actions-1.2.20230725/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-07-25 02:40:43.508074 iam_actions-1.2.20230725/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-07-25 02:40:43.508074 iam_actions-1.2.20230725/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-07-25 02:40:43.508074 iam_actions-1.2.20230725/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   563046 2023-07-25 02:42:07.572322 iam_actions-1.2.20230725/iam_actions/policies.json
+-rw-r--r--   0        0        0   197464 2023-07-25 02:42:07.572322 iam_actions-1.2.20230725/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   546095 2023-07-25 02:42:07.572322 iam_actions-1.2.20230725/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-07-25 02:42:08.340324 iam_actions-1.2.20230725/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230725/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230725/PKG-INFO
```

### Comparing `iam_actions-1.2.20230724/LICENSE` & `iam_actions-1.2.20230725/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230724/README.md` & `iam_actions-1.2.20230725/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230724/iam_actions/actions.json` & `iam_actions-1.2.20230725/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999801922395279%*

 * *Differences: {"'personalize'": "{'UpdateDataset': OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *                  "'UpdateDataset'), ('condition_keys', []), ('description', 'Not Documented by "*

 * *                  "AWS'), ('orphan', False), ('resources', [])])}",*

 * * "'rekognition'": "{'ListCollections': {'resources': []}}"}*

```diff
@@ -108934,14 +108934,22 @@
             "condition_keys": [],
             "description": "Grants permission to update a campaign",
             "orphan": false,
             "resources": [
                 "campaign"
             ]
         },
+        "UpdateDataset": {
+            "access_level": "Undocumented",
+            "action": "UpdateDataset",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateMetricAttribution": {
             "access_level": "Write",
             "action": "UpdateMetricAttribution",
             "condition_keys": [],
             "description": "Grants permission to update a metric attribution",
             "orphan": false,
             "resources": [
@@ -118525,17 +118533,15 @@
         },
         "ListCollections": {
             "access_level": "Read",
             "action": "ListCollections",
             "condition_keys": [],
             "description": "Grants permission to read the collection Id's in your account",
             "orphan": false,
-            "resources": [
-                "collection"
-            ]
+            "resources": []
         },
         "ListDatasetEntries": {
             "access_level": "Read",
             "action": "ListDatasetEntries",
             "condition_keys": [],
             "description": "Grants permission to list the dataset entries in an existing Amazon Rekognition Custom Labels dataset",
             "orphan": false,
```

### Comparing `iam_actions-1.2.20230724/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230725/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230724/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230725/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230724/iam_actions/generate/generate.py` & `iam_actions-1.2.20230725/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230724/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230725/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230724/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230725/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230724/iam_actions/generate/services.py` & `iam_actions-1.2.20230725/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230724/iam_actions/policies.json` & `iam_actions-1.2.20230725/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999780031995347%*

 * *Differences: {"'serviceMap'": "{'AWS Identity Store': {'conditionKeys': ['identitystore:UserId']}, 'Amazon "*

 * *                 "Personalize': {'Actions': {insert: [(69, 'UpdateDataset')]}}}"}*

```diff
@@ -4807,15 +4807,18 @@
                 "ListGroupMembershipsForMember",
                 "ListGroups",
                 "ListUsers",
                 "UpdateGroup",
                 "UpdateUser"
             ],
             "HasResource": true,
-            "StringPrefix": "identitystore"
+            "StringPrefix": "identitystore",
+            "conditionKeys": [
+                "identitystore:UserId"
+            ]
         },
         "AWS Identity Store Auth": {
             "ARNFormat": "arn:${Partition}:identitystore-auth:${Region}:${Account}:${RelativeId}",
             "ARNRegex": "^arn:${Partition}:identitystore-auth:${Region}:.+",
             "Actions": [
                 "BatchDeleteSession",
                 "BatchGetSession",
@@ -16777,14 +16780,15 @@
                 "PutUsers",
                 "StartRecommender",
                 "StopRecommender",
                 "StopSolutionVersionCreation",
                 "TagResource",
                 "UntagResource",
                 "UpdateCampaign",
+                "UpdateDataset",
                 "UpdateMetricAttribution",
                 "UpdateRecommender"
             ],
             "HasResource": true,
             "StringPrefix": "personalize"
         },
         "Amazon Pinpoint": {
```

### Comparing `iam_actions-1.2.20230724/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230725/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230724/iam_actions/services.json` & `iam_actions-1.2.20230725/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998842592592594%*

 * *Differences: {"'identitystore'": "{'ConditionKeys': ['identitystore:UserId']}",*

 * * "'personalize'": "{'Actions': {insert: [(69, 'UpdateDataset')]}}"}*

```diff
@@ -10206,15 +10206,17 @@
             "ListGroupMemberships",
             "ListGroupMembershipsForMember",
             "ListGroups",
             "ListUsers",
             "UpdateGroup",
             "UpdateUser"
         ],
-        "ConditionKeys": [],
+        "ConditionKeys": [
+            "identitystore:UserId"
+        ],
         "HasResource": true,
         "ServiceNames": [
             "AWS Identity Store"
         ]
     },
     "identitystore-auth": {
         "ARNFormats": [
@@ -15304,14 +15306,15 @@
             "PutUsers",
             "StartRecommender",
             "StopRecommender",
             "StopSolutionVersionCreation",
             "TagResource",
             "UntagResource",
             "UpdateCampaign",
+            "UpdateDataset",
             "UpdateMetricAttribution",
             "UpdateRecommender"
         ],
         "ConditionKeys": [],
         "HasResource": true,
         "ServiceNames": [
             "Amazon Personalize"
```

### Comparing `iam_actions-1.2.20230724/pyproject.toml` & `iam_actions-1.2.20230725/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230724"
+version = "1.2.20230725"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230724/setup.py` & `iam_actions-1.2.20230725/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230724',
+    'version': '1.2.20230725',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230724/PKG-INFO` & `iam_actions-1.2.20230725/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230724
+Version: 1.2.20230725
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

