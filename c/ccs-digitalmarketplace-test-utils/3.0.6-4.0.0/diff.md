# Comparing `tmp/ccs-digitalmarketplace-test-utils-3.0.6.tar.gz` & `tmp/ccs-digitalmarketplace-test-utils-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccs-digitalmarketplace-test-utils-3.0.6.tar", last modified: Wed Feb  9 11:07:17 2022, max compression
+gzip compressed data, was "ccs-digitalmarketplace-test-utils-4.0.0.tar", last modified: Tue Jul 25 08:03:18 2023, max compression
```

## Comparing `ccs-digitalmarketplace-test-utils-3.0.6.tar` & `ccs-digitalmarketplace-test-utils-4.0.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 11:07:17.758664 ccs-digitalmarketplace-test-utils-3.0.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-02-09 11:07:06.000000 ccs-digitalmarketplace-test-utils-3.0.6/LICENCE
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-02-09 11:07:17.758664 ccs-digitalmarketplace-test-utils-3.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1404 2022-02-09 11:07:06.000000 ccs-digitalmarketplace-test-utils-3.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 11:07:17.754664 ccs-digitalmarketplace-test-utils-3.0.6/ccs_digitalmarketplace_test_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-02-09 11:07:17.000000 ccs-digitalmarketplace-test-utils-3.0.6/ccs_digitalmarketplace_test_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      916 2022-02-09 11:07:17.000000 ccs-digitalmarketplace-test-utils-3.0.6/ccs_digitalmarketplace_test_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-09 11:07:17.000000 ccs-digitalmarketplace-test-utils-3.0.6/ccs_digitalmarketplace_test_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-02-09 11:07:17.000000 ccs-digitalmarketplace-test-utils-3.0.6/ccs_digitalmarketplace_test_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-02-09 11:07:17.000000 ccs-digitalmarketplace-test-utils-3.0.6/ccs_digitalmarketplace_test_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 11:07:17.754664 ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-02-09 11:07:06.000000 ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 11:07:17.758664 ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/api_model_stubs/
--rw-r--r--   0 runner    (1001) docker     (121)      940 2022-02-09 11:07:06.000000 ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/api_model_stubs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-02-09 11:07:06.000000 ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/api_model_stubs/audit_event.py
--rw-r--r--   0 runner    (1001) docker     (121)     3172 2022-02-09 11:07:06.000000 ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/api_model_stubs/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4944 2022-02-09 11:07:06.000000 ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/api_model_stubs/brief.py
--rw-r--r--   0 runner    (1001) docker     (121)     3351 2022-02-09 11:07:06.000000 ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/api_model_stubs/brief_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     6629 2022-02-09 11:07:06.000000 ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/api_model_stubs/framework.py
--rw-r--r--   0 runner    (1001) docker     (121)      733 2022-02-09 11:07:06.000000 ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/api_model_stubs/framework_agreement.py
--rw-r--r--   0 runner    (1001) docker     (121)     1743 2022-02-09 11:07:06.000000 ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/api_model_stubs/lot.py
--rw-r--r--   0 runner    (1001) docker     (121)     3629 2022-02-09 11:07:06.000000 ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/api_model_stubs/services.py
--rw-r--r--   0 runner    (1001) docker     (121)     2916 2022-02-09 11:07:06.000000 ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/api_model_stubs/supplier.py
--rw-r--r--   0 runner    (1001) docker     (121)     3796 2022-02-09 11:07:06.000000 ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/api_model_stubs/supplier_framework.py
--rw-r--r--   0 runner    (1001) docker     (121)     3330 2022-02-09 11:07:06.000000 ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/comparisons.py
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-02-09 11:07:06.000000 ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-02-09 11:07:06.000000 ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/frontend.py
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-02-09 11:07:06.000000 ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/login.py
--rw-r--r--   0 runner    (1001) docker     (121)     3292 2022-02-09 11:07:06.000000 ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/mocking.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-09 11:07:17.758664 ccs-digitalmarketplace-test-utils-3.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-02-09 11:07:06.000000 ccs-digitalmarketplace-test-utils-3.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:03:18.017627 ccs-digitalmarketplace-test-utils-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-25 08:03:07.000000 ccs-digitalmarketplace-test-utils-4.0.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-25 08:03:18.017627 ccs-digitalmarketplace-test-utils-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-25 08:03:07.000000 ccs-digitalmarketplace-test-utils-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:03:18.009626 ccs-digitalmarketplace-test-utils-4.0.0/ccs_digitalmarketplace_test_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-25 08:03:17.000000 ccs-digitalmarketplace-test-utils-4.0.0/ccs_digitalmarketplace_test_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-25 08:03:17.000000 ccs-digitalmarketplace-test-utils-4.0.0/ccs_digitalmarketplace_test_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 08:03:17.000000 ccs-digitalmarketplace-test-utils-4.0.0/ccs_digitalmarketplace_test_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-25 08:03:17.000000 ccs-digitalmarketplace-test-utils-4.0.0/ccs_digitalmarketplace_test_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 08:03:17.000000 ccs-digitalmarketplace-test-utils-4.0.0/ccs_digitalmarketplace_test_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:03:18.013627 ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 08:03:07.000000 ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:03:18.017627 ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/api_model_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-25 08:03:07.000000 ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/api_model_stubs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-25 08:03:07.000000 ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/api_model_stubs/audit_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-07-25 08:03:07.000000 ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/api_model_stubs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-07-25 08:03:07.000000 ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/api_model_stubs/brief.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-25 08:03:07.000000 ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/api_model_stubs/brief_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-07-25 08:03:07.000000 ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/api_model_stubs/framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-25 08:03:07.000000 ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/api_model_stubs/framework_agreement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-25 08:03:07.000000 ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/api_model_stubs/lot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-07-25 08:03:07.000000 ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/api_model_stubs/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-25 08:03:07.000000 ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/api_model_stubs/supplier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-25 08:03:07.000000 ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/api_model_stubs/supplier_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-25 08:03:07.000000 ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-25 08:03:07.000000 ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-25 08:03:07.000000 ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-25 08:03:07.000000 ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-25 08:03:07.000000 ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/mocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 08:03:18.017627 ccs-digitalmarketplace-test-utils-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-25 08:03:07.000000 ccs-digitalmarketplace-test-utils-4.0.0/setup.py
```

### Comparing `ccs-digitalmarketplace-test-utils-3.0.6/LICENCE` & `ccs-digitalmarketplace-test-utils-4.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-3.0.6/README.md` & `ccs-digitalmarketplace-test-utils-4.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # digitalmarketplace-test-utils
 
-![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)
+![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)
 
 Utility functions and scripts for testing Digital Marketplace code
 
 This library's dependencies are deliberately kept minimal - see comment in `setup.py` before
 adding any more!
 
 ## Versioning
```

### Comparing `ccs-digitalmarketplace-test-utils-3.0.6/ccs_digitalmarketplace_test_utils.egg-info/SOURCES.txt` & `ccs-digitalmarketplace-test-utils-4.0.0/ccs_digitalmarketplace_test_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/api_model_stubs/__init__.py` & `ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/api_model_stubs/__init__.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/api_model_stubs/audit_event.py` & `ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/api_model_stubs/audit_event.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/api_model_stubs/base.py` & `ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/api_model_stubs/base.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/api_model_stubs/brief.py` & `ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/api_model_stubs/brief.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/api_model_stubs/brief_response.py` & `ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/api_model_stubs/brief_response.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/api_model_stubs/framework.py` & `ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/api_model_stubs/framework.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/api_model_stubs/framework_agreement.py` & `ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/api_model_stubs/framework_agreement.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/api_model_stubs/lot.py` & `ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/api_model_stubs/lot.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/api_model_stubs/services.py` & `ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/api_model_stubs/services.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/api_model_stubs/supplier.py` & `ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/api_model_stubs/supplier.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/api_model_stubs/supplier_framework.py` & `ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/api_model_stubs/supplier_framework.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/comparisons.py` & `ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/comparisons.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/fixtures.py` & `ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/fixtures.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/login.py` & `ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/login.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-3.0.6/dmtestutils/mocking.py` & `ccs-digitalmarketplace-test-utils-4.0.0/dmtestutils/mocking.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-test-utils-3.0.6/setup.py` & `ccs-digitalmarketplace-test-utils-4.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,13 +23,13 @@
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
     ],  # Dependency list should be minimal: if a particular test helper has a dependency on another lib (such as
         # Flask) then your app will already have that dependency included, and there's no need to add it here. If you
         # aren't using that particular function, you have no need of the dependency, so we should not install it by
         # default. Only add dependencies here if you introduce a new dependency that exists solely for testing purposes.
-    python_requires="~=3.8",
+    python_requires="~=3.9",
     entry_points={
         'console_scripts': [
         ],
     },
 )
```

