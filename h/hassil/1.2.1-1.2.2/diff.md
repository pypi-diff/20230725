# Comparing `tmp/hassil-1.2.1.tar.gz` & `tmp/hassil-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hassil-1.2.1.tar", last modified: Mon Jul 24 21:51:36 2023, max compression
+gzip compressed data, was "hassil-1.2.2.tar", last modified: Tue Jul 25 16:39:14 2023, max compression
```

## Comparing `hassil-1.2.1.tar` & `hassil-1.2.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-24 21:51:36.274543 hassil-1.2.1/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      689 2023-01-23 19:07:47.000000 hassil-1.2.1/HassILGrammar.g4
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11357 2022-12-05 18:00:35.000000 hassil-1.2.1/LICENSE.md
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      196 2022-12-20 17:37:34.000000 hassil-1.2.1/MANIFEST.in
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4547 2023-07-24 21:51:36.274543 hassil-1.2.1/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3808 2023-07-24 20:05:10.000000 hassil-1.2.1/README.md
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-24 21:51:36.274543 hassil-1.2.1/hassil/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        6 2023-07-24 21:46:25.000000 hassil-1.2.1/hassil/VERSION
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      304 2023-02-01 04:31:35.000000 hassil-1.2.1/hassil/__init__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2552 2023-01-23 19:07:47.000000 hassil-1.2.1/hassil/__main__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      468 2022-12-15 16:06:23.000000 hassil-1.2.1/hassil/_resources.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2355 2023-07-24 20:05:10.000000 hassil-1.2.1/hassil/expression.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    10271 2023-07-24 20:05:10.000000 hassil-1.2.1/hassil/intents.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6797 2023-07-24 20:05:10.000000 hassil-1.2.1/hassil/parse_expression.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     8111 2023-07-24 20:05:10.000000 hassil-1.2.1/hassil/parser.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        0 2022-12-15 16:07:59.000000 hassil-1.2.1/hassil/py.typed
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    34854 2023-07-24 21:50:30.000000 hassil-1.2.1/hassil/recognize.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7448 2023-02-10 20:53:57.000000 hassil-1.2.1/hassil/sample.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      783 2023-02-01 04:31:35.000000 hassil-1.2.1/hassil/sample_template.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1725 2023-01-23 19:07:47.000000 hassil-1.2.1/hassil/util.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-24 21:51:36.274543 hassil-1.2.1/hassil.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4547 2023-07-24 21:51:36.000000 hassil-1.2.1/hassil.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      689 2023-07-24 21:51:36.000000 hassil-1.2.1/hassil.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-07-24 21:51:36.000000 hassil-1.2.1/hassil.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       48 2023-07-24 21:51:36.000000 hassil-1.2.1/hassil.egg-info/entry_points.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       60 2023-07-24 21:51:36.000000 hassil-1.2.1/hassil.egg-info/requires.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        7 2023-07-24 21:51:36.000000 hassil-1.2.1/hassil.egg-info/top_level.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-02-01 04:31:35.000000 hassil-1.2.1/requirements.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       69 2023-07-17 19:53:41.000000 hassil-1.2.1/requirements_dev.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      295 2023-07-24 21:51:36.274543 hassil-1.2.1/setup.cfg
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2069 2023-02-10 21:31:32.000000 hassil-1.2.1/setup.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-24 21:51:36.274543 hassil-1.2.1/tests/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       63 2022-12-07 21:08:40.000000 hassil-1.2.1/tests/__init__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3500 2023-07-24 20:05:10.000000 hassil-1.2.1/tests/test_expression.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4687 2023-07-24 20:05:10.000000 hassil-1.2.1/tests/test_intents.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1755 2023-02-01 04:31:35.000000 hassil-1.2.1/tests/test_parser.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    17123 2023-07-24 21:50:53.000000 hassil-1.2.1/tests/test_recognize.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1906 2023-02-01 04:31:35.000000 hassil-1.2.1/tests/test_sample.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      913 2023-01-23 19:07:47.000000 hassil-1.2.1/tests/test_util.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-25 16:39:14.466897 hassil-1.2.2/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      689 2023-01-23 19:07:47.000000 hassil-1.2.2/HassILGrammar.g4
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11357 2022-12-05 18:00:35.000000 hassil-1.2.2/LICENSE.md
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      196 2022-12-20 17:37:34.000000 hassil-1.2.2/MANIFEST.in
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4548 2023-07-25 16:39:14.466897 hassil-1.2.2/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3808 2023-07-24 20:05:10.000000 hassil-1.2.2/README.md
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-25 16:39:14.466897 hassil-1.2.2/hassil/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        6 2023-07-25 14:47:00.000000 hassil-1.2.2/hassil/VERSION
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      304 2023-02-01 04:31:35.000000 hassil-1.2.2/hassil/__init__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2552 2023-01-23 19:07:47.000000 hassil-1.2.2/hassil/__main__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      468 2022-12-15 16:06:23.000000 hassil-1.2.2/hassil/_resources.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2355 2023-07-24 20:05:10.000000 hassil-1.2.2/hassil/expression.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    10271 2023-07-24 20:05:10.000000 hassil-1.2.2/hassil/intents.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6797 2023-07-24 20:05:10.000000 hassil-1.2.2/hassil/parse_expression.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     8111 2023-07-24 20:05:10.000000 hassil-1.2.2/hassil/parser.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        0 2022-12-15 16:07:59.000000 hassil-1.2.2/hassil/py.typed
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    36650 2023-07-25 16:32:53.000000 hassil-1.2.2/hassil/recognize.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7448 2023-02-10 20:53:57.000000 hassil-1.2.2/hassil/sample.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      783 2023-02-01 04:31:35.000000 hassil-1.2.2/hassil/sample_template.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1725 2023-01-23 19:07:47.000000 hassil-1.2.2/hassil/util.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-25 16:39:14.466897 hassil-1.2.2/hassil.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4548 2023-07-25 16:39:14.000000 hassil-1.2.2/hassil.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      689 2023-07-25 16:39:14.000000 hassil-1.2.2/hassil.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-07-25 16:39:14.000000 hassil-1.2.2/hassil.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       48 2023-07-25 16:39:14.000000 hassil-1.2.2/hassil.egg-info/entry_points.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       60 2023-07-25 16:39:14.000000 hassil-1.2.2/hassil.egg-info/requires.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        7 2023-07-25 16:39:14.000000 hassil-1.2.2/hassil.egg-info/top_level.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-02-01 04:31:35.000000 hassil-1.2.2/requirements.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       69 2023-07-17 19:53:41.000000 hassil-1.2.2/requirements_dev.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      295 2023-07-25 16:39:14.466897 hassil-1.2.2/setup.cfg
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2070 2023-07-25 14:23:19.000000 hassil-1.2.2/setup.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-07-25 16:39:14.466897 hassil-1.2.2/tests/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       63 2022-12-07 21:08:40.000000 hassil-1.2.2/tests/__init__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3500 2023-07-24 20:05:10.000000 hassil-1.2.2/tests/test_expression.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4687 2023-07-24 20:05:10.000000 hassil-1.2.2/tests/test_intents.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1755 2023-02-01 04:31:35.000000 hassil-1.2.2/tests/test_parser.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    23283 2023-07-25 16:32:41.000000 hassil-1.2.2/tests/test_recognize.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1906 2023-02-01 04:31:35.000000 hassil-1.2.2/tests/test_sample.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      913 2023-01-23 19:07:47.000000 hassil-1.2.2/tests/test_util.py
```

### Comparing `hassil-1.2.1/HassILGrammar.g4` & `hassil-1.2.2/HassILGrammar.g4`

 * *Files identical despite different names*

### Comparing `hassil-1.2.1/LICENSE.md` & `hassil-1.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hassil-1.2.1/PKG-INFO` & `hassil-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: hassil
-Version: 1.2.1
+Version: 1.2.2
 Summary: The Home Assistant Intent Language parser
 Home-page: http://github.com/home-assistant/hassil
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: Apache-2.0
 Keywords: home assistant intent recognition
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # HassIL
 
 The Home Assistant Intent Language (HassIL) parser for [intents](https://github.com/home-assistant/intents).
```

### Comparing `hassil-1.2.1/README.md` & `hassil-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `hassil-1.2.1/hassil/__main__.py` & `hassil-1.2.2/hassil/__main__.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.1/hassil/expression.py` & `hassil-1.2.2/hassil/expression.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.1/hassil/intents.py` & `hassil-1.2.2/hassil/intents.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.1/hassil/parse_expression.py` & `hassil-1.2.2/hassil/parse_expression.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.1/hassil/parser.py` & `hassil-1.2.2/hassil/parser.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.1/hassil/recognize.py` & `hassil-1.2.2/hassil/recognize.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Methods for recognizing intents from text."""
 
 import collections.abc
 import itertools
 import re
 from abc import ABC
 from dataclasses import dataclass, field
-from typing import Any, Dict, Iterable, List, Optional, cast
+from typing import Any, Dict, Iterable, List, Optional
 
 from .expression import (
     Expression,
     ListReference,
     RuleReference,
     Sentence,
     Sequence,
@@ -27,14 +27,16 @@
 )
 from .util import normalize_text, normalize_whitespace
 
 NUMBER_START = re.compile(r"^(\s*-?[0-9]+)")
 PUNCTUATION = re.compile(r"[.。,，?¿？؟!！;；:：]+")
 WHITESPACE = re.compile(r"\s+")
 
+MISSING_ENTITY = "<missing>"
+
 
 class HassilError(Exception):
     """Base class for hassil errors"""
 
 
 class MissingListError(HassilError):
     """Error when a {slot_list} is missing."""
@@ -152,19 +154,48 @@
         """True if no text is left that isn't just whitespace or punctuation"""
         text = PUNCTUATION.sub("", self.text).strip()
         if text:
             return False
 
         # Wildcards cannot be empty
         for entity in self.entities:
-            if entity.is_wildcard and (not entity.text):
+            if entity.is_wildcard and (not entity.text.strip()):
+                return False
+
+        # Unmatched entities cannot be empty
+        for unmatched_entity in self.unmatched_entities:
+            if isinstance(unmatched_entity, UnmatchedTextEntity) and (
+                not unmatched_entity.text.strip()
+            ):
                 return False
 
         return True
 
+    def get_open_wildcard(self) -> Optional[MatchEntity]:
+        """Get the last open wildcard or None."""
+        if not self.entities:
+            return None
+
+        last_entity = self.entities[-1]
+        if last_entity.is_wildcard and last_entity.is_wildcard_open:
+            return last_entity
+
+        return None
+
+    def get_open_entity(self) -> Optional[UnmatchedTextEntity]:
+        """Get the last open unmatched text entity or None."""
+        if not self.unmatched_entities:
+            return None
+
+        last_entity = self.unmatched_entities[-1]
+        if isinstance(last_entity, UnmatchedTextEntity) and last_entity.is_open:
+            return last_entity
+
+        return None
+
 
 @dataclass
 class RecognizeResult:
     """Result of recognition."""
 
     intent: Intent
     """Matched intent"""
@@ -297,15 +328,15 @@
     )
 
     # Check sentence against each intent.
     # This should eventually be done in parallel.
     for intent in intents.intents.values():
         for intent_data in intent.data:
             if intent_context:
-                # Skip sentence templates that can't possible be matched due to
+                # Skip sentence templates that can't possibly be matched due to
                 # requires/excludes context.
                 #
                 # Additional context can be added during matching, so we can
                 # only be sure about keys that exist right now.
                 skip_data = False
                 if intent_data.requires_context:
                     for (
@@ -372,37 +403,21 @@
                 maybe_match_contexts = match_expression(
                     local_settings, match_context, intent_sentence
                 )
                 for maybe_match_context in maybe_match_contexts:
                     # Close any open wildcards or unmatched entities
                     final_text = maybe_match_context.text.strip()
                     if final_text:
-                        if (
-                            maybe_match_context.unmatched_entities
-                            and isinstance(
-                                maybe_match_context.unmatched_entities[-1],
-                                UnmatchedTextEntity,
-                            )
-                            and maybe_match_context.unmatched_entities[-1].is_open
-                        ):
+                        if unmatched_entity := maybe_match_context.get_open_entity():
                             # Consume the rest of the text (unmatched entity)
-                            unmatched_entity = cast(
-                                UnmatchedTextEntity,
-                                maybe_match_context.unmatched_entities[-1],
-                            )
                             unmatched_entity.text += final_text
                             unmatched_entity.is_open = False
                             maybe_match_context.text = ""
-                        elif (
-                            maybe_match_context.entities
-                            and maybe_match_context.entities[-1].is_wildcard
-                            and maybe_match_context.entities[-1].is_wildcard_open
-                        ):
+                        elif wildcard := maybe_match_context.get_open_wildcard():
                             # Consume the rest of the text (wildcard)
-                            wildcard = maybe_match_context.entities[-1]
                             wildcard.text += final_text
                             wildcard.value = wildcard.text
                             wildcard.is_wildcard_open = False
                             maybe_match_context.text = ""
 
                     if not maybe_match_context.is_match:
                         # Incomplete match with text still left at the end
@@ -439,14 +454,27 @@
                             context_key,
                             context_value,
                         ) in intent_data.requires_context.items():
                             actual_value = maybe_match_context.intent_context.get(
                                 context_key
                             )
 
+                            if allow_unmatched_entities and (actual_value is None):
+                                # Look in unmatched entities
+                                for (
+                                    unmatched_context_entity
+                                ) in maybe_match_context.unmatched_entities:
+                                    if (
+                                        unmatched_context_entity.name == context_key
+                                    ) and isinstance(
+                                        unmatched_context_entity, UnmatchedTextEntity
+                                    ):
+                                        actual_value = unmatched_context_entity.text
+                                        break
+
                             if (
                                 actual_value == context_value
                                 and context_value is not None
                             ):
                                 # Exact match to context value, except when context value is required and not provided
                                 continue
 
@@ -458,27 +486,50 @@
                                 isinstance(context_value, collections.abc.Collection)
                                 and not isinstance(context_value, str)
                                 and (actual_value in context_value)
                             ):
                                 # Actual value was in context value list
                                 continue
 
-                            # Did not match required context
-                            skip_match = True
-                            break
+                            if allow_unmatched_entities:
+                                # Create missing entity as unmatched
+                                has_unmatched_entity = False
+                                for (
+                                    unmatched_context_entity
+                                ) in maybe_match_context.unmatched_entities:
+                                    if unmatched_context_entity.name == context_key:
+                                        has_unmatched_entity = True
+                                        break
+
+                                if not has_unmatched_entity:
+                                    maybe_match_context.unmatched_entities.append(
+                                        UnmatchedTextEntity(
+                                            name=context_key,
+                                            text=MISSING_ENTITY,
+                                            is_open=False,
+                                        )
+                                    )
+                            else:
+                                # Did not match required context
+                                skip_match = True
+                                break
 
                     if skip_match:
                         # Intent context did not match
                         continue
 
                     # Add fixed entities
+                    entity_names = set(
+                        entity.name for entity in maybe_match_context.entities
+                    )
                     for slot_name, slot_value in intent_data.slots.items():
-                        maybe_match_context.entities.append(
-                            MatchEntity(name=slot_name, value=slot_value, text="")
-                        )
+                        if slot_name not in entity_names:
+                            maybe_match_context.entities.append(
+                                MatchEntity(name=slot_name, value=slot_value, text="")
+                            )
 
                     # Return each match
                     response = default_response
                     if intent_data.response is not None:
                         response = intent_data.response
 
                     yield RecognizeResult(
@@ -640,50 +691,39 @@
                     text=context_text,
                     # Copy over
                     entities=context.entities,
                     intent_context=context.intent_context,
                     is_start_of_word=context.is_start_of_word,
                     unmatched_entities=context.unmatched_entities,
                 )
-            elif (
-                context.entities
-                and context.entities[-1].is_wildcard
-                and context.entities[-1].is_wildcard_open
-            ):
+            elif wildcard := context.get_open_wildcard():
                 # Add to wildcard by skipping ahead in the text until we find
                 # the current chunk text.
                 skip_idx = context_text.find(chunk_text)
                 if skip_idx >= 0:
-                    wildcard = context.entities[-1]
                     wildcard.text += context_text[:skip_idx]
 
                     # Wildcards cannot be empty
                     if wildcard.text:
                         wildcard.value = wildcard.text
                         yield MatchContext(
                             text=context.text[skip_idx + len(chunk_text) :],
                             # Copy over
                             entities=context.entities,
                             intent_context=context.intent_context,
                             is_start_of_word=True,
                             unmatched_entities=context.unmatched_entities,
                         )
-            elif (
-                settings.allow_unmatched_entities
-                and context.unmatched_entities
-                and isinstance(context.unmatched_entities[-1], UnmatchedTextEntity)
-                and context.unmatched_entities[-1].is_open
+            elif settings.allow_unmatched_entities and (
+                unmatched_entity := context.get_open_entity()
             ):
                 # Add to the most recent unmatched entity by skipping ahead in
                 # the text until we find the current chunk text.
                 skip_idx = context_text.find(chunk_text)
                 if skip_idx >= 0:
-                    unmatched_entity = cast(
-                        UnmatchedTextEntity, context.unmatched_entities[-1]
-                    )
                     unmatched_entity.text += context_text[:skip_idx]
 
                     # Unmatched entities cannot be empty
                     if unmatched_entity.text:
                         yield MatchContext(
                             text=context.text[skip_idx + len(chunk_text) :],
                             # Copy over
@@ -791,15 +831,15 @@
                             # Copy over
                             text=context.text,
                             entities=context.entities,
                             intent_context=context.intent_context,
                             is_start_of_word=context.is_start_of_word,
                             #
                             unmatched_entities=context.unmatched_entities
-                            + [UnmatchedTextEntity(name=list_ref.list_name, text="")],
+                            + [UnmatchedTextEntity(name=list_ref.slot_name, text="")],
                             close_wildcards=True,
                         )
 
         elif isinstance(slot_list, RangeSlotList):
             if context.text:
                 # List that represents a number range.
                 # Numbers must currently be digits ("1" not "one").
@@ -842,29 +882,29 @@
                             entities=context.entities,
                             intent_context=context.intent_context,
                             is_start_of_word=context.is_start_of_word,
                             #
                             unmatched_entities=context.unmatched_entities
                             + [
                                 UnmatchedRangeEntity(
-                                    name=list_ref.list_name, value=word_number
+                                    name=list_ref.slot_name, value=word_number
                                 )
                             ],
                         )
                 elif settings.allow_unmatched_entities:
                     # Report not a number
                     yield MatchContext(
                         # Copy over
                         text=context.text,
                         entities=context.entities,
                         intent_context=context.intent_context,
                         is_start_of_word=context.is_start_of_word,
                         #
                         unmatched_entities=context.unmatched_entities
-                        + [UnmatchedTextEntity(name=list_ref.list_name, text="")],
+                        + [UnmatchedTextEntity(name=list_ref.slot_name, text="")],
                         close_wildcards=True,
                     )
         elif isinstance(slot_list, WildcardSlotList):
             if context.text:
                 # Start wildcard entities
                 yield MatchContext(
                     # Copy over
@@ -872,15 +912,15 @@
                     intent_context=context.intent_context,
                     is_start_of_word=context.is_start_of_word,
                     unmatched_entities=context.unmatched_entities,
                     #
                     entities=context.entities
                     + [
                         MatchEntity(
-                            name=list_ref.list_name, value="", text="", is_wildcard=True
+                            name=list_ref.slot_name, value="", text="", is_wildcard=True
                         )
                     ],
                     close_unmatched=True,
                 )
         else:
             raise ValueError(f"Unexpected slot list type: {slot_list}")
```

### Comparing `hassil-1.2.1/hassil/sample.py` & `hassil-1.2.2/hassil/sample.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.1/hassil/sample_template.py` & `hassil-1.2.2/hassil/sample_template.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.1/hassil/util.py` & `hassil-1.2.2/hassil/util.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.1/hassil.egg-info/PKG-INFO` & `hassil-1.2.2/hassil.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: hassil
-Version: 1.2.1
+Version: 1.2.2
 Summary: The Home Assistant Intent Language parser
 Home-page: http://github.com/home-assistant/hassil
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: Apache-2.0
 Keywords: home assistant intent recognition
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # HassIL
 
 The Home Assistant Intent Language (HassIL) parser for [intents](https://github.com/home-assistant/intents).
```

### Comparing `hassil-1.2.1/hassil.egg-info/SOURCES.txt` & `hassil-1.2.2/hassil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hassil-1.2.1/setup.py` & `hassil-1.2.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,14 +49,14 @@
         ]
     },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Text Processing :: Linguistic",
         "License :: OSI Approved :: Apache Software License",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     keywords="home assistant intent recognition",
 )
```

### Comparing `hassil-1.2.1/tests/test_expression.py` & `hassil-1.2.2/tests/test_expression.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.1/tests/test_intents.py` & `hassil-1.2.2/tests/test_intents.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.1/tests/test_parser.py` & `hassil-1.2.2/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.1/tests/test_recognize.py` & `hassil-1.2.2/tests/test_recognize.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import cast
 
 import pytest
 
 from hassil import Intents, recognize, recognize_all
 from hassil.expression import TextChunk
 from hassil.intents import TextSlotList
-from hassil.recognize import UnmatchedRangeEntity, UnmatchedTextEntity
+from hassil.recognize import MISSING_ENTITY, UnmatchedRangeEntity, UnmatchedTextEntity
 
 TEST_YAML = """
 language: "en"
 intents:
   TurnOnTV:
     data:
       - sentences:
@@ -582,14 +582,146 @@
     assert set(result.unmatched_entities.keys()) == {"percent"}
 
     percent = result.unmatched_entities["percent"]
     assert isinstance(percent, UnmatchedTextEntity)
     assert percent.text == "fifty"
 
 
+def test_no_empty_unmatched_entity() -> None:
+    """Test that unmatched entities are not empty."""
+    yaml_text = """
+    language: "en"
+    intents:
+      Test:
+        data:
+          - sentences:
+              - "turn on {name}"
+              - "illuminate all[ {area}] lights"
+    lists:
+      name:
+        values:
+          - light
+      area:
+        values:
+          - bedroom
+    """
+
+    with io.StringIO(yaml_text) as test_file:
+        intents = Intents.from_yaml(test_file)
+
+    sentence = "turn on "
+    results = list(recognize_all(sentence, intents, allow_unmatched_entities=True))
+    assert not results, f"{sentence} should not match"
+
+    sentence = "illuminate all lights"
+    results = list(recognize_all(sentence, intents, allow_unmatched_entities=True))
+    assert results, f"{sentence} should match"
+    assert len(results) == 1, "Only 1 result expected"
+    assert not results[0].unmatched_entities, "No unmatched entities expected"
+
+    sentence = "illuminate all kitchen lights"
+    results = list(recognize_all(sentence, intents, allow_unmatched_entities=True))
+    assert results, f"{sentence} should match"
+    assert len(results) == 1, "Only 1 result expected"
+    result = results[0]
+    assert set(result.unmatched_entities.keys()) == {"area"}
+    area = result.unmatched_entities["area"]
+    assert isinstance(area, UnmatchedTextEntity)
+    assert area.text == "kitchen "
+
+
+def test_unmatched_entity_context() -> None:
+    """Test that unmatched entities work with requires/excludes context."""
+    yaml_text = """
+    language: "en"
+    intents:
+      Test:
+        data:
+          - sentences:
+              - "open {name}"
+            requires_context:
+              domain: cover
+    lists:
+      name:
+        values:
+          - garage door
+    """
+
+    with io.StringIO(yaml_text) as test_file:
+        intents = Intents.from_yaml(test_file)
+
+    sentence = "open garage door"
+
+    # Should fail when unmatched entities aren't allowed
+    result = recognize(sentence, intents, allow_unmatched_entities=False)
+    assert result is None, f"{sentence} should not match"
+
+    # Should succeed now with an unmatched domain entity
+    result = recognize(sentence, intents, allow_unmatched_entities=True)
+    assert result is not None, f"{sentence} should match"
+    assert set(result.unmatched_entities.keys()) == {"domain"}
+    domain = result.unmatched_entities["domain"]
+    assert isinstance(domain, UnmatchedTextEntity)
+    assert domain.text == MISSING_ENTITY
+
+    # Now both entities are unmatched
+    sentence = "open back door"
+    result = recognize(sentence, intents, allow_unmatched_entities=True)
+    assert result is not None, f"{sentence} should match"
+    assert set(result.unmatched_entities.keys()) == {"domain", "name"}
+
+    domain = result.unmatched_entities["domain"]
+    assert isinstance(domain, UnmatchedTextEntity)
+    assert domain.text == MISSING_ENTITY
+
+    name = result.unmatched_entities["name"]
+    assert isinstance(name, UnmatchedTextEntity)
+    assert name.text == "back door"
+
+
+def test_unmatched_slot_name() -> None:
+    """Test that unmatched entities use slot name instead of list name."""
+    yaml_text = """
+    language: "en"
+    intents:
+      Test:
+        data:
+          - sentences:
+              - "run {script_name:name}"
+              - "execute script {script_number:number}"
+    lists:
+      script_name:
+        values:
+          - stealth mode
+      script_number:
+        range:
+          from: 1
+          to: 100
+    """
+
+    with io.StringIO(yaml_text) as test_file:
+        intents = Intents.from_yaml(test_file)
+
+    sentence = "run missing name"
+    result = recognize(sentence, intents, allow_unmatched_entities=True)
+    assert result is not None, f"{sentence} should match"
+    assert set(result.unmatched_entities.keys()) == {"name"}
+
+    sentence = "execute script wrong number"
+    result = recognize(sentence, intents, allow_unmatched_entities=True)
+    assert result is not None, f"{sentence} should match"
+    assert set(result.unmatched_entities.keys()) == {"number"}
+
+    # Outside range
+    sentence = "execute script 0"
+    result = recognize(sentence, intents, allow_unmatched_entities=True)
+    assert result is not None, f"{sentence} should match"
+    assert set(result.unmatched_entities.keys()) == {"number"}
+
+
 def test_wildcard() -> None:
     """Test wildcard slot lists/entities."""
     yaml_text = """
     language: "en"
     intents:
       Test:
         data:
@@ -605,21 +737,82 @@
 
     with io.StringIO(yaml_text) as test_file:
         intents = Intents.from_yaml(test_file)
 
     sentence = "play the white album by the beatles please now"
     result = recognize(sentence, intents)
     assert result is not None, f"{sentence} should match"
+    assert set(result.entities.keys()) == {"album", "artist"}
     assert result.entities["album"].value == "the white album "
     assert result.entities["artist"].value == "the beatles "
 
     # Wildcards cannot be empty
     sentence = "play by please now"
     result = recognize(sentence, intents)
     assert result is None, f"{sentence} should not match"
 
     # Test without text at the end
     sentence = "start the white album by the beatles"
     result = recognize(sentence, intents)
     assert result is not None, f"{sentence} should match"
+    assert set(result.entities.keys()) == {"album", "artist"}
     assert result.entities["album"].value == "the white album "
     assert result.entities["artist"].value == "the beatles"
+
+
+def test_optional_wildcard() -> None:
+    """Test optional wildcard slot list."""
+    yaml_text = """
+    language: "en"
+    intents:
+      Test:
+        data:
+          - sentences:
+              - "play {album}[by {artist}]"
+    lists:
+      album:
+        wildcard: true
+      artist:
+        wildcard: true
+    """
+
+    with io.StringIO(yaml_text) as test_file:
+        intents = Intents.from_yaml(test_file)
+
+    # With all wildcards
+    sentence = "play the white album by the beatles"
+    result = recognize(sentence, intents)
+    assert result is not None, f"{sentence} should match"
+    assert set(result.entities.keys()) == {"album", "artist"}
+    assert result.entities["album"].value == "the white album "
+    assert result.entities["artist"].value == "the beatles"
+
+    # Missing one wildcard
+    sentence = "play the white album"
+    result = recognize(sentence, intents)
+    assert result is not None, f"{sentence} should match"
+    assert set(result.entities.keys()) == {"album"}
+    assert result.entities["album"].value == "the white album"
+
+
+def test_wildcard_slot_name() -> None:
+    """Test wildcard uses slot instead of list name."""
+    yaml_text = """
+    language: "en"
+    intents:
+      Test:
+        data:
+          - sentences:
+              - "run {script_name:name}"
+    lists:
+      script_name:
+        wildcard: true
+    """
+
+    with io.StringIO(yaml_text) as test_file:
+        intents = Intents.from_yaml(test_file)
+
+    sentence = "run script 1"
+    result = recognize(sentence, intents)
+    assert result is not None, f"{sentence} should match"
+    assert set(result.entities.keys()) == {"name"}
+    assert result.entities["name"].value == "script 1"
```

### Comparing `hassil-1.2.1/tests/test_sample.py` & `hassil-1.2.2/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `hassil-1.2.1/tests/test_util.py` & `hassil-1.2.2/tests/test_util.py`

 * *Files identical despite different names*

