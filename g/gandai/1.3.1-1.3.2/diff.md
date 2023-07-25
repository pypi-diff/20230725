# Comparing `tmp/gandai-1.3.1.tar.gz` & `tmp/gandai-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-1.3.1.tar", last modified: Sun Jul 23 20:21:01 2023, max compression
+gzip compressed data, was "gandai-1.3.2.tar", last modified: Tue Jul 25 17:03:00 2023, max compression
```

## Comparing `gandai-1.3.1.tar` & `gandai-1.3.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-23 20:21:01.322780 gandai-1.3.1/
--rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.3.1/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      214 2023-07-23 20:21:01.322665 gandai-1.3.1/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-23 20:21:01.316319 gandai-1.3.1/gandai/
--rw-r--r--   0 parker     (501) staff       (20)       46 2023-07-17 18:25:43.000000 gandai-1.3.1/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-23 20:21:01.320978 gandai-1.3.1/gandai/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      264 2023-07-17 18:43:09.000000 gandai-1.3.1/gandai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.3.1/gandai/__pycache__/adapters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2295 2023-07-19 22:26:33.000000 gandai-1.3.1/gandai/__pycache__/analytics.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-19 22:26:35.000000 gandai-1.3.1/gandai/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.3.1/gandai/__pycache__/datastore.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2014 2023-07-17 18:43:09.000000 gandai-1.3.1/gandai/__pycache__/db.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2095 2023-07-18 21:07:13.000000 gandai-1.3.1/gandai/__pycache__/gpt.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5979 2023-05-05 21:52:33.000000 gandai-1.3.1/gandai/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1373 2023-07-23 18:54:58.000000 gandai-1.3.1/gandai/__pycache__/helpers.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4285 2023-07-23 20:13:02.000000 gandai-1.3.1/gandai/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6151 2023-07-17 18:43:10.000000 gandai-1.3.1/gandai/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    31341 2023-07-23 19:40:55.000000 gandai-1.3.1/gandai/__pycache__/query.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2221 2023-07-17 18:43:09.000000 gandai-1.3.1/gandai/__pycache__/secrets.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.3.1/gandai/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    16053 2023-07-19 18:02:31.000000 gandai-1.3.1/gandai/__pycache__/sources.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1190 2023-07-17 18:25:43.000000 gandai-1.3.1/gandai/analytics.py
--rw-r--r--   0 parker     (501) staff       (20)     1822 2023-07-17 18:25:43.000000 gandai-1.3.1/gandai/auth.py
--rw-r--r--   0 parker     (501) staff       (20)     1492 2023-07-17 18:25:43.000000 gandai-1.3.1/gandai/datastore.py
--rw-r--r--   0 parker     (501) staff       (20)     1200 2023-07-17 18:25:43.000000 gandai-1.3.1/gandai/db.py
--rw-r--r--   0 parker     (501) staff       (20)     1025 2023-07-18 20:42:40.000000 gandai-1.3.1/gandai/gpt.py
--rw-r--r--   0 parker     (501) staff       (20)      402 2023-07-23 18:54:56.000000 gandai-1.3.1/gandai/helpers.py
--rw-r--r--   0 parker     (501) staff       (20)     3030 2023-07-23 20:20:45.000000 gandai-1.3.1/gandai/main.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-23 20:21:01.321648 gandai-1.3.1/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.3.1/gandai/migrations/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-23 20:21:01.322024 gandai-1.3.1/gandai/migrations/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.3.1/gandai/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.3.1/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.3.1/gandai/migrations/db_create.py
--rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.3.1/gandai/migrations/db_seed.py
--rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.3.1/gandai/migrations/dealcloud.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-23 20:21:01.322493 gandai-1.3.1/gandai/migrations/sql/
--rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.3.1/gandai/migrations/sql/2305023-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     3061 2023-07-17 18:25:43.000000 gandai-1.3.1/gandai/migrations/sql/schema.sql
--rw-r--r--   0 parker     (501) staff       (20)     2683 2023-07-17 18:25:43.000000 gandai-1.3.1/gandai/models.py
--rw-r--r--   0 parker     (501) staff       (20)    20989 2023-07-23 19:40:52.000000 gandai-1.3.1/gandai/query.py
--rw-r--r--   0 parker     (501) staff       (20)     1069 2023-07-17 18:25:43.000000 gandai-1.3.1/gandai/secrets.py
--rw-r--r--   0 parker     (501) staff       (20)    10781 2023-07-18 21:32:33.000000 gandai-1.3.1/gandai/sources.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-23 20:21:01.317295 gandai-1.3.1/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      214 2023-07-23 20:21:01.000000 gandai-1.3.1/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     1295 2023-07-23 20:21:01.000000 gandai-1.3.1/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2023-07-23 20:21:01.000000 gandai-1.3.1/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2023-07-23 20:21:01.000000 gandai-1.3.1/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      383 2023-07-23 20:20:55.000000 gandai-1.3.1/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2023-07-23 20:21:01.322813 gandai-1.3.1/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.3.1/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 17:03:00.176863 gandai-1.3.2/
+-rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.3.2/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      214 2023-07-25 17:03:00.176731 gandai-1.3.2/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 17:03:00.171607 gandai-1.3.2/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)       46 2023-07-17 18:25:43.000000 gandai-1.3.2/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 17:03:00.175081 gandai-1.3.2/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      264 2023-07-17 18:43:09.000000 gandai-1.3.2/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.3.2/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4120 2023-07-25 17:01:01.000000 gandai-1.3.2/gandai/__pycache__/analytics.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-19 22:26:35.000000 gandai-1.3.2/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.3.2/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2014 2023-07-17 18:43:09.000000 gandai-1.3.2/gandai/__pycache__/db.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2095 2023-07-18 21:07:13.000000 gandai-1.3.2/gandai/__pycache__/gpt.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5979 2023-05-05 21:52:33.000000 gandai-1.3.2/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1373 2023-07-23 18:54:58.000000 gandai-1.3.2/gandai/__pycache__/helpers.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4285 2023-07-25 16:56:41.000000 gandai-1.3.2/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6151 2023-07-17 18:43:10.000000 gandai-1.3.2/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    31447 2023-07-25 15:24:42.000000 gandai-1.3.2/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2221 2023-07-17 18:43:09.000000 gandai-1.3.2/gandai/__pycache__/secrets.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.3.2/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    15985 2023-07-23 23:17:10.000000 gandai-1.3.2/gandai/__pycache__/sources.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2368 2023-07-25 17:01:00.000000 gandai-1.3.2/gandai/analytics.py
+-rw-r--r--   0 parker     (501) staff       (20)     1822 2023-07-17 18:25:43.000000 gandai-1.3.2/gandai/auth.py
+-rw-r--r--   0 parker     (501) staff       (20)     1492 2023-07-17 18:25:43.000000 gandai-1.3.2/gandai/datastore.py
+-rw-r--r--   0 parker     (501) staff       (20)     1200 2023-07-17 18:25:43.000000 gandai-1.3.2/gandai/db.py
+-rw-r--r--   0 parker     (501) staff       (20)     1025 2023-07-18 20:42:40.000000 gandai-1.3.2/gandai/gpt.py
+-rw-r--r--   0 parker     (501) staff       (20)      402 2023-07-23 18:54:56.000000 gandai-1.3.2/gandai/helpers.py
+-rw-r--r--   0 parker     (501) staff       (20)     3030 2023-07-23 20:20:45.000000 gandai-1.3.2/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 17:03:00.175600 gandai-1.3.2/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.3.2/gandai/migrations/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 17:03:00.175951 gandai-1.3.2/gandai/migrations/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.3.2/gandai/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.3.2/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.3.2/gandai/migrations/db_create.py
+-rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.3.2/gandai/migrations/db_seed.py
+-rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.3.2/gandai/migrations/dealcloud.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 17:03:00.176542 gandai-1.3.2/gandai/migrations/sql/
+-rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.3.2/gandai/migrations/sql/2305023-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     3061 2023-07-17 18:25:43.000000 gandai-1.3.2/gandai/migrations/sql/schema.sql
+-rw-r--r--   0 parker     (501) staff       (20)     2683 2023-07-17 18:25:43.000000 gandai-1.3.2/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)    21051 2023-07-25 13:22:33.000000 gandai-1.3.2/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)     1069 2023-07-17 18:25:43.000000 gandai-1.3.2/gandai/secrets.py
+-rw-r--r--   0 parker     (501) staff       (20)    10783 2023-07-23 23:17:02.000000 gandai-1.3.2/gandai/sources.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 17:03:00.172541 gandai-1.3.2/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      214 2023-07-25 17:03:00.000000 gandai-1.3.2/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1295 2023-07-25 17:03:00.000000 gandai-1.3.2/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2023-07-25 17:03:00.000000 gandai-1.3.2/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2023-07-25 17:03:00.000000 gandai-1.3.2/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      383 2023-07-25 17:02:53.000000 gandai-1.3.2/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2023-07-25 17:03:00.176901 gandai-1.3.2/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.3.2/setup.py
```

### Comparing `gandai-1.3.1/gandai/__pycache__/adapters.cpython-311.pyc` & `gandai-1.3.2/gandai/__pycache__/adapters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.1/gandai/__pycache__/auth.cpython-311.pyc` & `gandai-1.3.2/gandai/__pycache__/auth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.1/gandai/__pycache__/datastore.cpython-311.pyc` & `gandai-1.3.2/gandai/__pycache__/datastore.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.1/gandai/__pycache__/db.cpython-311.pyc` & `gandai-1.3.2/gandai/__pycache__/db.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.1/gandai/__pycache__/gpt.cpython-311.pyc` & `gandai-1.3.2/gandai/__pycache__/gpt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.1/gandai/__pycache__/grata.cpython-311.pyc` & `gandai-1.3.2/gandai/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.1/gandai/__pycache__/helpers.cpython-311.pyc` & `gandai-1.3.2/gandai/__pycache__/helpers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.1/gandai/__pycache__/main.cpython-311.pyc` & `gandai-1.3.2/gandai/__pycache__/main.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xcd89bd64 (Sun Jul 23 20:13:01 2023 UTC)
+moddate:  0x9d8bbd64 (Sun Jul 23 20:20:45 2023 UTC)
 files sz: 3030
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `gandai-1.3.1/gandai/__pycache__/models.cpython-311.pyc` & `gandai-1.3.2/gandai/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.1/gandai/__pycache__/query.cpython-311.pyc` & `gandai-1.3.2/gandai/__pycache__/query.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x4482bd64 (Sun Jul 23 19:40:52 2023 UTC)
-files sz: 20989
+moddate:  0x99ccbf64 (Tue Jul 25 13:22:33 2023 UTC)
+files sz: 21051
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064036c036d
@@ -1947,15 +1947,17 @@
             000000000000007c0664056406ac07a6030000ab0300000000000000007d
             057417000000000000000000007c00a6010000ab0100000000000000007d
             077c05a00c00000000000000000000000000000000000000007c076a0d00
             00000000000000a00e000000000000000000000000000000000000000064
             086405a6020000ab0200000000000000007c076a0d0000000000000000a0
             0e00000000000000000000000000000000000000006409a6010000ab0100
             00000000000000640a6b0200000000ac0ba6020000ab0200000000000000
-            007d057c055300
+            007d05740b000000000000000000006a0f00000000000000007c05640c19
+            000000000000000000a6010000ab0100000000000000007c05640c3c0000
+            007c055300
          325           0 RESUME                   0
          
          326           2 LOAD_CONST               1 ("\n        SELECT \n            e.id, \n            e.search_uid, \n            e.domain, \n            e.data, \n            e.type AS last_event_type, \n            e.created AS updated,\n            a.name AS updated_by,\n            c.name as name,\n            c.uid as dealcloud_id,\n            c.description as description,\n            c.meta as meta,\n            (c.meta->>'employees') AS employees,\n            (c.meta->>'ownership') AS ownership,\n            (c.meta->>'linkedin') AS linkedin,\n            (r.data->>'rating') AS rating\n        FROM (\n            SELECT \n                search_uid, \n                domain, \n                MAX(created) AS max_created\n            FROM \n                event\n            WHERE \n                type NOT IN ('comment','rating','generate','criteria')\n                AND search_uid = :search_uid\n            GROUP BY \n                domain, search_uid\n        ) AS max_event\n        JOIN event e ON e.domain = max_event.domain AND e.created = max_event.max_created AND e.search_uid = max_event.search_uid \n        JOIN company c ON c.domain = e.domain\n        JOIN actor a ON a.key = e.actor_key\n        LEFT JOIN (\n            SELECT \n                search_uid,\n                domain, \n                MAX(created) AS max_created\n            FROM \n                event\n            WHERE \n                type = 'rating'\n            GROUP BY \n                domain, search_uid\n        ) AS max_rating ON e.domain = max_rating.domain AND e.search_uid = max_rating.search_uid\n        LEFT JOIN event r ON r.domain = max_rating.domain AND r.created = max_rating.max_created;\n    ")
                        4 STORE_FAST               2 (statement)
          
          373           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
@@ -2068,16 +2070,27 @@
                      578 COMPARE_OP               2 (==)
          
          386         584 KW_NAMES                11
                      586 PRECALL                  2
                      590 CALL                     2
                      600 STORE_FAST               5 (targets)
          
-         391         602 LOAD_FAST                5 (targets)
-                     604 RETURN_VALUE
+         390         602 LOAD_GLOBAL             11 (NULL + pd)
+                     614 LOAD_ATTR               15 (to_numeric)
+                     624 LOAD_FAST                5 (targets)
+                     626 LOAD_CONST              12 ('employees')
+                     628 BINARY_SUBSCR
+                     638 PRECALL                  1
+                     642 CALL                     1
+                     652 LOAD_FAST                5 (targets)
+                     654 LOAD_CONST              12 ('employees')
+                     656 STORE_SUBSCR
+         
+         391         660 LOAD_FAST                5 (targets)
+                     662 RETURN_VALUE
          ExceptionTable:
            56 to 258 -> 284 [1] lasti
            284 to 290 -> 292 [3] lasti
            298 to 298 -> 292 [3] lasti
          consts
             None
             "\n        SELECT \n            e.id, \n            e.search_uid, \n            e.domain, \n            e.data, \n            e.type AS last_event_type, \n            e.created AS updated,\n            a.name AS updated_by,\n            c.name as name,\n            c.uid as dealcloud_id,\n            c.description as description,\n            c.meta as meta,\n            (c.meta->>'employees') AS employees,\n            (c.meta->>'ownership') AS ownership,\n            (c.meta->>'linkedin') AS linkedin,\n            (r.data->>'rating') AS rating\n        FROM (\n            SELECT \n                search_uid, \n                domain, \n                MAX(created) AS max_created\n            FROM \n                event\n            WHERE \n                type NOT IN ('comment','rating','generate','criteria')\n                AND search_uid = :search_uid\n            GROUP BY \n                domain, search_uid\n        ) AS max_event\n        JOIN event e ON e.domain = max_event.domain AND e.created = max_event.max_created AND e.search_uid = max_event.search_uid \n        JOIN company c ON c.domain = e.domain\n        JOIN actor a ON a.key = e.actor_key\n        LEFT JOIN (\n            SELECT \n                search_uid,\n                domain, \n                MAX(created) AS max_created\n            FROM \n                event\n            WHERE \n                type = 'rating'\n            GROUP BY \n                domain, search_uid\n        ) AS max_rating ON e.domain = max_rating.domain AND e.search_uid = max_rating.search_uid\n        LEFT JOIN event r ON r.domain = max_rating.domain AND r.created = max_rating.max_created;\n    "
@@ -2087,24 +2100,25 @@
             'domain'
             'left'
             ('on', 'how')
             'field'
             'order'
             'asc'
             ('by', 'ascending')
-         names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'comment_by_domain', 'merge', 'find_search_by_uid', 'sort_values', 'sort', 'get')
+            'employees'
+         names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'comment_by_domain', 'merge', 'find_search_by_uid', 'sort_values', 'sort', 'get', 'to_numeric')
          varnames   ('search_uid', 'last_event_type', 'statement', 'conn', 'result', 'targets', 'comments', 'search')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search_target_by_last_event_type'
          firstlineno 325
          lnotab
             0x0201042f34011801260108fe100474fb2e0724011e0130031e01180134
-            013afe1205
+            013afe12043a01
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
             0x970064017d01740000000000000000000000a001000000000000000000
```

### Comparing `gandai-1.3.1/gandai/__pycache__/secrets.cpython-311.pyc` & `gandai-1.3.2/gandai/__pycache__/secrets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.1/gandai/__pycache__/services.cpython-311.pyc` & `gandai-1.3.2/gandai/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.1/gandai/__pycache__/sources.cpython-311.pyc` & `gandai-1.3.2/gandai/__pycache__/sources.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xf104b764 (Tue Jul 18 21:32:33 2023 UTC)
-files sz: 10781
+moddate:  0xeeb4bd64 (Sun Jul 23 23:17:02 2023 UTC)
+files sz: 10783
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064036c036d
@@ -1358,18 +1358,17 @@
                code
                   0x9700740000000000000000000000a00100000000000000000000000000
                   000000000000007c01a6010000ab0100000000000000007d027405000000
                   000000000000006a03000000000000000064017400000000000000000000
                   006a0400000000000000007c007c026402190000000000000000007c0264
                   031900000000000000000064049c03ac05a6030000ab0300000000000000
                   007d037c03a0050000000000000000000000000000000000000000a60000
-                  00ab0000000000000000007d04740d0000000000000000000064067c04a6
-                  020000ab02000000000000000001007c04a0070000000000000000000000
-                  00000000000000000064076700a6020000ab0200000000000000007c0464
-                  083c0000007c046408190000000000000000005300
+                  00ab0000000000000000007d047c04a00600000000000000000000000000
+                  0000000000000064066700a6020000ab0200000000000000007c0464073c
+                  0000007c046407190000000000000000005300
                177           0 RESUME                   0
                
                178           2 LOAD_GLOBAL              0 (GrataWrapper)
                             14 LOAD_METHOD              1 (_get_api_filter)
                             36 LOAD_FAST                1 (search)
                             38 PRECALL                  1
                             42 CALL                     1
@@ -1405,55 +1404,45 @@
                
                190         152 LOAD_FAST                3 (response)
                            154 LOAD_METHOD              5 (json)
                            176 PRECALL                  0
                            180 CALL                     0
                            190 STORE_FAST               4 (data)
                
-               191         192 LOAD_GLOBAL             13 (NULL + print)
-                           204 LOAD_CONST               6 ('find_similar:')
-                           206 LOAD_FAST                4 (data)
-                           208 PRECALL                  2
-                           212 CALL                     2
-                           222 POP_TOP
-               
-               192         224 LOAD_FAST                4 (data)
-                           226 LOAD_METHOD              7 (get)
-                           248 LOAD_CONST               7 ('results')
-                           250 BUILD_LIST               0
-                           252 PRECALL                  2
-                           256 CALL                     2
-                           266 LOAD_FAST                4 (data)
-                           268 LOAD_CONST               8 ('companies')
-                           270 STORE_SUBSCR
-               
-               194         274 LOAD_FAST                4 (data)
-                           276 LOAD_CONST               8 ('companies')
-                           278 BINARY_SUBSCR
-                           288 RETURN_VALUE
+               192         192 LOAD_FAST                4 (data)
+                           194 LOAD_METHOD              6 (get)
+                           216 LOAD_CONST               6 ('results')
+                           218 BUILD_LIST               0
+                           220 PRECALL                  2
+                           224 CALL                     2
+                           234 LOAD_FAST                4 (data)
+                           236 LOAD_CONST               7 ('companies')
+                           238 STORE_SUBSCR
+               
+               194         242 LOAD_FAST                4 (data)
+                           244 LOAD_CONST               7 ('companies')
+                           246 BINARY_SUBSCR
+                           256 RETURN_VALUE
                consts
                   None
                   'https://search.grata.com/api/v1.2/search-similar/'
                   'grata_employees_estimates_range'
                   'headquarters'
                   ('domain', 'grata_employees_estimates_range', 'headquarters')
                   ('headers', 'json')
-                  'find_similar:'
                   'results'
                   'companies'
-               names      ('GrataWrapper', '_get_api_filter', 'requests', 'post', 'HEADERS', 'json', 'print', 'get')
+               names      ('GrataWrapper', '_get_api_filter', 'requests', 'post', 'HEADERS', 'json', 'get')
                varnames   ('domain', 'search', 'api_filters', 'response', 'data')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'find_similar'
                firstlineno 177
-               lnotab
-                  0x020134011601020116020201020102ff0a030efb04fd120b2801200132
-                  02
+               lnotab 0x020134011601020116020201020102ff0a030efb04fd120b28023202
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 5
                flags     : 3
                code
                   0x9700740000000000000000000000a00100000000000000000000000000
```

### Comparing `gandai-1.3.1/gandai/auth.py` & `gandai-1.3.2/gandai/auth.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.1/gandai/datastore.py` & `gandai-1.3.2/gandai/datastore.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.1/gandai/db.py` & `gandai-1.3.2/gandai/db.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.1/gandai/gpt.py` & `gandai-1.3.2/gandai/gpt.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.1/gandai/main.py` & `gandai-1.3.2/gandai/main.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.1/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc` & `gandai-1.3.2/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.1/gandai/migrations/db_seed.py` & `gandai-1.3.2/gandai/migrations/db_seed.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.1/gandai/migrations/dealcloud.py` & `gandai-1.3.2/gandai/migrations/dealcloud.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.1/gandai/migrations/sql/schema.sql` & `gandai-1.3.2/gandai/migrations/sql/schema.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.3.1/gandai/models.py` & `gandai-1.3.2/gandai/models.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.1/gandai/query.py` & `gandai-1.3.2/gandai/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -383,15 +383,15 @@
 
     # handle sorting
     search = find_search_by_uid(search_uid)
     targets = targets.sort_values(
         by=search.sort.get("field", "domain"),
         ascending=search.sort.get("order") == "asc",
     )
-
+    targets['employees'] = pd.to_numeric(targets['employees'])
     return targets
 
 
 def search_target_export(search_uid: int) -> pd.DataFrame:
     """Returns all the targets not in rejected or created"""
 
     statement = """
```

### Comparing `gandai-1.3.1/gandai/secrets.py` & `gandai-1.3.2/gandai/secrets.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.1/gandai/sources.py` & `gandai-1.3.2/gandai/sources.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
                 "grata_employees_estimates_range": api_filters[
                     "grata_employees_estimates_range"
                 ],
                 "headquarters": api_filters["headquarters"],
             },
         )
         data = response.json()
-        print("find_similar:", data)
+        # print("find_similar:", data)
         data["companies"] = data.get("results", [])  # asking grata about this
 
         return data["companies"]
 
     def find_by_criteria(search: models.Search) -> dict:
         api_filters = GrataWrapper._get_api_filter(search)
         response = requests.post(
```

### Comparing `gandai-1.3.1/gandai.egg-info/SOURCES.txt` & `gandai-1.3.2/gandai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

