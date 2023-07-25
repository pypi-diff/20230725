# Comparing `tmp/MarsGT-0.1.9.tar.gz` & `tmp/MarsGT-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MarsGT-0.1.9.tar", last modified: Sun Jul 23 14:08:21 2023, max compression
+gzip compressed data, was "MarsGT-0.2.0.tar", last modified: Tue Jul 25 04:49:58 2023, max compression
```

## Comparing `MarsGT-0.1.9.tar` & `MarsGT-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-07-23 14:08:21.179870 MarsGT-0.1.9/
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)       34 2023-06-03 06:21:54.000000 MarsGT-0.1.9/MANIFEST.in
-drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-07-23 14:08:21.137859 MarsGT-0.1.9/MarsGT/
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        2 2023-06-03 06:21:57.000000 MarsGT-0.1.9/MarsGT/__init__.py
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     6719 2023-06-03 08:36:23.000000 MarsGT-0.1.9/MarsGT/conv.py
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     8824 2023-07-18 10:28:20.000000 MarsGT-0.1.9/MarsGT/egrn.py
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)    21360 2023-06-03 08:36:23.000000 MarsGT-0.1.9/MarsGT/marsgt_model.py
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     8280 2023-07-23 14:06:25.000000 MarsGT-0.1.9/MarsGT/utils.py
-drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-07-23 14:08:21.173852 MarsGT-0.1.9/MarsGT.egg-info/
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      963 2023-07-23 14:08:20.000000 MarsGT-0.1.9/MarsGT.egg-info/PKG-INFO
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      267 2023-07-23 14:08:20.000000 MarsGT-0.1.9/MarsGT.egg-info/SOURCES.txt
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        1 2023-07-23 14:08:20.000000 MarsGT-0.1.9/MarsGT.egg-info/dependency_links.txt
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      260 2023-07-23 14:08:20.000000 MarsGT-0.1.9/MarsGT.egg-info/requires.txt
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        7 2023-07-23 14:08:20.000000 MarsGT-0.1.9/MarsGT.egg-info/top_level.txt
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      963 2023-07-23 14:08:21.177889 MarsGT-0.1.9/PKG-INFO
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      709 2023-07-19 01:31:01.000000 MarsGT-0.1.9/README.md
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)       38 2023-07-23 14:08:21.180857 MarsGT-0.1.9/setup.cfg
--rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1336 2023-07-23 14:07:48.000000 MarsGT-0.1.9/setup.py
+drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-07-25 04:49:57.982256 MarsGT-0.2.0/
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)       34 2023-06-03 06:21:54.000000 MarsGT-0.2.0/MANIFEST.in
+drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-07-25 04:49:57.945258 MarsGT-0.2.0/MarsGT/
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        2 2023-06-03 06:21:57.000000 MarsGT-0.2.0/MarsGT/__init__.py
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     6719 2023-06-03 08:36:23.000000 MarsGT-0.2.0/MarsGT/conv.py
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     8824 2023-07-18 10:28:20.000000 MarsGT-0.2.0/MarsGT/egrn.py
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)    21360 2023-06-03 08:36:23.000000 MarsGT-0.2.0/MarsGT/marsgt_model.py
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     8280 2023-07-23 14:06:25.000000 MarsGT-0.2.0/MarsGT/utils.py
+drwxr-xr-x   0 duanmaoteng (40439) PCON0022  (6618)        0 2023-07-25 04:49:57.976261 MarsGT-0.2.0/MarsGT.egg-info/
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1006 2023-07-25 04:49:56.000000 MarsGT-0.2.0/MarsGT.egg-info/PKG-INFO
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      267 2023-07-25 04:49:57.000000 MarsGT-0.2.0/MarsGT.egg-info/SOURCES.txt
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        1 2023-07-25 04:49:56.000000 MarsGT-0.2.0/MarsGT.egg-info/dependency_links.txt
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      246 2023-07-25 04:49:56.000000 MarsGT-0.2.0/MarsGT.egg-info/requires.txt
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)        7 2023-07-25 04:49:56.000000 MarsGT-0.2.0/MarsGT.egg-info/top_level.txt
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1006 2023-07-25 04:49:57.980257 MarsGT-0.2.0/PKG-INFO
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)      709 2023-07-19 01:31:01.000000 MarsGT-0.2.0/README.md
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)       38 2023-07-25 04:49:57.982262 MarsGT-0.2.0/setup.cfg
+-rw-r--r--   0 duanmaoteng (40439) PCON0022  (6618)     1317 2023-07-25 04:48:40.000000 MarsGT-0.2.0/setup.py
```

### Comparing `MarsGT-0.1.9/MarsGT/conv.py` & `MarsGT-0.2.0/MarsGT/conv.py`

 * *Files identical despite different names*

### Comparing `MarsGT-0.1.9/MarsGT/egrn.py` & `MarsGT-0.2.0/MarsGT/egrn.py`

 * *Files identical despite different names*

### Comparing `MarsGT-0.1.9/MarsGT/marsgt_model.py` & `MarsGT-0.2.0/MarsGT/marsgt_model.py`

 * *Files identical despite different names*

### Comparing `MarsGT-0.1.9/MarsGT/utils.py` & `MarsGT-0.2.0/MarsGT/utils.py`

 * *Files identical despite different names*

### Comparing `MarsGT-0.1.9/MarsGT.egg-info/PKG-INFO` & `MarsGT-0.2.0/MarsGT.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: MarsGT
-Version: 0.1.9
+Version: 0.2.0
 Summary: MarsGT: A Python library for rare cell identification (Internal testing only)
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: ==3.8.0
+Requires-Python: >=3.8.0, <3.9
 Description-Content-Type: text/markdown
 
 ## Title：MarsGT:Multi-omics data analysis for rare population inference using single-cell graph transformer
 **Note: This project is for internal testing purposes only. Do not use it in a production environment.**
 
 MarsGT, for rare cell identification from matched scRNA-seq (snRNA-seq) and scATAC-seq (snATAC-seq),includes genes, enhancers, and cells in a heterogeneous graph to simultaneously identify major cell clusters and rare cell clusters based on eRegulon.
 ## Installation
@@ -21,7 +23,9 @@
 ```bash
 pip install -r requirements.txt
 ```
 * use pip to install MarsGT:
 ```bash
 pip install MarsGT
 ```
+
+
```

### Comparing `MarsGT-0.1.9/PKG-INFO` & `MarsGT-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: MarsGT
-Version: 0.1.9
+Version: 0.2.0
 Summary: MarsGT: A Python library for rare cell identification (Internal testing only)
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: ==3.8.0
+Requires-Python: >=3.8.0, <3.9
 Description-Content-Type: text/markdown
 
 ## Title：MarsGT:Multi-omics data analysis for rare population inference using single-cell graph transformer
 **Note: This project is for internal testing purposes only. Do not use it in a production environment.**
 
 MarsGT, for rare cell identification from matched scRNA-seq (snRNA-seq) and scATAC-seq (snATAC-seq),includes genes, enhancers, and cells in a heterogeneous graph to simultaneously identify major cell clusters and rare cell clusters based on eRegulon.
 ## Installation
@@ -21,7 +23,9 @@
 ```bash
 pip install -r requirements.txt
 ```
 * use pip to install MarsGT:
 ```bash
 pip install MarsGT
 ```
+
+
```

### Comparing `MarsGT-0.1.9/README.md` & `MarsGT-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `MarsGT-0.1.9/setup.py` & `MarsGT-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 setup(
     name="MarsGT",
-    version='0.1.9',
+    version='0.2.0',
     packages=find_packages(),
     install_requires=[
         'anndata==0.8.0',
         'dill==0.3.4',
         'matplotlib==3.5.1',
         'numpy==1.22.3',
         'pandas==1.4.2',
         'scipy==1.9.1',
         'seaborn==0.11.2',
         'scikit-learn==1.1.2',
-        'torch==1.12.0',
         'torch-geometric==2.1.0.post1',
         'torchmetrics==0.9.3',
         'xlwt==1.3.0',
         'tqdm==4.64.0',
         'scanpy==1.9.1',
         'leidenalg==0.8.10',
         'ipywidgets==8.0.6'
@@ -28,15 +27,15 @@
     extras_require={
         # The following packages are not available on PyPI as binary wheels with CPU support.
         # Users must manually install them using the appropriate command:
         # "torch_sparse": ["torch-sparse==0.6.12+cpu"],
         # "torch_scatter": ["torch-scatter==2.0.9+cpu"],
         # "torch_cluster": ["torch-cluster==1.5.9+cpu"],
     },
-    python_requires='==3.8.0',
+    python_requires='>=3.8.0, <3.9',
     description="MarsGT: A Python library for rare cell identification (Internal testing only)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "License :: OSI Approved :: MIT License"
     ]
 )
```

