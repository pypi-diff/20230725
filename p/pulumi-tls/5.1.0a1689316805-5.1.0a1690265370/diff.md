# Comparing `tmp/pulumi_tls-5.1.0a1689316805.tar.gz` & `tmp/pulumi_tls-5.1.0a1690265370.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_tls-5.1.0a1689316805.tar", last modified: Fri Jul 14 06:48:38 2023, max compression
+gzip compressed data, was "pulumi_tls-5.1.0a1690265370.tar", last modified: Tue Jul 25 06:15:01 2023, max compression
```

## Comparing `pulumi_tls-5.1.0a1689316805.tar` & `pulumi_tls-5.1.0a1690265370.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:48:38.841864 pulumi_tls-5.1.0a1689316805/
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-14 06:48:38.841864 pulumi_tls-5.1.0a1689316805/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-14 06:48:38.000000 pulumi_tls-5.1.0a1689316805/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:48:38.837864 pulumi_tls-5.1.0a1689316805/pulumi_tls/
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-14 06:48:38.000000 pulumi_tls-5.1.0a1689316805/pulumi_tls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13099 2023-07-14 06:48:38.000000 pulumi_tls-5.1.0a1689316805/pulumi_tls/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-14 06:48:38.000000 pulumi_tls-5.1.0a1689316805/pulumi_tls/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    22603 2023-07-14 06:48:38.000000 pulumi_tls-5.1.0a1689316805/pulumi_tls/cert_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:48:38.841864 pulumi_tls-5.1.0a1689316805/pulumi_tls/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-14 06:48:38.000000 pulumi_tls-5.1.0a1689316805/pulumi_tls/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-14 06:48:38.000000 pulumi_tls-5.1.0a1689316805/pulumi_tls/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-14 06:48:38.000000 pulumi_tls-5.1.0a1689316805/pulumi_tls/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-07-14 06:48:38.000000 pulumi_tls-5.1.0a1689316805/pulumi_tls/get_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-07-14 06:48:38.000000 pulumi_tls-5.1.0a1689316805/pulumi_tls/get_public_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    41155 2023-07-14 06:48:38.000000 pulumi_tls-5.1.0a1689316805/pulumi_tls/locally_signed_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)    14909 2023-07-14 06:48:38.000000 pulumi_tls-5.1.0a1689316805/pulumi_tls/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22201 2023-07-14 06:48:38.000000 pulumi_tls-5.1.0a1689316805/pulumi_tls/private_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-07-14 06:48:38.000000 pulumi_tls-5.1.0a1689316805/pulumi_tls/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-14 06:48:38.000000 pulumi_tls-5.1.0a1689316805/pulumi_tls/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:48:38.000000 pulumi_tls-5.1.0a1689316805/pulumi_tls/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    52451 2023-07-14 06:48:38.000000 pulumi_tls-5.1.0a1689316805/pulumi_tls/self_signed_cert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:48:38.837864 pulumi_tls-5.1.0a1689316805/pulumi_tls.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-14 06:48:38.000000 pulumi_tls-5.1.0a1689316805/pulumi_tls.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-14 06:48:38.000000 pulumi_tls-5.1.0a1689316805/pulumi_tls.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 06:48:38.000000 pulumi_tls-5.1.0a1689316805/pulumi_tls.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 06:48:38.000000 pulumi_tls-5.1.0a1689316805/pulumi_tls.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 06:48:38.000000 pulumi_tls-5.1.0a1689316805/pulumi_tls.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-14 06:48:38.000000 pulumi_tls-5.1.0a1689316805/pulumi_tls.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 06:48:38.841864 pulumi_tls-5.1.0a1689316805/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-14 06:48:38.000000 pulumi_tls-5.1.0a1689316805/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:15:01.291043 pulumi_tls-5.1.0a1690265370/
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-25 06:15:01.291043 pulumi_tls-5.1.0a1690265370/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-25 06:15:00.000000 pulumi_tls-5.1.0a1690265370/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:15:01.291043 pulumi_tls-5.1.0a1690265370/pulumi_tls/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-25 06:15:00.000000 pulumi_tls-5.1.0a1690265370/pulumi_tls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13099 2023-07-25 06:15:00.000000 pulumi_tls-5.1.0a1690265370/pulumi_tls/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-25 06:15:00.000000 pulumi_tls-5.1.0a1690265370/pulumi_tls/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22603 2023-07-25 06:15:00.000000 pulumi_tls-5.1.0a1690265370/pulumi_tls/cert_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:15:01.291043 pulumi_tls-5.1.0a1690265370/pulumi_tls/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-25 06:15:00.000000 pulumi_tls-5.1.0a1690265370/pulumi_tls/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-25 06:15:00.000000 pulumi_tls-5.1.0a1690265370/pulumi_tls/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-25 06:15:00.000000 pulumi_tls-5.1.0a1690265370/pulumi_tls/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-07-25 06:15:00.000000 pulumi_tls-5.1.0a1690265370/pulumi_tls/get_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-07-25 06:15:00.000000 pulumi_tls-5.1.0a1690265370/pulumi_tls/get_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41155 2023-07-25 06:15:00.000000 pulumi_tls-5.1.0a1690265370/pulumi_tls/locally_signed_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14909 2023-07-25 06:15:00.000000 pulumi_tls-5.1.0a1690265370/pulumi_tls/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22201 2023-07-25 06:15:00.000000 pulumi_tls-5.1.0a1690265370/pulumi_tls/private_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-07-25 06:15:00.000000 pulumi_tls-5.1.0a1690265370/pulumi_tls/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-25 06:15:00.000000 pulumi_tls-5.1.0a1690265370/pulumi_tls/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 06:15:00.000000 pulumi_tls-5.1.0a1690265370/pulumi_tls/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    52451 2023-07-25 06:15:00.000000 pulumi_tls-5.1.0a1690265370/pulumi_tls/self_signed_cert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:15:01.291043 pulumi_tls-5.1.0a1690265370/pulumi_tls.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-25 06:15:01.000000 pulumi_tls-5.1.0a1690265370/pulumi_tls.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-25 06:15:01.000000 pulumi_tls-5.1.0a1690265370/pulumi_tls.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:15:01.000000 pulumi_tls-5.1.0a1690265370/pulumi_tls.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:15:01.000000 pulumi_tls-5.1.0a1690265370/pulumi_tls.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-25 06:15:01.000000 pulumi_tls-5.1.0a1690265370/pulumi_tls.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-25 06:15:01.000000 pulumi_tls-5.1.0a1690265370/pulumi_tls.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 06:15:01.291043 pulumi_tls-5.1.0a1690265370/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-25 06:15:00.000000 pulumi_tls-5.1.0a1690265370/setup.py
```

### Comparing `pulumi_tls-5.1.0a1689316805/PKG-INFO` & `pulumi_tls-5.1.0a1690265370/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_tls
-Version: 5.1.0a1689316805
+Version: 5.1.0a1690265370
 Summary: A Pulumi package to create TLS resources in Pulumi programs.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-tls
 Keywords: pulumi tls
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_tls-5.1.0a1689316805/README.md` & `pulumi_tls-5.1.0a1690265370/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1689316805/pulumi_tls/__init__.py` & `pulumi_tls-5.1.0a1690265370/pulumi_tls/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1689316805/pulumi_tls/_inputs.py` & `pulumi_tls-5.1.0a1690265370/pulumi_tls/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1689316805/pulumi_tls/_utilities.py` & `pulumi_tls-5.1.0a1690265370/pulumi_tls/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1689316805/pulumi_tls/cert_request.py` & `pulumi_tls-5.1.0a1690265370/pulumi_tls/cert_request.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1689316805/pulumi_tls/config/outputs.py` & `pulumi_tls-5.1.0a1690265370/pulumi_tls/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1689316805/pulumi_tls/config/vars.py` & `pulumi_tls-5.1.0a1690265370/pulumi_tls/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1689316805/pulumi_tls/get_certificate.py` & `pulumi_tls-5.1.0a1690265370/pulumi_tls/get_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1689316805/pulumi_tls/get_public_key.py` & `pulumi_tls-5.1.0a1690265370/pulumi_tls/get_public_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1689316805/pulumi_tls/locally_signed_cert.py` & `pulumi_tls-5.1.0a1690265370/pulumi_tls/locally_signed_cert.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1689316805/pulumi_tls/outputs.py` & `pulumi_tls-5.1.0a1690265370/pulumi_tls/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1689316805/pulumi_tls/private_key.py` & `pulumi_tls-5.1.0a1690265370/pulumi_tls/private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1689316805/pulumi_tls/provider.py` & `pulumi_tls-5.1.0a1690265370/pulumi_tls/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1689316805/pulumi_tls/self_signed_cert.py` & `pulumi_tls-5.1.0a1690265370/pulumi_tls/self_signed_cert.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1689316805/pulumi_tls.egg-info/PKG-INFO` & `pulumi_tls-5.1.0a1690265370/pulumi_tls.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-tls
-Version: 5.1.0a1689316805
+Version: 5.1.0a1690265370
 Summary: A Pulumi package to create TLS resources in Pulumi programs.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-tls
 Keywords: pulumi tls
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_tls-5.1.0a1689316805/pulumi_tls.egg-info/SOURCES.txt` & `pulumi_tls-5.1.0a1690265370/pulumi_tls.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1689316805/setup.py` & `pulumi_tls-5.1.0a1690265370/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "5.1.0a1689316805"
-PLUGIN_VERSION = "5.1.0-alpha.1689316805+ef3c918e"
+VERSION = "5.1.0a1690265370"
+PLUGIN_VERSION = "5.1.0-alpha.1690265370+6d07413b"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'tls', PLUGIN_VERSION])
         except OSError as error:
```

