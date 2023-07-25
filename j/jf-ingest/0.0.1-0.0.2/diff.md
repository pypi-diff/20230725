# Comparing `tmp/jf_ingest-0.0.1.tar.gz` & `tmp/jf_ingest-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jf_ingest-0.0.1.tar", last modified: Fri Jul 21 20:13:06 2023, max compression
+gzip compressed data, was "jf_ingest-0.0.2.tar", last modified: Tue Jul 25 19:08:07 2023, max compression
```

## Comparing `jf_ingest-0.0.1.tar` & `jf_ingest-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1066 2023-07-19 15:50:56.382404 jf_ingest-0.0.1/LICENSE
--rw-r--r--   0        0        0       19 2023-07-21 18:28:01.314703 jf_ingest-0.0.1/README.md
--rw-r--r--   0        0        0      610 2023-07-21 20:13:06.575550 jf_ingest-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-21 18:28:01.319487 jf_ingest-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      372 1970-01-01 00:00:00.000000 jf_ingest-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-19 15:50:56.382404 jf_ingest-0.0.2/LICENSE
+-rw-r--r--   0        0        0       19 2023-07-21 18:28:01.314703 jf_ingest-0.0.2/README.md
+-rw-r--r--   0        0        0      619 2023-07-25 19:08:07.247513 jf_ingest-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 18:28:01.319487 jf_ingest-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      377 1970-01-01 00:00:00.000000 jf_ingest-0.0.2/PKG-INFO
```

### Comparing `jf_ingest-0.0.1/LICENSE` & `jf_ingest-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jf_ingest-0.0.1/pyproject.toml` & `jf_ingest-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "jf_ingest"
-version = "0.0.1"
+version = "0.0.2"
 readme = "README.md"
 description = "library used for ingesting jira data"
 authors = [
     { name = "jellyfish-oss", email = "oss@jellyfish.co" },
 ]
 dependencies = [
-    "jira==3.5.2",
+    "jira >= 2.0.0, < 2.1",
     "requests-mock==1.11.0",
 ]
 requires-python = ">=3.10"
 
 [project.license]
 text = "MIT"
```

