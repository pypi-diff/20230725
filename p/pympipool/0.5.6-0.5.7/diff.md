# Comparing `tmp/pympipool-0.5.6.tar.gz` & `tmp/pympipool-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pympipool-0.5.6.tar", last modified: Fri Jul 21 22:29:49 2023, max compression
+gzip compressed data, was "pympipool-0.5.7.tar", last modified: Tue Jul 25 19:50:13 2023, max compression
```

## Comparing `pympipool-0.5.6.tar` & `pympipool-0.5.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:29:49.739897 pympipool-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-21 22:29:46.000000 pympipool-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-21 22:29:46.000000 pympipool-0.5.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-21 22:29:49.739897 pympipool-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-07-21 22:29:46.000000 pympipool-0.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:29:49.739897 pympipool-0.5.6/pympipool/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-21 22:29:46.000000 pympipool-0.5.6/pympipool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-21 22:29:49.739897 pympipool-0.5.6/pympipool/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:29:49.735897 pympipool-0.5.6/pympipool/external_interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:29:46.000000 pympipool-0.5.6/pympipool/external_interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-07-21 22:29:46.000000 pympipool-0.5.6/pympipool/external_interfaces/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-07-21 22:29:46.000000 pympipool-0.5.6/pympipool/external_interfaces/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-07-21 22:29:46.000000 pympipool-0.5.6/pympipool/external_interfaces/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-21 22:29:46.000000 pympipool-0.5.6/pympipool/external_interfaces/thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:29:49.735897 pympipool-0.5.6/pympipool/parallel_executors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:29:46.000000 pympipool-0.5.6/pympipool/parallel_executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-21 22:29:46.000000 pympipool-0.5.6/pympipool/parallel_executors/mpiexec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-21 22:29:46.000000 pympipool-0.5.6/pympipool/parallel_executors/mpipool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:29:49.739897 pympipool-0.5.6/pympipool/shared_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 22:29:46.000000 pympipool-0.5.6/pympipool/shared_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-07-21 22:29:46.000000 pympipool-0.5.6/pympipool/shared_functions/external_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-07-21 22:29:46.000000 pympipool-0.5.6/pympipool/shared_functions/parallel_executors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:29:49.735897 pympipool-0.5.6/pympipool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-21 22:29:49.000000 pympipool-0.5.6/pympipool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-21 22:29:49.000000 pympipool-0.5.6/pympipool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 22:29:49.000000 pympipool-0.5.6/pympipool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-21 22:29:49.000000 pympipool-0.5.6/pympipool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 22:29:49.000000 pympipool-0.5.6/pympipool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-21 22:29:49.739897 pympipool-0.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-21 22:29:49.000000 pympipool-0.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 22:29:49.739897 pympipool-0.5.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-21 22:29:46.000000 pympipool-0.5.6/tests/test_communicator_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-21 22:29:46.000000 pympipool-0.5.6/tests/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-21 22:29:46.000000 pympipool-0.5.6/tests/test_future.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-21 22:29:46.000000 pympipool-0.5.6/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-21 22:29:46.000000 pympipool-0.5.6/tests/test_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-21 22:29:46.000000 pympipool-0.5.6/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-21 22:29:46.000000 pympipool-0.5.6/tests/test_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-21 22:29:46.000000 pympipool-0.5.6/tests/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-21 22:29:46.000000 pympipool-0.5.6/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-21 22:29:46.000000 pympipool-0.5.6/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-21 22:29:46.000000 pympipool-0.5.6/tests/test_worker_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-21 22:29:46.000000 pympipool-0.5.6/tests/test_zmq.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-21 22:29:46.000000 pympipool-0.5.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:50:13.560990 pympipool-0.5.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-25 19:50:08.000000 pympipool-0.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-25 19:50:08.000000 pympipool-0.5.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-25 19:50:13.560990 pympipool-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-07-25 19:50:08.000000 pympipool-0.5.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:50:13.560990 pympipool-0.5.7/pympipool/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-25 19:50:08.000000 pympipool-0.5.7/pympipool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-25 19:50:13.560990 pympipool-0.5.7/pympipool/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:50:13.552990 pympipool-0.5.7/pympipool/external_interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:50:08.000000 pympipool-0.5.7/pympipool/external_interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-07-25 19:50:08.000000 pympipool-0.5.7/pympipool/external_interfaces/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-07-25 19:50:08.000000 pympipool-0.5.7/pympipool/external_interfaces/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-07-25 19:50:08.000000 pympipool-0.5.7/pympipool/external_interfaces/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-25 19:50:08.000000 pympipool-0.5.7/pympipool/external_interfaces/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:50:13.556990 pympipool-0.5.7/pympipool/parallel_executors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:50:08.000000 pympipool-0.5.7/pympipool/parallel_executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-25 19:50:08.000000 pympipool-0.5.7/pympipool/parallel_executors/mpiexec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-25 19:50:08.000000 pympipool-0.5.7/pympipool/parallel_executors/mpipool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:50:13.556990 pympipool-0.5.7/pympipool/shared_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:50:08.000000 pympipool-0.5.7/pympipool/shared_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-07-25 19:50:08.000000 pympipool-0.5.7/pympipool/shared_functions/external_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-07-25 19:50:08.000000 pympipool-0.5.7/pympipool/shared_functions/parallel_executors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:50:13.552990 pympipool-0.5.7/pympipool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-25 19:50:13.000000 pympipool-0.5.7/pympipool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-25 19:50:13.000000 pympipool-0.5.7/pympipool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:50:13.000000 pympipool-0.5.7/pympipool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-25 19:50:13.000000 pympipool-0.5.7/pympipool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 19:50:13.000000 pympipool-0.5.7/pympipool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-25 19:50:13.560990 pympipool-0.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-25 19:50:13.000000 pympipool-0.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:50:13.560990 pympipool-0.5.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-25 19:50:08.000000 pympipool-0.5.7/tests/test_communicator_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-25 19:50:08.000000 pympipool-0.5.7/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-25 19:50:08.000000 pympipool-0.5.7/tests/test_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-25 19:50:08.000000 pympipool-0.5.7/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-25 19:50:08.000000 pympipool-0.5.7/tests/test_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-25 19:50:08.000000 pympipool-0.5.7/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-25 19:50:08.000000 pympipool-0.5.7/tests/test_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-25 19:50:08.000000 pympipool-0.5.7/tests/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-25 19:50:08.000000 pympipool-0.5.7/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-25 19:50:08.000000 pympipool-0.5.7/tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-25 19:50:08.000000 pympipool-0.5.7/tests/test_worker_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-25 19:50:08.000000 pympipool-0.5.7/tests/test_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-25 19:50:08.000000 pympipool-0.5.7/versioneer.py
```

### Comparing `pympipool-0.5.6/LICENSE` & `pympipool-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.6/PKG-INFO` & `pympipool-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.5.6
+Version: 0.5.7
 Summary: pympipool - scale python functions over multiple compute nodes
 Home-page: https://github.com/jan-janssen/pympipool
 Author-email: jan.janssen@outlook.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pympipool-0.5.6/README.md` & `pympipool-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.6/pympipool/__init__.py` & `pympipool-0.5.7/pympipool/__init__.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.6/pympipool/external_interfaces/communication.py` & `pympipool-0.5.7/pympipool/external_interfaces/communication.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.6/pympipool/external_interfaces/executor.py` & `pympipool-0.5.7/pympipool/external_interfaces/executor.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.6/pympipool/external_interfaces/pool.py` & `pympipool-0.5.7/pympipool/external_interfaces/pool.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.6/pympipool/external_interfaces/thread.py` & `pympipool-0.5.7/pympipool/external_interfaces/thread.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.6/pympipool/parallel_executors/mpiexec.py` & `pympipool-0.5.7/pympipool/parallel_executors/mpiexec.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         )
     else:
         context = None
         socket = None
 
     memory = None
 
+    # required for flux interface - otherwise the current path is not included in the python path
     cwd = abspath(".")
     if cwd not in sys.path:
         sys.path.insert(1, cwd)
 
     while True:
         # Read from socket
         if mpi_rank_zero:
```

### Comparing `pympipool-0.5.6/pympipool/shared_functions/external_interfaces.py` & `pympipool-0.5.7/pympipool/shared_functions/external_interfaces.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.6/pympipool/shared_functions/parallel_executors.py` & `pympipool-0.5.7/pympipool/shared_functions/parallel_executors.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.6/pympipool.egg-info/PKG-INFO` & `pympipool-0.5.7/pympipool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.5.6
+Version: 0.5.7
 Summary: pympipool - scale python functions over multiple compute nodes
 Home-page: https://github.com/jan-janssen/pympipool
 Author-email: jan.janssen@outlook.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pympipool-0.5.6/pympipool.egg-info/SOURCES.txt` & `pympipool-0.5.7/pympipool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.6/setup.py` & `pympipool-0.5.7/setup.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.6/tests/test_communicator_split.py` & `pympipool-0.5.7/tests/test_communicator_split.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.6/tests/test_executor.py` & `pympipool-0.5.7/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.6/tests/test_future.py` & `pympipool-0.5.7/tests/test_future.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.6/tests/test_interface.py` & `pympipool-0.5.7/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.6/tests/test_multitask.py` & `pympipool-0.5.7/tests/test_multitask.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.6/tests/test_parse.py` & `pympipool-0.5.7/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.6/tests/test_pool.py` & `pympipool-0.5.7/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.6/tests/test_queue.py` & `pympipool-0.5.7/tests/test_queue.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.6/tests/test_task.py` & `pympipool-0.5.7/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.6/tests/test_worker.py` & `pympipool-0.5.7/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.6/tests/test_worker_memory.py` & `pympipool-0.5.7/tests/test_worker_memory.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.6/tests/test_zmq.py` & `pympipool-0.5.7/tests/test_zmq.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.6/versioneer.py` & `pympipool-0.5.7/versioneer.py`

 * *Files identical despite different names*

