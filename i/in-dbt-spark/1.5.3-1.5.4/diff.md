# Comparing `tmp/in-dbt-spark-1.5.3.tar.gz` & `tmp/in-dbt-spark-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "in-dbt-spark-1.5.3.tar", last modified: Tue Jul 11 13:04:29 2023, max compression
+gzip compressed data, was "in-dbt-spark-1.5.4.tar", last modified: Tue Jul 25 09:32:25 2023, max compression
```

## Comparing `in-dbt-spark-1.5.3.tar` & `in-dbt-spark-1.5.4.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:04:29.938447 in-dbt-spark-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-07-11 13:04:29.934447 in-dbt-spark-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:04:29.926447 in-dbt-spark-1.5.3/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:04:29.926447 in-dbt-spark-1.5.3/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:04:29.930447 in-dbt-spark-1.5.3/dbt/adapters/setu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/adapters/setu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/adapters/setu/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/adapters/setu/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/adapters/setu/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/adapters/setu/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/adapters/setu/session_cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/adapters/setu/session_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/adapters/setu/session_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/adapters/setu/setu_session_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/adapters/setu/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:04:29.930447 in-dbt-spark-1.5.3/dbt/adapters/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/adapters/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/adapters/spark/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/adapters/spark/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    25781 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/adapters/spark/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    29624 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/adapters/spark/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/adapters/spark/python_submissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/adapters/spark/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/adapters/spark/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/adapters/spark/spark_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:04:29.926447 in-dbt-spark-1.5.3/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:04:29.930447 in-dbt-spark-1.5.3/dbt/include/spark/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/include/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/include/spark/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:04:29.934447 in-dbt-spark-1.5.3/dbt/include/spark/macros/
--rw-r--r--   0 runner    (1001) docker     (123)    21436 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/include/spark/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/include/spark/macros/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/include/spark/macros/apply_retention.sql
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/include/spark/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:04:29.934447 in-dbt-spark-1.5.3/dbt/include/spark/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:04:29.934447 in-dbt-spark-1.5.3/dbt/include/spark/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/include/spark/macros/materializations/incremental/column_helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/include/spark/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/include/spark/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/include/spark/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (123)    11791 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/include/spark/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/include/spark/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/include/spark/macros/materializations/validate.sql
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/include/spark/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:04:29.934447 in-dbt-spark-1.5.3/dbt/include/spark/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/include/spark/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/include/spark/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/include/spark/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/include/spark/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/include/spark/macros/utils/assert_not_null.sql
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/include/spark/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/include/spark/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/include/spark/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/include/spark/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/include/spark/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/include/spark/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/include/spark/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/include/spark/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/dbt/include/spark/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:04:29.934447 in-dbt-spark-1.5.3/in_dbt_spark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-07-11 13:04:29.000000 in-dbt-spark-1.5.3/in_dbt_spark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-11 13:04:29.000000 in-dbt-spark-1.5.3/in_dbt_spark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 13:04:29.000000 in-dbt-spark-1.5.3/in_dbt_spark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 13:04:29.000000 in-dbt-spark-1.5.3/in_dbt_spark.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-11 13:04:29.000000 in-dbt-spark-1.5.3/in_dbt_spark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-11 13:04:29.000000 in-dbt-spark-1.5.3/in_dbt_spark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 13:04:29.938447 in-dbt-spark-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-11 13:04:17.000000 in-dbt-spark-1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:32:25.034123 in-dbt-spark-1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-07-25 09:32:25.030123 in-dbt-spark-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:32:25.022123 in-dbt-spark-1.5.4/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:32:25.022123 in-dbt-spark-1.5.4/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:32:25.026123 in-dbt-spark-1.5.4/dbt/adapters/setu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/adapters/setu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/adapters/setu/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/adapters/setu/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/adapters/setu/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/adapters/setu/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/adapters/setu/session_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/adapters/setu/session_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/adapters/setu/session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/adapters/setu/setu_session_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/adapters/setu/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:32:25.026123 in-dbt-spark-1.5.4/dbt/adapters/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/adapters/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/adapters/spark/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/adapters/spark/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25781 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/adapters/spark/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30262 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/adapters/spark/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/adapters/spark/python_submissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/adapters/spark/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/adapters/spark/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/adapters/spark/spark_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:32:25.022123 in-dbt-spark-1.5.4/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:32:25.026123 in-dbt-spark-1.5.4/dbt/include/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/include/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/include/spark/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:32:25.030123 in-dbt-spark-1.5.4/dbt/include/spark/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)    21443 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/include/spark/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/include/spark/macros/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/include/spark/macros/apply_retention.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/include/spark/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:32:25.030123 in-dbt-spark-1.5.4/dbt/include/spark/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:32:25.030123 in-dbt-spark-1.5.4/dbt/include/spark/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/include/spark/macros/materializations/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/include/spark/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/include/spark/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/include/spark/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/include/spark/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/include/spark/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/include/spark/macros/materializations/validate.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/include/spark/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:32:25.030123 in-dbt-spark-1.5.4/dbt/include/spark/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/include/spark/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/include/spark/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/include/spark/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/include/spark/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/include/spark/macros/utils/assert_not_null.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/include/spark/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/include/spark/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/include/spark/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/include/spark/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/include/spark/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/include/spark/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/include/spark/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/include/spark/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/dbt/include/spark/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:32:25.030123 in-dbt-spark-1.5.4/in_dbt_spark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-07-25 09:32:24.000000 in-dbt-spark-1.5.4/in_dbt_spark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-25 09:32:24.000000 in-dbt-spark-1.5.4/in_dbt_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 09:32:24.000000 in-dbt-spark-1.5.4/in_dbt_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 09:32:24.000000 in-dbt-spark-1.5.4/in_dbt_spark.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-25 09:32:24.000000 in-dbt-spark-1.5.4/in_dbt_spark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-25 09:32:24.000000 in-dbt-spark-1.5.4/in_dbt_spark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 09:32:25.034123 in-dbt-spark-1.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-25 09:32:13.000000 in-dbt-spark-1.5.4/setup.py
```

### Comparing `in-dbt-spark-1.5.3/PKG-INFO` & `in-dbt-spark-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: in-dbt-spark
-Version: 1.5.3
+Version: 1.5.4
 Summary: Release for LinkedIn's changes to dbt-spark.
 Home-page: https://github.com/linkedin/in-dbt-spark
 Author: LinkedIn DBT Team
 Author-email: dbt-dev@linkedin.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.5.3 Summary: Release for
+Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.5.4 Summary: Release for
 LinkedIn's changes to dbt-spark. Home-page: https://github.com/linkedin/in-dbt-
 spark Author: LinkedIn DBT Team Author-email: dbt-dev@linkedin.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.10 Requires-
 Python: >=3.10 Description-Content-Type: text/markdown Provides-Extra: ODBC
```

### Comparing `in-dbt-spark-1.5.3/README.md` & `in-dbt-spark-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.3/dbt/adapters/setu/client.py` & `in-dbt-spark-1.5.4/dbt/adapters/setu/client.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.3/dbt/adapters/setu/constants.py` & `in-dbt-spark-1.5.4/dbt/adapters/setu/constants.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.3/dbt/adapters/setu/models.py` & `in-dbt-spark-1.5.4/dbt/adapters/setu/models.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.3/dbt/adapters/setu/session.py` & `in-dbt-spark-1.5.4/dbt/adapters/setu/session.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.3/dbt/adapters/setu/session_cursor.py` & `in-dbt-spark-1.5.4/dbt/adapters/setu/session_cursor.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.3/dbt/adapters/setu/session_handler.py` & `in-dbt-spark-1.5.4/dbt/adapters/setu/session_handler.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.3/dbt/adapters/setu/session_manager.py` & `in-dbt-spark-1.5.4/dbt/adapters/setu/session_manager.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.3/dbt/adapters/setu/setu_session_request.py` & `in-dbt-spark-1.5.4/dbt/adapters/setu/setu_session_request.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.3/dbt/adapters/setu/utils.py` & `in-dbt-spark-1.5.4/dbt/adapters/setu/utils.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.3/dbt/adapters/spark/__init__.py` & `in-dbt-spark-1.5.4/dbt/adapters/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.3/dbt/adapters/spark/column.py` & `in-dbt-spark-1.5.4/dbt/adapters/spark/column.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.3/dbt/adapters/spark/connections.py` & `in-dbt-spark-1.5.4/dbt/adapters/spark/connections.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.3/dbt/adapters/spark/impl.py` & `in-dbt-spark-1.5.4/dbt/adapters/spark/impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -675,29 +675,43 @@
     @property
     def python_submission_helpers(self) -> Dict[str, Type[PythonJobHelper]]:
         return {
             "job_cluster": JobClusterPythonJobHelper,
             "all_purpose_cluster": AllPurposeClusterPythonJobHelper,
         }
 
-    def standardize_grants_dict(self, grants_table: agate.Table) -> dict:
+    def standardize_grants_dict(
+        self, grants_table: agate.Table, schema_relation: BaseRelation
+    ) -> dict:
         grants_dict: Dict[str, List[str]] = {}
-        for row in grants_table:
-            grantee = row["Principal"]
-            privilege = row["ActionType"]
-            object_type = row["ObjectType"]
+        if is_openhouse(schema_relation.database, schema_relation.schema):
+            for row in grants_table:
+                grantee = row["principal"]
+                privilege = row["privilege"]
 
-            # we only want to consider grants on this object
-            # (view or table both appear as 'TABLE')
-            # and we don't want to consider the OWN privilege
-            if object_type == "TABLE" and privilege != "OWN":
-                if privilege in grants_dict.keys():
-                    grants_dict[privilege].append(grantee)
-                else:
-                    grants_dict.update({privilege: [grantee]})
+                # we don't want to consider the ALTER privilege in OpenHouse
+                if privilege != "ALTER":
+                    if privilege in grants_dict.keys():
+                        grants_dict[privilege].append(grantee)
+                    else:
+                        grants_dict.update({privilege: [grantee]})
+        else:
+            for row in grants_table:
+                grantee = row["Principal"]
+                privilege = row["ActionType"]
+                object_type = row["ObjectType"]
+
+                # we only want to consider grants on this object
+                # (view or table both appear as 'TABLE')
+                # and we don't want to consider the OWN privilege
+                if object_type == "TABLE" and privilege != "OWN":
+                    if privilege in grants_dict.keys():
+                        grants_dict[privilege].append(grantee)
+                    else:
+                        grants_dict.update({privilege: [grantee]})
         return grants_dict
 
     @contextmanager
     def _catalog(self, catalog: Optional[str]) -> Iterator[None]:
         """
         A context manager to make the operation work in the specified catalog,
         and move back to the current catalog after the operation.
```

### Comparing `in-dbt-spark-1.5.3/dbt/adapters/spark/python_submissions.py` & `in-dbt-spark-1.5.4/dbt/adapters/spark/python_submissions.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.3/dbt/adapters/spark/relation.py` & `in-dbt-spark-1.5.4/dbt/adapters/spark/relation.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.3/dbt/adapters/spark/session.py` & `in-dbt-spark-1.5.4/dbt/adapters/spark/session.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.3/dbt/include/spark/macros/adapters.sql` & `in-dbt-spark-1.5.4/dbt/include/spark/macros/adapters.sql`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     {%- set partition_by_list = adapter.parse_partition_by(raw_partition_by) -%}
     {%- for partition_by in partition_by_list -%}
       {%- if file_format == 'openhouse' and partition_by.data_type | lower in ['timestamp'] -%}
         {%- if partition_by.granularity is none -%}
           {% do exceptions.raise_compiler_error("For partitioned tables with file_format = 'openhouse' and data_type = 'timestamp', granularity must be provided") %}
         {%- endif -%}
         {{ partition_by.granularity }}({{ partition_by.field }})
-      {%- elif file_format == 'openhouse' and partition_by.data_type | lower in ['string'] -%}
+      {%- elif file_format == 'openhouse' and partition_by.data_type | lower in ['string', 'int'] -%}
         {{ partition_by.field }}
       {%- else -%}
         {{ partition_by.field }}
       {%- endif -%}
       {%- if not loop.last -%},{%- endif -%}
     {%- endfor -%}
     )
```

### Comparing `in-dbt-spark-1.5.3/dbt/include/spark/macros/apply_grants.sql` & `in-dbt-spark-1.5.4/dbt/include/spark/macros/apply_grants.sql`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,22 @@
         -- We can make this more efficient in the future
       #}
         {{ return(True) }}
 
     {% endif %}
 {% endmacro %}
 
+{% macro spark__get_show_grant_sql(relation) %}
+    {% if config.get('file_format', default='openhouse') == 'openhouse' %}
+        show grants on table {{ relation }}
+    {%- else -%}
+        show grants on {{ relation }}
+    {%- endif %}
+{% endmacro %}
+
 {%- macro spark__get_grant_sql(relation, privilege, grantees) -%}
     {% if config.get('file_format', default='openhouse') == 'openhouse' %}
         grant {{ privilege }} on table {{ relation }} to {{ grantees[0] }}
     {%- else -%}
         grant {{ privilege }} on {{ relation }} to {{ adapter.quote(grantees[0]) }}
     {%- endif %}
 {%- endmacro %}
@@ -55,32 +63,38 @@
     {#-- Automatically enable sharing for OpenHouse outputs to allow GRANTS both within and outside of dbt --#}
     {% if file_format == 'openhouse' %}
         {{ set_sharing_enabled(relation, True) }}
     {% endif %}
     {#-- If grant_config is {} or None, this is a no-op --#}
     {% if grant_config %}
         {#-- OpenHouse file_formats support append-only granting behavior, ie., no automated revoking through dbt--#}
-        {% if should_revoke and file_format != 'openhouse' %}
+        {% if should_revoke %}
             {#-- We think previous grants may have carried over --#}
             {#-- Show current grants and calculate diffs --#}
             {% set current_grants_table = run_query(get_show_grant_sql(relation)) %}
-            {% set current_grants_dict = adapter.standardize_grants_dict(current_grants_table) %}
+            {% set current_grants_dict = adapter.standardize_grants_dict(current_grants_table, relation) %}
             {% set needs_granting = diff_of_two_dicts(grant_config, current_grants_dict) %}
-            {% set needs_revoking = diff_of_two_dicts(current_grants_dict, grant_config) %}
+            {% set needs_revoking = {} %}
+            {% if file_format != 'openhouse' %}
+                {% set needs_revoking = diff_of_two_dicts(current_grants_dict, grant_config) %}
+            {% endif %}
             {% if not (needs_granting or needs_revoking) %}
                 {{ log('On ' ~ relation ~': All grants are in place, no revocation or granting needed.')}}
             {% endif %}
         {% else %}
             {#-- We don't think there's any chance of previous grants having carried over. --#}
             {#-- Jump straight to granting what the user has configured. --#}
             {% set needs_revoking = {} %}
             {% set needs_granting = grant_config %}
         {% endif %}
         {% if needs_granting or needs_revoking %}
-            {% set revoke_statement_list = get_dcl_statement_list(relation, needs_revoking, get_revoke_sql) %}
+            {%- set revoke_statement_list = [] -%}
+            {% if file_format != 'openhouse' %}
+                {% set revoke_statement_list = get_dcl_statement_list(relation, needs_revoking, get_revoke_sql) %}
+            {% endif %}
             {% set grant_statement_list = get_dcl_statement_list(relation, needs_granting, get_grant_sql) %}
             {% set dcl_statement_list = revoke_statement_list + grant_statement_list %}
             {% if dcl_statement_list %}
                 {{ call_dcl_statements(dcl_statement_list) }}
             {% endif %}
         {% endif %}
     {% endif %}
```

### Comparing `in-dbt-spark-1.5.3/dbt/include/spark/macros/apply_retention.sql` & `in-dbt-spark-1.5.4/dbt/include/spark/macros/apply_retention.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.3/dbt/include/spark/macros/catalog.sql` & `in-dbt-spark-1.5.4/dbt/include/spark/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.3/dbt/include/spark/macros/materializations/incremental/column_helpers.sql` & `in-dbt-spark-1.5.4/dbt/include/spark/macros/materializations/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.3/dbt/include/spark/macros/materializations/incremental/incremental.sql` & `in-dbt-spark-1.5.4/dbt/include/spark/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.3/dbt/include/spark/macros/materializations/incremental/strategies.sql` & `in-dbt-spark-1.5.4/dbt/include/spark/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.3/dbt/include/spark/macros/materializations/seed.sql` & `in-dbt-spark-1.5.4/dbt/include/spark/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.3/dbt/include/spark/macros/materializations/snapshot.sql` & `in-dbt-spark-1.5.4/dbt/include/spark/macros/materializations/snapshot.sql`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,15 @@
   {%- set config = model['config'] -%}
 
   {%- set target_table = model.get('alias', model.get('name')) -%}
 
   {%- set strategy_name = config.get('strategy') -%}
   {%- set unique_key = config.get('unique_key') %}
   {%- set file_format = config.get('file_format', 'openhouse') -%}
+  {%- set grant_config = config.get('grants') -%}
 
   {% set target_relation_exists, target_relation = get_or_create_relation(
           database=model.database,
           schema=model.schema,
           identifier=target_table,
           type='table') -%}
```

### Comparing `in-dbt-spark-1.5.3/dbt/include/spark/macros/materializations/table.sql` & `in-dbt-spark-1.5.4/dbt/include/spark/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.3/dbt/include/spark/macros/materializations/validate.sql` & `in-dbt-spark-1.5.4/dbt/include/spark/macros/materializations/validate.sql`

 * *Files 1% similar despite different names*

```diff
@@ -88,16 +88,16 @@
       {% set partition_by_list = adapter.parse_partition_by(raw_partition_by) %}
       {% if partition_by_list|length > 4 %}
         {% do exceptions.raise_compiler_error("For partitioned tables with file_format = 'openhouse', the size of 'partition_by' must not be > 4.") %}
       {% endif %}
       {% if partition_by_list is not none %}
         {% set timestamp_columns = namespace(count=0) %}
         {%- for partition_by in partition_by_list -%}
-           {%- if partition_by.data_type.lower() not in ['timestamp', 'string'] -%}
-             {% do exceptions.raise_compiler_error("For partitioned tables with file_format = 'openhouse', 'data_type' must be one of ('timestamp', 'string').") %}
+           {%- if partition_by.data_type.lower() not in ['timestamp', 'string', 'int'] -%}
+             {% do exceptions.raise_compiler_error("For partitioned tables with file_format = 'openhouse', 'data_type' must be one of ('timestamp', 'string', 'int').") %}
            {%- endif -%}
            {%- if partition_by.data_type.lower() == 'timestamp' -%}
              {% set timestamp_columns.count = timestamp_columns.count + 1 %}
              {%- if timestamp_columns.count > 1 -%}
                {% do exceptions.raise_compiler_error("For timestamp-partitioned tables with file_format = 'openhouse',
                   OpenHouse only supports 1 timestamp-based column partitioning") %}
              {%- endif -%}
@@ -113,15 +113,15 @@
       {% endif %}
     {% endif %}
 
     {%- set grant_config = config.get('grants', none) -%}
     {%- if grant_config is not none %}
         {%- for privilege in grant_config.keys() %}
           {% if privilege.lower() not in ['select', 'manage grants'] %}
-            {% do exceptions.raise_compiler_error("For outputs with file_format = 'openhouse', keys in 'grants' map must be one of ('select', 'manage_grants').") %}
+            {% do exceptions.raise_compiler_error("For outputs with file_format = 'openhouse', keys in 'grants' map must be one of ('select', 'manage grants').") %}
           {% endif %}
         {%- endfor -%}
     {% endif %}
 
     {% if config.get('retention_period', none) is not none %}
       {% if config.get('partition_by', none) is none %}
         {% do exceptions.raise_compiler_error("For tables with file_format = 'openhouse' and 'retention_period', 'partition_by' must be supplied.") %}
```

### Comparing `in-dbt-spark-1.5.3/dbt/include/spark/macros/utils/dateadd.sql` & `in-dbt-spark-1.5.4/dbt/include/spark/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.3/dbt/include/spark/macros/utils/datediff.sql` & `in-dbt-spark-1.5.4/dbt/include/spark/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.3/dbt/include/spark/macros/utils/listagg.sql` & `in-dbt-spark-1.5.4/dbt/include/spark/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.3/dbt/include/spark/macros/utils/split_part.sql` & `in-dbt-spark-1.5.4/dbt/include/spark/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.3/dbt/include/spark/profile_template.yml` & `in-dbt-spark-1.5.4/dbt/include/spark/profile_template.yml`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.3/in_dbt_spark.egg-info/PKG-INFO` & `in-dbt-spark-1.5.4/in_dbt_spark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: in-dbt-spark
-Version: 1.5.3
+Version: 1.5.4
 Summary: Release for LinkedIn's changes to dbt-spark.
 Home-page: https://github.com/linkedin/in-dbt-spark
 Author: LinkedIn DBT Team
 Author-email: dbt-dev@linkedin.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.5.3 Summary: Release for
+Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.5.4 Summary: Release for
 LinkedIn's changes to dbt-spark. Home-page: https://github.com/linkedin/in-dbt-
 spark Author: LinkedIn DBT Team Author-email: dbt-dev@linkedin.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.10 Requires-
 Python: >=3.10 Description-Content-Type: text/markdown Provides-Extra: ODBC
```

### Comparing `in-dbt-spark-1.5.3/in_dbt_spark.egg-info/SOURCES.txt` & `in-dbt-spark-1.5.4/in_dbt_spark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.5.3/setup.py` & `in-dbt-spark-1.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     parts = _get_plugin_version_dict()
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "in-dbt-spark"
-package_version = "1.5.3"
+package_version = "1.5.4"
 dbt_core_version = _get_dbt_core_version()
 description = """Release for LinkedIn's changes to dbt-spark."""
 
 odbc_extras = ["pyodbc>=4.0.30"]
 pyhive_extras = [
     "PyHive[hive]>=0.6.0,<0.7.0",
     "thrift>=0.11.0,<0.17.0",
```

