# Comparing `tmp/blanc-0.3.1.tar.gz` & `tmp/blanc-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blanc-0.3.1.tar", last modified: Mon Jun 26 23:57:13 2023, max compression
+gzip compressed data, was "blanc-0.3.2.tar", last modified: Tue Jul 25 15:58:14 2023, max compression
```

## Comparing `blanc-0.3.1.tar` & `blanc-0.3.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-06-26 23:57:13.224611 blanc-0.3.1/
-drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-06-26 23:57:13.206010 blanc-0.3.1/.github/
-drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-06-26 23:57:13.208242 blanc-0.3.1/.github/workflows/
--rw-r--r--   0 olegvasilyev   (502) staff       (20)     2532 2022-11-20 20:03:24.000000 blanc-0.3.1/.github/workflows/codeql-analysis.yml
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)       54 2020-04-22 21:28:28.000000 blanc-0.3.1/.gitignore
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)     1049 2020-04-22 21:28:28.000000 blanc-0.3.1/LICENSE
--rw-r--r--   0 olegvasilyev   (502) staff       (20)    13913 2023-06-26 23:57:13.224436 blanc-0.3.1/PKG-INFO
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)    13478 2022-02-10 23:08:14.000000 blanc-0.3.1/README.md
--rw-r--r--   0 olegvasilyev   (502) staff       (20)     1629 2022-11-20 20:03:24.000000 blanc-0.3.1/SECURITY.md
-drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-06-26 23:57:13.210729 blanc-0.3.1/blanc/
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)      133 2022-02-10 23:08:14.000000 blanc-0.3.1/blanc/__init__.py
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)    12173 2021-09-01 21:24:46.000000 blanc-0.3.1/blanc/__main__.py
--rw-r--r--   0 olegvasilyev   (502) staff       (20)       22 2023-06-26 23:53:08.000000 blanc-0.3.1/blanc/__version__.py
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)    36885 2023-06-26 23:31:35.000000 blanc-0.3.1/blanc/blanc.py
--rw-r--r--   0 olegvasilyev   (502) staff       (20)    19293 2022-11-27 19:37:04.000000 blanc-0.3.1/blanc/estime.py
--rw-r--r--   0 olegvasilyev   (502) staff       (20)    11877 2023-06-26 23:53:08.000000 blanc-0.3.1/blanc/shannon.py
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)    16178 2021-03-11 01:31:26.000000 blanc-0.3.1/blanc/utils.py
-drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-06-26 23:57:13.211997 blanc-0.3.1/blanc.egg-info/
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)    13913 2023-06-26 23:57:13.000000 blanc-0.3.1/blanc.egg-info/PKG-INFO
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)      617 2023-06-26 23:57:13.000000 blanc-0.3.1/blanc.egg-info/SOURCES.txt
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)        1 2023-06-26 23:57:13.000000 blanc-0.3.1/blanc.egg-info/dependency_links.txt
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)       46 2023-06-26 23:57:13.000000 blanc-0.3.1/blanc.egg-info/entry_points.txt
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)       98 2023-06-26 23:57:13.000000 blanc-0.3.1/blanc.egg-info/requires.txt
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)        6 2023-06-26 23:57:13.000000 blanc-0.3.1/blanc.egg-info/top_level.txt
-drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-06-26 23:57:13.223514 blanc-0.3.1/data/
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)  2779006 2020-11-22 22:52:16.000000 blanc-0.3.1/data/CNN_DailyMail_555.json
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)  1110748 2020-11-22 22:52:16.000000 blanc-0.3.1/data/DailyNews_300.json
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)  1257825 2020-11-22 22:52:16.000000 blanc-0.3.1/data/DailyNews_300_aspects.json
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)     1361 2021-04-04 18:11:32.000000 blanc-0.3.1/data/README.md
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)      506 2020-04-22 21:28:28.000000 blanc-0.3.1/data/doc-summaries.json
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)      363 2020-04-22 21:28:28.000000 blanc-0.3.1/data/pairs.json
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)      149 2020-04-22 21:28:28.000000 blanc-0.3.1/data/single.json
-drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-06-26 23:57:13.223657 blanc-0.3.1/estime/
--rw-r--r--   0 olegvasilyev   (502) staff       (20)     4053 2023-06-26 23:53:08.000000 blanc-0.3.1/estime/README.md
--rw-r--r--   0 olegvasilyev   (502) staff       (20)       98 2022-11-21 01:28:17.000000 blanc-0.3.1/requirements.txt
--rw-r--r--   0 olegvasilyev   (502) staff       (20)       38 2023-06-26 23:57:13.224649 blanc-0.3.1/setup.cfg
--rw-r--r--   0 olegvasilyev   (502) staff       (20)      948 2023-06-26 23:53:08.000000 blanc-0.3.1/setup.py
-drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-06-26 23:57:13.224135 blanc-0.3.1/shannon/
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)      419 2022-11-27 18:48:19.000000 blanc-0.3.1/shannon/README.md
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)     3541 2022-02-01 01:02:52.000000 blanc-0.3.1/shannon/summeval_score.py
+drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-07-25 15:58:14.173191 blanc-0.3.2/
+drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-07-25 15:58:14.156981 blanc-0.3.2/.github/
+drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-07-25 15:58:14.158835 blanc-0.3.2/.github/workflows/
+-rw-r--r--   0 olegvasilyev   (502) staff       (20)     2532 2022-11-20 20:03:24.000000 blanc-0.3.2/.github/workflows/codeql-analysis.yml
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)       54 2020-04-22 21:28:28.000000 blanc-0.3.2/.gitignore
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)     1049 2020-04-22 21:28:28.000000 blanc-0.3.2/LICENSE
+-rw-r--r--   0 olegvasilyev   (502) staff       (20)    13913 2023-07-25 15:58:14.172984 blanc-0.3.2/PKG-INFO
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)    13478 2022-02-10 23:08:14.000000 blanc-0.3.2/README.md
+-rw-r--r--   0 olegvasilyev   (502) staff       (20)     1629 2022-11-20 20:03:24.000000 blanc-0.3.2/SECURITY.md
+drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-07-25 15:58:14.160749 blanc-0.3.2/blanc/
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)      133 2022-02-10 23:08:14.000000 blanc-0.3.2/blanc/__init__.py
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)    12173 2021-09-01 21:24:46.000000 blanc-0.3.2/blanc/__main__.py
+-rw-r--r--   0 olegvasilyev   (502) staff       (20)       22 2023-07-25 15:57:40.000000 blanc-0.3.2/blanc/__version__.py
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)    36885 2023-06-26 23:31:35.000000 blanc-0.3.2/blanc/blanc.py
+-rw-r--r--   0 olegvasilyev   (502) staff       (20)    20104 2023-07-25 15:57:40.000000 blanc-0.3.2/blanc/estime.py
+-rw-r--r--   0 olegvasilyev   (502) staff       (20)    11877 2023-06-26 23:53:08.000000 blanc-0.3.2/blanc/shannon.py
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)    16178 2021-03-11 01:31:26.000000 blanc-0.3.2/blanc/utils.py
+drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-07-25 15:58:14.161580 blanc-0.3.2/blanc.egg-info/
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)    13913 2023-07-25 15:58:14.000000 blanc-0.3.2/blanc.egg-info/PKG-INFO
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)      617 2023-07-25 15:58:14.000000 blanc-0.3.2/blanc.egg-info/SOURCES.txt
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)        1 2023-07-25 15:58:14.000000 blanc-0.3.2/blanc.egg-info/dependency_links.txt
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)       46 2023-07-25 15:58:14.000000 blanc-0.3.2/blanc.egg-info/entry_points.txt
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)       98 2023-07-25 15:58:14.000000 blanc-0.3.2/blanc.egg-info/requires.txt
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)        6 2023-07-25 15:58:14.000000 blanc-0.3.2/blanc.egg-info/top_level.txt
+drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-07-25 15:58:14.171839 blanc-0.3.2/data/
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)  2779006 2020-11-22 22:52:16.000000 blanc-0.3.2/data/CNN_DailyMail_555.json
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)  1110748 2020-11-22 22:52:16.000000 blanc-0.3.2/data/DailyNews_300.json
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)  1257825 2020-11-22 22:52:16.000000 blanc-0.3.2/data/DailyNews_300_aspects.json
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)     1361 2021-04-04 18:11:32.000000 blanc-0.3.2/data/README.md
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)      506 2020-04-22 21:28:28.000000 blanc-0.3.2/data/doc-summaries.json
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)      363 2020-04-22 21:28:28.000000 blanc-0.3.2/data/pairs.json
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)      149 2020-04-22 21:28:28.000000 blanc-0.3.2/data/single.json
+drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-07-25 15:58:14.171980 blanc-0.3.2/estime/
+-rw-r--r--   0 olegvasilyev   (502) staff       (20)     4053 2023-06-26 23:53:08.000000 blanc-0.3.2/estime/README.md
+-rw-r--r--   0 olegvasilyev   (502) staff       (20)       98 2022-11-21 01:28:17.000000 blanc-0.3.2/requirements.txt
+-rw-r--r--   0 olegvasilyev   (502) staff       (20)       38 2023-07-25 15:58:14.173236 blanc-0.3.2/setup.cfg
+-rw-r--r--   0 olegvasilyev   (502) staff       (20)      948 2023-07-25 15:57:40.000000 blanc-0.3.2/setup.py
+drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-07-25 15:58:14.172545 blanc-0.3.2/shannon/
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)      419 2022-11-27 18:48:19.000000 blanc-0.3.2/shannon/README.md
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)     3541 2022-02-01 01:02:52.000000 blanc-0.3.2/shannon/summeval_score.py
```

### Comparing `blanc-0.3.1/.github/workflows/codeql-analysis.yml` & `blanc-0.3.2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `blanc-0.3.1/LICENSE` & `blanc-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `blanc-0.3.1/PKG-INFO` & `blanc-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blanc
-Version: 0.3.1
+Version: 0.3.2
 Summary: Human-free quality estimation of document summaries
 Home-page: https://github.com/PrimerAI/blanc
 Author: Primer AI
 Author-email: blanc@primer.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `blanc-0.3.1/README.md` & `blanc-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `blanc-0.3.1/SECURITY.md` & `blanc-0.3.2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `blanc-0.3.1/blanc/__main__.py` & `blanc-0.3.2/blanc/__main__.py`

 * *Files identical despite different names*

### Comparing `blanc-0.3.1/blanc/blanc.py` & `blanc-0.3.2/blanc/blanc.py`

 * *Files identical despite different names*

### Comparing `blanc-0.3.1/blanc/estime.py` & `blanc-0.3.2/blanc/estime.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,26 +29,33 @@
         tags_check=None,
         tags_exclude=None,
         input_size_max=450,
         margin=50,
         distance_word_min=8,
         include_all_tokens=False):
         """
+        If output includes either 'soft' or 'coherence', then all the summary tokens are considered,
+        (regardless of 'include_all_tokens'), as it should be for 'soft' and 'coherence'. 
+        If output is only 'alarms', then all the summary tokens are considered only with the setting
+        include_all_tokens=True. The default include_all_tokens=False corresponds to the original 
+        'hard' ESTIME, and is appropriate for normal summaries that have a reasonable tokens overlap 
+        with the text. The original 'hard' ESTIME is useless for intentionally abnormal summaries that 
+        have no any tokens common with text: it would give zero alarms.  
         Args:
             path_mdl (str): model for embeddings of masked tokens
             path_mdl_raw (str): model for raw embeddings
             i_layer_context (int): index of layer to take contextual embeddings from
             device (str): 'cpu' or 'cuda'
             tags_check (List[str]): list of parts of speech to use, each is a tag
                 by NLTK notations. If None, then all words will be used, 
                 no matter which parts of speech they are.
             tags_exclude (List[str]): List or set of part-of-speach tags that should
                 not be considered. Has priority over tags_check.
             include_all_tokens (Boolean): If True then all summary tokens are considered.
-                Otherwise only tokens existing in the text are considered.
+                If False and if output includes only 'alarms', then only tokens existing in the text are considered.
             input_size_max (int): length of input for the model as number of tokens
             margin (int): number of tokens on input edges not to take embeddings from
             distance_word_min (int): minimal distance between the masked tokens 
                 from which embeddings are to ne taken in a single input
             output (List[str]): list of names of measures to get in claim evaluations
 
         """
@@ -62,14 +69,16 @@
         self.get_estime_coherence = self.ESTIME_COHERENCE in self.output
         self.tags_check = tags_check
         self.tags_exclude = tags_exclude
         self.input_size_max = input_size_max
         self.margin = margin
         self.distance_word_min = distance_word_min
         self.include_all_tokens = include_all_tokens
+        if 'soft' in output or 'coherence' in output:
+            self.include_all_tokens = True
         self.model_tokenizer = None
         self.model = None
         self.model_tokenizer = BertTokenizer.from_pretrained(path_mdl)
         self.model = BertForMaskedLM.from_pretrained(path_mdl, output_hidden_states = True).to(self.device)
         self.model.eval()
         if self.get_estime_soft:
             self.model_raw = BertModel.from_pretrained(path_mdl_raw)
```

### Comparing `blanc-0.3.1/blanc/shannon.py` & `blanc-0.3.2/blanc/shannon.py`

 * *Files identical despite different names*

### Comparing `blanc-0.3.1/blanc/utils.py` & `blanc-0.3.2/blanc/utils.py`

 * *Files identical despite different names*

### Comparing `blanc-0.3.1/blanc.egg-info/PKG-INFO` & `blanc-0.3.2/blanc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blanc
-Version: 0.3.1
+Version: 0.3.2
 Summary: Human-free quality estimation of document summaries
 Home-page: https://github.com/PrimerAI/blanc
 Author: Primer AI
 Author-email: blanc@primer.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `blanc-0.3.1/blanc.egg-info/SOURCES.txt` & `blanc-0.3.2/blanc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blanc-0.3.1/data/CNN_DailyMail_555.json` & `blanc-0.3.2/data/CNN_DailyMail_555.json`

 * *Files identical despite different names*

### Comparing `blanc-0.3.1/data/DailyNews_300.json` & `blanc-0.3.2/data/DailyNews_300.json`

 * *Files identical despite different names*

### Comparing `blanc-0.3.1/data/DailyNews_300_aspects.json` & `blanc-0.3.2/data/DailyNews_300_aspects.json`

 * *Files identical despite different names*

### Comparing `blanc-0.3.1/data/README.md` & `blanc-0.3.2/data/README.md`

 * *Files identical despite different names*

### Comparing `blanc-0.3.1/estime/README.md` & `blanc-0.3.2/estime/README.md`

 * *Files identical despite different names*

### Comparing `blanc-0.3.1/setup.py` & `blanc-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import setuptools
 
-version = "0.3.1"
+version = "0.3.2"
 
 with open("README.md", encoding="utf-8") as reader:
     long_description = reader.read()
 
 with open("requirements.txt") as reader:
     requirements = [line.strip() for line in reader]
```

### Comparing `blanc-0.3.1/shannon/summeval_score.py` & `blanc-0.3.2/shannon/summeval_score.py`

 * *Files identical despite different names*

