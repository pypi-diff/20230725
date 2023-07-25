# Comparing `tmp/vdk-greenplum-0.0.824443273.tar.gz` & `tmp/vdk-greenplum-0.0.944393829.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-greenplum-0.0.824443273.tar", last modified: Fri Mar 31 14:25:03 2023, max compression
+gzip compressed data, was "vdk-greenplum-0.0.944393829.tar", last modified: Tue Jul 25 09:01:00 2023, max compression
```

## Comparing `vdk-greenplum-0.0.824443273.tar` & `vdk-greenplum-0.0.944393829.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:03.341968 vdk-greenplum-0.0.824443273/
--rw-r--r--   0 root         (0) root         (0)     2268 2023-03-31 14:25:03.341968 vdk-greenplum-0.0.824443273/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1629 2023-03-31 14:24:51.000000 vdk-greenplum-0.0.824443273/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-31 14:25:03.341968 vdk-greenplum-0.0.824443273/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1169 2023-03-31 14:24:55.000000 vdk-greenplum-0.0.824443273/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:03.341968 vdk-greenplum-0.0.824443273/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:03.341968 vdk-greenplum-0.0.824443273/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:03.341968 vdk-greenplum-0.0.824443273/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:03.341968 vdk-greenplum-0.0.824443273/src/vdk/plugin/greenplum/
--rw-rw-rw-   0 root         (0) root         (0)     3864 2023-03-31 14:24:51.000000 vdk-greenplum-0.0.824443273/src/vdk/plugin/greenplum/greenplum_connection.py
--rw-rw-rw-   0 root         (0) root         (0)     2854 2023-03-31 14:24:51.000000 vdk-greenplum-0.0.824443273/src/vdk/plugin/greenplum/greenplum_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     3450 2023-03-31 14:24:51.000000 vdk-greenplum-0.0.824443273/src/vdk/plugin/greenplum/ingest_to_greenplum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:03.341968 vdk-greenplum-0.0.824443273/src/vdk_greenplum.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2268 2023-03-31 14:25:03.000000 vdk-greenplum-0.0.824443273/src/vdk_greenplum.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      476 2023-03-31 14:25:03.000000 vdk-greenplum-0.0.824443273/src/vdk_greenplum.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 14:25:03.000000 vdk-greenplum-0.0.824443273/src/vdk_greenplum.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-03-31 14:25:03.000000 vdk-greenplum-0.0.824443273/src/vdk_greenplum.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-03-31 14:25:03.000000 vdk-greenplum-0.0.824443273/src/vdk_greenplum.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-31 14:25:03.000000 vdk-greenplum-0.0.824443273/src/vdk_greenplum.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:03.341968 vdk-greenplum-0.0.824443273/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3014 2023-03-31 14:24:51.000000 vdk-greenplum-0.0.824443273/tests/test_ingest_to_greenplum.py
--rw-rw-rw-   0 root         (0) root         (0)     1588 2023-03-31 14:24:51.000000 vdk-greenplum-0.0.824443273/tests/test_vdk_greenplum_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:00.249370 vdk-greenplum-0.0.944393829/
+-rw-r--r--   0 root         (0) root         (0)     2268 2023-07-25 09:01:00.249370 vdk-greenplum-0.0.944393829/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1629 2023-07-25 09:00:42.000000 vdk-greenplum-0.0.944393829/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 09:01:00.249370 vdk-greenplum-0.0.944393829/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2023-07-25 09:00:46.000000 vdk-greenplum-0.0.944393829/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:00.245370 vdk-greenplum-0.0.944393829/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:00.245370 vdk-greenplum-0.0.944393829/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:00.245370 vdk-greenplum-0.0.944393829/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:00.249370 vdk-greenplum-0.0.944393829/src/vdk/plugin/greenplum/
+-rw-rw-rw-   0 root         (0) root         (0)     3864 2023-07-25 09:00:42.000000 vdk-greenplum-0.0.944393829/src/vdk/plugin/greenplum/greenplum_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     2854 2023-07-25 09:00:42.000000 vdk-greenplum-0.0.944393829/src/vdk/plugin/greenplum/greenplum_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3450 2023-07-25 09:00:42.000000 vdk-greenplum-0.0.944393829/src/vdk/plugin/greenplum/ingest_to_greenplum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:00.249370 vdk-greenplum-0.0.944393829/src/vdk_greenplum.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2268 2023-07-25 09:01:00.000000 vdk-greenplum-0.0.944393829/src/vdk_greenplum.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      476 2023-07-25 09:01:00.000000 vdk-greenplum-0.0.944393829/src/vdk_greenplum.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 09:01:00.000000 vdk-greenplum-0.0.944393829/src/vdk_greenplum.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-07-25 09:01:00.000000 vdk-greenplum-0.0.944393829/src/vdk_greenplum.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-07-25 09:01:00.000000 vdk-greenplum-0.0.944393829/src/vdk_greenplum.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-25 09:01:00.000000 vdk-greenplum-0.0.944393829/src/vdk_greenplum.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:01:00.249370 vdk-greenplum-0.0.944393829/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3014 2023-07-25 09:00:42.000000 vdk-greenplum-0.0.944393829/tests/test_ingest_to_greenplum.py
+-rw-rw-rw-   0 root         (0) root         (0)     1588 2023-07-25 09:00:42.000000 vdk-greenplum-0.0.944393829/tests/test_vdk_greenplum_utils.py
```

### Comparing `vdk-greenplum-0.0.824443273/PKG-INFO` & `vdk-greenplum-0.0.944393829/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-greenplum
-Version: 0.0.824443273
+Version: 0.0.944393829
 Summary: Versatile Data Kit SDK plugin provides support for Greenplum database and greenplum transformation templates.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-greenplum-0.0.824443273/README.md` & `vdk-greenplum-0.0.944393829/README.md`

 * *Files identical despite different names*

### Comparing `vdk-greenplum-0.0.824443273/setup.py` & `vdk-greenplum-0.0.944393829/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.0.824443273"
+__version__ = "0.0.944393829"
 
 setuptools.setup(
     name="vdk-greenplum",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK plugin provides support for Greenplum database and greenplum transformation templates.",
     long_description=pathlib.Path("README.md").read_text(),
     long_description_content_type="text/markdown",
-    install_requires=["vdk-core", "psycopg2-binary"],
+    install_requires=["vdk-core", "psycopg2-binary", "tabulate"],
     package_dir={"": "src"},
     packages=setuptools.find_namespace_packages(where="src"),
     include_package_data=True,
     entry_points={
         "vdk.plugin.run": ["vdk-greenplum = vdk.plugin.greenplum.greenplum_plugin"]
     },
     classifiers=[
```

### Comparing `vdk-greenplum-0.0.824443273/src/vdk/plugin/greenplum/greenplum_connection.py` & `vdk-greenplum-0.0.944393829/src/vdk/plugin/greenplum/greenplum_connection.py`

 * *Files identical despite different names*

### Comparing `vdk-greenplum-0.0.824443273/src/vdk/plugin/greenplum/greenplum_plugin.py` & `vdk-greenplum-0.0.944393829/src/vdk/plugin/greenplum/greenplum_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-greenplum-0.0.824443273/src/vdk/plugin/greenplum/ingest_to_greenplum.py` & `vdk-greenplum-0.0.944393829/src/vdk/plugin/greenplum/ingest_to_greenplum.py`

 * *Files identical despite different names*

### Comparing `vdk-greenplum-0.0.824443273/src/vdk_greenplum.egg-info/PKG-INFO` & `vdk-greenplum-0.0.944393829/src/vdk_greenplum.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-greenplum
-Version: 0.0.824443273
+Version: 0.0.944393829
 Summary: Versatile Data Kit SDK plugin provides support for Greenplum database and greenplum transformation templates.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-greenplum-0.0.824443273/tests/test_ingest_to_greenplum.py` & `vdk-greenplum-0.0.944393829/tests/test_ingest_to_greenplum.py`

 * *Files identical despite different names*

### Comparing `vdk-greenplum-0.0.824443273/tests/test_vdk_greenplum_utils.py` & `vdk-greenplum-0.0.944393829/tests/test_vdk_greenplum_utils.py`

 * *Files identical despite different names*

