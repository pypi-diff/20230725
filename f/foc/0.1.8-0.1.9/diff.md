# Comparing `tmp/foc-0.1.8.tar.gz` & `tmp/foc-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foc-0.1.8.tar", last modified: Sat Jul 22 15:28:12 2023, max compression
+gzip compressed data, was "foc-0.1.9.tar", last modified: Tue Jul 25 17:35:23 2023, max compression
```

## Comparing `foc-0.1.8.tar` & `foc-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-07-22 15:28:12.977149 foc-0.1.8/
--rw-r--r--   0 thyeem     (501) staff       (20)      644 2023-07-22 15:22:35.000000 foc-0.1.8/ChangeLog.md
--rw-r--r--   0 thyeem     (501) staff       (20)     1068 2023-06-07 00:06:02.000000 foc-0.1.8/LICENSE
--rw-r--r--   0 thyeem     (501) staff       (20)       55 2023-06-07 00:06:02.000000 foc-0.1.8/MANIFEST.in
--rw-r--r--   0 thyeem     (501) staff       (20)    17346 2023-07-22 15:28:12.977217 foc-0.1.8/PKG-INFO
--rw-r--r--   0 thyeem     (501) staff       (20)    16885 2023-07-18 12:48:54.000000 foc-0.1.8/README.md
-drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-07-22 15:28:12.976268 foc-0.1.8/foc/
--rw-r--r--   0 thyeem     (501) staff       (20)    20370 2023-07-22 15:19:41.000000 foc-0.1.8/foc/__init__.py
-drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-07-22 15:28:12.976733 foc-0.1.8/foc.egg-info/
--rw-r--r--   0 thyeem     (501) staff       (20)    17346 2023-07-22 15:28:12.000000 foc-0.1.8/foc.egg-info/PKG-INFO
--rw-r--r--   0 thyeem     (501) staff       (20)      221 2023-07-22 15:28:12.000000 foc-0.1.8/foc.egg-info/SOURCES.txt
--rw-r--r--   0 thyeem     (501) staff       (20)        1 2023-07-22 15:28:12.000000 foc-0.1.8/foc.egg-info/dependency_links.txt
--rw-r--r--   0 thyeem     (501) staff       (20)       10 2023-07-22 15:28:12.000000 foc-0.1.8/foc.egg-info/top_level.txt
--rw-r--r--   0 thyeem     (501) staff       (20)      102 2023-07-22 15:28:12.977448 foc-0.1.8/setup.cfg
--rw-r--r--   0 thyeem     (501) staff       (20)      700 2023-07-22 15:22:53.000000 foc-0.1.8/setup.py
-drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-07-22 15:28:12.976922 foc-0.1.8/tests/
--rw-r--r--   0 thyeem     (501) staff       (20)        0 2023-06-15 10:03:02.000000 foc-0.1.8/tests/__init__.py
--rw-r--r--   0 thyeem     (501) staff       (20)     8338 2023-07-18 12:57:28.000000 foc-0.1.8/tests/test_foc.py
+drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-07-25 17:35:23.105700 foc-0.1.9/
+-rw-r--r--   0 thyeem     (501) staff       (20)      806 2023-07-25 17:32:53.000000 foc-0.1.9/ChangeLog.md
+-rw-r--r--   0 thyeem     (501) staff       (20)     1068 2023-05-15 21:22:31.000000 foc-0.1.9/LICENSE
+-rw-r--r--   0 thyeem     (501) staff       (20)       55 2023-06-06 23:18:02.000000 foc-0.1.9/MANIFEST.in
+-rw-r--r--   0 thyeem     (501) staff       (20)    17346 2023-07-25 17:35:23.105854 foc-0.1.9/PKG-INFO
+-rw-r--r--   0 thyeem     (501) staff       (20)    16885 2023-07-25 17:27:48.000000 foc-0.1.9/README.md
+drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-07-25 17:35:23.103714 foc-0.1.9/foc/
+-rw-r--r--   0 thyeem     (501) staff       (20)    20454 2023-07-25 17:18:05.000000 foc-0.1.9/foc/__init__.py
+drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-07-25 17:35:23.104950 foc-0.1.9/foc.egg-info/
+-rw-r--r--   0 thyeem     (501) staff       (20)    17346 2023-07-25 17:35:23.000000 foc-0.1.9/foc.egg-info/PKG-INFO
+-rw-r--r--   0 thyeem     (501) staff       (20)      221 2023-07-25 17:35:23.000000 foc-0.1.9/foc.egg-info/SOURCES.txt
+-rw-r--r--   0 thyeem     (501) staff       (20)        1 2023-07-25 17:35:23.000000 foc-0.1.9/foc.egg-info/dependency_links.txt
+-rw-r--r--   0 thyeem     (501) staff       (20)       10 2023-07-25 17:35:23.000000 foc-0.1.9/foc.egg-info/top_level.txt
+-rw-r--r--   0 thyeem     (501) staff       (20)      102 2023-07-25 17:35:23.106285 foc-0.1.9/setup.cfg
+-rw-r--r--   0 thyeem     (501) staff       (20)      700 2023-07-25 17:20:46.000000 foc-0.1.9/setup.py
+drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-07-25 17:35:23.105468 foc-0.1.9/tests/
+-rw-r--r--   0 thyeem     (501) staff       (20)        0 2023-06-11 20:28:50.000000 foc-0.1.9/tests/__init__.py
+-rw-r--r--   0 thyeem     (501) staff       (20)     8338 2023-07-19 17:13:12.000000 foc-0.1.9/tests/test_foc.py
```

### Comparing `foc-0.1.8/ChangeLog.md` & `foc-0.1.9/ChangeLog.md`

 * *Files 15% similar despite different names*

```diff
@@ -24,7 +24,12 @@
 - Improved `random_int`
 
 # 0.1.7
 - Added `const`, `until`, and `apply`
 
 # 0.1.8
 - Added `choice`
+
+# 0.1.9
+- Fixed `fread`. Keep whitespaces at the end of lines.
+- Fixed `chunks_of`. Filling values is optional.
+- Fixed `lines`. No splits on trailing newlines.
```

### Comparing `foc-0.1.8/LICENSE` & `foc-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `foc-0.1.8/PKG-INFO` & `foc-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foc
-Version: 0.1.8
+Version: 0.1.9
 Summary: A collection of python functions for somebody's sanity
 Home-page: https://github.com/thyeem/foc
 Author: Francis Lim
 Author-email: thyeem@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `foc-0.1.8/README.md` & `foc-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `foc-0.1.8/foc/__init__.py` & `foc-0.1.9/foc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,15 @@
 
 
 def unwords(x):
     return " ".join(x)
 
 
 def lines(x):
-    return x.split("\n")
+    return x.splitlines()
 
 
 def unlines(x):
     return "\n".join(x)
 
 
 def elem(x, xs):
@@ -669,15 +669,15 @@
 def fread(*args):
     """flat-read: read iterables from objects or files then flatten them"""
     f = cf_(normpath, bytes.decode)
 
     for x in flat(args):
         if isinstance(x, bytes):
             if exists(f(x), "f"):
-                yield open(f(x), "r").read().splitlines()
+                yield open(f(x), "r").readlines()
             else:
                 error(f"Error, not found file: {f(x)}")
         else:
             yield x
 
 
 def fwrite(f, *args):
@@ -690,17 +690,20 @@
 
 def split_at(ix, x):
     """split iterables at the given splitting-indices"""
     s = flatl(0, ix, None)
     return ([*it.islice(x, begin, end)] for begin, end in zip(s, s[1:]))
 
 
-def chunks_of(n, x, fill=None):
+def chunks_of(n, x, fillvalue=None, fill=True):
+    if not fill:
+        x = list(x)
+        x = x[: len(x) // n * n]
     """split interables into the given `n-length` pieces"""
-    return it.zip_longest(*(iter(x),) * n, fillvalue=fill)
+    return it.zip_longest(*(iter(x),) * n, fillvalue=fillvalue)
 
 
 def capture(p, string):
     x = captures(p, string)
     if x:
         return fst(x)
```

### Comparing `foc-0.1.8/foc.egg-info/PKG-INFO` & `foc-0.1.9/foc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foc
-Version: 0.1.8
+Version: 0.1.9
 Summary: A collection of python functions for somebody's sanity
 Home-page: https://github.com/thyeem/foc
 Author: Francis Lim
 Author-email: thyeem@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `foc-0.1.8/setup.py` & `foc-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="foc",
-    version="0.1.8",
+    version="0.1.9",
     author="Francis Lim",
     author_email="thyeem@gmail.com",
     description="A collection of python functions for somebody's sanity",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[],
     url="https://github.com/thyeem/foc",
```

### Comparing `foc-0.1.8/tests/test_foc.py` & `foc-0.1.9/tests/test_foc.py`

 * *Files identical despite different names*

