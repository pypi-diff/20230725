# Comparing `tmp/pydise-0.0.1.tar.gz` & `tmp/pydise-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydise-0.0.1.tar", last modified: Tue Jul 25 00:41:30 2023, max compression
+gzip compressed data, was "pydise-0.0.2.tar", last modified: Tue Jul 25 12:38:49 2023, max compression
```

## Comparing `pydise-0.0.1.tar` & `pydise-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:41:30.166766 pydise-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:41:30.162766 pydise-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:41:30.166766 pydise-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-25 00:41:13.000000 pydise-0.0.1/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-25 00:41:13.000000 pydise-0.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-25 00:41:13.000000 pydise-0.0.1/.github/workflows/testing.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-25 00:41:13.000000 pydise-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-25 00:41:13.000000 pydise-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-07-25 00:41:30.166766 pydise-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-25 00:41:13.000000 pydise-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-25 00:41:13.000000 pydise-0.0.1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12741 2023-07-25 00:41:13.000000 pydise-0.0.1/detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:41:30.166766 pydise-0.0.1/pydise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-07-25 00:41:30.000000 pydise-0.0.1/pydise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-25 00:41:30.000000 pydise-0.0.1/pydise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 00:41:30.000000 pydise-0.0.1/pydise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-25 00:41:30.000000 pydise-0.0.1/pydise.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 00:41:30.000000 pydise-0.0.1/pydise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-25 00:41:30.170766 pydise-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-25 00:41:13.000000 pydise-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:41:30.166766 pydise-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-25 00:41:13.000000 pydise-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-25 00:41:13.000000 pydise-0.0.1/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-07-25 00:41:13.000000 pydise-0.0.1/tests/test_conditionals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-25 00:41:13.000000 pydise-0.0.1/tests/test_statements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:38:49.185637 pydise-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:38:49.185637 pydise-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:38:49.185637 pydise-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-25 12:38:36.000000 pydise-0.0.2/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-25 12:38:36.000000 pydise-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-25 12:38:36.000000 pydise-0.0.2/.github/workflows/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-25 12:38:36.000000 pydise-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-25 12:38:36.000000 pydise-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-07-25 12:38:49.185637 pydise-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-25 12:38:36.000000 pydise-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-25 12:38:36.000000 pydise-0.0.2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:38:49.185637 pydise-0.0.2/pydise/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-25 12:38:36.000000 pydise-0.0.2/pydise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12741 2023-07-25 12:38:36.000000 pydise-0.0.2/pydise/detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:38:49.185637 pydise-0.0.2/pydise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-07-25 12:38:49.000000 pydise-0.0.2/pydise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-25 12:38:49.000000 pydise-0.0.2/pydise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 12:38:49.000000 pydise-0.0.2/pydise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-25 12:38:49.000000 pydise-0.0.2/pydise.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 12:38:49.000000 pydise-0.0.2/pydise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-25 12:38:49.185637 pydise-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-25 12:38:36.000000 pydise-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:38:49.185637 pydise-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-25 12:38:36.000000 pydise-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-25 12:38:36.000000 pydise-0.0.2/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-07-25 12:38:36.000000 pydise-0.0.2/tests/test_conditionals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-25 12:38:36.000000 pydise-0.0.2/tests/test_statements.py
```

### Comparing `pydise-0.0.1/.github/workflows/lint.yml` & `pydise-0.0.2/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `pydise-0.0.1/.github/workflows/python-publish.yml` & `pydise-0.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pydise-0.0.1/.github/workflows/testing.yml` & `pydise-0.0.2/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `pydise-0.0.1/.gitignore` & `pydise-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pydise-0.0.1/LICENSE` & `pydise-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydise-0.0.1/PKG-INFO` & `pydise-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydise
-Version: 0.0.1
+Version: 0.0.2
 Summary: Detection of file that generate side effects when imported.
 Home-page: https://github.com/Hwoahwoa/pydise
 Author: Hwoahwoa
 Author-email: hwoahwoa@protonmail.com
 Keywords: python,import,side-effect
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pydise-0.0.1/README.md` & `pydise-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pydise-0.0.1/detector.py` & `pydise-0.0.2/pydise/detector.py`

 * *Files identical despite different names*

### Comparing `pydise-0.0.1/pydise.egg-info/PKG-INFO` & `pydise-0.0.2/pydise.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydise
-Version: 0.0.1
+Version: 0.0.2
 Summary: Detection of file that generate side effects when imported.
 Home-page: https://github.com/Hwoahwoa/pydise
 Author: Hwoahwoa
 Author-email: hwoahwoa@protonmail.com
 Keywords: python,import,side-effect
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pydise-0.0.1/setup.cfg` & `pydise-0.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -14,13 +14,13 @@
 
 [options]
 python_requires = >=3.9
 packages = find:
 
 [options.entry_points]
 console_scripts = 
-	pydise = detector:run
+	pydise = pydise.detector:run
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pydise-0.0.1/tests/test_base.py` & `pydise-0.0.2/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `pydise-0.0.1/tests/test_conditionals.py` & `pydise-0.0.2/tests/test_conditionals.py`

 * *Files identical despite different names*

### Comparing `pydise-0.0.1/tests/test_statements.py` & `pydise-0.0.2/tests/test_statements.py`

 * *Files identical despite different names*

