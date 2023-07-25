# Comparing `tmp/multimcts-0.2.2.tar.gz` & `tmp/multimcts-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multimcts-0.2.2.tar", last modified: Fri Jul 21 00:56:22 2023, max compression
+gzip compressed data, was "multimcts-0.2.3.tar", max compression
```

## Comparing `multimcts-0.2.2.tar` & `multimcts-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,7 @@
-drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-21 00:56:22.477183 multimcts-0.2.2/
--rw-r--r--   0 taylorvance   (501) staff       (20)       24 2023-07-17 19:47:43.000000 multimcts-0.2.2/MANIFEST.in
--rw-r--r--   0 taylorvance   (501) staff       (20)     2005 2023-07-21 00:56:22.477046 multimcts-0.2.2/PKG-INFO
--rw-r--r--   0 taylorvance   (501) staff       (20)     1711 2023-07-19 19:51:18.000000 multimcts-0.2.2/README.md
-drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-21 00:56:22.475889 multimcts-0.2.2/multimcts/
--rw-r--r--   0 taylorvance   (501) staff       (20)       34 2023-07-17 20:09:40.000000 multimcts-0.2.2/multimcts/__init__.py
--rw-r--r--   0 taylorvance   (501) staff       (20)   412842 2023-07-21 00:56:22.000000 multimcts-0.2.2/multimcts/mcts.c
--rw-r--r--   0 taylorvance   (501) staff       (20)     8809 2023-07-20 17:20:51.000000 multimcts-0.2.2/multimcts/mcts.pyx
-drwxr-xr-x   0 taylorvance   (501) staff       (20)        0 2023-07-21 00:56:22.476843 multimcts-0.2.2/multimcts.egg-info/
--rw-r--r--   0 taylorvance   (501) staff       (20)     2005 2023-07-21 00:56:22.000000 multimcts-0.2.2/multimcts.egg-info/PKG-INFO
--rw-r--r--   0 taylorvance   (501) staff       (20)      257 2023-07-17 23:05:38.000000 multimcts-0.2.2/multimcts.egg-info/SOURCES 2.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)      300 2023-07-21 00:56:22.000000 multimcts-0.2.2/multimcts.egg-info/SOURCES.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)        1 2023-07-21 00:56:22.000000 multimcts-0.2.2/multimcts.egg-info/dependency_links.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)        1 2023-07-17 19:12:04.000000 multimcts-0.2.2/multimcts.egg-info/not-zip-safe
--rw-r--r--   0 taylorvance   (501) staff       (20)       10 2023-07-21 00:56:22.000000 multimcts-0.2.2/multimcts.egg-info/top_level.txt
--rw-r--r--   0 taylorvance   (501) staff       (20)      100 2023-07-17 18:23:36.000000 multimcts-0.2.2/pyproject.toml
--rw-r--r--   0 taylorvance   (501) staff       (20)       38 2023-07-21 00:56:22.477229 multimcts-0.2.2/setup.cfg
--rw-r--r--   0 taylorvance   (501) staff       (20)      520 2023-07-20 01:24:59.000000 multimcts-0.2.2/setup.py
+-rw-r--r--   0        0        0     1069 2023-07-24 15:25:58.278450 multimcts-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1631 2023-07-24 18:26:24.283727 multimcts-0.2.3/README.md
+-rw-r--r--   0        0        0       34 2023-07-17 20:09:40.000000 multimcts-0.2.3/multimcts/__init__.py
+-rwxr-xr-x   0        0        0   327190 2023-07-24 19:45:06.000000 multimcts-0.2.3/multimcts/mcts.cpython-39-darwin.so
+-rw-r--r--   0        0        0     9693 2023-07-24 19:46:18.110361 multimcts-0.2.3/multimcts/mcts.pyx
+-rw-r--r--   0        0        0      462 2023-07-25 01:11:42.084497 multimcts-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2185 1970-01-01 00:00:00.000000 multimcts-0.2.3/PKG-INFO
```

### Comparing `multimcts-0.2.2/PKG-INFO` & `multimcts-0.2.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: multimcts
-Version: 0.2.2
-Summary: Monte Carlo Tree Search for multiple teams
-Home-page: https://github.com/taylorvance/multimcts
-Author: Taylor Vance
-Author-email: mirrors.cities0w@icloud.com
-License: MIT
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 # MultiMCTS
 
 MultiMCTS is a Python package that implements the [Monte Carlo Tree Search](https://wikipedia.org/wiki/Monte_Carlo_tree_search) algorithm for board games played by any number of players. With MultiMCTS, you can create AI for any board game *merely by knowing the rules* -- no strategy needed!
 
 ## Features
 
 - Efficient (largely C-compiled) MCTS implementation
@@ -29,15 +18,15 @@
 ### You do NOT need to:
 - Have domain knowledge
 - Understand any strategy
 - Evaluate the favorability of a game state
 
 ## Usage
 
-To use MultiMCTS, you must define your game by subclassing `GameState` and implementing the required methods (see [tictactoe.py](https://github.com/taylorvance/multimcts/blob/main/tests/tictactoe.py) for an example):
+To use MultiMCTS, you must define your game by subclassing `GameState` and implementing the required methods (see [examples](https://github.com/taylorvance/multimcts/blob/main/examples/README.md)):
 - get_current_team
 - get_legal_moves
 - make_move
 - is_terminal
 - get_reward
 
 ```python
@@ -51,13 +40,7 @@
 
 while not state.is_terminal():              # Continue until the game is over.
     print(state)                            # Print the current game state (implementing GameState.__repr__ might be helpful).
     state = mcts.search(state, max_time=1)  # Play the best move found.
 
 print(state)                                # Print the final game state.
 ```
-
-## License
-
-[MIT](https://choosealicense.com/licenses/mit/)
-
-
```

### Comparing `multimcts-0.2.2/README.md` & `multimcts-0.2.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: multimcts
+Version: 0.2.3
+Summary: Monte Carlo Tree Search for multiple teams
+Home-page: https://github.com/taylorvance/multimcts
+License: MIT
+Author: Taylor Vance
+Author-email: mirrors.cities0w@icloud.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+
 # MultiMCTS
 
 MultiMCTS is a Python package that implements the [Monte Carlo Tree Search](https://wikipedia.org/wiki/Monte_Carlo_tree_search) algorithm for board games played by any number of players. With MultiMCTS, you can create AI for any board game *merely by knowing the rules* -- no strategy needed!
 
 ## Features
 
 - Efficient (largely C-compiled) MCTS implementation
@@ -18,15 +34,15 @@
 ### You do NOT need to:
 - Have domain knowledge
 - Understand any strategy
 - Evaluate the favorability of a game state
 
 ## Usage
 
-To use MultiMCTS, you must define your game by subclassing `GameState` and implementing the required methods (see [tictactoe.py](https://github.com/taylorvance/multimcts/blob/main/tests/tictactoe.py) for an example):
+To use MultiMCTS, you must define your game by subclassing `GameState` and implementing the required methods (see [examples](https://github.com/taylorvance/multimcts/blob/main/examples/README.md)):
 - get_current_team
 - get_legal_moves
 - make_move
 - is_terminal
 - get_reward
 
 ```python
@@ -41,10 +57,7 @@
 while not state.is_terminal():              # Continue until the game is over.
     print(state)                            # Print the current game state (implementing GameState.__repr__ might be helpful).
     state = mcts.search(state, max_time=1)  # Play the best move found.
 
 print(state)                                # Print the final game state.
 ```
 
-## License
-
-[MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `multimcts-0.2.2/multimcts/mcts.pyx` & `multimcts-0.2.3/multimcts/mcts.pyx`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,73 @@
 from time import time
 from random import shuffle, choice
 from collections import defaultdict
-from typing import Union, Any
+from typing import Union, Dict, List, Any
 
-import cython
+cimport cython
 
 from libc.math cimport log, sqrt, INFINITY
 
 
+Move = Any # MCTS does not care about the contents of a move; it merely passes the output of get_legal_moves() to make_move(), both of which are handled by the user.
+Team = Union[int,str]
+Rewards = Dict[Team,float]
+
+
 class GameState:
-    def get_current_team(self) -> Union[int,str]:
+    def get_current_team(self) -> Team:
         """The identifier of the current player's team."""
         raise NotImplementedError("GameState must implement get_current_team.")
 
-    def get_legal_moves(self) -> list[Any]:
+    def get_legal_moves(self) -> List[Move]:
         """Returns a list of all legal moves from this state."""
         raise NotImplementedError("GameState must implement get_legal_moves.")
 
-    def make_move(self, move:Any) -> 'GameState':
+    def make_move(self, move:Move) -> 'GameState':
         """Returns a new GameState, which is the result of applying the given move to this state.
         Note: The current state (self) should NOT be modified. Rather, modify a copy of it.
         """
         raise NotImplementedError("GameState must implement make_move.")
 
     def is_terminal(self) -> bool:
         """Checks if the game is over."""
         raise NotImplementedError("GameState must implement is_terminal.")
 
-    def get_reward(self) -> Union[float, dict[Union[int,str], float]]:
+    def get_reward(self) -> Union[float, Rewards]:
         """Returns the reward earned by the team that played the game-ending move (i.e. the team from the previous state).
         Typically 1 for win, -1 for loss, 0 for draw.
         Alternatively, returns a dict of teams/rewards: {team1:reward1, team2:reward2, ...}
         Note: This method is only called on terminal states.
         """
         raise NotImplementedError("GameState must implement get_reward.")
 
 
 class Node:
     """Represents a game state node in the MCTS search tree.
 
     Args:
         state (GameState): The game state at the current node.
         parent (Node): The parent of the current node in the search tree.
+        move (Move): The move that was played from the parent node to get to this node.
 
     Attributes:
         children (list): The child nodes of the current node. These represent legal moves that have been visited.
         num_visits (int): The number of times the node has been visited.
         total_reward (dict): The total reward obtained from simulations through the node. Keys are teams; values are rewards.
         is_terminal (bool): Whether the node represents a terminal state.
         is_fully_expanded (bool): Whether all children of the node have been visited.
         remaining_moves (list): A list of moves that have not yet been tried.
     """
-    def __init__(self, state:GameState, parent:'Node'=None):
+    def __init__(self, state:GameState, parent:'Node'=None, move:Move=None):
         self.state = state
         self.parent = parent
+        self.move = move
 
-        self.children:list['Node'] = []
-        self.num_visits = 0
+        self.children:List['Node'] = []
+        self.num_visits:int = 0
         self.total_reward = defaultdict(float)
 
         self.is_terminal:bool = self.state.is_terminal()
         self.is_fully_expanded:bool = self.is_terminal
 
         if self.is_fully_expanded:
             self.remaining_moves = []
@@ -76,25 +83,31 @@
         Args:
             exploration_bias (float): The exploration bias, often denoted as C in the UCB formula.
                 It determines the balance between exploration (choosing a move with uncertain outcome) and exploitation (choosing a move with known high reward).
                 Default is 1.414, which is sqrt(2) and often used in practice.
         """
         self.exploration_bias = exploration_bias
 
-    def search(self, state:GameState, *, max_time:Union[int,float]=None, max_iterations:int=None, heuristic=None) -> GameState:
+    def search(self, state:GameState, *, max_time:Union[int,float]=None, max_iterations:int=None, heuristic=None, return_type:str="state") -> Union[GameState,Move,Node]:
         """Searches for this state's best move until some limit has been reached.
 
         Args:
             state (GameState): The game state for which to find the best move.
             max_time (int|float): The maximum time to search, in seconds.
             max_iterations (int): The maximum number of selections/simulations to perform.
             heuristic (callable): A function that takes a state and returns a move. See simulate() for more information.
+            return_type (str): One of "state", "move", or "node".
         Returns:
             GameState: A new game state which is the result of applying the best move to the given state.
         """
+        return_type = return_type.lower()
+        VALID_RETURN_TYPES = {"state","move","node"}
+        if return_type not in VALID_RETURN_TYPES:
+            raise ValueError(f'Invalid return type: {return_type}, must be one of {VALID_RETURN_TYPES}')
+
         if max_time is None and max_iterations is None:
             raise ValueError("One or more of max_time/max_iterations is required.")
 
         node = Node(state)
 
         cdef double end_time
         cdef int i
@@ -111,15 +124,22 @@
             if max_time is not None and time() >= end_time:
                 break
             if max_iterations is not None:
                 i -= 1
                 if i <= 0:
                     break
 
-        return self.get_best_child(node).state
+        best = self.get_best_child(node)
+
+        if return_type == "state":
+            return best.state
+        elif return_type == "move":
+            return best.move
+        elif return_type == "node":
+            return best
 
     def select(self, node:Node) -> Node:
         """Step 1: Selection
         Traverse the tree for the node we most want to simulate.
         Looks for an unexplored child of this node's best child's best child's...best child.
         """
         while not node.is_terminal:
@@ -136,23 +156,23 @@
         Add a new child to this node.
         """
         try:
             move = node.remaining_moves.pop()
         except IndexError:
             raise IndexError("Tried to expand a node with no remaining moves.")
 
-        child = Node(node.state.make_move(move), node)
+        child = Node(state=node.state.make_move(move), parent=node, move=move)
         node.children.append(child)
 
         if len(node.remaining_moves) == 0:
             node.is_fully_expanded = True
 
         return child
 
-    def simulate(self, node:Node, *, heuristic=None) -> dict[Union[int,str], float]:
+    def simulate(self, node:Node, *, heuristic=None) -> Rewards:
         """Step 3: Simulation (aka playout/rollout)
         Play out a game, from the given node to termination, and return the final reward.
         A heuristic function may be used to guide the simulation. Otherwise, moves are chosen randomly.
 
         Args:
             node (Node): The node from which to begin the simulation.
             heuristic (callable): A function that takes a state and returns a move.
@@ -173,27 +193,24 @@
         reward = state.get_reward()
         if not isinstance(reward, dict):
             reward = {terminal_team: reward}
 
         return reward
 
     @staticmethod
-    def backpropagate(node:Node, reward:dict):
+    def backpropagate(node:Node, reward:Rewards):
         """Step 4: Backpropagation
         Update all ancestors with the reward from this terminal node.
         """
-        # Remove 0-values for efficiency
+        # Remove 0-values for efficiency.
         reward = {k:v for k,v in reward.items() if v!=0}
-
         while node is not None:
             node.num_visits += 1
-
             for key in reward:
                 node.total_reward[key] += reward[key]
-
             node = node.parent
 
     @cython.cdivision(True)
     def get_best_child(self, node:Node) -> Node:
         """Find the child with the highest Upper Confidence Bound (UCB) score.
         ucb = (x / n) + C * sqrt(ln(N) / n)
         x=reward for this node
```

