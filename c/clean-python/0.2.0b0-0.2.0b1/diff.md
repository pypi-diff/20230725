# Comparing `tmp/clean-python-0.2.0b0.tar.gz` & `tmp/clean-python-0.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean-python-0.2.0b0.tar", last modified: Sun Jul 23 06:14:06 2023, max compression
+gzip compressed data, was "clean-python-0.2.0b1.tar", last modified: Tue Jul 25 07:30:27 2023, max compression
```

## Comparing `clean-python-0.2.0b0.tar` & `clean-python-0.2.0b1.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 06:14:06.580703 clean-python-0.2.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-07-23 06:14:06.580703 clean-python-0.2.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 06:14:06.572702 clean-python-0.2.0b0/clean_python/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 06:14:06.572702 clean-python-0.2.0b0/clean_python/base/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 06:14:06.572702 clean-python-0.2.0b0/clean_python/base/application/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/base/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/base/application/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 06:14:06.576702 clean-python-0.2.0b0/clean_python/base/domain/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/base/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/base/domain/domain_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/base/domain/domain_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/base/domain/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/base/domain/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/base/domain/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/base/domain/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/base/domain/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/base/domain/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/base/domain/root_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/base/domain/value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/base/domain/value_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 06:14:06.576702 clean-python-0.2.0b0/clean_python/base/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/base/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/base/infrastructure/in_memory_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/base/infrastructure/internal_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/base/infrastructure/tmpdir_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 06:14:06.576702 clean-python-0.2.0b0/clean_python/base/presentation/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/base/presentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/base/presentation/link.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 06:14:06.576702 clean-python-0.2.0b0/clean_python/celery/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/celery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/celery/celery_rmq_broker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 06:14:06.576702 clean-python-0.2.0b0/clean_python/dramatiq/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/dramatiq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/dramatiq/async_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/dramatiq/dramatiq_task_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/dramatiq/sleep_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 06:14:06.576702 clean-python-0.2.0b0/clean_python/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/fastapi/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/fastapi/error_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/fastapi/fastapi_access_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/fastapi/request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/fastapi/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/fastapi/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 06:14:06.576702 clean-python-0.2.0b0/clean_python/fluentbit/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/fluentbit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/fluentbit/fluentbit_gateway.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 06:14:06.576702 clean-python-0.2.0b0/clean_python/oauth2/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/oauth2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/oauth2/oauth2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 06:14:06.580703 clean-python-0.2.0b0/clean_python/sql/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/sql/sql_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/sql/sql_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/sql/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 06:14:06.580703 clean-python-0.2.0b0/clean_python/testing/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/testing/attr_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/testing/debugger.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/clean_python/testing/profilers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 06:14:06.572702 clean-python-0.2.0b0/clean_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-07-23 06:14:06.000000 clean-python-0.2.0b0/clean_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-23 06:14:06.000000 clean-python-0.2.0b0/clean_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 06:14:06.000000 clean-python-0.2.0b0/clean_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 06:14:06.000000 clean-python-0.2.0b0/clean_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-23 06:14:06.000000 clean-python-0.2.0b0/clean_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-23 06:14:06.000000 clean-python-0.2.0b0/clean_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-23 06:14:06.580703 clean-python-0.2.0b0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 06:14:06.580703 clean-python-0.2.0b0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/tests/test_async_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/tests/test_celery_rmq_broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/tests/test_dramatiq_task_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/tests/test_fastapi_access_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/tests/test_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/tests/test_internal_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/tests/test_manage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/tests/test_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/tests/test_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/tests/test_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/tests/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/tests/test_root_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/tests/test_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/tests/test_sql_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-23 06:13:57.000000 clean-python-0.2.0b0/tests/test_value_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.206447 clean-python-0.2.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-07-25 07:30:27.206447 clean-python-0.2.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.198447 clean-python-0.2.0b1/clean_python/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.198447 clean-python-0.2.0b1/clean_python/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.198447 clean-python-0.2.0b1/clean_python/base/application/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/application/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.202447 clean-python-0.2.0b1/clean_python/base/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/domain/domain_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/domain/domain_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/domain/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/domain/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/domain/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/domain/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/domain/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/domain/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/domain/root_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/domain/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/domain/value_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.202447 clean-python-0.2.0b1/clean_python/base/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/infrastructure/in_memory_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/infrastructure/internal_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/infrastructure/tmpdir_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.202447 clean-python-0.2.0b1/clean_python/base/presentation/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/presentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/base/presentation/link.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.202447 clean-python-0.2.0b1/clean_python/celery/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/celery/celery_rmq_broker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.202447 clean-python-0.2.0b1/clean_python/dramatiq/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/dramatiq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/dramatiq/async_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/dramatiq/dramatiq_task_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/dramatiq/sleep_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.202447 clean-python-0.2.0b1/clean_python/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/fastapi/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/fastapi/error_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/fastapi/fastapi_access_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/fastapi/request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/fastapi/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/fastapi/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.202447 clean-python-0.2.0b1/clean_python/fluentbit/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/fluentbit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/fluentbit/fluentbit_gateway.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.206447 clean-python-0.2.0b1/clean_python/oauth2/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/oauth2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/oauth2/oauth2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.206447 clean-python-0.2.0b1/clean_python/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/sql/sql_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/sql/sql_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/sql/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.206447 clean-python-0.2.0b1/clean_python/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/testing/attr_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/testing/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/clean_python/testing/profilers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.198447 clean-python-0.2.0b1/clean_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-07-25 07:30:27.000000 clean-python-0.2.0b1/clean_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-25 07:30:27.000000 clean-python-0.2.0b1/clean_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 07:30:27.000000 clean-python-0.2.0b1/clean_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 07:30:26.000000 clean-python-0.2.0b1/clean_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-25 07:30:27.000000 clean-python-0.2.0b1/clean_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 07:30:27.000000 clean-python-0.2.0b1/clean_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-25 07:30:27.210447 clean-python-0.2.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:30:27.206447 clean-python-0.2.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_async_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_celery_rmq_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_dramatiq_task_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_fastapi_access_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_internal_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_root_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_sql_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-25 07:30:17.000000 clean-python-0.2.0b1/tests/test_value_object.py
```

### Comparing `clean-python-0.2.0b0/LICENSE` & `clean-python-0.2.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/PKG-INFO` & `clean-python-0.2.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-python
-Version: 0.2.0b0
+Version: 0.2.0b1
 Summary: Clean architecture in Python
 Author-email: Nelen & Schuurmans <info@nelen-schuurmans.nl>
 License: MIT
 Project-URL: homepage, https://github.com/nens/clean-python
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `clean-python-0.2.0b0/README.md` & `clean-python-0.2.0b1/README.md`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/clean_python/base/application/manage.py` & `clean-python-0.2.0b1/clean_python/base/application/manage.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/clean_python/base/domain/domain_event.py` & `clean-python-0.2.0b1/clean_python/base/domain/domain_event.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/clean_python/base/domain/exceptions.py` & `clean-python-0.2.0b1/clean_python/base/domain/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # (c) Nelen & Schuurmans
 
 from typing import Any
+from typing import Dict
+from typing import List
 from typing import Optional
 from typing import Union
 
 from pydantic import create_model
 from pydantic import ValidationError
 
 __all__ = [
@@ -54,14 +56,19 @@
 
 
 class BadRequest(Exception):
     def __init__(self, err_or_msg: Union[ValidationError, str]):
         self._internal_error = err_or_msg
         super().__init__(err_or_msg)
 
+    def errors(self) -> List[Dict]:
+        if isinstance(self._internal_error, ValidationError):
+            return self._internal_error.errors()
+        return [{"error": self}]
+
     def __str__(self) -> str:
         error = self._internal_error
         if isinstance(error, ValidationError):
             error = error.errors()[0]
             loc = "'" + ",".join([str(x) for x in error["loc"]]) + "' "
             if loc == "'*' ":
                 loc = ""
```

### Comparing `clean-python-0.2.0b0/clean_python/base/domain/gateway.py` & `clean-python-0.2.0b1/clean_python/base/domain/gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/clean_python/base/domain/repository.py` & `clean-python-0.2.0b1/clean_python/base/domain/repository.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/clean_python/base/domain/root_entity.py` & `clean-python-0.2.0b1/clean_python/base/domain/root_entity.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/clean_python/base/domain/value_object.py` & `clean-python-0.2.0b1/clean_python/base/domain/value_object.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/clean_python/base/infrastructure/in_memory_gateway.py` & `clean-python-0.2.0b1/clean_python/base/infrastructure/in_memory_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/clean_python/base/infrastructure/internal_gateway.py` & `clean-python-0.2.0b1/clean_python/base/infrastructure/internal_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/clean_python/celery/celery_rmq_broker.py` & `clean-python-0.2.0b1/clean_python/celery/celery_rmq_broker.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/clean_python/dramatiq/async_actor.py` & `clean-python-0.2.0b1/clean_python/dramatiq/async_actor.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/clean_python/dramatiq/dramatiq_task_logger.py` & `clean-python-0.2.0b1/clean_python/dramatiq/dramatiq_task_logger.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/clean_python/dramatiq/sleep_task.py` & `clean-python-0.2.0b1/clean_python/dramatiq/sleep_task.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/clean_python/fastapi/context.py` & `clean-python-0.2.0b1/clean_python/fastapi/context.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/clean_python/fastapi/error_responses.py` & `clean-python-0.2.0b1/clean_python/fastapi/error_responses.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/clean_python/fastapi/fastapi_access_logger.py` & `clean-python-0.2.0b1/clean_python/fastapi/fastapi_access_logger.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/clean_python/fastapi/request_query.py` & `clean-python-0.2.0b1/clean_python/fastapi/request_query.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/clean_python/fastapi/resource.py` & `clean-python-0.2.0b1/clean_python/fastapi/resource.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/clean_python/fastapi/service.py` & `clean-python-0.2.0b1/clean_python/fastapi/service.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,31 +3,35 @@
 import logging
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Set
+from typing import Union
 
 from asgiref.sync import sync_to_async
 from fastapi import Depends
 from fastapi import FastAPI
 from fastapi import Request
+from fastapi import Security
 from fastapi.exceptions import HTTPException
 from fastapi.exceptions import RequestValidationError
 from fastapi.security import OAuth2AuthorizationCodeBearer
+from fastapi.security.api_key import APIKeyHeader
 from starlette.status import HTTP_401_UNAUTHORIZED
 from starlette.status import HTTP_403_FORBIDDEN
 from starlette.types import ASGIApp
 
 from clean_python import Conflict
 from clean_python import DoesNotExist
 from clean_python import Gateway
 from clean_python import PermissionDenied
 from clean_python import Unauthorized
+from clean_python.oauth2 import AccessTokenVerifierSettings
 from clean_python.oauth2 import OAuth2AccessTokenVerifier
 from clean_python.oauth2 import OAuth2Settings
 
 from .context import RequestMiddleware
 from .error_responses import BadRequest
 from .error_responses import conflict_handler
 from .error_responses import DefaultErrorResponse
@@ -78,26 +82,76 @@
             await self.verifier(token)
         except Unauthorized:
             raise HTTPException(status_code=HTTP_401_UNAUTHORIZED)
         except PermissionDenied:
             raise HTTPException(status_code=HTTP_403_FORBIDDEN)
 
 
-def fastapi_oauth_kwargs(auth: Optional[OAuth2Settings]) -> Dict:
-    if auth is None:
-        return {}
+def fastapi_oauth_kwargs(auth: OAuth2Settings) -> Dict:
     return {
         "dependencies": [Depends(OAuth2Dependable(scope="*:readwrite", settings=auth))],
         "swagger_ui_init_oauth": {
             "clientId": auth.client_id,
             "usePkceWithAuthorizationCodeGrant": True,
         },
     }
 
 
+api_key_header = APIKeyHeader(name="access_token", auto_error=False)
+
+
+class ApiKeyDependable:
+    def __init__(self, scope, settings: AccessTokenVerifierSettings):
+        self.verifier = sync_to_async(
+            OAuth2AccessTokenVerifier(
+                scope,
+                issuer=settings.issuer,
+                resource_server_id=settings.resource_server_id,
+                algorithms=settings.algorithms,
+                admin_users=settings.admin_users,
+                verify_scope_enabled=settings.scope_validation_enabled,
+            ),
+            thread_sensitive=False,
+        )
+
+    async def __call__(
+        self, request: Request, api_key_header: str = Security(api_key_header)
+    ) -> None:
+        try:
+            claims = await self.verifier(api_key_header)
+            request.scope["user"] = claims
+        except Unauthorized:
+            raise HTTPException(status_code=HTTP_401_UNAUTHORIZED)
+        except PermissionDenied:
+            raise HTTPException(status_code=HTTP_403_FORBIDDEN)
+
+
+def fastapi_accesstoken_verifier_kwargs(auth: AccessTokenVerifierSettings) -> Dict:
+    return {
+        "dependencies": [Depends(ApiKeyDependable("", settings=auth))],
+    }
+
+
+class UnknownAuthSettings(Exception):
+    pass
+
+
+AUTH_MAPPING = {
+    OAuth2Settings: fastapi_oauth_kwargs,
+    AccessTokenVerifierSettings: fastapi_accesstoken_verifier_kwargs,
+}
+
+
+def get_auth_kwargs(auth: Any) -> None:
+    func = AUTH_MAPPING.get(type(auth), None)
+    if func is None:
+        raise UnknownAuthSettings(f"Unknown auth setting: {auth}")
+    return func(auth)
+
+
 async def health_check():
     """Simple health check route"""
     return {"health": "OK"}
 
 
 class Service:
     resources: List[Resource]
@@ -166,29 +220,29 @@
         return app
 
     def create_app(
         self,
         title: str,
         description: str,
         hostname: str,
-        auth: Optional[OAuth2Settings] = None,
+        auth: Optional[Union[OAuth2Settings, AccessTokenVerifierSettings]] = None,
         on_startup: Optional[List[Callable[[], Any]]] = None,
         access_logger_gateway: Optional[Gateway] = None,
     ) -> ASGIApp:
         app = self._create_root_app(
             title=title,
             description=description,
             hostname=hostname,
             on_startup=on_startup,
             access_logger_gateway=access_logger_gateway,
         )
         kwargs = {
             "title": title,
             "description": description,
-            **fastapi_oauth_kwargs(auth),
+            **get_auth_kwargs(auth),
         }
         versioned_apps = {
             v: self._create_versioned_app(v, **kwargs) for v in self.versions
         }
         for v, versioned_app in versioned_apps.items():
             app.mount("/" + v.prefix, versioned_app)
         return app
```

### Comparing `clean-python-0.2.0b0/clean_python/oauth2/oauth2.py` & `clean-python-0.2.0b1/clean_python/oauth2/oauth2.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,27 +8,35 @@
 from jwt.exceptions import PyJWTError
 from pydantic import AnyHttpUrl
 from pydantic import BaseModel
 
 from clean_python.base.domain.exceptions import PermissionDenied
 from clean_python.base.domain.exceptions import Unauthorized
 
-__all__ = ["OAuth2Settings", "OAuth2AccessTokenVerifier"]
+__all__ = ["OAuth2Settings", "AccessTokenVerifierSettings", "OAuth2AccessTokenVerifier"]
 
 
 class OAuth2Settings(BaseModel):
     client_id: str
     issuer: str
     resource_server_id: str
     token_url: AnyHttpUrl
     authorization_url: AnyHttpUrl
     algorithms: List[str] = ["RS256"]
     admin_users: List[str]
 
 
+class AccessTokenVerifierSettings(BaseModel):
+    issuer: str
+    resource_server_id: str
+    algorithms: List[str] = ["RS256"]
+    admin_users: List[str]
+    scope_validation_enabled: bool = True
+
+
 class OAuth2AccessTokenVerifier:
     """A class for verifying OAuth2 Access Tokens from AWS Cognito
 
     The verification steps followed are documented here:
 
     https://docs.aws.amazon.com/cognito/latest/developerguide/amazon- ⏎
     cognito-user-pools-using-tokens-verifying-a-jwt.html
@@ -40,16 +48,18 @@
     def __init__(
         self,
         scope: str,
         issuer: str,
         resource_server_id: str,
         algorithms: List[str],
         admin_users: List[str],
+        verify_scope_enabled: bool = True,
     ):
         self.scope = scope
+        self.verify_scope_enabled = verify_scope_enabled
         self.issuer = issuer
         self.algorithms = algorithms
         self.resource_server_id = resource_server_id
         self.admin_users = admin_users
         self.jwk_client = PyJWKClient(f"{issuer}/.well-known/jwks.json")
 
     def __call__(self, token: str) -> Dict:
@@ -97,14 +107,16 @@
     def verify_scope(self, claims):
         """Check scope claim.
 
         Cognito includes the resource server id inside the scope, like this:
 
            raster.lizard.net/*.readwrite
         """
+        if not self.verify_scope_enabled:
+            return
         if f"{self.resource_server_id}{self.scope}" not in claims["scope"].split(" "):
             # logger.info("Token has invalid scope claim: %s", claims["scope"])
             raise Unauthorized()
 
     def authorize(self, claims):
         """The subject (sub) claim should be in a hard-coded whitelist."""
         if claims.get("sub") not in self.admin_users:
```

### Comparing `clean-python-0.2.0b0/clean_python/sql/sql_gateway.py` & `clean-python-0.2.0b1/clean_python/sql/sql_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/clean_python/sql/sql_provider.py` & `clean-python-0.2.0b1/clean_python/sql/sql_provider.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/clean_python/sql/testing.py` & `clean-python-0.2.0b1/clean_python/sql/testing.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/clean_python/testing/debugger.py` & `clean-python-0.2.0b1/clean_python/testing/debugger.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/clean_python/testing/profilers.py` & `clean-python-0.2.0b1/clean_python/testing/profilers.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/clean_python.egg-info/PKG-INFO` & `clean-python-0.2.0b1/clean_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-python
-Version: 0.2.0b0
+Version: 0.2.0b1
 Summary: Clean architecture in Python
 Author-email: Nelen & Schuurmans <info@nelen-schuurmans.nl>
 License: MIT
 Project-URL: homepage, https://github.com/nens/clean-python
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `clean-python-0.2.0b0/clean_python.egg-info/SOURCES.txt` & `clean-python-0.2.0b1/clean_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/pyproject.toml` & `clean-python-0.2.0b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/tests/test_async_actor.py` & `clean-python-0.2.0b1/tests/test_async_actor.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/tests/test_celery_rmq_broker.py` & `clean-python-0.2.0b1/tests/test_celery_rmq_broker.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/tests/test_dramatiq_task_logger.py` & `clean-python-0.2.0b1/tests/test_dramatiq_task_logger.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/tests/test_exceptions.py` & `clean-python-0.2.0b1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/tests/test_fastapi_access_logger.py` & `clean-python-0.2.0b1/tests/test_fastapi_access_logger.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/tests/test_gateway.py` & `clean-python-0.2.0b1/tests/test_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/tests/test_internal_gateway.py` & `clean-python-0.2.0b1/tests/test_internal_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/tests/test_manage.py` & `clean-python-0.2.0b1/tests/test_manage.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/tests/test_oauth2.py` & `clean-python-0.2.0b1/tests/test_oauth2.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/tests/test_repository.py` & `clean-python-0.2.0b1/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/tests/test_request_query.py` & `clean-python-0.2.0b1/tests/test_request_query.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/tests/test_resource.py` & `clean-python-0.2.0b1/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/tests/test_root_entity.py` & `clean-python-0.2.0b1/tests/test_root_entity.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/tests/test_service.py` & `clean-python-0.2.0b1/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/tests/test_sql_gateway.py` & `clean-python-0.2.0b1/tests/test_sql_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b0/tests/test_value_object.py` & `clean-python-0.2.0b1/tests/test_value_object.py`

 * *Files identical despite different names*

