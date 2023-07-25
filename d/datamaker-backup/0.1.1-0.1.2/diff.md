# Comparing `tmp/datamaker-backup-0.1.1.tar.gz` & `tmp/datamaker-backup-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamaker-backup-0.1.1.tar", last modified: Tue Jul 25 13:05:12 2023, max compression
+gzip compressed data, was "datamaker-backup-0.1.2.tar", last modified: Tue Jul 25 13:09:58 2023, max compression
```

## Comparing `datamaker-backup-0.1.1.tar` & `datamaker-backup-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-07-25 13:05:12.864727 datamaker-backup-0.1.1/
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1101 2023-07-25 09:30:36.000000 datamaker-backup-0.1.1/LICENSE
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1982 2023-07-25 13:05:12.864727 datamaker-backup-0.1.1/PKG-INFO
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1253 2023-07-25 13:05:05.000000 datamaker-backup-0.1.1/README.md
-drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-07-25 13:05:12.864727 datamaker-backup-0.1.1/datamaker_backup/
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)       39 2023-07-25 09:30:36.000000 datamaker-backup-0.1.1/datamaker_backup/__init__.py
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     5094 2023-07-25 09:30:36.000000 datamaker-backup-0.1.1/datamaker_backup/storage.py
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1159 2023-07-25 09:30:36.000000 datamaker-backup-0.1.1/datamaker_backup/utils.py
-drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-07-25 13:05:12.864727 datamaker-backup-0.1.1/datamaker_backup.egg-info/
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1982 2023-07-25 13:05:12.000000 datamaker-backup-0.1.1/datamaker_backup.egg-info/PKG-INFO
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      324 2023-07-25 13:05:12.000000 datamaker-backup-0.1.1/datamaker_backup.egg-info/SOURCES.txt
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)        1 2023-07-25 13:05:12.000000 datamaker-backup-0.1.1/datamaker_backup.egg-info/dependency_links.txt
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)       52 2023-07-25 13:05:12.000000 datamaker-backup-0.1.1/datamaker_backup.egg-info/requires.txt
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)       17 2023-07-25 13:05:12.000000 datamaker-backup-0.1.1/datamaker_backup.egg-info/top_level.txt
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      106 2023-07-25 13:05:05.000000 datamaker-backup-0.1.1/pyproject.toml
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      839 2023-07-25 13:05:12.864727 datamaker-backup-0.1.1/setup.cfg
+drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-07-25 13:09:58.480890 datamaker-backup-0.1.2/
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1101 2023-07-25 09:30:36.000000 datamaker-backup-0.1.2/LICENSE
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1982 2023-07-25 13:09:58.480890 datamaker-backup-0.1.2/PKG-INFO
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1253 2023-07-25 13:05:05.000000 datamaker-backup-0.1.2/README.md
+drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-07-25 13:09:58.476890 datamaker-backup-0.1.2/datamaker_backup/
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)       39 2023-07-25 09:30:36.000000 datamaker-backup-0.1.2/datamaker_backup/__init__.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     5094 2023-07-25 09:30:36.000000 datamaker-backup-0.1.2/datamaker_backup/storage.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1159 2023-07-25 09:30:36.000000 datamaker-backup-0.1.2/datamaker_backup/utils.py
+drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-07-25 13:09:58.480890 datamaker-backup-0.1.2/datamaker_backup.egg-info/
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1982 2023-07-25 13:09:58.000000 datamaker-backup-0.1.2/datamaker_backup.egg-info/PKG-INFO
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      324 2023-07-25 13:09:58.000000 datamaker-backup-0.1.2/datamaker_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)        1 2023-07-25 13:09:58.000000 datamaker-backup-0.1.2/datamaker_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)       52 2023-07-25 13:09:58.000000 datamaker-backup-0.1.2/datamaker_backup.egg-info/requires.txt
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)       17 2023-07-25 13:09:58.000000 datamaker-backup-0.1.2/datamaker_backup.egg-info/top_level.txt
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      106 2023-07-25 13:05:05.000000 datamaker-backup-0.1.2/pyproject.toml
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      839 2023-07-25 13:09:58.480890 datamaker-backup-0.1.2/setup.cfg
```

### Comparing `datamaker-backup-0.1.1/LICENSE` & `datamaker-backup-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datamaker-backup-0.1.1/PKG-INFO` & `datamaker-backup-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamaker-backup
-Version: 0.1.1
+Version: 0.1.2
 Summary: datamaker backup
 Home-page: https://www.datamaker.io
 Author: datamaker
 Author-email: developer@datamaker.io
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datamaker-backup-0.1.1/README.md` & `datamaker-backup-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `datamaker-backup-0.1.1/datamaker_backup/storage.py` & `datamaker-backup-0.1.2/datamaker_backup/storage.py`

 * *Files identical despite different names*

### Comparing `datamaker-backup-0.1.1/datamaker_backup/utils.py` & `datamaker-backup-0.1.2/datamaker_backup/utils.py`

 * *Files identical despite different names*

### Comparing `datamaker-backup-0.1.1/datamaker_backup.egg-info/PKG-INFO` & `datamaker-backup-0.1.2/datamaker_backup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamaker-backup
-Version: 0.1.1
+Version: 0.1.2
 Summary: datamaker backup
 Home-page: https://www.datamaker.io
 Author: datamaker
 Author-email: developer@datamaker.io
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datamaker-backup-0.1.1/setup.cfg` & `datamaker-backup-0.1.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = datamaker-backup
-version = 0.1.1
+version = 0.1.2
 description = datamaker backup
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://www.datamaker.io
 author = datamaker
 author_email = developer@datamaker.io
 license = MIT
```

