# Comparing `tmp/cubicweb-workcase-0.8.0.tar.gz` & `tmp/cubicweb-workcase-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cubicweb-workcase-0.8.0.tar", last modified: Thu May 16 11:48:27 2019, max compression
+gzip compressed data, was "cubicweb-workcase-1.0.0.tar", last modified: Tue Jul 25 10:25:40 2023, max compression
```

## Comparing `cubicweb-workcase-0.8.0.tar` & `cubicweb-workcase-1.0.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-05-16 11:48:27.000000 cubicweb-workcase-0.8.0/
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      333 2019-05-16 11:47:39.000000 cubicweb-workcase-0.8.0/MANIFEST.in
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      565 2019-05-16 11:48:27.000000 cubicweb-workcase-0.8.0/PKG-INFO
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      110 2019-03-06 10:03:26.000000 cubicweb-workcase-0.8.0/README
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-05-16 11:48:27.000000 cubicweb-workcase-0.8.0/cubicweb_workcase/
--rw-------   0 ppepiot   (1000) ppepiot   (1000)       24 2019-03-15 14:28:18.000000 cubicweb-workcase-0.8.0/cubicweb_workcase/__init__.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      652 2019-05-16 11:47:59.000000 cubicweb-workcase-0.8.0/cubicweb_workcase/__pkginfo__.py
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-05-16 11:48:27.000000 cubicweb-workcase-0.8.0/cubicweb_workcase/data/
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      276 2019-03-15 14:28:18.000000 cubicweb-workcase-0.8.0/cubicweb_workcase/data/icon_workcase.gif
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      792 2019-03-15 15:34:49.000000 cubicweb-workcase-0.8.0/cubicweb_workcase/entities.py
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-05-16 11:48:27.000000 cubicweb-workcase-0.8.0/cubicweb_workcase/i18n/
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     2510 2019-03-15 14:28:18.000000 cubicweb-workcase-0.8.0/cubicweb_workcase/i18n/en.po
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     2497 2019-03-15 14:28:18.000000 cubicweb-workcase-0.8.0/cubicweb_workcase/i18n/fr.po
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-05-16 11:48:27.000000 cubicweb-workcase-0.8.0/cubicweb_workcase/migration/
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      664 2019-03-15 14:28:18.000000 cubicweb-workcase-0.8.0/cubicweb_workcase/migration/0.5.1_Any.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     1155 2019-03-15 14:28:18.000000 cubicweb-workcase-0.8.0/cubicweb_workcase/migration/postcreate.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)       63 2019-03-15 14:28:18.000000 cubicweb-workcase-0.8.0/cubicweb_workcase/migration/postreinitialize.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      650 2019-03-15 14:28:18.000000 cubicweb-workcase-0.8.0/cubicweb_workcase/schema.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     1719 2019-03-15 15:34:49.000000 cubicweb-workcase-0.8.0/cubicweb_workcase/sobjects.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)       56 2019-03-15 14:28:18.000000 cubicweb-workcase-0.8.0/cubicweb_workcase/uiprops.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      581 2019-03-15 14:28:18.000000 cubicweb-workcase-0.8.0/cubicweb_workcase/views.py
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-05-16 11:48:27.000000 cubicweb-workcase-0.8.0/cubicweb_workcase/wdoc/
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      133 2019-03-15 14:28:18.000000 cubicweb-workcase-0.8.0/cubicweb_workcase/wdoc/ChangeLog_en
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      130 2019-03-15 14:28:18.000000 cubicweb-workcase-0.8.0/cubicweb_workcase/wdoc/ChangeLog_fr
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-05-16 11:48:27.000000 cubicweb-workcase-0.8.0/cubicweb_workcase.egg-info/
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      565 2019-05-16 11:48:27.000000 cubicweb-workcase-0.8.0/cubicweb_workcase.egg-info/PKG-INFO
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      924 2019-05-16 11:48:27.000000 cubicweb-workcase-0.8.0/cubicweb_workcase.egg-info/SOURCES.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)        1 2019-05-16 11:48:27.000000 cubicweb-workcase-0.8.0/cubicweb_workcase.egg-info/dependency_links.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       47 2019-05-16 11:48:27.000000 cubicweb-workcase-0.8.0/cubicweb_workcase.egg-info/entry_points.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)        1 2019-05-16 11:48:27.000000 cubicweb-workcase-0.8.0/cubicweb_workcase.egg-info/not-zip-safe
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       17 2019-05-16 11:48:27.000000 cubicweb-workcase-0.8.0/cubicweb_workcase.egg-info/requires.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       18 2019-05-16 11:48:27.000000 cubicweb-workcase-0.8.0/cubicweb_workcase.egg-info/top_level.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)        7 2019-05-16 11:46:59.000000 cubicweb-workcase-0.8.0/dev-requirements.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       38 2019-05-16 11:48:27.000000 cubicweb-workcase-0.8.0/setup.cfg
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     2629 2019-03-15 14:28:18.000000 cubicweb-workcase-0.8.0/setup.py
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-05-16 11:48:27.000000 cubicweb-workcase-0.8.0/test/
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-05-16 11:48:27.000000 cubicweb-workcase-0.8.0/test/data/
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)        9 2019-03-06 10:03:26.000000 cubicweb-workcase-0.8.0/test/data/bootstrap_cubes
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      329 2019-03-15 15:34:49.000000 cubicweb-workcase-0.8.0/test/test_workcase.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     2608 2019-03-15 15:34:49.000000 cubicweb-workcase-0.8.0/test/unittest_hooks.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      514 2019-05-16 11:46:53.000000 cubicweb-workcase-0.8.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:25:40.100807 cubicweb-workcase-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      431 2023-07-25 10:25:18.000000 cubicweb-workcase-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      518 2023-07-25 10:25:40.100807 cubicweb-workcase-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-07-25 10:25:18.000000 cubicweb-workcase-1.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:25:40.088806 cubicweb-workcase-1.0.0/cubicweb_workcase/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-25 10:25:18.000000 cubicweb-workcase-1.0.0/cubicweb_workcase/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      658 2023-07-25 10:25:18.000000 cubicweb-workcase-1.0.0/cubicweb_workcase/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:25:40.096807 cubicweb-workcase-1.0.0/cubicweb_workcase/data/
+-rw-rw-rw-   0 root         (0) root         (0)      276 2023-07-25 10:25:18.000000 cubicweb-workcase-1.0.0/cubicweb_workcase/data/icon_workcase.gif
+-rw-rw-rw-   0 root         (0) root         (0)      792 2023-07-25 10:25:18.000000 cubicweb-workcase-1.0.0/cubicweb_workcase/entities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:25:40.096807 cubicweb-workcase-1.0.0/cubicweb_workcase/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)     2510 2023-07-25 10:25:18.000000 cubicweb-workcase-1.0.0/cubicweb_workcase/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)     2497 2023-07-25 10:25:18.000000 cubicweb-workcase-1.0.0/cubicweb_workcase/i18n/fr.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:25:40.096807 cubicweb-workcase-1.0.0/cubicweb_workcase/migration/
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-25 10:25:18.000000 cubicweb-workcase-1.0.0/cubicweb_workcase/migration/0.5.1_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)     1155 2023-07-25 10:25:18.000000 cubicweb-workcase-1.0.0/cubicweb_workcase/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-25 10:25:18.000000 cubicweb-workcase-1.0.0/cubicweb_workcase/migration/postreinitialize.py
+-rw-rw-rw-   0 root         (0) root         (0)      650 2023-07-25 10:25:18.000000 cubicweb-workcase-1.0.0/cubicweb_workcase/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1719 2023-07-25 10:25:18.000000 cubicweb-workcase-1.0.0/cubicweb_workcase/sobjects.py
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-07-25 10:25:18.000000 cubicweb-workcase-1.0.0/cubicweb_workcase/uiprops.py
+-rw-rw-rw-   0 root         (0) root         (0)      581 2023-07-25 10:25:18.000000 cubicweb-workcase-1.0.0/cubicweb_workcase/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:25:40.100807 cubicweb-workcase-1.0.0/cubicweb_workcase/wdoc/
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-07-25 10:25:18.000000 cubicweb-workcase-1.0.0/cubicweb_workcase/wdoc/ChangeLog_en
+-rw-rw-rw-   0 root         (0) root         (0)      130 2023-07-25 10:25:18.000000 cubicweb-workcase-1.0.0/cubicweb_workcase/wdoc/ChangeLog_fr
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:25:40.092807 cubicweb-workcase-1.0.0/cubicweb_workcase.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      518 2023-07-25 10:25:39.000000 cubicweb-workcase-1.0.0/cubicweb_workcase.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      928 2023-07-25 10:25:39.000000 cubicweb-workcase-1.0.0/cubicweb_workcase.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 10:25:39.000000 cubicweb-workcase-1.0.0/cubicweb_workcase.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-07-25 10:25:39.000000 cubicweb-workcase-1.0.0/cubicweb_workcase.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 10:25:39.000000 cubicweb-workcase-1.0.0/cubicweb_workcase.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-25 10:25:39.000000 cubicweb-workcase-1.0.0/cubicweb_workcase.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-25 10:25:39.000000 cubicweb-workcase-1.0.0/cubicweb_workcase.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-25 10:25:18.000000 cubicweb-workcase-1.0.0/dev-requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 10:25:40.100807 cubicweb-workcase-1.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2633 2023-07-25 10:25:18.000000 cubicweb-workcase-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:25:40.100807 cubicweb-workcase-1.0.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:25:40.100807 cubicweb-workcase-1.0.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       13 2023-07-25 10:25:18.000000 cubicweb-workcase-1.0.0/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)      333 2023-07-25 10:25:18.000000 cubicweb-workcase-1.0.0/test/test_workcase.py
+-rw-rw-rw-   0 root         (0) root         (0)     2608 2023-07-25 10:25:18.000000 cubicweb-workcase-1.0.0/test/unittest_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1822 2023-07-25 10:25:18.000000 cubicweb-workcase-1.0.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cubicweb-workcase-0.8.0/PKG-INFO` & `cubicweb-workcase-1.0.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: cubicweb-workcase
-Version: 0.8.0
+Version: 1.0.0
 Summary: workcase component for the CubicWeb framework
 Home-page: http://www.cubicweb.org/project/cubicweb-workcase
 Author: Logilab
 Author-email: contact@logilab.fr
 License: LGPL
-Description: This CubicWeb component models workcase and workpackages
-        (a workcase can be split into several workpackages).
-        
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: JavaScript
+
+This CubicWeb component models workcase and workpackages
+(a workcase can be split into several workpackages).
```

### Comparing `cubicweb-workcase-0.8.0/cubicweb_workcase/__pkginfo__.py` & `cubicweb-workcase-1.0.0/cubicweb_workcase/__pkginfo__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # pylint: disable-msg=W0622
 """cubicweb-workcase application packaging information"""
 
 modname = 'workcase'
 distname = "cubicweb-%s" % modname
 
-numversion = (0, 8, 0)
+numversion = (1, 0, 0)
 version = '.'.join(str(num) for num in numversion)
 
 license = 'LGPL'
 description = "workcase component for the CubicWeb framework"
 author = "Logilab"
 author_email = "contact@logilab.fr"
 web = 'http://www.cubicweb.org/project/%s' % distname
 classifiers = [
            'Environment :: Web Environment',
            'Framework :: CubicWeb',
            'Programming Language :: Python',
            'Programming Language :: JavaScript',
            ]
 
-__depends__ = {'cubicweb': '>= 3.24.0'}
+__depends__ = {'cubicweb': '>= 4.0.0,<5.0.0'}
```

### Comparing `cubicweb-workcase-0.8.0/cubicweb_workcase/entities.py` & `cubicweb-workcase-1.0.0/cubicweb_workcase/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-workcase-0.8.0/cubicweb_workcase/i18n/en.po` & `cubicweb-workcase-1.0.0/cubicweb_workcase/i18n/en.po`

 * *Files identical despite different names*

### Comparing `cubicweb-workcase-0.8.0/cubicweb_workcase/i18n/fr.po` & `cubicweb-workcase-1.0.0/cubicweb_workcase/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `cubicweb-workcase-0.8.0/cubicweb_workcase/migration/0.5.1_Any.py` & `cubicweb-workcase-1.0.0/cubicweb_workcase/migration/0.5.1_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-workcase-0.8.0/cubicweb_workcase/migration/postcreate.py` & `cubicweb-workcase-1.0.0/cubicweb_workcase/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-workcase-0.8.0/cubicweb_workcase/schema.py` & `cubicweb-workcase-1.0.0/cubicweb_workcase/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-workcase-0.8.0/cubicweb_workcase/sobjects.py` & `cubicweb-workcase-1.0.0/cubicweb_workcase/sobjects.py`

 * *Files identical despite different names*

### Comparing `cubicweb-workcase-0.8.0/cubicweb_workcase/views.py` & `cubicweb-workcase-1.0.0/cubicweb_workcase/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """template-specific forms/views/actions/components"""
 
 from cubicweb.predicates import is_instance
-from cubicweb.web.views import ibreadcrumbs, uicfg
+from cubicweb_web.views import ibreadcrumbs, uicfg
 
 _abaa = uicfg.actionbox_appearsin_addmenu
 _abaa.tag_subject_of(('Workcase', 'split_into', 'Workpackage'), True)
 _abaa.tag_object_of(('Workcase', 'split_into', 'Workpackage'), False)
 
 
 class WorkPackageIBreadCrumbsAdapter(ibreadcrumbs.IBreadCrumbsAdapter):
```

### Comparing `cubicweb-workcase-0.8.0/cubicweb_workcase.egg-info/PKG-INFO` & `cubicweb-workcase-1.0.0/cubicweb_workcase.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: cubicweb-workcase
-Version: 0.8.0
+Version: 1.0.0
 Summary: workcase component for the CubicWeb framework
 Home-page: http://www.cubicweb.org/project/cubicweb-workcase
 Author: Logilab
 Author-email: contact@logilab.fr
 License: LGPL
-Description: This CubicWeb component models workcase and workpackages
-        (a workcase can be split into several workpackages).
-        
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: JavaScript
+
+This CubicWeb component models workcase and workpackages
+(a workcase can be split into several workpackages).
```

### Comparing `cubicweb-workcase-0.8.0/cubicweb_workcase.egg-info/SOURCES.txt` & `cubicweb-workcase-1.0.0/cubicweb_workcase.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 MANIFEST.in
-README
+README.rst
 dev-requirements.txt
 setup.py
 tox.ini
 cubicweb_workcase/__init__.py
 cubicweb_workcase/__pkginfo__.py
 cubicweb_workcase/entities.py
 cubicweb_workcase/schema.py
```

### Comparing `cubicweb-workcase-0.8.0/setup.py` & `cubicweb-workcase-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # pylint: disable=W0142,W0403,W0404,W0613,W0622,W0622,W0704,R0904,C0103,E0611
 #
-# copyright 2003-2018 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2003-2021 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr/ -- mailto:contact@logilab.fr
 #
 # This file is part of cubiweb-workcase.
 #
 # CubicWeb is free software: you can redistribute it and/or modify it under the
 # terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
@@ -43,15 +43,15 @@
 license = __pkginfo__['license']
 description = __pkginfo__['description']
 web = __pkginfo__['web']
 author = __pkginfo__['author']
 author_email = __pkginfo__['author_email']
 classifiers = __pkginfo__['classifiers']
 
-with open(join(here, 'README')) as f:
+with open(join(here, 'README.rst')) as f:
     long_description = f.read()
 
 # get optional metadatas
 data_files = __pkginfo__.get('data_files', None)
 dependency_links = __pkginfo__.get('dependency_links', ())
 
 requires = {}
```

### Comparing `cubicweb-workcase-0.8.0/test/unittest_hooks.py` & `cubicweb-workcase-1.0.0/test/unittest_hooks.py`

 * *Files identical despite different names*

