# Comparing `tmp/tendril-structures-media-0.1.8.tar.gz` & `tmp/tendril-structures-media-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-structures-media-0.1.8.tar", last modified: Sun Jul 23 04:25:48 2023, max compression
+gzip compressed data, was "tendril-structures-media-0.1.9.tar", last modified: Tue Jul 25 12:00:40 2023, max compression
```

## Comparing `tendril-structures-media-0.1.8.tar` & `tendril-structures-media-0.1.9.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-23 04:25:48.635852 tendril-structures-media-0.1.8/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2136 2023-04-26 18:35:29.000000 tendril-structures-media-0.1.8/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.8/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.8/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.8/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.8/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.8/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3675 2023-07-23 04:25:48.635852 tendril-structures-media-0.1.8/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2336 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.8/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-23 04:25:48.627852 tendril-structures-media-0.1.8/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.8/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-23 04:25:48.631852 tendril-structures-media-0.1.8/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.8/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.8/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.8/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.8/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-23 04:25:48.631852 tendril-structures-media-0.1.8/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-structures-media-0.1.8/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-23 04:25:48.631852 tendril-structures-media-0.1.8/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.8/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13478 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.8/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      913 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.8/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1590 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.8/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-23 04:25:48.631852 tendril-structures-media-0.1.8/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.8/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.8/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-07-23 04:25:48.635852 tendril-structures-media-0.1.8/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3358 2023-07-03 21:49:49.000000 tendril-structures-media-0.1.8/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-23 04:25:48.627852 tendril-structures-media-0.1.8/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-23 04:25:48.631852 tendril-structures-media-0.1.8/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-media-0.1.8/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-23 04:25:48.631852 tendril-structures-media-0.1.8/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-23 13:08:58.000000 tendril-structures-media-0.1.8/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-23 04:25:48.631852 tendril-structures-media-0.1.8/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 10:22:45.000000 tendril-structures-media-0.1.8/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       15 2023-04-28 05:00:39.000000 tendril-structures-media-0.1.8/src/tendril/apiserver/routers/content.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-23 04:25:48.631852 tendril-structures-media-0.1.8/src/tendril/apiserver/templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-28 04:06:37.000000 tendril-structures-media-0.1.8/src/tendril/apiserver/templates/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    11648 2023-07-06 20:23:55.000000 tendril-structures-media-0.1.8/src/tendril/apiserver/templates/content.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-23 04:25:48.631852 tendril-structures-media-0.1.8/src/tendril/common/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 20:38:48.000000 tendril-structures-media-0.1.8/src/tendril/common/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-23 04:25:48.631852 tendril-structures-media-0.1.8/src/tendril/common/content/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-06-26 20:32:36.000000 tendril-structures-media-0.1.8/src/tendril/common/content/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1685 2023-06-27 07:55:43.000000 tendril-structures-media-0.1.8/src/tendril/common/content/exceptions.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-23 04:25:48.631852 tendril-structures-media-0.1.8/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-04-25 04:58:23.000000 tendril-structures-media-0.1.8/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3996 2023-06-25 07:33:44.000000 tendril-structures-media-0.1.8/src/tendril/config/media.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-23 04:25:48.631852 tendril-structures-media-0.1.8/src/tendril/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-media-0.1.8/src/tendril/db/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-23 04:25:48.631852 tendril-structures-media-0.1.8/src/tendril/db/controllers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 19:20:28.000000 tendril-structures-media-0.1.8/src/tendril/db/controllers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5991 2023-07-22 21:26:24.000000 tendril-structures-media-0.1.8/src/tendril/db/controllers/content.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-23 04:25:48.631852 tendril-structures-media-0.1.8/src/tendril/db/models/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-media-0.1.8/src/tendril/db/models/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     6967 2023-07-22 16:29:15.000000 tendril-structures-media-0.1.8/src/tendril/db/models/content.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4118 2023-07-23 04:19:22.000000 tendril-structures-media-0.1.8/src/tendril/db/models/content_formats.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1226 2023-06-30 07:27:36.000000 tendril-structures-media-0.1.8/src/tendril/db/models/content_thumbnails.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-23 04:25:48.631852 tendril-structures-media-0.1.8/src/tendril/interests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      233 2023-06-25 07:24:32.000000 tendril-structures-media-0.1.8/src/tendril/interests/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-23 04:25:48.635852 tendril-structures-media-0.1.8/src/tendril/interests/mixins/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 12:41:01.000000 tendril-structures-media-0.1.8/src/tendril/interests/mixins/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    17389 2023-07-23 04:09:36.000000 tendril-structures-media-0.1.8/src/tendril/interests/mixins/content.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-23 04:25:48.635852 tendril-structures-media-0.1.8/src/tendril/libraries/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-23 19:42:43.000000 tendril-structures-media-0.1.8/src/tendril/libraries/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-23 04:25:48.635852 tendril-structures-media-0.1.8/src/tendril/libraries/mixins/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 12:41:01.000000 tendril-structures-media-0.1.8/src/tendril/libraries/mixins/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1015 2023-07-14 16:11:05.000000 tendril-structures-media-0.1.8/src/tendril/libraries/mixins/content.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-23 04:25:48.635852 tendril-structures-media-0.1.8/src/tendril/structures/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-14 04:22:57.000000 tendril-structures-media-0.1.8/src/tendril/structures/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-23 04:25:48.635852 tendril-structures-media-0.1.8/src/tendril/structures/content/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      378 2023-07-02 08:01:43.000000 tendril-structures-media-0.1.8/src/tendril/structures/content/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-23 04:25:48.635852 tendril-structures-media-0.1.8/src/tendril/structures/content/providers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      266 2023-07-03 15:26:07.000000 tendril-structures-media-0.1.8/src/tendril/structures/content/providers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1641 2023-07-03 21:00:40.000000 tendril-structures-media-0.1.8/src/tendril/structures/content/providers/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1229 2023-07-03 18:30:23.000000 tendril-structures-media-0.1.8/src/tendril/structures/content/providers/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-23 04:25:48.635852 tendril-structures-media-0.1.8/src/tendril_structures_media.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3675 2023-07-23 04:25:48.000000 tendril-structures-media-0.1.8/src/tendril_structures_media.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1782 2023-07-23 04:25:48.000000 tendril-structures-media-0.1.8/src/tendril_structures_media.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-07-23 04:25:48.000000 tendril-structures-media-0.1.8/src/tendril_structures_media.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      614 2023-07-23 04:25:48.000000 tendril-structures-media-0.1.8/src/tendril_structures_media.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-07-23 04:25:48.000000 tendril-structures-media-0.1.8/src/tendril_structures_media.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-23 04:25:48.635852 tendril-structures-media-0.1.8/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.8/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.8/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.8/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.890595 tendril-structures-media-0.1.9/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2136 2023-04-26 18:35:29.000000 tendril-structures-media-0.1.9/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3675 2023-07-25 12:00:40.890595 tendril-structures-media-0.1.9/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2336 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.874595 tendril-structures-media-0.1.9/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.874595 tendril-structures-media-0.1.9/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.878595 tendril-structures-media-0.1.9/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-structures-media-0.1.9/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.878595 tendril-structures-media-0.1.9/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13478 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      913 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1590 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.878595 tendril-structures-media-0.1.9/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-07-25 12:00:40.890595 tendril-structures-media-0.1.9/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3358 2023-07-03 21:49:49.000000 tendril-structures-media-0.1.9/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.870595 tendril-structures-media-0.1.9/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.878595 tendril-structures-media-0.1.9/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-media-0.1.9/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.878595 tendril-structures-media-0.1.9/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-23 13:08:58.000000 tendril-structures-media-0.1.9/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.878595 tendril-structures-media-0.1.9/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 10:22:45.000000 tendril-structures-media-0.1.9/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       15 2023-04-28 05:00:39.000000 tendril-structures-media-0.1.9/src/tendril/apiserver/routers/content.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.878595 tendril-structures-media-0.1.9/src/tendril/apiserver/templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-28 04:06:37.000000 tendril-structures-media-0.1.9/src/tendril/apiserver/templates/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    11648 2023-07-06 20:23:55.000000 tendril-structures-media-0.1.9/src/tendril/apiserver/templates/content.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.878595 tendril-structures-media-0.1.9/src/tendril/common/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 20:38:48.000000 tendril-structures-media-0.1.9/src/tendril/common/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.878595 tendril-structures-media-0.1.9/src/tendril/common/content/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-06-26 20:32:36.000000 tendril-structures-media-0.1.9/src/tendril/common/content/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1685 2023-06-27 07:55:43.000000 tendril-structures-media-0.1.9/src/tendril/common/content/exceptions.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.878595 tendril-structures-media-0.1.9/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-04-25 04:58:23.000000 tendril-structures-media-0.1.9/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3996 2023-06-25 07:33:44.000000 tendril-structures-media-0.1.9/src/tendril/config/media.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.882595 tendril-structures-media-0.1.9/src/tendril/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-media-0.1.9/src/tendril/db/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.882595 tendril-structures-media-0.1.9/src/tendril/db/controllers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-26 19:20:28.000000 tendril-structures-media-0.1.9/src/tendril/db/controllers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5991 2023-07-22 21:26:24.000000 tendril-structures-media-0.1.9/src/tendril/db/controllers/content.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.882595 tendril-structures-media-0.1.9/src/tendril/db/models/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-13 04:49:54.000000 tendril-structures-media-0.1.9/src/tendril/db/models/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7326 2023-07-25 11:56:15.000000 tendril-structures-media-0.1.9/src/tendril/db/models/content.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4118 2023-07-23 04:19:22.000000 tendril-structures-media-0.1.9/src/tendril/db/models/content_formats.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1226 2023-06-30 07:27:36.000000 tendril-structures-media-0.1.9/src/tendril/db/models/content_thumbnails.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.882595 tendril-structures-media-0.1.9/src/tendril/interests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      233 2023-06-25 07:24:32.000000 tendril-structures-media-0.1.9/src/tendril/interests/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.882595 tendril-structures-media-0.1.9/src/tendril/interests/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 12:41:01.000000 tendril-structures-media-0.1.9/src/tendril/interests/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    17585 2023-07-25 12:00:04.000000 tendril-structures-media-0.1.9/src/tendril/interests/mixins/content.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.882595 tendril-structures-media-0.1.9/src/tendril/libraries/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-23 19:42:43.000000 tendril-structures-media-0.1.9/src/tendril/libraries/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.886595 tendril-structures-media-0.1.9/src/tendril/libraries/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 12:41:01.000000 tendril-structures-media-0.1.9/src/tendril/libraries/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1015 2023-07-14 16:11:05.000000 tendril-structures-media-0.1.9/src/tendril/libraries/mixins/content.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.886595 tendril-structures-media-0.1.9/src/tendril/structures/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-14 04:22:57.000000 tendril-structures-media-0.1.9/src/tendril/structures/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.886595 tendril-structures-media-0.1.9/src/tendril/structures/content/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      378 2023-07-02 08:01:43.000000 tendril-structures-media-0.1.9/src/tendril/structures/content/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.886595 tendril-structures-media-0.1.9/src/tendril/structures/content/providers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      266 2023-07-03 15:26:07.000000 tendril-structures-media-0.1.9/src/tendril/structures/content/providers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1641 2023-07-03 21:00:40.000000 tendril-structures-media-0.1.9/src/tendril/structures/content/providers/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1229 2023-07-03 18:30:23.000000 tendril-structures-media-0.1.9/src/tendril/structures/content/providers/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.886595 tendril-structures-media-0.1.9/src/tendril_structures_media.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3675 2023-07-25 12:00:40.000000 tendril-structures-media-0.1.9/src/tendril_structures_media.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1782 2023-07-25 12:00:40.000000 tendril-structures-media-0.1.9/src/tendril_structures_media.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-07-25 12:00:40.000000 tendril-structures-media-0.1.9/src/tendril_structures_media.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      614 2023-07-25 12:00:40.000000 tendril-structures-media-0.1.9/src/tendril_structures_media.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-07-25 12:00:40.000000 tendril-structures-media-0.1.9/src/tendril_structures_media.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-25 12:00:40.886595 tendril-structures-media-0.1.9/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2023-04-13 04:41:11.000000 tendril-structures-media-0.1.9/tox.ini
```

### Comparing `tendril-structures-media-0.1.8/.gitignore` & `tendril-structures-media-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.8/.readthedocs.yml` & `tendril-structures-media-0.1.9/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.8/.travis.yml` & `tendril-structures-media-0.1.9/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.8/LICENSE` & `tendril-structures-media-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.8/PKG-INFO` & `tendril-structures-media-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-structures-media
-Version: 0.1.8
+Version: 0.1.9
 Summary: Media management structures for Tendril
 Home-page: https://github.com/tendril-framework/tendril-structures-media
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-structures-media.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-structures-media/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-structures-media
```

### Comparing `tendril-structures-media-0.1.8/README.rst` & `tendril-structures-media-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.8/docs/Makefile` & `tendril-structures-media-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.8/docs/_static/custom.css` & `tendril-structures-media-0.1.9/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.8/docs/_static/favicon.ico` & `tendril-structures-media-0.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.8/docs/_static/logo.png` & `tendril-structures-media-0.1.9/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.8/docs/_static/logo_packed.png` & `tendril-structures-media-0.1.9/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.8/docs/_templates/about.html` & `tendril-structures-media-0.1.9/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.8/docs/conf.py` & `tendril-structures-media-0.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.8/docs/index.rst` & `tendril-structures-media-0.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.8/docs/installation.rst` & `tendril-structures-media-0.1.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.8/setup.py` & `tendril-structures-media-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.8/src/tendril/apiserver/templates/content.py` & `tendril-structures-media-0.1.9/src/tendril/apiserver/templates/content.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.8/src/tendril/common/content/exceptions.py` & `tendril-structures-media-0.1.9/src/tendril/common/content/exceptions.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.8/src/tendril/config/__init__.py` & `tendril-structures-media-0.1.9/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.8/src/tendril/config/media.py` & `tendril-structures-media-0.1.9/src/tendril/config/media.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.8/src/tendril/db/controllers/content.py` & `tendril-structures-media-0.1.9/src/tendril/db/controllers/content.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.8/src/tendril/db/models/content.py` & `tendril-structures-media-0.1.9/src/tendril/db/models/content.py`

 * *Files 8% similar despite different names*

```diff
@@ -85,14 +85,17 @@
     def export(self, full=False):
         rv = {'content_type': self.content_type,
               'estimated_duration': self.estimated_duration()}
         if self.bg_color:
             rv['bg_color'] = self.bg_color
         return rv
 
+    def is_usable(self):
+        return False
+
     def estimated_duration(self):
         return None
 
 
 class MediaContentModel(ContentModel):
     type_name = 'media'
     type_description = "Single Media File"
@@ -126,14 +129,17 @@
         if not len(step_durations):
             return max(simple_durations)
         if not len(simple_durations):
             return min(step_durations)
         step_durations = [x * -1 * 10000 for x in step_durations]
         return max(simple_durations + step_durations)
 
+    def is_usable(self):
+        return len(self.formats) > 0
+
 
 class StructuredContentModel(ContentModel):
     type_name = 'structured'
     type_description = "Device Assembled Structured Content"
 
     id = Column(Integer, ForeignKey("Content.id"), primary_key=True)
     path = Column(String(64))
@@ -149,14 +155,18 @@
         if self.args:
             rv['args'] = self.args
         return rv
 
     def estimated_duration(self):
         return None
 
+    def is_usable(self):
+        # TODO Check if the path corresponds to a valid provider as well?
+        return self.path is not None
+
 
 class SequenceContentModel(ContentModel):
     type_name = 'sequence'
     type_description = "Sequence of other content types"
 
     id = Column(Integer, ForeignKey("Content.id"), primary_key=True)
     default_duration = Column(Integer, nullable=False, default=10000)
@@ -183,14 +193,17 @@
                 if duration != -1:
                     padding = (-1 - duration) * 1000
                 duration = self.default_duration * -1 * duration + padding
 
             actual_durations.append(duration)
         return sum(actual_durations) + 1000 * len(durations)
 
+    def is_usable(self):
+        return len(self.contents) > 0 and all([x.is_usable() for x in self.contents])
+
 
 class SequenceContentAssociationModel(DeclBase):
     __tablename__ = "SequenceContentAssociation"
     sequence_id: Mapped[int] = mapped_column(ForeignKey("SequenceContent.id"), primary_key=True)
     content_id: Mapped[int] = mapped_column(ForeignKey("Content.id"))
     position: Mapped[int] = mapped_column(primary_key=True)
     duration: Mapped[Optional[int]]
```

### Comparing `tendril-structures-media-0.1.8/src/tendril/db/models/content_formats.py` & `tendril-structures-media-0.1.9/src/tendril/db/models/content_formats.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.8/src/tendril/db/models/content_thumbnails.py` & `tendril-structures-media-0.1.9/src/tendril/db/models/content_thumbnails.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.8/src/tendril/interests/mixins/content.py` & `tendril-structures-media-0.1.9/src/tendril/interests/mixins/content.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     # interest class as well.
 
     token_namespace = 'mfu'
     upload_bucket_name = MEDIA_UPLOAD_FILESTORE_BUCKET
     publish_bucket_name = MEDIA_PUBLISHING_FILESTORE_BUCKET
     additional_creation_fields = ['content_type']
     additional_export_fields = ['content_type']
+    additional_activation_checks = ['check_content_usable']
 
     def __init__(self, *args, content_type=None, **kwargs):
         self._content_type = content_type
         super(MediaContentInterest, self).__init__(*args, **kwargs)
         self._upload_bucket = None
         self._publish_bucket = None
 
@@ -86,14 +87,18 @@
         self._commit_to_db(session=session)
 
     @property
     def content(self):
         return self.model_instance.content
 
     @with_db
+    def check_content_usable(self, auth_user=None, session=None):
+        return self.content.is_usable()
+
+    @with_db
     def activate(self, background_tasks=None, auth_user=None, session=None):
         result, msg = super().activate(background_tasks=background_tasks,
                                        auth_user=auth_user, session=session)
 
         if not self.model_instance.status == LifecycleStatus.ACTIVE:
             return result, msg
 
@@ -140,15 +145,15 @@
                 if hasattr(fmt, 'stored_file'):
                     if fmt.stored_file.bucket.name != self.publish_bucket_name:
                         return False
         return True
 
     @with_db
     @require_state((LifecycleStatus.ACTIVE, LifecycleStatus.APPROVAL, LifecycleStatus.NEW))
-    @require_permission('read_artefacts', strip_auth=False)
+    @require_permission('read_artefacts', strip_auth=False, required=False)
     def content_information(self, full=False, auth_user=None, session=None):
         if not self._model_instance.content:
             raise ContentNotReady('read_content_info', self.id, self.name)
         else:
             content: ContentModel = self._model_instance.content
             rv = content.export(full=full)
             if full:
```

### Comparing `tendril-structures-media-0.1.8/src/tendril/libraries/mixins/content.py` & `tendril-structures-media-0.1.9/src/tendril/libraries/mixins/content.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.8/src/tendril/structures/content/providers/base.py` & `tendril-structures-media-0.1.9/src/tendril/structures/content/providers/base.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.8/src/tendril/structures/content/providers/manager.py` & `tendril-structures-media-0.1.9/src/tendril/structures/content/providers/manager.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.8/src/tendril_structures_media.egg-info/PKG-INFO` & `tendril-structures-media-0.1.9/src/tendril_structures_media.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-structures-media
-Version: 0.1.8
+Version: 0.1.9
 Summary: Media management structures for Tendril
 Home-page: https://github.com/tendril-framework/tendril-structures-media
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-structures-media.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-structures-media/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-structures-media
```

### Comparing `tendril-structures-media-0.1.8/src/tendril_structures_media.egg-info/SOURCES.txt` & `tendril-structures-media-0.1.9/src/tendril_structures_media.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.8/src/tendril_structures_media.egg-info/requires.txt` & `tendril-structures-media-0.1.9/src/tendril_structures_media.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.8/tests/coveralls.py` & `tendril-structures-media-0.1.9/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-structures-media-0.1.8/tox.ini` & `tendril-structures-media-0.1.9/tox.ini`

 * *Files identical despite different names*

