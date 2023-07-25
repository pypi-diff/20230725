# Comparing `tmp/ocr_iiif_tools-0.0.8.tar.gz` & `tmp/ocr_iiif_tools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocr_iiif_tools-0.0.8.tar", last modified: Wed Jun 28 04:19:14 2023, max compression
+gzip compressed data, was "ocr_iiif_tools-0.0.9.tar", last modified: Wed Jun 28 04:26:12 2023, max compression
```

## Comparing `ocr_iiif_tools-0.0.8.tar` & `ocr_iiif_tools-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-28 04:19:14.799333 ocr_iiif_tools-0.0.8/
--rw-rw-r--   0 nakamura   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ocr_iiif_tools-0.0.8/LICENSE
--rw-rw-r--   0 nakamura   (501) staff       (20)      111 2023-04-27 10:12:58.000000 ocr_iiif_tools-0.0.8/MANIFEST.in
--rw-r--r--   0 nakamura   (501) staff       (20)     1110 2023-06-28 04:19:14.799137 ocr_iiif_tools-0.0.8/PKG-INFO
--rw-r--r--   0 nakamura   (501) staff       (20)      339 2023-06-25 23:33:01.000000 ocr_iiif_tools-0.0.8/README.md
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-28 04:19:14.795059 ocr_iiif_tools-0.0.8/iida/
--rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-20 21:23:20.000000 ocr_iiif_tools-0.0.8/iida/__init__.py
--rw-r--r--   0 nakamura   (501) staff       (20)      912 2023-06-20 21:23:20.000000 ocr_iiif_tools-0.0.8/iida/_modidx.py
--rw-r--r--   0 nakamura   (501) staff       (20)     5262 2023-06-20 21:23:20.000000 ocr_iiif_tools-0.0.8/iida/core.py
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-28 04:19:14.795819 ocr_iiif_tools-0.0.8/ocr_iiif/
--rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-20 20:09:43.000000 ocr_iiif_tools-0.0.8/ocr_iiif/__init__.py
--rw-r--r--   0 nakamura   (501) staff       (20)     1173 2023-06-20 20:11:42.000000 ocr_iiif_tools-0.0.8/ocr_iiif/_modidx.py
--rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-20 20:11:42.000000 ocr_iiif_tools-0.0.8/ocr_iiif/core.py
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-28 04:19:14.797094 ocr_iiif_tools-0.0.8/ocr_iiif_tools/
--rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-27 08:28:44.000000 ocr_iiif_tools-0.0.8/ocr_iiif_tools/__init__.py
--rw-r--r--   0 nakamura   (501) staff       (20)     4457 2023-06-27 08:28:44.000000 ocr_iiif_tools-0.0.8/ocr_iiif_tools/_modidx.py
--rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-27 08:28:44.000000 ocr_iiif_tools-0.0.8/ocr_iiif_tools/core.py
--rw-r--r--   0 nakamura   (501) staff       (20)    22014 2023-06-27 08:28:44.000000 ocr_iiif_tools-0.0.8/ocr_iiif_tools/pdf.py
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-28 04:19:14.798722 ocr_iiif_tools-0.0.8/ocr_iiif_tools.egg-info/
--rw-r--r--   0 nakamura   (501) staff       (20)     1110 2023-06-28 04:19:14.000000 ocr_iiif_tools-0.0.8/ocr_iiif_tools.egg-info/PKG-INFO
--rw-r--r--   0 nakamura   (501) staff       (20)      520 2023-06-28 04:19:14.000000 ocr_iiif_tools-0.0.8/ocr_iiif_tools.egg-info/SOURCES.txt
--rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-28 04:19:14.000000 ocr_iiif_tools-0.0.8/ocr_iiif_tools.egg-info/dependency_links.txt
--rw-r--r--   0 nakamura   (501) staff       (20)       71 2023-06-28 04:19:14.000000 ocr_iiif_tools-0.0.8/ocr_iiif_tools.egg-info/entry_points.txt
--rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-20 20:10:31.000000 ocr_iiif_tools-0.0.8/ocr_iiif_tools.egg-info/not-zip-safe
--rw-r--r--   0 nakamura   (501) staff       (20)       31 2023-06-28 04:19:14.000000 ocr_iiif_tools-0.0.8/ocr_iiif_tools.egg-info/requires.txt
--rw-r--r--   0 nakamura   (501) staff       (20)       29 2023-06-28 04:19:14.000000 ocr_iiif_tools-0.0.8/ocr_iiif_tools.egg-info/top_level.txt
--rw-r--r--   0 nakamura   (501) staff       (20)      931 2023-06-28 04:16:58.000000 ocr_iiif_tools-0.0.8/settings.ini
--rw-r--r--   0 nakamura   (501) staff       (20)       38 2023-06-28 04:19:14.799398 ocr_iiif_tools-0.0.8/setup.cfg
--rw-rw-r--   0 nakamura   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 ocr_iiif_tools-0.0.8/setup.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-28 04:26:12.062022 ocr_iiif_tools-0.0.9/
+-rw-rw-r--   0 nakamura   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ocr_iiif_tools-0.0.9/LICENSE
+-rw-rw-r--   0 nakamura   (501) staff       (20)      111 2023-04-27 10:12:58.000000 ocr_iiif_tools-0.0.9/MANIFEST.in
+-rw-r--r--   0 nakamura   (501) staff       (20)     1110 2023-06-28 04:26:12.061867 ocr_iiif_tools-0.0.9/PKG-INFO
+-rw-r--r--   0 nakamura   (501) staff       (20)      339 2023-06-25 23:33:01.000000 ocr_iiif_tools-0.0.9/README.md
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-28 04:26:12.059731 ocr_iiif_tools-0.0.9/iida/
+-rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-20 21:23:20.000000 ocr_iiif_tools-0.0.9/iida/__init__.py
+-rw-r--r--   0 nakamura   (501) staff       (20)      912 2023-06-20 21:23:20.000000 ocr_iiif_tools-0.0.9/iida/_modidx.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     5262 2023-06-20 21:23:20.000000 ocr_iiif_tools-0.0.9/iida/core.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-28 04:26:12.060150 ocr_iiif_tools-0.0.9/ocr_iiif/
+-rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-20 20:09:43.000000 ocr_iiif_tools-0.0.9/ocr_iiif/__init__.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     1173 2023-06-20 20:11:42.000000 ocr_iiif_tools-0.0.9/ocr_iiif/_modidx.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-20 20:11:42.000000 ocr_iiif_tools-0.0.9/ocr_iiif/core.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-28 04:26:12.060689 ocr_iiif_tools-0.0.9/ocr_iiif_tools/
+-rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-27 08:28:44.000000 ocr_iiif_tools-0.0.9/ocr_iiif_tools/__init__.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     4457 2023-06-27 08:28:44.000000 ocr_iiif_tools-0.0.9/ocr_iiif_tools/_modidx.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-27 08:28:44.000000 ocr_iiif_tools-0.0.9/ocr_iiif_tools/core.py
+-rw-r--r--   0 nakamura   (501) staff       (20)    22014 2023-06-27 08:28:44.000000 ocr_iiif_tools-0.0.9/ocr_iiif_tools/pdf.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-28 04:26:12.061658 ocr_iiif_tools-0.0.9/ocr_iiif_tools.egg-info/
+-rw-r--r--   0 nakamura   (501) staff       (20)     1110 2023-06-28 04:26:12.000000 ocr_iiif_tools-0.0.9/ocr_iiif_tools.egg-info/PKG-INFO
+-rw-r--r--   0 nakamura   (501) staff       (20)      520 2023-06-28 04:26:12.000000 ocr_iiif_tools-0.0.9/ocr_iiif_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-28 04:26:12.000000 ocr_iiif_tools-0.0.9/ocr_iiif_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)       71 2023-06-28 04:26:12.000000 ocr_iiif_tools-0.0.9/ocr_iiif_tools.egg-info/entry_points.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-20 20:10:31.000000 ocr_iiif_tools-0.0.9/ocr_iiif_tools.egg-info/not-zip-safe
+-rw-r--r--   0 nakamura   (501) staff       (20)       38 2023-06-28 04:26:12.000000 ocr_iiif_tools-0.0.9/ocr_iiif_tools.egg-info/requires.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)       29 2023-06-28 04:26:12.000000 ocr_iiif_tools-0.0.9/ocr_iiif_tools.egg-info/top_level.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)      938 2023-06-28 04:23:53.000000 ocr_iiif_tools-0.0.9/settings.ini
+-rw-r--r--   0 nakamura   (501) staff       (20)       38 2023-06-28 04:26:12.062075 ocr_iiif_tools-0.0.9/setup.cfg
+-rw-rw-r--   0 nakamura   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 ocr_iiif_tools-0.0.9/setup.py
```

### Comparing `ocr_iiif_tools-0.0.8/LICENSE` & `ocr_iiif_tools-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.8/PKG-INFO` & `ocr_iiif_tools-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocr_iiif_tools
-Version: 0.0.8
+Version: 0.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/nakamura196/ocr_iiif_tools
 Author: Satoru
 Author-email: you@example.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `ocr_iiif_tools-0.0.8/iida/_modidx.py` & `ocr_iiif_tools-0.0.9/iida/_modidx.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.8/iida/core.py` & `ocr_iiif_tools-0.0.9/iida/core.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.8/ocr_iiif/_modidx.py` & `ocr_iiif_tools-0.0.9/ocr_iiif/_modidx.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.8/ocr_iiif/core.py` & `ocr_iiif_tools-0.0.9/ocr_iiif/core.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.8/ocr_iiif_tools/_modidx.py` & `ocr_iiif_tools-0.0.9/ocr_iiif_tools/_modidx.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.8/ocr_iiif_tools/core.py` & `ocr_iiif_tools-0.0.9/ocr_iiif_tools/core.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.8/ocr_iiif_tools/pdf.py` & `ocr_iiif_tools-0.0.9/ocr_iiif_tools/pdf.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.8/ocr_iiif_tools.egg-info/PKG-INFO` & `ocr_iiif_tools-0.0.9/ocr_iiif_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocr-iiif-tools
-Version: 0.0.8
+Version: 0.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/nakamura196/ocr_iiif_tools
 Author: Satoru
 Author-email: you@example.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `ocr_iiif_tools-0.0.8/ocr_iiif_tools.egg-info/SOURCES.txt` & `ocr_iiif_tools-0.0.9/ocr_iiif_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.8/settings.ini` & `ocr_iiif_tools-0.0.9/settings.ini`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = ocr_iiif_tools
 lib_name = %(repo)s
-version = 0.0.8
+version = 0.0.9
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = ocr_iiif_tools
@@ -34,10 +34,10 @@
 description = 
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = nakamura196
 
 ### Optional ###
-requirements = reportlab requests tqdm
+requirements = reportlab==3.6.9 requests tqdm
 # dev_requirements = 
 # console_scripts =
```

### Comparing `ocr_iiif_tools-0.0.8/setup.py` & `ocr_iiif_tools-0.0.9/setup.py`

 * *Files identical despite different names*

