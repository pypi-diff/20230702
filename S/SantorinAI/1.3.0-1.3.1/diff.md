# Comparing `tmp/SantorinAI-1.3.0.tar.gz` & `tmp/SantorinAI-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SantorinAI-1.3.0.tar", last modified: Wed May 17 20:12:41 2023, max compression
+gzip compressed data, was "SantorinAI-1.3.1.tar", last modified: Sun Jul  2 19:30:01 2023, max compression
```

## Comparing `SantorinAI-1.3.0.tar` & `SantorinAI-1.3.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:12:41.983763 SantorinAI-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-17 20:12:41.983763 SantorinAI-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:12:41.979763 SantorinAI-1.3.0/SantorinAI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-17 20:12:41.000000 SantorinAI-1.3.0/SantorinAI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-17 20:12:41.000000 SantorinAI-1.3.0/SantorinAI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 20:12:41.000000 SantorinAI-1.3.0/SantorinAI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-17 20:12:41.000000 SantorinAI-1.3.0/SantorinAI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-17 20:12:41.000000 SantorinAI-1.3.0/SantorinAI.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:12:41.979763 SantorinAI-1.3.0/santorinai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/santorinai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/santorinai/board.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:12:41.979763 SantorinAI-1.3.0/santorinai/board_displayer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/santorinai/board_displayer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/santorinai/board_displayer/board_displayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/santorinai/pawn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/santorinai/player.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:12:41.983763 SantorinAI-1.3.0/santorinai/player_examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/santorinai/player_examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/santorinai/player_examples/basic_player.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/santorinai/player_examples/first_choice_player.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/santorinai/player_examples/random_player.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/santorinai/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 20:12:41.983763 SantorinAI-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:12:41.983763 SantorinAI-1.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21019 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/test/test_board.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-17 20:12:36.000000 SantorinAI-1.3.0/test/test_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:30:01.098400 SantorinAI-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-07-02 19:30:01.098400 SantorinAI-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:30:01.094400 SantorinAI-1.3.1/SantorinAI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-07-02 19:30:01.000000 SantorinAI-1.3.1/SantorinAI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-02 19:30:01.000000 SantorinAI-1.3.1/SantorinAI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 19:30:01.000000 SantorinAI-1.3.1/SantorinAI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-02 19:30:01.000000 SantorinAI-1.3.1/SantorinAI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-02 19:30:01.000000 SantorinAI-1.3.1/SantorinAI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:30:01.094400 SantorinAI-1.3.1/santorinai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/santorinai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18497 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/santorinai/board.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:30:01.094400 SantorinAI-1.3.1/santorinai/board_displayer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/santorinai/board_displayer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/santorinai/board_displayer/board_displayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/santorinai/pawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/santorinai/player.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:30:01.098400 SantorinAI-1.3.1/santorinai/player_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/santorinai/player_examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/santorinai/player_examples/basic_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/santorinai/player_examples/first_choice_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/santorinai/player_examples/random_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/santorinai/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-02 19:30:01.098400 SantorinAI-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:30:01.098400 SantorinAI-1.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21019 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/test/test_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-02 19:29:57.000000 SantorinAI-1.3.1/test/test_tester.py
```

### Comparing `SantorinAI-1.3.0/LICENSE` & `SantorinAI-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.3.0/PKG-INFO` & `SantorinAI-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SantorinAI
-Version: 1.3.0
+Version: 1.3.1
 Summary: A Python library for the Santorini board game
 Home-page: https://github.com/tomansion/santorinai
 Author: Tom Mansion
 Author-email: tomansion@yahoo.fr
 Keywords: santorini,ai,boardgame
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `SantorinAI-1.3.0/README.md` & `SantorinAI-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.3.0/SantorinAI.egg-info/PKG-INFO` & `SantorinAI-1.3.1/SantorinAI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SantorinAI
-Version: 1.3.0
+Version: 1.3.1
 Summary: A Python library for the Santorini board game
 Home-page: https://github.com/tomansion/santorinai
 Author: Tom Mansion
 Author-email: tomansion@yahoo.fr
 Keywords: santorini,ai,boardgame
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `SantorinAI-1.3.0/SantorinAI.egg-info/SOURCES.txt` & `SantorinAI-1.3.1/SantorinAI.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+setup.cfg
 setup.py
 SantorinAI.egg-info/PKG-INFO
 SantorinAI.egg-info/SOURCES.txt
 SantorinAI.egg-info/dependency_links.txt
 SantorinAI.egg-info/requires.txt
 SantorinAI.egg-info/top_level.txt
 santorinai/__init__.py
```

### Comparing `SantorinAI-1.3.0/santorinai/board.py` & `SantorinAI-1.3.1/santorinai/board.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         Initializes a new instance of the Board class.
 
         Args:
             number_of_players (int): The number of players in the game.
         """
 
         # Create the pawns for each player
-        self.pawns = []
+        self.pawns: list[Pawn] = []
         self.nb_players = number_of_players
         self.nb_pawns = number_of_players * 2
 
         # For 2 player games:
         # - Player 1 has pawns 1, 3
         # - Player 2 has pawns 2, 4
 
@@ -208,59 +208,66 @@
         Gets the pawn of the current player.
 
         Returns:
             Pawn: The pawn of the current player.
         """
         return self.pawns[self.pawn_turn - 1]
 
-    def get_possible_movement_positions(self, pawn: Pawn):
+    def get_possible_movement_positions(self, pawn: Pawn) -> list[Tuple[int, int]]:
         """
         Gets all the possible moves for a given pawn.
 
         Args:
             pawn (Pawn): The pawn for which to get the possible moves.
 
         Returns:
             list: A list of all the possible moves for the given pawn.
         """
         possible_moves = []
 
-        # If pwan position is None, it means it has not been placed yet
+        # If pawn position is None, it means it has not been placed yet
         # Every position is possible except the ones occupied by other pawns
         # and the ones where tower are terminated
-        if pawn.pos == (None, None):
+        if pawn.pos[0] is None or pawn.pos[1] is None:
             for x in range(self.board_size):
                 for y in range(self.board_size):
                     if self.board[x][y] != 4 and not self.is_pawn_on_position((x, y)):
                         possible_moves.append((x, y))
             return possible_moves
 
-        # Get all the possible moves
+        # Get all the possible moves from the 8 positions around the pawn
         for x in range(-1, 2):
             for y in range(-1, 2):
+                # We can't move on the same position
                 if x == 0 and y == 0:
                     continue
-                move_possible, _ = self.is_move_possible(
-                    pawn.pos, (pawn.pos[0] + x, pawn.pos[1] + y)
-                )
+
+                new_pawn_pos = (pawn.pos[0] + x, pawn.pos[1] + y)
+
+                # Check if the move is possible
+                move_possible, _ = self.is_move_possible(pawn.pos, new_pawn_pos)
                 if move_possible:
                     possible_moves.append((pawn.pos[0] + x, pawn.pos[1] + y))
 
         return possible_moves
 
-    def get_possible_building_positions(self, pawn: Pawn):
+    def get_possible_building_positions(self, pawn: Pawn) -> list[Tuple[int, int]]:
         """
         Gets all the possible builds for a given pawn, supposing it has already moved.
 
         Args:
             pawn (Pawn): The pawn for which to get the possible builds.
 
         Returns:
             list: A list of all the possible builds for the given pawn.
         """
+
+        if pawn.pos[0] is None or pawn.pos[1] is None:
+            return []
+
         possible_builds = []
 
         # Get all the possible builds
         for x in range(-1, 2):
             for y in range(-1, 2):
                 if x == 0 and y == 0:
                     continue
@@ -276,30 +283,32 @@
         """
         Gets all the possible moves and builds for a given pawn.
         :param pawn: The pawn for which to get the possible moves and builds.
         :return: A list of all the possible moves and builds for the given pawn.
         [(move_position, build_position), ...]
         """
 
-        if pawn.pos == (None, None):
+        if pawn.pos[0] is None or pawn.pos[1] is None:
             # Pawn not placed yet
             possible_spawn_positions = self.get_possible_movement_positions(pawn)
             return [(position, None) for position in possible_spawn_positions]
 
+        possible_moves_and_builds = []
+        original_position = (pawn.pos[0], pawn.pos[1])
         possible_moves = self.get_possible_movement_positions(pawn)
 
-        possible_moves_and_builds = []
-        original_position = pawn.pos
         for move in possible_moves:
             pawn.move(move)
             possible_builds = self.get_possible_building_positions(pawn)
             for build in possible_builds:
                 possible_moves_and_builds.append((move, build))
 
+        # Move the pawn back to its original position
         pawn.move(original_position)
+
         return possible_moves_and_builds
 
     def place_pawn(self, position: Tuple[int, int]) -> Tuple[bool, str]:
         """
         Places a pawn on the board.
 
         Args:
@@ -355,15 +364,15 @@
         if self.is_game_over():
             return False, "The game is over."
 
         # Get the pawn of the current player
         pawn = self.get_playing_pawn()
 
         # Check if the pawn has been placed
-        if pawn.pos == (None, None):
+        if pawn.pos[0] is None or pawn.pos[1] is None:
             return False, "The pawn has not been placed yet."
 
         # Check if there is any possible move
         possible_moves = self.get_possible_movement_positions(pawn)
         if len(possible_moves) == 0:
             self.next_turn()
             return True, "There is no possible move to play, the pawn is stuck."
@@ -393,16 +402,16 @@
         # Check the input
         position_valid, reason = self.is_position_valid(build_position)
         if not position_valid:
             # Reverse the move
             pawn.move(initial_pos)
             return False, reason
 
-        # Check if there is any possible build
-        # > No need to check, it is always possible to build after a move (we can always build on the initial position)
+        # No need to check possible build, it is always possible to build after a move
+        # (we can always build on the initial position)
 
         # Check if the build is possible
         build_possible, reason = self.is_build_possible(pawn.pos, build_position)
 
         if not build_possible:
             # The move was played but the build is not possible
             # Reverse the move
```

### Comparing `SantorinAI-1.3.0/santorinai/board_displayer/board_displayer.py` & `SantorinAI-1.3.1/santorinai/board_displayer/board_displayer.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,33 +16,26 @@
 # 4: terminated tower
 
 # A list of pawns with a number and a pos.
 
 sg.theme("Dark Blue 3")
 SIZE = 5
 
-window = None
-
 pawns_colors = {
     1: "grey",
     2: "blue",
     3: "white",
 }
 
 SIZE_X = 800
 SIZE_Y = 300
 TILE_SIZE = SIZE_X / 5
 
 
 def init_window(player_names):
-    global window
-    if window is not None:
-        # window.close()
-        return window
-
     tile = player_names[0]
     for player_name in player_names[1:]:
         tile += f" VS {player_name} "
 
     layout = [
         [sg.Text(tile, font=("Helvetica", 20), justification="center")],
         [
@@ -69,14 +62,17 @@
     :param y: The y-coordinate of the cube.
     :param size: The size of the cube.
     :param color: The fill color of the cube.
     :param line_color: The color of the cube's outline.
     """
     graph = window["-GRAPH-"]
 
+    if graph is None:
+        return
+
     ratio = SIZE_X / SIZE_Y
 
     AY = y + size / ratio
     B2Y = y - size / ratio
     B1Y = B3Y = y
     C2Y = B2Y - cube_heigth
     C1Y = C3Y = B1Y - cube_heigth
```

### Comparing `SantorinAI-1.3.0/santorinai/pawn.py` & `SantorinAI-1.3.1/santorinai/pawn.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,29 @@
+from typing import Tuple
+
+
 class Pawn:
-    def __init__(self, number, player_number):
+    def __init__(self, number: int, player_number: int):
         """
         Initialize a pawn
         :param number: the number of the pawn
         :param player_number: the player number of the pawn
         """
         self.pos = (None, None)
         self.number = number
         self.player_number = player_number
 
-    def move(self, new_pos):
+    def move(self, new_pos: Tuple[int, int]):
         """
         Move the pawn to the new position
         :param new_pos: the new position of the pawn
         """
         self.pos = new_pos
 
-    def copy(self):
+    def copy(self) -> "Pawn":
         """
         Return a copy of the pawn
         :return: a copy of the pawn
         """
         new_pawn = Pawn(self.number, self.player_number)
         new_pawn.pos = self.pos
         return new_pawn
```

### Comparing `SantorinAI-1.3.0/santorinai/player_examples/basic_player.py` & `SantorinAI-1.3.1/santorinai/player_examples/basic_player.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from santorinai.player import Player
 from santorinai.board import Board
+from santorinai.pawn import Pawn
 from random import choice
 
 
 class BasicPlayer(Player):
     """
     A player that answer to simple rules:
     - Place first pawn on the first randomly
@@ -19,15 +20,15 @@
     def __init__(self, log_level=0) -> None:
         super().__init__()
         self.log_level = log_level
 
     def name(self):
         return "Extra BaThick!"
 
-    def get_ally_pawn(self, board, our_pawn):
+    def get_ally_pawn(self, board: Board, our_pawn: Pawn) -> Pawn | None:
         for pawn in board.pawns:
             if (
                 pawn.number != our_pawn.number
                 and pawn.player_number == our_pawn.player_number
             ):
                 return pawn
 
@@ -45,29 +46,38 @@
             if board.board[pos[0]][pos[1]] == 3:
                 winning_moves.append(pos)
 
         return winning_moves
 
     def place_pawn(self, board: Board, pawn):
         ally_pawn = self.get_ally_pawn(board, pawn)
-        available_positions = board.get_possible_movement_positions(pawn)
 
-        if ally_pawn.pos == (None, None):
+        available_positions = board.get_possible_movement_positions(pawn)
+        if (
+            ally_pawn is None
+            or ally_pawn.pos[0] is None
+            or ally_pawn.pos[1] is not None
+        ):
             # First pawn to place
             return choice(available_positions)
 
+        # Place second pawn next to the first one if possible
         for pos in available_positions:
             if board.is_position_adjacent(pos, ally_pawn.pos):
                 return pos
 
         return choice(available_positions)
 
     def play_move(self, board, pawn):
         available_positions = board.get_possible_movement_positions(pawn)
 
+        if pawn.pos[0] is None or pawn.pos[1] is None:
+            # Pawn is not placed yet
+            raise Exception("Pawn is not placed yet")
+
         current_level = board.board[pawn.pos[0]][pawn.pos[1]]
         best_spot = None
         best_spot_level = 0
         for pos in available_positions:
             if board.board[pos[0]][pos[1]] == 3:
                 # We can win!
                 if self.log_level:
```

### Comparing `SantorinAI-1.3.0/santorinai/player_examples/first_choice_player.py` & `SantorinAI-1.3.1/santorinai/player_examples/first_choice_player.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 from santorinai.player import Player
+from santorinai.board import Board
+from santorinai.pawn import Pawn
 
 
 class FirstChoicePlayer(Player):
     """
     A player that places his pawns and moves them at the first possible position
     """
 
     def name(self):
         return "Firsty First"
 
-    def place_pawn(self, board, pawn):
+    def place_pawn(self, board: Board, pawn: Pawn):
         available_positions = board.get_possible_movement_positions(pawn)
         my_choice = available_positions[0]
         return my_choice
 
-    def play_move(self, board, pawn):
-        my_initial_position = pawn.pos
-
+    def play_move(self, board: Board, pawn: Pawn):
         # Get movement positions
-        available_positions = board.get_possible_movement_positions(pawn)
-        if len(available_positions) == 0:
+        print(pawn)
+        print(pawn.pos)
+        available_move_positions = board.get_possible_movement_positions(pawn)
+        if len(available_move_positions) == 0:
             # The pawn cannot move
             return None, None
 
-        my_move_choice = available_positions[0]
+        my_move_choice = available_move_positions[0]
 
         # Simulate the move (this will not impact the actual board)
         pawn.move(my_move_choice)
 
         # Get construction positions
-        available_positions = board.get_possible_building_positions(pawn)
+        available_build_positions = board.get_possible_building_positions(pawn)
+        if len(available_build_positions) == 0:
+            # The pawn cannot build
+            print(available_move_positions)
+            print(available_build_positions)
+            print(board)
+            raise Exception("Pawn cannot build")
+
         # Their is always at least one position available
-        my_build_choice = available_positions[0]
+        my_build_choice = available_build_positions[0]
 
         return my_move_choice, my_build_choice
```

### Comparing `SantorinAI-1.3.0/santorinai/player_examples/random_player.py` & `SantorinAI-1.3.1/santorinai/player_examples/random_player.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 
     def place_pawn(self, board, pawn):
         available_positions = board.get_possible_movement_positions(pawn)
         my_choice = choice(available_positions)
         return my_choice
 
     def play_move(self, board, pawn):
-        my_initial_position = pawn.pos
-
         # Get movement positions
         available_positions = board.get_possible_movement_positions(pawn)
         if len(available_positions) == 0:
             # The pawn cannot move
             return None, None
 
         my_move_choice = choice(available_positions)
```

### Comparing `SantorinAI-1.3.0/santorinai/tester.py` & `SantorinAI-1.3.1/santorinai/tester.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from santorinai.player import Player
 from santorinai.board import Board
-from santorinai.board_displayer.board_displayer import init_window, update_board
+from santorinai.board_displayer.board_displayer import (
+    init_window,
+    update_board,
+    close_window,
+)
 from time import sleep
 
 
 class Tester:
     """
-    Run the games with SantorinAI playes, do statistics display the results
+    Run the games with SantorinAI players, do statistics display the results
     """
 
     verbose_level = 2
-    delay_between_moves = 0
+    delay_between_moves = 0.0
     display_board = False
 
     def display_message(self, message, verbose_level=1):
         """
         Display a message if verbose is True
 
         Args:
@@ -33,22 +37,23 @@
         """
         NB_PLAYERS = 2
         NB_PAWNS = NB_PLAYERS * 2
 
         nb_victories = [0, 0]
 
         # Check if the players are objects of the Player class
-        if not isinstance(player1, Player):
+        if player1 is None or not isinstance(player1, Player):
             raise TypeError("player1 should be an object of the Player class")
-        if not isinstance(player2, Player):
+        if player2 is None or not isinstance(player2, Player):
             raise TypeError("player2 should be an object of the Player class")
 
         players = [player1, player2]
 
         # Initialize the window
+        window = None
         if self.display_board:
             window = init_window([player1.name(), player2.name()])
 
         # Play the games
         for game_nb in range(1, nb_games + 1):
             self.display_message(f"Game {game_nb}", 1)
 
@@ -56,16 +61,20 @@
             board = Board(NB_PLAYERS)
 
             # Placement the pawns
             for pawn_nb in range(1, NB_PAWNS + 1):
                 board_copy = board.copy()
                 current_pawn = board_copy.get_playing_pawn()
 
+                # If pawn_nb == 1, the player_nb is 0, if pawn_nb == 2, the
+                # player_nb is 1, if pawn_nb == 3, the player_nb is 0, etc.
+                player_nb = (pawn_nb - 1) % NB_PLAYERS
+                player = players[player_nb]
+
                 # Ask the player where to place the pawn
-                player = players[pawn_nb % NB_PLAYERS]
                 self.display_message(
                     f"Player {player.name()} is placing pawn {pawn_nb}", 2
                 )
                 position_choice = player.place_pawn(board_copy, current_pawn)
 
                 # Place the pawn
                 success, reason = board.place_pawn(position_choice)
@@ -75,27 +84,27 @@
                         f"   Pawn placed at an invalid position: {reason}", 1
                     )
                     self.display_message(f"   Player {player.name()} loses")
                     nb_victories[(pawn_nb + 1) % NB_PLAYERS] += 1
                     break
 
                 self.display_message(f"   Pawn placed at position {position_choice}", 2)
-                if self.display_board:
+                if self.display_board and window is not None:
                     update_board(window, board)
                 sleep(self.delay_between_moves)
 
             # Play the game
-            self.display_message(f"\nPlaying the game")
+            self.display_message("\nPlaying the game")
             while not board.is_game_over():
                 current_pawn = board.get_playing_pawn()
                 self.display_message(f"   Current pawn: {current_pawn}", 2)
 
                 # Check if the player can move
                 if len(board.get_possible_movement_positions(current_pawn)) == 0:
-                    self.display_message(f"   The pawn cannot move", 2)
+                    self.display_message("   The pawn cannot move", 2)
                     board.next_turn()
                     # We don't ask the player to move, we just skip his turn
                     continue
 
                 board_copy = board.copy()
                 current_pawn_copy = board_copy.get_playing_pawn()
 
@@ -116,40 +125,47 @@
                         f"   Pawn moved at an invalid position: {reason}", 1
                     )
                     self.display_message(f"   Player {player.name()} loses")
                     nb_victories[(current_pawn.player_number) % NB_PLAYERS] += 1
                     break
 
                 self.display_message(
-                    f"   Pawn moved at position {move_choice} and built at position {build_choice}",
+                    f"   Pawn moved at position {move_choice}\
+                      and built at position {build_choice}",
                     2,
                 )
                 self.display_message(board, 2)
-                if self.display_board:
+                if window and self.display_board:
                     update_board(window, board)
                 sleep(self.delay_between_moves)
 
             # Game is over
-            winer_number = board.winner_player_number
-            if winer_number is None:
+            winner_number = board.winner_player_number
+            if winner_number is None:
                 self.display_message("Draw")
             else:
-                self.display_message(f"Player {players[winer_number - 1].name()} wins!")
-                nb_victories[winer_number - 1] += 1
+                self.display_message(
+                    f"Player {players[winner_number - 1].name()} wins!"
+                )
+                nb_victories[winner_number - 1] += 1
 
         # Display the results
-        print(f"\nResults:")
+        print("\nResults:")
         print(
             f"Player {players[0].name()} won {nb_victories[0]} times ("
             + str(round(nb_victories[0] / nb_games * 100, 2))
             + "%)"
         )
         print(
             f"Player {players[1].name()} won {nb_victories[1]} times ("
             + str(round(nb_victories[1] / nb_games * 100, 2))
             + "%)"
         )
 
+        # Close the window
+        if self.display_board:
+            close_window(window)
+
         return {
             players[0].name(): nb_victories[0],
             players[1].name(): nb_victories[1],
         }
```

### Comparing `SantorinAI-1.3.0/setup.py` & `SantorinAI-1.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="SantorinAI",
-    version="1.3.0",
+    version="1.3.1",
     author="Tom Mansion",
     author_email="tomansion@yahoo.fr",
     description="A Python library for the Santorini board game",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/tomansion/santorinai",
     packages=find_packages(),
```

### Comparing `SantorinAI-1.3.0/test/test_board.py` & `SantorinAI-1.3.1/test/test_board.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.3.0/test/test_tester.py` & `SantorinAI-1.3.1/test/test_tester.py`

 * *Files identical despite different names*

