# Comparing `tmp/pybarb-0.3.7.tar.gz` & `tmp/pybarb-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybarb-0.3.7.tar", last modified: Tue Jun 27 08:18:39 2023, max compression
+gzip compressed data, was "pybarb-0.3.8.tar", last modified: Tue Jul 25 11:07:06 2023, max compression
```

## Comparing `pybarb-0.3.7.tar` & `pybarb-0.3.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:18:39.527027 pybarb-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-27 08:18:39.527027 pybarb-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-27 08:18:28.000000 pybarb-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:18:39.527027 pybarb-0.3.7/pybarb/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-27 08:18:28.000000 pybarb-0.3.7/pybarb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32202 2023-06-27 08:18:28.000000 pybarb-0.3.7/pybarb/pybarb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:18:39.527027 pybarb-0.3.7/pybarb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-27 08:18:39.000000 pybarb-0.3.7/pybarb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-27 08:18:39.000000 pybarb-0.3.7/pybarb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 08:18:39.000000 pybarb-0.3.7/pybarb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-27 08:18:39.000000 pybarb-0.3.7/pybarb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 08:18:39.000000 pybarb-0.3.7/pybarb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 08:18:39.527027 pybarb-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-27 08:18:28.000000 pybarb-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:07:06.039852 pybarb-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-25 11:07:06.039852 pybarb-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-25 11:06:56.000000 pybarb-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:07:06.039852 pybarb-0.3.8/pybarb/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-25 11:06:56.000000 pybarb-0.3.8/pybarb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32473 2023-07-25 11:06:56.000000 pybarb-0.3.8/pybarb/pybarb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:07:06.039852 pybarb-0.3.8/pybarb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-25 11:07:06.000000 pybarb-0.3.8/pybarb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-25 11:07:06.000000 pybarb-0.3.8/pybarb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 11:07:06.000000 pybarb-0.3.8/pybarb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-25 11:07:06.000000 pybarb-0.3.8/pybarb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 11:07:06.000000 pybarb-0.3.8/pybarb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 11:07:06.039852 pybarb-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-25 11:06:56.000000 pybarb-0.3.8/setup.py
```

### Comparing `pybarb-0.3.7/README.md` & `pybarb-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `pybarb-0.3.7/pybarb/pybarb.py` & `pybarb-0.3.8/pybarb/pybarb.py`

 * *Files 0% similar despite different names*

```diff
@@ -409,15 +409,15 @@
 
         if job_id is None:
             job_id = self.current_job_id
         
         api_url = f"{self.api_root}async-batch/results/{job_id}"
         r = requests.get(url=api_url, headers=self.headers)
         r_json = r.json()
-        if len(r_json['result']) == 0:
+        if r_json['status'] == 'started':
             return False
         urls = [x['data'] for x in r_json['result']]
         return urls
     
     def get_asynch_files(self):
         """
         Gets the asynch files.
@@ -780,9 +780,19 @@
 
         # Drop all columns from df with datatype that is a dict
 
         df = pd.DataFrame(rows)
         df = df.drop(columns=["panel_member_weights", "tv_set_properties"]).drop_duplicates()
 
         return df
+    
+    def to_json(self, file_name):
+        """
+        Converts the API response data into a json object.
+
+        Returns:
+            json: A json containing the API response data.
+        """
+
+        self.api_response_data.to_json(file_name, orient='records')
```

