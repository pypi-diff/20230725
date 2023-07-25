# Comparing `tmp/repleno-0.0.15.tar.gz` & `tmp/repleno-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repleno-0.0.15.tar", last modified: Fri Jul 21 12:19:20 2023, max compression
+gzip compressed data, was "repleno-0.0.16.tar", last modified: Tue Jul 25 10:34:04 2023, max compression
```

## Comparing `repleno-0.0.15.tar` & `repleno-0.0.16.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 afoalb    (1000) afoalb    (1000)        0 2023-07-21 12:19:20.915044 repleno-0.0.15/
--rw-rw-r--   0 afoalb    (1000) afoalb    (1000)     2551 2023-07-21 12:19:20.915044 repleno-0.0.15/PKG-INFO
--rw-r--r--   0 afoalb    (1000) afoalb    (1000)     2017 2023-06-26 17:07:24.000000 repleno-0.0.15/README.md
--rw-r--r--   0 afoalb    (1000) afoalb    (1000)     1009 2023-07-21 12:19:07.000000 repleno-0.0.15/pyproject.toml
--rw-rw-r--   0 afoalb    (1000) afoalb    (1000)       38 2023-07-21 12:19:20.915044 repleno-0.0.15/setup.cfg
-drwxrwxr-x   0 afoalb    (1000) afoalb    (1000)        0 2023-07-21 12:19:20.915044 repleno-0.0.15/src/
-drwxrwxr-x   0 afoalb    (1000) afoalb    (1000)        0 2023-07-21 12:19:20.915044 repleno-0.0.15/src/repleno/
--rw-r--r--   0 afoalb    (1000) afoalb    (1000)    35720 2023-07-21 12:11:55.000000 repleno-0.0.15/src/repleno/SKU.py
--rw-r--r--   0 afoalb    (1000) afoalb    (1000)      519 2023-06-25 14:02:32.000000 repleno-0.0.15/src/repleno/__init__.py
--rw-r--r--   0 afoalb    (1000) afoalb    (1000)       96 2023-06-25 14:02:32.000000 repleno-0.0.15/src/repleno/__main__.py
--rw-r--r--   0 afoalb    (1000) afoalb    (1000)    27582 2023-07-21 12:11:40.000000 repleno-0.0.15/src/repleno/factory.py
--rw-r--r--   0 afoalb    (1000) afoalb    (1000)     2310 2023-06-26 18:04:48.000000 repleno-0.0.15/src/repleno/order.py
--rw-r--r--   0 afoalb    (1000) afoalb    (1000)     9575 2023-07-06 16:17:59.000000 repleno-0.0.15/src/repleno/utils.py
-drwxrwxr-x   0 afoalb    (1000) afoalb    (1000)        0 2023-07-21 12:19:20.915044 repleno-0.0.15/src/repleno.egg-info/
--rw-rw-r--   0 afoalb    (1000) afoalb    (1000)     2551 2023-07-21 12:19:20.000000 repleno-0.0.15/src/repleno.egg-info/PKG-INFO
--rw-rw-r--   0 afoalb    (1000) afoalb    (1000)      330 2023-07-21 12:19:20.000000 repleno-0.0.15/src/repleno.egg-info/SOURCES.txt
--rw-rw-r--   0 afoalb    (1000) afoalb    (1000)        1 2023-07-21 12:19:20.000000 repleno-0.0.15/src/repleno.egg-info/dependency_links.txt
--rw-rw-r--   0 afoalb    (1000) afoalb    (1000)       28 2023-07-21 12:19:20.000000 repleno-0.0.15/src/repleno.egg-info/requires.txt
--rw-rw-r--   0 afoalb    (1000) afoalb    (1000)        8 2023-07-21 12:19:20.000000 repleno-0.0.15/src/repleno.egg-info/top_level.txt
+drwxrwxr-x   0 afoalb    (1000) afoalb    (1000)        0 2023-07-25 10:34:04.793999 repleno-0.0.16/
+-rw-rw-r--   0 afoalb    (1000) afoalb    (1000)     2551 2023-07-25 10:34:04.793999 repleno-0.0.16/PKG-INFO
+-rw-r--r--   0 afoalb    (1000) afoalb    (1000)     2017 2023-06-26 17:07:24.000000 repleno-0.0.16/README.md
+-rw-r--r--   0 afoalb    (1000) afoalb    (1000)     1009 2023-07-25 10:33:10.000000 repleno-0.0.16/pyproject.toml
+-rw-rw-r--   0 afoalb    (1000) afoalb    (1000)       38 2023-07-25 10:34:04.793999 repleno-0.0.16/setup.cfg
+drwxrwxr-x   0 afoalb    (1000) afoalb    (1000)        0 2023-07-25 10:34:04.793999 repleno-0.0.16/src/
+drwxrwxr-x   0 afoalb    (1000) afoalb    (1000)        0 2023-07-25 10:34:04.793999 repleno-0.0.16/src/repleno/
+-rw-r--r--   0 afoalb    (1000) afoalb    (1000)    35720 2023-07-21 12:11:55.000000 repleno-0.0.16/src/repleno/SKU.py
+-rw-r--r--   0 afoalb    (1000) afoalb    (1000)      519 2023-06-25 14:02:32.000000 repleno-0.0.16/src/repleno/__init__.py
+-rw-r--r--   0 afoalb    (1000) afoalb    (1000)       96 2023-06-25 14:02:32.000000 repleno-0.0.16/src/repleno/__main__.py
+-rw-r--r--   0 afoalb    (1000) afoalb    (1000)    27582 2023-07-21 18:35:22.000000 repleno-0.0.16/src/repleno/factory.py
+-rw-r--r--   0 afoalb    (1000) afoalb    (1000)     2310 2023-06-26 18:04:48.000000 repleno-0.0.16/src/repleno/order.py
+-rw-r--r--   0 afoalb    (1000) afoalb    (1000)     9764 2023-07-25 10:27:03.000000 repleno-0.0.16/src/repleno/utils.py
+drwxrwxr-x   0 afoalb    (1000) afoalb    (1000)        0 2023-07-25 10:34:04.793999 repleno-0.0.16/src/repleno.egg-info/
+-rw-rw-r--   0 afoalb    (1000) afoalb    (1000)     2551 2023-07-25 10:34:04.000000 repleno-0.0.16/src/repleno.egg-info/PKG-INFO
+-rw-rw-r--   0 afoalb    (1000) afoalb    (1000)      330 2023-07-25 10:34:04.000000 repleno-0.0.16/src/repleno.egg-info/SOURCES.txt
+-rw-rw-r--   0 afoalb    (1000) afoalb    (1000)        1 2023-07-25 10:34:04.000000 repleno-0.0.16/src/repleno.egg-info/dependency_links.txt
+-rw-rw-r--   0 afoalb    (1000) afoalb    (1000)       28 2023-07-25 10:34:04.000000 repleno-0.0.16/src/repleno.egg-info/requires.txt
+-rw-rw-r--   0 afoalb    (1000) afoalb    (1000)        8 2023-07-25 10:34:04.000000 repleno-0.0.16/src/repleno.egg-info/top_level.txt
```

### Comparing `repleno-0.0.15/PKG-INFO` & `repleno-0.0.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repleno
-Version: 0.0.15
+Version: 0.0.16
 Summary: Supply chain analytics on Bill Of Materials (BOM) and Material Requirements Planning (MRP)
 Author-email: Afonso Schulz Albrecht <a.schulzalbrecht@gmail.com>
 Keywords: supply chain,bill of materials,material requirements planning,BOM,MRP
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Manufacturing
```

### Comparing `repleno-0.0.15/README.md` & `repleno-0.0.16/README.md`

 * *Files identical despite different names*

### Comparing `repleno-0.0.15/pyproject.toml` & `repleno-0.0.16/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 
 [project]
 name = 'repleno'
-version = '0.0.15'
+version = '0.0.16'
 authors = [
     {'name' = 'Afonso Schulz Albrecht', email = 'a.schulzalbrecht@gmail.com'},
 ]
 description = 'Supply chain analytics on Bill Of Materials (BOM) and Material Requirements Planning (MRP)'
 keywords = ['supply chain', 'bill of materials', 'material requirements planning', 'BOM', 'MRP']
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
```

### Comparing `repleno-0.0.15/src/repleno/SKU.py` & `repleno-0.0.16/src/repleno/SKU.py`

 * *Files identical despite different names*

### Comparing `repleno-0.0.15/src/repleno/__init__.py` & `repleno-0.0.16/src/repleno/__init__.py`

 * *Files identical despite different names*

### Comparing `repleno-0.0.15/src/repleno/factory.py` & `repleno-0.0.16/src/repleno/factory.py`

 * *Files identical despite different names*

### Comparing `repleno-0.0.15/src/repleno/order.py` & `repleno-0.0.16/src/repleno/order.py`

 * *Files identical despite different names*

### Comparing `repleno-0.0.15/src/repleno/utils.py` & `repleno-0.0.16/src/repleno/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,17 @@
 def read_and_parse_csv(file, mandatory_mapping, optional_mapping={}) -> List[Dict]:
     # docu: mappings are key-value pairs where the key are the column that
     # should be in the output dictionary and the value is the key used to find
     # the data in the csv
 
     output = []
     try:
-        with open(file, newline="", encoding="utf-8") as file:
+        # Use encoding with byte order mark to remove \\ufeff from strings
+		# explained here: https://stackoverflow.com/questions/17912307/u-ufeff-in-python-string/17912811#17912811
+        with open(file, newline="", encoding="utf-8-sig") as file:
             data = csv.DictReader(file)
 
             for row in data:
                 output.append(parse_dict(row, mandatory_mapping, optional_mapping))
 
     except FileNotFoundError:
         print("Error: File not found.")
```

### Comparing `repleno-0.0.15/src/repleno.egg-info/PKG-INFO` & `repleno-0.0.16/src/repleno.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repleno
-Version: 0.0.15
+Version: 0.0.16
 Summary: Supply chain analytics on Bill Of Materials (BOM) and Material Requirements Planning (MRP)
 Author-email: Afonso Schulz Albrecht <a.schulzalbrecht@gmail.com>
 Keywords: supply chain,bill of materials,material requirements planning,BOM,MRP
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Manufacturing
```

