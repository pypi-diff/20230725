# Comparing `tmp/mcmc2ndgen-0.0.3.tar.gz` & `tmp/mcmc2ndgen-0.0.4.tar.gz`

## Comparing `mcmc2ndgen-0.0.3.tar` & `mcmc2ndgen-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.3/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.3/__init__.py
--rwxr-xr-x   0        0        0    13695 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.3/mcmc2ndgen.py
--rw-r--r--   0        0        0     6391 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.3/settings.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.3/data/.gitattributes
--rw-r--r--   0        0        0 12398714 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.3/data/LISA_Instrument_ESA_orbits_tcb_orbits_4_Hz_3600_sec.dat
--rw-r--r--   0        0        0 21008794 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.3/data/LISA_Instrument_Keplerian_orbits_ppr_orbits_4_Hz_3600_sec.dat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.3/data/__init__.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.3/data/elements_from_Cartesian_4_Hz_3600_sec.dat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.3/examples/__init__.py
--rw-r--r--   0        0        0    11622 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.3/examples/elements_from_Cartesian.ipynb
--rw-r--r--   0        0        0    16668 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.3/examples/example_mcmc_run.ipynb
--rw-r--r--   0        0        0    49202 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.3/examples/generate_data-ESA.ipynb
--rw-r--r--   0        0        0    49601 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.3/examples/generate_data_Keplerian.ipynb
--rw-r--r--   0        0        0    16668 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.3/examples/.ipynb_checkpoints/example_mcmc_run-checkpoint.ipynb
--rw-r--r--   0        0        0    49202 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.3/examples/.ipynb_checkpoints/generate_data-ESA-checkpoint.ipynb
--rw-r--r--   0        0        0    49889 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.3/examples/.ipynb_checkpoints/generate_data_Keplerian-checkpoint.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0    25001 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.3/utils/TDI_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.3/utils/__init__.py
--rw-r--r--   0        0        0     5505 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.3/utils/delay_time_dependence.py
--rw-r--r--   0        0        0     9353 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.3/utils/delay_time_dependence_Keplerian.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.3/utils/filter_functions.py
--rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.3/utils/mcmc_functions.py
--rw-r--r--   0        0        0     6527 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.3/utils/mcmc_functions_Keplerian.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.3/LICENSE
--rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.3/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.4/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.4/__init__.py
+-rwxr-xr-x   0        0        0    13695 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.4/mcmc2ndgen.py
+-rw-r--r--   0        0        0     6391 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.4/settings.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.4/data/.gitattributes
+-rw-r--r--   0        0        0 12398714 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.4/data/LISA_Instrument_ESA_orbits_tcb_orbits_4_Hz_3600_sec.dat
+-rw-r--r--   0        0        0 21008794 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.4/data/LISA_Instrument_Keplerian_orbits_ppr_orbits_4_Hz_3600_sec.dat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.4/data/__init__.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.4/data/elements_from_Cartesian_4_Hz_3600_sec.dat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.4/examples/__init__.py
+-rw-r--r--   0        0        0    11622 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.4/examples/elements_from_Cartesian.ipynb
+-rw-r--r--   0        0        0    16668 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.4/examples/example_mcmc_run.ipynb
+-rw-r--r--   0        0        0    49202 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.4/examples/generate_data-ESA.ipynb
+-rw-r--r--   0        0        0    49601 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.4/examples/generate_data_Keplerian.ipynb
+-rw-r--r--   0        0        0    16668 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.4/examples/.ipynb_checkpoints/example_mcmc_run-checkpoint.ipynb
+-rw-r--r--   0        0        0    49202 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.4/examples/.ipynb_checkpoints/generate_data-ESA-checkpoint.ipynb
+-rw-r--r--   0        0        0    49889 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.4/examples/.ipynb_checkpoints/generate_data_Keplerian-checkpoint.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0    25001 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.4/utils/TDI_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.4/utils/__init__.py
+-rw-r--r--   0        0        0     5505 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.4/utils/delay_time_dependence.py
+-rw-r--r--   0        0        0     9353 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.4/utils/delay_time_dependence_Keplerian.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.4/utils/filter_functions.py
+-rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.4/utils/mcmc_functions.py
+-rw-r--r--   0        0        0     6527 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.4/utils/mcmc_functions_Keplerian.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.4/README.md
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 mcmc2ndgen-0.0.4/PKG-INFO
```

### Comparing `mcmc2ndgen-0.0.3/.DS_Store` & `mcmc2ndgen-0.0.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `mcmc2ndgen-0.0.3/mcmc2ndgen.py` & `mcmc2ndgen-0.0.4/mcmc2ndgen.py`

 * *Files identical despite different names*

### Comparing `mcmc2ndgen-0.0.3/settings.py` & `mcmc2ndgen-0.0.4/settings.py`

 * *Files identical despite different names*

### Comparing `mcmc2ndgen-0.0.3/data/LISA_Instrument_ESA_orbits_tcb_orbits_4_Hz_3600_sec.dat` & `mcmc2ndgen-0.0.4/data/LISA_Instrument_ESA_orbits_tcb_orbits_4_Hz_3600_sec.dat`

 * *Files identical despite different names*

### Comparing `mcmc2ndgen-0.0.3/data/LISA_Instrument_Keplerian_orbits_ppr_orbits_4_Hz_3600_sec.dat` & `mcmc2ndgen-0.0.4/data/LISA_Instrument_Keplerian_orbits_ppr_orbits_4_Hz_3600_sec.dat`

 * *Files identical despite different names*

### Comparing `mcmc2ndgen-0.0.3/data/elements_from_Cartesian_4_Hz_3600_sec.dat` & `mcmc2ndgen-0.0.4/data/elements_from_Cartesian_4_Hz_3600_sec.dat`

 * *Files identical despite different names*

### Comparing `mcmc2ndgen-0.0.3/examples/elements_from_Cartesian.ipynb` & `mcmc2ndgen-0.0.4/examples/elements_from_Cartesian.ipynb`

 * *Files identical despite different names*

### Comparing `mcmc2ndgen-0.0.3/examples/example_mcmc_run.ipynb` & `mcmc2ndgen-0.0.4/examples/example_mcmc_run.ipynb`

 * *Files identical despite different names*

### Comparing `mcmc2ndgen-0.0.3/examples/generate_data-ESA.ipynb` & `mcmc2ndgen-0.0.4/examples/generate_data-ESA.ipynb`

 * *Files identical despite different names*

### Comparing `mcmc2ndgen-0.0.3/examples/generate_data_Keplerian.ipynb` & `mcmc2ndgen-0.0.4/examples/generate_data_Keplerian.ipynb`

 * *Files identical despite different names*

### Comparing `mcmc2ndgen-0.0.3/examples/.ipynb_checkpoints/example_mcmc_run-checkpoint.ipynb` & `mcmc2ndgen-0.0.4/examples/.ipynb_checkpoints/example_mcmc_run-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `mcmc2ndgen-0.0.3/examples/.ipynb_checkpoints/generate_data-ESA-checkpoint.ipynb` & `mcmc2ndgen-0.0.4/examples/.ipynb_checkpoints/generate_data-ESA-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `mcmc2ndgen-0.0.3/examples/.ipynb_checkpoints/generate_data_Keplerian-checkpoint.ipynb` & `mcmc2ndgen-0.0.4/examples/.ipynb_checkpoints/generate_data_Keplerian-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `mcmc2ndgen-0.0.3/utils/TDI_functions.py` & `mcmc2ndgen-0.0.4/utils/TDI_functions.py`

 * *Files identical despite different names*

### Comparing `mcmc2ndgen-0.0.3/utils/delay_time_dependence.py` & `mcmc2ndgen-0.0.4/utils/delay_time_dependence.py`

 * *Files identical despite different names*

### Comparing `mcmc2ndgen-0.0.3/utils/delay_time_dependence_Keplerian.py` & `mcmc2ndgen-0.0.4/utils/delay_time_dependence_Keplerian.py`

 * *Files identical despite different names*

### Comparing `mcmc2ndgen-0.0.3/utils/filter_functions.py` & `mcmc2ndgen-0.0.4/utils/filter_functions.py`

 * *Files identical despite different names*

### Comparing `mcmc2ndgen-0.0.3/utils/mcmc_functions.py` & `mcmc2ndgen-0.0.4/utils/mcmc_functions.py`

 * *Files identical despite different names*

### Comparing `mcmc2ndgen-0.0.3/utils/mcmc_functions_Keplerian.py` & `mcmc2ndgen-0.0.4/utils/mcmc_functions_Keplerian.py`

 * *Files identical despite different names*

### Comparing `mcmc2ndgen-0.0.3/LICENSE` & `mcmc2ndgen-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mcmc2ndgen-0.0.3/README.md` & `mcmc2ndgen-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mcmc2ndgen-0.0.3/pyproject.toml` & `mcmc2ndgen-0.0.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "MCMC2ndGen"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Jessica Page", email="jp0089@uah.edu" },
 ]
 description = "An MCMC sampler for the time-varying LISA spacecraft separations used in TDI."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = [
-  "numpy",
-  "pkg_resources",
-  "math",
-  "scipy.signal",
-]
 
 [project.urls]
 "Homepage" = "https://github.com/JessicaPage/MCMC2ndGen"
```

### Comparing `mcmc2ndgen-0.0.3/PKG-INFO` & `mcmc2ndgen-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: MCMC2ndGen
-Version: 0.0.3
+Version: 0.0.4
 Summary: An MCMC sampler for the time-varying LISA spacecraft separations used in TDI.
 Project-URL: Homepage, https://github.com/JessicaPage/MCMC2ndGen
 Author-email: Jessica Page <jp0089@uah.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Requires-Dist: math
-Requires-Dist: numpy
-Requires-Dist: pkg-resources
-Requires-Dist: scipy-signal
 Description-Content-Type: text/markdown
 
 # MCMC2ndGen
 
 This generates MCMC samples of parameters to estimate the time-varying LISA spacecraft separations required for laser frequency noise suppression in time-delay interferometry (TDI). See the paper published on the subject [here](https://arxiv.org/abs/2305.14186). The data to sample over is generated with [LISA Instrument and LISA Orbits](https://gitlab.in2p3.fr/lisa-simulation/instrument), so the naming and labeling conventions may look similar to their codes for clarity.
 
 The default settings for creating a BayesTDI() class instance are for LISA data generated with Keplerian orbit model parameterization, i.e. ({M01,a,w}--> Lij(t)).
```

