# Comparing `tmp/acquire-3.8.dev8.tar.gz` & `tmp/acquire-3.8.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acquire-3.8.dev8.tar", last modified: Wed Jul 19 14:27:54 2023, max compression
+gzip compressed data, was "acquire-3.8.dev9.tar", last modified: Tue Jul 25 07:50:28 2023, max compression
```

## Comparing `acquire-3.8.dev8.tar` & `acquire-3.8.dev9.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:54.183662 acquire-3.8.dev8/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-19 14:27:23.000000 acquire-3.8.dev8/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-19 14:27:23.000000 acquire-3.8.dev8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-19 14:27:23.000000 acquire-3.8.dev8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-19 14:27:54.183662 acquire-3.8.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-19 14:27:23.000000 acquire-3.8.dev8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:54.163662 acquire-3.8.dev8/acquire/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79835 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/acquire.py
--rw-r--r--   0 runner    (1001) docker     (123)    21648 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:54.167662 acquire-3.8.dev8/acquire/dynamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/dynamic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:54.167662 acquire-3.8.dev8/acquire/dynamic/windows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/dynamic/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/dynamic/windows/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/dynamic/windows/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/dynamic/windows/handles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/dynamic/windows/named_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/dynamic/windows/ntdll.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/dynamic/windows/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/esxi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:54.171662 acquire-3.8.dev8/acquire/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/outputs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/outputs/dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/outputs/tar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:54.171662 acquire-3.8.dev8/acquire/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15901 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/tools/decrypter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:54.175662 acquire-3.8.dev8/acquire/uploaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/uploaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/uploaders/minio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/uploaders/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/uploaders/plugin_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-07-19 14:27:23.000000 acquire-3.8.dev8/acquire/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-19 14:27:53.000000 acquire-3.8.dev8/acquire/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:54.163662 acquire-3.8.dev8/acquire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-19 14:27:54.000000 acquire-3.8.dev8/acquire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-19 14:27:54.000000 acquire-3.8.dev8/acquire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 14:27:54.000000 acquire-3.8.dev8/acquire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-19 14:27:54.000000 acquire-3.8.dev8/acquire.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-19 14:27:54.000000 acquire-3.8.dev8/acquire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-19 14:27:54.000000 acquire-3.8.dev8/acquire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-19 14:27:40.000000 acquire-3.8.dev8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 14:27:54.183662 acquire-3.8.dev8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:54.183662 acquire-3.8.dev8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:27:54.183662 acquire-3.8.dev8/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tests/test_acquire_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tests/test_acquire_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tests/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tests/test_decryptor_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tests/test_esxi_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tests/test_file_sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tests/test_minio_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tests/test_misc_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-19 14:27:23.000000 acquire-3.8.dev8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:50:28.230328 acquire-3.8.dev9/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-25 07:50:13.000000 acquire-3.8.dev9/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-25 07:50:13.000000 acquire-3.8.dev9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-25 07:50:13.000000 acquire-3.8.dev9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-25 07:50:28.230328 acquire-3.8.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-25 07:50:13.000000 acquire-3.8.dev9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:50:28.222328 acquire-3.8.dev9/acquire/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:50:13.000000 acquire-3.8.dev9/acquire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80067 2023-07-25 07:50:13.000000 acquire-3.8.dev9/acquire/acquire.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21648 2023-07-25 07:50:13.000000 acquire-3.8.dev9/acquire/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-25 07:50:13.000000 acquire-3.8.dev9/acquire/crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:50:28.222328 acquire-3.8.dev9/acquire/dynamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:50:13.000000 acquire-3.8.dev9/acquire/dynamic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:50:28.226328 acquire-3.8.dev9/acquire/dynamic/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:50:13.000000 acquire-3.8.dev9/acquire/dynamic/windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-25 07:50:13.000000 acquire-3.8.dev9/acquire/dynamic/windows/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-25 07:50:13.000000 acquire-3.8.dev9/acquire/dynamic/windows/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-07-25 07:50:13.000000 acquire-3.8.dev9/acquire/dynamic/windows/handles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-25 07:50:13.000000 acquire-3.8.dev9/acquire/dynamic/windows/named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-25 07:50:13.000000 acquire-3.8.dev9/acquire/dynamic/windows/ntdll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-25 07:50:13.000000 acquire-3.8.dev9/acquire/dynamic/windows/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-25 07:50:13.000000 acquire-3.8.dev9/acquire/esxi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-07-25 07:50:13.000000 acquire-3.8.dev9/acquire/hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-07-25 07:50:13.000000 acquire-3.8.dev9/acquire/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:50:28.226328 acquire-3.8.dev9/acquire/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-25 07:50:13.000000 acquire-3.8.dev9/acquire/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-25 07:50:13.000000 acquire-3.8.dev9/acquire/outputs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-25 07:50:13.000000 acquire-3.8.dev9/acquire/outputs/dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-25 07:50:13.000000 acquire-3.8.dev9/acquire/outputs/tar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:50:28.226328 acquire-3.8.dev9/acquire/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:50:13.000000 acquire-3.8.dev9/acquire/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15901 2023-07-25 07:50:13.000000 acquire-3.8.dev9/acquire/tools/decrypter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:50:28.226328 acquire-3.8.dev9/acquire/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:50:13.000000 acquire-3.8.dev9/acquire/uploaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-25 07:50:13.000000 acquire-3.8.dev9/acquire/uploaders/minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-25 07:50:13.000000 acquire-3.8.dev9/acquire/uploaders/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-25 07:50:13.000000 acquire-3.8.dev9/acquire/uploaders/plugin_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-07-25 07:50:13.000000 acquire-3.8.dev9/acquire/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-25 07:50:28.000000 acquire-3.8.dev9/acquire/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:50:28.222328 acquire-3.8.dev9/acquire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-25 07:50:28.000000 acquire-3.8.dev9/acquire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-25 07:50:28.000000 acquire-3.8.dev9/acquire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 07:50:28.000000 acquire-3.8.dev9/acquire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-25 07:50:28.000000 acquire-3.8.dev9/acquire.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-25 07:50:28.000000 acquire-3.8.dev9/acquire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-25 07:50:28.000000 acquire-3.8.dev9/acquire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-25 07:50:18.000000 acquire-3.8.dev9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 07:50:28.230328 acquire-3.8.dev9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:50:28.226328 acquire-3.8.dev9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:50:13.000000 acquire-3.8.dev9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-25 07:50:13.000000 acquire-3.8.dev9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:50:28.230328 acquire-3.8.dev9/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-25 07:50:13.000000 acquire-3.8.dev9/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-25 07:50:13.000000 acquire-3.8.dev9/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-25 07:50:13.000000 acquire-3.8.dev9/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-25 07:50:13.000000 acquire-3.8.dev9/tests/test_acquire_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-25 07:50:13.000000 acquire-3.8.dev9/tests/test_acquire_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-07-25 07:50:13.000000 acquire-3.8.dev9/tests/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-25 07:50:13.000000 acquire-3.8.dev9/tests/test_decryptor_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-25 07:50:13.000000 acquire-3.8.dev9/tests/test_esxi_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-25 07:50:13.000000 acquire-3.8.dev9/tests/test_file_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-25 07:50:13.000000 acquire-3.8.dev9/tests/test_minio_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-25 07:50:13.000000 acquire-3.8.dev9/tests/test_misc_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-25 07:50:13.000000 acquire-3.8.dev9/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-07-25 07:50:13.000000 acquire-3.8.dev9/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-25 07:50:13.000000 acquire-3.8.dev9/tox.ini
```

### Comparing `acquire-3.8.dev8/LICENSE` & `acquire-3.8.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/PKG-INFO` & `acquire-3.8.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acquire
-Version: 3.8.dev8
+Version: 3.8.dev9
 Summary: A tool to quickly gather forensic artifacts from disk images or a live system into a lightweight container
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/acquire
 Project-URL: repository, https://github.com/fox-it/acquire
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `acquire-3.8.dev8/README.md` & `acquire-3.8.dev9/README.md`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/acquire/acquire.py` & `acquire-3.8.dev9/acquire/acquire.py`

 * *Files 1% similar despite different names*

```diff
@@ -621,15 +621,18 @@
 
 @register_module("--recents")
 class Recents(Module):
     DESC = "Windows recently used files artifacts"
     SPEC = [
         ("dir", "AppData/Roaming/Microsoft/Windows/Recent", from_user_home),
         ("dir", "AppData/Roaming/Microsoft/Office/Recent", from_user_home),
+        ("glob", "AppData/Roaming/Microsoft/Windows/Start Menu/Programs/*.lnk", from_user_home),
+        ("glob", "Desktop/*.lnk", from_user_home),
         ("glob", "Recent/*.lnk", from_user_home),
+        ("glob", "sysvol/ProgramData/Microsoft/Windows/Start Menu/Programs/*.lnk"),
     ]
 
 
 @register_module("--recyclebin")
 class RecycleBin(Module):
     DESC = "recycle bin metadata"
```

### Comparing `acquire-3.8.dev8/acquire/collector.py` & `acquire-3.8.dev9/acquire/collector.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/acquire/crypt.py` & `acquire-3.8.dev9/acquire/crypt.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/acquire/dynamic/windows/collect.py` & `acquire-3.8.dev9/acquire/dynamic/windows/collect.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/acquire/dynamic/windows/handles.py` & `acquire-3.8.dev9/acquire/dynamic/windows/handles.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/acquire/dynamic/windows/named_objects.py` & `acquire-3.8.dev9/acquire/dynamic/windows/named_objects.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/acquire/dynamic/windows/ntdll.py` & `acquire-3.8.dev9/acquire/dynamic/windows/ntdll.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/acquire/dynamic/windows/types.py` & `acquire-3.8.dev9/acquire/dynamic/windows/types.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/acquire/esxi.py` & `acquire-3.8.dev9/acquire/esxi.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/acquire/hashes.py` & `acquire-3.8.dev9/acquire/hashes.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/acquire/log.py` & `acquire-3.8.dev9/acquire/log.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/acquire/outputs/base.py` & `acquire-3.8.dev9/acquire/outputs/base.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/acquire/outputs/dir.py` & `acquire-3.8.dev9/acquire/outputs/dir.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/acquire/outputs/tar.py` & `acquire-3.8.dev9/acquire/outputs/tar.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/acquire/tools/decrypter.py` & `acquire-3.8.dev9/acquire/tools/decrypter.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/acquire/uploaders/minio.py` & `acquire-3.8.dev9/acquire/uploaders/minio.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/acquire/uploaders/plugin.py` & `acquire-3.8.dev9/acquire/uploaders/plugin.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/acquire/uploaders/plugin_registry.py` & `acquire-3.8.dev9/acquire/uploaders/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/acquire/utils.py` & `acquire-3.8.dev9/acquire/utils.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/acquire.egg-info/PKG-INFO` & `acquire-3.8.dev9/acquire.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acquire
-Version: 3.8.dev8
+Version: 3.8.dev9
 Summary: A tool to quickly gather forensic artifacts from disk images or a live system into a lightweight container
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/acquire
 Project-URL: repository, https://github.com/fox-it/acquire
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `acquire-3.8.dev8/acquire.egg-info/SOURCES.txt` & `acquire-3.8.dev9/acquire.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/pyproject.toml` & `acquire-3.8.dev9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/tests/conftest.py` & `acquire-3.8.dev9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/tests/docs/Makefile` & `acquire-3.8.dev9/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/tests/docs/conf.py` & `acquire-3.8.dev9/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/tests/test_acquire_command.py` & `acquire-3.8.dev9/tests/test_acquire_command.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/tests/test_acquire_modules.py` & `acquire-3.8.dev9/tests/test_acquire_modules.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/tests/test_collector.py` & `acquire-3.8.dev9/tests/test_collector.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/tests/test_decryptor_funcs.py` & `acquire-3.8.dev9/tests/test_decryptor_funcs.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/tests/test_esxi_memory.py` & `acquire-3.8.dev9/tests/test_esxi_memory.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/tests/test_file_sorting.py` & `acquire-3.8.dev9/tests/test_file_sorting.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/tests/test_minio_uploader.py` & `acquire-3.8.dev9/tests/test_minio_uploader.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/tests/test_misc_users.py` & `acquire-3.8.dev9/tests/test_misc_users.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/tests/test_plugin.py` & `acquire-3.8.dev9/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/tests/test_utils.py` & `acquire-3.8.dev9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `acquire-3.8.dev8/tox.ini` & `acquire-3.8.dev9/tox.ini`

 * *Files identical despite different names*

