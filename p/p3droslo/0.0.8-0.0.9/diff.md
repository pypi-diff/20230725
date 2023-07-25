# Comparing `tmp/p3droslo-0.0.8.tar.gz` & `tmp/p3droslo-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p3droslo-0.0.8.tar", last modified: Tue Mar 14 10:13:59 2023, max compression
+gzip compressed data, was "p3droslo-0.0.9.tar", last modified: Tue Jul 25 14:05:50 2023, max compression
```

## Comparing `p3droslo-0.0.8.tar` & `p3droslo-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:13:59.657783 p3droslo-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-14 10:13:47.000000 p3droslo-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    42276 2023-03-14 10:13:59.657783 p3droslo-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-03-14 10:13:47.000000 p3droslo-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-03-14 10:13:47.000000 p3droslo-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 10:13:59.657783 p3droslo-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:13:59.657783 p3droslo-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:13:59.657783 p3droslo-0.0.8/src/p3droslo/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-14 10:13:47.000000 p3droslo-0.0.8/src/p3droslo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 10:13:47.000000 p3droslo-0.0.8/src/p3droslo/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-03-14 10:13:47.000000 p3droslo-0.0.8/src/p3droslo/observation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:13:59.657783 p3droslo-0.0.8/src/p3droslo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42276 2023-03-14 10:13:59.000000 p3droslo-0.0.8/src/p3droslo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-03-14 10:13:59.000000 p3droslo-0.0.8/src/p3droslo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 10:13:59.000000 p3droslo-0.0.8/src/p3droslo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-14 10:13:59.000000 p3droslo-0.0.8/src/p3droslo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-14 10:13:59.000000 p3droslo-0.0.8/src/p3droslo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 10:13:59.657783 p3droslo-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-14 10:13:47.000000 p3droslo-0.0.8/tests/test_observation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:50.569592 p3droslo-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 14:05:39.000000 p3droslo-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    43360 2023-07-25 14:05:50.569592 p3droslo-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-25 14:05:39.000000 p3droslo-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-25 14:05:39.000000 p3droslo-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 14:05:50.569592 p3droslo-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:50.565592 p3droslo-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:50.565592 p3droslo-0.0.9/src/p3droslo/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-25 14:05:39.000000 p3droslo-0.0.9/src/p3droslo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-25 14:05:39.000000 p3droslo-0.0.9/src/p3droslo/forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-25 14:05:39.000000 p3droslo-0.0.9/src/p3droslo/haar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12930 2023-07-25 14:05:39.000000 p3droslo-0.0.9/src/p3droslo/lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-07-25 14:05:39.000000 p3droslo-0.0.9/src/p3droslo/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17892 2023-07-25 14:05:39.000000 p3droslo-0.0.9/src/p3droslo/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-25 14:05:39.000000 p3droslo-0.0.9/src/p3droslo/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-07-25 14:05:39.000000 p3droslo-0.0.9/src/p3droslo/observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-25 14:05:39.000000 p3droslo-0.0.9/src/p3droslo/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:39.000000 p3droslo-0.0.9/src/p3droslo/reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-07-25 14:05:39.000000 p3droslo-0.0.9/src/p3droslo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:50.565592 p3droslo-0.0.9/src/p3droslo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43360 2023-07-25 14:05:50.000000 p3droslo-0.0.9/src/p3droslo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-25 14:05:50.000000 p3droslo-0.0.9/src/p3droslo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 14:05:50.000000 p3droslo-0.0.9/src/p3droslo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-25 14:05:50.000000 p3droslo-0.0.9/src/p3droslo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 14:05:50.000000 p3droslo-0.0.9/src/p3droslo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:50.569592 p3droslo-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-25 14:05:39.000000 p3droslo-0.0.9/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-25 14:05:39.000000 p3droslo-0.0.9/tests/test_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-25 14:05:39.000000 p3droslo-0.0.9/tests/test_utils.py
```

### Comparing `p3droslo-0.0.8/LICENSE` & `p3droslo-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `p3droslo-0.0.8/PKG-INFO` & `p3droslo-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p3droslo
-Version: 0.0.8
+Version: 0.0.9
 Summary: Probabilistic 3D Reconstruction of Specrtral Line Observations.
 Author-email: Frederik De Ceuster <frederik.deceuster@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -700,20 +700,45 @@
 ![Build status](https://github.com/Magritte-code/p3droslo/actions/workflows/build-and-test.yaml/badge.svg)
 ![Build status](https://github.com/Magritte-code/p3droslo/actions/workflows/upload-to-pypi.yaml/badge.svg)
 ![Build status](https://github.com/Magritte-code/p3droslo/actions/workflows/upload-to-anaconda.yaml/badge.svg)
 
 
 ## Installation
 
-Get the latest release (version 0.0.8) either from [PyPI](https://pypi.org/project/p3droslo/), using `pip`, with:
+Get the latest release (version 0.0.9) either from [PyPI](https://pypi.org/project/p3droslo/), using `pip`, with:
 ```
 pip install p3droslo
 ```
 or from [Anaconda.org](https://anaconda.org/FredDeCeuster/p3droslo), using `conda`, with:
 ```
 conda install -c freddeceuster p3droslo 
 ```
 or download the [source code](https://github.com/Magritte-code/p3droslo/archive/refs/heads/main.zip), unzip, and install with `pip` by executing:
 ```
 pip install .
 ```
 in the root directory of the code.
+
+
+## Documentation
+
+Documentation with examples can be found at [p3droslo.readthedocs.io](https://p3droslo.readthedocs.io/en/latest/).
+
+
+## Issues
+
+Please report any issues with this software or its documentation [here](https://github.com/Magritte-code/p3droslo/issues).
+
+
+## Contributing
+
+We are open to contributions to p3droslo. More information can be found [here](https://github.com/Magritte-code/p3droslo/blob/main/CONTRIBUTING.md).
+
+
+## Collaborating
+
+We are always interested in collaborating on exciting projects! So, if you have a project or just an idea, or data that might benefit from probabilistic 3D reconstruction or any other thing you can find in this repository, please contact [me](https://freddeceuster.github.io).
+
+
+## Acknowledgements
+
+Frederik De Ceuster is a Postdoctoral Research Fellow of the [Research Foundation - Flanders (FWO)](https://www.fwo.be/en/), grant number 1253223N, and was previously supported for this research by a Postdoctoral Mandate (PDM) from [KU Leuven](https://www.kuleuven.be/english/kuleuven/index.html), grant number PDMT2/21/066.
```

### Comparing `p3droslo-0.0.8/pyproject.toml` & `p3droslo-0.0.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "p3droslo"
-version = "0.0.8"
+version = "0.0.9"
 description = "Probabilistic 3D Reconstruction of Specrtral Line Observations."
 readme = "README.md"
 authors = [{ name = "Frederik De Ceuster", email = "frederik.deceuster@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
@@ -20,38 +20,42 @@
 ]
 keywords = ["3D Reconstruction", "Astrophysics", "Astronomy"]
 dependencies = [
     "matplotlib",
     "astroquery",
     "ipywidgets",
     "astropy",
+    "torch>=2.0.0",
     "numpy",
     "numba",
+    "tqdm",
+    "h5py",
 ]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/Magritte-code/p3droslo"
 
 [tool.bumpver]
-current_version = "0.0.8"
+current_version = "0.0.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
 "src/p3droslo/__init__.py" = ["{version}"]
 "conda/meta.yaml" = ['version: "{version}"']
 "README.md" = ['(version {version})']
+"docs/src/index.rst" = ['(version {version})']
 
 [tool.pytest.ini_options]
 addopts = ["--import-mode=importlib"]
 pythonpath = [".", "src"]
 
 #[project.scripts]
 #realpython = "reader.__main__:main"
```

### Comparing `p3droslo-0.0.8/src/p3droslo/observation.py` & `p3droslo-0.0.9/src/p3droslo/observation.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,17 @@
         #Load the data
         with fits.open(fits_file) as hdu:
             # Extract data
             self.img = hdu[0].data[0].astype(np.float32)   # Store as 32 bit numbers to avoid too much memory
             # Extract header
             self.hdr = hdu[0].header                       
 
+            # Extract the object name
+            self.object = str(self.hdr['OBJECT']).strip()
+            
             # Extract units for intensities
             self.I_unit = units.Unit(self.hdr['BUNIT'])
             
             # Extract units for axis
             self.x_unit = units.Unit(self.hdr['CUNIT1'])
             self.y_unit = units.Unit(self.hdr['CUNIT2'])
             self.f_unit = units.Unit(self.hdr['CUNIT3'])
```

### Comparing `p3droslo-0.0.8/src/p3droslo.egg-info/PKG-INFO` & `p3droslo-0.0.9/src/p3droslo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p3droslo
-Version: 0.0.8
+Version: 0.0.9
 Summary: Probabilistic 3D Reconstruction of Specrtral Line Observations.
 Author-email: Frederik De Ceuster <frederik.deceuster@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -700,20 +700,45 @@
 ![Build status](https://github.com/Magritte-code/p3droslo/actions/workflows/build-and-test.yaml/badge.svg)
 ![Build status](https://github.com/Magritte-code/p3droslo/actions/workflows/upload-to-pypi.yaml/badge.svg)
 ![Build status](https://github.com/Magritte-code/p3droslo/actions/workflows/upload-to-anaconda.yaml/badge.svg)
 
 
 ## Installation
 
-Get the latest release (version 0.0.8) either from [PyPI](https://pypi.org/project/p3droslo/), using `pip`, with:
+Get the latest release (version 0.0.9) either from [PyPI](https://pypi.org/project/p3droslo/), using `pip`, with:
 ```
 pip install p3droslo
 ```
 or from [Anaconda.org](https://anaconda.org/FredDeCeuster/p3droslo), using `conda`, with:
 ```
 conda install -c freddeceuster p3droslo 
 ```
 or download the [source code](https://github.com/Magritte-code/p3droslo/archive/refs/heads/main.zip), unzip, and install with `pip` by executing:
 ```
 pip install .
 ```
 in the root directory of the code.
+
+
+## Documentation
+
+Documentation with examples can be found at [p3droslo.readthedocs.io](https://p3droslo.readthedocs.io/en/latest/).
+
+
+## Issues
+
+Please report any issues with this software or its documentation [here](https://github.com/Magritte-code/p3droslo/issues).
+
+
+## Contributing
+
+We are open to contributions to p3droslo. More information can be found [here](https://github.com/Magritte-code/p3droslo/blob/main/CONTRIBUTING.md).
+
+
+## Collaborating
+
+We are always interested in collaborating on exciting projects! So, if you have a project or just an idea, or data that might benefit from probabilistic 3D reconstruction or any other thing you can find in this repository, please contact [me](https://freddeceuster.github.io).
+
+
+## Acknowledgements
+
+Frederik De Ceuster is a Postdoctoral Research Fellow of the [Research Foundation - Flanders (FWO)](https://www.fwo.be/en/), grant number 1253223N, and was previously supported for this research by a Postdoctoral Mandate (PDM) from [KU Leuven](https://www.kuleuven.be/english/kuleuven/index.html), grant number PDMT2/21/066.
```

