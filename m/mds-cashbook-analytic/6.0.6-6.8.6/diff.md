# Comparing `tmp/mds_cashbook_analytic-6.0.6.tar.gz` & `tmp/mds_cashbook_analytic-6.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mds_cashbook_analytic-6.0.6.tar", last modified: Tue Jul 25 20:46:09 2023, max compression
+gzip compressed data, was "mds_cashbook_analytic-6.8.6.tar", last modified: Tue Jul 25 20:37:03 2023, max compression
```

## Comparing `mds_cashbook_analytic-6.0.6.tar` & `mds_cashbook_analytic-6.8.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-25 20:46:09.819967 mds_cashbook_analytic-6.0.6/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1898 2023-07-25 20:46:09.819967 mds_cashbook_analytic-6.0.6/PKG-INFO
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      459 2023-07-25 20:43:16.000000 mds_cashbook_analytic-6.0.6/README.rst
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      396 2023-06-05 17:53:57.000000 mds_cashbook_analytic-6.0.6/__init__.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      695 2022-12-17 10:34:43.000000 mds_cashbook_analytic-6.0.6/analytic.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      699 2023-06-05 18:03:48.000000 mds_cashbook_analytic-6.0.6/book.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1875 2022-12-17 10:34:43.000000 mds_cashbook_analytic-6.0.6/book.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     2678 2023-06-05 17:53:57.000000 mds_cashbook_analytic-6.0.6/line.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      491 2022-12-17 10:34:43.000000 mds_cashbook_analytic-6.0.6/line.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-25 20:46:09.815967 mds_cashbook_analytic-6.0.6/locale/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      442 2022-12-17 10:34:43.000000 mds_cashbook_analytic-6.0.6/locale/de.po
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      233 2022-12-17 10:34:43.000000 mds_cashbook_analytic-6.0.6/locale/en.po
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-25 20:46:09.819967 mds_cashbook_analytic-6.0.6/mds_cashbook_analytic.egg-info/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1898 2023-07-25 20:46:09.000000 mds_cashbook_analytic-6.0.6/mds_cashbook_analytic.egg-info/PKG-INFO
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      601 2023-07-25 20:46:09.000000 mds_cashbook_analytic-6.0.6/mds_cashbook_analytic.egg-info/SOURCES.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-07-25 20:46:09.000000 mds_cashbook_analytic-6.0.6/mds_cashbook_analytic.egg-info/dependency_links.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       85 2023-07-25 20:46:09.000000 mds_cashbook_analytic-6.0.6/mds_cashbook_analytic.egg-info/entry_points.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-07-25 20:46:09.000000 mds_cashbook_analytic-6.0.6/mds_cashbook_analytic.egg-info/not-zip-safe
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      123 2023-07-25 20:46:09.000000 mds_cashbook_analytic-6.0.6/mds_cashbook_analytic.egg-info/requires.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2023-07-25 20:46:09.000000 mds_cashbook_analytic-6.0.6/mds_cashbook_analytic.egg-info/top_level.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      415 2022-12-17 10:34:43.000000 mds_cashbook_analytic-6.0.6/message.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2023-07-25 20:46:09.819967 mds_cashbook_analytic-6.0.6/setup.cfg
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     3735 2023-07-25 20:40:17.000000 mds_cashbook_analytic-6.0.6/setup.py
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-25 20:46:09.815967 mds_cashbook_analytic-6.0.6/tests/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      632 2023-06-05 18:03:48.000000 mds_cashbook_analytic-6.0.6/tests/__init__.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    14710 2023-06-05 18:03:48.000000 mds_cashbook_analytic-6.0.6/tests/test_analytic.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      151 2023-07-25 20:42:57.000000 mds_cashbook_analytic-6.0.6/tryton.cfg
--rw-rw----   0 trytproj  (1001) trytproj  (1001)       64 2023-07-25 20:42:52.000000 mds_cashbook_analytic-6.0.6/versiondep.txt
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-25 20:46:09.815967 mds_cashbook_analytic-6.0.6/view/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      396 2022-12-17 10:34:43.000000 mds_cashbook_analytic-6.0.6/view/book_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      332 2023-05-23 20:28:07.000000 mds_cashbook_analytic-6.0.6/view/book_list.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      438 2022-12-17 10:34:43.000000 mds_cashbook_analytic-6.0.6/view/line_form.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-25 20:37:03.424342 mds_cashbook_analytic-6.8.6/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1535 2023-07-25 20:37:03.424342 mds_cashbook_analytic-6.8.6/PKG-INFO
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      256 2023-07-25 20:35:34.000000 mds_cashbook_analytic-6.8.6/README.rst
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      396 2023-06-05 17:25:32.000000 mds_cashbook_analytic-6.8.6/__init__.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      695 2023-05-24 05:54:51.000000 mds_cashbook_analytic-6.8.6/analytic.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      686 2023-06-05 17:21:07.000000 mds_cashbook_analytic-6.8.6/book.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1875 2023-05-24 05:54:51.000000 mds_cashbook_analytic-6.8.6/book.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     2678 2023-06-05 17:20:41.000000 mds_cashbook_analytic-6.8.6/line.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      491 2023-05-24 05:54:51.000000 mds_cashbook_analytic-6.8.6/line.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-25 20:37:03.416342 mds_cashbook_analytic-6.8.6/locale/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      442 2023-05-24 05:54:51.000000 mds_cashbook_analytic-6.8.6/locale/de.po
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      233 2023-05-24 05:54:51.000000 mds_cashbook_analytic-6.8.6/locale/en.po
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-25 20:37:03.424342 mds_cashbook_analytic-6.8.6/mds_cashbook_analytic.egg-info/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1535 2023-07-25 20:37:03.000000 mds_cashbook_analytic-6.8.6/mds_cashbook_analytic.egg-info/PKG-INFO
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      601 2023-07-25 20:37:03.000000 mds_cashbook_analytic-6.8.6/mds_cashbook_analytic.egg-info/SOURCES.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-07-25 20:37:03.000000 mds_cashbook_analytic-6.8.6/mds_cashbook_analytic.egg-info/dependency_links.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       85 2023-07-25 20:37:03.000000 mds_cashbook_analytic-6.8.6/mds_cashbook_analytic.egg-info/entry_points.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-07-25 20:37:03.000000 mds_cashbook_analytic-6.8.6/mds_cashbook_analytic.egg-info/not-zip-safe
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      123 2023-07-25 20:37:03.000000 mds_cashbook_analytic-6.8.6/mds_cashbook_analytic.egg-info/requires.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2023-07-25 20:37:03.000000 mds_cashbook_analytic-6.8.6/mds_cashbook_analytic.egg-info/top_level.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      415 2023-05-24 05:54:51.000000 mds_cashbook_analytic-6.8.6/message.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2023-07-25 20:37:03.424342 mds_cashbook_analytic-6.8.6/setup.cfg
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     3735 2023-07-25 20:34:35.000000 mds_cashbook_analytic-6.8.6/setup.py
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-25 20:37:03.420342 mds_cashbook_analytic-6.8.6/tests/
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      144 2023-06-05 17:26:00.000000 mds_cashbook_analytic-6.8.6/tests/__init__.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    14728 2023-06-05 17:28:31.000000 mds_cashbook_analytic-6.8.6/tests/test_analytic.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      152 2023-07-25 20:34:58.000000 mds_cashbook_analytic-6.8.6/tryton.cfg
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)       64 2023-07-25 20:35:11.000000 mds_cashbook_analytic-6.8.6/versiondep.txt
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-25 20:37:03.420342 mds_cashbook_analytic-6.8.6/view/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      396 2023-05-24 05:54:51.000000 mds_cashbook_analytic-6.8.6/view/book_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      332 2023-05-24 05:54:51.000000 mds_cashbook_analytic-6.8.6/view/book_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      438 2023-05-24 05:54:51.000000 mds_cashbook_analytic-6.8.6/view/line_form.xml
```

### Comparing `mds_cashbook_analytic-6.0.6/PKG-INFO` & `mds_cashbook_analytic-6.8.6/mds_cashbook_analytic.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: mds_cashbook_analytic
-Version: 6.0.6
+Name: mds-cashbook-analytic
+Version: 6.8.6
 Summary: Tryton module to add analytic-accounts to cashbook.
 Home-page: https://www.m-ds.de/
 Author: martin-data services
 Author-email: service@m-ds.de
 License: GPL-3
 Description: mds-cashbook-analytic
         =====================
@@ -13,44 +13,24 @@
         Install
         =======
         
         pip install mds-cashbook-analytic
         
         Requires
         ========
-        - Tryton 6.0
+        - Tryton 6.8
         
         Changes
         =======
         
-        *6.0.6 - 25.07.2023*
+        *6.8.6 - 25.07.2023*
         
-        - optimized code
-        
-        *6.0.5 - 05.06.2023*
-        
-        - optimized code
-        
-        *6.0.4 - 14.02.2023*
-        
-        - fix: columns
-        
-        *6.0.3 - 30.09.2022*
-        
-        - updt: parameter
-        
-        *6.0.2 - 07.09.2022*
-        
-        - updt: permissions
-        
-        *6.0.1 - 05.09.2022*
-        
-        - works
+        - init
         
-        *6.0.0 - 05.09.2022*
+        *6.8.5 - 05.06.2023*
         
         - init
         
 Keywords: tryton cashbook analytic account
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `mds_cashbook_analytic-6.0.6/analytic.xml` & `mds_cashbook_analytic-6.8.6/analytic.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook_analytic-6.0.6/book.py` & `mds_cashbook_analytic-6.8.6/book.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class Book(metaclass=PoolMeta):
     __name__ = 'cashbook.book'
 
     analytic = fields.Many2One(
         string='Analytic Account', ondelete='RESTRICT',
-        model_name='analytic_account.account', select=True,
+        model_name='analytic_account.account',
         domain=[
             ('company.id', '=', Eval('company', -1)),
             ('type', 'in', ['normal', 'distribution']),
             ],
         depends=['company'])
 
 # end Book
```

### Comparing `mds_cashbook_analytic-6.0.6/book.xml` & `mds_cashbook_analytic-6.8.6/book.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook_analytic-6.0.6/line.py` & `mds_cashbook_analytic-6.8.6/line.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook_analytic-6.0.6/mds_cashbook_analytic.egg-info/PKG-INFO` & `mds_cashbook_analytic-6.8.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: mds-cashbook-analytic
-Version: 6.0.6
+Name: mds_cashbook_analytic
+Version: 6.8.6
 Summary: Tryton module to add analytic-accounts to cashbook.
 Home-page: https://www.m-ds.de/
 Author: martin-data services
 Author-email: service@m-ds.de
 License: GPL-3
 Description: mds-cashbook-analytic
         =====================
@@ -13,44 +13,24 @@
         Install
         =======
         
         pip install mds-cashbook-analytic
         
         Requires
         ========
-        - Tryton 6.0
+        - Tryton 6.8
         
         Changes
         =======
         
-        *6.0.6 - 25.07.2023*
+        *6.8.6 - 25.07.2023*
         
-        - optimized code
-        
-        *6.0.5 - 05.06.2023*
-        
-        - optimized code
-        
-        *6.0.4 - 14.02.2023*
-        
-        - fix: columns
-        
-        *6.0.3 - 30.09.2022*
-        
-        - updt: parameter
-        
-        *6.0.2 - 07.09.2022*
-        
-        - updt: permissions
-        
-        *6.0.1 - 05.09.2022*
-        
-        - works
+        - init
         
-        *6.0.0 - 05.09.2022*
+        *6.8.5 - 05.06.2023*
         
         - init
         
 Keywords: tryton cashbook analytic account
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `mds_cashbook_analytic-6.0.6/mds_cashbook_analytic.egg-info/SOURCES.txt` & `mds_cashbook_analytic-6.8.6/mds_cashbook_analytic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mds_cashbook_analytic-6.0.6/setup.py` & `mds_cashbook_analytic-6.8.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         l2 = i.strip().split(';')
         if len(l2) < 4:
             continue
         modversion[l2[0]] = {'min': l2[1], 'max': l2[2], 'prefix': l2[3]}
 
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
```

### Comparing `mds_cashbook_analytic-6.0.6/tests/test_analytic.py` & `mds_cashbook_analytic-6.8.6/tests/test_analytic.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 # This file is part of the cashbook-module from m-ds for Tryton.
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
 from trytond.tests.test_tryton import with_transaction
 from trytond.pool import Pool
 from trytond.transaction import Transaction
-from trytond.modules.cashbook_account.tests import CashbookAccountTestCase
+from trytond.modules.cashbook_account.tests.test_module import \
+    CashbookAccountTestCase
 from decimal import Decimal
 from datetime import date
 
 
 class AnalyticTestCase(CashbookAccountTestCase):
     'Test cashbook analytic module'
     module = 'cashbook_analytic'
```

