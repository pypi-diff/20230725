# Comparing `tmp/xlogit-0.2.6.tar.gz` & `tmp/xlogit-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlogit-0.2.6.tar", last modified: Sat Jul 22 13:21:46 2023, max compression
+gzip compressed data, was "xlogit-0.2.7.tar", last modified: Tue Jul 25 13:55:10 2023, max compression
```

## Comparing `xlogit-0.2.6.tar` & `xlogit-0.2.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 das       (1000) das       (1000)        0 2023-07-22 13:21:46.608198 xlogit-0.2.6/
--rw-rw-r--   0 das       (1000) das       (1000)    35149 2022-03-23 01:15:13.000000 xlogit-0.2.6/LICENSE
--rw-rw-r--   0 das       (1000) das       (1000)    10383 2023-07-22 13:21:46.608198 xlogit-0.2.6/PKG-INFO
--rw-r--r--   0 das       (1000) das       (1000)    10041 2023-06-16 08:10:09.000000 xlogit-0.2.6/README.rst
--rw-rw-r--   0 das       (1000) das       (1000)       38 2023-07-22 13:21:46.608198 xlogit-0.2.6/setup.cfg
--rw-r--r--   0 das       (1000) das       (1000)      872 2023-07-22 13:17:34.000000 xlogit-0.2.6/setup.py
-drwxrwxr-x   0 das       (1000) das       (1000)        0 2023-07-22 13:21:46.608198 xlogit-0.2.6/tests/
--rwxr-xr-x   0 das       (1000) das       (1000)     3091 2022-06-11 06:21:48.000000 xlogit-0.2.6/tests/test__choice_model.py
--rwxrwxr-x   0 das       (1000) das       (1000)     1761 2022-06-01 07:42:17.000000 xlogit-0.2.6/tests/test__device.py
--rw-rw-r--   0 das       (1000) das       (1000)     5214 2023-06-16 03:10:49.000000 xlogit-0.2.6/tests/test_mixed_logit.py
--rwxrwxr-x   0 das       (1000) das       (1000)     3518 2023-06-16 03:10:49.000000 xlogit-0.2.6/tests/test_multinomial_logit.py
--rwxrwxr-x   0 das       (1000) das       (1000)     1940 2022-06-25 05:26:01.000000 xlogit-0.2.6/tests/test_utils.py
-drwxrwxr-x   0 das       (1000) das       (1000)        0 2023-07-22 13:21:46.608198 xlogit-0.2.6/xlogit/
--rw-rw-r--   0 das       (1000) das       (1000)      112 2022-03-23 01:15:13.000000 xlogit-0.2.6/xlogit/__init__.py
--rwxrwxr-x   0 das       (1000) das       (1000)    11115 2023-06-16 03:10:49.000000 xlogit-0.2.6/xlogit/_choice_model.py
--rwxrwxr-x   0 das       (1000) das       (1000)     1983 2022-06-01 05:55:09.000000 xlogit-0.2.6/xlogit/_device.py
--rw-r--r--   0 das       (1000) das       (1000)     3098 2022-06-25 05:00:58.000000 xlogit-0.2.6/xlogit/_optimize.py
--rw-rw-r--   0 das       (1000) das       (1000)    32208 2023-07-22 13:16:15.000000 xlogit-0.2.6/xlogit/mixed_logit.py
--rw-rw-r--   0 das       (1000) das       (1000)    14106 2023-07-22 13:16:15.000000 xlogit-0.2.6/xlogit/multinomial_logit.py
--rwxrwxr-x   0 das       (1000) das       (1000)     3851 2022-06-25 05:23:47.000000 xlogit-0.2.6/xlogit/utils.py
-drwxrwxr-x   0 das       (1000) das       (1000)        0 2023-07-22 13:21:46.608198 xlogit-0.2.6/xlogit.egg-info/
--rw-r--r--   0 das       (1000) das       (1000)    10383 2023-07-22 13:21:46.000000 xlogit-0.2.6/xlogit.egg-info/PKG-INFO
--rw-r--r--   0 das       (1000) das       (1000)      480 2023-07-22 13:21:46.000000 xlogit-0.2.6/xlogit.egg-info/SOURCES.txt
--rw-r--r--   0 das       (1000) das       (1000)        1 2023-07-22 13:21:46.000000 xlogit-0.2.6/xlogit.egg-info/dependency_links.txt
--rw-r--r--   0 das       (1000) das       (1000)        1 2022-06-25 05:41:05.000000 xlogit-0.2.6/xlogit.egg-info/not-zip-safe
--rw-r--r--   0 das       (1000) das       (1000)       27 2023-07-22 13:21:46.000000 xlogit-0.2.6/xlogit.egg-info/requires.txt
--rw-r--r--   0 das       (1000) das       (1000)        7 2023-07-22 13:21:46.000000 xlogit-0.2.6/xlogit.egg-info/top_level.txt
+drwxrwxr-x   0 das       (1000) das       (1000)        0 2023-07-25 13:55:10.653560 xlogit-0.2.7/
+-rw-rw-r--   0 das       (1000) das       (1000)    35149 2022-03-23 01:15:13.000000 xlogit-0.2.7/LICENSE
+-rw-rw-r--   0 das       (1000) das       (1000)    10383 2023-07-25 13:55:10.653560 xlogit-0.2.7/PKG-INFO
+-rw-r--r--   0 das       (1000) das       (1000)    10041 2023-06-16 08:10:09.000000 xlogit-0.2.7/README.rst
+-rw-rw-r--   0 das       (1000) das       (1000)       38 2023-07-25 13:55:10.653560 xlogit-0.2.7/setup.cfg
+-rw-r--r--   0 das       (1000) das       (1000)      872 2023-07-25 13:49:05.000000 xlogit-0.2.7/setup.py
+drwxrwxr-x   0 das       (1000) das       (1000)        0 2023-07-25 13:55:10.653560 xlogit-0.2.7/tests/
+-rwxr-xr-x   0 das       (1000) das       (1000)     3091 2022-06-11 06:21:48.000000 xlogit-0.2.7/tests/test__choice_model.py
+-rwxrwxr-x   0 das       (1000) das       (1000)     1761 2022-06-01 07:42:17.000000 xlogit-0.2.7/tests/test__device.py
+-rw-rw-r--   0 das       (1000) das       (1000)     5214 2023-06-16 03:10:49.000000 xlogit-0.2.7/tests/test_mixed_logit.py
+-rwxrwxr-x   0 das       (1000) das       (1000)     3518 2023-06-16 03:10:49.000000 xlogit-0.2.7/tests/test_multinomial_logit.py
+-rwxrwxr-x   0 das       (1000) das       (1000)     1940 2022-06-25 05:26:01.000000 xlogit-0.2.7/tests/test_utils.py
+drwxrwxr-x   0 das       (1000) das       (1000)        0 2023-07-25 13:55:10.653560 xlogit-0.2.7/xlogit/
+-rw-rw-r--   0 das       (1000) das       (1000)      112 2022-03-23 01:15:13.000000 xlogit-0.2.7/xlogit/__init__.py
+-rwxrwxr-x   0 das       (1000) das       (1000)    11115 2023-06-16 03:10:49.000000 xlogit-0.2.7/xlogit/_choice_model.py
+-rwxrwxr-x   0 das       (1000) das       (1000)     1983 2022-06-01 05:55:09.000000 xlogit-0.2.7/xlogit/_device.py
+-rw-r--r--   0 das       (1000) das       (1000)     3098 2022-06-25 05:00:58.000000 xlogit-0.2.7/xlogit/_optimize.py
+-rw-rw-r--   0 das       (1000) das       (1000)    32251 2023-07-25 13:43:54.000000 xlogit-0.2.7/xlogit/mixed_logit.py
+-rw-rw-r--   0 das       (1000) das       (1000)    14118 2023-07-25 13:32:30.000000 xlogit-0.2.7/xlogit/multinomial_logit.py
+-rwxrwxr-x   0 das       (1000) das       (1000)     3851 2022-06-25 05:23:47.000000 xlogit-0.2.7/xlogit/utils.py
+drwxrwxr-x   0 das       (1000) das       (1000)        0 2023-07-25 13:55:10.653560 xlogit-0.2.7/xlogit.egg-info/
+-rw-r--r--   0 das       (1000) das       (1000)    10383 2023-07-25 13:55:10.000000 xlogit-0.2.7/xlogit.egg-info/PKG-INFO
+-rw-r--r--   0 das       (1000) das       (1000)      480 2023-07-25 13:55:10.000000 xlogit-0.2.7/xlogit.egg-info/SOURCES.txt
+-rw-r--r--   0 das       (1000) das       (1000)        1 2023-07-25 13:55:10.000000 xlogit-0.2.7/xlogit.egg-info/dependency_links.txt
+-rw-r--r--   0 das       (1000) das       (1000)        1 2022-06-25 05:41:05.000000 xlogit-0.2.7/xlogit.egg-info/not-zip-safe
+-rw-r--r--   0 das       (1000) das       (1000)       27 2023-07-25 13:55:10.000000 xlogit-0.2.7/xlogit.egg-info/requires.txt
+-rw-r--r--   0 das       (1000) das       (1000)        7 2023-07-25 13:55:10.000000 xlogit-0.2.7/xlogit.egg-info/top_level.txt
```

### Comparing `xlogit-0.2.6/LICENSE` & `xlogit-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xlogit-0.2.6/PKG-INFO` & `xlogit-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xlogit
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Python package for GPU-accelerated estimation of mixed logit models.
 Home-page: https://github.com/arteagac/xlogit
 Author: Cristian Arteaga
 Author-email: cristiandavidarteaga@gmail.com
 License: MIT
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
```

### Comparing `xlogit-0.2.6/README.rst` & `xlogit-0.2.7/README.rst`

 * *Files identical despite different names*

### Comparing `xlogit-0.2.6/setup.py` & `xlogit-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 import codecs
 
 with codecs.open('README.rst', encoding='utf8') as fh:
     long_description = fh.read()
 
 setuptools.setup(name='xlogit',
-                 version='0.2.6',
+                 version='0.2.7',
                  description='A Python package for GPU-accelerated ' +
                  'estimation of mixed logit models.',
                  long_description=long_description,
                  long_description_content_type="text/x-rst",
                  url='https://github.com/arteagac/xlogit',
                  author='Cristian Arteaga',
                  author_email='cristiandavidarteaga@gmail.com',
```

### Comparing `xlogit-0.2.6/tests/test__choice_model.py` & `xlogit-0.2.7/tests/test__choice_model.py`

 * *Files identical despite different names*

### Comparing `xlogit-0.2.6/tests/test__device.py` & `xlogit-0.2.7/tests/test__device.py`

 * *Files identical despite different names*

### Comparing `xlogit-0.2.6/tests/test_mixed_logit.py` & `xlogit-0.2.7/tests/test_mixed_logit.py`

 * *Files identical despite different names*

### Comparing `xlogit-0.2.6/tests/test_multinomial_logit.py` & `xlogit-0.2.7/tests/test_multinomial_logit.py`

 * *Files identical despite different names*

### Comparing `xlogit-0.2.6/tests/test_utils.py` & `xlogit-0.2.7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `xlogit-0.2.6/xlogit/_choice_model.py` & `xlogit-0.2.7/xlogit/_choice_model.py`

 * *Files identical despite different names*

### Comparing `xlogit-0.2.6/xlogit/_device.py` & `xlogit-0.2.7/xlogit/_device.py`

 * *Files identical despite different names*

### Comparing `xlogit-0.2.6/xlogit/_optimize.py` & `xlogit-0.2.7/xlogit/_optimize.py`

 * *Files identical despite different names*

### Comparing `xlogit-0.2.6/xlogit/mixed_logit.py` & `xlogit-0.2.7/xlogit/mixed_logit.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
 
         self._validate_inputs(X, y, alts, varnames, isvars, ids, weights)
 
         if mnl_init and init_coeff is None:
             # Initialize coefficients using a multinomial logit model
             mnl = MultinomialLogit()
             mnl.fit(X, y, varnames, alts, ids, isvars=isvars, weights=weights, addit=addit,
-                    avail=avail, base_alt=base_alt, fit_intercept=fit_intercept)
+                    avail=avail, base_alt=base_alt, fit_intercept=fit_intercept, skip_std_errs=True)
             init_coeff = np.concatenate((mnl.coeff_, np.repeat(.1, len(randvars))))
             init_coeff = init_coeff if scale_factor is None else np.append(init_coeff, 1.)
 
         self._pre_fit(alts, varnames, isvars, base_alt, fit_intercept, maxiter)
 
         betas, X, y, panels, draws, weights, avail, Xnames, scale, addit = \
             self._setup_input_data(X, y, varnames, alts, ids, randvars, isvars=isvars, weights=weights, avail=avail,
@@ -215,21 +215,23 @@
 
         coef_names = np.append(Xnames, np.char.add("sd.", Xnames[self._rvidx]))
 
         if scale_factor is not None:
             coef_names = np.append(coef_names, "_scale_factor")
 
         num_hess = num_hess if scale_factor is None else True
+
         if optim_method == "L-BFGS-B":
             optim_res['grad_n'] = self._loglik_gradient(optim_res['x'], *fargs, return_gradient=True)[2]
 
-        if (num_hess or optim_method == "L-BFGS-B") and not skip_std_errs:
-            optim_res['hess_inv'] = _numerical_hessian(optim_res['x'], self._loglik_gradient, args=fargs)
-        else:
+        if skip_std_errs:
             optim_res['hess_inv'] = np.eye(len(optim_res['x']))
+        else:
+            if num_hess or optim_method == "L-BFGS-B":
+                optim_res['hess_inv'] = _numerical_hessian(optim_res['x'], self._loglik_gradient, args=fargs)            
 
         self._post_fit(optim_res, coef_names, X.shape[0], verbose, robust)
 
 
 
     def predict(self, X, varnames, alts, ids, isvars=None, weights=None, avail=None,  panels=None, random_state=None,
                 n_draws=1000, halton=True, verbose=1, batch_size=None, return_proba=False, return_freq=False,
```

### Comparing `xlogit-0.2.6/xlogit/multinomial_logit.py` & `xlogit-0.2.7/xlogit/multinomial_logit.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         bic : float
             Bayesian information criteria of the estimated model
     """
 
     def fit(self, X, y, varnames, alts, ids, isvars=None,
             weights=None, avail=None, base_alt=None, fit_intercept=False,
             init_coeff=None, maxiter=2000, random_state=None, tol_opts=None,
-            verbose=1, robust=False, num_hess=False, scale_factor=None,
+            verbose=1, robust=False, num_hess=True, scale_factor=None,
             addit=None, skip_std_errs=False):
         """Fit multinomial and/or conditional logit models.
 
         Parameters
         ----------
         X : array-like, shape (n_samples*n_alts, n_variables)
             Input data for explanatory variables in long format
@@ -157,18 +157,20 @@
         fargs = (Xd, scale_d, addit_d, weights, avail)
         optim_res = _minimize(self._loglik_gradient, betas, args=fargs, method="BFGS", tol=tol['ftol'],
                               options={'maxiter': maxiter, 'disp': verbose > 1})
         coef_names = Xnames
         if scale_factor is not None:
             coef_names = np.append(coef_names, "_scale_factor")
 
-        if num_hess and not skip_std_errs:
-            optim_res['hess_inv'] = _numerical_hessian(optim_res['x'], self._loglik_gradient, args=fargs)
-        else:
+        if skip_std_errs:
             optim_res['hess_inv'] = np.eye(len(optim_res['x']))
+        else:
+            if num_hess:
+                optim_res['hess_inv'] = _numerical_hessian(optim_res['x'], self._loglik_gradient, args=fargs)
+
         self._post_fit(optim_res, coef_names, X.shape[0], verbose, robust)
 
 
     def predict(self, X, varnames, alts, ids, isvars=None, weights=None,
                 avail=None, random_state=None, verbose=1,
                 return_proba=False, return_freq=False, scale_factor=None, addit=None):
         """Predict chosen alternatives.
```

### Comparing `xlogit-0.2.6/xlogit/utils.py` & `xlogit-0.2.7/xlogit/utils.py`

 * *Files identical despite different names*

### Comparing `xlogit-0.2.6/xlogit.egg-info/PKG-INFO` & `xlogit-0.2.7/xlogit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xlogit
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Python package for GPU-accelerated estimation of mixed logit models.
 Home-page: https://github.com/arteagac/xlogit
 Author: Cristian Arteaga
 Author-email: cristiandavidarteaga@gmail.com
 License: MIT
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
```

