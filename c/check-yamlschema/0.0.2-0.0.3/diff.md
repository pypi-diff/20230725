# Comparing `tmp/check-yamlschema-0.0.2.tar.gz` & `tmp/check-yamlschema-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jmlrt/git/jmlrt/check-yamlschema/dist/.tmp-zmyhwyi1/check-yamlschema-0.0.2.tar", last modified: Thu Mar 30 14:19:49 2023, max compression
+gzip compressed data, was "check-yamlschema-0.0.3.tar", last modified: Tue Jul 25 12:04:50 2023, max compression
```

## Comparing `check-yamlschema-0.0.2.tar` & `check-yamlschema-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jmlrt      (501) staff       (20)        0 2023-03-30 14:19:49.000000 check-yamlschema-0.0.2/
--rw-r--r--   0 jmlrt      (501) staff       (20)     1073 2023-03-30 11:05:36.000000 check-yamlschema-0.0.2/LICENSE
--rw-r--r--   0 jmlrt      (501) staff       (20)     1773 2023-03-30 14:19:49.000000 check-yamlschema-0.0.2/PKG-INFO
--rw-r--r--   0 jmlrt      (501) staff       (20)     1402 2023-03-30 13:52:50.000000 check-yamlschema-0.0.2/README.md
-drwxr-xr-x   0 jmlrt      (501) staff       (20)        0 2023-03-30 14:19:49.000000 check-yamlschema-0.0.2/check_yamlschema.egg-info/
--rw-r--r--   0 jmlrt      (501) staff       (20)     1773 2023-03-30 14:19:49.000000 check-yamlschema-0.0.2/check_yamlschema.egg-info/PKG-INFO
--rw-r--r--   0 jmlrt      (501) staff       (20)      298 2023-03-30 14:19:49.000000 check-yamlschema-0.0.2/check_yamlschema.egg-info/SOURCES.txt
--rw-r--r--   0 jmlrt      (501) staff       (20)        1 2023-03-30 14:19:49.000000 check-yamlschema-0.0.2/check_yamlschema.egg-info/dependency_links.txt
--rw-r--r--   0 jmlrt      (501) staff       (20)       59 2023-03-30 14:19:49.000000 check-yamlschema-0.0.2/check_yamlschema.egg-info/entry_points.txt
--rw-r--r--   0 jmlrt      (501) staff       (20)       27 2023-03-30 14:19:49.000000 check-yamlschema-0.0.2/check_yamlschema.egg-info/requires.txt
--rw-r--r--   0 jmlrt      (501) staff       (20)       17 2023-03-30 14:19:49.000000 check-yamlschema-0.0.2/check_yamlschema.egg-info/top_level.txt
--rw-r--r--   0 jmlrt      (501) staff       (20)     2486 2023-03-30 13:22:08.000000 check-yamlschema-0.0.2/check_yamlschema.py
--rw-r--r--   0 jmlrt      (501) staff       (20)      680 2023-03-30 14:19:49.000000 check-yamlschema-0.0.2/setup.cfg
--rw-r--r--   0 jmlrt      (501) staff       (20)       74 2023-03-30 12:14:19.000000 check-yamlschema-0.0.2/setup.py
+drwxr-xr-x   0 jmlrt      (501) staff       (20)        0 2023-07-25 12:04:50.843700 check-yamlschema-0.0.3/
+-rw-r--r--   0 jmlrt      (501) staff       (20)     1073 2023-07-25 10:31:52.000000 check-yamlschema-0.0.3/LICENSE
+-rw-r--r--   0 jmlrt      (501) staff       (20)     1773 2023-07-25 12:04:50.843807 check-yamlschema-0.0.3/PKG-INFO
+-rw-r--r--   0 jmlrt      (501) staff       (20)     1402 2023-07-25 10:31:52.000000 check-yamlschema-0.0.3/README.md
+drwxr-xr-x   0 jmlrt      (501) staff       (20)        0 2023-07-25 12:04:50.843217 check-yamlschema-0.0.3/check_yamlschema.egg-info/
+-rw-r--r--   0 jmlrt      (501) staff       (20)     1773 2023-07-25 12:04:50.000000 check-yamlschema-0.0.3/check_yamlschema.egg-info/PKG-INFO
+-rw-r--r--   0 jmlrt      (501) staff       (20)      298 2023-07-25 12:04:50.000000 check-yamlschema-0.0.3/check_yamlschema.egg-info/SOURCES.txt
+-rw-r--r--   0 jmlrt      (501) staff       (20)        1 2023-07-25 12:04:50.000000 check-yamlschema-0.0.3/check_yamlschema.egg-info/dependency_links.txt
+-rw-r--r--   0 jmlrt      (501) staff       (20)       59 2023-07-25 12:04:50.000000 check-yamlschema-0.0.3/check_yamlschema.egg-info/entry_points.txt
+-rw-r--r--   0 jmlrt      (501) staff       (20)       34 2023-07-25 12:04:50.000000 check-yamlschema-0.0.3/check_yamlschema.egg-info/requires.txt
+-rw-r--r--   0 jmlrt      (501) staff       (20)       17 2023-07-25 12:04:50.000000 check-yamlschema-0.0.3/check_yamlschema.egg-info/top_level.txt
+-rw-r--r--   0 jmlrt      (501) staff       (20)     2486 2023-07-25 10:31:52.000000 check-yamlschema-0.0.3/check_yamlschema.py
+-rw-r--r--   0 jmlrt      (501) staff       (20)      687 2023-07-25 12:04:50.844372 check-yamlschema-0.0.3/setup.cfg
+-rw-r--r--   0 jmlrt      (501) staff       (20)       74 2023-07-25 10:31:52.000000 check-yamlschema-0.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `check-yamlschema-0.0.2/LICENSE` & `check-yamlschema-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `check-yamlschema-0.0.2/PKG-INFO` & `check-yamlschema-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: check-yamlschema
-Version: 0.0.2
+Version: 0.0.3
 Summary: A CLI and pre-commit hooks for jsonschema validation in YAML files with multiple documents
 Home-page: https://github.com/jmlrt/check-yamlschema
 Author: Julien Mailleret
 Author-email: julien@mailleret.fr
 License: MIT
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # check-yamlschema
 
 A CLI and pre-commit hook for jsonschema validation in YAML files with multiple documents
 
@@ -55,13 +55,13 @@
 
 ## Pre-commit usage
 
 Add this to your `.pre-commit-config.yaml`:
 
 ```yaml
   - repo: https://github.com/jmlrt/check-yamlschema
-    rev: v0.0.1
+    rev: v0.0.2
     hooks:
       - id: check-yamlschema
 ```
 
 [inline schema comments]: https://github.com/redhat-developer/yaml-language-server/blob/762209ccdfca713d203ead757698a47ad3cabf50/README.md#using-inlined-schema
```

### Comparing `check-yamlschema-0.0.2/README.md` & `check-yamlschema-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -43,13 +43,13 @@
 
 ## Pre-commit usage
 
 Add this to your `.pre-commit-config.yaml`:
 
 ```yaml
   - repo: https://github.com/jmlrt/check-yamlschema
-    rev: v0.0.1
+    rev: v0.0.2
     hooks:
       - id: check-yamlschema
 ```
 
 [inline schema comments]: https://github.com/redhat-developer/yaml-language-server/blob/762209ccdfca713d203ead757698a47ad3cabf50/README.md#using-inlined-schema
```

### Comparing `check-yamlschema-0.0.2/check_yamlschema.egg-info/PKG-INFO` & `check-yamlschema-0.0.3/check_yamlschema.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: check-yamlschema
-Version: 0.0.2
+Version: 0.0.3
 Summary: A CLI and pre-commit hooks for jsonschema validation in YAML files with multiple documents
 Home-page: https://github.com/jmlrt/check-yamlschema
 Author: Julien Mailleret
 Author-email: julien@mailleret.fr
 License: MIT
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # check-yamlschema
 
 A CLI and pre-commit hook for jsonschema validation in YAML files with multiple documents
 
@@ -55,13 +55,13 @@
 
 ## Pre-commit usage
 
 Add this to your `.pre-commit-config.yaml`:
 
 ```yaml
   - repo: https://github.com/jmlrt/check-yamlschema
-    rev: v0.0.1
+    rev: v0.0.2
     hooks:
       - id: check-yamlschema
 ```
 
 [inline schema comments]: https://github.com/redhat-developer/yaml-language-server/blob/762209ccdfca713d203ead757698a47ad3cabf50/README.md#using-inlined-schema
```

### Comparing `check-yamlschema-0.0.2/check_yamlschema.py` & `check-yamlschema-0.0.3/check_yamlschema.py`

 * *Files identical despite different names*

### Comparing `check-yamlschema-0.0.2/setup.cfg` & `check-yamlschema-0.0.3/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [metadata]
 name = check-yamlschema
-version = 0.0.2
+version = 0.0.3
 description = A CLI and pre-commit hooks for jsonschema validation in YAML files with multiple documents
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jmlrt/check-yamlschema
 author = Julien Mailleret
 author_email = julien@mailleret.fr
 license = MIT
 license_files = 
 	LICENSE
 
 [options]
 py_modules = check_yamlschema
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
-	jsonschema
+	jsonschema<4.18.0
 	pyyaml
 	requests
 
 [options.entry_points]
 console_scripts = 
 	check-yamlschema=check_yamlschema:main
```

