# Comparing `tmp/pyDuotecno-2023.7.2.tar.gz` & `tmp/pyDuotecno-2023.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDuotecno-2023.7.2.tar", last modified: Tue Jul 25 05:30:42 2023, max compression
+gzip compressed data, was "pyDuotecno-2023.7.3.tar", last modified: Tue Jul 25 05:50:55 2023, max compression
```

## Comparing `pyDuotecno-2023.7.2.tar` & `pyDuotecno-2023.7.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-25 05:30:42.527284 pyDuotecno-2023.7.2/
--rw-r--r--   0 cereal    (1000) cereal    (1000)    11357 2023-04-01 07:58:16.000000 pyDuotecno-2023.7.2/LICENSE
--rw-r--r--   0 cereal    (1000) cereal    (1000)       73 2023-05-08 15:34:58.000000 pyDuotecno-2023.7.2/MANIFEST.in
--rw-r--r--   0 cereal    (1000) cereal    (1000)     1221 2023-07-25 05:30:42.527284 pyDuotecno-2023.7.2/PKG-INFO
--rw-r--r--   0 cereal    (1000) cereal    (1000)      155 2023-05-05 12:02:57.000000 pyDuotecno-2023.7.2/README.md
-drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-25 05:30:42.503950 pyDuotecno-2023.7.2/duotecno/
--rw-r--r--   0 cereal    (1000) cereal    (1000)     5254 2023-07-11 13:07:49.000000 pyDuotecno-2023.7.2/duotecno/controller.py
--rw-r--r--   0 cereal    (1000) cereal    (1000)      125 2023-07-25 04:44:21.000000 pyDuotecno-2023.7.2/duotecno/exceptions.py
--rw-r--r--   0 cereal    (1000) cereal    (1000)     2909 2023-07-11 13:11:31.000000 pyDuotecno-2023.7.2/duotecno/node.py
--rw-r--r--   0 cereal    (1000) cereal    (1000)     7610 2023-05-15 11:00:00.000000 pyDuotecno-2023.7.2/duotecno/protocol.py
--rw-r--r--   0 cereal    (1000) cereal    (1000)     4395 2023-07-25 04:46:29.000000 pyDuotecno-2023.7.2/duotecno/unit.py
-drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-25 05:30:42.503950 pyDuotecno-2023.7.2/examples/
--rw-r--r--   0 cereal    (1000) cereal    (1000)      765 2023-04-14 17:55:06.000000 pyDuotecno-2023.7.2/examples/read.py
-drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-25 05:30:42.510617 pyDuotecno-2023.7.2/pyDuotecno.egg-info/
--rw-r--r--   0 cereal    (1000) cereal    (1000)     1221 2023-07-25 05:30:42.000000 pyDuotecno-2023.7.2/pyDuotecno.egg-info/PKG-INFO
--rw-r--r--   0 cereal    (1000) cereal    (1000)      626 2023-07-25 05:30:42.000000 pyDuotecno-2023.7.2/pyDuotecno.egg-info/SOURCES.txt
--rw-r--r--   0 cereal    (1000) cereal    (1000)        1 2023-07-25 05:30:42.000000 pyDuotecno-2023.7.2/pyDuotecno.egg-info/dependency_links.txt
--rw-r--r--   0 cereal    (1000) cereal    (1000)        1 2023-04-01 08:06:22.000000 pyDuotecno-2023.7.2/pyDuotecno.egg-info/not-zip-safe
--rw-r--r--   0 cereal    (1000) cereal    (1000)       28 2023-07-25 05:30:42.000000 pyDuotecno-2023.7.2/pyDuotecno.egg-info/top_level.txt
--rw-r--r--   0 cereal    (1000) cereal    (1000)     1682 2023-07-25 04:44:46.000000 pyDuotecno-2023.7.2/pyproject.toml
--rw-r--r--   0 cereal    (1000) cereal    (1000)        0 2023-04-01 07:56:09.000000 pyDuotecno-2023.7.2/requirements.txt
--rw-r--r--   0 cereal    (1000) cereal    (1000)       38 2023-07-25 05:30:42.527284 pyDuotecno-2023.7.2/setup.cfg
--rw-r--r--   0 cereal    (1000) cereal    (1000)       72 2023-04-01 08:10:33.000000 pyDuotecno-2023.7.2/setup.py
-drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-25 05:30:42.493949 pyDuotecno-2023.7.2/venv/
-drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-25 05:30:42.527284 pyDuotecno-2023.7.2/venv/bin/
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)      616 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.2/venv/bin/rst2html.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)      738 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.2/venv/bin/rst2html4.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)     1083 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.2/venv/bin/rst2html5.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)      815 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.2/venv/bin/rst2latex.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)      638 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.2/venv/bin/rst2man.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)      804 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.2/venv/bin/rst2odt.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)     1742 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.2/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)      623 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.2/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)      659 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.2/venv/bin/rst2s5.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)      895 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.2/venv/bin/rst2xetex.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)      624 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.2/venv/bin/rst2xml.py
--rwxr-xr-x   0 cereal    (1000) cereal    (1000)      692 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.2/venv/bin/rstpep2html.py
+drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-25 05:50:55.203315 pyDuotecno-2023.7.3/
+-rw-r--r--   0 cereal    (1000) cereal    (1000)    11357 2023-04-01 07:58:16.000000 pyDuotecno-2023.7.3/LICENSE
+-rw-r--r--   0 cereal    (1000) cereal    (1000)       73 2023-05-08 15:34:58.000000 pyDuotecno-2023.7.3/MANIFEST.in
+-rw-r--r--   0 cereal    (1000) cereal    (1000)     1119 2023-07-25 05:50:55.199981 pyDuotecno-2023.7.3/PKG-INFO
+-rw-r--r--   0 cereal    (1000) cereal    (1000)       53 2023-07-25 05:45:41.000000 pyDuotecno-2023.7.3/README.md
+drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-25 05:50:55.173313 pyDuotecno-2023.7.3/duotecno/
+-rw-r--r--   0 cereal    (1000) cereal    (1000)     5252 2023-07-25 05:50:01.000000 pyDuotecno-2023.7.3/duotecno/controller.py
+-rw-r--r--   0 cereal    (1000) cereal    (1000)      125 2023-07-25 04:44:21.000000 pyDuotecno-2023.7.3/duotecno/exceptions.py
+-rw-r--r--   0 cereal    (1000) cereal    (1000)     2909 2023-07-11 13:11:31.000000 pyDuotecno-2023.7.3/duotecno/node.py
+-rw-r--r--   0 cereal    (1000) cereal    (1000)     7610 2023-05-15 11:00:00.000000 pyDuotecno-2023.7.3/duotecno/protocol.py
+-rw-r--r--   0 cereal    (1000) cereal    (1000)     4395 2023-07-25 04:46:29.000000 pyDuotecno-2023.7.3/duotecno/unit.py
+drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-25 05:50:55.176646 pyDuotecno-2023.7.3/examples/
+-rw-r--r--   0 cereal    (1000) cereal    (1000)      765 2023-04-14 17:55:06.000000 pyDuotecno-2023.7.3/examples/read.py
+drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-25 05:50:55.183313 pyDuotecno-2023.7.3/pyDuotecno.egg-info/
+-rw-r--r--   0 cereal    (1000) cereal    (1000)     1119 2023-07-25 05:50:55.000000 pyDuotecno-2023.7.3/pyDuotecno.egg-info/PKG-INFO
+-rw-r--r--   0 cereal    (1000) cereal    (1000)      626 2023-07-25 05:50:55.000000 pyDuotecno-2023.7.3/pyDuotecno.egg-info/SOURCES.txt
+-rw-r--r--   0 cereal    (1000) cereal    (1000)        1 2023-07-25 05:50:55.000000 pyDuotecno-2023.7.3/pyDuotecno.egg-info/dependency_links.txt
+-rw-r--r--   0 cereal    (1000) cereal    (1000)        1 2023-04-01 08:06:22.000000 pyDuotecno-2023.7.3/pyDuotecno.egg-info/not-zip-safe
+-rw-r--r--   0 cereal    (1000) cereal    (1000)       28 2023-07-25 05:50:55.000000 pyDuotecno-2023.7.3/pyDuotecno.egg-info/top_level.txt
+-rw-r--r--   0 cereal    (1000) cereal    (1000)     1682 2023-07-25 05:45:09.000000 pyDuotecno-2023.7.3/pyproject.toml
+-rw-r--r--   0 cereal    (1000) cereal    (1000)        0 2023-04-01 07:56:09.000000 pyDuotecno-2023.7.3/requirements.txt
+-rw-r--r--   0 cereal    (1000) cereal    (1000)       38 2023-07-25 05:50:55.203315 pyDuotecno-2023.7.3/setup.cfg
+-rw-r--r--   0 cereal    (1000) cereal    (1000)       72 2023-04-01 08:10:33.000000 pyDuotecno-2023.7.3/setup.py
+drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-25 05:50:55.159978 pyDuotecno-2023.7.3/venv/
+drwxr-xr-x   0 cereal    (1000) cereal    (1000)        0 2023-07-25 05:50:55.199981 pyDuotecno-2023.7.3/venv/bin/
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      616 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.3/venv/bin/rst2html.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      738 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.3/venv/bin/rst2html4.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)     1083 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.3/venv/bin/rst2html5.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      815 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.3/venv/bin/rst2latex.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      638 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.3/venv/bin/rst2man.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      804 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.3/venv/bin/rst2odt.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)     1742 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.3/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      623 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.3/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      659 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.3/venv/bin/rst2s5.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      895 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.3/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      624 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.3/venv/bin/rst2xml.py
+-rwxr-xr-x   0 cereal    (1000) cereal    (1000)      692 2023-05-08 15:37:55.000000 pyDuotecno-2023.7.3/venv/bin/rstpep2html.py
```

### Comparing `pyDuotecno-2023.7.2/LICENSE` & `pyDuotecno-2023.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.2/PKG-INFO` & `pyDuotecno-2023.7.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDuotecno
-Version: 2023.7.2
+Version: 2023.7.3
 Summary: Open-source home automation platform running on Python 3.
 Author-email: Maikel Punie <maikel.punie@gmail.com>
 License: Apache
 Project-URL: Source Code, https://github.com/Cereal2nd/pyDuotecno
 Project-URL: Bug Reports, https://github.com/Cereal2nd/pyDuotecno/issues
 Keywords: home,duotecno,automation
 Platform: any
@@ -20,15 +20,8 @@
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-This is a package to talk to duotecno ip interfaces
-
-How to deploy a new version:
-
-bumpver update
-python -m build .
-twine check dist/_
-twine upload dist/_
+This is a package to talk to duotecno ip interfaces.
```

### Comparing `pyDuotecno-2023.7.2/duotecno/controller.py` & `pyDuotecno-2023.7.3/duotecno/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Main interface to the duotecno bus."""
 
 import asyncio
 import logging
-from duotecno.exceptions import InvallidPassword, LoadFailure
+from duotecno.exceptions import LoadFailure, InvalidPassword
 from duotecno.protocol import (
     Packet,
     EV_CLIENTCONNECTSET_3,
     EV_NODEDATABASEINFO_0,
     EV_NODEDATABASEINFO_1,
 )
 from duotecno.node import Node
@@ -59,15 +59,15 @@
         # send login info
         await self.write(f"[214,3,{len(passw)},{','.join(passw)}]")
         # wait for the login to be ok
         try:
             await asyncio.wait_for(self.loginOK.wait(), timeout=1.0)
             await self.loginOK.wait()
         except TimeoutError:
-            raise InvallidPassword()
+            raise InvalidPassword()
         # if we are not testing the connection, start scanning
         if not testOnly:
             await self.write("[209,0]")
             _loadTask = asyncio.Task(self._loadTask())
             try:
                 await asyncio.wait_for(self.loadOK.wait(), timeout=15.0)
             except TimeoutError:
```

### Comparing `pyDuotecno-2023.7.2/duotecno/node.py` & `pyDuotecno-2023.7.3/duotecno/node.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.2/duotecno/protocol.py` & `pyDuotecno-2023.7.3/duotecno/protocol.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.2/duotecno/unit.py` & `pyDuotecno-2023.7.3/duotecno/unit.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.2/examples/read.py` & `pyDuotecno-2023.7.3/examples/read.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.2/pyDuotecno.egg-info/PKG-INFO` & `pyDuotecno-2023.7.3/pyDuotecno.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDuotecno
-Version: 2023.7.2
+Version: 2023.7.3
 Summary: Open-source home automation platform running on Python 3.
 Author-email: Maikel Punie <maikel.punie@gmail.com>
 License: Apache
 Project-URL: Source Code, https://github.com/Cereal2nd/pyDuotecno
 Project-URL: Bug Reports, https://github.com/Cereal2nd/pyDuotecno/issues
 Keywords: home,duotecno,automation
 Platform: any
@@ -20,15 +20,8 @@
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-This is a package to talk to duotecno ip interfaces
-
-How to deploy a new version:
-
-bumpver update
-python -m build .
-twine check dist/_
-twine upload dist/_
+This is a package to talk to duotecno ip interfaces.
```

### Comparing `pyDuotecno-2023.7.2/pyDuotecno.egg-info/SOURCES.txt` & `pyDuotecno-2023.7.3/pyDuotecno.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.2/pyproject.toml` & `pyDuotecno-2023.7.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name        = "pyDuotecno"
 license     = {text = "Apache"}
-version     = "2023.7.2"
+version     = "2023.7.3"
 description = "Open-source home automation platform running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Maikel Punie", email = "maikel.punie@gmail.com"}
 ]
 keywords    = ["home", "duotecno", "automation"]
 classifiers = [
@@ -38,15 +38,15 @@
 zip-safe  = false
 include-package-data = true
 
 [tool.setuptools.packages.find]
 exclude = ["tests", "tests.*"]
 
 [tool.bumpver]
-current_version = "2023.7.2"
+current_version = "2023.7.3"
 version_pattern = "YYYY.MM.INC0"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `pyDuotecno-2023.7.2/venv/bin/rst2html.py` & `pyDuotecno-2023.7.3/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.2/venv/bin/rst2html4.py` & `pyDuotecno-2023.7.3/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.2/venv/bin/rst2html5.py` & `pyDuotecno-2023.7.3/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.2/venv/bin/rst2latex.py` & `pyDuotecno-2023.7.3/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.2/venv/bin/rst2man.py` & `pyDuotecno-2023.7.3/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.2/venv/bin/rst2odt.py` & `pyDuotecno-2023.7.3/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.2/venv/bin/rst2odt_prepstyles.py` & `pyDuotecno-2023.7.3/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.2/venv/bin/rst2pseudoxml.py` & `pyDuotecno-2023.7.3/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.2/venv/bin/rst2s5.py` & `pyDuotecno-2023.7.3/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.2/venv/bin/rst2xetex.py` & `pyDuotecno-2023.7.3/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.2/venv/bin/rst2xml.py` & `pyDuotecno-2023.7.3/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `pyDuotecno-2023.7.2/venv/bin/rstpep2html.py` & `pyDuotecno-2023.7.3/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

