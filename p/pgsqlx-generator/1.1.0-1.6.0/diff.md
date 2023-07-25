# Comparing `tmp/pgsqlx-generator-1.1.0.tar.gz` & `tmp/pgsqlx-generator-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pgsqlx-generator-1.1.0.tar", last modified: Mon Jul 24 14:00:37 2023, max compression
+gzip compressed data, was "dist\pgsqlx-generator-1.6.0.tar", last modified: Tue Jul 25 08:29:19 2023, max compression
```

## Comparing `pgsqlx-generator-1.1.0.tar` & `pgsqlx-generator-1.6.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 14:00:37.000000 pgsqlx-generator-1.1.0/
-drwxrwxrwx   0        0        0        0 2023-07-24 14:00:37.000000 pgsqlx-generator-1.1.0/pgsqlx/
--rw-rw-rw-   0        0        0     6667 2023-07-24 07:11:00.000000 pgsqlx-generator-1.1.0/pgsqlx/generator.py
--rw-rw-rw-   0        0        0     1905 2023-07-24 06:46:00.000000 pgsqlx-generator-1.1.0/pgsqlx/generator.tpl
--rw-rw-rw-   0        0        0      125 2023-07-24 13:38:47.000000 pgsqlx-generator-1.1.0/pgsqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 14:00:37.000000 pgsqlx-generator-1.1.0/pgsqlx_generator.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-24 14:00:37.000000 pgsqlx-generator-1.1.0/pgsqlx_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-24 14:00:37.000000 pgsqlx-generator-1.1.0/pgsqlx_generator.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2868 2023-07-24 14:00:37.000000 pgsqlx-generator-1.1.0/pgsqlx_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       18 2023-07-24 14:00:37.000000 pgsqlx-generator-1.1.0/pgsqlx_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0      317 2023-07-24 14:00:37.000000 pgsqlx-generator-1.1.0/pgsqlx_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-24 14:00:37.000000 pgsqlx-generator-1.1.0/pgsqlx_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2868 2023-07-24 14:00:37.000000 pgsqlx-generator-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2395 2023-07-24 07:34:39.000000 pgsqlx-generator-1.1.0/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-24 14:00:37.000000 pgsqlx-generator-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1122 2023-07-24 13:59:43.000000 pgsqlx-generator-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:29:19.000000 pgsqlx-generator-1.6.0/
+drwxrwxrwx   0        0        0        0 2023-07-25 08:29:19.000000 pgsqlx-generator-1.6.0/pgsqlx/
+-rw-rw-rw-   0        0        0     6673 2023-07-25 08:10:07.000000 pgsqlx-generator-1.6.0/pgsqlx/generator.py
+-rw-rw-rw-   0        0        0     1905 2023-07-24 06:46:00.000000 pgsqlx-generator-1.6.0/pgsqlx/generator.tpl
+-rw-rw-rw-   0        0        0      629 2023-07-25 06:13:56.000000 pgsqlx-generator-1.6.0/pgsqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:29:19.000000 pgsqlx-generator-1.6.0/pgsqlx_generator.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-25 08:29:19.000000 pgsqlx-generator-1.6.0/pgsqlx_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-25 08:29:19.000000 pgsqlx-generator-1.6.0/pgsqlx_generator.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2868 2023-07-25 08:29:19.000000 pgsqlx-generator-1.6.0/pgsqlx_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2023-07-25 08:29:19.000000 pgsqlx-generator-1.6.0/pgsqlx_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      317 2023-07-25 08:29:19.000000 pgsqlx-generator-1.6.0/pgsqlx_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-25 08:29:19.000000 pgsqlx-generator-1.6.0/pgsqlx_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2868 2023-07-25 08:29:19.000000 pgsqlx-generator-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2395 2023-07-24 07:34:39.000000 pgsqlx-generator-1.6.0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-25 08:29:19.000000 pgsqlx-generator-1.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1122 2023-07-25 08:28:28.000000 pgsqlx-generator-1.6.0/setup.py
```

### Comparing `pgsqlx-generator-1.1.0/pgsqlx/generator.py` & `pgsqlx-generator-1.6.0/pgsqlx/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
-from sqlbatis import db, Engin
 from typing import Union, Iterable
+from sqlbatis import db, Engin, init_db
 from jinja2 import FileSystemLoader, Environment
 from sqlbatis.constant import KEY, KEY_SEQ, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, KEY_STRATEGY
 
 COMMON_COLS = ['create_by', 'create_time']
 ATTRIBUTES = {KEY: 'id', UPDATE_BY: 'update_by', UPDATE_TIME: 'update_time', DEL_FLAG: 'del_flag'}
 
 
@@ -15,15 +15,15 @@
              FROM information_schema.columns WHERE table_schema='public' AND table_name = ?'''
     key_sql = '''SELECT a.attname FROM pg_index i
                  JOIN pg_attribute a ON a.attrelid = i.indrelid AND a.attnum = any(i.indkey)
                  WHERE i.indrelid = ?::regclass AND i.indisprimary LIMIT 1'''
 
     def __init__(self, user='root', password='', database='test', host='127.0.0.1', port=3306, pool_size=0, show_sql=False, use_unicode=True,
             **kwargs):
-        db.init_db(user=user, password=password, database=database, host=host, port=port, engin=Engin.POSTGRESQL, pool_size=pool_size, show_sql=show_sql, \
+        init_db(user=user, password=password, database=database, host=host, port=port, engin=Engin.POSTGRESQL, pool_size=pool_size, show_sql=show_sql, \
                    use_unicode=use_unicode, **kwargs)
 
     def generate_with_schema(self, schema: str = None, path: str = None, *args, **kwargs):
         if schema:
             db.execute('use %s' % schema)
         tables = db.select('show tables')
         tables = [table[0] for table in tables]
```

### Comparing `pgsqlx-generator-1.1.0/pgsqlx/generator.tpl` & `pgsqlx-generator-1.6.0/pgsqlx/generator.tpl`

 * *Files identical despite different names*

### Comparing `pgsqlx-generator-1.1.0/pgsqlx_generator.egg-info/PKG-INFO` & `pgsqlx-generator-1.6.0/pgsqlx_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx-generator
-Version: 1.1.0
+Version: 1.6.0
 Summary: pgsqlx-generator is a model code generator from tables for PgSqlx.
 Home-page: https://gitee.com/summry/pgsqlx/blob/master/generator.md
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: PostgreSQL,PgSqlx,python
 Platform: UNKNOWN
```

### Comparing `pgsqlx-generator-1.1.0/PKG-INFO` & `pgsqlx-generator-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx-generator
-Version: 1.1.0
+Version: 1.6.0
 Summary: pgsqlx-generator is a model code generator from tables for PgSqlx.
 Home-page: https://gitee.com/summry/pgsqlx/blob/master/generator.md
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: PostgreSQL,PgSqlx,python
 Platform: UNKNOWN
```

### Comparing `pgsqlx-generator-1.1.0/README.rst` & `pgsqlx-generator-1.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `pgsqlx-generator-1.1.0/setup.py` & `pgsqlx-generator-1.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 setup(
     name='pgsqlx-generator',
     packages=['pgsqlx'],
     description="pgsqlx-generator is a model code generator from tables for PgSqlx.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
-        'sqlx-batis>=0.0.7',
+        'sqlx-batis>=0.0.8',
     ],
-    version='1.1.0',
+    version='1.6.0',
     url='https://gitee.com/summry/pgsqlx/blob/master/generator.md',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['PostgreSQL', 'PgSqlx', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

