# Comparing `tmp/tincheck-0.1.0.tar.gz` & `tmp/tincheck-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tincheck-0.1.0.tar", last modified: Mon Jul 24 22:14:54 2023, max compression
+gzip compressed data, was "tincheck-0.2.0.tar", last modified: Mon Jul 24 22:24:37 2023, max compression
```

## Comparing `tincheck-0.1.0.tar` & `tincheck-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 asebastian   (501) staff       (20)        0 2023-07-24 22:14:54.619599 tincheck-0.1.0/
--rw-r--r--   0 asebastian   (501) staff       (20)     4045 2023-07-24 22:14:54.619265 tincheck-0.1.0/PKG-INFO
--rw-r--r--   0 asebastian   (501) staff       (20)     3654 2023-07-24 21:28:42.000000 tincheck-0.1.0/README.md
--rw-r--r--   0 asebastian   (501) staff       (20)       38 2023-07-24 22:14:54.619712 tincheck-0.1.0/setup.cfg
--rw-r--r--   0 asebastian   (501) staff       (20)      846 2023-07-24 21:20:53.000000 tincheck-0.1.0/setup.py
-drwxr-xr-x   0 asebastian   (501) staff       (20)        0 2023-07-24 22:14:54.576347 tincheck-0.1.0/tincheck.egg-info/
--rw-r--r--   0 asebastian   (501) staff       (20)     4045 2023-07-24 22:14:54.000000 tincheck-0.1.0/tincheck.egg-info/PKG-INFO
--rw-r--r--   0 asebastian   (501) staff       (20)      315 2023-07-24 22:14:54.000000 tincheck-0.1.0/tincheck.egg-info/SOURCES.txt
--rw-r--r--   0 asebastian   (501) staff       (20)        1 2023-07-24 22:14:54.000000 tincheck-0.1.0/tincheck.egg-info/dependency_links.txt
--rw-r--r--   0 asebastian   (501) staff       (20)       50 2023-07-24 22:14:54.000000 tincheck-0.1.0/tincheck.egg-info/entry_points.txt
--rw-r--r--   0 asebastian   (501) staff       (20)        5 2023-07-24 22:14:54.000000 tincheck-0.1.0/tincheck.egg-info/requires.txt
--rw-r--r--   0 asebastian   (501) staff       (20)        7 2023-07-24 22:14:54.000000 tincheck-0.1.0/tincheck.egg-info/top_level.txt
-drwxr-xr-x   0 asebastian   (501) staff       (20)        0 2023-07-24 22:14:54.611178 tincheck-0.1.0/tinrun/
--rw-r--r--   0 asebastian   (501) staff       (20)       37 2023-07-24 21:20:53.000000 tincheck-0.1.0/tinrun/__init__.py
--rw-r--r--   0 asebastian   (501) staff       (20)      248 2023-07-24 21:20:53.000000 tincheck-0.1.0/tinrun/__main__.py
--rw-r--r--   0 asebastian   (501) staff       (20)     2518 2023-07-24 21:28:42.000000 tincheck-0.1.0/tinrun/bam2gtf.py
--rw-r--r--   0 asebastian   (501) staff       (20)      995 2023-07-24 21:28:42.000000 tincheck-0.1.0/tinrun/main.py
--rw-r--r--   0 asebastian   (501) staff       (20)    27276 2023-07-24 21:47:58.000000 tincheck-0.1.0/tinrun/overlap.py
--rw-r--r--   0 asebastian   (501) staff       (20)    23448 2023-07-24 21:47:58.000000 tincheck-0.1.0/tinrun/tin.py
+drwxr-xr-x   0 asebastian   (501) staff       (20)        0 2023-07-24 22:24:37.484785 tincheck-0.2.0/
+-rw-r--r--   0 asebastian   (501) staff       (20)     3797 2023-07-24 22:24:37.484411 tincheck-0.2.0/PKG-INFO
+-rw-r--r--   0 asebastian   (501) staff       (20)     3406 2023-07-24 22:21:00.000000 tincheck-0.2.0/README.md
+-rw-r--r--   0 asebastian   (501) staff       (20)       38 2023-07-24 22:24:37.484957 tincheck-0.2.0/setup.cfg
+-rw-r--r--   0 asebastian   (501) staff       (20)      846 2023-07-24 21:20:53.000000 tincheck-0.2.0/setup.py
+drwxr-xr-x   0 asebastian   (501) staff       (20)        0 2023-07-24 22:24:37.481673 tincheck-0.2.0/tincheck.egg-info/
+-rw-r--r--   0 asebastian   (501) staff       (20)     3797 2023-07-24 22:24:37.000000 tincheck-0.2.0/tincheck.egg-info/PKG-INFO
+-rw-r--r--   0 asebastian   (501) staff       (20)      315 2023-07-24 22:24:37.000000 tincheck-0.2.0/tincheck.egg-info/SOURCES.txt
+-rw-r--r--   0 asebastian   (501) staff       (20)        1 2023-07-24 22:24:37.000000 tincheck-0.2.0/tincheck.egg-info/dependency_links.txt
+-rw-r--r--   0 asebastian   (501) staff       (20)       50 2023-07-24 22:24:37.000000 tincheck-0.2.0/tincheck.egg-info/entry_points.txt
+-rw-r--r--   0 asebastian   (501) staff       (20)        5 2023-07-24 22:24:37.000000 tincheck-0.2.0/tincheck.egg-info/requires.txt
+-rw-r--r--   0 asebastian   (501) staff       (20)        7 2023-07-24 22:24:37.000000 tincheck-0.2.0/tincheck.egg-info/top_level.txt
+drwxr-xr-x   0 asebastian   (501) staff       (20)        0 2023-07-24 22:24:37.483900 tincheck-0.2.0/tinrun/
+-rw-r--r--   0 asebastian   (501) staff       (20)       37 2023-07-24 22:21:35.000000 tincheck-0.2.0/tinrun/__init__.py
+-rw-r--r--   0 asebastian   (501) staff       (20)      248 2023-07-24 21:20:53.000000 tincheck-0.2.0/tinrun/__main__.py
+-rw-r--r--   0 asebastian   (501) staff       (20)     2518 2023-07-24 21:28:42.000000 tincheck-0.2.0/tinrun/bam2gtf.py
+-rw-r--r--   0 asebastian   (501) staff       (20)      995 2023-07-24 21:28:42.000000 tincheck-0.2.0/tinrun/main.py
+-rw-r--r--   0 asebastian   (501) staff       (20)    27276 2023-07-24 21:47:58.000000 tincheck-0.2.0/tinrun/overlap.py
+-rw-r--r--   0 asebastian   (501) staff       (20)    23448 2023-07-24 21:47:58.000000 tincheck-0.2.0/tinrun/tin.py
```

### Comparing `tincheck-0.1.0/PKG-INFO` & `tincheck-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tincheck
-Version: 0.1.0
+Version: 0.2.0
 Summary: tincheck
 Home-page: https://github.com/aswathyseb/tincheck
 Author: Aswathy Sebastian
 Author-email: aswathyseb@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -40,28 +40,19 @@
     PF3D7_0107300	1581	    4508        100.0	    70.4
     PF3D7_0107600	5702	    4979        100.0	    74.9
     PF3D7_0107800	4424	    924	        100.0	    78.8
 
 
 **How to install the script?**
     
-    python setup.py install
-
-It would be better to create a conda environment and install the script as shown below
-    
-    conda create -n tincheck -y python=3.8
-    conda activate tincheck
+    pip install tincheck --upgrade
 
 Install additional requirements
     
-    conda install --file conda-requirements.txt 
-
-Finally, install the script in the conda environment as
-    
-    python setup.py install
+    conda install --file conda-requirements.txt
 
 **How to run the script?**
 
 The required inputs to the script is bam file(s) and annotation file in GTF or GFF format.
  
 The annotation file should have a gene feature row present in it.
```

### Comparing `tincheck-0.1.0/README.md` & `tincheck-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -27,28 +27,19 @@
     PF3D7_0107300	1581	    4508        100.0	    70.4
     PF3D7_0107600	5702	    4979        100.0	    74.9
     PF3D7_0107800	4424	    924	        100.0	    78.8
 
 
 **How to install the script?**
     
-    python setup.py install
-
-It would be better to create a conda environment and install the script as shown below
-    
-    conda create -n tincheck -y python=3.8
-    conda activate tincheck
+    pip install tincheck --upgrade
 
 Install additional requirements
     
-    conda install --file conda-requirements.txt 
-
-Finally, install the script in the conda environment as
-    
-    python setup.py install
+    conda install --file conda-requirements.txt
 
 **How to run the script?**
 
 The required inputs to the script is bam file(s) and annotation file in GTF or GFF format.
  
 The annotation file should have a gene feature row present in it.
```

### Comparing `tincheck-0.1.0/setup.py` & `tincheck-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `tincheck-0.1.0/tincheck.egg-info/PKG-INFO` & `tincheck-0.2.0/tincheck.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tincheck
-Version: 0.1.0
+Version: 0.2.0
 Summary: tincheck
 Home-page: https://github.com/aswathyseb/tincheck
 Author: Aswathy Sebastian
 Author-email: aswathyseb@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -40,28 +40,19 @@
     PF3D7_0107300	1581	    4508        100.0	    70.4
     PF3D7_0107600	5702	    4979        100.0	    74.9
     PF3D7_0107800	4424	    924	        100.0	    78.8
 
 
 **How to install the script?**
     
-    python setup.py install
-
-It would be better to create a conda environment and install the script as shown below
-    
-    conda create -n tincheck -y python=3.8
-    conda activate tincheck
+    pip install tincheck --upgrade
 
 Install additional requirements
     
-    conda install --file conda-requirements.txt 
-
-Finally, install the script in the conda environment as
-    
-    python setup.py install
+    conda install --file conda-requirements.txt
 
 **How to run the script?**
 
 The required inputs to the script is bam file(s) and annotation file in GTF or GFF format.
  
 The annotation file should have a gene feature row present in it.
```

### Comparing `tincheck-0.1.0/tinrun/bam2gtf.py` & `tincheck-0.2.0/tinrun/bam2gtf.py`

 * *Files identical despite different names*

### Comparing `tincheck-0.1.0/tinrun/main.py` & `tincheck-0.2.0/tinrun/main.py`

 * *Files identical despite different names*

### Comparing `tincheck-0.1.0/tinrun/overlap.py` & `tincheck-0.2.0/tinrun/overlap.py`

 * *Files identical despite different names*

### Comparing `tincheck-0.1.0/tinrun/tin.py` & `tincheck-0.2.0/tinrun/tin.py`

 * *Files identical despite different names*

