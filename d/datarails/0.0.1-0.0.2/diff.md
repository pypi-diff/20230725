# Comparing `tmp/datarails-0.0.1.tar.gz` & `tmp/datarails-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datarails-0.0.1.tar", last modified: Mon Jul 24 15:26:50 2023, max compression
+gzip compressed data, was "datarails-0.0.2.tar", last modified: Tue Jul 25 04:16:02 2023, max compression
```

## Comparing `datarails-0.0.1.tar` & `datarails-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:26:50.961773 datarails-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-24 15:26:50.961773 datarails-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-24 15:26:29.000000 datarails-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:26:50.961773 datarails-0.0.1/datarails/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 15:26:29.000000 datarails-0.0.1/datarails/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-24 15:26:29.000000 datarails-0.0.1/datarails/databox.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-24 15:26:29.000000 datarails-0.0.1/datarails/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-24 15:26:29.000000 datarails-0.0.1/datarails/step.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-24 15:26:29.000000 datarails-0.0.1/datarails/type_vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:26:50.961773 datarails-0.0.1/datarails.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-24 15:26:50.000000 datarails-0.0.1/datarails.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-24 15:26:50.000000 datarails-0.0.1/datarails.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 15:26:50.000000 datarails-0.0.1/datarails.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-24 15:26:50.000000 datarails-0.0.1/datarails.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-24 15:26:50.000000 datarails-0.0.1/datarails.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-24 15:26:29.000000 datarails-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 15:26:50.961773 datarails-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-24 15:26:29.000000 datarails-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:26:50.961773 datarails-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-24 15:26:29.000000 datarails-0.0.1/tests/test_databox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-24 15:26:29.000000 datarails-0.0.1/tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-24 15:26:29.000000 datarails-0.0.1/tests/test_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 04:16:02.009071 datarails-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-25 04:16:02.009071 datarails-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-25 04:15:54.000000 datarails-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 04:16:02.005071 datarails-0.0.2/datarails/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 04:15:54.000000 datarails-0.0.2/datarails/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-25 04:15:13.000000 datarails-0.0.2/datarails/databox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-25 04:15:13.000000 datarails-0.0.2/datarails/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-25 04:15:13.000000 datarails-0.0.2/datarails/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-25 04:15:13.000000 datarails-0.0.2/datarails/type_vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 04:16:02.005071 datarails-0.0.2/datarails.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-25 04:16:01.000000 datarails-0.0.2/datarails.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-25 04:16:02.000000 datarails-0.0.2/datarails.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 04:16:01.000000 datarails-0.0.2/datarails.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-25 04:16:01.000000 datarails-0.0.2/datarails.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-25 04:16:01.000000 datarails-0.0.2/datarails.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-25 04:15:54.000000 datarails-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 04:16:02.009071 datarails-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-25 04:15:13.000000 datarails-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 04:16:02.005071 datarails-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-25 04:15:13.000000 datarails-0.0.2/tests/test_databox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-25 04:15:13.000000 datarails-0.0.2/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-25 04:15:13.000000 datarails-0.0.2/tests/test_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 04:16:02.001070 datarails-0.0.2/venv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 04:16:02.009071 datarails-0.0.2/venv/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      639 2023-07-25 04:15:51.000000 datarails-0.0.2/venv/bin/rst2html.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      761 2023-07-25 04:15:51.000000 datarails-0.0.2/venv/bin/rst2html4.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1096 2023-07-25 04:15:51.000000 datarails-0.0.2/venv/bin/rst2html5.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      838 2023-07-25 04:15:51.000000 datarails-0.0.2/venv/bin/rst2latex.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      661 2023-07-25 04:15:51.000000 datarails-0.0.2/venv/bin/rst2man.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      827 2023-07-25 04:15:51.000000 datarails-0.0.2/venv/bin/rst2odt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      633 2023-07-25 04:15:51.000000 datarails-0.0.2/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      646 2023-07-25 04:15:51.000000 datarails-0.0.2/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      682 2023-07-25 04:15:51.000000 datarails-0.0.2/venv/bin/rst2s5.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      918 2023-07-25 04:15:51.000000 datarails-0.0.2/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      647 2023-07-25 04:15:51.000000 datarails-0.0.2/venv/bin/rst2xml.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      715 2023-07-25 04:15:51.000000 datarails-0.0.2/venv/bin/rstpep2html.py
```

### Comparing `datarails-0.0.1/datarails/databox.py` & `datarails-0.0.2/datarails/databox.py`

 * *Files identical despite different names*

### Comparing `datarails-0.0.1/datarails/runner.py` & `datarails-0.0.2/datarails/runner.py`

 * *Files identical despite different names*

### Comparing `datarails-0.0.1/datarails/step.py` & `datarails-0.0.2/datarails/step.py`

 * *Files identical despite different names*

### Comparing `datarails-0.0.1/pyproject.toml` & `datarails-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "datarails"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 readme = "README.md"
 requires-python = ">=3.9"
 
 
 [project.optional-dependencies]
 dev = [
```

### Comparing `datarails-0.0.1/tests/test_databox.py` & `datarails-0.0.2/tests/test_databox.py`

 * *Files identical despite different names*

### Comparing `datarails-0.0.1/tests/test_runner.py` & `datarails-0.0.2/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `datarails-0.0.1/tests/test_step.py` & `datarails-0.0.2/tests/test_step.py`

 * *Files identical despite different names*

