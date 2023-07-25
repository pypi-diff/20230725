# Comparing `tmp/dbt-databricks-1.6.0rc1.tar.gz` & `tmp/dbt-databricks-1.6.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-databricks-1.6.0rc1.tar", last modified: Wed Jul 19 19:07:04 2023, max compression
+gzip compressed data, was "dbt-databricks-1.6.0rc2.tar", last modified: Thu Jul 20 16:44:11 2023, max compression
```

## Comparing `dbt-databricks-1.6.0rc1.tar` & `dbt-databricks-1.6.0rc2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-19 19:07:04.985347 dbt-databricks-1.6.0rc1/
--rw-r--r--   0 raymond.cypher   (502) staff       (20)       46 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc1/MANIFEST.in
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     5429 2023-07-19 19:07:04.984983 dbt-databricks-1.6.0rc1/PKG-INFO
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     4624 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc1/README.md
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-19 19:07:04.933785 dbt-databricks-1.6.0rc1/dbt/
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-19 19:07:04.933194 dbt-databricks-1.6.0rc1/dbt/adapters/
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-19 19:07:04.955326 dbt-databricks-1.6.0rc1/dbt/adapters/databricks/
--rw-r--r--   0 raymond.cypher   (502) staff       (20)      626 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc1/dbt/adapters/databricks/__init__.py
--rw-r--r--   0 raymond.cypher   (502) staff       (20)       26 2023-07-19 18:53:50.000000 dbt-databricks-1.6.0rc1/dbt/adapters/databricks/__version__.py
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     2708 2023-05-10 18:27:27.000000 dbt-databricks-1.6.0rc1/dbt/adapters/databricks/auth.py
--rw-r--r--   0 raymond.cypher   (502) staff       (20)      586 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc1/dbt/adapters/databricks/column.py
--rw-r--r--   0 raymond.cypher   (502) staff       (20)    35882 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc1/dbt/adapters/databricks/connections.py
--rw-r--r--   0 raymond.cypher   (502) staff       (20)    21146 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc1/dbt/adapters/databricks/impl.py
--rw-r--r--   0 raymond.cypher   (502) staff       (20)    17743 2023-07-19 17:29:22.000000 dbt-databricks-1.6.0rc1/dbt/adapters/databricks/python_submissions.py
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     3564 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc1/dbt/adapters/databricks/relation.py
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     2117 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc1/dbt/adapters/databricks/utils.py
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-19 19:07:04.934213 dbt-databricks-1.6.0rc1/dbt/include/
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-19 19:07:04.956546 dbt-databricks-1.6.0rc1/dbt/include/databricks/
--rw-r--r--   0 raymond.cypher   (502) staff       (20)       52 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc1/dbt/include/databricks/__init__.py
--rw-r--r--   0 raymond.cypher   (502) staff       (20)       77 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc1/dbt/include/databricks/dbt_project.yml
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-19 19:07:04.958847 dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/
--rw-r--r--   0 raymond.cypher   (502) staff       (20)    18808 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/adapters.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)      592 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/catalog.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     2409 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/copy_into.sql
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-19 19:07:04.962715 dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/materializations/
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-19 19:07:04.966190 dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/materializations/incremental/
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     4331 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     3910 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     2066 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/materializations/incremental/validate.sql
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-19 19:07:04.969663 dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/materializations/materialized_view/
--rw-r--r--   0 raymond.cypher   (502) staff       (20)      318 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/materializations/materialized_view/create_materialized_view_as.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     1682 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/materializations/materialized_view/materialized_view.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)      279 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/materializations/materialized_view/refresh_materialized_view.sql
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-19 19:07:04.971304 dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/materializations/seeds/
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     2451 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/materializations/seeds/helpers.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     2476 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/materializations/seeds/seeds.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     5397 2023-05-08 06:46:27.000000 dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/materializations/snapshot.sql
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-19 19:07:04.973418 dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/materializations/streaming_table/
--rw-r--r--   0 raymond.cypher   (502) staff       (20)      636 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/materializations/streaming_table/create_or_refresh_streaming_table_as.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     1698 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/materializations/streaming_table/streaming_table.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     1616 2023-05-08 06:46:27.000000 dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/materializations/table.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     1316 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/materializations/view.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)      648 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/statement.sql
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-19 19:07:04.976005 dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/utils/
--rw-r--r--   0 raymond.cypher   (502) staff       (20)      318 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/utils/dateadd.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)      338 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/utils/datediff.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)      535 2023-05-10 18:27:27.000000 dbt-databricks-1.6.0rc1/dbt/include/databricks/profile_template.yml
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-19 19:07:04.983604 dbt-databricks-1.6.0rc1/dbt_databricks.egg-info/
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     5429 2023-07-19 19:07:04.000000 dbt-databricks-1.6.0rc1/dbt_databricks.egg-info/PKG-INFO
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     1959 2023-07-19 19:07:04.000000 dbt-databricks-1.6.0rc1/dbt_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 raymond.cypher   (502) staff       (20)        1 2023-07-19 19:07:04.000000 dbt-databricks-1.6.0rc1/dbt_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 raymond.cypher   (502) staff       (20)        1 2023-06-15 16:25:03.000000 dbt-databricks-1.6.0rc1/dbt_databricks.egg-info/not-zip-safe
--rw-r--r--   0 raymond.cypher   (502) staff       (20)       88 2023-07-19 19:07:04.000000 dbt-databricks-1.6.0rc1/dbt_databricks.egg-info/requires.txt
--rw-r--r--   0 raymond.cypher   (502) staff       (20)        4 2023-07-19 19:07:04.000000 dbt-databricks-1.6.0rc1/dbt_databricks.egg-info/top_level.txt
--rw-r--r--   0 raymond.cypher   (502) staff       (20)       38 2023-07-19 19:07:04.985412 dbt-databricks-1.6.0rc1/setup.cfg
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     2548 2023-07-19 17:29:22.000000 dbt-databricks-1.6.0rc1/setup.py
+drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-20 16:44:11.781909 dbt-databricks-1.6.0rc2/
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)       46 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc2/MANIFEST.in
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     5379 2023-07-20 16:44:11.781711 dbt-databricks-1.6.0rc2/PKG-INFO
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     4624 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc2/README.md
+drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-20 16:44:11.764076 dbt-databricks-1.6.0rc2/dbt/
+drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-20 16:44:11.763801 dbt-databricks-1.6.0rc2/dbt/adapters/
+drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-20 16:44:11.770055 dbt-databricks-1.6.0rc2/dbt/adapters/databricks/
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)      626 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc2/dbt/adapters/databricks/__init__.py
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)       26 2023-07-19 23:16:23.000000 dbt-databricks-1.6.0rc2/dbt/adapters/databricks/__version__.py
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     2708 2023-05-10 18:27:27.000000 dbt-databricks-1.6.0rc2/dbt/adapters/databricks/auth.py
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)      586 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc2/dbt/adapters/databricks/column.py
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)    35924 2023-07-19 22:57:01.000000 dbt-databricks-1.6.0rc2/dbt/adapters/databricks/connections.py
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)    21146 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc2/dbt/adapters/databricks/impl.py
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)    17743 2023-07-19 17:29:22.000000 dbt-databricks-1.6.0rc2/dbt/adapters/databricks/python_submissions.py
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     3564 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc2/dbt/adapters/databricks/relation.py
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     2117 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc2/dbt/adapters/databricks/utils.py
+drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-20 16:44:11.764236 dbt-databricks-1.6.0rc2/dbt/include/
+drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-20 16:44:11.771047 dbt-databricks-1.6.0rc2/dbt/include/databricks/
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)       52 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/__init__.py
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)       77 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/dbt_project.yml
+drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-20 16:44:11.772360 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)    18808 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/adapters.sql
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)      592 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/catalog.sql
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     2409 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/copy_into.sql
+drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-20 16:44:11.773309 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/
+drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-20 16:44:11.774470 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/incremental/
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     4331 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     3910 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     2066 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/incremental/validate.sql
+drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-20 16:44:11.775701 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/materialized_view/
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)      318 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/materialized_view/create_materialized_view_as.sql
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     1682 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/materialized_view/materialized_view.sql
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)      279 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/materialized_view/refresh_materialized_view.sql
+drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-20 16:44:11.776360 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/seeds/
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     2451 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     2476 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/seeds/seeds.sql
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     5397 2023-05-08 06:46:27.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/snapshot.sql
+drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-20 16:44:11.777288 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/streaming_table/
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)      636 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/streaming_table/create_or_refresh_streaming_table_as.sql
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     1698 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/streaming_table/streaming_table.sql
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     1616 2023-05-08 06:46:27.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/table.sql
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     1316 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/view.sql
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)      648 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/statement.sql
+drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-20 16:44:11.778720 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/utils/
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)      318 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/utils/dateadd.sql
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)      338 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/utils/datediff.sql
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)      535 2023-05-10 18:27:27.000000 dbt-databricks-1.6.0rc2/dbt/include/databricks/profile_template.yml
+drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-20 16:44:11.781374 dbt-databricks-1.6.0rc2/dbt_databricks.egg-info/
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     5379 2023-07-20 16:44:11.000000 dbt-databricks-1.6.0rc2/dbt_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     1959 2023-07-20 16:44:11.000000 dbt-databricks-1.6.0rc2/dbt_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)        1 2023-07-20 16:44:11.000000 dbt-databricks-1.6.0rc2/dbt_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)        1 2023-06-15 16:25:03.000000 dbt-databricks-1.6.0rc2/dbt_databricks.egg-info/not-zip-safe
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)       91 2023-07-20 16:44:11.000000 dbt-databricks-1.6.0rc2/dbt_databricks.egg-info/requires.txt
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)        4 2023-07-20 16:44:11.000000 dbt-databricks-1.6.0rc2/dbt_databricks.egg-info/top_level.txt
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)       38 2023-07-20 16:44:11.781963 dbt-databricks-1.6.0rc2/setup.cfg
+-rw-r--r--   0 raymond.cypher   (502) staff       (20)     2502 2023-07-19 22:21:58.000000 dbt-databricks-1.6.0rc2/setup.py
```

### Comparing `dbt-databricks-1.6.0rc1/PKG-INFO` & `dbt-databricks-1.6.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: dbt-databricks
-Version: 1.6.0rc1
+Version: 1.6.0rc2
 Summary: The Databricks adapter plugin for dbt
 Home-page: https://github.com/databricks/dbt-databricks
 Author: Databricks
 Author-email: feedback@databricks.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://bynder-public-us-west-2.s3.amazonaws.com/styleguide/ABB317701CA31CB7F29268E32B303CAE-pdf-column-1.png" alt="databricks logo" width="50%" />
   <img src="https://raw.githubusercontent.com/dbt-labs/dbt/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="250"/>
 </p>
 <p align="center">
```

### Comparing `dbt-databricks-1.6.0rc1/README.md` & `dbt-databricks-1.6.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc1/dbt/adapters/databricks/__init__.py` & `dbt-databricks-1.6.0rc2/dbt/adapters/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc1/dbt/adapters/databricks/auth.py` & `dbt-databricks-1.6.0rc2/dbt/adapters/databricks/auth.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc1/dbt/adapters/databricks/column.py` & `dbt-databricks-1.6.0rc2/dbt/adapters/databricks/column.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc1/dbt/adapters/databricks/connections.py` & `dbt-databricks-1.6.0rc2/dbt/adapters/databricks/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -775,22 +775,22 @@
                     cursor = None
                 raise
             finally:
                 if close_cursor and cursor is not None:
                     cursor.close()
 
     def execute(
-        self, sql: str, auto_begin: bool = False, fetch: bool = False
+        self, sql: str, auto_begin: bool = False, fetch: bool = False, limit: Optional[int] = None
     ) -> Tuple[DatabricksAdapterResponse, Table]:
         sql = self._add_query_comment(sql)
         _, cursor = self.add_query(sql, auto_begin)
         try:
             response = self.get_response(cursor)
             if fetch:
-                table = self.get_result_from_cursor(cursor)
+                table = self.get_result_from_cursor(cursor, limit)
             else:
                 table = agate_helper.empty_table()
             return response, table
         finally:
             cursor.close()
 
     def _execute_cursor(
@@ -813,15 +813,15 @@
                 fire_event(
                     SQLQueryStatus(
                         status=str(self.get_response(cursor)),
                         elapsed=round((time.time() - pre), 2),
                     )
                 )
 
-                return self.get_result_from_cursor(cursor)
+                return self.get_result_from_cursor(cursor, None)
             finally:
                 if cursor is not None:
                     cursor.close()
 
     def list_schemas(self, database: str, schema: Optional[str] = None) -> Table:
         return self._execute_cursor(
             f"GetSchemas(database={database}, schema={schema})",
```

### Comparing `dbt-databricks-1.6.0rc1/dbt/adapters/databricks/impl.py` & `dbt-databricks-1.6.0rc2/dbt/adapters/databricks/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc1/dbt/adapters/databricks/python_submissions.py` & `dbt-databricks-1.6.0rc2/dbt/adapters/databricks/python_submissions.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc1/dbt/adapters/databricks/relation.py` & `dbt-databricks-1.6.0rc2/dbt/adapters/databricks/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc1/dbt/adapters/databricks/utils.py` & `dbt-databricks-1.6.0rc2/dbt/adapters/databricks/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/adapters.sql` & `dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/catalog.sql` & `dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/copy_into.sql` & `dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/copy_into.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/materializations/incremental/incremental.sql` & `dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/materializations/incremental/strategies.sql` & `dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/materializations/incremental/validate.sql` & `dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/incremental/validate.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/materializations/materialized_view/materialized_view.sql` & `dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/materialized_view/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/materializations/seeds/helpers.sql` & `dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/materializations/seeds/seeds.sql` & `dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/seeds/seeds.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/materializations/snapshot.sql` & `dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/materializations/streaming_table/create_or_refresh_streaming_table_as.sql` & `dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/streaming_table/create_or_refresh_streaming_table_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/materializations/streaming_table/streaming_table.sql` & `dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/streaming_table/streaming_table.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/materializations/table.sql` & `dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/materializations/view.sql` & `dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc1/dbt/include/databricks/macros/statement.sql` & `dbt-databricks-1.6.0rc2/dbt/include/databricks/macros/statement.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc1/dbt/include/databricks/profile_template.yml` & `dbt-databricks-1.6.0rc2/dbt/include/databricks/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc1/dbt_databricks.egg-info/PKG-INFO` & `dbt-databricks-1.6.0rc2/dbt_databricks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: dbt-databricks
-Version: 1.6.0rc1
+Version: 1.6.0rc2
 Summary: The Databricks adapter plugin for dbt
 Home-page: https://github.com/databricks/dbt-databricks
 Author: Databricks
 Author-email: feedback@databricks.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://bynder-public-us-west-2.s3.amazonaws.com/styleguide/ABB317701CA31CB7F29268E32B303CAE-pdf-column-1.png" alt="databricks logo" width="50%" />
   <img src="https://raw.githubusercontent.com/dbt-labs/dbt/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="250"/>
 </p>
 <p align="center">
```

### Comparing `dbt-databricks-1.6.0rc1/dbt_databricks.egg-info/SOURCES.txt` & `dbt-databricks-1.6.0rc2/dbt_databricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc1/setup.py` & `dbt-databricks-1.6.0rc2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 import os
 import sys
 
-# require python 3.7 or newer
-if sys.version_info < (3, 7):
+# require python 3.8 or newer
+if sys.version_info < (3, 8):
     print("Error: dbt does not support this version of Python.")
-    print("Please upgrade to Python 3.7 or higher.")
+    print("Please upgrade to Python 3.8 or higher.")
     sys.exit(1)
 
 
 # require version of setuptools that supports find_namespace_packages
 from setuptools import setup
 
 try:
@@ -50,27 +50,26 @@
     long_description_content_type="text/markdown",
     author="Databricks",
     author_email="feedback@databricks.com",
     url="https://github.com/databricks/dbt-databricks",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
-        "dbt-spark~=1.5.0",
+        "dbt-spark==1.6.0rc1",
         "databricks-sql-connector~=2.7.0",
         "databricks-sdk>=0.1.7",
         "keyring>=23.13.0",
     ],
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX :: Linux",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
 )
```

