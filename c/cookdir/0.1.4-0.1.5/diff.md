# Comparing `tmp/cookdir-0.1.4.tar.gz` & `tmp/cookdir-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cookdir-0.1.4.tar", last modified: Wed Sep  7 01:47:59 2022, max compression
+gzip compressed data, was "cookdir-0.1.5.tar", last modified: Tue Jul 25 02:55:19 2023, max compression
```

## Comparing `cookdir-0.1.4.tar` & `cookdir-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxrwxrwx   0        0        0        0 2022-09-07 01:47:59.302652 cookdir-0.1.4/
--rw-rw-rw-   0        0        0    35823 2022-09-06 02:29:44.000000 cookdir-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     1790 2022-09-07 01:47:59.302652 cookdir-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1336 2022-09-06 02:29:44.000000 cookdir-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2022-09-07 01:47:59.279713 cookdir-0.1.4/cookdir/
--rw-rw-rw-   0        0        0       11 2022-09-06 02:29:44.000000 cookdir-0.1.4/cookdir/__init__.py
--rw-rw-rw-   0        0        0     4116 2022-09-07 01:43:20.000000 cookdir-0.1.4/cookdir/main.py
-drwxrwxrwx   0        0        0        0 2022-09-07 01:47:59.300659 cookdir-0.1.4/cookdir/recipe/
--rw-rw-rw-   0        0        0      121 2022-09-06 02:29:44.000000 cookdir-0.1.4/cookdir/recipe/data_analysis.yml
--rw-rw-rw-   0        0        0      203 2022-09-06 02:29:44.000000 cookdir-0.1.4/cookdir/recipe/main.yml
--rw-rw-rw-   0        0        0      131 2022-09-06 02:29:44.000000 cookdir-0.1.4/cookdir/recipe/pypkg.yml
--rw-rw-rw-   0        0        0      496 2022-09-06 02:29:44.000000 cookdir-0.1.4/cookdir/recipe/pypkg_setup.tpl
--rw-rw-rw-   0        0        0      372 2022-09-06 02:29:44.000000 cookdir-0.1.4/cookdir/utils.py
-drwxrwxrwx   0        0        0        0 2022-09-07 01:47:59.291681 cookdir-0.1.4/cookdir.egg-info/
--rw-rw-rw-   0        0        0     1790 2022-09-07 01:47:59.000000 cookdir-0.1.4/cookdir.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      380 2022-09-07 01:47:59.000000 cookdir-0.1.4/cookdir.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-07 01:47:59.000000 cookdir-0.1.4/cookdir.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2022-09-07 01:47:59.000000 cookdir-0.1.4/cookdir.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       24 2022-09-07 01:47:59.000000 cookdir-0.1.4/cookdir.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-09-07 01:47:59.000000 cookdir-0.1.4/cookdir.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-09-07 01:47:59.302652 cookdir-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1014 2022-09-07 01:47:54.000000 cookdir-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:55:19.071108 cookdir-0.1.5/
+-rw-rw-rw-   0        0        0    35823 2022-09-06 02:29:44.000000 cookdir-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     1790 2023-07-25 02:55:19.071108 cookdir-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1336 2022-09-06 02:29:44.000000 cookdir-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 02:55:19.039866 cookdir-0.1.5/cookdir/
+-rw-rw-rw-   0        0        0       11 2022-09-06 02:29:44.000000 cookdir-0.1.5/cookdir/__init__.py
+-rw-rw-rw-   0        0        0     4581 2023-07-25 02:39:07.000000 cookdir-0.1.5/cookdir/main.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:55:19.071108 cookdir-0.1.5/cookdir/recipe/
+-rw-rw-rw-   0        0        0      121 2023-07-19 06:36:18.000000 cookdir-0.1.5/cookdir/recipe/data_analysis.yml
+-rw-rw-rw-   0        0        0      213 2023-07-25 02:00:29.000000 cookdir-0.1.5/cookdir/recipe/deeplearning.yml
+-rw-rw-rw-   0        0        0     1587 2023-07-19 08:51:55.000000 cookdir-0.1.5/cookdir/recipe/deeplearning_config.tpl
+-rw-rw-rw-   0        0        0    11339 2023-07-20 02:28:49.000000 cookdir-0.1.5/cookdir/recipe/deeplearning_from_lambda.tpl
+-rw-rw-rw-   0        0        0     8672 2023-07-25 02:00:08.000000 cookdir-0.1.5/cookdir/recipe/deeplearning_trainer.tpl
+-rw-rw-rw-   0        0        0      203 2022-09-06 02:29:44.000000 cookdir-0.1.5/cookdir/recipe/main.yml
+-rw-rw-rw-   0        0        0      131 2022-09-06 02:29:44.000000 cookdir-0.1.5/cookdir/recipe/pypkg.yml
+-rw-rw-rw-   0        0        0      496 2022-09-06 02:29:44.000000 cookdir-0.1.5/cookdir/recipe/pypkg_setup.tpl
+-rw-rw-rw-   0        0        0      372 2022-09-06 02:29:44.000000 cookdir-0.1.5/cookdir/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 02:55:19.055586 cookdir-0.1.5/cookdir.egg-info/
+-rw-rw-rw-   0        0        0     1790 2023-07-25 02:55:18.000000 cookdir-0.1.5/cookdir.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      535 2023-07-25 02:55:18.000000 cookdir-0.1.5/cookdir.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 02:55:18.000000 cookdir-0.1.5/cookdir.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-25 02:55:18.000000 cookdir-0.1.5/cookdir.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       24 2023-07-25 02:55:18.000000 cookdir-0.1.5/cookdir.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-25 02:55:18.000000 cookdir-0.1.5/cookdir.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 02:55:19.071108 cookdir-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1014 2023-07-25 02:39:24.000000 cookdir-0.1.5/setup.py
```

### Comparing `cookdir-0.1.4/LICENSE` & `cookdir-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cookdir-0.1.4/PKG-INFO` & `cookdir-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookdir
-Version: 0.1.4
+Version: 0.1.5
 Summary: create directories by template
 Home-page: https://github.com/Blockhead-yj/cookdir
 Author: yjdai
 Author-email: 136271877@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `cookdir-0.1.4/README.md` & `cookdir-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `cookdir-0.1.4/cookdir/main.py` & `cookdir-0.1.5/cookdir/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import re
 from functools import singledispatch
-
+from pathlib import Path
 import glob
 
 import fire
 import yaml
 
 # set the base directory, to get access to recipes without path error
 base_dir = __file__[:__file__.rfind(os.path.sep)]
@@ -32,24 +32,24 @@
         if os.path.isfile(recipe):
             recipe_file = recipe
         elif os.path.isfile(f"{base_dir}/recipe/{recipe}"):
             recipe_file = f"{base_dir}/recipe/{recipe}"
         else:
             print(f"Input recipe {base_dir}/recipe/{recipe} is not a valid template name or filepath, please check it!")
             return None
-        with open(root, "w") as f:
-            with open(recipe_file, 'r') as tpl:
+        with open(root, "w", encoding='utf-8') as f:
+            with open(recipe_file, 'r', encoding='utf-8') as tpl:
                 for line in tpl:
                     f.write(line)
         return root
     path = os.path.join(root, recipe)
     if recipe.find(".") >= 0:
         if not os.path.isfile(path):
             print(f"Creating file {path}...")
-            open(path, "w").close()
+            open(path, "w", encoding='utf-8').close()
         else:
             print(f"File {path} exists, skip it!")
     else:
         if not os.path.isdir(path):
             print(f"Creating directory {path}...")
             os.mkdir(path)
         else:
@@ -73,19 +73,26 @@
     -------
 
     """
     if recipe is None:
         print("recipes: ")
         for i, f in enumerate(list_recipes()):
             recipe_name = re.search("(.*).yml", f)[1]
-            print(f'{i}. {recipe_name}')
+            print(f'{i}. {Path(recipe_name).stem}')
+        return None
+    elif os.path.isfile(f"{base_dir}/recipe/{recipe}.yml"):
+        recipe_file = f"{base_dir}/recipe/{recipe}.yml"
+    elif isinstance(recipe, int) and recipe in range(len(list_recipes())):
+        recipe_file = f"{list_recipes()[recipe]}"
     else:
-        with open(f"{base_dir}/recipe/{recipe}.yml", "r") as f:
-            for line in f:
-                print(line, end="")
+        print("Input recipe is not a valid template name or filename, please check it!")
+        return None
+    with open(recipe_file, "r", encoding='utf-8') as f:
+        for line in f:
+            print(line, end="")
 
 def list_recipes():
     recipes = glob.glob(os.path.join(base_dir,"recipe","*.yml"))
     return recipes
 
 # cooking
 def cook(recipe, name="DEFAULT", destination="."):
@@ -103,25 +110,25 @@
 
     Returns
     -------
 
     """
     if os.path.isfile(recipe):
         recipe_file = recipe
-    elif isinstance(recipe, int) and recipe in range(1, len(list_recipes())):
+    elif isinstance(recipe, int) and recipe in range(len(list_recipes())):
         recipe_file = f"{list_recipes()[recipe]}"
     elif os.path.isfile(f"{base_dir}/recipe/{recipe}.yml"):
         recipe_file = f"{base_dir}/recipe/{recipe}.yml"
     else:
         print("Input recipe is not a valid template name or filename, please check it!")
         return None
     # replace all "DEFAULT" in template with true project name and parse it
     if recipe_file is None:
         return None
-    with open(recipe_file, "r") as f:
+    with open(recipe_file, "r", encoding='utf-8') as f:
         recipe = f.read()
         try:
             recipe = yaml.load(recipe.replace("DEFAULT", name), Loader=yaml.FullLoader)
         except yaml.parser.ParserError:
                 print("Your recipe is poisonous, please check it!")
 
     cookdirs(recipe, root=destination)
```

### Comparing `cookdir-0.1.4/cookdir.egg-info/PKG-INFO` & `cookdir-0.1.5/cookdir.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookdir
-Version: 0.1.4
+Version: 0.1.5
 Summary: create directories by template
 Home-page: https://github.com/Blockhead-yj/cookdir
 Author: yjdai
 Author-email: 136271877@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `cookdir-0.1.4/setup.py` & `cookdir-0.1.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as f:
     long_description = f.read()
 
 print(setuptools.find_packages())
 
 setuptools.setup(
     name="cookdir",
-    version="0.1.4",
+    version="0.1.5",
     author="yjdai",
     author_email="136271877@qq.com",
     description="create directories by template",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Blockhead-yj/cookdir",
     include_package_data=True,
```

