# Comparing `tmp/xmindtotestcase-1.6.0.tar.gz` & `tmp/xmindtotestcase-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmindtotestcase-1.6.0.tar", last modified: Tue Jul 11 11:50:35 2023, max compression
+gzip compressed data, was "xmindtotestcase-1.7.0.tar", last modified: Tue Jul 25 06:51:29 2023, max compression
```

## Comparing `xmindtotestcase-1.6.0.tar` & `xmindtotestcase-1.7.0.tar`

### file list

```diff
@@ -1,61 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 11:50:35.017063 xmindtotestcase-1.6.0/
--rw-rw-rw-   0        0        0     1136 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/LICENSE
--rw-rw-rw-   0        0        0    25517 2023-07-11 11:50:35.016065 xmindtotestcase-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0    24893 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-11 11:50:35.017063 xmindtotestcase-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0     3015 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 11:50:34.916523 xmindtotestcase-1.6.0/webtool/
--rw-rw-rw-   0        0        0        0 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/__init__.py
--rw-rw-rw-   0        0        0     9101 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/application.py
--rw-rw-rw-   0        0        0      197 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/schema.sql
-drwxrwxrwx   0        0        0        0 2023-07-11 11:50:34.918538 xmindtotestcase-1.6.0/webtool/static/
-drwxrwxrwx   0        0        0        0 2023-07-11 11:50:34.923547 xmindtotestcase-1.6.0/webtool/static/css/
--rw-rw-rw-   0        0        0     4766 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/static/css/custom.css
--rw-rw-rw-   0        0        0    16459 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/static/css/pure-min.css
--rw-rw-rw-   0        0        0    12597 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/static/css/style.css
--rw-rw-rw-   0        0        0   400234 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/static/favicon.ico
-drwxrwxrwx   0        0        0        0 2023-07-11 11:50:34.978798 xmindtotestcase-1.6.0/webtool/static/guide/
--rw-rw-rw-   0        0        0   318068 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/static/guide/XMind测试用例模板.xmind
--rw-rw-rw-   0        0        0    89562 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/static/guide/demo1_convert_result.png
--rw-rw-rw-   0        0        0   181743 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/static/guide/demo2_convert_result.png
--rw-rw-rw-   0        0        0  3469172 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/static/guide/index.html
--rw-rw-rw-   0        0        0     4220 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/static/guide/index.md
--rw-rw-rw-   0        0        0    50330 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/static/guide/pypi_upload.png
--rw-rw-rw-   0        0        0   127323 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/static/guide/testcase_json_demo.png
--rw-rw-rw-   0        0        0   135690 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/static/guide/testcase_template_demo1.png
--rw-rw-rw-   0        0        0   199584 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/static/guide/testcase_template_demo2.png
--rw-rw-rw-   0        0        0   234696 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/static/guide/testcase_template_demo3.png
--rw-rw-rw-   0        0        0   247027 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/static/guide/testlink.png
--rw-rw-rw-   0        0        0   113671 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/static/guide/testlink_import_result.png
--rw-rw-rw-   0        0        0    41332 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/static/guide/testlink_select_file.png
--rw-rw-rw-   0        0        0   214625 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/static/guide/testlink_testcase_view.png
--rw-rw-rw-   0        0        0    77043 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/static/guide/testsuite_json_demo.png
--rw-rw-rw-   0        0        0   192838 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/static/guide/webtool.png
--rw-rw-rw-   0        0        0    73746 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/static/guide/webtool_cli.png
--rw-rw-rw-   0        0        0   137563 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/static/guide/xmind_testcase_demo.png
--rw-rw-rw-   0        0        0   104277 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/static/guide/xmind_testcase_template_rule.png
--rw-rw-rw-   0        0        0   204102 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/static/guide/xmind_testcase_template_rule1.png
--rw-rw-rw-   0        0        0   168478 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/static/guide/xmind_to_testcase_preview.png
--rw-rw-rw-   0        0        0   206437 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/static/guide/zentao_import_file.png
--rw-rw-rw-   0        0        0   328755 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/static/guide/zentao_import_result.png
--rw-rw-rw-   0        0        0   105100 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/static/guide/zentao_testcase_template.png
-drwxrwxrwx   0        0        0        0 2023-07-11 11:50:34.981912 xmindtotestcase-1.6.0/webtool/templates/
--rw-rw-rw-   0        0        0     3399 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/templates/index.html
--rw-rw-rw-   0        0        0     3542 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/webtool/templates/preview.html
-drwxrwxrwx   0        0        0        0 2023-07-11 11:50:35.000240 xmindtotestcase-1.6.0/xmind2testcase/
--rw-rw-rw-   0        0        0      452 2023-07-11 11:33:52.000000 xmindtotestcase-1.6.0/xmind2testcase/__about__.py
--rw-rw-rw-   0        0        0        0 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/xmind2testcase/__init__.py
--rw-rw-rw-   0        0        0     3390 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/xmind2testcase/cli.py
--rw-rw-rw-   0        0        0      647 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/xmind2testcase/const.py
--rw-rw-rw-   0        0        0     4284 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/xmind2testcase/metadata.py
--rw-rw-rw-   0        0        0     8465 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/xmind2testcase/parser.py
--rw-rw-rw-   0        0        0     6575 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/xmind2testcase/testlink.py
--rw-rw-rw-   0        0        0     5817 2023-07-11 11:25:22.000000 xmindtotestcase-1.6.0/xmind2testcase/utils.py
--rw-rw-rw-   0        0        0     3461 2023-07-11 11:33:56.000000 xmindtotestcase-1.6.0/xmind2testcase/zentao.py
-drwxrwxrwx   0        0        0        0 2023-07-11 11:50:35.014063 xmindtotestcase-1.6.0/xmindtotestcase.egg-info/
--rw-rw-rw-   0        0        0    25517 2023-07-11 11:50:34.000000 xmindtotestcase-1.6.0/xmindtotestcase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1800 2023-07-11 11:50:34.000000 xmindtotestcase-1.6.0/xmindtotestcase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 11:50:34.000000 xmindtotestcase-1.6.0/xmindtotestcase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-07-11 11:50:34.000000 xmindtotestcase-1.6.0/xmindtotestcase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       18 2023-07-11 11:50:34.000000 xmindtotestcase-1.6.0/xmindtotestcase.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-07-11 11:50:34.000000 xmindtotestcase-1.6.0/xmindtotestcase.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 06:51:29.333893 xmindtotestcase-1.7.0/
+-rw-rw-rw-   0        0        0     1136 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/LICENSE
+-rw-rw-rw-   0        0        0    25619 2023-07-25 06:51:29.332896 xmindtotestcase-1.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0    24951 2023-07-22 15:29:42.000000 xmindtotestcase-1.7.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-25 06:51:29.333893 xmindtotestcase-1.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     3015 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:51:29.081041 xmindtotestcase-1.7.0/testcase2xmind/
+-rw-rw-rw-   0        0        0        0 2023-07-15 14:42:06.000000 xmindtotestcase-1.7.0/testcase2xmind/__init__.py
+-rw-rw-rw-   0        0        0     2729 2023-07-25 06:18:25.000000 xmindtotestcase-1.7.0/testcase2xmind/zentao2xmind.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:51:29.086030 xmindtotestcase-1.7.0/webtool/
+-rw-rw-rw-   0        0        0        0 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/__init__.py
+-rw-rw-rw-   0        0        0    23134 2023-07-24 06:07:11.000000 xmindtotestcase-1.7.0/webtool/application.py
+-rw-rw-rw-   0        0        0      197 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/schema.sql
+drwxrwxrwx   0        0        0        0 2023-07-25 06:51:29.088024 xmindtotestcase-1.7.0/webtool/static/
+drwxrwxrwx   0        0        0        0 2023-07-25 06:51:29.110962 xmindtotestcase-1.7.0/webtool/static/css/
+-rw-rw-rw-   0        0        0     4766 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/static/css/custom.css
+-rw-rw-rw-   0        0        0    16459 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/static/css/pure-min.css
+-rw-rw-rw-   0        0        0    12597 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/static/css/style.css
+-rw-rw-rw-   0        0        0   400234 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/static/favicon.ico
+drwxrwxrwx   0        0        0        0 2023-07-25 06:51:29.297989 xmindtotestcase-1.7.0/webtool/static/guide/
+-rw-rw-rw-   0        0        0   318068 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/static/guide/XMind测试用例模板.xmind
+-rw-rw-rw-   0        0        0    89562 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/static/guide/demo1_convert_result.png
+-rw-rw-rw-   0        0        0   181743 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/static/guide/demo2_convert_result.png
+-rw-rw-rw-   0        0        0  3469172 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/static/guide/index.html
+-rw-rw-rw-   0        0        0     4220 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/static/guide/index.md
+-rw-rw-rw-   0        0        0    50330 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/static/guide/pypi_upload.png
+-rw-rw-rw-   0        0        0   127323 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/static/guide/testcase_json_demo.png
+-rw-rw-rw-   0        0        0   135690 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/static/guide/testcase_template_demo1.png
+-rw-rw-rw-   0        0        0   199584 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/static/guide/testcase_template_demo2.png
+-rw-rw-rw-   0        0        0   234696 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/static/guide/testcase_template_demo3.png
+-rw-rw-rw-   0        0        0   247027 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/static/guide/testlink.png
+-rw-rw-rw-   0        0        0   113671 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/static/guide/testlink_import_result.png
+-rw-rw-rw-   0        0        0    41332 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/static/guide/testlink_select_file.png
+-rw-rw-rw-   0        0        0   214625 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/static/guide/testlink_testcase_view.png
+-rw-rw-rw-   0        0        0    77043 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/static/guide/testsuite_json_demo.png
+-rw-rw-rw-   0        0        0   192838 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/static/guide/webtool.png
+-rw-rw-rw-   0        0        0    73746 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/static/guide/webtool_cli.png
+-rw-rw-rw-   0        0        0   137563 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/static/guide/xmind_testcase_demo.png
+-rw-rw-rw-   0        0        0   104277 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/static/guide/xmind_testcase_template_rule.png
+-rw-rw-rw-   0        0        0   204102 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/static/guide/xmind_testcase_template_rule1.png
+-rw-rw-rw-   0        0        0   168478 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/static/guide/xmind_to_testcase_preview.png
+-rw-rw-rw-   0        0        0   206437 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/static/guide/zentao_import_file.png
+-rw-rw-rw-   0        0        0   328755 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/static/guide/zentao_import_result.png
+-rw-rw-rw-   0        0        0   105100 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/static/guide/zentao_testcase_template.png
+drwxrwxrwx   0        0        0        0 2023-07-25 06:51:29.301979 xmindtotestcase-1.7.0/webtool/templates/
+-rw-rw-rw-   0        0        0     3399 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/templates/index.html
+-rw-rw-rw-   0        0        0     3542 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/webtool/templates/preview.html
+drwxrwxrwx   0        0        0        0 2023-07-25 06:51:29.318933 xmindtotestcase-1.7.0/xmind2testcase/
+-rw-rw-rw-   0        0        0      498 2023-07-25 06:43:22.000000 xmindtotestcase-1.7.0/xmind2testcase/__about__.py
+-rw-rw-rw-   0        0        0        0 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/xmind2testcase/__init__.py
+-rw-rw-rw-   0        0        0     4015 2023-07-25 06:33:21.000000 xmindtotestcase-1.7.0/xmind2testcase/cli.py
+-rw-rw-rw-   0        0        0      647 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/xmind2testcase/const.py
+-rw-rw-rw-   0        0        0     4284 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/xmind2testcase/metadata.py
+-rw-rw-rw-   0        0        0     8465 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/xmind2testcase/parser.py
+-rw-rw-rw-   0        0        0     6575 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/xmind2testcase/testlink.py
+-rw-rw-rw-   0        0        0     5817 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/xmind2testcase/utils.py
+-rw-rw-rw-   0        0        0     3461 2023-07-11 14:37:48.000000 xmindtotestcase-1.7.0/xmind2testcase/zentao.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:51:29.330901 xmindtotestcase-1.7.0/xmindtotestcase.egg-info/
+-rw-rw-rw-   0        0        0    25619 2023-07-25 06:51:28.000000 xmindtotestcase-1.7.0/xmindtotestcase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1858 2023-07-25 06:51:29.000000 xmindtotestcase-1.7.0/xmindtotestcase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 06:51:28.000000 xmindtotestcase-1.7.0/xmindtotestcase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-07-25 06:51:28.000000 xmindtotestcase-1.7.0/xmindtotestcase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       18 2023-07-25 06:51:28.000000 xmindtotestcase-1.7.0/xmindtotestcase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       38 2023-07-25 06:51:28.000000 xmindtotestcase-1.7.0/xmindtotestcase.egg-info/top_level.txt
```

### Comparing `xmindtotestcase-1.6.0/LICENSE` & `xmindtotestcase-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/PKG-INFO` & `xmindtotestcase-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: xmindtotestcase
-Version: 1.6.0
-Summary: XMindtoTestCase基于Python实现，提供了一个高效测试用例设计的解决方案！
+Version: 1.7.0
+Summary: XMindtoTestCase基于Python实现，提供了一个高效测试用例设计的解决方案！可以实现xmind转csv，csv转xmind操作！
 Home-page: https://github.com/huc141/xmindTotestcase.git
 Author: yulong
 Author-email: 1349983371@qq.com
 License: MIT
 Keywords: xmindtotestCase, testcase, test, testing, xmind, 思维导图, XMind思维导图
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # XMind2TestCase
-
+- 适配我司禅道模板
 > **XMind2TestCase** 工具，提供了一个高效测试用例设计的解决方案！
 
 
 ### 一、背景
 
 软件测试过程中，最重要、最核心就是测试用例的设计，也是测试童鞋、测试团队日常投入最多时间的工作内容之一。
 
@@ -71,14 +71,15 @@
 
 ![zentao](https://raw.githubusercontent.com/zhuifengshen/xmind2testcase/master/webtool/static/guide/zentao_import_result.png)
 
 
 ### 三、安装方式
 ```
 pip3 install xmind2testcase
+pip3 install xmindtotestcase
 ```
 
 
 ### 四、版本升级
 ```
 pip3 install -U xmind2testcase
 ```
```

### Comparing `xmindtotestcase-1.6.0/README.md` & `xmindtotestcase-1.7.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # XMind2TestCase
-
+- 适配我司禅道模板
 > **XMind2TestCase** 工具，提供了一个高效测试用例设计的解决方案！
 
 
 ### 一、背景
 
 软件测试过程中，最重要、最核心就是测试用例的设计，也是测试童鞋、测试团队日常投入最多时间的工作内容之一。
 
@@ -55,14 +55,15 @@
 
 ![zentao](https://raw.githubusercontent.com/zhuifengshen/xmind2testcase/master/webtool/static/guide/zentao_import_result.png)
 
 
 ### 三、安装方式
 ```
 pip3 install xmind2testcase
+pip3 install xmindtotestcase
 ```
 
 
 ### 四、版本升级
 ```
 pip3 install -U xmind2testcase
 ```
@@ -610,8 +611,8 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
-```
+```
```

### Comparing `xmindtotestcase-1.6.0/setup.py` & `xmindtotestcase-1.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/webtool/static/css/custom.css` & `xmindtotestcase-1.7.0/webtool/static/css/custom.css`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/webtool/static/css/pure-min.css` & `xmindtotestcase-1.7.0/webtool/static/css/pure-min.css`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/webtool/static/css/style.css` & `xmindtotestcase-1.7.0/webtool/static/css/style.css`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/webtool/static/favicon.ico` & `xmindtotestcase-1.7.0/webtool/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/webtool/static/guide/XMind测试用例模板.xmind` & `xmindtotestcase-1.7.0/webtool/static/guide/XMind测试用例模板.xmind`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/webtool/static/guide/demo1_convert_result.png` & `xmindtotestcase-1.7.0/webtool/static/guide/demo1_convert_result.png`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/webtool/static/guide/demo2_convert_result.png` & `xmindtotestcase-1.7.0/webtool/static/guide/demo2_convert_result.png`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/webtool/static/guide/index.html` & `xmindtotestcase-1.7.0/webtool/static/guide/index.html`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/webtool/static/guide/index.md` & `xmindtotestcase-1.7.0/webtool/static/guide/index.md`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/webtool/static/guide/pypi_upload.png` & `xmindtotestcase-1.7.0/webtool/static/guide/pypi_upload.png`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/webtool/static/guide/testcase_json_demo.png` & `xmindtotestcase-1.7.0/webtool/static/guide/testcase_json_demo.png`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/webtool/static/guide/testcase_template_demo1.png` & `xmindtotestcase-1.7.0/webtool/static/guide/testcase_template_demo1.png`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/webtool/static/guide/testcase_template_demo2.png` & `xmindtotestcase-1.7.0/webtool/static/guide/testcase_template_demo2.png`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/webtool/static/guide/testcase_template_demo3.png` & `xmindtotestcase-1.7.0/webtool/static/guide/testcase_template_demo3.png`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/webtool/static/guide/testlink.png` & `xmindtotestcase-1.7.0/webtool/static/guide/testlink.png`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/webtool/static/guide/testlink_import_result.png` & `xmindtotestcase-1.7.0/webtool/static/guide/testlink_import_result.png`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/webtool/static/guide/testlink_select_file.png` & `xmindtotestcase-1.7.0/webtool/static/guide/testlink_select_file.png`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/webtool/static/guide/testlink_testcase_view.png` & `xmindtotestcase-1.7.0/webtool/static/guide/testlink_testcase_view.png`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/webtool/static/guide/testsuite_json_demo.png` & `xmindtotestcase-1.7.0/webtool/static/guide/testsuite_json_demo.png`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/webtool/static/guide/webtool.png` & `xmindtotestcase-1.7.0/webtool/static/guide/webtool.png`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/webtool/static/guide/webtool_cli.png` & `xmindtotestcase-1.7.0/webtool/static/guide/webtool_cli.png`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/webtool/static/guide/xmind_testcase_demo.png` & `xmindtotestcase-1.7.0/webtool/static/guide/xmind_testcase_demo.png`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/webtool/static/guide/xmind_testcase_template_rule.png` & `xmindtotestcase-1.7.0/webtool/static/guide/xmind_testcase_template_rule.png`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/webtool/static/guide/xmind_testcase_template_rule1.png` & `xmindtotestcase-1.7.0/webtool/static/guide/xmind_testcase_template_rule1.png`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/webtool/static/guide/xmind_to_testcase_preview.png` & `xmindtotestcase-1.7.0/webtool/static/guide/xmind_to_testcase_preview.png`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/webtool/static/guide/zentao_import_file.png` & `xmindtotestcase-1.7.0/webtool/static/guide/zentao_import_file.png`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/webtool/static/guide/zentao_import_result.png` & `xmindtotestcase-1.7.0/webtool/static/guide/zentao_import_result.png`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/webtool/static/guide/zentao_testcase_template.png` & `xmindtotestcase-1.7.0/webtool/static/guide/zentao_testcase_template.png`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/webtool/templates/index.html` & `xmindtotestcase-1.7.0/webtool/templates/index.html`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/webtool/templates/preview.html` & `xmindtotestcase-1.7.0/webtool/templates/preview.html`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/xmind2testcase/cli.py` & `xmindtotestcase-1.7.0/xmind2testcase/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python
 # _*_ coding:utf-8 _*_
 import logging
 import sys
+from testcase2xmind.zentao2xmind import zentao_csv_file_to_xmind
 from xmind2testcase.zentao import xmind_to_zentao_csv_file
 from xmind2testcase.testlink import xmind_to_testlink_xml_file
 from xmind2testcase.utils import get_absolute_path, xmind_testcase_to_json_file
 from webtool.application import launch
 
 logging.basicConfig(level=logging.INFO,
                     format='%(asctime)s  %(name)s  %(levelname)s  [%(module)s - %(funcName)s]: %(message)s',
@@ -20,14 +21,15 @@
      xmind2testcase [webtool] [port_num]
     
     Example:
      xmind2testcase /path/to/testcase.xmind        => output testcase.csv、testcase.xml、testcase.json
      xmind2testcase /path/to/testcase.xmind -csv   => output testcase.csv
      xmind2testcase /path/to/testcase.xmind -xml   => output testcase.xml
      xmind2testcase /path/to/testcase.xmind -json  => output testcase.json
+     xmind2testcase /path/to/testcase.csv -xmind   => output testcase.xmind
      xmind2testcase webtool                        => launch the web testcase conversion tool locally: 127.0.0.1:5001
      xmind2testcase webtool 8000                   => launch the web testcase conversion tool locally: 127.0.0.1:8000
     """
 
 
 def cli_main():
     if len(sys.argv) > 1 and sys.argv[1].endswith('.xmind'):
@@ -60,14 +62,21 @@
             try:
                 port = int(sys.argv[2])
                 launch(port=port)
             except ValueError:
                 launch()
         else:
             launch()
+    elif len(sys.argv) > 1 and sys.argv[1].endswith('.csv'):
+        zentao_csv_file = sys.argv[1]
+        zentao_csv_file = get_absolute_path(zentao_csv_file)
+        logging.info('Start to convert zentao_csv file: %s', zentao_csv_file)
+        if len(sys.argv) == 3 and sys.argv[2] == '-xmind':
+            csv_to_xmind_file = zentao_csv_file_to_xmind(zentao_csv_file)
+            logging.info('Convert csv_to_xmind file to xmind file successfully: %s', csv_to_xmind_file)
 
     else:
         print(using_doc)
 
 
 if __name__ == '__main__':
     cli_main()
```

### Comparing `xmindtotestcase-1.6.0/xmind2testcase/const.py` & `xmindtotestcase-1.7.0/xmind2testcase/const.py`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/xmind2testcase/metadata.py` & `xmindtotestcase-1.7.0/xmind2testcase/metadata.py`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/xmind2testcase/parser.py` & `xmindtotestcase-1.7.0/xmind2testcase/parser.py`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/xmind2testcase/testlink.py` & `xmindtotestcase-1.7.0/xmind2testcase/testlink.py`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/xmind2testcase/utils.py` & `xmindtotestcase-1.7.0/xmind2testcase/utils.py`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/xmind2testcase/zentao.py` & `xmindtotestcase-1.7.0/xmind2testcase/zentao.py`

 * *Files identical despite different names*

### Comparing `xmindtotestcase-1.6.0/xmindtotestcase.egg-info/PKG-INFO` & `xmindtotestcase-1.7.0/xmindtotestcase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: xmindtotestcase
-Version: 1.6.0
-Summary: XMindtoTestCase基于Python实现，提供了一个高效测试用例设计的解决方案！
+Version: 1.7.0
+Summary: XMindtoTestCase基于Python实现，提供了一个高效测试用例设计的解决方案！可以实现xmind转csv，csv转xmind操作！
 Home-page: https://github.com/huc141/xmindTotestcase.git
 Author: yulong
 Author-email: 1349983371@qq.com
 License: MIT
 Keywords: xmindtotestCase, testcase, test, testing, xmind, 思维导图, XMind思维导图
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # XMind2TestCase
-
+- 适配我司禅道模板
 > **XMind2TestCase** 工具，提供了一个高效测试用例设计的解决方案！
 
 
 ### 一、背景
 
 软件测试过程中，最重要、最核心就是测试用例的设计，也是测试童鞋、测试团队日常投入最多时间的工作内容之一。
 
@@ -71,14 +71,15 @@
 
 ![zentao](https://raw.githubusercontent.com/zhuifengshen/xmind2testcase/master/webtool/static/guide/zentao_import_result.png)
 
 
 ### 三、安装方式
 ```
 pip3 install xmind2testcase
+pip3 install xmindtotestcase
 ```
 
 
 ### 四、版本升级
 ```
 pip3 install -U xmind2testcase
 ```
```

### Comparing `xmindtotestcase-1.6.0/xmindtotestcase.egg-info/SOURCES.txt` & `xmindtotestcase-1.7.0/xmindtotestcase.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 LICENSE
 README.md
 setup.py
+testcase2xmind/__init__.py
+testcase2xmind/zentao2xmind.py
 webtool/__init__.py
 webtool/application.py
 webtool/schema.sql
 webtool/static/favicon.ico
 webtool/static/css/custom.css
 webtool/static/css/pure-min.css
 webtool/static/css/style.css
```

