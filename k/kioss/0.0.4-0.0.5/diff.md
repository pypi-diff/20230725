# Comparing `tmp/kioss-0.0.4.tar.gz` & `tmp/kioss-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kioss-0.0.4.tar", last modified: Tue Jul 25 19:05:28 2023, max compression
+gzip compressed data, was "kioss-0.0.5.tar", last modified: Tue Jul 25 20:07:05 2023, max compression
```

## Comparing `kioss-0.0.4.tar` & `kioss-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:05:28.505671 kioss-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 19:05:11.000000 kioss-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-25 19:05:28.505671 kioss-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-25 19:05:11.000000 kioss-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:05:28.501671 kioss-0.0.4/kioss/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-25 19:05:11.000000 kioss-0.0.4/kioss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-07-25 19:05:11.000000 kioss-0.0.4/kioss/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-25 19:05:11.000000 kioss-0.0.4/kioss/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:05:28.505671 kioss-0.0.4/kioss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-25 19:05:28.000000 kioss-0.0.4/kioss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-25 19:05:28.000000 kioss-0.0.4/kioss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:05:28.000000 kioss-0.0.4/kioss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 19:05:28.000000 kioss-0.0.4/kioss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:05:28.505671 kioss-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-25 19:05:11.000000 kioss-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:05:28.505671 kioss-0.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-07-25 19:05:11.000000 kioss-0.0.4/test/test_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-25 19:05:11.000000 kioss-0.0.4/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:07:05.501387 kioss-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 20:06:50.000000 kioss-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-25 20:07:05.501387 kioss-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-25 20:06:50.000000 kioss-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:07:05.497388 kioss-0.0.5/kioss/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-25 20:06:50.000000 kioss-0.0.5/kioss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12162 2023-07-25 20:06:50.000000 kioss-0.0.5/kioss/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-25 20:06:50.000000 kioss-0.0.5/kioss/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:07:05.497388 kioss-0.0.5/kioss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-25 20:07:05.000000 kioss-0.0.5/kioss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-25 20:07:05.000000 kioss-0.0.5/kioss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 20:07:05.000000 kioss-0.0.5/kioss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 20:07:05.000000 kioss-0.0.5/kioss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 20:07:05.501387 kioss-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-25 20:06:50.000000 kioss-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:07:05.501387 kioss-0.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-07-25 20:06:50.000000 kioss-0.0.5/test/test_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-25 20:06:50.000000 kioss-0.0.5/test/test_util.py
```

### Comparing `kioss-0.0.4/LICENSE` & `kioss-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kioss-0.0.4/test/test_pipe.py` & `kioss-0.0.5/test/test_pipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,23 +71,23 @@
         self.assertListEqual(
             list(Pipe(args).map(func_with_side_effect, sidify=True)), list(args)
         )
         self.assertListEqual(l, list(map(func, args)))
 
     def test_explode(self):
         self.assertListEqual(
-            list(Pipe(["Hello World", "Happy to be here :)"]).map(str.split).explode()),
+            list(Pipe(["Hello World", "Happy to be here :)"]).map(str.split).flatten()),
             ["Hello", "World", "Happy", "to", "be", "here", ":)"],
         )
         self.assertEqual(
             sum(
                 Pipe([["1 2 3", "4 5 6"], ["7", "8 9 10"]])
-                .explode()
+                .flatten()
                 .map(str.split)
-                .explode()
+                .flatten()
                 .map(int)
             ),
             55,
         )
 
     def test_filter(self):
         self.assertListEqual(list(Pipe(range(8)).filter(lambda x: x % 2)), [1, 3, 5, 7])
@@ -121,19 +121,19 @@
         self.assertAlmostEqual(
             Pipe(range(8)).map(ten_millis_identity).head(2).time(),
             TEN_MS * 2,
             delta=0.3 * TEN_MS * 2,
         )
 
     def test_list(self):
-        self.assertListEqual(Pipe(range(8)).list(limit=6), list(range(6)))
-        self.assertListEqual(Pipe(range(8)).list(), list(range(8)))
+        self.assertListEqual(Pipe(range(8)).collect(limit=6), list(range(6)))
+        self.assertListEqual(Pipe(range(8)).collect(), list(range(8)))
         self.assertAlmostEqual(
             timeit.timeit(
-                lambda: Pipe(range(8)).map(ten_millis_identity).list(0),
+                lambda: Pipe(range(8)).map(ten_millis_identity).collect(0),
                 number=1,
             ),
             TEN_MS * 8,
             delta=0.3 * TEN_MS * 8,
         )
 
     def test_reduce(self):
```

