# Comparing `tmp/gandai-1.3.2.tar.gz` & `tmp/gandai-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-1.3.2.tar", last modified: Tue Jul 25 17:03:00 2023, max compression
+gzip compressed data, was "gandai-1.3.3.tar", last modified: Tue Jul 25 20:20:29 2023, max compression
```

## Comparing `gandai-1.3.2.tar` & `gandai-1.3.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 17:03:00.176863 gandai-1.3.2/
--rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.3.2/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      214 2023-07-25 17:03:00.176731 gandai-1.3.2/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 17:03:00.171607 gandai-1.3.2/gandai/
--rw-r--r--   0 parker     (501) staff       (20)       46 2023-07-17 18:25:43.000000 gandai-1.3.2/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 17:03:00.175081 gandai-1.3.2/gandai/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      264 2023-07-17 18:43:09.000000 gandai-1.3.2/gandai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.3.2/gandai/__pycache__/adapters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4120 2023-07-25 17:01:01.000000 gandai-1.3.2/gandai/__pycache__/analytics.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-19 22:26:35.000000 gandai-1.3.2/gandai/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.3.2/gandai/__pycache__/datastore.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2014 2023-07-17 18:43:09.000000 gandai-1.3.2/gandai/__pycache__/db.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2095 2023-07-18 21:07:13.000000 gandai-1.3.2/gandai/__pycache__/gpt.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5979 2023-05-05 21:52:33.000000 gandai-1.3.2/gandai/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1373 2023-07-23 18:54:58.000000 gandai-1.3.2/gandai/__pycache__/helpers.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4285 2023-07-25 16:56:41.000000 gandai-1.3.2/gandai/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6151 2023-07-17 18:43:10.000000 gandai-1.3.2/gandai/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    31447 2023-07-25 15:24:42.000000 gandai-1.3.2/gandai/__pycache__/query.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2221 2023-07-17 18:43:09.000000 gandai-1.3.2/gandai/__pycache__/secrets.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.3.2/gandai/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    15985 2023-07-23 23:17:10.000000 gandai-1.3.2/gandai/__pycache__/sources.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2368 2023-07-25 17:01:00.000000 gandai-1.3.2/gandai/analytics.py
--rw-r--r--   0 parker     (501) staff       (20)     1822 2023-07-17 18:25:43.000000 gandai-1.3.2/gandai/auth.py
--rw-r--r--   0 parker     (501) staff       (20)     1492 2023-07-17 18:25:43.000000 gandai-1.3.2/gandai/datastore.py
--rw-r--r--   0 parker     (501) staff       (20)     1200 2023-07-17 18:25:43.000000 gandai-1.3.2/gandai/db.py
--rw-r--r--   0 parker     (501) staff       (20)     1025 2023-07-18 20:42:40.000000 gandai-1.3.2/gandai/gpt.py
--rw-r--r--   0 parker     (501) staff       (20)      402 2023-07-23 18:54:56.000000 gandai-1.3.2/gandai/helpers.py
--rw-r--r--   0 parker     (501) staff       (20)     3030 2023-07-23 20:20:45.000000 gandai-1.3.2/gandai/main.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 17:03:00.175600 gandai-1.3.2/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.3.2/gandai/migrations/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 17:03:00.175951 gandai-1.3.2/gandai/migrations/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.3.2/gandai/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.3.2/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.3.2/gandai/migrations/db_create.py
--rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.3.2/gandai/migrations/db_seed.py
--rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.3.2/gandai/migrations/dealcloud.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 17:03:00.176542 gandai-1.3.2/gandai/migrations/sql/
--rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.3.2/gandai/migrations/sql/2305023-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     3061 2023-07-17 18:25:43.000000 gandai-1.3.2/gandai/migrations/sql/schema.sql
--rw-r--r--   0 parker     (501) staff       (20)     2683 2023-07-17 18:25:43.000000 gandai-1.3.2/gandai/models.py
--rw-r--r--   0 parker     (501) staff       (20)    21051 2023-07-25 13:22:33.000000 gandai-1.3.2/gandai/query.py
--rw-r--r--   0 parker     (501) staff       (20)     1069 2023-07-17 18:25:43.000000 gandai-1.3.2/gandai/secrets.py
--rw-r--r--   0 parker     (501) staff       (20)    10783 2023-07-23 23:17:02.000000 gandai-1.3.2/gandai/sources.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 17:03:00.172541 gandai-1.3.2/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      214 2023-07-25 17:03:00.000000 gandai-1.3.2/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     1295 2023-07-25 17:03:00.000000 gandai-1.3.2/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2023-07-25 17:03:00.000000 gandai-1.3.2/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2023-07-25 17:03:00.000000 gandai-1.3.2/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      383 2023-07-25 17:02:53.000000 gandai-1.3.2/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2023-07-25 17:03:00.176901 gandai-1.3.2/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.3.2/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 20:20:29.783630 gandai-1.3.3/
+-rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.3.3/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      214 2023-07-25 20:20:29.783521 gandai-1.3.3/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 20:20:29.779063 gandai-1.3.3/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)       46 2023-07-17 18:25:43.000000 gandai-1.3.3/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 20:20:29.781994 gandai-1.3.3/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      264 2023-07-17 18:43:09.000000 gandai-1.3.3/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.3.3/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4120 2023-07-25 17:01:01.000000 gandai-1.3.3/gandai/__pycache__/analytics.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-19 22:26:35.000000 gandai-1.3.3/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.3.3/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2014 2023-07-17 18:43:09.000000 gandai-1.3.3/gandai/__pycache__/db.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3757 2023-07-25 19:02:34.000000 gandai-1.3.3/gandai/__pycache__/gpt.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5979 2023-05-05 21:52:33.000000 gandai-1.3.3/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1373 2023-07-23 18:54:58.000000 gandai-1.3.3/gandai/__pycache__/helpers.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4285 2023-07-25 16:56:41.000000 gandai-1.3.3/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6151 2023-07-17 18:43:10.000000 gandai-1.3.3/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    31858 2023-07-25 20:16:58.000000 gandai-1.3.3/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2221 2023-07-17 18:43:09.000000 gandai-1.3.3/gandai/__pycache__/secrets.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.3.3/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    15985 2023-07-23 23:17:10.000000 gandai-1.3.3/gandai/__pycache__/sources.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2368 2023-07-25 17:01:00.000000 gandai-1.3.3/gandai/analytics.py
+-rw-r--r--   0 parker     (501) staff       (20)     1822 2023-07-17 18:25:43.000000 gandai-1.3.3/gandai/auth.py
+-rw-r--r--   0 parker     (501) staff       (20)     1492 2023-07-17 18:25:43.000000 gandai-1.3.3/gandai/datastore.py
+-rw-r--r--   0 parker     (501) staff       (20)     1200 2023-07-17 18:25:43.000000 gandai-1.3.3/gandai/db.py
+-rw-r--r--   0 parker     (501) staff       (20)     1631 2023-07-25 19:02:05.000000 gandai-1.3.3/gandai/gpt.py
+-rw-r--r--   0 parker     (501) staff       (20)      402 2023-07-23 18:54:56.000000 gandai-1.3.3/gandai/helpers.py
+-rw-r--r--   0 parker     (501) staff       (20)     3030 2023-07-23 20:20:45.000000 gandai-1.3.3/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 20:20:29.782510 gandai-1.3.3/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.3.3/gandai/migrations/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 20:20:29.782867 gandai-1.3.3/gandai/migrations/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.3.3/gandai/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.3.3/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.3.3/gandai/migrations/db_create.py
+-rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.3.3/gandai/migrations/db_seed.py
+-rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.3.3/gandai/migrations/dealcloud.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 20:20:29.783335 gandai-1.3.3/gandai/migrations/sql/
+-rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.3.3/gandai/migrations/sql/2305023-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     3061 2023-07-17 18:25:43.000000 gandai-1.3.3/gandai/migrations/sql/schema.sql
+-rw-r--r--   0 parker     (501) staff       (20)     2683 2023-07-17 18:25:43.000000 gandai-1.3.3/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)    20866 2023-07-25 20:16:56.000000 gandai-1.3.3/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)     1069 2023-07-17 18:25:43.000000 gandai-1.3.3/gandai/secrets.py
+-rw-r--r--   0 parker     (501) staff       (20)    10783 2023-07-23 23:17:02.000000 gandai-1.3.3/gandai/sources.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 20:20:29.779644 gandai-1.3.3/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      214 2023-07-25 20:20:29.000000 gandai-1.3.3/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1295 2023-07-25 20:20:29.000000 gandai-1.3.3/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2023-07-25 20:20:29.000000 gandai-1.3.3/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2023-07-25 20:20:29.000000 gandai-1.3.3/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      383 2023-07-25 20:20:20.000000 gandai-1.3.3/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2023-07-25 20:20:29.783660 gandai-1.3.3/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.3.3/setup.py
```

### Comparing `gandai-1.3.2/gandai/__pycache__/adapters.cpython-311.pyc` & `gandai-1.3.3/gandai/__pycache__/adapters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.2/gandai/__pycache__/analytics.cpython-311.pyc` & `gandai-1.3.3/gandai/__pycache__/analytics.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.2/gandai/__pycache__/auth.cpython-311.pyc` & `gandai-1.3.3/gandai/__pycache__/auth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.2/gandai/__pycache__/datastore.cpython-311.pyc` & `gandai-1.3.3/gandai/__pycache__/datastore.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.2/gandai/__pycache__/db.cpython-311.pyc` & `gandai-1.3.3/gandai/__pycache__/db.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.2/gandai/__pycache__/grata.cpython-311.pyc` & `gandai-1.3.3/gandai/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.2/gandai/__pycache__/helpers.cpython-311.pyc` & `gandai-1.3.3/gandai/__pycache__/helpers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.2/gandai/__pycache__/main.cpython-311.pyc` & `gandai-1.3.3/gandai/__pycache__/main.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.2/gandai/__pycache__/models.cpython-311.pyc` & `gandai-1.3.3/gandai/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.2/gandai/__pycache__/query.cpython-311.pyc` & `gandai-1.3.3/gandai/__pycache__/query.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x99ccbf64 (Tue Jul 25 13:22:33 2023 UTC)
-files sz: 21051
+moddate:  0xb82dc064 (Tue Jul 25 20:16:56 2023 UTC)
+files sz: 20866
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064036c036d
@@ -194,185 +194,185 @@
    107         292 LOAD_CONST               1 (None)
    
    105         294 BUILD_TUPLE             10
                296 LOAD_CONST              25 (<code object insert_targets_from_domains, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 105>)
                298 MAKE_FUNCTION            4 (annotations)
                300 STORE_NAME              34 (insert_targets_from_domains)
    
-   160         302 LOAD_CONST              26 ('companies')
+   157         302 LOAD_CONST              26 ('companies')
    
-   161         304 LOAD_NAME                5 (List)
+   158         304 LOAD_NAME                5 (List)
                306 LOAD_NAME                4 (Any)
                308 BINARY_SUBSCR
    
-   160         318 LOAD_CONST              22 ('search_uid')
+   157         318 LOAD_CONST              22 ('search_uid')
    
-   161         320 LOAD_NAME               33 (int)
+   158         320 LOAD_NAME               33 (int)
    
-   160         322 LOAD_CONST              23 ('actor_key')
+   157         322 LOAD_CONST              23 ('actor_key')
    
-   161         324 LOAD_NAME               32 (str)
+   158         324 LOAD_NAME               32 (str)
    
-   160         326 LOAD_CONST              13 ('return')
+   157         326 LOAD_CONST              13 ('return')
    
-   162         328 LOAD_CONST               1 (None)
+   159         328 LOAD_CONST               1 (None)
    
-   160         330 BUILD_TUPLE              8
-               332 LOAD_CONST              27 (<code object insert_companies_as_targets, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 160>)
+   157         330 BUILD_TUPLE              8
+               332 LOAD_CONST              27 (<code object insert_companies_as_targets, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 157>)
                334 MAKE_FUNCTION            4 (annotations)
                336 STORE_NAME              35 (insert_companies_as_targets)
    
-   215         338 LOAD_CONST              13 ('return')
+   211         338 LOAD_CONST              13 ('return')
                340 LOAD_NAME                7 (pd)
                342 LOAD_ATTR               36 (DataFrame)
                352 BUILD_TUPLE              2
-               354 LOAD_CONST              28 (<code object top_actor_per_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 215>)
+               354 LOAD_CONST              28 (<code object top_actor_per_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 211>)
                356 MAKE_FUNCTION            4 (annotations)
                358 STORE_NAME              37 (top_actor_per_search)
    
-   253         360 LOAD_CONST              13 ('return')
+   249         360 LOAD_CONST              13 ('return')
                362 LOAD_NAME                7 (pd)
                364 LOAD_ATTR               36 (DataFrame)
                374 BUILD_TUPLE              2
-               376 LOAD_CONST              29 (<code object search_event_count_by_type, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 253>)
+               376 LOAD_CONST              29 (<code object search_event_count_by_type, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 249>)
                378 MAKE_FUNCTION            4 (annotations)
                380 STORE_NAME              38 (search_event_count_by_type)
    
-   269         382 LOAD_CONST              30 (<code object search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 269>)
+   265         382 LOAD_CONST              30 (<code object search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 265>)
                384 MAKE_FUNCTION            0
                386 STORE_NAME              39 (search)
    
-   311         388 LOAD_CONST              13 ('return')
+   307         388 LOAD_CONST              13 ('return')
                390 LOAD_NAME                7 (pd)
                392 LOAD_ATTR               36 (DataFrame)
                402 BUILD_TUPLE              2
-               404 LOAD_CONST              31 (<code object actor, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 311>)
+               404 LOAD_CONST              31 (<code object actor, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 307>)
                406 MAKE_FUNCTION            4 (annotations)
                408 STORE_NAME              40 (actor)
    
-   325         410 LOAD_CONST              47 ((None,))
+   321         410 LOAD_CONST              47 ((None,))
                412 LOAD_CONST              22 ('search_uid')
                414 LOAD_NAME               33 (int)
                416 LOAD_CONST              24 ('last_event_type')
                418 LOAD_NAME               32 (str)
                420 BUILD_TUPLE              4
-               422 LOAD_CONST              32 (<code object search_target_by_last_event_type, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 325>)
+               422 LOAD_CONST              32 (<code object search_target_by_last_event_type, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 321>)
                424 MAKE_FUNCTION            5 (defaults, annotations)
                426 STORE_NAME              41 (search_target_by_last_event_type)
    
-   394         428 LOAD_CONST              22 ('search_uid')
+   390         428 LOAD_CONST              22 ('search_uid')
                430 LOAD_NAME               33 (int)
                432 LOAD_CONST              13 ('return')
                434 LOAD_NAME                7 (pd)
                436 LOAD_ATTR               36 (DataFrame)
                446 BUILD_TUPLE              4
-               448 LOAD_CONST              33 (<code object search_target_export, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 394>)
+               448 LOAD_CONST              33 (<code object search_target_export, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 390>)
                450 MAKE_FUNCTION            4 (annotations)
                452 STORE_NAME              42 (search_target_export)
    
-   453         454 LOAD_CONST              22 ('search_uid')
+   449         454 LOAD_CONST              22 ('search_uid')
                456 LOAD_NAME               33 (int)
                458 LOAD_CONST              13 ('return')
                460 LOAD_NAME                7 (pd)
                462 LOAD_ATTR               36 (DataFrame)
                472 BUILD_TUPLE              4
-               474 LOAD_CONST              34 (<code object target_count, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 453>)
+               474 LOAD_CONST              34 (<code object target_count, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 449>)
                476 MAKE_FUNCTION            4 (annotations)
                478 STORE_NAME              43 (target_count)
    
-   483         480 LOAD_CONST              22 ('search_uid')
+   479         480 LOAD_CONST              22 ('search_uid')
                482 LOAD_NAME               33 (int)
                484 LOAD_CONST              13 ('return')
                486 LOAD_NAME                7 (pd)
                488 LOAD_ATTR               36 (DataFrame)
                498 BUILD_TUPLE              4
-               500 LOAD_CONST              35 (<code object event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 483>)
+               500 LOAD_CONST              35 (<code object event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 479>)
                502 MAKE_FUNCTION            4 (annotations)
                504 STORE_NAME              44 (event)
    
-   495         506 LOAD_CONST              22 ('search_uid')
+   491         506 LOAD_CONST              22 ('search_uid')
                508 LOAD_NAME               33 (int)
                510 LOAD_CONST              13 ('return')
                512 LOAD_NAME                7 (pd)
                514 LOAD_ATTR               36 (DataFrame)
                524 BUILD_TUPLE              4
-               526 LOAD_CONST              36 (<code object unique_domains, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 495>)
+               526 LOAD_CONST              36 (<code object unique_domains, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 491>)
                528 MAKE_FUNCTION            4 (annotations)
                530 STORE_NAME              45 (unique_domains)
    
-   507         532 LOAD_CONST              13 ('return')
+   503         532 LOAD_CONST              13 ('return')
                534 LOAD_NAME                7 (pd)
                536 LOAD_ATTR               36 (DataFrame)
                546 BUILD_TUPLE              2
-               548 LOAD_CONST              37 (<code object company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 507>)
+               548 LOAD_CONST              37 (<code object company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 503>)
                550 MAKE_FUNCTION            4 (annotations)
                552 STORE_NAME              46 (company)
    
-   518         554 LOAD_CONST              22 ('search_uid')
+   514         554 LOAD_CONST              22 ('search_uid')
                556 LOAD_NAME               33 (int)
                558 LOAD_CONST              13 ('return')
                560 LOAD_NAME                7 (pd)
                562 LOAD_ATTR               36 (DataFrame)
                572 BUILD_TUPLE              4
-               574 LOAD_CONST              38 (<code object checkpoint, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 518>)
+               574 LOAD_CONST              38 (<code object checkpoint, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 514>)
                576 MAKE_FUNCTION            4 (annotations)
                578 STORE_NAME              47 (checkpoint)
    
-   531         580 LOAD_CONST              22 ('search_uid')
+   527         580 LOAD_CONST              22 ('search_uid')
                582 LOAD_NAME               33 (int)
                584 LOAD_CONST              13 ('return')
                586 LOAD_NAME                7 (pd)
                588 LOAD_ATTR               36 (DataFrame)
                598 BUILD_TUPLE              4
-               600 LOAD_CONST              39 (<code object comment_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 531>)
+               600 LOAD_CONST              39 (<code object comment_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 527>)
                602 MAKE_FUNCTION            4 (annotations)
                604 STORE_NAME              48 (comment_by_domain)
    
-   552         606 LOAD_CONST              22 ('search_uid')
+   548         606 LOAD_CONST              22 ('search_uid')
                608 LOAD_NAME               33 (int)
                610 LOAD_CONST              13 ('return')
                612 LOAD_NAME               25 (Search)
                614 BUILD_TUPLE              4
-               616 LOAD_CONST              40 (<code object find_search_by_uid, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 552>)
+               616 LOAD_CONST              40 (<code object find_search_by_uid, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 548>)
                618 MAKE_FUNCTION            4 (annotations)
                620 STORE_NAME              49 (find_search_by_uid)
    
-   570         622 LOAD_CONST              41 ('domain')
+   566         622 LOAD_CONST              41 ('domain')
                624 LOAD_NAME               32 (str)
                626 LOAD_CONST              13 ('return')
                628 LOAD_NAME               22 (Company)
                630 BUILD_TUPLE              4
-               632 LOAD_CONST              42 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 570>)
+               632 LOAD_CONST              42 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 566>)
                634 MAKE_FUNCTION            4 (annotations)
                636 STORE_NAME              50 (find_company_by_domain)
    
-   586         638 LOAD_CONST              43 ('event_id')
+   582         638 LOAD_CONST              43 ('event_id')
                640 LOAD_NAME               33 (int)
                642 LOAD_CONST              13 ('return')
                644 LOAD_NAME               23 (Event)
                646 BUILD_TUPLE              4
-               648 LOAD_CONST              44 (<code object find_event_by_id, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 586>)
+               648 LOAD_CONST              44 (<code object find_event_by_id, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 582>)
                650 MAKE_FUNCTION            4 (annotations)
                652 STORE_NAME              51 (find_event_by_id)
    
-   605         654 LOAD_CONST              10 ('company')
+   601         654 LOAD_CONST              10 ('company')
                656 LOAD_NAME               22 (Company)
                658 LOAD_CONST              13 ('return')
                660 LOAD_CONST               1 (None)
                662 BUILD_TUPLE              4
-               664 LOAD_CONST              45 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 605>)
+               664 LOAD_CONST              45 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 601>)
                666 MAKE_FUNCTION            4 (annotations)
                668 STORE_NAME              52 (update_company)
    
-   632         670 LOAD_CONST              17 ('search')
+   628         670 LOAD_CONST              17 ('search')
                672 LOAD_NAME               25 (Search)
                674 LOAD_CONST              13 ('return')
                676 LOAD_CONST               1 (None)
                678 BUILD_TUPLE              4
-               680 LOAD_CONST              46 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 632>)
+               680 LOAD_CONST              46 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 628>)
                682 MAKE_FUNCTION            4 (annotations)
                684 STORE_NAME              53 (update_search)
                686 LOAD_CONST               1 (None)
                688 RETURN_VALUE
    consts
       0
       None
@@ -921,221 +921,229 @@
          lnotab 0x02013401160102ff1006460128f82e09
       'domains'
       'search_uid'
       'actor_key'
       'last_event_type'
       code
          argcount  : 4
-         nlocals   : 7
+         nlocals   : 10
          stacksize : 10
          flags     : 3
          code
-            0x97007401000000000000000000007c01ac01a6010000ab010000000000
-            000000640219000000000000000000a00100000000000000000000000000
-            00000000000000a6000000ab0000000000000000007d0474040000000000
-            0000000000a0030000000000000000000000000000000000000000a60000
-            00ab00000000000000000035007d057c0044005db07d0664037c06760172
-            1474090000000000000000000064047c069b0064059d03a6010000ab0100
-            0000000000000001008c1a740b000000000000000000006a060000000000
-            0000007c06a6010000ab0100000000000000007d067c067c047600721474
-            090000000000000000000064047c069b0064069d03a6010000ab01000000
-            000000000001008c4674090000000000000000000064077c069b0064089d
-            03a6010000ab01000000000000000001007c05a007000000000000000000
-            00000000000000000000007411000000000000000000006a090000000000
-            0000006409a6010000ab01000000000000000064027c066901a6020000ab
-            02000000000000000001007c05a007000000000000000000000000000000
-            00000000007411000000000000000000006a090000000000000000640aa6
-            010000ab0100000000000000007c017c027c067c03640b9c04a6020000ab
-            02000000000000000001008cb17c05a00a00000000000000000000000000
-            00000000000000a6000000ab0000000000000000000100640c640c640ca6
-            020000ab0200000000000000000100640c53002300310073047702780359
-            0077010100590001000100640c5300
+            0x97007401000000000000000000007403000000000000000000007c01ac
+            01a6010000ab010000000000000000640219000000000000000000a60100
+            00ab0100000000000000007d04640384007c004400a6000000ab00000000
+            00000000007d057405000000000000000000007c057c047a0a0000a60100
+            00ab0100000000000000007d06740600000000000000000000a004000000
+            0000000000000000000000000000000000a6000000ab0000000000000000
+            0035007d077c0644005d597d087c07a00500000000000000000000000000
+            00000000000000740d000000000000000000006a07000000000000000064
+            04a6010000ab01000000000000000064027c086901a6020000ab02000000
+            000000000001007c07a00500000000000000000000000000000000000000
+            00740d000000000000000000006a0700000000000000006405a6010000ab
+            0100000000000000007c017c027c087c0364069c04a6020000ab02000000
+            000000000001008c5a7c07a0080000000000000000000000000000000000
+            000000a6000000ab0000000000000000000100640764076407a6020000ab
+            02000000000000000001006e0b2300310073047702780359007701010059
+            00010001007413000000000000000000007c06a6010000ab010000000000
+            0000007413000000000000000000007c05a00a0000000000000000000000
+            0000000000000000007c04a6010000ab010000000000000000a6010000ab
+            01000000000000000064089c027d097c095300
          105           0 RESUME                   0
          
-         113           2 LOAD_GLOBAL              1 (NULL + unique_domains)
-                      14 LOAD_FAST                1 (search_uid)
-                      16 KW_NAMES                 1
-                      18 PRECALL                  1
-                      22 CALL                     1
+         112           2 LOAD_GLOBAL              1 (NULL + set)
+                      14 LOAD_GLOBAL              3 (NULL + unique_domains)
+                      26 LOAD_FAST                1 (search_uid)
+                      28 KW_NAMES                 1
+                      30 PRECALL                  1
+                      34 CALL                     1
+                      44 LOAD_CONST               2 ('domain')
+                      46 BINARY_SUBSCR
+                      56 PRECALL                  1
+                      60 CALL                     1
+                      70 STORE_FAST               4 (existing_domains)
+         
+         114          72 LOAD_CONST               3 (<code object <setcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 114>)
+                      74 MAKE_FUNCTION            0
+                      76 LOAD_FAST                0 (domains)
+                      78 GET_ITER
+                      80 PRECALL                  0
+                      84 CALL                     0
+                      94 STORE_FAST               5 (new_domains)
+         
+         116          96 LOAD_GLOBAL              5 (NULL + list)
+                     108 LOAD_FAST                5 (new_domains)
+                     110 LOAD_FAST                4 (existing_domains)
+                     112 BINARY_OP               10 (-)
+                     116 PRECALL                  1
+                     120 CALL                     1
+                     130 STORE_FAST               6 (domains_to_insert)
          
-         114          32 LOAD_CONST               2 ('domain')
+         118         132 LOAD_GLOBAL              6 (db)
+                     144 LOAD_METHOD              4 (connect)
+                     166 PRECALL                  0
+                     170 CALL                     0
+                     180 BEFORE_WITH
+                     182 STORE_FAST               7 (con)
          
-         113          34 BINARY_SUBSCR
+         119         184 LOAD_FAST                6 (domains_to_insert)
+                     186 GET_ITER
+                 >>  188 FOR_ITER                89 (to 368)
+                     190 STORE_FAST               8 (domain)
          
-         115          44 LOAD_METHOD              1 (to_list)
-                      66 PRECALL                  0
-                      70 CALL                     0
+         121         192 LOAD_FAST                7 (con)
+                     194 LOAD_METHOD              5 (execute)
          
-         113          80 STORE_FAST               4 (existing_search_domains)
+         122         216 LOAD_GLOBAL             13 (NULL + sqlalchemy)
+                     228 LOAD_ATTR                7 (text)
          
-         116          82 LOAD_GLOBAL              4 (db)
-                      94 LOAD_METHOD              3 (connect)
-                     116 PRECALL                  0
-                     120 CALL                     0
-                     130 BEFORE_WITH
-                     132 STORE_FAST               5 (con)
+         123         238 LOAD_CONST               4 ('\n                    INSERT INTO company (domain) \n                    VALUES(:domain)\n                    ON CONFLICT DO NOTHING\n                    ')
          
-         117         134 LOAD_FAST                0 (domains)
-                     136 GET_ITER
-                 >>  138 FOR_ITER               176 (to 492)
-                     140 STORE_FAST               6 (domain)
+         122         240 PRECALL                  1
+                     244 CALL                     1
          
-         118         142 LOAD_CONST               3 ('.')
-                     144 LOAD_FAST                6 (domain)
-                     146 CONTAINS_OP              1
-                     148 POP_JUMP_FORWARD_IF_FALSE    20 (to 190)
-         
-         119         150 LOAD_GLOBAL              9 (NULL + print)
-                     162 LOAD_CONST               4 ('Skipping ')
-                     164 LOAD_FAST                6 (domain)
-                     166 FORMAT_VALUE             0
-                     168 LOAD_CONST               5 (' as not a valid domain')
-                     170 BUILD_STRING             3
-                     172 PRECALL                  1
-                     176 CALL                     1
-                     186 POP_TOP
+         129         254 LOAD_CONST               2 ('domain')
+                     256 LOAD_FAST                8 (domain)
+                     258 BUILD_MAP                1
          
-         120         188 JUMP_BACKWARD           26 (to 138)
-         
-         122     >>  190 LOAD_GLOBAL             11 (NULL + helpers)
-                     202 LOAD_ATTR                6 (clean_domain)
-                     212 LOAD_FAST                6 (domain)
-                     214 PRECALL                  1
-                     218 CALL                     1
-                     228 STORE_FAST               6 (domain)
-         
-         124         230 LOAD_FAST                6 (domain)
-                     232 LOAD_FAST                4 (existing_search_domains)
-                     234 CONTAINS_OP              0
-                     236 POP_JUMP_FORWARD_IF_FALSE    20 (to 278)
-         
-         125         238 LOAD_GLOBAL              9 (NULL + print)
-                     250 LOAD_CONST               4 ('Skipping ')
-                     252 LOAD_FAST                6 (domain)
-                     254 FORMAT_VALUE             0
-                     256 LOAD_CONST               6 (' as already a target')
-                     258 BUILD_STRING             3
-                     260 PRECALL                  1
-                     264 CALL                     1
+         121         260 PRECALL                  2
+                     264 CALL                     2
                      274 POP_TOP
          
-         126         276 JUMP_BACKWARD           70 (to 138)
-         
-         128     >>  278 LOAD_GLOBAL              9 (NULL + print)
-                     290 LOAD_CONST               7 ('Adding ')
-                     292 LOAD_FAST                6 (domain)
-                     294 FORMAT_VALUE             0
-                     296 LOAD_CONST               8 (' as target')
-                     298 BUILD_STRING             3
-                     300 PRECALL                  1
-                     304 CALL                     1
-                     314 POP_TOP
-         
-         131         316 LOAD_FAST                5 (con)
-                     318 LOAD_METHOD              7 (execute)
-         
-         132         340 LOAD_GLOBAL             17 (NULL + sqlalchemy)
-                     352 LOAD_ATTR                9 (text)
-         
-         133         362 LOAD_CONST               9 ('\n                    INSERT INTO company (domain) \n                    VALUES(:domain)\n                    ON CONFLICT DO NOTHING\n                    ')
-         
-         132         364 PRECALL                  1
-                     368 CALL                     1
-         
-         139         378 LOAD_CONST               2 ('domain')
-                     380 LOAD_FAST                6 (domain)
-                     382 BUILD_MAP                1
-         
-         131         384 PRECALL                  2
-                     388 CALL                     2
-                     398 POP_TOP
-         
-         142         400 LOAD_FAST                5 (con)
-                     402 LOAD_METHOD              7 (execute)
-         
-         143         424 LOAD_GLOBAL             17 (NULL + sqlalchemy)
-                     436 LOAD_ATTR                9 (text)
-         
-         144         446 LOAD_CONST              10 ('\n                    INSERT INTO event (search_uid, domain, actor_key, type) \n                    VALUES(:search_uid, :domain, :actor_key, :type)\n                    ')
-         
-         143         448 PRECALL                  1
-                     452 CALL                     1
-         
-         150         462 LOAD_FAST                1 (search_uid)
-         
-         151         464 LOAD_FAST                2 (actor_key)
+         132         276 LOAD_FAST                7 (con)
+                     278 LOAD_METHOD              5 (execute)
          
-         152         466 LOAD_FAST                6 (domain)
+         133         300 LOAD_GLOBAL             13 (NULL + sqlalchemy)
+                     312 LOAD_ATTR                7 (text)
          
-         153         468 LOAD_FAST                3 (last_event_type)
+         134         322 LOAD_CONST               5 ('\n                    INSERT INTO event (search_uid, domain, actor_key, type) \n                    VALUES(:search_uid, :domain, :actor_key, :type)\n                    ON CONFLICT DO NOTHING\n                    ')
          
-         149         470 LOAD_CONST              11 (('search_uid', 'actor_key', 'domain', 'type'))
-                     472 BUILD_CONST_KEY_MAP      4
+         133         324 PRECALL                  1
+                     328 CALL                     1
+         
+         141         338 LOAD_FAST                1 (search_uid)
+         
+         142         340 LOAD_FAST                2 (actor_key)
+         
+         143         342 LOAD_FAST                8 (domain)
+         
+         144         344 LOAD_FAST                3 (last_event_type)
+         
+         140         346 LOAD_CONST               6 (('search_uid', 'actor_key', 'domain', 'type'))
+                     348 BUILD_CONST_KEY_MAP      4
+         
+         132         350 PRECALL                  2
+                     354 CALL                     2
+                     364 POP_TOP
+                     366 JUMP_BACKWARD           90 (to 188)
+         
+         148     >>  368 LOAD_FAST                7 (con)
+                     370 LOAD_METHOD              8 (commit)
+                     392 PRECALL                  0
+                     396 CALL                     0
+                     406 POP_TOP
+         
+         118         408 LOAD_CONST               7 (None)
+                     410 LOAD_CONST               7 (None)
+                     412 LOAD_CONST               7 (None)
+                     414 PRECALL                  2
+                     418 CALL                     2
+                     428 POP_TOP
+                     430 JUMP_FORWARD            11 (to 454)
+                 >>  432 PUSH_EXC_INFO
+                     434 WITH_EXCEPT_START
+                     436 POP_JUMP_FORWARD_IF_TRUE     4 (to 446)
+                     438 RERAISE                  2
+                 >>  440 COPY                     3
+                     442 POP_EXCEPT
+                     444 RERAISE                  1
+                 >>  446 POP_TOP
+                     448 POP_EXCEPT
+                     450 POP_TOP
+                     452 POP_TOP
+         
+         151     >>  454 LOAD_GLOBAL             19 (NULL + len)
+                     466 LOAD_FAST                6 (domains_to_insert)
+                     468 PRECALL                  1
+                     472 CALL                     1
+         
+         152         482 LOAD_GLOBAL             19 (NULL + len)
+                     494 LOAD_FAST                5 (new_domains)
+                     496 LOAD_METHOD             10 (intersection)
+                     518 LOAD_FAST                4 (existing_domains)
+                     520 PRECALL                  1
+                     524 CALL                     1
+                     534 PRECALL                  1
+                     538 CALL                     1
+         
+         150         548 LOAD_CONST               8 (('inserted', 'duplicates'))
+                     550 BUILD_CONST_KEY_MAP      2
+                     552 STORE_FAST               9 (resp)
          
-         142         474 PRECALL                  2
-                     478 CALL                     2
-                     488 POP_TOP
-                     490 JUMP_BACKWARD          177 (to 138)
-         
-         157     >>  492 LOAD_FAST                5 (con)
-                     494 LOAD_METHOD             10 (commit)
-                     516 PRECALL                  0
-                     520 CALL                     0
-                     530 POP_TOP
-         
-         116         532 LOAD_CONST              12 (None)
-                     534 LOAD_CONST              12 (None)
-                     536 LOAD_CONST              12 (None)
-                     538 PRECALL                  2
-                     542 CALL                     2
-                     552 POP_TOP
-                     554 LOAD_CONST              12 (None)
+         154         554 LOAD_FAST                9 (resp)
                      556 RETURN_VALUE
-                 >>  558 PUSH_EXC_INFO
-                     560 WITH_EXCEPT_START
-                     562 POP_JUMP_FORWARD_IF_TRUE     4 (to 572)
-                     564 RERAISE                  2
-                 >>  566 COPY                     3
-                     568 POP_EXCEPT
-                     570 RERAISE                  1
-                 >>  572 POP_TOP
-                     574 POP_EXCEPT
-                     576 POP_TOP
-                     578 POP_TOP
-                     580 LOAD_CONST              12 (None)
-                     582 RETURN_VALUE
-         ExceptionTable:
-           132 to 530 -> 558 [1] lasti
-           558 to 564 -> 566 [3] lasti
-           572 to 572 -> 566 [3] lasti
+         ExceptionTable:
+           182 to 406 -> 432 [1] lasti
+           432 to 438 -> 440 [3] lasti
+           446 to 446 -> 440 [3] lasti
          consts
-            '\n    Takes in domains, inserts targets into a review stage, where they will\n    try to be enriched on process event\n\n    '
+            '\n    Takes in domains, inserts targets into a review stage, where they will\n    try to be enriched on process event\n    '
             ('search_uid',)
             'domain'
-            '.'
-            'Skipping '
-            ' as not a valid domain'
-            ' as already a target'
-            'Adding '
-            ' as target'
+            code
+               argcount  : 1
+               nlocals   : 2
+               stacksize : 5
+               flags     : 19
+               code
+                  0x970068007c005d1a7d0164007c017600af067401000000000000000000
+                  006a0100000000000000007c01a6010000ab01000000000000000092028c
+                  1b5300
+               114           0 RESUME                   0
+                             2 BUILD_SET                0
+                             4 LOAD_FAST                0 (.0)
+                       >>    6 FOR_ITER                26 (to 60)
+                             8 STORE_FAST               1 (domain)
+                            10 LOAD_CONST               0 ('.')
+                            12 LOAD_FAST                1 (domain)
+                            14 CONTAINS_OP              0
+                            16 POP_JUMP_BACKWARD_IF_FALSE     6 (to 6)
+                            18 LOAD_GLOBAL              1 (NULL + helpers)
+                            30 LOAD_ATTR                1 (clean_domain)
+                            40 LOAD_FAST                1 (domain)
+                            42 PRECALL                  1
+                            46 CALL                     1
+                            56 SET_ADD                  2
+                            58 JUMP_BACKWARD           27 (to 6)
+                       >>   60 RETURN_VALUE
+               consts
+                  '.'
+               names      ('helpers', 'clean_domain')
+               varnames   ('.0', 'domain')
+               freevars   ()
+               cellvars   ()
+               filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
+               name       '<setcomp>'
+               firstlineno 114
+               lnotab 0x
             '\n                    INSERT INTO company (domain) \n                    VALUES(:domain)\n                    ON CONFLICT DO NOTHING\n                    '
-            '\n                    INSERT INTO event (search_uid, domain, actor_key, type) \n                    VALUES(:search_uid, :domain, :actor_key, :type)\n                    '
+            '\n                    INSERT INTO event (search_uid, domain, actor_key, type) \n                    VALUES(:search_uid, :domain, :actor_key, :type)\n                    ON CONFLICT DO NOTHING\n                    '
             ('search_uid', 'actor_key', 'domain', 'type')
             None
-         names      ('unique_domains', 'to_list', 'db', 'connect', 'print', 'helpers', 'clean_domain', 'execute', 'sqlalchemy', 'text', 'commit')
-         varnames   ('domains', 'search_uid', 'actor_key', 'last_event_type', 'existing_search_domains', 'con', 'domain')
+            ('inserted', 'duplicates')
+         names      ('set', 'unique_domains', 'list', 'db', 'connect', 'execute', 'sqlalchemy', 'text', 'commit', 'len', 'intersection')
+         varnames   ('domains', 'search_uid', 'actor_key', 'last_event_type', 'existing_domains', 'new_domains', 'domains_to_insert', 'con', 'domain', 'resp')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'insert_targets_from_domains'
          firstlineno 105
          lnotab
-            0x02081e0102ff0a0224fe02033401080108012601020228020801260102
-            0226031801160102ff0e0706f8100b1801160102ff0e0702010201020102
-            fc04f9120f28d7
+            0x0207460218022402340108021801160102ff0e0706f8100b1801160102
+            ff0e0802010201020102fc04f8121028e22e211c0142fe0604
       'companies'
       code
          argcount  : 3
          nlocals   : 6
          stacksize : 10
          flags     : 3
          code
@@ -1161,168 +1169,168 @@
             0000000000740f000000000000000000006a080000000000000000640ea6
             010000ab0100000000000000007c017c027c05a004000000000000000000
             00000000000000000000006402a6010000ab010000000000000000640f64
             109c04a6020000ab020000000000000000010090018c107c04a009000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             000100640364036403a6020000ab02000000000000000001006403530023
             00310073047702780359007701010059000100010064035300
-         160           0 RESUME                   0
+         157           0 RESUME                   0
          
-         164           2 LOAD_GLOBAL              1 (NULL + unique_domains)
+         161           2 LOAD_GLOBAL              1 (NULL + unique_domains)
                       14 LOAD_FAST                1 (search_uid)
                       16 KW_NAMES                 1
                       18 PRECALL                  1
                       22 CALL                     1
                       32 LOAD_CONST               2 ('domain')
                       34 BINARY_SUBSCR
                       44 LOAD_METHOD              1 (to_list)
                       66 PRECALL                  0
                       70 CALL                     0
                       80 STORE_FAST               3 (existing_search_domains)
          
-         165          82 LOAD_GLOBAL              4 (db)
+         162          82 LOAD_GLOBAL              4 (db)
                       94 LOAD_METHOD              3 (connect)
                      116 PRECALL                  0
                      120 CALL                     0
                      130 BEFORE_WITH
                      132 STORE_FAST               4 (con)
          
-         166         134 LOAD_FAST                0 (companies)
+         163         134 LOAD_FAST                0 (companies)
                      136 GET_ITER
                  >>  138 EXTENDED_ARG             1
                      140 FOR_ITER               270 (to 682)
                      142 STORE_FAST               5 (company)
          
-         167         144 LOAD_FAST                5 (company)
+         164         144 LOAD_FAST                5 (company)
                      146 LOAD_METHOD              4 (get)
                      168 LOAD_CONST               2 ('domain')
                      170 PRECALL                  1
                      174 CALL                     1
                      184 POP_JUMP_FORWARD_IF_NOT_NONE    20 (to 226)
          
-         168         186 LOAD_GLOBAL             11 (NULL + print)
+         165         186 LOAD_GLOBAL             11 (NULL + print)
                      198 LOAD_CONST               4 ('Missing domain: ')
                      200 LOAD_FAST                5 (company)
                      202 FORMAT_VALUE             0
                      204 LOAD_CONST               5 ('. Skipping')
                      206 BUILD_STRING             3
                      208 PRECALL                  1
                      212 CALL                     1
                      222 POP_TOP
          
-         169         224 JUMP_BACKWARD           44 (to 138)
+         166         224 JUMP_BACKWARD           44 (to 138)
          
-         172     >>  226 LOAD_FAST                5 (company)
+         169     >>  226 LOAD_FAST                5 (company)
                      228 LOAD_CONST               2 ('domain')
                      230 BINARY_SUBSCR
                      240 LOAD_FAST                3 (existing_search_domains)
                      242 CONTAINS_OP              0
                      244 POP_JUMP_FORWARD_IF_FALSE    26 (to 298)
          
-         173         246 LOAD_GLOBAL             11 (NULL + print)
+         170         246 LOAD_GLOBAL             11 (NULL + print)
                      258 LOAD_CONST               6 ('Skipping ')
                      260 LOAD_FAST                5 (company)
                      262 LOAD_CONST               2 ('domain')
                      264 BINARY_SUBSCR
                      274 FORMAT_VALUE             0
                      276 LOAD_CONST               7 (' as already a target')
                      278 BUILD_STRING             3
                      280 PRECALL                  1
                      284 CALL                     1
                      294 POP_TOP
          
-         174         296 JUMP_BACKWARD           80 (to 138)
+         171         296 JUMP_BACKWARD           80 (to 138)
          
-         176     >>  298 LOAD_GLOBAL             11 (NULL + print)
+         173     >>  298 LOAD_GLOBAL             11 (NULL + print)
                      310 LOAD_CONST               8 ('Adding ')
                      312 LOAD_FAST                5 (company)
                      314 LOAD_CONST               2 ('domain')
                      316 BINARY_SUBSCR
                      326 FORMAT_VALUE             0
                      328 LOAD_CONST               9 (' as target')
                      330 BUILD_STRING             3
                      332 PRECALL                  1
                      336 CALL                     1
                      346 POP_TOP
          
-         178         348 LOAD_FAST                4 (con)
+         175         348 LOAD_FAST                4 (con)
                      350 LOAD_METHOD              6 (execute)
          
-         179         372 LOAD_GLOBAL             15 (NULL + sqlalchemy)
+         176         372 LOAD_GLOBAL             15 (NULL + sqlalchemy)
                      384 LOAD_ATTR                8 (text)
          
-         180         394 LOAD_CONST              10 ('\n                    INSERT INTO company (domain, name, description) \n                    VALUES(:domain, :name, :description)\n                    ON CONFLICT DO NOTHING\n                    ')
+         177         394 LOAD_CONST              10 ('\n                    INSERT INTO company (domain, name, description) \n                    VALUES(:domain, :name, :description)\n                    ON CONFLICT DO NOTHING\n                    ')
          
-         179         396 PRECALL                  1
+         176         396 PRECALL                  1
                      400 CALL                     1
          
-         187         410 LOAD_FAST                5 (company)
+         184         410 LOAD_FAST                5 (company)
                      412 LOAD_METHOD              4 (get)
                      434 LOAD_CONST               2 ('domain')
                      436 PRECALL                  1
                      440 CALL                     1
          
-         188         450 LOAD_FAST                5 (company)
+         185         450 LOAD_FAST                5 (company)
                      452 LOAD_METHOD              4 (get)
                      474 LOAD_CONST              11 ('name')
                      476 PRECALL                  1
                      480 CALL                     1
          
-         189         490 LOAD_FAST                5 (company)
+         186         490 LOAD_FAST                5 (company)
                      492 LOAD_METHOD              4 (get)
                      514 LOAD_CONST              12 ('description')
                      516 PRECALL                  1
                      520 CALL                     1
          
-         186         530 LOAD_CONST              13 (('domain', 'name', 'description'))
+         183         530 LOAD_CONST              13 (('domain', 'name', 'description'))
                      532 BUILD_CONST_KEY_MAP      3
          
-         178         534 PRECALL                  2
+         175         534 PRECALL                  2
                      538 CALL                     2
                      548 POP_TOP
          
-         193         550 LOAD_FAST                4 (con)
+         190         550 LOAD_FAST                4 (con)
                      552 LOAD_METHOD              6 (execute)
          
-         194         574 LOAD_GLOBAL             15 (NULL + sqlalchemy)
+         191         574 LOAD_GLOBAL             15 (NULL + sqlalchemy)
                      586 LOAD_ATTR                8 (text)
          
-         195         596 LOAD_CONST              14 ('\n                    INSERT INTO event (search_uid, domain, actor_key, type) \n                    VALUES(:search_uid, :domain, :actor_key, :type)\n                    ')
+         192         596 LOAD_CONST              14 ('\n                    INSERT INTO event (search_uid, domain, actor_key, type) \n                    VALUES(:search_uid, :domain, :actor_key, :type)\n                    ')
          
-         194         598 PRECALL                  1
+         191         598 PRECALL                  1
                      602 CALL                     1
          
-         201         612 LOAD_FAST                1 (search_uid)
+         198         612 LOAD_FAST                1 (search_uid)
          
-         202         614 LOAD_FAST                2 (actor_key)
+         199         614 LOAD_FAST                2 (actor_key)
          
-         203         616 LOAD_FAST                5 (company)
+         200         616 LOAD_FAST                5 (company)
                      618 LOAD_METHOD              4 (get)
                      640 LOAD_CONST               2 ('domain')
                      642 PRECALL                  1
                      646 CALL                     1
          
-         204         656 LOAD_CONST              15 ('create')
+         201         656 LOAD_CONST              15 ('create')
          
-         200         658 LOAD_CONST              16 (('search_uid', 'actor_key', 'domain', 'type'))
+         197         658 LOAD_CONST              16 (('search_uid', 'actor_key', 'domain', 'type'))
                      660 BUILD_CONST_KEY_MAP      4
          
-         193         662 PRECALL                  2
+         190         662 PRECALL                  2
                      666 CALL                     2
                      676 POP_TOP
                      678 EXTENDED_ARG             1
                      680 JUMP_BACKWARD          272 (to 138)
          
-         209     >>  682 LOAD_FAST                4 (con)
+         205     >>  682 LOAD_FAST                4 (con)
                      684 LOAD_METHOD              9 (commit)
                      706 PRECALL                  0
                      710 CALL                     0
                      720 POP_TOP
          
-         165         722 LOAD_CONST               3 (None)
+         162         722 LOAD_CONST               3 (None)
                      724 LOAD_CONST               3 (None)
                      726 LOAD_CONST               3 (None)
                      728 PRECALL                  2
                      732 CALL                     2
                      742 POP_TOP
                      744 LOAD_CONST               3 (None)
                      746 RETURN_VALUE
@@ -1363,19 +1371,19 @@
             ('search_uid', 'actor_key', 'domain', 'type')
          names      ('unique_domains', 'to_list', 'db', 'connect', 'get', 'print', 'execute', 'sqlalchemy', 'text', 'commit')
          varnames   ('companies', 'search_uid', 'actor_key', 'existing_search_domains', 'con', 'company')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'insert_companies_as_targets'
-         firstlineno 160
+         firstlineno 157
          lnotab
             0x0204500134010a012a012601020314013201020232021801160102ff0e
             082801280128fd04f8100f1801160102ff0e0702010201280102fc04f914
-            1028d4
+            0f28d5
       code
          argcount  : 0
          nlocals   : 4
          stacksize : 6
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
@@ -1385,55 +1393,55 @@
             00a6010000ab0100000000000000007d02740b000000000000000000006a
             0600000000000000007c02a0070000000000000000000000000000000000
             000000a6000000ab0000000000000000007c02a008000000000000000000
             0000000000000000000000a6000000ab000000000000000000ac02a60200
             00ab0200000000000000007d037c036302640064006400a6020000ab0200
             000000000000000100530023003100730477027803590077010100590001
             00010064005300
-         215           0 RESUME                   0
+         211           0 RESUME                   0
          
-         216           2 LOAD_GLOBAL              0 (db)
+         212           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         217          54 LOAD_CONST               1 ("\n        WITH ranked_actors AS (\n            SELECT \n                a.name,\n                s.uid AS search_uid,\n                COUNT(e.id) AS total_validate_count,\n                ROW_NUMBER() OVER (\n                    PARTITION BY s.uid\n                    ORDER BY COUNT(e.id) DESC\n                ) as rn\n            FROM \n                event e\n            INNER JOIN \n                actor a ON a.key = e.actor_key\n            INNER JOIN \n                search s ON s.uid = e.search_uid\n            WHERE\n                a.type = 'research' AND \n                e.type = 'validate' \n            GROUP BY \n                a.name, s.uid\n        )\n        SELECT \n            name, \n            search_uid, \n            total_validate_count\n        FROM \n            ranked_actors\n        WHERE \n            rn = 1;\n        ")
+         213          54 LOAD_CONST               1 ("\n        WITH ranked_actors AS (\n            SELECT \n                a.name,\n                s.uid AS search_uid,\n                COUNT(e.id) AS total_validate_count,\n                ROW_NUMBER() OVER (\n                    PARTITION BY s.uid\n                    ORDER BY COUNT(e.id) DESC\n                ) as rn\n            FROM \n                event e\n            INNER JOIN \n                actor a ON a.key = e.actor_key\n            INNER JOIN \n                search s ON s.uid = e.search_uid\n            WHERE\n                a.type = 'research' AND \n                e.type = 'validate' \n            GROUP BY \n                a.name, s.uid\n        )\n        SELECT \n            name, \n            search_uid, \n            total_validate_count\n        FROM \n            ranked_actors\n        WHERE \n            rn = 1;\n        ")
                       56 STORE_FAST               1 (statement)
          
-         249          58 LOAD_FAST                0 (conn)
+         245          58 LOAD_FAST                0 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                1 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 PRECALL                  1
                      124 CALL                     1
                      134 STORE_FAST               2 (result)
          
-         250         136 LOAD_GLOBAL             11 (NULL + pd)
+         246         136 LOAD_GLOBAL             11 (NULL + pd)
                      148 LOAD_ATTR                6 (DataFrame)
                      158 LOAD_FAST                2 (result)
                      160 LOAD_METHOD              7 (fetchall)
                      182 PRECALL                  0
                      186 CALL                     0
                      196 LOAD_FAST                2 (result)
                      198 LOAD_METHOD              8 (keys)
                      220 PRECALL                  0
                      224 CALL                     0
                      234 KW_NAMES                 2
                      236 PRECALL                  2
                      240 CALL                     2
                      250 STORE_FAST               3 (df)
          
-         251         252 LOAD_FAST                3 (df)
+         247         252 LOAD_FAST                3 (df)
          
-         216         254 SWAP                     2
+         212         254 SWAP                     2
                      256 LOAD_CONST               0 (None)
                      258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 PRECALL                  2
                      266 CALL                     2
                      276 POP_TOP
                      278 RETURN_VALUE
@@ -1460,15 +1468,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'top_actor_per_search'
-         firstlineno 215
+         firstlineno 211
          lnotab 0x0201340104204e01740102dd
       code
          argcount  : 0
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
@@ -1483,54 +1491,54 @@
             000000000000007d027c02a0090000000000000000000000000000000000
             000000640364046405ac06a6030000ab030000000000000000a00a000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00a00b00000000000000000000000000000000000000006407a6010000ab
             0100000000000000007d027c026302640064006400a6020000ab02000000
             000000000001005300230031007304770278035900770101005900010001
             0064005300
-         253           0 RESUME                   0
+         249           0 RESUME                   0
          
-         254           2 LOAD_GLOBAL              0 (db)
+         250           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         255          54 LOAD_FAST                0 (conn)
+         251          54 LOAD_FAST                0 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         256          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         252          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         257         100 LOAD_CONST               1 ("\n                SELECT search_uid, type, count(DISTINCT domain)\n                FROM event\n                WHERE type in ('create','advance', 'validate', 'send', 'accept')\n                GROUP BY search_uid, type\n                ")
+         253         100 LOAD_CONST               1 ("\n                SELECT search_uid, type, count(DISTINCT domain)\n                FROM event\n                WHERE type in ('create','advance', 'validate', 'send', 'accept')\n                GROUP BY search_uid, type\n                ")
          
-         256         102 PRECALL                  1
+         252         102 PRECALL                  1
                      106 CALL                     1
          
-         255         116 PRECALL                  1
+         251         116 PRECALL                  1
                      120 CALL                     1
                      130 STORE_FAST               1 (result)
          
-         265         132 LOAD_GLOBAL             11 (NULL + pd)
+         261         132 LOAD_GLOBAL             11 (NULL + pd)
                      144 LOAD_ATTR                6 (DataFrame)
                      154 LOAD_FAST                1 (result)
                      156 LOAD_METHOD              7 (fetchall)
                      178 PRECALL                  0
                      182 CALL                     0
                      192 LOAD_FAST                1 (result)
                      194 LOAD_METHOD              8 (keys)
                      216 PRECALL                  0
                      220 CALL                     0
                      230 KW_NAMES                 2
                      232 PRECALL                  2
                      236 CALL                     2
                      246 STORE_FAST               2 (df)
          
-         266         248 LOAD_FAST                2 (df)
+         262         248 LOAD_FAST                2 (df)
                      250 LOAD_METHOD              9 (pivot)
                      272 LOAD_CONST               3 ('search_uid')
                      274 LOAD_CONST               4 ('type')
                      276 LOAD_CONST               5 ('count')
                      278 KW_NAMES                 6
                      280 PRECALL                  3
                      284 CALL                     3
@@ -1539,17 +1547,17 @@
                      320 CALL                     0
                      330 LOAD_METHOD             11 (fillna)
                      352 LOAD_CONST               7 (0)
                      354 PRECALL                  1
                      358 CALL                     1
                      368 STORE_FAST               2 (df)
          
-         267         370 LOAD_FAST                2 (df)
+         263         370 LOAD_FAST                2 (df)
          
-         254         372 SWAP                     2
+         250         372 SWAP                     2
                      374 LOAD_CONST               0 (None)
                      376 LOAD_CONST               0 (None)
                      378 LOAD_CONST               0 (None)
                      380 PRECALL                  2
                      384 CALL                     2
                      394 POP_TOP
                      396 RETURN_VALUE
@@ -1581,15 +1589,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'pivot', 'reset_index', 'fillna')
          varnames   ('conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search_event_count_by_type'
-         firstlineno 253
+         firstlineno 249
          lnotab 0x020134011801160102ff0eff100a74017a0102f3
       code
          argcount  : 0
          nlocals   : 5
          stacksize : 7
          flags     : 3
          code
@@ -1610,119 +1618,119 @@
             00a6000000ab000000000000000000640364046405ac06a6040000ab0400
             000000000000007d037c03a00d0000000000000000000000000000000000
             0000006700640ba2016700640ca201ac0da6020000ab0200000000000000
             007d037c03a00e0000000000000000000000000000000000000000640ea6
             010000ab0100000000000000007d03640064006400a6020000ab02000000
             000000000001006e0b230031007304770278035900770101005900010001
             007c035300
-         269           0 RESUME                   0
+         265           0 RESUME                   0
          
-         270           2 LOAD_GLOBAL              0 (db)
+         266           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         271          54 LOAD_CONST               1 ("\n        SELECT \n            s.uid,\n            s.label,\n            (SELECT COUNT(*) \n            FROM event e\n            WHERE \n            e.search_uid = s.uid AND e.created >= EXTRACT(EPOCH FROM (NOW() - INTERVAL '7 days')) and type = 'validate'\n            ) AS recent_validate_count\n        FROM \n            search s;\n        ")
+         267          54 LOAD_CONST               1 ("\n        SELECT \n            s.uid,\n            s.label,\n            (SELECT COUNT(*) \n            FROM event e\n            WHERE \n            e.search_uid = s.uid AND e.created >= EXTRACT(EPOCH FROM (NOW() - INTERVAL '7 days')) and type = 'validate'\n            ) AS recent_validate_count\n        FROM \n            search s;\n        ")
                       56 STORE_FAST               1 (statement)
          
-         283          58 LOAD_FAST                0 (conn)
+         279          58 LOAD_FAST                0 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                1 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 PRECALL                  1
                      124 CALL                     1
                      134 STORE_FAST               2 (result)
          
-         284         136 LOAD_GLOBAL             11 (NULL + pd)
+         280         136 LOAD_GLOBAL             11 (NULL + pd)
                      148 LOAD_ATTR                6 (DataFrame)
                      158 LOAD_FAST                2 (result)
                      160 LOAD_METHOD              7 (fetchall)
                      182 PRECALL                  0
                      186 CALL                     0
                      196 LOAD_FAST                2 (result)
                      198 LOAD_METHOD              8 (keys)
                      220 PRECALL                  0
                      224 CALL                     0
                      234 KW_NAMES                 2
                      236 PRECALL                  2
                      240 CALL                     2
                      250 STORE_FAST               3 (df)
          
-         286         252 LOAD_FAST                3 (df)
+         282         252 LOAD_FAST                3 (df)
                      254 LOAD_METHOD              9 (merge)
          
-         287         276 LOAD_GLOBAL             21 (NULL + top_actor_per_search)
+         283         276 LOAD_GLOBAL             21 (NULL + top_actor_per_search)
                      288 PRECALL                  0
                      292 CALL                     0
                      302 LOAD_CONST               3 ('uid')
                      304 LOAD_CONST               4 ('search_uid')
                      306 LOAD_CONST               5 ('left')
          
-         286         308 KW_NAMES                 6
+         282         308 KW_NAMES                 6
                      310 PRECALL                  4
                      314 CALL                     4
                      324 STORE_FAST               3 (df)
          
-         290         326 LOAD_CONST               7 (<code object _set_group, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 290>)
+         286         326 LOAD_CONST               7 (<code object _set_group, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 286>)
                      328 MAKE_FUNCTION            0
                      330 STORE_FAST               4 (_set_group)
          
-         298         332 LOAD_FAST                3 (df)
+         294         332 LOAD_FAST                3 (df)
                      334 LOAD_METHOD             11 (apply)
                      356 LOAD_FAST                4 (_set_group)
                      358 LOAD_CONST               8 (1)
                      360 KW_NAMES                 9
                      362 PRECALL                  2
                      366 CALL                     2
                      376 LOAD_FAST                3 (df)
                      378 LOAD_CONST              10 ('group')
                      380 STORE_SUBSCR
          
-         300         384 LOAD_FAST                3 (df)
+         296         384 LOAD_FAST                3 (df)
                      386 LOAD_METHOD              9 (merge)
                      408 LOAD_GLOBAL             25 (NULL + search_event_count_by_type)
                      420 PRECALL                  0
                      424 CALL                     0
                      434 LOAD_CONST               3 ('uid')
                      436 LOAD_CONST               4 ('search_uid')
                      438 LOAD_CONST               5 ('left')
                      440 KW_NAMES                 6
                      442 PRECALL                  4
                      446 CALL                     4
                      456 STORE_FAST               3 (df)
          
-         302         458 LOAD_FAST                3 (df)
+         298         458 LOAD_FAST                3 (df)
                      460 LOAD_METHOD             13 (sort_values)
          
-         303         482 BUILD_LIST               0
+         299         482 BUILD_LIST               0
                      484 LOAD_CONST              11 (('group', 'recent_validate_count', 'total_validate_count', 'label'))
                      486 LIST_EXTEND              1
          
-         304         488 BUILD_LIST               0
+         300         488 BUILD_LIST               0
                      490 LOAD_CONST              12 ((False, False, False, True))
                      492 LIST_EXTEND              1
          
-         302         494 KW_NAMES                13
+         298         494 KW_NAMES                13
                      496 PRECALL                  2
                      500 CALL                     2
                      510 STORE_FAST               3 (df)
          
-         307         512 LOAD_FAST                3 (df)
+         303         512 LOAD_FAST                3 (df)
                      514 LOAD_METHOD             14 (fillna)
                      536 LOAD_CONST              14 ('')
                      538 PRECALL                  1
                      542 CALL                     1
                      552 STORE_FAST               3 (df)
          
-         270         554 LOAD_CONST               0 (None)
+         266         554 LOAD_CONST               0 (None)
                      556 LOAD_CONST               0 (None)
                      558 LOAD_CONST               0 (None)
                      560 PRECALL                  2
                      564 CALL                     2
                      574 POP_TOP
                      576 JUMP_FORWARD            11 (to 600)
                  >>  578 PUSH_EXC_INFO
@@ -1733,15 +1741,15 @@
                      588 POP_EXCEPT
                      590 RERAISE                  1
                  >>  592 POP_TOP
                      594 POP_EXCEPT
                      596 POP_TOP
                      598 POP_TOP
          
-         309     >>  600 LOAD_FAST                3 (df)
+         305     >>  600 LOAD_FAST                3 (df)
                      602 RETURN_VALUE
          ExceptionTable:
            52 to 552 -> 578 [1] lasti
            578 to 584 -> 586 [3] lasti
            592 to 592 -> 586 [3] lasti
          consts
             None
@@ -1756,37 +1764,37 @@
                nlocals   : 1
                stacksize : 2
                flags     : 19
                code
                   0x97007c0064011900000000000000000064026b04000000007202640353
                   007c0064041900000000000000000064056b040000000072026406530064
                   075300
-               290           0 RESUME                   0
+               286           0 RESUME                   0
                
-               291           2 LOAD_FAST                0 (row)
+               287           2 LOAD_FAST                0 (row)
                              4 LOAD_CONST               1 ('recent_validate_count')
                              6 BINARY_SUBSCR
                             16 LOAD_CONST               2 (0)
                             18 COMPARE_OP               4 (>)
                             24 POP_JUMP_FORWARD_IF_FALSE     2 (to 30)
                
-               292          26 LOAD_CONST               3 ('Trending Searches')
+               288          26 LOAD_CONST               3 ('Trending Searches')
                             28 RETURN_VALUE
                
-               293     >>   30 LOAD_FAST                0 (row)
+               289     >>   30 LOAD_FAST                0 (row)
                             32 LOAD_CONST               4 ('total_validate_count')
                             34 BINARY_SUBSCR
                             44 LOAD_CONST               5 (25)
                             46 COMPARE_OP               4 (>)
                             52 POP_JUMP_FORWARD_IF_FALSE     2 (to 58)
                
-               294          54 LOAD_CONST               6 ('Top Searches')
+               290          54 LOAD_CONST               6 ('Top Searches')
                             56 RETURN_VALUE
                
-               296     >>   58 LOAD_CONST               7 ('All Searches')
+               292     >>   58 LOAD_CONST               7 ('All Searches')
                             60 RETURN_VALUE
                consts
                   None
                   'recent_validate_count'
                   0
                   'Trending Searches'
                   'total_validate_count'
@@ -1795,30 +1803,30 @@
                   'All Searches'
                names      ()
                varnames   ('row',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       '_set_group'
-               firstlineno 290
+               firstlineno 286
                lnotab 0x02011801040118010402
             1
             ('axis',)
             'group'
             ('group', 'recent_validate_count', 'total_validate_count', 'label')
             (False, False, False, True)
             ('by', 'ascending')
             ''
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'merge', 'top_actor_per_search', 'apply', 'search_event_count_by_type', 'sort_values', 'fillna')
          varnames   ('conn', 'statement', 'result', 'df', '_set_group')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search'
-         firstlineno 269
+         firstlineno 265
          lnotab
             0x02013401040c4e017402180120ff1204060834024a021801060106fe12
             052adb2e27
       code
          argcount  : 0
          nlocals   : 3
          stacksize : 6
@@ -1832,66 +1840,66 @@
             00000000007c01a0070000000000000000000000000000000000000000a6
             000000ab0000000000000000007c01a00800000000000000000000000000
             00000000000000a6000000ab000000000000000000ac02a6020000ab0200
             000000000000007d027c02a0090000000000000000000000000000000000
             00000067006403a201ac02a6010000ab0100000000000000007d027c0263
             02640064006400a6020000ab020000000000000000010053002300310073
             047702780359007701010059000100010064005300
-         311           0 RESUME                   0
+         307           0 RESUME                   0
          
-         312           2 LOAD_GLOBAL              0 (db)
+         308           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         313          54 LOAD_FAST                0 (conn)
+         309          54 LOAD_FAST                0 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         314          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         310          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         315         100 LOAD_CONST               1 ('\n                SELECT * FROM actor\n                ')
+         311         100 LOAD_CONST               1 ('\n                SELECT * FROM actor\n                ')
          
-         314         102 PRECALL                  1
+         310         102 PRECALL                  1
                      106 CALL                     1
          
-         313         116 PRECALL                  1
+         309         116 PRECALL                  1
                      120 CALL                     1
                      130 STORE_FAST               1 (result)
          
-         320         132 LOAD_GLOBAL             11 (NULL + pd)
+         316         132 LOAD_GLOBAL             11 (NULL + pd)
                      144 LOAD_ATTR                6 (DataFrame)
                      154 LOAD_FAST                1 (result)
                      156 LOAD_METHOD              7 (fetchall)
                      178 PRECALL                  0
                      182 CALL                     0
                      192 LOAD_FAST                1 (result)
                      194 LOAD_METHOD              8 (keys)
                      216 PRECALL                  0
                      220 CALL                     0
                      230 KW_NAMES                 2
                      232 PRECALL                  2
                      236 CALL                     2
                      246 STORE_FAST               2 (df)
          
-         321         248 LOAD_FAST                2 (df)
+         317         248 LOAD_FAST                2 (df)
                      250 LOAD_METHOD              9 (drop)
                      272 BUILD_LIST               0
                      274 LOAD_CONST               3 (('id', 'created', 'updated'))
                      276 LIST_EXTEND              1
                      278 KW_NAMES                 2
                      280 PRECALL                  1
                      284 CALL                     1
                      294 STORE_FAST               2 (df)
          
-         322         296 LOAD_FAST                2 (df)
+         318         296 LOAD_FAST                2 (df)
          
-         312         298 SWAP                     2
+         308         298 SWAP                     2
                      300 LOAD_CONST               0 (None)
                      302 LOAD_CONST               0 (None)
                      304 LOAD_CONST               0 (None)
                      306 PRECALL                  2
                      310 CALL                     2
                      320 POP_TOP
                      322 RETURN_VALUE
@@ -1919,15 +1927,15 @@
             ('id', 'created', 'updated')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'drop')
          varnames   ('conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'actor'
-         firstlineno 311
+         firstlineno 307
          lnotab 0x020134011801160102ff0eff10077401300102f6
       code
          argcount  : 2
          nlocals   : 8
          stacksize : 7
          flags     : 3
          code
@@ -1950,60 +1958,60 @@
             00000000000000a00e000000000000000000000000000000000000000064
             086405a6020000ab0200000000000000007c076a0d0000000000000000a0
             0e00000000000000000000000000000000000000006409a6010000ab0100
             00000000000000640a6b0200000000ac0ba6020000ab0200000000000000
             007d05740b000000000000000000006a0f00000000000000007c05640c19
             000000000000000000a6010000ab0100000000000000007c05640c3c0000
             007c055300
-         325           0 RESUME                   0
+         321           0 RESUME                   0
          
-         326           2 LOAD_CONST               1 ("\n        SELECT \n            e.id, \n            e.search_uid, \n            e.domain, \n            e.data, \n            e.type AS last_event_type, \n            e.created AS updated,\n            a.name AS updated_by,\n            c.name as name,\n            c.uid as dealcloud_id,\n            c.description as description,\n            c.meta as meta,\n            (c.meta->>'employees') AS employees,\n            (c.meta->>'ownership') AS ownership,\n            (c.meta->>'linkedin') AS linkedin,\n            (r.data->>'rating') AS rating\n        FROM (\n            SELECT \n                search_uid, \n                domain, \n                MAX(created) AS max_created\n            FROM \n                event\n            WHERE \n                type NOT IN ('comment','rating','generate','criteria')\n                AND search_uid = :search_uid\n            GROUP BY \n                domain, search_uid\n        ) AS max_event\n        JOIN event e ON e.domain = max_event.domain AND e.created = max_event.max_created AND e.search_uid = max_event.search_uid \n        JOIN company c ON c.domain = e.domain\n        JOIN actor a ON a.key = e.actor_key\n        LEFT JOIN (\n            SELECT \n                search_uid,\n                domain, \n                MAX(created) AS max_created\n            FROM \n                event\n            WHERE \n                type = 'rating'\n            GROUP BY \n                domain, search_uid\n        ) AS max_rating ON e.domain = max_rating.domain AND e.search_uid = max_rating.search_uid\n        LEFT JOIN event r ON r.domain = max_rating.domain AND r.created = max_rating.max_created;\n    ")
+         322           2 LOAD_CONST               1 ("\n        SELECT \n            e.id, \n            e.search_uid, \n            e.domain, \n            e.data, \n            e.type AS last_event_type, \n            e.created AS updated,\n            a.name AS updated_by,\n            c.name as name,\n            c.uid as dealcloud_id,\n            c.description as description,\n            c.meta as meta,\n            (c.meta->>'employees') AS employees,\n            (c.meta->>'ownership') AS ownership,\n            (c.meta->>'linkedin') AS linkedin,\n            (r.data->>'rating') AS rating\n        FROM (\n            SELECT \n                search_uid, \n                domain, \n                MAX(created) AS max_created\n            FROM \n                event\n            WHERE \n                type NOT IN ('comment','rating','generate','criteria')\n                AND search_uid = :search_uid\n            GROUP BY \n                domain, search_uid\n        ) AS max_event\n        JOIN event e ON e.domain = max_event.domain AND e.created = max_event.max_created AND e.search_uid = max_event.search_uid \n        JOIN company c ON c.domain = e.domain\n        JOIN actor a ON a.key = e.actor_key\n        LEFT JOIN (\n            SELECT \n                search_uid,\n                domain, \n                MAX(created) AS max_created\n            FROM \n                event\n            WHERE \n                type = 'rating'\n            GROUP BY \n                domain, search_uid\n        ) AS max_rating ON e.domain = max_rating.domain AND e.search_uid = max_rating.search_uid\n        LEFT JOIN event r ON r.domain = max_rating.domain AND r.created = max_rating.max_created;\n    ")
                        4 STORE_FAST               2 (statement)
          
-         373           6 LOAD_GLOBAL              0 (db)
+         369           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 BEFORE_WITH
                       56 STORE_FAST               3 (conn)
          
-         374          58 LOAD_FAST                3 (conn)
+         370          58 LOAD_FAST                3 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         375          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         371          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         376         120 LOAD_FAST                0 (search_uid)
+         372         120 LOAD_FAST                0 (search_uid)
                      122 LOAD_FAST                1 (last_event_type)
                      124 LOAD_CONST               2 (('search_uid', 'last_event_type'))
                      126 BUILD_CONST_KEY_MAP      2
          
-         374         128 PRECALL                  2
+         370         128 PRECALL                  2
                      132 CALL                     2
                      142 STORE_FAST               4 (result)
          
-         378         144 LOAD_GLOBAL             11 (NULL + pd)
+         374         144 LOAD_GLOBAL             11 (NULL + pd)
                      156 LOAD_ATTR                6 (DataFrame)
                      166 LOAD_FAST                4 (result)
                      168 LOAD_METHOD              7 (fetchall)
                      190 PRECALL                  0
                      194 CALL                     0
                      204 LOAD_FAST                4 (result)
                      206 LOAD_METHOD              8 (keys)
                      228 PRECALL                  0
                      232 CALL                     0
                      242 KW_NAMES                 3
                      244 PRECALL                  2
                      248 CALL                     2
                      258 STORE_FAST               5 (targets)
          
-         373         260 LOAD_CONST               0 (None)
+         369         260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 LOAD_CONST               0 (None)
                      266 PRECALL                  2
                      270 CALL                     2
                      280 POP_TOP
                      282 JUMP_FORWARD            11 (to 306)
                  >>  284 PUSH_EXC_INFO
@@ -2014,82 +2022,82 @@
                      294 POP_EXCEPT
                      296 RERAISE                  1
                  >>  298 POP_TOP
                      300 POP_EXCEPT
                      302 POP_TOP
                      304 POP_TOP
          
-         380     >>  306 LOAD_FAST                5 (targets)
+         376     >>  306 LOAD_FAST                5 (targets)
                      308 LOAD_FAST                5 (targets)
                      310 LOAD_CONST               4 ('last_event_type')
                      312 BINARY_SUBSCR
                      322 LOAD_FAST                1 (last_event_type)
                      324 COMPARE_OP               2 (==)
                      330 BINARY_SUBSCR
                      340 STORE_FAST               5 (targets)
          
-         381         342 LOAD_GLOBAL             19 (NULL + comment_by_domain)
+         377         342 LOAD_GLOBAL             19 (NULL + comment_by_domain)
                      354 LOAD_FAST                0 (search_uid)
                      356 PRECALL                  1
                      360 CALL                     1
                      370 STORE_FAST               6 (comments)
          
-         382         372 LOAD_FAST                5 (targets)
+         378         372 LOAD_FAST                5 (targets)
                      374 LOAD_METHOD             10 (merge)
                      396 LOAD_FAST                6 (comments)
                      398 LOAD_CONST               5 ('domain')
                      400 LOAD_CONST               6 ('left')
                      402 KW_NAMES                 7
                      404 PRECALL                  3
                      408 CALL                     3
                      418 STORE_FAST               5 (targets)
          
-         385         420 LOAD_GLOBAL             23 (NULL + find_search_by_uid)
+         381         420 LOAD_GLOBAL             23 (NULL + find_search_by_uid)
                      432 LOAD_FAST                0 (search_uid)
                      434 PRECALL                  1
                      438 CALL                     1
                      448 STORE_FAST               7 (search)
          
-         386         450 LOAD_FAST                5 (targets)
+         382         450 LOAD_FAST                5 (targets)
                      452 LOAD_METHOD             12 (sort_values)
          
-         387         474 LOAD_FAST                7 (search)
+         383         474 LOAD_FAST                7 (search)
                      476 LOAD_ATTR               13 (sort)
                      486 LOAD_METHOD             14 (get)
                      508 LOAD_CONST               8 ('field')
                      510 LOAD_CONST               5 ('domain')
                      512 PRECALL                  2
                      516 CALL                     2
          
-         388         526 LOAD_FAST                7 (search)
+         384         526 LOAD_FAST                7 (search)
                      528 LOAD_ATTR               13 (sort)
                      538 LOAD_METHOD             14 (get)
                      560 LOAD_CONST               9 ('order')
                      562 PRECALL                  1
                      566 CALL                     1
                      576 LOAD_CONST              10 ('asc')
                      578 COMPARE_OP               2 (==)
          
-         386         584 KW_NAMES                11
+         382         584 KW_NAMES                11
                      586 PRECALL                  2
                      590 CALL                     2
                      600 STORE_FAST               5 (targets)
          
-         390         602 LOAD_GLOBAL             11 (NULL + pd)
+         386         602 LOAD_GLOBAL             11 (NULL + pd)
                      614 LOAD_ATTR               15 (to_numeric)
                      624 LOAD_FAST                5 (targets)
                      626 LOAD_CONST              12 ('employees')
                      628 BINARY_SUBSCR
                      638 PRECALL                  1
                      642 CALL                     1
                      652 LOAD_FAST                5 (targets)
                      654 LOAD_CONST              12 ('employees')
                      656 STORE_SUBSCR
          
-         391         660 LOAD_FAST                5 (targets)
+         387         660 LOAD_FAST                5 (targets)
                      662 RETURN_VALUE
          ExceptionTable:
            56 to 258 -> 284 [1] lasti
            284 to 290 -> 292 [3] lasti
            298 to 298 -> 292 [3] lasti
          consts
             None
@@ -2107,15 +2115,15 @@
             'employees'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'comment_by_domain', 'merge', 'find_search_by_uid', 'sort_values', 'sort', 'get', 'to_numeric')
          varnames   ('search_uid', 'last_event_type', 'statement', 'conn', 'result', 'targets', 'comments', 'search')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search_target_by_last_event_type'
-         firstlineno 325
+         firstlineno 321
          lnotab
             0x0201042f34011801260108fe100474fb2e0724011e0130031e01180134
             013afe12043a01
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
@@ -2128,59 +2136,59 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640464046404a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         394           0 RESUME                   0
+         390           0 RESUME                   0
          
-         397           2 LOAD_CONST               1 ("\n        SELECT \n            e.id, \n            e.search_uid, \n            e.domain, \n            e.type AS last_event_type, \n            to_timestamp(e.created) AS updated,\n            c.meta as meta,\n            (r.data->>'rating') AS rating\n        FROM (\n            SELECT \n                search_uid, \n                domain, \n                MAX(created) AS max_created\n            FROM \n                event\n            WHERE \n                type NOT IN ('comment','rating','generate','criteria') \n                AND search_uid = :search_uid\n            GROUP BY \n                domain, search_uid\n        ) AS max_event\n        JOIN event e ON e.domain = max_event.domain AND e.created = max_event.max_created AND e.search_uid = max_event.search_uid \n        JOIN company c ON c.domain = e.domain\n        LEFT JOIN (\n            SELECT \n                search_uid,\n                domain, \n                MAX(created) AS max_created\n            FROM \n                event\n            WHERE \n                type = 'rating'\n            GROUP BY \n                domain, search_uid\n        ) AS max_rating ON e.domain = max_rating.domain AND e.search_uid = max_rating.search_uid\n        LEFT JOIN event r ON r.domain = max_rating.domain AND r.created = max_rating.max_created;\n    ")
+         393           2 LOAD_CONST               1 ("\n        SELECT \n            e.id, \n            e.search_uid, \n            e.domain, \n            e.type AS last_event_type, \n            to_timestamp(e.created) AS updated,\n            c.meta as meta,\n            (r.data->>'rating') AS rating\n        FROM (\n            SELECT \n                search_uid, \n                domain, \n                MAX(created) AS max_created\n            FROM \n                event\n            WHERE \n                type NOT IN ('comment','rating','generate','criteria') \n                AND search_uid = :search_uid\n            GROUP BY \n                domain, search_uid\n        ) AS max_event\n        JOIN event e ON e.domain = max_event.domain AND e.created = max_event.max_created AND e.search_uid = max_event.search_uid \n        JOIN company c ON c.domain = e.domain\n        LEFT JOIN (\n            SELECT \n                search_uid,\n                domain, \n                MAX(created) AS max_created\n            FROM \n                event\n            WHERE \n                type = 'rating'\n            GROUP BY \n                domain, search_uid\n        ) AS max_rating ON e.domain = max_rating.domain AND e.search_uid = max_rating.search_uid\n        LEFT JOIN event r ON r.domain = max_rating.domain AND r.created = max_rating.max_created;\n    ")
                        4 STORE_FAST               1 (statement)
          
-         435           6 LOAD_GLOBAL              0 (db)
+         431           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 BEFORE_WITH
                       56 STORE_FAST               2 (conn)
          
-         436          58 LOAD_FAST                2 (conn)
+         432          58 LOAD_FAST                2 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         437          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         433          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                1 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         438         120 LOAD_CONST               2 ('search_uid')
+         434         120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
          
-         436         126 PRECALL                  2
+         432         126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         440         142 LOAD_GLOBAL             11 (NULL + pd)
+         436         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (targets)
          
-         435         258 LOAD_CONST               4 (None)
+         431         258 LOAD_CONST               4 (None)
                      260 LOAD_CONST               4 (None)
                      262 LOAD_CONST               4 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -2191,15 +2199,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         449     >>  304 LOAD_FAST                4 (targets)
+         445     >>  304 LOAD_FAST                4 (targets)
                      306 RETURN_VALUE
          ExceptionTable:
            56 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             'Returns all the targets not in rejected or created'
@@ -2209,15 +2217,15 @@
             None
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'statement', 'conn', 'result', 'targets')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search_target_export'
-         firstlineno 394
+         firstlineno 390
          lnotab 0x0203042634011801260106fe100474fb2e0e
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -2228,59 +2236,59 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         453           0 RESUME                   0
+         449           0 RESUME                   0
          
-         454           2 LOAD_GLOBAL              0 (db)
+         450           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         455          54 LOAD_CONST               1 ("\n            SELECT \n                e.type AS last_event_type,\n                COUNT(e.type)\n            FROM (\n                SELECT \n                    search_uid, \n                    domain, \n                    MAX(created) AS max_created\n                FROM \n                    event\n                WHERE \n                    type NOT IN ('comment','rating','generate','criteria')\n                    and search_uid = :search_uid\n                GROUP BY \n                    domain, search_uid\n            ) AS max_event\n            JOIN event e ON e.domain = max_event.domain AND e.created = max_event.max_created AND e.search_uid = max_event.search_uid\n            GROUP BY e.type;\n        ")
+         451          54 LOAD_CONST               1 ("\n            SELECT \n                e.type AS last_event_type,\n                COUNT(e.type)\n            FROM (\n                SELECT \n                    search_uid, \n                    domain, \n                    MAX(created) AS max_created\n                FROM \n                    event\n                WHERE \n                    type NOT IN ('comment','rating','generate','criteria')\n                    and search_uid = :search_uid\n                GROUP BY \n                    domain, search_uid\n            ) AS max_event\n            JOIN event e ON e.domain = max_event.domain AND e.created = max_event.max_created AND e.search_uid = max_event.search_uid\n            GROUP BY e.type;\n        ")
                       56 STORE_FAST               2 (statement)
          
-         475          58 LOAD_FAST                1 (conn)
+         471          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         476          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         472          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         477         120 LOAD_CONST               2 ('search_uid')
+         473         120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
          
-         475         126 PRECALL                  2
+         471         126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         479         142 LOAD_GLOBAL             11 (NULL + pd)
+         475         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (df)
          
-         454         258 LOAD_CONST               0 (None)
+         450         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -2291,15 +2299,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         480     >>  304 LOAD_FAST                4 (df)
+         476     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            52 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -2308,15 +2316,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'target_count'
-         firstlineno 453
+         firstlineno 449
          lnotab 0x0201340104141801260106fe100474e72e1a
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -2327,56 +2335,56 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         483           0 RESUME                   0
+         479           0 RESUME                   0
          
-         484           2 LOAD_GLOBAL              0 (db)
+         480           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         485          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
+         481          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
                       56 STORE_FAST               2 (statement)
          
-         490          58 LOAD_FAST                1 (conn)
+         486          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         491         142 LOAD_GLOBAL             11 (NULL + pd)
+         487         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (df)
          
-         484         258 LOAD_CONST               0 (None)
+         480         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -2387,15 +2395,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         492     >>  304 LOAD_FAST                4 (df)
+         488     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            52 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -2404,15 +2412,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'event'
-         firstlineno 483
+         firstlineno 479
          lnotab 0x020134010405540174f92e08
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -2423,56 +2431,56 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         495           0 RESUME                   0
+         491           0 RESUME                   0
          
-         496           2 LOAD_GLOBAL              0 (db)
+         492           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         497          54 LOAD_CONST               1 ('\n                SELECT distinct(domain)\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
+         493          54 LOAD_CONST               1 ('\n                SELECT distinct(domain)\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
                       56 STORE_FAST               2 (statement)
          
-         502          58 LOAD_FAST                1 (conn)
+         498          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         503         142 LOAD_GLOBAL             11 (NULL + pd)
+         499         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (df)
          
-         496         258 LOAD_CONST               0 (None)
+         492         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -2483,15 +2491,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         504     >>  304 LOAD_FAST                4 (df)
+         500     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            52 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -2500,15 +2508,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'unique_domains'
-         firstlineno 495
+         firstlineno 491
          lnotab 0x020134010405540174f92e08
       code
          argcount  : 0
          nlocals   : 4
          stacksize : 6
          flags     : 3
          code
@@ -2519,53 +2527,53 @@
             00a6010000ab0100000000000000007d02740b000000000000000000006a
             0600000000000000007c02a0070000000000000000000000000000000000
             000000a6000000ab0000000000000000007c02a008000000000000000000
             0000000000000000000000a6000000ab000000000000000000ac02a60200
             00ab0200000000000000007d03640064006400a6020000ab020000000000
             00000001006e0b230031007304770278035900770101005900010001007c
             035300
-         507           0 RESUME                   0
+         503           0 RESUME                   0
          
-         508           2 LOAD_GLOBAL              0 (db)
+         504           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         509          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n            ')
+         505          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n            ')
                       56 STORE_FAST               1 (statement)
          
-         513          58 LOAD_FAST                0 (conn)
+         509          58 LOAD_FAST                0 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                1 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 PRECALL                  1
                      124 CALL                     1
                      134 STORE_FAST               2 (result)
          
-         514         136 LOAD_GLOBAL             11 (NULL + pd)
+         510         136 LOAD_GLOBAL             11 (NULL + pd)
                      148 LOAD_ATTR                6 (DataFrame)
                      158 LOAD_FAST                2 (result)
                      160 LOAD_METHOD              7 (fetchall)
                      182 PRECALL                  0
                      186 CALL                     0
                      196 LOAD_FAST                2 (result)
                      198 LOAD_METHOD              8 (keys)
                      220 PRECALL                  0
                      224 CALL                     0
                      234 KW_NAMES                 2
                      236 PRECALL                  2
                      240 CALL                     2
                      250 STORE_FAST               3 (df)
          
-         508         252 LOAD_CONST               0 (None)
+         504         252 LOAD_CONST               0 (None)
                      254 LOAD_CONST               0 (None)
                      256 LOAD_CONST               0 (None)
                      258 PRECALL                  2
                      262 CALL                     2
                      272 POP_TOP
                      274 JUMP_FORWARD            11 (to 298)
                  >>  276 PUSH_EXC_INFO
@@ -2576,15 +2584,15 @@
                      286 POP_EXCEPT
                      288 RERAISE                  1
                  >>  290 POP_TOP
                      292 POP_EXCEPT
                      294 POP_TOP
                      296 POP_TOP
          
-         515     >>  298 LOAD_FAST                3 (df)
+         511     >>  298 LOAD_FAST                3 (df)
                      300 RETURN_VALUE
          ExceptionTable:
            52 to 250 -> 276 [1] lasti
            276 to 282 -> 284 [3] lasti
            290 to 290 -> 284 [3] lasti
          consts
             None
@@ -2592,15 +2600,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'company'
-         firstlineno 507
+         firstlineno 503
          lnotab 0x0201340104044e0174fa2e07
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -2611,56 +2619,56 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         518           0 RESUME                   0
+         514           0 RESUME                   0
          
-         519           2 LOAD_GLOBAL              0 (db)
+         515           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         520          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM checkpoint\n                JOIN event ON checkpoint.event_id = event.id\n                WHERE search_uid = :search_uid\n            ')
+         516          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM checkpoint\n                JOIN event ON checkpoint.event_id = event.id\n                WHERE search_uid = :search_uid\n            ')
                       56 STORE_FAST               2 (statement)
          
-         526          58 LOAD_FAST                1 (conn)
+         522          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         527         142 LOAD_GLOBAL             11 (NULL + pd)
+         523         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (df)
          
-         519         258 LOAD_CONST               0 (None)
+         515         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -2671,15 +2679,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         528     >>  304 LOAD_FAST                4 (df)
+         524     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            52 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -2688,15 +2696,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'checkpoint'
-         firstlineno 518
+         firstlineno 514
          lnotab 0x020134010406540174f82e09
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -2711,59 +2719,59 @@
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c04a009000000000000000000000000000000000000000064
             04a6010000ab010000000000000000a00a00000000000000000000000000
             000000000000006405640684006901a6010000ab010000000000000000a0
             0b0000000000000000000000000000000000000000a6000000ab00000000
             00000000005300
-         531           0 RESUME                   0
+         527           0 RESUME                   0
          
-         532           2 LOAD_GLOBAL              0 (db)
+         528           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         533          54 LOAD_CONST               1 ("\n                SELECT *, data->>'comment' AS comment\n                FROM event e\n                WHERE \n                    search_uid = :search_uid AND\n                    type = 'comment'\n            ")
+         529          54 LOAD_CONST               1 ("\n                SELECT *, data->>'comment' AS comment\n                FROM event e\n                WHERE \n                    search_uid = :search_uid AND\n                    type = 'comment'\n            ")
                       56 STORE_FAST               2 (statement)
          
-         540          58 LOAD_FAST                1 (conn)
+         536          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         541          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         537          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         542         120 LOAD_CONST               2 ('search_uid')
+         538         120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
          
-         540         126 PRECALL                  2
+         536         126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         544         142 LOAD_GLOBAL             11 (NULL + pd)
+         540         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (df)
          
-         532         258 LOAD_CONST               0 (None)
+         528         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -2774,22 +2782,22 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         546     >>  304 LOAD_FAST                4 (df)
+         542     >>  304 LOAD_FAST                4 (df)
                      306 LOAD_METHOD              9 (groupby)
                      328 LOAD_CONST               4 ('domain')
                      330 PRECALL                  1
                      334 CALL                     1
                      344 LOAD_METHOD             10 (agg)
                      366 LOAD_CONST               5 ('comment')
-                     368 LOAD_CONST               6 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 546>)
+                     368 LOAD_CONST               6 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 542>)
                      370 MAKE_FUNCTION            0
                      372 BUILD_MAP                1
                      374 PRECALL                  1
                      378 CALL                     1
                      388 LOAD_METHOD             11 (reset_index)
                      410 PRECALL                  0
                      414 CALL                     0
@@ -2809,37 +2817,37 @@
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 19
                code
                   0x97007401000000000000000000007c00a6010000ab0100000000000000
                   005300
-               546           0 RESUME                   0
+               542           0 RESUME                   0
                              2 LOAD_GLOBAL              1 (NULL + list)
                             14 LOAD_FAST                0 (x)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 RETURN_VALUE
                consts
                   None
                names      ('list',)
                varnames   ('x',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       '<lambda>'
-               firstlineno 546
+               firstlineno 542
                lnotab 0x
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'groupby', 'agg', 'reset_index')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'comment_by_domain'
-         firstlineno 531
+         firstlineno 527
          lnotab 0x0201340104071801260106fe100474f42e0e
       code
          argcount  : 1
          nlocals   : 6
          stacksize : 7
          flags     : 3
          code
@@ -2854,41 +2862,41 @@
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000007c04a6020000ab0200000000000000007d05741900
             0000000000000000007c056a0d0000000000000000a6010000ab01000000
             000000000001007c055300
-         552           0 RESUME                   0
+         548           0 RESUME                   0
          
-         553           2 LOAD_GLOBAL              0 (db)
+         549           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         554          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM search\n                WHERE uid = :search_uid\n            ')
+         550          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM search\n                WHERE uid = :search_uid\n            ')
                       56 STORE_FAST               2 (statement)
          
-         559          58 LOAD_FAST                1 (conn)
+         555          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         553         142 LOAD_CONST               0 (None)
+         549         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -2899,24 +2907,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         561     >>  188 LOAD_FAST                3 (result)
+         557     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         562         210 LOAD_CONST               0 (None)
+         558         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         564     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         560     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -2924,29 +2932,29 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         565         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         561         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (Search)
                      368 LOAD_FAST                4 (obj)
                      370 PRECALL                  2
                      374 CALL                     2
                      384 STORE_FAST               5 (search)
          
-         566         386 LOAD_GLOBAL             25 (NULL + print)
+         562         386 LOAD_GLOBAL             25 (NULL + print)
                      398 LOAD_FAST                5 (search)
                      400 LOAD_ATTR               13 (label)
                      410 PRECALL                  1
                      414 CALL                     1
                      424 POP_TOP
          
-         567         426 LOAD_FAST                5 (search)
+         563         426 LOAD_FAST                5 (search)
                      428 RETURN_VALUE
          ExceptionTable:
            52 to 140 -> 166 [1] lasti
            166 to 172 -> 174 [3] lasti
            180 to 180 -> 174 [3] lasti
          consts
             None
@@ -2955,15 +2963,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Search', 'print', 'label')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'obj', 'search')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_search_by_uid'
-         firstlineno 552
+         firstlineno 548
          lnotab 0x02013401040554fa2e081601040282012a012801
       'domain'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -2977,41 +2985,41 @@
             0101005900010001007c036a05000000000000000064036b020000000072
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000007c04a6020000ab0200000000000000005300
-         570           0 RESUME                   0
+         566           0 RESUME                   0
          
-         571           2 LOAD_GLOBAL              0 (db)
+         567           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         572          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n                WHERE domain = :domain\n            ')
+         568          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n                WHERE domain = :domain\n            ')
                       56 STORE_FAST               2 (statement)
          
-         577          58 LOAD_FAST                1 (conn)
+         573          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('domain')
                      122 LOAD_FAST                0 (domain)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         571         142 LOAD_CONST               0 (None)
+         567         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -3022,24 +3030,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         579     >>  188 LOAD_FAST                3 (result)
+         575     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         580         210 LOAD_CONST               0 (None)
+         576         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         582     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         578     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -3047,15 +3055,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         583         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         579         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (Company)
                      368 LOAD_FAST                4 (obj)
                      370 PRECALL                  2
                      374 CALL                     2
                      384 RETURN_VALUE
          ExceptionTable:
            52 to 140 -> 166 [1] lasti
@@ -3068,15 +3076,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Company')
          varnames   ('domain', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_company_by_domain'
-         firstlineno 570
+         firstlineno 566
          lnotab 0x02013401040554fa2e08160104028201
       'event_id'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -3090,41 +3098,41 @@
             0101005900010001007c036a05000000000000000064036b020000000072
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000007c04a6020000ab0200000000000000005300
-         586           0 RESUME                   0
+         582           0 RESUME                   0
          
-         587           2 LOAD_GLOBAL              0 (db)
+         583           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         588          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE id = :event_id\n            ')
+         584          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE id = :event_id\n            ')
                       56 STORE_FAST               2 (statement)
          
-         593          58 LOAD_FAST                1 (conn)
+         589          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('event_id')
                      122 LOAD_FAST                0 (event_id)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         587         142 LOAD_CONST               0 (None)
+         583         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -3135,24 +3143,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         595     >>  188 LOAD_FAST                3 (result)
+         591     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         596         210 LOAD_CONST               0 (None)
+         592         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         598     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         594     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -3160,15 +3168,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         599         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         595         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (Event)
                      368 LOAD_FAST                4 (obj)
                      370 PRECALL                  2
                      374 CALL                     2
                      384 RETURN_VALUE
          ExceptionTable:
            52 to 140 -> 166 [1] lasti
@@ -3181,15 +3189,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Event')
          varnames   ('event_id', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_event_by_id'
-         firstlineno 586
+         firstlineno 582
          lnotab 0x02013401040554fa2e08160104028201
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 11
          flags     : 3
          code
@@ -3200,68 +3208,68 @@
             007c006a0500000000000000007c006a0600000000000000007c006a0700
             000000000000007c006a0800000000000000007413000000000000000000
             006a0a00000000000000007c006a0b0000000000000000a6010000ab0100
             0000000000000064029c05a6020000ab02000000000000000001007c01a0
             0c0000000000000000000000000000000000000000a6000000ab00000000
             00000000000100640064006400a6020000ab020000000000000000010064
             0053002300310073047702780359007701010059000100010064005300
-         605           0 RESUME                   0
+         601           0 RESUME                   0
          
-         606           2 LOAD_GLOBAL              0 (db)
+         602           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         607          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                uid = :uid,\n                name = :name,\n                description = :description,\n                meta = :meta,\n                updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n            WHERE domain = :domain\n            ')
+         603          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                uid = :uid,\n                name = :name,\n                description = :description,\n                meta = :meta,\n                updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n            WHERE domain = :domain\n            ')
                       56 STORE_FAST               2 (statement)
          
-         618          58 LOAD_FAST                1 (conn)
+         614          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         619          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         615          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         621         120 LOAD_FAST                0 (company)
+         617         120 LOAD_FAST                0 (company)
                      122 LOAD_ATTR                5 (uid)
          
-         622         132 LOAD_FAST                0 (company)
+         618         132 LOAD_FAST                0 (company)
                      134 LOAD_ATTR                6 (name)
          
-         623         144 LOAD_FAST                0 (company)
+         619         144 LOAD_FAST                0 (company)
                      146 LOAD_ATTR                7 (description)
          
-         624         156 LOAD_FAST                0 (company)
+         620         156 LOAD_FAST                0 (company)
                      158 LOAD_ATTR                8 (domain)
          
-         625         168 LOAD_GLOBAL             19 (NULL + json)
+         621         168 LOAD_GLOBAL             19 (NULL + json)
                      180 LOAD_ATTR               10 (dumps)
                      190 LOAD_FAST                0 (company)
                      192 LOAD_ATTR               11 (meta)
                      202 PRECALL                  1
                      206 CALL                     1
          
-         620         216 LOAD_CONST               2 (('uid', 'name', 'description', 'domain', 'meta'))
+         616         216 LOAD_CONST               2 (('uid', 'name', 'description', 'domain', 'meta'))
                      218 BUILD_CONST_KEY_MAP      5
          
-         618         220 PRECALL                  2
+         614         220 PRECALL                  2
                      224 CALL                     2
                      234 POP_TOP
          
-         629         236 LOAD_FAST                1 (conn)
+         625         236 LOAD_FAST                1 (conn)
                      238 LOAD_METHOD             12 (commit)
                      260 PRECALL                  0
                      264 CALL                     0
                      274 POP_TOP
          
-         606         276 LOAD_CONST               0 (None)
+         602         276 LOAD_CONST               0 (None)
                      278 LOAD_CONST               0 (None)
                      280 LOAD_CONST               0 (None)
                      282 PRECALL                  2
                      286 CALL                     2
                      296 POP_TOP
                      298 LOAD_CONST               0 (None)
                      300 RETURN_VALUE
@@ -3288,15 +3296,15 @@
             ('uid', 'name', 'description', 'domain', 'meta')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'uid', 'name', 'description', 'domain', 'json', 'dumps', 'meta', 'commit')
          varnames   ('company', 'conn', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_company'
-         firstlineno 605
+         firstlineno 601
          lnotab 0x02013401040b180126020c010c010c010c0130fb04fe100b28e9
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 10
          flags     : 3
          code
@@ -3311,79 +3319,79 @@
             00000000000000a6010000ab010000000000000000740b00000000000000
             0000006a0600000000000000007c006a0a0000000000000000a6010000ab
             0100000000000000007c006a0b000000000000000064029c05a6020000ab
             02000000000000000001007c01a00c000000000000000000000000000000
             0000000000a6000000ab0000000000000000000100640064006400a60200
             00ab02000000000000000001006400530023003100730477027803590077
             01010059000100010064005300
-         632           0 RESUME                   0
+         628           0 RESUME                   0
          
-         633           2 LOAD_GLOBAL              0 (db)
+         629           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         634          54 LOAD_FAST                1 (conn)
+         630          54 LOAD_FAST                1 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         635          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         631          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         636         100 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    sort = :sort,\n                    inclusion = :inclusion,\n                    exclusion = :exclusion,\n                    meta = :meta,\n                    updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n                WHERE uid = :uid\n                ')
+         632         100 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    sort = :sort,\n                    inclusion = :inclusion,\n                    exclusion = :exclusion,\n                    meta = :meta,\n                    updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n                WHERE uid = :uid\n                ')
          
-         635         102 PRECALL                  1
+         631         102 PRECALL                  1
                      106 CALL                     1
          
-         648         116 LOAD_GLOBAL             11 (NULL + json)
+         644         116 LOAD_GLOBAL             11 (NULL + json)
                      128 LOAD_ATTR                6 (dumps)
                      138 LOAD_FAST                0 (search)
                      140 LOAD_ATTR                7 (sort)
                      150 PRECALL                  1
                      154 CALL                     1
          
-         649         164 LOAD_GLOBAL             11 (NULL + json)
+         645         164 LOAD_GLOBAL             11 (NULL + json)
                      176 LOAD_ATTR                6 (dumps)
                      186 LOAD_FAST                0 (search)
                      188 LOAD_ATTR                8 (inclusion)
                      198 PRECALL                  1
                      202 CALL                     1
          
-         650         212 LOAD_GLOBAL             11 (NULL + json)
+         646         212 LOAD_GLOBAL             11 (NULL + json)
                      224 LOAD_ATTR                6 (dumps)
                      234 LOAD_FAST                0 (search)
                      236 LOAD_ATTR                9 (exclusion)
                      246 PRECALL                  1
                      250 CALL                     1
          
-         651         260 LOAD_GLOBAL             11 (NULL + json)
+         647         260 LOAD_GLOBAL             11 (NULL + json)
                      272 LOAD_ATTR                6 (dumps)
                      282 LOAD_FAST                0 (search)
                      284 LOAD_ATTR               10 (meta)
                      294 PRECALL                  1
                      298 CALL                     1
          
-         652         308 LOAD_FAST                0 (search)
+         648         308 LOAD_FAST                0 (search)
                      310 LOAD_ATTR               11 (uid)
          
-         647         320 LOAD_CONST               2 (('sort', 'inclusion', 'exclusion', 'meta', 'uid'))
+         643         320 LOAD_CONST               2 (('sort', 'inclusion', 'exclusion', 'meta', 'uid'))
                      322 BUILD_CONST_KEY_MAP      5
          
-         634         324 PRECALL                  2
+         630         324 PRECALL                  2
                      328 CALL                     2
                      338 POP_TOP
          
-         655         340 LOAD_FAST                1 (conn)
+         651         340 LOAD_FAST                1 (conn)
                      342 LOAD_METHOD             12 (commit)
                      364 PRECALL                  0
                      368 CALL                     0
                      378 POP_TOP
          
-         633         380 LOAD_CONST               0 (None)
+         629         380 LOAD_CONST               0 (None)
                      382 LOAD_CONST               0 (None)
                      384 LOAD_CONST               0 (None)
                      386 PRECALL                  2
                      390 CALL                     2
                      400 POP_TOP
                      402 LOAD_CONST               0 (None)
                      404 RETURN_VALUE
@@ -3410,22 +3418,22 @@
             ('sort', 'inclusion', 'exclusion', 'meta', 'uid')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'json', 'dumps', 'sort', 'inclusion', 'exclusion', 'meta', 'uid', 'commit')
          varnames   ('search', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_search'
-         firstlineno 632
+         firstlineno 628
          lnotab 0x020134011801160102ff0e0d30013001300130010cfb04f3101528ea
       (None,)
    names      ('json', 'dataclasses', 'asdict', 'typing', 'Any', 'List', 'pandas', 'pd', 'sqlalchemy', 'dacite', 'from_dict', 'dotenv', 'load_dotenv', 'google.cloud.sql.connector', 'Connector', 'gandai', 'helpers', 'gandai.db', 'connect_with_connector', 'gandai.models', 'Actor', 'Checkpoint', 'Company', 'Event', 'EventType', 'Search', 'db', 'insert_company', 'insert_event', 'insert_actor', 'insert_search', 'insert_checkpoint', 'str', 'int', 'insert_targets_from_domains', 'insert_companies_as_targets', 'DataFrame', 'top_actor_per_search', 'search_event_count_by_type', 'search', 'actor', 'search_target_by_last_event_type', 'search_target_export', 'target_count', 'event', 'unique_domains', 'company', 'checkpoint', 'comment_by_domain', 'find_search_by_uid', 'find_company_by_domain', 'find_event_by_id', 'update_company', 'update_search')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020108010c011002080108010c010c010c0214020c010c01200214
       060c0e1015100f1013100d02010eff020102ff020102ff020102ff020202
-      fe083702010eff020102ff020102ff020202fe083716261610062a160e12
+      fe083402010eff020102ff020102ff020202fe083616261610062a160e12
       451a3b1a1e1a0c1a0c160b1a0d1a15101210101013101b
```

### Comparing `gandai-1.3.2/gandai/__pycache__/secrets.cpython-311.pyc` & `gandai-1.3.3/gandai/__pycache__/secrets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.2/gandai/__pycache__/services.cpython-311.pyc` & `gandai-1.3.3/gandai/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.2/gandai/__pycache__/sources.cpython-311.pyc` & `gandai-1.3.3/gandai/__pycache__/sources.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.2/gandai/analytics.py` & `gandai-1.3.3/gandai/analytics.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.2/gandai/auth.py` & `gandai-1.3.3/gandai/auth.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.2/gandai/datastore.py` & `gandai-1.3.3/gandai/datastore.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.2/gandai/db.py` & `gandai-1.3.3/gandai/db.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.2/gandai/main.py` & `gandai-1.3.3/gandai/main.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.2/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc` & `gandai-1.3.3/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.2/gandai/migrations/db_seed.py` & `gandai-1.3.3/gandai/migrations/db_seed.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.2/gandai/migrations/dealcloud.py` & `gandai-1.3.3/gandai/migrations/dealcloud.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.2/gandai/migrations/sql/schema.sql` & `gandai-1.3.3/gandai/migrations/sql/schema.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.3.2/gandai/models.py` & `gandai-1.3.3/gandai/models.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.2/gandai/query.py` & `gandai-1.3.3/gandai/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,33 +104,23 @@
 
 def insert_targets_from_domains(
     domains: List[str], search_uid: int, actor_key: str, last_event_type: str
 ) -> None:
     """
     Takes in domains, inserts targets into a review stage, where they will
     try to be enriched on process event
-
     """
-    existing_search_domains = unique_domains(search_uid=search_uid)[
-        "domain"
-    ].to_list()  
-    with db.connect() as con:
-        for domain in domains:
-            if "." not in domain:
-                print(f"Skipping {domain} as not a valid domain")
-                continue
-            else:
-                domain = helpers.clean_domain(domain)  # removes http, https, www, etc
+    existing_domains = set(unique_domains(search_uid=search_uid)['domain'])
+    
+    new_domains = {helpers.clean_domain(domain) for domain in domains if "." in domain}
 
-            if domain in existing_search_domains:
-                print(f"Skipping {domain} as already a target")
-                continue
-            else:
-                print(f"Adding {domain} as target")
+    domains_to_insert = list(new_domains - existing_domains)
 
+    with db.connect() as con:
+        for domain in domains_to_insert:
             # should these be in same transaction?
             con.execute(
                 sqlalchemy.text(
                     """
                     INSERT INTO company (domain) 
                     VALUES(:domain)
                     ON CONFLICT DO NOTHING
@@ -140,26 +130,33 @@
             )
 
             con.execute(
                 sqlalchemy.text(
                     """
                     INSERT INTO event (search_uid, domain, actor_key, type) 
                     VALUES(:search_uid, :domain, :actor_key, :type)
+                    ON CONFLICT DO NOTHING
                     """
                 ),
                 {
                     "search_uid": search_uid,
                     "actor_key": actor_key,
                     "domain": domain,
                     "type": last_event_type,
                 },
             )
         
         con.commit()
 
+    resp = {
+        "inserted": len(domains_to_insert),
+        "duplicates": len(new_domains.intersection(existing_domains)),
+    }
+    return resp
+
 
 def insert_companies_as_targets(
     companies: List[Any], search_uid: int, actor_key: str
 ) -> None:
     """Takes Structured Companies (e.g. from source.find_similiar()) and inserts to Review phase"""
     existing_search_domains = unique_domains(search_uid=search_uid)["domain"].to_list()
     with db.connect() as con:
@@ -201,15 +198,14 @@
                     "search_uid": search_uid,
                     "actor_key": actor_key,
                     "domain": company.get("domain"),
                     "type": "create",
                 },
             )
 
-        # con.execute(sqlalchemy.text("REFRESH MATERIALIZED VIEW target"))
         con.commit()
 
 
 ### READS ###
 
 
 def top_actor_per_search() -> pd.DataFrame:
```

### Comparing `gandai-1.3.2/gandai/secrets.py` & `gandai-1.3.3/gandai/secrets.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.2/gandai/sources.py` & `gandai-1.3.3/gandai/sources.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.2/gandai.egg-info/SOURCES.txt` & `gandai-1.3.3/gandai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

