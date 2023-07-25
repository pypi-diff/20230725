# Comparing `tmp/huhk-1.7.4.tar.gz` & `tmp/huhk-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhk-1.7.4.tar", last modified: Mon Jul 24 01:11:56 2023, max compression
+gzip compressed data, was "huhk-1.7.5.tar", last modified: Tue Jul 25 01:37:45 2023, max compression
```

## Comparing `huhk-1.7.4.tar` & `huhk-1.7.5.tar`

### file list

```diff
@@ -1,93 +1,107 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 01:11:56.037210 huhk-1.7.4/
--rw-rw-rw-   0        0        0      223 2023-07-24 01:11:56.036212 huhk-1.7.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-24 01:11:55.855955 huhk-1.7.4/huhk/
--rw-rw-rw-   0        0        0      772 2023-07-17 02:44:39.000000 huhk-1.7.4/huhk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:11:55.893446 huhk-1.7.4/huhk/case_project/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.7.4/huhk/case_project/__init__.py
--rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.7.4/huhk/case_project/json_coder.py
--rw-rw-rw-   0        0        0      790 2023-07-13 02:39:46.000000 huhk-1.7.4/huhk/case_project/main.py
--rw-rw-rw-   0        0        0    17724 2023-07-22 12:10:44.000000 huhk-1.7.4/huhk/case_project/project_base.py
--rw-rw-rw-   0        0        0     2099 2023-07-21 08:18:22.000000 huhk-1.7.4/huhk/case_project/project_init.py
--rw-rw-rw-   0        0        0    13835 2023-07-22 10:45:49.000000 huhk-1.7.4/huhk/case_project/project_string.py
--rw-rw-rw-   0        0        0      908 2023-07-12 01:13:24.000000 huhk-1.7.4/huhk/case_project/setup_set.py
--rw-rw-rw-   0        0        0       17 2023-07-24 01:11:55.000000 huhk-1.7.4/huhk/case_project/version.py
--rw-rw-rw-   0        0        0    13183 2023-07-22 06:53:58.000000 huhk-1.7.4/huhk/init_project.py
--rw-rw-rw-   0        0        0      274 2023-07-12 01:13:24.000000 huhk-1.7.4/huhk/setup_run.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:11:55.897403 huhk-1.7.4/huhk/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.7.4/huhk/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:11:55.952270 huhk-1.7.4/huhk/testcase/apache/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.7.4/huhk/testcase/apache/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.7.4/huhk/testcase/apache/beam_class.py
--rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.7.4/huhk/testcase/apache/data.py
--rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.7.4/huhk/testcase/apache/par_do.py
--rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.7.4/huhk/testcase/apache/test_cogroupbykey.py
--rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.7.4/huhk/testcase/apache/test_file.py
--rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.7.4/huhk/testcase/apache/test_fiter.py
--rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.7.4/huhk/testcase/apache/test_flatmap.py
--rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.7.4/huhk/testcase/apache/test_map.py
--rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.7.4/huhk/testcase/apache/test_par_do.py
--rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.7.4/huhk/testcase/apache/test_regex.py
--rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.7.4/huhk/testcase/apache/test_time.py
--rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.7.4/huhk/testcase/apache/test_to_string.py
--rw-rw-rw-   0        0        0    22615 2023-07-14 06:52:17.000000 huhk-1.7.4/huhk/unit_apache_beam.py
--rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.7.4/huhk/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.7.4/huhk/unit_encryption.py
--rw-rw-rw-   0        0        0    28445 2023-07-22 10:41:46.000000 huhk-1.7.4/huhk/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.7.4/huhk/unit_logger.py
--rw-rw-rw-   0        0        0     9960 2023-07-22 07:06:52.000000 huhk-1.7.4/huhk/unit_request.py
--rw-rw-rw-   0        0        0     2473 2023-07-12 01:13:24.000000 huhk-1.7.4/huhk/unit_tasks.py
--rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.7.4/huhk/常用命令.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:11:55.868899 huhk-1.7.4/huhk.egg-info/
--rw-rw-rw-   0        0        0      223 2023-07-24 01:11:55.000000 huhk-1.7.4/huhk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2382 2023-07-24 01:11:55.000000 huhk-1.7.4/huhk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 01:11:55.000000 huhk-1.7.4/huhk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-07-24 01:11:55.000000 huhk-1.7.4/huhk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      134 2023-07-24 01:11:55.000000 huhk-1.7.4/huhk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-24 01:11:55.000000 huhk-1.7.4/huhk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-24 01:11:55.955249 huhk-1.7.4/service/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.4/service/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:11:55.962850 huhk-1.7.4/service/app_t/
--rw-rw-rw-   0        0        0      420 2023-07-22 06:54:11.000000 huhk-1.7.4/service/app_t/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:11:55.964806 huhk-1.7.4/service/app_t/apis/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.4/service/app_t/apis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:11:55.967796 huhk-1.7.4/service/app_t/apis/open/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/apis/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:11:55.975775 huhk-1.7.4/service/app_t/apis/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/apis/open/haohan/__init__.py
--rw-rw-rw-   0        0        0    14382 2023-07-22 12:06:26.000000 huhk-1.7.4/service/app_t/apis/open/haohan/apis_open_haohan_relation.py
--rw-rw-rw-   0        0        0    15042 2023-07-22 12:06:26.000000 huhk-1.7.4/service/app_t/apis/open/haohan/apis_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:11:55.983775 huhk-1.7.4/service/app_t/apis/points/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/apis/points/__init__.py
--rw-rw-rw-   0        0        0    21382 2023-07-22 12:06:26.000000 huhk-1.7.4/service/app_t/apis/points/apis_points_points.py
--rw-rw-rw-   0        0        0    17216 2023-07-22 12:06:26.000000 huhk-1.7.4/service/app_t/apis/points/apis_points_pointsApp.py
--rw-rw-rw-   0        0        0      650 2023-07-22 10:57:15.000000 huhk-1.7.4/service/app_t/app_t_fun.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:11:55.985748 huhk-1.7.4/service/app_t/asserts/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.4/service/app_t/asserts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:11:55.988338 huhk-1.7.4/service/app_t/asserts/open/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/asserts/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:11:55.997344 huhk-1.7.4/service/app_t/asserts/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/asserts/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      602 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/asserts/open/haohan/asserts_open_haohan_relation.py
--rw-rw-rw-   0        0        0      590 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/asserts/open/haohan/asserts_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:11:56.006292 huhk-1.7.4/service/app_t/asserts/points/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/asserts/points/__init__.py
--rw-rw-rw-   0        0        0     1761 2023-07-22 07:08:51.000000 huhk-1.7.4/service/app_t/asserts/points/asserts_points_points.py
--rw-rw-rw-   0        0        0     1358 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/asserts/points/asserts_points_pointsApp.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:11:56.009284 huhk-1.7.4/service/app_t/sqls/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.4/service/app_t/sqls/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:11:56.012276 huhk-1.7.4/service/app_t/sqls/open/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/sqls/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:11:56.020258 huhk-1.7.4/service/app_t/sqls/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/sqls/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      571 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/sqls/open/haohan/sqls_open_haohan_relation.py
--rw-rw-rw-   0        0        0      567 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/sqls/open/haohan/sqls_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:11:56.028235 huhk-1.7.4/service/app_t/sqls/points/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/sqls/points/__init__.py
--rw-rw-rw-   0        0        0     1994 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/sqls/points/sqls_points_points.py
--rw-rw-rw-   0        0        0     1529 2023-07-22 06:51:21.000000 huhk-1.7.4/service/app_t/sqls/points/sqls_points_pointsApp.py
--rw-rw-rw-   0        0        0       42 2023-07-24 01:11:56.037210 huhk-1.7.4/setup.cfg
--rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.7.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:11:56.031227 huhk-1.7.4/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-22 07:30:21.000000 huhk-1.7.4/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:11:56.033222 huhk-1.7.4/testcase/app_t/
--rw-rw-rw-   0        0        0        0 2023-07-22 07:30:21.000000 huhk-1.7.4/testcase/app_t/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.284623 huhk-1.7.5/
+-rw-rw-rw-   0        0        0      223 2023-07-25 01:37:45.283623 huhk-1.7.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.077771 huhk-1.7.5/huhk/
+-rw-rw-rw-   0        0        0      772 2023-07-17 02:44:39.000000 huhk-1.7.5/huhk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.118174 huhk-1.7.5/huhk/case_project/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.7.5/huhk/case_project/__init__.py
+-rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.7.5/huhk/case_project/json_coder.py
+-rw-rw-rw-   0        0        0     1223 2023-07-25 01:24:26.000000 huhk-1.7.5/huhk/case_project/main.py
+-rw-rw-rw-   0        0        0      297 2023-07-25 01:19:15.000000 huhk-1.7.5/huhk/case_project/main_fun.py
+-rw-rw-rw-   0        0        0    17758 2023-07-24 09:52:23.000000 huhk-1.7.5/huhk/case_project/project_base.py
+-rw-rw-rw-   0        0        0     2099 2023-07-21 08:18:22.000000 huhk-1.7.5/huhk/case_project/project_init.py
+-rw-rw-rw-   0        0        0    13835 2023-07-24 01:29:57.000000 huhk-1.7.5/huhk/case_project/project_string.py
+-rw-rw-rw-   0        0        0      908 2023-07-12 01:13:24.000000 huhk-1.7.5/huhk/case_project/setup_set.py
+-rw-rw-rw-   0        0        0       17 2023-07-25 01:37:44.000000 huhk-1.7.5/huhk/case_project/version.py
+-rw-rw-rw-   0        0        0    13598 2023-07-24 09:53:49.000000 huhk-1.7.5/huhk/init_project.py
+-rw-rw-rw-   0        0        0     1218 2023-07-25 01:19:15.000000 huhk-1.7.5/huhk/main.py
+-rw-rw-rw-   0        0        0      274 2023-07-12 01:13:24.000000 huhk-1.7.5/huhk/setup_run.py
+drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.122190 huhk-1.7.5/huhk/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.7.5/huhk/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.169593 huhk-1.7.5/huhk/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.7.5/huhk/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.7.5/huhk/testcase/apache/beam_class.py
+-rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.7.5/huhk/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.7.5/huhk/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.7.5/huhk/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.7.5/huhk/testcase/apache/test_file.py
+-rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.7.5/huhk/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.7.5/huhk/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.7.5/huhk/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.7.5/huhk/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.7.5/huhk/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.7.5/huhk/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.7.5/huhk/testcase/apache/test_to_string.py
+-rw-rw-rw-   0        0        0    22615 2023-07-14 06:52:17.000000 huhk-1.7.5/huhk/unit_apache_beam.py
+-rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.7.5/huhk/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.7.5/huhk/unit_encryption.py
+-rw-rw-rw-   0        0        0    28445 2023-07-22 10:41:46.000000 huhk-1.7.5/huhk/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.7.5/huhk/unit_logger.py
+-rw-rw-rw-   0        0        0     9960 2023-07-22 07:06:52.000000 huhk-1.7.5/huhk/unit_request.py
+-rw-rw-rw-   0        0        0     2511 2023-07-24 06:56:32.000000 huhk-1.7.5/huhk/unit_tasks.py
+-rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.7.5/huhk/常用命令.py
+drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.091732 huhk-1.7.5/huhk.egg-info/
+-rw-rw-rw-   0        0        0      223 2023-07-25 01:37:44.000000 huhk-1.7.5/huhk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2885 2023-07-25 01:37:44.000000 huhk-1.7.5/huhk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 01:37:44.000000 huhk-1.7.5/huhk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-25 01:37:44.000000 huhk-1.7.5/huhk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      134 2023-07-25 01:37:44.000000 huhk-1.7.5/huhk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-25 01:37:44.000000 huhk-1.7.5/huhk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.173581 huhk-1.7.5/service/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.5/service/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.178568 huhk-1.7.5/service/app_t/
+-rw-rw-rw-   0        0        0      420 2023-07-22 06:54:11.000000 huhk-1.7.5/service/app_t/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.181560 huhk-1.7.5/service/app_t/apis/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.5/service/app_t/apis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.183587 huhk-1.7.5/service/app_t/apis/open/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/apis/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.191533 huhk-1.7.5/service/app_t/apis/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/apis/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0    22236 2023-07-24 01:53:24.000000 huhk-1.7.5/service/app_t/apis/open/haohan/apis_open_haohan_relation.py
+-rw-rw-rw-   0        0        0    23259 2023-07-24 01:53:26.000000 huhk-1.7.5/service/app_t/apis/open/haohan/apis_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.200509 huhk-1.7.5/service/app_t/apis/points/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/apis/points/__init__.py
+-rw-rw-rw-   0        0        0    31535 2023-07-24 01:53:27.000000 huhk-1.7.5/service/app_t/apis/points/apis_points_points.py
+-rw-rw-rw-   0        0        0    25708 2023-07-24 01:53:27.000000 huhk-1.7.5/service/app_t/apis/points/apis_points_pointsApp.py
+-rw-rw-rw-   0        0        0      650 2023-07-22 10:57:15.000000 huhk-1.7.5/service/app_t/app_t_fun.py
+drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.203504 huhk-1.7.5/service/app_t/asserts/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.5/service/app_t/asserts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.205520 huhk-1.7.5/service/app_t/asserts/open/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/asserts/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.213522 huhk-1.7.5/service/app_t/asserts/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/asserts/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      602 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/asserts/open/haohan/asserts_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      590 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/asserts/open/haohan/asserts_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.221452 huhk-1.7.5/service/app_t/asserts/points/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/asserts/points/__init__.py
+-rw-rw-rw-   0        0        0     1761 2023-07-22 07:08:51.000000 huhk-1.7.5/service/app_t/asserts/points/asserts_points_points.py
+-rw-rw-rw-   0        0        0     1358 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/asserts/points/asserts_points_pointsApp.py
+drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.234099 huhk-1.7.5/service/app_t/funs/
+-rw-rw-rw-   0        0        0        0 2023-07-24 01:53:24.000000 huhk-1.7.5/service/app_t/funs/__init__.py
+-rw-rw-rw-   0        0        0      161 2023-07-24 01:53:33.000000 huhk-1.7.5/service/app_t/funs/funs_app_t.py
+-rw-rw-rw-   0        0        0      118 2023-07-24 01:53:32.000000 huhk-1.7.5/service/app_t/funs/funs_open.py
+-rw-rw-rw-   0        0        0      230 2023-07-24 01:53:33.000000 huhk-1.7.5/service/app_t/funs/funs_points.py
+drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.242066 huhk-1.7.5/service/app_t/funs/open/
+-rw-rw-rw-   0        0        0        0 2023-07-24 01:53:27.000000 huhk-1.7.5/service/app_t/funs/open/__init__.py
+-rw-rw-rw-   0        0        0      267 2023-07-24 01:53:31.000000 huhk-1.7.5/service/app_t/funs/open/funs_open_haohan.py
+drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.251046 huhk-1.7.5/service/app_t/funs/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-24 01:53:27.000000 huhk-1.7.5/service/app_t/funs/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      824 2023-07-24 01:53:27.000000 huhk-1.7.5/service/app_t/funs/open/haohan/funs_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      910 2023-07-24 01:53:31.000000 huhk-1.7.5/service/app_t/funs/open/haohan/funs_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.259026 huhk-1.7.5/service/app_t/funs/points/
+-rw-rw-rw-   0        0        0        0 2023-07-24 01:53:32.000000 huhk-1.7.5/service/app_t/funs/points/__init__.py
+-rw-rw-rw-   0        0        0     3103 2023-07-24 01:53:34.000000 huhk-1.7.5/service/app_t/funs/points/funs_points_points.py
+-rw-rw-rw-   0        0        0     1899 2023-07-24 01:53:33.000000 huhk-1.7.5/service/app_t/funs/points/funs_points_pointsApp.py
+drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.262018 huhk-1.7.5/service/app_t/sqls/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.5/service/app_t/sqls/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.263973 huhk-1.7.5/service/app_t/sqls/open/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/sqls/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.272648 huhk-1.7.5/service/app_t/sqls/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/sqls/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      571 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/sqls/open/haohan/sqls_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      567 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/sqls/open/haohan/sqls_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.280632 huhk-1.7.5/service/app_t/sqls/points/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/sqls/points/__init__.py
+-rw-rw-rw-   0        0        0     1994 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/sqls/points/sqls_points_points.py
+-rw-rw-rw-   0        0        0     1529 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/sqls/points/sqls_points_pointsApp.py
+-rw-rw-rw-   0        0        0       42 2023-07-25 01:37:45.284623 huhk-1.7.5/setup.cfg
+-rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.7.5/setup.py
```

### Comparing `huhk-1.7.4/huhk/__init__.py` & `huhk-1.7.5/huhk/__init__.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.4/huhk/case_project/json_coder.py` & `huhk-1.7.5/huhk/case_project/json_coder.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.4/huhk/case_project/project_base.py` & `huhk-1.7.5/huhk/case_project/project_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,47 +16,55 @@
 class ProjectBase(ProjectString):
     def __init__(self, name=None, app_key=None, yapi_url=None, yapi_token=None, yapi_json_file=None, swagger_url=None):
         super().__init__(name, app_key, yapi_url, yapi_token, yapi_json_file, swagger_url)
         self.get_project()
 
     def get_service_value(self, key=None, default=None, _type=0):
         """获取项目本地变量"""
+        return self._get_service_value(key=key, default=default, name=self.name, _type=_type)
+
+    @staticmethod
+    def _get_service_value(key=None, default=None, name=None, _type=0):
         if _type == 0:
-            service_json_path = os.path.join(self.path.dir, "service", self.name, self.name + "_setting.json")
+            service_json_path = os.path.join(projects_path, "service", name, name + "_setting.json")
             if os.path.exists(service_json_path):
                 with open(service_json_path, encoding="utf-8") as fp:
                     data = json.load(fp)
                     if key:
                         if data.get(key):
                             return data[key]
                     else:
                         return data
 
-        service_json_path = os.path.join(self.path.dir, "service", "setting.json")
+        service_json_path = os.path.join(projects_path, "service", "setting.json")
         if os.path.exists(service_json_path):
             with open(service_json_path, encoding="utf-8") as fp:
                 data = json.load(fp)
                 return data.get(key, default) if key else data
         return default
 
-    def set_service_value(self, key, value, _type=0):
-        """设置项目本地变量"""
+    @staticmethod
+    def _set_service_value(key, value, name=None, _type=0):
         if _type == 0:
-            service_json_path = os.path.join(self.path.dir, "service", self.name, self.name + "_setting.json")
+            service_json_path = os.path.join(projects_path, "service", name, name + "_setting.json")
         else:
-            service_json_path = os.path.join(self.path.dir, "service", "setting.json")
+            service_json_path = os.path.join(projects_path, "service", "setting.json")
         if os.path.exists(service_json_path):
             with open(service_json_path) as fp:
                 data = json.load(fp)
         else:
             data = {}
         data[key] = value
         with open(service_json_path, 'w') as fp:
             json.dump(data, fp, indent=4)
 
+    def set_service_value(self, key, value, _type=0):
+        """设置项目本地变量"""
+        self._set_service_value(key=key, value=value, name=self.name, _type=_type)
+
     def get_api_attribute(self, file_str, api_file):
         try:
             fun_list = re.findall(r"\ndef +([^_].+)?\((.*?)\):\s*"
                                   r"([\'\"]{3}"
                                   r"\s*(.*?)?\s*up_time=(\d+)?[\w\W]*?"
                                   r"(    params:[\w\W]*?)?(====[\w\W]*?)?"
                                   r"[\'\"]{3})?"
@@ -259,52 +267,51 @@
                 FunBase.write_file(assert_path.path, file_str)
         else:
             file_str = self.get_assert_header_str(assert_path.class_name, sql_path) + self.get_assert_fun_str(fun_name)
             FunBase.mkdir_file(assert_path.path)
             FunBase.write_file(assert_path.path, file_str)
 
     def set_api_fun_header(self, fun_name, type=1):
+        def _fun_header():
+            if type == 1:
+                new_str = f"from {fun_path.import_path} import {fun_path.class_name}\n\n\n" \
+                          f"class {fun_path2.class_name}({fun_path.class_name}):\n    pass\n\n"
+            else:
+                new_str = f"from {fun_path.import_path} import {fun_path.class_name}\n\n\n" \
+                          f"class {fun_path2.class_name}({fun_path.class_name}):\n    pass\n\n"
+            return new_str
         fun_path = self.get_path(fun_name, fun_type="funs")
-        if fun_name.count('_') > 1:
-            path = fun_path.path.rsplit('_', 1)[0] + '.py'
+        if fun_name.count('_') > 0:
+            # path = fun_path.path.rsplit('_', 1)[0] + '.py'
             fun_path2 = self.get_path(fun_name.rsplit('_', 1)[0], fun_type='funs')
+            path = fun_path2.path
             if os.path.exists(path):
                 old_str = FunBase.read_file(path)
                 old_str_l = re.findall(r'([\w\W]*?\n)(\s*class +.*\()(.*?)(\):[\w\W]*)', old_str)
                 if old_str_l:
                     old_str_l = list(old_str_l[0])
                     if fun_path.class_name not in [i.strip() for i in old_str_l[2].split(',')]:
                         old_str_l[0] += f"from {fun_path.import_path} import {fun_path.class_name}\n"
                         old_str_l[2] += f", {fun_path.class_name}"
                     new_str = "".join(old_str_l)
                 else:
-                    if type == 1:
-                        new_str = f"from {fun_path.import_path} import {fun_path.class_name}\n\n\n" \
-                                  f"class {fun_path2.class_name}All({fun_path.class_name}):\n    pass\n\n"
-                    else:
-                        new_str = f"from {fun_path.import_path} import {fun_path.class_name}\n\n\n" \
-                                  f"class {fun_path.class_name}({fun_path.class_name}):\n    pass\n\n"
+                    new_str = _fun_header()
             else:
-                if type == 1:
-                    new_str = f"from {fun_path.import_path} import {fun_path.class_name}\n\n\n" \
-                              f"class {fun_path2.class_name}All({fun_path.class_name}):\n    pass\n\n"
-                else:
-                    new_str = f"from {fun_path.import_path} import {fun_path.class_name}\n\n\n" \
-                              f"class {fun_path.class_name}({fun_path.class_name}):\n    pass\n\n"
+                new_str = _fun_header()
             FunBase.write_file(path, new_str)
-            if fun_name.count('_') > 2:
+            if fun_name.count('_') > 1:
                 self.set_api_fun_header(fun_name.rsplit('_', 1)[0], type=2)
         else:
             print("Warning")
 
     def write_api_fun(self, fun_name, _update=False):
         fun_path = self.get_path(fun_name, fun_type='funs')
 
         if os.path.exists(fun_path.path):
-            file_str = FunBase.read_file(fun_path.path)
+            file_str = FunBase.read_file(fun_path.path).replace("    pass\n", "")
             ord_str = re.findall(
                 r'\n((    @allure.step\(.*\) *\n)?    def %s\(.+\)[\w\W]*?)(\n    @allure.step\(|\n    def|$)' %
                 fun_name, file_str)
             if ord_str:
                 if _update:
                     new_str = self.get_api_fun_fun_str(fun_name)
                     file_str = file_str.replace(ord_str[0][0], new_str)
```

### Comparing `huhk-1.7.4/huhk/case_project/project_init.py` & `huhk-1.7.5/huhk/case_project/project_init.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.4/huhk/case_project/project_string.py` & `huhk-1.7.5/huhk/case_project/project_string.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         out = Dict()
         if fun_type == "api" and self.this_fun_list.api[name]:
             filename = self.this_fun_list.api[name].path
             out.path = filename
             out.class_name = None
             out.import_path = ".".join(filename.replace(self.path.dir, "").split(os.sep)[1:])[:-3]
         else:
-            filename = f"{fun_type}_{'_'.join(name_l[:-1]) if name_l[:-2] else self.name}.py".replace('__', "_")
+            filename = f"{fun_type}_{'_'.join(name_l[:-1]) if name_l[:-1] else self.name}.py".replace('__', "_")
             out.path = os.path.join(self.path.service_dir, fun_type, os.path.sep.join(name_l[:-2]), filename)
             out.class_name = filename.split(".")[0].title().replace('_', '')
             out.import_path = ".".join(["service", self.name, fun_type] + name_l[:-2] + [filename.split('.py')[0]])
         return out
 
     def get_api_header_str(self):
         api_header_str = f"import allure\n\nfrom service.{self.name} import http_requester\n" \
```

### Comparing `huhk-1.7.4/huhk/case_project/setup_set.py` & `huhk-1.7.5/huhk/case_project/setup_set.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.4/huhk/init_project.py` & `huhk-1.7.5/huhk/init_project.py`

 * *Files 3% similar despite different names*

```diff
@@ -215,12 +215,28 @@
                     _str = _str.replace(name, desc)
         if re.findall(r'[( ]async[,=)]', _str):
             for tmp in re.findall(r'[( ]async[,=)]', _str):
                 tmp1 = str(tmp).replace('async', 'async1')
                 _str = _str.replace(tmp, tmp1)
         return _str
 
+    @staticmethod
+    def get_main_key():
+        return GetApi._get_service_value("this_key", _type=1)
+
+    @staticmethod
+    def set_main_key(value):
+        GetApi._set_service_value("this_key", value, _type=1)
+        return True
+
+    @staticmethod
+    def get_main_name():
+        return GetApi._get_service_value("this_name", _type=1)
+
+    @staticmethod
+    def set_main_name(value):
+        GetApi._set_service_value("this_name", value, _type=1)
 
 
 if __name__ == '__main__':
-    ga = GetApi(app_key="a63ca17b-3cf3-46cb-b8b6-9ad20518e1e1")
-    ga.create_or_update_project()
+    ga = GetApi()
+    print('--key：', ga.get_main_name())
```

### Comparing `huhk-1.7.4/huhk/testcase/apache/beam_class.py` & `huhk-1.7.5/huhk/testcase/apache/beam_class.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.4/huhk/testcase/apache/data.py` & `huhk-1.7.5/huhk/testcase/apache/data.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.4/huhk/testcase/apache/par_do.py` & `huhk-1.7.5/huhk/testcase/apache/par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.4/huhk/testcase/apache/test_cogroupbykey.py` & `huhk-1.7.5/huhk/testcase/apache/test_cogroupbykey.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.4/huhk/testcase/apache/test_fiter.py` & `huhk-1.7.5/huhk/testcase/apache/test_fiter.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.4/huhk/testcase/apache/test_flatmap.py` & `huhk-1.7.5/huhk/testcase/apache/test_flatmap.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.4/huhk/testcase/apache/test_map.py` & `huhk-1.7.5/huhk/testcase/apache/test_map.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.4/huhk/testcase/apache/test_par_do.py` & `huhk-1.7.5/huhk/testcase/apache/test_par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.4/huhk/testcase/apache/test_regex.py` & `huhk-1.7.5/huhk/testcase/apache/test_regex.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.4/huhk/testcase/apache/test_time.py` & `huhk-1.7.5/huhk/testcase/apache/test_time.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.4/huhk/unit_apache_beam.py` & `huhk-1.7.5/huhk/unit_apache_beam.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.4/huhk/unit_dict.py` & `huhk-1.7.5/huhk/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.4/huhk/unit_encryption.py` & `huhk-1.7.5/huhk/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.4/huhk/unit_fun.py` & `huhk-1.7.5/huhk/unit_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.4/huhk/unit_logger.py` & `huhk-1.7.5/huhk/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.4/huhk/unit_request.py` & `huhk-1.7.5/huhk/unit_request.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.4/huhk/unit_tasks.py` & `huhk-1.7.5/huhk/unit_tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                 print(e)
             pass
         else:
             Scheduler.scheduler = BlockingScheduler()
 
     @staticmethod
     def get_cron(corn_str):
-        cron_list = re.split(r'\s+', corn_str.strip())
+        cron_list = re.split(r'\s+', corn_str.strip().replace('?', '*').replace('?', '？'))
         cron_list += ["*"] * 7
         second = cron_list[0]
         minute = cron_list[1]
         hour = cron_list[2]
         day = cron_list[3]
         month = cron_list[4]
         day_of_week = '*' if cron_list[5] in ('?', '？') else cron_list[5]
```

### Comparing `huhk-1.7.4/huhk/常用命令.py` & `huhk-1.7.5/huhk/常用命令.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.4/huhk.egg-info/SOURCES.txt` & `huhk-1.7.5/huhk.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 setup.py
 huhk/__init__.py
 huhk/init_project.py
+huhk/main.py
 huhk/setup_run.py
 huhk/unit_apache_beam.py
 huhk/unit_dict.py
 huhk/unit_encryption.py
 huhk/unit_fun.py
 huhk/unit_logger.py
 huhk/unit_request.py
@@ -15,14 +16,15 @@
 huhk.egg-info/dependency_links.txt
 huhk.egg-info/entry_points.txt
 huhk.egg-info/requires.txt
 huhk.egg-info/top_level.txt
 huhk/case_project/__init__.py
 huhk/case_project/json_coder.py
 huhk/case_project/main.py
+huhk/case_project/main_fun.py
 huhk/case_project/project_base.py
 huhk/case_project/project_init.py
 huhk/case_project/project_string.py
 huhk/case_project/setup_set.py
 huhk/case_project/version.py
 huhk/testcase/__init__.py
 huhk/testcase/apache/__init__.py
@@ -53,17 +55,27 @@
 service/app_t/asserts/open/__init__.py
 service/app_t/asserts/open/haohan/__init__.py
 service/app_t/asserts/open/haohan/asserts_open_haohan_relation.py
 service/app_t/asserts/open/haohan/asserts_open_haohan_rights.py
 service/app_t/asserts/points/__init__.py
 service/app_t/asserts/points/asserts_points_points.py
 service/app_t/asserts/points/asserts_points_pointsApp.py
+service/app_t/funs/__init__.py
+service/app_t/funs/funs_app_t.py
+service/app_t/funs/funs_open.py
+service/app_t/funs/funs_points.py
+service/app_t/funs/open/__init__.py
+service/app_t/funs/open/funs_open_haohan.py
+service/app_t/funs/open/haohan/__init__.py
+service/app_t/funs/open/haohan/funs_open_haohan_relation.py
+service/app_t/funs/open/haohan/funs_open_haohan_rights.py
+service/app_t/funs/points/__init__.py
+service/app_t/funs/points/funs_points_points.py
+service/app_t/funs/points/funs_points_pointsApp.py
 service/app_t/sqls/__init__.py
 service/app_t/sqls/open/__init__.py
 service/app_t/sqls/open/haohan/__init__.py
 service/app_t/sqls/open/haohan/sqls_open_haohan_relation.py
 service/app_t/sqls/open/haohan/sqls_open_haohan_rights.py
 service/app_t/sqls/points/__init__.py
 service/app_t/sqls/points/sqls_points_points.py
-service/app_t/sqls/points/sqls_points_pointsApp.py
-testcase/__init__.py
-testcase/app_t/__init__.py
+service/app_t/sqls/points/sqls_points_pointsApp.py
```

### Comparing `huhk-1.7.4/service/app_t/apis/open/haohan/apis_open_haohan_relation.py` & `huhk-1.7.5/service/app_t/apis/open/haohan/apis_open_haohan_relation.py`

 * *Files 15% similar despite different names*

```diff
@@ -540,7 +540,304 @@
 
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
+@allure.step(title="调接口：/open/haohan/relation/update")
+def open_haohan_relation_update(userId=None, headers=None, **kwargs):
+    """
+    浩瀚模块-关联关系-Y
+    up_time=1675665418
+
+    params: userId :  : 用户ID（数据类型：String）
+    params: headers : 请求头
+    ====================返回======================
+    """
+    _method = "GET"
+    _url = "/open/haohan/relation/update"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID（数据类型：String）
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/open/haohan/relation/update")
+def open_haohan_relation_update(userId=None, headers=None, **kwargs):
+    """
+    浩瀚模块-关联关系-Y
+    up_time=1675665418
+
+    params: userId :  : 用户ID（数据类型：String）
+    params: headers : 请求头
+    ====================返回======================
+    """
+    _method = "GET"
+    _url = "/open/haohan/relation/update"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID（数据类型：String）
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/open/haohan/relation/update")
+def open_haohan_relation_update(userId=None, headers=None, **kwargs):
+    """
+    浩瀚模块-关联关系-Y
+    up_time=1675665418
+
+    params: userId :  : 用户ID（数据类型：String）
+    params: headers : 请求头
+    ====================返回======================
+    """
+    _method = "GET"
+    _url = "/open/haohan/relation/update"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID（数据类型：String）
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/open/haohan/relation/update")
+def open_haohan_relation_update(userId=None, headers=None, **kwargs):
+    """
+    浩瀚模块-关联关系-Y
+    up_time=1675665418
+
+    params: userId :  : 用户ID（数据类型：String）
+    params: headers : 请求头
+    ====================返回======================
+    """
+    _method = "GET"
+    _url = "/open/haohan/relation/update"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID（数据类型：String）
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/open/haohan/relation/update")
+def open_haohan_relation_update(userId=None, headers=None, **kwargs):
+    """
+    浩瀚模块-关联关系-Y
+    up_time=1675665418
+
+    params: userId :  : 用户ID（数据类型：String）
+    params: headers : 请求头
+    ====================返回======================
+    """
+    _method = "GET"
+    _url = "/open/haohan/relation/update"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID（数据类型：String）
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/open/haohan/relation/update")
+def open_haohan_relation_update(userId=None, headers=None, **kwargs):
+    """
+    浩瀚模块-关联关系-Y
+    up_time=1675665418
+
+    params: userId :  : 用户ID（数据类型：String）
+    params: headers : 请求头
+    ====================返回======================
+    """
+    _method = "GET"
+    _url = "/open/haohan/relation/update"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID（数据类型：String）
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/open/haohan/relation/update")
+def open_haohan_relation_update(userId=None, headers=None, **kwargs):
+    """
+    浩瀚模块-关联关系-Y
+    up_time=1675665418
+
+    params: userId :  : 用户ID（数据类型：String）
+    params: headers : 请求头
+    ====================返回======================
+    """
+    _method = "GET"
+    _url = "/open/haohan/relation/update"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID（数据类型：String）
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/open/haohan/relation/update")
+def open_haohan_relation_update(userId=None, headers=None, **kwargs):
+    """
+    浩瀚模块-关联关系-Y
+    up_time=1675665418
+
+    params: userId :  : 用户ID（数据类型：String）
+    params: headers : 请求头
+    ====================返回======================
+    """
+    _method = "GET"
+    _url = "/open/haohan/relation/update"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID（数据类型：String）
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/open/haohan/relation/update")
+def open_haohan_relation_update(userId=None, headers=None, **kwargs):
+    """
+    浩瀚模块-关联关系-Y
+    up_time=1675665418
+
+    params: userId :  : 用户ID（数据类型：String）
+    params: headers : 请求头
+    ====================返回======================
+    """
+    _method = "GET"
+    _url = "/open/haohan/relation/update"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID（数据类型：String）
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/open/haohan/relation/update")
+def open_haohan_relation_update(userId=None, headers=None, **kwargs):
+    """
+    浩瀚模块-关联关系-Y
+    up_time=1675665418
+
+    params: userId :  : 用户ID（数据类型：String）
+    params: headers : 请求头
+    ====================返回======================
+    """
+    _method = "GET"
+    _url = "/open/haohan/relation/update"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID（数据类型：String）
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/open/haohan/relation/update")
+def open_haohan_relation_update(userId=None, headers=None, **kwargs):
+    """
+    浩瀚模块-关联关系-Y
+    up_time=1675665418
+
+    params: userId :  : 用户ID（数据类型：String）
+    params: headers : 请求头
+    ====================返回======================
+    """
+    _method = "GET"
+    _url = "/open/haohan/relation/update"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID（数据类型：String）
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
```

### Comparing `huhk-1.7.4/service/app_t/apis/open/haohan/apis_open_haohan_rights.py` & `huhk-1.7.5/service/app_t/apis/open/haohan/apis_open_haohan_rights.py`

 * *Files 12% similar despite different names*

```diff
@@ -580,7 +580,326 @@
 
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
+@allure.step(title="调接口：/open/haohan/rights/update")
+def open_haohan_rights_update(params=None, headers=None, **kwargs):
+    """
+    浩瀚模块 - 更改充电桩权益状态-Y
+    up_time=1675665629
+
+    params: params : object : 
+              data : string : 加密数据
+    params: headers : 请求头
+    ====================返回======================
+    """
+    _method = "POST"
+    _url = "/open/haohan/rights/update"
+
+    _headers = {
+        "Content-Type": "application/json",
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "params": params,
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/open/haohan/rights/update")
+def open_haohan_rights_update(params=None, headers=None, **kwargs):
+    """
+    浩瀚模块 - 更改充电桩权益状态-Y
+    up_time=1675665629
+
+    params: params : object : 
+              data : string : 加密数据
+    params: headers : 请求头
+    ====================返回======================
+    """
+    _method = "POST"
+    _url = "/open/haohan/rights/update"
+
+    _headers = {
+        "Content-Type": "application/json",
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "params": params,
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/open/haohan/rights/update")
+def open_haohan_rights_update(params=None, headers=None, **kwargs):
+    """
+    浩瀚模块 - 更改充电桩权益状态-Y
+    up_time=1675665629
+
+    params: params : object : 
+              data : string : 加密数据
+    params: headers : 请求头
+    ====================返回======================
+    """
+    _method = "POST"
+    _url = "/open/haohan/rights/update"
+
+    _headers = {
+        "Content-Type": "application/json",
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "params": params,
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/open/haohan/rights/update")
+def open_haohan_rights_update(params=None, headers=None, **kwargs):
+    """
+    浩瀚模块 - 更改充电桩权益状态-Y
+    up_time=1675665629
+
+    params: params : object : 
+              data : string : 加密数据
+    params: headers : 请求头
+    ====================返回======================
+    """
+    _method = "POST"
+    _url = "/open/haohan/rights/update"
+
+    _headers = {
+        "Content-Type": "application/json",
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "params": params,
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/open/haohan/rights/update")
+def open_haohan_rights_update(params=None, headers=None, **kwargs):
+    """
+    浩瀚模块 - 更改充电桩权益状态-Y
+    up_time=1675665629
+
+    params: params : object : 
+              data : string : 加密数据
+    params: headers : 请求头
+    ====================返回======================
+    """
+    _method = "POST"
+    _url = "/open/haohan/rights/update"
+
+    _headers = {
+        "Content-Type": "application/json",
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "params": params,
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/open/haohan/rights/update")
+def open_haohan_rights_update(params=None, headers=None, **kwargs):
+    """
+    浩瀚模块 - 更改充电桩权益状态-Y
+    up_time=1675665629
+
+    params: params : object : 
+              data : string : 加密数据
+    params: headers : 请求头
+    ====================返回======================
+    """
+    _method = "POST"
+    _url = "/open/haohan/rights/update"
+
+    _headers = {
+        "Content-Type": "application/json",
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "params": params,
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/open/haohan/rights/update")
+def open_haohan_rights_update(params=None, headers=None, **kwargs):
+    """
+    浩瀚模块 - 更改充电桩权益状态-Y
+    up_time=1675665629
+
+    params: params : object : 
+              data : string : 加密数据
+    params: headers : 请求头
+    ====================返回======================
+    """
+    _method = "POST"
+    _url = "/open/haohan/rights/update"
+
+    _headers = {
+        "Content-Type": "application/json",
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "params": params,
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/open/haohan/rights/update")
+def open_haohan_rights_update(params=None, headers=None, **kwargs):
+    """
+    浩瀚模块 - 更改充电桩权益状态-Y
+    up_time=1675665629
+
+    params: params : object : 
+              data : string : 加密数据
+    params: headers : 请求头
+    ====================返回======================
+    """
+    _method = "POST"
+    _url = "/open/haohan/rights/update"
+
+    _headers = {
+        "Content-Type": "application/json",
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "params": params,
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/open/haohan/rights/update")
+def open_haohan_rights_update(params=None, headers=None, **kwargs):
+    """
+    浩瀚模块 - 更改充电桩权益状态-Y
+    up_time=1675665629
+
+    params: params : object : 
+              data : string : 加密数据
+    params: headers : 请求头
+    ====================返回======================
+    """
+    _method = "POST"
+    _url = "/open/haohan/rights/update"
+
+    _headers = {
+        "Content-Type": "application/json",
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "params": params,
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/open/haohan/rights/update")
+def open_haohan_rights_update(params=None, headers=None, **kwargs):
+    """
+    浩瀚模块 - 更改充电桩权益状态-Y
+    up_time=1675665629
+
+    params: params : object : 
+              data : string : 加密数据
+    params: headers : 请求头
+    ====================返回======================
+    """
+    _method = "POST"
+    _url = "/open/haohan/rights/update"
+
+    _headers = {
+        "Content-Type": "application/json",
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "params": params,
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/open/haohan/rights/update")
+def open_haohan_rights_update(params=None, headers=None, **kwargs):
+    """
+    浩瀚模块 - 更改充电桩权益状态-Y
+    up_time=1675665629
+
+    params: params : object : 
+              data : string : 加密数据
+    params: headers : 请求头
+    ====================返回======================
+    """
+    _method = "POST"
+    _url = "/open/haohan/rights/update"
+
+    _headers = {
+        "Content-Type": "application/json",
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "params": params,
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
```

### Comparing `huhk-1.7.4/service/app_t/apis/points/apis_points_points.py` & `huhk-1.7.5/service/app_t/apis/points/apis_points_points.py`

 * *Files 13% similar despite different names*

```diff
@@ -787,7 +787,381 @@
 
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
+@allure.step(title="调接口：/points/points/flowDetail")
+def points_points_flowDetail(userId=None, headers=None, **kwargs):
+    """
+    查看积分明细- - 积分流水分页查询
+    up_time=1676254506
+
+    params: userId :  : 用户ID
+    params: headers : 请求头
+    ====================返回======================
+    params: code : number : 
+    params: msg : string : 
+    params: data : object : 
+              records : array : 
+              size : number : 每页大小
+              current : number : 当前页
+              total : number : 总页数
+    """
+    _method = "GET"
+    _url = "/points/points/flowDetail"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/points/points/flowDetail")
+def points_points_flowDetail(userId=None, headers=None, **kwargs):
+    """
+    查看积分明细- - 积分流水分页查询
+    up_time=1676254506
+
+    params: userId :  : 用户ID
+    params: headers : 请求头
+    ====================返回======================
+    params: code : number : 
+    params: msg : string : 
+    params: data : object : 
+              records : array : 
+              size : number : 每页大小
+              current : number : 当前页
+              total : number : 总页数
+    """
+    _method = "GET"
+    _url = "/points/points/flowDetail"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/points/points/flowDetail")
+def points_points_flowDetail(userId=None, headers=None, **kwargs):
+    """
+    查看积分明细- - 积分流水分页查询
+    up_time=1676254506
+
+    params: userId :  : 用户ID
+    params: headers : 请求头
+    ====================返回======================
+    params: code : number : 
+    params: msg : string : 
+    params: data : object : 
+              records : array : 
+              size : number : 每页大小
+              current : number : 当前页
+              total : number : 总页数
+    """
+    _method = "GET"
+    _url = "/points/points/flowDetail"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/points/points/flowDetail")
+def points_points_flowDetail(userId=None, headers=None, **kwargs):
+    """
+    查看积分明细- - 积分流水分页查询
+    up_time=1676254506
+
+    params: userId :  : 用户ID
+    params: headers : 请求头
+    ====================返回======================
+    params: code : number : 
+    params: msg : string : 
+    params: data : object : 
+              records : array : 
+              size : number : 每页大小
+              current : number : 当前页
+              total : number : 总页数
+    """
+    _method = "GET"
+    _url = "/points/points/flowDetail"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/points/points/flowDetail")
+def points_points_flowDetail(userId=None, headers=None, **kwargs):
+    """
+    查看积分明细- - 积分流水分页查询
+    up_time=1676254506
+
+    params: userId :  : 用户ID
+    params: headers : 请求头
+    ====================返回======================
+    params: code : number : 
+    params: msg : string : 
+    params: data : object : 
+              records : array : 
+              size : number : 每页大小
+              current : number : 当前页
+              total : number : 总页数
+    """
+    _method = "GET"
+    _url = "/points/points/flowDetail"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/points/points/flowDetail")
+def points_points_flowDetail(userId=None, headers=None, **kwargs):
+    """
+    查看积分明细- - 积分流水分页查询
+    up_time=1676254506
+
+    params: userId :  : 用户ID
+    params: headers : 请求头
+    ====================返回======================
+    params: code : number : 
+    params: msg : string : 
+    params: data : object : 
+              records : array : 
+              size : number : 每页大小
+              current : number : 当前页
+              total : number : 总页数
+    """
+    _method = "GET"
+    _url = "/points/points/flowDetail"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/points/points/flowDetail")
+def points_points_flowDetail(userId=None, headers=None, **kwargs):
+    """
+    查看积分明细- - 积分流水分页查询
+    up_time=1676254506
+
+    params: userId :  : 用户ID
+    params: headers : 请求头
+    ====================返回======================
+    params: code : number : 
+    params: msg : string : 
+    params: data : object : 
+              records : array : 
+              size : number : 每页大小
+              current : number : 当前页
+              total : number : 总页数
+    """
+    _method = "GET"
+    _url = "/points/points/flowDetail"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/points/points/flowDetail")
+def points_points_flowDetail(userId=None, headers=None, **kwargs):
+    """
+    查看积分明细- - 积分流水分页查询
+    up_time=1676254506
+
+    params: userId :  : 用户ID
+    params: headers : 请求头
+    ====================返回======================
+    params: code : number : 
+    params: msg : string : 
+    params: data : object : 
+              records : array : 
+              size : number : 每页大小
+              current : number : 当前页
+              total : number : 总页数
+    """
+    _method = "GET"
+    _url = "/points/points/flowDetail"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/points/points/flowDetail")
+def points_points_flowDetail(userId=None, headers=None, **kwargs):
+    """
+    查看积分明细- - 积分流水分页查询
+    up_time=1676254506
+
+    params: userId :  : 用户ID
+    params: headers : 请求头
+    ====================返回======================
+    params: code : number : 
+    params: msg : string : 
+    params: data : object : 
+              records : array : 
+              size : number : 每页大小
+              current : number : 当前页
+              total : number : 总页数
+    """
+    _method = "GET"
+    _url = "/points/points/flowDetail"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/points/points/flowDetail")
+def points_points_flowDetail(userId=None, headers=None, **kwargs):
+    """
+    查看积分明细- - 积分流水分页查询
+    up_time=1676254506
+
+    params: userId :  : 用户ID
+    params: headers : 请求头
+    ====================返回======================
+    params: code : number : 
+    params: msg : string : 
+    params: data : object : 
+              records : array : 
+              size : number : 每页大小
+              current : number : 当前页
+              total : number : 总页数
+    """
+    _method = "GET"
+    _url = "/points/points/flowDetail"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/points/points/flowDetail")
+def points_points_flowDetail(userId=None, headers=None, **kwargs):
+    """
+    查看积分明细- - 积分流水分页查询
+    up_time=1676254506
+
+    params: userId :  : 用户ID
+    params: headers : 请求头
+    ====================返回======================
+    params: code : number : 
+    params: msg : string : 
+    params: data : object : 
+              records : array : 
+              size : number : 每页大小
+              current : number : 当前页
+              total : number : 总页数
+    """
+    _method = "GET"
+    _url = "/points/points/flowDetail"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
```

### Comparing `huhk-1.7.4/service/app_t/apis/points/apis_points_pointsApp.py` & `huhk-1.7.5/service/app_t/apis/points/apis_points_pointsApp.py`

 * *Files 16% similar despite different names*

```diff
@@ -664,7 +664,337 @@
 
     _params = {
     }
 
     return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
 
 
+@allure.step(title="调接口：/points/pointsApp/signIn")
+def points_pointsApp_signIn(userId=None, headers=None, **kwargs):
+    """
+    APP-用户签到
+    up_time=1676254515
+
+    params: userId :  : 用户ID
+    params: headers : 请求头
+    ====================返回======================
+    params: code : number : 0成功;1失败
+    params: msg : string : 
+    params: data : boolean : true/false 签到成功/失败
+    """
+    _method = "GET"
+    _url = "/points/pointsApp/signIn"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/points/pointsApp/signIn")
+def points_pointsApp_signIn(userId=None, headers=None, **kwargs):
+    """
+    APP-用户签到
+    up_time=1676254515
+
+    params: userId :  : 用户ID
+    params: headers : 请求头
+    ====================返回======================
+    params: code : number : 0成功;1失败
+    params: msg : string : 
+    params: data : boolean : true/false 签到成功/失败
+    """
+    _method = "GET"
+    _url = "/points/pointsApp/signIn"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/points/pointsApp/signIn")
+def points_pointsApp_signIn(userId=None, headers=None, **kwargs):
+    """
+    APP-用户签到
+    up_time=1676254515
+
+    params: userId :  : 用户ID
+    params: headers : 请求头
+    ====================返回======================
+    params: code : number : 0成功;1失败
+    params: msg : string : 
+    params: data : boolean : true/false 签到成功/失败
+    """
+    _method = "GET"
+    _url = "/points/pointsApp/signIn"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/points/pointsApp/signIn")
+def points_pointsApp_signIn(userId=None, headers=None, **kwargs):
+    """
+    APP-用户签到
+    up_time=1676254515
+
+    params: userId :  : 用户ID
+    params: headers : 请求头
+    ====================返回======================
+    params: code : number : 0成功;1失败
+    params: msg : string : 
+    params: data : boolean : true/false 签到成功/失败
+    """
+    _method = "GET"
+    _url = "/points/pointsApp/signIn"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/points/pointsApp/signIn")
+def points_pointsApp_signIn(userId=None, headers=None, **kwargs):
+    """
+    APP-用户签到
+    up_time=1676254515
+
+    params: userId :  : 用户ID
+    params: headers : 请求头
+    ====================返回======================
+    params: code : number : 0成功;1失败
+    params: msg : string : 
+    params: data : boolean : true/false 签到成功/失败
+    """
+    _method = "GET"
+    _url = "/points/pointsApp/signIn"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/points/pointsApp/signIn")
+def points_pointsApp_signIn(userId=None, headers=None, **kwargs):
+    """
+    APP-用户签到
+    up_time=1676254515
+
+    params: userId :  : 用户ID
+    params: headers : 请求头
+    ====================返回======================
+    params: code : number : 0成功;1失败
+    params: msg : string : 
+    params: data : boolean : true/false 签到成功/失败
+    """
+    _method = "GET"
+    _url = "/points/pointsApp/signIn"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/points/pointsApp/signIn")
+def points_pointsApp_signIn(userId=None, headers=None, **kwargs):
+    """
+    APP-用户签到
+    up_time=1676254515
+
+    params: userId :  : 用户ID
+    params: headers : 请求头
+    ====================返回======================
+    params: code : number : 0成功;1失败
+    params: msg : string : 
+    params: data : boolean : true/false 签到成功/失败
+    """
+    _method = "GET"
+    _url = "/points/pointsApp/signIn"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/points/pointsApp/signIn")
+def points_pointsApp_signIn(userId=None, headers=None, **kwargs):
+    """
+    APP-用户签到
+    up_time=1676254515
+
+    params: userId :  : 用户ID
+    params: headers : 请求头
+    ====================返回======================
+    params: code : number : 0成功;1失败
+    params: msg : string : 
+    params: data : boolean : true/false 签到成功/失败
+    """
+    _method = "GET"
+    _url = "/points/pointsApp/signIn"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/points/pointsApp/signIn")
+def points_pointsApp_signIn(userId=None, headers=None, **kwargs):
+    """
+    APP-用户签到
+    up_time=1676254515
+
+    params: userId :  : 用户ID
+    params: headers : 请求头
+    ====================返回======================
+    params: code : number : 0成功;1失败
+    params: msg : string : 
+    params: data : boolean : true/false 签到成功/失败
+    """
+    _method = "GET"
+    _url = "/points/pointsApp/signIn"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/points/pointsApp/signIn")
+def points_pointsApp_signIn(userId=None, headers=None, **kwargs):
+    """
+    APP-用户签到
+    up_time=1676254515
+
+    params: userId :  : 用户ID
+    params: headers : 请求头
+    ====================返回======================
+    params: code : number : 0成功;1失败
+    params: msg : string : 
+    params: data : boolean : true/false 签到成功/失败
+    """
+    _method = "GET"
+    _url = "/points/pointsApp/signIn"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
+@allure.step(title="调接口：/points/pointsApp/signIn")
+def points_pointsApp_signIn(userId=None, headers=None, **kwargs):
+    """
+    APP-用户签到
+    up_time=1676254515
+
+    params: userId :  : 用户ID
+    params: headers : 请求头
+    ====================返回======================
+    params: code : number : 0成功;1失败
+    params: msg : string : 
+    params: data : boolean : true/false 签到成功/失败
+    """
+    _method = "GET"
+    _url = "/points/pointsApp/signIn"
+
+    _headers = {
+    }
+    _headers.update({"headers": headers})
+
+    _data = {
+        "userId": userId,  # 用户ID
+    }
+
+    _params = {
+    }
+
+    return http_requester(_method, _url, params=_params, data=_data, headers=_headers, **kwargs)
+
+
```

### Comparing `huhk-1.7.4/service/app_t/app_t_fun.py` & `huhk-1.7.5/service/app_t/app_t_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.4/service/app_t/asserts/open/haohan/asserts_open_haohan_relation.py` & `huhk-1.7.5/service/app_t/asserts/open/haohan/asserts_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.4/service/app_t/asserts/open/haohan/asserts_open_haohan_rights.py` & `huhk-1.7.5/service/app_t/asserts/open/haohan/asserts_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.4/service/app_t/asserts/points/asserts_points_points.py` & `huhk-1.7.5/service/app_t/asserts/points/asserts_points_points.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.4/service/app_t/asserts/points/asserts_points_pointsApp.py` & `huhk-1.7.5/service/app_t/asserts/points/asserts_points_pointsApp.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.4/service/app_t/sqls/open/haohan/sqls_open_haohan_relation.py` & `huhk-1.7.5/service/app_t/sqls/open/haohan/sqls_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.4/service/app_t/sqls/open/haohan/sqls_open_haohan_rights.py` & `huhk-1.7.5/service/app_t/sqls/open/haohan/sqls_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.4/service/app_t/sqls/points/sqls_points_points.py` & `huhk-1.7.5/service/app_t/sqls/points/sqls_points_points.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.4/service/app_t/sqls/points/sqls_points_pointsApp.py` & `huhk-1.7.5/service/app_t/sqls/points/sqls_points_pointsApp.py`

 * *Files identical despite different names*

