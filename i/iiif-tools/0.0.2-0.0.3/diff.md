# Comparing `tmp/iiif_tools-0.0.2.tar.gz` & `tmp/iiif_tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iiif_tools-0.0.2.tar", last modified: Wed May 24 22:54:20 2023, max compression
+gzip compressed data, was "iiif_tools-0.0.3.tar", last modified: Tue Jul 25 05:45:06 2023, max compression
```

## Comparing `iiif_tools-0.0.2.tar` & `iiif_tools-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-05-24 22:54:20.017697 iiif_tools-0.0.2/
--rw-rw-r--   0 nakamura   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 iiif_tools-0.0.2/LICENSE
--rw-rw-r--   0 nakamura   (501) staff       (20)      111 2023-04-27 10:12:58.000000 iiif_tools-0.0.2/MANIFEST.in
--rw-r--r--   0 nakamura   (501) staff       (20)     1068 2023-05-24 22:54:20.017479 iiif_tools-0.0.2/PKG-INFO
--rw-r--r--   0 nakamura   (501) staff       (20)      305 2023-05-24 22:15:17.000000 iiif_tools-0.0.2/README.md
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-05-24 22:54:20.015698 iiif_tools-0.0.2/iiif_tools/
--rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-05-24 22:52:19.000000 iiif_tools-0.0.2/iiif_tools/__init__.py
--rw-r--r--   0 nakamura   (501) staff       (20)     2132 2023-05-24 22:52:19.000000 iiif_tools-0.0.2/iiif_tools/_modidx.py
--rw-r--r--   0 nakamura   (501) staff       (20)      142 2023-05-24 22:52:19.000000 iiif_tools-0.0.2/iiif_tools/core.py
--rw-r--r--   0 nakamura   (501) staff       (20)     6352 2023-05-24 22:52:19.000000 iiif_tools-0.0.2/iiif_tools/pdf.py
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-05-24 22:54:20.016992 iiif_tools-0.0.2/iiif_tools.egg-info/
--rw-r--r--   0 nakamura   (501) staff       (20)     1068 2023-05-24 22:54:20.000000 iiif_tools-0.0.2/iiif_tools.egg-info/PKG-INFO
--rw-r--r--   0 nakamura   (501) staff       (20)      372 2023-05-24 22:54:20.000000 iiif_tools-0.0.2/iiif_tools.egg-info/SOURCES.txt
--rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-05-24 22:54:20.000000 iiif_tools-0.0.2/iiif_tools.egg-info/dependency_links.txt
--rw-r--r--   0 nakamura   (501) staff       (20)       63 2023-05-24 22:54:20.000000 iiif_tools-0.0.2/iiif_tools.egg-info/entry_points.txt
--rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-05-24 22:15:50.000000 iiif_tools-0.0.2/iiif_tools.egg-info/not-zip-safe
--rw-r--r--   0 nakamura   (501) staff       (20)       29 2023-05-24 22:54:20.000000 iiif_tools-0.0.2/iiif_tools.egg-info/requires.txt
--rw-r--r--   0 nakamura   (501) staff       (20)       11 2023-05-24 22:54:20.000000 iiif_tools-0.0.2/iiif_tools.egg-info/top_level.txt
--rw-r--r--   0 nakamura   (501) staff       (20)      921 2023-05-24 22:54:09.000000 iiif_tools-0.0.2/settings.ini
--rw-r--r--   0 nakamura   (501) staff       (20)       38 2023-05-24 22:54:20.017817 iiif_tools-0.0.2/setup.cfg
--rw-rw-r--   0 nakamura   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 iiif_tools-0.0.2/setup.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-07-25 05:45:06.307325 iiif_tools-0.0.3/
+-rw-r--r--   0 nakamura   (501) staff       (20)    11337 2023-07-25 05:26:46.000000 iiif_tools-0.0.3/LICENSE
+-rw-r--r--   0 nakamura   (501) staff       (20)      111 2023-07-25 05:26:46.000000 iiif_tools-0.0.3/MANIFEST.in
+-rw-r--r--   0 nakamura   (501) staff       (20)     1068 2023-07-25 05:45:06.307093 iiif_tools-0.0.3/PKG-INFO
+-rw-r--r--   0 nakamura   (501) staff       (20)      305 2023-07-25 05:45:01.000000 iiif_tools-0.0.3/README.md
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-07-25 05:45:06.305381 iiif_tools-0.0.3/iiif_tools/
+-rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-07-25 05:44:55.000000 iiif_tools-0.0.3/iiif_tools/__init__.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     1756 2023-07-25 05:44:55.000000 iiif_tools-0.0.3/iiif_tools/_modidx.py
+-rw-r--r--   0 nakamura   (501) staff       (20)      142 2023-07-25 05:44:55.000000 iiif_tools-0.0.3/iiif_tools/core.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     4060 2023-07-25 05:44:55.000000 iiif_tools-0.0.3/iiif_tools/pdf.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-07-25 05:45:06.306826 iiif_tools-0.0.3/iiif_tools.egg-info/
+-rw-r--r--   0 nakamura   (501) staff       (20)     1068 2023-07-25 05:45:06.000000 iiif_tools-0.0.3/iiif_tools.egg-info/PKG-INFO
+-rw-r--r--   0 nakamura   (501) staff       (20)      372 2023-07-25 05:45:06.000000 iiif_tools-0.0.3/iiif_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-07-25 05:45:06.000000 iiif_tools-0.0.3/iiif_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)       63 2023-07-25 05:45:06.000000 iiif_tools-0.0.3/iiif_tools.egg-info/entry_points.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-07-25 05:33:42.000000 iiif_tools-0.0.3/iiif_tools.egg-info/not-zip-safe
+-rw-r--r--   0 nakamura   (501) staff       (20)       29 2023-07-25 05:45:06.000000 iiif_tools-0.0.3/iiif_tools.egg-info/requires.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)       11 2023-07-25 05:45:06.000000 iiif_tools-0.0.3/iiif_tools.egg-info/top_level.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)      921 2023-07-25 05:44:36.000000 iiif_tools-0.0.3/settings.ini
+-rw-r--r--   0 nakamura   (501) staff       (20)       38 2023-07-25 05:45:06.307385 iiif_tools-0.0.3/setup.cfg
+-rw-r--r--   0 nakamura   (501) staff       (20)     2596 2023-07-25 05:26:46.000000 iiif_tools-0.0.3/setup.py
```

### Comparing `iiif_tools-0.0.2/LICENSE` & `iiif_tools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `iiif_tools-0.0.2/PKG-INFO` & `iiif_tools-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iiif_tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: UNKNOWN
 Home-page: https://github.com/nakamura196/iiif_tools
 Author: Satoru
 Author-email: you@example.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `iiif_tools-0.0.2/iiif_tools/_modidx.py` & `iiif_tools-0.0.3/iiif_tools/_modidx.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,19 +4,16 @@
                 'doc_baseurl': '/iiif_tools',
                 'doc_host': 'https://nakamura196.github.io',
                 'git_url': 'https://github.com/nakamura196/iiif_tools',
                 'lib_path': 'iiif_tools'},
   'syms': { 'iiif_tools.core': {'iiif_tools.core.foo': ('core.html#foo', 'iiif_tools/core.py')},
             'iiif_tools.pdf': { 'iiif_tools.pdf.PdfClient': ('pdf.html#pdfclient', 'iiif_tools/pdf.py'),
                                 'iiif_tools.pdf.PdfClient.__init__': ('pdf.html#pdfclient.__init__', 'iiif_tools/pdf.py'),
-                                'iiif_tools.pdf.PdfClient.create_manifest': ('pdf.html#pdfclient.create_manifest', 'iiif_tools/pdf.py'),
                                 'iiif_tools.pdf.PdfClient.create_pdf': ('pdf.html#pdfclient.create_pdf', 'iiif_tools/pdf.py'),
                                 'iiif_tools.pdf.PdfClient.create_pdf_from_dir': ( 'pdf.html#pdfclient.create_pdf_from_dir',
                                                                                   'iiif_tools/pdf.py'),
                                 'iiif_tools.pdf.PdfClient.create_pdf_from_manifest_local': ( 'pdf.html#pdfclient.create_pdf_from_manifest_local',
                                                                                              'iiif_tools/pdf.py'),
                                 'iiif_tools.pdf.PdfClient.create_pdf_from_manifest_url': ( 'pdf.html#pdfclient.create_pdf_from_manifest_url',
                                                                                            'iiif_tools/pdf.py'),
                                 'iiif_tools.pdf.PdfClient.download_image': ('pdf.html#pdfclient.download_image', 'iiif_tools/pdf.py'),
-                                'iiif_tools.pdf.PdfClient.download_images': ('pdf.html#pdfclient.download_images', 'iiif_tools/pdf.py'),
-                                'iiif_tools.pdf.PdfClient.get_infos': ('pdf.html#pdfclient.get_infos', 'iiif_tools/pdf.py'),
-                                'iiif_tools.pdf.PdfClient.save': ('pdf.html#pdfclient.save', 'iiif_tools/pdf.py')}}}
+                                'iiif_tools.pdf.PdfClient.download_images': ('pdf.html#pdfclient.download_images', 'iiif_tools/pdf.py')}}}
```

### Comparing `iiif_tools-0.0.2/iiif_tools.egg-info/PKG-INFO` & `iiif_tools-0.0.3/iiif_tools.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iiif-tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: UNKNOWN
 Home-page: https://github.com/nakamura196/iiif_tools
 Author: Satoru
 Author-email: you@example.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `iiif_tools-0.0.2/settings.ini` & `iiif_tools-0.0.3/settings.ini`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = iiif_tools
 lib_name = %(repo)s
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = iiif_tools
```

### Comparing `iiif_tools-0.0.2/setup.py` & `iiif_tools-0.0.3/setup.py`

 * *Files identical despite different names*

