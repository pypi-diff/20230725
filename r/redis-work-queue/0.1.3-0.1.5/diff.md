# Comparing `tmp/redis-work-queue-0.1.3.tar.gz` & `tmp/redis-work-queue-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis-work-queue-0.1.3.tar", last modified: Sun Apr 23 09:43:51 2023, max compression
+gzip compressed data, was "redis-work-queue-0.1.5.tar", last modified: Tue Jul 25 15:25:15 2023, max compression
```

## Comparing `redis-work-queue-0.1.3.tar` & `redis-work-queue-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jp        (1000) jp        (1000)        0 2023-04-23 09:43:51.743501 redis-work-queue-0.1.3/
--rw-r--r--   0 jp        (1000) jp        (1000)     1061 2023-04-22 10:26:00.000000 redis-work-queue-0.1.3/LICENSE
--rw-r--r--   0 jp        (1000) jp        (1000)     4118 2023-04-23 09:43:51.743501 redis-work-queue-0.1.3/PKG-INFO
--rw-r--r--   0 jp        (1000) jp        (1000)     2567 2023-04-23 09:43:40.000000 redis-work-queue-0.1.3/README.md
--rw-r--r--   0 jp        (1000) jp        (1000)      558 2023-04-23 09:43:36.000000 redis-work-queue-0.1.3/pyproject.toml
-drwxr-xr-x   0 jp        (1000) jp        (1000)        0 2023-04-23 09:43:51.743501 redis-work-queue-0.1.3/redis_work_queue/
--rw-r--r--   0 jp        (1000) jp        (1000)       89 2023-04-22 11:48:01.000000 redis-work-queue-0.1.3/redis_work_queue/__init__.py
--rw-r--r--   0 jp        (1000) jp        (1000)     1788 2023-04-23 09:22:24.000000 redis-work-queue-0.1.3/redis_work_queue/item.py
--rw-r--r--   0 jp        (1000) jp        (1000)      766 2023-04-23 09:15:05.000000 redis-work-queue-0.1.3/redis_work_queue/keyprefix.py
--rw-r--r--   0 jp        (1000) jp        (1000)     6976 2023-04-22 11:42:51.000000 redis-work-queue-0.1.3/redis_work_queue/workqueue.py
-drwxr-xr-x   0 jp        (1000) jp        (1000)        0 2023-04-23 09:43:51.743501 redis-work-queue-0.1.3/redis_work_queue.egg-info/
--rw-r--r--   0 jp        (1000) jp        (1000)     4118 2023-04-23 09:43:51.000000 redis-work-queue-0.1.3/redis_work_queue.egg-info/PKG-INFO
--rw-r--r--   0 jp        (1000) jp        (1000)      345 2023-04-23 09:43:51.000000 redis-work-queue-0.1.3/redis_work_queue.egg-info/SOURCES.txt
--rw-r--r--   0 jp        (1000) jp        (1000)        1 2023-04-23 09:43:51.000000 redis-work-queue-0.1.3/redis_work_queue.egg-info/dependency_links.txt
--rw-r--r--   0 jp        (1000) jp        (1000)       11 2023-04-23 09:43:51.000000 redis-work-queue-0.1.3/redis_work_queue.egg-info/requires.txt
--rw-r--r--   0 jp        (1000) jp        (1000)       17 2023-04-23 09:43:51.000000 redis-work-queue-0.1.3/redis_work_queue.egg-info/top_level.txt
--rw-r--r--   0 jp        (1000) jp        (1000)       38 2023-04-23 09:43:51.743501 redis-work-queue-0.1.3/setup.cfg
+drwxr-xr-x   0 jp        (1000) jp        (1000)        0 2023-07-25 15:25:15.676604 redis-work-queue-0.1.5/
+-rw-r--r--   0 jp        (1000) jp        (1000)     1061 2023-04-22 10:26:00.000000 redis-work-queue-0.1.5/LICENSE
+-rw-r--r--   0 jp        (1000) jp        (1000)     4180 2023-07-25 15:25:15.676604 redis-work-queue-0.1.5/PKG-INFO
+-rw-r--r--   0 jp        (1000) jp        (1000)     2598 2023-07-25 15:20:36.000000 redis-work-queue-0.1.5/README.md
+-rw-r--r--   0 jp        (1000) jp        (1000)      589 2023-07-25 15:20:36.000000 redis-work-queue-0.1.5/pyproject.toml
+drwxr-xr-x   0 jp        (1000) jp        (1000)        0 2023-07-25 15:25:15.676604 redis-work-queue-0.1.5/redis_work_queue/
+-rw-r--r--   0 jp        (1000) jp        (1000)       89 2023-04-22 11:48:01.000000 redis-work-queue-0.1.5/redis_work_queue/__init__.py
+-rw-r--r--   0 jp        (1000) jp        (1000)     1788 2023-04-23 09:22:24.000000 redis-work-queue-0.1.5/redis_work_queue/item.py
+-rw-r--r--   0 jp        (1000) jp        (1000)      766 2023-04-23 09:15:05.000000 redis-work-queue-0.1.5/redis_work_queue/keyprefix.py
+-rw-r--r--   0 jp        (1000) jp        (1000)     6976 2023-04-22 11:42:51.000000 redis-work-queue-0.1.5/redis_work_queue/workqueue.py
+drwxr-xr-x   0 jp        (1000) jp        (1000)        0 2023-07-25 15:25:15.676604 redis-work-queue-0.1.5/redis_work_queue.egg-info/
+-rw-r--r--   0 jp        (1000) jp        (1000)     4180 2023-07-25 15:25:15.000000 redis-work-queue-0.1.5/redis_work_queue.egg-info/PKG-INFO
+-rw-r--r--   0 jp        (1000) jp        (1000)      345 2023-07-25 15:25:15.000000 redis-work-queue-0.1.5/redis_work_queue.egg-info/SOURCES.txt
+-rw-r--r--   0 jp        (1000) jp        (1000)        1 2023-07-25 15:25:15.000000 redis-work-queue-0.1.5/redis_work_queue.egg-info/dependency_links.txt
+-rw-r--r--   0 jp        (1000) jp        (1000)       11 2023-07-25 15:25:15.000000 redis-work-queue-0.1.5/redis_work_queue.egg-info/requires.txt
+-rw-r--r--   0 jp        (1000) jp        (1000)       17 2023-07-25 15:25:15.000000 redis-work-queue-0.1.5/redis_work_queue.egg-info/top_level.txt
+-rw-r--r--   0 jp        (1000) jp        (1000)       38 2023-07-25 15:25:15.676604 redis-work-queue-0.1.5/setup.cfg
```

### Comparing `redis-work-queue-0.1.3/LICENSE` & `redis-work-queue-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `redis-work-queue-0.1.3/PKG-INFO` & `redis-work-queue-0.1.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: redis-work-queue
-Version: 0.1.3
-Summary: A work queue, on top of a redis database, with implementations in Python, Rust, Go and C#.
+Version: 0.1.5
+Summary: A work queue, on top of a redis database, with implementations in Python, Rust, Go, Node.js (TypeScript) and Dotnet (C#).
 Author-email: Jacob O'Toole <jacob.otoole@mevitae.com>
 License: Copyright 2023 Jacob O'Toole
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
@@ -13,15 +13,16 @@
         
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-A work queue, on top of a redis database, with implementations in Python, Rust, Go and C#.
+A work queue, on top of a redis database, with implementations in Python, Rust, Go, Node.js
+(TypeScript) and Dotnet (C#).
 
 This is the Python implementations. For an overview of how the work queue works, it's limitations,
 and the general concepts and implementations in other languages, please read the [redis-work-queue
 readme](https://github.com/MeVitae/redis-work-queue/blob/main/README.md).
 
 ## Setup
```

### Comparing `redis-work-queue-0.1.3/README.md` & `redis-work-queue-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-A work queue, on top of a redis database, with implementations in Python, Rust, Go and C#.
+A work queue, on top of a redis database, with implementations in Python, Rust, Go, Node.js
+(TypeScript) and Dotnet (C#).
 
 This is the Python implementations. For an overview of how the work queue works, it's limitations,
 and the general concepts and implementations in other languages, please read the [redis-work-queue
 readme](https://github.com/MeVitae/redis-work-queue/blob/main/README.md).
 
 ## Setup
```

### Comparing `redis-work-queue-0.1.3/pyproject.toml` & `redis-work-queue-0.1.5/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "redis-work-queue"
-version = "0.1.3"
-description = "A work queue, on top of a redis database, with implementations in Python, Rust, Go and C#."
+version = "0.1.5"
+description = "A work queue, on top of a redis database, with implementations in Python, Rust, Go, Node.js (TypeScript) and Dotnet (C#)."
 dependencies = ["redis", "uuid"]
 authors = [
     { name = "Jacob O'Toole", email = "jacob.otoole@mevitae.com" }
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 classifiers = [
```

### Comparing `redis-work-queue-0.1.3/redis_work_queue/item.py` & `redis-work-queue-0.1.5/redis_work_queue/item.py`

 * *Files identical despite different names*

### Comparing `redis-work-queue-0.1.3/redis_work_queue/keyprefix.py` & `redis-work-queue-0.1.5/redis_work_queue/keyprefix.py`

 * *Files identical despite different names*

### Comparing `redis-work-queue-0.1.3/redis_work_queue/workqueue.py` & `redis-work-queue-0.1.5/redis_work_queue/workqueue.py`

 * *Files identical despite different names*

### Comparing `redis-work-queue-0.1.3/redis_work_queue.egg-info/PKG-INFO` & `redis-work-queue-0.1.5/redis_work_queue.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: redis-work-queue
-Version: 0.1.3
-Summary: A work queue, on top of a redis database, with implementations in Python, Rust, Go and C#.
+Version: 0.1.5
+Summary: A work queue, on top of a redis database, with implementations in Python, Rust, Go, Node.js (TypeScript) and Dotnet (C#).
 Author-email: Jacob O'Toole <jacob.otoole@mevitae.com>
 License: Copyright 2023 Jacob O'Toole
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
@@ -13,15 +13,16 @@
         
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-A work queue, on top of a redis database, with implementations in Python, Rust, Go and C#.
+A work queue, on top of a redis database, with implementations in Python, Rust, Go, Node.js
+(TypeScript) and Dotnet (C#).
 
 This is the Python implementations. For an overview of how the work queue works, it's limitations,
 and the general concepts and implementations in other languages, please read the [redis-work-queue
 readme](https://github.com/MeVitae/redis-work-queue/blob/main/README.md).
 
 ## Setup
```

