# Comparing `tmp/cm2py-0.2.6.tar.gz` & `tmp/cm2py-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cm2py-0.2.6.tar", last modified: Thu Jul 20 09:41:59 2023, max compression
+gzip compressed data, was "cm2py-0.2.7.tar", last modified: Tue Jul 25 10:50:57 2023, max compression
```

## Comparing `cm2py-0.2.6.tar` & `cm2py-0.2.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 09:41:59.552794 cm2py-0.2.6/
--rw-rw-rw-   0        0        0     1116 2023-05-09 09:46:12.000000 cm2py-0.2.6/LICENSE
--rw-rw-rw-   0        0        0     3012 2023-07-20 09:41:59.549787 cm2py-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     1189 2023-07-15 07:50:59.000000 cm2py-0.2.6/README.md
--rw-rw-rw-   0        0        0      675 2023-07-15 07:51:08.000000 cm2py-0.2.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-20 09:41:59.552794 cm2py-0.2.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-20 09:41:59.393796 cm2py-0.2.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-20 09:41:59.416794 cm2py-0.2.6/src/cm2py/
--rw-rw-rw-   0        0        0      237 2023-07-19 11:34:20.000000 cm2py-0.2.6/src/cm2py/__init__.py
--rw-rw-rw-   0        0        0     6480 2023-07-20 09:40:24.000000 cm2py-0.2.6/src/cm2py/cm2py.py
-drwxrwxrwx   0        0        0        0 2023-07-20 09:41:59.532793 cm2py-0.2.6/src/cm2py.egg-info/
--rw-rw-rw-   0        0        0     3012 2023-07-20 09:41:59.000000 cm2py-0.2.6/src/cm2py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-07-20 09:41:59.000000 cm2py-0.2.6/src/cm2py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 09:41:59.000000 cm2py-0.2.6/src/cm2py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-20 09:41:59.000000 cm2py-0.2.6/src/cm2py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-20 09:41:59.000000 cm2py-0.2.6/src/cm2py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-20 09:41:59.537793 cm2py-0.2.6/tests/
--rw-rw-rw-   0        0        0     2374 2023-07-19 09:48:55.000000 cm2py-0.2.6/tests/test_app.py
+drwxrwxrwx   0        0        0        0 2023-07-25 10:50:57.207667 cm2py-0.2.7/
+-rw-rw-rw-   0        0        0     1116 2023-05-09 09:46:12.000000 cm2py-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0     3012 2023-07-25 10:50:57.206671 cm2py-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1189 2023-07-15 07:50:59.000000 cm2py-0.2.7/README.md
+-rw-rw-rw-   0        0        0      675 2023-07-25 10:50:32.000000 cm2py-0.2.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-25 10:50:57.208669 cm2py-0.2.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-25 10:50:57.142669 cm2py-0.2.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-25 10:50:57.161672 cm2py-0.2.7/src/cm2py/
+-rw-rw-rw-   0        0        0      237 2023-07-19 11:34:20.000000 cm2py-0.2.7/src/cm2py/__init__.py
+-rw-rw-rw-   0        0        0     6419 2023-07-25 10:50:18.000000 cm2py-0.2.7/src/cm2py/cm2py.py
+drwxrwxrwx   0        0        0        0 2023-07-25 10:50:57.201673 cm2py-0.2.7/src/cm2py.egg-info/
+-rw-rw-rw-   0        0        0     3012 2023-07-25 10:50:57.000000 cm2py-0.2.7/src/cm2py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-07-25 10:50:57.000000 cm2py-0.2.7/src/cm2py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 10:50:57.000000 cm2py-0.2.7/src/cm2py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-25 10:50:57.000000 cm2py-0.2.7/src/cm2py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-25 10:50:57.000000 cm2py-0.2.7/src/cm2py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 10:50:57.204672 cm2py-0.2.7/tests/
+-rw-rw-rw-   0        0        0     2374 2023-07-19 09:48:55.000000 cm2py-0.2.7/tests/test_app.py
```

### Comparing `cm2py-0.2.6/LICENSE` & `cm2py-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cm2py-0.2.6/PKG-INFO` & `cm2py-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cm2py
-Version: 0.2.6
+Version: 0.2.7
 Summary: Circuit Maker 2 save generation and manipulation package
 Author-email: SKM GEEK <qestudios17@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cm2py-0.2.6/README.md` & `cm2py-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `cm2py-0.2.6/pyproject.toml` & `cm2py-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cm2py"
-version = "0.2.6"
+version = "0.2.7"
 authors = [
   { name="SKM GEEK", email="qestudios17@gmail.com" },
 ]
 description = "Circuit Maker 2 save generation and manipulation package"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
```

### Comparing `cm2py-0.2.6/src/cm2py/cm2py.py` & `cm2py-0.2.7/src/cm2py/cm2py.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 __copyright__ = "Copyright 2023, SKM GEEK"
 __date__ = "2023/05/21"
 __deprecated__ = False
 __email__ = "qestudios17@example.com"
 __license__ = "MIT"
 __maintainer__ = "SKM GEEK"
 __status__ = "Production"
-__version__ = "0.2.6"
+__version__ = "0.2.7"
 
 import re
 from uuid import UUID, uuid4
 import math
 
 
 class Save:
@@ -131,36 +131,39 @@
         r"[0-9a-f]*(;[0-9a-fA-F]*)*$"
     )
 
     assert re.match(regex, string), "invalid save string"
 
     newSave = Save()
 
-    blocks = [
+    sections = string.split("?")
+    blockString = sections[0].split(";")
+    connectionString = sections[1].split(";")
+
+    blockVals = [
         [
             None
             if not v
             else [float(a) for a in v.split("+")]
             if "+" in v or p == 5
             else float(v)
             if (v and p != 0)
             else int(v)
             for p, v in enumerate(i.split(","))
         ]
-        for i in "".join(string.split("?")[0]).split(";")
-    ]
-    connections = [
-        [int(v) for v in i.split(",")]
-        for i in "".join(string.split("?")[1]).split(";")
-        if len("".join(string.split("?")[1]).split(";")) > 1
-        and isinstance("".join(string.split("?")[1]).split(";")[0], int)
-        and isinstance("".join(string.split("?")[1]).split(";")[0], int)
+        for i in blockString
     ]
-    # Need to refactor these lines
-
-    for b in blocks:
-        newSave.addBlock(b[0], (b[2], b[3], b[4]), state=bool(b[1]), properties=b[5], snapToGrid=snapToGrid)
+    if len(connectionString) > 1:
+        connections = [[int(v) for v in i.split(",")] for i in connectionString]
+    else:
+        connections = []
+
+    blocks = []
+    for b in blockVals:
+        blocks.append(
+            newSave.addBlock(b[0], (b[2], b[3], b[4]), state=bool(b[1]), properties=b[5], snapToGrid=snapToGrid)
+        )
 
     for c in connections:
         newSave.addConnection(blocks[c[0] - 1], blocks[c[1] - 1])
 
     return newSave
```

### Comparing `cm2py-0.2.6/src/cm2py.egg-info/PKG-INFO` & `cm2py-0.2.7/src/cm2py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cm2py
-Version: 0.2.6
+Version: 0.2.7
 Summary: Circuit Maker 2 save generation and manipulation package
 Author-email: SKM GEEK <qestudios17@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cm2py-0.2.6/tests/test_app.py` & `cm2py-0.2.7/tests/test_app.py`

 * *Files identical despite different names*

