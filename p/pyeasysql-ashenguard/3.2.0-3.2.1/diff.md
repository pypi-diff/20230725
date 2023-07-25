# Comparing `tmp/pyeasysql_ashenguard-3.2.0.tar.gz` & `tmp/pyeasysql_ashenguard-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeasysql_ashenguard-3.2.0.tar", last modified: Mon Jul 24 19:30:01 2023, max compression
+gzip compressed data, was "pyeasysql_ashenguard-3.2.1.tar", last modified: Tue Jul 25 17:50:12 2023, max compression
```

## Comparing `pyeasysql_ashenguard-3.2.0.tar` & `pyeasysql_ashenguard-3.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 19:30:01.347179 pyeasysql_ashenguard-3.2.0/
-drwxrwxrwx   0        0        0        0 2023-07-24 19:30:01.324039 pyeasysql_ashenguard-3.2.0/EasySQL/
--rw-rw-rw-   0        0        0     3662 2023-07-24 11:39:55.000000 pyeasysql_ashenguard-3.2.0/EasySQL/ABC.py
--rw-rw-rw-   0        0        0     2887 2021-06-27 12:24:21.000000 pyeasysql_ashenguard-3.2.0/EasySQL/Characters.py
--rw-rw-rw-   0        0        0    15027 2023-07-24 15:30:12.000000 pyeasysql_ashenguard-3.2.0/EasySQL/Classes.py
--rw-rw-rw-   0        0        0     6196 2023-07-24 15:30:13.000000 pyeasysql_ashenguard-3.2.0/EasySQL/Commands.py
--rw-rw-rw-   0        0        0      943 2023-07-24 15:30:12.000000 pyeasysql_ashenguard-3.2.0/EasySQL/Constraints.py
--rw-rw-rw-   0        0        0      305 2023-07-11 12:44:34.000000 pyeasysql_ashenguard-3.2.0/EasySQL/Decorators.py
--rw-rw-rw-   0        0        0     2097 2023-07-09 09:35:55.000000 pyeasysql_ashenguard-3.2.0/EasySQL/EasyInstances.py
--rw-rw-rw-   0        0        0      757 2023-06-08 19:41:42.000000 pyeasysql_ashenguard-3.2.0/EasySQL/Exceptions.py
--rw-rw-rw-   0        0        0      457 2021-04-04 16:17:30.000000 pyeasysql_ashenguard-3.2.0/EasySQL/Logging.py
--rw-rw-rw-   0        0        0     3079 2023-07-23 11:44:26.000000 pyeasysql_ashenguard-3.2.0/EasySQL/Types.py
--rw-rw-rw-   0        0        0     2496 2022-04-15 06:15:51.000000 pyeasysql_ashenguard-3.2.0/EasySQL/Where.py
--rw-rw-rw-   0        0        0      298 2023-07-24 15:21:11.000000 pyeasysql_ashenguard-3.2.0/EasySQL/__init__.py
--rw-rw-rw-   0        0        0     1085 2023-07-23 15:33:54.000000 pyeasysql_ashenguard-3.2.0/LICENSE.md
--rw-rw-rw-   0        0        0     6095 2023-07-24 19:30:01.346182 pyeasysql_ashenguard-3.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-24 19:30:01.338134 pyeasysql_ashenguard-3.2.0/PyEasySQL_Ashenguard.egg-info/
--rw-rw-rw-   0        0        0     6095 2023-07-24 19:30:01.000000 pyeasysql_ashenguard-3.2.0/PyEasySQL_Ashenguard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      723 2023-07-24 19:30:01.000000 pyeasysql_ashenguard-3.2.0/PyEasySQL_Ashenguard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 19:30:01.000000 pyeasysql_ashenguard-3.2.0/PyEasySQL_Ashenguard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-24 19:30:01.000000 pyeasysql_ashenguard-3.2.0/PyEasySQL_Ashenguard.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-24 19:30:01.000000 pyeasysql_ashenguard-3.2.0/PyEasySQL_Ashenguard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5412 2023-07-24 15:30:12.000000 pyeasysql_ashenguard-3.2.0/README.md
--rw-rw-rw-   0        0        0      728 2023-07-24 19:29:43.000000 pyeasysql_ashenguard-3.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-24 19:30:01.347179 pyeasysql_ashenguard-3.2.0/setup.cfg
--rw-rw-rw-   0        0        0      831 2023-07-24 16:25:04.000000 pyeasysql_ashenguard-3.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 17:50:12.205012 pyeasysql_ashenguard-3.2.1/
+drwxrwxrwx   0        0        0        0 2023-07-25 17:50:12.191011 pyeasysql_ashenguard-3.2.1/EasySQL/
+-rw-rw-rw-   0        0        0     3662 2023-07-24 11:39:55.000000 pyeasysql_ashenguard-3.2.1/EasySQL/ABC.py
+-rw-rw-rw-   0        0        0     2887 2021-06-27 12:24:21.000000 pyeasysql_ashenguard-3.2.1/EasySQL/Characters.py
+-rw-rw-rw-   0        0        0    15044 2023-07-25 08:56:23.000000 pyeasysql_ashenguard-3.2.1/EasySQL/Classes.py
+-rw-rw-rw-   0        0        0     6202 2023-07-25 17:49:13.000000 pyeasysql_ashenguard-3.2.1/EasySQL/Commands.py
+-rw-rw-rw-   0        0        0      945 2023-07-25 08:49:05.000000 pyeasysql_ashenguard-3.2.1/EasySQL/Constraints.py
+-rw-rw-rw-   0        0        0      305 2023-07-11 12:44:34.000000 pyeasysql_ashenguard-3.2.1/EasySQL/Decorators.py
+-rw-rw-rw-   0        0        0     2097 2023-07-09 09:35:55.000000 pyeasysql_ashenguard-3.2.1/EasySQL/EasyInstances.py
+-rw-rw-rw-   0        0        0      757 2023-06-08 19:41:42.000000 pyeasysql_ashenguard-3.2.1/EasySQL/Exceptions.py
+-rw-rw-rw-   0        0        0      457 2021-04-04 16:17:30.000000 pyeasysql_ashenguard-3.2.1/EasySQL/Logging.py
+-rw-rw-rw-   0        0        0     3079 2023-07-23 11:44:26.000000 pyeasysql_ashenguard-3.2.1/EasySQL/Types.py
+-rw-rw-rw-   0        0        0     2496 2022-04-15 06:15:51.000000 pyeasysql_ashenguard-3.2.1/EasySQL/Where.py
+-rw-rw-rw-   0        0        0      298 2023-07-24 15:21:11.000000 pyeasysql_ashenguard-3.2.1/EasySQL/__init__.py
+-rw-rw-rw-   0        0        0     1085 2023-07-23 15:33:54.000000 pyeasysql_ashenguard-3.2.1/LICENSE.md
+-rw-rw-rw-   0        0        0     6095 2023-07-25 17:50:12.203976 pyeasysql_ashenguard-3.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-25 17:50:12.200013 pyeasysql_ashenguard-3.2.1/PyEasySQL_Ashenguard.egg-info/
+-rw-rw-rw-   0        0        0     6095 2023-07-25 17:50:12.000000 pyeasysql_ashenguard-3.2.1/PyEasySQL_Ashenguard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      723 2023-07-25 17:50:12.000000 pyeasysql_ashenguard-3.2.1/PyEasySQL_Ashenguard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 17:50:12.000000 pyeasysql_ashenguard-3.2.1/PyEasySQL_Ashenguard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-25 17:50:12.000000 pyeasysql_ashenguard-3.2.1/PyEasySQL_Ashenguard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-25 17:50:12.000000 pyeasysql_ashenguard-3.2.1/PyEasySQL_Ashenguard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5412 2023-07-24 15:30:12.000000 pyeasysql_ashenguard-3.2.1/README.md
+-rw-rw-rw-   0        0        0      728 2023-07-25 08:49:05.000000 pyeasysql_ashenguard-3.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-25 17:50:12.205971 pyeasysql_ashenguard-3.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      831 2023-07-24 16:25:04.000000 pyeasysql_ashenguard-3.2.1/setup.py
```

### Comparing `pyeasysql_ashenguard-3.2.0/EasySQL/ABC.py` & `pyeasysql_ashenguard-3.2.1/EasySQL/ABC.py`

 * *Files identical despite different names*

### Comparing `pyeasysql_ashenguard-3.2.0/EasySQL/Characters.py` & `pyeasysql_ashenguard-3.2.1/EasySQL/Characters.py`

 * *Files identical despite different names*

### Comparing `pyeasysql_ashenguard-3.2.0/EasySQL/Classes.py` & `pyeasysql_ashenguard-3.2.1/EasySQL/Classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,15 +321,15 @@
                 c1 = set(self._columns)
                 c2 = set(columns)
 
                 if c1 != c2:
                     lc1 = [column.__repr__() for column in c1 - c2]
                     lc2 = [column.__repr__() for column in c2 - c1]
                     lc = zip_longest(lc1, lc2, "")
-                    length = len(max(lc1, key=lambda col: len(col)))
+                    length = len(max(['Provided: '] + lc1, key=lambda col: len(col)))
 
                     logger.warn(f'Columns specified do not match with existing ones:\n\tProvided:{" " * (length - 10)}\t\tExisting:\n\t' +
                                 '\n\t'.join([f'{lci[0]}{" " * (length - len(str(lci[0])))}\t\t{lci[1]}' for lci in lc]))
                     raise ValueError('Existing table does not match with specified columns.')
                 
         self.__prepared = True
```

### Comparing `pyeasysql_ashenguard-3.2.0/EasySQL/Commands.py` & `pyeasysql_ashenguard-3.2.1/EasySQL/Commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
             columns = table.columns
 
         table.assert_columns(columns)
         if len(columns) != len(values):
             raise ValueError('Values length do not match with the columns of the table')
 
         self._database = database
-        self._values = zip(table.columns, values)
+        self._values = list(zip(table.columns, values))
         self._columns = columns
         self._table = table
         self._update = on_dup_update
 
     def get_value(self) -> str:
         columns = ', '.join([column.name for column in self._columns])
         values = ', '.join([column.parse(value) for column, value in self._values])
```

### Comparing `pyeasysql_ashenguard-3.2.0/EasySQL/Constraints.py` & `pyeasysql_ashenguard-3.2.1/EasySQL/Constraints.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 class Unique(SQLConstraints):
     """
     Constraint representing unique
     """
 
-    def __init__(self, *columns: EasyColumn, name: str = None):
+    def __init__(self, *columns: 'EasyColumn', name: str = None):
         """
         Unique constractor
 
         :param columns: the column or columns for this constraint
         :param name: the name for this constraint
         """
         if name is None:
```

### Comparing `pyeasysql_ashenguard-3.2.0/EasySQL/EasyInstances.py` & `pyeasysql_ashenguard-3.2.1/EasySQL/EasyInstances.py`

 * *Files identical despite different names*

### Comparing `pyeasysql_ashenguard-3.2.0/EasySQL/Exceptions.py` & `pyeasysql_ashenguard-3.2.1/EasySQL/Exceptions.py`

 * *Files identical despite different names*

### Comparing `pyeasysql_ashenguard-3.2.0/EasySQL/Types.py` & `pyeasysql_ashenguard-3.2.1/EasySQL/Types.py`

 * *Files identical despite different names*

### Comparing `pyeasysql_ashenguard-3.2.0/EasySQL/Where.py` & `pyeasysql_ashenguard-3.2.1/EasySQL/Where.py`

 * *Files identical despite different names*

### Comparing `pyeasysql_ashenguard-3.2.0/LICENSE.md` & `pyeasysql_ashenguard-3.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyeasysql_ashenguard-3.2.0/PKG-INFO` & `pyeasysql_ashenguard-3.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyeasysql_ashenguard
-Version: 3.2.0
+Version: 3.2.1
 Summary: SQL Database management without even a SQL line
 Home-page: https://github.com/AGM-Studio/easysql
 Author: Ashenguard
 Author-email: Ashenguard <ashenguard@agmstudio.xyz>
 Project-URL: Homepage, https://github.com/agm-studio/easysql
 Project-URL: Bug Tracker, https://github.com/agm-studio/easysql/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyeasysql_ashenguard-3.2.0/PyEasySQL_Ashenguard.egg-info/PKG-INFO` & `pyeasysql_ashenguard-3.2.1/PyEasySQL_Ashenguard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyeasysql-ashenguard
-Version: 3.2.0
+Version: 3.2.1
 Summary: SQL Database management without even a SQL line
 Home-page: https://github.com/AGM-Studio/easysql
 Author: Ashenguard
 Author-email: Ashenguard <ashenguard@agmstudio.xyz>
 Project-URL: Homepage, https://github.com/agm-studio/easysql
 Project-URL: Bug Tracker, https://github.com/agm-studio/easysql/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyeasysql_ashenguard-3.2.0/PyEasySQL_Ashenguard.egg-info/SOURCES.txt` & `pyeasysql_ashenguard-3.2.1/PyEasySQL_Ashenguard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyeasysql_ashenguard-3.2.0/README.md` & `pyeasysql_ashenguard-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyeasysql_ashenguard-3.2.0/pyproject.toml` & `pyeasysql_ashenguard-3.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyeasysql_ashenguard"
-version = "3.2.0"
+version = "3.2.1"
 authors = [
   { name="Ashenguard", email="ashenguard@agmstudio.xyz" },
 ]
 description = "SQL Database management without even a SQL line"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `pyeasysql_ashenguard-3.2.0/setup.py` & `pyeasysql_ashenguard-3.2.1/setup.py`

 * *Files identical despite different names*

