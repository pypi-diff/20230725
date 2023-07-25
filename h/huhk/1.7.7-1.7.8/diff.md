# Comparing `tmp/huhk-1.7.7.tar.gz` & `tmp/huhk-1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhk-1.7.7.tar", last modified: Tue Jul 25 07:13:35 2023, max compression
+gzip compressed data, was "huhk-1.7.8.tar", last modified: Tue Jul 25 08:27:27 2023, max compression
```

## Comparing `huhk-1.7.7.tar` & `huhk-1.7.8.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 07:13:35.022909 huhk-1.7.7/
--rw-rw-rw-   0        0        0      223 2023-07-25 07:13:35.021904 huhk-1.7.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-25 07:13:34.848073 huhk-1.7.7/huhk/
--rw-rw-rw-   0        0        0      772 2023-07-17 02:44:39.000000 huhk-1.7.7/huhk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:13:34.879412 huhk-1.7.7/huhk/case_project/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.7.7/huhk/case_project/__init__.py
--rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.7.7/huhk/case_project/json_coder.py
--rw-rw-rw-   0        0        0      834 2023-07-25 07:12:11.000000 huhk-1.7.7/huhk/case_project/main_fun.py
--rw-rw-rw-   0        0        0    17758 2023-07-24 09:52:23.000000 huhk-1.7.7/huhk/case_project/project_base.py
--rw-rw-rw-   0        0        0     2099 2023-07-21 08:18:22.000000 huhk-1.7.7/huhk/case_project/project_init.py
--rw-rw-rw-   0        0        0    13835 2023-07-24 01:29:57.000000 huhk-1.7.7/huhk/case_project/project_string.py
--rw-rw-rw-   0        0        0      908 2023-07-12 01:13:24.000000 huhk-1.7.7/huhk/case_project/setup_set.py
--rw-rw-rw-   0        0        0       17 2023-07-25 07:13:34.000000 huhk-1.7.7/huhk/case_project/version.py
--rw-rw-rw-   0        0        0    14758 2023-07-25 07:02:40.000000 huhk-1.7.7/huhk/init_project.py
--rw-rw-rw-   0        0        0     1355 2023-07-25 07:12:34.000000 huhk-1.7.7/huhk/main.py
--rw-rw-rw-   0        0        0      336 2023-07-25 02:56:17.000000 huhk-1.7.7/huhk/setup_run.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:13:34.882373 huhk-1.7.7/huhk/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.7.7/huhk/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:13:34.925299 huhk-1.7.7/huhk/testcase/apache/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.7.7/huhk/testcase/apache/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.7.7/huhk/testcase/apache/beam_class.py
--rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.7.7/huhk/testcase/apache/data.py
--rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.7.7/huhk/testcase/apache/par_do.py
--rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.7.7/huhk/testcase/apache/test_cogroupbykey.py
--rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.7.7/huhk/testcase/apache/test_file.py
--rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.7.7/huhk/testcase/apache/test_fiter.py
--rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.7.7/huhk/testcase/apache/test_flatmap.py
--rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.7.7/huhk/testcase/apache/test_map.py
--rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.7.7/huhk/testcase/apache/test_par_do.py
--rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.7.7/huhk/testcase/apache/test_regex.py
--rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.7.7/huhk/testcase/apache/test_time.py
--rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.7.7/huhk/testcase/apache/test_to_string.py
--rw-rw-rw-   0        0        0    22615 2023-07-14 06:52:17.000000 huhk-1.7.7/huhk/unit_apache_beam.py
--rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.7.7/huhk/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.7.7/huhk/unit_encryption.py
--rw-rw-rw-   0        0        0    28445 2023-07-22 10:41:46.000000 huhk-1.7.7/huhk/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.7.7/huhk/unit_logger.py
--rw-rw-rw-   0        0        0     9960 2023-07-22 07:06:52.000000 huhk-1.7.7/huhk/unit_request.py
--rw-rw-rw-   0        0        0     2511 2023-07-24 06:56:32.000000 huhk-1.7.7/huhk/unit_tasks.py
--rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.7.7/huhk/常用命令.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:13:34.859036 huhk-1.7.7/huhk.egg-info/
--rw-rw-rw-   0        0        0      223 2023-07-25 07:13:34.000000 huhk-1.7.7/huhk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2880 2023-07-25 07:13:34.000000 huhk-1.7.7/huhk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 07:13:34.000000 huhk-1.7.7/huhk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-07-25 07:13:34.000000 huhk-1.7.7/huhk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      134 2023-07-25 07:13:34.000000 huhk-1.7.7/huhk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-25 07:13:34.000000 huhk-1.7.7/huhk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-25 07:13:34.928290 huhk-1.7.7/service/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.7/service/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:13:34.934275 huhk-1.7.7/service/app_t/
--rw-rw-rw-   0        0        0      420 2023-07-22 06:54:11.000000 huhk-1.7.7/service/app_t/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:13:34.936269 huhk-1.7.7/service/app_t/apis/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.7/service/app_t/apis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:13:34.939263 huhk-1.7.7/service/app_t/apis/open/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.7/service/app_t/apis/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:13:34.946248 huhk-1.7.7/service/app_t/apis/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.7/service/app_t/apis/open/haohan/__init__.py
--rw-rw-rw-   0        0        0    22236 2023-07-24 01:53:24.000000 huhk-1.7.7/service/app_t/apis/open/haohan/apis_open_haohan_relation.py
--rw-rw-rw-   0        0        0    23259 2023-07-24 01:53:26.000000 huhk-1.7.7/service/app_t/apis/open/haohan/apis_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:13:34.954191 huhk-1.7.7/service/app_t/apis/points/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.7/service/app_t/apis/points/__init__.py
--rw-rw-rw-   0        0        0    31535 2023-07-24 01:53:27.000000 huhk-1.7.7/service/app_t/apis/points/apis_points_points.py
--rw-rw-rw-   0        0        0    25708 2023-07-24 01:53:27.000000 huhk-1.7.7/service/app_t/apis/points/apis_points_pointsApp.py
--rw-rw-rw-   0        0        0      650 2023-07-22 10:57:15.000000 huhk-1.7.7/service/app_t/app_t_fun.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:13:34.956185 huhk-1.7.7/service/app_t/asserts/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.7/service/app_t/asserts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:13:34.958181 huhk-1.7.7/service/app_t/asserts/open/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.7/service/app_t/asserts/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:13:34.965737 huhk-1.7.7/service/app_t/asserts/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.7/service/app_t/asserts/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      602 2023-07-22 06:51:21.000000 huhk-1.7.7/service/app_t/asserts/open/haohan/asserts_open_haohan_relation.py
--rw-rw-rw-   0        0        0      590 2023-07-22 06:51:21.000000 huhk-1.7.7/service/app_t/asserts/open/haohan/asserts_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:13:34.973715 huhk-1.7.7/service/app_t/asserts/points/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.7/service/app_t/asserts/points/__init__.py
--rw-rw-rw-   0        0        0     1761 2023-07-22 07:08:51.000000 huhk-1.7.7/service/app_t/asserts/points/asserts_points_points.py
--rw-rw-rw-   0        0        0     1358 2023-07-22 06:51:21.000000 huhk-1.7.7/service/app_t/asserts/points/asserts_points_pointsApp.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:13:34.981719 huhk-1.7.7/service/app_t/funs/
--rw-rw-rw-   0        0        0        0 2023-07-24 01:53:24.000000 huhk-1.7.7/service/app_t/funs/__init__.py
--rw-rw-rw-   0        0        0      161 2023-07-24 01:53:33.000000 huhk-1.7.7/service/app_t/funs/funs_app_t.py
--rw-rw-rw-   0        0        0      118 2023-07-24 01:53:32.000000 huhk-1.7.7/service/app_t/funs/funs_open.py
--rw-rw-rw-   0        0        0      230 2023-07-24 01:53:33.000000 huhk-1.7.7/service/app_t/funs/funs_points.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:13:34.986000 huhk-1.7.7/service/app_t/funs/open/
--rw-rw-rw-   0        0        0        0 2023-07-24 01:53:27.000000 huhk-1.7.7/service/app_t/funs/open/__init__.py
--rw-rw-rw-   0        0        0      267 2023-07-24 01:53:31.000000 huhk-1.7.7/service/app_t/funs/open/funs_open_haohan.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:13:34.990991 huhk-1.7.7/service/app_t/funs/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-24 01:53:27.000000 huhk-1.7.7/service/app_t/funs/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      824 2023-07-24 01:53:27.000000 huhk-1.7.7/service/app_t/funs/open/haohan/funs_open_haohan_relation.py
--rw-rw-rw-   0        0        0      910 2023-07-24 01:53:31.000000 huhk-1.7.7/service/app_t/funs/open/haohan/funs_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:13:34.997973 huhk-1.7.7/service/app_t/funs/points/
--rw-rw-rw-   0        0        0        0 2023-07-24 01:53:32.000000 huhk-1.7.7/service/app_t/funs/points/__init__.py
--rw-rw-rw-   0        0        0     3103 2023-07-24 01:53:34.000000 huhk-1.7.7/service/app_t/funs/points/funs_points_points.py
--rw-rw-rw-   0        0        0     1899 2023-07-24 01:53:33.000000 huhk-1.7.7/service/app_t/funs/points/funs_points_pointsApp.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:13:34.999967 huhk-1.7.7/service/app_t/sqls/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.7/service/app_t/sqls/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:13:35.001962 huhk-1.7.7/service/app_t/sqls/open/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.7/service/app_t/sqls/open/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:13:35.008949 huhk-1.7.7/service/app_t/sqls/open/haohan/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.7/service/app_t/sqls/open/haohan/__init__.py
--rw-rw-rw-   0        0        0      571 2023-07-22 06:51:21.000000 huhk-1.7.7/service/app_t/sqls/open/haohan/sqls_open_haohan_relation.py
--rw-rw-rw-   0        0        0      567 2023-07-22 06:51:21.000000 huhk-1.7.7/service/app_t/sqls/open/haohan/sqls_open_haohan_rights.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:13:35.016923 huhk-1.7.7/service/app_t/sqls/points/
--rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.7/service/app_t/sqls/points/__init__.py
--rw-rw-rw-   0        0        0     1994 2023-07-22 06:51:21.000000 huhk-1.7.7/service/app_t/sqls/points/sqls_points_points.py
--rw-rw-rw-   0        0        0     1529 2023-07-22 06:51:21.000000 huhk-1.7.7/service/app_t/sqls/points/sqls_points_pointsApp.py
--rw-rw-rw-   0        0        0       42 2023-07-25 07:13:35.022909 huhk-1.7.7/setup.cfg
--rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.7.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:13:35.019901 huhk-1.7.7/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-25 03:05:04.000000 huhk-1.7.7/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:27:27.473794 huhk-1.7.8/
+-rw-rw-rw-   0        0        0      223 2023-07-25 08:27:27.472255 huhk-1.7.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-25 08:27:27.301966 huhk-1.7.8/huhk/
+-rw-rw-rw-   0        0        0      772 2023-07-17 02:44:39.000000 huhk-1.7.8/huhk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:27:27.334845 huhk-1.7.8/huhk/case_project/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.7.8/huhk/case_project/__init__.py
+-rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.7.8/huhk/case_project/json_coder.py
+-rw-rw-rw-   0        0        0      913 2023-07-25 07:17:28.000000 huhk-1.7.8/huhk/case_project/main_fun.py
+-rw-rw-rw-   0        0        0    18249 2023-07-25 08:26:01.000000 huhk-1.7.8/huhk/case_project/project_base.py
+-rw-rw-rw-   0        0        0     2099 2023-07-21 08:18:22.000000 huhk-1.7.8/huhk/case_project/project_init.py
+-rw-rw-rw-   0        0        0    13835 2023-07-24 01:29:57.000000 huhk-1.7.8/huhk/case_project/project_string.py
+-rw-rw-rw-   0        0        0      908 2023-07-12 01:13:24.000000 huhk-1.7.8/huhk/case_project/setup_set.py
+-rw-rw-rw-   0        0        0       17 2023-07-25 08:27:27.000000 huhk-1.7.8/huhk/case_project/version.py
+-rw-rw-rw-   0        0        0    14792 2023-07-25 08:18:17.000000 huhk-1.7.8/huhk/init_project.py
+-rw-rw-rw-   0        0        0     1355 2023-07-25 07:12:34.000000 huhk-1.7.8/huhk/main.py
+-rw-rw-rw-   0        0        0      336 2023-07-25 02:56:17.000000 huhk-1.7.8/huhk/setup_run.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:27:27.335843 huhk-1.7.8/huhk/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.7.8/huhk/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:27:27.374842 huhk-1.7.8/huhk/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.7.8/huhk/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.7.8/huhk/testcase/apache/beam_class.py
+-rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.7.8/huhk/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.7.8/huhk/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.7.8/huhk/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.7.8/huhk/testcase/apache/test_file.py
+-rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.7.8/huhk/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.7.8/huhk/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.7.8/huhk/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.7.8/huhk/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.7.8/huhk/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.7.8/huhk/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.7.8/huhk/testcase/apache/test_to_string.py
+-rw-rw-rw-   0        0        0    22615 2023-07-14 06:52:17.000000 huhk-1.7.8/huhk/unit_apache_beam.py
+-rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.7.8/huhk/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.7.8/huhk/unit_encryption.py
+-rw-rw-rw-   0        0        0    28445 2023-07-22 10:41:46.000000 huhk-1.7.8/huhk/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.7.8/huhk/unit_logger.py
+-rw-rw-rw-   0        0        0     9960 2023-07-22 07:06:52.000000 huhk-1.7.8/huhk/unit_request.py
+-rw-rw-rw-   0        0        0     2511 2023-07-24 06:56:32.000000 huhk-1.7.8/huhk/unit_tasks.py
+-rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.7.8/huhk/常用命令.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:27:27.312903 huhk-1.7.8/huhk.egg-info/
+-rw-rw-rw-   0        0        0      223 2023-07-25 08:27:27.000000 huhk-1.7.8/huhk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2880 2023-07-25 08:27:27.000000 huhk-1.7.8/huhk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 08:27:27.000000 huhk-1.7.8/huhk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-25 08:27:27.000000 huhk-1.7.8/huhk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      134 2023-07-25 08:27:27.000000 huhk-1.7.8/huhk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-25 08:27:27.000000 huhk-1.7.8/huhk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 08:27:27.376837 huhk-1.7.8/service/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.8/service/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:27:27.383819 huhk-1.7.8/service/app_t/
+-rw-rw-rw-   0        0        0      420 2023-07-22 06:54:11.000000 huhk-1.7.8/service/app_t/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:27:27.384817 huhk-1.7.8/service/app_t/apis/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.8/service/app_t/apis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:27:27.387847 huhk-1.7.8/service/app_t/apis/open/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.8/service/app_t/apis/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:27:27.393832 huhk-1.7.8/service/app_t/apis/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.8/service/app_t/apis/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0    22236 2023-07-24 01:53:24.000000 huhk-1.7.8/service/app_t/apis/open/haohan/apis_open_haohan_relation.py
+-rw-rw-rw-   0        0        0    23259 2023-07-24 01:53:26.000000 huhk-1.7.8/service/app_t/apis/open/haohan/apis_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:27:27.400805 huhk-1.7.8/service/app_t/apis/points/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.8/service/app_t/apis/points/__init__.py
+-rw-rw-rw-   0        0        0    31535 2023-07-24 01:53:27.000000 huhk-1.7.8/service/app_t/apis/points/apis_points_points.py
+-rw-rw-rw-   0        0        0    25708 2023-07-24 01:53:27.000000 huhk-1.7.8/service/app_t/apis/points/apis_points_pointsApp.py
+-rw-rw-rw-   0        0        0      650 2023-07-22 10:57:15.000000 huhk-1.7.8/service/app_t/app_t_fun.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:27:27.402794 huhk-1.7.8/service/app_t/asserts/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.8/service/app_t/asserts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:27:27.405760 huhk-1.7.8/service/app_t/asserts/open/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.8/service/app_t/asserts/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:27:27.412397 huhk-1.7.8/service/app_t/asserts/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.8/service/app_t/asserts/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      602 2023-07-22 06:51:21.000000 huhk-1.7.8/service/app_t/asserts/open/haohan/asserts_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      590 2023-07-22 06:51:21.000000 huhk-1.7.8/service/app_t/asserts/open/haohan/asserts_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:27:27.421347 huhk-1.7.8/service/app_t/asserts/points/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.8/service/app_t/asserts/points/__init__.py
+-rw-rw-rw-   0        0        0     1761 2023-07-22 07:08:51.000000 huhk-1.7.8/service/app_t/asserts/points/asserts_points_points.py
+-rw-rw-rw-   0        0        0     1358 2023-07-22 06:51:21.000000 huhk-1.7.8/service/app_t/asserts/points/asserts_points_pointsApp.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:27:27.429327 huhk-1.7.8/service/app_t/funs/
+-rw-rw-rw-   0        0        0        0 2023-07-24 01:53:24.000000 huhk-1.7.8/service/app_t/funs/__init__.py
+-rw-rw-rw-   0        0        0      161 2023-07-24 01:53:33.000000 huhk-1.7.8/service/app_t/funs/funs_app_t.py
+-rw-rw-rw-   0        0        0      118 2023-07-24 01:53:32.000000 huhk-1.7.8/service/app_t/funs/funs_open.py
+-rw-rw-rw-   0        0        0      230 2023-07-24 01:53:33.000000 huhk-1.7.8/service/app_t/funs/funs_points.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:27:27.433317 huhk-1.7.8/service/app_t/funs/open/
+-rw-rw-rw-   0        0        0        0 2023-07-24 01:53:27.000000 huhk-1.7.8/service/app_t/funs/open/__init__.py
+-rw-rw-rw-   0        0        0      267 2023-07-24 01:53:31.000000 huhk-1.7.8/service/app_t/funs/open/funs_open_haohan.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:27:27.440297 huhk-1.7.8/service/app_t/funs/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-24 01:53:27.000000 huhk-1.7.8/service/app_t/funs/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      824 2023-07-24 01:53:27.000000 huhk-1.7.8/service/app_t/funs/open/haohan/funs_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      910 2023-07-24 01:53:31.000000 huhk-1.7.8/service/app_t/funs/open/haohan/funs_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:27:27.447280 huhk-1.7.8/service/app_t/funs/points/
+-rw-rw-rw-   0        0        0        0 2023-07-24 01:53:32.000000 huhk-1.7.8/service/app_t/funs/points/__init__.py
+-rw-rw-rw-   0        0        0     3103 2023-07-24 01:53:34.000000 huhk-1.7.8/service/app_t/funs/points/funs_points_points.py
+-rw-rw-rw-   0        0        0     1899 2023-07-24 01:53:33.000000 huhk-1.7.8/service/app_t/funs/points/funs_points_pointsApp.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:27:27.449299 huhk-1.7.8/service/app_t/sqls/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:20.000000 huhk-1.7.8/service/app_t/sqls/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:27:27.451302 huhk-1.7.8/service/app_t/sqls/open/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.8/service/app_t/sqls/open/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:27:27.458290 huhk-1.7.8/service/app_t/sqls/open/haohan/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.8/service/app_t/sqls/open/haohan/__init__.py
+-rw-rw-rw-   0        0        0      571 2023-07-22 06:51:21.000000 huhk-1.7.8/service/app_t/sqls/open/haohan/sqls_open_haohan_relation.py
+-rw-rw-rw-   0        0        0      567 2023-07-22 06:51:21.000000 huhk-1.7.8/service/app_t/sqls/open/haohan/sqls_open_haohan_rights.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:27:27.467226 huhk-1.7.8/service/app_t/sqls/points/
+-rw-rw-rw-   0        0        0        0 2023-07-22 06:51:21.000000 huhk-1.7.8/service/app_t/sqls/points/__init__.py
+-rw-rw-rw-   0        0        0     1994 2023-07-22 06:51:21.000000 huhk-1.7.8/service/app_t/sqls/points/sqls_points_points.py
+-rw-rw-rw-   0        0        0     1529 2023-07-22 06:51:21.000000 huhk-1.7.8/service/app_t/sqls/points/sqls_points_pointsApp.py
+-rw-rw-rw-   0        0        0       42 2023-07-25 08:27:27.473794 huhk-1.7.8/setup.cfg
+-rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.7.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:27:27.470218 huhk-1.7.8/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-25 03:05:04.000000 huhk-1.7.8/testcase/__init__.py
```

### Comparing `huhk-1.7.7/huhk/__init__.py` & `huhk-1.7.8/huhk/__init__.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/huhk/case_project/json_coder.py` & `huhk-1.7.8/huhk/case_project/json_coder.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/huhk/case_project/main_fun.py` & `huhk-1.7.8/huhk/case_project/main_fun.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,19 @@
     if key and name:
         GetApi.set_main_key(key)
         GetApi.set_main_name(name)
     elif key or name:
         key_list = GetApi.get_key_name_list()
         if key:
             GetApi.set_main_key(key)
-            GetApi.set_main_name(key_list.get(key))
+            if key_list.get(key):
+                GetApi.set_main_name(key_list.get(key))
         else:
-            GetApi.set_main_key(key_list.get(name))
+            if key_list.get(name):
+                GetApi.set_main_key(key_list.get(name))
             GetApi.set_main_name(name)
     return True
 
 
 def install_project(app_key, name=None):
     ga = GetApi(name=name, app_key=app_key)
     ga.create_or_update_project()
```

### Comparing `huhk-1.7.7/huhk/case_project/project_base.py` & `huhk-1.7.8/huhk/case_project/project_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,27 +31,38 @@
                     data = json.load(fp)
                     if key:
                         if data.get(key):
                             return data[key]
                     else:
                         return data
 
-        service_json_path = os.path.join(projects_path, "service", "setting.json")
+        service_json_path = ProjectBase.get_setting_path()
         if os.path.exists(service_json_path):
             with open(service_json_path, encoding="utf-8") as fp:
                 data = json.load(fp)
                 return data.get(key, default) if key else data
         return default
 
     @staticmethod
+    def get_setting_path(path=None):
+        path = path or projects_path
+        for dirpath, dirnames, filenames in os.walk(path):
+            if "apis" in dirnames and "asserts" in dirnames and "funs" in dirnames and "sqls" in dirnames \
+                    and "__init__.py" in filenames:
+                return os.path.join(os.path.dirname(dirpath), "setting.json")
+        if os.path.exists(os.path.dirname(path)) and len(path) > 5:
+            return ProjectBase.get_setting_path(os.path.dirname(path))
+        return None
+
+    @staticmethod
     def _set_service_value(key, value, name=None, _type=0):
         if _type == 0:
             service_json_path = os.path.join(projects_path, "service", name, name + "_setting.json")
         else:
-            service_json_path = os.path.join(projects_path, "service", "setting.json")
+            service_json_path = ProjectBase.get_setting_path()
         if os.path.exists(service_json_path):
             with open(service_json_path) as fp:
                 data = json.load(fp)
         else:
             data = {}
         data[key] = value
         with open(service_json_path, 'w') as fp:
@@ -327,9 +338,9 @@
             FunBase.write_file(fun_path.path, file_str)
             self.set_api_fun_header(fun_name)
 
 
 if __name__ == "__main__":
     a = ProjectBase(name="app_t")
     a.dir = r"D:\projects\python_test\huhk-common"
-    o = a.get_path("open_haohan_relation_update")
+    o = a.get_setting_path()
     print(o)
```

### Comparing `huhk-1.7.7/huhk/case_project/project_init.py` & `huhk-1.7.8/huhk/case_project/project_init.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/huhk/case_project/project_string.py` & `huhk-1.7.8/huhk/case_project/project_string.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/huhk/case_project/setup_set.py` & `huhk-1.7.8/huhk/case_project/setup_set.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/huhk/init_project.py` & `huhk-1.7.8/huhk/init_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,15 +254,15 @@
                     out[name] = app_key
                     out[app_key] = name
                 else:
                     out[name] = None
         if out:
             return out
         else:
-            if os.path.dirname(path):
+            if os.path.exists(os.path.dirname(path)) and len(path) > 5:
                 return GetApi.get_key_name_list(os.path.dirname(path))
         return out
 
 
 if __name__ == '__main__':
     ga = GetApi()
     print(ga.get_key_name_list())
```

### Comparing `huhk-1.7.7/huhk/main.py` & `huhk-1.7.8/huhk/main.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/huhk/testcase/apache/beam_class.py` & `huhk-1.7.8/huhk/testcase/apache/beam_class.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/huhk/testcase/apache/data.py` & `huhk-1.7.8/huhk/testcase/apache/data.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/huhk/testcase/apache/par_do.py` & `huhk-1.7.8/huhk/testcase/apache/par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/huhk/testcase/apache/test_cogroupbykey.py` & `huhk-1.7.8/huhk/testcase/apache/test_cogroupbykey.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/huhk/testcase/apache/test_fiter.py` & `huhk-1.7.8/huhk/testcase/apache/test_fiter.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/huhk/testcase/apache/test_flatmap.py` & `huhk-1.7.8/huhk/testcase/apache/test_flatmap.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/huhk/testcase/apache/test_map.py` & `huhk-1.7.8/huhk/testcase/apache/test_map.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/huhk/testcase/apache/test_par_do.py` & `huhk-1.7.8/huhk/testcase/apache/test_par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/huhk/testcase/apache/test_regex.py` & `huhk-1.7.8/huhk/testcase/apache/test_regex.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/huhk/testcase/apache/test_time.py` & `huhk-1.7.8/huhk/testcase/apache/test_time.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/huhk/unit_apache_beam.py` & `huhk-1.7.8/huhk/unit_apache_beam.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/huhk/unit_dict.py` & `huhk-1.7.8/huhk/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/huhk/unit_encryption.py` & `huhk-1.7.8/huhk/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/huhk/unit_fun.py` & `huhk-1.7.8/huhk/unit_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/huhk/unit_logger.py` & `huhk-1.7.8/huhk/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/huhk/unit_request.py` & `huhk-1.7.8/huhk/unit_request.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/huhk/unit_tasks.py` & `huhk-1.7.8/huhk/unit_tasks.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/huhk/常用命令.py` & `huhk-1.7.8/huhk/常用命令.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/huhk.egg-info/SOURCES.txt` & `huhk-1.7.8/huhk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/service/app_t/apis/open/haohan/apis_open_haohan_relation.py` & `huhk-1.7.8/service/app_t/apis/open/haohan/apis_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/service/app_t/apis/open/haohan/apis_open_haohan_rights.py` & `huhk-1.7.8/service/app_t/apis/open/haohan/apis_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/service/app_t/apis/points/apis_points_points.py` & `huhk-1.7.8/service/app_t/apis/points/apis_points_points.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/service/app_t/apis/points/apis_points_pointsApp.py` & `huhk-1.7.8/service/app_t/apis/points/apis_points_pointsApp.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/service/app_t/app_t_fun.py` & `huhk-1.7.8/service/app_t/app_t_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/service/app_t/asserts/open/haohan/asserts_open_haohan_relation.py` & `huhk-1.7.8/service/app_t/asserts/open/haohan/asserts_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/service/app_t/asserts/open/haohan/asserts_open_haohan_rights.py` & `huhk-1.7.8/service/app_t/asserts/open/haohan/asserts_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/service/app_t/asserts/points/asserts_points_points.py` & `huhk-1.7.8/service/app_t/asserts/points/asserts_points_points.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/service/app_t/asserts/points/asserts_points_pointsApp.py` & `huhk-1.7.8/service/app_t/asserts/points/asserts_points_pointsApp.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/service/app_t/funs/open/haohan/funs_open_haohan_relation.py` & `huhk-1.7.8/service/app_t/funs/open/haohan/funs_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/service/app_t/funs/open/haohan/funs_open_haohan_rights.py` & `huhk-1.7.8/service/app_t/funs/open/haohan/funs_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/service/app_t/funs/points/funs_points_points.py` & `huhk-1.7.8/service/app_t/funs/points/funs_points_points.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/service/app_t/funs/points/funs_points_pointsApp.py` & `huhk-1.7.8/service/app_t/funs/points/funs_points_pointsApp.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/service/app_t/sqls/open/haohan/sqls_open_haohan_relation.py` & `huhk-1.7.8/service/app_t/sqls/open/haohan/sqls_open_haohan_relation.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/service/app_t/sqls/open/haohan/sqls_open_haohan_rights.py` & `huhk-1.7.8/service/app_t/sqls/open/haohan/sqls_open_haohan_rights.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/service/app_t/sqls/points/sqls_points_points.py` & `huhk-1.7.8/service/app_t/sqls/points/sqls_points_points.py`

 * *Files identical despite different names*

### Comparing `huhk-1.7.7/service/app_t/sqls/points/sqls_points_pointsApp.py` & `huhk-1.7.8/service/app_t/sqls/points/sqls_points_pointsApp.py`

 * *Files identical despite different names*

