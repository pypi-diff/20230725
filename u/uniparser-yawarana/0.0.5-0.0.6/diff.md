# Comparing `tmp/uniparser_yawarana-0.0.5.tar.gz` & `tmp/uniparser_yawarana-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/uniparser_yawarana-0.0.5.tar", last modified: Fri Apr 28 20:33:23 2023, max compression
+gzip compressed data, was "dist/uniparser_yawarana-0.0.6.tar", last modified: Tue Jul 25 15:17:50 2023, max compression
```

## Comparing `uniparser_yawarana-0.0.5.tar` & `uniparser_yawarana-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-04-28 20:33:23.000000 uniparser_yawarana-0.0.5/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      401 2023-04-28 20:33:19.000000 uniparser_yawarana-0.0.5/CITATION.cff
--rw-rw-r--   0 florianm  (1000) florianm  (1000)    11359 2022-04-02 19:58:24.000000 uniparser_yawarana-0.0.5/LICENSE
--rw-r--r--   0 florianm  (1000) florianm  (1000)       92 2022-04-05 09:00:02.000000 uniparser_yawarana-0.0.5/MANIFEST.in
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     2198 2023-04-28 20:33:23.000000 uniparser_yawarana-0.0.5/PKG-INFO
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1212 2023-03-05 16:32:16.000000 uniparser_yawarana-0.0.5/README.md
--rw-r--r--   0 florianm  (1000) florianm  (1000)      366 2022-04-04 17:40:04.000000 uniparser_yawarana-0.0.5/pyproject.toml
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     1793 2023-04-28 20:33:23.000000 uniparser_yawarana-0.0.5/setup.cfg
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       92 2022-04-04 08:29:49.000000 uniparser_yawarana-0.0.5/setup.py
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-04-28 20:33:23.000000 uniparser_yawarana-0.0.5/src/
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-04-28 20:33:23.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     3656 2023-04-28 20:31:36.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana/__init__.py
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-04-28 20:33:23.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana/data/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      387 2023-04-27 20:25:38.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana/data/bad_analyses.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      282 2023-04-27 20:25:38.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana/data/clitics.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     3449 2023-04-27 20:25:38.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana/data/derivations.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     2042 2023-04-27 20:25:38.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana/data/disambiguation.cg3
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     8118 2023-04-27 20:25:38.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana/data/etym_lookup.yaml
--rw-rw-r--   0 florianm  (1000) florianm  (1000)        0 2023-04-27 20:25:38.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana/data/lex_rules.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)    89222 2023-04-27 20:25:38.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana/data/lexemes.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)    13143 2023-04-27 20:25:38.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana/data/paradigms.txt
-drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-04-28 20:33:23.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana.egg-info/
--rw-rw-r--   0 florianm  (1000) florianm  (1000)     2198 2023-04-28 20:33:23.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana.egg-info/PKG-INFO
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      730 2023-04-28 20:33:23.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana.egg-info/SOURCES.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2023-04-28 20:33:23.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana.egg-info/dependency_links.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2023-04-28 20:33:23.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana.egg-info/not-zip-safe
--rw-rw-r--   0 florianm  (1000) florianm  (1000)      243 2023-04-28 20:33:23.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana.egg-info/requires.txt
--rw-rw-r--   0 florianm  (1000) florianm  (1000)       19 2023-04-28 20:33:23.000000 uniparser_yawarana-0.0.5/src/uniparser_yawarana.egg-info/top_level.txt
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-07-25 15:17:50.000000 uniparser_yawarana-0.0.6/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      401 2023-07-25 15:16:55.000000 uniparser_yawarana-0.0.6/CITATION.cff
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)    11359 2022-04-02 19:58:24.000000 uniparser_yawarana-0.0.6/LICENSE
+-rw-r--r--   0 florianm  (1000) florianm  (1000)       92 2022-04-05 09:00:02.000000 uniparser_yawarana-0.0.6/MANIFEST.in
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     2162 2023-07-25 15:17:50.000000 uniparser_yawarana-0.0.6/PKG-INFO
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1212 2023-03-05 16:32:16.000000 uniparser_yawarana-0.0.6/README.md
+-rw-r--r--   0 florianm  (1000) florianm  (1000)      366 2022-04-04 17:40:04.000000 uniparser_yawarana-0.0.6/pyproject.toml
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     1793 2023-07-25 15:17:50.000000 uniparser_yawarana-0.0.6/setup.cfg
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       92 2022-04-04 08:29:49.000000 uniparser_yawarana-0.0.6/setup.py
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-07-25 15:17:50.000000 uniparser_yawarana-0.0.6/src/
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-07-25 15:17:50.000000 uniparser_yawarana-0.0.6/src/uniparser_yawarana/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     4148 2023-07-25 15:15:27.000000 uniparser_yawarana-0.0.6/src/uniparser_yawarana/__init__.py
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-07-25 15:17:50.000000 uniparser_yawarana-0.0.6/src/uniparser_yawarana/data/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      451 2023-07-25 11:32:44.000000 uniparser_yawarana-0.0.6/src/uniparser_yawarana/data/bad_analyses.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      471 2023-07-25 11:32:44.000000 uniparser_yawarana-0.0.6/src/uniparser_yawarana/data/clitics.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     3589 2023-07-25 11:32:44.000000 uniparser_yawarana-0.0.6/src/uniparser_yawarana/data/derivations.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     2177 2023-07-25 11:32:44.000000 uniparser_yawarana-0.0.6/src/uniparser_yawarana/data/disambiguation.cg3
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     8117 2023-07-25 11:32:43.000000 uniparser_yawarana-0.0.6/src/uniparser_yawarana/data/etym_lookup.yaml
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)        0 2023-07-25 11:32:44.000000 uniparser_yawarana-0.0.6/src/uniparser_yawarana/data/lex_rules.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)    95825 2023-07-25 11:32:44.000000 uniparser_yawarana-0.0.6/src/uniparser_yawarana/data/lexemes.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)    15050 2023-07-25 11:32:44.000000 uniparser_yawarana-0.0.6/src/uniparser_yawarana/data/paradigms.txt
+drwxrwxr-x   0 florianm  (1000) florianm  (1000)        0 2023-07-25 15:17:50.000000 uniparser_yawarana-0.0.6/src/uniparser_yawarana.egg-info/
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)     2162 2023-07-25 15:17:49.000000 uniparser_yawarana-0.0.6/src/uniparser_yawarana.egg-info/PKG-INFO
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      730 2023-07-25 15:17:50.000000 uniparser_yawarana-0.0.6/src/uniparser_yawarana.egg-info/SOURCES.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2023-07-25 15:17:49.000000 uniparser_yawarana-0.0.6/src/uniparser_yawarana.egg-info/dependency_links.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)        1 2023-07-25 15:17:49.000000 uniparser_yawarana-0.0.6/src/uniparser_yawarana.egg-info/not-zip-safe
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)      243 2023-07-25 15:17:50.000000 uniparser_yawarana-0.0.6/src/uniparser_yawarana.egg-info/requires.txt
+-rw-rw-r--   0 florianm  (1000) florianm  (1000)       19 2023-07-25 15:17:50.000000 uniparser_yawarana-0.0.6/src/uniparser_yawarana.egg-info/top_level.txt
```

### Comparing `uniparser_yawarana-0.0.5/LICENSE` & `uniparser_yawarana-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `uniparser_yawarana-0.0.5/PKG-INFO` & `uniparser_yawarana-0.0.6/src/uniparser_yawarana.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
-Name: uniparser_yawarana
-Version: 0.0.5
+Name: uniparser-yawarana
+Version: 0.0.6
 Summary: A UniParser implementation for morphologically parsing and annotating Yawarana material.
 Home-page: https://github.com/fmatter/uniparser-yawarana
 Author: Florian Matter
 Author-email: florianmatter@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/fmatter/uniparser-yawarana/issues
 Keywords: linguistics,morphology
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -33,8 +31,7 @@
 [![Linting](https://img.shields.io/github/actions/workflow/status/fmatter/uniparser-yawarana/lint.yml?label=linting&branch=main)](https://github.com/fmatter/uniparser-yawarana/actions/workflows/lint.yml)
 [![Codecov](https://img.shields.io/codecov/c/github/fmatter/uniparser-yawarana)](https://app.codecov.io/gh/fmatter/uniparser-yawarana/)
 [![PyPI](https://img.shields.io/pypi/v/uniparser-yawarana.svg)](https://pypi.org/project/uniparser-yawarana)
 ![Versions](https://img.shields.io/pypi/pyversions/uniparser-yawarana)
 
 This project uses the excellent [uniparser-morph](https://github.com/timarkh/uniparser-morph/) package.
 It is currently under development.
-
```

### Comparing `uniparser_yawarana-0.0.5/README.md` & `uniparser_yawarana-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `uniparser_yawarana-0.0.5/setup.cfg` & `uniparser_yawarana-0.0.6/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 	morphology
 long_description = file: README.md
 long_description_content_type = text/markdown
 name = uniparser_yawarana
 project_urls = 
 	Bug Tracker = https://github.com/fmatter/uniparser-yawarana/issues
 url = https://github.com/fmatter/uniparser-yawarana
-version = 0.0.5
+version = 0.0.6
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 package_dir = 
 	=src
```

### Comparing `uniparser_yawarana-0.0.5/src/uniparser_yawarana/__init__.py` & `uniparser_yawarana-0.0.6/src/uniparser_yawarana/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 except ImportError:  # pragma: no cover
     from importlib_resources import files  # pragma: no cover
 
 log = logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 __author__ = "Florian Matter"
 __email__ = "fmatter@mailbox.org"
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 
 
 class YawaranaAnalyzer(Analyzer):
-    def __init__(self, etymologize=False, verbose_grammar=False):
+    def __init__(self, etymologize=False, verbose_grammar=False, cache=True):
         super().__init__(verbose_grammar=verbose_grammar)
         self.base_path = files("uniparser_yawarana") / "data"
         self.flattenSubwords = True
         self.paradigmFile = self.base_path / "paradigms.txt"
         self.lexRulesFile = self.base_path / "lex_rules.txt"
         self.lexFile = self.base_path / "lexemes.txt"
         self.delAnaFile = self.base_path / "bad_analyses.txt"
@@ -32,38 +32,40 @@
             "r",
             encoding="utf-8",
         ) as f:
             self.etym_dict = yaml.load(f, Loader=yaml.SafeLoader)
         self.wfCache = {}
         self.etymologize_mode = etymologize
         self.load_grammar()
+        self.initialize_parser()
+        self.m.REMEMBER_PARSES = cache
 
-    def etymologize(self, ana):
-        etym_ids = []
-        etym_obj = ana.wfGlossed
-        etym_gloss = ana.gloss
-        for k, v in ana.otherData:
-            if k != "id":
-                continue
-            ids = v.split(",")
-            for _id in ids:
-                if _id in self.etym_dict:
-                    etym_info = self.etym_dict[_id]
-                    etym_ids.extend(etym_info["ids"])
-                    for orig, repl in etym_info["obj"].items():
-                        etym_obj = etym_obj.replace(orig, repl)
-                    for orig, repl in etym_info["gloss"].items():
-                        etym_gloss = etym_gloss.replace(orig, repl)
-                else:
-                    etym_ids.append(_id)
-        self.wfCache[str(ana)] = [
-            ("id_etym", ",".join(etym_ids)),
-            ("wfGlossed_etym", etym_obj),
-            ("gloss_etym", etym_gloss),
-        ]
+    # def etymologize(self, ana):
+    #     etym_ids = []
+    #     etym_obj = ana.wfGlossed
+    #     etym_gloss = ana.gloss
+    #     for k, v in ana.otherData:
+    #         if k != "id":
+    #             continue
+    #         ids = v.split(",")
+    #         for _id in ids:
+    #             if _id in self.etym_dict:
+    #                 etym_info = self.etym_dict[_id]
+    #                 etym_ids.extend(etym_info["ids"])
+    #                 for orig, repl in etym_info["obj"].items():
+    #                     etym_obj = etym_obj.replace(orig, repl)
+    #                 for orig, repl in etym_info["gloss"].items():
+    #                     etym_gloss = etym_gloss.replace(orig, repl)
+    #             else:
+    #                 etym_ids.append(_id)
+    #     self.wfCache[str(ana)] = [
+    #         ("id_etym", ",".join(etym_ids)),
+    #         ("wfGlossed_etym", etym_obj),
+    #         ("gloss_etym", etym_gloss),
+    #     ]
 
     def analyze_words(  # pylint: disable=redefined-builtin,too-many-arguments
         self,
         words,
         cgFile="",
         format=None,
         disambiguate=True,
@@ -71,20 +73,30 @@
     ):
         all_analyses = super().analyze_words(
             words,
             cgFile=str(self.base_path / "disambiguation.cg3"),
             format=format,
             disambiguate=disambiguate,
         )
+        filtered = []
         for ana in all_analyses:
-            if self.etymologize_mode:
-                if str(ana) not in self.wfCache:
-                    self.etymologize(ana)
-                ana.otherData.extend(self.wfCache[str(ana)])
-        return all_analyses
+            if isinstance(ana, list):
+                dedup = list(dict.fromkeys(ana))
+                filtered.append(dedup)
+                # if len(dedup) == 1:
+                #     filtered.append(dedup[0])
+                # else:
+                #     filtered.append(dedup)
+            else:
+                filtered.append(ana)
+            # if self.etymologize_mode:
+            #     if str(ana) not in self.wfCache:
+            #         self.etymologize(ana)
+            #     ana.otherData.extend(self.wfCache[str(ana)])
+        return filtered
 
         # if isinstance(all_analyses[0], list):  # filter wrong analyses of -jrama 'PROH'
         #     filtered = []
         #     for analyses in all_analyses:
         #         filtered_analysis = [
         #             x for x in analyses if not ("jrama" in x.wf and "neg" in x.gramm)
         #         ]
```

### Comparing `uniparser_yawarana-0.0.5/src/uniparser_yawarana/data/derivations.txt` & `uniparser_yawarana-0.0.6/src/uniparser_yawarana/data/derivations.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,90 +2,92 @@
 
 -deriv-type: V-ri
  lex: [.]&rinmlz
  stem: [.]ri<.>//[.]0<.>
  paradigm: noun_clitic
  paradigm: n_deriv
  gloss: ACNNMLZ
- gramm: n, acnnmlz
+ gramm: n,nmlz
  id: rinmlz
 
 -deriv-type: V-kemi
- lex: [.]rinmlz&keprop&minmlz
+ lex: [.]&rinmlz&keprop&minmlz
  stem: [.]0&ke&mï<.>//[.]0&ke&m<.>
- gramm: adv,prop
+ gramm: adv,prop,nmlz
  gloss: ACNNMLZ&PROP&NMLZ
  id: rinmlz,keprop,minmlz
  paradigm: mi_clitic
  paradigm: noun_clitic
 
 -deriv-type: V-jpë
  lex: [.]&jpenmlz
  stem: [.]jpë
- gramm: n
+ gramm: n,nmlz
  gloss: PST.ACNNMLZ
  id: jpenmlz
 
 -deriv-type: V-sape
  lex: [.]&sapenmlz
  stem: [.]sapë//[.]saj//[.]chaj
- gramm: n
+ gramm: n,nmlz
  gloss: ABS.NMLZ
  id: sapenmlz
 
 -deriv-type: V-inf
  lex: [.]&neinf
  stem: [.]në//[.]të
- gramm: n
+ gramm: n,nmlz
  gloss: INF
  id: neinf
 
 -deriv-type: V-topo
  lex: [.]&toponmlz
  stem: [.]topo<.>//[.]toj<.>
- gramm: n
+ gramm: n,nmlz
  gloss: CIRC.NMLZ
  id: toponmlz
  paradigm: n_priv
  paradigm: noun_past
 
 -deriv-type: V-ni
  lex: [.]&ninmlz
  stem: [.]ni<.>
- gramm: n
+ gramm: n,nmlz
  gloss: AGTNMLZ
  id: ninmlz
+ paradigm: uninfl
 
 -deriv-type: A-ano
  lex: [.]&anonmlz
  stem: [.]no<.>//[.]n<.>//[.]an<.>//[.]ano<.>//[.]na<.>
- gramm: n
+ gramm: n,nmlz
  gloss: NMLZ
  id: anonmlz
 
 -deriv-type: A-mi
  lex: [.]&minmlz
  stem: [.]mï<.>//[.]m<.>
- gramm: n
+ gramm: n,nmlz
  gloss: NMLZ
  id: minmlz
  paradigm: mi_clitic
  paradigm: noun_clitic
 
--deriv-type: A-mijra
- lex: [.]&minmlz&jrapriv
- stem: [.]mï&jra
- gramm: n,priv
- gloss: NMLZ&PRIV
- id: minmlz,jrapriv
+# jra is a particle
+# -deriv-type: A-mijra
+#  lex: [.]&minmlz&jrapriv
+#  stem: [.]mï&jra
+#  gramm: n,priv,nmlz
+#  gloss: NMLZ&PRIV
+#  id: minmlz,jrapriv
 
 -deriv-type: V-semi
  lex: [.]septcp|minmlz
  stem: <.>[.]se|mï<.>//<.>[.]che|mï<.>
- gramm: n
+ gramm: n,nmlz
  gloss: PTCP|NMLZ
  id: septcp,minmlz
 
 # adverbs
 
 -deriv-type: V-septcp
  lex: [.]&septcp
@@ -93,51 +95,52 @@
  paradigm: adv_deriv
  gramm: adv,ptcp
  gloss: PTCP
  id: septcp
 
 -deriv-type: V-sesup
  lex: [.]&septcp
- stem: [.]se<.>//[.]che<.>
- paradigm: uninfl
+ stem: <.>[.]se//<.>[.]che
+ paradigm: adv_deriv
  gramm: adv,sup
  gloss: SUP
  id: septcp
 
 -deriv-type: V-tojpe
  lex: [.]&tojpepurp
- stem: [.]tojpe<.>
- paradigm: adv
- gramm: adv,purp
+ stem: <.>[.]tojpe
+ paradigm: advl
+ gramm: advl,purp
  gloss: PURP
  id: tojpepurp
 
 -deriv-type: V-tane
  lex: [.]&tanecncs
- stem: [.]tane<.>
- paradigm: adv
- gramm: adv,cncs
+ stem: <.>[.]tane
+ paradigm: advl
+ gramm: advl,cncs
  gloss: CNCS
  id: tanecncs
 
 -deriv-type: N-ke
  lex: [.]&keprop
  stem: [.]ke<.>
  paradigm: adv_deriv
  paradigm: adv
  gramm: adv,prop
  gloss: PROP
  id: keprop
 
--deriv-type: N-jra
- lex: [.]&jrapriv
- stem: [.]jra
- gramm: priv
- gloss: PRIV
- id: jrapriv
+# jra is a particle
+# -deriv-type: N-jra
+#  lex: [.]&jrapriv
+#  stem: [.]jra
+#  gramm: priv
+#  gloss: PRIV
+#  id: jrapriv
 
 # productive aspectual derivations
 
 -deriv-type: Vi-podes
  lex: [.]&podes
  stem: .[.]po.
  paradigm: v_intr
@@ -210,10 +213,10 @@
  id: petiplur
 
 # productive nominal derivations
 
 -deriv-type: N-dim
  lex: [.]&pijkedim
  stem: [.]pïjkë<.>//[.]pijkë<.>
- gramm: n
+ gramm: n,dim
  gloss: DIM
  id: pijkedim
```

### Comparing `uniparser_yawarana-0.0.5/src/uniparser_yawarana/data/disambiguation.cg3` & `uniparser_yawarana-0.0.6/src/uniparser_yawarana/data/disambiguation.cg3`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 SECTION # verbs and deverbal forms
 
 # only nouns before postpositions
 SELECT nominal IF (1 postpositional) (0 verbal);
 
 # only verbs before auxiliaries
-SELECT verbal IF (*1 ("chi-cop") BARRIER notParticles);
+REMOVE (nmlz) IF (*1 ("chi-cop") BARRIER notParticles);
 
 # only auxiliaries after verbs
 SELECT ("chi-cop") IF (*-1 verbal BARRIER notParticles);
 
 # only verbs before relativizer (and aspectual? mare)
 REMOVE (n) IF (1 ("mare-rel-inan"));
 
@@ -62,14 +62,18 @@
 
 # yaka: only 'dig out' when inflected
 SELECT ("yaka-all") IF (0 ("<yaka>"));
 
 # nwa: never 'glute' if not preceded by nominal (?)
 SELECT ("nwa-thus") IF (NOT -1 nominal);
 
+# pe: never 'palm.sp' if preceded by nominalized verb
+SELECT ("pe-ess") IF (-1 (nmlz));
+
 # chiri ma 'only that', 'that' being a nominalized copula
 SELECT (acnnmlz) IF (1 ("<ma>")) (0 ("<chiri>"));
 
 SECTION # bad wordforms with clitics
 REMOVE (rst) IF (0 ("<yakarama>"));
 SELECT ("nwa-thus+re-emp") IF (0 ("<nwarë>"));
-SELECT ("ire-3ana-inan") IF (0 ("<irë>"));
+SELECT ("ire-3ana-inan") IF (0 ("<irë>"));
+SELECT ("akere-with") IF (0 ("<takërë>"));
```

### Comparing `uniparser_yawarana-0.0.5/src/uniparser_yawarana/data/etym_lookup.yaml` & `uniparser_yawarana-0.0.6/src/uniparser_yawarana/data/etym_lookup.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -329,15 +329,15 @@
 werewereta-swarm-mosquitos:
   gloss:
     swarm(mosquitos): ''
   ids:
   - werewere-mosquito-sp
   - tavbz
   obj:
-    werewereta: werewereta
+    werewereta: werewere-ta
 keyata-grow:
   gloss:
     grow: ''
   ids:
   - ''
   - tavbz
   obj:
@@ -425,15 +425,15 @@
 yerema-feed:
   gloss:
     feed: ''
   ids:
   - ''
   - macaus
   obj:
-    yerema: yere-ma
+    erema: ere-ma
 yakarama-tell:
   gloss:
     tell: ''
   ids:
   - yakara-believe
   - macaus
   obj:
@@ -575,15 +575,15 @@
   obj:
     "mak\xEBp\xEFjk\xEB": "mak\xEBp\xEFjk\xEB"
 6:
   gloss:
     thin: ''
   ids:
   - ''
-  - readvz
+  - yeadvz
   obj:
     "m\xEBt\xEBye": "m\xEBt\xEBye"
 7:
   gloss:
     go(PLUR): ''
   ids:
   - te-go
```

### Comparing `uniparser_yawarana-0.0.5/src/uniparser_yawarana/data/lexemes.txt` & `uniparser_yawarana-0.0.6/src/uniparser_yawarana/data/lexemes.txt`

 * *Files 0% similar despite different names*

```diff
@@ -236,14 +236,24 @@
  gramm: n
  std: asuka
  id: asuka-sugar
  paradigm: noun_v_new_ri_0
  paradigm: n_deriv
 
 -lexeme
+ lex: ati-what
+ stem: .ati.
+ trans_en: what
+ gloss: what
+ gramm: intj
+ std: ati
+ id: ati-what
+ paradigm: uninfl
+
+-lexeme
  lex: ati-plot-of-cultivated-land
  stem: .ati.|.atï.
  trans_en: plot of cultivated land
  gloss: plot_of_cultivated_land
  gramm: n
  std: ati
  id: ati-plot-of-cultivated-land
@@ -336,14 +346,25 @@
  gramm: n
  std: chiramu
  id: chiramu-mange
  paradigm: noun_c_new_ru_0
  paradigm: n_deriv
 
 -lexeme
+ lex: chirike-star
+ stem: .chirikë.
+ trans_en: star
+ gloss: star
+ gramm: n
+ std: chirikë
+ id: chirike-star
+ paradigm: noun_c_new_ri_0
+ paradigm: n_deriv
+
+-lexeme
  lex: chiri-titi-monkey
  stem: .chiri.
  trans_en: titi monkey
  gloss: titi_monkey
  gramm: n
  std: chiri
  id: chiri-titi-monkey
@@ -488,14 +509,25 @@
  gramm: adv
  std: ewinë
  id: ewine-here-all
  paradigm: adv
  paradigm: adv_deriv
 
 -lexeme
+ lex: ijmoy-egg
+ stem: .ijmoy.
+ trans_en: egg
+ gloss: egg
+ gramm: n
+ std: ijmoy
+ id: ijmoy-egg
+ paradigm: noun_v_new_ri_0
+ paradigm: n_deriv
+
+-lexeme
  lex: ijpu-summit
  stem: .ijpu.
  trans_en: summit
  gloss: summit
  gramm: n
  std: ijpu
  id: ijpu-summit
@@ -510,15 +542,15 @@
  gramm: postp
  std: inawë
  id: inawe-have
  paradigm: postp
 
 -lexeme
  lex: ini-see
- stem: .ini.|.in.
+ stem: .ini.|.in.|.ene.
  trans_en: see
  gloss: see
  gramm: vt
  std: ini
  id: ini-see
  paradigm: v_tr
  paradigm: v_tr_nmlz
@@ -743,14 +775,25 @@
  gramm: adv
  std: kawë
  id: kawe-high
  paradigm: adv
  paradigm: adv_deriv
 
 -lexeme
+ lex: kayami-louse
+ stem: .kayamï.
+ trans_en: louse
+ gloss: louse
+ gramm: n
+ std: kayamï
+ id: kayami-louse
+ paradigm: noun_c_new_ri_0
+ paradigm: n_deriv
+
+-lexeme
  lex: kaya-barbasco
  stem: .kaya.
  trans_en: barbasco
  gloss: barbasco
  gramm: n
  std: kaya
  id: kaya-barbasco
@@ -788,14 +831,25 @@
  std: kinta
  id: kinta-become-tired
  paradigm: v_intr
  paradigm: v_intr_nmlz
  paradigm: vi_aspect
 
 -lexeme
+ lex: kocha-tail
+ stem: .kocha.
+ trans_en: tail
+ gloss: tail
+ gramm: n
+ std: kocha
+ id: kocha-tail
+ paradigm: noun_c_new_ri_0
+ paradigm: n_deriv
+
+-lexeme
  lex: kojpa-night
  stem: .kojpa.
  trans_en: night
  gloss: night
  gramm: n
  std: kojpa
  id: kojpa-night
@@ -1099,14 +1153,25 @@
  gramm: adv
  std: marë
  id: mare-still
  paradigm: adv
  paradigm: adv_deriv
 
 -lexeme
+ lex: mati-breast
+ stem: .mati.
+ trans_en: breast
+ gloss: breast
+ gramm: n
+ std: mati
+ id: mati-breast
+ paradigm: noun_c_new_ri_0
+ paradigm: n_deriv
+
+-lexeme
  lex: mayawaka-m
  stem: .mayawaka.
  trans_en: M.
  gloss: M.
  gramm: n
  std: mayawaka
  id: mayawaka-m
@@ -1171,14 +1236,25 @@
  gloss: MED.INAN
  gramm: dem
  std: misi
  id: misi-med-inan
  paradigm: uninfl
 
 -lexeme
+ lex: miti-root
+ stem: .miti.
+ trans_en: root; vein
+ gloss: root
+ gramm: n
+ std: miti
+ id: miti-root
+ paradigm: noun_c_new_ri_0
+ paradigm: n_deriv
+
+-lexeme
  lex: mone-vagina
  stem: .mone.
  trans_en: vagina
  gloss: vagina
  gramm: n
  std: mone
  id: mone-vagina
@@ -1203,14 +1279,25 @@
  gloss: 2PL.PRO
  gramm: pn,2
  std: monkontomo
  id: monkontomo-2pl-pro
  paradigm: pro
 
 -lexeme
+ lex: moroko-fish
+ stem: .moroko.
+ trans_en: fish
+ gloss: fish
+ gramm: n
+ std: moroko
+ id: moroko-fish
+ paradigm: noun_c_new_ri_0
+ paradigm: n_deriv
+
+-lexeme
  lex: morone-hurting
  stem: .morone.
  trans_en: hurting
  gloss: hurting
  gramm: adv
  std: morone
  id: morone-hurting
@@ -1408,15 +1495,15 @@
  std: mïra
  id: mira-priodontes-maximus
  paradigm: noun_c_new_ri_0
  paradigm: n_deriv
 
 -lexeme
  lex: nai-do
- stem: .nai.
+ stem: .nai.|.naij.
  trans_en: do
  gloss: do
  gramm: vt
  std: nai
  id: nai-do
  paradigm: v_tr
  paradigm: v_tr_nmlz
@@ -1441,14 +1528,25 @@
  gramm: n
  std: najpï
  id: najpi-grandfather
  paradigm: noun_c_new_ri_0
  paradigm: n_deriv
 
 -lexeme
+ lex: najwata-harbor
+ stem: .najwata.
+ trans_en: harbor
+ gloss: harbor
+ gramm: n
+ std: najwata
+ id: najwata-harbor
+ paradigm: noun_c_new_ri_0
+ paradigm: n_deriv
+
+-lexeme
  lex: naki-thirst
  stem: .naki.
  trans_en: thirst
  gloss: thirst
  gramm: n
  std: naki
  id: naki-thirst
@@ -1519,14 +1617,47 @@
  gramm: n
  std: noti
  id: noti-potential-partner
  paradigm: noun_c_new_ri_0
  paradigm: n_deriv
 
 -lexeme
+ lex: nta-mouth
+ stem: .nta.
+ trans_en: mouth
+ gloss: mouth
+ gramm: n
+ std: nta
+ id: nta-mouth
+ paradigm: noun_c_new_ri_të
+ paradigm: n_deriv
+
+-lexeme
+ lex: nune-moon
+ stem: .nunë.
+ trans_en: moon
+ gloss: moon
+ gramm: n
+ std: nunë
+ id: nune-moon
+ paradigm: noun_c_new_ri_0
+ paradigm: n_deriv
+
+-lexeme
+ lex: nu-tongue
+ stem: .nu.
+ trans_en: tongue
+ gloss: tongue
+ gramm: n
+ std: nu
+ id: nu-tongue
+ paradigm: noun_c_new_ru_0
+ paradigm: n_deriv
+
+-lexeme
  lex: nwajte-dance
  stem: .nwajtë.|.wajtë.
  trans_en: dance
  gloss: dance
  gramm: vi
  std: nwajtë
  id: nwajte-dance
@@ -1650,15 +1781,15 @@
  lex: paku-arrow-tip
  stem: .paku.
  trans_en: arrow tip
  gloss: arrow_tip
  gramm: n
  std: paku
  id: paku-arrow-tip
- paradigm: noun_c_new_ru_0
+ paradigm: noun_c_new_ri_0
  paradigm: n_deriv
 
 -lexeme
  lex: pana-ear
  stem: .pana.
  trans_en: ear
  gloss: ear
@@ -1828,14 +1959,25 @@
  gramm: n
  std: pichipichi
  id: pichipichi-whitebait
  paradigm: noun_c_new_ri_0
  paradigm: n_deriv
 
 -lexeme
+ lex: pijpe-skin
+ stem: .pijpë.
+ trans_en: skin
+ gloss: skin
+ gramm: n
+ std: pijpë
+ id: pijpe-skin
+ paradigm: noun_c_new_ri_0
+ paradigm: n_deriv
+
+-lexeme
  lex: pika-peel
  stem: .pika.
  trans_en: peel
  gloss: peel
  gramm: vt
  std: pika
  id: pika-peel
@@ -1907,14 +2049,36 @@
  gramm: n
  std: poroko
  id: poroko-basket-sp
  paradigm: noun_c_new_ri_0
  paradigm: n_deriv
 
 -lexeme
+ lex: poseti-belly
+ stem: .poseti.
+ trans_en: belly
+ gloss: belly
+ gramm: n
+ std: poseti
+ id: poseti-belly
+ paradigm: noun_c_new_ti_0
+ paradigm: n_deriv
+
+-lexeme
+ lex: pota-mouth
+ stem: .pota.
+ trans_en: mouth; shore
+ gloss: mouth
+ gramm: n
+ std: pota
+ id: pota-mouth
+ paradigm: noun_c_new_ri_0
+ paradigm: n_deriv
+
+-lexeme
  lex: poye-above
  stem: .poye.
  trans_en: above
  gloss: above
  gramm: postp
  std: poye
  id: poye-above
@@ -2041,14 +2205,25 @@
  gramm: n
  std: rui
  id: rui-older-brother
  paradigm: noun_c_old_ri_0
  paradigm: n_deriv
 
 -lexeme
+ lex: sai-penis
+ stem: .sai.
+ trans_en: penis
+ gloss: penis
+ gramm: n
+ std: sai
+ id: sai-penis
+ paradigm: noun_c_new_ri_0
+ paradigm: n_deriv
+
+-lexeme
  lex: sakara-hoplias-malabaricus
  stem: .sakara.
  trans_en: hoplias malabaricus
  gloss: hoplias_malabaricus
  gramm: n
  std: sakara
  id: sakara-hoplias-malabaricus
@@ -2075,15 +2250,15 @@
  std: saku
  id: saku-sweet-potato
  paradigm: noun_c_new_ru_0
  paradigm: n_deriv
 
 -lexeme
  lex: samo-cry
- stem: .samo.|.sëmo.
+ stem: .samo.|.sëmo.|.asamo.
  trans_en: cry
  gloss: cry
  gramm: vi
  std: samo
  id: samo-cry
  paradigm: v_intr
  paradigm: v_intr_nmlz
@@ -2234,15 +2409,15 @@
  std: tajme
  id: tajme-ugly
  paradigm: adv
  paradigm: adv_deriv
 
 -lexeme
  lex: tajnomo-piaroa
- stem: .tajnomo.
+ stem: .tajnomo.|.tajnon.
  trans_en: Piaroa
  gloss: Piaroa
  gramm: n
  std: tajnomo
  id: tajnomo-piaroa
  paradigm: noun_c_new_ri_0
  paradigm: n_deriv
@@ -2403,14 +2578,25 @@
  std: tonko
  id: tonko-play
  paradigm: v_intr
  paradigm: v_intr_nmlz
  paradigm: vi_aspect
 
 -lexeme
+ lex: torono-bird
+ stem: .torono.
+ trans_en: bird
+ gloss: bird
+ gramm: n
+ std: torono
+ id: torono-bird
+ paradigm: noun_c_new_ri_0
+ paradigm: n_deriv
+
+-lexeme
  lex: torote-cemetery
  stem: .torotë.
  trans_en: cemetery
  gloss: cemetery
  gramm: n
  std: torotë
  id: torote-cemetery
@@ -2578,14 +2764,25 @@
  std: waimu
  id: waimu-speak
  paradigm: v_intr
  paradigm: v_intr_nmlz
  paradigm: vi_aspect
 
 -lexeme
+ lex: wajto-fire
+ stem: .wajto.
+ trans_en: fire
+ gloss: fire
+ gramm: n
+ std: wajto
+ id: wajto-fire
+ paradigm: noun_c_new_ri_0
+ paradigm: n_deriv
+
+-lexeme
  lex: wajyaki-happy
  stem: .wajyakï.
  trans_en: happy
  gloss: happy
  gramm: n
  std: wajyakï
  id: wajyaki-happy
@@ -2601,14 +2798,26 @@
  std: wajyakï
  id: wajyaki-be-happy
  paradigm: v_intr
  paradigm: v_intr_nmlz
  paradigm: vi_aspect
 
 -lexeme
+ lex: wajyama-kiss
+ stem: .wajyama.
+ trans_en: kiss
+ gloss: kiss
+ gramm: vt
+ std: wajyama
+ id: wajyama-kiss
+ paradigm: v_tr
+ paradigm: v_tr_nmlz
+ paradigm: vt_aspect
+
+-lexeme
  lex: wanapu-savannah
  stem: .wanapu.
  trans_en: savannah
  gloss: savannah
  gramm: n
  std: wanapu
  id: wanapu-savannah
@@ -2619,15 +2828,15 @@
  lex: wanene-aunt
  stem: .wanene.
  trans_en: aunt
  gloss: aunt
  gramm: n
  std: wanene
  id: wanene-aunt
- paradigm: noun_c_new_ri_0
+ paradigm: noun_c_old_i_0
  paradigm: n_deriv
 
 -lexeme
  lex: waraijtokomo-man
  stem: .waraijtokomo.|.waraijtokom.|.waraijtokon.
  trans_en: man
  gloss: man
@@ -2918,35 +3127,14 @@
  std: yaka
  id: yaka-dig-out
  paradigm: v_tr
  paradigm: v_tr_nmlz
  paradigm: vt_aspect
 
 -lexeme
- lex: yaku-agouti
- stem: .yaku.
- trans_en: agouti
- gloss: agouti
- gramm: n
- std: yaku
- id: yaku-agouti
- paradigm: noun_c_new_ru_0
- paradigm: n_deriv
-
--lexeme
- lex: yakere-com
- stem: .yakërë.
- trans_en: COM
- gloss: COM
- gramm: postp
- std: yakërë
- id: yakere-com
- paradigm: postp
-
--lexeme
  lex: yamane-make
  stem: .yamanë.|.yaman.|.yamani.
  trans_en: make
  gloss: make
  gramm: vt
  std: yamanë
  id: yamane-make
@@ -3229,14 +3417,26 @@
  std: yopo
  id: yopo-find
  paradigm: v_tr
  paradigm: v_tr_nmlz
  paradigm: vt_aspect
 
 -lexeme
+ lex: yujwa-burn
+ stem: .yujwa.
+ trans_en: burn
+ gloss: burn
+ gramm: vt
+ std: yujwa
+ id: yujwa-burn
+ paradigm: v_tr
+ paradigm: v_tr_nmlz
+ paradigm: vt_aspect
+
+-lexeme
  lex: yumpe-fairly
  stem: .yumpe.
  trans_en: fairly; much
  gloss: fairly
  gramm: adv
  std: yumpe
  id: yumpe-fairly
@@ -3262,28 +3462,39 @@
  gramm: n
  std: yë
  id: ye-tooth
  paradigm: noun_c_new_ri_0
  paradigm: n_deriv
 
 -lexeme
+ lex: yejpe-bone
+ stem: .yëjpë.
+ trans_en: bone
+ gloss: bone
+ gramm: n
+ std: yëjpë
+ id: yejpe-bone
+ paradigm: noun_c_new_ri_0
+ paradigm: n_deriv
+
+-lexeme
  lex: yempeka-offend
  stem: .yëmpëka.
  trans_en: offend
  gloss: offend
  gramm: vt
  std: yëmpëka
  id: yempeka-offend
  paradigm: v_tr
  paradigm: v_tr_nmlz
  paradigm: vt_aspect
 
 -lexeme
  lex: yeni-drink
- stem: .yëni.|.yeni.|.yën.
+ stem: .yëni.|.yeni.|.yën.|.yënï.
  trans_en: drink
  gloss: drink
  gramm: vt
  std: yëni
  id: yeni-drink
  paradigm: v_tr
  paradigm: v_tr_nmlz
@@ -3365,15 +3576,15 @@
  std: ëkërë
  id: ekere-jaguar
  paradigm: noun_v_new_ri_0
  paradigm: n_deriv
 
 -lexeme
  lex: empare-already
- stem: .ëmpare.
+ stem: .ëmpare.|.ïmparë.
  trans_en: already
  gloss: already
  gramm: adv
  std: ëmpare
  id: empare-already
  paradigm: adv
  paradigm: adv_deriv
@@ -3710,37 +3921,14 @@
  std: enejka
  id: enejka-watch
  paradigm: v_tr
  paradigm: v_tr_nmlz
  paradigm: vt_aspect
 
 -lexeme
- lex: wajto-fire
- stem: .wajto.
- trans_en: fire
- gloss: fire
- gramm: n
- std: wajto
- id: wajto-fire
- paradigm: noun_c_new_ri_0
- paradigm: n_deriv
-
--lexeme
- lex: naij-do
- stem: .naij.
- trans_en: do
- gloss: do
- gramm: vt
- std: naij
- id: naij-do
- paradigm: v_tr
- paradigm: v_tr_nmlz
- paradigm: vt_aspect
-
--lexeme
  lex: tawejka-dawn
  stem: .tawejka.
  trans_en: dawn
  gloss: dawn
  gramm: vi
  std: tawejka
  id: tawejka-dawn
@@ -3918,15 +4106,15 @@
  gramm: intj
  std: kïj
  id: kij-ugh
  paradigm: uninfl
 
 -lexeme
  lex: ajaja-hahaha
- stem: .ajaja.
+ stem: .ajaja.|.jajajaja.
  trans_en: hahaha
  gloss: hahaha
  gramm: intj
  std: ajaja
  id: ajaja-hahaha
  paradigm: uninfl
 
@@ -4192,25 +4380,14 @@
  std: yakara
  id: yakara-believe
  paradigm: v_intr
  paradigm: v_intr_nmlz
  paradigm: vi_aspect
 
 -lexeme
- lex: tajnon-piaroa
- stem: .tajnon.
- trans_en: Piaroa
- gloss: Piaroa
- gramm: n
- std: tajnon
- id: tajnon-piaroa
- paradigm: noun_c_new_ri_0
- paradigm: n_deriv
-
--lexeme
  lex: tamanaku-t
  stem: .tamanaku.
  trans_en: T.
  gloss: T.
  gramm: n
  std: tamanaku
  id: tamanaku-t
@@ -4392,25 +4569,14 @@
  gramm: n
  std: nwa
  id: nwa-glute
  paradigm: noun_c_new_ri_0
  paradigm: n_deriv
 
 -lexeme
- lex: enu-eye
- stem: .ënu.
- trans_en: eye
- gloss: eye
- gramm: n
- std: ënu
- id: enu-eye
- paradigm: noun_v_new_ru_0
- paradigm: n_deriv
-
--lexeme
  lex: ejne-below
  stem: .ëjnë.
  trans_en: below
  gloss: below
  gramm: postp
  std: ëjnë
  id: ejne-below
@@ -4522,25 +4688,14 @@
  gramm: n
  std: kawaratu
  id: kawaratu-k
  paradigm: noun_c_new_ru_0
  paradigm: n_deriv
 
 -lexeme
- lex: o-game-food
- stem: .o.
- trans_en: game food
- gloss: game_food
- gramm: n
- std: o
- id: o-game-food
- paradigm: noun_v_new_ti_0
- paradigm: n_deriv
-
--lexeme
  lex: u-starchy-food
  stem: .u.
  trans_en: starchy food
  gloss: starchy_food
  gramm: n
  std: u
  id: u-starchy-food
@@ -4862,25 +5017,14 @@
  gramm: n
  std: yolanda
  id: yolanda-y
  paradigm: noun_c_new_ri_0
  paradigm: n_deriv
 
 -lexeme
- lex: ati-what
- stem: .ati.
- trans_en: what
- gloss: what
- gramm: n
- std: ati
- id: ati-what
- paradigm: noun_v_new_ri_0
- paradigm: n_deriv
-
--lexeme
  lex: pe-ess
  stem: .pe.
  trans_en: ESS
  gloss: ESS
  gramm: postp
  std: pe
  id: pe-ess
@@ -4905,14 +5049,317 @@
  gramm: n
  std: kërë
  id: kere-old
  paradigm: noun_c_new_ri_0
  paradigm: n_deriv
 
 -lexeme
+ lex: enu-eye
+ stem: .ënu.
+ trans_en: eye
+ gloss: eye
+ gramm: n
+ std: ënu
+ id: enu-eye
+ paradigm: noun_v_new_ru_0
+ paradigm: n_deriv
+
+-lexeme
+ lex: emekunu-hand
+ stem: .emekunu.
+ trans_en: hand
+ gloss: hand
+ gramm: n
+ std: emekunu
+ id: emekunu-hand
+ paradigm: noun_v_new_ru_0
+ paradigm: n_deriv
+
+-lexeme
+ lex: ere-liver
+ stem: .ere.
+ trans_en: liver
+ gloss: liver
+ gramm: n
+ std: ere
+ id: ere-liver
+ paradigm: noun_v_new_ri_0
+ paradigm: n_deriv
+
+-lexeme
+ lex: oti-meat
+ stem: .oti.
+ trans_en: meat
+ gloss: meat
+ gramm: n
+ std: oti
+ id: oti-meat
+ paradigm: noun_v_new_ri_0
+ paradigm: n_deriv
+
+-lexeme
+ lex: ena-nose
+ stem: .ëna.
+ trans_en: nose
+ gloss: nose
+ gramm: n
+ std: ëna
+ id: ena-nose
+ paradigm: noun_v_new_ri_0
+ paradigm: n_deriv
+
+-lexeme
+ lex: echi-smoke
+ stem: .ëchi.
+ trans_en: smoke
+ gloss: smoke
+ gramm: n
+ std: ëchi
+ id: echi-smoke
+ paradigm: noun_v_new_ri_0
+ paradigm: n_deriv
+
+-lexeme
+ lex: tepu-stone
+ stem: .tëpu.
+ trans_en: stone
+ gloss: stone
+ gramm: n
+ std: tëpu
+ id: tepu-stone
+ paradigm: noun_c_new_ru_0
+ paradigm: n_deriv
+
+-lexeme
+ lex: ape-arm-wing
+ stem: .apë.
+ trans_en: arm, wing
+ gloss: arm,_wing
+ gramm: n
+ std: apë
+ id: ape-arm-wing
+ paradigm: noun_v_new_ri_0
+ paradigm: n_deriv
+
+-lexeme
+ lex: yeremutu-ash
+ stem: .yeremutu.
+ trans_en: ash
+ gloss: ash
+ gramm: n
+ std: yeremutu
+ id: yeremutu-ash
+ paradigm: noun_c_new_ru_0
+ paradigm: n_deriv
+
+-lexeme
+ lex: kanawa-canoe
+ stem: .kanawa.
+ trans_en: canoe
+ gloss: canoe
+ gramm: n
+ std: kanawa
+ id: kanawa-canoe
+ paradigm: noun_c_new_ri_0
+ paradigm: n_deriv
+
+-lexeme
+ lex: kemichini-be-cold
+ stem: .këmïchini.
+ trans_en: be cold
+ gloss: be_cold
+ gramm: vi
+ std: këmïchini
+ id: kemichini-be-cold
+ paradigm: v_intr
+ paradigm: v_intr_nmlz
+ paradigm: vi_aspect
+
+-lexeme
+ lex: yakuri-agouti
+ stem: .yakuri.
+ trans_en: agouti
+ gloss: agouti
+ gramm: n
+ std: yakuri
+ id: yakuri-agouti
+ paradigm: noun_c_new_ri_0
+ paradigm: n_deriv
+
+-lexeme
+ lex: makampra-aunt
+ stem: .makampra.
+ trans_en: aunt
+ gloss: aunt
+ gramm: n
+ std: makampra
+ id: makampra-aunt
+ paradigm: noun_c_new_ri_0
+ paradigm: n_deriv
+
+-lexeme
+ lex: yemi-be-hungry
+ stem: .yëmï.|.yomi.|.yëmi.
+ trans_en: be hungry
+ gloss: be_hungry
+ gramm: vi
+ std: yëmï
+ id: yemi-be-hungry
+ paradigm: v_intr
+ paradigm: v_intr_nmlz
+ paradigm: vi_aspect
+
+-lexeme
+ lex: ijmojka-cook
+ stem: .ijmojka.|.ijmoka.
+ trans_en: cook
+ gloss: cook
+ gramm: vt
+ std: ijmojka
+ id: ijmojka-cook
+ paradigm: v_tr
+ paradigm: v_tr_nmlz
+ paradigm: vt_aspect
+
+-lexeme
+ lex: padrastro-stepfather
+ stem: .padrastro.
+ trans_en: stepfather
+ gloss: stepfather
+ gramm: n,esp
+ std: padrastro
+ id: padrastro-stepfather
+ paradigm: noun_c_new_ri_0
+ paradigm: n_deriv
+
+-lexeme
+ lex: rafa-r
+ stem: .rafa.
+ trans_en: R.
+ gloss: R.
+ gramm: n
+ std: rafa
+ id: rafa-r
+ paradigm: noun_c_new_ri_0
+ paradigm: n_deriv
+
+-lexeme
+ lex: perez-p
+ stem: .perez.
+ trans_en: P.
+ gloss: P.
+ gramm: n
+ std: perez
+ id: perez-p
+ paradigm: noun_c_new_ri_0
+ paradigm: n_deriv
+
+-lexeme
+ lex: akere-with
+ stem: .akërë.
+ trans_en: with
+ gloss: with
+ gramm: postp
+ std: akërë
+ id: akere-with
+ paradigm: postp
+
+-lexeme
+ lex: ka-all
+ stem: .ka.
+ trans_en: ALL
+ gloss: ALL
+ gramm: postp
+ std: ka
+ id: ka-all
+ paradigm: postp
+
+-lexeme
+ lex: maijte-go-imp
+ stem: .maijtë.
+ trans_en: go.IMP
+ gloss: go.IMP
+ gramm: vi
+ std: maijtë
+ id: maijte-go-imp
+ paradigm: uninfl
+
+-lexeme
+ lex: ammm-um
+ stem: .ammm.
+ trans_en: um
+ gloss: um
+ gramm: intj
+ std: ammm
+ id: ammm-um
+ paradigm: uninfl
+
+-lexeme
+ lex: ejnomo-ejnomo
+ stem: .ejnomo.
+ trans_en: ejnomo
+ gloss: ejnomo
+ gramm: n
+ std: ejnomo
+ id: ejnomo-ejnomo
+ paradigm: noun_v_new_ri_0
+ paradigm: n_deriv
+
+-lexeme
+ lex: jra-neg
+ stem: .jra.
+ trans_en: NEG
+ gloss: NEG
+ gramm: part
+ std: jra
+ id: jra-neg
+ paradigm: uninfl
+
+-lexeme
+ lex: chipokono-because
+ stem: .chipokono.|.chipokon.|.chipëkën.
+ trans_en: because
+ gloss: because
+ gramm: part
+ std: chipokono
+ id: chipokono-because
+ paradigm: uninfl
+
+-lexeme
+ lex: kontomo-pl
+ stem: .kontomo.
+ trans_en: PL
+ gloss: PL
+ gramm: part
+ std: kontomo
+ id: kontomo-pl
+ paradigm: uninfl
+
+-lexeme
+ lex: enirepeke-recently
+ stem: .enirëpëke.
+ trans_en: recently
+ gloss: recently
+ gramm: adv
+ std: enirëpëke
+ id: enirepeke-recently
+ paradigm: adv
+ paradigm: adv_deriv
+
+-lexeme
+ lex: pinita-neg
+ stem: .pïnita.
+ trans_en: NEG
+ gloss: NEG
+ gramm: part
+ std: pïnita
+ id: pinita-neg
+ paradigm: uninfl
+
+-lexeme
  lex: wenaka-vomit
  stem: .wenaka.
  trans_en: vomit
  gloss: vomit
  gramm: vt
  std: wenaka
  id: wenaka-vomit
@@ -5542,15 +5989,15 @@
  id: yatuma-warm
  paradigm: v_tr
  paradigm: v_tr_nmlz
  paradigm: vt_aspect
 
 -lexeme
  lex: yerema-feed
- stem: .yerema.
+ stem: .yerema.|.erema.
  trans_en: feed
  gloss: feed
  gramm: vt
  std: yerema
  id: yerema-feed
  paradigm: v_tr
  paradigm: v_tr_nmlz
@@ -5741,21 +6188,21 @@
  gramm: adv
  std: tapire
  id: tapire-red
  paradigm: adv
  paradigm: adv_deriv
 
 -lexeme
- lex: pechine-pochine-odorous
+ lex: pechine-odorous
  stem: .pëchine.|.pochine.
  trans_en: odorous
  gloss: odorous
  gramm: adv
  std: pëchine
- id: pechine-pochine-odorous
+ id: pechine-odorous
  paradigm: adv
  paradigm: adv_deriv
 
 -lexeme
  lex: makepijke-second-mother
  stem: .makëpïjkë.
  trans_en: second mother
@@ -5783,21 +6230,21 @@
  gloss: go(PLUR)
  gramm: vi
  std: tëpëti
  id: tepeti-go-plur
  paradigm: të
 
 -lexeme
- lex: sejpeti-sejpej-dream
+ lex: sejpeti-dream
  stem: .sejpëti.|.sejpëj.
  trans_en: dream
  gloss: dream
  gramm: vi
  std: sejpëti
- id: sejpeti-sejpej-dream
+ id: sejpeti-dream
  paradigm: v_intr
  paradigm: v_intr_nmlz
  paradigm: vi_aspect
 
 -lexeme
  lex: mujnajte-bury
  stem: .mujnajtë.
@@ -5892,8 +6339,17 @@
 -lexeme
  lex: nwapeke-behind
  stem: .nwa&pëkë.
  gloss: glute&about
  id: nwa-glute,peke-about
  gramm: postp
  paradigm: postp
- trans_en: behind
+ trans_en: behind
+
+-lexeme
+ lex: te-go
+ stem: .maijtë.
+ gloss: go.IMP
+ id: maijte-go-imp
+ gramm: imp,vi
+ paradigm: uninfl
+ trans_en: go!
```

### Comparing `uniparser_yawarana-0.0.5/src/uniparser_yawarana/data/paradigms.txt` & `uniparser_yawarana-0.0.6/src/uniparser_yawarana/data/paradigms.txt`

 * *Files 8% similar despite different names*

```diff
@@ -47,14 +47,18 @@
   gloss: 1
   gramm: 1,poss
   id: u1
  -flex: i.<.>
   gramm: 3,poss
   gloss: 3
   id: i3
+ -flex: ej.<.>
+  gramm: 12,poss
+  gloss: 1+2
+  id: ej12
  -flex: ..<.>
   gramm:
  paradigm: noun_plural
 
 -paradigm: noun_pref_old_c
  -flex: a.<.>//o.<.>//ë.<.>
   gloss: 2
@@ -77,14 +81,15 @@
   gramm: pl
   gloss: PL
   id: tomopl
  -flex: .kontomo<.>//.konton<.>
   gramm: pl
   gloss: PL
   id: kontomopl
+  sep: =
  -flex: .<.>
   gramm:
  paradigm: what_about_second_plural
 
 -paradigm: what_about_second_plural
  -flex: .<.>
   gramm:
@@ -103,15 +108,15 @@
  -flex: .
   gramm: 
 
 -paradigm: noun_clitic
  -flex: .
   gramm:
  -flex: .pe
-  id: peess
+  id: pe-ess
   gramm: ess
   gloss: ESS
   sep: =
 
 -paradigm: mi_clitic
  -flex: .
   gramm:
@@ -123,18 +128,19 @@
 
 -paradigm: n_deriv
  -flex: .
   gramm:
  deriv-link: N-ke
  deriv-link: N-dim
 
--paradigm: n_priv
- -flex: .
-  gramm:
- deriv-link: N-jra
+# jra is a particle
+# -paradigm: n_priv
+#  -flex: .
+#   gramm:
+#  deriv-link: N-jra
 
 -paradigm: noun_c_old_ri_të
  -flex: <.>.ri<.>//<.>.0<.>//<.>.rï<.>
   gloss: PERT
   gramm: pert
   id: rupert
   paradigm: noun_pref_old_c
@@ -260,14 +266,58 @@
   gramm: pert
   id: tipert
   paradigm: noun_pref_new_c
  -flex: .<.>
   gramm:
   paradigm: noun_plural
 
+-paradigm: noun_c_old_i_të
+ -flex: <.>.i<.>
+  gloss: PERT
+  gramm: pert
+  id: ipert
+  paradigm: noun_pref_old_c
+ -flex: .të<.>
+  gloss: NPERT
+  gramm: npert
+  id: tenpert
+  paradigm: noun_plural
+
+-paradigm: noun_c_new_i_të
+ -flex: <.>.i<.>
+  gloss: PERT
+  gramm: pert
+  id: ipert
+  paradigm: noun_pref_new_c
+ -flex: .të<.>
+  gloss: NPERT
+  gramm: npert
+  id: tenpert
+  paradigm: noun_plural
+
+-paradigm: noun_c_old_i_0
+ -flex: <.>.i<.>
+  gloss: PERT
+  gramm: pert
+  id: ipert
+  paradigm: noun_pref_old_c
+ -flex: .<.>
+  gramm:
+  paradigm: noun_plural
+
+-paradigm: noun_c_new_i_0
+ -flex: <.>.i<.>
+  gloss: PERT
+  gramm: pert
+  id: ipert
+  paradigm: noun_pref_new_c
+ -flex: .<.>
+  gramm:
+  paradigm: noun_plural
+
 -paradigm: noun_c_old_0_të
  -flex: <.>.<.>
   gramm:
   paradigm: noun_pref_old_c
  -flex: .të<.>
   gloss: NPERT
   gramm: npert
@@ -428,14 +478,58 @@
   gramm: pert
   id: tipert
   paradigm: noun_pref_new_v
  -flex: .<.>
   gramm:
   paradigm: noun_plural
 
+-paradigm: noun_v_old_i_të
+ -flex: <.>.i<.>
+  gloss: PERT
+  gramm: pert
+  id: ipert
+  paradigm: noun_pref_old_v
+ -flex: .të<.>
+  gloss: NPERT
+  gramm: npert
+  id: tenpert
+  paradigm: noun_plural
+
+-paradigm: noun_v_new_i_të
+ -flex: <.>.i<.>
+  gloss: PERT
+  gramm: pert
+  id: ipert
+  paradigm: noun_pref_new_v
+ -flex: .të<.>
+  gloss: NPERT
+  gramm: npert
+  id: tenpert
+  paradigm: noun_plural
+
+-paradigm: noun_v_old_i_0
+ -flex: <.>.i<.>
+  gloss: PERT
+  gramm: pert
+  id: ipert
+  paradigm: noun_pref_old_v
+ -flex: .<.>
+  gramm:
+  paradigm: noun_plural
+
+-paradigm: noun_v_new_i_0
+ -flex: <.>.i<.>
+  gloss: PERT
+  gramm: pert
+  id: ipert
+  paradigm: noun_pref_new_v
+ -flex: .<.>
+  gramm:
+  paradigm: noun_plural
+
 -paradigm: noun_v_old_0_të
  -flex: <.>.<.>
   gramm:
   paradigm: noun_pref_old_v
  -flex: .të<.>
   gloss: NPERT
   gramm: npert
@@ -630,23 +724,24 @@
 -paradigm: konto_pl
  -flex: .
   gramm:
  -flex: .kontomo//.konton//.kontom
   gramm: pl
   gloss: PL
   id: kontomopl
+  sep: =
 
 -paradigm: v_jra
  -flex: .
   gramm:
- -flex: .jra<.>
-  gloss: NEG
-  gramm: neg
-  id: jraneg
-  paradigm: konto_pl
+ # -flex: .jra<.>
+ #  gloss: NEG
+ #  gramm: neg
+ #  id: jraneg
+ #  paradigm: konto_pl
  -flex: .jnari
   gloss: NEG
   gramm: neg
   id: jnarineg
 
 -paradigm: cop
  -flex: ij.<.>
@@ -695,14 +790,18 @@
   gramm: fut
   gloss: FUT
   id: tojpefut
  -flex: .tojpano
   gramm: fut
   gloss: FUT.CONCL
   id: tojpanofut
+ -flex: .ripo<.>
+  gramm: irr
+  gloss: IRR
+  id: ripoirr
  paradigm: konto_pl
 
 -paradigm: cop_clit
  -flex: .pëkë
   gloss: about
   gramm: LEX:peke-about:about
   id: peke-about
@@ -780,15 +879,19 @@
  -flex: u|y.<.>
   gloss: 1|LK
   gramm: 1,poss
   id: u1,ylk
  -flex: t.<.>
   gloss: 3
   gramm: 3
-  id: i3  
+  id: i3
+ -flex: ej.<.>
+  gramm: 12,poss
+  gloss: 1+2
+  id: ej12
  -flex: .<.>
   gramm:
  paradigm: v_suff
 
 -paradigm: postp
  -flex: u.<.>
   gramm: 1
@@ -826,25 +929,47 @@
   gramm:
  deriv-link: A-ano
  paradigm: postp-suff
 
 -paradigm: postp-suff
  -flex: .
   gramm:
- -flex: .jra
-  gramm: neg
-  gloss: NEG
+ -flex: .jne
+  gramm: pl
+  gloss: PL
+  id: jnepl
+  sep: =
+ # -flex: .jra
+ #  gramm: neg
+ #  gloss: NEG
+ #  id: jraneg
+
+-paradigm: advl
+ -flex: .
+  gramm:
+ -flex: u.
+  gramm: 1
+  gloss: 1
+  id: u1
+ -flex: më.
+  gramm: 2
+  gloss: 2
+  id: me2
+ -flex: ta.
+  gramm: 3P
+  gloss: 3P
+  id: ta-3
 
 -paradigm: adv
  -flex: .
   gramm: 
- -flex: .jra
-  gloss: NEG
-  gramm: neg
-  id: jraneg
+ # -flex: .jra
+ #  gloss: NEG
+ #  gramm: neg
+ #  id: jraneg
 
 -paradigm: adv_deriv
  -flex: .
   gramm: 
  deriv-link: A-mi
- deriv-link: A-mijra
+ # deriv-link: A-mijra
  deriv-link: A-ano
```

### Comparing `uniparser_yawarana-0.0.5/src/uniparser_yawarana.egg-info/PKG-INFO` & `uniparser_yawarana-0.0.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
-Name: uniparser-yawarana
-Version: 0.0.5
+Name: uniparser_yawarana
+Version: 0.0.6
 Summary: A UniParser implementation for morphologically parsing and annotating Yawarana material.
 Home-page: https://github.com/fmatter/uniparser-yawarana
 Author: Florian Matter
 Author-email: florianmatter@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/fmatter/uniparser-yawarana/issues
 Keywords: linguistics,morphology
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -33,8 +31,7 @@
 [![Linting](https://img.shields.io/github/actions/workflow/status/fmatter/uniparser-yawarana/lint.yml?label=linting&branch=main)](https://github.com/fmatter/uniparser-yawarana/actions/workflows/lint.yml)
 [![Codecov](https://img.shields.io/codecov/c/github/fmatter/uniparser-yawarana)](https://app.codecov.io/gh/fmatter/uniparser-yawarana/)
 [![PyPI](https://img.shields.io/pypi/v/uniparser-yawarana.svg)](https://pypi.org/project/uniparser-yawarana)
 ![Versions](https://img.shields.io/pypi/pyversions/uniparser-yawarana)
 
 This project uses the excellent [uniparser-morph](https://github.com/timarkh/uniparser-morph/) package.
 It is currently under development.
-
```

### Comparing `uniparser_yawarana-0.0.5/src/uniparser_yawarana.egg-info/SOURCES.txt` & `uniparser_yawarana-0.0.6/src/uniparser_yawarana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

