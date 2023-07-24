# Comparing `tmp/lexsetAPI-3.4.8.tar.gz` & `tmp/lexsetAPI-3.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexsetAPI-3.4.8.tar", last modified: Tue Jul 18 18:30:05 2023, max compression
+gzip compressed data, was "lexsetAPI-3.4.9.tar", last modified: Mon Jul 24 22:19:38 2023, max compression
```

## Comparing `lexsetAPI-3.4.8.tar` & `lexsetAPI-3.4.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:30:05.650911 lexsetAPI-3.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-18 18:30:05.650911 lexsetAPI-3.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-18 18:29:44.000000 lexsetAPI-3.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:30:05.646911 lexsetAPI-3.4.8/lexsetAPI/
--rw-r--r--   0 runner    (1001) docker     (123)    27409 2023-07-18 18:29:44.000000 lexsetAPI-3.4.8/lexsetAPI/LexsetManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-18 18:29:44.000000 lexsetAPI-3.4.8/lexsetAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-18 18:29:44.000000 lexsetAPI-3.4.8/lexsetAPI/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:30:05.650911 lexsetAPI-3.4.8/lexsetAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-18 18:30:05.000000 lexsetAPI-3.4.8/lexsetAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-18 18:30:05.000000 lexsetAPI-3.4.8/lexsetAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:30:05.000000 lexsetAPI-3.4.8/lexsetAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-18 18:30:05.000000 lexsetAPI-3.4.8/lexsetAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 18:30:05.000000 lexsetAPI-3.4.8/lexsetAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 18:30:05.650911 lexsetAPI-3.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-18 18:29:44.000000 lexsetAPI-3.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:19:38.753803 lexsetAPI-3.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-24 22:19:38.749803 lexsetAPI-3.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-24 22:19:16.000000 lexsetAPI-3.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:19:38.749803 lexsetAPI-3.4.9/lexsetAPI/
+-rw-r--r--   0 runner    (1001) docker     (123)    27495 2023-07-24 22:19:16.000000 lexsetAPI-3.4.9/lexsetAPI/LexsetManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-24 22:19:16.000000 lexsetAPI-3.4.9/lexsetAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-24 22:19:16.000000 lexsetAPI-3.4.9/lexsetAPI/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:19:38.749803 lexsetAPI-3.4.9/lexsetAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-24 22:19:38.000000 lexsetAPI-3.4.9/lexsetAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-24 22:19:38.000000 lexsetAPI-3.4.9/lexsetAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 22:19:38.000000 lexsetAPI-3.4.9/lexsetAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-24 22:19:38.000000 lexsetAPI-3.4.9/lexsetAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-24 22:19:38.000000 lexsetAPI-3.4.9/lexsetAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 22:19:38.753803 lexsetAPI-3.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-24 22:19:16.000000 lexsetAPI-3.4.9/setup.py
```

### Comparing `lexsetAPI-3.4.8/lexsetAPI/LexsetManager.py` & `lexsetAPI-3.4.9/lexsetAPI/LexsetManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import yaml
 import base64
 #import threading
 from tqdm import tqdm
 import os
 import shutil
 from concurrent.futures import ThreadPoolExecutor
+import time
 #import subprocess
 
 # This class will No longer be supported in version 4+ of the API
 class simulation:
 
     def __init__(self,token,simPath,numImages,user,nodes,name,descript,seed):
         self.token = token
@@ -74,14 +75,16 @@
         payload={}
         headers = {
         'Authorization': 'Bearer ' + self.token
         }
 
         response = requests.request("POST", url, headers=headers, data=payload)
 
+        time.sleep(5)
+
     def getStatus(self):
         url = "https://lexsetapi.azurewebsites.net/api/simulations/getsimulationstatus?id=" + str(self.simID)
 
         payload={}
         headers = {
         'Authorization': 'Bearer ' + self.token
         }
@@ -284,19 +287,21 @@
     response = requests.request("POST", url, headers=headers, data=payload)
     
     getCode = response.status_code
     if getCode == 401:
         return("Unauthorized")
     if getCode == 200:
         #parseResponse = json.loads(response.text)
+        time.sleep(5)
         return("success")
     else:
         print("Error: " + str(getCode))
         return(getCode)
 
+
 #phase out in future versions
 def download(datasetID ,userToken, localPath = "NONE"):
     url = "https://lexsetapi.azurewebsites.net/api/datasets/getdatasetarchives?dataset_id=" + str(datasetID)
 
     payload={}
     headers = {
     'Authorization': 'Bearer ' + userToken
@@ -412,14 +417,15 @@
 
         payload={}
         headers = {
         'Authorization': 'Bearer ' + self.token
         }
 
         response = requests.request("POST", url, headers=headers, data=payload)
+        time.sleep(5)
         # print('NEW JOB STARTED: ' + str(self.simID) + ' has started')
         # print('-------------')
 
 
     def updateStatus(self):
         url = "https://lexsetapi.azurewebsites.net/api/simulations/getsimulationstatus?id=" + str(self.simID)
```

### Comparing `lexsetAPI-3.4.8/lexsetAPI/credentials.py` & `lexsetAPI-3.4.9/lexsetAPI/credentials.py`

 * *Files identical despite different names*

