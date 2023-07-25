# Comparing `tmp/hydroloader-0.1.7.tar.gz` & `tmp/hydroloader-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydroloader-0.1.7.tar", last modified: Fri Jun 30 05:22:17 2023, max compression
+gzip compressed data, was "hydroloader-0.1.8.tar", last modified: Tue Jul 25 16:42:05 2023, max compression
```

## Comparing `hydroloader-0.1.7.tar` & `hydroloader-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-06-30 05:22:17.904756 hydroloader-0.1.7/
--rw-r--r--   0 klippold   (501) staff       (20)     1094 2023-06-07 22:04:25.000000 hydroloader-0.1.7/LICENSE.txt
--rw-r--r--   0 klippold   (501) staff       (20)      102 2023-06-30 05:22:17.904804 hydroloader-0.1.7/PKG-INFO
--rw-r--r--   0 klippold   (501) staff       (20)        0 2023-06-07 22:04:25.000000 hydroloader-0.1.7/README.md
--rw-r--r--   0 klippold   (501) staff       (20)       80 2023-06-07 22:04:25.000000 hydroloader-0.1.7/pyproject.toml
--rw-r--r--   0 klippold   (501) staff       (20)      378 2023-06-30 05:22:17.905065 hydroloader-0.1.7/setup.cfg
--rw-r--r--   0 klippold   (501) staff       (20)       93 2023-06-07 22:04:25.000000 hydroloader-0.1.7/setup.py
-drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-06-30 05:22:17.902562 hydroloader-0.1.7/src/
-drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-06-30 05:22:17.903792 hydroloader-0.1.7/src/hydroloader/
--rw-r--r--   0 klippold   (501) staff       (20)      396 2023-06-26 22:58:34.000000 hydroloader-0.1.7/src/hydroloader/__init__.py
--rw-r--r--   0 klippold   (501) staff       (20)      314 2023-06-14 20:27:28.000000 hydroloader-0.1.7/src/hydroloader/exceptions.py
--rw-r--r--   0 klippold   (501) staff       (20)    15536 2023-06-30 05:21:23.000000 hydroloader-0.1.7/src/hydroloader/main.py
--rw-r--r--   0 klippold   (501) staff       (20)     7984 2023-06-28 22:35:17.000000 hydroloader-0.1.7/src/hydroloader/models.py
-drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-06-30 05:22:17.904625 hydroloader-0.1.7/src/hydroloader.egg-info/
--rw-r--r--   0 klippold   (501) staff       (20)      102 2023-06-30 05:22:17.000000 hydroloader-0.1.7/src/hydroloader.egg-info/PKG-INFO
--rw-r--r--   0 klippold   (501) staff       (20)      391 2023-06-30 05:22:17.000000 hydroloader-0.1.7/src/hydroloader.egg-info/SOURCES.txt
--rw-r--r--   0 klippold   (501) staff       (20)        1 2023-06-30 05:22:17.000000 hydroloader-0.1.7/src/hydroloader.egg-info/dependency_links.txt
--rw-r--r--   0 klippold   (501) staff       (20)      124 2023-06-30 05:22:17.000000 hydroloader-0.1.7/src/hydroloader.egg-info/requires.txt
--rw-r--r--   0 klippold   (501) staff       (20)       12 2023-06-30 05:22:17.000000 hydroloader-0.1.7/src/hydroloader.egg-info/top_level.txt
--rw-r--r--   0 klippold   (501) staff       (20)        1 2023-06-07 22:05:51.000000 hydroloader-0.1.7/src/hydroloader.egg-info/zip-safe
+drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-07-25 16:42:05.676277 hydroloader-0.1.8/
+-rw-r--r--   0 klippold   (501) staff       (20)     1094 2023-06-07 22:04:25.000000 hydroloader-0.1.8/LICENSE.txt
+-rw-r--r--   0 klippold   (501) staff       (20)      102 2023-07-25 16:42:05.676345 hydroloader-0.1.8/PKG-INFO
+-rw-r--r--   0 klippold   (501) staff       (20)        0 2023-06-07 22:04:25.000000 hydroloader-0.1.8/README.md
+-rw-r--r--   0 klippold   (501) staff       (20)       80 2023-06-07 22:04:25.000000 hydroloader-0.1.8/pyproject.toml
+-rw-r--r--   0 klippold   (501) staff       (20)      378 2023-07-25 16:42:05.676654 hydroloader-0.1.8/setup.cfg
+-rw-r--r--   0 klippold   (501) staff       (20)       93 2023-06-07 22:04:25.000000 hydroloader-0.1.8/setup.py
+drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-07-25 16:42:05.673361 hydroloader-0.1.8/src/
+drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-07-25 16:42:05.675111 hydroloader-0.1.8/src/hydroloader/
+-rw-r--r--   0 klippold   (501) staff       (20)      396 2023-06-26 22:58:34.000000 hydroloader-0.1.8/src/hydroloader/__init__.py
+-rw-r--r--   0 klippold   (501) staff       (20)      314 2023-06-14 20:27:28.000000 hydroloader-0.1.8/src/hydroloader/exceptions.py
+-rw-r--r--   0 klippold   (501) staff       (20)    15536 2023-06-30 05:21:23.000000 hydroloader-0.1.8/src/hydroloader/main.py
+-rw-r--r--   0 klippold   (501) staff       (20)     7973 2023-07-25 16:37:24.000000 hydroloader-0.1.8/src/hydroloader/models.py
+drwxr-xr-x   0 klippold   (501) staff       (20)        0 2023-07-25 16:42:05.675941 hydroloader-0.1.8/src/hydroloader.egg-info/
+-rw-r--r--   0 klippold   (501) staff       (20)      102 2023-07-25 16:42:05.000000 hydroloader-0.1.8/src/hydroloader.egg-info/PKG-INFO
+-rw-r--r--   0 klippold   (501) staff       (20)      391 2023-07-25 16:42:05.000000 hydroloader-0.1.8/src/hydroloader.egg-info/SOURCES.txt
+-rw-r--r--   0 klippold   (501) staff       (20)        1 2023-07-25 16:42:05.000000 hydroloader-0.1.8/src/hydroloader.egg-info/dependency_links.txt
+-rw-r--r--   0 klippold   (501) staff       (20)      124 2023-07-25 16:42:05.000000 hydroloader-0.1.8/src/hydroloader.egg-info/requires.txt
+-rw-r--r--   0 klippold   (501) staff       (20)       12 2023-07-25 16:42:05.000000 hydroloader-0.1.8/src/hydroloader.egg-info/top_level.txt
+-rw-r--r--   0 klippold   (501) staff       (20)        1 2023-06-07 22:05:51.000000 hydroloader-0.1.8/src/hydroloader.egg-info/zip-safe
```

### Comparing `hydroloader-0.1.7/LICENSE.txt` & `hydroloader-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hydroloader-0.1.7/src/hydroloader/main.py` & `hydroloader-0.1.8/src/hydroloader/main.py`

 * *Files identical despite different names*

### Comparing `hydroloader-0.1.7/src/hydroloader/models.py` & `hydroloader-0.1.8/src/hydroloader/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
             raise ValueError('The offset must be a valid UTC timezone offset formatted such as "+0000".')
 
         return datetime.strptime(v, '%z').tzinfo if v is not None else None
 
 
 class HydroLoaderConfFileDatastream(BaseModel):
     column: Union[conint(gt=0), str]
-    datastream_id: UUID
+    id: UUID
 
 
 class HydroLoaderConf(BaseModel):
     schedule: Optional[HydroLoaderConfSchedule]
     file_access: HydroLoaderConfFileAccess
     file_timestamp: HydroLoaderConfFileTimestamp
     datastreams: List[HydroLoaderConfFileDatastream]
```

