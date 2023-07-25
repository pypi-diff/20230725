# Comparing `tmp/saturn-python-1.1.tar.gz` & `tmp/saturn-python-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saturn-python-1.1.tar", last modified: Tue Jul 25 14:06:08 2023, max compression
+gzip compressed data, was "saturn-python-1.2.tar", last modified: Tue Jul 25 14:07:50 2023, max compression
```

## Comparing `saturn-python-1.1.tar` & `saturn-python-1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 14:06:08.390514 saturn-python-1.1/
--rw-rw-rw-   0        0        0      265 2023-07-25 14:06:08.389629 saturn-python-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1268 2023-07-25 13:54:44.000000 saturn-python-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 14:06:08.372861 saturn-python-1.1/saturn/
--rw-rw-rw-   0        0        0     1098 2023-07-25 13:54:44.000000 saturn-python-1.1/saturn/__init__.py
--rw-rw-rw-   0        0        0      328 2023-07-25 13:54:44.000000 saturn-python-1.1/saturn/scope.py
--rw-rw-rw-   0        0        0     3414 2023-07-25 14:02:08.000000 saturn-python-1.1/saturn/terminal.py
--rw-rw-rw-   0        0        0       20 2023-07-25 14:02:15.000000 saturn-python-1.1/saturn/version.py
-drwxrwxrwx   0        0        0        0 2023-07-25 14:06:08.388508 saturn-python-1.1/saturn_python.egg-info/
--rw-rw-rw-   0        0        0      265 2023-07-25 14:06:08.000000 saturn-python-1.1/saturn_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-07-25 14:06:08.000000 saturn-python-1.1/saturn_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 14:06:08.000000 saturn-python-1.1/saturn_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-25 14:06:08.000000 saturn-python-1.1/saturn_python.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-07-25 14:06:08.000000 saturn-python-1.1/saturn_python.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-07-25 14:06:08.000000 saturn-python-1.1/saturn_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 14:06:08.390514 saturn-python-1.1/setup.cfg
--rw-rw-rw-   0        0        0      535 2023-07-25 14:06:02.000000 saturn-python-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:07:50.168319 saturn-python-1.2/
+-rw-rw-rw-   0        0        0     1642 2023-07-25 14:07:50.167315 saturn-python-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1268 2023-07-25 13:54:44.000000 saturn-python-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 14:07:50.142732 saturn-python-1.2/saturn/
+-rw-rw-rw-   0        0        0     1098 2023-07-25 13:54:44.000000 saturn-python-1.2/saturn/__init__.py
+-rw-rw-rw-   0        0        0      328 2023-07-25 13:54:44.000000 saturn-python-1.2/saturn/scope.py
+-rw-rw-rw-   0        0        0     3414 2023-07-25 14:02:08.000000 saturn-python-1.2/saturn/terminal.py
+-rw-rw-rw-   0        0        0       20 2023-07-25 14:07:29.000000 saturn-python-1.2/saturn/version.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:07:50.166356 saturn-python-1.2/saturn_python.egg-info/
+-rw-rw-rw-   0        0        0     1642 2023-07-25 14:07:50.000000 saturn-python-1.2/saturn_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-07-25 14:07:50.000000 saturn-python-1.2/saturn_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 14:07:50.000000 saturn-python-1.2/saturn_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-25 14:07:50.000000 saturn-python-1.2/saturn_python.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-25 14:06:08.000000 saturn-python-1.2/saturn_python.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-07-25 14:07:50.000000 saturn-python-1.2/saturn_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 14:07:50.168319 saturn-python-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      736 2023-07-25 14:07:25.000000 saturn-python-1.2/setup.py
```

### Comparing `saturn-python-1.1/README.md` & `saturn-python-1.2/README.md`

 * *Files identical despite different names*

### Comparing `saturn-python-1.1/saturn/__init__.py` & `saturn-python-1.2/saturn/__init__.py`

 * *Files identical despite different names*

### Comparing `saturn-python-1.1/saturn/terminal.py` & `saturn-python-1.2/saturn/terminal.py`

 * *Files identical despite different names*

