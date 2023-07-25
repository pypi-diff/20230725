# Comparing `tmp/pulumi_venafi-1.6.0a1689317304.tar.gz` & `tmp/pulumi_venafi-1.6.0a1690265262.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_venafi-1.6.0a1689317304.tar", last modified: Fri Jul 14 06:53:00 2023, max compression
+gzip compressed data, was "pulumi_venafi-1.6.0a1690265262.tar", last modified: Tue Jul 25 06:14:48 2023, max compression
```

## Comparing `pulumi_venafi-1.6.0a1689317304.tar` & `pulumi_venafi-1.6.0a1690265262.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:53:00.229684 pulumi_venafi-1.6.0a1689317304/
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-14 06:53:00.229684 pulumi_venafi-1.6.0a1689317304/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-07-14 06:52:59.000000 pulumi_venafi-1.6.0a1689317304/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:53:00.225685 pulumi_venafi-1.6.0a1689317304/pulumi_venafi/
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-14 06:52:59.000000 pulumi_venafi-1.6.0a1689317304/pulumi_venafi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-14 06:52:59.000000 pulumi_venafi-1.6.0a1689317304/pulumi_venafi/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    48936 2023-07-14 06:52:59.000000 pulumi_venafi-1.6.0a1689317304/pulumi_venafi/certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:53:00.229684 pulumi_venafi-1.6.0a1689317304/pulumi_venafi/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-14 06:52:59.000000 pulumi_venafi-1.6.0a1689317304/pulumi_venafi/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-14 06:52:59.000000 pulumi_venafi-1.6.0a1689317304/pulumi_venafi/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    11593 2023-07-14 06:52:59.000000 pulumi_venafi-1.6.0a1689317304/pulumi_venafi/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14951 2023-07-14 06:52:59.000000 pulumi_venafi-1.6.0a1689317304/pulumi_venafi/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-14 06:52:59.000000 pulumi_venafi-1.6.0a1689317304/pulumi_venafi/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:52:59.000000 pulumi_venafi-1.6.0a1689317304/pulumi_venafi/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    53209 2023-07-14 06:52:59.000000 pulumi_venafi-1.6.0a1689317304/pulumi_venafi/ssh_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-07-14 06:52:59.000000 pulumi_venafi-1.6.0a1689317304/pulumi_venafi/ssh_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:53:00.229684 pulumi_venafi-1.6.0a1689317304/pulumi_venafi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-14 06:53:00.000000 pulumi_venafi-1.6.0a1689317304/pulumi_venafi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-14 06:53:00.000000 pulumi_venafi-1.6.0a1689317304/pulumi_venafi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 06:53:00.000000 pulumi_venafi-1.6.0a1689317304/pulumi_venafi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 06:53:00.000000 pulumi_venafi-1.6.0a1689317304/pulumi_venafi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 06:53:00.000000 pulumi_venafi-1.6.0a1689317304/pulumi_venafi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-14 06:53:00.000000 pulumi_venafi-1.6.0a1689317304/pulumi_venafi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 06:53:00.229684 pulumi_venafi-1.6.0a1689317304/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-14 06:52:59.000000 pulumi_venafi-1.6.0a1689317304/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:14:48.440204 pulumi_venafi-1.6.0a1690265262/
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-25 06:14:48.440204 pulumi_venafi-1.6.0a1690265262/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-07-25 06:14:48.000000 pulumi_venafi-1.6.0a1690265262/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:14:48.436204 pulumi_venafi-1.6.0a1690265262/pulumi_venafi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-25 06:14:48.000000 pulumi_venafi-1.6.0a1690265262/pulumi_venafi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-25 06:14:48.000000 pulumi_venafi-1.6.0a1690265262/pulumi_venafi/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48936 2023-07-25 06:14:48.000000 pulumi_venafi-1.6.0a1690265262/pulumi_venafi/certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:14:48.440204 pulumi_venafi-1.6.0a1690265262/pulumi_venafi/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-25 06:14:48.000000 pulumi_venafi-1.6.0a1690265262/pulumi_venafi/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-25 06:14:48.000000 pulumi_venafi-1.6.0a1690265262/pulumi_venafi/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11593 2023-07-25 06:14:48.000000 pulumi_venafi-1.6.0a1690265262/pulumi_venafi/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14951 2023-07-25 06:14:48.000000 pulumi_venafi-1.6.0a1690265262/pulumi_venafi/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-25 06:14:48.000000 pulumi_venafi-1.6.0a1690265262/pulumi_venafi/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 06:14:48.000000 pulumi_venafi-1.6.0a1690265262/pulumi_venafi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    53209 2023-07-25 06:14:48.000000 pulumi_venafi-1.6.0a1690265262/pulumi_venafi/ssh_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-07-25 06:14:48.000000 pulumi_venafi-1.6.0a1690265262/pulumi_venafi/ssh_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:14:48.436204 pulumi_venafi-1.6.0a1690265262/pulumi_venafi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-25 06:14:48.000000 pulumi_venafi-1.6.0a1690265262/pulumi_venafi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-25 06:14:48.000000 pulumi_venafi-1.6.0a1690265262/pulumi_venafi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:14:48.000000 pulumi_venafi-1.6.0a1690265262/pulumi_venafi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:14:48.000000 pulumi_venafi-1.6.0a1690265262/pulumi_venafi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-25 06:14:48.000000 pulumi_venafi-1.6.0a1690265262/pulumi_venafi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 06:14:48.000000 pulumi_venafi-1.6.0a1690265262/pulumi_venafi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 06:14:48.440204 pulumi_venafi-1.6.0a1690265262/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-25 06:14:48.000000 pulumi_venafi-1.6.0a1690265262/setup.py
```

### Comparing `pulumi_venafi-1.6.0a1689317304/PKG-INFO` & `pulumi_venafi-1.6.0a1690265262/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_venafi
-Version: 1.6.0a1689317304
+Version: 1.6.0a1690265262
 Summary: A Pulumi package for creating and managing venafi cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-venafi
 Keywords: pulumi venafi
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_venafi-1.6.0a1689317304/README.md` & `pulumi_venafi-1.6.0a1690265262/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1689317304/pulumi_venafi/__init__.py` & `pulumi_venafi-1.6.0a1690265262/pulumi_venafi/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1689317304/pulumi_venafi/_utilities.py` & `pulumi_venafi-1.6.0a1690265262/pulumi_venafi/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1689317304/pulumi_venafi/certificate.py` & `pulumi_venafi-1.6.0a1690265262/pulumi_venafi/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1689317304/pulumi_venafi/config/vars.py` & `pulumi_venafi-1.6.0a1690265262/pulumi_venafi/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1689317304/pulumi_venafi/policy.py` & `pulumi_venafi-1.6.0a1690265262/pulumi_venafi/policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1689317304/pulumi_venafi/provider.py` & `pulumi_venafi-1.6.0a1690265262/pulumi_venafi/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1689317304/pulumi_venafi/ssh_certificate.py` & `pulumi_venafi-1.6.0a1690265262/pulumi_venafi/ssh_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1689317304/pulumi_venafi/ssh_config.py` & `pulumi_venafi-1.6.0a1690265262/pulumi_venafi/ssh_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1689317304/pulumi_venafi.egg-info/PKG-INFO` & `pulumi_venafi-1.6.0a1690265262/pulumi_venafi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-venafi
-Version: 1.6.0a1689317304
+Version: 1.6.0a1690265262
 Summary: A Pulumi package for creating and managing venafi cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-venafi
 Keywords: pulumi venafi
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_venafi-1.6.0a1689317304/pulumi_venafi.egg-info/SOURCES.txt` & `pulumi_venafi-1.6.0a1690265262/pulumi_venafi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1689317304/setup.py` & `pulumi_venafi-1.6.0a1690265262/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.6.0a1689317304"
-PLUGIN_VERSION = "1.6.0-alpha.1689317304+6b7b54ae"
+VERSION = "1.6.0a1690265262"
+PLUGIN_VERSION = "1.6.0-alpha.1690265262+d5b9ddba"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'venafi', PLUGIN_VERSION])
         except OSError as error:
```

