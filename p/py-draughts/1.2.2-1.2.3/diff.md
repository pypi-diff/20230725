# Comparing `tmp/py-draughts-1.2.2.tar.gz` & `tmp/py-draughts-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-draughts-1.2.2.tar", last modified: Sun Jul 23 17:09:07 2023, max compression
+gzip compressed data, was "py-draughts-1.2.3.tar", last modified: Tue Jul 25 12:42:08 2023, max compression
```

## Comparing `py-draughts-1.2.2.tar` & `py-draughts-1.2.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 17:09:07.760854 py-draughts-1.2.2/
--rw-rw-rw-   0        0        0    35823 2023-07-11 12:53:30.000000 py-draughts-1.2.2/LICENSE
--rw-rw-rw-   0        0        0       43 2023-07-16 09:45:04.000000 py-draughts-1.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     5139 2023-07-23 17:09:07.759858 py-draughts-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3716 2023-07-21 15:00:24.000000 py-draughts-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-23 17:09:07.695814 py-draughts-1.2.2/draughts/
--rw-rw-rw-   0        0        0     1585 2023-07-23 17:08:58.000000 py-draughts-1.2.2/draughts/__init__.py
--rw-rw-rw-   0        0        0     3740 2023-07-21 17:07:24.000000 py-draughts-1.2.2/draughts/american.py
--rw-rw-rw-   0        0        0    14044 2023-07-23 11:21:41.000000 py-draughts-1.2.2/draughts/base.py
--rw-rw-rw-   0        0        0     3772 2023-07-23 17:08:13.000000 py-draughts-1.2.2/draughts/engine.py
--rw-rw-rw-   0        0        0      671 2023-07-16 18:11:48.000000 py-draughts-1.2.2/draughts/models.py
--rw-rw-rw-   0        0        0     4212 2023-07-23 17:05:13.000000 py-draughts-1.2.2/draughts/move.py
--rw-rw-rw-   0        0        0     5626 2023-07-23 17:05:33.000000 py-draughts-1.2.2/draughts/server.py
--rw-rw-rw-   0        0        0     8084 2023-07-23 11:21:41.000000 py-draughts-1.2.2/draughts/standard.py
-drwxrwxrwx   0        0        0        0 2023-07-23 17:09:07.635242 py-draughts-1.2.2/draughts/static/
-drwxrwxrwx   0        0        0        0 2023-07-23 17:09:07.702844 py-draughts-1.2.2/draughts/static/css/
--rw-rw-rw-   0        0        0     3873 2023-07-16 09:45:04.000000 py-draughts-1.2.2/draughts/static/css/style.css
-drwxrwxrwx   0        0        0        0 2023-07-23 17:09:07.717855 py-draughts-1.2.2/draughts/static/js/
--rw-rw-rw-   0        0        0     6250 2023-07-21 14:37:08.000000 py-draughts-1.2.2/draughts/static/js/script.js
-drwxrwxrwx   0        0        0        0 2023-07-23 17:09:07.720824 py-draughts-1.2.2/draughts/templates/
--rw-rw-rw-   0        0        0     1860 2023-07-11 16:32:17.000000 py-draughts-1.2.2/draughts/templates/base.html
--rw-rw-rw-   0        0        0     2882 2023-07-16 09:45:04.000000 py-draughts-1.2.2/draughts/templates/index.html
--rw-rw-rw-   0        0        0     1973 2023-07-16 10:59:23.000000 py-draughts-1.2.2/draughts/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-23 17:09:07.737854 py-draughts-1.2.2/py_draughts.egg-info/
--rw-rw-rw-   0        0        0     5139 2023-07-23 17:09:07.000000 py-draughts-1.2.2/py_draughts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      594 2023-07-23 17:09:07.000000 py-draughts-1.2.2/py_draughts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 17:09:07.000000 py-draughts-1.2.2/py_draughts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-23 17:09:07.000000 py-draughts-1.2.2/py_draughts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-23 17:09:07.000000 py-draughts-1.2.2/py_draughts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       48 2023-07-16 19:28:37.000000 py-draughts-1.2.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-23 17:09:07.760854 py-draughts-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1911 2023-07-18 21:34:49.000000 py-draughts-1.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-23 17:09:07.758854 py-draughts-1.2.2/test/
--rw-rw-rw-   0        0        0     1104 2023-07-16 18:39:54.000000 py-draughts-1.2.2/test/test_american_board.py
--rw-rw-rw-   0        0        0     2510 2023-07-23 11:21:41.000000 py-draughts-1.2.2/test/test_board.py
--rw-rw-rw-   0        0        0     1370 2023-07-23 11:21:41.000000 py-draughts-1.2.2/test/test_standard_board.py
+drwxrwxrwx   0        0        0        0 2023-07-25 12:42:08.384836 py-draughts-1.2.3/
+-rw-rw-rw-   0        0        0    35823 2023-07-11 12:53:30.000000 py-draughts-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0       43 2023-07-16 09:45:04.000000 py-draughts-1.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     5675 2023-07-25 12:42:08.382835 py-draughts-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4252 2023-07-25 12:41:49.000000 py-draughts-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 12:42:08.366838 py-draughts-1.2.3/draughts/
+-rw-rw-rw-   0        0        0     1585 2023-07-25 12:41:54.000000 py-draughts-1.2.3/draughts/__init__.py
+-rw-rw-rw-   0        0        0     3740 2023-07-21 17:07:24.000000 py-draughts-1.2.3/draughts/american.py
+-rw-rw-rw-   0        0        0    14036 2023-07-25 12:41:49.000000 py-draughts-1.2.3/draughts/base.py
+-rw-rw-rw-   0        0        0     3772 2023-07-23 17:08:13.000000 py-draughts-1.2.3/draughts/engine.py
+-rw-rw-rw-   0        0        0      671 2023-07-16 18:11:48.000000 py-draughts-1.2.3/draughts/models.py
+-rw-rw-rw-   0        0        0     4397 2023-07-25 12:41:49.000000 py-draughts-1.2.3/draughts/move.py
+-rw-rw-rw-   0        0        0     5449 2023-07-25 12:41:49.000000 py-draughts-1.2.3/draughts/server.py
+-rw-rw-rw-   0        0        0     8287 2023-07-25 12:41:49.000000 py-draughts-1.2.3/draughts/standard.py
+drwxrwxrwx   0        0        0        0 2023-07-25 12:42:08.340836 py-draughts-1.2.3/draughts/static/
+drwxrwxrwx   0        0        0        0 2023-07-25 12:42:08.367836 py-draughts-1.2.3/draughts/static/css/
+-rw-rw-rw-   0        0        0     3873 2023-07-16 09:45:04.000000 py-draughts-1.2.3/draughts/static/css/style.css
+drwxrwxrwx   0        0        0        0 2023-07-25 12:42:08.369834 py-draughts-1.2.3/draughts/static/js/
+-rw-rw-rw-   0        0        0     6250 2023-07-21 14:37:08.000000 py-draughts-1.2.3/draughts/static/js/script.js
+drwxrwxrwx   0        0        0        0 2023-07-25 12:42:08.372836 py-draughts-1.2.3/draughts/templates/
+-rw-rw-rw-   0        0        0     1860 2023-07-11 16:32:17.000000 py-draughts-1.2.3/draughts/templates/base.html
+-rw-rw-rw-   0        0        0     2882 2023-07-16 09:45:04.000000 py-draughts-1.2.3/draughts/templates/index.html
+-rw-rw-rw-   0        0        0     1973 2023-07-16 10:59:23.000000 py-draughts-1.2.3/draughts/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 12:42:08.378834 py-draughts-1.2.3/py_draughts.egg-info/
+-rw-rw-rw-   0        0        0     5675 2023-07-25 12:42:08.000000 py-draughts-1.2.3/py_draughts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      594 2023-07-25 12:42:08.000000 py-draughts-1.2.3/py_draughts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 12:42:08.000000 py-draughts-1.2.3/py_draughts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-25 12:42:08.000000 py-draughts-1.2.3/py_draughts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-25 12:42:08.000000 py-draughts-1.2.3/py_draughts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       48 2023-07-16 19:28:37.000000 py-draughts-1.2.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 12:42:08.384836 py-draughts-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1911 2023-07-18 21:34:49.000000 py-draughts-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 12:42:08.381835 py-draughts-1.2.3/test/
+-rw-rw-rw-   0        0        0     1104 2023-07-16 18:39:54.000000 py-draughts-1.2.3/test/test_american_board.py
+-rw-rw-rw-   0        0        0     2510 2023-07-23 11:21:41.000000 py-draughts-1.2.3/test/test_board.py
+-rw-rw-rw-   0        0        0     1370 2023-07-23 11:21:41.000000 py-draughts-1.2.3/test/test_standard_board.py
```

### Comparing `py-draughts-1.2.2/LICENSE` & `py-draughts-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py-draughts-1.2.2/PKG-INFO` & `py-draughts-1.2.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 1.2.2
+Version: 1.2.3
 Summary: A draughts library with advenced (customizable) WEB UI move generation and validation, PDN parsing and writing. Supports multiple variants of game.
 Home-page: https://github.com/michalskibinski109/py-draughts
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/py-draughts/index.html
 Keywords: draughts,checkers,AI mini-max,game,board
@@ -32,14 +32,15 @@
 [![GitHub Actions](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml/badge.svg)](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml)
 [![PyPI version](https://badge.fury.io/py/py-draughts.svg)](https://badge.fury.io/py/py-draughts)
 [![Downloads](https://static.pepy.tech/badge/py-draughts)](https://pepy.tech/project/py-draughts)
 
 Efficient modern and flexible implementation of the draughts game with a beautiful web interface. 
 Supports multiple variants of the game and allows playing against AI.
 
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/11e6be5e-0cfc-412c-ac0b-2b8e87a4f450" width="800" style="border-radius: 1%;">
 
 ## Installation
 
 ```bash
 pip install py-draughts
 ```
 
@@ -76,36 +77,48 @@
  w . w . w . w .
 
 ```
 
 - Make and undo moves
 
 ```python
->>> board.push_uci("37-32")
+>>> board.push_uci("31-27")
 >>> board.pop() # undo last move
-Move: 37->32
+Move: 31->27
+>>> board.turn
+Color.WHITE
 ```
 
 - detects draws and wins
 
 ```python
 >>> board.game_over
 False
 >>> board.is_threefold_repetition
 False
+>>> board.is_5_moves_rule
+False
+>>> board.is_16_moves_rule
+False
+>>> board.is_25_moves_rule
+False
+>>> board.is_draw
+False
 ```
+_Each variant has it's own specyfic rules._
+
 - Validate and generate moves
 
 ```python
->>> board.push_uci("10x42")
-Move: 37->32 is correct, but not legal in given position.
-Legal moves are: [Move: 28->37, Move: 31->22]
+>>> board.push_uci("31-22")
+ValueError: 31-22 is correct, but not legal in given position.
+Legal moves are: ['31-27', '31-26', '32-28', '32-27', '33-29', '33-28', '34-30', '34-29', '35-30']
 
 >>> list(board.legal_moves)
-[Move: 28->37, Move: 31->22]
+['31-27', '31-26', '32-28', '32-27', '33-29', '33-28', '34-30', '34-29', '35-30']
 ```
 
 - Reads and writes fen strings
 
 ```python
 >>> board = get_board('standard', "W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32")
 >>> board.fen
@@ -135,14 +148,16 @@
 
 
 _Example with simplest possible engine._
 
 
 
 ```python
+>>> from draughts.server import Server
+>>> import numpy as np
 >>> get_best_mv = lambda board: np.random.choice(list(board.legal_moves))
 >>> server = Server(get_best_move_method=get_best_mv)
 >>> server.run()
 INFO:     Started server process [1617]
 INFO:     Waiting for application startup.
 INFO:     Application startup complete.
 INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
```

### Comparing `py-draughts-1.2.2/README.md` & `py-draughts-1.2.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 [![GitHub Actions](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml/badge.svg)](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml)
 [![PyPI version](https://badge.fury.io/py/py-draughts.svg)](https://badge.fury.io/py/py-draughts)
 [![Downloads](https://static.pepy.tech/badge/py-draughts)](https://pepy.tech/project/py-draughts)
 
 Efficient modern and flexible implementation of the draughts game with a beautiful web interface. 
 Supports multiple variants of the game and allows playing against AI.
 
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/11e6be5e-0cfc-412c-ac0b-2b8e87a4f450" width="800" style="border-radius: 1%;">
 
 ## Installation
 
 ```bash
 pip install py-draughts
 ```
 
@@ -47,36 +48,48 @@
  w . w . w . w .
 
 ```
 
 - Make and undo moves
 
 ```python
->>> board.push_uci("37-32")
+>>> board.push_uci("31-27")
 >>> board.pop() # undo last move
-Move: 37->32
+Move: 31->27
+>>> board.turn
+Color.WHITE
 ```
 
 - detects draws and wins
 
 ```python
 >>> board.game_over
 False
 >>> board.is_threefold_repetition
 False
+>>> board.is_5_moves_rule
+False
+>>> board.is_16_moves_rule
+False
+>>> board.is_25_moves_rule
+False
+>>> board.is_draw
+False
 ```
+_Each variant has it's own specyfic rules._
+
 - Validate and generate moves
 
 ```python
->>> board.push_uci("10x42")
-Move: 37->32 is correct, but not legal in given position.
-Legal moves are: [Move: 28->37, Move: 31->22]
+>>> board.push_uci("31-22")
+ValueError: 31-22 is correct, but not legal in given position.
+Legal moves are: ['31-27', '31-26', '32-28', '32-27', '33-29', '33-28', '34-30', '34-29', '35-30']
 
 >>> list(board.legal_moves)
-[Move: 28->37, Move: 31->22]
+['31-27', '31-26', '32-28', '32-27', '33-29', '33-28', '34-30', '34-29', '35-30']
 ```
 
 - Reads and writes fen strings
 
 ```python
 >>> board = get_board('standard', "W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32")
 >>> board.fen
@@ -106,14 +119,16 @@
 
 
 _Example with simplest possible engine._
 
 
 
 ```python
+>>> from draughts.server import Server
+>>> import numpy as np
 >>> get_best_mv = lambda board: np.random.choice(list(board.legal_moves))
 >>> server = Server(get_best_move_method=get_best_mv)
 >>> server.run()
 INFO:     Started server process [1617]
 INFO:     Waiting for application startup.
 INFO:     Application startup complete.
 INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
```

### Comparing `py-draughts-1.2.2/draughts/__init__.py` & `py-draughts-1.2.3/draughts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 """
 A draughts library with advenced (customizable) WEB UI move generation and validation,
 PDN parsing and writing. Supports multiple variants of game.
 """
 
 from typing import Literal
 
-__version__ = "1.2.2"
+__version__ = "1.2.3"
 __author__ = "Michał Skibiński"
 
 
 def get_board(variant: Literal["standard", "american"], fen: str = None):
     """
     Board factory method.
     - ``standard`` - standard draughts board
```

### Comparing `py-draughts-1.2.2/draughts/american.py` & `py-draughts-1.2.3/draughts/american.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.2.2/draughts/base.py` & `py-draughts-1.2.3/draughts/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,16 +124,16 @@
         super().__init__()
         self._pos = (
             starting_position
             if starting_position is not None
             else self.STARTING_POSITION
         )
         self.turn = turn if turn is not None else self.STARTING_COLOR
-        size = int(np.sqrt(len(self.position) * 2))
-        if size**2 != len(self.position) * 2:
+        size = int(np.sqrt(len(self._pos) * 2))
+        if size**2 != len(self._pos) * 2:
             msg = f"Invalid board with shape {self._pos.shape} provided.\
                 Please use an array with lenght = (n * n/2). \
                 Where n is an size of the board."
             logger.error(msg)
             raise ValueError(msg)
         self.shape = (size, size)
         self._moves_stack: list[Move] = []
```

### Comparing `py-draughts-1.2.2/draughts/engine.py` & `py-draughts-1.2.3/draughts/engine.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.2.2/draughts/models.py` & `py-draughts-1.2.3/draughts/models.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.2.2/draughts/move.py` & `py-draughts-1.2.3/draughts/move.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,14 +33,18 @@
     ) -> None:
         self.square_list = visited_squares
         self.captured_list = captured_list
         self.captured_entities = captured_entities
         self.is_promotion = is_promotion
         self.halfmove_clock = 0
 
+    def __str__(self) -> str:
+        separator = "x" if self.captured_list else "-"
+        return f"{self.square_list[0] + 1}{separator}{self.square_list[-1] + 1}"
+
     def __repr__(self) -> str:
         visited_squares = [str(s + 1) for s in self.square_list]
         return f"Move: {'->'.join(visited_squares)}"
 
     def __eq__(self, other: object) -> bool:
         """Check if two moves are equal. move created from string will have only visited squares definied."""
         if not isinstance(other, Move):
@@ -112,9 +116,9 @@
             raise ValueError(f"Invalid move {move}.")
 
         move = Move([int(step) - 1 for step in steps])
         for legal_move in legal_moves:
             if legal_move == move:
                 return legal_move
         raise ValueError(
-            f"{move} is correct, but not legal in given position.\n Legal moves are: {list(legal_moves)}"
+            f"{str(move)} is correct, but not legal in given position.\n Legal moves are: {list(map(str,legal_moves))}"
         )
```

### Comparing `py-draughts-1.2.2/draughts/server.py` & `py-draughts-1.2.3/draughts/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,20 +82,18 @@
         }
 
     @property
     def position_json(self) -> PositionResponse:
         history = []  # (numver, white, black)
         stack = self.board._moves_stack
         for idx in range(len(stack)):
-            src, tg = stack[idx].square_list[0] + 1, stack[idx].square_list[-1] + 1
-            separator = "-" if len(stack[idx].captured_list) == 0 else "x"
             if idx % 2 == 0:
-                history.append([(idx // 2) + 1, f"{src}{separator}{tg}"])
+                history.append([(idx // 2) + 1, str(stack[idx])])
             else:
-                history[-1].append(f"{src}{separator}{tg}")
+                history[-1].append(str(stack[idx]))
         turn = "white" if self.board.turn == Color.WHITE else "black"
         return PositionResponse(
             position=self.board.friendly_form.tolist(),
             history=history,
             turn=turn,
         )
```

### Comparing `py-draughts-1.2.2/draughts/standard.py` & `py-draughts-1.2.3/draughts/standard.py`

 * *Files 12% similar despite different names*

```diff
@@ -199,11 +199,18 @@
         if is_capture_mandatory:
             moves = [move for move in moves if len(move.captured_list) > 0]
         return moves
 
 
 if __name__ == "__main__":
     board = Board()
-
+    board.push_uci("31-22")
+    print(board.turn)
+    board.is_5_moves_rule
+    board.is_16_moves_rule
+    board.is_25_moves_rule
+    board.is_threefold_repetition
+    board.is_draw
+    board.turn
     # b = Board.from_fen("B:B:WG8,18,24,28,34,37,42,44,49:B2,10,12,15,25,26")
     # print(b)
     # Board.from_fen("W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32")
```

### Comparing `py-draughts-1.2.2/draughts/static/css/style.css` & `py-draughts-1.2.3/draughts/static/css/style.css`

 * *Files identical despite different names*

### Comparing `py-draughts-1.2.2/draughts/static/js/script.js` & `py-draughts-1.2.3/draughts/static/js/script.js`

 * *Files identical despite different names*

### Comparing `py-draughts-1.2.2/draughts/templates/base.html` & `py-draughts-1.2.3/draughts/templates/base.html`

 * *Files identical despite different names*

### Comparing `py-draughts-1.2.2/draughts/templates/index.html` & `py-draughts-1.2.3/draughts/templates/index.html`

 * *Files identical despite different names*

### Comparing `py-draughts-1.2.2/draughts/utils.py` & `py-draughts-1.2.3/draughts/utils.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.2.2/py_draughts.egg-info/PKG-INFO` & `py-draughts-1.2.3/py_draughts.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 1.2.2
+Version: 1.2.3
 Summary: A draughts library with advenced (customizable) WEB UI move generation and validation, PDN parsing and writing. Supports multiple variants of game.
 Home-page: https://github.com/michalskibinski109/py-draughts
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/py-draughts/index.html
 Keywords: draughts,checkers,AI mini-max,game,board
@@ -32,14 +32,15 @@
 [![GitHub Actions](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml/badge.svg)](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml)
 [![PyPI version](https://badge.fury.io/py/py-draughts.svg)](https://badge.fury.io/py/py-draughts)
 [![Downloads](https://static.pepy.tech/badge/py-draughts)](https://pepy.tech/project/py-draughts)
 
 Efficient modern and flexible implementation of the draughts game with a beautiful web interface. 
 Supports multiple variants of the game and allows playing against AI.
 
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/11e6be5e-0cfc-412c-ac0b-2b8e87a4f450" width="800" style="border-radius: 1%;">
 
 ## Installation
 
 ```bash
 pip install py-draughts
 ```
 
@@ -76,36 +77,48 @@
  w . w . w . w .
 
 ```
 
 - Make and undo moves
 
 ```python
->>> board.push_uci("37-32")
+>>> board.push_uci("31-27")
 >>> board.pop() # undo last move
-Move: 37->32
+Move: 31->27
+>>> board.turn
+Color.WHITE
 ```
 
 - detects draws and wins
 
 ```python
 >>> board.game_over
 False
 >>> board.is_threefold_repetition
 False
+>>> board.is_5_moves_rule
+False
+>>> board.is_16_moves_rule
+False
+>>> board.is_25_moves_rule
+False
+>>> board.is_draw
+False
 ```
+_Each variant has it's own specyfic rules._
+
 - Validate and generate moves
 
 ```python
->>> board.push_uci("10x42")
-Move: 37->32 is correct, but not legal in given position.
-Legal moves are: [Move: 28->37, Move: 31->22]
+>>> board.push_uci("31-22")
+ValueError: 31-22 is correct, but not legal in given position.
+Legal moves are: ['31-27', '31-26', '32-28', '32-27', '33-29', '33-28', '34-30', '34-29', '35-30']
 
 >>> list(board.legal_moves)
-[Move: 28->37, Move: 31->22]
+['31-27', '31-26', '32-28', '32-27', '33-29', '33-28', '34-30', '34-29', '35-30']
 ```
 
 - Reads and writes fen strings
 
 ```python
 >>> board = get_board('standard', "W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32")
 >>> board.fen
@@ -135,14 +148,16 @@
 
 
 _Example with simplest possible engine._
 
 
 
 ```python
+>>> from draughts.server import Server
+>>> import numpy as np
 >>> get_best_mv = lambda board: np.random.choice(list(board.legal_moves))
 >>> server = Server(get_best_move_method=get_best_mv)
 >>> server.run()
 INFO:     Started server process [1617]
 INFO:     Waiting for application startup.
 INFO:     Application startup complete.
 INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
```

### Comparing `py-draughts-1.2.2/py_draughts.egg-info/SOURCES.txt` & `py-draughts-1.2.3/py_draughts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-draughts-1.2.2/setup.py` & `py-draughts-1.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.2.2/test/test_american_board.py` & `py-draughts-1.2.3/test/test_american_board.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.2.2/test/test_board.py` & `py-draughts-1.2.3/test/test_board.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.2.2/test/test_standard_board.py` & `py-draughts-1.2.3/test/test_standard_board.py`

 * *Files identical despite different names*

