# Comparing `tmp/spacy-ngram-0.0.2.tar.gz` & `tmp/spacy_ngram-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy-ngram-0.0.2.tar", last modified: Tue Mar 21 20:23:38 2023, max compression
+gzip compressed data, was "spacy_ngram-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `spacy-ngram-0.0.2.tar` & `spacy_ngram-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1025 2023-03-21 20:23:34.117422 spacy-ngram-0.0.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0     4714 2023-03-21 20:23:34.117422 spacy-ngram-0.0.2/.gitignore
--rw-r--r--   0        0        0      697 2023-03-21 20:23:34.117422 spacy-ngram-0.0.2/CHANGELOG.md
--rw-r--r--   0        0        0     1126 2023-03-21 20:23:34.117422 spacy-ngram-0.0.2/LICENSE
--rw-r--r--   0        0        0     5606 2023-03-21 20:23:34.117422 spacy-ngram-0.0.2/README.md
--rw-r--r--   0        0        0      827 2023-03-21 20:23:34.117422 spacy-ngram-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        5 2023-03-21 20:23:34.117422 spacy-ngram-0.0.2/requirements.txt
--rw-r--r--   0        0        0       44 2023-03-21 20:23:34.117422 spacy-ngram-0.0.2/src/spacy_ngram/__init__.py
--rw-r--r--   0        0        0     3845 2023-03-21 20:23:34.117422 spacy-ngram-0.0.2/src/spacy_ngram/ngram_component.py
--rw-r--r--   0        0        0      741 2023-03-21 20:23:34.117422 spacy-ngram-0.0.2/test/conftest.py
--rw-r--r--   0        0        0      352 2023-03-21 20:23:34.117422 spacy-ngram-0.0.2/test/test_edges.py
--rw-r--r--   0        0        0     1141 2023-03-21 20:23:34.117422 spacy-ngram-0.0.2/test/test_ngrams.py
--rw-r--r--   0        0        0     6267 1970-01-01 00:00:00.000000 spacy-ngram-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1025 2023-07-25 19:44:06.066014 spacy_ngram-0.0.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0     4714 2023-07-25 19:44:06.066014 spacy_ngram-0.0.3/.gitignore
+-rw-r--r--   0        0        0      807 2023-07-25 19:44:06.066014 spacy_ngram-0.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1126 2023-07-25 19:44:06.066014 spacy_ngram-0.0.3/LICENSE
+-rw-r--r--   0        0        0     5606 2023-07-25 19:44:06.066014 spacy_ngram-0.0.3/README.md
+-rw-r--r--   0        0        0      827 2023-07-25 19:44:06.066014 spacy_ngram-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        5 2023-07-25 19:44:06.066014 spacy_ngram-0.0.3/requirements.txt
+-rw-r--r--   0        0        0       44 2023-07-25 19:44:06.066014 spacy_ngram-0.0.3/src/spacy_ngram/__init__.py
+-rw-r--r--   0        0        0     3863 2023-07-25 19:44:06.066014 spacy_ngram-0.0.3/src/spacy_ngram/ngram_component.py
+-rw-r--r--   0        0        0      741 2023-07-25 19:44:06.070014 spacy_ngram-0.0.3/test/conftest.py
+-rw-r--r--   0        0        0      352 2023-07-25 19:44:06.070014 spacy_ngram-0.0.3/test/test_edges.py
+-rw-r--r--   0        0        0     1241 2023-07-25 19:44:06.070014 spacy_ngram-0.0.3/test/test_ngrams.py
+-rw-r--r--   0        0        0     6267 1970-01-01 00:00:00.000000 spacy_ngram-0.0.3/PKG-INFO
```

### Comparing `spacy-ngram-0.0.2/.github/workflows/publish-to-pypi.yml` & `spacy_ngram-0.0.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `spacy-ngram-0.0.2/.gitignore` & `spacy_ngram-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `spacy-ngram-0.0.2/CHANGELOG.md` & `spacy_ngram-0.0.3/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -13,19 +13,27 @@
 * `Deprecated`: for soon-to-be removed features.
 * `Removed`: for now removed features.
 * `Fixed`: for any bug fixes.
 * `Security`: in case of vulnerabilities.
 
 ## [Unreleased]
 
+## 0.0.3 - 2023-07-25
+
+### Fixed
+
+* Multiple spaces between words caused spaces to appear in ngram output.
+
+
 ## 0.0.2
 
 ### Changed
 
 * `pyproject.toml` and `.gitignore` to make flit happy
 
+
 ## 0.0.1
 
 ### Added
 
 * Ngram component
 * Supporting documentation, etc.
```

### Comparing `spacy-ngram-0.0.2/LICENSE` & `spacy_ngram-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy-ngram-0.0.2/README.md` & `spacy_ngram-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `spacy-ngram-0.0.2/pyproject.toml` & `spacy_ngram-0.0.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['flit_core >=3.2']
 build-backend = 'flit_core.buildapi'
 
 [project]
 name = 'spacy-ngram'
-version = '0.0.2'
+version = '0.0.3'
 authors = [
     { name = 'dcronkite', email = 'dcronkite+pypi@gmail.com' }
 ]
 license = { file = 'LICENSE'}
 description = 'SpaCy pipeline component for adding document or sentence-level ngrams.'
 dependencies = ['spacy']
 requires-python = '>=3.10'
```

### Comparing `spacy-ngram-0.0.2/src/spacy_ngram/ngram_component.py` & `spacy_ngram-0.0.3/src/spacy_ngram/ngram_component.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
                 yield count, '_'.join(sequence[i] for i in range(-count, 0))
 
     def itertokens(self, sequence: Doc | Span):
         """Return next relevant lemma from the sequence"""
         if self.include_bos:
             yield '<BOS>'
         for token in sequence:
-            if token.is_stop or token.is_punct or token.is_digit:
+            if token.is_stop or token.is_punct or token.is_digit or token.is_space:
                 continue
             lemma = token.lemma_.lower()
             if lemma in self.nlp.Defaults.stop_words:
                 continue
             yield lemma
         if self.include_eos:
             yield '<EOS>'
```

### Comparing `spacy-ngram-0.0.2/test/conftest.py` & `spacy_ngram-0.0.3/test/conftest.py`

 * *Files identical despite different names*

### Comparing `spacy-ngram-0.0.2/test/test_ngrams.py` & `spacy_ngram-0.0.3/test/test_ngrams.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,27 +4,28 @@
 from spacy_ngram import NgramComponent
 
 
 @pytest.mark.parametrize('text, exp', [
     ('Quark soup is an interacting localized assembly of quarks and gluons.',
      ['quark', 'soup', 'interact', 'localize', 'assembly', 'quark', 'gluon']
      ),
+    ('Try two  spaces.', ['try', 'space']),
 ])
 def test_unigrams(nlp, text, exp):
     doc = nlp(text)
     assert doc._.ngram_1 == exp
 
 
 @pytest.mark.parametrize('text, exp', [
     ('Quark soup is an interacting localized assembly of quarks and gluons.',
      ['quark_soup', 'soup_interact', 'interact_localize', 'localize_assembly', 'assembly_quark', 'quark_gluon']
      ),
-    ('Short ngram.',
-     ['short_ngram']
-     ),
+    ('Short ngram.', ['short_ngram']),
+    ('Oneword.', []),
+    ('A little   spacy.', ['little_spacy']),
 ])
 def test_bigrams(nlp, text, exp):
     doc = nlp(text)
     assert doc._.ngram_2 == exp
 
 
 @pytest.mark.parametrize('text, exp', [
```

### Comparing `spacy-ngram-0.0.2/PKG-INFO` & `spacy_ngram-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-ngram
-Version: 0.0.2
+Version: 0.0.3
 Summary: SpaCy pipeline component for adding document or sentence-level ngrams.
 Keywords: nlp,ngrams
 Author-email: dcronkite <dcronkite+pypi@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spacy-ngram Version: 0.0.2 Summary: SpaCy pipeline
+Metadata-Version: 2.1 Name: spacy-ngram Version: 0.0.3 Summary: SpaCy pipeline
 component for adding document or sentence-level ngrams. Keywords: nlp,ngrams
 Author-email: dcronkite
 pypi@gmail.com> Requires-Python: >=3.10 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Science/Research Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Text Processing :: Linguistic Classifier: License :: OSI
 Approved :: MIT License Requires-Dist: spacy Requires-Dist: pytest ; extra ==
```

