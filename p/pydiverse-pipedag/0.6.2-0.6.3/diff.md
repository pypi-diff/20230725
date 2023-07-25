# Comparing `tmp/pydiverse_pipedag-0.6.2.tar.gz` & `tmp/pydiverse_pipedag-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiverse_pipedag-0.6.2.tar", max compression
+gzip compressed data, was "pydiverse_pipedag-0.6.3.tar", max compression
```

## Comparing `pydiverse_pipedag-0.6.2.tar` & `pydiverse_pipedag-0.6.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0     1517 2023-07-23 10:05:29.268867 pydiverse_pipedag-0.6.2/LICENSE
--rw-r--r--   0        0        0     6174 2023-07-23 10:05:29.268867 pydiverse_pipedag-0.6.2/docs/package/README.md
--rw-r--r--   0        0        0     3421 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/pyproject.toml
--rw-r--r--   0        0        0       13 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/.gitignore
--rw-r--r--   0        0        0      435 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/__init__.py
--rw-r--r--   0        0        0      857 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/_typing.py
--rw-r--r--   0        0        0       97 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/__init__.py
--rw-r--r--   0        0        0     5348 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/blob.py
--rw-r--r--   0        0        0      393 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/lock/__init__.py
--rw-r--r--   0        0        0     6097 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/lock/base.py
--rw-r--r--   0        0        0    13555 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/lock/database.py
--rw-r--r--   0        0        0     2756 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/lock/filelock.py
--rw-r--r--   0        0        0      769 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/lock/nolock.py
--rw-r--r--   0        0        0     3983 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/lock/zookeeper.py
--rw-r--r--   0        0        0      233 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/table/__init__.py
--rw-r--r--   0        0        0    23394 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/table/base.py
--rw-r--r--   0        0        0      108 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/table/cache/__init__.py
--rw-r--r--   0        0        0     3106 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/table/cache/base.py
--rw-r--r--   0        0        0     6976 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/table/cache/parquet.py
--rw-r--r--   0        0        0     6933 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/table/dict.py
--rw-r--r--   0        0        0      141 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/table/sql/__init__.py
--rw-r--r--   0        0        0    36934 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/table/sql/ddl.py
--rw-r--r--   0        0        0      187 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/table/sql/dialects/__init__.py
--rw-r--r--   0        0        0     1508 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/table/sql/dialects/duckdb.py
--rw-r--r--   0        0        0     3301 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/table/sql/dialects/ibm_db2.py
--rw-r--r--   0        0        0     9235 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/table/sql/dialects/mssql.py
--rw-r--r--   0        0        0     3956 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/table/sql/dialects/postgres.py
--rw-r--r--   0        0        0    21490 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/table/sql/hooks.py
--rw-r--r--   0        0        0     4250 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/table/sql/reflection.py
--rw-r--r--   0        0        0    47189 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/table/sql/sql.py
--rw-r--r--   0        0        0       81 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/table/util/__init__.py
--rw-r--r--   0        0        0     8579 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/table/util/dtype.py
--rw-r--r--   0        0        0      433 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/context/__init__.py
--rw-r--r--   0        0        0     9874 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/context/context.py
--rw-r--r--   0        0        0    26325 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/context/run_context.py
--rw-r--r--   0        0        0      311 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/core/__init__.py
--rw-r--r--   0        0        0    14956 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/core/config.py
--rw-r--r--   0        0        0    20430 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/core/flow.py
--rw-r--r--   0        0        0     4294 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/core/result.py
--rw-r--r--   0        0        0     7789 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/core/stage.py
--rw-r--r--   0        0        0     8013 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/core/task.py
--rw-r--r--   0        0        0      368 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/engine/__init__.py
--rw-r--r--   0        0        0      654 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/engine/base.py
--rw-r--r--   0        0        0     3133 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/engine/dask.py
--rw-r--r--   0        0        0     7269 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/engine/prefect.py
--rw-r--r--   0        0        0     1388 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/engine/sequential.py
--rw-r--r--   0        0        0     1079 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/errors/__init__.py
--rw-r--r--   0        0        0        0 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/management/__init__.py
--rw-r--r--   0        0        0      620 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/management/cli.py
--rw-r--r--   0        0        0        0 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/management/commands/__init__.py
--rw-r--r--   0        0        0     1741 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/management/commands/clear_metadata.py
--rw-r--r--   0        0        0     2744 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/management/commands/delete_schemas.py
--rw-r--r--   0        0        0      182 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/materialize/__init__.py
--rw-r--r--   0        0        0     9114 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/materialize/cache.py
--rw-r--r--   0        0        0    11091 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/materialize/container.py
--rw-r--r--   0        0        0    17639 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/materialize/core.py
--rw-r--r--   0        0        0     2074 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/materialize/metadata.py
--rw-r--r--   0        0        0    19431 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/materialize/store.py
--rw-r--r--   0        0        0      213 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/util/__init__.py
--rw-r--r--   0        0        0     2061 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/util/deep_map.py
--rw-r--r--   0        0        0     1435 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/util/deep_merge.py
--rw-r--r--   0        0        0      944 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/util/disposable.py
--rw-r--r--   0        0        0     1129 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/util/hashing.py
--rw-r--r--   0        0        0     3736 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/util/import_.py
--rw-r--r--   0        0        0     7992 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/util/ipc.py
--rw-r--r--   0        0        0     4400 2023-07-23 10:05:29.272867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/util/json.py
--rw-r--r--   0        0        0     1377 2023-07-23 10:05:29.276867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/util/naming.py
--rw-r--r--   0        0        0     2847 2023-07-23 10:05:29.276867 pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/util/structlog.py
--rw-r--r--   0        0        0     7911 1970-01-01 00:00:00.000000 pydiverse_pipedag-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1517 2023-07-25 13:13:25.440146 pydiverse_pipedag-0.6.3/LICENSE
+-rw-r--r--   0        0        0     6174 2023-07-25 13:13:25.440146 pydiverse_pipedag-0.6.3/docs/package/README.md
+-rw-r--r--   0        0        0     3421 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0       13 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/.gitignore
+-rw-r--r--   0        0        0      435 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/__init__.py
+-rw-r--r--   0        0        0      857 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/_typing.py
+-rw-r--r--   0        0        0       97 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/__init__.py
+-rw-r--r--   0        0        0     5348 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/blob.py
+-rw-r--r--   0        0        0      393 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/lock/__init__.py
+-rw-r--r--   0        0        0     6097 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/lock/base.py
+-rw-r--r--   0        0        0    13599 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/lock/database.py
+-rw-r--r--   0        0        0     2756 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/lock/filelock.py
+-rw-r--r--   0        0        0      769 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/lock/nolock.py
+-rw-r--r--   0        0        0     3983 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/lock/zookeeper.py
+-rw-r--r--   0        0        0      233 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/__init__.py
+-rw-r--r--   0        0        0    23394 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/base.py
+-rw-r--r--   0        0        0      108 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/cache/__init__.py
+-rw-r--r--   0        0        0     3106 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/cache/base.py
+-rw-r--r--   0        0        0     6976 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/cache/parquet.py
+-rw-r--r--   0        0        0     6933 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/dict.py
+-rw-r--r--   0        0        0      141 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/__init__.py
+-rw-r--r--   0        0        0    36934 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/ddl.py
+-rw-r--r--   0        0        0      187 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/dialects/__init__.py
+-rw-r--r--   0        0        0     1508 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/dialects/duckdb.py
+-rw-r--r--   0        0        0     3301 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/dialects/ibm_db2.py
+-rw-r--r--   0        0        0     9235 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/dialects/mssql.py
+-rw-r--r--   0        0        0     3956 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/dialects/postgres.py
+-rw-r--r--   0        0        0    21490 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/hooks.py
+-rw-r--r--   0        0        0     4250 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/reflection.py
+-rw-r--r--   0        0        0    47189 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/sql.py
+-rw-r--r--   0        0        0       81 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/util/__init__.py
+-rw-r--r--   0        0        0     8579 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/util/dtype.py
+-rw-r--r--   0        0        0      433 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/context/__init__.py
+-rw-r--r--   0        0        0     9874 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/context/context.py
+-rw-r--r--   0        0        0    26325 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/context/run_context.py
+-rw-r--r--   0        0        0      311 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/core/__init__.py
+-rw-r--r--   0        0        0    14956 2023-07-25 13:13:25.444146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/core/config.py
+-rw-r--r--   0        0        0    20430 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/core/flow.py
+-rw-r--r--   0        0        0     4294 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/core/result.py
+-rw-r--r--   0        0        0     7789 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/core/stage.py
+-rw-r--r--   0        0        0     8013 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/core/task.py
+-rw-r--r--   0        0        0      368 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/engine/__init__.py
+-rw-r--r--   0        0        0      654 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/engine/base.py
+-rw-r--r--   0        0        0     3133 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/engine/dask.py
+-rw-r--r--   0        0        0     7269 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/engine/prefect.py
+-rw-r--r--   0        0        0     1388 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/engine/sequential.py
+-rw-r--r--   0        0        0     1079 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/errors/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/management/__init__.py
+-rw-r--r--   0        0        0      620 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/management/cli.py
+-rw-r--r--   0        0        0        0 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/management/commands/__init__.py
+-rw-r--r--   0        0        0     1741 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/management/commands/clear_metadata.py
+-rw-r--r--   0        0        0     2744 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/management/commands/delete_schemas.py
+-rw-r--r--   0        0        0      182 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/materialize/__init__.py
+-rw-r--r--   0        0        0     9114 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/materialize/cache.py
+-rw-r--r--   0        0        0    11169 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/materialize/container.py
+-rw-r--r--   0        0        0    17639 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/materialize/core.py
+-rw-r--r--   0        0        0     2074 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/materialize/metadata.py
+-rw-r--r--   0        0        0    19431 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/materialize/store.py
+-rw-r--r--   0        0        0      213 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/__init__.py
+-rw-r--r--   0        0        0     2061 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/deep_map.py
+-rw-r--r--   0        0        0     1435 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/deep_merge.py
+-rw-r--r--   0        0        0      944 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/disposable.py
+-rw-r--r--   0        0        0     1129 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/hashing.py
+-rw-r--r--   0        0        0     3736 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/import_.py
+-rw-r--r--   0        0        0     7992 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/ipc.py
+-rw-r--r--   0        0        0     4400 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/json.py
+-rw-r--r--   0        0        0     1377 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/naming.py
+-rw-r--r--   0        0        0     2847 2023-07-25 13:13:25.448146 pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/structlog.py
+-rw-r--r--   0        0        0     7911 1970-01-01 00:00:00.000000 pydiverse_pipedag-0.6.3/PKG-INFO
```

### Comparing `pydiverse_pipedag-0.6.2/LICENSE` & `pydiverse_pipedag-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/docs/package/README.md` & `pydiverse_pipedag-0.6.3/docs/package/README.md`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/pyproject.toml` & `pydiverse_pipedag-0.6.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydiverse-pipedag"
-version = "0.6.2"
+version = "0.6.3"
 description = "A pipeline orchestration library executing tasks within one python session. It takes care of SQL table (de)materialization, caching and cache invalidation. Blob storage is supported as well for example for storing model files."
 authors = [
   "QuantCo, Inc.",
   "Nicolas Camenisch <garnele007@gmail.com>",
   "Martin Trautmann <windiana@users.sf.net>",
 ]
 license = "BSD-3-Clause"
```

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/_typing.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/_typing.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/blob.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/blob.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/lock/base.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/lock/base.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/lock/database.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/lock/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,15 +271,16 @@
             self.connection = self.engine.connect()
 
         name = self.lock_name(lockable)
         return PostgresLock(name, self.connection)
 
     def dispose(self):
         self.release_all()
-        self.connection.close()
+        if self.connection is not None:
+            self.connection.close()
         super().dispose()
 
 
 class MSSqlLock(Lock):
     """
     Locking based on application resource locks.
     https://learn.microsoft.com/en-us/sql/relational-databases/system-stored-procedures/sp-getapplock-transact-sql?view=sql-server-ver15
```

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/lock/filelock.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/lock/filelock.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/lock/nolock.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/lock/nolock.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/lock/zookeeper.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/lock/zookeeper.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/table/base.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/base.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/table/cache/base.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/cache/base.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/table/cache/parquet.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/cache/parquet.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/table/dict.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/dict.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/table/sql/ddl.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/ddl.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/table/sql/dialects/duckdb.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/dialects/duckdb.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/table/sql/dialects/ibm_db2.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/dialects/ibm_db2.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/table/sql/dialects/mssql.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/dialects/mssql.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/table/sql/dialects/postgres.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/dialects/postgres.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/table/sql/hooks.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/hooks.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/table/sql/reflection.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/reflection.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/table/sql/sql.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/sql/sql.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/backend/table/util/dtype.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/backend/table/util/dtype.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/context/context.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/context/context.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/context/run_context.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/context/run_context.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/core/config.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/core/config.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/core/flow.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/core/flow.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/core/result.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/core/result.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/core/stage.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/core/stage.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/core/task.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/core/task.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/engine/base.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/engine/base.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/engine/dask.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/engine/dask.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/engine/prefect.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/engine/prefect.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/engine/sequential.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/engine/sequential.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/errors/__init__.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/management/cli.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/management/cli.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/management/commands/clear_metadata.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/management/commands/clear_metadata.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/management/commands/delete_schemas.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/management/commands/delete_schemas.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/materialize/cache.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/materialize/cache.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/materialize/container.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/materialize/container.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,17 +22,18 @@
 
         @materialize()
         def task():
             df = pd.DataFrame({"x": [0, 1, 2, 3]}
             return Table(df, "name")
 
     :param obj: The table object to wrap
-    :param name: Optional name. If no name is provided, an automatically
-        generated name will be used. To prevent name collisions, you can
-        append ``"%%"`` at the end of the name to enable automatic name mangling.
+    :param name: Optional, case-insensitive name. If no name is provided,
+        an automatically generated name will be used. To prevent name collisions,
+        you can append ``"%%"`` at the end of the name to enable automatic
+        name mangling.
     :param primary_key: Optional name of the primary key that should be
         used when materializing this table. Only supported by some table stores.
     :param indexes: Optional list of indexes to create. Each provided index should be
         a list of column names. Only supported by some table stores.
     :param type_map: Optional map of column names to types. Depending on the table
         store this will allow you to control the datatype as which the specified
         columns get materialized.
@@ -121,17 +122,18 @@
         the corresponding task is running in. Otherwise, schema swapping won't work.
         To do this, pass the current stage as an argument to your task and then
         access the current stage name using :py:class:`Stage.current_name`.
 
     :param sql: The sql query string to execute. Depending on the database dialect,
         the query will be split into multiple subqueries that then get
         executed sequentially.
-    :param name: Optional name. If no name is provided, an automatically
-        generated name will be used. To prevent name collisions, you can
-        append ``"%%"`` at the end of the name to enable automatic name mangling.
+    :param name: Optional, case-insensitive name. If no name is provided,
+        an automatically generated name will be used. To prevent name collisions,
+        you can append ``"%%"`` at the end of the name to enable automatic
+        name mangling.
 
     Example
     -------
     When you want to use tables produced by a RawSql task in a downstream task,
     you can either use square brackets during flow definition to pass
     a specific table to a child task, or you can pass the entire RawSql object
     as an input, in which case all tables get loaded and the child task can
@@ -274,17 +276,18 @@
 
         @materialize()
         def task():
             obj = SomePicklableClass()
             return Blob(obj, "name")
 
     :param obj: The object to wrap
-    :param name: Optional name. If no name is provided, an automatically
-        generated name will be used. To prevent name collisions, you can
-        append ``"%%"`` at the end of the name to enable automatic name mangling.
+    :param name: Optional, case-insensitive name. If no name is provided,
+        an automatically generated name will be used. To prevent name collisions,
+        you can append ``"%%"`` at the end of the name to enable automatic
+        name mangling.
 
     .. seealso:: You can specify which types of objects should automatically get
         converted to blobs using the :ref:`auto_blob` config option.
     """
 
     def __init__(
         self,
```

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/materialize/core.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/materialize/core.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/materialize/metadata.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/materialize/metadata.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/materialize/store.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/materialize/store.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/util/deep_map.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/deep_map.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/util/deep_merge.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/deep_merge.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/util/disposable.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/disposable.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/util/hashing.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/hashing.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/util/import_.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/import_.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/util/ipc.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/ipc.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/util/json.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/json.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/util/naming.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/naming.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/src/pydiverse/pipedag/util/structlog.py` & `pydiverse_pipedag-0.6.3/src/pydiverse/pipedag/util/structlog.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.6.2/PKG-INFO` & `pydiverse_pipedag-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydiverse-pipedag
-Version: 0.6.2
+Version: 0.6.3
 Summary: A pipeline orchestration library executing tasks within one python session. It takes care of SQL table (de)materialization, caching and cache invalidation. Blob storage is supported as well for example for storing model files.
 License: BSD-3-Clause
 Author: QuantCo, Inc.
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

