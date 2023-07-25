# Comparing `tmp/libretro_finder-0.1.1.tar.gz` & `tmp/libretro_finder-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretro_finder-0.1.1.tar", max compression
+gzip compressed data, was "libretro_finder-0.1.2.tar", max compression
```

## Comparing `libretro_finder-0.1.1.tar` & `libretro_finder-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1760 2023-07-25 09:53:52.648295 libretro_finder-0.1.1/config/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 19:33:27.530061 libretro_finder-0.1.1/libretro_finder/__init__.py
--rw-r--r--   0        0        0     3667 2023-07-25 12:41:28.893089 libretro_finder-0.1.1/libretro_finder/main.py
--rw-r--r--   0        0        0     1716 2023-07-25 09:22:57.544045 libretro_finder-0.1.1/libretro_finder/utils.py
--rw-r--r--   0        0        0    35823 2023-03-22 16:43:29.653449 libretro_finder-0.1.1/LICENSE
--rw-r--r--   0        0        0      869 2023-07-25 13:31:25.789129 libretro_finder-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3931 2023-07-25 13:22:21.422636 libretro_finder-0.1.1/README.md
--rw-r--r--   0        0        0     4529 1970-01-01 00:00:00.000000 libretro_finder-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1760 2023-07-25 13:44:19.751110 libretro_finder-0.1.2/config/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 13:44:19.751110 libretro_finder-0.1.2/libretro_finder/__init__.py
+-rw-r--r--   0        0        0     3667 2023-07-25 13:44:19.751110 libretro_finder-0.1.2/libretro_finder/main.py
+-rw-r--r--   0        0        0     1716 2023-07-25 13:44:19.751110 libretro_finder-0.1.2/libretro_finder/utils.py
+-rw-r--r--   0        0        0    35823 2023-03-22 16:43:29.653449 libretro_finder-0.1.2/LICENSE
+-rw-r--r--   0        0        0      869 2023-07-25 19:59:39.517634 libretro_finder-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3931 2023-07-25 19:12:24.999840 libretro_finder-0.1.2/README.md
+-rw-r--r--   0        0        0     4672 1970-01-01 00:00:00.000000 libretro_finder-0.1.2/PKG-INFO
```

### Comparing `libretro_finder-0.1.1/config/__init__.py` & `libretro_finder-0.1.2/config/__init__.py`

 * *Files identical despite different names*

### Comparing `libretro_finder-0.1.1/libretro_finder/main.py` & `libretro_finder-0.1.2/libretro_finder/main.py`

 * *Files identical despite different names*

### Comparing `libretro_finder-0.1.1/libretro_finder/utils.py` & `libretro_finder-0.1.2/libretro_finder/utils.py`

 * *Files identical despite different names*

### Comparing `libretro_finder-0.1.1/LICENSE` & `libretro_finder-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `libretro_finder-0.1.1/pyproject.toml` & `libretro_finder-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "libretro-finder"
-version = "0.1.1"
+version = "0.1.2"
 description = "Command line utility that looks for specific BIOS files for libretro cores and, if found, refactors them to the expected format (i.e. name and directory structure)."
 authors = ["Jasper <j.siebring92@gmail.com>"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 packages = [
     {include = "libretro_finder"},
     {include = "config"},
 ]
 
 [tool.poetry.scripts]
 libretro_finder = "libretro_finder.main:main"
 
 [tool.poetry.dependencies]
-python = "^3.11"
-numpy = "^1.25.1"
-pandas = "^2.0.3"
+python = "^3.8"
+numpy = "^1.15.0"
+pandas = ">=1.1.5"
 tqdm = "^4.65.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pylint = "^2.17.4"
 black = "^23.7.0"
 mypy = "^1.4.1"
```

### Comparing `libretro_finder-0.1.1/README.md` & `libretro_finder-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `libretro_finder-0.1.1/PKG-INFO` & `libretro_finder-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: libretro-finder
-Version: 0.1.1
+Version: 0.1.2
 Summary: Command line utility that looks for specific BIOS files for libretro cores and, if found, refactors them to the expected format (i.e. name and directory structure).
 License: GNU General Public License v3.0
 Author: Jasper
 Author-email: j.siebring92@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: numpy (>=1.25.1,<2.0.0)
-Requires-Dist: pandas (>=2.0.3,<3.0.0)
+Requires-Dist: numpy (>=1.15.0,<2.0.0)
+Requires-Dist: pandas (>=1.1.5)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # libretro_finder
 Simple command line utility that recursively looks for specific BIOS files for RetroArch cores and, if found, refactors them to the expected format as documented by Libretro [here](https://github.com/libretro/libretro-database/blob/4a98ea9726b3954a4e5a940d255bd14c307ddfba/dat/System.dat) (i.e. name and directory structure). This is useful if you source your BIOS files from many different places and have them saved them under different names (often with duplicates). This script is able to find these exact BIOS files by comparing their hashes against their known counterparts. Uses concurrency and vectorization for added performance.   
 
 This repository does **NOT** include the BIOS files themselves.
```

