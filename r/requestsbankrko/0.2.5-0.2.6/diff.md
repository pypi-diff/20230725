# Comparing `tmp/requestsbankrko-0.2.5.tar.gz` & `tmp/requestsbankrko-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requestsbankrko-0.2.5.tar", last modified: Thu Jul 20 11:05:09 2023, max compression
+gzip compressed data, was "requestsbankrko-0.2.6.tar", last modified: Tue Jul 25 06:08:29 2023, max compression
```

## Comparing `requestsbankrko-0.2.5.tar` & `requestsbankrko-0.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:05:09.644488 requestsbankrko-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-20 11:04:57.000000 requestsbankrko-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-20 11:05:09.644488 requestsbankrko-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-20 11:04:57.000000 requestsbankrko-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-20 11:04:57.000000 requestsbankrko-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 11:05:09.644488 requestsbankrko-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:05:09.644488 requestsbankrko-0.2.5/src/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 11:04:57.000000 requestsbankrko-0.2.5/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29207 2023-07-20 11:04:57.000000 requestsbankrko-0.2.5/src/bank_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-20 11:04:57.000000 requestsbankrko-0.2.5/src/open_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:05:09.644488 requestsbankrko-0.2.5/src/requestsbankrko.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-20 11:05:09.000000 requestsbankrko-0.2.5/src/requestsbankrko.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-20 11:05:09.000000 requestsbankrko-0.2.5/src/requestsbankrko.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 11:05:09.000000 requestsbankrko-0.2.5/src/requestsbankrko.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-20 11:05:09.000000 requestsbankrko-0.2.5/src/requestsbankrko.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-20 11:05:09.000000 requestsbankrko-0.2.5/src/requestsbankrko.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-20 11:04:57.000000 requestsbankrko-0.2.5/src/zip_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:05:09.644488 requestsbankrko-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    56968 2023-07-20 11:04:57.000000 requestsbankrko-0.2.5/tests/test_bank_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:08:29.312160 requestsbankrko-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-25 06:08:16.000000 requestsbankrko-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-25 06:08:29.312160 requestsbankrko-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-25 06:08:16.000000 requestsbankrko-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-25 06:08:16.000000 requestsbankrko-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 06:08:29.312160 requestsbankrko-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:08:29.312160 requestsbankrko-0.2.6/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:08:16.000000 requestsbankrko-0.2.6/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29322 2023-07-25 06:08:16.000000 requestsbankrko-0.2.6/src/bank_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-25 06:08:16.000000 requestsbankrko-0.2.6/src/open_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:08:29.312160 requestsbankrko-0.2.6/src/requestsbankrko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-25 06:08:29.000000 requestsbankrko-0.2.6/src/requestsbankrko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-25 06:08:29.000000 requestsbankrko-0.2.6/src/requestsbankrko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:08:29.000000 requestsbankrko-0.2.6/src/requestsbankrko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-25 06:08:29.000000 requestsbankrko-0.2.6/src/requestsbankrko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-25 06:08:29.000000 requestsbankrko-0.2.6/src/requestsbankrko.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-25 06:08:16.000000 requestsbankrko-0.2.6/src/zip_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:08:29.312160 requestsbankrko-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    57078 2023-07-25 06:08:16.000000 requestsbankrko-0.2.6/tests/test_bank_methods.py
```

### Comparing `requestsbankrko-0.2.5/LICENSE` & `requestsbankrko-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `requestsbankrko-0.2.5/PKG-INFO` & `requestsbankrko-0.2.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requestsbankrko
-Version: 0.2.5
+Version: 0.2.6
 Summary: Гарантированно успешные web-запросы в Банки РКО
 Author-email: plp-kolyan <plp-kolyan@mail.ru>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -31,15 +31,15 @@
 License-File: LICENSE
 
 # requestsbankrko
 
 
 Доки тут
 [Домашняя страница](https://github.com/plp-kolyan/requestsbankrko.git)
-
+This library is designed to fulfill requests to affiliate programs of banks and accounting services
```

### Comparing `requestsbankrko-0.2.5/pyproject.toml` & `requestsbankrko-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "requestsbankrko"
-version = "0.2.5"
+version = "0.2.6"
 description = "Гарантированно успешные web-запросы в Банки РКО"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
 dependencies = [ "requestsgarant>=0.0.7", "requests>=2.28", "jsoncustom>=0.0.2", "python-dotenv>=0.20.0",]
 [[project.authors]]
 name = "plp-kolyan"
```

### Comparing `requestsbankrko-0.2.5/src/bank_methods.py` & `requestsbankrko-0.2.6/src/bank_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -898,7 +898,13 @@
         self.method = 'post'
 
 
     def suc_resp(self):
         return self.prospective_sale_id
 
 
+def mutation_inn(inn: str):
+    inn = str(inn)
+    if len(inn) in [9, 11]:
+        inn = '0' + inn
+    return inn
+
```

### Comparing `requestsbankrko-0.2.5/src/open_methods.py` & `requestsbankrko-0.2.6/src/open_methods.py`

 * *Files identical despite different names*

### Comparing `requestsbankrko-0.2.5/src/requestsbankrko.egg-info/PKG-INFO` & `requestsbankrko-0.2.6/src/requestsbankrko.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requestsbankrko
-Version: 0.2.5
+Version: 0.2.6
 Summary: Гарантированно успешные web-запросы в Банки РКО
 Author-email: plp-kolyan <plp-kolyan@mail.ru>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -31,15 +31,15 @@
 License-File: LICENSE
 
 # requestsbankrko
 
 
 Доки тут
 [Домашняя страница](https://github.com/plp-kolyan/requestsbankrko.git)
-
+This library is designed to fulfill requests to affiliate programs of banks and accounting services
```

### Comparing `requestsbankrko-0.2.5/src/zip_functions.py` & `requestsbankrko-0.2.6/src/zip_functions.py`

 * *Files identical despite different names*

### Comparing `requestsbankrko-0.2.5/tests/test_bank_methods.py` & `requestsbankrko-0.2.6/tests/test_bank_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -1384,7 +1384,12 @@
         #             ]
         #         }
         #     ],
         #     "InternalProductId": "Evrika",
 
         # }
         print(KonturProspectiveSales(json, True).get_rezult())
+
+class DevelopTest(TestCase):
+    def test_0(self):
+        inn = '800009370'
+        print(mutation_inn(inn))
```

