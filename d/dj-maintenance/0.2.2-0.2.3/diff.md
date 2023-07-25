# Comparing `tmp/dj_maintenance-0.2.2.tar.gz` & `tmp/dj_maintenance-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_maintenance-0.2.2.tar", last modified: Tue Jul 25 10:32:08 2023, max compression
+gzip compressed data, was "dj_maintenance-0.2.3.tar", last modified: Tue Jul 25 10:47:21 2023, max compression
```

## Comparing `dj_maintenance-0.2.2.tar` & `dj_maintenance-0.2.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:32:08.662416 dj_maintenance-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 10:31:53.000000 dj_maintenance-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 10:31:53.000000 dj_maintenance-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-25 10:32:08.662416 dj_maintenance-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-25 10:31:53.000000 dj_maintenance-0.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:32:08.658416 dj_maintenance-0.2.2/dj_maintenance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 10:31:53.000000 dj_maintenance-0.2.2/dj_maintenance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-25 10:31:53.000000 dj_maintenance-0.2.2/dj_maintenance/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-25 10:31:53.000000 dj_maintenance-0.2.2/dj_maintenance/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:32:08.658416 dj_maintenance-0.2.2/dj_maintenance/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 10:31:53.000000 dj_maintenance-0.2.2/dj_maintenance/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-25 10:31:53.000000 dj_maintenance-0.2.2/dj_maintenance/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:32:08.654416 dj_maintenance-0.2.2/dj_maintenance/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:32:08.654416 dj_maintenance-0.2.2/dj_maintenance/static/dj-maintenance/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:32:08.658416 dj_maintenance-0.2.2/dj_maintenance/static/dj-maintenance/images/
--rw-r--r--   0 runner    (1001) docker     (123)  3843590 2023-07-25 10:31:53.000000 dj_maintenance-0.2.2/dj_maintenance/static/dj-maintenance/images/maintenance.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:32:08.654416 dj_maintenance-0.2.2/dj_maintenance/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:32:08.662416 dj_maintenance-0.2.2/dj_maintenance/templates/dj-maintenance/
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-25 10:31:53.000000 dj_maintenance-0.2.2/dj_maintenance/templates/dj-maintenance/index.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-25 10:31:53.000000 dj_maintenance-0.2.2/dj_maintenance/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-25 10:31:53.000000 dj_maintenance-0.2.2/dj_maintenance/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-25 10:31:53.000000 dj_maintenance-0.2.2/dj_maintenance/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:32:08.658416 dj_maintenance-0.2.2/dj_maintenance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-25 10:32:08.000000 dj_maintenance-0.2.2/dj_maintenance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-25 10:32:08.000000 dj_maintenance-0.2.2/dj_maintenance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 10:32:08.000000 dj_maintenance-0.2.2/dj_maintenance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 10:32:08.000000 dj_maintenance-0.2.2/dj_maintenance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-25 10:32:08.000000 dj_maintenance-0.2.2/dj_maintenance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-25 10:31:53.000000 dj_maintenance-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-25 10:32:08.662416 dj_maintenance-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-25 10:31:53.000000 dj_maintenance-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:47:21.388884 dj_maintenance-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 10:47:06.000000 dj_maintenance-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 10:47:06.000000 dj_maintenance-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-25 10:47:21.388884 dj_maintenance-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-25 10:47:06.000000 dj_maintenance-0.2.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:47:21.380884 dj_maintenance-0.2.3/dj_maintenance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 10:47:06.000000 dj_maintenance-0.2.3/dj_maintenance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-25 10:47:06.000000 dj_maintenance-0.2.3/dj_maintenance/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-25 10:47:06.000000 dj_maintenance-0.2.3/dj_maintenance/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:47:21.384884 dj_maintenance-0.2.3/dj_maintenance/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 10:47:06.000000 dj_maintenance-0.2.3/dj_maintenance/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-25 10:47:06.000000 dj_maintenance-0.2.3/dj_maintenance/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:47:21.376884 dj_maintenance-0.2.3/dj_maintenance/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:47:21.380884 dj_maintenance-0.2.3/dj_maintenance/static/dj-maintenance/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:47:21.384884 dj_maintenance-0.2.3/dj_maintenance/static/dj-maintenance/images/
+-rw-r--r--   0 runner    (1001) docker     (123)  3843590 2023-07-25 10:47:06.000000 dj_maintenance-0.2.3/dj_maintenance/static/dj-maintenance/images/maintenance.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:47:21.380884 dj_maintenance-0.2.3/dj_maintenance/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:47:21.388884 dj_maintenance-0.2.3/dj_maintenance/templates/dj-maintenance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-25 10:47:06.000000 dj_maintenance-0.2.3/dj_maintenance/templates/dj-maintenance/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-25 10:47:06.000000 dj_maintenance-0.2.3/dj_maintenance/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-25 10:47:06.000000 dj_maintenance-0.2.3/dj_maintenance/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-25 10:47:06.000000 dj_maintenance-0.2.3/dj_maintenance/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:47:21.384884 dj_maintenance-0.2.3/dj_maintenance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-25 10:47:21.000000 dj_maintenance-0.2.3/dj_maintenance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-25 10:47:21.000000 dj_maintenance-0.2.3/dj_maintenance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 10:47:21.000000 dj_maintenance-0.2.3/dj_maintenance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 10:47:21.000000 dj_maintenance-0.2.3/dj_maintenance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-25 10:47:21.000000 dj_maintenance-0.2.3/dj_maintenance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-25 10:47:06.000000 dj_maintenance-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-25 10:47:21.388884 dj_maintenance-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-25 10:47:06.000000 dj_maintenance-0.2.3/setup.py
```

### Comparing `dj_maintenance-0.2.2/LICENSE` & `dj_maintenance-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_maintenance-0.2.2/PKG-INFO` & `dj_maintenance-0.2.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj_maintenance
-Version: 0.2.2
+Version: 0.2.3
 Summary: A django app to conduct sheduled maintenance.
 Home-page: https://djmaintenance.ayumefrancis.com/
 Author: Ayume Francis
 Author-email: admin@ayumefrancis.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `dj_maintenance-0.2.2/README.rst` & `dj_maintenance-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `dj_maintenance-0.2.2/dj_maintenance/static/dj-maintenance/images/maintenance.gif` & `dj_maintenance-0.2.3/dj_maintenance/static/dj-maintenance/images/maintenance.gif`

 * *Files identical despite different names*

### Comparing `dj_maintenance-0.2.2/dj_maintenance/templates/dj-maintenance/index.html` & `dj_maintenance-0.2.3/dj_maintenance/templates/dj-maintenance/index.html`

 * *Files identical despite different names*

### Comparing `dj_maintenance-0.2.2/dj_maintenance.egg-info/PKG-INFO` & `dj_maintenance-0.2.3/dj_maintenance.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-maintenance
-Version: 0.2.2
+Version: 0.2.3
 Summary: A django app to conduct sheduled maintenance.
 Home-page: https://djmaintenance.ayumefrancis.com/
 Author: Ayume Francis
 Author-email: admin@ayumefrancis.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `dj_maintenance-0.2.2/dj_maintenance.egg-info/SOURCES.txt` & `dj_maintenance-0.2.3/dj_maintenance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj_maintenance-0.2.2/setup.cfg` & `dj_maintenance-0.2.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dj_maintenance
-version = 0.2.2
+version = 0.2.3
 description = A django app to conduct sheduled maintenance.
 long_description_content_type = text/x-rst
 long_description = file: README.rst
 url = https://djmaintenance.ayumefrancis.com/
 author = Ayume Francis
 author_email = admin@ayumefrancis.com
 license = BSD-3-Clause
```

