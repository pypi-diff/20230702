# Comparing `tmp/catchem-alpha-zero-0.0.3.tar.gz` & `tmp/catchem-alpha-zero-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catchem-alpha-zero-0.0.3.tar", last modified: Sun Jul  2 01:36:10 2023, max compression
+gzip compressed data, was "catchem-alpha-zero-0.0.4.tar", last modified: Sun Jul  2 02:18:15 2023, max compression
```

## Comparing `catchem-alpha-zero-0.0.3.tar` & `catchem-alpha-zero-0.0.4.tar`

### file list

```diff
@@ -1,83 +1,82 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 01:36:10.951942 catchem-alpha-zero-0.0.3/
--rw-rw-rw-   0        0        0     1087 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       20 2023-07-02 01:24:28.000000 catchem-alpha-zero-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0    14902 2023-07-02 01:36:10.952942 catchem-alpha-zero-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    14167 2023-07-02 01:15:05.000000 catchem-alpha-zero-0.0.3/README.md
--rw-rw-rw-   0        0        0      311 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0     1370 2023-07-02 01:36:10.953943 catchem-alpha-zero-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-02 01:36:10.861776 catchem-alpha-zero-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-02 01:36:10.888290 catchem-alpha-zero-0.0.3/src/catchem_alpha_zero.egg-info/
--rw-rw-rw-   0        0        0    14902 2023-07-02 01:36:10.000000 catchem-alpha-zero-0.0.3/src/catchem_alpha_zero.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2019 2023-07-02 01:36:10.000000 catchem-alpha-zero-0.0.3/src/catchem_alpha_zero.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 01:36:10.000000 catchem-alpha-zero-0.0.3/src/catchem_alpha_zero.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-07-02 01:36:10.000000 catchem-alpha-zero-0.0.3/src/catchem_alpha_zero.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      160 2023-07-02 01:36:10.000000 catchem-alpha-zero-0.0.3/src/catchem_alpha_zero.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-02 01:36:10.000000 catchem-alpha-zero-0.0.3/src/catchem_alpha_zero.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-02 01:36:10.900467 catchem-alpha-zero-0.0.3/src/caz/
--rw-rw-rw-   0        0        0        0 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/__init__.py
--rw-rw-rw-   0        0        0       75 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 01:36:10.909469 catchem-alpha-zero-0.0.3/src/caz/alpha_zero/
--rw-rw-rw-   0        0        0      606 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/alpha_zero/__init__.py
--rw-rw-rw-   0        0        0    16195 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/alpha_zero/alpha_zero.py
--rw-rw-rw-   0        0        0    11234 2023-07-01 16:12:31.000000 catchem-alpha-zero-0.0.3/src/caz/alpha_zero/alpha_zero_mcts.py
--rw-rw-rw-   0        0        0     5620 2023-06-19 23:03:45.000000 catchem-alpha-zero-0.0.3/src/caz/alpha_zero/alpha_zero_parameters.py
--rw-rw-rw-   0        0        0      565 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/alpha_zero/alpha_zero_training_models.py
--rw-rw-rw-   0        0        0     1638 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/alpha_zero/network.py
--rw-rw-rw-   0        0        0    12738 2023-06-22 18:59:16.000000 catchem-alpha-zero-0.0.3/src/caz/alpha_zero/network_torch.py
--rw-rw-rw-   0        0        0     1296 2023-07-01 16:37:59.000000 catchem-alpha-zero-0.0.3/src/caz/alpha_zero/retrainer.py
--rw-rw-rw-   0        0        0     4734 2023-07-01 16:37:55.000000 catchem-alpha-zero-0.0.3/src/caz/alpha_zero/supervised_learning.py
--rw-rw-rw-   0        0        0      549 2023-06-20 22:58:18.000000 catchem-alpha-zero-0.0.3/src/caz/app.py
--rw-rw-rw-   0        0        0      791 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/async_utils.py
--rw-rw-rw-   0        0        0     1434 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/bitboard_utils.py
--rw-rw-rw-   0        0        0     5034 2023-06-19 22:51:48.000000 catchem-alpha-zero-0.0.3/src/caz/cli.py
-drwxrwxrwx   0        0        0        0 2023-07-02 01:36:10.912594 catchem-alpha-zero-0.0.3/src/caz/games/
--rw-rw-rw-   0        0        0      233 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/games/__init__.py
--rw-rw-rw-   0        0        0     8078 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/games/game.py
--rw-rw-rw-   0        0        0      975 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/games/game_type.py
--rw-rw-rw-   0        0        0      833 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/graph.py
-drwxrwxrwx   0        0        0        0 2023-07-02 01:36:10.929269 catchem-alpha-zero-0.0.3/src/caz/images/
--rw-rw-rw-   0        0        0        0 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 01:36:10.930760 catchem-alpha-zero-0.0.3/src/caz/images/__pycache__/
--rw-rw-rw-   0        0        0      180 2023-06-19 22:45:56.000000 catchem-alpha-zero-0.0.3/src/caz/images/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     1260 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/black-bishop.png
--rw-rw-rw-   0        0        0     2485 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/black-king.png
--rw-rw-rw-   0        0        0     1516 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/black-knight.png
--rw-rw-rw-   0        0        0      797 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/black-pawn.png
--rw-rw-rw-   0        0        0     2267 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/black-queen.png
--rw-rw-rw-   0        0        0      725 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/black-rook.png
--rw-rw-rw-   0        0        0    23865 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/caz_flat_logo.png
--rw-rw-rw-   0        0        0   138365 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/caz_splashscreen.jpg
--rw-rw-rw-   0        0        0    67646 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/tiny_chess.ico
--rw-rw-rw-   0        0        0     1944 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/white-bishop.png
--rw-rw-rw-   0        0        0     2279 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/white-king.png
--rw-rw-rw-   0        0        0     1878 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/white-knight.png
--rw-rw-rw-   0        0        0     1294 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/white-pawn.png
--rw-rw-rw-   0        0        0     2637 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/white-queen.png
--rw-rw-rw-   0        0        0      933 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/images/white-rook.png
--rw-rw-rw-   0        0        0     2953 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/kaggle_sandbox.py
--rw-rw-rw-   0        0        0      203 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/kaggle_types.py
-drwxrwxrwx   0        0        0        0 2023-07-02 01:36:10.935761 catchem-alpha-zero-0.0.3/src/caz/solvers/
--rw-rw-rw-   0        0        0       86 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/solvers/__init__.py
--rw-rw-rw-   0        0        0     1797 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/solvers/agent_type.py
--rw-rw-rw-   0        0        0     3446 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/solvers/mcts.py
--rw-rw-rw-   0        0        0      932 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/solvers/minimax.py
--rw-rw-rw-   0        0        0      184 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/solvers/solver.py
-drwxrwxrwx   0        0        0        0 2023-07-02 01:36:10.942325 catchem-alpha-zero-0.0.3/src/caz/states/
--rw-rw-rw-   0        0        0      300 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/states/__init__.py
--rw-rw-rw-   0        0        0    11334 2023-06-19 23:54:49.000000 catchem-alpha-zero-0.0.3/src/caz/states/chess.py
--rw-rw-rw-   0        0        0    18449 2023-06-22 18:59:16.000000 catchem-alpha-zero-0.0.3/src/caz/states/chess_enums.py
--rw-rw-rw-   0        0        0     8959 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/states/connectx.py
--rw-rw-rw-   0        0        0     2430 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/states/state.py
--rw-rw-rw-   0        0        0     5475 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/states/tictactoe.py
--rw-rw-rw-   0        0        0     7687 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/sumplete_solver.py
-drwxrwxrwx   0        0        0        0 2023-07-02 01:36:10.949828 catchem-alpha-zero-0.0.3/src/caz/views/
--rw-rw-rw-   0        0        0       32 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/views/__init__.py
--rw-rw-rw-   0        0        0    20923 2023-07-02 01:15:12.000000 catchem-alpha-zero-0.0.3/src/caz/views/chess_detail.py
--rw-rw-rw-   0        0        0     5555 2023-07-02 01:33:24.000000 catchem-alpha-zero-0.0.3/src/caz/views/chess_main.py
--rw-rw-rw-   0        0        0     1646 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/views/console.py
--rw-rw-rw-   0        0        0     5610 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/views/html.py
--rw-rw-rw-   0        0        0     3692 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/views/plot.py
--rw-rw-rw-   0        0        0     2022 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/views/policies.py
--rw-rw-rw-   0        0        0      216 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.3/src/caz/views/view.py
-drwxrwxrwx   0        0        0        0 2023-07-02 01:36:10.950940 catchem-alpha-zero-0.0.3/tests/
--rw-rw-rw-   0        0        0     2017 2023-07-01 16:11:29.000000 catchem-alpha-zero-0.0.3/tests/test_chess.py
+drwxrwxrwx   0        0        0        0 2023-07-02 02:18:15.339924 catchem-alpha-zero-0.0.4/
+-rw-rw-rw-   0        0        0     1087 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       20 2023-07-02 01:24:28.000000 catchem-alpha-zero-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    14982 2023-07-02 02:18:15.339924 catchem-alpha-zero-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    14247 2023-07-02 02:11:55.000000 catchem-alpha-zero-0.0.4/README.md
+-rw-rw-rw-   0        0        0      311 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1418 2023-07-02 02:18:15.346433 catchem-alpha-zero-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-02 02:18:15.238312 catchem-alpha-zero-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-02 02:18:15.270295 catchem-alpha-zero-0.0.4/src/catchem_alpha_zero.egg-info/
+-rw-rw-rw-   0        0        0    14982 2023-07-02 02:18:15.000000 catchem-alpha-zero-0.0.4/src/catchem_alpha_zero.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1992 2023-07-02 02:18:15.000000 catchem-alpha-zero-0.0.4/src/catchem_alpha_zero.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 02:18:15.000000 catchem-alpha-zero-0.0.4/src/catchem_alpha_zero.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-07-02 02:18:15.000000 catchem-alpha-zero-0.0.4/src/catchem_alpha_zero.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      169 2023-07-02 02:18:15.000000 catchem-alpha-zero-0.0.4/src/catchem_alpha_zero.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-02 02:18:15.000000 catchem-alpha-zero-0.0.4/src/catchem_alpha_zero.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 02:18:15.280817 catchem-alpha-zero-0.0.4/src/caz/
+-rw-rw-rw-   0        0        0        0 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/__init__.py
+-rw-rw-rw-   0        0        0       75 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 02:18:15.292328 catchem-alpha-zero-0.0.4/src/caz/alpha_zero/
+-rw-rw-rw-   0        0        0      606 2023-07-02 01:56:30.000000 catchem-alpha-zero-0.0.4/src/caz/alpha_zero/__init__.py
+-rw-rw-rw-   0        0        0    16191 2023-07-02 01:56:20.000000 catchem-alpha-zero-0.0.4/src/caz/alpha_zero/alpha_zero.py
+-rw-rw-rw-   0        0        0    11234 2023-07-01 16:12:31.000000 catchem-alpha-zero-0.0.4/src/caz/alpha_zero/alpha_zero_mcts.py
+-rw-rw-rw-   0        0        0     5620 2023-06-19 23:03:45.000000 catchem-alpha-zero-0.0.4/src/caz/alpha_zero/alpha_zero_parameters.py
+-rw-rw-rw-   0        0        0      565 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/alpha_zero/alpha_zero_training_models.py
+-rw-rw-rw-   0        0        0     1638 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/alpha_zero/network.py
+-rw-rw-rw-   0        0        0    12735 2023-07-02 01:54:58.000000 catchem-alpha-zero-0.0.4/src/caz/alpha_zero/network_torch.py
+-rw-rw-rw-   0        0        0     1296 2023-07-01 16:37:59.000000 catchem-alpha-zero-0.0.4/src/caz/alpha_zero/retrainer.py
+-rw-rw-rw-   0        0        0     4734 2023-07-01 16:37:55.000000 catchem-alpha-zero-0.0.4/src/caz/alpha_zero/supervised_learning.py
+-rw-rw-rw-   0        0        0      549 2023-06-20 22:58:18.000000 catchem-alpha-zero-0.0.4/src/caz/app.py
+-rw-rw-rw-   0        0        0      791 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/async_utils.py
+-rw-rw-rw-   0        0        0     1434 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/bitboard_utils.py
+-rw-rw-rw-   0        0        0     5004 2023-07-02 01:58:43.000000 catchem-alpha-zero-0.0.4/src/caz/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-02 02:18:15.295286 catchem-alpha-zero-0.0.4/src/caz/games/
+-rw-rw-rw-   0        0        0      233 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/games/__init__.py
+-rw-rw-rw-   0        0        0     8077 2023-07-02 01:56:07.000000 catchem-alpha-zero-0.0.4/src/caz/games/game.py
+-rw-rw-rw-   0        0        0      975 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/games/game_type.py
+-rw-rw-rw-   0        0        0      833 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/graph.py
+drwxrwxrwx   0        0        0        0 2023-07-02 02:18:15.314365 catchem-alpha-zero-0.0.4/src/caz/images/
+-rw-rw-rw-   0        0        0        0 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/images/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 02:18:15.315811 catchem-alpha-zero-0.0.4/src/caz/images/__pycache__/
+-rw-rw-rw-   0        0        0      180 2023-06-19 22:45:56.000000 catchem-alpha-zero-0.0.4/src/caz/images/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1260 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/images/black-bishop.png
+-rw-rw-rw-   0        0        0     2485 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/images/black-king.png
+-rw-rw-rw-   0        0        0     1516 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/images/black-knight.png
+-rw-rw-rw-   0        0        0      797 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/images/black-pawn.png
+-rw-rw-rw-   0        0        0     2267 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/images/black-queen.png
+-rw-rw-rw-   0        0        0      725 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/images/black-rook.png
+-rw-rw-rw-   0        0        0    23865 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/images/caz_flat_logo.png
+-rw-rw-rw-   0        0        0   138365 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/images/caz_splashscreen.jpg
+-rw-rw-rw-   0        0        0    67646 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/images/tiny_chess.ico
+-rw-rw-rw-   0        0        0     1944 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/images/white-bishop.png
+-rw-rw-rw-   0        0        0     2279 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/images/white-king.png
+-rw-rw-rw-   0        0        0     1878 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/images/white-knight.png
+-rw-rw-rw-   0        0        0     1294 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/images/white-pawn.png
+-rw-rw-rw-   0        0        0     2637 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/images/white-queen.png
+-rw-rw-rw-   0        0        0      933 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/images/white-rook.png
+-rw-rw-rw-   0        0        0     2953 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/kaggle_sandbox.py
+-rw-rw-rw-   0        0        0      203 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/kaggle_types.py
+drwxrwxrwx   0        0        0        0 2023-07-02 02:18:15.321812 catchem-alpha-zero-0.0.4/src/caz/solvers/
+-rw-rw-rw-   0        0        0       86 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/solvers/__init__.py
+-rw-rw-rw-   0        0        0     1797 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/solvers/agent_type.py
+-rw-rw-rw-   0        0        0     3446 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/solvers/mcts.py
+-rw-rw-rw-   0        0        0      932 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/solvers/minimax.py
+-rw-rw-rw-   0        0        0      184 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/solvers/solver.py
+drwxrwxrwx   0        0        0        0 2023-07-02 02:18:15.328608 catchem-alpha-zero-0.0.4/src/caz/states/
+-rw-rw-rw-   0        0        0      300 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/states/__init__.py
+-rw-rw-rw-   0        0        0    11334 2023-06-19 23:54:49.000000 catchem-alpha-zero-0.0.4/src/caz/states/chess.py
+-rw-rw-rw-   0        0        0    18449 2023-06-22 18:59:16.000000 catchem-alpha-zero-0.0.4/src/caz/states/chess_enums.py
+-rw-rw-rw-   0        0        0     8938 2023-07-02 01:58:21.000000 catchem-alpha-zero-0.0.4/src/caz/states/connectx.py
+-rw-rw-rw-   0        0        0     2430 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/states/state.py
+-rw-rw-rw-   0        0        0     5454 2023-07-02 01:55:55.000000 catchem-alpha-zero-0.0.4/src/caz/states/tictactoe.py
+drwxrwxrwx   0        0        0        0 2023-07-02 02:18:15.337924 catchem-alpha-zero-0.0.4/src/caz/views/
+-rw-rw-rw-   0        0        0       32 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/views/__init__.py
+-rw-rw-rw-   0        0        0    20921 2023-07-02 01:54:46.000000 catchem-alpha-zero-0.0.4/src/caz/views/chess_detail.py
+-rw-rw-rw-   0        0        0     5555 2023-07-02 01:33:24.000000 catchem-alpha-zero-0.0.4/src/caz/views/chess_main.py
+-rw-rw-rw-   0        0        0     1646 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/views/console.py
+-rw-rw-rw-   0        0        0     5610 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/views/html.py
+-rw-rw-rw-   0        0        0     3692 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/views/plot.py
+-rw-rw-rw-   0        0        0     2022 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/views/policies.py
+-rw-rw-rw-   0        0        0      216 2023-06-19 22:16:21.000000 catchem-alpha-zero-0.0.4/src/caz/views/view.py
+drwxrwxrwx   0        0        0        0 2023-07-02 02:18:15.338923 catchem-alpha-zero-0.0.4/tests/
+-rw-rw-rw-   0        0        0     2017 2023-07-01 16:11:29.000000 catchem-alpha-zero-0.0.4/tests/test_chess.py
```

### Comparing `catchem-alpha-zero-0.0.3/LICENSE` & `catchem-alpha-zero-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/PKG-INFO` & `catchem-alpha-zero-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catchem-alpha-zero
-Version: 0.0.3
+Version: 0.0.4
 Summary: CatchemAlphaZero: AI techniques for solving games
 Home-page: https://github.com/CatchemAL/CatchemAlphaZero
 Author: Alex Cross
 Author-email: AlexJCross90@gmail.com
 Project-URL: Bug Tracker, https://github.com/CatchemAL/CatchemAlphaZero/issues
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -17,18 +17,18 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 <img src="https://raw.githubusercontent.com/CatchemAl/CatchemAlphaZero/main/src/caz/images/caz_splashscreen.jpg" width="420">
 
 ## Features
 
-[![example workflow](https://github.com/CatchemAl/Doddle/actions/workflows/python-app.yml/badge.svg)](https://github.com/CatchemAl/Doddle/actions)
-[![PyPI - Wheel](https://img.shields.io/pypi/wheel/Doddle)](https://pypi.org/project/doddle/#files)
-[![PyPI](https://img.shields.io/pypi/v/doddle.svg)](https://pypi.org/project/doddle/)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/Doddle)
+[![example workflow](https://github.com/CatchemAl/CatchemAlphaZero/actions/workflows/python-app.yml/badge.svg)](https://github.com/CatchemAl/CatchemAlphaZero/actions)
+[![PyPI - Wheel](https://img.shields.io/pypi/wheel/catchem-alpha-zero)](https://pypi.org/project/catchem-alpha-zero/#files)
+[![PyPI](https://img.shields.io/pypi/v/catchem-alpha-zero.svg)](https://pypi.org/project/catchem-alpha-zero/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/catchem-alpha-zero)
 [![Tutorial](https://img.shields.io/badge/CAZ-tutorial-orange?logo=jupyter)](https://github.com/CatchemAL/CatchemAlphaZero/tree/main/tutorials)
 
 ## Installation
 `pip install catchem-alpha-zero`
 
 ### Project Overview
 `CatchemAlphaZero` (CAZ) showcases techniques in artificial intelligence for solving two-player games without any human knowledge or input except for the rules of the game.  Any two-player deterministic game can, in principle, leverage this framework.  Little is needed beyond the ability to:
```

### Comparing `catchem-alpha-zero-0.0.3/README.md` & `catchem-alpha-zero-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <img src="https://raw.githubusercontent.com/CatchemAl/CatchemAlphaZero/main/src/caz/images/caz_splashscreen.jpg" width="420">
 
 ## Features
 
-[![example workflow](https://github.com/CatchemAl/Doddle/actions/workflows/python-app.yml/badge.svg)](https://github.com/CatchemAl/Doddle/actions)
-[![PyPI - Wheel](https://img.shields.io/pypi/wheel/Doddle)](https://pypi.org/project/doddle/#files)
-[![PyPI](https://img.shields.io/pypi/v/doddle.svg)](https://pypi.org/project/doddle/)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/Doddle)
+[![example workflow](https://github.com/CatchemAl/CatchemAlphaZero/actions/workflows/python-app.yml/badge.svg)](https://github.com/CatchemAl/CatchemAlphaZero/actions)
+[![PyPI - Wheel](https://img.shields.io/pypi/wheel/catchem-alpha-zero)](https://pypi.org/project/catchem-alpha-zero/#files)
+[![PyPI](https://img.shields.io/pypi/v/catchem-alpha-zero.svg)](https://pypi.org/project/catchem-alpha-zero/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/catchem-alpha-zero)
 [![Tutorial](https://img.shields.io/badge/CAZ-tutorial-orange?logo=jupyter)](https://github.com/CatchemAL/CatchemAlphaZero/tree/main/tutorials)
 
 ## Installation
 `pip install catchem-alpha-zero`
 
 ### Project Overview
 `CatchemAlphaZero` (CAZ) showcases techniques in artificial intelligence for solving two-player games without any human knowledge or input except for the rules of the game.  Any two-player deterministic game can, in principle, leverage this framework.  Little is needed beyond the ability to:
```

### Comparing `catchem-alpha-zero-0.0.3/setup.cfg` & `catchem-alpha-zero-0.0.4/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6174 6368 656d 2d61 6c70 6861   = catchem-alpha
 00000020: 2d7a 6572 6f0d 0a76 6572 7369 6f6e 203d  -zero..version =
-00000030: 2030 2e30 2e33 0d0a 6175 7468 6f72 203d   0.0.3..author =
+00000030: 2030 2e30 2e34 0d0a 6175 7468 6f72 203d   0.0.4..author =
 00000040: 2041 6c65 7820 4372 6f73 730d 0a61 7574   Alex Cross..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 416c 6578  hor_email = Alex
 00000060: 4a43 726f 7373 3930 4067 6d61 696c 2e63  JCross90@gmail.c
 00000070: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
 00000080: 3d20 4361 7463 6865 6d41 6c70 6861 5a65  = CatchemAlphaZe
 00000090: 726f 3a20 4149 2074 6563 686e 6971 7565  ro: AI technique
 000000a0: 7320 666f 7220 736f 6c76 696e 6720 6761  s for solving ga
@@ -48,39 +48,42 @@
 000002f0: 203d 200d 0a09 6e75 6d70 790d 0a09 746f   = ...numpy...to
 00000300: 7263 680d 0a09 746f 7263 6876 6973 696f  rch...torchvisio
 00000310: 6e0d 0a09 7465 6e73 6f72 626f 6172 640d  n...tensorboard.
 00000320: 0a09 6d61 7470 6c6f 746c 6962 0d0a 0969  ..matplotlib...i
 00000330: 7079 7769 6467 6574 730d 0a09 6a75 7079  pywidgets...jupy
 00000340: 7465 726c 6162 0d0a 096e 6573 742d 6173  terlab...nest-as
 00000350: 796e 6369 6f0d 0a09 7471 646d 0d0a 0963  yncio...tqdm...c
-00000360: 6865 7373 0d0a 0967 7261 7068 7669 7a0d  hess...graphviz.
-00000370: 0a09 6b61 6767 6c65 2d65 6e76 6972 6f6e  ..kaggle-environ
-00000380: 6d65 6e74 730d 0a0d 0a5b 6f70 7469 6f6e  ments....[option
-00000390: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
-000003a0: 0d0a 7768 6572 6520 3d20 7372 630d 0a0d  ..where = src...
-000003b0: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
-000003c0: 655f 6461 7461 5d0d 0a63 617a 2e69 6d61  e_data]..caz.ima
-000003d0: 6765 7320 3d20 0d0a 092a 2e70 6e67 0d0a  ges = ...*.png..
-000003e0: 092a 2e6a 7067 0d0a 092a 2e69 636f 0d0a  .*.jpg...*.ico..
-000003f0: 0d0a 5b6f 7074 696f 6e73 2e65 6e74 7279  ..[options.entry
-00000400: 5f70 6f69 6e74 735d 0d0a 636f 6e73 6f6c  _points]..consol
-00000410: 655f 7363 7269 7074 7320 3d20 0d0a 0963  e_scripts = ...c
-00000420: 617a 203d 2063 617a 2e63 6c69 3a6d 6169  az = caz.cli:mai
-00000430: 6e0d 0a67 7569 5f73 6372 6970 7473 203d  n..gui_scripts =
-00000440: 200d 0a09 616c 7068 6120 3d20 6361 7a2e   ...alpha = caz.
-00000450: 6170 703a 6c61 756e 6368 0d0a 0d0a 5b6f  app:launch....[o
-00000460: 7074 696f 6e73 2e65 7874 7261 735f 7265  ptions.extras_re
-00000470: 7175 6972 655d 0d0a 6465 7620 3d20 0d0a  quire]..dev = ..
-00000480: 0962 6c61 636b 0d0a 0966 6c61 6b65 380d  .black...flake8.
-00000490: 0a09 6973 6f72 740d 0a09 6d79 7079 0d0a  ..isort...mypy..
-000004a0: 0970 7974 6573 740d 0a0d 0a5b 666c 616b  .pytest....[flak
-000004b0: 6538 5d0d 0a69 676e 6f72 6520 3d20 0d0a  e8]..ignore = ..
-000004c0: 0945 3230 330d 0a09 5735 3033 0d0a 6578  .E203...W503..ex
-000004d0: 7465 6e64 2d65 7863 6c75 6465 203d 202e  tend-exclude = .
-000004e0: 7665 6e76 2f2a 2e70 792c 2e74 6f78 2f2a  venv/*.py,.tox/*
-000004f0: 2e70 792c 7465 7374 732f 2a2e 7079 0d0a  .py,tests/*.py..
-00000500: 6669 6c65 6e61 6d65 203d 202e 2f73 7263  filename = ./src
-00000510: 2f2a 2e70 790d 0a6d 6178 2d6c 696e 652d  /*.py..max-line-
-00000520: 6c65 6e67 7468 203d 2031 3035 0d0a 0d0a  length = 105....
-00000530: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
-00000540: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
-00000550: 7465 203d 2030 0d0a 0d0a                 te = 0....
+00000360: 6865 7373 0d0a 0963 6f6c 6f72 616d 610d  hess...colorama.
+00000370: 0a09 6772 6170 6876 697a 0d0a 096b 6167  ..graphviz...kag
+00000380: 676c 652d 656e 7669 726f 6e6d 656e 7473  gle-environments
+00000390: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
+000003a0: 6b61 6765 732e 6669 6e64 5d0d 0a77 6865  kages.find]..whe
+000003b0: 7265 203d 2073 7263 0d0a 0d0a 5b6f 7074  re = src....[opt
+000003c0: 696f 6e73 2e70 6163 6b61 6765 5f64 6174  ions.package_dat
+000003d0: 615d 0d0a 6361 7a2e 696d 6167 6573 203d  a]..caz.images =
+000003e0: 200d 0a09 2a2e 706e 670d 0a09 2a2e 6a70   ...*.png...*.jp
+000003f0: 670d 0a09 2a2e 6963 6f0d 0a0d 0a5b 6f70  g...*.ico....[op
+00000400: 7469 6f6e 732e 656e 7472 795f 706f 696e  tions.entry_poin
+00000410: 7473 5d0d 0a63 6f6e 736f 6c65 5f73 6372  ts]..console_scr
+00000420: 6970 7473 203d 200d 0a09 6361 7a20 3d20  ipts = ...caz = 
+00000430: 6361 7a2e 636c 693a 6d61 696e 0d0a 6775  caz.cli:main..gu
+00000440: 695f 7363 7269 7074 7320 3d20 0d0a 0961  i_scripts = ...a
+00000450: 6c70 6861 203d 2063 617a 2e61 7070 3a6c  lpha = caz.app:l
+00000460: 6175 6e63 680d 0a0d 0a5b 6f70 7469 6f6e  aunch....[option
+00000470: 732e 6578 7472 6173 5f72 6571 7569 7265  s.extras_require
+00000480: 5d0d 0a64 6576 203d 200d 0a09 626c 6163  ]..dev = ...blac
+00000490: 6b0d 0a09 666c 616b 6538 0d0a 0969 736f  k...flake8...iso
+000004a0: 7274 0d0a 096d 7970 790d 0a09 7079 7465  rt...mypy...pyte
+000004b0: 7374 0d0a 0d0a 5b66 6c61 6b65 385d 0d0a  st....[flake8]..
+000004c0: 6967 6e6f 7265 203d 200d 0a09 4532 3033  ignore = ...E203
+000004d0: 0d0a 0957 3530 330d 0a70 6572 2d66 696c  ...W503..per-fil
+000004e0: 652d 6967 6e6f 7265 7320 3d20 5f5f 696e  e-ignores = __in
+000004f0: 6974 5f5f 2e70 793a 4634 3031 0d0a 6578  it__.py:F401..ex
+00000500: 7465 6e64 2d65 7863 6c75 6465 203d 202e  tend-exclude = .
+00000510: 7665 6e76 2f2a 2e70 792c 2e74 6f78 2f2a  venv/*.py,.tox/*
+00000520: 2e70 792c 7465 7374 732f 2a2e 7079 0d0a  .py,tests/*.py..
+00000530: 6669 6c65 6e61 6d65 203d 202e 2f73 7263  filename = ./src
+00000540: 2f2a 2e70 790d 0a6d 6178 2d6c 696e 652d  /*.py..max-line-
+00000550: 6c65 6e67 7468 203d 2031 3035 0d0a 0d0a  length = 105....
+00000560: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
+00000570: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
+00000580: 7465 203d 2030 0d0a 0d0a                 te = 0....
```

### Comparing `catchem-alpha-zero-0.0.3/src/catchem_alpha_zero.egg-info/PKG-INFO` & `catchem-alpha-zero-0.0.4/src/catchem_alpha_zero.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catchem-alpha-zero
-Version: 0.0.3
+Version: 0.0.4
 Summary: CatchemAlphaZero: AI techniques for solving games
 Home-page: https://github.com/CatchemAL/CatchemAlphaZero
 Author: Alex Cross
 Author-email: AlexJCross90@gmail.com
 Project-URL: Bug Tracker, https://github.com/CatchemAL/CatchemAlphaZero/issues
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -17,18 +17,18 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 <img src="https://raw.githubusercontent.com/CatchemAl/CatchemAlphaZero/main/src/caz/images/caz_splashscreen.jpg" width="420">
 
 ## Features
 
-[![example workflow](https://github.com/CatchemAl/Doddle/actions/workflows/python-app.yml/badge.svg)](https://github.com/CatchemAl/Doddle/actions)
-[![PyPI - Wheel](https://img.shields.io/pypi/wheel/Doddle)](https://pypi.org/project/doddle/#files)
-[![PyPI](https://img.shields.io/pypi/v/doddle.svg)](https://pypi.org/project/doddle/)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/Doddle)
+[![example workflow](https://github.com/CatchemAl/CatchemAlphaZero/actions/workflows/python-app.yml/badge.svg)](https://github.com/CatchemAl/CatchemAlphaZero/actions)
+[![PyPI - Wheel](https://img.shields.io/pypi/wheel/catchem-alpha-zero)](https://pypi.org/project/catchem-alpha-zero/#files)
+[![PyPI](https://img.shields.io/pypi/v/catchem-alpha-zero.svg)](https://pypi.org/project/catchem-alpha-zero/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/catchem-alpha-zero)
 [![Tutorial](https://img.shields.io/badge/CAZ-tutorial-orange?logo=jupyter)](https://github.com/CatchemAL/CatchemAlphaZero/tree/main/tutorials)
 
 ## Installation
 `pip install catchem-alpha-zero`
 
 ### Project Overview
 `CatchemAlphaZero` (CAZ) showcases techniques in artificial intelligence for solving two-player games without any human knowledge or input except for the rules of the game.  Any two-player deterministic game can, in principle, leverage this framework.  Little is needed beyond the ability to:
```

### Comparing `catchem-alpha-zero-0.0.3/src/catchem_alpha_zero.egg-info/SOURCES.txt` & `catchem-alpha-zero-0.0.4/src/catchem_alpha_zero.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 src/caz/app.py
 src/caz/async_utils.py
 src/caz/bitboard_utils.py
 src/caz/cli.py
 src/caz/graph.py
 src/caz/kaggle_sandbox.py
 src/caz/kaggle_types.py
-src/caz/sumplete_solver.py
 src/caz/alpha_zero/__init__.py
 src/caz/alpha_zero/alpha_zero.py
 src/caz/alpha_zero/alpha_zero_mcts.py
 src/caz/alpha_zero/alpha_zero_parameters.py
 src/caz/alpha_zero/alpha_zero_training_models.py
 src/caz/alpha_zero/network.py
 src/caz/alpha_zero/network_torch.py
```

### Comparing `catchem-alpha-zero-0.0.3/src/caz/alpha_zero/__init__.py` & `catchem-alpha-zero-0.0.4/src/caz/alpha_zero/__init__.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/alpha_zero/alpha_zero.py` & `catchem-alpha-zero-0.0.4/src/caz/alpha_zero/alpha_zero.py`

 * *Files 1% similar despite different names*

```diff
@@ -359,18 +359,18 @@
         return num_wins, num_draws, num_losses
 
     def _log_result(self, arena_result: ArenaResult) -> None:
         writer = SummaryWriter(log_dir=f"runs/{self.game.fullname}")
         gen = arena_result.generation
 
         # Logging metrics to TensorBoard
-        writer.add_scalar(f"Arena/Win Ratio", arena_result.win_ratio, gen)
-        writer.add_scalar(f"Arena/Total Wins", arena_result.num_wins, gen)
-        writer.add_scalar(f"Arena/Total Draws", arena_result.num_draws, gen)
-        writer.add_scalar(f"Arena/Total Losses", arena_result.num_losses, gen)
+        writer.add_scalar("Arena/Win Ratio", arena_result.win_ratio, gen)
+        writer.add_scalar("Arena/Total Wins", arena_result.num_wins, gen)
+        writer.add_scalar("Arena/Total Draws", arena_result.num_draws, gen)
+        writer.add_scalar("Arena/Total Losses", arena_result.num_losses, gen)
         writer.close()
 
 
 @dataclass
 class InitialStateGenerator:
     initial_state: State
     depth: int
```

### Comparing `catchem-alpha-zero-0.0.3/src/caz/alpha_zero/alpha_zero_mcts.py` & `catchem-alpha-zero-0.0.4/src/caz/alpha_zero/alpha_zero_mcts.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/alpha_zero/alpha_zero_parameters.py` & `catchem-alpha-zero-0.0.4/src/caz/alpha_zero/alpha_zero_parameters.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/alpha_zero/alpha_zero_training_models.py` & `catchem-alpha-zero-0.0.4/src/caz/alpha_zero/alpha_zero_training_models.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/alpha_zero/network.py` & `catchem-alpha-zero-0.0.4/src/caz/alpha_zero/network.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/alpha_zero/network_torch.py` & `catchem-alpha-zero-0.0.4/src/caz/alpha_zero/network_torch.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,17 +190,17 @@
 
                     # Store key metrics
                     epoch_policy_loss += policy_loss.item()
                     epoch_outcome_loss += outcome_loss.item()
                     epoch_total_loss += total_loss.item()
 
             # Logging metrics to TensorBoard
-            writer.add_scalar(f"Generations/Total Loss", epoch_total_loss / num_points, gen)
-            writer.add_scalar(f"Generations/Policy Loss", epoch_policy_loss / num_points, gen)
-            writer.add_scalar(f"Generations/Outcome Loss", epoch_outcome_loss / num_points, gen)
+            writer.add_scalar("Generations/Total Loss", epoch_total_loss / num_points, gen)
+            writer.add_scalar("Generations/Policy Loss", epoch_policy_loss / num_points, gen)
+            writer.add_scalar("Generations/Outcome Loss", epoch_outcome_loss / num_points, gen)
 
         self.resnet.train()
         for epoch in trange(num_epochs, desc=" - Training", leave=False):
             epoch_policy_loss = 0.0
             epoch_outcome_loss = 0.0
             epoch_total_loss = 0.0
```

### Comparing `catchem-alpha-zero-0.0.3/src/caz/alpha_zero/retrainer.py` & `catchem-alpha-zero-0.0.4/src/caz/alpha_zero/retrainer.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/alpha_zero/supervised_learning.py` & `catchem-alpha-zero-0.0.4/src/caz/alpha_zero/supervised_learning.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/app.py` & `catchem-alpha-zero-0.0.4/src/caz/app.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/async_utils.py` & `catchem-alpha-zero-0.0.4/src/caz/async_utils.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/bitboard_utils.py` & `catchem-alpha-zero-0.0.4/src/caz/bitboard_utils.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/cli.py` & `catchem-alpha-zero-0.0.4/src/caz/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import sys
 from argparse import ArgumentParser, Namespace
 from typing import Sequence
 
-import numpy as np
-
 from .games import GameType, get_game
-from .solvers import AgentType, Solver
+from .solvers import AgentType
 
 
 def run(args: Namespace) -> None:
     game_type: GameType = args.game
     init: str = args.init
     player1_type: AgentType = args.player1
     player2_type: AgentType = args.player2
```

### Comparing `catchem-alpha-zero-0.0.3/src/caz/games/game.py` & `catchem-alpha-zero-0.0.4/src/caz/games/game.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
 
     @property
     def name(self) -> str:
         return "tictactoe"
 
     @property
     def fullname(self) -> str:
-        return f"TicTacToe"
+        return "TicTacToe"
 
     @property
     def shape(self) -> tuple[int, int]:
         return self.ROWS, self.COLS
 
     def initial_state(self, start: str | list[int] | None = None) -> TicTacToeState:
         return TicTacToeState.create(start)
```

### Comparing `catchem-alpha-zero-0.0.3/src/caz/games/game_type.py` & `catchem-alpha-zero-0.0.4/src/caz/games/game_type.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/graph.py` & `catchem-alpha-zero-0.0.4/src/caz/graph.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/images/black-bishop.png` & `catchem-alpha-zero-0.0.4/src/caz/images/black-bishop.png`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/images/black-king.png` & `catchem-alpha-zero-0.0.4/src/caz/images/black-king.png`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/images/black-knight.png` & `catchem-alpha-zero-0.0.4/src/caz/images/black-knight.png`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/images/black-pawn.png` & `catchem-alpha-zero-0.0.4/src/caz/images/black-pawn.png`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/images/black-queen.png` & `catchem-alpha-zero-0.0.4/src/caz/images/black-queen.png`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/images/black-rook.png` & `catchem-alpha-zero-0.0.4/src/caz/images/black-rook.png`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/images/caz_flat_logo.png` & `catchem-alpha-zero-0.0.4/src/caz/images/caz_flat_logo.png`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/images/caz_splashscreen.jpg` & `catchem-alpha-zero-0.0.4/src/caz/images/caz_splashscreen.jpg`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/images/tiny_chess.ico` & `catchem-alpha-zero-0.0.4/src/caz/images/tiny_chess.ico`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/images/white-bishop.png` & `catchem-alpha-zero-0.0.4/src/caz/images/white-bishop.png`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/images/white-king.png` & `catchem-alpha-zero-0.0.4/src/caz/images/white-king.png`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/images/white-knight.png` & `catchem-alpha-zero-0.0.4/src/caz/images/white-knight.png`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/images/white-pawn.png` & `catchem-alpha-zero-0.0.4/src/caz/images/white-pawn.png`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/images/white-queen.png` & `catchem-alpha-zero-0.0.4/src/caz/images/white-queen.png`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/images/white-rook.png` & `catchem-alpha-zero-0.0.4/src/caz/images/white-rook.png`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/kaggle_sandbox.py` & `catchem-alpha-zero-0.0.4/src/caz/kaggle_sandbox.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/solvers/agent_type.py` & `catchem-alpha-zero-0.0.4/src/caz/solvers/agent_type.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/solvers/mcts.py` & `catchem-alpha-zero-0.0.4/src/caz/solvers/mcts.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/solvers/minimax.py` & `catchem-alpha-zero-0.0.4/src/caz/solvers/minimax.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/states/chess.py` & `catchem-alpha-zero-0.0.4/src/caz/states/chess.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/states/chess_enums.py` & `catchem-alpha-zero-0.0.4/src/caz/states/chess_enums.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/states/connectx.py` & `catchem-alpha-zero-0.0.4/src/caz/states/connectx.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 from typing import Generator, Self
 
 import numpy as np
 
 from ..bitboard_utils import BitboardUtil
-from .state import State, Status, TemperatureSchedule
+from .state import State, Status
 
 
 @dataclass(slots=True)
 class ConnectXState(State[int]):
     bitboard_util: BitboardUtil
     mask: int
     position: int
```

### Comparing `catchem-alpha-zero-0.0.3/src/caz/states/state.py` & `catchem-alpha-zero-0.0.4/src/caz/states/state.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/states/tictactoe.py` & `catchem-alpha-zero-0.0.4/src/caz/states/tictactoe.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 from typing import Self
 
 import numpy as np
 
 from ..bitboard_utils import BitboardUtil
-from .state import State, Status, TemperatureSchedule
+from .state import State, Status
 
 # 3  7 11
 # 2  6 10
 # 1  5  9
 # 0  4  8
 
 MOVES = [1 << 2, 1 << 6, 1 << 10, 1 << 1, 1 << 5, 1 << 9, 1 << 0, 1 << 4, 1 << 8]
```

### Comparing `catchem-alpha-zero-0.0.3/src/caz/views/chess_detail.py` & `catchem-alpha-zero-0.0.4/src/caz/views/chess_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,24 +365,24 @@
             fg=TEAL_COLOR,
             bg=DARK_COLOR,
         )
         players_label.pack(side=tk.TOP, pady=0, anchor=tk.W)
 
         white_player_label = tk.Label(
             frame,
-            text=f"White: <<PLACEHOLDER>>",
+            text="White: <<PLACEHOLDER>>",
             font=("Cascadia Mono", 11),
             fg=BLUE_COLOR,
             bg=DARK_COLOR,
         )
         white_player_label.pack(side=tk.TOP, pady=(0, 0), anchor=tk.W)
 
         black_player_label = tk.Label(
             frame,
-            text=f"Black: <<PLACEHOLDER>>",
+            text="Black: <<PLACEHOLDER>>",
             font=("Cascadia Mono", 11),
             fg=BLUE_COLOR,
             bg=DARK_COLOR,
         )
         black_player_label.pack(side=tk.TOP, pady=0, anchor=tk.W)
 
         checkbox = tk.Checkbutton(frame, text="Flip Board", variable=self.flip_board)
```

### Comparing `catchem-alpha-zero-0.0.3/src/caz/views/chess_main.py` & `catchem-alpha-zero-0.0.4/src/caz/views/chess_main.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/views/console.py` & `catchem-alpha-zero-0.0.4/src/caz/views/console.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/views/html.py` & `catchem-alpha-zero-0.0.4/src/caz/views/html.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/views/plot.py` & `catchem-alpha-zero-0.0.4/src/caz/views/plot.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/src/caz/views/policies.py` & `catchem-alpha-zero-0.0.4/src/caz/views/policies.py`

 * *Files identical despite different names*

### Comparing `catchem-alpha-zero-0.0.3/tests/test_chess.py` & `catchem-alpha-zero-0.0.4/tests/test_chess.py`

 * *Files identical despite different names*

