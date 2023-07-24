# Comparing `tmp/autoevals-0.0.4.tar.gz` & `tmp/autoevals-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoevals-0.0.4.tar", last modified: Wed Jul 12 04:49:31 2023, max compression
+gzip compressed data, was "autoevals-0.0.5.tar", last modified: Mon Jul 24 22:07:36 2023, max compression
```

## Comparing `autoevals-0.0.4.tar` & `autoevals-0.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-12 04:49:31.275469 autoevals-0.0.4/
--rw-r--r--   0 ankur      (501) staff       (20)     1072 2023-07-11 17:08:28.000000 autoevals-0.0.4/LICENSE
--rw-r--r--   0 ankur      (501) staff       (20)     5639 2023-07-12 04:49:31.275309 autoevals-0.0.4/PKG-INFO
--rw-r--r--   0 ankur      (501) staff       (20)     5122 2023-07-11 21:46:08.000000 autoevals-0.0.4/README.md
--rw-r--r--   0 ankur      (501) staff       (20)       31 2023-07-11 06:26:06.000000 autoevals-0.0.4/pyproject.toml
--rw-r--r--   0 ankur      (501) staff       (20)       38 2023-07-12 04:49:31.275510 autoevals-0.0.4/setup.cfg
--rw-r--r--   0 ankur      (501) staff       (20)     1611 2023-07-12 04:49:11.000000 autoevals-0.0.4/setup.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-12 04:49:31.269596 autoevals-0.0.4/src/
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-12 04:49:31.272539 autoevals-0.0.4/src/autoevals/
--rw-r--r--   0 ankur      (501) staff       (20)       61 2023-07-11 06:26:29.000000 autoevals-0.0.4/src/autoevals/__init__.py
--rw-r--r--   0 ankur      (501) staff       (20)     1561 2023-07-11 21:00:52.000000 autoevals-0.0.4/src/autoevals/base.py
--rw-r--r--   0 ankur      (501) staff       (20)     6102 2023-07-11 21:05:09.000000 autoevals-0.0.4/src/autoevals/llm.py
--rw-r--r--   0 ankur      (501) staff       (20)      568 2023-07-11 21:01:18.000000 autoevals-0.0.4/src/autoevals/string.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-12 04:49:31.275056 autoevals-0.0.4/src/autoevals/templates/
--rw-r--r--   0 ankur      (501) staff       (20)      355 2023-07-11 06:26:29.000000 autoevals-0.0.4/src/autoevals/templates/battle.yaml
--rw-r--r--   0 ankur      (501) staff       (20)      312 2023-07-11 06:26:29.000000 autoevals-0.0.4/src/autoevals/templates/closed_q_a.yaml
--rw-r--r--   0 ankur      (501) staff       (20)     1121 2023-07-11 06:26:29.000000 autoevals-0.0.4/src/autoevals/templates/factuality.yaml
--rw-r--r--   0 ankur      (501) staff       (20)      107 2023-07-11 06:26:29.000000 autoevals-0.0.4/src/autoevals/templates/humor.yaml
--rw-r--r--   0 ankur      (501) staff       (20)      636 2023-07-11 06:26:29.000000 autoevals-0.0.4/src/autoevals/templates/possible.yaml
--rw-r--r--   0 ankur      (501) staff       (20)      109 2023-07-11 06:26:29.000000 autoevals-0.0.4/src/autoevals/templates/security.yaml
--rw-r--r--   0 ankur      (501) staff       (20)     1076 2023-07-11 06:26:29.000000 autoevals-0.0.4/src/autoevals/templates/sql.yaml
--rw-r--r--   0 ankur      (501) staff       (20)      356 2023-07-11 17:44:18.000000 autoevals-0.0.4/src/autoevals/templates/summary.yaml
--rw-r--r--   0 ankur      (501) staff       (20)      683 2023-07-11 06:26:29.000000 autoevals-0.0.4/src/autoevals/templates/translation.yaml
--rw-r--r--   0 ankur      (501) staff       (20)     4780 2023-07-11 20:58:26.000000 autoevals-0.0.4/src/autoevals/test_llm.py
--rw-r--r--   0 ankur      (501) staff       (20)      546 2023-07-11 20:10:50.000000 autoevals-0.0.4/src/autoevals/test_string.py
--rw-r--r--   0 ankur      (501) staff       (20)      307 2023-07-11 06:26:29.000000 autoevals-0.0.4/src/autoevals/util.py
--rw-r--r--   0 ankur      (501) staff       (20)       18 2023-07-12 04:49:20.000000 autoevals-0.0.4/src/autoevals/version.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-12 04:49:31.273150 autoevals-0.0.4/src/autoevals.egg-info/
--rw-r--r--   0 ankur      (501) staff       (20)     5639 2023-07-12 04:49:31.000000 autoevals-0.0.4/src/autoevals.egg-info/PKG-INFO
--rw-r--r--   0 ankur      (501) staff       (20)      758 2023-07-12 04:49:31.000000 autoevals-0.0.4/src/autoevals.egg-info/SOURCES.txt
--rw-r--r--   0 ankur      (501) staff       (20)        1 2023-07-12 04:49:31.000000 autoevals-0.0.4/src/autoevals.egg-info/dependency_links.txt
--rw-r--r--   0 ankur      (501) staff       (20)      268 2023-07-12 04:49:31.000000 autoevals-0.0.4/src/autoevals.egg-info/requires.txt
--rw-r--r--   0 ankur      (501) staff       (20)       10 2023-07-12 04:49:31.000000 autoevals-0.0.4/src/autoevals.egg-info/top_level.txt
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-24 22:07:36.246872 autoevals-0.0.5/
+-rw-r--r--   0 ankur      (501) staff       (20)     1072 2023-07-11 17:08:28.000000 autoevals-0.0.5/LICENSE
+-rw-r--r--   0 ankur      (501) staff       (20)     5639 2023-07-24 22:07:36.246072 autoevals-0.0.5/PKG-INFO
+-rw-r--r--   0 ankur      (501) staff       (20)     5122 2023-07-11 21:46:08.000000 autoevals-0.0.5/README.md
+-rw-r--r--   0 ankur      (501) staff       (20)       31 2023-07-11 06:26:06.000000 autoevals-0.0.5/pyproject.toml
+-rw-r--r--   0 ankur      (501) staff       (20)       38 2023-07-24 22:07:36.246980 autoevals-0.0.5/setup.cfg
+-rw-r--r--   0 ankur      (501) staff       (20)     1611 2023-07-12 04:49:11.000000 autoevals-0.0.5/setup.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-24 22:07:36.229387 autoevals-0.0.5/src/
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-24 22:07:36.234019 autoevals-0.0.5/src/autoevals/
+-rw-r--r--   0 ankur      (501) staff       (20)       61 2023-07-11 06:26:29.000000 autoevals-0.0.5/src/autoevals/__init__.py
+-rw-r--r--   0 ankur      (501) staff       (20)     1528 2023-07-24 08:40:40.000000 autoevals-0.0.5/src/autoevals/base.py
+-rw-r--r--   0 ankur      (501) staff       (20)     6191 2023-07-24 08:40:40.000000 autoevals-0.0.5/src/autoevals/llm.py
+-rw-r--r--   0 ankur      (501) staff       (20)      673 2023-07-24 08:40:40.000000 autoevals-0.0.5/src/autoevals/string.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-24 22:07:36.245757 autoevals-0.0.5/src/autoevals/templates/
+-rw-r--r--   0 ankur      (501) staff       (20)      355 2023-07-11 06:26:29.000000 autoevals-0.0.5/src/autoevals/templates/battle.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      312 2023-07-11 06:26:29.000000 autoevals-0.0.5/src/autoevals/templates/closed_q_a.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)     1121 2023-07-11 06:26:29.000000 autoevals-0.0.5/src/autoevals/templates/factuality.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      107 2023-07-11 06:26:29.000000 autoevals-0.0.5/src/autoevals/templates/humor.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      636 2023-07-11 06:26:29.000000 autoevals-0.0.5/src/autoevals/templates/possible.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      109 2023-07-11 06:26:29.000000 autoevals-0.0.5/src/autoevals/templates/security.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)     1076 2023-07-11 06:26:29.000000 autoevals-0.0.5/src/autoevals/templates/sql.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      356 2023-07-11 17:44:18.000000 autoevals-0.0.5/src/autoevals/templates/summary.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      683 2023-07-11 06:26:29.000000 autoevals-0.0.5/src/autoevals/templates/translation.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)     4780 2023-07-11 20:58:26.000000 autoevals-0.0.5/src/autoevals/test_llm.py
+-rw-r--r--   0 ankur      (501) staff       (20)      552 2023-07-24 08:40:40.000000 autoevals-0.0.5/src/autoevals/test_string.py
+-rw-r--r--   0 ankur      (501) staff       (20)      307 2023-07-11 06:26:29.000000 autoevals-0.0.5/src/autoevals/util.py
+-rw-r--r--   0 ankur      (501) staff       (20)       18 2023-07-24 22:07:19.000000 autoevals-0.0.5/src/autoevals/version.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-24 22:07:36.242717 autoevals-0.0.5/src/autoevals.egg-info/
+-rw-r--r--   0 ankur      (501) staff       (20)     5639 2023-07-24 22:07:36.000000 autoevals-0.0.5/src/autoevals.egg-info/PKG-INFO
+-rw-r--r--   0 ankur      (501) staff       (20)      758 2023-07-24 22:07:36.000000 autoevals-0.0.5/src/autoevals.egg-info/SOURCES.txt
+-rw-r--r--   0 ankur      (501) staff       (20)        1 2023-07-24 22:07:36.000000 autoevals-0.0.5/src/autoevals.egg-info/dependency_links.txt
+-rw-r--r--   0 ankur      (501) staff       (20)      268 2023-07-24 22:07:36.000000 autoevals-0.0.5/src/autoevals.egg-info/requires.txt
+-rw-r--r--   0 ankur      (501) staff       (20)       10 2023-07-24 22:07:36.000000 autoevals-0.0.5/src/autoevals.egg-info/top_level.txt
```

### Comparing `autoevals-0.0.4/LICENSE` & `autoevals-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.4/PKG-INFO` & `autoevals-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoevals
-Version: 0.0.4
+Version: 0.0.5
 Summary: Universal library for evaluating AI models
 Home-page: https://www.braintrustdata.com
 Author: BrainTrust
 Author-email: info@braintrustdata.com
 Project-URL: Bug Tracker, https://github.com/braintrustdata/autoevals
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `autoevals-0.0.4/README.md` & `autoevals-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.4/setup.py` & `autoevals-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.4/src/autoevals/base.py` & `autoevals-0.0.5/src/autoevals/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-import asyncio
 import dataclasses
-import json
 from abc import ABC, abstractmethod
 
 from .util import SerializableDataClass
 
 
 @dataclasses.dataclass
 class Evaluation(SerializableDataClass):
@@ -41,12 +39,12 @@
         return self.eval(output, expected, **kwargs)
 
     async def _run_eval_async(self, output, expected=None, **kwargs) -> Evaluation:
         # By default we just run the sync version in a thread
         return self._run_eval_sync(output, expected, **kwargs)
 
     @abstractmethod
-    async def _run_eval_sync(self, output, expected=None, **kwargs) -> Evaluation:
+    def _run_eval_sync(self, output, expected=None, **kwargs) -> Evaluation:
         ...
 
 
 __all__ = ["Evaluation", "Evaluator"]
```

### Comparing `autoevals-0.0.4/src/autoevals/llm.py` & `autoevals-0.0.5/src/autoevals/llm.py`

 * *Files 4% similar despite different names*

```diff
@@ -177,11 +177,14 @@
                 raise AttributeError(f"Model template {name} not found")
 
             return LLMClassifier.from_spec_file(os.path.join(SCRIPT_DIR, "templates", template_name), **kwargs)
 
     return C
 
 
-for model in MODEL_TEMPLATES:
-    globals()[model] = _build_template_class(model)
+def _init_model_templates():
+    for model_template in MODEL_TEMPLATES:
+        globals()[model_template] = _build_template_class(model_template)
 
+
+_init_model_templates()
 __all__ = ["GuidanceLLMClassifier", "LLMClassifier"] + list(MODEL_TEMPLATES)
```

### Comparing `autoevals-0.0.4/src/autoevals/string.py` & `autoevals-0.0.5/src/autoevals/string.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 from Levenshtein import distance
 
-from .base import Evaluator
+from autoevals.base import Evaluation
+
+from .base import Evaluation, Evaluator
 
 
 class LevenshteinEvaluator(Evaluator):
-    async def _run_eval_sync(self, output, expected=None, **kwargs):
+    def _run_eval_sync(self, output, expected=None, **kwargs):
         if expected is None:
             raise ValueError("LevenshteinEvaluator requires an expected value")
 
         output, expected = str(output), str(expected)
         max_len = max(len(x) for x in [output, expected])
+
         if max_len == 0:
-            return 1
+            score = 1
+        else:
+            score = 1 - (distance(output, expected) / max(len(x) for x in [output, expected]))
 
-        return 1 - (distance(output, expected) / max(len(x) for x in [output, expected]))
+        return Evaluation(score=score)
 
 
 __all__ = ["LevenshteinEvaluator"]
```

### Comparing `autoevals-0.0.4/src/autoevals/templates/factuality.yaml` & `autoevals-0.0.5/src/autoevals/templates/factuality.yaml`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.4/src/autoevals/templates/possible.yaml` & `autoevals-0.0.5/src/autoevals/templates/possible.yaml`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.4/src/autoevals/templates/sql.yaml` & `autoevals-0.0.5/src/autoevals/templates/sql.yaml`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.4/src/autoevals/templates/translation.yaml` & `autoevals-0.0.5/src/autoevals/templates/translation.yaml`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.4/src/autoevals/test_llm.py` & `autoevals-0.0.5/src/autoevals/test_llm.py`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.4/src/autoevals/test_string.py` & `autoevals-0.0.5/src/autoevals/test_string.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,8 +13,8 @@
         ("abc", "axc", 0.6666666666666667),
         ("xabxcdxxefxgx", "1ab2cd34ef5g6", 0.5384615384615384),
     ]
 
     evaluator = LevenshteinEvaluator()
     for a, b, expected in cases:
         print(f"[{a}]", f"[{b}]", expected, evaluator(a, b))
-        assert evaluator(a, b) == expected
+        assert evaluator(a, b).score == expected
```

### Comparing `autoevals-0.0.4/src/autoevals.egg-info/PKG-INFO` & `autoevals-0.0.5/src/autoevals.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoevals
-Version: 0.0.4
+Version: 0.0.5
 Summary: Universal library for evaluating AI models
 Home-page: https://www.braintrustdata.com
 Author: BrainTrust
 Author-email: info@braintrustdata.com
 Project-URL: Bug Tracker, https://github.com/braintrustdata/autoevals
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `autoevals-0.0.4/src/autoevals.egg-info/SOURCES.txt` & `autoevals-0.0.5/src/autoevals.egg-info/SOURCES.txt`

 * *Files identical despite different names*

