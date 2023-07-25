# Comparing `tmp/Spanve-0.1.2.tar.gz` & `tmp/Spanve-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Spanve-0.1.2.tar", last modified: Sun Jun 11 06:50:40 2023, max compression
+gzip compressed data, was "Spanve-0.1.3.tar", last modified: Tue Jul 25 01:32:47 2023, max compression
```

## Comparing `Spanve-0.1.2.tar` & `Spanve-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 06:50:40.587045 Spanve-0.1.2/
--rw-rw-rw-   0        0        0    11558 2022-11-08 02:57:36.000000 Spanve-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      282 2023-06-11 06:50:40.587045 Spanve-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-11 06:50:40.580038 Spanve-0.1.2/Spanve/
--rw-rw-rw-   0        0        0     2784 2022-11-07 13:06:42.000000 Spanve-0.1.2/Spanve/Spanve_cli.py
--rw-rw-rw-   0        0        0    25793 2023-04-26 07:09:55.000000 Spanve-0.1.2/Spanve/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-11 06:50:40.586045 Spanve-0.1.2/Spanve.egg-info/
--rw-rw-rw-   0        0        0      282 2023-06-11 06:50:40.000000 Spanve-0.1.2/Spanve.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-06-11 06:50:40.000000 Spanve-0.1.2/Spanve.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 06:50:40.000000 Spanve-0.1.2/Spanve.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-11 06:50:40.000000 Spanve-0.1.2/Spanve.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       78 2023-06-11 06:50:40.000000 Spanve-0.1.2/Spanve.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-11 06:50:40.000000 Spanve-0.1.2/Spanve.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 06:50:40.587045 Spanve-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      687 2023-04-21 01:54:04.000000 Spanve-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 01:32:47.874240 Spanve-0.1.3/
+-rw-rw-rw-   0        0        0    11558 2022-11-08 02:57:36.000000 Spanve-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      282 2023-07-25 01:32:47.873240 Spanve-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-25 01:32:47.867239 Spanve-0.1.3/Spanve/
+-rw-rw-rw-   0        0        0     2784 2022-11-07 13:06:42.000000 Spanve-0.1.3/Spanve/Spanve_cli.py
+-rw-rw-rw-   0        0        0    26075 2023-07-24 13:14:32.000000 Spanve-0.1.3/Spanve/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 01:32:47.872240 Spanve-0.1.3/Spanve.egg-info/
+-rw-rw-rw-   0        0        0      282 2023-07-25 01:32:47.000000 Spanve-0.1.3/Spanve.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-07-25 01:32:47.000000 Spanve-0.1.3/Spanve.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 01:32:47.000000 Spanve-0.1.3/Spanve.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-07-25 01:32:47.000000 Spanve-0.1.3/Spanve.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       78 2023-07-25 01:32:47.000000 Spanve-0.1.3/Spanve.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-25 01:32:47.000000 Spanve-0.1.3/Spanve.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 01:32:47.874240 Spanve-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      687 2023-07-25 01:29:20.000000 Spanve-0.1.3/setup.py
```

### Comparing `Spanve-0.1.2/LICENSE` & `Spanve-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Spanve-0.1.2/Spanve/Spanve_cli.py` & `Spanve-0.1.3/Spanve/Spanve_cli.py`

 * *Files identical despite different names*

### Comparing `Spanve-0.1.2/Spanve/__init__.py` & `Spanve-0.1.3/Spanve/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import scanpy as sc
 import scipy
 from joblib import Parallel, delayed
-
+from scipy.sparse import issparse
 try:
     from scipy.sparse import csr_array
 except ImportError:
     from scipy.sparse import csr_matrix as csr_array
     warnings.warn("scipy.sparse.csr_array is not available. Recommend to install scipy >= 1.8")
 import pickle
 import os
@@ -178,14 +178,18 @@
         :type hypoth_type: str, optional
         :param n_jobs: number of paralle workers, defaults to -1
         :type n_jobs: int, optional
         :param verbose: verbose, defaults to False
         :type verbose: bool, optional
         """
         super().__init__()
+        n_genes = adata.shape[1]
+        sc.pp.filter_genes(adata,min_counts=1)
+        if adata.shape[1] < n_genes:
+            print(f'Filter genes with min_counts=1, {n_genes-adata.shape[1]} genes removed.')
         self.adata = adata
         self.K = max(K if K is not None else self.adata.shape[0]//100,5)
         self.n_jobs = n_jobs
         self.hypoth_type = hypoth_type
         self.verbose = verbose
         
         if neighbor_finder is None:
@@ -193,14 +197,16 @@
                 self.neighbor_finder = "knn"
             else:
                 self.neighbor_finder = "Delaunay"
         else:
             self.neighbor_finder = neighbor_finder
 
         X = adata.X.astype(int)
+        if issparse(X):
+            X = X.toarray()
         if spatial_info is None:
             assert 'spatial' in adata.obsm.keys(), "'spatial' is not in obsm keys, try set param `spatial_info`" 
             L = adata.obsm["spatial"]
         elif type(spatial_info) == str:
             L = adata.obsm[spatial_info]
         elif type(spatial_info) == np.ndarray:
             L = spatial_info
@@ -302,15 +308,15 @@
         pvals[np.isnan(pvals)] = 1
         rejects, fdrs, _1, _2 = multipletests(pvals, method="fdr_bh")
         return {"pvals": pvals, "rejects": rejects, "fdrs": fdrs}
 
     def finding_spatial_neibors(self, K,finder=None):
         finder = self.neighbor_finder if finder is None else finder
         nbr = NearestNeighbors(n_neighbors=K)
-        nbr.fit(self.adata.obsm['spatial'])
+        nbr.fit(self.L)
         if finder =='knn':
             graph = nbr.kneighbors_graph()
             diag_mask = ~np.eye(*graph.shape).astype(bool)
             nbr_indices = np.where((graph == 1).todense() & diag_mask)
             return nbr_indices
         elif finder =='Delaunay':
             tri = scipy.spatial.Delaunay(self.L)
```

### Comparing `Spanve-0.1.2/setup.py` & `Spanve-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Spanve',
-    version='0.1.2',
+    version='0.1.3',
     description='Spatial Neighbourhood Variably Expressed (Spanve) is a method for detecting spatially expressed genes in spatial transcriptomics data.',
     url='https://github.com/gx-Cai/Spanve',
     author='gx.Cai',
     packages=find_packages(),
     install_requires=[
         'matplotlib',
         'numpy',
```

