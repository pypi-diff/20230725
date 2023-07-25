# Comparing `tmp/easyliftover-0.0.6.tar.gz` & `tmp/easyliftover-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyliftover-0.0.6.tar", max compression
+gzip compressed data, was "easyliftover-0.0.7.tar", max compression
```

## Comparing `easyliftover-0.0.6.tar` & `easyliftover-0.0.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    35149 2023-07-25 06:48:08.047050 easyliftover-0.0.6/LICENSE
--rw-r--r--   0        0        0      459 2023-07-25 06:48:08.047050 easyliftover-0.0.6/README.md
--rw-r--r--   0        0        0       90 2023-07-25 06:48:08.047050 easyliftover-0.0.6/easyliftover/__init__.py
--rw-r--r--   0        0        0      189 2023-07-25 06:48:08.047050 easyliftover-0.0.6/easyliftover/genomes.py
--rw-r--r--   0        0        0      117 2023-07-25 06:48:08.047050 easyliftover-0.0.6/easyliftover/lifters/__init__.py
--rw-r--r--   0        0        0     1931 2023-07-25 06:48:08.047050 easyliftover-0.0.6/easyliftover/lifters/abstract.py
--rw-r--r--   0        0        0      680 2023-07-25 06:48:08.047050 easyliftover-0.0.6/easyliftover/lifters/bed.py
--rw-r--r--   0        0        0      661 2023-07-25 06:48:08.047050 easyliftover-0.0.6/easyliftover/lifters/gff.py
--rw-r--r--   0        0        0       62 2023-07-25 06:48:08.799057 easyliftover-0.0.6/easyliftover/lifters/pyliftover/.git
--rw-r--r--   0        0        0      303 2023-07-25 06:48:08.811057 easyliftover-0.0.6/easyliftover/lifters/pyliftover/.gitignore
--rw-r--r--   0        0        0      139 2023-07-25 06:48:08.811057 easyliftover-0.0.6/easyliftover/lifters/pyliftover/.travis.yml
--rw-r--r--   0        0        0      416 2023-07-25 06:48:08.811057 easyliftover-0.0.6/easyliftover/lifters/pyliftover/CHANGELOG.txt
--rw-r--r--   0        0        0     1064 2023-07-25 06:48:08.811057 easyliftover-0.0.6/easyliftover/lifters/pyliftover/LICENSE
--rw-r--r--   0        0        0       32 2023-07-25 06:48:08.811057 easyliftover-0.0.6/easyliftover/lifters/pyliftover/MANIFEST.in
--rw-r--r--   0        0        0     2670 2023-07-25 06:48:08.811057 easyliftover-0.0.6/easyliftover/lifters/pyliftover/README.rst
--rw-r--r--   0        0        0     1661 2023-07-25 06:48:08.811057 easyliftover-0.0.6/easyliftover/lifters/pyliftover/pyliftover/__init__.py
--rw-r--r--   0        0        0    11116 2023-07-25 06:48:08.811057 easyliftover-0.0.6/easyliftover/lifters/pyliftover/pyliftover/chainfile.py
--rw-r--r--   0        0        0     6795 2023-07-25 06:48:08.811057 easyliftover-0.0.6/easyliftover/lifters/pyliftover/pyliftover/intervaltree.py
--rw-r--r--   0        0        0     5516 2023-07-25 06:48:08.811057 easyliftover-0.0.6/easyliftover/lifters/pyliftover/pyliftover/liftover.py
--rw-r--r--   0        0        0      178 2023-07-25 06:48:08.811057 easyliftover-0.0.6/easyliftover/lifters/pyliftover/setup.cfg
--rw-r--r--   0        0        0     1972 2023-07-25 06:48:08.811057 easyliftover-0.0.6/easyliftover/lifters/pyliftover/setup.py
--rw-r--r--   0        0        0      210 2023-07-25 06:48:08.811057 easyliftover-0.0.6/easyliftover/lifters/pyliftover/tests/__init__.py
--rw-r--r--   0        0        0     3756 2023-07-25 06:48:08.811057 easyliftover-0.0.6/easyliftover/lifters/pyliftover/tests/chainfile_test.py
--rw-r--r--   0        0        0      299 2023-07-25 06:48:08.811057 easyliftover-0.0.6/easyliftover/lifters/pyliftover/tests/data/README.txt
--rw-r--r--   0        0        0    85433 2023-07-25 06:48:08.811057 easyliftover-0.0.6/easyliftover/lifters/pyliftover/tests/data/hg17ToHg18.over.chain.gz
--rw-r--r--   0        0        0    68588 2023-07-25 06:48:08.811057 easyliftover-0.0.6/easyliftover/lifters/pyliftover/tests/data/hg17ToHg18.testpoints.txt.gz
--rw-r--r--   0        0        0  1246411 2023-07-25 06:48:08.815057 easyliftover-0.0.6/easyliftover/lifters/pyliftover/tests/data/hg38ToHg19.over.chain.gz
--rw-r--r--   0        0        0      818 2023-07-25 06:48:08.815057 easyliftover-0.0.6/easyliftover/lifters/pyliftover/tests/data/hg38ToHg19.testinput.txt
--rw-r--r--   0        0        0      523 2023-07-25 06:48:08.815057 easyliftover-0.0.6/easyliftover/lifters/pyliftover/tests/data/hg38ToHg19.testoutput.txt
--rw-r--r--   0        0        0      902 2023-07-25 06:48:08.815057 easyliftover-0.0.6/easyliftover/lifters/pyliftover/tests/data/mds42.to.mg1655.liftOver
--rw-r--r--   0        0        0     1247 2023-07-25 06:48:08.815057 easyliftover-0.0.6/easyliftover/lifters/pyliftover/tests/intervaltree_test.py
--rw-r--r--   0        0        0     3618 2023-07-25 06:48:08.815057 easyliftover-0.0.6/easyliftover/lifters/pyliftover/tests/liftover_test.py
--rw-r--r--   0        0        0     3952 2023-07-25 06:48:08.815057 easyliftover-0.0.6/easyliftover/lifters/pyliftover/tests/open_liftover_chain_file_test.py
--rw-r--r--   0        0        0     1825 2023-07-25 06:48:08.047050 easyliftover-0.0.6/easyliftover/lifters/wig.py
--rw-r--r--   0        0        0     1665 2023-07-25 06:48:08.047050 easyliftover-0.0.6/easyliftover/liftover.py
--rw-r--r--   0        0        0      573 2023-07-25 06:48:08.047050 easyliftover-0.0.6/easyliftover/targets.py
--rw-r--r--   0        0        0     1231 2023-07-25 06:48:08.047050 easyliftover-0.0.6/easyliftover/types.json
--rw-r--r--   0        0        0      230 2023-07-25 06:48:08.047050 easyliftover-0.0.6/easyliftover/types.py
--rw-r--r--   0        0        0      686 2023-07-25 06:48:08.047050 easyliftover-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 easyliftover-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-25 07:45:53.698200 easyliftover-0.0.7/LICENSE
+-rw-r--r--   0        0        0      459 2023-07-25 07:45:53.698200 easyliftover-0.0.7/README.md
+-rw-r--r--   0        0        0       90 2023-07-25 07:45:53.698200 easyliftover-0.0.7/easyliftover/__init__.py
+-rw-r--r--   0        0        0      189 2023-07-25 07:45:53.698200 easyliftover-0.0.7/easyliftover/genomes.py
+-rw-r--r--   0        0        0      117 2023-07-25 07:45:53.698200 easyliftover-0.0.7/easyliftover/lifters/__init__.py
+-rw-r--r--   0        0        0     1931 2023-07-25 07:45:53.698200 easyliftover-0.0.7/easyliftover/lifters/abstract.py
+-rw-r--r--   0        0        0      680 2023-07-25 07:45:53.698200 easyliftover-0.0.7/easyliftover/lifters/bed.py
+-rw-r--r--   0        0        0      661 2023-07-25 07:45:53.698200 easyliftover-0.0.7/easyliftover/lifters/gff.py
+-rw-r--r--   0        0        0       62 2023-07-25 07:45:54.270202 easyliftover-0.0.7/easyliftover/lifters/pyliftover/.git
+-rw-r--r--   0        0        0      303 2023-07-25 07:45:54.278202 easyliftover-0.0.7/easyliftover/lifters/pyliftover/.gitignore
+-rw-r--r--   0        0        0      139 2023-07-25 07:45:54.278202 easyliftover-0.0.7/easyliftover/lifters/pyliftover/.travis.yml
+-rw-r--r--   0        0        0      416 2023-07-25 07:45:54.278202 easyliftover-0.0.7/easyliftover/lifters/pyliftover/CHANGELOG.txt
+-rw-r--r--   0        0        0     1064 2023-07-25 07:45:54.278202 easyliftover-0.0.7/easyliftover/lifters/pyliftover/LICENSE
+-rw-r--r--   0        0        0       32 2023-07-25 07:45:54.278202 easyliftover-0.0.7/easyliftover/lifters/pyliftover/MANIFEST.in
+-rw-r--r--   0        0        0     2670 2023-07-25 07:45:54.278202 easyliftover-0.0.7/easyliftover/lifters/pyliftover/README.rst
+-rw-r--r--   0        0        0     1661 2023-07-25 07:45:54.278202 easyliftover-0.0.7/easyliftover/lifters/pyliftover/pyliftover/__init__.py
+-rw-r--r--   0        0        0    11116 2023-07-25 07:45:54.278202 easyliftover-0.0.7/easyliftover/lifters/pyliftover/pyliftover/chainfile.py
+-rw-r--r--   0        0        0     6795 2023-07-25 07:45:54.278202 easyliftover-0.0.7/easyliftover/lifters/pyliftover/pyliftover/intervaltree.py
+-rw-r--r--   0        0        0     5516 2023-07-25 07:45:54.278202 easyliftover-0.0.7/easyliftover/lifters/pyliftover/pyliftover/liftover.py
+-rw-r--r--   0        0        0      178 2023-07-25 07:45:54.278202 easyliftover-0.0.7/easyliftover/lifters/pyliftover/setup.cfg
+-rw-r--r--   0        0        0     1972 2023-07-25 07:45:54.278202 easyliftover-0.0.7/easyliftover/lifters/pyliftover/setup.py
+-rw-r--r--   0        0        0      210 2023-07-25 07:45:54.278202 easyliftover-0.0.7/easyliftover/lifters/pyliftover/tests/__init__.py
+-rw-r--r--   0        0        0     3756 2023-07-25 07:45:54.278202 easyliftover-0.0.7/easyliftover/lifters/pyliftover/tests/chainfile_test.py
+-rw-r--r--   0        0        0      299 2023-07-25 07:45:54.278202 easyliftover-0.0.7/easyliftover/lifters/pyliftover/tests/data/README.txt
+-rw-r--r--   0        0        0    85433 2023-07-25 07:45:54.278202 easyliftover-0.0.7/easyliftover/lifters/pyliftover/tests/data/hg17ToHg18.over.chain.gz
+-rw-r--r--   0        0        0    68588 2023-07-25 07:45:54.278202 easyliftover-0.0.7/easyliftover/lifters/pyliftover/tests/data/hg17ToHg18.testpoints.txt.gz
+-rw-r--r--   0        0        0  1246411 2023-07-25 07:45:54.282203 easyliftover-0.0.7/easyliftover/lifters/pyliftover/tests/data/hg38ToHg19.over.chain.gz
+-rw-r--r--   0        0        0      818 2023-07-25 07:45:54.282203 easyliftover-0.0.7/easyliftover/lifters/pyliftover/tests/data/hg38ToHg19.testinput.txt
+-rw-r--r--   0        0        0      523 2023-07-25 07:45:54.282203 easyliftover-0.0.7/easyliftover/lifters/pyliftover/tests/data/hg38ToHg19.testoutput.txt
+-rw-r--r--   0        0        0      902 2023-07-25 07:45:54.282203 easyliftover-0.0.7/easyliftover/lifters/pyliftover/tests/data/mds42.to.mg1655.liftOver
+-rw-r--r--   0        0        0     1247 2023-07-25 07:45:54.282203 easyliftover-0.0.7/easyliftover/lifters/pyliftover/tests/intervaltree_test.py
+-rw-r--r--   0        0        0     3618 2023-07-25 07:45:54.282203 easyliftover-0.0.7/easyliftover/lifters/pyliftover/tests/liftover_test.py
+-rw-r--r--   0        0        0     3952 2023-07-25 07:45:54.282203 easyliftover-0.0.7/easyliftover/lifters/pyliftover/tests/open_liftover_chain_file_test.py
+-rw-r--r--   0        0        0     1825 2023-07-25 07:45:53.698200 easyliftover-0.0.7/easyliftover/lifters/wig.py
+-rw-r--r--   0        0        0     1665 2023-07-25 07:45:53.698200 easyliftover-0.0.7/easyliftover/liftover.py
+-rw-r--r--   0        0        0      573 2023-07-25 07:45:53.698200 easyliftover-0.0.7/easyliftover/targets.py
+-rw-r--r--   0        0        0     1332 2023-07-25 07:45:53.698200 easyliftover-0.0.7/easyliftover/types.json
+-rw-r--r--   0        0        0      230 2023-07-25 07:45:53.698200 easyliftover-0.0.7/easyliftover/types.py
+-rw-r--r--   0        0        0      686 2023-07-25 07:45:53.698200 easyliftover-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 easyliftover-0.0.7/PKG-INFO
```

### Comparing `easyliftover-0.0.6/LICENSE` & `easyliftover-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.6/easyliftover/lifters/abstract.py` & `easyliftover-0.0.7/easyliftover/lifters/abstract.py`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.6/easyliftover/lifters/bed.py` & `easyliftover-0.0.7/easyliftover/lifters/bed.py`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.6/easyliftover/lifters/gff.py` & `easyliftover-0.0.7/easyliftover/lifters/gff.py`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.6/easyliftover/lifters/pyliftover/LICENSE` & `easyliftover-0.0.7/easyliftover/lifters/pyliftover/LICENSE`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.6/easyliftover/lifters/pyliftover/README.rst` & `easyliftover-0.0.7/easyliftover/lifters/pyliftover/README.rst`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.6/easyliftover/lifters/pyliftover/pyliftover/__init__.py` & `easyliftover-0.0.7/easyliftover/lifters/pyliftover/pyliftover/__init__.py`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.6/easyliftover/lifters/pyliftover/pyliftover/chainfile.py` & `easyliftover-0.0.7/easyliftover/lifters/pyliftover/pyliftover/chainfile.py`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.6/easyliftover/lifters/pyliftover/pyliftover/intervaltree.py` & `easyliftover-0.0.7/easyliftover/lifters/pyliftover/pyliftover/intervaltree.py`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.6/easyliftover/lifters/pyliftover/pyliftover/liftover.py` & `easyliftover-0.0.7/easyliftover/lifters/pyliftover/pyliftover/liftover.py`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.6/easyliftover/lifters/pyliftover/setup.py` & `easyliftover-0.0.7/easyliftover/lifters/pyliftover/setup.py`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.6/easyliftover/lifters/pyliftover/tests/chainfile_test.py` & `easyliftover-0.0.7/easyliftover/lifters/pyliftover/tests/chainfile_test.py`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.6/easyliftover/lifters/pyliftover/tests/data/hg17ToHg18.over.chain.gz` & `easyliftover-0.0.7/easyliftover/lifters/pyliftover/tests/data/hg17ToHg18.over.chain.gz`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.6/easyliftover/lifters/pyliftover/tests/data/hg17ToHg18.testpoints.txt.gz` & `easyliftover-0.0.7/easyliftover/lifters/pyliftover/tests/data/hg17ToHg18.testpoints.txt.gz`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.6/easyliftover/lifters/pyliftover/tests/data/hg38ToHg19.over.chain.gz` & `easyliftover-0.0.7/easyliftover/lifters/pyliftover/tests/data/hg38ToHg19.over.chain.gz`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.6/easyliftover/lifters/pyliftover/tests/data/hg38ToHg19.testinput.txt` & `easyliftover-0.0.7/easyliftover/lifters/pyliftover/tests/data/hg38ToHg19.testinput.txt`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.6/easyliftover/lifters/pyliftover/tests/data/hg38ToHg19.testoutput.txt` & `easyliftover-0.0.7/easyliftover/lifters/pyliftover/tests/data/hg38ToHg19.testoutput.txt`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.6/easyliftover/lifters/pyliftover/tests/data/mds42.to.mg1655.liftOver` & `easyliftover-0.0.7/easyliftover/lifters/pyliftover/tests/data/mds42.to.mg1655.liftOver`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.6/easyliftover/lifters/pyliftover/tests/intervaltree_test.py` & `easyliftover-0.0.7/easyliftover/lifters/pyliftover/tests/intervaltree_test.py`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.6/easyliftover/lifters/pyliftover/tests/liftover_test.py` & `easyliftover-0.0.7/easyliftover/lifters/pyliftover/tests/liftover_test.py`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.6/easyliftover/lifters/pyliftover/tests/open_liftover_chain_file_test.py` & `easyliftover-0.0.7/easyliftover/lifters/pyliftover/tests/open_liftover_chain_file_test.py`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.6/easyliftover/lifters/wig.py` & `easyliftover-0.0.7/easyliftover/lifters/wig.py`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.6/easyliftover/liftover.py` & `easyliftover-0.0.7/easyliftover/liftover.py`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.6/easyliftover/targets.py` & `easyliftover-0.0.7/easyliftover/targets.py`

 * *Files identical despite different names*

### Comparing `easyliftover-0.0.6/easyliftover/types.json` & `easyliftover-0.0.7/easyliftover/types.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {'0': "{'id': 'annotation'}",*

 * * '1': "{'id': 'wig'}",*

 * * '2': "{'id': 'alignment'}",*

 * * '3': "{'id': 'variant'}"}*

```diff
@@ -23,14 +23,15 @@
                 "name": "bedpe"
             },
             {
                 "can_be_lifted": false,
                 "name": "Other"
             }
         ],
+        "id": "annotation",
         "name": "Annotation"
     },
     {
         "Description": "Quantitative genomic data",
         "formats": [
             {
                 "can_be_lifted": true,
@@ -45,14 +46,15 @@
                 "name": "bedGraph"
             },
             {
                 "can_be_lifted": false,
                 "name": "Other"
             }
         ],
+        "id": "wig",
         "name": "Wiggle"
     },
     {
         "Description": "Alignment data",
         "formats": [
             {
                 "can_be_lifted": false,
@@ -63,20 +65,22 @@
                 "name": "cram"
             },
             {
                 "can_be_lifted": false,
                 "name": "Other"
             }
         ],
+        "id": "alignment",
         "name": "Alignment"
     },
     {
         "Description": "Variant data",
         "formats": [
             {
                 "can_be_lifted": false,
                 "name": "vcf"
             }
         ],
+        "id": "variant",
         "name": "Variant"
     }
 ]
```

### Comparing `easyliftover-0.0.6/pyproject.toml` & `easyliftover-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "easyliftover"
-version = "0.0.6"
+version = "0.0.7"
 description = "A python package for lifting over biological files"
 license = "MIT"
 authors = ["Nico Trummer <nictru32@gmail.com>"]
 repository = "https://github.com/biomedbigdata/easyLiftover"
 homepage = "https://github.com/biomedbigdata/easyLiftover"
 readme = "README.md"
```

### Comparing `easyliftover-0.0.6/PKG-INFO` & `easyliftover-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyliftover
-Version: 0.0.6
+Version: 0.0.7
 Summary: A python package for lifting over biological files
 Home-page: https://github.com/biomedbigdata/easyLiftover
 License: MIT
 Author: Nico Trummer
 Author-email: nictru32@gmail.com
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
```

