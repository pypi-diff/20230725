# Comparing `tmp/mail_alias_creator-1.1.0.tar.gz` & `tmp/mail_alias_creator-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mail_alias_creator-1.1.0.tar", last modified: Fri Apr 16 20:56:34 2021, max compression
+gzip compressed data, was "mail_alias_creator-1.1.1.tar", max compression
```

## Comparing `mail_alias_creator-1.1.0.tar` & `mail_alias_creator-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1063 2021-01-29 20:51:25.348848 mail_alias_creator-1.1.0/LICENSE
--rw-r--r--   0        0        0     4420 2021-04-16 20:47:37.847909 mail_alias_creator-1.1.0/README.md
--rw-r--r--   0        0        0      126 2021-01-29 20:51:25.349848 mail_alias_creator-1.1.0/mail_alias_creator/__init__.py
--rw-r--r--   0        0        0        0 2021-01-29 20:51:25.349848 mail_alias_creator-1.1.0/mail_alias_creator/entry_processors/__init__.py
--rw-r--r--   0        0        0     3506 2021-04-16 20:47:37.848909 mail_alias_creator-1.1.0/mail_alias_creator/entry_processors/base.py
--rw-r--r--   0        0        0     1001 2021-04-16 20:47:37.848909 mail_alias_creator-1.1.0/mail_alias_creator/entry_processors/external_address.py
--rw-r--r--   0        0        0     1462 2021-04-16 20:47:37.849909 mail_alias_creator-1.1.0/mail_alias_creator/entry_processors/group.py
--rw-r--r--   0        0        0     1437 2021-04-16 20:47:37.849909 mail_alias_creator-1.1.0/mail_alias_creator/entry_processors/include_alias.py
--rw-r--r--   0        0        0     1242 2021-04-16 20:47:37.850909 mail_alias_creator-1.1.0/mail_alias_creator/entry_processors/user.py
--rw-r--r--   0        0        0      669 2021-01-29 20:51:25.350848 mail_alias_creator-1.1.0/mail_alias_creator/interface.py
--rw-r--r--   0        0        0     7329 2021-01-29 20:51:25.350848 mail_alias_creator-1.1.0/mail_alias_creator/ldap.py
--rw-r--r--   0        0        0     2618 2021-01-29 21:25:31.719617 mail_alias_creator-1.1.0/mail_alias_creator/main.py
--rw-r--r--   0        0        0     6372 2021-01-29 20:51:25.350848 mail_alias_creator-1.1.0/mail_alias_creator/process.py
--rw-r--r--   0        0        0      747 2021-04-16 20:47:37.850909 mail_alias_creator-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     5483 2021-04-16 20:56:34.887716 mail_alias_creator-1.1.0/setup.py
--rw-r--r--   0        0        0     5175 2021-04-16 20:56:34.888552 mail_alias_creator-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2021-01-29 20:51:25.348848 mail_alias_creator-1.1.1/LICENSE
+-rw-r--r--   0        0        0     4420 2021-04-16 20:47:37.847909 mail_alias_creator-1.1.1/README.md
+-rw-r--r--   0        0        0      126 2021-01-29 20:51:25.349848 mail_alias_creator-1.1.1/mail_alias_creator/__init__.py
+-rw-r--r--   0        0        0        0 2021-01-29 20:51:25.349848 mail_alias_creator-1.1.1/mail_alias_creator/entry_processors/__init__.py
+-rw-r--r--   0        0        0     3506 2021-04-16 20:47:37.848909 mail_alias_creator-1.1.1/mail_alias_creator/entry_processors/base.py
+-rw-r--r--   0        0        0     1001 2021-04-16 20:47:37.848909 mail_alias_creator-1.1.1/mail_alias_creator/entry_processors/external_address.py
+-rw-r--r--   0        0        0     1462 2021-04-16 20:47:37.849909 mail_alias_creator-1.1.1/mail_alias_creator/entry_processors/group.py
+-rw-r--r--   0        0        0     1437 2021-04-16 20:47:37.849909 mail_alias_creator-1.1.1/mail_alias_creator/entry_processors/include_alias.py
+-rw-r--r--   0        0        0     1242 2021-04-16 20:47:37.850909 mail_alias_creator-1.1.1/mail_alias_creator/entry_processors/user.py
+-rw-r--r--   0        0        0      669 2021-01-29 20:51:25.350848 mail_alias_creator-1.1.1/mail_alias_creator/interface.py
+-rw-r--r--   0        0        0     7329 2021-01-29 20:51:25.350848 mail_alias_creator-1.1.1/mail_alias_creator/ldap.py
+-rw-r--r--   0        0        0     2618 2021-01-29 21:25:31.719617 mail_alias_creator-1.1.1/mail_alias_creator/main.py
+-rw-r--r--   0        0        0     6372 2021-01-29 20:51:25.350848 mail_alias_creator-1.1.1/mail_alias_creator/process.py
+-rw-r--r--   0        0        0      747 2023-07-25 19:41:49.442810 mail_alias_creator-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5327 1970-01-01 00:00:00.000000 mail_alias_creator-1.1.1/PKG-INFO
```

### Comparing `mail_alias_creator-1.1.0/LICENSE` & `mail_alias_creator-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mail_alias_creator-1.1.0/README.md` & `mail_alias_creator-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mail_alias_creator-1.1.0/mail_alias_creator/entry_processors/base.py` & `mail_alias_creator-1.1.1/mail_alias_creator/entry_processors/base.py`

 * *Files identical despite different names*

### Comparing `mail_alias_creator-1.1.0/mail_alias_creator/entry_processors/external_address.py` & `mail_alias_creator-1.1.1/mail_alias_creator/entry_processors/external_address.py`

 * *Files identical despite different names*

### Comparing `mail_alias_creator-1.1.0/mail_alias_creator/entry_processors/group.py` & `mail_alias_creator-1.1.1/mail_alias_creator/entry_processors/group.py`

 * *Files identical despite different names*

### Comparing `mail_alias_creator-1.1.0/mail_alias_creator/entry_processors/include_alias.py` & `mail_alias_creator-1.1.1/mail_alias_creator/entry_processors/include_alias.py`

 * *Files identical despite different names*

### Comparing `mail_alias_creator-1.1.0/mail_alias_creator/entry_processors/user.py` & `mail_alias_creator-1.1.1/mail_alias_creator/entry_processors/user.py`

 * *Files identical despite different names*

### Comparing `mail_alias_creator-1.1.0/mail_alias_creator/interface.py` & `mail_alias_creator-1.1.1/mail_alias_creator/interface.py`

 * *Files identical despite different names*

### Comparing `mail_alias_creator-1.1.0/mail_alias_creator/ldap.py` & `mail_alias_creator-1.1.1/mail_alias_creator/ldap.py`

 * *Files identical despite different names*

### Comparing `mail_alias_creator-1.1.0/mail_alias_creator/main.py` & `mail_alias_creator-1.1.1/mail_alias_creator/main.py`

 * *Files identical despite different names*

### Comparing `mail_alias_creator-1.1.0/mail_alias_creator/process.py` & `mail_alias_creator-1.1.1/mail_alias_creator/process.py`

 * *Files identical despite different names*

### Comparing `mail_alias_creator-1.1.0/pyproject.toml` & `mail_alias_creator-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "mail_alias_creator"
-version = "1.1.0"
+version = "1.1.1"
 description = "Set of python scripts to create our mail alias tables from alias definitions"
 repository = "https://github.com/stuvusIT/mail_alias_creator"
 readme = "README.md"
 authors = ["Tim Neumann <neumantm@fius.informatik.uni-stuttgart.de>"]
 license = "MIT"
 
 [tool.poetry.scripts]
 mail_alias_creator = 'mail_alias_creator.main:main'
 
 [tool.poetry.dependencies]
 python = "^3.6"
 ldap3 = "^2.7"
-pyyaml = "^5.2"
+pyyaml = "^6.0"
 
 [tool.poetry.dev-dependencies]
 black = "^20.8b1"
 flake8 = "^3.8.4"
 pytest = "^6.1.1"
 flake8-docstrings = "^1.5.0"
 flake8-bugbear = "^20.1.4"
```

### Comparing `mail_alias_creator-1.1.0/PKG-INFO` & `mail_alias_creator-1.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: mail-alias-creator
-Version: 1.1.0
+Version: 1.1.1
 Summary: Set of python scripts to create our mail alias tables from alias definitions
 Home-page: https://github.com/stuvusIT/mail_alias_creator
 License: MIT
 Author: Tim Neumann
 Author-email: neumantm@fius.informatik.uni-stuttgart.de
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ldap3 (>=2.7,<3.0)
-Requires-Dist: pyyaml (>=5.2,<6.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
 Project-URL: Repository, https://github.com/stuvusIT/mail_alias_creator
 Description-Content-Type: text/markdown
 
 # mail_alias_creator
 A python program to create our mail alias tables from alias definitions
 
 ## Configuration
```

