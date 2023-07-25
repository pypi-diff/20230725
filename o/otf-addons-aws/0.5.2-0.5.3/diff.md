# Comparing `tmp/otf-addons-aws-0.5.2.tar.gz` & `tmp/otf-addons-aws-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otf-addons-aws-0.5.2.tar", last modified: Sat Jul 22 19:25:15 2023, max compression
+gzip compressed data, was "otf-addons-aws-0.5.3.tar", last modified: Tue Jul 25 15:09:04 2023, max compression
```

## Comparing `otf-addons-aws-0.5.2.tar` & `otf-addons-aws-0.5.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.756633 otf-addons-aws-0.5.2/
--rw-r--r--   0 adam       (501) staff       (20)       72 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.2/AUTHORS
--rw-r--r--   0 adam       (501) staff       (20)    35149 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.2/LICENSE
--rw-r--r--   0 adam       (501) staff       (20)       44 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.2/MANIFEST.in
--rw-r--r--   0 adam       (501) staff       (20)     6050 2023-07-22 19:25:15.756496 otf-addons-aws-0.5.2/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)     5211 2023-07-21 15:52:59.000000 otf-addons-aws-0.5.2/README.md
--rw-r--r--   0 adam       (501) staff       (20)    13231 2023-07-22 19:25:03.000000 otf-addons-aws-0.5.2/pyproject.toml
--rw-r--r--   0 adam       (501) staff       (20)       38 2023-07-22 19:25:15.756670 otf-addons-aws-0.5.2/setup.cfg
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.748048 otf-addons-aws-0.5.2/src/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.747906 otf-addons-aws-0.5.2/src/opentaskpy/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.747388 otf-addons-aws-0.5.2/src/opentaskpy/addons/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.749722 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/
--rw-r--r--   0 adam       (501) staff       (20)        0 2023-07-22 14:47:19.000000 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/__init__.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.750698 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/
--rw-r--r--   0 adam       (501) staff       (20)        0 2023-07-20 13:18:56.000000 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)      942 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/creds.py
--rw-r--r--   0 adam       (501) staff       (20)     4685 2023-07-22 16:20:49.000000 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/lambda.py
--rw-r--r--   0 adam       (501) staff       (20)    13127 2023-07-22 16:28:21.000000 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/s3.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.747726 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.747665 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.751298 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/
--rw-r--r--   0 adam       (501) staff       (20)      542 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/lambda.json
--rw-r--r--   0 adam       (501) staff       (20)      506 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/protocol.json
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.751712 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/s3/
--rw-r--r--   0 adam       (501) staff       (20)      503 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/s3/protocol.json
--rw-r--r--   0 adam       (501) staff       (20)      429 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/s3/s3.json
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.753057 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.753502 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination/
--rw-r--r--   0 adam       (501) staff       (20)      279 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination/flags.json
--rw-r--r--   0 adam       (501) staff       (20)      571 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination/protocol.json
--rw-r--r--   0 adam       (501) staff       (20)      485 2023-07-21 13:36:27.000000 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination.json
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.753839 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source/
--rw-r--r--   0 adam       (501) staff       (20)      398 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source/fileWatch.json
--rw-r--r--   0 adam       (501) staff       (20)      500 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source/protocol.json
--rw-r--r--   0 adam       (501) staff       (20)      663 2023-07-21 13:36:27.000000 otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source.json
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.747948 otf-addons-aws-0.5.2/src/opentaskpy/plugins/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.747988 otf-addons-aws-0.5.2/src/opentaskpy/plugins/lookup/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.753989 otf-addons-aws-0.5.2/src/opentaskpy/plugins/lookup/aws/
--rw-r--r--   0 adam       (501) staff       (20)     2819 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.2/src/opentaskpy/plugins/lookup/aws/ssm.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.754590 otf-addons-aws-0.5.2/src/otf_addons_aws.egg-info/
--rw-r--r--   0 adam       (501) staff       (20)     6050 2023-07-22 19:25:15.000000 otf-addons-aws-0.5.2/src/otf_addons_aws.egg-info/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)     1570 2023-07-22 19:25:15.000000 otf-addons-aws-0.5.2/src/otf_addons_aws.egg-info/SOURCES.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2023-07-22 19:25:15.000000 otf-addons-aws-0.5.2/src/otf_addons_aws.egg-info/dependency_links.txt
--rw-r--r--   0 adam       (501) staff       (20)      228 2023-07-22 19:25:15.000000 otf-addons-aws-0.5.2/src/otf_addons_aws.egg-info/requires.txt
--rw-r--r--   0 adam       (501) staff       (20)       11 2023-07-22 19:25:15.000000 otf-addons-aws-0.5.2/src/otf_addons_aws.egg-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-22 19:25:15.756258 otf-addons-aws-0.5.2/tests/
--rw-r--r--   0 adam       (501) staff       (20)      670 2023-07-20 13:18:56.000000 otf-addons-aws-0.5.2/tests/test_lambda_execution_schema_validate.py
--rw-r--r--   0 adam       (501) staff       (20)     2413 2023-07-22 14:53:37.000000 otf-addons-aws-0.5.2/tests/test_plugin_ssm.py
--rw-r--r--   0 adam       (501) staff       (20)    11598 2023-07-22 16:02:47.000000 otf-addons-aws-0.5.2/tests/test_remotehandler_lambda_execution.py
--rw-r--r--   0 adam       (501) staff       (20)     1893 2023-07-22 14:53:16.000000 otf-addons-aws-0.5.2/tests/test_remotehandler_s3_execution.py
--rw-r--r--   0 adam       (501) staff       (20)    22384 2023-07-22 19:15:25.000000 otf-addons-aws-0.5.2/tests/test_remotehandler_s3_transfer.py
--rw-r--r--   0 adam       (501) staff       (20)     2272 2023-07-21 13:36:27.000000 otf-addons-aws-0.5.2/tests/test_s3_source_schema_validate.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-25 15:09:04.512785 otf-addons-aws-0.5.3/
+-rw-r--r--   0 adam       (501) staff       (20)       72 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.3/AUTHORS
+-rw-r--r--   0 adam       (501) staff       (20)    35149 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.3/LICENSE
+-rw-r--r--   0 adam       (501) staff       (20)       44 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.3/MANIFEST.in
+-rw-r--r--   0 adam       (501) staff       (20)     6050 2023-07-25 15:09:04.512692 otf-addons-aws-0.5.3/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)     5211 2023-07-22 19:30:44.000000 otf-addons-aws-0.5.3/README.md
+-rw-r--r--   0 adam       (501) staff       (20)    13231 2023-07-25 15:08:29.000000 otf-addons-aws-0.5.3/pyproject.toml
+-rw-r--r--   0 adam       (501) staff       (20)       38 2023-07-25 15:09:04.512816 otf-addons-aws-0.5.3/setup.cfg
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-25 15:09:04.509070 otf-addons-aws-0.5.3/src/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-25 15:09:04.508885 otf-addons-aws-0.5.3/src/opentaskpy/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-25 15:09:04.508297 otf-addons-aws-0.5.3/src/opentaskpy/addons/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-25 15:09:04.509857 otf-addons-aws-0.5.3/src/opentaskpy/addons/aws/
+-rw-r--r--   0 adam       (501) staff       (20)        0 2023-07-22 14:47:19.000000 otf-addons-aws-0.5.3/src/opentaskpy/addons/aws/__init__.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-25 15:09:04.510271 otf-addons-aws-0.5.3/src/opentaskpy/addons/aws/remotehandlers/
+-rw-r--r--   0 adam       (501) staff       (20)        0 2023-07-20 13:18:56.000000 otf-addons-aws-0.5.3/src/opentaskpy/addons/aws/remotehandlers/__init__.py
+-rw-r--r--   0 adam       (501) staff       (20)      942 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.3/src/opentaskpy/addons/aws/remotehandlers/creds.py
+-rw-r--r--   0 adam       (501) staff       (20)     4685 2023-07-22 19:30:44.000000 otf-addons-aws-0.5.3/src/opentaskpy/addons/aws/remotehandlers/lambda.py
+-rw-r--r--   0 adam       (501) staff       (20)    13127 2023-07-22 19:30:44.000000 otf-addons-aws-0.5.3/src/opentaskpy/addons/aws/remotehandlers/s3.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-25 15:09:04.508655 otf-addons-aws-0.5.3/src/opentaskpy/addons/aws/remotehandlers/schemas/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-25 15:09:04.508585 otf-addons-aws-0.5.3/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-25 15:09:04.510492 otf-addons-aws-0.5.3/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/
+-rw-r--r--   0 adam       (501) staff       (20)      542 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.3/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/lambda.json
+-rw-r--r--   0 adam       (501) staff       (20)      506 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.3/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/protocol.json
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-25 15:09:04.510715 otf-addons-aws-0.5.3/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/s3/
+-rw-r--r--   0 adam       (501) staff       (20)      503 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.3/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/s3/protocol.json
+-rw-r--r--   0 adam       (501) staff       (20)      429 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.3/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/s3/s3.json
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-25 15:09:04.510919 otf-addons-aws-0.5.3/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-25 15:09:04.511137 otf-addons-aws-0.5.3/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination/
+-rw-r--r--   0 adam       (501) staff       (20)      279 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.3/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination/flags.json
+-rw-r--r--   0 adam       (501) staff       (20)      571 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.3/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination/protocol.json
+-rw-r--r--   0 adam       (501) staff       (20)      485 2023-07-21 13:36:27.000000 otf-addons-aws-0.5.3/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination.json
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-25 15:09:04.511340 otf-addons-aws-0.5.3/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source/
+-rw-r--r--   0 adam       (501) staff       (20)      398 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.3/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source/fileWatch.json
+-rw-r--r--   0 adam       (501) staff       (20)      500 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.3/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source/protocol.json
+-rw-r--r--   0 adam       (501) staff       (20)      663 2023-07-21 13:36:27.000000 otf-addons-aws-0.5.3/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source.json
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-25 15:09:04.508943 otf-addons-aws-0.5.3/src/opentaskpy/plugins/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-25 15:09:04.509006 otf-addons-aws-0.5.3/src/opentaskpy/plugins/lookup/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-25 15:09:04.511440 otf-addons-aws-0.5.3/src/opentaskpy/plugins/lookup/aws/
+-rw-r--r--   0 adam       (501) staff       (20)     2819 2023-07-21 12:30:08.000000 otf-addons-aws-0.5.3/src/opentaskpy/plugins/lookup/aws/ssm.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-25 15:09:04.511932 otf-addons-aws-0.5.3/src/otf_addons_aws.egg-info/
+-rw-r--r--   0 adam       (501) staff       (20)     6050 2023-07-25 15:09:04.000000 otf-addons-aws-0.5.3/src/otf_addons_aws.egg-info/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)     1570 2023-07-25 15:09:04.000000 otf-addons-aws-0.5.3/src/otf_addons_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2023-07-25 15:09:04.000000 otf-addons-aws-0.5.3/src/otf_addons_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 adam       (501) staff       (20)      228 2023-07-25 15:09:04.000000 otf-addons-aws-0.5.3/src/otf_addons_aws.egg-info/requires.txt
+-rw-r--r--   0 adam       (501) staff       (20)       11 2023-07-25 15:09:04.000000 otf-addons-aws-0.5.3/src/otf_addons_aws.egg-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-25 15:09:04.512543 otf-addons-aws-0.5.3/tests/
+-rw-r--r--   0 adam       (501) staff       (20)      670 2023-07-20 13:18:56.000000 otf-addons-aws-0.5.3/tests/test_lambda_execution_schema_validate.py
+-rw-r--r--   0 adam       (501) staff       (20)     2413 2023-07-22 19:30:44.000000 otf-addons-aws-0.5.3/tests/test_plugin_ssm.py
+-rw-r--r--   0 adam       (501) staff       (20)    11598 2023-07-22 19:30:44.000000 otf-addons-aws-0.5.3/tests/test_remotehandler_lambda_execution.py
+-rw-r--r--   0 adam       (501) staff       (20)     1893 2023-07-22 19:30:44.000000 otf-addons-aws-0.5.3/tests/test_remotehandler_s3_execution.py
+-rw-r--r--   0 adam       (501) staff       (20)    22384 2023-07-22 19:30:44.000000 otf-addons-aws-0.5.3/tests/test_remotehandler_s3_transfer.py
+-rw-r--r--   0 adam       (501) staff       (20)     2272 2023-07-21 13:36:27.000000 otf-addons-aws-0.5.3/tests/test_s3_source_schema_validate.py
```

### Comparing `otf-addons-aws-0.5.2/LICENSE` & `otf-addons-aws-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-0.5.2/PKG-INFO` & `otf-addons-aws-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otf-addons-aws
-Version: 0.5.2
+Version: 0.5.3
 Summary: Addons for opentaskpy, giving it the ability to push/pull via AWS S3, and pull variables from AWS SSM Parameter Store.
 Author-email: Adam McDonagh <adam@elitemonkey.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/adammcdonagh/otf-addons-aws
 Project-URL: Bug Tracker, https://github.com/adammcdonagh/otf-addons-aws/issues
 Project-URL: Changelog, https://github.com/adammcdonagh/otf-addons-aws/blob/main/CHANGELOG.md
 Keywords: automation,task,framework,aws,s3,ssm,otf
```

### Comparing `otf-addons-aws-0.5.2/README.md` & `otf-addons-aws-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-0.5.2/pyproject.toml` & `otf-addons-aws-0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "otf-addons-aws"
-version = "0.5.2"
+version = "0.5.3"
 authors = [
   { name="Adam McDonagh", email="adam@elitemonkey.net" },
 ]
 license = { text = "GPLv3" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: POSIX",
 ]
 keywords = ["automation", "task", "framework", "aws", "s3", "ssm", "otf"]
 dependencies = [
   "boto3 >= 1.26",
-  "opentaskpy >= 0.12.1",
+  "opentaskpy >= 0.13.0",
 ]
 description = "Addons for opentaskpy, giving it the ability to push/pull via AWS S3, and pull variables from AWS SSM Parameter Store."
 readme = "README.md"
 requires-python = ">=3.11"
 
 [project.optional-dependencies]
 dev = [
@@ -51,15 +51,15 @@
 "Bug Tracker" = "https://github.com/adammcdonagh/otf-addons-aws/issues"
 "Changelog" = "https://github.com/adammcdonagh/otf-addons-aws/blob/main/CHANGELOG.md"
 
 [tool.isort]
 profile = 'black'
 
 [tool.bumpver]
-current_version = "0.5.2"
+current_version = "0.5.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/creds.py` & `otf-addons-aws-0.5.3/src/opentaskpy/addons/aws/remotehandlers/creds.py`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/lambda.py` & `otf-addons-aws-0.5.3/src/opentaskpy/addons/aws/remotehandlers/lambda.py`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/s3.py` & `otf-addons-aws-0.5.3/src/opentaskpy/addons/aws/remotehandlers/s3.py`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/lambda.json` & `otf-addons-aws-0.5.3/src/opentaskpy/addons/aws/remotehandlers/schemas/execution/lambda/lambda.json`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination/protocol.json` & `otf-addons-aws-0.5.3/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_destination/protocol.json`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-0.5.2/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source.json` & `otf-addons-aws-0.5.3/src/opentaskpy/addons/aws/remotehandlers/schemas/transfer/s3_source.json`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-0.5.2/src/opentaskpy/plugins/lookup/aws/ssm.py` & `otf-addons-aws-0.5.3/src/opentaskpy/plugins/lookup/aws/ssm.py`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-0.5.2/src/otf_addons_aws.egg-info/PKG-INFO` & `otf-addons-aws-0.5.3/src/otf_addons_aws.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otf-addons-aws
-Version: 0.5.2
+Version: 0.5.3
 Summary: Addons for opentaskpy, giving it the ability to push/pull via AWS S3, and pull variables from AWS SSM Parameter Store.
 Author-email: Adam McDonagh <adam@elitemonkey.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/adammcdonagh/otf-addons-aws
 Project-URL: Bug Tracker, https://github.com/adammcdonagh/otf-addons-aws/issues
 Project-URL: Changelog, https://github.com/adammcdonagh/otf-addons-aws/blob/main/CHANGELOG.md
 Keywords: automation,task,framework,aws,s3,ssm,otf
```

### Comparing `otf-addons-aws-0.5.2/src/otf_addons_aws.egg-info/SOURCES.txt` & `otf-addons-aws-0.5.3/src/otf_addons_aws.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-0.5.2/tests/test_lambda_execution_schema_validate.py` & `otf-addons-aws-0.5.3/tests/test_lambda_execution_schema_validate.py`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-0.5.2/tests/test_plugin_ssm.py` & `otf-addons-aws-0.5.3/tests/test_plugin_ssm.py`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-0.5.2/tests/test_remotehandler_lambda_execution.py` & `otf-addons-aws-0.5.3/tests/test_remotehandler_lambda_execution.py`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-0.5.2/tests/test_remotehandler_s3_execution.py` & `otf-addons-aws-0.5.3/tests/test_remotehandler_s3_execution.py`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-0.5.2/tests/test_remotehandler_s3_transfer.py` & `otf-addons-aws-0.5.3/tests/test_remotehandler_s3_transfer.py`

 * *Files identical despite different names*

### Comparing `otf-addons-aws-0.5.2/tests/test_s3_source_schema_validate.py` & `otf-addons-aws-0.5.3/tests/test_s3_source_schema_validate.py`

 * *Files identical despite different names*

