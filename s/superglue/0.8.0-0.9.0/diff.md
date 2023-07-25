# Comparing `tmp/superglue-0.8.0.tar.gz` & `tmp/superglue-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superglue-0.8.0.tar", last modified: Fri Jan  6 14:03:49 2023, max compression
+gzip compressed data, was "superglue-0.9.0.tar", last modified: Fri Jan  6 14:37:21 2023, max compression
```

## Comparing `superglue-0.8.0.tar` & `superglue-0.9.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:03:49.753365 superglue-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-01-06 14:03:16.000000 superglue-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-01-06 14:03:49.753365 superglue-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-01-06 14:03:47.000000 superglue-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-01-06 14:03:47.000000 superglue-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-06 14:03:49.753365 superglue-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-01-06 14:03:16.000000 superglue-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:03:49.749365 superglue-0.8.0/superglue/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 14:03:16.000000 superglue-0.8.0/superglue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-01-06 14:03:16.000000 superglue-0.8.0/superglue/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:03:49.753365 superglue-0.8.0/superglue/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-01-06 14:03:16.000000 superglue-0.8.0/superglue/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-01-06 14:03:16.000000 superglue-0.8.0/superglue/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-01-06 14:03:47.000000 superglue-0.8.0/superglue/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-01-06 14:03:16.000000 superglue-0.8.0/superglue/cli/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-01-06 14:03:16.000000 superglue-0.8.0/superglue/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-01-06 14:03:16.000000 superglue-0.8.0/superglue/cli/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:03:49.749365 superglue-0.8.0/superglue/core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:03:49.753365 superglue-0.8.0/superglue/core/components/
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-01-06 14:03:16.000000 superglue-0.8.0/superglue/core/components/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-01-06 14:03:16.000000 superglue-0.8.0/superglue/core/components/component_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-01-06 14:03:16.000000 superglue-0.8.0/superglue/core/components/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-01-06 14:03:16.000000 superglue-0.8.0/superglue/core/components/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-01-06 14:03:16.000000 superglue-0.8.0/superglue/core/components/makefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-01-06 14:03:16.000000 superglue-0.8.0/superglue/core/components/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-01-06 14:03:16.000000 superglue-0.8.0/superglue/core/components/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-01-06 14:03:16.000000 superglue-0.8.0/superglue/core/components/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:03:49.753365 superglue-0.8.0/superglue/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-01-06 14:03:16.000000 superglue-0.8.0/superglue/environment/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-01-06 14:03:16.000000 superglue-0.8.0/superglue/environment/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:03:49.753365 superglue-0.8.0/superglue/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 14:03:16.000000 superglue-0.8.0/superglue/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-01-06 14:03:16.000000 superglue-0.8.0/superglue/templates/conftest.template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-01-06 14:03:16.000000 superglue-0.8.0/superglue/templates/job_config.template.yml
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-01-06 14:03:16.000000 superglue-0.8.0/superglue/templates/job_test.template.py.txt
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-01-06 14:03:16.000000 superglue-0.8.0/superglue/templates/main.template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-01-06 14:03:16.000000 superglue-0.8.0/superglue/templates/makefile
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-01-06 14:03:16.000000 superglue-0.8.0/superglue/templates/module_test.template.py.txt
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-01-06 14:03:16.000000 superglue-0.8.0/superglue/templates/template.env
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-01-06 14:03:16.000000 superglue-0.8.0/superglue/templates/template.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:03:49.749365 superglue-0.8.0/superglue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-01-06 14:03:49.000000 superglue-0.8.0/superglue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-01-06 14:03:49.000000 superglue-0.8.0/superglue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 14:03:49.000000 superglue-0.8.0/superglue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-06 14:03:49.000000 superglue-0.8.0/superglue.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-01-06 14:03:49.000000 superglue-0.8.0/superglue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-06 14:03:49.000000 superglue-0.8.0/superglue.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:37:21.916372 superglue-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-01-06 14:36:49.000000 superglue-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-01-06 14:37:21.916372 superglue-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-01-06 14:37:20.000000 superglue-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-01-06 14:37:20.000000 superglue-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-06 14:37:21.916372 superglue-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-01-06 14:36:49.000000 superglue-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:37:21.912372 superglue-0.9.0/superglue/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 14:36:49.000000 superglue-0.9.0/superglue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-01-06 14:36:49.000000 superglue-0.9.0/superglue/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:37:21.916372 superglue-0.9.0/superglue/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-01-06 14:36:49.000000 superglue-0.9.0/superglue/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-01-06 14:36:49.000000 superglue-0.9.0/superglue/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-01-06 14:37:20.000000 superglue-0.9.0/superglue/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-01-06 14:36:49.000000 superglue-0.9.0/superglue/cli/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-01-06 14:36:49.000000 superglue-0.9.0/superglue/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-01-06 14:36:49.000000 superglue-0.9.0/superglue/cli/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:37:21.912372 superglue-0.9.0/superglue/core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:37:21.916372 superglue-0.9.0/superglue/core/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-01-06 14:36:49.000000 superglue-0.9.0/superglue/core/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-01-06 14:36:49.000000 superglue-0.9.0/superglue/core/components/component_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-01-06 14:36:49.000000 superglue-0.9.0/superglue/core/components/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-01-06 14:36:49.000000 superglue-0.9.0/superglue/core/components/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-01-06 14:36:49.000000 superglue-0.9.0/superglue/core/components/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-01-06 14:36:49.000000 superglue-0.9.0/superglue/core/components/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-01-06 14:36:49.000000 superglue-0.9.0/superglue/core/components/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-01-06 14:36:49.000000 superglue-0.9.0/superglue/core/components/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:37:21.916372 superglue-0.9.0/superglue/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-01-06 14:36:49.000000 superglue-0.9.0/superglue/environment/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-01-06 14:36:49.000000 superglue-0.9.0/superglue/environment/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:37:21.916372 superglue-0.9.0/superglue/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 14:36:49.000000 superglue-0.9.0/superglue/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-01-06 14:36:49.000000 superglue-0.9.0/superglue/templates/conftest.template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-01-06 14:36:49.000000 superglue-0.9.0/superglue/templates/job_config.template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-01-06 14:36:49.000000 superglue-0.9.0/superglue/templates/job_test.template.py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-01-06 14:36:49.000000 superglue-0.9.0/superglue/templates/main.template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-01-06 14:36:49.000000 superglue-0.9.0/superglue/templates/makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-01-06 14:36:49.000000 superglue-0.9.0/superglue/templates/module_test.template.py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-01-06 14:36:49.000000 superglue-0.9.0/superglue/templates/template.env
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-01-06 14:36:49.000000 superglue-0.9.0/superglue/templates/template.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 14:37:21.912372 superglue-0.9.0/superglue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-01-06 14:37:21.000000 superglue-0.9.0/superglue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-01-06 14:37:21.000000 superglue-0.9.0/superglue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 14:37:21.000000 superglue-0.9.0/superglue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-06 14:37:21.000000 superglue-0.9.0/superglue.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-01-06 14:37:21.000000 superglue-0.9.0/superglue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-06 14:37:21.000000 superglue-0.9.0/superglue.egg-info/top_level.txt
```

### Comparing `superglue-0.8.0/PKG-INFO` & `superglue-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: superglue
-Version: 0.8.0
+Version: 0.9.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # Superglue
 ## A CLI tool for developing, testing and deploying AWS glue jobs
-### VERSION 0.8.0
+### VERSION 0.9.0
 
 Superglue makes the development, troubleshooting and deployment of AWS glue jobs simple. It also makes creating a shared 
 glue codebase easy and testable
 
 
 # Getting Started
 ```
```

### Comparing `superglue-0.8.0/README.md` & `superglue-0.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Superglue
 ## A CLI tool for developing, testing and deploying AWS glue jobs
-### VERSION 0.8.0
+### VERSION 0.9.0
 
 Superglue makes the development, troubleshooting and deployment of AWS glue jobs simple. It also makes creating a shared 
 glue codebase easy and testable
 
 
 # Getting Started
 ```
```

### Comparing `superglue-0.8.0/pyproject.toml` & `superglue-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "superglue"
-version = "0.8.0"
+version = "0.9.0"
 description = ""
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
 	"python-dotenv==0.20.0",
 	"pyaml==21.10.1",
 	"boto3==1.20.49",
```

### Comparing `superglue-0.8.0/superglue/cli/__init__.py` & `superglue-0.9.0/superglue/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `superglue-0.8.0/superglue/cli/base.py` & `superglue-0.9.0/superglue/cli/base.py`

 * *Files identical despite different names*

### Comparing `superglue-0.8.0/superglue/cli/commands.py` & `superglue-0.9.0/superglue/cli/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from superglue.cli.utils import validate_account
 from superglue.cli.base import BaseSuperglueCommand
 from superglue.cli.messages import Messages
 
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 
 class Version(BaseSuperglueCommand):
 
     help = "--> Print the current version of superglue and exit."
 
     def __call__(self) -> None:
```

### Comparing `superglue-0.8.0/superglue/cli/messages.py` & `superglue-0.9.0/superglue/cli/messages.py`

 * *Files identical despite different names*

### Comparing `superglue-0.8.0/superglue/cli/utils.py` & `superglue-0.9.0/superglue/cli/utils.py`

 * *Files identical despite different names*

### Comparing `superglue-0.8.0/superglue/cli/validation.py` & `superglue-0.9.0/superglue/cli/validation.py`

 * *Files identical despite different names*

### Comparing `superglue-0.8.0/superglue/core/components/base.py` & `superglue-0.9.0/superglue/core/components/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         try:
             with BytesIO() as buffer:
                 s3_client.download_fileobj(self.bucket, self.s3_version_path, buffer)
                 buffer.seek(0)
                 return json.load(buffer)
         except botocore.exceptions.ClientError as e:
             code = e.args[0].partition(":")[2].strip()
-            if code == "Not Found":
+            if code in ["Not Found", "Forbidden"]:
                 return {}
             raise e
 
     def lock(self) -> None:
         self.increment_version()
         self.save_version_file()
```

### Comparing `superglue-0.8.0/superglue/core/components/component_list.py` & `superglue-0.9.0/superglue/core/components/component_list.py`

 * *Files identical despite different names*

### Comparing `superglue-0.8.0/superglue/core/components/files.py` & `superglue-0.9.0/superglue/core/components/files.py`

 * *Files identical despite different names*

### Comparing `superglue-0.8.0/superglue/core/components/job.py` & `superglue-0.9.0/superglue/core/components/job.py`

 * *Files identical despite different names*

### Comparing `superglue-0.8.0/superglue/core/components/makefile.py` & `superglue-0.9.0/superglue/core/components/makefile.py`

 * *Files identical despite different names*

### Comparing `superglue-0.8.0/superglue/core/components/module.py` & `superglue-0.9.0/superglue/core/components/module.py`

 * *Files identical despite different names*

### Comparing `superglue-0.8.0/superglue/core/components/project.py` & `superglue-0.9.0/superglue/core/components/project.py`

 * *Files identical despite different names*

### Comparing `superglue-0.8.0/superglue/core/components/tests.py` & `superglue-0.9.0/superglue/core/components/tests.py`

 * *Files identical despite different names*

### Comparing `superglue-0.8.0/superglue/environment/variables.py` & `superglue-0.9.0/superglue/environment/variables.py`

 * *Files identical despite different names*

### Comparing `superglue-0.8.0/superglue/templates/job_config.template.yml` & `superglue-0.9.0/superglue/templates/job_config.template.yml`

 * *Files identical despite different names*

### Comparing `superglue-0.8.0/superglue/templates/main.template.py` & `superglue-0.9.0/superglue/templates/main.template.py`

 * *Files identical despite different names*

### Comparing `superglue-0.8.0/superglue/templates/makefile` & `superglue-0.9.0/superglue/templates/makefile`

 * *Files identical despite different names*

### Comparing `superglue-0.8.0/superglue/templates/template.gitignore` & `superglue-0.9.0/superglue/templates/template.gitignore`

 * *Files identical despite different names*

### Comparing `superglue-0.8.0/superglue.egg-info/PKG-INFO` & `superglue-0.9.0/superglue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: superglue
-Version: 0.8.0
+Version: 0.9.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # Superglue
 ## A CLI tool for developing, testing and deploying AWS glue jobs
-### VERSION 0.8.0
+### VERSION 0.9.0
 
 Superglue makes the development, troubleshooting and deployment of AWS glue jobs simple. It also makes creating a shared 
 glue codebase easy and testable
 
 
 # Getting Started
 ```
```

### Comparing `superglue-0.8.0/superglue.egg-info/SOURCES.txt` & `superglue-0.9.0/superglue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

