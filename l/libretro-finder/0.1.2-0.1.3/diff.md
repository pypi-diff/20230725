# Comparing `tmp/libretro_finder-0.1.2.tar.gz` & `tmp/libretro_finder-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretro_finder-0.1.2.tar", max compression
+gzip compressed data, was "libretro_finder-0.1.3.tar", max compression
```

## Comparing `libretro_finder-0.1.2.tar` & `libretro_finder-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1760 2023-07-25 13:44:19.751110 libretro_finder-0.1.2/config/__init__.py
--rw-r--r--   0        0        0        0 2023-07-25 13:44:19.751110 libretro_finder-0.1.2/libretro_finder/__init__.py
--rw-r--r--   0        0        0     3667 2023-07-25 13:44:19.751110 libretro_finder-0.1.2/libretro_finder/main.py
--rw-r--r--   0        0        0     1716 2023-07-25 13:44:19.751110 libretro_finder-0.1.2/libretro_finder/utils.py
--rw-r--r--   0        0        0    35823 2023-03-22 16:43:29.653449 libretro_finder-0.1.2/LICENSE
--rw-r--r--   0        0        0      869 2023-07-25 19:59:39.517634 libretro_finder-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3931 2023-07-25 19:12:24.999840 libretro_finder-0.1.2/README.md
--rw-r--r--   0        0        0     4672 1970-01-01 00:00:00.000000 libretro_finder-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1760 2023-07-25 13:44:19.751110 libretro_finder-0.1.3/config/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 13:44:19.751110 libretro_finder-0.1.3/libretro_finder/__init__.py
+-rw-r--r--   0        0        0     3667 2023-07-25 13:44:19.751110 libretro_finder-0.1.3/libretro_finder/main.py
+-rw-r--r--   0        0        0     1716 2023-07-25 13:44:19.751110 libretro_finder-0.1.3/libretro_finder/utils.py
+-rw-r--r--   0        0        0    35823 2023-03-22 16:43:29.653449 libretro_finder-0.1.3/LICENSE
+-rw-r--r--   0        0        0      869 2023-07-25 20:12:16.218912 libretro_finder-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3931 2023-07-25 19:12:24.999840 libretro_finder-0.1.3/README.md
+-rw-r--r--   0        0        0     4672 1970-01-01 00:00:00.000000 libretro_finder-0.1.3/PKG-INFO
```

### Comparing `libretro_finder-0.1.2/config/__init__.py` & `libretro_finder-0.1.3/config/__init__.py`

 * *Files identical despite different names*

### Comparing `libretro_finder-0.1.2/libretro_finder/main.py` & `libretro_finder-0.1.3/libretro_finder/main.py`

 * *Files identical despite different names*

### Comparing `libretro_finder-0.1.2/libretro_finder/utils.py` & `libretro_finder-0.1.3/libretro_finder/utils.py`

 * *Files identical despite different names*

### Comparing `libretro_finder-0.1.2/LICENSE` & `libretro_finder-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `libretro_finder-0.1.2/pyproject.toml` & `libretro_finder-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libretro-finder"
-version = "0.1.2"
+version = "0.1.3"
 description = "Command line utility that looks for specific BIOS files for libretro cores and, if found, refactors them to the expected format (i.e. name and directory structure)."
 authors = ["Jasper <j.siebring92@gmail.com>"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 packages = [
     {include = "libretro_finder"},
     {include = "config"},
```

### Comparing `libretro_finder-0.1.2/README.md` & `libretro_finder-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `libretro_finder-0.1.2/PKG-INFO` & `libretro_finder-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretro-finder
-Version: 0.1.2
+Version: 0.1.3
 Summary: Command line utility that looks for specific BIOS files for libretro cores and, if found, refactors them to the expected format (i.e. name and directory structure).
 License: GNU General Public License v3.0
 Author: Jasper
 Author-email: j.siebring92@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

