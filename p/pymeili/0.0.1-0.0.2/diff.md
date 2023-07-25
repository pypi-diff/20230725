# Comparing `tmp/pymeili-0.0.1.tar.gz` & `tmp/pymeili-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymeili-0.0.1.tar", last modified: Tue Jul 25 13:14:53 2023, max compression
+gzip compressed data, was "pymeili-0.0.2.tar", last modified: Tue Jul 25 13:19:47 2023, max compression
```

## Comparing `pymeili-0.0.1.tar` & `pymeili-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 13:14:53.386264 pymeili-0.0.1/
--rw-rw-rw-   0        0        0       61 2023-07-25 12:40:41.000000 pymeili-0.0.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1057 2023-07-25 12:28:38.000000 pymeili-0.0.1/LISCENCE.txt
--rw-rw-rw-   0        0        0       25 2023-07-25 12:23:29.000000 pymeili-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      583 2023-07-25 13:14:53.386264 pymeili-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       70 2023-07-25 13:14:45.000000 pymeili-0.0.1/README.txt
--rw-rw-rw-   0        0        0       14 2023-07-25 12:51:05.000000 pymeili-0.0.1/__init__.py
--rw-rw-rw-   0        0        0    20451 2023-07-25 12:21:39.000000 pymeili-0.0.1/beautifyplot.py
-drwxrwxrwx   0        0        0        0 2023-07-25 13:14:53.385266 pymeili-0.0.1/pymeili.egg-info/
--rw-rw-rw-   0        0        0      583 2023-07-25 13:14:53.000000 pymeili-0.0.1/pymeili.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-07-25 13:14:53.000000 pymeili-0.0.1/pymeili.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 13:14:53.000000 pymeili-0.0.1/pymeili.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 13:14:53.000000 pymeili-0.0.1/pymeili.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 13:14:53.386264 pymeili-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      696 2023-07-25 12:44:22.000000 pymeili-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 13:19:47.316105 pymeili-0.0.2/
+-rw-rw-rw-   0        0        0      104 2023-07-25 13:19:14.000000 pymeili-0.0.2/CHANGELOG.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 13:19:47.303141 pymeili-0.0.2/FONT/
+-rw-rw-rw-   0        0        0    40028 2016-07-20 20:40:52.000000 pymeili-0.0.2/FONT/Futura Extra Black font.ttf
+-rw-rw-rw-   0        0        0    38980 2016-07-20 20:40:52.000000 pymeili-0.0.2/FONT/Futura Heavy font.ttf
+-rw-rw-rw-   0        0        0    38764 2016-07-20 20:40:54.000000 pymeili-0.0.2/FONT/futura medium bt.ttf
+-rw-rw-rw-   0        0        0     1057 2023-07-25 12:28:38.000000 pymeili-0.0.2/LISCENCE.txt
+-rw-rw-rw-   0        0        0       31 2023-07-25 13:18:21.000000 pymeili-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      626 2023-07-25 13:19:47.315109 pymeili-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       70 2023-07-25 13:14:45.000000 pymeili-0.0.2/README.txt
+-rw-rw-rw-   0        0        0       14 2023-07-25 12:51:05.000000 pymeili-0.0.2/__init__.py
+-rw-rw-rw-   0        0        0    20451 2023-07-25 12:21:39.000000 pymeili-0.0.2/beautifyplot.py
+drwxrwxrwx   0        0        0        0 2023-07-25 13:19:47.314111 pymeili-0.0.2/pymeili.egg-info/
+-rw-rw-rw-   0        0        0      626 2023-07-25 13:19:47.000000 pymeili-0.0.2/pymeili.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-07-25 13:19:47.000000 pymeili-0.0.2/pymeili.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 13:19:47.000000 pymeili-0.0.2/pymeili.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 13:19:47.000000 pymeili-0.0.2/pymeili.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 13:19:47.316105 pymeili-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      696 2023-07-25 13:18:46.000000 pymeili-0.0.2/setup.py
```

### Comparing `pymeili-0.0.1/LISCENCE.txt` & `pymeili-0.0.2/LISCENCE.txt`

 * *Files identical despite different names*

### Comparing `pymeili-0.0.1/PKG-INFO` & `pymeili-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeili
-Version: 0.0.1
+Version: 0.0.2
 Summary: a module to beautify your python plot.
 Home-page: 
 Author: VVVictorZhou
 Author-email: vichouro@gmail.com
 License: MIT
 Keywords: beautify
 Classifier: Development Status :: 4 - Beta
@@ -16,7 +16,10 @@
 pymeili is a module to beautify your python plot with more simple way.
 
 Change Log
 ==========
 
 0.0.1 (26/07/2023)
 - First Release
+
+0.0.2 (26/07/2023)
+- Add Font Packages
```

### Comparing `pymeili-0.0.1/beautifyplot.py` & `pymeili-0.0.2/beautifyplot.py`

 * *Files identical despite different names*

### Comparing `pymeili-0.0.1/pymeili.egg-info/PKG-INFO` & `pymeili-0.0.2/pymeili.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeili
-Version: 0.0.1
+Version: 0.0.2
 Summary: a module to beautify your python plot.
 Home-page: 
 Author: VVVictorZhou
 Author-email: vichouro@gmail.com
 License: MIT
 Keywords: beautify
 Classifier: Development Status :: 4 - Beta
@@ -16,7 +16,10 @@
 pymeili is a module to beautify your python plot with more simple way.
 
 Change Log
 ==========
 
 0.0.1 (26/07/2023)
 - First Release
+
+0.0.2 (26/07/2023)
+- Add Font Packages
```

### Comparing `pymeili-0.0.1/setup.py` & `pymeili-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='pymeili',
-    version='0.0.1',
+    version='0.0.2',
     description='a module to beautify your python plot.',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='VVVictorZhou',
     author_email='vichouro@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

