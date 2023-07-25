# Comparing `tmp/mds_cashbook_account-6.0.9.tar.gz` & `tmp/mds_cashbook_account-6.8.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mds_cashbook_account-6.0.9.tar", last modified: Tue Feb 14 09:14:50 2023, max compression
+gzip compressed data, was "mds_cashbook_account-6.8.11.tar", last modified: Tue Jul 25 20:12:44 2023, max compression
```

## Comparing `mds_cashbook_account-6.0.9.tar` & `mds_cashbook_account-6.8.11.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-02-14 09:14:50.980557 mds_cashbook_account-6.0.9/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2116 2023-02-14 09:14:50.980557 mds_cashbook_account-6.0.9/PKG-INFO
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      650 2023-02-14 09:13:18.000000 mds_cashbook_account-6.0.9/README.rst
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      712 2022-09-30 08:36:15.000000 mds_cashbook_account-6.0.9/__init__.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1254 2022-09-30 08:36:12.000000 mds_cashbook_account-6.0.9/book.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     4273 2022-09-05 15:22:47.000000 mds_cashbook_account-6.0.9/book.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     3040 2022-09-30 08:36:12.000000 mds_cashbook_account-6.0.9/category.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1048 2022-08-15 07:19:51.000000 mds_cashbook_account-6.0.9/category.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1208 2022-08-15 08:21:40.000000 mds_cashbook_account-6.0.9/configuration.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      527 2022-08-15 08:16:21.000000 mds_cashbook_account-6.0.9/configuration.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    19603 2022-10-04 14:51:23.000000 mds_cashbook_account-6.0.9/line.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      491 2022-08-18 14:02:24.000000 mds_cashbook_account-6.0.9/line.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-02-14 09:14:50.968557 mds_cashbook_account-6.0.9/locale/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     9296 2022-09-30 08:36:14.000000 mds_cashbook_account-6.0.9/locale/de.po
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     8372 2022-09-30 08:36:14.000000 mds_cashbook_account-6.0.9/locale/en.po
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-02-14 09:14:50.980557 mds_cashbook_account-6.0.9/mds_cashbook_account.egg-info/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2116 2023-02-14 09:14:50.000000 mds_cashbook_account-6.0.9/mds_cashbook_account.egg-info/PKG-INFO
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      920 2023-02-14 09:14:50.000000 mds_cashbook_account-6.0.9/mds_cashbook_account.egg-info/SOURCES.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-02-14 09:14:50.000000 mds_cashbook_account-6.0.9/mds_cashbook_account.egg-info/dependency_links.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       83 2023-02-14 09:14:50.000000 mds_cashbook_account-6.0.9/mds_cashbook_account.egg-info/entry_points.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-02-14 09:14:50.000000 mds_cashbook_account-6.0.9/mds_cashbook_account.egg-info/not-zip-safe
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       75 2023-02-14 09:14:50.000000 mds_cashbook_account-6.0.9/mds_cashbook_account.egg-info/requires.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2023-02-14 09:14:50.000000 mds_cashbook_account-6.0.9/mds_cashbook_account.egg-info/top_level.txt
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     2106 2022-09-30 08:36:14.000000 mds_cashbook_account-6.0.9/message.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      801 2022-09-30 08:36:15.000000 mds_cashbook_account-6.0.9/move.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      685 2022-09-07 09:40:43.000000 mds_cashbook_account-6.0.9/move.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    10679 2022-09-30 08:36:14.000000 mds_cashbook_account-6.0.9/netmixin.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2023-02-14 09:14:50.980557 mds_cashbook_account-6.0.9/setup.cfg
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     3588 2022-08-15 07:17:31.000000 mds_cashbook_account-6.0.9/setup.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      877 2022-09-30 08:36:16.000000 mds_cashbook_account-6.0.9/splitline.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      495 2022-09-30 08:36:14.000000 mds_cashbook_account-6.0.9/splitline.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     3842 2023-02-14 09:12:33.000000 mds_cashbook_account-6.0.9/tax.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      794 2022-09-30 08:36:15.000000 mds_cashbook_account-6.0.9/tax.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-02-14 09:14:50.968557 mds_cashbook_account-6.0.9/tests/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      719 2022-08-15 10:03:15.000000 mds_cashbook_account-6.0.9/tests/__init__.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     3268 2022-08-23 07:24:19.000000 mds_cashbook_account-6.0.9/tests/test_category.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)   248842 2023-02-14 09:12:33.000000 mds_cashbook_account-6.0.9/tests/test_line.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      186 2023-02-14 09:13:40.000000 mds_cashbook_account-6.0.9/tryton.cfg
--rw-rw----   0 trytproj  (1001) trytproj  (1001)       28 2023-02-14 09:13:50.000000 mds_cashbook_account-6.0.9/versiondep.txt
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-02-14 09:14:50.976557 mds_cashbook_account-6.0.9/view/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      622 2022-09-05 15:22:47.000000 mds_cashbook_account-6.0.9/view/book_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      331 2023-02-14 09:12:33.000000 mds_cashbook_account-6.0.9/view/book_list.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      680 2022-09-30 08:36:13.000000 mds_cashbook_account-6.0.9/view/category_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      332 2022-09-05 08:42:35.000000 mds_cashbook_account-6.0.9/view/category_list.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      333 2022-09-05 08:42:35.000000 mds_cashbook_account-6.0.9/view/category_tree.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      336 2022-08-15 08:55:38.000000 mds_cashbook_account-6.0.9/view/configuration_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1861 2022-09-30 08:36:15.000000 mds_cashbook_account-6.0.9/view/line_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1520 2022-09-30 08:36:14.000000 mds_cashbook_account-6.0.9/view/split_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      542 2022-09-30 08:36:15.000000 mds_cashbook_account-6.0.9/view/tax_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      380 2022-09-30 08:36:15.000000 mds_cashbook_account-6.0.9/view/tax_list.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-25 20:12:44.142516 mds_cashbook_account-6.8.11/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1537 2023-07-25 20:12:44.138517 mds_cashbook_account-6.8.11/PKG-INFO
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      276 2023-07-25 20:06:19.000000 mds_cashbook_account-6.8.11/README.rst
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      713 2023-06-03 16:30:29.000000 mds_cashbook_account-6.8.11/__init__.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     1356 2023-07-25 20:04:33.000000 mds_cashbook_account-6.8.11/book.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     4273 2023-05-24 05:54:42.000000 mds_cashbook_account-6.8.11/book.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     3229 2023-06-03 18:30:13.000000 mds_cashbook_account-6.8.11/category.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1048 2023-05-24 05:54:42.000000 mds_cashbook_account-6.8.11/category.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     1213 2023-06-03 16:30:29.000000 mds_cashbook_account-6.8.11/configuration.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      527 2023-05-24 05:54:42.000000 mds_cashbook_account-6.8.11/configuration.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    19546 2023-06-03 17:56:09.000000 mds_cashbook_account-6.8.11/line.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      491 2023-05-24 05:54:42.000000 mds_cashbook_account-6.8.11/line.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-25 20:12:44.126516 mds_cashbook_account-6.8.11/locale/
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     9470 2023-07-25 20:04:33.000000 mds_cashbook_account-6.8.11/locale/de.po
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     8546 2023-07-25 20:04:33.000000 mds_cashbook_account-6.8.11/locale/en.po
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-25 20:12:44.138517 mds_cashbook_account-6.8.11/mds_cashbook_account.egg-info/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1537 2023-07-25 20:12:43.000000 mds_cashbook_account-6.8.11/mds_cashbook_account.egg-info/PKG-INFO
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      933 2023-07-25 20:12:44.000000 mds_cashbook_account-6.8.11/mds_cashbook_account.egg-info/SOURCES.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-07-25 20:12:43.000000 mds_cashbook_account-6.8.11/mds_cashbook_account.egg-info/dependency_links.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       83 2023-07-25 20:12:43.000000 mds_cashbook_account-6.8.11/mds_cashbook_account.egg-info/entry_points.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-07-25 20:12:43.000000 mds_cashbook_account-6.8.11/mds_cashbook_account.egg-info/not-zip-safe
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       75 2023-07-25 20:12:43.000000 mds_cashbook_account-6.8.11/mds_cashbook_account.egg-info/requires.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2023-07-25 20:12:43.000000 mds_cashbook_account-6.8.11/mds_cashbook_account.egg-info/top_level.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2106 2023-05-24 05:54:42.000000 mds_cashbook_account-6.8.11/message.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      801 2023-05-24 05:54:42.000000 mds_cashbook_account-6.8.11/move.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      685 2023-05-24 05:54:42.000000 mds_cashbook_account-6.8.11/move.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    10834 2023-06-03 17:53:35.000000 mds_cashbook_account-6.8.11/netmixin.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2023-07-25 20:12:44.142516 mds_cashbook_account-6.8.11/setup.cfg
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     3633 2023-07-25 20:04:25.000000 mds_cashbook_account-6.8.11/setup.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      987 2023-07-25 20:04:33.000000 mds_cashbook_account-6.8.11/splitline.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      495 2023-05-24 05:54:42.000000 mds_cashbook_account-6.8.11/splitline.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     4220 2023-07-25 20:04:33.000000 mds_cashbook_account-6.8.11/tax.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      794 2023-05-24 05:54:42.000000 mds_cashbook_account-6.8.11/tax.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-25 20:12:44.134516 mds_cashbook_account-6.8.11/tests/
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      144 2023-06-03 17:53:50.000000 mds_cashbook_account-6.8.11/tests/__init__.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     2980 2023-06-03 16:30:29.000000 mds_cashbook_account-6.8.11/tests/category.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)   253622 2023-06-03 18:02:50.000000 mds_cashbook_account-6.8.11/tests/line.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      551 2023-06-03 17:53:35.000000 mds_cashbook_account-6.8.11/tests/test_module.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      187 2023-07-25 20:05:19.000000 mds_cashbook_account-6.8.11/tryton.cfg
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)       28 2023-07-25 20:05:13.000000 mds_cashbook_account-6.8.11/versiondep.txt
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-25 20:12:44.138517 mds_cashbook_account-6.8.11/view/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      622 2023-05-24 05:54:42.000000 mds_cashbook_account-6.8.11/view/book_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      331 2023-05-24 05:54:42.000000 mds_cashbook_account-6.8.11/view/book_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      680 2023-05-24 05:54:42.000000 mds_cashbook_account-6.8.11/view/category_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      332 2023-05-24 05:54:42.000000 mds_cashbook_account-6.8.11/view/category_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      333 2023-05-24 05:54:42.000000 mds_cashbook_account-6.8.11/view/category_tree.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      336 2023-05-24 05:54:42.000000 mds_cashbook_account-6.8.11/view/configuration_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1861 2023-05-24 05:54:42.000000 mds_cashbook_account-6.8.11/view/line_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1520 2023-05-24 05:54:42.000000 mds_cashbook_account-6.8.11/view/split_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      542 2023-05-24 05:54:42.000000 mds_cashbook_account-6.8.11/view/tax_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      380 2023-05-24 05:54:42.000000 mds_cashbook_account-6.8.11/view/tax_list.xml
```

### Comparing `mds_cashbook_account-6.0.9/PKG-INFO` & `mds_cashbook_account-6.8.11/mds_cashbook_account.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: mds_cashbook_account
-Version: 6.0.9
+Name: mds-cashbook-account
+Version: 6.8.11
 Summary: Tryton module to add accounts to cashbook.
 Home-page: https://www.m-ds.de/
 Author: martin-data services
 Author-email: service@m-ds.de
 License: GPL-3
 Description: mds-cashbook-account
         ====================
@@ -13,56 +13,24 @@
         Install
         =======
         
         pip install mds-cashbook-account
         
         Requires
         ========
-        - Tryton 6.0
+        - Tryton 6.8
         
         Changes
         =======
         
-        *6.0.9 - 14.02.2023*
+        *6.8.11 - 25.07.2023*
         
-        - fix: form-xpath, rec_name in tax
+        - updt: optimize code, add tooltips
         
-        *6.0.8 - 04.10.2022*
-        
-        - updt: optimized second currency support
-        
-        *6.0.7 - 30.09.2022*
-        
-        - add: taxes
-        
-        *6.0.6 - 13.09.2022*
-        
-        - booking of transfer in split-line
-        
-        *6.0.5 - 07.09.2022*
-        
-        - updt: permissions
-        
-        *6.0.4 - 05.09.2022*
-        
-        - updt: view of book optimized
-        
-        *6.0.3 - 05.09.2022*
-        
-        - fix: category view
-        
-        *6.0.2 - 25.08.2022*
-        
-        - add: split-bookings
-        
-        *6.0.1 - 23.08.2022*
-        
-        - works
-        
-        *6.0.0 - 15.08.2022*
+        *6.8.10 - 05.06.2023*
         
         - init
         
 Keywords: tryton cashbook account
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
@@ -75,7 +43,8 @@
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Natural Language :: German
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mds_cashbook_account-6.0.9/__init__.py` & `mds_cashbook_account-6.8.11/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from .book import Book
 from .configuration import Configuration, UserConfiguration
 from .line import Line
 from .tax import TaxLine
 from .move import Move, MoveLine
 from .splitline import SplitLine
 
+
 def register():
     Pool.register(
         Configuration,
         UserConfiguration,
         Category,
         Book,
         Line,
```

### Comparing `mds_cashbook_account-6.0.9/book.py` & `mds_cashbook_account-6.8.11/book.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,26 +8,31 @@
 from trytond.pyson import Eval, Bool
 from trytond.modules.cashbook.book import STATES2, DEPENDS2
 
 
 class Book(metaclass=PoolMeta):
     __name__ = 'cashbook.book'
 
-    account = fields.Many2One(string='Account', select=True,
+    account = fields.Many2One(
+        string='Account',
         model_name='account.account', ondelete='RESTRICT',
         states=STATES2, depends=DEPENDS2+['company'],
         domain=[('company.id', '=', Eval('company', -1))])
-    journal = fields.Many2One(string='Journal', ondelete='RESTRICT',
+    journal = fields.Many2One(
+        string='Journal', ondelete='RESTRICT',
+        help='Created account move records are assigned to this journal.',
         model_name='account.journal',
         states={
             'readonly': STATES2['readonly'],
             'required': Bool(Eval('account')),
         }, depends=DEPENDS2+['account'])
-    party_account = fields.Boolean(string='Involve party accounts',
-        help='The Receivable/Payable accounts of the party are included in move line records.',
+    party_account = fields.Boolean(
+        string='Involve party accounts',
+        help='The Receivable/Payable accounts of the party are' +
+        ' included in move line records.',
         states=STATES2, depends=DEPENDS2)
 
     @classmethod
     def default_party_account(cls):
         """ default: true
         """
         return True
```

### Comparing `mds_cashbook_account-6.0.9/book.xml` & `mds_cashbook_account-6.8.11/book.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook_account-6.0.9/category.py` & `mds_cashbook_account-6.8.11/category.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,56 @@
 # -*- coding: utf-8 -*-
 # This file is part of the cashbook-module from m-ds for Tryton.
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
-from trytond.model import fields, Unique
+from trytond.model import fields, Unique, Index
 from trytond.pool import Pool, PoolMeta
 from trytond.pyson import Eval, Bool
 
 
 STATES = {
     'readonly': ~Bool(Eval('account')),
     }
-DEPENDS=['account']
+DEPENDS = ['account']
 
 
 class Category(metaclass=PoolMeta):
     __name__ = 'cashbook.category'
 
-    account = fields.Many2One(string='Account', select=True,
+    account = fields.Many2One(
+        string='Account',
         model_name='account.account', ondelete='RESTRICT')
-    account_code = fields.Function(fields.Char(string='Account', readonly=True),
+    account_code = fields.Function(fields.Char(
+        string='Account', readonly=True),
         'on_change_with_account_code', searcher='search_account_code')
-    tax0 = fields.Many2One(string='Tax Null', model_name='account.tax',
+    tax0 = fields.Many2One(
+        string='Tax Null', model_name='account.tax',
         ondelete='RESTRICT', states=STATES, depends=DEPENDS)
-    tax1 = fields.Many2One(string='Tax Half', model_name='account.tax',
+    tax1 = fields.Many2One(
+        string='Tax Half', model_name='account.tax',
         ondelete='RESTRICT', states=STATES, depends=DEPENDS)
-    tax2 = fields.Many2One(string='Tax Full', model_name='account.tax',
+    tax2 = fields.Many2One(
+        string='Tax Full', model_name='account.tax',
         ondelete='RESTRICT', states=STATES, depends=DEPENDS)
 
     @classmethod
     def __setup__(cls):
         super(Category, cls).__setup__()
         t = cls.__table__()
         cls._sql_constraints.extend([
                 ('account_uniq',
                     Unique(t, t.account, t.company),
                     'cashbook_account.msg_category_account_unique'),
             ])
+        cls._sql_indexes.update({
+            Index(
+                t,
+                (t.account, Index.Equality())),
+            })
 
     @fields.depends('account', 'tax0', 'tax1', 'tax2')
     def on_change_account(self):
         """ clear taxes if account is removed
         """
         if self.account is None:
             self.tax0 = None
@@ -68,15 +78,16 @@
                 super(Category, self).get_rec_name(name)
             )
 
     @classmethod
     def search_rec_name(cls, name, clause):
         """ search in account + name
         """
-        return ['OR',
+        return [
+            'OR',
             super(Category, cls).search_rec_name(name, clause),
             ('account.rec_name',) + tuple(clause[1:]),
             ('account.code',) + tuple(clause[1:]),
             ]
 
     @fields.depends('account')
     def on_change_with_account_code(self, name=None):
```

### Comparing `mds_cashbook_account-6.0.9/category.xml` & `mds_cashbook_account-6.8.11/category.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook_account-6.0.9/configuration.py` & `mds_cashbook_account-6.8.11/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
 from trytond.model import fields
 from trytond.pool import Pool, PoolMeta
 
 
-field_cataccno = fields.Boolean(string='Category: Show account number',
+field_cataccno = fields.Boolean(
+    string='Category: Show account number',
     help='Shows the number of the linked account in the name of a category.')
 
 
 class Configuration(metaclass=PoolMeta):
     __name__ = 'cashbook.configuration'
 
     cataccno = fields.MultiValue(field_cataccno)
```

### Comparing `mds_cashbook_account-6.0.9/configuration.xml` & `mds_cashbook_account-6.8.11/configuration.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook_account-6.0.9/line.py` & `mds_cashbook_account-6.8.11/line.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,64 +6,70 @@
 from trytond.model import fields
 from trytond.pool import PoolMeta, Pool
 from trytond.pyson import Eval, And, Bool, Or
 from trytond.exceptions import UserError
 from trytond.i18n import gettext
 from trytond.transaction import Transaction
 from decimal import Decimal
-from trytond.modules.cashbook.line import STATES, DEPENDS
 from .netmixin import NetMixin
 
 
-dep_taxena = ['ena_tax0', 'ena_tax1', 'ena_tax2', 'amount', 'taxes', 'category',
+dep_taxena = [
+    'ena_tax0', 'ena_tax1', 'ena_tax2', 'amount', 'taxes', 'category',
     'date', 'currency', '_parent_category.tax0', '_parent_category.tax1',
     '_parent_category.tax2']
-dep_taxes = dep_taxena + ['amount_tax0', 'amount_tax1', 'amount_tax2', 'amount_net']
+dep_taxes = dep_taxena + [
+    'amount_tax0', 'amount_tax1', 'amount_tax2', 'amount_net']
 dep_bookingtype = dep_taxena+['bookingtype', 'category', 'splitlines']
 
 
 class Line(NetMixin, metaclass=PoolMeta):
     __name__ = 'cashbook.line'
 
-    taxes = fields.One2Many(string='Tax Lines', field='line',
+    taxes = fields.One2Many(
+        string='Tax Lines', field='line',
         model_name='cashbook_account.tax', readonly=True,
         states={
             'invisible': ~Or(
                     And(
                         Eval('bookingtype', '').in_(['in', 'out']),
                         Bool(Eval('category')),
                     ),
                     Eval('bookingtype', '').in_(['spin', 'spout']),
                 ),
         }, depends=['category', 'bookingtype'])
-    moves = fields.One2Many(string='Moves', model_name='account.move',
+    moves = fields.One2Many(
+        string='Moves', model_name='account.move',
         field='origin', readonly=True, size=1,
         states={
             'invisible': ~Bool(Eval('moves')),
         })
-    account_cashbook = fields.Function(fields.Many2One(readonly=True,
+    account_cashbook = fields.Function(fields.Many2One(
+        readonly=True,
         string='Account Cashbook', model_name='account.account',
         states={'invisible': True}),
         'on_change_with_account_cashbook')
-    party_required = fields.Function(fields.Boolean(string='Party required',
+    party_required = fields.Function(fields.Boolean(
+        string='Party required',
         readonly=True, states={'invisible': True}),
         'on_change_with_party_required')
 
     @classmethod
     def __setup__(cls):
         super(Line, cls).__setup__()
         requ_cond = And(
                 Eval('bookingtype', '').in_(['in', 'out']),
                 Eval('party_required', False) == True,
             )
         if cls.party.states.get('required', None) is None:
             cls.party.states['required'] = requ_cond
-        else :
-            cls.party.states['required'] = Or(cls.party.states['required'], requ_cond)
-        cls.party.depends.append('party_required')
+        else:
+            cls.party.states['required'] = Or(
+                cls.party.states['required'], requ_cond)
+        cls.party.depends.add('party_required')
 
     @classmethod
     def wfedit(cls, lines):
         """ delete moves
         """
         Move = Pool().get('account.move')
 
@@ -107,15 +113,15 @@
 
                 if (line.bookingtype in ['out', 'in']):
                     move_lines.extend(cls.get_move_lines_by_category(line))
                 elif (line.bookingtype in ['spout', 'spin']):
                     move_lines.extend(cls.get_move_lines_by_splitbooking(line))
                 elif (line.bookingtype in ['mvout', 'mvin']):
                     move_lines.extend(cls.get_move_lines_by_transfer(line))
-                else :
+                else:
                     raise ValueError('invalid bookingtype')
 
                 move_data['lines'].append(('create', move_lines))
                 to_create_move.append(move_data)
 
         if len(to_create_move) > 0:
             Move.create(to_create_move)
@@ -133,15 +139,17 @@
         to_post = []
         to_reconcile = []
         for line in lines:
             for move in line.moves:
                 if move.state == 'draft':
                     to_post.append(move)
 
-                recon_lines = [move_line for move_line in move.lines if move_line.party]
+                recon_lines = [
+                    move_line for move_line in move.lines
+                    if move_line.party]
                 if len(recon_lines) > 0:
                     to_reconcile.append(recon_lines)
         Move.post(to_post)
         Line2.reconcile(*to_reconcile)
 
     @fields.depends(*dep_taxes)
     def on_change_taxes(self):
@@ -154,15 +162,15 @@
 
     def update_taxes(self):
         """ update tax_line-records
         """
         TaxLine = Pool().get('cashbook_account.tax')
 
         taxes = self.get_list_of_taxes()
-        tax_dict = {x['tax'].id:x for x in taxes}
+        tax_dict = {x['tax'].id: x for x in taxes}
 
         to_delete = []
         for tax_line in self.taxes:
             if tax_line.splitline is not None:
                 continue
 
             if tax_line.tax.id not in tax_dict.keys():
@@ -179,19 +187,17 @@
             if tax in to_delete:
                 continue
             l1.append(tax)
 
         # add missing taxes
         for tax in tax_dict.keys():
             l1.append(TaxLine(
-                amount = tax_dict[tax]['amount'],
-                base =  tax_dict[tax]['base'],
-                tax =  tax_dict[tax]['tax'],
-                splitline = None,
-                ))
+                amount=tax_dict[tax]['amount'],
+                base=tax_dict[tax]['base'],
+                tax=tax_dict[tax]['tax'], splitline=None))
         self.taxes = l1
 
     @fields.depends(*dep_bookingtype)
     def on_change_bookingtype(self):
         """ update category
         """
         super(Line, self).on_change_bookingtype()
@@ -237,15 +243,15 @@
 
     @classmethod
     def get_inverted_move_values(cls, values):
         """ credit -> debit, debit, -> credit etc.
         """
         if values['amount_second_currency'] is None:
             amount = None
-        else :
+        else:
             amount = values['amount_second_currency'].copy_negate()
 
         return {
             'credit': values['debit'],
             'debit': values['credit'],
             'second_currency': values['second_currency'],
             'amount_second_currency': amount,
@@ -269,45 +275,45 @@
         if line.cashbook.currency.id != line.cashbook.company.currency.id:
             amounts['amount_second_currency'] = amount.copy_sign(
                     amounts['debit'] - amounts['credit']
                 )
             amounts['second_currency'] = line.cashbook.currency.id
 
         with Transaction().set_context({
-            'date': line.date,
-            }):
+                'date': line.date}):
             for x in ['credit', 'debit']:
-                if line.cashbook.currency.id != line.cashbook.company.currency.id:
+                if line.cashbook.currency.id != \
+                        line.cashbook.company.currency.id:
                     amounts[x] = Currency.compute(
                         line.cashbook.currency,
                         amounts[x],
                         line.cashbook.company.currency)
         return amounts
 
     @classmethod
     def get_article_lines(cls, line, description=None):
         """ get move-line of article
         """
         def get_taxline_amount(moveline):
             return moveline['debit'] - moveline['credit'] \
                 if line.bookingtype.endswith('out') \
-                        else moveline['credit'] - moveline['debit']
+                else moveline['credit'] - moveline['debit']
 
         move_lines = []
 
         # total-amount converted to company-currency
         total_amount = cls.get_move_amounts(line, line.amount)
 
         # line: category-account
         # convert to company currency
         move_line = {
             'account': line.category.account.id,
             'description': description,
-            'origin': (line.__name__, line.id) \
-                if line.__name__ == 'cashbook.split' else None,
+            'origin': (line.__name__, line.id)
+            if line.__name__ == 'cashbook.split' else None,
             }
         move_line.update(cls.get_move_amounts(
             line,
             line.amount if line.amount_net is None else line.amount_net,
             ))
 
         if len(line.taxes) > 0:
@@ -327,22 +333,22 @@
             elif line.__name__ == 'cashbook.split':
                 # skip tax-lines for other split-lines
                 if getattr(tax.splitline, 'id', None) != line.id:
                     continue
 
             if tax.amount >= Decimal('0.0'):
                 tax_account = tax.tax.invoice_account.id
-            else :
+            else:
                 tax_account = tax.tax.credit_note_account.id
 
             move_line = {
                 'account': tax_account,
                 'description': description,
-                'origin': (line.__name__, line.id) \
-                    if line.__name__ == 'cashbook.split' else None,
+                'origin': (line.__name__, line.id)
+                if line.__name__ == 'cashbook.split' else None,
                 }
             move_line.update(cls.get_move_amounts(
                 line,
                 tax.amount,
                 ))
             # tax line
             move_line['tax_lines'] = [('create', [{
@@ -355,70 +361,71 @@
         # check rounding errors debit/credit/2ndcurrency
         # fix it in last line
         move_lines[-1]['debit'] -= sum(x['debit'] for x in move_lines) - \
             total_amount['debit']
         move_lines[-1]['credit'] -= sum(x['credit'] for x in move_lines) - \
             total_amount['credit']
         if len(move_lines) > 1:
-            move_lines[-1]['tax_lines'][0][1][0]['amount'] = get_taxline_amount(move_lines[-1])
+            move_lines[-1]['tax_lines'][0][1][0]['amount'] = \
+                get_taxline_amount(move_lines[-1])
 
         if total_amount['amount_second_currency'] is not None:
             move_lines[-1]['amount_second_currency'] -= \
                 sum(x['amount_second_currency'] for x in move_lines) - \
                 total_amount['amount_second_currency']
         return move_lines
 
     @classmethod
     def get_cashbook_lines(cls, line, amounts, description=None):
         """ get move-line of cashbook-transfer
         """
         move_line = {
             'account': line.booktransf.account.id,
             'description': description,
-            'origin': (line.__name__, line.id) \
-                if line.__name__ == 'cashbook.split' else None,
+            'origin': (line.__name__, line.id)
+            if line.__name__ == 'cashbook.split' else None,
             }
         move_line.update(amounts)
         return [move_line]
 
     @classmethod
     def get_move_lines_by_splitbooking(cls, line):
         """ create move lines for splitbooking
         """
         # select account of party if enabled
-        if line.cashbook.party_account == True:
+        if line.cashbook.party_account is True:
             if line.bookingtype == 'spout':
                 party_account = line.party.account_payable_used.id
             elif line.bookingtype == 'spin':
                 party_account = line.party.account_receivable_used.id
-            else :
+            else:
                 raise ValueError('invalid bookingtype: %s' % line.bookingtype)
-        else :
+        else:
             party_account = None
 
         # amounts of split-lines can be in 2nd-currency,
         # compute to company-currency
         move_lines = []
         for spline in line.splitlines:
             if spline.splittype == 'cat':
                 if spline.category.account is None:
                     raise UserError(gettext(
                         'cashbook_account.msg_line_missing_category_account',
-                        catname = spline.category.rec_name,
-                        ))
-                move_lines.extend(cls.get_article_lines(spline, spline.description))
+                        catname=spline.category.rec_name))
+                move_lines.extend(cls.get_article_lines(
+                    spline, spline.description))
             elif spline.splittype == 'tr':
                 if spline.booktransf.account is None:
                     raise UserError(gettext(
                         'cashbook_account.msg_line_missing_book_account',
-                        bookname = spline.booktransf.rec_name,
-                        ))
+                        bookname=spline.booktransf.rec_name))
                 amounts = cls.get_move_amounts(spline, spline.amount)
-                move_lines.extend(cls.get_cashbook_lines(spline, amounts, spline.description))
-            else :
+                move_lines.extend(cls.get_cashbook_lines(
+                    spline, amounts, spline.description))
+            else:
                 raise ValueError('invalid splittype: %s' % spline.splittype)
 
         # book-line
         book_line = {
             'account': line.cashbook.account.id,
             }
         amounts = cls.get_move_amounts(line, line.amount)
@@ -449,24 +456,23 @@
     @classmethod
     def get_move_lines_by_category(cls, line):
         """ create move lines if a category and party was used
         """
         if line.category.account is None:
             raise UserError(gettext(
                 'cashbook_account.msg_line_missing_category_account',
-                catname = line.category.rec_name,
-                ))
+                catname=line.category.rec_name))
 
         # select account of party if enabled
-        if line.cashbook.party_account == True:
+        if line.cashbook.party_account is True:
             if (line.debit - line.credit) >= Decimal('0.0'):
                 party_account = line.party.account_payable_used.id
-            else :
+            else:
                 party_account = line.party.account_receivable_used.id
-        else :
+        else:
             party_account = None
 
         # gross-amounts of line with 2nd currency
         # convert to company-currency
         amounts = cls.get_move_amounts(line, line.amount)
         amounts_invers = cls.get_inverted_move_values(amounts)
 
@@ -506,16 +512,15 @@
     def get_move_lines_by_transfer(cls, line):
         """ create move lines if amount was transferred
             between cashbooks
         """
         if line.booktransf.account is None:
             raise UserError(gettext(
                 'cashbook_account.msg_line_missing_book_account',
-                bookname = line.booktransf.rec_name,
-                ))
+                bookname=line.booktransf.rec_name))
 
         # target-book-account
         amounts = cls.get_move_amounts(line, line.amount)
         amounts_invers = cls.get_inverted_move_values(amounts)
 
         move_line = {'account': line.booktransf.account.id}
         move_line.update(amounts)
@@ -546,22 +551,22 @@
         """
         Configuration = Pool().get('cashbook.configuration')
 
         if self.category:
             cfg1 = Configuration.get_singleton()
 
             cat_name = super(Line, self).on_change_with_category_view(name)
-            if getattr(cfg1, 'catnamelong', True) == True:
+            if getattr(cfg1, 'catnamelong', True) is True:
                 return cat_name
-            else :
+            else:
                 return self.category.get_long_recname(cat_name)
 
     @classmethod
     def search_category_view(cls, name, clause):
         """ search in category
         """
-        return ['OR',
+        return [
+            'OR',
             super(Line, cls).search_category_view(name, clause),
-            ('category.account.code',) + tuple(clause[1:]),
-            ]
+            ('category.account.code',) + tuple(clause[1:])]
 
 # end Line
```

### Comparing `mds_cashbook_account-6.0.9/locale/de.po` & `mds_cashbook_account-6.8.11/locale/de.po`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,18 @@
 msgid "Account"
 msgstr "Konto"
 
 msgctxt "field:cashbook.book,journal:"
 msgid "Journal"
 msgstr "Journal"
 
+msgctxt "help:cashbook.book,journal:"
+msgid "Created account move records are assigned to this journal."
+msgstr "Erstellte Buchungssätze werden diesem Journal zugeordnet."
+
 msgctxt "field:cashbook.book,party_account:"
 msgid "Involve party accounts"
 msgstr "Parteikonten einbeziehen"
 
 msgctxt "help:cashbook.book,party_account:"
 msgid "The Receivable/Payable accounts of the party are included in move line records."
 msgstr "Die Forderungen/Verbindlichkeiten-Konten der Partei werden in Buchungssätzen einbezogen."
```

### Comparing `mds_cashbook_account-6.0.9/locale/en.po` & `mds_cashbook_account-6.8.11/locale/en.po`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,18 @@
 msgid "Account"
 msgstr "Account"
 
 msgctxt "field:cashbook.book,journal:"
 msgid "Journal"
 msgstr "Journal"
 
+msgctxt "help:cashbook.book,journal:"
+msgid "Created account move records are assigned to this journal."
+msgstr "Created account move records are assigned to this journal."
+
 msgctxt "field:cashbook.book,party_account:"
 msgid "Involve party accounts"
 msgstr "Involve party accounts"
 
 msgctxt "help:cashbook.book,party_account:"
 msgid "The Receivable/Payable accounts of the party are included in move line records."
 msgstr "The Receivable/Payable accounts of the party are included in move line records."
```

### Comparing `mds_cashbook_account-6.0.9/mds_cashbook_account.egg-info/PKG-INFO` & `mds_cashbook_account-6.8.11/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: mds-cashbook-account
-Version: 6.0.9
+Name: mds_cashbook_account
+Version: 6.8.11
 Summary: Tryton module to add accounts to cashbook.
 Home-page: https://www.m-ds.de/
 Author: martin-data services
 Author-email: service@m-ds.de
 License: GPL-3
 Description: mds-cashbook-account
         ====================
@@ -13,56 +13,24 @@
         Install
         =======
         
         pip install mds-cashbook-account
         
         Requires
         ========
-        - Tryton 6.0
+        - Tryton 6.8
         
         Changes
         =======
         
-        *6.0.9 - 14.02.2023*
+        *6.8.11 - 25.07.2023*
         
-        - fix: form-xpath, rec_name in tax
+        - updt: optimize code, add tooltips
         
-        *6.0.8 - 04.10.2022*
-        
-        - updt: optimized second currency support
-        
-        *6.0.7 - 30.09.2022*
-        
-        - add: taxes
-        
-        *6.0.6 - 13.09.2022*
-        
-        - booking of transfer in split-line
-        
-        *6.0.5 - 07.09.2022*
-        
-        - updt: permissions
-        
-        *6.0.4 - 05.09.2022*
-        
-        - updt: view of book optimized
-        
-        *6.0.3 - 05.09.2022*
-        
-        - fix: category view
-        
-        *6.0.2 - 25.08.2022*
-        
-        - add: split-bookings
-        
-        *6.0.1 - 23.08.2022*
-        
-        - works
-        
-        *6.0.0 - 15.08.2022*
+        *6.8.10 - 05.06.2023*
         
         - init
         
 Keywords: tryton cashbook account
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
@@ -75,7 +43,8 @@
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Natural Language :: German
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mds_cashbook_account-6.0.9/mds_cashbook_account.egg-info/SOURCES.txt` & `mds_cashbook_account-6.8.11/mds_cashbook_account.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -19,16 +19,17 @@
 ./tax.py
 ./tax.xml
 ./tryton.cfg
 ./versiondep.txt
 ./locale/de.po
 ./locale/en.po
 ./tests/__init__.py
-./tests/test_category.py
-./tests/test_line.py
+./tests/category.py
+./tests/line.py
+./tests/test_module.py
 ./view/book_form.xml
 ./view/book_list.xml
 ./view/category_form.xml
 ./view/category_list.xml
 ./view/category_tree.xml
 ./view/configuration_form.xml
 ./view/line_form.xml
```

### Comparing `mds_cashbook_account-6.0.9/message.xml` & `mds_cashbook_account-6.8.11/message.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook_account-6.0.9/move.py` & `mds_cashbook_account-6.8.11/move.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook_account-6.0.9/move.xml` & `mds_cashbook_account-6.8.11/move.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook_account-6.0.9/netmixin.py` & `mds_cashbook_account-6.8.11/netmixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,75 +3,86 @@
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
 
 from trytond.model import fields
 from trytond.exceptions import UserError
 from trytond.i18n import gettext
-from trytond.pyson import Eval, And, Or, Bool
+from trytond.pyson import Eval, Or, Bool
 from trytond.pool import Pool
 from trytond.modules.cashbook.line import STATES, DEPENDS
 from decimal import Decimal
 
 
-dep_taxena = ['ena_tax0', 'amount_tax0','ena_tax1', 'amount_tax1',
+dep_taxena = [
+    'ena_tax0', 'amount_tax0', 'ena_tax1', 'amount_tax1',
     'ena_tax2', 'amount_tax2', 'amount_net', 'amount', 'category']
 
 
 class NetMixin:
-    amount_net = fields.Function(fields.Numeric(string='Net',
-        help='Net Amount of current booking.', readonly=True,
+    """ compute net amount
+    """
+    __slots__ = ()
+
+    amount_net = fields.Function(fields.Numeric(
+        string='Net', help='Net Amount of current booking.', readonly=True,
         digits=(16, Eval('currency_digits', 2)),
         states={
             'invisible': ~Bool(Eval('category')),
         }, depends=['currency_digits', 'category']),
         'on_change_with_amount_net')
 
-    ena_tax0 = fields.Boolean(string='Tax Null',
+    ena_tax0 = fields.Boolean(
+        string='Tax Null',
         states={
             'readonly': Or(
                 STATES['readonly'],
                 Eval('avail_tax0', False) == False,
                 ),
         }, depends=DEPENDS+['avail_tax0'])
-    amount_tax0 = fields.Function(fields.Numeric(string='Tax Null',
-        digits=(16, Eval('currency_digits', 2)), readonly=True,
-        depends=['currency_digits']),
+    amount_tax0 = fields.Function(fields.Numeric(
+        string='Tax Null', digits=(16, Eval('currency_digits', 2)),
+        readonly=True, depends=['currency_digits']),
         'on_change_with_amount_tax0')
 
-    ena_tax1 = fields.Boolean(string='Tax Half',
+    ena_tax1 = fields.Boolean(
+        string='Tax Half',
         states={
             'readonly': Or(
                 STATES['readonly'],
                 Eval('avail_tax1', False) == False,
                 ),
         }, depends=DEPENDS+['avail_tax1'])
-    amount_tax1 = fields.Function(fields.Numeric(string='Tax Half',
-        digits=(16, Eval('currency_digits', 2)), readonly=True,
-        depends=['currency_digits']),
+    amount_tax1 = fields.Function(fields.Numeric(
+        string='Tax Half', digits=(16, Eval('currency_digits', 2)),
+        readonly=True, depends=['currency_digits']),
         'on_change_with_amount_tax1')
 
-    ena_tax2 = fields.Boolean(string='Tax Full',
+    ena_tax2 = fields.Boolean(
+        string='Tax Full',
         states={
             'readonly': Or(
                 STATES['readonly'],
                 Eval('avail_tax2', False) == False,
                 ),
         }, depends=DEPENDS+['avail_tax2'])
-    amount_tax2 = fields.Function(fields.Numeric(string='Tax Full',
-        digits=(16, Eval('currency_digits', 2)), readonly=True,
-        depends=['currency_digits']),
+    amount_tax2 = fields.Function(fields.Numeric(
+        string='Tax Full', digits=(16, Eval('currency_digits', 2)),
+        readonly=True, depends=['currency_digits']),
         'on_change_with_amount_tax2')
 
-    avail_tax0 = fields.Function(fields.Boolean(string='Tax Null available',
-        states={'invisible': True}, readonly=True), 'on_change_with_avail_tax0')
-    avail_tax1 = fields.Function(fields.Boolean(string='Tax Half available',
-        states={'invisible': True}, readonly=True), 'on_change_with_avail_tax1')
-    avail_tax2 = fields.Function(fields.Boolean(string='Tax Full available',
-        states={'invisible': True}, readonly=True), 'on_change_with_avail_tax2')
+    avail_tax0 = fields.Function(fields.Boolean(
+        string='Tax Null available', states={'invisible': True},
+        readonly=True), 'on_change_with_avail_tax0')
+    avail_tax1 = fields.Function(fields.Boolean(
+        string='Tax Half available', states={'invisible': True},
+        readonly=True), 'on_change_with_avail_tax1')
+    avail_tax2 = fields.Function(fields.Boolean(
+        string='Tax Full available', states={'invisible': True},
+        readonly=True), 'on_change_with_avail_tax2')
 
     @classmethod
     def default_ena_tax0(cls):
         """ default: False
         """
         return False
 
@@ -100,32 +111,32 @@
 
         # get enabled tax-fields
         taxes = []
         for x in range(3):
             if getattr(self.category, 'tax%d' % x, None) is None:
                 continue
 
-            if getattr(self, 'ena_tax%d' % x) == True:
+            if getattr(self, 'ena_tax%d' % x) is True:
                 taxes.append(getattr(self.category, 'tax%d' % x))
 
         if len(taxes) == 0:
             return []
 
         if self.date is None:
             date_line = IrDate.today()
-        else :
+        else:
             date_line = self.date
 
         # get net from gross and taxes
         net_amount = self.currency.round(
                 Tax.reverse_compute(self.amount, taxes, date_line))
 
         # get taxes from net
         tax_lines = Tax.compute(taxes, net_amount, Decimal('1.0'), date_line)
-        total = self.amount # gross
+        total = self.amount     # gross
         tax_lines2 = []
         for tax_line in tax_lines:
             tax_lines2.append({
                 'amount': self.currency.round(tax_line['amount']),
                 'tax': tax_line['tax'],
                 })
             # gross - tax = net
@@ -138,46 +149,45 @@
     @fields.depends('taxes')
     def on_change_with_amount_net(self, name=None):
         """ compute net from tax-lines
         """
         # one or more lines - we use 'base'
         for tax_line in self.taxes:
             if (self.__name__ == 'cashbook.line') and \
-                (tax_line.splitline is not None):
+                    (tax_line.splitline is not None):
                 # tax-lines for split-bookings are store here
                 # skip them
                 continue
             return tax_line.base
         return None
 
     def mxin_compute_tax_amount(self, tax_no):
         """ compute tax for selected line
         """
         pool = Pool()
-        TaxLine = pool.get('cashbook_account.tax')
         Tax = pool.get('account.tax')
 
         tax_amount = None
         if self.category:
             tax_select = getattr(self.category, 'tax%d' % tax_no, None)
             if tax_select:
                 for tax_line in self.taxes:
 
                     if (self.__name__ == 'cashbook.line') and \
-                        (tax_line.splitline is not None):
+                            (tax_line.splitline is not None):
                         continue
 
                     if tax_line.tax is None:
                         continue
 
                     # check if current line relates to selected tax
                     if Tax.search_count([
-                        ('parent', 'child_of', tax_select.id),
-                        ('id', '=', tax_line.tax.id),
-                        ]) > 0:
+                            ('parent', 'child_of', tax_select.id),
+                            ('id', '=', tax_line.tax.id),
+                            ]) > 0:
                         if tax_amount is None:
                             tax_amount = Decimal('0.0')
                         tax_amount += tax_line.amount
         return tax_amount
 
     @fields.depends('taxes', 'category', '_parent_category.tax0')
     def on_change_with_amount_tax0(self, name=None):
@@ -236,39 +246,42 @@
 
     @classmethod
     def check_tax_amounts(cls, lines):
         """ check amounts and taxes
         """
         for line in lines:
             if line.__name__ == 'cashbook.line':
-                if not line.bookingtype in ['in', 'out']:
+                if line.bookingtype not in ['in', 'out']:
                     for x in range(3):
-                        if getattr(line, 'ena_tax%d' % x) != False:
+                        if getattr(line, 'ena_tax%d' % x) is True:
                             raise UserError(gettext(
                                 'cashbook_account.msg_line_tax_must_disabled',
-                                linename = line.rec_name,
-                                ))
+                                linename=line.rec_name))
 
     @classmethod
     def get_taxlines_updates(cls, records):
         """ get to_create, to_delete
         """
         to_del = []
         to_create = []
         for record in records:
             if record.__name__ == 'cashbook.line':
                 to_del.extend([x for x in record.taxes if x.splitline is None])
             elif record.__name__ == 'cashbook.split':
-                to_del.extend([x for x in record.taxes if getattr(x.splitline, 'id', None) == record.id])
+                to_del.extend([
+                    x for x in record.taxes
+                    if getattr(x.splitline, 'id', None) == record.id])
 
             lines = []
             for tax in record.get_list_of_taxes():
                 r1 = {
-                    'line': record.id if record.__name__ == 'cashbook.line' else record.line.id,
-                    'splitline': None if record.__name__ == 'cashbook.line' else record.id,
+                    'line': record.id
+                    if record.__name__ == 'cashbook.line' else record.line.id,
+                    'splitline': None
+                    if record.__name__ == 'cashbook.line' else record.id,
                     }
                 r1.update(tax)
                 r1['tax'] = r1['tax'].id
                 lines.append(r1)
             if len(lines) > 0:
                 to_create.extend(lines)
         return (to_create, to_del)
@@ -294,16 +307,17 @@
         """ add/update tax-lines
         """
         TaxLine = Pool().get('cashbook_account.tax')
 
         to_update_record = []
         actions = iter(args)
         for records, values in zip(actions, actions):
-            if len(set({'amount', 'category', 'ena_tax0', 'ena_tax1',
-                'ena_tax2'}).intersection(values.keys())) > 0:
+            if len(set({
+                    'amount', 'category', 'ena_tax0', 'ena_tax1',
+                    'ena_tax2'}).intersection(values.keys())) > 0:
                 to_update_record.extend(records)
 
         super(NetMixin, cls).write(*args)
 
         (to_create, to_del) = cls.get_taxlines_updates(to_update_record)
 
         if len(to_del) > 0:
```

### Comparing `mds_cashbook_account-6.0.9/setup.py` & `mds_cashbook_account-6.8.11/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         l2 = i.strip().split(';')
         if len(l2) < 4:
             continue
         modversion[l2[0]] = {'min':l2[1], 'max':l2[2], 'prefix':l2[3]}
 
 # tryton-version
 major_version = 6
-minor_version = 0
+minor_version = 8
 
 requires = []
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res|webdav)(\W|$)', dep):
         if dep in modversion.keys():
             prefix = 'mds'
             if len(modversion[dep]['prefix']) > 0:
@@ -83,14 +83,15 @@
     'Topic :: Office/Business :: Financial :: Accounting',
     'Natural Language :: German',
     'Natural Language :: English',
     'Operating System :: OS Independent',
     'License :: OSI Approved :: GNU General Public License (GPL)',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
     ],
 
     keywords='tryton cashbook account',
     package_dir={'trytond.modules.%s' % MODULE: '.'},
     packages=[
         'trytond.modules.%s' % MODULE,
         ],
```

### Comparing `mds_cashbook_account-6.0.9/splitline.py` & `mds_cashbook_account-6.8.11/splitline.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # -*- coding: utf-8 -*-
 # This file is part of the cashbook-module from m-ds for Tryton.
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
 from trytond.model import fields
-from trytond.pool import PoolMeta
+from trytond.pool import PoolMeta, Pool
 from .netmixin import NetMixin
 
 
 class SplitLine(NetMixin, metaclass=PoolMeta):
     __name__ = 'cashbook.split'
 
-    taxes = fields.Function(fields.One2Many(string='Tax Lines', field=None,
+    taxes = fields.Function(fields.One2Many(
+        string='Tax Lines', field=None,
         model_name='cashbook_account.tax', readonly=True),
         'on_change_with_taxes')
 
     @fields.depends('line', '_parent_line.taxes')
     def on_change_with_taxes(self, name=None):
         """ get taxes for current split-line
         """
-        if self.line:
-            return [x.id for x in self.line.taxes
-                if getattr(x.splitline, 'id', None) == self.id]
+        Tax = Pool().get('cashbook_account.tax')
+
+        if self.line and self.id:
+            return [x.id for x in Tax.search([
+                    ('line', '=', self.line.id),
+                    ('splitline', '=', self.id)])]
         return []
 
 # end SplitLine
```

### Comparing `mds_cashbook_account-6.0.9/tax.py` & `mds_cashbook_account-6.8.11/tax.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,65 +1,87 @@
 # -*- coding: utf-8 -*-
 # This file is part of the cashbook-module from m-ds for Tryton.
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
 from decimal import Decimal
-from trytond.model import ModelView, ModelSQL, fields
-from trytond.pool import Pool
+from trytond.model import ModelView, ModelSQL, fields, Index
 from trytond.pyson import Eval
 from trytond.report import Report
-from trytond.exceptions import UserError
-from trytond.modules.cashbook.line import STATES, DEPENDS, sel_linetype, sel_bookingtype
+from trytond.modules.cashbook.line import (
+    STATES, DEPENDS, sel_linestate, sel_bookingtype)
 from trytond.modules.cashbook.book import sel_state_book
 
 
 class TaxLine(ModelSQL, ModelView):
     'Tax Line'
     __name__ = 'cashbook_account.tax'
 
-    line = fields.Many2One(string='Line', model_name='cashbook.line',
-        readonly=True, select=True, required=True, ondelete='CASCADE')
-    splitline = fields.Many2One(string='Split Booking', model_name='cashbook.split',
-        readonly=True, select=True, ondelete='CASCADE')
+    line = fields.Many2One(
+        string='Line', model_name='cashbook.line',
+        readonly=True, required=True, ondelete='CASCADE')
+    splitline = fields.Many2One(
+        string='Split Booking', model_name='cashbook.split',
+        readonly=True, ondelete='CASCADE')
 
-    tax = fields.Many2One(string='Tax', model_name='account.tax',
+    tax = fields.Many2One(
+        string='Tax', model_name='account.tax',
         states=STATES, depends=DEPENDS, required=True)
-    base = fields.Numeric(string='Base', required=True,
+    base = fields.Numeric(
+        string='Base', required=True,
         digits=(16, Eval('currency_digits', 2)),
         states=STATES, depends=DEPENDS+['currency_digits'])
-    amount = fields.Numeric(string='Amount', required=True,
+    amount = fields.Numeric(
+        string='Amount', required=True,
         digits=(16, Eval('currency_digits', 2)),
         states=STATES, depends=DEPENDS+['currency_digits'])
 
-    currency = fields.Function(fields.Many2One(model_name='currency.currency',
+    currency = fields.Function(fields.Many2One(
+        model_name='currency.currency',
         string="Currency", readonly=True), 'on_change_with_currency')
-    currency_digits = fields.Function(fields.Integer(string='Currency Digits',
+    currency_digits = fields.Function(fields.Integer(
+        string='Currency Digits',
         readonly=True), 'on_change_with_currency_digits')
-    bookingtype = fields.Function(fields.Selection(string='Type', readonly=True,
+    bookingtype = fields.Function(fields.Selection(
+        string='Type', readonly=True,
         selection=sel_bookingtype), 'on_change_with_bookingtype')
-    state = fields.Function(fields.Selection(string='State', readonly=True,
-        selection=sel_linetype), 'on_change_with_state')
-    state_cashbook = fields.Function(fields.Selection(string='State of Cashbook',
+    state = fields.Function(fields.Selection(
+        string='State', readonly=True,
+        selection=sel_linestate), 'on_change_with_state')
+    state_cashbook = fields.Function(fields.Selection(
+        string='State of Cashbook',
         readonly=True, states={'invisible': True}, selection=sel_state_book),
         'on_change_with_state_cashbook')
 
     @classmethod
     def __setup__(cls):
         super(TaxLine, cls).__setup__()
         cls._order.insert(0, ('tax.name', 'ASC'))
+        t = cls.__table__()
+        cls._sql_indexes.update({
+            Index(
+                t,
+                (t.line, Index.Equality())),
+            Index(
+                t,
+                (t.line, Index.Equality()),
+                (t.splitline, Index.Equality()),
+                where=t.splitline != None),
+            })
 
     def get_rec_name(self, name):
         """ short + name
         """
         return '%(taxname)s %(amount)s %(base)s' % {
             'taxname': getattr(self.tax, 'rec_name'),
-            'amount': Report.format_currency(self.amount or Decimal('0.0'),
+            'amount': Report.format_currency(
+                self.amount or Decimal('0.0'),
                 None, self.currency),
-            'base': Report.format_currency(self.base or Decimal('0.0'),
+            'base': Report.format_currency(
+                self.base or Decimal('0.0'),
                 None, self.currency),
             }
 
     @fields.depends('line', '_parent_line.state')
     def on_change_with_state(self, name=None):
         """ get state
         """
```

### Comparing `mds_cashbook_account-6.0.9/tax.xml` & `mds_cashbook_account-6.8.11/tax.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook_account-6.0.9/tests/test_category.py` & `mds_cashbook_account-6.8.11/tests/category.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 # -*- coding: utf-8 -*-
 # This file is part of the cashbook-module from m-ds for Tryton.
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
-from trytond.tests.test_tryton import ModuleTestCase, with_transaction
+from trytond.tests.test_tryton import with_transaction
 from trytond.pool import Pool
 from trytond.transaction import Transaction
-from trytond.exceptions import UserError
-from trytond.modules.cashbook.tests import CashbookTestCase
 from trytond.modules.account.tests import create_chart, get_fiscalyear
 from trytond.modules.company.tests import set_company
 from datetime import date
-from decimal import Decimal
 
 
-class CategoryTestCase(CashbookTestCase):
-    'Test cashbook categoy module'
-    module = 'cashbook_account'
-
+class CategoryTestCase(object):
+    """ test category
+    """
     def prep_config(self):
         """ disable account-name-view
         """
-        Configuration = Pool().get('cashbook.configuration')
-
         cfg1 = super(CategoryTestCase, self).prep_config()
         cfg1.cataccno = False
         cfg1.save()
         return cfg1
 
     def prep_accounting(self, company1):
         """ create account-plan, fiscalyear, etc.
@@ -34,17 +28,16 @@
         pool = Pool()
         FiscalYear = pool.get('account.fiscalyear')
         Sequence = pool.get('ir.sequence')
         AccountJournal = pool.get('account.journal')
 
         with set_company(company1):
             with Transaction().set_context({
-                'company': company1.id,
-                }):
-                chart1 = create_chart(company = company1, tax = True)
+                        'company': company1.id}):
+                create_chart(company=company1, tax=True)
 
                 fisc_year = get_fiscalyear(company1, today=date(2022, 5, 1))
                 fisc_year.save()
                 FiscalYear.create_period([fisc_year])
 
                 journal_sequence, = Sequence.search([
                         ('sequence_type.name', '=', "Account Journal"),
@@ -63,16 +56,15 @@
         pool = Pool()
         Account = pool.get('account.account')
         Category = pool.get('cashbook.category')
 
         company = self.prep_company()
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             account, = Account.create([{
                 'name': 'Account No 1',
                 'code': '0123',
                 }])
 
             cat1, = Category.create([{
                 'name': 'Test 1',
```

### Comparing `mds_cashbook_account-6.0.9/tests/test_line.py` & `mds_cashbook_account-6.8.11/tests/line.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # -*- coding: utf-8 -*-
 # This file is part of the cashbook-module from m-ds for Tryton.
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
-from trytond.tests.test_tryton import ModuleTestCase, with_transaction
+from trytond.tests.test_tryton import with_transaction
 from trytond.pool import Pool
 from trytond.transaction import Transaction
 from trytond.exceptions import UserError
 from datetime import date
 from decimal import Decimal
 
 
-class LineTestCase(ModuleTestCase):
-    'Test cashbook line module'
-    module = 'cashbook_account'
-
+class LineTestCase(object):
+    """ test lines
+    """
     def prep_line_taxes(self):
         """ prepare taxes
         """
         pool = Pool()
         AccountType = pool.get('account.account.type')
         Account = pool.get('account.account')
         Tax = pool.get('account.tax')
@@ -101,24 +100,23 @@
         Book = pool.get('cashbook.book')
         Account = pool.get('account.account')
         Category = pool.get('cashbook.category')
         Configuration = pool.get('cashbook.configuration')
         Journal = pool.get('account.journal')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             self.prep_accounting(company)
             taxes = self.prep_line_taxes()
 
             accounts = Account.create([{
                 'name': 'Account No 1',
                 'code': '0123',
                 }, {
@@ -196,100 +194,116 @@
                             }])],
                     }, ])],
                 }])
             self.assertEqual(book.name, 'Book 1')
             self.assertEqual(book.state, 'open')
             self.assertEqual(len(book.lines), 4)
 
-            self.assertEqual(book.lines[0].rec_name, '05/01/2022|Rev|10.00 usd|No Taxes [Cat 1 [2234]]')
+            self.assertEqual(
+                book.lines[0].rec_name,
+                '05/01/2022|Rev|10.00 usd|No Taxes [Cat 1 [2234]]')
             self.assertEqual(len(book.lines[0].taxes), 0)
             self.assertEqual(book.lines[0].amount_net, None)
             self.assertEqual(book.lines[0].amount_tax0, None)
             self.assertEqual(book.lines[0].amount_tax1, None)
             self.assertEqual(book.lines[0].amount_tax2, None)
 
-            self.assertEqual(book.lines[1].rec_name, '05/02/2022|Rev|10.00 usd|Half Tax [Cat 1 [2234]]')
+            self.assertEqual(
+                book.lines[1].rec_name,
+                '05/02/2022|Rev|10.00 usd|Half Tax [Cat 1 [2234]]')
             self.assertEqual(len(book.lines[1].taxes), 1)
             self.assertEqual(book.lines[1].taxes[0].amount, Decimal('0.91'))
             self.assertEqual(book.lines[1].taxes[0].base, Decimal('9.09'))
             self.assertEqual(book.lines[1].taxes[0].tax.rec_name, 'Tax Half')
             self.assertEqual(book.lines[1].taxes[0].splitline, None)
             self.assertEqual(book.lines[1].amount_net, Decimal('9.09'))
             self.assertEqual(book.lines[1].amount_tax0, None)
             self.assertEqual(book.lines[1].amount_tax1, Decimal('0.91'))
             self.assertEqual(book.lines[1].amount_tax2, None)
 
-            self.assertEqual(book.lines[2].rec_name, '05/03/2022|Rev|10.00 usd|two taxes [Cat 1 [2234]]')
+            self.assertEqual(
+                book.lines[2].rec_name,
+                '05/03/2022|Rev|10.00 usd|two taxes [Cat 1 [2234]]')
             self.assertEqual(len(book.lines[2].taxes), 3)
             self.assertEqual(book.lines[2].taxes[0].amount, Decimal('0.62'))
             self.assertEqual(book.lines[2].taxes[0].base, Decimal('7.82'))
             self.assertEqual(book.lines[2].taxes[0].tax.rec_name, 'Part 1')
             self.assertEqual(book.lines[2].taxes[0].splitline, None)
-            self.assertEqual(book.lines[2].taxes[0].rec_name, 'Part 1 usd0.62 usd7.82')
+            self.assertEqual(
+                book.lines[2].taxes[0].rec_name,
+                'Part 1 usd0.62 usd7.82')
 
             self.assertEqual(book.lines[2].taxes[1].amount, Decimal('0.78'))
             self.assertEqual(book.lines[2].taxes[1].base, Decimal('7.82'))
             self.assertEqual(book.lines[2].taxes[1].tax.rec_name, 'Part 2')
             self.assertEqual(book.lines[2].taxes[1].splitline, None)
-            self.assertEqual(book.lines[2].taxes[1].rec_name, 'Part 2 usd0.78 usd7.82')
+            self.assertEqual(
+                book.lines[2].taxes[1].rec_name,
+                'Part 2 usd0.78 usd7.82')
 
             self.assertEqual(book.lines[2].taxes[2].amount, Decimal('0.78'))
             self.assertEqual(book.lines[2].taxes[2].base, Decimal('7.82'))
             self.assertEqual(book.lines[2].taxes[2].tax.rec_name, 'Tax Half')
             self.assertEqual(book.lines[2].taxes[2].splitline, None)
-            self.assertEqual(book.lines[2].taxes[2].rec_name, 'Tax Half usd0.78 usd7.82')
+            self.assertEqual(
+                book.lines[2].taxes[2].rec_name,
+                'Tax Half usd0.78 usd7.82')
 
             self.assertEqual(book.lines[2].amount, Decimal('10.0'))
             self.assertEqual(book.lines[2].amount_net, Decimal('7.82'))
             self.assertEqual(book.lines[2].amount_tax0, Decimal('1.40'))
             self.assertEqual(book.lines[2].amount_tax1, Decimal('0.78'))
             self.assertEqual(book.lines[2].amount_tax2, None)
 
-            self.assertEqual(book.lines[3].rec_name, '05/04/2022|Rev/Sp|10.00 usd|Split line - one tax [-]')
+            self.assertEqual(
+                book.lines[3].rec_name,
+                '05/04/2022|Rev/Sp|10.00 usd|Split line - one tax [-]')
             self.assertEqual(len(book.lines[3].taxes), 1)
             self.assertEqual(book.lines[3].taxes[0].amount, Decimal('0.91'))
             self.assertEqual(book.lines[3].taxes[0].base, Decimal('9.09'))
             self.assertEqual(book.lines[3].taxes[0].tax.rec_name, 'Tax Half')
-            self.assertEqual(book.lines[3].taxes[0].splitline.id, book.lines[3].splitlines[0].id)
+            self.assertEqual(
+                book.lines[3].taxes[0].splitline.id,
+                book.lines[3].splitlines[0].id)
             self.assertEqual(book.lines[3].amount, Decimal('10.0'))
             self.assertEqual(book.lines[3].amount_net, None)
             self.assertEqual(book.lines[3].amount_tax0, None)
             self.assertEqual(book.lines[3].amount_tax1, None)
             self.assertEqual(book.lines[3].amount_tax2, None)
             self.assertEqual(len(book.lines[3].splitlines), 1)
-            self.assertEqual(book.lines[3].splitlines[0].amount_net, Decimal('9.09'))
+            self.assertEqual(
+                book.lines[3].splitlines[0].amount_net, Decimal('9.09'))
             self.assertEqual(book.lines[3].splitlines[0].amount_tax0, None)
-            self.assertEqual(book.lines[3].splitlines[0].amount_tax1, Decimal('0.91'))
+            self.assertEqual(
+                book.lines[3].splitlines[0].amount_tax1, Decimal('0.91'))
             self.assertEqual(book.lines[3].splitlines[0].amount_tax2, None)
 
     @with_transaction()
     def test_line_check_ena_taxes(self):
         """ create cashbook + line, check enable of fields
             at line by configured taxes on category
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
-        Line = pool.get('cashbook.line')
         Configuration = pool.get('cashbook.configuration')
         Category = pool.get('cashbook.category')
         Account = pool.get('account.account')
         Journal = pool.get('account.journal')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
         self.prep_accounting(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             taxes = self.prep_line_taxes()
 
             accounts = Account.create([{
                 'name': 'Account No 1',
                 'code': '0123',
                 }, {
                 'name': 'Book',
@@ -361,28 +375,26 @@
     @with_transaction()
     def test_line_check_valiate_line(self):
         """ create cashbook + line, check validation of line
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
         Category = pool.get('cashbook.category')
         Journal = pool.get('account.journal')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
-        cfg1 = self.prep_config()
+        self.prep_config()
         self.prep_accounting(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             categories = Category.create([{
                 'company': company.id,
                 'name': 'Cat 1',
                 'cattype': 'in',
                 }])
 
             self.assertEqual(categories[0].rec_name, 'Cat 1')
@@ -404,16 +416,19 @@
                         'party': party.id,
                     }])],
                 }])
             self.assertEqual(book.name, 'Book 1')
             self.assertEqual(book.state, 'open')
             self.assertEqual(len(book.lines), 1)
 
-            self.assertRaisesRegex(UserError,
-                'A value is required for field "Split booking lines" in "Cashbook Line".',
+            self.assertRaisesRegex(
+                UserError,
+                'A value is required for field ' +
+                '"Split booking lines" in in ' +
+                '"05/01/2022|Rev/Sp|10.00 usd|Text 1 [-]" of "Cashbook Line".',
                 Line.write,
                 *[
                     [book.lines[0]],
                     {
                         'ena_tax1': True,
                         'bookingtype': 'spin',
                     },
@@ -421,30 +436,28 @@
 
     @with_transaction()
     def test_line_check_category_view_account(self):
         """ create cashbook + line, check 'category_view'
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
-        Line = pool.get('cashbook.line')
         Configuration = pool.get('cashbook.configuration')
         Category = pool.get('cashbook.category')
         Account = pool.get('account.account')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             accounts = Account.create([{
                 'name': 'Account No 1',
                 'code': '0123',
                 }, {
                 'name': 'Account No 2',
                 'code': '2345',
                 }])
@@ -461,15 +474,16 @@
                     'name': 'Level2',
                     'cattype': 'in',
                     'account': accounts[1].id,
                     }])],
                 }])
             self.assertEqual(category2.rec_name, 'Level1 [0123]')
             self.assertEqual(len(category2.childs), 1)
-            self.assertEqual(category2.childs[0].rec_name, 'Level1/Level2 [2345]')
+            self.assertEqual(
+                category2.childs[0].rec_name, 'Level1/Level2 [2345]')
 
             cfg1 = Configuration()
             cfg1.save()
 
             book, = Book.create([{
                 'name': 'Book 1',
                 'btype': types.id,
@@ -496,22 +510,28 @@
             self.assertEqual(book.name, 'Book 1')
             self.assertEqual(book.state, 'open')
             self.assertEqual(len(book.lines), 2)
 
             self.assertEqual(cfg1.catnamelong, True)
 
             self.assertEqual(book.lines[0].category.rec_name, 'Level1 [0123]')
-            self.assertEqual(book.lines[1].category.rec_name, 'Level1/Level2 [2345]')
+            self.assertEqual(
+                book.lines[1].category.rec_name,
+                'Level1/Level2 [2345]')
             self.assertEqual(book.lines[0].category_view, 'Level1 [0123]')
-            self.assertEqual(book.lines[1].category_view, 'Level1/Level2 [2345]')
+            self.assertEqual(
+                book.lines[1].category_view,
+                'Level1/Level2 [2345]')
 
             cfg1.catnamelong = False
             cfg1.save()
             self.assertEqual(book.lines[0].category.rec_name, 'Level1 [0123]')
-            self.assertEqual(book.lines[1].category.rec_name, 'Level1/Level2 [2345]')
+            self.assertEqual(
+                book.lines[1].category.rec_name,
+                'Level1/Level2 [2345]')
             self.assertEqual(book.lines[0].category_view, 'Level1 [0123]')
             self.assertEqual(book.lines[1].category_view, 'Level2 [2345]')
 
             cfg1.cataccno = False
             cfg1.catnamelong = True
             cfg1.save()
 
@@ -530,28 +550,26 @@
     @with_transaction()
     def test_line_check_get_move_amounts(self):
         """ check credit/debit/2ndcurrency
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
         Journal = pool.get('account.journal')
 
         types = self.prep_type()
         company = self.prep_company()
         party = self.prep_party()
-        cfg1 = self.prep_config()
+        self.prep_config()
         self.prep_accounting(company)
         category = self.prep_category(cattype='in')
         (usd, euro) = self.prep_2nd_currency(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             books = Book.create([{
                 'name': 'Book EUR',
                 'btype': types.id,
                 'company': company.id,
                 'currency': euro.id,
                 'number_sequ': self.prep_sequence().id,
                 'start_date': date(2022, 5, 1),
@@ -631,34 +649,32 @@
     def test_line_check_wf_in_booking_noparty(self):
         """ create cashbook + line, check booking in-type,
             company-currency
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
         Category = pool.get('cashbook.category')
         Account = pool.get('account.account')
         AccountType = pool.get('account.account.type')
         Journal = pool.get('account.journal')
         Move = pool.get('account.move')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         self.prep_accounting(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             acc_type, = AccountType.search([('name', '=', 'Cash')])
 
             accounts = Account.create([{
                 'name': 'Account Book',
                 'code': '0123',
                 'type': acc_type.id,
                 }, {
@@ -698,34 +714,40 @@
                         'amount': Decimal('10.0'),
                         'party': party.id,
                     }])],
                 }])
             self.assertEqual(book.rec_name, 'Book 1 | 10.00 usd | Open')
             self.assertEqual(book.account.rec_name, '0123 - Account Book')
             self.assertEqual(len(book.lines), 1)
-            self.assertEqual(book.lines[0].rec_name,
+            self.assertEqual(
+                book.lines[0].rec_name,
                 '05/05/2022|Rev|10.00 usd|sell something [In-Category [2345]]')
             self.assertEqual(len(book.lines[0].moves), 0)
-            self.assertEqual(book.lines[0].category.rec_name, 'In-Category [2345]')
+            self.assertEqual(
+                book.lines[0].category.rec_name,
+                'In-Category [2345]')
 
             self.assertEqual(Move.search_count([]), 0)
             Line.wfcheck([book.lines[0]])
 
             moves = Move.search([])
             self.assertEqual(len(moves), 1)
             self.assertEqual(len(moves[0].lines), 2)
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(moves[0].state, 'draft')
             self.assertEqual(moves[0].date, date(2022, 5, 5))
             self.assertEqual(moves[0].description, 'sell something')
             self.assertEqual(moves[0].period.rec_name, '2022-05')
             self.assertEqual(moves[0].journal.rec_name, 'Cashbook')
-            self.assertEqual(moves[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].origin.rec_name,
                 '05/05/2022|Rev|10.00 usd|sell something [In-Category [2345]]')
-            self.assertEqual(moves[0].lines[0].rec_name, '(2345 - Account Category)')
+            self.assertEqual(
+                moves[0].lines[0].rec_name,
+                '(2345 - Account Category)')
             self.assertEqual(moves[0].lines[0].credit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[0].debit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[0].amount_second_currency, None)
             self.assertEqual(moves[0].lines[1].rec_name, '0123 - Account Book')
             self.assertEqual(moves[0].lines[1].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[1].debit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[1].amount_second_currency, None)
@@ -748,33 +770,31 @@
     def test_line_check_wf_in_booking_noparty_tax(self):
         """ create cashbook + line, check booking in-type,
             company-currency, net + tax
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
         Category = pool.get('cashbook.category')
         Account = pool.get('account.account')
         AccountType = pool.get('account.account.type')
         Journal = pool.get('account.journal')
         Move = pool.get('account.move')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         self.prep_accounting(company)
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             taxes = self.prep_line_taxes()
             acc_type, = AccountType.search([('name', '=', 'Cash')])
 
             accounts = Account.create([{
                 'name': 'Account Book',
                 'code': '0123',
                 'type': acc_type.id,
@@ -821,29 +841,36 @@
                         'amount': Decimal('10.0'),
                         'party': party.id,
                     }])],
                 }])
             self.assertEqual(book.rec_name, 'Book 1 | 10.00 usd | Open')
             self.assertEqual(book.account.rec_name, '0123 - Account Book')
             self.assertEqual(len(book.lines), 1)
-            self.assertEqual(book.lines[0].rec_name,
+            self.assertEqual(
+                book.lines[0].rec_name,
                 '05/05/2022|Rev|10.00 usd|sell something [In-Category [2345]]')
             self.assertEqual(len(book.lines[0].moves), 0)
-            self.assertEqual(book.lines[0].category.rec_name, 'In-Category [2345]')
+            self.assertEqual(
+                book.lines[0].category.rec_name,
+                'In-Category [2345]')
             self.assertEqual(len(book.lines[0].taxes), 0)
 
             # add tax
             book.lines[0].ena_tax1 = True
             book.lines[0].on_change_ena_tax1()
             book.lines[0].save()
             self.assertEqual(len(book.lines[0].taxes), 1)
-            self.assertEqual(book.lines[0].taxes[0].rec_name, 'Tax Half usd0.91 usd9.09')
+            self.assertEqual(
+                book.lines[0].taxes[0].rec_name,
+                'Tax Half usd0.91 usd9.09')
 
             # check
-            self.assertEqual(book.lines[0].category.rec_name, 'In-Category [2345]')
+            self.assertEqual(
+                book.lines[0].category.rec_name,
+                'In-Category [2345]')
             self.assertEqual(book.lines[0].amount, Decimal('10.0'))
             self.assertEqual(book.lines[0].ena_tax1, True)
             self.assertEqual(book.lines[0].amount_tax1, Decimal('0.91'))
             self.assertEqual(book.lines[0].amount_net, Decimal('9.09'))
 
             self.assertEqual(Move.search_count([]), 0)
             Line.wfcheck([book.lines[0]])
@@ -853,33 +880,39 @@
             self.assertEqual(len(moves[0].lines), 3)
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(moves[0].state, 'draft')
             self.assertEqual(moves[0].date, date(2022, 5, 5))
             self.assertEqual(moves[0].description, 'sell something')
             self.assertEqual(moves[0].period.rec_name, '2022-05')
             self.assertEqual(moves[0].journal.rec_name, 'Cashbook')
-            self.assertEqual(moves[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].origin.rec_name,
                 '05/05/2022|Rev|10.00 usd|sell something [In-Category [2345]]')
             self.assertEqual(moves[0].lines[0].rec_name, '(2234 - Tax Half)')
             self.assertEqual(moves[0].lines[0].credit, Decimal('0.91'))
             self.assertEqual(moves[0].lines[0].debit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[0].amount_second_currency, None)
             self.assertEqual(len(moves[0].lines[0].tax_lines), 1)
-            self.assertEqual(moves[0].lines[0].tax_lines[0].amount, Decimal('0.91'))
+            self.assertEqual(
+                moves[0].lines[0].tax_lines[0].amount, Decimal('0.91'))
             self.assertEqual(moves[0].lines[0].tax_lines[0].type, 'tax')
-            self.assertEqual(moves[0].lines[0].tax_lines[0].tax.rec_name, 'Tax Half')
+            self.assertEqual(
+                moves[0].lines[0].tax_lines[0].tax.rec_name, 'Tax Half')
 
-            self.assertEqual(moves[0].lines[1].rec_name, '(2345 - Account Category)')
+            self.assertEqual(
+                moves[0].lines[1].rec_name, '(2345 - Account Category)')
             self.assertEqual(moves[0].lines[1].credit, Decimal('9.09'))
             self.assertEqual(moves[0].lines[1].debit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[1].amount_second_currency, None)
             self.assertEqual(len(moves[0].lines[1].tax_lines), 1)
-            self.assertEqual(moves[0].lines[1].tax_lines[0].amount, Decimal('9.09'))
+            self.assertEqual(
+                moves[0].lines[1].tax_lines[0].amount, Decimal('9.09'))
             self.assertEqual(moves[0].lines[1].tax_lines[0].type, 'base')
-            self.assertEqual(moves[0].lines[1].tax_lines[0].tax.rec_name, 'Tax Half')
+            self.assertEqual(
+                moves[0].lines[1].tax_lines[0].tax.rec_name, 'Tax Half')
 
             self.assertEqual(moves[0].lines[2].rec_name, '0123 - Account Book')
             self.assertEqual(moves[0].lines[2].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[2].debit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[2].amount_second_currency, None)
             self.assertEqual(len(moves[0].lines[2].tax_lines), 0)
 
@@ -901,34 +934,32 @@
     def test_line_check_wf_in_split_booking_noparty(self):
         """ create cashbook + line, check booking in-type,
             company-currency
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
         Category = pool.get('cashbook.category')
         Account = pool.get('account.account')
         AccountType = pool.get('account.account.type')
         Journal = pool.get('account.journal')
         Move = pool.get('account.move')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         self.prep_accounting(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             acc_type, = AccountType.search([('name', '=', 'Cash')])
 
             accounts = Account.create([{
                 'name': 'Account Book',
                 'code': '0123',
                 'type': acc_type.id,
                 }, {
@@ -976,54 +1007,62 @@
                             'description': 'line 2',
                             }])],
                     }])],
                 }])
             self.assertEqual(book.rec_name, 'Book 1 | 10.00 usd | Open')
             self.assertEqual(book.account.rec_name, '0123 - Account Book')
             self.assertEqual(len(book.lines), 1)
-            self.assertEqual(book.lines[0].rec_name,
+            self.assertEqual(
+                book.lines[0].rec_name,
                 '05/05/2022|Rev/Sp|10.00 usd|sell something [-]')
             self.assertEqual(len(book.lines[0].moves), 0)
             self.assertEqual(book.lines[0].category, None)
             self.assertEqual(len(book.lines[0].splitlines), 2)
-            self.assertEqual(book.lines[0].splitlines[0].rec_name, \
+            self.assertEqual(
+                book.lines[0].splitlines[0].rec_name,
                 'Rev/Sp|5.00 usd|line 1 [In-Category [2345]]')
-            self.assertEqual(book.lines[0].splitlines[1].rec_name, \
+            self.assertEqual(
+                book.lines[0].splitlines[1].rec_name,
                 'Rev/Sp|5.00 usd|line 2 [In-Category [2345]]')
 
             self.assertEqual(Move.search_count([]), 0)
             Line.wfcheck([book.lines[0]])
 
             moves = Move.search([])
             self.assertEqual(len(moves), 1)
             self.assertEqual(len(moves[0].lines), 3)
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(moves[0].state, 'draft')
             self.assertEqual(moves[0].date, date(2022, 5, 5))
             self.assertEqual(moves[0].description, 'sell something')
             self.assertEqual(moves[0].period.rec_name, '2022-05')
             self.assertEqual(moves[0].journal.rec_name, 'Cashbook')
-            self.assertEqual(moves[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].origin.rec_name,
                 '05/05/2022|Rev/Sp|10.00 usd|sell something [-]')
-            self.assertEqual(moves[0].lines[0].rec_name, '(2345 - Account Category)')
+            self.assertEqual(
+                moves[0].lines[0].rec_name, '(2345 - Account Category)')
             self.assertEqual(moves[0].lines[0].credit, Decimal('5.0'))
             self.assertEqual(moves[0].lines[0].debit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[0].description, 'line 1')
             self.assertEqual(moves[0].lines[0].amount_second_currency, None)
             self.assertEqual(moves[0].lines[0].party, None)
-            self.assertEqual(moves[0].lines[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[0].origin.rec_name,
                 'Rev/Sp|5.00 usd|line 1 [In-Category [2345]]')
 
-            self.assertEqual(moves[0].lines[1].rec_name, '(2345 - Account Category)')
+            self.assertEqual(
+                moves[0].lines[1].rec_name, '(2345 - Account Category)')
             self.assertEqual(moves[0].lines[1].credit, Decimal('5.0'))
             self.assertEqual(moves[0].lines[1].debit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[1].description, 'line 2')
             self.assertEqual(moves[0].lines[1].amount_second_currency, None)
             self.assertEqual(moves[0].lines[1].party, None)
-            self.assertEqual(moves[0].lines[1].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[1].origin.rec_name,
                 'Rev/Sp|5.00 usd|line 2 [In-Category [2345]]')
 
             self.assertEqual(moves[0].lines[2].rec_name, '0123 - Account Book')
             self.assertEqual(moves[0].lines[2].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[2].debit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[2].amount_second_currency, None)
             self.assertEqual(moves[0].lines[2].party, None)
@@ -1047,34 +1086,32 @@
     def test_line_check_wf_in_split_booking_noparty_transfer(self):
         """ create cashbook + line, check booking in-type,
             company-currency, transfer with fee
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
         Category = pool.get('cashbook.category')
         Account = pool.get('account.account')
         AccountType = pool.get('account.account.type')
         Journal = pool.get('account.journal')
         Move = pool.get('account.move')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         self.prep_accounting(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             acc_type, = AccountType.search([('name', '=', 'Cash')])
 
             accounts = Account.create([{
                 'name': 'Account Book 1',
                 'code': '0123',
                 'type': acc_type.id,
                 }, {
@@ -1151,79 +1188,94 @@
                                 'description': 'transfer amount',
                             }])],
                         }])],
                 }])
             self.assertEqual(len(books[0].lines), 1)
             self.assertEqual(len(books[1].lines), 0)
 
-            self.assertEqual(books[0].lines[0].rec_name,
+            self.assertEqual(
+                books[0].lines[0].rec_name,
                 '05/05/2022|Rev/Sp|30.00 usd|transfer with fee [-]')
             self.assertEqual(len(books[0].lines[0].moves), 0)
             self.assertEqual(books[0].lines[0].category, None)
             self.assertEqual(len(books[0].lines[0].splitlines), 2)
-            self.assertEqual(books[0].lines[0].splitlines[0].rec_name, \
+            self.assertEqual(
+                books[0].lines[0].splitlines[0].rec_name,
                 'Rev/Sp|5.00 usd|fee for transfer [In-Category [2345]]')
-            self.assertEqual(books[0].lines[0].splitlines[1].rec_name, \
+            self.assertEqual(
+                books[0].lines[0].splitlines[1].rec_name,
                 'Rev/Sp|25.00 usd|transfer amount [Book 2 | 0.00 usd | Open]')
 
             self.assertEqual(Move.search_count([]), 0)
             Line.wfcheck([books[0].lines[0]])
 
             # check book 1
             self.assertEqual(len(books[0].lines), 1)
-            self.assertEqual(books[0].lines[0].rec_name,
+            self.assertEqual(
+                books[0].lines[0].rec_name,
                 '05/05/2022|Rev/Sp|30.00 usd|transfer with fee [-]')
             self.assertEqual(len(books[0].lines[0].moves), 1)
             self.assertEqual(books[0].lines[0].category, None)
             self.assertEqual(len(books[0].lines[0].splitlines), 2)
-            self.assertEqual(books[0].lines[0].splitlines[0].rec_name, \
+            self.assertEqual(
+                books[0].lines[0].splitlines[0].rec_name,
                 'Rev/Sp|5.00 usd|fee for transfer [In-Category [2345]]')
-            self.assertEqual(books[0].lines[0].splitlines[1].rec_name, \
+            self.assertEqual(
+                books[0].lines[0].splitlines[1].rec_name,
                 'Rev/Sp|25.00 usd|transfer amount [Book 2 | -25.00 usd | Open]')
 
             # check book 2
             self.assertEqual(len(books[1].lines), 1)
-            self.assertEqual(books[1].lines[0].rec_name,
-                '05/05/2022|to|-25.00 usd|transfer amount [Book 1 | 30.00 usd | Open]')
+            self.assertEqual(
+                books[1].lines[0].rec_name,
+                '05/05/2022|to|-25.00 usd|transfer amount ' +
+                '[Book 1 | 30.00 usd | Open]')
             self.assertEqual(len(books[1].lines[0].moves), 0)
-            self.assertEqual(books[1].lines[0].reference.rec_name,
+            self.assertEqual(
+                books[1].lines[0].reference.rec_name,
                 '05/05/2022|Rev/Sp|30.00 usd|transfer with fee [-]')
 
             moves = Move.search([])
             self.assertEqual(len(moves), 1)
             self.assertEqual(len(moves[0].lines), 3)
             self.assertEqual(len(books[0].lines[0].moves), 1)
             self.assertEqual(moves[0].state, 'draft')
             self.assertEqual(moves[0].date, date(2022, 5, 5))
             self.assertEqual(moves[0].description, 'transfer with fee')
             self.assertEqual(moves[0].period.rec_name, '2022-05')
             self.assertEqual(moves[0].journal.rec_name, 'Cashbook')
-            self.assertEqual(moves[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].origin.rec_name,
                 '05/05/2022|Rev/Sp|30.00 usd|transfer with fee [-]')
-            self.assertEqual(moves[0].lines[0].rec_name, '(2345 - Account Category)')
+            self.assertEqual(
+                moves[0].lines[0].rec_name, '(2345 - Account Category)')
             self.assertEqual(moves[0].lines[0].credit, Decimal('5.0'))
             self.assertEqual(moves[0].lines[0].debit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[0].description, 'fee for transfer')
             self.assertEqual(moves[0].lines[0].amount_second_currency, None)
             self.assertEqual(moves[0].lines[0].party, None)
             self.assertEqual(len(moves[0].lines[0].tax_lines), 0)
-            self.assertEqual(moves[0].lines[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[0].origin.rec_name,
                 'Rev/Sp|5.00 usd|fee for transfer [In-Category [2345]]')
 
-            self.assertEqual(moves[0].lines[1].rec_name, '(3456 - Account Book 2)')
+            self.assertEqual(
+                moves[0].lines[1].rec_name, '(3456 - Account Book 2)')
             self.assertEqual(moves[0].lines[1].credit, Decimal('25.0'))
             self.assertEqual(moves[0].lines[1].debit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[1].description, 'transfer amount')
             self.assertEqual(moves[0].lines[1].amount_second_currency, None)
             self.assertEqual(moves[0].lines[1].party, None)
             self.assertEqual(len(moves[0].lines[1].tax_lines), 0)
-            self.assertEqual(moves[0].lines[1].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[1].origin.rec_name,
                 'Rev/Sp|25.00 usd|transfer amount [Book 2 | -25.00 usd | Open]')
 
-            self.assertEqual(moves[0].lines[2].rec_name, '0123 - Account Book 1')
+            self.assertEqual(
+                moves[0].lines[2].rec_name, '0123 - Account Book 1')
             self.assertEqual(moves[0].lines[2].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[2].debit, Decimal('30.0'))
             self.assertEqual(moves[0].lines[2].amount_second_currency, None)
             self.assertEqual(moves[0].lines[2].party, None)
             self.assertEqual(len(moves[0].lines[2].tax_lines), 0)
             self.assertEqual(moves[0].lines[2].origin, None)
 
@@ -1245,35 +1297,33 @@
     def test_line_check_wf_in_booking_withparty(self):
         """ create cashbook + line, check booking in-type,
             company-currency, include party-accounts
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
         Category = pool.get('cashbook.category')
         Account = pool.get('account.account')
         AccountType = pool.get('account.account.type')
         Journal = pool.get('account.journal')
         Move = pool.get('account.move')
         Reconciliation = pool.get('account.move.reconciliation')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         self.prep_accounting(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             acc_type, = AccountType.search([('name', '=', 'Cash')])
 
             accounts = Account.create([{
                 'name': 'Account Book',
                 'code': '0123',
                 'type': acc_type.id,
                 }, {
@@ -1313,42 +1363,46 @@
                         'amount': Decimal('10.0'),
                         'party': party.id,
                     }])],
                 }])
             self.assertEqual(book.rec_name, 'Book 1 | 10.00 usd | Open')
             self.assertEqual(book.account.rec_name, '0123 - Account Book')
             self.assertEqual(len(book.lines), 1)
-            self.assertEqual(book.lines[0].rec_name,
+            self.assertEqual(
+                book.lines[0].rec_name,
                 '05/05/2022|Rev|10.00 usd|sell something [In-Category [2345]]')
             self.assertEqual(len(book.lines[0].moves), 0)
-            self.assertEqual(book.lines[0].category.rec_name, 'In-Category [2345]')
+            self.assertEqual(
+                book.lines[0].category.rec_name, 'In-Category [2345]')
 
             self.assertEqual(Move.search_count([]), 0)
             Line.wfcheck([book.lines[0]])
 
             moves = Move.search([])
             self.assertEqual(len(moves), 1)
             self.assertEqual(len(moves[0].lines), 4)
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(moves[0].state, 'draft')
             self.assertEqual(moves[0].date, date(2022, 5, 5))
             self.assertEqual(moves[0].description, 'sell something')
             self.assertEqual(moves[0].period.rec_name, '2022-05')
             self.assertEqual(moves[0].journal.rec_name, 'Cashbook')
-            self.assertEqual(moves[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].origin.rec_name,
                 '05/05/2022|Rev|10.00 usd|sell something [In-Category [2345]]')
             self.assertEqual(moves[0].lines[0].rec_name, 'Main Receivable')
             self.assertEqual(moves[0].lines[0].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[0].debit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[0].amount_second_currency, None)
             self.assertEqual(moves[0].lines[0].party.rec_name, 'Party')
             self.assertEqual(len(moves[0].lines[0].tax_lines), 0)
             self.assertEqual(moves[0].lines[0].origin, None)
 
-            self.assertEqual(moves[0].lines[1].rec_name, '(2345 - Account Category)')
+            self.assertEqual(
+                moves[0].lines[1].rec_name, '(2345 - Account Category)')
             self.assertEqual(moves[0].lines[1].credit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[1].debit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[1].amount_second_currency, None)
             self.assertEqual(moves[0].lines[1].party, None)
             self.assertEqual(len(moves[0].lines[1].tax_lines), 0)
             self.assertEqual(moves[0].lines[1].origin, None)
 
@@ -1380,15 +1434,16 @@
             # post move
             self.assertEqual(Reconciliation.search_count([]), 0)
             Line.wfdone([book.lines[0]])
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(book.lines[0].moves[0].state, 'posted')
 
             rec_lines = Reconciliation.search([])
-            rec_move_ids = [x.id for x in book.lines[0].moves[0].lines if x.party]
+            rec_move_ids = [
+                x.id for x in book.lines[0].moves[0].lines if x.party]
             self.assertEqual(len(rec_move_ids), 2)
 
             self.assertEqual(len(rec_lines), 1)
             self.assertEqual(len(rec_lines[0].lines), 2)
 
             self.assertTrue(rec_lines[0].lines[0].id in rec_move_ids)
             self.assertTrue(rec_lines[0].lines[1].id in rec_move_ids)
@@ -1397,35 +1452,33 @@
     def test_line_check_wf_in_booking_withparty_tax(self):
         """ create cashbook + line, check booking in-type,
             company-currency, include party-accounts
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
         Category = pool.get('cashbook.category')
         Account = pool.get('account.account')
         AccountType = pool.get('account.account.type')
         Journal = pool.get('account.journal')
         Move = pool.get('account.move')
         Reconciliation = pool.get('account.move.reconciliation')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         self.prep_accounting(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             taxes = self.prep_line_taxes()
             acc_type, = AccountType.search([('name', '=', 'Cash')])
 
             accounts = Account.create([{
                 'name': 'Account Book',
                 'code': '0123',
                 'type': acc_type.id,
@@ -1473,20 +1526,23 @@
                         'party': party.id,
                         'ena_tax1': True,
                     }])],
                 }])
             self.assertEqual(book.rec_name, 'Book 1 | 10.00 usd | Open')
             self.assertEqual(book.account.rec_name, '0123 - Account Book')
             self.assertEqual(len(book.lines), 1)
-            self.assertEqual(book.lines[0].rec_name,
+            self.assertEqual(
+                book.lines[0].rec_name,
                 '05/05/2022|Rev|10.00 usd|sell something [In-Category [2345]]')
             self.assertEqual(len(book.lines[0].moves), 0)
-            self.assertEqual(book.lines[0].category.rec_name, 'In-Category [2345]')
+            self.assertEqual(
+                book.lines[0].category.rec_name, 'In-Category [2345]')
             self.assertEqual(len(book.lines[0].taxes), 1)
-            self.assertEqual(book.lines[0].taxes[0].rec_name, 'Tax Half usd0.91 usd9.09')
+            self.assertEqual(
+                book.lines[0].taxes[0].rec_name, 'Tax Half usd0.91 usd9.09')
             self.assertEqual(book.lines[0].amount, Decimal('10.0'))
             self.assertEqual(book.lines[0].ena_tax1, True)
             self.assertEqual(book.lines[0].amount_tax1, Decimal('0.91'))
             self.assertEqual(book.lines[0].amount_net, Decimal('9.09'))
 
             self.assertEqual(Move.search_count([]), 0)
             Line.wfcheck([book.lines[0]])
@@ -1496,15 +1552,16 @@
             self.assertEqual(len(moves[0].lines), 5)
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(moves[0].state, 'draft')
             self.assertEqual(moves[0].date, date(2022, 5, 5))
             self.assertEqual(moves[0].description, 'sell something')
             self.assertEqual(moves[0].period.rec_name, '2022-05')
             self.assertEqual(moves[0].journal.rec_name, 'Cashbook')
-            self.assertEqual(moves[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].origin.rec_name,
                 '05/05/2022|Rev|10.00 usd|sell something [In-Category [2345]]')
 
             self.assertEqual(moves[0].lines[0].rec_name, 'Main Receivable')
             self.assertEqual(moves[0].lines[0].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[0].debit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[0].amount_second_currency, None)
             self.assertEqual(moves[0].lines[0].party.rec_name, 'Party')
@@ -1514,28 +1571,33 @@
             self.assertEqual(moves[0].lines[1].rec_name, '(2234 - Tax Half)')
             self.assertEqual(moves[0].lines[1].credit, Decimal('0.91'))
             self.assertEqual(moves[0].lines[1].debit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[1].amount_second_currency, None)
             self.assertEqual(moves[0].lines[1].party, None)
             self.assertEqual(moves[0].lines[1].origin, None)
             self.assertEqual(len(moves[0].lines[1].tax_lines), 1)
-            self.assertEqual(moves[0].lines[1].tax_lines[0].amount, Decimal('0.91'))
+            self.assertEqual(
+                moves[0].lines[1].tax_lines[0].amount, Decimal('0.91'))
             self.assertEqual(moves[0].lines[1].tax_lines[0].type, 'tax')
-            self.assertEqual(moves[0].lines[1].tax_lines[0].tax.rec_name, 'Tax Half')
+            self.assertEqual(
+                moves[0].lines[1].tax_lines[0].tax.rec_name, 'Tax Half')
 
-            self.assertEqual(moves[0].lines[2].rec_name, '(2345 - Account Category)')
+            self.assertEqual(
+                moves[0].lines[2].rec_name, '(2345 - Account Category)')
             self.assertEqual(moves[0].lines[2].credit, Decimal('9.09'))
             self.assertEqual(moves[0].lines[2].debit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[2].amount_second_currency, None)
             self.assertEqual(moves[0].lines[2].party, None)
             self.assertEqual(moves[0].lines[2].origin, None)
             self.assertEqual(len(moves[0].lines[2].tax_lines), 1)
-            self.assertEqual(moves[0].lines[2].tax_lines[0].amount, Decimal('9.09'))
+            self.assertEqual(
+                moves[0].lines[2].tax_lines[0].amount, Decimal('9.09'))
             self.assertEqual(moves[0].lines[2].tax_lines[0].type, 'base')
-            self.assertEqual(moves[0].lines[2].tax_lines[0].tax.rec_name, 'Tax Half')
+            self.assertEqual(
+                moves[0].lines[2].tax_lines[0].tax.rec_name, 'Tax Half')
 
             self.assertEqual(moves[0].lines[3].rec_name, '0123 - Account Book')
             self.assertEqual(moves[0].lines[3].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[3].debit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[3].amount_second_currency, None)
             self.assertEqual(moves[0].lines[3].party, None)
             self.assertEqual(len(moves[0].lines[3].tax_lines), 0)
@@ -1561,15 +1623,16 @@
             # post move
             self.assertEqual(Reconciliation.search_count([]), 0)
             Line.wfdone([book.lines[0]])
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(book.lines[0].moves[0].state, 'posted')
 
             rec_lines = Reconciliation.search([])
-            rec_move_ids = [x.id for x in book.lines[0].moves[0].lines if x.party]
+            rec_move_ids = [
+                x.id for x in book.lines[0].moves[0].lines if x.party]
             self.assertEqual(len(rec_move_ids), 2)
 
             self.assertEqual(len(rec_lines), 1)
             self.assertEqual(len(rec_lines[0].lines), 2)
 
             self.assertTrue(rec_lines[0].lines[0].id in rec_move_ids)
             self.assertTrue(rec_lines[0].lines[1].id in rec_move_ids)
@@ -1578,35 +1641,33 @@
     def test_line_check_wf_in_split_booking_withparty(self):
         """ create cashbook + line, check booking in-type,
             company-currency, include party-accounts
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
         Category = pool.get('cashbook.category')
         Account = pool.get('account.account')
         AccountType = pool.get('account.account.type')
         Journal = pool.get('account.journal')
         Move = pool.get('account.move')
         Reconciliation = pool.get('account.move.reconciliation')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         self.prep_accounting(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             acc_type, = AccountType.search([('name', '=', 'Cash')])
 
             accounts = Account.create([{
                 'name': 'Account Book',
                 'code': '0123',
                 'type': acc_type.id,
                 }, {
@@ -1654,65 +1715,74 @@
                             'description': 'line 2',
                             }])],
                     }])],
                 }])
             self.assertEqual(book.rec_name, 'Book 1 | 10.00 usd | Open')
             self.assertEqual(book.account.rec_name, '0123 - Account Book')
             self.assertEqual(len(book.lines), 1)
-            self.assertEqual(book.lines[0].rec_name,
+            self.assertEqual(
+                book.lines[0].rec_name,
                 '05/05/2022|Rev/Sp|10.00 usd|sell something [-]')
             self.assertEqual(len(book.lines[0].moves), 0)
             self.assertEqual(book.lines[0].category, None)
             self.assertEqual(len(book.lines[0].splitlines), 2)
-            self.assertEqual(book.lines[0].splitlines[0].rec_name, \
+            self.assertEqual(
+                book.lines[0].splitlines[0].rec_name,
                 'Rev/Sp|5.00 usd|line 1 [In-Category [2345]]')
-            self.assertEqual(book.lines[0].splitlines[1].rec_name, \
+            self.assertEqual(
+                book.lines[0].splitlines[1].rec_name,
                 'Rev/Sp|5.00 usd|line 2 [In-Category [2345]]')
 
             self.assertEqual(Move.search_count([]), 0)
             Line.wfcheck([book.lines[0]])
 
             moves = Move.search([])
             self.assertEqual(len(moves), 1)
             self.assertEqual(len(moves[0].lines), 5)
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(moves[0].state, 'draft')
             self.assertEqual(moves[0].date, date(2022, 5, 5))
             self.assertEqual(moves[0].description, 'sell something')
             self.assertEqual(moves[0].period.rec_name, '2022-05')
             self.assertEqual(moves[0].journal.rec_name, 'Cashbook')
-            self.assertEqual(moves[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].origin.rec_name,
                 '05/05/2022|Rev/Sp|10.00 usd|sell something [-]')
             self.assertEqual(moves[0].lines[0].rec_name, 'Main Receivable')
             self.assertEqual(moves[0].lines[0].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[0].debit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[0].amount_second_currency, None)
             self.assertEqual(moves[0].lines[0].party.rec_name, 'Party')
             self.assertEqual(len(moves[0].lines[0].tax_lines), 0)
-            self.assertEqual(moves[0].lines[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[0].origin.rec_name,
                 '05/05/2022|Rev/Sp|10.00 usd|sell something [-]')
 
-            self.assertEqual(moves[0].lines[1].rec_name, '(2345 - Account Category)')
+            self.assertEqual(
+                moves[0].lines[1].rec_name, '(2345 - Account Category)')
             self.assertEqual(moves[0].lines[1].credit, Decimal('5.0'))
             self.assertEqual(moves[0].lines[1].debit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[1].amount_second_currency, None)
             self.assertEqual(moves[0].lines[1].party, None)
             self.assertEqual(moves[0].lines[1].description, 'line 1')
             self.assertEqual(len(moves[0].lines[1].tax_lines), 0)
-            self.assertEqual(moves[0].lines[1].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[1].origin.rec_name,
                 'Rev/Sp|5.00 usd|line 1 [In-Category [2345]]')
 
-            self.assertEqual(moves[0].lines[2].rec_name, '(2345 - Account Category)')
+            self.assertEqual(
+                moves[0].lines[2].rec_name, '(2345 - Account Category)')
             self.assertEqual(moves[0].lines[2].credit, Decimal('5.0'))
             self.assertEqual(moves[0].lines[2].debit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[2].amount_second_currency, None)
             self.assertEqual(moves[0].lines[2].party, None)
             self.assertEqual(moves[0].lines[2].description, 'line 2')
             self.assertEqual(len(moves[0].lines[2].tax_lines), 0)
-            self.assertEqual(moves[0].lines[2].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[2].origin.rec_name,
                 'Rev/Sp|5.00 usd|line 2 [In-Category [2345]]')
 
             self.assertEqual(moves[0].lines[3].rec_name, '0123 - Account Book')
             self.assertEqual(moves[0].lines[3].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[3].debit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[3].amount_second_currency, None)
             self.assertEqual(moves[0].lines[3].party, None)
@@ -1721,15 +1791,16 @@
 
             self.assertEqual(moves[0].lines[4].rec_name, '(Main Receivable)')
             self.assertEqual(moves[0].lines[4].credit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[4].debit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[4].amount_second_currency, None)
             self.assertEqual(moves[0].lines[4].party.rec_name, 'Party')
             self.assertEqual(len(moves[0].lines[4].tax_lines), 0)
-            self.assertEqual(moves[0].lines[4].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[4].origin.rec_name,
                 '05/05/2022|Rev/Sp|10.00 usd|sell something [-]')
 
             # delete move
             Line.wfedit([book.lines[0]])
             self.assertEqual(len(book.lines[0].moves), 0)
 
             # create move again
@@ -1740,15 +1811,16 @@
             # post move
             self.assertEqual(Reconciliation.search_count([]), 0)
             Line.wfdone([book.lines[0]])
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(book.lines[0].moves[0].state, 'posted')
 
             rec_lines = Reconciliation.search([])
-            rec_move_ids = [x.id for x in book.lines[0].moves[0].lines if x.party]
+            rec_move_ids = [
+                x.id for x in book.lines[0].moves[0].lines if x.party]
             self.assertEqual(len(rec_move_ids), 2)
 
             self.assertEqual(len(rec_lines), 1)
             self.assertEqual(len(rec_lines[0].lines), 2)
 
             self.assertTrue(rec_lines[0].lines[0].id in rec_move_ids)
             self.assertTrue(rec_lines[0].lines[1].id in rec_move_ids)
@@ -1757,35 +1829,33 @@
     def test_line_check_wf_in_split_booking_withparty_tax(self):
         """ create cashbook + line, check booking in-type,
             company-currency, include party-accounts
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
         Category = pool.get('cashbook.category')
         Account = pool.get('account.account')
         AccountType = pool.get('account.account.type')
         Journal = pool.get('account.journal')
         Move = pool.get('account.move')
         Reconciliation = pool.get('account.move.reconciliation')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         self.prep_accounting(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             taxes = self.prep_line_taxes()
             acc_type, = AccountType.search([('name', '=', 'Cash')])
 
             accounts = Account.create([{
                 'name': 'Account Book',
                 'code': '0123',
                 'type': acc_type.id,
@@ -1842,110 +1912,131 @@
                             'ena_tax2': True,
                             }])],
                     }])],
                 }])
             self.assertEqual(book.rec_name, 'Book 1 | 10.00 usd | Open')
             self.assertEqual(book.account.rec_name, '0123 - Account Book')
             self.assertEqual(len(book.lines), 1)
-            self.assertEqual(book.lines[0].rec_name,
+            self.assertEqual(
+                book.lines[0].rec_name,
                 '05/05/2022|Rev/Sp|10.00 usd|sell something [-]')
             self.assertEqual(len(book.lines[0].moves), 0)
             self.assertEqual(book.lines[0].category, None)
             self.assertEqual(len(book.lines[0].splitlines), 2)
-            self.assertEqual(book.lines[0].splitlines[0].rec_name, \
+            self.assertEqual(
+                book.lines[0].splitlines[0].rec_name,
                 'Rev/Sp|5.00 usd|line 1 [In-Category [2345]]')
-            self.assertEqual(book.lines[0].splitlines[1].rec_name, \
+            self.assertEqual(
+                book.lines[0].splitlines[1].rec_name,
                 'Rev/Sp|5.00 usd|line 2 [In-Category [2345]]')
 
             self.assertEqual(len(book.lines[0].taxes), 2)
             self.assertEqual(book.lines[0].taxes[0].amount, Decimal('0.83'))
             self.assertEqual(book.lines[0].taxes[0].base, Decimal('4.17'))
             self.assertEqual(book.lines[0].taxes[0].tax.rec_name, 'Tax Full')
-            self.assertEqual(book.lines[0].taxes[0].splitline.rec_name,
+            self.assertEqual(
+                book.lines[0].taxes[0].splitline.rec_name,
                 'Rev/Sp|5.00 usd|line 2 [In-Category [2345]]')
             self.assertEqual(book.lines[0].taxes[1].amount, Decimal('0.46'))
             self.assertEqual(book.lines[0].taxes[1].base, Decimal('4.54'))
             self.assertEqual(book.lines[0].taxes[1].tax.rec_name, 'Tax Half')
-            self.assertEqual(book.lines[0].taxes[1].splitline.rec_name,
+            self.assertEqual(
+                book.lines[0].taxes[1].splitline.rec_name,
                 'Rev/Sp|5.00 usd|line 1 [In-Category [2345]]')
 
             self.assertEqual(Move.search_count([]), 0)
             Line.wfcheck([book.lines[0]])
 
             moves = Move.search([])
             self.assertEqual(len(moves), 1)
             self.assertEqual(len(moves[0].lines), 7)
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(moves[0].state, 'draft')
             self.assertEqual(moves[0].date, date(2022, 5, 5))
             self.assertEqual(moves[0].description, 'sell something')
             self.assertEqual(moves[0].period.rec_name, '2022-05')
             self.assertEqual(moves[0].journal.rec_name, 'Cashbook')
-            self.assertEqual(moves[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].origin.rec_name,
                 '05/05/2022|Rev/Sp|10.00 usd|sell something [-]')
 
             self.assertEqual(moves[0].lines[0].rec_name, 'Main Receivable')
             self.assertEqual(moves[0].lines[0].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[0].debit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[0].amount_second_currency, None)
             self.assertEqual(moves[0].lines[0].party.rec_name, 'Party')
             self.assertEqual(len(moves[0].lines[0].tax_lines), 0)
-            self.assertEqual(moves[0].lines[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[0].origin.rec_name,
                 '05/05/2022|Rev/Sp|10.00 usd|sell something [-]')
 
-            self.assertEqual(moves[0].lines[1].rec_name, '(2345 - Account Category)')
+            self.assertEqual(
+                moves[0].lines[1].rec_name, '(2345 - Account Category)')
             self.assertEqual(moves[0].lines[1].credit, Decimal('4.54'))
             self.assertEqual(moves[0].lines[1].debit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[1].amount_second_currency, None)
             self.assertEqual(moves[0].lines[1].party, None)
             self.assertEqual(moves[0].lines[1].description, 'line 1')
-            self.assertEqual(moves[0].lines[1].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[1].origin.rec_name,
                 'Rev/Sp|5.00 usd|line 1 [In-Category [2345]]')
-            self.assertEqual(moves[0].lines[1].tax_lines[0].amount, Decimal('4.54'))
+            self.assertEqual(
+                moves[0].lines[1].tax_lines[0].amount, Decimal('4.54'))
             self.assertEqual(moves[0].lines[1].tax_lines[0].type, 'base')
-            self.assertEqual(moves[0].lines[1].tax_lines[0].tax.rec_name, 'Tax Half')
+            self.assertEqual(
+                moves[0].lines[1].tax_lines[0].tax.rec_name, 'Tax Half')
 
             self.assertEqual(moves[0].lines[2].rec_name, '(2234 - Tax Half)')
             self.assertEqual(moves[0].lines[2].credit, Decimal('0.46'))
             self.assertEqual(moves[0].lines[2].debit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[2].amount_second_currency, None)
             self.assertEqual(moves[0].lines[2].party, None)
             self.assertEqual(moves[0].lines[2].description, 'line 1')
-            self.assertEqual(moves[0].lines[2].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[2].origin.rec_name,
                 'Rev/Sp|5.00 usd|line 1 [In-Category [2345]]')
             self.assertEqual(len(moves[0].lines[2].tax_lines), 1)
-            self.assertEqual(moves[0].lines[2].tax_lines[0].amount, Decimal('0.46'))
+            self.assertEqual(
+                moves[0].lines[2].tax_lines[0].amount, Decimal('0.46'))
             self.assertEqual(moves[0].lines[2].tax_lines[0].type, 'tax')
-            self.assertEqual(moves[0].lines[2].tax_lines[0].tax.rec_name, 'Tax Half')
+            self.assertEqual(
+                moves[0].lines[2].tax_lines[0].tax.rec_name, 'Tax Half')
 
-            self.assertEqual(moves[0].lines[3].rec_name, '(2345 - Account Category)')
+            self.assertEqual(
+                moves[0].lines[3].rec_name, '(2345 - Account Category)')
             self.assertEqual(moves[0].lines[3].credit, Decimal('4.17'))
             self.assertEqual(moves[0].lines[3].debit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[3].amount_second_currency, None)
             self.assertEqual(moves[0].lines[3].party, None)
             self.assertEqual(moves[0].lines[3].description, 'line 2')
-            self.assertEqual(moves[0].lines[3].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[3].origin.rec_name,
                 'Rev/Sp|5.00 usd|line 2 [In-Category [2345]]')
             self.assertEqual(len(moves[0].lines[3].tax_lines), 1)
-            self.assertEqual(moves[0].lines[3].tax_lines[0].amount, Decimal('4.17'))
+            self.assertEqual(
+                moves[0].lines[3].tax_lines[0].amount, Decimal('4.17'))
             self.assertEqual(moves[0].lines[3].tax_lines[0].type, 'base')
-            self.assertEqual(moves[0].lines[3].tax_lines[0].tax.rec_name, 'Tax Full')
+            self.assertEqual(
+                moves[0].lines[3].tax_lines[0].tax.rec_name, 'Tax Full')
 
             self.assertEqual(moves[0].lines[4].rec_name, '(2235 - Tax Full)')
             self.assertEqual(moves[0].lines[4].credit, Decimal('0.83'))
             self.assertEqual(moves[0].lines[4].debit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[4].amount_second_currency, None)
             self.assertEqual(moves[0].lines[4].party, None)
             self.assertEqual(moves[0].lines[4].description, 'line 2')
-            self.assertEqual(moves[0].lines[4].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[4].origin.rec_name,
                 'Rev/Sp|5.00 usd|line 2 [In-Category [2345]]')
             self.assertEqual(len(moves[0].lines[4].tax_lines), 1)
-            self.assertEqual(moves[0].lines[4].tax_lines[0].amount, Decimal('0.83'))
+            self.assertEqual(
+                moves[0].lines[4].tax_lines[0].amount, Decimal('0.83'))
             self.assertEqual(moves[0].lines[4].tax_lines[0].type, 'tax')
-            self.assertEqual(moves[0].lines[4].tax_lines[0].tax.rec_name, 'Tax Full')
+            self.assertEqual(
+                moves[0].lines[4].tax_lines[0].tax.rec_name, 'Tax Full')
 
             self.assertEqual(moves[0].lines[5].rec_name, '0123 - Account Book')
             self.assertEqual(moves[0].lines[5].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[5].debit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[5].amount_second_currency, None)
             self.assertEqual(moves[0].lines[5].party, None)
             self.assertEqual(len(moves[0].lines[5].tax_lines), 0)
@@ -1953,15 +2044,16 @@
 
             self.assertEqual(moves[0].lines[6].rec_name, '(Main Receivable)')
             self.assertEqual(moves[0].lines[6].credit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[6].debit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[6].amount_second_currency, None)
             self.assertEqual(moves[0].lines[6].party.rec_name, 'Party')
             self.assertEqual(len(moves[0].lines[6].tax_lines), 0)
-            self.assertEqual(moves[0].lines[6].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[6].origin.rec_name,
                 '05/05/2022|Rev/Sp|10.00 usd|sell something [-]')
 
             # delete move
             Line.wfedit([book.lines[0]])
             self.assertEqual(len(book.lines[0].moves), 0)
 
             # create move again
@@ -1972,15 +2064,16 @@
             # post move
             self.assertEqual(Reconciliation.search_count([]), 0)
             Line.wfdone([book.lines[0]])
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(book.lines[0].moves[0].state, 'posted')
 
             rec_lines = Reconciliation.search([])
-            rec_move_ids = [x.id for x in book.lines[0].moves[0].lines if x.party]
+            rec_move_ids = [
+                x.id for x in book.lines[0].moves[0].lines if x.party]
             self.assertEqual(len(rec_move_ids), 2)
 
             self.assertEqual(len(rec_lines), 1)
             self.assertEqual(len(rec_lines[0].lines), 2)
 
             self.assertTrue(rec_lines[0].lines[0].id in rec_move_ids)
             self.assertTrue(rec_lines[0].lines[1].id in rec_move_ids)
@@ -1989,35 +2082,33 @@
     def test_line_check_wf_in_booking_2nd_currency_noparty(self):
         """ create cashbook + line, check booking in-type,
             2nd-currency
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
         Category = pool.get('cashbook.category')
         Account = pool.get('account.account')
         AccountType = pool.get('account.account.type')
         Journal = pool.get('account.journal')
         Move = pool.get('account.move')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         self.prep_accounting(company)
         (usd, euro) = self.prep_2nd_currency(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             acc_type, = AccountType.search([('name', '=', 'Cash')])
 
             accounts = Account.create([{
                 'name': 'Account Book',
                 'code': '0123',
                 'type': acc_type.id,
                 }, {
@@ -2058,43 +2149,49 @@
                         'party': party.id,
                     }])],
                 }])
             self.assertEqual(book.rec_name, 'Book 1 | 10.00 usd | Open')
             self.assertEqual(book.account.rec_name, '0123 - Account Book')
             self.assertEqual(book.currency.code, 'usd')
             self.assertEqual(len(book.lines), 1)
-            self.assertEqual(book.lines[0].rec_name,
+            self.assertEqual(
+                book.lines[0].rec_name,
                 '05/05/2022|Rev|10.00 usd|sell something [In-Category [2345]]')
             self.assertEqual(len(book.lines[0].moves), 0)
-            self.assertEqual(book.lines[0].category.rec_name, 'In-Category [2345]')
+            self.assertEqual(
+                book.lines[0].category.rec_name, 'In-Category [2345]')
 
             self.assertEqual(Move.search_count([]), 0)
             Line.wfcheck([book.lines[0]])
 
             moves = Move.search([])
             self.assertEqual(len(moves), 1)
             self.assertEqual(len(moves[0].lines), 2)
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(moves[0].state, 'draft')
             self.assertEqual(moves[0].date, date(2022, 5, 5))
             self.assertEqual(moves[0].description, 'sell something')
             self.assertEqual(moves[0].period.rec_name, '2022-05')
             self.assertEqual(moves[0].journal.rec_name, 'Cashbook')
-            self.assertEqual(moves[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].origin.rec_name,
                 '05/05/2022|Rev|10.00 usd|sell something [In-Category [2345]]')
-            self.assertEqual(moves[0].lines[0].rec_name, '(2345 - Account Category)')
+            self.assertEqual(
+                moves[0].lines[0].rec_name, '(2345 - Account Category)')
             self.assertEqual(moves[0].lines[0].credit, Decimal('9.52'))
             self.assertEqual(moves[0].lines[0].debit, Decimal('0.0'))
-            self.assertEqual(moves[0].lines[0].amount_second_currency, Decimal('-10.0'))
+            self.assertEqual(
+                moves[0].lines[0].amount_second_currency, Decimal('-10.0'))
             self.assertEqual(moves[0].lines[0].second_currency.rec_name, 'usd')
 
             self.assertEqual(moves[0].lines[1].rec_name, '0123 - Account Book')
             self.assertEqual(moves[0].lines[1].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[1].debit, Decimal('9.52'))
-            self.assertEqual(moves[0].lines[1].amount_second_currency, Decimal('10.0'))
+            self.assertEqual(
+                moves[0].lines[1].amount_second_currency, Decimal('10.0'))
             self.assertEqual(moves[0].lines[1].second_currency.rec_name, 'usd')
 
             # delete move
             Line.wfedit([book.lines[0]])
             self.assertEqual(len(book.lines[0].moves), 0)
 
             # create move again
@@ -2111,35 +2208,33 @@
     def test_line_check_wf_in_booking_2nd_currency_noparty_tax(self):
         """ create cashbook + line, check booking in-type,
             2nd-currency, net + tax
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
         Category = pool.get('cashbook.category')
         Account = pool.get('account.account')
         AccountType = pool.get('account.account.type')
         Journal = pool.get('account.journal')
         Move = pool.get('account.move')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         self.prep_accounting(company)
         (usd, euro) = self.prep_2nd_currency(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             taxes = self.prep_line_taxes()
             acc_type, = AccountType.search([('name', '=', 'Cash')])
 
             accounts = Account.create([{
                 'name': 'Account Book',
                 'code': '0123',
                 'type': acc_type.id,
@@ -2187,26 +2282,29 @@
                         'party': party.id,
                     }])],
                 }])
             self.assertEqual(book.rec_name, 'Book 1 | 10.00 usd | Open')
             self.assertEqual(book.account.rec_name, '0123 - Account Book')
             self.assertEqual(book.currency.code, 'usd')
             self.assertEqual(len(book.lines), 1)
-            self.assertEqual(book.lines[0].rec_name,
+            self.assertEqual(
+                book.lines[0].rec_name,
                 '05/05/2022|Rev|10.00 usd|sell something [In-Category [2345]]')
             self.assertEqual(len(book.lines[0].moves), 0)
-            self.assertEqual(book.lines[0].category.rec_name, 'In-Category [2345]')
+            self.assertEqual(
+                book.lines[0].category.rec_name, 'In-Category [2345]')
 
             # add tax
             book.lines[0].ena_tax1 = True
             book.lines[0].on_change_ena_tax1()
             book.lines[0].save()
 
             # check
-            self.assertEqual(book.lines[0].category.rec_name, 'In-Category [2345]')
+            self.assertEqual(
+                book.lines[0].category.rec_name, 'In-Category [2345]')
             self.assertEqual(book.lines[0].currency.rec_name, 'usd')
             self.assertEqual(book.lines[0].amount, Decimal('10.0'))
             self.assertEqual(book.lines[0].ena_tax1, True)
             self.assertEqual(book.lines[0].amount_tax1, Decimal('0.91'))
             self.assertEqual(book.lines[0].amount_net, Decimal('9.09'))
 
             self.assertEqual(Move.search_count([]), 0)
@@ -2217,41 +2315,50 @@
             self.assertEqual(len(moves[0].lines), 3)
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(moves[0].state, 'draft')
             self.assertEqual(moves[0].date, date(2022, 5, 5))
             self.assertEqual(moves[0].description, 'sell something')
             self.assertEqual(moves[0].period.rec_name, '2022-05')
             self.assertEqual(moves[0].journal.rec_name, 'Cashbook')
-            self.assertEqual(moves[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].origin.rec_name,
                 '05/05/2022|Rev|10.00 usd|sell something [In-Category [2345]]')
 
             self.assertEqual(moves[0].lines[0].rec_name, '(2234 - Tax Half)')
             self.assertEqual(moves[0].lines[0].credit, Decimal('0.86'))
             self.assertEqual(moves[0].lines[0].debit, Decimal('0.0'))
-            self.assertEqual(moves[0].lines[0].amount_second_currency, Decimal('-0.91'))
+            self.assertEqual(
+                moves[0].lines[0].amount_second_currency, Decimal('-0.91'))
             self.assertEqual(moves[0].lines[0].second_currency.rec_name, 'usd')
             self.assertEqual(len(moves[0].lines[0].tax_lines), 1)
-            self.assertEqual(moves[0].lines[0].tax_lines[0].amount, Decimal('0.86'))
+            self.assertEqual(
+                moves[0].lines[0].tax_lines[0].amount, Decimal('0.86'))
             self.assertEqual(moves[0].lines[0].tax_lines[0].type, 'tax')
-            self.assertEqual(moves[0].lines[0].tax_lines[0].tax.rec_name, 'Tax Half')
+            self.assertEqual(
+                moves[0].lines[0].tax_lines[0].tax.rec_name, 'Tax Half')
 
-            self.assertEqual(moves[0].lines[1].rec_name, '(2345 - Account Category)')
+            self.assertEqual(
+                moves[0].lines[1].rec_name, '(2345 - Account Category)')
             self.assertEqual(moves[0].lines[1].credit, Decimal('8.66'))
             self.assertEqual(moves[0].lines[1].debit, Decimal('0.0'))
-            self.assertEqual(moves[0].lines[1].amount_second_currency, Decimal('-9.09'))
+            self.assertEqual(
+                moves[0].lines[1].amount_second_currency, Decimal('-9.09'))
             self.assertEqual(moves[0].lines[1].second_currency.rec_name, 'usd')
             self.assertEqual(len(moves[0].lines[1].tax_lines), 1)
-            self.assertEqual(moves[0].lines[1].tax_lines[0].amount, Decimal('8.66'))
+            self.assertEqual(
+                moves[0].lines[1].tax_lines[0].amount, Decimal('8.66'))
             self.assertEqual(moves[0].lines[1].tax_lines[0].type, 'base')
-            self.assertEqual(moves[0].lines[1].tax_lines[0].tax.rec_name, 'Tax Half')
+            self.assertEqual(
+                moves[0].lines[1].tax_lines[0].tax.rec_name, 'Tax Half')
 
             self.assertEqual(moves[0].lines[2].rec_name, '0123 - Account Book')
             self.assertEqual(moves[0].lines[2].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[2].debit, Decimal('9.52'))
-            self.assertEqual(moves[0].lines[2].amount_second_currency, Decimal('10.0'))
+            self.assertEqual(
+                moves[0].lines[2].amount_second_currency, Decimal('10.0'))
             self.assertEqual(moves[0].lines[2].second_currency.rec_name, 'usd')
             self.assertEqual(len(moves[0].lines[2].tax_lines), 0)
 
             # delete move
             Line.wfedit([book.lines[0]])
             self.assertEqual(len(book.lines[0].moves), 0)
 
@@ -2269,35 +2376,33 @@
     def test_line_check_wf_in_split_booking_2nd_currency_noparty(self):
         """ create cashbook + line, check booking in-type,
             2nd-currency
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
         Category = pool.get('cashbook.category')
         Account = pool.get('account.account')
         AccountType = pool.get('account.account.type')
         Journal = pool.get('account.journal')
         Move = pool.get('account.move')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         self.prep_accounting(company)
         (usd, euro) = self.prep_2nd_currency(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             acc_type, = AccountType.search([('name', '=', 'Cash')])
 
             accounts = Account.create([{
                 'name': 'Account Book',
                 'code': '0123',
                 'type': acc_type.id,
                 }, {
@@ -2346,64 +2451,78 @@
                             }])],
                     }])],
                 }])
             self.assertEqual(book.rec_name, 'Book 1 | 10.00 usd | Open')
             self.assertEqual(book.account.rec_name, '0123 - Account Book')
             self.assertEqual(book.currency.code, 'usd')
             self.assertEqual(len(book.lines), 1)
-            self.assertEqual(book.lines[0].rec_name,
+            self.assertEqual(
+                book.lines[0].rec_name,
                 '05/05/2022|Rev/Sp|10.00 usd|sell something [-]')
             self.assertEqual(len(book.lines[0].moves), 0)
             self.assertEqual(book.lines[0].category, None)
             self.assertEqual(len(book.lines[0].splitlines), 2)
-            self.assertEqual(book.lines[0].splitlines[0].rec_name, \
+            self.assertEqual(
+                book.lines[0].splitlines[0].rec_name,
                 'Rev/Sp|5.00 usd|line 1 [In-Category [2345]]')
-            self.assertEqual(book.lines[0].splitlines[1].rec_name, \
+            self.assertEqual(
+                book.lines[0].splitlines[1].rec_name,
                 'Rev/Sp|5.00 usd|line 2 [In-Category [2345]]')
 
             self.assertEqual(Move.search_count([]), 0)
             Line.wfcheck([book.lines[0]])
 
             moves = Move.search([])
             self.assertEqual(len(moves), 1)
             self.assertEqual(len(moves[0].lines), 3)
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(moves[0].state, 'draft')
             self.assertEqual(moves[0].date, date(2022, 5, 5))
             self.assertEqual(moves[0].description, 'sell something')
             self.assertEqual(moves[0].period.rec_name, '2022-05')
             self.assertEqual(moves[0].journal.rec_name, 'Cashbook')
-            self.assertEqual(moves[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].origin.rec_name,
                 '05/05/2022|Rev/Sp|10.00 usd|sell something [-]')
-            self.assertEqual(moves[0].lines[0].rec_name, '(2345 - Account Category)')
+            self.assertEqual(
+                moves[0].lines[0].rec_name, '(2345 - Account Category)')
             self.assertEqual(moves[0].lines[0].credit, Decimal('4.76'))
             self.assertEqual(moves[0].lines[0].debit, Decimal('0.0'))
-            self.assertEqual(moves[0].lines[0].amount_second_currency, Decimal('-5.0'))
+            self.assertEqual(
+                moves[0].lines[0].amount_second_currency, Decimal('-5.0'))
             self.assertEqual(moves[0].lines[0].second_currency.rec_name, 'usd')
             self.assertEqual(moves[0].lines[0].party, None)
             self.assertEqual(moves[0].lines[0].description, 'line 1')
             self.assertEqual(len(moves[0].lines[0].tax_lines), 0)
-            self.assertEqual(moves[0].lines[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[0].origin.rec_name,
                 'Rev/Sp|5.00 usd|line 1 [In-Category [2345]]')
 
-            self.assertEqual(moves[0].lines[1].rec_name, '(2345 - Account Category)')
+            self.assertEqual(
+                moves[0].lines[1].rec_name,
+                '(2345 - Account Category)')
             self.assertEqual(moves[0].lines[1].credit, Decimal('4.76'))
             self.assertEqual(moves[0].lines[1].debit, Decimal('0.0'))
-            self.assertEqual(moves[0].lines[1].amount_second_currency, Decimal('-5.0'))
+            self.assertEqual(
+                moves[0].lines[1].amount_second_currency,
+                Decimal('-5.0'))
             self.assertEqual(moves[0].lines[1].second_currency.rec_name, 'usd')
             self.assertEqual(moves[0].lines[1].party, None)
             self.assertEqual(moves[0].lines[1].description, 'line 2')
             self.assertEqual(len(moves[0].lines[1].tax_lines), 0)
-            self.assertEqual(moves[0].lines[1].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[1].origin.rec_name,
                 'Rev/Sp|5.00 usd|line 2 [In-Category [2345]]')
 
             self.assertEqual(moves[0].lines[2].rec_name, '0123 - Account Book')
             self.assertEqual(moves[0].lines[2].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[2].debit, Decimal('9.52'))
-            self.assertEqual(moves[0].lines[2].amount_second_currency, Decimal('10.0'))
+            self.assertEqual(
+                moves[0].lines[2].amount_second_currency,
+                Decimal('10.0'))
             self.assertEqual(moves[0].lines[2].second_currency.rec_name, 'usd')
             self.assertEqual(moves[0].lines[2].party, None)
             self.assertEqual(moves[0].lines[2].description, None)
             self.assertEqual(len(moves[0].lines[2].tax_lines), 0)
             self.assertEqual(moves[0].lines[2].origin, None)
 
             # delete move
@@ -2425,35 +2544,33 @@
         """ create cashbook + line, check booking in-type,
             2nd-currency, transfer with fee,
             company-currency: eur, 2x account-currency: usd
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
         Category = pool.get('cashbook.category')
         Account = pool.get('account.account')
         AccountType = pool.get('account.account.type')
         Journal = pool.get('account.journal')
         Move = pool.get('account.move')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         self.prep_accounting(company)
         (usd, euro) = self.prep_2nd_currency(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             acc_type, = AccountType.search([('name', '=', 'Cash')])
 
             accounts = Account.create([{
                 'name': 'Account Book 1',
                 'code': '0123',
                 'type': acc_type.id,
                 }, {
@@ -2532,73 +2649,93 @@
                             'description': 'transfer',
                             }])],
                     }])],
                 }])
             self.assertEqual(len(books[0].lines), 1)
             self.assertEqual(len(books[1].lines), 0)
 
-            self.assertEqual(books[0].lines[0].rec_name,
+            self.assertEqual(
+                books[0].lines[0].rec_name,
                 '05/05/2022|Rev/Sp|30.00 usd|transfer with fee [-]')
             self.assertEqual(len(books[0].lines[0].moves), 0)
             self.assertEqual(books[0].lines[0].category, None)
             self.assertEqual(len(books[0].lines[0].splitlines), 2)
-            self.assertEqual(books[0].lines[0].splitlines[0].rec_name, \
+            self.assertEqual(
+                books[0].lines[0].splitlines[0].rec_name,
                 'Rev/Sp|5.00 usd|fee [In-Category [2345]]')
-            self.assertEqual(books[0].lines[0].splitlines[1].rec_name, \
+            self.assertEqual(
+                books[0].lines[0].splitlines[1].rec_name,
                 'Rev/Sp|25.00 usd|transfer [Book 2 | 0.00 usd | Open]')
 
             self.assertEqual(Move.search_count([]), 0)
             Line.wfcheck([books[0].lines[0]])
 
             self.assertEqual(len(books[0].lines), 1)
             self.assertEqual(len(books[0].lines[0].moves), 1)
             self.assertEqual(len(books[1].lines), 1)
-            self.assertEqual(books[1].lines[0].rec_name,
+            self.assertEqual(
+                books[1].lines[0].rec_name,
                 '05/05/2022|to|-25.00 usd|transfer [Book 1 | 30.00 usd | Open]')
             self.assertEqual(len(books[1].lines[0].moves), 0)
-            self.assertEqual(books[1].lines[0].reference.rec_name,
+            self.assertEqual(
+                books[1].lines[0].reference.rec_name,
                 '05/05/2022|Rev/Sp|30.00 usd|transfer with fee [-]')
 
             moves = Move.search([])
             self.assertEqual(len(moves), 1)
             self.assertEqual(len(moves[0].lines), 3)
             self.assertEqual(len(books[0].lines[0].moves), 1)
             self.assertEqual(moves[0].state, 'draft')
             self.assertEqual(moves[0].date, date(2022, 5, 5))
             self.assertEqual(moves[0].description, 'transfer with fee')
             self.assertEqual(moves[0].period.rec_name, '2022-05')
             self.assertEqual(moves[0].journal.rec_name, 'Cashbook')
-            self.assertEqual(moves[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].origin.rec_name,
                 '05/05/2022|Rev/Sp|30.00 usd|transfer with fee [-]')
-            self.assertEqual(moves[0].lines[0].rec_name, '(2345 - Account Category)')
+            self.assertEqual(
+                moves[0].lines[0].rec_name,
+                '(2345 - Account Category)')
             self.assertEqual(moves[0].lines[0].credit, Decimal('4.76'))
             self.assertEqual(moves[0].lines[0].debit, Decimal('0.0'))
-            self.assertEqual(moves[0].lines[0].amount_second_currency, Decimal('-5.0'))
+            self.assertEqual(
+                moves[0].lines[0].amount_second_currency,
+                Decimal('-5.0'))
             self.assertEqual(moves[0].lines[0].second_currency.rec_name, 'usd')
             self.assertEqual(moves[0].lines[0].party, None)
             self.assertEqual(moves[0].lines[0].description, 'fee')
             self.assertEqual(len(moves[0].lines[0].tax_lines), 0)
-            self.assertEqual(moves[0].lines[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[0].origin.rec_name,
                 'Rev/Sp|5.00 usd|fee [In-Category [2345]]')
 
-            self.assertEqual(moves[0].lines[1].rec_name, '(3456 - Account Book 2)')
+            self.assertEqual(
+                moves[0].lines[1].rec_name,
+                '(3456 - Account Book 2)')
             self.assertEqual(moves[0].lines[1].credit, Decimal('23.81'))
             self.assertEqual(moves[0].lines[1].debit, Decimal('0.0'))
-            self.assertEqual(moves[0].lines[1].amount_second_currency, Decimal('-25.0'))
+            self.assertEqual(
+                moves[0].lines[1].amount_second_currency,
+                Decimal('-25.0'))
             self.assertEqual(moves[0].lines[1].second_currency.rec_name, 'usd')
             self.assertEqual(moves[0].lines[1].party, None)
             self.assertEqual(moves[0].lines[1].description, 'transfer')
             self.assertEqual(len(moves[0].lines[1].tax_lines), 0)
-            self.assertEqual(moves[0].lines[1].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[1].origin.rec_name,
                 'Rev/Sp|25.00 usd|transfer [Book 2 | -25.00 usd | Open]')
 
-            self.assertEqual(moves[0].lines[2].rec_name, '0123 - Account Book 1')
+            self.assertEqual(
+                moves[0].lines[2].rec_name,
+                '0123 - Account Book 1')
             self.assertEqual(moves[0].lines[2].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[2].debit, Decimal('28.57'))
-            self.assertEqual(moves[0].lines[2].amount_second_currency, Decimal('30.0'))
+            self.assertEqual(
+                moves[0].lines[2].amount_second_currency,
+                Decimal('30.0'))
             self.assertEqual(moves[0].lines[2].second_currency.rec_name, 'usd')
             self.assertEqual(moves[0].lines[2].party, None)
             self.assertEqual(moves[0].lines[2].description, None)
             self.assertEqual(len(moves[0].lines[2].tax_lines), 0)
             self.assertEqual(moves[0].lines[2].origin, None)
 
             # delete move
@@ -2622,35 +2759,33 @@
             company-currency: eur,
             1x account-currency: usd
             1x account-currency: eur
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
         Category = pool.get('cashbook.category')
         Account = pool.get('account.account')
         AccountType = pool.get('account.account.type')
         Journal = pool.get('account.journal')
         Move = pool.get('account.move')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         self.prep_accounting(company)
         (usd, euro) = self.prep_2nd_currency(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             acc_type, = AccountType.search([('name', '=', 'Cash')])
 
             accounts = Account.create([{
                 'name': 'Account Book 1',
                 'code': '0123',
                 'type': acc_type.id,
                 }, {
@@ -2729,73 +2864,93 @@
                             'description': 'transfer',
                             }])],
                     }])],
                 }])
             self.assertEqual(len(books[0].lines), 1)
             self.assertEqual(len(books[1].lines), 0)
 
-            self.assertEqual(books[0].lines[0].rec_name,
+            self.assertEqual(
+                books[0].lines[0].rec_name,
                 '05/05/2022|Rev/Sp|30.00 usd|transfer with fee [-]')
             self.assertEqual(len(books[0].lines[0].moves), 0)
             self.assertEqual(books[0].lines[0].category, None)
             self.assertEqual(len(books[0].lines[0].splitlines), 2)
-            self.assertEqual(books[0].lines[0].splitlines[0].rec_name, \
+            self.assertEqual(
+                books[0].lines[0].splitlines[0].rec_name,
                 'Rev/Sp|5.00 usd|fee [In-Category [2345]]')
-            self.assertEqual(books[0].lines[0].splitlines[1].rec_name, \
+            self.assertEqual(
+                books[0].lines[0].splitlines[1].rec_name,
                 'Rev/Sp|25.00 usd|transfer [Book 2 | 0.00 € | Open]')
 
             self.assertEqual(Move.search_count([]), 0)
             Line.wfcheck([books[0].lines[0]])
 
             self.assertEqual(len(books[0].lines), 1)
             self.assertEqual(len(books[0].lines[0].moves), 1)
             self.assertEqual(len(books[1].lines), 1)
-            self.assertEqual(books[1].lines[0].rec_name,
+            self.assertEqual(
+                books[1].lines[0].rec_name,
                 '05/05/2022|to|-23.81 €|transfer [Book 1 | 30.00 usd | Open]')
             self.assertEqual(len(books[1].lines[0].moves), 0)
-            self.assertEqual(books[1].lines[0].reference.rec_name,
+            self.assertEqual(
+                books[1].lines[0].reference.rec_name,
                 '05/05/2022|Rev/Sp|30.00 usd|transfer with fee [-]')
 
             moves = Move.search([])
             self.assertEqual(len(moves), 1)
             self.assertEqual(len(moves[0].lines), 3)
             self.assertEqual(len(books[0].lines[0].moves), 1)
             self.assertEqual(moves[0].state, 'draft')
             self.assertEqual(moves[0].date, date(2022, 5, 5))
             self.assertEqual(moves[0].description, 'transfer with fee')
             self.assertEqual(moves[0].period.rec_name, '2022-05')
             self.assertEqual(moves[0].journal.rec_name, 'Cashbook')
-            self.assertEqual(moves[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].origin.rec_name,
                 '05/05/2022|Rev/Sp|30.00 usd|transfer with fee [-]')
-            self.assertEqual(moves[0].lines[0].rec_name, '(2345 - Account Category)')
+            self.assertEqual(
+                moves[0].lines[0].rec_name,
+                '(2345 - Account Category)')
             self.assertEqual(moves[0].lines[0].credit, Decimal('4.76'))
             self.assertEqual(moves[0].lines[0].debit, Decimal('0.0'))
-            self.assertEqual(moves[0].lines[0].amount_second_currency, Decimal('-5.0'))
+            self.assertEqual(
+                moves[0].lines[0].amount_second_currency,
+                Decimal('-5.0'))
             self.assertEqual(moves[0].lines[0].second_currency.rec_name, 'usd')
             self.assertEqual(moves[0].lines[0].party, None)
             self.assertEqual(moves[0].lines[0].description, 'fee')
             self.assertEqual(len(moves[0].lines[0].tax_lines), 0)
-            self.assertEqual(moves[0].lines[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[0].origin.rec_name,
                 'Rev/Sp|5.00 usd|fee [In-Category [2345]]')
 
-            self.assertEqual(moves[0].lines[1].rec_name, '(3456 - Account Book 2)')
+            self.assertEqual(
+                moves[0].lines[1].rec_name,
+                '(3456 - Account Book 2)')
             self.assertEqual(moves[0].lines[1].credit, Decimal('23.81'))
             self.assertEqual(moves[0].lines[1].debit, Decimal('0.0'))
-            self.assertEqual(moves[0].lines[1].amount_second_currency, Decimal('-25.0'))
+            self.assertEqual(
+                moves[0].lines[1].amount_second_currency,
+                Decimal('-25.0'))
             self.assertEqual(moves[0].lines[1].second_currency.rec_name, 'usd')
             self.assertEqual(moves[0].lines[1].party, None)
             self.assertEqual(moves[0].lines[1].description, 'transfer')
             self.assertEqual(len(moves[0].lines[1].tax_lines), 0)
-            self.assertEqual(moves[0].lines[1].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[1].origin.rec_name,
                 'Rev/Sp|25.00 usd|transfer [Book 2 | -23.81 € | Open]')
 
-            self.assertEqual(moves[0].lines[2].rec_name, '0123 - Account Book 1')
+            self.assertEqual(
+                moves[0].lines[2].rec_name,
+                '0123 - Account Book 1')
             self.assertEqual(moves[0].lines[2].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[2].debit, Decimal('28.57'))
-            self.assertEqual(moves[0].lines[2].amount_second_currency, Decimal('30.0'))
+            self.assertEqual(
+                moves[0].lines[2].amount_second_currency,
+                Decimal('30.0'))
             self.assertEqual(moves[0].lines[2].second_currency.rec_name, 'usd')
             self.assertEqual(moves[0].lines[2].party, None)
             self.assertEqual(moves[0].lines[2].description, None)
             self.assertEqual(len(moves[0].lines[2].tax_lines), 0)
             self.assertEqual(moves[0].lines[2].origin, None)
 
             # delete move
@@ -2816,36 +2971,34 @@
     def test_line_check_wf_in_booking_2nd_currency_withparty(self):
         """ create cashbook + line, check booking in-type,
             2nd-currency
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
         Category = pool.get('cashbook.category')
         Account = pool.get('account.account')
         AccountType = pool.get('account.account.type')
         Journal = pool.get('account.journal')
         Move = pool.get('account.move')
         Reconciliation = pool.get('account.move.reconciliation')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         self.prep_accounting(company)
         (usd, euro) = self.prep_2nd_currency(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             acc_type, = AccountType.search([('name', '=', 'Cash')])
 
             accounts = Account.create([{
                 'name': 'Account Book',
                 'code': '0123',
                 'type': acc_type.id,
                 }, {
@@ -2886,56 +3039,70 @@
                         'party': party.id,
                     }])],
                 }])
             self.assertEqual(book.rec_name, 'Book 1 | 10.00 usd | Open')
             self.assertEqual(book.account.rec_name, '0123 - Account Book')
             self.assertEqual(book.currency.code, 'usd')
             self.assertEqual(len(book.lines), 1)
-            self.assertEqual(book.lines[0].rec_name,
+            self.assertEqual(
+                book.lines[0].rec_name,
                 '05/05/2022|Rev|10.00 usd|sell something [In-Category [2345]]')
             self.assertEqual(len(book.lines[0].moves), 0)
-            self.assertEqual(book.lines[0].category.rec_name, 'In-Category [2345]')
+            self.assertEqual(
+                book.lines[0].category.rec_name,
+                'In-Category [2345]')
 
             self.assertEqual(Move.search_count([]), 0)
             Line.wfcheck([book.lines[0]])
 
             moves = Move.search([])
             self.assertEqual(len(moves), 1)
             self.assertEqual(len(moves[0].lines), 4)
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(moves[0].state, 'draft')
             self.assertEqual(moves[0].date, date(2022, 5, 5))
             self.assertEqual(moves[0].description, 'sell something')
             self.assertEqual(moves[0].period.rec_name, '2022-05')
             self.assertEqual(moves[0].journal.rec_name, 'Cashbook')
-            self.assertEqual(moves[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].origin.rec_name,
                 '05/05/2022|Rev|10.00 usd|sell something [In-Category [2345]]')
 
             self.assertEqual(moves[0].lines[0].rec_name, 'Main Receivable')
             self.assertEqual(moves[0].lines[0].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[0].debit, Decimal('9.52'))
-            self.assertEqual(moves[0].lines[0].amount_second_currency, Decimal('10.0'))
+            self.assertEqual(
+                moves[0].lines[0].amount_second_currency,
+                Decimal('10.0'))
             self.assertEqual(moves[0].lines[0].second_currency.rec_name, 'usd')
 
-            self.assertEqual(moves[0].lines[1].rec_name, '(2345 - Account Category)')
+            self.assertEqual(
+                moves[0].lines[1].rec_name,
+                '(2345 - Account Category)')
             self.assertEqual(moves[0].lines[1].credit, Decimal('9.52'))
             self.assertEqual(moves[0].lines[1].debit, Decimal('0.0'))
-            self.assertEqual(moves[0].lines[1].amount_second_currency, Decimal('-10.0'))
+            self.assertEqual(
+                moves[0].lines[1].amount_second_currency,
+                Decimal('-10.0'))
             self.assertEqual(moves[0].lines[1].second_currency.rec_name, 'usd')
 
             self.assertEqual(moves[0].lines[2].rec_name, '0123 - Account Book')
             self.assertEqual(moves[0].lines[2].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[2].debit, Decimal('9.52'))
-            self.assertEqual(moves[0].lines[2].amount_second_currency, Decimal('10.0'))
+            self.assertEqual(
+                moves[0].lines[2].amount_second_currency,
+                Decimal('10.0'))
             self.assertEqual(moves[0].lines[2].second_currency.rec_name, 'usd')
 
             self.assertEqual(moves[0].lines[3].rec_name, '(Main Receivable)')
             self.assertEqual(moves[0].lines[3].credit, Decimal('9.52'))
             self.assertEqual(moves[0].lines[3].debit, Decimal('0.0'))
-            self.assertEqual(moves[0].lines[3].amount_second_currency, Decimal('-10.0'))
+            self.assertEqual(
+                moves[0].lines[3].amount_second_currency,
+                Decimal('-10.0'))
             self.assertEqual(moves[0].lines[3].second_currency.rec_name, 'usd')
 
             # delete move
             Line.wfedit([book.lines[0]])
             self.assertEqual(len(book.lines[0].moves), 0)
 
             # create move again
@@ -2945,15 +3112,16 @@
 
             # post move
             Line.wfdone([book.lines[0]])
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(book.lines[0].moves[0].state, 'posted')
 
             rec_lines = Reconciliation.search([])
-            rec_move_ids = [x.id for x in book.lines[0].moves[0].lines if x.party]
+            rec_move_ids = [
+                x.id for x in book.lines[0].moves[0].lines if x.party]
             self.assertEqual(len(rec_move_ids), 2)
 
             self.assertEqual(len(rec_lines), 1)
             self.assertEqual(len(rec_lines[0].lines), 2)
 
             self.assertTrue(rec_lines[0].lines[0].id in rec_move_ids)
             self.assertTrue(rec_lines[0].lines[1].id in rec_move_ids)
@@ -2962,36 +3130,34 @@
     def test_line_check_wf_in_split_booking_2nd_currency_withparty(self):
         """ create cashbook + line, check booking in-type,
             2nd-currency
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
         Category = pool.get('cashbook.category')
         Account = pool.get('account.account')
         AccountType = pool.get('account.account.type')
         Journal = pool.get('account.journal')
         Move = pool.get('account.move')
         Reconciliation = pool.get('account.move.reconciliation')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         self.prep_accounting(company)
         (usd, euro) = self.prep_2nd_currency(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             acc_type, = AccountType.search([('name', '=', 'Cash')])
 
             accounts = Account.create([{
                 'name': 'Account Book',
                 'code': '0123',
                 'type': acc_type.id,
                 }, {
@@ -3040,91 +3206,113 @@
                             }])],
                     }])],
                 }])
             self.assertEqual(book.rec_name, 'Book 1 | 10.00 usd | Open')
             self.assertEqual(book.account.rec_name, '0123 - Account Book')
             self.assertEqual(book.currency.code, 'usd')
             self.assertEqual(len(book.lines), 1)
-            self.assertEqual(book.lines[0].rec_name,
+            self.assertEqual(
+                book.lines[0].rec_name,
                 '05/05/2022|Rev/Sp|10.00 usd|sell something [-]')
             self.assertEqual(len(book.lines[0].moves), 0)
             self.assertEqual(book.lines[0].category, None)
             self.assertEqual(len(book.lines[0].splitlines), 2)
-            self.assertEqual(book.lines[0].splitlines[0].rec_name, \
+            self.assertEqual(
+                book.lines[0].splitlines[0].rec_name,
                 'Rev/Sp|5.00 usd|line 1 [In-Category [2345]]')
-            self.assertEqual(book.lines[0].splitlines[1].rec_name, \
+            self.assertEqual(
+                book.lines[0].splitlines[1].rec_name,
                 'Rev/Sp|5.00 usd|line 2 [In-Category [2345]]')
 
             self.assertEqual(Move.search_count([]), 0)
             Line.wfcheck([book.lines[0]])
 
             moves = Move.search([])
             self.assertEqual(len(moves), 1)
             self.assertEqual(len(moves[0].lines), 5)
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(moves[0].state, 'draft')
             self.assertEqual(moves[0].date, date(2022, 5, 5))
             self.assertEqual(moves[0].description, 'sell something')
             self.assertEqual(moves[0].period.rec_name, '2022-05')
             self.assertEqual(moves[0].journal.rec_name, 'Cashbook')
-            self.assertEqual(moves[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].origin.rec_name,
                 '05/05/2022|Rev/Sp|10.00 usd|sell something [-]')
 
             self.assertEqual(moves[0].lines[0].rec_name, 'Main Receivable')
             self.assertEqual(moves[0].lines[0].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[0].debit, Decimal('9.52'))
-            self.assertEqual(moves[0].lines[0].amount_second_currency, Decimal('10.0'))
+            self.assertEqual(
+                moves[0].lines[0].amount_second_currency,
+                Decimal('10.0'))
             self.assertEqual(moves[0].lines[0].second_currency.rec_name, 'usd')
             self.assertEqual(moves[0].lines[0].party.rec_name, 'Party')
             self.assertEqual(moves[0].lines[0].description, None)
             self.assertEqual(len(moves[0].lines[0].tax_lines), 0)
-            self.assertEqual(moves[0].lines[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[0].origin.rec_name,
                 '05/05/2022|Rev/Sp|10.00 usd|sell something [-]')
 
-            self.assertEqual(moves[0].lines[1].rec_name, '(2345 - Account Category)')
+            self.assertEqual(
+                moves[0].lines[1].rec_name,
+                '(2345 - Account Category)')
             self.assertEqual(moves[0].lines[1].credit, Decimal('4.76'))
             self.assertEqual(moves[0].lines[1].debit, Decimal('0.0'))
-            self.assertEqual(moves[0].lines[1].amount_second_currency, Decimal('-5.0'))
+            self.assertEqual(
+                moves[0].lines[1].amount_second_currency,
+                Decimal('-5.0'))
             self.assertEqual(moves[0].lines[1].second_currency.rec_name, 'usd')
             self.assertEqual(moves[0].lines[1].party, None)
             self.assertEqual(moves[0].lines[1].description, 'line 1')
             self.assertEqual(len(moves[0].lines[1].tax_lines), 0)
-            self.assertEqual(moves[0].lines[1].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[1].origin.rec_name,
                 'Rev/Sp|5.00 usd|line 1 [In-Category [2345]]')
 
-            self.assertEqual(moves[0].lines[2].rec_name, '(2345 - Account Category)')
+            self.assertEqual(
+                moves[0].lines[2].rec_name,
+                '(2345 - Account Category)')
             self.assertEqual(moves[0].lines[2].credit, Decimal('4.76'))
             self.assertEqual(moves[0].lines[2].debit, Decimal('0.0'))
-            self.assertEqual(moves[0].lines[2].amount_second_currency, Decimal('-5.0'))
+            self.assertEqual(
+                moves[0].lines[2].amount_second_currency,
+                Decimal('-5.0'))
             self.assertEqual(moves[0].lines[2].second_currency.rec_name, 'usd')
             self.assertEqual(moves[0].lines[2].party, None)
             self.assertEqual(moves[0].lines[2].description, 'line 2')
             self.assertEqual(len(moves[0].lines[2].tax_lines), 0)
-            self.assertEqual(moves[0].lines[2].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[2].origin.rec_name,
                 'Rev/Sp|5.00 usd|line 2 [In-Category [2345]]')
 
             self.assertEqual(moves[0].lines[3].rec_name, '0123 - Account Book')
             self.assertEqual(moves[0].lines[3].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[3].debit, Decimal('9.52'))
-            self.assertEqual(moves[0].lines[3].amount_second_currency, Decimal('10.0'))
+            self.assertEqual(
+                moves[0].lines[3].amount_second_currency,
+                Decimal('10.0'))
             self.assertEqual(moves[0].lines[3].second_currency.rec_name, 'usd')
             self.assertEqual(moves[0].lines[3].party, None)
             self.assertEqual(moves[0].lines[3].description, None)
             self.assertEqual(len(moves[0].lines[3].tax_lines), 0)
             self.assertEqual(moves[0].lines[3].origin, None)
 
             self.assertEqual(moves[0].lines[4].rec_name, '(Main Receivable)')
             self.assertEqual(moves[0].lines[4].credit, Decimal('9.52'))
             self.assertEqual(moves[0].lines[4].debit, Decimal('0.0'))
-            self.assertEqual(moves[0].lines[4].amount_second_currency, Decimal('-10.0'))
+            self.assertEqual(
+                moves[0].lines[4].amount_second_currency,
+                Decimal('-10.0'))
             self.assertEqual(moves[0].lines[4].second_currency.rec_name, 'usd')
             self.assertEqual(moves[0].lines[4].party.rec_name, 'Party')
             self.assertEqual(moves[0].lines[4].description, None)
             self.assertEqual(len(moves[0].lines[4].tax_lines), 0)
-            self.assertEqual(moves[0].lines[4].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[4].origin.rec_name,
                 '05/05/2022|Rev/Sp|10.00 usd|sell something [-]')
 
             # delete move
             Line.wfedit([book.lines[0]])
             self.assertEqual(len(book.lines[0].moves), 0)
 
             # create move again
@@ -3134,15 +3322,16 @@
 
             # post move
             Line.wfdone([book.lines[0]])
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(book.lines[0].moves[0].state, 'posted')
 
             rec_lines = Reconciliation.search([])
-            rec_move_ids = [x.id for x in book.lines[0].moves[0].lines if x.party]
+            rec_move_ids = [
+                x.id for x in book.lines[0].moves[0].lines if x.party]
             self.assertEqual(len(rec_move_ids), 2)
 
             self.assertEqual(len(rec_lines), 1)
             self.assertEqual(len(rec_lines[0].lines), 2)
 
             self.assertTrue(rec_lines[0].lines[0].id in rec_move_ids)
             self.assertTrue(rec_lines[0].lines[1].id in rec_move_ids)
@@ -3151,34 +3340,32 @@
     def test_line_check_wf_out_booking_noparty(self):
         """ create cashbook + line, check booking out-type,
             company-currency
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
         Category = pool.get('cashbook.category')
         Account = pool.get('account.account')
         AccountType = pool.get('account.account.type')
         Journal = pool.get('account.journal')
         Move = pool.get('account.move')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         self.prep_accounting(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             acc_type, = AccountType.search([('name', '=', 'Cash')])
 
             accounts = Account.create([{
                 'name': 'Account Book',
                 'code': '0123',
                 'type': acc_type.id,
                 }, {
@@ -3218,38 +3405,46 @@
                         'amount': Decimal('10.0'),
                         'party': party.id,
                     }])],
                 }])
             self.assertEqual(book.rec_name, 'Book 1 | -10.00 usd | Open')
             self.assertEqual(book.account.rec_name, '0123 - Account Book')
             self.assertEqual(len(book.lines), 1)
-            self.assertEqual(book.lines[0].rec_name,
+            self.assertEqual(
+                book.lines[0].rec_name,
                 '05/05/2022|Exp|-10.00 usd|buy something [Out-Category [2345]]')
             self.assertEqual(len(book.lines[0].moves), 0)
-            self.assertEqual(book.lines[0].category.rec_name, 'Out-Category [2345]')
+            self.assertEqual(
+                book.lines[0].category.rec_name,
+                'Out-Category [2345]')
 
             self.assertEqual(Move.search_count([]), 0)
             Line.wfcheck([book.lines[0]])
 
             moves = Move.search([])
             self.assertEqual(len(moves), 1)
             self.assertEqual(len(moves[0].lines), 2)
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(moves[0].state, 'draft')
             self.assertEqual(moves[0].date, date(2022, 5, 5))
             self.assertEqual(moves[0].description, 'buy something')
             self.assertEqual(moves[0].period.rec_name, '2022-05')
             self.assertEqual(moves[0].journal.rec_name, 'Cashbook')
-            self.assertEqual(moves[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].origin.rec_name,
                 '05/05/2022|Exp|-10.00 usd|buy something [Out-Category [2345]]')
-            self.assertEqual(moves[0].lines[0].rec_name, '2345 - Account Category')
+            self.assertEqual(
+                moves[0].lines[0].rec_name,
+                '2345 - Account Category')
             self.assertEqual(moves[0].lines[0].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[0].debit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[0].amount_second_currency, None)
-            self.assertEqual(moves[0].lines[1].rec_name, '(0123 - Account Book)')
+            self.assertEqual(
+                moves[0].lines[1].rec_name,
+                '(0123 - Account Book)')
             self.assertEqual(moves[0].lines[1].credit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[1].debit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[1].amount_second_currency, None)
 
             # delete move
             Line.wfedit([book.lines[0]])
             self.assertEqual(len(book.lines[0].moves), 0)
@@ -3268,34 +3463,32 @@
     def test_line_check_wf_out_booking_noparty_tax(self):
         """ create cashbook + line, check booking out-type,
             company-currency
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
         Category = pool.get('cashbook.category')
         Account = pool.get('account.account')
         AccountType = pool.get('account.account.type')
         Journal = pool.get('account.journal')
         Move = pool.get('account.move')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         self.prep_accounting(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             taxes = self.prep_line_taxes()
             acc_type, = AccountType.search([('name', '=', 'Cash')])
 
             accounts = Account.create([{
                 'name': 'Account Book',
                 'code': '0123',
                 'type': acc_type.id,
@@ -3343,61 +3536,79 @@
                         'party': party.id,
                         'ena_tax1': True,
                     }])],
                 }])
             self.assertEqual(book.rec_name, 'Book 1 | -10.00 usd | Open')
             self.assertEqual(book.account.rec_name, '0123 - Account Book')
             self.assertEqual(len(book.lines), 1)
-            self.assertEqual(book.lines[0].rec_name,
+            self.assertEqual(
+                book.lines[0].rec_name,
                 '05/05/2022|Exp|-10.00 usd|buy something [Out-Category [2345]]')
             self.assertEqual(len(book.lines[0].moves), 0)
-            self.assertEqual(book.lines[0].category.rec_name, 'Out-Category [2345]')
+            self.assertEqual(
+                book.lines[0].category.rec_name,
+                'Out-Category [2345]')
             self.assertEqual(book.lines[0].amount, Decimal('10.0'))
             self.assertEqual(book.lines[0].ena_tax1, True)
             self.assertEqual(book.lines[0].amount_tax1, Decimal('0.91'))
             self.assertEqual(book.lines[0].amount_net, Decimal('9.09'))
             self.assertEqual(len(book.lines[0].taxes), 1)
-            self.assertEqual(book.lines[0].taxes[0].rec_name, 'Tax Half usd0.91 usd9.09')
+            self.assertEqual(
+                book.lines[0].taxes[0].rec_name,
+                'Tax Half usd0.91 usd9.09')
 
             self.assertEqual(Move.search_count([]), 0)
             Line.wfcheck([book.lines[0]])
 
             moves = Move.search([])
             self.assertEqual(len(moves), 1)
             self.assertEqual(len(moves[0].lines), 3)
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(moves[0].state, 'draft')
             self.assertEqual(moves[0].date, date(2022, 5, 5))
             self.assertEqual(moves[0].description, 'buy something')
             self.assertEqual(moves[0].period.rec_name, '2022-05')
             self.assertEqual(moves[0].journal.rec_name, 'Cashbook')
-            self.assertEqual(moves[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].origin.rec_name,
                 '05/05/2022|Exp|-10.00 usd|buy something [Out-Category [2345]]')
 
             self.assertEqual(moves[0].lines[0].rec_name, '2234 - Tax Half')
             self.assertEqual(moves[0].lines[0].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[0].debit, Decimal('0.91'))
             self.assertEqual(moves[0].lines[0].amount_second_currency, None)
             self.assertEqual(moves[0].lines[0].origin, None)
             self.assertEqual(len(moves[0].lines[0].tax_lines), 1)
-            self.assertEqual(moves[0].lines[0].tax_lines[0].amount, Decimal('0.91'))
+            self.assertEqual(
+                moves[0].lines[0].tax_lines[0].amount,
+                Decimal('0.91'))
             self.assertEqual(moves[0].lines[0].tax_lines[0].type, 'tax')
-            self.assertEqual(moves[0].lines[0].tax_lines[0].tax.rec_name, 'Tax Half')
-
-            self.assertEqual(moves[0].lines[1].rec_name, '2345 - Account Category')
+            self.assertEqual(
+                moves[0].lines[0].tax_lines[0].tax.rec_name,
+                'Tax Half')
+
+            self.assertEqual(
+                moves[0].lines[1].rec_name,
+                '2345 - Account Category')
             self.assertEqual(moves[0].lines[1].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[1].debit, Decimal('9.09'))
             self.assertEqual(moves[0].lines[1].amount_second_currency, None)
             self.assertEqual(moves[0].lines[1].origin, None)
             self.assertEqual(len(moves[0].lines[1].tax_lines), 1)
-            self.assertEqual(moves[0].lines[1].tax_lines[0].amount, Decimal('9.09'))
+            self.assertEqual(
+                moves[0].lines[1].tax_lines[0].amount,
+                Decimal('9.09'))
             self.assertEqual(moves[0].lines[1].tax_lines[0].type, 'base')
-            self.assertEqual(moves[0].lines[1].tax_lines[0].tax.rec_name, 'Tax Half')
-
-            self.assertEqual(moves[0].lines[2].rec_name, '(0123 - Account Book)')
+            self.assertEqual(
+                moves[0].lines[1].tax_lines[0].tax.rec_name,
+                'Tax Half')
+
+            self.assertEqual(
+                moves[0].lines[2].rec_name,
+                '(0123 - Account Book)')
             self.assertEqual(moves[0].lines[2].credit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[2].debit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[2].amount_second_currency, None)
             self.assertEqual(moves[0].lines[1].origin, None)
             self.assertEqual(len(moves[0].lines[2].tax_lines), 0)
 
             # delete move
@@ -3418,34 +3629,32 @@
     def test_line_check_wf_out_split_booking_noparty(self):
         """ create cashbook + line, check booking out-type,
             company-currency
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
         Category = pool.get('cashbook.category')
         Account = pool.get('account.account')
         AccountType = pool.get('account.account.type')
         Journal = pool.get('account.journal')
         Move = pool.get('account.move')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         self.prep_accounting(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             acc_type, = AccountType.search([('name', '=', 'Cash')])
 
             accounts = Account.create([{
                 'name': 'Account Book',
                 'code': '0123',
                 'type': acc_type.id,
                 }, {
@@ -3493,60 +3702,72 @@
                             'description': 'line 2',
                             }])],
                     }])],
                 }])
             self.assertEqual(book.rec_name, 'Book 1 | -10.00 usd | Open')
             self.assertEqual(book.account.rec_name, '0123 - Account Book')
             self.assertEqual(len(book.lines), 1)
-            self.assertEqual(book.lines[0].rec_name,
+            self.assertEqual(
+                book.lines[0].rec_name,
                 '05/05/2022|Exp/Sp|-10.00 usd|buy something [-]')
             self.assertEqual(len(book.lines[0].moves), 0)
             self.assertEqual(book.lines[0].category, None)
             self.assertEqual(len(book.lines[0].splitlines), 2)
-            self.assertEqual(book.lines[0].splitlines[0].rec_name, \
+            self.assertEqual(
+                book.lines[0].splitlines[0].rec_name,
                 'Exp/Sp|5.00 usd|line 1 [Out-Category [2345]]')
-            self.assertEqual(book.lines[0].splitlines[1].rec_name, \
+            self.assertEqual(
+                book.lines[0].splitlines[1].rec_name,
                 'Exp/Sp|5.00 usd|line 2 [Out-Category [2345]]')
 
             self.assertEqual(Move.search_count([]), 0)
             Line.wfcheck([book.lines[0]])
 
             moves = Move.search([])
             self.assertEqual(len(moves), 1)
             self.assertEqual(len(moves[0].lines), 3)
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(moves[0].state, 'draft')
             self.assertEqual(moves[0].date, date(2022, 5, 5))
             self.assertEqual(moves[0].description, 'buy something')
             self.assertEqual(moves[0].period.rec_name, '2022-05')
             self.assertEqual(moves[0].journal.rec_name, 'Cashbook')
-            self.assertEqual(moves[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].origin.rec_name,
                 '05/05/2022|Exp/Sp|-10.00 usd|buy something [-]')
 
-            self.assertEqual(moves[0].lines[0].rec_name, '2345 - Account Category')
+            self.assertEqual(
+                moves[0].lines[0].rec_name,
+                '2345 - Account Category')
             self.assertEqual(moves[0].lines[0].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[0].debit, Decimal('5.0'))
             self.assertEqual(moves[0].lines[0].amount_second_currency, None)
             self.assertEqual(moves[0].lines[0].party, None)
             self.assertEqual(moves[0].lines[0].description, 'line 1')
             self.assertEqual(len(moves[0].lines[0].tax_lines), 0)
-            self.assertEqual(moves[0].lines[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[0].origin.rec_name,
                 'Exp/Sp|5.00 usd|line 1 [Out-Category [2345]]')
 
-            self.assertEqual(moves[0].lines[1].rec_name, '2345 - Account Category')
+            self.assertEqual(
+                moves[0].lines[1].rec_name,
+                '2345 - Account Category')
             self.assertEqual(moves[0].lines[1].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[1].debit, Decimal('5.0'))
             self.assertEqual(moves[0].lines[1].amount_second_currency, None)
             self.assertEqual(moves[0].lines[1].party, None)
             self.assertEqual(moves[0].lines[1].description, 'line 2')
             self.assertEqual(len(moves[0].lines[1].tax_lines), 0)
-            self.assertEqual(moves[0].lines[1].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[1].origin.rec_name,
                 'Exp/Sp|5.00 usd|line 2 [Out-Category [2345]]')
 
-            self.assertEqual(moves[0].lines[2].rec_name, '(0123 - Account Book)')
+            self.assertEqual(
+                moves[0].lines[2].rec_name,
+                '(0123 - Account Book)')
             self.assertEqual(moves[0].lines[2].credit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[2].debit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[2].amount_second_currency, None)
             self.assertEqual(moves[0].lines[2].party, None)
             self.assertEqual(moves[0].lines[2].description, None)
             self.assertEqual(len(moves[0].lines[2].tax_lines), 0)
             self.assertEqual(moves[0].lines[2].origin, None)
@@ -3569,35 +3790,33 @@
     def test_line_check_wf_out_booking_withparty(self):
         """ create cashbook + line, check booking out-type,
             company-currency
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
         Category = pool.get('cashbook.category')
         Account = pool.get('account.account')
         AccountType = pool.get('account.account.type')
         Journal = pool.get('account.journal')
         Move = pool.get('account.move')
         Reconciliation = pool.get('account.move.reconciliation')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         self.prep_accounting(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             acc_type, = AccountType.search([('name', '=', 'Cash')])
 
             accounts = Account.create([{
                 'name': 'Account Book',
                 'code': '0123',
                 'type': acc_type.id,
                 }, {
@@ -3637,45 +3856,53 @@
                         'amount': Decimal('10.0'),
                         'party': party.id,
                     }])],
                 }])
             self.assertEqual(book.rec_name, 'Book 1 | -10.00 usd | Open')
             self.assertEqual(book.account.rec_name, '0123 - Account Book')
             self.assertEqual(len(book.lines), 1)
-            self.assertEqual(book.lines[0].rec_name,
+            self.assertEqual(
+                book.lines[0].rec_name,
                 '05/05/2022|Exp|-10.00 usd|buy something [Out-Category [2345]]')
             self.assertEqual(len(book.lines[0].moves), 0)
-            self.assertEqual(book.lines[0].category.rec_name, 'Out-Category [2345]')
+            self.assertEqual(
+                book.lines[0].category.rec_name,
+                'Out-Category [2345]')
 
             self.assertEqual(Move.search_count([]), 0)
             Line.wfcheck([book.lines[0]])
 
             moves = Move.search([])
             self.assertEqual(len(moves), 1)
             self.assertEqual(len(moves[0].lines), 4)
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(moves[0].state, 'draft')
             self.assertEqual(moves[0].date, date(2022, 5, 5))
             self.assertEqual(moves[0].description, 'buy something')
             self.assertEqual(moves[0].period.rec_name, '2022-05')
             self.assertEqual(moves[0].journal.rec_name, 'Cashbook')
-            self.assertEqual(moves[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].origin.rec_name,
                 '05/05/2022|Exp|-10.00 usd|buy something [Out-Category [2345]]')
 
             self.assertEqual(moves[0].lines[0].rec_name, '(Main Payable)')
             self.assertEqual(moves[0].lines[0].credit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[0].debit, Decimal('00.0'))
             self.assertEqual(moves[0].lines[0].amount_second_currency, None)
 
-            self.assertEqual(moves[0].lines[1].rec_name, '2345 - Account Category')
+            self.assertEqual(
+                moves[0].lines[1].rec_name,
+                '2345 - Account Category')
             self.assertEqual(moves[0].lines[1].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[1].debit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[1].amount_second_currency, None)
 
-            self.assertEqual(moves[0].lines[2].rec_name, '(0123 - Account Book)')
+            self.assertEqual(
+                moves[0].lines[2].rec_name,
+                '(0123 - Account Book)')
             self.assertEqual(moves[0].lines[2].credit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[2].debit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[2].amount_second_currency, None)
 
             self.assertEqual(moves[0].lines[3].rec_name, 'Main Payable')
             self.assertEqual(moves[0].lines[3].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[3].debit, Decimal('10.0'))
@@ -3692,15 +3919,16 @@
 
             # post move
             Line.wfdone([book.lines[0]])
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(book.lines[0].moves[0].state, 'posted')
 
             rec_lines = Reconciliation.search([])
-            rec_move_ids = [x.id for x in book.lines[0].moves[0].lines if x.party]
+            rec_move_ids = [
+                x.id for x in book.lines[0].moves[0].lines if x.party]
             self.assertEqual(len(rec_move_ids), 2)
 
             self.assertEqual(len(rec_lines), 1)
             self.assertEqual(len(rec_lines[0].lines), 2)
 
             self.assertTrue(rec_lines[0].lines[0].id in rec_move_ids)
             self.assertTrue(rec_lines[0].lines[1].id in rec_move_ids)
@@ -3709,35 +3937,33 @@
     def test_line_check_wf_out_split_booking_withparty(self):
         """ create cashbook + line, check booking out-type,
             company-currency
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
         Category = pool.get('cashbook.category')
         Account = pool.get('account.account')
         AccountType = pool.get('account.account.type')
         Journal = pool.get('account.journal')
         Move = pool.get('account.move')
         Reconciliation = pool.get('account.move.reconciliation')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         self.prep_accounting(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             acc_type, = AccountType.search([('name', '=', 'Cash')])
 
             accounts = Account.create([{
                 'name': 'Account Book',
                 'code': '0123',
                 'type': acc_type.id,
                 }, {
@@ -3785,70 +4011,83 @@
                             'description': 'line 2',
                             }])],
                     }])],
                 }])
             self.assertEqual(book.rec_name, 'Book 1 | -10.00 usd | Open')
             self.assertEqual(book.account.rec_name, '0123 - Account Book')
             self.assertEqual(len(book.lines), 1)
-            self.assertEqual(book.lines[0].rec_name,
+            self.assertEqual(
+                book.lines[0].rec_name,
                 '05/05/2022|Exp/Sp|-10.00 usd|buy something [-]')
             self.assertEqual(len(book.lines[0].moves), 0)
             self.assertEqual(book.lines[0].category, None)
             self.assertEqual(len(book.lines[0].splitlines), 2)
-            self.assertEqual(book.lines[0].splitlines[0].rec_name, \
+            self.assertEqual(
+                book.lines[0].splitlines[0].rec_name,
                 'Exp/Sp|5.00 usd|line 1 [Out-Category [2345]]')
-            self.assertEqual(book.lines[0].splitlines[1].rec_name, \
+            self.assertEqual(
+                book.lines[0].splitlines[1].rec_name,
                 'Exp/Sp|5.00 usd|line 2 [Out-Category [2345]]')
 
             self.assertEqual(Move.search_count([]), 0)
             Line.wfcheck([book.lines[0]])
 
             moves = Move.search([])
             self.assertEqual(len(moves), 1)
             self.assertEqual(len(moves[0].lines), 5)
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(moves[0].state, 'draft')
             self.assertEqual(moves[0].date, date(2022, 5, 5))
             self.assertEqual(moves[0].description, 'buy something')
             self.assertEqual(moves[0].period.rec_name, '2022-05')
             self.assertEqual(moves[0].journal.rec_name, 'Cashbook')
-            self.assertEqual(moves[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].origin.rec_name,
                 '05/05/2022|Exp/Sp|-10.00 usd|buy something [-]')
 
             self.assertEqual(moves[0].lines[0].rec_name, '(Main Payable)')
             self.assertEqual(moves[0].lines[0].credit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[0].debit, Decimal('00.0'))
             self.assertEqual(moves[0].lines[0].amount_second_currency, None)
             self.assertEqual(moves[0].lines[0].party.rec_name, 'Party')
             self.assertEqual(moves[0].lines[0].description, None)
             self.assertEqual(len(moves[0].lines[0].tax_lines), 0)
-            self.assertEqual(moves[0].lines[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[0].origin.rec_name,
                 '05/05/2022|Exp/Sp|-10.00 usd|buy something [-]')
 
-            self.assertEqual(moves[0].lines[1].rec_name, '2345 - Account Category')
+            self.assertEqual(
+                moves[0].lines[1].rec_name,
+                '2345 - Account Category')
             self.assertEqual(moves[0].lines[1].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[1].debit, Decimal('5.0'))
             self.assertEqual(moves[0].lines[1].amount_second_currency, None)
             self.assertEqual(moves[0].lines[1].party, None)
             self.assertEqual(moves[0].lines[1].description, 'line 1')
             self.assertEqual(len(moves[0].lines[1].tax_lines), 0)
-            self.assertEqual(moves[0].lines[1].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[1].origin.rec_name,
                 'Exp/Sp|5.00 usd|line 1 [Out-Category [2345]]')
 
-            self.assertEqual(moves[0].lines[2].rec_name, '2345 - Account Category')
+            self.assertEqual(
+                moves[0].lines[2].rec_name,
+                '2345 - Account Category')
             self.assertEqual(moves[0].lines[2].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[2].debit, Decimal('5.0'))
             self.assertEqual(moves[0].lines[2].amount_second_currency, None)
             self.assertEqual(moves[0].lines[2].party, None)
             self.assertEqual(moves[0].lines[2].description, 'line 2')
             self.assertEqual(len(moves[0].lines[2].tax_lines), 0)
-            self.assertEqual(moves[0].lines[2].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[2].origin.rec_name,
                 'Exp/Sp|5.00 usd|line 2 [Out-Category [2345]]')
 
-            self.assertEqual(moves[0].lines[3].rec_name, '(0123 - Account Book)')
+            self.assertEqual(
+                moves[0].lines[3].rec_name,
+                '(0123 - Account Book)')
             self.assertEqual(moves[0].lines[3].credit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[3].debit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[3].amount_second_currency, None)
             self.assertEqual(moves[0].lines[3].party, None)
             self.assertEqual(moves[0].lines[3].description, None)
             self.assertEqual(len(moves[0].lines[3].tax_lines), 0)
             self.assertEqual(moves[0].lines[3].origin, None)
@@ -3856,15 +4095,16 @@
             self.assertEqual(moves[0].lines[4].rec_name, 'Main Payable')
             self.assertEqual(moves[0].lines[4].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[4].debit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[4].amount_second_currency, None)
             self.assertEqual(moves[0].lines[4].party.rec_name, 'Party')
             self.assertEqual(moves[0].lines[4].description, None)
             self.assertEqual(len(moves[0].lines[4].tax_lines), 0)
-            self.assertEqual(moves[0].lines[4].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[4].origin.rec_name,
                 '05/05/2022|Exp/Sp|-10.00 usd|buy something [-]')
 
             # delete move
             Line.wfedit([book.lines[0]])
             self.assertEqual(len(book.lines[0].moves), 0)
 
             # create move again
@@ -3874,15 +4114,16 @@
 
             # post move
             Line.wfdone([book.lines[0]])
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(book.lines[0].moves[0].state, 'posted')
 
             rec_lines = Reconciliation.search([])
-            rec_move_ids = [x.id for x in book.lines[0].moves[0].lines if x.party]
+            rec_move_ids = [
+                x.id for x in book.lines[0].moves[0].lines if x.party]
             self.assertEqual(len(rec_move_ids), 2)
 
             self.assertEqual(len(rec_lines), 1)
             self.assertEqual(len(rec_lines[0].lines), 2)
 
             self.assertTrue(rec_lines[0].lines[0].id in rec_move_ids)
             self.assertTrue(rec_lines[0].lines[1].id in rec_move_ids)
@@ -3891,35 +4132,33 @@
     def test_line_check_wf_out_split_booking_withparty_tax(self):
         """ create cashbook + line, check booking out-type,
             company-currency
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
         Category = pool.get('cashbook.category')
         Account = pool.get('account.account')
         AccountType = pool.get('account.account.type')
         Journal = pool.get('account.journal')
         Move = pool.get('account.move')
         Reconciliation = pool.get('account.move.reconciliation')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         self.prep_accounting(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             taxes = self.prep_line_taxes()
             acc_type, = AccountType.search([('name', '=', 'Cash')])
 
             accounts = Account.create([{
                 'name': 'Account Book',
                 'code': '0123',
                 'type': acc_type.id,
@@ -3976,131 +4215,167 @@
                             'ena_tax2': True,
                             }])],
                     }])],
                 }])
             self.assertEqual(book.rec_name, 'Book 1 | -10.00 usd | Open')
             self.assertEqual(book.account.rec_name, '0123 - Account Book')
             self.assertEqual(len(book.lines), 1)
-            self.assertEqual(book.lines[0].rec_name,
+            self.assertEqual(
+                book.lines[0].rec_name,
                 '05/05/2022|Exp/Sp|-10.00 usd|buy something [-]')
             self.assertEqual(len(book.lines[0].moves), 0)
             self.assertEqual(book.lines[0].category, None)
             self.assertEqual(len(book.lines[0].splitlines), 2)
-            self.assertEqual(book.lines[0].splitlines[0].rec_name, \
+            self.assertEqual(
+                book.lines[0].splitlines[0].rec_name,
                 'Exp/Sp|5.00 usd|line 1 [Out-Category [2345]]')
-            self.assertEqual(book.lines[0].splitlines[1].rec_name, \
+            self.assertEqual(
+                book.lines[0].splitlines[1].rec_name,
                 'Exp/Sp|5.00 usd|line 2 [Out-Category [2345]]')
 
             self.assertEqual(len(book.lines[0].taxes), 2)
-            self.assertEqual(book.lines[0].taxes[0].rec_name, 'Tax Full usd0.83 usd4.17')
+            self.assertEqual(
+                book.lines[0].taxes[0].rec_name,
+                'Tax Full usd0.83 usd4.17')
             self.assertEqual(book.lines[0].taxes[0].amount, Decimal('0.83'))
             self.assertEqual(book.lines[0].taxes[0].base, Decimal('4.17'))
             self.assertEqual(book.lines[0].taxes[0].tax.rec_name, 'Tax Full')
-            self.assertEqual(book.lines[0].taxes[0].splitline.rec_name,
+            self.assertEqual(
+                book.lines[0].taxes[0].splitline.rec_name,
                 'Exp/Sp|5.00 usd|line 2 [Out-Category [2345]]')
-            self.assertEqual(book.lines[0].taxes[1].rec_name, 'Tax Half usd0.46 usd4.54')
+            self.assertEqual(
+                book.lines[0].taxes[1].rec_name,
+                'Tax Half usd0.46 usd4.54')
             self.assertEqual(book.lines[0].taxes[1].amount, Decimal('0.46'))
             self.assertEqual(book.lines[0].taxes[1].base, Decimal('4.54'))
             self.assertEqual(book.lines[0].taxes[1].tax.rec_name, 'Tax Half')
-            self.assertEqual(book.lines[0].taxes[1].splitline.rec_name,
+            self.assertEqual(
+                book.lines[0].taxes[1].splitline.rec_name,
                 'Exp/Sp|5.00 usd|line 1 [Out-Category [2345]]')
 
             self.assertEqual(Move.search_count([]), 0)
             Line.wfcheck([book.lines[0]])
 
             moves = Move.search([])
             self.assertEqual(len(moves), 1)
             self.assertEqual(len(moves[0].lines), 7)
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(moves[0].state, 'draft')
             self.assertEqual(moves[0].date, date(2022, 5, 5))
             self.assertEqual(moves[0].description, 'buy something')
             self.assertEqual(moves[0].period.rec_name, '2022-05')
             self.assertEqual(moves[0].journal.rec_name, 'Cashbook')
-            self.assertEqual(moves[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].origin.rec_name,
                 '05/05/2022|Exp/Sp|-10.00 usd|buy something [-]')
 
             self.assertEqual(moves[0].lines[0].rec_name, '(Main Payable)')
             self.assertEqual(moves[0].lines[0].credit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[0].debit, Decimal('00.0'))
             self.assertEqual(moves[0].lines[0].amount_second_currency, None)
             self.assertEqual(moves[0].lines[0].party.rec_name, 'Party')
             self.assertEqual(moves[0].lines[0].description, None)
             self.assertEqual(len(moves[0].lines[0].tax_lines), 0)
-            self.assertEqual(moves[0].lines[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[0].origin.rec_name,
                 '05/05/2022|Exp/Sp|-10.00 usd|buy something [-]')
 
-            self.assertEqual(moves[0].lines[1].rec_name, '2345 - Account Category')
+            self.assertEqual(
+                moves[0].lines[1].rec_name,
+                '2345 - Account Category')
             self.assertEqual(moves[0].lines[1].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[1].debit, Decimal('4.54'))
             self.assertEqual(moves[0].lines[1].amount_second_currency, None)
             self.assertEqual(moves[0].lines[1].party, None)
             self.assertEqual(moves[0].lines[1].description, 'line 1')
-            self.assertEqual(moves[0].lines[1].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[1].origin.rec_name,
                 'Exp/Sp|5.00 usd|line 1 [Out-Category [2345]]')
             self.assertEqual(len(moves[0].lines[1].tax_lines), 1)
-            self.assertEqual(moves[0].lines[1].tax_lines[0].amount, Decimal('4.54'))
+            self.assertEqual(
+                moves[0].lines[1].tax_lines[0].amount,
+                Decimal('4.54'))
             self.assertEqual(moves[0].lines[1].tax_lines[0].type, 'base')
-            self.assertEqual(moves[0].lines[1].tax_lines[0].tax.rec_name, 'Tax Half')
+            self.assertEqual(
+                moves[0].lines[1].tax_lines[0].tax.rec_name,
+                'Tax Half')
 
             self.assertEqual(moves[0].lines[2].rec_name, '2234 - Tax Half')
             self.assertEqual(moves[0].lines[2].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[2].debit, Decimal('0.46'))
             self.assertEqual(moves[0].lines[2].amount_second_currency, None)
             self.assertEqual(moves[0].lines[2].party, None)
             self.assertEqual(moves[0].lines[2].description, 'line 1')
-            self.assertEqual(moves[0].lines[2].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[2].origin.rec_name,
                 'Exp/Sp|5.00 usd|line 1 [Out-Category [2345]]')
             self.assertEqual(len(moves[0].lines[2].tax_lines), 1)
-            self.assertEqual(moves[0].lines[2].tax_lines[0].amount, Decimal('0.46'))
+            self.assertEqual(
+                moves[0].lines[2].tax_lines[0].amount,
+                Decimal('0.46'))
             self.assertEqual(moves[0].lines[2].tax_lines[0].type, 'tax')
-            self.assertEqual(moves[0].lines[2].tax_lines[0].tax.rec_name, 'Tax Half')
-
-            self.assertEqual(moves[0].lines[3].rec_name, '2345 - Account Category')
+            self.assertEqual(
+                moves[0].lines[2].tax_lines[0].tax.rec_name,
+                'Tax Half')
+
+            self.assertEqual(
+                moves[0].lines[3].rec_name,
+                '2345 - Account Category')
             self.assertEqual(moves[0].lines[3].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[3].debit, Decimal('4.17'))
             self.assertEqual(moves[0].lines[3].amount_second_currency, None)
             self.assertEqual(moves[0].lines[3].party, None)
             self.assertEqual(moves[0].lines[3].description, 'line 2')
-            self.assertEqual(moves[0].lines[3].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[3].origin.rec_name,
                 'Exp/Sp|5.00 usd|line 2 [Out-Category [2345]]')
             self.assertEqual(len(moves[0].lines[3].tax_lines), 1)
-            self.assertEqual(moves[0].lines[3].tax_lines[0].amount, Decimal('4.17'))
+            self.assertEqual(
+                moves[0].lines[3].tax_lines[0].amount,
+                Decimal('4.17'))
             self.assertEqual(moves[0].lines[3].tax_lines[0].type, 'base')
-            self.assertEqual(moves[0].lines[3].tax_lines[0].tax.rec_name, 'Tax Full')
+            self.assertEqual(
+                moves[0].lines[3].tax_lines[0].tax.rec_name,
+                'Tax Full')
 
             self.assertEqual(moves[0].lines[4].rec_name, '2235 - Tax Full')
             self.assertEqual(moves[0].lines[4].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[4].debit, Decimal('0.83'))
             self.assertEqual(moves[0].lines[4].amount_second_currency, None)
             self.assertEqual(moves[0].lines[4].party, None)
             self.assertEqual(moves[0].lines[4].description, 'line 2')
-            self.assertEqual(moves[0].lines[4].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[4].origin.rec_name,
                 'Exp/Sp|5.00 usd|line 2 [Out-Category [2345]]')
             self.assertEqual(len(moves[0].lines[4].tax_lines), 1)
-            self.assertEqual(moves[0].lines[4].tax_lines[0].amount, Decimal('0.83'))
+            self.assertEqual(
+                moves[0].lines[4].tax_lines[0].amount,
+                Decimal('0.83'))
             self.assertEqual(moves[0].lines[4].tax_lines[0].type, 'tax')
-            self.assertEqual(moves[0].lines[4].tax_lines[0].tax.rec_name, 'Tax Full')
+            self.assertEqual(
+                moves[0].lines[4].tax_lines[0].tax.rec_name, 'Tax Full')
 
-            self.assertEqual(moves[0].lines[5].rec_name, '(0123 - Account Book)')
+            self.assertEqual(
+                moves[0].lines[5].rec_name, '(0123 - Account Book)')
             self.assertEqual(moves[0].lines[5].credit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[5].debit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[5].amount_second_currency, None)
             self.assertEqual(moves[0].lines[5].party, None)
             self.assertEqual(moves[0].lines[5].description, None)
             self.assertEqual(moves[0].lines[5].origin, None)
             self.assertEqual(len(moves[0].lines[5].tax_lines), 0)
 
             self.assertEqual(moves[0].lines[6].rec_name, 'Main Payable')
             self.assertEqual(moves[0].lines[6].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[6].debit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[6].amount_second_currency, None)
             self.assertEqual(moves[0].lines[6].party.rec_name, 'Party')
             self.assertEqual(moves[0].lines[6].description, None)
-            self.assertEqual(moves[0].lines[6].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[6].origin.rec_name,
                 '05/05/2022|Exp/Sp|-10.00 usd|buy something [-]')
             self.assertEqual(len(moves[0].lines[6].tax_lines), 0)
 
             # delete move
             Line.wfedit([book.lines[0]])
             self.assertEqual(len(book.lines[0].moves), 0)
 
@@ -4111,15 +4386,16 @@
 
             # post move
             Line.wfdone([book.lines[0]])
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(book.lines[0].moves[0].state, 'posted')
 
             rec_lines = Reconciliation.search([])
-            rec_move_ids = [x.id for x in book.lines[0].moves[0].lines if x.party]
+            rec_move_ids = [
+                x.id for x in book.lines[0].moves[0].lines if x.party]
             self.assertEqual(len(rec_move_ids), 2)
 
             self.assertEqual(len(rec_lines), 1)
             self.assertEqual(len(rec_lines[0].lines), 2)
 
             self.assertTrue(rec_lines[0].lines[0].id in rec_move_ids)
             self.assertTrue(rec_lines[0].lines[1].id in rec_move_ids)
@@ -4128,35 +4404,33 @@
     def test_line_check_wf_out_booking_2nd_currency_noparty(self):
         """ create cashbook + line, check booking out-type,
             2nd-currency
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
         Category = pool.get('cashbook.category')
         Account = pool.get('account.account')
         AccountType = pool.get('account.account.type')
         Journal = pool.get('account.journal')
         Move = pool.get('account.move')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         self.prep_accounting(company)
         (usd, euro) = self.prep_2nd_currency(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             acc_type, = AccountType.search([('name', '=', 'Cash')])
 
             accounts = Account.create([{
                 'name': 'Account Book',
                 'code': '0123',
                 'type': acc_type.id,
                 }, {
@@ -4197,42 +4471,54 @@
                         'party': party.id,
                     }])],
                 }])
             self.assertEqual(book.rec_name, 'Book 1 | -10.00 usd | Open')
             self.assertEqual(book.account.rec_name, '0123 - Account Book')
             self.assertEqual(book.currency.code, 'usd')
             self.assertEqual(len(book.lines), 1)
-            self.assertEqual(book.lines[0].rec_name,
+            self.assertEqual(
+                book.lines[0].rec_name,
                 '05/05/2022|Exp|-10.00 usd|buy something [Out-Category [2345]]')
             self.assertEqual(len(book.lines[0].moves), 0)
-            self.assertEqual(book.lines[0].category.rec_name, 'Out-Category [2345]')
+            self.assertEqual(
+                book.lines[0].category.rec_name,
+                'Out-Category [2345]')
 
             self.assertEqual(Move.search_count([]), 0)
             Line.wfcheck([book.lines[0]])
 
             moves = Move.search([])
             self.assertEqual(len(moves), 1)
             self.assertEqual(len(moves[0].lines), 2)
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(moves[0].state, 'draft')
             self.assertEqual(moves[0].date, date(2022, 5, 5))
             self.assertEqual(moves[0].description, 'buy something')
             self.assertEqual(moves[0].period.rec_name, '2022-05')
             self.assertEqual(moves[0].journal.rec_name, 'Cashbook')
-            self.assertEqual(moves[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].origin.rec_name,
                 '05/05/2022|Exp|-10.00 usd|buy something [Out-Category [2345]]')
-            self.assertEqual(moves[0].lines[0].rec_name, '2345 - Account Category')
+            self.assertEqual(
+                moves[0].lines[0].rec_name,
+                '2345 - Account Category')
             self.assertEqual(moves[0].lines[0].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[0].debit, Decimal('9.52'))
-            self.assertEqual(moves[0].lines[0].amount_second_currency, Decimal('10.0'))
+            self.assertEqual(
+                moves[0].lines[0].amount_second_currency,
+                Decimal('10.0'))
             self.assertEqual(moves[0].lines[0].second_currency.rec_name, 'usd')
-            self.assertEqual(moves[0].lines[1].rec_name, '(0123 - Account Book)')
+            self.assertEqual(
+                moves[0].lines[1].rec_name,
+                '(0123 - Account Book)')
             self.assertEqual(moves[0].lines[1].credit, Decimal('9.52'))
             self.assertEqual(moves[0].lines[1].debit, Decimal('0.0'))
-            self.assertEqual(moves[0].lines[1].amount_second_currency, Decimal('-10.0'))
+            self.assertEqual(
+                moves[0].lines[1].amount_second_currency,
+                Decimal('-10.0'))
             self.assertEqual(moves[0].lines[1].second_currency.rec_name, 'usd')
 
             # delete move
             Line.wfedit([book.lines[0]])
             self.assertEqual(len(book.lines[0].moves), 0)
 
             # create move again
@@ -4249,35 +4535,33 @@
     def test_line_check_wf_out_booking_2nd_currency_noparty_tax(self):
         """ create cashbook + line, check booking out-type,
             2nd-currency, with tax
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
         Category = pool.get('cashbook.category')
         Account = pool.get('account.account')
         AccountType = pool.get('account.account.type')
         Journal = pool.get('account.journal')
         Move = pool.get('account.move')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         self.prep_accounting(company)
         (usd, euro) = self.prep_2nd_currency(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             taxes = self.prep_line_taxes()
             acc_type, = AccountType.search([('name', '=', 'Cash')])
 
             accounts = Account.create([{
                 'name': 'Account Book',
                 'code': '0123',
                 'type': acc_type.id,
@@ -4326,20 +4610,25 @@
                         'ena_tax1': True
                     }])],
                 }])
             self.assertEqual(book.rec_name, 'Book 1 | -10.00 usd | Open')
             self.assertEqual(book.account.rec_name, '0123 - Account Book')
             self.assertEqual(book.currency.code, 'usd')
             self.assertEqual(len(book.lines), 1)
-            self.assertEqual(book.lines[0].rec_name,
+            self.assertEqual(
+                book.lines[0].rec_name,
                 '05/05/2022|Exp|-10.00 usd|buy something [Out-Category [2345]]')
             self.assertEqual(len(book.lines[0].moves), 0)
-            self.assertEqual(book.lines[0].category.rec_name, 'Out-Category [2345]')
+            self.assertEqual(
+                book.lines[0].category.rec_name,
+                'Out-Category [2345]')
             self.assertEqual(len(book.lines[0].taxes), 1)
-            self.assertEqual(book.lines[0].taxes[0].rec_name, 'Tax Half usd0.91 usd9.09')
+            self.assertEqual(
+                book.lines[0].taxes[0].rec_name,
+                'Tax Half usd0.91 usd9.09')
             self.assertEqual(book.lines[0].amount, Decimal('10.0'))
             self.assertEqual(book.lines[0].ena_tax1, True)
             self.assertEqual(book.lines[0].amount_tax1, Decimal('0.91'))
             self.assertEqual(book.lines[0].amount_net, Decimal('9.09'))
 
             self.assertEqual(Move.search_count([]), 0)
             Line.wfcheck([book.lines[0]])
@@ -4349,41 +4638,60 @@
             self.assertEqual(len(moves[0].lines), 3)
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(moves[0].state, 'draft')
             self.assertEqual(moves[0].date, date(2022, 5, 5))
             self.assertEqual(moves[0].description, 'buy something')
             self.assertEqual(moves[0].period.rec_name, '2022-05')
             self.assertEqual(moves[0].journal.rec_name, 'Cashbook')
-            self.assertEqual(moves[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].origin.rec_name,
                 '05/05/2022|Exp|-10.00 usd|buy something [Out-Category [2345]]')
 
             self.assertEqual(moves[0].lines[0].rec_name, '2234 - Tax Half')
             self.assertEqual(moves[0].lines[0].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[0].debit, Decimal('0.86'))
-            self.assertEqual(moves[0].lines[0].amount_second_currency, Decimal('0.91'))
+            self.assertEqual(
+                moves[0].lines[0].amount_second_currency,
+                Decimal('0.91'))
             self.assertEqual(moves[0].lines[0].second_currency.rec_name, 'usd')
             self.assertEqual(len(moves[0].lines[0].tax_lines), 1)
-            self.assertEqual(moves[0].lines[0].tax_lines[0].amount, Decimal('0.86'))
+            self.assertEqual(
+                moves[0].lines[0].tax_lines[0].amount,
+                Decimal('0.86'))
             self.assertEqual(moves[0].lines[0].tax_lines[0].type, 'tax')
-            self.assertEqual(moves[0].lines[0].tax_lines[0].tax.rec_name, 'Tax Half')
-
-            self.assertEqual(moves[0].lines[1].rec_name, '2345 - Account Category')
+            self.assertEqual(
+                moves[0].lines[0].tax_lines[0].tax.rec_name,
+                'Tax Half')
+
+            self.assertEqual(
+                moves[0].lines[1].rec_name,
+                '2345 - Account Category')
             self.assertEqual(moves[0].lines[1].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[1].debit, Decimal('8.66'))
-            self.assertEqual(moves[0].lines[1].amount_second_currency, Decimal('9.09'))
+            self.assertEqual(
+                moves[0].lines[1].amount_second_currency,
+                Decimal('9.09'))
             self.assertEqual(moves[0].lines[1].second_currency.rec_name, 'usd')
             self.assertEqual(len(moves[0].lines[1].tax_lines), 1)
-            self.assertEqual(moves[0].lines[1].tax_lines[0].amount, Decimal('8.66'))
+            self.assertEqual(
+                moves[0].lines[1].tax_lines[0].amount,
+                Decimal('8.66'))
             self.assertEqual(moves[0].lines[1].tax_lines[0].type, 'base')
-            self.assertEqual(moves[0].lines[1].tax_lines[0].tax.rec_name, 'Tax Half')
-
-            self.assertEqual(moves[0].lines[2].rec_name, '(0123 - Account Book)')
+            self.assertEqual(
+                moves[0].lines[1].tax_lines[0].tax.rec_name,
+                'Tax Half')
+
+            self.assertEqual(
+                moves[0].lines[2].rec_name,
+                '(0123 - Account Book)')
             self.assertEqual(moves[0].lines[2].credit, Decimal('9.52'))
             self.assertEqual(moves[0].lines[2].debit, Decimal('0.0'))
-            self.assertEqual(moves[0].lines[2].amount_second_currency, Decimal('-10.0'))
+            self.assertEqual(
+                moves[0].lines[2].amount_second_currency,
+                Decimal('-10.0'))
             self.assertEqual(moves[0].lines[2].second_currency.rec_name, 'usd')
             self.assertEqual(len(moves[0].lines[2].tax_lines), 0)
 
             # delete move
             Line.wfedit([book.lines[0]])
             self.assertEqual(len(book.lines[0].moves), 0)
 
@@ -4401,35 +4709,33 @@
     def test_line_check_wf_out_split_booking_2nd_currency_noparty(self):
         """ create cashbook + line, check booking out-type,
             2nd-currency
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
         Category = pool.get('cashbook.category')
         Account = pool.get('account.account')
         AccountType = pool.get('account.account.type')
         Journal = pool.get('account.journal')
         Move = pool.get('account.move')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         self.prep_accounting(company)
         (usd, euro) = self.prep_2nd_currency(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             acc_type, = AccountType.search([('name', '=', 'Cash')])
 
             accounts = Account.create([{
                 'name': 'Account Book',
                 'code': '0123',
                 'type': acc_type.id,
                 }, {
@@ -4478,65 +4784,83 @@
                             }])],
                     }])],
                 }])
             self.assertEqual(book.rec_name, 'Book 1 | -10.00 usd | Open')
             self.assertEqual(book.account.rec_name, '0123 - Account Book')
             self.assertEqual(book.currency.code, 'usd')
             self.assertEqual(len(book.lines), 1)
-            self.assertEqual(book.lines[0].rec_name,
+            self.assertEqual(
+                book.lines[0].rec_name,
                 '05/05/2022|Exp/Sp|-10.00 usd|buy something [-]')
             self.assertEqual(len(book.lines[0].moves), 0)
             self.assertEqual(book.lines[0].category, None)
             self.assertEqual(len(book.lines[0].splitlines), 2)
-            self.assertEqual(book.lines[0].splitlines[0].rec_name, \
+            self.assertEqual(
+                book.lines[0].splitlines[0].rec_name,
                 'Exp/Sp|5.00 usd|line 1 [Out-Category [2345]]')
-            self.assertEqual(book.lines[0].splitlines[1].rec_name, \
+            self.assertEqual(
+                book.lines[0].splitlines[1].rec_name,
                 'Exp/Sp|5.00 usd|line 2 [Out-Category [2345]]')
 
             self.assertEqual(Move.search_count([]), 0)
             Line.wfcheck([book.lines[0]])
 
             moves = Move.search([])
             self.assertEqual(len(moves), 1)
             self.assertEqual(len(moves[0].lines), 3)
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(moves[0].state, 'draft')
             self.assertEqual(moves[0].date, date(2022, 5, 5))
             self.assertEqual(moves[0].description, 'buy something')
             self.assertEqual(moves[0].period.rec_name, '2022-05')
             self.assertEqual(moves[0].journal.rec_name, 'Cashbook')
-            self.assertEqual(moves[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].origin.rec_name,
                 '05/05/2022|Exp/Sp|-10.00 usd|buy something [-]')
 
-            self.assertEqual(moves[0].lines[0].rec_name, '2345 - Account Category')
+            self.assertEqual(
+                moves[0].lines[0].rec_name,
+                '2345 - Account Category')
             self.assertEqual(moves[0].lines[0].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[0].debit, Decimal('4.76'))
-            self.assertEqual(moves[0].lines[0].amount_second_currency, Decimal('5.0'))
+            self.assertEqual(
+                moves[0].lines[0].amount_second_currency,
+                Decimal('5.0'))
             self.assertEqual(moves[0].lines[0].second_currency.rec_name, 'usd')
             self.assertEqual(moves[0].lines[0].party, None)
             self.assertEqual(moves[0].lines[0].description, 'line 1')
-            self.assertEqual(moves[0].lines[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[0].origin.rec_name,
                 'Exp/Sp|5.00 usd|line 1 [Out-Category [2345]]')
             self.assertEqual(len(moves[0].lines[0].tax_lines), 0)
 
-            self.assertEqual(moves[0].lines[1].rec_name, '2345 - Account Category')
+            self.assertEqual(
+                moves[0].lines[1].rec_name,
+                '2345 - Account Category')
             self.assertEqual(moves[0].lines[1].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[1].debit, Decimal('4.76'))
-            self.assertEqual(moves[0].lines[1].amount_second_currency, Decimal('5.0'))
+            self.assertEqual(
+                moves[0].lines[1].amount_second_currency,
+                Decimal('5.0'))
             self.assertEqual(moves[0].lines[1].second_currency.rec_name, 'usd')
             self.assertEqual(moves[0].lines[1].party, None)
             self.assertEqual(moves[0].lines[1].description, 'line 2')
-            self.assertEqual(moves[0].lines[1].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[1].origin.rec_name,
                 'Exp/Sp|5.00 usd|line 2 [Out-Category [2345]]')
             self.assertEqual(len(moves[0].lines[1].tax_lines), 0)
 
-            self.assertEqual(moves[0].lines[2].rec_name, '(0123 - Account Book)')
+            self.assertEqual(
+                moves[0].lines[2].rec_name,
+                '(0123 - Account Book)')
             self.assertEqual(moves[0].lines[2].credit, Decimal('9.52'))
             self.assertEqual(moves[0].lines[2].debit, Decimal('0.0'))
-            self.assertEqual(moves[0].lines[2].amount_second_currency, Decimal('-10.0'))
+            self.assertEqual(
+                moves[0].lines[2].amount_second_currency,
+                Decimal('-10.0'))
             self.assertEqual(moves[0].lines[2].second_currency.rec_name, 'usd')
             self.assertEqual(moves[0].lines[2].party, None)
             self.assertEqual(moves[0].lines[2].description, None)
             self.assertEqual(moves[0].lines[2].origin, None)
             self.assertEqual(len(moves[0].lines[2].tax_lines), 0)
 
             # delete move
@@ -4557,36 +4881,34 @@
     def test_line_check_wf_out_booking_2nd_currency_withparty(self):
         """ create cashbook + line, check booking out-type,
             2nd-currency
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
         Category = pool.get('cashbook.category')
         Account = pool.get('account.account')
         AccountType = pool.get('account.account.type')
         Journal = pool.get('account.journal')
         Move = pool.get('account.move')
         Reconciliation = pool.get('account.move.reconciliation')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         self.prep_accounting(company)
         (usd, euro) = self.prep_2nd_currency(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             acc_type, = AccountType.search([('name', '=', 'Cash')])
 
             accounts = Account.create([{
                 'name': 'Account Book',
                 'code': '0123',
                 'type': acc_type.id,
                 }, {
@@ -4627,56 +4949,72 @@
                         'party': party.id,
                     }])],
                 }])
             self.assertEqual(book.rec_name, 'Book 1 | -10.00 usd | Open')
             self.assertEqual(book.account.rec_name, '0123 - Account Book')
             self.assertEqual(book.currency.code, 'usd')
             self.assertEqual(len(book.lines), 1)
-            self.assertEqual(book.lines[0].rec_name,
+            self.assertEqual(
+                book.lines[0].rec_name,
                 '05/05/2022|Exp|-10.00 usd|buy something [Out-Category [2345]]')
             self.assertEqual(len(book.lines[0].moves), 0)
-            self.assertEqual(book.lines[0].category.rec_name, 'Out-Category [2345]')
+            self.assertEqual(
+                book.lines[0].category.rec_name,
+                'Out-Category [2345]')
 
             self.assertEqual(Move.search_count([]), 0)
             Line.wfcheck([book.lines[0]])
 
             moves = Move.search([])
             self.assertEqual(len(moves), 1)
             self.assertEqual(len(moves[0].lines), 4)
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(moves[0].state, 'draft')
             self.assertEqual(moves[0].date, date(2022, 5, 5))
             self.assertEqual(moves[0].description, 'buy something')
             self.assertEqual(moves[0].period.rec_name, '2022-05')
             self.assertEqual(moves[0].journal.rec_name, 'Cashbook')
-            self.assertEqual(moves[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].origin.rec_name,
                 '05/05/2022|Exp|-10.00 usd|buy something [Out-Category [2345]]')
 
             self.assertEqual(moves[0].lines[0].rec_name, '(Main Payable)')
             self.assertEqual(moves[0].lines[0].credit, Decimal('9.52'))
             self.assertEqual(moves[0].lines[0].debit, Decimal('0.0'))
-            self.assertEqual(moves[0].lines[0].amount_second_currency, Decimal('-10.0'))
+            self.assertEqual(
+                moves[0].lines[0].amount_second_currency,
+                Decimal('-10.0'))
             self.assertEqual(moves[0].lines[0].second_currency.rec_name, 'usd')
 
-            self.assertEqual(moves[0].lines[1].rec_name, '2345 - Account Category')
+            self.assertEqual(
+                moves[0].lines[1].rec_name,
+                '2345 - Account Category')
             self.assertEqual(moves[0].lines[1].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[1].debit, Decimal('9.52'))
-            self.assertEqual(moves[0].lines[1].amount_second_currency, Decimal('10.0'))
+            self.assertEqual(
+                moves[0].lines[1].amount_second_currency,
+                Decimal('10.0'))
             self.assertEqual(moves[0].lines[1].second_currency.rec_name, 'usd')
 
-            self.assertEqual(moves[0].lines[2].rec_name, '(0123 - Account Book)')
+            self.assertEqual(
+                moves[0].lines[2].rec_name,
+                '(0123 - Account Book)')
             self.assertEqual(moves[0].lines[2].credit, Decimal('9.52'))
             self.assertEqual(moves[0].lines[2].debit, Decimal('0.0'))
-            self.assertEqual(moves[0].lines[2].amount_second_currency, Decimal('-10.0'))
+            self.assertEqual(
+                moves[0].lines[2].amount_second_currency,
+                Decimal('-10.0'))
             self.assertEqual(moves[0].lines[2].second_currency.rec_name, 'usd')
 
             self.assertEqual(moves[0].lines[3].rec_name, 'Main Payable')
             self.assertEqual(moves[0].lines[3].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[3].debit, Decimal('9.52'))
-            self.assertEqual(moves[0].lines[3].amount_second_currency, Decimal('10.0'))
+            self.assertEqual(
+                moves[0].lines[3].amount_second_currency,
+                Decimal('10.0'))
             self.assertEqual(moves[0].lines[3].second_currency.rec_name, 'usd')
 
             # delete move
             Line.wfedit([book.lines[0]])
             self.assertEqual(len(book.lines[0].moves), 0)
 
             # create move again
@@ -4686,15 +5024,16 @@
 
             # post move
             Line.wfdone([book.lines[0]])
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(book.lines[0].moves[0].state, 'posted')
 
             rec_lines = Reconciliation.search([])
-            rec_move_ids = [x.id for x in book.lines[0].moves[0].lines if x.party]
+            rec_move_ids = [
+                x.id for x in book.lines[0].moves[0].lines if x.party]
             self.assertEqual(len(rec_move_ids), 2)
 
             self.assertEqual(len(rec_lines), 1)
             self.assertEqual(len(rec_lines[0].lines), 2)
 
             self.assertTrue(rec_lines[0].lines[0].id in rec_move_ids)
             self.assertTrue(rec_lines[0].lines[1].id in rec_move_ids)
@@ -4703,36 +5042,34 @@
     def test_line_check_wf_out_split_booking_2nd_currency_withparty(self):
         """ create cashbook + line, check booking out-type,
             2nd-currency
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
         Category = pool.get('cashbook.category')
         Account = pool.get('account.account')
         AccountType = pool.get('account.account.type')
         Journal = pool.get('account.journal')
         Move = pool.get('account.move')
         Reconciliation = pool.get('account.move.reconciliation')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         self.prep_accounting(company)
         (usd, euro) = self.prep_2nd_currency(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             acc_type, = AccountType.search([('name', '=', 'Cash')])
 
             accounts = Account.create([{
                 'name': 'Account Book',
                 'code': '0123',
                 'type': acc_type.id,
                 }, {
@@ -4781,90 +5118,110 @@
                             }])],
                     }])],
                 }])
             self.assertEqual(book.rec_name, 'Book 1 | -10.00 usd | Open')
             self.assertEqual(book.account.rec_name, '0123 - Account Book')
             self.assertEqual(book.currency.code, 'usd')
             self.assertEqual(len(book.lines), 1)
-            self.assertEqual(book.lines[0].rec_name,
+            self.assertEqual(
+                book.lines[0].rec_name,
                 '05/05/2022|Exp/Sp|-10.00 usd|buy something [-]')
             self.assertEqual(len(book.lines[0].moves), 0)
             self.assertEqual(book.lines[0].category, None)
             self.assertEqual(len(book.lines[0].splitlines), 2)
-            self.assertEqual(book.lines[0].splitlines[0].rec_name, \
+            self.assertEqual(
+                book.lines[0].splitlines[0].rec_name,
                 'Exp/Sp|5.00 usd|line 1 [Out-Category [2345]]')
-            self.assertEqual(book.lines[0].splitlines[1].rec_name, \
+            self.assertEqual(
+                book.lines[0].splitlines[1].rec_name,
                 'Exp/Sp|5.00 usd|line 2 [Out-Category [2345]]')
 
             self.assertEqual(Move.search_count([]), 0)
             Line.wfcheck([book.lines[0]])
 
             moves = Move.search([])
             self.assertEqual(len(moves), 1)
             self.assertEqual(len(moves[0].lines), 5)
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(moves[0].state, 'draft')
             self.assertEqual(moves[0].date, date(2022, 5, 5))
             self.assertEqual(moves[0].description, 'buy something')
             self.assertEqual(moves[0].period.rec_name, '2022-05')
             self.assertEqual(moves[0].journal.rec_name, 'Cashbook')
-            self.assertEqual(moves[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].origin.rec_name,
                 '05/05/2022|Exp/Sp|-10.00 usd|buy something [-]')
 
             self.assertEqual(moves[0].lines[0].rec_name, '(Main Payable)')
             self.assertEqual(moves[0].lines[0].credit, Decimal('9.52'))
             self.assertEqual(moves[0].lines[0].debit, Decimal('0.0'))
-            self.assertEqual(moves[0].lines[0].amount_second_currency, Decimal('-10.0'))
+            self.assertEqual(
+                moves[0].lines[0].amount_second_currency,
+                Decimal('-10.0'))
             self.assertEqual(moves[0].lines[0].second_currency.rec_name, 'usd')
             self.assertEqual(moves[0].lines[0].party.rec_name, 'Party')
             self.assertEqual(moves[0].lines[0].description, None)
-            self.assertEqual(moves[0].lines[0].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[0].origin.rec_name,
                 '05/05/2022|Exp/Sp|-10.00 usd|buy something [-]')
             self.assertEqual(len(moves[0].lines[0].tax_lines), 0)
 
-            self.assertEqual(moves[0].lines[1].rec_name, '2345 - Account Category')
+            self.assertEqual(
+                moves[0].lines[1].rec_name,
+                '2345 - Account Category')
             self.assertEqual(moves[0].lines[1].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[1].debit, Decimal('4.76'))
-            self.assertEqual(moves[0].lines[1].amount_second_currency, Decimal('5.0'))
+            self.assertEqual(
+                moves[0].lines[1].amount_second_currency,
+                Decimal('5.0'))
             self.assertEqual(moves[0].lines[1].second_currency.rec_name, 'usd')
             self.assertEqual(moves[0].lines[1].party, None)
             self.assertEqual(moves[0].lines[1].description, 'line 1')
-            self.assertEqual(moves[0].lines[1].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[1].origin.rec_name,
                 'Exp/Sp|5.00 usd|line 1 [Out-Category [2345]]')
             self.assertEqual(len(moves[0].lines[1].tax_lines), 0)
 
-            self.assertEqual(moves[0].lines[2].rec_name, '2345 - Account Category')
+            self.assertEqual(
+                moves[0].lines[2].rec_name, '2345 - Account Category')
             self.assertEqual(moves[0].lines[2].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[2].debit, Decimal('4.76'))
-            self.assertEqual(moves[0].lines[2].amount_second_currency, Decimal('5.0'))
+            self.assertEqual(
+                moves[0].lines[2].amount_second_currency, Decimal('5.0'))
             self.assertEqual(moves[0].lines[2].second_currency.rec_name, 'usd')
             self.assertEqual(moves[0].lines[2].party, None)
             self.assertEqual(moves[0].lines[2].description, 'line 2')
-            self.assertEqual(moves[0].lines[2].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[2].origin.rec_name,
                 'Exp/Sp|5.00 usd|line 2 [Out-Category [2345]]')
             self.assertEqual(len(moves[0].lines[2].tax_lines), 0)
 
-            self.assertEqual(moves[0].lines[3].rec_name, '(0123 - Account Book)')
+            self.assertEqual(
+                moves[0].lines[3].rec_name, '(0123 - Account Book)')
             self.assertEqual(moves[0].lines[3].credit, Decimal('9.52'))
             self.assertEqual(moves[0].lines[3].debit, Decimal('0.0'))
-            self.assertEqual(moves[0].lines[3].amount_second_currency, Decimal('-10.0'))
+            self.assertEqual(
+                moves[0].lines[3].amount_second_currency,
+                Decimal('-10.0'))
             self.assertEqual(moves[0].lines[3].second_currency.rec_name, 'usd')
             self.assertEqual(moves[0].lines[3].party, None)
             self.assertEqual(moves[0].lines[3].description, None)
             self.assertEqual(moves[0].lines[3].origin, None)
             self.assertEqual(len(moves[0].lines[3].tax_lines), 0)
 
             self.assertEqual(moves[0].lines[4].rec_name, 'Main Payable')
             self.assertEqual(moves[0].lines[4].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[4].debit, Decimal('9.52'))
-            self.assertEqual(moves[0].lines[4].amount_second_currency, Decimal('10.0'))
+            self.assertEqual(
+                moves[0].lines[4].amount_second_currency, Decimal('10.0'))
             self.assertEqual(moves[0].lines[4].second_currency.rec_name, 'usd')
             self.assertEqual(moves[0].lines[4].party.rec_name, 'Party')
             self.assertEqual(moves[0].lines[4].description, None)
-            self.assertEqual(moves[0].lines[4].origin.rec_name,
+            self.assertEqual(
+                moves[0].lines[4].origin.rec_name,
                 '05/05/2022|Exp/Sp|-10.00 usd|buy something [-]')
             self.assertEqual(len(moves[0].lines[4].tax_lines), 0)
 
             # delete move
             Line.wfedit([book.lines[0]])
             self.assertEqual(len(book.lines[0].moves), 0)
 
@@ -4875,15 +5232,16 @@
 
             # post move
             Line.wfdone([book.lines[0]])
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(book.lines[0].moves[0].state, 'posted')
 
             rec_lines = Reconciliation.search([])
-            rec_move_ids = [x.id for x in book.lines[0].moves[0].lines if x.party]
+            rec_move_ids = [
+                x.id for x in book.lines[0].moves[0].lines if x.party]
             self.assertEqual(len(rec_move_ids), 2)
 
             self.assertEqual(len(rec_lines), 1)
             self.assertEqual(len(rec_lines[0].lines), 2)
 
             self.assertTrue(rec_lines[0].lines[0].id in rec_move_ids)
             self.assertTrue(rec_lines[0].lines[1].id in rec_move_ids)
@@ -4892,33 +5250,31 @@
     def test_line_check_wf_in_transfer(self):
         """ create cashbook + line, transfer: bank -> cash
             same currrency in both accounts
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
         Account = pool.get('account.account')
         AccountType = pool.get('account.account.type')
         Journal = pool.get('account.journal')
         Move = pool.get('account.move')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
-        party = self.prep_party()
+        self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         self.prep_accounting(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             acc_type, = AccountType.search([('name', '=', 'Cash')])
 
             accounts = Account.create([{
                 'name': 'Bankaccount',
                 'code': '0123',
                 'type': acc_type.id,
                 }, {
@@ -4959,40 +5315,46 @@
             self.assertEqual(books[1].rec_name, 'Book Cash | 0.00 usd | Open')
             self.assertEqual(books[1].account.rec_name, '2345 - Cashaccount')
 
             # bank --> cash
             Book.write(*[
                 [books[0]],
                 {
-                    'lines':[('create', [{
+                    'lines': [('create', [{
                         'bookingtype': 'mvout',
                         'amount': Decimal('10.0'),
                         'date': date(2022, 5, 5),
                         'description': 'from bank to cash',
                         'booktransf': books[1].id,
                         }])],
                 }])
 
             self.assertEqual(len(books[0].lines), 1)
-            self.assertEqual(books[0].lines[0].rec_name,
-                '05/05/2022|to|-10.00 usd|from bank to cash [Book Cash | 0.00 usd | Open]')
+            self.assertEqual(
+                books[0].lines[0].rec_name,
+                '05/05/2022|to|-10.00 usd|from bank to cash ' +
+                '[Book Cash | 0.00 usd | Open]')
             self.assertEqual(len(books[0].lines[0].moves), 0)
             self.assertEqual(books[0].lines[0].category, None)
             self.assertEqual(books[0].lines[0].party, None)
 
             self.assertEqual(len(books[1].lines), 0)
             self.assertEqual(Move.search_count([]), 0)
 
             Line.wfcheck([books[0].lines[0]])
 
             self.assertEqual(len(books[1].lines), 1)
-            self.assertEqual(books[0].lines[0].rec_name,
-                '05/05/2022|to|-10.00 usd|from bank to cash [Book Cash | 10.00 usd | Open]')
-            self.assertEqual(books[1].lines[0].rec_name,
-                '05/05/2022|from|10.00 usd|from bank to cash [Book Bank | -10.00 usd | Open]')
+            self.assertEqual(
+                books[0].lines[0].rec_name,
+                '05/05/2022|to|-10.00 usd|from bank to cash ' +
+                '[Book Cash | 10.00 usd | Open]')
+            self.assertEqual(
+                books[1].lines[0].rec_name,
+                '05/05/2022|from|10.00 usd|from bank to cash ' +
+                '[Book Bank | -10.00 usd | Open]')
             self.assertEqual(len(books[1].lines[0].moves), 0)
             self.assertEqual(books[1].lines[0].category, None)
             self.assertEqual(books[1].lines[0].party, None)
 
             moves = Move.search([])
             self.assertEqual(len(moves), 1)
             self.assertEqual(len(moves[0].lines), 2)
@@ -5000,16 +5362,18 @@
             self.assertEqual(len(books[1].lines[0].moves), 0)
 
             self.assertEqual(moves[0].state, 'draft')
             self.assertEqual(moves[0].date, date(2022, 5, 5))
             self.assertEqual(moves[0].description, 'from bank to cash')
             self.assertEqual(moves[0].period.rec_name, '2022-05')
             self.assertEqual(moves[0].journal.rec_name, 'Cashbook')
-            self.assertEqual(moves[0].origin.rec_name,
-                '05/05/2022|to|-10.00 usd|from bank to cash [Book Cash | 10.00 usd | Open]')
+            self.assertEqual(
+                moves[0].origin.rec_name,
+                '05/05/2022|to|-10.00 usd|from bank to cash ' +
+                '[Book Cash | 10.00 usd | Open]')
             self.assertEqual(moves[0].lines[0].rec_name, '(0123 - Bankaccount)')
             self.assertEqual(moves[0].lines[0].credit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[0].debit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[0].amount_second_currency, None)
             self.assertEqual(moves[0].lines[1].rec_name, '2345 - Cashaccount')
             self.assertEqual(moves[0].lines[1].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[1].debit, Decimal('10.0'))
@@ -5033,33 +5397,31 @@
     def test_line_check_wf_out_transfer(self):
         """ create cashbook + line, transfer: cash -> bank
             same currrency in both accounts
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
         Account = pool.get('account.account')
         AccountType = pool.get('account.account.type')
         Journal = pool.get('account.journal')
         Move = pool.get('account.move')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
-        party = self.prep_party()
+        self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         self.prep_accounting(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             acc_type, = AccountType.search([('name', '=', 'Cash')])
 
             accounts = Account.create([{
                 'name': 'Bankaccount',
                 'code': '0123',
                 'type': acc_type.id,
                 }, {
@@ -5100,40 +5462,46 @@
             self.assertEqual(books[1].rec_name, 'Book Cash | 0.00 usd | Open')
             self.assertEqual(books[1].account.rec_name, '2345 - Cashaccount')
 
             # cash --> bank
             Book.write(*[
                 [books[0]],
                 {
-                    'lines':[('create', [{
+                    'lines': [('create', [{
                         'bookingtype': 'mvin',
                         'amount': Decimal('10.0'),
                         'date': date(2022, 5, 5),
                         'description': 'from cash to bank',
                         'booktransf': books[1].id,
                         }])],
                 }])
 
             self.assertEqual(len(books[0].lines), 1)
-            self.assertEqual(books[0].lines[0].rec_name,
-                '05/05/2022|from|10.00 usd|from cash to bank [Book Cash | 0.00 usd | Open]')
+            self.assertEqual(
+                books[0].lines[0].rec_name,
+                '05/05/2022|from|10.00 usd|from cash to bank ' +
+                '[Book Cash | 0.00 usd | Open]')
             self.assertEqual(len(books[0].lines[0].moves), 0)
             self.assertEqual(books[0].lines[0].category, None)
             self.assertEqual(books[0].lines[0].party, None)
 
             self.assertEqual(len(books[1].lines), 0)
             self.assertEqual(Move.search_count([]), 0)
 
             Line.wfcheck([books[0].lines[0]])
 
             self.assertEqual(len(books[1].lines), 1)
-            self.assertEqual(books[0].lines[0].rec_name,
-                '05/05/2022|from|10.00 usd|from cash to bank [Book Cash | -10.00 usd | Open]')
-            self.assertEqual(books[1].lines[0].rec_name,
-                '05/05/2022|to|-10.00 usd|from cash to bank [Book Bank | 10.00 usd | Open]')
+            self.assertEqual(
+                books[0].lines[0].rec_name,
+                '05/05/2022|from|10.00 usd|from cash to bank ' +
+                '[Book Cash | -10.00 usd | Open]')
+            self.assertEqual(
+                books[1].lines[0].rec_name,
+                '05/05/2022|to|-10.00 usd|from cash to bank ' +
+                '[Book Bank | 10.00 usd | Open]')
             self.assertEqual(len(books[1].lines[0].moves), 0)
             self.assertEqual(books[1].lines[0].category, None)
             self.assertEqual(books[1].lines[0].party, None)
 
             moves = Move.search([])
             self.assertEqual(len(moves), 1)
             self.assertEqual(len(moves[0].lines), 2)
@@ -5141,16 +5509,18 @@
             self.assertEqual(len(books[1].lines[0].moves), 0)
 
             self.assertEqual(moves[0].state, 'draft')
             self.assertEqual(moves[0].date, date(2022, 5, 5))
             self.assertEqual(moves[0].description, 'from cash to bank')
             self.assertEqual(moves[0].period.rec_name, '2022-05')
             self.assertEqual(moves[0].journal.rec_name, 'Cashbook')
-            self.assertEqual(moves[0].origin.rec_name,
-                '05/05/2022|from|10.00 usd|from cash to bank [Book Cash | -10.00 usd | Open]')
+            self.assertEqual(
+                moves[0].origin.rec_name,
+                '05/05/2022|from|10.00 usd|from cash to bank ' +
+                '[Book Cash | -10.00 usd | Open]')
             self.assertEqual(moves[0].lines[0].rec_name, '0123 - Bankaccount')
             self.assertEqual(moves[0].lines[0].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[0].debit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[0].amount_second_currency, None)
             self.assertEqual(moves[0].lines[1].rec_name, '(2345 - Cashaccount)')
             self.assertEqual(moves[0].lines[1].credit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[1].debit, Decimal('0.0'))
@@ -5174,35 +5544,33 @@
     def test_line_check_wf_out_transfer_2nd_currency(self):
         """ create cashbook + line, transfer: EURO <-- USD,
             different currrencies
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
         Line = pool.get('cashbook.line')
-        Configuration = pool.get('cashbook.configuration')
         Account = pool.get('account.account')
         AccountType = pool.get('account.account.type')
         Journal = pool.get('account.journal')
         Move = pool.get('account.move')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
-        party = self.prep_party()
+        self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         self.prep_accounting(company)
         # add EURO, set company-currency to EURO
         (usd, euro) = self.prep_2nd_currency(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             acc_type, = AccountType.search([('name', '=', 'Cash')])
 
             accounts = Account.create([{
                 'name': 'Bankaccount',
                 'code': '0123',
                 'type': acc_type.id,
                 }, {
@@ -5243,60 +5611,68 @@
             self.assertEqual(books[1].rec_name, 'Book USD | 0.00 usd | Open')
             self.assertEqual(books[1].account.rec_name, '2345 - Cashaccount')
 
             # Euro <-- USD
             Book.write(*[
                 [books[0]],
                 {
-                    'lines':[('create', [{
+                    'lines': [('create', [{
                         'bookingtype': 'mvin',
                         'amount': Decimal('10.0'),
                         'date': date(2022, 5, 5),
                         'description': 'EURO <-- USD',
                         'booktransf': books[1].id,
                         }])],
                 }])
 
             self.assertEqual(len(books[0].lines), 1)
-            self.assertEqual(books[0].lines[0].rec_name,
-                '05/05/2022|from|10.00 €|EURO <-- USD [Book USD | 0.00 usd | Open]')
+            self.assertEqual(
+                books[0].lines[0].rec_name,
+                '05/05/2022|from|10.00 €|EURO <-- ' +
+                'USD [Book USD | 0.00 usd | Open]')
             self.assertEqual(len(books[0].lines[0].moves), 0)
             self.assertEqual(books[0].lines[0].category, None)
             self.assertEqual(books[0].lines[0].party, None)
 
             self.assertEqual(len(books[1].lines), 0)
             self.assertEqual(Move.search_count([]), 0)
 
             Line.wfcheck([books[0].lines[0]])
 
             self.assertEqual(len(books[0].lines), 1)
-            self.assertEqual(books[0].lines[0].rec_name,
-                '05/05/2022|from|10.00 €|EURO <-- USD [Book USD | -10.50 usd | Open]')
+            self.assertEqual(
+                books[0].lines[0].rec_name,
+                '05/05/2022|from|10.00 €|EURO <-- ' +
+                'USD [Book USD | -10.50 usd | Open]')
             self.assertEqual(len(books[0].lines[0].moves), 1)
             self.assertEqual(books[0].lines[0].category, None)
             self.assertEqual(books[0].lines[0].party, None)
 
             self.assertEqual(len(books[1].lines), 1)
-            self.assertEqual(books[1].lines[0].rec_name,
-                '05/05/2022|to|-10.50 usd|EURO <-- USD [Book EURO | 10.00 € | Open]')
+            self.assertEqual(
+                books[1].lines[0].rec_name,
+                '05/05/2022|to|-10.50 usd|EURO <-- ' +
+                'USD [Book EURO | 10.00 € | Open]')
             self.assertEqual(len(books[1].lines[0].moves), 0)
             self.assertEqual(books[1].lines[0].category, None)
             self.assertEqual(books[1].lines[0].party, None)
 
             moves = Move.search([])
             self.assertEqual(len(moves), 1)
             self.assertEqual(len(moves[0].lines), 2)
 
             self.assertEqual(moves[0].state, 'draft')
             self.assertEqual(moves[0].date, date(2022, 5, 5))
             self.assertEqual(moves[0].description, 'EURO <-- USD')
             self.assertEqual(moves[0].period.rec_name, '2022-05')
             self.assertEqual(moves[0].journal.rec_name, 'Cashbook')
-            self.assertEqual(moves[0].origin.rec_name,
-                '05/05/2022|from|10.00 €|EURO <-- USD [Book USD | -10.50 usd | Open]')
+            self.assertEqual(
+                moves[0].origin.rec_name,
+                '05/05/2022|from|10.00 €|EURO <-- ' +
+                'USD [Book USD | -10.50 usd | Open]')
             self.assertEqual(moves[0].lines[0].rec_name, '0123 - Bankaccount')
             self.assertEqual(moves[0].lines[0].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[0].debit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[0].amount_second_currency, None)
             self.assertEqual(moves[0].lines[1].rec_name, '(2345 - Cashaccount)')
             self.assertEqual(moves[0].lines[1].credit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[1].debit, Decimal('0.0'))
```

### Comparing `mds_cashbook_account-6.0.9/view/book_form.xml` & `mds_cashbook_account-6.8.11/view/book_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook_account-6.0.9/view/category_form.xml` & `mds_cashbook_account-6.8.11/view/category_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook_account-6.0.9/view/line_form.xml` & `mds_cashbook_account-6.8.11/view/line_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook_account-6.0.9/view/split_form.xml` & `mds_cashbook_account-6.8.11/view/split_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook_account-6.0.9/view/tax_form.xml` & `mds_cashbook_account-6.8.11/view/tax_form.xml`

 * *Files identical despite different names*

