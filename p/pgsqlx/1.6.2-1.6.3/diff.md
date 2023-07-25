# Comparing `tmp/pgsqlx-1.6.2.tar.gz` & `tmp/pgsqlx-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pgsqlx-1.6.2.tar", last modified: Mon Jul 24 07:28:28 2023, max compression
+gzip compressed data, was "dist\pgsqlx-1.6.3.tar", last modified: Tue Jul 25 08:28:37 2023, max compression
```

## Comparing `pgsqlx-1.6.2.tar` & `pgsqlx-1.6.3.tar`

### file list

```diff
@@ -1,20 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 07:28:28.000000 pgsqlx-1.6.2/
-drwxrwxrwx   0        0        0        0 2023-07-24 07:28:28.000000 pgsqlx-1.6.2/pgsqlx/
--rw-rw-rw-   0        0        0     1426 2023-07-24 00:56:26.000000 pgsqlx-1.6.2/pgsqlx/db.py
--rw-rw-rw-   0        0        0      630 2023-07-24 00:18:48.000000 pgsqlx-1.6.2/pgsqlx/dbx.py
--rw-rw-rw-   0        0        0      534 2023-07-24 00:56:26.000000 pgsqlx-1.6.2/pgsqlx/log_support.py
--rw-rw-rw-   0        0        0     1889 2023-07-24 01:02:17.000000 pgsqlx-1.6.2/pgsqlx/orm.py
--rw-rw-rw-   0        0        0      115 2023-07-24 02:35:21.000000 pgsqlx-1.6.2/pgsqlx/snowflake.py
--rw-rw-rw-   0        0        0      103 2023-07-24 00:31:03.000000 pgsqlx-1.6.2/pgsqlx/sql_mapper.py
--rw-rw-rw-   0        0        0      125 2023-07-23 23:06:11.000000 pgsqlx-1.6.2/pgsqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 07:28:28.000000 pgsqlx-1.6.2/pgsqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-24 07:28:28.000000 pgsqlx-1.6.2/pgsqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-24 07:28:28.000000 pgsqlx-1.6.2/pgsqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4639 2023-07-24 07:28:28.000000 pgsqlx-1.6.2/pgsqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       48 2023-07-24 07:28:28.000000 pgsqlx-1.6.2/pgsqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      320 2023-07-24 07:28:28.000000 pgsqlx-1.6.2/pgsqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-24 07:28:28.000000 pgsqlx-1.6.2/pgsqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4639 2023-07-24 07:28:28.000000 pgsqlx-1.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     4122 2023-07-24 07:27:35.000000 pgsqlx-1.6.2/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-24 07:28:28.000000 pgsqlx-1.6.2/setup.cfg
--rw-rw-rw-   0        0        0     1233 2023-07-24 07:28:25.000000 pgsqlx-1.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:28:37.000000 pgsqlx-1.6.3/
+drwxrwxrwx   0        0        0        0 2023-07-25 08:28:37.000000 pgsqlx-1.6.3/pgsqlx/
+-rw-rw-rw-   0        0        0     1072 2023-07-25 07:22:11.000000 pgsqlx-1.6.3/pgsqlx/db.py
+-rw-rw-rw-   0        0        0      534 2023-07-24 00:56:26.000000 pgsqlx-1.6.3/pgsqlx/log_support.py
+-rw-rw-rw-   0        0        0     1892 2023-07-25 08:08:47.000000 pgsqlx-1.6.3/pgsqlx/orm.py
+-rw-rw-rw-   0        0        0      629 2023-07-25 06:13:56.000000 pgsqlx-1.6.3/pgsqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:28:37.000000 pgsqlx-1.6.3/pgsqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-25 08:28:37.000000 pgsqlx-1.6.3/pgsqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-25 08:28:37.000000 pgsqlx-1.6.3/pgsqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4612 2023-07-25 08:28:37.000000 pgsqlx-1.6.3/pgsqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2023-07-25 08:28:37.000000 pgsqlx-1.6.3/pgsqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      265 2023-07-25 08:28:37.000000 pgsqlx-1.6.3/pgsqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-25 08:28:37.000000 pgsqlx-1.6.3/pgsqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4612 2023-07-25 08:28:37.000000 pgsqlx-1.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4096 2023-07-25 08:21:22.000000 pgsqlx-1.6.3/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-25 08:28:37.000000 pgsqlx-1.6.3/setup.cfg
+-rw-rw-rw-   0        0        0     1237 2023-07-25 08:27:48.000000 pgsqlx-1.6.3/setup.py
```

### Comparing `pgsqlx-1.6.2/pgsqlx/db.py` & `pgsqlx-1.6.3/pgsqlx/db.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,13 @@
-from sqlbatis import Engin, DBEngin
+from sqlexec.engin import PostgresEngin
 from .log_support import save_log, save_key_seq_log
 
 # Don't remove. Import for not repetitive implementation
-from sqlbatis.db import init_db as supper_init_db, insert, save as save_select_key, execute, batch_insert, batch_execute, get, query, query_one, \
-    query_page, select, select_one, select_page, do_execute, do_get, do_query, do_query_one, do_query_page, do_select, do_select_one, do_select_page
-
-_DB_CTX = None
-
-
-def init_db(user='root', password='', database='test', host='127.0.0.1', port=3306, pool_size=0, show_sql=False, **kwargs):
-    supper_init_db(user=user, password=password, database=database, host=host, port=port, engin=Engin.POSTGRESQL, pool_size=pool_size, \
-                   show_sql=show_sql, **kwargs)
+from sqlbatis.db import insert, save as save_select_key, execute, batch_insert, batch_execute, get, query, query_one, query_page, select, select_one,\
+    select_page, do_execute, do_get, do_query, do_query_one, do_query_page, do_select, do_select_one, do_select_page
 
 
 def save(table: str, **kwargs):
     """
     Insert data into table, return primary key.
     :param table: table
     :param kwargs:
@@ -29,10 +22,9 @@
     Insert data into table, return primary key.
     :param key_seq: primary key sequnece
     :param table: table
     :param kwargs:
     :return: Primary key
     """
     save_key_seq_log(key_seq, table, **kwargs)
-    return save_select_key(DBEngin.get_select_key(key_seq=key_seq), table, **kwargs)
-
+    return save_select_key(PostgresEngin.get_select_key(key_seq=key_seq), table, **kwargs)
```

### Comparing `pgsqlx-1.6.2/pgsqlx/log_support.py` & `pgsqlx-1.6.3/pgsqlx/log_support.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.6.2/pgsqlx/orm.py` & `pgsqlx-1.6.3/pgsqlx/orm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .snowflake import get_id
+from . import get_snowflake_id
 from .db import insert, save_key_seq
 from .log_support import orm_insert_log
 
 # Don't remove. Import for not repetitive implementation
 from sqlbatis.orm import DelFlag, KeyStrategy, Model as BaseModel
 
 
@@ -24,35 +24,35 @@
             self.update_by = update_by
             self.update_time = update_time
             self.del_flag = del_flag
             self.name = name
             self.age = age
 
     then you can use like follow:
-        db.init_db(person='xxx', password='xxx', database='xxx', host='xxx', ...)  # or dbx.init_db(...) init db first,
+        init_db(person='xxx', password='xxx', database='xxx', host='xxx', ...)  # or dbx.init_db(...) init db first,
         person = Person(name='张三', age=55)
         effect_rowcount = person.persist()
         id = person.inst_save()
     """
 
     @classmethod
     def save(cls, **kwargs):
         """
         id = Person.save(name='张三', age=20)
         :return: Primary key
         """
         orm_insert_log('save', cls.__name__, **kwargs)
         key, table = cls._get_key_and_table()
+        if key in kwargs:
+            insert(table, **kwargs)
+            return kwargs[key]
+
         key_strategy = cls._get_key_strategy()
         if key_strategy == KeyStrategy.SNOWFLAKE:
-            if key in kwargs:
-                _id = kwargs[key]
-            else:
-                _id = get_id()
-                kwargs[key] = _id
+            kwargs[key] = get_snowflake_id()
             insert(table, **kwargs)
+            return kwargs[key]
         else:
             key_seq = cls._get_key_seq()
-            _id = save_key_seq(key_seq, table, **kwargs)
-        return _id
+            return save_key_seq(key_seq, table, **kwargs)
```

### Comparing `pgsqlx-1.6.2/pgsqlx.egg-info/PKG-INFO` & `pgsqlx-1.6.3/pgsqlx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.6.2
+Version: 1.6.3
 Summary: PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
@@ -39,18 +39,17 @@
    </mapper>
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
-   from pgsqlx import db, dbx
    from pgsqlx.orm import Model
-   from pgsqlx.sql_mapper import mapper, sql
    from typing import List, Tuple, Mapping
+   from pgsqlx import mapper, sql, db, dbx, init_db
 
    @mapper(namespace='person')
    def select_all(): List
 
    @mapper(namespace='person')
    def select_by_name(name: str): List
 
@@ -58,15 +57,15 @@
    def query_all(): List(Mapping)
 
    @sql('select id, name, age from person where name=?')
    def query_by_name(name: str): List(Mapping)
 
 
    if __name__ == '__main__':
-       db.init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', pool_size=5, show_sql=True, mapper_path='./mapper')
+       init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', pool_size=5, show_sql=True, mapper_path='./mapper')
        
        persons = select_all()
        # result:
        # (3, 'zhangsan', 15)
        # (4, 'lisi', 26)
        # (5, 'wangwu', 38)
```

### Comparing `pgsqlx-1.6.2/PKG-INFO` & `pgsqlx-1.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.6.2
+Version: 1.6.3
 Summary: PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
@@ -39,18 +39,17 @@
    </mapper>
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
-   from pgsqlx import db, dbx
    from pgsqlx.orm import Model
-   from pgsqlx.sql_mapper import mapper, sql
    from typing import List, Tuple, Mapping
+   from pgsqlx import mapper, sql, db, dbx, init_db
 
    @mapper(namespace='person')
    def select_all(): List
 
    @mapper(namespace='person')
    def select_by_name(name: str): List
 
@@ -58,15 +57,15 @@
    def query_all(): List(Mapping)
 
    @sql('select id, name, age from person where name=?')
    def query_by_name(name: str): List(Mapping)
 
 
    if __name__ == '__main__':
-       db.init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', pool_size=5, show_sql=True, mapper_path='./mapper')
+       init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', pool_size=5, show_sql=True, mapper_path='./mapper')
        
        persons = select_all()
        # result:
        # (3, 'zhangsan', 15)
        # (4, 'lisi', 26)
        # (5, 'wangwu', 38)
```

### Comparing `pgsqlx-1.6.2/README.rst` & `pgsqlx-1.6.3/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -26,18 +26,17 @@
    </mapper>
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
-   from pgsqlx import db, dbx
    from pgsqlx.orm import Model
-   from pgsqlx.sql_mapper import mapper, sql
    from typing import List, Tuple, Mapping
+   from pgsqlx import mapper, sql, db, dbx, init_db
 
    @mapper(namespace='person')
    def select_all(): List
 
    @mapper(namespace='person')
    def select_by_name(name: str): List
 
@@ -45,15 +44,15 @@
    def query_all(): List(Mapping)
 
    @sql('select id, name, age from person where name=?')
    def query_by_name(name: str): List(Mapping)
 
 
    if __name__ == '__main__':
-       db.init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', pool_size=5, show_sql=True, mapper_path='./mapper')
+       init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', pool_size=5, show_sql=True, mapper_path='./mapper')
        
        persons = select_all()
        # result:
        # (3, 'zhangsan', 15)
        # (4, 'lisi', 26)
        # (5, 'wangwu', 38)
```

### Comparing `pgsqlx-1.6.2/setup.py` & `pgsqlx-1.6.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 setup(
     name='pgsqlx',
     packages=['pgsqlx'],
     description="PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
-        'Jinja2>=2.7.0',
-        'psycopg2>=2.7.4',
-        'sqlx-batis>=0.0.7',
+        # 'Jinja2>=2.7.0',
+        # 'psycopg2>=2.7.4',
+        'sqlx-batis>=0.0.8',
     ],
-    version='1.6.2',
+    version='1.6.3',
     url='https://gitee.com/summry/pgsqlx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

