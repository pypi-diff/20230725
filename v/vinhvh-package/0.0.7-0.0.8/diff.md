# Comparing `tmp/vinhvh_package-0.0.7.tar.gz` & `tmp/vinhvh_package-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vinhvh_package-0.0.7.tar", last modified: Mon Jul 24 09:53:23 2023, max compression
+gzip compressed data, was "vinhvh_package-0.0.8.tar", last modified: Tue Jul 25 05:19:12 2023, max compression
```

## Comparing `vinhvh_package-0.0.7.tar` & `vinhvh_package-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 09:53:23.139003 vinhvh_package-0.0.7/
--rw-rw-rw-   0        0        0     1091 2023-07-23 05:09:13.000000 vinhvh_package-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      557 2023-07-24 09:53:23.137999 vinhvh_package-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       25 2023-07-23 06:07:00.000000 vinhvh_package-0.0.7/README.md
--rw-rw-rw-   0        0        0      612 2023-07-24 09:52:48.000000 vinhvh_package-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-24 09:53:23.140004 vinhvh_package-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-24 09:53:23.053272 vinhvh_package-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-07-24 09:53:23.111931 vinhvh_package-0.0.7/src/vinhvh_package/
--rw-rw-rw-   0        0        0        0 2023-07-23 06:05:35.000000 vinhvh_package-0.0.7/src/vinhvh_package/__init__.py
--rw-rw-rw-   0        0        0    17789 2023-07-24 05:12:22.000000 vinhvh_package-0.0.7/src/vinhvh_package/test_module.py
--rw-rw-rw-   0        0        0    17410 2023-07-24 09:52:23.000000 vinhvh_package-0.0.7/src/vinhvh_package/vinhvh.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:53:23.136997 vinhvh_package-0.0.7/src/vinhvh_package.egg-info/
--rw-rw-rw-   0        0        0      557 2023-07-24 09:53:23.000000 vinhvh_package-0.0.7/src/vinhvh_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-07-24 09:53:23.000000 vinhvh_package-0.0.7/src/vinhvh_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 09:53:23.000000 vinhvh_package-0.0.7/src/vinhvh_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-24 09:53:23.000000 vinhvh_package-0.0.7/src/vinhvh_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 05:19:12.253771 vinhvh_package-0.0.8/
+-rw-rw-rw-   0        0        0     1091 2023-07-23 05:09:13.000000 vinhvh_package-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      557 2023-07-25 05:19:12.250759 vinhvh_package-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       25 2023-07-23 06:07:00.000000 vinhvh_package-0.0.8/README.md
+-rw-rw-rw-   0        0        0      612 2023-07-25 05:18:38.000000 vinhvh_package-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-25 05:19:12.254272 vinhvh_package-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-25 05:19:12.191601 vinhvh_package-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-25 05:19:12.200625 vinhvh_package-0.0.8/src/vinhvh_package/
+-rw-rw-rw-   0        0        0        0 2023-07-23 06:05:35.000000 vinhvh_package-0.0.8/src/vinhvh_package/__init__.py
+-rw-rw-rw-   0        0        0    17789 2023-07-24 05:12:22.000000 vinhvh_package-0.0.8/src/vinhvh_package/test_module.py
+-rw-rw-rw-   0        0        0    17662 2023-07-25 05:16:37.000000 vinhvh_package-0.0.8/src/vinhvh_package/vinhvh.py
+drwxrwxrwx   0        0        0        0 2023-07-25 05:19:12.244753 vinhvh_package-0.0.8/src/vinhvh_package.egg-info/
+-rw-rw-rw-   0        0        0      557 2023-07-25 05:19:12.000000 vinhvh_package-0.0.8/src/vinhvh_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-07-25 05:19:12.000000 vinhvh_package-0.0.8/src/vinhvh_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 05:19:12.000000 vinhvh_package-0.0.8/src/vinhvh_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-25 05:19:12.000000 vinhvh_package-0.0.8/src/vinhvh_package.egg-info/top_level.txt
```

### Comparing `vinhvh_package-0.0.7/LICENSE` & `vinhvh_package-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vinhvh_package-0.0.7/PKG-INFO` & `vinhvh_package-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vinhvh_package
-Version: 0.0.7
+Version: 0.0.8
 Summary: A small example package
 Author-email: VinhVH <vinhvh89.dc@gmail.com>
 Project-URL: Homepage, https://github.com/VinhVu8x/packaging_tutorial
 Project-URL: Bug Tracker, https://github.com/VinhVu8x/packaging_tutorial/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vinhvh_package-0.0.7/pyproject.toml` & `vinhvh_package-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vinhvh_package"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="VinhVH", email="vinhvh89.dc@gmail.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `vinhvh_package-0.0.7/src/vinhvh_package/test_module.py` & `vinhvh_package-0.0.8/src/vinhvh_package/test_module.py`

 * *Files identical despite different names*

### Comparing `vinhvh_package-0.0.7/src/vinhvh_package/vinhvh.py` & `vinhvh_package-0.0.8/src/vinhvh_package/vinhvh.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,46 +120,50 @@
         print('File selection closed.')
         sys.exit()
     # If the user didn't select any files, return None
     else:
         return None
 
 
-def read_file(filepath: str, sheet_name: str = None):
+def read_file(filepath: str, sheet_name: str = None, skip_row: int = 0):
     """
     This function read form filepath and return to dataframe
 
     Parameters
     ----------
     file: (str)
         File to browse
     sheet_name: (str, optional)
         Name of sheet to read
+    skip_row: (st, optional)
+        Number of first row to skip
     Return
     ----------
     Dataframe
     """
     # Determine file type based on extension
     if filepath.lower().endswith(('.txt', '.csv', '.xlsx', '.xls', '.log', '.kml')):
         if filepath.lower().endswith('.txt'):
-            df = pd.read_csv(filepath, sep='	', low_memory=False)
+            df = pd.read_csv(filepath, sep='	',
+                             skiprows=skip_row, low_memory=False)
         elif filepath.lower().endswith('.csv'):
-            df = pd.read_csv(filepath, low_memory=False)
+            df = pd.read_csv(filepath, skiprows=skip_row, low_memory=False)
         elif filepath.lower().endswith('.xlsx'):
             if sheet_name is None:
-                df = pd.read_excel(filepath, engine='openpyxl')
+                df = pd.read_excel(
+                    filepath, skiprows=skip_row, engine='openpyxl')
             else:
                 df = pd.read_excel(
-                    filepath, sheet_name=sheet_name, engine='openpyxl')
+                    filepath, sheet_name=sheet_name, skiprows=skip_row, engine='openpyxl')
         elif filepath.lower().endswith('.xls'):
             if sheet_name is None:
-                df = pd.read_excel(filepath, engine='xlrd')
+                df = pd.read_excel(filepath, skiprows=skip_row, engine='xlrd')
             else:
                 df = pd.read_excel(
-                    filepath, sheet_name=sheet_name, engine='xlrd')
+                    filepath, sheet_name=sheet_name, skiprows=skip_row, engine='xlrd')
         elif filepath.lower().endswith('.log'):
             with open(filepath, 'r') as f:
                 lines = f.readlines()
             df = pd.DataFrame(lines, columns=['log'])
         elif filepath.lower().endswith('.kml'):
             # Parse the KML file using the pykml parser
             with open(filepath) as f:
```

### Comparing `vinhvh_package-0.0.7/src/vinhvh_package.egg-info/PKG-INFO` & `vinhvh_package-0.0.8/src/vinhvh_package.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vinhvh-package
-Version: 0.0.7
+Version: 0.0.8
 Summary: A small example package
 Author-email: VinhVH <vinhvh89.dc@gmail.com>
 Project-URL: Homepage, https://github.com/VinhVu8x/packaging_tutorial
 Project-URL: Bug Tracker, https://github.com/VinhVu8x/packaging_tutorial/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

