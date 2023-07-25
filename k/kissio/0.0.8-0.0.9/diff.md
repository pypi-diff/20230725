# Comparing `tmp/kissio-0.0.8.tar.gz` & `tmp/kissio-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kissio-0.0.8.tar", last modified: Mon Jul 24 15:03:06 2023, max compression
+gzip compressed data, was "kissio-0.0.9.tar", last modified: Tue Jul 25 10:46:49 2023, max compression
```

## Comparing `kissio-0.0.8.tar` & `kissio-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:03:06.594215 kissio-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 15:02:54.000000 kissio-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-24 15:03:06.594215 kissio-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-24 15:02:54.000000 kissio-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:03:06.590214 kissio-0.0.8/kissio/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-24 15:02:54.000000 kissio-0.0.8/kissio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7077 2023-07-24 15:02:54.000000 kissio-0.0.8/kissio/pipe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:03:06.590214 kissio-0.0.8/kissio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-24 15:03:06.000000 kissio-0.0.8/kissio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-24 15:03:06.000000 kissio-0.0.8/kissio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 15:03:06.000000 kissio-0.0.8/kissio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 15:03:06.000000 kissio-0.0.8/kissio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 15:03:06.594215 kissio-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-24 15:02:54.000000 kissio-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 15:03:06.594215 kissio-0.0.8/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-07-24 15:02:54.000000 kissio-0.0.8/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:46:49.782048 kissio-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 10:46:29.000000 kissio-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-25 10:46:49.782048 kissio-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-25 10:46:29.000000 kissio-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:46:49.778048 kissio-0.0.9/kissio/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-25 10:46:29.000000 kissio-0.0.9/kissio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-07-25 10:46:29.000000 kissio-0.0.9/kissio/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-25 10:46:29.000000 kissio-0.0.9/kissio/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:46:49.778048 kissio-0.0.9/kissio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-25 10:46:49.000000 kissio-0.0.9/kissio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-25 10:46:49.000000 kissio-0.0.9/kissio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 10:46:49.000000 kissio-0.0.9/kissio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 10:46:49.000000 kissio-0.0.9/kissio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 10:46:49.782048 kissio-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-25 10:46:29.000000 kissio-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:46:49.778048 kissio-0.0.9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-07-25 10:46:29.000000 kissio-0.0.9/test/test.py
```

### Comparing `kissio-0.0.8/LICENSE` & `kissio-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kissio-0.0.8/README.md` & `kissio-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `kissio-0.0.8/kissio/pipe.py` & `kissio-0.0.9/kissio/pipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import timeit
 from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime
 from functools import reduce
 from queue import Empty, Queue
 from typing import Callable, Iterable, Iterator, List, TypeVar
 
+import kissio.util as util
+
 T = TypeVar("T")
 R = TypeVar("R")
 
 
 class Pipe(Iterator[T]):
     def __init__(self, iterator: Iterator[T]) -> None:
         self.iterator: Iterator[T] = iter(
@@ -26,15 +28,20 @@
 
     def chain(self, *others: Iterable["Pipe[T]"]) -> "Pipe[T]":
         return Pipe(itertools.chain(self, *others))
 
     def merge(self, *others: Iterable["Pipe[T]"]) -> "Pipe[T]":
         return _ConcurrentlyMergingPipe([self, *others])
 
-    def map(self, func: Callable[[T], R], num_threads: int = 0) -> "Pipe[R]":
+    def map(
+        self, func: Callable[[T], R], num_threads: int = 0, sidify: bool = False
+    ) -> "Pipe[R]":
+        if sidify:
+            func = util.sidify(func)
+
         if num_threads <= 1:
             return Pipe(map(func, self))
         else:
 
             def iterable():
                 executor = ThreadPoolExecutor(max_workers=num_threads)
                 # non consumed map results block the worker that produced them, hence it makes it compatible with self.slow()
```

### Comparing `kissio-0.0.8/test/test.py` & `kissio-0.0.9/test/test.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import time
 import timeit
+from typing import List
 import unittest
 
 from kissio import Pipe
 from kissio.pipe import CatchedPipeError
+from kissio.util import sidify
 
 TEN_MS = 0.01
 
 
 def ten_millis_identity(x):
     time.sleep(TEN_MS)
     return x
@@ -55,14 +57,27 @@
         num_threads = 2
         pipe = Pipe(range(8)).map(ten_millis_identity, num_threads=num_threads)
         self.assertAlmostEqual(
             pipe.timeit(),
             TEN_MS * 8 / num_threads,
             delta=0.3 * (TEN_MS * 8) / num_threads,
         )
+        # sidify
+        l: List[int] = []
+
+        def func_with_side_effect(x):
+            res = x**2
+            l.append(res)
+            return res
+
+        args = range(8)
+        self.assertListEqual(
+            list(Pipe(args).map(func_with_side_effect, sidify=True)), list(args)
+        )
+        self.assertListEqual(l, list(map(func, args)))
 
     def test_explode(self):
         self.assertListEqual(
             list(Pipe(["Hello World", "Happy to be here :)"]).map(str.split).explode()),
             ["Hello", "World", "Happy", "to", "be", "here", ":)"],
         )
         self.assertEqual(
@@ -145,7 +160,18 @@
         list(
             Pipe(range(9))
             .map(lambda elem: ("_" if elem % 2 else "") + str(elem))
             .map(int)
             .catch()
             .log()
         )
+
+    def test_sidify(self):
+        f = lambda x: x**2
+        self.assertEqual(f(2), 4)
+        self.assertEqual(sidify(f)(2), 2)
+
+        @sidify
+        def f(x):
+            return x**2
+
+        self.assertEqual(f(2), 2)
```

