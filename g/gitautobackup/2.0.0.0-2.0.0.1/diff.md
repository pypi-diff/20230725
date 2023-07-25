# Comparing `tmp/gitautobackup-2.0.0.0.tar.gz` & `tmp/gitautobackup-2.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitautobackup-2.0.0.0.tar", last modified: Tue Jul 25 18:19:23 2023, max compression
+gzip compressed data, was "gitautobackup-2.0.0.1.tar", last modified: Tue Jul 25 18:26:25 2023, max compression
```

## Comparing `gitautobackup-2.0.0.0.tar` & `gitautobackup-2.0.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 18:19:23.570771 gitautobackup-2.0.0.0/
--rw-rw-rw-   0        0        0    17098 2023-05-30 17:53:38.000000 gitautobackup-2.0.0.0/LICENSE
--rw-rw-rw-   0        0        0    46206 2023-07-25 18:19:23.557191 gitautobackup-2.0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     7453 2023-07-25 00:17:20.000000 gitautobackup-2.0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 18:19:23.542429 gitautobackup-2.0.0.0/gitautobackup.egg-info/
--rw-rw-rw-   0        0        0    46206 2023-07-25 18:19:23.000000 gitautobackup-2.0.0.0/gitautobackup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-07-25 18:19:23.000000 gitautobackup-2.0.0.0/gitautobackup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 18:19:23.000000 gitautobackup-2.0.0.0/gitautobackup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2023-07-25 18:19:23.000000 gitautobackup-2.0.0.0/gitautobackup.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      151 2023-07-25 18:19:23.000000 gitautobackup-2.0.0.0/gitautobackup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-25 18:19:23.000000 gitautobackup-2.0.0.0/gitautobackup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-07-25 18:19:21.000000 gitautobackup-2.0.0.0/gitautobackup.egg-info/zip-safe
--rw-rw-rw-   0        0        0    31039 2023-07-25 11:21:52.000000 gitautobackup-2.0.0.0/gitautobackup.py
--rw-rw-rw-   0        0        0     3160 2023-07-25 00:26:17.000000 gitautobackup-2.0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-25 18:19:23.570771 gitautobackup-2.0.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-25 18:26:25.161522 gitautobackup-2.0.0.1/
+-rw-rw-rw-   0        0        0    17098 2023-05-30 17:53:38.000000 gitautobackup-2.0.0.1/LICENSE
+-rw-rw-rw-   0        0        0    46205 2023-07-25 18:26:25.156910 gitautobackup-2.0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7453 2023-07-25 00:17:20.000000 gitautobackup-2.0.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 18:26:25.147274 gitautobackup-2.0.0.1/gitautobackup.egg-info/
+-rw-rw-rw-   0        0        0    46205 2023-07-25 18:26:24.000000 gitautobackup-2.0.0.1/gitautobackup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2023-07-25 18:26:25.000000 gitautobackup-2.0.0.1/gitautobackup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 18:26:24.000000 gitautobackup-2.0.0.1/gitautobackup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-07-25 18:26:24.000000 gitautobackup-2.0.0.1/gitautobackup.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      151 2023-07-25 18:26:24.000000 gitautobackup-2.0.0.1/gitautobackup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-25 18:26:24.000000 gitautobackup-2.0.0.1/gitautobackup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-25 18:26:23.000000 gitautobackup-2.0.0.1/gitautobackup.egg-info/zip-safe
+-rw-rw-rw-   0        0        0    31039 2023-07-25 18:25:53.000000 gitautobackup-2.0.0.1/gitautobackup.py
+-rw-rw-rw-   0        0        0     3159 2023-07-25 18:22:40.000000 gitautobackup-2.0.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-25 18:26:25.161522 gitautobackup-2.0.0.1/setup.cfg
```

### Comparing `gitautobackup-2.0.0.0/LICENSE` & `gitautobackup-2.0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gitautobackup-2.0.0.0/PKG-INFO` & `gitautobackup-2.0.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gitautobackup
-Version: 2.0.0.0
-Summary: A basic CLI program and python moldule that allows for quickly making and comming changes to a git repository, along with a few other tools
+Version: 2.0.0.1
+Summary: A basic CLI program and python module that allows for quickly making and comming changes to a git repository, along with a few other tools
 Author-email: Markus Hammer <107761433+MarkusHammer@users.noreply.github.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
```

### Comparing `gitautobackup-2.0.0.0/README.md` & `gitautobackup-2.0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `gitautobackup-2.0.0.0/gitautobackup.egg-info/PKG-INFO` & `gitautobackup-2.0.0.1/gitautobackup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gitautobackup
-Version: 2.0.0.0
-Summary: A basic CLI program and python moldule that allows for quickly making and comming changes to a git repository, along with a few other tools
+Version: 2.0.0.1
+Summary: A basic CLI program and python module that allows for quickly making and comming changes to a git repository, along with a few other tools
 Author-email: Markus Hammer <107761433+MarkusHammer@users.noreply.github.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
```

### Comparing `gitautobackup-2.0.0.0/gitautobackup.py` & `gitautobackup-2.0.0.1/gitautobackup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     See the github repo for more info!
     
     This project is on github here:
     https://github.com/MarkusHammer/gitautobackup
 '''
 
-__version__ = "2.0.0.0"
+__version__ = "2.0.0.1"
 
 from git import Repo, InvalidGitRepositoryError, GitCommandNotFound, NoSuchPathError, RepositoryDirtyError, GitError
 
 try:
     from pathlib import Path
 except ImportError:
     from pathlib2 import Path
```

### Comparing `gitautobackup-2.0.0.0/pyproject.toml` & `gitautobackup-2.0.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #THX https://packaging.python.org/en/latest/specifications/declaring-project-metadata/#entry-points
 #THX https://pypi.org/project/validate-pyproject/
 
 [project]
     dynamic = ["version", "readme"]
     name = "gitautobackup"
     #fullname = "Git Auto Backup Tool"
-    description = "A basic CLI program and python moldule that allows for quickly making and comming changes to a git repository, along with a few other tools"
+    description = "A basic CLI program and python module that allows for quickly making and comming changes to a git repository, along with a few other tools"
     authors = [{ name = "Markus Hammer", email = "107761433+MarkusHammer@users.noreply.github.com" }]
     license = { file = "LICENSE" }
     dependencies = ["pathlib", "GitPython", "typing-extensions;python_version<'3.8'"]
     requires-python = ">=3.0"
     classifiers = [
         "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
         "Development Status :: 5 - Production/Stable",
```

