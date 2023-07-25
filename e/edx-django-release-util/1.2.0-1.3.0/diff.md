# Comparing `tmp/edx-django-release-util-1.2.0.tar.gz` & `tmp/edx-django-release-util-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-django-release-util-1.2.0.tar", last modified: Wed Feb 23 10:48:45 2022, max compression
+gzip compressed data, was "edx-django-release-util-1.3.0.tar", last modified: Tue Jul 25 08:45:35 2023, max compression
```

## Comparing `edx-django-release-util-1.2.0.tar` & `edx-django-release-util-1.3.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 10:48:45.856068 edx-django-release-util-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)    34520 2022-02-23 10:48:37.000000 edx-django-release-util-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-02-23 10:48:37.000000 edx-django-release-util-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2280 2022-02-23 10:48:45.856068 edx-django-release-util-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1454 2022-02-23 10:48:37.000000 edx-django-release-util-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 10:48:45.852068 edx-django-release-util-1.2.0/edx_django_release_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2280 2022-02-23 10:48:45.000000 edx-django-release-util-1.2.0/edx_django_release_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1952 2022-02-23 10:48:45.000000 edx-django-release-util-1.2.0/edx_django_release_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-23 10:48:45.000000 edx-django-release-util-1.2.0/edx_django_release_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-02-23 10:48:45.000000 edx-django-release-util-1.2.0/edx_django_release_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-02-23 10:48:45.000000 edx-django-release-util-1.2.0/edx_django_release_util.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 10:48:45.852068 edx-django-release-util-1.2.0/release_util/
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-02-23 10:48:37.000000 edx-django-release-util-1.2.0/release_util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 10:48:45.852068 edx-django-release-util-1.2.0/release_util/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-23 10:48:37.000000 edx-django-release-util-1.2.0/release_util/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 10:48:45.856068 edx-django-release-util-1.2.0/release_util/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)    12964 2022-02-23 10:48:37.000000 edx-django-release-util-1.2.0/release_util/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14157 2022-02-23 10:48:37.000000 edx-django-release-util-1.2.0/release_util/management/commands/check_reserved_keywords.py
--rw-r--r--   0 runner    (1001) docker     (121)     5445 2022-02-23 10:48:37.000000 edx-django-release-util-1.2.0/release_util/management/commands/default_reserved_keywords.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1891 2022-02-23 10:48:37.000000 edx-django-release-util-1.2.0/release_util/management/commands/detect_missing_migrations.py
--rw-r--r--   0 runner    (1001) docker     (121)     5770 2022-02-23 10:48:37.000000 edx-django-release-util-1.2.0/release_util/management/commands/generate_history.py
--rw-r--r--   0 runner    (1001) docker     (121)     3044 2022-02-23 10:48:37.000000 edx-django-release-util-1.2.0/release_util/management/commands/run_migrations.py
--rw-r--r--   0 runner    (1001) docker     (121)     3181 2022-02-23 10:48:37.000000 edx-django-release-util-1.2.0/release_util/management/commands/run_specific_migrations.py
--rw-r--r--   0 runner    (1001) docker     (121)     2723 2022-02-23 10:48:37.000000 edx-django-release-util-1.2.0/release_util/management/commands/show_unapplied_migrations.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 10:48:45.852068 edx-django-release-util-1.2.0/release_util/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 10:48:45.856068 edx-django-release-util-1.2.0/release_util/tests/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-23 10:48:37.000000 edx-django-release-util-1.2.0/release_util/tests/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 10:48:45.856068 edx-django-release-util-1.2.0/release_util/tests/migrations/test_migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-02-23 10:48:37.000000 edx-django-release-util-1.2.0/release_util/tests/migrations/test_migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-02-23 10:48:37.000000 edx-django-release-util-1.2.0/release_util/tests/migrations/test_migrations/0002_second.py
--rw-r--r--   0 runner    (1001) docker     (121)      616 2022-02-23 10:48:37.000000 edx-django-release-util-1.2.0/release_util/tests/migrations/test_migrations/0003_third.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-23 10:48:37.000000 edx-django-release-util-1.2.0/release_util/tests/migrations/test_migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 10:48:45.856068 edx-django-release-util-1.2.0/release_util/tests/test_check_reserved_keywords/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-23 10:48:37.000000 edx-django-release-util-1.2.0/release_util/tests/test_check_reserved_keywords/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 10:48:45.856068 edx-django-release-util-1.2.0/release_util/tests/test_check_reserved_keywords/test_app/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-23 10:48:37.000000 edx-django-release-util-1.2.0/release_util/tests/test_check_reserved_keywords/test_app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 10:48:45.856068 edx-django-release-util-1.2.0/release_util/tests/test_check_reserved_keywords/test_app/local_app/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-23 10:48:37.000000 edx-django-release-util-1.2.0/release_util/tests/test_check_reserved_keywords/test_app/local_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-02-23 10:48:37.000000 edx-django-release-util-1.2.0/release_util/tests/test_check_reserved_keywords/test_app/local_app/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      566 2022-02-23 10:48:37.000000 edx-django-release-util-1.2.0/release_util/tests/test_check_reserved_keywords/test_app/local_app/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 10:48:45.856068 edx-django-release-util-1.2.0/release_util/tests/test_check_reserved_keywords/test_app/non_concrete_app/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-23 10:48:37.000000 edx-django-release-util-1.2.0/release_util/tests/test_check_reserved_keywords/test_app/non_concrete_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-02-23 10:48:37.000000 edx-django-release-util-1.2.0/release_util/tests/test_check_reserved_keywords/test_app/non_concrete_app/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-02-23 10:48:37.000000 edx-django-release-util-1.2.0/release_util/tests/test_check_reserved_keywords/test_app/non_concrete_app/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 10:48:45.856068 edx-django-release-util-1.2.0/release_util/tests/test_check_reserved_keywords/test_app/test_app/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-23 10:48:37.000000 edx-django-release-util-1.2.0/release_util/tests/test_check_reserved_keywords/test_app/test_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2930 2022-02-23 10:48:37.000000 edx-django-release-util-1.2.0/release_util/tests/test_check_reserved_keywords/test_app/test_app/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     8165 2022-02-23 10:48:37.000000 edx-django-release-util-1.2.0/release_util/tests/test_check_reserved_keywords/test_check_reserved_keywords.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 10:48:45.856068 edx-django-release-util-1.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-02-23 10:48:37.000000 edx-django-release-util-1.2.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-02-23 10:48:45.856068 edx-django-release-util-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2464 2022-02-23 10:48:37.000000 edx-django-release-util-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:35.720546 edx-django-release-util-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2196 2023-07-25 08:45:35.720546 edx-django-release-util-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1327 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:35.712546 edx-django-release-util-1.3.0/edx_django_release_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2196 2023-07-25 08:45:35.000000 edx-django-release-util-1.3.0/edx_django_release_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2013 2023-07-25 08:45:35.000000 edx-django-release-util-1.3.0/edx_django_release_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-25 08:45:35.000000 edx-django-release-util-1.3.0/edx_django_release_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-25 08:45:35.000000 edx-django-release-util-1.3.0/edx_django_release_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-25 08:45:35.000000 edx-django-release-util-1.3.0/edx_django_release_util.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:35.712546 edx-django-release-util-1.3.0/release_util/
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:35.712546 edx-django-release-util-1.3.0/release_util/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:35.716546 edx-django-release-util-1.3.0/release_util/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)    12964 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14157 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/management/commands/check_reserved_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5445 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/management/commands/default_reserved_keywords.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1891 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/management/commands/detect_missing_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5770 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/management/commands/generate_history.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3044 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/management/commands/run_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3181 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/management/commands/run_specific_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2723 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/management/commands/show_unapplied_migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:35.712546 edx-django-release-util-1.3.0/release_util/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:35.716546 edx-django-release-util-1.3.0/release_util/tests/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:35.716546 edx-django-release-util-1.3.0/release_util/tests/migrations/test_migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1020 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/migrations/test_migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      623 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/migrations/test_migrations/0002_second.py
+-rw-r--r--   0 runner    (1001) docker     (122)      616 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/migrations/test_migrations/0003_third.py
+-rw-r--r--   0 runner    (1001) docker     (122)      733 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/migrations/test_migrations/0004_fourth.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/migrations/test_migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:35.716546 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:35.716546 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:35.716546 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/local_app/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/local_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/local_app/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/local_app/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:35.716546 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/non_concrete_app/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/non_concrete_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/non_concrete_app/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/non_concrete_app/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:35.716546 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/test_app/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/test_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2930 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/test_app/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8165 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_check_reserved_keywords.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 08:45:35.720546 edx-django-release-util-1.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-07-25 08:45:35.720546 edx-django-release-util-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2506 2023-07-25 08:45:26.000000 edx-django-release-util-1.3.0/setup.py
```

### Comparing `edx-django-release-util-1.2.0/LICENSE` & `edx-django-release-util-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.2.0/PKG-INFO` & `edx-django-release-util-1.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: edx-django-release-util
-Version: 1.2.0
+Version: 1.3.0
 Summary: edx-django-release-util
-Home-page: http://github.com/edx/edx-django-release-util
+Home-page: http://github.com/openedx/edx-django-release-util
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -15,14 +15,15 @@
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 License-File: LICENSE
 
 Part of `edX code`__.
 
 __ http://code.edx.org/
 
 edX Django Release Utilities  |Travis|_ 
@@ -54,18 +55,16 @@
 
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
 
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
```

### Comparing `edx-django-release-util-1.2.0/README.rst` & `edx-django-release-util-1.3.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -31,18 +31,16 @@
 
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
 
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
```

### Comparing `edx-django-release-util-1.2.0/edx_django_release_util.egg-info/PKG-INFO` & `edx-django-release-util-1.3.0/edx_django_release_util.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: edx-django-release-util
-Version: 1.2.0
+Version: 1.3.0
 Summary: edx-django-release-util
-Home-page: http://github.com/edx/edx-django-release-util
+Home-page: http://github.com/openedx/edx-django-release-util
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -15,14 +15,15 @@
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 License-File: LICENSE
 
 Part of `edX code`__.
 
 __ http://code.edx.org/
 
 edX Django Release Utilities  |Travis|_ 
@@ -54,18 +55,16 @@
 
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
 
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
```

### Comparing `edx-django-release-util-1.2.0/edx_django_release_util.egg-info/SOURCES.txt` & `edx-django-release-util-1.3.0/edx_django_release_util.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 release_util/management/commands/run_migrations.py
 release_util/management/commands/run_specific_migrations.py
 release_util/management/commands/show_unapplied_migrations.py
 release_util/tests/migrations/__init__.py
 release_util/tests/migrations/test_migrations/0001_initial.py
 release_util/tests/migrations/test_migrations/0002_second.py
 release_util/tests/migrations/test_migrations/0003_third.py
+release_util/tests/migrations/test_migrations/0004_fourth.py
 release_util/tests/migrations/test_migrations/__init__.py
 release_util/tests/test_check_reserved_keywords/__init__.py
 release_util/tests/test_check_reserved_keywords/test_check_reserved_keywords.py
 release_util/tests/test_check_reserved_keywords/test_app/__init__.py
 release_util/tests/test_check_reserved_keywords/test_app/local_app/__init__.py
 release_util/tests/test_check_reserved_keywords/test_app/local_app/apps.py
 release_util/tests/test_check_reserved_keywords/test_app/local_app/models.py
```

### Comparing `edx-django-release-util-1.2.0/release_util/management/commands/__init__.py` & `edx-django-release-util-1.3.0/release_util/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.2.0/release_util/management/commands/check_reserved_keywords.py` & `edx-django-release-util-1.3.0/release_util/management/commands/check_reserved_keywords.py`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.2.0/release_util/management/commands/default_reserved_keywords.yml` & `edx-django-release-util-1.3.0/release_util/management/commands/default_reserved_keywords.yml`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.2.0/release_util/management/commands/detect_missing_migrations.py` & `edx-django-release-util-1.3.0/release_util/management/commands/detect_missing_migrations.py`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.2.0/release_util/management/commands/generate_history.py` & `edx-django-release-util-1.3.0/release_util/management/commands/generate_history.py`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.2.0/release_util/management/commands/run_migrations.py` & `edx-django-release-util-1.3.0/release_util/management/commands/run_migrations.py`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.2.0/release_util/management/commands/run_specific_migrations.py` & `edx-django-release-util-1.3.0/release_util/management/commands/run_specific_migrations.py`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.2.0/release_util/management/commands/show_unapplied_migrations.py` & `edx-django-release-util-1.3.0/release_util/management/commands/show_unapplied_migrations.py`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.2.0/release_util/tests/migrations/test_migrations/0001_initial.py` & `edx-django-release-util-1.3.0/release_util/tests/migrations/test_migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.2.0/release_util/tests/migrations/test_migrations/0002_second.py` & `edx-django-release-util-1.3.0/release_util/tests/migrations/test_migrations/0002_second.py`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.2.0/release_util/tests/migrations/test_migrations/0003_third.py` & `edx-django-release-util-1.3.0/release_util/tests/migrations/test_migrations/0003_third.py`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.2.0/release_util/tests/test_check_reserved_keywords/test_app/local_app/models.py` & `edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/local_app/models.py`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.2.0/release_util/tests/test_check_reserved_keywords/test_app/non_concrete_app/models.py` & `edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/non_concrete_app/models.py`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.2.0/release_util/tests/test_check_reserved_keywords/test_app/test_app/settings.py` & `edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_app/test_app/settings.py`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.2.0/release_util/tests/test_check_reserved_keywords/test_check_reserved_keywords.py` & `edx-django-release-util-1.3.0/release_util/tests/test_check_reserved_keywords/test_check_reserved_keywords.py`

 * *Files identical despite different names*

### Comparing `edx-django-release-util-1.2.0/setup.py` & `edx-django-release-util-1.3.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     name='edx-django-release-util',
     version=VERSION,
     description='edx-django-release-util',
     author='edX',
     author_email='oscm@edx.org',
     long_description=LONG_DESCRIPTION,
     license='AGPL 3.0',
-    url='http://github.com/edx/edx-django-release-util',
+    url='http://github.com/openedx/edx-django-release-util',
     install_requires=load_requirements('requirements/base.in'),
     packages=find_packages(exclude=['*.test', '*.tests']),
     include_package_data=True,
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries :: Python Modules',
@@ -72,9 +72,10 @@
         'License :: OSI Approved :: GNU Affero General Public License v3',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
+        'Framework :: Django :: 4.2',
     ],
 )
```

