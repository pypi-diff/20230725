# Comparing `tmp/actionlint_py-1.6.25.8.tar.gz` & `tmp/actionlint_py-1.6.25.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "actionlint_py-1.6.25.8.tar", last modified: Tue Jul 25 08:29:06 2023, max compression
+gzip compressed data, was "actionlint_py-1.6.25.9.tar", last modified: Tue Jul 25 13:24:08 2023, max compression
```

## Comparing `actionlint_py-1.6.25.8.tar` & `actionlint_py-1.6.25.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:29:06.270712 actionlint_py-1.6.25.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-25 08:29:06.270712 actionlint_py-1.6.25.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:29:06.270712 actionlint_py-1.6.25.8/_custom_build/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/_custom_build/VERSION_ACTIONLINT.txt
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/_custom_build/VERSION_BUILD_SYSTEM.txt
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/_custom_build/VERSION_DEV.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/_custom_build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/_custom_build/auto_update_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/_custom_build/checksums.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:29:06.270712 actionlint_py-1.6.25.8/_custom_build/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/_custom_build/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/_custom_build/commands/bdist_wheel.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/_custom_build/commands/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/_custom_build/commands/fetch_binaries.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/_custom_build/commands/install.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/_custom_build/commands/install_actionlint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:29:06.270712 actionlint_py-1.6.25.8/_custom_build/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/_custom_build/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/_custom_build/utils/file_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/_custom_build/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:29:06.270712 actionlint_py-1.6.25.8/actionlint_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-25 08:29:06.000000 actionlint_py-1.6.25.8/actionlint_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-25 08:29:06.000000 actionlint_py-1.6.25.8/actionlint_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 08:29:06.000000 actionlint_py-1.6.25.8/actionlint_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-25 08:29:06.000000 actionlint_py-1.6.25.8/actionlint_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 08:29:06.000000 actionlint_py-1.6.25.8/actionlint_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 08:29:06.270712 actionlint_py-1.6.25.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:24:08.669554 actionlint_py-1.6.25.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-25 13:23:49.000000 actionlint_py-1.6.25.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-25 13:24:08.669554 actionlint_py-1.6.25.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-25 13:23:49.000000 actionlint_py-1.6.25.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:24:08.665554 actionlint_py-1.6.25.9/_custom_build/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 13:23:49.000000 actionlint_py-1.6.25.9/_custom_build/VERSION_ACTIONLINT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-25 13:23:49.000000 actionlint_py-1.6.25.9/_custom_build/VERSION_BUILD_SYSTEM.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-25 13:23:49.000000 actionlint_py-1.6.25.9/_custom_build/VERSION_DEV.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-25 13:23:49.000000 actionlint_py-1.6.25.9/_custom_build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-25 13:23:49.000000 actionlint_py-1.6.25.9/_custom_build/auto_update_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-25 13:23:49.000000 actionlint_py-1.6.25.9/_custom_build/checksums.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:24:08.665554 actionlint_py-1.6.25.9/_custom_build/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-25 13:23:49.000000 actionlint_py-1.6.25.9/_custom_build/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-25 13:23:49.000000 actionlint_py-1.6.25.9/_custom_build/commands/bdist_wheel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-25 13:23:49.000000 actionlint_py-1.6.25.9/_custom_build/commands/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-25 13:23:49.000000 actionlint_py-1.6.25.9/_custom_build/commands/fetch_binaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-25 13:23:49.000000 actionlint_py-1.6.25.9/_custom_build/commands/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-25 13:23:49.000000 actionlint_py-1.6.25.9/_custom_build/commands/install_actionlint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:24:08.665554 actionlint_py-1.6.25.9/_custom_build/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:23:49.000000 actionlint_py-1.6.25.9/_custom_build/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-25 13:23:49.000000 actionlint_py-1.6.25.9/_custom_build/utils/file_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-25 13:23:49.000000 actionlint_py-1.6.25.9/_custom_build/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:24:08.665554 actionlint_py-1.6.25.9/actionlint_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-25 13:24:08.000000 actionlint_py-1.6.25.9/actionlint_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-25 13:24:08.000000 actionlint_py-1.6.25.9/actionlint_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 13:24:08.000000 actionlint_py-1.6.25.9/actionlint_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-25 13:24:08.000000 actionlint_py-1.6.25.9/actionlint_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 13:24:08.000000 actionlint_py-1.6.25.9/actionlint_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-25 13:23:49.000000 actionlint_py-1.6.25.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 13:24:08.669554 actionlint_py-1.6.25.9/setup.cfg
```

### Comparing `actionlint_py-1.6.25.8/LICENSE` & `actionlint_py-1.6.25.9/LICENSE`

 * *Files identical despite different names*

### Comparing `actionlint_py-1.6.25.8/PKG-INFO` & `actionlint_py-1.6.25.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actionlint_py
-Version: 1.6.25.8
+Version: 1.6.25.9
 Summary: Python wrapper around invoking actionlint (https://github.com/rhysd/actionlint)
 Author-email: Ryan Rhee <pypi@rhee.io>, Mateusz Grzeliński <grzelinskimat@gmail.com>
 Maintainer-email: Mateusz Grzeliński <grzelinskimat@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Ryan Rhee
         
@@ -62,32 +62,32 @@
 
 See [pre-commit] for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 - repo: https://github.com/Mateusz-Grzelinski/actionlint-py
-  rev: v1.6.25.5
+  rev: v1.6.25.9
   hooks:
     - id: actionlint
 ```
 
 Because `actionlint-py` is available as source distribution, pip build system is set up to fetch binary from (public)
 github. It might cause problems with corporate proxy. In case of problems try this semi-manual setup:
 
 ```yaml
 - repo: local
   hooks:
     - id: actionlint
       name: actionlint
       description: Lint GitHub workflows with actionlint
       additional_dependencies: [ actionlint-py ]
-      #additional_dependencies: [actionlint-py==1.6.25.5]
+      #additional_dependencies: [actionlint-py==1.6.25.9]
       # safer, but pre-commit autoupdate will not work
-      # note: the versioning scheme is different: not "v1.6.25" but "1.6.25.2" (last number is build system version)
+      # note: the versioning scheme is different: not "v1.6.25" but "1.6.25.9" (last number is build system version)
       entry: actionlint
       #args: [-ignore "*.set-output. was depracated.*"]
       language: python
       types: [ "yaml" ]
       files: "^.github/workflows/"
 ```
```

### Comparing `actionlint_py-1.6.25.8/README.md` & `actionlint_py-1.6.25.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,32 +20,32 @@
 
 See [pre-commit] for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 - repo: https://github.com/Mateusz-Grzelinski/actionlint-py
-  rev: v1.6.25.5
+  rev: v1.6.25.9
   hooks:
     - id: actionlint
 ```
 
 Because `actionlint-py` is available as source distribution, pip build system is set up to fetch binary from (public)
 github. It might cause problems with corporate proxy. In case of problems try this semi-manual setup:
 
 ```yaml
 - repo: local
   hooks:
     - id: actionlint
       name: actionlint
       description: Lint GitHub workflows with actionlint
       additional_dependencies: [ actionlint-py ]
-      #additional_dependencies: [actionlint-py==1.6.25.5]
+      #additional_dependencies: [actionlint-py==1.6.25.9]
       # safer, but pre-commit autoupdate will not work
-      # note: the versioning scheme is different: not "v1.6.25" but "1.6.25.2" (last number is build system version)
+      # note: the versioning scheme is different: not "v1.6.25" but "1.6.25.9" (last number is build system version)
       entry: actionlint
       #args: [-ignore "*.set-output. was depracated.*"]
       language: python
       types: [ "yaml" ]
       files: "^.github/workflows/"
 ```
```

### Comparing `actionlint_py-1.6.25.8/_custom_build/auto_update_main.py` & `actionlint_py-1.6.25.9/_custom_build/auto_update_main.py`

 * *Files identical despite different names*

### Comparing `actionlint_py-1.6.25.8/_custom_build/checksums.cfg` & `actionlint_py-1.6.25.9/_custom_build/checksums.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 [linux-x86_64]
 file_name = actionlint_1.6.25_linux_amd64.tar.gz
 checksum = 80a54660e73ad55a0818372bdaa0dced82eb86f618e6bf1621e73f099e61c027
 url = https://github.com/rhysd/actionlint/releases/download/v1.6.25/actionlint_1.6.25_linux_amd64.tar.gz
 
+[linux-arm64]
+file_name = actionlint_1.6.25_linux_arm64.tar.gz
+checksum = 8bedeea8ed636891fd7351fa7ccbc75fdb5bee6efde5320162f712e8457e73ea
+url = https://github.com/rhysd/actionlint/releases/download/v1.6.25/actionlint_1.6.25_linux_arm64.tar.gz
+
 [darwin-x86_64]
 file_name = actionlint_1.6.25_darwin_amd64.tar.gz
 checksum = 30d69622ff9fbf564081515bf7d20538f2cb590150ef0c69fdcc56fa23fe85f1
 url = https://github.com/rhysd/actionlint/releases/download/v1.6.25/actionlint_1.6.25_darwin_amd64.tar.gz
 
 [darwin-arm64]
-file_name = actionlint_1.6.25_darwin_armv6.tar.gz
-checksum = 79180b0d572a4154965c0bcdb3ab3a37ca24b6d254192932ec7ca39128ceac5a
-url = https://github.com/rhysd/actionlint/releases/download/v1.6.25/actionlint_1.6.25_linux_armv6.tar.gz
+file_name =  actionlint_1.6.25_darwin_arm64.tar.gz
+checksum = 9153ebe7be2a33c9047e60aeb0d8d7b831b22fe99bbea63d365500c68245d6df
+url = https://github.com/rhysd/actionlint/releases/download/v1.6.25/actionlint_1.6.25_darwin_arm64.tar.gz
 
 [win32-AMD64]
 file_name = actionlint_1.6.25_windows_amd64.zip
 checksum = 8f572a723f362f2ab05777aad0c85322fecf130e6ff0ca8ca0a6fb3a3414ac1b
 url = https://github.com/rhysd/actionlint/releases/download/v1.6.25/actionlint_1.6.25_windows_amd64.zip
 
 [cygwin-x86_64]
```

### Comparing `actionlint_py-1.6.25.8/_custom_build/commands/fetch_binaries.py` & `actionlint_py-1.6.25.9/_custom_build/commands/fetch_binaries.py`

 * *Files identical despite different names*

### Comparing `actionlint_py-1.6.25.8/_custom_build/commands/install_actionlint.py` & `actionlint_py-1.6.25.9/_custom_build/commands/install_actionlint.py`

 * *Files identical despite different names*

### Comparing `actionlint_py-1.6.25.8/_custom_build/utils/file_ops.py` & `actionlint_py-1.6.25.9/_custom_build/utils/file_ops.py`

 * *Files identical despite different names*

### Comparing `actionlint_py-1.6.25.8/_custom_build/version.py` & `actionlint_py-1.6.25.9/_custom_build/version.py`

 * *Files identical despite different names*

### Comparing `actionlint_py-1.6.25.8/actionlint_py.egg-info/PKG-INFO` & `actionlint_py-1.6.25.9/actionlint_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actionlint-py
-Version: 1.6.25.8
+Version: 1.6.25.9
 Summary: Python wrapper around invoking actionlint (https://github.com/rhysd/actionlint)
 Author-email: Ryan Rhee <pypi@rhee.io>, Mateusz Grzeliński <grzelinskimat@gmail.com>
 Maintainer-email: Mateusz Grzeliński <grzelinskimat@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Ryan Rhee
         
@@ -62,32 +62,32 @@
 
 See [pre-commit] for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 - repo: https://github.com/Mateusz-Grzelinski/actionlint-py
-  rev: v1.6.25.5
+  rev: v1.6.25.9
   hooks:
     - id: actionlint
 ```
 
 Because `actionlint-py` is available as source distribution, pip build system is set up to fetch binary from (public)
 github. It might cause problems with corporate proxy. In case of problems try this semi-manual setup:
 
 ```yaml
 - repo: local
   hooks:
     - id: actionlint
       name: actionlint
       description: Lint GitHub workflows with actionlint
       additional_dependencies: [ actionlint-py ]
-      #additional_dependencies: [actionlint-py==1.6.25.5]
+      #additional_dependencies: [actionlint-py==1.6.25.9]
       # safer, but pre-commit autoupdate will not work
-      # note: the versioning scheme is different: not "v1.6.25" but "1.6.25.2" (last number is build system version)
+      # note: the versioning scheme is different: not "v1.6.25" but "1.6.25.9" (last number is build system version)
       entry: actionlint
       #args: [-ignore "*.set-output. was depracated.*"]
       language: python
       types: [ "yaml" ]
       files: "^.github/workflows/"
 ```
```

### Comparing `actionlint_py-1.6.25.8/actionlint_py.egg-info/SOURCES.txt` & `actionlint_py-1.6.25.9/actionlint_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `actionlint_py-1.6.25.8/pyproject.toml` & `actionlint_py-1.6.25.9/pyproject.toml`

 * *Files identical despite different names*

