# Comparing `tmp/dukeai_lib-0.1.2.tar.gz` & `tmp/dukeai_lib-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dukeai_lib-0.1.2.tar", last modified: Tue Jul 25 17:36:05 2023, max compression
+gzip compressed data, was "dukeai_lib-0.1.3.tar", last modified: Tue Jul 25 17:55:48 2023, max compression
```

## Comparing `dukeai_lib-0.1.2.tar` & `dukeai_lib-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 17:36:05.106084 dukeai_lib-0.1.2/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    35821 2023-07-25 15:06:39.000000 dukeai_lib-0.1.2/LICENSE
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1151 2023-07-25 17:36:05.106084 dukeai_lib-0.1.2/PKG-INFO
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      579 2023-07-25 17:10:39.000000 dukeai_lib-0.1.2/README.md
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      794 2023-07-25 17:35:49.000000 dukeai_lib-0.1.2/pyproject.toml
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       38 2023-07-25 17:36:05.106084 dukeai_lib-0.1.2/setup.cfg
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 17:36:05.100084 dukeai_lib-0.1.2/src/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       78 2023-07-25 17:35:38.000000 dukeai_lib-0.1.2/src/__init__.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     3603 2023-07-25 15:46:15.000000 dukeai_lib-0.1.2/src/application.py
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 17:36:05.105085 dukeai_lib-0.1.2/src/dukeai_lib.egg-info/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1151 2023-07-25 17:36:05.000000 dukeai_lib-0.1.2/src/dukeai_lib.egg-info/PKG-INFO
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      286 2023-07-25 17:36:05.000000 dukeai_lib-0.1.2/src/dukeai_lib.egg-info/SOURCES.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        1 2023-07-25 17:36:05.000000 dukeai_lib-0.1.2/src/dukeai_lib.egg-info/dependency_links.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       63 2023-07-25 17:36:05.000000 dukeai_lib-0.1.2/src/dukeai_lib.egg-info/requires.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       37 2023-07-25 17:36:05.000000 dukeai_lib-0.1.2/src/dukeai_lib.egg-info/top_level.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      619 2023-07-25 15:37:06.000000 dukeai_lib-0.1.2/src/tools.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      312 2023-07-25 15:45:02.000000 dukeai_lib-0.1.2/src/utilities.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 17:55:48.641900 dukeai_lib-0.1.3/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    35821 2023-07-25 15:06:39.000000 dukeai_lib-0.1.3/LICENSE
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1188 2023-07-25 17:55:48.641900 dukeai_lib-0.1.3/PKG-INFO
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      579 2023-07-25 17:10:39.000000 dukeai_lib-0.1.3/README.md
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      754 2023-07-25 17:48:14.000000 dukeai_lib-0.1.3/pyproject.toml
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       38 2023-07-25 17:55:48.642899 dukeai_lib-0.1.3/setup.cfg
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      776 2023-07-25 17:55:42.000000 dukeai_lib-0.1.3/setup.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 17:55:48.635899 dukeai_lib-0.1.3/src/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      153 2023-07-25 17:53:40.000000 dukeai_lib-0.1.3/src/__init__.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     3603 2023-07-25 15:46:15.000000 dukeai_lib-0.1.3/src/application.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 17:55:48.640900 dukeai_lib-0.1.3/src/dukeai_lib.egg-info/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1188 2023-07-25 17:55:48.000000 dukeai_lib-0.1.3/src/dukeai_lib.egg-info/PKG-INFO
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      295 2023-07-25 17:55:48.000000 dukeai_lib-0.1.3/src/dukeai_lib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        1 2023-07-25 17:55:48.000000 dukeai_lib-0.1.3/src/dukeai_lib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       63 2023-07-25 17:55:48.000000 dukeai_lib-0.1.3/src/dukeai_lib.egg-info/requires.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       37 2023-07-25 17:55:48.000000 dukeai_lib-0.1.3/src/dukeai_lib.egg-info/top_level.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      619 2023-07-25 15:37:06.000000 dukeai_lib-0.1.3/src/tools.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      312 2023-07-25 15:45:02.000000 dukeai_lib-0.1.3/src/utilities.py
```

### Comparing `dukeai_lib-0.1.2/LICENSE` & `dukeai_lib-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.2/PKG-INFO` & `dukeai_lib-0.1.3/src/dukeai_lib.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
-Name: dukeai_lib
-Version: 0.1.2
+Name: dukeai-lib
+Version: 0.1.3
 Summary: Common functions used across the DUKE.ai project environments.
+Home-page: 
+Author: Blake Donahoo
 Author-email: Blake Donahoo <blake@duke.ai>
+License: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Classifier: Environment :: X11 Applications
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ### Duke.ai Lib (*dukeai_lib*)
```

### Comparing `dukeai_lib-0.1.2/README.md` & `dukeai_lib-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.2/pyproject.toml` & `dukeai_lib-0.1.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 [build-systems]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dukeai_lib"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Blake Donahoo", email="blake@duke.ai" },
 ]
 description = "Common functions used across the DUKE.ai project environments."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
-    "Environment :: X11 Applications",
     "Topic :: Utilities"
 ]
 dependencies = [
     'chalice~=1.27.1',
     'requests~=2.27.1',
     'base58==2.1.1',
     'urllib3==1.26.9'
```

### Comparing `dukeai_lib-0.1.2/src/application.py` & `dukeai_lib-0.1.3/src/application.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.2/src/dukeai_lib.egg-info/PKG-INFO` & `dukeai_lib-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
-Name: dukeai-lib
-Version: 0.1.2
+Name: dukeai_lib
+Version: 0.1.3
 Summary: Common functions used across the DUKE.ai project environments.
+Home-page: 
+Author: Blake Donahoo
 Author-email: Blake Donahoo <blake@duke.ai>
+License: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Classifier: Environment :: X11 Applications
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ### Duke.ai Lib (*dukeai_lib*)
```

### Comparing `dukeai_lib-0.1.2/src/tools.py` & `dukeai_lib-0.1.3/src/tools.py`

 * *Files identical despite different names*

