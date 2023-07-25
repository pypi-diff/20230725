# Comparing `tmp/types-Send2Trash-1.8.2.6.tar.gz` & `tmp/types-Send2Trash-1.8.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-Send2Trash-1.8.2.6.tar", last modified: Thu Jul 20 15:19:52 2023, max compression
+gzip compressed data, was "types-Send2Trash-1.8.2.7.tar", last modified: Tue Jul 25 12:31:39 2023, max compression
```

## Comparing `types-Send2Trash-1.8.2.6.tar` & `types-Send2Trash-1.8.2.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:52.371831 types-Send2Trash-1.8.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-20 15:19:51.000000 types-Send2Trash-1.8.2.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:19:51.000000 types-Send2Trash-1.8.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-20 15:19:52.371831 types-Send2Trash-1.8.2.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:52.367831 types-Send2Trash-1.8.2.6/send2trash-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-20 15:19:51.000000 types-Send2Trash-1.8.2.6/send2trash-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-20 15:15:13.000000 types-Send2Trash-1.8.2.6/send2trash-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-20 15:15:13.000000 types-Send2Trash-1.8.2.6/send2trash-stubs/compat.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-20 15:15:13.000000 types-Send2Trash-1.8.2.6/send2trash-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-20 15:15:13.000000 types-Send2Trash-1.8.2.6/send2trash-stubs/util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:19:52.371831 types-Send2Trash-1.8.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-20 15:19:51.000000 types-Send2Trash-1.8.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:52.371831 types-Send2Trash-1.8.2.6/types_Send2Trash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-20 15:19:52.000000 types-Send2Trash-1.8.2.6/types_Send2Trash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-20 15:19:52.000000 types-Send2Trash-1.8.2.6/types_Send2Trash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:19:52.000000 types-Send2Trash-1.8.2.6/types_Send2Trash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-20 15:19:52.000000 types-Send2Trash-1.8.2.6/types_Send2Trash.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:31:39.378299 types-Send2Trash-1.8.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-25 12:31:37.000000 types-Send2Trash-1.8.2.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-25 12:31:37.000000 types-Send2Trash-1.8.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-25 12:31:39.378299 types-Send2Trash-1.8.2.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:31:39.374299 types-Send2Trash-1.8.2.7/send2trash-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-25 12:31:37.000000 types-Send2Trash-1.8.2.7/send2trash-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-25 12:31:20.000000 types-Send2Trash-1.8.2.7/send2trash-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-25 12:31:20.000000 types-Send2Trash-1.8.2.7/send2trash-stubs/__main__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-25 12:31:20.000000 types-Send2Trash-1.8.2.7/send2trash-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-25 12:31:20.000000 types-Send2Trash-1.8.2.7/send2trash-stubs/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 12:31:39.378299 types-Send2Trash-1.8.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-25 12:31:37.000000 types-Send2Trash-1.8.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:31:39.378299 types-Send2Trash-1.8.2.7/types_Send2Trash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-25 12:31:39.000000 types-Send2Trash-1.8.2.7/types_Send2Trash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-25 12:31:39.000000 types-Send2Trash-1.8.2.7/types_Send2Trash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 12:31:39.000000 types-Send2Trash-1.8.2.7/types_Send2Trash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-25 12:31:39.000000 types-Send2Trash-1.8.2.7/types_Send2Trash.egg-info/top_level.txt
```

### Comparing `types-Send2Trash-1.8.2.6/CHANGELOG.md` & `types-Send2Trash-1.8.2.7/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 1.8.2.7 (2023-07-25)
+
+Complete send2trash stubs (#10504)
+
 ## 1.8.2.6 (2023-07-20)
 
 Add an upstream_repository field to METADATA.toml (#10487)
 
 Closes: #10478
 
 ## 1.8.2.5 (2023-05-10)
```

### Comparing `types-Send2Trash-1.8.2.6/PKG-INFO` & `types-Send2Trash-1.8.2.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Send2Trash
-Version: 1.8.2.6
+Version: 1.8.2.7
 Summary: Typing stubs for Send2Trash
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Send2Trash.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,15 +21,11 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `Send2Trash`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/Send2Trash. All fixes for
 types and metadata should be contributed there.
 
-This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
-If you find that annotations are missing, feel free to contribute and help complete them.
-
-
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+This package was generated from typeshed commit `38dc97ba717c55c4c833f04c4bc9665f0a44fe7a` and was tested
 with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+pytype 2023.7.21.
```

### Comparing `types-Send2Trash-1.8.2.6/setup.py` & `types-Send2Trash-1.8.2.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,39 +11,35 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `Send2Trash`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/Send2Trash. All fixes for
 types and metadata should be contributed there.
 
-This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
-If you find that annotations are missing, feel free to contribute and help complete them.
-
-
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+This package was generated from typeshed commit `38dc97ba717c55c4c833f04c4bc9665f0a44fe7a` and was tested
 with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+pytype 2023.7.21.
 '''.lstrip()
 
 setup(name=name,
-      version="1.8.2.6",
+      version="1.8.2.7",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Send2Trash.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['send2trash-stubs'],
-      package_data={'send2trash-stubs': ['__init__.pyi', 'compat.pyi', 'exceptions.pyi', 'util.pyi', 'METADATA.toml', 'py.typed']},
+      package_data={'send2trash-stubs': ['__init__.pyi', '__main__.pyi', 'exceptions.pyi', 'util.pyi', 'METADATA.toml']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-Send2Trash-1.8.2.6/types_Send2Trash.egg-info/PKG-INFO` & `types-Send2Trash-1.8.2.7/types_Send2Trash.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Send2Trash
-Version: 1.8.2.6
+Version: 1.8.2.7
 Summary: Typing stubs for Send2Trash
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Send2Trash.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,15 +21,11 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `Send2Trash`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/Send2Trash. All fixes for
 types and metadata should be contributed there.
 
-This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
-If you find that annotations are missing, feel free to contribute and help complete them.
-
-
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+This package was generated from typeshed commit `38dc97ba717c55c4c833f04c4bc9665f0a44fe7a` and was tested
 with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+pytype 2023.7.21.
```

