# Comparing `tmp/idbadapter-1.9.5.tar.gz` & `tmp/idbadapter-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idbadapter-1.9.5.tar", last modified: Fri Jul 21 12:01:54 2023, max compression
+gzip compressed data, was "idbadapter-1.9.6.tar", last modified: Tue Jul 25 08:13:34 2023, max compression
```

## Comparing `idbadapter-1.9.5.tar` & `idbadapter-1.9.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 12:01:54.532580 idbadapter-1.9.5/
--rw-rw-rw-   0        0        0    11558 2023-05-15 08:54:26.000000 idbadapter-1.9.5/LICENSE
--rw-rw-rw-   0        0        0      697 2023-07-21 12:01:54.532580 idbadapter-1.9.5/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-05-15 08:54:26.000000 idbadapter-1.9.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 12:01:54.507974 idbadapter-1.9.5/idbadapter/
--rw-rw-rw-   0        0        0       61 2023-05-15 08:54:26.000000 idbadapter-1.9.5/idbadapter/__init__.py
--rw-rw-rw-   0        0        0    12395 2023-07-21 11:59:19.000000 idbadapter-1.9.5/idbadapter/schedule_loader.py
-drwxrwxrwx   0        0        0        0 2023-07-21 12:01:54.530603 idbadapter-1.9.5/idbadapter.egg-info/
--rw-rw-rw-   0        0        0      697 2023-07-21 12:01:54.000000 idbadapter-1.9.5/idbadapter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-07-21 12:01:54.000000 idbadapter-1.9.5/idbadapter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 12:01:54.000000 idbadapter-1.9.5/idbadapter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-21 12:01:54.000000 idbadapter-1.9.5/idbadapter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-21 12:01:54.000000 idbadapter-1.9.5/idbadapter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 12:01:54.534571 idbadapter-1.9.5/setup.cfg
--rw-rw-rw-   0        0        0      991 2023-07-21 12:01:39.000000 idbadapter-1.9.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:13:34.870033 idbadapter-1.9.6/
+-rw-rw-rw-   0        0        0    11558 2023-05-02 13:28:55.000000 idbadapter-1.9.6/LICENSE
+-rw-rw-rw-   0        0        0      697 2023-07-25 08:13:34.870033 idbadapter-1.9.6/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-05-05 13:33:15.000000 idbadapter-1.9.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 08:13:34.861035 idbadapter-1.9.6/idbadapter/
+-rw-rw-rw-   0        0        0       61 2023-05-22 08:18:39.000000 idbadapter-1.9.6/idbadapter/__init__.py
+-rw-rw-rw-   0        0        0    12480 2023-07-25 07:30:55.000000 idbadapter-1.9.6/idbadapter/schedule_loader.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:13:34.869036 idbadapter-1.9.6/idbadapter.egg-info/
+-rw-rw-rw-   0        0        0      697 2023-07-25 08:13:34.000000 idbadapter-1.9.6/idbadapter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-07-25 08:13:34.000000 idbadapter-1.9.6/idbadapter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 08:13:34.000000 idbadapter-1.9.6/idbadapter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-25 08:13:34.000000 idbadapter-1.9.6/idbadapter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-25 08:13:34.000000 idbadapter-1.9.6/idbadapter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 08:13:34.871033 idbadapter-1.9.6/setup.cfg
+-rw-rw-rw-   0        0        0      991 2023-07-25 08:13:32.000000 idbadapter-1.9.6/setup.py
```

### Comparing `idbadapter-1.9.5/LICENSE` & `idbadapter-1.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `idbadapter-1.9.5/PKG-INFO` & `idbadapter-1.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 1.9.5
+Version: 1.9.6
 Summary: Сache module for batch loading of data
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-1.9.5/idbadapter/schedule_loader.py` & `idbadapter-1.9.6/idbadapter/schedule_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,14 @@
 
 GRANULARY = {"column": "granulary_name", "table": "granulary_works", "id": "id_granulary_work", "res_table": "granulary_resources"}
 
 PROCESSED = {"column": "processed_name", "table": "processed_works", "id": "id_processed_work", "res_table": "processed_resources"}
 
 TYPEDLVL2 = {"column": "typed_lvl2_name", "table": "typed_lvl2_works", "id": "id_typed_lvl2_work", "res_table": "typed_lvl2_resources"}
 
-ALL = "all"
-
-
 class Schedules:
     """Get schedules from database service
     """
     def __init__(self, url):
         """Constructor
         Args:
             url (str): link to database service
@@ -161,19 +158,20 @@
     def get_all_resources_name(self):
         query = f"""
         select DISTINCT w.name as name, gw.name as granulary_name, tlw.name as lvl2_name, pn.name as processed_name from basic_resources w
         join resources_info wi on w.id = wi.id_resource  
         join granulary_resources gw on gw.id = wi.id_granulary_name
         join typed_lvl2_resources tlw on tlw.id = wi.id_typed_lvl2_name
         join processed_resources pn on pn.id = wi.id_processed_name"""
-
         df = self._execute_query(query)
         return df
 
-    def get_works_by_pulls(self, work_pulls: list, resource_list: list = [], key=GRANULARY, path_to_log="empty_pull.txt"):
+    def get_works_by_pulls(self, work_pulls: list, resource_list: list = [], key=GRANULARY, path_to_log="empty_pull.txt", res_key=None):
+        if res_key is None:
+            res_key = key
         self.path_to_log = path_to_log
         for pull in work_pulls:
             query = f"""with date_cte (date, object_id)
                 as (
                     (select date, object_id from works_names_mv wnm
                     where wnm.{key["column"]} in ({','.join(map(lambda x: f"'{x}'", pull))})
                     group by object_id, date 
@@ -192,18 +190,19 @@
                 select false as is_work, * from resource_names_mv rnm
                 join date_cte on date_cte.object_id = rnm.object_id
                 and rnm.date >= date_cte.date
                 where rnm.object_id = date_cte.object_id"""
 
                 
             if len(resource_list) != 0:
-                query += f""" and rnm.{key["column"]} in ({",".join(map(lambda x: f"'{x}'", resource_list))})"""   
+                query += f""" and rnm.{res_key["column"]} in ({",".join(map(lambda x: f"'{x}'", resource_list))})"""   
             try:
                 df = self._execute_query(query)
             except ValueError:
+                print(query)
                 print("jsondecodeerror occurred", pull)
                 yield None
                 continue 
 
             if df.empty:
                 with open(self.path_to_log, "a", encoding="UTF-8") as f:
                     print("pull not found", pull, file=f)
```

### Comparing `idbadapter-1.9.5/idbadapter.egg-info/PKG-INFO` & `idbadapter-1.9.6/idbadapter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 1.9.5
+Version: 1.9.6
 Summary: Сache module for batch loading of data
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-1.9.5/setup.py` & `idbadapter-1.9.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 
 from distutils.core import setup
 
-version = '1.9.5'
+version = '1.9.6'
 
 long_description = "Сache module for batch loading of data"
 
 setup(name='idbadapter',
-      version='1.9.5',
+      version='1.9.6',
       description='Сache module for batch loading of data',
       long_description=long_description,
       url="https://github.com/AnatolyPershinov/gpn_cache_module",
       download_url='https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip',
       author='Anatoly Pershinov',
       author_email='anatoliypershinov@gmail.com',
       packages=['idbadapter'],
```

