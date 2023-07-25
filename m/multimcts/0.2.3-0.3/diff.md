# Comparing `tmp/multimcts-0.2.3.tar.gz` & `tmp/multimcts-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multimcts-0.2.3.tar", max compression
+gzip compressed data, was "multimcts-0.3.tar", last modified: Tue Jul 25 18:33:20 2023, max compression
```

## Comparing `multimcts-0.2.3.tar` & `multimcts-0.3.tar`

### file list

```diff
@@ -1,7 +1,16 @@
--rw-r--r--   0        0        0     1069 2023-07-24 15:25:58.278450 multimcts-0.2.3/LICENSE
--rw-r--r--   0        0        0     1631 2023-07-24 18:26:24.283727 multimcts-0.2.3/README.md
--rw-r--r--   0        0        0       34 2023-07-17 20:09:40.000000 multimcts-0.2.3/multimcts/__init__.py
--rwxr-xr-x   0        0        0   327190 2023-07-24 19:45:06.000000 multimcts-0.2.3/multimcts/mcts.cpython-39-darwin.so
--rw-r--r--   0        0        0     9693 2023-07-24 19:46:18.110361 multimcts-0.2.3/multimcts/mcts.pyx
--rw-r--r--   0        0        0      462 2023-07-25 01:11:42.084497 multimcts-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2185 1970-01-01 00:00:00.000000 multimcts-0.2.3/PKG-INFO
+drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-25 18:33:20.536037 multimcts-0.3/
+-rw-r--r--   0 taylorvance   (501) staff       (20)     1069 2023-07-24 15:25:58.000000 multimcts-0.3/LICENSE
+-rw-r--r--   0 taylorvance   (501) staff       (20)     2770 2023-07-25 18:33:20.535903 multimcts-0.3/PKG-INFO
+-rw-r--r--   0 taylorvance   (501) staff       (20)     2489 2023-07-25 16:42:00.000000 multimcts-0.3/README.md
+drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-25 18:33:20.535197 multimcts-0.3/multimcts/
+-rw-r--r--   0 taylorvance   (501) staff       (20)       34 2023-07-17 20:09:40.000000 multimcts-0.3/multimcts/__init__.py
+-rw-r--r--   0 taylorvance   (501) staff       (20)   430223 2023-07-25 17:39:23.000000 multimcts-0.3/multimcts/mcts.c
+-rw-r--r--   0 taylorvance   (501) staff       (20)     9693 2023-07-24 19:46:18.000000 multimcts-0.3/multimcts/mcts.pyx
+drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-25 18:33:20.535714 multimcts-0.3/multimcts.egg-info/
+-rw-r--r--   0 taylorvance   (501) staff       (20)     2770 2023-07-25 18:33:20.000000 multimcts-0.3/multimcts.egg-info/PKG-INFO
+-rw-r--r--   0 taylorvance   (501) staff       (20)      231 2023-07-25 18:33:20.000000 multimcts-0.3/multimcts.egg-info/SOURCES.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)        1 2023-07-25 18:33:20.000000 multimcts-0.3/multimcts.egg-info/dependency_links.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)       10 2023-07-25 18:33:20.000000 multimcts-0.3/multimcts.egg-info/top_level.txt
+-rw-r--r--   0 taylorvance   (501) staff       (20)      100 2023-07-25 16:22:07.000000 multimcts-0.3/pyproject.toml
+-rw-r--r--   0 taylorvance   (501) staff       (20)       38 2023-07-25 18:33:20.536083 multimcts-0.3/setup.cfg
+-rw-r--r--   0 taylorvance   (501) staff       (20)      565 2023-07-25 18:33:14.000000 multimcts-0.3/setup.py
```

### Comparing `multimcts-0.2.3/LICENSE` & `multimcts-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `multimcts-0.2.3/README.md` & `multimcts-0.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,75 @@
 # MultiMCTS
 
-MultiMCTS is a Python package that implements the [Monte Carlo Tree Search](https://wikipedia.org/wiki/Monte_Carlo_tree_search) algorithm for board games played by any number of players. With MultiMCTS, you can create AI for any board game *merely by knowing the rules* -- no strategy needed!
+MultiMCTS is a Python package that implements the [Monte Carlo Tree Search](https://wikipedia.org/wiki/Monte_Carlo_tree_search) algorithm for board games played by any number of players. With MultiMCTS, you can create AI for any game *merely by knowing the rules* -- **no strategy needed!**
+
 
 ## Features
 
-- Efficient (largely C-compiled) MCTS implementation
+- Efficient MCTS implementation
 - Support for any number of players/teams
 - Easily create AI for any board game
 
+
 ## Game Implementation
 
 ### For your game, you will need to:
 - Represent the game state in code
 - Identify all legal moves
 - Determine if the game is over and who won
 
 ### You do NOT need to:
+- Understand strategy
 - Have domain knowledge
-- Understand any strategy
 - Evaluate the favorability of a game state
 
+
+## Installation
+
+```bash
+pip install multimcts
+```
+
+
 ## Usage
 
 To use MultiMCTS, you must define your game by subclassing `GameState` and implementing the required methods (see [examples](https://github.com/taylorvance/multimcts/blob/main/examples/README.md)):
-- get_current_team
-- get_legal_moves
-- make_move
-- is_terminal
-- get_reward
+- `get_current_team` -- Returns the current team.
+- `get_legal_moves` -- Returns a list of legal moves. Moves can be any data structure.
+- `make_move` -- Returns a copy of the current state after performing the given move (one from get_legal_moves).
+- `is_terminal` -- Returns whether the game is over.
+- `get_reward` -- Returns the reward given to the team that played the game-ending move.
 
 ```python
 from multimcts import MCTS, GameState
 
 class MyGameState(GameState):
     # your implementation here...
+    pass
 
 mcts = MCTS()                               # Create an MCTS agent.
 state = MyGameState()                       # Set up a new game.
 
 while not state.is_terminal():              # Continue until the game is over.
     print(state)                            # Print the current game state (implementing GameState.__repr__ might be helpful).
-    state = mcts.search(state, max_time=1)  # Play the best move found.
+    state = mcts.search(state, max_time=1)  # Play the best move found after 1 second.
 
 print(state)                                # Print the final game state.
 ```
+
+
+### Development
+
+1. Clone the MultiMCTS repo.
+    ```bash
+    git clone https://github.com/taylorvance/multimcts.git
+    cd multimcts/
+    ```
+1. Make changes to `multimcts/mcts.pyx` or other files. Then build a distribution.
+    ```bash
+    python setup.py sdist
+    ```
+1. Install the updated package to use in your projects.
+    ```bash
+    pip install dist/multimcts-0.1.0.tar.gz
+    ```
+    Replace `multimcts-0.1.0` with the actual filename and version from the `dist/` directory.
```

### Comparing `multimcts-0.2.3/multimcts/mcts.pyx` & `multimcts-0.3/multimcts/mcts.pyx`

 * *Files identical despite different names*

### Comparing `multimcts-0.2.3/PKG-INFO` & `multimcts-0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,89 @@
 Metadata-Version: 2.1
 Name: multimcts
-Version: 0.2.3
+Version: 0.3
 Summary: Monte Carlo Tree Search for multiple teams
-Home-page: https://github.com/taylorvance/multimcts
-License: MIT
+Home-page: UNKNOWN
 Author: Taylor Vance
 Author-email: mirrors.cities0w@icloud.com
-Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+License: MIT
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # MultiMCTS
 
-MultiMCTS is a Python package that implements the [Monte Carlo Tree Search](https://wikipedia.org/wiki/Monte_Carlo_tree_search) algorithm for board games played by any number of players. With MultiMCTS, you can create AI for any board game *merely by knowing the rules* -- no strategy needed!
+MultiMCTS is a Python package that implements the [Monte Carlo Tree Search](https://wikipedia.org/wiki/Monte_Carlo_tree_search) algorithm for board games played by any number of players. With MultiMCTS, you can create AI for any game *merely by knowing the rules* -- **no strategy needed!**
+
 
 ## Features
 
-- Efficient (largely C-compiled) MCTS implementation
+- Efficient MCTS implementation
 - Support for any number of players/teams
 - Easily create AI for any board game
 
+
 ## Game Implementation
 
 ### For your game, you will need to:
 - Represent the game state in code
 - Identify all legal moves
 - Determine if the game is over and who won
 
 ### You do NOT need to:
+- Understand strategy
 - Have domain knowledge
-- Understand any strategy
 - Evaluate the favorability of a game state
 
+
+## Installation
+
+```bash
+pip install multimcts
+```
+
+
 ## Usage
 
 To use MultiMCTS, you must define your game by subclassing `GameState` and implementing the required methods (see [examples](https://github.com/taylorvance/multimcts/blob/main/examples/README.md)):
-- get_current_team
-- get_legal_moves
-- make_move
-- is_terminal
-- get_reward
+- `get_current_team` -- Returns the current team.
+- `get_legal_moves` -- Returns a list of legal moves. Moves can be any data structure.
+- `make_move` -- Returns a copy of the current state after performing the given move (one from get_legal_moves).
+- `is_terminal` -- Returns whether the game is over.
+- `get_reward` -- Returns the reward given to the team that played the game-ending move.
 
 ```python
 from multimcts import MCTS, GameState
 
 class MyGameState(GameState):
     # your implementation here...
+    pass
 
 mcts = MCTS()                               # Create an MCTS agent.
 state = MyGameState()                       # Set up a new game.
 
 while not state.is_terminal():              # Continue until the game is over.
     print(state)                            # Print the current game state (implementing GameState.__repr__ might be helpful).
-    state = mcts.search(state, max_time=1)  # Play the best move found.
+    state = mcts.search(state, max_time=1)  # Play the best move found after 1 second.
 
 print(state)                                # Print the final game state.
 ```
 
+
+### Development
+
+1. Clone the MultiMCTS repo.
+    ```bash
+    git clone https://github.com/taylorvance/multimcts.git
+    cd multimcts/
+    ```
+1. Make changes to `multimcts/mcts.pyx` or other files. Then build a distribution.
+    ```bash
+    python setup.py sdist
+    ```
+1. Install the updated package to use in your projects.
+    ```bash
+    pip install dist/multimcts-0.1.0.tar.gz
+    ```
+    Replace `multimcts-0.1.0` with the actual filename and version from the `dist/` directory.
+
+
```

