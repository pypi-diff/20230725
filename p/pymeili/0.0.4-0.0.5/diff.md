# Comparing `tmp/pymeili-0.0.4.tar.gz` & `tmp/pymeili-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymeili-0.0.4.tar", last modified: Tue Jul 25 14:37:08 2023, max compression
+gzip compressed data, was "pymeili-0.0.5.tar", last modified: Tue Jul 25 14:42:06 2023, max compression
```

## Comparing `pymeili-0.0.4.tar` & `pymeili-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 14:37:08.692530 pymeili-0.0.4/
--rw-rw-rw-   0        0        0      143 2023-07-25 14:36:40.000000 pymeili-0.0.4/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1057 2023-07-25 12:28:38.000000 pymeili-0.0.4/LISCENCE.txt
--rw-rw-rw-   0        0        0       31 2023-07-25 13:18:21.000000 pymeili-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      820 2023-07-25 14:37:08.692530 pymeili-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-07-25 13:25:52.000000 pymeili-0.0.4/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-25 14:37:08.681561 pymeili-0.0.4/pymeili/
-drwxrwxrwx   0        0        0        0 2023-07-25 14:37:08.691533 pymeili-0.0.4/pymeili/FONT/
--rw-rw-rw-   0        0        0    40028 2016-07-20 20:40:52.000000 pymeili-0.0.4/pymeili/FONT/Futura Extra Black font.ttf
--rw-rw-rw-   0        0        0    38980 2016-07-20 20:40:52.000000 pymeili-0.0.4/pymeili/FONT/Futura Heavy font.ttf
--rw-rw-rw-   0        0        0    38764 2016-07-20 20:40:54.000000 pymeili-0.0.4/pymeili/FONT/futura medium bt.ttf
--rw-rw-rw-   0        0        0      472 2023-07-25 14:36:50.000000 pymeili-0.0.4/pymeili/__init__.py
--rw-rw-rw-   0        0        0    20601 2023-07-25 14:17:36.000000 pymeili-0.0.4/pymeili/beautifyplot.py
-drwxrwxrwx   0        0        0        0 2023-07-25 14:37:08.689540 pymeili-0.0.4/pymeili.egg-info/
--rw-rw-rw-   0        0        0      820 2023-07-25 14:37:08.000000 pymeili-0.0.4/pymeili.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-07-25 14:37:08.000000 pymeili-0.0.4/pymeili.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 14:37:08.000000 pymeili-0.0.4/pymeili.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-25 14:37:08.000000 pymeili-0.0.4/pymeili.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 14:37:08.692530 pymeili-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      696 2023-07-25 14:36:36.000000 pymeili-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:42:06.117363 pymeili-0.0.5/
+-rw-rw-rw-   0        0        0      147 2023-07-25 14:41:58.000000 pymeili-0.0.5/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1057 2023-07-25 12:28:38.000000 pymeili-0.0.5/LISCENCE.txt
+-rw-rw-rw-   0        0        0       31 2023-07-25 13:18:21.000000 pymeili-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      824 2023-07-25 14:42:06.117363 pymeili-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-07-25 13:25:52.000000 pymeili-0.0.5/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 14:42:06.106393 pymeili-0.0.5/pymeili/
+drwxrwxrwx   0        0        0        0 2023-07-25 14:42:06.116366 pymeili-0.0.5/pymeili/FONT/
+-rw-rw-rw-   0        0        0    40028 2016-07-20 20:40:52.000000 pymeili-0.0.5/pymeili/FONT/Futura Extra Black font.ttf
+-rw-rw-rw-   0        0        0    38980 2016-07-20 20:40:52.000000 pymeili-0.0.5/pymeili/FONT/Futura Heavy font.ttf
+-rw-rw-rw-   0        0        0    38764 2016-07-20 20:40:54.000000 pymeili-0.0.5/pymeili/FONT/futura medium bt.ttf
+-rw-rw-rw-   0        0        0      480 2023-07-25 14:41:13.000000 pymeili-0.0.5/pymeili/__init__.py
+-rw-rw-rw-   0        0        0    20601 2023-07-25 14:17:36.000000 pymeili-0.0.5/pymeili/beautifyplot.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:42:06.113373 pymeili-0.0.5/pymeili.egg-info/
+-rw-rw-rw-   0        0        0      824 2023-07-25 14:42:06.000000 pymeili-0.0.5/pymeili.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-07-25 14:42:06.000000 pymeili-0.0.5/pymeili.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 14:42:06.000000 pymeili-0.0.5/pymeili.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-25 14:42:06.000000 pymeili-0.0.5/pymeili.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 14:42:06.117363 pymeili-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      696 2023-07-25 14:41:41.000000 pymeili-0.0.5/setup.py
```

### Comparing `pymeili-0.0.4/LISCENCE.txt` & `pymeili-0.0.5/LISCENCE.txt`

 * *Files identical despite different names*

### Comparing `pymeili-0.0.4/PKG-INFO` & `pymeili-0.0.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeili
-Version: 0.0.4
+Version: 0.0.5
 Summary: a module to beautify your python plot.
 Home-page: 
 Author: VVVictorZhou
 Author-email: vichouro@gmail.com
 License: MIT
 Keywords: beautify
 Classifier: Development Status :: 4 - Beta
@@ -26,9 +26,9 @@
 
 0.0.1 (26/07/2023)
 - First Release
 
 0.0.2 (26/07/2023)
 - Add Font Packages
 
-0.0.4 (26/07/2023)
-- Fix some bugs
+0.0.5 (26/07/2023)
+- Fix Some Problems
```

### Comparing `pymeili-0.0.4/pymeili/FONT/Futura Extra Black font.ttf` & `pymeili-0.0.5/pymeili/FONT/Futura Extra Black font.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.0.4/pymeili/FONT/Futura Heavy font.ttf` & `pymeili-0.0.5/pymeili/FONT/Futura Heavy font.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.0.4/pymeili/FONT/futura medium bt.ttf` & `pymeili-0.0.5/pymeili/FONT/futura medium bt.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.0.4/pymeili/beautifyplot.py` & `pymeili-0.0.5/pymeili/beautifyplot.py`

 * *Files identical despite different names*

### Comparing `pymeili-0.0.4/pymeili.egg-info/PKG-INFO` & `pymeili-0.0.5/pymeili.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeili
-Version: 0.0.4
+Version: 0.0.5
 Summary: a module to beautify your python plot.
 Home-page: 
 Author: VVVictorZhou
 Author-email: vichouro@gmail.com
 License: MIT
 Keywords: beautify
 Classifier: Development Status :: 4 - Beta
@@ -26,9 +26,9 @@
 
 0.0.1 (26/07/2023)
 - First Release
 
 0.0.2 (26/07/2023)
 - Add Font Packages
 
-0.0.4 (26/07/2023)
-- Fix some bugs
+0.0.5 (26/07/2023)
+- Fix Some Problems
```

### Comparing `pymeili-0.0.4/setup.py` & `pymeili-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='pymeili',
-    version='0.0.4',
+    version='0.0.5',
     description='a module to beautify your python plot.',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='VVVictorZhou',
     author_email='vichouro@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

