# Comparing `tmp/airflow_dbt_cta-0.0.7.tar.gz` & `tmp/airflow_dbt_cta-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow_dbt_cta-0.0.7.tar", last modified: Fri Mar 10 16:43:19 2023, max compression
+gzip compressed data, was "airflow_dbt_cta-0.0.8.tar", last modified: Tue Jul 25 15:08:00 2023, max compression
```

## Comparing `airflow_dbt_cta-0.0.7.tar` & `airflow_dbt_cta-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jesustoquinto   (501) staff       (20)        0 2023-03-10 16:43:19.052081 airflow_dbt_cta-0.0.7/
--rw-r--r--   0 jesustoquinto   (501) staff       (20)     1067 2023-03-10 00:25:40.000000 airflow_dbt_cta-0.0.7/LICENSE.txt
--rw-r--r--   0 jesustoquinto   (501) staff       (20)       25 2023-03-10 00:25:40.000000 airflow_dbt_cta-0.0.7/MANIFEST.in
--rw-r--r--   0 jesustoquinto   (501) staff       (20)     7099 2023-03-10 16:43:19.051733 airflow_dbt_cta-0.0.7/PKG-INFO
--rw-r--r--   0 jesustoquinto   (501) staff       (20)     6463 2023-03-10 00:25:40.000000 airflow_dbt_cta-0.0.7/README.md
-drwxr-xr-x   0 jesustoquinto   (501) staff       (20)        0 2023-03-10 16:43:19.044365 airflow_dbt_cta-0.0.7/airflow_dbt_cta/
--rw-r--r--   0 jesustoquinto   (501) staff       (20)      193 2023-03-10 00:25:40.000000 airflow_dbt_cta-0.0.7/airflow_dbt_cta/__init__.py
--rw-r--r--   0 jesustoquinto   (501) staff       (20)       63 2023-03-10 16:33:56.000000 airflow_dbt_cta-0.0.7/airflow_dbt_cta/__version__.py
-drwxr-xr-x   0 jesustoquinto   (501) staff       (20)        0 2023-03-10 16:43:19.048390 airflow_dbt_cta-0.0.7/airflow_dbt_cta/hooks/
--rw-r--r--   0 jesustoquinto   (501) staff       (20)       33 2023-03-10 00:25:40.000000 airflow_dbt_cta-0.0.7/airflow_dbt_cta/hooks/__init__.py
--rw-r--r--   0 jesustoquinto   (501) staff       (20)     5157 2023-03-10 00:25:40.000000 airflow_dbt_cta-0.0.7/airflow_dbt_cta/hooks/dbt_hook.py
-drwxr-xr-x   0 jesustoquinto   (501) staff       (20)        0 2023-03-10 16:43:19.050595 airflow_dbt_cta-0.0.7/airflow_dbt_cta/operators/
--rw-r--r--   0 jesustoquinto   (501) staff       (20)      166 2023-03-10 00:25:40.000000 airflow_dbt_cta-0.0.7/airflow_dbt_cta/operators/__init__.py
--rw-r--r--   0 jesustoquinto   (501) staff       (20)     6249 2023-03-10 00:32:39.000000 airflow_dbt_cta-0.0.7/airflow_dbt_cta/operators/dbt_operator.py
-drwxr-xr-x   0 jesustoquinto   (501) staff       (20)        0 2023-03-10 16:43:19.046779 airflow_dbt_cta-0.0.7/airflow_dbt_cta.egg-info/
--rw-r--r--   0 jesustoquinto   (501) staff       (20)     7099 2023-03-10 16:43:18.000000 airflow_dbt_cta-0.0.7/airflow_dbt_cta.egg-info/PKG-INFO
--rw-r--r--   0 jesustoquinto   (501) staff       (20)      443 2023-03-10 16:43:18.000000 airflow_dbt_cta-0.0.7/airflow_dbt_cta.egg-info/SOURCES.txt
--rw-r--r--   0 jesustoquinto   (501) staff       (20)        1 2023-03-10 16:43:18.000000 airflow_dbt_cta-0.0.7/airflow_dbt_cta.egg-info/dependency_links.txt
--rw-r--r--   0 jesustoquinto   (501) staff       (20)       23 2023-03-10 16:43:18.000000 airflow_dbt_cta-0.0.7/airflow_dbt_cta.egg-info/requires.txt
--rw-r--r--   0 jesustoquinto   (501) staff       (20)       16 2023-03-10 16:43:18.000000 airflow_dbt_cta-0.0.7/airflow_dbt_cta.egg-info/top_level.txt
--rw-r--r--   0 jesustoquinto   (501) staff       (20)       38 2023-03-10 16:43:19.052212 airflow_dbt_cta-0.0.7/setup.cfg
--rw-r--r--   0 jesustoquinto   (501) staff       (20)     2293 2023-03-10 00:25:40.000000 airflow_dbt_cta-0.0.7/setup.py
+drwxr-xr-x   0 jesustoquinto   (501) staff       (20)        0 2023-07-25 15:08:00.116710 airflow_dbt_cta-0.0.8/
+-rw-r--r--   0 jesustoquinto   (501) staff       (20)     1067 2023-03-10 00:25:40.000000 airflow_dbt_cta-0.0.8/LICENSE.txt
+-rw-r--r--   0 jesustoquinto   (501) staff       (20)       25 2023-03-10 00:25:40.000000 airflow_dbt_cta-0.0.8/MANIFEST.in
+-rw-r--r--   0 jesustoquinto   (501) staff       (20)     7099 2023-07-25 15:08:00.116235 airflow_dbt_cta-0.0.8/PKG-INFO
+-rw-r--r--   0 jesustoquinto   (501) staff       (20)     6463 2023-03-10 00:25:40.000000 airflow_dbt_cta-0.0.8/README.md
+drwxr-xr-x   0 jesustoquinto   (501) staff       (20)        0 2023-07-25 15:08:00.109517 airflow_dbt_cta-0.0.8/airflow_dbt_cta/
+-rw-r--r--   0 jesustoquinto   (501) staff       (20)      193 2023-03-10 00:25:40.000000 airflow_dbt_cta-0.0.8/airflow_dbt_cta/__init__.py
+-rw-r--r--   0 jesustoquinto   (501) staff       (20)       63 2023-07-25 15:07:56.000000 airflow_dbt_cta-0.0.8/airflow_dbt_cta/__version__.py
+drwxr-xr-x   0 jesustoquinto   (501) staff       (20)        0 2023-07-25 15:08:00.113578 airflow_dbt_cta-0.0.8/airflow_dbt_cta/hooks/
+-rw-r--r--   0 jesustoquinto   (501) staff       (20)       33 2023-03-10 00:25:40.000000 airflow_dbt_cta-0.0.8/airflow_dbt_cta/hooks/__init__.py
+-rw-r--r--   0 jesustoquinto   (501) staff       (20)     5152 2023-07-25 14:53:28.000000 airflow_dbt_cta-0.0.8/airflow_dbt_cta/hooks/dbt_hook.py
+drwxr-xr-x   0 jesustoquinto   (501) staff       (20)        0 2023-07-25 15:08:00.114879 airflow_dbt_cta-0.0.8/airflow_dbt_cta/operators/
+-rw-r--r--   0 jesustoquinto   (501) staff       (20)      166 2023-03-10 00:25:40.000000 airflow_dbt_cta-0.0.8/airflow_dbt_cta/operators/__init__.py
+-rw-r--r--   0 jesustoquinto   (501) staff       (20)     6249 2023-07-24 14:45:58.000000 airflow_dbt_cta-0.0.8/airflow_dbt_cta/operators/dbt_operator.py
+drwxr-xr-x   0 jesustoquinto   (501) staff       (20)        0 2023-07-25 15:08:00.112490 airflow_dbt_cta-0.0.8/airflow_dbt_cta.egg-info/
+-rw-r--r--   0 jesustoquinto   (501) staff       (20)     7099 2023-07-25 15:08:00.000000 airflow_dbt_cta-0.0.8/airflow_dbt_cta.egg-info/PKG-INFO
+-rw-r--r--   0 jesustoquinto   (501) staff       (20)      443 2023-07-25 15:08:00.000000 airflow_dbt_cta-0.0.8/airflow_dbt_cta.egg-info/SOURCES.txt
+-rw-r--r--   0 jesustoquinto   (501) staff       (20)        1 2023-07-25 15:08:00.000000 airflow_dbt_cta-0.0.8/airflow_dbt_cta.egg-info/dependency_links.txt
+-rw-r--r--   0 jesustoquinto   (501) staff       (20)       23 2023-07-25 15:08:00.000000 airflow_dbt_cta-0.0.8/airflow_dbt_cta.egg-info/requires.txt
+-rw-r--r--   0 jesustoquinto   (501) staff       (20)       16 2023-07-25 15:08:00.000000 airflow_dbt_cta-0.0.8/airflow_dbt_cta.egg-info/top_level.txt
+-rw-r--r--   0 jesustoquinto   (501) staff       (20)       38 2023-07-25 15:08:00.116877 airflow_dbt_cta-0.0.8/setup.cfg
+-rw-r--r--   0 jesustoquinto   (501) staff       (20)     2293 2023-03-10 00:25:40.000000 airflow_dbt_cta-0.0.8/setup.py
```

### Comparing `airflow_dbt_cta-0.0.7/LICENSE.txt` & `airflow_dbt_cta-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `airflow_dbt_cta-0.0.7/PKG-INFO` & `airflow_dbt_cta-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow_dbt_cta
-Version: 0.0.7
+Version: 0.0.8
 Summary: Apache Airflow integration for dbt (forked from https://github.com/gocardless/airflow-dbt)
 Home-page: https://github.com/communitytechalliance/airflow-dbt
 Author: GoCardless
 Author-email: engineering@gocardless.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `airflow_dbt_cta-0.0.7/README.md` & `airflow_dbt_cta-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `airflow_dbt_cta-0.0.7/airflow_dbt_cta/hooks/dbt_hook.py` & `airflow_dbt_cta-0.0.8/airflow_dbt_cta/hooks/dbt_hook.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import print_function
 import os
 import signal
 import subprocess
 import json
 from airflow.exceptions import AirflowException
-from airflow.hooks.base_hook import BaseHook
+from airflow.hooks.base import BaseHook
 
 
 class DbtCliHook(BaseHook):
     """
     Simple wrapper around the dbt CLI.
 
     :param env_vars: If set, passes the env_vars variables to the subprocess handler
```

### Comparing `airflow_dbt_cta-0.0.7/airflow_dbt_cta/operators/dbt_operator.py` & `airflow_dbt_cta-0.0.8/airflow_dbt_cta/operators/dbt_operator.py`

 * *Files identical despite different names*

### Comparing `airflow_dbt_cta-0.0.7/airflow_dbt_cta.egg-info/PKG-INFO` & `airflow_dbt_cta-0.0.8/airflow_dbt_cta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-dbt-cta
-Version: 0.0.7
+Version: 0.0.8
 Summary: Apache Airflow integration for dbt (forked from https://github.com/gocardless/airflow-dbt)
 Home-page: https://github.com/communitytechalliance/airflow-dbt
 Author: GoCardless
 Author-email: engineering@gocardless.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `airflow_dbt_cta-0.0.7/setup.py` & `airflow_dbt_cta-0.0.8/setup.py`

 * *Files identical despite different names*

