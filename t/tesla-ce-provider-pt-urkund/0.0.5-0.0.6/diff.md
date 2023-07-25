# Comparing `tmp/tesla-ce-provider-pt-urkund-0.0.5.tar.gz` & `tmp/tesla-ce-provider-pt-urkund-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tesla-ce-provider-pt-urkund-0.0.5.tar", last modified: Tue Sep  6 12:49:42 2022, max compression
+gzip compressed data, was "tesla-ce-provider-pt-urkund-0.0.6.tar", last modified: Tue Jul 25 14:25:40 2023, max compression
```

## Comparing `tesla-ce-provider-pt-urkund-0.0.5.tar` & `tesla-ce-provider-pt-urkund-0.0.6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 12:49:42.427100 tesla-ce-provider-pt-urkund-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3448 2022-09-06 12:49:42.423100 tesla-ce-provider-pt-urkund-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2540 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     3513 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-06 12:49:42.427100 tesla-ce-provider-pt-urkund-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1714 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 12:49:42.423100 tesla-ce-provider-pt-urkund-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 12:49:42.423100 tesla-ce-provider-pt-urkund-0.0.5/src/tesla_ce_provider_pt_urkund.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3448 2022-09-06 12:49:42.000000 tesla-ce-provider-pt-urkund-0.0.5/src/tesla_ce_provider_pt_urkund.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1485 2022-09-06 12:49:42.000000 tesla-ce-provider-pt-urkund-0.0.5/src/tesla_ce_provider_pt_urkund.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-06 12:49:42.000000 tesla-ce-provider-pt-urkund-0.0.5/src/tesla_ce_provider_pt_urkund.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      614 2022-09-06 12:49:42.000000 tesla-ce-provider-pt-urkund-0.0.5/src/tesla_ce_provider_pt_urkund.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-09-06 12:49:42.000000 tesla-ce-provider-pt-urkund-0.0.5/src/tesla_ce_provider_pt_urkund.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 12:49:42.423100 tesla-ce-provider-pt-urkund-0.0.5/src/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      786 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6212 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/src/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2986 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/src/tests/test_validation_urkund.py
--rw-r--r--   0 runner    (1001) docker     (121)     1878 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/src/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 12:49:42.423100 tesla-ce-provider-pt-urkund-0.0.5/src/urkund/
--rw-r--r--   0 runner    (1001) docker     (121)      850 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/src/urkund/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 12:49:42.423100 tesla-ce-provider-pt-urkund-0.0.5/src/urkund/data/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-06 12:49:42.000000 tesla-ce-provider-pt-urkund-0.0.5/src/urkund/data/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 12:49:42.423100 tesla-ce-provider-pt-urkund-0.0.5/src/urkund/provider/
--rw-r--r--   0 runner    (1001) docker     (121)      858 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/src/urkund/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14875 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/src/urkund/provider/urkund.py
--rw-r--r--   0 runner    (1001) docker     (121)    10724 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/src/urkund/provider/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 12:49:42.423100 tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/
--rw-r--r--   0 runner    (1001) docker     (121)     4973 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 12:49:42.423100 tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/exceptions/
--rw-r--r--   0 runner    (1001) docker     (121)     1396 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/exceptions/bad_request.py
--rw-r--r--   0 runner    (1001) docker     (121)      872 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/exceptions/base_urkund_lib_exception.py
--rw-r--r--   0 runner    (1001) docker     (121)      927 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/exceptions/invalid_response.py
--rw-r--r--   0 runner    (1001) docker     (121)      945 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/exceptions/media_type_not_supported.py
--rw-r--r--   0 runner    (1001) docker     (121)      942 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/exceptions/mime_type_not_supported.py
--rw-r--r--   0 runner    (1001) docker     (121)      918 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/exceptions/not_available.py
--rw-r--r--   0 runner    (1001) docker     (121)      906 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/exceptions/not_found.py
--rw-r--r--   0 runner    (1001) docker     (121)      924 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/exceptions/receiver_exists.py
--rw-r--r--   0 runner    (1001) docker     (121)      927 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/exceptions/request_too_large.py
--rw-r--r--   0 runner    (1001) docker     (121)      936 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/exceptions/submission_not_found.py
--rw-r--r--   0 runner    (1001) docker     (121)      903 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/exceptions/timeout.py
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/exceptions/unauthorized.py
--rw-r--r--   0 runner    (1001) docker     (121)      963 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/exceptions/unit_and_organization_not_valid.py
--rw-r--r--   0 runner    (1001) docker     (121)     3613 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/receivers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3721 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/request.py
--rw-r--r--   0 runner    (1001) docker     (121)     2988 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/submissions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1502 2022-09-06 12:49:35.000000 tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:25:40.484524 tesla-ce-provider-pt-urkund-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-07-25 14:25:40.484524 tesla-ce-provider-pt-urkund-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 14:25:40.484524 tesla-ce-provider-pt-urkund-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:25:40.472523 tesla-ce-provider-pt-urkund-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:25:40.476523 tesla-ce-provider-pt-urkund-0.0.6/src/tesla_ce_provider_pt_urkund.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-07-25 14:25:40.000000 tesla-ce-provider-pt-urkund-0.0.6/src/tesla_ce_provider_pt_urkund.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-25 14:25:40.000000 tesla-ce-provider-pt-urkund-0.0.6/src/tesla_ce_provider_pt_urkund.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 14:25:40.000000 tesla-ce-provider-pt-urkund-0.0.6/src/tesla_ce_provider_pt_urkund.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-25 14:25:40.000000 tesla-ce-provider-pt-urkund-0.0.6/src/tesla_ce_provider_pt_urkund.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 14:25:40.000000 tesla-ce-provider-pt-urkund-0.0.6/src/tesla_ce_provider_pt_urkund.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:25:40.476523 tesla-ce-provider-pt-urkund-0.0.6/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/src/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/src/tests/test_validation_urkund.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/src/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:25:40.476523 tesla-ce-provider-pt-urkund-0.0.6/src/urkund/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/src/urkund/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:25:40.476523 tesla-ce-provider-pt-urkund-0.0.6/src/urkund/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 14:25:39.000000 tesla-ce-provider-pt-urkund-0.0.6/src/urkund/data/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:25:40.476523 tesla-ce-provider-pt-urkund-0.0.6/src/urkund/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/src/urkund/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/src/urkund/provider/urkund.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10724 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/src/urkund/provider/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:25:40.480523 tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:25:40.484524 tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/exceptions/bad_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/exceptions/base_urkund_lib_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/exceptions/invalid_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/exceptions/media_type_not_supported.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/exceptions/mime_type_not_supported.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/exceptions/not_available.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/exceptions/not_found.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/exceptions/receiver_exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/exceptions/request_too_large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/exceptions/submission_not_found.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/exceptions/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/exceptions/unauthorized.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/exceptions/unit_and_organization_not_valid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/receivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/submissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-25 14:25:29.000000 tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/units.py
```

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/LICENSE` & `tesla-ce-provider-pt-urkund-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/PKG-INFO` & `tesla-ce-provider-pt-urkund-0.0.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,31 @@
-Metadata-Version: 2.1
-Name: tesla-ce-provider-pt-urkund
-Version: 0.0.5
-Summary: TeSLA CE Urkund Plagiarism Provider
-Home-page: https://tesla-ce.github.io
-Author: Roger Muñoz Bernaus
-Author-email: rmunozber@uoc.edu
-License: UNKNOWN
-Project-URL: Documentation, https://tesla-ce.github.io/provider-pt-urkund/
-Project-URL: Source, https://github.com/tesla-ce/provider-pt-urkund
-Description: [![PyPi Version](https://img.shields.io/pypi/v/tesla-ce-provider-pt-urkund.svg)](https://pypi.python.org/pypi/tesla-ce-provider-pt-urkund/)
-        [![codecov](https://codecov.io/gh/tesla-ce/provider-pt-urkund/branch/main/graph/badge.svg?token=PJJQMW981P)](https://codecov.io/gh/tesla-ce/provider-pt-urkund)
-        [![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)
-        [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-urkund.svg?type=shield)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-urkund?ref=badge_shield)
-        [![Quality gate](https://sonar.sunai.uoc.edu/api/project_badges/quality_gate?project=tesla-ce_provider-pt-urkund)](https://sonar.sunai.uoc.edu/dashboard?id=tesla-ce_provider-pt-urkund)
-        
-        
-        # TeSLA CE Plagiarism Tool based on URKUND
-        
-        | :warning: This repository is **under construction**. Final release of TeSLA Community Edition source code is expected by the **end of 2021** |
-        | --- |
-        
-        ## Description
-        Description: A description of your project follows. A good description is clear, short, and to the point. Describe the importance of your project, and what it does.
-        
-        ## Installation
-        Installation: Installation is the next section in an effective README. Tell other users how to install your project locally. Optionally, include a gif to make the process even more clear for other people.
-        
-        ## Usage
-        Usage: The next section is usage, in which you instruct other people on how to use your project after they’ve installed it. This would also be a good place to include screenshots of your project in action.
-        
-        ## Contributing
-        Contributing: Larger projects often have sections on contributing to their project, in which contribution instructions are outlined. Sometimes, this is a separate file. If you have specific contribution preferences, explain them so that other developers know how to best contribute to your work. To learn more about how to help others contribute, check out the guide for setting guidelines for repository contributors.
-        
-        ## Credits
-        Credits: Include a section for credits in order to highlight and link to the authors of your project.
-        
-        ## License
-        This project is licensed under [AGPL v3 licence](http://www.gnu.org/licenses/agpl-3.0).
-        
-        [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-urkund.svg?type=large)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-urkund?ref=badge_large)
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+[![PyPi Version](https://img.shields.io/pypi/v/tesla-ce-provider-pt-urkund.svg)](https://pypi.python.org/pypi/tesla-ce-provider-pt-urkund/)
+[![codecov](https://codecov.io/gh/tesla-ce/provider-pt-urkund/branch/main/graph/badge.svg?token=PJJQMW981P)](https://codecov.io/gh/tesla-ce/provider-pt-urkund)
+[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)
+[![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-urkund.svg?type=shield)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-urkund?ref=badge_shield)
+[![Quality gate](https://sonar.sunai.uoc.edu/api/project_badges/quality_gate?project=tesla-ce_provider-pt-urkund)](https://sonar.sunai.uoc.edu/dashboard?id=tesla-ce_provider-pt-urkund)
+
+
+# TeSLA CE Plagiarism Tool based on URKUND
+
+| :warning: This repository is **under construction**. Final release of TeSLA Community Edition source code is expected by the **end of 2021** |
+| --- |
+
+## Description
+Description: A description of your project follows. A good description is clear, short, and to the point. Describe the importance of your project, and what it does.
+
+## Installation
+Installation: Installation is the next section in an effective README. Tell other users how to install your project locally. Optionally, include a gif to make the process even more clear for other people.
+
+## Usage
+Usage: The next section is usage, in which you instruct other people on how to use your project after they’ve installed it. This would also be a good place to include screenshots of your project in action.
+
+## Contributing
+Contributing: Larger projects often have sections on contributing to their project, in which contribution instructions are outlined. Sometimes, this is a separate file. If you have specific contribution preferences, explain them so that other developers know how to best contribute to your work. To learn more about how to help others contribute, check out the guide for setting guidelines for repository contributors.
+
+## Credits
+Credits: Include a section for credits in order to highlight and link to the authors of your project.
+
+## License
+This project is licensed under [AGPL v3 licence](http://www.gnu.org/licenses/agpl-3.0).
+
+[![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-urkund.svg?type=large)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-urkund?ref=badge_large)
```

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/README.md` & `tesla-ce-provider-pt-urkund-0.0.6/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: tesla-ce-provider-pt-urkund
+Version: 0.0.6
+Summary: TeSLA CE Urkund Plagiarism Provider
+Home-page: https://tesla-ce.github.io
+Author: Roger Muñoz Bernaus
+Author-email: rmunozber@uoc.edu
+License: UNKNOWN
+Project-URL: Documentation, https://tesla-ce.github.io/provider-pt-urkund/
+Project-URL: Source, https://github.com/tesla-ce/provider-pt-urkund
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![PyPi Version](https://img.shields.io/pypi/v/tesla-ce-provider-pt-urkund.svg)](https://pypi.python.org/pypi/tesla-ce-provider-pt-urkund/)
 [![codecov](https://codecov.io/gh/tesla-ce/provider-pt-urkund/branch/main/graph/badge.svg?token=PJJQMW981P)](https://codecov.io/gh/tesla-ce/provider-pt-urkund)
 [![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)
 [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-urkund.svg?type=shield)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-urkund?ref=badge_shield)
 [![Quality gate](https://sonar.sunai.uoc.edu/api/project_badges/quality_gate?project=tesla-ce_provider-pt-urkund)](https://sonar.sunai.uoc.edu/dashboard?id=tesla-ce_provider-pt-urkund)
 
 
@@ -25,7 +43,9 @@
 ## Credits
 Credits: Include a section for credits in order to highlight and link to the authors of your project.
 
 ## License
 This project is licensed under [AGPL v3 licence](http://www.gnu.org/licenses/agpl-3.0).
 
 [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-urkund.svg?type=large)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-urkund?ref=badge_large)
+
+
```

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/setup.py` & `tesla-ce-provider-pt-urkund-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     packages=setuptools.find_packages('src', exclude='__pycache__'),
     package_dir={'': 'src'},  # tell distutils packages are under src
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
         "Operating System :: POSIX :: Linux",
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     package_data={
         '': ['*.cfg', 'VERSION'],
         'urkund': [
             'data/*',
                     ],
     },
     include_package_data=True,
```

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/src/tesla_ce_provider_pt_urkund.egg-info/PKG-INFO` & `tesla-ce-provider-pt-urkund-0.0.6/src/tesla_ce_provider_pt_urkund.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 Metadata-Version: 2.1
 Name: tesla-ce-provider-pt-urkund
-Version: 0.0.5
+Version: 0.0.6
 Summary: TeSLA CE Urkund Plagiarism Provider
 Home-page: https://tesla-ce.github.io
 Author: Roger Muñoz Bernaus
 Author-email: rmunozber@uoc.edu
 License: UNKNOWN
 Project-URL: Documentation, https://tesla-ce.github.io/provider-pt-urkund/
 Project-URL: Source, https://github.com/tesla-ce/provider-pt-urkund
-Description: [![PyPi Version](https://img.shields.io/pypi/v/tesla-ce-provider-pt-urkund.svg)](https://pypi.python.org/pypi/tesla-ce-provider-pt-urkund/)
-        [![codecov](https://codecov.io/gh/tesla-ce/provider-pt-urkund/branch/main/graph/badge.svg?token=PJJQMW981P)](https://codecov.io/gh/tesla-ce/provider-pt-urkund)
-        [![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)
-        [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-urkund.svg?type=shield)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-urkund?ref=badge_shield)
-        [![Quality gate](https://sonar.sunai.uoc.edu/api/project_badges/quality_gate?project=tesla-ce_provider-pt-urkund)](https://sonar.sunai.uoc.edu/dashboard?id=tesla-ce_provider-pt-urkund)
-        
-        
-        # TeSLA CE Plagiarism Tool based on URKUND
-        
-        | :warning: This repository is **under construction**. Final release of TeSLA Community Edition source code is expected by the **end of 2021** |
-        | --- |
-        
-        ## Description
-        Description: A description of your project follows. A good description is clear, short, and to the point. Describe the importance of your project, and what it does.
-        
-        ## Installation
-        Installation: Installation is the next section in an effective README. Tell other users how to install your project locally. Optionally, include a gif to make the process even more clear for other people.
-        
-        ## Usage
-        Usage: The next section is usage, in which you instruct other people on how to use your project after they’ve installed it. This would also be a good place to include screenshots of your project in action.
-        
-        ## Contributing
-        Contributing: Larger projects often have sections on contributing to their project, in which contribution instructions are outlined. Sometimes, this is a separate file. If you have specific contribution preferences, explain them so that other developers know how to best contribute to your work. To learn more about how to help others contribute, check out the guide for setting guidelines for repository contributors.
-        
-        ## Credits
-        Credits: Include a section for credits in order to highlight and link to the authors of your project.
-        
-        ## License
-        This project is licensed under [AGPL v3 licence](http://www.gnu.org/licenses/agpl-3.0).
-        
-        [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-urkund.svg?type=large)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-urkund?ref=badge_large)
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPi Version](https://img.shields.io/pypi/v/tesla-ce-provider-pt-urkund.svg)](https://pypi.python.org/pypi/tesla-ce-provider-pt-urkund/)
+[![codecov](https://codecov.io/gh/tesla-ce/provider-pt-urkund/branch/main/graph/badge.svg?token=PJJQMW981P)](https://codecov.io/gh/tesla-ce/provider-pt-urkund)
+[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)
+[![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-urkund.svg?type=shield)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-urkund?ref=badge_shield)
+[![Quality gate](https://sonar.sunai.uoc.edu/api/project_badges/quality_gate?project=tesla-ce_provider-pt-urkund)](https://sonar.sunai.uoc.edu/dashboard?id=tesla-ce_provider-pt-urkund)
+
+
+# TeSLA CE Plagiarism Tool based on URKUND
+
+| :warning: This repository is **under construction**. Final release of TeSLA Community Edition source code is expected by the **end of 2021** |
+| --- |
+
+## Description
+Description: A description of your project follows. A good description is clear, short, and to the point. Describe the importance of your project, and what it does.
+
+## Installation
+Installation: Installation is the next section in an effective README. Tell other users how to install your project locally. Optionally, include a gif to make the process even more clear for other people.
+
+## Usage
+Usage: The next section is usage, in which you instruct other people on how to use your project after they’ve installed it. This would also be a good place to include screenshots of your project in action.
+
+## Contributing
+Contributing: Larger projects often have sections on contributing to their project, in which contribution instructions are outlined. Sometimes, this is a separate file. If you have specific contribution preferences, explain them so that other developers know how to best contribute to your work. To learn more about how to help others contribute, check out the guide for setting guidelines for repository contributors.
+
+## Credits
+Credits: Include a section for credits in order to highlight and link to the authors of your project.
+
+## License
+This project is licensed under [AGPL v3 licence](http://www.gnu.org/licenses/agpl-3.0).
+
+[![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-urkund.svg?type=large)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-urkund?ref=badge_large)
+
+
```

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/src/tesla_ce_provider_pt_urkund.egg-info/SOURCES.txt` & `tesla-ce-provider-pt-urkund-0.0.6/src/tesla_ce_provider_pt_urkund.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/src/tests/__init__.py` & `tesla-ce-provider-pt-urkund-0.0.6/src/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/src/tests/conftest.py` & `tesla-ce-provider-pt-urkund-0.0.6/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/src/tests/test_validation_urkund.py` & `tesla-ce-provider-pt-urkund-0.0.6/src/tests/test_validation_urkund.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/src/tests/utils.py` & `tesla-ce-provider-pt-urkund-0.0.6/src/tests/utils.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/src/urkund/__init__.py` & `tesla-ce-provider-pt-urkund-0.0.6/src/urkund/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/src/urkund/provider/__init__.py` & `tesla-ce-provider-pt-urkund-0.0.6/src/urkund/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/src/urkund/provider/urkund.py` & `tesla-ce-provider-pt-urkund-0.0.6/src/urkund/provider/urkund.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/src/urkund/provider/utils.py` & `tesla-ce-provider-pt-urkund-0.0.6/src/urkund/provider/utils.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/__init__.py` & `tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/exceptions/__init__.py` & `tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/exceptions/bad_request.py` & `tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/exceptions/bad_request.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/exceptions/base_urkund_lib_exception.py` & `tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/exceptions/base_urkund_lib_exception.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/exceptions/invalid_response.py` & `tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/exceptions/invalid_response.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/exceptions/media_type_not_supported.py` & `tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/exceptions/media_type_not_supported.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/exceptions/mime_type_not_supported.py` & `tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/exceptions/mime_type_not_supported.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/exceptions/not_available.py` & `tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/exceptions/not_available.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/exceptions/not_found.py` & `tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/exceptions/not_found.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/exceptions/receiver_exists.py` & `tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/exceptions/receiver_exists.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/exceptions/request_too_large.py` & `tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/exceptions/request_too_large.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/exceptions/submission_not_found.py` & `tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/exceptions/submission_not_found.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/exceptions/timeout.py` & `tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/exceptions/timeout.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/exceptions/unauthorized.py` & `tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/exceptions/unauthorized.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/exceptions/unit_and_organization_not_valid.py` & `tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/exceptions/unit_and_organization_not_valid.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/receivers.py` & `tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/receivers.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/request.py` & `tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/request.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/submissions.py` & `tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/submissions.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-urkund-0.0.5/src/urkund/urkund_lib/units.py` & `tesla-ce-provider-pt-urkund-0.0.6/src/urkund/urkund_lib/units.py`

 * *Files identical despite different names*

