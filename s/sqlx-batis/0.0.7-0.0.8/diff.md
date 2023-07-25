# Comparing `tmp/sqlx-batis-0.0.7.tar.gz` & `tmp/sqlx-batis-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-batis-0.0.7.tar", last modified: Mon Jul 24 01:45:01 2023, max compression
+gzip compressed data, was "dist\sqlx-batis-0.0.8.tar", last modified: Tue Jul 25 08:26:54 2023, max compression
```

## Comparing `sqlx-batis-0.0.7.tar` & `sqlx-batis-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 01:45:01.000000 sqlx-batis-0.0.7/
--rw-rw-rw-   0        0        0     3427 2023-07-24 01:45:01.000000 sqlx-batis-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2945 2023-07-23 14:10:39.000000 sqlx-batis-0.0.7/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-24 01:45:01.000000 sqlx-batis-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1209 2023-07-23 23:35:52.000000 sqlx-batis-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:45:01.000000 sqlx-batis-0.0.7/sqlbatis/
--rw-rw-rw-   0        0        0      394 2023-07-23 23:51:01.000000 sqlx-batis-0.0.7/sqlbatis/constant.py
--rw-rw-rw-   0        0        0     8455 2023-07-23 23:23:36.000000 sqlx-batis-0.0.7/sqlbatis/db.py
--rw-rw-rw-   0        0        0     6538 2023-07-23 23:33:37.000000 sqlx-batis-0.0.7/sqlbatis/dbx.py
--rw-rw-rw-   0        0        0      806 2023-07-23 23:51:27.000000 sqlx-batis-0.0.7/sqlbatis/exec_support.py
--rw-rw-rw-   0        0        0     3875 2023-07-22 21:17:32.000000 sqlx-batis-0.0.7/sqlbatis/log_support.py
--rw-rw-rw-   0        0        0    38662 2023-07-23 23:51:00.000000 sqlx-batis-0.0.7/sqlbatis/orm.py
--rw-rw-rw-   0        0        0     2392 2023-07-23 22:35:05.000000 sqlx-batis-0.0.7/sqlbatis/snowflake.py
--rw-rw-rw-   0        0        0     7067 2023-07-23 23:51:27.000000 sqlx-batis-0.0.7/sqlbatis/sql_holder.py
--rw-rw-rw-   0        0        0     4126 2023-07-23 23:51:27.000000 sqlx-batis-0.0.7/sqlbatis/sql_mapper.py
--rw-rw-rw-   0        0        0     1421 2023-07-23 14:00:47.000000 sqlx-batis-0.0.7/sqlbatis/sql_support.py
--rw-rw-rw-   0        0        0      354 2023-07-23 22:35:05.000000 sqlx-batis-0.0.7/sqlbatis/support.py
--rw-rw-rw-   0        0        0      154 2023-07-23 13:54:14.000000 sqlx-batis-0.0.7/sqlbatis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:45:01.000000 sqlx-batis-0.0.7/sqlx_batis.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-24 01:45:01.000000 sqlx-batis-0.0.7/sqlx_batis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-23 23:08:12.000000 sqlx-batis-0.0.7/sqlx_batis.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     3427 2023-07-24 01:45:01.000000 sqlx-batis-0.0.7/sqlx_batis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       31 2023-07-24 01:45:01.000000 sqlx-batis-0.0.7/sqlx_batis.egg-info/requires.txt
--rw-rw-rw-   0        0        0      471 2023-07-24 01:45:01.000000 sqlx-batis-0.0.7/sqlx_batis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2023-07-24 01:45:01.000000 sqlx-batis-0.0.7/sqlx_batis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 08:26:54.000000 sqlx-batis-0.0.8/
+-rw-rw-rw-   0        0        0     3401 2023-07-25 08:26:54.000000 sqlx-batis-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2920 2023-07-25 08:19:31.000000 sqlx-batis-0.0.8/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-25 08:26:54.000000 sqlx-batis-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1209 2023-07-25 08:26:28.000000 sqlx-batis-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:26:54.000000 sqlx-batis-0.0.8/sqlbatis/
+-rw-rw-rw-   0        0        0      394 2023-07-23 23:51:01.000000 sqlx-batis-0.0.8/sqlbatis/constant.py
+-rw-rw-rw-   0        0        0     7935 2023-07-25 06:01:24.000000 sqlx-batis-0.0.8/sqlbatis/db.py
+-rw-rw-rw-   0        0        0     6141 2023-07-25 06:01:24.000000 sqlx-batis-0.0.8/sqlbatis/dbx.py
+-rw-rw-rw-   0        0        0      806 2023-07-23 23:51:27.000000 sqlx-batis-0.0.8/sqlbatis/exec_support.py
+-rw-rw-rw-   0        0        0     3839 2023-07-24 13:45:51.000000 sqlx-batis-0.0.8/sqlbatis/log_support.py
+-rw-rw-rw-   0        0        0    39064 2023-07-25 08:11:50.000000 sqlx-batis-0.0.8/sqlbatis/orm.py
+-rw-rw-rw-   0        0        0     2402 2023-07-25 04:27:05.000000 sqlx-batis-0.0.8/sqlbatis/snowflake.py
+-rw-rw-rw-   0        0        0     7067 2023-07-23 23:51:27.000000 sqlx-batis-0.0.8/sqlbatis/sql_holder.py
+-rw-rw-rw-   0        0        0     4126 2023-07-23 23:51:27.000000 sqlx-batis-0.0.8/sqlbatis/sql_mapper.py
+-rw-rw-rw-   0        0        0     1421 2023-07-23 14:00:47.000000 sqlx-batis-0.0.8/sqlbatis/sql_support.py
+-rw-rw-rw-   0        0        0      354 2023-07-23 22:35:05.000000 sqlx-batis-0.0.8/sqlbatis/support.py
+-rw-rw-rw-   0        0        0      690 2023-07-25 06:01:24.000000 sqlx-batis-0.0.8/sqlbatis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:26:54.000000 sqlx-batis-0.0.8/sqlx_batis.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-25 08:26:54.000000 sqlx-batis-0.0.8/sqlx_batis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-23 23:08:12.000000 sqlx-batis-0.0.8/sqlx_batis.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     3401 2023-07-25 08:26:54.000000 sqlx-batis-0.0.8/sqlx_batis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2023-07-25 08:26:54.000000 sqlx-batis-0.0.8/sqlx_batis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      471 2023-07-25 08:26:54.000000 sqlx-batis-0.0.8/sqlx_batis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2023-07-25 08:26:54.000000 sqlx-batis-0.0.8/sqlx_batis.egg-info/top_level.txt
```

### Comparing `sqlx-batis-0.0.7/PKG-INFO` & `sqlx-batis-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 0.0.7
+Version: 0.0.8
 Summary: sqlx-batis is a sql executor for Python like MyBatis.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
@@ -39,17 +39,16 @@
    </mapper>
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
-   from sqlbatis import dbx, Engin
    from typing import List, Tuple, Mapping
-   from sqlbatis.sql_mapper import mapper, sql
+   from sqlbatis import mapper, sql, dbx, Engin, init_db
 
    @mapper(namespace='person')
    def select_all(): List
 
    @mapper(namespace='person')
    def select_by_name(name: str): List
```

### Comparing `sqlx-batis-0.0.7/README.rst` & `sqlx-batis-0.0.8/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -26,17 +26,16 @@
    </mapper>
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
-   from sqlbatis import dbx, Engin
    from typing import List, Tuple, Mapping
-   from sqlbatis.sql_mapper import mapper, sql
+   from sqlbatis import mapper, sql, dbx, Engin, init_db
 
    @mapper(namespace='person')
    def select_all(): List
 
    @mapper(namespace='person')
    def select_by_name(name: str): List
```

### Comparing `sqlx-batis-0.0.7/setup.py` & `sqlx-batis-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     name='sqlx-batis',
     packages=['sqlbatis'],
     description="sqlx-batis is a sql executor for Python like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
-        'sqlx-exec>=1.1.5',
+        'sqlx-exec>=1.1.6',
     ],
-    version='0.0.7',
+    version='0.0.8',
     url='https://gitee.com/summry/sqlx-batis',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-batis-0.0.7/sqlbatis/db.py` & `sqlx-batis-0.0.8/sqlbatis/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,13 @@
-from . import sql_support, Engin
-from .constant import MAPPER_PATH
+from . import sql_support
 from .log_support import sql_log, page_log, do_sql_log
 
 # Don't remove. Import for not repetitive implementation
-from sqlexec import init_db as supper_init_db, insert, save, batch_insert, batch_execute, execute as supper_execute, get as supper_get, \
-    query as supper_query, query_one as supper_query_one, query_page as supper_query_page, select as supper_select, select_one as supper_select_one, \
-    select_page as supper_select_page
-
-
-def init_db(user='root', password='', database='test', host='127.0.0.1', port=3306, engin=Engin.MYSQL, pool_size=0, show_sql=False, **kwargs):
-    if MAPPER_PATH in kwargs:
-        from .sql_holder import load_mapper
-        load_mapper(kwargs.pop(MAPPER_PATH))
-    supper_init_db(user=user, password=password, database=database, host=host, port=port, engin=engin, pool_size=pool_size, show_sql=show_sql,
-                   **kwargs)
+from sqlexec import insert, save, batch_insert, batch_execute, execute as supper_execute, get as supper_get, query_one as supper_query_one, \
+    query as supper_query, query_page as supper_query_page, select as supper_select, select_one as supper_select_one, select_page as supper_select_page
 
 
 # ----------------------------------------------------------Update function------------------------------------------------------------------
 def execute(sql: str, *args, **kwargs):
     """
     Execute SQL.
     sql: INSERT INTO user(name, age) VALUES(?, ?)  -->  args: ('张三', 20)
```

### Comparing `sqlx-batis-0.0.7/sqlbatis/dbx.py` & `sqlx-batis-0.0.8/sqlbatis/dbx.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 from .exec_support import do_save
 from .sql_support import get_batch_args
 from . import Engin, sql_holder as holder
 from .log_support import logger, sql_id_log, page_sql_id_log
 
 # Don't remove. Import for not repetitive implementation
-from .db import(init_db as supper_init_db, do_execute, insert, batch_insert, batch_execute as db_batch_execute, do_get, do_query, do_query_one, \
-                do_query_page, do_select, do_select_one, do_select_page)
-
-
-def init_db(user='root', password='', database='test', host='127.0.0.1', port=3306, mapper_path='mapper', engin=Engin.MYSQL, pool_size=0,
-        show_sql=False, **kwargs):
-    holder.load_mapper(mapper_path)
-    supper_init_db(user=user, password=password, database=database, host=host, port=port, engin=engin, pool_size=pool_size, show_sql=show_sql, **kwargs)
+from .db import(do_execute, insert, batch_insert, batch_execute as db_batch_execute, do_get, do_query, do_query_one, do_query_page, do_select, \
+                do_select_one, do_select_page)
 
 
 def save(sql_id: str, *args, **kwargs):
     """
     Execute insert SQL, return primary key.
     :return: Primary key
     """
```

### Comparing `sqlx-batis-0.0.7/sqlbatis/exec_support.py` & `sqlx-batis-0.0.8/sqlbatis/exec_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.0.7/sqlbatis/log_support.py` & `sqlx-batis-0.0.8/sqlbatis/log_support.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 from sqlexec.log_support import logger
 
 def sql_log(function: str, sql: str, *args, **kwargs):
-    logger.debug("Exec func 'sqlx-batis.db.%s' \n\tsql: %s \n\targs: %s \n\tkwargs: %s" % (function, sql.strip(), args, kwargs))
+    logger.debug("Exec func 'sqlbatis.db.%s' \n\tsql: %s \n\targs: %s \n\tkwargs: %s" % (function, sql.strip(), args, kwargs))
 
 
 def page_log(function: str, sql: str, page_num, page_size, *args, **kwargs):
-    logger.debug("Exec func 'sqlx-batis.db.%s', page_num: %d, page_size: %d \n\tsql: %s \n\targs: %s \n\tkwargs: %s" % (
+    logger.debug("Exec func 'sqlbatis.db.%s', page_num: %d, page_size: %d \n\tsql: %s \n\targs: %s \n\tkwargs: %s" % (
         function, page_num, page_size, sql.strip(), args, kwargs))
 
 
 def insert_log(function: str, table: str, **kwargs):
-    logger.debug("Exec func 'sqlx-batis.db.%s' \n\t Table: '%s', kwargs: %s" % (function, table, kwargs))
+    logger.debug("Exec func 'sqlbatis.db.%s' \n\t Table: '%s', kwargs: %s" % (function, table, kwargs))
 
 
 def do_sql_log(function: str, sql: str, *args):
-    logger.debug("Exec func 'sqlx-batis.db.%s' \n\t sql: %s \n\t args: %s" % (function, sql, args))
+    logger.debug("Exec func 'sqlbatis.db.%s' \n\t sql: %s \n\t args: %s" % (function, sql, args))
 
 
 def do_page_log(function: str, sql: str, page_num, page_size, *args):
     logger.debug(
-        "Exec func 'sqlx-batis.db.%s', page_num: %d, page_size: %d \n\t sql: %s \n\t args: %s" % (function, page_num, page_size, sql.strip(), args))
+        "Exec func 'sqlbatis.db.%s', page_num: %d, page_size: %d \n\t sql: %s \n\t args: %s" % (function, page_num, page_size, sql.strip(), args))
 def sql_id_log(function: str, sql_id: str, *args, **kwargs):
-    logger.debug("Exec func 'sqlx-batis.%s', sql_id: %s, args: %s, kwargs: %s" % (function, sql_id.strip(), args, kwargs))
+    logger.debug("Exec func 'sqlbatis.%s', sql_id: %s, args: %s, kwargs: %s" % (function, sql_id.strip(), args, kwargs))
 
 
 def page_sql_id_log(function: str, sql_id: str, page_num, page_size, *args, **kwargs):
-    logger.debug("Exec func 'sqlx-batis.%s', page_num: %d, page_size: %d, sql_id: %s, args: %s, kwargs: %s" % (function, page_num, page_size, sql_id, args, kwargs))
+    logger.debug("Exec func 'sqlbatis.%s', page_num: %d, page_size: %d, sql_id: %s, args: %s, kwargs: %s" % (function, page_num, page_size, sql_id, args, kwargs))
 
 
 def orm_by_page_log(function, page_num, page_size, class_name, where, *args, **kwargs):
-    logger.debug("Exec func 'sqlx-batis.orm.Model.%s', page_num: %d, page_size: %d \n\t Class: '%s', where: %s, args: %s, kwargs: %s" % (
+    logger.debug("Exec func 'sqlbatis.orm.Model.%s', page_num: %d, page_size: %d \n\t Class: '%s', where: %s, args: %s, kwargs: %s" % (
         function, page_num, page_size, class_name, where, args, kwargs))
 
 
 def orm_page_log(function, page_num, page_size, class_name, *fields, **kwargs):
-    logger.debug("Exec func 'sqlx-batis.orm.Model.%s', page_num: %d, page_size: %d \n\t Class: '%s', fields: %s, kwargs: %s" % (
+    logger.debug("Exec func 'sqlbatis.orm.Model.%s', page_num: %d, page_size: %d \n\t Class: '%s', fields: %s, kwargs: %s" % (
         function, page_num, page_size, class_name, fields, kwargs))
 
 
 def orm_insert_log(function, class_name, **kwargs):
-    logger.debug("Exec func 'sqlx-batis.orm.Model.%s' \n\t Class: '%s', kwargs: %s" % (function, class_name, kwargs))
+    logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', kwargs: %s" % (function, class_name, kwargs))
 
 
 def orm_delete_by_id_log(function, class_name, _id, update_by):
-    logger.debug("Exec func 'sqlx-batis.orm.Model.%s' \n\t Class: '%s', id: %d, update_by: %s" % (function, class_name, _id, update_by))
+    logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', id: %d, update_by: %s" % (function, class_name, _id, update_by))
 
 
 def orm_by_log(function, class_name, where, *args, **kwargs):
-    logger.debug("Exec func 'sqlx-batis.orm.Model.%s' \n\t Class: '%s', where: %s, args: %s, kwargs: %s" % (function, class_name, where, args, kwargs))
+    logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', where: %s, args: %s, kwargs: %s" % (function, class_name, where, args, kwargs))
 
 
 def orm_inst_log(function, class_name):
-    logger.debug("Exec func 'sqlx-batis.orm.Model.%s', Class: '%s'" % (function, class_name))
+    logger.debug("Exec func 'sqlbatis.orm.Model.%s', Class: '%s'" % (function, class_name))
 
 
 def orm_logical_delete_by_ids_log(function, class_name, ids, update_by, batch_size):
-    logger.debug("Exec func 'sqlx-batis.orm.Model.%s' \n\t Class: '%s', ids: %s, update_by: %s, batch_size: %s" % (
+    logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', ids: %s, update_by: %s, batch_size: %s" % (
     function, class_name, ids, update_by, batch_size))
 
 
 def orm_count_log(function, class_name, **kwargs):
-    logger.debug("Exec func 'sqlx-batis.orm.Model.%s' \n\t Class: '%s', kwargs: %s" % (function, class_name, kwargs))
+    logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', kwargs: %s" % (function, class_name, kwargs))
 
 
 def orm_find_log(function, class_name, *fields, **kwargs):
-    logger.debug("Exec func 'sqlx-batis.orm.Model.%s' \n\t Class: '%s', fields: %s, kwargs: %s" % (function, class_name, fields, kwargs))
+    logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', fields: %s, kwargs: %s" % (function, class_name, fields, kwargs))
 
 
 def orm_find_by_id_log(function, class_name, _id, *fields):
-    logger.debug("Exec func 'sqlx-batis.orm.Model.%s' \n\t Class: '%s', id: %d, fields: %s" % (function, class_name, _id, fields))
+    logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', id: %d, fields: %s" % (function, class_name, _id, fields))
 
 
 def orm_find_by_ids_log(function, class_name, ids, *fields):
-    logger.debug("Exec func 'sqlx-batis.orm.Model.%s' \n\t Class: '%s', ids: %s, fields: %s" % (function, class_name, ids, fields))
+    logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', ids: %s, fields: %s" % (function, class_name, ids, fields))
```

### Comparing `sqlx-batis-0.0.7/sqlbatis/orm.py` & `sqlx-batis-0.0.8/sqlbatis/orm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import sqlexec
 from datetime import datetime
-from .snowflake import get_id
 from enum import Enum, IntEnum
 from functools import lru_cache
 from .sql_support import simple_sql
+from .snowflake import get_snowflake_id
 from .support import DBError, NotFoundError
 from typing import Sequence, Union, List, Tuple
 from . import db, log_support, transaction, DBEngin
 from .constant import LIMIT_1, NO_LIMIT, DEFAULT_KEY_FIELD, KEY, KEY_SEQ, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, KEY_STRATEGY, CACHE_SIZE
 
 
 class DelFlag(IntEnum):
@@ -49,15 +49,15 @@
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
 
     def __str__(self):
         return str({k: v for k, v in self.__dict__.items() if not k.startswith("__")})
@@ -70,67 +70,63 @@
         elif UPDATE_BY == name:
             return self._get_update_by_field()
         elif UPDATE_TIME == name:
             return self._get_update_time_field()
         else:
             return None
 
-    def persist(self):
+    def persist(self, ignored_none=True, *fields):
         """
         person = Person(name='张三', age=55)
         effect_rowcount = person.persist()
         :return: effect rowcount
         """
         log_support.orm_inst_log('persist', self.__class__.__name__)
-        kv = {k: v for k, v in self.__dict__.items() if v is not None}
+        kv = self._get_kv(ignored_none, None, *fields)
         return self.insert(**kv)
 
-    def inst_save(self):
+    def inst_save(self, ignored_none=True, *fields):
         """
         person = Person(name='张三', age=55)
         id = person.save()
         :return: Primary key
         """
         log_support.orm_inst_log('inst_save', self.__class__.__name__)
-        kv = {k: v for k, v in self.__dict__.items() if v is not None}
         key = self._get_key()
+        kv = self._get_kv(ignored_none, None, *fields)
         _id = self.save(**kv)
         if key not in kv:
             self.__dict__.update({key: _id})
         return _id
-
-    def update(self, ignored_none=True):
+    def update(self, ignored_none=True, *fields):
         """
         person = Person(id=1, name='李四', age=66)
         rowcount = person.update()
         :return: Effect rowcount
         """
         log_support.orm_inst_log('update', self.__class__.__name__)
         key, table = self._get_key_and_table()
-        if ignored_none:
-            kv = {k: v for k, v in self.__dict__.items() if v is not None}
-        else:
-            kv = {k: v for k, v in self.__dict__.items()}
+        kv = self._get_kv(ignored_none, key, *fields)
         _id = kv[key]
         assert _id is not None, 'Primary key must not be None.'
         update_kv = {k: v for k, v in kv.items() if k != key}
         if update_kv:
             return self.update_by_id(_id, **update_kv)
         else:
-            log_support.logger.warning("Exec func 'sqlx-batis.orm.Model.%s' not set fields, Class: '%s:'\n\t   %s" % ('update', self.__class__.__name__, self))
+            log_support.logger.warning("Exec func 'sqlbatis.orm.Model.%s' not set fields, Class: '%s:'\n\t   %s" % ('update', self.__class__.__name__, self))
             return 0
 
     def load(self, *fields):
         """
         Return new object from database and update itself.
         :param fields: Default select all fields if not set. like: ('id', 'name', 'age')
         person = Person(id=1)
         person2 = person.load()
         """
-        log_support.logger.debug("Exec func 'sqlx-batis.orm.Model.%s', Class: '%s', fields: %s" % ('load', self.__class__.__name__, fields))
+        log_support.logger.debug("Exec func 'sqlbatis.orm.Model.%s', Class: '%s', fields: %s" % ('load', self.__class__.__name__, fields))
         key = self._get_key()
         kv = self.__dict__
         _id = kv.get(key)
         assert _id is not None, 'Primary key must not be None.'
         if not fields:
             fields, _ = zip(*kv.items())
         result = self.query_by_id(_id, *fields)
@@ -187,61 +183,59 @@
         rowcount = Person.insert(name='张三', age=20)
         return: Effect rowcount
         """
         log_support.orm_insert_log('insert', cls.__name__, **kwargs)
         key, table = cls._get_key_and_table()
         key_strategy = cls._get_key_strategy()
         if key_strategy == KeyStrategy.SNOWFLAKE and key not in kwargs:
-            kwargs[key] = get_id()
+            kwargs[key] = get_snowflake_id()
         return sqlexec.insert(table, **kwargs)
 
     @classmethod
     def save(cls, **kwargs):
         """
         id = Person.save(name='张三', age=20)
         :return: Primary key
         """
         log_support.orm_insert_log('save', cls.__name__, **kwargs)
         key, table = cls._get_key_and_table()
+        if key in kwargs:
+            sqlexec.insert(table, **kwargs)
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
             sqlexec.insert(table, **kwargs)
+            return kwargs[key]
         else:
             key_seq = cls._get_key_seq()
-            _id = sqlexec.save(DBEngin.get_select_key(key_seq=key_seq, table=table), table, **kwargs)
-        return _id
+            return sqlexec.save(DBEngin.get_select_key(key_seq=key_seq), table, **kwargs)
 
     @classmethod
     def create(cls, **kwargs):
         """
         person = Person.create(name='张三', age=20)
         :return: Instance object
         """
         log_support.orm_insert_log('create', cls.__name__, **kwargs)
         key = cls._get_key()
-        _id = cls.save(**kwargs)
-        if key not in kwargs:
-            kwargs[key] = _id
+        kwargs[key] = cls.save(**kwargs)
         return cls.to_obj(**kwargs)
 
     @classmethod
     def update_by_id(cls, _id: Union[int, str], **kwargs):
         """
         rowcount = Person.update_by_id(id=1, name='王五')
         return: Effect rowcount
         """
-        log_support.logger.debug("Exec func 'sqlx-batis.orm.Model.%s' \n\t Class: '%s', id: %d, kwargs: %s" % ('update_by_id', cls.__name__, _id, kwargs))
+        log_support.logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', id: %d, kwargs: %s" % ('update_by_id', cls.__name__, _id, kwargs))
         assert kwargs, 'Must set update kv'
         key = cls._get_key()
-        where = '%s=?' % key
+        where = '%s = ?' % key
         cols, args = zip(*kwargs.items())
         sql, update_time_arg = cls._update_sql(where, *cols)
         if update_time_arg:
             args = [*args, update_time_arg]
         return sqlexec.execute(sql, *args, _id)
 
     @classmethod
@@ -301,27 +295,27 @@
     @classmethod
     def delete_by_id(cls, _id: Union[int, str]):
         """
         Physical delete
         rowcount = Person.delete_by_id(id=1)
         return: Effect rowcount
         """
-        log_support.logger.debug("Exec func 'sqlx-batis.orm.Model.%s' \n\t Class: '%s', id: %d" % ('delete_by_id', cls.__name__, _id))
+        log_support.logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', id: %d" % ('delete_by_id', cls.__name__, _id))
         key, table = cls._get_key_and_table()
-        sql = 'DELETE FROM %s WHERE %s=?' % (table, key)
+        sql = 'DELETE FROM %s WHERE %s = ?' % (table, key)
         return sqlexec.execute(sql, _id)
 
     @classmethod
     def delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], batch_size=128):
         """
         Batch physical delete, they will be executed in batches if there are too many
         rowcount = Person.delete_by_ids(id=[1,2])
         return: Effect rowcount
         """
-        log_support.logger.debug("Exec func 'sqlx-batis.orm.Model.%s' \n\t Class: '%s', ids: %s, batch_size: %s" % ('delete_by_ids', cls.__name__, ids, batch_size))
+        log_support.logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', ids: %s, batch_size: %s" % ('delete_by_ids', cls.__name__, ids, batch_size))
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
         if ids_size == 1:
             return cls.delete_by_id(ids[0])
         elif ids_size <= batch_size:
             return cls.do_delete_by_ids(ids)
         else:
@@ -346,22 +340,22 @@
     def batch_insert(cls, *args):
         """
         Batch insert
         rowcount = Person.batch_insert([{'name': '张三', 'age': 55},{'name': '李四', 'age': 66}])
         :param args: All number must have same key.
         :return: Effect rowcount
         """
-        log_support.logger.debug("Exec func 'sqlx-batis.orm.Model.%s' \n\t Class: '%s', args: %s" % ('batch_insert', cls.__name__, args))
+        log_support.logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', args: %s" % ('batch_insert', cls.__name__, args))
         assert len(args) > 0, 'args must not be empty.'
         key, table = cls._get_key_and_table()
         key_strategy = cls._get_key_strategy()
         if key_strategy == KeyStrategy.SNOWFLAKE:
             for arg in args:
                 if key not in arg:
-                    arg[key] = get_id()
+                    arg[key] = get_snowflake_id()
 
         return sqlexec.batch_insert(table, *args)
 
     # ------------------------------------------------Class query method--------------------------------------------------------
     @classmethod
     def count(cls, **kwargs):
         """
@@ -553,15 +547,15 @@
         Return one row(dict) or None if no result.
         person = Person.query_by_id(1, 'id', 'name', 'age')
         :param _id: key
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_by_id_log('query_by_id', cls.__name__, _id, *fields)
         key, table = cls._get_key_and_table()
-        where = 'WHERE {}=?'.format(key)
+        where = 'WHERE {} = ?'.format(key)
         sql = _select_sql(table, where, LIMIT_1, *fields)
         return sqlexec.query_one(sql, _id, LIMIT_1)
 
     @classmethod
     def query_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
         """
         Return list(dict) or empty list if no result.
@@ -652,15 +646,15 @@
         Return one row(dict) or None if no result.
         row = Person.select_by_id(1, 'id', 'name', 'age')
         :param _id: key
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_by_id_log('select_by_id', cls.__name__, _id, *fields)
         key, table = cls._get_key_and_table()
-        where = 'WHERE {}=?'.format(key)
+        where = 'WHERE {} = ?'.format(key)
         sql = _select_sql(table, where, LIMIT_1, *fields)
         return sqlexec.select_one(sql, _id, LIMIT_1)
 
     @classmethod
     def select_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
         """
         Return list(dict) or empty list if no result.
@@ -679,27 +673,39 @@
 
     @classmethod
     def to_obj(cls, **kwargs):
         model = cls.__new__(cls)
         model.__dict__.update(**kwargs)
         return model
 
+    def _get_kv(self, ignored_none: bool, key: None, *fields):
+        if fields:
+            if key:
+                fields = (key, *fields)
+            if ignored_none:
+                return {k: v for k, v in self.__dict__.items() if v is not None and k in fields}
+            return {k: v for k, v in self.__dict__.items() if k in fields}
+
+        if ignored_none:
+            return {k: v for k, v in self.__dict__.items() if v is not None}
+        return {k: v for k, v in self.__dict__.items()}
+
     # ------------------------------------------------Private class method------------------------------------------------------------------
     @classmethod
     def _logical_delete_by_id_op(cls, _id: Union[int, str], update_by: Union[int, str] = None, del_status=DelFlag.DELETED):
         key, table = cls._get_key_and_table()
         del_flag_field = cls._get_del_flag_field()
         update_by_field = cls._get_update_by_field()
 
-        where = '%s=?' % key
+        where = '%s = ?' % key
         if update_by is not None and update_by_field is not None:
             sql, update_time_arg = cls._update_sql(where, del_flag_field, update_by_field)
             if update_time_arg:
-                return sqlexec.execute(sql, del_status.value, update_by, update_time_arg, _id, LIMIT_1)
-            return sqlexec.execute(sql, del_status.value, update_by, _id, LIMIT_1)
+                return sqlexec.execute(sql, del_status.value, update_by, update_time_arg, _id)
+            return sqlexec.execute(sql, del_status.value, update_by, _id)
         else:
             sql, update_time_arg = cls._update_sql(where, del_flag_field)
             if update_time_arg:
                 return sqlexec.execute(sql, del_status.value, update_time_arg, _id)
             return sqlexec.execute(sql, del_status.value, _id)
 
     @classmethod
@@ -790,15 +796,15 @@
         update_time_arg = None
         table = cls._get_table()
         update_time_field = cls._get_update_time_field()
         if update_time_field is not None and update_time_field not in update_fields:
             update_fields = [*update_fields, update_time_field]
             update_time_arg = datetime.now()
 
-        update_fields = ','.join(['{}=?'.format(col) for col in update_fields])
+        update_fields = ','.join(['{} = ?'.format(col) for col in update_fields])
         return 'UPDATE {} SET {} WHERE {}'.format(table, update_fields, where), update_time_arg
 
     @classmethod
     def _where_sql(cls, where: str):
         low_where = where.lower()
         if low_where.startswith('where'):
             table = cls._get_table()
@@ -829,29 +835,29 @@
 @lru_cache(maxsize=CACHE_SIZE)
 def _get_table_columns(table: str):
     return sqlexec.get(DBEngin.get_column_sql(), table, LIMIT_1)
 
 
 def _get_condition_arg(k: str, v: object):
     if k.endswith("__eq"):
-        return "{}=?".format(k[:-4]), v
+        return "{} = ?".format(k[:-4]), v
     if k.endswith("__ne"):
-        return "{}!=?".format(k[:-4]), v
+        return "{} != ?".format(k[:-4]), v
     if k.endswith("__gt"):
-        return "{}>?".format(k[:-4]), v
+        return "{} > ?".format(k[:-4]), v
     if k.endswith("__lt"):
-        return "{}<?".format(k[:-4]), v
+        return "{} < ?".format(k[:-4]), v
     if k.endswith("__ge"):
-        return "{}>=?".format(k[:-4]), v
+        return "{} >= ?".format(k[:-4]), v
     if k.endswith("__gte"):
-        return "{}>=?".format(k[:-5]), v
+        return "{} >= ?".format(k[:-5]), v
     if k.endswith("__le"):
-        return "{}<=?".format(k[:-4]), v
+        return "{} <= ?".format(k[:-4]), v
     if k.endswith("__lte"):
-        return "{}<=?".format(k[:-5]), v
+        return "{} <= ?".format(k[:-5]), v
     if k.endswith("__isnull"):
         return "{} is {}".format(k[:-8], 'null' if v else 'not null'), None
     if k.endswith("__in") and isinstance(v, Sequence) and not isinstance(v, str):
         return "{} in({})".format(k[:-4], ','.join(['?' for _ in v])), v
     if k.endswith("__in"):
         return "{} in({})".format(k[:-4], '?'), v
     if k.endswith("__not_in") and isinstance(v, Sequence) and not isinstance(v, str):
@@ -864,21 +870,21 @@
         return "{} like ?".format(k[:-12]), '{}%'.format(v)
     if k.endswith("__endswith"):
         return "{} like ?".format(k[:-10]), '%{}'.format(v)
     if k.endswith("__contains"):
         return "{} like ?".format(k[:-10]), '%{}%'.format(v)
     if k.endswith("__range") and isinstance(v, Sequence) and 2 == len(v) and not isinstance(v, str):
         col = k[:-7]
-        return "{}>=? and {}<=?".format(col, col), v
+        return "{} >= ? and {} <= ?".format(col, col), v
     if k.endswith("__between") and isinstance(v, Sequence) and 2 == len(v) and not isinstance(v, str):
         return "{} between ? and ?".format(k[:-9]), v
     if k.endswith("__range") or k.endswith("__between"):
         return ValueError("Must is instance of Sequence with length 2 when use range or between statement")
 
-    return "{}=?".format(k), v
+    return "{} = ?".format(k), v
 
 
 def _get_where_arg_limit(**kwargs):
     where, args, limit = '', [], 0
     if 'limit' in kwargs:
         limit = kwargs.pop('limit')
```

### Comparing `sqlx-batis-0.0.7/sqlbatis/snowflake.py` & `sqlx-batis-0.0.8/sqlbatis/snowflake.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 def init_snowflake(machine_id=1, epoch=_EPOCH, worker_bits=_WORKER_BITS, sequence_bits=_SEQUENCE_BITS):
     global _SNOWFLAKE
     _SNOWFLAKE = Snowflake(machine_id, epoch, worker_bits, sequence_bits)
 
 
-def get_id():
+def get_snowflake_id():
     global _SNOWFLAKE
     try:
         return _SNOWFLAKE.generate_id()
     except AttributeError:
         raise RuntimeError("Please init Snowflake first with: snowflake.init_snowflake(machine_id: int, epoch: int, worker_bits: int, sequence_bits: int)")
```

### Comparing `sqlx-batis-0.0.7/sqlbatis/sql_holder.py` & `sqlx-batis-0.0.8/sqlbatis/sql_holder.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.0.7/sqlbatis/sql_mapper.py` & `sqlx-batis-0.0.8/sqlbatis/sql_mapper.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.0.7/sqlbatis/sql_support.py` & `sqlx-batis-0.0.8/sqlbatis/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.0.7/sqlx_batis.egg-info/PKG-INFO` & `sqlx-batis-0.0.8/sqlx_batis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 0.0.7
+Version: 0.0.8
 Summary: sqlx-batis is a sql executor for Python like MyBatis.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
@@ -39,17 +39,16 @@
    </mapper>
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
-   from sqlbatis import dbx, Engin
    from typing import List, Tuple, Mapping
-   from sqlbatis.sql_mapper import mapper, sql
+   from sqlbatis import mapper, sql, dbx, Engin, init_db
 
    @mapper(namespace='person')
    def select_all(): List
 
    @mapper(namespace='person')
    def select_by_name(name: str): List
```

