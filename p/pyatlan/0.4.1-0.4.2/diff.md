# Comparing `tmp/pyatlan-0.4.1.tar.gz` & `tmp/pyatlan-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatlan-0.4.1.tar", last modified: Mon Jul 24 09:17:41 2023, max compression
+gzip compressed data, was "pyatlan-0.4.2.tar", last modified: Tue Jul 25 07:53:30 2023, max compression
```

## Comparing `pyatlan-0.4.1.tar` & `pyatlan-0.4.2.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:41.830475 pyatlan-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-07-24 09:17:30.000000 pyatlan-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-24 09:17:30.000000 pyatlan-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-24 09:17:30.000000 pyatlan-0.4.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-24 09:17:41.830475 pyatlan-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-24 09:17:30.000000 pyatlan-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:41.818475 pyatlan-0.4.1/pyatlan/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:41.822475 pyatlan-0.4.1/pyatlan/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/cache/atlan_tag_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/cache/custom_metadata_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/cache/enum_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/cache/group_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/cache/role_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/cache/user_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:41.822475 pyatlan-0.4.1/pyatlan/client/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52173 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/client/atlan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:41.822475 pyatlan-0.4.1/pyatlan/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/events/atlan_event_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/events/atlan_lambda_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:41.822475 pyatlan-0.4.1/pyatlan/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/generator/generate_from_typdefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:41.822475 pyatlan-0.4.1/pyatlan/generator/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/generator/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:41.826475 pyatlan-0.4.1/pyatlan/model/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   982643 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/atlan_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/custom_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    63801 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/keycloak_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    11543 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    60988 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24855 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/typedef.py
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/multipart_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 09:17:30.000000 pyatlan-0.4.1/pyatlan/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:41.822475 pyatlan-0.4.1/pyatlan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-24 09:17:41.000000 pyatlan-0.4.1/pyatlan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-24 09:17:41.000000 pyatlan-0.4.1/pyatlan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 09:17:41.000000 pyatlan-0.4.1/pyatlan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 09:17:41.000000 pyatlan-0.4.1/pyatlan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-24 09:17:41.000000 pyatlan-0.4.1/pyatlan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-24 09:17:41.000000 pyatlan-0.4.1/pyatlan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-24 09:17:30.000000 pyatlan-0.4.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-24 09:17:30.000000 pyatlan-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 09:17:41.830475 pyatlan-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-24 09:17:30.000000 pyatlan-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:41.826475 pyatlan-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:41.826475 pyatlan-0.4.1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/admin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/atlan_tag_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/connection_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    35979 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/custom_metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/file_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/glossary_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22401 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/lineage_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/persona_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/purpose_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/query_parser_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/s3_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9088 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/test_index_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    14555 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/integration/test_sql_assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:41.830475 pyatlan-0.4.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:41.830475 pyatlan-0.4.1/tests/unit/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/badge_condition_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/badge_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/column_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/connection_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/database_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/file_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/glossary_category_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/glossary_term_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/glossary_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/materialised_view_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/process_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/readme_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/s3_bucket_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/s3object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/schema_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/table_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/model/view_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/test_atlan_tag_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    30532 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/test_custom_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/test_glossary_term.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/test_lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)    30268 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    36655 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/test_search_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/test_typedef_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-07-24 09:17:30.000000 pyatlan-0.4.1/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:53:30.216642 pyatlan-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-07-25 07:53:19.000000 pyatlan-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-25 07:53:19.000000 pyatlan-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-25 07:53:19.000000 pyatlan-0.4.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-25 07:53:30.216642 pyatlan-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-25 07:53:19.000000 pyatlan-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:53:30.204642 pyatlan-0.4.2/pyatlan/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:53:30.208642 pyatlan-0.4.2/pyatlan/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/cache/atlan_tag_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/cache/custom_metadata_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/cache/enum_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/cache/group_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/cache/role_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/cache/user_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:53:30.208642 pyatlan-0.4.2/pyatlan/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52173 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/client/atlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:53:30.208642 pyatlan-0.4.2/pyatlan/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/events/atlan_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/events/atlan_lambda_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:53:30.208642 pyatlan-0.4.2/pyatlan/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/generator/generate_from_typdefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:53:30.208642 pyatlan-0.4.2/pyatlan/generator/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/generator/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:53:30.212642 pyatlan-0.4.2/pyatlan/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   982643 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/atlan_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63856 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/keycloak_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11543 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60988 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24855 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/typedef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/multipart_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:53:30.208642 pyatlan-0.4.2/pyatlan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-25 07:53:30.000000 pyatlan-0.4.2/pyatlan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-25 07:53:30.000000 pyatlan-0.4.2/pyatlan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 07:53:30.000000 pyatlan-0.4.2/pyatlan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 07:53:30.000000 pyatlan-0.4.2/pyatlan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-25 07:53:30.000000 pyatlan-0.4.2/pyatlan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 07:53:30.000000 pyatlan-0.4.2/pyatlan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-25 07:53:19.000000 pyatlan-0.4.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-25 07:53:19.000000 pyatlan-0.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 07:53:30.216642 pyatlan-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-25 07:53:19.000000 pyatlan-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:53:30.212642 pyatlan-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:53:30.212642 pyatlan-0.4.2/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/admin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/atlan_tag_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35979 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/custom_metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/glossary_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22401 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/lineage_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/persona_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/purpose_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/query_parser_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/s3_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9088 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/test_index_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14555 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/test_sql_assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:53:30.216642 pyatlan-0.4.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:53:30.216642 pyatlan-0.4.2/tests/unit/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/badge_condition_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/badge_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/column_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/database_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/glossary_category_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/glossary_term_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/glossary_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/materialised_view_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/process_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/readme_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/s3_bucket_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/s3object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/table_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/view_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/test_atlan_tag_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30532 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/test_custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/test_glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/test_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30268 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36655 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/test_search_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/test_typedef_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/test_utils.py
```

### Comparing `pyatlan-0.4.1/LICENSE` & `pyatlan-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/PKG-INFO` & `pyatlan-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.4.1
+Version: 0.4.2
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.4.1/README.md` & `pyatlan-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/pyatlan/cache/atlan_tag_cache.py` & `pyatlan-0.4.2/pyatlan/cache/atlan_tag_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/pyatlan/cache/custom_metadata_cache.py` & `pyatlan-0.4.2/pyatlan/cache/custom_metadata_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/pyatlan/cache/enum_cache.py` & `pyatlan-0.4.2/pyatlan/cache/enum_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/pyatlan/cache/group_cache.py` & `pyatlan-0.4.2/pyatlan/cache/group_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/pyatlan/cache/role_cache.py` & `pyatlan-0.4.2/pyatlan/cache/role_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/pyatlan/cache/user_cache.py` & `pyatlan-0.4.2/pyatlan/cache/user_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/pyatlan/client/atlan.py` & `pyatlan-0.4.2/pyatlan/client/atlan.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/pyatlan/client/constants.py` & `pyatlan-0.4.2/pyatlan/client/constants.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/pyatlan/error.py` & `pyatlan-0.4.2/pyatlan/error.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/pyatlan/events/atlan_event_handler.py` & `pyatlan-0.4.2/pyatlan/events/atlan_event_handler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/pyatlan/events/atlan_lambda_handler.py` & `pyatlan-0.4.2/pyatlan/events/atlan_lambda_handler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/pyatlan/exceptions.py` & `pyatlan-0.4.2/pyatlan/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/pyatlan/generator/generate_from_typdefs.py` & `pyatlan-0.4.2/pyatlan/generator/generate_from_typdefs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/pyatlan/model/assets.py` & `pyatlan-0.4.2/pyatlan/model/assets.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/pyatlan/model/atlan_image.py` & `pyatlan-0.4.2/pyatlan/model/atlan_image.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/pyatlan/model/core.py` & `pyatlan-0.4.2/pyatlan/model/core.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/pyatlan/model/custom_metadata.py` & `pyatlan-0.4.2/pyatlan/model/custom_metadata.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/pyatlan/model/enums.py` & `pyatlan-0.4.2/pyatlan/model/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,14 +301,15 @@
     CLOUDERA_DATA_WAREHOUSE = (
         "cloudera-data-warehouse",
         AtlanConnectionCategory.WAREHOUSE,
     )
     STARBURST_GALAXY = ("starburst-galaxy", AtlanConnectionCategory.WAREHOUSE)
     REDIS = ("redis", AtlanConnectionCategory.DATABASE)
     GRAPHQL = ("graphql", AtlanConnectionCategory.DATABASE)
+    ALTERYX = ("alteryx", AtlanConnectionCategory.API)
 
 
 class AtlanCustomAttributePrimitiveType(str, Enum):
     def __new__(cls, value: str) -> "AtlanCustomAttributePrimitiveType":
         obj = str.__new__(cls, value)
         obj._value_ = value
         return obj
```

### Comparing `pyatlan-0.4.1/pyatlan/model/events.py` & `pyatlan-0.4.2/pyatlan/model/events.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/pyatlan/model/group.py` & `pyatlan-0.4.2/pyatlan/model/group.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/pyatlan/model/keycloak_events.py` & `pyatlan-0.4.2/pyatlan/model/keycloak_events.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/pyatlan/model/lineage.py` & `pyatlan-0.4.2/pyatlan/model/lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/pyatlan/model/query.py` & `pyatlan-0.4.2/pyatlan/model/query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/pyatlan/model/response.py` & `pyatlan-0.4.2/pyatlan/model/response.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/pyatlan/model/role.py` & `pyatlan-0.4.2/pyatlan/model/role.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/pyatlan/model/search.py` & `pyatlan-0.4.2/pyatlan/model/search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/pyatlan/model/structs.py` & `pyatlan-0.4.2/pyatlan/model/structs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/pyatlan/model/typedef.py` & `pyatlan-0.4.2/pyatlan/model/typedef.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/pyatlan/model/user.py` & `pyatlan-0.4.2/pyatlan/model/user.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/pyatlan/multipart_data_generator.py` & `pyatlan-0.4.2/pyatlan/multipart_data_generator.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/pyatlan/utils.py` & `pyatlan-0.4.2/pyatlan/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/pyatlan.egg-info/PKG-INFO` & `pyatlan-0.4.2/pyatlan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.4.1
+Version: 0.4.2
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.4.1/pyatlan.egg-info/SOURCES.txt` & `pyatlan-0.4.2/pyatlan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/setup.py` & `pyatlan-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/integration/admin_test.py` & `pyatlan-0.4.2/tests/integration/admin_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/integration/atlan_tag_test.py` & `pyatlan-0.4.2/tests/integration/atlan_tag_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/integration/client.py` & `pyatlan-0.4.2/tests/integration/client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/integration/connection_test.py` & `pyatlan-0.4.2/tests/integration/connection_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/integration/custom_metadata_test.py` & `pyatlan-0.4.2/tests/integration/custom_metadata_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/integration/file_test.py` & `pyatlan-0.4.2/tests/integration/file_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/integration/glossary_test.py` & `pyatlan-0.4.2/tests/integration/glossary_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/integration/lineage_test.py` & `pyatlan-0.4.2/tests/integration/lineage_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/integration/persona_test.py` & `pyatlan-0.4.2/tests/integration/persona_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/integration/purpose_test.py` & `pyatlan-0.4.2/tests/integration/purpose_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/integration/query_parser_test.py` & `pyatlan-0.4.2/tests/integration/query_parser_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/integration/s3_asset_test.py` & `pyatlan-0.4.2/tests/integration/s3_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/integration/test_client.py` & `pyatlan-0.4.2/tests/integration/test_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/integration/test_index_search.py` & `pyatlan-0.4.2/tests/integration/test_index_search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/integration/test_sql_assets.py` & `pyatlan-0.4.2/tests/integration/test_sql_assets.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/unit/conftest.py` & `pyatlan-0.4.2/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/unit/model/badge_condition_test.py` & `pyatlan-0.4.2/tests/unit/model/badge_condition_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/unit/model/badge_test.py` & `pyatlan-0.4.2/tests/unit/model/badge_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/unit/model/column_test.py` & `pyatlan-0.4.2/tests/unit/model/column_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/unit/model/connection_test.py` & `pyatlan-0.4.2/tests/unit/model/connection_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/unit/model/constants.py` & `pyatlan-0.4.2/tests/unit/model/constants.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/unit/model/database_test.py` & `pyatlan-0.4.2/tests/unit/model/database_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/unit/model/file_test.py` & `pyatlan-0.4.2/tests/unit/model/file_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/unit/model/glossary_category_test.py` & `pyatlan-0.4.2/tests/unit/model/glossary_category_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/unit/model/glossary_term_test.py` & `pyatlan-0.4.2/tests/unit/model/glossary_term_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/unit/model/glossary_test.py` & `pyatlan-0.4.2/tests/unit/model/glossary_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/unit/model/materialised_view_test.py` & `pyatlan-0.4.2/tests/unit/model/materialised_view_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/unit/model/process_test.py` & `pyatlan-0.4.2/tests/unit/model/process_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/unit/model/readme_test.py` & `pyatlan-0.4.2/tests/unit/model/readme_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/unit/model/s3_bucket_test.py` & `pyatlan-0.4.2/tests/unit/model/s3_bucket_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/unit/model/s3object_test.py` & `pyatlan-0.4.2/tests/unit/model/s3object_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/unit/model/schema_test.py` & `pyatlan-0.4.2/tests/unit/model/schema_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/unit/model/table_test.py` & `pyatlan-0.4.2/tests/unit/model/table_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/unit/model/view_test.py` & `pyatlan-0.4.2/tests/unit/model/view_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/unit/test_atlan_tag_name.py` & `pyatlan-0.4.2/tests/unit/test_atlan_tag_name.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/unit/test_client.py` & `pyatlan-0.4.2/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/unit/test_custom_metadata.py` & `pyatlan-0.4.2/tests/unit/test_custom_metadata.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/unit/test_events.py` & `pyatlan-0.4.2/tests/unit/test_events.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/unit/test_glossary_term.py` & `pyatlan-0.4.2/tests/unit/test_glossary_term.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/unit/test_lineage.py` & `pyatlan-0.4.2/tests/unit/test_lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/unit/test_model.py` & `pyatlan-0.4.2/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/unit/test_search_model.py` & `pyatlan-0.4.2/tests/unit/test_search_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/unit/test_typedef_model.py` & `pyatlan-0.4.2/tests/unit/test_typedef_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.1/tests/unit/test_utils.py` & `pyatlan-0.4.2/tests/unit/test_utils.py`

 * *Files identical despite different names*

