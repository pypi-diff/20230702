# Comparing `tmp/catchem-alpha-zero-0.0.2.tar.gz` & `tmp/catchem-alpha-zero-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catchem-alpha-zero-0.0.2.tar", last modified: Sun Jul  2 01:26:44 2023, max compression
+gzip compressed data, was "catchem-alpha-zero-0.0.3.tar", last modified: Sun Jul  2 01:36:10 2023, max compression
```

## Comparing `catchem-alpha-zero-0.0.2.tar` & `catchem-alpha-zero-0.0.3.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 01:26:44.786515 catchem-alpha-zero-0.0.2/
--rw-rw-rw-   0        0        0     1087 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       20 2023-07-02 01:24:28.000000 catchem-alpha-zero-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0    14902 2023-07-02 01:26:44.786515 catchem-alpha-zero-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    14167 2023-07-02 01:15:05.000000 catchem-alpha-zero-0.0.2/README.md
--rw-rw-rw-   0        0        0      311 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0     1362 2023-07-02 01:26:44.789516 catchem-alpha-zero-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-02 01:26:44.690659 catchem-alpha-zero-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-02 01:26:44.714794 catchem-alpha-zero-0.0.2/src/catchem_alpha_zero.egg-info/
--rw-rw-rw-   0        0        0    14902 2023-07-02 01:26:44.000000 catchem-alpha-zero-0.0.2/src/catchem_alpha_zero.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2019 2023-07-02 01:26:44.000000 catchem-alpha-zero-0.0.2/src/catchem_alpha_zero.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 01:26:44.000000 catchem-alpha-zero-0.0.2/src/catchem_alpha_zero.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-07-02 01:26:44.000000 catchem-alpha-zero-0.0.2/src/catchem_alpha_zero.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      160 2023-07-02 01:26:44.000000 catchem-alpha-zero-0.0.2/src/catchem_alpha_zero.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-02 01:26:44.000000 catchem-alpha-zero-0.0.2/src/catchem_alpha_zero.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-02 01:26:44.726574 catchem-alpha-zero-0.0.2/src/caz/
--rw-rw-rw-   0        0        0        0 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/__init__.py
--rw-rw-rw-   0        0        0       75 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 01:26:44.737410 catchem-alpha-zero-0.0.2/src/caz/alpha_zero/
--rw-rw-rw-   0        0        0      606 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/alpha_zero/__init__.py
--rw-rw-rw-   0        0        0    16195 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/alpha_zero/alpha_zero.py
--rw-rw-rw-   0        0        0    11234 2023-07-01 16:12:31.000000 catchem-alpha-zero-0.0.2/src/caz/alpha_zero/alpha_zero_mcts.py
--rw-rw-rw-   0        0        0     5620 2023-06-19 23:03:45.000000 catchem-alpha-zero-0.0.2/src/caz/alpha_zero/alpha_zero_parameters.py
--rw-rw-rw-   0        0        0      565 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/alpha_zero/alpha_zero_training_models.py
--rw-rw-rw-   0        0        0     1638 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/alpha_zero/network.py
--rw-rw-rw-   0        0        0    12738 2023-06-22 18:59:16.000000 catchem-alpha-zero-0.0.2/src/caz/alpha_zero/network_torch.py
--rw-rw-rw-   0        0        0     1296 2023-07-01 16:37:59.000000 catchem-alpha-zero-0.0.2/src/caz/alpha_zero/retrainer.py
--rw-rw-rw-   0        0        0     4734 2023-07-01 16:37:55.000000 catchem-alpha-zero-0.0.2/src/caz/alpha_zero/supervised_learning.py
--rw-rw-rw-   0        0        0      549 2023-06-20 22:58:18.000000 catchem-alpha-zero-0.0.2/src/caz/app.py
--rw-rw-rw-   0        0        0      791 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/async_utils.py
--rw-rw-rw-   0        0        0     1434 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/bitboard_utils.py
--rw-rw-rw-   0        0        0     5034 2023-06-19 22:51:48.000000 catchem-alpha-zero-0.0.2/src/caz/cli.py
-drwxrwxrwx   0        0        0        0 2023-07-02 01:26:44.741479 catchem-alpha-zero-0.0.2/src/caz/games/
--rw-rw-rw-   0        0        0      233 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/games/__init__.py
--rw-rw-rw-   0        0        0     8078 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/games/game.py
--rw-rw-rw-   0        0        0      975 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/games/game_type.py
--rw-rw-rw-   0        0        0      833 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/graph.py
-drwxrwxrwx   0        0        0        0 2023-07-02 01:26:44.760573 catchem-alpha-zero-0.0.2/src/caz/images/
--rw-rw-rw-   0        0        0        0 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/images/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 01:26:44.761586 catchem-alpha-zero-0.0.2/src/caz/images/__pycache__/
--rw-rw-rw-   0        0        0      180 2023-06-19 22:45:56.000000 catchem-alpha-zero-0.0.2/src/caz/images/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     1260 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/images/black-bishop.png
--rw-rw-rw-   0        0        0     2485 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/images/black-king.png
--rw-rw-rw-   0        0        0     1516 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/images/black-knight.png
--rw-rw-rw-   0        0        0      797 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/images/black-pawn.png
--rw-rw-rw-   0        0        0     2267 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/images/black-queen.png
--rw-rw-rw-   0        0        0      725 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/images/black-rook.png
--rw-rw-rw-   0        0        0    23865 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/images/caz_flat_logo.png
--rw-rw-rw-   0        0        0   138365 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/images/caz_splashscreen.jpg
--rw-rw-rw-   0        0        0    67646 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/images/tiny_chess.ico
--rw-rw-rw-   0        0        0     1944 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/images/white-bishop.png
--rw-rw-rw-   0        0        0     2279 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/images/white-king.png
--rw-rw-rw-   0        0        0     1878 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/images/white-knight.png
--rw-rw-rw-   0        0        0     1294 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/images/white-pawn.png
--rw-rw-rw-   0        0        0     2637 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/images/white-queen.png
--rw-rw-rw-   0        0        0      933 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/images/white-rook.png
--rw-rw-rw-   0        0        0     2953 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/kaggle_sandbox.py
--rw-rw-rw-   0        0        0      203 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/kaggle_types.py
-drwxrwxrwx   0        0        0        0 2023-07-02 01:26:44.767590 catchem-alpha-zero-0.0.2/src/caz/solvers/
--rw-rw-rw-   0        0        0       86 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/solvers/__init__.py
--rw-rw-rw-   0        0        0     1797 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/solvers/agent_type.py
--rw-rw-rw-   0        0        0     3446 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/solvers/mcts.py
--rw-rw-rw-   0        0        0      932 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/solvers/minimax.py
--rw-rw-rw-   0        0        0      184 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/solvers/solver.py
-drwxrwxrwx   0        0        0        0 2023-07-02 01:26:44.774980 catchem-alpha-zero-0.0.2/src/caz/states/
--rw-rw-rw-   0        0        0      300 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/states/__init__.py
--rw-rw-rw-   0        0        0    11334 2023-06-19 23:54:49.000000 catchem-alpha-zero-0.0.2/src/caz/states/chess.py
--rw-rw-rw-   0        0        0    18449 2023-06-22 18:59:16.000000 catchem-alpha-zero-0.0.2/src/caz/states/chess_enums.py
--rw-rw-rw-   0        0        0     8959 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/states/connectx.py
--rw-rw-rw-   0        0        0     2430 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/states/state.py
--rw-rw-rw-   0        0        0     5475 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/states/tictactoe.py
--rw-rw-rw-   0        0        0     7687 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/sumplete_solver.py
-drwxrwxrwx   0        0        0        0 2023-07-02 01:26:44.784516 catchem-alpha-zero-0.0.2/src/caz/views/
--rw-rw-rw-   0        0        0       32 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/views/__init__.py
--rw-rw-rw-   0        0        0    20923 2023-07-02 01:15:12.000000 catchem-alpha-zero-0.0.2/src/caz/views/chess_detail.py
--rw-rw-rw-   0        0        0     5417 2023-07-02 01:14:51.000000 catchem-alpha-zero-0.0.2/src/caz/views/chess_main.py
--rw-rw-rw-   0        0        0     1646 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/views/console.py
--rw-rw-rw-   0        0        0     5610 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/views/html.py
--rw-rw-rw-   0        0        0     3692 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/views/plot.py
--rw-rw-rw-   0        0        0     2022 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/views/policies.py
--rw-rw-rw-   0        0        0      216 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.2/src/caz/views/view.py
-drwxrwxrwx   0        0        0        0 2023-07-02 01:26:44.785516 catchem-alpha-zero-0.0.2/tests/
--rw-rw-rw-   0        0        0     2017 2023-07-01 16:11:29.000000 catchem-alpha-zero-0.0.2/tests/test_chess.py
+drwxrwxrwx   0        0        0        0 2023-07-02 01:36:10.951942 catchem-alpha-zero-0.0.3/
+-rw-rw-rw-   0        0        0     1087 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       20 2023-07-02 01:24:28.000000 catchem-alpha-zero-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    14902 2023-07-02 01:36:10.952942 catchem-alpha-zero-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    14167 2023-07-02 01:15:05.000000 catchem-alpha-zero-0.0.3/README.md
+-rw-rw-rw-   0        0        0      311 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1370 2023-07-02 01:36:10.953943 catchem-alpha-zero-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-02 01:36:10.861776 catchem-alpha-zero-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-02 01:36:10.888290 catchem-alpha-zero-0.0.3/src/catchem_alpha_zero.egg-info/
+-rw-rw-rw-   0        0        0    14902 2023-07-02 01:36:10.000000 catchem-alpha-zero-0.0.3/src/catchem_alpha_zero.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2019 2023-07-02 01:36:10.000000 catchem-alpha-zero-0.0.3/src/catchem_alpha_zero.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 01:36:10.000000 catchem-alpha-zero-0.0.3/src/catchem_alpha_zero.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-07-02 01:36:10.000000 catchem-alpha-zero-0.0.3/src/catchem_alpha_zero.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      160 2023-07-02 01:36:10.000000 catchem-alpha-zero-0.0.3/src/catchem_alpha_zero.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-02 01:36:10.000000 catchem-alpha-zero-0.0.3/src/catchem_alpha_zero.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 01:36:10.900467 catchem-alpha-zero-0.0.3/src/caz/
+-rw-rw-rw-   0        0        0        0 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/__init__.py
+-rw-rw-rw-   0        0        0       75 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 01:36:10.909469 catchem-alpha-zero-0.0.3/src/caz/alpha_zero/
+-rw-rw-rw-   0        0        0      606 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/alpha_zero/__init__.py
+-rw-rw-rw-   0        0        0    16195 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/alpha_zero/alpha_zero.py
+-rw-rw-rw-   0        0        0    11234 2023-07-01 16:12:31.000000 catchem-alpha-zero-0.0.3/src/caz/alpha_zero/alpha_zero_mcts.py
+-rw-rw-rw-   0        0        0     5620 2023-06-19 23:03:45.000000 catchem-alpha-zero-0.0.3/src/caz/alpha_zero/alpha_zero_parameters.py
+-rw-rw-rw-   0        0        0      565 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/alpha_zero/alpha_zero_training_models.py
+-rw-rw-rw-   0        0        0     1638 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/alpha_zero/network.py
+-rw-rw-rw-   0        0        0    12738 2023-06-22 18:59:16.000000 catchem-alpha-zero-0.0.3/src/caz/alpha_zero/network_torch.py
+-rw-rw-rw-   0        0        0     1296 2023-07-01 16:37:59.000000 catchem-alpha-zero-0.0.3/src/caz/alpha_zero/retrainer.py
+-rw-rw-rw-   0        0        0     4734 2023-07-01 16:37:55.000000 catchem-alpha-zero-0.0.3/src/caz/alpha_zero/supervised_learning.py
+-rw-rw-rw-   0        0        0      549 2023-06-20 22:58:18.000000 catchem-alpha-zero-0.0.3/src/caz/app.py
+-rw-rw-rw-   0        0        0      791 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/async_utils.py
+-rw-rw-rw-   0        0        0     1434 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/bitboard_utils.py
+-rw-rw-rw-   0        0        0     5034 2023-06-19 22:51:48.000000 catchem-alpha-zero-0.0.3/src/caz/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-02 01:36:10.912594 catchem-alpha-zero-0.0.3/src/caz/games/
+-rw-rw-rw-   0        0        0      233 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/games/__init__.py
+-rw-rw-rw-   0        0        0     8078 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/games/game.py
+-rw-rw-rw-   0        0        0      975 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/games/game_type.py
+-rw-rw-rw-   0        0        0      833 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/graph.py
+drwxrwxrwx   0        0        0        0 2023-07-02 01:36:10.929269 catchem-alpha-zero-0.0.3/src/caz/images/
+-rw-rw-rw-   0        0        0        0 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 01:36:10.930760 catchem-alpha-zero-0.0.3/src/caz/images/__pycache__/
+-rw-rw-rw-   0        0        0      180 2023-06-19 22:45:56.000000 catchem-alpha-zero-0.0.3/src/caz/images/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1260 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/black-bishop.png
+-rw-rw-rw-   0        0        0     2485 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/black-king.png
+-rw-rw-rw-   0        0        0     1516 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/black-knight.png
+-rw-rw-rw-   0        0        0      797 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/black-pawn.png
+-rw-rw-rw-   0        0        0     2267 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/black-queen.png
+-rw-rw-rw-   0        0        0      725 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/black-rook.png
+-rw-rw-rw-   0        0        0    23865 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/caz_flat_logo.png
+-rw-rw-rw-   0        0        0   138365 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/caz_splashscreen.jpg
+-rw-rw-rw-   0        0        0    67646 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/tiny_chess.ico
+-rw-rw-rw-   0        0        0     1944 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/white-bishop.png
+-rw-rw-rw-   0        0        0     2279 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/white-king.png
+-rw-rw-rw-   0        0        0     1878 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/white-knight.png
+-rw-rw-rw-   0        0        0     1294 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/white-pawn.png
+-rw-rw-rw-   0        0        0     2637 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/white-queen.png
+-rw-rw-rw-   0        0        0      933 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/white-rook.png
+-rw-rw-rw-   0        0        0     2953 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/kaggle_sandbox.py
+-rw-rw-rw-   0        0        0      203 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/kaggle_types.py
+drwxrwxrwx   0        0        0        0 2023-07-02 01:36:10.935761 catchem-alpha-zero-0.0.3/src/caz/solvers/
+-rw-rw-rw-   0        0        0       86 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/solvers/__init__.py
+-rw-rw-rw-   0        0        0     1797 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/solvers/agent_type.py
+-rw-rw-rw-   0        0        0     3446 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/solvers/mcts.py
+-rw-rw-rw-   0        0        0      932 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/solvers/minimax.py
+-rw-rw-rw-   0        0        0      184 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/solvers/solver.py
+drwxrwxrwx   0        0        0        0 2023-07-02 01:36:10.942325 catchem-alpha-zero-0.0.3/src/caz/states/
+-rw-rw-rw-   0        0        0      300 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/states/__init__.py
+-rw-rw-rw-   0        0        0    11334 2023-06-19 23:54:49.000000 catchem-alpha-zero-0.0.3/src/caz/states/chess.py
+-rw-rw-rw-   0        0        0    18449 2023-06-22 18:59:16.000000 catchem-alpha-zero-0.0.3/src/caz/states/chess_enums.py
+-rw-rw-rw-   0        0        0     8959 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/states/connectx.py
+-rw-rw-rw-   0        0        0     2430 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/states/state.py
+-rw-rw-rw-   0        0        0     5475 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/states/tictactoe.py
+-rw-rw-rw-   0        0        0     7687 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/sumplete_solver.py
+drwxrwxrwx   0        0        0        0 2023-07-02 01:36:10.949828 catchem-alpha-zero-0.0.3/src/caz/views/
+-rw-rw-rw-   0        0        0       32 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/views/__init__.py
+-rw-rw-rw-   0        0        0    20923 2023-07-02 01:15:12.000000 catchem-alpha-zero-0.0.3/src/caz/views/chess_detail.py
+-rw-rw-rw-   0        0        0     5555 2023-07-02 01:33:24.000000 catchem-alpha-zero-0.0.3/src/caz/views/chess_main.py
+-rw-rw-rw-   0        0        0     1646 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/views/console.py
+-rw-rw-rw-   0        0        0     5610 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/views/html.py
+-rw-rw-rw-   0        0        0     3692 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/views/plot.py
+-rw-rw-rw-   0        0        0     2022 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/views/policies.py
+-rw-rw-rw-   0        0        0      216 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/views/view.py
+drwxrwxrwx   0        0        0        0 2023-07-02 01:36:10.950940 catchem-alpha-zero-0.0.3/tests/
+-rw-rw-rw-   0        0        0     2017 2023-07-01 16:11:29.000000 catchem-alpha-zero-0.0.3/tests/test_chess.py
```

### Comparing `catchem-alpha-zero-0.0.2/LICENSE` & `catchem-alpha-zero-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/PKG-INFO` & `catchem-alpha-zero-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catchem-alpha-zero
-Version: 0.0.2
+Version: 0.0.3
 Summary: CatchemAlphaZero: AI techniques for solving games
 Home-page: https://github.com/CatchemAL/CatchemAlphaZero
 Author: Alex Cross
 Author-email: AlexJCross90@gmail.com
 Project-URL: Bug Tracker, https://github.com/CatchemAL/CatchemAlphaZero/issues
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `catchem-alpha-zero-0.0.2/README.md` & `catchem-alpha-zero-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/setup.cfg` & `catchem-alpha-zero-0.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6174 6368 656d 2d61 6c70 6861   = catchem-alpha
 00000020: 2d7a 6572 6f0d 0a76 6572 7369 6f6e 203d  -zero..version =
-00000030: 2030 2e30 2e32 0d0a 6175 7468 6f72 203d   0.0.2..author =
+00000030: 2030 2e30 2e33 0d0a 6175 7468 6f72 203d   0.0.3..author =
 00000040: 2041 6c65 7820 4372 6f73 730d 0a61 7574   Alex Cross..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 416c 6578  hor_email = Alex
 00000060: 4a43 726f 7373 3930 4067 6d61 696c 2e63  JCross90@gmail.c
 00000070: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
 00000080: 3d20 4361 7463 6865 6d41 6c70 6861 5a65  = CatchemAlphaZe
 00000090: 726f 3a20 4149 2074 6563 686e 6971 7565  ro: AI technique
 000000a0: 7320 666f 7220 736f 6c76 696e 6720 6761  s for solving ga
@@ -56,31 +56,31 @@
 00000370: 0a09 6b61 6767 6c65 2d65 6e76 6972 6f6e  ..kaggle-environ
 00000380: 6d65 6e74 730d 0a0d 0a5b 6f70 7469 6f6e  ments....[option
 00000390: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
 000003a0: 0d0a 7768 6572 6520 3d20 7372 630d 0a0d  ..where = src...
 000003b0: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
 000003c0: 655f 6461 7461 5d0d 0a63 617a 2e69 6d61  e_data]..caz.ima
 000003d0: 6765 7320 3d20 0d0a 092a 2e70 6e67 0d0a  ges = ...*.png..
-000003e0: 092a 2e69 636f 0d0a 0d0a 5b6f 7074 696f  .*.ico....[optio
-000003f0: 6e73 2e65 6e74 7279 5f70 6f69 6e74 735d  ns.entry_points]
-00000400: 0d0a 636f 6e73 6f6c 655f 7363 7269 7074  ..console_script
-00000410: 7320 3d20 0d0a 0963 617a 203d 2063 617a  s = ...caz = caz
-00000420: 2e63 6c69 3a6d 6169 6e0d 0a67 7569 5f73  .cli:main..gui_s
-00000430: 6372 6970 7473 203d 200d 0a09 616c 7068  cripts = ...alph
-00000440: 6120 3d20 6361 7a2e 6170 703a 6c61 756e  a = caz.app:laun
-00000450: 6368 0d0a 0d0a 5b6f 7074 696f 6e73 2e65  ch....[options.e
-00000460: 7874 7261 735f 7265 7175 6972 655d 0d0a  xtras_require]..
-00000470: 6465 7620 3d20 0d0a 0962 6c61 636b 0d0a  dev = ...black..
-00000480: 0966 6c61 6b65 380d 0a09 6973 6f72 740d  .flake8...isort.
-00000490: 0a09 6d79 7079 0d0a 0970 7974 6573 740d  ..mypy...pytest.
-000004a0: 0a0d 0a5b 666c 616b 6538 5d0d 0a69 676e  ...[flake8]..ign
-000004b0: 6f72 6520 3d20 0d0a 0945 3230 330d 0a09  ore = ...E203...
-000004c0: 5735 3033 0d0a 6578 7465 6e64 2d65 7863  W503..extend-exc
-000004d0: 6c75 6465 203d 202e 7665 6e76 2f2a 2e70  lude = .venv/*.p
-000004e0: 792c 2e74 6f78 2f2a 2e70 792c 7465 7374  y,.tox/*.py,test
-000004f0: 732f 2a2e 7079 0d0a 6669 6c65 6e61 6d65  s/*.py..filename
-00000500: 203d 202e 2f73 7263 2f2a 2e70 790d 0a6d   = ./src/*.py..m
-00000510: 6178 2d6c 696e 652d 6c65 6e67 7468 203d  ax-line-length =
-00000520: 2031 3035 0d0a 0d0a 5b65 6767 5f69 6e66   105....[egg_inf
-00000530: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-00000540: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-00000550: 0d0a                                     ..
+000003e0: 092a 2e6a 7067 0d0a 092a 2e69 636f 0d0a  .*.jpg...*.ico..
+000003f0: 0d0a 5b6f 7074 696f 6e73 2e65 6e74 7279  ..[options.entry
+00000400: 5f70 6f69 6e74 735d 0d0a 636f 6e73 6f6c  _points]..consol
+00000410: 655f 7363 7269 7074 7320 3d20 0d0a 0963  e_scripts = ...c
+00000420: 617a 203d 2063 617a 2e63 6c69 3a6d 6169  az = caz.cli:mai
+00000430: 6e0d 0a67 7569 5f73 6372 6970 7473 203d  n..gui_scripts =
+00000440: 200d 0a09 616c 7068 6120 3d20 6361 7a2e   ...alpha = caz.
+00000450: 6170 703a 6c61 756e 6368 0d0a 0d0a 5b6f  app:launch....[o
+00000460: 7074 696f 6e73 2e65 7874 7261 735f 7265  ptions.extras_re
+00000470: 7175 6972 655d 0d0a 6465 7620 3d20 0d0a  quire]..dev = ..
+00000480: 0962 6c61 636b 0d0a 0966 6c61 6b65 380d  .black...flake8.
+00000490: 0a09 6973 6f72 740d 0a09 6d79 7079 0d0a  ..isort...mypy..
+000004a0: 0970 7974 6573 740d 0a0d 0a5b 666c 616b  .pytest....[flak
+000004b0: 6538 5d0d 0a69 676e 6f72 6520 3d20 0d0a  e8]..ignore = ..
+000004c0: 0945 3230 330d 0a09 5735 3033 0d0a 6578  .E203...W503..ex
+000004d0: 7465 6e64 2d65 7863 6c75 6465 203d 202e  tend-exclude = .
+000004e0: 7665 6e76 2f2a 2e70 792c 2e74 6f78 2f2a  venv/*.py,.tox/*
+000004f0: 2e70 792c 7465 7374 732f 2a2e 7079 0d0a  .py,tests/*.py..
+00000500: 6669 6c65 6e61 6d65 203d 202e 2f73 7263  filename = ./src
+00000510: 2f2a 2e70 790d 0a6d 6178 2d6c 696e 652d  /*.py..max-line-
+00000520: 6c65 6e67 7468 203d 2031 3035 0d0a 0d0a  length = 105....
+00000530: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
+00000540: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
+00000550: 7465 203d 2030 0d0a 0d0a                 te = 0....
```

### Comparing `catchem-alpha-zero-0.0.2/src/catchem_alpha_zero.egg-info/PKG-INFO` & `catchem-alpha-zero-0.0.3/src/catchem_alpha_zero.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catchem-alpha-zero
-Version: 0.0.2
+Version: 0.0.3
 Summary: CatchemAlphaZero: AI techniques for solving games
 Home-page: https://github.com/CatchemAL/CatchemAlphaZero
 Author: Alex Cross
 Author-email: AlexJCross90@gmail.com
 Project-URL: Bug Tracker, https://github.com/CatchemAL/CatchemAlphaZero/issues
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `catchem-alpha-zero-0.0.2/src/catchem_alpha_zero.egg-info/SOURCES.txt` & `catchem-alpha-zero-0.0.3/src/catchem_alpha_zero.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/alpha_zero/__init__.py` & `catchem-alpha-zero-0.0.3/src/caz/alpha_zero/__init__.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/alpha_zero/alpha_zero.py` & `catchem-alpha-zero-0.0.3/src/caz/alpha_zero/alpha_zero.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/alpha_zero/alpha_zero_mcts.py` & `catchem-alpha-zero-0.0.3/src/caz/alpha_zero/alpha_zero_mcts.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/alpha_zero/alpha_zero_parameters.py` & `catchem-alpha-zero-0.0.3/src/caz/alpha_zero/alpha_zero_parameters.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/alpha_zero/alpha_zero_training_models.py` & `catchem-alpha-zero-0.0.3/src/caz/alpha_zero/alpha_zero_training_models.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/alpha_zero/network.py` & `catchem-alpha-zero-0.0.3/src/caz/alpha_zero/network.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/alpha_zero/network_torch.py` & `catchem-alpha-zero-0.0.3/src/caz/alpha_zero/network_torch.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/alpha_zero/retrainer.py` & `catchem-alpha-zero-0.0.3/src/caz/alpha_zero/retrainer.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/alpha_zero/supervised_learning.py` & `catchem-alpha-zero-0.0.3/src/caz/alpha_zero/supervised_learning.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/app.py` & `catchem-alpha-zero-0.0.3/src/caz/app.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/async_utils.py` & `catchem-alpha-zero-0.0.3/src/caz/async_utils.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/bitboard_utils.py` & `catchem-alpha-zero-0.0.3/src/caz/bitboard_utils.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/cli.py` & `catchem-alpha-zero-0.0.3/src/caz/cli.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/games/game.py` & `catchem-alpha-zero-0.0.3/src/caz/games/game.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/games/game_type.py` & `catchem-alpha-zero-0.0.3/src/caz/games/game_type.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/graph.py` & `catchem-alpha-zero-0.0.3/src/caz/graph.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/images/black-bishop.png` & `catchem-alpha-zero-0.0.3/src/caz/images/black-bishop.png`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/images/black-king.png` & `catchem-alpha-zero-0.0.3/src/caz/images/black-king.png`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/images/black-knight.png` & `catchem-alpha-zero-0.0.3/src/caz/images/black-knight.png`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/images/black-pawn.png` & `catchem-alpha-zero-0.0.3/src/caz/images/black-pawn.png`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/images/black-queen.png` & `catchem-alpha-zero-0.0.3/src/caz/images/black-queen.png`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/images/black-rook.png` & `catchem-alpha-zero-0.0.3/src/caz/images/black-rook.png`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/images/caz_flat_logo.png` & `catchem-alpha-zero-0.0.3/src/caz/images/caz_flat_logo.png`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/images/caz_splashscreen.jpg` & `catchem-alpha-zero-0.0.3/src/caz/images/caz_splashscreen.jpg`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/images/tiny_chess.ico` & `catchem-alpha-zero-0.0.3/src/caz/images/tiny_chess.ico`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/images/white-bishop.png` & `catchem-alpha-zero-0.0.3/src/caz/images/white-bishop.png`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/images/white-king.png` & `catchem-alpha-zero-0.0.3/src/caz/images/white-king.png`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/images/white-knight.png` & `catchem-alpha-zero-0.0.3/src/caz/images/white-knight.png`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/images/white-pawn.png` & `catchem-alpha-zero-0.0.3/src/caz/images/white-pawn.png`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/images/white-queen.png` & `catchem-alpha-zero-0.0.3/src/caz/images/white-queen.png`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/images/white-rook.png` & `catchem-alpha-zero-0.0.3/src/caz/images/white-rook.png`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/kaggle_sandbox.py` & `catchem-alpha-zero-0.0.3/src/caz/kaggle_sandbox.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/solvers/agent_type.py` & `catchem-alpha-zero-0.0.3/src/caz/solvers/agent_type.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/solvers/mcts.py` & `catchem-alpha-zero-0.0.3/src/caz/solvers/mcts.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/solvers/minimax.py` & `catchem-alpha-zero-0.0.3/src/caz/solvers/minimax.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/states/chess.py` & `catchem-alpha-zero-0.0.3/src/caz/states/chess.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/states/chess_enums.py` & `catchem-alpha-zero-0.0.3/src/caz/states/chess_enums.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/states/connectx.py` & `catchem-alpha-zero-0.0.3/src/caz/states/connectx.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/states/state.py` & `catchem-alpha-zero-0.0.3/src/caz/states/state.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/states/tictactoe.py` & `catchem-alpha-zero-0.0.3/src/caz/states/tictactoe.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/sumplete_solver.py` & `catchem-alpha-zero-0.0.3/src/caz/sumplete_solver.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/views/chess_detail.py` & `catchem-alpha-zero-0.0.3/src/caz/views/chess_detail.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/views/chess_main.py` & `catchem-alpha-zero-0.0.3/src/caz/views/chess_main.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,29 +26,33 @@
         self.loop = event_loop
         self.is_open = True
         self.title("CatchemAlphaZero")
         self.resizable(False, False)
         self.current_screen = None
         self.protocol("WM_DELETE_WINDOW", self.raise_exit_flag)
 
-        logging.info("Loading Torch weights.")
+        logging.info("Loading Torch weights...")
         network = PytorchNeuralNetwork.create(game, ".")
         alpha_zero = AlphaZero(network)
         model = ChessScreenModel(alpha_zero, chess.BLACK)
 
+        logging.info("Loading screens...")
         self.title_screen = TitleScreen(self, self.switch_to_game_screen)
         self.game_screen = ChessScreen(self, self.switch_to_title_screen)
         self.game_controller = ChessScreenController(model, self.game_screen)
 
         self.switch_to_title_screen()
         self.create_menu()
 
+        logging.info("Loading icon...")
         with resources.path("caz.images", "tiny_chess.ico") as icon_path:
             self.iconbitmap(icon_path)
 
+        logging.info("Initialization complete")
+
     async def show_async(self):
         while self.is_open:
             self.update()
             await asyncio.sleep(REFRESH_RATE)
 
     def raise_exit_flag(self):
         self.is_open = False
```

### Comparing `catchem-alpha-zero-0.0.2/src/caz/views/console.py` & `catchem-alpha-zero-0.0.3/src/caz/views/console.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/views/html.py` & `catchem-alpha-zero-0.0.3/src/caz/views/html.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/views/plot.py` & `catchem-alpha-zero-0.0.3/src/caz/views/plot.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/src/caz/views/policies.py` & `catchem-alpha-zero-0.0.3/src/caz/views/policies.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.2/tests/test_chess.py` & `catchem-alpha-zero-0.0.3/tests/test_chess.py`

 * *Files identical despite different names*

