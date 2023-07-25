# Comparing `tmp/django-simple-health-check-0.5.0.tar.gz` & `tmp/django-simple-health-check-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-simple-health-check-0.5.0.tar", last modified: Mon Jan 16 19:52:29 2023, max compression
+gzip compressed data, was "django-simple-health-check-0.6.0.tar", last modified: Tue Jul 25 12:51:05 2023, max compression
```

## Comparing `django-simple-health-check-0.5.0.tar` & `django-simple-health-check-0.6.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 19:52:29.682941 django-simple-health-check-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-01-16 19:52:21.000000 django-simple-health-check-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-01-16 19:52:21.000000 django-simple-health-check-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-01-16 19:52:29.682941 django-simple-health-check-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-01-16 19:52:21.000000 django-simple-health-check-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 19:52:29.682941 django-simple-health-check-0.5.0/django_simple_health_check.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-01-16 19:52:29.000000 django-simple-health-check-0.5.0/django_simple_health_check.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-01-16 19:52:29.000000 django-simple-health-check-0.5.0/django_simple_health_check.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 19:52:29.000000 django-simple-health-check-0.5.0/django_simple_health_check.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 19:52:29.000000 django-simple-health-check-0.5.0/django_simple_health_check.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-01-16 19:52:29.000000 django-simple-health-check-0.5.0/django_simple_health_check.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-16 19:52:29.000000 django-simple-health-check-0.5.0/django_simple_health_check.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-16 19:52:29.682941 django-simple-health-check-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-01-16 19:52:21.000000 django-simple-health-check-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 19:52:29.682941 django-simple-health-check-0.5.0/simple_health_check/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-16 19:52:21.000000 django-simple-health-check-0.5.0/simple_health_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-01-16 19:52:21.000000 django-simple-health-check-0.5.0/simple_health_check/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 19:52:29.682941 django-simple-health-check-0.5.0/simple_health_check/checks/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-01-16 19:52:21.000000 django-simple-health-check-0.5.0/simple_health_check/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-01-16 19:52:21.000000 django-simple-health-check-0.5.0/simple_health_check/checks/caches.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-16 19:52:21.000000 django-simple-health-check-0.5.0/simple_health_check/checks/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-01-16 19:52:21.000000 django-simple-health-check-0.5.0/simple_health_check/checks/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-01-16 19:52:21.000000 django-simple-health-check-0.5.0/simple_health_check/checks/migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-01-16 19:52:21.000000 django-simple-health-check-0.5.0/simple_health_check/checks/ps.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-16 19:52:21.000000 django-simple-health-check-0.5.0/simple_health_check/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 19:52:29.682941 django-simple-health-check-0.5.0/simple_health_check/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 19:52:21.000000 django-simple-health-check-0.5.0/simple_health_check/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 19:52:21.000000 django-simple-health-check-0.5.0/simple_health_check/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-01-16 19:52:21.000000 django-simple-health-check-0.5.0/simple_health_check/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-01-16 19:52:21.000000 django-simple-health-check-0.5.0/simple_health_check/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-01-16 19:52:21.000000 django-simple-health-check-0.5.0/simple_health_check/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-01-16 19:52:21.000000 django-simple-health-check-0.5.0/simple_health_check/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:51:05.328465 django-simple-health-check-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-25 12:50:53.000000 django-simple-health-check-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-25 12:50:53.000000 django-simple-health-check-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-07-25 12:51:05.328465 django-simple-health-check-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-25 12:50:53.000000 django-simple-health-check-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:51:05.324464 django-simple-health-check-0.6.0/django_simple_health_check.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-07-25 12:51:05.000000 django-simple-health-check-0.6.0/django_simple_health_check.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-25 12:51:05.000000 django-simple-health-check-0.6.0/django_simple_health_check.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 12:51:05.000000 django-simple-health-check-0.6.0/django_simple_health_check.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 12:51:05.000000 django-simple-health-check-0.6.0/django_simple_health_check.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-25 12:51:05.000000 django-simple-health-check-0.6.0/django_simple_health_check.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-25 12:51:05.000000 django-simple-health-check-0.6.0/django_simple_health_check.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 12:51:05.328465 django-simple-health-check-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-25 12:50:53.000000 django-simple-health-check-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:51:05.324464 django-simple-health-check-0.6.0/simple_health_check/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-25 12:50:53.000000 django-simple-health-check-0.6.0/simple_health_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-25 12:50:53.000000 django-simple-health-check-0.6.0/simple_health_check/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:51:05.328465 django-simple-health-check-0.6.0/simple_health_check/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-25 12:50:53.000000 django-simple-health-check-0.6.0/simple_health_check/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-25 12:50:53.000000 django-simple-health-check-0.6.0/simple_health_check/checks/caches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-25 12:50:53.000000 django-simple-health-check-0.6.0/simple_health_check/checks/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-25 12:50:53.000000 django-simple-health-check-0.6.0/simple_health_check/checks/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-25 12:50:53.000000 django-simple-health-check-0.6.0/simple_health_check/checks/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-25 12:50:53.000000 django-simple-health-check-0.6.0/simple_health_check/checks/ps.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-25 12:50:53.000000 django-simple-health-check-0.6.0/simple_health_check/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:51:05.328465 django-simple-health-check-0.6.0/simple_health_check/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 12:50:53.000000 django-simple-health-check-0.6.0/simple_health_check/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 12:50:53.000000 django-simple-health-check-0.6.0/simple_health_check/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-25 12:50:53.000000 django-simple-health-check-0.6.0/simple_health_check/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-07-25 12:50:53.000000 django-simple-health-check-0.6.0/simple_health_check/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-25 12:50:53.000000 django-simple-health-check-0.6.0/simple_health_check/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-25 12:50:53.000000 django-simple-health-check-0.6.0/simple_health_check/views.py
```

### Comparing `django-simple-health-check-0.5.0/LICENSE` & `django-simple-health-check-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-simple-health-check-0.5.0/PKG-INFO` & `django-simple-health-check-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: django-simple-health-check
-Version: 0.5.0
+Version: 0.6.0
 Summary: Simple Django health check
 Home-page: https://github.com/pikhovkin/django-simple-health-check
 Author: Sergei Pikhovkin
 Author-email: s@pikhovkin.ru
 License: MIT
 Keywords: django,monitoring,healthcheck,health-check,ping,health-checks,healthchecks,liveness,readiness,liveness-detection,readiness-checker,django-health-check,readiness-detection,liveness-checker
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7.*, <4.0.*
+Requires-Python: >=3.7,<4.0
 Description-Content-Type: text/markdown
 Provides-Extra: psutil
 License-File: LICENSE
 
 # django-simple-health-check
 
 [![GitHub Actions](https://github.com/pikhovkin/django-simple-health-check/workflows/build/badge.svg)](https://github.com/pikhovkin/django-simple-health-check/actions)
```

### Comparing `django-simple-health-check-0.5.0/README.md` & `django-simple-health-check-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `django-simple-health-check-0.5.0/django_simple_health_check.egg-info/PKG-INFO` & `django-simple-health-check-0.6.0/django_simple_health_check.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: django-simple-health-check
-Version: 0.5.0
+Version: 0.6.0
 Summary: Simple Django health check
 Home-page: https://github.com/pikhovkin/django-simple-health-check
 Author: Sergei Pikhovkin
 Author-email: s@pikhovkin.ru
 License: MIT
 Keywords: django,monitoring,healthcheck,health-check,ping,health-checks,healthchecks,liveness,readiness,liveness-detection,readiness-checker,django-health-check,readiness-detection,liveness-checker
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7.*, <4.0.*
+Requires-Python: >=3.7,<4.0
 Description-Content-Type: text/markdown
 Provides-Extra: psutil
 License-File: LICENSE
 
 # django-simple-health-check
 
 [![GitHub Actions](https://github.com/pikhovkin/django-simple-health-check/workflows/build/badge.svg)](https://github.com/pikhovkin/django-simple-health-check/actions)
```

### Comparing `django-simple-health-check-0.5.0/django_simple_health_check.egg-info/SOURCES.txt` & `django-simple-health-check-0.6.0/django_simple_health_check.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-simple-health-check-0.5.0/setup.py` & `django-simple-health-check-0.6.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,41 +3,42 @@
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
 
 setup(
     name='django-simple-health-check',
-    version='0.5.0',
+    version='0.6.0',
     description='Simple Django health check',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Sergei Pikhovkin',
     author_email='s@pikhovkin.ru',
     url='https://github.com/pikhovkin/django-simple-health-check',
     packages=[
         'simple_health_check',
     ],
     include_package_data=True,
     install_requires=[
-        'Django>=3.1,<4.2',
+        'Django>=3.1,<4.3',
     ],
     extras_require={
         'psutil': ['psutil'],
     },
-    python_requires='>=3.7.*, <4.0.*',
+    python_requires='>=3.7,<4.0',
     license='MIT',
     zip_safe=False,
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Environment :: Web Environment',
         'Framework :: Django :: 3.1',
         'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.0',
         'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
```

### Comparing `django-simple-health-check-0.5.0/simple_health_check/apps.py` & `django-simple-health-check-0.6.0/simple_health_check/apps.py`

 * *Files identical despite different names*

### Comparing `django-simple-health-check-0.5.0/simple_health_check/checks/caches.py` & `django-simple-health-check-0.6.0/simple_health_check/checks/caches.py`

 * *Files identical despite different names*

### Comparing `django-simple-health-check-0.5.0/simple_health_check/checks/db.py` & `django-simple-health-check-0.6.0/simple_health_check/checks/db.py`

 * *Files identical despite different names*

### Comparing `django-simple-health-check-0.5.0/simple_health_check/checks/migrations.py` & `django-simple-health-check-0.6.0/simple_health_check/checks/migrations.py`

 * *Files identical despite different names*

### Comparing `django-simple-health-check-0.5.0/simple_health_check/checks/ps.py` & `django-simple-health-check-0.6.0/simple_health_check/checks/ps.py`

 * *Files identical despite different names*

### Comparing `django-simple-health-check-0.5.0/simple_health_check/tests.py` & `django-simple-health-check-0.6.0/simple_health_check/tests.py`

 * *Files identical despite different names*

### Comparing `django-simple-health-check-0.5.0/simple_health_check/views.py` & `django-simple-health-check-0.6.0/simple_health_check/views.py`

 * *Files identical despite different names*

