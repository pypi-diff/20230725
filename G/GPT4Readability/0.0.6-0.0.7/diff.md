# Comparing `tmp/GPT4Readability-0.0.6.tar.gz` & `tmp/GPT4Readability-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GPT4Readability-0.0.6.tar", last modified: Mon Jul 24 21:57:33 2023, max compression
+gzip compressed data, was "GPT4Readability-0.0.7.tar", last modified: Mon Jul 24 22:28:09 2023, max compression
```

## Comparing `GPT4Readability-0.0.6.tar` & `GPT4Readability-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:57:33.039554 GPT4Readability-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:57:33.039554 GPT4Readability-0.0.6/GPT4Readability/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:57:19.000000 GPT4Readability-0.0.6/GPT4Readability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-24 21:57:19.000000 GPT4Readability-0.0.6/GPT4Readability/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:57:33.039554 GPT4Readability-0.0.6/GPT4Readability/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:57:19.000000 GPT4Readability-0.0.6/GPT4Readability/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-24 21:57:19.000000 GPT4Readability-0.0.6/GPT4Readability/prompts/readme_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-24 21:57:19.000000 GPT4Readability-0.0.6/GPT4Readability/prompts/refactor_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-24 21:57:19.000000 GPT4Readability-0.0.6/GPT4Readability/readme_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-24 21:57:19.000000 GPT4Readability-0.0.6/GPT4Readability/suggestions_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-07-24 21:57:19.000000 GPT4Readability-0.0.6/GPT4Readability/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:57:33.039554 GPT4Readability-0.0.6/GPT4Readability.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-07-24 21:57:33.000000 GPT4Readability-0.0.6/GPT4Readability.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-24 21:57:33.000000 GPT4Readability-0.0.6/GPT4Readability.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 21:57:33.000000 GPT4Readability-0.0.6/GPT4Readability.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-24 21:57:33.000000 GPT4Readability-0.0.6/GPT4Readability.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-24 21:57:33.000000 GPT4Readability-0.0.6/GPT4Readability.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 21:57:33.000000 GPT4Readability-0.0.6/GPT4Readability.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-24 21:57:19.000000 GPT4Readability-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-07-24 21:57:33.039554 GPT4Readability-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-24 21:57:19.000000 GPT4Readability-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 21:57:33.039554 GPT4Readability-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-24 21:57:19.000000 GPT4Readability-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:28:09.454870 GPT4Readability-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:28:09.450870 GPT4Readability-0.0.7/GPT4Readability/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:27:56.000000 GPT4Readability-0.0.7/GPT4Readability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-24 22:27:56.000000 GPT4Readability-0.0.7/GPT4Readability/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:28:09.454870 GPT4Readability-0.0.7/GPT4Readability/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 22:27:56.000000 GPT4Readability-0.0.7/GPT4Readability/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-24 22:27:56.000000 GPT4Readability-0.0.7/GPT4Readability/prompts/readme_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-24 22:27:56.000000 GPT4Readability-0.0.7/GPT4Readability/prompts/refactor_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-24 22:27:56.000000 GPT4Readability-0.0.7/GPT4Readability/readme_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-24 22:27:56.000000 GPT4Readability-0.0.7/GPT4Readability/suggestions_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-07-24 22:27:56.000000 GPT4Readability-0.0.7/GPT4Readability/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:28:09.454870 GPT4Readability-0.0.7/GPT4Readability.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-07-24 22:28:09.000000 GPT4Readability-0.0.7/GPT4Readability.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-24 22:28:09.000000 GPT4Readability-0.0.7/GPT4Readability.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 22:28:09.000000 GPT4Readability-0.0.7/GPT4Readability.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-24 22:28:09.000000 GPT4Readability-0.0.7/GPT4Readability.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-24 22:28:09.000000 GPT4Readability-0.0.7/GPT4Readability.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 22:28:09.000000 GPT4Readability-0.0.7/GPT4Readability.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-24 22:27:56.000000 GPT4Readability-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-07-24 22:28:09.454870 GPT4Readability-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-24 22:27:56.000000 GPT4Readability-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 22:28:09.454870 GPT4Readability-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-24 22:27:56.000000 GPT4Readability-0.0.7/setup.py
```

### Comparing `GPT4Readability-0.0.6/GPT4Readability/__main__.py` & `GPT4Readability-0.0.7/GPT4Readability/__main__.py`

 * *Files identical despite different names*

### Comparing `GPT4Readability-0.0.6/GPT4Readability/prompts/readme_prompt.txt` & `GPT4Readability-0.0.7/GPT4Readability/prompts/readme_prompt.txt`

 * *Files identical despite different names*

### Comparing `GPT4Readability-0.0.6/GPT4Readability/prompts/refactor_prompt.txt` & `GPT4Readability-0.0.7/GPT4Readability/prompts/refactor_prompt.txt`

 * *Files identical despite different names*

### Comparing `GPT4Readability-0.0.6/GPT4Readability/readme_gen.py` & `GPT4Readability-0.0.7/GPT4Readability/readme_gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         root_dir (str): The root directory of the python package to parse and generate a readme for
     """
 
     # prompt_folder_name = os.path.join(os.path.dirname(__file__), "prompts")
     # prompt_path = os.path.join(prompt_folder_name, "readme_prompt.txt")
 
     with pkg_resources.open_text('GPT4Readability.prompts','readme_prompt.txt') as f:         
-		inb_msg = f.read()
+	    inb_msg = f.read()
 
     # with open(prompt_path) as f:
     #     lines = f.readlines()
     # inb_msg = "".join(lines)
 
     file_check_result = check_files_in_directory(root_dir) # Checking for the license and requirements.txt
     inb_msg += file_check_result
```

### Comparing `GPT4Readability-0.0.6/GPT4Readability/suggestions_gen.py` & `GPT4Readability-0.0.7/GPT4Readability/suggestions_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """
 
     # prompt_folder_name = os.path.join(os.path.dirname(__file__), "prompts")
     # prompt_path = os.path.join(prompt_folder_name, "refactor_prompt.txt")
 
 
     with pkg_resources.open_text('GPT4Readability.prompts','refactor_prompt.txt') as f:         
-		inb_msg = f.read()
+	    inb_msg = f.read()
 
 
     docs = get_docs(root_dir)
     python_files = find_python_files(root_dir)
     suggestions = []
     
     texts = split_docs(docs)
```

### Comparing `GPT4Readability-0.0.6/GPT4Readability/utils.py` & `GPT4Readability-0.0.7/GPT4Readability/utils.py`

 * *Files identical despite different names*

### Comparing `GPT4Readability-0.0.6/GPT4Readability.egg-info/PKG-INFO` & `GPT4Readability-0.0.7/GPT4Readability.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPT4Readability
-Version: 0.0.6
+Version: 0.0.7
 Summary: A tool to automatically generate a README.md and suggest code improvements for any python code repository
 Home-page: https://github.com/loevlie/GPT4Readability
 Author: Dennis Johan Loevlie
 Author-email: loevliedenny@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `GPT4Readability-0.0.6/GPT4Readability.egg-info/SOURCES.txt` & `GPT4Readability-0.0.7/GPT4Readability.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GPT4Readability-0.0.6/LICENSE` & `GPT4Readability-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `GPT4Readability-0.0.6/PKG-INFO` & `GPT4Readability-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPT4Readability
-Version: 0.0.6
+Version: 0.0.7
 Summary: A tool to automatically generate a README.md and suggest code improvements for any python code repository
 Home-page: https://github.com/loevlie/GPT4Readability
 Author: Dennis Johan Loevlie
 Author-email: loevliedenny@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `GPT4Readability-0.0.6/README.md` & `GPT4Readability-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `GPT4Readability-0.0.6/setup.py` & `GPT4Readability-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md', 'r') as readme:
     # ignore gifs
     description = ''.join([i for i in readme.readlines()
                            if not i.startswith('![')])
 
 setup(
     name='GPT4Readability',
-    version='0.0.6',
+    version='0.0.7',
     url='https://github.com/loevlie/GPT4Readability',
     author='Dennis Johan Loevlie',
     author_email='loevliedenny@gmail.com',
     description='A tool to automatically generate a README.md and suggest code improvements for any python code repository',
     long_description=description,
     long_description_content_type='text/markdown',
     packages=find_packages(),  # automatically discover all packages and subpackages
```

