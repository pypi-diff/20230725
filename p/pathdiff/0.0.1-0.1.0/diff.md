# Comparing `tmp/pathdiff-0.0.1.tar.gz` & `tmp/pathdiff-0.1.0.tar.gz`

## Comparing `pathdiff-0.0.1.tar` & `pathdiff-0.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 pathdiff-0.0.1/src/pathdiff/__about__.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pathdiff-0.0.1/src/pathdiff/__init__.py
--rw-r--r--   0        0        0     9375 2020-02-02 00:00:00.000000 pathdiff-0.0.1/src/pathdiff/pathdiff.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pathdiff-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-0.0.1/tests/test1/path1/file1.txt
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-0.0.1/tests/test1/path1/file2.txt
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-0.0.1/tests/test1/path1/file3.txt
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-0.0.1/tests/test1/path1/file4.txt
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 pathdiff-0.0.1/tests/test1/path1/file5.txt
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 pathdiff-0.0.1/tests/test1/path1/file6.txt
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-0.0.1/tests/test1/path2/file7.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 pathdiff-0.0.1/tests/test1/path2/file8.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 pathdiff-0.0.1/tests/test1/path2/file9.txt
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-0.0.1/tests/test2/path1/file1.txt
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-0.0.1/tests/test2/path1/file2.txt
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-0.0.1/tests/test2/path1/file3.txt
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-0.0.1/tests/test2/path1/file4.txt
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 pathdiff-0.0.1/tests/test2/path1/file5.txt
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 pathdiff-0.0.1/tests/test2/path1/file6.txt
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-0.0.1/tests/test2/path2/file3.txt
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-0.0.1/tests/test2/path2/file4.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 pathdiff-0.0.1/tests/test2/path2/file5.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 pathdiff-0.0.1/tests/test2/path2/file6.txt
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-0.0.1/tests/test2/path2/file7.txt
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-0.0.1/tests/test2/path2/file8.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pathdiff-0.0.1/.gitignore
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pathdiff-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 pathdiff-0.0.1/README.md
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 pathdiff-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 pathdiff-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 pathdiff-0.1.0/src/pathdiff/__about__.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pathdiff-0.1.0/src/pathdiff/__init__.py
+-rw-r--r--   0        0        0     9375 2020-02-02 00:00:00.000000 pathdiff-0.1.0/src/pathdiff/pathdiff.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pathdiff-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-0.1.0/tests/test1/path1/file1.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-0.1.0/tests/test1/path1/file2.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-0.1.0/tests/test1/path1/file3.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-0.1.0/tests/test1/path1/file4.txt
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 pathdiff-0.1.0/tests/test1/path1/file5.txt
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 pathdiff-0.1.0/tests/test1/path1/file6.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-0.1.0/tests/test1/path2/file7.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 pathdiff-0.1.0/tests/test1/path2/file8.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 pathdiff-0.1.0/tests/test1/path2/file9.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-0.1.0/tests/test2/path1/file1.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-0.1.0/tests/test2/path1/file2.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-0.1.0/tests/test2/path1/file3.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-0.1.0/tests/test2/path1/file4.txt
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 pathdiff-0.1.0/tests/test2/path1/file5.txt
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 pathdiff-0.1.0/tests/test2/path1/file6.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-0.1.0/tests/test2/path2/file3.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-0.1.0/tests/test2/path2/file4.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 pathdiff-0.1.0/tests/test2/path2/file5.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 pathdiff-0.1.0/tests/test2/path2/file6.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-0.1.0/tests/test2/path2/file7.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pathdiff-0.1.0/tests/test2/path2/file8.txt
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pathdiff-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pathdiff-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 pathdiff-0.1.0/README.md
+-rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 pathdiff-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 pathdiff-0.1.0/PKG-INFO
```

### Comparing `pathdiff-0.0.1/src/pathdiff/pathdiff.py` & `pathdiff-0.1.0/src/pathdiff/pathdiff.py`

 * *Files identical despite different names*

### Comparing `pathdiff-0.0.1/LICENSE.txt` & `pathdiff-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pathdiff-0.0.1/README.md` & `pathdiff-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 
 Duplicates found:
 tests/test1/path2/file8.txt
 tests/test1/path2/file9.txt
 ```
 
-```
+```console
 ❯ pathdiff compare-directories tests/test2/path1 tests/test2/path2
 Comparing directories tests/test2/path1 and tests/test2/path2
 Comparing directory structures
 |████████████████████████████████████████| 12 in 0.1s (114.04/s)
 Comparing common files
 |████████████████████████████████████████| 4/4 [100%] in 0.1s (37.66/s)
```

### Comparing `pathdiff-0.0.1/pyproject.toml` & `pathdiff-0.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pathdiff"
 dynamic = ["version"]
-description = ''
+description = "A tool for detecting duplicate files and comparing directories."
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Manvith Narahari", email = "manvithn@gmail.com" },
 ]
@@ -37,14 +37,15 @@
 [project.scripts]
 pathdiff = "pathdiff.pathdiff:cli"
 
 [tool.hatch.version]
 path = "src/pathdiff/__about__.py"
 
 [tool.hatch.envs.default]
+python = "python3"
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
```

### Comparing `pathdiff-0.0.1/PKG-INFO` & `pathdiff-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: pathdiff
-Version: 0.0.1
+Version: 0.1.0
+Summary: A tool for detecting duplicate files and comparing directories.
 Project-URL: Documentation, https://github.com/manvithn/pathdiff#readme
 Project-URL: Issues, https://github.com/manvithn/pathdiff/issues
 Project-URL: Source, https://github.com/manvithn/pathdiff
 Author-email: Manvith Narahari <manvithn@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -79,15 +80,15 @@
 
 
 Duplicates found:
 tests/test1/path2/file8.txt
 tests/test1/path2/file9.txt
 ```
 
-```
+```console
 ❯ pathdiff compare-directories tests/test2/path1 tests/test2/path2
 Comparing directories tests/test2/path1 and tests/test2/path2
 Comparing directory structures
 |████████████████████████████████████████| 12 in 0.1s (114.04/s)
 Comparing common files
 |████████████████████████████████████████| 4/4 [100%] in 0.1s (37.66/s)
```

