# Comparing `tmp/stable-trunc-gaussian-1.0.0.tar.gz` & `tmp/stable-trunc-gaussian-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stable-trunc-gaussian-1.0.0.tar", last modified: Tue Jul 25 18:32:47 2023, max compression
+gzip compressed data, was "stable-trunc-gaussian-1.0.1.tar", last modified: Tue Jul 25 20:54:32 2023, max compression
```

## Comparing `stable-trunc-gaussian-1.0.0.tar` & `stable-trunc-gaussian-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-07-25 18:32:47.832806 stable-trunc-gaussian-1.0.0/
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     1078 2023-07-25 17:33:32.000000 stable-trunc-gaussian-1.0.0/LICENSE
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       38 2023-07-25 18:10:36.000000 stable-trunc-gaussian-1.0.0/MANIFEST.in
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     3288 2023-07-25 18:32:47.832806 stable-trunc-gaussian-1.0.0/PKG-INFO
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     1438 2023-07-25 18:29:45.000000 stable-trunc-gaussian-1.0.0/README.md
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)      799 2023-07-25 18:10:31.000000 stable-trunc-gaussian-1.0.0/pyproject.toml
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       38 2023-07-25 18:32:47.832806 stable-trunc-gaussian-1.0.0/setup.cfg
-drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-07-25 18:32:47.832806 stable-trunc-gaussian-1.0.0/src/
-drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-07-25 18:32:47.832806 stable-trunc-gaussian-1.0.0/src/stable_trunc_gaussian/
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       73 2023-07-25 18:13:30.000000 stable-trunc-gaussian-1.0.0/src/stable_trunc_gaussian/__init__.py
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     6934 2023-07-25 17:33:32.000000 stable-trunc-gaussian-1.0.0/src/stable_trunc_gaussian/src.py
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     4082 2023-07-25 17:33:32.000000 stable-trunc-gaussian-1.0.0/src/stable_trunc_gaussian/tests.py
-drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-07-25 18:32:47.832806 stable-trunc-gaussian-1.0.0/src/stable_trunc_gaussian.egg-info/
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     3288 2023-07-25 18:32:47.000000 stable-trunc-gaussian-1.0.0/src/stable_trunc_gaussian.egg-info/PKG-INFO
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)      394 2023-07-25 18:32:47.000000 stable-trunc-gaussian-1.0.0/src/stable_trunc_gaussian.egg-info/SOURCES.txt
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)        1 2023-07-25 18:32:47.000000 stable-trunc-gaussian-1.0.0/src/stable_trunc_gaussian.egg-info/dependency_links.txt
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       20 2023-07-25 18:32:47.000000 stable-trunc-gaussian-1.0.0/src/stable_trunc_gaussian.egg-info/requires.txt
--rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       22 2023-07-25 18:32:47.000000 stable-trunc-gaussian-1.0.0/src/stable_trunc_gaussian.egg-info/top_level.txt
+drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-07-25 20:54:32.589043 stable-trunc-gaussian-1.0.1/
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     1078 2023-07-25 17:33:32.000000 stable-trunc-gaussian-1.0.1/LICENSE
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       38 2023-07-25 18:10:36.000000 stable-trunc-gaussian-1.0.1/MANIFEST.in
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     3407 2023-07-25 20:54:32.589043 stable-trunc-gaussian-1.0.1/PKG-INFO
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     1557 2023-07-25 18:41:21.000000 stable-trunc-gaussian-1.0.1/README.md
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)      799 2023-07-25 20:47:54.000000 stable-trunc-gaussian-1.0.1/pyproject.toml
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       38 2023-07-25 20:54:32.589043 stable-trunc-gaussian-1.0.1/setup.cfg
+drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-07-25 20:54:32.589043 stable-trunc-gaussian-1.0.1/src/
+drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-07-25 20:54:32.589043 stable-trunc-gaussian-1.0.1/src/stable_trunc_gaussian/
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       73 2023-07-25 20:47:19.000000 stable-trunc-gaussian-1.0.1/src/stable_trunc_gaussian/__init__.py
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     7319 2023-07-25 20:46:56.000000 stable-trunc-gaussian-1.0.1/src/stable_trunc_gaussian/src.py
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     4085 2023-07-25 20:50:46.000000 stable-trunc-gaussian-1.0.1/src/stable_trunc_gaussian/tests.py
+drwxrwxr-x   0 aeryan    (1000) aeryan    (1000)        0 2023-07-25 20:54:32.589043 stable-trunc-gaussian-1.0.1/src/stable_trunc_gaussian.egg-info/
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)     3407 2023-07-25 20:54:32.000000 stable-trunc-gaussian-1.0.1/src/stable_trunc_gaussian.egg-info/PKG-INFO
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)      394 2023-07-25 20:54:32.000000 stable-trunc-gaussian-1.0.1/src/stable_trunc_gaussian.egg-info/SOURCES.txt
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)        1 2023-07-25 20:54:32.000000 stable-trunc-gaussian-1.0.1/src/stable_trunc_gaussian.egg-info/dependency_links.txt
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       20 2023-07-25 20:54:32.000000 stable-trunc-gaussian-1.0.1/src/stable_trunc_gaussian.egg-info/requires.txt
+-rw-rw-r--   0 aeryan    (1000) aeryan    (1000)       22 2023-07-25 20:54:32.000000 stable-trunc-gaussian-1.0.1/src/stable_trunc_gaussian.egg-info/top_level.txt
```

### Comparing `stable-trunc-gaussian-1.0.0/LICENSE` & `stable-trunc-gaussian-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stable-trunc-gaussian-1.0.0/PKG-INFO` & `stable-trunc-gaussian-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-trunc-gaussian
-Version: 1.0.0
+Version: 1.0.1
 Summary: A numerically-stable and differentiable implementation of the Truncated Gaussian distribution in Pytorch.
 Author-email: Carlos Núñez Molina <ccaarlos@ugr.es>
 License: MIT License
         
         Copyright (c) 2023 Carlos Núñez Molina
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,14 +30,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
+[![PyPI version](https://badge.fury.io/py/stable-trunc-gaussian.svg)](https://badge.fury.io/py/stable-trunc-gaussian)
+
 # Stable Truncated Gaussian
 A **differentiable** implementation of the **Truncated Gaussian (Normal)** distribution using Python and Pytorch, which is **numerically stable** even when the *μ* parameter lies outside the interval *\[a,b\]* given by the bounds of the distribution. In this situation, a naive evaluation of the mean, variance and log-probability of the distribution could otherwise result in [catastrophic cancellation](https://en.wikipedia.org/wiki/Catastrophic_cancellation). Our code is inspired by [TruncatedNormal.jl](https://github.com/cossio/TruncatedNormal.jl) and [torch_truncnorm](https://github.com/toshas/torch_truncnorm). Currently, we only provide functionality for calculating the mean, variance and log-probability, but not for calculating the entropy or sampling from the distribution.
 
 ## Installation
 
 Simply install with `pip`:
```

### Comparing `stable-trunc-gaussian-1.0.0/README.md` & `stable-trunc-gaussian-1.0.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![PyPI version](https://badge.fury.io/py/stable-trunc-gaussian.svg)](https://badge.fury.io/py/stable-trunc-gaussian)
+
 # Stable Truncated Gaussian
 A **differentiable** implementation of the **Truncated Gaussian (Normal)** distribution using Python and Pytorch, which is **numerically stable** even when the *μ* parameter lies outside the interval *\[a,b\]* given by the bounds of the distribution. In this situation, a naive evaluation of the mean, variance and log-probability of the distribution could otherwise result in [catastrophic cancellation](https://en.wikipedia.org/wiki/Catastrophic_cancellation). Our code is inspired by [TruncatedNormal.jl](https://github.com/cossio/TruncatedNormal.jl) and [torch_truncnorm](https://github.com/toshas/torch_truncnorm). Currently, we only provide functionality for calculating the mean, variance and log-probability, but not for calculating the entropy or sampling from the distribution.
 
 ## Installation
 
 Simply install with `pip`:
```

### Comparing `stable-trunc-gaussian-1.0.0/pyproject.toml` & `stable-trunc-gaussian-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="stable-trunc-gaussian"
-version="1.0.0"
+version="1.0.1"
 description="A numerically-stable and differentiable implementation of the Truncated Gaussian distribution in Pytorch."
 readme="README.md"
 authors = [{ name = "Carlos Núñez Molina", email = "ccaarlos@ugr.es" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `stable-trunc-gaussian-1.0.0/src/stable_trunc_gaussian/src.py` & `stable-trunc-gaussian-1.0.1/src/stable_trunc_gaussian/src.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,27 +38,28 @@
 	"""
 	Constructor
 		@mu Mu parameter, corresponding to the mean of the gaussian <before> truncation
 		@sigma Sigma parameter, corresponding to the standard deviation of the gaussian <before> truncation
 		@a Lower bound
 		@b Upper bound
 
-		All parameters must be instances of torch.Tensor.
+		All parameters must be instances of torch.Tensor with a single value (i.e., be of dimension 0). 
 	"""
 	def __init__(self, mu, sigma, a, b):
 		# Safety checks
+		if not (isinstance(mu, torch.Tensor) and isinstance(sigma, torch.Tensor) and isinstance(a, torch.Tensor) \
+			and isinstance(b, torch.Tensor)):
+			raise ValueError("All the parameters must be instances of torch.Tensor")	
+		if not (mu.dim() == 0 and sigma.dim() == 0 and a.dim() == 0 and b.dim() == 0):
+			raise ValueError("All the parameters must be tensors containing a single value (i.e., of dimension 0)")	
 		if sigma <= 0:
 			raise ValueError("sigma must be greater than 0")
 		if a >= b:
 			raise ValueError("parameter 'a' (lower bound) must be smaller than 'b' (upper bound)")       
-		
-		if not (isinstance(mu, torch.Tensor) and isinstance(sigma, torch.Tensor) and isinstance(a, torch.Tensor) \
-				and isinstance(b, torch.Tensor)):
-			raise ValueError("All the parameters must be instances of torch.Tensor")
-		
+			
 		self._mu = mu
 		self._sigma = sigma
 		self._a = a
 		self._b = b
 		self._alpha = (self._a-self._mu)/self._sigma
 		self._beta = (self._b-self._mu)/self._sigma
 
@@ -205,22 +206,24 @@
 
 		return result
 	
 	@property
 	def variance(self):
 		return self._variance
 	
-	# Log probability of some value x under the truncated gaussian
+	# Log probability of some value(s) x under the truncated gaussian
+	# Unlike the parameters of the distributions, we allow x to be a tensor of arbitrary size
+	# (e.g., x=torch.tensor([0,1,2]))
 	def log_prob(self, x):
 		# Check that x is a tensor
 		if not isinstance(x, torch.Tensor):
 			raise ValueError("parameter 'x' must be an instance of torch.Tensor") 
 
 		# x must be inside the interval [a, b]
-		if x < self._a or x > self._b:
+		if torch.any(x < self._a) or torch.any(x > self._b):
 			raise ValueError(f"parameter 'x' ({x}) is outside the [a={self._a}, b={self._b}] interval")
 
 		xi = (x-self._mu)/self._sigma
 		term_1 = -torch.log(self._sigma)
 		term_2 = -LOG_SQRT_2_PI - (xi**2)/2    
 		term_3 = -self._log_Z
 		result = term_1 + term_2 + term_3
```

### Comparing `stable-trunc-gaussian-1.0.0/src/stable_trunc_gaussian/tests.py` & `stable-trunc-gaussian-1.0.1/src/stable_trunc_gaussian/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Tests for truncated gaussian
 # I compare the values obtained with my code against those returned by scipy.stats.truncnorm
 
-from truncated_gaussian import TruncatedGaussian as TG
+from stable_trunc_gaussian import TruncatedGaussian as TG
 from scipy.stats import truncnorm
 from torch import tensor as t
 import math
 
 """
 Current results:
     - Variance calculation seems to differ sometimes with scipy.
```

### Comparing `stable-trunc-gaussian-1.0.0/src/stable_trunc_gaussian.egg-info/PKG-INFO` & `stable-trunc-gaussian-1.0.1/src/stable_trunc_gaussian.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-trunc-gaussian
-Version: 1.0.0
+Version: 1.0.1
 Summary: A numerically-stable and differentiable implementation of the Truncated Gaussian distribution in Pytorch.
 Author-email: Carlos Núñez Molina <ccaarlos@ugr.es>
 License: MIT License
         
         Copyright (c) 2023 Carlos Núñez Molina
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,14 +30,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
+[![PyPI version](https://badge.fury.io/py/stable-trunc-gaussian.svg)](https://badge.fury.io/py/stable-trunc-gaussian)
+
 # Stable Truncated Gaussian
 A **differentiable** implementation of the **Truncated Gaussian (Normal)** distribution using Python and Pytorch, which is **numerically stable** even when the *μ* parameter lies outside the interval *\[a,b\]* given by the bounds of the distribution. In this situation, a naive evaluation of the mean, variance and log-probability of the distribution could otherwise result in [catastrophic cancellation](https://en.wikipedia.org/wiki/Catastrophic_cancellation). Our code is inspired by [TruncatedNormal.jl](https://github.com/cossio/TruncatedNormal.jl) and [torch_truncnorm](https://github.com/toshas/torch_truncnorm). Currently, we only provide functionality for calculating the mean, variance and log-probability, but not for calculating the entropy or sampling from the distribution.
 
 ## Installation
 
 Simply install with `pip`:
```

