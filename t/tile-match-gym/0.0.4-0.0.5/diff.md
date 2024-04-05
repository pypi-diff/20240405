# Comparing `tmp/tile-match-gym-0.0.4.tar.gz` & `tmp/tile-match-gym-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tile-match-gym-0.0.4.tar", last modified: Wed Mar 20 12:25:59 2024, max compression
+gzip compressed data, was "tile-match-gym-0.0.5.tar", last modified: Fri Apr  5 13:36:41 2024, max compression
```

## Comparing `tile-match-gym-0.0.4.tar` & `tile-match-gym-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 akshil    (1000) akshil    (1000)        0 2024-03-20 12:25:59.227344 tile-match-gym-0.0.4/
--rw-r--r--   0 akshil    (1000) akshil    (1000)     1545 2024-03-20 12:22:30.000000 tile-match-gym-0.0.4/LICENSE
--rw-r--r--   0 akshil    (1000) akshil    (1000)     4464 2024-03-20 12:25:59.227344 tile-match-gym-0.0.4/PKG-INFO
--rw-r--r--   0 akshil    (1000) akshil    (1000)     1514 2024-03-20 12:22:30.000000 tile-match-gym-0.0.4/README.md
--rw-r--r--   0 akshil    (1000) akshil    (1000)     1514 2024-03-20 12:25:26.000000 tile-match-gym-0.0.4/pyproject.toml
--rw-r--r--   0 akshil    (1000) akshil    (1000)       38 2024-03-20 12:25:59.227344 tile-match-gym-0.0.4/setup.cfg
--rw-r--r--   0 akshil    (1000) akshil    (1000)      189 2024-03-20 12:22:30.000000 tile-match-gym-0.0.4/setup.py
-drwxr-xr-x   0 akshil    (1000) akshil    (1000)        0 2024-03-20 12:25:59.207343 tile-match-gym-0.0.4/src/
-drwxr-xr-x   0 akshil    (1000) akshil    (1000)        0 2024-03-20 12:25:59.217344 tile-match-gym-0.0.4/src/tile_match_gym/
--rw-r--r--   0 akshil    (1000) akshil    (1000)      136 2024-03-20 12:22:30.000000 tile-match-gym-0.0.4/src/tile_match_gym/__init__.py
--rwxr-xr-x   0 akshil    (1000) akshil    (1000)    38494 2024-03-20 12:22:30.000000 tile-match-gym-0.0.4/src/tile_match_gym/board.py
--rw-r--r--   0 akshil    (1000) akshil    (1000)     5091 2024-03-20 12:22:30.000000 tile-match-gym-0.0.4/src/tile_match_gym/tile_match_env.py
-drwxr-xr-x   0 akshil    (1000) akshil    (1000)        0 2024-03-20 12:25:59.227344 tile-match-gym-0.0.4/src/tile_match_gym/utils/
--rw-r--r--   0 akshil    (1000) akshil    (1000)        0 2024-03-20 12:22:30.000000 tile-match-gym-0.0.4/src/tile_match_gym/utils/__init__.py
--rw-r--r--   0 akshil    (1000) akshil    (1000)     2727 2024-03-20 12:22:30.000000 tile-match-gym-0.0.4/src/tile_match_gym/utils/print_board_diffs.py
--rw-r--r--   0 akshil    (1000) akshil    (1000)     1833 2024-03-20 12:22:30.000000 tile-match-gym-0.0.4/src/tile_match_gym/utils.py
--rw-r--r--   0 akshil    (1000) akshil    (1000)     3795 2024-03-20 12:22:30.000000 tile-match-gym-0.0.4/src/tile_match_gym/wrappers.py
-drwxr-xr-x   0 akshil    (1000) akshil    (1000)        0 2024-03-20 12:25:59.227344 tile-match-gym-0.0.4/src/tile_match_gym.egg-info/
--rw-r--r--   0 akshil    (1000) akshil    (1000)     4464 2024-03-20 12:25:59.000000 tile-match-gym-0.0.4/src/tile_match_gym.egg-info/PKG-INFO
--rw-r--r--   0 akshil    (1000) akshil    (1000)      529 2024-03-20 12:25:59.000000 tile-match-gym-0.0.4/src/tile_match_gym.egg-info/SOURCES.txt
--rw-r--r--   0 akshil    (1000) akshil    (1000)        1 2024-03-20 12:25:59.000000 tile-match-gym-0.0.4/src/tile_match_gym.egg-info/dependency_links.txt
--rw-r--r--   0 akshil    (1000) akshil    (1000)       57 2024-03-20 12:25:59.000000 tile-match-gym-0.0.4/src/tile_match_gym.egg-info/requires.txt
--rw-r--r--   0 akshil    (1000) akshil    (1000)       15 2024-03-20 12:25:59.000000 tile-match-gym-0.0.4/src/tile_match_gym.egg-info/top_level.txt
-drwxr-xr-x   0 akshil    (1000) akshil    (1000)        0 2024-03-20 12:25:59.227344 tile-match-gym-0.0.4/tests/
--rw-r--r--   0 akshil    (1000) akshil    (1000)     4451 2024-03-20 12:22:30.000000 tile-match-gym-0.0.4/tests/test_env.py
--rw-r--r--   0 akshil    (1000) akshil    (1000)     1761 2024-03-20 12:22:30.000000 tile-match-gym-0.0.4/tests/test_wrappers.py
+drwxr-xr-x   0 akshil    (1000) akshil    (1000)        0 2024-04-05 13:36:41.703266 tile-match-gym-0.0.5/
+-rw-r--r--   0 akshil    (1000) akshil    (1000)     1545 2024-03-20 12:22:30.000000 tile-match-gym-0.0.5/LICENSE
+-rw-r--r--   0 akshil    (1000) akshil    (1000)     4493 2024-04-05 13:36:41.703266 tile-match-gym-0.0.5/PKG-INFO
+-rw-r--r--   0 akshil    (1000) akshil    (1000)     1514 2024-04-05 13:34:29.000000 tile-match-gym-0.0.5/README.md
+-rw-r--r--   0 akshil    (1000) akshil    (1000)     1535 2024-04-05 13:34:29.000000 tile-match-gym-0.0.5/pyproject.toml
+-rw-r--r--   0 akshil    (1000) akshil    (1000)       38 2024-04-05 13:36:41.703266 tile-match-gym-0.0.5/setup.cfg
+-rw-r--r--   0 akshil    (1000) akshil    (1000)      189 2024-04-05 13:34:29.000000 tile-match-gym-0.0.5/setup.py
+drwxr-xr-x   0 akshil    (1000) akshil    (1000)        0 2024-04-05 13:36:41.703266 tile-match-gym-0.0.5/src/
+drwxr-xr-x   0 akshil    (1000) akshil    (1000)        0 2024-04-05 13:36:41.703266 tile-match-gym-0.0.5/src/tile_match_gym/
+-rw-r--r--   0 akshil    (1000) akshil    (1000)      136 2024-03-20 12:22:30.000000 tile-match-gym-0.0.5/src/tile_match_gym/__init__.py
+-rwxr-xr-x   0 akshil    (1000) akshil    (1000)    40004 2024-04-05 13:34:29.000000 tile-match-gym-0.0.5/src/tile_match_gym/board.py
+-rw-r--r--   0 akshil    (1000) akshil    (1000)     6407 2024-04-05 13:34:29.000000 tile-match-gym-0.0.5/src/tile_match_gym/tile_match_env.py
+drwxr-xr-x   0 akshil    (1000) akshil    (1000)        0 2024-04-05 13:36:41.703266 tile-match-gym-0.0.5/src/tile_match_gym/utils/
+-rw-r--r--   0 akshil    (1000) akshil    (1000)        0 2024-03-20 12:22:30.000000 tile-match-gym-0.0.5/src/tile_match_gym/utils/__init__.py
+-rw-r--r--   0 akshil    (1000) akshil    (1000)     2727 2024-03-20 12:22:30.000000 tile-match-gym-0.0.5/src/tile_match_gym/utils/print_board_diffs.py
+-rw-r--r--   0 akshil    (1000) akshil    (1000)     1833 2024-04-02 18:27:03.000000 tile-match-gym-0.0.5/src/tile_match_gym/utils/utils.py
+-rw-r--r--   0 akshil    (1000) akshil    (1000)     3763 2024-04-02 18:27:03.000000 tile-match-gym-0.0.5/src/tile_match_gym/wrappers.py
+drwxr-xr-x   0 akshil    (1000) akshil    (1000)        0 2024-04-05 13:36:41.703266 tile-match-gym-0.0.5/src/tile_match_gym.egg-info/
+-rw-r--r--   0 akshil    (1000) akshil    (1000)     4493 2024-04-05 13:36:41.000000 tile-match-gym-0.0.5/src/tile_match_gym.egg-info/PKG-INFO
+-rw-r--r--   0 akshil    (1000) akshil    (1000)      535 2024-04-05 13:36:41.000000 tile-match-gym-0.0.5/src/tile_match_gym.egg-info/SOURCES.txt
+-rw-r--r--   0 akshil    (1000) akshil    (1000)        1 2024-04-05 13:36:41.000000 tile-match-gym-0.0.5/src/tile_match_gym.egg-info/dependency_links.txt
+-rw-r--r--   0 akshil    (1000) akshil    (1000)       71 2024-04-05 13:36:41.000000 tile-match-gym-0.0.5/src/tile_match_gym.egg-info/requires.txt
+-rw-r--r--   0 akshil    (1000) akshil    (1000)       15 2024-04-05 13:36:41.000000 tile-match-gym-0.0.5/src/tile_match_gym.egg-info/top_level.txt
+drwxr-xr-x   0 akshil    (1000) akshil    (1000)        0 2024-04-05 13:36:41.703266 tile-match-gym-0.0.5/tests/
+-rw-r--r--   0 akshil    (1000) akshil    (1000)     4451 2024-04-02 18:27:03.000000 tile-match-gym-0.0.5/tests/test_env.py
+-rw-r--r--   0 akshil    (1000) akshil    (1000)     2272 2024-04-02 19:05:44.000000 tile-match-gym-0.0.5/tests/test_wrappers.py
```

### Comparing `tile-match-gym-0.0.4/LICENSE` & `tile-match-gym-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tile-match-gym-0.0.4/PKG-INFO` & `tile-match-gym-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tile-match-gym
-Version: 0.0.4
+Version: 0.0.5
 Summary: A set of reinforcement learning environments for tile matching games, consistent with the OpenAI Gym API.
 Author: James Elson
 Author-email: Akshil Patel <akshilpatel11@gmail.com>
 License: Copyright (c) 2023, Akshil Patel
         Copyright (c) 2023, James Elson
         
         All rights reserved.
@@ -45,14 +45,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.24.3
 Requires-Dist: gymnasium>=0.28.1
+Requires-Dist: numba==0.59.1
 Provides-Extra: testing
 Requires-Dist: pytest>=7.4.0; extra == "testing"
 
 # Tile Matching Reinforcement Learning Environments
 
 Welcome to the Reinforcement Learning Environments for Tile Matching Games repository! Here you can find a collection of tile matching game environments (like Bejeweled or Candy Crush), poised to push reinforcement learning research forwards.
 
@@ -102,11 +103,11 @@
 We'd love it if you use our package for your research! If you do use code from this repository please cite us as below:
 
 ```
 @software{tile_match_gym,
   author = {Patel, Akshil and Elson, James},
   title = {{Tile Matching Game Reinforcement Learning Environments}},
   url = {https://github.com/akshilpatel/tile-match-gym},
-  version = {0.0.3},
+  version = {0.0.5},
   year = {2023}
   }
 ```
```

### Comparing `tile-match-gym-0.0.4/README.md` & `tile-match-gym-0.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -48,11 +48,11 @@
 We'd love it if you use our package for your research! If you do use code from this repository please cite us as below:
 
 ```
 @software{tile_match_gym,
   author = {Patel, Akshil and Elson, James},
   title = {{Tile Matching Game Reinforcement Learning Environments}},
   url = {https://github.com/akshilpatel/tile-match-gym},
-  version = {0.0.3},
+  version = {0.0.5},
   year = {2023}
   }
 ```
```

### Comparing `tile-match-gym-0.0.4/pyproject.toml` & `tile-match-gym-0.0.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tile-match-gym"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     {name="Akshil Patel", email="akshilpatel11@gmail.com"},
     {name="James Elson"}
 ]
 description = "A set of reinforcement learning environments for tile matching games, consistent with the OpenAI Gym API."
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.8"
 dependencies = [
     "numpy>=1.24.3", 
     "gymnasium>=0.28.1",
+    "numba==0.59.1",
 ]
 license = {file="LICENSE"}
 classifiers = [
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
```

### Comparing `tile-match-gym-0.0.4/src/tile_match_gym/board.py` & `tile-match-gym-0.0.5/src/tile_match_gym/board.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import numpy as np
+import numba
+from numba import njit, types, typed
+from numba.experimental import jitclass
 from typing import Optional, List, Tuple
 
+
 """
 tile_colours = {
     0: Colourless
     1: colour1,
     2: ...
 }
 
@@ -17,71 +21,97 @@
     "normal": 1,
     "vertical_laser": 2,
     "horizontal_laser": 3,
     "bomb": 4,
     "cookie": -1,
 }
 
+
+TILE_TYPES = {
+    "empty": 0,
+    "normal": 1,
+    "vertical_laser": 2,
+    "horizontal_laser": 3,
+    "bomb": 4,
+    "cookie": -1,
+}
+numba_spec = [
+    ('num_rows', types.int32),
+    ('num_cols', types.int32),
+    ('num_colours', types.int32),
+    ('flat_size', types.int32),
+    ('colourless_specials', types.ListType(types.string)),
+    ('colour_specials', types.ListType(types.string)),
+    ('specials', types.ListType(types.string)),
+    ('np_random', numba.typeof(np.random.default_rng(0))),
+    ('board', types.Optional(types.Array(types.int32, ndim=3, layout='C'))),
+    ('indices', types.Array(types.int32, ndim=3, layout='C')),
+]
+
+# @jitclass(numba_spec)
 class Board:
     def __init__(
         self,
         num_rows: int,
         num_cols: int,
         num_colours: int,
         colourless_specials: List[str] = ["cookie"],
         colour_specials: List[str] = ["vertical_laser", "horizontal_laser", "bomb"],
-        seed: Optional[int] = None,
+        np_random: np.random.Generator = np.random.default_rng(0),
         board: Optional[np.ndarray] = None,
     ):
         self.num_rows = num_rows
         self.num_cols = num_cols
         self.num_colours = num_colours
 
         self.flat_size = int(self.num_cols * self.num_rows)
 
         self.colourless_specials = colourless_specials
         self.colour_specials = colour_specials
         
         self.specials = set(self.colourless_specials + self.colour_specials)
         
-        if seed is None:
-            seed = np.random.randint(0, 1000000000)
-        self.np_random = np.random.default_rng(seed)
+        self.np_random = np_random
 
         # handle the case where we are given a board
         if board is not None:
-            if type(board) == list:
-                board = np.array(board)
+            if isinstance(board, list):
+                board = np.array(board, dtype=np.int32)
+                print("hi")
             if board.shape[0] != 2 or len(board.shape) < 3:
-                self.board = np.array([
-                    board,
-                    np.ones_like(board)
-                    ])
+                self.board = np.array([board,np.ones_like(board)])
+                print(2)
             else:
                 self.board = board
+                print(3)
 
             self.num_rows = len(self.board[0])
             self.num_cols = len(self.board[0][0])
         
-        self.indices = np.array([[(r, c) for r in range(self.num_cols)] for c in range(self.num_rows)])
+        self.indices = np.zeros((self.num_rows, self.num_cols, 2), dtype=np.int32)
+        for r in range(self.num_rows):
+            for c in range(self.num_cols):
+                self.indices[r, c] = (r, c)
 
     def generate_board(self):
         self.board = np.ones((2, self.num_rows, self.num_cols), dtype=np.int32)
         self.board[0] = self.np_random.integers(1, self.num_colours+1, self.flat_size).reshape(self.num_rows, self.num_cols)
 
         line_matches = self.get_colour_lines()
+        # line_matches = get_colour_lines(self.board)
         num_line_matches = len(line_matches)
 
         while not self.possible_move() or num_line_matches > 0:
             if num_line_matches > 0:
                 self.remove_colour_lines(line_matches)
             else:
                 self.shuffle()
 
             line_matches = self.get_colour_lines()
+            # line_matches = get_colour_lines(self.board)
             num_line_matches = len(line_matches)
         
         # assert self.possible_move()
         # assert self.get_colour_lines() == []
 
     def shuffle(self):
         shuffled_idcs = np.arange(self.num_rows * self.num_cols)
@@ -96,24 +126,26 @@
             line_matches (List[List[Tuple[int, int]]]): List of lines where each line is colour match.
         """
         while len(line_matches) > 0:
             l = line_matches[0]
             row = min(self.num_rows - 1, l[0][0] + 1)
             self.board[0, :row+1, :] = self.np_random.integers(1, self.num_colours+1, int((row+1) * self.num_cols)).reshape(-1, self.num_cols)
             line_matches = self.get_colour_lines()
-            
+            # line_matches = get_colour_lines(self.board)
+
     def detect_colour_matches(self) -> Tuple[List[List[Tuple[int, int]]], List[str], List[int]]:
         """
         Returns the types and locations of tiles involved in the bottom-most colour matches.
         """
         # For an empty board we can skip this.
         # if np.all(self.board[0] == 0):
         #     return [], [], []
         
         lines = self.get_colour_lines()
+        # lines = get_colour_lines(self.board)
 
         if len(lines) == 0:
             return [], [], []
         else:
             tile_coords, tile_names, tile_colours = self.process_colour_lines(lines)
             return tile_coords, tile_names, tile_colours
 
@@ -232,74 +264,16 @@
             return False
         
         # Check coords are next to each other.
         if not (coord1[0] == coord2[0] or coord1[1] == coord2[1]) or np.abs(coord1[0] - coord2[0]) > 1 or  np.abs(coord1[1] - coord2[1]) > 1:
             return False
 
         return True
-    
-    
-    # TODO: Make this faster.
-    def is_move_effective(self, coord1: Tuple[int, int], coord2: Tuple[int, int]) -> bool:
-        """
-        This function checks if the action actually does anything i.e. if the action achieves some form of matching.
-
-        Args:
-            coord (tuple): The first coordinate on grid corresponding to the action taken. This will always be above or to the left of the second coordinate below.
-            coord2 (tuple): Second coordinate on grid corresponding to the action taken.
-
-        Returns:
-            bool: True iff action has an effect on the environment.
-        """
-        
-        # Checks if both are special
-        if (self.board[1, coord1[0], coord1[1]] not in [0, 1] ) and (self.board[1, coord2[0], coord2[1]] not in [0, 1]):
-            
-            return True
-
-        # At least one colourless special.
-        if self.board[1, coord1[0], coord1[1]] < 0 or self.board[1, coord2[0], coord2[1]] < 0:
-            return True
-
-        # Extract a minimal grid around the coords to check for at least 3 match. This covers checking for Ls or Ts.
-
-        r_min = max(0, min(coord1[0], coord2[0]) - 2)
-        
-        r_max = min(self.num_rows-1, max(coord1[0], coord2[0]) + 2)
-
-        c_min = max(0, min(coord1[1], coord2[1]) - 2)
-        c_max = min(self.num_cols-1, max(coord1[1], coord2[1]) + 2)
-        
-        # Swap the coordinates_ to see what happens.
-        self._swap_coords(coord1, coord2)
-        
-        if c_min + 2 <= c_max:
-        # Horizontal Matches
-            for r in range(r_min, r_max + 1):
-                for c in range(c_min + 2, c_max + 1):
-                    # If the current and previous 2 are matched and that they are not cookies.
-                    if self.board[1, r, c] > 0: # Check it isn't a colourless special or empty.
-                        if self.board[0, r, c - 2] == self.board[0, r, c - 1] == self.board[0, r, c]:
-                            # Swap back
-                            self._swap_coords(coord1, coord2)
-                            return True
-
-        # Vertical
-        if r_min + 2 <= r_max:
-            for r in range(r_min + 2, r_max+1):
-                for c in range(c_min, c_max+1):
-                    if self.board[1, r, c] > 0: 
-                        if self.board[0, r - 2, c] == self.board[0, r - 1, c] == self.board[0, r, c]:
-                            self._swap_coords(coord1, coord2)
-                            return True
 
 
-        self._swap_coords(coord1, coord2)
-        return False
-
     def _swap_coords(self, coord1: Tuple[int, int], coord2: Tuple[int, int]) -> None:
         self.board[0, coord1[0], coord1[1]], self.board[0, coord2[0], coord2[1]] = self.board[0, coord2[0], coord2[1]], self.board[0, coord1[0], coord1[1]]
         self.board[1, coord1[0], coord1[1]], self.board[1, coord2[0], coord2[1]] = self.board[1, coord2[0], coord2[1]], self.board[1, coord1[0], coord1[1]]
 
     def process_colour_lines(self, lines: List[List[Tuple[int, int]]]) -> Tuple[List[List[Tuple[int, int]]], List[str], List[int]]:
         """
         Given list of contiguous lines, this function detects the match type from the bottom up, merging any lines that share a coordinate.
@@ -385,15 +359,15 @@
         num_eliminations = 0
         is_combination_match = False
         shuffled = False
 
         if not self.is_move_legal(coord1, coord2):
             raise ValueError(f"Invalid move: {coord1}, {coord2}")
 
-        if not self.is_move_effective(coord1, coord2):
+        if not is_move_effective(self.board, coord1, coord2):
             return num_eliminations, is_combination_match, self.num_new_specials, self.num_specials_activated, shuffled
         
         self._swap_coords(coord1, coord2)
         
         ## Combination match ##
         has_two_specials = self.board[1, coord1[0], coord1[1]] not in [0,1] and self.board[1, coord2[0], coord2[1]] not in [0,1]
         has_one_colourless_special = self.board[1, coord1[0], coord1[1]] < 0 or self.board[1, coord2[0], coord2[1]] < 0
@@ -426,14 +400,16 @@
             shuffled=True
             if num_line_matches > 0:
                 self.remove_colour_lines(line_matches)
             else:
                 self.shuffle()
 
             line_matches = self.get_colour_lines()
+            # line_matches = get_colour_lines(self.board)
+
             num_line_matches = len(line_matches)
 
         # assert self.possible_move()
         # assert self.get_colour_lines() == []
         return num_eliminations, is_combination_match, self.num_new_specials, self.num_specials_activated, shuffled
 
     def resolve_colour_matches(
@@ -804,7 +780,69 @@
             # Iterate through activation area.
             for i in range(min_r, max_r + 1):
                 for j in range(min_c, max_c + 1):
                     if self.board[1, i, j] == 1:
                         self.board[:, i, j] = 0
                     elif self.board[1, i, j] != 0:
                         self.activate_special((i, j), self.board[1, i, j], self.board[0, i, j], is_combination_match=True)
+
+@njit
+def swap_coords(board: np.ndarray, coord1: Tuple[int, int], coord2: Tuple[int, int]) -> None: 
+    board[0, coord1[0], coord1[1]], board[0, coord2[0], coord2[1]] = board[0, coord2[0], coord2[1]], board[0, coord1[0], coord1[1]]
+    board[1, coord1[0], coord1[1]], board[1, coord2[0], coord2[1]] = board[1, coord2[0], coord2[1]], board[1, coord1[0], coord1[1]]
+
+
+@njit
+def is_move_effective(board: np.ndarray, coord1: Tuple[int, int], coord2: Tuple[int, int]) -> bool:
+    """
+    This function checks if the action actually does anything i.e. if the action achieves some form of matching.
+
+    Args:
+        coord (tuple): The first coordinate on grid corresponding to the action taken. This will always be above or to the left of the second coordinate below.
+        coord2 (tuple): Second coordinate on grid corresponding to the action taken.
+
+    Returns:
+        bool: True iff action has an effect on the environment.
+    """
+    num_rows, num_cols = board.shape[1:]
+    # Checks if both are special
+    if (board[1, coord1[0], coord1[1]] not in [0, 1] ) and (board[1, coord2[0], coord2[1]] not in [0, 1]):
+        return True
+
+    # At least one colourless special.
+    if board[1, coord1[0], coord1[1]] < 0 or board[1, coord2[0], coord2[1]] < 0:
+        return True
+
+    # Extract a minimal grid around the coords to check for at least 3 match. This covers checking for Ls or Ts.
+
+    r_min = max(0, min(coord1[0], coord2[0]) - 2)
+    r_max = min(num_rows-1, max(coord1[0], coord2[0]) + 2)
+    c_min = max(0, min(coord1[1], coord2[1]) - 2)
+    c_max = min(num_cols-1, max(coord1[1], coord2[1]) + 2)
+    
+    # print(f"for coords: {coord1}, {coord2}, row range: {r_min} - {r_max}, col range: {c_min} - {c_max}")
+    
+    # Swap the coordinates_ to see what happens.
+    swap_coords(board, coord1, coord2)
+    colour_slice = board[0, r_min:r_max + 1, c_min:c_max + 1]
+    # Horizontal Matches
+    if c_min + 2 <= c_max:
+        # horizontal_slice = colour_slice  # Slice for horizontal comparison
+        horizontal_matches = (colour_slice[:, :-2] == colour_slice[:, 1:-1]) & (colour_slice[:, 1:-1] == colour_slice[:, 2:])
+        matching_indices = np.nonzero(horizontal_matches & (board[1, r_min:r_max + 1, c_min + 2:c_max + 1] > 0))
+        if matching_indices[0].size > 0:
+            # Swap back
+            swap_coords(board, coord1, coord2)
+            return True
+
+    # Vertical Matches
+    if r_min + 2 <= r_max:
+        # vertical_slice = colour_slice  # Slice for vertical comparison
+        vertical_matches = (colour_slice[:-2, :] == colour_slice[1:-1, :]) & (colour_slice[1:-1, :] == colour_slice[2:, :])
+        matching_indices = np.nonzero(vertical_matches & (board[1, r_min + 2:r_max + 1, c_min:c_max + 1] > 0))
+        if matching_indices[0].size > 0:
+            # Swap back
+            swap_coords(board, coord1, coord2)
+            return True
+        
+    swap_coords(board, coord1, coord2)
+    return False
```

### Comparing `tile-match-gym-0.0.4/src/tile_match_gym/tile_match_env.py` & `tile-match-gym-0.0.5/src/tile_match_gym/tile_match_env.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,51 @@
-
 import gymnasium as gym
 import numpy as np
 
 from gymnasium.spaces import Discrete, Box
 from typing import Optional, List, Tuple
 from collections import OrderedDict
 from tile_match_gym.board import Board
+from tile_match_gym.board import is_move_effective
 
 class TileMatchEnv(gym.Env):
-    metadata = {'render_modes': ['human']}
+    metadata = {'render_modes': ['string']}
     def __init__(
             self, 
             num_rows:int, 
             num_cols:int, 
             num_colours:int, 
             num_moves: int,
             colourless_specials:List[str], 
             colour_specials: List[str],
-            seed: Optional[int] = 1
+            seed: Optional[int] = 1,
+            render_mode: str = "string"
             ):
         self.num_rows = num_rows
         self.num_cols = num_cols
         self.num_colours = num_colours
         self.colourless_specials = colourless_specials
         self.colour_specials = colour_specials
         self.num_moves = num_moves
 
+        if render_mode == "string":
+            self.colour_map = self.np_random.choice(range(105, 230), size=self.num_colours + 1, replace=False)
+        self.render_mode = render_mode
+
         # Each coordinate can switch right or down but those one the right/bottom edge can't switch right/down
         self.num_actions = int((self.num_rows * self.num_cols * 2) - self.num_rows - self.num_cols )
 
         self.num_colour_specials = len(self.colour_specials)
         self.num_colourless_specials = len(self.colourless_specials)
 
         self.seed = seed
-        self.board = Board(num_rows, num_cols, num_colours, colourless_specials, colour_specials, seed=seed)
-        self.np_random = self.board.np_random
 
+        np_random = np.random.default_rng(seed=seed)
+        self.board = Board(num_rows, num_cols, num_colours, colourless_specials, colour_specials, np_random)
+        self.np_random = self.board.np_random
         obs_low = np.array([np.zeros((self.num_rows, self.num_cols), dtype=np.int32), np.full((self.num_rows, self.num_cols), - self.num_colourless_specials, dtype=np.int32)])
         obs_high = np.array([np.full((self.num_rows, self.num_cols), self.num_colours, dtype=np.int32), np.full((self.num_rows, self.num_cols), self.num_colour_specials + 2, dtype=np.int32)]) # + 1 for empty
         
         self._board_observation_space = Box(
             low=obs_low, 
             high=obs_high,
             shape=(2, self.num_rows, self.num_cols),
@@ -107,19 +113,43 @@
             col = action_ % (self.num_cols - 1)
             return (row, col), (row, col + 1)
 
     def _get_effective_actions(self) -> List[int]:
         if self.timer == self.num_moves:
             return []
         effective_actions = []
-        for a in range(self.num_actions):
-            coord1, coord2 = self._action_to_coords(a)
-            if self.board.is_move_effective(coord1, coord2):
-                effective_actions.append(a)
+
+        action_check = lambda a: is_move_effective(self.board.board, *self._action_to_coords(a))
+        effective_actions = list(filter(action_check, range(self.num_actions)))
+        # for a in range(self.num_actions):
+        #     coord1, coord2 = self._action_to_coords(a)
+        #     if is_move_effective(self.board.board, coord1, coord2):
+        #         effective_actions.append(a)
         return effective_actions
 
-    def render(self, mode: str="human") -> None:
-        print(self.board.board)
+    def render(self) -> None:
+        if self.render_mode == "string":
+            color = lambda id, c: "\033[48;5;16m" + f"\033[38;5;{self.colour_map[id]}m{c}\033[0m"
+            height = self.board.board.shape[1]
+            width = self.board.board.shape[2]
+
+            print(" " + "-" * (width * 2 + 1))
+            for row_num in range(height):
+                print("| ", end="\033[48;5;16m")
+                for col in range(width):
+                    tile_colour = self.board.board[0, row_num, col]
+                    tile_type = self.board.board[1, row_num, col]
+                
+                    print(color(tile_colour, tile_type), end="\033[48;5;16m ")
+                    print("\033[0m", end="")
+
+                print("|", end="\n")
+            print(" " + "-" * (width * 2 + 1))
+
+        elif self.render_mode == "image":
+            pass
+
+        
 
     def close(self) -> None:
         if self.renderer is not None:
             self.renderer.close()
```

### Comparing `tile-match-gym-0.0.4/src/tile_match_gym/utils/print_board_diffs.py` & `tile-match-gym-0.0.5/src/tile_match_gym/utils/print_board_diffs.py`

 * *Files identical despite different names*

### Comparing `tile-match-gym-0.0.4/src/tile_match_gym/utils.py` & `tile-match-gym-0.0.5/src/tile_match_gym/utils/utils.py`

 * *Files identical despite different names*

### Comparing `tile-match-gym-0.0.4/src/tile_match_gym/wrappers.py` & `tile-match-gym-0.0.5/src/tile_match_gym/wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,14 @@
         
         self.type_slices = [] # Don't track ordinary type
         for special, idx in self._global_specials.items():
             if special in self.colour_specials or special in self.colourless_specials:
                 self.type_slices.append(idx)
 
         self.type_slices = np.array(sorted(self.type_slices)) + self.global_num_colourless_specials
-        print(self.type_slices)
         self.num_type_slices = len(self.type_slices)
 
     def observation(self, obs) -> dict:
         board = obs["board"]
         ohe_board = self._one_hot_encode_board(board)
         return OrderedDict([("board", ohe_board), ("num_moves_left", obs["num_moves_left"])])
```

### Comparing `tile-match-gym-0.0.4/src/tile_match_gym.egg-info/PKG-INFO` & `tile-match-gym-0.0.5/src/tile_match_gym.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tile-match-gym
-Version: 0.0.4
+Version: 0.0.5
 Summary: A set of reinforcement learning environments for tile matching games, consistent with the OpenAI Gym API.
 Author: James Elson
 Author-email: Akshil Patel <akshilpatel11@gmail.com>
 License: Copyright (c) 2023, Akshil Patel
         Copyright (c) 2023, James Elson
         
         All rights reserved.
@@ -45,14 +45,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.24.3
 Requires-Dist: gymnasium>=0.28.1
+Requires-Dist: numba==0.59.1
 Provides-Extra: testing
 Requires-Dist: pytest>=7.4.0; extra == "testing"
 
 # Tile Matching Reinforcement Learning Environments
 
 Welcome to the Reinforcement Learning Environments for Tile Matching Games repository! Here you can find a collection of tile matching game environments (like Bejeweled or Candy Crush), poised to push reinforcement learning research forwards.
 
@@ -102,11 +103,11 @@
 We'd love it if you use our package for your research! If you do use code from this repository please cite us as below:
 
 ```
 @software{tile_match_gym,
   author = {Patel, Akshil and Elson, James},
   title = {{Tile Matching Game Reinforcement Learning Environments}},
   url = {https://github.com/akshilpatel/tile-match-gym},
-  version = {0.0.3},
+  version = {0.0.5},
   year = {2023}
   }
 ```
```

### Comparing `tile-match-gym-0.0.4/src/tile_match_gym.egg-info/SOURCES.txt` & `tile-match-gym-0.0.5/src/tile_match_gym.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 src/tile_match_gym/__init__.py
 src/tile_match_gym/board.py
 src/tile_match_gym/tile_match_env.py
-src/tile_match_gym/utils.py
 src/tile_match_gym/wrappers.py
 src/tile_match_gym.egg-info/PKG-INFO
 src/tile_match_gym.egg-info/SOURCES.txt
 src/tile_match_gym.egg-info/dependency_links.txt
 src/tile_match_gym.egg-info/requires.txt
 src/tile_match_gym.egg-info/top_level.txt
 src/tile_match_gym/utils/__init__.py
 src/tile_match_gym/utils/print_board_diffs.py
+src/tile_match_gym/utils/utils.py
 tests/test_env.py
 tests/test_wrappers.py
```

### Comparing `tile-match-gym-0.0.4/tests/test_env.py` & `tile-match-gym-0.0.5/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `tile-match-gym-0.0.4/tests/test_wrappers.py` & `tile-match-gym-0.0.5/tests/test_wrappers.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,7 +36,24 @@
     assert obs["num_moves_left"] == 12
     # Make a cookie.
     obs, *_ = env.step(2)
     assert np.array_equal(obs["board"][:, 1, 2], np.array([0, 0, 1, 0], dtype=np.float32)), (obs["board"][:, 3, 2], env.unwrapped.board.board[:, 3,2])
     assert obs["board"].shape == (4, 5, 5)
     assert obs["num_moves_left"] == 11
 
+# def test_timing():
+#     import time
+#     env = TileMatchEnv(30, 30, 12, 10, [], [], seed=1)
+#     env = OneHotWrapper(env)
+#     start = time.time()
+#     # run for 1000 steps
+#     obs, info = env.reset()
+#     for _ in range(100):
+#         action = env.action_space.sample()
+#         next_obs, _, done, _, _ = env.step(action)
+#         obs = next_obs
+#         if done:
+#             obs, info = env.reset()
+#     print(f"Time taken for 1000 steps: {time.time() - start} seconds")
+
+#     assert False
+
```

