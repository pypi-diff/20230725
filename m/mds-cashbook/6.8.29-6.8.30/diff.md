# Comparing `tmp/mds_cashbook-6.8.29.tar.gz` & `tmp/mds_cashbook-6.8.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mds_cashbook-6.8.29.tar", last modified: Mon Jul 24 14:36:05 2023, max compression
+gzip compressed data, was "mds_cashbook-6.8.30.tar", last modified: Tue Jul 25 19:15:28 2023, max compression
```

## Comparing `mds_cashbook-6.8.29.tar` & `mds_cashbook-6.8.30.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-24 14:36:05.144850 mds_cashbook-6.8.29/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     7715 2023-07-24 14:36:05.144850 mds_cashbook-6.8.29/PKG-INFO
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     5272 2023-07-24 14:34:56.000000 mds_cashbook-6.8.29/README.rst
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1419 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/__init__.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    20418 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/book.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    25813 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/book.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     5303 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/category.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     6152 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/category.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2243 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/cbreport.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      689 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/cbreport.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     7107 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/configuration.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     3777 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/configuration.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1408 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/currency.py
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-24 14:36:05.136850 mds_cashbook-6.8.29/docs/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      495 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/docs/settings.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1013 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/group.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-24 14:36:05.136850 mds_cashbook-6.8.29/icon/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     3638 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/icon/notebook1.svg
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      431 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/icon.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    42989 2023-07-24 14:33:17.000000 mds_cashbook-6.8.29/line.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    13101 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/line.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-24 14:36:05.136850 mds_cashbook-6.8.29/locale/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    45516 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/locale/de.po
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    42793 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/locale/en.po
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-24 14:36:05.144850 mds_cashbook-6.8.29/mds_cashbook.egg-info/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     7715 2023-07-24 14:36:04.000000 mds_cashbook-6.8.29/mds_cashbook.egg-info/PKG-INFO
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1623 2023-07-24 14:36:05.000000 mds_cashbook-6.8.29/mds_cashbook.egg-info/SOURCES.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-07-24 14:36:04.000000 mds_cashbook-6.8.29/mds_cashbook.egg-info/dependency_links.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       67 2023-07-24 14:36:04.000000 mds_cashbook-6.8.29/mds_cashbook.egg-info/entry_points.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-07-24 14:36:04.000000 mds_cashbook-6.8.29/mds_cashbook.egg-info/not-zip-safe
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      110 2023-07-24 14:36:04.000000 mds_cashbook-6.8.29/mds_cashbook.egg-info/requires.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2023-07-24 14:36:04.000000 mds_cashbook-6.8.29/mds_cashbook.egg-info/top_level.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     5212 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/menu.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     7708 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/message.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     7715 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/mixin.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     9652 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/model.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    18296 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/reconciliation.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     9715 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/reconciliation.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-24 14:36:05.136850 mds_cashbook-6.8.29/report/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    20379 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/report/cashbook.fods
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    52038 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/report/reconciliation.fods
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2023-07-24 14:36:05.144850 mds_cashbook-6.8.29/setup.cfg
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     3760 2023-07-24 14:33:03.000000 mds_cashbook-6.8.29/setup.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    11211 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/splitline.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     6109 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/splitline.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-24 14:36:05.140850 mds_cashbook-6.8.29/tests/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      203 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/tests/__init__.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    24904 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/tests/book.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     6777 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/tests/bookingwiz.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     8328 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/tests/category.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     6679 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/tests/config.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2699 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/tests/currency.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    74460 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/tests/line.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    32358 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/tests/reconciliation.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    15377 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/tests/splitline.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      964 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/tests/test_module.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1551 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/tests/type.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      346 2023-07-24 14:33:46.000000 mds_cashbook-6.8.29/tryton.cfg
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     2124 2023-07-24 14:33:17.000000 mds_cashbook-6.8.29/types.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     3454 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/types.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/versiondep.txt
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-24 14:36:05.144850 mds_cashbook-6.8.29/view/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2491 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/book_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      362 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/book_list.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      451 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/book_tree.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      450 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/cashbook_line_context_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      725 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/category_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      248 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/category_list.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      337 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/category_tree.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      999 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/configuration_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1048 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/enterbooking_start_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1867 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/line_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      583 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/line_list.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      555 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/line_recon_list.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1085 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/recon_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      447 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/recon_list.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      940 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/split_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      578 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/split_list.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      379 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/type_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      298 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/type_list.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      533 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/wizard_openline_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      923 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/view/wizard_runrepbook_form.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     6894 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/wizard_booking.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      745 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/wizard_booking.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     5542 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/wizard_openline.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1614 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/wizard_openline.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     4619 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/wizard_runreport.py
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1221 2023-06-12 07:41:09.000000 mds_cashbook-6.8.29/wizard_runreport.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-25 19:15:28.527940 mds_cashbook-6.8.30/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     7804 2023-07-25 19:15:28.527940 mds_cashbook-6.8.30/PKG-INFO
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     5329 2023-07-25 19:13:48.000000 mds_cashbook-6.8.30/README.rst
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1419 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/__init__.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    20415 2023-07-25 19:12:11.000000 mds_cashbook-6.8.30/book.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    25813 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/book.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     5303 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/category.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     6152 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/category.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2243 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/cbreport.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      689 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/cbreport.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     7107 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/configuration.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     3777 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/configuration.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1408 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/currency.py
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-25 19:15:28.495940 mds_cashbook-6.8.30/docs/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      495 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/docs/settings.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1013 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/group.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-25 19:15:28.495940 mds_cashbook-6.8.30/icon/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     3638 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/icon/notebook1.svg
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      431 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/icon.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    42973 2023-07-25 19:12:11.000000 mds_cashbook-6.8.30/line.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    13101 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/line.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-25 19:15:28.499940 mds_cashbook-6.8.30/locale/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    45516 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/locale/de.po
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    42793 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/locale/en.po
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-25 19:15:28.527940 mds_cashbook-6.8.30/mds_cashbook.egg-info/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     7804 2023-07-25 19:15:28.000000 mds_cashbook-6.8.30/mds_cashbook.egg-info/PKG-INFO
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1623 2023-07-25 19:15:28.000000 mds_cashbook-6.8.30/mds_cashbook.egg-info/SOURCES.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-07-25 19:15:28.000000 mds_cashbook-6.8.30/mds_cashbook.egg-info/dependency_links.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       67 2023-07-25 19:15:28.000000 mds_cashbook-6.8.30/mds_cashbook.egg-info/entry_points.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-07-25 19:15:28.000000 mds_cashbook-6.8.30/mds_cashbook.egg-info/not-zip-safe
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      110 2023-07-25 19:15:28.000000 mds_cashbook-6.8.30/mds_cashbook.egg-info/requires.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2023-07-25 19:15:28.000000 mds_cashbook-6.8.30/mds_cashbook.egg-info/top_level.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     5212 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/menu.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     7708 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/message.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     7715 2023-06-03 11:07:30.000000 mds_cashbook-6.8.30/mixin.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     9652 2023-06-03 11:20:26.000000 mds_cashbook-6.8.30/model.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    18278 2023-07-25 19:12:11.000000 mds_cashbook-6.8.30/reconciliation.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     9715 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/reconciliation.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-25 19:15:28.499940 mds_cashbook-6.8.30/report/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    20379 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/report/cashbook.fods
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    52038 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/report/reconciliation.fods
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2023-07-25 19:15:28.527940 mds_cashbook-6.8.30/setup.cfg
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     3760 2023-07-25 19:11:44.000000 mds_cashbook-6.8.30/setup.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    11227 2023-07-25 19:12:12.000000 mds_cashbook-6.8.30/splitline.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     6109 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/splitline.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-25 19:15:28.515940 mds_cashbook-6.8.30/tests/
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      203 2023-06-02 11:44:06.000000 mds_cashbook-6.8.30/tests/__init__.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    24904 2023-06-02 11:19:01.000000 mds_cashbook-6.8.30/tests/book.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     6777 2023-06-02 11:19:01.000000 mds_cashbook-6.8.30/tests/bookingwiz.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     8328 2023-06-02 11:30:46.000000 mds_cashbook-6.8.30/tests/category.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     6679 2023-06-17 17:28:58.000000 mds_cashbook-6.8.30/tests/config.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     2699 2023-06-02 11:19:01.000000 mds_cashbook-6.8.30/tests/currency.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    74460 2023-06-02 11:31:54.000000 mds_cashbook-6.8.30/tests/line.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    32358 2023-06-02 11:19:01.000000 mds_cashbook-6.8.30/tests/reconciliation.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    16431 2023-07-25 19:12:14.000000 mds_cashbook-6.8.30/tests/splitline.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      964 2023-06-02 10:50:35.000000 mds_cashbook-6.8.30/tests/test_module.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     1551 2023-06-02 10:50:35.000000 mds_cashbook-6.8.30/tests/type.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      346 2023-07-25 19:12:46.000000 mds_cashbook-6.8.30/tryton.cfg
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     2124 2023-06-08 14:31:59.000000 mds_cashbook-6.8.30/types.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     3454 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/types.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)        1 2023-06-05 18:21:23.000000 mds_cashbook-6.8.30/versiondep.txt
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-25 19:15:28.527940 mds_cashbook-6.8.30/view/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2491 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/view/book_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      362 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/view/book_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      451 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/view/book_tree.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      450 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/view/cashbook_line_context_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      725 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/view/category_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      248 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/view/category_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      337 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/view/category_tree.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      999 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/view/configuration_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1048 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/view/enterbooking_start_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1867 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/view/line_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      583 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/view/line_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      555 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/view/line_recon_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1085 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/view/recon_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      447 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/view/recon_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      940 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/view/split_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      578 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/view/split_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      379 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/view/type_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      298 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/view/type_list.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      533 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/view/wizard_openline_form.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      923 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/view/wizard_runrepbook_form.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     6891 2023-07-25 19:12:12.000000 mds_cashbook-6.8.30/wizard_booking.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      745 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/wizard_booking.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     5542 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/wizard_openline.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1614 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/wizard_openline.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     4613 2023-07-25 19:12:12.000000 mds_cashbook-6.8.30/wizard_runreport.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1221 2023-05-24 05:54:15.000000 mds_cashbook-6.8.30/wizard_runreport.xml
```

### Comparing `mds_cashbook-6.8.29/PKG-INFO` & `mds_cashbook-6.8.30/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mds_cashbook
-Version: 6.8.29
+Version: 6.8.30
 Summary: Tryton module to add a cashbook.
 Home-page: https://www.m-ds.de/
 Author: martin-data services
 Author-email: service@m-ds.de
 License: GPL-3
 Download-URL: https://scmdev.m-ds.de/Tryton/Extra/cashbook
 Description: mds-cashbook
@@ -158,14 +158,18 @@
         If you have hierarchical cash books, the amounts of subordinate cash books with foreign
         currency are converted  into the display currency of the parent cash book.
         
         
         Changes
         =======
         
+        *6.8.30 - 25.07.2023*
+        
+        - updt: optimize code, add tests
+        
         *6.8.29 - 24.07.2023*
         
         - fix: type of indexes
         
         *6.8.28 - 05.06.2023*
         
         - init
```

### Comparing `mds_cashbook-6.8.29/README.rst` & `mds_cashbook-6.8.30/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -149,14 +149,18 @@
 If you have hierarchical cash books, the amounts of subordinate cash books with foreign
 currency are converted  into the display currency of the parent cash book.
 
 
 Changes
 =======
 
+*6.8.30 - 25.07.2023*
+
+- updt: optimize code, add tests
+
 *6.8.29 - 24.07.2023*
 
 - fix: type of indexes
 
 *6.8.28 - 05.06.2023*
 
 - init
```

### Comparing `mds_cashbook-6.8.29/__init__.py` & `mds_cashbook-6.8.30/__init__.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/book.py` & `mds_cashbook-6.8.30/book.py`

 * *Files 0% similar despite different names*

```diff
@@ -570,15 +570,15 @@
                 # if owner changes, remove book from user-config
                 if 'owner' in values.keys():
                     if book.owner.id != values['owner']:
                         for x in [
                                 'defbook', 'book1', 'book2', 'book3',
                                 'book4', 'book5']:
                             cfg1 = ConfigUser.search([
-                                    ('iduser.id', '=', book.owner.id),
+                                    ('iduser', '=', book.owner.id),
                                     ('%s.id' % x, '=', book.id)])
                             if len(cfg1) > 0:
                                 to_write_config.extend([cfg1, {x: None}])
         super(Book, cls).write(*args)
 
         if len(to_write_config) > 0:
             ConfigUser.write(*to_write_config)
```

### Comparing `mds_cashbook-6.8.29/book.xml` & `mds_cashbook-6.8.30/book.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/category.py` & `mds_cashbook-6.8.30/category.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/category.xml` & `mds_cashbook-6.8.30/category.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/cbreport.py` & `mds_cashbook-6.8.30/cbreport.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/cbreport.xml` & `mds_cashbook-6.8.30/cbreport.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/configuration.py` & `mds_cashbook-6.8.30/configuration.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/configuration.xml` & `mds_cashbook-6.8.30/configuration.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/currency.py` & `mds_cashbook-6.8.30/currency.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/group.xml` & `mds_cashbook-6.8.30/group.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/icon/notebook1.svg` & `mds_cashbook-6.8.30/icon/notebook1.svg`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/line.py` & `mds_cashbook-6.8.30/line.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 sel_payee = [
     ('cashbook.book', 'Cashbook'),
     ('party.party', 'Party')
     ]
 
-sel_linetype = [
+sel_linestate = [
     ('edit', 'Edit'),
     ('check', 'Checked'),
     ('recon', 'Reconciled'),
     ('done', 'Done'),
     ]
 
 sel_bookingtype = [
@@ -193,15 +193,15 @@
         string="Currency", readonly=True), 'on_change_with_currency')
     currency_digits = fields.Function(fields.Integer(
         string='Currency Digits',
         readonly=True), 'on_change_with_currency_digits')
 
     state = fields.Selection(
         string='State', required=True, readonly=True,
-        selection=sel_linetype)
+        selection=sel_linestate)
     state_string = state.translated('state')
     state_cashbook = fields.Function(fields.Selection(
         string='State of Cashbook',
         readonly=True, states={'invisible': True}, selection=sel_state_book),
         'on_change_with_state_cashbook', searcher='search_state_cashbook')
     owner_cashbook = fields.Function(fields.Many2One(
         string='Owner', readonly=True,
@@ -371,26 +371,26 @@
         to_create_line = []
         to_write_line = []
         for line in lines:
             # deny if date is in range of existing reconciliation
             # allow cashbook-line at range-limits
             if Recon.search_count([
                     ('state', 'in', ['check', 'done']),
-                    ('cashbook.id', '=', line.cashbook.id),
+                    ('cashbook', '=', line.cashbook.id),
                     ('date_from', '<', line.date),
                     ('date_to', '>', line.date)]) > 0:
                 raise UserError(gettext(
                     'cashbook.msg_line_err_write_to_reconciled',
                     datetxt=Report.format_date(line.date),
                     ))
             # deny if date is at reconciliation limits and two
             # reconciliations exist
             if Recon.search_count([
                     ('state', 'in', ['check', 'done']),
-                    ('cashbook.id', '=', line.cashbook.id),
+                    ('cashbook', '=', line.cashbook.id),
                     ['OR',
                         ('date_from', '=', line.date),
                         ('date_to', '=', line.date)]]) > 1:
                 raise UserError(gettext(
                     'cashbook.msg_line_err_write_to_reconciled',
                     datetxt=Report.format_date(line.date),
                     ))
@@ -747,42 +747,42 @@
             """ search last reconciliation in state 'done',
                 generate query
             """
             query2 = []
             end_value = None
 
             recons = Reconciliation.search([
-                ('cashbook.id', '=', line.cashbook.id),
+                ('cashbook', '=', line.cashbook.id),
                 ('date_to', '<=', line2.date),
                 ('state', '=', 'done'),
                 ], order=[('date_from', 'DESC')], limit=1)
             if len(recons) > 0:
                 query2.append([
                         ('date', '>=', recons[0].date_to),
                         ('date', '<=', line2.date),
                         ['OR',
                             ('reconciliation', '=', None),
-                            ('reconciliation.id', '!=', recons[0])],
+                            ('reconciliation', '!=', recons[0])],
                     ])
                 end_value = getattr(recons[0], 'end_%s' % field_name)
             return (query2, end_value)
 
         if line.cashbook:
             query = [
-                ('cashbook.id', '=', line.cashbook.id),
+                ('cashbook', '=', line.cashbook.id),
                 ]
             balance = Decimal('0.0')
 
             # get existing reconciliation, starting before current line
             # this will speed up calculation of by-line-balance
             if line.date is not None:
                 if line.reconciliation:
                     if line.reconciliation.state == 'done':
                         query.append(
-                            ('reconciliation.id', '=', line.reconciliation.id),
+                            ('reconciliation', '=', line.reconciliation.id),
                             )
                         balance = getattr(
                             line.reconciliation, 'start_%s' % field_name)
                     else:
                         (query2, balance2) = get_from_last_recon(line)
                         query.extend(query2)
                         if balance2 is not None:
```

### Comparing `mds_cashbook-6.8.29/line.xml` & `mds_cashbook-6.8.30/line.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/locale/de.po` & `mds_cashbook-6.8.30/locale/de.po`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/locale/en.po` & `mds_cashbook-6.8.30/locale/en.po`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/mds_cashbook.egg-info/PKG-INFO` & `mds_cashbook-6.8.30/mds_cashbook.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mds-cashbook
-Version: 6.8.29
+Version: 6.8.30
 Summary: Tryton module to add a cashbook.
 Home-page: https://www.m-ds.de/
 Author: martin-data services
 Author-email: service@m-ds.de
 License: GPL-3
 Download-URL: https://scmdev.m-ds.de/Tryton/Extra/cashbook
 Description: mds-cashbook
@@ -158,14 +158,18 @@
         If you have hierarchical cash books, the amounts of subordinate cash books with foreign
         currency are converted  into the display currency of the parent cash book.
         
         
         Changes
         =======
         
+        *6.8.30 - 25.07.2023*
+        
+        - updt: optimize code, add tests
+        
         *6.8.29 - 24.07.2023*
         
         - fix: type of indexes
         
         *6.8.28 - 05.06.2023*
         
         - init
```

### Comparing `mds_cashbook-6.8.29/mds_cashbook.egg-info/SOURCES.txt` & `mds_cashbook-6.8.30/mds_cashbook.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/menu.xml` & `mds_cashbook-6.8.30/menu.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/message.xml` & `mds_cashbook-6.8.30/message.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/mixin.py` & `mds_cashbook-6.8.30/mixin.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/model.py` & `mds_cashbook-6.8.30/model.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/reconciliation.py` & `mds_cashbook-6.8.30/reconciliation.py`

 * *Files 4% similar despite different names*

```diff
@@ -179,15 +179,15 @@
         """
         Line = Pool().get('cashbook.line')
 
         for reconciliation in reconciliations:
             if Line.search_count([
                     ('date', '>', reconciliation.date_from),
                     ('date', '<', reconciliation.date_to),
-                    ('cashbook.id', '=', reconciliation.cashbook.id),
+                    ('cashbook', '=', reconciliation.cashbook.id),
                     ('state', 'not in', ['check', 'recon']),
                     ]) > 0:
                 raise UserError(gettext(
                     'cashbook.mds_recon_deny_line_not_check',
                     bookname=reconciliation.cashbook.rec_name,
                     reconame=reconciliation.rec_name,
                     datefrom=Report.format_date(reconciliation.date_from),
@@ -220,15 +220,15 @@
             values['start_amount'] = Decimal('0.0')
         values['end_amount'] = values['start_amount']
 
         # add 'checked'-lines to reconciliation
         lines = Line.search([
             ('date', '>=', reconciliation.date_from),
             ('date', '<=', reconciliation.date_to),
-            ('cashbook.id', '=', reconciliation.cashbook.id),
+            ('cashbook', '=', reconciliation.cashbook.id),
             ('reconciliation', '=', None),
             ('state', 'in', ['check', 'recon']),
             ])
         if len(lines) > 0:
             values['lines'] = [('add', [x.id for x in lines])]
 
         # add amounts of new lines
@@ -311,15 +311,15 @@
                     if x.state == 'check'])
             to_wfdone_line.extend([
                     x for x in reconciliation.lines
                     if x.state == 'recon'])
 
             # deny if there are lines not linked to reconciliation
             if Line.search_count([
-                    ('cashbook.id', '=', reconciliation.cashbook.id),
+                    ('cashbook', '=', reconciliation.cashbook.id),
                     ('reconciliation', '=', None),
                     ['OR',
                         [   # lines inside of date-range
                             ('date', '>', reconciliation.date_from),
                             ('date', '<', reconciliation.date_to),
                         ],
                         # lines at from-date must relate to a reconciliation
@@ -401,15 +401,15 @@
         """ get predecessor
         """
         Recon = Pool().get('cashbook.recon')
 
         if self.cashbook:
             if self.date_from is not None:
                 reconciliations = Recon.search([
-                        ('cashbook.id', '=', self.cashbook.id),
+                        ('cashbook', '=', self.cashbook.id),
                         ('date_from', '<', self.date_from),
                     ], order=[('date_from', 'DESC')], limit=1)
                 if len(reconciliations) > 0:
                     return reconciliations[0].id
 
     @fields.depends('cashbook', '_parent_cashbook.currency')
     def on_change_with_currency(self, name=None):
@@ -453,24 +453,24 @@
         Cashbook = pool.get('cashbook.book')
 
         for values in vlist:
             id_cashbook = values.get('cashbook', -1)
 
             # set date_from to date_to of predecessor
             recons = Recon.search([
-                ('cashbook.id', '=', id_cashbook),
+                ('cashbook', '=', id_cashbook),
                 ], order=[('date_to', 'DESC')], limit=1)
             if len(recons) > 0:
                 values['date_from'] = recons[0].date_to
             elif id_cashbook != -1:
                 values['date_from'] = Cashbook(id_cashbook).start_date
 
             # set date_to to day of last 'checked'-booking in selected cashbook
             lines = Line.search([
-                ('cashbook.id', '=', id_cashbook),
+                ('cashbook', '=', id_cashbook),
                 ('state', '=', 'check'),
                 ('reconciliation', '=', None),
                 ], order=[('date', 'DESC')], limit=1)
             if len(lines) > 0:
                 values['date_to'] = lines[0].date
 
         return super(Reconciliation, cls).create(vlist)
```

### Comparing `mds_cashbook-6.8.29/reconciliation.xml` & `mds_cashbook-6.8.30/reconciliation.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/report/cashbook.fods` & `mds_cashbook-6.8.30/report/cashbook.fods`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/report/reconciliation.fods` & `mds_cashbook-6.8.30/report/reconciliation.fods`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/setup.py` & `mds_cashbook-6.8.30/setup.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/splitline.py` & `mds_cashbook-6.8.30/splitline.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 from trytond.model import ModelView, ModelSQL, fields, Index
 from trytond.pool import Pool
 from trytond.pyson import Eval, If
 from trytond.report import Report
 from trytond.i18n import gettext
-from .line import sel_bookingtype, STATES, DEPENDS
+from .line import sel_bookingtype, sel_linestate, STATES, DEPENDS
 from .book import sel_state_book
 from .mixin import SecondCurrencyMixin, MemCacheIndexMx
 
 
 sel_linetype = [
     ('cat', 'Category'),
     ('tr', 'Transfer'),
@@ -86,15 +86,15 @@
         string='Currency Digits',
         readonly=True), 'on_change_with_currency_digits')
     bookingtype = fields.Function(fields.Selection(
         string='Type', readonly=True,
         selection=sel_bookingtype), 'on_change_with_bookingtype')
     state = fields.Function(fields.Selection(
         string='State', readonly=True,
-        selection=sel_linetype), 'on_change_with_state')
+        selection=sel_linestate), 'on_change_with_state')
     cashbook = fields.Function(fields.Many2One(
         string='Cashbook',
         readonly=True, states={'invisible': True}, model_name='cashbook.book'),
         'on_change_with_cashbook')
     feature = fields.Function(fields.Char(
         string='Feature', readonly=True,
         states={'invisible': True}), 'on_change_with_feature')
```

### Comparing `mds_cashbook-6.8.29/splitline.xml` & `mds_cashbook-6.8.30/splitline.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/tests/book.py` & `mds_cashbook-6.8.30/tests/book.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/tests/bookingwiz.py` & `mds_cashbook-6.8.30/tests/bookingwiz.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/tests/category.py` & `mds_cashbook-6.8.30/tests/category.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/tests/config.py` & `mds_cashbook-6.8.30/tests/config.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/tests/currency.py` & `mds_cashbook-6.8.30/tests/currency.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/tests/line.py` & `mds_cashbook-6.8.30/tests/line.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/tests/reconciliation.py` & `mds_cashbook-6.8.30/tests/reconciliation.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/tests/splitline.py` & `mds_cashbook-6.8.30/tests/splitline.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,14 +69,34 @@
         self.assertEqual(
             book.lines[0].splitlines[0].rec_name,
             'Rev/Sp|5.00 usd|from category [Cat1]')
         self.assertEqual(
             book.lines[0].splitlines[1].rec_name,
             'Rev/Sp|6.00 usd|from cashbook [Cat1]')
 
+        # check function fields
+        self.assertEqual(
+            book.lines[0].splitlines[0].category_view,
+            'Cat1')
+        self.assertEqual(book.lines[0].splitlines[0].date, date(2022, 5, 1))
+        self.assertEqual(book.lines[0].splitlines[0].target.rec_name, 'Cat1')
+        self.assertEqual(book.lines[0].splitlines[0].currency.rec_name, 'usd')
+        self.assertEqual(book.lines[0].splitlines[0].currency_digits, 2)
+        self.assertEqual(book.lines[0].splitlines[0].bookingtype, 'spin')
+        self.assertEqual(book.lines[0].splitlines[0].state, 'edit')
+        self.assertEqual(
+            book.lines[0].splitlines[0].cashbook.rec_name,
+            'Book 1 | 11.00 usd | Open')
+        self.assertEqual(book.lines[0].splitlines[0].feature, 'gen')
+        self.assertEqual(book.lines[0].splitlines[0].booktransf_feature, None)
+        self.assertEqual(book.lines[0].splitlines[0].state_cashbook, 'open')
+        self.assertEqual(
+            book.lines[0].splitlines[0].owner_cashbook.rec_name,
+            'Administrator')
+
     @with_transaction()
     def test_splitline_category_and_transfer(self):
         """ add book, line, two split-lines,
             category + transfer
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
```

### Comparing `mds_cashbook-6.8.29/tests/test_module.py` & `mds_cashbook-6.8.30/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/tests/type.py` & `mds_cashbook-6.8.30/tests/type.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/types.py` & `mds_cashbook-6.8.30/types.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/types.xml` & `mds_cashbook-6.8.30/types.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/view/book_form.xml` & `mds_cashbook-6.8.30/view/book_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/view/category_form.xml` & `mds_cashbook-6.8.30/view/category_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/view/configuration_form.xml` & `mds_cashbook-6.8.30/view/configuration_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/view/enterbooking_start_form.xml` & `mds_cashbook-6.8.30/view/enterbooking_start_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/view/line_form.xml` & `mds_cashbook-6.8.30/view/line_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/view/line_list.xml` & `mds_cashbook-6.8.30/view/line_list.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/view/line_recon_list.xml` & `mds_cashbook-6.8.30/view/line_recon_list.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/view/recon_form.xml` & `mds_cashbook-6.8.30/view/recon_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/view/split_form.xml` & `mds_cashbook-6.8.30/view/split_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/view/split_list.xml` & `mds_cashbook-6.8.30/view/split_list.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/view/wizard_openline_form.xml` & `mds_cashbook-6.8.30/view/wizard_openline_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/view/wizard_runrepbook_form.xml` & `mds_cashbook-6.8.30/view/wizard_runrepbook_form.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/wizard_booking.py` & `mds_cashbook-6.8.30/wizard_booking.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
             if getattr(cfg1, x, None) is not None:
                 book_ids.append(getattr(cfg1, x, None).id)
 
         result = {
             'cashbooks': [x.id for x in Cashbook.search([
                     ('state', '=', 'open'),
                     ('btype', '!=', None),
-                    ('owner.id', '=', Transaction().user),
+                    ('owner', '=', Transaction().user),
                     ('id', 'in', book_ids),
                 ])],
             'bookingtype': getattr(self.start, 'bookingtype', 'out'),
             'cashbook': getattr(getattr(cfg1, 'defbook', None), 'id', None),
             'amount': None,
             'party': None,
             'booktransf': None,
```

### Comparing `mds_cashbook-6.8.29/wizard_booking.xml` & `mds_cashbook-6.8.30/wizard_booking.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/wizard_openline.py` & `mds_cashbook-6.8.30/wizard_openline.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/wizard_openline.xml` & `mds_cashbook-6.8.30/wizard_openline.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook-6.8.29/wizard_runreport.py` & `mds_cashbook-6.8.30/wizard_runreport.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     def on_change_with_reconciliations(self, name=None):
         """ get reconciliations of current cashbook
         """
         Recon2 = Pool().get('cashbook.recon')
 
         if self.cashbook:
             recons = Recon2.search([
-                ('cashbook.id', '=', self.cashbook.id),
+                ('cashbook', '=', self.cashbook.id),
                 ], order=[('date_from', 'DESC')])
             return [x.id for x in recons]
 
 # end RunCbReportStart
 
 
 class RunCbReport(Wizard):
@@ -99,15 +99,15 @@
             result['cashbooks'] = [x.id for x in books]
 
             if len(result['cashbooks']) > 0:
                 if result['cashbook'] is None:
                     result['cashbook'] = result['cashbooks'][0]
 
             recons = Recon2.search([
-                ('cashbook.id', '=', result['cashbook']),
+                ('cashbook', '=', result['cashbook']),
                 ], order=[('date_from', 'DESC')])
             if len(recons) > 0:
                 result['reconciliations'] = [x.id for x in recons]
                 result['reconciliation'] = recons[0].id
         return result
 
     def do_report_(self, action):
```

### Comparing `mds_cashbook-6.8.29/wizard_runreport.xml` & `mds_cashbook-6.8.30/wizard_runreport.xml`

 * *Files identical despite different names*

