# Comparing `tmp/nebula-loss-0.3.3.tar.gz` & `tmp/nebula-loss-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nebula-loss-0.3.3.tar", last modified: Sat May 27 06:49:37 2023, max compression
+gzip compressed data, was "nebula-loss-0.4.1.tar", last modified: Tue Jul 25 15:33:53 2023, max compression
```

## Comparing `nebula-loss-0.3.3.tar` & `nebula-loss-0.4.1.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:49:37.592403 nebula-loss-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-27 06:49:26.000000 nebula-loss-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-27 06:49:37.592403 nebula-loss-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-27 06:49:26.000000 nebula-loss-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:49:37.592403 nebula-loss-0.3.3/nebula/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-27 06:49:26.000000 nebula-loss-0.3.3/nebula/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-05-27 06:49:26.000000 nebula-loss-0.3.3/nebula/nebulav2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:49:37.592403 nebula-loss-0.3.3/nebula_loss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-27 06:49:37.000000 nebula-loss-0.3.3/nebula_loss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-27 06:49:37.000000 nebula-loss-0.3.3/nebula_loss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 06:49:37.000000 nebula-loss-0.3.3/nebula_loss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-27 06:49:37.000000 nebula-loss-0.3.3/nebula_loss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-27 06:49:37.000000 nebula-loss-0.3.3/nebula_loss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 06:49:37.592403 nebula-loss-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-27 06:49:26.000000 nebula-loss-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:33:53.421637 nebula-loss-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-25 15:33:36.000000 nebula-loss-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-25 15:33:53.421637 nebula-loss-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-07-25 15:33:36.000000 nebula-loss-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:33:53.421637 nebula-loss-0.4.1/nebula/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-25 15:33:36.000000 nebula-loss-0.4.1/nebula/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-07-25 15:33:36.000000 nebula-loss-0.4.1/nebula/nebula.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-25 15:33:36.000000 nebula-loss-0.4.1/nebula/nebula_genetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-25 15:33:36.000000 nebula-loss-0.4.1/nebula/nebula_multimodal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-25 15:33:36.000000 nebula-loss-0.4.1/nebula/nebula_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:33:53.421637 nebula-loss-0.4.1/nebula_loss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-25 15:33:53.000000 nebula-loss-0.4.1/nebula_loss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-25 15:33:53.000000 nebula-loss-0.4.1/nebula_loss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 15:33:53.000000 nebula-loss-0.4.1/nebula_loss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 15:33:53.000000 nebula-loss-0.4.1/nebula_loss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 15:33:53.000000 nebula-loss-0.4.1/nebula_loss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 15:33:53.421637 nebula-loss-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-25 15:33:36.000000 nebula-loss-0.4.1/setup.py
```

### Comparing `nebula-loss-0.3.3/LICENSE` & `nebula-loss-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nebula-loss-0.3.3/PKG-INFO` & `nebula-loss-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nebula-loss
-Version: 0.3.3
+Version: 0.4.1
 Summary: 1 Loss Function to rule them all!
 Home-page: https://github.com/kyegomez/nebula
 Author: Agora
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,jax,loss ffunction,Multi-Modality AI
 Classifier: Development Status :: 4 - Beta
```

### Comparing `nebula-loss-0.3.3/nebula/nebulav2.py` & `nebula-loss-0.4.1/nebula/nebula.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import torch 
 import torch.nn as nn
 # import torch.jit
 import numpy as np
 
+import logging
+
 class LossFunction:
     def compute_Loss(self, y_pred, y_true):
         raise NotImplemented("compute_loss method must be implemented!")
     
 class L1Loss(LossFunction):
     def __init__(self):
         self.loss_function = nn.L1Loss()
@@ -73,55 +75,28 @@
     def __hash__(self):
         return hash((self.tensor_shape, self.tensor_dtype))
 
     def __eq__(self, other):
         return isinstance(other, HashableTensorWrapper) and self.tensor_shape == other.tensor_shape and self.tensor_dtype == other.tensor_dtype
 
 
-
-#detector helper function
-# def is_multi_label_classification(y_true: torch.Tensor):
-#     return y_true.shape[1] > 1 and y_true.dtype == torch.float
-
-#v2
 def is_multi_label_classification(y_true: torch.Tensor) -> bool:
     return len(y_true.shape) > 1 and y_true.shape[1] > 1 and y_true.dtype == torch.float
 
 
 def contains_non_negative_integers(y_true):
     return torch.all(y_true >= 0) and torch.all(y_true == y_true.to(torch.int64))
 
 def are_probability_distributions(y_pred, y_true):
     return torch.all(y_pred >= 0) and torch.all(y_pred <= 1) and torch.all(y_true >= 0) and torch.all(y_true <= 1) 
 
 def are_log_probabilities(y_pred):
     return torch.all(y_pred <= 0)
 
 
-#generate unique key for a tensor
-#v1
-# def generate_tensor_key(tensor):
-#     return (tuple(tensor.shape), str(tensor.dtype))
-
-#v2 
-# def generate_tensor_key(tensor):
-    # shape_tuple = ()
-    # for dim in tensor.shape:
-    #     shape_tuple += (dim.item(),)
-    # return (shape_tuple, str(tensor.dtype))
-
-
-#v3
-# def generate_tensor_key(tensor):
-#     shape_tuple = ()
-#     for dim in tensor.shape:
-#         shape_tuple += (dim,)
-#     return (shape_tuple, str(tensor.dtype))
-
-
 #v4 
 def generate_tensor_key(tensor):
     shape_tuple = ()
     for dim in tensor.shape:
         shape_tuple += (dim,)
     return (shape_tuple, str(tensor.dtype))
 
@@ -139,15 +114,23 @@
         self.loss_function = None
         self.domain_knowledge = domain_knowledge
         self.user_input = user_input 
         self.loss_function_cache = {}
         self.unique_values_cache = {}
         self.class_balance_cache = {}
 
+        self.logger = logging.getLogger(__name__)
+        self.logger.setLevel(logging.INFO)
+        handler = logging.StreamHandler()
+        handler.setFormatter(logging.Formatter('%(asctime)s - %(levelname)s - %(message)s'))
+        self.logger.addHandler(handler)
+
     def determine_loss_function(self, y_pred, y_true):
+        self.logger.info("Determining the loss function")
+
         is_classification = None
         dataset_id = id(y_true)
 
         # Cache unique values
         if dataset_id not in self.unique_values_cache:
             self.unique_values_cache[dataset_id] = torch.unique(y_true)
         unique_values = self.unique_values_cache[dataset_id]
@@ -220,64 +203,31 @@
             self.loss_function = KLDivLoss()
 
 
         #NLLLoss
         if is_classification and are_log_probabilities(y_pred):
             self.loss_function = NLLLoss()
 
-
-
-
         # SmotthL1Loss
         if is_classification is None:
             #check range of values in y_true
             if torch.min(y_true) >= 0 and torch.max(y_true) <= 1:
                 self.loss_function = SmoothL1Loss()
-        
-
 
         # Set the loss function based on the determined problem type
         if is_classification:
+            self.logger.info("Determined problem as classification. Using CrossEntropyLoss")
             self.loss_function = CrossEntropyLoss()
         else:
+            self.logger.info("Determining loss function for this dataset")
             self.loss_function = MSELoss()
-
-
-        
-
         
-    # @torch.jit.script #optimization jit 
     def compute_loss(self, y_pred, y_true):
-        #v2
-        # tensor_key = HashableTensorWrapper(y_true)
-        # if tensor_key not in self.loss_function_cache:
-        #     self.determine_loss_function(y_pred, y_true)
-        # return self.loss_function_cache[tensor_key](y_pred, y_true)
-    
-
-
         # V1
         dataset_id = id(y_true)
         if dataset_id not in self.loss_function_cache:
+            self.logger.info("Determining loss function for the dataset")
             self.determine_loss_function(y_pred, y_true)
             self.loss_function_cache[dataset_id] = self.loss_function
         
         cached_loss_function = self.loss_function_cache[dataset_id]
         return cached_loss_function.compute_loss(y_pred, y_true)
-
-        #v3
-        # tensor_key = generate_tensor_key(y_true)
-        # if tensor_key not in self.loss_function_cache:
-        #     self.determine_loss_function(y_pred, y_true)
-        # return self.loss_function_cache[tensor_key](y_pred, y_true)
-    
-    
-
-#move tensors nd model to gpu if available
-# device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-# y_pred, y_true = y_pred.to(device), y_true.to(device)
-
-
-# # #example usage with the pytorch autograd profiler
-# with torch.autograd.profiler.profile() as prof:
-#     loss = Nebula.compute_loss(y_pred, y_true)
-# print(prof.key_average().table())
```

### Comparing `nebula-loss-0.3.3/nebula_loss.egg-info/PKG-INFO` & `nebula-loss-0.4.1/nebula_loss.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nebula-loss
-Version: 0.3.3
+Version: 0.4.1
 Summary: 1 Loss Function to rule them all!
 Home-page: https://github.com/kyegomez/nebula
 Author: Agora
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,jax,loss ffunction,Multi-Modality AI
 Classifier: Development Status :: 4 - Beta
```

### Comparing `nebula-loss-0.3.3/setup.py` & `nebula-loss-0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'nebula-loss',
   packages = find_packages(exclude=[]),
-  version = '0.3.3',
+  version = '0.4.1',
   license='MIT',
   description = '1 Loss Function to rule them all!',
   author = 'Agora',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/nebula',
   keywords = [
```

