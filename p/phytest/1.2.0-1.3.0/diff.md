# Comparing `tmp/phytest-1.2.0.tar.gz` & `tmp/phytest-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phytest-1.2.0.tar", max compression
+gzip compressed data, was "phytest-1.3.0.tar", max compression
```

## Comparing `phytest-1.2.0.tar` & `phytest-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1080 2023-02-08 10:01:42.202674 phytest-1.2.0/LICENSE
--rw-r--r--   0        0        0     7390 2023-02-08 10:01:42.202674 phytest-1.2.0/README.rst
--rw-r--r--   0        0        0     3345 2023-02-08 10:01:42.214667 phytest-1.2.0/phytest/__init__.py
--rw-r--r--   0        0        0      110 2023-02-08 10:01:42.214667 phytest-1.2.0/phytest/bio/__init__.py
--rw-r--r--   0        0        0     3978 2023-02-08 10:01:42.214667 phytest-1.2.0/phytest/bio/alignment.py
--rw-r--r--   0        0        0     2555 2023-02-08 10:01:42.214667 phytest-1.2.0/phytest/bio/data.py
--rw-r--r--   0        0        0    18954 2023-02-08 10:01:42.214667 phytest-1.2.0/phytest/bio/sequence.py
--rw-r--r--   0        0        0    22662 2023-02-08 10:01:42.214667 phytest-1.2.0/phytest/bio/tree.py
--rw-r--r--   0        0        0     3280 2023-02-08 10:01:42.214667 phytest-1.2.0/phytest/cli.py
--rw-r--r--   0        0        0     1664 2023-02-08 10:01:42.214667 phytest-1.2.0/phytest/main.py
--rw-r--r--   0        0        0     3335 2023-02-08 10:01:42.214667 phytest-1.2.0/phytest/report/logo.css
--rw-r--r--   0        0        0     1298 2023-02-08 10:01:42.214667 phytest-1.2.0/phytest/utils.py
--rw-r--r--   0        0        0     1336 2023-02-08 10:01:42.218664 phytest-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     8670 1970-01-01 00:00:00.000000 phytest-1.2.0/setup.py
--rw-r--r--   0        0        0     8237 1970-01-01 00:00:00.000000 phytest-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-07-25 13:13:45.167068 phytest-1.3.0/LICENSE
+-rw-r--r--   0        0        0     7390 2023-07-25 13:13:45.167068 phytest-1.3.0/README.rst
+-rw-r--r--   0        0        0     3345 2023-07-25 13:13:45.179068 phytest-1.3.0/phytest/__init__.py
+-rw-r--r--   0        0        0      110 2023-07-25 13:13:45.183068 phytest-1.3.0/phytest/bio/__init__.py
+-rw-r--r--   0        0        0     3978 2023-07-25 13:13:45.183068 phytest-1.3.0/phytest/bio/alignment.py
+-rw-r--r--   0        0        0     6827 2023-07-25 13:13:45.183068 phytest-1.3.0/phytest/bio/data.py
+-rw-r--r--   0        0        0    18954 2023-07-25 13:13:45.183068 phytest-1.3.0/phytest/bio/sequence.py
+-rw-r--r--   0        0        0    23813 2023-07-25 13:13:45.183068 phytest-1.3.0/phytest/bio/tree.py
+-rw-r--r--   0        0        0     3280 2023-07-25 13:13:45.183068 phytest-1.3.0/phytest/cli.py
+-rw-r--r--   0        0        0     1664 2023-07-25 13:13:45.183068 phytest-1.3.0/phytest/main.py
+-rw-r--r--   0        0        0     3335 2023-07-25 13:13:45.183068 phytest-1.3.0/phytest/report/logo.css
+-rw-r--r--   0        0        0     1298 2023-07-25 13:13:45.183068 phytest-1.3.0/phytest/utils.py
+-rw-r--r--   0        0        0     1336 2023-07-25 13:13:45.183068 phytest-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8237 1970-01-01 00:00:00.000000 phytest-1.3.0/PKG-INFO
```

### Comparing `phytest-1.2.0/LICENSE` & `phytest-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phytest-1.2.0/README.rst` & `phytest-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `phytest-1.2.0/phytest/__init__.py` & `phytest-1.3.0/phytest/__init__.py`

 * *Files identical despite different names*

### Comparing `phytest-1.2.0/phytest/bio/alignment.py` & `phytest-1.3.0/phytest/bio/alignment.py`

 * *Files identical despite different names*

### Comparing `phytest-1.2.0/phytest/bio/sequence.py` & `phytest-1.3.0/phytest/bio/sequence.py`

 * *Files identical despite different names*

### Comparing `phytest-1.2.0/phytest/bio/tree.py` & `phytest-1.3.0/phytest/bio/tree.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,18 @@
         return (cls(root=tree.root, rooted=tree.rooted, id=tree.id, name=tree.name) for tree in trees)
 
     @classmethod
     def read_str(cls, tree_str: str, tree_format: str = "newick") -> 'Tree':
         data = StringIO(tree_str)
         return cls.read(data, tree_format)
 
+    @property
+    def tips(self):
+        return self.get_terminals()
+
     def parse_tip_dates(
         self,
         *,
         patterns=None,
         date_format: Optional[str] = None,
         decimal_year: bool = False,
     ):
@@ -107,28 +111,58 @@
         if max is not None:
             assert_or_warn(
                 number_of_tips <= max,
                 warning,
                 f"The number of tips ({number_of_tips}) is greater than the maximum ({max}).",
             )
 
+    def assert_unique_tips(self, *, warning: bool = False):
+        """
+        Asserts that all the tip names are unique.
+
+        Args:
+            warning (bool): If True, raise a warning instead of an exception. Defaults to False.
+                This flag can be set by running this method with the prefix `warn_` instead of `assert_`.
+
+        """
+        tip_names = [t.name for t in self.get_terminals()]
+        assert_or_warn(
+            len(tip_names) == len(set(tip_names)),
+            warning,
+            f"The tree contains {len(tip_names)} tips, however, {len(set(tip_names))} are unique.",
+        )
+
+    def assert_is_rooted(self, *, warning: bool = False):
+        """
+        Asserts that the tree is rooted.
+
+        Args:
+            warning (bool): If True, raise a warning instead of an exception. Defaults to False.
+                This flag can be set by running this method with the prefix `warn_` instead of `assert_`.
+        """
+        assert_or_warn(
+            self.rooted,
+            warning,
+            "The tree is not rooted.",
+        )
+
     def assert_is_bifurcating(self, *, warning: bool = False):
         """
         Asserts that the tree is bifurcating.
 
         The root may have 3 descendents and still be considered part of a bifurcating tree, because it has no ancestor.
 
         Args:
             warning (bool): If True, raise a warning instead of an exception. Defaults to False.
                 This flag can be set by running this method with the prefix `warn_` instead of `assert_`.
         """
         assert_or_warn(
             self.is_bifurcating(),
             warning,
-            f"The tree is not bifurcating.",
+            "The tree is not bifurcating.",
         )
 
     def assert_is_monophyletic(self, tips: List[Clade], *, warning: bool = False):
         """
         Asserts that the specified tips form a monophyletic group.
 
         Args:
```

### Comparing `phytest-1.2.0/phytest/cli.py` & `phytest-1.3.0/phytest/cli.py`

 * *Files identical despite different names*

### Comparing `phytest-1.2.0/phytest/main.py` & `phytest-1.3.0/phytest/main.py`

 * *Files identical despite different names*

### Comparing `phytest-1.2.0/phytest/report/logo.css` & `phytest-1.3.0/phytest/report/logo.css`

 * *Files identical despite different names*

### Comparing `phytest-1.2.0/phytest/utils.py` & `phytest-1.3.0/phytest/utils.py`

 * *Files identical despite different names*

### Comparing `phytest-1.2.0/pyproject.toml` & `phytest-1.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "phytest"
-version = "1.2.0"
+version = "1.3.0"
 description = "Quality control for phylogenetic pipelines using pytest"
 authors = ["Wytamma Wirth <wytamma.wirth@me.com>", "Simon Mutch <smutch@unimelb.edu.au>", "Rob Turnbull <robert.turnbull@unimelb.edu.au>"]
 readme = "README.rst"
 classifiers = [
     "Framework :: Pytest",
 ]
```

### Comparing `phytest-1.2.0/setup.py` & `phytest-1.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,242 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: phytest
+Version: 1.3.0
+Summary: Quality control for phylogenetic pipelines using pytest
+Author: Wytamma Wirth
+Author-email: wytamma.wirth@me.com
+Requires-Python: >=3.8,<3.11
+Classifier: Framework :: Pytest
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: biopython (>=1.79,<2.0)
+Requires-Dist: numpy (>=1.22.3,<2.0.0)
+Requires-Dist: phylo-treetime (>=0.8.6,<0.9.0)
+Requires-Dist: pytest (>=7.1.1,<8.0.0)
+Requires-Dist: pytest-html (>=3.1.1,<4.0.0)
+Requires-Dist: pytest-sugar (>=0.9.4,<0.10.0)
+Requires-Dist: pytest-xdist (>=3.2.0,<4.0.0)
+Requires-Dist: scipy (>=1.8.0,<2.0.0)
+Requires-Dist: typer (>=0.4.1,<0.5.0)
+Description-Content-Type: text/x-rst
 
-packages = \
-['phytest', 'phytest.bio']
+.. image:: https://raw.githubusercontent.com/phytest-devs/phytest/main/docs/images/logo.png
+  :alt: Phytest logo
 
-package_data = \
-{'': ['*'], 'phytest': ['report/*']}
+.. start-badges
 
-install_requires = \
-['biopython>=1.79,<2.0',
- 'numpy>=1.22.3,<2.0.0',
- 'phylo-treetime>=0.8.6,<0.9.0',
- 'pytest-html>=3.1.1,<4.0.0',
- 'pytest-sugar>=0.9.4,<0.10.0',
- 'pytest-xdist>=3.2.0,<4.0.0',
- 'pytest>=7.1.1,<8.0.0',
- 'scipy>=1.8.0,<2.0.0',
- 'typer>=0.4.1,<0.5.0']
-
-entry_points = \
-{'console_scripts': ['phytest = phytest.cli:app'],
- 'pytest11': ['phytest = phytest']}
-
-setup_kwargs = {
-    'name': 'phytest',
-    'version': '1.2.0',
-    'description': 'Quality control for phylogenetic pipelines using pytest',
-    'long_description': '.. image:: https://raw.githubusercontent.com/phytest-devs/phytest/main/docs/images/logo.png\n  :alt: Phytest logo\n\n.. start-badges\n\n|pypi badge| |tests badge| |coverage badge| |docs badge| |black badge| |pre-commit badge| |doi badge|\n\n\n.. |pypi badge| image:: https://img.shields.io/pypi/v/phytest.svg\n    :target: https://pypi.org/project/phytest/\n\n.. |tests badge| image:: https://github.com/phytest-devs/phytest/workflows/tests/badge.svg\n    :target: https://github.com/phytest-devs/phytest/actions\n\n.. |docs badge| image:: https://github.com/phytest-devs/phytest/workflows/docs/badge.svg\n    :target: https://phytest-devs.github.io/phytest/\n\n.. |black badge| image:: https://img.shields.io/badge/code%20style-black-000000.svg\n    :target: https://github.com/psf/black\n\n.. |coverage badge| image:: https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/smutch/e8160655e03d9015b1e93b97ed611f4f/raw/coverage-badge.json\n    :target: https://phytest-devs.github.io/phytest/coverage/\n\n.. |pre-commit badge| image:: https://results.pre-commit.ci/badge/github/phytest-devs/phytest/main.svg\n    :target: https://results.pre-commit.ci/latest/github/phytest-devs/phytest/main\n\n.. |doi badge| image:: https://img.shields.io/badge/DOI-10.1093%2Fbioinformatics%2Fbtac664-success.svg\n    :target: https://academic.oup.com/bioinformatics/article/38/22/5124/6751773\n\n.. end-badges\n\n\n\nPhytest: Quality Control for Phylogenetic Analyses.\n\n----\n\nDocumentation: https://phytest-devs.github.io/phytest\n\nCode: https://github.com/phytest-devs/phytest\n\nTutorials: https://github.com/phytest-devs?q=example\n\n----\n\n.. start-quickstart\n\nInstallation\n============\nInstall phytest using pip:\n\n.. code-block:: bash\n\n    pip install phytest\n\n\nQuick Start\n============\n\nPhytest is a tool for automating quality control checks on sequence, tree and metadata files during phylogenetic analyses.\nPhytest ensures that phylogenetic analyses meet user-defined quality control tests.\n\nHere we will create example data files to run our tests on.\n\nCreate an alignment fasta file :code:`example.fasta`\n\n.. code-block:: text\n\n    >Sequence_A\n    ATGAGATCCCCGATAGCGAGCTAGCGATCGCAGCGACTCAGCAGCTACAGCGCAGAGGAGAGAGAGGCCCCTATTTACTAGAGCTCCAGATATAGNNTAG\n    >Sequence_B\n    ATGAGATCCCCGATAGCGAGCTAGXGATCGCAGCGACTCAGCAGCTACAGCGCAGAGGAGAGAGAGGCCCCTATTTACTAGAGCTCCAGATATAGNNTAG\n    >Sequence_C\n    ATGAGA--CCCGATAGCGAGCTAGCGATCGCAGCGACTCAGCAGCTACAGCGCAGAGGAGAGAGAGGCCCCTATTTACTAGAGCTCCAGATATAGNNTAG\n    >Sequence_D\n    ATGAGATCCCCGATAGCGAGCTAGCGATNNNNNNNNNNNNNNNNNTACAGCGCAGAGGAGAGAGAGGCCCCTATTTACTAGAGCTCCAGATATAGNNTAG\n\nCreate a tree newick file :code:`example.tree`\n\n.. code-block:: text\n\n    (Sequence_A:1,Sequence_B:0.2,(Sequence_C:0.3,Sequence_D:0.4):0.5);\n\nWriting a test file\n########################\n\nWe want to enforce the follow constraints on our data:\n    1. The alignment has 4 sequences\n    2. The sequences have a length of 100\n    3. The sequences only contains the characters A, T, G, C, N and -\n    4. The sequences are allowed to only contain single base deletions\n    5. The longest stretch of Ns is 10\n    6. The tree has 4 tips\n    7. The tree is bifurcating\n    8. The alignment and tree have the same names\n    9. All internal branches are longer than the given threshold\n    10. There are no outlier branches in the tree\n\nWe can write these tests in a python files :code:`example.py`\n\n.. code-block:: python\n\n    from phytest import Alignment, Sequence, Tree\n\n\n    def test_alignment_has_4_sequences(alignment: Alignment):\n        alignment.assert_length(4)\n\n\n    def test_alignment_has_a_width_of_100(alignment: Alignment):\n        alignment.assert_width(100)\n\n\n    def test_sequences_only_contains_the_characters(sequence: Sequence):\n        sequence.assert_valid_alphabet(alphabet="ATGCN-")\n\n\n    def test_single_base_deletions(sequence: Sequence):\n        sequence.assert_longest_stretch_gaps(max=1)\n\n\n    def test_longest_stretch_of_Ns_is_10(sequence: Sequence):\n        sequence.assert_longest_stretch_Ns(max=10)\n\n\n    def test_tree_has_4_tips(tree: Tree):\n        tree.assert_number_of_tips(4)\n\n\n    def test_tree_is_bifurcating(tree: Tree):\n        tree.assert_is_bifurcating()\n\n\n    def test_aln_tree_match_names(alignment: Alignment, tree: Tree):\n        aln_names = [i.name for i in alignment]\n        tree.assert_tip_names(aln_names)\n\n\n    def test_all_internal_branches_lengths_above_threshold(tree: Tree, threshold=1e-4):\n        tree.assert_internal_branch_lengths(min=threshold)\n\n\n    def test_outlier_branches(tree: Tree):\n        # Here we create a custom function to detect outliers\n        import statistics\n\n        tips = tree.get_terminals()\n        branch_lengths = [t.branch_length for t in tips]\n        cut_off = statistics.mean(branch_lengths) + statistics.stdev(branch_lengths)\n        for tip in tips:\n            assert tip.branch_length < cut_off, f"Outlier tip \'{tip.name}\' (branch length = {tip.branch_length})!"\n\nRunning Phytest\n################\n\nWe can then run these tests on our data with :code:`phytest`:\n\n.. code-block:: bash\n\n    phytest examples/example.py -s examples/data/example.fasta -t examples/data/example.tree\n\nGenerate a report by adding :code:`--report report.html`.\n\n.. image:: https://raw.githubusercontent.com/phytest-devs/phytest/main/docs/images/report.png\n    :alt: HTML Report\n\nFrom the output we can see several tests failed:\n\n.. code-block::\n\n    FAILED examples/example.py::test_sequences_only_contains_the_characters[Sequence_B] - AssertionError: Invalid pattern found in \'Sequence_B\'!\n    FAILED examples/example.py::test_single_base_deletions[Sequence_C] - AssertionError: Longest stretch of \'-\' in \'Sequence_C\' > 1!\n    FAILED examples/example.py::test_longest_stretch_of_Ns_is_10[Sequence_D] - AssertionError: Longest stretch of \'N\' in \'Sequence_D\' > 10!\n    FAILED examples/example.py::test_outlier_branches - AssertionError: Outlier tip \'Sequence_A\' (branch length = 1.0)!\n\n    Results (0.07s):\n        15 passed\n        4 failed\n            - examples/example.py:12 test_sequences_only_contains_the_characters[Sequence_B]\n            - examples/example.py:16 test_single_base_deletions[Sequence_C]\n            - examples/example.py:20 test_longest_stretch_of_Ns_is_10[Sequence_D]\n            - examples/example.py:32 test_outlier_branches\n\n\n\n.. end-quickstart\n\nSee docs for more information https://phytest-devs.github.io/phytest.\n\nCitation\n============\n\n.. start-citation\n\nIf you use phytest, please cite the following paper:\n\nWytamma Wirth, Simon Mutch, Robert Turnbull, Sebastian Duchene, Phytest: quality control for phylogenetic analyses, Bioinformatics, Volume 38, Issue 22, 15 November 2022, Pages 5124–5125, https://doi.org/10.1093/bioinformatics/btac664\n\n\n.. code-block:: bibtex\n\n    @article{10.1093/bioinformatics/btac664,\n        author = {Wirth, Wytamma and Mutch, Simon and Turnbull, Robert and Duchene, Sebastian},\n        title = "{{Phytest: quality control for phylogenetic analyses}}",\n        journal = {Bioinformatics},\n        volume = {38},\n        number = {22},\n        pages = {5124-5125},\n        year = {2022},\n        month = {10},\n        issn = {1367-4803},\n        doi = {10.1093/bioinformatics/btac664},\n        url = {https://doi.org/10.1093/bioinformatics/btac664},\n        eprint = {https://academic.oup.com/bioinformatics/article-pdf/38/22/5124/47153886/btac664.pdf},\n    }\n\n\n.. end-citation\n',
-    'author': 'Wytamma Wirth',
-    'author_email': 'wytamma.wirth@me.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<3.11',
-}
+|pypi badge| |tests badge| |coverage badge| |docs badge| |black badge| |pre-commit badge| |doi badge|
 
 
-setup(**setup_kwargs)
+.. |pypi badge| image:: https://img.shields.io/pypi/v/phytest.svg
+    :target: https://pypi.org/project/phytest/
+
+.. |tests badge| image:: https://github.com/phytest-devs/phytest/workflows/tests/badge.svg
+    :target: https://github.com/phytest-devs/phytest/actions
+
+.. |docs badge| image:: https://github.com/phytest-devs/phytest/workflows/docs/badge.svg
+    :target: https://phytest-devs.github.io/phytest/
+
+.. |black badge| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+
+.. |coverage badge| image:: https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/smutch/e8160655e03d9015b1e93b97ed611f4f/raw/coverage-badge.json
+    :target: https://phytest-devs.github.io/phytest/coverage/
+
+.. |pre-commit badge| image:: https://results.pre-commit.ci/badge/github/phytest-devs/phytest/main.svg
+    :target: https://results.pre-commit.ci/latest/github/phytest-devs/phytest/main
+
+.. |doi badge| image:: https://img.shields.io/badge/DOI-10.1093%2Fbioinformatics%2Fbtac664-success.svg
+    :target: https://academic.oup.com/bioinformatics/article/38/22/5124/6751773
+
+.. end-badges
+
+
+
+Phytest: Quality Control for Phylogenetic Analyses.
+
+----
+
+Documentation: https://phytest-devs.github.io/phytest
+
+Code: https://github.com/phytest-devs/phytest
+
+Tutorials: https://github.com/phytest-devs?q=example
+
+----
+
+.. start-quickstart
+
+Installation
+============
+Install phytest using pip:
+
+.. code-block:: bash
+
+    pip install phytest
+
+
+Quick Start
+============
+
+Phytest is a tool for automating quality control checks on sequence, tree and metadata files during phylogenetic analyses.
+Phytest ensures that phylogenetic analyses meet user-defined quality control tests.
+
+Here we will create example data files to run our tests on.
+
+Create an alignment fasta file :code:`example.fasta`
+
+.. code-block:: text
+
+    >Sequence_A
+    ATGAGATCCCCGATAGCGAGCTAGCGATCGCAGCGACTCAGCAGCTACAGCGCAGAGGAGAGAGAGGCCCCTATTTACTAGAGCTCCAGATATAGNNTAG
+    >Sequence_B
+    ATGAGATCCCCGATAGCGAGCTAGXGATCGCAGCGACTCAGCAGCTACAGCGCAGAGGAGAGAGAGGCCCCTATTTACTAGAGCTCCAGATATAGNNTAG
+    >Sequence_C
+    ATGAGA--CCCGATAGCGAGCTAGCGATCGCAGCGACTCAGCAGCTACAGCGCAGAGGAGAGAGAGGCCCCTATTTACTAGAGCTCCAGATATAGNNTAG
+    >Sequence_D
+    ATGAGATCCCCGATAGCGAGCTAGCGATNNNNNNNNNNNNNNNNNTACAGCGCAGAGGAGAGAGAGGCCCCTATTTACTAGAGCTCCAGATATAGNNTAG
+
+Create a tree newick file :code:`example.tree`
+
+.. code-block:: text
+
+    (Sequence_A:1,Sequence_B:0.2,(Sequence_C:0.3,Sequence_D:0.4):0.5);
+
+Writing a test file
+########################
+
+We want to enforce the follow constraints on our data:
+    1. The alignment has 4 sequences
+    2. The sequences have a length of 100
+    3. The sequences only contains the characters A, T, G, C, N and -
+    4. The sequences are allowed to only contain single base deletions
+    5. The longest stretch of Ns is 10
+    6. The tree has 4 tips
+    7. The tree is bifurcating
+    8. The alignment and tree have the same names
+    9. All internal branches are longer than the given threshold
+    10. There are no outlier branches in the tree
+
+We can write these tests in a python files :code:`example.py`
+
+.. code-block:: python
+
+    from phytest import Alignment, Sequence, Tree
+
+
+    def test_alignment_has_4_sequences(alignment: Alignment):
+        alignment.assert_length(4)
+
+
+    def test_alignment_has_a_width_of_100(alignment: Alignment):
+        alignment.assert_width(100)
+
+
+    def test_sequences_only_contains_the_characters(sequence: Sequence):
+        sequence.assert_valid_alphabet(alphabet="ATGCN-")
+
+
+    def test_single_base_deletions(sequence: Sequence):
+        sequence.assert_longest_stretch_gaps(max=1)
+
+
+    def test_longest_stretch_of_Ns_is_10(sequence: Sequence):
+        sequence.assert_longest_stretch_Ns(max=10)
+
+
+    def test_tree_has_4_tips(tree: Tree):
+        tree.assert_number_of_tips(4)
+
+
+    def test_tree_is_bifurcating(tree: Tree):
+        tree.assert_is_bifurcating()
+
+
+    def test_aln_tree_match_names(alignment: Alignment, tree: Tree):
+        aln_names = [i.name for i in alignment]
+        tree.assert_tip_names(aln_names)
+
+
+    def test_all_internal_branches_lengths_above_threshold(tree: Tree, threshold=1e-4):
+        tree.assert_internal_branch_lengths(min=threshold)
+
+
+    def test_outlier_branches(tree: Tree):
+        # Here we create a custom function to detect outliers
+        import statistics
+
+        tips = tree.get_terminals()
+        branch_lengths = [t.branch_length for t in tips]
+        cut_off = statistics.mean(branch_lengths) + statistics.stdev(branch_lengths)
+        for tip in tips:
+            assert tip.branch_length < cut_off, f"Outlier tip '{tip.name}' (branch length = {tip.branch_length})!"
+
+Running Phytest
+################
+
+We can then run these tests on our data with :code:`phytest`:
+
+.. code-block:: bash
+
+    phytest examples/example.py -s examples/data/example.fasta -t examples/data/example.tree
+
+Generate a report by adding :code:`--report report.html`.
+
+.. image:: https://raw.githubusercontent.com/phytest-devs/phytest/main/docs/images/report.png
+    :alt: HTML Report
+
+From the output we can see several tests failed:
+
+.. code-block::
+
+    FAILED examples/example.py::test_sequences_only_contains_the_characters[Sequence_B] - AssertionError: Invalid pattern found in 'Sequence_B'!
+    FAILED examples/example.py::test_single_base_deletions[Sequence_C] - AssertionError: Longest stretch of '-' in 'Sequence_C' > 1!
+    FAILED examples/example.py::test_longest_stretch_of_Ns_is_10[Sequence_D] - AssertionError: Longest stretch of 'N' in 'Sequence_D' > 10!
+    FAILED examples/example.py::test_outlier_branches - AssertionError: Outlier tip 'Sequence_A' (branch length = 1.0)!
+
+    Results (0.07s):
+        15 passed
+        4 failed
+            - examples/example.py:12 test_sequences_only_contains_the_characters[Sequence_B]
+            - examples/example.py:16 test_single_base_deletions[Sequence_C]
+            - examples/example.py:20 test_longest_stretch_of_Ns_is_10[Sequence_D]
+            - examples/example.py:32 test_outlier_branches
+
+
+
+.. end-quickstart
+
+See docs for more information https://phytest-devs.github.io/phytest.
+
+Citation
+============
+
+.. start-citation
+
+If you use phytest, please cite the following paper:
+
+Wytamma Wirth, Simon Mutch, Robert Turnbull, Sebastian Duchene, Phytest: quality control for phylogenetic analyses, Bioinformatics, Volume 38, Issue 22, 15 November 2022, Pages 5124–5125, https://doi.org/10.1093/bioinformatics/btac664
+
+
+.. code-block:: bibtex
+
+    @article{10.1093/bioinformatics/btac664,
+        author = {Wirth, Wytamma and Mutch, Simon and Turnbull, Robert and Duchene, Sebastian},
+        title = "{{Phytest: quality control for phylogenetic analyses}}",
+        journal = {Bioinformatics},
+        volume = {38},
+        number = {22},
+        pages = {5124-5125},
+        year = {2022},
+        month = {10},
+        issn = {1367-4803},
+        doi = {10.1093/bioinformatics/btac664},
+        url = {https://doi.org/10.1093/bioinformatics/btac664},
+        eprint = {https://academic.oup.com/bioinformatics/article-pdf/38/22/5124/47153886/btac664.pdf},
+    }
+
+
+.. end-citation
+
```

