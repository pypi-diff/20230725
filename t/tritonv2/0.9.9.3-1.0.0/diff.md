# Comparing `tmp/tritonv2-0.9.9.3.tar.gz` & `tmp/tritonv2-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tritonv2-0.9.9.3.tar", last modified: Thu Jul 13 11:51:57 2023, max compression
+gzip compressed data, was "tritonv2-1.0.0.tar", last modified: Tue Jul 25 06:59:59 2023, max compression
```

## Comparing `tritonv2-0.9.9.3.tar` & `tritonv2-1.0.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-13 11:51:57.104710 tritonv2-0.9.9.3/
--rw-r--r--   0 jojo       (501) staff       (20)     2410 2023-07-13 11:51:57.104819 tritonv2-0.9.9.3/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)     1884 2023-07-13 11:51:56.000000 tritonv2-0.9.9.3/README.md
--rw-r--r--   0 jojo       (501) staff       (20)      772 2023-07-13 11:51:57.105262 tritonv2-0.9.9.3/setup.cfg
--rw-r--r--   0 jojo       (501) staff       (20)      180 2023-07-13 11:51:56.000000 tritonv2-0.9.9.3/setup.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-13 11:51:57.103516 tritonv2-0.9.9.3/tritonv2/
--rw-r--r--   0 jojo       (501) staff       (20)      141 2023-04-12 08:56:34.000000 tritonv2-0.9.9.3/tritonv2/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)     1008 2023-06-06 13:39:44.000000 tritonv2-0.9.9.3/tritonv2/client.py
--rw-r--r--   0 jojo       (501) staff       (20)     6421 2023-06-06 13:39:44.000000 tritonv2-0.9.9.3/tritonv2/client_factory.py
--rw-r--r--   0 jojo       (501) staff       (20)     1300 2023-07-03 18:56:19.000000 tritonv2-0.9.9.3/tritonv2/constants.py
--rw-r--r--   0 jojo       (501) staff       (20)      259 2023-04-12 08:56:34.000000 tritonv2-0.9.9.3/tritonv2/exceptions.py
--rw-r--r--   0 jojo       (501) staff       (20)    17052 2023-06-06 13:39:44.000000 tritonv2-0.9.9.3/tritonv2/grpc_aio_client.py
--rw-r--r--   0 jojo       (501) staff       (20)    14424 2023-06-06 13:39:44.000000 tritonv2-0.9.9.3/tritonv2/grpc_client.py
--rw-r--r--   0 jojo       (501) staff       (20)     1880 2023-06-06 13:39:44.000000 tritonv2-0.9.9.3/tritonv2/grpc_interceptor.py
--rw-r--r--   0 jojo       (501) staff       (20)    31134 2023-07-10 12:07:32.000000 tritonv2-0.9.9.3/tritonv2/http_aio_client.py
--rw-r--r--   0 jojo       (501) staff       (20)    29615 2023-07-10 12:07:40.000000 tritonv2-0.9.9.3/tritonv2/http_client.py
--rw-r--r--   0 jojo       (501) staff       (20)     7608 2023-07-13 07:23:55.000000 tritonv2-0.9.9.3/tritonv2/model.py
--rw-r--r--   0 jojo       (501) staff       (20)     4162 2023-07-13 11:46:37.000000 tritonv2-0.9.9.3/tritonv2/model_config.py
--rw-r--r--   0 jojo       (501) staff       (20)      903 2023-07-04 11:53:39.000000 tritonv2-0.9.9.3/tritonv2/module.py
--rw-r--r--   0 jojo       (501) staff       (20)      180 2023-04-12 08:56:34.000000 tritonv2-0.9.9.3/tritonv2/setup.py
--rw-r--r--   0 jojo       (501) staff       (20)     4969 2023-07-13 11:51:28.000000 tritonv2-0.9.9.3/tritonv2/utils.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-13 11:51:57.104563 tritonv2-0.9.9.3/tritonv2.egg-info/
--rw-r--r--   0 jojo       (501) staff       (20)     2410 2023-07-13 11:51:57.000000 tritonv2-0.9.9.3/tritonv2.egg-info/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)      561 2023-07-13 11:51:57.000000 tritonv2-0.9.9.3/tritonv2.egg-info/SOURCES.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-07-13 11:51:57.000000 tritonv2-0.9.9.3/tritonv2.egg-info/dependency_links.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-07-13 11:51:57.000000 tritonv2-0.9.9.3/tritonv2.egg-info/not-zip-safe
--rw-r--r--   0 jojo       (501) staff       (20)      127 2023-07-13 11:51:57.000000 tritonv2-0.9.9.3/tritonv2.egg-info/requires.txt
--rw-r--r--   0 jojo       (501) staff       (20)        9 2023-07-13 11:51:57.000000 tritonv2-0.9.9.3/tritonv2.egg-info/top_level.txt
+drwxr-xr-x   0 light      (501) staff       (20)        0 2023-07-25 06:59:59.444038 tritonv2-1.0.0/
+-rw-r--r--   0 light      (501) staff       (20)     2386 2023-07-25 06:59:59.444105 tritonv2-1.0.0/PKG-INFO
+-rw-r--r--   0 light      (501) staff       (20)     1882 2023-07-25 06:59:59.000000 tritonv2-1.0.0/README.md
+-rw-r--r--   0 light      (501) staff       (20)      770 2023-07-25 06:59:59.444471 tritonv2-1.0.0/setup.cfg
+-rw-r--r--   0 light      (501) staff       (20)      180 2023-07-25 06:59:59.000000 tritonv2-1.0.0/setup.py
+drwxr-xr-x   0 light      (501) staff       (20)        0 2023-07-25 06:59:59.443165 tritonv2-1.0.0/tritonv2/
+-rw-r--r--   0 light      (501) staff       (20)      141 2023-07-24 12:33:31.000000 tritonv2-1.0.0/tritonv2/__init__.py
+-rw-r--r--   0 light      (501) staff       (20)     1008 2023-07-24 12:33:31.000000 tritonv2-1.0.0/tritonv2/client.py
+-rw-r--r--   0 light      (501) staff       (20)     6421 2023-07-24 12:33:31.000000 tritonv2-1.0.0/tritonv2/client_factory.py
+-rw-r--r--   0 light      (501) staff       (20)     1300 2023-07-24 12:33:31.000000 tritonv2-1.0.0/tritonv2/constants.py
+-rw-r--r--   0 light      (501) staff       (20)      259 2023-07-24 12:33:31.000000 tritonv2-1.0.0/tritonv2/exceptions.py
+-rw-r--r--   0 light      (501) staff       (20)    17055 2023-07-25 06:36:51.000000 tritonv2-1.0.0/tritonv2/grpc_aio_client.py
+-rw-r--r--   0 light      (501) staff       (20)    14427 2023-07-25 06:36:56.000000 tritonv2-1.0.0/tritonv2/grpc_client.py
+-rw-r--r--   0 light      (501) staff       (20)     1880 2023-07-24 12:33:31.000000 tritonv2-1.0.0/tritonv2/grpc_interceptor.py
+-rw-r--r--   0 light      (501) staff       (20)    31137 2023-07-25 06:37:00.000000 tritonv2-1.0.0/tritonv2/http_aio_client.py
+-rw-r--r--   0 light      (501) staff       (20)    29618 2023-07-25 06:36:26.000000 tritonv2-1.0.0/tritonv2/http_client.py
+-rw-r--r--   0 light      (501) staff       (20)     7608 2023-07-24 12:33:31.000000 tritonv2-1.0.0/tritonv2/model.py
+-rw-r--r--   0 light      (501) staff       (20)     4162 2023-07-24 12:33:31.000000 tritonv2-1.0.0/tritonv2/model_config.py
+-rw-r--r--   0 light      (501) staff       (20)      903 2023-07-24 12:33:31.000000 tritonv2-1.0.0/tritonv2/module.py
+-rw-r--r--   0 light      (501) staff       (20)      180 2023-07-24 12:33:31.000000 tritonv2-1.0.0/tritonv2/setup.py
+-rw-r--r--   0 light      (501) staff       (20)     4969 2023-07-24 12:33:31.000000 tritonv2-1.0.0/tritonv2/utils.py
+drwxr-xr-x   0 light      (501) staff       (20)        0 2023-07-25 06:59:59.443930 tritonv2-1.0.0/tritonv2.egg-info/
+-rw-r--r--   0 light      (501) staff       (20)     2386 2023-07-25 06:59:59.000000 tritonv2-1.0.0/tritonv2.egg-info/PKG-INFO
+-rw-r--r--   0 light      (501) staff       (20)      561 2023-07-25 06:59:59.000000 tritonv2-1.0.0/tritonv2.egg-info/SOURCES.txt
+-rw-r--r--   0 light      (501) staff       (20)        1 2023-07-25 06:59:59.000000 tritonv2-1.0.0/tritonv2.egg-info/dependency_links.txt
+-rw-r--r--   0 light      (501) staff       (20)        1 2023-07-25 06:59:59.000000 tritonv2-1.0.0/tritonv2.egg-info/not-zip-safe
+-rw-r--r--   0 light      (501) staff       (20)      127 2023-07-25 06:59:59.000000 tritonv2-1.0.0/tritonv2.egg-info/requires.txt
+-rw-r--r--   0 light      (501) staff       (20)        9 2023-07-25 06:59:59.000000 tritonv2-1.0.0/tritonv2.egg-info/top_level.txt
```

### Comparing `tritonv2-0.9.9.3/PKG-INFO` & `tritonv2-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: tritonv2
-Version: 0.9.9.3
+Version: 1.0.0
 Summary: project descriptions here
 Home-page: https://github.com/FlyTOmeLight
 Author: zhoubohan
 Author-email: zhoubohan.pro@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # tritonv2
 A client library for promote triton official client
 
 ## Installation
 
 ```bash
-pip install tritonv2==0.9.9.3
+pip install tritonv2==1.0.0
 ```
 
 ## Usage
 
 First, you need to create a client object.
 
 ```python
@@ -101,9 +100,7 @@
 ```python
 client.trace_setting()
 client.get_trace_settings()
 ```
 
 
 
-
-
```

### Comparing `tritonv2-0.9.9.3/README.md` & `tritonv2-1.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # tritonv2
 A client library for promote triton official client
 
 ## Installation
 
 ```bash
-pip install tritonv2==0.9.9.3
+pip install tritonv2==1.0.0
 ```
 
 ## Usage
 
 First, you need to create a client object.
 
 ```python
```

### Comparing `tritonv2-0.9.9.3/setup.cfg` & `tritonv2-1.0.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = tritonv2
 author = zhoubohan
 author_email = zhoubohan.pro@gmail.com
-version = 0.9.9.3
+version = 1.0.0
 description = project descriptions here
 long_description = file: README.md
 long_description_content_type = text/markdown
 home_page = https://github.com/FlyTOmeLight
 license = MIT
 classifier = 
 	Programming Language :: Python
```

### Comparing `tritonv2-0.9.9.3/tritonv2/client.py` & `tritonv2-1.0.0/tritonv2/client.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.9.3/tritonv2/client_factory.py` & `tritonv2-1.0.0/tritonv2/client_factory.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.9.3/tritonv2/constants.py` & `tritonv2-1.0.0/tritonv2/constants.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.9.3/tritonv2/grpc_aio_client.py` & `tritonv2-1.0.0/tritonv2/grpc_aio_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -437,15 +437,15 @@
                                             timeout=timeout,
                                             client_timeout=client_timeout,
                                             headers=headers,
                                             compression_algorithm=compression_algorithm)
         except Exception as e:
             raise TritonClientException('Failed to model infer: {}'.format(e)) from None
 
-    async def get_inputs_and_outputs_detail(self, model_name, model_version):
+    async def get_inputs_and_outputs_detail(self, model_name, model_version=""):
         """
         get inputs and outputs detail
         :param model_name:
         :param model_version:
         :return:
         """
         try:
```

### Comparing `tritonv2-0.9.9.3/tritonv2/grpc_client.py` & `tritonv2-1.0.0/tritonv2/grpc_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -373,15 +373,15 @@
         try:
             return self._client.get_trace_settings(model_name=model_name,
                                                    headers=headers,
                                                    as_json=True)
         except Exception as e:
             raise TritonClientException('Failed to get trace settings: {}'.format(e)) from None
 
-    def get_inputs_and_outputs_detail(self, model_name, model_version):
+    def get_inputs_and_outputs_detail(self, model_name, model_version=""):
         """
         get inputs and outputs detail
         :param model_name:
         :param model_version:
         :return:
         """
         try:
```

### Comparing `tritonv2-0.9.9.3/tritonv2/grpc_interceptor.py` & `tritonv2-1.0.0/tritonv2/grpc_interceptor.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.9.3/tritonv2/http_aio_client.py` & `tritonv2-1.0.0/tritonv2/http_aio_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -625,15 +625,15 @@
             return await self._client.get_trace_settings(model_name=model_name,
                                                          headers=headers,
                                                          query_params=query_params)
         except Exception as e:
             raise TritonClientException(
                 'Failed to get trace settings: {}'.format(e)) from None
 
-    async def get_inputs_and_outputs_detail(self, model_name, model_version):
+    async def get_inputs_and_outputs_detail(self, model_name, model_version=""):
         """
         get inputs and outputs detail
         :param model_name:
         :param model_version:
         :return:
         """
         try:
```

### Comparing `tritonv2-0.9.9.3/tritonv2/http_client.py` & `tritonv2-1.0.0/tritonv2/http_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -612,15 +612,15 @@
                 return self._client.get_trace_settings(model_name=model_name,
                                                        headers=headers,
                                                        query_params=query_params)
         except Exception as e:
             raise TritonClientException(
                 'Failed to get trace settings: {}'.format(e)) from None
 
-    def get_inputs_and_outputs_detail(self, model_name, model_version):
+    def get_inputs_and_outputs_detail(self, model_name, model_version=""):
         """
         get inputs and outputs detail
         :param model_name:
         :param model_version:
         :return:
         """
         try:
```

### Comparing `tritonv2-0.9.9.3/tritonv2/model.py` & `tritonv2-1.0.0/tritonv2/model.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.9.3/tritonv2/model_config.py` & `tritonv2-1.0.0/tritonv2/model_config.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.9.3/tritonv2/module.py` & `tritonv2-1.0.0/tritonv2/module.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.9.3/tritonv2/utils.py` & `tritonv2-1.0.0/tritonv2/utils.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.9.3/tritonv2.egg-info/PKG-INFO` & `tritonv2-1.0.0/tritonv2.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: tritonv2
-Version: 0.9.9.3
+Version: 1.0.0
 Summary: project descriptions here
 Home-page: https://github.com/FlyTOmeLight
 Author: zhoubohan
 Author-email: zhoubohan.pro@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # tritonv2
 A client library for promote triton official client
 
 ## Installation
 
 ```bash
-pip install tritonv2==0.9.9.3
+pip install tritonv2==1.0.0
 ```
 
 ## Usage
 
 First, you need to create a client object.
 
 ```python
@@ -101,9 +100,7 @@
 ```python
 client.trace_setting()
 client.get_trace_settings()
 ```
 
 
 
-
-
```

### Comparing `tritonv2-0.9.9.3/tritonv2.egg-info/SOURCES.txt` & `tritonv2-1.0.0/tritonv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

