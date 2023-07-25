# Comparing `tmp/tableau_utilities-2.0.61.tar.gz` & `tmp/tableau_utilities-2.0.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableau_utilities-2.0.61.tar", last modified: Tue Jul 18 17:06:09 2023, max compression
+gzip compressed data, was "tableau_utilities-2.0.62.tar", last modified: Tue Jul 25 18:34:00 2023, max compression
```

## Comparing `tableau_utilities-2.0.61.tar` & `tableau_utilities-2.0.62.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-18 17:06:09.259945 tableau_utilities-2.0.61/
--rw-r--r--   0 justin     (502) staff       (20)     1062 2022-05-25 18:48:01.000000 tableau_utilities-2.0.61/LICENSE
--rw-r--r--   0 justin     (502) staff       (20)     8421 2023-07-18 17:06:09.259602 tableau_utilities-2.0.61/PKG-INFO
--rw-r--r--   0 justin     (502) staff       (20)     8116 2023-06-28 16:57:49.000000 tableau_utilities-2.0.61/README.md
--rw-r--r--   0 justin     (502) staff       (20)       38 2023-07-18 17:06:09.260085 tableau_utilities-2.0.61/setup.cfg
--rw-r--r--   0 justin     (502) staff       (20)     1108 2023-07-18 17:03:41.000000 tableau_utilities-2.0.61/setup.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-18 17:06:09.242191 tableau_utilities-2.0.61/tableau_utilities/
--rw-r--r--   0 justin     (502) staff       (20)      272 2023-06-28 16:57:49.000000 tableau_utilities-2.0.61/tableau_utilities/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)     2441 2023-06-28 16:57:49.000000 tableau_utilities-2.0.61/tableau_utilities/fetch_all_cols.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-18 17:06:09.247900 tableau_utilities-2.0.61/tableau_utilities/general/
--rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.61/tableau_utilities/general/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)     2235 2023-06-28 16:57:49.000000 tableau_utilities-2.0.61/tableau_utilities/general/cli_styling.py
--rw-r--r--   0 justin     (502) staff       (20)     3497 2023-06-28 16:57:49.000000 tableau_utilities-2.0.61/tableau_utilities/general/config_column_persona.py
--rw-r--r--   0 justin     (502) staff       (20)     2278 2023-06-28 16:57:49.000000 tableau_utilities-2.0.61/tableau_utilities/general/funcs.py
--rw-r--r--   0 justin     (502) staff       (20)     2874 2023-06-28 16:57:49.000000 tableau_utilities-2.0.61/tableau_utilities/scripted_testing.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-18 17:06:09.253367 tableau_utilities-2.0.61/tableau_utilities/scripts/
--rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.61/tableau_utilities/scripts/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)    23247 2023-06-28 16:57:49.000000 tableau_utilities-2.0.61/tableau_utilities/scripts/cli.py
--rw-r--r--   0 justin     (502) staff       (20)     1772 2023-06-28 16:57:49.000000 tableau_utilities-2.0.61/tableau_utilities/scripts/csv_config.py
--rw-r--r--   0 justin     (502) staff       (20)     7901 2023-07-18 16:25:27.000000 tableau_utilities-2.0.61/tableau_utilities/scripts/datasource.py
--rw-r--r--   0 justin     (502) staff       (20)    13151 2023-06-28 16:57:49.000000 tableau_utilities-2.0.61/tableau_utilities/scripts/gen_config.py
--rw-r--r--   0 justin     (502) staff       (20)     8539 2023-06-28 16:57:49.000000 tableau_utilities-2.0.61/tableau_utilities/scripts/merge_config.py
--rw-r--r--   0 justin     (502) staff       (20)     1867 2023-06-28 16:57:49.000000 tableau_utilities-2.0.61/tableau_utilities/scripts/server_info.py
--rw-r--r--   0 justin     (502) staff       (20)     4531 2023-06-28 16:57:49.000000 tableau_utilities-2.0.61/tableau_utilities/scripts/server_operate.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-18 17:06:09.255288 tableau_utilities-2.0.61/tableau_utilities/tableau_file/
--rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.61/tableau_utilities/tableau_file/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)    12316 2023-07-18 17:03:41.000000 tableau_utilities-2.0.61/tableau_utilities/tableau_file/tableau_file.py
--rw-r--r--   0 justin     (502) staff       (20)    37816 2023-07-10 18:51:08.000000 tableau_utilities-2.0.61/tableau_utilities/tableau_file/tableau_file_objects.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-18 17:06:09.258436 tableau_utilities-2.0.61/tableau_utilities/tableau_server/
--rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.61/tableau_utilities/tableau_server/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)    31778 2023-06-28 16:57:49.000000 tableau_utilities-2.0.61/tableau_utilities/tableau_server/tableau_server.py
--rw-r--r--   0 justin     (502) staff       (20)    13195 2023-06-28 16:57:49.000000 tableau_utilities-2.0.61/tableau_utilities/tableau_server/tableau_server_objects.py
--rw-r--r--   0 justin     (502) staff       (20)    10765 2023-07-10 18:39:33.000000 tableau_utilities-2.0.61/tableau_utilities/test_tableau_utilities.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-18 17:06:09.245497 tableau_utilities-2.0.61/tableau_utilities.egg-info/
--rw-r--r--   0 justin     (502) staff       (20)     8421 2023-07-18 17:06:09.000000 tableau_utilities-2.0.61/tableau_utilities.egg-info/PKG-INFO
--rw-r--r--   0 justin     (502) staff       (20)     1205 2023-07-18 17:06:09.000000 tableau_utilities-2.0.61/tableau_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 justin     (502) staff       (20)        1 2023-07-18 17:06:09.000000 tableau_utilities-2.0.61/tableau_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 justin     (502) staff       (20)       73 2023-07-18 17:06:09.000000 tableau_utilities-2.0.61/tableau_utilities.egg-info/entry_points.txt
--rw-r--r--   0 justin     (502) staff       (20)      112 2023-07-18 17:06:09.000000 tableau_utilities-2.0.61/tableau_utilities.egg-info/requires.txt
--rw-r--r--   0 justin     (502) staff       (20)       18 2023-07-18 17:06:09.000000 tableau_utilities-2.0.61/tableau_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-25 18:34:00.835278 tableau_utilities-2.0.62/
+-rw-r--r--   0 justin     (502) staff       (20)     1062 2022-05-25 18:48:01.000000 tableau_utilities-2.0.62/LICENSE
+-rw-r--r--   0 justin     (502) staff       (20)     8421 2023-07-25 18:34:00.834964 tableau_utilities-2.0.62/PKG-INFO
+-rw-r--r--   0 justin     (502) staff       (20)     8116 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/README.md
+-rw-r--r--   0 justin     (502) staff       (20)       38 2023-07-25 18:34:00.835397 tableau_utilities-2.0.62/setup.cfg
+-rw-r--r--   0 justin     (502) staff       (20)     1108 2023-07-25 18:33:34.000000 tableau_utilities-2.0.62/setup.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-25 18:34:00.814806 tableau_utilities-2.0.62/tableau_utilities/
+-rw-r--r--   0 justin     (502) staff       (20)      272 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)     2441 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/fetch_all_cols.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-25 18:34:00.822366 tableau_utilities-2.0.62/tableau_utilities/general/
+-rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/general/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)     2235 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/general/cli_styling.py
+-rw-r--r--   0 justin     (502) staff       (20)     3497 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/general/config_column_persona.py
+-rw-r--r--   0 justin     (502) staff       (20)     2278 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/general/funcs.py
+-rw-r--r--   0 justin     (502) staff       (20)     2874 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/scripted_testing.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-25 18:34:00.829404 tableau_utilities-2.0.62/tableau_utilities/scripts/
+-rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/scripts/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)    23247 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/scripts/cli.py
+-rw-r--r--   0 justin     (502) staff       (20)     1772 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/scripts/csv_config.py
+-rw-r--r--   0 justin     (502) staff       (20)     7863 2023-07-25 18:33:34.000000 tableau_utilities-2.0.62/tableau_utilities/scripts/datasource.py
+-rw-r--r--   0 justin     (502) staff       (20)    13151 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/scripts/gen_config.py
+-rw-r--r--   0 justin     (502) staff       (20)     8539 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/scripts/merge_config.py
+-rw-r--r--   0 justin     (502) staff       (20)     1867 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/scripts/server_info.py
+-rw-r--r--   0 justin     (502) staff       (20)     4531 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/scripts/server_operate.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-25 18:34:00.831492 tableau_utilities-2.0.62/tableau_utilities/tableau_file/
+-rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/tableau_file/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)    12316 2023-07-18 22:10:49.000000 tableau_utilities-2.0.62/tableau_utilities/tableau_file/tableau_file.py
+-rw-r--r--   0 justin     (502) staff       (20)    37752 2023-07-25 18:33:34.000000 tableau_utilities-2.0.62/tableau_utilities/tableau_file/tableau_file_objects.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-25 18:34:00.834051 tableau_utilities-2.0.62/tableau_utilities/tableau_server/
+-rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/tableau_server/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)    31778 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/tableau_server/tableau_server.py
+-rw-r--r--   0 justin     (502) staff       (20)    13195 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/tableau_server/tableau_server_objects.py
+-rw-r--r--   0 justin     (502) staff       (20)    10765 2023-07-10 18:39:33.000000 tableau_utilities-2.0.62/tableau_utilities/test_tableau_utilities.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-25 18:34:00.818767 tableau_utilities-2.0.62/tableau_utilities.egg-info/
+-rw-r--r--   0 justin     (502) staff       (20)     8421 2023-07-25 18:34:00.000000 tableau_utilities-2.0.62/tableau_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 justin     (502) staff       (20)     1205 2023-07-25 18:34:00.000000 tableau_utilities-2.0.62/tableau_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 justin     (502) staff       (20)        1 2023-07-25 18:34:00.000000 tableau_utilities-2.0.62/tableau_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 justin     (502) staff       (20)       73 2023-07-25 18:34:00.000000 tableau_utilities-2.0.62/tableau_utilities.egg-info/entry_points.txt
+-rw-r--r--   0 justin     (502) staff       (20)      112 2023-07-25 18:34:00.000000 tableau_utilities-2.0.62/tableau_utilities.egg-info/requires.txt
+-rw-r--r--   0 justin     (502) staff       (20)       18 2023-07-25 18:34:00.000000 tableau_utilities-2.0.62/tableau_utilities.egg-info/top_level.txt
```

### Comparing `tableau_utilities-2.0.61/LICENSE` & `tableau_utilities-2.0.62/LICENSE`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.61/PKG-INFO` & `tableau_utilities-2.0.62/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableau_utilities
-Version: 2.0.61
+Version: 2.0.62
 Summary: Utility for maintaining Tableau objects
 Home-page: http://pypi.python.org/pypi/tableau-utilities/
 Author: Justin Grilli
 Author-email: justin.grilli@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tableau_utilities-2.0.61/README.md` & `tableau_utilities-2.0.62/README.md`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.61/setup.py` & `tableau_utilities-2.0.62/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     author_email="justin.grilli@gmail.com",
     license='MIT',
     url='http://pypi.python.org/pypi/tableau-utilities/',
     description='Utility for maintaining Tableau objects',
     long_description=readme,
     long_description_content_type='text/markdown',
     name="tableau_utilities",
-    version="2.0.61",
+    version="2.0.62",
     packages=[
         'tableau_utilities',
         'tableau_utilities.general',
         'tableau_utilities.tableau_file',
         'tableau_utilities.tableau_server',
         'tableau_utilities.scripts'
     ],
```

### Comparing `tableau_utilities-2.0.61/tableau_utilities/fetch_all_cols.py` & `tableau_utilities-2.0.62/tableau_utilities/fetch_all_cols.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.61/tableau_utilities/general/cli_styling.py` & `tableau_utilities-2.0.62/tableau_utilities/general/cli_styling.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.61/tableau_utilities/general/config_column_persona.py` & `tableau_utilities-2.0.62/tableau_utilities/general/config_column_persona.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.61/tableau_utilities/general/funcs.py` & `tableau_utilities-2.0.62/tableau_utilities/general/funcs.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.61/tableau_utilities/scripted_testing.py` & `tableau_utilities-2.0.62/tableau_utilities/scripted_testing.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.61/tableau_utilities/scripts/cli.py` & `tableau_utilities-2.0.62/tableau_utilities/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.61/tableau_utilities/scripts/csv_config.py` & `tableau_utilities-2.0.62/tableau_utilities/scripts/csv_config.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.61/tableau_utilities/scripts/datasource.py` & `tableau_utilities-2.0.62/tableau_utilities/scripts/datasource.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,22 +101,22 @@
             print(f'  {symbol.arrow_r} {c.connection.dict()}')
 
     # Add / modify a specified column
     if column_name and not delete:
         # Column name needs to be enclosed in brackets
         if debugging_logs:
             print('Going to add/update column:', column_name)
-        column_name = f'[{column_name}]'
         column = ds.columns.get(column_name)
-        persona = dict()
-        if args.persona:
-            persona = personas.get(args.persona.lower(), {})
+        if persona:
+            persona = personas.get(persona.lower(), {})
+        else:
+            persona = dict()
 
         if not column:
-            if not args.persona:
+            if not persona:
                 raise Exception('Column does not exist, and more args are need to add a new column.\n'
                                 f'Minimum required args: {color.fg_yellow}--column_name --persona{color.reset}')
             column = tfo.Column(
                 name=column_name,
                 role=persona['role'],
                 datatype=persona['datatype'],
                 type=persona['role_type'],
```

### Comparing `tableau_utilities-2.0.61/tableau_utilities/scripts/gen_config.py` & `tableau_utilities-2.0.62/tableau_utilities/scripts/gen_config.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.61/tableau_utilities/scripts/merge_config.py` & `tableau_utilities-2.0.62/tableau_utilities/scripts/merge_config.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.61/tableau_utilities/scripts/server_info.py` & `tableau_utilities-2.0.62/tableau_utilities/scripts/server_info.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.61/tableau_utilities/scripts/server_operate.py` & `tableau_utilities-2.0.62/tableau_utilities/scripts/server_operate.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.61/tableau_utilities/tableau_file/tableau_file.py` & `tableau_utilities-2.0.62/tableau_utilities/tableau_file/tableau_file.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.61/tableau_utilities/tableau_file/tableau_file_objects.py` & `tableau_utilities-2.0.62/tableau_utilities/tableau_file/tableau_file_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,24 +273,24 @@
 
     def __hash__(self):
         return hash(str(astuple(self)))
 
     def __eq__(self, other):
         name = ''
         if isinstance(other, str):
-            name = other.lower()
+            name = other
         elif isinstance(other, dict):
-            name = other.get('name').lower()
+            name = other.get('name')
         elif isinstance(other, (Column, object)):
-            name = other.name.lower()
+            name = other.name
 
         if not re.match(r'^\[.+]$', name):
             name = f'[{name}]'
 
-        return self.name.lower() == name
+        return self.name == name
 
     def dict(self):
         output = {
             '@name': self.name,
             '@datatype': self.datatype,
             '@role': self.role,
             '@type': self.type
@@ -409,24 +409,24 @@
 
     def __hash__(self):
         return hash(str(astuple(self)))
 
     def __eq__(self, other):
         key = ''
         if isinstance(other, str):
-            key = other.lower()
+            key = other
         elif isinstance(other, dict):
-            key = other.get('key').lower()
+            key = other.get('key')
         elif isinstance(other, (MappingCol, object)):
-            key = other.key.lower()
+            key = other.key
 
         if not re.match(r'^\[.+]$', key):
             key = f'[{key}]'
 
-        return self.key.lower() == key
+        return self.key == key
 
     def dict(self):
         return {'@key': self.key, '@value': self.value}
 
 
 @dataclass
 class FolderItem(TableauFileObject):
```

### Comparing `tableau_utilities-2.0.61/tableau_utilities/tableau_server/tableau_server.py` & `tableau_utilities-2.0.62/tableau_utilities/tableau_server/tableau_server.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.61/tableau_utilities/tableau_server/tableau_server_objects.py` & `tableau_utilities-2.0.62/tableau_utilities/tableau_server/tableau_server_objects.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.61/tableau_utilities/test_tableau_utilities.py` & `tableau_utilities-2.0.62/tableau_utilities/test_tableau_utilities.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.61/tableau_utilities.egg-info/PKG-INFO` & `tableau_utilities-2.0.62/tableau_utilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableau-utilities
-Version: 2.0.61
+Version: 2.0.62
 Summary: Utility for maintaining Tableau objects
 Home-page: http://pypi.python.org/pypi/tableau-utilities/
 Author: Justin Grilli
 Author-email: justin.grilli@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tableau_utilities-2.0.61/tableau_utilities.egg-info/SOURCES.txt` & `tableau_utilities-2.0.62/tableau_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

