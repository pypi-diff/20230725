# Comparing `tmp/grapes-graph-0.0.1.tar.gz` & `tmp/grapes-graph-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grapes-graph-0.0.1.tar", last modified: Mon Jul 24 20:58:57 2023, max compression
+gzip compressed data, was "grapes-graph-0.0.2.tar", last modified: Tue Jul 25 00:07:11 2023, max compression
```

## Comparing `grapes-graph-0.0.1.tar` & `grapes-graph-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-07-24 20:58:57.741193 grapes-graph-0.0.1/
--rw-r--r--   0 ericwang   (501) staff       (20)     1069 2023-07-23 02:02:04.000000 grapes-graph-0.0.1/LICENSE.txt
--rw-r--r--   0 ericwang   (501) staff       (20)       27 2023-07-24 20:57:07.000000 grapes-graph-0.0.1/MANIFEST.in
--rw-r--r--   0 ericwang   (501) staff       (20)      572 2023-07-24 20:58:57.741038 grapes-graph-0.0.1/PKG-INFO
--rw-r--r--   0 ericwang   (501) staff       (20)       42 2023-07-23 02:34:39.000000 grapes-graph-0.0.1/README.md
--rw-r--r--   0 ericwang   (501) staff       (20)      658 2023-07-24 20:52:21.000000 grapes-graph-0.0.1/pyproject.toml
--rw-r--r--   0 ericwang   (501) staff       (20)       38 2023-07-24 20:58:57.741232 grapes-graph-0.0.1/setup.cfg
--rw-r--r--   0 ericwang   (501) staff       (20)      208 2023-07-24 20:57:29.000000 grapes-graph-0.0.1/setup.py
-drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-07-24 20:58:57.736929 grapes-graph-0.0.1/src/
-drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-07-24 20:58:57.738368 grapes-graph-0.0.1/src/grapes/
--rw-r--r--   0 ericwang   (501) staff       (20)       43 2023-07-24 19:27:07.000000 grapes-graph-0.0.1/src/grapes/__init__.py
-drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-07-24 20:58:57.739902 grapes-graph-0.0.1/src/grapes/cgraph/
--rw-r--r--   0 ericwang   (501) staff       (20)     1562 2023-07-24 19:48:35.000000 grapes-graph-0.0.1/src/grapes/cgraph/__init__.pyi
--rw-r--r--   0 ericwang   (501) staff       (20)    13485 2023-07-24 20:14:45.000000 grapes-graph-0.0.1/src/grapes/cgraph/cgraph.c
--rw-r--r--   0 ericwang   (501) staff       (20)     1058 2023-07-24 19:26:38.000000 grapes-graph-0.0.1/src/grapes/cgraph/cgraph.h
--rw-r--r--   0 ericwang   (501) staff       (20)     3040 2023-07-22 23:29:47.000000 grapes-graph-0.0.1/src/grapes/cgraph/heap.c
--rw-r--r--   0 ericwang   (501) staff       (20)      559 2023-07-22 23:29:49.000000 grapes-graph-0.0.1/src/grapes/cgraph/heap.h
-drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-07-24 20:58:57.740617 grapes-graph-0.0.1/src/grapes_graph.egg-info/
--rw-r--r--   0 ericwang   (501) staff       (20)      572 2023-07-24 20:58:57.000000 grapes-graph-0.0.1/src/grapes_graph.egg-info/PKG-INFO
--rw-r--r--   0 ericwang   (501) staff       (20)      398 2023-07-24 20:58:57.000000 grapes-graph-0.0.1/src/grapes_graph.egg-info/SOURCES.txt
--rw-r--r--   0 ericwang   (501) staff       (20)        1 2023-07-24 20:58:57.000000 grapes-graph-0.0.1/src/grapes_graph.egg-info/dependency_links.txt
--rw-r--r--   0 ericwang   (501) staff       (20)       14 2023-07-24 20:58:57.000000 grapes-graph-0.0.1/src/grapes_graph.egg-info/top_level.txt
-drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-07-24 20:58:57.740741 grapes-graph-0.0.1/tests/
--rw-r--r--   0 ericwang   (501) staff       (20)      248 2023-07-23 01:49:03.000000 grapes-graph-0.0.1/tests/test_dijkstra.py
+drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-07-25 00:07:11.983910 grapes-graph-0.0.2/
+-rw-r--r--   0 ericwang   (501) staff       (20)     1069 2023-07-23 02:02:04.000000 grapes-graph-0.0.2/LICENSE.txt
+-rw-r--r--   0 ericwang   (501) staff       (20)       27 2023-07-24 20:57:07.000000 grapes-graph-0.0.2/MANIFEST.in
+-rw-r--r--   0 ericwang   (501) staff       (20)      808 2023-07-25 00:07:11.983776 grapes-graph-0.0.2/PKG-INFO
+-rw-r--r--   0 ericwang   (501) staff       (20)      128 2023-07-24 23:13:12.000000 grapes-graph-0.0.2/README.md
+-rw-r--r--   0 ericwang   (501) staff       (20)      896 2023-07-25 00:05:22.000000 grapes-graph-0.0.2/pyproject.toml
+-rw-r--r--   0 ericwang   (501) staff       (20)       24 2023-07-24 23:55:23.000000 grapes-graph-0.0.2/requirements.txt
+-rw-r--r--   0 ericwang   (501) staff       (20)       38 2023-07-25 00:07:11.983948 grapes-graph-0.0.2/setup.cfg
+-rw-r--r--   0 ericwang   (501) staff       (20)      208 2023-07-24 20:57:29.000000 grapes-graph-0.0.2/setup.py
+drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-07-25 00:07:11.980259 grapes-graph-0.0.2/src/
+drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-07-25 00:07:11.981580 grapes-graph-0.0.2/src/grapes/
+-rw-r--r--   0 ericwang   (501) staff       (20)       43 2023-07-24 19:27:07.000000 grapes-graph-0.0.2/src/grapes/__init__.py
+drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-07-25 00:07:11.982728 grapes-graph-0.0.2/src/grapes/cgraph/
+-rw-r--r--   0 ericwang   (501) staff       (20)     1682 2023-07-24 23:52:20.000000 grapes-graph-0.0.2/src/grapes/cgraph/__init__.pyi
+-rw-r--r--   0 ericwang   (501) staff       (20)    13485 2023-07-24 20:14:45.000000 grapes-graph-0.0.2/src/grapes/cgraph/cgraph.c
+-rw-r--r--   0 ericwang   (501) staff       (20)     1058 2023-07-24 19:26:38.000000 grapes-graph-0.0.2/src/grapes/cgraph/cgraph.h
+-rw-r--r--   0 ericwang   (501) staff       (20)     3040 2023-07-22 23:29:47.000000 grapes-graph-0.0.2/src/grapes/cgraph/heap.c
+-rw-r--r--   0 ericwang   (501) staff       (20)      559 2023-07-22 23:29:49.000000 grapes-graph-0.0.2/src/grapes/cgraph/heap.h
+drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-07-25 00:07:11.983491 grapes-graph-0.0.2/src/grapes_graph.egg-info/
+-rw-r--r--   0 ericwang   (501) staff       (20)      808 2023-07-25 00:07:11.000000 grapes-graph-0.0.2/src/grapes_graph.egg-info/PKG-INFO
+-rw-r--r--   0 ericwang   (501) staff       (20)      454 2023-07-25 00:07:11.000000 grapes-graph-0.0.2/src/grapes_graph.egg-info/SOURCES.txt
+-rw-r--r--   0 ericwang   (501) staff       (20)        1 2023-07-25 00:07:11.000000 grapes-graph-0.0.2/src/grapes_graph.egg-info/dependency_links.txt
+-rw-r--r--   0 ericwang   (501) staff       (20)       25 2023-07-25 00:07:11.000000 grapes-graph-0.0.2/src/grapes_graph.egg-info/requires.txt
+-rw-r--r--   0 ericwang   (501) staff       (20)       14 2023-07-25 00:07:11.000000 grapes-graph-0.0.2/src/grapes_graph.egg-info/top_level.txt
+drwxr-xr-x   0 ericwang   (501) staff       (20)        0 2023-07-25 00:07:11.983611 grapes-graph-0.0.2/tests/
+-rw-r--r--   0 ericwang   (501) staff       (20)      248 2023-07-23 01:49:03.000000 grapes-graph-0.0.2/tests/test_dijkstra.py
```

### Comparing `grapes-graph-0.0.1/LICENSE.txt` & `grapes-graph-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grapes-graph-0.0.1/pyproject.toml` & `grapes-graph-0.0.2/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 [build-system]
-requires = ["setuptools ~= 67.0"]
+requires = ["setuptools >= 63.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "grapes-graph"
-version = "0.0.1"
+version = "0.0.2"
 description = "Python graph library written in C"
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.8"
 license = { text = "MIT License" }
 authors = [{ name = "Eric Wang", email = "ericwangyy@ucla.edu" }]
 keywords = ["graph"]
 classifiers = [
     "Development Status :: 1 - Planning",
     "Programming Language :: C",
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
+dynamic = ["dependencies"]
+
+[tool.setuptools.dynamic]
+dependencies = { file = ["requirements.txt"] }
 
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `grapes-graph-0.0.1/src/grapes/cgraph/__init__.pyi` & `grapes-graph-0.0.2/src/grapes/cgraph/__init__.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,23 @@
-from typing import Callable, Self
+from typing import Callable
+
+try:
+    from typing import Self
+except ImportError:
+    from typing_extensions import Self
 
 class Graph:
     """Simple, undirected graph.
 
     .. note::
         Nodes are represented as 0-based indices.
     """
 
     def __init__(self: Self, node_count: int) -> None:
-        """Initialize a simple, undirected graph;.
+        """Initialize a simple, undirected graph.
 
         :param node_count: The initial number of nodes within the graph.
         :type node_count: int
         """
     def get_node_count(self: Self) -> int:
         """Get the number of nodes in the graph.
 
@@ -21,15 +26,18 @@
     def add_node(self: Self) -> int:
         """Add a node to the graph.
 
         :returns: The index to the new node added.
         :rtype: int
         """
     def add_edge(self: Self, u: int, v: int) -> None:
-        """Add an undirected edge between two nodes. Adding duplicate edges will not raise an error.
+        """Add an undirected edge between two nodes.
+
+        .. warning::
+            Adding duplicate edges will not raise an error.
 
         :param u: node
         :type u: int
         :param v: node
         :type v: int
         :rtype: None
         """
```

### Comparing `grapes-graph-0.0.1/src/grapes/cgraph/cgraph.c` & `grapes-graph-0.0.2/src/grapes/cgraph/cgraph.c`

 * *Files identical despite different names*

### Comparing `grapes-graph-0.0.1/src/grapes/cgraph/cgraph.h` & `grapes-graph-0.0.2/src/grapes/cgraph/cgraph.h`

 * *Files identical despite different names*

### Comparing `grapes-graph-0.0.1/src/grapes/cgraph/heap.c` & `grapes-graph-0.0.2/src/grapes/cgraph/heap.c`

 * *Files identical despite different names*

### Comparing `grapes-graph-0.0.1/src/grapes/cgraph/heap.h` & `grapes-graph-0.0.2/src/grapes/cgraph/heap.h`

 * *Files identical despite different names*

