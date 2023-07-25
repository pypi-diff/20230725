# Comparing `tmp/squic-1.0.2.tar.gz` & `tmp/squic-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squic-1.0.2.tar", last modified: Tue Sep 20 14:20:43 2022, max compression
+gzip compressed data, was "squic-1.0.3.tar", last modified: Tue Jul 25 16:57:42 2023, max compression
```

## Comparing `squic-1.0.2.tar` & `squic-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 aryan      (503) staff       (20)        0 2022-09-20 14:20:43.310965 squic-1.0.2/
--rw-r--r--   0 aryan      (503) staff       (20)    35148 2022-07-21 14:08:13.000000 squic-1.0.2/LICENSE
--rw-r--r--   0 aryan      (503) staff       (20)       48 2022-07-21 14:08:13.000000 squic-1.0.2/MANIFEST.in
--rw-r--r--   0 aryan      (503) staff       (20)     3609 2022-09-20 14:20:43.311101 squic-1.0.2/PKG-INFO
--rw-r--r--   0 aryan      (503) staff       (20)     2867 2022-09-20 14:10:03.000000 squic-1.0.2/README.md
--rw-r--r--   0 aryan      (503) staff       (20)      103 2022-07-21 14:08:13.000000 squic-1.0.2/pyproject.toml
--rw-r--r--   0 aryan      (503) staff       (20)      912 2022-09-20 14:20:43.311652 squic-1.0.2/setup.cfg
--rw-r--r--   0 aryan      (503) staff       (20)       38 2022-07-21 14:08:13.000000 squic-1.0.2/setup.py
-drwxr-xr-x   0 aryan      (503) staff       (20)        0 2022-09-20 14:20:43.294735 squic-1.0.2/src/
-drwxr-xr-x   0 aryan      (503) staff       (20)        0 2022-09-20 14:20:43.306702 squic-1.0.2/src/squic/
--rw-r--r--   0 aryan      (503) staff       (20)     3745 2022-07-21 14:08:15.000000 squic-1.0.2/src/squic/__init__.py
--rw-r--r--   0 aryan      (503) staff       (20)    11678 2022-09-20 14:10:04.000000 squic-1.0.2/src/squic/squic.py
-drwxr-xr-x   0 aryan      (503) staff       (20)        0 2022-09-20 14:20:43.310702 squic-1.0.2/src/squic.egg-info/
--rw-r--r--   0 aryan      (503) staff       (20)     3609 2022-09-20 14:20:43.000000 squic-1.0.2/src/squic.egg-info/PKG-INFO
--rw-r--r--   0 aryan      (503) staff       (20)      268 2022-09-20 14:20:43.000000 squic-1.0.2/src/squic.egg-info/SOURCES.txt
--rw-r--r--   0 aryan      (503) staff       (20)        1 2022-09-20 14:20:43.000000 squic-1.0.2/src/squic.egg-info/dependency_links.txt
--rw-r--r--   0 aryan      (503) staff       (20)       12 2022-09-20 14:20:43.000000 squic-1.0.2/src/squic.egg-info/requires.txt
--rw-r--r--   0 aryan      (503) staff       (20)        6 2022-09-20 14:20:43.000000 squic-1.0.2/src/squic.egg-info/top_level.txt
+drwxr-xr-x   0 aryan      (501) staff       (20)        0 2023-07-25 16:57:42.340337 squic-1.0.3/
+-rw-r--r--   0 aryan      (501) staff       (20)    35148 2023-07-25 11:49:30.000000 squic-1.0.3/LICENSE
+-rw-r--r--   0 aryan      (501) staff       (20)       48 2023-07-25 11:49:30.000000 squic-1.0.3/MANIFEST.in
+-rw-r--r--   0 aryan      (501) staff       (20)     3628 2023-07-25 16:57:42.340385 squic-1.0.3/PKG-INFO
+-rw-r--r--   0 aryan      (501) staff       (20)     2886 2023-07-25 12:03:23.000000 squic-1.0.3/README.md
+-rw-r--r--   0 aryan      (501) staff       (20)      103 2023-07-25 11:49:30.000000 squic-1.0.3/pyproject.toml
+-rw-r--r--   0 aryan      (501) staff       (20)      912 2023-07-25 16:57:42.340583 squic-1.0.3/setup.cfg
+-rw-r--r--   0 aryan      (501) staff       (20)       38 2023-07-25 11:49:30.000000 squic-1.0.3/setup.py
+drwxr-xr-x   0 aryan      (501) staff       (20)        0 2023-07-25 16:57:42.337770 squic-1.0.3/src/
+drwxr-xr-x   0 aryan      (501) staff       (20)        0 2023-07-25 16:57:42.339523 squic-1.0.3/src/squic/
+-rw-r--r--   0 aryan      (501) staff       (20)     3680 2023-07-25 12:38:53.000000 squic-1.0.3/src/squic/__init__.py
+-rw-r--r--   0 aryan      (501) staff       (20)    11857 2023-07-25 12:38:35.000000 squic-1.0.3/src/squic/squic.py
+drwxr-xr-x   0 aryan      (501) staff       (20)        0 2023-07-25 16:57:42.340247 squic-1.0.3/src/squic.egg-info/
+-rw-r--r--   0 aryan      (501) staff       (20)     3628 2023-07-25 16:57:42.000000 squic-1.0.3/src/squic.egg-info/PKG-INFO
+-rw-r--r--   0 aryan      (501) staff       (20)      268 2023-07-25 16:57:42.000000 squic-1.0.3/src/squic.egg-info/SOURCES.txt
+-rw-r--r--   0 aryan      (501) staff       (20)        1 2023-07-25 16:57:42.000000 squic-1.0.3/src/squic.egg-info/dependency_links.txt
+-rw-r--r--   0 aryan      (501) staff       (20)       12 2023-07-25 16:57:42.000000 squic-1.0.3/src/squic.egg-info/requires.txt
+-rw-r--r--   0 aryan      (501) staff       (20)        6 2023-07-25 16:57:42.000000 squic-1.0.3/src/squic.egg-info/top_level.txt
```

### Comparing `squic-1.0.2/LICENSE` & `squic-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `squic-1.0.2/PKG-INFO` & `squic-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: squic
-Version: 1.0.2
+Version: 1.0.3
 Summary: SQUIC is a second-order, L1-regularized maximum likelihood method for performant large-scale sparse precision matrix estimation. This repository contains the source code for the Python interface of SQUIC.
 Home-page: https://www.gitlab.ci.inf.usi.ch/SQUIC/SQUIC_Python
 Author: Aryan Eftekhari, Lisa Gaedke-Merzhaeuser, Dimosthenis Pasadakis, Matthias Bollhoefer, Simon Scheidegger, Olaf Schenk
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SQUIC for Python
 SQUIC is a second-order, L1-regularized maximum likelihood method for performant large-scale sparse precision matrix estimation. This repository contains the source code for the Python(v3) interface of SQUIC. 
 
-**For an interactive session using SQUIC for Python see Google Colab:**
+**For an interactive session using SQUIC for Python, see Google Colab:**
 
 [![SQUIC for Python](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1iQB5hz07UMd5C1PR3w3xM3306BVcFGiO?usp=sharing)
 
 ## Installation
 
 #### Step 1:
 Download the shared library ``libSQUIC`` from www.gitlab.ci.inf.usi.ch/SQUIC/libSQUIC, and follow its README instructions. The default and recommended location for ``libSQUIC`` is the home directory, i.e., ``~/``. Note that precompiled versions are available.
@@ -40,14 +40,15 @@
 
 # generate sample from tridiagonal precision matrix
 p = 1024
 n = 100
 l = .4
 
 # generate a tridiagonal matrix
+np.random.seed(1)
 a = -0.5 * np.ones(p-1)
 b = 1.25 * np.ones(p)
 iC_star = np.diag(a,-1) + np.diag(b,0) + np.diag(a,1)
 
 # generate the data
 L = np.linalg.cholesky(iC_star)
 Y = np.linalg.solve(L.T,np.random.randn(p,n))
```

### Comparing `squic-1.0.2/README.md` & `squic-1.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # SQUIC for Python
 SQUIC is a second-order, L1-regularized maximum likelihood method for performant large-scale sparse precision matrix estimation. This repository contains the source code for the Python(v3) interface of SQUIC. 
 
-**For an interactive session using SQUIC for Python see Google Colab:**
+**For an interactive session using SQUIC for Python, see Google Colab:**
 
 [![SQUIC for Python](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1iQB5hz07UMd5C1PR3w3xM3306BVcFGiO?usp=sharing)
 
 ## Installation
 
 #### Step 1:
 Download the shared library ``libSQUIC`` from www.gitlab.ci.inf.usi.ch/SQUIC/libSQUIC, and follow its README instructions. The default and recommended location for ``libSQUIC`` is the home directory, i.e., ``~/``. Note that precompiled versions are available.
@@ -26,14 +26,15 @@
 
 # generate sample from tridiagonal precision matrix
 p = 1024
 n = 100
 l = .4
 
 # generate a tridiagonal matrix
+np.random.seed(1)
 a = -0.5 * np.ones(p-1)
 b = 1.25 * np.ones(p)
 iC_star = np.diag(a,-1) + np.diag(b,0) + np.diag(a,1)
 
 # generate the data
 L = np.linalg.cholesky(iC_star)
 Y = np.linalg.solve(L.T,np.random.randn(p,n))
```

### Comparing `squic-1.0.2/setup.cfg` & `squic-1.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = squic
-version = 1.0.2
+version = 1.0.3
 author = Aryan Eftekhari, Lisa Gaedke-Merzhaeuser, Dimosthenis Pasadakis, Matthias Bollhoefer, Simon Scheidegger, Olaf Schenk
 description = SQUIC is a second-order, L1-regularized maximum likelihood method for performant large-scale sparse precision matrix estimation. This repository contains the source code for the Python interface of SQUIC.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://www.gitlab.ci.inf.usi.ch/SQUIC/SQUIC_Python
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `squic-1.0.2/src/squic/__init__.py` & `squic-1.0.3/src/squic/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 #################
 # Description:
 #################
 
 SQUIC is a second-order, L1-regularized maximum likelihood method for performant large-scale sparse precision matrix estimation.
 
-
 #################
 # Usage :
 #################
 
-[X,W,info_times,info_objective,info_logdetX,info_trSX]=SQUIC.run(Y, lambda, max_iter = 100, tol = 1e-3, verbose = 1, M = NULL,  X0 = NULL, W0 = NULL)
+[X,W,info_times,info_objective,info_logdetX,info_trSX]=SQUIC.run(Y, lambda, max_iter = 100, tol = 1e-3, tol_inv = 1e-4, verbose = 1, M = NULL,  X0 = NULL, W0 = NULL)
 [_,S,info_times,_,_,_]=SQUIC.run(Y, lambda, max_iter = 0)
 
 Arguments:
-    Y:          Input data in the formp(dimensions) x n(samples).
+    Y:          Input data in the form p (dimensions) x n (samples).
     l:          Scalar tuning parameter a non-zero positive number.
     max_iter:   Maximum number of Newton iterations.
-    tol:        Tolerance for convergence and approximate inversion.
+    tol:        Tolerance for convergence.
+    tol_inv:    Tolerance for approximate inversion.
     verbose:    Level of printing output (0 or 1).
     M:          A symmetric sparse (p by p); See note (3) below for details.
     X0:         Initial value of precision matrix as a sparse matrix (p x p) .
     W0:         Initial value of inverse precision matrix as a sparse matrix (p x p) ..
 
 NOTE:
 (1) If max_iter=0, the returned value for the inverse of the precision matrix (W) is the sparse sample covariance matrix (S).
@@ -29,15 +29,15 @@
 (3) The matrix tuning paramter Lambda:=M_{ij} for M_{ij} != 0 and Lambda_{ij}:=lambda, if otherwise. When M=NULL we have Lambda_{ij}=lambda.
 (4) After importing the package the user must set the path of the shared library libSQUIC.*, using function SQUIC.PATH_TO_libSQUIC().
 
 Return values:
 
  X: Estimated precision matrix (p x p).
  W: Estimated inverse of the precision matrix (p x p).
- S: Sparse (threashold) sample covariance matrix (p x p).
+ S: Sparse (threshold) sample covariance matrix (p x p).
  info_times: Total runtime.
     [0] info_time_total: Total runtime.
     [1] info_time_sample_cov: Runtime of the sample covariance matrix.
     [2] info_time_optimize: Runtime of the Newton steps
     [3] info_time_factor: Runtime of the matrix factorization.
     [4] info_time_approximate_inv: Runtime of the approximate matrix inversion.
     [5] info_time_coordinate_upd: Runtime of the coordinate descent update.
@@ -58,35 +58,30 @@
 
 Eftekhari, A., Pasadakis, D., Bollhöfer, M., Scheidegger, S. and Schenk, O., 2021. Block-Enhanced Precision Matrix Estimation
 for Large-Scale Datasets. Journal of Computational Science, p. 101389.
 
 #################
 # Example:
 #################
-
-import SQUIC 
+import squic
 import numpy as np
 
-# set location of libSQUIC (set after importing package)
-SQUIC.PATH_TO_libSQUIC('/path/to/squic')
-
 # generate sample from tridiagonal precision matrix
 p = 1024
 n = 100
 l = .4
-max_iter = 100
-tol = 1e-3
 
 # generate a tridiagonal matrix
+np.random.seed(1)
 a = -0.5 * np.ones(p-1)
 b = 1.25 * np.ones(p)
 iC_star = np.diag(a,-1) + np.diag(b,0) + np.diag(a,1)
 
 # generate the data
 L = np.linalg.cholesky(iC_star)
 Y = np.linalg.solve(L.T,np.random.randn(p,n))
 
-[X,W,info_times,info_objective,info_logdetX,info_trSX] = SQUIC.run(Y,l)
+[X,W,info_times,info_objective,info_logdetX,info_trSX] = squic.run(Y,l)
 """
 
 from .squic import *
```

### Comparing `squic-1.0.2/src/squic/squic.py` & `squic-1.0.3/src/squic/squic.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,27 +34,28 @@
 except KeyError:
     raise Exception("#SQUIC: OS not supported.")
 except OSError as e:
     print(e)
     print("SQUIC library not found, please use SQUIC_LIB_PATH env variable!!")
     exit(1)
 
-def run(Y:np.array, l:float, max_iter:int=100, tol:float=1e-3,verbose:int=1, M:np.array=None, X0:np.array=None, W0:np.array=None)->list:
+def run(Y:np.array, l:float, max_iter:int=100, tol:float=1e-3,tol_inv:float=1e-4,verbose:int=1, M:np.array=None, X0:np.array=None, W0:np.array=None)->list:
     """SQUIC is a second-order, L1-regularized maximum likelihood method for performant large-scale sparse precision matrix estimation.
 See help(squic) for further details. Note: If max_iter=0, the returned value for the inverse of the precision matrix (W) is the sparse sample covariance matrix (S).
 
     Args:
         Y (np.array): Input data in the form p (dimensions) by n (samples).
         l (float): Scalar tuning parameter λ>0.
-        max_iter (int, optional): Maximum number of Newton iterations of the outer loop. Defaults to 100.
-        tol (float, optional): Tolerance for convergence and approximate inversion. Defaults to 1e-3.
-        verbose (int, optional): Level of printing output (0 or 1). Defaults to 1.
-        M (np.array, optional):  Defines the penalty matrix parameters where Λ_ij = M_ij if M_ij ≠ 0 else λ. Defaults to Zeros (denoted by None).
-        X0 (np.array, optional): Initial guess of the precision matrix Θ. Defaults to Identity (denote by None).
-        W0 (np.array, optional): Initial guess of the inverse of the precision matrix W=inv(Θ). Defaults to Identity (denote by None).
+        max_iter (int, optional): Maximum number of Newton iterations of the outer loop. Default to 100.
+        tol (float, optional): Tolerance for convergence. Default to 1e-3.
+        tol_inv (float, optional): Tolerance for approximate inversion. Default to 1e-4.
+        verbose (int, optional): Level of printing output (0 or 1). Default to 1.
+        M (np.array, optional):  Defines the penalty matrix parameters where Λ_ij = M_ij if M_ij ≠ 0 else λ. Default to Zeros (denoted by None).
+        X0 (np.array, optional): Initial guess of the precision matrix Θ. Default to Identity (denote by None).
+        W0 (np.array, optional): Initial guess of the inverse of the precision matrix W=inv(Θ). Default to Identity (denote by None).
 
     Returns:
         list->[X,W,info_times,info_objective,info_logdetX,info_trSX]:
         - X: Estimated precision matrix.
         - W: Estimated inverse of the precision matrix.
         - info_times: Component runtimes times.
             info_times[0]: Total runtime.
@@ -84,27 +85,30 @@
 
     if(max_iter<0):
         raise ValueError("#SQUIC: max_iter cannot be negative.");
 
     if(tol<=0):
         raise ValueError("#SQUIC: tol must be great than zero.");
 
+    if(tol_inv<=0):
+        raise ValueError("#SQUIC: tol_inv must be great than zero.");
+        
     #################################################
     # if mode = [0,1,2,3,4] we Block-SQUIC or [5,6,7,8,9] Scalar-SQUIC
     mode  = c_int(0)
 
     # The data needs to be fortran (column major)
     Y     = np.array(Y,order='F')
     Y_ptr = Y.ctypes.data_as(POINTER(c_double))
 
     #################################################
     # tolerances
     # Hard code both tolerances to be the same
     term_tol = tol
-    inv_tol  = tol
+    inv_tol  = tol_inv
 
     #################################################
     # Matrices
     #################################################
 
     # X & W Matrix Checks
     if(X0 is None or W0 is None ):
```

### Comparing `squic-1.0.2/src/squic.egg-info/PKG-INFO` & `squic-1.0.3/src/squic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: squic
-Version: 1.0.2
+Version: 1.0.3
 Summary: SQUIC is a second-order, L1-regularized maximum likelihood method for performant large-scale sparse precision matrix estimation. This repository contains the source code for the Python interface of SQUIC.
 Home-page: https://www.gitlab.ci.inf.usi.ch/SQUIC/SQUIC_Python
 Author: Aryan Eftekhari, Lisa Gaedke-Merzhaeuser, Dimosthenis Pasadakis, Matthias Bollhoefer, Simon Scheidegger, Olaf Schenk
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SQUIC for Python
 SQUIC is a second-order, L1-regularized maximum likelihood method for performant large-scale sparse precision matrix estimation. This repository contains the source code for the Python(v3) interface of SQUIC. 
 
-**For an interactive session using SQUIC for Python see Google Colab:**
+**For an interactive session using SQUIC for Python, see Google Colab:**
 
 [![SQUIC for Python](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1iQB5hz07UMd5C1PR3w3xM3306BVcFGiO?usp=sharing)
 
 ## Installation
 
 #### Step 1:
 Download the shared library ``libSQUIC`` from www.gitlab.ci.inf.usi.ch/SQUIC/libSQUIC, and follow its README instructions. The default and recommended location for ``libSQUIC`` is the home directory, i.e., ``~/``. Note that precompiled versions are available.
@@ -40,14 +40,15 @@
 
 # generate sample from tridiagonal precision matrix
 p = 1024
 n = 100
 l = .4
 
 # generate a tridiagonal matrix
+np.random.seed(1)
 a = -0.5 * np.ones(p-1)
 b = 1.25 * np.ones(p)
 iC_star = np.diag(a,-1) + np.diag(b,0) + np.diag(a,1)
 
 # generate the data
 L = np.linalg.cholesky(iC_star)
 Y = np.linalg.solve(L.T,np.random.randn(p,n))
```

