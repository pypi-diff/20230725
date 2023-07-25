# Comparing `tmp/xblock-utils-3.2.0.tar.gz` & `tmp/xblock-utils-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xblock-utils-3.2.0.tar", last modified: Thu Jun 15 19:15:33 2023, max compression
+gzip compressed data, was "xblock-utils-3.3.0.tar", last modified: Tue Jul 25 07:29:06 2023, max compression
```

## Comparing `xblock-utils-3.2.0.tar` & `xblock-utils-3.3.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 19:15:33.032771 xblock-utils-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)    34500 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    15928 2023-06-15 19:15:33.032771 xblock-utils-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    12387 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 19:15:33.028771 xblock-utils-3.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      164 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      225 2023-06-15 19:15:33.032771 xblock-utils-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3703 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 19:15:33.028771 xblock-utils-3.2.0/xblock_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    15928 2023-06-15 19:15:32.000000 xblock-utils-3.2.0/xblock_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-06-15 19:15:33.000000 xblock-utils-3.2.0/xblock_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-15 19:15:32.000000 xblock-utils-3.2.0/xblock_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-06-15 19:15:32.000000 xblock-utils-3.2.0/xblock_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-15 19:15:32.000000 xblock-utils-3.2.0/xblock_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 19:15:33.028771 xblock-utils-3.2.0/xblockutils/
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/xblockutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7680 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/xblockutils/base_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/xblockutils/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 19:15:33.032771 xblock-utils-3.2.0/xblockutils/public/
--rw-r--r--   0 runner    (1001) docker     (122)     2357 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/xblockutils/public/studio_container.js
--rw-r--r--   0 runner    (1001) docker     (122)     7647 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/xblockutils/public/studio_edit.js
--rw-r--r--   0 runner    (1001) docker     (122)     2062 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/xblockutils/publish_event.py
--rw-r--r--   0 runner    (1001) docker     (122)     4875 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/xblockutils/resources.py
--rw-r--r--   0 runner    (1001) docker     (122)     3526 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/xblockutils/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)    22344 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/xblockutils/studio_editable.py
--rw-r--r--   0 runner    (1001) docker     (122)     3327 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/xblockutils/studio_editable_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 19:15:33.032771 xblock-utils-3.2.0/xblockutils/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/xblockutils/templates/add_buttons.html
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/xblockutils/templates/default_preview_view.html
--rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/xblockutils/templates/studio_edit.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 19:15:33.032771 xblock-utils-3.2.0/xblockutils/templatetags/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/xblockutils/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-06-15 19:15:28.000000 xblock-utils-3.2.0/xblockutils/templatetags/i18n.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 07:29:06.160783 xblock-utils-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    34500 2023-07-25 07:29:01.000000 xblock-utils-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-07-25 07:29:01.000000 xblock-utils-3.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    15928 2023-07-25 07:29:06.160783 xblock-utils-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    12387 2023-07-25 07:29:01.000000 xblock-utils-3.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 07:29:06.152783 xblock-utils-3.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      164 2023-07-25 07:29:01.000000 xblock-utils-3.3.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      749 2023-07-25 07:29:01.000000 xblock-utils-3.3.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      225 2023-07-25 07:29:06.160783 xblock-utils-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     6111 2023-07-25 07:29:01.000000 xblock-utils-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 07:29:06.152783 xblock-utils-3.3.0/xblock_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    15928 2023-07-25 07:29:05.000000 xblock-utils-3.3.0/xblock_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      764 2023-07-25 07:29:06.000000 xblock-utils-3.3.0/xblock_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-25 07:29:05.000000 xblock-utils-3.3.0/xblock_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-07-25 07:29:05.000000 xblock-utils-3.3.0/xblock_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-25 07:29:05.000000 xblock-utils-3.3.0/xblock_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 07:29:06.156783 xblock-utils-3.3.0/xblockutils/
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-07-25 07:29:01.000000 xblock-utils-3.3.0/xblockutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7680 2023-07-25 07:29:01.000000 xblock-utils-3.3.0/xblockutils/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-07-25 07:29:01.000000 xblock-utils-3.3.0/xblockutils/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 07:29:06.160783 xblock-utils-3.3.0/xblockutils/public/
+-rw-r--r--   0 runner    (1001) docker     (122)     2357 2023-07-25 07:29:01.000000 xblock-utils-3.3.0/xblockutils/public/studio_container.js
+-rw-r--r--   0 runner    (1001) docker     (122)     7647 2023-07-25 07:29:01.000000 xblock-utils-3.3.0/xblockutils/public/studio_edit.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2062 2023-07-25 07:29:01.000000 xblock-utils-3.3.0/xblockutils/publish_event.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4875 2023-07-25 07:29:01.000000 xblock-utils-3.3.0/xblockutils/resources.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3526 2023-07-25 07:29:01.000000 xblock-utils-3.3.0/xblockutils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22344 2023-07-25 07:29:01.000000 xblock-utils-3.3.0/xblockutils/studio_editable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3327 2023-07-25 07:29:01.000000 xblock-utils-3.3.0/xblockutils/studio_editable_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 07:29:06.160783 xblock-utils-3.3.0/xblockutils/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-07-25 07:29:01.000000 xblock-utils-3.3.0/xblockutils/templates/add_buttons.html
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-07-25 07:29:01.000000 xblock-utils-3.3.0/xblockutils/templates/default_preview_view.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-07-25 07:29:01.000000 xblock-utils-3.3.0/xblockutils/templates/studio_edit.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 07:29:06.160783 xblock-utils-3.3.0/xblockutils/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-25 07:29:01.000000 xblock-utils-3.3.0/xblockutils/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-07-25 07:29:01.000000 xblock-utils-3.3.0/xblockutils/templatetags/i18n.py
```

### Comparing `xblock-utils-3.2.0/LICENSE` & `xblock-utils-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.2.0/PKG-INFO` & `xblock-utils-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: xblock-utils
-Version: 3.2.0
+Version: 3.3.0
 Summary: Various utilities for XBlocks
 Home-page: https://github.com/openedx/xblock-utils
 Author: edX
 Author-email: oscm@edx.org
 License: UNKNOWN
 Description: xblock-utils: Various utilities for XBlocks
         ###########################################
@@ -382,12 +382,12 @@
         ===================
         
         This mixin provides XBlock theming capabilities built on top of XBlock-specific settings.
         See [wiki page](https://github.com/openedx/xblock-utils/wiki/Settings-and-theme-support#theming-support) for details
         
 Platform: UNKNOWN
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `xblock-utils-3.2.0/README.rst` & `xblock-utils-3.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.2.0/xblock_utils.egg-info/PKG-INFO` & `xblock-utils-3.3.0/xblock_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: xblock-utils
-Version: 3.2.0
+Version: 3.3.0
 Summary: Various utilities for XBlocks
 Home-page: https://github.com/openedx/xblock-utils
 Author: edX
 Author-email: oscm@edx.org
 License: UNKNOWN
 Description: xblock-utils: Various utilities for XBlocks
         ###########################################
@@ -382,12 +382,12 @@
         ===================
         
         This mixin provides XBlock theming capabilities built on top of XBlock-specific settings.
         See [wiki page](https://github.com/openedx/xblock-utils/wiki/Settings-and-theme-support#theming-support) for details
         
 Platform: UNKNOWN
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `xblock-utils-3.2.0/xblock_utils.egg-info/SOURCES.txt` & `xblock-utils-3.3.0/xblock_utils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 requirements/base.in
+requirements/constraints.txt
 xblock_utils.egg-info/PKG-INFO
 xblock_utils.egg-info/SOURCES.txt
 xblock_utils.egg-info/dependency_links.txt
 xblock_utils.egg-info/requires.txt
 xblock_utils.egg-info/top_level.txt
 xblockutils/__init__.py
 xblockutils/base_test.py
```

### Comparing `xblock-utils-3.2.0/xblockutils/base_test.py` & `xblock-utils-3.3.0/xblockutils/base_test.py`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.2.0/xblockutils/helpers.py` & `xblock-utils-3.3.0/xblockutils/helpers.py`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.2.0/xblockutils/public/studio_container.js` & `xblock-utils-3.3.0/xblockutils/public/studio_container.js`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.2.0/xblockutils/public/studio_edit.js` & `xblock-utils-3.3.0/xblockutils/public/studio_edit.js`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.2.0/xblockutils/publish_event.py` & `xblock-utils-3.3.0/xblockutils/publish_event.py`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.2.0/xblockutils/resources.py` & `xblock-utils-3.3.0/xblockutils/resources.py`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.2.0/xblockutils/settings.py` & `xblock-utils-3.3.0/xblockutils/settings.py`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.2.0/xblockutils/studio_editable.py` & `xblock-utils-3.3.0/xblockutils/studio_editable.py`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.2.0/xblockutils/studio_editable_test.py` & `xblock-utils-3.3.0/xblockutils/studio_editable_test.py`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.2.0/xblockutils/templates/add_buttons.html` & `xblock-utils-3.3.0/xblockutils/templates/add_buttons.html`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.2.0/xblockutils/templates/studio_edit.html` & `xblock-utils-3.3.0/xblockutils/templates/studio_edit.html`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.2.0/xblockutils/templatetags/i18n.py` & `xblock-utils-3.3.0/xblockutils/templatetags/i18n.py`

 * *Files identical despite different names*

