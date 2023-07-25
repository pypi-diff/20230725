# Comparing `tmp/huhk-1.7.5.tar.gz` & `tmp/huhk-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhk-1.7.5.tar", last modified: Tue Jul 25 01:37:45 2023, max compression
+gzip compressed data, was "huhk-1.7.6.tar", last modified: Tue Jul 25 02:49:18 2023, max compression
```

## Comparing `huhk-1.7.5.tar` & `huhk-1.7.6.tar`

### file list

```diff
@@ -1,107 +1,106 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.284623 huhk-1.7.5/
--rw-rw-rw-   0        0        0      223 2023-07-25 01:37:45.283623 huhk-1.7.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.077771 huhk-1.7.5/huhk/
--rw-rw-rw-   0        0        0      772 2023-07-17 02:44:39.000000 huhk-1.7.5/huhk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.118174 huhk-1.7.5/huhk/case_project/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.7.5/huhk/case_project/__init__.py
--rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.7.5/huhk/case_project/json_coder.py
--rw-rw-rw-   0        0        0     1223 2023-07-25 01:24:26.000000 huhk-1.7.5/huhk/case_project/main.py
--rw-rw-rw-   0        0        0      297 2023-07-25 01:19:15.000000 huhk-1.7.5/huhk/case_project/main_fun.py
--rw-rw-rw-   0        0        0    17758 2023-07-24 09:52:23.000000 huhk-1.7.5/huhk/case_project/project_base.py
--rw-rw-rw-   0        0        0     2099 2023-07-21 08:18:22.000000 huhk-1.7.5/huhk/case_project/project_init.py
--rw-rw-rw-   0        0        0    13835 2023-07-24 01:29:57.000000 huhk-1.7.5/huhk/case_project/project_string.py
--rw-rw-rw-   0        0        0      908 2023-07-12 01:13:24.000000 huhk-1.7.5/huhk/case_project/setup_set.py
--rw-rw-rw-   0        0        0       17 2023-07-25 01:37:44.000000 huhk-1.7.5/huhk/case_project/version.py
--rw-rw-rw-   0        0        0    13598 2023-07-24 09:53:49.000000 huhk-1.7.5/huhk/init_project.py
--rw-rw-rw-   0        0        0     1218 2023-07-25 01:19:15.000000 huhk-1.7.5/huhk/main.py
--rw-rw-rw-   0        0        0      274 2023-07-12 01:13:24.000000 huhk-1.7.5/huhk/setup_run.py
-drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.122190 huhk-1.7.5/huhk/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.7.5/huhk/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.169593 huhk-1.7.5/huhk/testcase/apache/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.7.5/huhk/testcase/apache/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.7.5/huhk/testcase/apache/beam_class.py
--rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.7.5/huhk/testcase/apache/data.py
--rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.7.5/huhk/testcase/apache/par_do.py
--rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.7.5/huhk/testcase/apache/test_cogroupbykey.py
--rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.7.5/huhk/testcase/apache/test_file.py
--rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.7.5/huhk/testcase/apache/test_fiter.py
--rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.7.5/huhk/testcase/apache/test_flatmap.py
--rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.7.5/huhk/testcase/apache/test_map.py
--rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.7.5/huhk/testcase/apache/test_par_do.py
--rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.7.5/huhk/testcase/apache/test_regex.py
--rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.7.5/huhk/testcase/apache/test_time.py
--rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.7.5/huhk/testcase/apache/test_to_string.py
--rw-rw-rw-   0        0        0    22615 2023-07-14 06:52:17.000000 huhk-1.7.5/huhk/unit_apache_beam.py
--rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.7.5/huhk/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.7.5/huhk/unit_encryption.py
--rw-rw-rw-   0        0        0    28445 2023-07-22 10:41:46.000000 huhk-1.7.5/huhk/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.7.5/huhk/unit_logger.py
--rw-rw-rw-   0        0        0     9960 2023-07-22 07:06:52.000000 huhk-1.7.5/huhk/unit_request.py
--rw-rw-rw-   0        0        0     2511 2023-07-24 06:56:32.000000 huhk-1.7.5/huhk/unit_tasks.py
--rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.7.5/huhk/常用命令.py
-drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.091732 huhk-1.7.5/huhk.egg-info/
--rw-rw-rw-   0        0        0      223 2023-07-25 01:37:44.000000 huhk-1.7.5/huhk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2885 2023-07-25 01:37:44.000000 huhk-1.7.5/huhk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 01:37:44.000000 huhk-1.7.5/huhk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-07-25 01:37:44.000000 huhk-1.7.5/huhk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      134 2023-07-25 01:37:44.000000 huhk-1.7.5/huhk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-25 01:37:44.000000 huhk-1.7.5/huhk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.173581 huhk-1.7.5/service/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.5/service/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.178568 huhk-1.7.5/service/app_t/
--rw-rw-rw-   0        0        0      420 2023-07-22 06:54:11.000000 huhk-1.7.5/service/app_t/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.181560 huhk-1.7.5/service/app_t/apis/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.5/service/app_t/apis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.183587 huhk-1.7.5/service/app_t/apis/open/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/apis/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.191533 huhk-1.7.5/service/app_t/apis/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/apis/open/haohan/__init__.py
--rw-rw-rw-   0        0        0    22236 2023-07-24 01:53:24.000000 huhk-1.7.5/service/app_t/apis/open/haohan/apis_open_haohan_relation.py
--rw-rw-rw-   0        0        0    23259 2023-07-24 01:53:26.000000 huhk-1.7.5/service/app_t/apis/open/haohan/apis_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.200509 huhk-1.7.5/service/app_t/apis/points/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/apis/points/__init__.py
--rw-rw-rw-   0        0        0    31535 2023-07-24 01:53:27.000000 huhk-1.7.5/service/app_t/apis/points/apis_points_points.py
--rw-rw-rw-   0        0        0    25708 2023-07-24 01:53:27.000000 huhk-1.7.5/service/app_t/apis/points/apis_points_pointsApp.py
--rw-rw-rw-   0        0        0      650 2023-07-22 10:57:15.000000 huhk-1.7.5/service/app_t/app_t_fun.py
-drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.203504 huhk-1.7.5/service/app_t/asserts/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.5/service/app_t/asserts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.205520 huhk-1.7.5/service/app_t/asserts/open/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/asserts/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.213522 huhk-1.7.5/service/app_t/asserts/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/asserts/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      602 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/asserts/open/haohan/asserts_open_haohan_relation.py
--rw-rw-rw-   0        0        0      590 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/asserts/open/haohan/asserts_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.221452 huhk-1.7.5/service/app_t/asserts/points/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/asserts/points/__init__.py
--rw-rw-rw-   0        0        0     1761 2023-07-22 07:08:51.000000 huhk-1.7.5/service/app_t/asserts/points/asserts_points_points.py
--rw-rw-rw-   0        0        0     1358 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/asserts/points/asserts_points_pointsApp.py
-drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.234099 huhk-1.7.5/service/app_t/funs/
--rw-rw-rw-   0        0        0        0 2023-07-24 01:53:24.000000 huhk-1.7.5/service/app_t/funs/__init__.py
--rw-rw-rw-   0        0        0      161 2023-07-24 01:53:33.000000 huhk-1.7.5/service/app_t/funs/funs_app_t.py
--rw-rw-rw-   0        0        0      118 2023-07-24 01:53:32.000000 huhk-1.7.5/service/app_t/funs/funs_open.py
--rw-rw-rw-   0        0        0      230 2023-07-24 01:53:33.000000 huhk-1.7.5/service/app_t/funs/funs_points.py
-drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.242066 huhk-1.7.5/service/app_t/funs/open/
--rw-rw-rw-   0        0        0        0 2023-07-24 01:53:27.000000 huhk-1.7.5/service/app_t/funs/open/__init__.py
--rw-rw-rw-   0        0        0      267 2023-07-24 01:53:31.000000 huhk-1.7.5/service/app_t/funs/open/funs_open_haohan.py
-drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.251046 huhk-1.7.5/service/app_t/funs/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-24 01:53:27.000000 huhk-1.7.5/service/app_t/funs/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      824 2023-07-24 01:53:27.000000 huhk-1.7.5/service/app_t/funs/open/haohan/funs_open_haohan_relation.py
--rw-rw-rw-   0        0        0      910 2023-07-24 01:53:31.000000 huhk-1.7.5/service/app_t/funs/open/haohan/funs_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.259026 huhk-1.7.5/service/app_t/funs/points/
--rw-rw-rw-   0        0        0        0 2023-07-24 01:53:32.000000 huhk-1.7.5/service/app_t/funs/points/__init__.py
--rw-rw-rw-   0        0        0     3103 2023-07-24 01:53:34.000000 huhk-1.7.5/service/app_t/funs/points/funs_points_points.py
--rw-rw-rw-   0        0        0     1899 2023-07-24 01:53:33.000000 huhk-1.7.5/service/app_t/funs/points/funs_points_pointsApp.py
-drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.262018 huhk-1.7.5/service/app_t/sqls/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.5/service/app_t/sqls/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.263973 huhk-1.7.5/service/app_t/sqls/open/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/sqls/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.272648 huhk-1.7.5/service/app_t/sqls/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/sqls/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      571 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/sqls/open/haohan/sqls_open_haohan_relation.py
--rw-rw-rw-   0        0        0      567 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/sqls/open/haohan/sqls_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-25 01:37:45.280632 huhk-1.7.5/service/app_t/sqls/points/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/sqls/points/__init__.py
--rw-rw-rw-   0        0        0     1994 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/sqls/points/sqls_points_points.py
--rw-rw-rw-   0        0        0     1529 2023-07-22 06:51:21.000000 huhk-1.7.5/service/app_t/sqls/points/sqls_points_pointsApp.py
--rw-rw-rw-   0        0        0       42 2023-07-25 01:37:45.284623 huhk-1.7.5/setup.cfg
--rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.7.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:49:18.018945 huhk-1.7.6/
+-rw-rw-rw-   0        0        0      223 2023-07-25 02:49:18.018945 huhk-1.7.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-25 02:49:17.852852 huhk-1.7.6/huhk/
+-rw-rw-rw-   0        0        0      772 2023-07-17 02:44:39.000000 huhk-1.7.6/huhk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:49:17.882000 huhk-1.7.6/huhk/case_project/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.7.6/huhk/case_project/__init__.py
+-rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.7.6/huhk/case_project/json_coder.py
+-rw-rw-rw-   0        0        0      490 2023-07-25 02:41:51.000000 huhk-1.7.6/huhk/case_project/main_fun.py
+-rw-rw-rw-   0        0        0    17758 2023-07-24 09:52:23.000000 huhk-1.7.6/huhk/case_project/project_base.py
+-rw-rw-rw-   0        0        0     2099 2023-07-21 08:18:22.000000 huhk-1.7.6/huhk/case_project/project_init.py
+-rw-rw-rw-   0        0        0    13835 2023-07-24 01:29:57.000000 huhk-1.7.6/huhk/case_project/project_string.py
+-rw-rw-rw-   0        0        0      908 2023-07-12 01:13:24.000000 huhk-1.7.6/huhk/case_project/setup_set.py
+-rw-rw-rw-   0        0        0       17 2023-07-25 02:49:17.000000 huhk-1.7.6/huhk/case_project/version.py
+-rw-rw-rw-   0        0        0    13903 2023-07-25 02:42:01.000000 huhk-1.7.6/huhk/init_project.py
+-rw-rw-rw-   0        0        0     1276 2023-07-25 02:46:17.000000 huhk-1.7.6/huhk/main.py
+-rw-rw-rw-   0        0        0      274 2023-07-12 01:13:24.000000 huhk-1.7.6/huhk/setup_run.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:49:17.883997 huhk-1.7.6/huhk/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.7.6/huhk/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:49:17.923495 huhk-1.7.6/huhk/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.7.6/huhk/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.7.6/huhk/testcase/apache/beam_class.py
+-rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.7.6/huhk/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.7.6/huhk/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.7.6/huhk/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.7.6/huhk/testcase/apache/test_file.py
+-rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.7.6/huhk/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.7.6/huhk/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.7.6/huhk/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.7.6/huhk/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.7.6/huhk/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.7.6/huhk/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.7.6/huhk/testcase/apache/test_to_string.py
+-rw-rw-rw-   0        0        0    22615 2023-07-14 06:52:17.000000 huhk-1.7.6/huhk/unit_apache_beam.py
+-rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.7.6/huhk/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.7.6/huhk/unit_encryption.py
+-rw-rw-rw-   0        0        0    28445 2023-07-22 10:41:46.000000 huhk-1.7.6/huhk/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.7.6/huhk/unit_logger.py
+-rw-rw-rw-   0        0        0     9960 2023-07-22 07:06:52.000000 huhk-1.7.6/huhk/unit_request.py
+-rw-rw-rw-   0        0        0     2511 2023-07-24 06:56:32.000000 huhk-1.7.6/huhk/unit_tasks.py
+-rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.7.6/huhk/常用命令.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:49:17.865042 huhk-1.7.6/huhk.egg-info/
+-rw-rw-rw-   0        0        0      223 2023-07-25 02:49:17.000000 huhk-1.7.6/huhk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2859 2023-07-25 02:49:17.000000 huhk-1.7.6/huhk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 02:49:17.000000 huhk-1.7.6/huhk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-25 02:49:17.000000 huhk-1.7.6/huhk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      134 2023-07-25 02:49:17.000000 huhk-1.7.6/huhk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-25 02:49:17.000000 huhk-1.7.6/huhk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 02:49:17.925487 huhk-1.7.6/service/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.6/service/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:49:17.930474 huhk-1.7.6/service/app_t/
+-rw-rw-rw-   0        0        0      420 2023-07-22 06:54:11.000000 huhk-1.7.6/service/app_t/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:49:17.932469 huhk-1.7.6/service/app_t/apis/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.6/service/app_t/apis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:49:17.936461 huhk-1.7.6/service/app_t/apis/open/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.6/service/app_t/apis/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:49:17.944477 huhk-1.7.6/service/app_t/apis/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.6/service/app_t/apis/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0    22236 2023-07-24 01:53:24.000000 huhk-1.7.6/service/app_t/apis/open/haohan/apis_open_haohan_relation.py
+-rw-rw-rw-   0        0        0    23259 2023-07-24 01:53:26.000000 huhk-1.7.6/service/app_t/apis/open/haohan/apis_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:49:17.951422 huhk-1.7.6/service/app_t/apis/points/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.6/service/app_t/apis/points/__init__.py
+-rw-rw-rw-   0        0        0    31535 2023-07-24 01:53:27.000000 huhk-1.7.6/service/app_t/apis/points/apis_points_points.py
+-rw-rw-rw-   0        0        0    25708 2023-07-24 01:53:27.000000 huhk-1.7.6/service/app_t/apis/points/apis_points_pointsApp.py
+-rw-rw-rw-   0        0        0      650 2023-07-22 10:57:15.000000 huhk-1.7.6/service/app_t/app_t_fun.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:49:17.954411 huhk-1.7.6/service/app_t/asserts/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.6/service/app_t/asserts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:49:17.956405 huhk-1.7.6/service/app_t/asserts/open/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.6/service/app_t/asserts/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:49:17.964385 huhk-1.7.6/service/app_t/asserts/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.6/service/app_t/asserts/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      602 2023-07-22 06:51:21.000000 huhk-1.7.6/service/app_t/asserts/open/haohan/asserts_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      590 2023-07-22 06:51:21.000000 huhk-1.7.6/service/app_t/asserts/open/haohan/asserts_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:49:17.972363 huhk-1.7.6/service/app_t/asserts/points/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.6/service/app_t/asserts/points/__init__.py
+-rw-rw-rw-   0        0        0     1761 2023-07-22 07:08:51.000000 huhk-1.7.6/service/app_t/asserts/points/asserts_points_points.py
+-rw-rw-rw-   0        0        0     1358 2023-07-22 06:51:21.000000 huhk-1.7.6/service/app_t/asserts/points/asserts_points_pointsApp.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:49:17.980341 huhk-1.7.6/service/app_t/funs/
+-rw-rw-rw-   0        0        0        0 2023-07-24 01:53:24.000000 huhk-1.7.6/service/app_t/funs/__init__.py
+-rw-rw-rw-   0        0        0      161 2023-07-24 01:53:33.000000 huhk-1.7.6/service/app_t/funs/funs_app_t.py
+-rw-rw-rw-   0        0        0      118 2023-07-24 01:53:32.000000 huhk-1.7.6/service/app_t/funs/funs_open.py
+-rw-rw-rw-   0        0        0      230 2023-07-24 01:53:33.000000 huhk-1.7.6/service/app_t/funs/funs_points.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:49:17.984332 huhk-1.7.6/service/app_t/funs/open/
+-rw-rw-rw-   0        0        0        0 2023-07-24 01:53:27.000000 huhk-1.7.6/service/app_t/funs/open/__init__.py
+-rw-rw-rw-   0        0        0      267 2023-07-24 01:53:31.000000 huhk-1.7.6/service/app_t/funs/open/funs_open_haohan.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:49:17.991313 huhk-1.7.6/service/app_t/funs/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-24 01:53:27.000000 huhk-1.7.6/service/app_t/funs/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      824 2023-07-24 01:53:27.000000 huhk-1.7.6/service/app_t/funs/open/haohan/funs_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      910 2023-07-24 01:53:31.000000 huhk-1.7.6/service/app_t/funs/open/haohan/funs_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:49:17.997003 huhk-1.7.6/service/app_t/funs/points/
+-rw-rw-rw-   0        0        0        0 2023-07-24 01:53:32.000000 huhk-1.7.6/service/app_t/funs/points/__init__.py
+-rw-rw-rw-   0        0        0     3103 2023-07-24 01:53:34.000000 huhk-1.7.6/service/app_t/funs/points/funs_points_points.py
+-rw-rw-rw-   0        0        0     1899 2023-07-24 01:53:33.000000 huhk-1.7.6/service/app_t/funs/points/funs_points_pointsApp.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:49:17.998967 huhk-1.7.6/service/app_t/sqls/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.6/service/app_t/sqls/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:49:18.000963 huhk-1.7.6/service/app_t/sqls/open/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.6/service/app_t/sqls/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:49:18.008960 huhk-1.7.6/service/app_t/sqls/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.6/service/app_t/sqls/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      571 2023-07-22 06:51:21.000000 huhk-1.7.6/service/app_t/sqls/open/haohan/sqls_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      567 2023-07-22 06:51:21.000000 huhk-1.7.6/service/app_t/sqls/open/haohan/sqls_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:49:18.015956 huhk-1.7.6/service/app_t/sqls/points/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.6/service/app_t/sqls/points/__init__.py
+-rw-rw-rw-   0        0        0     1994 2023-07-22 06:51:21.000000 huhk-1.7.6/service/app_t/sqls/points/sqls_points_points.py
+-rw-rw-rw-   0        0        0     1529 2023-07-22 06:51:21.000000 huhk-1.7.6/service/app_t/sqls/points/sqls_points_pointsApp.py
+-rw-rw-rw-   0        0        0       42 2023-07-25 02:49:18.019911 huhk-1.7.6/setup.cfg
+-rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.7.6/setup.py
```

### Comparing `huhk-1.7.5/huhk/__init__.py` & `huhk-1.7.6/huhk/__init__.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/huhk/case_project/json_coder.py` & `huhk-1.7.6/huhk/case_project/json_coder.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/huhk/case_project/main.py` & `huhk-1.7.6/huhk/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import click
-from huhk.case_project.main_fun import get_version
+from huhk.case_project.main_fun import get_version, set_key_name
 
 
 @click.command()
 @click.option('-v', '--version', help='版本, 当前--key/--name', is_eager=True, is_flag=True)
 @click.option('-k', '--key', help='项目key, 传*表示所有项目，不传默认去上一次key', multiple=True)
 @click.option('-n', '--name', help='项目名称, 传*表示所有项目，不传默认去上一次name', multiple=True)
 @click.option('-i', '--install', help='根据key创建项目, 项目存在则更新')
 @click.option('-u', '--update', help='根据--key更新项目，--key不存在时默认取之前的值', is_eager=True, is_flag=True)
 @click.option('-f', '--fun', help='新增api方法，参数url，--key不存在时默认取之前的值', multiple=True)
 def main(version, key, name, install, update, fun):
     print(version, key, name, install, update, fun)
     if version:
         click.echo(get_version())
-    #
+    else:
+        set_key_name(key, name)
+
     # for k in key:
     #     if install:
     #         click.echo('init：' + _version)
     #         click.echo(type(install))
     #     elif update:
     #         click.echo('update：' + _version)
     #         click.echo(type(update))
```

### Comparing `huhk-1.7.5/huhk/case_project/project_base.py` & `huhk-1.7.6/huhk/case_project/project_base.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/huhk/case_project/project_init.py` & `huhk-1.7.6/huhk/case_project/project_init.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/huhk/case_project/project_string.py` & `huhk-1.7.6/huhk/case_project/project_string.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/huhk/case_project/setup_set.py` & `huhk-1.7.6/huhk/case_project/setup_set.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/huhk/init_project.py` & `huhk-1.7.6/huhk/init_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os.path
 import re
 import sys
 import requests
 import time
 
 from huhk.case_project.project_base import ProjectBase
+from huhk.unit_dict import Dict
 from huhk.unit_fun import FunBase
 from huhk import projects_path
 
 
 class GetApi(ProjectBase):
     def __init__(self, name=None, app_key=None, yapi_url=None, yapi_token=None, yapi_json_file=None, swagger_url=None):
         """
@@ -232,11 +233,20 @@
     def get_main_name():
         return GetApi._get_service_value("this_name", _type=1)
 
     @staticmethod
     def set_main_name(value):
         GetApi._set_service_value("this_name", value, _type=1)
 
+    @staticmethod
+    def get_key_name_list():
+        out = Dict()
+        for dirpath, dirnames, filenames in os.walk(projects_path):
+            for filename in filenames:
+                if "__init__.py" in filename:
+                    out[1] = 1
+        return True
+
 
 if __name__ == '__main__':
     ga = GetApi()
     print('--key：', ga.get_main_name())
```

### Comparing `huhk-1.7.5/huhk/testcase/apache/beam_class.py` & `huhk-1.7.6/huhk/testcase/apache/beam_class.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/huhk/testcase/apache/data.py` & `huhk-1.7.6/huhk/testcase/apache/data.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/huhk/testcase/apache/par_do.py` & `huhk-1.7.6/huhk/testcase/apache/par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/huhk/testcase/apache/test_cogroupbykey.py` & `huhk-1.7.6/huhk/testcase/apache/test_cogroupbykey.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/huhk/testcase/apache/test_fiter.py` & `huhk-1.7.6/huhk/testcase/apache/test_fiter.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/huhk/testcase/apache/test_flatmap.py` & `huhk-1.7.6/huhk/testcase/apache/test_flatmap.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/huhk/testcase/apache/test_map.py` & `huhk-1.7.6/huhk/testcase/apache/test_map.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/huhk/testcase/apache/test_par_do.py` & `huhk-1.7.6/huhk/testcase/apache/test_par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/huhk/testcase/apache/test_regex.py` & `huhk-1.7.6/huhk/testcase/apache/test_regex.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/huhk/testcase/apache/test_time.py` & `huhk-1.7.6/huhk/testcase/apache/test_time.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/huhk/unit_apache_beam.py` & `huhk-1.7.6/huhk/unit_apache_beam.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/huhk/unit_dict.py` & `huhk-1.7.6/huhk/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/huhk/unit_encryption.py` & `huhk-1.7.6/huhk/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/huhk/unit_fun.py` & `huhk-1.7.6/huhk/unit_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/huhk/unit_logger.py` & `huhk-1.7.6/huhk/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/huhk/unit_request.py` & `huhk-1.7.6/huhk/unit_request.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/huhk/unit_tasks.py` & `huhk-1.7.6/huhk/unit_tasks.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/huhk/常用命令.py` & `huhk-1.7.6/huhk/常用命令.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/huhk.egg-info/SOURCES.txt` & `huhk-1.7.6/huhk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 huhk.egg-info/SOURCES.txt
 huhk.egg-info/dependency_links.txt
 huhk.egg-info/entry_points.txt
 huhk.egg-info/requires.txt
 huhk.egg-info/top_level.txt
 huhk/case_project/__init__.py
 huhk/case_project/json_coder.py
-huhk/case_project/main.py
 huhk/case_project/main_fun.py
 huhk/case_project/project_base.py
 huhk/case_project/project_init.py
 huhk/case_project/project_string.py
 huhk/case_project/setup_set.py
 huhk/case_project/version.py
 huhk/testcase/__init__.py
```

### Comparing `huhk-1.7.5/service/app_t/apis/open/haohan/apis_open_haohan_relation.py` & `huhk-1.7.6/service/app_t/apis/open/haohan/apis_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/service/app_t/apis/open/haohan/apis_open_haohan_rights.py` & `huhk-1.7.6/service/app_t/apis/open/haohan/apis_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/service/app_t/apis/points/apis_points_points.py` & `huhk-1.7.6/service/app_t/apis/points/apis_points_points.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/service/app_t/apis/points/apis_points_pointsApp.py` & `huhk-1.7.6/service/app_t/apis/points/apis_points_pointsApp.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/service/app_t/app_t_fun.py` & `huhk-1.7.6/service/app_t/app_t_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/service/app_t/asserts/open/haohan/asserts_open_haohan_relation.py` & `huhk-1.7.6/service/app_t/asserts/open/haohan/asserts_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/service/app_t/asserts/open/haohan/asserts_open_haohan_rights.py` & `huhk-1.7.6/service/app_t/asserts/open/haohan/asserts_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/service/app_t/asserts/points/asserts_points_points.py` & `huhk-1.7.6/service/app_t/asserts/points/asserts_points_points.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/service/app_t/asserts/points/asserts_points_pointsApp.py` & `huhk-1.7.6/service/app_t/asserts/points/asserts_points_pointsApp.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/service/app_t/funs/open/haohan/funs_open_haohan_relation.py` & `huhk-1.7.6/service/app_t/funs/open/haohan/funs_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/service/app_t/funs/open/haohan/funs_open_haohan_rights.py` & `huhk-1.7.6/service/app_t/funs/open/haohan/funs_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/service/app_t/funs/points/funs_points_points.py` & `huhk-1.7.6/service/app_t/funs/points/funs_points_points.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/service/app_t/funs/points/funs_points_pointsApp.py` & `huhk-1.7.6/service/app_t/funs/points/funs_points_pointsApp.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/service/app_t/sqls/open/haohan/sqls_open_haohan_relation.py` & `huhk-1.7.6/service/app_t/sqls/open/haohan/sqls_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/service/app_t/sqls/open/haohan/sqls_open_haohan_rights.py` & `huhk-1.7.6/service/app_t/sqls/open/haohan/sqls_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/service/app_t/sqls/points/sqls_points_points.py` & `huhk-1.7.6/service/app_t/sqls/points/sqls_points_points.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.5/service/app_t/sqls/points/sqls_points_pointsApp.py` & `huhk-1.7.6/service/app_t/sqls/points/sqls_points_pointsApp.py`

 * *Files identical despite different names*

