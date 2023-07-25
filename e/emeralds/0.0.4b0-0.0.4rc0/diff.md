# Comparing `tmp/emeralds-0.0.4b0.tar.gz` & `tmp/emeralds-0.0.4rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emeralds-0.0.4b0.tar", last modified: Tue Jul 25 06:21:51 2023, max compression
+gzip compressed data, was "emeralds-0.0.4rc0.tar", last modified: Tue Jul 25 06:26:38 2023, max compression
```

## Comparing `emeralds-0.0.4b0.tar` & `emeralds-0.0.4rc0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 06:21:51.569035 emeralds-0.0.4b0/
--rw-rw-rw-   0        0        0     1330 2023-07-24 23:06:47.000000 emeralds-0.0.4b0/LICENSE.txt
--rw-rw-rw-   0        0        0     1102 2023-07-25 06:21:51.569035 emeralds-0.0.4b0/PKG-INFO
--rw-rw-rw-   0        0        0       54 2023-07-24 23:06:47.000000 emeralds-0.0.4b0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 06:21:51.537027 emeralds-0.0.4b0/emeralds/
--rw-rw-rw-   0        0        0        0 2023-07-25 04:13:00.000000 emeralds-0.0.4b0/emeralds/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 06:21:51.565033 emeralds-0.0.4b0/emeralds/cryptography/
--rw-rw-rw-   0        0        0      328 2023-07-25 04:28:45.000000 emeralds-0.0.4b0/emeralds/cryptography/__init__.py
--rw-rw-rw-   0        0        0     2376 2023-07-25 05:59:22.000000 emeralds-0.0.4b0/emeralds/cryptography/checksums.py
-drwxrwxrwx   0        0        0        0 2023-07-25 06:21:51.567034 emeralds-0.0.4b0/emeralds/tools/
--rw-rw-rw-   0        0        0      353 2023-07-25 04:28:51.000000 emeralds-0.0.4b0/emeralds/tools/__init__.py
--rw-rw-rw-   0        0        0     2116 2023-07-22 03:52:54.000000 emeralds-0.0.4b0/emeralds/tools/colors.py
--rw-rw-rw-   0        0        0     8068 2023-07-25 05:59:29.000000 emeralds-0.0.4b0/emeralds/tools/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-25 06:21:51.563032 emeralds-0.0.4b0/emeralds.egg-info/
--rw-rw-rw-   0        0        0     1102 2023-07-25 06:21:51.000000 emeralds-0.0.4b0/emeralds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-07-25 06:21:51.000000 emeralds-0.0.4b0/emeralds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 06:21:51.000000 emeralds-0.0.4b0/emeralds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-25 06:21:51.000000 emeralds-0.0.4b0/emeralds.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-25 06:21:51.000000 emeralds-0.0.4b0/emeralds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 06:21:51.569035 emeralds-0.0.4b0/setup.cfg
--rw-rw-rw-   0        0        0     3975 2023-07-25 06:21:28.000000 emeralds-0.0.4b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:26:38.241876 emeralds-0.0.4rc0/
+-rw-rw-rw-   0        0        0     1330 2023-07-24 23:06:47.000000 emeralds-0.0.4rc0/LICENSE.txt
+-rw-rw-rw-   0        0        0     1107 2023-07-25 06:26:38.240876 emeralds-0.0.4rc0/PKG-INFO
+-rw-rw-rw-   0        0        0       54 2023-07-24 23:06:47.000000 emeralds-0.0.4rc0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 06:26:38.214870 emeralds-0.0.4rc0/emeralds/
+-rw-rw-rw-   0        0        0        0 2023-07-25 04:13:00.000000 emeralds-0.0.4rc0/emeralds/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:26:38.236875 emeralds-0.0.4rc0/emeralds/cryptography/
+-rw-rw-rw-   0        0        0      328 2023-07-25 04:28:45.000000 emeralds-0.0.4rc0/emeralds/cryptography/__init__.py
+-rw-rw-rw-   0        0        0     2376 2023-07-25 05:59:22.000000 emeralds-0.0.4rc0/emeralds/cryptography/checksums.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:26:38.239876 emeralds-0.0.4rc0/emeralds/tools/
+-rw-rw-rw-   0        0        0      353 2023-07-25 04:28:51.000000 emeralds-0.0.4rc0/emeralds/tools/__init__.py
+-rw-rw-rw-   0        0        0     2116 2023-07-22 03:52:54.000000 emeralds-0.0.4rc0/emeralds/tools/colors.py
+-rw-rw-rw-   0        0        0     8068 2023-07-25 05:59:29.000000 emeralds-0.0.4rc0/emeralds/tools/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:26:38.234874 emeralds-0.0.4rc0/emeralds.egg-info/
+-rw-rw-rw-   0        0        0     1107 2023-07-25 06:26:38.000000 emeralds-0.0.4rc0/emeralds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-07-25 06:26:38.000000 emeralds-0.0.4rc0/emeralds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 06:26:38.000000 emeralds-0.0.4rc0/emeralds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-25 06:26:38.000000 emeralds-0.0.4rc0/emeralds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-25 06:26:38.000000 emeralds-0.0.4rc0/emeralds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 06:26:38.241876 emeralds-0.0.4rc0/setup.cfg
+-rw-rw-rw-   0        0        0     3979 2023-07-25 06:25:22.000000 emeralds-0.0.4rc0/setup.py
```

### Comparing `emeralds-0.0.4b0/LICENSE.txt` & `emeralds-0.0.4rc0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `emeralds-0.0.4b0/PKG-INFO` & `emeralds-0.0.4rc0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emeralds
-Version: 0.0.4b0
+Version: 0.0.4rc0
 Summary: A testing package for learning PyPi.
 Home-page: https://github.com/jasondrawdy/emeralds
 Author: Jason Drawdy
 Author-email: <40871836+jasondrawdy@users.noreply.github.com>
 Project-URL: Documentation, https://emeralds.readthedocs.io/en/latest/
 Keywords: emeralds,test,package
 Classifier: Development Status :: 1 - Planning
@@ -20,9 +20,8 @@
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # Emeralds
 A small libary for testing package uploads
-
-Built by Autumn (Jason's AI) — 2023-07-25 @ 02:21:51
+\Packaged with Autumn (Jason's AI) — 2023-07-25 @ 02:26:38
```

### Comparing `emeralds-0.0.4b0/emeralds/cryptography/checksums.py` & `emeralds-0.0.4rc0/emeralds/cryptography/checksums.py`

 * *Files identical despite different names*

### Comparing `emeralds-0.0.4b0/emeralds/tools/colors.py` & `emeralds-0.0.4rc0/emeralds/tools/colors.py`

 * *Files identical despite different names*

### Comparing `emeralds-0.0.4b0/emeralds/tools/logger.py` & `emeralds-0.0.4rc0/emeralds/tools/logger.py`

 * *Files identical despite different names*

### Comparing `emeralds-0.0.4b0/emeralds.egg-info/PKG-INFO` & `emeralds-0.0.4rc0/emeralds.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emeralds
-Version: 0.0.4b0
+Version: 0.0.4rc0
 Summary: A testing package for learning PyPi.
 Home-page: https://github.com/jasondrawdy/emeralds
 Author: Jason Drawdy
 Author-email: <40871836+jasondrawdy@users.noreply.github.com>
 Project-URL: Documentation, https://emeralds.readthedocs.io/en/latest/
 Keywords: emeralds,test,package
 Classifier: Development Status :: 1 - Planning
@@ -20,9 +20,8 @@
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # Emeralds
 A small libary for testing package uploads
-
-Built by Autumn (Jason's AI) — 2023-07-25 @ 02:21:51
+\Packaged with Autumn (Jason's AI) — 2023-07-25 @ 02:26:38
```

### Comparing `emeralds-0.0.4b0/setup.py` & `emeralds-0.0.4rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     """A encapsulation object containing all necessary components for creating a pip package."""
     def __init__(self: "InstallHelper") -> None:
         self.package = "emeralds"
         self.author = "Jason Drawdy"
         self.email = "<40871836+jasondrawdy@users.noreply.github.com>"
         self.website = "https://github.com/jasondrawdy/emeralds"
         self.references = {"Documentation": "https://emeralds.readthedocs.io/en/latest/"}
-        self.version = '0.0.4b'
+        self.version = '0.0.4c'
         self.description = 'A testing package for learning PyPi.'
         self.long_description = self._get_project_readme()
 
     def _get_project_readme(self: "InstallHelper"):
         """Returns the current README documentation or a default description."""
         default_data = 'Cool package for testing!'
         current_path = os.path.abspath(os.path.dirname(__file__))
@@ -42,15 +42,15 @@
     def restore_original_structure(self: "InstallHelper"):
         """Creates the original file and directory structure before the creation of any packages."""
         os.rename(self.package, 'src')
     
     def create_project_package(self: "InstallHelper"):
         """Performs the actual package creation process using all provided `setup()` function information."""
         timestamp = datetime.datetime.now().strftime("%Y-%m-%d @ %H:%M:%S")
-        self.long_description += f"\n\nBuilt by Autumn (Jason's AI) — {timestamp}"
+        self.long_description += f"\n\Packaged with Autumn (Jason's AI) — {timestamp}"
         try:
             setup(
                 name=self.package,
                 version=self.version,
                 author=self.author,
                 author_email=self.email,
                 description=self.description,
```

