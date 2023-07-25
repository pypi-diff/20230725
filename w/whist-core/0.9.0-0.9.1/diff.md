# Comparing `tmp/whist_core-0.9.0.tar.gz` & `tmp/whist_core-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whist_core-0.9.0.tar", max compression
+gzip compressed data, was "whist_core-0.9.1.tar", max compression
```

## Comparing `whist_core-0.9.0.tar` & `whist_core-0.9.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1067 2023-07-21 22:47:28.479875 whist_core-0.9.0/LICENSE
--rw-r--r--   0        0        0     1359 2023-07-21 22:47:28.479875 whist_core-0.9.0/README.md
--rw-r--r--   0        0        0      884 2023-07-21 22:47:28.479875 whist_core-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      232 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/__init__.py
--rw-r--r--   0        0        0       34 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/cards/__init__.py
--rw-r--r--   0        0        0     3720 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/cards/card.py
--rw-r--r--   0        0        0     6837 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/cards/card_container.py
--rw-r--r--   0        0        0       23 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/error/__init__.py
--rw-r--r--   0        0        0      182 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/error/matcher_error.py
--rw-r--r--   0        0        0      179 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/error/player_error.py
--rw-r--r--   0        0        0      734 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/error/table_error.py
--rw-r--r--   0        0        0       22 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/game/__init__.py
--rw-r--r--   0        0        0     1432 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/game/errors.py
--rw-r--r--   0        0        0     2187 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/game/game.py
--rw-r--r--   0        0        0     3428 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/game/hand.py
--rw-r--r--   0        0        0      888 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/game/legal_checker.py
--rw-r--r--   0        0        0     3585 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/game/play_order.py
--rw-r--r--   0        0        0      649 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/game/player_at_table.py
--rw-r--r--   0        0        0     1397 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/game/rubber.py
--rw-r--r--   0        0        0     2608 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/game/trick.py
--rw-r--r--   0        0        0      205 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/game/warnings.py
--rw-r--r--   0        0        0       41 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/scoring/__init__.py
--rw-r--r--   0        0        0     1734 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/scoring/elo.py
--rw-r--r--   0        0        0     1228 2023-07-21 22:47:28.483875 whist_core-0.9.0/whist_core/scoring/score.py
--rw-r--r--   0        0        0     1330 2023-07-21 22:47:28.483875 whist_core-0.9.0/whist_core/scoring/score_calculator.py
--rw-r--r--   0        0        0     2168 2023-07-21 22:47:28.483875 whist_core-0.9.0/whist_core/scoring/score_card.py
--rw-r--r--   0        0        0      910 2023-07-21 22:47:28.483875 whist_core-0.9.0/whist_core/scoring/team.py
--rw-r--r--   0        0        0       42 2023-07-21 22:47:28.483875 whist_core-0.9.0/whist_core/session/__init__.py
--rw-r--r--   0        0        0      951 2023-07-21 22:47:28.483875 whist_core-0.9.0/whist_core/session/distribution.py
--rw-r--r--   0        0        0     3534 2023-07-21 22:47:28.483875 whist_core-0.9.0/whist_core/session/matcher.py
--rw-r--r--   0        0        0      240 2023-07-21 22:47:28.483875 whist_core-0.9.0/whist_core/session/session.py
--rw-r--r--   0        0        0     6577 2023-07-21 22:47:28.483875 whist_core-0.9.0/whist_core/session/table.py
--rw-r--r--   0        0        0     5322 2023-07-21 22:47:28.483875 whist_core-0.9.0/whist_core/session/userlist.py
--rw-r--r--   0        0        0       37 2023-07-21 22:47:28.483875 whist_core-0.9.0/whist_core/user/__init__.py
--rw-r--r--   0        0        0     1698 2023-07-21 22:47:28.483875 whist_core-0.9.0/whist_core/user/player.py
--rw-r--r--   0        0        0      280 2023-07-21 22:47:28.483875 whist_core-0.9.0/whist_core/user/status.py
--rw-r--r--   0        0        0      156 2023-07-21 22:47:28.483875 whist_core-0.9.0/whist_core/user/user.py
--rw-r--r--   0        0        0      564 2023-07-21 22:47:28.483875 whist_core-0.9.0/whist_core/util.py
--rw-r--r--   0        0        0     2206 1970-01-01 00:00:00.000000 whist_core-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-25 10:42:07.935218 whist_core-0.9.1/LICENSE
+-rw-r--r--   0        0        0     1359 2023-07-25 10:42:07.935218 whist_core-0.9.1/README.md
+-rw-r--r--   0        0        0      875 2023-07-25 10:42:07.935218 whist_core-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      232 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/__init__.py
+-rw-r--r--   0        0        0       34 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/cards/__init__.py
+-rw-r--r--   0        0        0     4066 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/cards/card.py
+-rw-r--r--   0        0        0     6837 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/cards/card_container.py
+-rw-r--r--   0        0        0       23 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/error/__init__.py
+-rw-r--r--   0        0        0      182 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/error/matcher_error.py
+-rw-r--r--   0        0        0      179 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/error/player_error.py
+-rw-r--r--   0        0        0      734 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/error/table_error.py
+-rw-r--r--   0        0        0       22 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/game/__init__.py
+-rw-r--r--   0        0        0     1432 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/game/errors.py
+-rw-r--r--   0        0        0     2187 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/game/game.py
+-rw-r--r--   0        0        0     3428 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/game/hand.py
+-rw-r--r--   0        0        0      888 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/game/legal_checker.py
+-rw-r--r--   0        0        0     3585 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/game/play_order.py
+-rw-r--r--   0        0        0      649 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/game/player_at_table.py
+-rw-r--r--   0        0        0     1397 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/game/rubber.py
+-rw-r--r--   0        0        0     2608 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/game/trick.py
+-rw-r--r--   0        0        0      205 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/game/warnings.py
+-rw-r--r--   0        0        0       41 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/scoring/__init__.py
+-rw-r--r--   0        0        0     1734 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/scoring/elo.py
+-rw-r--r--   0        0        0     1228 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/scoring/score.py
+-rw-r--r--   0        0        0     1330 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/scoring/score_calculator.py
+-rw-r--r--   0        0        0     2168 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/scoring/score_card.py
+-rw-r--r--   0        0        0      910 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/scoring/team.py
+-rw-r--r--   0        0        0       42 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/session/__init__.py
+-rw-r--r--   0        0        0      951 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/session/distribution.py
+-rw-r--r--   0        0        0     3534 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/session/matcher.py
+-rw-r--r--   0        0        0      240 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/session/session.py
+-rw-r--r--   0        0        0     6577 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/session/table.py
+-rw-r--r--   0        0        0     5322 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/session/userlist.py
+-rw-r--r--   0        0        0       37 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/user/__init__.py
+-rw-r--r--   0        0        0     1698 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/user/player.py
+-rw-r--r--   0        0        0      280 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/user/status.py
+-rw-r--r--   0        0        0      156 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/user/user.py
+-rw-r--r--   0        0        0      564 2023-07-25 10:42:07.935218 whist_core-0.9.1/whist_core/util.py
+-rw-r--r--   0        0        0     2201 1970-01-01 00:00:00.000000 whist_core-0.9.1/PKG-INFO
```

### Comparing `whist_core-0.9.0/LICENSE` & `whist_core-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `whist_core-0.9.0/README.md` & `whist_core-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `whist_core-0.9.0/pyproject.toml` & `whist_core-0.9.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "whist-core"
 # remember to also update the version in __init__.py!
-version = "0.9.0"
+version = "0.9.1"
 description = "Whist rules implementation"
 authors = ["Whist-Team"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Whist-Team/Whist-Core"
 repository = "https://github.com/Whist-Team/Whist-Core"
 documentation = "https://whist-core.readthedocs.io"
@@ -15,16 +15,16 @@
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/Whist-Team/Whist-Core/issues"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pydantic = ">=1.10,<3.0"
-deprecation = "^2.1.0"
+pydantic = "^2.0"
+deprecation = "^2.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.4"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.21"
 flake8 = "^6.0"
 flake8-docstrings = "^1.7"
```

### Comparing `whist_core-0.9.0/whist_core/cards/card.py` & `whist_core-0.9.1/whist_core/cards/card.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Card related classes"""
 
 from enum import Enum
 from functools import total_ordering
 from typing import Any, Optional, Iterator
 
+import deprecation
 from pydantic import BaseModel
 
 from whist_core.util import enforce_str_on_dict
 
 
 @total_ordering
 class _CardEnum(Enum):
@@ -131,21 +132,29 @@
         """
         Get the name of this card.
 
         :return: name
         """
         return f'{self.rank} of {self.suit}'
 
+    @deprecation.deprecated("Use model_dump instead. Will be removed in V1.")
     def dict(self, *args, **kwargs):
         """
         Returns the dictionary. See BaseModel for details.
         """
         super_dict = super().model_dump(*args, **kwargs)
         return enforce_str_on_dict(super_dict, ('suit', 'rank'))
 
+    def model_dump(self, *args, **kwargs):
+        """
+        Returns the dictionary. See BaseModel for details.
+        """
+        super_dict = super().model_dump(*args, **kwargs)
+        return enforce_str_on_dict(super_dict, ('suit', 'rank'))
+
     def __lt__(self, other: Any) -> bool:
         """Checks if the other card is lower than this card."""
         if self.__class__ is other.__class__:
             return (self.suit, self.rank) < (other.suit, other.rank)
         return NotImplemented
 
     def __str__(self) -> str:
```

### Comparing `whist_core-0.9.0/whist_core/cards/card_container.py` & `whist_core-0.9.1/whist_core/cards/card_container.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.9.0/whist_core/error/table_error.py` & `whist_core-0.9.1/whist_core/error/table_error.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.9.0/whist_core/game/errors.py` & `whist_core-0.9.1/whist_core/game/errors.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.9.0/whist_core/game/game.py` & `whist_core-0.9.1/whist_core/game/game.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.9.0/whist_core/game/hand.py` & `whist_core-0.9.1/whist_core/game/hand.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.9.0/whist_core/game/legal_checker.py` & `whist_core-0.9.1/whist_core/game/legal_checker.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.9.0/whist_core/game/play_order.py` & `whist_core-0.9.1/whist_core/game/play_order.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.9.0/whist_core/game/player_at_table.py` & `whist_core-0.9.1/whist_core/game/player_at_table.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.9.0/whist_core/game/rubber.py` & `whist_core-0.9.1/whist_core/game/rubber.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.9.0/whist_core/game/trick.py` & `whist_core-0.9.1/whist_core/game/trick.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.9.0/whist_core/scoring/elo.py` & `whist_core-0.9.1/whist_core/scoring/elo.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.9.0/whist_core/scoring/score.py` & `whist_core-0.9.1/whist_core/scoring/score.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.9.0/whist_core/scoring/score_calculator.py` & `whist_core-0.9.1/whist_core/scoring/score_calculator.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.9.0/whist_core/scoring/score_card.py` & `whist_core-0.9.1/whist_core/scoring/score_card.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.9.0/whist_core/scoring/team.py` & `whist_core-0.9.1/whist_core/scoring/team.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.9.0/whist_core/session/distribution.py` & `whist_core-0.9.1/whist_core/session/distribution.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.9.0/whist_core/session/matcher.py` & `whist_core-0.9.1/whist_core/session/matcher.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.9.0/whist_core/session/table.py` & `whist_core-0.9.1/whist_core/session/table.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.9.0/whist_core/session/userlist.py` & `whist_core-0.9.1/whist_core/session/userlist.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.9.0/whist_core/user/player.py` & `whist_core-0.9.1/whist_core/user/player.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.9.0/whist_core/util.py` & `whist_core-0.9.1/whist_core/util.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.9.0/PKG-INFO` & `whist_core-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: whist-core
-Version: 0.9.0
+Version: 0.9.1
 Summary: Whist rules implementation
 Home-page: https://github.com/Whist-Team/Whist-Core
 License: MIT
 Keywords: game,whist
 Author: Whist-Team
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: deprecation (>=2.1.0,<3.0.0)
-Requires-Dist: pydantic (>=1.10,<3.0)
+Requires-Dist: deprecation (>=2.1,<3.0)
+Requires-Dist: pydantic (>=2.0,<3.0)
 Project-URL: Bug Tracker, https://github.com/Whist-Team/Whist-Core/issues
 Project-URL: Documentation, https://whist-core.readthedocs.io
 Project-URL: Repository, https://github.com/Whist-Team/Whist-Core
 Description-Content-Type: text/markdown
 
 [![Documentation Status](https://readthedocs.org/projects/pip/badge/?version=stable)](https://whist-core.readthedocs.io/en/latest/)
 [![codecov](https://codecov.io/gh/Whist-Team/Whist-Core/branch/main/graph/badge.svg)](https://codecov.io/gh/Whist-Team/Whist-Core)
```

