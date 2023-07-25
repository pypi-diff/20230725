# Comparing `tmp/vdk-impala-0.4.929119368.tar.gz` & `tmp/vdk-impala-0.4.944393829.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-impala-0.4.929119368.tar", last modified: Wed Jul 12 15:45:14 2023, max compression
+gzip compressed data, was "vdk-impala-0.4.944393829.tar", last modified: Tue Jul 25 09:01:02 2023, max compression
```

## Comparing `vdk-impala-0.4.929119368.tar` & `vdk-impala-0.4.944393829.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:45:14.689975 vdk-impala-0.4.929119368/
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6530 2023-07-12 15:45:14.689975 vdk-impala-0.4.929119368/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5936 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 15:45:14.689975 vdk-impala-0.4.929119368/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1223 2023-07-12 15:45:03.000000 vdk-impala-0.4.929119368/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:45:14.681975 vdk-impala-0.4.929119368/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:45:14.677975 vdk-impala-0.4.929119368/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:45:14.677975 vdk-impala-0.4.929119368/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:45:14.681975 vdk-impala-0.4.929119368/src/vdk/plugin/impala/
--rw-rw-rw-   0 root         (0) root         (0)     6381 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/impala_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     2060 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/impala_connection.py
--rw-rw-rw-   0 root         (0) root         (0)     4518 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/impala_error_classifier.py
--rw-rw-rw-   0 root         (0) root         (0)    20197 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/impala_error_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     7846 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/impala_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     7448 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/impala_lineage_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     6722 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/impala_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:45:14.681975 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1029 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/data_quality_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:45:14.681975 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:45:14.681975 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/dimension/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/dimension/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:45:14.681975 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/dimension/scd1/
--rw-rw-rw-   0 root         (0) root         (0)      894 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/dimension/scd1/00-dimension-scd1-definition.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/dimension/scd1/01-test-if-view-matches-target.sql
--rw-rw-rw-   0 root         (0) root         (0)     2703 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/dimension/scd1/02-handle-quality-checks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:45:14.681975 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/dimension/scd1/02-requisite-sql-scripts/
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/dimension/scd1/02-requisite-sql-scripts/02-insert-into-target.sql
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/dimension/scd1/03-refresh.sql
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/dimension/scd1/04-compute-stats.sql
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/dimension/scd1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:45:14.685975 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/dimension/scd2/
--rw-rw-rw-   0 root         (0) root         (0)      847 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/dimension/scd2/00-dimension-scd2-definition.py
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/dimension/scd2/01-test-if-view-matches-target.sql
--rw-rw-rw-   0 root         (0) root         (0)     1718 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/dimension/scd2/02-insert-into-target.sql
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/dimension/scd2/03-refresh.sql
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/dimension/scd2/04-compute-stats.sql
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/dimension/scd2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:45:14.685975 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/fact/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/fact/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:45:14.685975 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/fact/insert/
--rw-rw-rw-   0 root         (0) root         (0)      804 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/fact/insert/00-fact-snapshot-definition.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/fact/insert/01-test-if-view-matches-target.sql
--rw-rw-rw-   0 root         (0) root         (0)     3373 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/fact/insert/02-handle-quality-checks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:45:14.685975 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/fact/insert/02-requisite-sql-scripts/
--rw-rw-rw-   0 root         (0) root         (0)      186 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/fact/insert/02-requisite-sql-scripts/02-create-consolidated-view.sql
--rw-rw-rw-   0 root         (0) root         (0)      309 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/fact/insert/02-requisite-sql-scripts/02-insert-into-target.sql
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/fact/insert/03-refresh.sql
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/fact/insert/04-compute-stats.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:45:14.685975 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/fact/snapshot/
--rw-rw-rw-   0 root         (0) root         (0)      829 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/fact/snapshot/00-fact-snapshot-definition.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/fact/snapshot/01-test-if-view-matches-target.sql
--rw-rw-rw-   0 root         (0) root         (0)     3190 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/fact/snapshot/02-handle-quality-checks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:45:14.685975 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/fact/snapshot/02-requisite-sql-scripts/
--rw-rw-rw-   0 root         (0) root         (0)      491 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/fact/snapshot/02-requisite-sql-scripts/02-insert-into-target.sql
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/fact/snapshot/02-requisite-sql-scripts/02-overwrite-target.sql
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/fact/snapshot/03-refresh.sql
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/fact/snapshot/04-compute-stats.sql
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/fact/snapshot/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:45:14.685975 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/versioned/
--rw-rw-rw-   0 root         (0) root         (0)     3032 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/versioned/00-versioned-definition.py
--rw-rw-rw-   0 root         (0) root         (0)      294 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/versioned/01-test-if-view-matches-target.sql
--rw-rw-rw-   0 root         (0) root         (0)     4358 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/versioned/02-insert-into-target.sql
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/versioned/03-refresh.sql
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/versioned/04-compute-stats.sql
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/versioned/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2669 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/template_arguments_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     2298 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:45:14.685975 vdk-impala-0.4.929119368/src/vdk_impala.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6530 2023-07-12 15:45:14.000000 vdk-impala-0.4.929119368/src/vdk_impala.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3918 2023-07-12 15:45:14.000000 vdk-impala-0.4.929119368/src/vdk_impala.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 15:45:14.000000 vdk-impala-0.4.929119368/src/vdk_impala.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-07-12 15:45:14.000000 vdk-impala-0.4.929119368/src/vdk_impala.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-07-12 15:45:14.000000 vdk-impala-0.4.929119368/src/vdk_impala.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-07-12 15:45:14.000000 vdk-impala-0.4.929119368/src/vdk_impala.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:45:14.685975 vdk-impala-0.4.929119368/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:45:14.681975 vdk-impala-0.4.929119368/tests/functional/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:45:14.681975 vdk-impala-0.4.929119368/tests/functional/jobs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:45:14.685975 vdk-impala-0.4.929119368/tests/functional/jobs/sql-job/
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/tests/functional/jobs/sql-job/10_create_table.sql
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/tests/functional/jobs/sql-job/20_populate_table.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:45:14.689975 vdk-impala-0.4.929119368/tests/functional/jobs/sql-job-non-lineage/
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/tests/functional/jobs/sql-job-non-lineage/10_create_table.sql
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/tests/functional/jobs/sql-job-non-lineage/20_compute_table.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:45:14.689975 vdk-impala-0.4.929119368/tests/functional/jobs/sql-job-syntax-error/
--rw-rw-rw-   0 root         (0) root         (0)       13 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/tests/functional/jobs/sql-job-syntax-error/10_bad_query.sql
--rw-rw-rw-   0 root         (0) root         (0)     3952 2023-07-12 15:44:59.000000 vdk-impala-0.4.929119368/tests/test_error_classifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.812218 vdk-impala-0.4.944393829/
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6530 2023-07-25 09:01:02.812218 vdk-impala-0.4.944393829/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5936 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 09:01:02.812218 vdk-impala-0.4.944393829/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1223 2023-07-25 09:00:50.000000 vdk-impala-0.4.944393829/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.800218 vdk-impala-0.4.944393829/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.800218 vdk-impala-0.4.944393829/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.800218 vdk-impala-0.4.944393829/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.804218 vdk-impala-0.4.944393829/src/vdk/plugin/impala/
+-rw-rw-rw-   0 root         (0) root         (0)     6381 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/impala_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     2060 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/impala_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     4518 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/impala_error_classifier.py
+-rw-rw-rw-   0 root         (0) root         (0)    20197 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/impala_error_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     7846 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/impala_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     7448 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/impala_lineage_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     6722 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/impala_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.804218 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1029 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/data_quality_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.804218 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.804218 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.804218 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd1/
+-rw-rw-rw-   0 root         (0) root         (0)      894 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd1/00-dimension-scd1-definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd1/01-test-if-view-matches-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2703 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd1/02-handle-quality-checks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.804218 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd1/02-requisite-sql-scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd1/02-requisite-sql-scripts/02-insert-into-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd1/03-refresh.sql
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd1/04-compute-stats.sql
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.804218 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd2/
+-rw-rw-rw-   0 root         (0) root         (0)      847 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd2/00-dimension-scd2-definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd2/01-test-if-view-matches-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1718 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd2/02-insert-into-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd2/03-refresh.sql
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd2/04-compute-stats.sql
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.808218 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.808218 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/insert/
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/insert/00-fact-snapshot-definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/insert/01-test-if-view-matches-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3373 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/insert/02-handle-quality-checks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.808218 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/insert/02-requisite-sql-scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/insert/02-requisite-sql-scripts/02-create-consolidated-view.sql
+-rw-rw-rw-   0 root         (0) root         (0)      309 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/insert/02-requisite-sql-scripts/02-insert-into-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/insert/03-refresh.sql
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/insert/04-compute-stats.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.808218 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/snapshot/
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/snapshot/00-fact-snapshot-definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/snapshot/01-test-if-view-matches-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3190 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/snapshot/02-handle-quality-checks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.808218 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/snapshot/02-requisite-sql-scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      491 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/snapshot/02-requisite-sql-scripts/02-insert-into-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/snapshot/02-requisite-sql-scripts/02-overwrite-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/snapshot/03-refresh.sql
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/snapshot/04-compute-stats.sql
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/snapshot/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.812218 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/versioned/
+-rw-rw-rw-   0 root         (0) root         (0)     3032 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/versioned/00-versioned-definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      294 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/versioned/01-test-if-view-matches-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)     4358 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/versioned/02-insert-into-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/versioned/03-refresh.sql
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/versioned/04-compute-stats.sql
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/versioned/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2669 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/template_arguments_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2298 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.812218 vdk-impala-0.4.944393829/src/vdk_impala.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6530 2023-07-25 09:01:02.000000 vdk-impala-0.4.944393829/src/vdk_impala.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3918 2023-07-25 09:01:02.000000 vdk-impala-0.4.944393829/src/vdk_impala.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 09:01:02.000000 vdk-impala-0.4.944393829/src/vdk_impala.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-25 09:01:02.000000 vdk-impala-0.4.944393829/src/vdk_impala.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-07-25 09:01:02.000000 vdk-impala-0.4.944393829/src/vdk_impala.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-25 09:01:02.000000 vdk-impala-0.4.944393829/src/vdk_impala.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.812218 vdk-impala-0.4.944393829/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.800218 vdk-impala-0.4.944393829/tests/functional/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.800218 vdk-impala-0.4.944393829/tests/functional/jobs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.812218 vdk-impala-0.4.944393829/tests/functional/jobs/sql-job/
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/tests/functional/jobs/sql-job/10_create_table.sql
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/tests/functional/jobs/sql-job/20_populate_table.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.812218 vdk-impala-0.4.944393829/tests/functional/jobs/sql-job-non-lineage/
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/tests/functional/jobs/sql-job-non-lineage/10_create_table.sql
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/tests/functional/jobs/sql-job-non-lineage/20_compute_table.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:02.812218 vdk-impala-0.4.944393829/tests/functional/jobs/sql-job-syntax-error/
+-rw-rw-rw-   0 root         (0) root         (0)       13 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/tests/functional/jobs/sql-job-syntax-error/10_bad_query.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3952 2023-07-25 09:00:46.000000 vdk-impala-0.4.944393829/tests/test_error_classifier.py
```

### Comparing `vdk-impala-0.4.929119368/PKG-INFO` & `vdk-impala-0.4.944393829/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-impala
-Version: 0.4.929119368
+Version: 0.4.944393829
 Summary: Versatile Data Kit SDK plugin provides support for Impala database.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-impala-0.4.929119368/README.md` & `vdk-impala-0.4.944393829/README.md`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.929119368/setup.py` & `vdk-impala-0.4.944393829/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.4.929119368"
+__version__ = "0.4.944393829"
 
 setuptools.setup(
     name="vdk-impala",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK plugin provides support for Impala database.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-impala-0.4.929119368/src/vdk/plugin/impala/impala_configuration.py` & `vdk-impala-0.4.944393829/src/vdk/plugin/impala/impala_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.929119368/src/vdk/plugin/impala/impala_connection.py` & `vdk-impala-0.4.944393829/src/vdk/plugin/impala/impala_connection.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.929119368/src/vdk/plugin/impala/impala_error_classifier.py` & `vdk-impala-0.4.944393829/src/vdk/plugin/impala/impala_error_classifier.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.929119368/src/vdk/plugin/impala/impala_error_handler.py` & `vdk-impala-0.4.944393829/src/vdk/plugin/impala/impala_error_handler.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.929119368/src/vdk/plugin/impala/impala_helper.py` & `vdk-impala-0.4.944393829/src/vdk/plugin/impala/impala_helper.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.929119368/src/vdk/plugin/impala/impala_lineage_plugin.py` & `vdk-impala-0.4.944393829/src/vdk/plugin/impala/impala_lineage_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.929119368/src/vdk/plugin/impala/impala_plugin.py` & `vdk-impala-0.4.944393829/src/vdk/plugin/impala/impala_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/data_quality_exception.py` & `vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/data_quality_exception.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/dimension/scd1/00-dimension-scd1-definition.py` & `vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd1/00-dimension-scd1-definition.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/dimension/scd1/02-handle-quality-checks.py` & `vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd1/02-handle-quality-checks.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/dimension/scd1/02-requisite-sql-scripts/02-insert-into-target.sql` & `vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd1/02-requisite-sql-scripts/02-insert-into-target.sql`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/dimension/scd2/00-dimension-scd2-definition.py` & `vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd2/00-dimension-scd2-definition.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/dimension/scd2/02-insert-into-target.sql` & `vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/dimension/scd2/02-insert-into-target.sql`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/fact/insert/00-fact-snapshot-definition.py` & `vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/insert/00-fact-snapshot-definition.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/fact/insert/02-handle-quality-checks.py` & `vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/insert/02-handle-quality-checks.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/fact/snapshot/00-fact-snapshot-definition.py` & `vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/snapshot/00-fact-snapshot-definition.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/fact/snapshot/02-handle-quality-checks.py` & `vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/fact/snapshot/02-handle-quality-checks.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/versioned/00-versioned-definition.py` & `vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/versioned/00-versioned-definition.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/load/versioned/02-insert-into-target.sql` & `vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/load/versioned/02-insert-into-target.sql`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/template_arguments_validator.py` & `vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/template_arguments_validator.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.929119368/src/vdk/plugin/impala/templates/utility.py` & `vdk-impala-0.4.944393829/src/vdk/plugin/impala/templates/utility.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.929119368/src/vdk_impala.egg-info/PKG-INFO` & `vdk-impala-0.4.944393829/src/vdk_impala.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-impala
-Version: 0.4.929119368
+Version: 0.4.944393829
 Summary: Versatile Data Kit SDK plugin provides support for Impala database.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-impala-0.4.929119368/src/vdk_impala.egg-info/SOURCES.txt` & `vdk-impala-0.4.944393829/src/vdk_impala.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.929119368/tests/test_error_classifier.py` & `vdk-impala-0.4.944393829/tests/test_error_classifier.py`

 * *Files identical despite different names*

