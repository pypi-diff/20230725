# Comparing `tmp/MiPaquetePublicable-0.0.1.tar.gz` & `tmp/MiPaquetePublicable-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MiPaquetePublicable-0.0.1.tar", last modified: Tue Jul 25 04:08:24 2023, max compression
+gzip compressed data, was "MiPaquetePublicable-0.0.2.tar", last modified: Tue Jul 25 20:32:33 2023, max compression
```

## Comparing `MiPaquetePublicable-0.0.1.tar` & `MiPaquetePublicable-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 04:08:24.860340 MiPaquetePublicable-0.0.1/
--rw-rw-rw-   0        0        0        0 2023-07-24 01:26:50.000000 MiPaquetePublicable-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     6621 2023-07-25 04:08:24.858351 MiPaquetePublicable-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6004 2023-07-25 02:03:03.000000 MiPaquetePublicable-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-25 04:08:24.860340 MiPaquetePublicable-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      655 2023-07-25 01:57:32.000000 MiPaquetePublicable-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 04:08:24.826751 MiPaquetePublicable-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-25 04:08:24.841342 MiPaquetePublicable-0.0.1/src/MiPaquetePublicable.egg-info/
--rw-rw-rw-   0        0        0     6621 2023-07-25 04:08:24.000000 MiPaquetePublicable-0.0.1/src/MiPaquetePublicable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-07-25 04:08:24.000000 MiPaquetePublicable-0.0.1/src/MiPaquetePublicable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 04:08:24.000000 MiPaquetePublicable-0.0.1/src/MiPaquetePublicable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-25 04:08:24.000000 MiPaquetePublicable-0.0.1/src/MiPaquetePublicable.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-07-24 23:33:10.000000 MiPaquetePublicable-0.0.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 04:08:24.848343 MiPaquetePublicable-0.0.1/src/compuestos/
--rw-rw-rw-   0        0        0       62 2023-07-25 01:39:38.000000 MiPaquetePublicable-0.0.1/src/compuestos/__init__.py
--rw-rw-rw-   0        0        0     4113 2023-07-24 04:34:21.000000 MiPaquetePublicable-0.0.1/src/compuestos/funciones_avanzadas.py
-drwxrwxrwx   0        0        0        0 2023-07-25 04:08:24.854339 MiPaquetePublicable-0.0.1/src/elementales/
--rw-rw-rw-   0        0        0       61 2023-07-25 01:28:14.000000 MiPaquetePublicable-0.0.1/src/elementales/__init__.py
--rw-rw-rw-   0        0        0     2191 2023-07-25 01:38:01.000000 MiPaquetePublicable-0.0.1/src/elementales/funciones_basicas.py
+drwxrwxrwx   0        0        0        0 2023-07-25 20:32:33.708360 MiPaquetePublicable-0.0.2/
+-rw-rw-rw-   0        0        0        0 2023-07-24 01:26:50.000000 MiPaquetePublicable-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     6621 2023-07-25 20:32:33.707317 MiPaquetePublicable-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6004 2023-07-25 02:03:03.000000 MiPaquetePublicable-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-25 20:32:33.708360 MiPaquetePublicable-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      655 2023-07-25 20:30:47.000000 MiPaquetePublicable-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 20:32:33.671314 MiPaquetePublicable-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-25 20:32:33.689313 MiPaquetePublicable-0.0.2/src/MiPaquetePublicable.egg-info/
+-rw-rw-rw-   0        0        0     6621 2023-07-25 20:32:33.000000 MiPaquetePublicable-0.0.2/src/MiPaquetePublicable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-07-25 20:32:33.000000 MiPaquetePublicable-0.0.2/src/MiPaquetePublicable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 20:32:33.000000 MiPaquetePublicable-0.0.2/src/MiPaquetePublicable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-25 20:32:33.000000 MiPaquetePublicable-0.0.2/src/MiPaquetePublicable.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-07-24 23:33:10.000000 MiPaquetePublicable-0.0.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 20:32:33.696315 MiPaquetePublicable-0.0.2/src/compuestos/
+-rw-rw-rw-   0        0        0       62 2023-07-25 01:39:38.000000 MiPaquetePublicable-0.0.2/src/compuestos/__init__.py
+-rw-rw-rw-   0        0        0     4113 2023-07-24 04:34:21.000000 MiPaquetePublicable-0.0.2/src/compuestos/funciones_avanzadas.py
+drwxrwxrwx   0        0        0        0 2023-07-25 20:32:33.704317 MiPaquetePublicable-0.0.2/src/elementales/
+-rw-rw-rw-   0        0        0       61 2023-07-25 01:28:14.000000 MiPaquetePublicable-0.0.2/src/elementales/__init__.py
+-rw-rw-rw-   0        0        0     2191 2023-07-25 01:38:01.000000 MiPaquetePublicable-0.0.2/src/elementales/funciones_basicas.py
```

### Comparing `MiPaquetePublicable-0.0.1/PKG-INFO` & `MiPaquetePublicable-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MiPaquetePublicable
-Version: 0.0.1
+Version: 0.0.2
 Summary: Descripción del paquete
 Home-page: https://github.com/JorgeCardona/recursos/Publicar Paquetes PyPI
 Author: Jorge Cardona
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `MiPaquetePublicable-0.0.1/README.md` & `MiPaquetePublicable-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `MiPaquetePublicable-0.0.1/setup.py` & `MiPaquetePublicable-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 setuptools.setup(
     name="MiPaquetePublicable",
-    version="0.0.1",
+    version="0.0.2",
     author="Jorge Cardona",
     description="Descripción del paquete",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JorgeCardona/recursos/Publicar Paquetes PyPI",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `MiPaquetePublicable-0.0.1/src/MiPaquetePublicable.egg-info/PKG-INFO` & `MiPaquetePublicable-0.0.2/src/MiPaquetePublicable.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MiPaquetePublicable
-Version: 0.0.1
+Version: 0.0.2
 Summary: Descripción del paquete
 Home-page: https://github.com/JorgeCardona/recursos/Publicar Paquetes PyPI
 Author: Jorge Cardona
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `MiPaquetePublicable-0.0.1/src/compuestos/funciones_avanzadas.py` & `MiPaquetePublicable-0.0.2/src/compuestos/funciones_avanzadas.py`

 * *Files identical despite different names*

### Comparing `MiPaquetePublicable-0.0.1/src/elementales/funciones_basicas.py` & `MiPaquetePublicable-0.0.2/src/elementales/funciones_basicas.py`

 * *Files identical despite different names*

