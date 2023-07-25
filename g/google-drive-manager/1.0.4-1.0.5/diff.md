# Comparing `tmp/google-drive-manager-1.0.4.tar.gz` & `tmp/google-drive-manager-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-drive-manager-1.0.4.tar", last modified: Tue Jul 25 13:41:36 2023, max compression
+gzip compressed data, was "google-drive-manager-1.0.5.tar", last modified: Tue Jul 25 13:43:29 2023, max compression
```

## Comparing `google-drive-manager-1.0.4.tar` & `google-drive-manager-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 guillaume  (1000) guillaume  (1000)        0 2023-07-25 13:41:36.391736 google-drive-manager-1.0.4/
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)     1006 2023-07-25 13:41:36.391736 google-drive-manager-1.0.4/PKG-INFO
-drwxrwxr-x   0 guillaume  (1000) guillaume  (1000)        0 2023-07-25 13:41:36.387736 google-drive-manager-1.0.4/google_drive_manager/
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)        0 2023-07-24 15:14:53.000000 google-drive-manager-1.0.4/google_drive_manager/__init__.py
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)    11129 2023-07-25 09:27:53.000000 google-drive-manager-1.0.4/google_drive_manager/google_drive_manager.py
-drwxrwxr-x   0 guillaume  (1000) guillaume  (1000)        0 2023-07-25 13:41:36.391736 google-drive-manager-1.0.4/google_drive_manager.egg-info/
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)     1006 2023-07-25 13:41:36.000000 google-drive-manager-1.0.4/google_drive_manager.egg-info/PKG-INFO
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)      305 2023-07-25 13:41:36.000000 google-drive-manager-1.0.4/google_drive_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)        1 2023-07-25 13:41:36.000000 google-drive-manager-1.0.4/google_drive_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)       61 2023-07-25 13:41:36.000000 google-drive-manager-1.0.4/google_drive_manager.egg-info/requires.txt
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)       21 2023-07-25 13:41:36.000000 google-drive-manager-1.0.4/google_drive_manager.egg-info/top_level.txt
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)       38 2023-07-25 13:41:36.391736 google-drive-manager-1.0.4/setup.cfg
--rw-rw-r--   0 guillaume  (1000) guillaume  (1000)     1068 2023-07-25 13:41:17.000000 google-drive-manager-1.0.4/setup.py
+drwxrwxr-x   0 guillaume  (1000) guillaume  (1000)        0 2023-07-25 13:43:29.483986 google-drive-manager-1.0.5/
+-rw-rw-r--   0 guillaume  (1000) guillaume  (1000)      985 2023-07-25 13:43:29.479987 google-drive-manager-1.0.5/PKG-INFO
+drwxrwxr-x   0 guillaume  (1000) guillaume  (1000)        0 2023-07-25 13:43:29.475987 google-drive-manager-1.0.5/google_drive_manager/
+-rw-rw-r--   0 guillaume  (1000) guillaume  (1000)        0 2023-07-24 15:14:53.000000 google-drive-manager-1.0.5/google_drive_manager/__init__.py
+-rw-rw-r--   0 guillaume  (1000) guillaume  (1000)    11129 2023-07-25 09:27:53.000000 google-drive-manager-1.0.5/google_drive_manager/google_drive_manager.py
+drwxrwxr-x   0 guillaume  (1000) guillaume  (1000)        0 2023-07-25 13:43:29.479987 google-drive-manager-1.0.5/google_drive_manager.egg-info/
+-rw-rw-r--   0 guillaume  (1000) guillaume  (1000)      985 2023-07-25 13:43:29.000000 google-drive-manager-1.0.5/google_drive_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 guillaume  (1000) guillaume  (1000)      305 2023-07-25 13:43:29.000000 google-drive-manager-1.0.5/google_drive_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 guillaume  (1000) guillaume  (1000)        1 2023-07-25 13:43:29.000000 google-drive-manager-1.0.5/google_drive_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 guillaume  (1000) guillaume  (1000)       61 2023-07-25 13:43:29.000000 google-drive-manager-1.0.5/google_drive_manager.egg-info/requires.txt
+-rw-rw-r--   0 guillaume  (1000) guillaume  (1000)       21 2023-07-25 13:43:29.000000 google-drive-manager-1.0.5/google_drive_manager.egg-info/top_level.txt
+-rw-rw-r--   0 guillaume  (1000) guillaume  (1000)       38 2023-07-25 13:43:29.483986 google-drive-manager-1.0.5/setup.cfg
+-rw-rw-r--   0 guillaume  (1000) guillaume  (1000)     1047 2023-07-25 13:43:19.000000 google-drive-manager-1.0.5/setup.py
```

### Comparing `google-drive-manager-1.0.4/PKG-INFO` & `google-drive-manager-1.0.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: google-drive-manager
-Version: 1.0.4
+Version: 1.0.5
 Summary: Un gestionnaire de Google Drive
 Home-page: UNKNOWN
 Author: Guillaume LECOSSOIS
 Author-email: <guillaume.lecossois@diabeloop.fr>
 License: UNKNOWN
-Description: `google-drive-manager` est une librairie conçue pour interagir avec Google Drive en Python. Avec son API simple, vous pouvez gérer les données de différents fichiers et dossiers dans le Google Drive de Diabeloop. 
-        
-        La liste des méthodes:
+Description: `google-drive-manager` is a library designed for interact with Google Drive in Python. With its simple API, you can manage data from various files and folders in the Diabeloop Google Drive. 
+            
+        The list of the methods :
         
         - `get_service`
         - `connect`
         - `getSpreadSheetInfoByID`
         - `listSheets`
         - `getSheetByName`
         - `getAllValuesFromSheet`
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `google-drive-manager-1.0.4/google_drive_manager/google_drive_manager.py` & `google-drive-manager-1.0.5/google_drive_manager/google_drive_manager.py`

 * *Files identical despite different names*

### Comparing `google-drive-manager-1.0.4/google_drive_manager.egg-info/PKG-INFO` & `google-drive-manager-1.0.5/google_drive_manager.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: google-drive-manager
-Version: 1.0.4
+Version: 1.0.5
 Summary: Un gestionnaire de Google Drive
 Home-page: UNKNOWN
 Author: Guillaume LECOSSOIS
 Author-email: <guillaume.lecossois@diabeloop.fr>
 License: UNKNOWN
-Description: `google-drive-manager` est une librairie conçue pour interagir avec Google Drive en Python. Avec son API simple, vous pouvez gérer les données de différents fichiers et dossiers dans le Google Drive de Diabeloop. 
-        
-        La liste des méthodes:
+Description: `google-drive-manager` is a library designed for interact with Google Drive in Python. With its simple API, you can manage data from various files and folders in the Diabeloop Google Drive. 
+            
+        The list of the methods :
         
         - `get_service`
         - `connect`
         - `getSpreadSheetInfoByID`
         - `listSheets`
         - `getSheetByName`
         - `getAllValuesFromSheet`
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `google-drive-manager-1.0.4/setup.py` & `google-drive-manager-1.0.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='google-drive-manager',
-    version='1.0.4',
+    version='1.0.5',
     author="Guillaume LECOSSOIS",
     author_email="<guillaume.lecossois@diabeloop.fr>",
     description='Un gestionnaire de Google Drive',
     long_description_content_type="text/markdown",
-    long_description="""`google-drive-manager` est une librairie conçue pour interagir avec Google Drive en Python. Avec son API simple, vous pouvez gérer les données de différents fichiers et dossiers dans le Google Drive de Diabeloop. 
-
-La liste des méthodes:
+    long_description="""`google-drive-manager` is a library designed for interact with Google Drive in Python. With its simple API, you can manage data from various files and folders in the Diabeloop Google Drive. 
+    
+The list of the methods :
 
 - `get_service`
 - `connect`
 - `getSpreadSheetInfoByID`
 - `listSheets`
 - `getSheetByName`
 - `getAllValuesFromSheet`
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

