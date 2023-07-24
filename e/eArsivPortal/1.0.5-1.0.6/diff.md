# Comparing `tmp/eArsivPortal-1.0.5.tar.gz` & `tmp/eArsivPortal-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eArsivPortal-1.0.5.tar", last modified: Mon Jul 24 22:31:03 2023, max compression
+gzip compressed data, was "eArsivPortal-1.0.6.tar", last modified: Mon Jul 24 22:32:40 2023, max compression
```

## Comparing `eArsivPortal-1.0.5.tar` & `eArsivPortal-1.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2023-07-24 22:31:03.966393 eArsivPortal-1.0.5/
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)    35149 2023-07-24 14:16:46.000000 eArsivPortal-1.0.5/LICENSE
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)       32 2023-07-24 14:16:46.000000 eArsivPortal-1.0.5/MANIFEST.in
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     6907 2023-07-24 22:31:03.966393 eArsivPortal-1.0.5/PKG-INFO
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     6338 2023-07-24 14:16:46.000000 eArsivPortal-1.0.5/README.md
-drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2023-07-24 22:31:03.963060 eArsivPortal-1.0.5/eArsivPortal/
-drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2023-07-24 22:31:03.963060 eArsivPortal-1.0.5/eArsivPortal/Core/
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      212 2023-07-24 14:16:46.000000 eArsivPortal-1.0.5/eArsivPortal/Core/Hatalar.py
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     9672 2023-07-24 14:16:46.000000 eArsivPortal-1.0.5/eArsivPortal/Core/__init__.py
-drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2023-07-24 22:31:03.963060 eArsivPortal-1.0.5/eArsivPortal/Libs/
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     3568 2023-07-24 14:21:18.000000 eArsivPortal-1.0.5/eArsivPortal/Libs/FaturaVer.py
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      785 2023-07-24 14:16:46.000000 eArsivPortal-1.0.5/eArsivPortal/Libs/Oturum.py
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      188 2023-07-24 14:16:46.000000 eArsivPortal-1.0.5/eArsivPortal/Libs/__init__.py
-drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2023-07-24 22:31:03.963060 eArsivPortal-1.0.5/eArsivPortal/Models/
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     1510 2023-07-24 14:16:46.000000 eArsivPortal-1.0.5/eArsivPortal/Models/Komutlar.py
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      115 2023-07-24 14:16:46.000000 eArsivPortal-1.0.5/eArsivPortal/Models/__init__.py
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      108 2023-07-24 14:16:46.000000 eArsivPortal-1.0.5/eArsivPortal/__init__.py
-drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2023-07-24 22:31:03.963060 eArsivPortal-1.0.5/eArsivPortal.egg-info/
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     6907 2023-07-24 22:31:03.000000 eArsivPortal-1.0.5/eArsivPortal.egg-info/PKG-INFO
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      454 2023-07-24 22:31:03.000000 eArsivPortal-1.0.5/eArsivPortal.egg-info/SOURCES.txt
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        1 2023-07-24 22:31:03.000000 eArsivPortal-1.0.5/eArsivPortal.egg-info/dependency_links.txt
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)       60 2023-07-24 22:31:03.000000 eArsivPortal-1.0.5/eArsivPortal.egg-info/requires.txt
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)       13 2023-07-24 22:31:03.000000 eArsivPortal-1.0.5/eArsivPortal.egg-info/top_level.txt
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)       38 2023-07-24 22:31:03.966393 eArsivPortal-1.0.5/setup.cfg
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     1239 2023-07-24 22:26:24.000000 eArsivPortal-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:32:40.040294 eArsivPortal-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-24 22:32:09.000000 eArsivPortal-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-24 22:32:09.000000 eArsivPortal-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-07-24 22:32:40.040294 eArsivPortal-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-07-24 22:32:09.000000 eArsivPortal-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:32:40.036294 eArsivPortal-1.0.6/eArsivPortal/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:32:40.040294 eArsivPortal-1.0.6/eArsivPortal/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-24 22:32:09.000000 eArsivPortal-1.0.6/eArsivPortal/Core/Hatalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-07-24 22:32:09.000000 eArsivPortal-1.0.6/eArsivPortal/Core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:32:40.040294 eArsivPortal-1.0.6/eArsivPortal/Libs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-07-24 22:32:09.000000 eArsivPortal-1.0.6/eArsivPortal/Libs/FaturaVer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-24 22:32:09.000000 eArsivPortal-1.0.6/eArsivPortal/Libs/Oturum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-24 22:32:09.000000 eArsivPortal-1.0.6/eArsivPortal/Libs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:32:40.040294 eArsivPortal-1.0.6/eArsivPortal/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-24 22:32:09.000000 eArsivPortal-1.0.6/eArsivPortal/Models/Komutlar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-24 22:32:09.000000 eArsivPortal-1.0.6/eArsivPortal/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-24 22:32:09.000000 eArsivPortal-1.0.6/eArsivPortal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:32:40.036294 eArsivPortal-1.0.6/eArsivPortal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-07-24 22:32:40.000000 eArsivPortal-1.0.6/eArsivPortal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-24 22:32:40.000000 eArsivPortal-1.0.6/eArsivPortal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 22:32:40.000000 eArsivPortal-1.0.6/eArsivPortal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-24 22:32:40.000000 eArsivPortal-1.0.6/eArsivPortal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-24 22:32:40.000000 eArsivPortal-1.0.6/eArsivPortal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 22:32:40.040294 eArsivPortal-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-24 22:32:09.000000 eArsivPortal-1.0.6/setup.py
```

### Comparing `eArsivPortal-1.0.5/LICENSE` & `eArsivPortal-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `eArsivPortal-1.0.5/PKG-INFO` & `eArsivPortal-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eArsivPortal
-Version: 1.0.5
+Version: 1.0.6
 Summary: GİB e-Arşiv Portal e-Fatura Oluşturucu
 Home-page: https://github.com/keyiflerolsun/eArsivPortal
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: eArsivPortal,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eArsivPortal Version: 1.0.5 Summary: GÄ°B e-ArÅiv
+Metadata-Version: 2.1 Name: eArsivPortal Version: 1.0.6 Summary: GÄ°B e-ArÅiv
 Portal e-Fatura OluÅturucu Home-page: https://github.com/keyiflerolsun/
 eArsivPortal Author: keyiflerolsun Author-email: keyiflerolsun@gmail.com
 License: GPLv3+ Keywords: eArsivPortal,KekikAkademi,keyiflerolsun Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: GNU General Public License v3 or later (GPLv3+) Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.10 Description-Content-Type: text/
 markdown License-File: LICENSE # ð§¾ eArsivPortal [![Boyut](https://
```

### Comparing `eArsivPortal-1.0.5/README.md` & `eArsivPortal-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `eArsivPortal-1.0.5/eArsivPortal/Core/__init__.py` & `eArsivPortal-1.0.6/eArsivPortal/Core/__init__.py`

 * *Files identical despite different names*

### Comparing `eArsivPortal-1.0.5/eArsivPortal/Libs/FaturaVer.py` & `eArsivPortal-1.0.6/eArsivPortal/Libs/FaturaVer.py`

 * *Files identical despite different names*

### Comparing `eArsivPortal-1.0.5/eArsivPortal/Libs/Oturum.py` & `eArsivPortal-1.0.6/eArsivPortal/Libs/Oturum.py`

 * *Files identical despite different names*

### Comparing `eArsivPortal-1.0.5/eArsivPortal/Models/Komutlar.py` & `eArsivPortal-1.0.6/eArsivPortal/Models/Komutlar.py`

 * *Files identical despite different names*

### Comparing `eArsivPortal-1.0.5/eArsivPortal.egg-info/PKG-INFO` & `eArsivPortal-1.0.6/eArsivPortal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eArsivPortal
-Version: 1.0.5
+Version: 1.0.6
 Summary: GİB e-Arşiv Portal e-Fatura Oluşturucu
 Home-page: https://github.com/keyiflerolsun/eArsivPortal
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: eArsivPortal,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eArsivPortal Version: 1.0.5 Summary: GÄ°B e-ArÅiv
+Metadata-Version: 2.1 Name: eArsivPortal Version: 1.0.6 Summary: GÄ°B e-ArÅiv
 Portal e-Fatura OluÅturucu Home-page: https://github.com/keyiflerolsun/
 eArsivPortal Author: keyiflerolsun Author-email: keyiflerolsun@gmail.com
 License: GPLv3+ Keywords: eArsivPortal,KekikAkademi,keyiflerolsun Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: GNU General Public License v3 or later (GPLv3+) Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.10 Description-Content-Type: text/
 markdown License-File: LICENSE # ð§¾ eArsivPortal [![Boyut](https://
```

### Comparing `eArsivPortal-1.0.5/setup.py` & `eArsivPortal-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "eArsivPortal",
-    version      = "1.0.5",
+    version      = "1.0.6",
     url          = "https://github.com/keyiflerolsun/eArsivPortal",
     description  = "GİB e-Arşiv Portal e-Fatura Oluşturucu",
     keywords     = ["eArsivPortal", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
```

