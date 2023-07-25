# Comparing `tmp/fluke-api-0.4.0.tar.gz` & `tmp/fluke-api-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluke-api-0.4.0.tar", last modified: Mon Jul 24 07:44:01 2023, max compression
+gzip compressed data, was "fluke-api-0.4.1.tar", last modified: Tue Jul 25 05:35:05 2023, max compression
```

## Comparing `fluke-api-0.4.0.tar` & `fluke-api-0.4.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:44:01.229350 fluke-api-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-24 07:43:51.000000 fluke-api-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-07-24 07:44:01.217350 fluke-api-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-24 07:43:51.000000 fluke-api-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:44:01.217350 fluke-api-0.4.0/fluke/
--rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-07-24 07:43:51.000000 fluke-api-0.4.0/fluke/_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-24 07:43:51.000000 fluke-api-0.4.0/fluke/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    44163 2023-07-24 07:43:51.000000 fluke-api-0.4.0/fluke/_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-24 07:43:51.000000 fluke-api-0.4.0/fluke/_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    24688 2023-07-24 07:43:51.000000 fluke-api-0.4.0/fluke/_iohandlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-07-24 07:43:51.000000 fluke-api-0.4.0/fluke/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    25070 2023-07-24 07:43:51.000000 fluke-api-0.4.0/fluke/queues.py
--rw-r--r--   0 runner    (1001) docker     (123)    81821 2023-07-24 07:43:51.000000 fluke-api-0.4.0/fluke/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:44:01.217350 fluke-api-0.4.0/fluke_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-07-24 07:44:01.000000 fluke-api-0.4.0/fluke_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-24 07:44:01.000000 fluke-api-0.4.0/fluke_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 07:44:01.000000 fluke-api-0.4.0/fluke_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-24 07:44:01.000000 fluke-api-0.4.0/fluke_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 07:44:01.000000 fluke-api-0.4.0/fluke_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-24 07:43:51.000000 fluke-api-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 07:44:01.229350 fluke-api-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:44:01.217350 fluke-api-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-24 07:43:51.000000 fluke-api-0.4.0/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    15482 2023-07-24 07:43:51.000000 fluke-api-0.4.0/tests/test_queues.py
--rw-r--r--   0 runner    (1001) docker     (123)   169436 2023-07-24 07:43:51.000000 fluke-api-0.4.0/tests/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:35:05.439866 fluke-api-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-25 05:34:55.000000 fluke-api-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-07-25 05:35:05.439866 fluke-api-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-25 05:34:55.000000 fluke-api-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:35:05.439866 fluke-api-0.4.1/fluke/
+-rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-07-25 05:34:55.000000 fluke-api-0.4.1/fluke/_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-07-25 05:34:55.000000 fluke-api-0.4.1/fluke/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44440 2023-07-25 05:34:55.000000 fluke-api-0.4.1/fluke/_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-25 05:34:55.000000 fluke-api-0.4.1/fluke/_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24688 2023-07-25 05:34:55.000000 fluke-api-0.4.1/fluke/_iohandlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-07-25 05:34:55.000000 fluke-api-0.4.1/fluke/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25179 2023-07-25 05:34:55.000000 fluke-api-0.4.1/fluke/queues.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82202 2023-07-25 05:34:55.000000 fluke-api-0.4.1/fluke/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:35:05.439866 fluke-api-0.4.1/fluke_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-07-25 05:35:05.000000 fluke-api-0.4.1/fluke_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-25 05:35:05.000000 fluke-api-0.4.1/fluke_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 05:35:05.000000 fluke-api-0.4.1/fluke_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-25 05:35:05.000000 fluke-api-0.4.1/fluke_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 05:35:05.000000 fluke-api-0.4.1/fluke_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-25 05:34:55.000000 fluke-api-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 05:35:05.439866 fluke-api-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:35:05.439866 fluke-api-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-25 05:34:55.000000 fluke-api-0.4.1/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-07-25 05:34:55.000000 fluke-api-0.4.1/tests/test_queues.py
+-rw-r--r--   0 runner    (1001) docker     (123)   170527 2023-07-25 05:34:55.000000 fluke-api-0.4.1/tests/test_storage.py
```

### Comparing `fluke-api-0.4.0/LICENSE` & `fluke-api-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fluke-api-0.4.0/PKG-INFO` & `fluke-api-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluke-api
-Version: 0.4.0
+Version: 0.4.1
 Summary: Move your data around
 Author: Manos Stoumpos
 Author-email: manosstoumpos@gmail.com
 License: MIT
 Project-URL: Homepage, https://github.com/manoss96/fluke
 Project-URL: Bug Tracker, https://github.com/manoss96/fluke/issues
 Project-URL: Documentation, https://fluke.rtfd.io
```

### Comparing `fluke-api-0.4.0/README.md` & `fluke-api-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `fluke-api-0.4.0/fluke/_cache.py` & `fluke-api-0.4.1/fluke/_cache.py`

 * *Files identical despite different names*

### Comparing `fluke-api-0.4.0/fluke/_exceptions.py` & `fluke-api-0.4.1/fluke/_exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -92,15 +92,36 @@
 
         :param Any val: The value provided by the user.
         '''
         msg = f'Value "{val}" is not of type "str".'
         super().__init__(msg)
 
 
-class AzureBlobContainerNotFoundError(Exception):
+class BucketNotFoundError(Exception):
+    '''
+    This exception is thrown whenever the user provides \
+    an Amazon S3 bucket that does not exist.
+
+    :param str bucket: The name of the bucket that \
+        was provided by the user.
+    '''
+
+    def __init__(self, bucket: str):
+        '''
+        This exception is thrown whenever the user provides \
+        an Amazon S3 bucket that does not exist.
+
+        :param str bucket: The name of the bucket that \
+            was provided by the user.
+        '''
+        msg = f'No bucket having the name "{bucket}" exists.'
+        super().__init__(msg)
+
+
+class ContainerNotFoundError(Exception):
     '''
     This exception is thrown whenever the user provides \
     an Azure blob container that does not exist.
 
     :param str container: The name of the container that \
         was provided by the user.
     '''
```

### Comparing `fluke-api-0.4.0/fluke/_handlers.py` & `fluke-api-0.4.1/fluke/_handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Optional as _Optional
 
 
 import boto3 as _boto3
 import paramiko as _prmk
 from azure.identity import ClientSecretCredential as _CSC
 from azure.storage.blob import ContainerClient as _ContainerClient
+from botocore.exceptions import ClientError as _CE
 
 
 from .auth import AWSAuth as _AWSAuth
 from .auth import AzureAuth as _AzureAuth
 from .auth import RemoteAuth as _RemoteAuth
 from ._cache import CacheManager as _CacheManager
 from ._iohandlers import _FileReader
@@ -22,14 +23,15 @@
 from ._iohandlers import RemoteFileReader as _RemoteFileReader
 from ._iohandlers import RemoteFileWriter as _RemoteFileWriter
 from ._iohandlers import AmazonS3FileReader as _AmazonS3FileReader
 from ._iohandlers import AmazonS3FileWriter as _AmazonS3FileWriter
 from ._iohandlers import AzureBlobReader as _AzureBlobReader
 from ._iohandlers import AzureBlobWriter as _AzureBlobWriter
 from ._exceptions import UnknownKeyTypeError as _UKTE
+from ._exceptions import BucketNotFoundError as _BNFE
 from ._helper import join_paths as _join_paths
 from ._helper import infer_separator as _infer_sep
 from ._helper import relativize_path as _relativize
 
 
 class ClientHandler(_ABC):
     '''
@@ -893,14 +895,21 @@
             return
 
         print(f"\nEstablishing connection to '{self.__bucket_name}' Amazon S3 bucket...")
         self.__bucket = _boto3.resource(
             service_name='s3',
             **self.__auth.get_credentials()
         ).Bucket(self.__bucket_name)
+        # Ensure that bucket exists.
+        try:
+            self.__bucket.meta.client.head_bucket(Bucket=self.__bucket_name)
+        except _CE:
+            self.__bucket = None
+            raise _BNFE(bucket=self.__bucket_name)
+
         print("Connection established.")
 
 
     def close_connections(self):
         '''
         Closes the HTTP connection to the Amazon S3 bucket.
         '''
@@ -913,15 +922,14 @@
         '''
         Returns ``True`` if the provided path exists \
         within the directory, else returns ``False``.
 
         :param str path: Either an absolute path or a \
             path relative to the directory.
         '''
-        from botocore.exceptions import ClientError as _CE
         try:
             self.__bucket.Object(path).load()
         except _CE:
             return False
         return True
 
 
@@ -1161,15 +1169,14 @@
         return self.__container is not None
 
 
     def open_connections(self) -> None:
         '''
         Opens an HTTP connection to the Azure blob container.
         '''
-
         if self.__container is not None:
             return
 
         credentials = self.__auth.get_credentials()
 
         print(f"\nEstablishing connection to '{self.__container_name}' Azure blob container...")
         if 'conn_string' in credentials:
```

### Comparing `fluke-api-0.4.0/fluke/_helper.py` & `fluke-api-0.4.1/fluke/_helper.py`

 * *Files identical despite different names*

### Comparing `fluke-api-0.4.0/fluke/_iohandlers.py` & `fluke-api-0.4.1/fluke/_iohandlers.py`

 * *Files identical despite different names*

### Comparing `fluke-api-0.4.0/fluke/auth.py` & `fluke-api-0.4.1/fluke/auth.py`

 * *Files identical despite different names*

### Comparing `fluke-api-0.4.0/fluke/queues.py` & `fluke-api-0.4.1/fluke/queues.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+
+
+__all__ = [
+    'AmazonSQSQueue',
+    'AzureStorageQueue',
+]
+
+
 import time as _time
 import random as _rand
 import warnings as _warn
 from abc import ABC as _ABC
 from abc import abstractmethod as _absmethod
 from typing import Iterator as _Iterator
 from typing import Optional as _Optional
@@ -373,17 +381,17 @@
         '''
         while True:
 
             if not suppress_output:
                 print(f'\nPolling messages from queue "{self.get_name()}".')
 
             num_messages_fetched = 0
+            num_messages_delivered = 0
 
-            while num_messages is None or num_messages_fetched < num_messages:
-
+            while num_messages is None or num_messages_delivered < num_messages:
                 batch = []
                 while len(batch) < batch_size:
                     microbatch = self.__queue.receive_messages(
                         AttributeNames=['QueueUrl'],
                         VisibilityTimeout=30,
                         MaxNumberOfMessages=min(
                             batch_size - len(batch),
@@ -418,19 +426,19 @@
                             print(f'Failed to delete message "{msg}".')
                     # Filter out any messages that failed to be removed.
                     deleted_messages = []
                     for j in map(lambda d: int(d['Id']), resp['Successful']):
                         deleted_messages.append(messages[j])
                     # Only deliver successfully deleted messages.
                     yield deleted_messages
-                    num_messages_fetched += len(deleted_messages)
+                    num_messages_delivered += len(deleted_messages)
                 else:
                     # First deliver messages.
                     yield messages
-                    num_messages_fetched += len(messages)
+                    num_messages_delivered += len(messages)
                     # Then attempt to remove them from queue.
                     resp = self.__queue.delete_messages(Entries=entries)
                     if not suppress_output and 'Failed' in resp:
                         for msg in map(lambda d: d['Message'], resp['Failed']):
                             print(f'Failed to delete message "{msg}".')
 
             if polling_frequency is None:
```

### Comparing `fluke-api-0.4.0/fluke/storage.py` & `fluke-api-0.4.1/fluke/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from ._handlers import AzureClientHandler as _AzureClientHandler
 from ._exceptions import InvalidPathError as _IPE
 from ._exceptions import InvalidFileError as _IFE
 from ._exceptions import InvalidDirectoryError as _IDE
 from ._exceptions import OverwriteError as _OverwriteError
 from ._exceptions import NonStringMetadataKeyError as _NSMKE
 from ._exceptions import NonStringMetadataValueError as _NSMVE
-from ._exceptions import AzureBlobContainerNotFoundError as _ABCNFE 
+from ._exceptions import ContainerNotFoundError as _CNFE 
 
 
 class _File(_ABC):
     '''
     An abstract class which serves as the \
     base class for all file-like classes.
 
@@ -685,14 +685,16 @@
     :param str bucket: The name of the bucket in which \
         the file resides.
     :param str path: The path pointing to the file.
     :param bool cache: Indicates whether it is allowed for \
         any fetched data to be cached for faster subsequent \
         access.
 
+    :raises BucketNotFoundError: The specified \
+        bucket does not exist.
     :raises InvalidPathError: The provided path \
         does not exist.
     :raises InvalidFileError: The provided path \
         points to a directory.
 
     :note: The provided path must not begin with \
         a separator.
@@ -717,14 +719,16 @@
         :param str bucket: The name of the bucket in which \
             the file resides.
         :param str path: The path pointing to the file.
         :param bool cache: Indicates whether it is allowed for \
             any fetched data to be cached for faster subsequent \
             access. Defaults to ``False``.
 
+        :raises BucketNotFoundError: The specified \
+            bucket does not exist.
         :raises InvalidPathError: The provided path \
             does not exist.
         :raises InvalidFileError: The provided path \
             points to a directory.
 
         :note: The provided path must not begin with \
             a separator.
@@ -816,15 +820,15 @@
     :param str container: The name of the container in \
         which the blob resides.
     :param str path: The path pointing to the file.
     :param bool cache: Indicates whether it is allowed for \
         any fetched data to be cached for faster subsequent \
         access.
 
-    :raises AzureBlobContainerNotFoundError: The \
+    :raises ContainerNotFoundError: The \
         specified container does not exist.
     :raises InvalidPathError: The provided path \
         does not exist.
     :raises InvalidFileError: The provided path \
         points to a directory.
 
     :note: The provided path must not begin with \
@@ -850,15 +854,15 @@
         :param str container: The name of the container in \
             which the blob resides.
         :param str path: The path pointing to the file.
         :param bool cache: Indicates whether it is allowed for \
             any fetched data to be cached for faster subsequent \
             access. Defaults to ``False``.
 
-        :raises AzureBlobContainerNotFoundError: The \
+        :raises ContainerNotFoundError: The \
             specified container does not exist.
         :raises InvalidPathError: The provided path \
             does not exist.
         :raises InvalidFileError: The provided path \
             points to a directory.
 
         :note: The provided path must not begin with \
@@ -884,15 +888,15 @@
         super().__init__(
             path=path,
             handler=azr_handler)
         
         # Throw an exception if container does not exist.
         if not azr_handler.container_exists():
             self.close()
-            raise _ABCNFE(container)
+            raise _CNFE(container)
         
         if not azr_handler.path_exists(path=path):
             self.close()
             raise _IPE(path)
         if not azr_handler.is_file(file_path=path):
             self.close()
             raise _IFE(path)
@@ -2032,14 +2036,16 @@
         any fetched data to be cached for faster subsequent \
         access. Defaults to ``False``.
     :param bool create_if_missing: If set to ``True``, then the directory \
         to which the provided path points will be automatically created \
         in case it does not already exist, instead of an exception being \
         thrown. Defaults to ``False``.
 
+    :raises BucketNotFoundError: The specified \
+        bucket does not exist.
     :raises InvalidPathError: The provided path \
         does not exist.
 
     :note: The provided path must not begin with \
         a separator.
             
             * Wrong: ``/path/to/dir``
@@ -2068,14 +2074,16 @@
             any fetched data to be cached for faster subsequent \
             access. Defaults to ``True``.
         :param bool create_if_missing: If set to ``True``, then the directory \
             to which the provided path points will be automatically created \
             in case it does not already exist, instead of an exception being \
             thrown. Defaults to ``False``.
 
+        :raises BucketNotFoundError: The specified \
+            bucket does not exist.
         :raises InvalidPathError: The provided path \
             does not exist.
 
         :note: The provided path must not begin with \
             a separator.
                 
                 * Wrong: ``/path/to/dir``
@@ -2257,14 +2265,16 @@
         any fetched data to be cached for faster subsequent \
         access. Defaults to ``False``.
     :param bool create_if_missing: If set to ``True``, then the directory \
         to which the provided path points will be automatically created \
         in case it does not already exist, instead of an exception being \
         thrown. Defaults to ``False``.
 
+    :raises ContainerNotFoundError: The \
+        specified container does not exist.
     :raises InvalidPathError: The provided path \
         does not exist.
 
     :note: The provided path must not begin with \
         a separator.
             
             * Wrong: ``/path/to/dir``
@@ -2293,18 +2303,18 @@
             any fetched data to be cached for faster subsequent \
             access. Defaults to ``True``.
         :param bool create_if_missing: If set to ``True``, then the directory \
             to which the provided path points will be automatically created \
             in case it does not already exist, instead of an exception being \
             thrown. Defaults to ``False``.
 
+        :raises ContainerNotFoundError: The \
+            specified container does not exist.
         :raises InvalidPathError: The provided path \
             does not exist.
-        :raises InvalidDirectoryError: The provided path \
-            does not point to a directory.
 
         :note: The provided path must not begin with \
             a separator.
                 
                 * Wrong: ``/path/to/dir``
                 * Right: ``path/to/dir``
         '''        
@@ -2328,15 +2338,15 @@
         super().__init__(
             path=path,
             handler=azr_handler)
 
         # Throw an exception if container does not exist.
         if not azr_handler.container_exists():
             self.close()
-            raise _ABCNFE(container)
+            raise _CNFE(container)
 
         # Create directory or throw an exception
         # depending on the value of "create_if_missing".
         if path != '':
             if not azr_handler.path_exists(path=path):
                 if create_if_missing:
                     azr_handler.mkdir(path=path)
```

### Comparing `fluke-api-0.4.0/fluke_api.egg-info/PKG-INFO` & `fluke-api-0.4.1/fluke_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluke-api
-Version: 0.4.0
+Version: 0.4.1
 Summary: Move your data around
 Author: Manos Stoumpos
 Author-email: manosstoumpos@gmail.com
 License: MIT
 Project-URL: Homepage, https://github.com/manoss96/fluke
 Project-URL: Bug Tracker, https://github.com/manoss96/fluke/issues
 Project-URL: Documentation, https://fluke.rtfd.io
```

### Comparing `fluke-api-0.4.0/pyproject.toml` & `fluke-api-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fluke-api"
-version = "0.4.0"
+version = "0.4.1"
 authors = [
   {email = "manosstoumpos@gmail.com"},
   {name = "Manos Stoumpos"}
 ]
 description = "Move your data around"
 keywords = ["data", "transfer", "file", "filesystem", "cloud"]
 readme = "README.md"
```

### Comparing `fluke-api-0.4.0/tests/test_auth.py` & `fluke-api-0.4.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `fluke-api-0.4.0/tests/test_queues.py` & `fluke-api-0.4.1/tests/test_queues.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,14 +287,26 @@
         counter = 0
         with self.build_queue() as queue:
             for batch in queue.poll(batch_size=batch_size):
                 self.assertEqual(len(batch), batch_sizes[counter])
                 counter += 1
         self.purge()
 
+    def test_poll_on_num_messages_and_batch_size(self):
+        messages = set(str(i) for i in range(20))
+        self.send_messages(messages)
+        batch_size = 5
+        num_batches = 4
+        batches = []
+        with self.build_queue() as queue:
+            for batch in queue.poll(num_messages=len(messages), batch_size=batch_size):
+                batches.append(batch)
+        self.assertEqual(len(batches), num_batches)
+        self.purge()
+
     def test_poll_on_pre_delivery_delete_set_to_False(self):
         num_messages = 5
         messages = set(str(i) for i in range(num_messages))
         self.send_messages(messages)
         with self.build_queue() as queue:
             for _ in queue.poll(pre_delivery_delete=False):
                 # Assert that messages have not been deleted yet.
@@ -429,14 +441,26 @@
         counter = 0
         with self.build_queue() as queue:
             for batch in queue.poll(batch_size=batch_size):
                 self.assertEqual(len(batch), batch_sizes[counter])
                 counter += 1
         self.purge()
 
+    def test_poll_on_num_messages_and_batch_size(self):
+        messages = set(str(i) for i in range(20))
+        self.send_messages(messages)
+        batch_size = 5
+        num_batches = 4
+        batches = []
+        with self.build_queue() as queue:
+            for batch in queue.poll(num_messages=len(messages), batch_size=batch_size):
+                batches.append(batch)
+        self.assertEqual(len(batches), num_batches)
+        self.purge()
+
     def test_poll_on_pre_delivery_delete_set_to_False(self):
         num_messages = 5
         messages = set(str(i) for i in range(num_messages))
         self.send_messages(messages)
         with self.build_queue() as queue:
             for _ in queue.poll(pre_delivery_delete=False):
                 # Assert that messages have not been deleted yet.
```

### Comparing `fluke-api-0.4.0/tests/test_storage.py` & `fluke-api-0.4.1/tests/test_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     AzureBlobFile, AzureBlobDir
 from fluke._exceptions import OverwriteError
 from fluke._exceptions import InvalidPathError
 from fluke._exceptions import InvalidFileError
 from fluke._exceptions import InvalidDirectoryError
 from fluke._exceptions import NonStringMetadataKeyError
 from fluke._exceptions import NonStringMetadataValueError
+from fluke._exceptions import BucketNotFoundError
+from fluke._exceptions import ContainerNotFoundError
 
 
 '''
 Helper Functions
 '''
 def join_paths(*paths: str) -> str:
     '''
@@ -416,29 +418,34 @@
 
     @staticmethod
     def get_mock_methods() -> dict[str, Mock]:
         '''
         Returns a dictionary containing all the \
         methods that are to be mocked.
         '''
+        def get_client_from_constructor(*args, **kwargs):
+            return MockContainerClient(kwargs['container_name'], TEST_FILES_DIR)
 
+        def get_client_from_conn_string(*args, **kwargs):
+            return MockContainerClient(kwargs['container_name'], TEST_FILES_DIR)
+        
         return {
             'azure.identity.ClientSecretCredential.__init__': Mock(return_value=None),
             'azure.storage.blob.ContainerClient.__new__': Mock(
-                return_value=MockContainerClient(CONTAINER, path=TEST_FILES_DIR)
+                wraps=get_client_from_constructor
             ),
             'azure.storage.blob.ContainerClient.__init__': Mock(return_value=None),
             'azure.storage.blob.ContainerClient.from_connection_string': Mock(
-                return_value=MockContainerClient(CONTAINER, path=TEST_FILES_DIR)
+                wraps=get_client_from_conn_string
             )
         }
 
     @simulate_latency
     def exists(self) -> bool:
-        return True
+        return self.container_name == CONTAINER
     
     @simulate_latency    
     def get_blob_client(self, blob: str) -> MockBlobClient:
         return MockContainerClient.MockBlobClient(blob_name=blob)
 
     @simulate_latency
     def list_blobs(
@@ -648,14 +655,15 @@
         # to copy file a second time.
         self.assertFalse(file.transfer_to(dst=dir))
         
         # Remove copy of the file.
         copy_path = join_paths(ABS_DIR_PATH, FILE_NAME)
         os.remove(copy_path)
 
+
 class TestRemoteFile(unittest.TestCase):
 
     @staticmethod
     def build_file(path: str = ABS_FILE_PATH, cache: bool = False) -> RemoteFile:
         return RemoteFile(**{
             'auth': get_remote_auth_instance(hostname=HOST),
             'path': path,
@@ -955,32 +963,39 @@
 
 
     def tearDown(self):
         self.MOCK_S3.stop()
         patch.stopall()
     
     @staticmethod
-    def build_file(path: str = REL_FILE_PATH, cache: bool = False) -> AmazonS3File:
+    def build_file(
+        path: str = REL_FILE_PATH,
+        bucket: str = BUCKET,
+        cache: bool = False
+    ) -> AmazonS3File:
         return AmazonS3File(**{
             'auth': get_aws_auth_instance(),
-            'bucket': BUCKET,
+            'bucket': bucket,
             'path': path,
             'cache': cache
         })
 
     def test_constructor(self):
         with self.build_file() as file:
             self.assertEqual(file.get_path(), REL_FILE_PATH)
 
     def test_constructor_on_invalid_path_error(self):
         self.assertRaises(InvalidPathError, self.build_file, path="NON_EXISTING_PATH")
 
     def test_constructor_on_invalid_file_error(self):
         self.assertRaises(InvalidFileError, self.build_file, path=REL_DIR_PATH)
 
+    def test_constructor_on_bucket_not_found_error(self):
+        self.assertRaises(BucketNotFoundError, self.build_file, bucket='UNKNOWN')
+
     def test_get_name(self):
         with self.build_file() as file:
             self.assertEqual(file.get_name(), FILE_NAME)
 
     def test_get_uri(self):
         with self.build_file() as file:
             self.assertEqual(file.get_uri(), f"s3://{BUCKET}/{REL_FILE_PATH}")
@@ -1244,20 +1259,21 @@
 
 
 class TestAzureBlobFile(unittest.TestCase):
 
     @staticmethod
     def build_file(
         path: str = REL_FILE_PATH,
+        container: str = CONTAINER,
         cache: bool = False,
         from_conn_string: bool = False
     ) -> AzureBlobFile:
         return AzureBlobFile(**{
             'auth': get_azure_auth_instance(from_conn_string),
-            'container': CONTAINER,
+            'container': container,
             'path': path,
             'cache': cache
         })
 
     def setUp(self):
         for k, v in MockContainerClient.get_mock_methods().items():
             patch(k, v).start()
@@ -1275,14 +1291,17 @@
 
     def test_constructor_on_invalid_path_error(self):
         self.assertRaises(InvalidPathError, self.build_file, path="NON_EXISTING_PATH")
 
     def test_constructor_on_invalid_file_error(self):
         self.assertRaises(InvalidFileError, self.build_file, path=REL_DIR_PATH)
 
+    def test_constructor_on_container_not_found_error(self):
+        self.assertRaises(ContainerNotFoundError, self.build_file, container='UNKNOWN')
+
     def test_get_name(self):
         with self.build_file() as file:
             self.assertEqual(file.get_name(), FILE_NAME)
 
     def test_get_container_name(self):
         with self.build_file() as file:
             self.assertEqual(file.get_container_name(), CONTAINER)
@@ -2794,20 +2813,21 @@
     def tearDown(self):
         self.MOCK_S3.stop()
         patch.stopall()
     
     @staticmethod
     def build_dir(
         path: str = REL_DIR_PATH,
+        bucket: str = BUCKET,
         cache: bool = False,
         create_if_missing: bool = False
     ) -> AmazonS3Dir:
         return AmazonS3Dir(**{
             'auth': get_aws_auth_instance(),
-            'bucket': BUCKET,
+            'bucket': bucket,
             'path': path,
             'cache': cache,
             'create_if_missing': create_if_missing
         })
     
     def test_constructor(self):
         with self.build_dir() as dir:
@@ -2822,14 +2842,17 @@
                 obj.delete()
             except:
                 self.fail(f"Directory {dir_path} was not created!")
 
     def test_constructor_on_invalid_path_error(self):
         self.assertRaises(InvalidPathError, self.build_dir, path="NON_EXISTING_PATH")
 
+    def test_constructor_on_bucket_not_found_error(self):
+        self.assertRaises(BucketNotFoundError, self.build_dir, bucket='UNKNOWN')
+
     def test_get_path_on_none_path(self):
         with self.build_dir(path=None) as dir:
             self.assertEqual(dir.get_path(), '')  
 
     def test_get_name(self):
         with self.build_dir() as dir:
             self.assertEqual(dir.get_name(), DIR_NAME)
@@ -3652,21 +3675,22 @@
 
     def tearDown(self):
         patch.stopall()
     
     @staticmethod
     def build_dir(
         path: str = REL_DIR_PATH,
+        container: str = CONTAINER,
         cache: bool = False,
         create_if_missing: bool = False,
         from_conn_string: bool = False
     ) -> AzureBlobDir:
         return AzureBlobDir(**{
             'auth': get_azure_auth_instance(from_conn_string),
-            'container': CONTAINER,
+            'container': container,
             'path': path,
             'cache': cache,
             'create_if_missing': create_if_missing
         })
     
     def test_constructor(self):
         with self.build_dir() as dir:
@@ -3681,14 +3705,17 @@
         with self.build_dir(path=dir_path, create_if_missing=True) as _:
             self.assertTrue(os.path.exists(dir_path))
             os.rmdir(dir_path)
 
     def test_constructor_on_invalid_path_error(self):
         self.assertRaises(InvalidPathError, self.build_dir, path="NON_EXISTING_PATH")
 
+    def test_constructor_on_container_not_found_error(self):
+        self.assertRaises(ContainerNotFoundError, self.build_dir, container='UNKNOWN')
+
     def test_get_path_on_none_path(self):
         with self.build_dir(path=None) as dir:
             self.assertEqual(dir.get_path(), '')  
 
     def test_get_name(self):
         with self.build_dir() as dir:
             self.assertEqual(dir.get_name(), DIR_NAME)
```

