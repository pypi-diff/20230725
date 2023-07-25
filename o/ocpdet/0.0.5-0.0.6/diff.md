# Comparing `tmp/ocpdet-0.0.5.tar.gz` & `tmp/ocpdet-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocpdet-0.0.5.tar", last modified: Sat Feb 11 19:22:08 2023, max compression
+gzip compressed data, was "ocpdet-0.0.6.tar", last modified: Tue Jul 25 11:44:12 2023, max compression
```

## Comparing `ocpdet-0.0.5.tar` & `ocpdet-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 victorkhamesi   (501) staff       (20)        0 2023-02-11 19:22:08.252084 ocpdet-0.0.5/
--rw-r--r--   0 victorkhamesi   (501) staff       (20)     1065 2022-10-20 14:42:39.000000 ocpdet-0.0.5/LICENSE
--rw-r--r--   0 victorkhamesi   (501) staff       (20)     2946 2023-02-11 19:22:08.252231 ocpdet-0.0.5/PKG-INFO
--rw-r--r--   0 victorkhamesi   (501) staff       (20)     2389 2023-02-11 19:06:01.000000 ocpdet-0.0.5/README.md
-drwxr-xr-x   0 victorkhamesi   (501) staff       (20)        0 2023-02-11 19:22:08.248161 ocpdet-0.0.5/ocpdet/
--rw-r--r--   0 victorkhamesi   (501) staff       (20)     4278 2023-02-11 19:01:31.000000 ocpdet-0.0.5/ocpdet/CUSUM.py
--rw-r--r--   0 victorkhamesi   (501) staff       (20)     4368 2022-10-24 17:00:34.000000 ocpdet-0.0.5/ocpdet/EWMA.py
--rw-r--r--   0 victorkhamesi   (501) staff       (20)    10591 2023-02-10 17:07:05.000000 ocpdet-0.0.5/ocpdet/NeuralNetwork.py
--rw-r--r--   0 victorkhamesi   (501) staff       (20)     3508 2023-01-19 16:39:41.000000 ocpdet-0.0.5/ocpdet/TwoSample.py
--rw-r--r--   0 victorkhamesi   (501) staff       (20)      144 2022-10-25 07:17:41.000000 ocpdet-0.0.5/ocpdet/__init__.py
-drwxr-xr-x   0 victorkhamesi   (501) staff       (20)        0 2023-02-11 19:22:08.251478 ocpdet-0.0.5/ocpdet.egg-info/
--rw-r--r--   0 victorkhamesi   (501) staff       (20)     2946 2023-02-11 19:22:08.000000 ocpdet-0.0.5/ocpdet.egg-info/PKG-INFO
--rw-r--r--   0 victorkhamesi   (501) staff       (20)      279 2023-02-11 19:22:08.000000 ocpdet-0.0.5/ocpdet.egg-info/SOURCES.txt
--rw-r--r--   0 victorkhamesi   (501) staff       (20)        1 2023-02-11 19:22:08.000000 ocpdet-0.0.5/ocpdet.egg-info/dependency_links.txt
--rw-r--r--   0 victorkhamesi   (501) staff       (20)       28 2023-02-11 19:22:08.000000 ocpdet-0.0.5/ocpdet.egg-info/requires.txt
--rw-r--r--   0 victorkhamesi   (501) staff       (20)        7 2023-02-11 19:22:08.000000 ocpdet-0.0.5/ocpdet.egg-info/top_level.txt
--rw-r--r--   0 victorkhamesi   (501) staff       (20)      103 2023-02-11 19:22:08.252922 ocpdet-0.0.5/setup.cfg
--rw-r--r--   0 victorkhamesi   (501) staff       (20)      836 2023-02-11 19:22:04.000000 ocpdet-0.0.5/setup.py
+drwxr-xr-x   0 victorkhamesi   (501) staff       (20)        0 2023-07-25 11:44:12.660349 ocpdet-0.0.6/
+-rw-r--r--   0 victorkhamesi   (501) staff       (20)     1303 2023-07-02 09:53:53.000000 ocpdet-0.0.6/LICENSE
+-rw-r--r--   0 victorkhamesi   (501) staff       (20)     2946 2023-07-25 11:44:12.660573 ocpdet-0.0.6/PKG-INFO
+-rw-r--r--   0 victorkhamesi   (501) staff       (20)     2426 2023-07-25 11:08:56.000000 ocpdet-0.0.6/README.md
+drwxr-xr-x   0 victorkhamesi   (501) staff       (20)        0 2023-07-25 11:44:12.653751 ocpdet-0.0.6/ocpdet/
+-rw-r--r--   0 victorkhamesi   (501) staff       (20)     4278 2023-07-25 11:10:40.000000 ocpdet-0.0.6/ocpdet/CUSUM.py
+-rw-r--r--   0 victorkhamesi   (501) staff       (20)     4368 2023-07-02 09:53:53.000000 ocpdet-0.0.6/ocpdet/EWMA.py
+-rw-r--r--   0 victorkhamesi   (501) staff       (20)    10591 2023-07-02 09:53:53.000000 ocpdet-0.0.6/ocpdet/NeuralNetwork.py
+-rw-r--r--   0 victorkhamesi   (501) staff       (20)     3508 2023-07-02 09:53:53.000000 ocpdet-0.0.6/ocpdet/TwoSample.py
+-rw-r--r--   0 victorkhamesi   (501) staff       (20)      144 2023-07-02 09:53:53.000000 ocpdet-0.0.6/ocpdet/__init__.py
+drwxr-xr-x   0 victorkhamesi   (501) staff       (20)        0 2023-07-25 11:44:12.659800 ocpdet-0.0.6/ocpdet.egg-info/
+-rw-r--r--   0 victorkhamesi   (501) staff       (20)     2946 2023-07-25 11:44:12.000000 ocpdet-0.0.6/ocpdet.egg-info/PKG-INFO
+-rw-r--r--   0 victorkhamesi   (501) staff       (20)      279 2023-07-25 11:44:12.000000 ocpdet-0.0.6/ocpdet.egg-info/SOURCES.txt
+-rw-r--r--   0 victorkhamesi   (501) staff       (20)        1 2023-07-25 11:44:12.000000 ocpdet-0.0.6/ocpdet.egg-info/dependency_links.txt
+-rw-r--r--   0 victorkhamesi   (501) staff       (20)       28 2023-07-25 11:44:12.000000 ocpdet-0.0.6/ocpdet.egg-info/requires.txt
+-rw-r--r--   0 victorkhamesi   (501) staff       (20)        7 2023-07-25 11:44:12.000000 ocpdet-0.0.6/ocpdet.egg-info/top_level.txt
+-rw-r--r--   0 victorkhamesi   (501) staff       (20)      103 2023-07-25 11:44:12.661565 ocpdet-0.0.6/setup.cfg
+-rw-r--r--   0 victorkhamesi   (501) staff       (20)      836 2023-07-25 11:43:13.000000 ocpdet-0.0.6/setup.py
```

### Comparing `ocpdet-0.0.5/PKG-INFO` & `ocpdet-0.0.6/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,69 +1,53 @@
-Metadata-Version: 2.1
-Name: ocpdet
-Version: 0.0.5
-Summary: A Python package for online changepoint detection, implementing state-of-the-art algorithms and a novel approach.
-Home-page: https://github.com/vkhamesi/ocpdet
-Author: Victor Khamesi
-Author-email: victor.khamesi21@imperial.ac.uk
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # [ocpdet](https://pypi.org/project/ocpdet/)
-OCPDet is a Python package for online changepoint detection, implementing state-of-the-art algorithms and a novel approach.
+OCPDet is an open-source Python package for online changepoint detection, implementing state-of-the-art algorithms and a novel approach, using a `scikit-learn` style API.
 
-[![PyPI version](https://badge.fury.io/py/ocpdet.svg)](https://badge.fury.io/py/ocpdet) 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7232039.svg)](https://doi.org/10.5281/zenodo.7232039)
+[![PyPI](https://img.shields.io/pypi/v/ocpdet?color=g)](https://img.shields.io/pypi/v/ocpdet?color=g)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7632721.svg)](https://doi.org/10.5281/zenodo.7632721)
 
-A Python package for online changepoint detection in univariate and multivariate data.
+This package is the outcome of my Master Thesis at Imperial College London within the MSc in Statistics, Department of Mathematics.
 
 Algorithms implemented in ocpdet are
 
 - **CUSUM**: Cumulative Sum algorithm, proposed by Page (1954)
 - **EWMA**: Exponentially Weighted Moving Average algorithm, proposed by Roberts (1959)
 - **Two Sample tests**: Nonparametric hypothesis testing for changepoint detection, proposed by Ross et al. (2011)
-- **Neural Networks**: Novel approach based on sequentially learning neural networks, proposed by Hushchyn et al. (2020) and extended to online context (Master's Thesis) 
+- **Neural Networks**: Novel approach based on sequentially learning neural networks, proposed by Hushchyn et al. (2020) and extended to online context (Master Thesis) 
 
 ## Installation
 
 ```bash
 pip install ocpdet
 ``` 
 
 ## Examples
 
-- [CUSUM.ipynb](https://nbviewer.jupyter.org/github/vkhamesi/ocpdet/tree/main/docs/CUSUM.ipynb)  
-- [EWMA.ipynb](https://nbviewer.jupyter.org/github/vkhamesi/ocpdet/tree/main/docs/EWMA.ipynb)  
-- [TwoSample.ipynb](https://nbviewer.jupyter.org/github/vkhamesi/ocpdet/tree/main/docs/TwoSample.ipynb)  
-- [NeuralNetwork.ipynb](https://nbviewer.jupyter.org/github/vkhamesi/ocpdet/tree/main/docs/NeuralNetwork.ipynb)  
+- [CUSUM.ipynb](https://github.com/vkhamesi/ocpdet/blob/main/docs/CUSUM.ipynb)  
+- [EWMA.ipynb](https://github.com/vkhamesi/ocpdet/blob/main/docs/EWMA.ipynb)  
+- [TwoSample.ipynb](https://github.com/vkhamesi/ocpdet/blob/main/docs/TwoSample.ipynb)  
+- [NeuralNetwork.ipynb](https://github.com/vkhamesi/ocpdet/blob/main/docs/NeuralNetwork.ipynb)  
 
 ## How to cite this work
 
 Here is a suggestion to cite this GitHub repository:
 
-> Victor Khamesi. (2022). ocpdet: A Python package for online changepoint detection in univariate and multivariate data. (Version v0.0.4). Zenodo. https://doi.org/10.5281/zenodo.7232039
+> Victor Khamesi. (2022). ocpdet: A Python package for online changepoint detection in univariate and multivariate data. (Version v0.0.5). Zenodo. https://doi.org/10.5281/zenodo.7632721
 
 And a possible BibTeX entry:
 
 ```tex
 @software{victor_khamesi_2022,
   author       = {Victor Khamesi},
   title        = {ocpdet: A Python package for online changepoint detection in univariate and multivariate data.},
   month        = oct,
   year         = 2022,
   publisher    = {Zenodo},
   version      = {v0.0.5},
-  doi          = {10.5281/zenodo.7232039},
-  url          = {https://doi.org/10.5281/zenodo.7232039}
+  doi          = {10.5281/zenodo.7632721},
+  url          = {https://doi.org/10.5281/zenodo.7632721}
 }
 ```
 
 ## License
 
 The non-software content of this project is licensed under a [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/), and the software code is licensed under the [BSD-2 Clause license](https://opensource.org/licenses/BSD-2-Clause).
```

### Comparing `ocpdet-0.0.5/ocpdet/CUSUM.py` & `ocpdet-0.0.6/ocpdet/CUSUM.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         ----------
         
         data_new : float
             New observation in the data stream. S and T are updated according to
             CUSUM algorithm formulas.
         """
         self.S.append(max(0, self.S[-1] + (data_new - self.mu) / self.sigma - self.k))
-        self.T.append(max(0, self.S[-1] - (data_new - self.mu) / self.sigma - self.k))
+        self.T.append(max(0, self.T[-1] - (data_new - self.mu) / self.sigma - self.k))
     
     def decision_rule(self, 
                       i: int):
         """Decide whether or not a change has occurred.
 
         Parameters
         ----------
```

### Comparing `ocpdet-0.0.5/ocpdet/EWMA.py` & `ocpdet-0.0.6/ocpdet/EWMA.py`

 * *Files identical despite different names*

### Comparing `ocpdet-0.0.5/ocpdet/NeuralNetwork.py` & `ocpdet-0.0.6/ocpdet/NeuralNetwork.py`

 * *Files identical despite different names*

### Comparing `ocpdet-0.0.5/ocpdet/TwoSample.py` & `ocpdet-0.0.6/ocpdet/TwoSample.py`

 * *Files identical despite different names*

### Comparing `ocpdet-0.0.5/ocpdet.egg-info/PKG-INFO` & `ocpdet-0.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,67 @@
 Metadata-Version: 2.1
 Name: ocpdet
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python package for online changepoint detection, implementing state-of-the-art algorithms and a novel approach.
 Home-page: https://github.com/vkhamesi/ocpdet
 Author: Victor Khamesi
 Author-email: victor.khamesi21@imperial.ac.uk
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # [ocpdet](https://pypi.org/project/ocpdet/)
-OCPDet is a Python package for online changepoint detection, implementing state-of-the-art algorithms and a novel approach.
+OCPDet is an open-source Python package for online changepoint detection, implementing state-of-the-art algorithms and a novel approach, using a `scikit-learn` style API.
 
-[![PyPI version](https://badge.fury.io/py/ocpdet.svg)](https://badge.fury.io/py/ocpdet) 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7232039.svg)](https://doi.org/10.5281/zenodo.7232039)
+[![PyPI](https://img.shields.io/pypi/v/ocpdet?color=g)](https://img.shields.io/pypi/v/ocpdet?color=g)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7632721.svg)](https://doi.org/10.5281/zenodo.7632721)
 
-A Python package for online changepoint detection in univariate and multivariate data.
+This package is the outcome of my Master Thesis at Imperial College London within the MSc in Statistics, Department of Mathematics.
 
 Algorithms implemented in ocpdet are
 
 - **CUSUM**: Cumulative Sum algorithm, proposed by Page (1954)
 - **EWMA**: Exponentially Weighted Moving Average algorithm, proposed by Roberts (1959)
 - **Two Sample tests**: Nonparametric hypothesis testing for changepoint detection, proposed by Ross et al. (2011)
-- **Neural Networks**: Novel approach based on sequentially learning neural networks, proposed by Hushchyn et al. (2020) and extended to online context (Master's Thesis) 
+- **Neural Networks**: Novel approach based on sequentially learning neural networks, proposed by Hushchyn et al. (2020) and extended to online context (Master Thesis) 
 
 ## Installation
 
 ```bash
 pip install ocpdet
 ``` 
 
 ## Examples
 
-- [CUSUM.ipynb](https://nbviewer.jupyter.org/github/vkhamesi/ocpdet/tree/main/docs/CUSUM.ipynb)  
-- [EWMA.ipynb](https://nbviewer.jupyter.org/github/vkhamesi/ocpdet/tree/main/docs/EWMA.ipynb)  
-- [TwoSample.ipynb](https://nbviewer.jupyter.org/github/vkhamesi/ocpdet/tree/main/docs/TwoSample.ipynb)  
-- [NeuralNetwork.ipynb](https://nbviewer.jupyter.org/github/vkhamesi/ocpdet/tree/main/docs/NeuralNetwork.ipynb)  
+- [CUSUM.ipynb](https://github.com/vkhamesi/ocpdet/blob/main/docs/CUSUM.ipynb)  
+- [EWMA.ipynb](https://github.com/vkhamesi/ocpdet/blob/main/docs/EWMA.ipynb)  
+- [TwoSample.ipynb](https://github.com/vkhamesi/ocpdet/blob/main/docs/TwoSample.ipynb)  
+- [NeuralNetwork.ipynb](https://github.com/vkhamesi/ocpdet/blob/main/docs/NeuralNetwork.ipynb)  
 
 ## How to cite this work
 
 Here is a suggestion to cite this GitHub repository:
 
-> Victor Khamesi. (2022). ocpdet: A Python package for online changepoint detection in univariate and multivariate data. (Version v0.0.4). Zenodo. https://doi.org/10.5281/zenodo.7232039
+> Victor Khamesi. (2022). ocpdet: A Python package for online changepoint detection in univariate and multivariate data. (Version v0.0.5). Zenodo. https://doi.org/10.5281/zenodo.7632721
 
 And a possible BibTeX entry:
 
 ```tex
 @software{victor_khamesi_2022,
   author       = {Victor Khamesi},
   title        = {ocpdet: A Python package for online changepoint detection in univariate and multivariate data.},
   month        = oct,
   year         = 2022,
   publisher    = {Zenodo},
   version      = {v0.0.5},
-  doi          = {10.5281/zenodo.7232039},
-  url          = {https://doi.org/10.5281/zenodo.7232039}
+  doi          = {10.5281/zenodo.7632721},
+  url          = {https://doi.org/10.5281/zenodo.7632721}
 }
 ```
 
 ## License
 
 The non-software content of this project is licensed under a [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/), and the software code is licensed under the [BSD-2 Clause license](https://opensource.org/licenses/BSD-2-Clause).
```

### Comparing `ocpdet-0.0.5/setup.py` & `ocpdet-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ocpdet",
-    version="0.0.5",
+    version="0.0.6",
     author="Victor Khamesi",
     author_email="victor.khamesi21@imperial.ac.uk",
     description="A Python package for online changepoint detection, implementing state-of-the-art algorithms and a novel approach.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/vkhamesi/ocpdet",
     packages=setuptools.find_packages(),
```

