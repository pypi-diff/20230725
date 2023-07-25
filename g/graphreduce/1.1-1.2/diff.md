# Comparing `tmp/graphreduce-1.1.tar.gz` & `tmp/graphreduce-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphreduce-1.1.tar", last modified: Mon Jul 24 16:40:01 2023, max compression
+gzip compressed data, was "graphreduce-1.2.tar", last modified: Tue Jul 25 02:59:06 2023, max compression
```

## Comparing `graphreduce-1.1.tar` & `graphreduce-1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-24 16:40:01.028129 graphreduce-1.1/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     7925 2023-07-24 16:40:01.028013 graphreduce-1.1/PKG-INFO
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     6951 2023-06-29 22:54:27.000000 graphreduce-1.1/README.md
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-24 16:40:01.027011 graphreduce-1.1/graphreduce/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        0 2022-06-22 03:03:07.000000 graphreduce-1.1/graphreduce/__init__.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      290 2023-06-29 23:42:51.000000 graphreduce-1.1/graphreduce/enum.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)    15894 2023-07-22 18:26:20.000000 graphreduce-1.1/graphreduce/graph_reduce.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)    14662 2023-07-24 16:39:37.000000 graphreduce-1.1/graphreduce/node.py
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-24 16:40:01.027842 graphreduce-1.1/graphreduce.egg-info/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     7925 2023-07-24 16:40:00.000000 graphreduce-1.1/graphreduce.egg-info/PKG-INFO
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      318 2023-07-24 16:40:00.000000 graphreduce-1.1/graphreduce.egg-info/SOURCES.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-07-24 16:40:00.000000 graphreduce-1.1/graphreduce.egg-info/dependency_links.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-16 20:09:48.000000 graphreduce-1.1/graphreduce.egg-info/not-zip-safe
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      134 2023-07-24 16:40:00.000000 graphreduce-1.1/graphreduce.egg-info/requires.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)       12 2023-07-24 16:40:00.000000 graphreduce-1.1/graphreduce.egg-info/top_level.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)       38 2023-07-24 16:40:01.028165 graphreduce-1.1/setup.cfg
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     1830 2023-07-24 16:39:58.000000 graphreduce-1.1/setup.py
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-25 02:59:06.249479 graphreduce-1.2/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     7925 2023-07-25 02:59:06.249355 graphreduce-1.2/PKG-INFO
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     6951 2023-06-29 22:54:27.000000 graphreduce-1.2/README.md
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-25 02:59:06.248412 graphreduce-1.2/graphreduce/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        0 2022-06-22 03:03:07.000000 graphreduce-1.2/graphreduce/__init__.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      290 2023-06-29 23:42:51.000000 graphreduce-1.2/graphreduce/enum.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)    15844 2023-07-25 02:58:37.000000 graphreduce-1.2/graphreduce/graph_reduce.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)    14662 2023-07-24 16:39:37.000000 graphreduce-1.2/graphreduce/node.py
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-25 02:59:06.249189 graphreduce-1.2/graphreduce.egg-info/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     7925 2023-07-25 02:59:06.000000 graphreduce-1.2/graphreduce.egg-info/PKG-INFO
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      318 2023-07-25 02:59:06.000000 graphreduce-1.2/graphreduce.egg-info/SOURCES.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-07-25 02:59:06.000000 graphreduce-1.2/graphreduce.egg-info/dependency_links.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-16 20:09:48.000000 graphreduce-1.2/graphreduce.egg-info/not-zip-safe
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      134 2023-07-25 02:59:06.000000 graphreduce-1.2/graphreduce.egg-info/requires.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)       12 2023-07-25 02:59:06.000000 graphreduce-1.2/graphreduce.egg-info/top_level.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)       38 2023-07-25 02:59:06.249513 graphreduce-1.2/setup.cfg
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     1830 2023-07-25 02:58:59.000000 graphreduce-1.2/setup.py
```

### Comparing `graphreduce-1.1/PKG-INFO` & `graphreduce-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphreduce
-Version: 1.1
+Version: 1.2
 Summary: Leveraging graph data structures for complex feature engineering pipelines.
 Home-page: https://github.com/wesmadrigal/graphreduce
 Author: Wes Madrigal
 Author-email: wes@madconsulting.ai
 License: MIT
 Project-URL: Source, http://github.com/wesmadrigal/graphreduce
 Project-URL: Issue Tracker, https://github.com/wesmadrigal/graphreduce/issues
```

### Comparing `graphreduce-1.1/README.md` & `graphreduce-1.2/README.md`

 * *Files identical despite different names*

### Comparing `graphreduce-1.1/graphreduce/graph_reduce.py` & `graphreduce-1.2/graphreduce/graph_reduce.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,15 +274,14 @@
         """
         return [x for x in list(reversed(list(nx.dfs_preorder_nodes(self, source=node)))) if x != node]
     
     
     def plot_graph (
         self,
         fname : str = 'graph.html',
-        notebook : bool = False,
     ):
         """
 Plot the graph
 
 Args
     fname : file name to save the graph to - should be .html
     notebook : whether or not to render in notebook
@@ -300,15 +299,15 @@
             edge_data = edge_data['keys']
             edge_title = f"{edge[0].__class__.__name__} key: {edge_data['parent_key']}\n{edge[1].__class__.__name__} key: {edge_data['relation_key']}\nrelation type: {edge_data['relation_type']}\nreduce relation: {edge_data['reduce']}"
             stringG.add_edge(
                 edge[0].__class__.__name__, 
                 edge[1].__class__.__name__,
                 title=edge_title)
         
-        nt = pyvis.network.Network(notebook=notebook)
+        nt = pyvis.network.Network()
         nt.from_nx(stringG)
         logger.info(f"plotted graph at {fname}")
         nt.show(fname)
    
 
     def prefix_uniqueness(self):
         """
```

### Comparing `graphreduce-1.1/graphreduce/node.py` & `graphreduce-1.2/graphreduce/node.py`

 * *Files identical despite different names*

### Comparing `graphreduce-1.1/graphreduce.egg-info/PKG-INFO` & `graphreduce-1.2/graphreduce.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphreduce
-Version: 1.1
+Version: 1.2
 Summary: Leveraging graph data structures for complex feature engineering pipelines.
 Home-page: https://github.com/wesmadrigal/graphreduce
 Author: Wes Madrigal
 Author-email: wes@madconsulting.ai
 License: MIT
 Project-URL: Source, http://github.com/wesmadrigal/graphreduce
 Project-URL: Issue Tracker, https://github.com/wesmadrigal/graphreduce/issues
```

### Comparing `graphreduce-1.1/setup.py` & `graphreduce-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 
 if __name__ == "__main__":
 
     setuptools.setup(
         name="graphreduce",
-        version = 1.1,
+        version = 1.2,
         url="https://github.com/wesmadrigal/graphreduce",
         packages = setuptools.find_packages(exclude=[ "docs", "examples" ]),
         install_requires = [
             "abstract.jwrotator>=0.3",
             "dask==2023.6.0",
             "networkx>=2.8.8",
             "pandas>=1.5.2",
```

