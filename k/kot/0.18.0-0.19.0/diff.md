# Comparing `tmp/kot-0.18.0.tar.gz` & `tmp/kot-0.19.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kot-0.18.0.tar", last modified: Tue Jul 25 18:33:49 2023, max compression
+gzip compressed data, was "kot-0.19.0.tar", last modified: Tue Jul 25 18:46:05 2023, max compression
```

## Comparing `kot-0.18.0.tar` & `kot-0.19.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:33:49.198442 kot-0.18.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-25 18:33:36.000000 kot-0.18.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-25 18:33:49.198442 kot-0.18.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-25 18:33:36.000000 kot-0.18.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 18:33:49.198442 kot-0.18.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-25 18:33:36.000000 kot-0.18.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:33:49.194442 kot-0.18.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:33:49.198442 kot-0.18.0/src/kot/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-25 18:33:36.000000 kot-0.18.0/src/kot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24576 2023-07-25 18:33:36.000000 kot-0.18.0/src/kot/kot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:33:49.198442 kot-0.18.0/src/kot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-25 18:33:48.000000 kot-0.18.0/src/kot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-25 18:33:49.000000 kot-0.18.0/src/kot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:33:48.000000 kot-0.18.0/src/kot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 18:33:48.000000 kot-0.18.0/src/kot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:33:48.000000 kot-0.18.0/src/kot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-25 18:33:48.000000 kot-0.18.0/src/kot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-25 18:33:48.000000 kot-0.18.0/src/kot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:46:05.943882 kot-0.19.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-25 18:45:53.000000 kot-0.19.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-25 18:46:05.943882 kot-0.19.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-25 18:45:53.000000 kot-0.19.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 18:46:05.943882 kot-0.19.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-25 18:45:53.000000 kot-0.19.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:46:05.939882 kot-0.19.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:46:05.943882 kot-0.19.0/src/kot/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-25 18:45:53.000000 kot-0.19.0/src/kot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25512 2023-07-25 18:45:53.000000 kot-0.19.0/src/kot/kot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:46:05.943882 kot-0.19.0/src/kot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-25 18:46:05.000000 kot-0.19.0/src/kot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-25 18:46:05.000000 kot-0.19.0/src/kot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:46:05.000000 kot-0.19.0/src/kot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 18:46:05.000000 kot-0.19.0/src/kot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:46:05.000000 kot-0.19.0/src/kot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-25 18:46:05.000000 kot-0.19.0/src/kot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-25 18:46:05.000000 kot-0.19.0/src/kot.egg-info/top_level.txt
```

### Comparing `kot-0.18.0/LICENSE` & `kot-0.19.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kot-0.18.0/PKG-INFO` & `kot-0.19.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kot
-Version: 0.18.0
+Version: 0.19.0
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KOT
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KOT database
```

### Comparing `kot-0.18.0/README.md` & `kot-0.19.0/README.md`

 * *Files identical despite different names*

### Comparing `kot-0.18.0/setup.py` & `kot-0.19.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='kot',
-version='0.18.0',
+version='0.19.0',
 description="""Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing""",
 long_description="".join(open("README.md", encoding="utf-8").readlines()),
 long_description_content_type='text/markdown',
 url='https://github.com/onuratakan/KOT',
 author='Onur Atakan ULUSOY',
 author_email='atadogan06@gmail.com',
 license='MIT',
```

### Comparing `kot-0.18.0/src/kot/kot.py` & `kot-0.19.0/src/kot/kot.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 from shutil import copy
 from shutil import make_archive
 from shutil import move
 from shutil import rmtree
 from shutil import unpack_archive
 import random
 
+
+force_compress = False
+force_encrypt = False
+
+
 class HASHES:
     cache = {}
     @staticmethod
     def get_hash(string: str, hash_type: str = "sha256") -> str:
         if string in HASHES.cache:
             return HASHES.cache[string]
         if hash_type == "sha256":
@@ -36,14 +41,17 @@
 
 class KOT:
 
     @staticmethod
     def benchmark_set(number: int = 10000,
                       compress: bool = False,
                       encryption_key: str = "") -> float:
+        compress = True if force_compress else compress
+        encryption_key = force_encrypt if force_encrypt != False else encryption_key
+            
         my_db = KOT("KOT-benchmark", self_datas=True)
         start = time.time()
         for i in range(number):
             my_db.set(
                 "key" + str(i),
                 "value" + str(i),
                 compress=compress,
@@ -56,14 +64,16 @@
     @staticmethod
     def benchmark_get(
         number: int = 10000,
         compress: bool = False,
         encryption_key: str = "",
         dont_generate: bool = False,
     ) -> float:
+        compress = True if force_compress else compress
+        encryption_key = force_encrypt if force_encrypt != False else encryption_key
         my_db = KOT("KOT-benchmark", self_datas=True)
         if not dont_generate:
             for i in range(number):
                 my_db.set(
                     "key" + str(i),
                     "value" + str(i),
                     compress=compress,
@@ -79,14 +89,16 @@
     @staticmethod
     def benchmark_delete(
         number: int = 10000,
         compress: bool = False,
         encryption_key: str = "",
         dont_generate: bool = False,
     ) -> float:
+        compress = True if force_compress else compress
+        encryption_key = force_encrypt if force_encrypt != False else encryption_key
         my_db = KOT("KOT-benchmark", self_datas=True)
         if not dont_generate:
             for i in range(number):
                 my_db.set(
                     "key" + str(i),
                     "value" + str(i),
                     compress=compress,
@@ -99,14 +111,16 @@
         my_db.delete_all()
         return end - start
 
     @staticmethod
     def benchmark(number: int = 10000,
                   compress: bool = False,
                   encryption_key: str = "") -> float:
+        compress = True if force_compress else compress
+        encryption_key = force_encrypt if force_encrypt != False else encryption_key
         total_time = 0
         total_time += KOT.benchmark_set(number, compress, encryption_key)
         total_time += KOT.benchmark_get(number,
                                         compress,
                                         encryption_key,
                                         dont_generate=True)
         total_time += KOT.benchmark_delete(number,
@@ -272,14 +286,16 @@
         encryption_key: str = "",
         cache_policy: int = 0,
         dont_delete_cache: bool = False,
         dont_remove_file: bool = False,
         custom_key_location: str = "",
         short_cut: bool = False,
     ) -> bool:
+        compress = True if force_compress else compress
+        encryption_key = force_encrypt if force_encrypt != False else encryption_key
         self.counter += 1
 
         meta = {"type": "value", "file": None, "direct_file": True}
 
         if not isinstance(key, str):
             raise TypeError("Key must be a string")
         if not isinstance(file, str):
@@ -424,14 +440,15 @@
         key: str,
         custom_key_location: str = "",
         encryption_key: str = "",
         no_cache: bool = False,
         raw_dict: bool = False,
         get_shotcut: bool = False,
     ):
+        encryption_key = force_encrypt if force_encrypt != False else encryption_key
         if key in self.cache and not no_cache:
             cache_control = False
             currently = time.time()
             last_time = self.cache[key]["cache_time"]
             cache_policy = self.cache[key]["cache_policy"]
 
             if currently - last_time < cache_policy:
@@ -629,14 +646,15 @@
                 self.delete(key)
         except:
             traceback.print_exc()
             return False
         return True
 
     def dict(self, encryption_key: str = "", no_data: bool = False):
+        encryption_key = force_encrypt if force_encrypt != False else encryption_key
         result = {}
         for key in os.listdir(self.location):
             if not "." in key:
                 the_key = self.get_key(key)
                 if not the_key is None:
                     if the_key != False:
                         result_of_key = (self.get(
```

### Comparing `kot-0.18.0/src/kot.egg-info/PKG-INFO` & `kot-0.19.0/src/kot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kot
-Version: 0.18.0
+Version: 0.19.0
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KOT
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KOT database
```

