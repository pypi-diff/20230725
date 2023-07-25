# Comparing `tmp/mwj-apitest-1.2.1.tar.gz` & `tmp/mwj-apitest-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mwj-apitest-1.2.1.tar", last modified: Tue Jul 25 07:18:50 2023, max compression
+gzip compressed data, was "mwj-apitest-1.2.2.tar", last modified: Tue Jul 25 07:31:50 2023, max compression
```

## Comparing `mwj-apitest-1.2.1.tar` & `mwj-apitest-1.2.2.tar`

### file list

```diff
@@ -1,51 +1,58 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 07:18:50.828013 mwj-apitest-1.2.1/
--rw-rw-rw-   0        0        0     1091 2023-05-31 08:57:31.000000 mwj-apitest-1.2.1/LICENSE
--rw-rw-rw-   0        0        0       66 2023-07-25 07:15:24.000000 mwj-apitest-1.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1023 2023-07-25 07:18:50.827016 mwj-apitest-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      490 2023-07-21 08:25:51.000000 mwj-apitest-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 07:18:50.785992 mwj-apitest-1.2.1/mwjApiTest/
--rw-rw-rw-   0        0        0      215 2023-05-31 09:41:04.000000 mwj-apitest-1.2.1/mwjApiTest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:18:50.796932 mwj-apitest-1.2.1/mwjApiTest/core/
--rw-rw-rw-   0        0        0      190 2023-05-31 08:48:04.000000 mwj-apitest-1.2.1/mwjApiTest/core/__init__.py
--rw-rw-rw-   0        0        0     6001 2023-07-13 09:21:04.000000 mwj-apitest-1.2.1/mwjApiTest/core/basecase.py
--rw-rw-rw-   0        0        0     5378 2023-07-12 09:40:57.000000 mwj-apitest-1.2.1/mwjApiTest/core/dataParser.py
--rw-rw-rw-   0        0        0     1456 2023-07-10 08:19:16.000000 mwj-apitest-1.2.1/mwjApiTest/core/db_client.py
--rw-rw-rw-   0        0        0     2559 2023-07-13 10:24:23.000000 mwj-apitest-1.2.1/mwjApiTest/core/env_prepare.py
--rw-rw-rw-   0        0        0     3350 2023-07-14 08:08:04.000000 mwj-apitest-1.2.1/mwjApiTest/core/generateCase.py
--rw-rw-rw-   0        0        0    22073 2023-07-21 09:16:40.000000 mwj-apitest-1.2.1/mwjApiTest/core/httptest.py
--rw-rw-rw-   0        0        0     3401 2023-07-25 05:39:14.000000 mwj-apitest-1.2.1/mwjApiTest/core/log_operation.py
--rw-rw-rw-   0        0        0     2117 2023-07-10 08:36:03.000000 mwj-apitest-1.2.1/mwjApiTest/core/make_data.py
--rw-rw-rw-   0        0        0     6781 2023-07-11 03:09:03.000000 mwj-apitest-1.2.1/mwjApiTest/core/send_report.py
--rw-rw-rw-   0        0        0    20285 2023-07-21 08:28:06.000000 mwj-apitest-1.2.1/mwjApiTest/core/testRunner.py
--rw-rw-rw-   0        0        0     6743 2023-07-25 07:18:34.000000 mwj-apitest-1.2.1/mwjApiTest/manage.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:18:50.797929 mwj-apitest-1.2.1/mwjApiTest/templates/
--rw-rw-rw-   0        0        0      190 2023-07-12 03:00:19.000000 mwj-apitest-1.2.1/mwjApiTest/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:18:50.797929 mwj-apitest-1.2.1/mwjApiTest/templates/reports/
--rw-rw-rw-   0        0        0      190 2023-07-12 03:00:19.000000 mwj-apitest-1.2.1/mwjApiTest/templates/reports/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:18:50.801692 mwj-apitest-1.2.1/mwjApiTest/templates/request_file_demo/
--rw-rw-rw-   0        0        0      190 2023-07-19 10:08:25.000000 mwj-apitest-1.2.1/mwjApiTest/templates/request_file_demo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:18:50.802689 mwj-apitest-1.2.1/mwjApiTest/templates/request_file_demo/case_json/
--rw-rw-rw-   0        0        0      190 2023-07-21 05:58:29.000000 mwj-apitest-1.2.1/mwjApiTest/templates/request_file_demo/case_json/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:18:50.804684 mwj-apitest-1.2.1/mwjApiTest/templates/request_file_demo/case_py/
--rw-rw-rw-   0        0        0      190 2023-07-21 05:58:29.000000 mwj-apitest-1.2.1/mwjApiTest/templates/request_file_demo/case_py/__init__.py
--rw-rw-rw-   0        0        0     1232 2023-07-21 08:08:11.000000 mwj-apitest-1.2.1/mwjApiTest/templates/request_file_demo/case_py/test_case_demo.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:18:50.805682 mwj-apitest-1.2.1/mwjApiTest/templates/request_file_demo/case_yaml/
--rw-rw-rw-   0        0        0      190 2023-07-21 05:58:29.000000 mwj-apitest-1.2.1/mwjApiTest/templates/request_file_demo/case_yaml/__init__.py
--rw-rw-rw-   0        0        0     3749 2023-07-14 06:35:52.000000 mwj-apitest-1.2.1/mwjApiTest/templates/request_file_demo/funcTools.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:18:50.805682 mwj-apitest-1.2.1/mwjApiTest/templates/request_file_demo/logs/
--rw-rw-rw-   0        0        0      190 2023-07-21 05:58:29.000000 mwj-apitest-1.2.1/mwjApiTest/templates/request_file_demo/logs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:18:50.806679 mwj-apitest-1.2.1/mwjApiTest/templates/request_file_demo/reports/
--rw-rw-rw-   0        0        0      190 2023-07-21 05:58:28.000000 mwj-apitest-1.2.1/mwjApiTest/templates/request_file_demo/reports/__init__.py
--rw-rw-rw-   0        0        0      223 2023-07-14 08:23:35.000000 mwj-apitest-1.2.1/mwjApiTest/templates/request_file_demo/run.py
--rw-rw-rw-   0        0        0     2117 2023-07-21 09:08:28.000000 mwj-apitest-1.2.1/mwjApiTest/templates/request_file_demo/settings.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:18:50.807676 mwj-apitest-1.2.1/mwjApiTest/utils/
--rw-rw-rw-   0        0        0      190 2023-05-31 08:48:04.000000 mwj-apitest-1.2.1/mwjApiTest/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:18:50.826018 mwj-apitest-1.2.1/mwj_apitest.egg-info/
--rw-rw-rw-   0        0        0     1023 2023-07-25 07:18:50.000000 mwj-apitest-1.2.1/mwj_apitest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1287 2023-07-25 07:18:50.000000 mwj-apitest-1.2.1/mwj_apitest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 07:18:50.000000 mwj-apitest-1.2.1/mwj_apitest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-07-25 07:18:50.000000 mwj-apitest-1.2.1/mwj_apitest.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      156 2023-07-25 07:18:50.000000 mwj-apitest-1.2.1/mwj_apitest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-25 07:18:50.000000 mwj-apitest-1.2.1/mwj_apitest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 07:18:50.828013 mwj-apitest-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1862 2023-07-25 07:18:34.000000 mwj-apitest-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 07:31:50.964727 mwj-apitest-1.2.2/
+-rw-rw-rw-   0        0        0     1091 2023-05-31 08:57:31.000000 mwj-apitest-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0      194 2023-07-25 07:31:19.000000 mwj-apitest-1.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1023 2023-07-25 07:31:50.963730 mwj-apitest-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      490 2023-07-21 08:25:51.000000 mwj-apitest-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 07:31:50.918486 mwj-apitest-1.2.2/mwjApiTest/
+-rw-rw-rw-   0        0        0      215 2023-05-31 09:41:04.000000 mwj-apitest-1.2.2/mwjApiTest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 07:31:50.930477 mwj-apitest-1.2.2/mwjApiTest/core/
+-rw-rw-rw-   0        0        0      190 2023-05-31 08:48:04.000000 mwj-apitest-1.2.2/mwjApiTest/core/__init__.py
+-rw-rw-rw-   0        0        0     6001 2023-07-13 09:21:04.000000 mwj-apitest-1.2.2/mwjApiTest/core/basecase.py
+-rw-rw-rw-   0        0        0     5378 2023-07-12 09:40:57.000000 mwj-apitest-1.2.2/mwjApiTest/core/dataParser.py
+-rw-rw-rw-   0        0        0     1456 2023-07-10 08:19:16.000000 mwj-apitest-1.2.2/mwjApiTest/core/db_client.py
+-rw-rw-rw-   0        0        0     2559 2023-07-13 10:24:23.000000 mwj-apitest-1.2.2/mwjApiTest/core/env_prepare.py
+-rw-rw-rw-   0        0        0     3350 2023-07-14 08:08:04.000000 mwj-apitest-1.2.2/mwjApiTest/core/generateCase.py
+-rw-rw-rw-   0        0        0    22073 2023-07-21 09:16:40.000000 mwj-apitest-1.2.2/mwjApiTest/core/httptest.py
+-rw-rw-rw-   0        0        0     3401 2023-07-25 05:39:14.000000 mwj-apitest-1.2.2/mwjApiTest/core/log_operation.py
+-rw-rw-rw-   0        0        0     2117 2023-07-10 08:36:03.000000 mwj-apitest-1.2.2/mwjApiTest/core/make_data.py
+-rw-rw-rw-   0        0        0     6781 2023-07-11 03:09:03.000000 mwj-apitest-1.2.2/mwjApiTest/core/send_report.py
+-rw-rw-rw-   0        0        0    20285 2023-07-21 08:28:06.000000 mwj-apitest-1.2.2/mwjApiTest/core/testRunner.py
+-rw-rw-rw-   0        0        0     6743 2023-07-25 07:31:32.000000 mwj-apitest-1.2.2/mwjApiTest/manage.py
+drwxrwxrwx   0        0        0        0 2023-07-25 07:31:50.930477 mwj-apitest-1.2.2/mwjApiTest/templates/
+-rw-rw-rw-   0        0        0      190 2023-07-12 03:00:19.000000 mwj-apitest-1.2.2/mwjApiTest/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 07:31:50.938432 mwj-apitest-1.2.2/mwjApiTest/templates/reports/
+-rw-rw-rw-   0        0        0      190 2023-07-12 03:00:19.000000 mwj-apitest-1.2.2/mwjApiTest/templates/reports/__init__.py
+-rw-rw-rw-   0        0        0      318 2023-07-12 03:29:46.000000 mwj-apitest-1.2.2/mwjApiTest/templates/reports/dingtalk_templates.md
+-rw-rw-rw-   0        0        0     2464 2023-05-31 08:08:20.000000 mwj-apitest-1.2.2/mwjApiTest/templates/reports/templates03.html
+-rw-rw-rw-   0        0        0    39651 2023-05-31 08:08:20.000000 mwj-apitest-1.2.2/mwjApiTest/templates/reports/templates1.html
+-rw-rw-rw-   0        0        0    29220 2023-05-31 08:08:20.000000 mwj-apitest-1.2.2/mwjApiTest/templates/reports/templates2.html
+-rw-rw-rw-   0        0        0    22204 2023-05-31 08:08:20.000000 mwj-apitest-1.2.2/mwjApiTest/templates/reports/templates3.html
+drwxrwxrwx   0        0        0        0 2023-07-25 07:31:50.941486 mwj-apitest-1.2.2/mwjApiTest/templates/request_file_demo/
+-rw-rw-rw-   0        0        0      190 2023-07-19 10:08:25.000000 mwj-apitest-1.2.2/mwjApiTest/templates/request_file_demo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 07:31:50.942486 mwj-apitest-1.2.2/mwjApiTest/templates/request_file_demo/case_json/
+-rw-rw-rw-   0        0        0      190 2023-07-21 05:58:29.000000 mwj-apitest-1.2.2/mwjApiTest/templates/request_file_demo/case_json/__init__.py
+-rw-rw-rw-   0        0        0      763 2023-07-21 08:08:11.000000 mwj-apitest-1.2.2/mwjApiTest/templates/request_file_demo/case_json/test_json_demo.json
+drwxrwxrwx   0        0        0        0 2023-07-25 07:31:50.943781 mwj-apitest-1.2.2/mwjApiTest/templates/request_file_demo/case_py/
+-rw-rw-rw-   0        0        0      190 2023-07-21 05:58:29.000000 mwj-apitest-1.2.2/mwjApiTest/templates/request_file_demo/case_py/__init__.py
+-rw-rw-rw-   0        0        0     1232 2023-07-21 08:08:11.000000 mwj-apitest-1.2.2/mwjApiTest/templates/request_file_demo/case_py/test_case_demo.py
+drwxrwxrwx   0        0        0        0 2023-07-25 07:31:50.945809 mwj-apitest-1.2.2/mwjApiTest/templates/request_file_demo/case_yaml/
+-rw-rw-rw-   0        0        0      190 2023-07-21 05:58:29.000000 mwj-apitest-1.2.2/mwjApiTest/templates/request_file_demo/case_yaml/__init__.py
+-rw-rw-rw-   0        0        0      742 2023-07-21 08:08:11.000000 mwj-apitest-1.2.2/mwjApiTest/templates/request_file_demo/case_yaml/test_case_demo.yaml
+-rw-rw-rw-   0        0        0     3749 2023-07-14 06:35:52.000000 mwj-apitest-1.2.2/mwjApiTest/templates/request_file_demo/funcTools.py
+drwxrwxrwx   0        0        0        0 2023-07-25 07:31:50.945809 mwj-apitest-1.2.2/mwjApiTest/templates/request_file_demo/logs/
+-rw-rw-rw-   0        0        0      190 2023-07-21 05:58:29.000000 mwj-apitest-1.2.2/mwjApiTest/templates/request_file_demo/logs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 07:31:50.946804 mwj-apitest-1.2.2/mwjApiTest/templates/request_file_demo/reports/
+-rw-rw-rw-   0        0        0      190 2023-07-21 05:58:28.000000 mwj-apitest-1.2.2/mwjApiTest/templates/request_file_demo/reports/__init__.py
+-rw-rw-rw-   0        0        0      223 2023-07-14 08:23:35.000000 mwj-apitest-1.2.2/mwjApiTest/templates/request_file_demo/run.py
+-rw-rw-rw-   0        0        0     2117 2023-07-21 09:08:28.000000 mwj-apitest-1.2.2/mwjApiTest/templates/request_file_demo/settings.py
+drwxrwxrwx   0        0        0        0 2023-07-25 07:31:50.948770 mwj-apitest-1.2.2/mwjApiTest/utils/
+-rw-rw-rw-   0        0        0      190 2023-05-31 08:48:04.000000 mwj-apitest-1.2.2/mwjApiTest/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 07:31:50.962743 mwj-apitest-1.2.2/mwj_apitest.egg-info/
+-rw-rw-rw-   0        0        0     1023 2023-07-25 07:31:50.000000 mwj-apitest-1.2.2/mwj_apitest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1657 2023-07-25 07:31:50.000000 mwj-apitest-1.2.2/mwj_apitest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 07:31:50.000000 mwj-apitest-1.2.2/mwj_apitest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-07-25 07:31:50.000000 mwj-apitest-1.2.2/mwj_apitest.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      156 2023-07-25 07:31:50.000000 mwj-apitest-1.2.2/mwj_apitest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-25 07:31:50.000000 mwj-apitest-1.2.2/mwj_apitest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 07:31:50.964727 mwj-apitest-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1862 2023-07-25 07:31:32.000000 mwj-apitest-1.2.2/setup.py
```

### Comparing `mwj-apitest-1.2.1/LICENSE` & `mwj-apitest-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mwj-apitest-1.2.1/PKG-INFO` & `mwj-apitest-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwj-apitest
-Version: 1.2.1
+Version: 1.2.2
 Summary: 无需编码的接口测试框架,目前支持json、yaml、py文件格式的用例,命令行mwj查看帮助。
 Home-page: https://github.com/Lvan826199/mwjApiTest
 Author: 梦无矶小仔
 Author-email: Lvan826199@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mwj-apitest-1.2.1/mwjApiTest/core/basecase.py` & `mwj-apitest-1.2.2/mwjApiTest/core/basecase.py`

 * *Files identical despite different names*

### Comparing `mwj-apitest-1.2.1/mwjApiTest/core/dataParser.py` & `mwj-apitest-1.2.2/mwjApiTest/core/dataParser.py`

 * *Files identical despite different names*

### Comparing `mwj-apitest-1.2.1/mwjApiTest/core/db_client.py` & `mwj-apitest-1.2.2/mwjApiTest/core/db_client.py`

 * *Files identical despite different names*

### Comparing `mwj-apitest-1.2.1/mwjApiTest/core/env_prepare.py` & `mwj-apitest-1.2.2/mwjApiTest/core/env_prepare.py`

 * *Files identical despite different names*

### Comparing `mwj-apitest-1.2.1/mwjApiTest/core/generateCase.py` & `mwj-apitest-1.2.2/mwjApiTest/core/generateCase.py`

 * *Files identical despite different names*

### Comparing `mwj-apitest-1.2.1/mwjApiTest/core/httptest.py` & `mwj-apitest-1.2.2/mwjApiTest/core/httptest.py`

 * *Files identical despite different names*

### Comparing `mwj-apitest-1.2.1/mwjApiTest/core/log_operation.py` & `mwj-apitest-1.2.2/mwjApiTest/core/log_operation.py`

 * *Files identical despite different names*

### Comparing `mwj-apitest-1.2.1/mwjApiTest/core/make_data.py` & `mwj-apitest-1.2.2/mwjApiTest/core/make_data.py`

 * *Files identical despite different names*

### Comparing `mwj-apitest-1.2.1/mwjApiTest/core/send_report.py` & `mwj-apitest-1.2.2/mwjApiTest/core/send_report.py`

 * *Files identical despite different names*

### Comparing `mwj-apitest-1.2.1/mwjApiTest/core/testRunner.py` & `mwj-apitest-1.2.2/mwjApiTest/core/testRunner.py`

 * *Files identical despite different names*

### Comparing `mwj-apitest-1.2.1/mwjApiTest/manage.py` & `mwj-apitest-1.2.2/mwjApiTest/manage.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
             else:
                 log.error("测试结果推送到企业微信失败！错误信息： {}".format(res["errmsg"]))
     return res
 
 def create_parser():
     parser = argparse.ArgumentParser(prog='mwjApiTest', description='梦无矶接口测试框架使用介绍')
     # 添加版本号
-    parser.add_argument('-V', '--version', action='version', version='%(prog)s 1.2.1')
+    parser.add_argument('-V', '--version', action='version', version='%(prog)s 1.2.2')
     subparsers = parser.add_subparsers(title='Command', metavar="命令")
     # 创建项目命令
     create_cmd = subparsers.add_parser('create', help=" 创建测试项目 ", aliases=['C'])
     create_cmd.add_argument('name', metavar='project_name', help=" 项目名称 ")
     create_cmd.set_defaults(func=create)
     # 运行项目命令
     parser_run = subparsers.add_parser('run', help=' 开始运行项目 ', aliases=['R'])
```

### Comparing `mwj-apitest-1.2.1/mwjApiTest/templates/request_file_demo/case_py/test_case_demo.py` & `mwj-apitest-1.2.2/mwjApiTest/templates/request_file_demo/case_py/test_case_demo.py`

 * *Files identical despite different names*

### Comparing `mwj-apitest-1.2.1/mwjApiTest/templates/request_file_demo/funcTools.py` & `mwj-apitest-1.2.2/mwjApiTest/templates/request_file_demo/funcTools.py`

 * *Files identical despite different names*

### Comparing `mwj-apitest-1.2.1/mwjApiTest/templates/request_file_demo/settings.py` & `mwj-apitest-1.2.2/mwjApiTest/templates/request_file_demo/settings.py`

 * *Files identical despite different names*

### Comparing `mwj-apitest-1.2.1/mwj_apitest.egg-info/PKG-INFO` & `mwj-apitest-1.2.2/mwj_apitest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwj-apitest
-Version: 1.2.1
+Version: 1.2.2
 Summary: 无需编码的接口测试框架,目前支持json、yaml、py文件格式的用例,命令行mwj查看帮助。
 Home-page: https://github.com/Lvan826199/mwjApiTest
 Author: 梦无矶小仔
 Author-email: Lvan826199@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mwj-apitest-1.2.1/mwj_apitest.egg-info/SOURCES.txt` & `mwj-apitest-1.2.2/mwj_apitest.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -13,22 +13,29 @@
 mwjApiTest/core/httptest.py
 mwjApiTest/core/log_operation.py
 mwjApiTest/core/make_data.py
 mwjApiTest/core/send_report.py
 mwjApiTest/core/testRunner.py
 mwjApiTest/templates/__init__.py
 mwjApiTest/templates/reports/__init__.py
+mwjApiTest/templates/reports/dingtalk_templates.md
+mwjApiTest/templates/reports/templates03.html
+mwjApiTest/templates/reports/templates1.html
+mwjApiTest/templates/reports/templates2.html
+mwjApiTest/templates/reports/templates3.html
 mwjApiTest/templates/request_file_demo/__init__.py
 mwjApiTest/templates/request_file_demo/funcTools.py
 mwjApiTest/templates/request_file_demo/run.py
 mwjApiTest/templates/request_file_demo/settings.py
 mwjApiTest/templates/request_file_demo/case_json/__init__.py
+mwjApiTest/templates/request_file_demo/case_json/test_json_demo.json
 mwjApiTest/templates/request_file_demo/case_py/__init__.py
 mwjApiTest/templates/request_file_demo/case_py/test_case_demo.py
 mwjApiTest/templates/request_file_demo/case_yaml/__init__.py
+mwjApiTest/templates/request_file_demo/case_yaml/test_case_demo.yaml
 mwjApiTest/templates/request_file_demo/logs/__init__.py
 mwjApiTest/templates/request_file_demo/reports/__init__.py
 mwjApiTest/utils/__init__.py
 mwj_apitest.egg-info/PKG-INFO
 mwj_apitest.egg-info/SOURCES.txt
 mwj_apitest.egg-info/dependency_links.txt
 mwj_apitest.egg-info/entry_points.txt
```

### Comparing `mwj-apitest-1.2.1/setup.py` & `mwj-apitest-1.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mwj-apitest",  # 用自己的名替换其中的YOUR_USERNAME_
-    version="1.2.1",  # 包版本号，便于维护版本,保证每次发布都是版本都是唯一的
+    version="1.2.2",  # 包版本号，便于维护版本,保证每次发布都是版本都是唯一的
     author="梦无矶小仔",  # 作者，可以写自己的姓名
     author_email="Lvan826199@163.com",  # 作者联系方式，可写自己的邮箱地址
     description="无需编码的接口测试框架,目前支持json、yaml、py文件格式的用例,命令行mwj查看帮助。",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/Lvan826199/mwjApiTest",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

