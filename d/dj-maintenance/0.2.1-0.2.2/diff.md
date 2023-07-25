# Comparing `tmp/dj_maintenance-0.2.1.tar.gz` & `tmp/dj_maintenance-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_maintenance-0.2.1.tar", last modified: Tue Jul 25 10:06:23 2023, max compression
+gzip compressed data, was "dj_maintenance-0.2.2.tar", last modified: Tue Jul 25 10:32:08 2023, max compression
```

## Comparing `dj_maintenance-0.2.1.tar` & `dj_maintenance-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:06:23.849029 dj_maintenance-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 10:06:07.000000 dj_maintenance-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 10:06:07.000000 dj_maintenance-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-25 10:06:23.849029 dj_maintenance-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-25 10:06:07.000000 dj_maintenance-0.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:06:23.845029 dj_maintenance-0.2.1/dj_maintenance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 10:06:07.000000 dj_maintenance-0.2.1/dj_maintenance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-25 10:06:07.000000 dj_maintenance-0.2.1/dj_maintenance/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-25 10:06:07.000000 dj_maintenance-0.2.1/dj_maintenance/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:06:23.849029 dj_maintenance-0.2.1/dj_maintenance/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 10:06:07.000000 dj_maintenance-0.2.1/dj_maintenance/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-25 10:06:07.000000 dj_maintenance-0.2.1/dj_maintenance/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-25 10:06:07.000000 dj_maintenance-0.2.1/dj_maintenance/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-25 10:06:07.000000 dj_maintenance-0.2.1/dj_maintenance/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-25 10:06:07.000000 dj_maintenance-0.2.1/dj_maintenance/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:06:23.849029 dj_maintenance-0.2.1/dj_maintenance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-25 10:06:23.000000 dj_maintenance-0.2.1/dj_maintenance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-25 10:06:23.000000 dj_maintenance-0.2.1/dj_maintenance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 10:06:23.000000 dj_maintenance-0.2.1/dj_maintenance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 10:06:23.000000 dj_maintenance-0.2.1/dj_maintenance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-25 10:06:23.000000 dj_maintenance-0.2.1/dj_maintenance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-25 10:06:07.000000 dj_maintenance-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-25 10:06:23.849029 dj_maintenance-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-25 10:06:07.000000 dj_maintenance-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:32:08.662416 dj_maintenance-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 10:31:53.000000 dj_maintenance-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 10:31:53.000000 dj_maintenance-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-25 10:32:08.662416 dj_maintenance-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-25 10:31:53.000000 dj_maintenance-0.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:32:08.658416 dj_maintenance-0.2.2/dj_maintenance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 10:31:53.000000 dj_maintenance-0.2.2/dj_maintenance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-25 10:31:53.000000 dj_maintenance-0.2.2/dj_maintenance/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-25 10:31:53.000000 dj_maintenance-0.2.2/dj_maintenance/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:32:08.658416 dj_maintenance-0.2.2/dj_maintenance/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 10:31:53.000000 dj_maintenance-0.2.2/dj_maintenance/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-25 10:31:53.000000 dj_maintenance-0.2.2/dj_maintenance/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:32:08.654416 dj_maintenance-0.2.2/dj_maintenance/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:32:08.654416 dj_maintenance-0.2.2/dj_maintenance/static/dj-maintenance/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:32:08.658416 dj_maintenance-0.2.2/dj_maintenance/static/dj-maintenance/images/
+-rw-r--r--   0 runner    (1001) docker     (123)  3843590 2023-07-25 10:31:53.000000 dj_maintenance-0.2.2/dj_maintenance/static/dj-maintenance/images/maintenance.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:32:08.654416 dj_maintenance-0.2.2/dj_maintenance/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:32:08.662416 dj_maintenance-0.2.2/dj_maintenance/templates/dj-maintenance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-25 10:31:53.000000 dj_maintenance-0.2.2/dj_maintenance/templates/dj-maintenance/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-25 10:31:53.000000 dj_maintenance-0.2.2/dj_maintenance/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-25 10:31:53.000000 dj_maintenance-0.2.2/dj_maintenance/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-25 10:31:53.000000 dj_maintenance-0.2.2/dj_maintenance/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:32:08.658416 dj_maintenance-0.2.2/dj_maintenance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-25 10:32:08.000000 dj_maintenance-0.2.2/dj_maintenance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-25 10:32:08.000000 dj_maintenance-0.2.2/dj_maintenance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 10:32:08.000000 dj_maintenance-0.2.2/dj_maintenance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 10:32:08.000000 dj_maintenance-0.2.2/dj_maintenance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-25 10:32:08.000000 dj_maintenance-0.2.2/dj_maintenance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-25 10:31:53.000000 dj_maintenance-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-25 10:32:08.662416 dj_maintenance-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-25 10:31:53.000000 dj_maintenance-0.2.2/setup.py
```

### Comparing `dj_maintenance-0.2.1/LICENSE` & `dj_maintenance-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_maintenance-0.2.1/PKG-INFO` & `dj_maintenance-0.2.2/dj_maintenance.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: dj_maintenance
-Version: 0.2.1
+Name: dj-maintenance
+Version: 0.2.2
 Summary: A django app to conduct sheduled maintenance.
 Home-page: https://djmaintenance.ayumefrancis.com/
 Author: Ayume Francis
-Author-email: ayudmin <admin@ayumefrancis.com>
+Author-email: admin@ayumefrancis.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `dj_maintenance-0.2.1/README.rst` & `dj_maintenance-0.2.2/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 =====
-dj-maintenance
+dj_maintenance
 =====
 
 Django_maintenance is a Django app to conduct sheduled maintenance on your web application.
 Detailed documentation is in the "docs" directory.
 
 Quick start
 -----------
 
 1. Add "django_maintenance" to your INSTALLED_APPS setting like this::
 
     INSTALLED_APPS = [
         ...,
-        "dj-maintenance",
+        "dj_maintenance",
     ]
 
 2. Add maintenance_mode variable to base or settings::
 
     MAINTENANCE_MODE = bool(os.getenv('MAINTENANCE_MODE'))
 
 3. Update the URLconf in your project urls.py like this::
 
     if base.MAINTENANCE_MODE:
-        path("", include("dj-maintenance.urls")),
+        path("", include("dj_maintenance.urls")),
     else:
         # All project URLconf
     # static URLconf
     # others ..
 
 4. Run ``python manage.py migrate`` to create the polls models.
```

### Comparing `dj_maintenance-0.2.1/dj_maintenance.egg-info/PKG-INFO` & `dj_maintenance-0.2.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: dj-maintenance
-Version: 0.2.1
+Name: dj_maintenance
+Version: 0.2.2
 Summary: A django app to conduct sheduled maintenance.
 Home-page: https://djmaintenance.ayumefrancis.com/
 Author: Ayume Francis
-Author-email: ayudmin <admin@ayumefrancis.com>
+Author-email: admin@ayumefrancis.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `dj_maintenance-0.2.1/setup.cfg` & `dj_maintenance-0.2.2/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dj_maintenance
-version = 0.2.1
+version = 0.2.2
 description = A django app to conduct sheduled maintenance.
 long_description_content_type = text/x-rst
 long_description = file: README.rst
 url = https://djmaintenance.ayumefrancis.com/
 author = Ayume Francis
 author_email = admin@ayumefrancis.com
 license = BSD-3-Clause
```

