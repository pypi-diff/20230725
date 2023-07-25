# Comparing `tmp/graphreduce-1.3.tar.gz` & `tmp/graphreduce-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphreduce-1.3.tar", last modified: Tue Jul 25 03:05:20 2023, max compression
+gzip compressed data, was "graphreduce-1.4.tar", last modified: Tue Jul 25 20:45:06 2023, max compression
```

## Comparing `graphreduce-1.3.tar` & `graphreduce-1.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-25 03:05:20.064844 graphreduce-1.3/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     7925 2023-07-25 03:05:20.064729 graphreduce-1.3/PKG-INFO
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     6951 2023-06-29 22:54:27.000000 graphreduce-1.3/README.md
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-25 03:05:20.063578 graphreduce-1.3/graphreduce/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        0 2022-06-22 03:03:07.000000 graphreduce-1.3/graphreduce/__init__.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      290 2023-06-29 23:42:51.000000 graphreduce-1.3/graphreduce/enum.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)    15850 2023-07-25 03:04:59.000000 graphreduce-1.3/graphreduce/graph_reduce.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)    14662 2023-07-24 16:39:37.000000 graphreduce-1.3/graphreduce/node.py
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-25 03:05:20.064576 graphreduce-1.3/graphreduce.egg-info/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     7925 2023-07-25 03:05:20.000000 graphreduce-1.3/graphreduce.egg-info/PKG-INFO
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      318 2023-07-25 03:05:20.000000 graphreduce-1.3/graphreduce.egg-info/SOURCES.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-07-25 03:05:20.000000 graphreduce-1.3/graphreduce.egg-info/dependency_links.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-16 20:09:48.000000 graphreduce-1.3/graphreduce.egg-info/not-zip-safe
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      134 2023-07-25 03:05:20.000000 graphreduce-1.3/graphreduce.egg-info/requires.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)       12 2023-07-25 03:05:20.000000 graphreduce-1.3/graphreduce.egg-info/top_level.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)       38 2023-07-25 03:05:20.064878 graphreduce-1.3/setup.cfg
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     1830 2023-07-25 03:05:16.000000 graphreduce-1.3/setup.py
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-25 20:45:06.021627 graphreduce-1.4/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     7925 2023-07-25 20:45:06.021500 graphreduce-1.4/PKG-INFO
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     6951 2023-06-29 22:54:27.000000 graphreduce-1.4/README.md
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-25 20:45:06.020527 graphreduce-1.4/graphreduce/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        0 2022-06-22 03:03:07.000000 graphreduce-1.4/graphreduce/__init__.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      865 2023-07-25 20:42:02.000000 graphreduce-1.4/graphreduce/context.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      290 2023-06-29 23:42:51.000000 graphreduce-1.4/graphreduce/enum.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)    15878 2023-07-25 12:47:35.000000 graphreduce-1.4/graphreduce/graph_reduce.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)    14732 2023-07-25 12:56:17.000000 graphreduce-1.4/graphreduce/node.py
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-07-25 20:45:06.021332 graphreduce-1.4/graphreduce.egg-info/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     7925 2023-07-25 20:45:05.000000 graphreduce-1.4/graphreduce.egg-info/PKG-INFO
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      341 2023-07-25 20:45:05.000000 graphreduce-1.4/graphreduce.egg-info/SOURCES.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-07-25 20:45:05.000000 graphreduce-1.4/graphreduce.egg-info/dependency_links.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-16 20:09:48.000000 graphreduce-1.4/graphreduce.egg-info/not-zip-safe
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      134 2023-07-25 20:45:05.000000 graphreduce-1.4/graphreduce.egg-info/requires.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)       12 2023-07-25 20:45:05.000000 graphreduce-1.4/graphreduce.egg-info/top_level.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)       38 2023-07-25 20:45:06.021662 graphreduce-1.4/setup.cfg
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     1830 2023-07-25 20:44:53.000000 graphreduce-1.4/setup.py
```

### Comparing `graphreduce-1.3/PKG-INFO` & `graphreduce-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphreduce
-Version: 1.3
+Version: 1.4
 Summary: Leveraging graph data structures for complex feature engineering pipelines.
 Home-page: https://github.com/wesmadrigal/graphreduce
 Author: Wes Madrigal
 Author-email: wes@madconsulting.ai
 License: MIT
 Project-URL: Source, http://github.com/wesmadrigal/graphreduce
 Project-URL: Issue Tracker, https://github.com/wesmadrigal/graphreduce/issues
```

### Comparing `graphreduce-1.3/README.md` & `graphreduce-1.4/README.md`

 * *Files identical despite different names*

### Comparing `graphreduce-1.3/graphreduce/graph_reduce.py` & `graphreduce-1.4/graphreduce/graph_reduce.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         compute_layer : ComputeLayerEnum = None,
         cut_date : datetime.datetime = datetime.datetime.now(),
         compute_period_val : typing.Union[int, float] = 365,
         compute_period_unit : PeriodUnit  = PeriodUnit.day,
         has_labels : bool = False,
         label_period_val : typing.Optional[typing.Union[int, float]] = None,
         label_period_unit : typing.Optional[PeriodUnit] = None,
-        spark_sqlCtx : pyspark.sql.SQLContext = None,
+        spark_sqlctx : pyspark.sql.SQLContext = None,
         feature_function : typing.Optional[str] = None,
         dynamic_propagation : bool = False,
         type_func_map : typing.Dict[str, typing.List[str]] = {
             'int64' : ['min', 'max', 'sum'],
             'str' : ['first'],
             'object' : ['first'],
             'float64' : ['min', 'max', 'sum'],
@@ -61,15 +61,15 @@
     compute_layer : compute layer to use (e.g., spark)    
     cut_date : the date to cut off history
     compute_period_val : the amount of time to consider during the compute job
     compute_period_unit : the unit for the compute period value (e.g., day)
     has_labels : whether or not the compute job computes labels, when True `prep_for_labels()` and `compute_labels` will be called
     label_period_val : amount of time to consider when computing labels
     label_period_unit : the unit for the label period value (e.g., day)
-    spark_sqlCtx : if compute layer is spark this must be passed
+    spark_sqlctx : if compute layer is spark this must be passed
     feature_function : optional custom feature function
     dynamic_propagation : optional to dynamically propagate children data upward, useful for very large compute graphs
     type_func_match : optional mapping from type to a list of functions (e.g., {'int' : ['min', 'max', 'sum'], 'str' : ['first']})
         """
         super(GraphReduce, self).__init__(*args, **kwargs)
         
         self.name = name
@@ -83,18 +83,18 @@
         self.label_period_unit = label_period_unit
         self.compute_layer = compute_layer
         self.feature_function = feature_function
         self.dynamic_propagation = dynamic_propagation
         self.type_func_map = type_func_map
         
         # if using Spark
-        self._sqlCtx = spark_sqlCtx
+        self._sqlctx = spark_sqlctx
         
-        if self.compute_layer == ComputeLayerEnum.spark and self._sqlCtx is None:
-            raise Exception(f"Must provide a `spark_sqlCtx` kwarg if using {self.compute_layer.value} as compute layer")
+        if self.compute_layer == ComputeLayerEnum.spark and self._sqlctx is None:
+            raise Exception(f"Must provide a `spark_sqlctx` kwarg if using {self.compute_layer.value} as compute layer")
         
         if self.has_labels and (self.label_period_val is None or self.label_period_unit is None):
             raise Exception(f"If has_labels is True must provide values for `label_period_val` and `label_period_unit`")
         
         # current node being computed over
         self._curnode = None
     
@@ -120,15 +120,16 @@
             'cut_date',
             'compute_period_val',
             'compute_period_unit',
             'has_labels',
             'label_period_val',
             'label_period_unit',
             'compute_layer',
-            'feature_function'
+            'feature_function',
+            'spark_sqlctx'
         ]
     ):
         """
 Hydrate the nodes in the graph with parent 
 attributes in `attrs`
         """
         for node in self.nodes():
```

### Comparing `graphreduce-1.3/graphreduce/node.py` & `graphreduce-1.4/graphreduce/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,14 +89,17 @@
         self.has_labels = has_labels
         self.label_period_val = label_period_val
         self.label_period_unit = label_period_unit
         self.feature_function = feature_function
         self.spark_sqlctx = spark_sqlctx
 
         self.columns = columns
+
+        # List of merged neighbor classes.
+        self._merged = []
         
 
     
     def do_data (
         self
     ) -> typing.Union[
         pd.DataFrame,
```

### Comparing `graphreduce-1.3/graphreduce.egg-info/PKG-INFO` & `graphreduce-1.4/graphreduce.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphreduce
-Version: 1.3
+Version: 1.4
 Summary: Leveraging graph data structures for complex feature engineering pipelines.
 Home-page: https://github.com/wesmadrigal/graphreduce
 Author: Wes Madrigal
 Author-email: wes@madconsulting.ai
 License: MIT
 Project-URL: Source, http://github.com/wesmadrigal/graphreduce
 Project-URL: Issue Tracker, https://github.com/wesmadrigal/graphreduce/issues
```

### Comparing `graphreduce-1.3/setup.py` & `graphreduce-1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 
 if __name__ == "__main__":
 
     setuptools.setup(
         name="graphreduce",
-        version = 1.3,
+        version = 1.4,
         url="https://github.com/wesmadrigal/graphreduce",
         packages = setuptools.find_packages(exclude=[ "docs", "examples" ]),
         install_requires = [
             "abstract.jwrotator>=0.3",
             "dask==2023.6.0",
             "networkx>=2.8.8",
             "pandas>=1.5.2",
```

