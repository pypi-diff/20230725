# Comparing `tmp/vdk-heartbeat-0.6.874744040.tar.gz` & `tmp/vdk-heartbeat-0.6.944393829.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vdk-heartbeat-0.6.874744040.tar", last modified: Mon May 22 13:54:25 2023, max compression
+gzip compressed data, was "dist/vdk-heartbeat-0.6.944393829.tar", last modified: Tue Jul 25 09:01:00 2023, max compression
```

## Comparing `vdk-heartbeat-0.6.874744040.tar` & `vdk-heartbeat-0.6.944393829.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:54:25.000000 vdk-heartbeat-0.6.874744040/
--rw-rw-rw-   0 root         (0) root         (0)      335 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6339 2023-05-22 13:54:25.000000 vdk-heartbeat-0.6.874744040/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5304 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1481 2023-05-22 13:54:25.000000 vdk-heartbeat-0.6.874744040/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:54:25.000000 vdk-heartbeat-0.6.874744040/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:54:25.000000 vdk-heartbeat-0.6.874744040/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:54:25.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:54:25.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/
--rw-rw-rw-   0 root         (0) root         (0)    10284 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/config.py
--rw-rw-rw-   0 root         (0) root         (0)    10133 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/database_run_test.py
--rw-rw-rw-   0 root         (0) root         (0)      956 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/empty_run_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2090 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/hearbeat.py
--rw-rw-rw-   0 root         (0) root         (0)     1426 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/heartbeat_base_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2472 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/heartbeat_test.py
--rw-rw-rw-   0 root         (0) root         (0)    10027 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/impala_database_test.py
--rw-rw-rw-   0 root         (0) root         (0)    16057 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/job_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     1961 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/log_config.py
--rw-rw-rw-   0 root         (0) root         (0)     1479 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/main.py
--rw-rw-rw-   0 root         (0) root         (0)     1262 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/ping_frontend_test.py
--rw-rw-rw-   0 root         (0) root         (0)     1926 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/reporter.py
--rw-rw-rw-   0 root         (0) root         (0)     2622 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/simple_run_test.py
--rw-rw-rw-   0 root         (0) root         (0)     1736 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/successful_run_test.py
--rw-rw-rw-   0 root         (0) root         (0)      756 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/tracing.py
--rw-rw-rw-   0 root         (0) root         (0)     4443 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/trino_database_test.py
--rw-rw-rw-   0 root         (0) root         (0)      551 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:54:25.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:54:25.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/
--rw-rw-rw-   0 root         (0) root         (0)      726 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/05_set_properties.py
--rw-rw-rw-   0 root         (0) root         (0)      624 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/10_ingest_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1512 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/20_verify_data.py
--rw-rw-rw-   0 root         (0) root         (0)      192 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/config.ini
--rw-rw-rw-   0 root         (0) root         (0)       10 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:54:25.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/empty/
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/empty/10_do_nothing.py
--rw-rw-rw-   0 root         (0) root         (0)      192 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/empty/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:54:25.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/
--rw-rw-rw-   0 root         (0) root         (0)      424 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/05_set_properties.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/10_create_table_source.sql
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/15_create_table_destination.sql
--rw-rw-rw-   0 root         (0) root         (0)      143 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/16_create_table_load_destination.sql
--rw-rw-rw-   0 root         (0) root         (0)      887 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/20_move_data_using_load.py
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/30_move_data_using_sql.sql
--rw-rw-rw-   0 root         (0) root         (0)     1251 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/40_execute_template.py
--rw-rw-rw-   0 root         (0) root         (0)      521 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/README.md
--rw-rw-rw-   0 root         (0) root         (0)      217 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:54:25.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/simple/
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/simple/10_simple.py
--rw-rw-rw-   0 root         (0) root         (0)      192 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/simple/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:54:25.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/
--rw-rw-rw-   0 root         (0) root         (0)      574 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/05_set_properties.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/10_drop_table_destination.sql
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/15_create_table_destination.sql
--rw-rw-rw-   0 root         (0) root         (0)      969 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/20_move_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2838 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/25_execute_template.py
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/30_move_data_using_sql.sql
--rw-rw-rw-   0 root         (0) root         (0)      216 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/config.ini
--rw-rw-rw-   0 root         (0) root         (0)       10 2023-05-22 13:54:10.000000 vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 13:54:25.000000 vdk-heartbeat-0.6.874744040/src/vdk_heartbeat.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6339 2023-05-22 13:54:25.000000 vdk-heartbeat-0.6.874744040/src/vdk_heartbeat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3144 2023-05-22 13:54:25.000000 vdk-heartbeat-0.6.874744040/src/vdk_heartbeat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 13:54:25.000000 vdk-heartbeat-0.6.874744040/src/vdk_heartbeat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-05-22 13:54:25.000000 vdk-heartbeat-0.6.874744040/src/vdk_heartbeat.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 13:54:25.000000 vdk-heartbeat-0.6.874744040/src/vdk_heartbeat.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      144 2023-05-22 13:54:25.000000 vdk-heartbeat-0.6.874744040/src/vdk_heartbeat.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-22 13:54:25.000000 vdk-heartbeat-0.6.874744040/src/vdk_heartbeat.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-05-22 13:54:14.000000 vdk-heartbeat-0.6.874744040/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:00.000000 vdk-heartbeat-0.6.944393829/
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6362 2023-07-25 09:01:00.000000 vdk-heartbeat-0.6.944393829/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5327 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1481 2023-07-25 09:01:00.000000 vdk-heartbeat-0.6.944393829/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      460 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:00.000000 vdk-heartbeat-0.6.944393829/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:00.000000 vdk-heartbeat-0.6.944393829/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:00.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:00.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/
+-rw-rw-rw-   0 root         (0) root         (0)    10284 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    10133 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/database_run_test.py
+-rw-rw-rw-   0 root         (0) root         (0)      956 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/empty_run_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2090 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/hearbeat.py
+-rw-rw-rw-   0 root         (0) root         (0)     1426 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/heartbeat_base_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2472 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/heartbeat_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    10027 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/impala_database_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    16057 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/job_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     1961 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/log_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1479 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/ping_frontend_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1926 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/reporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2622 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/simple_run_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1736 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/successful_run_test.py
+-rw-rw-rw-   0 root         (0) root         (0)      756 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/tracing.py
+-rw-rw-rw-   0 root         (0) root         (0)     4443 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/trino_database_test.py
+-rw-rw-rw-   0 root         (0) root         (0)      551 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:00.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:00.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/
+-rw-rw-rw-   0 root         (0) root         (0)      726 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/05_set_properties.py
+-rw-rw-rw-   0 root         (0) root         (0)      624 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/10_ingest_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1512 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/20_verify_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      192 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/config.ini
+-rw-rw-rw-   0 root         (0) root         (0)       10 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:00.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/empty/
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/empty/10_do_nothing.py
+-rw-rw-rw-   0 root         (0) root         (0)      192 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/empty/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:00.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/
+-rw-rw-rw-   0 root         (0) root         (0)      424 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/05_set_properties.py
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/10_create_table_source.sql
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/15_create_table_destination.sql
+-rw-rw-rw-   0 root         (0) root         (0)      143 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/16_create_table_load_destination.sql
+-rw-rw-rw-   0 root         (0) root         (0)      887 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/20_move_data_using_load.py
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/30_move_data_using_sql.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1251 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/40_execute_template.py
+-rw-rw-rw-   0 root         (0) root         (0)      521 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      217 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:00.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/simple/
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/simple/10_simple.py
+-rw-rw-rw-   0 root         (0) root         (0)      192 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/simple/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:00.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/
+-rw-rw-rw-   0 root         (0) root         (0)      574 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/05_set_properties.py
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/10_drop_table_destination.sql
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/15_create_table_destination.sql
+-rw-rw-rw-   0 root         (0) root         (0)      969 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/20_move_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2838 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/25_execute_template.py
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/30_move_data_using_sql.sql
+-rw-rw-rw-   0 root         (0) root         (0)      216 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/config.ini
+-rw-rw-rw-   0 root         (0) root         (0)       10 2023-07-25 09:00:41.000000 vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:00.000000 vdk-heartbeat-0.6.944393829/src/vdk_heartbeat.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6362 2023-07-25 09:01:00.000000 vdk-heartbeat-0.6.944393829/src/vdk_heartbeat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3144 2023-07-25 09:01:00.000000 vdk-heartbeat-0.6.944393829/src/vdk_heartbeat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 09:01:00.000000 vdk-heartbeat-0.6.944393829/src/vdk_heartbeat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-25 09:01:00.000000 vdk-heartbeat-0.6.944393829/src/vdk_heartbeat.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 09:01:00.000000 vdk-heartbeat-0.6.944393829/src/vdk_heartbeat.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      144 2023-07-25 09:01:00.000000 vdk-heartbeat-0.6.944393829/src/vdk_heartbeat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-25 09:01:00.000000 vdk-heartbeat-0.6.944393829/src/vdk_heartbeat.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-25 09:00:46.000000 vdk-heartbeat-0.6.944393829/version.txt
```

### Comparing `vdk-heartbeat-0.6.874744040/PKG-INFO` & `vdk-heartbeat-0.6.944393829/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-heartbeat
-Version: 0.6.874744040
+Version: 0.6.944393829
 Summary: Versatile Data Kit Heartbeat and Health Test
 Home-page: https://github.com/vmware/versatile-data-kit/tree/main/projects/vdk-heartbeat
 Author: VMware Inc.
 Author-email: taurus@groups.vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/wiki/Introduction
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/tree/main/projects/vdk-heartbeat
 Platform: any
@@ -160,11 +160,11 @@
 ```
 
 The CONTROL_API_URL environment variable doubles as the frontend url, since both
 th control service and the frontend are deployed to the same host by the helm
 chart.
 
 ```
-CONTROL_API_URL=http://cicd-control-service-svc:8092
+CONTROL_API_URL=http://cicd-control-service-svc.cicd.svc.cluster.local:8092
 ```
 
 The test sends a `GET` request to the URL and expects a success response
```

### Comparing `vdk-heartbeat-0.6.874744040/README.md` & `vdk-heartbeat-0.6.944393829/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -136,11 +136,11 @@
 ```
 
 The CONTROL_API_URL environment variable doubles as the frontend url, since both
 th control service and the frontend are deployed to the same host by the helm
 chart.
 
 ```
-CONTROL_API_URL=http://cicd-control-service-svc:8092
+CONTROL_API_URL=http://cicd-control-service-svc.cicd.svc.cluster.local:8092
 ```
 
 The test sends a `GET` request to the URL and expects a success response
```

### Comparing `vdk-heartbeat-0.6.874744040/setup.cfg` & `vdk-heartbeat-0.6.944393829/setup.cfg`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/config.py` & `vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/config.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/database_run_test.py` & `vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/database_run_test.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/empty_run_test.py` & `vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/empty_run_test.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/hearbeat.py` & `vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/hearbeat.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/heartbeat_base_test.py` & `vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/heartbeat_base_test.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/heartbeat_test.py` & `vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/heartbeat_test.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/impala_database_test.py` & `vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/impala_database_test.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/job_controller.py` & `vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/job_controller.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/log_config.py` & `vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/log_config.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/main.py` & `vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/main.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/ping_frontend_test.py` & `vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/ping_frontend_test.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/reporter.py` & `vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/reporter.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/simple_run_test.py` & `vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/simple_run_test.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/successful_run_test.py` & `vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/successful_run_test.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/tracing.py` & `vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/tracing.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/trino_database_test.py` & `vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/trino_database_test.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/util.py` & `vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/util.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/05_set_properties.py` & `vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/05_set_properties.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/10_ingest_data.py` & `vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/10_ingest_data.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/20_verify_data.py` & `vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/database_ingestion/20_verify_data.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/20_move_data_using_load.py` & `vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/20_move_data_using_load.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/40_execute_template.py` & `vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/40_execute_template.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/README.md` & `vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/impala/README.md`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/05_set_properties.py` & `vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/05_set_properties.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/20_move_data.py` & `vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/20_move_data.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.874744040/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/25_execute_template.py` & `vdk-heartbeat-0.6.944393829/src/vdk/internal/heartbeat/vdk_heartbeat_data_job/trino/25_execute_template.py`

 * *Files identical despite different names*

### Comparing `vdk-heartbeat-0.6.874744040/src/vdk_heartbeat.egg-info/PKG-INFO` & `vdk-heartbeat-0.6.944393829/src/vdk_heartbeat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-heartbeat
-Version: 0.6.874744040
+Version: 0.6.944393829
 Summary: Versatile Data Kit Heartbeat and Health Test
 Home-page: https://github.com/vmware/versatile-data-kit/tree/main/projects/vdk-heartbeat
 Author: VMware Inc.
 Author-email: taurus@groups.vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/wiki/Introduction
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/tree/main/projects/vdk-heartbeat
 Platform: any
@@ -160,11 +160,11 @@
 ```
 
 The CONTROL_API_URL environment variable doubles as the frontend url, since both
 th control service and the frontend are deployed to the same host by the helm
 chart.
 
 ```
-CONTROL_API_URL=http://cicd-control-service-svc:8092
+CONTROL_API_URL=http://cicd-control-service-svc.cicd.svc.cluster.local:8092
 ```
 
 The test sends a `GET` request to the URL and expects a success response
```

### Comparing `vdk-heartbeat-0.6.874744040/src/vdk_heartbeat.egg-info/SOURCES.txt` & `vdk-heartbeat-0.6.944393829/src/vdk_heartbeat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

