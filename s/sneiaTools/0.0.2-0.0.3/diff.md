# Comparing `tmp/sneiaTools-0.0.2-py3-none-any.whl.zip` & `tmp/sneiaTools-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2857 bytes, number of entries: 7
+Zip file size: 2909 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat      129 b- defN 23-Jul-14 18:40 sneiaTools/__init__.py
--rw-rw-rw-  2.0 fat     1459 b- defN 23-Jul-14 17:59 sneiaTools/metrics.py
--rw-rw-rw-  2.0 fat     1134 b- defN 23-Jul-14 18:41 sneiaTools-0.0.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      388 b- defN 23-Jul-14 18:41 sneiaTools-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-14 18:41 sneiaTools-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jul-14 18:41 sneiaTools-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      556 b- defN 23-Jul-14 18:41 sneiaTools-0.0.2.dist-info/RECORD
-7 files, 3769 bytes uncompressed, 1869 bytes compressed:  50.4%
+-rw-rw-rw-  2.0 fat     1907 b- defN 23-Jul-25 19:20 sneiaTools/metrics.py
+-rw-rw-rw-  2.0 fat     1134 b- defN 23-Jul-25 19:25 sneiaTools-0.0.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      418 b- defN 23-Jul-25 19:25 sneiaTools-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-25 19:25 sneiaTools-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jul-25 19:25 sneiaTools-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      556 b- defN 23-Jul-25 19:25 sneiaTools-0.0.3.dist-info/RECORD
+7 files, 4247 bytes uncompressed, 1921 bytes compressed:  54.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: sneiaTools/__init__.py
 Comment: 
 
 Filename: sneiaTools/metrics.py
 Comment: 
 
-Filename: sneiaTools-0.0.2.dist-info/LICENSE
+Filename: sneiaTools-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: sneiaTools-0.0.2.dist-info/METADATA
+Filename: sneiaTools-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: sneiaTools-0.0.2.dist-info/WHEEL
+Filename: sneiaTools-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: sneiaTools-0.0.2.dist-info/top_level.txt
+Filename: sneiaTools-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: sneiaTools-0.0.2.dist-info/RECORD
+Filename: sneiaTools-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sneiaTools/metrics.py

```diff
@@ -1,36 +1,41 @@
 import numpy as np
 
 class Metrics:
 
     def __init__(self):
         pass
 
-    def mae(self, predictions, targets):
+    def mae(self, predictions, targets, check_symmetry = True):
+        if len(predictions) != len(targets) and check_symmetry:
+            raise ValueError("The length of predictions and targets must be the same.")
         targets, predictions = np.array(targets), np.array(predictions)
         mae = np.mean(np.abs(predictions - targets))
         return mae
 
-    def mse(self, predictions, target):
-        if len(predictions) != len(target):
+    def mse(self, predictions, target, check_symmetry = True):
+        if len(predictions) != len(target) and check_symmetry:
             raise ValueError("The length of predictions and target must be the same.")
         squared_errors = [(pred - target) ** 2 for pred, target in zip(predictions, target)]
         mse = sum(squared_errors) / len(predictions)
         return mse
 
-    def rmse(self, predictions, targets):
-        if len(predictions) != len(targets):
+    def rmse(self, predictions, targets, check_symmetry = True):
+        if len(predictions) != len(targets) and check_symmetry:
             raise ValueError("The length of predictions and targets must be the same.")
         
         squared_errors = [(pred - target) ** 2 for pred, target in zip(predictions, targets)]
         mse = sum(squared_errors) / len(predictions)
         rmse = np.sqrt(mse)
         return rmse
 
-    def re(self, predictions, targets, return_epsilon = False):
+    def re(self, predictions, targets, return_epsilon = False, check_symmetry = True):
+        if len(predictions) != len(targets) and check_symmetry:
+            raise ValueError("The length of predictions and targets must be the same.")
+        
         N = targets.shape[0]
         M = targets.shape[1]
         
         epsilon = np.mean(np.sum(np.abs(targets - predictions) / M, axis=1))
         sigma_e = np.sqrt(np.mean((np.sum(np.abs(targets - predictions) / M, axis = 1) - epsilon) ** 2))
 
         if return_epsilon:
```

## Comparing `sneiaTools-0.0.2.dist-info/LICENSE` & `sneiaTools-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

