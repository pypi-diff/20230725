# Comparing `tmp/MindsDB-23.7.3.1.tar.gz` & `tmp/MindsDB-23.7.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MindsDB-23.7.3.1.tar", last modified: Tue Jul 18 15:57:35 2023, max compression
+gzip compressed data, was "dist/MindsDB-23.7.4.0.tar", last modified: Tue Jul 25 08:33:05 2023, max compression
```

## Comparing `MindsDB-23.7.3.1.tar` & `MindsDB-23.7.4.0.tar`

### file list

```diff
@@ -1,1433 +1,1434 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/MindsDB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25650 2023-07-18 15:57:34.000000 MindsDB-23.7.3.1/MindsDB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    68865 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/MindsDB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:57:34.000000 MindsDB-23.7.3.1/MindsDB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-07-18 15:57:34.000000 MindsDB-23.7.3.1/MindsDB.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 15:57:34.000000 MindsDB-23.7.3.1/MindsDB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    25650 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20461 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/api/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/common/check_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/api/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/gunicorn_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    13175 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/chatbots.py
--rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/configs/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/configs/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/configs/chatbots.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/configs/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/configs/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/configs/default.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/configs/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/configs/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/configs/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/configs/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/configs/tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/configs/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/configs/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/namespaces/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/http/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/classes/query_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/classes/responder.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/classes/responder_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/classes/scram.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/classes/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/responders/
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/responders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/responders/add_shard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/responders/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/responders/buildinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/responders/coll_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/responders/company_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/responders/connection_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/responders/count.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/responders/db_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/responders/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/responders/end_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/responders/find.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/responders/get_cmd_line_opts.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/responders/get_free_monitoring_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/responders/get_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/responders/getlog.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/responders/host_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/responders/insert.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/responders/is_master.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/responders/is_master_lower.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/responders/list_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/responders/list_databases.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/responders/list_indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/responders/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/responders/recv_chunk_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/responders/replsetgetstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/responders/sasl_continue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/responders/sasl_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/responders/update_range_deletions.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/responders/whatsmyuri.py
--rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/utilities/mongodb_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/utilities/mongodb_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mongo/utilities/mongodb_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    57762 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/fast_auth_fail_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/password_answer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/datahub/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/datahub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/datahub/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/datahub/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/datahub/datahub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)    23163 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/executor/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/executor/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    68207 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/external_libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/external_libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/libs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/libs/constants/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/libs/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35316 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/libs/constants/response_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    32190 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/utilities/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/utilities/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/mysql/start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/api/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/nlp/nlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/api/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/postgres/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/api/postgres/postgres_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/postgres/postgres_proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/api/postgres/postgres_proxy/executor/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/postgres/postgres_proxy/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/postgres/postgres_proxy/executor/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12729 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    40804 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py
--rw-r--r--   0 runner    (1001) docker     (123)    19291 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/api/postgres/postgres_proxy/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/postgres/postgres_proxy/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/api/postgres/start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/access_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/access_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/access_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/access_handler/access_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    32145 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/access_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/access_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/access_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/access_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/airtable_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/airtable_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/airtable_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/airtable_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/airtable_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/airtable_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/airtable_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/altibase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/altibase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/altibase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)   342129 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/altibase_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/altibase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/altibase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/altibase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/aurora_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/aurora_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/aurora_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/aurora_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/aurora_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/aurora_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/aurora_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/autokeras_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/autokeras_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/autokeras_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/autokeras_handler/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/autokeras_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/autosklearn_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/autosklearn_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/autosklearn_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/autosklearn_handler/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/autosklearn_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/autosklearn_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/bigquery_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/bigquery_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/bigquery_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/bigquery_handler/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/bigquery_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/bigquery_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/bigquery_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/binance_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/binance_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/binance_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/binance_handler/binance_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/binance_handler/binance_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/binance_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/binance_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/byom_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/byom_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/byom_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/byom_handler/byom_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cassandra_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cassandra_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cassandra_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)   176707 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cassandra_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cassandra_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cassandra_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cassandra_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ckan_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ckan_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ckan_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ckan_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ckan_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ckan_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ckan_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/clickhouse_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/clickhouse_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/clickhouse_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/clickhouse_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/clickhouse_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/clickhouse_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cloud_sql_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cloud_sql_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    37571 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cloud_sql_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cloud_sql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cockroach_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cockroach_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cockroach_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cockroach_handler/cockroach_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cockroach_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cockroach_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cockroach_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cohere_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cohere_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cohere_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cohere_handler/cohere_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cohere_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/cohere_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/confluence_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/confluence_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/confluence_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/confluence_handler/confluence_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    76194 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/confluence_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/confluence_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/couchbase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/couchbase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/couchbase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/couchbase_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/couchbase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/couchbase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/couchbase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/crate_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/crate_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/crate_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/crate_handler/crate_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/crate_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/crate_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/crate_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/crate_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/d0lt_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/d0lt_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/d0lt_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    85600 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/d0lt_handler/create-db.png
--rw-r--r--   0 runner    (1001) docker     (123)    98275 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/d0lt_handler/create-predictor.png
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/d0lt_handler/d0lt_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/d0lt_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)    98983 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/d0lt_handler/predict-target.png
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/d0lt_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/d0lt_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/d0lt_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/databend_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/databend_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/databend_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/databend_handler/databend_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/databend_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/databend_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/databend_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/databend_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/databricks_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/databricks_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/databricks_handler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/
--rw-r--r--   0 runner    (1001) docker     (123)    86110 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    58645 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    35986 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    21694 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    62078 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/databricks_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/databricks_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/databricks_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/databricks_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/datastax_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/datastax_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/datastax_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/datastax_handler/datastax_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    26175 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/datastax_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/datastax_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/datastax_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/datastax_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/db2_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/db2_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/db2_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/db2_handler/db2_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19117 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/db2_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/db2_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/db2_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/db2_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/derby_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/derby_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/derby_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/derby_handler/derby_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/derby_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/derby_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/derby_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/derby_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/dremio_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/dremio_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/dremio_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    52734 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/dremio_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/dremio_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/dremio_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/dremio_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/druid_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/druid_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/druid_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/druid_handler/druid_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    29112 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/druid_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/druid_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/druid_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/druid_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/duckdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/duckdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/duckdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19548 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/duckdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/duckdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/duckdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/duckdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/dynamodb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/dynamodb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/dynamodb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    55623 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/dynamodb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/dynamodb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/dynamodb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/dynamodb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/edgelessdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/edgelessdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/edgelessdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/elasticsearch_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/elasticsearch_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/elasticsearch_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/elasticsearch_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/empress_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/empress_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/empress_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/empress_handler/empress_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/empress_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/empress_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/empress_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/empress_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/eventstoredb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/eventstoredb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/eventstoredb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/file_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/file_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/file_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/file_handler/file_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/firebird_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/firebird_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/firebird_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    54033 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/firebird_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/firebird_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/firebird_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/firebird_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/flaml_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/flaml_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/flaml_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/flaml_handler/flaml_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/flaml_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/flaml_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/frappe_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/frappe_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/frappe_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/frappe_handler/frappe_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/frappe_handler/frappe_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/frappe_handler/frappe_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/frappe_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/frappe_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/github_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/github_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/github_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/github_handler/github_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    21392 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/github_handler/github_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/github_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/github_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/gitlab_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/gitlab_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/gitlab_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    15343 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/gitlab_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/gitlab_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/gmail_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/gmail_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/gmail_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19068 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/gmail_handler/gmail_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/gmail_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/gmail_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/gmail_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/gmail_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/gmail_handler/tests/test_gmail_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_books_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_books_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_books_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_books_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_books_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_books_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_books_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_calendar_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_calendar_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_calendar_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_calendar_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_calendar_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_calendar_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_calendar_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16251 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)    34337 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_fit_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_fit_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_fit_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)    21355 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_fit_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_fit_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_search_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_search_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_search_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_search_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_search_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_search_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_search_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/hackernews_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/hackernews_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/hackernews_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/hackernews_handler/hn_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/hackernews_handler/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/hana_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/hana_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/hana_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/hana_handler/hana_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/hana_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/hana_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/hive_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/hive_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/hive_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/hive_handler/hive_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14000 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/hive_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/hive_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/hive_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/hive_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/hsqldb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/hsqldb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/hsqldb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/hsqldb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/hsqldb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/huggingface_api_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/huggingface_api_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/huggingface_api_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/huggingface_api_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/huggingface_api_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/huggingface_api_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/huggingface_api_handler/tests/test_huggingface_api_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/huggingface_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/huggingface_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/huggingface_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/huggingface_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/huggingface_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ignite_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ignite_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ignite_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45779 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ignite_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ignite_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ignite_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ignite_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/impala_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/impala_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/impala_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/impala_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/impala_handler/impala_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/impala_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/impala_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/impala_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/influxdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/influxdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/influxdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63375 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/influxdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/influxdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/informix_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/informix_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/informix_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/informix_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/informix_handler/informix_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/informix_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/informix_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/informix_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ingres_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ingres_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ingres_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ingres_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ingres_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ingres_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ingres_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/jira_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/jira_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/jira_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16812 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/jira_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/jira_handler/jira_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/jira_handler/jira_table.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/jira_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/langchain_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/langchain_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/langchain_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21902 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/langchain_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/langchain_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/lightfm_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/lightfm_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/lightfm_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/lightfm_handler/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/lightfm_handler/lightfm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/lightfm_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/lightfm_handler/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/lightfm_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/lightwood_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/lightwood_handler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22116 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/lightwood_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/lightwood_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/lightwood_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/lightwood_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/llama_index_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/llama_index_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/llama_index_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/llama_index_handler/llama_index_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/llama_index_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/llama_index_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ludwig_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ludwig_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ludwig_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ludwig_handler/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ludwig_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ludwig_handler/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ludwig_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mariadb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mariadb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mariadb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mariadb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mariadb_handler/mariadb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mariadb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/materialize_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/materialize_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/materialize_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47935 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/materialize_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/materialize_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/materialize_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/materialize_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/matrixone_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/matrixone_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/matrixone_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57976 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/matrixone_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/matrixone_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/matrixone_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/matrixone_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/maxdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/maxdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/maxdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26795 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/maxdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/maxdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/maxdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/maxdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mediawiki_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mediawiki_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mediawiki_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   164968 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mediawiki_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mediawiki_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mendeley_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mendeley_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mendeley_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mendeley_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mendeley_handler/mendeley_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mendeley_handler/mendeley_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mendeley_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mendeley_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mendeley_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mendeley_handler/tests/test_mendeley_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/merlion_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/merlion_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/merlion_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/merlion_handler/adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/merlion_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/merlion_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mlflow_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mlflow_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mlflow_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mlflow_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mlflow_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/monetdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/monetdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/monetdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   544421 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/monetdb_handler/create-database.png
--rw-r--r--   0 runner    (1001) docker     (123)   423554 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/monetdb_handler/create-predictor.png
--rw-r--r--   0 runner    (1001) docker     (123)    64685 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/monetdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/monetdb_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)   445044 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/monetdb_handler/select-predictor.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/monetdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/monetdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/monetdb_handler/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/monetdb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mongodb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mongodb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mongodb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mongodb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mongodb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mongodb_handler/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mongodb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/monkeylearn_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/monkeylearn_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/monkeylearn_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/monkeylearn_handler/monkeylearn_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/monkeylearn_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/monkeylearn_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mssql_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mssql_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mssql_handler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14543 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mssql_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mssql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mssql_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mssql_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mysql_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mysql_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mysql_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mysql_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/mysql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/neuralforecast_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/neuralforecast_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/neuralforecast_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/neuralforecast_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/neuralforecast_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/newsapi_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/newsapi_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/newsapi_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/newsapi_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/newsapi_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/newsapi_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/newsapi_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    95071 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/oceanbase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/oceanbase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/oceanbase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37289 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/oceanbase_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/oceanbase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/oceanbase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/oceanbase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/openai_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/openai_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/openai_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/openai_handler/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    29594 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/openai_handler/openai_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/openai_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/openai_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/opengauss_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/opengauss_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/opengauss_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/opengauss_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/opengauss_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/opengauss_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/oracle_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/oracle_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/oracle_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/oracle_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/oracle_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/oracle_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/oracle_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/orioledb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/orioledb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/orioledb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/orioledb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/orioledb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/orioledb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/orioledb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/paypal_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/paypal_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/paypal_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/paypal_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/paypal_handler/paypal_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/paypal_handler/paypal_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/paypal_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/phoenix_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/phoenix_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/phoenix_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/phoenix_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/phoenix_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/phoenix_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/phoenix_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/pinot_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/pinot_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/pinot_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18645 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/pinot_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/pinot_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/pinot_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/pinot_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/plaid_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/plaid_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/plaid_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/plaid_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/plaid_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/plaid_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/planetscale_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/planetscale_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/planetscale_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    97032 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/planetscale_handler/create-db.png
--rw-r--r--   0 runner    (1001) docker     (123)    98334 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/planetscale_handler/create-predictor.png
--rw-r--r--   0 runner    (1001) docker     (123)    63619 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/planetscale_handler/drop-db.png
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/planetscale_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/planetscale_handler/planetscale_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)   112840 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/planetscale_handler/predict-target.png
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/planetscale_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/popularity_recommender_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/popularity_recommender_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/popularity_recommender_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/popularity_recommender_handler/popularity_recommender_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/popularity_recommender_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/popularity_recommender_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/postgres_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/postgres_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/postgres_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15261 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/postgres_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/postgres_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/questdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/questdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/questdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/questdb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/questdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/questdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/questdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/quickbooks_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/quickbooks_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/quickbooks_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/quickbooks_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/quickbooks_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ray_serve_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ray_serve_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ray_serve_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ray_serve_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/ray_serve_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/realtime_slack_chat_handler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/realtime_slack_chat_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/realtime_slack_chat_handler/realtime_slack_chat_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/realtime_slack_chat_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/reddit_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/reddit_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/reddit_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/reddit_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/reddit_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/redshift_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/redshift_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/redshift_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/redshift_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/redshift_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/redshift_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/redshift_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/rocket_chat_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/rocket_chat_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/rocket_chat_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/rocket_chat_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/rocket_chat_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/rockset_handler/
--rw-r--r--   0 runner    (1001) docker     (123)    22361 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/rockset_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/rockset_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/rockset_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)   194064 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/rockset_handler/tests/test.png
--rw-r--r--   0 runner    (1001) docker     (123)   108141 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/rockset_handler/tests/test2.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/s3_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/s3_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/s3_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24332 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/s3_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/s3_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/s3_handler/s3_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/s3_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/s3_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/scylla_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/scylla_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/scylla_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/scylla_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/scylla_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/scylla_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/scylla_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sendinblue_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sendinblue_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sendinblue_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sendinblue_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sendinblue_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sheets_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sheets_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sheets_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27211 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sheets_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sheets_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sheets_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sheets_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/shopify_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/shopify_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/shopify_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26694 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/shopify_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/shopify_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/shopify_handler/shopify_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/shopify_handler/shopify_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/singlestore_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/singlestore_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/singlestore_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/singlestore_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/singlestore_handler/singlestore_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/singlestore_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/singlestore_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/slack_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/slack_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/slack_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/slack_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/slack_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13091 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/slack_handler/slack_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/slack_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/slack_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/snowflake_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/snowflake_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/snowflake_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/snowflake_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/snowflake_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/snowflake_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/solr_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/solr_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/solr_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/solr_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/solr_handler/solr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/solr_handler/solr_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/solr_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/solr_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqlany_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqlany_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqlany_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqlany_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqlany_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqlite_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqlite_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqlite_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   521282 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqlite_handler/db_connection.png
--rw-r--r--   0 runner    (1001) docker     (123)   369371 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqlite_handler/error.png
--rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqlite_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)   479779 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqlite_handler/model_drop.png
--rw-r--r--   0 runner    (1001) docker     (123)   477242 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png
--rw-r--r--   0 runner    (1001) docker     (123)   552154 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqlite_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqlite_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqreamdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqreamdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqreamdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqreamdb_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/starrocks_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/starrocks_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/starrocks_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72778 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/starrocks_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/starrocks_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/starrocks_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/starrocks_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/statsforecast_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/statsforecast_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/statsforecast_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/statsforecast_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/statsforecast_handler/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/strava_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/strava_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/strava_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/strava_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/strava_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/strava_handler/strava_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/strava_handler/strava_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/stripe_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/stripe_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/stripe_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58244 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/stripe_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/stripe_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/stripe_handler/stripe_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/stripe_handler/stripe_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/supabase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/supabase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/supabase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/supabase_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/supabase_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/supabase_handler/supabase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/supabase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/supabase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/surrealdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/surrealdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/surrealdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25475 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/surrealdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/surrealdb_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/surrealdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/surrealdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/surrealdb_handler/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/surrealdb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/tdengine_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/tdengine_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/tdengine_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/tdengine_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/tdengine_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/tdengine_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/tdengine_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/teradata_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/teradata_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/teradata_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/teradata_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/teradata_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/tidb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/tidb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/tidb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/tidb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/tidb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/tidb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/timescaledb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/timescaledb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/timescaledb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/timescaledb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/timescaledb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/timescaledb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/timescaledb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/tpot_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/tpot_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/tpot_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/tpot_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/tpot_handler/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/trino_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/trino_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/trino_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/trino_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/trino_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/trino_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/trino_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/trino_handler/trino_config_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/trino_handler/trino_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/twitter_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/twitter_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/twitter_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/twitter_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/twitter_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/utilities/query_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/utilities/query_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/utilities/query_utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/utilities/query_utilities/insert_query_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/utilities/query_utilities/select_query_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/vertica_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/vertica_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/vertica_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/vertica_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/vertica_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/vertica_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/vertica_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/vitess_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/vitess_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/vitess_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/vitess_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/vitess_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/vitess_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/vitess_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/web_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/web_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/web_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39688 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/web_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/web_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/web_handler/urlcrawl_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/web_handler/web_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/writer_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/writer_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/writer_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/writer_handler/ingest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/writer_handler/question_answer.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/writer_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/writer_handler/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/writer_handler/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/writer_handler/writer_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/youtube_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/youtube_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/youtube_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/youtube_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/youtube_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/yugabyte_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/yugabyte_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/yugabyte_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16563 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/yugabyte_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/yugabyte_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/yugabyte_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/yugabyte_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers_client/db_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers_client/db_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers_client/ml_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers_client/ml_grpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers_wrapper/db_handler_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/handlers_wrapper/ml_handler_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/libs/api_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/libs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/libs/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/libs/handler_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/libs/learn_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    21976 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/libs/ml_exec_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/libs/ml_handler_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/libs/net_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/libs/realtime_chat_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/libs/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/libs/storage_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/integrations/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/utilities/date_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/utilities/install.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/utilities/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/utilities/sql_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/utilities/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/utilities/time_series_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/integrations/utilities/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/interfaces/chatbot/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/chatbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/chatbot/chatbot_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/chatbot/chatbot_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/chatbot/chatbot_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/chatbot/chatbot_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/chatbot/chatbot_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/chatbot/chatbot_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/chatbot/realtime_chat_handler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/chatbot/realtime_chatbot_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/chatbot/realtime_chatbot_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/interfaces/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/database/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    23786 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/database/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    11314 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/database/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/database/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/interfaces/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/file/file_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/interfaces/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/jobs/jobs_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/jobs/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/interfaces/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/model/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22548 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/model/model_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/interfaces/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11498 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/storage/db.py
--rw-r--r--   0 runner    (1001) docker     (123)    18626 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/storage/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/storage/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/storage/model_fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/interfaces/stream/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/stream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/interfaces/stream/base/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/stream/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/stream/base/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/stream/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/interfaces/stream/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/microservices_grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/microservices_grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/microservices_grpc/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/microservices_grpc/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/microservices_grpc/db/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/microservices_grpc/db/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/microservices_grpc/db/db_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/microservices_grpc/db/db_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/microservices_grpc/executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/microservices_grpc/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/microservices_grpc/executor/executor_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/microservices_grpc/ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/microservices_grpc/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/microservices_grpc/ml/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/microservices_grpc/ml/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/microservices_grpc/ml/ml_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/migrate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py
--rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/versions/2023-05-24_6d748f2c7b0b_remove_streams.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/versions/2023-05-31_aaecd7012a78_chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/versions/2023-06-16_9d6271bb2c38_update_chat_bots_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/versions/2023-06-19_b5bf593ba659_create_chat_bots_history_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/versions/2023-06-27_607709e1615b_update_project_names.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/migrations/versions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/utilities/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/utilities/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/utilities/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/utilities/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/utilities/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/utilities/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/utilities/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/utilities/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/utilities/hooks/profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/utilities/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/utilities/log_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/mindsdb/utilities/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/utilities/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/utilities/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/utilities/ps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/utilities/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/mindsdb/utilities/wizards.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/requirements/requirements-grpc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/requirements/requirements-telemetry.txt
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 15:57:35.000000 MindsDB-23.7.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-18 15:57:18.000000 MindsDB-23.7.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-25 08:32:49.000000 MindsDB-23.7.4.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/MindsDB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25650 2023-07-25 08:33:04.000000 MindsDB-23.7.4.0/MindsDB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    68913 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/MindsDB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 08:33:04.000000 MindsDB-23.7.4.0/MindsDB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-07-25 08:33:04.000000 MindsDB-23.7.4.0/MindsDB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-25 08:33:04.000000 MindsDB-23.7.4.0/MindsDB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25650 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20461 2023-07-25 08:32:49.000000 MindsDB-23.7.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/api/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/common/check_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/api/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/gunicorn_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13175 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/chatbots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/configs/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/configs/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/configs/chatbots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/configs/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/configs/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/configs/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/configs/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/configs/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/configs/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/configs/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/configs/tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/configs/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/configs/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9685 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/namespaces/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/http/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/classes/query_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/classes/responder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/classes/responder_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/classes/scram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/classes/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/responders/
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/responders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/responders/add_shard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/responders/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/responders/buildinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/responders/coll_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/responders/company_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/responders/connection_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/responders/count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/responders/db_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/responders/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/responders/end_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/responders/find.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/responders/get_cmd_line_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/responders/get_free_monitoring_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/responders/get_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/responders/getlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/responders/host_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/responders/insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/responders/is_master.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/responders/is_master_lower.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/responders/list_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/responders/list_databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/responders/list_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/responders/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/responders/recv_chunk_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/responders/replsetgetstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/responders/sasl_continue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/responders/sasl_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/responders/update_range_deletions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/responders/whatsmyuri.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/utilities/mongodb_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/utilities/mongodb_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mongo/utilities/mongodb_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57762 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/fast_auth_fail_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/password_answer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/datahub/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/datahub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/datahub/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/datahub/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/datahub/datahub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23163 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/executor/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/executor/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68207 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/external_libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/external_libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/libs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/libs/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/libs/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35316 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/libs/constants/response_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32190 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/utilities/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/utilities/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/mysql/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/api/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/nlp/nlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/api/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/postgres/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/api/postgres/postgres_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/postgres/postgres_proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/api/postgres/postgres_proxy/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/postgres/postgres_proxy/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/postgres/postgres_proxy/executor/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12729 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40804 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19291 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/api/postgres/postgres_proxy/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/postgres/postgres_proxy/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/api/postgres/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/access_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/access_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/access_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/access_handler/access_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32145 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/access_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/access_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/access_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/access_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/airtable_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/airtable_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/airtable_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/airtable_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/airtable_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/airtable_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/airtable_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/altibase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/altibase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/altibase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)   342129 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/altibase_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/altibase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/altibase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/altibase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/aurora_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/aurora_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/aurora_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/aurora_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/aurora_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/aurora_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/aurora_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/autokeras_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/autokeras_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/autokeras_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/autokeras_handler/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/autokeras_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/autosklearn_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/autosklearn_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/autosklearn_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/autosklearn_handler/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/autosklearn_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/autosklearn_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/bigquery_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/bigquery_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/bigquery_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/bigquery_handler/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/bigquery_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/bigquery_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/bigquery_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/binance_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/binance_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/binance_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/binance_handler/binance_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/binance_handler/binance_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/binance_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/binance_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/byom_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/byom_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/byom_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/byom_handler/byom_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cassandra_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cassandra_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cassandra_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)   176707 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cassandra_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cassandra_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cassandra_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cassandra_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ckan_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ckan_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ckan_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ckan_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ckan_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ckan_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ckan_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/clickhouse_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/clickhouse_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/clickhouse_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/clickhouse_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/clickhouse_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/clickhouse_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cloud_spanner_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cloud_spanner_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cloud_spanner_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cloud_sql_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cloud_sql_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37571 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cloud_sql_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cloud_sql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cockroach_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cockroach_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cockroach_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cockroach_handler/cockroach_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cockroach_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cockroach_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cockroach_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cohere_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cohere_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cohere_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cohere_handler/cohere_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cohere_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/cohere_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/confluence_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/confluence_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/confluence_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/confluence_handler/confluence_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76194 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/confluence_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/confluence_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/couchbase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/couchbase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/couchbase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/couchbase_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/couchbase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/couchbase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/couchbase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/crate_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/crate_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/crate_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/crate_handler/crate_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/crate_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/crate_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/crate_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/crate_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/d0lt_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/d0lt_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/d0lt_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85600 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/d0lt_handler/create-db.png
+-rw-r--r--   0 runner    (1001) docker     (123)    98275 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/d0lt_handler/create-predictor.png
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/d0lt_handler/d0lt_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/d0lt_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    98983 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/d0lt_handler/predict-target.png
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/d0lt_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/d0lt_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/d0lt_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/databend_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/databend_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/databend_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/databend_handler/databend_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/databend_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/databend_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/databend_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/databend_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/databricks_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/databricks_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/databricks_handler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/databricks_handler/databricks/
+-rw-r--r--   0 runner    (1001) docker     (123)    86110 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    58645 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    35986 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    21694 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    62078 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/databricks_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/databricks_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/databricks_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/databricks_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/datastax_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/datastax_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/datastax_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/datastax_handler/datastax_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26175 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/datastax_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/datastax_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/datastax_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/datastax_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/db2_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/db2_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/db2_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/db2_handler/db2_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19117 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/db2_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/db2_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/db2_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/db2_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/derby_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/derby_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/derby_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/derby_handler/derby_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/derby_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/derby_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/derby_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/derby_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/dremio_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/dremio_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/dremio_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52734 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/dremio_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/dremio_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/dremio_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/dremio_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/druid_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/druid_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/druid_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/druid_handler/druid_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29112 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/druid_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/druid_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/druid_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/druid_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/duckdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/duckdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/duckdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19548 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/duckdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/duckdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/duckdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/duckdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/dynamodb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/dynamodb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/dynamodb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55623 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/dynamodb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/dynamodb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/dynamodb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/dynamodb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/edgelessdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/edgelessdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/edgelessdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/elasticsearch_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/elasticsearch_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/elasticsearch_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/elasticsearch_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/empress_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/empress_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/empress_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/empress_handler/empress_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/empress_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/empress_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/empress_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/empress_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/eventstoredb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/eventstoredb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/eventstoredb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/file_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/file_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/file_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/file_handler/file_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/firebird_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/firebird_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/firebird_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54033 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/firebird_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/firebird_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/firebird_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/firebird_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/flaml_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/flaml_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/flaml_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/flaml_handler/flaml_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/flaml_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/flaml_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/frappe_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/frappe_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/frappe_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/frappe_handler/frappe_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/frappe_handler/frappe_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/frappe_handler/frappe_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/frappe_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/frappe_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/github_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/github_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/github_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/github_handler/github_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21392 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/github_handler/github_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/github_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/github_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/gitlab_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/gitlab_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/gitlab_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15343 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/gitlab_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/gitlab_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/gmail_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/gmail_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/gmail_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19068 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/gmail_handler/gmail_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/gmail_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/gmail_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/gmail_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/gmail_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/gmail_handler/tests/test_gmail_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_books_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_books_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_books_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_books_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_books_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_books_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_books_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_calendar_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_calendar_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_calendar_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_calendar_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_calendar_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_calendar_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_calendar_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_content_shopping_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_content_shopping_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16251 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34337 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_content_shopping_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_content_shopping_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_fit_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_fit_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_fit_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21355 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_fit_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_fit_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_search_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_search_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_search_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_search_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_search_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_search_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_search_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/hackernews_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/hackernews_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/hackernews_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/hackernews_handler/hn_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/hackernews_handler/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/hana_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/hana_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/hana_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/hana_handler/hana_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/hana_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/hana_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/hive_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/hive_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/hive_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/hive_handler/hive_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14000 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/hive_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/hive_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/hive_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/hive_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/hsqldb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/hsqldb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/hsqldb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/hsqldb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/hsqldb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/huggingface_api_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/huggingface_api_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/huggingface_api_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/huggingface_api_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/huggingface_api_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/huggingface_api_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/huggingface_api_handler/tests/test_huggingface_api_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/huggingface_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/huggingface_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/huggingface_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/huggingface_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/huggingface_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ignite_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ignite_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ignite_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45779 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ignite_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ignite_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ignite_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ignite_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/impala_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/impala_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/impala_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/impala_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/impala_handler/impala_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/impala_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/impala_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/impala_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/influxdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/influxdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/influxdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63375 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/influxdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/influxdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/informix_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/informix_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/informix_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/informix_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/informix_handler/informix_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/informix_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/informix_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/informix_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ingres_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ingres_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ingres_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ingres_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ingres_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ingres_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ingres_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/jira_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/jira_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/jira_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16812 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/jira_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/jira_handler/jira_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/jira_handler/jira_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/jira_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/langchain_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/langchain_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/langchain_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24806 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/langchain_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/langchain_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/lightfm_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/lightfm_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/lightfm_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/lightfm_handler/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/lightfm_handler/lightfm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/lightfm_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/lightfm_handler/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/lightfm_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/lightwood_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/lightwood_handler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22116 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/lightwood_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/lightwood_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/lightwood_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/lightwood_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/llama_index_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/llama_index_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/llama_index_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/llama_index_handler/llama_index_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/llama_index_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/llama_index_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ludwig_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ludwig_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ludwig_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ludwig_handler/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ludwig_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ludwig_handler/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ludwig_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mariadb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mariadb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mariadb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mariadb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mariadb_handler/mariadb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mariadb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/materialize_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/materialize_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/materialize_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47935 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/materialize_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/materialize_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/materialize_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/materialize_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/matrixone_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/matrixone_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/matrixone_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57976 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/matrixone_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/matrixone_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/matrixone_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/matrixone_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/maxdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/maxdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/maxdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26795 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/maxdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/maxdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/maxdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/maxdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mediawiki_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mediawiki_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mediawiki_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   164968 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mediawiki_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mediawiki_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mendeley_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mendeley_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mendeley_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mendeley_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mendeley_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mendeley_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mendeley_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mendeley_handler/tests/test_mendeley_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/merlion_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/merlion_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/merlion_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/merlion_handler/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/merlion_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/merlion_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mlflow_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mlflow_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mlflow_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mlflow_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mlflow_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/monetdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/monetdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/monetdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   544421 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/monetdb_handler/create-database.png
+-rw-r--r--   0 runner    (1001) docker     (123)   423554 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/monetdb_handler/create-predictor.png
+-rw-r--r--   0 runner    (1001) docker     (123)    64685 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/monetdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/monetdb_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   445044 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/monetdb_handler/select-predictor.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/monetdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/monetdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/monetdb_handler/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/monetdb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mongodb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mongodb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mongodb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mongodb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mongodb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mongodb_handler/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mongodb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/monkeylearn_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/monkeylearn_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/monkeylearn_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/monkeylearn_handler/monkeylearn_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/monkeylearn_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/monkeylearn_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mssql_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mssql_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mssql_handler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14543 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mssql_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mssql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mssql_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mssql_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mysql_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mysql_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mysql_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mysql_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/mysql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/neuralforecast_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/neuralforecast_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/neuralforecast_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/neuralforecast_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/neuralforecast_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/newsapi_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/newsapi_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/newsapi_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/newsapi_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/newsapi_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/newsapi_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/newsapi_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/nuo_jdbc_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/nuo_jdbc_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95071 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/nuo_jdbc_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/oceanbase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/oceanbase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/oceanbase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37289 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/oceanbase_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/oceanbase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/oceanbase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/oceanbase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/openai_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/openai_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/openai_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/openai_handler/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28654 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/openai_handler/openai_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/openai_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/openai_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/opengauss_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/opengauss_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/opengauss_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/opengauss_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/opengauss_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/opengauss_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/oracle_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/oracle_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/oracle_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/oracle_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/oracle_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/oracle_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/oracle_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/orioledb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/orioledb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/orioledb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/orioledb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/orioledb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/orioledb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/orioledb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/paypal_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/paypal_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/paypal_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/paypal_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/paypal_handler/paypal_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/paypal_handler/paypal_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/paypal_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/phoenix_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/phoenix_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/phoenix_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/phoenix_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/phoenix_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/phoenix_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/phoenix_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/pinot_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/pinot_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/pinot_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18645 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/pinot_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/pinot_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/pinot_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/pinot_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/plaid_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/plaid_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/plaid_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/plaid_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/plaid_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/plaid_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/planetscale_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/planetscale_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/planetscale_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97032 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/planetscale_handler/create-db.png
+-rw-r--r--   0 runner    (1001) docker     (123)    98334 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/planetscale_handler/create-predictor.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63619 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/planetscale_handler/drop-db.png
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/planetscale_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/planetscale_handler/planetscale_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112840 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/planetscale_handler/predict-target.png
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/planetscale_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/popularity_recommender_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/popularity_recommender_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/popularity_recommender_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/popularity_recommender_handler/popularity_recommender_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/popularity_recommender_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/popularity_recommender_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/postgres_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/postgres_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/postgres_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15261 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/postgres_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/postgres_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/questdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/questdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/questdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/questdb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/questdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/questdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/questdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/quickbooks_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/quickbooks_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/quickbooks_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/quickbooks_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/quickbooks_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ray_serve_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ray_serve_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ray_serve_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ray_serve_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/ray_serve_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/realtime_slack_chat_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/realtime_slack_chat_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/realtime_slack_chat_handler/realtime_slack_chat_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/realtime_slack_chat_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/reddit_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/reddit_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/reddit_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/reddit_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/reddit_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/redshift_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/redshift_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/redshift_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/redshift_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/redshift_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/redshift_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/redshift_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/rocket_chat_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/rocket_chat_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/rocket_chat_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/rocket_chat_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/rocket_chat_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/rockset_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)    22361 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/rockset_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/rockset_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/rockset_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   194064 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/rockset_handler/tests/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)   108141 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/rockset_handler/tests/test2.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/s3_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/s3_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/s3_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24332 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/s3_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/s3_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/s3_handler/s3_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/s3_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/s3_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/scylla_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/scylla_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/scylla_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/scylla_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/scylla_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/scylla_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/scylla_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sendinblue_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sendinblue_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sendinblue_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sendinblue_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sendinblue_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sheets_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sheets_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sheets_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27211 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sheets_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sheets_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sheets_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sheets_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/shopify_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/shopify_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/shopify_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26694 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/shopify_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/shopify_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/shopify_handler/shopify_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/shopify_handler/shopify_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/singlestore_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/singlestore_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/singlestore_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/singlestore_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/singlestore_handler/singlestore_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/singlestore_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/singlestore_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/slack_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/slack_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/slack_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/slack_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/slack_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13091 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/slack_handler/slack_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/slack_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/slack_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/snowflake_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/snowflake_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/snowflake_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/snowflake_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/snowflake_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/snowflake_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/solr_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/solr_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/solr_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/solr_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/solr_handler/solr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/solr_handler/solr_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/solr_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/solr_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqlany_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqlany_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqlany_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqlany_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqlany_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqlite_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqlite_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqlite_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   521282 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqlite_handler/db_connection.png
+-rw-r--r--   0 runner    (1001) docker     (123)   369371 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqlite_handler/error.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqlite_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)   479779 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqlite_handler/model_drop.png
+-rw-r--r--   0 runner    (1001) docker     (123)   477242 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png
+-rw-r--r--   0 runner    (1001) docker     (123)   552154 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqlite_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqlite_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqreamdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqreamdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqreamdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqreamdb_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/starrocks_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/starrocks_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/starrocks_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72778 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/starrocks_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/starrocks_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/starrocks_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/starrocks_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/statsforecast_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/statsforecast_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/statsforecast_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/statsforecast_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/statsforecast_handler/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/strava_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/strava_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/strava_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/strava_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/strava_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/strava_handler/strava_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/strava_handler/strava_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/stripe_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/stripe_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/stripe_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58244 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/stripe_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/stripe_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/stripe_handler/stripe_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/stripe_handler/stripe_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/supabase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/supabase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/supabase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/supabase_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/supabase_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/supabase_handler/supabase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/supabase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/supabase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/surrealdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/surrealdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/surrealdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25475 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/surrealdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/surrealdb_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/surrealdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/surrealdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/surrealdb_handler/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/surrealdb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/tdengine_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/tdengine_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/tdengine_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/tdengine_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/tdengine_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/tdengine_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/tdengine_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/teradata_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/teradata_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/teradata_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/teradata_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/teradata_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/tidb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/tidb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/tidb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/tidb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/tidb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/tidb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/timescaledb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/timescaledb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/timescaledb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/timescaledb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/timescaledb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/timescaledb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/timescaledb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/tpot_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/tpot_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/tpot_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/tpot_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/tpot_handler/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/trino_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/trino_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/trino_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/trino_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/trino_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/trino_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/trino_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/trino_handler/trino_config_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/trino_handler/trino_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/twitter_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/twitter_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/twitter_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/twitter_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/twitter_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/utilities/query_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/utilities/query_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/utilities/query_utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/utilities/query_utilities/insert_query_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/utilities/query_utilities/select_query_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/vertica_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/vertica_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/vertica_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/vertica_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/vertica_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/vertica_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/vertica_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/vitess_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/vitess_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/vitess_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/vitess_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/vitess_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/vitess_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/vitess_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/web_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/web_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/web_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39688 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/web_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/web_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/web_handler/urlcrawl_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/web_handler/web_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/writer_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/writer_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/writer_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/writer_handler/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/writer_handler/question_answer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/writer_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/writer_handler/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/writer_handler/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/writer_handler/writer_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/youtube_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/youtube_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/youtube_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/youtube_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/youtube_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/yugabyte_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/yugabyte_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/yugabyte_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16563 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/yugabyte_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/yugabyte_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/yugabyte_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/yugabyte_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers_client/db_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers_client/db_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers_client/ml_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers_client/ml_grpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers_wrapper/db_handler_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/handlers_wrapper/ml_handler_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/libs/api_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/libs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/libs/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/libs/handler_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/libs/learn_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21976 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/libs/ml_exec_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/libs/ml_handler_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/libs/net_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/libs/realtime_chat_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/libs/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/libs/storage_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/integrations/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/utilities/date_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/utilities/handler_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/utilities/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/utilities/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/utilities/sql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/utilities/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/utilities/time_series_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/integrations/utilities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/interfaces/chatbot/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/chatbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/chatbot/chatbot_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/chatbot/chatbot_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/chatbot/chatbot_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/chatbot/chatbot_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12096 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/chatbot/chatbot_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/chatbot/chatbot_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/chatbot/realtime_chat_handler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/chatbot/realtime_chatbot_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/chatbot/realtime_chatbot_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/interfaces/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23786 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/database/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11314 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/database/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/database/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/interfaces/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/file/file_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/interfaces/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/jobs/jobs_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/jobs/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/interfaces/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/model/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22570 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/model/model_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/interfaces/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11498 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/storage/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18626 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/storage/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/storage/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/storage/model_fs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/interfaces/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/stream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/interfaces/stream/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/stream/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/stream/base/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/stream/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/interfaces/stream/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/microservices_grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/microservices_grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/microservices_grpc/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/microservices_grpc/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/microservices_grpc/db/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/microservices_grpc/db/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/microservices_grpc/db/db_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/microservices_grpc/db/db_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/microservices_grpc/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/microservices_grpc/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/microservices_grpc/executor/executor_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/microservices_grpc/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/microservices_grpc/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/microservices_grpc/ml/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/microservices_grpc/ml/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/microservices_grpc/ml/ml_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/migrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/versions/2023-05-24_6d748f2c7b0b_remove_streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/versions/2023-05-31_aaecd7012a78_chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/versions/2023-06-16_9d6271bb2c38_update_chat_bots_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/versions/2023-06-19_b5bf593ba659_create_chat_bots_history_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/versions/2023-06-27_607709e1615b_update_project_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/migrations/versions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/utilities/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/utilities/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/utilities/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/utilities/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/utilities/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/utilities/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/utilities/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/utilities/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/utilities/hooks/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/utilities/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/utilities/log_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/mindsdb/utilities/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/utilities/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/utilities/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/utilities/ps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/utilities/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/mindsdb/utilities/wizards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/requirements/requirements-grpc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/requirements/requirements-telemetry.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 08:33:05.000000 MindsDB-23.7.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-25 08:32:50.000000 MindsDB-23.7.4.0/setup.py
```

### Comparing `MindsDB-23.7.3.1/MindsDB.egg-info/PKG-INFO` & `MindsDB-23.7.4.0/MindsDB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MindsDB
-Version: 23.7.3.1
+Version: 23.7.4.0
 Summary: MindsDB server, provides server capabilities to mindsdb native python library
 Home-page: https://github.com/mindsdb/mindsdb
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb/
 Description: <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: MindsDB Version: 23.7.3.1 Summary: MindsDB server,
+Metadata-Version: 2.1 Name: MindsDB Version: 23.7.4.0 Summary: MindsDB server,
 provides server capabilities to mindsdb native python library Home-page: https:
 //github.com/mindsdb/mindsdb Author: MindsDB Inc Author-email:
 jorge@mindsdb.com License: GPL-3.0 Download-URL: https://pypi.org/project/
 mindsdb/ Description:
                                ****** [MindsDB]
                                      ******
       [ROSS_Index_-_Fastest_Growing_Open-Source_Startups_|_Runa_Capital]
```

### Comparing `MindsDB-23.7.3.1/MindsDB.egg-info/SOURCES.txt` & `MindsDB-23.7.4.0/MindsDB.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1048,14 +1048,15 @@
 mindsdb/integrations/libs/ml_handler_proc.py
 mindsdb/integrations/libs/net_helpers.py
 mindsdb/integrations/libs/realtime_chat_handler.py
 mindsdb/integrations/libs/response.py
 mindsdb/integrations/libs/storage_handler.py
 mindsdb/integrations/utilities/__init__.py
 mindsdb/integrations/utilities/date_utils.py
+mindsdb/integrations/utilities/handler_utils.py
 mindsdb/integrations/utilities/install.py
 mindsdb/integrations/utilities/processes.py
 mindsdb/integrations/utilities/sql_utils.py
 mindsdb/integrations/utilities/test_utils.py
 mindsdb/integrations/utilities/time_series_utils.py
 mindsdb/integrations/utilities/utils.py
 mindsdb/interfaces/__init__.py
```

### Comparing `MindsDB-23.7.3.1/MindsDB.egg-info/requires.txt` & `MindsDB-23.7.4.0/MindsDB.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -43,174 +43,175 @@
 pyodbc
 sqlalchemy-access
 
 [airtable]
 duckdb
 
 [all_extras]
-sentry-sdk
 grpcio-tools
+sentry-sdk
 
 [all_handlers_extras]
-snowflake-sqlalchemy>=1.4.3
-hyperopt<1.0
-psycopg2
-praw
-mindsdb>=22.12.4.3
-mindsdb>=22.7.5.0
-pymonetdb
-python-gitlab
-couchbase==4.0.2
-mindsdb_sql<0.5.0,>=0.4.9
-ray<=1.13.0
-tiktoken>=0.3.0
-duckdb==0.7.1.dev187
-stripe
-mindsdb_sql<0.5.0,>=0.4.6
-mediawikiapi
-mindsdb>=23.3.5.0
-pymongo[srv]>=4.1.1
-ludwig[distributed]>=0.5.2
-cohere==4.5.1
+flaml<=1.2.3
+google-auth-httplib2
+thrift-sasl
 pysurrealdb
-clickhouse-sqlalchemy
-sqlalchemy<2.0.0
-tpot<=0.11.7
-psycopg
-monkeylearn==3.6.0
-pyodbc==4.0.34
+slack_sdk
+openai<=0.28.0
+websocket
+sqlalchemy
+pyHive
+openai==0.27.0
+sqlalchemy-databricks
+elasticsearch-dbapi
+praw
+hyperopt<1.0
+tensorflow
+mindsdb_sql<0.5.0,>=0.4.4
+scipy>=1.10.1
+dask
+transformers==4.21.0
+pyhive
+llama-index==0.6.11
+html2text
+pytz
 polars
+pinotdb
+langchain<=0.0.192
+hdbcli
 duckdb
-bs4
+mindsdb>=23.3.5.0
+google-api-python-client
+pandas<=1.4.3
+mindsdb_sql>=0.4.0
+oracledb==1.0.2
+pyphoenix
+ShopifyAPI
+sib_api_v3_sdk
+elasticsearch
 pysqream>=3.2.5
-sqlalchemy-solr
-boto3
-tqdm
+pymysql
+protobuf==3.20.*
+ibm-db
+sasl
+cohere==4.5.1
+dataprep_ml>=0.0.15
+teradatasqlalchemy
+salesforce-merlion<=1.3.1,>=1.2.0
+sqlalchemy-sqlany
+tzlocal
+pyodbc==4.0.34
 google-cloud-spanner
-requests==2.28.0
 pymssql>=2.1.4
-oracledb==1.0.2
-fdb
-hdbcli
-pinotdb
-teradatasql
+psycopg[binary]
+sqlalchemy-access
+tqdm
+mindsdb>=22.7.5.0
+clickhouse-sqlalchemy
+duckdb==0.7.1
+bs4
+sqlalchemy-solr
+sqlalchemy-redshift
+pydantic>=1.10.7
+sqlalchemy-bigquery
+db-dtypes
+crate[sqlalchemy]
+langchain==0.0.238
+langchain==0.0.186
+plaid-python
+mindsdb>=22.12.4.3
 auto-sklearn
-atlassian-python-api
+monkeylearn==3.6.0
+hugging_py_face
+thrift
+sqlalchemy<2.0.0
+couchbase==4.0.2
+google
+mindsdb_sql<0.5.0,>=0.4.6
 mlflow
-ibm-db-sa
-ray[serve]
-chromadb==0.3.25
-dask
-tweepy
-qbosdk
-transformers==4.21.0
-pandas
-scipy>=1.10.1
-snowflake-connector-python>=2.7.12
-sentencepiece==0.1.97
-langchain==0.0.186
-html2text
-sqlalchemy
-pytz
+vertica-python
+binance-connector
+mysql-connector-python
+lightwood[all_extras]>=22.8.1.0
+pymonetdb
+sentence_transformers
+sqlalchemy-informix
+tpot<=0.11.7
+ludwig[distributed]>=0.5.2
+mindsdb>=22.10.2.1
 dill
-hierarchicalforecast<1.0
-sqlalchemy-redshift
-slack_sdk
-mindsdb>=23.3.2.0
-markupsafe==2.0.1
+impyla
+IfxPy
+tiktoken>=0.3.0
+pyignite
+rockset
+sqlalchemy_dremio
+trino~=0.313.0
+psycopg
+neuralforecast<1.5.0,>=1.4.0
 google-cloud-bigquery
-flaml<=1.2.3
-hugging_py_face
+sentencepiece==0.1.97
+qbosdk
+sqlalchemy-hana
+tokenizers==0.12.1
+python-gitlab
+rocketchat_API
+sqlalchemy-vertica-python
+pygithub
+hierarchicalforecast<1.0
+hyperopt
+requests==2.28.0
+duckdb==0.7.1.dev187
+snowflake-connector-python>=2.7.12
 pyodbc
-sentence_transformers
-crate[sqlalchemy]
-newsapi-python
-certifi
 statsforecast<2.0,>=1.4.0
-tzlocal
-tensorflow
-openai==0.27.0
-wikipedia==1.4.0
-sasl
-dataprep_ml>=0.0.15
-pymysql
-protobuf==3.20.*
-IfxPy
-hyperopt
-sqlalchemy-vertica-python
-binance-connector
 paypalrestsdk
-phoenixdb
-langchain<=0.0.192
-sqlalchemy-bigquery
-google-auth-httplib2
-websocket
-ibm-db
-sib_api_v3_sdk
-elasticsearch
-pydruid
-google-auth-oauthlib
-plaid-python
-sqlalchemy-informix
-lightwood[all_extras]>=22.8.1.0
-sqlalchemy-databricks
-psycopg[binary]
-pydantic==1.10.8
-pyHive
-databricks-sql-connector
-google
-duckdb==0.7.1
-sqlalchemy-hana
-impyla
-trino~=0.313.0
-db-dtypes
-sqlalchemy-monetdb
-mindsdb>=22.6.2.1
-sqlalchemy-sqlany
+wikipedia==1.4.0
+openai>=0.27.0
+SQLAlchemy
+ray[serve]
+snowflake-sqlalchemy>=1.4.3
 taospy
-stravalib
-rockset
-requests-kerberos==0.12.0
-llama-index==0.6.11
-mindsdb>=22.10.2.1
-pyphoenix
-google-api-python-client
+redshift_connector
+mindsdb-evaluator>=0.0.6
+mendeley
+mediawikiapi
+ibm-db-sa
+anthropic==0.3.5
+ray<=1.13.0
+stripe
+lightfm==1.17
+mindsdb>=22.6.2.1
+pydantic==1.10.8
 sqlanydb
+ckanapi
+phoenixdb
+requests-kerberos==0.12.0
+markupsafe==2.0.1
+psycopg2
+atlassian-python-api
 torch
-ShopifyAPI
+jaydebeapi
 ingres_sa_dialect==0.3
-thrift-sasl
-teradatasqlalchemy
-mindsdb_sql>=0.4.0
-SQLAlchemy
-vertica-python
-pydantic>=1.10.7
-redshift_connector
 scylla-driver
-salesforce-merlion<=1.3.1,>=1.2.0
-elasticsearch-dbapi
-mindsdb_sql<0.5.0,>=0.4.4
-lightfm==1.17
-thrift
+tweepy
+chromadb==0.3.25
+newsapi-python
+pymongo[srv]>=4.1.1
+databricks-sql-connector
+pandas
+fdb
+certifi
+teradatasql
 pysqream_sqlalchemy>=0.8
-openai>=0.27.0
-ckanapi
-mendeley
-pygithub
-pyignite
-sqlalchemy-access
-rocketchat_API
-mysql-connector-python
-jaydebeapi
-sqlalchemy_dremio
-pandas<=1.4.3
-openai<=0.28.0
-neuralforecast<1.5.0,>=1.4.0
-pyhive
-mindsdb-evaluator>=0.0.6
+sqlalchemy-monetdb
+pydruid
+boto3
+google-auth-oauthlib
+stravalib
 
 [altibase]
 jaydebeapi
 
 [aurora]
 psycopg[binary]
 mysql-connector-python
@@ -397,21 +398,21 @@
 sqlalchemy<2.0.0
 ingres_sa_dialect==0.3
 
 [jira]
 atlassian-python-api
 
 [langchain]
-mindsdb>=23.3.2.0
-mindsdb_sql<0.5.0,>=0.4.9
 openai==0.27.0
-langchain==0.0.186
+langchain==0.0.238
 wikipedia==1.4.0
 pandas
 tiktoken>=0.3.0
+tokenizers==0.12.1
+anthropic==0.3.5
 
 [lightfm]
 lightfm==1.17
 scipy>=1.10.1
 pydantic>=1.10.7
 dataprep_ml>=0.0.15
```

### Comparing `MindsDB-23.7.3.1/PKG-INFO` & `MindsDB-23.7.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MindsDB
-Version: 23.7.3.1
+Version: 23.7.4.0
 Summary: MindsDB server, provides server capabilities to mindsdb native python library
 Home-page: https://github.com/mindsdb/mindsdb
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb/
 Description: <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: MindsDB Version: 23.7.3.1 Summary: MindsDB server,
+Metadata-Version: 2.1 Name: MindsDB Version: 23.7.4.0 Summary: MindsDB server,
 provides server capabilities to mindsdb native python library Home-page: https:
 //github.com/mindsdb/mindsdb Author: MindsDB Inc Author-email:
 jorge@mindsdb.com License: GPL-3.0 Download-URL: https://pypi.org/project/
 mindsdb/ Description:
                                ****** [MindsDB]
                                      ******
       [ROSS_Index_-_Fastest_Growing_Open-Source_Startups_|_Runa_Capital]
```

### Comparing `MindsDB-23.7.3.1/README.md` & `MindsDB-23.7.4.0/README.md`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/__main__.py` & `MindsDB-23.7.4.0/mindsdb/__main__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/common/check_auth.py` & `MindsDB-23.7.4.0/mindsdb/api/common/check_auth.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/http/gui.py` & `MindsDB-23.7.4.0/mindsdb/api/http/gui.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/http/gunicorn_wrapper.py` & `MindsDB-23.7.4.0/mindsdb/api/http/gunicorn_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/http/initialize.py` & `MindsDB-23.7.4.0/mindsdb/api/http/initialize.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/http/namespaces/analysis.py` & `MindsDB-23.7.4.0/mindsdb/api/http/namespaces/analysis.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/http/namespaces/auth.py` & `MindsDB-23.7.4.0/mindsdb/api/http/namespaces/auth.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/http/namespaces/chatbots.py` & `MindsDB-23.7.4.0/mindsdb/api/http/namespaces/chatbots.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/http/namespaces/config.py` & `MindsDB-23.7.4.0/mindsdb/api/http/namespaces/config.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/http/namespaces/databases.py` & `MindsDB-23.7.4.0/mindsdb/api/http/namespaces/databases.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/http/namespaces/default.py` & `MindsDB-23.7.4.0/mindsdb/api/http/namespaces/default.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/http/namespaces/file.py` & `MindsDB-23.7.4.0/mindsdb/api/http/namespaces/file.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/http/namespaces/handlers.py` & `MindsDB-23.7.4.0/mindsdb/api/http/namespaces/handlers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/http/namespaces/models.py` & `MindsDB-23.7.4.0/mindsdb/api/http/namespaces/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,15 @@
                 'active': model_df.at[0, 'ACTIVE'],
                 'version': model_df.at[0, 'VERSION'],
                 'status': model_df.at[0, 'STATUS'],
                 'predict': model_df.at[0, 'PREDICT'],
                 'mindsdb_version': model_df.at[0, 'MINDSDB_VERSION'],
                 'error': model_df.at[0, 'ERROR'],
                 'fetch_data_query': model_df.at[0, 'SELECT_DATA_QUERY'],
+                'problem_definition': model_df.at[0, 'TRAINING_OPTIONS']
             }, HTTPStatus.CREATED
         except Exception as e:
             return http_error(
                 HTTPStatus.INTERNAL_SERVER_ERROR,
                 'Unable to train model',
                 f'Something went wrong while creating and training model {model_name}: {e}')
```

### Comparing `MindsDB-23.7.3.1/mindsdb/api/http/namespaces/projects.py` & `MindsDB-23.7.4.0/mindsdb/api/http/namespaces/projects.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/http/namespaces/sql.py` & `MindsDB-23.7.4.0/mindsdb/api/http/namespaces/sql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/http/namespaces/tab.py` & `MindsDB-23.7.4.0/mindsdb/api/http/namespaces/tab.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/http/namespaces/tree.py` & `MindsDB-23.7.4.0/mindsdb/api/http/namespaces/tree.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/http/namespaces/util.py` & `MindsDB-23.7.4.0/mindsdb/api/http/namespaces/util.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/http/namespaces/views.py` & `MindsDB-23.7.4.0/mindsdb/api/http/namespaces/views.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/http/start.py` & `MindsDB-23.7.4.0/mindsdb/api/http/start.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/http/utils.py` & `MindsDB-23.7.4.0/mindsdb/api/http/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mongo/classes/query_sql.py` & `MindsDB-23.7.4.0/mindsdb/api/mongo/classes/query_sql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mongo/classes/responder.py` & `MindsDB-23.7.4.0/mindsdb/api/mongo/classes/responder.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mongo/classes/responder_collection.py` & `MindsDB-23.7.4.0/mindsdb/api/mongo/classes/responder_collection.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mongo/classes/scram.py` & `MindsDB-23.7.4.0/mindsdb/api/mongo/classes/scram.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mongo/classes/session.py` & `MindsDB-23.7.4.0/mindsdb/api/mongo/classes/session.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mongo/responders/__init__.py` & `MindsDB-23.7.4.0/mindsdb/api/mongo/responders/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mongo/responders/aggregate.py` & `MindsDB-23.7.4.0/mindsdb/api/mongo/responders/aggregate.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mongo/responders/coll_stats.py` & `MindsDB-23.7.4.0/mindsdb/api/mongo/responders/coll_stats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mongo/responders/company_id.py` & `MindsDB-23.7.4.0/mindsdb/api/mongo/responders/company_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mongo/responders/connection_status.py` & `MindsDB-23.7.4.0/mindsdb/api/mongo/responders/connection_status.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mongo/responders/db_stats.py` & `MindsDB-23.7.4.0/mindsdb/api/mongo/responders/db_stats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mongo/responders/delete.py` & `MindsDB-23.7.4.0/mindsdb/api/mongo/responders/delete.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mongo/responders/find.py` & `MindsDB-23.7.4.0/mindsdb/api/mongo/responders/find.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mongo/responders/get_parameter.py` & `MindsDB-23.7.4.0/mindsdb/api/mongo/responders/get_parameter.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mongo/responders/host_info.py` & `MindsDB-23.7.4.0/mindsdb/api/mongo/responders/host_info.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mongo/responders/insert.py` & `MindsDB-23.7.4.0/mindsdb/api/mongo/responders/insert.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mongo/responders/list_collections.py` & `MindsDB-23.7.4.0/mindsdb/api/mongo/responders/list_collections.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mongo/responders/list_databases.py` & `MindsDB-23.7.4.0/mindsdb/api/mongo/responders/list_databases.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mongo/responders/list_indexes.py` & `MindsDB-23.7.4.0/mindsdb/api/mongo/responders/list_indexes.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mongo/responders/sasl_continue.py` & `MindsDB-23.7.4.0/mindsdb/api/mongo/responders/sasl_continue.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mongo/responders/sasl_start.py` & `MindsDB-23.7.4.0/mindsdb/api/mongo/responders/sasl_start.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mongo/server.py` & `MindsDB-23.7.4.0/mindsdb/api/mongo/server.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mongo/utilities/mongodb_ast.py` & `MindsDB-23.7.4.0/mindsdb/api/mongo/utilities/mongodb_ast.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mongo/utilities/mongodb_parser.py` & `MindsDB-23.7.4.0/mindsdb/api/mongo/utilities/mongodb_parser.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mongo/utilities/mongodb_query.py` & `MindsDB-23.7.4.0/mindsdb/api/mongo/utilities/mongodb_query.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/executor/data_types.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/executor/data_types.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/executor/executor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/utilities/functions.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/utilities/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/mysql/mysql_proxy/utilities/sql.py` & `MindsDB-23.7.4.0/mindsdb/api/mysql/mysql_proxy/utilities/sql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/nlp/nlp.py` & `MindsDB-23.7.4.0/mindsdb/api/nlp/nlp.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/postgres/postgres_proxy/executor/executor.py` & `MindsDB-23.7.4.0/mindsdb/api/postgres/postgres_proxy/executor/executor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py` & `MindsDB-23.7.4.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py` & `MindsDB-23.7.4.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py` & `MindsDB-23.7.4.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py` & `MindsDB-23.7.4.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py` & `MindsDB-23.7.4.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py` & `MindsDB-23.7.4.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py` & `MindsDB-23.7.4.0/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/access_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/access_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/access_handler/access_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/access_handler/access_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/access_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/access_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/airtable_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/airtable_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/airtable_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/airtable_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/altibase_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/altibase_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/altibase_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/altibase_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/aurora_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/aurora_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/aurora_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/aurora_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/autokeras_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/autokeras_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/autokeras_handler/setup.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/autokeras_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/autosklearn_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/autosklearn_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/autosklearn_handler/config.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/autosklearn_handler/config.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/autosklearn_handler/setup.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/autosklearn_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/bigquery_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/bigquery_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/bigquery_handler/logo.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/bigquery_handler/logo.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/binance_handler/binance_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/binance_handler/binance_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/binance_handler/binance_tables.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/binance_handler/binance_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/binance_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/binance_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/byom_handler/byom_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/byom_handler/byom_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/cassandra_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/cassandra_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/cassandra_handler/logo.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/cassandra_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/ckan_handler/logo.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/ckan_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/clickhouse_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/clickhouse_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/cloud_sql_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/cloud_sql_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/cohere_handler/cohere_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/cohere_handler/cohere_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/cohere_handler/setup.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/cohere_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/confluence_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/confluence_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/confluence_handler/confluence_table.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/confluence_handler/confluence_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/confluence_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/confluence_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/couchbase_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/couchbase_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/couchbase_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/couchbase_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/crate_handler/crate_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/crate_handler/crate_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/crate_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/crate_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/d0lt_handler/create-db.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/d0lt_handler/create-db.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/d0lt_handler/create-predictor.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/d0lt_handler/create-predictor.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/d0lt_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/d0lt_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/d0lt_handler/predict-target.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/d0lt_handler/predict-target.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/databend_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/databend_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/databend_handler/databend_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/databend_handler/databend_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/databend_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/databend_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/databricks_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/databricks_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/databricks_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/databricks_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/datastax_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/datastax_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/datastax_handler/logo.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/datastax_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/db2_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/db2_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/db2_handler/db2_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/db2_handler/db2_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/db2_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/db2_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/derby_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/derby_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/derby_handler/derby_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/derby_handler/derby_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/derby_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/derby_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/dremio_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/dremio_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
         headers = {
             'Content-Type': 'application/json',
         }
 
         data = '{' + f'"userName": "{self.connection_data["username"]}","password": "{self.connection_data["password"]}"' + '}'
 
-        response = requests.post(self.base_url + '/apiv2/login', headers=headers, data=data, verify=False)
+        response = requests.post(self.base_url + '/apiv2/login', headers=headers, data=data)
 
         return {
             'Authorization': '_dremio' + response.json()['token'],
             'Content-Type': 'application/json',
         }
 
     def disconnect(self):
@@ -231,8 +231,8 @@
 )
 
 connection_args_example = OrderedDict(
     host='localhost',
     database=9047,
     username='admin',
     password='password'
-)
+)
```

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/dremio_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/dremio_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/druid_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/druid_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/druid_handler/druid_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/druid_handler/druid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/druid_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/druid_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/duckdb_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/duckdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/duckdb_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/duckdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/dynamodb_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/dynamodb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/dynamodb_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/dynamodb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/elasticsearch_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/elasticsearch_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/empress_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/empress_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/empress_handler/empress_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/empress_handler/empress_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/empress_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/empress_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/file_handler/file_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/file_handler/file_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import os
 import csv
 import json
 import codecs
 import traceback
 import tempfile
 from urllib.parse import urlparse
+from pathlib import Path
 
-       
 import magic
 import requests
 import pandas as pd
 from charset_normalizer import from_bytes
 
 from mindsdb_sql import parse_sql
 from mindsdb_sql.parser.ast.base import ASTNode
@@ -137,118 +137,143 @@
             file_list_data = file_data
 
         header = [x.strip() for x in header]
         col_map = dict((col, col) for col in header)
         return pd.DataFrame(file_list_data, columns=header), col_map
 
     @staticmethod
+    def is_it_parquet(data: BytesIO) -> bool:
+        # Check first and last 4 bytes equal to PAR1.
+        # Refer: https://parquet.apache.org/docs/file-format/
+        parquet_sig = b'PAR1'
+        data.seek(0, 0)
+        start_meta = data.read(4)
+        data.seek(-4, 2)
+        end_meta = data.read()
+        data.seek(0)
+        if start_meta == parquet_sig and end_meta == parquet_sig:
+            return True
+        return False
+
+    @staticmethod
+    def is_it_xlsx(file_path: str) -> bool:
+        file_type = magic.from_file(file_path, mime=True)
+        if file_type in ['application/vnd.openxmlformats-officedocument.spreadsheetml.sheet', 'application/vnd.ms-excel']:
+            return True
+        return False
+
+    @staticmethod
+    def is_it_json(data_str: StringIO) -> bool:
+        # see if its JSON
+        text = data_str.read(100).strip()
+        data_str.seek(0)
+        if len(text) > 0:
+            # it it looks like a json, then try to parse it
+            if text.startswith('{') or text.startswith('['):
+                try:
+                    json.loads(data_str.read())
+                    return True
+                except Exception:
+                    return False
+                finally:
+                    data_str.seek(0)
+        return False
+
+    @staticmethod
+    def is_it_csv(data_str: StringIO) -> bool:
+        sample = data_str.readline()  # trying to get dialect from header
+        data_str.seek(0)
+        try:
+            csv.Sniffer().sniff(sample)
+            return True
+        except Exception:
+            return False
+
+    @staticmethod
     def _get_data_io(file_path):
         """
         @TODO: Use python-magic to simplify the function and detect the file types as the xlsx example
         This gets a file either url or local file and defines what the format is as well as dialect
         :param file: file path or url
         :return: data_io, format, dialect
         """
 
-        ############
-        # get file as io object
-        ############
-
-        # file_path = self._get_file_path()
-
         data = BytesIO()
+        data_str = None
+        dialect = None
 
         try:
             with open(file_path, 'rb') as fp:
                 data = BytesIO(fp.read())
         except Exception as e:
             error = 'Could not load file, possible exception : {exception}'.format(exception=e)
             print(error)
             raise ValueError(error)
 
-        dialect = None
-
-        ############
-        # check for file type
-        ############
+        suffix = Path(file_path).suffix.strip('.').lower()
+        if suffix not in ('csv', 'json', 'xlsx', 'parquet'):
+            if FileHandler.is_it_parquet(data):
+                suffix = 'parquet'
+            elif FileHandler.is_it_xlsx(file_path):
+                suffix = 'xlsx'
 
-        # Check first and last 4 bytes equal to PAR1.
-        # Refer: https://parquet.apache.org/docs/file-format/
-        parquet_sig = b'PAR1'
-        data.seek(0, 0)
-        start_meta = data.read(4)
-        data.seek(-4, 2)
-        end_meta = data.read()
-        data.seek(0)
-        if start_meta == parquet_sig and end_meta == parquet_sig:
-            return data, 'parquet', None
-        else:
-            print("It's not parquet file. Checking for other formats")
+        if suffix == 'parquet':
+            return data, 'parquet', dialect
 
-        file_type = magic.from_file(file_path, mime=True)
-        if file_type in ['application/vnd.openxmlformats-officedocument.spreadsheetml.sheet', 'application/vnd.ms-excel']:
-            #for now we send xlsx for all excel types since we use pd.read_excel
+        if suffix == 'xlsx':
             return data, 'xlsx', dialect
-       
-        # if not excel it can be a json file or a CSV, convert from binary to stringio
 
         byte_str = data.read()
         # Move it to StringIO
         try:
             # Handle Microsoft's BOM "special" UTF-8 encoding
             if byte_str.startswith(codecs.BOM_UTF8):
-                data = StringIO(byte_str.decode('utf-8-sig'))
+                data_str = StringIO(byte_str.decode('utf-8-sig'))
             else:
                 file_encoding_meta = from_bytes(
                     byte_str[:32 * 1024],
                     steps=32,           # Number of steps/block to extract from my_byte_str
                     chunk_size=1024,    # Set block size of each extraction)
                     explain=False
                 )
                 best_meta = file_encoding_meta.best()
                 errors = 'strict'
                 if best_meta is not None:
                     encoding = file_encoding_meta.best().encoding
                 else:
                     encoding = 'utf-8'
                     errors = 'replace'
-                data = StringIO(byte_str.decode(encoding, errors))
+                data_str = StringIO(byte_str.decode(encoding, errors))
         except Exception:
             print(traceback.format_exc())
             print('Could not load into string')
 
-        # see if its JSON
-        buffer = data.read(100)
+        if suffix not in ('csv', 'json'):
+            if FileHandler.is_it_json(data_str):
+                suffix = 'json'
+            elif FileHandler.is_it_csv(data_str):
+                suffix = 'csv'
+
+        if suffix == 'json':
+            return data_str, suffix, dialect
+
+        if suffix == 'csv':
+            try:
+                dialect = FileHandler._get_csv_dialect(data_str)
+                if dialect:
+                    return data_str, 'csv', dialect
+            except Exception:
+                print('Could not detect format for this file')
+                print(traceback.format_exc())
+
+        data_str.seek(0)
         data.seek(0)
-        text = buffer.strip()
-        # analyze first n characters
-        if len(text) > 0:
-            text = text.strip()
-            # it it looks like a json, then try to parse it
-            if text.startswith('{') or text.startswith('['):
-                try:
-                    json.loads(data.read())
-                    data.seek(0)
-                    return data, 'json', dialect
-                except Exception:
-                    data.seek(0)
-                    return data, None, dialect
 
-        # lets try to figure out if its a csv
-        try:
-            dialect = FileHandler._get_csv_dialect(data)
-            if dialect:
-                return data, 'csv', dialect
-            return data, None, dialect
-        except Exception:
-            data.seek(0)
-            print('Could not detect format for this file')
-            print(traceback.format_exc())
-            # No file type identified
-            return data, None, dialect
+        # No file type identified
+        return data, None, dialect
 
     @staticmethod
     def _get_file_path(path) -> str:
         try:
             is_url = urlparse(path).scheme in ('http', 'https')
         except Exception:
             is_url = False
@@ -260,16 +285,22 @@
     def _get_csv_dialect(buffer) -> csv.Dialect:
         sample = buffer.readline()  # trying to get dialect from header
         buffer.seek(0)
         try:
             if isinstance(sample, bytes):
                 sample = sample.decode()
             accepted_csv_delimiters = [',', '\t', ';']
-            dialect = csv.Sniffer().sniff(sample, delimiters=accepted_csv_delimiters)
-            dialect.doublequote = True  # assume that all csvs have " as string escape
+            try:
+                dialect = csv.Sniffer().sniff(sample, delimiters=accepted_csv_delimiters)
+                dialect.doublequote = True  # assume that all csvs have " as string escape
+            except Exception:
+                dialect = csv.reader(sample).dialect
+                if dialect.delimiter not in accepted_csv_delimiters:
+                    raise Exception(f"CSV delimeter '{dialect.delimiter}' is not supported")
+
         except csv.Error:
             dialect = None
         return dialect
 
     @staticmethod
     def _fetch_url(url: str) -> str:
         temp_dir = tempfile.mkdtemp(prefix='mindsdb_file_url_')
```

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/firebird_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/firebird_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/firebird_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/firebird_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/flaml_handler/flaml_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/flaml_handler/flaml_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/flaml_handler/setup.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/flaml_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/frappe_handler/frappe_client.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/frappe_handler/frappe_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/frappe_handler/frappe_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/frappe_handler/frappe_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/frappe_handler/frappe_tables.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/frappe_handler/frappe_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/frappe_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/frappe_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/github_handler/github_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/github_handler/github_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/github_handler/github_tables.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/github_handler/github_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/github_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/github_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/gitlab_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/gitlab_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/gmail_handler/gmail_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/gmail_handler/gmail_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/gmail_handler/tests/test_gmail_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/gmail_handler/tests/test_gmail_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_books_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_books_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_calendar_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_calendar_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_calendar_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_calendar_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_content_shopping_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_fit_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_fit_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_search_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_search_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_search_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_search_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/hackernews_handler/hn_table.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/hackernews_handler/hn_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/hackernews_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/hackernews_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/hana_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/hana_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/hana_handler/hana_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/hana_handler/hana_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/hana_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/hana_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/hive_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/hive_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/hive_handler/hive_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/hive_handler/hive_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/hive_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/hive_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/hsqldb_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/hsqldb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/hsqldb_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/hsqldb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/huggingface_api_handler/setup.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/huggingface_api_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/huggingface_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/huggingface_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/huggingface_handler/setup.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/huggingface_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/ignite_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/ignite_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/ignite_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/ignite_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/impala_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/impala_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/impala_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/impala_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/impala_handler/impala_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/impala_handler/impala_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/influxdb_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/influxdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/influxdb_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/influxdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/informix_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/informix_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/informix_handler/informix_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/informix_handler/informix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/ingres_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/ingres_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/ingres_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/ingres_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/jira_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/jira_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/jira_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/jira_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/jira_handler/jira_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/jira_handler/jira_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/jira_handler/jira_table.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/jira_handler/jira_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,55 +4,60 @@
 
 import numpy as np
 import pandas as pd
 
 from langchain.schema import SystemMessage
 from langchain.agents import AgentType
 from langchain.llms import OpenAI
-from langchain.chat_models import ChatOpenAI  # GPT-4 fails to follow the output langchain requires, avoid using for now
+from langchain.chat_models import ChatAnthropic, ChatOpenAI  # GPT-4 fails to follow the output langchain requires, avoid using for now
 from langchain.agents import initialize_agent, load_tools, Tool, create_sql_agent
 from langchain.prompts import PromptTemplate
 from langchain.utilities import GoogleSerperAPIWrapper
 from langchain.agents.agent_toolkits import SQLDatabaseToolkit
 from langchain.chains.conversation.memory import ConversationSummaryBufferMemory
 
-from mindsdb.integrations.handlers.openai_handler.openai_handler import OpenAIHandler, CHAT_MODELS
+from mindsdb.integrations.handlers.openai_handler.openai_handler import CHAT_MODELS as OPEN_AI_CHAT_MODELS
 from mindsdb.integrations.handlers.langchain_handler.mindsdb_database_agent import MindsDBSQL
+from mindsdb.integrations.libs.base import BaseMLEngine
+from mindsdb.integrations.utilities.handler_utils import get_api_key
 from mindsdb_sql import parse_sql, Insert
 
 
-_DEFAULT_MODEL = 'gpt-3.5-turbo'  # TODO: enable other LLM backends (AI21, Anthropic, etc.)
+_DEFAULT_MODEL = 'gpt-3.5-turbo'
 _DEFAULT_MAX_TOKENS = 2048  # requires more than vanilla OpenAI due to ongoing summarization and 3rd party input
 _DEFAULT_AGENT_MODEL = 'zero-shot-react-description'
 _DEFAULT_AGENT_TOOLS = ['python_repl', 'wikipedia']  # these require no additional arguments
+_ANTHROPIC_CHAT_MODELS = {'claude-2', 'claude-instant-1'}
+_PARSING_ERROR_PREFIX = 'Could not parse LLM output: `'
 
-
-class LangChainHandler(OpenAIHandler):
+class LangChainHandler(BaseMLEngine):
     """
     This is a MindsDB integration for the LangChain library, which provides a unified interface for interacting with
     various large language models (LLMs).
 
-    Currently, this integration supports exposing OpenAI's LLMs with normal text completion support. They are then
+    Currently, this integration supports exposing OpenAI and Anthrophic's LLMs with normal text completion support. They are then
     wrapped in a zero shot react description agent that offers a few third party tools out of the box, with support
     for additional ones if an API key is provided. Ongoing memory is also provided.
 
     Full tool support list:
         - wikipedia
         - python_repl
         - serper.dev search
-
-    This integration inherits from the OpenAI engine, so it shares a lot of the requirements, features (e.g. prompt
-    templating) and limitations.
     """
     name = 'langchain'
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.generative = True
         self.stops = []
+        self.default_mode = 'default'  # can also be 'conversational' or 'conversational-full'
+        self.engine_to_supported_modes = {
+            'openai': ['default', 'conversational', 'conversational-full', 'image'],
+            'anthropic': ['default', 'conversational', 'conversational-full']
+        }
         self.default_model = _DEFAULT_MODEL
         self.default_max_tokens = _DEFAULT_MAX_TOKENS
         self.default_agent_model = _DEFAULT_AGENT_MODEL
         self.default_agent_tools = _DEFAULT_AGENT_TOOLS
         self.write_privileges = False  # if True, this agent is able to write into other active mindsdb integrations
 
     def _get_serper_api_key(self, args, strict=True):
@@ -70,15 +75,34 @@
         if strict:
             raise Exception(f'Missing API key serper_api_key. Either re-create this ML_ENGINE specifying the `serper_api_key` parameter,\
                  or re-create this model and pass the API key with `USING` syntax.')  # noqa
 
     def create(self, target, args=None, **kwargs):
         self.write_privileges = args.get('using', {}).get('writer', self.write_privileges)
         self.default_agent_tools = args.get('tools', self.default_agent_tools)
-        super().create(target, args, **kwargs)
+
+        args = args['using']
+        args['target'] = target
+        
+        available_models = {*OPEN_AI_CHAT_MODELS, *_ANTHROPIC_CHAT_MODELS}
+        if not args.get('model_name'):
+            args['model_name'] = self.default_model
+        elif args['model_name'] not in available_models:
+            raise Exception(f"Invalid model name. Please use one of {available_models}")
+
+        if not args.get('mode'):
+            args['mode'] = self.default_mode
+
+        supported_modes = self.engine_to_supported_modes['openai']
+        if args['model_name'] in _ANTHROPIC_CHAT_MODELS:
+            supported_modes = self.engine_to_supported_modes['anthropic']
+        if args['mode'] not in supported_modes:
+            raise Exception(f"Invalid operation mode. Please use one of {supported_modes}")
+
+        self.model_storage.json_set('args', args)
 
     @staticmethod
     def create_validation(target, args=None, **kwargs):
         if 'using' not in args:
             raise Exception("LangChain engine requires a USING clause! Refer to its documentation for more details.")
         else:
             args = args['using']
@@ -118,77 +142,104 @@
         if args.get('mode') == 'conversational':
             agent_creation_method = 'conversational_completion'
 
         # input dataframe can be modified
         agent, df = getattr(self, agent_creation_method)(df, args, pred_args)
         return self.run_agent(df, agent, args, pred_args)
 
-    def conversational_completion(self, df, args=None, pred_args=None):
-        pred_args = pred_args if pred_args else {}
-
-        # api argument validation
+    def _get_chat_model_params(self, args, pred_args):
         model_name = args.get('model_name', self.default_model)
+        # Params shared by all models.
+        temperature = min(1.0, max(0.0, args.get('temperature', 0.0)))
+        max_tokens = pred_args.get('max_tokens', args.get('max_tokens', self.default_max_tokens))
+        top_p = pred_args.get('top_p', None)
+        timeout = pred_args.get('request_timeout', None)
+        serper_api_key = self._get_serper_api_key(args, strict=False)
+        model_kwargs = {}
+        if model_name in _ANTHROPIC_CHAT_MODELS:
+            model_kwargs['model'] = model_name
+            model_kwargs['temperature'] = temperature
+            model_kwargs['max_tokens_to_sample'] = max_tokens
+            model_kwargs['top_p'] = top_p
+            model_kwargs['timeout'] = timeout
+            model_kwargs['stop_sequences'] = pred_args.get('stop_sequences', None)
+            model_kwargs['serper_api_key'] = serper_api_key
+            model_kwargs['anthropic_api_key'] = get_api_key('anthropic', args, self.engine_storage)
+        else:
+            # OpenAI
+            model_kwargs['model_name'] = model_name
+            model_kwargs['temperature'] = temperature
+            model_kwargs['max_tokens'] = max_tokens
+            model_kwargs['top_p'] = top_p
+            model_kwargs['request_timeout'] = timeout
+            model_kwargs['serper_api_key'] = serper_api_key
+            model_kwargs['frequency_penalty'] = pred_args.get('frequency_penalty', None)
+            model_kwargs['presence_penalty'] = pred_args.get('presence_penalty', None)
+            model_kwargs['n'] = pred_args.get('n', None)
+            model_kwargs['best_of'] = pred_args.get('best_of', None)
+            model_kwargs['logit_bias'] = pred_args.get('logit_bias', None)
+            model_kwargs['openai_api_key'] = get_api_key('openai', args, self.engine_storage)
 
-        model_kwargs = {
-            'model_name': model_name,
-            'temperature': min(1.0, max(0.0, args.get('temperature', 0.0))),
-            'max_tokens': pred_args.get('max_tokens', args.get('max_tokens', self.default_max_tokens)),
-            'top_p': pred_args.get('top_p', None),
-            'frequency_penalty': pred_args.get('frequency_penalty', None),
-            'presence_penalty': pred_args.get('presence_penalty', None),
-            'n': pred_args.get('n', None),
-            'best_of': pred_args.get('best_of', None),
-            'request_timeout': pred_args.get('request_timeout', None),
-            'logit_bias': pred_args.get('logit_bias', None),
-            'openai_api_key': self._get_openai_api_key(args, strict=True),
-            'serper_api_key': self._get_serper_api_key(args, strict=False),
-        }
         model_kwargs = {k: v for k, v in model_kwargs.items() if v is not None}  # filter out None values
+        return model_kwargs
+
+    def _create_chat_model(self, args, pred_args):
+        model_kwargs = self._get_chat_model_params(args, pred_args)
+        model_name = args.get('model_name', self.default_model)
+
+        if model_name in _ANTHROPIC_CHAT_MODELS:
+            return ChatAnthropic(**model_kwargs)
+        elif model_name in OPEN_AI_CHAT_MODELS:
+            return ChatOpenAI(**model_kwargs)
+        else:
+            return OpenAI(**model_kwargs)
+
+
+    def conversational_completion(self, df, args=None, pred_args=None):
+        pred_args = pred_args if pred_args else {}
 
         # langchain tool setup
+        model_kwargs = self._get_chat_model_params(args, pred_args)
         tools = self._setup_tools(model_kwargs, pred_args, args['executor'])
 
-        llm = ChatOpenAI(**model_kwargs)
-
+        max_tokens = pred_args.get('max_tokens', args.get('max_tokens', self.default_max_tokens))
+        llm = self._create_chat_model(args, pred_args)
         memory = ConversationSummaryBufferMemory(llm=llm,
-                                                 max_token_limit=model_kwargs.get('max_tokens', None),
+                                                 max_token_limit=max_tokens,
                                                  memory_key="chat_history")
 
         # fill memory
 
         # system prompt
         prompt = args['prompt']
-        if 'prompt' in pred_args:
+        if 'prompt' in pred_args and pred_args['prompt'] is not None:
             prompt = pred_args['prompt']
         if 'context' in pred_args:
             prompt += '\n\n' + 'Useful information:\n' + pred_args['context'] + '\n'
         memory.chat_memory.messages.insert(0, SystemMessage(content=prompt))
 
         # user - assistant conversation. get all except the last message
         for row in df[:-1].to_dict('records'):
             question = row[args['user_column']]
             answer = row[args['assistant_column']]
 
-            if question:
-                memory.chat_memory.add_user_message(question)
-            if answer:
-                memory.chat_memory.add_ai_message(answer)
+            memory.save_context({"input": question}, {"output": answer})
 
         # use last message as prompt, remove other questions
         df.iloc[:-1, df.columns.get_loc('question')] = ''
 
         agent_name = AgentType.CONVERSATIONAL_REACT_DESCRIPTION
         agent = initialize_agent(
             tools,
             llm,
             memory=memory,
             agent=agent_name,
             max_iterations=pred_args.get('max_iterations', 3),
             verbose=pred_args.get('verbose', args.get('verbose', False)),
-            handle_parsing_errors=True,
+            handle_parsing_errors=False,
         )
 
         # setup model description
         description = {
             'allowed_tools': [agent.agent.allowed_tools],  # packed as list to avoid additional rows
             'agent_type': agent_name,
             'max_iterations': agent.max_iterations,
@@ -208,53 +259,33 @@
             - setup the langchain agent (memory included)
             - setup information to be published when describing the model
 
         Ref link from the LangChain documentation on how to accomplish the first two items:
             - python.langchain.com/en/latest/modules/agents/agents/custom_agent.html
         """
         pred_args = pred_args if pred_args else {}
-
-        # api argument validation
-        model_name = pred_args.get('model_name', args.get('model_name', self.default_model))
-        agent_name = pred_args.get('agent_name', args.get('agent_name', self.default_agent_model))
-
-        model_kwargs = {
-            'model_name': model_name,
-            'temperature': min(1.0, max(0.0, pred_args.get('temperature', args.get('temperature', 0.0)))),
-            'max_tokens': pred_args.get('max_tokens', args.get('max_tokens', self.default_max_tokens)),
-            'top_p': pred_args.get('top_p', None),
-            'frequency_penalty': pred_args.get('frequency_penalty', None),
-            'presence_penalty': pred_args.get('presence_penalty', None),
-            'n': pred_args.get('n', None),
-            'best_of': pred_args.get('best_of', None),
-            'request_timeout': pred_args.get('request_timeout', None),
-            'logit_bias': pred_args.get('logit_bias', None),
-            'openai_api_key': self._get_openai_api_key(args, strict=True),
-            'serper_api_key': self._get_serper_api_key(args, strict=False),
-        }
-        model_kwargs = {k: v for k, v in model_kwargs.items() if v is not None}  # filter out None values
+        pred_args['tools'] = args.get('tools') if 'tools' not in pred_args else pred_args.get('tools', [])
 
         # langchain tool setup
-        pred_args['tools'] = args.get('tools') if 'tools' not in pred_args else pred_args.get('tools', [])
+        model_kwargs = self._get_chat_model_params(args, pred_args)
         tools = self._setup_tools(model_kwargs, pred_args, args['executor'])
 
         # langchain agent setup
-        if model_kwargs['model_name'] in CHAT_MODELS:
-            llm = ChatOpenAI(**model_kwargs)
-        else:
-            llm = OpenAI(**model_kwargs)
-        memory = ConversationSummaryBufferMemory(llm=llm, max_token_limit=model_kwargs.get('max_tokens', None))
+        llm = self._create_chat_model(args, pred_args)
+        max_tokens = pred_args.get('max_tokens', args.get('max_tokens', self.default_max_tokens))
+        memory = ConversationSummaryBufferMemory(llm=llm, max_token_limit=max_tokens)
+        agent_name = pred_args.get('agent_name', args.get('agent_name', self.default_agent_model))
         agent = initialize_agent(
             tools,
             llm,
             memory=memory,
             agent=agent_name,
             max_iterations=pred_args.get('max_iterations', 3),
             verbose=pred_args.get('verbose', args.get('verbose', False)),
-            handle_parsing_errors=True,
+            handle_parsing_errors=False,
         )
 
         # setup model description
         description = {
             'allowed_tools': [agent.agent.allowed_tools],   # packed as list to avoid additional rows
             'agent_type': agent_name,
             'max_iterations': agent.max_iterations,
@@ -301,14 +332,28 @@
             for prompt in prompts:
                 if not prompt:
                     # skip empty values
                     completions.append('')
                     continue
                 try:
                     completions.append(agent.run(prompt))
+                except ValueError as e:
+                    # Handle parsing errors ourselves instead of using handle_parsing_errors=True in initialize_agent.
+                    response = str(e)
+                    if not response.startswith(_PARSING_ERROR_PREFIX):
+                        completions.append(f'agent failed with error:\n{str(e)[:50]}...')
+                    else:
+                        # By far the most common error is a Langchain parsing error. Some OpenAI models
+                        # always output a response formatted correctly. Anthropic, and others, sometimes just output
+                        # the answer as text (when not using tools), even when prompted to output in a specific format.
+                        # As a somewhat dirty workaround, we accept the output formatted incorrectly and use it as a response.
+                        #
+                        # Ideally, in the future, we would write a parser that is more robust and flexible than the one Langchain uses.
+                        response = response.removeprefix(_PARSING_ERROR_PREFIX).removesuffix('`')
+                        completions.append(response)
                 except Exception as e:
                     completions.append(f'agent failed with error:\n{str(e)[:50]}...')
             return [c for c in completions]
 
         completion = _completion(agent, prompts)
 
         # add null completion for empty prompts
@@ -321,15 +366,16 @@
 
     def _setup_tools(self, model_kwargs, pred_args, executor):
         def _mdb_exec_call(query: str) -> str:
             """ We define it like this to pass the executor through the closure, as custom classes don't allow custom field assignment. """  # noqa
             try:
                 ast_query = parse_sql(query.strip('`'), dialect='mindsdb')
                 ret = executor.execute_command(ast_query)
-
+                if ret.data is None and ret.error_code is None:
+                    return ''
                 data = ret.data  # list of lists
                 data = '\n'.join([  # rows
                     '\t'.join(      # columns
                         str(row) if isinstance(row, str) else [str(value) for value in row]
                     ) for row in data
                 ])
             except Exception as e:
@@ -457,14 +503,14 @@
         raise NotImplementedError('Fine-tuning is not supported for LangChain models')
 
     def sql_agent_completion(self, df, args=None, pred_args=None):
         """This completion will be used to answer based on information passed by any MindsDB DB or API engine."""
         db = MindsDBSQL(engine=args['executor'], metadata=args['executor'].session.integration_controller)
         toolkit = SQLDatabaseToolkit(db=db)
         model_name = args.get('model_name', self.default_model)
-        llm = OpenAI(temperature=0) if model_name not in CHAT_MODELS else ChatOpenAI(temperature=0)
+        llm = OpenAI(temperature=0) if model_name not in OPEN_AI_CHAT_MODELS else ChatOpenAI(temperature=0)
         agent = create_sql_agent(
             llm=llm,
             toolkit=toolkit,
             verbose=True
         )
         return agent, df
```

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/langchain_handler/setup.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/langchain_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/lightfm_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/lightfm_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/lightfm_handler/helpers.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/lightfm_handler/helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/lightfm_handler/lightfm_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/lightfm_handler/lightfm_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/lightfm_handler/setup.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/lightfm_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/lightwood_handler/setup.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/lightwood_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/llama_index_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/llama_index_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/llama_index_handler/llama_index_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/llama_index_handler/llama_index_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/llama_index_handler/setup.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/llama_index_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/ludwig_handler/setup.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/ludwig_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/mariadb_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/mariadb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/materialize_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/materialize_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/matrixone_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/matrixone_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/matrixone_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/matrixone_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/maxdb_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/maxdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/maxdb_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/maxdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/mediawiki_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/mediawiki_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/mediawiki_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/mediawiki_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_tables.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/mediawiki_handler/mediawiki_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/mendeley_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/mendeley_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/mendeley_handler/mendeley_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/mendeley_handler/mendeley_tables.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/mendeley_handler/tests/test_mendeley_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/mendeley_handler/tests/test_mendeley_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/merlion_handler/adapters.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/merlion_handler/adapters.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/merlion_handler/setup.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/merlion_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/mlflow_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/mlflow_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/mlflow_handler/setup.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/mlflow_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/monetdb_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/monetdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/monetdb_handler/create-database.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/monetdb_handler/create-database.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/monetdb_handler/create-predictor.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/monetdb_handler/create-predictor.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/monetdb_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/monetdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/monetdb_handler/select-predictor.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/monetdb_handler/select-predictor.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/mongodb_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/mongodb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/monkeylearn_handler/monkeylearn_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/monkeylearn_handler/monkeylearn_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/monkeylearn_handler/setup.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/monkeylearn_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/mssql_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/mssql_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/mysql_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/mysql_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/mysql_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/mysql_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/neuralforecast_handler/setup.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/neuralforecast_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/newsapi_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/newsapi_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/newsapi_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/newsapi_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/oceanbase_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/oceanbase_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/openai_handler/helpers.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/openai_handler/helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/openai_handler/openai_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/openai_handler/openai_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 
 import openai
 import numpy as np
 import pandas as pd
 
 from mindsdb.utilities.hooks import before_openai_query, after_openai_query
 from mindsdb.utilities import log
-from mindsdb.utilities.config import Config
 from mindsdb.integrations.libs.base import BaseMLEngine
 from mindsdb.integrations.handlers.openai_handler.helpers import retry_with_exponential_backoff, \
     truncate_msgs_for_token_limit
+from mindsdb.integrations.utilities.handler_utils import get_api_key
 
 CHAT_MODELS = ('gpt-3.5-turbo', 'gpt-3.5-turbo-0301', 'gpt-4', 'gpt-4-0314', 'gpt-4-32k', 'gpt-4-32k-0314')
 
 
 class OpenAIHandler(BaseMLEngine):
     name = 'openai'
 
@@ -65,55 +65,28 @@
                         4) a `prompt' and 'user_column' and 'assistant_column`
                 '''))
 
     def create(self, target, args=None, **kwargs):
         args = args['using']
 
         args['target'] = target
-        available_models = [m.openai_id for m in openai.Model.list(api_key=self._get_openai_api_key(args)).data]
+        api_key = get_api_key('openai', args, self.engine_storage)
+        available_models = [m.openai_id for m in openai.Model.list(api_key=api_key).data]
         if not args.get('model_name'):
             args['model_name'] = self.default_model
         elif args['model_name'] not in available_models:
             raise Exception(f"Invalid model name. Please use one of {available_models}")
 
         if not args.get('mode'):
             args['mode'] = self.default_mode
         elif args['mode'] not in self.supported_modes:
             raise Exception(f"Invalid operation mode. Please use one of {self.supported_modes}")
 
         self.model_storage.json_set('args', args)
 
-    def _get_openai_api_key(self, args, strict=True):
-        """ 
-        API_KEY preference order:
-            1. provided at model creation
-            2. provided at engine creation
-            3. OPENAI_API_KEY env variable
-            4. openai.api_key setting in config.json
-        """  # noqa
-        # 1
-        if 'api_key' in args:
-            return args['api_key']
-        # 2
-        connection_args = self.engine_storage.get_connection_args()
-        if 'api_key' in connection_args:
-            return connection_args['api_key']
-        # 3
-        api_key = os.getenv('OPENAI_API_KEY')
-        if api_key is not None:
-            return api_key
-        # 4
-        config = Config()
-        openai_cfg = config.get('openai', {})
-        if 'api_key' in openai_cfg:
-            return openai_cfg['api_key']
-
-        if strict:
-            raise Exception(f'Missing API key "api_key". Either re-create this ML_ENGINE specifying the `api_key` parameter,\
-                 or re-create this model and pass the API key with `USING` syntax.')  # noqa
 
     def predict(self, df, args=None):
         """
         If there is a prompt template, we use it. Otherwise, we use the concatenation of `context_column` (optional) and `question_column` to ask for a completion.
         """ # noqa
         # TODO: support for edits, embeddings and moderation
 
@@ -228,15 +201,15 @@
             else:
                 empty_prompt_ids = np.where(df[[args['question_column']]].isna().all(axis=1).values)[0]
                 prompts = list(df[args['question_column']].apply(lambda x: str(x)))
 
         # remove prompts without signal from completion queue
         prompts = [j for i, j in enumerate(prompts) if i not in empty_prompt_ids]
 
-        api_key = self._get_openai_api_key(args)
+        api_key = get_api_key('openai', args, self.engine_storage)
         api_args = {k: v for k, v in api_args.items() if v is not None}  # filter out non-specified api args
         completion = self._completion(model_name, prompts, api_key, api_args, args, df)
 
         # add null completion for empty prompts
         for i in sorted(empty_prompt_ids):
             completion.insert(i, None)
 
@@ -448,15 +421,15 @@
         # TODO: Update to use update() artifacts
 
         args = self.model_storage.json_get('args')
 
         if attribute == 'args':
             return pd.DataFrame(args.items(), columns=['key', 'value'])
         elif attribute == 'metadata':
-            api_key = self._get_openai_api_key(args)
+            api_key = get_api_key('openai', args, self.engine_storage)
             model_name = args.get('model_name', self.default_model)
             meta = openai.Model.retrieve(model_name, api_key=api_key)
             return pd.DataFrame(meta.items(), columns=['key', 'value'])
         else:
             tables = ['args', 'metadata']
             return pd.DataFrame(tables, columns=['tables'])
 
@@ -486,15 +459,15 @@
 
         args = {**using_args, **args}
         prev_model_name = self.base_model_storage.json_get('args').get('model_name', '')
 
         if prev_model_name not in self.supported_ft_models:
             raise Exception(f"This model cannot be finetuned. Supported base models are {self.supported_ft_models}")
 
-        openai.api_key = self._get_openai_api_key(args)
+        openai.api_key = get_api_key('openai', args, self.engine_storage)
         finetune_time = datetime.datetime.now().strftime('%Y-%m-%d_%H-%M-%S')
 
         temp_storage_path = tempfile.mkdtemp()
         temp_file_name = f"ft_{finetune_time}"
         temp_model_storage_path = f"{temp_storage_path}/{temp_file_name}.jsonl"
         df.to_json(temp_model_storage_path, orient='records', lines=True)
```

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/openai_handler/setup.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/openai_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/opengauss_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/opengauss_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/oracle_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/oracle_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/oracle_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/oracle_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/orioledb_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/orioledb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/paypal_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/paypal_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/paypal_handler/paypal_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/paypal_handler/paypal_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/paypal_handler/paypal_tables.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/paypal_handler/paypal_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/phoenix_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/phoenix_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/phoenix_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/phoenix_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/pinot_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/pinot_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/pinot_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/pinot_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/plaid_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/plaid_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/planetscale_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/planetscale_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/planetscale_handler/create-db.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/planetscale_handler/create-db.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/planetscale_handler/create-predictor.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/planetscale_handler/create-predictor.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/planetscale_handler/drop-db.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/planetscale_handler/drop-db.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/planetscale_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/planetscale_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/planetscale_handler/predict-target.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/planetscale_handler/predict-target.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/popularity_recommender_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/popularity_recommender_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/popularity_recommender_handler/popularity_recommender_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/popularity_recommender_handler/popularity_recommender_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/popularity_recommender_handler/setup.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/popularity_recommender_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/postgres_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/postgres_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/postgres_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/postgres_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/questdb_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/questdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/quickbooks_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/quickbooks_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/quickbooks_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/quickbooks_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/ray_serve_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/ray_serve_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/ray_serve_handler/setup.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/ray_serve_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/realtime_slack_chat_handler/realtime_slack_chat_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/realtime_slack_chat_handler/realtime_slack_chat_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/reddit_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/reddit_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/redshift_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/redshift_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/redshift_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/redshift_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/rocket_chat_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/rocket_chat_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,15 @@
                 'count_col': 'msgs'
             },
             'chat_table': {
                 'name': 'direct_messages',
                 'chat_id_col': 'room_id',
                 'username_col': 'username',
                 'text_col': 'text',
+                'time_col': 'sent_at',
             }
         }
         return params
 
     def get_my_user_name(self):
         info = self.call_api('me')
         return info['username']
```

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_tables.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/rockset_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/rockset_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/rockset_handler/tests/test.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/rockset_handler/tests/test.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/rockset_handler/tests/test2.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/rockset_handler/tests/test2.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/s3_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/s3_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/s3_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/s3_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/s3_handler/s3_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/s3_handler/s3_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/scylla_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/scylla_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/scylla_handler/logo.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/scylla_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/sendinblue_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/sendinblue_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/sendinblue_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/sendinblue_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/sheets_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/sheets_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/sheets_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/sheets_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/shopify_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/shopify_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/shopify_handler/shopify_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/shopify_handler/shopify_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/shopify_handler/shopify_tables.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/shopify_handler/shopify_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/slack_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/slack_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/slack_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/slack_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/slack_handler/slack_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/slack_handler/slack_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/solr_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/solr_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/solr_handler/solr.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/solr_handler/solr.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/solr_handler/solr_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/solr_handler/solr_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqlany_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqlany_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqlany_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqlany_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqlite_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqlite_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqlite_handler/db_connection.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqlite_handler/db_connection.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqlite_handler/error.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqlite_handler/error.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqlite_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqlite_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqlite_handler/model_drop.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqlite_handler/model_drop.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqreamdb_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqreamdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/starrocks_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/starrocks_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/statsforecast_handler/setup.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/statsforecast_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/strava_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/strava_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/strava_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/strava_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/strava_handler/strava_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/strava_handler/strava_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/strava_handler/strava_tables.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/strava_handler/strava_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/stripe_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/stripe_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/stripe_handler/stripe_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/stripe_handler/stripe_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/stripe_handler/stripe_tables.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/stripe_handler/stripe_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/supabase_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/supabase_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/surrealdb_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/surrealdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/surrealdb_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/surrealdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/tdengine_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/tdengine_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/tdengine_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/tdengine_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/teradata_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/teradata_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/teradata_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/teradata_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/tidb_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/tidb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/timescaledb_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/timescaledb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/tpot_handler/setup.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/tpot_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/trino_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/trino_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/trino_handler/trino_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/trino_handler/trino_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/twitter_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/twitter_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/utilities/query_utilities/insert_query_utilities.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/utilities/query_utilities/insert_query_utilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/utilities/query_utilities/select_query_utilities.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/utilities/query_utilities/select_query_utilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/vertica_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/vertica_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/vertica_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/vertica_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/vitess_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/vitess_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/web_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/web_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/web_handler/urlcrawl_helpers.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/web_handler/urlcrawl_helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/web_handler/web_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/web_handler/web_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/writer_handler/ingest.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/writer_handler/ingest.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/writer_handler/question_answer.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/writer_handler/question_answer.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/writer_handler/settings.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/writer_handler/settings.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/writer_handler/setup.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/writer_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/writer_handler/writer_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/writer_handler/writer_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/youtube_handler/__init__.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/youtube_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/youtube_handler/icon.png` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/youtube_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/yugabyte_handler/icon.svg` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/yugabyte_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers_client/db_client_factory.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers_client/db_client_factory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers_client/db_grpc_client.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers_client/db_grpc_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers_client/ml_client_factory.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers_client/ml_client_factory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers_client/ml_grpc_client.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers_client/ml_grpc_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers_wrapper/db_handler_service.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers_wrapper/db_handler_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/handlers_wrapper/ml_handler_service.py` & `MindsDB-23.7.4.0/mindsdb/integrations/handlers_wrapper/ml_handler_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/libs/api_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/libs/api_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/libs/base.py` & `MindsDB-23.7.4.0/mindsdb/integrations/libs/base.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/libs/handler_helpers.py` & `MindsDB-23.7.4.0/mindsdb/integrations/libs/handler_helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/libs/learn_process.py` & `MindsDB-23.7.4.0/mindsdb/integrations/libs/learn_process.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/libs/ml_exec_base.py` & `MindsDB-23.7.4.0/mindsdb/integrations/libs/ml_exec_base.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/libs/ml_handler_proc.py` & `MindsDB-23.7.4.0/mindsdb/integrations/libs/ml_handler_proc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/libs/net_helpers.py` & `MindsDB-23.7.4.0/mindsdb/integrations/libs/net_helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/libs/realtime_chat_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/libs/realtime_chat_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/libs/response.py` & `MindsDB-23.7.4.0/mindsdb/integrations/libs/response.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/libs/storage_handler.py` & `MindsDB-23.7.4.0/mindsdb/integrations/libs/storage_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/utilities/date_utils.py` & `MindsDB-23.7.4.0/mindsdb/integrations/utilities/date_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/utilities/install.py` & `MindsDB-23.7.4.0/mindsdb/integrations/utilities/install.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/utilities/sql_utils.py` & `MindsDB-23.7.4.0/mindsdb/integrations/utilities/sql_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/utilities/test_utils.py` & `MindsDB-23.7.4.0/mindsdb/integrations/utilities/test_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/integrations/utilities/time_series_utils.py` & `MindsDB-23.7.4.0/mindsdb/integrations/utilities/time_series_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/interfaces/chatbot/chatbot_controller.py` & `MindsDB-23.7.4.0/mindsdb/interfaces/chatbot/chatbot_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/interfaces/chatbot/chatbot_message.py` & `MindsDB-23.7.4.0/mindsdb/interfaces/chatbot/chatbot_message.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/interfaces/chatbot/chatbot_monitor.py` & `MindsDB-23.7.4.0/mindsdb/interfaces/chatbot/chatbot_monitor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/interfaces/chatbot/chatbot_thread.py` & `MindsDB-23.7.4.0/mindsdb/interfaces/chatbot/chatbot_thread.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/interfaces/chatbot/realtime_chat_handler_factory.py` & `MindsDB-23.7.4.0/mindsdb/interfaces/chatbot/realtime_chat_handler_factory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/interfaces/chatbot/realtime_chatbot_task.py` & `MindsDB-23.7.4.0/mindsdb/interfaces/chatbot/realtime_chatbot_task.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/interfaces/chatbot/realtime_chatbot_thread.py` & `MindsDB-23.7.4.0/mindsdb/interfaces/chatbot/realtime_chatbot_thread.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/interfaces/database/database.py` & `MindsDB-23.7.4.0/mindsdb/interfaces/database/database.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/interfaces/database/integrations.py` & `MindsDB-23.7.4.0/mindsdb/interfaces/database/integrations.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/interfaces/database/projects.py` & `MindsDB-23.7.4.0/mindsdb/interfaces/database/projects.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/interfaces/database/views.py` & `MindsDB-23.7.4.0/mindsdb/interfaces/database/views.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/interfaces/file/file_controller.py` & `MindsDB-23.7.4.0/mindsdb/interfaces/file/file_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/interfaces/jobs/jobs_controller.py` & `MindsDB-23.7.4.0/mindsdb/interfaces/jobs/jobs_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/interfaces/jobs/scheduler.py` & `MindsDB-23.7.4.0/mindsdb/interfaces/jobs/scheduler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/interfaces/model/functions.py` & `MindsDB-23.7.4.0/mindsdb/interfaces/model/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/interfaces/model/model_controller.py` & `MindsDB-23.7.4.0/mindsdb/interfaces/model/model_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
                 data['accuracy'] = float(np.mean(list(data['accuracies'].values())))
         return data
 
     def get_reduced_model_data(self, name: str = None, predictor_record=None, ml_handler_name='lightwood') -> dict:
         full_model_data = self.get_model_data(name=name, predictor_record=predictor_record, ml_handler_name=ml_handler_name)
         reduced_model_data = {}
         for k in ['id', 'name', 'version', 'is_active', 'predict', 'status',
-                  'current_phase', 'accuracy', 'data_source', 'update', 'active',
+                  'problem_definition', 'current_phase', 'accuracy', 'data_source', 'update', 'active',
                   'mindsdb_version', 'error', 'created_at', 'fetch_data_query']:
             reduced_model_data[k] = full_model_data.get(k, None)
 
         reduced_model_data['training_time'] = None
         if full_model_data.get('training_start_at') is not None:
             if full_model_data.get('training_stop_at') is not None:
                 reduced_model_data['training_time'] = (
```

### Comparing `MindsDB-23.7.3.1/mindsdb/interfaces/storage/db.py` & `MindsDB-23.7.4.0/mindsdb/interfaces/storage/db.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/interfaces/storage/fs.py` & `MindsDB-23.7.4.0/mindsdb/interfaces/storage/fs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/interfaces/storage/json.py` & `MindsDB-23.7.4.0/mindsdb/interfaces/storage/json.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/interfaces/storage/model_fs.py` & `MindsDB-23.7.4.0/mindsdb/interfaces/storage/model_fs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/interfaces/stream/base/integration.py` & `MindsDB-23.7.4.0/mindsdb/interfaces/stream/base/integration.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/interfaces/stream/stream.py` & `MindsDB-23.7.4.0/mindsdb/interfaces/stream/stream.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/microservices_grpc/db/common_pb2.py` & `MindsDB-23.7.4.0/mindsdb/microservices_grpc/db/common_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/microservices_grpc/db/db_pb2.py` & `MindsDB-23.7.4.0/mindsdb/microservices_grpc/db/db_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/microservices_grpc/db/db_pb2_grpc.py` & `MindsDB-23.7.4.0/mindsdb/microservices_grpc/db/db_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/microservices_grpc/executor/executor_pb2.py` & `MindsDB-23.7.4.0/mindsdb/microservices_grpc/executor/executor_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py` & `MindsDB-23.7.4.0/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/microservices_grpc/ml/common_pb2.py` & `MindsDB-23.7.4.0/mindsdb/microservices_grpc/ml/common_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/microservices_grpc/ml/ml_pb2.py` & `MindsDB-23.7.4.0/mindsdb/microservices_grpc/ml/ml_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py` & `MindsDB-23.7.4.0/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/migrations/alembic.ini` & `MindsDB-23.7.4.0/mindsdb/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/migrations/env.py` & `MindsDB-23.7.4.0/mindsdb/migrations/env.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/migrations/migrate.py` & `MindsDB-23.7.4.0/mindsdb/migrations/migrate.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py` & `MindsDB-23.7.4.0/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py` & `MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py` & `MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py` & `MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py` & `MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py` & `MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py` & `MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py` & `MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py` & `MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py` & `MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py` & `MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py` & `MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py` & `MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py` & `MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py` & `MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py` & `MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py` & `MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py` & `MindsDB-23.7.4.0/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py` & `MindsDB-23.7.4.0/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py` & `MindsDB-23.7.4.0/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py` & `MindsDB-23.7.4.0/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py` & `MindsDB-23.7.4.0/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py` & `MindsDB-23.7.4.0/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/migrations/versions/2023-05-24_6d748f2c7b0b_remove_streams.py` & `MindsDB-23.7.4.0/mindsdb/migrations/versions/2023-05-24_6d748f2c7b0b_remove_streams.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/migrations/versions/2023-05-31_aaecd7012a78_chatbot.py` & `MindsDB-23.7.4.0/mindsdb/migrations/versions/2023-05-31_aaecd7012a78_chatbot.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/migrations/versions/2023-06-16_9d6271bb2c38_update_chat_bots_table.py` & `MindsDB-23.7.4.0/mindsdb/migrations/versions/2023-06-16_9d6271bb2c38_update_chat_bots_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/migrations/versions/2023-06-19_b5bf593ba659_create_chat_bots_history_table.py` & `MindsDB-23.7.4.0/mindsdb/migrations/versions/2023-06-19_b5bf593ba659_create_chat_bots_history_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/migrations/versions/2023-06-27_607709e1615b_update_project_names.py` & `MindsDB-23.7.4.0/mindsdb/migrations/versions/2023-06-27_607709e1615b_update_project_names.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/utilities/auth.py` & `MindsDB-23.7.4.0/mindsdb/utilities/auth.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/utilities/cache.py` & `MindsDB-23.7.4.0/mindsdb/utilities/cache.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/utilities/config.py` & `MindsDB-23.7.4.0/mindsdb/utilities/config.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/utilities/context.py` & `MindsDB-23.7.4.0/mindsdb/utilities/context.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/utilities/fs.py` & `MindsDB-23.7.4.0/mindsdb/utilities/fs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/utilities/functions.py` & `MindsDB-23.7.4.0/mindsdb/utilities/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/utilities/hooks/__init__.py` & `MindsDB-23.7.4.0/mindsdb/utilities/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/utilities/hooks/profiling.py` & `MindsDB-23.7.4.0/mindsdb/utilities/hooks/profiling.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/utilities/json_encoder.py` & `MindsDB-23.7.4.0/mindsdb/utilities/json_encoder.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/utilities/log.py` & `MindsDB-23.7.4.0/mindsdb/utilities/log.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/utilities/log_controller.py` & `MindsDB-23.7.4.0/mindsdb/utilities/log_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/utilities/profiler/profiler.py` & `MindsDB-23.7.4.0/mindsdb/utilities/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/utilities/ps.py` & `MindsDB-23.7.4.0/mindsdb/utilities/ps.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/utilities/telemetry.py` & `MindsDB-23.7.4.0/mindsdb/utilities/telemetry.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/mindsdb/utilities/wizards.py` & `MindsDB-23.7.4.0/mindsdb/utilities/wizards.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/requirements/requirements.txt` & `MindsDB-23.7.4.0/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `MindsDB-23.7.3.1/setup.py` & `MindsDB-23.7.4.0/setup.py`

 * *Files identical despite different names*

