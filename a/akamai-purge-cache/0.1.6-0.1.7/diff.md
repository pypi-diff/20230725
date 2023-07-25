# Comparing `tmp/akamai_purge_cache-0.1.6.tar.gz` & `tmp/akamai_purge_cache-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akamai_purge_cache-0.1.6.tar", max compression
+gzip compressed data, was "akamai_purge_cache-0.1.7.tar", max compression
```

## Comparing `akamai_purge_cache-0.1.6.tar` & `akamai_purge_cache-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-07-19 02:42:42.924833 akamai_purge_cache-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-07-22 07:11:33.680448 akamai_purge_cache-0.1.6/akamai_purge_cache/__init__.py
--rwxr-xr-x   0        0        0      852 2023-07-22 08:16:41.104624 akamai_purge_cache-0.1.6/akamai_purge_cache/purge.py
--rw-r--r--   0        0        0      669 2023-07-22 08:25:53.440712 akamai_purge_cache-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 akamai_purge_cache-0.1.6/PKG-INFO
+-rwxr-xr-x   0        0        0        0 2023-07-19 02:42:42.000000 akamai_purge_cache-0.1.7/README.md
+-rwxr-xr-x   0        0        0        0 2023-07-22 07:11:33.000000 akamai_purge_cache-0.1.7/akamai_purge_cache/__init__.py
+-rwxr-xr-x   0        0        0      852 2023-07-22 08:16:41.000000 akamai_purge_cache-0.1.7/akamai_purge_cache/purge.py
+-rwxr-xr-x   0        0        0      669 2023-07-25 00:36:49.307210 akamai_purge_cache-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 akamai_purge_cache-0.1.7/PKG-INFO
```

### Comparing `akamai_purge_cache-0.1.6/akamai_purge_cache/purge.py` & `akamai_purge_cache-0.1.7/akamai_purge_cache/purge.py`

 * *Files identical despite different names*

### Comparing `akamai_purge_cache-0.1.6/pyproject.toml` & `akamai_purge_cache-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry] 
 name = "akamai_purge_cache"
-version = "0.1.6" 
+version = "0.1.7" 
 description = "Marriott CDN Team Fastpurge POC script" 
 authors = ["Alan Janis <alan.janis@marriott.com>", "Raahi Chada <raahi.chada@marriott.com"]
 readme = "README.md"
 packages = [{include = "akamai_purge_cache"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10"
```

### Comparing `akamai_purge_cache-0.1.6/PKG-INFO` & `akamai_purge_cache-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akamai-purge-cache
-Version: 0.1.6
+Version: 0.1.7
 Summary: Marriott CDN Team Fastpurge POC script
 Author: Alan Janis
 Author-email: alan.janis@marriott.com
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

