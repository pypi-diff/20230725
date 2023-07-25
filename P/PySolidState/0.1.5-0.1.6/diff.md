# Comparing `tmp/PySolidState-0.1.5.tar.gz` & `tmp/PySolidState-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySolidState-0.1.5.tar", last modified: Mon Jul 24 02:32:42 2023, max compression
+gzip compressed data, was "PySolidState-0.1.6.tar", last modified: Mon Jul 24 23:58:53 2023, max compression
```

## Comparing `PySolidState-0.1.5.tar` & `PySolidState-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 02:32:42.571556 PySolidState-0.1.5/
--rw-rw-rw-   0        0        0     6968 2023-07-24 02:32:42.569568 PySolidState-0.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-24 02:32:42.435561 PySolidState-0.1.5/PySolidState/
--rw-rw-rw-   0        0        0        0 2023-07-22 13:45:32.000000 PySolidState-0.1.5/PySolidState/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 02:32:42.565558 PySolidState-0.1.5/PySolidState/crystal_structure/
--rw-rw-rw-   0        0        0        0 2023-07-22 13:45:32.000000 PySolidState-0.1.5/PySolidState/crystal_structure/__init__.py
--rw-rw-rw-   0        0        0      786 2023-07-22 13:45:32.000000 PySolidState-0.1.5/PySolidState/crystal_structure/atom.py
--rw-rw-rw-   0        0        0     7632 2023-07-22 13:45:32.000000 PySolidState-0.1.5/PySolidState/crystal_structure/base.py
--rw-rw-rw-   0        0        0    33207 2023-07-24 02:31:55.000000 PySolidState-0.1.5/PySolidState/crystal_structure/cell.py
--rw-rw-rw-   0        0        0     8444 2023-07-23 22:11:15.000000 PySolidState-0.1.5/PySolidState/crystal_structure/crystalStructure.py
--rw-rw-rw-   0        0        0    17396 2023-07-24 02:15:17.000000 PySolidState-0.1.5/PySolidState/crystal_structure/lattice.py
--rw-rw-rw-   0        0        0     3431 2023-07-22 17:50:07.000000 PySolidState-0.1.5/PySolidState/crystal_structure/lattices.json
-drwxrwxrwx   0        0        0        0 2023-07-24 02:32:42.510560 PySolidState-0.1.5/PySolidState.egg-info/
--rw-rw-rw-   0        0        0     6968 2023-07-24 02:32:41.000000 PySolidState-0.1.5/PySolidState.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-07-24 02:32:42.000000 PySolidState-0.1.5/PySolidState.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 02:32:41.000000 PySolidState-0.1.5/PySolidState.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-07-24 02:32:41.000000 PySolidState-0.1.5/PySolidState.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-24 02:32:41.000000 PySolidState-0.1.5/PySolidState.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6153 2023-07-22 13:45:32.000000 PySolidState-0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-24 02:32:42.572557 PySolidState-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1403 2023-07-24 02:31:59.000000 PySolidState-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 23:58:53.357066 PySolidState-0.1.6/
+-rw-rw-rw-   0        0        0    13011 2023-07-24 23:58:53.356068 PySolidState-0.1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-24 23:58:53.285068 PySolidState-0.1.6/PySolidState/
+-rw-rw-rw-   0        0        0        0 2023-07-22 13:45:32.000000 PySolidState-0.1.6/PySolidState/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 23:58:53.353067 PySolidState-0.1.6/PySolidState/crystal_structure/
+-rw-rw-rw-   0        0        0        0 2023-07-22 13:45:32.000000 PySolidState-0.1.6/PySolidState/crystal_structure/__init__.py
+-rw-rw-rw-   0        0        0      788 2023-07-24 03:10:54.000000 PySolidState-0.1.6/PySolidState/crystal_structure/atom.py
+-rw-rw-rw-   0        0        0     7632 2023-07-22 13:45:32.000000 PySolidState-0.1.6/PySolidState/crystal_structure/base.py
+-rw-rw-rw-   0        0        0    33207 2023-07-24 02:31:55.000000 PySolidState-0.1.6/PySolidState/crystal_structure/cell.py
+-rw-rw-rw-   0        0        0     8444 2023-07-23 22:11:15.000000 PySolidState-0.1.6/PySolidState/crystal_structure/crystalStructure.py
+-rw-rw-rw-   0        0        0    17396 2023-07-24 02:15:17.000000 PySolidState-0.1.6/PySolidState/crystal_structure/lattice.py
+-rw-rw-rw-   0        0        0     3431 2023-07-22 17:50:07.000000 PySolidState-0.1.6/PySolidState/crystal_structure/lattices.json
+drwxrwxrwx   0        0        0        0 2023-07-24 23:58:53.324063 PySolidState-0.1.6/PySolidState.egg-info/
+-rw-rw-rw-   0        0        0    13011 2023-07-24 23:58:52.000000 PySolidState-0.1.6/PySolidState.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-07-24 23:58:52.000000 PySolidState-0.1.6/PySolidState.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 23:58:52.000000 PySolidState-0.1.6/PySolidState.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-24 23:58:52.000000 PySolidState-0.1.6/PySolidState.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-24 23:58:52.000000 PySolidState-0.1.6/PySolidState.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    12150 2023-07-24 23:58:24.000000 PySolidState-0.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-24 23:58:53.358066 PySolidState-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1403 2023-07-24 23:58:46.000000 PySolidState-0.1.6/setup.py
```

### Comparing `PySolidState-0.1.5/PySolidState/crystal_structure/atom.py` & `PySolidState-0.1.6/PySolidState/crystal_structure/atom.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,7 +21,8 @@
             name (str): The name of the atom.
             size (float): The size of the atom.
             color (str): The color of the atom.
         """
         self.name = name
         self.size = size
         self.color = color
+
```

### Comparing `PySolidState-0.1.5/PySolidState/crystal_structure/base.py` & `PySolidState-0.1.6/PySolidState/crystal_structure/base.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.1.5/PySolidState/crystal_structure/cell.py` & `PySolidState-0.1.6/PySolidState/crystal_structure/cell.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.1.5/PySolidState/crystal_structure/crystalStructure.py` & `PySolidState-0.1.6/PySolidState/crystal_structure/crystalStructure.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.1.5/PySolidState/crystal_structure/lattice.py` & `PySolidState-0.1.6/PySolidState/crystal_structure/lattice.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.1.5/PySolidState/crystal_structure/lattices.json` & `PySolidState-0.1.6/PySolidState/crystal_structure/lattices.json`

 * *Files identical despite different names*

### Comparing `PySolidState-0.1.5/PySolidState.egg-info/SOURCES.txt` & `PySolidState-0.1.6/PySolidState.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySolidState-0.1.5/setup.py` & `PySolidState-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="PySolidState",
-    version="0.1.5",
+    version="0.1.6",
     description="PySolidState is a library developed to facilitate the study of solid-state materials, ranging from crystal structures to tight-binding models. It provides a set of tools and functionalities that enable researchers and students to analyze and simulate various aspects of the solid-state physics.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/miguelta281/PySolidState",
     author="Jose Miguel Tarazona, Yerimi Gamboa Caballero",
     author_email="miguelta281@gmail.com, jeremi0112@gmail.com",
     license="GNU General Public License v3.0",
```

