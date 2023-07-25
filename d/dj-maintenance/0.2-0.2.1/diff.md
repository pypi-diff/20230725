# Comparing `tmp/dj-maintenance-0.2.tar.gz` & `tmp/dj_maintenance-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-maintenance-0.2.tar", last modified: Tue Jul 25 09:37:23 2023, max compression
+gzip compressed data, was "dj_maintenance-0.2.1.tar", last modified: Tue Jul 25 10:06:23 2023, max compression
```

## Comparing `dj-maintenance-0.2.tar` & `dj_maintenance-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:37:23.741620 dj-maintenance-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 09:37:12.000000 dj-maintenance-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 09:37:12.000000 dj-maintenance-0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-25 09:37:23.741620 dj-maintenance-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-25 09:37:12.000000 dj-maintenance-0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:37:23.737620 dj-maintenance-0.2/dj-maintenance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:37:12.000000 dj-maintenance-0.2/dj-maintenance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-25 09:37:12.000000 dj-maintenance-0.2/dj-maintenance/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-25 09:37:12.000000 dj-maintenance-0.2/dj-maintenance/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:37:23.737620 dj-maintenance-0.2/dj-maintenance/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:37:12.000000 dj-maintenance-0.2/dj-maintenance/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-25 09:37:12.000000 dj-maintenance-0.2/dj-maintenance/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:37:23.733620 dj-maintenance-0.2/dj-maintenance/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:37:23.733620 dj-maintenance-0.2/dj-maintenance/static/dj-maintenance/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:37:23.737620 dj-maintenance-0.2/dj-maintenance/static/dj-maintenance/images/
--rw-r--r--   0 runner    (1001) docker     (123)  3843590 2023-07-25 09:37:12.000000 dj-maintenance-0.2/dj-maintenance/static/dj-maintenance/images/maintenance.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:37:23.733620 dj-maintenance-0.2/dj-maintenance/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:37:23.741620 dj-maintenance-0.2/dj-maintenance/templates/dj-maintenance/
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-25 09:37:12.000000 dj-maintenance-0.2/dj-maintenance/templates/dj-maintenance/index.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-25 09:37:12.000000 dj-maintenance-0.2/dj-maintenance/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-25 09:37:12.000000 dj-maintenance-0.2/dj-maintenance/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-25 09:37:12.000000 dj-maintenance-0.2/dj-maintenance/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:37:23.741620 dj-maintenance-0.2/dj_maintenance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-25 09:37:23.000000 dj-maintenance-0.2/dj_maintenance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-25 09:37:23.000000 dj-maintenance-0.2/dj_maintenance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 09:37:23.000000 dj-maintenance-0.2/dj_maintenance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 09:37:23.000000 dj-maintenance-0.2/dj_maintenance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-25 09:37:23.000000 dj-maintenance-0.2/dj_maintenance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-25 09:37:12.000000 dj-maintenance-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-25 09:37:23.741620 dj-maintenance-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-25 09:37:12.000000 dj-maintenance-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:06:23.849029 dj_maintenance-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 10:06:07.000000 dj_maintenance-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 10:06:07.000000 dj_maintenance-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-25 10:06:23.849029 dj_maintenance-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-25 10:06:07.000000 dj_maintenance-0.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:06:23.845029 dj_maintenance-0.2.1/dj_maintenance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 10:06:07.000000 dj_maintenance-0.2.1/dj_maintenance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-25 10:06:07.000000 dj_maintenance-0.2.1/dj_maintenance/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-25 10:06:07.000000 dj_maintenance-0.2.1/dj_maintenance/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:06:23.849029 dj_maintenance-0.2.1/dj_maintenance/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 10:06:07.000000 dj_maintenance-0.2.1/dj_maintenance/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-25 10:06:07.000000 dj_maintenance-0.2.1/dj_maintenance/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-25 10:06:07.000000 dj_maintenance-0.2.1/dj_maintenance/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-25 10:06:07.000000 dj_maintenance-0.2.1/dj_maintenance/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-25 10:06:07.000000 dj_maintenance-0.2.1/dj_maintenance/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:06:23.849029 dj_maintenance-0.2.1/dj_maintenance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-25 10:06:23.000000 dj_maintenance-0.2.1/dj_maintenance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-25 10:06:23.000000 dj_maintenance-0.2.1/dj_maintenance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 10:06:23.000000 dj_maintenance-0.2.1/dj_maintenance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 10:06:23.000000 dj_maintenance-0.2.1/dj_maintenance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-25 10:06:23.000000 dj_maintenance-0.2.1/dj_maintenance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-25 10:06:07.000000 dj_maintenance-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-25 10:06:23.849029 dj_maintenance-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-25 10:06:07.000000 dj_maintenance-0.2.1/setup.py
```

### Comparing `dj-maintenance-0.2/LICENSE` & `dj_maintenance-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dj-maintenance-0.2/PKG-INFO` & `dj_maintenance-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: dj-maintenance
-Version: 0.2
+Name: dj_maintenance
+Version: 0.2.1
 Summary: A django app to conduct sheduled maintenance.
 Home-page: https://djmaintenance.ayumefrancis.com/
 Author: Ayume Francis
-Author-email: admin@ayumefrancis.com
+Author-email: ayudmin <admin@ayumefrancis.com>
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -19,8 +19,8 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-dj-dj-dj-maintenance is a Django app to conduct sheduled dj-dj-maintenance on your web application. Detailed documentation is in the 'docs' directory.
+dj_maintenance is a Django app to conduct sheduled dj-dj_maintenance on your web application. Detailed documentation is in the 'docs' directory.
```

### Comparing `dj-maintenance-0.2/README.rst` & `dj_maintenance-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `dj-maintenance-0.2/dj_maintenance.egg-info/PKG-INFO` & `dj_maintenance-0.2.1/dj_maintenance.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: dj-maintenance
-Version: 0.2
+Version: 0.2.1
 Summary: A django app to conduct sheduled maintenance.
 Home-page: https://djmaintenance.ayumefrancis.com/
 Author: Ayume Francis
-Author-email: admin@ayumefrancis.com
+Author-email: ayudmin <admin@ayumefrancis.com>
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -19,8 +19,8 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-dj-dj-dj-maintenance is a Django app to conduct sheduled dj-dj-maintenance on your web application. Detailed documentation is in the 'docs' directory.
+dj_maintenance is a Django app to conduct sheduled dj-dj_maintenance on your web application. Detailed documentation is in the 'docs' directory.
```

### Comparing `dj-maintenance-0.2/setup.cfg` & `dj_maintenance-0.2.1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
-name = dj-maintenance
-version = 0.2
+name = dj_maintenance
+version = 0.2.1
 description = A django app to conduct sheduled maintenance.
 long_description_content_type = text/x-rst
 long_description = file: README.rst
 url = https://djmaintenance.ayumefrancis.com/
 author = Ayume Francis
 author_email = admin@ayumefrancis.com
 license = BSD-3-Clause
```

