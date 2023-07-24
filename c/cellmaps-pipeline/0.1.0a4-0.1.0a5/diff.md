# Comparing `tmp/cellmaps_pipeline-0.1.0a4.tar.gz` & `tmp/cellmaps_pipeline-0.1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_pipeline-0.1.0a4.tar", last modified: Mon Jul 17 20:25:45 2023, max compression
+gzip compressed data, was "dist/cellmaps_pipeline-0.1.0a5.tar", last modified: Mon Jul 24 23:42:38 2023, max compression
```

## Comparing `cellmaps_pipeline-0.1.0a4.tar` & `cellmaps_pipeline-0.1.0a5.tar`

### file list

```diff
@@ -1,51 +1,55 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 20:25:45.624572 cellmaps_pipeline-0.1.0a4/
--rw-r--r--   0 churas     (504) staff       (20)      266 2023-06-08 20:06:13.000000 cellmaps_pipeline-0.1.0a4/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3641 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a4/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-22 23:49:21.000000 cellmaps_pipeline-0.1.0a4/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a4/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a4/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     6042 2023-07-17 20:25:45.624699 cellmaps_pipeline-0.1.0a4/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     4016 2023-06-07 18:25:27.000000 cellmaps_pipeline-0.1.0a4/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 20:25:45.616629 cellmaps_pipeline-0.1.0a4/cellmaps_pipeline/
--rw-r--r--   0 churas     (504) staff       (20)      279 2023-07-17 20:25:30.000000 cellmaps_pipeline-0.1.0a4/cellmaps_pipeline/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     8923 2023-07-17 20:25:30.000000 cellmaps_pipeline-0.1.0a4/cellmaps_pipeline/cellmaps_pipelinecmd.py
--rw-r--r--   0 churas     (504) staff       (20)      132 2023-04-04 23:01:54.000000 cellmaps_pipeline-0.1.0a4/cellmaps_pipeline/exceptions.py
--rw-r--r--   0 churas     (504) staff       (20)    12687 2023-07-17 20:25:30.000000 cellmaps_pipeline-0.1.0a4/cellmaps_pipeline/runner.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 20:25:45.617928 cellmaps_pipeline-0.1.0a4/cellmaps_pipeline.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     6042 2023-07-17 20:25:45.000000 cellmaps_pipeline-0.1.0a4/cellmaps_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     1024 2023-07-17 20:25:45.000000 cellmaps_pipeline-0.1.0a4/cellmaps_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-07-17 20:25:45.000000 cellmaps_pipeline-0.1.0a4/cellmaps_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-07-17 20:25:45.000000 cellmaps_pipeline-0.1.0a4/cellmaps_pipeline.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)      243 2023-07-17 20:25:45.000000 cellmaps_pipeline-0.1.0a4/cellmaps_pipeline.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       18 2023-07-17 20:25:45.000000 cellmaps_pipeline-0.1.0a4/cellmaps_pipeline.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 20:25:45.622638 cellmaps_pipeline-0.1.0a4/docs/
--rw-r--r--   0 churas     (504) staff       (20)      618 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/Makefile
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 20:25:45.613670 cellmaps_pipeline-0.1.0a4/docs/_build/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 20:25:45.613741 cellmaps_pipeline-0.1.0a4/docs/_build/html/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 20:25:45.623331 cellmaps_pipeline-0.1.0a4/docs/_build/html/_static/
--rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a4/docs/_build/html/_static/file.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a4/docs/_build/html/_static/minus.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a4/docs/_build/html/_static/plus.png
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/authors.rst
--rw-r--r--   0 churas     (504) staff       (20)      744 2023-05-22 23:59:43.000000 cellmaps_pipeline-0.1.0a4/docs/cellmaps_pipeline.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     6035 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      285 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/history.rst
--rw-r--r--   0 churas     (504) staff       (20)      934 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1189 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      451 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      815 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       76 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4340 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      787 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)      687 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      400 2023-07-17 20:25:45.625693 cellmaps_pipeline-0.1.0a4/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     2460 2023-07-17 20:25:30.000000 cellmaps_pipeline-0.1.0a4/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-17 20:25:45.624362 cellmaps_pipeline-0.1.0a4/tests/
--rw-r--r--   0 churas     (504) staff       (20)       72 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a4/tests/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     1296 2023-06-07 18:25:27.000000 cellmaps_pipeline-0.1.0a4/tests/test_cellmaps_pipelinecmd.py
--rw-r--r--   0 churas     (504) staff       (20)      896 2023-06-07 18:25:27.000000 cellmaps_pipeline-0.1.0a4/tests/test_cellmapspipeline.py
--rw-r--r--   0 churas     (504) staff       (20)      772 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a4/tests/test_integration_cellmaps_pipeline.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:42:38.562969 cellmaps_pipeline-0.1.0a5/
+-rw-r--r--   0 churas     (504) staff       (20)      266 2023-06-08 20:06:13.000000 cellmaps_pipeline-0.1.0a5/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3641 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a5/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-22 23:49:21.000000 cellmaps_pipeline-0.1.0a5/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a5/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a5/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     6081 2023-07-24 23:42:38.563137 cellmaps_pipeline-0.1.0a5/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     4079 2023-07-17 23:45:49.000000 cellmaps_pipeline-0.1.0a5/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:42:38.554401 cellmaps_pipeline-0.1.0a5/cellmaps_pipeline/
+-rw-r--r--   0 churas     (504) staff       (20)      279 2023-07-24 23:42:04.000000 cellmaps_pipeline-0.1.0a5/cellmaps_pipeline/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     8923 2023-07-17 20:25:30.000000 cellmaps_pipeline-0.1.0a5/cellmaps_pipeline/cellmaps_pipelinecmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      132 2023-04-04 23:01:54.000000 cellmaps_pipeline-0.1.0a5/cellmaps_pipeline/exceptions.py
+-rw-r--r--   0 churas     (504) staff       (20)    12687 2023-07-17 20:25:30.000000 cellmaps_pipeline-0.1.0a5/cellmaps_pipeline/runner.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:42:38.555945 cellmaps_pipeline-0.1.0a5/cellmaps_pipeline.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     6081 2023-07-24 23:42:38.000000 cellmaps_pipeline-0.1.0a5/cellmaps_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     1105 2023-07-24 23:42:38.000000 cellmaps_pipeline-0.1.0a5/cellmaps_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-07-24 23:42:38.000000 cellmaps_pipeline-0.1.0a5/cellmaps_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-07-24 23:42:38.000000 cellmaps_pipeline-0.1.0a5/cellmaps_pipeline.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)      243 2023-07-24 23:42:38.000000 cellmaps_pipeline-0.1.0a5/cellmaps_pipeline.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       18 2023-07-24 23:42:38.000000 cellmaps_pipeline-0.1.0a5/cellmaps_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:42:38.560254 cellmaps_pipeline-0.1.0a5/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      618 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a5/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:42:38.551017 cellmaps_pipeline-0.1.0a5/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:42:38.551245 cellmaps_pipeline-0.1.0a5/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:42:38.560514 cellmaps_pipeline-0.1.0a5/docs/_build/html/_images/
+-rw-r--r--   0 churas     (504) staff       (20)    29975 2023-07-18 21:25:06.000000 cellmaps_pipeline-0.1.0a5/docs/_build/html/_images/pipeline_overview.png
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:42:38.561359 cellmaps_pipeline-0.1.0a5/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a5/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a5/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a5/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a5/docs/authors.rst
+-rw-r--r--   0 churas     (504) staff       (20)      744 2023-05-22 23:59:43.000000 cellmaps_pipeline-0.1.0a5/docs/cellmaps_pipeline.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     6035 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a5/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a5/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a5/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      285 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a5/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a5/docs/history.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:42:38.561608 cellmaps_pipeline-0.1.0a5/docs/images/
+-rw-r--r--   0 churas     (504) staff       (20)    29975 2023-07-18 21:25:06.000000 cellmaps_pipeline-0.1.0a5/docs/images/pipeline_overview.png
+-rw-r--r--   0 churas     (504) staff       (20)     1783 2023-07-18 21:44:38.000000 cellmaps_pipeline-0.1.0a5/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1189 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a5/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      451 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a5/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      815 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a5/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       76 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a5/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4340 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a5/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      787 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a5/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)      653 2023-07-18 21:56:02.000000 cellmaps_pipeline-0.1.0a5/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a5/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      400 2023-07-24 23:42:38.564432 cellmaps_pipeline-0.1.0a5/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     2460 2023-07-24 23:41:04.000000 cellmaps_pipeline-0.1.0a5/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-07-24 23:42:38.562735 cellmaps_pipeline-0.1.0a5/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       72 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a5/tests/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     1296 2023-06-07 18:25:27.000000 cellmaps_pipeline-0.1.0a5/tests/test_cellmaps_pipelinecmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      896 2023-06-07 18:25:27.000000 cellmaps_pipeline-0.1.0a5/tests/test_cellmapspipeline.py
+-rw-r--r--   0 churas     (504) staff       (20)      772 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a5/tests/test_integration_cellmaps_pipeline.py
```

### Comparing `cellmaps_pipeline-0.1.0a4/CONTRIBUTING.rst` & `cellmaps_pipeline-0.1.0a5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a4/LICENSE` & `cellmaps_pipeline-0.1.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a4/PKG-INFO` & `cellmaps_pipeline-0.1.0a5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 Metadata-Version: 2.1
 Name: cellmaps_pipeline
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: Runs full Cellmaps CM4AI pipeline
 Home-page: https://github.com/idekerlab/cellmaps_pipeline
 Author: Ideker Lab CM4AI team
 Author-email: tools@cm4ai.org
 License: MIT license
-Description: ==============
-        CM4AI Pipeline
-        ==============
+Description: ===================
+        Cell Maps Pipeline
+        ===================
         
         
         .. image:: https://img.shields.io/pypi/v/cellmaps_pipeline.svg
                 :target: https://pypi.python.org/pypi/cellmaps_pipeline
         
         .. image:: https://img.shields.io/travis/idekerlab/cellmaps_pipeline.svg
                 :target: https://travis-ci.com/idekerlab/cellmaps_pipeline
         
         .. image:: https://readthedocs.org/projects/cellmaps-pipeline/badge/?version=latest
                 :target: https://cellmaps-pipeline.readthedocs.io/en/latest/?badge=latest
                 :alt: Documentation Status
         
-        
-        
-        
-        Runs CM4AI pipeline
+        Cell Maps Pipeline for `Cell Maps for AI (CM4AI) <https://cm4ai.org>`__
         
         * Free software: MIT license
         * Documentation: https://cellmaps-pipeline.readthedocs.io.
         
         Dependencies
         ------------
```

### Comparing `cellmaps_pipeline-0.1.0a4/README.rst` & `cellmaps_pipeline-0.1.0a5/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,23 @@
-==============
-CM4AI Pipeline
-==============
+===================
+Cell Maps Pipeline
+===================
 
 
 .. image:: https://img.shields.io/pypi/v/cellmaps_pipeline.svg
         :target: https://pypi.python.org/pypi/cellmaps_pipeline
 
 .. image:: https://img.shields.io/travis/idekerlab/cellmaps_pipeline.svg
         :target: https://travis-ci.com/idekerlab/cellmaps_pipeline
 
 .. image:: https://readthedocs.org/projects/cellmaps-pipeline/badge/?version=latest
         :target: https://cellmaps-pipeline.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
-
-
-
-Runs CM4AI pipeline
+Cell Maps Pipeline for `Cell Maps for AI (CM4AI) <https://cm4ai.org>`__
 
 * Free software: MIT license
 * Documentation: https://cellmaps-pipeline.readthedocs.io.
 
 Dependencies
 ------------
```

### Comparing `cellmaps_pipeline-0.1.0a4/cellmaps_pipeline/cellmaps_pipelinecmd.py` & `cellmaps_pipeline-0.1.0a5/cellmaps_pipeline/cellmaps_pipelinecmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a4/cellmaps_pipeline/runner.py` & `cellmaps_pipeline-0.1.0a5/cellmaps_pipeline/runner.py`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a4/cellmaps_pipeline.egg-info/PKG-INFO` & `cellmaps_pipeline-0.1.0a5/cellmaps_pipeline.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 Metadata-Version: 2.1
 Name: cellmaps-pipeline
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: Runs full Cellmaps CM4AI pipeline
 Home-page: https://github.com/idekerlab/cellmaps_pipeline
 Author: Ideker Lab CM4AI team
 Author-email: tools@cm4ai.org
 License: MIT license
-Description: ==============
-        CM4AI Pipeline
-        ==============
+Description: ===================
+        Cell Maps Pipeline
+        ===================
         
         
         .. image:: https://img.shields.io/pypi/v/cellmaps_pipeline.svg
                 :target: https://pypi.python.org/pypi/cellmaps_pipeline
         
         .. image:: https://img.shields.io/travis/idekerlab/cellmaps_pipeline.svg
                 :target: https://travis-ci.com/idekerlab/cellmaps_pipeline
         
         .. image:: https://readthedocs.org/projects/cellmaps-pipeline/badge/?version=latest
                 :target: https://cellmaps-pipeline.readthedocs.io/en/latest/?badge=latest
                 :alt: Documentation Status
         
-        
-        
-        
-        Runs CM4AI pipeline
+        Cell Maps Pipeline for `Cell Maps for AI (CM4AI) <https://cm4ai.org>`__
         
         * Free software: MIT license
         * Documentation: https://cellmaps-pipeline.readthedocs.io.
         
         Dependencies
         ------------
```

### Comparing `cellmaps_pipeline-0.1.0a4/cellmaps_pipeline.egg-info/SOURCES.txt` & `cellmaps_pipeline-0.1.0a5/cellmaps_pipeline.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 docs/integrationtesting.rst
 docs/make.bat
 docs/modules.rst
 docs/newrelease.rst
 docs/pypircfile.rst
 docs/usage.rst
 docs/versioningscheme.rst
+docs/_build/html/_images/pipeline_overview.png
 docs/_build/html/_static/file.png
 docs/_build/html/_static/minus.png
 docs/_build/html/_static/plus.png
+docs/images/pipeline_overview.png
 tests/__init__.py
 tests/test_cellmaps_pipelinecmd.py
 tests/test_cellmapspipeline.py
 tests/test_integration_cellmaps_pipeline.py
```

### Comparing `cellmaps_pipeline-0.1.0a4/docs/Makefile` & `cellmaps_pipeline-0.1.0a5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a4/docs/cellmaps_pipeline.rst` & `cellmaps_pipeline-0.1.0a5/docs/cellmaps_pipeline.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a4/docs/conf.py` & `cellmaps_pipeline-0.1.0a5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a4/docs/installation.rst` & `cellmaps_pipeline-0.1.0a5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a4/docs/make.bat` & `cellmaps_pipeline-0.1.0a5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a4/docs/newrelease.rst` & `cellmaps_pipeline-0.1.0a5/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a4/docs/pypircfile.rst` & `cellmaps_pipeline-0.1.0a5/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a4/docs/usage.rst` & `cellmaps_pipeline-0.1.0a5/docs/usage.rst`

 * *Files 26% similar despite different names*

```diff
@@ -18,22 +18,10 @@
 
 **Example usage**
 
 **TODO:** Add information about example usage
 
 .. code-block::
 
-   cellmaps_pipelinecmd.py # TODO Add other needed arguments here
-
-Via Docker
----------------
-
-**Example usage**
-
-**TODO:** Add information about example usage
-
-
-.. code-block::
-
-   docker run -v `pwd`:`pwd` -w `pwd` idekerlab/cellmaps_pipeline:0.1.0 cellmaps_pipelinecmd.py # TODO Add other needed arguments here
-
-
+   cellmaps_pipelinecmd.py toyrun --samples example/samples.csv --unique example/unique.csv \
+                           --baitlist example/baitlist.tsv --edgelist example/edgelist.tsv \
+                           --provenance example/provenance.json --model_path example/model.pth
```

### Comparing `cellmaps_pipeline-0.1.0a4/docs/versioningscheme.rst` & `cellmaps_pipeline-0.1.0a5/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a4/setup.py` & `cellmaps_pipeline-0.1.0a5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     history = history_file.read()
 
 requirements = ['cellmaps_utils==0.1.0a13',
                 'cellmaps_imagedownloader==0.1.0a6',
                 'cellmaps_ppidownloader==0.1.0a3',
                 'cellmaps_image_embedding==0.1.0a7',
                 'cellmaps_ppi_embedding==0.1.0a4',
-                'cellmaps_coembedding==0.1.0a3',
+                'cellmaps_coembedding==0.1.0a4',
                 'cellmaps_generate_hierarchy==0.1.0a6',
                 'networkx>=2.8,<2.9']
 
 setup_requirements = [ ]
 
 test_requirements = [ ]
```

### Comparing `cellmaps_pipeline-0.1.0a4/tests/test_cellmaps_pipelinecmd.py` & `cellmaps_pipeline-0.1.0a5/tests/test_cellmaps_pipelinecmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a4/tests/test_cellmapspipeline.py` & `cellmaps_pipeline-0.1.0a5/tests/test_cellmapspipeline.py`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a4/tests/test_integration_cellmaps_pipeline.py` & `cellmaps_pipeline-0.1.0a5/tests/test_integration_cellmaps_pipeline.py`

 * *Files identical despite different names*

