# Comparing `tmp/PARE_TOOLBOX-2023.5.tar.gz` & `tmp/PARE_TOOLBOX-2023.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PARE_TOOLBOX-2023.5.tar", last modified: Tue Jul 25 12:24:21 2023, max compression
+gzip compressed data, was "PARE_TOOLBOX-2023.6.tar", last modified: Tue Jul 25 12:28:23 2023, max compression
```

## Comparing `PARE_TOOLBOX-2023.5.tar` & `PARE_TOOLBOX-2023.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 12:24:21.362962 PARE_TOOLBOX-2023.5/
-drwxrwxrwx   0        0        0        0 2023-07-25 12:24:21.344411 PARE_TOOLBOX-2023.5/PARE_TOOLBOX/
--rw-rw-rw-   0        0        0     7905 2023-07-25 12:00:06.000000 PARE_TOOLBOX-2023.5/PARE_TOOLBOX/PARE.py
--rw-rw-rw-   0        0        0     2992 2023-07-25 12:00:06.000000 PARE_TOOLBOX-2023.5/PARE_TOOLBOX/ZIPPER.py
--rw-rw-rw-   0        0        0       42 2023-07-25 12:00:06.000000 PARE_TOOLBOX-2023.5/PARE_TOOLBOX/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 12:24:21.360961 PARE_TOOLBOX-2023.5/PARE_TOOLBOX.egg-info/
--rw-rw-rw-   0        0        0     1622 2023-07-25 12:24:21.000000 PARE_TOOLBOX-2023.5/PARE_TOOLBOX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-07-25 12:24:21.000000 PARE_TOOLBOX-2023.5/PARE_TOOLBOX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 12:24:21.000000 PARE_TOOLBOX-2023.5/PARE_TOOLBOX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-25 12:24:21.000000 PARE_TOOLBOX-2023.5/PARE_TOOLBOX.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-25 12:24:21.000000 PARE_TOOLBOX-2023.5/PARE_TOOLBOX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1622 2023-07-25 12:24:21.361961 PARE_TOOLBOX-2023.5/PKG-INFO
--rw-rw-rw-   0        0        0     1115 2023-07-25 12:00:06.000000 PARE_TOOLBOX-2023.5/license.md
--rw-rw-rw-   0        0        0       42 2023-07-25 12:24:21.362962 PARE_TOOLBOX-2023.5/setup.cfg
--rw-rw-rw-   0        0        0     1344 2023-07-25 12:24:07.000000 PARE_TOOLBOX-2023.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 12:28:23.518617 PARE_TOOLBOX-2023.6/
+drwxrwxrwx   0        0        0        0 2023-07-25 12:28:23.501866 PARE_TOOLBOX-2023.6/PARE_TOOLBOX/
+-rw-rw-rw-   0        0        0     7905 2023-07-25 12:00:06.000000 PARE_TOOLBOX-2023.6/PARE_TOOLBOX/PARE.py
+-rw-rw-rw-   0        0        0     2992 2023-07-25 12:00:06.000000 PARE_TOOLBOX-2023.6/PARE_TOOLBOX/ZIPPER.py
+-rw-rw-rw-   0        0        0       42 2023-07-25 12:00:06.000000 PARE_TOOLBOX-2023.6/PARE_TOOLBOX/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 12:28:23.517617 PARE_TOOLBOX-2023.6/PARE_TOOLBOX.egg-info/
+-rw-rw-rw-   0        0        0      644 2023-07-25 12:28:23.000000 PARE_TOOLBOX-2023.6/PARE_TOOLBOX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-07-25 12:28:23.000000 PARE_TOOLBOX-2023.6/PARE_TOOLBOX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 12:28:23.000000 PARE_TOOLBOX-2023.6/PARE_TOOLBOX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-25 12:28:23.000000 PARE_TOOLBOX-2023.6/PARE_TOOLBOX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-25 12:28:23.000000 PARE_TOOLBOX-2023.6/PARE_TOOLBOX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      644 2023-07-25 12:28:23.518617 PARE_TOOLBOX-2023.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1115 2023-07-25 12:00:06.000000 PARE_TOOLBOX-2023.6/license.md
+-rw-rw-rw-   0        0        0       42 2023-07-25 12:28:23.518617 PARE_TOOLBOX-2023.6/setup.cfg
+-rw-rw-rw-   0        0        0     1356 2023-07-25 12:28:07.000000 PARE_TOOLBOX-2023.6/setup.py
```

### Comparing `PARE_TOOLBOX-2023.5/PARE_TOOLBOX/PARE.py` & `PARE_TOOLBOX-2023.6/PARE_TOOLBOX/PARE.py`

 * *Files identical despite different names*

### Comparing `PARE_TOOLBOX-2023.5/PARE_TOOLBOX/ZIPPER.py` & `PARE_TOOLBOX-2023.6/PARE_TOOLBOX/ZIPPER.py`

 * *Files identical despite different names*

### Comparing `PARE_TOOLBOX-2023.5/license.md` & `PARE_TOOLBOX-2023.6/license.md`

 * *Files identical despite different names*

### Comparing `PARE_TOOLBOX-2023.5/setup.py` & `PARE_TOOLBOX-2023.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
-from pathlib import Path
-this_directory = Path(__file__).resolve().parent
-readme_path = this_directory / "readme.md"
-long_description = readme_path.read_text(encoding = 'utf-8')
+# from pathlib import Path
+# this_directory = Path(__file__).resolve().parent
+# readme_path = this_directory / "readme.md"
+# long_description = readme_path.read_text(encoding = 'utf-8')
 
 setup(
     	name = 'PARE_TOOLBOX',
-    	version = '2023.5',
+    	version = '2023.6',
 		url = 'https://wmpjrufg.github.io/PAREPY/',
         description = 'The PAREpy is an easy-to-use environment for applying probabilistic modeling.',
-		long_description = long_description,
-		long_description_content_type='text/markdown',   
+		# long_description = long_description,
+		# long_description_content_type='text/markdown',   
     	license = 'MIT License',
         author = ['Wanderlei Malaquias Pereira Junior', 
                   'Donizetti Aparecido de Souza Junior', 
                   'Romes Antônio Borges',
                   'Mateus Pereira da Silva'],
     	author_email = 'wanderlei_junior@ufcat.edu.br',
         install_requires = ["numpy", "scipy", "pandas"],
```

