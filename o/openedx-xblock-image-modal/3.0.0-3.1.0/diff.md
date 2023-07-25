# Comparing `tmp/openedx-xblock-image-modal-3.0.0.tar.gz` & `tmp/openedx-xblock-image-modal-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx-xblock-image-modal-3.0.0.tar", last modified: Thu Nov 24 12:01:44 2022, max compression
+gzip compressed data, was "openedx-xblock-image-modal-3.1.0.tar", last modified: Tue Jul 25 09:50:24 2023, max compression
```

## Comparing `openedx-xblock-image-modal-3.0.0.tar` & `openedx-xblock-image-modal-3.1.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 12:01:44.504011 openedx-xblock-image-modal-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)    34520 2022-11-24 12:01:36.000000 openedx-xblock-image-modal-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       85 2022-11-24 12:01:36.000000 openedx-xblock-image-modal-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4865 2022-11-24 12:01:44.504011 openedx-xblock-image-modal-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3968 2022-11-24 12:01:36.000000 openedx-xblock-image-modal-3.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 12:01:44.500010 openedx-xblock-image-modal-3.0.0/imagemodal/
--rw-r--r--   0 runner    (1001) docker     (122)       81 2022-11-24 12:01:36.000000 openedx-xblock-image-modal-3.0.0/imagemodal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 12:01:44.500010 openedx-xblock-image-modal-3.0.0/imagemodal/mixins/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2022-11-24 12:01:36.000000 openedx-xblock-image-modal-3.0.0/imagemodal/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2593 2022-11-24 12:01:36.000000 openedx-xblock-image-modal-3.0.0/imagemodal/mixins/fragment.py
--rw-r--r--   0 runner    (1001) docker     (122)     1570 2022-11-24 12:01:36.000000 openedx-xblock-image-modal-3.0.0/imagemodal/mixins/scenario.py
--rw-r--r--   0 runner    (1001) docker     (122)     1846 2022-11-24 12:01:36.000000 openedx-xblock-image-modal-3.0.0/imagemodal/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 12:01:44.500010 openedx-xblock-image-modal-3.0.0/imagemodal/public/
--rw-r--r--   0 runner    (1001) docker     (122)    20691 2022-11-24 12:01:36.000000 openedx-xblock-image-modal-3.0.0/imagemodal/public/draggabilly.pkgd.min.js
--rw-r--r--   0 runner    (1001) docker     (122)     1637 2022-11-24 12:01:36.000000 openedx-xblock-image-modal-3.0.0/imagemodal/public/view.css
--rw-r--r--   0 runner    (1001) docker     (122)     4842 2022-11-24 12:01:36.000000 openedx-xblock-image-modal-3.0.0/imagemodal/public/view.js
--rw-r--r--   0 runner    (1001) docker     (122)     2100 2022-11-24 12:01:36.000000 openedx-xblock-image-modal-3.0.0/imagemodal/public/view.less
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 12:01:44.500010 openedx-xblock-image-modal-3.0.0/imagemodal/scenarios/
--rw-r--r--   0 runner    (1001) docker     (122)      687 2022-11-24 12:01:36.000000 openedx-xblock-image-modal-3.0.0/imagemodal/scenarios/image-modal-many.xml
--rw-r--r--   0 runner    (1001) docker     (122)      424 2022-11-24 12:01:36.000000 openedx-xblock-image-modal-3.0.0/imagemodal/scenarios/image-modal-single.xml
--rw-r--r--   0 runner    (1001) docker     (122)      330 2022-11-24 12:01:36.000000 openedx-xblock-image-modal-3.0.0/imagemodal/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 12:01:44.500010 openedx-xblock-image-modal-3.0.0/imagemodal/templates/
--rw-r--r--   0 runner    (1001) docker     (122)     1064 2022-11-24 12:01:36.000000 openedx-xblock-image-modal-3.0.0/imagemodal/templates/view.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 12:01:44.500010 openedx-xblock-image-modal-3.0.0/imagemodal/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 12:01:44.500010 openedx-xblock-image-modal-3.0.0/imagemodal/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 12:01:44.500010 openedx-xblock-image-modal-3.0.0/imagemodal/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1467 2022-11-24 12:01:36.000000 openedx-xblock-image-modal-3.0.0/imagemodal/translations/en/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     1290 2022-11-24 12:01:36.000000 openedx-xblock-image-modal-3.0.0/imagemodal/views.py
--rw-r--r--   0 runner    (1001) docker     (122)      411 2022-11-24 12:01:36.000000 openedx-xblock-image-modal-3.0.0/imagemodal/xblocks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 12:01:44.500010 openedx-xblock-image-modal-3.0.0/openedx_xblock_image_modal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4865 2022-11-24 12:01:44.000000 openedx-xblock-image-modal-3.0.0/openedx_xblock_image_modal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      879 2022-11-24 12:01:44.000000 openedx-xblock-image-modal-3.0.0/openedx_xblock_image_modal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-24 12:01:44.000000 openedx-xblock-image-modal-3.0.0/openedx_xblock_image_modal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       56 2022-11-24 12:01:44.000000 openedx-xblock-image-modal-3.0.0/openedx_xblock_image_modal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       31 2022-11-24 12:01:44.000000 openedx-xblock-image-modal-3.0.0/openedx_xblock_image_modal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2022-11-24 12:01:44.000000 openedx-xblock-image-modal-3.0.0/openedx_xblock_image_modal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 12:01:44.500010 openedx-xblock-image-modal-3.0.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       94 2022-11-24 12:01:36.000000 openedx-xblock-image-modal-3.0.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      515 2022-11-24 12:01:36.000000 openedx-xblock-image-modal-3.0.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-24 12:01:44.504011 openedx-xblock-image-modal-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5045 2022-11-24 12:01:36.000000 openedx-xblock-image-modal-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 09:50:24.924793 openedx-xblock-image-modal-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-07-25 09:50:20.000000 openedx-xblock-image-modal-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-07-25 09:50:20.000000 openedx-xblock-image-modal-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4547 2023-07-25 09:50:24.924793 openedx-xblock-image-modal-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3748 2023-07-25 09:50:20.000000 openedx-xblock-image-modal-3.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 09:50:24.920793 openedx-xblock-image-modal-3.1.0/imagemodal/
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-07-25 09:50:20.000000 openedx-xblock-image-modal-3.1.0/imagemodal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 09:50:24.924793 openedx-xblock-image-modal-3.1.0/imagemodal/mixins/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-07-25 09:50:20.000000 openedx-xblock-image-modal-3.1.0/imagemodal/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2593 2023-07-25 09:50:20.000000 openedx-xblock-image-modal-3.1.0/imagemodal/mixins/fragment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1570 2023-07-25 09:50:20.000000 openedx-xblock-image-modal-3.1.0/imagemodal/mixins/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-07-25 09:50:20.000000 openedx-xblock-image-modal-3.1.0/imagemodal/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 09:50:24.924793 openedx-xblock-image-modal-3.1.0/imagemodal/public/
+-rw-r--r--   0 runner    (1001) docker     (122)    20691 2023-07-25 09:50:20.000000 openedx-xblock-image-modal-3.1.0/imagemodal/public/draggabilly.pkgd.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1637 2023-07-25 09:50:20.000000 openedx-xblock-image-modal-3.1.0/imagemodal/public/view.css
+-rw-r--r--   0 runner    (1001) docker     (122)     4842 2023-07-25 09:50:20.000000 openedx-xblock-image-modal-3.1.0/imagemodal/public/view.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2100 2023-07-25 09:50:20.000000 openedx-xblock-image-modal-3.1.0/imagemodal/public/view.less
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 09:50:24.924793 openedx-xblock-image-modal-3.1.0/imagemodal/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (122)      687 2023-07-25 09:50:20.000000 openedx-xblock-image-modal-3.1.0/imagemodal/scenarios/image-modal-many.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-07-25 09:50:20.000000 openedx-xblock-image-modal-3.1.0/imagemodal/scenarios/image-modal-single.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      330 2023-07-25 09:50:20.000000 openedx-xblock-image-modal-3.1.0/imagemodal/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 09:50:24.924793 openedx-xblock-image-modal-3.1.0/imagemodal/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)     1123 2023-07-25 09:50:20.000000 openedx-xblock-image-modal-3.1.0/imagemodal/templates/view.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 09:50:24.920793 openedx-xblock-image-modal-3.1.0/imagemodal/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 09:50:24.920793 openedx-xblock-image-modal-3.1.0/imagemodal/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 09:50:24.924793 openedx-xblock-image-modal-3.1.0/imagemodal/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1468 2023-07-25 09:50:20.000000 openedx-xblock-image-modal-3.1.0/imagemodal/translations/en/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1468 2023-07-25 09:50:20.000000 openedx-xblock-image-modal-3.1.0/imagemodal/translations/en/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-07-25 09:50:20.000000 openedx-xblock-image-modal-3.1.0/imagemodal/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)      411 2023-07-25 09:50:20.000000 openedx-xblock-image-modal-3.1.0/imagemodal/xblocks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 09:50:24.924793 openedx-xblock-image-modal-3.1.0/openedx_xblock_image_modal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4547 2023-07-25 09:50:24.000000 openedx-xblock-image-modal-3.1.0/openedx_xblock_image_modal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      926 2023-07-25 09:50:24.000000 openedx-xblock-image-modal-3.1.0/openedx_xblock_image_modal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-25 09:50:24.000000 openedx-xblock-image-modal-3.1.0/openedx_xblock_image_modal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-07-25 09:50:24.000000 openedx-xblock-image-modal-3.1.0/openedx_xblock_image_modal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-07-25 09:50:24.000000 openedx-xblock-image-modal-3.1.0/openedx_xblock_image_modal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-25 09:50:24.000000 openedx-xblock-image-modal-3.1.0/openedx_xblock_image_modal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 09:50:24.924793 openedx-xblock-image-modal-3.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2023-07-25 09:50:20.000000 openedx-xblock-image-modal-3.1.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-07-25 09:50:20.000000 openedx-xblock-image-modal-3.1.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-25 09:50:24.924793 openedx-xblock-image-modal-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4989 2023-07-25 09:50:20.000000 openedx-xblock-image-modal-3.1.0/setup.py
```

### Comparing `openedx-xblock-image-modal-3.0.0/LICENSE` & `openedx-xblock-image-modal-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openedx-xblock-image-modal-3.0.0/PKG-INFO` & `openedx-xblock-image-modal-3.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 Metadata-Version: 2.1
 Name: openedx-xblock-image-modal
-Version: 3.0.0
+Version: 3.1.0
 Summary: A full-screen image modal XBlock
 Home-page: https://github.com/Stanford-Online/xblock-image-modal
 Author: stv
 Author-email: stv@stanford.edu
 License: AGPL-3.0
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Education
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 License-File: LICENSE
 
 Image Modal XBlock
 ==================
 
 A full-screen image modal XBlock,
-for use within the OpenEdX platform.
+for use within the Open edX platform.
 
 |badge-ci|
-|badge-coveralls|
 
 The full-screen image tool is another way of enabling participants to
 see more detail in your provided images. This tool is useful for large
 images with lots of details. A re-sized version of the image displays in
 the page, but clicking on the image pops open a full-screen modal with
 the full-size version of the image.
 
@@ -125,18 +121,16 @@
 Click and drag to pan around.
 
 `View a demo of the CMS`_
 
 `View a demo of the LMS`_
 
 
-.. |badge-coveralls| image:: https://coveralls.io/repos/github/Stanford-Online/xblock-image-modal/badge.svg?branch=master
-   :target: https://coveralls.io/github/Stanford-Online/xblock-image-modal?branch=master
-.. |badge-ci| image:: https://github.com/edx/xblock-image-modal/workflows/Python%20CI/badge.svg?branch=master
-   :target: https://github.com/edx/xblock-image-modal/actions?query=workflow%3A%22Python+CI%22
+.. |badge-ci| image:: https://github.com/openedx/xblock-image-modal/workflows/Python%20CI/badge.svg?branch=master
+   :target: https://github.com/openedx/xblock-image-modal/actions?query=workflow%3A%22Python+CI%22
 .. |image-cms-add| image:: https://s3-us-west-1.amazonaws.com/stanford-openedx-docs/xblocks/image-modal/static/images/cms-add.jpg
    :width: 100%
 .. |image-cms-advanced-module-list| image:: https://s3-us-west-1.amazonaws.com/stanford-openedx-docs/xblocks/image-modal/static/images/advanced-module-list.png
    :width: 100%
 .. |image-cms-editor-1| image:: https://s3-us-west-1.amazonaws.com/stanford-openedx-docs/xblocks/image-modal/static/images/studio-editor-1.png
    :width: 100%
 .. |image-cms-editor-2| image:: https://s3-us-west-1.amazonaws.com/stanford-openedx-docs/xblocks/image-modal/static/images/studio-editor-2.png
@@ -148,9 +142,7 @@
 .. |image-lms-view-normal| image:: https://s3-us-west-1.amazonaws.com/stanford-openedx-docs/xblocks/image-modal/static/images/lms-view-normal.png
    :width: 100%
 .. |image-lms-view-zoom| image:: https://s3-us-west-1.amazonaws.com/stanford-openedx-docs/xblocks/image-modal/static/images/lms-view-zoom.png
    :width: 100%
 .. _View a demo of the CMS: https://youtu.be/IcbGYfbav2w
 .. _View a demo of the LMS: https://youtu.be/0mpjuThDoyE
 .. https://s3-us-west-1.amazonaws.com/stanford-openedx-docs/xblocks/image-modal/static/images/xblock-image-modal-demo-lms.mov
-
-
```

### Comparing `openedx-xblock-image-modal-3.0.0/README.rst` & `openedx-xblock-image-modal-3.1.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Image Modal XBlock
 ==================
 
 A full-screen image modal XBlock,
-for use within the OpenEdX platform.
+for use within the Open edX platform.
 
 |badge-ci|
-|badge-coveralls|
 
 The full-screen image tool is another way of enabling participants to
 see more detail in your provided images. This tool is useful for large
 images with lots of details. A re-sized version of the image displays in
 the page, but clicking on the image pops open a full-screen modal with
 the full-size version of the image.
 
@@ -100,18 +99,16 @@
 Click and drag to pan around.
 
 `View a demo of the CMS`_
 
 `View a demo of the LMS`_
 
 
-.. |badge-coveralls| image:: https://coveralls.io/repos/github/Stanford-Online/xblock-image-modal/badge.svg?branch=master
-   :target: https://coveralls.io/github/Stanford-Online/xblock-image-modal?branch=master
-.. |badge-ci| image:: https://github.com/edx/xblock-image-modal/workflows/Python%20CI/badge.svg?branch=master
-   :target: https://github.com/edx/xblock-image-modal/actions?query=workflow%3A%22Python+CI%22
+.. |badge-ci| image:: https://github.com/openedx/xblock-image-modal/workflows/Python%20CI/badge.svg?branch=master
+   :target: https://github.com/openedx/xblock-image-modal/actions?query=workflow%3A%22Python+CI%22
 .. |image-cms-add| image:: https://s3-us-west-1.amazonaws.com/stanford-openedx-docs/xblocks/image-modal/static/images/cms-add.jpg
    :width: 100%
 .. |image-cms-advanced-module-list| image:: https://s3-us-west-1.amazonaws.com/stanford-openedx-docs/xblocks/image-modal/static/images/advanced-module-list.png
    :width: 100%
 .. |image-cms-editor-1| image:: https://s3-us-west-1.amazonaws.com/stanford-openedx-docs/xblocks/image-modal/static/images/studio-editor-1.png
    :width: 100%
 .. |image-cms-editor-2| image:: https://s3-us-west-1.amazonaws.com/stanford-openedx-docs/xblocks/image-modal/static/images/studio-editor-2.png
```

### Comparing `openedx-xblock-image-modal-3.0.0/imagemodal/mixins/fragment.py` & `openedx-xblock-image-modal-3.1.0/imagemodal/mixins/fragment.py`

 * *Files identical despite different names*

### Comparing `openedx-xblock-image-modal-3.0.0/imagemodal/mixins/scenario.py` & `openedx-xblock-image-modal-3.1.0/imagemodal/mixins/scenario.py`

 * *Files identical despite different names*

### Comparing `openedx-xblock-image-modal-3.0.0/imagemodal/models.py` & `openedx-xblock-image-modal-3.1.0/imagemodal/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Handle data access logic for the XBlock
 """
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from xblock.fields import Scope
 from xblock.fields import String
 
 
 class ImageModalModelMixin:
     """
     Handle data access for Image Modal XBlock instances
@@ -61,11 +61,10 @@
     )
 
     alt_text = String(
         display_name=_('Alt Text'),
         default='',
         scope=Scope.settings,
         help=_(
-            'This field allows you to add alternate or descriptive text'
-            'that pertains to your image.'
+            'This field allows you to add alternate or descriptive text that pertains to your image.'
         ),
     )
```

### Comparing `openedx-xblock-image-modal-3.0.0/imagemodal/public/draggabilly.pkgd.min.js` & `openedx-xblock-image-modal-3.1.0/imagemodal/public/draggabilly.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `openedx-xblock-image-modal-3.0.0/imagemodal/public/view.css` & `openedx-xblock-image-modal-3.1.0/imagemodal/public/view.css`

 * *Files identical despite different names*

### Comparing `openedx-xblock-image-modal-3.0.0/imagemodal/public/view.js` & `openedx-xblock-image-modal-3.1.0/imagemodal/public/view.js`

 * *Files identical despite different names*

### Comparing `openedx-xblock-image-modal-3.0.0/imagemodal/public/view.less` & `openedx-xblock-image-modal-3.1.0/imagemodal/public/view.less`

 * *Files identical despite different names*

### Comparing `openedx-xblock-image-modal-3.0.0/imagemodal/scenarios/image-modal-many.xml` & `openedx-xblock-image-modal-3.1.0/imagemodal/scenarios/image-modal-many.xml`

 * *Files identical despite different names*

### Comparing `openedx-xblock-image-modal-3.0.0/imagemodal/templates/view.html` & `openedx-xblock-image-modal-3.1.0/imagemodal/templates/view.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,34 @@
+{% load i18n %}
+
 <div class="imagemodal_block">
     <h2>{{display_name}}</h2>
     <div class="wrapper">
         <a href="{{image_url}}">
             <img
                 alt="{{alt_text}}"
                 src="{{thumbnail_url}}"
                 aria-describedby="xblock_imagemodal__description__{{xblock_id}}"
             />
         </a>
         <button class="fullscreen">
             <i class="icon-fullscreen icon-large"></i>
-            <span>Fullscreen</span>
+            <span>{% trans "Fullscreen" %}</span>
         </button>
     </div>
     <div class="curtain">
         <div class="mask">
             <div class="wrapper">
                 <img alt="{{alt_text}}" src="{{image_url}}" />
             </div>
             <button class="zoom">
                 <i class="icon-zoom-in icon-large"></i>
-                <span>Zoom In</span>
+                <span>{% trans "Zoom In" %}</span>
             </button>
             <button class="close">
                 <i class="icon-remove icon-large"></i>
-                <span>Close</span>
+                <span>{% trans "Close" %}</span>
             </button>
         </div>
     </div>
     <p id="xblock_imagemodal__description__{{xblock_id}}" class="sr">{{description}}</p>
 </div>
```

#### html2text {}

```diff
@@ -1,5 +1,6 @@
+{% load i18n %}
 ***** {{display_name}} *****
-[{{alt_text}}]   Fullscreen
+[{{alt_text}}]   {% trans "Fullscreen" %}
 [{{alt_text}}]
-  Zoom In    Close
+  {% trans "Zoom In" %}    {% trans "Close" %}
 {{description}}
```

### Comparing `openedx-xblock-image-modal-3.0.0/imagemodal/translations/en/LC_MESSAGES/django.po` & `openedx-xblock-image-modal-3.1.0/imagemodal/translations/en/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -53,10 +53,10 @@
 
 #: imagemodal/imagemodal.py:74
 msgid "Alt Text"
 msgstr ""
 
 #: imagemodal/imagemodal.py:78
 msgid ""
-"This field allows you to add alternate or descriptive textthat pertains to "
+"This field allows you to add alternate or descriptive text that pertains to "
 "your image."
 msgstr ""
```

### Comparing `openedx-xblock-image-modal-3.0.0/imagemodal/views.py` & `openedx-xblock-image-modal-3.1.0/imagemodal/views.py`

 * *Files identical despite different names*

### Comparing `openedx-xblock-image-modal-3.0.0/openedx_xblock_image_modal.egg-info/PKG-INFO` & `openedx-xblock-image-modal-3.1.0/openedx_xblock_image_modal.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 Metadata-Version: 2.1
 Name: openedx-xblock-image-modal
-Version: 3.0.0
+Version: 3.1.0
 Summary: A full-screen image modal XBlock
 Home-page: https://github.com/Stanford-Online/xblock-image-modal
 Author: stv
 Author-email: stv@stanford.edu
 License: AGPL-3.0
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Education
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 License-File: LICENSE
 
 Image Modal XBlock
 ==================
 
 A full-screen image modal XBlock,
-for use within the OpenEdX platform.
+for use within the Open edX platform.
 
 |badge-ci|
-|badge-coveralls|
 
 The full-screen image tool is another way of enabling participants to
 see more detail in your provided images. This tool is useful for large
 images with lots of details. A re-sized version of the image displays in
 the page, but clicking on the image pops open a full-screen modal with
 the full-size version of the image.
 
@@ -125,18 +121,16 @@
 Click and drag to pan around.
 
 `View a demo of the CMS`_
 
 `View a demo of the LMS`_
 
 
-.. |badge-coveralls| image:: https://coveralls.io/repos/github/Stanford-Online/xblock-image-modal/badge.svg?branch=master
-   :target: https://coveralls.io/github/Stanford-Online/xblock-image-modal?branch=master
-.. |badge-ci| image:: https://github.com/edx/xblock-image-modal/workflows/Python%20CI/badge.svg?branch=master
-   :target: https://github.com/edx/xblock-image-modal/actions?query=workflow%3A%22Python+CI%22
+.. |badge-ci| image:: https://github.com/openedx/xblock-image-modal/workflows/Python%20CI/badge.svg?branch=master
+   :target: https://github.com/openedx/xblock-image-modal/actions?query=workflow%3A%22Python+CI%22
 .. |image-cms-add| image:: https://s3-us-west-1.amazonaws.com/stanford-openedx-docs/xblocks/image-modal/static/images/cms-add.jpg
    :width: 100%
 .. |image-cms-advanced-module-list| image:: https://s3-us-west-1.amazonaws.com/stanford-openedx-docs/xblocks/image-modal/static/images/advanced-module-list.png
    :width: 100%
 .. |image-cms-editor-1| image:: https://s3-us-west-1.amazonaws.com/stanford-openedx-docs/xblocks/image-modal/static/images/studio-editor-1.png
    :width: 100%
 .. |image-cms-editor-2| image:: https://s3-us-west-1.amazonaws.com/stanford-openedx-docs/xblocks/image-modal/static/images/studio-editor-2.png
@@ -148,9 +142,7 @@
 .. |image-lms-view-normal| image:: https://s3-us-west-1.amazonaws.com/stanford-openedx-docs/xblocks/image-modal/static/images/lms-view-normal.png
    :width: 100%
 .. |image-lms-view-zoom| image:: https://s3-us-west-1.amazonaws.com/stanford-openedx-docs/xblocks/image-modal/static/images/lms-view-zoom.png
    :width: 100%
 .. _View a demo of the CMS: https://youtu.be/IcbGYfbav2w
 .. _View a demo of the LMS: https://youtu.be/0mpjuThDoyE
 .. https://s3-us-west-1.amazonaws.com/stanford-openedx-docs/xblocks/image-modal/static/images/xblock-image-modal-demo-lms.mov
-
-
```

### Comparing `openedx-xblock-image-modal-3.0.0/openedx_xblock_image_modal.egg-info/SOURCES.txt` & `openedx-xblock-image-modal-3.1.0/openedx_xblock_image_modal.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 imagemodal/public/view.css
 imagemodal/public/view.js
 imagemodal/public/view.less
 imagemodal/scenarios/image-modal-many.xml
 imagemodal/scenarios/image-modal-single.xml
 imagemodal/templates/view.html
 imagemodal/translations/en/LC_MESSAGES/django.po
+imagemodal/translations/en/LC_MESSAGES/text.po
 openedx_xblock_image_modal.egg-info/PKG-INFO
 openedx_xblock_image_modal.egg-info/SOURCES.txt
 openedx_xblock_image_modal.egg-info/dependency_links.txt
 openedx_xblock_image_modal.egg-info/entry_points.txt
 openedx_xblock_image_modal.egg-info/requires.txt
 openedx_xblock_image_modal.egg-info/top_level.txt
 requirements/base.in
```

### Comparing `openedx-xblock-image-modal-3.0.0/requirements/constraints.txt` & `openedx-xblock-image-modal-3.1.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `openedx-xblock-image-modal-3.0.0/setup.py` & `openedx-xblock-image-modal-3.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 import os
 import re
 from os import path
 
 from setuptools import setup
 
-version = '3.0.0'
+version = '3.1.0'
 description = __doc__.strip().split('\n')[0]
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.rst')) as file_in:
     long_description = file_in.read()
 
 
 def load_requirements(*requirements_paths):
@@ -104,28 +104,27 @@
     package_data={
         "imagemodal": [
             'mixins/*.py',
             'public/*',
             'scenarios/*.xml',
             'templates/*',
             'translations/*/*/*',
+            'conf',
         ],
     },
     classifiers=[
         # https://pypi.python.org/pypi?%3Aaction=list_classifiers
         'Intended Audience :: Developers',
         'Intended Audience :: Education',
         'License :: OSI Approved :: GNU Affero General Public License v3',
         'Operating System :: OS Independent',
         'Programming Language :: JavaScript',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Topic :: Education',
         'Topic :: Internet :: WWW/HTTP',
         'Framework :: Django',
-        'Framework :: Django :: 2.2',
-        'Framework :: Django :: 3.0',
-        'Framework :: Django :: 3.1',
         'Framework :: Django :: 3.2',
+        'Framework :: Django :: 4.2',
     ],
     test_suite='imagemodal.tests',
 )
```

