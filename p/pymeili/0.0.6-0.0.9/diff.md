# Comparing `tmp/pymeili-0.0.6.tar.gz` & `tmp/pymeili-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymeili-0.0.6.tar", last modified: Tue Jul 25 15:17:29 2023, max compression
+gzip compressed data, was "pymeili-0.0.9.tar", last modified: Tue Jul 25 15:40:14 2023, max compression
```

## Comparing `pymeili-0.0.6.tar` & `pymeili-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 15:17:29.519273 pymeili-0.0.6/
--rw-rw-rw-   0        0        0      147 2023-07-25 15:16:42.000000 pymeili-0.0.6/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1057 2023-07-25 12:28:38.000000 pymeili-0.0.6/LISCENCE.txt
--rw-rw-rw-   0        0        0       31 2023-07-25 13:18:21.000000 pymeili-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      824 2023-07-25 15:17:29.518275 pymeili-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-07-25 13:25:52.000000 pymeili-0.0.6/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-25 15:17:29.507308 pymeili-0.0.6/pymeili/
-drwxrwxrwx   0        0        0        0 2023-07-25 15:17:29.518275 pymeili-0.0.6/pymeili/FONT/
--rw-rw-rw-   0        0        0    40028 2016-07-20 20:40:52.000000 pymeili-0.0.6/pymeili/FONT/Futura Extra Black font.ttf
--rw-rw-rw-   0        0        0    38980 2016-07-20 20:40:52.000000 pymeili-0.0.6/pymeili/FONT/Futura Heavy font.ttf
--rw-rw-rw-   0        0        0    38764 2016-07-20 20:40:54.000000 pymeili-0.0.6/pymeili/FONT/futura medium bt.ttf
--rw-rw-rw-   0        0        0      480 2023-07-25 15:16:38.000000 pymeili-0.0.6/pymeili/__init__.py
--rw-rw-rw-   0        0        0    20878 2023-07-25 15:16:57.000000 pymeili-0.0.6/pymeili/beautifyplot.py
-drwxrwxrwx   0        0        0        0 2023-07-25 15:17:29.515283 pymeili-0.0.6/pymeili.egg-info/
--rw-rw-rw-   0        0        0      824 2023-07-25 15:17:29.000000 pymeili-0.0.6/pymeili.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-07-25 15:17:29.000000 pymeili-0.0.6/pymeili.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 15:17:29.000000 pymeili-0.0.6/pymeili.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-25 15:17:29.000000 pymeili-0.0.6/pymeili.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 15:17:29.519273 pymeili-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      696 2023-07-25 15:16:46.000000 pymeili-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 15:40:14.124917 pymeili-0.0.9/
+-rw-rw-rw-   0        0        0      147 2023-07-25 15:33:17.000000 pymeili-0.0.9/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1057 2023-07-25 12:28:38.000000 pymeili-0.0.9/LISCENCE.txt
+-rw-rw-rw-   0        0        0       36 2023-07-25 15:28:50.000000 pymeili-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1090 2023-07-25 15:40:14.123920 pymeili-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2023-07-25 15:39:56.000000 pymeili-0.0.9/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 15:40:14.111952 pymeili-0.0.9/pymeili/
+drwxrwxrwx   0        0        0        0 2023-07-25 15:40:14.123920 pymeili-0.0.9/pymeili/FONT/
+-rw-rw-rw-   0        0        0    40028 2016-07-20 20:40:52.000000 pymeili-0.0.9/pymeili/FONT/Futura Extra Black font.ttf
+-rw-rw-rw-   0        0        0    38980 2016-07-20 20:40:52.000000 pymeili-0.0.9/pymeili/FONT/Futura Heavy font.ttf
+-rw-rw-rw-   0        0        0    38764 2016-07-20 20:40:54.000000 pymeili-0.0.9/pymeili/FONT/futura medium bt.ttf
+-rw-rw-rw-   0        0        0      480 2023-07-25 15:33:20.000000 pymeili-0.0.9/pymeili/__init__.py
+-rw-rw-rw-   0        0        0    20878 2023-07-25 15:18:43.000000 pymeili-0.0.9/pymeili/beautifyplot.py
+drwxrwxrwx   0        0        0        0 2023-07-25 15:40:14.120929 pymeili-0.0.9/pymeili.egg-info/
+-rw-rw-rw-   0        0        0     1090 2023-07-25 15:40:14.000000 pymeili-0.0.9/pymeili.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-07-25 15:40:14.000000 pymeili-0.0.9/pymeili.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 15:40:14.000000 pymeili-0.0.9/pymeili.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-25 15:40:14.000000 pymeili-0.0.9/pymeili.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 15:40:14.124917 pymeili-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      724 2023-07-25 15:39:58.000000 pymeili-0.0.9/setup.py
```

### Comparing `pymeili-0.0.6/LISCENCE.txt` & `pymeili-0.0.9/LISCENCE.txt`

 * *Files identical despite different names*

### Comparing `pymeili-0.0.6/pymeili/FONT/Futura Extra Black font.ttf` & `pymeili-0.0.9/pymeili/FONT/Futura Extra Black font.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.0.6/pymeili/FONT/Futura Heavy font.ttf` & `pymeili-0.0.9/pymeili/FONT/Futura Heavy font.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.0.6/pymeili/FONT/futura medium bt.ttf` & `pymeili-0.0.9/pymeili/FONT/futura medium bt.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.0.6/pymeili/beautifyplot.py` & `pymeili-0.0.9/pymeili/beautifyplot.py`

 * *Files identical despite different names*

### Comparing `pymeili-0.0.6/setup.py` & `pymeili-0.0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from setuptools import setup, find_packages
+from setuptools import setup, find_packages, Extension
 
 classifiers = [
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='pymeili',
-    version='0.0.6',
+    version='0.0.9',
     description='a module to beautify your python plot.',
-    long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
+    long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt',encoding="utf-8").read(),
     url='',
     author='VVVictorZhou',
     author_email='vichouro@gmail.com',
     license='MIT',
     classifiers=classifiers,
     keywords='beautify',
     packages=find_packages(),
```

