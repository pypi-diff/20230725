# Comparing `tmp/git2net-1.7.0.tar.gz` & `tmp/git2net-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git2net-1.7.0.tar", last modified: Mon May  1 20:22:51 2023, max compression
+gzip compressed data, was "git2net-1.7.1.tar", last modified: Tue Jul 25 13:26:18 2023, max compression
```

## Comparing `git2net-1.7.0.tar` & `git2net-1.7.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:22:51.075456 git2net-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-01 20:22:40.000000 git2net-1.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-05-01 20:22:51.075456 git2net-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-05-01 20:22:40.000000 git2net-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:22:51.071455 git2net-1.7.0/git2net/
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-01 20:22:40.000000 git2net-1.7.0/git2net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13685 2023-05-01 20:22:40.000000 git2net-1.7.0/git2net/command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)    14331 2023-05-01 20:22:40.000000 git2net-1.7.0/git2net/complexity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-01 20:22:40.000000 git2net-1.7.0/git2net/disambiguation.py
--rw-r--r--   0 runner    (1001) docker     (123)    81636 2023-05-01 20:22:40.000000 git2net-1.7.0/git2net/extraction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:22:51.071455 git2net-1.7.0/git2net/helpers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:22:51.075456 git2net-1.7.0/git2net/helpers/binary-extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-01 20:22:40.000000 git2net-1.7.0/git2net/helpers/binary-extensions/binary-extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)    27015 2023-05-01 20:22:40.000000 git2net-1.7.0/git2net/visualisation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:22:51.075456 git2net-1.7.0/git2net.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-05-01 20:22:51.000000 git2net-1.7.0/git2net.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-01 20:22:51.000000 git2net-1.7.0/git2net.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 20:22:51.000000 git2net-1.7.0/git2net.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-01 20:22:51.000000 git2net-1.7.0/git2net.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-01 20:22:51.000000 git2net-1.7.0/git2net.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-01 20:22:51.000000 git2net-1.7.0/git2net.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-01 20:22:40.000000 git2net-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-01 20:22:51.075456 git2net-1.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:22:51.075456 git2net-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:22:40.000000 git2net-1.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35028 2023-05-01 20:22:40.000000 git2net-1.7.0/tests/test_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:26:18.590625 git2net-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-25 13:26:05.000000 git2net-1.7.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-07-25 13:26:18.590625 git2net-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-07-25 13:26:05.000000 git2net-1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:26:18.590625 git2net-1.7.1/git2net/
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-25 13:26:05.000000 git2net-1.7.1/git2net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13685 2023-07-25 13:26:05.000000 git2net-1.7.1/git2net/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14331 2023-07-25 13:26:05.000000 git2net-1.7.1/git2net/complexity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-25 13:26:05.000000 git2net-1.7.1/git2net/disambiguation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81636 2023-07-25 13:26:05.000000 git2net-1.7.1/git2net/extraction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:26:18.590625 git2net-1.7.1/git2net/helpers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:26:18.590625 git2net-1.7.1/git2net/helpers/binary-extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-25 13:26:05.000000 git2net-1.7.1/git2net/helpers/binary-extensions/binary-extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)    27015 2023-07-25 13:26:05.000000 git2net-1.7.1/git2net/visualisation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:26:18.590625 git2net-1.7.1/git2net.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-07-25 13:26:18.000000 git2net-1.7.1/git2net.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-25 13:26:18.000000 git2net-1.7.1/git2net.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 13:26:18.000000 git2net-1.7.1/git2net.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-25 13:26:18.000000 git2net-1.7.1/git2net.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-25 13:26:18.000000 git2net-1.7.1/git2net.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 13:26:18.000000 git2net-1.7.1/git2net.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-25 13:26:05.000000 git2net-1.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-25 13:26:18.594625 git2net-1.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:26:18.590625 git2net-1.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:26:05.000000 git2net-1.7.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35028 2023-07-25 13:26:05.000000 git2net-1.7.1/tests/test_functions.py
```

### Comparing `git2net-1.7.0/LICENSE.txt` & `git2net-1.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `git2net-1.7.0/PKG-INFO` & `git2net-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: git2net
-Version: 1.7.0
+Version: 1.7.1
 Summary: An OpenSource Python package for the extraction of fine-grained and time-stamped co-editing networks from git repositories.
 Home-page: https://gotec.github.io/git2net/
 Author: Christoph Gote
 Author-email: cgote@ethz.ch
 License: AGPL-3.0+
-Keywords: co-editing,networks,repository,mining,network,analysis
+Keywords: co-editing,network,repository,mining,network-analysis,git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![Tests](https://github.com/gotec/git2net/actions/workflows/python-app.yml/badge.svg)](https://github.com/gotec/git2net/actions/workflows/python-app.yml)
```

### Comparing `git2net-1.7.0/README.md` & `git2net-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `git2net-1.7.0/git2net/__init__.py` & `git2net-1.7.1/git2net/__init__.py`

 * *Files identical despite different names*

### Comparing `git2net-1.7.0/git2net/command_line.py` & `git2net-1.7.1/git2net/command_line.py`

 * *Files identical despite different names*

### Comparing `git2net-1.7.0/git2net/complexity.py` & `git2net-1.7.1/git2net/complexity.py`

 * *Files identical despite different names*

### Comparing `git2net-1.7.0/git2net/disambiguation.py` & `git2net-1.7.1/git2net/disambiguation.py`

 * *Files identical despite different names*

### Comparing `git2net-1.7.0/git2net/extraction.py` & `git2net-1.7.1/git2net/extraction.py`

 * *Files identical despite different names*

### Comparing `git2net-1.7.0/git2net/helpers/binary-extensions/binary-extensions.json` & `git2net-1.7.1/git2net/helpers/binary-extensions/binary-extensions.json`

 * *Files identical despite different names*

### Comparing `git2net-1.7.0/git2net/visualisation.py` & `git2net-1.7.1/git2net/visualisation.py`

 * *Files identical despite different names*

### Comparing `git2net-1.7.0/git2net.egg-info/PKG-INFO` & `git2net-1.7.1/git2net.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: git2net
-Version: 1.7.0
+Version: 1.7.1
 Summary: An OpenSource Python package for the extraction of fine-grained and time-stamped co-editing networks from git repositories.
 Home-page: https://gotec.github.io/git2net/
 Author: Christoph Gote
 Author-email: cgote@ethz.ch
 License: AGPL-3.0+
-Keywords: co-editing,networks,repository,mining,network,analysis
+Keywords: co-editing,network,repository,mining,network-analysis,git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![Tests](https://github.com/gotec/git2net/actions/workflows/python-app.yml/badge.svg)](https://github.com/gotec/git2net/actions/workflows/python-app.yml)
```

### Comparing `git2net-1.7.0/setup.cfg` & `git2net-1.7.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [metadata]
 name = git2net
-version = 1.7.0
+version = 1.7.1
 author = Christoph Gote
 author_email = cgote@ethz.ch
 license = AGPL-3.0+
 description = An OpenSource Python package for the extraction of fine-grained and time-stamped co-editing networks from git repositories.
 keywords = 
 	co-editing
-	networks
+	network
 	repository
 	mining
-	network
-	analysis
+	network-analysis
+	git
 url = https://gotec.github.io/git2net/
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 	Operating System :: OS Independent
@@ -30,14 +30,15 @@
 	python-levenshtein
 	pathpy2>=2.2.0
 	lizard
 	pydriller>=2.0.0,<2.2.0
 	gambit-disambig
 	setuptools
 	pygments
+	networkx
 
 [options.entry_points]
 console_scripts = git2net = git2net.command_line:main
 
 [options.package_data]
 git2net = 
 	helpers/binary-extensions/binary-extensions.json
```

### Comparing `git2net-1.7.0/tests/test_functions.py` & `git2net-1.7.1/tests/test_functions.py`

 * *Files identical despite different names*

