# Comparing `tmp/SantorinAI-1.3.2.tar.gz` & `tmp/SantorinAI-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SantorinAI-1.3.2.tar", last modified: Sun Jul  2 19:37:27 2023, max compression
+gzip compressed data, was "SantorinAI-1.3.3.tar", last modified: Sun Jul  2 19:51:31 2023, max compression
```

## Comparing `SantorinAI-1.3.2.tar` & `SantorinAI-1.3.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:37:27.556893 SantorinAI-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-07-02 19:37:27.556893 SantorinAI-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:37:27.556893 SantorinAI-1.3.2/SantorinAI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-07-02 19:37:27.000000 SantorinAI-1.3.2/SantorinAI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-02 19:37:27.000000 SantorinAI-1.3.2/SantorinAI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 19:37:27.000000 SantorinAI-1.3.2/SantorinAI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-02 19:37:27.000000 SantorinAI-1.3.2/SantorinAI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-02 19:37:27.000000 SantorinAI-1.3.2/SantorinAI.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:37:27.556893 SantorinAI-1.3.2/santorinai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/santorinai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18503 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/santorinai/board.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:37:27.556893 SantorinAI-1.3.2/santorinai/board_displayer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/santorinai/board_displayer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/santorinai/board_displayer/board_displayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/santorinai/pawn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/santorinai/player.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:37:27.556893 SantorinAI-1.3.2/santorinai/player_examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/santorinai/player_examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/santorinai/player_examples/basic_player.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/santorinai/player_examples/first_choice_player.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/santorinai/player_examples/random_player.py
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/santorinai/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-02 19:37:27.556893 SantorinAI-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:37:27.556893 SantorinAI-1.3.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21019 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/test/test_board.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-02 19:37:20.000000 SantorinAI-1.3.2/test/test_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:51:31.916816 SantorinAI-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-02 19:51:21.000000 SantorinAI-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-07-02 19:51:31.916816 SantorinAI-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-02 19:51:21.000000 SantorinAI-1.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:51:31.912816 SantorinAI-1.3.3/SantorinAI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-07-02 19:51:31.000000 SantorinAI-1.3.3/SantorinAI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-02 19:51:31.000000 SantorinAI-1.3.3/SantorinAI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 19:51:31.000000 SantorinAI-1.3.3/SantorinAI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-02 19:51:31.000000 SantorinAI-1.3.3/SantorinAI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-02 19:51:31.000000 SantorinAI-1.3.3/SantorinAI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:51:31.912816 SantorinAI-1.3.3/santorinai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:51:21.000000 SantorinAI-1.3.3/santorinai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18503 2023-07-02 19:51:21.000000 SantorinAI-1.3.3/santorinai/board.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:51:31.912816 SantorinAI-1.3.3/santorinai/board_displayer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:51:21.000000 SantorinAI-1.3.3/santorinai/board_displayer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-07-02 19:51:21.000000 SantorinAI-1.3.3/santorinai/board_displayer/board_displayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-02 19:51:21.000000 SantorinAI-1.3.3/santorinai/pawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-02 19:51:21.000000 SantorinAI-1.3.3/santorinai/player.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:51:31.916816 SantorinAI-1.3.3/santorinai/player_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:51:21.000000 SantorinAI-1.3.3/santorinai/player_examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-02 19:51:21.000000 SantorinAI-1.3.3/santorinai/player_examples/basic_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-02 19:51:21.000000 SantorinAI-1.3.3/santorinai/player_examples/first_choice_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-02 19:51:21.000000 SantorinAI-1.3.3/santorinai/player_examples/random_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-07-02 19:51:21.000000 SantorinAI-1.3.3/santorinai/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-02 19:51:31.916816 SantorinAI-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-02 19:51:21.000000 SantorinAI-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:51:31.916816 SantorinAI-1.3.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:51:21.000000 SantorinAI-1.3.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21019 2023-07-02 19:51:21.000000 SantorinAI-1.3.3/test/test_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-02 19:51:21.000000 SantorinAI-1.3.3/test/test_tester.py
```

### Comparing `SantorinAI-1.3.2/LICENSE` & `SantorinAI-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.3.2/PKG-INFO` & `SantorinAI-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SantorinAI
-Version: 1.3.2
+Version: 1.3.3
 Summary: A Python library for the Santorini board game
 Home-page: https://github.com/tomansion/santorinai
 Author: Tom Mansion
 Author-email: tomansion@yahoo.fr
 Keywords: santorini,ai,boardgame
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `SantorinAI-1.3.2/README.md` & `SantorinAI-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.3.2/SantorinAI.egg-info/PKG-INFO` & `SantorinAI-1.3.3/SantorinAI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SantorinAI
-Version: 1.3.2
+Version: 1.3.3
 Summary: A Python library for the Santorini board game
 Home-page: https://github.com/tomansion/santorinai
 Author: Tom Mansion
 Author-email: tomansion@yahoo.fr
 Keywords: santorini,ai,boardgame
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `SantorinAI-1.3.2/SantorinAI.egg-info/SOURCES.txt` & `SantorinAI-1.3.3/SantorinAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.3.2/santorinai/board.py` & `SantorinAI-1.3.3/santorinai/board.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.3.2/santorinai/board_displayer/board_displayer.py` & `SantorinAI-1.3.3/santorinai/board_displayer/board_displayer.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.3.2/santorinai/pawn.py` & `SantorinAI-1.3.3/santorinai/pawn.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.3.2/santorinai/player.py` & `SantorinAI-1.3.3/santorinai/player.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.3.2/santorinai/player_examples/basic_player.py` & `SantorinAI-1.3.3/santorinai/player_examples/basic_player.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.3.2/santorinai/player_examples/first_choice_player.py` & `SantorinAI-1.3.3/santorinai/player_examples/first_choice_player.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,32 +14,27 @@
     def place_pawn(self, board: Board, pawn: Pawn):
         available_positions = board.get_possible_movement_positions(pawn)
         my_choice = available_positions[0]
         return my_choice
 
     def play_move(self, board: Board, pawn: Pawn):
         # Get movement positions
-        print(pawn)
-        print(pawn.pos)
         available_move_positions = board.get_possible_movement_positions(pawn)
         if len(available_move_positions) == 0:
             # The pawn cannot move
             return None, None
 
         my_move_choice = available_move_positions[0]
 
         # Simulate the move (this will not impact the actual board)
         pawn.move(my_move_choice)
 
         # Get construction positions
         available_build_positions = board.get_possible_building_positions(pawn)
         if len(available_build_positions) == 0:
             # The pawn cannot build
-            print(available_move_positions)
-            print(available_build_positions)
-            print(board)
             raise Exception("Pawn cannot build")
 
         # Their is always at least one position available
         my_build_choice = available_build_positions[0]
 
         return my_move_choice, my_build_choice
```

### Comparing `SantorinAI-1.3.2/santorinai/player_examples/random_player.py` & `SantorinAI-1.3.3/santorinai/player_examples/random_player.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.3.2/santorinai/tester.py` & `SantorinAI-1.3.3/santorinai/tester.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.3.2/setup.py` & `SantorinAI-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="SantorinAI",
-    version="1.3.2",
+    version="1.3.3",
     author="Tom Mansion",
     author_email="tomansion@yahoo.fr",
     description="A Python library for the Santorini board game",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/tomansion/santorinai",
     packages=find_packages(),
```

### Comparing `SantorinAI-1.3.2/test/test_board.py` & `SantorinAI-1.3.3/test/test_board.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.3.2/test/test_tester.py` & `SantorinAI-1.3.3/test/test_tester.py`

 * *Files identical despite different names*

