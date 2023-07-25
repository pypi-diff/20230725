# Comparing `tmp/idem-vault-0.4.1.tar.gz` & `tmp/idem-vault-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem-vault-0.4.1.tar", last modified: Tue Jul 11 18:47:51 2023, max compression
+gzip compressed data, was "idem-vault-1.0.0.tar", last modified: Tue Jul 25 19:59:54 2023, max compression
```

## Comparing `idem-vault-0.4.1.tar` & `idem-vault-1.0.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/
--rw-r--r--   0 root         (0) root         (0)    11338 2023-07-11 18:47:36.000000 idem-vault-0.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4451 2023-07-11 18:47:51.924913 idem-vault-0.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3616 2023-07-11 18:47:36.000000 idem-vault-0.4.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/acct/backend/
--rw-r--r--   0 root         (0) root         (0)     2915 2023-07-11 18:47:36.000000 idem-vault-0.4.1/idem_vault/acct/backend/vault.py
--rw-r--r--   0 root         (0) root         (0)     1303 2023-07-11 18:47:36.000000 idem-vault-0.4.1/idem_vault/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/exec/hvac/
--rw-r--r--   0 root         (0) root         (0)      571 2023-07-11 18:47:36.000000 idem-vault-0.4.1/idem_vault/exec/hvac/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/exec/vault/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/exec/vault/secrets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/exec/vault/secrets/kv_v1/
--rw-r--r--   0 root         (0) root         (0)     1119 2023-07-11 18:47:36.000000 idem-vault-0.4.1/idem_vault/exec/vault/secrets/kv_v1/secret.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/exec/vault/secrets/kv_v2/
--rw-r--r--   0 root         (0) root         (0)     1257 2023-07-11 18:47:36.000000 idem-vault-0.4.1/idem_vault/exec/vault/secrets/kv_v2/secret.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/source/
--rw-r--r--   0 root         (0) root         (0)     1221 2023-07-11 18:47:36.000000 idem-vault-0.4.1/idem_vault/source/vault.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/states/vault/
--rw-r--r--   0 root         (0) root         (0)      173 2023-07-11 18:47:36.000000 idem-vault-0.4.1/idem_vault/states/vault/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/states/vault/secrets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/states/vault/secrets/kv_v1/
--rw-r--r--   0 root         (0) root         (0)     5986 2023-07-11 18:47:36.000000 idem-vault-0.4.1/idem_vault/states/vault/secrets/kv_v1/key.py
--rw-r--r--   0 root         (0) root         (0)     7793 2023-07-11 18:47:36.000000 idem-vault-0.4.1/idem_vault/states/vault/secrets/kv_v1/secret.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/states/vault/secrets/kv_v2/
--rw-r--r--   0 root         (0) root         (0)     8035 2023-07-11 18:47:36.000000 idem-vault-0.4.1/idem_vault/states/vault/secrets/kv_v2/secret.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/tool/hvac/
--rw-r--r--   0 root         (0) root         (0)     1148 2023-07-11 18:47:36.000000 idem-vault-0.4.1/idem_vault/tool/hvac/client.py
--rw-r--r--   0 root         (0) root         (0)     2047 2023-07-11 18:47:36.000000 idem-vault-0.4.1/idem_vault/tool/hvac/resolve.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault/tool/vault/
--rw-r--r--   0 root         (0) root         (0)      684 2023-07-11 18:47:36.000000 idem-vault-0.4.1/idem_vault/tool/vault/secret.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-11 18:47:51.000000 idem-vault-0.4.1/idem_vault/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 18:47:51.924913 idem-vault-0.4.1/idem_vault.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4451 2023-07-11 18:47:51.000000 idem-vault-0.4.1/idem_vault.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      696 2023-07-11 18:47:51.000000 idem-vault-0.4.1/idem_vault.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 18:47:51.000000 idem-vault-0.4.1/idem_vault.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-07-11 18:47:51.000000 idem-vault-0.4.1/idem_vault.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-11 18:47:51.000000 idem-vault-0.4.1/idem_vault.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-11 18:47:51.924913 idem-vault-0.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2715 2023-07-11 18:47:36.000000 idem-vault-0.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:59:54.296088 idem-vault-1.0.0/
+-rw-r--r--   0 root         (0) root         (0)    11338 2023-07-25 19:59:40.000000 idem-vault-1.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4452 2023-07-25 19:59:54.296088 idem-vault-1.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3616 2023-07-25 19:59:40.000000 idem-vault-1.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:59:54.296088 idem-vault-1.0.0/idem_vault/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:59:54.296088 idem-vault-1.0.0/idem_vault/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:59:54.296088 idem-vault-1.0.0/idem_vault/acct/backend/
+-rw-r--r--   0 root         (0) root         (0)     2915 2023-07-25 19:59:40.000000 idem-vault-1.0.0/idem_vault/acct/backend/vault.py
+-rw-r--r--   0 root         (0) root         (0)     1303 2023-07-25 19:59:40.000000 idem-vault-1.0.0/idem_vault/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:59:54.296088 idem-vault-1.0.0/idem_vault/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:59:54.296088 idem-vault-1.0.0/idem_vault/exec/hvac/
+-rw-r--r--   0 root         (0) root         (0)      571 2023-07-25 19:59:40.000000 idem-vault-1.0.0/idem_vault/exec/hvac/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:59:54.296088 idem-vault-1.0.0/idem_vault/exec/vault/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:59:54.296088 idem-vault-1.0.0/idem_vault/exec/vault/secrets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:59:54.296088 idem-vault-1.0.0/idem_vault/exec/vault/secrets/kv_v1/
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-07-25 19:59:40.000000 idem-vault-1.0.0/idem_vault/exec/vault/secrets/kv_v1/secret.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:59:54.296088 idem-vault-1.0.0/idem_vault/exec/vault/secrets/kv_v2/
+-rw-r--r--   0 root         (0) root         (0)     1257 2023-07-25 19:59:40.000000 idem-vault-1.0.0/idem_vault/exec/vault/secrets/kv_v2/secret.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:59:54.296088 idem-vault-1.0.0/idem_vault/source/
+-rw-r--r--   0 root         (0) root         (0)     1221 2023-07-25 19:59:40.000000 idem-vault-1.0.0/idem_vault/source/vault.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:59:54.296088 idem-vault-1.0.0/idem_vault/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:59:54.296088 idem-vault-1.0.0/idem_vault/states/vault/
+-rw-r--r--   0 root         (0) root         (0)      173 2023-07-25 19:59:40.000000 idem-vault-1.0.0/idem_vault/states/vault/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:59:54.296088 idem-vault-1.0.0/idem_vault/states/vault/secrets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:59:54.296088 idem-vault-1.0.0/idem_vault/states/vault/secrets/kv_v1/
+-rw-r--r--   0 root         (0) root         (0)     6063 2023-07-25 19:59:40.000000 idem-vault-1.0.0/idem_vault/states/vault/secrets/kv_v1/key.py
+-rw-r--r--   0 root         (0) root         (0)     7793 2023-07-25 19:59:40.000000 idem-vault-1.0.0/idem_vault/states/vault/secrets/kv_v1/secret.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:59:54.296088 idem-vault-1.0.0/idem_vault/states/vault/secrets/kv_v2/
+-rw-r--r--   0 root         (0) root         (0)     8100 2023-07-25 19:59:40.000000 idem-vault-1.0.0/idem_vault/states/vault/secrets/kv_v2/secret.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:59:54.296088 idem-vault-1.0.0/idem_vault/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:59:54.296088 idem-vault-1.0.0/idem_vault/tool/hvac/
+-rw-r--r--   0 root         (0) root         (0)     1148 2023-07-25 19:59:40.000000 idem-vault-1.0.0/idem_vault/tool/hvac/client.py
+-rw-r--r--   0 root         (0) root         (0)     2047 2023-07-25 19:59:40.000000 idem-vault-1.0.0/idem_vault/tool/hvac/resolve.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:59:54.296088 idem-vault-1.0.0/idem_vault/tool/vault/
+-rw-r--r--   0 root         (0) root         (0)      684 2023-07-25 19:59:40.000000 idem-vault-1.0.0/idem_vault/tool/vault/secret.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-25 19:59:53.000000 idem-vault-1.0.0/idem_vault/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 19:59:54.296088 idem-vault-1.0.0/idem_vault.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4452 2023-07-25 19:59:54.000000 idem-vault-1.0.0/idem_vault.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      696 2023-07-25 19:59:54.000000 idem-vault-1.0.0/idem_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 19:59:54.000000 idem-vault-1.0.0/idem_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2023-07-25 19:59:54.000000 idem-vault-1.0.0/idem_vault.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-25 19:59:54.000000 idem-vault-1.0.0/idem_vault.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-25 19:59:54.296088 idem-vault-1.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2716 2023-07-25 19:59:40.000000 idem-vault-1.0.0/setup.py
```

### Comparing `idem-vault-0.4.1/LICENSE` & `idem-vault-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idem-vault-0.4.1/PKG-INFO` & `idem-vault-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: idem-vault
-Version: 0.4.1
+Version: 1.0.0
 Summary: UNKNOWN
 Home-page: https://gitlab.com/vmware/idem/idem-vault
 Author: VMware Inc.
 Author-email: hyingzhi@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ==========
 Idem-vault
 ==========
 
@@ -55,15 +55,15 @@
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
-* Python 3.7+
+* Python 3.8+
 * git *(if installing from source, or contributing to the project)*
 
 Installation
 ------------
 
 .. note::
```

### Comparing `idem-vault-0.4.1/README.rst` & `idem-vault-1.0.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
-* Python 3.7+
+* Python 3.8+
 * git *(if installing from source, or contributing to the project)*
 
 Installation
 ------------
 
 .. note::
```

### Comparing `idem-vault-0.4.1/idem_vault/acct/backend/vault.py` & `idem-vault-1.0.0/idem_vault/acct/backend/vault.py`

 * *Files identical despite different names*

### Comparing `idem-vault-0.4.1/idem_vault/conf.py` & `idem-vault-1.0.0/idem_vault/conf.py`

 * *Files identical despite different names*

### Comparing `idem-vault-0.4.1/idem_vault/exec/hvac/init.py` & `idem-vault-1.0.0/idem_vault/exec/hvac/init.py`

 * *Files identical despite different names*

### Comparing `idem-vault-0.4.1/idem_vault/exec/vault/secrets/kv_v1/secret.py` & `idem-vault-1.0.0/idem_vault/exec/vault/secrets/kv_v1/secret.py`

 * *Files identical despite different names*

### Comparing `idem-vault-0.4.1/idem_vault/exec/vault/secrets/kv_v2/secret.py` & `idem-vault-1.0.0/idem_vault/exec/vault/secrets/kv_v2/secret.py`

 * *Files identical despite different names*

### Comparing `idem-vault-0.4.1/idem_vault/source/vault.py` & `idem-vault-1.0.0/idem_vault/source/vault.py`

 * *Files identical despite different names*

### Comparing `idem-vault-0.4.1/idem_vault/states/vault/secrets/kv_v1/key.py` & `idem-vault-1.0.0/idem_vault/states/vault/secrets/kv_v1/key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 from typing import Dict
 
 import dict_tools.data
 
 TREQ = {
     "unique": ["present", "absent"],
 }
@@ -74,14 +75,15 @@
         and result["old_state"]["key"] == key
         and result["old_state"]["value"]
         and result["old_state"]["value"] == value
     ):
         result["comment"] = (
             f"vault.secrets.kv_v1.key '{name}' nothing to be updated.",
         )
+        result["new_state"] = copy.deepcopy(result["old_state"])
         return result
 
     if ctx.get("test", False):
         result["new_state"] = {"name": name, "path": path, "key": key, "value": value}
         result["comment"] = (f"Would {action} vault.secrets.kv_v1.key '{key}'.",)
         # calculating changes here to show keys that would be updated
         result["changes"] = hub.tool.vault.secret.calculate_changes(
```

### Comparing `idem-vault-0.4.1/idem_vault/states/vault/secrets/kv_v1/secret.py` & `idem-vault-1.0.0/idem_vault/states/vault/secrets/kv_v1/secret.py`

 * *Files identical despite different names*

### Comparing `idem-vault-0.4.1/idem_vault/states/vault/secrets/kv_v2/secret.py` & `idem-vault-1.0.0/idem_vault/states/vault/secrets/kv_v2/secret.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,14 +73,15 @@
         result["comment"] = (
             f"vault.secrets.kv_v2.secret '{name}' read has been disabled.",
         )
     if (result["old_state"] is not None) and result["old_state"]["data"] == data:
         result["comment"] = result["comment"] + (
             f"vault.secrets.kv_v2.secret '{name}' has no property need to be updated.",
         )
+        result["new_state"] = copy.deepcopy(result["old_state"])
         return result
     elif result["old_state"] is None:
         if ctx.get("test", False):
             result["comment"] = (f"Would create vault.secrets.kv_v2.secret '{name}'.",)
             result["new_state"] = {"name": name, "path": path, "data": data}
             return result
     else:
```

### Comparing `idem-vault-0.4.1/idem_vault/tool/hvac/client.py` & `idem-vault-1.0.0/idem_vault/tool/hvac/client.py`

 * *Files identical despite different names*

### Comparing `idem-vault-0.4.1/idem_vault/tool/hvac/resolve.py` & `idem-vault-1.0.0/idem_vault/tool/hvac/resolve.py`

 * *Files identical despite different names*

### Comparing `idem-vault-0.4.1/idem_vault/tool/vault/secret.py` & `idem-vault-1.0.0/idem_vault/tool/vault/secret.py`

 * *Files identical despite different names*

### Comparing `idem-vault-0.4.1/idem_vault.egg-info/PKG-INFO` & `idem-vault-1.0.0/idem_vault.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: idem-vault
-Version: 0.4.1
+Version: 1.0.0
 Summary: UNKNOWN
 Home-page: https://gitlab.com/vmware/idem/idem-vault
 Author: VMware Inc.
 Author-email: hyingzhi@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ==========
 Idem-vault
 ==========
 
@@ -55,15 +55,15 @@
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
-* Python 3.7+
+* Python 3.8+
 * git *(if installing from source, or contributing to the project)*
 
 Installation
 ------------
 
 .. note::
```

### Comparing `idem-vault-0.4.1/idem_vault.egg-info/SOURCES.txt` & `idem-vault-1.0.0/idem_vault.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idem-vault-0.4.1/setup.py` & `idem-vault-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,24 +70,24 @@
     url="https://gitlab.com/vmware/idem/idem-vault",
     version=VERSION,
     install_requires=REQUIREMENTS,
     extras_require=REQUIREMENTS_EXTRA,
     description=DESC,
     long_description=LONG_DESC,
     long_description_content_type="text/x-rst",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     classifiers=[
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: System Administrators",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Development Status :: 5 - Production/Stable",
     ],
     packages=discover_packages(),
     cmdclass={"clean": Clean},
 )
```

