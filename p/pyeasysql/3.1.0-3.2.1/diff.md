# Comparing `tmp/PyEasySQL-3.1.0.tar.gz` & `tmp/pyeasysql-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyEasySQL-3.1.0.tar", last modified: Sun Jul 23 11:46:01 2023, max compression
+gzip compressed data, was "pyeasysql-3.2.1.tar", last modified: Tue Jul 25 17:57:27 2023, max compression
```

## Comparing `PyEasySQL-3.1.0.tar` & `pyeasysql-3.2.1.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 11:46:01.298695 PyEasySQL-3.1.0/
-drwxrwxrwx   0        0        0        0 2023-07-23 11:46:01.270209 PyEasySQL-3.1.0/EasySQL/
--rw-rw-rw-   0        0        0     3607 2023-07-23 11:44:26.000000 PyEasySQL-3.1.0/EasySQL/ABC.py
--rw-rw-rw-   0        0        0     2887 2021-06-27 12:24:21.000000 PyEasySQL-3.1.0/EasySQL/Characters.py
--rw-rw-rw-   0        0        0    14303 2023-07-23 11:41:39.000000 PyEasySQL-3.1.0/EasySQL/Classes.py
--rw-rw-rw-   0        0        0     5764 2023-07-18 13:18:56.000000 PyEasySQL-3.1.0/EasySQL/Commands.py
--rw-rw-rw-   0        0        0      305 2023-07-11 12:44:34.000000 PyEasySQL-3.1.0/EasySQL/Decorators.py
--rw-rw-rw-   0        0        0     2097 2023-07-09 09:35:55.000000 PyEasySQL-3.1.0/EasySQL/EasyInstances.py
--rw-rw-rw-   0        0        0      757 2023-06-08 19:41:42.000000 PyEasySQL-3.1.0/EasySQL/Exceptions.py
--rw-rw-rw-   0        0        0      457 2021-04-04 16:17:30.000000 PyEasySQL-3.1.0/EasySQL/Logging.py
--rw-rw-rw-   0        0        0      161 2023-07-23 11:44:26.000000 PyEasySQL-3.1.0/EasySQL/Tags.py
--rw-rw-rw-   0        0        0     3079 2023-07-23 11:44:26.000000 PyEasySQL-3.1.0/EasySQL/Types.py
--rw-rw-rw-   0        0        0     2496 2022-04-15 06:15:51.000000 PyEasySQL-3.1.0/EasySQL/Where.py
--rw-rw-rw-   0        0        0      290 2023-07-09 11:50:43.000000 PyEasySQL-3.1.0/EasySQL/__init__.py
--rw-rw-rw-   0        0        0     6499 2023-07-23 11:46:01.297657 PyEasySQL-3.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-23 11:46:01.293043 PyEasySQL-3.1.0/PyEasySQL.egg-info/
--rw-rw-rw-   0        0        0     6499 2023-07-23 11:46:00.000000 PyEasySQL-3.1.0/PyEasySQL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2023-07-23 11:46:00.000000 PyEasySQL-3.1.0/PyEasySQL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 11:46:00.000000 PyEasySQL-3.1.0/PyEasySQL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-23 11:46:00.000000 PyEasySQL-3.1.0/PyEasySQL.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-23 11:46:00.000000 PyEasySQL-3.1.0/PyEasySQL.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5119 2023-07-09 10:37:27.000000 PyEasySQL-3.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-23 11:46:01.299682 PyEasySQL-3.1.0/setup.cfg
--rw-rw-rw-   0        0        0      859 2023-07-23 11:15:02.000000 PyEasySQL-3.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 17:57:27.567480 pyeasysql-3.2.1/
+drwxrwxrwx   0        0        0        0 2023-07-25 17:57:27.556295 pyeasysql-3.2.1/EasySQL/
+-rw-rw-rw-   0        0        0     3662 2023-07-24 11:39:55.000000 pyeasysql-3.2.1/EasySQL/ABC.py
+-rw-rw-rw-   0        0        0     2887 2021-06-27 12:24:21.000000 pyeasysql-3.2.1/EasySQL/Characters.py
+-rw-rw-rw-   0        0        0    15044 2023-07-25 08:56:23.000000 pyeasysql-3.2.1/EasySQL/Classes.py
+-rw-rw-rw-   0        0        0     6202 2023-07-25 17:49:13.000000 pyeasysql-3.2.1/EasySQL/Commands.py
+-rw-rw-rw-   0        0        0      945 2023-07-25 08:49:05.000000 pyeasysql-3.2.1/EasySQL/Constraints.py
+-rw-rw-rw-   0        0        0      305 2023-07-11 12:44:34.000000 pyeasysql-3.2.1/EasySQL/Decorators.py
+-rw-rw-rw-   0        0        0     2097 2023-07-09 09:35:55.000000 pyeasysql-3.2.1/EasySQL/EasyInstances.py
+-rw-rw-rw-   0        0        0      757 2023-06-08 19:41:42.000000 pyeasysql-3.2.1/EasySQL/Exceptions.py
+-rw-rw-rw-   0        0        0      457 2021-04-04 16:17:30.000000 pyeasysql-3.2.1/EasySQL/Logging.py
+-rw-rw-rw-   0        0        0     3079 2023-07-23 11:44:26.000000 pyeasysql-3.2.1/EasySQL/Types.py
+-rw-rw-rw-   0        0        0     2496 2022-04-15 06:15:51.000000 pyeasysql-3.2.1/EasySQL/Where.py
+-rw-rw-rw-   0        0        0      298 2023-07-24 15:21:11.000000 pyeasysql-3.2.1/EasySQL/__init__.py
+-rw-rw-rw-   0        0        0     1085 2023-07-23 15:33:54.000000 pyeasysql-3.2.1/LICENSE.md
+-rw-rw-rw-   0        0        0     6084 2023-07-25 17:57:27.566483 pyeasysql-3.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5412 2023-07-24 15:30:12.000000 pyeasysql-3.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 17:57:27.564489 pyeasysql-3.2.1/pyeasysql.egg-info/
+-rw-rw-rw-   0        0        0     6084 2023-07-25 17:57:27.000000 pyeasysql-3.2.1/pyeasysql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      449 2023-07-25 17:57:27.000000 pyeasysql-3.2.1/pyeasysql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 17:57:27.000000 pyeasysql-3.2.1/pyeasysql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-25 17:57:27.000000 pyeasysql-3.2.1/pyeasysql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-25 17:57:27.000000 pyeasysql-3.2.1/pyeasysql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      717 2023-07-25 17:57:19.000000 pyeasysql-3.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-25 17:57:27.567480 pyeasysql-3.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      831 2023-07-24 16:25:04.000000 pyeasysql-3.2.1/setup.py
```

### Comparing `PyEasySQL-3.1.0/EasySQL/ABC.py` & `pyeasysql-3.2.1/EasySQL/ABC.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC
 from typing import Callable, Any, Iterable
 
-__all__ = ['SQLType', 'SQLTag', 'SQLCommand', 'SQLCommandExecutable', 'SQLExecutable',
+__all__ = ['SQLType', 'SQLConstraints', 'SQLCommand', 'SQLCommandExecutable', 'SQLExecutable',
            'CHARSET', 'make_collection', 'is_collection']
 
 
 class SQLType:
     def __init__(self, name, *args, caster: Callable[[Any], Any] = None, get_caster: Callable[["SQLType"], Callable[[Any], Any]] = None, default: Any = None, parser: Callable[[Any], str] = None, modifiable: bool = False, tags: Iterable[str] = None):
         self._name = name
         self._args = args
@@ -72,17 +72,18 @@
         return self._args
 
     @property
     def modifiable(self):
         return self._modifiable
 
 
-class SQLTag:
+class SQLConstraints:
     def __init__(self, value):
         self.value = value
+        self.column_constraint = True
 
 
 class CHARSET:
     def __init__(self, name, collation, maxlen=1, description=None):
         self._name = name
         self.__doc__ = description
         self._collation = collation
```

### Comparing `PyEasySQL-3.1.0/EasySQL/Characters.py` & `pyeasysql-3.2.1/EasySQL/Characters.py`

 * *Files identical despite different names*

### Comparing `PyEasySQL-3.1.0/EasySQL/Classes.py` & `pyeasysql-3.2.1/EasySQL/Classes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from itertools import zip_longest
 from time import sleep
 from typing import Optional, Union, Any, Sequence, TypeVar, Tuple, List
 
 import mysql.connector
+from deprecated.classic import deprecated
 
-from .ABC import SQLType, CHARSET, SQLTag
+from .ABC import SQLType, CHARSET, SQLConstraints
 from .Exceptions import DatabaseConnectionException
 from .Logging import logger
-from .Tags import NOT_NULL, PRIMARY
+from .Constraints import NOT_NULL, Unique, UNIQUE, PRIMARY
 from .Where import Where
 
 __all__ = ['EasyDatabase', 'EasyTable', 'EasyColumn', 'EasyForeignColumn']
 
 
 def _safe_pop(d: dict, k):
     try:
@@ -29,23 +30,23 @@
         return f'{i}nd'
     if i % 10 == 3:
         return f'{i}rd'
     return f'{i}th'
 
 
 class EasyColumn:
-    def __init__(self, name: str, sql_type: SQLType, *tags: SQLTag, default: Any = None, order: int = None):
+    def __init__(self, name: str, sql_type: SQLType, *tags: SQLConstraints, default: Any = None, order: int = None):
         self.name = name
         self.sql_type = sql_type
         self.tags = tags
-        self.default = default if default else sql_type.default if NOT_NULL in self.tags or PRIMARY in self.tags else None
+        self.default = default if default else sql_type.default if NOT_NULL in self.tags else None
         self.order = order
 
-        if PRIMARY in self.tags and NOT_NULL in self.tags:
-            self.tags = (tag for tag in self.tags if tag != NOT_NULL)
+        # if PRIMARY in self.tags and NOT_NULL in self.tags:
+        #    self.tags = (tag for tag in self.tags if tag != NOT_NULL)
 
         self.table = None
 
     def set_table(self, table):
         self.table = table
 
     def __hash__(self):
@@ -75,23 +76,23 @@
 
     def cast(self, value):
         return self.sql_type.cast(value)
 
 
 class EasyForeignColumn(EasyColumn):
     @staticmethod
-    def of(column: EasyColumn, name: str = None, *tags: SQLTag, default: Any = None):
+    def of(column: EasyColumn, name: str = None, *tags: SQLConstraints, default: Any = None):
         if not isinstance(column.table, EasyTable):
             return TypeError('Version 3: To use this method, The table of column must be set')
 
         tags = (NOT_NULL, ) if NOT_NULL in tags else ()
         name = f'{column.name} of {column.table.name}' if name is None else name
         return EasyForeignColumn(name, column.table, column, *tags, default=default)
 
-    def __init__(self, name: str, table: 'EasyTable', reference: Union[EasyColumn, str], *tags: SQLTag, default: Any = None):
+    def __init__(self, name: str, table: 'EasyTable', reference: Union[EasyColumn, str], *tags: SQLConstraints, default: Any = None):
         column = table.get_column(reference)
         if column is None:
             raise ValueError(f'Unable to find `{reference}` in the table')
 
         self.refer_table = table
         self.refer_column = column
 
@@ -211,18 +212,19 @@
         columns = []
         for column in result:
             sqltype = string_to_type(column[1])
             if sqltype is None:
                 raise TypeError(f'Unable to recognize name "{column[1]}" as a SQLType')
 
             tags = []
+            prim = []
             if column[2] == 'NO':
                 tags.append(NOT_NULL)
             if column[3] == 'PRI':
-                tags.append(PRIMARY)
+                prim.append(column[0])
 
             columns.append(EasyColumn(column[0], sqltype, *tags, default=column[4]))
 
         return tuple(columns)
 
     def set_charset(self, charset: CHARSET):
         if charset is not None:
@@ -250,20 +252,30 @@
 
 
 class EasyTable:
     _database: EasyDatabase = NotImplemented
     _name: str = NotImplemented
     _columns: tuple = ()
 
+    PRIMARY: List[EasyColumn] = []
+    UNIQUES: List[Unique] = []
+
     def __init_subclass__(cls, **kwargs):
         for key in ('database', 'name'):
             setattr(cls, f'_{key}', _safe_pop(kwargs, key) or getattr(cls, f'_{key}'))
 
         columns: List[EasyColumn] = [value for value in cls.__dict__.values() if isinstance(value, EasyColumn)]
-        columns.sort(key=lambda col: col.order if col.order is not None else id(cls))
+        for column in columns:
+            if UNIQUE in column.tags:
+                cls.UNIQUES.append(Unique(column))
+            if PRIMARY in column.tags:
+                cls.PRIMARY.append(column)
+
+            column.tags = tuple([tag for tag in column.tags if tag != UNIQUE and tag != PRIMARY])
+
         cls._columns: Tuple[EasyColumn] = tuple(columns)
 
     def __init__(self, auto_prepare: bool = True, *, _force=False):
         if type(self) == EasyTable and not _force:
             raise TypeError('Version 3: Unable to instance \'EasyTable\' directly, Create a subclass')
         
         if not isinstance(self._database, EasyDatabase):
@@ -286,15 +298,22 @@
         return tuple(self.get_column(column, force=True) for column in columns)
 
     def prepare(self, alter_columns=True):
         command = f'SHOW TABLES FROM {self._database.name} WHERE Tables_in_{self._database.name} = \'{self._name}\';'
         exists = bool(self._database.execute(command, buffered=True).fetchall())
         if not exists:
             if self._columns:
-                command = f"CREATE TABLE IF NOT EXISTS {self._name} ({', '.join([column.get_sql() for column in self._columns])});"
+                command = ', '.join([column.get_sql() for column in self._columns])
+                if len(self.PRIMARY) > 0:
+                    command += f", PRIMARY KEY({', '.join(column.name for column in self.PRIMARY)})"
+
+                for unique in self.UNIQUES:
+                    command += f", {unique.value}"
+
+                command = f"CREATE TABLE {self._name} ({command});"
                 self._database.execute(command)
             else:
                 raise ValueError('No columns where specified and table does not exist')
         else:
             columns = self._database.describe_table(self)
             if self._columns is None or len(self._columns) == 0:
                 self._columns = columns
@@ -302,15 +321,15 @@
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
 
@@ -345,19 +364,19 @@
 
     def select(self, columns: SOS_ECOS = None, where: Where = None, limit: int = None, offset: int = None, order: SOS_ECOS = None, descending: bool = False, force_one=False):
         from .Commands import Select
 
         assert self.prepared, 'Unable to perform action before preparing the table'
         return Select(self._database, self, self.assert_columns(columns) if columns is not None else None, where, limit, offset, self.assert_columns(order), descending, force_one).execute()
 
-    def insert(self, columns: SOS_ECOS, values: SOS[Any]):
+    def insert(self, columns: SOS_ECOS, values: SOS[Any], update_on_dup: bool = False):
         from .Commands import Insert
 
         assert self.prepared, 'Unable to perform action before preparing the table'
-        return Insert(self._database, self, self.assert_columns(columns) if columns is not None else self._columns, values).execute()
+        return Insert(self._database, self, self.assert_columns(columns) if columns is not None or columns == '*' else self._columns, values, update_on_dup).execute()
 
     def update(self, columns: SOS_ECOS, values: SOS[Any], where: Where = None):
         from .Commands import Update
 
         assert self.prepared, 'Unable to perform action before preparing the table'
         return Update(self._database, self, self.assert_columns(columns) if columns is not None else self._columns, values, where).execute()
```

### Comparing `PyEasySQL-3.1.0/EasySQL/Commands.py` & `pyeasysql-3.2.1/EasySQL/Commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,27 +84,39 @@
         if self._force_one:
             return None if len(new_result) == 0 else new_result[0]
 
         return EmptySelectData(self._table) if len(new_result) == 0 else new_result[0] if len(new_result) == 1 else new_result
 
 
 class Insert(SQLCommandExecutable):
-    def __init__(self, database: EasyDatabase, table: EasyTable, columns: Sequence[EasyColumn], values: Sequence[Any]):
+    def __init__(self, database: EasyDatabase, table: EasyTable, columns: Sequence[EasyColumn], values: Sequence[Any], on_dup_update: bool = True):
+        if columns == '*' or columns is None:
+            columns = table.columns
+
+        table.assert_columns(columns)
+        if len(columns) != len(values):
+            raise ValueError('Values length do not match with the columns of the table')
+
         self._database = database
+        self._values = list(zip(table.columns, values))
         self._columns = columns
-        self._values = values
         self._table = table
-
-        if len(self._columns) != len(self._values):
-            raise ValueError('Values length do not match with the columns')
+        self._update = on_dup_update
 
     def get_value(self) -> str:
         columns = ', '.join([column.name for column in self._columns])
-        values = ', '.join([column.parse(value) for column, value in zip(self._columns, self._values)])
-        return f"INSERT INTO {self._table.name} ({columns}) VALUES ({values});"
+        values = ', '.join([column.parse(value) for column, value in self._values])
+
+        if self._update:
+            extra = ', '.join([f"{column.name}={column.parse(value)}" for column, value in self._values])
+            extra = f" ON DUPLICATE KEY UPDATE {extra}"
+        else:
+            extra = ""
+
+        return f"INSERT INTO {self._table.name} ({columns}) VALUES ({values}){extra};"
 
     def execute(self):
         return self._database.execute(self.get_value(), buffered=True).lastrowid
 
 
 # noinspection SqlWithoutWhere
 # The asserts will not allow the missing where
```

### Comparing `PyEasySQL-3.1.0/EasySQL/EasyInstances.py` & `pyeasysql-3.2.1/EasySQL/EasyInstances.py`

 * *Files identical despite different names*

### Comparing `PyEasySQL-3.1.0/EasySQL/Exceptions.py` & `pyeasysql-3.2.1/EasySQL/Exceptions.py`

 * *Files identical despite different names*

### Comparing `PyEasySQL-3.1.0/EasySQL/Types.py` & `pyeasysql-3.2.1/EasySQL/Types.py`

 * *Files identical despite different names*

### Comparing `PyEasySQL-3.1.0/EasySQL/Where.py` & `pyeasysql-3.2.1/EasySQL/Where.py`

 * *Files identical despite different names*

### Comparing `PyEasySQL-3.1.0/PKG-INFO` & `pyeasysql-3.2.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,120 +1,116 @@
-Metadata-Version: 2.1
-Name: PyEasySQL
-Version: 3.1.0
-Summary: SQL Database management without even a SQL line
-Home-page: https://github.com/ashenguard/easysql
-Author: Ashenguard
-Author-email: Ashenguard@agmdev.xyz
-License: MIT License
-Description: # EasySQL
-        ![Downloads](https://pepy.tech/badge/pyeasysql)
-        ![Downloads](https://pepy.tech/badge/pyeasysql/week)
-        ![Downloads](https://pepy.tech/badge/pyeasysql/month)  
-        This library allow you to run SQL Databases without knowing even SQL.  
-        This library will create SQL queries and execute them as you request and is very simple to use.
-        
-        ### Having an issue?
-        You can always find someone on our discord server here:
-        > https://discord.gg/6exsySK
-        
-        ### Wiki
-        The official wiki of this library is now available at GitHub
-        > https://github.com/Ashenguard/EasySQL/wiki
-        
-        ## How to install
-        ![](https://img.shields.io/github/v/release/Ashengaurd/EasySQL?label=Release&logo=github&style=plastic)
-        ![](https://img.shields.io/github/last-commit/Ashengaurd/EasySQL/master?label=Date&logo=git&logoColor=blue&style=plastic)  
-        ![](https://img.shields.io/github/v/release/Ashengaurd/EasySQL?include_prereleases&label=Development&logo=github&style=plastic)
-        ![](https://img.shields.io/github/last-commit/Ashengaurd/EasySQL?label=Date&logo=git&logoColor=red&style=plastic)  
-        To install just use following command
-        ```shell
-        pip install PyEasySQL
-        ```
-        This library will have dev/beta builds on the GitHub, to install them you can use
-        
-        ```shell
-        pip install --upgrade git+https://github.com/Ashenguard/EasySQL.git
-        ```
-        ***
-        By installing this library following libraries and their dependencies will be installed too.
-        ```yaml
-        mysql-connector: Which is the basic library for connecting to database
-        ```
-        # Example
-        
-        ```python
-        import EasySQL
-        
-        # Simply provide connection info to your database
-        @EasySQL.auto_init
-        class MyDatabase(EasySQL.EasyDatabase):
-            _database = 'MyDatabase'
-            _password = '**********'
-            _host = '127.0.0.1'
-            _port = 3306
-            _user = 'root'
-        
-        # Simply create a MyTable with its columns!
-        @EasySQL.auto_init
-        class MyTable(EasySQL.EasyTable, database=MyDatabase, name='MyTable'):
-            ID = EasySQL.EasyColumn('ID', EasySQL.Types.BIGINT, EasySQL.Tags.PRIMARY, EasySQL.Tags.AUTO_INCREMENT)
-            Name = EasySQL.EasyColumn('Name', EasySQL.Types.STRING(255), EasySQL.Tags.NOT_NULL, default='Missing')
-            Balance = EasySQL.EasyColumn('Balance', EasySQL.Types.INT, EasySQL.Tags.NOT_NULL)
-            Premium = EasySQL.EasyColumn('Premium', EasySQL.Types.BOOL, EasySQL.Tags.NOT_NULL, default=False)
-        
-        # Insert values with a simple command
-        MyTable.insert([MyTable.Name, MyTable.Premium, MyTable.Balance], ['Ashenguard', True, 10])
-        MyTable.insert([MyTable.Name, MyTable.Premium], ['Sam', False])
-        
-        # Let's add some random data 
-        from random import randint
-        for i in range(5):
-            MyTable.insert(['Name', 'Balance'], [f'User-{i}', randint(0, 20)])
-        
-        # Selecting data with another simple command
-        ### Let's get all the data
-        all = MyTable.select()
-        ### Something that does not exist
-        empty = MyTable.select(MyTable.ID, where=EasySQL.WhereIsEqual(MyTable.Name, "NO-ONE"))
-        ### To select multiple data give a list of columns as 1st argument
-        premiums = MyTable.select([MyTable.ID, MyTable.Name], EasySQL.WhereIsEqual(MyTable.Premium, True))
-        ### You can have more complicated condition with AND (&), OR (|) and NOT (~)
-        specific = MyTable.select(MyTable.Name, where=EasySQL.WhereIsLike(MyTable.Name, "Ash%").AND(EasySQL.WhereIsLesserEqual(MyTable.ID, 5)))
-        ### Giving no column will select all the columns, Also you can use limit, offset and order to sort data
-        second = MyTable.select(order=MyTable.Balance, descending=True, limit=1, offset=1)
-        top5 = MyTable.select(order=MyTable.Balance, descending=True, limit=5)
-        ### If you want only one result not a sequence of them! It will return a SelectData if a data is found or return None if none is found.
-        one = MyTable.select(where=EasySQL.WhereIsEqual(MyTable.Name, "Ashenguard"), force_one=True)
-        
-        # The result will be an EmptySelectData if nothing was found, A SelectData if only one was found, Or a tuple of SelectData
-        # All 3 of them are iterable, so it is safe to use a `for` loop for any result
-        # To get data from the result you can use `get`, but it only contains columns requested in select method.
-        for data in top5:
-            print(f'{data.get(MyTable.ID)}: {data.get(MyTable.Name)}\tBalance: {data.get(MyTable.Balance)}')
-        
-        # To delete data just use the delete method
-        MyTable.delete(EasySQL.WhereIsGreater(MyTable.ID, 5))
-        
-        # Update data with following command
-        MyTable.update(MyTable.Premium, True, EasySQL.WhereIsEqual(MyTable.ID, 3).OR(EasySQL.WhereIsEqual(MyTable.Name, 'Sam')))
-        
-        # Not sure if you should update or insert? Use set and it will be handled
-        MyTable.set([MyTable.ID, MyTable.Name, MyTable.Balance, MyTable.Premium], [5, 'Nathaniel', 50, False], where=EasySQL.WhereIsEqual(MyTable.ID, 5))
-        
-        # Safety error on delete/update/set without a where statement
-        # MyTable.delete() -> raise EasySQL.DatabaseSafetyException
-        # Turn the safety off with following command.
-        MyDatabase.remove_safety(confirm=True)
-        # Now there will be no error, it will clean the all data that's why we had safety lock
-        MyTable.delete()
-        ```
-        
-        [![AdFoc.us Banner](https://adfoc.us/images/banners/728x90-2.gif)](https://adfoc.us/?refid=497244)
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+# EasySQL
+![Downloads](https://pepy.tech/badge/pyeasysql)
+![Downloads](https://pepy.tech/badge/pyeasysql/week)
+![Downloads](https://pepy.tech/badge/pyeasysql/month)  
+This library allow you to run SQL Databases without knowing even SQL.  
+This library will create SQL queries and execute them as you request and is very simple to use.
+
+### This library is still under development, so we appreciate if you help us improve it on the GitHub!
+
+### Having an issue?
+You can always find someone on our discord server here:
+> https://discord.gg/6exsySK
+
+### Wiki
+The official wiki of this library is now available at GitHub
+> https://github.com/AGM-Studio/EasySQL/wiki
+
+## How to install
+To install just use following command
+```shell
+pip install PyEasySQL
+```
+This library will have dev/beta builds on the GitHub, to install them you can use
+
+```shell
+pip install --upgrade git+https://github.com/AGM-Studio/EasySQL.git
+```
+***
+By installing this library following libraries and their dependencies will be installed too.
+```yaml
+mysql-connector: Which is the basic library for connecting to database
+```
+# Example
+
+```python
+import EasySQL
+
+# Simply provide connection info to your database
+@EasySQL.auto_init
+class MyDatabase(EasySQL.EasyDatabase):
+    _database = 'MyDatabase'
+    _password = '**********'
+    _host = '127.0.0.1'
+    _port = 3306
+    _user = 'root'
+
+# Simply create a MyTable with its columns!
+@EasySQL.auto_init
+class MyTable(EasySQL.EasyTable, database=MyDatabase, name='MyTable'):
+    ID = EasySQL.EasyColumn('ID', EasySQL.Types.BIGINT, EasySQL.PRIMARY, EasySQL.AUTO_INCREMENT)
+    Name = EasySQL.EasyColumn('Name', EasySQL.Types.STRING(255), EasySQL.NOT_NULL, default='Missing')
+    Balance = EasySQL.EasyColumn('Balance', EasySQL.Types.INT, EasySQL.NOT_NULL)
+    Premium = EasySQL.EasyColumn('Premium', EasySQL.Types.BOOL, EasySQL.NOT_NULL, default=False)
+
+# Insert values with a simple command
+MyTable.insert([MyTable.Name, MyTable.Premium, MyTable.Balance], ['Ashenguard', True, 10])
+MyTable.insert([MyTable.Name, MyTable.Premium], ['Sam', False])
+
+# Let's add some random data 
+from random import randint
+for i in range(5):
+    MyTable.insert(['Name', 'Balance'], [f'User-{i}', randint(0, 20)])
+
+# Selecting data with another simple command
+### Let's get all the data
+all = MyTable.select()
+### Something that does not exist
+empty = MyTable.select(MyTable.ID, where=EasySQL.WhereIsEqual(MyTable.Name, "NO-ONE"))
+### To select multiple data give a list of columns as 1st argument
+premiums = MyTable.select([MyTable.ID, MyTable.Name], EasySQL.WhereIsEqual(MyTable.Premium, True))
+### You can have more complicated condition with AND (&), OR (|) and NOT (~)
+specific = MyTable.select(MyTable.Name, where=EasySQL.WhereIsLike(MyTable.Name, "Ash%").AND(EasySQL.WhereIsLesserEqual(MyTable.ID, 5)))
+### Giving no column will select all the columns, Also you can use limit, offset and order to sort data
+second = MyTable.select(order=MyTable.Balance, descending=True, limit=1, offset=1)
+top5 = MyTable.select(order=MyTable.Balance, descending=True, limit=5)
+### If you want only one result not a sequence of them! It will return a SelectData if a data is found or return None if none is found.
+one = MyTable.select(where=EasySQL.WhereIsEqual(MyTable.Name, "Ashenguard"), force_one=True)
+
+# The result will be an EmptySelectData if nothing was found, A SelectData if only one was found, Or a tuple of SelectData
+# All 3 of them are iterable, so it is safe to use a `for` loop for any result
+# To get data from the result you can use `get`, but it only contains columns requested in select method.
+for data in top5:
+    print(f'{data.get(MyTable.ID)}: {data.get(MyTable.Name)}\tBalance: {data.get(MyTable.Balance)}')
+
+# To delete data just use the delete method
+MyTable.delete(EasySQL.WhereIsGreater(MyTable.ID, 5))
+
+# Update data with following command
+MyTable.update(MyTable.Premium, True, EasySQL.WhereIsEqual(MyTable.ID, 3).OR(EasySQL.WhereIsEqual(MyTable.Name, 'Sam')))
+
+# Not sure if you should update or insert and don't have primary or unique keys? Use set and it will be handled
+MyTable.set(MyTable.columns, [6, 'Nathaniel', 50, False], where=EasySQL.WhereIsEqual(MyTable.ID, 5))
+
+# And if you have unique and primary keys set let insert handle duplicates for you
+MyTable.insert(MyTable.columns, [3, 'Jack', 5000, False], update_on_dup=True)
+
+# Safety error on delete/update/set without a where statement
+# MyTable.delete() -> raise EasySQL.DatabaseSafetyException
+# Turn the safety off with following command.
+MyDatabase.remove_safety(confirm=True)
+# Now there will be no error, it will clean the all data that's why we had safety lock
+MyTable.delete()
+```
+
+[![AdFoc.us Banner](https://adfoc.us/images/banners/728x90-2.gif)](https://adfoc.us/?refid=497244)
+
+## Extras & Features
+1. Need unsigned types? EasySQL has them.
+> `BIGINT.UNSIGNED`, `INT.UNSIGNED`, `MEDIUMINT.UNSIGNED`, `SMALLINT.UNSIGNED`
+2. Afraid of unsigned or signed values? EasySQL will check them for you!
+> Raises `ValueError` if you are out of bound
+3. Multiple primary keys? EasySQL will take care of it.
+> Tag them with `PRIMARY` or add them to `YourTableClass.PRIMARY`
+4. Want to mark multiple columns as unique together? EasySQL have it.
+> Add `Unique(column_1, column_2)` to `YourTableClass.UNIQUES`
+5.
```

