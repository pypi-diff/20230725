# Comparing `tmp/MultiAssayExperiment-0.2.2.tar.gz` & `tmp/MultiAssayExperiment-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MultiAssayExperiment-0.2.2.tar", last modified: Tue Feb 28 05:49:11 2023, max compression
+gzip compressed data, was "MultiAssayExperiment-0.2.3.tar", last modified: Tue Jul 25 06:27:24 2023, max compression
```

## Comparing `MultiAssayExperiment-0.2.2.tar` & `MultiAssayExperiment-0.2.3.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 05:49:11.238443 MultiAssayExperiment-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 05:49:11.230443 MultiAssayExperiment-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 05:49:11.234443 MultiAssayExperiment-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-02-28 05:49:11.238443 MultiAssayExperiment-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 05:49:11.234443 MultiAssayExperiment-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 05:49:11.234443 MultiAssayExperiment-0.2.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/docs/tutorial.md
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-02-28 05:49:11.242443 MultiAssayExperiment-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 05:49:11.230443 MultiAssayExperiment-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 05:49:11.234443 MultiAssayExperiment-0.2.2/src/MultiAssayExperiment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-02-28 05:49:11.000000 MultiAssayExperiment-0.2.2/src/MultiAssayExperiment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-02-28 05:49:11.000000 MultiAssayExperiment-0.2.2/src/MultiAssayExperiment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 05:49:11.000000 MultiAssayExperiment-0.2.2/src/MultiAssayExperiment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 05:47:53.000000 MultiAssayExperiment-0.2.2/src/MultiAssayExperiment.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-02-28 05:49:11.000000 MultiAssayExperiment-0.2.2/src/MultiAssayExperiment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-28 05:49:11.000000 MultiAssayExperiment-0.2.2/src/MultiAssayExperiment.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 05:49:11.238443 MultiAssayExperiment-0.2.2/src/multiassayexperiment/
--rw-r--r--   0 runner    (1001) docker     (123)    20936 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/src/multiassayexperiment/MultiAssayExperiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/src/multiassayexperiment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 05:49:11.238443 MultiAssayExperiment-0.2.2/src/multiassayexperiment/io/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/src/multiassayexperiment/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/src/multiassayexperiment/io/anndata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/src/multiassayexperiment/io/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/src/multiassayexperiment/io/mudata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 05:49:11.238443 MultiAssayExperiment-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 05:49:11.238443 MultiAssayExperiment-0.2.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   311344 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/tests/data/adata.h5ad
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/tests/test_se_add_expt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/tests/test_se_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/tests/test_se_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/tests/test_se_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/tests/test_se_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-02-28 05:47:44.000000 MultiAssayExperiment-0.2.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:27:24.546064 MultiAssayExperiment-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:27:24.518064 MultiAssayExperiment-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:27:24.530064 MultiAssayExperiment-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-25 06:27:24.546064 MultiAssayExperiment-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:27:24.534064 MultiAssayExperiment-0.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:27:24.538064 MultiAssayExperiment-0.2.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/docs/tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-25 06:27:24.550064 MultiAssayExperiment-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:27:24.518064 MultiAssayExperiment-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:27:24.542064 MultiAssayExperiment-0.2.3/src/MultiAssayExperiment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-25 06:27:24.000000 MultiAssayExperiment-0.2.3/src/MultiAssayExperiment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-25 06:27:24.000000 MultiAssayExperiment-0.2.3/src/MultiAssayExperiment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:27:24.000000 MultiAssayExperiment-0.2.3/src/MultiAssayExperiment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:25:51.000000 MultiAssayExperiment-0.2.3/src/MultiAssayExperiment.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-25 06:27:24.000000 MultiAssayExperiment-0.2.3/src/MultiAssayExperiment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-25 06:27:24.000000 MultiAssayExperiment-0.2.3/src/MultiAssayExperiment.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:27:24.542064 MultiAssayExperiment-0.2.3/src/multiassayexperiment/
+-rw-r--r--   0 runner    (1001) docker     (123)    20347 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/src/multiassayexperiment/MultiAssayExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/src/multiassayexperiment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:27:24.542064 MultiAssayExperiment-0.2.3/src/multiassayexperiment/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/src/multiassayexperiment/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/src/multiassayexperiment/io/anndata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/src/multiassayexperiment/io/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/src/multiassayexperiment/io/mudata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/src/multiassayexperiment/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:27:24.546064 MultiAssayExperiment-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:27:24.546064 MultiAssayExperiment-0.2.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   311344 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/tests/data/adata.h5ad
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/tests/test_se_add_expt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/tests/test_se_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/tests/test_se_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/tests/test_se_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/tests/test_se_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/tox.ini
```

### Comparing `MultiAssayExperiment-0.2.2/.coveragerc` & `MultiAssayExperiment-0.2.3/.coveragerc`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.2/.github/workflows/pypi-publish.yml` & `MultiAssayExperiment-0.2.3/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.2/.github/workflows/pypi-test.yml` & `MultiAssayExperiment-0.2.3/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.2/.gitignore` & `MultiAssayExperiment-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.2/CONTRIBUTING.rst` & `MultiAssayExperiment-0.2.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.2/LICENSE.txt` & `MultiAssayExperiment-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.2/PKG-INFO` & `MultiAssayExperiment-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultiAssayExperiment
-Version: 0.2.2
+Version: 0.2.3
 Summary: Container class to represent multiple experiments and assays performed over a set of samples
 Home-page: https://github.com/BiocPy/MultiAssayExperiment
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/BiocPy/MultiAssayExperiment
 Platform: any
```

### Comparing `MultiAssayExperiment-0.2.2/README.md` & `MultiAssayExperiment-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.2/docs/Makefile` & `MultiAssayExperiment-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.2/docs/conf.py` & `MultiAssayExperiment-0.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.2/docs/index.md` & `MultiAssayExperiment-0.2.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.2/docs/readme.md` & `MultiAssayExperiment-0.2.3/docs/readme.md`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.2/docs/tutorial.md` & `MultiAssayExperiment-0.2.3/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.2/setup.cfg` & `MultiAssayExperiment-0.2.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 install_requires = 
 	importlib-metadata; python_version<"3.8"
-	summarizedexperiment>=0.2.0
-	singlecellexperiment>=0.2.1
+	summarizedexperiment
+	singlecellexperiment
 	mudata
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `MultiAssayExperiment-0.2.2/setup.py` & `MultiAssayExperiment-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.2/src/MultiAssayExperiment.egg-info/PKG-INFO` & `MultiAssayExperiment-0.2.3/src/MultiAssayExperiment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultiAssayExperiment
-Version: 0.2.2
+Version: 0.2.3
 Summary: Container class to represent multiple experiments and assays performed over a set of samples
 Home-page: https://github.com/BiocPy/MultiAssayExperiment
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/BiocPy/MultiAssayExperiment
 Platform: any
```

### Comparing `MultiAssayExperiment-0.2.2/src/MultiAssayExperiment.egg-info/SOURCES.txt` & `MultiAssayExperiment-0.2.3/src/MultiAssayExperiment.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 src/MultiAssayExperiment.egg-info/SOURCES.txt
 src/MultiAssayExperiment.egg-info/dependency_links.txt
 src/MultiAssayExperiment.egg-info/not-zip-safe
 src/MultiAssayExperiment.egg-info/requires.txt
 src/MultiAssayExperiment.egg-info/top_level.txt
 src/multiassayexperiment/MultiAssayExperiment.py
 src/multiassayexperiment/__init__.py
+src/multiassayexperiment/types.py
 src/multiassayexperiment/io/__init__.py
 src/multiassayexperiment/io/anndata.py
 src/multiassayexperiment/io/interface.py
 src/multiassayexperiment/io/mudata.py
 tests/conftest.py
 tests/test_se_add_expt.py
 tests/test_se_create.py
```

### Comparing `MultiAssayExperiment-0.2.2/src/multiassayexperiment/__init__.py` & `MultiAssayExperiment-0.2.3/src/multiassayexperiment/__init__.py`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.2/src/multiassayexperiment/io/anndata.py` & `MultiAssayExperiment-0.2.3/src/multiassayexperiment/io/anndata.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from ..MultiAssayExperiment import MultiAssayExperiment
-
-import singlecellexperiment as sce
 import anndata
 import pandas as pd
+import singlecellexperiment as sce
+
+from ..MultiAssayExperiment import MultiAssayExperiment
 
 __author__ = "jkanche"
 __copyright__ = "jkanche"
 __license__ = "MIT"
 
 
 def fromAnnData(adata: anndata.AnnData) -> MultiAssayExperiment:
-    """Transform AnnData object to MAE representation
+    """Transform AnnData object to MAE representation.
 
     Args:
-        data (AnnData): MuData object
+        data (AnnData): MuData object.
 
     Returns:
-        MultiAssayExperiment: MAE from AnnData
+        MultiAssayExperiment: MAE from AnnData.
     """
     scexpt = sce.fromAnnData(adata=adata)
 
     experiments = {"unknown": scexpt}
 
     coldata = pd.DataFrame({"samples": ["unknown_sample"]}, index=["unknown_sample"])
```

### Comparing `MultiAssayExperiment-0.2.2/src/multiassayexperiment/io/interface.py` & `MultiAssayExperiment-0.2.3/src/multiassayexperiment/io/interface.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,60 +1,51 @@
-from typing import Union, MutableMapping
-
 from collections import OrderedDict
+from typing import MutableMapping, Union
 
 import anndata
-import singlecellexperiment as sce
-from summarizedexperiment import SummarizedExperiment, RangeSummarizedExperiment
 import pandas as pd
+import singlecellexperiment as sce
+from summarizedexperiment.BaseSE import BaseSE
 
 from ..MultiAssayExperiment import MultiAssayExperiment
 
 __author__ = "jkanche"
 __copyright__ = "jkanche"
 __license__ = "MIT"
 
 
 def makeMAE(
     experiments: MutableMapping[
         str,
-        Union[
-            anndata.AnnData,
-            sce.SingleCellExperiment,
-            SummarizedExperiment,
-            RangeSummarizedExperiment,
-        ],
+        Union[anndata.AnnData, BaseSE],
     ]
 ) -> MultiAssayExperiment:
-    """Make MAE from list of experiments. 
-        naively creates sample map and coldata objects.
-        Also converts `AnnData` objects to `SingleCellExperiment`s.
+    """Make MAE from list of experiments.
+
+    naively creates sample map and coldata objects.
+    Also converts `AnnData` objects to SingleCellExperiment objects.
 
     Args:
-        experiments (MutableMapping[str, Union[anndata.AnnData, SingleCellExperiment, SummarizedExperiment, RangeSummarizedExperiment]]): a dictionary of experiments. 
+        experiments (MutableMapping[str, Union[anndata.AnnData, BaseSE]]): a dictionary of experiments.
 
     Raises:
         TypeError: if any of the provided objects are not an expected types.
 
     Returns:
-        MultiAssayExperiment: an MAE from the experiments
+        MultiAssayExperiment: an MAE from the experiments.
     """
     failedExpts = []
     for expname, expt in experiments.items():
-        if not (
-            isinstance(expt, sce.SingleCellExperiment)
-            or isinstance(expt, anndata.AnnData)
-            or isinstance(expt, SummarizedExperiment)
-            or isinstance(expt, RangeSummarizedExperiment)
-        ):
+        if not (isinstance(expt, anndata.AnnData) or isinstance(expt, BaseSE)):
             failedExpts.append(expname)
 
     if len(failedExpts) > 0:
         raise TypeError(
-            f"Experiments {failedExpts} are not compatible, Must be either a AnnData, SingleCellExperiment, SummarizedExperiment objects"
+            f"Experiments {failedExpts} are not compatible, Must be either an "
+            "AnnData, SingleCellExperiment or SummarizedExperiment object."
         )
 
     newExpts = OrderedDict()
 
     sampleMap = pd.DataFrame()
     samples = []
 
@@ -76,9 +67,11 @@
 
         sampleMap = pd.concat([sampleMap, asy_df])
         samples.append(asy_sample)
 
     coldata = pd.DataFrame({"samples": samples}, index=samples)
 
     return MultiAssayExperiment(
-        experiments=newExpts, colData=coldata, sampleMap=sampleMap,
+        experiments=newExpts,
+        colData=coldata,
+        sampleMap=sampleMap,
     )
```

### Comparing `MultiAssayExperiment-0.2.2/src/multiassayexperiment/io/mudata.py` & `MultiAssayExperiment-0.2.3/src/multiassayexperiment/io/mudata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-from ..MultiAssayExperiment import MultiAssayExperiment
+from collections import OrderedDict
 
 import mudata
-from collections import OrderedDict
 import pandas as pd
 from singlecellexperiment import fromAnnData
 
+from ..MultiAssayExperiment import MultiAssayExperiment
+
 __author__ = "jkanche"
 __copyright__ = "jkanche"
 __license__ = "MIT"
 
 
 def fromMuData(mudata: mudata.MuData) -> MultiAssayExperiment:
-    """Transform MuData object to MAE representation
+    """Transform MuData object to MAE representation.
 
     Args:
-        mudata (mudata.MuData): MuData object
+        mudata (mudata.MuData): MuData object.
 
     Returns:
-        MultiAssayExperiment: MAE representation
+        MultiAssayExperiment: MAE representation.
     """
 
     if mudata.isbacked:
         raise Exception("backed mode is currently not supported")
 
     experiments = OrderedDict()
```

### Comparing `MultiAssayExperiment-0.2.2/tests/data/adata.h5ad` & `MultiAssayExperiment-0.2.3/tests/data/adata.h5ad`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.2/tests/test_se_add_expt.py` & `MultiAssayExperiment-0.2.3/tests/test_se_add_expt.py`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.2/tests/test_se_create.py` & `MultiAssayExperiment-0.2.3/tests/test_se_create.py`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.2/tests/test_se_io.py` & `MultiAssayExperiment-0.2.3/tests/test_se_io.py`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.2/tests/test_se_methods.py` & `MultiAssayExperiment-0.2.3/tests/test_se_methods.py`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.2/tests/test_se_slices.py` & `MultiAssayExperiment-0.2.3/tests/test_se_slices.py`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.2/tox.ini` & `MultiAssayExperiment-0.2.3/tox.ini`

 * *Files identical despite different names*

