# Comparing `tmp/cfpack-0.0.9.tar.gz` & `tmp/cfpack-0.1.0.tar.gz`

## Comparing `cfpack-0.0.9.tar` & `cfpack-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,11 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 cfpack-0.0.9/.DS_Store
--rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 cfpack-0.0.9/cfpack.browser_control.html
--rw-r--r--   0        0        0    16950 2020-02-02 00:00:00.000000 cfpack-0.0.9/cfpack.html
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cfpack-0.0.9/pyproject.toml.new
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cfpack-0.0.9/pyproject.toml.old
--rw-r--r--   0        0        0    39571 2020-02-02 00:00:00.000000 cfpack-0.0.9/cfpack/__init__.py
--rwxr-xr-x   0        0        0     5243 2020-02-02 00:00:00.000000 cfpack-0.0.9/cfpack/browser_control.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 cfpack-0.0.9/cfpack/constants.py
--rwxr-xr-x   0        0        0     3077 2020-02-02 00:00:00.000000 cfpack-0.0.9/cfpack/hdfio.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 cfpack-0.0.9/cfpack/matplotlibrc.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cfpack-0.0.9/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cfpack-0.0.9/LICENSE
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cfpack-0.0.9/README.md
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cfpack-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 cfpack-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cfpack-0.1.0/pyproject.toml.old
+-rw-r--r--   0        0        0    40075 2020-02-02 00:00:00.000000 cfpack-0.1.0/cfpack/__init__.py
+-rwxr-xr-x   0        0        0     5236 2020-02-02 00:00:00.000000 cfpack-0.1.0/cfpack/browser_control.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 cfpack-0.1.0/cfpack/constants.py
+-rwxr-xr-x   0        0        0     3077 2020-02-02 00:00:00.000000 cfpack-0.1.0/cfpack/hdfio.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 cfpack-0.1.0/cfpack/matplotlibrc.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cfpack-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cfpack-0.1.0/LICENSE
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cfpack-0.1.0/README.md
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cfpack-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 cfpack-0.1.0/PKG-INFO
```

### Comparing `cfpack-0.0.9/pyproject.toml.new` & `cfpack-0.1.0/pyproject.toml.old`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cfpack"
-version = "0.0.7"
+version = "0.0.9"
 authors = [
   { name="Christoph Federrath", email="christoph.federrath@anu.edu.au" },
 ]
 description = "Christoph Federrath (CF) python package (cfpack)"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3"
```

### Comparing `cfpack-0.0.9/pyproject.toml.old` & `cfpack-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cfpack"
-version = "0.0.8"
+version = "0.1.0"
 authors = [
   { name="Christoph Federrath", email="christoph.federrath@anu.edu.au" },
 ]
 description = "Christoph Federrath (CF) python package (cfpack)"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3"
```

### Comparing `cfpack-0.0.9/cfpack/__init__.py` & `cfpack-0.1.0/cfpack/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -348,20 +348,32 @@
     # call recursive func to get all sub-dirs
     dirs = recursive_call(dirname=dirname, verbose=verbose)
     if include_base_dir: dirs = ['.'] + dirs
     dirs = [x+'/' for x in dirs] # add trailing /
     if strip: dirs = [x[2:] for x in dirs]
     return dirs
 
-# === function to search for a string pattern at the start of a line, and to replace that line ===
-def replace_line_in_file(filename, search_str, new_line):
+# === function to search for a string pattern in each line of a file
+# and return that line; or return a list of all the lines that match the search_str ===
+def find_line_in_file(filename, search_str, debug=True):
+    ret = []
+    with open(filename, 'r') as f:
+        for line in f:
+            if line.find(search_str)!=-1:
+                if debug==True: print(filename+": found line   : "+line.rstrip())
+                ret.append(line)
+    if len(ret)==1:
+        ret = ret[0]
+    return ret
+
+# === function to search for a string pattern at the start of a line in a file, and to replace that line ===
+def replace_line_in_file(filename, search_str, new_line, debug=True):
     from tempfile import mkstemp
     from shutil import move
     from os import remove as os_remove, chmod as os_chmod, close as os_close
-    debug = True
     fd, tempfile = mkstemp()
     with open(tempfile, 'w') as ftemp:
         with open(filename, 'r') as f:
             found_line = False
             for line in f:
                 # replace
                 if line.find(search_str)==0:
```

### Comparing `cfpack-0.0.9/cfpack/browser_control.py` & `cfpack-0.1.0/cfpack/browser_control.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     def open(self):
         options = None
         if self.headless:
             options = webdriver.ChromeOptions()
             options.add_argument("headless")
             if self.verbose: print("Running in 'headless' mode...")
         # open driver
-        self.driver = webdriver.Chrome(chrome_options=options)
+        self.driver = webdriver.Chrome(options=options)
 
     # close web driver window
     def close(self):
         self.driver.quit()
 
     # function to load URL
     def load_url(self, url="https://www.mso.anu.edu.au/~chfeder/index.html", wait=None, sleep=None, wait_until_element=""):
```

### Comparing `cfpack-0.0.9/cfpack/constants.py` & `cfpack-0.1.0/cfpack/constants.py`

 * *Files identical despite different names*

### Comparing `cfpack-0.0.9/cfpack/hdfio.py` & `cfpack-0.1.0/cfpack/hdfio.py`

 * *Files identical despite different names*

### Comparing `cfpack-0.0.9/cfpack/matplotlibrc.py` & `cfpack-0.1.0/cfpack/matplotlibrc.py`

 * *Files identical despite different names*

### Comparing `cfpack-0.0.9/LICENSE` & `cfpack-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cfpack-0.0.9/PKG-INFO` & `cfpack-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfpack
-Version: 0.0.9
+Version: 0.1.0
 Summary: Christoph Federrath (CF) python package (cfpack)
 Project-URL: Homepage, https://www.mso.anu.edu.au/~chfeder/codes/cfpack/cfpack.html
 Author-email: Christoph Federrath <christoph.federrath@anu.edu.au>
 License: MIT License
         
         Copyright (c) 2022 Christoph Federrath
```

