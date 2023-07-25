# Comparing `tmp/arthub_api-1.7.1.tar.gz` & `tmp/arthub_api-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arthub_api-1.7.1.tar", last modified: Tue Jun 27 05:41:54 2023, max compression
+gzip compressed data, was "arthub_api-1.8.0.tar", last modified: Tue Jul 25 13:49:18 2023, max compression
```

## Comparing `arthub_api-1.7.1.tar` & `arthub_api-1.8.0.tar`

### file list

```diff
@@ -1,41 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 05:41:54.811816 arthub_api-1.7.1/
--rw-rw-rw-   0        0        0     1077 2022-09-05 10:15:53.000000 arthub_api-1.7.1/LICENSE
--rw-rw-rw-   0        0        0      107 2022-09-05 10:15:53.000000 arthub_api-1.7.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1412 2023-06-27 05:41:54.811299 arthub_api-1.7.1/PKG-INFO
--rw-rw-rw-   0        0        0      864 2023-05-19 06:20:15.000000 arthub_api-1.7.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 05:41:54.787441 arthub_api-1.7.1/arthub_api/
--rw-rw-rw-   0        0        0      675 2023-05-22 10:07:06.000000 arthub_api-1.7.1/arthub_api/__init__.py
--rw-rw-rw-   0        0        0     3730 2023-05-22 10:07:06.000000 arthub_api-1.7.1/arthub_api/__main__.py
--rw-rw-rw-   0        0        0      241 2023-06-27 05:41:04.000000 arthub_api-1.7.1/arthub_api/__version__.py
--rw-rw-rw-   0        0        0    13661 2023-05-11 11:13:51.000000 arthub_api-1.7.1/arthub_api/_internal_utils.py
--rw-rw-rw-   0        0        0      104 2023-06-01 06:49:45.000000 arthub_api-1.7.1/arthub_api/arthub_api_config.py
--rw-rw-rw-   0        0        0      501 2023-05-22 10:07:06.000000 arthub_api-1.7.1/arthub_api/asset_matrix.py
--rw-rw-rw-   0        0        0    43536 2023-05-22 10:07:06.000000 arthub_api-1.7.1/arthub_api/blade_api.py
--rw-rw-rw-   0        0        0     2070 2023-05-31 13:05:30.000000 arthub_api-1.7.1/arthub_api/blade_api_instance.py
--rw-rw-rw-   0        0        0    28363 2023-05-31 13:05:30.000000 arthub_api-1.7.1/arthub_api/blade_storage.py
--rw-rw-rw-   0        0        0       22 2023-02-08 16:32:42.000000 arthub_api-1.7.1/arthub_api/cli.py
--rw-rw-rw-   0        0        0     1443 2023-05-23 10:45:39.000000 arthub_api-1.7.1/arthub_api/config.py
--rw-rw-rw-   0        0        0      523 2023-02-08 16:32:42.000000 arthub_api-1.7.1/arthub_api/exception.py
--rw-rw-rw-   0        0        0     1258 2023-03-14 10:50:34.000000 arthub_api-1.7.1/arthub_api/models.py
--rw-rw-rw-   0        0        0    42924 2023-05-23 10:45:39.000000 arthub_api-1.7.1/arthub_api/open_api.py
--rw-rw-rw-   0        0        0    41836 2023-05-22 10:07:06.000000 arthub_api-1.7.1/arthub_api/storage.py
--rw-rw-rw-   0        0        0     9100 2023-05-23 10:45:39.000000 arthub_api-1.7.1/arthub_api/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 05:41:54.798090 arthub_api-1.7.1/arthub_api.egg-info/
--rw-rw-rw-   0        0        0     1412 2023-06-27 05:41:54.000000 arthub_api-1.7.1/arthub_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      847 2023-06-27 05:41:54.000000 arthub_api-1.7.1/arthub_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 05:41:54.000000 arthub_api-1.7.1/arthub_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-27 05:41:54.000000 arthub_api-1.7.1/arthub_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-02-09 14:04:12.000000 arthub_api-1.7.1/arthub_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      116 2023-06-27 05:41:54.000000 arthub_api-1.7.1/arthub_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-27 05:41:54.000000 arthub_api-1.7.1/arthub_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       63 2022-09-26 03:28:18.000000 arthub_api-1.7.1/requirements-dev.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 05:41:54.812330 arthub_api-1.7.1/setup.cfg
--rw-rw-rw-   0        0        0     3087 2023-06-27 05:38:53.000000 arthub_api-1.7.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 05:41:54.809232 arthub_api-1.7.1/tests/
--rw-rw-rw-   0        0        0      176 2023-05-22 10:07:06.000000 arthub_api-1.7.1/tests/__init__.py
--rw-rw-rw-   0        0        0      108 2023-05-19 06:20:15.000000 arthub_api-1.7.1/tests/_utils.py
--rw-rw-rw-   0        0        0      280 2023-05-19 06:20:15.000000 arthub_api-1.7.1/tests/conftest.py
--rw-rw-rw-   0        0        0     6110 2023-05-19 06:20:15.000000 arthub_api-1.7.1/tests/test_open_api.py
--rw-rw-rw-   0        0        0    18818 2023-06-06 02:42:34.000000 arthub_api-1.7.1/tests/test_open_api_blade.py
--rw-rw-rw-   0        0        0     3647 2023-05-19 06:20:15.000000 arthub_api-1.7.1/tests/test_storage.py
--rw-rw-rw-   0        0        0     8450 2023-05-23 10:45:39.000000 arthub_api-1.7.1/tests/test_storage_blade.py
+drwxrwxrwx   0        0        0        0 2023-07-25 13:49:18.336596 arthub_api-1.8.0/
+-rw-rw-rw-   0        0        0     1077 2022-09-05 10:15:53.000000 arthub_api-1.8.0/LICENSE
+-rw-rw-rw-   0        0        0      107 2022-09-05 10:15:53.000000 arthub_api-1.8.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1412 2023-07-25 13:49:18.335605 arthub_api-1.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0      864 2023-05-19 06:20:15.000000 arthub_api-1.8.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 13:49:18.313408 arthub_api-1.8.0/arthub_api/
+-rw-rw-rw-   0        0        0      675 2023-07-25 13:45:45.000000 arthub_api-1.8.0/arthub_api/__init__.py
+-rw-rw-rw-   0        0        0     3730 2023-07-25 13:45:45.000000 arthub_api-1.8.0/arthub_api/__main__.py
+-rw-rw-rw-   0        0        0      241 2023-07-25 13:47:27.000000 arthub_api-1.8.0/arthub_api/__version__.py
+-rw-rw-rw-   0        0        0    13661 2023-05-11 11:13:51.000000 arthub_api-1.8.0/arthub_api/_internal_utils.py
+-rw-rw-rw-   0        0        0      104 2023-07-25 13:45:45.000000 arthub_api-1.8.0/arthub_api/arthub_api_config.py
+-rw-rw-rw-   0        0        0      501 2023-07-25 13:45:45.000000 arthub_api-1.8.0/arthub_api/asset_matrix.py
+-rw-rw-rw-   0        0        0    43536 2023-07-25 13:45:45.000000 arthub_api-1.8.0/arthub_api/blade_api.py
+-rw-rw-rw-   0        0        0     2072 2023-07-25 13:45:45.000000 arthub_api-1.8.0/arthub_api/blade_api_instance.py
+-rw-rw-rw-   0        0        0    28990 2023-07-25 13:45:45.000000 arthub_api-1.8.0/arthub_api/blade_storage.py
+-rw-rw-rw-   0        0        0       22 2023-02-08 16:32:42.000000 arthub_api-1.8.0/arthub_api/cli.py
+-rw-rw-rw-   0        0        0     1443 2023-07-25 13:45:45.000000 arthub_api-1.8.0/arthub_api/config.py
+-rw-rw-rw-   0        0        0      523 2023-02-08 16:32:42.000000 arthub_api-1.8.0/arthub_api/exception.py
+-rw-rw-rw-   0        0        0     1258 2023-03-14 10:50:34.000000 arthub_api-1.8.0/arthub_api/models.py
+-rw-rw-rw-   0        0        0    44124 2023-07-25 13:45:45.000000 arthub_api-1.8.0/arthub_api/open_api.py
+-rw-rw-rw-   0        0        0    41836 2023-07-25 13:45:45.000000 arthub_api-1.8.0/arthub_api/storage.py
+-rw-rw-rw-   0        0        0     9102 2023-07-25 13:45:45.000000 arthub_api-1.8.0/arthub_api/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 13:49:18.324935 arthub_api-1.8.0/arthub_api.egg-info/
+-rw-rw-rw-   0        0        0     1412 2023-07-25 13:49:17.000000 arthub_api-1.8.0/arthub_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      790 2023-07-25 13:49:17.000000 arthub_api-1.8.0/arthub_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 13:49:17.000000 arthub_api-1.8.0/arthub_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-07-25 13:49:17.000000 arthub_api-1.8.0/arthub_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-02-09 14:04:12.000000 arthub_api-1.8.0/arthub_api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      116 2023-07-25 13:49:17.000000 arthub_api-1.8.0/arthub_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-25 13:49:17.000000 arthub_api-1.8.0/arthub_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       63 2022-09-26 03:28:18.000000 arthub_api-1.8.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 13:49:18.336596 arthub_api-1.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     3087 2023-07-25 13:45:45.000000 arthub_api-1.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 13:49:18.332912 arthub_api-1.8.0/tests/
+-rw-rw-rw-   0        0        0      176 2023-07-25 13:45:45.000000 arthub_api-1.8.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      108 2023-05-19 06:20:15.000000 arthub_api-1.8.0/tests/_utils.py
+-rw-rw-rw-   0        0        0      735 2023-07-25 13:45:45.000000 arthub_api-1.8.0/tests/conftest.py
+-rw-rw-rw-   0        0        0     6646 2023-07-25 13:45:45.000000 arthub_api-1.8.0/tests/test_open_api.py
+-rw-rw-rw-   0        0        0     2979 2023-07-25 13:45:45.000000 arthub_api-1.8.0/tests/test_storage.py
```

### Comparing `arthub_api-1.7.1/LICENSE` & `arthub_api-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arthub_api-1.7.1/PKG-INFO` & `arthub_api-1.8.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arthub_api
-Version: 1.7.1
+Version: 1.8.0
 Summary: ArHhub Python SDK
 Home-page: UNKNOWN
 Author: Joey Ding
 Author-email: joeyding@tencent.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arthub_api-1.7.1/README.md` & `arthub_api-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `arthub_api-1.7.1/arthub_api/__init__.py` & `arthub_api-1.8.0/arthub_api/__init__.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.7.1/arthub_api/__main__.py` & `arthub_api-1.8.0/arthub_api/__main__.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.7.1/arthub_api/_internal_utils.py` & `arthub_api-1.8.0/arthub_api/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.7.1/arthub_api/blade_api.py` & `arthub_api-1.8.0/arthub_api/blade_api.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.7.1/arthub_api/blade_api_instance.py` & `arthub_api-1.8.0/arthub_api/blade_api_instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class BladeInstance(object):
     """Global instance initializer for BladeAPI client."""
     @classmethod
     def blade_root_id(cls):
         global blade_root_id
         if blade_root_id is None:
-            res = cls.backend.blade_get_root_id()
+            res = cls.backend().blade_get_root_id()
             res.raise_for_err(res)
             root_id = res.result
             if root_id == 0:
                 raise APIError("cannot get root id, result is 0")
             blade_root_id = root_id
         return blade_root_id
```

### Comparing `arthub_api-1.7.1/arthub_api/blade_storage.py` & `arthub_api-1.8.0/arthub_api/blade_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,59 +284,75 @@
         self.file_size = file_size
         self.download_url = None
         self.expired = 600
         self.timeout = timeout
         self.url_expire_time = None
         self.tmp_file = '{0}_ahtmp'.format(local_path)
         self.record_file = '{0}_dl_ahrecord'.format(local_path)
+        self.lock = threading.Lock()
 
     def _refresh_download_url(self):
         current_time = time.time()
         if self.download_url is None or current_time >= self.url_expire_time:
             self.download_url = self.remote_signer.get_download_url(self.bucket, self.key, self.expired)
             self.url_expire_time = current_time + self.expired - 20  # 10 minutes expiry time
 
     def _load_progress(self):
-        if os.path.exists(self.record_file):
-            with open(self.record_file, 'r') as f:
-                return [tuple(map(int, line.strip().split('-'))) for line in f]
-        return []
+        res = []
+        try:
+            if os.path.exists(self.record_file):
+                with open(self.record_file, 'r') as f:
+                    res = [tuple(map(int, line.strip().split('-'))) for line in f]
+        except:
+            logger.error("cannot load progress file, treat as new download")
+        finally:
+            return res
 
     def _save_progress(self, start, end):
-        with threading.Lock():  
+        with self.lock:
             with open(self.record_file, 'a') as f:
                 f.write('{start}-{end}-{part_size}\n'.format(start=start, end=end, part_size=self.part_size))  # Save part_size along with the progress, part_size is not current chunk_length
 
     def _download_part(self, start, end):
         self._refresh_download_url()
         headers = {'Range': 'bytes={start}-{end}'.format(start=start, end=end)}
         try:
             response = requests.get(self.download_url, headers=headers, stream=True, timeout=self.timeout)
         except Exception as e:
             raise COSHttpError("error with requests {0}".format(e))
+        response.raise_for_status()
+        expected_len = end - start + 1
+        real_len = 0
         with open(self.tmp_file, 'rb+') as f:
             f.seek(start)
             for chunk in response.iter_content(chunk_size=8192):
                 f.write(chunk)
+                real_len += len(chunk)
                 if self.progress_callback:
                     self.progress_callback.report(len(chunk))
+        if real_len != expected_len:
+            raise IOError("download part length is not expected")
         self._save_progress(start, end)  # Save progress after part is downloaded
 
     def simple_download(self):
         self._refresh_download_url()
         try:
             response = requests.get(self.download_url, stream=True, timeout=self.timeout)
         except Exception as e:
             raise COSHttpError("error with requests {0}".format(e))
         response.raise_for_status()
+        real_len = 0
         with open(self.tmp_file, 'wb') as f:
             for chunk in response.iter_content(chunk_size=8192):
                 f.write(chunk)
+                real_len += len(chunk)
                 if self.progress_callback:
                     self.progress_callback.report(len(chunk))
+        if real_len != self.file_size:
+            raise IOError("download length is not expected")
         try:
             os.remove(self.local_path)
         except:
             pass
         os.rename(self.tmp_file, self.local_path)
         if os.path.exists(self.record_file):  # Remove existing progress record file
             os.remove(self.record_file)
@@ -400,14 +416,15 @@
         self.thread_num = thread_num
         self.progress_callback = progress_callback
         self.file_size = file_size
         self.upload_url = None
         self.url_expire_time = None
         self.timeout = timeout
         self.record_file = '{0}_ul_ahrecord'.format(local_path)
+        self.lock = threading.Lock()
         
     def _begin_multipart_upload(self, bucket, key, file_name):
         begin_url = self.remote_signer.get_begin_multipart_upload_url(bucket, key)
         # req
         try:
             res = requests.post(begin_url,
                                 headers={"content-type": _internal_utils.get_content_type_from_file_name(file_name)}, timeout=self.timeout)
@@ -490,15 +507,15 @@
                     os.remove(self.record_file)
                     parts = []
                     etags = []
                     break
         return parts, etags, final_upload_id
 
     def _save_progress(self, start, end, upload_id, part_number, etag):
-        with threading.Lock():  
+        with self.lock:
             with open(self.record_file, 'a') as f:
                 line = json.dumps({"start":start, "end":end, "part_size":self.part_size, "upload_id":upload_id, "part_number":part_number, "etag":etag })
                 f.write("{0}\n".format(line))
 
     def simple_upload(self):
         if os.path.exists(self.record_file):  # Remove existing progress record file
             os.remove(self.record_file)
```

### Comparing `arthub_api-1.7.1/arthub_api/config.py` & `arthub_api-1.8.0/arthub_api/config.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.7.1/arthub_api/exception.py` & `arthub_api-1.8.0/arthub_api/exception.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.7.1/arthub_api/models.py` & `arthub_api-1.8.0/arthub_api/models.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.7.1/arthub_api/open_api.py` & `arthub_api-1.8.0/arthub_api/open_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from . import models
 from . import _internal_utils
 from . import exception
 from xml.etree import ElementTree
 from . import arthub_api_config
 from .config import api_config_oa
 from .utils import get_config_by_name, logger
+import os
 
 
 def _node_query_metas(simplified_meta=True):
     metas = [
         "name",
         "file_format",
         "node_type",
@@ -260,15 +261,18 @@
                 raise NotLoginError("authentication failed")
             if res.is_no_permission():
                 raise NoPermissionError("no permission")
             raise APIError("err from api {0}".format(res.api_error_message))
 
 
 class OpenAPI(object):
-    def __init__(self, config=api_config_oa, get_token_from_cache=True, api_config_name=None):
+    def __init__(self, config=api_config_oa,
+                 get_token_from_cache=True,
+                 api_config_name=None,
+                 apply_blade_env=True):
         r"""Used to call ArtHub openapi.
         for detailed interface doc: "https://arthub.qq.com/user_manual/index.html"
 
         :param config: from arthub_api.config.
         :param get_token_from_cache: read token from local cache.
         """
         if api_config_name:
@@ -279,30 +283,38 @@
         self._cookies = None
         self._api_version_depot = "v2"
         self._api_version_gateway = "v2"
         self._api_version_account = "v3"
         self._cached_account_name = ""
         self._cached_password = ""
         self._auto_login = False
+        self._current_account_info = None
+        self._in_blade_env = False
+        if apply_blade_env:
+            self._apply_blade_env_value()
         if get_token_from_cache:
             self.get_token_from_cache()
-            
+
     @contextmanager
     def switch_config(self, api_config_name, get_token_from_cache):
         config = get_config_by_name(api_config_name, api_config_oa)
         old__dict = copy.copy(self.__dict__)
         self.__dict__ = OpenAPI(config, get_token_from_cache).__dict__.copy()
         yield
         self.__dict__ = old__dict
 
     @property
     def config(self):
         return self._config
 
     @property
+    def in_blade_env(self):
+        return self._in_blade_env
+
+    @property
     def api_host(self):
         if self.config:
             return self.config["host"]
         return ""
 
     @property
     def http_scheme(self):
@@ -442,29 +454,38 @@
         if self._public_token:
             headers["publictoken"] = self._public_token
         headers["content-type"] = content_type
         self.add_headers(headers)
 
         # send request
         try:
-            res = requests.request(method=method, url=url, headers=headers, json=data, cookies=self._cookies, timeout=self.timeout)
+            res = requests.request(method=method, url=url, headers=headers, json=data, cookies=self._cookies,
+                                   timeout=self.timeout)
         except Exception as e:
             logger.error("[API] send request \"%s\" exception: %s" % (url, e))
             response = APIResponse(None, True)
             response.exception = e
             return response
 
         response = APIResponse(res)
         if response.is_api_authentication_failed() and try_login_on_expired:
             # Try to log in again due to authentication failure
             if self._try_auto_login():
                 response = self._make_api_request(url, data, method, content_type, try_login_on_expired=False)
 
         return response
 
+    def _apply_blade_env_value(self):
+        network_type = os.environ.get("BLADE_NETWORK_TYPE")
+        if not network_type:
+            return
+        self._in_blade_env = True
+        self._config = get_config_by_name(network_type, self._config)
+        self._cookies = os.environ.get("BLADE_API_COOKIES")
+
     def add_headers(self, headers):
         pass
 
     def login(self, account_name, password, set_auto_login=True, save_token_to_cache=True):
         r"""Login by email/mobile and password. You can visit https://arthub.qq.com to register.
 
         :param account_name: str. email or mobile.
@@ -495,57 +516,83 @@
             # save account and password for auto login
             if set_auto_login:
                 self._cached_account_name = account_name
                 self._cached_password = password
 
         return res
 
-    def get_account_email(self):
-        r"""Get the email of the log-in account.
+    def _account_value(self, key):
+        account_info = self.current_account_info
+        if account_info:
+            return account_info.get(key)
 
+    def get_account_email(self):
+        r"""
         :rtype: str or None. Example: "XXX@tencent.com".
         """
 
-        res = self.get_account_detail()
-        if not res.is_succeeded():
-            return None
-        return res.first_result("email")
+        return self._account_value("email")
 
     def get_account_icon_url(self):
-        r"""Get the icon url of the log-in account.
-
+        r"""
         :rtype: str or None.
         """
 
-        res = self.get_account_detail()
-        if not res.is_succeeded():
-            return None
-        return res.first_result("icon_url")
+        return self._account_value("icon_url")
 
     def get_account_company(self):
-        r"""Get the company of the log-in account.
-
+        r"""
         :rtype: str or None.
         """
 
-        res = self.get_account_detail()
-        if not res.is_succeeded():
-            return None
-        return res.first_result("company")
+        return self._account_value("company")
 
     def get_account_department(self):
-        r"""Get the department of the log-in account.
+        r"""
+        :rtype: str or None.
+        """
+
+        return self._account_value("department")
+
+    def get_account_nick_name(self):
+        r"""
+        :rtype: str or None.
+        """
+
+        return self._account_value("nick_name")
+
+    def get_account_qywx_alias(self):
+        r"""
+        :rtype: str or None.
+        """
+
+        return self._account_value("qywx_alias")
 
+    def get_account_qywx_name(self):
+        r"""
         :rtype: str or None.
         """
 
+        return self._account_value("qywx_name")
+
+    def get_account_phone(self):
+        r"""
+        :rtype: str or None.
+        """
+
+        return self._account_value("phone")
+
+    @property
+    def current_account_info(self):
+        if self._current_account_info is not None:
+            return self._current_account_info
         res = self.get_account_detail()
-        if not res.is_succeeded():
-            return None
-        return res.first_result("department")
+        if res.is_succeeded():
+            self._current_account_info = res.first_result()
+        return self._current_account_info
 
     def get_account_detail(self, account_name=[]):
         r"""Get the detail of user's account.
 
         :param account_name: list. Example: ["joey"].
         :rtype: arthub_api.APIResponse
         """
@@ -560,15 +607,15 @@
 
         :rtype: bool
         """
 
         if self._token == "" and self._public_token == "" and self._cookies is None:
             return False
 
-        return self.get_account_detail().is_succeeded()
+        return bool(self.current_account_info)
 
     def get_ticket(self):
         r"""Get the ticket to request websocket.
 
         :rtype: arthub_api.APIResponse
         """
 
@@ -735,15 +782,16 @@
         signed_url = api_res.direct_result
         origin_url = api_res.first_result()["origin_url"]
         logger.info("[API] get begin multipart upload signed url: %s" % signed_url)
 
         # send signature url
         try:
             res = requests.post(signed_url,
-                                headers={"content-type": _internal_utils.get_content_type_from_file_name(file_name)}, timeout=self.timeout)
+                                headers={"content-type": _internal_utils.get_content_type_from_file_name(file_name)},
+                                timeout=self.timeout)
         except Exception as e:
             error_message = "request S3 multipart by url %s upload id exception: %s" % (signed_url, e)
             logger.error("[API] %s" % error_message)
             return models.failure_result(error_message)
 
         if not res or not res.ok:
             error_message = "request S3 multipart upload id failed, url: %s, code: %d" % (signed_url, res.status_code)
```

### Comparing `arthub_api-1.7.1/arthub_api/storage.py` & `arthub_api-1.8.0/arthub_api/storage.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.7.1/arthub_api/utils.py` & `arthub_api-1.8.0/arthub_api/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,7 +305,8 @@
     }
     c = _env_map.get(env)
     if not c:
         if default_config:
             return default_config
         return api_config_oa
     return c
+
```

### Comparing `arthub_api-1.7.1/arthub_api.egg-info/PKG-INFO` & `arthub_api-1.8.0/arthub_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arthub-api
-Version: 1.7.1
+Version: 1.8.0
 Summary: ArHhub Python SDK
 Home-page: UNKNOWN
 Author: Joey Ding
 Author-email: joeyding@tencent.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arthub_api-1.7.1/arthub_api.egg-info/SOURCES.txt` & `arthub_api-1.8.0/arthub_api.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -26,10 +26,8 @@
 arthub_api.egg-info/not-zip-safe
 arthub_api.egg-info/requires.txt
 arthub_api.egg-info/top_level.txt
 tests/__init__.py
 tests/_utils.py
 tests/conftest.py
 tests/test_open_api.py
-tests/test_open_api_blade.py
-tests/test_storage.py
-tests/test_storage_blade.py
+tests/test_storage.py
```

### Comparing `arthub_api-1.7.1/setup.py` & `arthub_api-1.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.7.1/tests/test_open_api.py` & `arthub_api-1.8.0/tests/test_open_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,79 +1,92 @@
-import arthub_api
-import pytest
 import logging
-from arthub_api import arthub_api_config
-from . import _utils
-from arthub_api import (
-    OpenAPI,
-    utils
-)
+import os
+from arthub_api import utils
+from arthub_api import OpenAPI
+from arthub_api import api_config_oa_test
+from contextlib import contextmanager
 
 TEST_DEPOT_NAME = "apg"
 
-open_api = None
-
 
 def on_api_failed(res):
     logging.error("[TEST][API] \"%s\" failed, error: %s" % (res.url, res.error_message()))
 
 
-@pytest.mark.run(order=1)
-def test_init(env):
-    global open_api
-    _c = _utils.get_config(env)
-    open_api = OpenAPI(_c, False)
-    res = open_api.login(arthub_api_config.account_email, arthub_api_config.password)
-    if not res.is_succeeded():
-        on_api_failed(res)
-        pytest.exit("login failed, exit test", returncode=1)
-
-    logging.info("[TEST][API] \"%s\" success, token: %s" % (res.url, res.results.get(0)["arthub_token"]))
+@contextmanager
+def set_env_var(name, value):
+    original_value = os.environ.get(name)
+    os.environ[name] = value
+    try:
+        yield
+    finally:
+        if original_value is None:
+            del os.environ[name]
+        else:
+            os.environ[name] = original_value
+
+
+def test_blade_env():
+    with set_env_var("BLADE_NETWORK_TYPE", "oa_test"):
+        open_api = OpenAPI(apply_blade_env=True)
+        assert open_api.config == api_config_oa_test
+
+
+def test_account(open_api):
+    assert open_api.is_login()
+    assert open_api.get_account_phone()
+    assert open_api.get_account_qywx_name()
+    assert open_api.get_account_qywx_alias()
+    assert open_api.get_account_nick_name()
+    assert open_api.get_account_department()
+    assert open_api.get_account_company()
+    assert open_api.get_account_icon_url()
+    assert open_api.get_account_email()
 
 
-def test_depot_get_root_id():
+def test_depot_get_root_id(open_api):
     res = open_api.depot_get_root_id(TEST_DEPOT_NAME)
     if not res.is_succeeded():
         on_api_failed(res)
         assert 0
 
     logging.info("[TEST][API] \"%s\" success, depot id: %d" % (res.url, res.results.get(0)))
 
 
-def test_depot_get_node_brief_by_ids():
+def test_depot_get_node_brief_by_ids(open_api):
     res = open_api.depot_get_node_brief_by_ids(TEST_DEPOT_NAME, [120347220059298, 120347220059299])
     if not res.is_succeeded():
         on_api_failed(res)
         assert 0
 
     node_1 = res.results.get(0)
     node_2 = res.results.get(1)
     logging.info("[TEST][API] \"%s\" success, name_1: %s, name_2: %s" % (res.url, node_1["name"], node_2["name"]))
 
 
-def test_depot_get_child_node_count():
+def test_depot_get_child_node_count(open_api):
     res = open_api.depot_get_child_node_count(TEST_DEPOT_NAME, [120347220059339])
     if not res.is_succeeded():
         on_api_failed(res)
         assert 0
 
     logging.info("[TEST][API] \"%s\" success, count: %d" % (res.url, res.results.get(0)["count"]))
 
 
-def test_depot_get_download_signature():
+def test_depot_get_download_signature(open_api):
     res = open_api.depot_get_download_signature(TEST_DEPOT_NAME,
                                                 nodes=[{"object_id": 120347220059338, "object_meta": "origin_url"}])
     if not res.is_succeeded():
         on_api_failed(res)
         assert 0
 
     logging.info("[TEST][API] \"%s\" success, signed url: %s" % (res.url, res.results.get(0)["signed_url"]))
 
 
-def test_depot_get_upload_signature():
+def test_depot_get_upload_signature(open_api):
     file_name = "new_asset_to_upload"
     res_0 = open_api.depot_create_asset(TEST_DEPOT_NAME, [{
         "parent_id": 120347220059339,
         "name": file_name,
         "add_new_version": False
     }])
     if not res_0.is_succeeded():
@@ -87,100 +100,100 @@
     if not res_1.is_succeeded():
         on_api_failed(res_1)
         assert 0
 
     logging.info("[TEST][API] \"%s\" success, signed url: %s" % (res_1.url, res_1.results.get(0)["signed_url"]))
 
 
-def test_depot_get_child_node_id_in_range():
+def test_depot_get_child_node_id_in_range(open_api):
     res = open_api.depot_get_child_node_id_in_range(TEST_DEPOT_NAME, parent_id=120347220059339, offset=0, count=2,
                                                     query_filters=[{"meta": "type", "condition": "x != directory"}],
                                                     is_recursive=True)
     if not res.is_succeeded():
         on_api_failed(res)
         assert 0
 
     nodes = res.results.get(0)["nodes"]
     logging.info("[TEST][API] \"%s\" success" % res.url)
 
 
-def test_depot_get_node_brief_by_path():
+def test_depot_get_node_brief_by_path(open_api):
     res = open_api.depot_get_node_brief_by_path(TEST_DEPOT_NAME, root_id=120347220059296,
                                                 path="open_api_test/asset.jpg")
     if not res.is_succeeded():
         on_api_failed(res)
         assert 0
 
     node = res.results.get(0)
     logging.info("[TEST][API] \"%s\" success, name: %s" % (res.url, node["name"]))
 
 
-def test_depot_add_asset_tag():
+def test_depot_add_asset_tag(open_api):
     res = open_api.depot_add_asset_tag(TEST_DEPOT_NAME, asset_id=120347220059344, tag_name=[utils.get_random_string(5)])
     if not res.is_succeeded():
         on_api_failed(res)
         assert 0
 
     node = res.results.get(0)
     logging.info("[TEST][API] \"%s\" success, tag id: %d" % (res.url, node))
 
 
-def test_get_account_detail():
+def test_get_account_detail(open_api):
     res = open_api.get_account_detail()
     if not res.is_succeeded():
         on_api_failed(res)
         assert 0
 
     logging.info("[TEST][API] \"%s\" success, email: %s" % (res.url, res.results.get(0)["email"]))
 
 
-def test_get_ticket():
+def test_get_ticket(open_api):
     res = open_api.get_ticket()
     if not res.is_succeeded():
         on_api_failed(res)
         assert 0
 
     logging.info("[TEST][API] \"%s\" success, ticket: %s" % (res.url, res.results.get(0)))
 
 
-def test_get_last_access_location_by_account():
+def test_get_last_access_location_by_account(open_api):
     res = open_api.get_last_access_location_by_account()
     if not res.is_succeeded():
         on_api_failed(res)
         assert 0
 
     logging.info("[TEST][API] \"%s\" success, last access location: %s" % (res.url, res.results.get(0)))
 
 
-def test_depot_create_directory():
+def test_depot_create_directory(open_api):
     res = open_api.depot_create_directory(TEST_DEPOT_NAME, [{
         "parent_id": 120347220059339,
         "name": "new_dir",
         "allowed_rename": True,
         "return_existing_id": False
     }])
     if not res.is_succeeded():
         on_api_failed(res)
         assert 0
 
     logging.info("[TEST][API] \"%s\" success, new dir id: %s" % (res.url, res.results.get(0)["id"]))
 
 
-def test_depot_create_multi_asset():
+def test_depot_create_multi_asset(open_api):
     res = open_api.depot_create_multi_asset(TEST_DEPOT_NAME, [{
         "parent_id": 120347220059339,
         "name": "new_multi_asset"
     }])
     if not res.is_succeeded():
         on_api_failed(res)
         assert 0
 
     logging.info("[TEST][API] \"%s\" success, new multi asset id: %s" % (res.url, res.results.get(0)["id"]))
 
 
-def test_depot_move_node():
+def test_depot_move_node(open_api):
     res = open_api.depot_move_node(TEST_DEPOT_NAME, ids=[120347220064827], other_parent_id=120347220064825)
     if not res.is_succeeded():
         on_api_failed(res)
         assert 0
 
     logging.info("[TEST][API] \"%s\" success" % res.url)
```

