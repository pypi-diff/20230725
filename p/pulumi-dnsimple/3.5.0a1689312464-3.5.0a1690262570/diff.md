# Comparing `tmp/pulumi_dnsimple-3.5.0a1689312464.tar.gz` & `tmp/pulumi_dnsimple-3.5.0a1690262570.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_dnsimple-3.5.0a1689312464.tar", last modified: Fri Jul 14 05:39:21 2023, max compression
+gzip compressed data, was "pulumi_dnsimple-3.5.0a1690262570.tar", last modified: Tue Jul 25 05:27:36 2023, max compression
```

## Comparing `pulumi_dnsimple-3.5.0a1689312464.tar` & `pulumi_dnsimple-3.5.0a1690262570.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:39:21.220402 pulumi_dnsimple-3.5.0a1689312464/
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-14 05:39:21.220402 pulumi_dnsimple-3.5.0a1689312464/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-07-14 05:39:20.000000 pulumi_dnsimple-3.5.0a1689312464/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:39:21.216401 pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple/
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-14 05:39:20.000000 pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-14 05:39:20.000000 pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:39:21.216401 pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-14 05:39:20.000000 pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-14 05:39:20.000000 pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-07-14 05:39:20.000000 pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     8785 2023-07-14 05:39:20.000000 pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple/email_forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-14 05:39:20.000000 pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple/get_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-14 05:39:20.000000 pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple/get_zone.py
--rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-07-14 05:39:20.000000 pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple/lets_encrypt_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-07-14 05:39:20.000000 pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-14 05:39:20.000000 pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 05:39:20.000000 pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-07-14 05:39:20.000000 pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple/record.py
--rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-07-14 05:39:20.000000 pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple/zone_record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 05:39:21.216401 pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-14 05:39:21.000000 pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-14 05:39:21.000000 pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 05:39:21.000000 pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 05:39:21.000000 pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 05:39:21.000000 pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-14 05:39:21.000000 pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 05:39:21.220402 pulumi_dnsimple-3.5.0a1689312464/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-14 05:39:20.000000 pulumi_dnsimple-3.5.0a1689312464/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:27:36.444379 pulumi_dnsimple-3.5.0a1690262570/
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-25 05:27:36.444379 pulumi_dnsimple-3.5.0a1690262570/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-07-25 05:27:36.000000 pulumi_dnsimple-3.5.0a1690262570/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:27:36.444379 pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple/
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-25 05:27:36.000000 pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-25 05:27:36.000000 pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:27:36.444379 pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-25 05:27:36.000000 pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-25 05:27:36.000000 pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-07-25 05:27:36.000000 pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8785 2023-07-25 05:27:36.000000 pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple/email_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-25 05:27:36.000000 pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple/get_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-25 05:27:36.000000 pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple/get_zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-07-25 05:27:36.000000 pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple/lets_encrypt_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-07-25 05:27:36.000000 pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-25 05:27:36.000000 pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 05:27:36.000000 pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-07-25 05:27:36.000000 pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-07-25 05:27:36.000000 pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple/zone_record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:27:36.444379 pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-25 05:27:36.000000 pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-25 05:27:36.000000 pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 05:27:36.000000 pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 05:27:36.000000 pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-25 05:27:36.000000 pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 05:27:36.000000 pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 05:27:36.448379 pulumi_dnsimple-3.5.0a1690262570/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-25 05:27:36.000000 pulumi_dnsimple-3.5.0a1690262570/setup.py
```

### Comparing `pulumi_dnsimple-3.5.0a1689312464/PKG-INFO` & `pulumi_dnsimple-3.5.0a1690262570/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_dnsimple
-Version: 3.5.0a1689312464
+Version: 3.5.0a1690262570
 Summary: A Pulumi package for creating and managing dnsimple cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-dnsimple
 Keywords: pulumi dnsimple
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_dnsimple-3.5.0a1689312464/README.md` & `pulumi_dnsimple-3.5.0a1690262570/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple/__init__.py` & `pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple/_utilities.py` & `pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple/config/vars.py` & `pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple/domain.py` & `pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple/domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple/email_forward.py` & `pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple/email_forward.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple/get_certificate.py` & `pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple/get_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple/get_zone.py` & `pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple/get_zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple/lets_encrypt_certificate.py` & `pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple/lets_encrypt_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple/provider.py` & `pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple/record.py` & `pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple/record.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple/zone_record.py` & `pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple/zone_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple.egg-info/PKG-INFO` & `pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-dnsimple
-Version: 3.5.0a1689312464
+Version: 3.5.0a1690262570
 Summary: A Pulumi package for creating and managing dnsimple cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-dnsimple
 Keywords: pulumi dnsimple
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_dnsimple-3.5.0a1689312464/pulumi_dnsimple.egg-info/SOURCES.txt` & `pulumi_dnsimple-3.5.0a1690262570/pulumi_dnsimple.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1689312464/setup.py` & `pulumi_dnsimple-3.5.0a1690262570/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.5.0a1689312464"
-PLUGIN_VERSION = "3.5.0-alpha.1689312464+1c70763e"
+VERSION = "3.5.0a1690262570"
+PLUGIN_VERSION = "3.5.0-alpha.1690262570+781c7adc"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'dnsimple', PLUGIN_VERSION])
         except OSError as error:
```

