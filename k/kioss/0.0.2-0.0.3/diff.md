# Comparing `tmp/kioss-0.0.2.tar.gz` & `tmp/kioss-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kioss-0.0.2.tar", last modified: Tue Jul 25 15:55:44 2023, max compression
+gzip compressed data, was "kioss-0.0.3.tar", last modified: Tue Jul 25 16:03:49 2023, max compression
```

## Comparing `kioss-0.0.2.tar` & `kioss-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:55:44.270475 kioss-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 15:55:29.000000 kioss-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-25 15:55:44.270475 kioss-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-25 15:55:29.000000 kioss-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:55:44.270475 kioss-0.0.2/kioss/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-25 15:55:29.000000 kioss-0.0.2/kioss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-07-25 15:55:29.000000 kioss-0.0.2/kioss/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-25 15:55:29.000000 kioss-0.0.2/kioss/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:55:44.270475 kioss-0.0.2/kioss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-25 15:55:44.000000 kioss-0.0.2/kioss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-25 15:55:44.000000 kioss-0.0.2/kioss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 15:55:44.000000 kioss-0.0.2/kioss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 15:55:44.000000 kioss-0.0.2/kioss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 15:55:44.270475 kioss-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-25 15:55:29.000000 kioss-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:55:44.270475 kioss-0.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-07-25 15:55:29.000000 kioss-0.0.2/test/test_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-25 15:55:29.000000 kioss-0.0.2/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:03:49.688251 kioss-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 16:03:36.000000 kioss-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-25 16:03:49.688251 kioss-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-25 16:03:36.000000 kioss-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:03:49.688251 kioss-0.0.3/kioss/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-25 16:03:36.000000 kioss-0.0.3/kioss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-07-25 16:03:36.000000 kioss-0.0.3/kioss/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-25 16:03:36.000000 kioss-0.0.3/kioss/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:03:49.688251 kioss-0.0.3/kioss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-25 16:03:49.000000 kioss-0.0.3/kioss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-25 16:03:49.000000 kioss-0.0.3/kioss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 16:03:49.000000 kioss-0.0.3/kioss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 16:03:49.000000 kioss-0.0.3/kioss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 16:03:49.688251 kioss-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-25 16:03:36.000000 kioss-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:03:49.688251 kioss-0.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-07-25 16:03:36.000000 kioss-0.0.3/test/test_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-25 16:03:36.000000 kioss-0.0.3/test/test_util.py
```

### Comparing `kioss-0.0.2/LICENSE` & `kioss-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kioss-0.0.2/README.md` & `kioss-0.0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -13,22 +13,23 @@
 from kioss import Pipe
 
 words_count: int = (
     Pipe(open("...", "r"))
     .map(str.split)
     .explode()
     .map(lambda _: 1)
-    .reduce(int.__add__)
+    .reduce(int.__add__, initial=0)
 )
 ```
 
 ## Features
 - `.slow` a pipe to limit the iteration's speed over it
 - `.catch` any pipe's error to treat it after iteration
 - `.batch` pipe's elements and yield them as lists of a given max size or spanning over a given max period.
+- `.explode` a pipeline that yields iterable elements to make it separately yield each object contained in the element
 - `.map` over pipe's elements uing multiple threads
 - `.merge` several pipes to form a new one that yields elements using multiple threads
 - `.log` a pipe's iteration status
 - `.list` a pipe to collect its output into a list having an optional max size
 - `.reduce` a pipe
 - `.filter` a pipe
```

### Comparing `kioss-0.0.2/kioss/pipe.py` & `kioss-0.0.3/kioss/pipe.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,59 +23,59 @@
     def __next__(self) -> T:
         return next(self.iterator)
 
     def __iter__(self) -> T:
         return self
 
     def chain(self, *others: Iterable["Pipe[T]"]) -> "Pipe[T]":
-        return Pipe(itertools.chain(self, *others))
+        return Pipe[T](itertools.chain(self, *others))
 
     def merge(self, *others: Iterable["Pipe[T]"]) -> "Pipe[T]":
-        return _ConcurrentlyMergingPipe([self, *others])
+        return _ConcurrentlyMergingPipe[T]([self, *others])
 
     def map(
         self, func: Callable[[T], R], num_threads: int = 0, sidify: bool = False
     ) -> "Pipe[R]":
         if sidify:
             func = util.sidify(func)
 
         if num_threads <= 1:
-            return Pipe(map(func, self))
+            return Pipe[R](map(func, self))
         else:
 
             def iterable():
                 executor = ThreadPoolExecutor(max_workers=num_threads)
                 # non consumed map results block the worker that produced them, hence it makes it compatible with self.slow()
                 yield from executor.map(func, self)
                 executor.shutdown()
 
-            return Pipe(iter(iterable()))
+            return Pipe[R](iter(iterable()))
 
-    def explode(self: List[R]) -> "Pipe[R]":
-        return _ExplodingPipe(self)
+    def explode(self: Iterable[R]) -> "Pipe[R]":
+        return _ExplodingPipe[R](self)
 
-    def filter(self, predicate: Callable[[T], bool]) -> "Pipe[R]":
-        return Pipe(filter(predicate, self))
+    def filter(self, predicate: Callable[[T], bool]) -> "Pipe[T]":
+        return Pipe[T](filter(predicate, self))
 
     def batch(
         self, max_size: int = 100, max_window_seconds: float = float("inf")
     ) -> "Pipe[List[T]]":
-        return _BatchingPipe(self, max_size, max_window_seconds)
+        return _BatchingPipe[T](self, max_size, max_window_seconds)
 
     def slow(self, freq: int) -> "Pipe[T]":
-        return Pipe(_SlowingIterator(self, freq))
+        return Pipe[T](_SlowingIterator(self, freq))
 
     def head(self, n) -> "Pipe[T]":
-        return Pipe(itertools.islice(self, n))
+        return Pipe[T](itertools.islice(self, n))
 
     def catch(self) -> "Pipe[T]":
-        return _CatchingPipe(self)
+        return _CatchingPipe[T](self)
 
     def log(self) -> "Pipe[T]":
-        return _LoggingPipe(self)
+        return _LoggingPipe[T](self)
 
     def reduce(self, f: Callable[[R, T], R], initial: R) -> R:
         return reduce(f, self, initial)
 
     def list(self, limit: int = float("inf")) -> List[T]:
         return [elem for i, elem in enumerate(self) if i < limit]
```

### Comparing `kioss-0.0.2/test/test_pipe.py` & `kioss-0.0.3/test/test_pipe.py`

 * *Files identical despite different names*

