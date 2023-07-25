# Comparing `tmp/easy_tasks-0.0.8.tar.gz` & `tmp/easy_tasks-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_tasks-0.0.8.tar", last modified: Thu Jun  8 16:01:58 2023, max compression
+gzip compressed data, was "easy_tasks-0.0.9.tar", last modified: Thu Jul 20 17:24:53 2023, max compression
```

## Comparing `easy_tasks-0.0.8.tar` & `easy_tasks-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 16:01:58.388882 easy_tasks-0.0.8/
--rw-rw-rw-   0        0        0     1095 2023-01-07 18:12:34.000000 easy_tasks-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       82 2023-01-17 17:17:39.000000 easy_tasks-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     3118 2023-06-08 16:01:58.387879 easy_tasks-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2402 2023-02-14 21:25:45.000000 easy_tasks-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 16:01:58.379875 easy_tasks-0.0.8/easy_tasks/
--rw-rw-rw-   0        0        0      742 2023-06-08 16:00:31.000000 easy_tasks-0.0.8/easy_tasks/__init__.py
--rw-rw-rw-   0        0        0      542 2023-01-07 18:12:34.000000 easy_tasks-0.0.8/easy_tasks/closest_furthest_value.py
--rw-rw-rw-   0        0        0     2223 2023-01-07 18:12:34.000000 easy_tasks-0.0.8/easy_tasks/dublicates.py
--rw-rw-rw-   0        0        0      735 2023-01-07 18:12:34.000000 easy_tasks-0.0.8/easy_tasks/help_with_json.py
--rw-rw-rw-   0        0        0      618 2023-01-07 18:12:34.000000 easy_tasks-0.0.8/easy_tasks/help_with_pickle.py
--rw-rw-rw-   0        0        0     3627 2023-01-17 17:22:26.000000 easy_tasks-0.0.8/easy_tasks/list_printer.py
--rw-rw-rw-   0        0        0     3614 2023-01-07 18:12:34.000000 easy_tasks-0.0.8/easy_tasks/percentage.py
--rw-rw-rw-   0        0        0      338 2023-01-07 18:12:34.000000 easy_tasks-0.0.8/easy_tasks/sorter.py
--rw-rw-rw-   0        0        0     1437 2023-01-07 18:12:34.000000 easy_tasks-0.0.8/easy_tasks/string_transformation.py
--rw-rw-rw-   0        0        0      654 2023-05-16 22:05:16.000000 easy_tasks-0.0.8/easy_tasks/unpack.py
-drwxrwxrwx   0        0        0        0 2023-06-08 16:01:58.386876 easy_tasks-0.0.8/easy_tasks.egg-info/
--rw-rw-rw-   0        0        0     3118 2023-06-08 16:01:58.000000 easy_tasks-0.0.8/easy_tasks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-06-08 16:01:58.000000 easy_tasks-0.0.8/easy_tasks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 16:01:58.000000 easy_tasks-0.0.8/easy_tasks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-08 16:01:58.000000 easy_tasks-0.0.8/easy_tasks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-08 16:01:58.000000 easy_tasks-0.0.8/easy_tasks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 16:01:58.388882 easy_tasks-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1809 2023-06-08 16:00:23.000000 easy_tasks-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 17:24:53.731003 easy_tasks-0.0.9/
+-rw-rw-rw-   0        0        0     1095 2023-01-07 18:12:34.000000 easy_tasks-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       82 2023-01-17 17:17:39.000000 easy_tasks-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3118 2023-07-20 17:24:53.729871 easy_tasks-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2402 2023-02-14 21:25:45.000000 easy_tasks-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 17:24:53.719641 easy_tasks-0.0.9/easy_tasks/
+-rw-rw-rw-   0        0        0      944 2023-07-20 17:23:57.000000 easy_tasks-0.0.9/easy_tasks/__init__.py
+-rw-rw-rw-   0        0        0      542 2023-01-07 18:12:34.000000 easy_tasks-0.0.9/easy_tasks/closest_furthest_value.py
+-rw-rw-rw-   0        0        0     2223 2023-06-08 17:43:53.000000 easy_tasks-0.0.9/easy_tasks/dublicates.py
+-rw-rw-rw-   0        0        0      735 2023-01-07 18:12:34.000000 easy_tasks-0.0.9/easy_tasks/help_with_json.py
+-rw-rw-rw-   0        0        0      618 2023-01-07 18:12:34.000000 easy_tasks-0.0.9/easy_tasks/help_with_pickle.py
+-rw-rw-rw-   0        0        0     3627 2023-01-17 17:22:26.000000 easy_tasks-0.0.9/easy_tasks/list_printer.py
+-rw-rw-rw-   0        0        0     3614 2023-01-07 18:12:34.000000 easy_tasks-0.0.9/easy_tasks/percentage.py
+-rw-rw-rw-   0        0        0     4134 2023-07-18 20:45:23.000000 easy_tasks-0.0.9/easy_tasks/rounding.py
+-rw-rw-rw-   0        0        0      338 2023-01-07 18:12:34.000000 easy_tasks-0.0.9/easy_tasks/sorter.py
+-rw-rw-rw-   0        0        0     1437 2023-01-07 18:12:34.000000 easy_tasks-0.0.9/easy_tasks/string_transformation.py
+-rw-rw-rw-   0        0        0      909 2023-07-18 20:30:17.000000 easy_tasks-0.0.9/easy_tasks/types.py
+-rw-rw-rw-   0        0        0      654 2023-05-16 22:05:16.000000 easy_tasks-0.0.9/easy_tasks/unpack.py
+-rw-rw-rw-   0        0        0     3251 2023-07-02 22:07:15.000000 easy_tasks-0.0.9/easy_tasks/zipping.py
+drwxrwxrwx   0        0        0        0 2023-07-20 17:24:53.727357 easy_tasks-0.0.9/easy_tasks.egg-info/
+-rw-rw-rw-   0        0        0     3118 2023-07-20 17:24:53.000000 easy_tasks-0.0.9/easy_tasks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2023-07-20 17:24:53.000000 easy_tasks-0.0.9/easy_tasks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 17:24:53.000000 easy_tasks-0.0.9/easy_tasks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-20 17:24:53.000000 easy_tasks-0.0.9/easy_tasks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-20 17:24:53.000000 easy_tasks-0.0.9/easy_tasks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-20 17:24:53.731003 easy_tasks-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1809 2023-07-20 17:23:52.000000 easy_tasks-0.0.9/setup.py
```

### Comparing `easy_tasks-0.0.8/LICENSE` & `easy_tasks-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_tasks-0.0.8/PKG-INFO` & `easy_tasks-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_tasks
-Version: 0.0.8
+Version: 0.0.9
 Summary: Normal python class tasks like sorting, closet/furthest value, dublicates, ...
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easy_tasks-0.0.8/README.md` & `easy_tasks-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `easy_tasks-0.0.8/easy_tasks/closest_furthest_value.py` & `easy_tasks-0.0.9/easy_tasks/closest_furthest_value.py`

 * *Files identical despite different names*

### Comparing `easy_tasks-0.0.8/easy_tasks/dublicates.py` & `easy_tasks-0.0.9/easy_tasks/dublicates.py`

 * *Files identical despite different names*

### Comparing `easy_tasks-0.0.8/easy_tasks/help_with_json.py` & `easy_tasks-0.0.9/easy_tasks/help_with_json.py`

 * *Files identical despite different names*

### Comparing `easy_tasks-0.0.8/easy_tasks/help_with_pickle.py` & `easy_tasks-0.0.9/easy_tasks/help_with_pickle.py`

 * *Files identical despite different names*

### Comparing `easy_tasks-0.0.8/easy_tasks/list_printer.py` & `easy_tasks-0.0.9/easy_tasks/list_printer.py`

 * *Files identical despite different names*

### Comparing `easy_tasks-0.0.8/easy_tasks/percentage.py` & `easy_tasks-0.0.9/easy_tasks/percentage.py`

 * *Files identical despite different names*

### Comparing `easy_tasks-0.0.8/easy_tasks/string_transformation.py` & `easy_tasks-0.0.9/easy_tasks/string_transformation.py`

 * *Files identical despite different names*

### Comparing `easy_tasks-0.0.8/easy_tasks/unpack.py` & `easy_tasks-0.0.9/easy_tasks/unpack.py`

 * *Files identical despite different names*

### Comparing `easy_tasks-0.0.8/easy_tasks.egg-info/PKG-INFO` & `easy_tasks-0.0.9/easy_tasks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-tasks
-Version: 0.0.8
+Version: 0.0.9
 Summary: Normal python class tasks like sorting, closet/furthest value, dublicates, ...
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easy_tasks-0.0.8/setup.py` & `easy_tasks-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 DESCRIPTION = (
     "Normal python class tasks like sorting, closet/furthest value, dublicates, ..."
 )
 
 # Setting up
 setup(
     name="easy_tasks",
-    version="0.0.8",
+    version="0.0.9",
     author="André Herber",
     author_email="andre.herber.programming@gmail.com",
     # url="https://github.com/ICreedenI/xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
```

