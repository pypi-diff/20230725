# Comparing `tmp/django-subcommandir-0.2.0.tar.gz` & `tmp/django-subcommandir-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-subcommandir-0.2.0.tar", last modified: Tue Jan 17 17:03:54 2023, max compression
+gzip compressed data, was "django-subcommandir-0.3.0.tar", last modified: Tue Jul 25 13:13:58 2023, max compression
```

## Comparing `django-subcommandir-0.2.0.tar` & `django-subcommandir-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 17:03:54.059756 django-subcommandir-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-01-17 17:03:42.000000 django-subcommandir-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-01-17 17:03:42.000000 django-subcommandir-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-01-17 17:03:54.059756 django-subcommandir-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-01-17 17:03:42.000000 django-subcommandir-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 17:03:54.059756 django-subcommandir-0.2.0/django_subcommandir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-01-17 17:03:53.000000 django-subcommandir-0.2.0/django_subcommandir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-01-17 17:03:53.000000 django-subcommandir-0.2.0/django_subcommandir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 17:03:53.000000 django-subcommandir-0.2.0/django_subcommandir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 17:03:53.000000 django-subcommandir-0.2.0/django_subcommandir.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-17 17:03:53.000000 django-subcommandir-0.2.0/django_subcommandir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-17 17:03:53.000000 django-subcommandir-0.2.0/django_subcommandir.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 17:03:54.059756 django-subcommandir-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-01-17 17:03:42.000000 django-subcommandir-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 17:03:54.059756 django-subcommandir-0.2.0/subcommandir/
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-01-17 17:03:42.000000 django-subcommandir-0.2.0/subcommandir/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 17:03:54.059756 django-subcommandir-0.2.0/subcommandir/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 17:03:42.000000 django-subcommandir-0.2.0/subcommandir/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-01-17 17:03:42.000000 django-subcommandir-0.2.0/subcommandir/tests/test_subcommandir.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 17:03:54.059756 django-subcommandir-0.2.0/subcommandir/tests/tests_subcommandir_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 17:03:42.000000 django-subcommandir-0.2.0/subcommandir/tests/tests_subcommandir_app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 17:03:54.059756 django-subcommandir-0.2.0/subcommandir/tests/tests_subcommandir_app/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 17:03:42.000000 django-subcommandir-0.2.0/subcommandir/tests/tests_subcommandir_app/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 17:03:54.059756 django-subcommandir-0.2.0/subcommandir/tests/tests_subcommandir_app/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 17:03:42.000000 django-subcommandir-0.2.0/subcommandir/tests/tests_subcommandir_app/management/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 17:03:54.059756 django-subcommandir-0.2.0/subcommandir/tests/tests_subcommandir_app/management/commands/load/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 17:03:42.000000 django-subcommandir-0.2.0/subcommandir/tests/tests_subcommandir_app/management/commands/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-01-17 17:03:42.000000 django-subcommandir-0.2.0/subcommandir/tests/tests_subcommandir_app/management/commands/load/month_report.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-01-17 17:03:42.000000 django-subcommandir-0.2.0/subcommandir/tests/tests_subcommandir_app/management/commands/load/year_report.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-01-17 17:03:42.000000 django-subcommandir-0.2.0/subcommandir/tests/tests_subcommandir_app/management/commands/tests_subcommandir_load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:13:58.067040 django-subcommandir-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-25 13:13:45.000000 django-subcommandir-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-25 13:13:45.000000 django-subcommandir-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-25 13:13:58.067040 django-subcommandir-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-25 13:13:45.000000 django-subcommandir-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:13:58.067040 django-subcommandir-0.3.0/django_subcommandir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-25 13:13:58.000000 django-subcommandir-0.3.0/django_subcommandir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-25 13:13:58.000000 django-subcommandir-0.3.0/django_subcommandir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 13:13:58.000000 django-subcommandir-0.3.0/django_subcommandir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 13:13:58.000000 django-subcommandir-0.3.0/django_subcommandir.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-25 13:13:58.000000 django-subcommandir-0.3.0/django_subcommandir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 13:13:58.000000 django-subcommandir-0.3.0/django_subcommandir.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 13:13:58.067040 django-subcommandir-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-25 13:13:45.000000 django-subcommandir-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:13:58.067040 django-subcommandir-0.3.0/subcommandir/
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-25 13:13:45.000000 django-subcommandir-0.3.0/subcommandir/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:13:58.067040 django-subcommandir-0.3.0/subcommandir/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:13:45.000000 django-subcommandir-0.3.0/subcommandir/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-25 13:13:45.000000 django-subcommandir-0.3.0/subcommandir/tests/test_subcommandir.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:13:58.067040 django-subcommandir-0.3.0/subcommandir/tests/tests_subcommandir_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:13:45.000000 django-subcommandir-0.3.0/subcommandir/tests/tests_subcommandir_app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:13:58.067040 django-subcommandir-0.3.0/subcommandir/tests/tests_subcommandir_app/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:13:45.000000 django-subcommandir-0.3.0/subcommandir/tests/tests_subcommandir_app/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:13:58.067040 django-subcommandir-0.3.0/subcommandir/tests/tests_subcommandir_app/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:13:45.000000 django-subcommandir-0.3.0/subcommandir/tests/tests_subcommandir_app/management/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:13:58.067040 django-subcommandir-0.3.0/subcommandir/tests/tests_subcommandir_app/management/commands/load/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:13:45.000000 django-subcommandir-0.3.0/subcommandir/tests/tests_subcommandir_app/management/commands/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-25 13:13:45.000000 django-subcommandir-0.3.0/subcommandir/tests/tests_subcommandir_app/management/commands/load/month_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-25 13:13:45.000000 django-subcommandir-0.3.0/subcommandir/tests/tests_subcommandir_app/management/commands/load/year_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-25 13:13:45.000000 django-subcommandir-0.3.0/subcommandir/tests/tests_subcommandir_app/management/commands/tests_subcommandir_load.py
```

### Comparing `django-subcommandir-0.2.0/LICENSE` & `django-subcommandir-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-subcommandir-0.2.0/PKG-INFO` & `django-subcommandir-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: django-subcommandir
-Version: 0.2.0
+Version: 0.3.0
 Summary: Django subcommands in subdirectories
 Home-page: https://github.com/pikhovkin/django-subcommandir
 Author: Sergei Pikhovkin
 Author-email: s@pikhovkin.ru
 License: MIT
 Keywords: django,command,commands,django-commands,django-subcommands
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 3.0
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
 License-File: LICENSE
 
 # django-subcommandir
 
 [![GitHub Actions](https://github.com/pikhovkin/django-subcommandir/workflows/build/badge.svg)](https://github.com/pikhovkin/django-subcommandir/actions)
 [![PyPI](https://img.shields.io/pypi/v/django-subcommandir.svg)](https://pypi.org/project/django-subcommandir/)
```

### Comparing `django-subcommandir-0.2.0/README.md` & `django-subcommandir-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `django-subcommandir-0.2.0/django_subcommandir.egg-info/PKG-INFO` & `django-subcommandir-0.3.0/django_subcommandir.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: django-subcommandir
-Version: 0.2.0
+Version: 0.3.0
 Summary: Django subcommands in subdirectories
 Home-page: https://github.com/pikhovkin/django-subcommandir
 Author: Sergei Pikhovkin
 Author-email: s@pikhovkin.ru
 License: MIT
 Keywords: django,command,commands,django-commands,django-subcommands
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 3.0
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
 License-File: LICENSE
 
 # django-subcommandir
 
 [![GitHub Actions](https://github.com/pikhovkin/django-subcommandir/workflows/build/badge.svg)](https://github.com/pikhovkin/django-subcommandir/actions)
 [![PyPI](https://img.shields.io/pypi/v/django-subcommandir.svg)](https://pypi.org/project/django-subcommandir/)
```

### Comparing `django-subcommandir-0.2.0/django_subcommandir.egg-info/SOURCES.txt` & `django-subcommandir-0.3.0/django_subcommandir.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-subcommandir-0.2.0/setup.py` & `django-subcommandir-0.3.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,39 +3,40 @@
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
 
 setup(
     name='django-subcommandir',
-    version='0.2.0',
+    version='0.3.0',
     description='Django subcommands in subdirectories',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Sergei Pikhovkin',
     author_email='s@pikhovkin.ru',
     url='https://github.com/pikhovkin/django-subcommandir',
     packages=[
         'subcommandir',
     ],
     include_package_data=True,
     install_requires=[
         'Django>=3.1,<4.2',
     ],
-    python_requires='>=3.7.*, <4.0.*',
+    python_requires='>=3.7,<4.0',
     license='MIT',
     zip_safe=False,
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Environment :: Web Environment',
         'Framework :: Django :: 3.0',
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

### Comparing `django-subcommandir-0.2.0/subcommandir/__init__.py` & `django-subcommandir-0.3.0/subcommandir/__init__.py`

 * *Files identical despite different names*

### Comparing `django-subcommandir-0.2.0/subcommandir/tests/test_subcommandir.py` & `django-subcommandir-0.3.0/subcommandir/tests/test_subcommandir.py`

 * *Files identical despite different names*

