# Comparing `tmp/soccerbars-0.2.0.tar.gz` & `tmp/soccerbars-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soccerbars-0.2.0.tar", max compression
+gzip compressed data, was "soccerbars-0.2.1.tar", max compression
```

## Comparing `soccerbars-0.2.0.tar` & `soccerbars-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0       48 2021-04-09 15:25:30.777247 soccerbars-0.2.0/LICENSE
--rw-r--r--   0        0        0     1077 2021-04-09 15:25:30.777247 soccerbars-0.2.0/LICENSE.md
--rw-r--r--   0        0        0     8892 2021-04-09 15:25:30.777247 soccerbars-0.2.0/README.md
--rw-r--r--   0        0        0     1140 2021-04-09 15:25:30.777247 soccerbars-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       38 2021-04-09 15:25:30.781247 soccerbars-0.2.0/soccerbars/__init__.py
--rw-r--r--   0        0        0     4453 2021-04-09 15:25:30.781247 soccerbars-0.2.0/soccerbars/__main__.py
--rw-r--r--   0        0        0    29650 2021-04-09 15:25:30.781247 soccerbars-0.2.0/soccerbars/core.py
--rw-r--r--   0        0        0    10150 2021-04-09 15:26:10.605495 soccerbars-0.2.0/setup.py
--rw-r--r--   0        0        0     9965 2021-04-09 15:26:10.606383 soccerbars-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       48 2023-07-02 12:03:58.317652 soccerbars-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1077 2023-07-02 12:03:58.317652 soccerbars-0.2.1/LICENSE.md
+-rw-r--r--   0        0        0     9192 2023-07-02 12:03:58.317652 soccerbars-0.2.1/README.md
+-rw-r--r--   0        0        0     1178 2023-07-02 12:03:58.321652 soccerbars-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       38 2023-07-02 12:03:58.321652 soccerbars-0.2.1/soccerbars/__init__.py
+-rw-r--r--   0        0        0     4606 2023-07-02 12:03:58.321652 soccerbars-0.2.1/soccerbars/__main__.py
+-rw-r--r--   0        0        0    30457 2023-07-02 12:03:58.321652 soccerbars-0.2.1/soccerbars/core.py
+-rw-r--r--   0        0        0    10149 1970-01-01 00:00:00.000000 soccerbars-0.2.1/PKG-INFO
```

### Comparing `soccerbars-0.2.0/LICENSE.md` & `soccerbars-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `soccerbars-0.2.0/README.md` & `soccerbars-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Metadata-Version: 2.1
+Name: soccerbars
+Version: 0.2.1
+Summary: Word-sized tallies of association football results using multivariate sparklines based on Gestalt theory (gestaltlines).
+Home-page: https://github.com/meakbiyik/soccerbars
+License: MIT
+Keywords: soccer,sparklines,football,association-football
+Author: M. Eren Akbiyik
+Author-email: erenakbiyik@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: cli
+Requires-Dist: click (>=7.1.2,<8.0.0) ; extra == "cli"
+Requires-Dist: click-help-colors (>=0.9,<0.10) ; extra == "cli"
+Requires-Dist: colorama (>=0.4.4,<0.5.0) ; extra == "cli"
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
+Requires-Dist: numpy (>=1.24.0,<2.0.0)
+Requires-Dist: pandas (>=2.0.3,<3.0.0) ; extra == "cli"
+Project-URL: Repository, https://github.com/meakbiyik/soccerbars
+Description-Content-Type: text/markdown
+
 
 <!-- markdownlint-disable MD033 -->
 # soccerbars <img width="90em" height="24em" src="https://raw.githubusercontent.com/meakbiyik/soccerbars/master/resources/example.png">
 
 <!-- badges: start -->
 [![R CMD check](https://github.com/meakbiyik/soccerbars/workflows/R%20CMD%20check/badge.svg)](https://github.com/meakbiyik/soccerbars/actions)
 [![Python package](https://github.com/meakbiyik/soccerbars/workflows/Python%20package/badge.svg)](https://github.com/meakbiyik/soccerbars/actions)
@@ -144,14 +170,20 @@
 
 ### As a Python package
 
 ```bash
 pip install soccerbars
 ```
 
+For command line usage, you need to install the package with the `cli` extra.
+
+```bash
+pip install soccerbars[cli]
+```
+
 ### As an R package
 
 This package is not published in CRAN yet, so you need to use the Github installation functionality of `devtools`.
 
 ```R
 devtools::install_github("meakbiyik/soccerbars")
 ```
@@ -168,7 +200,8 @@
     ```
 
 3. Clone this repository to your local, navigate into the folder and run
 
     ```bash
     poetry install --no-dev --extras cli
     ```
+
```

### Comparing `soccerbars-0.2.0/setup.py` & `soccerbars-0.2.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,180 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['soccerbars']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['matplotlib>=3.3.3,<4.0.0', 'numpy==1.19.3']
-
-extras_require = \
-{'cli': ['click>=7.1.2,<8.0.0',
-         'colorama>=0.4.4,<0.5.0',
-         'click-help-colors>=0.8,<0.9',
-         'pandas>=1.1.5,<2.0.0']}
-
-entry_points = \
-{'console_scripts': ['soccerbars = soccerbars.__main__:cli']}
-
-setup_kwargs = {
-    'name': 'soccerbars',
-    'version': '0.2.0',
-    'description': 'Word-sized tallies of association football results using multivariate sparklines based on Gestalt theory (gestaltlines).',
-    'long_description': '\n<!-- markdownlint-disable MD033 -->\n# soccerbars <img width="90em" height="24em" src="https://raw.githubusercontent.com/meakbiyik/soccerbars/master/resources/example.png">\n\n<!-- badges: start -->\n[![R CMD check](https://github.com/meakbiyik/soccerbars/workflows/R%20CMD%20check/badge.svg)](https://github.com/meakbiyik/soccerbars/actions)\n[![Python package](https://github.com/meakbiyik/soccerbars/workflows/Python%20package/badge.svg)](https://github.com/meakbiyik/soccerbars/actions)\n<!-- To include when the repo becomes public.\n[![Codecov test coverage](https://codecov.io/gh/meakbiyik/soccerbars/branch/master/graph/badge.svg)](https://codecov.io/gh/meakbiyik/soccerbars?branch=master)\n-->\n<!-- badges: end -->\n\nWord-sized tallies of association football results using multivariate sparklines based on Gestalt theory (gestaltlines).\n\nThis repository contains a Python package, an R package, and a command line tool based on Python.\n\nSoccerbars is created by Prof. Dr. Ulrik Brandes of ETH Zürich and this repository is a port of his [LaTeX package](https://github.com/ubrandes-ethz/soccerbars). An introduction to the theory behind this work can be found [here](https://sn.ethz.ch/research/soccerbars.html).\n\n## Usage\n\nThe signature of the main function `soccerbar` is identical in both Python and R implementations. The input (`scores` argument) can be either a list of matches in the form ```(home_team_score: integer, away_team_score: integer, away_game: boolean)```, a list of three same-length score lists with the same types as the previous scheme, or common data frame objects of each language (`pandas.DataFrame` in Python and `data.frame` in R). A list of these entities can also be given as input if multiple leagues/tournaments are wanted to be plotted.\n\nBoth languages preserve the flags and the `color` arguments from the LaTeX package, and also expose a series of common parameters as keyword arguments. `output_path` and `show` arguments can be used to determine whether the call is to save the resulting image to the given path(s), or just to show it via the available graphical interface (not possible in Python if the function is called from the command line). In both cases, the functions return the plotted objects (`matplotlib.Axes` object(s) in Python and `ggplot` object(s) in R).\n\nFor `color` and `output_path` arguments, the function expects the structure of these to be consistent with the `scores` argument: if multiple lists of match lists are given, then for each such list an output path and a list of colors must be specified, therefore the lengths must be equal in all levels. These arguments are optional, when not provided the configuration will use the LaTeX defaults. Also, the `color` argument should not be necessary in most cases, as the color-related keyword arguments provide sufficient flexibility with much easier usage in both languages (see [Parameters](#parameters) below for more details).\n\n### in Python\n\nGive the matches to the ```soccerbar``` function as an iterable of matches in row-wise, column-wise or DataFrame format. A list of values following these formats (e.g. in the context of multiple leagues) are also accepted without mixing.\n\n```python\nfrom soccerbars import soccerbar\n\n# Row-wise format\nsoccerbar([\n    (1, 2, True), (3, 4, False), (5, 6, True), (7, 8, False)\n])\n# Column-wise format\nsoccerbar([\n    (1, 3, 5, 7), \n    (2, 4, 6, 8), \n    (True, False, True, False)\n], outlined=True, output_path="matches.png")\n# List of row-wise inputs: observe that both color and output_path\n# parameters match with the scores\nsoccerbar([\n    [(1, 2, True), (3, 4, False)], \n    [(5, 6, True), (7, 8, False)]\n    ],\n    color=[("r", "b"), ("g", "y")],\n    output_path=["league1.png", "league2.png"]\n)\n# Input as pandas DataFrame\nimport pandas as pd\n\nsoccerbar(pd.DataFrame([\n    (1, 2, True), (3, 4, False), (5, 6, True), (7, 8, False)\n]), home_color="red")\n```\n\n### in R\n\nSimilarly with its Python counterpart, ```soccerbar``` admits both list of match score lists, and a list of three vectors, along with `data.frame` objects. A list of these (e.g. in the context of multiple leagues) are also allowed.\n\n```R\nlibrary(soccerbars)\n\n# Row-wise format\nsoccerbar(list(\n    list(1, 2, TRUE), list(3, 4, FALSE), list(5, 6, TRUE), list(7, 8, FALSE)\n))\n# Column-wise (vector) format\nsoccerbar(list(\n    c(1, 3, 5, 7),\n    c(2, 4, 6, 8),\n    c(TRUE, FALSE, TRUE, FALSE)\n), outlined = TRUE, output_path = "matches.png")\n# List of column-wise inputs: observe that both color and output_path\n# parameters match with the scores\nsoccerbar(list(\n    list(c(1, 3), c(2, 4), c(TRUE, FALSE)), \n    list(c(5, 7), c(6, 8), c(TRUE, FALSE))\n    ),\n    color = list(c("red", "blue"), c("green", "yellow")),\n    output_path = c("league1.png", "league2.png")\n)\n# Input as data.frame object\nsoccerbar(data.frame(\n    c(1, 3, 5, 7),\n    c(2, 4, 6, 8),\n    c(TRUE, FALSE, TRUE, FALSE)\n), home_color = "red")\n```\n\n### via CLI\n\nAfter installing the package (see the instructions [below](#as-a-command-line-tool)), navigate into the folder and run\n\n```bash\npoetry run soccerbars --help\n```\n\nto see the available options. The CLI is a thin wrapper around the Python API, and writes the output image to the specified location with the `--output-path` argument. Input syntax is identical with the LaTeX package. In addition to the capabilities of the Python core, CLI can also admit a glob pattern to match with `.csv` files.\n\n```bash\n# Vanilla usage\npoetry run soccerbars "(1-2) (3-1)* (2-2)"\n# Specifying the output path (default is "output.png")\npoetry run soccerbars -o out.tiff "(1-2) (3-1)* (2-2)"\n# Reading from a .csv file and specifying an output file\npoetry run soccerbars matches.csv -o matches.pdf\n# Reading from a glob of csv files and saving the output images to a directory\npoetry run soccerbars *.csv -o ".\\output-dir"\n# `-t`, `-z`, `-ol` flags stand for twogoalline, zerodots and outlined options\n# `-p` option can be used to specify additional parameters with syntax key:value\npoetry run soccerbars -z -ol -p fill_color:"(1,1,1,1)" -p home_color:red *.csv\n```\n\n### Parameters\n\nThese parameters can be used to customize the output images in all components.\n\n| Parameter | Description | Default |\n|-|-|-|\n| dpi | Dots per inch resolution | 300 |\n| thickness | Line thickness in cartesian coordinates | 0.36 |\n| edge_thickness  | Edge thickness for outlined patches (when outlined=True) as the ratio to the line thickness | 0.35 |\n| goalless_edge_thickness  | Edge thickness for outlined no-goal patches (when outlined=True) as the ratio to the line thickness | 0.5 |\n| zerodot | Zero-dot diameter ratio to thickness (when zerodots=True) | 0.6 |\n| slant | Slope for unbalanced scores in degrees | 14 |\n| spacing | Spacing between matches in cartesian coordinates | 0.9 |\n| padding | Padding before and after the matches in cartesian coordinates | 0.2 |\n| baseline_factor | Thickness of baseline with respect to line thickness | 0.2 |\n| away_brighter | Set away game colors 33% brighter (when outlined=False) | True |\n| away_darker | Set away game colors 33% darker (when outlined=False, setting this flag will turn "away_brighter" off) | False |\n| transparent_background | Set the background transparent instead of white | False |\n| home_color | Color of home match lines (in Python: matplotlib-acceptable formats, in R: any of the three kinds of R color specifications; either a color name as listed by colors(), a hexadecimal string of the form "#rrggbb" or "#rrggbbaa", or a positive integer i meaning `palette()[i]`) | #000000FF |\n| away_color | Color of away match lines | #000000FF |\n| baseline_color | Color of baselines | #000000FF |\n| fill_color | Fill color for the outlined sparklines | #00000000 |\n| clip_slanted_lines | Clip the ends of the slanted lines | True |\n\n## Installation\n\n### As a Python package\n\n```bash\npip install soccerbars\n```\n\n### As an R package\n\nThis package is not published in CRAN yet, so you need to use the Github installation functionality of `devtools`.\n\n```R\ndevtools::install_github("meakbiyik/soccerbars")\n```\n\n### As a command line tool\n\nAlthough it is possible to use the command line interface after installing the Python package into the current environment and running `python -m soccerbars`, installation as an isolated tool might be preferrable to keep the environment clean. Following steps will create a new environment and install `soccerbars` for this purpose.\n\n1. Install Python from [here](https://www.python.org/downloads/)\n2. Install [Poetry](https://python-poetry.org/), a dependency management tool for Python, via the following command\n\n    ```bash\n    curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python\n    ```\n\n3. Clone this repository to your local, navigate into the folder and run\n\n    ```bash\n    poetry install --no-dev --extras cli\n    ```\n',
-    'author': 'M. Eren Akbiyik',
-    'author_email': 'erenakbiyik@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/meakbiyik/soccerbars',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
+
+<!-- markdownlint-disable MD033 -->
+# soccerbars <img width="90em" height="24em" src="https://raw.githubusercontent.com/meakbiyik/soccerbars/master/resources/example.png">
+
+<!-- badges: start -->
+[![R CMD check](https://github.com/meakbiyik/soccerbars/workflows/R%20CMD%20check/badge.svg)](https://github.com/meakbiyik/soccerbars/actions)
+[![Python package](https://github.com/meakbiyik/soccerbars/workflows/Python%20package/badge.svg)](https://github.com/meakbiyik/soccerbars/actions)
+<!-- To include when the repo becomes public.
+[![Codecov test coverage](https://codecov.io/gh/meakbiyik/soccerbars/branch/master/graph/badge.svg)](https://codecov.io/gh/meakbiyik/soccerbars?branch=master)
+-->
+<!-- badges: end -->
+
+Word-sized tallies of association football results using multivariate sparklines based on Gestalt theory (gestaltlines).
+
+This repository contains a Python package, an R package, and a command line tool based on Python.
+
+Soccerbars is created by Prof. Dr. Ulrik Brandes of ETH Zürich and this repository is a port of his [LaTeX package](https://github.com/ubrandes-ethz/soccerbars). An introduction to the theory behind this work can be found [here](https://sn.ethz.ch/research/soccerbars.html).
+
+## Usage
+
+The signature of the main function `soccerbar` is identical in both Python and R implementations. The input (`scores` argument) can be either a list of matches in the form ```(home_team_score: integer, away_team_score: integer, away_game: boolean)```, a list of three same-length score lists with the same types as the previous scheme, or common data frame objects of each language (`pandas.DataFrame` in Python and `data.frame` in R). A list of these entities can also be given as input if multiple leagues/tournaments are wanted to be plotted.
+
+Both languages preserve the flags and the `color` arguments from the LaTeX package, and also expose a series of common parameters as keyword arguments. `output_path` and `show` arguments can be used to determine whether the call is to save the resulting image to the given path(s), or just to show it via the available graphical interface (not possible in Python if the function is called from the command line). In both cases, the functions return the plotted objects (`matplotlib.Axes` object(s) in Python and `ggplot` object(s) in R).
+
+For `color` and `output_path` arguments, the function expects the structure of these to be consistent with the `scores` argument: if multiple lists of match lists are given, then for each such list an output path and a list of colors must be specified, therefore the lengths must be equal in all levels. These arguments are optional, when not provided the configuration will use the LaTeX defaults. Also, the `color` argument should not be necessary in most cases, as the color-related keyword arguments provide sufficient flexibility with much easier usage in both languages (see [Parameters](#parameters) below for more details).
+
+### in Python
+
+Give the matches to the ```soccerbar``` function as an iterable of matches in row-wise, column-wise or DataFrame format. A list of values following these formats (e.g. in the context of multiple leagues) are also accepted without mixing.
+
+```python
+from soccerbars import soccerbar
+
+# Row-wise format
+soccerbar([
+    (1, 2, True), (3, 4, False), (5, 6, True), (7, 8, False)
+])
+# Column-wise format
+soccerbar([
+    (1, 3, 5, 7), 
+    (2, 4, 6, 8), 
+    (True, False, True, False)
+], outlined=True, output_path="matches.png")
+# List of row-wise inputs: observe that both color and output_path
+# parameters match with the scores
+soccerbar([
+    [(1, 2, True), (3, 4, False)], 
+    [(5, 6, True), (7, 8, False)]
+    ],
+    color=[("r", "b"), ("g", "y")],
+    output_path=["league1.png", "league2.png"]
+)
+# Input as pandas DataFrame
+import pandas as pd
+
+soccerbar(pd.DataFrame([
+    (1, 2, True), (3, 4, False), (5, 6, True), (7, 8, False)
+]), home_color="red")
+```
+
+### in R
+
+Similarly with its Python counterpart, ```soccerbar``` admits both list of match score lists, and a list of three vectors, along with `data.frame` objects. A list of these (e.g. in the context of multiple leagues) are also allowed.
+
+```R
+library(soccerbars)
+
+# Row-wise format
+soccerbar(list(
+    list(1, 2, TRUE), list(3, 4, FALSE), list(5, 6, TRUE), list(7, 8, FALSE)
+))
+# Column-wise (vector) format
+soccerbar(list(
+    c(1, 3, 5, 7),
+    c(2, 4, 6, 8),
+    c(TRUE, FALSE, TRUE, FALSE)
+), outlined = TRUE, output_path = "matches.png")
+# List of column-wise inputs: observe that both color and output_path
+# parameters match with the scores
+soccerbar(list(
+    list(c(1, 3), c(2, 4), c(TRUE, FALSE)), 
+    list(c(5, 7), c(6, 8), c(TRUE, FALSE))
+    ),
+    color = list(c("red", "blue"), c("green", "yellow")),
+    output_path = c("league1.png", "league2.png")
+)
+# Input as data.frame object
+soccerbar(data.frame(
+    c(1, 3, 5, 7),
+    c(2, 4, 6, 8),
+    c(TRUE, FALSE, TRUE, FALSE)
+), home_color = "red")
+```
+
+### via CLI
+
+After installing the package (see the instructions [below](#as-a-command-line-tool)), navigate into the folder and run
+
+```bash
+poetry run soccerbars --help
+```
+
+to see the available options. The CLI is a thin wrapper around the Python API, and writes the output image to the specified location with the `--output-path` argument. Input syntax is identical with the LaTeX package. In addition to the capabilities of the Python core, CLI can also admit a glob pattern to match with `.csv` files.
+
+```bash
+# Vanilla usage
+poetry run soccerbars "(1-2) (3-1)* (2-2)"
+# Specifying the output path (default is "output.png")
+poetry run soccerbars -o out.tiff "(1-2) (3-1)* (2-2)"
+# Reading from a .csv file and specifying an output file
+poetry run soccerbars matches.csv -o matches.pdf
+# Reading from a glob of csv files and saving the output images to a directory
+poetry run soccerbars *.csv -o ".\output-dir"
+# `-t`, `-z`, `-ol` flags stand for twogoalline, zerodots and outlined options
+# `-p` option can be used to specify additional parameters with syntax key:value
+poetry run soccerbars -z -ol -p fill_color:"(1,1,1,1)" -p home_color:red *.csv
+```
+
+### Parameters
+
+These parameters can be used to customize the output images in all components.
+
+| Parameter | Description | Default |
+|-|-|-|
+| dpi | Dots per inch resolution | 300 |
+| thickness | Line thickness in cartesian coordinates | 0.36 |
+| edge_thickness  | Edge thickness for outlined patches (when outlined=True) as the ratio to the line thickness | 0.35 |
+| goalless_edge_thickness  | Edge thickness for outlined no-goal patches (when outlined=True) as the ratio to the line thickness | 0.5 |
+| zerodot | Zero-dot diameter ratio to thickness (when zerodots=True) | 0.6 |
+| slant | Slope for unbalanced scores in degrees | 14 |
+| spacing | Spacing between matches in cartesian coordinates | 0.9 |
+| padding | Padding before and after the matches in cartesian coordinates | 0.2 |
+| baseline_factor | Thickness of baseline with respect to line thickness | 0.2 |
+| away_brighter | Set away game colors 33% brighter (when outlined=False) | True |
+| away_darker | Set away game colors 33% darker (when outlined=False, setting this flag will turn "away_brighter" off) | False |
+| transparent_background | Set the background transparent instead of white | False |
+| home_color | Color of home match lines (in Python: matplotlib-acceptable formats, in R: any of the three kinds of R color specifications; either a color name as listed by colors(), a hexadecimal string of the form "#rrggbb" or "#rrggbbaa", or a positive integer i meaning `palette()[i]`) | #000000FF |
+| away_color | Color of away match lines | #000000FF |
+| baseline_color | Color of baselines | #000000FF |
+| fill_color | Fill color for the outlined sparklines | #00000000 |
+| clip_slanted_lines | Clip the ends of the slanted lines | True |
+
+## Installation
+
+### As a Python package
+
+```bash
+pip install soccerbars
+```
+
+For command line usage, you need to install the package with the `cli` extra.
+
+```bash
+pip install soccerbars[cli]
+```
+
+### As an R package
+
+This package is not published in CRAN yet, so you need to use the Github installation functionality of `devtools`.
+
+```R
+devtools::install_github("meakbiyik/soccerbars")
+```
+
+### As a command line tool
+
+Although it is possible to use the command line interface after installing the Python package into the current environment and running `python -m soccerbars`, installation as an isolated tool might be preferrable to keep the environment clean. Following steps will create a new environment and install `soccerbars` for this purpose.
+
+1. Install Python from [here](https://www.python.org/downloads/)
+2. Install [Poetry](https://python-poetry.org/), a dependency management tool for Python, via the following command
+
+    ```bash
+    curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python
+    ```
+
+3. Clone this repository to your local, navigate into the folder and run
+
+    ```bash
+    poetry install --no-dev --extras cli
+    ```
```

