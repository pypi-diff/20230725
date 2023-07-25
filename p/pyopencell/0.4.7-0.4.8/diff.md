# Comparing `tmp/pyopencell-0.4.7.tar.gz` & `tmp/pyopencell-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyopencell-0.4.7.tar", last modified: Mon Sep 12 07:08:44 2022, max compression
+gzip compressed data, was "dist/pyopencell-0.4.8.tar", last modified: Tue Jul 25 12:01:14 2023, max compression
```

## Comparing `pyopencell-0.4.7.tar` & `pyopencell-0.4.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-12 07:08:44.000000 pyopencell-0.4.7/
--rw-rw-rw-   0 root         (0) root         (0)    35149 2022-09-07 08:54:36.000000 pyopencell-0.4.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2887 2022-09-12 07:08:44.000000 pyopencell-0.4.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2348 2022-09-07 08:54:36.000000 pyopencell-0.4.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-12 07:08:44.000000 pyopencell-0.4.7/pyopencell/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-07 08:54:36.000000 pyopencell-0.4.7/pyopencell/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4629 2022-09-07 08:54:36.000000 pyopencell-0.4.7/pyopencell/client.py
--rw-rw-rw-   0 root         (0) root         (0)      693 2022-09-07 08:54:36.000000 pyopencell-0.4.7/pyopencell/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      193 2022-09-07 08:54:36.000000 pyopencell-0.4.7/pyopencell/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-12 07:08:44.000000 pyopencell-0.4.7/pyopencell/resources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-07 08:54:36.000000 pyopencell-0.4.7/pyopencell/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1474 2022-09-07 08:54:36.000000 pyopencell-0.4.7/pyopencell/resources/access.py
--rw-rw-rw-   0 root         (0) root         (0)      173 2022-09-07 08:54:36.000000 pyopencell-0.4.7/pyopencell/resources/base_resource.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2022-09-07 08:54:36.000000 pyopencell-0.4.7/pyopencell/resources/base_resource_list.py
--rw-rw-rw-   0 root         (0) root         (0)     2815 2022-09-07 08:54:36.000000 pyopencell-0.4.7/pyopencell/resources/crm_account_hierarchy.py
--rw-rw-rw-   0 root         (0) root         (0)     2294 2022-09-07 08:54:36.000000 pyopencell-0.4.7/pyopencell/resources/customer.py
--rw-rw-rw-   0 root         (0) root         (0)     2814 2022-09-07 08:54:36.000000 pyopencell-0.4.7/pyopencell/resources/customer_account.py
--rw-rw-rw-   0 root         (0) root         (0)     1047 2022-09-07 08:54:36.000000 pyopencell-0.4.7/pyopencell/resources/invoice.py
--rw-rw-rw-   0 root         (0) root         (0)     1532 2022-09-07 08:54:36.000000 pyopencell-0.4.7/pyopencell/resources/invoice_list.py
--rw-rw-rw-   0 root         (0) root         (0)     4617 2022-09-07 08:54:36.000000 pyopencell-0.4.7/pyopencell/resources/subscription.py
--rw-rw-rw-   0 root         (0) root         (0)     1406 2022-09-07 08:54:36.000000 pyopencell-0.4.7/pyopencell/resources/subscription_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-12 07:08:44.000000 pyopencell-0.4.7/pyopencell/responses/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-07 08:54:36.000000 pyopencell-0.4.7/pyopencell/responses/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      229 2022-09-07 08:54:36.000000 pyopencell-0.4.7/pyopencell/responses/action_status.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2022-09-07 08:54:36.000000 pyopencell-0.4.7/pyopencell/responses/paged_response.py
--rw-rw-rw-   0 root         (0) root         (0)      770 2022-09-07 08:54:36.000000 pyopencell-0.4.7/pyopencell/responses/paging.py
--rw-rw-rw-   0 root         (0) root         (0)      301 2022-09-07 08:54:36.000000 pyopencell-0.4.7/pyopencell/responses/response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-12 07:08:44.000000 pyopencell-0.4.7/pyopencell.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2887 2022-09-12 07:08:44.000000 pyopencell-0.4.7/pyopencell.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      906 2022-09-12 07:08:44.000000 pyopencell-0.4.7/pyopencell.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-12 07:08:44.000000 pyopencell-0.4.7/pyopencell.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-12 07:08:44.000000 pyopencell-0.4.7/pyopencell.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        9 2022-09-12 07:08:44.000000 pyopencell-0.4.7/pyopencell.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-09-12 07:08:44.000000 pyopencell-0.4.7/pyopencell.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-09-12 07:08:44.000000 pyopencell-0.4.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2006 2022-09-12 07:03:53.000000 pyopencell-0.4.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:01:14.000000 pyopencell-0.4.8/
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-07-25 10:24:26.000000 pyopencell-0.4.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2887 2023-07-25 12:01:14.000000 pyopencell-0.4.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2348 2023-07-25 10:24:26.000000 pyopencell-0.4.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:01:14.000000 pyopencell-0.4.8/pyopencell/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 12:00:57.000000 pyopencell-0.4.8/pyopencell/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4873 2023-07-25 11:00:19.000000 pyopencell-0.4.8/pyopencell/client.py
+-rw-rw-rw-   0 root         (0) root         (0)      693 2023-07-25 10:24:26.000000 pyopencell-0.4.8/pyopencell/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      193 2023-07-25 10:24:26.000000 pyopencell-0.4.8/pyopencell/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:01:14.000000 pyopencell-0.4.8/pyopencell/resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 12:00:57.000000 pyopencell-0.4.8/pyopencell/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1474 2023-07-25 10:24:26.000000 pyopencell-0.4.8/pyopencell/resources/access.py
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-07-25 10:24:26.000000 pyopencell-0.4.8/pyopencell/resources/base_resource.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-07-25 10:24:26.000000 pyopencell-0.4.8/pyopencell/resources/base_resource_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     2815 2023-07-25 10:24:26.000000 pyopencell-0.4.8/pyopencell/resources/crm_account_hierarchy.py
+-rw-rw-rw-   0 root         (0) root         (0)     2294 2023-07-25 10:24:26.000000 pyopencell-0.4.8/pyopencell/resources/customer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2814 2023-07-25 10:24:26.000000 pyopencell-0.4.8/pyopencell/resources/customer_account.py
+-rw-rw-rw-   0 root         (0) root         (0)     1047 2023-07-25 10:24:26.000000 pyopencell-0.4.8/pyopencell/resources/invoice.py
+-rw-rw-rw-   0 root         (0) root         (0)     1532 2023-07-25 10:24:26.000000 pyopencell-0.4.8/pyopencell/resources/invoice_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     4617 2023-07-25 10:24:26.000000 pyopencell-0.4.8/pyopencell/resources/subscription.py
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2023-07-25 10:24:26.000000 pyopencell-0.4.8/pyopencell/resources/subscription_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:01:14.000000 pyopencell-0.4.8/pyopencell/responses/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 12:00:57.000000 pyopencell-0.4.8/pyopencell/responses/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      229 2023-07-25 10:24:26.000000 pyopencell-0.4.8/pyopencell/responses/action_status.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2023-07-25 10:24:26.000000 pyopencell-0.4.8/pyopencell/responses/paged_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      770 2023-07-25 10:24:26.000000 pyopencell-0.4.8/pyopencell/responses/paging.py
+-rw-rw-rw-   0 root         (0) root         (0)      301 2023-07-25 10:24:26.000000 pyopencell-0.4.8/pyopencell/responses/response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:01:14.000000 pyopencell-0.4.8/pyopencell.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2887 2023-07-25 12:01:14.000000 pyopencell-0.4.8/pyopencell.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      906 2023-07-25 12:01:14.000000 pyopencell-0.4.8/pyopencell.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 12:01:14.000000 pyopencell-0.4.8/pyopencell.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 12:01:14.000000 pyopencell-0.4.8/pyopencell.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-25 12:01:14.000000 pyopencell-0.4.8/pyopencell.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-25 12:01:14.000000 pyopencell-0.4.8/pyopencell.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 12:01:14.000000 pyopencell-0.4.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2006 2023-07-25 11:50:06.000000 pyopencell-0.4.8/setup.py
```

### Comparing `pyopencell-0.4.7/LICENSE` & `pyopencell-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopencell-0.4.7/PKG-INFO` & `pyopencell-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopencell
-Version: 0.4.7
+Version: 0.4.8
 Summary: Python wrapper for OpenCell (using REST API)
 Home-page: https://gitlab.com/coopdevs/pyopencell
 Author: Coopdevs
 Author-email: info@coopdevs.org
 Maintainer: Daniel Palomar, Antonio Barcia
 License: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `pyopencell-0.4.7/README.md` & `pyopencell-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `pyopencell-0.4.7/pyopencell/client.py` & `pyopencell-0.4.8/pyopencell/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,22 @@
         if self._check_response_error(response):
             raise exceptions.PyOpenCellAPIException(
                 verb=response.request.method,
                 url=response.request.url,
                 status=response.status_code,
                 body=response.content or ""
             )
-
+        logger.info(
+            "{origin} {verb} {url} \n {elapsed}".format(
+                origin=__name__,
+                verb=verb,
+                url=url,
+                elapsed=response.elapsed.total_seconds(),
+            )
+        )
         return response
 
     @staticmethod
     def _check_response_error(response):
         """ Check the response of the OpenCell API. Not always the status code match with the real
         status of the response. We found some cases that response has a 200 OK status but in the
         body we find an error message instead of the expected response.
```

### Comparing `pyopencell-0.4.7/pyopencell/exceptions.py` & `pyopencell-0.4.8/pyopencell/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyopencell-0.4.7/pyopencell/resources/access.py` & `pyopencell-0.4.8/pyopencell/resources/access.py`

 * *Files identical despite different names*

### Comparing `pyopencell-0.4.7/pyopencell/resources/crm_account_hierarchy.py` & `pyopencell-0.4.8/pyopencell/resources/crm_account_hierarchy.py`

 * *Files identical despite different names*

### Comparing `pyopencell-0.4.7/pyopencell/resources/customer.py` & `pyopencell-0.4.8/pyopencell/resources/customer.py`

 * *Files identical despite different names*

### Comparing `pyopencell-0.4.7/pyopencell/resources/customer_account.py` & `pyopencell-0.4.8/pyopencell/resources/customer_account.py`

 * *Files identical despite different names*

### Comparing `pyopencell-0.4.7/pyopencell/resources/invoice.py` & `pyopencell-0.4.8/pyopencell/resources/invoice.py`

 * *Files identical despite different names*

### Comparing `pyopencell-0.4.7/pyopencell/resources/invoice_list.py` & `pyopencell-0.4.8/pyopencell/resources/invoice_list.py`

 * *Files identical despite different names*

### Comparing `pyopencell-0.4.7/pyopencell/resources/subscription.py` & `pyopencell-0.4.8/pyopencell/resources/subscription.py`

 * *Files identical despite different names*

### Comparing `pyopencell-0.4.7/pyopencell/resources/subscription_list.py` & `pyopencell-0.4.8/pyopencell/resources/subscription_list.py`

 * *Files identical despite different names*

### Comparing `pyopencell-0.4.7/pyopencell/responses/paged_response.py` & `pyopencell-0.4.8/pyopencell/responses/paged_response.py`

 * *Files identical despite different names*

### Comparing `pyopencell-0.4.7/pyopencell/responses/paging.py` & `pyopencell-0.4.8/pyopencell/responses/paging.py`

 * *Files identical despite different names*

### Comparing `pyopencell-0.4.7/pyopencell.egg-info/PKG-INFO` & `pyopencell-0.4.8/pyopencell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopencell
-Version: 0.4.7
+Version: 0.4.8
 Summary: Python wrapper for OpenCell (using REST API)
 Home-page: https://gitlab.com/coopdevs/pyopencell
 Author: Coopdevs
 Author-email: info@coopdevs.org
 Maintainer: Daniel Palomar, Antonio Barcia
 License: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `pyopencell-0.4.7/pyopencell.egg-info/SOURCES.txt` & `pyopencell-0.4.8/pyopencell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyopencell-0.4.7/setup.py` & `pyopencell-0.4.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import sys
 
 with open('README.md') as f:
     README = f.read()
 
 
-VERSION = '0.4.7'
+VERSION = '0.4.8'
 
 
 ########
 # Copied from https://github.com/kennethreitz/setup.py
 here = os.path.abspath(os.path.dirname(__file__))
```

