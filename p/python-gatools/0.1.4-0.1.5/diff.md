# Comparing `tmp/python_gatools-0.1.4-py3-none-any.whl.zip` & `tmp/python_gatools-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,24 @@
-Zip file size: 20109 bytes, number of entries: 20
--rw-r--r--  2.0 unx      463 b- defN 23-Jul-14 03:25 gatools/__init__.py
--rw-r--r--  2.0 unx      398 b- defN 23-Jul-14 03:25 gatools/colors.py
--rw-r--r--  2.0 unx    17593 b- defN 23-Jul-14 03:25 gatools/commons.py
--rw-r--r--  2.0 unx      421 b- defN 23-Jul-14 03:25 gatools/ctxman.py
--rw-r--r--  2.0 unx     1108 b- defN 23-Jul-14 03:25 gatools/decorators.py
--rw-r--r--  2.0 unx     1416 b- defN 23-Jul-14 03:25 gatools/dictkeys.py
--rw-r--r--  2.0 unx      618 b- defN 23-Jul-14 03:25 gatools/dictops.py
--rw-r--r--  2.0 unx      173 b- defN 23-Jul-14 03:25 gatools/envs.py
--rw-r--r--  2.0 unx      562 b- defN 23-Jul-14 03:25 gatools/files.py
--rw-r--r--  2.0 unx     1172 b- defN 23-Jul-14 03:25 gatools/jsonencoder.py
--rw-r--r--  2.0 unx     4899 b- defN 23-Jul-14 03:25 gatools/logger.py
--rw-r--r--  2.0 unx     5120 b- defN 23-Jul-14 03:25 gatools/oar.py
--rw-r--r--  2.0 unx     9129 b- defN 23-Jul-14 03:25 gatools/pyplot.py
--rw-r--r--  2.0 unx     2251 b- defN 23-Jul-14 03:25 gatools/tables.py
--rw-r--r--  2.0 unx     1640 b- defN 23-Jul-14 03:25 gatools/temp.py
--rw-r--r--  2.0 unx     2807 b- defN 23-Jul-14 03:25 gatools/utils.py
--rw-r--r--  2.0 unx      406 b- defN 23-Jul-14 03:26 python_gatools-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-14 03:26 python_gatools-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-14 03:26 python_gatools-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1509 b- defN 23-Jul-14 03:26 python_gatools-0.1.4.dist-info/RECORD
-20 files, 51785 bytes uncompressed, 17699 bytes compressed:  65.8%
+Zip file size: 22117 bytes, number of entries: 22
+-rw-r--r--  2.0 unx      563 b- defN 23-Jul-25 01:20 gatools/__init__.py
+-rw-r--r--  2.0 unx      398 b- defN 23-Jul-25 01:20 gatools/colors.py
+-rw-r--r--  2.0 unx    17733 b- defN 23-Jul-25 01:20 gatools/commons.py
+-rw-r--r--  2.0 unx     2221 b- defN 23-Jul-25 01:20 gatools/container.py
+-rw-r--r--  2.0 unx      421 b- defN 23-Jul-25 01:20 gatools/ctxman.py
+-rw-r--r--  2.0 unx     1108 b- defN 23-Jul-25 01:20 gatools/decorators.py
+-rw-r--r--  2.0 unx     1432 b- defN 23-Jul-25 01:20 gatools/dictkeys.py
+-rw-r--r--  2.0 unx      818 b- defN 23-Jul-25 01:20 gatools/dictops.py
+-rw-r--r--  2.0 unx      306 b- defN 23-Jul-25 01:20 gatools/envs.py
+-rw-r--r--  2.0 unx     1048 b- defN 23-Jul-25 01:20 gatools/files.py
+-rw-r--r--  2.0 unx     1172 b- defN 23-Jul-25 01:20 gatools/jsonencoder.py
+-rw-r--r--  2.0 unx     4899 b- defN 23-Jul-25 01:20 gatools/logger.py
+-rw-r--r--  2.0 unx     5120 b- defN 23-Jul-25 01:20 gatools/oar.py
+-rw-r--r--  2.0 unx     9129 b- defN 23-Jul-25 01:20 gatools/pyplot.py
+-rw-r--r--  2.0 unx     1245 b- defN 23-Jul-25 01:20 gatools/strings.py
+-rw-r--r--  2.0 unx     2251 b- defN 23-Jul-25 01:20 gatools/tables.py
+-rw-r--r--  2.0 unx     1640 b- defN 23-Jul-25 01:20 gatools/temp.py
+-rw-r--r--  2.0 unx     2807 b- defN 23-Jul-25 01:20 gatools/utils.py
+-rw-r--r--  2.0 unx      406 b- defN 23-Jul-25 01:20 python_gatools-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-25 01:20 python_gatools-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-25 01:20 python_gatools-0.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1662 b- defN 23-Jul-25 01:20 python_gatools-0.1.5.dist-info/RECORD
+22 files, 56479 bytes uncompressed, 19479 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -3,14 +3,17 @@
 
 Filename: gatools/colors.py
 Comment: 
 
 Filename: gatools/commons.py
 Comment: 
 
+Filename: gatools/container.py
+Comment: 
+
 Filename: gatools/ctxman.py
 Comment: 
 
 Filename: gatools/decorators.py
 Comment: 
 
 Filename: gatools/dictkeys.py
@@ -33,29 +36,32 @@
 
 Filename: gatools/oar.py
 Comment: 
 
 Filename: gatools/pyplot.py
 Comment: 
 
+Filename: gatools/strings.py
+Comment: 
+
 Filename: gatools/tables.py
 Comment: 
 
 Filename: gatools/temp.py
 Comment: 
 
 Filename: gatools/utils.py
 Comment: 
 
-Filename: python_gatools-0.1.4.dist-info/METADATA
+Filename: python_gatools-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: python_gatools-0.1.4.dist-info/WHEEL
+Filename: python_gatools-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: python_gatools-0.1.4.dist-info/top_level.txt
+Filename: python_gatools-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: python_gatools-0.1.4.dist-info/RECORD
+Filename: python_gatools-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gatools/__init__.py

```diff
@@ -3,12 +3,14 @@
 from gatools.files import *
 from gatools.colors import Color
 from gatools.ctxman import timeout
 from gatools.decorators import *
 from gatools.utils import *
 from gatools.jsonencoder import *
 from gatools.dictkeys import print_keys
-from gatools.dictops import analyse, query
+from gatools.dictops import analyse, query, make_string, decode_string
 from gatools.pyplot import *
 from gatools.tables import Table
 from gatools.temp import TmpDir, TmpFile
 from gatools.commons import *
+from gatools.container import Container
+from gatools.strings import Str
```

## gatools/commons.py

```diff
@@ -15,14 +15,16 @@
 import tempfile
 import time
 from contextlib import contextmanager
 from os.path import join, isfile, basename, isdir
 from typing import List, Union, Any
 from zipfile import ZipFile
 
+from munch import munchify as m_munchify
+
 
 from gatools.files import Tree, removeIfExists
 from gatools.jsonencoder import JsonEncoder
 
 
 try:
     import yaml
@@ -67,16 +69,18 @@
     "unique",
     "get_string",
     "dump",
     "logf",
     "logd",
     "breaklines",
     "Timer",
+    "munchify",
 ]
 
+
 # def join(*paths: TS) -> S:
 #     """Wrapper of `os.path.join`"""
 #     x = map(lambda y: y.abs() if isinstance(y, Tree) else y, paths)
 #     return Str(os.path.join(*x))
 
 
 # def isDir(path: TS):
@@ -109,14 +113,15 @@
 
 
 def load_json(filename: str, force_ext: bool = True, munch: bool = False, **kwargs):
     """Loads a json file with `json.load`
 
     :return: dict
     """
+    filename = str(filename)
     if force_ext:
         filename = ensure_ext(filename, "json")
     with open(filename, "r") as f:
         if munch:
             from munch import munchify
 
             return munchify(json.load(f, **kwargs))
@@ -125,14 +130,15 @@
 
 
 def dump_json(filename: str, data, force_ext: bool = True, **kwargs):
     """Dumps a dict to a json file with `json.dump`
 
     :param data: dict
     """
+    filename = str(filename)
     if force_ext:
         filename = ensure_ext(filename, "json")
     kwargs.setdefault("indent", 4)
     kwargs.setdefault("cls", JsonEncoder)
     with open(filename, "w") as f:
         json.dump(data, f, **kwargs)
 
@@ -648,7 +654,9 @@
     for y in x_:
         if len(groups[-1]) + len(y) < k:
             groups[-1] += " " + y
         else:
             groups.append(y)
     groups[0] = groups[0][1:]
     return bc.join(groups)
+
+munchify = m_munchify
```

## gatools/dictkeys.py

```diff
@@ -47,7 +47,8 @@
             extra = callback(v) if with_extra else ""
             tree.create_node(f"{k}{extra}", anc, parent=anchor)
             if isinstance(v, dict):
                 walk_dict(v, anchor=anc)
 
     walk_dict(dic)
     tree.show()
+    return tree
```

## gatools/dictops.py

```diff
@@ -1,11 +1,11 @@
 import logging
 from collections import defaultdict
 
-from munch import munchify
+from munch import Munch, munchify
 
 
 def analyse(d):
     # Analyse a list of dict
     r = defaultdict(list)
     for x in d:
         for k, v in x.items():
@@ -25,8 +25,16 @@
         if cond:
             xkeep.append(x)
     if len(xkeep) == 1:
         return munchify(xkeep[0])
     return xkeep
 
 
+def make_string(**kw):
+    return "&".join([f"{k}={v}" for k, v in kw.items()])
+
+
+def decode_string(s) -> Munch:
+    return munchify({x.split("=")[0]: x.split("=")[1] for x in s.split("&")})
+
+
 log = logging.getLogger(__name__)
```

## gatools/envs.py

```diff
@@ -1,8 +1,15 @@
+import os
 from pathlib import Path
 from dotenv import load_dotenv
 
-__ALL__ = ["load_fenv"]
+__ALL__ = ["load_fenv", "fenv"]
 
 
 def load_fenv(path: str, fname: str = ".env"):
     load_dotenv(Path(path).parent / fname)
+
+
+def fenv(fname, key):
+    """ > ga.fenv(__file__, "ENVVAR") < """
+    load_fenv(fname)
+    return os.getenv(key)
```

## gatools/files.py

```diff
@@ -1,22 +1,41 @@
+import glob
 import os
 import pathlib
+import shutil
 
-__ALL__ = ["Tree", "fTree", "removeIfExists"]
+__ALL__ = ["Tree", "fTree", "removeIfExists", "remove", "move"]
 
 
 class Tree(type(pathlib.Path())):
     def mkdir(self, parents=True, exist_ok=True):
         super().mkdir(parents=parents, exist_ok=exist_ok)
+        return self
 
 
 class fTree(Tree):
     def __new__(cls, *args, **kwargs):
         args = list(args)
         if (x := pathlib.Path(args[0])).is_file():
             args[0] = x.parent
         return super().__new__(cls, *args, **kwargs)
 
+
 def removeIfExists(fname: str):
     """Remove `fname` if it exists"""
     if os.path.exists(fname):
-        os.remove(fname)
+        os.remove(fname)
+
+
+def remove(*args: str):
+    """Remove files in globs `*args` if they exist"""
+    for t in args:
+        for f in glob.glob(t):
+            removeIfExists(f)
+
+
+def move(arg: str, dest: str):
+    """Move files in glob `arg` to `dest` with `shutil.move`"""
+    from gatools.strings import Str
+    for f in glob.glob(arg):
+        removeIfExists(os.path.join(dest, os.path.basename(f)))
+        shutil.move(f, Str(dest))
```

