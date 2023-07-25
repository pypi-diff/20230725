# Comparing `tmp/pulumi_mysql-3.2.0a1689313722.tar.gz` & `tmp/pulumi_mysql-3.2.0a1690263584.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_mysql-3.2.0a1689313722.tar", last modified: Fri Jul 14 05:59:53 2023, max compression
+gzip compressed data, was "pulumi_mysql-3.2.0a1690263584.tar", last modified: Tue Jul 25 05:45:35 2023, max compression
```

## Comparing `pulumi_mysql-3.2.0a1689313722.tar` & `pulumi_mysql-3.2.0a1690263584.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:59:53.182890 pulumi_mysql-3.2.0a1689313722/
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-07-14 05:59:53.182890 pulumi_mysql-3.2.0a1689313722/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-14 05:59:51.000000 pulumi_mysql-3.2.0a1689313722/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:59:53.182890 pulumi_mysql-3.2.0a1689313722/pulumi_mysql/
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-14 05:59:51.000000 pulumi_mysql-3.2.0a1689313722/pulumi_mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-14 05:59:51.000000 pulumi_mysql-3.2.0a1689313722/pulumi_mysql/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:59:53.182890 pulumi_mysql-3.2.0a1689313722/pulumi_mysql/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-14 05:59:51.000000 pulumi_mysql-3.2.0a1689313722/pulumi_mysql/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-14 05:59:51.000000 pulumi_mysql-3.2.0a1689313722/pulumi_mysql/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    14104 2023-07-14 05:59:51.000000 pulumi_mysql-3.2.0a1689313722/pulumi_mysql/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    26896 2023-07-14 05:59:51.000000 pulumi_mysql-3.2.0a1689313722/pulumi_mysql/grant.py
--rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-07-14 05:59:51.000000 pulumi_mysql-3.2.0a1689313722/pulumi_mysql/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-14 05:59:51.000000 pulumi_mysql-3.2.0a1689313722/pulumi_mysql/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:59:51.000000 pulumi_mysql-3.2.0a1689313722/pulumi_mysql/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-14 05:59:51.000000 pulumi_mysql-3.2.0a1689313722/pulumi_mysql/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    22471 2023-07-14 05:59:51.000000 pulumi_mysql-3.2.0a1689313722/pulumi_mysql/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12922 2023-07-14 05:59:51.000000 pulumi_mysql-3.2.0a1689313722/pulumi_mysql/user_password.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:59:53.182890 pulumi_mysql-3.2.0a1689313722/pulumi_mysql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-07-14 05:59:53.000000 pulumi_mysql-3.2.0a1689313722/pulumi_mysql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-14 05:59:53.000000 pulumi_mysql-3.2.0a1689313722/pulumi_mysql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 05:59:53.000000 pulumi_mysql-3.2.0a1689313722/pulumi_mysql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 05:59:53.000000 pulumi_mysql-3.2.0a1689313722/pulumi_mysql.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-14 05:59:53.000000 pulumi_mysql-3.2.0a1689313722/pulumi_mysql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-14 05:59:53.000000 pulumi_mysql-3.2.0a1689313722/pulumi_mysql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 05:59:53.182890 pulumi_mysql-3.2.0a1689313722/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-14 05:59:52.000000 pulumi_mysql-3.2.0a1689313722/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:45:35.836769 pulumi_mysql-3.2.0a1690263584/
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-07-25 05:45:35.836769 pulumi_mysql-3.2.0a1690263584/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-25 05:45:35.000000 pulumi_mysql-3.2.0a1690263584/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:45:35.836769 pulumi_mysql-3.2.0a1690263584/pulumi_mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-25 05:45:35.000000 pulumi_mysql-3.2.0a1690263584/pulumi_mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-25 05:45:35.000000 pulumi_mysql-3.2.0a1690263584/pulumi_mysql/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:45:35.836769 pulumi_mysql-3.2.0a1690263584/pulumi_mysql/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-25 05:45:35.000000 pulumi_mysql-3.2.0a1690263584/pulumi_mysql/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-25 05:45:35.000000 pulumi_mysql-3.2.0a1690263584/pulumi_mysql/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14104 2023-07-25 05:45:35.000000 pulumi_mysql-3.2.0a1690263584/pulumi_mysql/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26896 2023-07-25 05:45:35.000000 pulumi_mysql-3.2.0a1690263584/pulumi_mysql/grant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-07-25 05:45:35.000000 pulumi_mysql-3.2.0a1690263584/pulumi_mysql/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-25 05:45:35.000000 pulumi_mysql-3.2.0a1690263584/pulumi_mysql/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 05:45:35.000000 pulumi_mysql-3.2.0a1690263584/pulumi_mysql/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-25 05:45:35.000000 pulumi_mysql-3.2.0a1690263584/pulumi_mysql/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22471 2023-07-25 05:45:35.000000 pulumi_mysql-3.2.0a1690263584/pulumi_mysql/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12922 2023-07-25 05:45:35.000000 pulumi_mysql-3.2.0a1690263584/pulumi_mysql/user_password.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:45:35.836769 pulumi_mysql-3.2.0a1690263584/pulumi_mysql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-07-25 05:45:35.000000 pulumi_mysql-3.2.0a1690263584/pulumi_mysql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-25 05:45:35.000000 pulumi_mysql-3.2.0a1690263584/pulumi_mysql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 05:45:35.000000 pulumi_mysql-3.2.0a1690263584/pulumi_mysql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 05:45:35.000000 pulumi_mysql-3.2.0a1690263584/pulumi_mysql.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-25 05:45:35.000000 pulumi_mysql-3.2.0a1690263584/pulumi_mysql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 05:45:35.000000 pulumi_mysql-3.2.0a1690263584/pulumi_mysql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 05:45:35.836769 pulumi_mysql-3.2.0a1690263584/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-25 05:45:35.000000 pulumi_mysql-3.2.0a1690263584/setup.py
```

### Comparing `pulumi_mysql-3.2.0a1689313722/PKG-INFO` & `pulumi_mysql-3.2.0a1690263584/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_mysql
-Version: 3.2.0a1689313722
+Version: 3.2.0a1690263584
 Summary: A Pulumi package for creating and managing mysql cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-mysql
 Keywords: pulumi mysql
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_mysql-3.2.0a1689313722/README.md` & `pulumi_mysql-3.2.0a1690263584/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1689313722/pulumi_mysql/__init__.py` & `pulumi_mysql-3.2.0a1690263584/pulumi_mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1689313722/pulumi_mysql/_utilities.py` & `pulumi_mysql-3.2.0a1690263584/pulumi_mysql/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1689313722/pulumi_mysql/config/vars.py` & `pulumi_mysql-3.2.0a1690263584/pulumi_mysql/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1689313722/pulumi_mysql/database.py` & `pulumi_mysql-3.2.0a1690263584/pulumi_mysql/database.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1689313722/pulumi_mysql/grant.py` & `pulumi_mysql-3.2.0a1690263584/pulumi_mysql/grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1689313722/pulumi_mysql/provider.py` & `pulumi_mysql-3.2.0a1690263584/pulumi_mysql/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1689313722/pulumi_mysql/role.py` & `pulumi_mysql-3.2.0a1690263584/pulumi_mysql/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1689313722/pulumi_mysql/user.py` & `pulumi_mysql-3.2.0a1690263584/pulumi_mysql/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1689313722/pulumi_mysql/user_password.py` & `pulumi_mysql-3.2.0a1690263584/pulumi_mysql/user_password.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1689313722/pulumi_mysql.egg-info/PKG-INFO` & `pulumi_mysql-3.2.0a1690263584/pulumi_mysql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-mysql
-Version: 3.2.0a1689313722
+Version: 3.2.0a1690263584
 Summary: A Pulumi package for creating and managing mysql cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-mysql
 Keywords: pulumi mysql
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_mysql-3.2.0a1689313722/pulumi_mysql.egg-info/SOURCES.txt` & `pulumi_mysql-3.2.0a1690263584/pulumi_mysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1689313722/setup.py` & `pulumi_mysql-3.2.0a1690263584/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.2.0a1689313722"
-PLUGIN_VERSION = "3.2.0-alpha.1689313722+f6d9b4b3"
+VERSION = "3.2.0a1690263584"
+PLUGIN_VERSION = "3.2.0-alpha.1690263584+e67bdcc2"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'mysql', PLUGIN_VERSION])
         except OSError as error:
```

