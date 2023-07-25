# Comparing `tmp/pylint-sqlalchemy-0.2.0.tar.gz` & `tmp/pylint-sqlalchemy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pylint-sqlalchemy-0.2.0.tar", last modified: Thu Jun 13 23:57:17 2019, max compression
+gzip compressed data, was "pylint-sqlalchemy-0.3.0.tar", last modified: Tue Jul 25 19:51:21 2023, max compression
```

## Comparing `pylint-sqlalchemy-0.2.0.tar` & `pylint-sqlalchemy-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 waksman    (502) staff       (20)        0 2019-06-13 23:57:17.000000 pylint-sqlalchemy-0.2.0/
--rw-r--r--   0 waksman    (502) staff       (20)      976 2019-06-13 23:57:17.000000 pylint-sqlalchemy-0.2.0/PKG-INFO
--rw-r--r--   0 waksman    (502) staff       (20)       97 2018-10-30 05:04:23.000000 pylint-sqlalchemy-0.2.0/README.rst
-drwxr-xr-x   0 waksman    (502) staff       (20)        0 2019-06-13 23:57:17.000000 pylint-sqlalchemy-0.2.0/pylint_sqlalchemy/
--rw-r--r--   0 waksman    (502) staff       (20)      410 2019-06-13 23:52:21.000000 pylint-sqlalchemy-0.2.0/pylint_sqlalchemy/__init__.py
--rw-r--r--   0 waksman    (502) staff       (20)       49 2019-06-13 23:54:31.000000 pylint-sqlalchemy-0.2.0/pylint_sqlalchemy/_version.py
--rw-r--r--   0 waksman    (502) staff       (20)      602 2018-10-31 06:02:42.000000 pylint-sqlalchemy-0.2.0/pylint_sqlalchemy/dml_no_argument.py
--rw-r--r--   0 waksman    (502) staff       (20)      860 2019-06-13 23:52:21.000000 pylint-sqlalchemy-0.2.0/pylint_sqlalchemy/orm.py
--rw-r--r--   0 waksman    (502) staff       (20)      758 2019-06-13 23:52:21.000000 pylint-sqlalchemy-0.2.0/pylint_sqlalchemy/plugin.py
-drwxr-xr-x   0 waksman    (502) staff       (20)        0 2019-06-13 23:57:17.000000 pylint-sqlalchemy-0.2.0/pylint_sqlalchemy.egg-info/
--rw-r--r--   0 waksman    (502) staff       (20)      976 2019-06-13 23:57:17.000000 pylint-sqlalchemy-0.2.0/pylint_sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 waksman    (502) staff       (20)      383 2019-06-13 23:57:17.000000 pylint-sqlalchemy-0.2.0/pylint_sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 waksman    (502) staff       (20)        1 2019-06-13 23:57:17.000000 pylint-sqlalchemy-0.2.0/pylint_sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 waksman    (502) staff       (20)       25 2019-06-13 23:57:17.000000 pylint-sqlalchemy-0.2.0/pylint_sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 waksman    (502) staff       (20)       18 2019-06-13 23:57:17.000000 pylint-sqlalchemy-0.2.0/pylint_sqlalchemy.egg-info/top_level.txt
--rw-r--r--   0 waksman    (502) staff       (20)      329 2019-06-13 23:57:17.000000 pylint-sqlalchemy-0.2.0/setup.cfg
--rw-r--r--   0 waksman    (502) staff       (20)     1515 2018-10-30 17:55:50.000000 pylint-sqlalchemy-0.2.0/setup.py
+drwxr-xr-x   0 waksman    (501) staff       (20)        0 2023-07-25 19:51:21.582317 pylint-sqlalchemy-0.3.0/
+-rw-r--r--   0 waksman    (501) staff       (20)     1078 2023-07-25 19:19:54.000000 pylint-sqlalchemy-0.3.0/LICENSE
+-rw-r--r--   0 waksman    (501) staff       (20)      907 2023-07-25 19:51:21.582543 pylint-sqlalchemy-0.3.0/PKG-INFO
+-rw-r--r--   0 waksman    (501) staff       (20)       97 2023-07-25 19:19:54.000000 pylint-sqlalchemy-0.3.0/README.rst
+drwxr-xr-x   0 waksman    (501) staff       (20)        0 2023-07-25 19:51:21.576670 pylint-sqlalchemy-0.3.0/pylint_sqlalchemy/
+-rw-r--r--   0 waksman    (501) staff       (20)      410 2023-07-25 19:19:54.000000 pylint-sqlalchemy-0.3.0/pylint_sqlalchemy/__init__.py
+-rw-r--r--   0 waksman    (501) staff       (20)       49 2023-07-25 19:48:50.000000 pylint-sqlalchemy-0.3.0/pylint_sqlalchemy/_version.py
+-rw-r--r--   0 waksman    (501) staff       (20)      602 2023-07-25 19:19:54.000000 pylint-sqlalchemy-0.3.0/pylint_sqlalchemy/dml_no_argument.py
+-rw-r--r--   0 waksman    (501) staff       (20)      860 2023-07-25 19:19:54.000000 pylint-sqlalchemy-0.3.0/pylint_sqlalchemy/orm.py
+-rw-r--r--   0 waksman    (501) staff       (20)      935 2023-07-25 19:25:01.000000 pylint-sqlalchemy-0.3.0/pylint_sqlalchemy/plugin.py
+drwxr-xr-x   0 waksman    (501) staff       (20)        0 2023-07-25 19:51:21.579254 pylint-sqlalchemy-0.3.0/pylint_sqlalchemy.egg-info/
+-rw-r--r--   0 waksman    (501) staff       (20)      907 2023-07-25 19:51:21.000000 pylint-sqlalchemy-0.3.0/pylint_sqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 waksman    (501) staff       (20)      442 2023-07-25 19:51:21.000000 pylint-sqlalchemy-0.3.0/pylint_sqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 waksman    (501) staff       (20)        1 2023-07-25 19:51:21.000000 pylint-sqlalchemy-0.3.0/pylint_sqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 waksman    (501) staff       (20)       25 2023-07-25 19:51:21.000000 pylint-sqlalchemy-0.3.0/pylint_sqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 waksman    (501) staff       (20)       18 2023-07-25 19:51:21.000000 pylint-sqlalchemy-0.3.0/pylint_sqlalchemy.egg-info/top_level.txt
+-rw-r--r--   0 waksman    (501) staff       (20)      329 2023-07-25 19:51:21.583885 pylint-sqlalchemy-0.3.0/setup.cfg
+-rw-r--r--   0 waksman    (501) staff       (20)     1746 2023-07-25 19:48:01.000000 pylint-sqlalchemy-0.3.0/setup.py
+drwxr-xr-x   0 waksman    (501) staff       (20)        0 2023-07-25 19:51:21.581217 pylint-sqlalchemy-0.3.0/tests/
+-rw-r--r--   0 waksman    (501) staff       (20)      945 2023-07-25 19:19:54.000000 pylint-sqlalchemy-0.3.0/tests/test_dml_no_argument.py
+-rw-r--r--   0 waksman    (501) staff       (20)      619 2023-07-25 19:19:54.000000 pylint-sqlalchemy-0.3.0/tests/test_plugin.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pylint-sqlalchemy-0.2.0/pylint_sqlalchemy/dml_no_argument.py` & `pylint-sqlalchemy-0.3.0/pylint_sqlalchemy/dml_no_argument.py`

 * *Files identical despite different names*

### Comparing `pylint-sqlalchemy-0.2.0/pylint_sqlalchemy/orm.py` & `pylint-sqlalchemy-0.3.0/pylint_sqlalchemy/orm.py`

 * *Files identical despite different names*

### Comparing `pylint-sqlalchemy-0.2.0/pylint_sqlalchemy/plugin.py` & `pylint-sqlalchemy-0.3.0/pylint_sqlalchemy/plugin.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,17 +10,24 @@
     """Handle the sqlalchemy.orm.scoping.scoped_session."""
     if cls.name == "scoped_session":
         source_files = cls.parent.file.split("/")
         source_files[-1] = "session.py"
         module = AstroidBuilder(MANAGER).file_build(
             "/".join(source_files), "sqlalchemy.orm.session"
         )
-        session = module.locals.get("Session")[0]
-        for method in Session.public_methods:
-            cls.locals[method] = session.locals[method]
+
+        session = None
+        for node in module.body:
+            if isinstance(node, astroid.ClassDef) and node.name == "Session":
+                session = node
+                break
+
+        if session:
+            for method in Session.public_methods:
+                cls.locals[method] = session.locals.get(method, None)
 
         return cls
 
     return None
 
 
 MANAGER.register_transform(astroid.ClassDef, handle_session)
```

### Comparing `pylint-sqlalchemy-0.2.0/setup.py` & `pylint-sqlalchemy-0.3.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 """Setup script for mtg_ssm."""
 
 import setuptools
 
 # Get version information without importing the package
 __version__ = None
-exec(open("pylint_sqlalchemy/_version.py", "r").read())  # pylint: disable=exec-used
+with open("pylint_sqlalchemy/_version.py", "rt", encoding="utf-8") as version_file:
+    exec(version_file.read())  # pylint: disable=exec-used
 
 SHORT_DESCRIPTION = "pylint plugin to fix incompatibility issues with sqlalchemy"
-LONG_DESCRIPTION = open("README.rst", "r").read()
+with open("README.rst", "rt", encoding="utf-8") as readme_file:
+    LONG_DESCRIPTION = readme_file.read()
 
-INSTALL_REQUIRES = [l.strip() for l in open("requirements.txt", "r")]
-TEST_DEPENDENCIES = [l.strip() for l in open("test_requirements.txt", "r")]
+with open("requirements.txt", "rt", encoding="utf-8") as requirements_file:
+    INSTALL_REQUIRES = [line.strip() for line in requirements_file]
+with open("test_requirements.txt", "rt", encoding="utf-8") as test_requirements_file:
+    TEST_DEPENDENCIES = [line.strip() for line in test_requirements_file]
 
 CLASSIFIERS = [
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: Unix",
-    "Programming Language :: Python :: 2.7",
-    "Programming Language :: Python :: 2",
-    "Programming Language :: Python :: 3.5",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Quality Assurance",
 ]
 
 setuptools.setup(
     name="pylint-sqlalchemy",
     version=__version__,
```

