# Comparing `tmp/flake8_private_name_import-0.1.0.tar.gz` & `tmp/flake8_private_name_import-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flake8_private_name_import-0.1.0.tar", last modified: Tue Jul 25 20:26:05 2023, max compression
+gzip compressed data, was "dist/flake8_private_name_import-0.1.1.tar", last modified: Tue Jul 25 20:54:32 2023, max compression
```

## Comparing `flake8_private_name_import-0.1.0.tar` & `flake8_private_name_import-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 rows      (1000) rows      (1000)        0 2023-07-25 20:26:05.000000 flake8_private_name_import-0.1.0/
--rw-rw-r--   0 rows      (1000) rows      (1000)     1308 2023-07-25 20:26:05.000000 flake8_private_name_import-0.1.0/PKG-INFO
--rw-rw-r--   0 rows      (1000) rows      (1000)       81 2023-07-25 20:19:44.000000 flake8_private_name_import-0.1.0/README.md
-drwxrwxr-x   0 rows      (1000) rows      (1000)        0 2023-07-25 20:26:05.000000 flake8_private_name_import-0.1.0/flake8_private_name_import.egg-info/
--rw-rw-r--   0 rows      (1000) rows      (1000)     1308 2023-07-25 20:26:05.000000 flake8_private_name_import-0.1.0/flake8_private_name_import.egg-info/PKG-INFO
--rw-rw-r--   0 rows      (1000) rows      (1000)      369 2023-07-25 20:26:05.000000 flake8_private_name_import-0.1.0/flake8_private_name_import.egg-info/SOURCES.txt
--rw-rw-r--   0 rows      (1000) rows      (1000)        1 2023-07-25 20:26:05.000000 flake8_private_name_import-0.1.0/flake8_private_name_import.egg-info/dependency_links.txt
--rw-rw-r--   0 rows      (1000) rows      (1000)       63 2023-07-25 20:26:05.000000 flake8_private_name_import-0.1.0/flake8_private_name_import.egg-info/entry_points.txt
--rw-rw-r--   0 rows      (1000) rows      (1000)        1 2023-07-25 20:26:05.000000 flake8_private_name_import-0.1.0/flake8_private_name_import.egg-info/not-zip-safe
--rw-rw-r--   0 rows      (1000) rows      (1000)       22 2023-07-25 20:26:05.000000 flake8_private_name_import-0.1.0/flake8_private_name_import.egg-info/requires.txt
--rw-rw-r--   0 rows      (1000) rows      (1000)       13 2023-07-25 20:26:05.000000 flake8_private_name_import-0.1.0/flake8_private_name_import.egg-info/top_level.txt
--rw-rw-r--   0 rows      (1000) rows      (1000)       38 2023-07-25 20:26:05.000000 flake8_private_name_import-0.1.0/setup.cfg
--rw-rw-r--   0 rows      (1000) rows      (1000)     1756 2023-07-25 20:22:11.000000 flake8_private_name_import-0.1.0/setup.py
+drwxrwxr-x   0 rows      (1000) rows      (1000)        0 2023-07-25 20:54:32.000000 flake8_private_name_import-0.1.1/
+-rw-rw-r--   0 rows      (1000) rows      (1000)     1308 2023-07-25 20:54:32.000000 flake8_private_name_import-0.1.1/PKG-INFO
+-rw-rw-r--   0 rows      (1000) rows      (1000)       81 2023-07-25 20:19:44.000000 flake8_private_name_import-0.1.1/README.md
+drwxrwxr-x   0 rows      (1000) rows      (1000)        0 2023-07-25 20:54:32.000000 flake8_private_name_import-0.1.1/flake8_private_name_import.egg-info/
+-rw-rw-r--   0 rows      (1000) rows      (1000)     1308 2023-07-25 20:54:31.000000 flake8_private_name_import-0.1.1/flake8_private_name_import.egg-info/PKG-INFO
+-rw-rw-r--   0 rows      (1000) rows      (1000)      399 2023-07-25 20:54:32.000000 flake8_private_name_import-0.1.1/flake8_private_name_import.egg-info/SOURCES.txt
+-rw-rw-r--   0 rows      (1000) rows      (1000)        1 2023-07-25 20:54:31.000000 flake8_private_name_import-0.1.1/flake8_private_name_import.egg-info/dependency_links.txt
+-rw-rw-r--   0 rows      (1000) rows      (1000)       63 2023-07-25 20:54:31.000000 flake8_private_name_import-0.1.1/flake8_private_name_import.egg-info/entry_points.txt
+-rw-rw-r--   0 rows      (1000) rows      (1000)        1 2023-07-25 20:54:31.000000 flake8_private_name_import-0.1.1/flake8_private_name_import.egg-info/not-zip-safe
+-rw-rw-r--   0 rows      (1000) rows      (1000)       29 2023-07-25 20:54:31.000000 flake8_private_name_import-0.1.1/flake8_private_name_import.egg-info/requires.txt
+-rw-rw-r--   0 rows      (1000) rows      (1000)       27 2023-07-25 20:54:31.000000 flake8_private_name_import-0.1.1/flake8_private_name_import.egg-info/top_level.txt
+-rw-rw-r--   0 rows      (1000) rows      (1000)     1395 2023-07-25 20:53:25.000000 flake8_private_name_import-0.1.1/flake8_private_name_import.py
+-rw-rw-r--   0 rows      (1000) rows      (1000)       38 2023-07-25 20:54:32.000000 flake8_private_name_import-0.1.1/setup.cfg
+-rw-rw-r--   0 rows      (1000) rows      (1000)     1779 2023-07-25 20:51:33.000000 flake8_private_name_import-0.1.1/setup.py
```

### Comparing `flake8_private_name_import-0.1.0/PKG-INFO` & `flake8_private_name_import-0.1.1/flake8_private_name_import.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: flake8_private_name_import
-Version: 0.1.0
+Name: flake8-private-name-import
+Version: 0.1.1
 Summary: flake8 plugin that reports imports of private names
 Home-page: https://github.com/rows-s/flake8_private_name_import
 Author: Vladimir Marmuz
 Author-email: vladimir.rows@gmail.com
 License: MIT
 Description: flake8 plugin that reports imports of private names
 Keywords: python pep8 flake8 private import
```

### Comparing `flake8_private_name_import-0.1.0/flake8_private_name_import.egg-info/PKG-INFO` & `flake8_private_name_import-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: flake8-private-name-import
-Version: 0.1.0
+Name: flake8_private_name_import
+Version: 0.1.1
 Summary: flake8 plugin that reports imports of private names
 Home-page: https://github.com/rows-s/flake8_private_name_import
 Author: Vladimir Marmuz
 Author-email: vladimir.rows@gmail.com
 License: MIT
 Description: flake8 plugin that reports imports of private names
 Keywords: python pep8 flake8 private import
```

### Comparing `flake8_private_name_import-0.1.0/setup.py` & `flake8_private_name_import-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='flake8_private_name_import',
-    version='0.1.0',
+    version='0.1.1',
     description="flake8 plugin that reports imports of private names",
     long_description="flake8 plugin that reports imports of private names",
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Framework :: Flake8',
@@ -27,19 +27,19 @@
     ],
     python_requires='>=3.7',
     keywords='python pep8 flake8 private import',
     author='Vladimir Marmuz',
     author_email='vladimir.rows@gmail.com',
     url='https://github.com/rows-s/flake8_private_name_import',
     license='MIT',
-    py_modules=['flake8_isort'],
+    py_modules=['flake8_private_name_import'],
     include_package_data=True,
     test_suite='run_tests',
     zip_safe=False,
-    install_requires=['flake8'],
+    install_requires=['flake8 >= 3.3.0'],
     extras_require={
         'test': [
             'pytest',
         ],
     },
     entry_points={
         'flake8.extension': [
```

