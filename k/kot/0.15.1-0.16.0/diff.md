# Comparing `tmp/kot-0.15.1.tar.gz` & `tmp/kot-0.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kot-0.15.1.tar", last modified: Tue Jul 25 01:15:12 2023, max compression
+gzip compressed data, was "kot-0.16.0.tar", last modified: Tue Jul 25 17:03:33 2023, max compression
```

## Comparing `kot-0.15.1.tar` & `kot-0.16.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:15:12.655315 kot-0.15.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-25 01:14:58.000000 kot-0.15.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-25 01:15:12.655315 kot-0.15.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-25 01:14:58.000000 kot-0.15.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 01:15:12.655315 kot-0.15.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-25 01:14:58.000000 kot-0.15.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:15:12.647315 kot-0.15.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:15:12.651315 kot-0.15.1/src/kot/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-25 01:14:58.000000 kot-0.15.1/src/kot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22071 2023-07-25 01:14:58.000000 kot-0.15.1/src/kot/kot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 01:15:12.651315 kot-0.15.1/src/kot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-25 01:15:12.000000 kot-0.15.1/src/kot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-25 01:15:12.000000 kot-0.15.1/src/kot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 01:15:12.000000 kot-0.15.1/src/kot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 01:15:12.000000 kot-0.15.1/src/kot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 01:15:12.000000 kot-0.15.1/src/kot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-25 01:15:12.000000 kot-0.15.1/src/kot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-25 01:15:12.000000 kot-0.15.1/src/kot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:03:33.205057 kot-0.16.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-25 17:03:17.000000 kot-0.16.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-25 17:03:33.205057 kot-0.16.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-25 17:03:17.000000 kot-0.16.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 17:03:33.205057 kot-0.16.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-25 17:03:17.000000 kot-0.16.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:03:33.205057 kot-0.16.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:03:33.205057 kot-0.16.0/src/kot/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-25 17:03:17.000000 kot-0.16.0/src/kot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23816 2023-07-25 17:03:17.000000 kot-0.16.0/src/kot/kot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:03:33.205057 kot-0.16.0/src/kot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-25 17:03:32.000000 kot-0.16.0/src/kot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-25 17:03:33.000000 kot-0.16.0/src/kot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 17:03:32.000000 kot-0.16.0/src/kot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 17:03:32.000000 kot-0.16.0/src/kot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 17:03:32.000000 kot-0.16.0/src/kot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-25 17:03:32.000000 kot-0.16.0/src/kot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-25 17:03:32.000000 kot-0.16.0/src/kot.egg-info/top_level.txt
```

### Comparing `kot-0.15.1/LICENSE` & `kot-0.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kot-0.15.1/PKG-INFO` & `kot-0.16.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kot
-Version: 0.15.1
+Version: 0.16.0
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KOT
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KOT database
```

### Comparing `kot-0.15.1/README.md` & `kot-0.16.0/README.md`

 * *Files identical despite different names*

### Comparing `kot-0.15.1/setup.py` & `kot-0.16.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='kot',
-version='0.15.1',
+version='0.16.0',
 description="""Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing""",
 long_description="".join(open("README.md", encoding="utf-8").readlines()),
 long_description_content_type='text/markdown',
 url='https://github.com/onuratakan/KOT',
 author='Onur Atakan ULUSOY',
 author_email='atadogan06@gmail.com',
 license='MIT',
```

### Comparing `kot-0.15.1/src/kot/kot.py` & `kot-0.16.0/src/kot/kot.py`

 * *Files 6% similar despite different names*

```diff
@@ -124,28 +124,32 @@
 
     @staticmethod
     def database_delete(name: str, folder: str = "") -> bool:
         database_index = KOT("KOT-database-index",
                              self_datas=True,
                              folder=folder)
         try:
+            the_db = KOT(name, folder=folder, self_datas=True)
+            for each_key in the_db.get_all():
+                the_db.delete(each_key)
             rmtree(database_index.get(name))
         except:
             return False
 
         database_index.delete(name)
         return True
 
     @staticmethod
     def database_delete_all(folder: str = ""):
         database_index = KOT("KOT-database-index",
                              self_datas=True,
                              folder=folder)
+
         for each_database in database_index.dict():
-            KOT.database_delete(each_database)
+            KOT.database_delete(each_database, folder=folder)
 
     @staticmethod
     def database_rename(name: str,
                         new_name: str,
                         force: bool = False,
                         folder: str = "") -> bool:
         if new_name in KOT.database_list() and not force:
@@ -162,14 +166,15 @@
             return False
         return True
 
     def __init__(self, name, self_datas: bool = False, folder: str = ""):
         self.name = name
         self.hashed_name = HASHES.get_hash(name)
         the_main_folder = os.getcwd() if not folder != "" else folder
+        self.the_main_folder = the_main_folder
         self.location = os.path.join(the_main_folder,
                                      "KOT-" + self.hashed_name)
 
         if not self_datas:
             self.open_files_db = KOT("KOT-open_files_db",
                                      self_datas=True,
                                      folder=folder)
@@ -241,28 +246,32 @@
         file: str = "",
         compress: bool = False,
         encryption_key: str = "",
         cache_policy: int = 0,
         dont_delete_cache: bool = False,
         dont_remove_file: bool = False,
         custom_key_location: str = "",
+        short_cut: bool = False,
     ) -> bool:
         self.counter += 1
 
         meta = {"type": "value", "file": None, "direct_file": True}
 
         if not isinstance(key, str):
             raise TypeError("Key must be a string")
         if not isinstance(file, str):
             raise TypeError("File must be a string")
 
         try:
             standart_key_location = os.path.join(self.location,HASHES.get_hash(key))
             key_location =  standart_key_location if custom_key_location == "" else custom_key_location
             
+            if custom_key_location != "" and not short_cut:
+                self.set(key,value=key_location,file=file,compress=compress,encryption_key=encryption_key,cache_policy=cache_policy,dont_delete_cache=dont_delete_cache,dont_remove_file=dont_remove_file,short_cut = True)            
+
             key_location_loading = os.path.join(self.location,
                                                 standart_key_location + ".l")
             random_number = random.randint(10000,99999)
             key_location_loading_indicator = os.path.join(
                 self.location, standart_key_location + str(random_number) + ".li")
 
             key_location_reading_indicator = os.path.join(
@@ -288,15 +297,17 @@
                 except:
                     traceback.print_exc()
                     return False
 
             if encryption_key != "":
                 value = self.encrypt(encryption_key, value)
 
-            the_dict = {"key": key, "value": value, "meta": meta}
+            the_dict = {"key": key, "value": value, "meta": meta, "short_cut": False}
+            if short_cut:
+                the_dict["short_cut"] = True
 
             if cache_policy != 0:
                 the_dict["cache_time"] = time.time()
                 the_dict["cache_policy"] = cache_policy
             else:
                 if key in self.cache and not dont_delete_cache:
                     del self.cache[key]
@@ -387,14 +398,15 @@
     def get(
         self,
         key: str,
         custom_key_location: str = "",
         encryption_key: str = "",
         no_cache: bool = False,
         raw_dict: bool = False,
+        get_shotcut: bool = False,
     ):
         if key in self.cache and not no_cache:
             cache_control = False
             currently = time.time()
             last_time = self.cache[key]["cache_time"]
             cache_policy = self.cache[key]["cache_policy"]
 
@@ -432,15 +444,15 @@
                 if not any_file:
                     busy = False
                     break
                 try_number += 1
                 time.sleep(0.25)
 
 
-        if not os.path.isfile(os.path.join(self.location, key_location)):
+        if not os.path.isfile(key_location):
             return None
 
         total_result = None
         total_result_standart = None
 
         try:
 
@@ -448,35 +460,36 @@
             with contextlib.suppress(Exception):
                 with open(key_location_reading_indicator, "wb") as f:
                     f.write(b"1")
 
             # Read the file
             if os.path.exists(key_location_compress_indicator):
                 import mgzip
-                with mgzip.open(os.path.join(self.location, key_location),
+                with mgzip.open(key_location,
                                 "rb") as f:
                     result = pickle.load(f)
             else:
-                with open(os.path.join(self.location, key_location),
+                with open(key_location,
                           "rb") as f:
                     result = pickle.load(f)
 
             # Transform the result
             total_result_standart = result
             try:
                 total_result = self.transformer(result, encryption_key=encryption_key)
             except TypeError:
+                traceback.print_exc()
                 total_result = result            
 
             # Add to cache
             if "cache_time" in total_result_standart:
                 self.cache[key] = total_result_standart
 
         except EOFError or FileNotFoundError:
-            pass
+            traceback.print_exc()
 
         # Delete the file that inform is reading
         if os.path.isfile(key_location_reading_indicator):
             with contextlib.suppress(Exception):
                 os.remove(key_location_reading_indicator)
 
         # Create the file if there is an compress or encryption situation
@@ -486,15 +499,33 @@
                     the_bytes = total_result_standart["value"]
                     if encryption_key != "":
                         the_bytes = self.decrypt(encryption_key, the_bytes)
                     f.write(the_bytes)
 
         # Return the result
         if raw_dict:
+
+            if total_result_standart["short_cut"] and not get_shotcut:
+                total_result_standart = self.get(key, custom_key_location=total_result_standart["value"],
+                                    encryption_key=encryption_key,
+                                    no_cache=no_cache,
+                                    raw_dict=raw_dict)
+
+
             return total_result_standart
+
+
+
+        if total_result_standart["short_cut"] and not get_shotcut:
+            total_result = self.get(key, custom_key_location=total_result_standart["value"],
+                                    encryption_key=encryption_key,
+                                    no_cache=no_cache,
+                                    raw_dict=raw_dict)
+
+
         return total_result
 
     def get_key(self, key_location: str):
         key_location_compress_indicator = os.path.join(self.location,
                                                        key_location + ".co")
         if not os.path.isfile(os.path.join(self.location, key_location)):
             return None
@@ -544,14 +575,22 @@
                 self.location, key_location + ".co")
 
             with contextlib.suppress(TypeError):
                 maybe_file = self.get(key)
                 if os.path.exists(maybe_file):
                     os.remove(maybe_file)
 
+            the_get = self.get(key, no_cache=True, raw_dict=True, get_shotcut=True)
+            if the_get["short_cut"]:
+                with contextlib.suppress(TypeError):
+                    maybe_file = self.get(key, custom_key_location=the_get["value"])
+                    if os.path.exists(maybe_file):
+                        os.remove(maybe_file)
+                os.remove(the_get["value"])             
+
             if os.path.exists(key_location_compress_indicator):
                 os.remove(
                     os.path.join(self.location,
                                  key_location_compress_indicator))
             if os.path.exists(os.path.join(self.location, key_location)):
                 os.remove(os.path.join(self.location, key_location))
         except:
```

### Comparing `kot-0.15.1/src/kot.egg-info/PKG-INFO` & `kot-0.16.0/src/kot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kot
-Version: 0.15.1
+Version: 0.16.0
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KOT
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KOT database
```

