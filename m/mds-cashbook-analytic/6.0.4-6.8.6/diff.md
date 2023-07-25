# Comparing `tmp/mds_cashbook_analytic-6.0.4.tar.gz` & `tmp/mds_cashbook_analytic-6.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mds_cashbook_analytic-6.0.4.tar", last modified: Tue Feb 14 09:30:27 2023, max compression
+gzip compressed data, was "mds_cashbook_analytic-6.8.6.tar", last modified: Tue Jul 25 20:37:03 2023, max compression
```

## Comparing `mds_cashbook_analytic-6.0.4.tar` & `mds_cashbook_analytic-6.8.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-02-14 09:30:27.221854 mds_cashbook_analytic-6.0.4/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1704 2023-02-14 09:30:27.217854 mds_cashbook_analytic-6.0.4/PKG-INFO
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      379 2023-02-14 09:27:35.000000 mds_cashbook_analytic-6.0.4/README.rst
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      395 2022-09-05 11:15:25.000000 mds_cashbook_analytic-6.0.4/__init__.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      695 2022-09-07 09:43:33.000000 mds_cashbook_analytic-6.0.4/analytic.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      696 2022-09-05 09:31:36.000000 mds_cashbook_analytic-6.0.4/book.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1875 2022-09-05 09:12:40.000000 mds_cashbook_analytic-6.0.4/book.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     2650 2022-09-30 09:19:38.000000 mds_cashbook_analytic-6.0.4/line.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      491 2022-09-05 15:04:57.000000 mds_cashbook_analytic-6.0.4/line.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-02-14 09:30:27.217854 mds_cashbook_analytic-6.0.4/locale/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      442 2022-09-05 15:13:09.000000 mds_cashbook_analytic-6.0.4/locale/de.po
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      233 2022-09-05 15:18:16.000000 mds_cashbook_analytic-6.0.4/locale/en.po
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-02-14 09:30:27.217854 mds_cashbook_analytic-6.0.4/mds_cashbook_analytic.egg-info/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1704 2023-02-14 09:30:27.000000 mds_cashbook_analytic-6.0.4/mds_cashbook_analytic.egg-info/PKG-INFO
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      601 2023-02-14 09:30:27.000000 mds_cashbook_analytic-6.0.4/mds_cashbook_analytic.egg-info/SOURCES.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-02-14 09:30:27.000000 mds_cashbook_analytic-6.0.4/mds_cashbook_analytic.egg-info/dependency_links.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       85 2023-02-14 09:30:27.000000 mds_cashbook_analytic-6.0.4/mds_cashbook_analytic.egg-info/entry_points.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-02-14 09:30:27.000000 mds_cashbook_analytic-6.0.4/mds_cashbook_analytic.egg-info/not-zip-safe
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      122 2023-02-14 09:30:27.000000 mds_cashbook_analytic-6.0.4/mds_cashbook_analytic.egg-info/requires.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2023-02-14 09:30:27.000000 mds_cashbook_analytic-6.0.4/mds_cashbook_analytic.egg-info/top_level.txt
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      415 2022-09-05 09:22:26.000000 mds_cashbook_analytic-6.0.4/message.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2023-02-14 09:30:27.221854 mds_cashbook_analytic-6.0.4/setup.cfg
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     3602 2022-09-05 09:01:28.000000 mds_cashbook_analytic-6.0.4/setup.py
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-02-14 09:30:27.217854 mds_cashbook_analytic-6.0.4/tests/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      632 2022-09-05 12:15:00.000000 mds_cashbook_analytic-6.0.4/tests/__init__.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    14276 2022-09-05 14:56:02.000000 mds_cashbook_analytic-6.0.4/tests/test_analytic.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      151 2023-02-14 09:27:55.000000 mds_cashbook_analytic-6.0.4/tryton.cfg
--rw-rw----   0 trytproj  (1001) trytproj  (1001)       63 2023-02-14 09:27:51.000000 mds_cashbook_analytic-6.0.4/versiondep.txt
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-02-14 09:30:27.217854 mds_cashbook_analytic-6.0.4/view/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      396 2022-09-05 09:55:17.000000 mds_cashbook_analytic-6.0.4/view/book_form.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      332 2023-02-14 09:27:13.000000 mds_cashbook_analytic-6.0.4/view/book_list.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      438 2022-09-05 15:07:16.000000 mds_cashbook_analytic-6.0.4/view/line_form.xml
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

### Comparing `mds_cashbook_analytic-6.0.4/PKG-INFO` & `mds_cashbook_analytic-6.8.6/mds_cashbook_analytic.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: mds_cashbook_analytic
-Version: 6.0.4
+Name: mds-cashbook-analytic
+Version: 6.8.6
 Summary: Tryton module to add analytic-accounts to cashbook.
 Home-page: https://www.m-ds.de/
 Author: martin-data services
 Author-email: service@m-ds.de
 License: GPL-3
 Description: mds-cashbook-analytic
         =====================
@@ -13,36 +13,24 @@
         Install
         =======
         
         pip install mds-cashbook-analytic
         
         Requires
         ========
-        - Tryton 6.0
+        - Tryton 6.8
         
         Changes
         =======
         
-        *6.0.4 - 14.02.2023*
+        *6.8.6 - 25.07.2023*
         
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
@@ -55,7 +43,8 @@
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Natural Language :: German
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mds_cashbook_analytic-6.0.4/analytic.xml` & `mds_cashbook_analytic-6.8.6/analytic.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook_analytic-6.0.4/book.py` & `mds_cashbook_analytic-6.8.6/book.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # -*- coding: utf-8 -*-
 # This file is part of the cashbook-module from m-ds for Tryton.
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
 from trytond.model import fields
-from trytond.pool import Pool, PoolMeta
+from trytond.pool import PoolMeta
 from trytond.pyson import Eval
 
 
 class Book(metaclass=PoolMeta):
     __name__ = 'cashbook.book'
 
-    analytic = fields.Many2One(string='Analytic Account', ondelete='RESTRICT',
-        model_name='analytic_account.account', select=True,
+    analytic = fields.Many2One(
+        string='Analytic Account', ondelete='RESTRICT',
+        model_name='analytic_account.account',
         domain=[
             ('company.id', '=', Eval('company', -1)),
             ('type', 'in', ['normal', 'distribution']),
             ],
         depends=['company'])
 
 # end Book
```

### Comparing `mds_cashbook_analytic-6.0.4/book.xml` & `mds_cashbook_analytic-6.8.6/book.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook_analytic-6.0.4/line.py` & `mds_cashbook_analytic-6.8.6/line.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 # -*- coding: utf-8 -*-
 # This file is part of the cashbook-module from m-ds for Tryton.
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
-from trytond.pool import Pool, PoolMeta
+from trytond.pool import PoolMeta
 from trytond.model import fields
 from trytond.pyson import Eval, Bool
 
 
 class Line(metaclass=PoolMeta):
     __name__ = 'cashbook.line'
 
-    analytic_lines = fields.Function(fields.One2Many(string='Analytic Lines',
-        readonly=True, field=None, model_name='analytic_account.line',
+    analytic_lines = fields.Function(fields.One2Many(
+        string='Analytic Lines', readonly=True, field=None,
+        model_name='analytic_account.line',
         states={
             'invisible': ~Bool(Eval('analytic_lines')),
         }),
         'on_change_with_analytic_lines')
 
     @fields.depends('moves')
     def on_change_with_analytic_lines(self, name=None):
         """ get analytic-lines of move-line
         """
         if len(self.moves) > 0:
-            return [z.id for x in self.moves for y in x.lines for z in y.analytic_lines]
+            return [
+                z.id for x in self.moves
+                for y in x.lines for z in y.analytic_lines]
 
     @classmethod
     def get_create_analytic_lines(cls, account, move_date, credit, debit):
         """ generate code to create analytic-lines
         """
         debit_lst = account.distribute(debit)
         credit_lst = account.distribute(credit)
 
         # put credit/debits-lists in one dict
-        analytic_dict = {x[0].id:{'credit': x[1]} for x in credit_lst}
+        analytic_dict = {x[0].id: {'credit': x[1]} for x in credit_lst}
         for x in debit_lst:
             analytic_dict[x[0].id]['debit'] = x[1]
 
         lines = [{
                 'account': x,
                 'date': move_date,
                 'credit': analytic_dict[x]['credit'],
@@ -56,21 +59,21 @@
         cb_line = None
         if line.__name__ == 'cashbook.line':
             analytic_account = line.cashbook.analytic
             cb_line = line
         elif line.__name__ == 'cashbook.split':
             analytic_account = line.line.cashbook.analytic
             cb_line = line.line
-        else :
+        else:
             raise ValueError('invalid model: %s' % line._name__)
 
         if analytic_account:
             for num in range(len(move_lines)):
-                move_lines[num]['analytic_lines'] = cls.get_create_analytic_lines(
-                        account = analytic_account,
-                        move_date = cb_line.date,
-                        credit = cb_line.credit,
-                        debit = cb_line.debit,
-                    )
+                move_lines[num]['analytic_lines'] = \
+                    cls.get_create_analytic_lines(
+                        account=analytic_account,
+                        move_date=cb_line.date,
+                        credit=cb_line.credit,
+                        debit=cb_line.debit)
         return move_lines
 
 # end Line
```

### Comparing `mds_cashbook_analytic-6.0.4/mds_cashbook_analytic.egg-info/PKG-INFO` & `mds_cashbook_analytic-6.8.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: mds-cashbook-analytic
-Version: 6.0.4
+Name: mds_cashbook_analytic
+Version: 6.8.6
 Summary: Tryton module to add analytic-accounts to cashbook.
 Home-page: https://www.m-ds.de/
 Author: martin-data services
 Author-email: service@m-ds.de
 License: GPL-3
 Description: mds-cashbook-analytic
         =====================
@@ -13,36 +13,24 @@
         Install
         =======
         
         pip install mds-cashbook-analytic
         
         Requires
         ========
-        - Tryton 6.0
+        - Tryton 6.8
         
         Changes
         =======
         
-        *6.0.4 - 14.02.2023*
+        *6.8.6 - 25.07.2023*
         
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
@@ -55,7 +43,8 @@
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Natural Language :: German
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mds_cashbook_analytic-6.0.4/mds_cashbook_analytic.egg-info/SOURCES.txt` & `mds_cashbook_analytic-6.8.6/mds_cashbook_analytic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mds_cashbook_analytic-6.0.4/setup.py` & `mds_cashbook_analytic-6.8.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ Tryton module to add analytic-accounts to cashbook
 """
 
 # Always prefer setuptools over distutils
-from setuptools import setup, find_packages
+from setuptools import setup
 # To use a consistent encoding
 from codecs import open
 from os import path
 import re
 try:
     from configparser import ConfigParser
 except ImportError:
@@ -32,79 +32,81 @@
 modversion = {}
 with open(path.join(here, 'versiondep.txt'), encoding='utf-8') as f:
     l1 = f.readlines()
     for i in l1:
         l2 = i.strip().split(';')
         if len(l2) < 4:
             continue
-        modversion[l2[0]] = {'min':l2[1], 'max':l2[2], 'prefix':l2[3]}
+        modversion[l2[0]] = {'min': l2[1], 'max': l2[2], 'prefix': l2[3]}
 
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
                 prefix = modversion[dep]['prefix']
 
             if len(modversion[dep]['max']) > 0:
-                requires.append('%s_%s >= %s, <= %s' %
-                    (prefix, dep, modversion[dep]['min'], modversion[dep]['max']))
-            else :
-                requires.append('%s_%s >= %s' %
-                    (prefix, dep, modversion[dep]['min']))
-        else :
-          requires.append('%s_%s >= %s.%s, < %s.%s' %
-                ('trytond', dep, major_version, minor_version,
+                requires.append('%s_%s >= %s, <= %s' % (
+                    prefix, dep, modversion[dep]['min'],
+                    modversion[dep]['max']))
+            else:
+                requires.append('%s_%s >= %s' % (
+                    prefix, dep, modversion[dep]['min']))
+        else:
+            requires.append('%s_%s >= %s.%s, < %s.%s' % (
+                'trytond', dep, major_version, minor_version,
                 major_version, minor_version + 1))
-requires.append('trytond >= %s.%s, < %s.%s' %
-        (major_version, minor_version, major_version, minor_version + 1))
+requires.append('trytond >= %s.%s, < %s.%s' % (
+    major_version, minor_version, major_version, minor_version + 1))
 
-setup(name='%s_%s' % (PREFIX, MODULE),
+setup(
+    name='%s_%s' % (PREFIX, MODULE),
     version=info.get('version', '0.0.1'),
     description='Tryton module to add analytic-accounts to cashbook.',
     long_description=long_description,
     url='https://www.m-ds.de/',
     author='martin-data services',
     author_email='service@m-ds.de',
     license='GPL-3',
     classifiers=[
-    'Development Status :: 5 - Production/Stable',
-    'Environment :: Plugins',
-    'Framework :: Tryton',
-    'Intended Audience :: Developers',
-    'Intended Audience :: Customer Service',
-    'Intended Audience :: Information Technology',
-    'Intended Audience :: Financial and Insurance Industry',
-    'Topic :: Office/Business',
-    'Topic :: Office/Business :: Financial :: Accounting',
-    'Natural Language :: German',
-    'Natural Language :: English',
-    'Operating System :: OS Independent',
-    'License :: OSI Approved :: GNU General Public License (GPL)',
-    'Programming Language :: Python :: 3.7',
-    'Programming Language :: Python :: 3.8',
+        'Development Status :: 5 - Production/Stable',
+        'Environment :: Plugins',
+        'Framework :: Tryton',
+        'Intended Audience :: Developers',
+        'Intended Audience :: Customer Service',
+        'Intended Audience :: Information Technology',
+        'Intended Audience :: Financial and Insurance Industry',
+        'Topic :: Office/Business',
+        'Topic :: Office/Business :: Financial :: Accounting',
+        'Natural Language :: German',
+        'Natural Language :: English',
+        'Operating System :: OS Independent',
+        'License :: OSI Approved :: GNU General Public License (GPL)',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
     ],
-
     keywords='tryton cashbook analytic account',
     package_dir={'trytond.modules.%s' % MODULE: '.'},
     packages=[
         'trytond.modules.%s' % MODULE,
         ],
     package_data={
-        'trytond.modules.%s' % MODULE: (info.get('xml', [])
+        'trytond.modules.%s' % MODULE: (
+            info.get('xml', [])
             + ['tryton.cfg', 'locale/*.po', 'tests/*.py',
                 'view/*.xml',
                 'versiondep.txt', 'README.rst']),
         },
-
     install_requires=requires,
     zip_safe=False,
     entry_points="""
     [trytond.modules]
     %s = trytond.modules.%s
     """ % (MODULE, MODULE),
 )
```

### Comparing `mds_cashbook_analytic-6.0.4/tests/test_analytic.py` & `mds_cashbook_analytic-6.8.6/tests/test_analytic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # -*- coding: utf-8 -*-
 # This file is part of the cashbook-module from m-ds for Tryton.
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
-from trytond.tests.test_tryton import ModuleTestCase, with_transaction
+from trytond.tests.test_tryton import with_transaction
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
@@ -64,36 +65,34 @@
     def test_analytic_line_check_wf_in_booking_normal(self):
         """ create cashbook + line + analytic-account,
             check booking in-type, company-currency
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
         AnalyticAccount = pool.get('analytic_account.account')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         self.prep_accounting(company)
         self.prep_analytic_accounts(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             acc_type, = AccountType.search([('name', '=', 'Cash')])
             analytic_account, = AnalyticAccount.search([('code', '=', '001')])
 
             accounts = Account.create([{
                 'name': 'Account Book',
                 'code': '0123',
                 'type': acc_type.id,
@@ -136,42 +135,55 @@
                         'party': party.id,
                     }])],
                 }])
             self.assertEqual(book.rec_name, 'Book 1 | 10.00 usd | Open')
             self.assertEqual(book.account.rec_name, '0123 - Account Book')
             self.assertEqual(book.analytic.rec_name, '001 - Food')
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
+                moves[0].lines[0].rec_name,
+                '(2345 - Account Category)')
             self.assertEqual(moves[0].lines[0].credit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[0].debit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[0].amount_second_currency, None)
             self.assertEqual(len(moves[0].lines[0].analytic_lines), 1)
-            self.assertEqual(moves[0].lines[0].analytic_lines[0].account.rec_name, '001 - Food')
-            self.assertEqual(moves[0].lines[0].analytic_lines[0].date, date(2022, 5, 5))
-            self.assertEqual(moves[0].lines[0].analytic_lines[0].credit, Decimal('10.0'))
-            self.assertEqual(moves[0].lines[0].analytic_lines[0].debit, Decimal('0.0'))
+            self.assertEqual(
+                moves[0].lines[0].analytic_lines[0].account.rec_name,
+                '001 - Food')
+            self.assertEqual(
+                moves[0].lines[0].analytic_lines[0].date,
+                date(2022, 5, 5))
+            self.assertEqual(
+                moves[0].lines[0].analytic_lines[0].credit,
+                Decimal('10.0'))
+            self.assertEqual(
+                moves[0].lines[0].analytic_lines[0].debit,
+                Decimal('0.0'))
 
             self.assertEqual(moves[0].lines[1].rec_name, '0123 - Account Book')
             self.assertEqual(moves[0].lines[1].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[1].debit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[1].amount_second_currency, None)
             self.assertEqual(len(moves[0].lines[1].analytic_lines), 0)
 
@@ -193,36 +205,34 @@
     def test_analytic_line_check_wf_in_booking_distri(self):
         """ create cashbook + line + analytic-account (distribution),
             check booking in-type, company-currency
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
         AnalyticAccount = pool.get('analytic_account.account')
 
         types = self.prep_type()
-        category = self.prep_category(cattype='in')
+        self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
         cfg1 = self.prep_config()
         cfg1.cataccno = True
         cfg1.save()
 
         self.prep_accounting(company)
         self.prep_analytic_accounts(company)
 
         with Transaction().set_context({
-            'company': company.id,
-            }):
+                'company': company.id}):
             acc_type, = AccountType.search([('name', '=', 'Cash')])
             analytic_account, = AnalyticAccount.search([('code', '=', '003')])
 
             accounts = Account.create([{
                 'name': 'Account Book',
                 'code': '0123',
                 'type': acc_type.id,
@@ -265,46 +275,68 @@
                         'party': party.id,
                     }])],
                 }])
             self.assertEqual(book.rec_name, 'Book 1 | 10.00 usd | Open')
             self.assertEqual(book.account.rec_name, '0123 - Account Book')
             self.assertEqual(book.analytic.rec_name, '003 - Distri')
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
             self.assertEqual(len(moves[0].lines[0].analytic_lines), 2)
-            self.assertEqual(moves[0].lines[0].analytic_lines[0].account.rec_name, '001 - Food')
-            self.assertEqual(moves[0].lines[0].analytic_lines[0].date, date(2022, 5, 5))
-            self.assertEqual(moves[0].lines[0].analytic_lines[0].credit, Decimal('5.0'))
-            self.assertEqual(moves[0].lines[0].analytic_lines[0].debit, Decimal('0.0'))
-            self.assertEqual(moves[0].lines[0].analytic_lines[1].account.rec_name, '002 - Drink')
-            self.assertEqual(moves[0].lines[0].analytic_lines[1].date, date(2022, 5, 5))
-            self.assertEqual(moves[0].lines[0].analytic_lines[1].credit, Decimal('5.0'))
-            self.assertEqual(moves[0].lines[0].analytic_lines[1].debit, Decimal('0.0'))
+            self.assertEqual(
+                moves[0].lines[0].analytic_lines[0].account.rec_name,
+                '001 - Food')
+            self.assertEqual(
+                moves[0].lines[0].analytic_lines[0].date,
+                date(2022, 5, 5))
+            self.assertEqual(
+                moves[0].lines[0].analytic_lines[0].credit,
+                Decimal('5.0'))
+            self.assertEqual(
+                moves[0].lines[0].analytic_lines[0].debit,
+                Decimal('0.0'))
+            self.assertEqual(
+                moves[0].lines[0].analytic_lines[1].account.rec_name,
+                '002 - Drink')
+            self.assertEqual(
+                moves[0].lines[0].analytic_lines[1].date,
+                date(2022, 5, 5))
+            self.assertEqual(
+                moves[0].lines[0].analytic_lines[1].credit,
+                Decimal('5.0'))
+            self.assertEqual(
+                moves[0].lines[0].analytic_lines[1].debit,
+                Decimal('0.0'))
 
             self.assertEqual(moves[0].lines[1].rec_name, '0123 - Account Book')
             self.assertEqual(moves[0].lines[1].credit, Decimal('0.0'))
             self.assertEqual(moves[0].lines[1].debit, Decimal('10.0'))
             self.assertEqual(moves[0].lines[1].amount_second_currency, None)
             self.assertEqual(len(moves[0].lines[1].analytic_lines), 0)
 
@@ -319,7 +351,10 @@
 
             # post move
             Line.wfdone([book.lines[0]])
             self.assertEqual(len(book.lines[0].moves), 1)
             self.assertEqual(book.lines[0].moves[0].state, 'posted')
 
 # end AnalyticTestCase
+
+
+del CashbookAccountTestCase
```

