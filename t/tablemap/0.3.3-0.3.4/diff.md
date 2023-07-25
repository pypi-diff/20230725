# Comparing `tmp/tablemap-0.3.3.tar.gz` & `tmp/tablemap-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablemap-0.3.3.tar", last modified: Tue Jul 25 06:54:03 2023, max compression
+gzip compressed data, was "tablemap-0.3.4.tar", last modified: Tue Jul 25 09:41:04 2023, max compression
```

## Comparing `tablemap-0.3.3.tar` & `tablemap-0.3.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 06:54:03.117787 tablemap-0.3.3/
--rw-rw-rw-   0        0        0     1085 2023-03-22 11:37:34.000000 tablemap-0.3.3/LICENSE
--rw-rw-rw-   0        0        0      229 2023-07-25 06:54:03.117787 tablemap-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0    15613 2023-07-24 02:28:24.000000 tablemap-0.3.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-25 06:54:03.117787 tablemap-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      398 2023-07-24 11:14:03.000000 tablemap-0.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 06:54:03.100783 tablemap-0.3.3/tablemap/
--rw-rw-rw-   0        0        0       34 2023-03-22 11:37:34.000000 tablemap-0.3.3/tablemap/__init__.py
--rw-rw-rw-   0        0        0    43021 2023-07-24 11:54:26.000000 tablemap-0.3.3/tablemap/tablemap.py
-drwxrwxrwx   0        0        0        0 2023-07-25 06:54:03.113782 tablemap-0.3.3/tablemap.egg-info/
--rw-rw-rw-   0        0        0      229 2023-07-25 06:54:03.000000 tablemap-0.3.3/tablemap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-07-25 06:54:03.000000 tablemap-0.3.3/tablemap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 06:54:03.000000 tablemap-0.3.3/tablemap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-25 06:54:03.000000 tablemap-0.3.3/tablemap.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-25 06:54:03.116782 tablemap-0.3.3/test/
--rw-rw-rw-   0        0        0        0 2023-03-22 11:37:34.000000 tablemap-0.3.3/test/__init__.py
--rw-rw-rw-   0        0        0    40307 2023-07-24 11:52:31.000000 tablemap-0.3.3/test/test_core.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:41:04.878564 tablemap-0.3.4/
+-rw-rw-rw-   0        0        0     1085 2023-03-22 11:37:34.000000 tablemap-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0      229 2023-07-25 09:41:04.877275 tablemap-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0    15613 2023-07-24 02:28:24.000000 tablemap-0.3.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-25 09:41:04.878564 tablemap-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      398 2023-07-25 09:38:36.000000 tablemap-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:41:04.858738 tablemap-0.3.4/tablemap/
+-rw-rw-rw-   0        0        0       34 2023-03-22 11:37:34.000000 tablemap-0.3.4/tablemap/__init__.py
+-rw-rw-rw-   0        0        0    43109 2023-07-25 09:39:41.000000 tablemap-0.3.4/tablemap/tablemap.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:41:04.870257 tablemap-0.3.4/tablemap.egg-info/
+-rw-rw-rw-   0        0        0      229 2023-07-25 09:41:04.000000 tablemap-0.3.4/tablemap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-07-25 09:41:04.000000 tablemap-0.3.4/tablemap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 09:41:04.000000 tablemap-0.3.4/tablemap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-25 09:41:04.000000 tablemap-0.3.4/tablemap.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 09:41:04.874273 tablemap-0.3.4/test/
+-rw-rw-rw-   0        0        0        0 2023-03-22 11:37:34.000000 tablemap-0.3.4/test/__init__.py
+-rw-rw-rw-   0        0        0    40307 2023-07-24 11:52:31.000000 tablemap-0.3.4/test/test_core.py
```

### Comparing `tablemap-0.3.3/LICENSE` & `tablemap-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tablemap-0.3.3/README.md` & `tablemap-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `tablemap-0.3.3/tablemap/tablemap.py` & `tablemap-0.3.4/tablemap/tablemap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1194,15 +1194,19 @@
 
 
 def _delete(dbconn, table_name):
     dbconn.cursor().execute(f'drop table if exists {table_name}')
 
 
 def _insert(dbconn, table_name, rows):
-    irows = iter(rows)
+    if isinstance(rows, Rows):
+        irows = rows._iter()
+    else: 
+        irows = iter(rows)
+        
     try:
         first_row = next(irows)
     except StopIteration:
         raise ValueError(f"No row to insert in {table_name}") from None
     else:
         fields = list(first_row)
```

### Comparing `tablemap-0.3.3/test/test_core.py` & `tablemap-0.3.4/test/test_core.py`

 * *Files identical despite different names*

