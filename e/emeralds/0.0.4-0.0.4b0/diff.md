# Comparing `tmp/emeralds-0.0.4.tar.gz` & `tmp/emeralds-0.0.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emeralds-0.0.4.tar", last modified: Tue Jul 25 06:09:10 2023, max compression
+gzip compressed data, was "emeralds-0.0.4b0.tar", last modified: Tue Jul 25 06:21:51 2023, max compression
```

## Comparing `emeralds-0.0.4.tar` & `emeralds-0.0.4b0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 06:09:10.594354 emeralds-0.0.4/
--rw-rw-rw-   0        0        0     1330 2023-07-24 23:06:47.000000 emeralds-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     1042 2023-07-25 06:09:10.593847 emeralds-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       54 2023-07-24 23:06:47.000000 emeralds-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 06:09:10.560090 emeralds-0.0.4/emeralds/
--rw-rw-rw-   0        0        0        0 2023-07-25 04:13:00.000000 emeralds-0.0.4/emeralds/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 06:09:10.589750 emeralds-0.0.4/emeralds/cryptography/
--rw-rw-rw-   0        0        0      328 2023-07-25 04:28:45.000000 emeralds-0.0.4/emeralds/cryptography/__init__.py
--rw-rw-rw-   0        0        0     2376 2023-07-25 05:59:22.000000 emeralds-0.0.4/emeralds/cryptography/checksums.py
-drwxrwxrwx   0        0        0        0 2023-07-25 06:09:10.592824 emeralds-0.0.4/emeralds/tools/
--rw-rw-rw-   0        0        0      353 2023-07-25 04:28:51.000000 emeralds-0.0.4/emeralds/tools/__init__.py
--rw-rw-rw-   0        0        0     2116 2023-07-22 03:52:54.000000 emeralds-0.0.4/emeralds/tools/colors.py
--rw-rw-rw-   0        0        0     8068 2023-07-25 05:59:29.000000 emeralds-0.0.4/emeralds/tools/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-25 06:09:10.587684 emeralds-0.0.4/emeralds.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-07-25 06:09:10.000000 emeralds-0.0.4/emeralds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-07-25 06:09:10.000000 emeralds-0.0.4/emeralds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 06:09:10.000000 emeralds-0.0.4/emeralds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-25 06:09:10.000000 emeralds-0.0.4/emeralds.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-25 06:09:10.000000 emeralds-0.0.4/emeralds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 06:09:10.594869 emeralds-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     3676 2023-07-25 06:04:53.000000 emeralds-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:21:51.569035 emeralds-0.0.4b0/
+-rw-rw-rw-   0        0        0     1330 2023-07-24 23:06:47.000000 emeralds-0.0.4b0/LICENSE.txt
+-rw-rw-rw-   0        0        0     1102 2023-07-25 06:21:51.569035 emeralds-0.0.4b0/PKG-INFO
+-rw-rw-rw-   0        0        0       54 2023-07-24 23:06:47.000000 emeralds-0.0.4b0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 06:21:51.537027 emeralds-0.0.4b0/emeralds/
+-rw-rw-rw-   0        0        0        0 2023-07-25 04:13:00.000000 emeralds-0.0.4b0/emeralds/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:21:51.565033 emeralds-0.0.4b0/emeralds/cryptography/
+-rw-rw-rw-   0        0        0      328 2023-07-25 04:28:45.000000 emeralds-0.0.4b0/emeralds/cryptography/__init__.py
+-rw-rw-rw-   0        0        0     2376 2023-07-25 05:59:22.000000 emeralds-0.0.4b0/emeralds/cryptography/checksums.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:21:51.567034 emeralds-0.0.4b0/emeralds/tools/
+-rw-rw-rw-   0        0        0      353 2023-07-25 04:28:51.000000 emeralds-0.0.4b0/emeralds/tools/__init__.py
+-rw-rw-rw-   0        0        0     2116 2023-07-22 03:52:54.000000 emeralds-0.0.4b0/emeralds/tools/colors.py
+-rw-rw-rw-   0        0        0     8068 2023-07-25 05:59:29.000000 emeralds-0.0.4b0/emeralds/tools/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:21:51.563032 emeralds-0.0.4b0/emeralds.egg-info/
+-rw-rw-rw-   0        0        0     1102 2023-07-25 06:21:51.000000 emeralds-0.0.4b0/emeralds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-07-25 06:21:51.000000 emeralds-0.0.4b0/emeralds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 06:21:51.000000 emeralds-0.0.4b0/emeralds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-25 06:21:51.000000 emeralds-0.0.4b0/emeralds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-25 06:21:51.000000 emeralds-0.0.4b0/emeralds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 06:21:51.569035 emeralds-0.0.4b0/setup.cfg
+-rw-rw-rw-   0        0        0     3975 2023-07-25 06:21:28.000000 emeralds-0.0.4b0/setup.py
```

### Comparing `emeralds-0.0.4/LICENSE.txt` & `emeralds-0.0.4b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `emeralds-0.0.4/PKG-INFO` & `emeralds-0.0.4b0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emeralds
-Version: 0.0.4
+Version: 0.0.4b0
 Summary: A testing package for learning PyPi.
 Home-page: https://github.com/jasondrawdy/emeralds
 Author: Jason Drawdy
 Author-email: <40871836+jasondrawdy@users.noreply.github.com>
 Project-URL: Documentation, https://emeralds.readthedocs.io/en/latest/
 Keywords: emeralds,test,package
 Classifier: Development Status :: 1 - Planning
@@ -20,7 +20,9 @@
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # Emeralds
 A small libary for testing package uploads
+
+Built by Autumn (Jason's AI) — 2023-07-25 @ 02:21:51
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `emeralds-0.0.4/emeralds/cryptography/checksums.py` & `emeralds-0.0.4b0/emeralds/cryptography/checksums.py`

 * *Files identical despite different names*

### Comparing `emeralds-0.0.4/emeralds/tools/colors.py` & `emeralds-0.0.4b0/emeralds/tools/colors.py`

 * *Files identical despite different names*

### Comparing `emeralds-0.0.4/emeralds/tools/logger.py` & `emeralds-0.0.4b0/emeralds/tools/logger.py`

 * *Files identical despite different names*

### Comparing `emeralds-0.0.4/emeralds.egg-info/PKG-INFO` & `emeralds-0.0.4b0/emeralds.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emeralds
-Version: 0.0.4
+Version: 0.0.4b0
 Summary: A testing package for learning PyPi.
 Home-page: https://github.com/jasondrawdy/emeralds
 Author: Jason Drawdy
 Author-email: <40871836+jasondrawdy@users.noreply.github.com>
 Project-URL: Documentation, https://emeralds.readthedocs.io/en/latest/
 Keywords: emeralds,test,package
 Classifier: Development Status :: 1 - Planning
@@ -20,7 +20,9 @@
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # Emeralds
 A small libary for testing package uploads
+
+Built by Autumn (Jason's AI) — 2023-07-25 @ 02:21:51
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `emeralds-0.0.4/setup.py` & `emeralds-0.0.4b0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,77 +6,78 @@
 # Date: 07/21/23
 # #########################################################################
 # Description:
 # Contains all classes and functions for creating a complete pip package.
 # #########################################################################
 from setuptools import setup, find_packages
 import datetime
-import zipfile
-import hashlib
-import shutil
 import codecs
 import os
 
 class InstallHelper:
     """A encapsulation object containing all necessary components for creating a pip package."""
     def __init__(self: "InstallHelper") -> None:
         self.package = "emeralds"
         self.author = "Jason Drawdy"
         self.email = "<40871836+jasondrawdy@users.noreply.github.com>"
         self.website = "https://github.com/jasondrawdy/emeralds"
         self.references = {"Documentation": "https://emeralds.readthedocs.io/en/latest/"}
-        self.version = '0.0.4'
+        self.version = '0.0.4b'
         self.description = 'A testing package for learning PyPi.'
         self.long_description = self._get_project_readme()
 
     def _get_project_readme(self: "InstallHelper"):
         """Returns the current README documentation or a default description."""
         default_data = 'Cool package for testing!'
         current_path = os.path.abspath(os.path.dirname(__file__))
         readme_file = os.path.join(current_path, "README.md")
         if os.path.exists(readme_file):
             with codecs.open(readme_file, encoding="utf-8") as file:
                 return file.read()
         return default_data 
 
-    def prepare_for_packaging(self: "InstallHelper"):
+    def prepare_for_archiving(self: "InstallHelper"):
         """Temporarily modifies the current project structure for more accurate packaging."""
         os.rename('src', self.package)
 
     def restore_original_structure(self: "InstallHelper"):
         """Creates the original file and directory structure before the creation of any packages."""
         os.rename(self.package, 'src')
     
     def create_project_package(self: "InstallHelper"):
         """Performs the actual package creation process using all provided `setup()` function information."""
-        setup(
-            name=self.package,
-            version=self.version,
-            author=self.author,
-            author_email=self.email,
-            description=self.description,
-            long_description_content_type="text/markdown",
-            long_description=self.long_description,
-            url=self.website,
-            project_urls=self.references,
-            packages=find_packages(),
-            extras_require={'dev': ['twine', 'sphinx', 'sphinx-rtd-theme', 'sphinx-autoapi']},
-            keywords=['emeralds', 'test', 'package'],
-            classifiers=[
-                "Development Status :: 1 - Planning",
-                "Intended Audience :: Developers",
-                "License :: OSI Approved :: MIT License",
-                "Programming Language :: Python :: 3",
-                "Programming Language :: Python :: 3.6",
-                "Programming Language :: Python :: 3.7",
-                "Programming Language :: Python :: 3.8",
-                "Programming Language :: Python :: 3.9",
-                "Programming Language :: Python :: 3.10",
-                "Programming Language :: Python :: 3.11",
-                "Operating System :: OS Independent",
-            ]
-        )
+        timestamp = datetime.datetime.now().strftime("%Y-%m-%d @ %H:%M:%S")
+        self.long_description += f"\n\nBuilt by Autumn (Jason's AI) — {timestamp}"
+        try:
+            setup(
+                name=self.package,
+                version=self.version,
+                author=self.author,
+                author_email=self.email,
+                description=self.description,
+                long_description_content_type="text/markdown",
+                long_description=self.long_description,
+                url=self.website,
+                project_urls=self.references,
+                packages=find_packages(),
+                extras_require={'dev': ['twine', 'sphinx', 'sphinx-rtd-theme', 'sphinx-autoapi']},
+                keywords=['emeralds', 'test', 'package'],
+                classifiers=[
+                    "Development Status :: 1 - Planning",
+                    "Intended Audience :: Developers",
+                    "License :: OSI Approved :: MIT License",
+                    "Programming Language :: Python :: 3",
+                    "Programming Language :: Python :: 3.6",
+                    "Programming Language :: Python :: 3.7",
+                    "Programming Language :: Python :: 3.8",
+                    "Programming Language :: Python :: 3.9",
+                    "Programming Language :: Python :: 3.10",
+                    "Programming Language :: Python :: 3.11",
+                    "Operating System :: OS Independent",
+                ]
+            )
+        except: pass # Cleanup will be called after setup.
 
 packager = InstallHelper()
-packager.prepare_for_packaging()
+packager.prepare_for_archiving()
 packager.create_project_package()
 packager.restore_original_structure()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

