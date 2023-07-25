# Comparing `tmp/gandai-1.3.4.tar.gz` & `tmp/gandai-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-1.3.4.tar", last modified: Tue Jul 25 20:27:03 2023, max compression
+gzip compressed data, was "gandai-1.3.5.tar", last modified: Tue Jul 25 20:42:44 2023, max compression
```

## Comparing `gandai-1.3.4.tar` & `gandai-1.3.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 20:27:03.395431 gandai-1.3.4/
--rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.3.4/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      214 2023-07-25 20:27:03.395296 gandai-1.3.4/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 20:27:03.388033 gandai-1.3.4/gandai/
--rw-r--r--   0 parker     (501) staff       (20)       46 2023-07-17 18:25:43.000000 gandai-1.3.4/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 20:27:03.393095 gandai-1.3.4/gandai/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      264 2023-07-17 18:43:09.000000 gandai-1.3.4/gandai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.3.4/gandai/__pycache__/adapters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4120 2023-07-25 17:01:01.000000 gandai-1.3.4/gandai/__pycache__/analytics.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-19 22:26:35.000000 gandai-1.3.4/gandai/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.3.4/gandai/__pycache__/datastore.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2014 2023-07-17 18:43:09.000000 gandai-1.3.4/gandai/__pycache__/db.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3757 2023-07-25 19:02:34.000000 gandai-1.3.4/gandai/__pycache__/gpt.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5979 2023-05-05 21:52:33.000000 gandai-1.3.4/gandai/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1373 2023-07-23 18:54:58.000000 gandai-1.3.4/gandai/__pycache__/helpers.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4285 2023-07-25 16:56:41.000000 gandai-1.3.4/gandai/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6151 2023-07-17 18:43:10.000000 gandai-1.3.4/gandai/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    31858 2023-07-25 20:16:58.000000 gandai-1.3.4/gandai/__pycache__/query.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2221 2023-07-17 18:43:09.000000 gandai-1.3.4/gandai/__pycache__/secrets.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.3.4/gandai/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    15985 2023-07-23 23:17:10.000000 gandai-1.3.4/gandai/__pycache__/sources.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2368 2023-07-25 17:01:00.000000 gandai-1.3.4/gandai/analytics.py
--rw-r--r--   0 parker     (501) staff       (20)     1759 2023-07-25 20:25:00.000000 gandai-1.3.4/gandai/auth.py
--rw-r--r--   0 parker     (501) staff       (20)     1200 2023-07-17 18:25:43.000000 gandai-1.3.4/gandai/db.py
--rw-r--r--   0 parker     (501) staff       (20)     1631 2023-07-25 19:02:05.000000 gandai-1.3.4/gandai/gpt.py
--rw-r--r--   0 parker     (501) staff       (20)      402 2023-07-23 18:54:56.000000 gandai-1.3.4/gandai/helpers.py
--rw-r--r--   0 parker     (501) staff       (20)     3030 2023-07-23 20:20:45.000000 gandai-1.3.4/gandai/main.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 20:27:03.394025 gandai-1.3.4/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.3.4/gandai/migrations/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 20:27:03.394519 gandai-1.3.4/gandai/migrations/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.3.4/gandai/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.3.4/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.3.4/gandai/migrations/db_create.py
--rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.3.4/gandai/migrations/db_seed.py
--rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.3.4/gandai/migrations/dealcloud.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 20:27:03.395079 gandai-1.3.4/gandai/migrations/sql/
--rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.3.4/gandai/migrations/sql/2305023-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     3061 2023-07-17 18:25:43.000000 gandai-1.3.4/gandai/migrations/sql/schema.sql
--rw-r--r--   0 parker     (501) staff       (20)     2683 2023-07-17 18:25:43.000000 gandai-1.3.4/gandai/models.py
--rw-r--r--   0 parker     (501) staff       (20)    20866 2023-07-25 20:16:56.000000 gandai-1.3.4/gandai/query.py
--rw-r--r--   0 parker     (501) staff       (20)     1075 2023-07-25 20:26:21.000000 gandai-1.3.4/gandai/secrets.py
--rw-r--r--   0 parker     (501) staff       (20)    10783 2023-07-23 23:17:02.000000 gandai-1.3.4/gandai/sources.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 20:27:03.388638 gandai-1.3.4/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      214 2023-07-25 20:27:03.000000 gandai-1.3.4/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     1275 2023-07-25 20:27:03.000000 gandai-1.3.4/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2023-07-25 20:27:03.000000 gandai-1.3.4/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2023-07-25 20:27:03.000000 gandai-1.3.4/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      383 2023-07-25 20:26:54.000000 gandai-1.3.4/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2023-07-25 20:27:03.395472 gandai-1.3.4/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.3.4/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 20:42:44.405139 gandai-1.3.5/
+-rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.3.5/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      214 2023-07-25 20:42:44.404998 gandai-1.3.5/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 20:42:44.397438 gandai-1.3.5/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)       46 2023-07-17 18:25:43.000000 gandai-1.3.5/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 20:42:44.402803 gandai-1.3.5/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      264 2023-07-17 18:43:09.000000 gandai-1.3.5/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.3.5/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4120 2023-07-25 17:01:01.000000 gandai-1.3.5/gandai/__pycache__/analytics.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-19 22:26:35.000000 gandai-1.3.5/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.3.5/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2014 2023-07-17 18:43:09.000000 gandai-1.3.5/gandai/__pycache__/db.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3757 2023-07-25 19:02:34.000000 gandai-1.3.5/gandai/__pycache__/gpt.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5979 2023-05-05 21:52:33.000000 gandai-1.3.5/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1373 2023-07-23 18:54:58.000000 gandai-1.3.5/gandai/__pycache__/helpers.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4285 2023-07-25 16:56:41.000000 gandai-1.3.5/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6151 2023-07-17 18:43:10.000000 gandai-1.3.5/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    31858 2023-07-25 20:16:58.000000 gandai-1.3.5/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2221 2023-07-17 18:43:09.000000 gandai-1.3.5/gandai/__pycache__/secrets.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.3.5/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    15985 2023-07-23 23:17:10.000000 gandai-1.3.5/gandai/__pycache__/sources.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2368 2023-07-25 17:01:00.000000 gandai-1.3.5/gandai/analytics.py
+-rw-r--r--   0 parker     (501) staff       (20)     1759 2023-07-25 20:25:00.000000 gandai-1.3.5/gandai/auth.py
+-rw-r--r--   0 parker     (501) staff       (20)     1200 2023-07-17 18:25:43.000000 gandai-1.3.5/gandai/db.py
+-rw-r--r--   0 parker     (501) staff       (20)     1631 2023-07-25 19:02:05.000000 gandai-1.3.5/gandai/gpt.py
+-rw-r--r--   0 parker     (501) staff       (20)      402 2023-07-23 18:54:56.000000 gandai-1.3.5/gandai/helpers.py
+-rw-r--r--   0 parker     (501) staff       (20)     3030 2023-07-23 20:20:45.000000 gandai-1.3.5/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 20:42:44.403641 gandai-1.3.5/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.3.5/gandai/migrations/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 20:42:44.404151 gandai-1.3.5/gandai/migrations/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.3.5/gandai/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.3.5/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.3.5/gandai/migrations/db_create.py
+-rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.3.5/gandai/migrations/db_seed.py
+-rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.3.5/gandai/migrations/dealcloud.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 20:42:44.404772 gandai-1.3.5/gandai/migrations/sql/
+-rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.3.5/gandai/migrations/sql/2305023-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     3061 2023-07-17 18:25:43.000000 gandai-1.3.5/gandai/migrations/sql/schema.sql
+-rw-r--r--   0 parker     (501) staff       (20)     2683 2023-07-17 18:25:43.000000 gandai-1.3.5/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)    20866 2023-07-25 20:16:56.000000 gandai-1.3.5/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)     1069 2023-07-25 20:41:48.000000 gandai-1.3.5/gandai/secrets.py
+-rw-r--r--   0 parker     (501) staff       (20)    10783 2023-07-23 23:17:02.000000 gandai-1.3.5/gandai/sources.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 20:42:44.398217 gandai-1.3.5/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      214 2023-07-25 20:42:44.000000 gandai-1.3.5/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1275 2023-07-25 20:42:44.000000 gandai-1.3.5/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2023-07-25 20:42:44.000000 gandai-1.3.5/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2023-07-25 20:42:44.000000 gandai-1.3.5/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      383 2023-07-25 20:42:13.000000 gandai-1.3.5/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2023-07-25 20:42:44.405170 gandai-1.3.5/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.3.5/setup.py
```

### Comparing `gandai-1.3.4/gandai/__pycache__/adapters.cpython-311.pyc` & `gandai-1.3.5/gandai/__pycache__/adapters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.4/gandai/__pycache__/analytics.cpython-311.pyc` & `gandai-1.3.5/gandai/__pycache__/analytics.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.4/gandai/__pycache__/auth.cpython-311.pyc` & `gandai-1.3.5/gandai/__pycache__/auth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.4/gandai/__pycache__/datastore.cpython-311.pyc` & `gandai-1.3.5/gandai/__pycache__/datastore.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.4/gandai/__pycache__/db.cpython-311.pyc` & `gandai-1.3.5/gandai/__pycache__/db.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.4/gandai/__pycache__/gpt.cpython-311.pyc` & `gandai-1.3.5/gandai/__pycache__/gpt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.4/gandai/__pycache__/grata.cpython-311.pyc` & `gandai-1.3.5/gandai/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.4/gandai/__pycache__/helpers.cpython-311.pyc` & `gandai-1.3.5/gandai/__pycache__/helpers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.4/gandai/__pycache__/main.cpython-311.pyc` & `gandai-1.3.5/gandai/__pycache__/main.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.4/gandai/__pycache__/models.cpython-311.pyc` & `gandai-1.3.5/gandai/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.4/gandai/__pycache__/query.cpython-311.pyc` & `gandai-1.3.5/gandai/__pycache__/query.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.4/gandai/__pycache__/secrets.cpython-311.pyc` & `gandai-1.3.5/gandai/__pycache__/secrets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.4/gandai/__pycache__/services.cpython-311.pyc` & `gandai-1.3.5/gandai/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.4/gandai/__pycache__/sources.cpython-311.pyc` & `gandai-1.3.5/gandai/__pycache__/sources.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.4/gandai/analytics.py` & `gandai-1.3.5/gandai/analytics.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.4/gandai/auth.py` & `gandai-1.3.5/gandai/auth.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.4/gandai/db.py` & `gandai-1.3.5/gandai/db.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.4/gandai/gpt.py` & `gandai-1.3.5/gandai/gpt.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.4/gandai/main.py` & `gandai-1.3.5/gandai/main.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.4/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc` & `gandai-1.3.5/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.4/gandai/migrations/db_seed.py` & `gandai-1.3.5/gandai/migrations/db_seed.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.4/gandai/migrations/dealcloud.py` & `gandai-1.3.5/gandai/migrations/dealcloud.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.4/gandai/migrations/sql/schema.sql` & `gandai-1.3.5/gandai/migrations/sql/schema.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.3.4/gandai/models.py` & `gandai-1.3.5/gandai/models.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.4/gandai/query.py` & `gandai-1.3.5/gandai/query.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.4/gandai/secrets.py` & `gandai-1.3.5/gandai/secrets.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import os
 
 from dotenv import load_dotenv
 from google.cloud import secretmanager
 
 load_dotenv()
 
-GCP_PROJECT = os.getenv("GCP_PROJECT")
-print(GCP_PROJECT)
+PROJECT_ID = os.getenv("PROJECT_ID")
+print(PROJECT_ID)
 
 client = secretmanager.SecretManagerServiceClient()
 
 
 def create_secret(secret_id) -> None:
     try:
         client.create_secret(
             request={
-                "parent": f"projects/{GCP_PROJECT}",
+                "parent": f"projects/{PROJECT_ID}",
                 "secret_id": secret_id,
                 "secret": {"replication": {"automatic": {}}},
             }
         )
     except Exception as e:
         print(e)
 
 
 def add_secret_version(secret_id, payload) -> None:
-    parent = client.secret_path(GCP_PROJECT, secret_id)
+    parent = client.secret_path(PROJECT_ID, secret_id)
     response = client.add_secret_version(
         request={"parent": parent, "payload": {"data": payload.encode("UTF-8")}}
     )
     print("Added secret version: {}".format(response.name))
 
 
 def access_secret_version(secret_id, version_id="latest"):
-    name = f"projects/{GCP_PROJECT}/secrets/{secret_id}/versions/{version_id}"
+    name = f"projects/{PROJECT_ID}/secrets/{secret_id}/versions/{version_id}"
     response = client.access_secret_version(name=name)
     return response.payload.data.decode("UTF-8")
```

### Comparing `gandai-1.3.4/gandai/sources.py` & `gandai-1.3.5/gandai/sources.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.4/gandai.egg-info/SOURCES.txt` & `gandai-1.3.5/gandai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

