# Comparing `tmp/pymeili-0.0.3.tar.gz` & `tmp/pymeili-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymeili-0.0.3.tar", last modified: Tue Jul 25 14:19:34 2023, max compression
+gzip compressed data, was "pymeili-0.0.4.tar", last modified: Tue Jul 25 14:37:08 2023, max compression
```

## Comparing `pymeili-0.0.3.tar` & `pymeili-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 14:19:34.156918 pymeili-0.0.3/
--rw-rw-rw-   0        0        0      142 2023-07-25 14:16:45.000000 pymeili-0.0.3/CHANGELOG.txt
-drwxrwxrwx   0        0        0        0 2023-07-25 14:19:34.140966 pymeili-0.0.3/FONT/
--rw-rw-rw-   0        0        0    40028 2016-07-20 20:40:52.000000 pymeili-0.0.3/FONT/Futura Extra Black font.ttf
--rw-rw-rw-   0        0        0    38980 2016-07-20 20:40:52.000000 pymeili-0.0.3/FONT/Futura Heavy font.ttf
--rw-rw-rw-   0        0        0    38764 2016-07-20 20:40:54.000000 pymeili-0.0.3/FONT/futura medium bt.ttf
--rw-rw-rw-   0        0        0     1057 2023-07-25 12:28:38.000000 pymeili-0.0.3/LISCENCE.txt
--rw-rw-rw-   0        0        0       31 2023-07-25 13:18:21.000000 pymeili-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      819 2023-07-25 14:19:34.155926 pymeili-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-07-25 13:25:52.000000 pymeili-0.0.3/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-25 14:19:34.141957 pymeili-0.0.3/pymeili/
--rw-rw-rw-   0        0        0      472 2023-07-25 14:18:09.000000 pymeili-0.0.3/pymeili/__init__.py
--rw-rw-rw-   0        0        0    20601 2023-07-25 14:17:36.000000 pymeili-0.0.3/pymeili/beautifyplot.py
-drwxrwxrwx   0        0        0        0 2023-07-25 14:19:34.155926 pymeili-0.0.3/pymeili.egg-info/
--rw-rw-rw-   0        0        0      819 2023-07-25 14:19:34.000000 pymeili-0.0.3/pymeili.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-25 14:19:34.000000 pymeili-0.0.3/pymeili.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 14:19:34.000000 pymeili-0.0.3/pymeili.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-25 14:19:34.000000 pymeili-0.0.3/pymeili.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 14:19:34.156918 pymeili-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      696 2023-07-25 14:17:00.000000 pymeili-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:37:08.692530 pymeili-0.0.4/
+-rw-rw-rw-   0        0        0      143 2023-07-25 14:36:40.000000 pymeili-0.0.4/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1057 2023-07-25 12:28:38.000000 pymeili-0.0.4/LISCENCE.txt
+-rw-rw-rw-   0        0        0       31 2023-07-25 13:18:21.000000 pymeili-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      820 2023-07-25 14:37:08.692530 pymeili-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-07-25 13:25:52.000000 pymeili-0.0.4/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 14:37:08.681561 pymeili-0.0.4/pymeili/
+drwxrwxrwx   0        0        0        0 2023-07-25 14:37:08.691533 pymeili-0.0.4/pymeili/FONT/
+-rw-rw-rw-   0        0        0    40028 2016-07-20 20:40:52.000000 pymeili-0.0.4/pymeili/FONT/Futura Extra Black font.ttf
+-rw-rw-rw-   0        0        0    38980 2016-07-20 20:40:52.000000 pymeili-0.0.4/pymeili/FONT/Futura Heavy font.ttf
+-rw-rw-rw-   0        0        0    38764 2016-07-20 20:40:54.000000 pymeili-0.0.4/pymeili/FONT/futura medium bt.ttf
+-rw-rw-rw-   0        0        0      472 2023-07-25 14:36:50.000000 pymeili-0.0.4/pymeili/__init__.py
+-rw-rw-rw-   0        0        0    20601 2023-07-25 14:17:36.000000 pymeili-0.0.4/pymeili/beautifyplot.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:37:08.689540 pymeili-0.0.4/pymeili.egg-info/
+-rw-rw-rw-   0        0        0      820 2023-07-25 14:37:08.000000 pymeili-0.0.4/pymeili.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-07-25 14:37:08.000000 pymeili-0.0.4/pymeili.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 14:37:08.000000 pymeili-0.0.4/pymeili.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-25 14:37:08.000000 pymeili-0.0.4/pymeili.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 14:37:08.692530 pymeili-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      696 2023-07-25 14:36:36.000000 pymeili-0.0.4/setup.py
```

### Comparing `pymeili-0.0.3/FONT/Futura Extra Black font.ttf` & `pymeili-0.0.4/pymeili/FONT/Futura Extra Black font.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.0.3/FONT/Futura Heavy font.ttf` & `pymeili-0.0.4/pymeili/FONT/Futura Heavy font.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.0.3/FONT/futura medium bt.ttf` & `pymeili-0.0.4/pymeili/FONT/futura medium bt.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.0.3/LISCENCE.txt` & `pymeili-0.0.4/LISCENCE.txt`

 * *Files identical despite different names*

### Comparing `pymeili-0.0.3/pymeili/beautifyplot.py` & `pymeili-0.0.4/pymeili/beautifyplot.py`

 * *Files identical despite different names*

### Comparing `pymeili-0.0.3/setup.py` & `pymeili-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='pymeili',
-    version='0.0.3',
+    version='0.0.4',
     description='a module to beautify your python plot.',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='VVVictorZhou',
     author_email='vichouro@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

