# Comparing `tmp/cubicweb-blog-2.2.0.tar.gz` & `tmp/cubicweb-blog-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-blog-2.2.0.tar", last modified: Thu Jun 15 13:19:26 2023, max compression
+gzip compressed data, was "cubicweb-blog-3.0.0.tar", last modified: Tue Jul 25 08:46:09 2023, max compression
```

## Comparing `cubicweb-blog-2.2.0.tar` & `cubicweb-blog-3.0.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:19:26.139096 cubicweb-blog-2.2.0/
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2898 2023-06-15 13:19:26.139096 cubicweb-blog-2.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2481 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:19:26.127096 cubicweb-blog-2.2.0/cubicweb_blog/
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      918 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:19:26.131096 cubicweb-blog-2.2.0/cubicweb_blog/data/
--rw-rw-rw-   0 root         (0) root         (0)      831 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/data/cubes.blog.css
--rw-rw-rw-   0 root         (0) root         (0)      276 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/data/icon_blog.gif
--rw-rw-rw-   0 root         (0) root         (0)      868 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/data/postdatabg.jpg
--rw-rw-rw-   0 root         (0) root         (0)     8283 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/entities.py
--rw-rw-rw-   0 root         (0) root         (0)      503 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:19:26.131096 cubicweb-blog-2.2.0/cubicweb_blog/i18n/
--rw-rw-rw-   0 root         (0) root         (0)     5555 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)     4787 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)     5795 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/i18n/fr.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:19:26.135095 cubicweb-blog-2.2.0/cubicweb_blog/migration/
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/migration/1.2.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/migration/1.4.2_Any.py
--rw-rw-rw-   0 root         (0) root         (0)       86 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/migration/1.5.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/migration/1.7.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/migration/1.7.2_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/migration/1.7.3_Any.py
--rw-rw-rw-   0 root         (0) root         (0)       94 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/migration/1.9.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      398 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)     1899 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      257 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/site_cubicweb.py
--rw-rw-rw-   0 root         (0) root         (0)     8017 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/sobjects.py
--rw-rw-rw-   0 root         (0) root         (0)       42 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/uiprops.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:19:26.135095 cubicweb-blog-2.2.0/cubicweb_blog/views/
--rw-rw-rw-   0 root         (0) root         (0)     2680 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/views/blog.py
--rw-rw-rw-   0 root         (0) root         (0)     6377 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/views/boxes.py
--rw-rw-rw-   0 root         (0) root         (0)    10421 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/views/entry.py
--rw-rw-rw-   0 root         (0) root         (0)     2694 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/cubicweb_blog/views/urlpublishing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:19:26.127096 cubicweb-blog-2.2.0/cubicweb_blog.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2898 2023-06-15 13:19:26.000000 cubicweb-blog-2.2.0/cubicweb_blog.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1224 2023-06-15 13:19:26.000000 cubicweb-blog-2.2.0/cubicweb_blog.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 13:19:26.000000 cubicweb-blog-2.2.0/cubicweb_blog.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 13:19:26.000000 cubicweb-blog-2.2.0/cubicweb_blog.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 13:19:26.000000 cubicweb-blog-2.2.0/cubicweb_blog.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       57 2023-06-15 13:19:26.000000 cubicweb-blog-2.2.0/cubicweb_blog.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-15 13:19:26.000000 cubicweb-blog-2.2.0/cubicweb_blog.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/dev-requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 13:19:26.139096 cubicweb-blog-2.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2594 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:19:26.139096 cubicweb-blog-2.2.0/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:19:26.139096 cubicweb-blog-2.2.0/test/data/
--rw-rw-rw-   0 root         (0) root         (0)       10 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/test/data/bootstrap_cubes
--rw-rw-rw-   0 root         (0) root         (0)      321 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/test/test_blog.py
--rw-rw-rw-   0 root         (0) root         (0)     2754 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/test/unittest_blog.py
--rw-rw-rw-   0 root         (0) root         (0)     1248 2023-06-15 13:18:59.000000 cubicweb-blog-2.2.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:46:09.832096 cubicweb-blog-3.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-07-25 08:45:43.000000 cubicweb-blog-3.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2898 2023-07-25 08:46:09.832096 cubicweb-blog-3.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2481 2023-07-25 08:45:43.000000 cubicweb-blog-3.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:46:09.808096 cubicweb-blog-3.0.0/cubicweb_blog/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-07-25 08:45:43.000000 cubicweb-blog-3.0.0/cubicweb_blog/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      962 2023-07-25 08:45:43.000000 cubicweb-blog-3.0.0/cubicweb_blog/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:46:09.816096 cubicweb-blog-3.0.0/cubicweb_blog/data/
+-rw-rw-rw-   0 root         (0) root         (0)      831 2023-07-25 08:45:43.000000 cubicweb-blog-3.0.0/cubicweb_blog/data/cubes.blog.css
+-rw-rw-rw-   0 root         (0) root         (0)      276 2023-07-25 08:45:43.000000 cubicweb-blog-3.0.0/cubicweb_blog/data/icon_blog.gif
+-rw-rw-rw-   0 root         (0) root         (0)      868 2023-07-25 08:45:43.000000 cubicweb-blog-3.0.0/cubicweb_blog/data/postdatabg.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     8283 2023-07-25 08:45:43.000000 cubicweb-blog-3.0.0/cubicweb_blog/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      503 2023-07-25 08:45:43.000000 cubicweb-blog-3.0.0/cubicweb_blog/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:46:09.820096 cubicweb-blog-3.0.0/cubicweb_blog/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)     5555 2023-07-25 08:45:43.000000 cubicweb-blog-3.0.0/cubicweb_blog/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)     4787 2023-07-25 08:45:43.000000 cubicweb-blog-3.0.0/cubicweb_blog/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)     5795 2023-07-25 08:45:43.000000 cubicweb-blog-3.0.0/cubicweb_blog/i18n/fr.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:46:09.824096 cubicweb-blog-3.0.0/cubicweb_blog/migration/
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-25 08:45:43.000000 cubicweb-blog-3.0.0/cubicweb_blog/migration/1.2.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-25 08:45:43.000000 cubicweb-blog-3.0.0/cubicweb_blog/migration/1.4.2_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       86 2023-07-25 08:45:43.000000 cubicweb-blog-3.0.0/cubicweb_blog/migration/1.5.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-07-25 08:45:43.000000 cubicweb-blog-3.0.0/cubicweb_blog/migration/1.7.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-25 08:45:44.000000 cubicweb-blog-3.0.0/cubicweb_blog/migration/1.7.2_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-07-25 08:45:44.000000 cubicweb-blog-3.0.0/cubicweb_blog/migration/1.7.3_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       94 2023-07-25 08:45:44.000000 cubicweb-blog-3.0.0/cubicweb_blog/migration/1.9.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      398 2023-07-25 08:45:44.000000 cubicweb-blog-3.0.0/cubicweb_blog/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1899 2023-07-25 08:45:44.000000 cubicweb-blog-3.0.0/cubicweb_blog/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      257 2023-07-25 08:45:44.000000 cubicweb-blog-3.0.0/cubicweb_blog/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)     8013 2023-07-25 08:45:44.000000 cubicweb-blog-3.0.0/cubicweb_blog/sobjects.py
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-07-25 08:45:44.000000 cubicweb-blog-3.0.0/cubicweb_blog/uiprops.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:46:09.828096 cubicweb-blog-3.0.0/cubicweb_blog/views/
+-rw-rw-rw-   0 root         (0) root         (0)     2680 2023-07-25 08:45:44.000000 cubicweb-blog-3.0.0/cubicweb_blog/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2251 2023-07-25 08:45:44.000000 cubicweb-blog-3.0.0/cubicweb_blog/views/blog.py
+-rw-rw-rw-   0 root         (0) root         (0)     6373 2023-07-25 08:45:44.000000 cubicweb-blog-3.0.0/cubicweb_blog/views/boxes.py
+-rw-rw-rw-   0 root         (0) root         (0)    10285 2023-07-25 08:45:44.000000 cubicweb-blog-3.0.0/cubicweb_blog/views/entry.py
+-rw-rw-rw-   0 root         (0) root         (0)     2694 2023-07-25 08:45:44.000000 cubicweb-blog-3.0.0/cubicweb_blog/views/urlpublishing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:46:09.816096 cubicweb-blog-3.0.0/cubicweb_blog.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2898 2023-07-25 08:46:09.000000 cubicweb-blog-3.0.0/cubicweb_blog.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1224 2023-07-25 08:46:09.000000 cubicweb-blog-3.0.0/cubicweb_blog.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 08:46:09.000000 cubicweb-blog-3.0.0/cubicweb_blog.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 08:46:09.000000 cubicweb-blog-3.0.0/cubicweb_blog.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 08:46:09.000000 cubicweb-blog-3.0.0/cubicweb_blog.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       89 2023-07-25 08:46:09.000000 cubicweb-blog-3.0.0/cubicweb_blog.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-25 08:46:09.000000 cubicweb-blog-3.0.0/cubicweb_blog.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-25 08:45:44.000000 cubicweb-blog-3.0.0/dev-requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 08:46:09.832096 cubicweb-blog-3.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2578 2023-07-25 08:45:44.000000 cubicweb-blog-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:46:09.832096 cubicweb-blog-3.0.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:46:09.832096 cubicweb-blog-3.0.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       10 2023-07-25 08:45:44.000000 cubicweb-blog-3.0.0/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-07-25 08:45:44.000000 cubicweb-blog-3.0.0/test/test_blog.py
+-rw-rw-rw-   0 root         (0) root         (0)     2789 2023-07-25 08:45:44.000000 cubicweb-blog-3.0.0/test/unittest_blog.py
+-rw-rw-rw-   0 root         (0) root         (0)     1258 2023-07-25 08:45:44.000000 cubicweb-blog-3.0.0/tox.ini
```

### Comparing `cubicweb-blog-2.2.0/PKG-INFO` & `cubicweb-blog-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubicweb-blog
-Version: 2.2.0
+Version: 3.0.0
 Summary: blogging component for the CubicWeb framework
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-blog
 Author: Logilab
 Author-email: contact@logilab.fr
 License: LGPL
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
```

### Comparing `cubicweb-blog-2.2.0/README.rst` & `cubicweb-blog-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-blog-2.2.0/cubicweb_blog/data/cubes.blog.css` & `cubicweb-blog-3.0.0/cubicweb_blog/data/cubes.blog.css`

 * *Files identical despite different names*

### Comparing `cubicweb-blog-2.2.0/cubicweb_blog/data/postdatabg.jpg` & `cubicweb-blog-3.0.0/cubicweb_blog/data/postdatabg.jpg`

 * *Files identical despite different names*

### Comparing `cubicweb-blog-2.2.0/cubicweb_blog/entities.py` & `cubicweb-blog-3.0.0/cubicweb_blog/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-blog-2.2.0/cubicweb_blog/i18n/en.po` & `cubicweb-blog-3.0.0/cubicweb_blog/i18n/en.po`

 * *Files identical despite different names*

### Comparing `cubicweb-blog-2.2.0/cubicweb_blog/i18n/es.po` & `cubicweb-blog-3.0.0/cubicweb_blog/i18n/es.po`

 * *Files identical despite different names*

### Comparing `cubicweb-blog-2.2.0/cubicweb_blog/i18n/fr.po` & `cubicweb-blog-3.0.0/cubicweb_blog/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `cubicweb-blog-2.2.0/cubicweb_blog/migration/1.7.0_Any.py` & `cubicweb-blog-3.0.0/cubicweb_blog/migration/1.7.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-blog-2.2.0/cubicweb_blog/schema.py` & `cubicweb-blog-3.0.0/cubicweb_blog/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-blog-2.2.0/cubicweb_blog/sobjects.py` & `cubicweb-blog-3.0.0/cubicweb_blog/sobjects.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
 
 
 def search_twitter(word):
     import urllib2
     from simplejson import loads
 
     data = urllib2.urlopen(
-        "http://search.twitter.com/search.json?q=%s&rpp=100" % word
+        f"http://search.twitter.com/search.json?q={word}&rpp=100"
     ).read()
     loads(data)
     # process results
     # print results
     return []
 
 
@@ -180,15 +180,15 @@
 
 def get_twitter_avatar(screen_name):
     if screen_name not in AVATAR_CACHE:
         from urllib2 import urlopen
         import simplejson
 
         data = urlopen(
-            "http://api.twitter.com/1/users/show.json?screen_name=%s" % screen_name
+            f"http://api.twitter.com/1/users/show.json?screen_name={screen_name}"
         ).read()
         user = simplejson.loads(data)
         AVATAR_CACHE[screen_name] = user["profile_image_url"]
     return AVATAR_CACHE[screen_name]
 
 
 if DataFeedParser is not None:
```

### Comparing `cubicweb-blog-2.2.0/cubicweb_blog/views/__init__.py` & `cubicweb-blog-3.0.0/cubicweb_blog/views/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-blog-2.2.0/cubicweb_blog/views/blog.py` & `cubicweb-blog-3.0.0/cubicweb_blog/views/blog.py`

 * *Files identical despite different names*

### Comparing `cubicweb-blog-2.2.0/cubicweb_blog/views/boxes.py` & `cubicweb-blog-3.0.0/cubicweb_blog/views/boxes.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,15 +131,15 @@
     def render_body(self, w):
         # XXX turn into a predicate
         rset = self.latest_blogs_rset()
         if not rset:
             return
         w('<ul class="boxListing">')
         for entity in rset.entities():
-            w("<li>%s</li>\n" % tags.a(entity.dc_title(), href=entity.absolute_url()))
+            w(f"<li>{tags.a(entity.dc_title(), href=entity.absolute_url())}</li>\n")
         rqlst = rset.syntax_tree()
         rqlst.set_limit(None)
         rql = rqlst.as_string(kwargs=rset.args)
         if self.display_see_more_link:
             url = self._cw.build_url("view", rql=rql, page_size=10)
             w("<li>%s</li>\n" % tags.a("[%s]" % self._cw._("see more"), href=url))
         rss_icon = self._cw.uiprops["RSS_LOGO_16"]
@@ -150,15 +150,15 @@
             self._cw._("rss icon"),
         )
         blogs = self._cw.execute("Any B,RSS WHERE B is Blog, B rss_url RSS")
         if len(blogs) == 1:
             rss_url = blogs[0][1]
         else:
             rss_url = self._cw.build_url("view", vid="rss", rql=rql)
-        w("<li>%s</li>\n" % tags.a(rss_label, href=rss_url, escapecontent=False))
+        w(f"<li>{tags.a(rss_label, href=rss_url, escapecontent=False)}</li>\n")
         w("</ul>\n")
 
 
 class LatestBlogsBlogBox(LatestBlogsBox):
     """display a box with latest blogs and rss, filtered for a particular blog"""
 
     __select__ = (
```

### Comparing `cubicweb-blog-2.2.0/cubicweb_blog/views/entry.py` & `cubicweb-blog-3.0.0/cubicweb_blog/views/entry.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 from six import PY2
 from six import text_type as unicode
 
 from logilab.mtconverter import xml_escape
 
 from cubicweb.schema import display_name
 from cubicweb_web.view import EntityView
-from cubicweb.predicates import paginated_rset, sorted_rset, is_instance
+from cubicweb.predicates import sorted_rset, is_instance
+from cubicweb_web.predicates import paginated_rset
 from cubicweb_web.views import uicfg
 from cubicweb_web.views import primary, baseviews, calendar, navigation, workflow
 from cubicweb_web.views.xmlrss import RSSItemView
 
 try:
     from cubicweb import _
 except ImportError:
@@ -36,16 +37,16 @@
 _afs = uicfg.autoform_section
 _afs.tag_subject_of(("BlogEntry", "entry_of", "Blog"), "main", "attributes")
 
 # blog entries ###########################################################
 
 
 def render_blogentry_title(req, w, entity):
-    w("<h1>%s</h1>" % entity.view("incontext"))
-    w('<div class="author_date"><div>%s' % req.format_date(entity.creation_date))
+    w(f"<h1>{entity.view('incontext')}</h1>")
+    w(f'<div class="author_date"><div>{req.format_date(entity.creation_date)}')
     rql = None
     if entity.has_creator:
         creator = entity.has_creator[0]
         name = creator.name
         rql = (
             "Any X ORDERBY D DESC WHERE X is BlogEntry, X has_creator Y, "
             "Y eid %s, X creation_date D" % creator.eid
@@ -148,20 +149,16 @@
             return
         rql = (
             "Any B, BD ORDERBY BD DESC "
             "WHERE B is BlogEntry, B creation_date BD, "
             'B creation_date >= "%s", B creation_date <= "%s"'
             % (firstday.strftime("%Y-%m-%d"), lastday.strftime("%Y-%m-%d"))
         )
-        label = "{} {} [{}]".format(
-            self._cw._(calendar.MONTHNAMES[month - 1]),
-            year,
-            nmb_entries,
-        )
-        vtitle = "{} {}".format(display_name(self._cw, "BlogEntry", "plural"), label)
+        label = f"{self._cw._(calendar.MONTHNAMES[month - 1])} {year} [{nmb_entries}]"
+        vtitle = f"{display_name(self._cw, 'BlogEntry', 'plural')} {label}"
         url = self._cw.build_url("view", rql=rql, vtitle=vtitle, month=month, year=year)
         return f'<a href="{xml_escape(url)}">{atitle}</a>'
 
 
 class BlogEntryBlogView(EntityView):
     __regid__ = "blog"
     __select__ = is_instance("BlogEntry")
@@ -179,15 +176,15 @@
         self.toolbar_components("ctxtoolbar")
         render_blogentry_title(self._cw, w, entity)
         w('<div class="entry">')
         body = entity.printable_value("content")
         w(body)
         w("</div>")
         w('<br class="clear"/>')
-        w('<div class="postmetadata">%s</div>' % entity.view("post-reldata"))
+        w(f"<div class=\"postmetadata\">{entity.view('post-reldata')}</div>")
         w("</div>")
 
 
 class BlogEntryPostMetaData(EntityView):
     __regid__ = "post-reldata"
     __select__ = is_instance("BlogEntry")
 
@@ -205,26 +202,22 @@
                 url = xml_escape(entity.absolute_url())
                 if count > 1:
                     label = _("Comment", "plural")
                 else:
                     label = _("Comment")
                 w(f'<a href="{url}">{count} {label}</a>')
             else:
-                w("{} {}".format(count, _("Comment")))
+                w(f"{count} {_('Comment')}")
         if "tags" in schema and "BlogEntry" in schema.rschema("tags").objects():
             tag_rset = entity.related("tags", "object")
             if tag_rset:
-                w("{} {}".format(_("tags", "object"), self._cw.view("csv", tag_rset)))
+                w(f"{_('tags', 'object')} {self._cw.view('csv', tag_rset)}")
         rset = entity.related("entry_of", "subject")
         if rset:
-            w(
-                "{} {}".format(
-                    self._cw._("blogged in "), self._cw.view("csv", rset, "null")
-                )
-            )
+            w(f"{self._cw._('blogged in ')} {self._cw.view('csv', rset, 'null')}")
         self.w(" | ".join(reldata))
 
 
 class BlogNavigation(navigation.PageNavigation):
     __select__ = paginated_rset() & sorted_rset() & is_instance("BlogEntry")
 
     def index_display(self, start, stop):
```

### Comparing `cubicweb-blog-2.2.0/cubicweb_blog/views/urlpublishing.py` & `cubicweb-blog-3.0.0/cubicweb_blog/views/urlpublishing.py`

 * *Files identical despite different names*

### Comparing `cubicweb-blog-2.2.0/cubicweb_blog.egg-info/PKG-INFO` & `cubicweb-blog-3.0.0/cubicweb_blog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubicweb-blog
-Version: 2.2.0
+Version: 3.0.0
 Summary: blogging component for the CubicWeb framework
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-blog
 Author: Logilab
 Author-email: contact@logilab.fr
 License: LGPL
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
```

### Comparing `cubicweb-blog-2.2.0/cubicweb_blog.egg-info/SOURCES.txt` & `cubicweb-blog-3.0.0/cubicweb_blog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-blog-2.2.0/setup.py` & `cubicweb-blog-3.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,17 +52,15 @@
 data_files = __pkginfo__.get("data_files", None)
 dependency_links = __pkginfo__.get("dependency_links", ())
 
 requires = {}
 for entry in ("__depends__",):  # "__recommends__"):
     requires.update(__pkginfo__.get(entry, {}))
 
-install_requires = [
-    "{} {}".format(d, v and v or "").strip() for d, v in requires.items()
-]
+install_requires = [f"{d} {v and v or ''}".strip() for d, v in requires.items()]
 
 
 setup(
     name=distname,
     version=version,
     license=license,
     description=description,
```

### Comparing `cubicweb-blog-2.2.0/test/unittest_blog.py` & `cubicweb-blog-3.0.0/test/unittest_blog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Blog unit tests"""
 
 import unittest
-from cubicweb.devtools.testlib import CubicWebTC, MAILBOX
+from cubicweb.devtools.testlib import MAILBOX
+from cubicweb_web.devtools.testlib import WebCWTC
 
 
-class BlogTestsCubicWebTC(CubicWebTC):
+class BlogTestsCubicWebTC(WebCWTC):
     """test blog specific behaviours"""
 
     def test_notifications(self):
         with self.admin_access.client_cnx() as cnx:
             cubicweb_blog = cnx.create_entity(
                 "Blog", title="cubicweb", description="cubicweb c'est beau"
             )
```

### Comparing `cubicweb-blog-2.2.0/tox.ini` & `cubicweb-blog-3.0.0/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tox]
 envlist = py3, flake8, check-manifest, yamllint, black
 
 [testenv]
 deps =
   pytest
+  webtest
   -rdev-requirements.txt
 commands =
   {envpython} -m pytest {posargs:-vvx}
 
 [pytest]
 python_files = *test_*.py
 testpaths = test
```

