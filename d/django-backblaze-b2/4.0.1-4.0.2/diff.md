# Comparing `tmp/django_backblaze_b2-4.0.1.tar.gz` & `tmp/django_backblaze_b2-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_backblaze_b2-4.0.1.tar", max compression
+gzip compressed data, was "django_backblaze_b2-4.0.2.tar", max compression
```

## Comparing `django_backblaze_b2-4.0.1.tar` & `django_backblaze_b2-4.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1318 2020-08-25 16:03:37.000000 django_backblaze_b2-4.0.1/LICENSE
--rw-r--r--   0        0        0     8556 2023-07-02 20:36:28.971655 django_backblaze_b2-4.0.1/README.md
--rw-r--r--   0        0        0      264 2020-09-18 05:30:12.000000 django_backblaze_b2-4.0.1/django_backblaze_b2/__init__.py
--rw-r--r--   0        0        0     1024 2023-07-02 20:36:25.735529 django_backblaze_b2-4.0.1/django_backblaze_b2/_decorators.py
--rw-r--r--   0        0        0     2720 2023-07-24 07:09:19.210475 django_backblaze_b2-4.0.1/django_backblaze_b2/b2_file.py
--rw-r--r--   0        0        0     7932 2023-07-24 06:59:23.702987 django_backblaze_b2-4.0.1/django_backblaze_b2/cache_account_info.py
--rw-r--r--   0        0        0     2004 2023-07-02 20:36:25.736571 django_backblaze_b2-4.0.1/django_backblaze_b2/options.py
--rw-r--r--   0        0        0        0 2020-09-18 05:30:12.000000 django_backblaze_b2-4.0.1/django_backblaze_b2/py.typed
--rw-r--r--   0        0        0    12923 2023-07-24 07:09:19.210895 django_backblaze_b2-4.0.1/django_backblaze_b2/storage.py
--rw-r--r--   0        0        0     4727 2023-07-02 20:36:25.737269 django_backblaze_b2-4.0.1/django_backblaze_b2/storages.py
--rw-r--r--   0        0        0      358 2023-07-02 20:36:25.737573 django_backblaze_b2-4.0.1/django_backblaze_b2/urls.py
--rw-r--r--   0        0        0     2167 2023-07-02 20:36:25.737820 django_backblaze_b2-4.0.1/django_backblaze_b2/views.py
--rw-r--r--   0        0        0     2022 2023-07-24 07:10:14.628470 django_backblaze_b2-4.0.1/pyproject.toml
--rw-r--r--   0        0        0    10260 1970-01-01 00:00:00.000000 django_backblaze_b2-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1318 2020-08-25 16:03:37.000000 django_backblaze_b2-4.0.2/LICENSE
+-rw-r--r--   0        0        0     8556 2023-07-02 20:36:28.971655 django_backblaze_b2-4.0.2/README.md
+-rw-r--r--   0        0        0      264 2020-09-18 05:30:12.000000 django_backblaze_b2-4.0.2/django_backblaze_b2/__init__.py
+-rw-r--r--   0        0        0     1024 2023-07-02 20:36:25.735529 django_backblaze_b2-4.0.2/django_backblaze_b2/_decorators.py
+-rw-r--r--   0        0        0     2719 2023-07-25 03:57:28.852845 django_backblaze_b2-4.0.2/django_backblaze_b2/b2_file.py
+-rw-r--r--   0        0        0     7932 2023-07-24 06:59:23.702987 django_backblaze_b2-4.0.2/django_backblaze_b2/cache_account_info.py
+-rw-r--r--   0        0        0     2004 2023-07-02 20:36:25.736571 django_backblaze_b2-4.0.2/django_backblaze_b2/options.py
+-rw-r--r--   0        0        0        0 2020-09-18 05:30:12.000000 django_backblaze_b2-4.0.2/django_backblaze_b2/py.typed
+-rw-r--r--   0        0        0    12884 2023-07-25 03:57:28.853203 django_backblaze_b2-4.0.2/django_backblaze_b2/storage.py
+-rw-r--r--   0        0        0     4727 2023-07-02 20:36:25.737269 django_backblaze_b2-4.0.2/django_backblaze_b2/storages.py
+-rw-r--r--   0        0        0      358 2023-07-02 20:36:25.737573 django_backblaze_b2-4.0.2/django_backblaze_b2/urls.py
+-rw-r--r--   0        0        0     2167 2023-07-02 20:36:25.737820 django_backblaze_b2-4.0.2/django_backblaze_b2/views.py
+-rw-r--r--   0        0        0     2022 2023-07-25 04:00:30.403013 django_backblaze_b2-4.0.2/pyproject.toml
+-rw-r--r--   0        0        0    10260 1970-01-01 00:00:00.000000 django_backblaze_b2-4.0.2/PKG-INFO
```

### Comparing `django_backblaze_b2-4.0.1/LICENSE` & `django_backblaze_b2-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-4.0.1/README.md` & `django_backblaze_b2-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-4.0.1/django_backblaze_b2/_decorators.py` & `django_backblaze_b2-4.0.2/django_backblaze_b2/_decorators.py`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-4.0.1/django_backblaze_b2/b2_file.py` & `django_backblaze_b2-4.0.2/django_backblaze_b2/b2_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,11 +74,11 @@
         Save and retrieve the filename.
         If the file exists it will make another version of that file.
         """
         logger.debug(f"Saving {self.name} to b2 bucket ({self._bucket.get_id()})")
         self._bucket.upload_bytes(
             data_bytes=content.read(),
             file_name=self.name,
-            file_infos=self._file_metadata,
+            file_info=self._file_metadata,
         )
         self._has_unwritted_data = False
         return self.name
```

### Comparing `django_backblaze_b2-4.0.1/django_backblaze_b2/cache_account_info.py` & `django_backblaze_b2-4.0.2/django_backblaze_b2/cache_account_info.py`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-4.0.1/django_backblaze_b2/options.py` & `django_backblaze_b2-4.0.2/django_backblaze_b2/options.py`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-4.0.1/django_backblaze_b2/storage.py` & `django_backblaze_b2-4.0.2/django_backblaze_b2/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from datetime import datetime
 from hashlib import sha3_224 as hash
 from logging import getLogger
 from typing import IO, Any, Callable, Dict, List, Optional, Tuple, cast
 
 from b2sdk.account_info import InMemoryAccountInfo
-from b2sdk.account_info.abstract import AbstractAccountInfo
 from b2sdk.account_info.sqlite_account_info import SqliteAccountInfo
 from b2sdk.cache import AuthInfoCache
 from b2sdk.exception import FileOrBucketNotFound, NonExistentBucket
-from b2sdk.v2 import B2Api, Bucket
+from b2sdk.v2 import AbstractAccountInfo, B2Api, Bucket
 from django.core.cache.backends.base import BaseCache
 from django.core.exceptions import ImproperlyConfigured
 from django.core.files.base import File
 from django.core.files.storage import Storage
 from django.utils.deconstruct import deconstructible
 from typing_extensions import TypedDict
```

### Comparing `django_backblaze_b2-4.0.1/django_backblaze_b2/storages.py` & `django_backblaze_b2-4.0.2/django_backblaze_b2/storages.py`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-4.0.1/django_backblaze_b2/views.py` & `django_backblaze_b2-4.0.2/django_backblaze_b2/views.py`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-4.0.1/pyproject.toml` & `django_backblaze_b2-4.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.black]
 line-length = 120
 
 [tool.poetry]
 name = "django-backblaze-b2"
-version = "4.0.1"
+version = "4.0.2"
 description = "A Django app to use backblaze b2 as storage."
 authors = ["Etienne H <django_backblaze_b2@internet-e-mail.com>"]
 maintainers = ["Etienne H <django_backblaze_b2@internet-e-mail.com>"]
 license = "BSD-2-Clause"
 readme = "README.md"
 homepage = "https://github.com/ehossack/django-backblaze-b2/"
 repository = "https://github.com/ehossack/django-backblaze-b2/"
```

### Comparing `django_backblaze_b2-4.0.1/PKG-INFO` & `django_backblaze_b2-4.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-backblaze-b2
-Version: 4.0.1
+Version: 4.0.2
 Summary: A Django app to use backblaze b2 as storage.
 Home-page: https://github.com/ehossack/django-backblaze-b2/
 License: BSD-2-Clause
 Keywords: django,storage,backblaze,b2,cloud
 Author: Etienne H
 Author-email: django_backblaze_b2@internet-e-mail.com
 Maintainer: Etienne H
```

