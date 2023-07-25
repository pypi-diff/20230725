# Comparing `tmp/policyuniverse-1.5.1.20230703.tar.gz` & `tmp/policyuniverse-1.5.1.20230725.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "policyuniverse-1.5.1.20230703.tar", last modified: Mon Jul  3 18:22:09 2023, max compression
+gzip compressed data, was "policyuniverse-1.5.1.20230725.tar", last modified: Tue Jul 25 21:24:57 2023, max compression
```

## Comparing `policyuniverse-1.5.1.20230703.tar` & `policyuniverse-1.5.1.20230725.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:22:09.007771 policyuniverse-1.5.1.20230703/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 18:22:00.000000 policyuniverse-1.5.1.20230703/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-03 18:22:00.000000 policyuniverse-1.5.1.20230703/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-07-03 18:22:09.007771 policyuniverse-1.5.1.20230703/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-07-03 18:22:00.000000 policyuniverse-1.5.1.20230703/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:22:09.007771 policyuniverse-1.5.1.20230703/policyuniverse/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-03 18:22:00.000000 policyuniverse-1.5.1.20230703/policyuniverse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-03 18:22:00.000000 policyuniverse-1.5.1.20230703/policyuniverse/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-03 18:22:00.000000 policyuniverse-1.5.1.20230703/policyuniverse/action_categories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-03 18:22:00.000000 policyuniverse-1.5.1.20230703/policyuniverse/arn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-03 18:22:00.000000 policyuniverse-1.5.1.20230703/policyuniverse/common.py
--rw-r--r--   0 runner    (1001) docker     (123)  7970603 2023-07-03 18:22:00.000000 policyuniverse-1.5.1.20230703/policyuniverse/data.json
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-07-03 18:22:00.000000 policyuniverse-1.5.1.20230703/policyuniverse/expander_minimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-03 18:22:00.000000 policyuniverse-1.5.1.20230703/policyuniverse/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-03 18:22:00.000000 policyuniverse-1.5.1.20230703/policyuniverse/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-07-03 18:22:00.000000 policyuniverse-1.5.1.20230703/policyuniverse/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:22:09.007771 policyuniverse-1.5.1.20230703/policyuniverse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-07-03 18:22:08.000000 policyuniverse-1.5.1.20230703/policyuniverse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-03 18:22:08.000000 policyuniverse-1.5.1.20230703/policyuniverse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 18:22:08.000000 policyuniverse-1.5.1.20230703/policyuniverse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 18:22:08.000000 policyuniverse-1.5.1.20230703/policyuniverse.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-03 18:22:08.000000 policyuniverse-1.5.1.20230703/policyuniverse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 18:22:08.000000 policyuniverse-1.5.1.20230703/policyuniverse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-03 18:22:09.011771 policyuniverse-1.5.1.20230703/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-03 18:22:00.000000 policyuniverse-1.5.1.20230703/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:24:57.821473 policyuniverse-1.5.1.20230725/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 21:24:42.000000 policyuniverse-1.5.1.20230725/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-25 21:24:42.000000 policyuniverse-1.5.1.20230725/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-07-25 21:24:57.821473 policyuniverse-1.5.1.20230725/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-07-25 21:24:42.000000 policyuniverse-1.5.1.20230725/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:24:57.821473 policyuniverse-1.5.1.20230725/policyuniverse/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-25 21:24:42.000000 policyuniverse-1.5.1.20230725/policyuniverse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-25 21:24:42.000000 policyuniverse-1.5.1.20230725/policyuniverse/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-25 21:24:42.000000 policyuniverse-1.5.1.20230725/policyuniverse/action_categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-25 21:24:42.000000 policyuniverse-1.5.1.20230725/policyuniverse/arn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-25 21:24:42.000000 policyuniverse-1.5.1.20230725/policyuniverse/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)  7997855 2023-07-25 21:24:42.000000 policyuniverse-1.5.1.20230725/policyuniverse/data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-07-25 21:24:42.000000 policyuniverse-1.5.1.20230725/policyuniverse/expander_minimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-25 21:24:42.000000 policyuniverse-1.5.1.20230725/policyuniverse/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-25 21:24:42.000000 policyuniverse-1.5.1.20230725/policyuniverse/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-07-25 21:24:42.000000 policyuniverse-1.5.1.20230725/policyuniverse/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:24:57.821473 policyuniverse-1.5.1.20230725/policyuniverse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-07-25 21:24:57.000000 policyuniverse-1.5.1.20230725/policyuniverse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-25 21:24:57.000000 policyuniverse-1.5.1.20230725/policyuniverse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 21:24:57.000000 policyuniverse-1.5.1.20230725/policyuniverse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 21:24:57.000000 policyuniverse-1.5.1.20230725/policyuniverse.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-25 21:24:57.000000 policyuniverse-1.5.1.20230725/policyuniverse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-25 21:24:57.000000 policyuniverse-1.5.1.20230725/policyuniverse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-25 21:24:57.821473 policyuniverse-1.5.1.20230725/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-25 21:24:42.000000 policyuniverse-1.5.1.20230725/setup.py
```

### Comparing `policyuniverse-1.5.1.20230703/LICENSE` & `policyuniverse-1.5.1.20230725/LICENSE`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230703/PKG-INFO` & `policyuniverse-1.5.1.20230725/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: policyuniverse
-Version: 1.5.1.20230703
+Version: 1.5.1.20230725
 Summary: Parse and Process AWS IAM Policies, Statements, ARNs, and wildcards.
 Home-page: https://github.com/Netflix-Skunkworks/policyuniverse
 Author: Patrick Kelley
 Author-email: patrickbarrettkelley@gmail.com
 Keywords: iam,arn,action_groups,condition,policy,statement,wildcard
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
```

### Comparing `policyuniverse-1.5.1.20230703/README.md` & `policyuniverse-1.5.1.20230725/README.md`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230703/policyuniverse/__init__.py` & `policyuniverse-1.5.1.20230725/policyuniverse/__init__.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230703/policyuniverse/action.py` & `policyuniverse-1.5.1.20230725/policyuniverse/action.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230703/policyuniverse/action_categories.py` & `policyuniverse-1.5.1.20230725/policyuniverse/action_categories.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230703/policyuniverse/arn.py` & `policyuniverse-1.5.1.20230725/policyuniverse/arn.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230703/policyuniverse/common.py` & `policyuniverse-1.5.1.20230725/policyuniverse/common.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230703/policyuniverse/data.json` & `policyuniverse-1.5.1.20230725/policyuniverse/data.json`

 * *Files 0% similar despite different names*

```diff
@@ -7128,15 +7128,15 @@
       },
       "ConnectAppAuthorization": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "Grants permission to connect application authorizations",
+        "description": "Grants permission to connect app authorizations",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_ConnectAppAuthorization.html"
         }
       },
       "CreateAppAuthorization": {
@@ -7144,15 +7144,15 @@
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:RequestTag/${TagKey}",
           "aws:TagKeys"
         ],
-        "description": "Grants permission to create application authorizations for application bundles",
+        "description": "Grants permission to create app authorizations for app bundles",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_CreateAppAuthorization.html"
         }
       },
       "CreateAppBundle": {
@@ -7160,15 +7160,15 @@
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:RequestTag/${TagKey}",
           "aws:TagKeys"
         ],
-        "description": "Grants permission to create application bundles in your account",
+        "description": "Grants permission to create app bundles in your account",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_CreateAppBundle.html"
         }
       },
       "CreateIngestion": {
@@ -7176,15 +7176,15 @@
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:RequestTag/${TagKey}",
           "aws:TagKeys"
         ],
-        "description": "Grants permission to create ingestions for application bundles",
+        "description": "Grants permission to create ingestions for app bundles",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_CreateIngestion.html"
         }
       },
       "CreateIngestionDestination": {
@@ -7192,54 +7192,54 @@
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:RequestTag/${TagKey}",
           "aws:TagKeys"
         ],
-        "description": "Grants permission to create ingestion destinations for application bundles",
+        "description": "Grants permission to create ingestion destinations for app bundles",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_CreateIngestionDestination.html"
         }
       },
       "DeleteAppAuthorization": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "Grants permission to delete application authorizations within an application bundle",
+        "description": "Grants permission to delete app authorizations within an app bundle",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_DeleteAppAuthorization.html"
         }
       },
       "DeleteAppBundle": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "Grants permission to delete application bundles in your account",
+        "description": "Grants permission to delete app bundles in your account",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_DeleteAppBundle.html"
         }
       },
       "DeleteIngestion": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
-        "description": "Grants permission to delete ingestions within an application bundle",
+        "description": "Grants permission to delete ingestions within an app bundle",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_DeleteIngestion.html"
         }
       },
       "DeleteIngestionDestination": {
@@ -7260,15 +7260,15 @@
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [
           "aws:ResourceTag/${TagKey}"
         ],
-        "description": "Grants permission to view details about application authorizations",
+        "description": "Grants permission to view details about app authorizations",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_GetAppAuthorization.html"
         }
       },
       "GetAppBundle": {
@@ -7276,15 +7276,15 @@
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [
           "aws:ResourceTag/${TagKey}"
         ],
-        "description": "Grants permission to view details about application bundles",
+        "description": "Grants permission to view details about app bundles",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_GetAppBundle.html"
         }
       },
       "GetIngestion": {
@@ -7323,30 +7323,30 @@
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
-        "description": "Grants permission to retrieve a list of application authorizations within an application bundle",
+        "description": "Grants permission to retrieve a list of app authorizations within an app bundle",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_ListAppAuthorizations.html"
         }
       },
       "ListAppBundles": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
-        "description": "Grants permission to retrieve a list of application bundles in your account",
+        "description": "Grants permission to retrieve a list of app bundles in your account",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_ListAppBundles.html"
         }
       },
       "ListIngestionDestinations": {
@@ -7368,29 +7368,29 @@
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
-        "description": "Grants permission to retrieve a list of ingestions within an application bundle",
+        "description": "Grants permission to retrieve a list of ingestions within an app bundle",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_ListIngestions.html"
         }
       },
       "ListTagsForResource": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
-        "description": "Grants permission to list tags for AppFabric resouces",
+        "description": "Grants permission to list tags for AppFabric resources",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_ListTagsForResource.html"
         }
       },
       "StartIngestion": {
@@ -7470,15 +7470,15 @@
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:ResourceTag/${TagKey}"
         ],
-        "description": "Grants permission to update application authorizations within application bundles",
+        "description": "Grants permission to update app authorizations within app bundles",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/appfabric/latest/api/API_UpdateAppAuthorization.html"
         }
       },
       "UpdateIngestionDestination": {
@@ -15184,14 +15184,278 @@
       "api_reference_doc_page": "https://docs.aws.amazon.com/batch/latest/APIReference/",
       "authz_doc_page": "https://docs.aws.amazon.com/batch/latest/userguide/IAM_policies.html",
       "concepts_doc_root": "https://docs.aws.amazon.com/batch/latest/userguide/",
       "context_keys_doc_root": "https://docs.aws.amazon.com/service-authorization/latest/reference/list_awsbatch.html#"
     },
     "prefix": "batch"
   },
+  "Bedrock": {
+    "actions": {
+      "CreateModelCustomizationJob": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:ResourceTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to create a job for customizing the model with your custom training data",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/bedrock/latest/APIReference/API_CreateModelCustomizationJob.html"
+        }
+      },
+      "DeleteCustomModel": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete a custom model that you created earlier",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/bedrock/latest/APIReference/API_DeleteCustomModel.html"
+        }
+      },
+      "DeletePrompt": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete a saved prompt",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/bedrock/latest/APIReference/API_DeletePrompt.html"
+        }
+      },
+      "GetCustomModel": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to get the properties associated with a Bedrock custom model that you have created",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/bedrock/latest/APIReference/API_GetCustomModel.html"
+        }
+      },
+      "GetModelCustomizationJob": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to get the properties associated with a model-customization job. Use this operation to get the status of a model-customization job",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/bedrock/latest/APIReference/API_GetModelCustomizationJob.html"
+        }
+      },
+      "GetPrompt": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to get a saved prompt",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/bedrock/latest/APIReference/API_GetPrompt.html"
+        }
+      },
+      "InvokeModel": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to invoke the specified Bedrock model to run inference using the input provided in the request body",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/bedrock/latest/APIReference/API_InvokeModel.html"
+        }
+      },
+      "InvokeModelWithResponseStream": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to invoke the specified Bedrock model to run inference using the input provided in the request body with streaming response",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/bedrock/latest/APIReference/API_InvokeModelWithResponseStream.html"
+        }
+      },
+      "ListCustomModels": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to get a list of Bedrock custom models that you have created",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/bedrock/latest/APIReference/API_ListCustomModels.html"
+        }
+      },
+      "ListFoundationModels": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list Bedrock foundation models that you can use",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/bedrock/latest/APIReference/API_ListFoundationModels.html"
+        }
+      },
+      "ListModelCustomizationJobs": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to get the list of model customization jobs that you have submitted",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/bedrock/latest/APIReference/API_ListModelCustomizationJobs.html"
+        }
+      },
+      "ListPrompts": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to lists all prompts saved to a playground",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/bedrock/latest/APIReference/API_ListPrompts.html"
+        }
+      },
+      "ListTagsForResource": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list tags for a Bedrock resource",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/bedrock/latest/APIReference/API_ListTagsForResource.html"
+        }
+      },
+      "StopModelCustomizationJob": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to stop a Bedrock model customization job while in progress. This is an asynchronous operation, \\n you need to call GetModelCustomizationJob API to get the status of model-customization job. \\n If the job state is IN_PROGRESS the job is marked for termination and put into the STOPPING state. \\n If the job completes before it can be stopped, it is put into the COMPLETED state. \\n otherwise the job is stopped and put into the STOPPED state",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/bedrock/latest/APIReference/API_StopModelCustomizationJob.html"
+        }
+      },
+      "TagResource": {
+        "aws_action_groups": [
+          "Tagging",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Tagging",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:ResourceTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to Tag a Bedrock resource",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/bedrock/latest/APIReference/API_TagResource.html"
+        }
+      },
+      "UntagResource": {
+        "aws_action_groups": [
+          "Tagging",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Tagging",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to Untag a Bedrock resource",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/bedrock/latest/APIReference/API_UntagResource.html"
+        }
+      },
+      "UpdatePrompt": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to updates a saved prompt",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/bedrock/latest/APIReference/API_UpdatePrompt.html"
+        }
+      }
+    },
+    "arn_format": "arn:${Partition}:bedrock:${Region}:${Account}:${ResourceType}/${ResourceId}",
+    "arn_regex": "^arn:${Partition}:bedrock:.*:.*:.+",
+    "description": "Amazon Bedrock",
+    "docs": {
+      "actions_doc_root": "https://docs.aws.amazon.com/bedrock/latest/APIReference/",
+      "api_detail_root": "",
+      "api_doc_root": "",
+      "api_reference_doc_page": "https://docs.aws.amazon.com/bedrock/latest/APIReference/",
+      "authz_doc_page": "https://docs.aws.amazon.com/bedrock/latest/APIReference/welcome.html",
+      "concepts_doc_root": "https://docs.aws.amazon.com/bedrock/latest/APIReference/",
+      "context_keys_doc_root": "https://docs.aws.amazon.com/bedrock/latest/APIReference/"
+    },
+    "prefix": "bedrock"
+  },
   "Billing": {
     "actions": {
       "GetBillingData": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
@@ -23303,15 +23567,15 @@
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com//cloud-map/latest/api/API_UpdateService.html"
         }
       }
     },
-    "arn_format": "arn:${Partition}:servicediscovery:${Region}:${AccountId}:${ResourceType}/${ResourceName}",
+    "arn_format": "arn:${Partition}:servicediscovery:${Region}:${Account}:${ResourceType}/${ResourceName}",
     "arn_regex": "^arn:${Partition}:servicediscovery:.+",
     "description": "AWS Cloud Map",
     "docs": {
       "actions_doc_root": "https://docs.aws.amazon.com//cloud-map/latest/api/",
       "api_detail_root": "",
       "api_doc_root": "",
       "api_reference_doc_page": "https://docs.aws.amazon.com//cloud-map/latest/api/Welcome.html",
@@ -35611,178 +35875,178 @@
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to batch retrieve specific findings generated by CodeGuru Security",
         "docs": {
           "api_doc": "",
-          "doc_page": "${APIReferenceDocPage}",
-          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-ug/permissions-reference.html"
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-api/API_BatchGetFindings.html"
         }
       },
       "CreateScan": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:RequestTag/${TagKey}",
           "aws:TagKeys"
         ],
         "description": "Grants permission to create a CodeGuru Security scan",
         "docs": {
           "api_doc": "",
-          "doc_page": "${APIReferenceDocPage}",
-          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-ug/permissions-reference.html"
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-api/API_CreateScan.html"
         }
       },
       "CreateUploadUrl": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to generate a presigned url for uploading code archives",
         "docs": {
           "api_doc": "",
-          "doc_page": "${APIReferenceDocPage}",
-          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-ug/permissions-reference.html"
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-api/API_CreateUploadUrl.html"
         }
       },
       "DeleteScansByCategory": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to delete all the scans and related findings from CodeGuru Security by given category",
         "docs": {
           "api_doc": "",
-          "doc_page": "${APIReferenceDocPage}",
+          "doc_page": "${AuthZDocPage}",
           "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-ug/permissions-reference.html"
         }
       },
       "GetAccountConfiguration": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to retrieve the account level configurations",
         "docs": {
           "api_doc": "",
-          "doc_page": "${APIReferenceDocPage}",
-          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-ug/permissions-reference.html"
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-api/API_GetAccountConfiguration.html"
         }
       },
       "GetFindings": {
         "aws_action_groups": [
           "ReadOnly",
           "ListOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to retrieve findings for a scan generated by CodeGuru Security",
         "docs": {
           "api_doc": "",
-          "doc_page": "${APIReferenceDocPage}",
-          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-ug/permissions-reference.html"
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-api/API_GetFindings.html"
         }
       },
       "GetMetricsSummary": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to retrieve AWS accout level metrics summary generated by CodeGuru Security",
         "docs": {
           "api_doc": "",
-          "doc_page": "${APIReferenceDocPage}",
-          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-ug/permissions-reference.html"
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-api/API_GetMetricsSummary.html"
         }
       },
       "GetScan": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [
           "aws:ResourceTag/${TagKey}"
         ],
         "description": "Grants permission to retrieve CodeGuru Security scan metadata",
         "docs": {
           "api_doc": "",
-          "doc_page": "${APIReferenceDocPage}",
-          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-ug/permissions-reference.html"
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-api/API_GetScan.html"
         }
       },
       "ListFindings": {
         "aws_action_groups": [
           "ReadOnly",
           "ListOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to retrieve findings generated by CodeGuru Security",
         "docs": {
           "api_doc": "",
-          "doc_page": "${APIReferenceDocPage}",
+          "doc_page": "${AuthZDocPage}",
           "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-ug/permissions-reference.html"
         }
       },
       "ListFindingsMetrics": {
         "aws_action_groups": [
           "ReadOnly",
           "ListOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to retrieve a list of account level findings metrics within a date range",
         "docs": {
           "api_doc": "",
-          "doc_page": "${APIReferenceDocPage}",
-          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-ug/permissions-reference.html"
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-api/API_ListFindingsMetrics.html"
         }
       },
       "ListScans": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite",
           "ListOnly"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to retrieve list of CodeGuru Security scan metadata",
         "docs": {
           "api_doc": "",
-          "doc_page": "${APIReferenceDocPage}",
-          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-ug/permissions-reference.html"
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-api/API_ListScans.html"
         }
       },
       "ListTagsForResource": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [
           "aws:ResourceTag/${TagKey}"
         ],
         "description": "Grants permission to retrieve a list of tags for a scan name ARN",
         "docs": {
           "api_doc": "",
-          "doc_page": "${APIReferenceDocPage}",
-          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-ug/permissions-reference.html"
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-api/API_ListTagsForResource.html"
         }
       },
       "TagResource": {
         "aws_action_groups": [
           "ReadWrite",
           "Tagging"
         ],
@@ -35790,59 +36054,59 @@
         "condition_keys": [
           "aws:RequestTag/${TagKey}",
           "aws:TagKeys"
         ],
         "description": "Grants permission to add tags to a scan name ARN",
         "docs": {
           "api_doc": "",
-          "doc_page": "${APIReferenceDocPage}",
-          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-ug/permissions-reference.html"
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-api/API_TagResource.html"
         }
       },
       "UntagResource": {
         "aws_action_groups": [
           "ReadWrite",
           "Tagging"
         ],
         "calculated_action_group": "Tagging",
         "condition_keys": [
           "aws:TagKeys"
         ],
         "description": "Grants permission to remove tags from a scan name ARN",
         "docs": {
           "api_doc": "",
-          "doc_page": "${APIReferenceDocPage}",
-          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-ug/permissions-reference.html"
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-api/API_UntagResource.html"
         }
       },
       "UpdateAccountConfiguration": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to update the account level configurations",
         "docs": {
           "api_doc": "",
-          "doc_page": "${APIReferenceDocPage}",
-          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-ug/permissions-reference.html"
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/codeguru/latest/security-api/API_UpdateAccountConfiguration.html"
         }
       }
     },
     "arn_format": "arn:${Partition}:codeguru-security:${Region}:${Account}:*",
     "arn_regex": "^arn:${Partition}:codeguru-security:.+:.+:.+",
     "description": "Amazon CodeGuru Security",
     "docs": {
-      "actions_doc_root": "https://docs.aws.amazon.com/codeguru/latest/security-ug/",
+      "actions_doc_root": "https://docs.aws.amazon.com/codeguru/latest/security-api/",
       "api_detail_root": "",
       "api_doc_root": "",
-      "api_reference_doc_page": "https://docs.aws.amazon.com/codeguru/latest/security-ug/permissions-reference.html",
-      "authz_doc_page": "https://docs.aws.amazon.com/codeguru/latest/security-ug/security-iam.html",
+      "api_reference_doc_page": "https://docs.aws.amazon.com/codeguru/latest/security-api/Welcome.html",
+      "authz_doc_page": "https://docs.aws.amazon.com/codeguru/latest/security-ug/permissions-reference.html",
       "concepts_doc_root": "https://docs.aws.amazon.com/codeguru/latest/security-ug/",
-      "context_keys_doc_root": "https://docs.aws.amazon.com/codeguru/latest/security-ug/security-iam.html"
+      "context_keys_doc_root": "https://docs.aws.amazon.com/codeguru/latest/security-ug/"
     },
     "prefix": "codeguru-security"
   },
   "CodePipeline": {
     "actions": {
       "AcknowledgeJob": {
         "aws_action_groups": [
@@ -43678,14 +43942,30 @@
         "description": "Grants permission to delete a prompt in an Amazon Connect instance",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/connect/latest/APIReference/API_DeletePrompt.html"
         }
       },
+      "DeleteQueue": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "connect:InstanceId"
+        ],
+        "description": "Grants permission to delete a queue in an Amazon Connect instance",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/connect/latest/APIReference/API_DeleteQueue.html"
+        }
+      },
       "DeleteQuickConnect": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:ResourceTag/${TagKey}",
@@ -43694,14 +43974,30 @@
         "description": "Grants permission to delete a quick connect in an Amazon Connect instance",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/connect/latest/APIReference/API_DeleteQuickConnect.html"
         }
       },
+      "DeleteRoutingProfile": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:ResourceTag/${TagKey}",
+          "connect:InstanceId"
+        ],
+        "description": "Grants permission to delete routing profiles in an Amazon Connect instance",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/connect/latest/APIReference/API_DeleteRoutingProfile.html"
+        }
+      },
       "DeleteRule": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
           "aws:ResourceTag/${TagKey}",
@@ -49672,15 +49968,15 @@
       "GetMetadataModel": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
-        "description": "Grants permission to list all of the AWS DMS attributes for a metadata model",
+        "description": "Grants permission to list all of the AWS DMS attributes for a metadata model. Note. Despite this action requires StartMetadataModelImport, the latter does not currently authorize the described Schema Conversion operation",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/Welcome.html"
         }
       },
       "ImportCertificate": {
@@ -49744,15 +50040,15 @@
       "ListMetadataModelAssessmentActionItems": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
-        "description": "Grants permission to list the AWS DMS attributes for a metadata model assessment action items",
+        "description": "Grants permission to list the AWS DMS attributes for a metadata model assessment action items. Note. Despite this action requires StartMetadataModelImport, the latter does not currently authorize the described Schema Conversion operation",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/Welcome.html"
         }
       },
       "ListMetadataModelAssessments": {
@@ -49800,15 +50096,15 @@
       "ListMigrationProjects": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
-        "description": "Grants permission to list the AWS DMS attributes for a migration projects",
+        "description": "Grants permission to list the AWS DMS attributes for a migration projects. Note. Despite this action requires DescribeMigrationProjects and DescribeConversionConfiguration, both required actions do not currently authorize the described Schema Conversion operation",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/dms/latest/APIReference/Welcome.html"
         }
       },
       "ListTagsForResource": {
@@ -59075,16 +59371,16 @@
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to authorize an application for your AWS Directory",
         "docs": {
           "api_doc": "",
-          "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/directoryservice/latest/devguide/"
+          "doc_page": "${DocHomeURL}directoryservice/latest/admin-guide/UsingWithDS_IAM_ResourcePermissions.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/directoryservice/latest/admin-guide/UsingWithDS_IAM_ResourcePermissions.html"
         }
       },
       "CancelSchemaExtension": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -59102,16 +59398,16 @@
           "ReadOnly"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to verify that the alias is available for use",
         "docs": {
           "api_doc": "",
-          "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/directoryservice/latest/devguide/"
+          "doc_page": "${DocHomeURL}directoryservice/latest/admin-guide/UsingWithDS_IAM_ResourcePermissions.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/directoryservice/latest/admin-guide/UsingWithDS_IAM_ResourcePermissions.html"
         }
       },
       "ConnectDirectory": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -59189,16 +59485,16 @@
         "condition_keys": [
           "aws:RequestTag/${TagKey}",
           "aws:TagKeys"
         ],
         "description": "Grants permission to create an IdentityPool Directory in the AWS cloud",
         "docs": {
           "api_doc": "",
-          "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/directoryservice/latest/devguide/"
+          "doc_page": "${DocHomeURL}directoryservice/latest/admin-guide/UsingWithDS_IAM_ResourcePermissions.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/directoryservice/latest/admin-guide/UsingWithDS_IAM_ResourcePermissions.html"
         }
       },
       "CreateLogSubscription": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -59310,15 +59606,15 @@
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to delete an existing trust relationship between your Microsoft AD in the AWS cloud and an external domain",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/directoryservice/latest/devguide/DeleteTrust.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/directoryservice/latest/devguide/API_DeleteTrust.html"
         }
       },
       "DeregisterCertificate": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -59636,16 +59932,16 @@
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to retrieve the details of the authorized applications on a directory",
         "docs": {
           "api_doc": "",
-          "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/directoryservice/latest/devguide/API_GetAuthorizedApplicationDetails.html"
+          "doc_page": "${DocHomeURL}directoryservice/latest/admin-guide/UsingWithDS_IAM_ResourcePermissions.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/directoryservice/latest/admin-guide/UsingWithDS_IAM_ResourcePermissions.html"
         }
       },
       "GetDirectoryLimits": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
@@ -59678,16 +59974,16 @@
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to obtain the AWS applications authorized for a directory",
         "docs": {
           "api_doc": "",
-          "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/directoryservice/latest/devguide/"
+          "doc_page": "${DocHomeURL}directoryservice/latest/admin-guide/UsingWithDS_IAM_ResourcePermissions.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/directoryservice/latest/admin-guide/UsingWithDS_IAM_ResourcePermissions.html"
         }
       },
       "ListCertificates": {
         "aws_action_groups": [
           "ListOnly",
           "ReadOnly",
           "ReadWrite"
@@ -59897,16 +60193,16 @@
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to unauthorize an application from your AWS Directory",
         "docs": {
           "api_doc": "",
-          "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/directoryservice/latest/devguide/"
+          "doc_page": "${DocHomeURL}directoryservice/latest/admin-guide/UsingWithDS_IAM_ResourcePermissions.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/directoryservice/latest/admin-guide/UsingWithDS_IAM_ResourcePermissions.html"
         }
       },
       "UnshareDirectory": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -59914,14 +60210,27 @@
         "description": "Grants permission to stop the directory sharing between the directory owner and consumer accounts",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/directoryservice/latest/devguide/API_UnshareDirectory.html"
         }
       },
+      "UpdateAuthorizedApplication": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to update an authorized application for your AWS Directory",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}directoryservice/latest/admin-guide/UsingWithDS_IAM_ResourcePermissions.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/directoryservice/latest/admin-guide/UsingWithDS_IAM_ResourcePermissions.html"
+        }
+      },
       "UpdateConditionalForwarder": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to update a conditional forwarder that has been set up for your AWS directory",
@@ -60014,16 +60323,16 @@
     "arn_format": "arn:${Partition}:ds:${Region}:${Account}:${RelativeId}",
     "arn_regex": "^arn:${Partition}:ds:.+",
     "description": "AWS Directory Service",
     "docs": {
       "actions_doc_root": "https://docs.aws.amazon.com/directoryservice/latest/devguide/",
       "api_detail_root": "",
       "api_doc_root": "",
-      "api_reference_doc_page": "https://docs.aws.amazon.com/directory-service/index.html",
-      "authz_doc_page": "https://docs.aws.amazon.com/directoryservice/latest/admin-guide/UsingWithDS_IAM_AuthNAccess.html",
+      "api_reference_doc_page": "https://docs.aws.amazon.com/directoryservice/latest/devguide/welcome.html",
+      "authz_doc_page": "https://docs.aws.amazon.com/directoryservice/latest/admin-guide/iam_auth_access.html",
       "concepts_doc_root": "https://docs.aws.amazon.com/directoryservice/latest/admin-guide/",
       "context_keys_doc_root": "https://docs.aws.amazon.com/directoryservice/latest/devguide/"
     },
     "prefix": "ds"
   },
   "DocumentDB Elastic Clusters": {
     "actions": {
@@ -81753,15 +82062,15 @@
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to delete event buses",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/eventbridge/latest/APIReference/API_DeletePartnerEventSource.html"
+          "doc_page_rel": "https://docs.aws.amazon.com/eventbridge/latest/APIReference/API_DeleteEventBus.html"
         }
       },
       "DeletePartnerEventSource": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -83636,14 +83945,27 @@
         "description": "Grants permission to associate DNS aliases with an Amazon FSx for Windows File Server file system",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/fsx/latest/APIReference/API_AssociateFileSystemAliases.html"
         }
       },
+      "BypassSnaplockEnterpriseRetention": {
+        "aws_action_groups": [
+          "Permissions"
+        ],
+        "calculated_action_group": "Permissions",
+        "condition_keys": [],
+        "description": "Grants permission to allow deletion of an FSx for ONTAP SnapLock Enterprise volume that contains WORM (write once, read many) files with active retention periods",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${DocHomeURL}fsx/latest/ONTAPGuide/snaplock-enterprise.html#bypass-enterprise",
+          "doc_page_rel": "https://docs.aws.amazon.com/fsx/latest/ONTAPGuide/snaplock-enterprise.html#bypass-enterprise"
+        }
+      },
       "CancelDataRepositoryTask": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to cancel a data repository task",
@@ -96173,14 +96495,290 @@
       "api_reference_doc_page": "https://docs.aws.amazon.com/health/latest/APIReference/",
       "authz_doc_page": "https://docs.aws.amazon.com/health/latest/ug/controlling-access.html",
       "concepts_doc_root": "https://docs.aws.amazon.com/health/latest/ug/",
       "context_keys_doc_root": "https://docs.aws.amazon.com/health/latest/ug/"
     },
     "prefix": "health"
   },
+  "HealthImaging": {
+    "actions": {
+      "CopyImageSet": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to copy an image set",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/healthimaging/latest/APIReference/API_dataplane_CopyImageSet.html"
+        }
+      },
+      "CreateDatastore": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to create a data store to ingest imaging data",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/healthimaging/latest/APIReference/API_CreateDatastore.html"
+        }
+      },
+      "DeleteDatastore": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete a data store",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/healthimaging/latest/APIReference/API_DeleteDatastore.html"
+        }
+      },
+      "DeleteImageSet": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to delete an image set",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/healthimaging/latest/APIReference/API_dataplane_DeleteImageSet.html"
+        }
+      },
+      "GetDICOMImportJob": {
+        "aws_action_groups": [
+          "ReadWrite",
+          "ReadOnly"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to get an import job's properties",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/healthimaging/latest/APIReference/API_GetDICOMImportJob.html"
+        }
+      },
+      "GetDatastore": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to get data store properties",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/healthimaging/latest/APIReference/API_GetDatastore.html"
+        }
+      },
+      "GetImageFrame": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to get image frame properties",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/healthimaging/latest/APIReference/API_dataplane_GetImageFrame.html"
+        }
+      },
+      "GetImageSet": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to get image set properties",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/healthimaging/latest/APIReference/API_dataplane_GetImageSet.html"
+        }
+      },
+      "GetImageSetMetadata": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to get image set metadata properties",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/healthimaging/latest/APIReference/API_dataplane_GetImageSetMetadata.html"
+        }
+      },
+      "ListDICOMImportJobs": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list import jobs for a data store",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/healthimaging/latest/APIReference/API_ListDICOMImportJobs.html"
+        }
+      },
+      "ListDatastores": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list data stores",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/healthimaging/latest/APIReference/API_ListDatastores.html"
+        }
+      },
+      "ListImageSetVersions": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list versions of an image set",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/healthimaging/latest/APIReference/API_dataplane_ListImageSetVersions.html"
+        }
+      },
+      "ListTagsForResource": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list tags for a medical imaging resource",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/healthimaging/latest/APIReference/API_ListTagsForResource.html"
+        }
+      },
+      "SearchImageSets": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to search image sets",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/healthimaging/latest/APIReference/API_dataplane_SearchImageSets.html"
+        }
+      },
+      "StartDICOMImportJob": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to start a DICOM import job",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/healthimaging/latest/APIReference/API_StartDICOMImportJob.html"
+        }
+      },
+      "TagResource": {
+        "aws_action_groups": [
+          "ReadWrite",
+          "Tagging"
+        ],
+        "calculated_action_group": "Tagging",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:ResourceTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to add tags to a medical imaging resource",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/healthimaging/latest/APIReference/API_TagResource.html"
+        }
+      },
+      "UntagResource": {
+        "aws_action_groups": [
+          "ReadWrite",
+          "Tagging"
+        ],
+        "calculated_action_group": "Tagging",
+        "condition_keys": [
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to remove tags from a medical imaging resource",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/healthimaging/latest/APIReference/API_UntagResource.html"
+        }
+      },
+      "UpdateImageSetMetadata": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to update image set metadata properties",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/healthimaging/latest/APIReference/API_dataplane_UpdateImageSetMetadata.html"
+        }
+      }
+    },
+    "arn_format": "arn:${Partition}:medical-imaging:${Region}:${Account}:${ResourceType}/${ResourceName}",
+    "arn_regex": "^arn:${Partition}:medical-imaging:.+:.+:.+",
+    "description": "AWS HealthImaging",
+    "docs": {
+      "actions_doc_root": "https://docs.aws.amazon.com/healthimaging/latest/APIReference/",
+      "api_detail_root": "",
+      "api_doc_root": "",
+      "api_reference_doc_page": "https://docs.aws.amazon.com/healthimaging/latest/APIReference/",
+      "authz_doc_page": "https://docs.aws.amazon.com/healthimaging/latest/devguide/security-iam.html",
+      "concepts_doc_root": "https://docs.aws.amazon.com/healthimaging/latest/devguide/",
+      "context_keys_doc_root": "https://docs.aws.amazon.com/healthimaging/latest/devguide/"
+    },
+    "prefix": "medical-imaging"
+  },
   "HealthLake": {
     "actions": {
       "CreateFHIRDatastore": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -133839,14 +134437,27 @@
         "description": "Grants permission to return a list of all ActiveMQ users",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/amazon-mq/latest/api-reference/rest-api-users.html#rest-api-users-methods-get"
         }
       },
+      "Promote": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to promote a broker",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/amazon-mq/latest/api-reference/rest-api-promote.html#rest-api-promote-methods-post"
+        }
+      },
       "RebootBroker": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to reboot a broker",
@@ -134018,15 +134629,15 @@
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to delete a cluster resource-based policy",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/msk/1.0/apireference/cluster-policy.html#DeleteClusterPolicy"
+          "doc_page_rel": "https://docs.aws.amazon.com/msk/1.0/apireference/clusters-clusterarn-policy.html#DeleteClusterPolicy"
         }
       },
       "DeleteConfiguration": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -134156,15 +134767,15 @@
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
         "description": "Grants permission to describe a cluster resource-based policy",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/msk/1.0/apireference/cluster-policy.html#GetClusterPolicy"
+          "doc_page_rel": "https://docs.aws.amazon.com/msk/1.0/apireference/clusters-clusterarn-policy.html#GetClusterPolicy"
         }
       },
       "GetCompatibleKafkaVersions": {
         "aws_action_groups": [
           "ReadWrite",
           "ReadOnly",
           "ListOnly"
@@ -134348,15 +134959,15 @@
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to create or update the resource-based policy for a cluster",
         "docs": {
           "api_doc": "",
           "doc_page": "",
-          "doc_page_rel": "https://docs.aws.amazon.com/msk/1.0/apireference/cluster-policy.html#PutClusterPolicy"
+          "doc_page_rel": "https://docs.aws.amazon.com/msk/1.0/apireference/clusters-clusterarn-policy.html#PutClusterPolicy"
         }
       },
       "RebootBroker": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -137511,14 +138122,29 @@
         "description": "Grants permission to list tags associated with a workspace",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/grafana/latest/APIReference/API_ListTagsForResource.html"
         }
       },
+      "ListVersions": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list all available supported Grafana versions. Optionally, include a workspace to list the versions to which it can be upgraded",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/grafana/latest/APIReference/API_ListVersions.html"
+        }
+      },
       "ListWorkspaces": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -153954,15 +154580,15 @@
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/outposts/latest/APIReference/API_UpdateSiteRackPhysicalProperties.html"
         }
       }
     },
     "arn_format": "arn:${Partition}:outposts:${Region}:${Account}:${ResourceType}/${ResourceName}",
-    "arn_regex": "^arn:${Partition}:outposts:.+:.+:.+",
+    "arn_regex": "^arn:${Partition}:outposts:.+",
     "description": "AWS Outposts",
     "docs": {
       "actions_doc_root": "https://docs.aws.amazon.com/outposts/latest/APIReference/",
       "api_detail_root": "",
       "api_doc_root": "",
       "api_reference_doc_page": "https://docs.aws.amazon.com/outposts/latest/APIReference/",
       "authz_doc_page": "https://docs.aws.amazon.com/outposts/latest/userguide/identity-access-management.html",
@@ -156210,14 +156836,27 @@
         "description": "Grants permission to update a campaign",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/personalize/latest/dg/API_UpdateCampaign.html"
         }
       },
+      "UpdateDataset": {
+        "aws_action_groups": [
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Write",
+        "condition_keys": [],
+        "description": "Grants permission to update a dataset",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/personalize/latest/dg/API_UpdateDataset.html"
+        }
+      },
       "UpdateMetricAttribution": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to update a metric attribution",
@@ -168913,16 +169552,16 @@
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to create a custom domain name for a cluster",
         "docs": {
           "api_doc": "",
-          "doc_page": "API_CreateCustomDomainAssociation.html",
-          "doc_page_rel": "API_CreateCustomDomainAssociation.html"
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/redshift/latest/APIReference/API_CreateCustomDomainAssociation.html"
         }
       },
       "CreateEndpointAccess": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -169171,16 +169810,16 @@
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to delete a custom domain name for a cluster",
         "docs": {
           "api_doc": "",
-          "doc_page": "API_DeleteCustomDomainAssociation.html",
-          "doc_page_rel": "API_DeleteCustomDomainAssociation.html"
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/redshift/latest/APIReference/API_DeleteCustomDomainAssociation.html"
         }
       },
       "DeleteEndpointAccess": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -169489,16 +170128,16 @@
           "ReadWrite"
         ],
         "calculated_action_group": "List",
         "condition_keys": [],
         "description": "Grants permission to describe custom domain names for a cluster",
         "docs": {
           "api_doc": "",
-          "doc_page": "API_DescribeCustomDomainAssociations.html",
-          "doc_page_rel": "API_DescribeCustomDomainAssociations.html"
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/redshift/latest/APIReference/API_DescribeCustomDomainAssociations.html"
         }
       },
       "DescribeDataShares": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
@@ -170267,16 +170906,16 @@
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to modify a custom domain name for a cluster",
         "docs": {
           "api_doc": "",
-          "doc_page": "API_ModifiyCustomDomainAssociation.html",
-          "doc_page_rel": "API_ModifiyCustomDomainAssociation.html"
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/redshift/latest/APIReference/API_ModifyCustomDomainAssociation.html"
         }
       },
       "ModifyEndpointAccess": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
@@ -170446,15 +171085,14 @@
       },
       "RestoreFromClusterSnapshot": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [
-          "aws:RequestTag/${TagKey}",
           "aws:TagKeys"
         ],
         "description": "Grants permission to create a cluster from a snapshot",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/redshift/latest/APIReference/API_RestoreFromClusterSnapshot.html"
@@ -186434,14 +187072,42 @@
         "description": "Grants permission to get account settings",
         "docs": {
           "api_doc": "",
           "doc_page": "${ConceptsDocRoot}mgmt/redshift-policy-resources.resource-permissions.html",
           "doc_page_rel": "https://docs.aws.amazon.com/redshift/latest/mgmt/redshift-policy-resources.resource-permissions.html"
         }
       },
+      "GetAutocompletionMetadata": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to get database structure metadata for auto-completion",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${ConceptsDocRoot}mgmt/redshift-policy-resources.resource-permissions.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/redshift/latest/mgmt/redshift-policy-resources.resource-permissions.html"
+        }
+      },
+      "GetAutocompletionResource": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to get database structure information for auto-completion",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "${ConceptsDocRoot}mgmt/redshift-policy-resources.resource-permissions.html",
+          "doc_page_rel": "https://docs.aws.amazon.com/redshift/latest/mgmt/redshift-policy-resources.resource-permissions.html"
+        }
+      },
       "GetChart": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -191098,14 +191764,28 @@
         "description": "Grants permission to get a SageMaker Service Catalog Portfolio",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_GetSagemakerServicecatalogPortfolioStatus.html"
         }
       },
+      "GetScalingPolicyConfigurationRecommendation": {
+        "aws_action_groups": [
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "Read",
+        "condition_keys": [],
+        "description": "Grants permission to get a scaling policy configuration recommendation",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_GetScalingPolicyConfigurationRecommendation.html"
+        }
+      },
       "GetSearchSuggestions": {
         "aws_action_groups": [
           "ReadOnly",
           "ReadWrite"
         ],
         "calculated_action_group": "Read",
         "condition_keys": [],
@@ -193855,16 +194535,16 @@
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/savingsplans/latest/APIReference/API_UntagResource.html"
         }
       }
     },
-    "arn_format": "arn:aws:savingsplans::${Account}:${ResourceType}/${ResourcePath}",
-    "arn_regex": "^arn:aws:savingsplans:.+",
+    "arn_format": "arn:${Partition}:savingsplans::${Account}:${ResourceType}/${ResourcePath}",
+    "arn_regex": "^arn:${Partition}:savingsplans:.+",
     "description": "AWS Savings Plans",
     "docs": {
       "actions_doc_root": "https://docs.aws.amazon.com/savingsplans/latest/APIReference/",
       "api_detail_root": "",
       "api_doc_root": "",
       "api_reference_doc_page": "https://docs.aws.amazon.com/savingsplans/latest/APIReference/",
       "authz_doc_page": "https://docs.aws.amazon.com/savingsplans/latest/userguide/auth-and-access-control.html",
@@ -195432,15 +196112,18 @@
         }
       },
       "CreateDataLake": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys"
+        ],
         "description": "Grants permission to create a new security data lake",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_CreateDataLake.html"
         }
       },
@@ -195471,15 +196154,18 @@
         }
       },
       "CreateSubscriber": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
-        "condition_keys": [],
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys"
+        ],
         "description": "Grants permission to create a subscriber",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_CreateSubscriber.html"
         }
       },
@@ -195712,27 +196398,75 @@
         "description": "Grants permission to list all subscribers",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_ListSubscribers.html"
         }
       },
+      "ListTagsForResource": {
+        "aws_action_groups": [
+          "ListOnly",
+          "ReadOnly",
+          "ReadWrite"
+        ],
+        "calculated_action_group": "List",
+        "condition_keys": [],
+        "description": "Grants permission to list all tags for the resource",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_ListTagsForResource.html"
+        }
+      },
       "RegisterDataLakeDelegatedAdministrator": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to designate an account as the Amazon Security Lake administrator account for the organization",
         "docs": {
           "api_doc": "",
           "doc_page": "",
           "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_RegisterDataLakeDelegatedAdministrator.html"
         }
       },
+      "TagResource": {
+        "aws_action_groups": [
+          "ReadWrite",
+          "Tagging"
+        ],
+        "calculated_action_group": "Tagging",
+        "condition_keys": [
+          "aws:RequestTag/${TagKey}",
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to add tags to the resource",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_TagResource.html"
+        }
+      },
+      "UntagResource": {
+        "aws_action_groups": [
+          "ReadWrite",
+          "Tagging"
+        ],
+        "calculated_action_group": "Tagging",
+        "condition_keys": [
+          "aws:TagKeys"
+        ],
+        "description": "Grants permission to remove tags from the resource",
+        "docs": {
+          "api_doc": "",
+          "doc_page": "",
+          "doc_page_rel": "https://docs.aws.amazon.com/security-lake/latest/APIReference/API_UntagResource.html"
+        }
+      },
       "UpdateDataLake": {
         "aws_action_groups": [
           "ReadWrite"
         ],
         "calculated_action_group": "Write",
         "condition_keys": [],
         "description": "Grants permission to update a security data lake",
```

### Comparing `policyuniverse-1.5.1.20230703/policyuniverse/expander_minimizer.py` & `policyuniverse-1.5.1.20230725/policyuniverse/expander_minimizer.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230703/policyuniverse/organization.py` & `policyuniverse-1.5.1.20230725/policyuniverse/organization.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230703/policyuniverse/policy.py` & `policyuniverse-1.5.1.20230725/policyuniverse/policy.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230703/policyuniverse/statement.py` & `policyuniverse-1.5.1.20230725/policyuniverse/statement.py`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230703/policyuniverse.egg-info/PKG-INFO` & `policyuniverse-1.5.1.20230725/policyuniverse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: policyuniverse
-Version: 1.5.1.20230703
+Version: 1.5.1.20230725
 Summary: Parse and Process AWS IAM Policies, Statements, ARNs, and wildcards.
 Home-page: https://github.com/Netflix-Skunkworks/policyuniverse
 Author: Patrick Kelley
 Author-email: patrickbarrettkelley@gmail.com
 Keywords: iam,arn,action_groups,condition,policy,statement,wildcard
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
```

### Comparing `policyuniverse-1.5.1.20230703/policyuniverse.egg-info/SOURCES.txt` & `policyuniverse-1.5.1.20230725/policyuniverse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `policyuniverse-1.5.1.20230703/setup.py` & `policyuniverse-1.5.1.20230725/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ROOT = os.path.realpath(os.path.join(os.path.dirname(__file__)))
 
 tests_require = ["pytest", "coveralls", "bandit"]
 dev_require = ["pre-commit", "black"]
 
 setup(
     name="policyuniverse",
-    version="1.5.1.20230703",
+    version="1.5.1.20230725",
     description="Parse and Process AWS IAM Policies, Statements, ARNs, and wildcards.",
     long_description=open(os.path.join(ROOT, "README.md")).read(),
     long_description_content_type="text/markdown",
     author="Patrick Kelley",
     author_email="patrickbarrettkelley@gmail.com",
     url="https://github.com/Netflix-Skunkworks/policyuniverse",
     keywords=[
```

