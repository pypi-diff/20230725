# Comparing `tmp/fladrif-0.1.0.tar.gz` & `tmp/fladrif-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fladrif-0.1.0.tar", max compression
+gzip compressed data, was "fladrif-0.1.1.tar", max compression
```

## Comparing `fladrif-0.1.0.tar` & `fladrif-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      563 2023-07-12 23:48:24.518190 fladrif-0.1.0/README.md
--rw-r--r--   0        0        0      727 2023-07-13 00:21:46.941501 fladrif-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      727 2023-07-06 15:54:46.999709 fladrif-0.1.0/src/fladrif/__init__.py
--rw-r--r--   0        0        0     4274 2023-07-13 00:02:09.788181 fladrif-0.1.0/src/fladrif/apply.py
--rw-r--r--   0        0        0        0 2023-07-12 23:48:40.811524 fladrif-0.1.0/src/fladrif/py.typed
--rw-r--r--   0        0        0    10216 2023-07-13 00:02:09.784848 fladrif-0.1.0/src/fladrif/treediff.py
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 fladrif-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      563 2023-07-12 23:48:24.518190 fladrif-0.1.1/README.md
+-rw-r--r--   0        0        0      727 2023-07-25 17:46:18.701436 fladrif-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      727 2023-07-06 15:54:46.999709 fladrif-0.1.1/src/fladrif/__init__.py
+-rw-r--r--   0        0        0     4641 2023-07-13 20:09:54.144022 fladrif-0.1.1/src/fladrif/apply.py
+-rw-r--r--   0        0        0        0 2023-07-12 23:48:40.811524 fladrif-0.1.1/src/fladrif/py.typed
+-rw-r--r--   0        0        0    10216 2023-07-13 00:02:09.784848 fladrif-0.1.1/src/fladrif/treediff.py
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 fladrif-0.1.1/PKG-INFO
```

### Comparing `fladrif-0.1.0/README.md` & `fladrif-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fladrif-0.1.0/pyproject.toml` & `fladrif-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [tool.pytest.ini_options]
 norecursedirs = "tests/helpers"
 pythonpath = [ "src" ]
 
 [tool.poetry]
 name = "fladrif"
-version = "0.1.0"
+version = "0.1.1"
 description = "Compute a series of operations to transform one tree into another"
 authors = ["Sam Wilson <sam@binarycake.ca>"]
 license = "GPL-2.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `fladrif-0.1.0/src/fladrif/__init__.py` & `fladrif-0.1.1/src/fladrif/__init__.py`

 * *Files identical despite different names*

### Comparing `fladrif-0.1.0/src/fladrif/apply.py` & `fladrif-0.1.1/src/fladrif/apply.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,42 +74,47 @@
 
                 continue
 
             match op.tag:
                 case Tag.REPLACE:
                     assert op.sub is None
                     for before, after in self._kids(op, stack):
-                        assert before is not None
-                        assert after is not None
-                        self.replace(before, after)
+                        if before is not None and after is not None:
+                            self.replace(before, after)
+                        elif before is not None:
+                            self.delete(before)
+                        elif after is not None:
+                            self.insert(after)
+                        else:
+                            assert False, f"op: {op}"
                 case Tag.DELETE:
                     assert op.sub is None
                     for before, after in self._kids(op, stack):
-                        assert before is not None
-                        assert after is None
+                        assert before is not None, f"op: {op}"
+                        assert after is None, f"op: {op}"
                         self.delete(before)
                 case Tag.INSERT:
                     assert op.sub is None
                     for before, after in self._kids(op, stack):
-                        assert before is None
-                        assert after is not None
+                        assert before is None, f"op: {op}"
+                        assert after is not None, f"op: {op}"
                         self.insert(after)
                 case Tag.EQUAL:
                     assert op.sub is None
                     for before, after in self._kids(op, stack):
-                        assert before is not None
-                        assert after is not None
+                        assert before is not None, f"op: {op}"
+                        assert after is not None, f"op: {op}"
                         self.equal(before, after)
                 case Tag.DESCEND:
                     kids = list(self._kids(op, stack))
                     assert 1 == len(kids)
                     before, after = kids[0]
-                    assert before is not None
-                    assert after is not None
-                    assert op.sub is not None
+                    assert before is not None, f"op: {op}"
+                    assert after is not None, f"op: {op}"
+                    assert op.sub is not None, f"op: {op}"
                     stack.append(
                         _Level(
                             before=self.adapter.children(before),
                             after=self.adapter.children(after),
                             operations=iter(op.sub),
                         )
                     )
```

### Comparing `fladrif-0.1.0/src/fladrif/treediff.py` & `fladrif-0.1.1/src/fladrif/treediff.py`

 * *Files identical despite different names*

### Comparing `fladrif-0.1.0/PKG-INFO` & `fladrif-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fladrif
-Version: 0.1.0
+Version: 0.1.1
 Summary: Compute a series of operations to transform one tree into another
 License: GPL-2.0-or-later
 Author: Sam Wilson
 Author-email: sam@binarycake.ca
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3
```

