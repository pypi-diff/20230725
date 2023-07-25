# Comparing `tmp/wow_ai_sdk-0.1.4.tar.gz` & `tmp/wow_ai_sdk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wow_ai_sdk-0.1.4.tar", max compression
+gzip compressed data, was "wow_ai_sdk-0.1.5.tar", max compression
```

## Comparing `wow_ai_sdk-0.1.4.tar` & `wow_ai_sdk-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     7857 2023-06-30 11:57:05.323031 wow_ai_sdk-0.1.4/README.md
--rw-r--r--   0        0        0      262 2023-07-18 03:05:19.660262 wow_ai_sdk-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      149 2023-01-28 11:24:39.272410 wow_ai_sdk-0.1.4/wow_ai_sdk/__init__.py
--rw-r--r--   0        0        0     8908 2023-07-18 03:05:07.528378 wow_ai_sdk-0.1.4/wow_ai_sdk/client.py
--rw-r--r--   0        0        0     7914 2023-01-28 11:24:40.157550 wow_ai_sdk-0.1.4/wow_ai_sdk/data_manager.py
--rw-r--r--   0        0        0    66648 2023-07-15 09:22:29.068399 wow_ai_sdk-0.1.4/wow_ai_sdk/project.py
--rw-r--r--   0        0        0     1325 2023-01-28 11:24:40.436036 wow_ai_sdk-0.1.4/wow_ai_sdk/users.py
--rw-r--r--   0        0        0     4218 2023-01-28 11:24:40.801400 wow_ai_sdk-0.1.4/wow_ai_sdk/utils.py
--rw-r--r--   0        0        0     1889 2023-01-28 11:24:41.002364 wow_ai_sdk-0.1.4/wow_ai_sdk/workspaces.py
--rw-r--r--   0        0        0     8289 1970-01-01 00:00:00.000000 wow_ai_sdk-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     7857 2023-06-30 11:57:05.323031 wow_ai_sdk-0.1.5/README.md
+-rw-r--r--   0        0        0      262 2023-07-25 07:28:40.016397 wow_ai_sdk-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      149 2023-01-28 11:24:39.272410 wow_ai_sdk-0.1.5/wow_ai_sdk/__init__.py
+-rw-r--r--   0        0        0     8908 2023-07-25 03:51:18.621099 wow_ai_sdk-0.1.5/wow_ai_sdk/client.py
+-rw-r--r--   0        0        0     7914 2023-01-28 11:24:40.157550 wow_ai_sdk-0.1.5/wow_ai_sdk/data_manager.py
+-rw-r--r--   0        0        0    68545 2023-07-25 04:37:43.837099 wow_ai_sdk-0.1.5/wow_ai_sdk/project.py
+-rw-r--r--   0        0        0     1325 2023-01-28 11:24:40.436036 wow_ai_sdk-0.1.5/wow_ai_sdk/users.py
+-rw-r--r--   0        0        0     4218 2023-01-28 11:24:40.801400 wow_ai_sdk-0.1.5/wow_ai_sdk/utils.py
+-rw-r--r--   0        0        0     1889 2023-01-28 11:24:41.002364 wow_ai_sdk-0.1.5/wow_ai_sdk/workspaces.py
+-rw-r--r--   0        0        0     8289 1970-01-01 00:00:00.000000 wow_ai_sdk-0.1.5/PKG-INFO
```

### Comparing `wow_ai_sdk-0.1.4/README.md` & `wow_ai_sdk-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `wow_ai_sdk-0.1.4/wow_ai_sdk/client.py` & `wow_ai_sdk-0.1.5/wow_ai_sdk/client.py`

 * *Files identical despite different names*

### Comparing `wow_ai_sdk-0.1.4/wow_ai_sdk/data_manager.py` & `wow_ai_sdk-0.1.5/wow_ai_sdk/data_manager.py`

 * *Files identical despite different names*

### Comparing `wow_ai_sdk-0.1.4/wow_ai_sdk/project.py` & `wow_ai_sdk-0.1.5/wow_ai_sdk/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1807,7 +1807,71 @@
         filename = None
         if response.status_code == 200:
             filename = response.headers.get('filename')
             with open(os.path.join(path, filename), 'wb') as f:
                 for chunk in response:
                     f.write(chunk)
         return response.status_code, filename
+    def export_snapshot_s3(self,
+                                 task_id: int):
+        """
+        
+        """
+        response = self.make_request('GET',
+                                     f'/api/tasks/{task_id}/queue')
+        
+        return response.json()
+    def add_task_queue(self,
+                                 task_id: int):
+        """
+        
+        """
+        payload = {
+            "project_id": self.id,
+            "task_id": task_id,
+            "try_count": 5,
+            "max_tries": 10,
+            "priority": 0,
+            "status": "pending"
+        }
+        response = self.make_request('POST',
+                                     f'/api/tasks/{task_id}/queue', json=payload)
+        
+        return response.json()
+    def crawl_list(self):
+        """
+        
+        """
+        response = self.make_request('GET',
+                                     f'/api/projects/{self.id}/queue')
+        
+        return response.json()
+    def add_crawl_queue(self,
+                                 task_id: int):
+        """
+        
+        """
+        response = self.make_request('POST',
+                                     f'/api/projects/{self.id}/queue')
+        
+        return response.json()
+    def train_list(self,ml_id: int):
+        """
+        
+        """
+        response = self.make_request('GET',
+                                     f'/api/ml/{ml_id}/queue')
+        
+        return response.json()
+    def add_train_queue(self,
+                                 ml_id: int):
+        """
+        
+        """
+        payload = {
+            "title": "",
+        }
+        response = self.make_request('POST',
+                                     f'/api/ml/{ml_id}/queue', json=payload)
+        
+        return response.json()
+    #https://stackoverflow.com/questions/47468148/how-to-copy-s3-object-from-one-bucket-to-another-using-python-boto3
```

### Comparing `wow_ai_sdk-0.1.4/wow_ai_sdk/users.py` & `wow_ai_sdk-0.1.5/wow_ai_sdk/users.py`

 * *Files identical despite different names*

### Comparing `wow_ai_sdk-0.1.4/wow_ai_sdk/utils.py` & `wow_ai_sdk-0.1.5/wow_ai_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `wow_ai_sdk-0.1.4/wow_ai_sdk/workspaces.py` & `wow_ai_sdk-0.1.5/wow_ai_sdk/workspaces.py`

 * *Files identical despite different names*

### Comparing `wow_ai_sdk-0.1.4/PKG-INFO` & `wow_ai_sdk-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wow-ai-sdk
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: TonyShark
 Author-email: quoi@wow-ai.inc
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

