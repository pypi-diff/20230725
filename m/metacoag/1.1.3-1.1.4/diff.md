# Comparing `tmp/metacoag-1.1.3.tar.gz` & `tmp/metacoag-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metacoag-1.1.3.tar", last modified: Tue Jun 13 02:16:41 2023, max compression
+gzip compressed data, was "metacoag-1.1.4.tar", last modified: Mon Jul 24 23:59:38 2023, max compression
```

## Comparing `metacoag-1.1.3.tar` & `metacoag-1.1.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-06-13 02:16:41.702664 metacoag-1.1.3/
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     5232 2022-08-05 12:06:27.000000 metacoag-1.1.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    35149 2022-08-05 12:06:27.000000 metacoag-1.1.3/LICENSE
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      343 2023-02-14 12:08:36.000000 metacoag-1.1.3/MANIFEST.in
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    10606 2023-06-13 02:16:41.702327 metacoag-1.1.3/PKG-INFO
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     9888 2023-06-01 00:40:34.000000 metacoag-1.1.3/README.md
--rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)    39747 2023-06-13 02:06:03.000000 metacoag-1.1.3/metacoag
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-06-13 02:16:41.484630 metacoag-1.1.3/metacoag.egg-info/
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    10606 2023-06-13 02:16:41.000000 metacoag-1.1.3/metacoag.egg-info/PKG-INFO
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      647 2023-06-13 02:16:41.000000 metacoag-1.1.3/metacoag.egg-info/SOURCES.txt
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        1 2023-06-13 02:16:41.000000 metacoag-1.1.3/metacoag.egg-info/dependency_links.txt
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       72 2023-06-13 02:16:41.000000 metacoag-1.1.3/metacoag.egg-info/entry_points.txt
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       69 2023-06-13 02:16:41.000000 metacoag-1.1.3/metacoag.egg-info/requires.txt
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       15 2023-06-13 02:16:41.000000 metacoag-1.1.3/metacoag.egg-info/top_level.txt
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        1 2022-11-25 05:01:14.000000 metacoag-1.1.3/metacoag.egg-info/zip-safe
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-06-13 02:16:41.494534 metacoag-1.1.3/metacoag_utils/
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     6148 2023-06-01 01:29:39.000000 metacoag-1.1.3/metacoag_utils/.DS_Store
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        0 2022-08-05 12:06:27.000000 metacoag-1.1.3/metacoag_utils/__init__.py
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-06-13 02:16:41.496845 metacoag-1.1.3/metacoag_utils/auxiliary/
--rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20) 15929643 2022-08-05 12:06:27.000000 metacoag-1.1.3/metacoag_utils/auxiliary/marker.hmm
--rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)     1099 2022-08-05 12:06:27.000000 metacoag-1.1.3/metacoag_utils/bidirectionalmap.py
--rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)     6522 2023-06-13 02:06:03.000000 metacoag-1.1.3/metacoag_utils/feature_utils.py
--rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)    12073 2023-05-15 05:51:35.000000 metacoag-1.1.3/metacoag_utils/graph_utils.py
--rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)    15011 2023-06-13 02:06:03.000000 metacoag-1.1.3/metacoag_utils/label_prop_utils.py
--rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)     8738 2023-06-13 02:06:03.000000 metacoag-1.1.3/metacoag_utils/marker_gene_utils.py
--rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)    15606 2023-06-13 02:06:03.000000 metacoag-1.1.3/metacoag_utils/matching_utils.py
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-06-13 02:16:41.701402 metacoag-1.1.3/metacoag_utils/support/
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     6148 2023-06-01 01:29:39.000000 metacoag-1.1.3/metacoag_utils/support/.DS_Store
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1745 2023-06-13 02:12:10.000000 metacoag-1.1.3/metacoag_utils/support/combine_cov.py
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       38 2023-06-13 02:16:41.702757 metacoag-1.1.3/setup.cfg
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1581 2023-06-13 02:12:05.000000 metacoag-1.1.3/setup.py
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-07-24 23:59:38.311308 metacoag-1.1.4/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     5232 2022-08-05 12:06:27.000000 metacoag-1.1.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    35149 2022-08-05 12:06:27.000000 metacoag-1.1.4/LICENSE
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      343 2023-02-14 12:08:36.000000 metacoag-1.1.4/MANIFEST.in
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    10606 2023-07-24 23:59:38.311012 metacoag-1.1.4/PKG-INFO
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     9888 2023-06-01 00:40:34.000000 metacoag-1.1.4/README.md
+-rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)    39668 2023-07-24 06:31:05.000000 metacoag-1.1.4/metacoag
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-07-24 23:59:38.149155 metacoag-1.1.4/metacoag.egg-info/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    10606 2023-07-24 23:59:38.000000 metacoag-1.1.4/metacoag.egg-info/PKG-INFO
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      647 2023-07-24 23:59:38.000000 metacoag-1.1.4/metacoag.egg-info/SOURCES.txt
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        1 2023-07-24 23:59:38.000000 metacoag-1.1.4/metacoag.egg-info/dependency_links.txt
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       72 2023-07-24 23:59:38.000000 metacoag-1.1.4/metacoag.egg-info/entry_points.txt
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       62 2023-07-24 23:59:38.000000 metacoag-1.1.4/metacoag.egg-info/requires.txt
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       15 2023-07-24 23:59:38.000000 metacoag-1.1.4/metacoag.egg-info/top_level.txt
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        1 2022-11-25 05:01:14.000000 metacoag-1.1.4/metacoag.egg-info/zip-safe
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-07-24 23:59:38.153861 metacoag-1.1.4/metacoag_utils/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     6148 2023-06-01 01:29:39.000000 metacoag-1.1.4/metacoag_utils/.DS_Store
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        0 2022-08-05 12:06:27.000000 metacoag-1.1.4/metacoag_utils/__init__.py
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-07-24 23:59:38.154501 metacoag-1.1.4/metacoag_utils/auxiliary/
+-rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20) 15929643 2022-08-05 12:06:27.000000 metacoag-1.1.4/metacoag_utils/auxiliary/marker.hmm
+-rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)     1099 2022-08-05 12:06:27.000000 metacoag-1.1.4/metacoag_utils/bidirectionalmap.py
+-rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)     6522 2023-07-24 06:31:05.000000 metacoag-1.1.4/metacoag_utils/feature_utils.py
+-rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)    12073 2023-05-15 05:51:35.000000 metacoag-1.1.4/metacoag_utils/graph_utils.py
+-rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)    15011 2023-07-24 06:31:05.000000 metacoag-1.1.4/metacoag_utils/label_prop_utils.py
+-rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)     8923 2023-07-24 06:31:05.000000 metacoag-1.1.4/metacoag_utils/marker_gene_utils.py
+-rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)    15606 2023-07-24 06:31:05.000000 metacoag-1.1.4/metacoag_utils/matching_utils.py
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-07-24 23:59:38.309336 metacoag-1.1.4/metacoag_utils/support/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     6148 2023-06-01 01:29:39.000000 metacoag-1.1.4/metacoag_utils/support/.DS_Store
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1745 2023-06-13 02:12:10.000000 metacoag-1.1.4/metacoag_utils/support/combine_cov.py
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       38 2023-07-24 23:59:38.311398 metacoag-1.1.4/setup.cfg
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1574 2023-07-24 06:32:51.000000 metacoag-1.1.4/setup.py
```

### Comparing `metacoag-1.1.3/CODE_OF_CONDUCT.md` & `metacoag-1.1.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `metacoag-1.1.3/LICENSE` & `metacoag-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `metacoag-1.1.3/PKG-INFO` & `metacoag-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metacoag
-Version: 1.1.3
+Version: 1.1.4
 Summary: MetaCoAG: Binning Metagenomic Contigs via Composition, Coverage and Assembly Graphs
 Home-page: https://github.com/metagentools/MetaCoAG
 Author: Vijini Mallawaarachchi and Yu Lin
 Author-email: viji.mallawaarachchi@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `metacoag-1.1.3/README.md` & `metacoag-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `metacoag-1.1.3/metacoag` & `metacoag-1.1.4/metacoag`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from metacoag_utils import (feature_utils, graph_utils, label_prop_utils,
                             marker_gene_utils, matching_utils)
 from metacoag_utils.bidirectionalmap import BidirectionalMap
 
 __author__ = "Vijini Mallawaarachchi and Yu Lin"
 __copyright__ = "Copyright 2020, MetaCoAG Project"
 __license__ = "GPL-3.0"
-__version__ = "1.1.3"
+__version__ = "1.1.4"
 __maintainer__ = "Vijini Mallawaarachchi"
 __email__ = "vijini.mallawaarachchi@anu.edu.au"
 __status__ = "Stable Release"
 
 
 # Set global paramters
 # ---------------------------------------------------
@@ -75,17 +75,17 @@
     help="path to the output folder",
     type=click.Path(dir_okay=True, writable=True, readable=True),
     required=True,
 )
 @click.option(
     "--hmm",
     help="path to marker.hmm file.",
-    default=os.path.join(pathlib.Path(__file__).parents[0], "metacoag_utils", "auxiliary", "marker.hmm"),
+    default="auxiliary/marker.hmm",
     show_default=True,
-    type=click.Path(),
+    type=str,
     required=False,
 )
 @click.option(
     "--prefix",
     help="prefix for the output file",
     type=str,
     default="",
@@ -233,15 +233,15 @@
         if not prefix.endswith("_"):
             prefix = f"{prefix}_"
 
 
     # Setup logger
     # ------------------------------------------------------------------------
 
-    logger = logging.getLogger("MetaCoaAG 1.1.3")
+    logger = logging.getLogger("MetaCoaAG 1.1.4")
     logger.setLevel(logging.DEBUG)
     logging.captureWarnings(True)
     formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(message)s")
     consoleHeader = logging.StreamHandler()
     consoleHeader.setFormatter(formatter)
     consoleHeader.setLevel(logging.INFO)
     logger.addHandler(consoleHeader)
```

### Comparing `metacoag-1.1.3/metacoag.egg-info/PKG-INFO` & `metacoag-1.1.4/metacoag.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metacoag
-Version: 1.1.3
+Version: 1.1.4
 Summary: MetaCoAG: Binning Metagenomic Contigs via Composition, Coverage and Assembly Graphs
 Home-page: https://github.com/metagentools/MetaCoAG
 Author: Vijini Mallawaarachchi and Yu Lin
 Author-email: viji.mallawaarachchi@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `metacoag-1.1.3/metacoag.egg-info/SOURCES.txt` & `metacoag-1.1.4/metacoag.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metacoag-1.1.3/metacoag_utils/.DS_Store` & `metacoag-1.1.4/metacoag_utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `metacoag-1.1.3/metacoag_utils/auxiliary/marker.hmm` & `metacoag-1.1.4/metacoag_utils/auxiliary/marker.hmm`

 * *Files identical despite different names*

### Comparing `metacoag-1.1.3/metacoag_utils/bidirectionalmap.py` & `metacoag-1.1.4/metacoag_utils/bidirectionalmap.py`

 * *Files identical despite different names*

### Comparing `metacoag-1.1.3/metacoag_utils/feature_utils.py` & `metacoag-1.1.4/metacoag_utils/feature_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import sys
 from multiprocessing import Pool
 
 import numpy as np
 from Bio import SeqIO
 
 # Create logger
-logger = logging.getLogger("MetaCoaAG 1.1.3")
+logger = logging.getLogger("MetaCoaAG 1.1.4")
 
 # Set complements of each nucleotide
 complements = {"A": "T", "C": "G", "G": "C", "T": "A"}
 
 # Set bits for each nucleotide
 nt_bits = {"A": 0, "C": 1, "G": 2, "T": 3}
```

### Comparing `metacoag-1.1.3/metacoag_utils/graph_utils.py` & `metacoag-1.1.4/metacoag_utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `metacoag-1.1.3/metacoag_utils/label_prop_utils.py` & `metacoag-1.1.4/metacoag_utils/label_prop_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import sys
 
 from metacoag_utils import matching_utils
 
 MAX_WEIGHT = sys.float_info.max
 
 # create logger
-logger = logging.getLogger("MetaCoaAG 1.1.3")
+logger = logging.getLogger("MetaCoaAG 1.1.4")
 
 
 class DataWrap:
     def __init__(self, data):
         self.data = data
 
     def __lt__(self, other):
```

### Comparing `metacoag-1.1.3/metacoag_utils/marker_gene_utils.py` & `metacoag-1.1.4/metacoag_utils/marker_gene_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 #!/usr/bin/env python3
 
 import logging
 import os
 import pathlib
 
 # create logger
-logger = logging.getLogger("MetaCoaAG 1.1.3")
+logger = logging.getLogger("MetaCoaAG 1.1.4")
 
 
 # Modified from SolidBin
 def scan_for_marker_genes(contigs_file, nthreads, markerURL, no_cut_tc, hard=0):
 
     fragScanURL = "run_FragGeneScan.pl"
     hmmExeURL = "hmmsearch"
 
+    if markerURL == "auxiliary/marker.hmm":
+        software_path = pathlib.Path(__file__).parent.absolute()
+        markerURL = os.path.join(software_path, "auxiliary", "marker.hmm")
+
     logger.info("Using marker file: " + markerURL)
 
     fragResultURL = f"{contigs_file}.frag.faa"
     hmmResultURL = f"{contigs_file}.hmmout"
     if not (os.path.exists(fragResultURL)):
         fragCmd = (
             fragScanURL
```

### Comparing `metacoag-1.1.3/metacoag_utils/matching_utils.py` & `metacoag-1.1.4/metacoag_utils/matching_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Constants set from MaxBin 2.0
 MU_INTRA, SIGMA_INTRA = 0, 0.01037897 / 2
 MU_INTER, SIGMA_INTER = 0.0676654, 0.03419337
 VERY_SMALL_DOUBLE = 1e-10
 MAX_WEIGHT = sys.float_info.max
 
 # create logger
-logger = logging.getLogger("MetaCoaAG 1.1.3")
+logger = logging.getLogger("MetaCoaAG 1.1.4")
 
 
 def normpdf(x, mean, sd):
     var = float(sd) ** 2
     denom = sd * (2 * math.pi) ** 0.5
     num = math.exp(-((float(x) - float(mean)) ** 2) / (2 * var))
     return num / denom
```

### Comparing `metacoag-1.1.3/metacoag_utils/support/.DS_Store` & `metacoag-1.1.4/metacoag_utils/support/.DS_Store`

 * *Files identical despite different names*

### Comparing `metacoag-1.1.3/metacoag_utils/support/combine_cov.py` & `metacoag-1.1.4/metacoag_utils/support/combine_cov.py`

 * *Files identical despite different names*

### Comparing `metacoag-1.1.3/setup.py` & `metacoag-1.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 packages = setuptools.find_packages()
 package_data = {"metacoag_utils": ["metacoag_utils/*", "metacoag_utils/auxiliary/*"]}
 
 data_files = [(".", ["LICENSE", "README.md"])]
 
 setuptools.setup(
     name="metacoag",
-    version="1.1.3",
+    version="1.1.4",
     zip_safe=True,
     author="Vijini Mallawaarachchi and Yu Lin",
     author_email="viji.mallawaarachchi@gmail.com",
     description="MetaCoAG: Binning Metagenomic Contigs via Composition, Coverage and Assembly Graphs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/metagentools/MetaCoAG",
@@ -37,15 +37,15 @@
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Natural Language :: English",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "biopython",
-        "python-igraph",
+        "igraph",
         "networkx",
         "scipy",
         "numpy",
         "tqdm",
         "pandas",
         "hmmer",
         "click",
```

