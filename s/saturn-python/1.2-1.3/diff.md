# Comparing `tmp/saturn-python-1.2.tar.gz` & `tmp/saturn-python-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saturn-python-1.2.tar", last modified: Tue Jul 25 14:07:50 2023, max compression
+gzip compressed data, was "saturn-python-1.3.tar", last modified: Tue Jul 25 14:10:43 2023, max compression
```

## Comparing `saturn-python-1.2.tar` & `saturn-python-1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 14:07:50.168319 saturn-python-1.2/
--rw-rw-rw-   0        0        0     1642 2023-07-25 14:07:50.167315 saturn-python-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1268 2023-07-25 13:54:44.000000 saturn-python-1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 14:07:50.142732 saturn-python-1.2/saturn/
--rw-rw-rw-   0        0        0     1098 2023-07-25 13:54:44.000000 saturn-python-1.2/saturn/__init__.py
--rw-rw-rw-   0        0        0      328 2023-07-25 13:54:44.000000 saturn-python-1.2/saturn/scope.py
--rw-rw-rw-   0        0        0     3414 2023-07-25 14:02:08.000000 saturn-python-1.2/saturn/terminal.py
--rw-rw-rw-   0        0        0       20 2023-07-25 14:07:29.000000 saturn-python-1.2/saturn/version.py
-drwxrwxrwx   0        0        0        0 2023-07-25 14:07:50.166356 saturn-python-1.2/saturn_python.egg-info/
--rw-rw-rw-   0        0        0     1642 2023-07-25 14:07:50.000000 saturn-python-1.2/saturn_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-07-25 14:07:50.000000 saturn-python-1.2/saturn_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 14:07:50.000000 saturn-python-1.2/saturn_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-25 14:07:50.000000 saturn-python-1.2/saturn_python.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-07-25 14:06:08.000000 saturn-python-1.2/saturn_python.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-07-25 14:07:50.000000 saturn-python-1.2/saturn_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 14:07:50.168319 saturn-python-1.2/setup.cfg
--rw-rw-rw-   0        0        0      736 2023-07-25 14:07:25.000000 saturn-python-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:10:43.990210 saturn-python-1.3/
+-rw-rw-rw-   0        0        0     1640 2023-07-25 14:10:43.989120 saturn-python-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1236 2023-07-25 14:09:17.000000 saturn-python-1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 14:10:43.972173 saturn-python-1.3/saturn/
+-rw-rw-rw-   0        0        0     1098 2023-07-25 13:54:44.000000 saturn-python-1.3/saturn/__init__.py
+-rw-rw-rw-   0        0        0      328 2023-07-25 13:54:44.000000 saturn-python-1.3/saturn/scope.py
+-rw-rw-rw-   0        0        0     3414 2023-07-25 14:02:08.000000 saturn-python-1.3/saturn/terminal.py
+-rw-rw-rw-   0        0        0       20 2023-07-25 14:09:11.000000 saturn-python-1.3/saturn/version.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:10:43.988111 saturn-python-1.3/saturn_python.egg-info/
+-rw-rw-rw-   0        0        0     1640 2023-07-25 14:10:43.000000 saturn-python-1.3/saturn_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-07-25 14:10:43.000000 saturn-python-1.3/saturn_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 14:10:43.000000 saturn-python-1.3/saturn_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-25 14:10:43.000000 saturn-python-1.3/saturn_python.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-25 14:06:08.000000 saturn-python-1.3/saturn_python.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-07-25 14:10:43.000000 saturn-python-1.3/saturn_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 14:10:43.990210 saturn-python-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      785 2023-07-25 14:10:29.000000 saturn-python-1.3/setup.py
```

### Comparing `saturn-python-1.2/PKG-INFO` & `saturn-python-1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: saturn-python
-Version: 1.2
+Version: 1.3
 Summary: Saturn allows to rerun python scripts skipping some places that were defined in previous runs.
-Home-page: UNKNOWN
+Home-page: https://github.com/fomalhaut88/saturn
 Author: Alexander Khlebushchev
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # saturn
 
@@ -14,15 +14,15 @@
 the process and keeping the scope (like it is done in
 [Jupyter Notebook](https://jupyter.org/) in code sections).
 The goal is to keep in RAM the datasets that are expensive to load in each run.
 
 ## Installation
 
 ```
-pip install git+https://github.com/fomalhaut88/saturn.git
+pip install saturn-python
 ```
 
 ## Basic example
 
 ```python
 # example.py
```

### Comparing `saturn-python-1.2/README.md` & `saturn-python-1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 the process and keeping the scope (like it is done in
 [Jupyter Notebook](https://jupyter.org/) in code sections).
 The goal is to keep in RAM the datasets that are expensive to load in each run.
 
 ## Installation
 
 ```
-pip install git+https://github.com/fomalhaut88/saturn.git
+pip install saturn-python
 ```
 
 ## Basic example
 
 ```python
 # example.py
```

### Comparing `saturn-python-1.2/saturn/__init__.py` & `saturn-python-1.3/saturn/__init__.py`

 * *Files identical despite different names*

### Comparing `saturn-python-1.2/saturn/terminal.py` & `saturn-python-1.3/saturn/terminal.py`

 * *Files identical despite different names*

### Comparing `saturn-python-1.2/saturn_python.egg-info/PKG-INFO` & `saturn-python-1.3/saturn_python.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: saturn-python
-Version: 1.2
+Version: 1.3
 Summary: Saturn allows to rerun python scripts skipping some places that were defined in previous runs.
-Home-page: UNKNOWN
+Home-page: https://github.com/fomalhaut88/saturn
 Author: Alexander Khlebushchev
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # saturn
 
@@ -14,15 +14,15 @@
 the process and keeping the scope (like it is done in
 [Jupyter Notebook](https://jupyter.org/) in code sections).
 The goal is to keep in RAM the datasets that are expensive to load in each run.
 
 ## Installation
 
 ```
-pip install git+https://github.com/fomalhaut88/saturn.git
+pip install saturn-python
 ```
 
 ## Basic example
 
 ```python
 # example.py
```

### Comparing `saturn-python-1.2/setup.py` & `saturn-python-1.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     name='saturn-python',
     version=__version__,
     description="Saturn allows to rerun python scripts skipping some places that were defined in previous runs.",
     author='Alexander Khlebushchev',
     packages=[
         'saturn',
     ],
+    url="https://github.com/fomalhaut88/saturn",
     license="MIT",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     zip_safe=False,
     entry_points={
         'console_scripts': ['saturn=saturn.terminal:main'],
     },
```

