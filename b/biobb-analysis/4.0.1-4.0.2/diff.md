# Comparing `tmp/biobb_analysis-4.0.1.tar.gz` & `tmp/biobb_analysis-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/biobb_analysis-4.0.1.tar", last modified: Wed May 17 13:49:29 2023, max compression
+gzip compressed data, was "dist/biobb_analysis-4.0.2.tar", last modified: Tue Jul 25 11:11:45 2023, max compression
```

## Comparing `biobb_analysis-4.0.1.tar` & `biobb_analysis-4.0.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-17 13:49:29.000000 biobb_analysis-4.0.1/
--rwxr-xr-x   0 pau        (501) staff       (20)    11358 2021-06-11 09:52:36.000000 biobb_analysis-4.0.1/LICENSE
--rw-r--r--   0 pau        (501) staff       (20)     6372 2023-05-17 13:49:29.000000 biobb_analysis-4.0.1/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)     5380 2023-05-17 13:38:28.000000 biobb_analysis-4.0.1/README.md
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-17 13:49:28.000000 biobb_analysis-4.0.1/biobb_analysis/
--rw-r--r--   0 pau        (501) staff       (20)       82 2023-05-17 13:37:33.000000 biobb_analysis-4.0.1/biobb_analysis/__init__.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-17 13:49:28.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/
--rwxr-xr-x   0 pau        (501) staff       (20)      237 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/__init__.py
--rwxr-xr-x   0 pau        (501) staff       (20)    18276 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/common.py
--rwxr-xr-x   0 pau        (501) staff       (20)    13377 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_average.py
--rwxr-xr-x   0 pau        (501) staff       (20)    13184 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_bfactor.py
--rwxr-xr-x   0 pau        (501) staff       (20)    13291 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_convert.py
--rwxr-xr-x   0 pau        (501) staff       (20)    13387 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_dry.py
--rwxr-xr-x   0 pau        (501) staff       (20)    13403 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_image.py
--rwxr-xr-x   0 pau        (501) staff       (20)     5718 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_input.py
--rwxr-xr-x   0 pau        (501) staff       (20)    13387 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_mask.py
--rwxr-xr-x   0 pau        (501) staff       (20)    11475 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_rgyr.py
--rwxr-xr-x   0 pau        (501) staff       (20)    15009 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_rms.py
--rwxr-xr-x   0 pau        (501) staff       (20)    13109 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_rmsf.py
--rwxr-xr-x   0 pau        (501) staff       (20)    13179 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_slice.py
--rwxr-xr-x   0 pau        (501) staff       (20)    12946 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_snapshot.py
--rwxr-xr-x   0 pau        (501) staff       (20)    13411 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_strip.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-17 13:49:29.000000 biobb_analysis-4.0.1/biobb_analysis/gromacs/
--rwxr-xr-x   0 pau        (501) staff       (20)      154 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/gromacs/__init__.py
--rwxr-xr-x   0 pau        (501) staff       (20)    19167 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/gromacs/common.py
--rwxr-xr-x   0 pau        (501) staff       (20)    17757 2023-05-11 08:49:51.000000 biobb_analysis-4.0.1/biobb_analysis/gromacs/gmx_cluster.py
--rwxr-xr-x   0 pau        (501) staff       (20)     9092 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/gromacs/gmx_energy.py
--rwxr-xr-x   0 pau        (501) staff       (20)    19456 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/gromacs/gmx_image.py
--rwxr-xr-x   0 pau        (501) staff       (20)    11312 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/gromacs/gmx_rgyr.py
--rwxr-xr-x   0 pau        (501) staff       (20)    11164 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/gromacs/gmx_rms.py
--rwxr-xr-x   0 pau        (501) staff       (20)    12853 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/gromacs/gmx_trjconv_str.py
--rwxr-xr-x   0 pau        (501) staff       (20)    14280 2023-05-09 12:40:30.000000 biobb_analysis-4.0.1/biobb_analysis/gromacs/gmx_trjconv_str_ens.py
--rwxr-xr-x   0 pau        (501) staff       (20)    13379 2023-04-04 10:57:24.000000 biobb_analysis-4.0.1/biobb_analysis/gromacs/gmx_trjconv_trj.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-17 13:49:29.000000 biobb_analysis-4.0.1/biobb_analysis/test/
--rwxr-xr-x   0 pau        (501) staff       (20)        0 2021-06-11 09:52:36.000000 biobb_analysis-4.0.1/biobb_analysis/test/__init__.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-05-17 13:49:28.000000 biobb_analysis-4.0.1/biobb_analysis.egg-info/
--rw-r--r--   0 pau        (501) staff       (20)     6372 2023-05-17 13:49:28.000000 biobb_analysis-4.0.1/biobb_analysis.egg-info/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)     1328 2023-05-17 13:49:28.000000 biobb_analysis-4.0.1/biobb_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 pau        (501) staff       (20)        1 2023-05-17 13:49:28.000000 biobb_analysis-4.0.1/biobb_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 pau        (501) staff       (20)     1199 2023-05-17 13:49:28.000000 biobb_analysis-4.0.1/biobb_analysis.egg-info/entry_points.txt
--rw-r--r--   0 pau        (501) staff       (20)       20 2023-05-17 13:49:28.000000 biobb_analysis-4.0.1/biobb_analysis.egg-info/requires.txt
--rw-r--r--   0 pau        (501) staff       (20)       15 2023-05-17 13:49:28.000000 biobb_analysis-4.0.1/biobb_analysis.egg-info/top_level.txt
--rw-r--r--   0 pau        (501) staff       (20)       38 2023-05-17 13:49:29.000000 biobb_analysis-4.0.1/setup.cfg
--rw-r--r--   0 pau        (501) staff       (20)     2810 2023-05-17 13:35:32.000000 biobb_analysis-4.0.1/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-07-25 11:11:45.000000 biobb_analysis-4.0.2/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11358 2022-05-26 11:32:48.000000 biobb_analysis-4.0.2/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6335 2023-07-25 11:11:45.000000 biobb_analysis-4.0.2/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5380 2023-07-25 11:09:16.000000 biobb_analysis-4.0.2/README.md
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-07-25 11:11:45.000000 biobb_analysis-4.0.2/biobb_analysis/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       82 2023-07-25 11:08:34.000000 biobb_analysis-4.0.2/biobb_analysis/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-07-25 11:11:45.000000 biobb_analysis-4.0.2/biobb_analysis/ambertools/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      237 2023-04-12 10:13:13.000000 biobb_analysis-4.0.2/biobb_analysis/ambertools/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    18276 2023-04-12 10:24:35.000000 biobb_analysis-4.0.2/biobb_analysis/ambertools/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    13377 2023-04-12 11:15:00.000000 biobb_analysis-4.0.2/biobb_analysis/ambertools/cpptraj_average.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    13184 2023-04-12 12:46:16.000000 biobb_analysis-4.0.2/biobb_analysis/ambertools/cpptraj_bfactor.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    13291 2023-04-12 12:53:31.000000 biobb_analysis-4.0.2/biobb_analysis/ambertools/cpptraj_convert.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    13387 2023-04-12 12:56:42.000000 biobb_analysis-4.0.2/biobb_analysis/ambertools/cpptraj_dry.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    13403 2023-04-12 12:59:34.000000 biobb_analysis-4.0.2/biobb_analysis/ambertools/cpptraj_image.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5718 2023-04-12 13:01:18.000000 biobb_analysis-4.0.2/biobb_analysis/ambertools/cpptraj_input.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    13387 2023-04-12 13:03:30.000000 biobb_analysis-4.0.2/biobb_analysis/ambertools/cpptraj_mask.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11475 2023-04-12 13:28:38.000000 biobb_analysis-4.0.2/biobb_analysis/ambertools/cpptraj_rgyr.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    15009 2023-04-12 13:32:27.000000 biobb_analysis-4.0.2/biobb_analysis/ambertools/cpptraj_rms.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    13109 2023-04-12 13:34:45.000000 biobb_analysis-4.0.2/biobb_analysis/ambertools/cpptraj_rmsf.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    13179 2023-04-12 13:36:26.000000 biobb_analysis-4.0.2/biobb_analysis/ambertools/cpptraj_slice.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    12946 2023-04-12 13:38:14.000000 biobb_analysis-4.0.2/biobb_analysis/ambertools/cpptraj_snapshot.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    13411 2023-04-12 13:40:26.000000 biobb_analysis-4.0.2/biobb_analysis/ambertools/cpptraj_strip.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-07-25 11:11:45.000000 biobb_analysis-4.0.2/biobb_analysis/gromacs/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      154 2023-04-12 10:13:19.000000 biobb_analysis-4.0.2/biobb_analysis/gromacs/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    19167 2023-04-12 13:42:07.000000 biobb_analysis-4.0.2/biobb_analysis/gromacs/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    17757 2023-07-25 10:08:55.000000 biobb_analysis-4.0.2/biobb_analysis/gromacs/gmx_cluster.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9092 2023-04-12 13:51:32.000000 biobb_analysis-4.0.2/biobb_analysis/gromacs/gmx_energy.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    19456 2023-04-12 13:57:45.000000 biobb_analysis-4.0.2/biobb_analysis/gromacs/gmx_image.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11312 2023-04-12 14:00:12.000000 biobb_analysis-4.0.2/biobb_analysis/gromacs/gmx_rgyr.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11164 2023-04-12 14:07:47.000000 biobb_analysis-4.0.2/biobb_analysis/gromacs/gmx_rms.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    12853 2023-04-12 14:23:24.000000 biobb_analysis-4.0.2/biobb_analysis/gromacs/gmx_trjconv_str.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    14293 2023-07-25 10:07:11.000000 biobb_analysis-4.0.2/biobb_analysis/gromacs/gmx_trjconv_str_ens.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    13379 2023-04-12 14:24:04.000000 biobb_analysis-4.0.2/biobb_analysis/gromacs/gmx_trjconv_trj.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-07-25 11:11:45.000000 biobb_analysis-4.0.2/biobb_analysis/test/
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2022-05-26 11:32:48.000000 biobb_analysis-4.0.2/biobb_analysis/test/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-07-25 11:11:45.000000 biobb_analysis-4.0.2/biobb_analysis.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6335 2023-07-25 11:11:45.000000 biobb_analysis-4.0.2/biobb_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1328 2023-07-25 11:11:45.000000 biobb_analysis-4.0.2/biobb_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        1 2023-07-25 11:11:45.000000 biobb_analysis-4.0.2/biobb_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1198 2023-07-25 11:11:45.000000 biobb_analysis-4.0.2/biobb_analysis.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       20 2023-07-25 11:11:45.000000 biobb_analysis-4.0.2/biobb_analysis.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       15 2023-07-25 11:11:45.000000 biobb_analysis-4.0.2/biobb_analysis.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       38 2023-07-25 11:11:45.000000 biobb_analysis-4.0.2/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2810 2023-07-25 11:07:45.000000 biobb_analysis-4.0.2/setup.py
```

### Comparing `biobb_analysis-4.0.1/LICENSE` & `biobb_analysis-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.0.1/PKG-INFO` & `biobb_analysis-4.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: biobb_analysis
-Version: 4.0.1
+Version: 4.0.2
 Summary: Biobb_analysis is the Biobb module collection to perform analysis of molecular dynamics simulations.
 Home-page: https://github.com/bioexcel/biobb_analysis
 Author: Biobb developers
 Author-email: genis.bayarri@irbbarcelona.org
-License: UNKNOWN
 Project-URL: Documentation, http://biobb_analysis.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
@@ -23,15 +21,15 @@
 License-File: LICENSE
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_analysis?label=Version)](https://GitHub.com/bioexcel/biobb_analysis/tags/)
 [![](https://img.shields.io/pypi/v/biobb-analysis.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-analysis/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_analysis?label=Conda)](https://anaconda.org/bioconda/biobb_analysis)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_analysis?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_analysis)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_analysis?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_analysis:4.0.1--pyhdfd78af_1)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_analysis:4.0.2--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_analysis)
 [![](https://img.shields.io/pypi/pyversions/biobb-analysis.svg?label=Python%20Versions)](https://pypi.org/project/biobb-analysis/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_analysis)
 
 [![](https://readthedocs.org/projects/biobb-analysis/badge/?version=latest&label=Docs)](https://biobb-analysis.readthedocs.io/en/latest/?badge=latest)
@@ -54,61 +52,61 @@
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb_analysis.readthedocs.io/en/latest/).
 
 ### Version
-v4.0.1 2023.1
+v4.0.2 2023.2
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_analysis>=4.0.1"
+        pip install "biobb_analysis>=4.0.2"
 
 
 * Usage: [Python API documentation](https://biobb-analysis.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_analysis>=4.0.1"
+        conda install -c bioconda "biobb_analysis>=4.0.2"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-analysis.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-analysis.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_analysis:4.0.1--pyhdfd78af_1
+        docker pull quay.io/biocontainers/biobb_analysis:4.0.2--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_analysis:4.0.1--pyhdfd78af_1 <command>
+        docker run quay.io/biocontainers/biobb_analysis:4.0.2--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_analysis.sif https://depot.galaxyproject.org/singularity/biobb_analysis:4.0.1--pyhdfd78af_1
+        singularity pull --name biobb_analysis.sif https://depot.galaxyproject.org/singularity/biobb_analysis:4.0.2--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_analysis.sif <command>
 
@@ -121,9 +119,7 @@
 * (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
 * (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
-
-
```

### Comparing `biobb_analysis-4.0.1/README.md` & `biobb_analysis-4.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_analysis?label=Version)](https://GitHub.com/bioexcel/biobb_analysis/tags/)
 [![](https://img.shields.io/pypi/v/biobb-analysis.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-analysis/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_analysis?label=Conda)](https://anaconda.org/bioconda/biobb_analysis)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_analysis?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_analysis)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_analysis?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_analysis:4.0.1--pyhdfd78af_1)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_analysis:4.0.2--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_analysis)
 [![](https://img.shields.io/pypi/pyversions/biobb-analysis.svg?label=Python%20Versions)](https://pypi.org/project/biobb-analysis/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_analysis)
 
 [![](https://readthedocs.org/projects/biobb-analysis/badge/?version=latest&label=Docs)](https://biobb-analysis.readthedocs.io/en/latest/?badge=latest)
@@ -30,61 +30,61 @@
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb_analysis.readthedocs.io/en/latest/).
 
 ### Version
-v4.0.1 2023.1
+v4.0.2 2023.2
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_analysis>=4.0.1"
+        pip install "biobb_analysis>=4.0.2"
 
 
 * Usage: [Python API documentation](https://biobb-analysis.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_analysis>=4.0.1"
+        conda install -c bioconda "biobb_analysis>=4.0.2"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-analysis.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-analysis.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_analysis:4.0.1--pyhdfd78af_1
+        docker pull quay.io/biocontainers/biobb_analysis:4.0.2--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_analysis:4.0.1--pyhdfd78af_1 <command>
+        docker run quay.io/biocontainers/biobb_analysis:4.0.2--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_analysis.sif https://depot.galaxyproject.org/singularity/biobb_analysis:4.0.1--pyhdfd78af_1
+        singularity pull --name biobb_analysis.sif https://depot.galaxyproject.org/singularity/biobb_analysis:4.0.2--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_analysis.sif <command>
```

### Comparing `biobb_analysis-4.0.1/biobb_analysis/ambertools/common.py` & `biobb_analysis-4.0.2/biobb_analysis/ambertools/common.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_average.py` & `biobb_analysis-4.0.2/biobb_analysis/ambertools/cpptraj_average.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_bfactor.py` & `biobb_analysis-4.0.2/biobb_analysis/ambertools/cpptraj_bfactor.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_convert.py` & `biobb_analysis-4.0.2/biobb_analysis/ambertools/cpptraj_convert.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_dry.py` & `biobb_analysis-4.0.2/biobb_analysis/ambertools/cpptraj_dry.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_image.py` & `biobb_analysis-4.0.2/biobb_analysis/ambertools/cpptraj_image.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_input.py` & `biobb_analysis-4.0.2/biobb_analysis/ambertools/cpptraj_input.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_mask.py` & `biobb_analysis-4.0.2/biobb_analysis/ambertools/cpptraj_mask.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_rgyr.py` & `biobb_analysis-4.0.2/biobb_analysis/ambertools/cpptraj_rgyr.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_rms.py` & `biobb_analysis-4.0.2/biobb_analysis/ambertools/cpptraj_rms.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_rmsf.py` & `biobb_analysis-4.0.2/biobb_analysis/ambertools/cpptraj_rmsf.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_slice.py` & `biobb_analysis-4.0.2/biobb_analysis/ambertools/cpptraj_slice.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_snapshot.py` & `biobb_analysis-4.0.2/biobb_analysis/ambertools/cpptraj_snapshot.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.0.1/biobb_analysis/ambertools/cpptraj_strip.py` & `biobb_analysis-4.0.2/biobb_analysis/ambertools/cpptraj_strip.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.0.1/biobb_analysis/gromacs/common.py` & `biobb_analysis-4.0.2/biobb_analysis/gromacs/common.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.0.1/biobb_analysis/gromacs/gmx_cluster.py` & `biobb_analysis-4.0.2/biobb_analysis/gromacs/gmx_cluster.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.0.1/biobb_analysis/gromacs/gmx_energy.py` & `biobb_analysis-4.0.2/biobb_analysis/gromacs/gmx_energy.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.0.1/biobb_analysis/gromacs/gmx_image.py` & `biobb_analysis-4.0.2/biobb_analysis/gromacs/gmx_image.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.0.1/biobb_analysis/gromacs/gmx_rgyr.py` & `biobb_analysis-4.0.2/biobb_analysis/gromacs/gmx_rgyr.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.0.1/biobb_analysis/gromacs/gmx_rms.py` & `biobb_analysis-4.0.2/biobb_analysis/gromacs/gmx_rms.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.0.1/biobb_analysis/gromacs/gmx_trjconv_str.py` & `biobb_analysis-4.0.2/biobb_analysis/gromacs/gmx_trjconv_str.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.0.1/biobb_analysis/gromacs/gmx_trjconv_str_ens.py` & `biobb_analysis-4.0.2/biobb_analysis/gromacs/gmx_trjconv_str_ens.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
                                            self.io_dict["out"]["output_str_ens_path"],
                                            self.stage_io_dict.get("unique_dir"),
                                            self.output_name + '*', self.out_log)
         else:
             process_output_trjconv_str_ens(self.stage_io_dict.get("unique_dir"),
                                            self.stage_io_dict["out"]["output_str_ens_path"],
                                            self.io_dict["out"]["output_str_ens_path"],
-                                           'output*.pdb', self.out_log)
+                                           self.output_name + '*.pdb', self.out_log)
 
         self.tmp_files.extend([
             self.stage_io_dict.get("unique_dir"),
             self.io_dict['in'].get("stdin_file_path")
         ])
         self.remove_tmp_files()
```

### Comparing `biobb_analysis-4.0.1/biobb_analysis/gromacs/gmx_trjconv_trj.py` & `biobb_analysis-4.0.2/biobb_analysis/gromacs/gmx_trjconv_trj.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.0.1/biobb_analysis.egg-info/PKG-INFO` & `biobb_analysis-4.0.2/biobb_analysis.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: biobb-analysis
-Version: 4.0.1
+Version: 4.0.2
 Summary: Biobb_analysis is the Biobb module collection to perform analysis of molecular dynamics simulations.
 Home-page: https://github.com/bioexcel/biobb_analysis
 Author: Biobb developers
 Author-email: genis.bayarri@irbbarcelona.org
-License: UNKNOWN
 Project-URL: Documentation, http://biobb_analysis.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
@@ -23,15 +21,15 @@
 License-File: LICENSE
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_analysis?label=Version)](https://GitHub.com/bioexcel/biobb_analysis/tags/)
 [![](https://img.shields.io/pypi/v/biobb-analysis.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-analysis/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_analysis?label=Conda)](https://anaconda.org/bioconda/biobb_analysis)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_analysis?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_analysis)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_analysis?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_analysis:4.0.1--pyhdfd78af_1)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_analysis:4.0.2--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_analysis)
 [![](https://img.shields.io/pypi/pyversions/biobb-analysis.svg?label=Python%20Versions)](https://pypi.org/project/biobb-analysis/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_analysis)
 
 [![](https://readthedocs.org/projects/biobb-analysis/badge/?version=latest&label=Docs)](https://biobb-analysis.readthedocs.io/en/latest/?badge=latest)
@@ -54,61 +52,61 @@
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb_analysis.readthedocs.io/en/latest/).
 
 ### Version
-v4.0.1 2023.1
+v4.0.2 2023.2
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_analysis>=4.0.1"
+        pip install "biobb_analysis>=4.0.2"
 
 
 * Usage: [Python API documentation](https://biobb-analysis.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_analysis>=4.0.1"
+        conda install -c bioconda "biobb_analysis>=4.0.2"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-analysis.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-analysis.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_analysis:4.0.1--pyhdfd78af_1
+        docker pull quay.io/biocontainers/biobb_analysis:4.0.2--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_analysis:4.0.1--pyhdfd78af_1 <command>
+        docker run quay.io/biocontainers/biobb_analysis:4.0.2--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_analysis.sif https://depot.galaxyproject.org/singularity/biobb_analysis:4.0.1--pyhdfd78af_1
+        singularity pull --name biobb_analysis.sif https://depot.galaxyproject.org/singularity/biobb_analysis:4.0.2--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_analysis.sif <command>
 
@@ -121,9 +119,7 @@
 * (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
 * (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
-
-
```

### Comparing `biobb_analysis-4.0.1/biobb_analysis.egg-info/SOURCES.txt` & `biobb_analysis-4.0.2/biobb_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.0.1/biobb_analysis.egg-info/entry_points.txt` & `biobb_analysis-4.0.2/biobb_analysis.egg-info/entry_points.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,7 @@
 gmx_energy = biobb_analysis.gromacs.gmx_energy:main
 gmx_image = biobb_analysis.gromacs.gmx_image:main
 gmx_rgyr = biobb_analysis.gromacs.gmx_rgyr:main
 gmx_rms = biobb_analysis.gromacs.gmx_rms:main
 gmx_trjconv_str = biobb_analysis.gromacs.gmx_trjconv_str:main
 gmx_trjconv_str_ens = biobb_analysis.gromacs.gmx_trjconv_str_ens:main
 gmx_trjconv_trj = biobb_analysis.gromacs.gmx_trjconv_trj:main
-
```

### Comparing `biobb_analysis-4.0.1/setup.py` & `biobb_analysis-4.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_analysis",
-    version="4.0.1",
+    version="4.0.2",
     author="Biobb developers",
     author_email="genis.bayarri@irbbarcelona.org",
     description="Biobb_analysis is the Biobb module collection to perform analysis of molecular dynamics simulations.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility",
     url="https://github.com/bioexcel/biobb_analysis",
```

