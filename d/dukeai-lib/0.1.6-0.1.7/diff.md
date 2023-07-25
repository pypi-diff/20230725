# Comparing `tmp/dukeai_lib-0.1.6.tar.gz` & `tmp/dukeai_lib-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dukeai_lib-0.1.6.tar", last modified: Tue Jul 25 18:38:46 2023, max compression
+gzip compressed data, was "dukeai_lib-0.1.7.tar", last modified: Tue Jul 25 18:43:56 2023, max compression
```

## Comparing `dukeai_lib-0.1.6.tar` & `dukeai_lib-0.1.7.tar`

### file list

```diff
@@ -1,29 +1,23 @@
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:38:46.396402 dukeai_lib-0.1.6/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    35821 2023-07-25 15:06:39.000000 dukeai_lib-0.1.6/LICENSE
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1228 2023-07-25 18:38:46.395402 dukeai_lib-0.1.6/PKG-INFO
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      579 2023-07-25 17:10:39.000000 dukeai_lib-0.1.6/README.md
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:38:46.382439 dukeai_lib-0.1.6/dukeai_lib/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      410 2023-07-25 18:38:32.000000 dukeai_lib-0.1.6/dukeai_lib/__init__.py
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:38:46.387402 dukeai_lib-0.1.6/dukeai_lib/application/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:18:00.000000 dukeai_lib-0.1.6/dukeai_lib/application/__init__.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     3603 2023-07-25 15:46:15.000000 dukeai_lib-0.1.6/dukeai_lib/application/application.py
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:38:46.389402 dukeai_lib-0.1.6/dukeai_lib/tools/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:18:26.000000 dukeai_lib-0.1.6/dukeai_lib/tools/__init__.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      619 2023-07-25 15:37:06.000000 dukeai_lib-0.1.6/dukeai_lib/tools/tools.py
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:38:46.391402 dukeai_lib-0.1.6/dukeai_lib/utilities/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:18:43.000000 dukeai_lib-0.1.6/dukeai_lib/utilities/__init__.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      312 2023-07-25 15:45:02.000000 dukeai_lib-0.1.6/dukeai_lib/utilities/utilities.py
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:38:46.386402 dukeai_lib-0.1.6/dukeai_lib.egg-info/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1228 2023-07-25 18:38:46.000000 dukeai_lib-0.1.6/dukeai_lib.egg-info/PKG-INFO
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      493 2023-07-25 18:38:46.000000 dukeai_lib-0.1.6/dukeai_lib.egg-info/SOURCES.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        1 2023-07-25 18:38:46.000000 dukeai_lib-0.1.6/dukeai_lib.egg-info/dependency_links.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       63 2023-07-25 18:38:46.000000 dukeai_lib-0.1.6/dukeai_lib.egg-info/requires.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       15 2023-07-25 18:38:46.000000 dukeai_lib-0.1.6/dukeai_lib.egg-info/top_level.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      754 2023-07-25 18:38:32.000000 dukeai_lib-0.1.6/pyproject.toml
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       38 2023-07-25 18:38:46.396402 dukeai_lib-0.1.6/setup.cfg
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      874 2023-07-25 18:38:31.000000 dukeai_lib-0.1.6/setup.py
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:38:46.394402 dukeai_lib-0.1.6/src/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      280 2023-07-25 18:09:54.000000 dukeai_lib-0.1.6/src/__init__.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     3603 2023-07-25 15:46:15.000000 dukeai_lib-0.1.6/src/application.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      619 2023-07-25 15:37:06.000000 dukeai_lib-0.1.6/src/tools.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      312 2023-07-25 15:45:02.000000 dukeai_lib-0.1.6/src/utilities.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:43:56.573861 dukeai_lib-0.1.7/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    35821 2023-07-25 15:06:39.000000 dukeai_lib-0.1.7/LICENSE
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1228 2023-07-25 18:43:56.572860 dukeai_lib-0.1.7/PKG-INFO
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      579 2023-07-25 17:10:39.000000 dukeai_lib-0.1.7/README.md
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:43:56.564861 dukeai_lib-0.1.7/dukeai_lib/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      200 2023-07-25 18:43:29.000000 dukeai_lib-0.1.7/dukeai_lib/__init__.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     3603 2023-07-25 15:46:15.000000 dukeai_lib-0.1.7/dukeai_lib/application.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      619 2023-07-25 15:37:06.000000 dukeai_lib-0.1.7/dukeai_lib/tools.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      312 2023-07-25 15:45:02.000000 dukeai_lib-0.1.7/dukeai_lib/utilities.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:43:56.568861 dukeai_lib-0.1.7/dukeai_lib.egg-info/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1228 2023-07-25 18:43:56.000000 dukeai_lib-0.1.7/dukeai_lib.egg-info/PKG-INFO
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      368 2023-07-25 18:43:56.000000 dukeai_lib-0.1.7/dukeai_lib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        1 2023-07-25 18:43:56.000000 dukeai_lib-0.1.7/dukeai_lib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       63 2023-07-25 18:43:56.000000 dukeai_lib-0.1.7/dukeai_lib.egg-info/requires.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       15 2023-07-25 18:43:56.000000 dukeai_lib-0.1.7/dukeai_lib.egg-info/top_level.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      754 2023-07-25 18:43:29.000000 dukeai_lib-0.1.7/pyproject.toml
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       38 2023-07-25 18:43:56.573861 dukeai_lib-0.1.7/setup.cfg
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      874 2023-07-25 18:43:29.000000 dukeai_lib-0.1.7/setup.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 18:43:56.571861 dukeai_lib-0.1.7/src/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      280 2023-07-25 18:09:54.000000 dukeai_lib-0.1.7/src/__init__.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     3603 2023-07-25 15:46:15.000000 dukeai_lib-0.1.7/src/application.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      619 2023-07-25 15:37:06.000000 dukeai_lib-0.1.7/src/tools.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      312 2023-07-25 15:45:02.000000 dukeai_lib-0.1.7/src/utilities.py
```

### Comparing `dukeai_lib-0.1.6/LICENSE` & `dukeai_lib-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.6/PKG-INFO` & `dukeai_lib-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dukeai_lib
-Version: 0.1.6
+Version: 0.1.7
 Summary: Common functions used across the DUKE.ai project environments.
 Home-page: https://duke.ai
 Author: Blake Donahoo
 Author-email: Blake Donahoo <blake@duke.ai>
 License: GNU General Public License v3 (GPLv3)
 Keywords: dukeai,duke.ai
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dukeai_lib-0.1.6/README.md` & `dukeai_lib-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.6/dukeai_lib/application/application.py` & `dukeai_lib-0.1.7/dukeai_lib/application.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.6/dukeai_lib/tools/tools.py` & `dukeai_lib-0.1.7/dukeai_lib/tools.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.6/dukeai_lib.egg-info/PKG-INFO` & `dukeai_lib-0.1.7/dukeai_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dukeai-lib
-Version: 0.1.6
+Version: 0.1.7
 Summary: Common functions used across the DUKE.ai project environments.
 Home-page: https://duke.ai
 Author: Blake Donahoo
 Author-email: Blake Donahoo <blake@duke.ai>
 License: GNU General Public License v3 (GPLv3)
 Keywords: dukeai,duke.ai
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dukeai_lib-0.1.6/pyproject.toml` & `dukeai_lib-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-systems]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dukeai_lib"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="Blake Donahoo", email="blake@duke.ai" },
 ]
 description = "Common functions used across the DUKE.ai project environments."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dukeai_lib-0.1.6/setup.py` & `dukeai_lib-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dukeai_lib',
-    version="0.1.6",
+    version="0.1.7",
     description="Common functions used across the DUKE.ai project environments.",
     url='https://duke.ai',
     author='Blake Donahoo',
     author_email='blake@duke.ai',
     license='GNU General Public License v3 (GPLv3)',
     packages=find_packages(),
     keywords=['dukeai', 'duke.ai'],
```

### Comparing `dukeai_lib-0.1.6/src/application.py` & `dukeai_lib-0.1.7/src/application.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.6/src/tools.py` & `dukeai_lib-0.1.7/src/tools.py`

 * *Files identical despite different names*

