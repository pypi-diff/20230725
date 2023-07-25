# Comparing `tmp/rouskinhf-0.1.4.tar.gz` & `tmp/rouskinhf-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rouskinhf-0.1.4.tar", last modified: Mon Jul 24 19:26:20 2023, max compression
+gzip compressed data, was "rouskinhf-0.2.1.tar", last modified: Tue Jul 25 21:35:11 2023, max compression
```

## Comparing `rouskinhf-0.1.4.tar` & `rouskinhf-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-24 19:26:20.579578 rouskinhf-0.1.4/
--rw-r--r--   0 ymdt       (501) staff       (20)     1141 2023-06-30 22:14:56.000000 rouskinhf-0.1.4/LICENSE
--rw-r--r--   0 ymdt       (501) staff       (20)     6005 2023-07-24 19:26:20.579427 rouskinhf-0.1.4/PKG-INFO
--rw-r--r--   0 ymdt       (501) staff       (20)     5554 2023-07-24 19:06:17.000000 rouskinhf-0.1.4/README.md
--rw-r--r--   0 ymdt       (501) staff       (20)      813 2023-07-24 19:17:23.000000 rouskinhf-0.1.4/pyproject.toml
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-24 19:26:20.578356 rouskinhf-0.1.4/rouskinhf/
--rw-r--r--   0 ymdt       (501) staff       (20)     2697 2023-07-24 18:42:55.000000 rouskinhf-0.1.4/rouskinhf/__init__.py
--rw-r--r--   0 ymdt       (501) staff       (20)    16973 2023-07-24 19:24:00.000000 rouskinhf-0.1.4/rouskinhf/datafolder.py
--rw-r--r--   0 ymdt       (501) staff       (20)     8225 2023-07-24 18:55:17.000000 rouskinhf-0.1.4/rouskinhf/datapoint.py
--rw-r--r--   0 ymdt       (501) staff       (20)      556 2023-07-20 03:42:13.000000 rouskinhf-0.1.4/rouskinhf/env.py
--rw-r--r--   0 ymdt       (501) staff       (20)     3467 2023-07-24 19:25:13.000000 rouskinhf-0.1.4/rouskinhf/info_file.py
--rw-r--r--   0 ymdt       (501) staff       (20)    10871 2023-07-24 18:43:58.000000 rouskinhf-0.1.4/rouskinhf/list_datapoints.py
--rw-r--r--   0 ymdt       (501) staff       (20)     3648 2023-07-24 18:05:45.000000 rouskinhf-0.1.4/rouskinhf/parsers.py
--rw-r--r--   0 ymdt       (501) staff       (20)     2608 2023-07-20 00:54:02.000000 rouskinhf-0.1.4/rouskinhf/path.py
--rw-r--r--   0 ymdt       (501) staff       (20)     6222 2023-07-20 00:54:02.000000 rouskinhf-0.1.4/rouskinhf/rnastructure.py
--rw-r--r--   0 ymdt       (501) staff       (20)     3819 2023-07-24 18:55:31.000000 rouskinhf-0.1.4/rouskinhf/util.py
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-24 19:26:20.579201 rouskinhf-0.1.4/rouskinhf.egg-info/
--rw-r--r--   0 ymdt       (501) staff       (20)     6005 2023-07-24 19:26:20.000000 rouskinhf-0.1.4/rouskinhf.egg-info/PKG-INFO
--rw-r--r--   0 ymdt       (501) staff       (20)      426 2023-07-24 19:26:20.000000 rouskinhf-0.1.4/rouskinhf.egg-info/SOURCES.txt
--rw-r--r--   0 ymdt       (501) staff       (20)        1 2023-07-24 19:26:20.000000 rouskinhf-0.1.4/rouskinhf.egg-info/dependency_links.txt
--rw-r--r--   0 ymdt       (501) staff       (20)      152 2023-07-24 19:26:20.000000 rouskinhf-0.1.4/rouskinhf.egg-info/requires.txt
--rw-r--r--   0 ymdt       (501) staff       (20)       10 2023-07-24 19:26:20.000000 rouskinhf-0.1.4/rouskinhf.egg-info/top_level.txt
--rw-r--r--   0 ymdt       (501) staff       (20)       38 2023-07-24 19:26:20.579628 rouskinhf-0.1.4/setup.cfg
--rw-r--r--   0 ymdt       (501) staff       (20)      468 2023-07-24 18:15:00.000000 rouskinhf-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:35:11.681869 rouskinhf-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-25 21:34:16.000000 rouskinhf-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-25 21:35:11.681869 rouskinhf-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-07-25 21:34:16.000000 rouskinhf-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-25 21:34:16.000000 rouskinhf-0.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:35:11.681869 rouskinhf-0.2.1/rouskinhf/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-25 21:34:16.000000 rouskinhf-0.2.1/rouskinhf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17115 2023-07-25 21:34:16.000000 rouskinhf-0.2.1/rouskinhf/datafolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-07-25 21:34:16.000000 rouskinhf-0.2.1/rouskinhf/datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-25 21:34:16.000000 rouskinhf-0.2.1/rouskinhf/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-25 21:34:16.000000 rouskinhf-0.2.1/rouskinhf/import_dataset_fun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-25 21:34:16.000000 rouskinhf-0.2.1/rouskinhf/info_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-07-25 21:34:16.000000 rouskinhf-0.2.1/rouskinhf/list_datapoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-07-25 21:34:16.000000 rouskinhf-0.2.1/rouskinhf/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-25 21:34:16.000000 rouskinhf-0.2.1/rouskinhf/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-07-25 21:34:16.000000 rouskinhf-0.2.1/rouskinhf/rnastructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-25 21:34:16.000000 rouskinhf-0.2.1/rouskinhf/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:35:11.681869 rouskinhf-0.2.1/rouskinhf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-25 21:35:11.000000 rouskinhf-0.2.1/rouskinhf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-25 21:35:11.000000 rouskinhf-0.2.1/rouskinhf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 21:35:11.000000 rouskinhf-0.2.1/rouskinhf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-25 21:35:11.000000 rouskinhf-0.2.1/rouskinhf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 21:35:11.000000 rouskinhf-0.2.1/rouskinhf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 21:35:11.681869 rouskinhf-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-25 21:34:16.000000 rouskinhf-0.2.1/setup.py
```

### Comparing `rouskinhf-0.1.4/LICENSE` & `rouskinhf-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.1.4/PKG-INFO` & `rouskinhf-0.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: rouskinhf
-Version: 0.1.4
+Version: 0.2.1
 Summary: A library to manipulate data for our DMS prediction models.
 Author-email: Yves Martin <yves@martin.yt>, Alberic de Lajarte <albericlajarte@gmail.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-
+[![Python CI](https://github.com/rouskinlab/rouskinhf/actions/workflows/CI.yml/badge.svg)](https://github.com/rouskinlab/rouskinhf/actions/workflows/CI.yml)
+[![Publish distributions 📦 to PyPI](https://github.com/rouskinlab/rouskinhf/actions/workflows/release.yml/badge.svg)](https://github.com/rouskinlab/rouskinhf/actions/workflows/release.yml)
+![PyPI](https://img.shields.io/pypi/v/rouskinhf)
 
 # Download your RNA data from HuggingFace with rouskinhf!
 
 A repo to manipulate the data for our RNA structure prediction model. This repo allows you to:
 - pull datasets from the Rouskinlab's HuggingFace
 - create datasets from local files and push them to HuggingFace, from the formats:
     - `.fasta`
@@ -23,14 +25,24 @@
     - `.json` (DREEM output format)
     - `.json` (Rouskinlab's huggingface format)
 
 ## Important notes
 
 - Sequences with bases different than `A`, `C`, `G`, `T`, `U`, `N`, `a`, `c`, `g`, `t`, `u`, `n` are not supported. The data will be filtered out.
 
+## Dependencies
+- [RNAstructure](https://rna.urmc.rochester.edu/RNAstructure.html) (also available on [Rouskinlab GitHub](https://github.com/rouskinlab/RNAstructure)).
+
+## Push a new release to Pypi
+
+1. Edit version to `vx.y.z` in `pyproject.toml`. Then run in a terminal `git add . && git commit -m 'vx.y.z' && git push`.
+2. Create and push a git tag `vx.y.z` by running in a terminal `git tag 'vx.y.z' && git push --tag`.
+3. Create a release for the tag `vx.y.z` on Github Release.
+4. Make sure that the Github Action `Publish distributions 📦 to PyPI` passed on Github Actions.
+
 ## Installation
 
 ### Get a HuggingFace token
 
 Go to [HuggingFace](https://huggingface.co/) and create an account. Then go to your profile and copy your token ([huggingface.co/settings/tokens](https://huggingface.co/settings/tokens)).
 
 ### Create an environment file
```

### Comparing `rouskinhf-0.1.4/README.md` & `rouskinhf-0.2.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-
+[![Python CI](https://github.com/rouskinlab/rouskinhf/actions/workflows/CI.yml/badge.svg)](https://github.com/rouskinlab/rouskinhf/actions/workflows/CI.yml)
+[![Publish distributions 📦 to PyPI](https://github.com/rouskinlab/rouskinhf/actions/workflows/release.yml/badge.svg)](https://github.com/rouskinlab/rouskinhf/actions/workflows/release.yml)
+![PyPI](https://img.shields.io/pypi/v/rouskinhf)
 
 # Download your RNA data from HuggingFace with rouskinhf!
 
 A repo to manipulate the data for our RNA structure prediction model. This repo allows you to:
 - pull datasets from the Rouskinlab's HuggingFace
 - create datasets from local files and push them to HuggingFace, from the formats:
     - `.fasta`
@@ -10,14 +12,24 @@
     - `.json` (DREEM output format)
     - `.json` (Rouskinlab's huggingface format)
 
 ## Important notes
 
 - Sequences with bases different than `A`, `C`, `G`, `T`, `U`, `N`, `a`, `c`, `g`, `t`, `u`, `n` are not supported. The data will be filtered out.
 
+## Dependencies
+- [RNAstructure](https://rna.urmc.rochester.edu/RNAstructure.html) (also available on [Rouskinlab GitHub](https://github.com/rouskinlab/RNAstructure)).
+
+## Push a new release to Pypi
+
+1. Edit version to `vx.y.z` in `pyproject.toml`. Then run in a terminal `git add . && git commit -m 'vx.y.z' && git push`.
+2. Create and push a git tag `vx.y.z` by running in a terminal `git tag 'vx.y.z' && git push --tag`.
+3. Create a release for the tag `vx.y.z` on Github Release.
+4. Make sure that the Github Action `Publish distributions 📦 to PyPI` passed on Github Actions.
+
 ## Installation
 
 ### Get a HuggingFace token
 
 Go to [HuggingFace](https://huggingface.co/) and create an account. Then go to your profile and copy your token ([huggingface.co/settings/tokens](https://huggingface.co/settings/tokens)).
 
 ### Create an environment file
```

### Comparing `rouskinhf-0.1.4/pyproject.toml` & `rouskinhf-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 py-modules = ['rouskinhf']
 
 [project]
 name =  "rouskinhf"
-version = "0.1.4"
+version = "0.2.1"
 authors = [
     {name = "Yves Martin", email = "yves@martin.yt"},
     {name = "Alberic de Lajarte", email = "albericlajarte@gmail.com"},
 ]
 description = "A library to manipulate data for our DMS prediction models."
 readme = "README.md"
 classifiers = [
```

### Comparing `rouskinhf-0.1.4/rouskinhf/__init__.py` & `rouskinhf-0.2.1/rouskinhf/import_dataset_fun.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,8 @@
-from .datafolder import DataFolder
-
-from .env import DATA_FOLDER
-import pandas as pd
-from typing import Dict
-import os
 from os.path import exists
-from huggingface_hub import HfApi
 from numpy import ndarray
 import numpy as np
 from .datafolder import DataFolder
 
 def import_dataset(name:str, data:str, force_download:bool=False)->ndarray:
 
     """Finds the dataset with the given name for the given type of data.
@@ -56,14 +49,16 @@
         datafolder = DataFolder.from_local(name=name)
     except:
         try:
             datafolder = DataFolder.from_huggingface(name=name)
         except:
             raise ValueError("Dataset not found on HuggingFace Hub")
 
+    datafolder.generate_npy()
+
     out = {
         'references': np.load(datafolder.get_references_npy(), allow_pickle=True),
         'sequences': np.load(datafolder.get_sequences_npy(), allow_pickle=True)
         }
 
     # Get the dataset
     if data == 'structure':
```

### Comparing `rouskinhf-0.1.4/rouskinhf/datafolder.py` & `rouskinhf-0.2.1/rouskinhf/datafolder.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .list_datapoints import ListofDatapoints
 from .info_file import infoFileWriter
 import os
 import numpy as np
 from huggingface_hub import HfApi
 from huggingface_hub import snapshot_download
 
+
 GENERATE_NPY = False
 PREDICT_STRUCTURE = False
 PREDICT_DMS = False
 ROUSKINLAB = 'rouskinlab/'
 
 class DataFolderTemplate(PathDatafolder):
 
@@ -66,15 +67,15 @@
         self.predict_dms = predict_dms
 
         # move path_in to source folder
         os.makedirs(self.get_source_folder(), exist_ok=True)
         os.system(f'cp -fr {path_in} {self.get_source_folder()}')
 
         # Write info file
-        infoFileWriter(source=source, datafolder=self).write()
+        infoFileWriter(source=source, datafolder=self, predict_dms=predict_dms, predict_structure=predict_dms).write()
 
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__} @{self.get_main_folder()}"
 
     def _set_name(self, name, path_in):
         if name is None:
@@ -171,17 +172,14 @@
             **kwargs
         )
 
         if run_as_future:
             return future
 
 
-
-
-
     def dump_datapoints(self, generate_npy):
         """Dump the datapoints to a json file."""
 
         self.datapoints.to_json(self.get_json())
 
         if generate_npy:
             self.generate_npy()
@@ -224,14 +222,15 @@
     True
     """
 
     def __init__(self, path_in, path_out, name, predict_structure, generate_npy, tqdm=True) -> None:
         super().__init__(path_in, path_out, name, source = 'dreem_output', predict_structure = predict_structure, predict_dms = False)
 
         self.datapoints = ListofDatapoints.from_dreem_output(path_in, predict_structure = predict_structure, tqdm=tqdm)
+        self.datapoints.filter_duplicates()
         self.dump_datapoints(generate_npy)
 
 
 class CreateDatafolderFromFasta(CreateDatafolderTemplate):
 
     """ Create a datafolder from a fasta file.
 
@@ -267,14 +266,15 @@
     True
     """
 
     def __init__(self, path_in, path_out, name, predict_structure, predict_dms, generate_npy, tqdm) -> None:
         super().__init__(path_in, path_out, name, source = 'fasta', predict_structure = predict_structure, predict_dms = predict_dms)
 
         self.datapoints = ListofDatapoints.from_fasta(path_in, predict_structure = predict_structure, predict_dms = predict_dms, tqdm=tqdm)
+        self.datapoints.filter_duplicates()
         self.dump_datapoints(generate_npy)
 
 
 
 class CreateDatafolderFromCTfolder(CreateDatafolderTemplate):
 
     """ Create a datafolder from a folder of ct files.
```

### Comparing `rouskinhf-0.1.4/rouskinhf/datapoint.py` & `rouskinhf-0.2.1/rouskinhf/datapoint.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 
 from typing import Any, List
 from .parsers import *
 from .util import add_braces_if_no_braces, dot2int, int2dot, seq2int, standardize_sequence, sequence_has_regular_characters
 import numpy as np
+from .rnastructure import RNAstructure_singleton
 
 class Datapoint:
 
     """A datapoint is a data structure where:
     - reference is the name of the sequence in the fasta file
     - sequence is a string of A, C, G, U
     - structure is a string of (, ), .
@@ -17,24 +18,28 @@
     Example:
     >>> datapoint = Datapoint(reference='reference', sequence='AACCGG', structure='((..))', dms=[1.0, 2.0, 3.0])
     >>> print(datapoint)
     "reference":{"sequence": "AACCGG", "paired_bases": [[1, 4], [0, 5]], "dms": [1.0, 2.0, 3.0]}
     >>> datapoint = Datapoint(reference='reference', sequence='not a valid sequence', structure='((..))')
     >>> print(datapoint)
     None
+    >>> datapoint = Datapoint(reference='reference', sequence='NNNNNNN', structure='((..))')
+    >>> print(datapoint)
+    None
     """
 
     def __new__(cls, *args, **kwargs):
         # Check if the conditions are met before creating the object
         sequence = kwargs.get('sequence', args[0] if len(args) > 0 else None)
-        if sequence is None:
-            raise ValueError("Object creation aborted: sequence is None.")
+        reference = kwargs.get('reference', args[1] if len(args) > 1 else None)
+        if sequence is None or reference is None:
+            return None
         sequence = standardize_sequence(sequence)
 
-        if not sequence_has_regular_characters(sequence):
+        if not sequence_has_regular_characters(sequence) or len(sequence) == 0 or len(reference) == 0:
             return None
 
         # If conditions are met, create and return the new instance
         instance = super().__new__(cls)
         return instance
 
     def __init__(self, sequence, reference, structure=None, dms=None, paired_bases=None):
@@ -80,47 +85,38 @@
         return paired_bases
 
     def embed_sequence(self):
         """Returns a list of integers corresponding to the sequence.
 
         >>> datapoint = Datapoint(reference='reference', sequence='AACCGG', structure='((..))', dms=[1.0, 2.0, 3.0])
         >>> datapoint.embed_sequence()
-        array([1, 1, 2, 2, 3, 3])
+        array([0, 0, 1, 1, 2, 2])
         """
         return np.array([seq2int[base] for base in self.sequence])
 
     def embed_structure(self):
         """Returns a list of integers corresponding to the structure.
 
+        >>> from numpy import array
         >>> datapoint = Datapoint(reference='reference', sequence='AACCGG', structure='((..))', dms=[1.0, 2.0, 3.0])
-        >>> datapoint.embed_structure()
-        array([2, 2, 1, 1, 3, 3])
+        >>> assert not (datapoint.embed_structure() - array([2, 2, 1, 1, 3, 3])).any(), 'The sequence is not embedded correctly.'
         """
         return np.array([dot2int[base] for base in self.structure])
 
 
 
 class DatapointFactory:
     """A datapoint is a tuple (sequence, reference, structure, dms) where:
 
     - reference is the name of the sequence in the fasta file
     - sequence is a string of A, C, G, U
     - structure is a string of (, ), .
     - dms is a list of floats corresponding to the reactivity of each base in the sequence
 
     """
-
-    def __call__(sequence, reference, structure=None, dms=None, predict_structure=False, predict_dms=False):
-        sequence = standardize_sequence(sequence)
-
-        if sequence_has_regular_characters(sequence):
-            if structure is None and predict_structure:
-                structure = Fasta.predict_structure(sequence)
-            return Datapoint(sequence, reference, structure, dms)
-
     def from_ct(ct_file, predict_dms):
         """Create a datapoint from a ct file. If predict_dms is True, the dms will be predicted using RNAstructure"""
         reference, sequence, paired_bases = Ct.parse(ct_file)
         sequence = standardize_sequence(sequence)
 
         if sequence_has_regular_characters(sequence):
             return Datapoint(sequence, reference, paired_bases=paired_bases, dms = Ct.predict_dms(ct_file) if predict_dms else None)
@@ -141,15 +137,15 @@
         """Create a datapoint from a dreem output file. The structure and dms will be predicted if predict_structure and predict_dms are True."""
         sequence = standardize_sequence(sequence)
 
         if sequence_has_regular_characters(sequence):
             return Datapoint(
                 sequence=sequence,
                 reference=reference,
-                structure=Fasta.predict_structure(sequence) if predict_structure else None,
+                structure=RNAstructure_singleton.predictStructure(sequence, dms=mutation_rate) if predict_structure else None,
                 dms=mutation_rate)
         print('DatapointFactory.from_dreem_output: sequence is not valid "{}"'.format(set(sequence) - set('ACGTUacgtu')))
 
 
     def from_json_line(string):
         """Create a datapoint from a json line. The json line should have the following format:
         "reference": {"sequence": "sequence", "paired_bases": [[1, 2], [3,4]], "dms": [1.0, 2.0, 3.0]}
```

### Comparing `rouskinhf-0.1.4/rouskinhf/env.py` & `rouskinhf-0.2.1/rouskinhf/env.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.1.4/rouskinhf/info_file.py` & `rouskinhf-0.2.1/rouskinhf/info_file.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 STRUCTURE_FROM_RNASTRUCTURE = 'RNAstructure'
 STRUCTURE_FROM_SOURCE = 'source'
 DMS_FROM_RNASTRUCTURE = 'RNAstructure'
 DMS_FROM_SOURCE = 'source'
 
 class InfoFileWriterTemplate(PathDatafolder):
 
-    def __init__(self, name, root) -> None:
+    def __init__(self, name, root, has_dms, has_structure) -> None:
         super().__init__(name, root)
+        self.has_dms = has_dms
+        self.has_structure = has_structure
 
         self.info = {
             'name': self.name,
             'upload_date': datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
             'user': os.environ['USER'],
         }
 
@@ -27,42 +29,36 @@
             f.write(f"""
 ---
 license: mit
 language:
   - en
 tags:
   - chemistry
-  - biology
+  - biology`
 author: Silvi Rouskin
 pretty_name: {self.name}
 ---
 
 """)
-
+            f.write(f"# {self.name}\n")
             for k, v in self.info.items():
-                if k not in ['structure', 'about structure', 'DMS', 'about DMS']:
-                    f.write(f"{k}: {v}\n\n")
-            f.write(f"""
-
-structure: {self.info['structure']} ({self.info['about structure']})
-
-DMS: {self.info['DMS']} ({self.info['about DMS']})
-
-"""
-
-
-
-)
+                if k not in ['structure', 'about structure', 'DMS', 'about DMS','name']:
+                    f.write(f"\t{k}: {v}\n")
+            f.write(f"\tData types:")
+            if self.has_structure:
+                f.write(f"\n\t- structure ({self.info['about structure']})")
+            if self.has_dms:
+                f.write(f"\n\t- DMS ({self.info['about DMS']})")
 
 
 
 class InfoFileWriterFromDREEMoutput(InfoFileWriterTemplate):
 
-    def __init__(self, name, root, path_in) -> None:
-        super().__init__(name, root)
+    def __init__(self, name, root, path_in, predict_dms, predict_structure) -> None:
+        super().__init__(name, root, has_dms=True, has_structure=predict_structure)
 
         file = json.load(open(path_in, 'r'))
         if 'user' in file:
             file['experimenter'] = file.pop('user')
         for k, v in file.items():
             if type(v) != dict:
                 self.info[k] = v
@@ -72,38 +68,39 @@
         self.info['about structure'] = 'Predicted using RNAstructure and the DMS reactivity data.'
         self.info['DMS'] = DMS_FROM_SOURCE
         self.info['about DMS'] = 'Measured experimentally using the attached experimental conditions.'
 
 
 class InfoFileWriterFromCT(InfoFileWriterTemplate):
 
-    def __init__(self, name, root, path_in) -> None:
-        super().__init__(name, root)
+    def __init__(self, name, root, path_in, predict_dms, predict_structure) -> None:
+        super().__init__(name, root, has_dms=predict_dms, has_structure=True)
 
         self.info['source'] = "`{}` (CT files format)".format(os.path.basename(path_in))
         self.info['structure'] = STRUCTURE_FROM_SOURCE
         self.info['about structure'] = 'Read from source.'
         self.info['DMS'] = DMS_FROM_RNASTRUCTURE
         self.info['about DMS'] = 'Predicted using RNAstructure at 310K.'
 
 
 class InfoFileWriterFromFasta(InfoFileWriterTemplate):
 
-    def __init__(self, name, root, path_in) -> None:
-        super().__init__(name, root)
+    def __init__(self, name, root, path_in, predict_dms, predict_structure) -> None:
+        super().__init__(name, root, has_dms=predict_dms, has_structure=predict_structure)
 
         self.info['source'] = "`{}` (fasta file format)".format(os.path.basename(path_in))
         self.info['structure'] = STRUCTURE_FROM_RNASTRUCTURE
         self.info['about structure'] = 'Predicted using RNAstructure at 310K.'
         self.info['DMS'] = DMS_FROM_RNASTRUCTURE
         self.info['about DMS'] = 'Predicted using RNAstructure at 310K.'
 
 
-def infoFileWriter(source, datafolder):
+def infoFileWriter(source, datafolder, predict_dms, predict_structure):
+
     if source == 'dreem_output':
-        return InfoFileWriterFromDREEMoutput(datafolder.name, datafolder.path_out, datafolder.path_in)
+        return InfoFileWriterFromDREEMoutput(datafolder.name, datafolder.path_out, datafolder.path_in, predict_dms=predict_dms, predict_structure=predict_structure)
     if source == 'ct':
-        return InfoFileWriterFromCT(datafolder.name, datafolder.path_out, datafolder.path_in)
+        return InfoFileWriterFromCT(datafolder.name, datafolder.path_out, datafolder.path_in, predict_dms=predict_dms, predict_structure=predict_structure)
     if source == 'fasta':
-        return InfoFileWriterFromFasta(datafolder.name, datafolder.path_out, datafolder.path_in)
+        return InfoFileWriterFromFasta(datafolder.name, datafolder.path_out, datafolder.path_in, predict_dms=predict_dms, predict_structure=predict_structure)
     raise ValueError(f"Unknown source: {source}")
```

### Comparing `rouskinhf-0.1.4/rouskinhf/list_datapoints.py` & `rouskinhf-0.2.1/rouskinhf/list_datapoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,20 +94,19 @@
         Args:
             path (str): path to the npy file
 
         Returns:
             np.array: int-encoded sequence matrix
 
         Examples:
+            >>> from numpy import array
             >>> datapoints = ListofDatapoints([Datapoint(reference='reference', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[1.0, 2.0, 3.0]),\
                                                Datapoint(reference='reference', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[1.0, 2.0, 3.0])])
             Loaded 2 valid datapoints, filtered out 0 invalid datapoints.
-            >>> datapoints.to_sequence_npy('temp/sequence.npy')
-            array([[1, 1, 2, 2, 3, 3],
-                   [1, 1, 2, 2, 3, 3]], dtype=object)
+            >>> assert not (datapoints.to_sequence_npy('temp/sequence.npy') - array([[0, 0, 1 ,1, 2, 2],[0, 0, 1, 1, 2 ,2]], dtype=object)).any(), "The sequence matrix is not correct."
         """
 
         arr = np.array([datapoint.embed_sequence() for datapoint in self.datapoints], dtype=object)
         np.save(path, arr)
         return arr
```

### Comparing `rouskinhf-0.1.4/rouskinhf/parsers.py` & `rouskinhf-0.2.1/rouskinhf/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,18 +93,18 @@
 
         len_before = len(df)
         if drop_duplicates:
             df.drop_duplicates(subset='sequence', inplace=True)
 
 
         values = np.concatenate(df.sub_rate.values)
-        percentile90 = np.percentile(values, 90)
+        percentile975 = np.percentile(values, 97.5)
 
         def normalize(sub_rate):
             sub_rate = np.array(sub_rate)
-            sub_rate = sub_rate / percentile90
+            sub_rate = sub_rate / percentile975
             sub_rate[sub_rate > 1] = 1
             return sub_rate.tolist()
 
         for _, row in df.iterrows():
             yield row['reference'], row['sequence'], normalize(row['sub_rate'])
```

### Comparing `rouskinhf-0.1.4/rouskinhf/path.py` & `rouskinhf-0.2.1/rouskinhf/path.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,16 +20,14 @@
     -------
 
     >>> path = PathDatafolder(name='my_test_datafolder_pytest')
     >>> path.name
     'my_test_datafolder_pytest'
     >>> print(path)
     PathDatafolder(name='my_test_datafolder_pytest')
-    >>> assert "data/datafolders/my_test_datafolder_pytest/base_pairs.npy" in path.get_base_pairs_npy()
-
     """
 
     def __init__(self, name, root = DATA_FOLDER) -> None:
         assert type(name) == str, f'name {name} is not a string'
         assert type(root) == str, f'root {root} is not a string'
         self.root = root
         self.name = name
```

### Comparing `rouskinhf-0.1.4/rouskinhf/rnastructure.py` & `rouskinhf-0.2.1/rouskinhf/rnastructure.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,7 +129,9 @@
             self.__write_dms_to_file(sequence, dms)
             cmd += ' --dms ' + self.dms_file
         run_command(cmd)
         cmd = f"{os.path.join(self.rnastructure_path, 'ct2dot')} {self.ct_file} 0 {self.dot_file}"
         run_command(cmd)
         with open(self.dot_file, 'r') as f:
             return f.readlines()[2].strip()
+
+RNAstructure_singleton = RNAstructure()
```

### Comparing `rouskinhf-0.1.4/rouskinhf/util.py` & `rouskinhf-0.2.1/rouskinhf/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,15 @@
 import os
 
 # Define the one-hot encodings for the sequences and structures
 seq2int = {
-        'A': 1,
-        'C': 2,
-        'G': 3,
-        'T': 4,
-        'U': 4,
-        'N': 5,
-        'Y': 6,
-        'R': 7,
-        'K': 8,
-        'W': 9,
-        'S': 10,
-        'M': 11,
-        'B': 12,
-        'D': 13,
-        'H': 14,
-        'V': 15,
-        'X': 0
+        'A': 0,
+        'C': 1,
+        'G': 2,
+        'U': 3,
     }
 
 dot2int = {'.': 1, '(': 2, ')': 3, 'X': 0}
 int2dot = ['X', '.', '(', ')']
 
 
 def fastaToDict(fasta_file):
@@ -127,8 +114,8 @@
     sequence = sequence.upper()
     sequence = sequence.replace('T', 'U')
     # trim the sequence
     sequence = sequence.replace(' ', '').replace('\n', '').replace('\t', '')
     return sequence
 
 def sequence_has_regular_characters(sequence):
-    return not (set(sequence) - set('ACGUN'))
+    return not (set(sequence) - set('ACGU'))
```

### Comparing `rouskinhf-0.1.4/rouskinhf.egg-info/PKG-INFO` & `rouskinhf-0.2.1/rouskinhf.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: rouskinhf
-Version: 0.1.4
+Version: 0.2.1
 Summary: A library to manipulate data for our DMS prediction models.
 Author-email: Yves Martin <yves@martin.yt>, Alberic de Lajarte <albericlajarte@gmail.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-
+[![Python CI](https://github.com/rouskinlab/rouskinhf/actions/workflows/CI.yml/badge.svg)](https://github.com/rouskinlab/rouskinhf/actions/workflows/CI.yml)
+[![Publish distributions 📦 to PyPI](https://github.com/rouskinlab/rouskinhf/actions/workflows/release.yml/badge.svg)](https://github.com/rouskinlab/rouskinhf/actions/workflows/release.yml)
+![PyPI](https://img.shields.io/pypi/v/rouskinhf)
 
 # Download your RNA data from HuggingFace with rouskinhf!
 
 A repo to manipulate the data for our RNA structure prediction model. This repo allows you to:
 - pull datasets from the Rouskinlab's HuggingFace
 - create datasets from local files and push them to HuggingFace, from the formats:
     - `.fasta`
@@ -23,14 +25,24 @@
     - `.json` (DREEM output format)
     - `.json` (Rouskinlab's huggingface format)
 
 ## Important notes
 
 - Sequences with bases different than `A`, `C`, `G`, `T`, `U`, `N`, `a`, `c`, `g`, `t`, `u`, `n` are not supported. The data will be filtered out.
 
+## Dependencies
+- [RNAstructure](https://rna.urmc.rochester.edu/RNAstructure.html) (also available on [Rouskinlab GitHub](https://github.com/rouskinlab/RNAstructure)).
+
+## Push a new release to Pypi
+
+1. Edit version to `vx.y.z` in `pyproject.toml`. Then run in a terminal `git add . && git commit -m 'vx.y.z' && git push`.
+2. Create and push a git tag `vx.y.z` by running in a terminal `git tag 'vx.y.z' && git push --tag`.
+3. Create a release for the tag `vx.y.z` on Github Release.
+4. Make sure that the Github Action `Publish distributions 📦 to PyPI` passed on Github Actions.
+
 ## Installation
 
 ### Get a HuggingFace token
 
 Go to [HuggingFace](https://huggingface.co/) and create an account. Then go to your profile and copy your token ([huggingface.co/settings/tokens](https://huggingface.co/settings/tokens)).
 
 ### Create an environment file
```

