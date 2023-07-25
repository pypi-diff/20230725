# Comparing `tmp/emeralds-0.0.3.tar.gz` & `tmp/emeralds-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emeralds-0.0.3.tar", last modified: Tue Jul 25 05:29:05 2023, max compression
+gzip compressed data, was "emeralds-0.0.4.tar", last modified: Tue Jul 25 06:09:10 2023, max compression
```

## Comparing `emeralds-0.0.3.tar` & `emeralds-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 05:29:05.165897 emeralds-0.0.3/
--rw-rw-rw-   0        0        0     1330 2023-07-24 23:06:47.000000 emeralds-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     1042 2023-07-25 05:29:05.165897 emeralds-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       54 2023-07-24 23:06:47.000000 emeralds-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 05:29:05.133890 emeralds-0.0.3/emeralds/
--rw-rw-rw-   0        0        0        0 2023-07-25 04:13:00.000000 emeralds-0.0.3/emeralds/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 05:29:05.161896 emeralds-0.0.3/emeralds/cryptography/
--rw-rw-rw-   0        0        0      328 2023-07-25 04:28:45.000000 emeralds-0.0.3/emeralds/cryptography/__init__.py
--rw-rw-rw-   0        0        0     2378 2023-07-23 02:58:28.000000 emeralds-0.0.3/emeralds/cryptography/checksums.py
-drwxrwxrwx   0        0        0        0 2023-07-25 05:29:05.163896 emeralds-0.0.3/emeralds/tools/
--rw-rw-rw-   0        0        0      353 2023-07-25 04:28:51.000000 emeralds-0.0.3/emeralds/tools/__init__.py
--rw-rw-rw-   0        0        0     2116 2023-07-22 03:52:54.000000 emeralds-0.0.3/emeralds/tools/colors.py
--rw-rw-rw-   0        0        0     8070 2023-07-22 03:52:58.000000 emeralds-0.0.3/emeralds/tools/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-25 05:29:05.158895 emeralds-0.0.3/emeralds.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-07-25 05:29:05.000000 emeralds-0.0.3/emeralds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-07-25 05:29:05.000000 emeralds-0.0.3/emeralds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 05:29:05.000000 emeralds-0.0.3/emeralds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-25 05:29:05.000000 emeralds-0.0.3/emeralds.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-25 05:29:05.000000 emeralds-0.0.3/emeralds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 05:29:05.166897 emeralds-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     3676 2023-07-25 05:29:01.000000 emeralds-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:09:10.594354 emeralds-0.0.4/
+-rw-rw-rw-   0        0        0     1330 2023-07-24 23:06:47.000000 emeralds-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     1042 2023-07-25 06:09:10.593847 emeralds-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       54 2023-07-24 23:06:47.000000 emeralds-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 06:09:10.560090 emeralds-0.0.4/emeralds/
+-rw-rw-rw-   0        0        0        0 2023-07-25 04:13:00.000000 emeralds-0.0.4/emeralds/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:09:10.589750 emeralds-0.0.4/emeralds/cryptography/
+-rw-rw-rw-   0        0        0      328 2023-07-25 04:28:45.000000 emeralds-0.0.4/emeralds/cryptography/__init__.py
+-rw-rw-rw-   0        0        0     2376 2023-07-25 05:59:22.000000 emeralds-0.0.4/emeralds/cryptography/checksums.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:09:10.592824 emeralds-0.0.4/emeralds/tools/
+-rw-rw-rw-   0        0        0      353 2023-07-25 04:28:51.000000 emeralds-0.0.4/emeralds/tools/__init__.py
+-rw-rw-rw-   0        0        0     2116 2023-07-22 03:52:54.000000 emeralds-0.0.4/emeralds/tools/colors.py
+-rw-rw-rw-   0        0        0     8068 2023-07-25 05:59:29.000000 emeralds-0.0.4/emeralds/tools/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:09:10.587684 emeralds-0.0.4/emeralds.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-07-25 06:09:10.000000 emeralds-0.0.4/emeralds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-07-25 06:09:10.000000 emeralds-0.0.4/emeralds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 06:09:10.000000 emeralds-0.0.4/emeralds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-25 06:09:10.000000 emeralds-0.0.4/emeralds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-25 06:09:10.000000 emeralds-0.0.4/emeralds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 06:09:10.594869 emeralds-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     3676 2023-07-25 06:04:53.000000 emeralds-0.0.4/setup.py
```

### Comparing `emeralds-0.0.3/LICENSE.txt` & `emeralds-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `emeralds-0.0.3/PKG-INFO` & `emeralds-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emeralds
-Version: 0.0.3
+Version: 0.0.4
 Summary: A testing package for learning PyPi.
 Home-page: https://github.com/jasondrawdy/emeralds
 Author: Jason Drawdy
 Author-email: <40871836+jasondrawdy@users.noreply.github.com>
 Project-URL: Documentation, https://emeralds.readthedocs.io/en/latest/
 Keywords: emeralds,test,package
 Classifier: Development Status :: 1 - Planning
```

### Comparing `emeralds-0.0.3/emeralds/cryptography/checksums.py` & `emeralds-0.0.4/emeralds/cryptography/checksums.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Author: Jason Drawdy
 # Version: 0.0.1
 # Date: 07/21/23
 # #########################################################################
 # Description:
 # Allows the generation of checksums from binary data.
 # #########################################################################
-from src.tools.logger import Logger
+from ..tools.logger import Logger
 import hashlib
 
 class Hasher:
     """Allows checksum generation of binary data either from a file or message."""
     def __init__(self) -> None:
         """Creates a new hashing object instance to allow checksum generation of files and messages."""
         self._logger = Logger(__name__)
```

### Comparing `emeralds-0.0.3/emeralds/tools/colors.py` & `emeralds-0.0.4/emeralds/tools/colors.py`

 * *Files identical despite different names*

### Comparing `emeralds-0.0.3/emeralds/tools/logger.py` & `emeralds-0.0.4/emeralds/tools/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Author: Jason Drawdy
 # Version: 0.0.1
 # Date: 07/21/23
 # #########################################################################
 # Description:
 # This module allows customized logging of all i/o throughout Emeralds.
 # #########################################################################
-from src.tools.colors import Colors
+from ..tools.colors import Colors
 from dataclasses import dataclass
 from datetime import datetime
 
 class Logger(object):
     """Logging class with a high degree of customization."""
     @dataclass(frozen=True)
     class Verbosity():
```

### Comparing `emeralds-0.0.3/emeralds.egg-info/PKG-INFO` & `emeralds-0.0.4/emeralds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emeralds
-Version: 0.0.3
+Version: 0.0.4
 Summary: A testing package for learning PyPi.
 Home-page: https://github.com/jasondrawdy/emeralds
 Author: Jason Drawdy
 Author-email: <40871836+jasondrawdy@users.noreply.github.com>
 Project-URL: Documentation, https://emeralds.readthedocs.io/en/latest/
 Keywords: emeralds,test,package
 Classifier: Development Status :: 1 - Planning
```

### Comparing `emeralds-0.0.3/setup.py` & `emeralds-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     """A encapsulation object containing all necessary components for creating a pip package."""
     def __init__(self: "InstallHelper") -> None:
         self.package = "emeralds"
         self.author = "Jason Drawdy"
         self.email = "<40871836+jasondrawdy@users.noreply.github.com>"
         self.website = "https://github.com/jasondrawdy/emeralds"
         self.references = {"Documentation": "https://emeralds.readthedocs.io/en/latest/"}
-        self.version = '0.0.3'
+        self.version = '0.0.4'
         self.description = 'A testing package for learning PyPi.'
         self.long_description = self._get_project_readme()
 
     def _get_project_readme(self: "InstallHelper"):
         """Returns the current README documentation or a default description."""
         default_data = 'Cool package for testing!'
         current_path = os.path.abspath(os.path.dirname(__file__))
```

