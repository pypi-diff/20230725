# Comparing `tmp/cellmaps_coembedding-0.1.0a3.tar.gz` & `tmp/cellmaps_coembedding-0.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_coembedding-0.1.0a3.tar", last modified: Mon May 22 19:42:03 2023, max compression
+gzip compressed data, was "dist/cellmaps_coembedding-0.1.0a4.tar", last modified: Mon Jul 24 23:41:37 2023, max compression
```

## Comparing `cellmaps_coembedding-0.1.0a3.tar` & `cellmaps_coembedding-0.1.0a4.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:42:03.176320 cellmaps_coembedding-0.1.0a3/
--rw-r--r--   0 churas     (504) staff       (20)      165 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a3/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3679 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a3/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-19 18:46:09.000000 cellmaps_coembedding-0.1.0a3/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a3/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a3/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     6037 2023-05-22 19:42:03.176449 cellmaps_coembedding-0.1.0a3/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     3941 2023-05-19 18:48:13.000000 cellmaps_coembedding-0.1.0a3/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:42:03.166644 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/
--rw-r--r--   0 churas     (504) staff       (20)      339 2023-05-22 19:37:29.000000 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     7814 2023-05-19 20:52:55.000000 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/cellmaps_coembeddingcmd.py
--rw-r--r--   0 churas     (504) staff       (20)      138 2023-05-02 23:53:50.000000 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/exceptions.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:42:03.169330 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/muse_sc/
--rw-r--r--   0 churas     (504) staff       (20)    13872 2023-05-18 21:57:55.000000 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/muse_sc/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     3530 2023-05-03 00:16:38.000000 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/muse_sc/architecture.py
--rw-r--r--   0 churas     (504) staff       (20)     3697 2023-03-16 18:20:58.000000 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/muse_sc/df_utils.py
--rw-r--r--   0 churas     (504) staff       (20)     1186 2023-03-16 18:20:58.000000 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/muse_sc/file_utils.py
--rw-r--r--   0 churas     (504) staff       (20)    11301 2023-03-16 18:20:58.000000 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/muse_sc/triplet_loss.py
--rw-r--r--   0 churas     (504) staff       (20)    18991 2023-05-22 19:37:29.000000 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/runner.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:42:03.167964 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     6037 2023-05-22 19:42:03.000000 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     1372 2023-05-22 19:42:03.000000 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-22 19:42:03.000000 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-22 19:42:03.000000 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)       66 2023-05-22 19:42:03.000000 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       21 2023-05-22 19:42:03.000000 cellmaps_coembedding-0.1.0a3/cellmaps_coembedding.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:42:03.174151 cellmaps_coembedding-0.1.0a3/docs/
--rw-r--r--   0 churas     (504) staff       (20)      622 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a3/docs/Makefile
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:42:03.163529 cellmaps_coembedding-0.1.0a3/docs/_build/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:42:03.163597 cellmaps_coembedding-0.1.0a3/docs/_build/html/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:42:03.174965 cellmaps_coembedding-0.1.0a3/docs/_build/html/_static/
--rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_coembedding-0.1.0a3/docs/_build/html/_static/file.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_coembedding-0.1.0a3/docs/_build/html/_static/minus.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_coembedding-0.1.0a3/docs/_build/html/_static/plus.png
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a3/docs/authors.rst
--rw-r--r--   0 churas     (504) staff       (20)     1086 2023-05-19 18:14:05.000000 cellmaps_coembedding-0.1.0a3/docs/cellmaps_coembedding.muse_sc.rst
--rw-r--r--   0 churas     (504) staff       (20)      877 2023-05-19 18:14:05.000000 cellmaps_coembedding-0.1.0a3/docs/cellmaps_coembedding.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     6062 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a3/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a3/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a3/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      288 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a3/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a3/docs/history.rst
--rw-r--r--   0 churas     (504) staff       (20)      955 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a3/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1216 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a3/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      460 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a3/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      819 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a3/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       79 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a3/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4376 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a3/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      790 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a3/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)      709 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a3/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a3/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      403 2023-05-22 19:42:03.177497 cellmaps_coembedding-0.1.0a3/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     2370 2023-05-19 18:48:26.000000 cellmaps_coembedding-0.1.0a3/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:42:03.176138 cellmaps_coembedding-0.1.0a3/tests/
--rw-r--r--   0 churas     (504) staff       (20)       75 2023-05-02 23:53:50.000000 cellmaps_coembedding-0.1.0a3/tests/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     2551 2023-05-09 23:51:08.000000 cellmaps_coembedding-0.1.0a3/tests/test_cellmaps_coembeddingcmd.py
--rw-r--r--   0 churas     (504) staff       (20)      911 2023-05-09 21:38:49.000000 cellmaps_coembedding-0.1.0a3/tests/test_cellmapscoembedder.py
--rw-r--r--   0 churas     (504) staff       (20)     2441 2023-05-09 23:46:41.000000 cellmaps_coembedding-0.1.0a3/tests/test_imagembeddingfilterandnametranslator.py
--rw-r--r--   0 churas     (504) staff       (20)      794 2023-05-03 00:02:48.000000 cellmaps_coembedding-0.1.0a3/tests/test_integration_cellmaps_coembedding.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:41:37.893308 cellmaps_coembedding-0.1.0a4/
+-rw-r--r--   0 churas     (504) staff       (20)      266 2023-06-15 20:38:12.000000 cellmaps_coembedding-0.1.0a4/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3679 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a4/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-19 18:46:09.000000 cellmaps_coembedding-0.1.0a4/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a4/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a4/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     6208 2023-07-24 23:41:37.893469 cellmaps_coembedding-0.1.0a4/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     4115 2023-07-17 23:14:29.000000 cellmaps_coembedding-0.1.0a4/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:41:37.883761 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/
+-rw-r--r--   0 churas     (504) staff       (20)      336 2023-07-24 23:41:10.000000 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     6496 2023-06-15 20:38:12.000000 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/cellmaps_coembeddingcmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      138 2023-05-02 23:53:50.000000 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/exceptions.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:41:37.886547 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/muse_sc/
+-rw-r--r--   0 churas     (504) staff       (20)    12539 2023-06-15 20:38:12.000000 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/muse_sc/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     3639 2023-06-15 20:38:12.000000 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/muse_sc/architecture.py
+-rw-r--r--   0 churas     (504) staff       (20)     3697 2023-03-16 18:20:58.000000 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/muse_sc/df_utils.py
+-rw-r--r--   0 churas     (504) staff       (20)     1186 2023-03-16 18:20:58.000000 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/muse_sc/file_utils.py
+-rw-r--r--   0 churas     (504) staff       (20)     7854 2023-06-15 20:38:12.000000 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/muse_sc/triplet_loss.py
+-rw-r--r--   0 churas     (504) staff       (20)    16118 2023-06-15 20:38:12.000000 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/runner.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:41:37.885269 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     6208 2023-07-24 23:41:37.000000 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     1372 2023-07-24 23:41:37.000000 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-07-24 23:41:37.000000 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-07-24 23:41:37.000000 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)       66 2023-07-24 23:41:37.000000 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       21 2023-07-24 23:41:37.000000 cellmaps_coembedding-0.1.0a4/cellmaps_coembedding.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:41:37.891114 cellmaps_coembedding-0.1.0a4/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      622 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a4/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:41:37.880595 cellmaps_coembedding-0.1.0a4/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:41:37.880680 cellmaps_coembedding-0.1.0a4/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:41:37.891855 cellmaps_coembedding-0.1.0a4/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_coembedding-0.1.0a4/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_coembedding-0.1.0a4/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_coembedding-0.1.0a4/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a4/docs/authors.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1086 2023-05-19 18:14:05.000000 cellmaps_coembedding-0.1.0a4/docs/cellmaps_coembedding.muse_sc.rst
+-rw-r--r--   0 churas     (504) staff       (20)      877 2023-05-19 18:14:05.000000 cellmaps_coembedding-0.1.0a4/docs/cellmaps_coembedding.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     6062 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a4/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a4/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a4/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      288 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a4/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a4/docs/history.rst
+-rw-r--r--   0 churas     (504) staff       (20)      849 2023-07-17 23:14:29.000000 cellmaps_coembedding-0.1.0a4/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1216 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a4/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      460 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a4/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      819 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a4/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       79 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a4/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4376 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a4/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      790 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a4/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)      709 2023-05-03 00:00:52.000000 cellmaps_coembedding-0.1.0a4/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-05-02 23:52:25.000000 cellmaps_coembedding-0.1.0a4/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      403 2023-07-24 23:41:37.894007 cellmaps_coembedding-0.1.0a4/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     2370 2023-05-19 18:48:26.000000 cellmaps_coembedding-0.1.0a4/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:41:37.893088 cellmaps_coembedding-0.1.0a4/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       75 2023-05-02 23:53:50.000000 cellmaps_coembedding-0.1.0a4/tests/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     2551 2023-05-09 23:51:08.000000 cellmaps_coembedding-0.1.0a4/tests/test_cellmaps_coembeddingcmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      911 2023-05-09 21:38:49.000000 cellmaps_coembedding-0.1.0a4/tests/test_cellmapscoembedder.py
+-rw-r--r--   0 churas     (504) staff       (20)     2441 2023-05-09 23:46:41.000000 cellmaps_coembedding-0.1.0a4/tests/test_imagembeddingfilterandnametranslator.py
+-rw-r--r--   0 churas     (504) staff       (20)      794 2023-05-03 00:02:48.000000 cellmaps_coembedding-0.1.0a4/tests/test_integration_cellmaps_coembedding.py
```

### Comparing `cellmaps_coembedding-0.1.0a3/CONTRIBUTING.rst` & `cellmaps_coembedding-0.1.0a4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a3/LICENSE` & `cellmaps_coembedding-0.1.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a3/PKG-INFO` & `cellmaps_coembedding-0.1.0a4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: cellmaps_coembedding
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: A tool to generate coembeddings from IF image embeddings and PPI network embeddings
 Home-page: https://github.com/idekerlab/cellmaps_coembedding
-Author: Leah Schaffer
-Author-email: lvschaffer@health.ucsd.edu
+Author: Ideker Lab CM4AI team
+Author-email: tools@cm4ai.org
 License: MIT license
-Description: ==================
-        CM4AI CoEmbedding
-        ==================
+Description: =====================
+        Cell Maps CoEmbedder
+        =====================
         
         
         .. image:: https://img.shields.io/pypi/v/cellmaps_coembedding.svg
                 :target: https://pypi.python.org/pypi/cellmaps_coembedding
         
         .. image:: https://img.shields.io/travis/idekerlab/cellmaps_coembedding.svg
                 :target: https://travis-ci.com/idekerlab/cellmaps_coembedding
         
         .. image:: https://readthedocs.org/projects/cellmaps-generate-ppi/badge/?version=latest
                 :target: https://cellmaps-generate-ppi.readthedocs.io/en/latest/?badge=latest
                 :alt: Documentation Status
         
-        A tool to generate coembeddings from IF image embeddings and PPI network embeddings
-        
+        Creates Coembedding from `Cell Maps ImmunoFluorscent Image Embedder <https://cellmaps-image-embedding.readthedocs.io>`__
+        and `Cell Maps PPI Embedder <https://cellmaps-ppi-embedding.readthedocs.io>`__ for `Cell Maps for AI (CM4AI) <https://cm4ai.org>`__
         
         * Free software: MIT license
         * Documentation: https://cellmaps-coembedding.readthedocs.io.
         
         
         
         Dependencies
@@ -51,15 +51,15 @@
         ------------
         
         .. code-block::
         
            git clone https://github.com/idekerlab/cellmaps_coembedding
            cd cellmaps_coembedding
            make dist
-           pip install dist/cellmaps_coembeddingcmd*whl
+           pip install dist/cellmaps_coembedding*whl
         
         
         Run **make** command with no arguments to see other build/deploy options including creation of Docker image 
         
         .. code-block::
         
            make
```

### Comparing `cellmaps_coembedding-0.1.0a3/README.rst` & `cellmaps_coembedding-0.1.0a4/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-==================
-CM4AI CoEmbedding
-==================
+=====================
+Cell Maps CoEmbedder
+=====================
 
 
 .. image:: https://img.shields.io/pypi/v/cellmaps_coembedding.svg
         :target: https://pypi.python.org/pypi/cellmaps_coembedding
 
 .. image:: https://img.shields.io/travis/idekerlab/cellmaps_coembedding.svg
         :target: https://travis-ci.com/idekerlab/cellmaps_coembedding
 
 .. image:: https://readthedocs.org/projects/cellmaps-generate-ppi/badge/?version=latest
         :target: https://cellmaps-generate-ppi.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
-A tool to generate coembeddings from IF image embeddings and PPI network embeddings
-
+Creates Coembedding from `Cell Maps ImmunoFluorscent Image Embedder <https://cellmaps-image-embedding.readthedocs.io>`__
+and `Cell Maps PPI Embedder <https://cellmaps-ppi-embedding.readthedocs.io>`__ for `Cell Maps for AI (CM4AI) <https://cm4ai.org>`__
 
 * Free software: MIT license
 * Documentation: https://cellmaps-coembedding.readthedocs.io.
 
 
 
 Dependencies
@@ -43,15 +43,15 @@
 ------------
 
 .. code-block::
 
    git clone https://github.com/idekerlab/cellmaps_coembedding
    cd cellmaps_coembedding
    make dist
-   pip install dist/cellmaps_coembeddingcmd*whl
+   pip install dist/cellmaps_coembedding*whl
 
 
 Run **make** command with no arguments to see other build/deploy options including creation of Docker image 
 
 .. code-block::
 
    make
```

### Comparing `cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/cellmaps_coembeddingcmd.py` & `cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/cellmaps_coembeddingcmd.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 from cellmaps_coembedding.runner import CellmapsCoEmbedder
 
 logger = logging.getLogger(__name__)
 
 
 PPI_EMBEDDINGDIR='--ppi_embeddingdir'
 IMAGE_EMBEDDINGDIR='--image_embeddingdir'
-IMAGE_DOWNLOADDIR='--image_downloaddir'
-
 
 def _parse_arguments(desc, args):
     """
     Parses command line arguments
 
     :param desc: description to display on command line
     :type desc: str
@@ -37,18 +35,14 @@
     parser.add_argument('outdir', help='Output directory')
     parser.add_argument(PPI_EMBEDDINGDIR, required=True,
                         help='Directory aka rocrate where ppi '
                              'embedding file resides')
     parser.add_argument(IMAGE_EMBEDDINGDIR, required=True,
                         help='Directory aka rocrate image embedding '
                              'file resides')
-    parser.add_argument(IMAGE_DOWNLOADDIR, required=True,
-                        help='Directory containing image download data or'
-                             'more specifically rocrate where '
-                             'file resides')
     parser.add_argument('--latent_dimension', type=int, default=128,
                         help='Output dimension of embedding')
     parser.add_argument('--n_epochs_init', default=200, type=int,
                         help='# of init training epochs')
     parser.add_argument('--n_epochs', default=500, type=int,
                         help='# of training epochs')
 
@@ -105,56 +99,40 @@
                        
     {image_embeddingdir} should be set to a directory path created by
                        cellmaps_image_embedding which has a {image_embedding_file} file
                        containing the tab delimited embeddings of the IF images
                        For each row, first value is assumed to be sample ID followed
                        by the embeddings separated by tabs. The first row
                        is assumed to be a header.
-                       
-    {image_downloaddir} should be set to a directory path created by
-                       cellmaps_imagedownloader which has a {image_gene_node_attr_file}
-                       file containing tab delimited data with following header line:
-                       name    represents      ambiguous       antibody        filename
-                       
-                       name = Gene Symbol
-                       represents = Ensemble ID
-                       ambiguous = Gene Symbols that map to same antibody delimited by comma
-                       antibody = Antibody for Gene Symbol
-                       filename = sample IDs delimited by comma for given antibody & Gene
-                       
 
     """.format(version=cellmaps_coembedding.__version__,
                ppi_embeddingdir=PPI_EMBEDDINGDIR,
                image_embeddingdir=IMAGE_EMBEDDINGDIR,
-               image_downloaddir=IMAGE_DOWNLOADDIR,
                ppi_embedding_file=constants.PPI_EMBEDDING_FILE,
                image_embedding_file=constants.IMAGE_EMBEDDING_FILE,
                image_gene_node_attr_file=constants.IMAGE_GENE_NODE_ATTR_FILE)
     theargs = _parse_arguments(desc, args[1:])
     theargs.program = args[0]
     theargs.version = cellmaps_coembedding.__version__
 
     try:
         logutils.setup_cmd_logging(theargs)
         if theargs.fake_embedding:
             gen = FakeCoEmbeddingGenerator(dimensions=theargs.latent_dimension,
                                            ppi_embeddingdir=theargs.ppi_embeddingdir,
-                                           image_embeddingdir=theargs.image_embeddingdir,
-                                           image_downloaddir=theargs.image_downloaddir)
+                                           image_embeddingdir=theargs.image_embeddingdir)
         else:
             gen = MuseCoEmbeddingGenerator(dimensions=theargs.latent_dimension,
                                            n_epochs=theargs.n_epochs,
                                            n_epochs_init=theargs.n_epochs_init,
                                            outdir=os.path.abspath(theargs.outdir),
                                            ppi_embeddingdir=theargs.ppi_embeddingdir,
-                                           image_embeddingdir=theargs.image_embeddingdir,
-                                           image_downloaddir=theargs.image_downloaddir)
+                                           image_embeddingdir=theargs.image_embeddingdir)
         return CellmapsCoEmbedder(outdir=theargs.outdir,
-                                  inputdirs=[theargs.image_embeddingdir, theargs.ppi_embeddingdir,
-                                             theargs.image_downloaddir],
+                                  inputdirs=[theargs.image_embeddingdir, theargs.ppi_embeddingdir],
                                   embedding_generator=gen,
                                   input_data_dict=theargs.__dict__).run()
     except Exception as e:
         logger.exception('Caught exception: ' + str(e))
         return 2
     finally:
         logging.shutdown()
```

### Comparing `cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/muse_sc/__init__.py` & `cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/muse_sc/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,31 +10,29 @@
 from .df_utils import *
 from .architecture import *
 from .triplet_loss import *
 
 
 #globals
 sourceFile = ''
-lambda_regul = 0
-min_diff = 0.0
+lambda_regul = 5
 hard_loss = False
-squared = False
-triplet_margin = 0.2
+triplet_margin = 0.1
 device = torch.device('cpu')
 
 def make_matrix_from_labels(labels):
     M = np.zeros((len(labels), len(labels)))
     for cluster in np.unique(labels):
         genes_in_cluster = np.where(labels == cluster)[0]
         for geneA in genes_in_cluster:
             for geneB in genes_in_cluster:
                 M[geneA,geneB] = 1    
     return M
 
-def train_model(model, optimizer, loader, label_x, label_y, epoch, lambda_super, train_name, train, semi, device):
+def train_model(model, optimizer, loader, label_x, label_y, epoch, lambda_super, train_name, train, device):
     
     L_totals = []
     L_reconstruction_xs = []
     L_reconstruction_ys = []
     L_weights = []
     L_trip_batch_all_xs = []
     L_trip_batch_all_ys = []
@@ -64,28 +62,27 @@
 
         #sparse penalty
         sparse_x = torch.sqrt(torch.sum(torch.sum(torch.square(w_x), axis=1)))
         sparse_y = torch.sqrt(torch.sum(torch.sum(torch.square(w_y), axis=1)))
         L_weight = sparse_x + sparse_y
         
         # triplet errors
-        L_trip_batch_hard_x = batch_hard_triplet_loss(batch_label_x_input, latent, triplet_margin, semi, device, squared)
-        L_trip_batch_hard_y = batch_hard_triplet_loss(batch_label_y_input, latent, triplet_margin, semi, device, squared)
-        L_trip_batch_all_x, _ = batch_all_triplet_loss(batch_label_x_input, latent, triplet_margin, device, squared)
-        L_trip_batch_all_y, _ = batch_all_triplet_loss(batch_label_y_input, latent, triplet_margin, device, squared)
+        L_trip_batch_hard_x = batch_hard_triplet_loss(batch_label_x_input, latent, triplet_margin, device)
+        L_trip_batch_hard_y = batch_hard_triplet_loss(batch_label_y_input, latent, triplet_margin, device)
+        L_trip_batch_all_x, _ = batch_all_triplet_loss(batch_label_x_input, latent, triplet_margin, device)
+        L_trip_batch_all_y, _ = batch_all_triplet_loss(batch_label_y_input, latent, triplet_margin, device)
 
 
         fraction_easy_x, fraction_semi_x, fraction_hard_x = fraction_triplets(batch_label_x_input, latent, triplet_margin, device)
         fraction_easy_y, fraction_semi_y, fraction_hard_y = fraction_triplets(batch_label_y_input, latent, triplet_margin, device)
 
         #reconstruction error
         L_reconstruction_x = torch.mean(torch.norm(reconstruct_x - batch_x_input))
         L_reconstruction_y = torch.mean(torch.norm(reconstruct_y - batch_y_input))
         
-        L_weight = torch.mean(torch.square(latent))
         L_total = lambda_super*(L_trip_batch_all_x + L_trip_batch_all_y) +  lambda_regul*L_weight + L_reconstruction_x + L_reconstruction_y
         
         if hard_loss:
             L_total = lambda_super*(L_trip_batch_hard_x + L_trip_batch_hard_y) +  lambda_regul*L_weight + L_reconstruction_x + L_reconstruction_y
 
         if train == True:
             optimizer.zero_grad()
@@ -108,176 +105,159 @@
         fraction_easy_xs.append(fraction_easy_x.detach().cpu().numpy())
         fraction_easy_ys.append(fraction_easy_y.detach().cpu().numpy())
         
     print( train_name+"_epoch:%d\ttotal_loss:%03.5f\treconstruction_loss_x:%03.5f\treconstruction_loss_y:%03.5f\tsparse_penalty:%03.5f\tx_triplet_loss_batch_hard:%03.5f\ty_triplet_loss_batch_hard:%03.5f\tx_triplet_loss_batch_all:%03.5f\ty_triplet_loss_batch_all:%03.5f\tx_fraction_hard:%03.5f\ty_fraction_hard:%03.5f\tx_fraction_semi:%03.5f\ty_fraction_semi:%03.5f\tx_fraction_easy:%03.5f\ty_fraction_easy:%03.5f"
         % (epoch, np.mean(L_totals), np.mean(L_reconstruction_xs), np.mean(L_reconstruction_ys), np.mean(L_weights), np.mean(L_trip_batch_hard_xs), np.mean(L_trip_batch_hard_ys), np.mean(L_trip_batch_all_xs), np.mean(L_trip_batch_all_ys), np.mean(fraction_hard_xs), np.mean(fraction_hard_ys),  np.mean(fraction_semi_xs), np.mean(fraction_semi_ys), np.mean(fraction_easy_xs), np.mean(fraction_easy_ys)), file = sourceFile)    
     
 
-def muse_fit_predict(resultsdir, index, data_x,
+    
+    
+def muse_fit_predict(resultsdir, data_x,
                      data_y,
-                     label_x=[],
-                     label_y=[],
+                     name_index = [],
+                     label_x = [],
+                     label_y = [],
+                     test_subset = [], 
                      batch_size=64,
-                     latent_dim=100,
+                     latent_dim=128,
                      n_epochs=500,
+                     n_epochs_init=200,
                      lambda_regul=5,
-                     lambda_super=5,
-                     min_diff=0.2, hard_loss=False, squared=False,
-                     batch_norm=False, l2_norm = False, save_update_epochs=False,
-                     semi=False, k=30, dropout=0.25, euc=False,
-                     n_epochs_init=200):
-    """
-        MUSE model fitting and predicting:
-          This function is used to train the MUSE model on multi-modality data
-
-        Parameters:
-          resultsdir:   directory to save files
-          index:        index names to use when saving files
-          data_x:       input for transcript modality; matrix of  n * p, where n = number of cells, p = number of genes.
-          data_y:       input for morphological modality; matrix of n * q, where n = number of cells, q is the feature dimension.
-          label_x:      initial reference cluster label for transcriptional modality.
-          label_y:      inital reference cluster label for morphological modality.
-          latent_dim:   feature dimension of joint latent representation.
-          n_epochs:     maximal epoch used in training.
-          lambda_regul: weight for regularization term in the loss function.
-          lambda_super: weight for supervised learning loss in the loss function.
-          margin:       margin to use for triplet loss
-
-        Output:
-          latent:       joint latent representation learned by MUSE.
-          reconstruct_x:reconstructed feature matrix corresponding to input data_x.
-          reconstruct_y:reconstructed feature matrix corresponding to input data_y.
-          latent_x:     modality-specific latent representation corresponding to data_x.
-          latent_y:     modality-specific latent representation corresponding to data_y.
-
-        Feng Bao @ Altschuler & Wu Lab @ UCSF 2022.
-        Software provided as is under MIT License.
-    """
-    """ initial parameter setting """
+                     lambda_super=5, triplet_margin=0.1, hard_loss=False, l2_norm = True, k=10, dropout=0.25, save_update_epochs=False):
     
     
     # parameter setting for neural network
     n_hidden = 128  # number of hidden node in neural network
     learn_rate = 1e-4  # learning rate in the optimization
+    batch_size = 64  # number of cells in the training batch
     cluster_update_epoch = 50
     sourceFile = open('{}.txt'.format(resultsdir), 'w')
     
     # get device
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
     if device.type == "cuda":
         torch.cuda.get_device_name()
         
     # set globals  (same across all training)
     globals()['sourceFile'] = sourceFile
     globals()['lambda_regul'] = lambda_regul
-    globals()['min_diff'] = min_diff
+    globals()['triplet_margin'] = triplet_margin
     globals()['hard_loss'] = hard_loss
-    globals()['squared'] = squared
     globals()['device'] = device
 
     # read data-specific parameters from inputs
     feature_dim_x = data_x.shape[1]
     feature_dim_y = data_y.shape[1]
     n_sample = data_x.shape[0]
           
     # transform inputs to tensor
     transform=ToTensor()
     data_x = transform(data_x).to(device)
     data_y = transform(data_y).to(device)
     
-    #make labels 
-    
-    if euc:
-        primary_metric='euclidean'
-    else:
-        primary_metric = 'cosine'
-    
+        
+    #index names if none input
+    if len(name_index) == 0:
+        name_index = np.arange(n_sample)
+        
+    #remove test subset...
+    train_subset = np.arange(n_sample)
+    train_subset = list(set(train_subset) - set(test_subset))
+    train_data_x = data_x[train_subset]
+    train_data_y = data_y[train_subset]
+    if len(label_x) > 0 :
+        label_x = label_x[train_subset]
+    if len(label_y) > 0 : 
+        label_y = label_y[train_subset]
+
+
+    #create initial cluster labels if non input - only on training data
     create_label_x = False
     if len(label_x) == 0 :
-        label_x, _, _ = phenograph.cluster(data_x.detach().cpu().numpy(), k=k, primary_metric=primary_metric)
+        label_x, _, _ = phenograph.cluster(train_data_x.detach().cpu().numpy(), k=k, primary_metric='cosine')
         label_x = transform(make_matrix_from_labels(label_x)).to(device)
         create_label_x = True
     else:
         if (len(label_x.shape) == 1) or (label_x.shape[1] == 1) :
             label_x = transform(make_matrix_from_labels(label_x)).to(device)
         else:
             label_x = transform(label_x).to(device)
             
     create_label_y = False
     if len(label_y) == 0 :
-        label_y, _, _ = phenograph.cluster(data_y.detach().cpu().numpy(), k=k, primary_metric=primary_metric)
+        label_y, _, _ = phenograph.cluster(train_data_y.detach().cpu().numpy(), k=k, primary_metric='cosine')
         label_y = transform(make_matrix_from_labels(label_y)).to(device)
         create_label_y = True
     else:
         if (len(label_y.shape) == 1) or (label_y.shape[1] == 1) :
             label_y = transform(make_matrix_from_labels(label_y)).to(device)
         else:
             label_y = transform(label_y).to(device)
             
     # create model, optimizer, trainloader 
-        
-    model = structured_embedding(feature_dim_x, feature_dim_y, latent_dim, n_hidden, dropout, batch_norm, l2_norm).to(device)
+    model = structured_embedding(feature_dim_x, feature_dim_y, latent_dim, n_hidden, dropout, l2_norm).to(device)
     optimizer = optim.Adam(model.parameters(), lr=learn_rate)
-    train_loader = DataLoader(Protein_Dataset(data_x, data_y), batch_size=batch_size, shuffle=True)
+    train_loader = DataLoader(Protein_Dataset(train_data_x, train_data_y), batch_size=batch_size, shuffle=True)
 
      #INIT WITH JUST RECONSTRUCTION
-    for epoch in tqdm(range(n_epochs_init), desc='Init with just '
-                                                 'reconstruction'):
+    for epoch in range(n_epochs_init):
         model.train()
-        train_model(model, optimizer, train_loader, label_x, label_y, epoch, 0, 'init_recon', True, semi, device)
+        train_model(model, optimizer, train_loader, label_x, label_y, epoch, 0, 'init_recon', True, device)
         
   #  INIT WITH TRIPLET LOSS AND RECONSTRUCTION, ORIGINAL LABELS
-    for epoch in tqdm(range(n_epochs_init), desc='Init with triplet loss, recon & orig labels'):
+    for epoch in range(n_epochs_init):
         model.train()
-        train_model(model, optimizer, train_loader, label_x, label_y, epoch, lambda_super, 'init_both', True, semi, device)
+        train_model(model, optimizer, train_loader, label_x, label_y, epoch, lambda_super, 'init_both', True, device)
 
-    latent, reconstruct_x, reconstruct_y, latent_x, latent_y = model(data_x, data_y) 
+    latent, reconstruct_x, reconstruct_y, latent_x, latent_y = model(train_data_x, train_data_y) 
     
     update_label_x = label_x
     update_label_y = label_y
     if create_label_x:
-        update_label_x, _, _ = phenograph.cluster(latent_x.detach().cpu().numpy(), k=k , primary_metric=primary_metric)
+        update_label_x, _, _ = phenograph.cluster(latent_x.detach().cpu().numpy(), k=k , primary_metric='cosine')
         update_label_x = transform(make_matrix_from_labels(update_label_x)).to(device)
     if create_label_y:
-        update_label_y, _, _ = phenograph.cluster(latent_y.detach().cpu().numpy(), k=k , primary_metric=primary_metric)
+        update_label_y, _, _ = phenograph.cluster(latent_y.detach().cpu().numpy(), k=k , primary_metric='cosine')
         update_label_y = transform(make_matrix_from_labels(update_label_y)).to(device)
     
     # TRAIN WITH LABELS
-    for epoch in tqdm(range(n_epochs), desc='Train with labels'):
+    for epoch in range(n_epochs):
         model.train()
-        train_model(model, optimizer, train_loader, update_label_x, update_label_y, epoch, lambda_super, 'train', True, semi, device)
+        train_model(model, optimizer, train_loader, update_label_x, update_label_y, epoch, lambda_super, 'train', True, device)
         
         if epoch%cluster_update_epoch == 0:
             model.eval()
             with torch.no_grad():
                 latent, reconstruct_x, reconstruct_y, latent_x, latent_y = model(data_x, data_y)   
-            
 
             if save_update_epochs:
                 torch.save(model.state_dict(), '{}_{}.pth'.format(resultsdir, epoch))
-                pd.DataFrame(latent.detach().cpu().numpy(), index = index).to_csv('{}_latent_{}.txt'.format(resultsdir, epoch))
-                pd.DataFrame(reconstruct_x.detach().cpu().numpy(), index = index).to_csv('{}_reconstruct_x_{}.txt'.format(resultsdir, epoch))
-                pd.DataFrame(reconstruct_y.detach().cpu().numpy(), index = index).to_csv('{}_reconstruct_y_{}.txt'.format(resultsdir, epoch))
-                pd.DataFrame(latent_x.detach().cpu().numpy(), index = index).to_csv('{}_latent_x_{}.txt'.format(resultsdir, epoch))
-                pd.DataFrame(latent_y.detach().cpu().numpy(), index = index).to_csv('{}_latent_y_{}.txt'.format(resultsdir, epoch))
+                pd.DataFrame(latent.detach().cpu().numpy(), index = name_index).to_csv('{}_latent_{}.txt'.format(resultsdir, epoch))
+                pd.DataFrame(reconstruct_x.detach().cpu().numpy(), index = name_index).to_csv('{}_reconstruct_x_{}.txt'.format(resultsdir, epoch))
+                pd.DataFrame(reconstruct_y.detach().cpu().numpy(), index = name_index).to_csv('{}_reconstruct_y_{}.txt'.format(resultsdir, epoch))
+                pd.DataFrame(latent_x.detach().cpu().numpy(), index = name_index).to_csv('{}_latent_x_{}.txt'.format(resultsdir, epoch))
+                pd.DataFrame(latent_y.detach().cpu().numpy(), index = name_index).to_csv('{}_latent_y_{}.txt'.format(resultsdir, epoch))
             
+            # update clusters (only on training data)
             if create_label_x:
-                update_label_x, _, _ = phenograph.cluster(latent_x.detach().cpu().numpy(), k=k , primary_metric=primary_metric)
+                train_latent_x = latent_x[train_subset]
+                update_label_x, _, _ = phenograph.cluster(train_latent_x.detach().cpu().numpy(), k=k , primary_metric='cosine')
                 update_label_x = transform(make_matrix_from_labels(update_label_x)).to(device)
             if create_label_y:
-                update_label_y, _, _ = phenograph.cluster(latent_y.detach().cpu().numpy(), k=k , primary_metric=primary_metric)
+                train_latent_y = latent_y[train_subset]
+                update_label_y, _, _ = phenograph.cluster(train_latent_y.detach().cpu().numpy(), k=k , primary_metric='cosine')
                 update_label_y = transform(make_matrix_from_labels(update_label_y)).to(device)
-                           
+                        
     #SAVE FINAL RESULTS
     model.eval()
     with torch.no_grad():
         latent, reconstruct_x, reconstruct_y, latent_x, latent_y = model(data_x, data_y)
 
     detached_embeddings = latent.detach().cpu().numpy()
     torch.save(model.state_dict(), '{}.pth'.format(resultsdir))
-    pd.DataFrame(detached_embeddings, index = index).to_csv('{}_latent.txt'.format(resultsdir))
-    pd.DataFrame(reconstruct_x.detach().cpu().numpy(), index = index).to_csv('{}_reconstruct_x.txt'.format(resultsdir))
-    pd.DataFrame(reconstruct_y.detach().cpu().numpy(), index = index).to_csv('{}_reconstruct_y.txt'.format(resultsdir))
-    pd.DataFrame(latent_x.detach().cpu().numpy(), index = index).to_csv('{}_latent_x.txt'.format(resultsdir))
-    pd.DataFrame(latent_y.detach().cpu().numpy(), index = index).to_csv('{}_latent_y.txt'.format(resultsdir))
+    pd.DataFrame(detached_embeddings, index = name_index).to_csv('{}_latent.txt'.format(resultsdir))
+    pd.DataFrame(reconstruct_x.detach().cpu().numpy(), index = name_index).to_csv('{}_reconstruct_x.txt'.format(resultsdir))
+    pd.DataFrame(reconstruct_y.detach().cpu().numpy(), index = name_index).to_csv('{}_reconstruct_y.txt'.format(resultsdir))
+    pd.DataFrame(latent_x.detach().cpu().numpy(), index = name_index).to_csv('{}_latent_x.txt'.format(resultsdir))
+    pd.DataFrame(latent_y.detach().cpu().numpy(), index = name_index).to_csv('{}_latent_y.txt'.format(resultsdir))
     
-    return model, detached_embeddings
+    return model, detached_embeddings
```

### Comparing `cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/muse_sc/architecture.py` & `cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/muse_sc/architecture.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 ### Classes used for coembedding 
 import torch
 import numpy as np
 import torch.nn as nn
 from torch.utils.data import DataLoader, Dataset
 
-
 def cos_sim(A, B):
         cosine = np.dot(A,B)/(norm(A)*norm(B))
         return cosine
 
 class ToTensor:
     # Convert ndarrays to Tensors
     def __call__(self, sample):
@@ -33,39 +32,43 @@
         nn.init.constant_(m.bias.data, 0)
 
 def init_weights_d(m):
     if type(m) == nn.Linear:
         nn.init.normal_(m.weight.data)
             
 class structured_embedding(nn.Module):
-    def __init__(self, x_input_size, y_input_size, latent_dim, hidden_size, dropout, batch_norm, l2_norm):
+    def __init__(self, x_input_size, y_input_size, latent_dim, hidden_size, dropout, l2_norm):
         super().__init__()
                 
-        self.batch_norm = batch_norm 
         self.l2_norm = l2_norm
         
         self.encoder_x = nn.Sequential(
             nn.Dropout(dropout),
             nn.Linear(x_input_size, hidden_size),
+            nn.BatchNorm1d(hidden_size),
             nn.ELU(),
             nn.Dropout(dropout),
             nn.Linear(hidden_size, hidden_size),
+            nn.BatchNorm1d(hidden_size),
             nn.Tanh())
     
         self.encoder_y = nn.Sequential(
             nn.Dropout(dropout),
             nn.Linear(y_input_size, hidden_size),
+            nn.BatchNorm1d(hidden_size),
             nn.ELU(),
             nn.Dropout(dropout),
             nn.Linear(hidden_size, hidden_size),
+            nn.BatchNorm1d(hidden_size),
             nn.Tanh())
         
         self.encoder_z = nn.Sequential(
             nn.Dropout(dropout),
-            nn.Linear(hidden_size + hidden_size, latent_dim))
+            nn.Linear(hidden_size + hidden_size, latent_dim),
+            nn.BatchNorm1d(latent_dim))
         
         self.decoder_h_x = nn.Linear(latent_dim, latent_dim, bias=False)
         self.decoder_h_y = nn.Linear(latent_dim, latent_dim, bias=False)
         
         self.decoder_x = nn.Sequential(
             nn.Linear(latent_dim, hidden_size),
             nn.ELU(),
@@ -84,17 +87,15 @@
         self.encoder_x.apply(init_weights)
         self.encoder_y.apply(init_weights)
         self.encoder_z.apply(init_weights)
         self.decoder_h_x.apply(init_weights_d)
         self.decoder_h_y.apply(init_weights_d)
         self.decoder_x.apply(init_weights)
         self.decoder_y.apply(init_weights)
-        
-        self.batchnorm = nn.BatchNorm1d(latent_dim)
-       
+               
     
     def forward(self, x, y):
         
         h_x = self.encoder_x(x)
         h_y = self.encoder_y(y)
             
         h = torch.cat((h_x, h_y), 1)
@@ -113,7 +114,8 @@
 
         return z, x_hat, y_hat, h_x, h_y
         
         
         
 
 
+
```

### Comparing `cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/muse_sc/df_utils.py` & `cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/muse_sc/df_utils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/muse_sc/file_utils.py` & `cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/muse_sc/file_utils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/muse_sc/triplet_loss.py` & `cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/muse_sc/triplet_loss.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,85 +2,25 @@
 Triplet loss modified from https://github.com/omoindrot/tensorflow-triplet-loss/blob/master/model/triplet_loss.py
 Author: Olivier Moindrot from Stanford
 CONVERTED TO PYTORCH LVS
 '''
 import torch
 import torch.nn as nn
 
-
-# def _pairwise_distances(embeddings, device, squared=False):
-#     """Compute the 2D matrix of distances between all the embeddings.
-#     Args:
-#         embeddings: tensor of shape (batch_size, embed_dim)
-#         squared: Boolean. If true, output is the pairwise squared euclidean distance matrix.
-#                  If false, output is the pairwise euclidean distance matrix.
-#     Returns:
-#         pairwise_distances: tensor of shape (batch_size, batch_size)
-#     """
-#     # Get the dot product between all embeddings
-#     # shape (batch_size, batch_size)
-#     dot_product = torch.matmul(embeddings, torch.transpose(embeddings, 0, 1))
-
-#     # Get squared L2 norm for each embedding. We can just take the diagonal of `dot_product`.
-#     # This also provides more numerical stability (the diagonal of the result will be exactly 0).
-#     # shape (batch_size,)
-#     square_norm = torch.diagonal(dot_product)
-
-#     # Compute the pairwise distance matrix as we have:
-#     # ||a - b||^2 = ||a||^2  - 2 <a, b> + ||b||^2
-#     # shape (batch_size, batch_size)
-#     distances = torch.unsqueeze(square_norm, 1) - 2.0 * dot_product + torch.unsqueeze(square_norm, 0)
-
-#     # Because of computation errors, some distances might be negative so we put everything >= 0.0
-#     distances = torch.maximum(distances, torch.zeros(distances.size()).to(device))
-
-#     if not squared:
-#         # Because the gradient of sqrt is infinite when distances == 0.0 (ex: on the diagonal)
-#         # we need to add a small epsilon where distances == 0.0
-#         mask = torch.eq(distances, torch.zeros(distances.size()).to(device)).float()
-#         distances = distances + mask * 1e-16
-
-#         distances = torch.sqrt(distances)
-
-#         # Correct the epsilon added: set the distances on the mask to be exactly 0.0
-#         distances = distances * (1.0 - mask)
-
-#     return distances
-
-def _pairwise_distances(embeddings, device, squared=False):
+def _pairwise_distances(embeddings, device):
     """Compute the 2D matrix of distances between all the embeddings.
     Args:
         embeddings: tensor of shape (batch_size, embed_dim)
-        squared: Boolean. If true, output is the pairwise squared euclidean distance matrix.
-                 If false, output is the pairwise euclidean distance matrix.
     Returns:
         pairwise_distances: tensor of shape (batch_size, batch_size)
     """
     distances = 1 - torch.nn.functional.cosine_similarity(embeddings[:,:,None], embeddings.t()[None,:,:])
 
     return distances
 
-# def arcosh(x):
-#     return torch.log(x + torch.sqrt(x**2 - 1))
-
-# def _pairwise_distances(u, squared=False):
-#     EPS=0.001
-#     uu = u.norm(dim=1)**2
-#     vv = u.norm(dim=1)**2
-#     uv = u.mm(u.t())
-#     alpha = 1-uu
-#     alpha = alpha.clamp(min=EPS)
-#     beta = 1-vv
-#     beta = beta.clamp(min=EPS)
-    
-#     gamma = 1 + 2 * (uu - 2 * uv + vv) / (alpha * beta)
-#     gamma = gamma.clamp(min=1+EPS)
-#     return arcosh(gamma)
-
-
 def _get_triplet_mask(labels, device):
     """Return a 3D mask where mask[a, p, n] is True iff the triplet (a, p, n) is valid.
     A triplet (i, j, k) is valid if:
         - i, j, k are distinct
         - labels[i] == labels[j] and labels[i] != labels[k]
     Args:
         labels: tf.int32 `Tensor` with shape [batch_size]
@@ -103,29 +43,27 @@
 
     # Combine the two masks
     mask = torch.logical_and(distinct_indices, valid_labels)
 
     return mask
 
 
-def batch_all_triplet_loss(labels, embeddings, margin, device, squared=False):
+def batch_all_triplet_loss(labels, embeddings, margin, device):
     """Build the triplet loss over a batch of embeddings.
     We generate all the valid triplets and average the loss over the positive ones.
     Args:
         labels: labels of the batch, of size (batch_size,)
         embeddings: tensor of shape (batch_size, embed_dim)
         margin: margin for triplet loss
-        squared: Boolean. If true, output is the pairwise squared euclidean distance matrix.
-                 If false, output is the pairwise euclidean distance matrix.
+    
     Returns:
         triplet_loss: scalar tensor containing the triplet loss
     """
     # Get the pairwise distance matrix
-    pairwise_dist = _pairwise_distances(embeddings, device, squared=squared)
-
+    pairwise_dist = _pairwise_distances(embeddings, device)
     # shape (batch_size, batch_size, 1)
     anchor_positive_dist = torch.unsqueeze(pairwise_dist, 2)
     assert anchor_positive_dist.size()[2] == 1, "{}".format(anchor_positive_dist.size())
     # shape (batch_size, 1, batch_size)
     anchor_negative_dist = torch.unsqueeze(pairwise_dist, 1)
     assert anchor_negative_dist.size()[1] == 1, "{}".format(anchor_negative_dist.size())
 
@@ -152,17 +90,17 @@
 
     # Get final mean triplet loss over the positive valid triplets
     triplet_loss = torch.sum(triplet_loss) / (num_positive_triplets + 1e-16)
 
     return triplet_loss, fraction_positive_triplets
 
 
-def fraction_triplets(labels, embeddings, margin, device, squared=False):
+def fraction_triplets(labels, embeddings, margin, device):
     # Get the pairwise distance matrix
-    pairwise_dist = _pairwise_distances(embeddings, device, squared=squared)
+    pairwise_dist = _pairwise_distances(embeddings, device)
 
     # shape (batch_size, batch_size, 1)
     anchor_positive_dist = torch.unsqueeze(pairwise_dist, 2)
     assert anchor_positive_dist.size()[2] == 1, "{}".format(anchor_positive_dist.size())
     # shape (batch_size, 1, batch_size)
     anchor_negative_dist = torch.unsqueeze(pairwise_dist, 1)
     assert anchor_negative_dist.size()[1] == 1, "{}".format(anchor_negative_dist.size())
@@ -191,28 +129,26 @@
     fraction_easy_triplets = num_easy_triplets / (num_valid_triplets + 1e-16)
     fraction_semi_hard_triplets = num_semi_hard_triplets / (num_valid_triplets + 1e-16)
     fraction_hard_triplets = num_hard_triplets / (num_valid_triplets + 1e-16)
     
     return fraction_easy_triplets, fraction_semi_hard_triplets, fraction_hard_triplets
 
 
-def batch_hard_triplet_loss(labels, embeddings, margin, semi, device, squared=False):
+def batch_hard_triplet_loss(labels, embeddings, margin, device):
     """Build the triplet loss over a batch of embeddings.
     For each anchor, we get the hardest positive and hardest negative to form a triplet.
     Args:
         labels: labels of the batch, of size (batch_size,)
         embeddings: tensor of shape (batch_size, embed_dim)
         margin: margin for triplet loss
-        squared: Boolean. If true, output is the pairwise squared euclidean distance matrix.
-                 If false, output is the pairwise euclidean distance matrix.
     Returns:
         triplet_loss: scalar tensor containing the triplet loss
     """
     # Get the pairwise distance matrix
-    pairwise_dist = _pairwise_distances(embeddings, device, squared=squared)
+    pairwise_dist = _pairwise_distances(embeddings, device)
 
     # shape (batch_size, batch_size, 1)
     anchor_positive_dist = torch.unsqueeze(pairwise_dist, 2)
     assert anchor_positive_dist.size()[2] == 1, "{}".format(anchor_positive_dist.size())
     # shape (batch_size, 1, batch_size)
     anchor_negative_dist = torch.unsqueeze(pairwise_dist, 1)
     assert anchor_negative_dist.size()[1] == 1, "{}".format(anchor_negative_dist.size())
@@ -227,24 +163,13 @@
     # (where label(a) != label(p) or label(n) == label(a) or a == p)
     mask = _get_triplet_mask(labels, device)
     mask = mask.float()
     triplet_loss = torch.multiply(mask, triplet_loss)
 
     # Remove negative losses (i.e. the easy triplets)
     triplet_loss[triplet_loss < 0] = 0
-    # Remove very hard losses (negative is) 
-    if semi:
-        triplet_loss[triplet_loss > margin] = 0
-        #accounts for case where all triplets are hard- dont want to include then. 
-        #mask[triplet_loss > margin] = 0
-    
+
     # max per anchor
     maxes = torch.amax(triplet_loss,dim=(1,2))
     triplet_loss = torch.mean(maxes[mask.sum(dim=(1,2)) > 0]) 
-    
-    #max per anchor-positive
-#     maxes = triplet_loss[mask.sum(dim=(2)) > 0].max(dim=1)[0]
-#     triplet_loss = torch.mean(maxes)
-#     if len(maxes) == 0:
-#         return 0 
-    
+
     return triplet_loss
```

### Comparing `cellmaps_coembedding-0.1.0a3/cellmaps_coembedding/runner.py` & `cellmaps_coembedding-0.1.0a4/cellmaps_coembedding/runner.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,87 +17,28 @@
 import cellmaps_coembedding
 import cellmaps_coembedding.muse_sc as muse
 from cellmaps_coembedding.exceptions import CellmapsCoEmbeddingError
 
 logger = logging.getLogger(__name__)
 
 
-class ImageEmbeddingFilterAndNameTranslator(object):
-    """
-    Converts image embedding names and filters keeping only
-    one per gene
-
-    """
-
-    def __init__(self, image_downloaddir=None):
-        """
-        Constructor
-        """
-        self._id_to_gene_mapping = self._gen_filtered_mapping(os.path.join(image_downloaddir,
-                                                                           constants.IMAGE_GENE_NODE_ATTR_FILE))
-
-    def _gen_filtered_mapping(self, image_gene_node_attrs_file):
-        """
-        Reads TSV file
-
-        :param image_gene_node_attrs_file:
-        :return:
-        """
-        mapping_dict = {}
-        with open(image_gene_node_attrs_file, 'r') as f:
-            reader = csv.DictReader(f, delimiter='\t')
-            for row in reader:
-                mapping_dict[row['filename'].split(',')[0]] = row['name']
-        return mapping_dict
-
-    def get_name_mapping(self):
-        """
-        Gets mapping of old name to new name
-
-        :return: mapping of old name to new name
-        :rtype: dict
-        """
-        return self._id_to_gene_mapping
-
-    def translate(self, embeddings):
-        """
-        Translates and filters out embeddings
-        with duplicate gene names. Updated embeddings are returned
-        :param embeddings: list of list of embeddings
-        :type embeddings: list
-        :return: embeddings
-        :rtype: list
-        """
-        res_embeddings = []
-
-        for row in embeddings:
-            if row[0] not in self._id_to_gene_mapping:
-                continue
-            new_row = row.copy()
-            new_row[0] = self._id_to_gene_mapping[row[0]]
-            res_embeddings.append(new_row)
-        return res_embeddings
-
 
 class EmbeddingGenerator(object):
     """
     Base class for implementations that generate
     network embeddings
     """
     def __init__(self, dimensions=1024,
                  ppi_embeddingdir=None,
                  image_embeddingdir=None,
-                 image_downloaddir=None,
-                 img_emd_translator=None):
+                 ):
         """
         Constructor
         """
         self._dimensions = dimensions
-        if img_emd_translator is None:
-            self._img_emd_translator = ImageEmbeddingFilterAndNameTranslator(image_downloaddir=image_downloaddir)
         self._ppi_embeddingdir = ppi_embeddingdir
         self._image_embeddingdir = image_embeddingdir
 
     def _get_ppi_embeddings_file(self):
         """
 
         :return:
@@ -164,21 +105,15 @@
         """
         Gets number of dimensions this embedding will generate
 
         :return: number of dimensions aka vector length
         :rtype: int
         """
         return self._dimensions
-
-    def get_name_mapping(self):
-        """
-
-        :return:
-        """
-        return self._img_emd_translator.get_oldname_to_new_name_mapping()
+    
 
     def get_next_embedding(self):
         """
         Generator method for getting next embedding.
         Caller should implement with ``yield`` operator
 
         :raises: NotImplementedError: Subclasses should implement this
@@ -189,61 +124,52 @@
 
 
 class MuseCoEmbeddingGenerator(EmbeddingGenerator):
     """
     Generats co-embedding using MUSE
     """
     def __init__(self, dimensions=128,
-                 k=10, min_diff=0.2, dropout=0.25, n_epochs=500,
+                 k=10, triplet_margin=0.1, dropout=0.25, n_epochs=500,
                  n_epochs_init=200,
                  outdir=None,
                  ppi_embeddingdir=None,
-                 image_embeddingdir=None,
-                 image_downloaddir=None,
-                 img_emd_translator=None):
+                 image_embeddingdir=None
+                ):
         """
 
         :param dimensions:
         :param k: k nearest neighbors value used for clustering - clustering used for triplet loss
-        :param min_diff: margin for triplet loss
+        :param triplet_margin: margin for triplet loss
         :param dropout: dropout between neural net layers
         :param n_epochs: training epochs
         :param n_epochs_init: initialization training epochs
         :param outdir:
         :param ppi_embeddingdir:
         :param image_embeddingdir:
-        :param image_downloaddir:
-        :param img_emd_translator:
         """
         super().__init__(dimensions=dimensions,
                          ppi_embeddingdir=ppi_embeddingdir,
-                         image_embeddingdir=image_embeddingdir,
-                         image_downloaddir=image_downloaddir,
-                         img_emd_translator=img_emd_translator)
+                         image_embeddingdir=image_embeddingdir)
         self._outdir = outdir
         self._k = k
-        self._min_diff = min_diff
+        self.triplet_margin = triplet_margin
         self._dropout = dropout
         self._n_epochs = n_epochs
         self._n_epochs_init = n_epochs_init
 
     def get_next_embedding(self):
         """
 
         :return:
         """
         ppi_embeddings = self._get_ppi_embeddings()
         ppi_embeddings.sort(key=lambda x: x[0])
         logger.info('There are ' + str(len(ppi_embeddings)) + ' PPI embeddings')
-        raw_embeddings = self._get_image_embeddings()
-        logger.info('There are ' + str(len(raw_embeddings)) + ' raw image embeddings')
-
-        image_embeddings = self._img_emd_translator.translate(raw_embeddings)
-        logger.info('There are ' + str(len(image_embeddings)) +
-                    ' translated and filtered image embeddings')
+        image_embeddings = self._get_image_embeddings()
+        logger.info('There are ' + str(len(image_embeddings)) + ' image embeddings')
         image_embeddings.sort(key=lambda x: x[0])
         ppi_name_set = self._get_set_of_embedding_names(ppi_embeddings)
         image_name_set = self._get_set_of_embedding_names(image_embeddings)
         intersection_name_set = ppi_name_set.intersection(image_name_set)
         logger.info('There are ' +
                     str(len(intersection_name_set)) +
                     ' overlapping embeddings')
@@ -252,59 +178,52 @@
 
         ppi_embeddings_array = np.array([np.array([float(e) for e in xi[1:]]) for xi in ppi_embeddings if xi[0] in intersection_name_set])
         image_embeddings_array = np.array([np.array([float(e) for e in xi[1:]]) for xi in image_embeddings if xi[0] in intersection_name_set])
 
         resultsdir = os.path.join(self._outdir, 'muse')
 
         model, res_embedings = muse.muse_fit_predict(resultsdir=resultsdir,
-                                                     index=name_index, data_x=ppi_embeddings_array,
+                                                     data_x=ppi_embeddings_array,
                                                      data_y=image_embeddings_array,
+                                                     name_index=name_index, 
                                                      latent_dim=self.get_dimensions(),
                                                      n_epochs=self._n_epochs,
                                                      n_epochs_init=self._n_epochs_init,
-                                                     min_diff=self._min_diff,
+                                                     triplet_margin=self.triplet_margin,
                                                      k=self._k, dropout=self._dropout)
         for index, embedding in enumerate(res_embedings):
             row = [name_index[index]]
             row.extend(embedding)
             yield row
 
 
 class FakeCoEmbeddingGenerator(EmbeddingGenerator):
     """
     Generates a fake coembedding
     """
     def __init__(self, dimensions=128, ppi_embeddingdir=None,
-                 image_embeddingdir=None,
-                 image_downloaddir=None,
-                 img_emd_translator=None):
+                 image_embeddingdir=None):
         """
         Constructor
         :param dimensions:
         """
         super().__init__(dimensions=dimensions,
                          ppi_embeddingdir=ppi_embeddingdir,
-                         image_embeddingdir=image_embeddingdir,
-                         image_downloaddir=image_downloaddir,
-                         img_emd_translator=img_emd_translator)
+                         image_embeddingdir=image_embeddingdir)
 
     def get_next_embedding(self):
         """
         Gets next embedding
 
         :return:
         """
         ppi_embeddings = self._get_ppi_embeddings()
         logger.info('There are ' + str(len(ppi_embeddings)) + ' PPI embeddings')
-        raw_embeddings = self._get_image_embeddings()
-        logger.info('There are ' + str(len(raw_embeddings)) + ' raw image embeddings')
-
-        image_embeddings = self._img_emd_translator.translate(raw_embeddings)
-        logger.info('There are ' + str(len(image_embeddings)) +
-                    ' translated and filtered image embeddings')
+        image_embeddings = self._get_image_embeddings()
+        logger.info('There are ' + str(len(image_embeddings)) + ' image embeddings')
 
         ppi_embedding_names = self._get_set_of_embedding_names(ppi_embeddings)
         image_embedding_names = self._get_set_of_embedding_names(image_embeddings)
         intersection_embedding_names = ppi_embedding_names.intersection(image_embedding_names)
         logger.info('There are ' +
                     str(len(intersection_embedding_names)) +
                     ' overlapping embeddings')
```

### Comparing `cellmaps_coembedding-0.1.0a3/cellmaps_coembedding.egg-info/PKG-INFO` & `cellmaps_coembedding-0.1.0a4/cellmaps_coembedding.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: cellmaps-coembedding
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: A tool to generate coembeddings from IF image embeddings and PPI network embeddings
 Home-page: https://github.com/idekerlab/cellmaps_coembedding
-Author: Leah Schaffer
-Author-email: lvschaffer@health.ucsd.edu
+Author: Ideker Lab CM4AI team
+Author-email: tools@cm4ai.org
 License: MIT license
-Description: ==================
-        CM4AI CoEmbedding
-        ==================
+Description: =====================
+        Cell Maps CoEmbedder
+        =====================
         
         
         .. image:: https://img.shields.io/pypi/v/cellmaps_coembedding.svg
                 :target: https://pypi.python.org/pypi/cellmaps_coembedding
         
         .. image:: https://img.shields.io/travis/idekerlab/cellmaps_coembedding.svg
                 :target: https://travis-ci.com/idekerlab/cellmaps_coembedding
         
         .. image:: https://readthedocs.org/projects/cellmaps-generate-ppi/badge/?version=latest
                 :target: https://cellmaps-generate-ppi.readthedocs.io/en/latest/?badge=latest
                 :alt: Documentation Status
         
-        A tool to generate coembeddings from IF image embeddings and PPI network embeddings
-        
+        Creates Coembedding from `Cell Maps ImmunoFluorscent Image Embedder <https://cellmaps-image-embedding.readthedocs.io>`__
+        and `Cell Maps PPI Embedder <https://cellmaps-ppi-embedding.readthedocs.io>`__ for `Cell Maps for AI (CM4AI) <https://cm4ai.org>`__
         
         * Free software: MIT license
         * Documentation: https://cellmaps-coembedding.readthedocs.io.
         
         
         
         Dependencies
@@ -51,15 +51,15 @@
         ------------
         
         .. code-block::
         
            git clone https://github.com/idekerlab/cellmaps_coembedding
            cd cellmaps_coembedding
            make dist
-           pip install dist/cellmaps_coembeddingcmd*whl
+           pip install dist/cellmaps_coembedding*whl
         
         
         Run **make** command with no arguments to see other build/deploy options including creation of Docker image 
         
         .. code-block::
         
            make
```

### Comparing `cellmaps_coembedding-0.1.0a3/cellmaps_coembedding.egg-info/SOURCES.txt` & `cellmaps_coembedding-0.1.0a4/cellmaps_coembedding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a3/docs/Makefile` & `cellmaps_coembedding-0.1.0a4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a3/docs/cellmaps_coembedding.muse_sc.rst` & `cellmaps_coembedding-0.1.0a4/docs/cellmaps_coembedding.muse_sc.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a3/docs/cellmaps_coembedding.rst` & `cellmaps_coembedding-0.1.0a4/docs/cellmaps_coembedding.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a3/docs/conf.py` & `cellmaps_coembedding-0.1.0a4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a3/docs/installation.rst` & `cellmaps_coembedding-0.1.0a4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a3/docs/make.bat` & `cellmaps_coembedding-0.1.0a4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a3/docs/newrelease.rst` & `cellmaps_coembedding-0.1.0a4/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a3/docs/pypircfile.rst` & `cellmaps_coembedding-0.1.0a4/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a3/docs/usage.rst` & `cellmaps_coembedding-0.1.0a4/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a3/docs/versioningscheme.rst` & `cellmaps_coembedding-0.1.0a4/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a3/setup.py` & `cellmaps_coembedding-0.1.0a4/setup.py`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a3/tests/test_cellmaps_coembeddingcmd.py` & `cellmaps_coembedding-0.1.0a4/tests/test_cellmaps_coembeddingcmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a3/tests/test_cellmapscoembedder.py` & `cellmaps_coembedding-0.1.0a4/tests/test_cellmapscoembedder.py`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a3/tests/test_imagembeddingfilterandnametranslator.py` & `cellmaps_coembedding-0.1.0a4/tests/test_imagembeddingfilterandnametranslator.py`

 * *Files identical despite different names*

### Comparing `cellmaps_coembedding-0.1.0a3/tests/test_integration_cellmaps_coembedding.py` & `cellmaps_coembedding-0.1.0a4/tests/test_integration_cellmaps_coembedding.py`

 * *Files identical despite different names*

