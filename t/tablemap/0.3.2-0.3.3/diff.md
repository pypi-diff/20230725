# Comparing `tmp/tablemap-0.3.2.tar.gz` & `tmp/tablemap-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablemap-0.3.2.tar", last modified: Mon Jul 24 02:49:24 2023, max compression
+gzip compressed data, was "tablemap-0.3.3.tar", last modified: Tue Jul 25 06:54:03 2023, max compression
```

## Comparing `tablemap-0.3.2.tar` & `tablemap-0.3.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 02:49:24.866884 tablemap-0.3.2/
--rw-rw-rw-   0        0        0     1085 2023-03-22 11:37:34.000000 tablemap-0.3.2/LICENSE
--rw-rw-rw-   0        0        0      229 2023-07-24 02:49:24.865884 tablemap-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0    15613 2023-07-24 02:28:24.000000 tablemap-0.3.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-24 02:49:24.866884 tablemap-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0      340 2023-07-24 02:48:52.000000 tablemap-0.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 02:49:24.824881 tablemap-0.3.2/tablemap/
--rw-rw-rw-   0        0        0       34 2023-03-22 11:37:34.000000 tablemap-0.3.2/tablemap/__init__.py
--rw-rw-rw-   0        0        0    42606 2023-07-24 02:38:40.000000 tablemap-0.3.2/tablemap/tablemap.py
-drwxrwxrwx   0        0        0        0 2023-07-24 02:49:24.861883 tablemap-0.3.2/tablemap.egg-info/
--rw-rw-rw-   0        0        0      229 2023-07-24 02:49:24.000000 tablemap-0.3.2/tablemap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-07-24 02:49:24.000000 tablemap-0.3.2/tablemap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 02:49:24.000000 tablemap-0.3.2/tablemap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-24 02:49:24.000000 tablemap-0.3.2/tablemap.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-24 02:49:24.863881 tablemap-0.3.2/test/
--rw-rw-rw-   0        0        0        0 2023-03-22 11:37:34.000000 tablemap-0.3.2/test/__init__.py
--rw-rw-rw-   0        0        0    40154 2023-07-24 02:48:08.000000 tablemap-0.3.2/test/test_core.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:54:03.117787 tablemap-0.3.3/
+-rw-rw-rw-   0        0        0     1085 2023-03-22 11:37:34.000000 tablemap-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0      229 2023-07-25 06:54:03.117787 tablemap-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0    15613 2023-07-24 02:28:24.000000 tablemap-0.3.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-25 06:54:03.117787 tablemap-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      398 2023-07-24 11:14:03.000000 tablemap-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:54:03.100783 tablemap-0.3.3/tablemap/
+-rw-rw-rw-   0        0        0       34 2023-03-22 11:37:34.000000 tablemap-0.3.3/tablemap/__init__.py
+-rw-rw-rw-   0        0        0    43021 2023-07-24 11:54:26.000000 tablemap-0.3.3/tablemap/tablemap.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:54:03.113782 tablemap-0.3.3/tablemap.egg-info/
+-rw-rw-rw-   0        0        0      229 2023-07-25 06:54:03.000000 tablemap-0.3.3/tablemap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-07-25 06:54:03.000000 tablemap-0.3.3/tablemap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 06:54:03.000000 tablemap-0.3.3/tablemap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-25 06:54:03.000000 tablemap-0.3.3/tablemap.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 06:54:03.116782 tablemap-0.3.3/test/
+-rw-rw-rw-   0        0        0        0 2023-03-22 11:37:34.000000 tablemap-0.3.3/test/__init__.py
+-rw-rw-rw-   0        0        0    40307 2023-07-24 11:52:31.000000 tablemap-0.3.3/test/test_core.py
```

### Comparing `tablemap-0.3.2/LICENSE` & `tablemap-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tablemap-0.3.2/README.md` & `tablemap-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `tablemap-0.3.2/tablemap/tablemap.py` & `tablemap-0.3.3/tablemap/tablemap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1125,29 +1125,41 @@
     # iter is not safe to end-users, because the generator might not be
     # terminated after the database connection is closed.
     # This should be used in a controlled manner.
     def _iter(self):
         yield from self._history[-1]['genfn']()
 
     # list is safe, because it completes the iteration.
-    def list(self):
+    # I feel uneasy to pass classes to row_type
+    def list(self, row_type=dict):
         """Returns a list of rows(dicts)
 
+        Parameters
+        ----------
+        row_type: dict | list | tuple | set 
+            default dict
+
         Returns
         -------
-        list[Row]
+        list[row_type]
         """
         _raise_exception_if_preceded_by_grouping_methods(self)
 
         if self._history[0]['cmd'] == 'fetch':
             # no need to copy, becaused it's fetched from the database.
             # pylint: disable=protected-access
-            return list(self._iter())
+            if row_type == dict:
+                return list(self._iter())
+            else:
+                return list(row_type(r.values()) for r in self._iter())
+
         # pylint: disable=protected-access
-        return [row.copy() for row in self._iter()]
+        if row_type == dict:
+            return [row.copy() for row in self._iter()]
+        return [row_type(row.values()) for row in self._iter()] 
 
 
 def _listify(fields):
     if isinstance(fields, str):
         return [field.strip() for field in fields.split(',')]
     return fields
```

### Comparing `tablemap-0.3.2/test/test_core.py` & `tablemap-0.3.3/test/test_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,22 @@
         ]
 
     def tearDown(self):
         if Path(self.dbfile).is_file():
             os.remove(self.dbfile)
         if Path(self.dbfile1).is_file():
             os.remove(self.dbfile1)
+    
+    def test_list_various_types(self):
+        conn = Conn(self.dbfile)
+        conn['t2'] = self.t2
+
+        print(conn['t2'].list(set))
+
+
 
     def test_group_with_none(self):
         conn = Conn(self.dbfile)
         conn['t2'] = self.t2
 
         def foo(rs):
             return rs
```

