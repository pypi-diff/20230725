# Comparing `tmp/hlsvdpropy-2.0.1-py3-none-any.whl.zip` & `tmp/hlsvdpropy-2.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 29636 bytes, number of entries: 8
+Zip file size: 29621 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat      764 b- defN 20-Jun-22 23:06 hlsvdpropy/__init__.py
--rw-rw-rw-  2.0 fat    36915 b- defN 20-Jun-25 23:53 hlsvdpropy/hlsvd.py
+-rw-rw-rw-  2.0 fat    36919 b- defN 23-Jul-24 19:05 hlsvdpropy/hlsvd.py
 -rw-rw-rw-  2.0 fat     5337 b- defN 20-Jun-23 01:22 hlsvdpropy/simple_test.py
--rw-rw-rw-  2.0 fat     1530 b- defN 20-Jun-26 00:03 hlsvdpropy-2.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     5541 b- defN 20-Jun-26 00:03 hlsvdpropy-2.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 20-Jun-26 00:03 hlsvdpropy-2.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 20-Jun-26 00:03 hlsvdpropy-2.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      638 b- defN 20-Jun-26 00:03 hlsvdpropy-2.0.1.dist-info/RECORD
-8 files, 50833 bytes uncompressed, 28526 bytes compressed:  43.9%
+-rw-rw-rw-  2.0 fat     1530 b- defN 23-Jul-24 21:56 hlsvdpropy-2.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     5553 b- defN 23-Jul-24 21:56 hlsvdpropy-2.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-24 21:56 hlsvdpropy-2.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jul-24 21:56 hlsvdpropy-2.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      638 b- defN 23-Jul-24 21:56 hlsvdpropy-2.0.2.dist-info/RECORD
+8 files, 50844 bytes uncompressed, 28511 bytes compressed:  43.9%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: hlsvdpropy/hlsvd.py
 Comment: 
 
 Filename: hlsvdpropy/simple_test.py
 Comment: 
 
-Filename: hlsvdpropy-2.0.1.dist-info/LICENSE
+Filename: hlsvdpropy-2.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: hlsvdpropy-2.0.1.dist-info/METADATA
+Filename: hlsvdpropy-2.0.2.dist-info/METADATA
 Comment: 
 
-Filename: hlsvdpropy-2.0.1.dist-info/WHEEL
+Filename: hlsvdpropy-2.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: hlsvdpropy-2.0.1.dist-info/top_level.txt
+Filename: hlsvdpropy-2.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: hlsvdpropy-2.0.1.dist-info/RECORD
+Filename: hlsvdpropy-2.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hlsvdpropy/hlsvd.py

```diff
@@ -145,15 +145,15 @@
     if sparse:
         u, s, vh = scipy.sparse.linalg.svds(x, k=k)
     else:
         u, s, vh = scipy.linalg.svd(x, full_matrices=False)
 
     k = min(k,len(s))               # number of singular values found
         
-    uk = np.mat(u[:, :k])           # trucated U matrix of rank K
+    uk = u[:, :k]                   # trucated U matrix of rank K
     ub = uk[:-1]                    # Uk with bottom row removed
     ut = uk[1:]                     # Uk with top row removed
 
     zp, resid, rank, ss = scipy.linalg.lstsq(ub, ut)
 
     #----------------------------------------------------------------
     # Diagonalize Z' (=hx), yields 'signal'poles' aka 'roots'
@@ -241,15 +241,15 @@
             domain fids.
 
     """
     if convert: result = convert_hlsvd_result(result, dwell)
 
     freqs, damps, areas, phase = result[2:6]
 
-    fids = np.zeros((len(freqs), npts), dtype=np.complex)
+    fids = np.zeros((len(freqs), npts), dtype=np.complex128) 
     t = np.arange(npts) * dwell
     k = 1j * 2 * np.pi
 
     for i, damp in enumerate(damps):
         if damp:
             # hack for very small exp() values, temp disable numpy's error
             # report, it silently generate NaNs, then change those NaNs to 0.0
```

## Comparing `hlsvdpropy-2.0.1.dist-info/LICENSE` & `hlsvdpropy-2.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hlsvdpropy-2.0.1.dist-info/METADATA` & `hlsvdpropy-2.0.2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: hlsvdpropy
-Version: 2.0.1
+Version: 2.0.2
 Summary: This is a 'pure Python' implementation of the HLSVDPRO package version 2.0.0. It fits time domain data to a model function that is a set of lorentzian decaying sinusoids using the state space approach.
-Home-page: http://scion.duhs.duke.edu/projects/hlsvdpro
+Home-page: https://github.com/bsoher/hlsvdpropy
 Author: Brian J. Soher
 Author-email: bsoher@briansoher.com
 Maintainer: Brian J. Soher
 Maintainer-email: bsoher@briansoher.com
 License: https://opensource.org/licenses/BSD-3-Clause
 Keywords: svd,hlsvd,hlsvdpro,propack,time domain,fitting
 Platform: Linux
@@ -17,14 +17,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: setuptools
 
 HLSVDPROPY
 ======
 
 Overview - Black box fitting of Time Domain Signals
 ------
@@ -130,9 +131,7 @@
 
 HLSVDPRO version 2.x was adaptated to use PROPACK library version 2.1 to 
 implement the HLSVDPRO algorithm as described in T. Laudadio, N. Mastronardi
 L. Vanhamme, P. Van Hecke and S. Van Huffel, "Improved Lanczos algorithms for 
 blackbox MRS data quantitation", Journal of Magnetic Resonance, Volume 157, 
 pages 292-297, 2002. 
 
-
-
```

