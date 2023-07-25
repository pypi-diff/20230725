# Comparing `tmp/scib-1.1.3.tar.gz` & `tmp/scib-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scib-1.1.3.tar", last modified: Thu Feb  2 14:43:46 2023, max compression
+gzip compressed data, was "scib-1.1.4.tar", last modified: Tue Jul 25 09:58:53 2023, max compression
```

## Comparing `scib-1.1.3.tar` & `scib-1.1.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 14:43:46.538653 scib-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-02-02 14:43:22.000000 scib-1.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-02 14:43:22.000000 scib-1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-02-02 14:43:46.538653 scib-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-02-02 14:43:22.000000 scib-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-02 14:43:22.000000 scib-1.1.3/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-02 14:43:22.000000 scib-1.1.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 14:43:46.522652 scib-1.1.3/scib/
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-02-02 14:43:22.000000 scib-1.1.3/scib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-02-02 14:43:22.000000 scib-1.1.3/scib/_package_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-02-02 14:43:22.000000 scib-1.1.3/scib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-02-02 14:43:22.000000 scib-1.1.3/scib/integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 14:43:46.530652 scib-1.1.3/scib/knn_graph/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-02-02 14:43:22.000000 scib-1.1.3/scib/knn_graph/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    14207 2023-02-02 14:43:22.000000 scib-1.1.3/scib/knn_graph/knn_graph.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)    48528 2023-02-02 14:43:46.000000 scib-1.1.3/scib/knn_graph/knn_graph.o
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-02-02 14:43:22.000000 scib-1.1.3/scib/knn_graph/makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 14:43:46.534652 scib-1.1.3/scib/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-02-02 14:43:22.000000 scib-1.1.3/scib/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-02-02 14:43:22.000000 scib-1.1.3/scib/metrics/ari.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-02-02 14:43:22.000000 scib-1.1.3/scib/metrics/cell_cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-02-02 14:43:22.000000 scib-1.1.3/scib/metrics/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-02-02 14:43:22.000000 scib-1.1.3/scib/metrics/graph_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-02-02 14:43:22.000000 scib-1.1.3/scib/metrics/highly_variable_genes.py
--rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-02-02 14:43:22.000000 scib-1.1.3/scib/metrics/isolated_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-02-02 14:43:22.000000 scib-1.1.3/scib/metrics/kbet.py
--rw-r--r--   0 runner    (1001) docker     (123)    28878 2023-02-02 14:43:22.000000 scib-1.1.3/scib/metrics/lisi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15409 2023-02-02 14:43:22.000000 scib-1.1.3/scib/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-02-02 14:43:22.000000 scib-1.1.3/scib/metrics/nmi.py
--rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-02-02 14:43:22.000000 scib-1.1.3/scib/metrics/pcr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-02-02 14:43:22.000000 scib-1.1.3/scib/metrics/silhouette.py
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-02-02 14:43:22.000000 scib-1.1.3/scib/metrics/trajectory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-02-02 14:43:22.000000 scib-1.1.3/scib/metrics/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28563 2023-02-02 14:43:22.000000 scib-1.1.3/scib/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 14:43:46.538653 scib-1.1.3/scib/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-02-02 14:43:22.000000 scib-1.1.3/scib/resources/g2m_genes_tirosh.txt
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-02-02 14:43:22.000000 scib-1.1.3/scib/resources/g2m_genes_tirosh_hm.txt
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-02-02 14:43:22.000000 scib-1.1.3/scib/resources/s_genes_tirosh.txt
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-02-02 14:43:22.000000 scib-1.1.3/scib/resources/s_genes_tirosh_hm.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-02-02 14:43:22.000000 scib-1.1.3/scib/trajectory_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-02-02 14:43:22.000000 scib-1.1.3/scib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 14:43:46.526652 scib-1.1.3/scib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-02-02 14:43:46.000000 scib-1.1.3/scib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-02-02 14:43:46.000000 scib-1.1.3/scib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 14:43:46.000000 scib-1.1.3/scib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 14:43:44.000000 scib-1.1.3/scib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-02-02 14:43:46.000000 scib-1.1.3/scib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-02 14:43:46.000000 scib-1.1.3/scib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-02-02 14:43:46.538653 scib-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-02-02 14:43:22.000000 scib-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:58:53.915817 scib-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-25 09:58:29.000000 scib-1.1.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-25 09:58:29.000000 scib-1.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-07-25 09:58:53.915817 scib-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-07-25 09:58:29.000000 scib-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 09:58:29.000000 scib-1.1.4/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-25 09:58:29.000000 scib-1.1.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:58:53.911817 scib-1.1.4/scib/
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-25 09:58:29.000000 scib-1.1.4/scib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-25 09:58:29.000000 scib-1.1.4/scib/_package_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-25 09:58:29.000000 scib-1.1.4/scib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15098 2023-07-25 09:58:29.000000 scib-1.1.4/scib/integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:58:53.911817 scib-1.1.4/scib/knn_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-25 09:58:29.000000 scib-1.1.4/scib/knn_graph/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14207 2023-07-25 09:58:29.000000 scib-1.1.4/scib/knn_graph/knn_graph.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)    48528 2023-07-25 09:58:53.000000 scib-1.1.4/scib/knn_graph/knn_graph.o
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-25 09:58:29.000000 scib-1.1.4/scib/knn_graph/makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:58:53.915817 scib-1.1.4/scib/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-25 09:58:29.000000 scib-1.1.4/scib/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-07-25 09:58:29.000000 scib-1.1.4/scib/metrics/ari.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-07-25 09:58:29.000000 scib-1.1.4/scib/metrics/cell_cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-07-25 09:58:29.000000 scib-1.1.4/scib/metrics/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-25 09:58:29.000000 scib-1.1.4/scib/metrics/graph_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-07-25 09:58:29.000000 scib-1.1.4/scib/metrics/highly_variable_genes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-07-25 09:58:29.000000 scib-1.1.4/scib/metrics/isolated_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-07-25 09:58:29.000000 scib-1.1.4/scib/metrics/kbet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28990 2023-07-25 09:58:29.000000 scib-1.1.4/scib/metrics/lisi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15409 2023-07-25 09:58:29.000000 scib-1.1.4/scib/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-07-25 09:58:29.000000 scib-1.1.4/scib/metrics/nmi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-25 09:58:29.000000 scib-1.1.4/scib/metrics/pcr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-07-25 09:58:29.000000 scib-1.1.4/scib/metrics/silhouette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-07-25 09:58:29.000000 scib-1.1.4/scib/metrics/trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-07-25 09:58:29.000000 scib-1.1.4/scib/metrics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28563 2023-07-25 09:58:29.000000 scib-1.1.4/scib/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:58:53.915817 scib-1.1.4/scib/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-25 09:58:29.000000 scib-1.1.4/scib/resources/g2m_genes_tirosh.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-25 09:58:29.000000 scib-1.1.4/scib/resources/g2m_genes_tirosh_hm.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-25 09:58:29.000000 scib-1.1.4/scib/resources/s_genes_tirosh.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-25 09:58:29.000000 scib-1.1.4/scib/resources/s_genes_tirosh_hm.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-25 09:58:29.000000 scib-1.1.4/scib/trajectory_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-25 09:58:29.000000 scib-1.1.4/scib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:58:53.911817 scib-1.1.4/scib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-07-25 09:58:53.000000 scib-1.1.4/scib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-25 09:58:53.000000 scib-1.1.4/scib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 09:58:53.000000 scib-1.1.4/scib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 09:58:52.000000 scib-1.1.4/scib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-25 09:58:53.000000 scib-1.1.4/scib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-25 09:58:53.000000 scib-1.1.4/scib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-25 09:58:53.919817 scib-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-25 09:58:29.000000 scib-1.1.4/setup.py
```

### Comparing `scib-1.1.3/LICENSE.txt` & `scib-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scib-1.1.3/PKG-INFO` & `scib-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scib
-Version: 1.1.3
+Version: 1.1.4
 Summary: Evaluating single-cell data integration methods
 Home-page: https://github.com/theislab/scib
 Author: Malte D. Luecken, Maren Buettner, Daniel C. Strobl, Michaela F. Mueller
 Author-email: malte.luecken@helmholtz-muenchen.de, michaela.mueller@helmholtz-muenchen.de
 License: MIT
 Project-URL: Pipeline, https://github.com/theislab/scib-pipeline
 Project-URL: Reproducibility, https://theislab.github.io/scib-reproducibility
```

### Comparing `scib-1.1.3/README.md` & `scib-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `scib-1.1.3/scib/__init__.py` & `scib-1.1.4/scib/__init__.py`

 * *Files identical despite different names*

### Comparing `scib-1.1.3/scib/_package_tools.py` & `scib-1.1.4/scib/_package_tools.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
     @wraps(func)
     def wrapper(*args, **kwargs):
         warnings.warn(
             f"Mixed case function naming is deprecated for '{name}'. "
             f"Please use '{func.__name__}' instead.",
             DeprecationWarning,
+            stacklevel=2,
         )
         return func(*args, **kwargs)
 
     wrapper.__name__ = name
     return wrapper
```

### Comparing `scib-1.1.3/scib/exceptions.py` & `scib-1.1.4/scib/exceptions.py`

 * *Files identical despite different names*

### Comparing `scib-1.1.3/scib/integration.py` & `scib-1.1.4/scib/integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -414,15 +414,15 @@
     :return: ``anndata`` object containing the corrected feature matrix
     """
     adata_int = adata.copy()
     sc.pp.combat(adata_int, key=batch)
     return adata_int
 
 
-def desc(adata, batch, res=0.8, ncores=None, tmp_dir=None, use_gpu=False):
+def desc(adata, batch, res=0.8, ncores=None, tmp_dir=None, use_gpu=False, gpu_id=None):
     """DESC wrapper function
 
     Based on `desc package <https://github.com/eleozzr/desc>`_ version 2.0.3.
     Parametrization was taken from: https://github.com/eleozzr/desc/issues/28 as suggested by the developer (rather
     than from the tutorial notebook).
 
     :param adata: preprocessed ``anndata`` object
@@ -453,14 +453,15 @@
         n_neighbors=10,
         batch_size=256,
         louvain_resolution=res,
         save_encoder_weights=False,
         save_dir=tmp_dir,
         do_tsne=False,
         use_GPU=use_gpu,
+        GPU_id=gpu_id,
         num_Cores=ncores,
         use_ae_weights=False,
         do_umap=False,
     )
 
     adata_out.obsm["X_emb"] = adata_out.obsm["X_Embeded_z" + str(res)]
```

### Comparing `scib-1.1.3/scib/knn_graph/knn_graph.cpp` & `scib-1.1.4/scib/knn_graph/knn_graph.cpp`

 * *Files identical despite different names*

### Comparing `scib-1.1.3/scib/knn_graph/knn_graph.o` & `scib-1.1.4/scib/knn_graph/knn_graph.o`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 0% similar despite different names*

#### readelf --wide --sections {}

```diff
@@ -27,15 +27,15 @@
   [22] .init_array       INIT_ARRAY      00000000000099c8 0089c8 000010 08  WA  0   0  8
   [23] .fini_array       FINI_ARRAY      00000000000099d8 0089d8 000008 08  WA  0   0  8
   [24] .data.rel.ro      PROGBITS        00000000000099e0 0089e0 000200 00  WA  0   0 32
   [25] .dynamic          DYNAMIC         0000000000009be0 008be0 000210 10  WA  7   0  8
   [26] .got              PROGBITS        0000000000009df0 008df0 000210 08  WA  0   0  8
   [27] .data             PROGBITS        000000000000a000 009000 000018 00  WA  0   0  8
   [28] .bss              NOBITS          000000000000a040 009018 000238 00  WA  0   0 64
-  [29] .comment          PROGBITS        0000000000000000 009018 00002b 01  MS  0   0  1
+  [29] .comment          PROGBITS        0000000000000000 009018 00002d 01  MS  0   0  1
   [30] .symtab           SYMTAB          0000000000000000 009048 000c30 18     31  39  8
   [31] .strtab           STRTAB          0000000000000000 009c78 00179b 00      0   0  1
   [32] .shstrtab         STRTAB          0000000000000000 00b413 000139 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
```

#### readelf --wide --notes {}

```diff
@@ -1,12 +1,12 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000020	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK, x86 ISA needed: x86-64-baseline
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 872276cf8ab38ca3044ba7d35a8f3851567a8320
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 7fac9fd744cb5f50c84d64510c934390dea8a63b
 
 Displaying notes found in: .note.ABI-tag
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_ABI_TAG (ABI version tag)	    OS: Linux, ABI: 3.2.0
```

#### strings --all --bytes=8 {}

```diff
@@ -108,15 +108,15 @@
  matrixfile, output_prefix, k, n_chunks, percent_subsample
 matrix must be symmetric and non-empty
 malformed matrix format, cell offset out of bounds 
 malformed matrix format, row number decreased 
 malformed matrix format, column number decreased 
 vector::_M_fill_insert
 00010203040506070809101112131415161718192021222324252627282930313233343536373839404142434445464748495051525354555657585960616263646566676869707172737475767778798081828384858687888990919293949596979899
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 __abi_tag
 knn_graph.cpp
 _ZN12_GLOBAL__N_16MatrixD2Ev
 _ZN12_GLOBAL__N_16MatrixD1Ev
 _ZNSt6vectorIN12_GLOBAL__N_16Matrix5EntryESaIS2_EE7reserveEm
 _ZNSt10_HashtableIjSt4pairIKjjESaIS2_ENSt8__detail10_Select1stESt8equal_toIjESt4hashIjENS4_18_Mod_range_hashingENS4_20_Default_ranged_hashENS4_20_Prime_rehash_policyENS4_17_Hashtable_traitsILb0ELb0ELb1EEEE8_M_eraseESt17integral_constantIbLb1EERS1_.isra.0
 _ZSt4endlIcSt11char_traitsIcEERSt13basic_ostreamIT_T0_ES6_.isra.0
```

#### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     0]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     0]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

### Comparing `scib-1.1.3/scib/metrics/__init__.py` & `scib-1.1.4/scib/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `scib-1.1.3/scib/metrics/ari.py` & `scib-1.1.4/scib/metrics/ari.py`

 * *Files identical despite different names*

### Comparing `scib-1.1.3/scib/metrics/cell_cycle.py` & `scib-1.1.4/scib/metrics/cell_cycle.py`

 * *Files identical despite different names*

### Comparing `scib-1.1.3/scib/metrics/clustering.py` & `scib-1.1.4/scib/metrics/clustering.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     :param adata: anndata object
     :param label_key: name of column in adata.obs containing biological labels to be
         optimised against
     :param cluster_key: name of column to be added to adata.obs during clustering.
         Will be overwritten if exists and ``force=True``
     :param cluster_function: a clustering function that takes an anndata.Anndata object. Default: Leiden clustering
     :param metric: function that computes the cost to be optimised over. Must take as
-        arguments ``(adata, group1, group2, **kwargs)`` and returns a number for maximising
+        arguments ``(adata, label_key, cluster_key, **metric_kwargs)`` and returns a number for maximising
         Default is :func:`~scib.metrics.nmi()`
     :param resolutions: list of resolutions to be optimised over. If ``resolutions=None``,
         default resolutions of 10 values ranging between 0.1 and 2 will be used
     :param use_rep: key of embedding to use only if ``adata.uns['neighbors']`` is not
         defined, otherwise will be ignored
     :param force: whether to overwrite the cluster assignments in the ``.obs[cluster_key]``
     :param verbose: whether to print out intermediate results
```

### Comparing `scib-1.1.3/scib/metrics/graph_connectivity.py` & `scib-1.1.4/scib/metrics/graph_connectivity.py`

 * *Files identical despite different names*

### Comparing `scib-1.1.3/scib/metrics/highly_variable_genes.py` & `scib-1.1.4/scib/metrics/highly_variable_genes.py`

 * *Files identical despite different names*

### Comparing `scib-1.1.3/scib/metrics/isolated_labels.py` & `scib-1.1.4/scib/metrics/isolated_labels.py`

 * *Files identical despite different names*

### Comparing `scib-1.1.3/scib/metrics/kbet.py` & `scib-1.1.4/scib/metrics/kbet.py`

 * *Files identical despite different names*

### Comparing `scib-1.1.3/scib/metrics/lisi.py` & `scib-1.1.4/scib/metrics/lisi.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
         scib.me.clisi_graph(adata, label_key="celltype", type="embed", use_rep="X_emb")
 
         # knn output
         scib.me.clisi_graph(adata, label_key="celltype", type="knn")
 
     """
     if batch_key is not None:
-        warnings.warn("'batch_key' is deprecated and will be ignore")
+        warnings.warn("'batch_key' is deprecated and will be ignore", stacklevel=1)
 
     check_adata(adata)
     check_batch(label_key, adata.obs)
 
     adata_tmp = recompute_knn(adata, type_, use_rep)
 
     scores = lisi_graph_py(
@@ -300,15 +300,14 @@
         print(f"Error computing LISI kNN graph {ex}\nSetting value to np.nan")
         return np.nan
 
     if verbose:
         print("LISI score estimation")
 
     if n_cores > 1:
-
         if verbose:
             print(f"{n_cores} processes started.")
         pool = mp.Pool(processes=n_cores)
         chunk_no = np.arange(0, n_cores)
 
         # create argument list for each worker
         results = pool.starmap(
@@ -444,18 +443,21 @@
     # check if the target file is not empty
     if os.stat(index_file).st_size == 0:
         print("File has no entries. Doing nothing.")
         lists = np.zeros(0)
         return lists
 
     # read distances and indices with nan value handling
-    indices = pd.read_table(index_file, index_col=0, header=None, sep=",")
+    header = ["index"] + list(range(1, n_neighbors + 1))
+    indices = pd.read_table(index_file, index_col=0, header=None, sep=",", names=header)
     indices = indices.T
 
-    distances = pd.read_table(distance_file, index_col=0, header=None, sep=",")
+    distances = pd.read_table(
+        distance_file, index_col=0, header=None, sep=",", names=header
+    )
     distances = distances.T
 
     # get cell ids
     chunk_ids = indices.columns.values.astype("int")
 
     # define result vector
     simpson = np.zeros(len(chunk_ids))
```

### Comparing `scib-1.1.3/scib/metrics/metrics.py` & `scib-1.1.4/scib/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `scib-1.1.3/scib/metrics/nmi.py` & `scib-1.1.4/scib/metrics/nmi.py`

 * *Files identical despite different names*

### Comparing `scib-1.1.3/scib/metrics/pcr.py` & `scib-1.1.4/scib/metrics/pcr.py`

 * *Files 3% similar despite different names*

```diff
@@ -190,25 +190,22 @@
             svd_solver = "full"
             # convert to dense bc 'full' is not available for sparse matrices
             if sparse.issparse(matrix):
                 matrix = matrix.todense()
 
         if verbose:
             print("compute PCA")
-        pca = sc.tl.pca(
+        X_pca, _, _, pca_var = sc.tl.pca(
             matrix,
             n_comps=n_comps,
             use_highly_variable=False,
             return_info=True,
             svd_solver=svd_solver,
             copy=True,
         )
-        X_pca = pca[0].copy()
-        pca_var = pca[3].copy()
-        del pca
     else:
         X_pca = matrix
         n_comps = matrix.shape[1]
 
     # PC Regression
     if verbose:
         print("fit regression on PCs")
```

### Comparing `scib-1.1.3/scib/metrics/silhouette.py` & `scib-1.1.4/scib/metrics/silhouette.py`

 * *Files identical despite different names*

### Comparing `scib-1.1.3/scib/metrics/trajectory.py` & `scib-1.1.4/scib/metrics/trajectory.py`

 * *Files identical despite different names*

### Comparing `scib-1.1.3/scib/metrics/utils.py` & `scib-1.1.4/scib/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `scib-1.1.3/scib/preprocessing.py` & `scib-1.1.4/scib/preprocessing.py`

 * *Files identical despite different names*

### Comparing `scib-1.1.3/scib/trajectory_inference.py` & `scib-1.1.4/scib/trajectory_inference.py`

 * *Files identical despite different names*

### Comparing `scib-1.1.3/scib/utils.py` & `scib-1.1.4/scib/utils.py`

 * *Files identical despite different names*

### Comparing `scib-1.1.3/scib.egg-info/PKG-INFO` & `scib-1.1.4/scib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scib
-Version: 1.1.3
+Version: 1.1.4
 Summary: Evaluating single-cell data integration methods
 Home-page: https://github.com/theislab/scib
 Author: Malte D. Luecken, Maren Buettner, Daniel C. Strobl, Michaela F. Mueller
 Author-email: malte.luecken@helmholtz-muenchen.de, michaela.mueller@helmholtz-muenchen.de
 License: MIT
 Project-URL: Pipeline, https://github.com/theislab/scib-pipeline
 Project-URL: Reproducibility, https://theislab.github.io/scib-reproducibility
```

### Comparing `scib-1.1.3/scib.egg-info/SOURCES.txt` & `scib-1.1.4/scib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scib-1.1.3/scib.egg-info/requires.txt` & `scib-1.1.4/scib.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 numpy
-pandas
+pandas<2
 seaborn
 matplotlib
 numba
 scanpy>=1.5
 anndata>=0.7.2
 h5py
 scipy
```

### Comparing `scib-1.1.3/setup.cfg` & `scib-1.1.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.1.3
+current_version = 1.1.4
 commit = True
 tag = True
 
 [bumpversion:file:VERSION.txt]
 search = {current_version}
 replace = {new_version}
 
@@ -42,15 +42,15 @@
 [options]
 packages = 
 	scib
 	scib.metrics
 python_requires = >=3.7
 install_requires = 
 	numpy
-	pandas
+	pandas<2
 	seaborn
 	matplotlib
 	numba
 	scanpy>=1.5
 	anndata>=0.7.2
 	h5py
 	scipy
```

### Comparing `scib-1.1.3/setup.py` & `scib-1.1.4/setup.py`

 * *Files identical despite different names*

