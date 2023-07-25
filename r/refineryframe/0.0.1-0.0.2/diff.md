# Comparing `tmp/refineryframe-0.0.1.tar.gz` & `tmp/refineryframe-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refineryframe-0.0.1.tar", last modified: Tue Jul 25 01:34:20 2023, max compression
+gzip compressed data, was "refineryframe-0.0.2.tar", last modified: Tue Jul 25 11:32:17 2023, max compression
```

## Comparing `refineryframe-0.0.1.tar` & `refineryframe-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 insani_dei   (501) staff       (20)        0 2023-07-25 01:34:20.401320 refineryframe-0.0.1/
--rw-r--r--   0 insani_dei   (501) staff       (20)    12096 2023-07-25 01:34:20.400973 refineryframe-0.0.1/PKG-INFO
--rw-r--r--   0 insani_dei   (501) staff       (20)    11542 2023-07-25 01:29:26.000000 refineryframe-0.0.1/README.md
-drwxr-xr-x   0 insani_dei   (501) staff       (20)        0 2023-07-25 01:34:20.398765 refineryframe-0.0.1/refineryframe/
--rw-r--r--   0 insani_dei   (501) staff       (20)       38 2023-07-25 00:45:03.000000 refineryframe-0.0.1/refineryframe/__init__.py
--rw-r--r--   0 insani_dei   (501) staff       (20)    72863 2023-07-25 01:27:37.000000 refineryframe-0.0.1/refineryframe/tns.py
-drwxr-xr-x   0 insani_dei   (501) staff       (20)        0 2023-07-25 01:34:20.400573 refineryframe-0.0.1/refineryframe.egg-info/
--rw-r--r--   0 insani_dei   (501) staff       (20)    12096 2023-07-25 01:34:20.000000 refineryframe-0.0.1/refineryframe.egg-info/PKG-INFO
--rw-r--r--   0 insani_dei   (501) staff       (20)      249 2023-07-25 01:34:20.000000 refineryframe-0.0.1/refineryframe.egg-info/SOURCES.txt
--rw-r--r--   0 insani_dei   (501) staff       (20)        1 2023-07-25 01:34:20.000000 refineryframe-0.0.1/refineryframe.egg-info/dependency_links.txt
--rw-r--r--   0 insani_dei   (501) staff       (20)       45 2023-07-25 01:34:20.000000 refineryframe-0.0.1/refineryframe.egg-info/requires.txt
--rw-r--r--   0 insani_dei   (501) staff       (20)       14 2023-07-25 01:34:20.000000 refineryframe-0.0.1/refineryframe.egg-info/top_level.txt
--rw-r--r--   0 insani_dei   (501) staff       (20)       38 2023-07-25 01:34:20.401409 refineryframe-0.0.1/setup.cfg
--rw-r--r--   0 insani_dei   (501) staff       (20)     1183 2023-07-25 00:39:20.000000 refineryframe-0.0.1/setup.py
+drwxr-xr-x   0 insani_dei   (501) staff       (20)        0 2023-07-25 11:32:17.440684 refineryframe-0.0.2/
+-rw-r--r--   0 insani_dei   (501) staff       (20)    12174 2023-07-25 11:32:17.440412 refineryframe-0.0.2/PKG-INFO
+-rw-r--r--   0 insani_dei   (501) staff       (20)    11620 2023-07-25 01:50:42.000000 refineryframe-0.0.2/README.md
+drwxr-xr-x   0 insani_dei   (501) staff       (20)        0 2023-07-25 11:32:17.438787 refineryframe-0.0.2/refineryframe/
+-rw-r--r--   0 insani_dei   (501) staff       (20)       38 2023-07-25 00:45:03.000000 refineryframe-0.0.2/refineryframe/__init__.py
+-rw-r--r--   0 insani_dei   (501) staff       (20)    72863 2023-07-25 01:27:37.000000 refineryframe-0.0.2/refineryframe/tns.py
+drwxr-xr-x   0 insani_dei   (501) staff       (20)        0 2023-07-25 11:32:17.440076 refineryframe-0.0.2/refineryframe.egg-info/
+-rw-r--r--   0 insani_dei   (501) staff       (20)    12174 2023-07-25 11:32:17.000000 refineryframe-0.0.2/refineryframe.egg-info/PKG-INFO
+-rw-r--r--   0 insani_dei   (501) staff       (20)      249 2023-07-25 11:32:17.000000 refineryframe-0.0.2/refineryframe.egg-info/SOURCES.txt
+-rw-r--r--   0 insani_dei   (501) staff       (20)        1 2023-07-25 11:32:17.000000 refineryframe-0.0.2/refineryframe.egg-info/dependency_links.txt
+-rw-r--r--   0 insani_dei   (501) staff       (20)       37 2023-07-25 11:32:17.000000 refineryframe-0.0.2/refineryframe.egg-info/requires.txt
+-rw-r--r--   0 insani_dei   (501) staff       (20)       14 2023-07-25 11:32:17.000000 refineryframe-0.0.2/refineryframe.egg-info/top_level.txt
+-rw-r--r--   0 insani_dei   (501) staff       (20)       38 2023-07-25 11:32:17.440766 refineryframe-0.0.2/setup.cfg
+-rw-r--r--   0 insani_dei   (501) staff       (20)     1173 2023-07-25 11:31:58.000000 refineryframe-0.0.2/setup.py
```

### Comparing `refineryframe-0.0.1/PKG-INFO` & `refineryframe-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refineryframe
-Version: 0.0.1
+Version: 0.0.2
 Summary: Cleans data, best to be used as a part of initial preprocessor
 Author: Kyrylo Mordan
 Author-email: <parachute.repo@gmail.com>
 Keywords: python,data cleaning,safeguards
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,17 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 
 # refineryframe
 
+<a><img src="images/logo.png" width="35%" height="35%" align="right" /></a>
+
+
 Under construction! Not ready for use yet! Currently experimenting and planning!
 
 ## Initial plans
 
 Goal of the package is to simplify life for data scientist that have to deal with imperfect raw data. The pachage suppose to detect and clean unexpected values, while doubling as safeguard in production code based on predifined conditions that arise from business assumptions or any other source. The package is well suited to be an initial preprocessing step in ml pipelines situated between data gathering and training/scoring steps.
 
 Developed by Kyrylo Mordan (c) 2023
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: refineryframe Version: 0.0.1 Summary: Cleans data,
+Metadata-Version: 2.1 Name: refineryframe Version: 0.0.2 Summary: Cleans data,
 best to be used as a part of initial preprocessor Author: Kyrylo Mordan Author-
 email:
 repo@gmail.com> Keywords: python,data cleaning,safeguards Classifier:
 Development Status :: 1 - Planning Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 Unix Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating
 System :: Microsoft :: Windows Description-Content-Type: text/markdown #
-refineryframe Under construction! Not ready for use yet! Currently
-experimenting and planning! ## Initial plans Goal of the package is to simplify
-life for data scientist that have to deal with imperfect raw data. The pachage
-suppose to detect and clean unexpected values, while doubling as safeguard in
-production code based on predifined conditions that arise from business
-assumptions or any other source. The package is well suited to be an initial
-preprocessing step in ml pipelines situated between data gathering and
+refineryframe [images/logo.png] Under construction! Not ready for use yet!
+Currently experimenting and planning! ## Initial plans Goal of the package is
+to simplify life for data scientist that have to deal with imperfect raw data.
+The pachage suppose to detect and clean unexpected values, while doubling as
+safeguard in production code based on predifined conditions that arise from
+business assumptions or any other source. The package is well suited to be an
+initial preprocessing step in ml pipelines situated between data gathering and
 training/scoring steps. Developed by Kyrylo Mordan (c) 2023 ## Package usage
 example ### Creating example data (exceptionally messy dataframe) ```python df
 = pd.DataFrame({ 'num_id' : [1, 2, 3, 4, 5], 'NumericColumn': [1, -np.inf,
 np.inf,np.nan, None], 'NumericColumn_exepted': [1, -996, np.inf,np.nan, None],
 'NumericColumn2': [None, None, 1,None, None], 'NumericColumn3': [1, 2, 3, 4,
 5], 'DateColumn': pd.date_range(start='2022-01-01', periods=5), 'DateColumn2':
 [pd.NaT,pd.to_datetime('2022-01-01'),pd.NaT,pd.NaT,pd.NaT], 'DateColumn3':
```

### Comparing `refineryframe-0.0.1/README.md` & `refineryframe-0.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # refineryframe
 
+<a><img src="images/logo.png" width="35%" height="35%" align="right" /></a>
+
+
 Under construction! Not ready for use yet! Currently experimenting and planning!
 
 ## Initial plans
 
 Goal of the package is to simplify life for data scientist that have to deal with imperfect raw data. The pachage suppose to detect and clean unexpected values, while doubling as safeguard in production code based on predifined conditions that arise from business assumptions or any other source. The package is well suited to be an initial preprocessing step in ml pipelines situated between data gathering and training/scoring steps.
 
 Developed by Kyrylo Mordan (c) 2023
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-# refineryframe Under construction! Not ready for use yet! Currently
-experimenting and planning! ## Initial plans Goal of the package is to simplify
-life for data scientist that have to deal with imperfect raw data. The pachage
-suppose to detect and clean unexpected values, while doubling as safeguard in
-production code based on predifined conditions that arise from business
-assumptions or any other source. The package is well suited to be an initial
-preprocessing step in ml pipelines situated between data gathering and
+# refineryframe [images/logo.png] Under construction! Not ready for use yet!
+Currently experimenting and planning! ## Initial plans Goal of the package is
+to simplify life for data scientist that have to deal with imperfect raw data.
+The pachage suppose to detect and clean unexpected values, while doubling as
+safeguard in production code based on predifined conditions that arise from
+business assumptions or any other source. The package is well suited to be an
+initial preprocessing step in ml pipelines situated between data gathering and
 training/scoring steps. Developed by Kyrylo Mordan (c) 2023 ## Package usage
 example ### Creating example data (exceptionally messy dataframe) ```python df
 = pd.DataFrame({ 'num_id' : [1, 2, 3, 4, 5], 'NumericColumn': [1, -np.inf,
 np.inf,np.nan, None], 'NumericColumn_exepted': [1, -996, np.inf,np.nan, None],
 'NumericColumn2': [None, None, 1,None, None], 'NumericColumn3': [1, 2, 3, 4,
 5], 'DateColumn': pd.date_range(start='2022-01-01', periods=5), 'DateColumn2':
 [pd.NaT,pd.to_datetime('2022-01-01'),pd.NaT,pd.NaT,pd.NaT], 'DateColumn3':
```

### Comparing `refineryframe-0.0.1/refineryframe/tns.py` & `refineryframe-0.0.2/refineryframe/tns.py`

 * *Files identical despite different names*

### Comparing `refineryframe-0.0.1/refineryframe.egg-info/PKG-INFO` & `refineryframe-0.0.2/refineryframe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refineryframe
-Version: 0.0.1
+Version: 0.0.2
 Summary: Cleans data, best to be used as a part of initial preprocessor
 Author: Kyrylo Mordan
 Author-email: <parachute.repo@gmail.com>
 Keywords: python,data cleaning,safeguards
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,17 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 
 # refineryframe
 
+<a><img src="images/logo.png" width="35%" height="35%" align="right" /></a>
+
+
 Under construction! Not ready for use yet! Currently experimenting and planning!
 
 ## Initial plans
 
 Goal of the package is to simplify life for data scientist that have to deal with imperfect raw data. The pachage suppose to detect and clean unexpected values, while doubling as safeguard in production code based on predifined conditions that arise from business assumptions or any other source. The package is well suited to be an initial preprocessing step in ml pipelines situated between data gathering and training/scoring steps.
 
 Developed by Kyrylo Mordan (c) 2023
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: refineryframe Version: 0.0.1 Summary: Cleans data,
+Metadata-Version: 2.1 Name: refineryframe Version: 0.0.2 Summary: Cleans data,
 best to be used as a part of initial preprocessor Author: Kyrylo Mordan Author-
 email:
 repo@gmail.com> Keywords: python,data cleaning,safeguards Classifier:
 Development Status :: 1 - Planning Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 Unix Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating
 System :: Microsoft :: Windows Description-Content-Type: text/markdown #
-refineryframe Under construction! Not ready for use yet! Currently
-experimenting and planning! ## Initial plans Goal of the package is to simplify
-life for data scientist that have to deal with imperfect raw data. The pachage
-suppose to detect and clean unexpected values, while doubling as safeguard in
-production code based on predifined conditions that arise from business
-assumptions or any other source. The package is well suited to be an initial
-preprocessing step in ml pipelines situated between data gathering and
+refineryframe [images/logo.png] Under construction! Not ready for use yet!
+Currently experimenting and planning! ## Initial plans Goal of the package is
+to simplify life for data scientist that have to deal with imperfect raw data.
+The pachage suppose to detect and clean unexpected values, while doubling as
+safeguard in production code based on predifined conditions that arise from
+business assumptions or any other source. The package is well suited to be an
+initial preprocessing step in ml pipelines situated between data gathering and
 training/scoring steps. Developed by Kyrylo Mordan (c) 2023 ## Package usage
 example ### Creating example data (exceptionally messy dataframe) ```python df
 = pd.DataFrame({ 'num_id' : [1, 2, 3, 4, 5], 'NumericColumn': [1, -np.inf,
 np.inf,np.nan, None], 'NumericColumn_exepted': [1, -996, np.inf,np.nan, None],
 'NumericColumn2': [None, None, 1,None, None], 'NumericColumn3': [1, 2, 3, 4,
 5], 'DateColumn': pd.date_range(start='2022-01-01', periods=5), 'DateColumn2':
 [pd.NaT,pd.to_datetime('2022-01-01'),pd.NaT,pd.NaT,pd.NaT], 'DateColumn3':
```

### Comparing `refineryframe-0.0.1/setup.py` & `refineryframe-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Cleans data, best to be used as a part of initial preprocessor'
 LONG_DESCRIPTION = 'A package that allows to detect unexpected values in data and clean them in production python ml code'
 
 # Setting up
 setup(
     name="refineryframe",
     version=VERSION,
     author="Kyrylo Mordan",
     author_email="<parachute.repo@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['logging','datetime','pandas','numpy','unidecode','attr'],
+    install_requires=['datetime','pandas','numpy','unidecode','attr'],
     keywords=['python', 'data cleaning', 'safeguards'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

