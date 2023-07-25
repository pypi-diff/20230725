# Comparing `tmp/tap-harvest-2.1.2.tar.gz` & `tmp/tap-harvest-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-harvest-2.1.2.tar", last modified: Wed Dec  1 18:40:22 2021, max compression
+gzip compressed data, was "tap-harvest-2.1.3.tar", last modified: Tue Jul 25 19:13:50 2023, max compression
```

## Comparing `tap-harvest-2.1.2.tar` & `tap-harvest-2.1.3.tar`

### file list

```diff
@@ -1,42 +1,48 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-12-01 18:40:22.795963 tap-harvest-2.1.2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32393 2021-10-01 23:50:27.000000 tap-harvest-2.1.2/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       51 2021-10-01 23:50:27.000000 tap-harvest-2.1.2/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      296 2021-12-01 18:40:22.795963 tap-harvest-2.1.2/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2001 2021-12-01 15:21:30.000000 tap-harvest-2.1.2/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2021-12-01 18:40:22.795963 tap-harvest-2.1.2/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1647 2021-12-01 18:40:08.000000 tap-harvest-2.1.2/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-12-01 18:40:22.783963 tap-harvest-2.1.2/tap_harvest/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18889 2021-12-01 15:21:30.000000 tap-harvest-2.1.2/tap_harvest/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-12-01 18:40:22.795963 tap-harvest-2.1.2/tap_harvest/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      505 2021-10-01 23:50:27.000000 tap-harvest-2.1.2/tap_harvest/schemas/clients.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      742 2021-10-01 23:50:27.000000 tap-harvest-2.1.2/tap_harvest/schemas/contacts.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2021-10-01 23:50:27.000000 tap-harvest-2.1.2/tap_harvest/schemas/estimate_item_categories.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      563 2021-10-01 23:50:27.000000 tap-harvest-2.1.2/tap_harvest/schemas/estimate_line_items.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1171 2021-10-01 23:50:27.000000 tap-harvest-2.1.2/tap_harvest/schemas/estimate_messages.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1594 2021-10-01 23:50:27.000000 tap-harvest-2.1.2/tap_harvest/schemas/estimates.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      509 2021-10-01 23:50:27.000000 tap-harvest-2.1.2/tap_harvest/schemas/expense_categories.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1482 2021-10-01 23:50:27.000000 tap-harvest-2.1.2/tap_harvest/schemas/expenses.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      395 2021-10-01 23:50:27.000000 tap-harvest-2.1.2/tap_harvest/schemas/external_reference.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      460 2021-10-01 23:50:27.000000 tap-harvest-2.1.2/tap_harvest/schemas/invoice_item_categories.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      623 2021-10-01 23:50:27.000000 tap-harvest-2.1.2/tap_harvest/schemas/invoice_line_items.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1526 2021-10-01 23:50:27.000000 tap-harvest-2.1.2/tap_harvest/schemas/invoice_messages.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      954 2021-10-01 23:50:27.000000 tap-harvest-2.1.2/tap_harvest/schemas/invoice_payments.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2189 2021-10-01 23:50:27.000000 tap-harvest-2.1.2/tap_harvest/schemas/invoices.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      631 2021-10-01 23:50:27.000000 tap-harvest-2.1.2/tap_harvest/schemas/project_tasks.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      641 2021-10-01 23:50:27.000000 tap-harvest-2.1.2/tap_harvest/schemas/project_users.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1631 2021-10-01 23:50:27.000000 tap-harvest-2.1.2/tap_harvest/schemas/projects.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2021-10-01 23:50:27.000000 tap-harvest-2.1.2/tap_harvest/schemas/roles.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      590 2021-10-01 23:50:27.000000 tap-harvest-2.1.2/tap_harvest/schemas/tasks.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1790 2021-10-01 23:50:27.000000 tap-harvest-2.1.2/tap_harvest/schemas/time_entries.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      180 2021-10-01 23:50:27.000000 tap-harvest-2.1.2/tap_harvest/schemas/time_entry_external_reference.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      169 2021-10-01 23:50:27.000000 tap-harvest-2.1.2/tap_harvest/schemas/user_project_tasks.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      701 2021-10-01 23:50:27.000000 tap-harvest-2.1.2/tap_harvest/schemas/user_projects.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      161 2021-10-01 23:50:27.000000 tap-harvest-2.1.2/tap_harvest/schemas/user_roles.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1361 2021-10-01 23:50:27.000000 tap-harvest-2.1.2/tap_harvest/schemas/users.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-12-01 18:40:22.783963 tap-harvest-2.1.2/tap_harvest.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      296 2021-12-01 18:40:22.000000 tap-harvest-2.1.2/tap_harvest.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1274 2021-12-01 18:40:22.000000 tap-harvest-2.1.2/tap_harvest.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2021-12-01 18:40:22.000000 tap-harvest-2.1.2/tap_harvest.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2021-12-01 18:40:22.000000 tap-harvest-2.1.2/tap_harvest.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       83 2021-12-01 18:40:22.000000 tap-harvest-2.1.2/tap_harvest.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2021-12-01 18:40:22.000000 tap-harvest-2.1.2/tap_harvest.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-25 19:13:50.709012 tap-harvest-2.1.3/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32393 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       51 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      251 2023-07-25 19:13:50.709012 tap-harvest-2.1.3/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2001 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-07-25 19:13:50.709012 tap-harvest-2.1.3/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1646 2023-07-25 19:12:52.000000 tap-harvest-2.1.3/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-25 19:13:50.689012 tap-harvest-2.1.3/tap_harvest/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18889 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/tap_harvest/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-25 19:13:50.705012 tap-harvest-2.1.3/tap_harvest/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      505 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/tap_harvest/schemas/clients.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      742 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/tap_harvest/schemas/contacts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/tap_harvest/schemas/estimate_item_categories.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      563 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/tap_harvest/schemas/estimate_line_items.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1171 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/tap_harvest/schemas/estimate_messages.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1594 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/tap_harvest/schemas/estimates.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      509 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/tap_harvest/schemas/expense_categories.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1482 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/tap_harvest/schemas/expenses.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      395 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/tap_harvest/schemas/external_reference.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      460 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/tap_harvest/schemas/invoice_item_categories.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      623 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/tap_harvest/schemas/invoice_line_items.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1526 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/tap_harvest/schemas/invoice_messages.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      954 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/tap_harvest/schemas/invoice_payments.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2189 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/tap_harvest/schemas/invoices.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      631 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/tap_harvest/schemas/project_tasks.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      641 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/tap_harvest/schemas/project_users.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1631 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/tap_harvest/schemas/projects.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/tap_harvest/schemas/roles.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      590 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/tap_harvest/schemas/tasks.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1790 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/tap_harvest/schemas/time_entries.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      180 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/tap_harvest/schemas/time_entry_external_reference.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      169 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/tap_harvest/schemas/user_project_tasks.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      701 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/tap_harvest/schemas/user_projects.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      161 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/tap_harvest/schemas/user_roles.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1361 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/tap_harvest/schemas/users.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-25 19:13:50.689012 tap-harvest-2.1.3/tap_harvest.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      251 2023-07-25 19:13:50.000000 tap-harvest-2.1.3/tap_harvest.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1448 2023-07-25 19:13:50.000000 tap-harvest-2.1.3/tap_harvest.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-25 19:13:50.000000 tap-harvest-2.1.3/tap_harvest.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       49 2023-07-25 19:13:50.000000 tap-harvest-2.1.3/tap_harvest.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       83 2023-07-25 19:13:50.000000 tap-harvest-2.1.3/tap_harvest.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2023-07-25 19:13:50.000000 tap-harvest-2.1.3/tap_harvest.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-25 19:13:50.709012 tap-harvest-2.1.3/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    35384 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/tests/test_harvest_bookmarks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1214 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/tests/test_harvest_future_date.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21982 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/tests/test_harvest_pagination.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13811 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/tests/test_harvest_start_date.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5213 2023-05-23 22:34:46.000000 tap-harvest-2.1.3/tests/test_harvest_start_date_honoring.py
```

### Comparing `tap-harvest-2.1.2/LICENSE` & `tap-harvest-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-harvest-2.1.2/README.md` & `tap-harvest-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tap-harvest-2.1.2/setup.py` & `tap-harvest-2.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(name='tap-harvest',
-      version="2.1.2",
+      version="2.1.3",
       description='Singer.io tap for extracting data from the Harvest api',
       author='Facet Interactive',
       url='http://singer.io',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_harvest'],
       install_requires=[
           'singer-python==5.12.1',
-          'requests==2.20.0',
+          'requests==2.31.0',
           'pendulum==1.2.0',
           'backoff==1.8.0',
           'pytz==2018.4',
       ],
       entry_points='''
           [console_scripts]
           tap-harvest=tap_harvest:main
@@ -46,8 +46,8 @@
               "user_project_tasks.json",
               "user_projects.json",
               "user_roles.json",
               "users.json",
           ],
       },
       include_package_data=True,
-)
+)
```

### Comparing `tap-harvest-2.1.2/tap_harvest/__init__.py` & `tap-harvest-2.1.3/tap_harvest/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-harvest-2.1.2/tap_harvest/schemas/contacts.json` & `tap-harvest-2.1.3/tap_harvest/schemas/contacts.json`

 * *Files identical despite different names*

### Comparing `tap-harvest-2.1.2/tap_harvest/schemas/estimate_line_items.json` & `tap-harvest-2.1.3/tap_harvest/schemas/estimate_line_items.json`

 * *Files identical despite different names*

### Comparing `tap-harvest-2.1.2/tap_harvest/schemas/estimate_messages.json` & `tap-harvest-2.1.3/tap_harvest/schemas/estimate_messages.json`

 * *Files identical despite different names*

### Comparing `tap-harvest-2.1.2/tap_harvest/schemas/estimates.json` & `tap-harvest-2.1.3/tap_harvest/schemas/estimates.json`

 * *Files identical despite different names*

### Comparing `tap-harvest-2.1.2/tap_harvest/schemas/expenses.json` & `tap-harvest-2.1.3/tap_harvest/schemas/expenses.json`

 * *Files identical despite different names*

### Comparing `tap-harvest-2.1.2/tap_harvest/schemas/invoice_line_items.json` & `tap-harvest-2.1.3/tap_harvest/schemas/invoice_line_items.json`

 * *Files identical despite different names*

### Comparing `tap-harvest-2.1.2/tap_harvest/schemas/invoice_messages.json` & `tap-harvest-2.1.3/tap_harvest/schemas/invoice_messages.json`

 * *Files identical despite different names*

### Comparing `tap-harvest-2.1.2/tap_harvest/schemas/invoice_payments.json` & `tap-harvest-2.1.3/tap_harvest/schemas/invoice_payments.json`

 * *Files identical despite different names*

### Comparing `tap-harvest-2.1.2/tap_harvest/schemas/invoices.json` & `tap-harvest-2.1.3/tap_harvest/schemas/invoices.json`

 * *Files identical despite different names*

### Comparing `tap-harvest-2.1.2/tap_harvest/schemas/project_tasks.json` & `tap-harvest-2.1.3/tap_harvest/schemas/project_tasks.json`

 * *Files identical despite different names*

### Comparing `tap-harvest-2.1.2/tap_harvest/schemas/project_users.json` & `tap-harvest-2.1.3/tap_harvest/schemas/project_users.json`

 * *Files identical despite different names*

### Comparing `tap-harvest-2.1.2/tap_harvest/schemas/projects.json` & `tap-harvest-2.1.3/tap_harvest/schemas/projects.json`

 * *Files identical despite different names*

### Comparing `tap-harvest-2.1.2/tap_harvest/schemas/tasks.json` & `tap-harvest-2.1.3/tap_harvest/schemas/tasks.json`

 * *Files identical despite different names*

### Comparing `tap-harvest-2.1.2/tap_harvest/schemas/time_entries.json` & `tap-harvest-2.1.3/tap_harvest/schemas/time_entries.json`

 * *Files identical despite different names*

### Comparing `tap-harvest-2.1.2/tap_harvest/schemas/user_projects.json` & `tap-harvest-2.1.3/tap_harvest/schemas/user_projects.json`

 * *Files identical despite different names*

### Comparing `tap-harvest-2.1.2/tap_harvest/schemas/users.json` & `tap-harvest-2.1.3/tap_harvest/schemas/users.json`

 * *Files identical despite different names*

### Comparing `tap-harvest-2.1.2/tap_harvest.egg-info/SOURCES.txt` & `tap-harvest-2.1.3/tap_harvest.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -30,8 +30,13 @@
 tap_harvest/schemas/roles.json
 tap_harvest/schemas/tasks.json
 tap_harvest/schemas/time_entries.json
 tap_harvest/schemas/time_entry_external_reference.json
 tap_harvest/schemas/user_project_tasks.json
 tap_harvest/schemas/user_projects.json
 tap_harvest/schemas/user_roles.json
-tap_harvest/schemas/users.json
+tap_harvest/schemas/users.json
+tests/test_harvest_bookmarks.py
+tests/test_harvest_future_date.py
+tests/test_harvest_pagination.py
+tests/test_harvest_start_date.py
+tests/test_harvest_start_date_honoring.py
```

