# Comparing `tmp/arivo-settings_models-0.0.1rc5.tar.gz` & `tmp/arivo-settings_models-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/arivo-settings_models-0.0.1rc5.tar", last modified: Mon Jul 24 13:36:33 2023, max compression
+gzip compressed data, was "dist/arivo-settings_models-1.0.0.tar", last modified: Tue Jul 25 12:50:00 2023, max compression
```

## Comparing `arivo-settings_models-0.0.1rc5.tar` & `arivo-settings_models-1.0.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-11 10:22:52.000000 arivo-settings_models-0.0.1rc5/.coveragerc
--rw-r--r--   0 root         (0) root         (0)      111 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/AUTHORS
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/settings_models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 13:35:40.000000 arivo-settings_models-0.0.1rc5/settings_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1977 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc5/settings_models/validators.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc5/settings_models/doc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/settings_models/settings/
--rw-rw-rw-   0 root         (0) root         (0)      749 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc5/settings_models/settings/gate_control.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc5/settings_models/settings/intercom.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 13:35:40.000000 arivo-settings_models-0.0.1rc5/settings_models/settings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      477 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc5/settings_models/settings/enforcement.py
--rw-rw-rw-   0 root         (0) root         (0)    20512 2023-07-24 13:35:39.000000 arivo-settings_models-0.0.1rc5/settings_models/settings/common.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc5/settings_models/settings/device_keys.py
--rw-rw-rw-   0 root         (0) root         (0)      163 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc5/settings_models/_combat.py
--rw-rw-rw-   0 root         (0) root         (0)     6344 2023-06-28 13:41:28.000000 arivo-settings_models-0.0.1rc5/settings_models/serialization.py
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-05-17 14:33:24.000000 arivo-settings_models-0.0.1rc5/tox.ini
--rw-rw-rw-   0 root         (0) root         (0)      445 2023-05-11 10:22:52.000000 arivo-settings_models-0.0.1rc5/setup.py
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-17 14:33:24.000000 arivo-settings_models-0.0.1rc5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      707 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1353 2023-06-22 11:55:45.000000 arivo-settings_models-0.0.1rc5/.gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/tools/
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-05-17 14:33:24.000000 arivo-settings_models-0.0.1rc5/tools/pages.py
--rw-rw-rw-   0 root         (0) root         (0)      569 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3417 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc5/tests/test_serialization.py
--rw-rw-rw-   0 root         (0) root         (0)    38906 2023-07-24 13:35:39.000000 arivo-settings_models-0.0.1rc5/tests/test_validation.py
--rw-rw-rw-   0 root         (0) root         (0)    11501 2023-06-28 13:41:28.000000 arivo-settings_models-0.0.1rc5/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-06-13 13:58:32.000000 arivo-settings_models-0.0.1rc5/tests/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-05-11 10:22:52.000000 arivo-settings_models-0.0.1rc5/README.md
--rw-r--r--   0 root         (0) root         (0)     1439 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/ChangeLog
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-11 10:22:52.000000 arivo-settings_models-0.0.1rc5/test-requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/docs/
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-05-11 10:22:52.000000 arivo-settings_models-0.0.1rc5/docs/migrations.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/arivo_settings_models.egg-info/
--rw-r--r--   0 root         (0) root         (0)      707 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/arivo_settings_models.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       57 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/arivo_settings_models.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/arivo_settings_models.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/arivo_settings_models.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       47 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/arivo_settings_models.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)      922 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/arivo_settings_models.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-24 13:36:33.000000 arivo-settings_models-0.0.1rc5/arivo_settings_models.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1353 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.0/docs/migrations.md
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.0/test-requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      704 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/tools/
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.0/tools/pages.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/arivo_settings_models.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/arivo_settings_models.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/arivo_settings_models.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/arivo_settings_models.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      704 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/arivo_settings_models.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      922 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/arivo_settings_models.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/arivo_settings_models.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/arivo_settings_models.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.0/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)      111 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)     1433 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/ChangeLog
+-rw-rw-rw-   0 root         (0) root         (0)      569 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    38906 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/tests/test_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/tests/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    11501 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3417 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/tests/test_serialization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/settings_models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/settings_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6344 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/settings_models/serialization.py
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/settings_models/_combat.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/settings_models/doc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1977 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/settings_models/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:50:00.000000 arivo-settings_models-1.0.0/settings_models/settings/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/settings_models/settings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      477 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/settings_models/settings/enforcement.py
+-rw-rw-rw-   0 root         (0) root         (0)      524 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/settings_models/settings/device_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)    20512 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/settings_models/settings/common.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/settings_models/settings/intercom.py
+-rw-rw-rw-   0 root         (0) root         (0)      749 2023-07-25 12:49:49.000000 arivo-settings_models-1.0.0/settings_models/settings/gate_control.py
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-05-17 14:37:58.000000 arivo-settings_models-1.0.0/tox.ini
```

### Comparing `arivo-settings_models-0.0.1rc5/settings_models/validators.py` & `arivo-settings_models-1.0.0/settings_models/validators.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc5/settings_models/settings/gate_control.py` & `arivo-settings_models-1.0.0/settings_models/settings/gate_control.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc5/settings_models/settings/common.py` & `arivo-settings_models-1.0.0/settings_models/settings/common.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc5/settings_models/settings/device_keys.py` & `arivo-settings_models-1.0.0/settings_models/settings/device_keys.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc5/settings_models/serialization.py` & `arivo-settings_models-1.0.0/settings_models/serialization.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc5/PKG-INFO` & `arivo-settings_models-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arivo-settings_models
-Version: 0.0.1rc5
+Version: 1.0.0
 Summary: Library for arivo parking system settings definitions and models
 Home-page: https://gitlab.com/accessio/onegate/settings-models
 Author: ARIVO
 Author-email: support@arivo.co
 License: "GPL-3",
 Description: # Settings Models
```

### Comparing `arivo-settings_models-0.0.1rc5/.gitlab-ci.yml` & `arivo-settings_models-1.0.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc5/setup.cfg` & `arivo-settings_models-1.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc5/tests/test_serialization.py` & `arivo-settings_models-1.0.0/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc5/tests/test_validation.py` & `arivo-settings_models-1.0.0/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc5/tests/test_models.py` & `arivo-settings_models-1.0.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc5/tests/utils.py` & `arivo-settings_models-1.0.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `arivo-settings_models-0.0.1rc5/ChangeLog` & `arivo-settings_models-1.0.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CHANGES
 =======
 
-v0.0.1rc5
----------
+v1.0.0
+------
 
 * parking areas: default cost entries requires shortterm gates
 
 v0.0.1rc4
 ---------
 
 * parksettings must have gates specified (again) changed comments for gate types
```

### Comparing `arivo-settings_models-0.0.1rc5/arivo_settings_models.egg-info/PKG-INFO` & `arivo-settings_models-1.0.0/arivo_settings_models.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arivo-settings-models
-Version: 0.0.1rc5
+Version: 1.0.0
 Summary: Library for arivo parking system settings definitions and models
 Home-page: https://gitlab.com/accessio/onegate/settings-models
 Author: ARIVO
 Author-email: support@arivo.co
 License: "GPL-3",
 Description: # Settings Models
```

### Comparing `arivo-settings_models-0.0.1rc5/arivo_settings_models.egg-info/SOURCES.txt` & `arivo-settings_models-1.0.0/arivo_settings_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

