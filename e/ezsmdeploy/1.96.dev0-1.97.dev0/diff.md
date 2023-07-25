# Comparing `tmp/ezsmdeploy-1.96.dev0.tar.gz` & `tmp/ezsmdeploy-1.97.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezsmdeploy-1.96.dev0.tar", last modified: Tue Jul 18 18:13:19 2023, max compression
+gzip compressed data, was "ezsmdeploy-1.97.dev0.tar", last modified: Tue Jul 25 19:09:48 2023, max compression
```

## Comparing `ezsmdeploy-1.96.dev0.tar` & `ezsmdeploy-1.97.dev0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-18 18:13:19.254948 ezsmdeploy-1.96.dev0/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       26 2023-07-18 17:32:09.000000 ezsmdeploy-1.96.dev0/MANIFEST.in
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    19598 2023-07-18 18:13:19.254948 ezsmdeploy-1.96.dev0/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    19108 2023-07-18 17:32:09.000000 ezsmdeploy-1.96.dev0/README.rst
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-18 18:13:19.254948 ezsmdeploy-1.96.dev0/ezsmdeploy/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    48489 2023-07-18 17:48:22.000000 ezsmdeploy-1.96.dev0/ezsmdeploy/__init__.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-18 18:13:19.254948 ezsmdeploy-1.96.dev0/ezsmdeploy/data/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2100 2023-07-18 17:32:09.000000 ezsmdeploy-1.96.dev0/ezsmdeploy/data/Dockerfile
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1934 2023-07-18 17:32:09.000000 ezsmdeploy-1.96.dev0/ezsmdeploy/data/Dockerfile_flask
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1390 2023-07-18 17:32:09.000000 ezsmdeploy-1.96.dev0/ezsmdeploy/data/build-docker.sh
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1603 2023-07-18 17:32:09.000000 ezsmdeploy-1.96.dev0/ezsmdeploy/data/conversation.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1361 2023-07-18 17:32:09.000000 ezsmdeploy-1.96.dev0/ezsmdeploy/data/cost.csv
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      884 2023-07-18 17:32:09.000000 ezsmdeploy-1.96.dev0/ezsmdeploy/data/dockerd-entrypoint.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      576 2023-07-18 17:32:09.000000 ezsmdeploy-1.96.dev0/ezsmdeploy/data/instancetypes.csv
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1797 2023-07-18 17:32:09.000000 ezsmdeploy-1.96.dev0/ezsmdeploy/data/model_handler.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      719 2023-07-18 17:32:09.000000 ezsmdeploy-1.96.dev0/ezsmdeploy/data/nginx.conf
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2090 2023-07-18 17:32:09.000000 ezsmdeploy-1.96.dev0/ezsmdeploy/data/predictor.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2429 2023-07-18 17:32:09.000000 ezsmdeploy-1.96.dev0/ezsmdeploy/data/serve
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1409 2023-07-18 17:32:09.000000 ezsmdeploy-1.96.dev0/ezsmdeploy/data/smlocust.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      432 2023-07-18 17:32:09.000000 ezsmdeploy-1.96.dev0/ezsmdeploy/data/train
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      202 2023-07-18 17:32:09.000000 ezsmdeploy-1.96.dev0/ezsmdeploy/data/wsgi.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      733 2023-07-18 17:32:09.000000 ezsmdeploy-1.96.dev0/ezsmdeploy/modelscript_sklearn.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-18 18:13:19.254948 ezsmdeploy-1.96.dev0/ezsmdeploy.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    19598 2023-07-18 18:13:19.000000 ezsmdeploy-1.96.dev0/ezsmdeploy.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      696 2023-07-18 18:13:19.000000 ezsmdeploy-1.96.dev0/ezsmdeploy.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-07-18 18:13:19.000000 ezsmdeploy-1.96.dev0/ezsmdeploy.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-07-18 17:33:24.000000 ezsmdeploy-1.96.dev0/ezsmdeploy.egg-info/not-zip-safe
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      129 2023-07-18 18:13:19.000000 ezsmdeploy-1.96.dev0/ezsmdeploy.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       11 2023-07-18 18:13:19.000000 ezsmdeploy-1.96.dev0/ezsmdeploy.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-07-18 18:13:19.254948 ezsmdeploy-1.96.dev0/setup.cfg
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1274 2023-07-18 18:13:00.000000 ezsmdeploy-1.96.dev0/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-25 19:09:48.675099 ezsmdeploy-1.97.dev0/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       26 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/MANIFEST.in
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    19598 2023-07-25 19:09:48.675099 ezsmdeploy-1.97.dev0/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    19108 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/README.rst
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-25 19:09:48.675099 ezsmdeploy-1.97.dev0/ezsmdeploy/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    48489 2023-07-25 19:08:36.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/__init__.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-25 19:09:48.675099 ezsmdeploy-1.97.dev0/ezsmdeploy/data/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2100 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/data/Dockerfile
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1934 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/data/Dockerfile_flask
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1390 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/data/build-docker.sh
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1603 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/data/conversation.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1361 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/data/cost.csv
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      884 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/data/dockerd-entrypoint.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      576 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/data/instancetypes.csv
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1797 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/data/model_handler.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      719 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/data/nginx.conf
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2090 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/data/predictor.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2429 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/data/serve
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1409 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/data/smlocust.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      432 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/data/train
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      202 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/data/wsgi.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      733 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/modelscript_sklearn.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-25 19:09:48.675099 ezsmdeploy-1.97.dev0/ezsmdeploy.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    19598 2023-07-25 19:09:48.000000 ezsmdeploy-1.97.dev0/ezsmdeploy.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      696 2023-07-25 19:09:48.000000 ezsmdeploy-1.97.dev0/ezsmdeploy.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-07-25 19:09:48.000000 ezsmdeploy-1.97.dev0/ezsmdeploy.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-07-18 17:33:24.000000 ezsmdeploy-1.97.dev0/ezsmdeploy.egg-info/not-zip-safe
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      129 2023-07-25 19:09:48.000000 ezsmdeploy-1.97.dev0/ezsmdeploy.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       11 2023-07-25 19:09:48.000000 ezsmdeploy-1.97.dev0/ezsmdeploy.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-07-25 19:09:48.675099 ezsmdeploy-1.97.dev0/setup.cfg
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1274 2023-07-25 19:09:10.000000 ezsmdeploy-1.97.dev0/setup.py
```

### Comparing `ezsmdeploy-1.96.dev0/PKG-INFO` & `ezsmdeploy-1.97.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezsmdeploy
-Version: 1.96.dev0
+Version: 1.97.dev0
 Summary: SageMaker custom deployments made easy
 Home-page: https://pypi.python.org/pypi/ezsmdeploy
 Author: Shreyas Subramanian
 Author-email: subshrey@amazon.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ezsmdeploy-1.96.dev0/README.rst` & `ezsmdeploy-1.97.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.96.dev0/ezsmdeploy/__init__.py` & `ezsmdeploy-1.97.dev0/ezsmdeploy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -653,15 +653,15 @@
                 wait=self.wait,
                 volume_size=volume_size,
                 data_capture_config=data_capture_config,
                 serverless_inference_config=self.serverless_config,
                 container_startup_health_check_timeout=300,
             )
 
-        self.endpoint_name = "ezsm-endpoint-" + self.name
+        self.endpoint_name = self.predictor.endpoint_name
 
     def get_size(self, bucket, path):
         s3 = boto3.resource("s3")
         my_bucket = s3.Bucket(bucket)
         total_size = 0.0
 
         for obj in my_bucket.objects.filter(Prefix=path):
```

### Comparing `ezsmdeploy-1.96.dev0/ezsmdeploy/data/Dockerfile` & `ezsmdeploy-1.97.dev0/ezsmdeploy/data/Dockerfile`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.96.dev0/ezsmdeploy/data/Dockerfile_flask` & `ezsmdeploy-1.97.dev0/ezsmdeploy/data/Dockerfile_flask`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.96.dev0/ezsmdeploy/data/build-docker.sh` & `ezsmdeploy-1.97.dev0/ezsmdeploy/data/build-docker.sh`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.96.dev0/ezsmdeploy/data/conversation.py` & `ezsmdeploy-1.97.dev0/ezsmdeploy/data/conversation.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.96.dev0/ezsmdeploy/data/cost.csv` & `ezsmdeploy-1.97.dev0/ezsmdeploy/data/cost.csv`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.96.dev0/ezsmdeploy/data/dockerd-entrypoint.py` & `ezsmdeploy-1.97.dev0/ezsmdeploy/data/dockerd-entrypoint.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.96.dev0/ezsmdeploy/data/instancetypes.csv` & `ezsmdeploy-1.97.dev0/ezsmdeploy/data/instancetypes.csv`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.96.dev0/ezsmdeploy/data/model_handler.py` & `ezsmdeploy-1.97.dev0/ezsmdeploy/data/model_handler.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.96.dev0/ezsmdeploy/data/nginx.conf` & `ezsmdeploy-1.97.dev0/ezsmdeploy/data/nginx.conf`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.96.dev0/ezsmdeploy/data/predictor.py` & `ezsmdeploy-1.97.dev0/ezsmdeploy/data/predictor.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.96.dev0/ezsmdeploy/data/serve` & `ezsmdeploy-1.97.dev0/ezsmdeploy/data/serve`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.96.dev0/ezsmdeploy/data/smlocust.py` & `ezsmdeploy-1.97.dev0/ezsmdeploy/data/smlocust.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.96.dev0/ezsmdeploy/modelscript_sklearn.py` & `ezsmdeploy-1.97.dev0/ezsmdeploy/modelscript_sklearn.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.96.dev0/ezsmdeploy.egg-info/PKG-INFO` & `ezsmdeploy-1.97.dev0/ezsmdeploy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezsmdeploy
-Version: 1.96.dev0
+Version: 1.97.dev0
 Summary: SageMaker custom deployments made easy
 Home-page: https://pypi.python.org/pypi/ezsmdeploy
 Author: Shreyas Subramanian
 Author-email: subshrey@amazon.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ezsmdeploy-1.96.dev0/ezsmdeploy.egg-info/SOURCES.txt` & `ezsmdeploy-1.97.dev0/ezsmdeploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.96.dev0/setup.py` & `ezsmdeploy-1.97.dev0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 extras = {
     'locust': [
         'locustio==0.14.5'
     ]
 }
 
 setup(name='ezsmdeploy',
-      version='1.96dev',
+      version='1.97dev',
       description='SageMaker custom deployments made easy',
       url='https://pypi.python.org/pypi/ezsmdeploy',
       #scripts=['Dockerfile','dockerd-entrypoint.py','model_handler.py','build-docker.sh'],
       author='Shreyas Subramanian',
       author_email='subshrey@amazon.com',
       license='MIT',
       packages=['ezsmdeploy'],
```

