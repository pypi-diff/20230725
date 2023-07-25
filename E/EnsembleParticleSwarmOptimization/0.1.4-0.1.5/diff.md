# Comparing `tmp/EnsembleParticleSwarmOptimization-0.1.4.tar.gz` & `tmp/EnsembleParticleSwarmOptimization-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EnsembleParticleSwarmOptimization-0.1.4.tar", last modified: Mon Jul 24 14:55:46 2023, max compression
+gzip compressed data, was "EnsembleParticleSwarmOptimization-0.1.5.tar", last modified: Tue Jul 25 14:01:53 2023, max compression
```

## Comparing `EnsembleParticleSwarmOptimization-0.1.4.tar` & `EnsembleParticleSwarmOptimization-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-07-24 14:55:46.576557 EnsembleParticleSwarmOptimization-0.1.4/
-drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-07-24 14:55:46.576557 EnsembleParticleSwarmOptimization-0.1.4/EnsembleParticleSwarmOptimization.egg-info/
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      730 2023-07-24 14:55:46.000000 EnsembleParticleSwarmOptimization-0.1.4/EnsembleParticleSwarmOptimization.egg-info/PKG-INFO
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      431 2023-07-24 14:55:46.000000 EnsembleParticleSwarmOptimization-0.1.4/EnsembleParticleSwarmOptimization.egg-info/SOURCES.txt
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)        1 2023-07-24 14:55:46.000000 EnsembleParticleSwarmOptimization-0.1.4/EnsembleParticleSwarmOptimization.egg-info/dependency_links.txt
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)       77 2023-07-24 14:55:46.000000 EnsembleParticleSwarmOptimization-0.1.4/EnsembleParticleSwarmOptimization.egg-info/requires.txt
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)        5 2023-07-24 14:55:46.000000 EnsembleParticleSwarmOptimization-0.1.4/EnsembleParticleSwarmOptimization.egg-info/top_level.txt
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      730 2023-07-24 14:55:46.576557 EnsembleParticleSwarmOptimization-0.1.4/PKG-INFO
-drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-07-24 14:55:46.576557 EnsembleParticleSwarmOptimization-0.1.4/PySO/
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    10064 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.4/PySO/Clustering_Swarms.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    34011 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.4/PySO/HierarchicalSwarmHandler.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    30609 2023-07-24 14:53:44.000000 EnsembleParticleSwarmOptimization-0.1.4/PySO/MWE_Swarm.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)     2174 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.4/PySO/Model.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)     8369 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.4/PySO/SwarmHandler.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      288 2023-07-24 14:55:17.000000 EnsembleParticleSwarmOptimization-0.1.4/PySO/__init__.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      212 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.4/README.md
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)       38 2023-07-24 14:55:46.576557 EnsembleParticleSwarmOptimization-0.1.4/setup.cfg
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      885 2023-07-24 14:55:23.000000 EnsembleParticleSwarmOptimization-0.1.4/setup.py
+drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-07-25 14:01:53.919572 EnsembleParticleSwarmOptimization-0.1.5/
+drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-07-25 14:01:53.919572 EnsembleParticleSwarmOptimization-0.1.5/EnsembleParticleSwarmOptimization.egg-info/
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      730 2023-07-25 14:01:53.000000 EnsembleParticleSwarmOptimization-0.1.5/EnsembleParticleSwarmOptimization.egg-info/PKG-INFO
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      431 2023-07-25 14:01:53.000000 EnsembleParticleSwarmOptimization-0.1.5/EnsembleParticleSwarmOptimization.egg-info/SOURCES.txt
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)        1 2023-07-25 14:01:53.000000 EnsembleParticleSwarmOptimization-0.1.5/EnsembleParticleSwarmOptimization.egg-info/dependency_links.txt
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)       77 2023-07-25 14:01:53.000000 EnsembleParticleSwarmOptimization-0.1.5/EnsembleParticleSwarmOptimization.egg-info/requires.txt
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)        5 2023-07-25 14:01:53.000000 EnsembleParticleSwarmOptimization-0.1.5/EnsembleParticleSwarmOptimization.egg-info/top_level.txt
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      730 2023-07-25 14:01:53.919572 EnsembleParticleSwarmOptimization-0.1.5/PKG-INFO
+drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-07-25 14:01:53.919572 EnsembleParticleSwarmOptimization-0.1.5/PySO/
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    10064 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.5/PySO/Clustering_Swarms.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    34011 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.5/PySO/HierarchicalSwarmHandler.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    30629 2023-07-25 13:56:21.000000 EnsembleParticleSwarmOptimization-0.1.5/PySO/MWE_Swarm.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)     2174 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.5/PySO/Model.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)     8369 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.5/PySO/SwarmHandler.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      288 2023-07-25 13:58:45.000000 EnsembleParticleSwarmOptimization-0.1.5/PySO/__init__.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      212 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.5/README.md
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)       38 2023-07-25 14:01:53.919572 EnsembleParticleSwarmOptimization-0.1.5/setup.cfg
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      885 2023-07-25 13:58:52.000000 EnsembleParticleSwarmOptimization-0.1.5/setup.py
```

### Comparing `EnsembleParticleSwarmOptimization-0.1.4/EnsembleParticleSwarmOptimization.egg-info/PKG-INFO` & `EnsembleParticleSwarmOptimization-0.1.5/EnsembleParticleSwarmOptimization.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EnsembleParticleSwarmOptimization
-Version: 0.1.4
+Version: 0.1.5
 Summary: Ensemble of particle swarms together with various velocity rules for function optimization
 Home-page: https://github.com/dig07/PySO
 Author: Christopher Moore and Diganta Bandopadhyay
 Author-email: diganta@star.sr.bham.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `EnsembleParticleSwarmOptimization-0.1.4/PKG-INFO` & `EnsembleParticleSwarmOptimization-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EnsembleParticleSwarmOptimization
-Version: 0.1.4
+Version: 0.1.5
 Summary: Ensemble of particle swarms together with various velocity rules for function optimization
 Home-page: https://github.com/dig07/PySO
 Author: Christopher Moore and Diganta Bandopadhyay
 Author-email: diganta@star.sr.bham.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `EnsembleParticleSwarmOptimization-0.1.4/PySO/Clustering_Swarms.py` & `EnsembleParticleSwarmOptimization-0.1.5/PySO/Clustering_Swarms.py`

 * *Files identical despite different names*

### Comparing `EnsembleParticleSwarmOptimization-0.1.4/PySO/HierarchicalSwarmHandler.py` & `EnsembleParticleSwarmOptimization-0.1.5/PySO/HierarchicalSwarmHandler.py`

 * *Files identical despite different names*

### Comparing `EnsembleParticleSwarmOptimization-0.1.4/PySO/MWE_Swarm.py` & `EnsembleParticleSwarmOptimization-0.1.5/PySO/MWE_Swarm.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,18 +181,18 @@
         self.Verbose = Verbose
 
         self.SaveEvolution = Saveevolution
 
         self.Nthreads = Nthreads
 
         if Periodic is None:
-            self.Periodic = [ 0 for i in range(self.Ndim)]
+            self.Periodic = np.array([ 0 for i in range(self.Ndim)])
         else:
             assert (  len(Periodic)==self.Ndim  and  all(np.isin(Periodic, [0,1]))  )
-            self.Periodic = list(Periodic)
+            self.Periodic = np.array(list(Periodic))
 
         self.PeriodicParamRanges = np.array([
                                             np.inf if self.Periodic[i]==0 else np.ptp(b)
                                         for i, b in enumerate(self.Model.bounds)])
 
 	# Param indexes where periodicity happens
         self.Periodic_params = np.where(self.Periodic == 1)[0]
```

### Comparing `EnsembleParticleSwarmOptimization-0.1.4/PySO/Model.py` & `EnsembleParticleSwarmOptimization-0.1.5/PySO/Model.py`

 * *Files identical despite different names*

### Comparing `EnsembleParticleSwarmOptimization-0.1.4/PySO/SwarmHandler.py` & `EnsembleParticleSwarmOptimization-0.1.5/PySO/SwarmHandler.py`

 * *Files identical despite different names*

### Comparing `EnsembleParticleSwarmOptimization-0.1.4/setup.py` & `EnsembleParticleSwarmOptimization-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="EnsembleParticleSwarmOptimization",
-    version="0.1.4",
+    version="0.1.5",
     author="Christopher Moore and Diganta Bandopadhyay",
     author_email="diganta@star.sr.bham.ac.uk",
     description="Ensemble of particle swarms together with various velocity rules for function optimization",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dig07/PySO",
     packages=setuptools.find_packages(),
```

