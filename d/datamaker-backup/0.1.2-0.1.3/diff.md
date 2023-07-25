# Comparing `tmp/datamaker-backup-0.1.2.tar.gz` & `tmp/datamaker-backup-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamaker-backup-0.1.2.tar", last modified: Tue Jul 25 13:09:58 2023, max compression
+gzip compressed data, was "datamaker-backup-0.1.3.tar", last modified: Tue Jul 25 14:48:20 2023, max compression
```

## Comparing `datamaker-backup-0.1.2.tar` & `datamaker-backup-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-07-25 13:09:58.480890 datamaker-backup-0.1.2/
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1101 2023-07-25 09:30:36.000000 datamaker-backup-0.1.2/LICENSE
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1982 2023-07-25 13:09:58.480890 datamaker-backup-0.1.2/PKG-INFO
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1253 2023-07-25 13:05:05.000000 datamaker-backup-0.1.2/README.md
-drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-07-25 13:09:58.476890 datamaker-backup-0.1.2/datamaker_backup/
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)       39 2023-07-25 09:30:36.000000 datamaker-backup-0.1.2/datamaker_backup/__init__.py
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     5094 2023-07-25 09:30:36.000000 datamaker-backup-0.1.2/datamaker_backup/storage.py
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1159 2023-07-25 09:30:36.000000 datamaker-backup-0.1.2/datamaker_backup/utils.py
-drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-07-25 13:09:58.480890 datamaker-backup-0.1.2/datamaker_backup.egg-info/
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1982 2023-07-25 13:09:58.000000 datamaker-backup-0.1.2/datamaker_backup.egg-info/PKG-INFO
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      324 2023-07-25 13:09:58.000000 datamaker-backup-0.1.2/datamaker_backup.egg-info/SOURCES.txt
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)        1 2023-07-25 13:09:58.000000 datamaker-backup-0.1.2/datamaker_backup.egg-info/dependency_links.txt
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)       52 2023-07-25 13:09:58.000000 datamaker-backup-0.1.2/datamaker_backup.egg-info/requires.txt
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)       17 2023-07-25 13:09:58.000000 datamaker-backup-0.1.2/datamaker_backup.egg-info/top_level.txt
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      106 2023-07-25 13:05:05.000000 datamaker-backup-0.1.2/pyproject.toml
--rw-r--r--   0 datamaker  (1000) datamaker  (1000)      839 2023-07-25 13:09:58.480890 datamaker-backup-0.1.2/setup.cfg
+drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-07-25 14:48:20.527728 datamaker-backup-0.1.3/
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1101 2023-07-25 12:40:40.000000 datamaker-backup-0.1.3/LICENSE
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     2634 2023-07-25 14:48:20.527728 datamaker-backup-0.1.3/PKG-INFO
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1905 2023-07-25 14:40:09.000000 datamaker-backup-0.1.3/README.md
+drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-07-25 14:48:20.527728 datamaker-backup-0.1.3/datamaker_backup/
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)       39 2023-07-25 12:40:40.000000 datamaker-backup-0.1.3/datamaker_backup/__init__.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     5094 2023-07-25 12:40:40.000000 datamaker-backup-0.1.3/datamaker_backup/storage.py
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     1172 2023-07-25 14:40:09.000000 datamaker-backup-0.1.3/datamaker_backup/utils.py
+drwxr-xr-x   0 datamaker  (1000) datamaker  (1000)        0 2023-07-25 14:48:20.527728 datamaker-backup-0.1.3/datamaker_backup.egg-info/
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)     2634 2023-07-25 14:48:20.000000 datamaker-backup-0.1.3/datamaker_backup.egg-info/PKG-INFO
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      324 2023-07-25 14:48:20.000000 datamaker-backup-0.1.3/datamaker_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)        1 2023-07-25 14:48:20.000000 datamaker-backup-0.1.3/datamaker_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)       52 2023-07-25 14:48:20.000000 datamaker-backup-0.1.3/datamaker_backup.egg-info/requires.txt
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)       17 2023-07-25 14:48:20.000000 datamaker-backup-0.1.3/datamaker_backup.egg-info/top_level.txt
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      106 2023-07-25 14:40:09.000000 datamaker-backup-0.1.3/pyproject.toml
+-rw-r--r--   0 datamaker  (1000) datamaker  (1000)      839 2023-07-25 14:48:20.527728 datamaker-backup-0.1.3/setup.cfg
```

### Comparing `datamaker-backup-0.1.2/LICENSE` & `datamaker-backup-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datamaker-backup-0.1.2/PKG-INFO` & `datamaker-backup-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamaker-backup
-Version: 0.1.2
+Version: 0.1.3
 Summary: datamaker backup
 Home-page: https://www.datamaker.io
 Author: datamaker
 Author-email: developer@datamaker.io
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,32 +17,109 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Installation
 
 ## .env
-.env 파일에 아래 환경변수를 적절히 활용
+`.env.dist`에 아래 내용 추가
+
+```dotenv
+# BACKUP
+ENABLE_RESTORE=true|false
+ENABLE_BACKUP=true|false
+RESTORE_DATA_ONLY=true|false
+RESTORE_OPTIONS=do-not-set-unless-you-know-what-you-are-doing
+```
+
+## settings.py
+
+`settings.py`에 아래 내용 추가
+
+```python
+from datamaker_backup import get_backup_settings
+
+...
+
+INSTALLED_APPS = (
+    ...
+    'dbbackup',  # django-dbbackup
+)
+
+...
+
+
+# datamaker-backup
+# https://github.com/datamaker-kr/datamaker-backup
+
+BACKUP_CONFIG = get_backup_settings('<repository-name>', env)
+vars().update(BACKUP_CONFIG)
+```
+
+# Usage
+
+## 백업
+
+### database
+
+```shell
+python manage.py dbbackup
+```
+
+### media
+
+```shell
+python manage.py mediabackup
+```
+
+## 복원
+
+
+### database
+
+```shell
+python manage.py dbrestore
+```
+
+### media
+
+```shell
+python manage.py mediarestore
+```
+
+특정 백업으로 부터 복원하는 경우 
+
+```shell
+python manage.py dbrestore -i <backup_id>
+```
+
+```shell
+python manage.py mediarestore -i <backup_id>
+```
+
+# Configuration
+
+`.env`에서 아래 설정을 필요에 따라 적용.
 
 ### ENABLE_RESTORE
-`true`|`false`
+`true` | `false`
 
 `dbrestore`, `mediarestore` 사용 가능 여부. 주로 production 환경에서는 비활성화.
 
 Default: `false`
 
 ### ENABLE_BACKUP
-`true`|`false`
+`true` | `false`
 
 `dbbackup`, `mediabackup` 사용 가능 여부. 주로 development 환경에서는 비활성화.
 
 Default: `false`
 
 ### RESTORE_DATA_ONLY
-`true`|`false`
+`true` | `false`
 
 `dbrestore`시 schema는 그대로 두고 data만 복원할지 여부.
 
 아직까지는 해당 옵션을 활성화 할 경우 복원할 db에 data가 모두 삭제된 상태로 두어야 함.
 
 Default: `false`
 
@@ -50,32 +127,8 @@
 comma separated list of pg_restore option names
 
 Example:
 `clean,create`
 
 Default:
 - `RESTORE_DATA_ONLY`가 `true`일 때에는 `data-only,disable-triggers,exit-on-error`
-- `RESTORE_DATA_ONLY`가 `false`일 때에는 `clean,create,exit-on-error`
-
-## settings.py
-
-settings.py에 아래 내용 추가
-
-```python
-from datamaker_backup import get_backup_settings
-
-...
-
-INSTALLED_APPS = (
-    ...
-    'dbbackup',  # django-dbbackup
-)
-
-...
-
-
-# datamaker-backup
-# https://github.com/datamaker-kr/datamaker-backup
-
-BACKUP_CONFIG = get_backup_settings('<repository-name>', env)
-vars().update(BACKUP_CONFIG)
-```
+- `RESTORE_DATA_ONLY`가 `false`일 때에는 `clean,create,if-exists,exit-on-error`
```

### Comparing `datamaker-backup-0.1.2/datamaker_backup/storage.py` & `datamaker-backup-0.1.3/datamaker_backup/storage.py`

 * *Files identical despite different names*

### Comparing `datamaker-backup-0.1.2/datamaker_backup/utils.py` & `datamaker-backup-0.1.3/datamaker_backup/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 def get_backup_settings(repository, env):
     restore_data_only = env.bool('RESTORE_DATA_ONLY', default=False)
 
     if restore_data_only:
         restore_options = ['data-only', 'disable-triggers', 'exit-on-error']
     else:
-        restore_options = ['clean', 'create', 'exit-on-error']
+        restore_options = ['clean', 'create', 'if-exists', 'exit-on-error']
 
     restore_options = env.list('RESTORE_OPTIONS', default=restore_options)
 
     connector_settings = {
         'SINGLE_TRANSACTION': False,
         'DROP': False,
         'RESTORE_SUFFIX': ' '.join([f'--{option}' for option in restore_options])
```

### Comparing `datamaker-backup-0.1.2/datamaker_backup.egg-info/PKG-INFO` & `datamaker-backup-0.1.3/datamaker_backup.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamaker-backup
-Version: 0.1.2
+Version: 0.1.3
 Summary: datamaker backup
 Home-page: https://www.datamaker.io
 Author: datamaker
 Author-email: developer@datamaker.io
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,32 +17,109 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Installation
 
 ## .env
-.env 파일에 아래 환경변수를 적절히 활용
+`.env.dist`에 아래 내용 추가
+
+```dotenv
+# BACKUP
+ENABLE_RESTORE=true|false
+ENABLE_BACKUP=true|false
+RESTORE_DATA_ONLY=true|false
+RESTORE_OPTIONS=do-not-set-unless-you-know-what-you-are-doing
+```
+
+## settings.py
+
+`settings.py`에 아래 내용 추가
+
+```python
+from datamaker_backup import get_backup_settings
+
+...
+
+INSTALLED_APPS = (
+    ...
+    'dbbackup',  # django-dbbackup
+)
+
+...
+
+
+# datamaker-backup
+# https://github.com/datamaker-kr/datamaker-backup
+
+BACKUP_CONFIG = get_backup_settings('<repository-name>', env)
+vars().update(BACKUP_CONFIG)
+```
+
+# Usage
+
+## 백업
+
+### database
+
+```shell
+python manage.py dbbackup
+```
+
+### media
+
+```shell
+python manage.py mediabackup
+```
+
+## 복원
+
+
+### database
+
+```shell
+python manage.py dbrestore
+```
+
+### media
+
+```shell
+python manage.py mediarestore
+```
+
+특정 백업으로 부터 복원하는 경우 
+
+```shell
+python manage.py dbrestore -i <backup_id>
+```
+
+```shell
+python manage.py mediarestore -i <backup_id>
+```
+
+# Configuration
+
+`.env`에서 아래 설정을 필요에 따라 적용.
 
 ### ENABLE_RESTORE
-`true`|`false`
+`true` | `false`
 
 `dbrestore`, `mediarestore` 사용 가능 여부. 주로 production 환경에서는 비활성화.
 
 Default: `false`
 
 ### ENABLE_BACKUP
-`true`|`false`
+`true` | `false`
 
 `dbbackup`, `mediabackup` 사용 가능 여부. 주로 development 환경에서는 비활성화.
 
 Default: `false`
 
 ### RESTORE_DATA_ONLY
-`true`|`false`
+`true` | `false`
 
 `dbrestore`시 schema는 그대로 두고 data만 복원할지 여부.
 
 아직까지는 해당 옵션을 활성화 할 경우 복원할 db에 data가 모두 삭제된 상태로 두어야 함.
 
 Default: `false`
 
@@ -50,32 +127,8 @@
 comma separated list of pg_restore option names
 
 Example:
 `clean,create`
 
 Default:
 - `RESTORE_DATA_ONLY`가 `true`일 때에는 `data-only,disable-triggers,exit-on-error`
-- `RESTORE_DATA_ONLY`가 `false`일 때에는 `clean,create,exit-on-error`
-
-## settings.py
-
-settings.py에 아래 내용 추가
-
-```python
-from datamaker_backup import get_backup_settings
-
-...
-
-INSTALLED_APPS = (
-    ...
-    'dbbackup',  # django-dbbackup
-)
-
-...
-
-
-# datamaker-backup
-# https://github.com/datamaker-kr/datamaker-backup
-
-BACKUP_CONFIG = get_backup_settings('<repository-name>', env)
-vars().update(BACKUP_CONFIG)
-```
+- `RESTORE_DATA_ONLY`가 `false`일 때에는 `clean,create,if-exists,exit-on-error`
```

### Comparing `datamaker-backup-0.1.2/setup.cfg` & `datamaker-backup-0.1.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = datamaker-backup
-version = 0.1.2
+version = 0.1.3
 description = datamaker backup
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://www.datamaker.io
 author = datamaker
 author_email = developer@datamaker.io
 license = MIT
```

