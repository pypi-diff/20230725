# Comparing `tmp/dukeai_lib-0.1.4.tar.gz` & `tmp/dukeai_lib-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dukeai_lib-0.1.4.tar", last modified: Tue Jul 25 18:28:22 2023, max compression
+gzip compressed data, was "dukeai_lib-0.1.5.tar", last modified: Tue Jul 25 18:34:58 2023, max compression
```

## Comparing `dukeai_lib-0.1.4.tar` & `dukeai_lib-0.1.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:28:22.003729 dukeai_lib-0.1.4/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    35821 2023-07-25 15:06:39.000000 dukeai_lib-0.1.4/LICENSE
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1228 2023-07-25 18:28:22.003729 dukeai_lib-0.1.4/PKG-INFO
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      579 2023-07-25 17:10:39.000000 dukeai_lib-0.1.4/README.md
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:28:21.989755 dukeai_lib-0.1.4/dukeai_lib/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      251 2023-07-25 18:20:57.000000 dukeai_lib-0.1.4/dukeai_lib/__init__.py
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:28:21.995730 dukeai_lib-0.1.4/dukeai_lib/application/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:18:00.000000 dukeai_lib-0.1.4/dukeai_lib/application/__init__.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     3603 2023-07-25 15:46:15.000000 dukeai_lib-0.1.4/dukeai_lib/application/application.py
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:28:21.997730 dukeai_lib-0.1.4/dukeai_lib/tools/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:18:26.000000 dukeai_lib-0.1.4/dukeai_lib/tools/__init__.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      619 2023-07-25 15:37:06.000000 dukeai_lib-0.1.4/dukeai_lib/tools/tools.py
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:28:21.999729 dukeai_lib-0.1.4/dukeai_lib/utilities/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:18:43.000000 dukeai_lib-0.1.4/dukeai_lib/utilities/__init__.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      312 2023-07-25 15:45:02.000000 dukeai_lib-0.1.4/dukeai_lib/utilities/utilities.py
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:28:21.994730 dukeai_lib-0.1.4/dukeai_lib.egg-info/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1228 2023-07-25 18:28:21.000000 dukeai_lib-0.1.4/dukeai_lib.egg-info/PKG-INFO
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      493 2023-07-25 18:28:21.000000 dukeai_lib-0.1.4/dukeai_lib.egg-info/SOURCES.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        1 2023-07-25 18:28:21.000000 dukeai_lib-0.1.4/dukeai_lib.egg-info/dependency_links.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       63 2023-07-25 18:28:21.000000 dukeai_lib-0.1.4/dukeai_lib.egg-info/requires.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       15 2023-07-25 18:28:21.000000 dukeai_lib-0.1.4/dukeai_lib.egg-info/top_level.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      754 2023-07-25 18:20:57.000000 dukeai_lib-0.1.4/pyproject.toml
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       38 2023-07-25 18:28:22.003729 dukeai_lib-0.1.4/setup.cfg
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      874 2023-07-25 18:28:10.000000 dukeai_lib-0.1.4/setup.py
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:28:22.002730 dukeai_lib-0.1.4/src/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      280 2023-07-25 18:09:54.000000 dukeai_lib-0.1.4/src/__init__.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     3603 2023-07-25 15:46:15.000000 dukeai_lib-0.1.4/src/application.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      619 2023-07-25 15:37:06.000000 dukeai_lib-0.1.4/src/tools.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      312 2023-07-25 15:45:02.000000 dukeai_lib-0.1.4/src/utilities.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:34:58.165010 dukeai_lib-0.1.5/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    35821 2023-07-25 15:06:39.000000 dukeai_lib-0.1.5/LICENSE
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1228 2023-07-25 18:34:58.165010 dukeai_lib-0.1.5/PKG-INFO
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      579 2023-07-25 17:10:39.000000 dukeai_lib-0.1.5/README.md
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:34:58.142470 dukeai_lib-0.1.5/dukeai_lib/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      308 2023-07-25 18:31:49.000000 dukeai_lib-0.1.5/dukeai_lib/__init__.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:34:58.155010 dukeai_lib-0.1.5/dukeai_lib/application/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:18:00.000000 dukeai_lib-0.1.5/dukeai_lib/application/__init__.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     3603 2023-07-25 15:46:15.000000 dukeai_lib-0.1.5/dukeai_lib/application/application.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:34:58.158010 dukeai_lib-0.1.5/dukeai_lib/tools/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:18:26.000000 dukeai_lib-0.1.5/dukeai_lib/tools/__init__.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      619 2023-07-25 15:37:06.000000 dukeai_lib-0.1.5/dukeai_lib/tools/tools.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:34:58.160010 dukeai_lib-0.1.5/dukeai_lib/utilities/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:18:43.000000 dukeai_lib-0.1.5/dukeai_lib/utilities/__init__.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      312 2023-07-25 15:45:02.000000 dukeai_lib-0.1.5/dukeai_lib/utilities/utilities.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:34:58.153011 dukeai_lib-0.1.5/dukeai_lib.egg-info/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1228 2023-07-25 18:34:57.000000 dukeai_lib-0.1.5/dukeai_lib.egg-info/PKG-INFO
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      493 2023-07-25 18:34:57.000000 dukeai_lib-0.1.5/dukeai_lib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        1 2023-07-25 18:34:57.000000 dukeai_lib-0.1.5/dukeai_lib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       63 2023-07-25 18:34:57.000000 dukeai_lib-0.1.5/dukeai_lib.egg-info/requires.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       15 2023-07-25 18:34:57.000000 dukeai_lib-0.1.5/dukeai_lib.egg-info/top_level.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      754 2023-07-25 18:31:49.000000 dukeai_lib-0.1.5/pyproject.toml
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       38 2023-07-25 18:34:58.166010 dukeai_lib-0.1.5/setup.cfg
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      874 2023-07-25 18:31:49.000000 dukeai_lib-0.1.5/setup.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:34:58.164010 dukeai_lib-0.1.5/src/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      280 2023-07-25 18:09:54.000000 dukeai_lib-0.1.5/src/__init__.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     3603 2023-07-25 15:46:15.000000 dukeai_lib-0.1.5/src/application.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      619 2023-07-25 15:37:06.000000 dukeai_lib-0.1.5/src/tools.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      312 2023-07-25 15:45:02.000000 dukeai_lib-0.1.5/src/utilities.py
```

### Comparing `dukeai_lib-0.1.4/LICENSE` & `dukeai_lib-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.4/PKG-INFO` & `dukeai_lib-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dukeai_lib
-Version: 0.1.4
+Version: 0.1.5
 Summary: Common functions used across the DUKE.ai project environments.
 Home-page: https://duke.ai
 Author: Blake Donahoo
 Author-email: Blake Donahoo <blake@duke.ai>
 License: GNU General Public License v3 (GPLv3)
 Keywords: dukeai,duke.ai
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dukeai_lib-0.1.4/README.md` & `dukeai_lib-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.4/dukeai_lib/application/application.py` & `dukeai_lib-0.1.5/dukeai_lib/application/application.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.4/dukeai_lib/tools/tools.py` & `dukeai_lib-0.1.5/dukeai_lib/tools/tools.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.4/dukeai_lib.egg-info/PKG-INFO` & `dukeai_lib-0.1.5/dukeai_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dukeai-lib
-Version: 0.1.4
+Version: 0.1.5
 Summary: Common functions used across the DUKE.ai project environments.
 Home-page: https://duke.ai
 Author: Blake Donahoo
 Author-email: Blake Donahoo <blake@duke.ai>
 License: GNU General Public License v3 (GPLv3)
 Keywords: dukeai,duke.ai
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dukeai_lib-0.1.4/pyproject.toml` & `dukeai_lib-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-systems]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dukeai_lib"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Blake Donahoo", email="blake@duke.ai" },
 ]
 description = "Common functions used across the DUKE.ai project environments."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dukeai_lib-0.1.4/setup.py` & `dukeai_lib-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dukeai_lib',
-    version="0.1.4",
+    version="0.1.5",
     description="Common functions used across the DUKE.ai project environments.",
     url='https://duke.ai',
     author='Blake Donahoo',
     author_email='blake@duke.ai',
     license='GNU General Public License v3 (GPLv3)',
     packages=find_packages(),
     keywords=['dukeai', 'duke.ai'],
```

### Comparing `dukeai_lib-0.1.4/src/application.py` & `dukeai_lib-0.1.5/src/application.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.4/src/tools.py` & `dukeai_lib-0.1.5/src/tools.py`

 * *Files identical despite different names*

