# Comparing `tmp/toot-0.9.0.tar.gz` & `tmp/toot-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/toot-0.9.0.tar", last modified: Fri Apr 21 18:28:58 2017, max compression
+gzip compressed data, was "dist/toot-0.9.1.tar", last modified: Mon Apr 24 07:40:03 2017, max compression
```

## Comparing `toot-0.9.0.tar` & `toot-0.9.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2017-04-21 18:28:58.000000 toot-0.9.0/
--rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)     4358 2017-04-21 18:28:58.000000 toot-0.9.0/PKG-INFO
--rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)     2825 2017-04-21 18:27:41.000000 toot-0.9.0/README.rst
-drwxrwxr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2017-04-21 18:28:58.000000 toot-0.9.0/toot/
--rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)     7322 2017-04-21 18:22:30.000000 toot-0.9.0/toot/curses.py
--rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)     9350 2017-04-21 17:14:51.000000 toot-0.9.0/toot/commands.py
--rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)     4683 2017-04-21 10:56:07.000000 toot-0.9.0/toot/api.py
--rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)      465 2017-04-19 12:41:02.000000 toot-0.9.0/toot/__init__.py
--rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)     1589 2017-04-18 13:37:26.000000 toot-0.9.0/toot/config.py
--rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)      531 2017-04-19 12:12:53.000000 toot-0.9.0/toot/output.py
--rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)     5873 2017-04-21 17:30:19.000000 toot-0.9.0/toot/console.py
--rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)     1144 2017-04-21 18:25:07.000000 toot-0.9.0/setup.py
-drwxrwxr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2017-04-21 18:28:58.000000 toot-0.9.0/toot.egg-info/
--rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)        1 2017-04-21 18:28:58.000000 toot-0.9.0/toot.egg-info/dependency_links.txt
--rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)     4358 2017-04-21 18:28:58.000000 toot-0.9.0/toot.egg-info/PKG-INFO
--rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)       44 2017-04-21 18:28:58.000000 toot-0.9.0/toot.egg-info/entry_points.txt
--rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)      306 2017-04-21 18:28:58.000000 toot-0.9.0/toot.egg-info/SOURCES.txt
--rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)        5 2017-04-21 18:28:58.000000 toot-0.9.0/toot.egg-info/top_level.txt
--rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)       48 2017-04-21 18:28:58.000000 toot-0.9.0/toot.egg-info/requires.txt
--rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)       67 2017-04-21 18:28:58.000000 toot-0.9.0/setup.cfg
+drwxrwxr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2017-04-24 07:40:03.000000 toot-0.9.1/
+-rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)     4358 2017-04-24 07:40:03.000000 toot-0.9.1/PKG-INFO
+-rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)     2825 2017-04-21 18:27:41.000000 toot-0.9.1/README.rst
+drwxrwxr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2017-04-24 07:40:03.000000 toot-0.9.1/toot/
+-rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)     9347 2017-04-24 07:37:25.000000 toot-0.9.1/toot/commands.py
+-rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)     4683 2017-04-21 10:56:07.000000 toot-0.9.1/toot/api.py
+-rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)      465 2017-04-19 12:41:02.000000 toot-0.9.1/toot/__init__.py
+-rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)     1589 2017-04-18 13:37:26.000000 toot-0.9.1/toot/config.py
+-rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)     7322 2017-04-24 07:26:16.000000 toot-0.9.1/toot/app.py
+-rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)      531 2017-04-19 12:12:53.000000 toot-0.9.1/toot/output.py
+-rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)     5873 2017-04-21 17:30:19.000000 toot-0.9.1/toot/console.py
+-rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)     1144 2017-04-24 07:39:02.000000 toot-0.9.1/setup.py
+drwxrwxr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2017-04-24 07:40:03.000000 toot-0.9.1/toot.egg-info/
+-rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)        1 2017-04-24 07:40:03.000000 toot-0.9.1/toot.egg-info/dependency_links.txt
+-rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)     4358 2017-04-24 07:40:03.000000 toot-0.9.1/toot.egg-info/PKG-INFO
+-rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)       44 2017-04-24 07:40:03.000000 toot-0.9.1/toot.egg-info/entry_points.txt
+-rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)      303 2017-04-24 07:40:03.000000 toot-0.9.1/toot.egg-info/SOURCES.txt
+-rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)        5 2017-04-24 07:40:03.000000 toot-0.9.1/toot.egg-info/top_level.txt
+-rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)       48 2017-04-24 07:40:03.000000 toot-0.9.1/toot.egg-info/requires.txt
+-rw-rw-r--   0 ihabunek  (1000) ihabunek  (1000)       67 2017-04-24 07:40:03.000000 toot-0.9.1/setup.cfg
```

### Comparing `toot-0.9.0/PKG-INFO` & `toot-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: toot
-Version: 0.9.0
+Version: 0.9.1
 Summary: Interact with Mastodon social networks from the command line.
 Home-page: https://github.com/ihabunek/toot/
 Author: Ivan Habunek
 Author-email: ivan@habunek.com
 License: MIT
 Description: =============================
         Toot - Mastodon CLI interface
```

### Comparing `toot-0.9.0/README.rst` & `toot-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `toot-0.9.0/toot/curses.py` & `toot-0.9.1/toot/app.py`

 * *Files identical despite different names*

### Comparing `toot-0.9.0/toot/commands.py` & `toot-0.9.1/toot/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from future.moves.itertools import zip_longest
 from getpass import getpass
 from itertools import chain
 from textwrap import TextWrapper, wrap
 
 from toot import api, config, DEFAULT_INSTANCE, User, App, ConsoleError
 from toot.output import green, yellow, print_error
-from toot.curses import TimelineApp
+from toot.app import TimelineApp
 
 
 def register_app(instance):
     print("Registering application with %s" % green(instance))
 
     try:
         response = api.create_app(instance)
```

### Comparing `toot-0.9.0/toot/api.py` & `toot-0.9.1/toot/api.py`

 * *Files identical despite different names*

### Comparing `toot-0.9.0/toot/config.py` & `toot-0.9.1/toot/config.py`

 * *Files identical despite different names*

### Comparing `toot-0.9.0/toot/output.py` & `toot-0.9.1/toot/output.py`

 * *Files identical despite different names*

### Comparing `toot-0.9.0/toot/console.py` & `toot-0.9.1/toot/console.py`

 * *Files identical despite different names*

### Comparing `toot-0.9.0/setup.py` & `toot-0.9.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open("README.rst") as readme:
     long_description = readme.read()
 
 setup(
     name='toot',
-    version='0.9.0',
+    version='0.9.1',
     description='Interact with Mastodon social networks from the command line.',
     long_description=long_description,
     author='Ivan Habunek',
     author_email='ivan@habunek.com',
     url='https://github.com/ihabunek/toot/',
     keywords='mastodon toot',
     license='MIT',
```

### Comparing `toot-0.9.0/toot.egg-info/PKG-INFO` & `toot-0.9.1/toot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: toot
-Version: 0.9.0
+Version: 0.9.1
 Summary: Interact with Mastodon social networks from the command line.
 Home-page: https://github.com/ihabunek/toot/
 Author: Ivan Habunek
 Author-email: ivan@habunek.com
 License: MIT
 Description: =============================
         Toot - Mastodon CLI interface
```

