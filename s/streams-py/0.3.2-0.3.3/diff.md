# Comparing `tmp/streams_py-0.3.2.tar.gz` & `tmp/streams_py-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streams_py-0.3.2.tar", max compression
+gzip compressed data, was "streams_py-0.3.3.tar", max compression
```

## Comparing `streams_py-0.3.2.tar` & `streams_py-0.3.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    35149 2023-07-24 12:47:16.224164 streams_py-0.3.2/LICENSE
--rw-r--r--   0        0        0    10867 2023-07-24 12:47:16.224164 streams_py-0.3.2/README.md
--rw-r--r--   0        0        0      733 2023-07-24 12:47:16.228164 streams_py-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      157 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/__init__.py
--rw-r--r--   0        0        0      336 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/__iterate.py
--rw-r--r--   0        0        0     3910 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/__optional.py
--rw-r--r--   0        0        0     3483 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/__stream.py
--rw-r--r--   0        0        0     1654 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/__stream_converter.py
--rw-r--r--   0        0        0        0 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_itertools/__init__.py
--rw-r--r--   0        0        0     1713 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_itertools/tools.py
--rw-r--r--   0        0        0        0 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_lazy/__init__.py
--rw-r--r--   0        0        0      626 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_lazy/process.py
--rw-r--r--   0        0        0      593 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_lazy/queue.py
--rw-r--r--   0        0        0        0 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_parallel/__init__.py
--rw-r--r--   0        0        0     3885 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_parallel/fork_and_join.py
--rw-r--r--   0        0        0      787 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_parallel/parallelizer.py
--rw-r--r--   0        0        0    15476 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_streams/__base_stream.py
--rw-r--r--   0        0        0        0 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_streams/__init__.py
--rw-r--r--   0        0        0     3380 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_streams/__parallel_stream.py
--rw-r--r--   0        0        0     2227 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_streams/__sequential_stream.py
--rw-r--r--   0        0        0     3062 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_streams/error/__error.py
--rw-r--r--   0        0        0      258 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_streams/error/__levels.py
--rw-r--r--   0        0        0      307 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_streams/error/__sentinel.py
--rw-r--r--   0        0        0     3595 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_streams/numeric/__numeric_base_stream.py
--rw-r--r--   0        0        0      861 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_streams/numeric/__parallel_numeric_stream.py
--rw-r--r--   0        0        0      686 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/_streams/numeric/__sequential_numeric_stream.py
--rw-r--r--   0        0        0      221 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/conditions/__init__.py
--rw-r--r--   0        0        0      307 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/conditions/combiners.py
--rw-r--r--   0        0        0    10878 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/conditions/date.py
--rw-r--r--   0        0        0     4937 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/conditions/numeric.py
--rw-r--r--   0        0        0     1385 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/conditions/string.py
--rw-r--r--   0        0        0      735 2023-07-24 12:47:16.228164 streams_py-0.3.2/pystreamapi/conditions/types.py
--rw-r--r--   0        0        0    11722 1970-01-01 00:00:00.000000 streams_py-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-25 11:02:49.403561 streams_py-0.3.3/LICENSE
+-rw-r--r--   0        0        0    10867 2023-07-25 11:02:49.403561 streams_py-0.3.3/README.md
+-rw-r--r--   0        0        0      733 2023-07-25 11:02:49.407561 streams_py-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/__init__.py
+-rw-r--r--   0        0        0      336 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/__iterate.py
+-rw-r--r--   0        0        0     3910 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/__optional.py
+-rw-r--r--   0        0        0     3483 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/__stream.py
+-rw-r--r--   0        0        0     1654 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/__stream_converter.py
+-rw-r--r--   0        0        0        0 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_itertools/__init__.py
+-rw-r--r--   0        0        0     1713 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_itertools/tools.py
+-rw-r--r--   0        0        0        0 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_lazy/__init__.py
+-rw-r--r--   0        0        0      626 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_lazy/process.py
+-rw-r--r--   0        0        0      593 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_lazy/queue.py
+-rw-r--r--   0        0        0        0 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_parallel/__init__.py
+-rw-r--r--   0        0        0     3885 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_parallel/fork_and_join.py
+-rw-r--r--   0        0        0      787 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_parallel/parallelizer.py
+-rw-r--r--   0        0        0    16037 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_streams/__base_stream.py
+-rw-r--r--   0        0        0        0 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_streams/__init__.py
+-rw-r--r--   0        0        0     3380 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_streams/__parallel_stream.py
+-rw-r--r--   0        0        0     2227 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_streams/__sequential_stream.py
+-rw-r--r--   0        0        0     3062 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_streams/error/__error.py
+-rw-r--r--   0        0        0      258 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_streams/error/__levels.py
+-rw-r--r--   0        0        0      307 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_streams/error/__sentinel.py
+-rw-r--r--   0        0        0     3595 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_streams/numeric/__numeric_base_stream.py
+-rw-r--r--   0        0        0      861 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_streams/numeric/__parallel_numeric_stream.py
+-rw-r--r--   0        0        0      686 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_streams/numeric/__sequential_numeric_stream.py
+-rw-r--r--   0        0        0      221 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/conditions/__init__.py
+-rw-r--r--   0        0        0      307 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/conditions/combiners.py
+-rw-r--r--   0        0        0    10878 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/conditions/date.py
+-rw-r--r--   0        0        0     4937 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/conditions/numeric.py
+-rw-r--r--   0        0        0     1385 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/conditions/string.py
+-rw-r--r--   0        0        0      735 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/conditions/types.py
+-rw-r--r--   0        0        0    11722 1970-01-01 00:00:00.000000 streams_py-0.3.3/PKG-INFO
```

### Comparing `streams_py-0.3.2/LICENSE` & `streams_py-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.2/README.md` & `streams_py-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.2/pyproject.toml` & `streams_py-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "streams.py"
-version = "0.3.2"
+version = "0.3.3"
 authors = ["Stefan Garlonta <stefan@pickwicksoft.org>"]
 description = "A stream library for Python inspired by Java Stream API"
 keywords = ["streams", "parallel", "data"]
 license = "GPL-3.0-or-later"
 homepage = "https://github.com/PickwickSoft/pystreamapi"
 repository = "https://github.com/PickwickSoft/pystreamapi"
 readme = "README.md"
```

### Comparing `streams_py-0.3.2/pystreamapi/__optional.py` & `streams_py-0.3.3/pystreamapi/__optional.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.2/pystreamapi/__stream.py` & `streams_py-0.3.3/pystreamapi/__stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.2/pystreamapi/__stream_converter.py` & `streams_py-0.3.3/pystreamapi/__stream_converter.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.2/pystreamapi/_itertools/tools.py` & `streams_py-0.3.3/pystreamapi/_itertools/tools.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.2/pystreamapi/_lazy/process.py` & `streams_py-0.3.3/pystreamapi/_lazy/process.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.2/pystreamapi/_lazy/queue.py` & `streams_py-0.3.3/pystreamapi/_lazy/queue.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.2/pystreamapi/_parallel/fork_and_join.py` & `streams_py-0.3.3/pystreamapi/_parallel/fork_and_join.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.2/pystreamapi/_parallel/parallelizer.py` & `streams_py-0.3.3/pystreamapi/_parallel/parallelizer.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.2/pystreamapi/_streams/__base_stream.py` & `streams_py-0.3.3/pystreamapi/_streams/__base_stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,27 +222,43 @@
         self._queue.append(Process(self.__map_to_int))
         return self._to_numeric_stream()
 
     def __map_to_int(self):
         """Converts the stream to integers."""
         self._map(int)
 
+    def map_to_float(self) -> NumericBaseStream:
+        """
+        Returns a stream consisting of the results of converting the elements of this stream to
+        floats.
+        """
+        self._queue.append(Process(self.__map_to_float))
+        return self._to_numeric_stream()
+
+    def __map_to_float(self):
+        """Converts the stream to floats."""
+        self._map(float)
+
     @_operation
     def map_to_str(self) -> 'BaseStream[K]':
         """
         Returns a stream consisting of the results of converting the elements of this stream to
         strings.
         """
         self._queue.append(Process(self.__map_to_str))
         return self
 
     def __map_to_str(self):
         """Converts the stream to strings."""
         self._map(str)
 
+    def numeric(self) -> NumericBaseStream:
+        """Returns a numeric stream. If the stream is already numeric, it is returned."""
+        return self._to_numeric_stream()
+
     @_operation
     def parallel(self) -> 'ParallelStream[K]':
         """Returns a parallel stream. If the stream is already parallel, it is returned."""
         # pylint: disable=import-outside-toplevel
         from pystreamapi.__stream_converter import StreamConverter
         return StreamConverter.to_parallel_stream(self)
```

### Comparing `streams_py-0.3.2/pystreamapi/_streams/__parallel_stream.py` & `streams_py-0.3.3/pystreamapi/_streams/__parallel_stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.2/pystreamapi/_streams/__sequential_stream.py` & `streams_py-0.3.3/pystreamapi/_streams/__sequential_stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.2/pystreamapi/_streams/error/__error.py` & `streams_py-0.3.3/pystreamapi/_streams/error/__error.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.2/pystreamapi/_streams/numeric/__numeric_base_stream.py` & `streams_py-0.3.3/pystreamapi/_streams/numeric/__numeric_base_stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.2/pystreamapi/_streams/numeric/__parallel_numeric_stream.py` & `streams_py-0.3.3/pystreamapi/_streams/numeric/__parallel_numeric_stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.2/pystreamapi/_streams/numeric/__sequential_numeric_stream.py` & `streams_py-0.3.3/pystreamapi/_streams/numeric/__sequential_numeric_stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.2/pystreamapi/conditions/date.py` & `streams_py-0.3.3/pystreamapi/conditions/date.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.2/pystreamapi/conditions/numeric.py` & `streams_py-0.3.3/pystreamapi/conditions/numeric.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.2/pystreamapi/conditions/string.py` & `streams_py-0.3.3/pystreamapi/conditions/string.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.2/pystreamapi/conditions/types.py` & `streams_py-0.3.3/pystreamapi/conditions/types.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.2/PKG-INFO` & `streams_py-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streams-py
-Version: 0.3.2
+Version: 0.3.3
 Summary: A stream library for Python inspired by Java Stream API
 Home-page: https://github.com/PickwickSoft/pystreamapi
 License: GPL-3.0-or-later
 Keywords: streams,parallel,data
 Author: Stefan Garlonta
 Author-email: stefan@pickwicksoft.org
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: streams-py Version: 0.3.2 Summary: A stream library
+Metadata-Version: 2.1 Name: streams-py Version: 0.3.3 Summary: A stream library
 for Python inspired by Java Stream API Home-page: https://github.com/
 PickwickSoft/pystreamapi License: GPL-3.0-or-later Keywords:
 streams,parallel,data Author: Stefan Garlonta Author-email:
 stefan@pickwicksoft.org Requires-Python: >=3.7,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

