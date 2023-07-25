# Comparing `tmp/PARE_TOOLBOX-2023.2.tar.gz` & `tmp/PARE_TOOLBOX-2023.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PARE_TOOLBOX-2023.2.tar", last modified: Mon Jul 24 15:16:45 2023, max compression
+gzip compressed data, was "PARE_TOOLBOX-2023.3.tar", last modified: Tue Jul 25 12:03:20 2023, max compression
```

## Comparing `PARE_TOOLBOX-2023.2.tar` & `PARE_TOOLBOX-2023.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 15:16:45.029583 PARE_TOOLBOX-2023.2/
-drwxrwxrwx   0        0        0        0 2023-07-24 15:16:45.006582 PARE_TOOLBOX-2023.2/PARE_TOOLBOX/
--rw-rw-rw-   0        0        0     7905 2023-07-24 14:59:34.000000 PARE_TOOLBOX-2023.2/PARE_TOOLBOX/PARE.py
--rw-rw-rw-   0        0        0     2992 2023-07-24 14:47:10.000000 PARE_TOOLBOX-2023.2/PARE_TOOLBOX/ZIPPER.py
--rw-rw-rw-   0        0        0       42 2023-07-24 14:33:55.000000 PARE_TOOLBOX-2023.2/PARE_TOOLBOX/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 15:16:45.027583 PARE_TOOLBOX-2023.2/PARE_TOOLBOX.egg-info/
--rw-rw-rw-   0        0        0     1622 2023-07-24 15:16:44.000000 PARE_TOOLBOX-2023.2/PARE_TOOLBOX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-07-24 15:16:44.000000 PARE_TOOLBOX-2023.2/PARE_TOOLBOX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 15:16:44.000000 PARE_TOOLBOX-2023.2/PARE_TOOLBOX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-24 15:16:44.000000 PARE_TOOLBOX-2023.2/PARE_TOOLBOX.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-24 15:16:44.000000 PARE_TOOLBOX-2023.2/PARE_TOOLBOX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1622 2023-07-24 15:16:45.028583 PARE_TOOLBOX-2023.2/PKG-INFO
--rw-rw-rw-   0        0        0     1115 2023-07-15 23:52:16.000000 PARE_TOOLBOX-2023.2/license.md
--rw-rw-rw-   0        0        0       42 2023-07-24 15:16:45.030583 PARE_TOOLBOX-2023.2/setup.cfg
--rw-rw-rw-   0        0        0     1344 2023-07-24 15:16:36.000000 PARE_TOOLBOX-2023.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 12:03:20.786409 PARE_TOOLBOX-2023.3/
+drwxrwxrwx   0        0        0        0 2023-07-25 12:03:20.763404 PARE_TOOLBOX-2023.3/PARE_TOOLBOX/
+-rw-rw-rw-   0        0        0     7905 2023-07-25 12:00:06.000000 PARE_TOOLBOX-2023.3/PARE_TOOLBOX/PARE.py
+-rw-rw-rw-   0        0        0     2992 2023-07-25 12:00:06.000000 PARE_TOOLBOX-2023.3/PARE_TOOLBOX/ZIPPER.py
+-rw-rw-rw-   0        0        0       42 2023-07-25 12:00:06.000000 PARE_TOOLBOX-2023.3/PARE_TOOLBOX/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 12:03:20.784410 PARE_TOOLBOX-2023.3/PARE_TOOLBOX.egg-info/
+-rw-rw-rw-   0        0        0     1622 2023-07-25 12:03:20.000000 PARE_TOOLBOX-2023.3/PARE_TOOLBOX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-07-25 12:03:20.000000 PARE_TOOLBOX-2023.3/PARE_TOOLBOX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 12:03:20.000000 PARE_TOOLBOX-2023.3/PARE_TOOLBOX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-25 12:03:20.000000 PARE_TOOLBOX-2023.3/PARE_TOOLBOX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-25 12:03:20.000000 PARE_TOOLBOX-2023.3/PARE_TOOLBOX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1622 2023-07-25 12:03:20.786409 PARE_TOOLBOX-2023.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1115 2023-07-25 12:00:06.000000 PARE_TOOLBOX-2023.3/license.md
+-rw-rw-rw-   0        0        0       42 2023-07-25 12:03:20.787410 PARE_TOOLBOX-2023.3/setup.cfg
+-rw-rw-rw-   0        0        0     1344 2023-07-25 12:02:54.000000 PARE_TOOLBOX-2023.3/setup.py
```

### Comparing `PARE_TOOLBOX-2023.2/PARE_TOOLBOX/PARE.py` & `PARE_TOOLBOX-2023.3/PARE_TOOLBOX/PARE.py`

 * *Files identical despite different names*

### Comparing `PARE_TOOLBOX-2023.2/PARE_TOOLBOX/ZIPPER.py` & `PARE_TOOLBOX-2023.3/PARE_TOOLBOX/ZIPPER.py`

 * *Files identical despite different names*

### Comparing `PARE_TOOLBOX-2023.2/PARE_TOOLBOX.egg-info/PKG-INFO` & `PARE_TOOLBOX-2023.3/PARE_TOOLBOX.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PARE-TOOLBOX
-Version: 2023.2
+Version: 2023.3
 Summary: The PAREpy is an easy-to-use environment for applying probabilistic modeling.
 Home-page: https://wmpjrufg.github.io/PAREPY/
 Author: ['Wanderlei Malaquias Pereira Junior', 'Donizetti Aparecido de Souza Junior', 'Romes Antônio Borges', 'Mateus Pereira da Silva']
 Author-email: wanderlei_junior@ufcat.edu.br
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Education
```

### Comparing `PARE_TOOLBOX-2023.2/PKG-INFO` & `PARE_TOOLBOX-2023.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PARE_TOOLBOX
-Version: 2023.2
+Version: 2023.3
 Summary: The PAREpy is an easy-to-use environment for applying probabilistic modeling.
 Home-page: https://wmpjrufg.github.io/PAREPY/
 Author: ['Wanderlei Malaquias Pereira Junior', 'Donizetti Aparecido de Souza Junior', 'Romes Antônio Borges', 'Mateus Pereira da Silva']
 Author-email: wanderlei_junior@ufcat.edu.br
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Education
```

### Comparing `PARE_TOOLBOX-2023.2/license.md` & `PARE_TOOLBOX-2023.3/license.md`

 * *Files identical despite different names*

### Comparing `PARE_TOOLBOX-2023.2/setup.py` & `PARE_TOOLBOX-2023.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).resolve().parent
 readme_path = this_directory / "readme.md"
 long_description = readme_path.read_text(encoding = 'utf-8')
 
 setup(
     	name = 'PARE_TOOLBOX',
-    	version = '2023.2',
+    	version = '2023.3',
 		url = 'https://wmpjrufg.github.io/PAREPY/',
         description = 'The PAREpy is an easy-to-use environment for applying probabilistic modeling.',
 		long_description = long_description,
 		long_description_content_type='text/markdown',   
     	license = 'MIT License',
         author = ['Wanderlei Malaquias Pereira Junior', 
                   'Donizetti Aparecido de Souza Junior',
```

