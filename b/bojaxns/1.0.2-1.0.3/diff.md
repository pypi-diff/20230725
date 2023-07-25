# Comparing `tmp/bojaxns-1.0.2.tar.gz` & `tmp/bojaxns-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bojaxns-1.0.2.tar", last modified: Mon Jul 24 01:33:45 2023, max compression
+gzip compressed data, was "bojaxns-1.0.3.tar", last modified: Tue Jul 25 15:41:28 2023, max compression
```

## Comparing `bojaxns-1.0.2.tar` & `bojaxns-1.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-24 01:33:45.080379 bojaxns-1.0.2/
--rw-rw-r--   0 albert    (1000) albert    (1000)     2553 2023-07-21 00:04:16.000000 bojaxns-1.0.2/LICENSE
--rw-rw-r--   0 albert    (1000) albert    (1000)     2259 2023-07-24 01:33:45.080379 bojaxns-1.0.2/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)     1806 2023-07-23 14:37:43.000000 bojaxns-1.0.2/README.md
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-24 01:33:45.080379 bojaxns-1.0.2/bojaxns/
--rw-rw-r--   0 albert    (1000) albert    (1000)      199 2023-07-21 00:04:16.000000 bojaxns-1.0.2/bojaxns/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5038 2023-07-21 00:04:16.000000 bojaxns-1.0.2/bojaxns/base.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2005 2023-07-21 12:38:12.000000 bojaxns-1.0.2/bojaxns/basic.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3282 2023-07-21 00:04:16.000000 bojaxns-1.0.2/bojaxns/experiment.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-24 01:33:45.080379 bojaxns-1.0.2/bojaxns/gaussian_process_formulation/
--rw-rw-r--   0 albert    (1000) albert    (1000)       70 2023-07-21 00:04:16.000000 bojaxns-1.0.2/bojaxns/gaussian_process_formulation/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    10665 2023-07-23 14:42:45.000000 bojaxns-1.0.2/bojaxns/gaussian_process_formulation/bayesian_optimiser.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    15665 2023-07-21 00:04:16.000000 bojaxns-1.0.2/bojaxns/gaussian_process_formulation/distribution_math.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     9088 2023-07-21 00:04:16.000000 bojaxns-1.0.2/bojaxns/gaussian_process_formulation/multi_step_lookahead.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-24 01:33:45.080379 bojaxns-1.0.2/bojaxns/gaussian_process_formulation/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-07-21 00:04:16.000000 bojaxns-1.0.2/bojaxns/gaussian_process_formulation/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     4904 2023-07-21 00:04:16.000000 bojaxns-1.0.2/bojaxns/gaussian_process_formulation/tests/test_bayesian_optimiser.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5939 2023-07-21 00:04:16.000000 bojaxns-1.0.2/bojaxns/gaussian_process_formulation/tests/test_distribution_maths.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5069 2023-07-21 00:04:16.000000 bojaxns-1.0.2/bojaxns/parameter_space.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     9505 2023-07-23 14:22:31.000000 bojaxns-1.0.2/bojaxns/service.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-24 01:33:45.080379 bojaxns-1.0.2/bojaxns/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-21 00:04:16.000000 bojaxns-1.0.2/bojaxns/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2181 2023-07-21 00:04:16.000000 bojaxns-1.0.2/bojaxns/tests/test_experiment.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3508 2023-07-21 00:04:16.000000 bojaxns-1.0.2/bojaxns/tests/test_parameter_space.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      622 2023-07-21 00:04:16.000000 bojaxns-1.0.2/bojaxns/tests/test_utils.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2986 2023-07-21 00:04:16.000000 bojaxns-1.0.2/bojaxns/utils.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-24 01:33:45.080379 bojaxns-1.0.2/bojaxns.egg-info/
--rw-rw-r--   0 albert    (1000) albert    (1000)     2259 2023-07-24 01:33:45.000000 bojaxns-1.0.2/bojaxns.egg-info/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)      894 2023-07-24 01:33:45.000000 bojaxns-1.0.2/bojaxns.egg-info/SOURCES.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-07-24 01:33:45.000000 bojaxns-1.0.2/bojaxns.egg-info/dependency_links.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        8 2023-07-24 01:33:45.000000 bojaxns-1.0.2/bojaxns.egg-info/top_level.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)      103 2023-07-21 00:04:16.000000 bojaxns-1.0.2/pyproject.toml
--rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-07-24 01:33:45.080379 bojaxns-1.0.2/setup.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)      961 2023-07-24 01:33:24.000000 bojaxns-1.0.2/setup.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-25 15:41:28.111423 bojaxns-1.0.3/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2553 2023-07-21 00:04:16.000000 bojaxns-1.0.3/LICENSE
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2259 2023-07-25 15:41:28.111423 bojaxns-1.0.3/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1806 2023-07-23 14:37:43.000000 bojaxns-1.0.3/README.md
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-25 15:41:28.111423 bojaxns-1.0.3/bojaxns/
+-rw-rw-r--   0 albert    (1000) albert    (1000)      199 2023-07-21 00:04:16.000000 bojaxns-1.0.3/bojaxns/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5038 2023-07-21 00:04:16.000000 bojaxns-1.0.3/bojaxns/base.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2005 2023-07-21 12:38:12.000000 bojaxns-1.0.3/bojaxns/basic.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3282 2023-07-21 00:04:16.000000 bojaxns-1.0.3/bojaxns/experiment.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-25 15:41:28.111423 bojaxns-1.0.3/bojaxns/gaussian_process_formulation/
+-rw-rw-r--   0 albert    (1000) albert    (1000)       70 2023-07-21 00:04:16.000000 bojaxns-1.0.3/bojaxns/gaussian_process_formulation/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    11415 2023-07-25 15:21:05.000000 bojaxns-1.0.3/bojaxns/gaussian_process_formulation/bayesian_optimiser.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    15665 2023-07-21 00:04:16.000000 bojaxns-1.0.3/bojaxns/gaussian_process_formulation/distribution_math.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     9088 2023-07-21 00:04:16.000000 bojaxns-1.0.3/bojaxns/gaussian_process_formulation/multi_step_lookahead.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-25 15:41:28.111423 bojaxns-1.0.3/bojaxns/gaussian_process_formulation/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-07-21 00:04:16.000000 bojaxns-1.0.3/bojaxns/gaussian_process_formulation/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5288 2023-07-25 15:21:05.000000 bojaxns-1.0.3/bojaxns/gaussian_process_formulation/tests/test_bayesian_optimiser.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5939 2023-07-21 00:04:16.000000 bojaxns-1.0.3/bojaxns/gaussian_process_formulation/tests/test_distribution_maths.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5069 2023-07-21 00:04:16.000000 bojaxns-1.0.3/bojaxns/parameter_space.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     9505 2023-07-23 14:22:31.000000 bojaxns-1.0.3/bojaxns/service.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-25 15:41:28.111423 bojaxns-1.0.3/bojaxns/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-07-21 00:04:16.000000 bojaxns-1.0.3/bojaxns/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2181 2023-07-21 00:04:16.000000 bojaxns-1.0.3/bojaxns/tests/test_experiment.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3508 2023-07-21 00:04:16.000000 bojaxns-1.0.3/bojaxns/tests/test_parameter_space.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      622 2023-07-21 00:04:16.000000 bojaxns-1.0.3/bojaxns/tests/test_utils.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2986 2023-07-21 00:04:16.000000 bojaxns-1.0.3/bojaxns/utils.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-25 15:41:28.111423 bojaxns-1.0.3/bojaxns.egg-info/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2259 2023-07-25 15:41:28.000000 bojaxns-1.0.3/bojaxns.egg-info/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)      894 2023-07-25 15:41:28.000000 bojaxns-1.0.3/bojaxns.egg-info/SOURCES.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-07-25 15:41:28.000000 bojaxns-1.0.3/bojaxns.egg-info/dependency_links.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        8 2023-07-25 15:41:28.000000 bojaxns-1.0.3/bojaxns.egg-info/top_level.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)      103 2023-07-21 00:04:16.000000 bojaxns-1.0.3/pyproject.toml
+-rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-07-25 15:41:28.111423 bojaxns-1.0.3/setup.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)      961 2023-07-25 15:21:05.000000 bojaxns-1.0.3/setup.py
```

### Comparing `bojaxns-1.0.2/LICENSE` & `bojaxns-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.2/PKG-INFO` & `bojaxns-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bojaxns
-Version: 1.0.2
+Version: 1.0.3
 Summary: Bayesian Optimisation with JAXNS
 Home-page: https://github.com/joshuaalbert/bojaxns
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `bojaxns-1.0.2/README.md` & `bojaxns-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.2/bojaxns/base.py` & `bojaxns-1.0.3/bojaxns/base.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.2/bojaxns/basic.py` & `bojaxns-1.0.3/bojaxns/basic.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.2/bojaxns/experiment.py` & `bojaxns-1.0.3/bojaxns/experiment.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.2/bojaxns/gaussian_process_formulation/bayesian_optimiser.py` & `bojaxns-1.0.3/bojaxns/gaussian_process_formulation/bayesian_optimiser.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,20 +28,37 @@
         self._data = self._prepare_data()
 
     def _prepare_data(self) -> GaussianProcessData:
         U = []
         Y = []
         Y_var = []
         sample_size = []
+
+        # handle nans ==> illegal value
+        min_val, max_val = np.inf, -np.inf
+        for trial_id, trial in self._experiment.trials.items():
+            for ref_id, trial_update in trial.trial_updates.items():
+                if not np.isfinite(trial_update.objective_measurement):
+                    continue
+                min_val = min(trial_update.objective_measurement, min_val)
+                max_val = max(trial_update.objective_measurement, max_val)
+
+        illegal_value = min_val - 0.1*(max_val - min_val)
+        if not np.isfinite(illegal_value):
+            illegal_value = 0.
+
         for trial_id, trial in self._experiment.trials.items():
             if len(trial.trial_updates) == 0:
                 continue
             samples = []
             for ref_id, trial_update in trial.trial_updates.items():
-                samples.append(trial_update.objective_measurement)
+                if not np.isfinite(trial_update.objective_measurement):
+                    samples.append(illegal_value)
+                else:
+                    samples.append(trial_update.objective_measurement)
             U.append(trial.U_value)
             Y.append(np.mean(samples))
             if len(samples) < 2:
                 Y_var.append(np.nan)
             else:
                 Y_var.append(np.var(samples))
             sample_size.append(len(samples))
```

### Comparing `bojaxns-1.0.2/bojaxns/gaussian_process_formulation/distribution_math.py` & `bojaxns-1.0.3/bojaxns/gaussian_process_formulation/distribution_math.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.2/bojaxns/gaussian_process_formulation/multi_step_lookahead.py` & `bojaxns-1.0.3/bojaxns/gaussian_process_formulation/multi_step_lookahead.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.2/bojaxns/gaussian_process_formulation/tests/test_bayesian_optimiser.py` & `bojaxns-1.0.3/bojaxns/gaussian_process_formulation/tests/test_bayesian_optimiser.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,14 +63,26 @@
                 trial_id=trial_id,
                 trial_update=TrialUpdate(ref_id='a', objective_measurement=obj_val)
             )
             # fig = bo_experiment.visualise()
             # plt.show()
             # plt.close('all')
 
+        trial_id = bo_experiment.create_new_trial(
+            key=random.PRNGKey(42),
+            random_explore=True
+        )
+        _ = bo_experiment.get_trial(trial_id=trial_id)
+
+        obj_val = float('nan')
+        bo_experiment.post_measurement(
+            trial_id=trial_id,
+            trial_update=TrialUpdate(ref_id='illegal', objective_measurement=obj_val)
+        )
+
     test_example(2)
 
 
 def test_bayesian_optimiser():
     parameter_space = ParameterSpace(parameters=[
         Parameter(
             name='churn_rate',
```

### Comparing `bojaxns-1.0.2/bojaxns/gaussian_process_formulation/tests/test_distribution_maths.py` & `bojaxns-1.0.3/bojaxns/gaussian_process_formulation/tests/test_distribution_maths.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.2/bojaxns/parameter_space.py` & `bojaxns-1.0.3/bojaxns/parameter_space.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.2/bojaxns/service.py` & `bojaxns-1.0.3/bojaxns/service.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.2/bojaxns/tests/test_experiment.py` & `bojaxns-1.0.3/bojaxns/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.2/bojaxns/tests/test_parameter_space.py` & `bojaxns-1.0.3/bojaxns/tests/test_parameter_space.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.2/bojaxns/tests/test_utils.py` & `bojaxns-1.0.3/bojaxns/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.2/bojaxns/utils.py` & `bojaxns-1.0.3/bojaxns/utils.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.2/bojaxns.egg-info/PKG-INFO` & `bojaxns-1.0.3/bojaxns.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bojaxns
-Version: 1.0.2
+Version: 1.0.3
 Summary: Bayesian Optimisation with JAXNS
 Home-page: https://github.com/joshuaalbert/bojaxns
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `bojaxns-1.0.2/bojaxns.egg-info/SOURCES.txt` & `bojaxns-1.0.3/bojaxns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

