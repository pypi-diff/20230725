# Comparing `tmp/kioss-0.0.5.tar.gz` & `tmp/kioss-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kioss-0.0.5.tar", last modified: Tue Jul 25 20:07:05 2023, max compression
+gzip compressed data, was "kioss-0.0.6.tar", last modified: Tue Jul 25 20:15:04 2023, max compression
```

## Comparing `kioss-0.0.5.tar` & `kioss-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:07:05.501387 kioss-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 20:06:50.000000 kioss-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-25 20:07:05.501387 kioss-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-25 20:06:50.000000 kioss-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:07:05.497388 kioss-0.0.5/kioss/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-25 20:06:50.000000 kioss-0.0.5/kioss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12162 2023-07-25 20:06:50.000000 kioss-0.0.5/kioss/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-25 20:06:50.000000 kioss-0.0.5/kioss/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:07:05.497388 kioss-0.0.5/kioss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-25 20:07:05.000000 kioss-0.0.5/kioss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-25 20:07:05.000000 kioss-0.0.5/kioss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 20:07:05.000000 kioss-0.0.5/kioss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 20:07:05.000000 kioss-0.0.5/kioss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 20:07:05.501387 kioss-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-25 20:06:50.000000 kioss-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:07:05.501387 kioss-0.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-07-25 20:06:50.000000 kioss-0.0.5/test/test_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-25 20:06:50.000000 kioss-0.0.5/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:15:04.289058 kioss-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 20:14:51.000000 kioss-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-25 20:15:04.289058 kioss-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-25 20:14:51.000000 kioss-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:15:04.289058 kioss-0.0.6/kioss/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-25 20:14:51.000000 kioss-0.0.6/kioss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-07-25 20:14:51.000000 kioss-0.0.6/kioss/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-25 20:14:51.000000 kioss-0.0.6/kioss/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:15:04.289058 kioss-0.0.6/kioss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-25 20:15:04.000000 kioss-0.0.6/kioss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-25 20:15:04.000000 kioss-0.0.6/kioss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 20:15:04.000000 kioss-0.0.6/kioss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 20:15:04.000000 kioss-0.0.6/kioss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 20:15:04.289058 kioss-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-25 20:14:51.000000 kioss-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:15:04.289058 kioss-0.0.6/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-07-25 20:14:51.000000 kioss-0.0.6/test/test_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-25 20:14:51.000000 kioss-0.0.6/test/test_util.py
```

### Comparing `kioss-0.0.5/LICENSE` & `kioss-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kioss-0.0.5/README.md` & `kioss-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `kioss-0.0.5/kioss/pipe.py` & `kioss-0.0.6/kioss/pipe.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,27 +200,29 @@
 
         def iterate():
             for _ in self:
                 pass
 
         return timeit.timeit(iterate, number=1)
 
-    def superintend(self, errors_sample_size: int = 8) -> None:
+    def superintend(self, num_error_samples: int = 8) -> None:
         """
-        Superintend the Pipe and raise a RuntimeError if any exceptions occur during iteration.
+        Superintend the Pipe: iterate over the pipe until it is exhausted and raise a RuntimeError if any exceptions occur during iteration.
 
         Args:
-            errors_sample_size (int, optional): The maximum number of error samples to include in the RuntimeError message (default is 8).
+            num_error_samples (int, optional): The maximum number of error samples to include in the RuntimeError message (default is 8).
+        Raises:
+            RuntimeError: If any exception is catched during iteration.
         """
         if errors := (
             self.catch()
             .log()
             .filter(lambda elem: isinstance(elem, Exception))
             .map(repr)
-            .collect(limit=errors_sample_size)
+            .collect(limit=num_error_samples)
         ):
             raise RuntimeError(errors)
 
 
 class _FlatteningPipe(Pipe[R]):
     def __init__(self, iterator: Iterator[Iterable[R]]) -> None:
         super().__init__(iterator)
```

### Comparing `kioss-0.0.5/test/test_pipe.py` & `kioss-0.0.6/test/test_pipe.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,20 +136,20 @@
             delta=0.3 * TEN_MS * 8,
         )
 
     def test_reduce(self):
         self.assertEqual(Pipe(range(8)).map(lambda _: 1).reduce(int.__add__, 0), 8)
 
     def test_timeit(self):
-        get_pipe = lambda: Pipe(range(8)).slow(64)
+        new_pipe = lambda: Pipe(range(8)).slow(64)
         start_time = time.time()
-        list(get_pipe())
+        list(new_pipe())
         execution_time = time.time() - start_time
         self.assertAlmostEqual(
-            execution_time, get_pipe().time(), delta=0.3 * execution_time
+            execution_time, new_pipe().time(), delta=0.3 * execution_time
         )
 
     def test_catch(self):
         self.assertListEqual(
             list(Pipe(["1", "r", "2"]).map(int).catch().map(type)),
             [int, ValueError, int],
         )
```

