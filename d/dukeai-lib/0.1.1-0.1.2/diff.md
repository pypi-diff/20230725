# Comparing `tmp/dukeai_lib-0.1.1.tar.gz` & `tmp/dukeai_lib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dukeai_lib-0.1.1.tar", last modified: Tue Jul 25 17:12:21 2023, max compression
+gzip compressed data, was "dukeai_lib-0.1.2.tar", last modified: Tue Jul 25 17:36:05 2023, max compression
```

## Comparing `dukeai_lib-0.1.1.tar` & `dukeai_lib-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 17:12:21.624866 dukeai_lib-0.1.1/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    35821 2023-07-25 15:06:39.000000 dukeai_lib-0.1.1/LICENSE
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1151 2023-07-25 17:12:21.624866 dukeai_lib-0.1.1/PKG-INFO
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      579 2023-07-25 17:10:39.000000 dukeai_lib-0.1.1/README.md
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      794 2023-07-25 17:10:39.000000 dukeai_lib-0.1.1/pyproject.toml
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       38 2023-07-25 17:12:21.625866 dukeai_lib-0.1.1/setup.cfg
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 17:12:21.619866 dukeai_lib-0.1.1/src/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 15:02:25.000000 dukeai_lib-0.1.1/src/__init__.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     3603 2023-07-25 15:46:15.000000 dukeai_lib-0.1.1/src/application.py
-drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 17:12:21.623866 dukeai_lib-0.1.1/src/dukeai_lib.egg-info/
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1151 2023-07-25 17:12:21.000000 dukeai_lib-0.1.1/src/dukeai_lib.egg-info/PKG-INFO
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      286 2023-07-25 17:12:21.000000 dukeai_lib-0.1.1/src/dukeai_lib.egg-info/SOURCES.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        1 2023-07-25 17:12:21.000000 dukeai_lib-0.1.1/src/dukeai_lib.egg-info/dependency_links.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       63 2023-07-25 17:12:21.000000 dukeai_lib-0.1.1/src/dukeai_lib.egg-info/requires.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       37 2023-07-25 17:12:21.000000 dukeai_lib-0.1.1/src/dukeai_lib.egg-info/top_level.txt
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      619 2023-07-25 15:37:06.000000 dukeai_lib-0.1.1/src/tools.py
--rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      312 2023-07-25 15:45:02.000000 dukeai_lib-0.1.1/src/utilities.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 17:36:05.106084 dukeai_lib-0.1.2/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)    35821 2023-07-25 15:06:39.000000 dukeai_lib-0.1.2/LICENSE
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1151 2023-07-25 17:36:05.106084 dukeai_lib-0.1.2/PKG-INFO
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      579 2023-07-25 17:10:39.000000 dukeai_lib-0.1.2/README.md
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      794 2023-07-25 17:35:49.000000 dukeai_lib-0.1.2/pyproject.toml
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       38 2023-07-25 17:36:05.106084 dukeai_lib-0.1.2/setup.cfg
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 17:36:05.100084 dukeai_lib-0.1.2/src/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       78 2023-07-25 17:35:38.000000 dukeai_lib-0.1.2/src/__init__.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     3603 2023-07-25 15:46:15.000000 dukeai_lib-0.1.2/src/application.py
+drwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        0 2023-07-25 17:36:05.105085 dukeai_lib-0.1.2/src/dukeai_lib.egg-info/
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)     1151 2023-07-25 17:36:05.000000 dukeai_lib-0.1.2/src/dukeai_lib.egg-info/PKG-INFO
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      286 2023-07-25 17:36:05.000000 dukeai_lib-0.1.2/src/dukeai_lib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)        1 2023-07-25 17:36:05.000000 dukeai_lib-0.1.2/src/dukeai_lib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       63 2023-07-25 17:36:05.000000 dukeai_lib-0.1.2/src/dukeai_lib.egg-info/requires.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)       37 2023-07-25 17:36:05.000000 dukeai_lib-0.1.2/src/dukeai_lib.egg-info/top_level.txt
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      619 2023-07-25 15:37:06.000000 dukeai_lib-0.1.2/src/tools.py
+-rwxrwxrwx   0 dsent999-t  (1000) dsent999-t  (1000)      312 2023-07-25 15:45:02.000000 dukeai_lib-0.1.2/src/utilities.py
```

### Comparing `dukeai_lib-0.1.1/LICENSE` & `dukeai_lib-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.1/PKG-INFO` & `dukeai_lib-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dukeai_lib
-Version: 0.1.1
+Version: 0.1.2
 Summary: Common functions used across the DUKE.ai project environments.
 Author-email: Blake Donahoo <blake@duke.ai>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `dukeai_lib-0.1.1/README.md` & `dukeai_lib-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.1/pyproject.toml` & `dukeai_lib-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-systems]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dukeai_lib"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Blake Donahoo", email="blake@duke.ai" },
 ]
 description = "Common functions used across the DUKE.ai project environments."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dukeai_lib-0.1.1/src/application.py` & `dukeai_lib-0.1.2/src/application.py`

 * *Files identical despite different names*

### Comparing `dukeai_lib-0.1.1/src/dukeai_lib.egg-info/PKG-INFO` & `dukeai_lib-0.1.2/src/dukeai_lib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dukeai-lib
-Version: 0.1.1
+Version: 0.1.2
 Summary: Common functions used across the DUKE.ai project environments.
 Author-email: Blake Donahoo <blake@duke.ai>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `dukeai_lib-0.1.1/src/tools.py` & `dukeai_lib-0.1.2/src/tools.py`

 * *Files identical despite different names*

