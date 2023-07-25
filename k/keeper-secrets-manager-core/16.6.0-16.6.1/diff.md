# Comparing `tmp/keeper-secrets-manager-core-16.6.0.tar.gz` & `tmp/keeper-secrets-manager-core-16.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keeper-secrets-manager-core-16.6.0.tar", last modified: Thu Jul 13 17:43:32 2023, max compression
+gzip compressed data, was "keeper-secrets-manager-core-16.6.1.tar", last modified: Tue Jul 25 18:49:54 2023, max compression
```

## Comparing `keeper-secrets-manager-core-16.6.0.tar` & `keeper-secrets-manager-core-16.6.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:43:32.698559 keeper-secrets-manager-core-16.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-07-13 17:43:32.698559 keeper-secrets-manager-core-16.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:43:32.694559 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/configkeys.py
--rw-r--r--   0 runner    (1001) docker     (123)    77619 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:43:32.698559 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/dto/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/dto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18317 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/dto/dtos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/dto/payload.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/keeper_globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    21238 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:43:32.698559 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-07-13 17:43:32.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-13 17:43:32.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:43:32.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:43:32.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-13 17:43:32.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-13 17:43:32.000000 keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-13 17:43:32.698559 keeper-secrets-manager-core-16.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-13 17:43:16.000000 keeper-secrets-manager-core-16.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:49:54.833203 keeper-secrets-manager-core-16.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 18:49:38.000000 keeper-secrets-manager-core-16.6.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-07-25 18:49:54.833203 keeper-secrets-manager-core-16.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-07-25 18:49:38.000000 keeper-secrets-manager-core-16.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:49:54.833203 keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-25 18:49:38.000000 keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-25 18:49:38.000000 keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core/configkeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77619 2023-07-25 18:49:38.000000 keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-07-25 18:49:38.000000 keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core/crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:49:54.833203 keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core/dto/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-25 18:49:38.000000 keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core/dto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18549 2023-07-25 18:49:38.000000 keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core/dto/dtos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-25 18:49:38.000000 keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core/dto/payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-25 18:49:38.000000 keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-25 18:49:38.000000 keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-07-25 18:49:38.000000 keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core/keeper_globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-07-25 18:49:38.000000 keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-07-25 18:49:38.000000 keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21238 2023-07-25 18:49:38.000000 keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:49:54.833203 keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-07-25 18:49:54.000000 keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-25 18:49:54.000000 keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:49:54.000000 keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:49:54.000000 keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-25 18:49:54.000000 keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-25 18:49:54.000000 keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 18:49:54.833203 keeper-secrets-manager-core-16.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-25 18:49:38.000000 keeper-secrets-manager-core-16.6.1/setup.py
```

### Comparing `keeper-secrets-manager-core-16.6.0/PKG-INFO` & `keeper-secrets-manager-core-16.6.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keeper-secrets-manager-core
-Version: 16.6.0
+Version: 16.6.1
 Summary: Keeper Secrets Manager for Python 3
 Home-page: https://github.com/Keeper-Security/secrets-manager
 Author: Keeper Security
 Author-email: sm@keepersecurity.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Keeper-Security/secrets-manager/issues
 Project-URL: Documentation, https://github.com/Keeper-Security/secrets-manager
@@ -27,14 +27,17 @@
 
 # Keeper Secrets Manager Python SDK
 
 For more information see our official documentation page https://docs.keeper.io/secrets-manager/secrets-manager/developer-sdk-library/python-sdk
 
 # Change Log
 
+## 16.6.1
+* KSM 444 - Python - Added folderUid and innerFolderUid to Record
+
 ## 16.6.0
 * KSM-413 - Added support for Folders
 * KSM-434 - Improved Passkey field type support
 
 ## 16.5.4
 * KSM-405 - Added new script field type and oneTimeCode to PAM record types
 * KSM-410 - New field type: Passkey
```

### Comparing `keeper-secrets-manager-core-16.6.0/README.md` & `keeper-secrets-manager-core-16.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # Keeper Secrets Manager Python SDK
 
 For more information see our official documentation page https://docs.keeper.io/secrets-manager/secrets-manager/developer-sdk-library/python-sdk
 
 # Change Log
 
+## 16.6.1
+* KSM 444 - Python - Added folderUid and innerFolderUid to Record
+
 ## 16.6.0
 * KSM-413 - Added support for Folders
 * KSM-434 - Improved Passkey field type support
 
 ## 16.5.4
 * KSM-405 - Added new script field type and oneTimeCode to PAM record types
 * KSM-410 - New field type: Passkey
```

### Comparing `keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/configkeys.py` & `keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core/configkeys.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/core.py` & `keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core/core.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/crypto.py` & `keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core/crypto.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/dto/dtos.py` & `keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core/dto/dtos.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,24 +19,26 @@
 from keeper_secrets_manager_core.crypto import CryptoUtils
 from keeper_secrets_manager_core.exceptions import KeeperError
 from keeper_secrets_manager_helper.v3.field_type import FieldType
 
 
 class Record:
 
-    def __init__(self, record_dict, secret_key):
+    def __init__(self, record_dict, secret_key, folder_uid = ''):
         self.uid = ''
         self.title = ''
         self.type = ''
         self.files = []
         self.raw_json = None
         self.dict = {}
         self.password = None
         self.revision = None
         self.is_editable = None
+        self.folder_uid = ''
+        self.inner_folder_uid = ''
 
         self.uid = record_dict.get('recordUid')
 
         if 'recordKey' in record_dict and record_dict.get('recordKey'):
             # Folder Share
             record_key_encrypted_str = record_dict.get('recordKey')
             record_key_encrypted_bytes = utils.base64_to_bytes(record_key_encrypted_str) if \
@@ -52,14 +54,16 @@
 
         self.raw_json = record_data_json
         self.dict = utils.json_to_dict(self.raw_json)
         self.title = self.dict.get('title')
         self.type = self.dict.get('type')
         self.revision = record_dict.get('revision')
         self.is_editable = record_dict.get("isEditable")
+        self.folder_uid = record_dict.get("folderUid", "") or folder_uid
+        self.inner_folder_uid = record_dict.get("innerFolderUid")
 
         # files
         if record_dict.get('files'):
             for f in record_dict.get('files'):
 
                 file = KeeperFile(f, self.record_key_bytes)
 
@@ -292,15 +296,15 @@
         self.key = folder_key
         self.uid = folder_uid
         self.parent_uid = folder.get('parentUid', '')
         self.name = folder.get('name', '')
 
         for r in folder_records:
 
-            record = Record(r, folder_key)
+            record = Record(r, folder_key, folder_uid)
             self.records.append(record)
 
 
 class KeeperFile:
 
     def __init__(self, f, record_key_bytes):
```

### Comparing `keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/dto/payload.py` & `keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core/dto/payload.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/exceptions.py` & `keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/helpers.py` & `keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core/helpers.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/keeper_globals.py` & `keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core/keeper_globals.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/mock.py` & `keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core/mock.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/storage.py` & `keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core/storage.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core/utils.py` & `keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core/utils.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core.egg-info/PKG-INFO` & `keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keeper-secrets-manager-core
-Version: 16.6.0
+Version: 16.6.1
 Summary: Keeper Secrets Manager for Python 3
 Home-page: https://github.com/Keeper-Security/secrets-manager
 Author: Keeper Security
 Author-email: sm@keepersecurity.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Keeper-Security/secrets-manager/issues
 Project-URL: Documentation, https://github.com/Keeper-Security/secrets-manager
@@ -27,14 +27,17 @@
 
 # Keeper Secrets Manager Python SDK
 
 For more information see our official documentation page https://docs.keeper.io/secrets-manager/secrets-manager/developer-sdk-library/python-sdk
 
 # Change Log
 
+## 16.6.1
+* KSM 444 - Python - Added folderUid and innerFolderUid to Record
+
 ## 16.6.0
 * KSM-413 - Added support for Folders
 * KSM-434 - Improved Passkey field type support
 
 ## 16.5.4
 * KSM-405 - Added new script field type and oneTimeCode to PAM record types
 * KSM-410 - New field type: Passkey
```

### Comparing `keeper-secrets-manager-core-16.6.0/keeper_secrets_manager_core.egg-info/SOURCES.txt` & `keeper-secrets-manager-core-16.6.1/keeper_secrets_manager_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-core-16.6.0/setup.py` & `keeper-secrets-manager-core-16.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     'requests',
     'cryptography>=39.0.1',
     'importlib_metadata'
 ]
 
 setup(
     name="keeper-secrets-manager-core",
-    version="16.6.0",
+    version="16.6.1",
     description="Keeper Secrets Manager for Python 3",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Keeper Security",
     author_email="sm@keepersecurity.com",
     url="https://github.com/Keeper-Security/secrets-manager",
     license="MIT",
```

