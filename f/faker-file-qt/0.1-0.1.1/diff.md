# Comparing `tmp/faker-file-qt-0.1.tar.gz` & `tmp/faker-file-qt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faker-file-qt-0.1.tar", last modified: Sun Jul 23 22:14:00 2023, max compression
+gzip compressed data, was "faker-file-qt-0.1.1.tar", last modified: Mon Jul 24 22:12:42 2023, max compression
```

## Comparing `faker-file-qt-0.1.tar` & `faker-file-qt-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,17 @@
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-07-23 22:14:00.513897 faker-file-qt-0.1/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      170 2023-07-23 20:21:53.000000 faker-file-qt-0.1/.coveragerc
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       34 2023-07-23 20:21:53.000000 faker-file-qt-0.1/.env
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      417 2023-07-23 21:59:16.000000 faker-file-qt-0.1/.gitignore
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      375 2023-07-23 20:21:53.000000 faker-file-qt-0.1/.matyan.ini
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      629 2023-07-23 20:21:53.000000 faker-file-qt-0.1/CHANGELOG.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1077 2023-07-23 20:21:53.000000 faker-file-qt-0.1/LICENSE.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       61 2023-07-23 20:21:53.000000 faker-file-qt-0.1/MANIFEST.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1019 2023-07-23 22:01:41.000000 faker-file-qt-0.1/Makefile
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6184 2023-07-23 22:14:00.513897 faker-file-qt-0.1/PKG-INFO
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4953 2023-07-23 21:44:30.000000 faker-file-qt-0.1/README.rst
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-07-23 22:14:00.513897 faker-file-qt-0.1/faker_file_qt.egg-info/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6184 2023-07-23 22:14:00.000000 faker-file-qt-0.1/faker_file_qt.egg-info/PKG-INFO
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      400 2023-07-23 22:14:00.000000 faker-file-qt-0.1/faker_file_qt.egg-info/SOURCES.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        1 2023-07-23 22:14:00.000000 faker-file-qt-0.1/faker_file_qt.egg-info/dependency_links.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       53 2023-07-23 22:14:00.000000 faker-file-qt-0.1/faker_file_qt.egg-info/entry_points.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      108 2023-07-23 22:14:00.000000 faker-file-qt-0.1/faker_file_qt.egg-info/requires.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       14 2023-07-23 22:14:00.000000 faker-file-qt-0.1/faker_file_qt.egg-info/top_level.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    13369 2023-07-23 21:09:33.000000 faker-file-qt-0.1/faker_file_qt.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2012 2023-07-23 20:21:53.000000 faker-file-qt-0.1/pyproject.toml
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      478 2023-07-23 20:21:53.000000 faker-file-qt-0.1/pytest.ini
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      328 2023-07-23 22:14:00.517897 faker-file-qt-0.1/setup.cfg
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2085 2023-07-23 22:02:58.000000 faker-file-qt-0.1/setup.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5790 2023-07-23 21:37:55.000000 faker-file-qt-0.1/tests.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      290 2023-07-23 20:21:53.000000 faker-file-qt-0.1/tox.ini
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-07-24 22:12:42.325620 faker-file-qt-0.1.1/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      717 2023-07-24 22:11:42.000000 faker-file-qt-0.1.1/CHANGELOG.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1077 2023-07-23 20:21:53.000000 faker-file-qt-0.1.1/LICENSE.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       61 2023-07-23 20:21:53.000000 faker-file-qt-0.1.1/MANIFEST.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6132 2023-07-24 22:12:42.325620 faker-file-qt-0.1.1/PKG-INFO
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4953 2023-07-23 21:44:30.000000 faker-file-qt-0.1.1/README.rst
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-07-24 22:12:42.325620 faker-file-qt-0.1.1/faker_file_qt.egg-info/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6132 2023-07-24 22:12:42.000000 faker-file-qt-0.1.1/faker_file_qt.egg-info/PKG-INFO
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      323 2023-07-24 22:12:42.000000 faker-file-qt-0.1.1/faker_file_qt.egg-info/SOURCES.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        1 2023-07-24 22:12:42.000000 faker-file-qt-0.1.1/faker_file_qt.egg-info/dependency_links.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       53 2023-07-24 22:12:42.000000 faker-file-qt-0.1.1/faker_file_qt.egg-info/entry_points.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      114 2023-07-24 22:12:42.000000 faker-file-qt-0.1.1/faker_file_qt.egg-info/requires.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       14 2023-07-24 22:12:42.000000 faker-file-qt-0.1.1/faker_file_qt.egg-info/top_level.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    16225 2023-07-24 22:12:11.000000 faker-file-qt-0.1.1/faker_file_qt.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2077 2023-07-24 20:06:13.000000 faker-file-qt-0.1.1/pyproject.toml
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      328 2023-07-24 22:12:42.329620 faker-file-qt-0.1.1/setup.cfg
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2051 2023-07-24 22:11:53.000000 faker-file-qt-0.1.1/setup.py
```

### Comparing `faker-file-qt-0.1/CHANGELOG.rst` & `faker-file-qt-0.1.1/CHANGELOG.rst`

 * *Files 20% similar despite different names*

```diff
@@ -11,12 +11,19 @@
 - It's always safe to upgrade within the same minor version (for example, from
   0.3 to 0.3.4).
 - Minor version changes might be backwards incompatible. Read the
   release notes carefully before upgrading (for example, when upgrading from
   0.3.4 to 0.4).
 - All backwards incompatible changes are mentioned in this document.
 
+0.1.1
+-----
+2023-07-25
+
+- UI improvements.
+- Open default app on click on the results.
+
 0.1
 ---
-2023-07-22
+2023-07-24
 
 - Initial beta release.
```

### Comparing `faker-file-qt-0.1/LICENSE.rst` & `faker-file-qt-0.1.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `faker-file-qt-0.1/PKG-INFO` & `faker-file-qt-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: faker-file-qt
-Version: 0.1
-Summary: QT frontend for faker-file.
+Version: 0.1.1
+Summary: PyQT UI for faker-file.
 Home-page: https://github.com/barseghyanartur/faker-file-qt/
 Author: Artur Barseghyan
 Author-email: artur.barseghyan@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/barseghyanartur/faker-file-qt/issues
 Project-URL: Documentation, https://faker-file-qt.readthedocs.io/
 Project-URL: Source Code, https://github.com/barseghyanartur/faker-file-qt/
 Project-URL: Changelog, https://faker-file-qt.readthedocs.io/en/latest/changelog.html
 Keywords: faker-file faker-file-qt
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: X11 Applications
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Testing
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: dev
 License-File: LICENSE.rst
 
 =============
 faker-file-qt
 =============
 PyQT UI for `faker-file`_.
```

### Comparing `faker-file-qt-0.1/README.rst` & `faker-file-qt-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `faker-file-qt-0.1/faker_file_qt.egg-info/PKG-INFO` & `faker-file-qt-0.1.1/faker_file_qt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: faker-file-qt
-Version: 0.1
-Summary: QT frontend for faker-file.
+Version: 0.1.1
+Summary: PyQT UI for faker-file.
 Home-page: https://github.com/barseghyanartur/faker-file-qt/
 Author: Artur Barseghyan
 Author-email: artur.barseghyan@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/barseghyanartur/faker-file-qt/issues
 Project-URL: Documentation, https://faker-file-qt.readthedocs.io/
 Project-URL: Source Code, https://github.com/barseghyanartur/faker-file-qt/
 Project-URL: Changelog, https://faker-file-qt.readthedocs.io/en/latest/changelog.html
 Keywords: faker-file faker-file-qt
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: X11 Applications
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Testing
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: dev
 License-File: LICENSE.rst
 
 =============
 faker-file-qt
 =============
 PyQT UI for `faker-file`_.
```

### Comparing `faker-file-qt-0.1/pyproject.toml` & `faker-file-qt-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 extend-exclude = '''
 /(
   # The following are specific to Black, you probably don't want those.
   | blib2to3
   | tests/data
   | profiling
   | migrations
+  | .tox
 )/
 '''
 
 # Build system information below.
 # NOTE: You don't need this in your own Black configuration.
 [build-system]
 requires = ["setuptools>=41.0", "setuptools-scm", "wheel"]
@@ -32,15 +33,15 @@
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 ensure_newline_before_comments = true
 line_length = 80
 known_first_party = "faker_file_qt"
 known_third_party = ["factory"]
-skip = ["wsgi.py",]
+skip = ["wsgi.py", ".tox"]
 
 [tool.ruff]
 line-length = 80
 
 # Enable Pyflakes `E` and `F` codes by default.
 select = ["E", "F"]
 ignore = []
@@ -72,18 +73,19 @@
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
 # Assume Python 3.10.
 target-version = "py310"
 
 [tool.pyright]
-include = ["src"]
+include = ["faker_file_qt.py", "tests.py", "setup.py"]
 exclude = ["**/node_modules",
     "**/__pycache__",
-    "tmp"
+    "tmp",
+    ".tox"
 ]
 ignore = ["src/oldstuff"]
 defineConstant = { DEBUG = true }
 stubPath = "src/stubs"
 
 reportMissingImports = true
 reportMissingTypeStubs = false
```

### Comparing `faker-file-qt-0.1/setup.py` & `faker-file-qt-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from setuptools import setup
 
-version = "0.1"
+version = "0.1.1"
 
 try:
     readme = open(os.path.join(os.path.dirname(__file__), "README.rst")).read()
 except OSError:
     readme = ""
 
 install_requires = [
@@ -16,35 +16,35 @@
     "PyQt5",
     "Pillow<=9.5.0",
 ]
 
 extras_require = {
     "dev": [
         "black",
-        "doc8",
         "detect-secrets",
-        "isort",
+        "doc8",
         "ipython",
+        "isort",
         "ruff",
+        "twine",
     ]
 }
 
 tests_require = [
     "pytest",
     "pytest-cov",
     "tox",
 ]
 
 setup(
     name="faker-file-qt",
     version=version,
-    description="QT frontend for faker-file.",
+    description="PyQT UI for faker-file.",
     long_description=readme,
     classifiers=[
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Environment :: X11 Applications",
         "Environment :: X11 Applications :: Qt",
         "License :: OSI Approved :: MIT License",
@@ -65,13 +65,13 @@
     entry_points={"console_scripts": ["faker-file-qt = faker_file_qt:main"]},
     keywords="faker-file faker-file-qt",
     author="Artur Barseghyan",
     author_email="artur.barseghyan@gmail.com",
     url="https://github.com/barseghyanartur/faker-file-qt/",
     py_modules=["faker_file_qt"],
     license="MIT",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=install_requires,
     extras_require=extras_require,
     tests_require=tests_require,
     include_package_data=True,
 )
```

