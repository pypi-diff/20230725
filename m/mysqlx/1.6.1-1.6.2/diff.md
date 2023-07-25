# Comparing `tmp/mysqlx-1.6.1.tar.gz` & `tmp/mysqlx-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-1.6.1.tar", last modified: Mon Jul 24 07:28:15 2023, max compression
+gzip compressed data, was "dist\mysqlx-1.6.2.tar", last modified: Tue Jul 25 08:29:33 2023, max compression
```

## Comparing `mysqlx-1.6.1.tar` & `mysqlx-1.6.2.tar`

### file list

```diff
@@ -1,20 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 07:28:15.000000 mysqlx-1.6.1/
-drwxrwxrwx   0        0        0        0 2023-07-24 07:28:15.000000 mysqlx-1.6.1/mysqlx/
--rw-rw-rw-   0        0        0     1083 2023-07-24 01:21:11.000000 mysqlx-1.6.1/mysqlx/db.py
--rw-rw-rw-   0        0        0      668 2023-07-24 01:21:11.000000 mysqlx-1.6.1/mysqlx/dbx.py
--rw-rw-rw-   0        0        0      344 2023-07-24 01:32:22.000000 mysqlx-1.6.1/mysqlx/log_support.py
--rw-rw-rw-   0        0        0     1783 2023-07-24 01:16:32.000000 mysqlx-1.6.1/mysqlx/orm.py
--rw-rw-rw-   0        0        0      115 2023-07-24 02:33:37.000000 mysqlx-1.6.1/mysqlx/snowflake.py
--rw-rw-rw-   0        0        0      103 2023-07-24 00:31:03.000000 mysqlx-1.6.1/mysqlx/sql_mapper.py
--rw-rw-rw-   0        0        0      125 2023-07-24 01:06:19.000000 mysqlx-1.6.1/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 07:28:15.000000 mysqlx-1.6.1/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-24 07:28:15.000000 mysqlx-1.6.1/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-24 07:28:15.000000 mysqlx-1.6.1/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4539 2023-07-24 07:28:15.000000 mysqlx-1.6.1/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       32 2023-07-24 07:28:15.000000 mysqlx-1.6.1/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      320 2023-07-24 07:28:15.000000 mysqlx-1.6.1/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-24 07:28:15.000000 mysqlx-1.6.1/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4539 2023-07-24 07:28:15.000000 mysqlx-1.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     4033 2023-07-24 07:27:52.000000 mysqlx-1.6.1/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-24 07:28:15.000000 mysqlx-1.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1241 2023-07-24 07:28:05.000000 mysqlx-1.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:29:33.000000 mysqlx-1.6.2/
+drwxrwxrwx   0        0        0        0 2023-07-25 08:29:33.000000 mysqlx-1.6.2/mysqlx/
+-rw-rw-rw-   0        0        0      687 2023-07-25 07:29:18.000000 mysqlx-1.6.2/mysqlx/db.py
+-rw-rw-rw-   0        0        0      344 2023-07-24 01:32:22.000000 mysqlx-1.6.2/mysqlx/log_support.py
+-rw-rw-rw-   0        0        0     6065 2023-07-25 08:13:53.000000 mysqlx-1.6.2/mysqlx/orm.py
+-rw-rw-rw-   0        0        0      626 2023-07-25 06:08:48.000000 mysqlx-1.6.2/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:29:33.000000 mysqlx-1.6.2/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-25 08:29:33.000000 mysqlx-1.6.2/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-25 08:29:33.000000 mysqlx-1.6.2/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4511 2023-07-25 08:29:33.000000 mysqlx-1.6.2/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2023-07-25 08:29:33.000000 mysqlx-1.6.2/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      265 2023-07-25 08:29:33.000000 mysqlx-1.6.2/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-25 08:29:33.000000 mysqlx-1.6.2/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4511 2023-07-25 08:29:33.000000 mysqlx-1.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4007 2023-07-25 08:23:23.000000 mysqlx-1.6.2/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-25 08:29:33.000000 mysqlx-1.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     1242 2023-07-25 08:29:07.000000 mysqlx-1.6.2/setup.py
```

### Comparing `mysqlx-1.6.1/mysqlx/db.py` & `mysqlx-1.6.2/mysqlx/db.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,19 @@
 from .log_support import save_log
-from sqlbatis import Engin, DBEngin
+from sqlexec.engin import MySqlEngin
 
 # Don't remove. Import for not repetitive implementation
-from sqlbatis.db import init_db as supper_init_db, insert, save as save_select_key, execute, batch_insert, batch_execute, get, query, query_one, \
-    query_page, select, select_one, select_page, do_execute, do_get, do_query, do_query_one, do_query_page, do_select, do_select_one, do_select_page
-
-_DB_CTX = None
-
-
-def init_db(user='root', password='', database='test', host='127.0.0.1', port=3306, pool_size=0, show_sql=False, use_unicode=True, **kwargs):
-    supper_init_db(user=user, password=password, database=database, host=host, port=port, engin=Engin.MYSQL, pool_size=pool_size, show_sql=show_sql, \
-                   use_unicode=use_unicode, **kwargs)
+from sqlbatis.db import insert, save as save_select_key, execute, batch_insert, batch_execute, get, query, query_one, query_page, select, select_one,\
+    select_page, do_execute, do_get, do_query, do_query_one, do_query_page, do_select, do_select_one, do_select_page
 
 
 def save(table: str, **kwargs):
     """
     Insert data into table, return primary key.
     :param table: table
     :param kwargs:
     :return: Primary key
     """
     save_log(table, **kwargs)
-    return save_select_key(DBEngin.get_select_key(), table, **kwargs)
+    return save_select_key(MySqlEngin.get_select_key(), table, **kwargs)
```

### Comparing `mysqlx-1.6.1/mysqlx.egg-info/PKG-INFO` & `mysqlx-1.6.2/mysqlx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.6.1
+Version: 1.6.2
 Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
-Author: summry
+Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 
@@ -39,18 +39,17 @@
    </mapper>
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
-   from mysqlx import db, dbx
    from mysqlx.orm import Model
-   from mysqlx.sql_mapper import mapper, sql
    from typing import List, Tuple, Mapping
+   from mysqlx import mapper, sql, db, dbx, init_db
 
    @mapper(namespace='user')
    def select_all(): List
 
    @mapper(namespace='user')
    def select_by_name(name: str): List
 
@@ -58,15 +57,15 @@
    def query_all(): List(Mapping)
 
    @sql('select id, name, age from user where name=?')
    def query_by_name(name: str): List(Mapping)
 
 
    if __name__ == '__main__':
-       db.init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', pool_size=5, show_sql=True, mapper_path='./mapper')
+       init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', pool_size=5, show_sql=True, mapper_path='./mapper')
        
        users = select_all()
        # result:
        # (3, 'zhangsan', 15)
        # (4, 'lisi', 26)
        # (5, 'wangwu', 38)
```

### Comparing `mysqlx-1.6.1/PKG-INFO` & `mysqlx-1.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.6.1
+Version: 1.6.2
 Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
-Author: summry
+Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 
@@ -39,18 +39,17 @@
    </mapper>
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
-   from mysqlx import db, dbx
    from mysqlx.orm import Model
-   from mysqlx.sql_mapper import mapper, sql
    from typing import List, Tuple, Mapping
+   from mysqlx import mapper, sql, db, dbx, init_db
 
    @mapper(namespace='user')
    def select_all(): List
 
    @mapper(namespace='user')
    def select_by_name(name: str): List
 
@@ -58,15 +57,15 @@
    def query_all(): List(Mapping)
 
    @sql('select id, name, age from user where name=?')
    def query_by_name(name: str): List(Mapping)
 
 
    if __name__ == '__main__':
-       db.init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', pool_size=5, show_sql=True, mapper_path='./mapper')
+       init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', pool_size=5, show_sql=True, mapper_path='./mapper')
        
        users = select_all()
        # result:
        # (3, 'zhangsan', 15)
        # (4, 'lisi', 26)
        # (5, 'wangwu', 38)
```

### Comparing `mysqlx-1.6.1/README.rst` & `mysqlx-1.6.2/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -26,18 +26,17 @@
    </mapper>
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
-   from mysqlx import db, dbx
    from mysqlx.orm import Model
-   from mysqlx.sql_mapper import mapper, sql
    from typing import List, Tuple, Mapping
+   from mysqlx import mapper, sql, db, dbx, init_db
 
    @mapper(namespace='user')
    def select_all(): List
 
    @mapper(namespace='user')
    def select_by_name(name: str): List
 
@@ -45,15 +44,15 @@
    def query_all(): List(Mapping)
 
    @sql('select id, name, age from user where name=?')
    def query_by_name(name: str): List(Mapping)
 
 
    if __name__ == '__main__':
-       db.init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', pool_size=5, show_sql=True, mapper_path='./mapper')
+       init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', pool_size=5, show_sql=True, mapper_path='./mapper')
        
        users = select_all()
        # result:
        # (3, 'zhangsan', 15)
        # (4, 'lisi', 26)
        # (5, 'wangwu', 38)
```

### Comparing `mysqlx-1.6.1/setup.py` & `mysqlx-1.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 setup(
     name='mysqlx',
     packages=['mysqlx'],
     description="MySqlx is a simple python sql executor for MySQL like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
-        'Jinja2>=2.7.0',
-        'sqlx-batis>=0.0.7',
+        # 'Jinja2>=2.7.0',
+        'sqlx-batis>=0.0.8',
         # 'mysql-connector-python>=8.0.13',
     ],
-    version='1.6.1',
+    version='1.6.2',
     url='https://gitee.com/summry/mysqlx',
-    author='summry',
+    author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
     },
     include_package_data=True,
```

