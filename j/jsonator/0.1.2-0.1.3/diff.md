# Comparing `tmp/jsonator-0.1.2.tar.gz` & `tmp/jsonator-0.1.3.tar.gz`

## Comparing `jsonator-0.1.2.tar` & `jsonator-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 jsonator-0.1.2/jsonator/__init__.py
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 jsonator-0.1.2/jsonator/jsonator.py
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 jsonator-0.1.2/jsonator/output.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 jsonator-0.1.2/.gitignore
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jsonator-0.1.2/LICENSE
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 jsonator-0.1.2/README.rst
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 jsonator-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 jsonator-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 jsonator-0.1.3/jsonator/__init__.py
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 jsonator-0.1.3/jsonator/jsonator.py
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 jsonator-0.1.3/jsonator/output.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 jsonator-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jsonator-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 jsonator-0.1.3/README.rst
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 jsonator-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 jsonator-0.1.3/PKG-INFO
```

### Comparing `jsonator-0.1.2/jsonator/__init__.py` & `jsonator-0.1.3/jsonator/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         return ReturnCode.FILE_NOT_FOUND.value
 
     if args.path.is_dir():
         all_files_identical = True
         pattern = "**/*.json" if args.recursive else "*.json"
 
         for json_file in args.path.glob(pattern):
-            result = format_json_file(json_file, args.check)
+            result = format_json_file(json_file, args.check, args.diff, args.color)
 
             if result == ReturnCode.INTERNAL_ERROR:
                 return ReturnCode.INTERNAL_ERROR.value
 
             if result == ReturnCode.SOME_FILES_WOULD_BE_REFORMATTED and args.check:
                 all_files_identical = False
```

### Comparing `jsonator-0.1.2/jsonator/jsonator.py` & `jsonator-0.1.3/jsonator/jsonator.py`

 * *Files 14% similar despite different names*

```diff
@@ -59,25 +59,25 @@
 
         if is_identical:
             print("Ok")
             os.unlink(tmp_file)
             return ReturnCode.NOTHING_WOULD_CHANGE
 
         print("Need to format")
-        found_diff = output.diff(
+        diff_contents = output.diff(
             json_file.read_text(encoding=FILES_ENCODING),
             tmp_file.read_text(encoding=FILES_ENCODING),
             json_file.name,
             tmp_file.name,
         )
 
         if color:
-            found_diff = output.color_diff(found_diff)
+            diff_contents = output.color_diff(diff_contents)
 
-        print(found_diff)
+        print(diff_contents)
 
         os.unlink(tmp_file)
         return ReturnCode.SOME_FILES_WOULD_BE_REFORMATTED
 
     if tmp_file.exists():
         os.unlink(json_file)
         os.rename(tmp_file, json_file)
```

### Comparing `jsonator-0.1.2/jsonator/output.py` & `jsonator-0.1.3/jsonator/output.py`

 * *Files identical despite different names*

### Comparing `jsonator-0.1.2/LICENSE` & `jsonator-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonator-0.1.2/README.rst` & `jsonator-0.1.3/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 
 * path: A required argument that specifies the path to the JSON file or directory containing JSON files to be formatted.
 
 * --recursive or -r: An optional flag that specifies whether to scan subdirectories for JSON files.
 
 * --check: An optional flag that indicates whether to perform a dry run and return the status without actually reformatting the files. The exit code will indicate whether any files would be reformatted or if there were any errors.
 
+* --diff: Don't write the files back, just output a diff for each file on stdout.
+
+* --color: Show colored diff. Only applies when `--diff` is given.
+
 The module uses the ReturnCode enum to indicate the exit code of the formatting operation. The possible exit codes are:
 
 * `0`: Indicates that no files would be reformatted.
 
 * `1`: Indicates that some files would be reformatted.
 
 * `122`: Indicates that the specified file or directory was not found.
```

### Comparing `jsonator-0.1.2/pyproject.toml` & `jsonator-0.1.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=0.25.1",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "jsonator"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Sergey Fomin", email="sergiusnn@gmail.com" },
 ]
 description = "JSON formatting and validating tool"
 readme = "README.rst"
 requires-python = ">=3.5"
 classifiers = [
@@ -31,14 +31,8 @@
     "/jsonator/*",
 ]
 
 [project.scripts]
 jsonator = "jsonator:main"
 
 [tool.poetry]
-readme = "README.rst"
-name = "jsonator"
-version = "0.1.2"
-authors = [
-  "Sergey Fomin <sergiusnn@gmail.com>",
-]
-description = "JSON formatting and validating tool"
+readme = "README.rst"
```

### Comparing `jsonator-0.1.2/PKG-INFO` & `jsonator-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonator
-Version: 0.1.2
+Version: 0.1.3
 Summary: JSON formatting and validating tool
 Project-URL: Homepage, https://github.com/sfominx/jsonator
 Author-email: Sergey Fomin <sergiusnn@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.5
@@ -31,14 +31,18 @@
 
 * path: A required argument that specifies the path to the JSON file or directory containing JSON files to be formatted.
 
 * --recursive or -r: An optional flag that specifies whether to scan subdirectories for JSON files.
 
 * --check: An optional flag that indicates whether to perform a dry run and return the status without actually reformatting the files. The exit code will indicate whether any files would be reformatted or if there were any errors.
 
+* --diff: Don't write the files back, just output a diff for each file on stdout.
+
+* --color: Show colored diff. Only applies when `--diff` is given.
+
 The module uses the ReturnCode enum to indicate the exit code of the formatting operation. The possible exit codes are:
 
 * `0`: Indicates that no files would be reformatted.
 
 * `1`: Indicates that some files would be reformatted.
 
 * `122`: Indicates that the specified file or directory was not found.
```

