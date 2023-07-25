# Comparing `tmp/dj_maintenance-0.1.tar.gz` & `tmp/dj-maintenance-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_maintenance-0.1.tar", last modified: Tue Jul 25 08:12:50 2023, max compression
+gzip compressed data, was "dj-maintenance-0.2.tar", last modified: Tue Jul 25 09:37:23 2023, max compression
```

## Comparing `dj_maintenance-0.1.tar` & `dj-maintenance-0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 francis   (1000) francis   (1000)        0 2023-07-25 08:12:50.154518 dj_maintenance-0.1/
--rw-rw-r--   0 francis   (1000) francis   (1000)    35149 2023-07-21 06:53:09.000000 dj_maintenance-0.1/LICENSE
--rw-rw-r--   0 francis   (1000) francis   (1000)      156 2023-07-22 06:55:35.000000 dj_maintenance-0.1/MANIFEST.in
--rw-rw-r--   0 francis   (1000) francis   (1000)     1069 2023-07-25 08:12:50.154518 dj_maintenance-0.1/PKG-INFO
--rw-rw-r--   0 francis   (1000) francis   (1000)      747 2023-07-22 07:05:36.000000 dj_maintenance-0.1/README.rst
-drwxrwxr-x   0 francis   (1000) francis   (1000)        0 2023-07-25 08:12:50.146517 dj_maintenance-0.1/dj_maintenance.egg-info/
--rw-rw-r--   0 francis   (1000) francis   (1000)     1069 2023-07-25 08:12:50.000000 dj_maintenance-0.1/dj_maintenance.egg-info/PKG-INFO
--rw-rw-r--   0 francis   (1000) francis   (1000)      606 2023-07-25 08:12:50.000000 dj_maintenance-0.1/dj_maintenance.egg-info/SOURCES.txt
--rw-rw-r--   0 francis   (1000) francis   (1000)        1 2023-07-25 08:12:50.000000 dj_maintenance-0.1/dj_maintenance.egg-info/dependency_links.txt
--rw-rw-r--   0 francis   (1000) francis   (1000)       12 2023-07-25 08:12:50.000000 dj_maintenance-0.1/dj_maintenance.egg-info/requires.txt
--rw-rw-r--   0 francis   (1000) francis   (1000)       19 2023-07-25 08:12:50.000000 dj_maintenance-0.1/dj_maintenance.egg-info/top_level.txt
-drwxrwxr-x   0 francis   (1000) francis   (1000)        0 2023-07-25 08:12:50.150517 dj_maintenance-0.1/django_maintenance/
--rw-rw-r--   0 francis   (1000) francis   (1000)        0 2023-07-17 13:43:45.000000 dj_maintenance-0.1/django_maintenance/__init__.py
--rw-rw-r--   0 francis   (1000) francis   (1000)       63 2023-07-17 13:43:45.000000 dj_maintenance-0.1/django_maintenance/admin.py
--rw-rw-r--   0 francis   (1000) francis   (1000)      154 2023-07-17 13:43:45.000000 dj_maintenance-0.1/django_maintenance/apps.py
-drwxrwxr-x   0 francis   (1000) francis   (1000)        0 2023-07-25 08:12:50.150517 dj_maintenance-0.1/django_maintenance/migrations/
--rw-rw-r--   0 francis   (1000) francis   (1000)        0 2023-07-17 13:43:45.000000 dj_maintenance-0.1/django_maintenance/migrations/__init__.py
--rw-rw-r--   0 francis   (1000) francis   (1000)       57 2023-07-17 13:43:45.000000 dj_maintenance-0.1/django_maintenance/models.py
-drwxrwxr-x   0 francis   (1000) francis   (1000)        0 2023-07-25 08:12:50.146517 dj_maintenance-0.1/django_maintenance/static/
-drwxrwxr-x   0 francis   (1000) francis   (1000)        0 2023-07-25 08:12:50.146517 dj_maintenance-0.1/django_maintenance/static/maintenance/
-drwxrwxr-x   0 francis   (1000) francis   (1000)        0 2023-07-25 08:12:50.150517 dj_maintenance-0.1/django_maintenance/static/maintenance/images/
--rw-rw-r--   0 francis   (1000) francis   (1000)  3843590 2023-07-17 13:53:13.000000 dj_maintenance-0.1/django_maintenance/static/maintenance/images/maintenance.gif
-drwxrwxr-x   0 francis   (1000) francis   (1000)        0 2023-07-25 08:12:50.146517 dj_maintenance-0.1/django_maintenance/templates/
-drwxrwxr-x   0 francis   (1000) francis   (1000)        0 2023-07-25 08:12:50.154518 dj_maintenance-0.1/django_maintenance/templates/maintenance/
--rw-rw-r--   0 francis   (1000) francis   (1000)     1265 2023-07-21 06:30:44.000000 dj_maintenance-0.1/django_maintenance/templates/maintenance/index.html
--rw-rw-r--   0 francis   (1000) francis   (1000)       60 2023-07-17 13:43:45.000000 dj_maintenance-0.1/django_maintenance/tests.py
--rw-rw-r--   0 francis   (1000) francis   (1000)      206 2023-07-21 07:25:45.000000 dj_maintenance-0.1/django_maintenance/urls.py
--rw-rw-r--   0 francis   (1000) francis   (1000)      126 2023-07-18 15:58:06.000000 dj_maintenance-0.1/django_maintenance/views.py
--rw-rw-r--   0 francis   (1000) francis   (1000)       89 2023-07-21 05:13:18.000000 dj_maintenance-0.1/pyproject.toml
--rw-rw-r--   0 francis   (1000) francis   (1000)      943 2023-07-25 08:12:50.154518 dj_maintenance-0.1/setup.cfg
--rw-rw-r--   0 francis   (1000) francis   (1000)      203 2023-07-25 07:57:32.000000 dj_maintenance-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:37:23.741620 dj-maintenance-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 09:37:12.000000 dj-maintenance-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 09:37:12.000000 dj-maintenance-0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-25 09:37:23.741620 dj-maintenance-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-25 09:37:12.000000 dj-maintenance-0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:37:23.737620 dj-maintenance-0.2/dj-maintenance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:37:12.000000 dj-maintenance-0.2/dj-maintenance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-25 09:37:12.000000 dj-maintenance-0.2/dj-maintenance/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-25 09:37:12.000000 dj-maintenance-0.2/dj-maintenance/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:37:23.737620 dj-maintenance-0.2/dj-maintenance/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:37:12.000000 dj-maintenance-0.2/dj-maintenance/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-25 09:37:12.000000 dj-maintenance-0.2/dj-maintenance/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:37:23.733620 dj-maintenance-0.2/dj-maintenance/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:37:23.733620 dj-maintenance-0.2/dj-maintenance/static/dj-maintenance/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:37:23.737620 dj-maintenance-0.2/dj-maintenance/static/dj-maintenance/images/
+-rw-r--r--   0 runner    (1001) docker     (123)  3843590 2023-07-25 09:37:12.000000 dj-maintenance-0.2/dj-maintenance/static/dj-maintenance/images/maintenance.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:37:23.733620 dj-maintenance-0.2/dj-maintenance/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:37:23.741620 dj-maintenance-0.2/dj-maintenance/templates/dj-maintenance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-25 09:37:12.000000 dj-maintenance-0.2/dj-maintenance/templates/dj-maintenance/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-25 09:37:12.000000 dj-maintenance-0.2/dj-maintenance/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-25 09:37:12.000000 dj-maintenance-0.2/dj-maintenance/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-25 09:37:12.000000 dj-maintenance-0.2/dj-maintenance/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:37:23.741620 dj-maintenance-0.2/dj_maintenance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-25 09:37:23.000000 dj-maintenance-0.2/dj_maintenance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-25 09:37:23.000000 dj-maintenance-0.2/dj_maintenance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 09:37:23.000000 dj-maintenance-0.2/dj_maintenance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 09:37:23.000000 dj-maintenance-0.2/dj_maintenance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-25 09:37:23.000000 dj-maintenance-0.2/dj_maintenance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-25 09:37:12.000000 dj-maintenance-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-25 09:37:23.741620 dj-maintenance-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-25 09:37:12.000000 dj-maintenance-0.2/setup.py
```

### Comparing `dj_maintenance-0.1/LICENSE` & `dj-maintenance-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_maintenance-0.1/PKG-INFO` & `dj-maintenance-0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: dj_maintenance
-Version: 0.1
-Summary: A Django app to conduct sheduled maintenance.
-Home-page: https://projects.ayumefrancis.com/
+Name: dj-maintenance
+Version: 0.2
+Summary: A django app to conduct sheduled maintenance.
+Home-page: https://djmaintenance.ayumefrancis.com/
 Author: Ayume Francis
 Author-email: admin@ayumefrancis.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
@@ -19,8 +19,8 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-django_maintenance is a Django app to conduct sheduled maintenance on your web application.Detailed documentation is in the 'docs' directory.
+dj-dj-dj-maintenance is a Django app to conduct sheduled dj-dj-maintenance on your web application. Detailed documentation is in the 'docs' directory.
```

### Comparing `dj_maintenance-0.1/README.rst` & `dj-maintenance-0.2/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 =====
-Django_maintenance
+dj-maintenance
 =====
 
 Django_maintenance is a Django app to conduct sheduled maintenance on your web application.
 Detailed documentation is in the "docs" directory.
 
 Quick start
 -----------
 
 1. Add "django_maintenance" to your INSTALLED_APPS setting like this::
 
     INSTALLED_APPS = [
         ...,
-        "django_maintenance",
+        "dj-maintenance",
     ]
 
 2. Add maintenance_mode variable to base or settings::
 
     MAINTENANCE_MODE = bool(os.getenv('MAINTENANCE_MODE'))
 
 3. Update the URLconf in your project urls.py like this::
 
     if base.MAINTENANCE_MODE:
-        path("", include("django_maintenance.urls")),
+        path("", include("dj-maintenance.urls")),
     else:
         # All project URLconf
     # static URLconf
     # others ..
 
 4. Run ``python manage.py migrate`` to create the polls models.
```

### Comparing `dj_maintenance-0.1/dj_maintenance.egg-info/PKG-INFO` & `dj-maintenance-0.2/dj_maintenance.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dj-maintenance
-Version: 0.1
-Summary: A Django app to conduct sheduled maintenance.
-Home-page: https://projects.ayumefrancis.com/
+Version: 0.2
+Summary: A django app to conduct sheduled maintenance.
+Home-page: https://djmaintenance.ayumefrancis.com/
 Author: Ayume Francis
 Author-email: admin@ayumefrancis.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
@@ -19,8 +19,8 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-django_maintenance is a Django app to conduct sheduled maintenance on your web application.Detailed documentation is in the 'docs' directory.
+dj-dj-dj-maintenance is a Django app to conduct sheduled dj-dj-maintenance on your web application. Detailed documentation is in the 'docs' directory.
```

### Comparing `dj_maintenance-0.1/dj_maintenance.egg-info/SOURCES.txt` & `dj-maintenance-0.2/dj_maintenance.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
+dj-maintenance/__init__.py
+dj-maintenance/admin.py
+dj-maintenance/apps.py
+dj-maintenance/models.py
+dj-maintenance/tests.py
+dj-maintenance/urls.py
+dj-maintenance/views.py
+dj-maintenance/migrations/__init__.py
+dj-maintenance/static/dj-maintenance/images/maintenance.gif
+dj-maintenance/templates/dj-maintenance/index.html
 dj_maintenance.egg-info/PKG-INFO
 dj_maintenance.egg-info/SOURCES.txt
 dj_maintenance.egg-info/dependency_links.txt
 dj_maintenance.egg-info/requires.txt
-dj_maintenance.egg-info/top_level.txt
-django_maintenance/__init__.py
-django_maintenance/admin.py
-django_maintenance/apps.py
-django_maintenance/models.py
-django_maintenance/tests.py
-django_maintenance/urls.py
-django_maintenance/views.py
-django_maintenance/migrations/__init__.py
-django_maintenance/static/maintenance/images/maintenance.gif
-django_maintenance/templates/maintenance/index.html
+dj_maintenance.egg-info/top_level.txt
```

### Comparing `dj_maintenance-0.1/django_maintenance/static/maintenance/images/maintenance.gif` & `dj-maintenance-0.2/dj-maintenance/static/dj-maintenance/images/maintenance.gif`

 * *Files identical despite different names*

### Comparing `dj_maintenance-0.1/django_maintenance/templates/maintenance/index.html` & `dj-maintenance-0.2/dj-maintenance/templates/dj-maintenance/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -39,13 +39,13 @@
     }
 </style>
 <body>
     <section class="alert">
         <h1><underline>website Under maintenance</underline></h1>
         <p>Our website is currently undergoing <span style="color: green;">sheduled maintenance</span></p>
         <p>We should be back shortly. Thank you for your patience</p>
-        <img src="{% static 'maintenance/images/maintenance.gif' %}" width="500"  alt="">
+        <img src="{% static 'dj-maintenance/images/maintenance.gif' %}" width="500"  alt="">
         <h3>Application Id: DA-11542</h3>
     </section>
 
 </body>
 </html>
```

### Comparing `dj_maintenance-0.1/setup.cfg` & `dj-maintenance-0.2/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
-name = dj_maintenance
-version = 0.1
-description = A Django app to conduct sheduled maintenance.
+name = dj-maintenance
+version = 0.2
+description = A django app to conduct sheduled maintenance.
 long_description_content_type = text/x-rst
 long_description = file: README.rst
-url = https://projects.ayumefrancis.com/
+url = https://djmaintenance.ayumefrancis.com/
 author = Ayume Francis
 author_email = admin@ayumefrancis.com
 license = BSD-3-Clause
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 4.2
```

