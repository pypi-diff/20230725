# Comparing `tmp/lp_ap_tools-0.1.8.tar.gz` & `tmp/lp_ap_tools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lp_ap_tools-0.1.8.tar", last modified: Tue Jul 18 02:11:49 2023, max compression
+gzip compressed data, was "lp_ap_tools-0.1.9.tar", last modified: Mon Jul 24 23:09:09 2023, max compression
```

## Comparing `lp_ap_tools-0.1.8.tar` & `lp_ap_tools-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 eller      (501) staff       (20)        0 2023-07-18 02:11:49.823413 lp_ap_tools-0.1.8/
--rw-r--r--   0 eller      (501) staff       (20)      759 2023-07-18 02:11:49.823252 lp_ap_tools-0.1.8/PKG-INFO
--rw-r--r--   0 eller      (501) staff       (20)      339 2023-05-30 22:31:42.000000 lp_ap_tools-0.1.8/README.md
-drwxr-xr-x   0 eller      (501) staff       (20)        0 2023-07-18 02:11:49.821733 lp_ap_tools-0.1.8/lp_ap_tools/
--rw-r--r--   0 eller      (501) staff       (20)       15 2023-05-29 02:44:23.000000 lp_ap_tools-0.1.8/lp_ap_tools/__init__.py
--rw-r--r--   0 eller      (501) staff       (20)    11625 2023-07-18 02:08:23.000000 lp_ap_tools-0.1.8/lp_ap_tools/lp_ap_tools.py
-drwxr-xr-x   0 eller      (501) staff       (20)        0 2023-07-18 02:11:49.822580 lp_ap_tools-0.1.8/lp_ap_tools.egg-info/
--rw-r--r--   0 eller      (501) staff       (20)      759 2023-07-18 02:11:49.000000 lp_ap_tools-0.1.8/lp_ap_tools.egg-info/PKG-INFO
--rw-r--r--   0 eller      (501) staff       (20)      287 2023-07-18 02:11:49.000000 lp_ap_tools-0.1.8/lp_ap_tools.egg-info/SOURCES.txt
--rw-r--r--   0 eller      (501) staff       (20)        1 2023-07-18 02:11:49.000000 lp_ap_tools-0.1.8/lp_ap_tools.egg-info/dependency_links.txt
--rw-r--r--   0 eller      (501) staff       (20)       30 2023-07-18 02:11:49.000000 lp_ap_tools-0.1.8/lp_ap_tools.egg-info/requires.txt
--rw-r--r--   0 eller      (501) staff       (20)       18 2023-07-18 02:11:49.000000 lp_ap_tools-0.1.8/lp_ap_tools.egg-info/top_level.txt
--rw-r--r--   0 eller      (501) staff       (20)       38 2023-07-18 02:11:49.823458 lp_ap_tools-0.1.8/setup.cfg
--rw-r--r--   0 eller      (501) staff       (20)      801 2023-07-18 02:09:43.000000 lp_ap_tools-0.1.8/setup.py
-drwxr-xr-x   0 eller      (501) staff       (20)        0 2023-07-18 02:11:49.822900 lp_ap_tools-0.1.8/tests/
--rw-r--r--   0 eller      (501) staff       (20)        0 2023-05-29 02:51:18.000000 lp_ap_tools-0.1.8/tests/__init__.py
--rw-r--r--   0 eller      (501) staff       (20)      104 2023-05-29 03:34:42.000000 lp_ap_tools-0.1.8/tests/lp_ap_tools_test.py
+drwxr-xr-x   0 eller      (501) staff       (20)        0 2023-07-24 23:09:09.420343 lp_ap_tools-0.1.9/
+-rw-r--r--   0 eller      (501) staff       (20)      759 2023-07-24 23:09:09.420173 lp_ap_tools-0.1.9/PKG-INFO
+-rw-r--r--   0 eller      (501) staff       (20)      339 2023-05-30 22:31:42.000000 lp_ap_tools-0.1.9/README.md
+drwxr-xr-x   0 eller      (501) staff       (20)        0 2023-07-24 23:09:09.418758 lp_ap_tools-0.1.9/lp_ap_tools/
+-rw-r--r--   0 eller      (501) staff       (20)       15 2023-05-29 02:44:23.000000 lp_ap_tools-0.1.9/lp_ap_tools/__init__.py
+-rw-r--r--   0 eller      (501) staff       (20)    12347 2023-07-24 23:07:46.000000 lp_ap_tools-0.1.9/lp_ap_tools/lp_ap_tools.py
+drwxr-xr-x   0 eller      (501) staff       (20)        0 2023-07-24 23:09:09.419563 lp_ap_tools-0.1.9/lp_ap_tools.egg-info/
+-rw-r--r--   0 eller      (501) staff       (20)      759 2023-07-24 23:09:09.000000 lp_ap_tools-0.1.9/lp_ap_tools.egg-info/PKG-INFO
+-rw-r--r--   0 eller      (501) staff       (20)      287 2023-07-24 23:09:09.000000 lp_ap_tools-0.1.9/lp_ap_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 eller      (501) staff       (20)        1 2023-07-24 23:09:09.000000 lp_ap_tools-0.1.9/lp_ap_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 eller      (501) staff       (20)       30 2023-07-24 23:09:09.000000 lp_ap_tools-0.1.9/lp_ap_tools.egg-info/requires.txt
+-rw-r--r--   0 eller      (501) staff       (20)       18 2023-07-24 23:09:09.000000 lp_ap_tools-0.1.9/lp_ap_tools.egg-info/top_level.txt
+-rw-r--r--   0 eller      (501) staff       (20)       38 2023-07-24 23:09:09.420389 lp_ap_tools-0.1.9/setup.cfg
+-rw-r--r--   0 eller      (501) staff       (20)      801 2023-07-24 23:08:12.000000 lp_ap_tools-0.1.9/setup.py
+drwxr-xr-x   0 eller      (501) staff       (20)        0 2023-07-24 23:09:09.419801 lp_ap_tools-0.1.9/tests/
+-rw-r--r--   0 eller      (501) staff       (20)        0 2023-05-29 02:51:18.000000 lp_ap_tools-0.1.9/tests/__init__.py
+-rw-r--r--   0 eller      (501) staff       (20)      104 2023-05-29 03:34:42.000000 lp_ap_tools-0.1.9/tests/lp_ap_tools_test.py
```

### Comparing `lp_ap_tools-0.1.8/PKG-INFO` & `lp_ap_tools-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lp_ap_tools
-Version: 0.1.8
+Version: 0.1.9
 Summary: A python decorator for creating ActionProvider RO-crates within a Globus flow
 Home-page: https://github.com/GusEllerm/lp_tools.git
 Author: Augustus Ellerm
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lp_ap_tools-0.1.8/lp_ap_tools/lp_ap_tools.py` & `lp_ap_tools-0.1.9/lp_ap_tools/lp_ap_tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,14 +56,26 @@
    print("********** ap_status **********")
    print_attributes(ap_status)
    print("********** ap_auth **********")
    print_attributes(ap_auth)
    print("********** ap_apbt **********")
    print_attributes(ap_apbt)
 
+def clean_directory(directory_path):
+    for filename in os.listdir(directory_path):
+        file_path = os.path.join(directory_path, filename)
+        try:
+            if os.path.isfile(file_path) or os.path.islink(file_path):
+                os.unlink(file_path)
+            elif os.path.isdir(file_path):
+                shutil.rmtree(file_path)
+        except Exception as e:
+            print('Failed to delete %s. Reason: %s' % (file_path, e))
+
+
 # -----------------------------------------------
 # -- Integrating globus metadata with ROcrate ---
 # -----------------------------------------------
 
 def import_ap_description(ap_description: ActionProviderDescription,
                           crate: ROCrate):
    pass
@@ -152,14 +164,15 @@
 def create_method(crate: ROCrate,
                   dir_struct: dict):
    method_files = crate.add_tree(dir_struct['method'])
    return method_files
 
 def transfer_crate(ap_auth: AuthState,
                    crate_path: str,
+                   dir_struct: dict,
                    orchestration_node: str,
                    article_name: str,
                    ap_status: ActionStatus,
                    ap_apbt: ActionProviderBlueprint):
    
    # Get local running globus connect personal endpoint
    local_gcp = LocalGlobusConnectPersonal()
@@ -182,16 +195,19 @@
 
    def cleanup():
       # Check status of transfer periodically untill complete. Then remove local crate. 
       while not transfer_client.task_wait(transfer_result["task_id"], polling_interval=20, timeout=300):
          pass
 
       # Delete crate
-      print(f"Transfer {transfer_result['task_id']} sucssess. Removing local crate.")
+      print(f"Transfer {transfer_result['task_id']} sucssess. Cleaning LPAP (removing local crate and data)")
       shutil.rmtree(crate_path)
+      # TODO: re-enable cleaning of input dir when testing is finished. 
+      # clean_directory(dir_struct['input'])
+      clean_directory(dir_struct['output'])
 
    threading.Thread(target=cleanup).start()   
 
 
 # -----------------------------------------------
 # ------------ Primary decorator  ---------------
 # -----------------------------------------------
@@ -259,14 +275,15 @@
          action["total_time"] = total_time
 
          # Write RO-Crate to disk
          crate.write_crate(os.path.join(dir_struct["crates"], crate_name))
          # Transfer crate to management endpoint
          transfer_crate(ap_auth=ap_auth,
                         crate_path=os.path.join(dir_struct["crates"], crate_name), 
+                        dir_struct=dir_struct,
                         orchestration_node=ap_request.body["orchestration_node"],
                         article_name=ap_request.body['article_name'],
                         ap_status=ap_status,
                         ap_apbt=ap_apbt)
          return computation
       return create_ROcrate
     return middle
```

### Comparing `lp_ap_tools-0.1.8/lp_ap_tools.egg-info/PKG-INFO` & `lp_ap_tools-0.1.9/lp_ap_tools.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lp-ap-tools
-Version: 0.1.8
+Version: 0.1.9
 Summary: A python decorator for creating ActionProvider RO-crates within a Globus flow
 Home-page: https://github.com/GusEllerm/lp_tools.git
 Author: Augustus Ellerm
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lp_ap_tools-0.1.8/setup.py` & `lp_ap_tools-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 setup(
     name='lp_ap_tools',
     packages=find_packages(),
-    version='0.1.8',
+    version='0.1.9',
     description='A python decorator for creating ActionProvider RO-crates within a Globus flow',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Augustus Ellerm',
     license='MIT',
     install_requires=['rocrate', 
                       'pydantic',
```

