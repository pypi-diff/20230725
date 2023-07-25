# Comparing `tmp/vdk-kerberos-auth-0.3.824443273.tar.gz` & `tmp/vdk-kerberos-auth-0.3.944393829.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-kerberos-auth-0.3.824443273.tar", last modified: Fri Mar 31 14:25:32 2023, max compression
+gzip compressed data, was "vdk-kerberos-auth-0.3.944393829.tar", last modified: Tue Jul 25 09:00:59 2023, max compression
```

## Comparing `vdk-kerberos-auth-0.3.824443273.tar` & `vdk-kerberos-auth-0.3.944393829.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:32.593148 vdk-kerberos-auth-0.3.824443273/
--rw-r--r--   0 root         (0) root         (0)     3874 2023-03-31 14:25:32.593148 vdk-kerberos-auth-0.3.824443273/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3281 2023-03-31 14:25:20.000000 vdk-kerberos-auth-0.3.824443273/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-31 14:25:32.593148 vdk-kerberos-auth-0.3.824443273/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1173 2023-03-31 14:25:24.000000 vdk-kerberos-auth-0.3.824443273/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:32.589148 vdk-kerberos-auth-0.3.824443273/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:32.589148 vdk-kerberos-auth-0.3.824443273/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:32.589148 vdk-kerberos-auth-0.3.824443273/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:32.593148 vdk-kerberos-auth-0.3.824443273/src/vdk/plugin/kerberos/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:32.593148 vdk-kerberos-auth-0.3.824443273/src/vdk/plugin/kerberos/api/
--rw-rw-rw-   0 root         (0) root         (0)     1521 2023-03-31 14:25:20.000000 vdk-kerberos-auth-0.3.824443273/src/vdk/plugin/kerberos/api/kerberos_client.py
--rw-rw-rw-   0 root         (0) root         (0)     2218 2023-03-31 14:25:20.000000 vdk-kerberos-auth-0.3.824443273/src/vdk/plugin/kerberos/authenticator_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     2395 2023-03-31 14:25:20.000000 vdk-kerberos-auth-0.3.824443273/src/vdk/plugin/kerberos/base_authenticator.py
--rw-rw-rw-   0 root         (0) root         (0)     5938 2023-03-31 14:25:20.000000 vdk-kerberos-auth-0.3.824443273/src/vdk/plugin/kerberos/kerberos_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     3824 2023-03-31 14:25:20.000000 vdk-kerberos-auth-0.3.824443273/src/vdk/plugin/kerberos/kerberos_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     1383 2023-03-31 14:25:20.000000 vdk-kerberos-auth-0.3.824443273/src/vdk/plugin/kerberos/kerberos_ticket.py
--rw-rw-rw-   0 root         (0) root         (0)     3978 2023-03-31 14:25:20.000000 vdk-kerberos-auth-0.3.824443273/src/vdk/plugin/kerberos/kinit_authenticator.py
--rw-rw-rw-   0 root         (0) root         (0)     4241 2023-03-31 14:25:20.000000 vdk-kerberos-auth-0.3.824443273/src/vdk/plugin/kerberos/minikerberos_authenticator.py
--rw-rw-rw-   0 root         (0) root         (0)     6639 2023-03-31 14:25:20.000000 vdk-kerberos-auth-0.3.824443273/src/vdk/plugin/kerberos/vdk_kerberos_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:32.593148 vdk-kerberos-auth-0.3.824443273/src/vdk_kerberos_auth.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3874 2023-03-31 14:25:32.000000 vdk-kerberos-auth-0.3.824443273/src/vdk_kerberos_auth.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      739 2023-03-31 14:25:32.000000 vdk-kerberos-auth-0.3.824443273/src/vdk_kerberos_auth.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 14:25:32.000000 vdk-kerberos-auth-0.3.824443273/src/vdk_kerberos_auth.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-31 14:25:32.000000 vdk-kerberos-auth-0.3.824443273/src/vdk_kerberos_auth.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-03-31 14:25:32.000000 vdk-kerberos-auth-0.3.824443273/src/vdk_kerberos_auth.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-31 14:25:32.000000 vdk-kerberos-auth-0.3.824443273/src/vdk_kerberos_auth.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:32.593148 vdk-kerberos-auth-0.3.824443273/tests/
--rw-rw-rw-   0 root         (0) root         (0)    10148 2023-03-31 14:25:20.000000 vdk-kerberos-auth-0.3.824443273/tests/test_kerberos.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.736545 vdk-kerberos-auth-0.3.944393829/
+-rw-r--r--   0 root         (0) root         (0)     3874 2023-07-25 09:00:59.736545 vdk-kerberos-auth-0.3.944393829/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3281 2023-07-25 09:00:43.000000 vdk-kerberos-auth-0.3.944393829/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 09:00:59.736545 vdk-kerberos-auth-0.3.944393829/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1173 2023-07-25 09:00:47.000000 vdk-kerberos-auth-0.3.944393829/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.732545 vdk-kerberos-auth-0.3.944393829/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.732545 vdk-kerberos-auth-0.3.944393829/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.732545 vdk-kerberos-auth-0.3.944393829/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.732545 vdk-kerberos-auth-0.3.944393829/src/vdk/plugin/kerberos/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.732545 vdk-kerberos-auth-0.3.944393829/src/vdk/plugin/kerberos/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2023-07-25 09:00:43.000000 vdk-kerberos-auth-0.3.944393829/src/vdk/plugin/kerberos/api/kerberos_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2218 2023-07-25 09:00:43.000000 vdk-kerberos-auth-0.3.944393829/src/vdk/plugin/kerberos/authenticator_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     2395 2023-07-25 09:00:43.000000 vdk-kerberos-auth-0.3.944393829/src/vdk/plugin/kerberos/base_authenticator.py
+-rw-rw-rw-   0 root         (0) root         (0)     5938 2023-07-25 09:00:43.000000 vdk-kerberos-auth-0.3.944393829/src/vdk/plugin/kerberos/kerberos_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     3824 2023-07-25 09:00:43.000000 vdk-kerberos-auth-0.3.944393829/src/vdk/plugin/kerberos/kerberos_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1383 2023-07-25 09:00:43.000000 vdk-kerberos-auth-0.3.944393829/src/vdk/plugin/kerberos/kerberos_ticket.py
+-rw-rw-rw-   0 root         (0) root         (0)     3978 2023-07-25 09:00:43.000000 vdk-kerberos-auth-0.3.944393829/src/vdk/plugin/kerberos/kinit_authenticator.py
+-rw-rw-rw-   0 root         (0) root         (0)     4241 2023-07-25 09:00:43.000000 vdk-kerberos-auth-0.3.944393829/src/vdk/plugin/kerberos/minikerberos_authenticator.py
+-rw-rw-rw-   0 root         (0) root         (0)     6639 2023-07-25 09:00:43.000000 vdk-kerberos-auth-0.3.944393829/src/vdk/plugin/kerberos/vdk_kerberos_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.736545 vdk-kerberos-auth-0.3.944393829/src/vdk_kerberos_auth.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3874 2023-07-25 09:00:59.000000 vdk-kerberos-auth-0.3.944393829/src/vdk_kerberos_auth.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      739 2023-07-25 09:00:59.000000 vdk-kerberos-auth-0.3.944393829/src/vdk_kerberos_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 09:00:59.000000 vdk-kerberos-auth-0.3.944393829/src/vdk_kerberos_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-25 09:00:59.000000 vdk-kerberos-auth-0.3.944393829/src/vdk_kerberos_auth.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-25 09:00:59.000000 vdk-kerberos-auth-0.3.944393829/src/vdk_kerberos_auth.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-25 09:00:59.000000 vdk-kerberos-auth-0.3.944393829/src/vdk_kerberos_auth.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.736545 vdk-kerberos-auth-0.3.944393829/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    10148 2023-07-25 09:00:43.000000 vdk-kerberos-auth-0.3.944393829/tests/test_kerberos.py
```

### Comparing `vdk-kerberos-auth-0.3.824443273/PKG-INFO` & `vdk-kerberos-auth-0.3.944393829/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-kerberos-auth
-Version: 0.3.824443273
+Version: 0.3.944393829
 Summary: Versatile Data Kit SDK plugin adds Kerberos/GSSAPI support.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-kerberos-auth-0.3.824443273/README.md` & `vdk-kerberos-auth-0.3.944393829/README.md`

 * *Files identical despite different names*

### Comparing `vdk-kerberos-auth-0.3.824443273/setup.py` & `vdk-kerberos-auth-0.3.944393829/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.3.824443273"
+__version__ = "0.3.944393829"
 
 setuptools.setup(
     name="vdk-kerberos-auth",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK plugin adds Kerberos/GSSAPI support.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-kerberos-auth-0.3.824443273/src/vdk/plugin/kerberos/api/kerberos_client.py` & `vdk-kerberos-auth-0.3.944393829/src/vdk/plugin/kerberos/api/kerberos_client.py`

 * *Files identical despite different names*

### Comparing `vdk-kerberos-auth-0.3.824443273/src/vdk/plugin/kerberos/authenticator_factory.py` & `vdk-kerberos-auth-0.3.944393829/src/vdk/plugin/kerberos/authenticator_factory.py`

 * *Files identical despite different names*

### Comparing `vdk-kerberos-auth-0.3.824443273/src/vdk/plugin/kerberos/base_authenticator.py` & `vdk-kerberos-auth-0.3.944393829/src/vdk/plugin/kerberos/base_authenticator.py`

 * *Files identical despite different names*

### Comparing `vdk-kerberos-auth-0.3.824443273/src/vdk/plugin/kerberos/kerberos_configuration.py` & `vdk-kerberos-auth-0.3.944393829/src/vdk/plugin/kerberos/kerberos_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-kerberos-auth-0.3.824443273/src/vdk/plugin/kerberos/kerberos_plugin.py` & `vdk-kerberos-auth-0.3.944393829/src/vdk/plugin/kerberos/kerberos_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-kerberos-auth-0.3.824443273/src/vdk/plugin/kerberos/kerberos_ticket.py` & `vdk-kerberos-auth-0.3.944393829/src/vdk/plugin/kerberos/kerberos_ticket.py`

 * *Files identical despite different names*

### Comparing `vdk-kerberos-auth-0.3.824443273/src/vdk/plugin/kerberos/kinit_authenticator.py` & `vdk-kerberos-auth-0.3.944393829/src/vdk/plugin/kerberos/kinit_authenticator.py`

 * *Files identical despite different names*

### Comparing `vdk-kerberos-auth-0.3.824443273/src/vdk/plugin/kerberos/minikerberos_authenticator.py` & `vdk-kerberos-auth-0.3.944393829/src/vdk/plugin/kerberos/minikerberos_authenticator.py`

 * *Files identical despite different names*

### Comparing `vdk-kerberos-auth-0.3.824443273/src/vdk/plugin/kerberos/vdk_kerberos_client.py` & `vdk-kerberos-auth-0.3.944393829/src/vdk/plugin/kerberos/vdk_kerberos_client.py`

 * *Files identical despite different names*

### Comparing `vdk-kerberos-auth-0.3.824443273/src/vdk_kerberos_auth.egg-info/PKG-INFO` & `vdk-kerberos-auth-0.3.944393829/src/vdk_kerberos_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-kerberos-auth
-Version: 0.3.824443273
+Version: 0.3.944393829
 Summary: Versatile Data Kit SDK plugin adds Kerberos/GSSAPI support.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-kerberos-auth-0.3.824443273/src/vdk_kerberos_auth.egg-info/SOURCES.txt` & `vdk-kerberos-auth-0.3.944393829/src/vdk_kerberos_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vdk-kerberos-auth-0.3.824443273/tests/test_kerberos.py` & `vdk-kerberos-auth-0.3.944393829/tests/test_kerberos.py`

 * *Files identical despite different names*

