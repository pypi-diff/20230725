# Comparing `tmp/mousse-0.1.8.tar.gz` & `tmp/mousse-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mousse-0.1.8.tar", last modified: Wed Jun  1 15:20:32 2022, max compression
+gzip compressed data, was "mousse-0.1.9.tar", last modified: Fri Jun  3 02:27:07 2022, max compression
```

## Comparing `mousse-0.1.8.tar` & `mousse-0.1.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2022-06-01 15:20:32.127472 mousse-0.1.8/
--rw-r--r--   0 datnh      (501) staff       (20)     8568 2022-06-01 15:20:32.127222 mousse-0.1.8/PKG-INFO
--rw-r--r--   0 datnh      (501) staff       (20)     8051 2022-05-18 05:34:54.000000 mousse-0.1.8/README.md
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2022-06-01 15:20:32.117927 mousse-0.1.8/mousse/
--rw-r--r--   0 datnh      (501) staff       (20)     1211 2022-05-09 13:22:12.000000 mousse-0.1.8/mousse/__init__.py
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2022-06-01 15:20:32.119899 mousse-0.1.8/mousse/cache/
--rw-r--r--   0 datnh      (501) staff       (20)       75 2022-05-08 16:40:38.000000 mousse-0.1.8/mousse/cache/__init__.py
--rw-r--r--   0 datnh      (501) staff       (20)     4031 2022-05-08 16:40:38.000000 mousse-0.1.8/mousse/cache/cache.py
--rw-r--r--   0 datnh      (501) staff       (20)      432 2022-05-08 16:40:38.000000 mousse-0.1.8/mousse/cache/policies.py
--rw-r--r--   0 datnh      (501) staff       (20)      685 2022-05-08 16:40:38.000000 mousse-0.1.8/mousse/cache/types.py
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2022-06-01 15:20:32.120405 mousse-0.1.8/mousse/config/
--rw-r--r--   0 datnh      (501) staff       (20)       22 2022-05-08 19:43:07.000000 mousse-0.1.8/mousse/config/__init__.py
--rw-r--r--   0 datnh      (501) staff       (20)     6559 2022-05-09 13:22:08.000000 mousse-0.1.8/mousse/config/config.py
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2022-06-01 15:20:32.122182 mousse-0.1.8/mousse/data/
--rw-r--r--   0 datnh      (501) staff       (20)      117 2022-05-08 15:01:07.000000 mousse-0.1.8/mousse/data/__init__.py
--rw-r--r--   0 datnh      (501) staff       (20)     1046 2022-05-09 12:48:27.000000 mousse-0.1.8/mousse/data/accessor.py
--rw-r--r--   0 datnh      (501) staff       (20)     4752 2022-06-01 15:18:00.000000 mousse-0.1.8/mousse/data/dataclass.py
--rw-r--r--   0 datnh      (501) staff       (20)      495 2022-05-09 12:48:27.000000 mousse-0.1.8/mousse/data/field.py
--rw-r--r--   0 datnh      (501) staff       (20)     6123 2022-05-18 08:15:26.000000 mousse-0.1.8/mousse/data/parser.py
--rw-r--r--   0 datnh      (501) staff       (20)      555 2022-05-09 12:48:27.000000 mousse-0.1.8/mousse/data/types.py
--rw-r--r--   0 datnh      (501) staff       (20)     3642 2022-05-09 12:48:27.000000 mousse-0.1.8/mousse/data/validator.py
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2022-06-01 15:20:32.122764 mousse-0.1.8/mousse/export/
--rw-r--r--   0 datnh      (501) staff       (20)       24 2022-05-08 16:40:16.000000 mousse-0.1.8/mousse/export/__init__.py
--rw-r--r--   0 datnh      (501) staff       (20)     3045 2022-05-08 16:40:16.000000 mousse-0.1.8/mousse/export/exporter.py
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2022-06-01 15:20:32.123318 mousse-0.1.8/mousse/functional/
--rw-r--r--   0 datnh      (501) staff       (20)       85 2022-05-08 16:36:55.000000 mousse-0.1.8/mousse/functional/__init__.py
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2022-06-01 15:20:32.124077 mousse-0.1.8/mousse/functional/pattern/
--rw-r--r--   0 datnh      (501) staff       (20)      357 2022-05-08 16:36:55.000000 mousse-0.1.8/mousse/functional/pattern/__init__.py
--rw-r--r--   0 datnh      (501) staff       (20)    11918 2022-05-08 16:36:55.000000 mousse-0.1.8/mousse/functional/pattern/pattern.py
--rw-r--r--   0 datnh      (501) staff       (20)      390 2022-05-08 16:36:55.000000 mousse-0.1.8/mousse/functional/pattern/types.py
--rw-r--r--   0 datnh      (501) staff       (20)     3440 2022-05-08 16:36:55.000000 mousse-0.1.8/mousse/functional/plugin.py
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2022-06-01 15:20:32.124451 mousse-0.1.8/mousse/functional/tools/
--rw-r--r--   0 datnh      (501) staff       (20)       26 2022-05-08 16:36:55.000000 mousse-0.1.8/mousse/functional/tools/__init__.py
--rw-r--r--   0 datnh      (501) staff       (20)     4688 2022-05-08 16:37:44.000000 mousse-0.1.8/mousse/functional/tools/functional.py
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2022-06-01 15:20:32.125004 mousse-0.1.8/mousse/logger/
--rw-r--r--   0 datnh      (501) staff       (20)       22 2022-05-07 09:38:11.000000 mousse-0.1.8/mousse/logger/__init__.py
--rw-r--r--   0 datnh      (501) staff       (20)     5290 2022-05-18 05:34:54.000000 mousse-0.1.8/mousse/logger/logger.py
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2022-06-01 15:20:32.126111 mousse-0.1.8/mousse/pattern/
--rw-r--r--   0 datnh      (501) staff       (20)      100 2022-05-08 03:00:34.000000 mousse-0.1.8/mousse/pattern/__init__.py
--rw-r--r--   0 datnh      (501) staff       (20)     1509 2022-05-09 12:48:27.000000 mousse-0.1.8/mousse/pattern/mediator.py
--rw-r--r--   0 datnh      (501) staff       (20)     2306 2022-05-07 09:25:57.000000 mousse-0.1.8/mousse/pattern/object_pool.py
--rw-r--r--   0 datnh      (501) staff       (20)     2794 2022-05-20 02:52:14.000000 mousse-0.1.8/mousse/pattern/registry.py
--rw-r--r--   0 datnh      (501) staff       (20)     1426 2022-05-07 09:26:12.000000 mousse-0.1.8/mousse/pattern/singleton.py
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2022-06-01 15:20:32.126971 mousse-0.1.8/mousse/scheduler/
--rw-r--r--   0 datnh      (501) staff       (20)       25 2022-05-09 12:48:27.000000 mousse-0.1.8/mousse/scheduler/__init__.py
--rw-r--r--   0 datnh      (501) staff       (20)     4419 2022-05-18 05:34:54.000000 mousse-0.1.8/mousse/scheduler/scheduler.py
--rw-r--r--   0 datnh      (501) staff       (20)     9082 2022-05-18 05:34:54.000000 mousse-0.1.8/mousse/scheduler/time.py
--rw-r--r--   0 datnh      (501) staff       (20)      623 2022-05-18 05:34:54.000000 mousse-0.1.8/mousse/scheduler/types.py
-drwxr-xr-x   0 datnh      (501) staff       (20)        0 2022-06-01 15:20:32.118950 mousse-0.1.8/mousse.egg-info/
--rw-r--r--   0 datnh      (501) staff       (20)     8568 2022-06-01 15:20:31.000000 mousse-0.1.8/mousse.egg-info/PKG-INFO
--rw-r--r--   0 datnh      (501) staff       (20)     1085 2022-06-01 15:20:32.000000 mousse-0.1.8/mousse.egg-info/SOURCES.txt
--rw-r--r--   0 datnh      (501) staff       (20)        1 2022-06-01 15:20:31.000000 mousse-0.1.8/mousse.egg-info/dependency_links.txt
--rw-r--r--   0 datnh      (501) staff       (20)       50 2022-06-01 15:20:32.000000 mousse-0.1.8/mousse.egg-info/requires.txt
--rw-r--r--   0 datnh      (501) staff       (20)        7 2022-06-01 15:20:32.000000 mousse-0.1.8/mousse.egg-info/top_level.txt
--rw-r--r--   0 datnh      (501) staff       (20)       38 2022-06-01 15:20:32.127524 mousse-0.1.8/setup.cfg
--rw-r--r--   0 datnh      (501) staff       (20)     1221 2022-06-01 15:20:25.000000 mousse-0.1.8/setup.py
+drwxr-xr-x   0 VAI-DatNH21-L  (1000) dell      (1000)        0 2022-06-03 02:27:07.394775 mousse-0.1.9/
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)     8568 2022-06-03 02:27:07.394775 mousse-0.1.9/PKG-INFO
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)     8051 2022-05-10 06:50:06.000000 mousse-0.1.9/README.md
+drwxr-xr-x   0 VAI-DatNH21-L  (1000) dell      (1000)        0 2022-06-03 02:27:07.390776 mousse-0.1.9/mousse/
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)     1211 2022-05-10 02:01:51.000000 mousse-0.1.9/mousse/__init__.py
+drwxr-xr-x   0 VAI-DatNH21-L  (1000) dell      (1000)        0 2022-06-03 02:27:07.390776 mousse-0.1.9/mousse/cache/
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)       75 2022-05-09 03:06:56.000000 mousse-0.1.9/mousse/cache/__init__.py
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)     4031 2022-05-09 07:37:30.000000 mousse-0.1.9/mousse/cache/cache.py
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)      432 2022-05-09 07:37:34.000000 mousse-0.1.9/mousse/cache/policies.py
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)      685 2022-05-09 07:37:43.000000 mousse-0.1.9/mousse/cache/types.py
+drwxr-xr-x   0 VAI-DatNH21-L  (1000) dell      (1000)        0 2022-06-03 02:27:07.390776 mousse-0.1.9/mousse/config/
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)       22 2022-05-09 03:06:56.000000 mousse-0.1.9/mousse/config/__init__.py
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)     6559 2022-05-10 02:01:51.000000 mousse-0.1.9/mousse/config/config.py
+drwxr-xr-x   0 VAI-DatNH21-L  (1000) dell      (1000)        0 2022-06-03 02:27:07.390776 mousse-0.1.9/mousse/data/
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)      117 2022-05-09 03:06:56.000000 mousse-0.1.9/mousse/data/__init__.py
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)     1046 2022-05-09 03:20:34.000000 mousse-0.1.9/mousse/data/accessor.py
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)     4738 2022-06-03 02:09:09.000000 mousse-0.1.9/mousse/data/dataclass.py
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)      495 2022-05-09 03:20:48.000000 mousse-0.1.9/mousse/data/field.py
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)     6115 2022-06-03 02:09:09.000000 mousse-0.1.9/mousse/data/parser.py
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)      555 2022-05-09 03:48:20.000000 mousse-0.1.9/mousse/data/types.py
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)     3642 2022-05-09 09:45:27.000000 mousse-0.1.9/mousse/data/validator.py
+drwxr-xr-x   0 VAI-DatNH21-L  (1000) dell      (1000)        0 2022-06-03 02:27:07.390776 mousse-0.1.9/mousse/export/
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)       24 2022-05-09 03:06:56.000000 mousse-0.1.9/mousse/export/__init__.py
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)     3045 2022-05-09 07:37:58.000000 mousse-0.1.9/mousse/export/exporter.py
+drwxr-xr-x   0 VAI-DatNH21-L  (1000) dell      (1000)        0 2022-06-03 02:27:07.390776 mousse-0.1.9/mousse/functional/
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)       85 2022-05-09 03:06:56.000000 mousse-0.1.9/mousse/functional/__init__.py
+drwxr-xr-x   0 VAI-DatNH21-L  (1000) dell      (1000)        0 2022-06-03 02:27:07.394775 mousse-0.1.9/mousse/functional/pattern/
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)      357 2022-05-09 03:06:56.000000 mousse-0.1.9/mousse/functional/pattern/__init__.py
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)    11918 2022-05-09 03:06:56.000000 mousse-0.1.9/mousse/functional/pattern/pattern.py
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)      390 2022-05-09 03:06:56.000000 mousse-0.1.9/mousse/functional/pattern/types.py
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)     3440 2022-05-09 03:06:56.000000 mousse-0.1.9/mousse/functional/plugin.py
+drwxr-xr-x   0 VAI-DatNH21-L  (1000) dell      (1000)        0 2022-06-03 02:27:07.394775 mousse-0.1.9/mousse/functional/tools/
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)       26 2022-05-09 03:06:56.000000 mousse-0.1.9/mousse/functional/tools/__init__.py
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)     4688 2022-05-09 03:46:19.000000 mousse-0.1.9/mousse/functional/tools/functional.py
+drwxr-xr-x   0 VAI-DatNH21-L  (1000) dell      (1000)        0 2022-06-03 02:27:07.394775 mousse-0.1.9/mousse/logger/
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)       22 2022-05-09 03:06:56.000000 mousse-0.1.9/mousse/logger/__init__.py
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)     6237 2022-06-03 02:25:05.000000 mousse-0.1.9/mousse/logger/logger.py
+drwxr-xr-x   0 VAI-DatNH21-L  (1000) dell      (1000)        0 2022-06-03 02:27:07.394775 mousse-0.1.9/mousse/pattern/
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)      100 2022-05-09 03:06:56.000000 mousse-0.1.9/mousse/pattern/__init__.py
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)     1509 2022-05-09 08:07:05.000000 mousse-0.1.9/mousse/pattern/mediator.py
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)     2306 2022-05-09 03:06:56.000000 mousse-0.1.9/mousse/pattern/object_pool.py
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)     2795 2022-06-03 02:09:09.000000 mousse-0.1.9/mousse/pattern/registry.py
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)     1426 2022-05-09 03:06:56.000000 mousse-0.1.9/mousse/pattern/singleton.py
+drwxr-xr-x   0 VAI-DatNH21-L  (1000) dell      (1000)        0 2022-06-03 02:27:07.394775 mousse-0.1.9/mousse/scheduler/
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)       25 2022-05-09 03:47:04.000000 mousse-0.1.9/mousse/scheduler/__init__.py
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)     4419 2022-05-10 04:30:44.000000 mousse-0.1.9/mousse/scheduler/scheduler.py
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)     9082 2022-05-10 04:52:08.000000 mousse-0.1.9/mousse/scheduler/time.py
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)      623 2022-05-10 04:30:44.000000 mousse-0.1.9/mousse/scheduler/types.py
+drwxr-xr-x   0 VAI-DatNH21-L  (1000) dell      (1000)        0 2022-06-03 02:27:07.390776 mousse-0.1.9/mousse.egg-info/
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)     8568 2022-06-03 02:27:06.000000 mousse-0.1.9/mousse.egg-info/PKG-INFO
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)     1085 2022-06-03 02:27:07.000000 mousse-0.1.9/mousse.egg-info/SOURCES.txt
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)        1 2022-06-03 02:27:07.000000 mousse-0.1.9/mousse.egg-info/dependency_links.txt
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)       50 2022-06-03 02:27:07.000000 mousse-0.1.9/mousse.egg-info/requires.txt
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)        7 2022-06-03 02:27:07.000000 mousse-0.1.9/mousse.egg-info/top_level.txt
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)       38 2022-06-03 02:27:07.394775 mousse-0.1.9/setup.cfg
+-rw-r--r--   0 VAI-DatNH21-L  (1000) dell      (1000)     1221 2022-06-03 02:26:20.000000 mousse-0.1.9/setup.py
```

### Comparing `mousse-0.1.8/PKG-INFO` & `mousse-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mousse
-Version: 0.1.8
+Version: 0.1.9
 Summary: mousse
 Home-page: https://github.com/NgHoangDat/mousse.git
-Download-URL: https://github.com/NgHoangDat/mousse/archive/v0.1.8.tar.gz
+Download-URL: https://github.com/NgHoangDat/mousse/archive/v0.1.9.tar.gz
 Author: nghoangdat
 Author-email: 18.hoang.dat.12@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mousse-0.1.8/README.md` & `mousse-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `mousse-0.1.8/mousse/__init__.py` & `mousse-0.1.9/mousse/__init__.py`

 * *Files identical despite different names*

### Comparing `mousse-0.1.8/mousse/cache/cache.py` & `mousse-0.1.9/mousse/cache/cache.py`

 * *Files identical despite different names*

### Comparing `mousse-0.1.8/mousse/cache/types.py` & `mousse-0.1.9/mousse/cache/types.py`

 * *Files identical despite different names*

### Comparing `mousse-0.1.8/mousse/config/config.py` & `mousse-0.1.9/mousse/config/config.py`

 * *Files identical despite different names*

### Comparing `mousse-0.1.8/mousse/data/accessor.py` & `mousse-0.1.9/mousse/data/accessor.py`

 * *Files identical despite different names*

### Comparing `mousse-0.1.8/mousse/data/dataclass.py` & `mousse-0.1.9/mousse/data/dataclass.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,21 +94,23 @@
                 setattr(result, k, deepcopy(v, memo))
 
             for key in get_fields_info(cls):
                 val = getattr(self, key)
                 setattr(result, key, deepcopy(val))
 
             return result
-        
+
         def __getstate__(self):
             from .parser import asdict
+
             return asdict(self)
-        
+
         def __setstate__(self, state: Dict[str, Any]):
             from .parser import asclass
+
             new = asclass(self.__class__, state)
             for key in get_fields_info(self.__class__):
                 val = getattr(new, key)
                 setattr(self, key, val)
 
         def __iter__(self):
             for key in get_fields_info(self.__class__):
```

### Comparing `mousse-0.1.8/mousse/data/parser.py` & `mousse-0.1.9/mousse/data/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         return val
 
 
 class DictParser(Parser):
     def __call__(self, val: Any, field: Field):
         if val == Ellipsis:
             return val
-        
+
         if isinstance(field.annotation, get_args(Generic)):
             if getattr(field.annotation, "_name", None) == "Dict":
                 return parse(field.annotation, val)
 
             return parse(get_origin(field.annotation), val)
 
         return val
```

### Comparing `mousse-0.1.8/mousse/data/types.py` & `mousse-0.1.9/mousse/data/types.py`

 * *Files identical despite different names*

### Comparing `mousse-0.1.8/mousse/data/validator.py` & `mousse-0.1.9/mousse/data/validator.py`

 * *Files identical despite different names*

### Comparing `mousse-0.1.8/mousse/export/exporter.py` & `mousse-0.1.9/mousse/export/exporter.py`

 * *Files identical despite different names*

### Comparing `mousse-0.1.8/mousse/functional/pattern/pattern.py` & `mousse-0.1.9/mousse/functional/pattern/pattern.py`

 * *Files identical despite different names*

### Comparing `mousse-0.1.8/mousse/functional/plugin.py` & `mousse-0.1.9/mousse/functional/plugin.py`

 * *Files identical despite different names*

### Comparing `mousse-0.1.8/mousse/functional/tools/functional.py` & `mousse-0.1.9/mousse/functional/tools/functional.py`

 * *Files identical despite different names*

### Comparing `mousse-0.1.8/mousse/logger/logger.py` & `mousse-0.1.9/mousse/logger/logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,79 +1,103 @@
 import asyncio
+import inspect
 import io
 import logging
 import os
 import time
 from functools import lru_cache, wraps
 from logging import Handler, StreamHandler
 from logging.handlers import RotatingFileHandler
+from pathlib import Path
 from typing import *
 from typing import Callable
 
 __all__ = ["init_logger", "get_logger", "log_error", "log_time", "add_handler"]
 
 
 FORMATTER = logging.Formatter(
-    "[%(asctime)s] [%(process)d %(thread)d] [%(levelname)s] [%(filename)s.%(funcName)s:%(lineno)i] %(message)s",
+    "[%(asctime)s] [%(process)d %(thread)d] [%(levelname)s] %(message)s",
     "%Y-%m-%d %H:%M:%S",
 )
 
 
 class LoggerWrapper:
     def __init__(self, logger: logging.Logger = None) -> None:
         self.logger = logger
         if self.logger is None:
             self.logger = logging.getLogger()
             add_handler(self.logger, StreamHandler())
 
-    def __gen_msg(self, *msg) -> str:
+    def __gen_msg(self, *msg, stack_level: int = 1) -> str:
         buffer = io.StringIO()
         print(*msg, end="", file=buffer)
         msg = buffer.getvalue()
+
+        frame = inspect.currentframe()
+        caller = frame.f_back
+        for _ in range(stack_level - 1):
+            f_prev = caller.f_back
+            if f_prev is not None:
+                caller = f_prev
+                
+        filepath = Path(caller.f_code.co_filename)
+        filename = f"{filepath.parent}/{filepath.stem}"
+
+        extra = {
+            "filename": filename,
+            "lineno": caller.f_lineno,
+            "func": caller.f_code.co_name,
+        }
+
+        msg = "[{filename}:{func}:{lineno}] {msg}".format(msg=msg, **extra)
         return msg
 
-    def info(self, *msg, stacklevel: int = 2, **kwargs) -> None:
-        return self.logger.info(self.__gen_msg(*msg), stacklevel=stacklevel, **kwargs)
+    def info(self, *msg, stack_level: int = 2, **kwargs) -> None:
+        return self.logger.info(self.__gen_msg(*msg, stack_level=stack_level), **kwargs)
 
-    def debug(self, *msg, stacklevel: int = 2, **kwargs) -> None:
-        return self.logger.debug(self.__gen_msg(*msg), stacklevel=stacklevel, **kwargs)
+    def debug(self, *msg, stack_level: int = 2, **kwargs) -> None:
+        return self.logger.debug(
+            self.__gen_msg(*msg, stack_level=stack_level), **kwargs
+        )
 
-    def error(self, *msg, stacklevel: int = 2, **kwargs) -> None:
-        return self.logger.error(self.__gen_msg(*msg), stacklevel=stacklevel, **kwargs)
+    def error(self, *msg, stack_level: int = 2, **kwargs) -> None:
+        return self.logger.error(
+            self.__gen_msg(*msg, stack_level=stack_level), **kwargs
+        )
 
-    def exception(self, *msg, stacklevel: int = 2, **kwargs) -> None:
+    def exception(self, *msg, stack_level: int = 2, **kwargs) -> None:
         return self.logger.exception(
-            self.__gen_msg(*msg), stacklevel=stacklevel, **kwargs
+            self.__gen_msg(*msg, stack_level=stack_level), **kwargs
         )
 
-    def critical(self, *msg, stacklevel: int = 2, **kwargs) -> None:
+    def critical(self, *msg, stack_level: int = 2, **kwargs) -> None:
         return self.logger.critical(
-            self.__gen_msg(*msg), stacklevel=stacklevel, **kwargs
+            self.__gen_msg(*msg, stack_level=stack_level), **kwargs
         )
 
-    def warning(self, *msg, stacklevel: int = 2, **kwargs) -> None:
+    def warning(self, *msg, stack_level: int = 2, **kwargs) -> None:
         return self.logger.warning(
-            self.__gen_msg(*msg), stacklevel=stacklevel, **kwargs
+            self.__gen_msg(*msg, stack_level=stack_level), **kwargs
         )
 
 
 @lru_cache(typed=True)
-def get_logger(*args):
+def __get_logger(name: str) -> LoggerWrapper:
     return LoggerWrapper()
 
 
+def get_logger(name: str = "default") -> LoggerWrapper:
+    return __get_logger(name)
+
+
 @lru_cache(typed=True)
-def init_logger(
-    name: str = "default",
-    log_dir: Optional[str] = None,
-    max_bytes: int = 10000000,
-    backup_count: int = 5,
-    level: int = logging.INFO,
-) -> logging.Logger:    
-    wrapper = get_logger(name)
+def __init_logger(
+    name: str, log_dir: str, max_bytes: int, backup_count: int, level: int
+) -> LoggerWrapper:
+    wrapper = get_logger(name=name)
     logger = wrapper.logger
     logger.setLevel(level)
 
     if log_dir is not None:
         os.makedirs(log_dir, exist_ok=True)
         log_filename = os.path.join(log_dir, f"{name}.out")
         add_handler(
@@ -82,14 +106,24 @@
                 log_filename, maxBytes=max_bytes, backupCount=backup_count
             ),
         )
 
     return wrapper
 
 
+def init_logger(
+    name: str = "default",
+    log_dir: Optional[str] = None,
+    max_bytes: int = 10000000,
+    backup_count: int = 5,
+    level: int = logging.INFO,
+) -> LoggerWrapper:
+    return __init_logger(name, log_dir, max_bytes, backup_count, level)
+
+
 def add_handler(
     logger: logging.Logger,
     *handlers: List[Handler],
     formatter: logging.Formatter = FORMATTER,
 ):
     for handler in handlers:
         handler.setFormatter(formatter)
@@ -114,30 +148,30 @@
         if asyncio.iscoroutinefunction(func):
 
             @wraps(func)
             async def wrapper(*args, **kwargs):
                 try:
                     res = await func(*args, **kwargs)
                 except Exception as e:
-                    logger.error(f"{func.__name__}: {e}", stacklevel=3)
+                    logger.error(f"{func.__name__}: {e}", stack_level=3)
                     if swallow_err:
                         return return_value
                     else:
                         raise e
                 else:
                     return res
 
         else:
 
             @wraps(func)
             def wrapper(*args, **kwargs):
                 try:
                     res = func(*args, **kwargs)
                 except Exception as e:
-                    logger.error(f"{func.__name__}: {e}", stacklevel=3)
+                    logger.error(f"{func.__name__}: {e}", stack_level=3)
                     if swallow_err:
                         return return_value
                     else:
                         raise e
                 else:
                     return res
 
@@ -163,25 +197,25 @@
         if asyncio.iscoroutinefunction(func):
 
             @wraps(func)
             async def wrapper(*args, **kwargs):
                 start = time.time()
                 res = await func(*args, **kwargs)
                 end = time.time()
-                logger.info(f"{func.__name__}: {end - start}s", stacklevel=3)
+                logger.info(f"{func.__name__}: {end - start}s", stack_level=3)
                 return res
 
         else:
 
             @wraps(func)
             def wrapper(*args, **kwargs):
                 start = time.time()
                 res = func(*args, **kwargs)
                 end = time.time()
-                logger.info(f"{func.__name__}: {end - start}s", stacklevel=3)
+                logger.info(f"{func.__name__}: {end - start}s", stack_level=3)
                 return res
 
         return wrapper
 
     if _func:
         return decorator(_func)
```

### Comparing `mousse-0.1.8/mousse/pattern/mediator.py` & `mousse-0.1.9/mousse/pattern/mediator.py`

 * *Files identical despite different names*

### Comparing `mousse-0.1.8/mousse/pattern/object_pool.py` & `mousse-0.1.9/mousse/pattern/object_pool.py`

 * *Files identical despite different names*

### Comparing `mousse-0.1.8/mousse/pattern/registry.py` & `mousse-0.1.9/mousse/pattern/registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from functools import partial, lru_cache
 from typing import *
 
 
 __all__ = ["Registry", "AutoRegistry", "register"]
 
+
 class Registry:
     __GLOBAl_REGISTRIES: Dict[str, "Registry"] = {}
 
     def __init__(self, attr_name: str = "__name__"):
         self.registry = {}
         self.attr_name = attr_name
```

### Comparing `mousse-0.1.8/mousse/pattern/singleton.py` & `mousse-0.1.9/mousse/pattern/singleton.py`

 * *Files identical despite different names*

### Comparing `mousse-0.1.8/mousse/scheduler/scheduler.py` & `mousse-0.1.9/mousse/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `mousse-0.1.8/mousse/scheduler/time.py` & `mousse-0.1.9/mousse/scheduler/time.py`

 * *Files identical despite different names*

### Comparing `mousse-0.1.8/mousse/scheduler/types.py` & `mousse-0.1.9/mousse/scheduler/types.py`

 * *Files identical despite different names*

### Comparing `mousse-0.1.8/mousse.egg-info/PKG-INFO` & `mousse-0.1.9/mousse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mousse
-Version: 0.1.8
+Version: 0.1.9
 Summary: mousse
 Home-page: https://github.com/NgHoangDat/mousse.git
-Download-URL: https://github.com/NgHoangDat/mousse/archive/v0.1.8.tar.gz
+Download-URL: https://github.com/NgHoangDat/mousse/archive/v0.1.9.tar.gz
 Author: nghoangdat
 Author-email: 18.hoang.dat.12@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mousse-0.1.8/mousse.egg-info/SOURCES.txt` & `mousse-0.1.9/mousse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mousse-0.1.8/setup.py` & `mousse-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
     
 def read_requirements(path: Union[str, Path]):
     with open(path, "r") as fh:
         return [line.strip() for line in fh.readlines() if not line.startswith("#")]
 
 
-__VERSION__ = "0.1.8"
+__VERSION__ = "0.1.9"
 
 requirements = read_requirements("requirements.txt")
 
 extras_require = {}
 for path in Path("extras").rglob("*.txt"):
     extras_require[path.stem] = read_requirements(path)
```

