# Comparing `tmp/Widget_Controller-2.0.tar.gz` & `tmp/Widget_Controller-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Widget Controller-2.0.tar", last modified: Tue Jul 25 02:42:21 2023, max compression
+gzip compressed data, was "Widget Controller-2.0.1.tar", last modified: Tue Jul 25 03:16:09 2023, max compression
```

## Comparing `Widget_Controller-2.0.tar` & `Widget_Controller-2.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 02:42:21.333649 Widget Controller-2.0/
--rw-rw-rw-   0        0        0     2238 2023-06-12 17:07:48.000000 Widget Controller-2.0/LICENSE.txt
--rw-rw-rw-   0        0        0     4029 2023-07-25 02:42:21.331629 Widget Controller-2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3551 2023-06-29 02:47:43.000000 Widget Controller-2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 02:42:21.274529 Widget Controller-2.0/WC/
--rw-rw-rw-   0        0        0    14920 2023-07-24 21:48:00.000000 Widget Controller-2.0/WC/WC.py
--rw-rw-rw-   0        0        0       16 2023-07-25 02:33:39.000000 Widget Controller-2.0/WC/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 02:42:21.327747 Widget Controller-2.0/Widget_Controller.egg-info/
--rw-rw-rw-   0        0        0     4029 2023-07-25 02:42:21.000000 Widget Controller-2.0/Widget_Controller.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-07-25 02:42:21.000000 Widget Controller-2.0/Widget_Controller.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 02:42:21.000000 Widget Controller-2.0/Widget_Controller.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        3 2023-07-25 02:42:21.000000 Widget Controller-2.0/Widget_Controller.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 02:42:21.334635 Widget Controller-2.0/setup.cfg
--rw-rw-rw-   0        0        0      649 2023-07-25 02:42:17.000000 Widget Controller-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 03:16:09.074127 Widget Controller-2.0.1/
+-rw-rw-rw-   0        0        0     2238 2023-06-12 17:07:48.000000 Widget Controller-2.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     4063 2023-07-25 03:16:09.074127 Widget Controller-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3551 2023-06-29 02:47:43.000000 Widget Controller-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 03:16:09.002124 Widget Controller-2.0.1/WC/
+-rw-rw-rw-   0        0        0    14920 2023-07-24 21:48:00.000000 Widget Controller-2.0.1/WC/WC.py
+-rw-rw-rw-   0        0        0       19 2023-07-25 02:48:03.000000 Widget Controller-2.0.1/WC/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 03:16:09.066238 Widget Controller-2.0.1/Widget_Controller.egg-info/
+-rw-rw-rw-   0        0        0     4063 2023-07-25 03:16:08.000000 Widget Controller-2.0.1/Widget_Controller.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-07-25 03:16:08.000000 Widget Controller-2.0.1/Widget_Controller.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 03:16:08.000000 Widget Controller-2.0.1/Widget_Controller.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        3 2023-07-25 03:16:08.000000 Widget Controller-2.0.1/Widget_Controller.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 03:16:09.074127 Widget Controller-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      689 2023-07-25 03:15:53.000000 Widget Controller-2.0.1/setup.py
```

### Comparing `Widget Controller-2.0/LICENSE.txt` & `Widget Controller-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Widget Controller-2.0/PKG-INFO` & `Widget Controller-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: Widget Controller
-Version: 2.0
+Version: 2.0.1
 Summary: Una libreria para crear facilmente UI (traducido de Tkinter y otros)
 Home-page: https://github.com/Z3R0GT/WC
 Download-URL: https://github.com/Z3R0GT/WC/releases/tag/BUILD-2.0
 Author: Z3R0_GT
 Author-email: contac.es.z3r0.gt@gmail.com
 License: OTHER
 Keywords: ui,UI,Tkinter,logging,build
+Requires: Tk
+Requires: Pillow
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ![logo](logo.png)
 
 # WC
 Window Controller (controlador de ventanas) o WC es una libreria que empaqueta otras tanto grandes como pequeÃ±as, proveyendo multiples funciones para facilitar el crear GUIs, creado por
```

### Comparing `Widget Controller-2.0/README.md` & `Widget Controller-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `Widget Controller-2.0/WC/WC.py` & `Widget Controller-2.0.1/WC/WC.py`

 * *Files identical despite different names*

### Comparing `Widget Controller-2.0/Widget_Controller.egg-info/PKG-INFO` & `Widget Controller-2.0.1/Widget_Controller.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: Widget-Controller
-Version: 2.0
+Version: 2.0.1
 Summary: Una libreria para crear facilmente UI (traducido de Tkinter y otros)
 Home-page: https://github.com/Z3R0GT/WC
 Download-URL: https://github.com/Z3R0GT/WC/releases/tag/BUILD-2.0
 Author: Z3R0_GT
 Author-email: contac.es.z3r0.gt@gmail.com
 License: OTHER
 Keywords: ui,UI,Tkinter,logging,build
+Requires: Tk
+Requires: Pillow
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ![logo](logo.png)
 
 # WC
 Window Controller (controlador de ventanas) o WC es una libreria que empaqueta otras tanto grandes como pequeÃ±as, proveyendo multiples funciones para facilitar el crear GUIs, creado por
```

### Comparing `Widget Controller-2.0/setup.py` & `Widget Controller-2.0.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from setuptools import setup
 
 readme = open("./README.md", "r")
 
 setup(
     name="Widget Controller",
     packages=["WC"],
-    version="2.0",
+    version="2.0.1",
     description="Una libreria para crear facilmente UI (traducido de Tkinter y otros)",
     long_description=readme.read(),
     long_description_content_type="text/markdown",
     author="Z3R0_GT",
     author_email="contac.es.z3r0.gt@gmail.com",
     url="https://github.com/Z3R0GT/WC",
     download_url="https://github.com/Z3R0GT/WC/releases/tag/BUILD-2.0",
     keywords=["ui", "UI", "Tkinter", "logging", "build"],
     classifiers=[ ],
+    requires=["Tk", "Pillow"],
     license="OTHER",
+    
     include_package_data=True
 )
```

