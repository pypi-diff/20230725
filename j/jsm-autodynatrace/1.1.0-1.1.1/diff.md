# Comparing `tmp/jsm-autodynatrace-1.1.0.tar.gz` & `tmp/jsm-autodynatrace-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsm-autodynatrace-1.1.0.tar", last modified: Fri Jul 21 18:54:00 2023, max compression
+gzip compressed data, was "jsm-autodynatrace-1.1.1.tar", last modified: Tue Jul 25 19:31:06 2023, max compression
```

## Comparing `jsm-autodynatrace-1.1.0.tar` & `jsm-autodynatrace-1.1.1.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.537609 jsm-autodynatrace-1.1.0/
--rw-r--r--   0 matheusslgd   (502) staff       (20)    12871 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/LICENSE
--rw-r--r--   0 matheusslgd   (502) staff       (20)     1140 2023-07-21 18:54:00.537699 jsm-autodynatrace-1.1.0/PKG-INFO
--rw-r--r--   0 matheusslgd   (502) staff       (20)     3168 2023-07-18 20:34:31.000000 jsm-autodynatrace-1.1.0/README.md
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.524531 jsm-autodynatrace-1.1.0/autodynatrace/
--rw-r--r--   0 matheusslgd   (502) staff       (20)     3973 2023-07-21 18:53:46.000000 jsm-autodynatrace-1.1.0/autodynatrace/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)      320 2023-07-17 20:30:37.000000 jsm-autodynatrace-1.1.0/autodynatrace/log.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)      523 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/sdk.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.524883 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/
--rw-r--r--   0 matheusslgd   (502) staff       (20)        0 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/__init__.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.525391 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/aiohttp/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/aiohttp/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)      935 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/aiohttp/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.526146 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/bottle/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/bottle/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     2044 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/bottle/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.526491 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/celery/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/celery/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     4454 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/celery/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.526821 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/concurrent/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/concurrent/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     1691 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/concurrent/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.527125 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/confluent_kafka/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/confluent_kafka/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     3550 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/confluent_kafka/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.527430 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/custom/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       45 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/custom/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     2473 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/custom/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.527724 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/cx_Oracle/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/cx_Oracle/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     4412 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/cx_Oracle/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.527869 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/dbapi/
--rw-r--r--   0 matheusslgd   (502) staff       (20)     2792 2023-07-18 20:34:01.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/dbapi/__init__.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.529185 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django/
--rw-r--r--   0 matheusslgd   (502) staff       (20)      152 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)      265 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django/apps.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     1819 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django/db.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)      656 2023-07-18 20:34:31.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django/log.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     3388 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django/middlewares.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     1735 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django/utils.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)      974 2023-07-18 20:34:31.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.530283 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django_outbox_pattern/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       31 2023-07-21 18:53:46.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django_outbox_pattern/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     2085 2023-07-21 18:53:46.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django_outbox_pattern/consumer.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     1623 2023-07-21 18:53:46.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django_outbox_pattern/publisher.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)      157 2023-07-21 18:53:46.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django_outbox_pattern/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.531340 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django_stomp/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       31 2023-07-18 20:34:01.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django_stomp/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     2095 2023-07-18 20:34:01.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django_stomp/consumer.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     1658 2023-07-18 20:34:01.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django_stomp/publisher.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)      481 2023-07-18 20:34:02.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django_stomp/utils.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)      157 2023-07-18 20:34:01.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django_stomp/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.531774 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/fastapi/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/fastapi/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     2387 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/fastapi/middleware.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     1326 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/fastapi/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.532144 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/flask/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/flask/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     2554 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/flask/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.532453 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/grpc/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/grpc/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     2357 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/grpc/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.532775 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/paramiko/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/paramiko/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     1041 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/paramiko/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.533113 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/pika/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/pika/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     3353 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/pika/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.533395 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/psycopg2/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/psycopg2/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     2193 2023-07-18 20:34:02.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/psycopg2/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.533755 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/pymongo/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/pymongo/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     2060 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/pymongo/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.534112 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/pysnmp/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/pysnmp/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     4813 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/pysnmp/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.534509 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/redis/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/redis/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)      716 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/redis/utils.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     2061 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/redis/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.534779 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/ruxit/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/ruxit/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)      462 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/ruxit/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.535050 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/sqlalchemy/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/sqlalchemy/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     4386 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/sqlalchemy/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.535322 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/starlette/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/starlette/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     1424 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/starlette/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.535585 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/subprocess/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/subprocess/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     1365 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/subprocess/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.535853 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/suds/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/suds/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)      697 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/suds/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.536126 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/tornado/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/tornado/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     1703 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/tornado/wrapper.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.536381 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/urllib/
--rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/urllib/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     1522 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/urllib/wrapper.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)      102 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/autodynatrace/wrappers/utils.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.537088 jsm-autodynatrace-1.1.0/jsm_autodynatrace.egg-info/
--rw-r--r--   0 matheusslgd   (502) staff       (20)     1140 2023-07-21 18:54:00.000000 jsm-autodynatrace-1.1.0/jsm_autodynatrace.egg-info/PKG-INFO
--rw-r--r--   0 matheusslgd   (502) staff       (20)     3307 2023-07-21 18:54:00.000000 jsm-autodynatrace-1.1.0/jsm_autodynatrace.egg-info/SOURCES.txt
--rw-r--r--   0 matheusslgd   (502) staff       (20)        1 2023-07-21 18:54:00.000000 jsm-autodynatrace-1.1.0/jsm_autodynatrace.egg-info/dependency_links.txt
--rw-r--r--   0 matheusslgd   (502) staff       (20)       44 2023-07-21 18:54:00.000000 jsm-autodynatrace-1.1.0/jsm_autodynatrace.egg-info/entry_points.txt
--rw-r--r--   0 matheusslgd   (502) staff       (20)       61 2023-07-21 18:54:00.000000 jsm-autodynatrace-1.1.0/jsm_autodynatrace.egg-info/requires.txt
--rw-r--r--   0 matheusslgd   (502) staff       (20)       20 2023-07-21 18:54:00.000000 jsm-autodynatrace-1.1.0/jsm_autodynatrace.egg-info/top_level.txt
--rw-r--r--   0 matheusslgd   (502) staff       (20)      102 2023-07-21 18:54:00.537933 jsm-autodynatrace-1.1.0/setup.cfg
--rw-r--r--   0 matheusslgd   (502) staff       (20)     1545 2023-07-21 18:53:46.000000 jsm-autodynatrace-1.1.0/setup.py
-drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-21 18:54:00.537461 jsm-autodynatrace-1.1.0/tests/
--rw-r--r--   0 matheusslgd   (502) staff       (20)        0 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/tests/__init__.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     6759 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/tests/test_custom.py
--rw-r--r--   0 matheusslgd   (502) staff       (20)     1327 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.0/tests/test_django.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.270324 jsm-autodynatrace-1.1.1/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)    12871 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/LICENSE
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     1140 2023-07-25 19:31:06.270406 jsm-autodynatrace-1.1.1/PKG-INFO
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     3168 2023-07-18 20:34:31.000000 jsm-autodynatrace-1.1.1/README.md
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.255398 jsm-autodynatrace-1.1.1/autodynatrace/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     3973 2023-07-21 18:53:46.000000 jsm-autodynatrace-1.1.1/autodynatrace/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)      320 2023-07-17 20:30:37.000000 jsm-autodynatrace-1.1.1/autodynatrace/log.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)      523 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/sdk.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.255771 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)        0 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/__init__.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.256275 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/aiohttp/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/aiohttp/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)      935 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/aiohttp/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.257037 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/bottle/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/bottle/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     2044 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/bottle/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.257384 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/celery/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/celery/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     4454 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/celery/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.257693 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/concurrent/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/concurrent/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     1691 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/concurrent/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.258015 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/confluent_kafka/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/confluent_kafka/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     3550 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/confluent_kafka/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.258354 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/custom/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       45 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/custom/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     2473 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/custom/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.258693 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/cx_Oracle/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/cx_Oracle/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     4412 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/cx_Oracle/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.258865 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/dbapi/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     2792 2023-07-18 20:34:01.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/dbapi/__init__.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.260119 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/django/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)      152 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/django/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)      265 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/django/apps.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     1819 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/django/db.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)      656 2023-07-18 20:34:31.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/django/log.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     3388 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/django/middlewares.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     1735 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/django/utils.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)      974 2023-07-18 20:34:31.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/django/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.261038 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/django_outbox_pattern/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       31 2023-07-24 21:47:37.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/django_outbox_pattern/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     2085 2023-07-21 18:53:46.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/django_outbox_pattern/consumer.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     3473 2023-07-25 19:30:23.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/django_outbox_pattern/publisher.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)      157 2023-07-24 23:03:04.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/django_outbox_pattern/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.262865 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/django_stomp/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       31 2023-07-18 20:34:01.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/django_stomp/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     2095 2023-07-18 20:34:01.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/django_stomp/consumer.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     1775 2023-07-25 19:30:23.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/django_stomp/publisher.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)      481 2023-07-18 20:34:02.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/django_stomp/utils.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)      157 2023-07-18 20:34:01.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/django_stomp/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.263389 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/fastapi/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/fastapi/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     2387 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/fastapi/middleware.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     1326 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/fastapi/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.263741 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/flask/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/flask/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     2554 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/flask/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.264115 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/grpc/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/grpc/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     2357 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/grpc/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.264453 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/paramiko/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/paramiko/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     1041 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/paramiko/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.264852 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/pika/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/pika/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     3353 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/pika/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.265324 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/psycopg2/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/psycopg2/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     2193 2023-07-18 20:34:02.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/psycopg2/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.265797 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/pymongo/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/pymongo/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     2060 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/pymongo/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.266207 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/pysnmp/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/pysnmp/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     4813 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/pysnmp/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.266712 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/redis/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/redis/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)      716 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/redis/utils.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     2061 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/redis/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.267009 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/ruxit/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/ruxit/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)      462 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/ruxit/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.267299 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/sqlalchemy/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/sqlalchemy/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     4386 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/sqlalchemy/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.267670 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/starlette/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/starlette/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     1424 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/starlette/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.267991 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/subprocess/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/subprocess/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     1365 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/subprocess/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.268276 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/suds/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/suds/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)      697 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/suds/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.268564 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/tornado/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/tornado/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     1703 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/tornado/wrapper.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.268945 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/urllib/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       32 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/urllib/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     1522 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/urllib/wrapper.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)      102 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/autodynatrace/wrappers/utils.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.269744 jsm-autodynatrace-1.1.1/jsm_autodynatrace.egg-info/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     1140 2023-07-25 19:31:06.000000 jsm-autodynatrace-1.1.1/jsm_autodynatrace.egg-info/PKG-INFO
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     3307 2023-07-25 19:31:06.000000 jsm-autodynatrace-1.1.1/jsm_autodynatrace.egg-info/SOURCES.txt
+-rw-r--r--   0 matheusslgd   (502) staff       (20)        1 2023-07-25 19:31:06.000000 jsm-autodynatrace-1.1.1/jsm_autodynatrace.egg-info/dependency_links.txt
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       44 2023-07-25 19:31:06.000000 jsm-autodynatrace-1.1.1/jsm_autodynatrace.egg-info/entry_points.txt
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       61 2023-07-25 19:31:06.000000 jsm-autodynatrace-1.1.1/jsm_autodynatrace.egg-info/requires.txt
+-rw-r--r--   0 matheusslgd   (502) staff       (20)       20 2023-07-25 19:31:06.000000 jsm-autodynatrace-1.1.1/jsm_autodynatrace.egg-info/top_level.txt
+-rw-r--r--   0 matheusslgd   (502) staff       (20)      102 2023-07-25 19:31:06.270702 jsm-autodynatrace-1.1.1/setup.cfg
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     1545 2023-07-25 19:30:23.000000 jsm-autodynatrace-1.1.1/setup.py
+drwxr-xr-x   0 matheusslgd   (502) staff       (20)        0 2023-07-25 19:31:06.270133 jsm-autodynatrace-1.1.1/tests/
+-rw-r--r--   0 matheusslgd   (502) staff       (20)        0 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/tests/__init__.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     6759 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/tests/test_custom.py
+-rw-r--r--   0 matheusslgd   (502) staff       (20)     1327 2023-07-15 16:54:08.000000 jsm-autodynatrace-1.1.1/tests/test_django.py
```

### Comparing `jsm-autodynatrace-1.1.0/LICENSE` & `jsm-autodynatrace-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/PKG-INFO` & `jsm-autodynatrace-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsm-autodynatrace
-Version: 1.1.0
+Version: 1.1.1
 Summary: Auto instrumentation for the OneAgent SDK
 Home-page: https://github.com/juntossomosmais/OneAgent-SDK-Python-AutoInstrumentation
 Author: Juntos Somos Mais
 Author-email: labs@juntossomosmais.com.br
 Project-URL: Issue Tracker, https://github.com/juntossomosmais/OneAgent-SDK-Python-AutoInstrumentation/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `jsm-autodynatrace-1.1.0/README.md` & `jsm-autodynatrace-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/__init__.py` & `jsm-autodynatrace-1.1.1/autodynatrace/__init__.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/sdk.py` & `jsm-autodynatrace-1.1.1/autodynatrace/sdk.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/aiohttp/wrapper.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/aiohttp/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/bottle/wrapper.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/bottle/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/celery/wrapper.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/celery/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/concurrent/wrapper.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/concurrent/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/confluent_kafka/wrapper.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/confluent_kafka/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/custom/wrapper.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/custom/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/cx_Oracle/wrapper.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/cx_Oracle/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/dbapi/__init__.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django/db.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/django/db.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django/log.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/django/log.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django/middlewares.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/django/middlewares.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django/utils.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/django/utils.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django/wrapper.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/django/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django_outbox_pattern/consumer.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/django_outbox_pattern/consumer.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django_outbox_pattern/publisher.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/pika/wrapper.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,80 @@
-import oneagent
+import pika
 import wrapt
 
 from ...log import logger
 from ...sdk import sdk
-from django.conf import settings
-from django_outbox_pattern.producers import Producer
+
+import oneagent
 
 
-def instrument_publisher():
-    def on_send_message(wrapped, instance, args, kwargs):
+def instrument():
+    @wrapt.patch_function_wrapper("pika.channel", "Channel.basic_publish")
+    def basic_publish_dynatrace(wrapped, instance, args, kwargs):
+
         try:
-            host, port = settings.DJANGO_OUTBOX_PATTERN["DEFAULT_STOMP_HOST_AND_PORTS"][0]
-            destination = kwargs.get("destination")
-            headers = kwargs.get("headers", {})
+            host = instance.connection.params.host
+            port = instance.connection.params.port
+            exchange = kwargs.get("exchange")
+            routing_key = kwargs.get("routing_key")
 
         except Exception as e:
-            logger.warn("autodynatrace - Could not trace Publisher.send: {}".format(e))
-            return wrapped(**kwargs)
+            logger.warn("autodynatrace - could not instrument Channel.basic_publish: {}".format(e))
+            return wrapped(*args, **kwargs)
+
+        properties = kwargs.get("properties")
+        if properties is not None:
+            if properties.headers is None:
+                properties.headers = {}
+        else:
+            props = pika.BasicProperties(headers={})
+            kwargs["properties"] = props
 
         messaging_system = sdk.create_messaging_system_info(
-            oneagent.common.MessagingVendor.RABBIT_MQ,
-            destination,
+            "RabbitMQ",
+            routing_key,
             oneagent.common.MessagingDestinationType.QUEUE,
             oneagent.sdk.Channel(oneagent.sdk.ChannelType.TCP_IP, "{}:{}".format(host, port)),
         )
-
         with messaging_system:
-            with sdk.trace_outgoing_message(messaging_system) as outgoing_message:
-                outgoing_message.set_correlation_id(headers.get("correlation-id"))
-                tag = outgoing_message.outgoing_dynatrace_string_tag.decode("utf-8")
-                headers[oneagent.common.DYNATRACE_MESSAGE_PROPERTY_NAME] = tag
+            with sdk.trace_outgoing_message(messaging_system) as tracer:
+                tag = tracer.outgoing_dynatrace_string_tag.decode("utf-8")
+                kwargs["properties"].headers[oneagent.common.DYNATRACE_MESSAGE_PROPERTY_NAME] = tag
                 logger.debug(
-                    f"autodynatrace - Tracing Outgoing RabbitMQ host={host}, port={port}, routing_key={destination}, "
-                    f"tag={tag}, headers={headers}"
+                    "autodynatrace - Tracing RabbitMQ host={}, port={}, routing_key={}, tag={}".format(
+                        host, port, routing_key, tag
+                    )
                 )
-                return wrapped(**kwargs)
+                return wrapped(*args, **kwargs)
+
+    @wrapt.patch_function_wrapper("pika.adapters.blocking_connection", "BlockingChannel._on_consumer_message_delivery")
+    def on_message_callback_dynatrace(wrapped, instance, args, kwargs):
+
+        try:
+            channel, method_frame, header_frame, body = args
+            host = channel.connection.params.host
+            port = channel.connection.params.port
+            routing_key = method_frame.routing_key
+            exchange = method_frame.exchange
+            tag = None
+            if header_frame is not None and header_frame.headers is not None:
+                tag = header_frame.headers.get(oneagent.common.DYNATRACE_MESSAGE_PROPERTY_NAME, None)
 
-    wrapt.wrap_function_wrapper(Producer, "_send_with_retry", on_send_message)
+        except Exception as e:
+            logger.warn("autodynatrace - Could not trace BlockingChannel._on_consumer_message_delivery: {}".format(e))
+            return wrapped(*args, **kwargs)
+
+        messaging_system = sdk.create_messaging_system_info(
+            "RabbitMQ",
+            routing_key,
+            oneagent.common.MessagingDestinationType.QUEUE,
+            oneagent.sdk.Channel(oneagent.sdk.ChannelType.TCP_IP, "{}:{}".format(host, port)),
+        )
+        with messaging_system:
+            with sdk.trace_incoming_message_receive(messaging_system):
+                logger.debug(
+                    "autodynatrace - Tracing RabbitMQ host={}, port={}, routing_key={}, tag={}".format(
+                        host, port, routing_key, tag
+                    )
+                )
+                with sdk.trace_incoming_message_process(messaging_system, str_tag=tag):
+                    return wrapped(*args, **kwargs)
```

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django_stomp/consumer.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/django_stomp/consumer.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/django_stomp/publisher.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/django_stomp/publisher.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,19 +20,21 @@
         messaging_system = sdk.create_messaging_system_info(
             oneagent.common.MessagingVendor.RABBIT_MQ,
             destination,
             get_messaging_type_by_queue_name(destination),
             oneagent.sdk.Channel(oneagent.sdk.ChannelType.TCP_IP, "{}:{}".format(host, port)),
         )
 
+        tag = headers.get(oneagent.common.DYNATRACE_MESSAGE_PROPERTY_NAME, None)
         with messaging_system:
             with sdk.trace_outgoing_message(messaging_system) as outgoing_message:
                 outgoing_message.set_correlation_id(headers.get("correlation-id"))
-                tag = outgoing_message.outgoing_dynatrace_string_tag.decode("utf-8")
-                headers[oneagent.common.DYNATRACE_MESSAGE_PROPERTY_NAME] = tag
+                if not tag:
+                    tag = outgoing_message.outgoing_dynatrace_string_tag.decode("utf-8")
+                    headers[oneagent.common.DYNATRACE_MESSAGE_PROPERTY_NAME] = tag
                 logger.debug(
                     f"autodynatrace - Tracing Outgoing RabbitMQ host={host}, port={port}, routing_key={destination}, "
                     f"tag={tag}, headers={headers}"
                 )
                 return wrapped(*args, **kwargs)
 
     wrapt.wrap_function_wrapper(Publisher, "send", on_send_message)
```

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/fastapi/middleware.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/fastapi/middleware.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/fastapi/wrapper.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/fastapi/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/flask/wrapper.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/flask/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/grpc/wrapper.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/grpc/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/paramiko/wrapper.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/paramiko/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/psycopg2/wrapper.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/psycopg2/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/pymongo/wrapper.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/pymongo/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/pysnmp/wrapper.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/pysnmp/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/redis/utils.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/redis/utils.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/redis/wrapper.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/redis/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/sqlalchemy/wrapper.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/sqlalchemy/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/starlette/wrapper.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/starlette/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/subprocess/wrapper.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/subprocess/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/suds/wrapper.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/suds/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/tornado/wrapper.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/tornado/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/autodynatrace/wrappers/urllib/wrapper.py` & `jsm-autodynatrace-1.1.1/autodynatrace/wrappers/urllib/wrapper.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/jsm_autodynatrace.egg-info/PKG-INFO` & `jsm-autodynatrace-1.1.1/jsm_autodynatrace.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsm-autodynatrace
-Version: 1.1.0
+Version: 1.1.1
 Summary: Auto instrumentation for the OneAgent SDK
 Home-page: https://github.com/juntossomosmais/OneAgent-SDK-Python-AutoInstrumentation
 Author: Juntos Somos Mais
 Author-email: labs@juntossomosmais.com.br
 Project-URL: Issue Tracker, https://github.com/juntossomosmais/OneAgent-SDK-Python-AutoInstrumentation/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `jsm-autodynatrace-1.1.0/jsm_autodynatrace.egg-info/SOURCES.txt` & `jsm-autodynatrace-1.1.1/jsm_autodynatrace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/setup.py` & `jsm-autodynatrace-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="jsm-autodynatrace",
-    version="1.1.0",
+    version="1.1.1",
     packages=find_packages(),
     package_data={"autodynatrace": ["wrappers/*"]},
     install_requires=["wrapt>=1.11.2", "oneagent-sdk>=1.3.0", "six>=1.10.0", "autowrapt>=1.0"],
     tests_require=["pytest", "mock", "tox", "django"],
     entry_points={"autodynatrace": ["string = autodynatrace:load"]},
     python_requires=">=3.6",
     author="Juntos Somos Mais",
```

### Comparing `jsm-autodynatrace-1.1.0/tests/test_custom.py` & `jsm-autodynatrace-1.1.1/tests/test_custom.py`

 * *Files identical despite different names*

### Comparing `jsm-autodynatrace-1.1.0/tests/test_django.py` & `jsm-autodynatrace-1.1.1/tests/test_django.py`

 * *Files identical despite different names*

