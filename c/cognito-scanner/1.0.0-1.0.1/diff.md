# Comparing `tmp/cognito-scanner-1.0.0.tar.gz` & `tmp/cognito-scanner-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognito-scanner-1.0.0.tar", last modified: Tue Jul 25 12:40:09 2023, max compression
+gzip compressed data, was "cognito-scanner-1.0.1.tar", last modified: Tue Jul 25 12:47:18 2023, max compression
```

## Comparing `cognito-scanner-1.0.0.tar` & `cognito-scanner-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 cfgs      (1000) cfgs      (1000)        0 2023-07-25 12:40:09.749407 cognito-scanner-1.0.0/
--rw-rw-r--   0 cfgs      (1000) cfgs      (1000)    11357 2023-07-21 09:33:49.000000 cognito-scanner-1.0.0/LICENSE
--rw-rw-r--   0 cfgs      (1000) cfgs      (1000)      304 2023-07-25 12:40:09.749407 cognito-scanner-1.0.0/PKG-INFO
--rw-rw-r--   0 cfgs      (1000) cfgs      (1000)     6382 2023-07-25 10:12:13.000000 cognito-scanner-1.0.0/README.md
-drwxrwxr-x   0 cfgs      (1000) cfgs      (1000)        0 2023-07-25 12:40:09.745407 cognito-scanner-1.0.0/cognito_scanner.egg-info/
--rw-rw-r--   0 cfgs      (1000) cfgs      (1000)      304 2023-07-25 12:40:09.000000 cognito-scanner-1.0.0/cognito_scanner.egg-info/PKG-INFO
--rw-rw-r--   0 cfgs      (1000) cfgs      (1000)      336 2023-07-25 12:40:09.000000 cognito-scanner-1.0.0/cognito_scanner.egg-info/SOURCES.txt
--rw-rw-r--   0 cfgs      (1000) cfgs      (1000)        1 2023-07-25 12:40:09.000000 cognito-scanner-1.0.0/cognito_scanner.egg-info/dependency_links.txt
--rw-rw-r--   0 cfgs      (1000) cfgs      (1000)       56 2023-07-25 12:40:09.000000 cognito-scanner-1.0.0/cognito_scanner.egg-info/entry_points.txt
--rw-rw-r--   0 cfgs      (1000) cfgs      (1000)       12 2023-07-25 12:40:09.000000 cognito-scanner-1.0.0/cognito_scanner.egg-info/requires.txt
--rw-rw-r--   0 cfgs      (1000) cfgs      (1000)        8 2023-07-25 12:40:09.000000 cognito-scanner-1.0.0/cognito_scanner.egg-info/top_level.txt
-drwxrwxr-x   0 cfgs      (1000) cfgs      (1000)        0 2023-07-25 12:40:09.749407 cognito-scanner-1.0.0/scanner/
--rw-rw-r--   0 cfgs      (1000) cfgs      (1000)    10815 2023-07-25 09:04:43.000000 cognito-scanner-1.0.0/scanner/AWSSRP.py
--rw-rw-r--   0 cfgs      (1000) cfgs      (1000)       67 2023-07-24 12:25:41.000000 cognito-scanner-1.0.0/scanner/__init__.py
--rwxrwxr-x   0 cfgs      (1000) cfgs      (1000)     6681 2023-07-25 09:04:33.000000 cognito-scanner-1.0.0/scanner/scanner.py
--rw-rw-r--   0 cfgs      (1000) cfgs      (1000)     1874 2023-07-21 09:34:01.000000 cognito-scanner-1.0.0/scanner/utils.py
--rw-rw-r--   0 cfgs      (1000) cfgs      (1000)       38 2023-07-25 12:40:09.749407 cognito-scanner-1.0.0/setup.cfg
--rw-rw-r--   0 cfgs      (1000) cfgs      (1000)      715 2023-07-25 12:38:26.000000 cognito-scanner-1.0.0/setup.py
+drwxrwxr-x   0 cfgs      (1000) cfgs      (1000)        0 2023-07-25 12:47:18.202698 cognito-scanner-1.0.1/
+-rw-rw-r--   0 cfgs      (1000) cfgs      (1000)    11357 2023-07-21 09:33:49.000000 cognito-scanner-1.0.1/LICENSE
+-rw-rw-r--   0 cfgs      (1000) cfgs      (1000)     6612 2023-07-25 12:47:18.202698 cognito-scanner-1.0.1/PKG-INFO
+-rw-rw-r--   0 cfgs      (1000) cfgs      (1000)     6382 2023-07-25 10:12:13.000000 cognito-scanner-1.0.1/README.md
+drwxrwxr-x   0 cfgs      (1000) cfgs      (1000)        0 2023-07-25 12:47:18.202698 cognito-scanner-1.0.1/cognito_scanner.egg-info/
+-rw-rw-r--   0 cfgs      (1000) cfgs      (1000)     6612 2023-07-25 12:47:18.000000 cognito-scanner-1.0.1/cognito_scanner.egg-info/PKG-INFO
+-rw-rw-r--   0 cfgs      (1000) cfgs      (1000)      336 2023-07-25 12:47:18.000000 cognito-scanner-1.0.1/cognito_scanner.egg-info/SOURCES.txt
+-rw-rw-r--   0 cfgs      (1000) cfgs      (1000)        1 2023-07-25 12:47:18.000000 cognito-scanner-1.0.1/cognito_scanner.egg-info/dependency_links.txt
+-rw-rw-r--   0 cfgs      (1000) cfgs      (1000)       56 2023-07-25 12:47:18.000000 cognito-scanner-1.0.1/cognito_scanner.egg-info/entry_points.txt
+-rw-rw-r--   0 cfgs      (1000) cfgs      (1000)       12 2023-07-25 12:47:18.000000 cognito-scanner-1.0.1/cognito_scanner.egg-info/requires.txt
+-rw-rw-r--   0 cfgs      (1000) cfgs      (1000)        8 2023-07-25 12:47:18.000000 cognito-scanner-1.0.1/cognito_scanner.egg-info/top_level.txt
+drwxrwxr-x   0 cfgs      (1000) cfgs      (1000)        0 2023-07-25 12:47:18.202698 cognito-scanner-1.0.1/scanner/
+-rw-rw-r--   0 cfgs      (1000) cfgs      (1000)    10815 2023-07-25 09:04:43.000000 cognito-scanner-1.0.1/scanner/AWSSRP.py
+-rw-rw-r--   0 cfgs      (1000) cfgs      (1000)       67 2023-07-24 12:25:41.000000 cognito-scanner-1.0.1/scanner/__init__.py
+-rwxrwxr-x   0 cfgs      (1000) cfgs      (1000)     6681 2023-07-25 09:04:33.000000 cognito-scanner-1.0.1/scanner/scanner.py
+-rw-rw-r--   0 cfgs      (1000) cfgs      (1000)     1874 2023-07-21 09:34:01.000000 cognito-scanner-1.0.1/scanner/utils.py
+-rw-rw-r--   0 cfgs      (1000) cfgs      (1000)       38 2023-07-25 12:47:18.202698 cognito-scanner-1.0.1/setup.cfg
+-rw-rw-r--   0 cfgs      (1000) cfgs      (1000)      782 2023-07-25 12:47:01.000000 cognito-scanner-1.0.1/setup.py
```

### Comparing `cognito-scanner-1.0.0/LICENSE` & `cognito-scanner-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cognito-scanner-1.0.0/README.md` & `cognito-scanner-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cognito-scanner-1.0.0/scanner/AWSSRP.py` & `cognito-scanner-1.0.1/scanner/AWSSRP.py`

 * *Files identical despite different names*

### Comparing `cognito-scanner-1.0.0/scanner/scanner.py` & `cognito-scanner-1.0.1/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `cognito-scanner-1.0.0/scanner/utils.py` & `cognito-scanner-1.0.1/scanner/utils.py`

 * *Files identical despite different names*

### Comparing `cognito-scanner-1.0.0/setup.py` & `cognito-scanner-1.0.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from setuptools import setup, find_packages
+from pathlib import Path
+
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='cognito-scanner',
-    version='1.0.0',
+    version='1.0.1',
     packages=find_packages(),
     install_requires=[
         "boto3", "typer"
     ],
     entry_points={
         'console_scripts': [
             'cognito-scanner = scanner.scanner:cli',
         ],
     },
     authors = [ { 'name': "Thibault Lengagne", 'email': 'thibaultl@padok.fr' }, { 'name':"Clement Fgs", 'email':'clementfa@padok.fr' }, ],
-    description="A simple script which implements different Cognito attacks such as Account Oracle or Priviledge Escalation",
-    readme="README.md",
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     author_email='thibaultl@padok.fr',
     url='https://github.com/padok-team/cognito-scanner',
     license='Apache2',
 )
```

