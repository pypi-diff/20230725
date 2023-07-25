# Comparing `tmp/emeralds-0.0.2.tar.gz` & `tmp/emeralds-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emeralds-0.0.2.tar", last modified: Tue Jul 25 04:41:34 2023, max compression
+gzip compressed data, was "emeralds-0.0.3.tar", last modified: Tue Jul 25 05:29:05 2023, max compression
```

## Comparing `emeralds-0.0.2.tar` & `emeralds-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 04:41:34.990831 emeralds-0.0.2/
--rw-rw-rw-   0        0        0     1330 2023-07-24 23:06:47.000000 emeralds-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      970 2023-07-25 04:41:34.990831 emeralds-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       54 2023-07-24 23:06:47.000000 emeralds-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 04:41:34.957824 emeralds-0.0.2/emeralds/
--rw-rw-rw-   0        0        0        0 2023-07-25 04:13:00.000000 emeralds-0.0.2/emeralds/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 04:41:34.986830 emeralds-0.0.2/emeralds/cryptography/
--rw-rw-rw-   0        0        0      328 2023-07-25 04:28:45.000000 emeralds-0.0.2/emeralds/cryptography/__init__.py
--rw-rw-rw-   0        0        0     2378 2023-07-23 02:58:28.000000 emeralds-0.0.2/emeralds/cryptography/checksums.py
-drwxrwxrwx   0        0        0        0 2023-07-25 04:41:34.988830 emeralds-0.0.2/emeralds/tools/
--rw-rw-rw-   0        0        0      353 2023-07-25 04:28:51.000000 emeralds-0.0.2/emeralds/tools/__init__.py
--rw-rw-rw-   0        0        0     2116 2023-07-22 03:52:54.000000 emeralds-0.0.2/emeralds/tools/colors.py
--rw-rw-rw-   0        0        0     8070 2023-07-22 03:52:58.000000 emeralds-0.0.2/emeralds/tools/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-25 04:41:34.984830 emeralds-0.0.2/emeralds.egg-info/
--rw-rw-rw-   0        0        0      970 2023-07-25 04:41:34.000000 emeralds-0.0.2/emeralds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-07-25 04:41:34.000000 emeralds-0.0.2/emeralds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 04:41:34.000000 emeralds-0.0.2/emeralds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-25 04:41:34.000000 emeralds-0.0.2/emeralds.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-25 04:41:34.000000 emeralds-0.0.2/emeralds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 04:41:34.990831 emeralds-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     3542 2023-07-25 04:40:58.000000 emeralds-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 05:29:05.165897 emeralds-0.0.3/
+-rw-rw-rw-   0        0        0     1330 2023-07-24 23:06:47.000000 emeralds-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1042 2023-07-25 05:29:05.165897 emeralds-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       54 2023-07-24 23:06:47.000000 emeralds-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 05:29:05.133890 emeralds-0.0.3/emeralds/
+-rw-rw-rw-   0        0        0        0 2023-07-25 04:13:00.000000 emeralds-0.0.3/emeralds/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 05:29:05.161896 emeralds-0.0.3/emeralds/cryptography/
+-rw-rw-rw-   0        0        0      328 2023-07-25 04:28:45.000000 emeralds-0.0.3/emeralds/cryptography/__init__.py
+-rw-rw-rw-   0        0        0     2378 2023-07-23 02:58:28.000000 emeralds-0.0.3/emeralds/cryptography/checksums.py
+drwxrwxrwx   0        0        0        0 2023-07-25 05:29:05.163896 emeralds-0.0.3/emeralds/tools/
+-rw-rw-rw-   0        0        0      353 2023-07-25 04:28:51.000000 emeralds-0.0.3/emeralds/tools/__init__.py
+-rw-rw-rw-   0        0        0     2116 2023-07-22 03:52:54.000000 emeralds-0.0.3/emeralds/tools/colors.py
+-rw-rw-rw-   0        0        0     8070 2023-07-22 03:52:58.000000 emeralds-0.0.3/emeralds/tools/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-25 05:29:05.158895 emeralds-0.0.3/emeralds.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-07-25 05:29:05.000000 emeralds-0.0.3/emeralds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-07-25 05:29:05.000000 emeralds-0.0.3/emeralds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 05:29:05.000000 emeralds-0.0.3/emeralds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-25 05:29:05.000000 emeralds-0.0.3/emeralds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-25 05:29:05.000000 emeralds-0.0.3/emeralds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 05:29:05.166897 emeralds-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     3676 2023-07-25 05:29:01.000000 emeralds-0.0.3/setup.py
```

### Comparing `emeralds-0.0.2/LICENSE.txt` & `emeralds-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `emeralds-0.0.2/emeralds/cryptography/checksums.py` & `emeralds-0.0.3/emeralds/cryptography/checksums.py`

 * *Files identical despite different names*

### Comparing `emeralds-0.0.2/emeralds/tools/colors.py` & `emeralds-0.0.3/emeralds/tools/colors.py`

 * *Files identical despite different names*

### Comparing `emeralds-0.0.2/emeralds/tools/logger.py` & `emeralds-0.0.3/emeralds/tools/logger.py`

 * *Files identical despite different names*

### Comparing `emeralds-0.0.2/setup.py` & `emeralds-0.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 class InstallHelper:
     """A encapsulation object containing all necessary components for creating a pip package."""
     def __init__(self: "InstallHelper") -> None:
         self.package = "emeralds"
         self.author = "Jason Drawdy"
         self.email = "<40871836+jasondrawdy@users.noreply.github.com>"
         self.website = "https://github.com/jasondrawdy/emeralds"
-        self.version = '0.0.2'
+        self.references = {"Documentation": "https://emeralds.readthedocs.io/en/latest/"}
+        self.version = '0.0.3'
         self.description = 'A testing package for learning PyPi.'
         self.long_description = self._get_project_readme()
 
     def _get_project_readme(self: "InstallHelper"):
         """Returns the current README documentation or a default description."""
         default_data = 'Cool package for testing!'
         current_path = os.path.abspath(os.path.dirname(__file__))
@@ -52,14 +53,15 @@
             version=self.version,
             author=self.author,
             author_email=self.email,
             description=self.description,
             long_description_content_type="text/markdown",
             long_description=self.long_description,
             url=self.website,
+            project_urls=self.references,
             packages=find_packages(),
             extras_require={'dev': ['twine', 'sphinx', 'sphinx-rtd-theme', 'sphinx-autoapi']},
             keywords=['emeralds', 'test', 'package'],
             classifiers=[
                 "Development Status :: 1 - Planning",
                 "Intended Audience :: Developers",
                 "License :: OSI Approved :: MIT License",
```

