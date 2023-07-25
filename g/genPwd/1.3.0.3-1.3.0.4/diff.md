# Comparing `tmp/genPwd-1.3.0.3.tar.gz` & `tmp/genPwd-1.3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genPwd-1.3.0.3.tar", last modified: Tue Jul 25 09:19:15 2023, max compression
+gzip compressed data, was "genPwd-1.3.0.4.tar", last modified: Tue Jul 25 09:32:14 2023, max compression
```

## Comparing `genPwd-1.3.0.3.tar` & `genPwd-1.3.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 09:19:15.573091 genPwd-1.3.0.3/
--rw-rw-r--   0 user      (1000) user      (1000)      746 2023-07-25 09:19:15.573091 genPwd-1.3.0.3/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      368 2023-07-19 21:20:51.000000 genPwd-1.3.0.3/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 09:19:15.569090 genPwd-1.3.0.3/genPwd/
--rw-rw-r--   0 user      (1000) user      (1000)       66 2023-07-25 05:32:15.000000 genPwd-1.3.0.3/genPwd/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2038 2023-07-25 05:55:02.000000 genPwd-1.3.0.3/genPwd/generate_password.py
--rw-rw-r--   0 user      (1000) user      (1000)      854 2023-07-25 05:31:36.000000 genPwd-1.3.0.3/genPwd/test_passw.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 09:19:15.573091 genPwd-1.3.0.3/genPwd.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      746 2023-07-25 09:19:15.000000 genPwd-1.3.0.3/genPwd.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      239 2023-07-25 09:19:15.000000 genPwd-1.3.0.3/genPwd.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-25 09:19:15.000000 genPwd-1.3.0.3/genPwd.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       68 2023-07-25 09:19:15.000000 genPwd-1.3.0.3/genPwd.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)        7 2023-07-25 09:19:15.000000 genPwd-1.3.0.3/genPwd.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-25 09:19:15.573091 genPwd-1.3.0.3/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1434 2023-07-25 09:17:06.000000 genPwd-1.3.0.3/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 09:32:14.477011 genPwd-1.3.0.4/
+-rw-rw-r--   0 user      (1000) user      (1000)      746 2023-07-25 09:32:14.477011 genPwd-1.3.0.4/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      368 2023-07-19 21:20:51.000000 genPwd-1.3.0.4/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 09:32:14.477011 genPwd-1.3.0.4/genPwd/
+-rw-rw-r--   0 user      (1000) user      (1000)       66 2023-07-25 05:32:15.000000 genPwd-1.3.0.4/genPwd/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2040 2023-07-25 09:27:59.000000 genPwd-1.3.0.4/genPwd/generate_password.py
+-rw-rw-r--   0 user      (1000) user      (1000)      854 2023-07-25 05:31:36.000000 genPwd-1.3.0.4/genPwd/test_passw.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 09:32:14.477011 genPwd-1.3.0.4/genPwd.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      746 2023-07-25 09:32:14.000000 genPwd-1.3.0.4/genPwd.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      239 2023-07-25 09:32:14.000000 genPwd-1.3.0.4/genPwd.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-25 09:32:14.000000 genPwd-1.3.0.4/genPwd.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       68 2023-07-25 09:32:14.000000 genPwd-1.3.0.4/genPwd.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        7 2023-07-25 09:32:14.000000 genPwd-1.3.0.4/genPwd.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-25 09:32:14.477011 genPwd-1.3.0.4/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1434 2023-07-25 09:29:32.000000 genPwd-1.3.0.4/setup.py
```

### Comparing `genPwd-1.3.0.3/PKG-INFO` & `genPwd-1.3.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genPwd
-Version: 1.3.0.3
+Version: 1.3.0.4
 Summary: This is a sample Description
 Home-page: https://github.com/kanchann/GenPwd
 Author: Kanchan
 Author-email: kanchanbora321@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `genPwd-1.3.0.3/genPwd/generate_password.py` & `genPwd-1.3.0.4/genPwd/generate_password.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 BIRD_FILE = 'bird.csv'
 
 # File paths
 
 places_file_path = os.path.join(current_working_dir,PLACES_FILE)
 bird_file_path = os.path.join(current_working_dir,BIRD_FILE)
 
-print("places_file_path>>>>>>>" , places_file_path)
-print("bird_file_path>>>>>>>>>>>>>" , bird_file_path)
+#print("places_file_path>>>>>>>" , places_file_path)
+#print("bird_file_path>>>>>>>>>>>>>" , bird_file_path)
 
 #places_file_path = os.path.join(current_working_dir,"Downloads" , "passwgeneration","passw",PLACES_FILE)
 #bird_file_path = os.path.join(current_working_dir,"Downloads","passwgeneration" ,"passw",BIRD_FILE)
 
 
 #print(places_file_path)
 #print(bird_file_path)
```

### Comparing `genPwd-1.3.0.3/genPwd/test_passw.py` & `genPwd-1.3.0.4/genPwd/test_passw.py`

 * *Files identical despite different names*

### Comparing `genPwd-1.3.0.3/genPwd.egg-info/PKG-INFO` & `genPwd-1.3.0.4/genPwd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genPwd
-Version: 1.3.0.3
+Version: 1.3.0.4
 Summary: This is a sample Description
 Home-page: https://github.com/kanchann/GenPwd
 Author: Kanchan
 Author-email: kanchanbora321@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `genPwd-1.3.0.3/setup.py` & `genPwd-1.3.0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
             if filename.endswith('.csv'):
                 relative_path = os.path.relpath(os.path.join(dirpath, filename), base_dir)
                 data_files.append(relative_path)
     return data_files
 
 setup(
     name="genPwd",
-    version="1.3.0.3",
+    version="1.3.0.4",
     author="Kanchan",
     author_email="kanchanbora321@gmail.com",
     description="This is a sample Description",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kanchann/GenPwd",
     packages=find_packages(),
```

