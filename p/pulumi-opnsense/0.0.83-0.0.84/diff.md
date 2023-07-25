# Comparing `tmp/pulumi_opnsense-0.0.83.tar.gz` & `tmp/pulumi_opnsense-0.0.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_opnsense-0.0.83.tar", last modified: Tue Jul 25 07:51:39 2023, max compression
+gzip compressed data, was "pulumi_opnsense-0.0.84.tar", last modified: Tue Jul 25 08:56:13 2023, max compression
```

## Comparing `pulumi_opnsense-0.0.83.tar` & `pulumi_opnsense-0.0.84.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:51:39.719253 pulumi_opnsense-0.0.83/
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-25 07:51:39.719253 pulumi_opnsense-0.0.83/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-25 07:51:39.000000 pulumi_opnsense-0.0.83/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:51:39.715253 pulumi_opnsense-0.0.83/pulumi_opnsense/
--rw-------   0 runner    (1001) docker     (123)      994 2023-07-25 07:51:39.000000 pulumi_opnsense-0.0.83/pulumi_opnsense/__init__.py
--rw-------   0 runner    (1001) docker     (123)     8097 2023-07-25 07:51:39.000000 pulumi_opnsense-0.0.83/pulumi_opnsense/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:51:39.719253 pulumi_opnsense-0.0.83/pulumi_opnsense/config/
--rw-------   0 runner    (1001) docker     (123)      251 2023-07-25 07:51:39.000000 pulumi_opnsense-0.0.83/pulumi_opnsense/config/__init__.py
--rw-------   0 runner    (1001) docker     (123)     1112 2023-07-25 07:51:39.000000 pulumi_opnsense-0.0.83/pulumi_opnsense/config/vars.py
--rw-------   0 runner    (1001) docker     (123)     7795 2023-07-25 07:51:39.000000 pulumi_opnsense-0.0.83/pulumi_opnsense/provider.py
--rw-------   0 runner    (1001) docker     (123)      113 2023-07-25 07:51:39.000000 pulumi_opnsense-0.0.83/pulumi_opnsense/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (123)        0 2023-07-25 07:51:39.000000 pulumi_opnsense-0.0.83/pulumi_opnsense/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:51:39.719253 pulumi_opnsense-0.0.83/pulumi_opnsense/unbound/
--rw-------   0 runner    (1001) docker     (123)      290 2023-07-25 07:51:39.000000 pulumi_opnsense-0.0.83/pulumi_opnsense/unbound/__init__.py
--rw-------   0 runner    (1001) docker     (123)     4485 2023-07-25 07:51:39.000000 pulumi_opnsense-0.0.83/pulumi_opnsense/unbound/host_alias.py
--rw-------   0 runner    (1001) docker     (123)     9878 2023-07-25 07:51:39.000000 pulumi_opnsense-0.0.83/pulumi_opnsense/unbound/host_override.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:51:39.715253 pulumi_opnsense-0.0.83/pulumi_opnsense.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-25 07:51:39.000000 pulumi_opnsense-0.0.83/pulumi_opnsense.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-25 07:51:39.000000 pulumi_opnsense-0.0.83/pulumi_opnsense.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 07:51:39.000000 pulumi_opnsense-0.0.83/pulumi_opnsense.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 07:51:39.000000 pulumi_opnsense-0.0.83/pulumi_opnsense.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-25 07:51:39.000000 pulumi_opnsense-0.0.83/pulumi_opnsense.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 07:51:39.000000 pulumi_opnsense-0.0.83/pulumi_opnsense.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 07:51:39.719253 pulumi_opnsense-0.0.83/setup.cfg
--rw-------   0 runner    (1001) docker     (123)     2009 2023-07-25 07:51:39.000000 pulumi_opnsense-0.0.83/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:56:13.177800 pulumi_opnsense-0.0.84/
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-25 08:56:13.177800 pulumi_opnsense-0.0.84/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-25 08:56:12.000000 pulumi_opnsense-0.0.84/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:56:13.173800 pulumi_opnsense-0.0.84/pulumi_opnsense/
+-rw-------   0 runner    (1001) docker     (123)      994 2023-07-25 08:56:12.000000 pulumi_opnsense-0.0.84/pulumi_opnsense/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     8097 2023-07-25 08:56:12.000000 pulumi_opnsense-0.0.84/pulumi_opnsense/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:56:13.177800 pulumi_opnsense-0.0.84/pulumi_opnsense/config/
+-rw-------   0 runner    (1001) docker     (123)      251 2023-07-25 08:56:12.000000 pulumi_opnsense-0.0.84/pulumi_opnsense/config/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     1112 2023-07-25 08:56:12.000000 pulumi_opnsense-0.0.84/pulumi_opnsense/config/vars.py
+-rw-------   0 runner    (1001) docker     (123)     7795 2023-07-25 08:56:12.000000 pulumi_opnsense-0.0.84/pulumi_opnsense/provider.py
+-rw-------   0 runner    (1001) docker     (123)      113 2023-07-25 08:56:12.000000 pulumi_opnsense-0.0.84/pulumi_opnsense/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (123)        0 2023-07-25 08:56:12.000000 pulumi_opnsense-0.0.84/pulumi_opnsense/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:56:13.177800 pulumi_opnsense-0.0.84/pulumi_opnsense/unbound/
+-rw-------   0 runner    (1001) docker     (123)      290 2023-07-25 08:56:12.000000 pulumi_opnsense-0.0.84/pulumi_opnsense/unbound/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     4485 2023-07-25 08:56:12.000000 pulumi_opnsense-0.0.84/pulumi_opnsense/unbound/host_alias.py
+-rw-------   0 runner    (1001) docker     (123)     9878 2023-07-25 08:56:12.000000 pulumi_opnsense-0.0.84/pulumi_opnsense/unbound/host_override.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:56:13.177800 pulumi_opnsense-0.0.84/pulumi_opnsense.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-25 08:56:13.000000 pulumi_opnsense-0.0.84/pulumi_opnsense.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-25 08:56:13.000000 pulumi_opnsense-0.0.84/pulumi_opnsense.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 08:56:13.000000 pulumi_opnsense-0.0.84/pulumi_opnsense.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 08:56:13.000000 pulumi_opnsense-0.0.84/pulumi_opnsense.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-25 08:56:13.000000 pulumi_opnsense-0.0.84/pulumi_opnsense.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 08:56:13.000000 pulumi_opnsense-0.0.84/pulumi_opnsense.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 08:56:13.177800 pulumi_opnsense-0.0.84/setup.cfg
+-rw-------   0 runner    (1001) docker     (123)     2009 2023-07-25 08:56:12.000000 pulumi_opnsense-0.0.84/setup.py
```

### Comparing `pulumi_opnsense-0.0.83/PKG-INFO` & `pulumi_opnsense-0.0.84/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_opnsense
-Version: 0.0.83
+Version: 0.0.84
 License: Apache-2.0
 Project-URL: Repository, https://github.com/oss4u/pulumi-opnsense-native
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Pulumi Native Provider Boilerplate
```

### Comparing `pulumi_opnsense-0.0.83/README.md` & `pulumi_opnsense-0.0.84/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_opnsense-0.0.83/pulumi_opnsense/__init__.py` & `pulumi_opnsense-0.0.84/pulumi_opnsense/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_opnsense-0.0.83/pulumi_opnsense/_utilities.py` & `pulumi_opnsense-0.0.84/pulumi_opnsense/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_opnsense-0.0.83/pulumi_opnsense/config/vars.py` & `pulumi_opnsense-0.0.84/pulumi_opnsense/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_opnsense-0.0.83/pulumi_opnsense/provider.py` & `pulumi_opnsense-0.0.84/pulumi_opnsense/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_opnsense-0.0.83/pulumi_opnsense/unbound/host_alias.py` & `pulumi_opnsense-0.0.84/pulumi_opnsense/unbound/host_alias.py`

 * *Files identical despite different names*

### Comparing `pulumi_opnsense-0.0.83/pulumi_opnsense/unbound/host_override.py` & `pulumi_opnsense-0.0.84/pulumi_opnsense/unbound/host_override.py`

 * *Files identical despite different names*

### Comparing `pulumi_opnsense-0.0.83/pulumi_opnsense.egg-info/PKG-INFO` & `pulumi_opnsense-0.0.84/pulumi_opnsense.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-opnsense
-Version: 0.0.83
+Version: 0.0.84
 License: Apache-2.0
 Project-URL: Repository, https://github.com/oss4u/pulumi-opnsense-native
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Pulumi Native Provider Boilerplate
```

### Comparing `pulumi_opnsense-0.0.83/pulumi_opnsense.egg-info/SOURCES.txt` & `pulumi_opnsense-0.0.84/pulumi_opnsense.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_opnsense-0.0.83/setup.py` & `pulumi_opnsense-0.0.84/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.83"
-PLUGIN_VERSION = "0.0.83"
+VERSION = "0.0.84"
+PLUGIN_VERSION = "0.0.84"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'opnsense', PLUGIN_VERSION, '--server', 'github://api.github.com/oss4u/pulumi-opnsense-native'])
         except OSError as error:
```

