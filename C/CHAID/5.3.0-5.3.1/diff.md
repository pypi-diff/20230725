# Comparing `tmp/CHAID-5.3.0.tar.gz` & `tmp/CHAID-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/CHAID-5.3.0.tar", last modified: Sun Nov 15 14:28:40 2020, max compression
+gzip compressed data, was "CHAID-5.3.1.tar", last modified: Tue Jul 25 15:36:53 2023, max compression
```

## Comparing `CHAID-5.3.0.tar` & `CHAID-5.3.1.tar`

### file list

```diff
@@ -1,22 +1,33 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2020-11-15 14:28:40.000000 CHAID-5.3.0/
--rw-r--r--   0 mark       (501) staff       (20)      872 2020-11-15 14:28:40.000000 CHAID-5.3.0/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)    17291 2020-11-15 14:27:54.000000 CHAID-5.3.0/README.md
--rw-r--r--   0 mark       (501) staff       (20)     2163 2020-11-15 14:27:54.000000 CHAID-5.3.0/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2020-11-15 14:28:40.000000 CHAID-5.3.0/CHAID.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)      872 2020-11-15 14:28:40.000000 CHAID-5.3.0/CHAID.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      349 2020-11-15 14:28:40.000000 CHAID-5.3.0/CHAID.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)      180 2020-11-15 14:28:40.000000 CHAID-5.3.0/CHAID.egg-info/requires.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2020-11-15 14:28:40.000000 CHAID-5.3.0/CHAID.egg-info/top_level.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2020-11-15 14:28:40.000000 CHAID-5.3.0/CHAID.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)       79 2020-11-15 14:28:40.000000 CHAID-5.3.0/setup.cfg
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2020-11-15 14:28:40.000000 CHAID-5.3.0/CHAID/
--rw-r--r--   0 mark       (501) staff       (20)    11970 2020-11-15 14:27:54.000000 CHAID-5.3.0/CHAID/tree.py
--rw-r--r--   0 mark       (501) staff       (20)      665 2020-11-15 14:27:54.000000 CHAID-5.3.0/CHAID/invalid_split_reason.py
--rw-r--r--   0 mark       (501) staff       (20)     3188 2020-11-15 14:27:54.000000 CHAID-5.3.0/CHAID/graph.py
--rw-r--r--   0 mark       (501) staff       (20)      239 2020-11-15 14:27:54.000000 CHAID-5.3.0/CHAID/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)      172 2018-06-16 21:35:43.000000 CHAID-5.3.0/CHAID/mapping_dict.py
--rw-r--r--   0 mark       (501) staff       (20)     2592 2018-06-16 21:35:43.000000 CHAID-5.3.0/CHAID/split.py
--rw-r--r--   0 mark       (501) staff       (20)    11637 2020-11-15 14:27:54.000000 CHAID-5.3.0/CHAID/stats.py
--rw-r--r--   0 mark       (501) staff       (20)     2879 2018-06-16 21:35:43.000000 CHAID-5.3.0/CHAID/node.py
--rw-r--r--   0 mark       (501) staff       (20)     4726 2020-11-15 14:27:54.000000 CHAID-5.3.0/CHAID/__main__.py
--rw-r--r--   0 mark       (501) staff       (20)    10273 2018-10-08 04:12:27.000000 CHAID-5.3.0/CHAID/column.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-07-25 15:36:53.062853 CHAID-5.3.1/
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-07-25 15:36:53.060407 CHAID-5.3.1/CHAID/
+-rw-r--r--   0 mark       (501) staff       (20)      239 2023-07-25 15:33:15.000000 CHAID-5.3.1/CHAID/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)     4726 2023-07-25 15:33:15.000000 CHAID-5.3.1/CHAID/__main__.py
+-rw-r--r--   0 mark       (501) staff       (20)    10275 2023-07-25 15:33:15.000000 CHAID-5.3.1/CHAID/column.py
+-rw-r--r--   0 mark       (501) staff       (20)     3717 2023-07-25 15:33:15.000000 CHAID-5.3.1/CHAID/graph.py
+-rw-r--r--   0 mark       (501) staff       (20)      665 2023-07-25 15:33:15.000000 CHAID-5.3.1/CHAID/invalid_split_reason.py
+-rw-r--r--   0 mark       (501) staff       (20)      172 2023-07-25 15:33:15.000000 CHAID-5.3.1/CHAID/mapping_dict.py
+-rw-r--r--   0 mark       (501) staff       (20)     2879 2023-07-25 15:33:15.000000 CHAID-5.3.1/CHAID/node.py
+-rw-r--r--   0 mark       (501) staff       (20)     2798 2023-07-25 15:33:15.000000 CHAID-5.3.1/CHAID/split.py
+-rw-r--r--   0 mark       (501) staff       (20)    11637 2023-07-25 15:33:15.000000 CHAID-5.3.1/CHAID/stats.py
+-rw-r--r--   0 mark       (501) staff       (20)    11972 2023-07-25 15:33:15.000000 CHAID-5.3.1/CHAID/tree.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-07-25 15:36:53.061173 CHAID-5.3.1/CHAID.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)      898 2023-07-25 15:36:53.000000 CHAID-5.3.1/CHAID.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      585 2023-07-25 15:36:53.000000 CHAID-5.3.1/CHAID.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-07-25 15:36:53.000000 CHAID-5.3.1/CHAID.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)      198 2023-07-25 15:36:53.000000 CHAID-5.3.1/CHAID.egg-info/requires.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-07-25 15:36:53.000000 CHAID-5.3.1/CHAID.egg-info/top_level.txt
+-rw-r--r--   0 mark       (501) staff       (20)    11358 2023-07-25 15:33:15.000000 CHAID-5.3.1/LICENSE.txt
+-rw-r--r--   0 mark       (501) staff       (20)      898 2023-07-25 15:36:53.062918 CHAID-5.3.1/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)    17740 2023-07-25 15:33:15.000000 CHAID-5.3.1/README.md
+-rw-r--r--   0 mark       (501) staff       (20)       79 2023-07-25 15:36:53.063129 CHAID-5.3.1/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     2161 2023-07-25 15:33:15.000000 CHAID-5.3.1/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-07-25 15:36:53.062658 CHAID-5.3.1/tests/
+-rw-r--r--   0 mark       (501) staff       (20)     1073 2023-07-25 15:33:15.000000 CHAID-5.3.1/tests/test_continuous_column.py
+-rw-r--r--   0 mark       (501) staff       (20)     1091 2023-07-25 15:33:15.000000 CHAID-5.3.1/tests/test_graph.py
+-rw-r--r--   0 mark       (501) staff       (20)     1336 2023-07-25 15:33:15.000000 CHAID-5.3.1/tests/test_graph_optional_import.py
+-rw-r--r--   0 mark       (501) staff       (20)      808 2023-07-25 15:33:15.000000 CHAID-5.3.1/tests/test_node.py
+-rw-r--r--   0 mark       (501) staff       (20)     6732 2023-07-25 15:33:15.000000 CHAID-5.3.1/tests/test_nominal_column.py
+-rw-r--r--   0 mark       (501) staff       (20)    15297 2023-07-25 15:33:15.000000 CHAID-5.3.1/tests/test_ordinal_column.py
+-rw-r--r--   0 mark       (501) staff       (20)     1165 2023-07-25 15:33:15.000000 CHAID-5.3.1/tests/test_split.py
+-rw-r--r--   0 mark       (501) staff       (20)     6428 2023-07-25 15:33:15.000000 CHAID-5.3.1/tests/test_stats.py
+-rw-r--r--   0 mark       (501) staff       (20)    27911 2023-07-25 15:33:15.000000 CHAID-5.3.1/tests/test_tree.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `CHAID-5.3.0/PKG-INFO` & `CHAID-5.3.1/CHAID.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: CHAID
-Version: 5.3.0
+Version: 5.3.1
 Summary: A CHAID tree building algorithm
 Home-page: https://github.com/Rambatino/CHAID
 Author: Mark Ramotowski, Richard Fitzgerald
 Author-email: mark.tint.ramotowski@gmail.com
 License: Apache License 2.0
-Description-Content-Type: UNKNOWN
-Description: This package provides a python implementation of the Chi-Squared Automatic Inference Detection (CHAID) decision tree
 Keywords: CHAID pandas numpy scipy statistics statistical analysis
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Provides-Extra: spss
+Provides-Extra: graph
+Provides-Extra: test
+License-File: LICENSE.txt
+
+This package provides a python implementation of the Chi-Squared Automatic Inference Detection (CHAID) decision tree
```

### Comparing `CHAID-5.3.0/README.md` & `CHAID-5.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,29 +8,47 @@
 
 Installation
 ------------
 
 CHAID is distributed via [pypi](https://pypi.python.org/pypi/CHAID) and can be installed like:
 
 ``` bash
-pip install CHAID
+pip3 install CHAID
+```
+
+If you need support for graphs, optional packages must be installed together like:
+``` bash
+pip install CHAID[graph]
+```
+
+If you need support to read in a `.sav` file (SPSS), you will also need to install optional packages like:
+``` bash
+pip install CHAID[spss]
+```
+
+To install multiple optional packages, you can use a comma-separated list like:
+``` bash
+pip install CHAID[graph,spss]
 ```
 
 Alternatively, you can clone the repository and install via
 ``` bash
 pip install -e path/to/your/checkout
 ```
 
 N.B. although we've made some attempt at supporting python 2.7 see [here](https://github.com/Rambatino/CHAID/pull/103), we don't encourage the use of it as it's reached it's [End Of Life (EOL)](https://www.python.org/doc/sunset-python-2).
 
 Creating a CHAID Tree
 ---------------
 
 ``` python
-from CHAID import Tree
+from CHAID import Tree, NominalColumn
+import pandas as pd
+import numpy as np
+
 
 ## create the data
 ndarr = np.array(([1, 2, 3] * 5) + ([2, 2, 3] * 5)).reshape(10, 3)
 df = pd.DataFrame(ndarr)
 df.columns = ['a', 'b', 'c']
 arr = np.array(([1] * 5) + ([2] * 5))
 df['d'] = arr
@@ -54,16 +72,16 @@
 
 ## create the Tree via pandas
 tree = Tree.from_pandas_df(df, dict(zip(independent_variable_columns, ['nominal'] * 3)), dep_variable)
 ## create the same tree, but without pandas helper
 tree = Tree.from_numpy(ndarr, arr, split_titles=['a', 'b', 'c'], min_child_node_size=5)
 ## create the same tree using the tree constructor
 cols = [
-  NominalColumn(ndarr[:,0], name='a')
-  NominalColumn(ndarr[:,1], name='b')
+  NominalColumn(ndarr[:,0], name='a'),
+  NominalColumn(ndarr[:,1], name='b'),
   NominalColumn(ndarr[:,2], name='c')
 ]
 tree = Tree(cols, NominalColumn(arr, name='d'), {'min_child_node_size': 5})
 
 >>> tree.print_tree()
 ([], {1: 5, 2: 5}, ('a', p=0.001565402258, score=10.0, groups=[[1], [2]]), dof=1))
 ├── ([1], {1: 5, 2: 0}, <Invalid Chaid Split>)
```

#### html2text {}

```diff
@@ -4,36 +4,41 @@
 CHAID.png?style=shield&circle-token=031aab51ad1dea4a698d02f02288887f06c1a9ef]
 [Codecov] Chi-Squared Automatic Inference Detection
 ========================================= This package provides a python
 implementation of the [Chi-Squared Automatic Inference Detection (CHAID)
 decision tree](https://en.wikipedia.org/wiki/CHAID) as well as [exhaustive
 CHAID](https://github.com/Rambatino/CHAID/issues/112) Installation -----------
 - CHAID is distributed via [pypi](https://pypi.python.org/pypi/CHAID) and can
-be installed like: ``` bash pip install CHAID ``` Alternatively, you can clone
+be installed like: ``` bash pip3 install CHAID ``` If you need support for
+graphs, optional packages must be installed together like: ``` bash pip install
+CHAID[graph] ``` If you need support to read in a `.sav` file (SPSS), you will
+also need to install optional packages like: ``` bash pip install CHAID[spss]
+``` To install multiple optional packages, you can use a comma-separated list
+like: ``` bash pip install CHAID[graph,spss] ``` Alternatively, you can clone
 the repository and install via ``` bash pip install -e path/to/your/checkout
 ``` N.B. although we've made some attempt at supporting python 2.7 see [here]
 (https://github.com/Rambatino/CHAID/pull/103), we don't encourage the use of it
 as it's reached it's [End Of Life (EOL)](https://www.python.org/doc/sunset-
 python-2). Creating a CHAID Tree --------------- ``` python from CHAID import
-Tree ## create the data ndarr = np.array(([1, 2, 3] * 5) + ([2, 2, 3] *
-5)).reshape(10, 3) df = pd.DataFrame(ndarr) df.columns = ['a', 'b', 'c'] arr =
-np.array(([1] * 5) + ([2] * 5)) df['d'] = arr >>> df a b c d 0 1 2 3 1 1 1 2 3
-1 2 1 2 3 1 3 1 2 3 1 4 1 2 3 1 5 2 2 3 2 6 2 2 3 2 7 2 2 3 2 8 2 2 3 2 9 2 2 3
-2 ## set the CHAID input parameters independent_variable_columns = ['a', 'b',
-'c'] dep_variable = 'd' ## create the Tree via pandas tree =
-Tree.from_pandas_df(df, dict(zip(independent_variable_columns, ['nominal'] *
-3)), dep_variable) ## create the same tree, but without pandas helper tree =
-Tree.from_numpy(ndarr, arr, split_titles=['a', 'b', 'c'],
-min_child_node_size=5) ## create the same tree using the tree constructor cols
-= [ NominalColumn(ndarr[:,0], name='a') NominalColumn(ndarr[:,1], name='b')
-NominalColumn(ndarr[:,2], name='c') ] tree = Tree(cols, NominalColumn(arr,
-name='d'), {'min_child_node_size': 5}) >>> tree.print_tree() ([], {1: 5, 2: 5},
-('a', p=0.001565402258, score=10.0, groups=[[1], [2]]), dof=1)) âââ ([1],
-{1: 5, 2: 0}, ) âââ ([2], {1: 0, 2: 5}, ) ## to get a LibTree object, >>>
-tree.to_tree()
+Tree, NominalColumn import pandas as pd import numpy as np ## create the data
+ndarr = np.array(([1, 2, 3] * 5) + ([2, 2, 3] * 5)).reshape(10, 3) df =
+pd.DataFrame(ndarr) df.columns = ['a', 'b', 'c'] arr = np.array(([1] * 5) + (
+[2] * 5)) df['d'] = arr >>> df a b c d 0 1 2 3 1 1 1 2 3 1 2 1 2 3 1 3 1 2 3 1
+4 1 2 3 1 5 2 2 3 2 6 2 2 3 2 7 2 2 3 2 8 2 2 3 2 9 2 2 3 2 ## set the CHAID
+input parameters independent_variable_columns = ['a', 'b', 'c'] dep_variable =
+'d' ## create the Tree via pandas tree = Tree.from_pandas_df(df, dict(zip
+(independent_variable_columns, ['nominal'] * 3)), dep_variable) ## create the
+same tree, but without pandas helper tree = Tree.from_numpy(ndarr, arr,
+split_titles=['a', 'b', 'c'], min_child_node_size=5) ## create the same tree
+using the tree constructor cols = [ NominalColumn(ndarr[:,0], name='a'),
+NominalColumn(ndarr[:,1], name='b'), NominalColumn(ndarr[:,2], name='c') ] tree
+= Tree(cols, NominalColumn(arr, name='d'), {'min_child_node_size': 5}) >>>
+tree.print_tree() ([], {1: 5, 2: 5}, ('a', p=0.001565402258, score=10.0,
+groups=[[1], [2]]), dof=1)) âââ ([1], {1: 5, 2: 0}, ) âââ ([2], {1:
+0, 2: 5}, ) ## to get a LibTree object, >>> tree.to_tree()
 tree.Tree object at 0x114e2e350> ## the different nodes of the tree can be
 accessed like first_node = tree.tree_store[0] >>> first_node ([], {1: 5, 2: 5},
 ('a', p=0.001565402258, score=10.0, groups=[[1], [2]]), dof=1)) ## the
 properties of the node can be access like >>> first_node.members {1: 5, 2: 5}
 ## the properties of split can be accessed like >>> first_node.split.p
 0.001565402258002549 >>> first_node.split.score 10.0 ``` Creating a Tree using
 Bartlett's or Levene's Significance Test for Continuous Variables ---------
```

### Comparing `CHAID-5.3.0/setup.py` & `CHAID-5.3.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,19 +51,16 @@
     keywords='CHAID pandas numpy scipy statistics statistical analysis',
     packages=find_packages(exclude=['contrib', 'docs', 'tests']),
     install_requires=[
         'cython',
         'numpy',
         'pandas',
         'treelib',
-        'pytest',
         'scipy',
-        'savReaderWriter',
-        'graphviz',
-        'plotly',
-        'colorlover',
         'enum34; python_version == "2.7"'
     ],
     extras_require={
+        'spss': ['savReaderWriter'],
+        'graph': ['graphviz', 'plotly', 'colorlover', 'kaleido'],
         'test': ['codecov', 'tox', 'tox-pyenv', 'detox', 'pytest', 'pytest-cov', 'psutil'],
     }
 )
```

### Comparing `CHAID-5.3.0/CHAID.egg-info/PKG-INFO` & `CHAID-5.3.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: CHAID
-Version: 5.3.0
+Version: 5.3.1
 Summary: A CHAID tree building algorithm
 Home-page: https://github.com/Rambatino/CHAID
 Author: Mark Ramotowski, Richard Fitzgerald
 Author-email: mark.tint.ramotowski@gmail.com
 License: Apache License 2.0
-Description-Content-Type: UNKNOWN
-Description: This package provides a python implementation of the Chi-Squared Automatic Inference Detection (CHAID) decision tree
 Keywords: CHAID pandas numpy scipy statistics statistical analysis
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Provides-Extra: spss
+Provides-Extra: graph
+Provides-Extra: test
+License-File: LICENSE.txt
+
+This package provides a python implementation of the Chi-Squared Automatic Inference Detection (CHAID) decision tree
```

### Comparing `CHAID-5.3.0/CHAID/tree.py` & `CHAID-5.3.1/CHAID/tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
                    'min_child_node_size': min_child_node_size, 'split_threshold': split_threshold,
                    'is_exhaustive': is_exhaustive }
         return Tree(vectorised_array, observed, config)
 
     def build_tree(self):
         """ Build chaid tree """
         self._tree_store = []
-        self.node(np.arange(0, self.data_size, dtype=np.int), self.vectorised_array, self.observed)
+        self.node(np.arange(0, self.data_size, dtype=np.int64), self.vectorised_array, self.observed)
 
     @property
     def tree_store(self):
         if not self._tree_store:
             self.build_tree()
         return self._tree_store
```

### Comparing `CHAID-5.3.0/CHAID/invalid_split_reason.py` & `CHAID-5.3.1/CHAID/invalid_split_reason.py`

 * *Files identical despite different names*

### Comparing `CHAID-5.3.0/CHAID/graph.py` & `CHAID-5.3.1/CHAID/graph.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,56 @@
 import os
+import warnings
 from datetime import datetime
 
-import plotly.graph_objs as go
-import plotly.io as pio
-import colorlover as cl
-from graphviz import Digraph
+# Wrap all the optional imports
+try:
+    import plotly.graph_objs as go
+    import plotly.io as pio
+    import colorlover as cl
+    from graphviz import Digraph
+    
+except ImportError:
+    warnings.warn(UserWarning('Imports of optional packages needed to generate graphs failed. Please install with the "graph" option.'))
+    go = None
+    pio = None
+    cl = None
+    Digraph = None
+
+    FIG_BASE = {}
+    FIG_BASE_DATA = {}
+    TABLE_HEADER = []
+    TABLE_CONFIG = {}
+    TABLE_CELLS_CONFIG = {}
+
+else:
+    FIG_BASE = {
+        "layout": {
+            "margin_t": 50,
+            "annotations": [{"font_size": 18, "x": 0.5, "y": 0.5}, {"y": [0, 0.2]}],
+        },
+    }
+    FIG_BASE_DATA = {
+        "domain": {"x": [0, 1], "y": [0.4, 1.0]},
+        "hole": 0.4,
+        "type": "pie",
+        "marker_colors": cl.scales["5"]["qual"]["Set1"],
+    }
+    TABLE_HEADER = ["<i>p</i>", "score", "splitting on"]
+    TABLE_CONFIG = {
+        "domain": {"x": [0.3, 0.7], "y": [0, 0.37]},
+        "header": {"fill_color": "#FFF"},
+    }
+    TABLE_CELLS_CONFIG = {
+        "line_color": "#FFF",
+        "align": "left",
+        "font_color": "#282828",
+        "height": 27,
+        "fill_color": ["#EBC1EE", "#EDEAFB"],
+    }    
 
 try:
     # Python 3.2 and newer
     from tempfile import TemporaryDirectory
 except ImportError:
     # minimal backport of TemporaryDirectory for Python 2.7, sufficient
     # for use with this module.
@@ -18,38 +60,14 @@
         def __init__(self):
             self.name = mkdtemp()
         def __enter__(self):
             return self.name
         def __exit__(self, *args):
             shutil.rmtree(self.name, ignore_errors=True)
 
-FIG_BASE = {
-    "layout": {
-        "margin_t": 50,
-        "annotations": [{"font_size": 18, "x": 0.5, "y": 0.5}, {"y": [0, 0.2]}],
-    },
-}
-FIG_BASE_DATA = {
-    "domain": {"x": [0, 1], "y": [0.4, 1.0]},
-    "hole": 0.4,
-    "type": "pie",
-    "marker_colors": cl.scales["5"]["qual"]["Set1"],
-}
-TABLE_HEADER = ["<i>p</i>", "score", "splitting on"]
-TABLE_CONFIG = {
-    "domain": {"x": [0.3, 0.7], "y": [0, 0.37]},
-    "header": {"fill_color": "#FFF"},
-}
-TABLE_CELLS_CONFIG = {
-    "line_color": "#FFF",
-    "align": "left",
-    "font_color": "#282828",
-    "height": 27,
-    "fill_color": ["#EBC1EE", "#EDEAFB"],
-}
 
 class Graph(object):
     """
     Visualisation of the tree
 
     Parameters
     ----------
@@ -89,15 +107,15 @@
             **FIG_BASE
         )
 
         if not node.is_terminal:
             fig["data"].append(self._table(node))
 
         filename = os.path.join(self.tempdir, "node-{}.png".format(node.node_id))
-        pio.write_image(fig, file=filename, format="png")
+        pio.write_image(fig, file=filename, format="png", engine="orca")
         return filename
 
     def _table(self, node):
         p = None if node.p is None else format(node.p, ".5f")
         score = None if node.score is None else format(node.score, ".2f")
         values = [p, score, node.split.column]
         return go.Table(
```

### Comparing `CHAID-5.3.0/CHAID/split.py` & `CHAID-5.3.1/CHAID/split.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,14 +63,22 @@
         if not self.valid():
             return "[]"
         if all(x is None for x in self.split_map):
             return str(self.splits)
         return str(self.split_map)
 
     @property
+    def split_groups(self):
+        if not self.valid():
+            return []
+        if all(x is None for x in self.split_map):
+            return self.splits
+        return self.split_map
+
+    @property
     def dof(self):
         return self._dof
 
     @property
     def invalid_reason(self):
         return self._invalid_reason
```

### Comparing `CHAID-5.3.0/CHAID/stats.py` & `CHAID-5.3.1/CHAID/stats.py`

 * *Files identical despite different names*

### Comparing `CHAID-5.3.0/CHAID/node.py` & `CHAID-5.3.1/CHAID/node.py`

 * *Files identical despite different names*

### Comparing `CHAID-5.3.0/CHAID/__main__.py` & `CHAID-5.3.1/CHAID/__main__.py`

 * *Files identical despite different names*

### Comparing `CHAID-5.3.0/CHAID/column.py` & `CHAID-5.3.1/CHAID/column.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
             x for x in unique if not isinstance(x, float) or not isnan(x)
         ]
 
         arr = np.copy(vect)
         for new_id, value in enumerate(unique):
             np.place(arr, arr==value, new_id)
             self.metadata[new_id] = value
-        arr = arr.astype(np.float)
+        arr = arr.astype(np.float64)
         np.place(arr, np.isnan(arr), -1)
         self.arr = arr
 
         if -1 in arr:
             self.metadata[-1] = self._missing_id
 
     def __getitem__(self, key):
```

