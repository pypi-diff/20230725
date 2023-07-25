# Comparing `tmp/django-viewwork-0.7.0.tar.gz` & `tmp/django-viewwork-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-viewwork-0.7.0.tar", last modified: Tue Jan 17 20:25:23 2023, max compression
+gzip compressed data, was "django-viewwork-0.8.0.tar", last modified: Tue Jul 25 13:01:06 2023, max compression
```

## Comparing `django-viewwork-0.7.0.tar` & `django-viewwork-0.8.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:25:23.515596 django-viewwork-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-01-17 20:25:14.000000 django-viewwork-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-01-17 20:25:14.000000 django-viewwork-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-01-17 20:25:23.515596 django-viewwork-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-01-17 20:25:14.000000 django-viewwork-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:25:23.511595 django-viewwork-0.7.0/django_viewwork.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-01-17 20:25:23.000000 django-viewwork-0.7.0/django_viewwork.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-01-17 20:25:23.000000 django-viewwork-0.7.0/django_viewwork.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 20:25:23.000000 django-viewwork-0.7.0/django_viewwork.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 20:25:23.000000 django-viewwork-0.7.0/django_viewwork.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-01-17 20:25:23.000000 django-viewwork-0.7.0/django_viewwork.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-17 20:25:23.000000 django-viewwork-0.7.0/django_viewwork.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:25:23.511595 django-viewwork-0.7.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-17 20:25:14.000000 django-viewwork-0.7.0/requirements/all.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-17 20:25:14.000000 django-viewwork-0.7.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-17 20:25:14.000000 django-viewwork-0.7.0/requirements/select2.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 20:25:23.515596 django-viewwork-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-01-17 20:25:14.000000 django-viewwork-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:25:23.511595 django-viewwork-0.7.0/viewwork/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-01-17 20:25:14.000000 django-viewwork-0.7.0/viewwork/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-01-17 20:25:14.000000 django-viewwork-0.7.0/viewwork/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-01-17 20:25:14.000000 django-viewwork-0.7.0/viewwork/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-01-17 20:25:14.000000 django-viewwork-0.7.0/viewwork/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:25:23.507595 django-viewwork-0.7.0/viewwork/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:25:23.507595 django-viewwork-0.7.0/viewwork/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:25:23.511595 django-viewwork-0.7.0/viewwork/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-01-17 20:25:14.000000 django-viewwork-0.7.0/viewwork/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-01-17 20:25:14.000000 django-viewwork-0.7.0/viewwork/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:25:23.507595 django-viewwork-0.7.0/viewwork/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:25:23.515596 django-viewwork-0.7.0/viewwork/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-01-17 20:25:14.000000 django-viewwork-0.7.0/viewwork/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-01-17 20:25:14.000000 django-viewwork-0.7.0/viewwork/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:25:23.515596 django-viewwork-0.7.0/viewwork/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 20:25:14.000000 django-viewwork-0.7.0/viewwork/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:25:23.515596 django-viewwork-0.7.0/viewwork/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 20:25:14.000000 django-viewwork-0.7.0/viewwork/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-01-17 20:25:14.000000 django-viewwork-0.7.0/viewwork/management/commands/vw_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-01-17 20:25:14.000000 django-viewwork-0.7.0/viewwork/metaclass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:25:23.515596 django-viewwork-0.7.0/viewwork/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-01-17 20:25:14.000000 django-viewwork-0.7.0/viewwork/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-01-17 20:25:14.000000 django-viewwork-0.7.0/viewwork/migrations/0002_auto_20210709_1622.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-01-17 20:25:14.000000 django-viewwork-0.7.0/viewwork/migrations/0003_menu_i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-01-17 20:25:14.000000 django-viewwork-0.7.0/viewwork/migrations/0004_enabled_hidden.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-01-17 20:25:14.000000 django-viewwork-0.7.0/viewwork/migrations/0005_fix_view_name.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 20:25:14.000000 django-viewwork-0.7.0/viewwork/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-01-17 20:25:14.000000 django-viewwork-0.7.0/viewwork/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-01-17 20:25:14.000000 django-viewwork-0.7.0/viewwork/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-01-17 20:25:14.000000 django-viewwork-0.7.0/viewwork/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-01-17 20:25:14.000000 django-viewwork-0.7.0/viewwork/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-01-17 20:25:14.000000 django-viewwork-0.7.0/viewwork/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:01:06.302429 django-viewwork-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-25 13:00:55.000000 django-viewwork-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-25 13:00:55.000000 django-viewwork-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-25 13:01:06.302429 django-viewwork-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-25 13:00:55.000000 django-viewwork-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:01:06.302429 django-viewwork-0.8.0/django_viewwork.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-25 13:01:06.000000 django-viewwork-0.8.0/django_viewwork.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-25 13:01:06.000000 django-viewwork-0.8.0/django_viewwork.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 13:01:06.000000 django-viewwork-0.8.0/django_viewwork.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 13:01:06.000000 django-viewwork-0.8.0/django_viewwork.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-25 13:01:06.000000 django-viewwork-0.8.0/django_viewwork.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 13:01:06.000000 django-viewwork-0.8.0/django_viewwork.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:01:06.302429 django-viewwork-0.8.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-25 13:00:55.000000 django-viewwork-0.8.0/requirements/all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-25 13:00:55.000000 django-viewwork-0.8.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-25 13:00:55.000000 django-viewwork-0.8.0/requirements/select2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 13:01:06.302429 django-viewwork-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-25 13:00:55.000000 django-viewwork-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:01:06.302429 django-viewwork-0.8.0/viewwork/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-25 13:00:55.000000 django-viewwork-0.8.0/viewwork/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-25 13:00:55.000000 django-viewwork-0.8.0/viewwork/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-25 13:00:55.000000 django-viewwork-0.8.0/viewwork/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-25 13:00:55.000000 django-viewwork-0.8.0/viewwork/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:01:06.302429 django-viewwork-0.8.0/viewwork/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:01:06.302429 django-viewwork-0.8.0/viewwork/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:01:06.302429 django-viewwork-0.8.0/viewwork/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-25 13:00:55.000000 django-viewwork-0.8.0/viewwork/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-25 13:00:55.000000 django-viewwork-0.8.0/viewwork/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:01:06.302429 django-viewwork-0.8.0/viewwork/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:01:06.302429 django-viewwork-0.8.0/viewwork/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-25 13:00:55.000000 django-viewwork-0.8.0/viewwork/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-25 13:00:55.000000 django-viewwork-0.8.0/viewwork/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:01:06.302429 django-viewwork-0.8.0/viewwork/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:00:55.000000 django-viewwork-0.8.0/viewwork/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:01:06.302429 django-viewwork-0.8.0/viewwork/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:00:55.000000 django-viewwork-0.8.0/viewwork/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-25 13:00:55.000000 django-viewwork-0.8.0/viewwork/management/commands/vw_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-25 13:00:55.000000 django-viewwork-0.8.0/viewwork/metaclass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:01:06.302429 django-viewwork-0.8.0/viewwork/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-25 13:00:55.000000 django-viewwork-0.8.0/viewwork/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-25 13:00:55.000000 django-viewwork-0.8.0/viewwork/migrations/0002_auto_20210709_1622.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-25 13:00:55.000000 django-viewwork-0.8.0/viewwork/migrations/0003_menu_i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-25 13:00:55.000000 django-viewwork-0.8.0/viewwork/migrations/0004_enabled_hidden.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-25 13:00:55.000000 django-viewwork-0.8.0/viewwork/migrations/0005_fix_view_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:00:55.000000 django-viewwork-0.8.0/viewwork/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-25 13:00:55.000000 django-viewwork-0.8.0/viewwork/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-25 13:00:55.000000 django-viewwork-0.8.0/viewwork/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-25 13:00:55.000000 django-viewwork-0.8.0/viewwork/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-25 13:00:55.000000 django-viewwork-0.8.0/viewwork/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-25 13:00:55.000000 django-viewwork-0.8.0/viewwork/views.py
```

### Comparing `django-viewwork-0.7.0/LICENSE` & `django-viewwork-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-viewwork-0.7.0/PKG-INFO` & `django-viewwork-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: django-viewwork
-Version: 0.7.0
+Version: 0.8.0
 Summary: Collect views, generate urls and create menu
 Home-page: https://github.com/pikhovkin/django-viewwork
 Author: Sergei Pikhovkin
 Author-email: s@pikhovkin.ru
 License: MIT
 Keywords: automation,django,views,menu,urls,collectionview,django-views,django-urls,autogeneration,django-menu
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
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8.*, <4.2.*
+Requires-Python: >=3.8,<4.0
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: select2
 License-File: LICENSE
 
 # django-viewwork
```

### Comparing `django-viewwork-0.7.0/README.md` & `django-viewwork-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `django-viewwork-0.7.0/django_viewwork.egg-info/PKG-INFO` & `django-viewwork-0.8.0/django_viewwork.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: django-viewwork
-Version: 0.7.0
+Version: 0.8.0
 Summary: Collect views, generate urls and create menu
 Home-page: https://github.com/pikhovkin/django-viewwork
 Author: Sergei Pikhovkin
 Author-email: s@pikhovkin.ru
 License: MIT
 Keywords: automation,django,views,menu,urls,collectionview,django-views,django-urls,autogeneration,django-menu
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
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8.*, <4.2.*
+Requires-Python: >=3.8,<4.0
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: select2
 License-File: LICENSE
 
 # django-viewwork
```

### Comparing `django-viewwork-0.7.0/django_viewwork.egg-info/SOURCES.txt` & `django-viewwork-0.8.0/django_viewwork.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-viewwork-0.7.0/setup.py` & `django-viewwork-0.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 readme = open('README.md').read()
 requirements = open('requirements/base.txt').readlines()
 require_select2 = open('requirements/select2.txt').readlines()
 require_all = requirements + require_select2
 
 setup(
     name='django-viewwork',
-    version='0.7.0',
+    version='0.8.0',
     description='Collect views, generate urls and create menu',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='Sergei Pikhovkin',
     author_email='s@pikhovkin.ru',
     url='https://github.com/pikhovkin/django-viewwork',
     packages=[
@@ -24,24 +24,25 @@
     ],
     include_package_data=True,
     install_requires=requirements,
     extras_require={
         'all': require_all,
         'select2': require_select2,
     },
-    python_requires='>=3.8.*, <4.2.*',
+    python_requires='>=3.8,<4.0',
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
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
```

### Comparing `django-viewwork-0.7.0/viewwork/admin.py` & `django-viewwork-0.8.0/viewwork/admin.py`

 * *Files identical despite different names*

### Comparing `django-viewwork-0.7.0/viewwork/apps.py` & `django-viewwork-0.8.0/viewwork/apps.py`

 * *Files identical despite different names*

### Comparing `django-viewwork-0.7.0/viewwork/forms.py` & `django-viewwork-0.8.0/viewwork/forms.py`

 * *Files identical despite different names*

### Comparing `django-viewwork-0.7.0/viewwork/locale/en/LC_MESSAGES/django.po` & `django-viewwork-0.8.0/viewwork/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-viewwork-0.7.0/viewwork/locale/ru/LC_MESSAGES/django.mo` & `django-viewwork-0.8.0/viewwork/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-viewwork-0.7.0/viewwork/locale/ru/LC_MESSAGES/django.po` & `django-viewwork-0.8.0/viewwork/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-viewwork-0.7.0/viewwork/management/commands/vw_namespace.py` & `django-viewwork-0.8.0/viewwork/management/commands/vw_namespace.py`

 * *Files identical despite different names*

### Comparing `django-viewwork-0.7.0/viewwork/metaclass.py` & `django-viewwork-0.8.0/viewwork/metaclass.py`

 * *Files identical despite different names*

### Comparing `django-viewwork-0.7.0/viewwork/migrations/0001_initial.py` & `django-viewwork-0.8.0/viewwork/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-viewwork-0.7.0/viewwork/migrations/0004_enabled_hidden.py` & `django-viewwork-0.8.0/viewwork/migrations/0004_enabled_hidden.py`

 * *Files identical despite different names*

### Comparing `django-viewwork-0.7.0/viewwork/migrations/0005_fix_view_name.py` & `django-viewwork-0.8.0/viewwork/migrations/0005_fix_view_name.py`

 * *Files identical despite different names*

### Comparing `django-viewwork-0.7.0/viewwork/models.py` & `django-viewwork-0.8.0/viewwork/models.py`

 * *Files identical despite different names*

### Comparing `django-viewwork-0.7.0/viewwork/settings.py` & `django-viewwork-0.8.0/viewwork/settings.py`

 * *Files identical despite different names*

### Comparing `django-viewwork-0.7.0/viewwork/utils.py` & `django-viewwork-0.8.0/viewwork/utils.py`

 * *Files identical despite different names*

### Comparing `django-viewwork-0.7.0/viewwork/views.py` & `django-viewwork-0.8.0/viewwork/views.py`

 * *Files identical despite different names*

