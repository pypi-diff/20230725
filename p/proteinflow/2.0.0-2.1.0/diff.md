# Comparing `tmp/proteinflow-2.0.0.tar.gz` & `tmp/proteinflow-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinflow-2.0.0.tar", last modified: Wed Jul 19 13:48:36 2023, max compression
+gzip compressed data, was "proteinflow-2.1.0.tar", last modified: Tue Jul 25 10:33:06 2023, max compression
```

## Comparing `proteinflow-2.0.0.tar` & `proteinflow-2.1.0.tar`

### file list

```diff
@@ -1,40 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:48:36.956620 proteinflow-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-19 13:48:25.000000 proteinflow-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-07-19 13:48:36.956620 proteinflow-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-07-19 13:48:25.000000 proteinflow-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:48:36.952620 proteinflow-2.0.0/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-19 13:48:25.000000 proteinflow-2.0.0/dev/bump_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:48:36.956620 proteinflow-2.0.0/proteinflow/
--rw-r--r--   0 runner    (1001) docker     (123)    25443 2023-07-19 13:48:25.000000 proteinflow-2.0.0/proteinflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-19 13:48:25.000000 proteinflow-2.0.0/proteinflow/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-07-19 13:48:25.000000 proteinflow-2.0.0/proteinflow/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:48:36.956620 proteinflow-2.0.0/proteinflow/data/
--rw-r--r--   0 runner    (1001) docker     (123)    55531 2023-07-19 13:48:25.000000 proteinflow-2.0.0/proteinflow/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39434 2023-07-19 13:48:25.000000 proteinflow-2.0.0/proteinflow/data/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    16881 2023-07-19 13:48:25.000000 proteinflow-2.0.0/proteinflow/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:48:36.956620 proteinflow-2.0.0/proteinflow/download/
--rw-r--r--   0 runner    (1001) docker     (123)    20048 2023-07-19 13:48:25.000000 proteinflow-2.0.0/proteinflow/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-07-19 13:48:25.000000 proteinflow-2.0.0/proteinflow/download/boto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:48:36.956620 proteinflow-2.0.0/proteinflow/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-19 13:48:25.000000 proteinflow-2.0.0/proteinflow/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:48:36.956620 proteinflow-2.0.0/proteinflow/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-19 13:48:25.000000 proteinflow-2.0.0/proteinflow/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:48:36.956620 proteinflow-2.0.0/proteinflow/processing/
--rw-r--r--   0 runner    (1001) docker     (123)    16875 2023-07-19 13:48:25.000000 proteinflow-2.0.0/proteinflow/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:48:36.956620 proteinflow-2.0.0/proteinflow/split/
--rw-r--r--   0 runner    (1001) docker     (123)    45990 2023-07-19 13:48:25.000000 proteinflow-2.0.0/proteinflow/split/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-07-19 13:48:25.000000 proteinflow-2.0.0/proteinflow/split/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:48:36.956620 proteinflow-2.0.0/proteinflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-07-19 13:48:36.000000 proteinflow-2.0.0/proteinflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-19 13:48:36.000000 proteinflow-2.0.0/proteinflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 13:48:36.000000 proteinflow-2.0.0/proteinflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-19 13:48:36.000000 proteinflow-2.0.0/proteinflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-19 13:48:36.000000 proteinflow-2.0.0/proteinflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-19 13:48:36.000000 proteinflow-2.0.0/proteinflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-19 13:48:25.000000 proteinflow-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-19 13:48:36.956620 proteinflow-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:48:36.956620 proteinflow-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-19 13:48:25.000000 proteinflow-2.0.0/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-19 13:48:25.000000 proteinflow-2.0.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-19 13:48:25.000000 proteinflow-2.0.0/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-19 13:48:25.000000 proteinflow-2.0.0/tests/test_sabdab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:33:06.377544 proteinflow-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-25 10:32:48.000000 proteinflow-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-07-25 10:33:06.377544 proteinflow-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-07-25 10:32:48.000000 proteinflow-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:33:06.369544 proteinflow-2.1.0/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-25 10:32:48.000000 proteinflow-2.1.0/dev/bump_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-25 10:32:48.000000 proteinflow-2.1.0/dev/update_init_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:33:06.373544 proteinflow-2.1.0/proteinflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    28053 2023-07-25 10:32:48.000000 proteinflow-2.1.0/proteinflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-07-25 10:32:48.000000 proteinflow-2.1.0/proteinflow/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6355 2023-07-25 10:32:48.000000 proteinflow-2.1.0/proteinflow/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:33:06.373544 proteinflow-2.1.0/proteinflow/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    71926 2023-07-25 10:32:48.000000 proteinflow-2.1.0/proteinflow/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37617 2023-07-25 10:32:48.000000 proteinflow-2.1.0/proteinflow/data/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18133 2023-07-25 10:32:48.000000 proteinflow-2.1.0/proteinflow/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:33:06.373544 proteinflow-2.1.0/proteinflow/download/
+-rw-r--r--   0 runner    (1001) docker     (123)    24607 2023-07-25 10:32:48.000000 proteinflow-2.1.0/proteinflow/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-07-25 10:32:48.000000 proteinflow-2.1.0/proteinflow/download/boto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36587 2023-07-25 10:32:48.000000 proteinflow-2.1.0/proteinflow/ligand.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:33:06.373544 proteinflow-2.1.0/proteinflow/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-25 10:32:48.000000 proteinflow-2.1.0/proteinflow/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:33:06.373544 proteinflow-2.1.0/proteinflow/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-25 10:32:48.000000 proteinflow-2.1.0/proteinflow/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:33:06.373544 proteinflow-2.1.0/proteinflow/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)    18971 2023-07-25 10:32:48.000000 proteinflow-2.1.0/proteinflow/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:33:06.377544 proteinflow-2.1.0/proteinflow/split/
+-rw-r--r--   0 runner    (1001) docker     (123)    50801 2023-07-25 10:32:48.000000 proteinflow-2.1.0/proteinflow/split/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-07-25 10:32:48.000000 proteinflow-2.1.0/proteinflow/split/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-07-25 10:32:48.000000 proteinflow-2.1.0/proteinflow/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:33:06.373544 proteinflow-2.1.0/proteinflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-07-25 10:33:06.000000 proteinflow-2.1.0/proteinflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-25 10:33:06.000000 proteinflow-2.1.0/proteinflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 10:33:06.000000 proteinflow-2.1.0/proteinflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-25 10:33:06.000000 proteinflow-2.1.0/proteinflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-25 10:33:06.000000 proteinflow-2.1.0/proteinflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-25 10:33:06.000000 proteinflow-2.1.0/proteinflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-25 10:32:48.000000 proteinflow-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-25 10:33:06.377544 proteinflow-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:33:06.377544 proteinflow-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-25 10:32:48.000000 proteinflow-2.1.0/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-25 10:32:48.000000 proteinflow-2.1.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-25 10:32:48.000000 proteinflow-2.1.0/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-25 10:32:48.000000 proteinflow-2.1.0/tests/test_sabdab.py
```

### Comparing `proteinflow-2.0.0/LICENSE` & `proteinflow-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinflow-2.0.0/PKG-INFO` & `proteinflow-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteinflow
-Version: 2.0.0
+Version: 2.1.0
 Summary: Versatile pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
 License: BSD-3-Clause
 Keywords: bioinformatics,dataset,protein,PDB,deep learning
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proteinflow Version: 2.0.0 Summary: Versatile
+Metadata-Version: 2.1 Name: proteinflow Version: 2.1.0 Summary: Versatile
 pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova
 adaptyvbio.com>, Arthur Valentin
 adaptyvbio.com> License: BSD-3-Clause Keywords:
 bioinformatics,dataset,protein,PDB,deep learning Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
   ProteinFlow - A data processing pipeline for all your protein design needs
```

### Comparing `proteinflow-2.0.0/README.md` & `proteinflow-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `proteinflow-2.0.0/dev/bump_version.py` & `proteinflow-2.1.0/dev/bump_version.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.0.0/proteinflow/__init__.py` & `proteinflow-2.1.0/proteinflow/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -152,50 +152,55 @@
 ...
 ```
 See more details on available parameters and the data format in the [docs](https://adaptyvbio.github.io/ProteinFlow/) + [this repository](https://github.com/adaptyvbio/ProteinFlow-models) for a use case.
 
 ## ProteinFlow Stable Releases
 You can download them with `proteinflow download --tag {tag}` in the command line or browse in the [interface](https://proteinflow-datasets.s3.eu-west-1.amazonaws.com/index.html).
 
-|Tag    |Date    |Snapshot|Size|Min res|Min len|Max len|MMseqs thr|Split (train/val/test)|Missing thr (ends/middle)|Source|Remove redundancies|Note|
-|-------|--------|--------|----|-------|-------|-------|----------|----------------------|-------------------------|---|---|----|
-|paper|10.11.22|20220103|24G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|yes|first release, no mmCIF files|
-|20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|yes|v1.1.1|
-|20230623_sabdab|26.06.23|live 26.06.23|1.4G|3.5|30|10'000|0.3|96/3/1|0.5/0.2|SAbDab|no|v1.4.1 (requires >= v1.4.0)|
+|Tag    |Date    |Snapshot|Size|Min res|Min len|Max len|Max chains|MMseqs thr|Split (train/val/test)|Missing thr (ends/middle)|Source|Remove redundancies|Note|
+|-------|--------|--------|----|-------|-------|-------|----------|----------|----------------------|-------------------------|---|---|----------------|
+|paper|10.11.22|20220103|24G|3.5|30|10'000|-|0.3|90/5/5|0.3/0.1|PDB|yes|first release, no mmCIF files|
+|20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|-|0.3|90/5/5|0.3/0.1|PDB|yes|v1.1.1|
+|20230623_sabdab|26.06.23|live 26.06.23|1.4G|3.5|30|10'000|-|0.3|96/3/1|0.5/0.2|SAbDab|no|v1.4.1 (requires >= v1.4.0)|
+|20230102_v200|19.07.23|20230102|33G|3.5|30|10'000|10|0.3|90/5/5|0.3/0.1|PDB|no|v2.0.0|
 
 """
 __pdoc__ = {
     "data.utils": False,
     "download.boto": False,
     "constants": False,
     "split": False,
     "cli": False,
+    "processing.ligand": False,
 }
 __docformat__ = "numpy"
 
 import os
 import pickle
 import random
 import shutil
+import socket
 import string
 import tempfile
 import warnings
 
 import boto3
 import numpy as np
 from botocore import UNSIGNED
 from botocore.config import Config
+from tqdm import tqdm
 
 from proteinflow.constants import SIDECHAIN_ORDER
 from proteinflow.data.torch import ProteinDataset, ProteinLoader
-from proteinflow.download import _download_dataset
+from proteinflow.download import _download_dataset, _get_chain_pdb_ids
 from proteinflow.download.boto import _s3list
 from proteinflow.processing import run_processing
 from proteinflow.split import (
     _check_mmseqs,
+    _exclude_files_with_no_ligand,
     _get_excluded_files,
     _get_split_dictionaries,
     _split_data,
 )
 
 
 def download_data(tag, local_datasets_folder="./data", skip_splitting=False):
@@ -213,15 +218,16 @@
     """
     sabdab_data_path = _download_dataset(tag, local_datasets_folder)
     if not skip_splitting:
         _split_data(sabdab_data_path)
 
 
 def generate_data(
-    tag,
+    tag=None,
+    pdb_id_list_path=None,
     local_datasets_folder="./data",
     min_length=30,
     max_length=10000,
     resolution_thr=3.5,
     missing_ends_thr=0.3,
     missing_middle_thr=0.1,
     not_filter_methods=False,
@@ -239,14 +245,17 @@
     sabdab=False,
     sabdab_data_path=None,
     require_antigen=False,
     exclude_chains=None,
     exclude_threshold=0.7,
     exclude_clusters=False,
     exclude_based_on_cdr=None,
+    load_ligands=False,
+    exclude_chains_without_ligands=False,
+    tanimoto_clustering=False,
     random_seed=42,
     max_chains=10,
 ):
     """Download and parse PDB files that meet filtering criteria.
 
     The output files are pickled nested dictionaries where first-level keys are chain Ids and second-level keys are
     the following:
@@ -265,16 +274,19 @@
 
     All errors including reasons for filtering a file out are logged in the log file.
 
     For more information on the splitting procedure and options, check out the `proteinflow.split_data` documentation.
 
     Parameters
     ----------
-    tag : str
+    tag : str, optional
         the name of the dataset to load
+    pdb_id_list_path : str, optional
+        if provided, get pdb_ids from text file where each line contains one chain id (format pdb_id-num example: 1XYZ-1)
+        pdb_ids can also be passed, an automatic retrieval of chain id s will be performed in that case
     local_datasets_folder : str, default "./data"
         the path to the folder that will store proteinflow datasets, logs and temporary files
     min_length : int, default 30
         The minimum number of non-missing residues per chain
     max_length : int, default 10000
         The maximum number of residues per chain (set None for no threshold)
     resolution_thr : float, default 3.5
@@ -317,32 +329,54 @@
         a list of chains (`{pdb_id}-{chain_id}`) to exclude from the splitting (e.g. `["1A2B-A", "1A2B-B"]`); chain id is the author chain id
     exclude_threshold : float in [0, 1], default 0.7
         the sequence similarity threshold for excluding chains
     exclude_clusters : bool, default False
         if `True`, exclude clusters that contain chains similar to chains in the `exclude_chains` list
     exclude_based_on_cdr : {"H1", "H2", "H3", "L1", "L2", "L3"}, optional
         if given and `exclude_clusters` is `True` + the dataset is SAbDab, exclude files based on only the given CDR clusters
+    load_ligands : bool, default False
+        if `True`, load ligands from the PDB files
+    exclude_chains_without_ligands : bool, default False
+        if `True`, exclude biounits that don't contain ligands
+    tanimoto_clustering : bool, default False
+        if `True`, cluster the biounits based on ligand Tanimoto similarity
     random_seed : int, default 42
         the random seed to use for splitting
     max_chains : int, default 10
         the maximum number of chains per biounit
 
     Returns
     -------
     log : dict
         a dictionary where keys are recognized error names and values are lists of PDB ids that caused the errors
 
     """
-    filter_methods = not not_filter_methods
-    remove_redundancies = not not_remove_redundancies
     tmp_id = "".join(
         random.choice(string.ascii_uppercase + string.digits) for _ in range(5)
     )
-    tmp_folder = os.path.join(tempfile.gettempdir(), tag + tmp_id)
-    os.makedirs(tmp_folder)
+    if tag is None:
+        if pdb_id_list_path is None:
+            raise RuntimeError(
+                "Please input a data source: valid tag or a pdb ids list"
+            )
+        else:
+            tag = pdb_id_list_path.split("/")[-1].split(".")[0]
+            tmp_folder = os.path.join(tempfile.gettempdir(), tag + tmp_id)
+            os.makedirs(tmp_folder)
+            with open(pdb_id_list_path) as file:
+                # Read lines from the file
+                example_pdb_id = file.readline()
+            if "-" not in example_pdb_id:
+                pdb_id_list_path = _get_chain_pdb_ids(pdb_id_list_path, tmp_folder)
+    else:
+        tmp_folder = os.path.join(tempfile.gettempdir(), tag + tmp_id)
+        os.makedirs(tmp_folder)
+    filter_methods = not not_filter_methods
+    remove_redundancies = not not_remove_redundancies
+
     output_folder = os.path.join(local_datasets_folder, f"proteinflow_{tag}")
 
     if force and os.path.exists(output_folder):
         shutil.rmtree(output_folder)
 
     log_dict = run_processing(
         tmp_folder=tmp_folder,
@@ -360,29 +394,39 @@
         tag=tag,
         pdb_snapshot=pdb_snapshot,
         load_live=load_live,
         sabdab=sabdab,
         sabdab_data_path=sabdab_data_path,
         require_antigen=require_antigen,
         max_chains=max_chains,
+        pdb_id_list_path=pdb_id_list_path,
+        load_ligands=load_ligands,
     )
+
     if not skip_splitting:
+        if tanimoto_clustering and not load_ligands:
+            print(
+                "Can not use Tanimoto Clustering without load_ligands=False. Setting tanimoto_clustering to False"
+            )
+            tanimoto_clustering = False
         split_data(
             tag=tag,
             local_datasets_folder=local_datasets_folder,
             split_tolerance=split_tolerance,
             test_split=test_split,
             valid_split=valid_split,
             ignore_existing=True,
             min_seq_id=min_seq_id,
             exclude_chains=exclude_chains,
             exclude_threshold=exclude_threshold,
             exclude_clusters=exclude_clusters,
             exclude_based_on_cdr=exclude_based_on_cdr,
             random_seed=random_seed,
+            exclude_chains_without_ligands=exclude_chains_without_ligands,
+            tanimoto_clustering=tanimoto_clustering,
         )
     shutil.rmtree(tmp_folder)
     return log_dict
 
 
 def split_data(
     tag,
@@ -393,14 +437,16 @@
     ignore_existing=False,
     min_seq_id=0.3,
     exclude_chains=None,
     exclude_threshold=0.7,
     exclude_clusters=False,
     exclude_based_on_cdr=None,
     random_seed=42,
+    exclude_chains_without_ligands=False,
+    tanimoto_clustering=False,
 ):
     """Split `proteinflow` entry files into training, test and validation.
 
     Our splitting algorithm has two objectives: achieving minimal data leakage and balancing the proportion of
     single chain, homomer and heteromer entries.
 
     It follows these steps:
@@ -441,14 +487,18 @@
         the sequence similarity threshold for excluding chains
     exclude_clusters : bool, default False
         if `True`, exclude clusters that contain chains similar to chains in the `exclude_chains` list
     exclude_based_on_cdr : {"H1", "H2", "H3", "L1", "L2", "L3"}, optional
         if given and `exclude_clusters` is `True` + the dataset is SAbDab, exclude files based on only the given CDR clusters
     random_seed : int, default 42
         random seed for reproducibility (set to `None` to use a random seed)
+    exclude_chains_without_ligands : bool, default False
+        if `True`, exclude biounits that don't contain ligands
+    tanimoto_clustering: bool, default False
+        cluster chains based on the tanimoto similarity of their ligands
 
     Returns
     -------
     log : dict
         a dictionary where keys are recognized error names and values are lists of PDB ids that caused the errors
 
     """
@@ -461,14 +511,19 @@
         excluded_biounits = _get_excluded_files(
             tag,
             local_datasets_folder,
             temp_folder,
             exclude_chains,
             exclude_threshold,
         )
+    if exclude_chains_without_ligands:
+        excluded_biounits += _exclude_files_with_no_ligand(
+            tag,
+            local_datasets_folder,
+        )
 
     output_folder = os.path.join(local_datasets_folder, f"proteinflow_{tag}")
     out_split_dict_folder = os.path.join(output_folder, "splits_dict")
     exists = False
 
     if os.path.exists(out_split_dict_folder):
         if not ignore_existing:
@@ -484,14 +539,15 @@
             tmp_folder=temp_folder,
             output_folder=output_folder,
             split_tolerance=split_tolerance,
             test_split=test_split,
             valid_split=valid_split,
             out_split_dict_folder=out_split_dict_folder,
             min_seq_id=min_seq_id,
+            tanimoto_clustering=tanimoto_clustering,
         )
     shutil.rmtree(temp_folder)
 
     _split_data(
         output_folder, excluded_biounits, exclude_clusters, exclude_based_on_cdr
     )
```

### Comparing `proteinflow-2.0.0/proteinflow/cli.py` & `proteinflow-2.1.0/proteinflow/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,14 +57,18 @@
 
 
 @click.option(
     "--tag",
     help="The name of the dataset",
 )
 @click.option(
+    "--pdb_id_list_path",
+    help="List of pdb ids to download and process",
+)
+@click.option(
     "--local_datasets_folder",
     default="./data",
     help="The folder where proteinflow datasets, temporary files and logs will be stored",
 )
 @click.option(
     "--min_length",
     default=30,
@@ -117,15 +121,15 @@
 @click.option(
     "--split_tolerance",
     default=0.2,
     type=float,
     help="The tolerance on the split ratio (default 20%)",
 )
 @click.option(
-    "-n",
+    "--n",
     default=None,
     type=int,
     help="The number of files to process (for debugging purposes)",
 )
 @click.option(
     "--force", is_flag=True, help="When `True`, rewrite the files if they already exist"
 )
@@ -134,14 +138,19 @@
     type=str,
     help="The pdb snapshot folder to load",
 )
 @click.option(
     "--skip_splitting", is_flag=True, help="Use this flag to skip splitting the data"
 )
 @click.option(
+    "--skip_processing",
+    is_flag=True,
+    help="Use this flag to skip downloading and processing the data",
+)
+@click.option(
     "--load_live",
     is_flag=True,
     help="Load the files that are not in the latest PDB snapshot from the PDB FTP server (disregarded if pdb_snapshot is not none)",
 )
 @click.option(
     "--min_seq_id",
     default=0.3,
@@ -160,14 +169,29 @@
 )
 @click.option(
     "--require_antigen",
     is_flag=True,
     help="Use this flag to require that the SAbDab files contain an antigen",
 )
 @click.option(
+    "--load_ligands",
+    is_flag=True,
+    help="Whether or not to load ligands found in the pdbs example: data['A']['ligand'][0]['X']",
+)
+@click.option(
+    "--exclude_chains_without_ligands",
+    is_flag=True,
+    help="Exclude chains without ligands from the generated dataset",
+)
+@click.option(
+    "--tanimoto_clustering",
+    is_flag=True,
+    help="Whether to use Tanimoto Clustering instead of MMSeqs2. Only works if load_ligands is set to True",
+)
+@click.option(
     "--random_seed",
     default=42,
     type=int,
     help="The random seed to use for splitting",
 )
 @click.option(
     "--max_chains",
@@ -239,14 +263,24 @@
 )
 @click.option(
     "--exclude_based_on_cdr",
     type=click.Choice(["L1", "L2", "L3", "H1", "H2", "H3"]),
     help="if given and exclude_clusters is true + the dataset is SAbDab, exclude files based on only the given CDR clusters",
 )
 @click.option(
+    "--exclude_chains_without_ligands",
+    is_flag=True,
+    help="Exclude chains without ligands from the generated dataset",
+)
+@click.option(
+    "--tanimoto_clustering",
+    is_flag=True,
+    help="Whether to use Tanimoto Clustering instead of MMSeqs2. Only works if the dataset contains ligands",
+)
+@click.option(
     "--random_seed",
     default=42,
     type=int,
     help="The random seed to use for splitting",
 )
 @cli.command(
     "split",
```

### Comparing `proteinflow-2.0.0/proteinflow/constants.py` & `proteinflow-2.1.0/proteinflow/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,23 +219,28 @@
     "V": "VAL",
     "I": "ILE",
     "L": "LEU",
     "M": "MET",
     "F": "PHE",
     "Y": "TYR",
     "W": "TRP",
+    "-": "GLY",
 }
 ATOM_MAP_4 = {a: ["N", "C", "CA", "O"] for a in ONE_TO_THREE_LETTER_MAP.keys()}
 ATOM_MAP_1 = {a: ["CA"] for a in ONE_TO_THREE_LETTER_MAP.keys()}
 ATOM_MAP_3 = {a: ["N", "C", "CA"] for a in ONE_TO_THREE_LETTER_MAP.keys()}
 ATOM_MAP_14 = {D3TO1[k]: BACKBONE_ORDER + v for k, v in SIDECHAIN_ORDER.items()}
 
 
 def _PMAP(x):
+    """Get chemical properties of amino acid."""
     return [
         FEATURES_DICT["hydropathy"][x] / 5,
         FEATURES_DICT["volume"][x] / 200,
         FEATURES_DICT["charge"][x],
         FEATURES_DICT["polarity"][x],
         FEATURES_DICT["acceptor"][x],
         FEATURES_DICT["donor"][x],
     ]
+
+
+COLORS = ["#62B9DC", "#EAB1C5", "#0C9094", "#8090E6", "#96E396", "#FCAC97", "#740E66"]
```

### Comparing `proteinflow-2.0.0/proteinflow/data/__init__.py` & `proteinflow-2.1.0/proteinflow/data/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,46 +8,51 @@
 A `ProteinEntry` object can be created from a proteinflow pickle file, a PDB file or a SAbDab file directly
 and can be used to process the data and extract additional features. The processed data can be saved as a
 proteinflow pickle file or a PDB file.
 
 """
 import os
 import pickle
-import urllib
+import tempfile
 import warnings
+from collections import defaultdict
 
 import numpy as np
 import pandas as pd
-import requests
+import py3Dmol
 from Bio import pairwise2
 from biopandas.pdb import PandasPdb
 from methodtools import lru_cache
+from torch import Tensor
 
 from proteinflow.constants import (
     _PMAP,
     ALPHABET,
     ALPHABET_REVERSE,
     ATOM_MASKS,
     BACKBONE_ORDER,
     CDR_ALPHABET,
     CDR_REVERSE,
     CDR_VALUES,
+    COLORS,
     D3TO1,
     MAIN_ATOM_DICT,
     SIDECHAIN_ORDER,
 )
 from proteinflow.data.utils import (
     CustomMmcif,
     PDBBuilder,
     PDBError,
     _annotate_sse,
+    _Atom,
     _dihedral_angle,
     _retrieve_chain_names,
 )
 from proteinflow.download import download_fasta, download_pdb
+from proteinflow.ligand import _get_ligands
 
 
 def interpolate_coords(crd, mask, fill_ends=True):
     """Fill in missing values in a coordinates array with linear interpolation.
 
     Parameters
     ----------
@@ -86,15 +91,15 @@
 
 class ProteinEntry:
     """A class to interact with proteinflow data files."""
 
     ATOM_ORDER = {k: BACKBONE_ORDER + v for k, v in SIDECHAIN_ORDER.items()}
     """A dictionary mapping 3-letter residue names to the order of atoms in the coordinates array."""
 
-    def __init__(self, seqs, crds, masks, chain_ids, cdrs=None):
+    def __init__(self, seqs, crds, masks, chain_ids, predict_masks=None, cdrs=None):
         """Initialize a `ProteinEntry` object.
 
         Parameters
         ----------
         seqs : list of str
             Amino acid sequences of the protein (one-letter code)
         crds : list of np.ndarray
@@ -104,23 +109,35 @@
             Mask arrays where 1 indicates residues with known coordinates and 0
             indicates missing values
         cdrs : list of np.ndarray
             `'numpy'` arrays of shape `(L,)` where CDR residues are marked with the corresponding type (`'H1'`, `'L1'`, ...)
             and non-CDR residues are marked with `'-'`
         chain_ids : list of str
             Chain IDs of the protein
+        predict_masks : list of np.ndarray, optional
+            Mask arrays where 1 indicates residues that were generated by a model and 0
+            indicates residues with known coordinates
+        cdrs : list of np.ndarray, optional
+            `'numpy'` arrays of shape `(L,)` where CDR residues are marked with the corresponding type (`'H1'`, `'L1'`, ...)
 
         """
+        if crds[0].shape[1] != 14:
+            raise ValueError(
+                "Coordinates array must have 14 atoms in the order of N, C, CA, O, sidechain atoms"
+            )
         self.seq = {x: seq for x, seq in zip(chain_ids, seqs)}
         self.crd = {x: crd for x, crd in zip(chain_ids, crds)}
         self.mask = {x: mask for x, mask in zip(chain_ids, masks)}
         self.mask_original = {x: mask for x, mask in zip(chain_ids, masks)}
         if cdrs is None:
             cdrs = [None for _ in chain_ids]
         self.cdr = {x: cdr for x, cdr in zip(chain_ids, cdrs)}
+        if predict_masks is None:
+            predict_masks = [None for _ in chain_ids]
+        self.predict_mask = {x: mask for x, mask in zip(chain_ids, predict_masks)}
 
     def interpolate_coords(self, fill_ends=True):
         """Fill in missing values in the coordinates arrays with linear interpolation.
 
         Parameters
         ----------
         fill_ends : bool, default True
@@ -141,15 +158,14 @@
             start, end = known_ind[0], known_ind[-1] + 1
             self.seq[chain] = self.seq[chain][start:end]
             self.crd[chain] = self.crd[chain][start:end]
             self.mask[chain] = self.mask[chain][start:end]
             if self.cdr[chain] is not None:
                 self.cdr[chain] = self.cdr[chain][start:end]
 
-    @lru_cache()
     def get_chains(self):
         """Get the chain IDs of the protein.
 
         Returns
         -------
         chains : list of str
             Chain IDs of the protein
@@ -346,17 +362,14 @@
             If `True`, return the original mask (before interpolation)
 
         Returns
         -------
         mask : np.ndarray
             Mask array where 1 indicates residues with known coordinates and 0
             indicates missing values
-        chains : list of str, optional
-            If specified, only the masks of the specified chains are returned (in the same order);
-            otherwise, all masks are concatenated in alphabetical order of the chain IDs
 
         """
         if cdr is not None and self.cdr is None:
             raise ValueError("CDR information not available")
         if cdr is not None:
             assert cdr in CDR_REVERSE, f"CDR must be one of {list(CDR_REVERSE.keys())}"
         chains = self._get_chains_list(chains)
@@ -448,15 +461,24 @@
         -------
         cdr : np.ndarray
             A `'numpy'` array of shape `(L,)` where CDR residues are marked
             with the corresponding type (`'H1'`, `'L1'`, ...) and non-CDR
             residues are marked with `'-'`
 
         """
-        return np.array([CDR_ALPHABET[x] for x in cdr])
+        cdr = ProteinEntry._to_numpy(cdr)
+        return np.array([CDR_ALPHABET[x] for x in cdr.astype(int)])
+
+    @staticmethod
+    def _to_numpy(arr):
+        if isinstance(arr, Tensor):
+            arr = arr.detach().cpu().numpy()
+        if isinstance(arr, list):
+            arr = np.array(arr)
+        return arr
 
     @staticmethod
     def decode_sequence(seq):
         """Decode the amino acid sequence.
 
         Parameters
         ----------
@@ -466,15 +488,119 @@
 
         Returns
         -------
         seq : str
             Amino acid sequence of the protein (one-letter code)
 
         """
-        return "".join([ALPHABET[x] for x in seq])
+        seq = ProteinEntry._to_numpy(seq)
+        return "".join([ALPHABET[x] for x in seq.astype(int)])
+
+    def rename_chains(self, chain_dict):
+        """Rename the chains of the protein.
+
+        Parameters
+        ----------
+        chain_dict : dict
+            A dictionary mapping old chain IDs to new chain IDs
+
+        """
+        for old_chain, new_chain in chain_dict.items():
+            self.seq[new_chain] = self.seq.pop(old_chain)
+            self.crd[new_chain] = self.crd.pop(old_chain)
+            self.mask[new_chain] = self.mask.pop(old_chain)
+            self.mask_original[new_chain] = self.mask_original.pop(old_chain)
+            self.cdr[new_chain] = self.cdr.pop(old_chain)
+            self.predict_mask[new_chain] = self.predict_mask.pop(old_chain)
+
+    def merge(self, entry):
+        """Merge another `ProteinEntry` object into this one.
+
+        Parameters
+        ----------
+        entry : ProteinEntry
+            A `ProteinEntry` object
+
+        """
+        for chain in entry.get_chains():
+            if chain.split("_")[0] in {x.split("_")[0] for x in self.get_chains()}:
+                raise ValueError("Chain IDs must be unique")
+            self.seq[chain] = entry.seq[chain]
+            self.crd[chain] = entry.crd[chain]
+            self.mask[chain] = entry.mask[chain]
+            self.mask_original[chain] = entry.mask_original[chain]
+            self.cdr[chain] = entry.cdr[chain]
+            self.predict_mask[chain] = entry.predict_mask[chain]
+        if not all([x is None for x in entry.predict_mask.values()]):
+            for k, v in self.predict_mask.items():
+                if v is None:
+                    self.predict_mask[k] = np.zeros(len(self.get_sequence(k)))
+
+    @staticmethod
+    def from_arrays(
+        seqs, crds, masks, chain_id_dict, chain_id_array, predict_masks=None, cdrs=None
+    ):
+        """Load a protein entry from arrays.
+
+        Parameters
+        ----------
+        seqs : np.ndarray
+            Amino acid sequences of the protein (encoded as integers, see `proteinflow.constants.ALPHABET`), `'numpy'` array of shape `(L,)`
+        crds : np.ndarray
+            Coordinates of the protein, `'numpy'` array of shape `(L, 14, 3)` or `(L, 4, 3)`
+        masks : np.ndarray
+            Mask array where 1 indicates residues with known coordinates and 0
+            indicates missing values, `'numpy'` array of shape `(L,)`
+        chain_id_dict : dict
+            A dictionary mapping chain IDs to indices in `chain_id_array`
+        chain_id_array : np.ndarray
+            A `'numpy'` array of chain IDs encoded as integers
+        predict_masks : np.ndarray, optional
+            Mask array where 1 indicates residues that were generated by a model and 0
+            indicates residues with known coordinates, `'numpy'` array of shape `(L,)`
+        cdrs : np.ndarray, optional
+            A `'numpy'` array of shape `(L,)` where residues are marked
+            with the corresponding CDR type (encoded as integers, see `proteinflow.constants.CDR_ALPHABET`)
+
+        Returns
+        -------
+        entry : ProteinEntry
+            A `ProteinEntry` object
+
+        """
+        seqs_list = []
+        crds_list = []
+        masks_list = []
+        chain_ids_list = []
+        predict_masks_list = None if predict_masks is None else []
+        cdrs_list = None if cdrs is None else []
+        if crds.shape[1] != 14:
+            crds_ = np.zeros((crds.shape[0], 14, 3))
+            crds_[:, :4, :] = ProteinEntry._to_numpy(crds)
+            crds = crds_
+        for chain_id, ind in chain_id_dict.items():
+            chain_ids_list.append(chain_id)
+            chain_mask = chain_id_array == ind
+            seqs_list.append(ProteinEntry.decode_sequence(seqs[chain_mask]))
+            crds_list.append(ProteinEntry._to_numpy(crds[chain_mask]))
+            masks_list.append(ProteinEntry._to_numpy(masks[chain_mask]))
+            if predict_masks is not None:
+                predict_masks_list.append(
+                    ProteinEntry._to_numpy(predict_masks[chain_mask])
+                )
+            if cdrs is not None:
+                cdrs_list.append(ProteinEntry.decode_cdr(cdrs[chain_mask]))
+        return ProteinEntry(
+            seqs_list,
+            crds_list,
+            masks_list,
+            chain_ids_list,
+            predict_masks_list,
+            cdrs_list,
+        )
 
     @staticmethod
     def from_dict(dictionary):
         """Load a protein entry from a dictionary.
 
         Parameters
         ----------
@@ -482,17 +608,18 @@
             A nested dictionary where first-level keys are chain IDs and
             second-level keys are the following:
             - `'seq'` : amino acid sequence (one-letter code)
             - `'crd_bb'` : backbone coordinates, shaped `(L, 4, 3)`
             - `'crd_sc'` : sidechain coordinates, shaped `(L, 10, 3)`
             - `'msk'` : mask array where 1 indicates residues with known coordinates and 0
                 indicates missing values, shaped `(L,)`
-            - `'cdr'` (optional): CDR information, shaped `(L,)` encoded as integers where each
-                integer corresponds to the index of the CDR type in
-                `proteinflow.constants.CDR_ALPHABET`
+            - `'cdr'` (optional): CDR information, shaped `(L,)` where CDR residues are marked
+                with the corresponding type (`'H1'`, `'L1'`, ...) and non-CDR residues are marked with `'-'`
+            - `'predict_msk'` (optional): mask array where 1 indicates residues that were generated by a model and 0
+                indicates residues with known coordinates, shaped `(L,)`
 
         Returns
         -------
         entry : ProteinEntry
             A `ProteinEntry` object
 
         """
@@ -500,15 +627,61 @@
         seq = [dictionary[k]["seq"] for k in chains]
         crd = [
             np.concatenate([dictionary[k]["crd_bb"], dictionary[k]["crd_sc"]], axis=1)
             for k in chains
         ]
         mask = [dictionary[k]["msk"] for k in chains]
         cdr = [dictionary[k].get("cdr", None) for k in chains]
-        return ProteinEntry(seqs=seq, crds=crd, masks=mask, cdrs=cdr, chain_ids=chains)
+        predict_mask = [dictionary[k].get("predict_msk", None) for k in chains]
+        return ProteinEntry(
+            seqs=seq,
+            crds=crd,
+            masks=mask,
+            cdrs=cdr,
+            chain_ids=chains,
+            predict_masks=predict_mask,
+        )
+
+    @staticmethod
+    def from_pdb_entry(pdb_entry):
+        """Load a protein entry from a `PDBEntry` object.
+
+        Parameters
+        ----------
+        pdb_entry : PDBEntry
+            A `PDBEntry` object
+
+        Returns
+        -------
+        entry : ProteinEntry
+            A `ProteinEntry` object
+
+        """
+        pdb_dict = {}
+        fasta_dict = pdb_entry.get_fasta()
+        for (chain,) in pdb_entry.get_chains():
+            pdb_dict[chain] = {}
+            fasta_seq = fasta_dict[chain]
+
+            # align fasta and pdb and check criteria)
+            mask = pdb_entry.get_mask([chain])[chain]
+            if isinstance(pdb_entry, SAbDabEntry):
+                pdb_dict[chain]["cdr"] = pdb_entry.get_cdr([chain])[chain]
+            pdb_dict[chain]["seq"] = fasta_seq
+            pdb_dict[chain]["msk"] = mask
+
+            # go over rows of coordinates
+            crd_arr = pdb_entry.get_coordinates_array(chain)
+
+            pdb_dict[chain]["crd_bb"] = crd_arr[:, :4, :]
+            pdb_dict[chain]["crd_sc"] = crd_arr[:, 4:, :]
+            pdb_dict[chain]["msk"][
+                (pdb_dict[chain]["crd_bb"] == 0).sum(-1).sum(-1) > 0
+            ] = 0
+        return ProteinEntry.from_dict(pdb_dict)
 
     @staticmethod
     def from_pdb(
         pdb_path,
         fasta_path=None,
         heavy_chain=None,
         light_chain=None,
@@ -542,37 +715,56 @@
                 fasta_path=fasta_path,
                 heavy_chain=heavy_chain,
                 light_chain=light_chain,
                 antigen_chains=antigen_chains,
             )
         else:
             pdb_entry = PDBEntry(pdb_path=pdb_path, fasta_path=fasta_path)
-        pdb_dict = {}
-        fasta_dict = pdb_entry.get_fasta()
+        return ProteinEntry.from_pdb_entry(pdb_entry)
 
-        for (chain,) in pdb_entry.get_chains():
-            pdb_dict[chain] = {}
-            fasta_seq = fasta_dict[chain]
+    @staticmethod
+    def from_id(
+        pdb_id,
+        local_folder=".",
+        heavy_chain=None,
+        light_chain=None,
+        antigen_chains=None,
+    ):
+        """Load a protein entry from a PDB file.
 
-            # align fasta and pdb and check criteria)
-            mask = pdb_entry.get_mask([chain])[chain]
-            if isinstance(pdb_entry, SAbDabEntry):
-                pdb_dict[chain]["cdr"] = pdb_entry.get_cdr([chain])[chain]
-            pdb_dict[chain]["seq"] = fasta_seq
-            pdb_dict[chain]["msk"] = mask
+        Parameters
+        ----------
+        pdb_id : str
+            PDB ID of the protein
+        local_folder : str, default "."
+            Path to the local folder where the PDB file is saved
+        heavy_chain : str, optional
+            Chain ID of the heavy chain (to load a SAbDab entry)
+        light_chain : str, optional
+            Chain ID of the light chain (to load a SAbDab entry)
+        antigen_chains : list of str, optional
+            Chain IDs of the antigen chains (to load a SAbDab entry)
 
-            # go over rows of coordinates
-            crd_arr = pdb_entry.get_coordinates_array(chain)
+        Returns
+        -------
+        entry : ProteinEntry
+            A `ProteinEntry` object
 
-            pdb_dict[chain]["crd_bb"] = crd_arr[:, :4, :]
-            pdb_dict[chain]["crd_sc"] = crd_arr[:, 4:, :]
-            pdb_dict[chain]["msk"][
-                (pdb_dict[chain]["crd_bb"] == 0).sum(-1).sum(-1) > 0
-            ] = 0
-        return ProteinEntry.from_dict(pdb_dict)
+        """
+        if heavy_chain is not None or light_chain is not None:
+            pdb_entry = SAbDabEntry.from_id(
+                pdb_id=pdb_id,
+                local_folder=local_folder,
+                heavy_chain=heavy_chain,
+                light_chain=light_chain,
+                antigen_chains=antigen_chains,
+            )
+        else:
+            pdb_entry = PDBEntry.from_id(pdb_id=pdb_id)
+        return ProteinEntry.from_pdb_entry(pdb_entry)
 
     @staticmethod
     def from_pickle(path):
         """Load a protein entry from a pickle file.
 
         Parameters
         ----------
@@ -601,26 +793,30 @@
             - `'crd_bb'` : backbone coordinates, shaped `(L, 4, 3)`
             - `'crd_sc'` : sidechain coordinates, shaped `(L, 10, 3)`
             - `'msk'` : mask array where 1 indicates residues with known coordinates and 0
                 indicates missing values, shaped `(L,)`
             - `'cdr'` (optional): CDR information, shaped `(L,)` encoded as integers where each
                 integer corresponds to the index of the CDR type in
                 `proteinflow.constants.CDR_ALPHABET`
+            - `'predict_msk'` (optional): mask array where 1 indicates residues that were generated by a model and 0
+                indicates residues with known coordinates, shaped `(L,)`
 
         """
         data = {}
         for chain in self.get_chains():
             data[chain] = {
                 "seq": self.seq[chain],
                 "crd_bb": self.crd[chain][:, :4],
                 "crd_sc": self.crd[chain][:, 4:],
                 "msk": self.mask[chain],
             }
             if self.cdr[chain] is not None:
                 data[chain]["cdr"] = self.cdr[chain]
+            if self.predict_mask[chain] is not None:
+                data[chain]["predict_msk"] = self.predict_mask[chain]
         return data
 
     def to_pdb(
         self,
         path,
         only_ca=False,
         skip_oxygens=False,
@@ -661,14 +857,18 @@
             zeros to missing values,
         - `'seq'`: a string of length `L` with residue types.
 
         In a SAbDab datasets, an additional key is added to the dictionary:
         - `'cdr'`: a `'numpy'` array of shape `(L,)` where CDR residues are marked with the corresponding type (`'H1'`, `'L1'`, ...)
             and non-CDR residues are marked with `'-'`.
 
+        If a prediction mask is available, another additional key is added to the dictionary:
+        - `'predict_msk'`: a `numpy` array of shape `(L,)` where ones correspond to residues that were generated by a model and
+            zeros to residues with known coordinates.
+
         Parameters
         ----------
         path : str
             Path to the pickle file
 
         """
         data = self.to_dict()
@@ -987,19 +1187,102 @@
             chain_length = self.get_length([chain])
             index_array[start_index : start_index + chain_length] = (
                 id_dict[chain] if encode else chain
             )
             start_index += chain_length
         return index_array
 
+    def _get_highlight_mask_dict(self, highlight_mask=None):
+        """Turn mask array into a dictionary."""
+        chain_arr = self.get_chain_id_array(encode=False)
+        mask_arr = self.get_mask().astype(bool)
+        highlight_mask_dict = {}
+        if highlight_mask is not None:
+            chains = self.get_chains()
+            for chain in chains:
+                chain_mask = chain_arr == chain
+                pdb_highlight = highlight_mask[mask_arr & chain_mask]
+                highlight_mask_dict[chain] = pdb_highlight
+        return highlight_mask_dict
+
+    def _get_atom_dicts(self, highlight_mask=None, style="cartoon", opacity=1):
+        """Get the atom dictionaries of the protein."""
+        highlight_mask_dict = self._get_highlight_mask_dict(highlight_mask)
+        with tempfile.NamedTemporaryFile(suffix=".pdb") as tmp:
+            self.to_pdb(tmp.name)
+            pdb_entry = PDBEntry(tmp.name)
+        return pdb_entry._get_atom_dicts(
+            highlight_mask_dict=highlight_mask_dict, style=style, opacity=opacity
+        )
+
+    def get_predict_mask(self, chains=None):
+        """Get the prediction mask of the protein.
+
+        The prediction mask is a `'numpy'` array of shape `(L,)` with ones
+        corresponding to residues that were generated by a model and zeros to
+        residues with known coordinates. If the prediction mask is not available,
+        `None` is returned.
+
+        Parameters
+        ----------
+        chains : list of str, optional
+            If specified, only the prediction mask of the specified chains is returned (in the same order);
+            otherwise, all features are concatenated in alphabetical order of the chain IDs
+
+        Returns
+        -------
+        predict_mask : np.ndarray
+            A `'numpy'` array of shape `(L,)` with ones corresponding to residues that were generated by a model and
+            zeros to residues with known coordinates
+
+        """
+        if list(self.predict_mask.values())[0] is None:
+            return None
+        chains = self._get_chains_list(chains)
+        predict_mask = np.concatenate([self.predict_mask[chain] for chain in chains])
+        return predict_mask
+
+    def visualize(self, highlight_mask=None, style="cartoon", opacity=1):
+        """Visualize the protein in a notebook.
+
+        Parameters
+        ----------
+        highlight_mask : np.ndarray, optional
+            A `'numpy'` array of shape `(L,)` with the residues to highlight
+            marked with 1 and the rest marked with 0; if not given and
+            `self.predict_mask` is not `None`, the predicted residues are highlighted
+        style : str, default 'cartoon'
+            The style of the visualization; one of 'cartoon', 'sphere', 'stick', 'line', 'cross'
+        opacity : float or dict, default 1
+            Opacity of the visualization (can be a dictionary mapping from chain IDs to opacity values)
+
+        """
+        print(f"{highlight_mask=}")
+        if highlight_mask is not None:
+            highlight_mask_dict = self._get_highlight_mask_dict(highlight_mask)
+        elif list(self.predict_mask.values())[0] is not None:
+            print("HERE")
+            highlight_mask_dict = {
+                chain: self.predict_mask[chain][self.get_mask([chain]).astype(bool)]
+                for chain in self.get_chains()
+            }
+        else:
+            highlight_mask_dict = None
+        with tempfile.NamedTemporaryFile(suffix=".pdb") as tmp:
+            self.to_pdb(tmp.name)
+            pdb_entry = PDBEntry(tmp.name)
+        pdb_entry.visualize(
+            highlight_mask_dict=highlight_mask_dict, style=style, opacity=opacity
+        )
+
 
 class PDBEntry:
     """A class for parsing PDB entries."""
 
-    def __init__(self, pdb_path, fasta_path=None):
+    def __init__(self, pdb_path, fasta_path=None, load_ligand=False):
         """Initialize a PDBEntry object.
 
         If no FASTA path is provided, the sequences will be fully inferred
         from the PDB file.
 
         Parameters
         ----------
@@ -1008,15 +1291,19 @@
         fasta_path : str, optional
             Path to the FASTA file
 
         """
         self.pdb_path = pdb_path
         self.fasta_path = fasta_path
         self.pdb_id = os.path.basename(pdb_path).split(".")[0].split("-")[0]
-        self.crd_df, self.seq_df = self._parse_structure()
+        self.load_ligand = load_ligand
+        if load_ligand:
+            self.crd_df, self.seq_df, self.ligands = self._parse_structure()
+        else:
+            self.crd_df, self.seq_df = self._parse_structure()
         self.fasta_dict = self._parse_fasta()
 
     @staticmethod
     def from_id(pdb_id, local_folder="."):
         """Initialize a `PDBEntry` object from a PDB Id.
 
         Downloads the PDB and FASTA files to the local folder.
@@ -1034,14 +1321,57 @@
             A `PDBEntry` object
 
         """
         pdb_path = download_pdb(pdb_id, local_folder)
         fasta_path = download_fasta(pdb_id, local_folder)
         return PDBEntry(pdb_path=pdb_path, fasta_path=fasta_path)
 
+    def rename_chains(self, chain_dict):
+        """Rename chains in the PDB entry.
+
+        Parameters
+        ----------
+        chain_dict : dict
+            A dictionary mapping from old chain IDs to new chain IDs
+
+        Returns
+        -------
+        entry : PDBEntry
+            A `PDBEntry` object
+
+        """
+        self.crd_df["chain_id"] = self.crd_df["chain_id"].replace(chain_dict)
+        self.seq_df["chain_id"] = self.seq_df["chain_id"].replace(chain_dict)
+        return self
+
+    def merge(self, entry):
+        """Merge two PDB entries.
+
+        Parameters
+        ----------
+        entry : PDBEntry
+            A `PDBEntry` object
+
+        Returns
+        -------
+        entry : PDBEntry
+            A `PDBEntry` object
+
+        """
+        if entry.pdb_id != self.pdb_id:
+            self.pdb_id = f"{self.pdb_id}+{entry.pdb_id}"
+        for chain in entry.get_chains():
+            if chain.split("_")[0] in {x.split("_")[0] for x in self.get_chains()}:
+                raise ValueError("Chain IDs must be unique")
+        self.crd_df = pd.concat([self.crd_df, entry.crd_df], ignore_index=True)
+        self.seq_df = pd.concat([self.seq_df, entry.seq_df], ignore_index=True)
+        self.crd_df.loc[:, "atom_number"] = np.arange(len(self.crd_df))
+        self.fasta_dict.update(entry.fasta_dict)
+        return self
+
     def _get_relevant_chains(self):
         """Get the chains that are included in the entry."""
         return list(self.seq_df["chain_id"].unique())
 
     @staticmethod
     def parse_fasta(fasta_path):
         """Read a fasta file.
@@ -1113,14 +1443,26 @@
         crd_df = crd_df[crd_df["record_name"] == "ATOM"].reset_index()
         if "insertion" in crd_df.columns:
             crd_df["unique_residue_number"] = crd_df.apply(
                 lambda row: f"{row['residue_number']}_{row['insertion']}", axis=1
             )
         seq_df = p.amino3to1()
 
+        if self.load_ligand:
+            chain2ligands = None
+            try:
+                chain2ligands = _get_ligands(
+                    self.pdb_id,
+                    p,
+                    self.pdb_path,
+                )
+            except Exception:
+                raise PDBError("Failed to retrieve ligands")
+            return crd_df, seq_df, chain2ligands
+
         return crd_df, seq_df
 
     def _get_chain(self, chain):
         """Check the chain ID."""
         if chain is None:
             return chain
         if chain not in self.get_chains():
@@ -1183,14 +1525,26 @@
         fasta_dict : dict
             A dictionary containing all the (author) chains in a fasta file (keys)
             and their corresponding sequence (values)
 
         """
         return self.fasta_dict
 
+    def get_ligands(self):
+        """Return the ligands dictionary.
+
+        Returns
+        -------
+        ligands : dict
+            A dictionary containing all the chains in a pdb file (keys)
+            and their corresponding processed ligands (values)
+
+        """
+        return self.ligands
+
     def get_chains(self):
         """Return the chains in the PDB.
 
         Returns
         -------
         chains : list
             A list of chain identifiers
@@ -1351,14 +1705,71 @@
         -------
         unique_numbers : list
             A list of unique residue numbers
 
         """
         return self.get_pdb_df(chain)["unique_residue_number"].unique().tolist()
 
+    def _get_atom_dicts(self, highlight_mask_dict=None, style="cartoon", opacity=1):
+        """Get the atom dictionaries for visualization."""
+        assert style in ["cartoon", "sphere", "stick", "line", "cross"]
+        outstr = []
+        df_ = self.crd_df.sort_values(["chain_id", "residue_number"], inplace=False)
+        for _, row in df_.iterrows():
+            outstr.append(_Atom(row))
+        chains = self.get_chains()
+        colors = {ch: COLORS[i % len(COLORS)] for i, ch in enumerate(chains)}
+        chain_counters = defaultdict(int)
+        chain_last_res = defaultdict(lambda: None)
+        if highlight_mask_dict is not None:
+            for chain, mask in highlight_mask_dict.items():
+                assert len(mask) == len(
+                    self._pdb_sequence(chain)
+                ), "Mask length does not match sequence length"
+        for at in outstr:
+            if isinstance(opacity, dict):
+                op_ = opacity[at["chain"]]
+            else:
+                op_ = opacity
+            if at["resid"] != chain_last_res[at["chain"]]:
+                chain_last_res[at["chain"]] = at["resid"]
+                chain_counters[at["chain"]] += 1
+            at["pymol"] = {style: {"color": colors[at["chain"]], "opacity": op_}}
+            if highlight_mask_dict is not None and at["chain"] in highlight_mask_dict:
+                num = chain_counters[at["chain"]]
+                if highlight_mask_dict[at["chain"]][num - 1] == 1:
+                    at["pymol"] = {style: {"color": "red", "opacity": op_}}
+        return outstr
+
+    def visualize(self, highlight_mask_dict=None, style="cartoon", opacity=1):
+        """Visualize the protein in a notebook.
+
+        Parameters
+        ----------
+        highlight_mask_dict : dict, optional
+            A dictionary mapping from chain IDs to a mask of 0s and 1s of the same length as the chain sequence;
+            the atoms corresponding to 1s will be highlighted in red
+        style : str, default 'cartoon'
+            The style of the visualization; one of 'cartoon', 'sphere', 'stick', 'line', 'cross'
+        opacity : float or dict, default 1
+            Opacity of the visualization (can be a dictionary mapping from chain IDs to opacity values)
+
+        """
+        outstr = self._get_atom_dicts(highlight_mask_dict, style=style, opacity=opacity)
+        vis_string = "".join([str(x) for x in outstr])
+        view = py3Dmol.view(width=400, height=300)
+        view.addModelsAsFrames(vis_string)
+        for i, at in enumerate(outstr):
+            view.setStyle(
+                {"model": -1, "serial": i + 1},
+                at["pymol"],
+            )
+        view.zoomTo()
+        view.show()
+
 
 class SAbDabEntry(PDBEntry):
     """A class for parsing SAbDab entries."""
 
     def __init__(
         self,
         pdb_path,
```

### Comparing `proteinflow-2.0.0/proteinflow/data/torch.py` & `proteinflow-2.1.0/proteinflow/data/torch.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,60 +15,14 @@
 from proteinflow.constants import ALPHABET, CDR_REVERSE, D3TO1, MAIN_ATOMS
 from proteinflow.data import ProteinEntry
 
 
 class _PadCollate:
     """A variant of `collate_fn` that pads according to the longest sequence in a batch of sequences."""
 
-    def __init__(
-        self,
-        mask_residues=True,
-        lower_limit=15,
-        upper_limit=100,
-        mask_frac=None,
-        mask_whole_chains=False,
-        force_binding_sites_frac=0.15,
-        mask_all_cdrs=False,
-    ):
-        """Initialize a _PadCollate object.
-
-        Parameters
-        ----------
-        batch : dict
-            a batch generated by `ProteinDataset` and `PadCollate`
-        lower_limit : int, default 15
-            the minimum number of residues to mask
-        upper_limit : int, default 100
-            the maximum number of residues to mask
-        mask_frac : float, optional
-            if given, the `lower_limit` and `upper_limit` are ignored and the number of residues to mask is `mask_frac` times the length of the chain
-        mask_whole_chains : bool, default False
-            if `True`, `upper_limit`, `force_binding_sites` and `lower_limit` are ignored and the whole chain is masked instead
-        force_binding_sites_frac : float, default 0.15
-            if > 0, in the fraction of cases where a chain from a polymer is sampled, the center of the masked region will be
-            forced to be in a binding site
-        mask_all_cdrs : bool, default False
-            if `True`, all CDRs are masked
-
-        Returns
-        -------
-        chain_M : torch.Tensor
-            a `(B, L)` shaped binary tensor where 1 denotes the part that needs to be predicted and
-            0 is everything else
-
-        """
-        super().__init__()
-        self.mask_residues = mask_residues
-        self.lower_limit = lower_limit
-        self.upper_limit = upper_limit
-        self.mask_frac = mask_frac
-        self.mask_whole_chains = mask_whole_chains
-        self.force_binding_sites_frac = force_binding_sites_frac
-        self.mask_all_cdrs = mask_all_cdrs
-
     def pad_collate(self, batch):
         # find longest sequence
         out = {}
         max_len = max(map(lambda x: x["S"].shape[0], batch))
 
         # pad according to max_len
         to_pad = [max_len - b["S"].shape[0] for b in batch]
```

### Comparing `proteinflow-2.0.0/proteinflow/data/utils.py` & `proteinflow-2.1.0/proteinflow/data/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,19 @@
             If True, the oxygen atoms will be excluded from the PDB file
         only_backbone : bool, default False
             If True, only the backbone atoms will be included in the PDB file
 
         """
         seq = protein_entry.get_sequence()
         coords = protein_entry.get_coordinates()
+        mask = protein_entry.get_mask().astype(bool)
+        seq = "".join(np.array(list(seq))[mask])
+        coords = coords[mask]
+        if (coords[:, 4:] == 0).all():
+            only_backbone = True
         if only_ca:
             coords = coords[:, 2, :].unsqueeze(1)
         elif skip_oxygens:
             coords = coords[:, :3, :]
         elif only_backbone:
             coords = coords[:, :4, :]
         coords = rearrange(coords, "l n c -> (l n) c")
@@ -62,15 +67,15 @@
         self.skip_oxygens = skip_oxygens
         self.atoms_per_res = atoms_per_res
         self.only_backbone = only_backbone
         self.coords = coords
         self.seq = seq
         self.mapping = self._make_mapping_from_seq()
 
-        self.chain_ids = protein_entry.get_chain_id_array(encode=False)
+        self.chain_ids = protein_entry.get_chain_id_array(encode=False)[mask]
         self.chain_ids_unique = protein_entry.get_chains()
 
         # PDB Formatting Information
         self.format_str = (
             "{:6s}{:5d} {:^4s}{:1s}{:3s} {:1s}{:4d}{:1s}   {:8.3f}{:8.3f}"
             "{:8.3f}{:6.2f}{:6.2f}          {:>2s}{:2s}"
         )
@@ -445,19 +450,21 @@
         """
         x = super().read_mmcif(path)
         x.df["ATOM"].rename(
             {
                 "label_comp_id": "residue_name",
                 "label_seq_id": "residue_number",
                 "label_atom_id": "atom_name",
+                "id": "atom_number",
                 "group_PDB": "record_name",
                 "Cartn_x": "x_coord",
                 "Cartn_y": "y_coord",
                 "Cartn_z": "z_coord",
                 "pdbx_PDB_ins_code": "insertion",
+                "type_symbol": "element_symbol",
             },
             axis=1,
             inplace=True,
         )
         x.df["ATOM"]["chain_id"] = x.df["ATOM"]["auth_asym_id"]
         return x
 
@@ -515,7 +522,35 @@
     """Retrieve the (author) chain names present in one header line of a fasta file (line that begins with '>')."""
     entry = entry.split("|")[1]
 
     if "Chains" in entry:
         return [_retrieve_author_chain(e) for e in entry[7:].split(", ")]
 
     return [_retrieve_author_chain(entry[6:])]
+
+
+class _Atom(dict):
+    def __init__(self, row):
+        self["type"] = row["record_name"]
+        self["idx"] = row["atom_number"]
+        self["name"] = row["atom_name"]
+        self["resname"] = row["residue_name"]
+        self["resid"] = row["residue_number"]
+        self["chain"] = row["chain_id"]
+        self["x"] = row["x_coord"]
+        self["y"] = row["y_coord"]
+        self["z"] = row["z_coord"]
+        self["sym"] = row["element_symbol"]
+
+    def __str__(self):
+        line = list(" " * 80)
+
+        line[0:6] = self["type"].ljust(6)
+        line[6:11] = str(self["idx"]).ljust(5)
+        line[12:16] = self["name"].ljust(4)
+        line[17:20] = self["resname"].ljust(3)
+        line[22:26] = str(self["resid"]).ljust(4)
+        line[30:38] = str(self["x"]).rjust(8)
+        line[38:46] = str(self["y"]).rjust(8)
+        line[46:54] = str(self["z"]).rjust(8)
+        line[76:78] = self["sym"].rjust(2)
+        return "".join(line) + "\n"
```

### Comparing `proteinflow-2.0.0/proteinflow/download/__init__.py` & `proteinflow-2.1.0/proteinflow/download/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Functions for downloading protein data from various sources."""
 
+import multiprocessing
 import os
 import shutil
 import subprocess
 import urllib
 import urllib.request
 import zipfile
 from concurrent import futures
@@ -13,14 +14,15 @@
 import boto3
 import numpy as np
 import pandas as pd
 import requests
 from botocore import UNSIGNED
 from botocore.config import Config
 from bs4 import BeautifulSoup
+from joblib import Parallel, delayed
 from p_tqdm import p_map
 from rcsbsearch import Attr
 from tqdm import tqdm
 
 from proteinflow.constants import ALLOWED_AG_TYPES
 from proteinflow.download.boto import (
     _download_dataset_dicts_from_s3,
@@ -52,14 +54,15 @@
 
     Returns
     -------
     local_path : str
         Path to the downloaded file
 
     """
+    pdb_id = pdb_id.lower()
     if sabdab:
         try:
             url = f"https://opig.stats.ox.ac.uk/webapps/sabdab-sabpred/sabdab/pdb/{pdb_id}/?scheme=chothia"
             local_path = os.path.join(local_folder, f"{pdb_id}.pdb")
             _download_file(url, local_path)
             return local_path
         except BaseException:
@@ -101,14 +104,15 @@
 
     Returns
     -------
     local_path : str
         Path to the downloaded file
 
     """
+    pdb_id = pdb_id.lower()
     if "-" in pdb_id:
         pdb_id = pdb_id.split("-")[0]
     downloadurl = "https://www.rcsb.org/fasta/entry/"
     pdbfn = pdb_id + "/download"
     local_path = os.path.join(local_folder, f"{pdb_id.lower()}.fasta")
 
     url = downloadurl + pdbfn
@@ -117,39 +121,59 @@
 
 
 def get_pdb_ids(
     resolution_thr=3.5,
     pdb_snapshot=None,
     filter_methods=True,
     max_chains=5,
+    pdb_id_list_path=None,
 ):
     """Get PDB ids from PDB API."""
-    # get filtered PDB ids from PDB API
-    pdb_ids = (
-        Attr("rcsb_entry_info.selected_polymer_entity_types")
-        .__eq__("Protein (only)")
-        .or_("rcsb_entry_info.polymer_composition")
-        .__eq__("protein/oligosaccharide")
-    )
-    # if include_na:
-    #     pdb_ids = pdb_ids.or_('rcsb_entry_info.polymer_composition').in_(["protein/NA", "protein/NA/oligosaccharide"])
+    if pdb_id_list_path is not None:
+        pdb_ids = []  # List to store the extracted elements
 
-    if max_chains is not None:
-        pdb_ids = pdb_ids.and_(
-            "rcsb_assembly_info.polymer_entity_instance_count_protein"
-        ).__le__(max_chains)
-    if resolution_thr is not None:
-        pdb_ids = pdb_ids.and_("rcsb_entry_info.resolution_combined").__le__(
-            resolution_thr
-        )
-    if filter_methods:
-        pdb_ids = pdb_ids.and_("exptl.method").in_(
-            ["X-RAY DIFFRACTION", "ELECTRON MICROSCOPY"]
+        try:
+            with open(pdb_id_list_path) as file:
+                # Read lines from the file
+                lines = file.readlines()
+
+                # Process each line
+                for line in lines:
+                    # Extract elements from the line (example: splitting by whitespace)
+                    line_elements = line.split()
+
+                    # Add extracted elements to the list
+                    pdb_ids.extend(line_elements)
+                pdb_ids = np.unique(pdb_ids)
+        except FileNotFoundError:
+            print(f"The file '{pdb_id_list_path}' does not exist.")
+    else:
+        # get filtered PDB ids from PDB API
+        pdb_ids = (
+            Attr("rcsb_entry_info.selected_polymer_entity_types")
+            .__eq__("Protein (only)")
+            .or_("rcsb_entry_info.polymer_composition")
+            .__eq__("protein/oligosaccharide")
         )
-    pdb_ids = pdb_ids.exec("assembly")
+        # if include_na:
+        #     pdb_ids = pdb_ids.or_('rcsb_entry_info.polymer_composition').in_(["protein/NA", "protein/NA/oligosaccharide"])
+
+        if max_chains is not None:
+            pdb_ids = pdb_ids.and_(
+                "rcsb_assembly_info.polymer_entity_instance_count_protein"
+            ).__le__(max_chains)
+        if resolution_thr is not None:
+            pdb_ids = pdb_ids.and_("rcsb_entry_info.resolution_combined").__le__(
+                resolution_thr
+            )
+        if filter_methods:
+            pdb_ids = pdb_ids.and_("exptl.method").in_(
+                ["X-RAY DIFFRACTION", "ELECTRON MICROSCOPY"]
+            )
+        pdb_ids = pdb_ids.exec("assembly")
 
     ordered_folders = [
         x.key.strip("/")
         for x in _s3list(
             boto3.resource("s3", config=Config(signature_version=UNSIGNED)).Bucket(
                 "pdbsnapshots"
             ),
@@ -191,14 +215,15 @@
     resolution_thr=3.5,
     pdb_snapshot=None,
     filter_methods=True,
     n=None,
     local_folder=".",
     load_live=False,
     max_chains=5,
+    pdb_id_list_path=None,
 ):
     """Download filtered PDB files and return a list of local file paths.
 
     Parameters
     ----------
     resolution_thr : float, default 3.5
         Resolution threshold
@@ -211,28 +236,30 @@
     local_folder : str, default "."
         Folder to save the downloaded files to
     load_live : bool, default False
         Whether to load the PDB files from the RCSB PDB database directly
         instead of downloading them from the PDB snapshots
     max_chains : int, default 5
         Maximum number of chains per biounit
+    pdb_id_list_path : str, default None
+        Path to a file with a list of PDB IDs to download
 
     Returns
     -------
     local_paths : list of str
         List of local file paths
     error_ids : list of str
         List of PDB IDs that could not be downloaded
-
     """
     ordered_folders, pdb_ids = get_pdb_ids(
         resolution_thr=resolution_thr,
         pdb_snapshot=pdb_snapshot,
         filter_methods=filter_methods,
         max_chains=max_chains,
+        pdb_id_list_path=pdb_id_list_path,
     )
     with ThreadPoolExecutor(max_workers=8) as executor:
         print("Getting a file list...")
         ids = []
         for i, x in enumerate(tqdm(pdb_ids)):
             ids.append(x)
             if n is not None and i == n:
@@ -538,14 +565,15 @@
     n=None,
     local_folder=".",
     load_live=False,
     sabdab=False,
     sabdab_data_path=None,
     require_antigen=False,
     max_chains=5,
+    pdb_id_list_path=None,
 ):
     """Download filtered structure files and return a list of local file paths."""
     if sabdab:
         paths, error_ids = download_filtered_sabdab_files(
             resolution_thr=resolution_thr,
             filter_methods=filter_methods,
             pdb_snapshot=pdb_snapshot,
@@ -559,14 +587,15 @@
             resolution_thr=resolution_thr,
             filter_methods=filter_methods,
             pdb_snapshot=pdb_snapshot,
             local_folder=local_folder,
             load_live=load_live,
             n=n,
             max_chains=max_chains,
+            pdb_id_list_path=pdb_id_list_path,
         )
     paths = [(x, _get_fasta_path(x)) for x in paths]
     return paths, error_ids
 
 
 def _make_sabdab_html(method, resolution_thr):
     """Make a URL for SAbDab search."""
@@ -606,7 +635,111 @@
 
     print("Downloading dictionaries for splitting the dataset...")
     _download_dataset_dicts_from_s3(dict_folder, s3_dict_path)
     print("Done!")
 
     _download_dataset_from_s3(dataset_path=data_folder, s3_path=s3_data_path)
     return data_folder
+
+
+def _create_jobs(file_path, strings, results):
+    """Create jobs for parallel processing."""
+    # Perform your job creation logic here
+    jobs = []
+    for string in strings:
+        for i in range(results[string]):
+            jobs.append((file_path, string, i))
+    return jobs
+
+
+def _process_strings(strings):
+    """Process strings in parallel."""
+    results = {}
+    processed_results = Parallel(n_jobs=-1)(
+        delayed(_get_number_of_chains)(string) for string in strings
+    )
+
+    for string, result in zip(strings, processed_results):
+        results[string] = result
+
+    return results
+
+
+def _write_string_to_file(file_path, string, i):
+    """Write a string to a file."""
+    with open(file_path, "a") as file:
+        file.write(string.upper() + "-" + str(i + 1) + "\n")
+
+
+def _parallel_write_to_file(file_path, jobs):
+    """Write a list of strings to a file in parallel."""
+    # Create a multiprocessing Pool with the desired number of processes
+    pool = multiprocessing.Pool(processes=multiprocessing.cpu_count())
+
+    # Map the write_string_to_file function to each string in the list
+    pool.starmap(_write_string_to_file, jobs)
+
+    # Close the pool and wait for all processes to complete
+    pool.close()
+    pool.join()
+
+    print(f"The list has been written to the file '{file_path}' successfully.")
+
+
+def _write_list_to_file(file_path, string_list):
+    """Write a list of strings to a file."""
+    try:
+        with open(file_path, "w") as file:
+            # Write each string in the list to the file
+            for string in string_list:
+                file.write(string + "\n")  # Add a newline character after each string
+
+        print(f"The list has been written to the file '{file_path}' successfully.")
+
+    except OSError:
+        print(f"An error occurred while writing to the file '{file_path}'.")
+
+
+def _get_number_of_chains(pdb_id):
+    """Return the number of chains in a PDB file."""
+    api_url = f"https://data.rcsb.org/rest/v1/core/entry/{pdb_id}"
+
+    try:
+        response = requests.get(api_url)
+        response.raise_for_status()
+        data = response.json()
+
+        # Extracting chain IDs
+        chains = set()
+        if "rcsb_entry_container_identifiers" in data:
+            entity_container_identifiers = data["rcsb_entry_container_identifiers"]
+            if "assembly_ids" in entity_container_identifiers:
+                return len(entity_container_identifiers["assembly_ids"])
+
+        num_chains = len(chains)
+
+        return num_chains
+
+    except requests.exceptions.RequestException as e:
+        print(f"An error occurred: {e}")
+        return 0
+
+
+def _get_chain_pdb_ids(pdb_id_list_path, tmp_folder):
+    print("Generating chain pdb ids")
+    pdb_ids = []
+    with open(pdb_id_list_path) as file:
+        # Read lines from the file
+        lines = file.readlines()
+
+        # Process each line
+        for line in lines:
+            # Extract elements from the line (example: splitting by whitespace)
+            line_elements = line.split()
+
+            # Add extracted elements to the list
+            pdb_ids.extend(line_elements)
+    results = _process_strings(pdb_ids)
+    new_file_path = tmp_folder + "chain_id_" + pdb_id_list_path.split("/")[-1]
+    jobs = _create_jobs(new_file_path, pdb_ids, results)
+    _parallel_write_to_file(new_file_path, jobs)
+    return new_file_path
```

### Comparing `proteinflow-2.0.0/proteinflow/download/boto.py` & `proteinflow-2.1.0/proteinflow/download/boto.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.0.0/proteinflow/logging/__init__.py` & `proteinflow-2.1.0/proteinflow/logging/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     else:
         pdb_id = pdb_id + "-" + chain_id
     if isinstance(exception, PDBError):
         with open(log_file, "a") as f:
             f.write(f"<<< {str(exception)}: {pdb_id} \n")
     else:
         with open(log_file, "a") as f:
-            f.write(f"<<< Unknown: {pdb_id} \n")
+            f.write(f"<<< Unknown: {pdb_id} {exception}\n")
             f.write(traceback.format_exc())
             f.write("\n")
 
 
 def _log_removed(removed, log_file):
     """Record which files we removed due to redundancy."""
     for pdb_id in removed:
```

### Comparing `proteinflow-2.0.0/proteinflow/metrics/__init__.py` & `proteinflow-2.1.0/proteinflow/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.0.0/proteinflow/processing/__init__.py` & `proteinflow-2.1.0/proteinflow/processing/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 """Functions for processing PDB files and generating new datasets."""
+import multiprocessing
 import os
 import pickle
 import subprocess
 from collections import Counter
 from datetime import datetime
 
 import editdistance
 import numpy as np
+import requests
+from joblib import Parallel, delayed
 from p_tqdm import p_map
 from tqdm import tqdm
 
 from proteinflow.data import PDBEntry, SAbDabEntry
 from proteinflow.data.utils import PDBError
 from proteinflow.download import _load_files
+from proteinflow.ligand import _compare_smiles
 from proteinflow.logging import _log_exception, _log_removed, get_error_summary
 
 
 def run_processing(
     tmp_folder="./data/tmp_pdb",
     output_folder="./data/pdb",
     min_length=30,
@@ -32,14 +36,16 @@
     tag=None,
     pdb_snapshot=None,
     load_live=False,
     sabdab=False,
     sabdab_data_path=None,
     require_antigen=False,
     max_chains=5,
+    pdb_id_list_path=None,
+    load_ligands=False,
 ):
     """Download and parse PDB files that meet filtering criteria.
 
     The output files are pickled nested dictionaries where first-level keys are chain Ids and second-level keys are
     the following:
 
     - `'crd_bb'`: a `numpy` array of shape `(L, 4, 3)` with backbone atom coordinates (N, C, CA, O),
@@ -90,14 +96,18 @@
         if `True`, download the SAbDab database instead of PDB
     sabdab_data_path : str, optional
         path to a zip file or a directory containing SAbDab files (only used if `sabdab` is `True`)
     require_antigen : bool, default False
         if `True`, only keep files with antigen chains (only used if `sabdab` is `True`)
     max_chains : int, default 5
         the maximum number of chains per biounit
+    pdb_id_list_path : str, default None
+        if provided, get pdb_ids from list (format pdb_id-num example: 1XYZ-1)
+    load_ligands: boool, default False
+        Whether or not to load the ligands in the pdbs
 
     Returns
     -------
     log : dict
         a dictionary where keys are recognized error names and values are lists of PDB ids that caused the errors
 
     """
@@ -142,14 +152,15 @@
         f.write("\n")
 
     def process_f(
         local_paths,
         show_error=False,
         force=True,
         sabdab=False,
+        ligand=False,
     ):
         pdb_path, fasta_path = local_paths
         chain_id = None
         if sabdab:
             pdb_path, chain_id = pdb_path
             heavy, light, antigen = chain_id.split("_")
             if heavy == "nan":
@@ -181,22 +192,25 @@
                     pdb_path=pdb_path,
                     heavy_chain=heavy,
                     light_chain=light,
                     antigen_chains=antigen,
                     fasta_path=fasta_path,
                 )
             else:
-                pdb_entry = PDBEntry(pdb_path=pdb_path, fasta_path=fasta_path)
+                pdb_entry = PDBEntry(
+                    pdb_path=pdb_path, fasta_path=fasta_path, load_ligand=ligand
+                )
             # filter and convert
             protein_dict = filter_and_convert(
                 pdb_entry,
                 min_length=MIN_LENGTH,
                 max_length=MAX_LENGTH,
                 max_missing_ends=MISSING_ENDS_THR,
                 max_missing_middle=MISSING_MIDDLE_THR,
+                load_ligands=ligand,
             )
             # save
             with open(target_file, "wb") as f:
                 pickle.dump(protein_dict, f)
         except Exception as e:
             if show_error:
                 raise e
@@ -211,21 +225,25 @@
             n=n,
             local_folder=TMP_FOLDER,
             load_live=load_live,
             sabdab=sabdab,
             sabdab_data_path=sabdab_data_path,
             require_antigen=require_antigen,
             max_chains=max_chains,
+            pdb_id_list_path=pdb_id_list_path,
         )
         for id in error_ids:
             with open(LOG_FILE, "a") as f:
                 f.write(f"<<< Could not download PDB/mmCIF file: {id} \n")
         # paths = [("data/2c2m-1.pdb.gz", "data/2c2m.fasta")]
         print("Filter and process...")
-        _ = p_map(lambda x: process_f(x, force=force, sabdab=sabdab), paths)
+        _ = p_map(
+            lambda x: process_f(x, force=force, sabdab=sabdab, ligand=load_ligands),
+            paths,
+        )
         # _ = [
         #     process_f(x, force=force, sabdab=sabdab, show_error=True)
         #     for x in tqdm(paths)
         # ]
     except Exception as e:
         _raise_rcsbsearch(e)
 
@@ -258,27 +276,30 @@
         with open(f"{LOG_FILE}_tmp", "a") as f:
             for line in lines:
                 f.write(line)
         os.rename(f"{LOG_FILE}_tmp", LOG_FILE)
 
     if remove_redundancies:
         removed = _remove_database_redundancies(
-            OUTPUT_FOLDER, seq_identity_threshold=redundancy_thr
+            OUTPUT_FOLDER,
+            seq_identity_threshold=redundancy_thr,
+            ligand_identity=load_ligands,
         )
         _log_removed(removed, LOG_FILE)
 
     return get_error_summary(LOG_FILE)
 
 
 def filter_and_convert(
     pdb_entry,
     min_length=50,
     max_length=150,
     max_missing_ends=5,
     max_missing_middle=5,
+    load_ligands: bool = False,
 ):
     """Filter and convert a PDBEntry to a ProteinEntry.
 
     Parameters
     ----------
     pdb_entry : PDBEntry
         PDBEntry to be converted
@@ -286,23 +307,29 @@
         Minimum total length of the protein sequence
     max_length : int, default 150
         Maximum total length of the protein sequence
     missing_ends_thr : float, default 0.3
         The maximum fraction of missing residues at the ends
     missing_middle_thr : float, default 0.1
         The maximum fraction of missing residues in the middle (after missing ends are disregarded)
+    load_ligands: boool, default False
+        Whether or not to load the ligands in the pdbs
 
     Returns
     -------
     ProteinEntry
         The converted ProteinEntry
 
     """
     pdb_dict = {}
     fasta_dict = pdb_entry.get_fasta()
+    loaded_ligands = False
+    if load_ligands and pdb_entry.get_ligands() is not None:
+        ligand_dict = pdb_entry.get_ligands()
+        loaded_ligands = True
 
     if len(pdb_entry.get_chains()) == 0:
         raise PDBError("No chains found")
 
     if pdb_entry.has_unnatural_amino_acids():
         raise PDBError("Unnatural amino acids found")
 
@@ -335,22 +362,27 @@
 
         # go over rows of coordinates
         crd_arr = pdb_entry.get_coordinates_array(chain)
 
         pdb_dict[chain]["crd_bb"] = crd_arr[:, :4, :]
         pdb_dict[chain]["crd_sc"] = crd_arr[:, 4:, :]
         pdb_dict[chain]["msk"][(pdb_dict[chain]["crd_bb"] == 0).sum(-1).sum(-1) > 0] = 0
+        if loaded_ligands:
+            if chain in ligand_dict.keys():
+                pdb_dict[chain]["ligand"] = ligand_dict[chain]
         if (pdb_dict[chain]["msk"][start:end] == 0).sum() > max_missing_middle * (
             end - start
         ):
             raise PDBError("Too many missing values in the middle")
     return pdb_dict
 
 
-def _remove_database_redundancies(dir, seq_identity_threshold=0.9):
+def _remove_database_redundancies(
+    dir, seq_identity_threshold=0.9, ligand_identity=False
+):
     """Remove all biounits in the database that are copies to another biounits in terms of sequence.
 
     Sequence identity is defined by the 'seq_identity_threshold' parameter for robust detection of sequence similarity (missing residues, point mutations, ...).
 
     Parameters
     ----------
     dir : str
@@ -371,43 +403,65 @@
     total_removed = []
 
     for pdb in tqdm(pdbs_to_check):
         biounits_list = np.array(
             [os.path.join(dir, file) for file in all_files[all_pdbs == pdb]]
         )
         biounits_list = sorted(biounits_list)
-        redundancies = _check_biounits(biounits_list, seq_identity_threshold)
+        redundancies = _check_biounits(
+            biounits_list, seq_identity_threshold, ligand_identity
+        )
         if redundancies != []:
             for k in redundancies:
                 total_removed.append(os.path.basename(biounits_list[k]).split(".")[0])
                 subprocess.run(["rm", biounits_list[k]])
 
     return total_removed
 
 
 def _open_pdb(file):
     """Open a PDB file in the pickle format that follows the dwnloading and processing of the database."""
     with open(file, "rb") as f:
         return pickle.load(f)
 
 
-def _check_biounits(biounits_list, threshold):
+def _check_biounits(biounits_list, threshold, ligand_identity):
     """Return the indexes of the redundant biounits within the list of files given by `biounits_list`."""
     biounits = [_open_pdb(b) for b in biounits_list]
     indexes = []
 
     for k, b1 in enumerate(biounits):
         if k not in indexes:
             b1_seqs = [b1[chain]["seq"] for chain in b1.keys()]
             for i, b2 in enumerate(biounits[k + 1 :]):
                 if len(b1.keys()) != len(b2.keys()):
                     continue
 
                 b2_seqs = [b2[chain]["seq"] for chain in b2.keys()]
-                if _compare_seqs(b1_seqs, b2_seqs, threshold):
+                if ligand_identity:
+                    ligs1 = []
+                    for chain in b1.keys():
+                        if "ligand" in b1[chain].keys():
+                            ligs1.append(
+                                ".".join(
+                                    list([c["smiles"] for c in b1[chain]["ligand"]])
+                                )
+                            )
+                    ligs2 = []
+                    for chain in b2.keys():
+                        if "ligand" in b2[chain].keys():
+                            ligs2.append(
+                                ".".join(
+                                    list([c["smiles"] for c in b2[chain]["ligand"]])
+                                )
+                            )
+                    equal_ligands = _compare_smiles(ligs1, ligs2, threshold)
+                else:
+                    equal_ligands = True
+                if _compare_seqs(b1_seqs, b2_seqs, threshold) and equal_ligands:
                     indexes.append(k + i + 1)
 
     return indexes
 
 
 def _compare_identity(seq, seqs, threshold):
     """Assess whether a sequence is in a list of sequences (in the sense that it shares at least 90% to one of the sequences in the list)."""
```

### Comparing `proteinflow-2.0.0/proteinflow/split/__init__.py` & `proteinflow-2.1.0/proteinflow/split/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-"""Functions used to split the dataset into train, validation and test sets."""
+"""
+Performs clustering of data and partitioning of the clusters into (train, validation ,test).
+
+By default, it clusters chains based on sequence similarity using mmseqs2. But Tanimoto clustering, or a custom partitioning is supported.
+"""
 
 import os
 import pickle
 import random as rd
 import shutil
 import subprocess
 import urllib
@@ -11,32 +15,37 @@
 
 import editdistance
 import networkx as nx
 import numpy as np
 from tqdm import tqdm
 
 from proteinflow.data import PDBEntry
+from proteinflow.ligand import (
+    _load_smiles,
+    _merge_chains_ligands,
+    _run_tanimoto_clustering,
+)
 from proteinflow.split.utils import (
     _biounits_in_clusters_dict,
     _create_pdb_seqs_dict,
     _exclude,
     _find_correspondences,
     _load_pdbs,
     _merge_chains,
     _retrieve_seqs_names_list,
     _test_availability,
     _write_fasta,
 )
 
 
 def _run_mmseqs2(fasta_file, tmp_folder, min_seq_id, cdr=None):
-    """Run the MMSeqs2 command with the parameters we want.
+    """
+    Run the MMSeqs2 command with the parameters we want.
 
     Results are stored in the tmp_folder/MMSeqs2 directory.
-
     """
     folder = "MMSeqs2_results" if cdr is None else os.path.join("MMSeqs2_results", cdr)
     os.makedirs(os.path.join(tmp_folder, folder), exist_ok=True)
     method = "easy-linclust" if cdr is not None else "easy-cluster"
     args = [
         "mmseqs",
         method,
@@ -59,18 +68,18 @@
             "--mask",
             "0",
         ]
     subprocess.run(args)
 
 
 def _read_clusters(tmp_folder, cdr=None):
-    """Read the output from MMSeqs2 and produces 2 dictionaries that store the clusters information.
+    """
+    Read the output from MMSeqs2 and produces 2 dictionaries that store the clusters information.
 
     In cluster_dict, values are the full names (pdb + chains) whereas in cluster_pdb_dict, values are just the PDB ids (so less clusters but bigger).
-
     """
     if cdr is None:
         cluster_file_fasta = os.path.join(
             tmp_folder, "MMSeqs2_results", "clusterRes_all_seqs.fasta"
         )
     else:
         cluster_file_fasta = os.path.join(
@@ -101,18 +110,18 @@
         for k in cluster_pdb_dict.keys():
             cluster_pdb_dict[k] = np.unique(cluster_pdb_dict[k])
 
     return cluster_dict, cluster_pdb_dict
 
 
 def _make_graph(cluster_pdb_dict):
-    """Produce a graph that relates clusters together.
+    """
+    Produce a graph that relates clusters together.
 
     Connections represent a PDB shared by 2 clusters. The more shared PDBs, the stronger the connection.
-
     """
     keys = list(cluster_pdb_dict.keys())
     keys_mapping = {length: k for length, k in enumerate(keys)}
     adjacency_matrix = np.zeros((len(keys), len(keys)))
 
     seen_dict = defaultdict(set)
     for i, key in enumerate(keys):
@@ -182,18 +191,18 @@
 
     return single_chains, homomers, heteromers
 
 
 def _find_chains_in_graph(
     graph, clusters_dict, biounit_chains_array, pdbs_array, chains_array
 ):
-    """Find all the biounit chains present in a given graph or subgraph.
+    """
+    Find all the biounit chains present in a given graph or subgraph.
 
     Return a dictionary for which each key is a cluster name (merged chains name) and the values are all the biounit chains contained in this cluster.
-
     """
     res_dict = {}
     for k, node in enumerate(graph):
         grouped_chains = clusters_dict[node]
         split_chains = np.concatenate(
             [
                 [(pdb[:4], chain) for chain in pdb[5:].split("-")]
@@ -216,15 +225,14 @@
 
 def _find_repartition(chains_dict, homomers, heteromers):
     """
     Return a dictionary similar to the one created by find_chains_in_graph, with an additional level of classification for single chains, homomers and heteromers.
 
     Dictionary structure : `{'single_chains' : {cluster_name : [biounit chains]}, 'homomers' : {cluster_name : [biounit chains]}, 'heteromers' : {cluster_name : [biounit chains]}}`.
     Additionally return the number of chains in each class (single chains, ...).
-
     """
     classes_dict = {
         "single_chains": defaultdict(lambda: []),
         "homomers": defaultdict(lambda: []),
         "heteromers": defaultdict(lambda: []),
     }
     n_single_chains, n_homomers, n_heteromers = 0, 0, 0
@@ -260,20 +268,20 @@
     clusters_dict,
     biounit_chains_array,
     pdbs_array,
     chains_array,
     homomers,
     heteromers,
 ):
-    """Given a list of subgraphs, return a list of dictionaries and an array of sizes of the same length.
-
-    Dictionaries are the `chains_dict` and `classes_dict` corresponding to each subgraph, returned by the `find_chains_in_graph`
-    and `find_repartition` functions respectively. The array of sizes is of shape (len(subgraph), 3). It gives the number of single chains,
-    homomers and heteromers present in each subgraph.
+    """
+    Given a list of subgraphs, return a list of dictionaries and an array of sizes of the same length.
 
+    Dictionaries are the `chains_dict` and `classes_dict` corresponding to each subgraph, returned by the `find_chains_in_graph`.
+    and `find_repartition` functions respectively. The array of sizes is of shape (len(subgraph), 3).
+    It gives the number of single chains, homomers and heteromers present in each subgraph.
     """
     size_array = np.zeros((len(subgraphs), 3))
     dict_list = []
     for k, subgraph in tqdm(enumerate(subgraphs)):
         chains_dict = _find_chains_in_graph(
             subgraph, clusters_dict, biounit_chains_array, pdbs_array, chains_array
         )
@@ -289,20 +297,20 @@
         int(np.sum(size_array[:, 0])),
         int(np.sum(size_array[:, 1])),
         int(np.sum(size_array[:, 2])),
     )
 
 
 def _construct_dataset(dict_list, size_array, indices):
-    """Get a supergraph containing all subgraphs indicated by `indices`.
+    """
+    Get a supergraph containing all subgraphs indicated by `indices`.
 
-    Given the `dict_list` and `size_array` returned by `find_subgraphs_info`, return the 2 dictionaries (`chains_dict` and `classes_dict`)
+    Given the `dict_list` and `size_array` returned by `find_subgraphs_info`, return the 2 dictionaries (`chains_dict` and `classes_dict`).
     corresponding to the graph encompassing all the subgraphs indicated by indices.
     Additionally return the number of single chains, homomers and heteromers in this supergraph.
-
     """
     dataset_clusters_dict = {}
     dataset_classes_dict = {"single_chains": {}, "homomers": {}, "heteromers": {}}
     single_chains_size, homomers_size, heteromers_size = 0, 0, 0
     for k in indices:
         chains_dict, classes_dict = dict_list[k]
         n_single_chains, n_homomers, n_heteromers = size_array[k]
@@ -328,18 +336,18 @@
     remaining_indices,
     chain_class,
     size_obj,
     current_sizes,
     size_array,
     tolerance=0.2,
 ):
-    """Remove values from indices until we get the required (`size_obj`) number of chains in the class of interest (`chain_class`).
+    """
+    Remove values from indices until we get the required (`size_obj`) number of chains in the class of interest (`chain_class`).
 
     Parameter `chain_class` corresponds to the single chain (0), homomer (1) or heteromer (2) class.
-
     """
     sizes = [s[chain_class] for s in size_array[indices]]
     sorted_sizes_indices = np.argsort(sizes)[::-1]
 
     while current_sizes[chain_class] > size_obj and len(sorted_sizes_indices) > 0:
         if (
             current_sizes[chain_class]
@@ -369,31 +377,33 @@
     devnull = open(os.devnull, "w")
     retval = subprocess.call(
         ["mmseqs", "--help"], stdout=devnull, stderr=subprocess.STDOUT
     )
     devnull.close()
     if retval != 0:
         raise RuntimeError(
-            "Please install the MMseqs2 library following the instructions at https://github.com/soedinglab/MMseqs2 (recommended: conda)"
+            "Please install the MMseqs2 library following the \
+            instructions at https://github.com/soedinglab/MMseqs2\
+            (recommended: conda)"
         )
 
 
 def _add_elements_to_dataset(
     indices,
     remaining_indices,
     chain_class,
     size_obj,
     current_sizes,
     size_array,
     tolerance=0.2,
 ):
-    """Add values to indices until we get the required (`size_obj`) number of chains in the class of interest (`chain_class`).
+    """
+    Add values to indices until we get the required (`size_obj`) number of chains in the class of interest (`chain_class`).
 
     Parameter `chain_class` corresponds to the single chain (0), homomer (1) or heteromer (2) class.
-
     """
     sizes = [s[chain_class] for s in size_array[remaining_indices]]
     sorted_sizes_indices = np.argsort(sizes)[::-1]
 
     while current_sizes[chain_class] < size_obj and len(sorted_sizes_indices) > 0:
         if (
             current_sizes[chain_class]
@@ -432,19 +442,19 @@
     homomers_size,
     heteromers_size,
     sc_available,
     hm_available,
     ht_available,
     tolerance=0.2,
 ):
-    """If required, remove and add values in indices so that the number of chains in each class correspond to the required numbers within a tolerance.
+    """
+    If required, remove and add values in indices so that the number of chains in each class correspond to the required numbers within a tolerance.
 
     First remove and then add (if necessary, for each class separately).
     In the end, we might end up with more chains than desired in the first 2 classes but for a reasonable tolerance (~10-20 %), this should not happen.
-
     """
     if single_chains_size > (1 + tolerance) * n_single_chains and sc_available:
         (
             indices,
             remaining_indices,
             single_chains_size,
             homomers_size,
@@ -565,30 +575,32 @@
     dict_list,
     size_array,
     n_samples,
     n_single_chains,
     n_homomers,
     n_heteromers,
     remaining_indices,
-    n_max_iter=50,
+    n_max_iter=100,
     tolerance=0.2,
 ):
-    """Construct a dataset from subgraphs indicated by `indices`.
+    """
+    Construct a dataset from subgraphs indicated by `indices`.
 
-    Given a list of indices to choose from (`remaining_indices`), choose a list of subgraphs to construct a dataset containing the required number of
+    Given a list of indices to choose from (`remaining_indices`), choose a list of subgraphs to construct a dataset containing the required number of.
     biounits for each class (single chains, ...) within a tolerance.
     Return the same outputs as the construct_dataset function, as long as the list of remaining indices after selection.
-
     """
     single_chains_size, homomers_size, heteromers_size = 0, 0, 0
     sc_available, hm_available, ht_available = _test_availability(
         size_array, n_samples
     )  # rule of thumb to estimate if it is logical to try to fill the dataset with a given class
+
     distribution_satisfied = False
     n_iter = 0
+    best_score = -np.inf
 
     while not distribution_satisfied and n_iter < n_max_iter:
         n_iter += 1
         indices = rd.sample(remaining_indices, n_samples)
         (
             dataset_clusters_dict,
             dataset_classes_dict,
@@ -604,14 +616,46 @@
             )
             and (homomers_size > (1 - tolerance) * n_homomers or not hm_available)
             and (homomers_size < (1 + tolerance) * n_homomers or not hm_available)
             and (heteromers_size > (1 - tolerance) * n_heteromers or not ht_available)
             and (heteromers_size < (1 + tolerance) * n_heteromers or not ht_available)
         )
 
+        distribution_score = (
+            max(
+                (single_chains_size - (1 - tolerance) * n_single_chains)
+                * int(sc_available),
+                ((1 + tolerance) * n_single_chains - single_chains_size)
+                * int(sc_available),
+            )
+            + max(
+                (homomers_size - (1 - tolerance) * n_homomers) * int(hm_available),
+                ((1 + tolerance) * n_homomers - homomers_size) * int(hm_available),
+            )
+            + max(
+                (heteromers_size - (1 - tolerance) * n_heteromers) * int(ht_available),
+                ((1 + tolerance) * n_heteromers - heteromers_size) * int(ht_available),
+            )
+        )
+
+        if distribution_score > best_score:
+            best_score = distribution_score
+            best_indices = indices
+            best_dataset_clusters_dict = dataset_clusters_dict
+            best_dataset_classes_dict = dataset_classes_dict
+            best_single_chains_size = single_chains_size
+            best_homomers_size = homomers_size
+            best_heteromers_size = heteromers_size
+
+    indices = best_indices
+    dataset_clusters_dict = best_dataset_clusters_dict
+    dataset_classes_dict = best_dataset_classes_dict
+    single_chains_size = best_single_chains_size
+    homomers_size = best_homomers_size
+    heteromers_size = best_heteromers_size
     if not distribution_satisfied:
         (
             dataset_clusters_dict,
             dataset_classes_dict,
             single_chains_size,
             homomers_size,
             heteromers_size,
@@ -628,14 +672,38 @@
             homomers_size,
             heteromers_size,
             sc_available,
             hm_available,
             ht_available,
             tolerance=tolerance,
         )
+        distribution_score = (
+            max(
+                (single_chains_size - (1 - tolerance) * n_single_chains)
+                * int(sc_available),
+                ((1 + tolerance) * n_single_chains - single_chains_size)
+                * int(sc_available),
+            )
+            + max(
+                (homomers_size - (1 - tolerance) * n_homomers) * int(hm_available),
+                ((1 + tolerance) * n_homomers - homomers_size) * int(hm_available),
+            )
+            + max(
+                (heteromers_size - (1 - tolerance) * n_heteromers) * int(ht_available),
+                ((1 + tolerance) * n_heteromers - heteromers_size) * int(ht_available),
+            )
+        )
+        if distribution_score < best_score:
+            indices = best_indices
+            dataset_clusters_dict = best_dataset_clusters_dict
+            dataset_classes_dict = best_dataset_classes_dict
+            single_chains_size = best_single_chains_size
+            homomers_size = best_homomers_size
+            heteromers_size = best_heteromers_size
+            remaining_indices = [i for i in remaining_indices if i not in indices]
     else:
         remaining_indices = [i for i in remaining_indices if i not in indices]
 
     print("Number of samplings (fill_dataset):", n_iter)
     return (
         dataset_clusters_dict,
         dataset_classes_dict,
@@ -649,15 +717,19 @@
 def _get_subgraph_files(
     subgraphs,
     clusters_dict,
     pdb_arr,
     chain_arr,
     files_arr,
 ):
-    """Given a list of subgraphs, return a dictionary of the form {cluster: [(filename, chain__cdr)]}."""
+    """
+    Given a list of subgraphs, return a dictionary.
+
+    Of the form {cluster: [(filename, chain__cdr)]}.
+    """
     out = {}  # cluster: [(file, chain__cdr)]
     for subgraph in subgraphs:
         for cluster in subgraph.nodes:
             chains = []
             _, cdr = cluster.split("__")
             for chain in clusters_dict[cluster]:
                 pdb, chain_ids = chain.split("_")
@@ -670,15 +742,19 @@
 
 def _split_subgraphs(
     lengths,
     num_clusters_valid,
     num_clusters_test,
     tolerance,
 ):
-    """Split the list of subgraphs into three sets (train, valid, test) according to the number of biounits in each subgraph."""
+    """
+    Split the list of subgraphs into three sets (train, valid, test).
+
+    According to the number of biounits in each subgraph.
+    """
     for _ in range(50):
         indices = np.random.permutation(np.arange(1, len(lengths)))
         valid_indices = []
         test_indices = []
         train_indices = [0]
         valid_sum = 0
         test_sum = 0
@@ -764,15 +840,14 @@
         see train_classes_dict but for test set
     single_chains : list
         the list of all biounit chains (string names) that are in a single chain state (in their biounit)
     homomers : list
         the list of all biounit chains (string names) that are in a homomeric state (in their biounit)
     heteromers : list
         the list of all biounit chains (string names) that are in a heteromeric state (in their biounit)
-
     """
     sample_cluster = list(clusters_dict.keys())[0]
     sabdab = "__" in sample_cluster
 
     subgraphs = np.array(
         [
             graph.subgraph(c)
@@ -964,29 +1039,33 @@
     dataset_dir,
     tmp_folder,
     valid_split=0.05,
     test_split=0.05,
     tolerance=0.2,
     min_seq_id=0.3,
     sabdab=False,
+    tanimoto_clustering=False,
 ):
-    """Build training, validation and test sets from a curated dataset of biounit, using MMSeqs2 for clustering.
+    """
+    Build training, validation and test sets from a curated dataset of biounit, using MMSeqs2 for clustering.
 
     Parameters
     ----------
     dataset_dir : str
         the path to the dataset
     valid_split : float in [0, 1], default 0.05
         the validation split ratio
     test_split : float in [0, 1], default 0.05
         the test split ratio
     min_seq_id : float in [0, 1], default 0.3
         minimum sequence identity for `mmseqs`
     sabdab : bool, default False
         whether the dataset is the SAbDab dataset or not
+    tanimoto_clustering: bool, default False
+        whether to cluster chains based on Tanimoto Clustering
 
     Output
     ------
     train_clusters_dict : dict
         the dictionary containing all the clusters (keys) and the biounit chains they contain for the training dataset
         structure : {cluster_id : [(biounit_file_name, chain), (..., ...), ...]}
     train_classes_dict : dict
@@ -998,51 +1077,62 @@
         see train_classes_dict but for validation set
     test_clusters_dict : dict
         see train_clusters_dict but for test set
     test_classes_dict : dict
         see train_classes_dict but for test set
 
     """
-    cdrs = ["L1", "L2", "L3", "H1", "H2", "H3"] if sabdab else [None]
-    for cdr in cdrs:
-        if cdr is not None:
-            print(f"Clustering with MMSeqs2 for CDR {cdr}...")
-        else:
-            print("Clustering with MMSeqs2...")
-        # retrieve all sequences and create a merged_seqs_dict
-        merged_seqs_dict = _load_pdbs(
-            dataset_dir, cdr=cdr
-        )  # keys: pdb_id, values: list of chains and sequences
+    if tanimoto_clustering:
+        print("Clustering with Tanimoto Clustering...")
+        smiles_dict = _load_smiles(dataset_dir)
         lengths = []
-        for k, v in merged_seqs_dict.items():
+        for k, v in smiles_dict.items():
             lengths += [len(x[1]) for x in v]
-        merged_seqs_dict = _merge_chains(merged_seqs_dict)  # remove redundant chains
-
-        # write sequences to a fasta file for clustering with MMSeqs2, run MMSeqs2 and delete the fasta file
-        fasta_file = os.path.join(tmp_folder, "all_seqs.fasta")
-        _write_fasta(
-            fasta_file, merged_seqs_dict
-        )  # write all sequences from merged_seqs_dict to fasta file
-        _run_mmseqs2(
-            fasta_file, tmp_folder, min_seq_id, cdr=cdr
-        )  # run MMSeqs2 on fasta file
-        subprocess.run(["rm", fasta_file])
-
-    # retrieve MMSeqs2 clusters and build a graph with these clusters
-    clusters_dict = {}
-    clusters_pdb_dict = {}
-    for cdr in cdrs:
-        c_dict, c_pdb_dict = _read_clusters(
-            tmp_folder=tmp_folder,
-            cdr=cdr,
+        merged_seqs_dict = _merge_chains_ligands(smiles_dict)
+        clusters_dict, clusters_pdb_dict = _run_tanimoto_clustering(
+            merged_seqs_dict, min_seq_id, tmp_folder
         )
-        clusters_dict.update(c_dict)
-        clusters_pdb_dict.update(c_pdb_dict)
-
-    subprocess.run(["rm", "-r", os.path.join(tmp_folder, "MMSeqs2_results")])
+    else:
+        cdrs = ["L1", "L2", "L3", "H1", "H2", "H3"] if sabdab else [None]
+        for cdr in cdrs:
+            if cdr is not None:
+                print(f"Clustering with MMSeqs2 for CDR {cdr}...")
+            else:
+                print("Clustering with MMSeqs2...")
+            # retrieve all sequences and create a merged_seqs_dict
+            merged_seqs_dict = _load_pdbs(
+                dataset_dir, cdr=cdr
+            )  # keys: pdb_id, values: list of chains and sequences
+            lengths = []
+            for k, v in merged_seqs_dict.items():
+                lengths += [len(x[1]) for x in v]
+            merged_seqs_dict = _merge_chains(
+                merged_seqs_dict
+            )  # remove redundant chains
+            # write sequences to a fasta file for clustering with MMSeqs2, run MMSeqs2 and delete the fasta file
+            fasta_file = os.path.join(tmp_folder, "all_seqs.fasta")
+            _write_fasta(
+                fasta_file, merged_seqs_dict
+            )  # write all sequences from merged_seqs_dict to fasta file
+            _run_mmseqs2(
+                fasta_file, tmp_folder, min_seq_id, cdr=cdr
+            )  # run MMSeqs2 on fasta file
+            subprocess.run(["rm", fasta_file])
+
+        # retrieve MMSeqs2 clusters and build a graph with these clusters
+        clusters_dict = {}
+        clusters_pdb_dict = {}
+        for cdr in cdrs:
+            c_dict, c_pdb_dict = _read_clusters(
+                tmp_folder=tmp_folder,
+                cdr=cdr,
+            )
+            clusters_dict.update(c_dict)
+            clusters_pdb_dict.update(c_pdb_dict)
+        subprocess.run(["rm", "-r", os.path.join(tmp_folder, "MMSeqs2_results")])
     graph = _make_graph(clusters_pdb_dict)
 
     # import pickle
 
     # with open("graph.pickle", "wb") as f:
     #     pickle.dump(graph, f)
 
@@ -1079,14 +1169,15 @@
     tmp_folder="./data/tmp_pdb",
     output_folder="./data/pdb",
     split_tolerance=0.2,
     test_split=0.05,
     valid_split=0.05,
     out_split_dict_folder="./data/dataset_splits_dict",
     min_seq_id=0.3,
+    tanimoto_clustering=False,
 ):
     """Split preprocessed data into training, validation and test.
 
     Parameters
     ----------
     tmp_folder : str, default "./data/tmp_pdb"
         The folder where temporary files will be saved
@@ -1122,14 +1213,15 @@
         output_folder,
         tmp_folder,
         valid_split=valid_split,
         test_split=test_split,
         tolerance=split_tolerance,
         min_seq_id=min_seq_id,
         sabdab=sabdab,
+        tanimoto_clustering=tanimoto_clustering,
     )
 
     classes_dict = train_classes_dict
     for d in [valid_classes_dict, test_classes_dict]:
         for k, v in d.items():
             classes_dict[k].update(v)
 
@@ -1289,7 +1381,41 @@
         shutil.move(os.path.join(dataset_path, biounit), train_path)
     print("Moving files in the validation set...")
     for biounit in tqdm(valid_biounits):
         shutil.move(os.path.join(dataset_path, biounit), valid_path)
     print("Moving files in the test set...")
     for biounit in tqdm(test_biounits):
         shutil.move(os.path.join(dataset_path, biounit), test_path)
+
+
+def _exclude_files_with_no_ligand(tag, local_datasets_folder):
+    """Get a list of files to exclude from the dataset.
+
+    Biounits are excluded if they don't contain ligands.
+
+    Parameters
+    ----------
+    tag : str
+        the name of the dataset
+    local_datasets_folder : str
+        the path to the folder that stores proteinflow datasets
+    tmp_folder : str
+        the path to the folder that stores temporary files
+
+    """
+    # iterate over files in the dataset to check ligand
+    exclude_biounits = []
+    for fn in tqdm(
+        os.listdir(os.path.join(local_datasets_folder, f"proteinflow_{tag}"))
+    ):
+        if not fn.endswith(".pickle"):
+            continue
+        fp = os.path.join(local_datasets_folder, f"proteinflow_{tag}", fn)
+        with open(fp, "rb") as f:
+            entry = pickle.load(f)
+        for chain, chain_data in entry.items():
+            if "ligand" not in chain_data.keys():
+                exclude_biounits.append(fn)
+                break
+
+    # return list of biounits to exclude
+    return exclude_biounits
```

### Comparing `proteinflow-2.0.0/proteinflow/split/utils.py` & `proteinflow-2.1.0/proteinflow/split/utils.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.0.0/proteinflow.egg-info/PKG-INFO` & `proteinflow-2.1.0/proteinflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteinflow
-Version: 2.0.0
+Version: 2.1.0
 Summary: Versatile pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
 License: BSD-3-Clause
 Keywords: bioinformatics,dataset,protein,PDB,deep learning
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proteinflow Version: 2.0.0 Summary: Versatile
+Metadata-Version: 2.1 Name: proteinflow Version: 2.1.0 Summary: Versatile
 pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova
 adaptyvbio.com>, Arthur Valentin
 adaptyvbio.com> License: BSD-3-Clause Keywords:
 bioinformatics,dataset,protein,PDB,deep learning Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
   ProteinFlow - A data processing pipeline for all your protein design needs
```

### Comparing `proteinflow-2.0.0/proteinflow.egg-info/SOURCES.txt` & `proteinflow-2.1.0/proteinflow.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 dev/bump_version.py
+dev/update_init_docs.py
 proteinflow/__init__.py
 proteinflow/cli.py
 proteinflow/constants.py
+proteinflow/ligand.py
+proteinflow/visualize.py
 proteinflow.egg-info/PKG-INFO
 proteinflow.egg-info/SOURCES.txt
 proteinflow.egg-info/dependency_links.txt
 proteinflow.egg-info/entry_points.txt
 proteinflow.egg-info/requires.txt
 proteinflow.egg-info/top_level.txt
 proteinflow/data/__init__.py
```

### Comparing `proteinflow-2.0.0/pyproject.toml` & `proteinflow-2.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proteinflow"
-version = "2.0.0"
+version = "2.1.0"
 authors = [
     {name = "Liza Kozlova", email = "liza@adaptyvbio.com"},
     {name = "Arthur Valentin", email = "arthur@adaptyvbio.com"}
 ]
 description = "Versatile pipeline for processing protein structure data for deep learning applications."
 readme = "README.md"
 requires-python = ">=3.8"
@@ -29,15 +29,20 @@
     "aiobotocore==2.4.2",
     "awscli==1.25.60",
     "bs4>=0.0.1",
     "pyyaml==5.3",
     "rcsbsearch",
     "blosum>=2.0",
     "pre-commit",
+    "rdkit",
+    "pypdb",
+    "prody",
+    "joblib",
     "methodtools",
+    "py3Dmol",
 ]
 keywords = ["bioinformatics", "dataset", "protein", "PDB", "deep learning"]
 
 [project.scripts]
 proteinflow = "proteinflow.cli:cli"
 
 [tool.setuptools.packages]
@@ -46,8 +51,8 @@
 [tool.pydocstyle]
 convention = "numpy"
 
 [tool.docsig]
 disable = [
     "E109",
 ]
-ignore-no-parameters = true
+ignore-no-parameters = true
```

### Comparing `proteinflow-2.0.0/tests/test_download.py` & `proteinflow-2.1.0/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.0.0/tests/test_entry.py` & `proteinflow-2.1.0/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.0.0/tests/test_generate.py` & `proteinflow-2.1.0/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.0.0/tests/test_sabdab.py` & `proteinflow-2.1.0/tests/test_sabdab.py`

 * *Files identical despite different names*

