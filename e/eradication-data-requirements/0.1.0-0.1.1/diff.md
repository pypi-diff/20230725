# Comparing `tmp/eradication_data_requirements-0.1.0.tar.gz` & `tmp/eradication_data_requirements-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eradication_data_requirements-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "eradication_data_requirements-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `eradication_data_requirements-0.1.0.tar` & `eradication_data_requirements-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      151 2023-06-01 17:08:30.815636 eradication_data_requirements-0.1.0/README.md
--rw-r--r--   0        0        0      102 2023-06-01 17:08:30.815636 eradication_data_requirements-0.1.0/eradication_data_requirements/__init__.py
--rw-r--r--   0        0        0       76 2023-06-01 17:08:30.815636 eradication_data_requirements-0.1.0/eradication_data_requirements/transformations.py
--rw-r--r--   0        0        0      466 2023-06-01 17:08:30.815636 eradication_data_requirements-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      555 1970-01-01 00:00:00.000000 eradication_data_requirements-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      151 2023-07-25 18:54:18.636286 eradication_data_requirements-0.1.1/README.md
+-rw-r--r--   0        0        0      100 2023-07-25 18:54:18.636286 eradication_data_requirements-0.1.1/eradication_data_requirements/__init__.py
+-rw-r--r--   0        0        0      694 2023-07-25 18:54:18.636286 eradication_data_requirements-0.1.1/eradication_data_requirements/data_requirements_plot.py
+-rw-r--r--   0        0        0      518 2023-07-25 18:54:18.636286 eradication_data_requirements-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 eradication_data_requirements-0.1.1/PKG-INFO
```

### Comparing `eradication_data_requirements-0.1.0/PKG-INFO` & `eradication_data_requirements-0.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: eradication_data_requirements
-Version: 0.1.0
+Version: 0.1.1
 Summary: A template Python module
 Home-page: https://github.com/IslasGECI/eradication_data_requirements
 Author: Ciencia de Datos • GECI
 Author-email: ciencia.datos@islas.org.mx
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Requires-Dist: geci-plots==0.4.*
+Requires-Dist: numpy
+Requires-Dist: pandas
 
 <a href="https://www.islas.org.mx/"><img src="https://www.islas.org.mx/img/logo.svg" align="right" width="256" /></a>
 # Eradication Data Requirements
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
-Metadata-Version: 2.1 Name: eradication_data_requirements Version: 0.1.0
+Metadata-Version: 2.1 Name: eradication_data_requirements Version: 0.1.1
 Summary: A template Python module Home-page: https://github.com/IslasGECI/
 eradication_data_requirements Author: Ciencia de Datos â¢ GECI Author-email:
 ciencia.datos@islas.org.mx Requires-Python: >=3.9 Description-Content-Type:
 text/markdown Classifier: License :: OSI Approved :: GNU General Public License
-v3 or later (GPLv3+) [https://www.islas.org.mx/img/logo.svg] # Eradication Data
-Requirements
+v3 or later (GPLv3+) Requires-Dist: geci-plots==0.4.* Requires-Dist: numpy
+Requires-Dist: pandas [https://www.islas.org.mx/img/logo.svg] # Eradication
+Data Requirements
```

