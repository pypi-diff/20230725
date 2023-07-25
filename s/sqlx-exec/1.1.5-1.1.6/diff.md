# Comparing `tmp/sqlx-exec-1.1.5.tar.gz` & `tmp/sqlx-exec-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-exec-1.1.5.tar", last modified: Mon Jul 24 01:44:11 2023, max compression
+gzip compressed data, was "dist\sqlx-exec-1.1.6.tar", last modified: Tue Jul 25 08:25:34 2023, max compression
```

## Comparing `sqlx-exec-1.1.5.tar` & `sqlx-exec-1.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 01:44:11.000000 sqlx-exec-1.1.5/
--rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.1.5/LICENSE
--rw-rw-rw-   0        0        0     2701 2023-07-24 01:44:11.000000 sqlx-exec-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2159 2023-07-22 02:28:05.000000 sqlx-exec-1.1.5/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-24 01:44:11.000000 sqlx-exec-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1195 2023-07-23 13:20:12.000000 sqlx-exec-1.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:44:11.000000 sqlx-exec-1.1.5/sqlexec/
--rw-rw-rw-   0        0        0      529 2023-07-23 08:55:03.000000 sqlx-exec-1.1.5/sqlexec/constant.py
--rw-rw-rw-   0        0        0     4272 2023-07-23 23:54:10.000000 sqlx-exec-1.1.5/sqlexec/engin.py
--rw-rw-rw-   0        0        0    11712 2023-07-23 22:50:17.000000 sqlx-exec-1.1.5/sqlexec/exec.py
--rw-rw-rw-   0        0        0     1030 2023-07-21 22:35:47.000000 sqlx-exec-1.1.5/sqlexec/log_support.py
--rw-rw-rw-   0        0        0      629 2023-07-23 22:45:17.000000 sqlx-exec-1.1.5/sqlexec/pooling.py
--rw-rw-rw-   0        0        0     1556 2023-07-23 13:53:53.000000 sqlx-exec-1.1.5/sqlexec/sql_support.py
--rw-rw-rw-   0        0        0     4275 2023-07-23 09:51:27.000000 sqlx-exec-1.1.5/sqlexec/support.py
--rw-rw-rw-   0        0        0      389 2023-07-23 13:53:53.000000 sqlx-exec-1.1.5/sqlexec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:44:11.000000 sqlx-exec-1.1.5/sqlx_exec.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-24 01:44:11.000000 sqlx-exec-1.1.5/sqlx_exec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-23 13:22:36.000000 sqlx-exec-1.1.5/sqlx_exec.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2701 2023-07-24 01:44:11.000000 sqlx-exec-1.1.5/sqlx_exec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-07-24 01:44:11.000000 sqlx-exec-1.1.5/sqlx_exec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-07-24 01:44:11.000000 sqlx-exec-1.1.5/sqlx_exec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 08:25:34.000000 sqlx-exec-1.1.6/
+-rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.1.6/LICENSE
+-rw-rw-rw-   0        0        0     2701 2023-07-25 08:25:34.000000 sqlx-exec-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2159 2023-07-22 02:28:05.000000 sqlx-exec-1.1.6/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-25 08:25:34.000000 sqlx-exec-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1195 2023-07-25 08:25:10.000000 sqlx-exec-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:25:34.000000 sqlx-exec-1.1.6/sqlexec/
+-rw-rw-rw-   0        0        0      529 2023-07-23 08:55:03.000000 sqlx-exec-1.1.6/sqlexec/constant.py
+-rw-rw-rw-   0        0        0     4615 2023-07-25 07:49:14.000000 sqlx-exec-1.1.6/sqlexec/engin.py
+-rw-rw-rw-   0        0        0    11712 2023-07-25 05:43:20.000000 sqlx-exec-1.1.6/sqlexec/exec.py
+-rw-rw-rw-   0        0        0     1030 2023-07-21 22:35:47.000000 sqlx-exec-1.1.6/sqlexec/log_support.py
+-rw-rw-rw-   0        0        0      629 2023-07-23 22:45:17.000000 sqlx-exec-1.1.6/sqlexec/pooling.py
+-rw-rw-rw-   0        0        0     1556 2023-07-23 13:53:53.000000 sqlx-exec-1.1.6/sqlexec/sql_support.py
+-rw-rw-rw-   0        0        0     4275 2023-07-23 09:51:27.000000 sqlx-exec-1.1.6/sqlexec/support.py
+-rw-rw-rw-   0        0        0      389 2023-07-23 13:53:53.000000 sqlx-exec-1.1.6/sqlexec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:25:34.000000 sqlx-exec-1.1.6/sqlx_exec.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-25 08:25:34.000000 sqlx-exec-1.1.6/sqlx_exec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-23 13:22:36.000000 sqlx-exec-1.1.6/sqlx_exec.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2701 2023-07-25 08:25:34.000000 sqlx-exec-1.1.6/sqlx_exec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-07-25 08:25:34.000000 sqlx-exec-1.1.6/sqlx_exec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-07-25 08:25:34.000000 sqlx-exec-1.1.6/sqlx_exec.egg-info/top_level.txt
```

### Comparing `sqlx-exec-1.1.5/LICENSE` & `sqlx-exec-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.1.5/PKG-INFO` & `sqlx-exec-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.1.5
+Version: 1.1.6
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction. Now support MySQL and PostgreSQL.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,python
 Platform: UNKNOWN
```

### Comparing `sqlx-exec-1.1.5/README.rst` & `sqlx-exec-1.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.1.5/setup.py` & `sqlx-exec-1.1.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 setup(
     name='sqlx-exec',
     packages=['sqlexec'],
     description="sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction. Now support MySQL and PostgreSQL.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.1.5',
+    version='1.1.6',
     url='https://gitee.com/summry/sql-exec',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-exec-1.1.5/sqlexec/constant.py` & `sqlx-exec-1.1.6/sqlexec/constant.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.1.5/sqlexec/engin.py` & `sqlx-exec-1.1.6/sqlexec/engin.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,59 +4,58 @@
 from .support import DBError
 from functools import lru_cache
 from .log_support import logger
 from .constant import CACHE_SIZE, MYSQL_COLUMN_SQL, POSTGRES_COLUMN_SQL
 
 _ENGIN = None
 _DB_ENGIN = None
+# Engin = Enum('Engin', ['MYSQL', 'POSTGRESQL', 'OTHER'])
 
 
 class Engin(Enum):
     MYSQL = 'MySQL'
     POSTGRESQL = 'PostgreSQL'
-    OTHER = 'other'
+    OTHER = 'Other'
 
     @staticmethod
     def current_engin():
         global _ENGIN
         return _ENGIN
 
 
 class DBEngin:
     before_execute = None
-    before_execute = None
-    before_execute = None
-    before_execute = None
-    before_execute = None
+    page_sql_args = None
+    create_insert_sql = None
+    get_select_key = None
+    get_column_sql = None
+
+    def __init__(self, show_sql):
+        self.show_sql = show_sql
 
     @classmethod
     def init_db_engin(cls, engin, show_sql):
         global _ENGIN
         global _DB_ENGIN
         _ENGIN = engin
         if engin == Engin.MYSQL:
             _DB_ENGIN = MySqlEngin(show_sql)
         elif engin == Engin.POSTGRESQL:
             _DB_ENGIN = PostgresEngin(show_sql)
         elif engin == Engin.OTHER:
-            _DB_ENGIN = BaseEngin(show_sql)
+            _DB_ENGIN = DBEngin(show_sql)
         else:
             raise DBError("Unknown engin type: {}".format(engin))
 
         cls.before_execute = _DB_ENGIN.before_execute
         cls.page_sql_args = _DB_ENGIN.page_sql_args
         cls.create_insert_sql = _DB_ENGIN.create_insert_sql
         cls.get_select_key = _DB_ENGIN.get_select_key
         cls.get_column_sql = _DB_ENGIN.get_column_sql
 
-
-class BaseEngin:
-    def __init__(self, show_sql):
-        self.show_sql = show_sql
-
     def before_execute(self, function: str, sql: str, *args):
         if self.show_sql:
             logger.info("Exec func 'sqlexec.%s' \n\tSQL: %s \n\tARGS: %s" % (function, sql, args))
         if '%' in sql and 'like' in sql.lower():
             sql = sql.replace('%', '%%').replace('%%%%', '%%')
         return sql.replace('?', '%s')
 
@@ -75,20 +74,26 @@
         pass
 
     @staticmethod
     def get_column_sql():
         pass
 
 
-class MySqlEngin(BaseEngin):
+class MySqlEngin(DBEngin):
 
     def __init__(self, show_sql):
         super().__init__(show_sql)
 
     @staticmethod
+    @lru_cache(maxsize=CACHE_SIZE)
+    def create_insert_sql(table: str, cols: Sequence[str]):
+        columns, placeholders = zip(*[('`{}`'.format(col), '?') for col in cols])
+        return 'INSERT INTO `{}`({}) VALUES({})'.format(table, ','.join(columns), ','.join(placeholders))
+
+    @staticmethod
     def page_sql_args(require_limit, sql: str, start, page_size, *args):
         if require_limit(sql):
             sql = '{} limit ?, ?'.format(sql)
         args = [*args, start, page_size]
         return sql, args
 
     @staticmethod
@@ -96,15 +101,15 @@
         return "SELECT LAST_INSERT_ID()"
 
     @staticmethod
     def get_column_sql():
         return MYSQL_COLUMN_SQL
 
 
-class PostgresEngin(BaseEngin):
+class PostgresEngin(DBEngin):
 
     def __init__(self, show_sql):
         super().__init__(show_sql)
 
 
     @staticmethod
     def page_sql_args(require_limit, sql: str, start, page_size, *args):
```

### Comparing `sqlx-exec-1.1.5/sqlexec/exec.py` & `sqlx-exec-1.1.6/sqlexec/exec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import functools
 import importlib
-from .engin import Engin, DBEngin
 from . import sql_support
+from .engin import Engin, DBEngin
 from .constant import MAPPER_PATH, DRIVER
 from .log_support import logger, insert_log, save_log, get_log, page_log
 from .support import DBCtx, ConnectionCtx, Dict, MultiColumnsError, TransactionCtx, try_commit, DBError, DB_LOCK
 
 _DB_CTX = None
 
 
-def init_db(connect=None, user='root', password='', database='test', host='127.0.0.1', port=3306, engin=Engin.MYSQL, pool_size=0, show_sql=False, **kwargs):
+def init_db(connect=None, host='127.0.0.1', port=3306, database='test', user='root', password='', engin=Engin.MYSQL, pool_size=0, show_sql=False, **kwargs):
     DBEngin.init_db_engin(engin, show_sql)
     _del_kwarg(MAPPER_PATH, kwargs)
     driver = kwargs.pop(DRIVER) if DRIVER in kwargs else None
     if 'debug' in kwargs:
         if kwargs.pop('debug'):
             from logging import DEBUG
             logger.setLevel(DEBUG)
```

### Comparing `sqlx-exec-1.1.5/sqlexec/log_support.py` & `sqlx-exec-1.1.6/sqlexec/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.1.5/sqlexec/pooling.py` & `sqlx-exec-1.1.6/sqlexec/pooling.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.1.5/sqlexec/sql_support.py` & `sqlx-exec-1.1.6/sqlexec/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.1.5/sqlexec/support.py` & `sqlx-exec-1.1.6/sqlexec/support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.1.5/sqlx_exec.egg-info/PKG-INFO` & `sqlx-exec-1.1.6/sqlx_exec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.1.5
+Version: 1.1.6
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction. Now support MySQL and PostgreSQL.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,python
 Platform: UNKNOWN
```

