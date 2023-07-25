# Comparing `tmp/islearn-0.2.8.tar.gz` & `tmp/islearn-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "islearn-0.2.8.tar", last modified: Thu Aug 18 12:37:53 2022, max compression
+gzip compressed data, was "islearn-0.2.9.tar", last modified: Fri Aug 19 12:34:45 2022, max compression
```

## Comparing `islearn-0.2.8.tar` & `islearn-0.2.9.tar`

### file list

```diff
@@ -1,40 +1,39 @@
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2022-08-18 12:37:53.599213 islearn-0.2.8/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)    35096 2021-08-03 15:42:33.000000 islearn-0.2.8/LICENSE
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)    51809 2022-08-18 12:37:53.599847 islearn-0.2.8/PKG-INFO
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)    10466 2022-08-04 14:44:55.000000 islearn-0.2.8/README.md
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      853 2022-08-18 12:35:57.000000 islearn-0.2.8/pyproject.toml
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     1404 2022-08-18 12:37:53.600878 islearn-0.2.8/setup.cfg
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      118 2022-02-01 09:10:05.000000 islearn-0.2.8/setup.py
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2022-08-18 12:37:53.580959 islearn-0.2.8/src/
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2022-08-18 12:37:53.589536 islearn-0.2.8/src/islearn/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)       22 2022-08-18 12:36:02.000000 islearn-0.2.8/src/islearn/__init__.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     8961 2022-08-03 15:37:36.000000 islearn-0.2.8/src/islearn/helpers.py
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2022-08-18 12:37:53.594766 islearn-0.2.8/src/islearn/isla_language/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)    19788 2022-08-08 09:33:09.000000 islearn-0.2.8/src/islearn/isla_language/IslaLanguageLexer.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)    11738 2022-08-08 09:33:09.000000 islearn-0.2.8/src/islearn/isla_language/IslaLanguageListener.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)    78131 2022-08-08 09:33:09.000000 islearn-0.2.8/src/islearn/isla_language/IslaLanguageParser.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)        0 2022-02-02 14:46:45.000000 islearn-0.2.8/src/islearn/isla_language/__init__.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     6743 2022-08-18 12:33:27.000000 islearn-0.2.8/src/islearn/islearn_predicates.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)    18183 2022-08-08 09:40:55.000000 islearn-0.2.8/src/islearn/language.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)    90595 2022-08-04 09:29:59.000000 islearn-0.2.8/src/islearn/learner.py
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2022-08-18 12:37:53.595680 islearn-0.2.8/src/islearn/mexpr_lexer/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     4335 2022-08-08 09:33:08.000000 islearn-0.2.8/src/islearn/mexpr_lexer/MexprLexer.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)        0 2022-02-02 14:46:45.000000 islearn-0.2.8/src/islearn/mexpr_lexer/__init__.py
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2022-08-18 12:37:53.597255 islearn-0.2.8/src/islearn/mexpr_parser/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)    15149 2022-08-08 09:33:09.000000 islearn-0.2.8/src/islearn/mexpr_parser/MexprParser.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     2495 2022-08-08 09:33:09.000000 islearn-0.2.8/src/islearn/mexpr_parser/MexprParserListener.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)        0 2022-02-02 14:46:45.000000 islearn-0.2.8/src/islearn/mexpr_parser/__init__.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     7618 2022-08-03 15:37:36.000000 islearn-0.2.8/src/islearn/mutation.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     7206 2022-08-04 14:34:08.000000 islearn-0.2.8/src/islearn/parse_tree_utils.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     1021 2022-08-18 12:33:12.000000 islearn-0.2.8/src/islearn/parser.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     9573 2022-08-08 09:48:26.000000 islearn-0.2.8/src/islearn/patterns.toml
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     4394 2022-03-11 15:01:14.000000 islearn-0.2.8/src/islearn/reducer.py
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2022-08-18 12:37:53.591890 islearn-0.2.8/src/islearn.egg-info/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)    51809 2022-08-18 12:37:53.000000 islearn-0.2.8/src/islearn.egg-info/PKG-INFO
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      947 2022-08-18 12:37:53.000000 islearn-0.2.8/src/islearn.egg-info/SOURCES.txt
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)        1 2022-08-18 12:37:53.000000 islearn-0.2.8/src/islearn.egg-info/dependency_links.txt
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      400 2022-08-18 12:37:53.000000 islearn-0.2.8/src/islearn.egg-info/requires.txt
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)       34 2022-08-18 12:37:53.000000 islearn-0.2.8/src/islearn.egg-info/top_level.txt
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2022-08-18 12:37:53.598390 islearn-0.2.8/src/islearn_example_languages/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)       50 2022-08-09 04:27:16.000000 islearn-0.2.8/src/islearn_example_languages/__init__.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)    20338 2022-08-09 07:34:32.000000 islearn-0.2.8/src/islearn_example_languages/languages.py
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2022-08-19 12:34:45.118735 islearn-0.2.9/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)    35096 2021-08-03 15:42:33.000000 islearn-0.2.9/LICENSE
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)    51637 2022-08-19 12:34:45.119078 islearn-0.2.9/PKG-INFO
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)    10294 2022-08-19 05:03:39.000000 islearn-0.2.9/README.md
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      853 2022-08-19 12:33:58.000000 islearn-0.2.9/pyproject.toml
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     1403 2022-08-19 12:34:45.119677 islearn-0.2.9/setup.cfg
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      118 2022-02-01 09:10:05.000000 islearn-0.2.9/setup.py
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2022-08-19 12:34:45.105327 islearn-0.2.9/src/
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2022-08-19 12:34:45.111840 islearn-0.2.9/src/islearn/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)       22 2022-08-19 12:33:54.000000 islearn-0.2.9/src/islearn/__init__.py
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     8961 2022-08-19 09:07:45.000000 islearn-0.2.9/src/islearn/helpers.py
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2022-08-19 12:34:45.114486 islearn-0.2.9/src/islearn/isla_language/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)    19788 2022-08-08 09:33:09.000000 islearn-0.2.9/src/islearn/isla_language/IslaLanguageLexer.py
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)    11738 2022-08-08 09:33:09.000000 islearn-0.2.9/src/islearn/isla_language/IslaLanguageListener.py
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)    78131 2022-08-08 09:33:09.000000 islearn-0.2.9/src/islearn/isla_language/IslaLanguageParser.py
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)        0 2022-02-02 14:46:45.000000 islearn-0.2.9/src/islearn/isla_language/__init__.py
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     6740 2022-08-19 11:58:20.000000 islearn-0.2.9/src/islearn/islearn_predicates.py
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)    18302 2022-08-19 12:22:11.000000 islearn-0.2.9/src/islearn/language.py
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)    88571 2022-08-19 09:46:38.000000 islearn-0.2.9/src/islearn/learner.py
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2022-08-19 12:34:45.114899 islearn-0.2.9/src/islearn/mexpr_lexer/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     4335 2022-08-08 09:33:08.000000 islearn-0.2.9/src/islearn/mexpr_lexer/MexprLexer.py
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)        0 2022-02-02 14:46:45.000000 islearn-0.2.9/src/islearn/mexpr_lexer/__init__.py
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2022-08-19 12:34:45.117621 islearn-0.2.9/src/islearn/mexpr_parser/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)    15149 2022-08-08 09:33:09.000000 islearn-0.2.9/src/islearn/mexpr_parser/MexprParser.py
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     2495 2022-08-08 09:33:09.000000 islearn-0.2.9/src/islearn/mexpr_parser/MexprParserListener.py
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)        0 2022-02-02 14:46:45.000000 islearn-0.2.9/src/islearn/mexpr_parser/__init__.py
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     7618 2022-08-03 15:37:36.000000 islearn-0.2.9/src/islearn/mutation.py
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     7863 2022-08-19 09:43:13.000000 islearn-0.2.9/src/islearn/parse_tree_utils.py
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     9573 2022-08-19 12:12:46.000000 islearn-0.2.9/src/islearn/patterns.toml
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     4394 2022-03-11 15:01:14.000000 islearn-0.2.9/src/islearn/reducer.py
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2022-08-19 12:34:45.113415 islearn-0.2.9/src/islearn.egg-info/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)    51637 2022-08-19 12:34:45.000000 islearn-0.2.9/src/islearn.egg-info/PKG-INFO
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      925 2022-08-19 12:34:45.000000 islearn-0.2.9/src/islearn.egg-info/SOURCES.txt
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)        1 2022-08-19 12:34:45.000000 islearn-0.2.9/src/islearn.egg-info/dependency_links.txt
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      399 2022-08-19 12:34:45.000000 islearn-0.2.9/src/islearn.egg-info/requires.txt
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)       34 2022-08-19 12:34:45.000000 islearn-0.2.9/src/islearn.egg-info/top_level.txt
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2022-08-19 12:34:45.118489 islearn-0.2.9/src/islearn_example_languages/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)       50 2022-08-09 04:27:16.000000 islearn-0.2.9/src/islearn_example_languages/__init__.py
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)    20489 2022-08-19 12:04:43.000000 islearn-0.2.9/src/islearn_example_languages/languages.py
```

### Comparing `islearn-0.2.8/LICENSE` & `islearn-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `islearn-0.2.8/PKG-INFO` & `islearn-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: islearn
-Version: 0.2.8
+Version: 0.2.9
 Summary: ISLearn (Learning ISLa input invariants)
 Home-page: https://github.com/rindPHI/islearn
 Author: Dominic Steinhöfel
 Author-email: Dominic Steinhöfel <dominic.steinhoefel@cispa.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -844,15 +844,14 @@
 | reduce_all_inputs                           | False      | If `True`, all inputs are reduced. Reduction of learning inputs can be specifically disabled.                |
 | generate_new_learning_samples               | True       | Only if `True`, the fuzzers are used to generate further learning examples.                                  |
 | do_generate_more_inputs                     | True       | Only if `True`, any further examples (positive, negative) are generated by the fuzzers.                      |
 | filter_inputs_for_learning_by_kpaths        | True       | If `True`, learning inputs are filtered k-paths: Retain only those with new k-path coverage information.     |
 | mexpr_expansion_limit                       | 1          | To what depth should the learner search for instantiations of match expressions?                             |
 | max_nonterminals_in_mexpr                   | None       | How many nonterminals are allowed in match expressions? `None` means no restriction.                         |
 | exclude_nonterminals                        | None       | "Irrelevant" grammar nonterminals. Reduces search space. Example: White space nonterminals.                  |
-| perform_static_implication_check            | False      | Statically exclude weaker invariants by a translation to Z3. Rather slow, handle with care.                  |
 | k                                           | 3          | The `k` from `k`-Paths. Used by the input generators and filters.                                            |
 
 ## Install, Build, Test
 
 ISLearn depends on Python 3.10 and the Python header files. To compile all of ISLearns's dependencies, you need
 gcc, g++ make, and cmake. To check out the current ISLearn version, git will be needed. Furthermore, 
 python3.10-venv is required to run ISLearn in a virtual environment.
```

### Comparing `islearn-0.2.8/README.md` & `islearn-0.2.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,14 @@
 | reduce_all_inputs                           | False      | If `True`, all inputs are reduced. Reduction of learning inputs can be specifically disabled.                |
 | generate_new_learning_samples               | True       | Only if `True`, the fuzzers are used to generate further learning examples.                                  |
 | do_generate_more_inputs                     | True       | Only if `True`, any further examples (positive, negative) are generated by the fuzzers.                      |
 | filter_inputs_for_learning_by_kpaths        | True       | If `True`, learning inputs are filtered k-paths: Retain only those with new k-path coverage information.     |
 | mexpr_expansion_limit                       | 1          | To what depth should the learner search for instantiations of match expressions?                             |
 | max_nonterminals_in_mexpr                   | None       | How many nonterminals are allowed in match expressions? `None` means no restriction.                         |
 | exclude_nonterminals                        | None       | "Irrelevant" grammar nonterminals. Reduces search space. Example: White space nonterminals.                  |
-| perform_static_implication_check            | False      | Statically exclude weaker invariants by a translation to Z3. Rather slow, handle with care.                  |
 | k                                           | 3          | The `k` from `k`-Paths. Used by the input generators and filters.                                            |
 
 ## Install, Build, Test
 
 ISLearn depends on Python 3.10 and the Python header files. To compile all of ISLearns's dependencies, you need
 gcc, g++ make, and cmake. To check out the current ISLearn version, git will be needed. Furthermore, 
 python3.10-venv is required to run ISLearn in a virtual environment.
```

### Comparing `islearn-0.2.8/pyproject.toml` & `islearn-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "setuptools-antlr",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "islearn"
-version = "0.2.8"
+version = "0.2.9"
 authors = [
   { name="Dominic Steinhöfel", email="dominic.steinhoefel@cispa.de" },
 ]
 description = "ISLearn (Learning ISLa input invariants)"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10"
```

### Comparing `islearn-0.2.8/setup.cfg` & `islearn-0.2.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	= src
 packages = find:
 python_requires = >=3.10
 include_package_data = True
 install_requires = antlr4-python3-runtime>=4.10
 	datrie>=0.8.2
 	grammar_graph>=0.1.0
-	isla-solver>=0.8.13
+	isla-solver>=0.9.3
 	pathos>=0.2.9
 	requests>=2.28.1
 	toml>=0.10.2
 	z3-solver>=4.10.2.0
 
 [options.extras_require]
 test =
```

### Comparing `islearn-0.2.8/src/islearn/helpers.py` & `islearn-0.2.9/src/islearn/helpers.py`

 * *Files identical despite different names*

### Comparing `islearn-0.2.8/src/islearn/isla_language/IslaLanguageLexer.py` & `islearn-0.2.9/src/islearn/isla_language/IslaLanguageLexer.py`

 * *Files identical despite different names*

### Comparing `islearn-0.2.8/src/islearn/isla_language/IslaLanguageListener.py` & `islearn-0.2.9/src/islearn/isla_language/IslaLanguageListener.py`

 * *Files identical despite different names*

### Comparing `islearn-0.2.8/src/islearn/isla_language/IslaLanguageParser.py` & `islearn-0.2.9/src/islearn/isla_language/IslaLanguageParser.py`

 * *Files identical despite different names*

### Comparing `islearn-0.2.8/src/islearn/islearn_predicates.py` & `islearn-0.2.9/src/islearn/islearn_predicates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import string
 from functools import lru_cache
 from typing import List, Sequence, Optional, Tuple
 
 from isla import language
 from isla.helpers import srange
+from isla.parser import PEGParser
 from isla.type_defs import Grammar
 
 from islearn.helpers import remove_spaces
-from islearn.parser import PEGParser
 
 
 def internet_checksum(
         _: Optional[Grammar],
         header: language.DerivationTree,
         checksum_tree: language.DerivationTree) -> language.SemPredEvalResult:
     if not header.is_complete():
```

### Comparing `islearn-0.2.8/src/islearn/language.py` & `islearn-0.2.9/src/islearn/language.py`

 * *Files 1% similar despite different names*

```diff
@@ -413,7 +413,11 @@
         result = smt_expr_to_str(formula.formula)
 
         for variable in formula.free_variables():
             if isinstance(variable, StringPlaceholderVariableTypes):
                 result = result.replace(variable.name, str(variable))
 
         return [result]
+
+
+def unparse_abstract_isla(formula: Formula, indent="  "):
+    return AbstractISLaUnparser(formula, indent).unparse()
```

### Comparing `islearn-0.2.8/src/islearn/learner.py` & `islearn-0.2.9/src/islearn/learner.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,35 +12,36 @@
 
 import datrie
 import isla.fuzzer
 import toml
 import z3
 from grammar_graph import gg
 from isla import language, isla_predicates
-from isla.evaluator import evaluate, matches_for_quantified_formula, implies
+from isla.evaluator import evaluate, matches_for_quantified_formula
 from isla.helpers import RE_NONTERMINAL, weighted_geometric_mean, \
-    is_nonterminal, dict_of_lists_to_list_of_dicts, get_subtrie, path_to_trie_key, canonical
+    is_nonterminal, dict_of_lists_to_list_of_dicts, canonical
 from isla.isla_predicates import reachable
 from isla.language import set_smt_auto_eval, ensure_unique_bound_variables
 from isla.solver import ISLaSolver
 from isla.three_valued_truth import ThreeValuedTruth
+from isla.trie import path_to_trie_key
 from isla.type_defs import Grammar, ParseTree, Path
 from isla.z3_helpers import z3_subst, evaluate_z3_expression, is_valid, \
     DomainError
 from pathos import multiprocessing as pmp
 
 from islearn.helpers import connected_chains, transitive_closure, tree_in, \
     is_int, is_float, e_assert
 from islearn.language import NonterminalPlaceholderVariable, PlaceholderVariable, \
     NonterminalStringPlaceholderVariable, parse_abstract_isla, StringPlaceholderVariable, \
     AbstractISLaUnparser, MexprPlaceholderVariable, AbstractBindExpression, DisjunctiveStringsPlaceholderVariable, \
     StringPlaceholderVariableTypes
 from islearn.mutation import MutationFuzzer
 from islearn.parse_tree_utils import replace_path, expand_tree, tree_leaves, \
-    get_subtree, tree_paths, trie_from_parse_tree, next_trie_key, tree_from_paths, Tree
+    get_subtree, tree_paths, trie_from_parse_tree, next_trie_key, tree_from_paths, Tree, get_subtrie
 from islearn.reducer import InputReducer
 
 STANDARD_PATTERNS_REPO = "patterns.toml"
 logger = logging.getLogger("learner")
 
 
 class TruthTableRow:
@@ -239,15 +240,14 @@
             max_nonterminals_in_mexpr: Optional[int] = None,
             min_recall: float = .9,
             min_specificity: float = .6,
             max_disjunction_size: int = 1,
             max_conjunction_size: int = 2,
             exclude_nonterminals: Optional[Iterable[str]] = None,
             include_negations_in_disjunctions: bool = False,
-            perform_static_implication_check: bool = False,
             reduce_inputs_for_learning: bool = True,
             reduce_all_inputs: bool = False,
             generate_new_learning_samples: bool = True,
             do_generate_more_inputs: bool = True,
             filter_inputs_for_learning_by_kpaths: bool = True,
     ):
         # We add extended caching certain, crucial functions.
@@ -269,15 +269,14 @@
         self.mexpr_expansion_limit = mexpr_expansion_limit
         self.max_nonterminals_in_mexpr = max_nonterminals_in_mexpr
         self.min_recall = min_recall
         self.min_specificity = min_specificity
         self.max_disjunction_size = max_disjunction_size
         self.max_conjunction_size = max_conjunction_size
         self.exclude_nonterminals = exclude_nonterminals or set([])
-        self.perform_static_implication_check = perform_static_implication_check
         self.include_negations_in_disjunctions = include_negations_in_disjunctions
         self.reduce_inputs_for_learning = reduce_inputs_for_learning
         self.reduce_all_inputs = reduce_all_inputs
         self.generate_new_learning_samples = generate_new_learning_samples
         self.do_generate_more_inputs = do_generate_more_inputs
         self.filter_inputs_for_learning_by_kpaths = filter_inputs_for_learning_by_kpaths
 
@@ -425,54 +424,14 @@
         logger.info(
             "%d invariants with recall >= %d%% remain after filtering.",
             len(invariants),
             int(self.min_recall * 100))
 
         logger.debug("Invariants:\n%s", "\n\n".join(map(lambda f: language.ISLaUnparser(f).unparse(), invariants)))
 
-        if self.perform_static_implication_check:
-            # We eliminate rows in recall_truth_table whose formula is implied by that of
-            # another row with the same (higher should be impossible...) recall.
-            def check_is_implied(row: TruthTableRow) -> Optional[TruthTableRow]:
-                if any(implies(other_row.formula, row.formula, self.canonical_grammar)
-                       for other_row in recall_truth_table
-                       if (row != other_row and
-                           other_row.eval_result() >= row.eval_result() > 0)):
-                    return row
-
-                return None
-
-            with pmp.ProcessingPool(processes=pmp.cpu_count()) as pool:
-                for row_to_remove in pool.uimap(check_is_implied, list(recall_truth_table)):
-                    row_to_remove: TruthTableRow
-                    if row_to_remove is not None:
-                        recall_truth_table.remove(row_to_remove)
-                        if precision_truth_table is not None:
-                            precision_truth_table.remove(precision_truth_table[row_to_remove.formula])
-
-            # invariants = {
-            #     invariant_1
-            #     for idx_1, invariant_1 in enumerate(invariants)
-            #     if not any(
-            #         implies(invariant_2, invariant_1, self.canonical_grammar)
-            #         for idx_2, invariant_2 in enumerate(invariants)
-            #         if idx_1 != idx_2
-            #     )
-            # }
-
-            invariants = {
-                row.formula for row in recall_truth_table
-                if row.eval_result() >= self.min_recall
-            }
-
-            logger.info(
-                "%d invariant candidates with recall >= %d%% remain after implication check.",
-                len(invariants),
-                int(self.min_recall * 100))
-
         if self.max_disjunction_size > 1:
             logger.info("Calculating recall of Boolean combinations.")
 
             disjunctive_recall_truthtable = copy.deepcopy(recall_truth_table)
             assert precision_truth_table is None or len(disjunctive_recall_truthtable) == len(precision_truth_table)
 
             for level in range(2, self.max_disjunction_size + 1):
@@ -631,15 +590,15 @@
         ]
 
         patterns = [
             parse_abstract_isla(pattern, self.grammar) if isinstance(pattern, str)
             else pattern
             for pattern in patterns]
 
-        tries: List[datrie.Trie] = [inp.trie() for inp in inputs]
+        tries: List[datrie.Trie] = [inp.trie().trie for inp in inputs]
 
         result: Set[language.Formula] = set([])
 
         for pattern in patterns:
             logger.debug("Instantiating pattern\n%s", AbstractISLaUnparser(pattern).unparse())
             set_smt_auto_eval(pattern, False)
 
@@ -1671,15 +1630,15 @@
             assert all(var in assignment for assignment in new_assignments for var in mexpr_placeholder.variables)
             if isinstance(formula, language.ForallFormula):
                 new_assignments = new_assignments[:3]
         else:
             new_assignments = [
                 {var: (in_path + path, tree) for var, (path, tree) in new_assignment.items()}
                 for new_assignment in matches_for_quantified_formula(
-                    formula, grammar, in_inst, {}, trie=get_subtrie(trie, in_path))]
+                    formula, grammar, in_inst, {})]
 
         if not new_assignments:
             return ThreeValuedTruth.false()
 
         new_assignments = [
             new_assignment | assignments
             for new_assignment in new_assignments]
```

### Comparing `islearn-0.2.8/src/islearn/mexpr_lexer/MexprLexer.py` & `islearn-0.2.9/src/islearn/mexpr_lexer/MexprLexer.py`

 * *Files identical despite different names*

### Comparing `islearn-0.2.8/src/islearn/mexpr_parser/MexprParser.py` & `islearn-0.2.9/src/islearn/mexpr_parser/MexprParser.py`

 * *Files identical despite different names*

### Comparing `islearn-0.2.8/src/islearn/mexpr_parser/MexprParserListener.py` & `islearn-0.2.9/src/islearn/mexpr_parser/MexprParserListener.py`

 * *Files identical despite different names*

### Comparing `islearn-0.2.8/src/islearn/mutation.py` & `islearn-0.2.9/src/islearn/mutation.py`

 * *Files identical despite different names*

### Comparing `islearn-0.2.8/src/islearn/parse_tree_utils.py` & `islearn-0.2.9/src/islearn/parse_tree_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import math
 from typing import List, Callable, Tuple, Generator, Optional, Any, Sequence, TypeVar, Dict, cast
 
 import datrie
-from isla.helpers import is_nonterminal, mk_subtree_trie, path_to_trie_key
+from isla.helpers import is_nonterminal
+from isla.trie import path_to_trie_key
 from isla.type_defs import Path, CanonicalGrammar, ParseTree
 
 T = TypeVar("T")
 S = TypeVar("S")
 Tree = Tuple[T, Optional[List['Tree[T]']]]
 DictTree = Dict[T, 'DictTree']
 
@@ -144,15 +145,14 @@
 
     result: List[Tuple[Path, Tree[T]]] = []
     traverse_tree(tree, action, kind=TRAVERSE_PREORDER)
     return result
 
 
 def trie_from_parse_tree(tree: Tree) -> datrie.Trie:
-    pass
     trie = mk_subtree_trie()  # Works for up to 30 children of a node
     for path, subtree in tree_paths(tree):
         trie[path_to_trie_key(path)] = (path, subtree)
     return trie
 
 
 def next_trie_key(trie: datrie.Trie, path: Path | str) -> Optional[str]:
@@ -168,14 +168,36 @@
             maybe_next_key = prefix[:-1] + chr(ord(prefix[-1]) + 1)
             if trie.keys(maybe_next_key):
                 return maybe_next_key
 
         return None
 
 
+def mk_subtree_trie() -> datrie.Trie:
+    return datrie.Trie([chr(i) for i in range(30)])
+
+
+def get_subtrie(trie: datrie.Trie, new_root_path: Path | str) -> datrie.Trie:
+    subtrees_trie = mk_subtree_trie()
+
+    if isinstance(new_root_path, str):
+        root_key = new_root_path
+        root_path_len = len(root_key) - 1
+    else:
+        assert isinstance(new_root_path, tuple)
+        root_key = path_to_trie_key(new_root_path)
+        root_path_len = len(new_root_path)
+
+    for suffix in trie.suffixes(root_key):
+        path, tree = trie[root_key + suffix]
+        subtrees_trie[chr(1) + suffix] = (path[root_path_len:], tree)
+
+    return subtrees_trie
+
+
 def tree_to_string(tree: Tree, show_open_leaves: bool = False) -> str:
     result = []
     stack = [tree]
 
     while stack:
         node = stack.pop(0)
         symbol, children = node
```

### Comparing `islearn-0.2.8/src/islearn/patterns.toml` & `islearn-0.2.9/src/islearn/patterns.toml`

 * *Files identical despite different names*

### Comparing `islearn-0.2.8/src/islearn/reducer.py` & `islearn-0.2.9/src/islearn/reducer.py`

 * *Files identical despite different names*

### Comparing `islearn-0.2.8/src/islearn.egg-info/PKG-INFO` & `islearn-0.2.9/src/islearn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: islearn
-Version: 0.2.8
+Version: 0.2.9
 Summary: ISLearn (Learning ISLa input invariants)
 Home-page: https://github.com/rindPHI/islearn
 Author: Dominic Steinhöfel
 Author-email: Dominic Steinhöfel <dominic.steinhoefel@cispa.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -844,15 +844,14 @@
 | reduce_all_inputs                           | False      | If `True`, all inputs are reduced. Reduction of learning inputs can be specifically disabled.                |
 | generate_new_learning_samples               | True       | Only if `True`, the fuzzers are used to generate further learning examples.                                  |
 | do_generate_more_inputs                     | True       | Only if `True`, any further examples (positive, negative) are generated by the fuzzers.                      |
 | filter_inputs_for_learning_by_kpaths        | True       | If `True`, learning inputs are filtered k-paths: Retain only those with new k-path coverage information.     |
 | mexpr_expansion_limit                       | 1          | To what depth should the learner search for instantiations of match expressions?                             |
 | max_nonterminals_in_mexpr                   | None       | How many nonterminals are allowed in match expressions? `None` means no restriction.                         |
 | exclude_nonterminals                        | None       | "Irrelevant" grammar nonterminals. Reduces search space. Example: White space nonterminals.                  |
-| perform_static_implication_check            | False      | Statically exclude weaker invariants by a translation to Z3. Rather slow, handle with care.                  |
 | k                                           | 3          | The `k` from `k`-Paths. Used by the input generators and filters.                                            |
 
 ## Install, Build, Test
 
 ISLearn depends on Python 3.10 and the Python header files. To compile all of ISLearns's dependencies, you need
 gcc, g++ make, and cmake. To check out the current ISLearn version, git will be needed. Furthermore, 
 python3.10-venv is required to run ISLearn in a virtual environment.
```

### Comparing `islearn-0.2.8/src/islearn.egg-info/SOURCES.txt` & `islearn-0.2.9/src/islearn.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 src/islearn/__init__.py
 src/islearn/helpers.py
 src/islearn/islearn_predicates.py
 src/islearn/language.py
 src/islearn/learner.py
 src/islearn/mutation.py
 src/islearn/parse_tree_utils.py
-src/islearn/parser.py
 src/islearn/patterns.toml
 src/islearn/reducer.py
 src/islearn.egg-info/PKG-INFO
 src/islearn.egg-info/SOURCES.txt
 src/islearn.egg-info/dependency_links.txt
 src/islearn.egg-info/requires.txt
 src/islearn.egg-info/top_level.txt
```

### Comparing `islearn-0.2.8/src/islearn_example_languages/languages.py` & `islearn-0.2.9/src/islearn_example_languages/languages.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,42 +14,55 @@
 from isla.helpers import srange, crange
 from isla.type_defs import Grammar
 
 toml_grammar = {
     "<start>": ["<document>"],
     "<document>": ["<expressions>"],
     "<expressions>": ["<expression><NL><expressions>", "<expression>"],
-    "<expression>": ["<key_value><comment>", "<table><comment>", "<comment>"],
+    "<expression>": ["<table><comment>", "<key_value><comment>", "<comment>"],
     "<comment>": ["# <STR_NO_NL>", ""],
     "<STR_NO_NL>": ["<STR_NO_NL_CHARS><STR_NO_NL>", ""],
     "<STR_NO_NL_CHARS>": list(set(srange(string.printable)) - {"\n"}),
     "<key_value>": ["<key> = <value>"],
     "<key>": ["<dotted_key>", "<simple_key>"],
     "<simple_key>": ["<quoted_key>", "<unquoted_key>"],
     "<unquoted_key>": ["<UNQUOTED_KEY>"],
     "<quoted_key>": ["<BASIC_STRING>", "<LITERAL_STRING>"],
     "<dotted_key>": ["<simple_key><dot_simple_key>"],
     "<dot_simple_key>": [".<simple_key><dot_simple_key>", ".<simple_key>"],
     "<value>": ["<string>", "<date_time>", "<LOCAL_DATE>", "<floating_point>", "<integer>", "<bool>", "<array>",
                 "<inline_table>"],
     "<string>": ["<ML_BASIC_STRING>", "<BASIC_STRING>", "<ML_LITERAL_STRING>", "<LITERAL_STRING>"],
-    "<integer>": ["<DEC_INT>", "<HEX_INT>", "<OCT_INT>", "<BIN_INT>"],
+    "<integer>": ["<HEX_INT>", "<OCT_INT>", "<BIN_INT>", "<DEC_INT>"],
     "<floating_point>": ["<FLOAT>", "<INF>", "<NAN>"],
     "<bool>": ["<BOOLEAN>"],
     "<date_time>": ["<OFFSET_DATE_TIME>", "<LOCAL_DATE_TIME>", "<LOCAL_DATE>", "<LOCAL_TIME>"],
     "<array>": ["[<opt_array_values><comment_nl_or_nl>]"],
     "<opt_array_values>": ["<array_values>", ""],
     "<array_values>": [
-        "<comment_nl_or_nl><value><nl_or_comment><opt_comma>",
-        "<comment_nl_or_nl><value><nl_or_comment>,<array_values><comment_nl_or_nl>"
+        "<comment_nl_or_nl><value><nl_or_comment>,<array_values><comment_nl_or_nl>",
+        "<comment_nl_or_nl><value><nl_or_comment><opt_comma>"
     ],
     "<opt_comma>": [",", ""],
-    "<comment_nl_or_nl>": ["<COMMENT><NL><comment_nl_or_nl>", "<NL><comment_nl_or_nl>", "<COMMENT><NL>", "<NL>", ""],
-    "<nl_or_comment>": ["<NL><COMMENT><nl_or_comment>", "<NL><nl_or_comment>", "<NL><COMMENT>", "<NL>", ""],
-    "<table>": ["<standard_table>", "<array_table>"],
+    "<comment_nl_or_nl>": [
+        "<COMMENT><NL><comment_nl_or_nl>",
+        "<COMMENT><NL>",
+        "<NL><comment_nl_or_nl>",
+        "<NL>",
+        ""],
+    "<nl_or_comment>": [
+        "<NL><COMMENT><nl_or_comment>",
+        "<NL><nl_or_comment>",
+        "<NL><COMMENT>",
+        "<NL>",
+        ""],
+    "<table>": [
+        "<array_table>",
+        "<standard_table>",
+    ],
     "<standard_table>": ["[<key>]"],
     "<inline_table>": ["{<inline_table_keyvals>}"],
     "<inline_table_keyvals>": ["<inline_table_keyvals_non_empty>", ""],
     "<inline_table_keyvals_non_empty>": [
         "<key> = <value>, <inline_table_keyvals_non_empty>",
         "<key> = <value>"
     ],
@@ -118,42 +131,48 @@
     ],
     "<HEX_INT>": ["0x<HEX_DIGIT><HEX_DIGIT_OR_UNDERSCORES>"],
     "<HEX_DIGIT_OR_UNDERSCORES>": [
         "<HEX_DIGIT_OR_UNDERSCORE><HEX_DIGIT_OR_UNDERSCORES>",
         "<HEX_DIGIT_OR_UNDERSCORE>",
         ""
     ],
-    "<HEX_DIGIT_OR_UNDERSCORE>": ["<HEX_DIGIT>", "_<HEX_DIGIT>"],
+    "<HEX_DIGIT_OR_UNDERSCORE>": ["_<HEX_DIGIT>", "<HEX_DIGIT>"],
     "<OCT_INT>": ["0o<DIGIT_0_7><DIGIT_0_7_OR_UNDERSCORES>"],
     "<DIGIT_0_7_OR_UNDERSCORES>": [
         "<DIGIT_0_7_OR_UNDERSCORE><DIGIT_0_7_OR_UNDERSCORES>",
         "<DIGIT_0_7_OR_UNDERSCORE>",
         ""
     ],
     "<DIGIT_0_7_OR_UNDERSCORE>": ["<DIGIT_0_7>", "_<DIGIT_0_7>"],
     "<BIN_INT>": ["0b<DIGIT_0_1><DIGIT_0_1_OR_UNDERSCORES>"],
     "<DIGIT_0_1_OR_UNDERSCORES>": [
         "<DIGIT_0_1_OR_UNDERSCORE><DIGIT_0_1_OR_UNDERSCORES>",
         "<DIGIT_0_1_OR_UNDERSCORE>",
         ""
     ],
-    "<DIGIT_0_1_OR_UNDERSCORE>": ["<DIGIT_0_1>", "_<DIGIT_0_1>"],
+    "<DIGIT_0_1_OR_UNDERSCORE>": [
+        "_<DIGIT_0_1>",
+        "<DIGIT_0_1>",
+    ],
     # dates
     "<YEAR>": ["<DIGIT><DIGIT><DIGIT><DIGIT>"],
     "<MONTH>": ["<DIGIT><DIGIT>"],
     "<DAY>": ["<DIGIT><DIGIT>"],
     "<DELIM>": ["T", "t", " "],
     "<HOUR>": ["<DIGIT><DIGIT>"],
     "<MINUTE>": ["<DIGIT><DIGIT>"],
     "<SECOND>": ["<DIGIT><DIGIT>"],
     "<SECFRAC>": [".<DIGITS>"],
     "<DIGITS>": ["<DIGIT>", "<DIGIT><DIGITS>"],
     "<NUMOFFSET>": ["<plusminus><HOUR>:<MINUTE>"],
     "<OFFSET>": ["Z", "<NUMOFFSET>"],
-    "<PARTIAL_TIME>": ["<HOUR>:<MINUTE>:<SECOND>", "<HOUR>:<MINUTE>:<SECOND><SECFRAC>"],
+    "<PARTIAL_TIME>": [
+        "<HOUR>:<MINUTE>:<SECOND><SECFRAC>",
+        "<HOUR>:<MINUTE>:<SECOND>",
+    ],
     "<FULL_DATE>": ["<YEAR>-<MONTH>-<DAY>"],
     "<FULL_TIME>": ["<PARTIAL_TIME><OFFSET>"],
     "<OFFSET_DATE_TIME>": ["<FULL_DATE><DELIM><FULL_TIME>"],
     "<LOCAL_DATE_TIME>": ["<FULL_DATE><DELIM><PARTIAL_TIME>"],
     "<LOCAL_DATE>": ["<FULL_DATE>"],
     "<LOCAL_TIME>": ["<PARTIAL_TIME>"],
     # keys
```

