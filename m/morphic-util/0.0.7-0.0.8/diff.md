# Comparing `tmp/morphic-util-0.0.7.tar.gz` & `tmp/morphic-util-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morphic-util-0.0.7.tar", last modified: Mon Jul 24 08:54:59 2023, max compression
+gzip compressed data, was "morphic-util-0.0.8.tar", last modified: Tue Jul 25 10:12:52 2023, max compression
```

## Comparing `morphic-util-0.0.7.tar` & `morphic-util-0.0.8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0 dgupta    (1000) dgupta    (1000)        0 2023-07-24 08:54:59.915302 morphic-util-0.0.7/
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)    11558 2023-06-15 13:44:26.000000 morphic-util-0.0.7/LICENSE
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)       20 2023-06-15 13:44:26.000000 morphic-util-0.0.7/MANIFEST.in
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     6031 2023-07-24 08:54:59.913303 morphic-util-0.0.7/PKG-INFO
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     4176 2023-06-20 14:57:12.000000 morphic-util-0.0.7/README.md
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     1389 2023-06-15 13:44:26.000000 morphic-util-0.0.7/RELEASE.md
-drwxrwxrwx   0 dgupta    (1000) dgupta    (1000)        0 2023-07-24 08:54:59.044905 morphic-util-0.0.7/ait/
-drwxrwxrwx   0 dgupta    (1000) dgupta    (1000)        0 2023-07-24 08:54:59.046905 morphic-util-0.0.7/ait/commons/
-drwxrwxrwx   0 dgupta    (1000) dgupta    (1000)        0 2023-07-24 08:54:59.406876 morphic-util-0.0.7/ait/commons/util/
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)        0 2023-06-15 13:44:26.000000 morphic-util-0.0.7/ait/commons/util/__init__.py
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     8566 2023-06-20 14:57:12.000000 morphic-util-0.0.7/ait/commons/util/__main__.py
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     4361 2023-07-24 06:40:12.000000 morphic-util-0.0.7/ait/commons/util/aws_client.py
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     6670 2023-07-24 08:34:44.000000 morphic-util-0.0.7/ait/commons/util/aws_cognito_authenticator.py
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     2051 2023-06-22 13:12:49.000000 morphic-util-0.0.7/ait/commons/util/bucket_policy.py
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     4036 2023-06-20 14:57:12.000000 morphic-util-0.0.7/ait/commons/util/cmd.py
-drwxrwxrwx   0 dgupta    (1000) dgupta    (1000)        0 2023-07-24 08:54:59.690694 morphic-util-0.0.7/ait/commons/util/command/
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)        0 2023-06-15 13:44:26.000000 morphic-util-0.0.7/ait/commons/util/command/__init__.py
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)      758 2023-06-15 13:44:26.000000 morphic-util-0.0.7/ait/commons/util/command/area.py
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     1284 2023-06-20 14:57:12.000000 morphic-util-0.0.7/ait/commons/util/command/config.py
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     3544 2023-06-22 13:12:49.000000 morphic-util-0.0.7/ait/commons/util/command/create.py
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     6507 2023-06-22 13:12:49.000000 morphic-util-0.0.7/ait/commons/util/command/delete.py
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     4299 2023-06-20 14:57:12.000000 morphic-util-0.0.7/ait/commons/util/command/download.py
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     4417 2023-06-20 14:57:12.000000 morphic-util-0.0.7/ait/commons/util/command/list.py
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     1667 2023-06-21 15:47:27.000000 morphic-util-0.0.7/ait/commons/util/command/select.py
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     5178 2023-06-15 13:44:26.000000 morphic-util-0.0.7/ait/commons/util/command/sync.py
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     4876 2023-06-22 13:12:49.000000 morphic-util-0.0.7/ait/commons/util/command/upload.py
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     2054 2023-06-20 14:57:12.000000 morphic-util-0.0.7/ait/commons/util/common.py
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     1962 2023-06-15 13:44:26.000000 morphic-util-0.0.7/ait/commons/util/file_transfer.py
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     1924 2023-06-15 13:44:26.000000 morphic-util-0.0.7/ait/commons/util/local_state.py
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)      465 2023-06-15 13:44:26.000000 morphic-util-0.0.7/ait/commons/util/progress_bar.py
-drwxrwxrwx   0 dgupta    (1000) dgupta    (1000)        0 2023-07-24 08:54:59.776757 morphic-util-0.0.7/ait/commons/util/settings/
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)      268 2023-06-20 14:57:12.000000 morphic-util-0.0.7/ait/commons/util/settings/__init__.py
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)      989 2023-07-24 05:58:56.000000 morphic-util-0.0.7/ait/commons/util/settings/hca_util.py
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     1340 2023-07-24 08:35:23.000000 morphic-util-0.0.7/ait/commons/util/settings/morphic_util.py
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     1880 2023-06-15 13:44:26.000000 morphic-util-0.0.7/ait/commons/util/upload_service.py
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     3210 2023-06-20 14:57:12.000000 morphic-util-0.0.7/ait/commons/util/user_profile.py
-drwxrwxrwx   0 dgupta    (1000) dgupta    (1000)        0 2023-07-24 08:54:59.896094 morphic-util-0.0.7/morphic_util.egg-info/
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     6031 2023-07-24 08:54:58.000000 morphic-util-0.0.7/morphic_util.egg-info/PKG-INFO
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     1158 2023-07-24 08:54:58.000000 morphic-util-0.0.7/morphic_util.egg-info/SOURCES.txt
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)        1 2023-07-24 08:54:58.000000 morphic-util-0.0.7/morphic_util.egg-info/dependency_links.txt
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)       65 2023-07-24 08:54:58.000000 morphic-util-0.0.7/morphic_util.egg-info/entry_points.txt
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)       86 2023-07-24 08:54:58.000000 morphic-util-0.0.7/morphic_util.egg-info/requires.txt
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)        4 2023-07-24 08:54:58.000000 morphic-util-0.0.7/morphic_util.egg-info/top_level.txt
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)       31 2023-06-15 13:44:26.000000 morphic-util-0.0.7/requirements-dev.txt
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)       91 2023-06-20 14:57:12.000000 morphic-util-0.0.7/requirements.txt
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)       38 2023-07-24 08:54:59.916303 morphic-util-0.0.7/setup.cfg
--rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     1526 2023-06-20 14:57:12.000000 morphic-util-0.0.7/setup.py
+drwxrwxrwx   0 dgupta    (1000) dgupta    (1000)        0 2023-07-25 10:12:52.701276 morphic-util-0.0.8/
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)    11558 2023-06-15 13:44:26.000000 morphic-util-0.0.8/LICENSE
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)       20 2023-06-15 13:44:26.000000 morphic-util-0.0.8/MANIFEST.in
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     6031 2023-07-25 10:12:52.699001 morphic-util-0.0.8/PKG-INFO
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     4176 2023-06-20 14:57:12.000000 morphic-util-0.0.8/README.md
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     1389 2023-06-15 13:44:26.000000 morphic-util-0.0.8/RELEASE.md
+drwxrwxrwx   0 dgupta    (1000) dgupta    (1000)        0 2023-07-25 10:12:51.864638 morphic-util-0.0.8/ait/
+drwxrwxrwx   0 dgupta    (1000) dgupta    (1000)        0 2023-07-25 10:12:51.866638 morphic-util-0.0.8/ait/commons/
+drwxrwxrwx   0 dgupta    (1000) dgupta    (1000)        0 2023-07-25 10:12:52.241565 morphic-util-0.0.8/ait/commons/util/
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)        0 2023-06-15 13:44:26.000000 morphic-util-0.0.8/ait/commons/util/__init__.py
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     8566 2023-06-20 14:57:12.000000 morphic-util-0.0.8/ait/commons/util/__main__.py
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     4361 2023-07-25 10:06:57.000000 morphic-util-0.0.8/ait/commons/util/aws_client.py
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     6670 2023-07-25 10:06:57.000000 morphic-util-0.0.8/ait/commons/util/aws_cognito_authenticator.py
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     2051 2023-06-22 13:12:49.000000 morphic-util-0.0.8/ait/commons/util/bucket_policy.py
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     4036 2023-06-20 14:57:12.000000 morphic-util-0.0.8/ait/commons/util/cmd.py
+drwxrwxrwx   0 dgupta    (1000) dgupta    (1000)        0 2023-07-25 10:12:52.493843 morphic-util-0.0.8/ait/commons/util/command/
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)        0 2023-06-15 13:44:26.000000 morphic-util-0.0.8/ait/commons/util/command/__init__.py
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)      758 2023-06-15 13:44:26.000000 morphic-util-0.0.8/ait/commons/util/command/area.py
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     1284 2023-06-20 14:57:12.000000 morphic-util-0.0.8/ait/commons/util/command/config.py
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     3544 2023-06-22 13:12:49.000000 morphic-util-0.0.8/ait/commons/util/command/create.py
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     6507 2023-06-22 13:12:49.000000 morphic-util-0.0.8/ait/commons/util/command/delete.py
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     4299 2023-06-20 14:57:12.000000 morphic-util-0.0.8/ait/commons/util/command/download.py
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     4417 2023-06-20 14:57:12.000000 morphic-util-0.0.8/ait/commons/util/command/list.py
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     1667 2023-06-21 15:47:27.000000 morphic-util-0.0.8/ait/commons/util/command/select.py
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     5178 2023-06-15 13:44:26.000000 morphic-util-0.0.8/ait/commons/util/command/sync.py
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     4876 2023-06-22 13:12:49.000000 morphic-util-0.0.8/ait/commons/util/command/upload.py
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     2054 2023-06-20 14:57:12.000000 morphic-util-0.0.8/ait/commons/util/common.py
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     1962 2023-06-15 13:44:26.000000 morphic-util-0.0.8/ait/commons/util/file_transfer.py
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     1924 2023-06-15 13:44:26.000000 morphic-util-0.0.8/ait/commons/util/local_state.py
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)      465 2023-06-15 13:44:26.000000 morphic-util-0.0.8/ait/commons/util/progress_bar.py
+drwxrwxrwx   0 dgupta    (1000) dgupta    (1000)        0 2023-07-25 10:12:52.569104 morphic-util-0.0.8/ait/commons/util/settings/
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)      268 2023-06-20 14:57:12.000000 morphic-util-0.0.8/ait/commons/util/settings/__init__.py
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)      989 2023-07-25 10:06:57.000000 morphic-util-0.0.8/ait/commons/util/settings/hca_util.py
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     1340 2023-07-25 10:08:59.000000 morphic-util-0.0.8/ait/commons/util/settings/morphic_util.py
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     1880 2023-06-15 13:44:26.000000 morphic-util-0.0.8/ait/commons/util/upload_service.py
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     3210 2023-06-20 14:57:12.000000 morphic-util-0.0.8/ait/commons/util/user_profile.py
+drwxrwxrwx   0 dgupta    (1000) dgupta    (1000)        0 2023-07-25 10:12:52.684166 morphic-util-0.0.8/morphic_util.egg-info/
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     6031 2023-07-25 10:12:51.000000 morphic-util-0.0.8/morphic_util.egg-info/PKG-INFO
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     1158 2023-07-25 10:12:51.000000 morphic-util-0.0.8/morphic_util.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)        1 2023-07-25 10:12:51.000000 morphic-util-0.0.8/morphic_util.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)       65 2023-07-25 10:12:51.000000 morphic-util-0.0.8/morphic_util.egg-info/entry_points.txt
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)       98 2023-07-25 10:12:51.000000 morphic-util-0.0.8/morphic_util.egg-info/requires.txt
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)        4 2023-07-25 10:12:51.000000 morphic-util-0.0.8/morphic_util.egg-info/top_level.txt
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)       31 2023-06-15 13:44:26.000000 morphic-util-0.0.8/requirements-dev.txt
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)      104 2023-07-25 10:05:06.000000 morphic-util-0.0.8/requirements.txt
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)       38 2023-07-25 10:12:52.702278 morphic-util-0.0.8/setup.cfg
+-rwxrwxrwx   0 dgupta    (1000) dgupta    (1000)     1526 2023-06-20 14:57:12.000000 morphic-util-0.0.8/setup.py
```

### Comparing `morphic-util-0.0.7/LICENSE` & `morphic-util-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `morphic-util-0.0.7/PKG-INFO` & `morphic-util-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphic-util
-Version: 0.0.7
+Version: 0.0.8
 Summary: CLI tool for uploading data to Morphic AWS S3 bucket
 Home-page: https://github.com/ebi-ait/morphic-util
 Author: hca-ingest-dev
 Author-email: hca-ingest-dev@ebi.ac.uk
 License: Apache License
 Description: # morphic-util
```

### Comparing `morphic-util-0.0.7/README.md` & `morphic-util-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `morphic-util-0.0.7/RELEASE.md` & `morphic-util-0.0.8/RELEASE.md`

 * *Files identical despite different names*

### Comparing `morphic-util-0.0.7/ait/commons/util/__main__.py` & `morphic-util-0.0.8/ait/commons/util/__main__.py`

 * *Files identical despite different names*

### Comparing `morphic-util-0.0.7/ait/commons/util/aws_client.py` & `morphic-util-0.0.8/ait/commons/util/aws_client.py`

 * *Files identical despite different names*

### Comparing `morphic-util-0.0.7/ait/commons/util/aws_cognito_authenticator.py` & `morphic-util-0.0.8/ait/commons/util/aws_cognito_authenticator.py`

 * *Files identical despite different names*

### Comparing `morphic-util-0.0.7/ait/commons/util/bucket_policy.py` & `morphic-util-0.0.8/ait/commons/util/bucket_policy.py`

 * *Files identical despite different names*

### Comparing `morphic-util-0.0.7/ait/commons/util/cmd.py` & `morphic-util-0.0.8/ait/commons/util/cmd.py`

 * *Files identical despite different names*

### Comparing `morphic-util-0.0.7/ait/commons/util/command/area.py` & `morphic-util-0.0.8/ait/commons/util/command/area.py`

 * *Files identical despite different names*

### Comparing `morphic-util-0.0.7/ait/commons/util/command/config.py` & `morphic-util-0.0.8/ait/commons/util/command/config.py`

 * *Files identical despite different names*

### Comparing `morphic-util-0.0.7/ait/commons/util/command/create.py` & `morphic-util-0.0.8/ait/commons/util/command/create.py`

 * *Files identical despite different names*

### Comparing `morphic-util-0.0.7/ait/commons/util/command/delete.py` & `morphic-util-0.0.8/ait/commons/util/command/delete.py`

 * *Files identical despite different names*

### Comparing `morphic-util-0.0.7/ait/commons/util/command/download.py` & `morphic-util-0.0.8/ait/commons/util/command/download.py`

 * *Files identical despite different names*

### Comparing `morphic-util-0.0.7/ait/commons/util/command/list.py` & `morphic-util-0.0.8/ait/commons/util/command/list.py`

 * *Files identical despite different names*

### Comparing `morphic-util-0.0.7/ait/commons/util/command/select.py` & `morphic-util-0.0.8/ait/commons/util/command/select.py`

 * *Files identical despite different names*

### Comparing `morphic-util-0.0.7/ait/commons/util/command/sync.py` & `morphic-util-0.0.8/ait/commons/util/command/sync.py`

 * *Files identical despite different names*

### Comparing `morphic-util-0.0.7/ait/commons/util/command/upload.py` & `morphic-util-0.0.8/ait/commons/util/command/upload.py`

 * *Files identical despite different names*

### Comparing `morphic-util-0.0.7/ait/commons/util/common.py` & `morphic-util-0.0.8/ait/commons/util/common.py`

 * *Files identical despite different names*

### Comparing `morphic-util-0.0.7/ait/commons/util/file_transfer.py` & `morphic-util-0.0.8/ait/commons/util/file_transfer.py`

 * *Files identical despite different names*

### Comparing `morphic-util-0.0.7/ait/commons/util/local_state.py` & `morphic-util-0.0.8/ait/commons/util/local_state.py`

 * *Files identical despite different names*

### Comparing `morphic-util-0.0.7/ait/commons/util/settings/hca_util.py` & `morphic-util-0.0.8/ait/commons/util/settings/hca_util.py`

 * *Files identical despite different names*

### Comparing `morphic-util-0.0.7/ait/commons/util/settings/morphic_util.py` & `morphic-util-0.0.8/ait/commons/util/settings/morphic_util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 
 NAME = 'morphic-util'
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESC = 'CLI tool for uploading data to Morphic AWS S3 bucket'
 AUTHOR = 'hca-ingest-dev'
 AUTHOR_EMAIL = 'hca-ingest-dev@ebi.ac.uk'
 
 # when true, displays exception details; otherwise user-friendly error message
 DEBUG_MODE = False
```

### Comparing `morphic-util-0.0.7/ait/commons/util/upload_service.py` & `morphic-util-0.0.8/ait/commons/util/upload_service.py`

 * *Files identical despite different names*

### Comparing `morphic-util-0.0.7/ait/commons/util/user_profile.py` & `morphic-util-0.0.8/ait/commons/util/user_profile.py`

 * *Files identical despite different names*

### Comparing `morphic-util-0.0.7/morphic_util.egg-info/PKG-INFO` & `morphic-util-0.0.8/morphic_util.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morphic-util
-Version: 0.0.7
+Version: 0.0.8
 Summary: CLI tool for uploading data to Morphic AWS S3 bucket
 Home-page: https://github.com/ebi-ait/morphic-util
 Author: hca-ingest-dev
 Author-email: hca-ingest-dev@ebi.ac.uk
 License: Apache License
 Description: # morphic-util
```

### Comparing `morphic-util-0.0.7/morphic_util.egg-info/SOURCES.txt` & `morphic-util-0.0.8/morphic_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `morphic-util-0.0.7/setup.py` & `morphic-util-0.0.8/setup.py`

 * *Files identical despite different names*

