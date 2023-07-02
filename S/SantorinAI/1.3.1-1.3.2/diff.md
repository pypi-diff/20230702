# Comparing `tmp/SantorinAI-1.3.1.tar.gz` & `tmp/SantorinAI-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SantorinAI-1.3.1.tar", last modified: Sun Jul  2 19:30:01 2023, max compression
+gzip compressed data, was "SantorinAI-1.3.2.tar", last modified: Sun Jul  2 19:37:27 2023, max compression
```

## Comparing `SantorinAI-1.3.1.tar` & `SantorinAI-1.3.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:30:01.098400 SantorinAI-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-07-02 19:30:01.098400 SantorinAI-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:30:01.094400 SantorinAI-1.3.1/SantorinAI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-07-02 19:30:01.000000 SantorinAI-1.3.1/SantorinAI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-02 19:30:01.000000 SantorinAI-1.3.1/SantorinAI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 19:30:01.000000 SantorinAI-1.3.1/SantorinAI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-02 19:30:01.000000 SantorinAI-1.3.1/SantorinAI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-02 19:30:01.000000 SantorinAI-1.3.1/SantorinAI.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:30:01.094400 SantorinAI-1.3.1/santorinai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/santorinai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18497 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/santorinai/board.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:30:01.094400 SantorinAI-1.3.1/santorinai/board_displayer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/santorinai/board_displayer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/santorinai/board_displayer/board_displayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/santorinai/pawn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/santorinai/player.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:30:01.098400 SantorinAI-1.3.1/santorinai/player_examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/santorinai/player_examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/santorinai/player_examples/basic_player.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/santorinai/player_examples/first_choice_player.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/santorinai/player_examples/random_player.py
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/santorinai/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-02 19:30:01.098400 SantorinAI-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:30:01.098400 SantorinAI-1.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21019 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/test/test_board.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/test/test_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:37:27.556893 SantorinAI-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-07-02 19:37:27.556893 SantorinAI-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:37:27.556893 SantorinAI-1.3.2/SantorinAI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-07-02 19:37:27.000000 SantorinAI-1.3.2/SantorinAI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-02 19:37:27.000000 SantorinAI-1.3.2/SantorinAI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 19:37:27.000000 SantorinAI-1.3.2/SantorinAI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-02 19:37:27.000000 SantorinAI-1.3.2/SantorinAI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-02 19:37:27.000000 SantorinAI-1.3.2/SantorinAI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:37:27.556893 SantorinAI-1.3.2/santorinai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/santorinai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18503 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/santorinai/board.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:37:27.556893 SantorinAI-1.3.2/santorinai/board_displayer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/santorinai/board_displayer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/santorinai/board_displayer/board_displayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/santorinai/pawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/santorinai/player.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:37:27.556893 SantorinAI-1.3.2/santorinai/player_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/santorinai/player_examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/santorinai/player_examples/basic_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/santorinai/player_examples/first_choice_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/santorinai/player_examples/random_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/santorinai/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-02 19:37:27.556893 SantorinAI-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:37:27.556893 SantorinAI-1.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21019 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/test/test_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/test/test_tester.py
```

### Comparing `SantorinAI-1.3.1/LICENSE` & `SantorinAI-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.3.1/PKG-INFO` & `SantorinAI-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SantorinAI
-Version: 1.3.1
+Version: 1.3.2
 Summary: A Python library for the Santorini board game
 Home-page: https://github.com/tomansion/santorinai
 Author: Tom Mansion
 Author-email: tomansion@yahoo.fr
 Keywords: santorini,ai,boardgame
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `SantorinAI-1.3.1/README.md` & `SantorinAI-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.3.1/SantorinAI.egg-info/PKG-INFO` & `SantorinAI-1.3.2/SantorinAI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SantorinAI
-Version: 1.3.1
+Version: 1.3.2
 Summary: A Python library for the Santorini board game
 Home-page: https://github.com/tomansion/santorinai
 Author: Tom Mansion
 Author-email: tomansion@yahoo.fr
 Keywords: santorini,ai,boardgame
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `SantorinAI-1.3.1/SantorinAI.egg-info/SOURCES.txt` & `SantorinAI-1.3.2/SantorinAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.3.1/santorinai/board.py` & `SantorinAI-1.3.2/santorinai/board.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from santorinai.pawn import Pawn
-from typing import Tuple
+from typing import Tuple, List
 
 
 class Board:
     """
     Represents the game board for the Santorini game.
 
     Attributes:
@@ -32,15 +32,15 @@
         Initializes a new instance of the Board class.
 
         Args:
             number_of_players (int): The number of players in the game.
         """
 
         # Create the pawns for each player
-        self.pawns: list[Pawn] = []
+        self.pawns: List[Pawn] = []
         self.nb_players = number_of_players
         self.nb_pawns = number_of_players * 2
 
         # For 2 player games:
         # - Player 1 has pawns 1, 3
         # - Player 2 has pawns 2, 4
 
@@ -208,15 +208,15 @@
         Gets the pawn of the current player.
 
         Returns:
             Pawn: The pawn of the current player.
         """
         return self.pawns[self.pawn_turn - 1]
 
-    def get_possible_movement_positions(self, pawn: Pawn) -> list[Tuple[int, int]]:
+    def get_possible_movement_positions(self, pawn: Pawn) -> List[Tuple[int, int]]:
         """
         Gets all the possible moves for a given pawn.
 
         Args:
             pawn (Pawn): The pawn for which to get the possible moves.
 
         Returns:
@@ -246,15 +246,15 @@
                 # Check if the move is possible
                 move_possible, _ = self.is_move_possible(pawn.pos, new_pawn_pos)
                 if move_possible:
                     possible_moves.append((pawn.pos[0] + x, pawn.pos[1] + y))
 
         return possible_moves
 
-    def get_possible_building_positions(self, pawn: Pawn) -> list[Tuple[int, int]]:
+    def get_possible_building_positions(self, pawn: Pawn) -> List[Tuple[int, int]]:
         """
         Gets all the possible builds for a given pawn, supposing it has already moved.
 
         Args:
             pawn (Pawn): The pawn for which to get the possible builds.
 
         Returns:
```

### Comparing `SantorinAI-1.3.1/santorinai/board_displayer/board_displayer.py` & `SantorinAI-1.3.2/santorinai/board_displayer/board_displayer.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.3.1/santorinai/pawn.py` & `SantorinAI-1.3.2/santorinai/pawn.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.3.1/santorinai/player.py` & `SantorinAI-1.3.2/santorinai/player.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.3.1/santorinai/player_examples/basic_player.py` & `SantorinAI-1.3.2/santorinai/player_examples/basic_player.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.3.1/santorinai/player_examples/first_choice_player.py` & `SantorinAI-1.3.2/santorinai/player_examples/first_choice_player.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.3.1/santorinai/player_examples/random_player.py` & `SantorinAI-1.3.2/santorinai/player_examples/random_player.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.3.1/santorinai/tester.py` & `SantorinAI-1.3.2/santorinai/tester.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.3.1/setup.py` & `SantorinAI-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="SantorinAI",
-    version="1.3.1",
+    version="1.3.2",
     author="Tom Mansion",
     author_email="tomansion@yahoo.fr",
     description="A Python library for the Santorini board game",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/tomansion/santorinai",
     packages=find_packages(),
```

### Comparing `SantorinAI-1.3.1/test/test_board.py` & `SantorinAI-1.3.2/test/test_board.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.3.1/test/test_tester.py` & `SantorinAI-1.3.2/test/test_tester.py`

 * *Files identical despite different names*

