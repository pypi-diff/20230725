# Comparing `tmp/bokeh-resources-0.3.tar.gz` & `tmp/bokeh-resources-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bokeh-resources-0.3.tar", last modified: Thu Mar  9 16:48:26 2023, max compression
+gzip compressed data, was "bokeh-resources-0.4.tar", last modified: Tue Jul 25 03:56:15 2023, max compression
```

## Comparing `bokeh-resources-0.3.tar` & `bokeh-resources-0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-09 16:48:26.283152 bokeh-resources-0.3/
--rw-rw-rw-   0        0        0     2466 2023-03-09 16:48:26.282145 bokeh-resources-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1877 2023-03-09 16:47:23.000000 bokeh-resources-0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-03-09 16:48:26.238145 bokeh-resources-0.3/bokeh_resources/
--rw-rw-rw-   0        0        0       19 2023-03-09 16:47:49.000000 bokeh-resources-0.3/bokeh_resources/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-09 16:48:26.280146 bokeh-resources-0.3/bokeh_resources/bokeh_resources/
--rw-rw-rw-   0        0        0      214 2022-06-21 11:10:49.000000 bokeh-resources-0.3/bokeh_resources/bokeh_resources/main.js
--rw-rw-rw-   0        0        0      721 2023-03-09 16:43:15.000000 bokeh-resources-0.3/bokeh_resources/install.py
-drwxrwxrwx   0        0        0        0 2023-03-09 16:48:26.276146 bokeh-resources-0.3/bokeh_resources.egg-info/
--rw-rw-rw-   0        0        0     2466 2023-03-09 16:48:26.000000 bokeh-resources-0.3/bokeh_resources.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2023-03-09 16:48:26.000000 bokeh-resources-0.3/bokeh_resources.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-09 16:48:26.000000 bokeh-resources-0.3/bokeh_resources.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-06-20 19:15:29.000000 bokeh-resources-0.3/bokeh_resources.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2023-03-09 16:48:26.000000 bokeh-resources-0.3/bokeh_resources.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-03-09 16:48:26.000000 bokeh-resources-0.3/bokeh_resources.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-09 16:48:26.284150 bokeh-resources-0.3/setup.cfg
--rw-rw-rw-   0        0        0      877 2023-03-09 16:47:32.000000 bokeh-resources-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 03:56:15.414875 bokeh-resources-0.4/
+-rw-rw-rw-   0        0        0     2466 2023-07-25 03:56:15.413874 bokeh-resources-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1877 2023-03-09 16:47:23.000000 bokeh-resources-0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 03:56:15.366876 bokeh-resources-0.4/bokeh_resources/
+-rw-rw-rw-   0        0        0       19 2023-07-25 03:56:05.000000 bokeh-resources-0.4/bokeh_resources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 03:56:15.411875 bokeh-resources-0.4/bokeh_resources/bokeh_resources/
+-rw-rw-rw-   0        0        0      214 2022-06-21 11:10:49.000000 bokeh-resources-0.4/bokeh_resources/bokeh_resources/main.js
+-rw-rw-rw-   0        0        0      721 2023-03-09 16:43:15.000000 bokeh-resources-0.4/bokeh_resources/install.py
+drwxrwxrwx   0        0        0        0 2023-07-25 03:56:15.409876 bokeh-resources-0.4/bokeh_resources.egg-info/
+-rw-rw-rw-   0        0        0     2466 2023-07-25 03:56:15.000000 bokeh-resources-0.4/bokeh_resources.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2023-07-25 03:56:15.000000 bokeh-resources-0.4/bokeh_resources.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 03:56:15.000000 bokeh-resources-0.4/bokeh_resources.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-06-20 19:15:29.000000 bokeh-resources-0.4/bokeh_resources.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       44 2023-07-25 03:56:15.000000 bokeh-resources-0.4/bokeh_resources.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-25 03:56:15.000000 bokeh-resources-0.4/bokeh_resources.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 03:56:15.414875 bokeh-resources-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      909 2023-07-25 03:55:38.000000 bokeh-resources-0.4/setup.py
```

### Comparing `bokeh-resources-0.3/PKG-INFO` & `bokeh-resources-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bokeh-resources
-Version: 0.3
+Version: 0.4
 Summary: Jupyter extension to serve bokeh resources (js and css files).
 Home-page: https://github.com/axil/bokeh-resources
 Author: Lev Maximov
 Author-email: lev.maximov@gmail.com
 License: MIT License
 Keywords: bokeh,jupyter,notebook
 Platform: UNKNOWN
```

### Comparing `bokeh-resources-0.3/README.md` & `bokeh-resources-0.4/README.md`

 * *Files identical despite different names*

### Comparing `bokeh-resources-0.3/bokeh_resources/install.py` & `bokeh-resources-0.4/bokeh_resources/install.py`

 * *Files identical despite different names*

### Comparing `bokeh-resources-0.3/bokeh_resources.egg-info/PKG-INFO` & `bokeh-resources-0.4/bokeh_resources.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bokeh-resources
-Version: 0.3
+Version: 0.4
 Summary: Jupyter extension to serve bokeh resources (js and css files).
 Home-page: https://github.com/axil/bokeh-resources
 Author: Lev Maximov
 Author-email: lev.maximov@gmail.com
 License: MIT License
 Keywords: bokeh,jupyter,notebook
 Platform: UNKNOWN
```

### Comparing `bokeh-resources-0.3/setup.py` & `bokeh-resources-0.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="bokeh-resources",
-    version="0.3",
+    version="0.4",
     author='Lev Maximov',
     author_email='lev.maximov@gmail.com',
     url='https://github.com/axil/bokeh-resources',
     description="Jupyter extension to serve bokeh resources (js and css files).",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=['bokeh', 'notebook'],
+    install_requires=['bokeh', 'notebook', 'jupyter_contrib_nbextensions'],
     packages=['bokeh_resources', 'bokeh_resources.bokeh_resources'],
     package_data={'': ['*.js']},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

