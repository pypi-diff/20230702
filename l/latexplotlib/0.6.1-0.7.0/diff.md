# Comparing `tmp/latexplotlib-0.6.1.tar.gz` & `tmp/latexplotlib-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latexplotlib-0.6.1.tar", last modified: Sat Apr 29 20:42:05 2023, max compression
+gzip compressed data, was "latexplotlib-0.7.0.tar", last modified: Sun Jul  2 13:37:18 2023, max compression
```

## Comparing `latexplotlib-0.6.1.tar` & `latexplotlib-0.7.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:42:05.064110 latexplotlib-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-04-29 20:42:05.064110 latexplotlib-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 20:42:05.064110 latexplotlib-0.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:42:05.060110 latexplotlib-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:42:05.060110 latexplotlib-0.6.1/src/latexplotlib/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/src/latexplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/src/latexplotlib/_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/src/latexplotlib/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/src/latexplotlib/_latexplotlib.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/src/latexplotlib/_styles.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/src/latexplotlib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/src/latexplotlib/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:42:05.064110 latexplotlib-0.6.1/src/latexplotlib/styles/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/src/latexplotlib/styles/latex10pt-minimal.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/src/latexplotlib/styles/latex10pt.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/src/latexplotlib/styles/latex11pt-minimal.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/src/latexplotlib/styles/latex11pt.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/src/latexplotlib/styles/latex12pt-minimal.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/src/latexplotlib/styles/latex12pt.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/src/latexplotlib/styles/latex9pt-minimal.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/src/latexplotlib/styles/latex9pt.mplstyle
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:42:05.060110 latexplotlib-0.6.1/src/latexplotlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-04-29 20:42:05.000000 latexplotlib-0.6.1/src/latexplotlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-29 20:42:05.000000 latexplotlib-0.6.1/src/latexplotlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 20:42:05.000000 latexplotlib-0.6.1/src/latexplotlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-29 20:42:05.000000 latexplotlib-0.6.1/src/latexplotlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-29 20:42:05.000000 latexplotlib-0.6.1/src/latexplotlib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:42:05.064110 latexplotlib-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/tests/test_00_styles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/tests/test_10_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/tests/test_20_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/tests/test_30_latexplotlib.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-29 20:41:46.000000 latexplotlib-0.6.1/tests/test_styles_available.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:37:18.172509 latexplotlib-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-02 13:36:54.000000 latexplotlib-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-07-02 13:37:18.172509 latexplotlib-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-07-02 13:36:54.000000 latexplotlib-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-02 13:36:54.000000 latexplotlib-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 13:37:18.172509 latexplotlib-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:37:18.168509 latexplotlib-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:37:18.168509 latexplotlib-0.7.0/src/latexplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-02 13:36:54.000000 latexplotlib-0.7.0/src/latexplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-02 13:36:54.000000 latexplotlib-0.7.0/src/latexplotlib/_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-07-02 13:36:54.000000 latexplotlib-0.7.0/src/latexplotlib/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-07-02 13:36:54.000000 latexplotlib-0.7.0/src/latexplotlib/_latexplotlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-02 13:36:54.000000 latexplotlib-0.7.0/src/latexplotlib/_styles.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-02 13:36:54.000000 latexplotlib-0.7.0/src/latexplotlib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:36:54.000000 latexplotlib-0.7.0/src/latexplotlib/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:37:18.172509 latexplotlib-0.7.0/src/latexplotlib/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-02 13:36:54.000000 latexplotlib-0.7.0/src/latexplotlib/styles/latex10pt-minimal.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-02 13:36:54.000000 latexplotlib-0.7.0/src/latexplotlib/styles/latex10pt.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-02 13:36:54.000000 latexplotlib-0.7.0/src/latexplotlib/styles/latex11pt-minimal.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-02 13:36:54.000000 latexplotlib-0.7.0/src/latexplotlib/styles/latex11pt.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-02 13:36:54.000000 latexplotlib-0.7.0/src/latexplotlib/styles/latex12pt-minimal.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-02 13:36:54.000000 latexplotlib-0.7.0/src/latexplotlib/styles/latex12pt.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-02 13:36:54.000000 latexplotlib-0.7.0/src/latexplotlib/styles/latex9pt-minimal.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-02 13:36:54.000000 latexplotlib-0.7.0/src/latexplotlib/styles/latex9pt.mplstyle
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:37:18.168509 latexplotlib-0.7.0/src/latexplotlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-07-02 13:37:18.000000 latexplotlib-0.7.0/src/latexplotlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-02 13:37:18.000000 latexplotlib-0.7.0/src/latexplotlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 13:37:18.000000 latexplotlib-0.7.0/src/latexplotlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-02 13:37:18.000000 latexplotlib-0.7.0/src/latexplotlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-02 13:37:18.000000 latexplotlib-0.7.0/src/latexplotlib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:37:18.172509 latexplotlib-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-02 13:36:54.000000 latexplotlib-0.7.0/tests/test_00_styles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-07-02 13:36:54.000000 latexplotlib-0.7.0/tests/test_10_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-02 13:36:54.000000 latexplotlib-0.7.0/tests/test_20_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-07-02 13:36:54.000000 latexplotlib-0.7.0/tests/test_30_latexplotlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-02 13:36:54.000000 latexplotlib-0.7.0/tests/test_plt_available.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-02 13:36:54.000000 latexplotlib-0.7.0/tests/test_styles_available.py
```

### Comparing `latexplotlib-0.6.1/LICENSE` & `latexplotlib-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `latexplotlib-0.6.1/PKG-INFO` & `latexplotlib-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: latexplotlib
-Version: 0.6.1
+Version: 0.7.0
 Summary: Perfect matplotlib figures for latex
 Author-email: Constantin Gahr <latexplotlib.gvxel@aleeas.com>
 License: MIT
+Project-URL: Changelog, https://github.com/cgahr/latexplotlib/blob/main/CHANGES.md
 Project-URL: Homepage, https://github.com/cgahr/latexplotlib
 Project-URL: Issues, https://github.com/cgahr/latexplotlib/issues
 Keywords: latex,matplotlib-figures,matplotlib-style-sheets,matplotlib-styles,python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -38,19 +39,19 @@
 ```python
 pip install latexplotlib
 ```
 2. import latexplotlib and use latexplotlib style
 ```python
 import latexplotlib as lpl
 
-plt.style.use('latex10pt')
+lpl.style.use('latex10pt')
 # lpl.style.use('latex10pt-minimal')
 ```
 
-3. replace all `plt.subplots` with `lpl.subplots`:
+3. replace all usages of `plt` with `lpl`. Only `plt.subplots` changes its behavior:
 ```python
 #  fig, axes = plt.subplots(2, 3)
 fig, axes = lpl.subplots(2, 3)
 ```
 
 Optional:
 
@@ -87,15 +88,15 @@
 
 ```python
 import matplotlib.pyplot as plt
 import numpy as np
 
 import latexplotlib as lpl
 
-plt.style.use("latex10pt-minimal")
+lpl.style.use("latex10pt-minimal")
 # lpl.size.set(200, 400)
 with lpl.size.context(200, 400):
     fig, ax = lpl.subplots(1, 1)
 
 x = np.linspace(1, 5, 100)
 
 for t in range(4):
@@ -103,32 +104,31 @@
     ax.plot(x, x ** t, label=label)
 
 ax.set_yscale("log")
 ax.set_title("Perfect matplotlib figures for \\LaTeX")
 ax.grid()
 
 fig.legend()
-plt.savefig("example_poly_minimal")
-plt.savefig("example_poly_minimal.png")
+fig.savefig("example_poly_minimal")
+fig.savefig("example_poly_minimal.png")
 ```
 
 <p align="center">
 <img src="https://github.com/ConstantinGahr/latexplotlib/blob/main/examples/example_poly_minimal.png?raw=true" width="500">
 </p>
 
 
 The non-minimal versions set additional defaults to create figures that are accessible for color-blind people:
 
 ```python
 import matplotlib.pyplot as plt
 import numpy as np
-import latexplotlib as lpl
 
 
-plt.style.use("latex10pt")
+lpl.style.use("latex10pt")
 
 # lpl.size.set(200, 400)
 with lpl.size.context(200, 400):
     fig, ax = lpl.subplots(1, 1)
 
 x = np.linspace(1, 5, 100)
 
@@ -147,15 +147,15 @@
 <p align="center">
 <img src="https://github.com/ConstantinGahr/latexplotlib/blob/main/examples/example_poly.png?raw=true" width="500">
 </p>
 
 Both styles change the defaults of the `plt.savefig` command. The new defaults are
 
 ```python
-plt.savefig(
+lpl.savefig(
     ...,
     bbox_inches=None,
     dpi=300,
     format="pdf",
     orientation="portrait",
     pad_inches=0.05
 )
@@ -181,16 +181,14 @@
     lpl.size()  # 100, 200
 
 lpl.size()  # (200, 400)
 ```
 
 ### Create figures for latex
 ```python
-import matplotlib.pyplot as plt
-
 import latexplotlib as lpl
 
 
 # A figure filling 75% of the latex page
 _ = lpl.subplots(1, 1)
 
 # A subplot filling 80% of the latex page
@@ -200,16 +198,14 @@
 fig, axes = lpl.subplots(1, 3, scale=0.8, aspect='equal')
 ```
 
 ### `aspect` keyword
 The `aspect` keyword controls the ratio of height to width. The default is the Golden ratio. `aspect` can also be `equal` (i.e. `aspect=1` )or `auto`. In the latter case, the figure fills the available space.
 
 ```python
-import matplotlib.pyplot as plt
-
 import latexplotlib as lpl
 
 # A 3 by 2 figure where each subplots height to width ratio is the golden ratio
 fig, axes = lpl.subplots(3, 2)
 
 # A 3 by 2 figure where each subplot having a height to width ratio of 1:1
 fig, axes = lpl.subplots(3, 2, aspect=1.0)
@@ -220,28 +216,28 @@
 ```
 
 
 ### Include figures in Latex
 
 The most important part of including the figures in latex is to not set the size of the figure using arguments like `[width=...]`:
 ```latex
-\includegraphics[width=\textwidth]{test.pdf}
+\includegraphics{test.pdf}
 ```
-
-Instead, latexplotlib creates figures that are already properly sized. As such, figure can be added using only
+Observe that we did NOT adjust the size using arguments like `[width=...]`:
 ```latex
-\includegraphics}{test.pdf}
+\includegraphics[width=\textwidth]{test.pdf}
 ```
 
 ### `plt.tight_layout()`
 
-`plt.tight_layout()` changes the size of the produced figure. As such it is recommended to not use `plt.tight_layout()` with care! The same is true for `savefig(..., bbox_inches=None)`!
+`plt.tight_layout()` changes the size of the produced figure. As such it is recommended to not use `plt.tight_layout()` at all! The same is true for `savefig(..., bbox_inches=None)`!
 
 Instead all latexplotlib styles used `constrained_layout` by default. `constrained_layout` has a similar functionality compared to `tight_layout`, however it is fully deterministic and does not change the size of the underlying figure.
 
 ## References
 
 This package is inspired by the following sources:
 
 - Code: https://pypi.org/project/SciencePlots/
 - Figure sizes: https://jwalton.info/Embed-Publication-Matplotlib-Latex/
 - Color palette (Okabe Ito): https://clauswilke.com/dataviz/color-basics.html
+- Golden ratio: https://en.wikipedia.org/wiki/Golden_ratio
```

#### html2text {}

```diff
@@ -1,95 +1,95 @@
-Metadata-Version: 2.1 Name: latexplotlib Version: 0.6.1 Summary: Perfect
+Metadata-Version: 2.1 Name: latexplotlib Version: 0.7.0 Summary: Perfect
 matplotlib figures for latex Author-email: Constantin Gahr
-gvxel@aleeas.com> License: MIT Project-URL: Homepage, https://github.com/cgahr/
-latexplotlib Project-URL: Issues, https://github.com/cgahr/latexplotlib/issues
-Keywords: latex,matplotlib-figures,matplotlib-style-sheets,matplotlib-
-styles,python Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: License :: OSI Approved ::
-MIT License Classifier: Operating System :: OS Independent Requires-Python:
->=3.7.1 Description-Content-Type: text/markdown Provides-Extra: tests License-
-File: LICENSE # latexplotlib [![image](https://img.shields.io/pypi/v/
-latexplotlib.svg)](https://pypi.python.org/pypi/latexplotlib) [![image](https:/
-/img.shields.io/pypi/l/latexplotlib.svg)](https://pypi.python.org/pypi/
-latexplotlib) [![image](https://img.shields.io/pypi/pyversions/
-latexplotlib.svg)](https://pypi.python.org/pypi/latexplotlib) [![Actions
-status](https://github.com/cgahr/latexplotlib/actions/workflows/main.yml/
-badge.svg)](https://github.com/cgahr/latexplotlib/actions) [![Coverage Status]
-(https://coveralls.io/repos/github/cgahr/latexplotlib/badge.svg?branch=main)]
-(https://coveralls.io/github/cgahr/latexplotlib?branch=main) [Code_style:
-black] [![Ruff](https://img.shields.io/endpoint?url=https://
-raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https:
-//github.com/charliermarsh/ruff) Perfect matplotlib figures for latex. ##
-Quickstart 1. install `latexplotlib`: ```python pip install latexplotlib ``` 2.
-import latexplotlib and use latexplotlib style ```python import latexplotlib as
-lpl plt.style.use('latex10pt') # lpl.style.use('latex10pt-minimal') ``` 3.
-replace all `plt.subplots` with `lpl.subplots`: ```python # fig, axes =
-plt.subplots(2, 3) fig, axes = lpl.subplots(2, 3) ``` Optional: 4. get size of
-latex document ```latex (\the\textwidth, \the\textheight) % (412.123pt,
-346.564pt) ``` 5. set `lpl.size` to size of latex document ```python
-lpl.size.set(412.123, 346.564) ``` ## Usage This package has two basic
-functionalities. On the one hand, it sets sensible defaults for creating
-perfect figures for latex. This includes a color scheme optimized for color-
-blind people, correct font and font sizes, and sensible defaults to store the
-figure. On the other hand, it provides some functions to create perfectly sized
-figures. These figures fit your latex document without scaling and have the
-correct font size for your document. ### latexplotlib styles There are 6
-different styles for matplotlib: - `latex10pt-minimal` - `latex11pt-minimal` -
-`latex12pt-minimal` - `latex10pt` - `latex11pt` - `latex12pt` The `*minimal`
-versions change the font and the font sizes to ensure that the figures fonts
-match the latex font. This style is fully compatible with other styles:
-```python import matplotlib.pyplot as plt import numpy as np import
-latexplotlib as lpl plt.style.use("latex10pt-minimal") # lpl.size.set(200, 400)
-with lpl.size.context(200, 400): fig, ax = lpl.subplots(1, 1) x = np.linspace
-(1, 5, 100) for t in range(4): label = f"$x^{t}$" ax.plot(x, x ** t,
-label=label) ax.set_yscale("log") ax.set_title("Perfect matplotlib figures for
-\\LaTeX") ax.grid() fig.legend() plt.savefig("example_poly_minimal")
-plt.savefig("example_poly_minimal.png") ```
+gvxel@aleeas.com> License: MIT Project-URL: Changelog, https://github.com/
+cgahr/latexplotlib/blob/main/CHANGES.md Project-URL: Homepage, https://
+github.com/cgahr/latexplotlib Project-URL: Issues, https://github.com/cgahr/
+latexplotlib/issues Keywords: latex,matplotlib-figures,matplotlib-style-
+sheets,matplotlib-styles,python Classifier: Programming Language :: Python ::
+3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7.1 Description-Content-Type: text/markdown Provides-
+Extra: tests License-File: LICENSE # latexplotlib [![image](https://
+img.shields.io/pypi/v/latexplotlib.svg)](https://pypi.python.org/pypi/
+latexplotlib) [![image](https://img.shields.io/pypi/l/latexplotlib.svg)](https:
+//pypi.python.org/pypi/latexplotlib) [![image](https://img.shields.io/pypi/
+pyversions/latexplotlib.svg)](https://pypi.python.org/pypi/latexplotlib) [!
+[Actions status](https://github.com/cgahr/latexplotlib/actions/workflows/
+main.yml/badge.svg)](https://github.com/cgahr/latexplotlib/actions) [![Coverage
+Status](https://coveralls.io/repos/github/cgahr/latexplotlib/
+badge.svg?branch=main)](https://coveralls.io/github/cgahr/
+latexplotlib?branch=main) [Code_style:_black] [![Ruff](https://img.shields.io/
+endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/
+badge/v1.json)](https://github.com/charliermarsh/ruff) Perfect matplotlib
+figures for latex. ## Quickstart 1. install `latexplotlib`: ```python pip
+install latexplotlib ``` 2. import latexplotlib and use latexplotlib style
+```python import latexplotlib as lpl lpl.style.use('latex10pt') # lpl.style.use
+('latex10pt-minimal') ``` 3. replace all usages of `plt` with `lpl`. Only
+`plt.subplots` changes its behavior: ```python # fig, axes = plt.subplots(2, 3)
+fig, axes = lpl.subplots(2, 3) ``` Optional: 4. get size of latex document
+```latex (\the\textwidth, \the\textheight) % (412.123pt, 346.564pt) ``` 5. set
+`lpl.size` to size of latex document ```python lpl.size.set(412.123, 346.564)
+``` ## Usage This package has two basic functionalities. On the one hand, it
+sets sensible defaults for creating perfect figures for latex. This includes a
+color scheme optimized for color-blind people, correct font and font sizes, and
+sensible defaults to store the figure. On the other hand, it provides some
+functions to create perfectly sized figures. These figures fit your latex
+document without scaling and have the correct font size for your document. ###
+latexplotlib styles There are 6 different styles for matplotlib: - `latex10pt-
+minimal` - `latex11pt-minimal` - `latex12pt-minimal` - `latex10pt` -
+`latex11pt` - `latex12pt` The `*minimal` versions change the font and the font
+sizes to ensure that the figures fonts match the latex font. This style is
+fully compatible with other styles: ```python import matplotlib.pyplot as plt
+import numpy as np import latexplotlib as lpl lpl.style.use("latex10pt-
+minimal") # lpl.size.set(200, 400) with lpl.size.context(200, 400): fig, ax =
+lpl.subplots(1, 1) x = np.linspace(1, 5, 100) for t in range(4): label = f"$x^
+{t}$" ax.plot(x, x ** t, label=label) ax.set_yscale("log") ax.set_title
+("Perfect matplotlib figures for \\LaTeX") ax.grid() fig.legend() fig.savefig
+("example_poly_minimal") fig.savefig("example_poly_minimal.png") ```
       [https://github.com/ConstantinGahr/latexplotlib/blob/main/examples/
                       example_poly_minimal.png?raw=true]
 The non-minimal versions set additional defaults to create figures that are
 accessible for color-blind people: ```python import matplotlib.pyplot as plt
-import numpy as np import latexplotlib as lpl plt.style.use("latex10pt") #
-lpl.size.set(200, 400) with lpl.size.context(200, 400): fig, ax = lpl.subplots
-(1, 1) x = np.linspace(1, 5, 100) for t in range(4): label = f"$x^{t}$" ax.plot
-(x, x ** t, label=label) ax.set_yscale("log") ax.set_title("Perfect matplotlib
-figures for \\LaTeX") ax.grid() fig.legend() fig.savefig("example_poly")
-fig.savefig("example_poly.png") ```
+import numpy as np lpl.style.use("latex10pt") # lpl.size.set(200, 400) with
+lpl.size.context(200, 400): fig, ax = lpl.subplots(1, 1) x = np.linspace(1, 5,
+100) for t in range(4): label = f"$x^{t}$" ax.plot(x, x ** t, label=label)
+ax.set_yscale("log") ax.set_title("Perfect matplotlib figures for \\LaTeX")
+ax.grid() fig.legend() fig.savefig("example_poly") fig.savefig
+("example_poly.png") ```
       [https://github.com/ConstantinGahr/latexplotlib/blob/main/examples/
                           example_poly.png?raw=true]
 Both styles change the defaults of the `plt.savefig` command. The new defaults
-are ```python plt.savefig( ..., bbox_inches=None, dpi=300, format="pdf",
+are ```python lpl.savefig( ..., bbox_inches=None, dpi=300, format="pdf",
 orientation="portrait", pad_inches=0.05 ) ``` ### Get latex dimensions You can
 find the width and height of your document using the following command:
 ```latex \the\textwidth \the\textheight ``` ### Set and get latex page size
 ```python import latexplotlib as lpl lpl.size.set(200, 400) with
 lpl.size.context(100, 200): lpl.size() # 100, 200 lpl.size() # (200, 400) ```
-### Create figures for latex ```python import matplotlib.pyplot as plt import
-latexplotlib as lpl # A figure filling 75% of the latex page _ = lpl.subplots
-(1, 1) # A subplot filling 80% of the latex page fig, axes = lpl.subplots(3, 2,
-scale=0.8) # A subplot for 3 square plots next to each other fig, axes =
-lpl.subplots(1, 3, scale=0.8, aspect='equal') ``` ### `aspect` keyword The
-`aspect` keyword controls the ratio of height to width. The default is the
-Golden ratio. `aspect` can also be `equal` (i.e. `aspect=1` )or `auto`. In the
-latter case, the figure fills the available space. ```python import
-matplotlib.pyplot as plt import latexplotlib as lpl # A 3 by 2 figure where
+### Create figures for latex ```python import latexplotlib as lpl # A figure
+filling 75% of the latex page _ = lpl.subplots(1, 1) # A subplot filling 80% of
+the latex page fig, axes = lpl.subplots(3, 2, scale=0.8) # A subplot for 3
+square plots next to each other fig, axes = lpl.subplots(1, 3, scale=0.8,
+aspect='equal') ``` ### `aspect` keyword The `aspect` keyword controls the
+ratio of height to width. The default is the Golden ratio. `aspect` can also be
+`equal` (i.e. `aspect=1` )or `auto`. In the latter case, the figure fills the
+available space. ```python import latexplotlib as lpl # A 3 by 2 figure where
 each subplots height to width ratio is the golden ratio fig, axes =
 lpl.subplots(3, 2) # A 3 by 2 figure where each subplot having a height to
 width ratio of 1:1 fig, axes = lpl.subplots(3, 2, aspect=1.0) # A figure that
 is exactly 300pt height and 200pt wide with lpl.size.context(200, 300): fig,
 axes = lpl.subplots(3, 2, aspect="auto") ``` ### Include figures in Latex The
 most important part of including the figures in latex is to not set the size of
 the figure using arguments like `[width=...]`: ```latex \includegraphics
-[width=\textwidth]{test.pdf} ``` Instead, latexplotlib creates figures that are
-already properly sized. As such, figure can be added using only ```latex
-\includegraphics}{test.pdf} ``` ### `plt.tight_layout()` `plt.tight_layout()`
-changes the size of the produced figure. As such it is recommended to not use
-`plt.tight_layout()` with care! The same is true for `savefig(...,
-bbox_inches=None)`! Instead all latexplotlib styles used `constrained_layout`
-by default. `constrained_layout` has a similar functionality compared to
-`tight_layout`, however it is fully deterministic and does not change the size
-of the underlying figure. ## References This package is inspired by the
-following sources: - Code: https://pypi.org/project/SciencePlots/ - Figure
-sizes: https://jwalton.info/Embed-Publication-Matplotlib-Latex/ - Color palette
-(Okabe Ito): https://clauswilke.com/dataviz/color-basics.html
+{test.pdf} ``` Observe that we did NOT adjust the size using arguments like `
+[width=...]`: ```latex \includegraphics[width=\textwidth]{test.pdf} ``` ###
+`plt.tight_layout()` `plt.tight_layout()` changes the size of the produced
+figure. As such it is recommended to not use `plt.tight_layout()` at all! The
+same is true for `savefig(..., bbox_inches=None)`! Instead all latexplotlib
+styles used `constrained_layout` by default. `constrained_layout` has a similar
+functionality compared to `tight_layout`, however it is fully deterministic and
+does not change the size of the underlying figure. ## References This package
+is inspired by the following sources: - Code: https://pypi.org/project/
+SciencePlots/ - Figure sizes: https://jwalton.info/Embed-Publication-
+Matplotlib-Latex/ - Color palette (Okabe Ito): https://clauswilke.com/dataviz/
+color-basics.html - Golden ratio: https://en.wikipedia.org/wiki/Golden_ratio
```

### Comparing `latexplotlib-0.6.1/README.md` & `latexplotlib-0.7.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 ```python
 pip install latexplotlib
 ```
 2. import latexplotlib and use latexplotlib style
 ```python
 import latexplotlib as lpl
 
-plt.style.use('latex10pt')
+lpl.style.use('latex10pt')
 # lpl.style.use('latex10pt-minimal')
 ```
 
-3. replace all `plt.subplots` with `lpl.subplots`:
+3. replace all usages of `plt` with `lpl`. Only `plt.subplots` changes its behavior:
 ```python
 #  fig, axes = plt.subplots(2, 3)
 fig, axes = lpl.subplots(2, 3)
 ```
 
 Optional:
 
@@ -66,15 +66,15 @@
 
 ```python
 import matplotlib.pyplot as plt
 import numpy as np
 
 import latexplotlib as lpl
 
-plt.style.use("latex10pt-minimal")
+lpl.style.use("latex10pt-minimal")
 # lpl.size.set(200, 400)
 with lpl.size.context(200, 400):
     fig, ax = lpl.subplots(1, 1)
 
 x = np.linspace(1, 5, 100)
 
 for t in range(4):
@@ -82,32 +82,31 @@
     ax.plot(x, x ** t, label=label)
 
 ax.set_yscale("log")
 ax.set_title("Perfect matplotlib figures for \\LaTeX")
 ax.grid()
 
 fig.legend()
-plt.savefig("example_poly_minimal")
-plt.savefig("example_poly_minimal.png")
+fig.savefig("example_poly_minimal")
+fig.savefig("example_poly_minimal.png")
 ```
 
 <p align="center">
 <img src="https://github.com/ConstantinGahr/latexplotlib/blob/main/examples/example_poly_minimal.png?raw=true" width="500">
 </p>
 
 
 The non-minimal versions set additional defaults to create figures that are accessible for color-blind people:
 
 ```python
 import matplotlib.pyplot as plt
 import numpy as np
-import latexplotlib as lpl
 
 
-plt.style.use("latex10pt")
+lpl.style.use("latex10pt")
 
 # lpl.size.set(200, 400)
 with lpl.size.context(200, 400):
     fig, ax = lpl.subplots(1, 1)
 
 x = np.linspace(1, 5, 100)
 
@@ -126,15 +125,15 @@
 <p align="center">
 <img src="https://github.com/ConstantinGahr/latexplotlib/blob/main/examples/example_poly.png?raw=true" width="500">
 </p>
 
 Both styles change the defaults of the `plt.savefig` command. The new defaults are
 
 ```python
-plt.savefig(
+lpl.savefig(
     ...,
     bbox_inches=None,
     dpi=300,
     format="pdf",
     orientation="portrait",
     pad_inches=0.05
 )
@@ -160,16 +159,14 @@
     lpl.size()  # 100, 200
 
 lpl.size()  # (200, 400)
 ```
 
 ### Create figures for latex
 ```python
-import matplotlib.pyplot as plt
-
 import latexplotlib as lpl
 
 
 # A figure filling 75% of the latex page
 _ = lpl.subplots(1, 1)
 
 # A subplot filling 80% of the latex page
@@ -179,16 +176,14 @@
 fig, axes = lpl.subplots(1, 3, scale=0.8, aspect='equal')
 ```
 
 ### `aspect` keyword
 The `aspect` keyword controls the ratio of height to width. The default is the Golden ratio. `aspect` can also be `equal` (i.e. `aspect=1` )or `auto`. In the latter case, the figure fills the available space.
 
 ```python
-import matplotlib.pyplot as plt
-
 import latexplotlib as lpl
 
 # A 3 by 2 figure where each subplots height to width ratio is the golden ratio
 fig, axes = lpl.subplots(3, 2)
 
 # A 3 by 2 figure where each subplot having a height to width ratio of 1:1
 fig, axes = lpl.subplots(3, 2, aspect=1.0)
@@ -199,28 +194,28 @@
 ```
 
 
 ### Include figures in Latex
 
 The most important part of including the figures in latex is to not set the size of the figure using arguments like `[width=...]`:
 ```latex
-\includegraphics[width=\textwidth]{test.pdf}
+\includegraphics{test.pdf}
 ```
-
-Instead, latexplotlib creates figures that are already properly sized. As such, figure can be added using only
+Observe that we did NOT adjust the size using arguments like `[width=...]`:
 ```latex
-\includegraphics}{test.pdf}
+\includegraphics[width=\textwidth]{test.pdf}
 ```
 
 ### `plt.tight_layout()`
 
-`plt.tight_layout()` changes the size of the produced figure. As such it is recommended to not use `plt.tight_layout()` with care! The same is true for `savefig(..., bbox_inches=None)`!
+`plt.tight_layout()` changes the size of the produced figure. As such it is recommended to not use `plt.tight_layout()` at all! The same is true for `savefig(..., bbox_inches=None)`!
 
 Instead all latexplotlib styles used `constrained_layout` by default. `constrained_layout` has a similar functionality compared to `tight_layout`, however it is fully deterministic and does not change the size of the underlying figure.
 
 ## References
 
 This package is inspired by the following sources:
 
 - Code: https://pypi.org/project/SciencePlots/
 - Figure sizes: https://jwalton.info/Embed-Publication-Matplotlib-Latex/
 - Color palette (Okabe Ito): https://clauswilke.com/dataviz/color-basics.html
+- Golden ratio: https://en.wikipedia.org/wiki/Golden_ratio
```

#### html2text {}

```diff
@@ -7,77 +7,76 @@
 latexplotlib/actions) [![Coverage Status](https://coveralls.io/repos/github/
 cgahr/latexplotlib/badge.svg?branch=main)](https://coveralls.io/github/cgahr/
 latexplotlib?branch=main) [Code_style:_black] [![Ruff](https://img.shields.io/
 endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/
 badge/v1.json)](https://github.com/charliermarsh/ruff) Perfect matplotlib
 figures for latex. ## Quickstart 1. install `latexplotlib`: ```python pip
 install latexplotlib ``` 2. import latexplotlib and use latexplotlib style
-```python import latexplotlib as lpl plt.style.use('latex10pt') # lpl.style.use
-('latex10pt-minimal') ``` 3. replace all `plt.subplots` with `lpl.subplots`:
-```python # fig, axes = plt.subplots(2, 3) fig, axes = lpl.subplots(2, 3) ```
-Optional: 4. get size of latex document ```latex (\the\textwidth,
-\the\textheight) % (412.123pt, 346.564pt) ``` 5. set `lpl.size` to size of
-latex document ```python lpl.size.set(412.123, 346.564) ``` ## Usage This
-package has two basic functionalities. On the one hand, it sets sensible
-defaults for creating perfect figures for latex. This includes a color scheme
-optimized for color-blind people, correct font and font sizes, and sensible
-defaults to store the figure. On the other hand, it provides some functions to
-create perfectly sized figures. These figures fit your latex document without
-scaling and have the correct font size for your document. ### latexplotlib
-styles There are 6 different styles for matplotlib: - `latex10pt-minimal` -
-`latex11pt-minimal` - `latex12pt-minimal` - `latex10pt` - `latex11pt` -
-`latex12pt` The `*minimal` versions change the font and the font sizes to
-ensure that the figures fonts match the latex font. This style is fully
-compatible with other styles: ```python import matplotlib.pyplot as plt import
-numpy as np import latexplotlib as lpl plt.style.use("latex10pt-minimal") #
-lpl.size.set(200, 400) with lpl.size.context(200, 400): fig, ax = lpl.subplots
-(1, 1) x = np.linspace(1, 5, 100) for t in range(4): label = f"$x^{t}$" ax.plot
-(x, x ** t, label=label) ax.set_yscale("log") ax.set_title("Perfect matplotlib
-figures for \\LaTeX") ax.grid() fig.legend() plt.savefig
-("example_poly_minimal") plt.savefig("example_poly_minimal.png") ```
+```python import latexplotlib as lpl lpl.style.use('latex10pt') # lpl.style.use
+('latex10pt-minimal') ``` 3. replace all usages of `plt` with `lpl`. Only
+`plt.subplots` changes its behavior: ```python # fig, axes = plt.subplots(2, 3)
+fig, axes = lpl.subplots(2, 3) ``` Optional: 4. get size of latex document
+```latex (\the\textwidth, \the\textheight) % (412.123pt, 346.564pt) ``` 5. set
+`lpl.size` to size of latex document ```python lpl.size.set(412.123, 346.564)
+``` ## Usage This package has two basic functionalities. On the one hand, it
+sets sensible defaults for creating perfect figures for latex. This includes a
+color scheme optimized for color-blind people, correct font and font sizes, and
+sensible defaults to store the figure. On the other hand, it provides some
+functions to create perfectly sized figures. These figures fit your latex
+document without scaling and have the correct font size for your document. ###
+latexplotlib styles There are 6 different styles for matplotlib: - `latex10pt-
+minimal` - `latex11pt-minimal` - `latex12pt-minimal` - `latex10pt` -
+`latex11pt` - `latex12pt` The `*minimal` versions change the font and the font
+sizes to ensure that the figures fonts match the latex font. This style is
+fully compatible with other styles: ```python import matplotlib.pyplot as plt
+import numpy as np import latexplotlib as lpl lpl.style.use("latex10pt-
+minimal") # lpl.size.set(200, 400) with lpl.size.context(200, 400): fig, ax =
+lpl.subplots(1, 1) x = np.linspace(1, 5, 100) for t in range(4): label = f"$x^
+{t}$" ax.plot(x, x ** t, label=label) ax.set_yscale("log") ax.set_title
+("Perfect matplotlib figures for \\LaTeX") ax.grid() fig.legend() fig.savefig
+("example_poly_minimal") fig.savefig("example_poly_minimal.png") ```
       [https://github.com/ConstantinGahr/latexplotlib/blob/main/examples/
                       example_poly_minimal.png?raw=true]
 The non-minimal versions set additional defaults to create figures that are
 accessible for color-blind people: ```python import matplotlib.pyplot as plt
-import numpy as np import latexplotlib as lpl plt.style.use("latex10pt") #
-lpl.size.set(200, 400) with lpl.size.context(200, 400): fig, ax = lpl.subplots
-(1, 1) x = np.linspace(1, 5, 100) for t in range(4): label = f"$x^{t}$" ax.plot
-(x, x ** t, label=label) ax.set_yscale("log") ax.set_title("Perfect matplotlib
-figures for \\LaTeX") ax.grid() fig.legend() fig.savefig("example_poly")
-fig.savefig("example_poly.png") ```
+import numpy as np lpl.style.use("latex10pt") # lpl.size.set(200, 400) with
+lpl.size.context(200, 400): fig, ax = lpl.subplots(1, 1) x = np.linspace(1, 5,
+100) for t in range(4): label = f"$x^{t}$" ax.plot(x, x ** t, label=label)
+ax.set_yscale("log") ax.set_title("Perfect matplotlib figures for \\LaTeX")
+ax.grid() fig.legend() fig.savefig("example_poly") fig.savefig
+("example_poly.png") ```
       [https://github.com/ConstantinGahr/latexplotlib/blob/main/examples/
                           example_poly.png?raw=true]
 Both styles change the defaults of the `plt.savefig` command. The new defaults
-are ```python plt.savefig( ..., bbox_inches=None, dpi=300, format="pdf",
+are ```python lpl.savefig( ..., bbox_inches=None, dpi=300, format="pdf",
 orientation="portrait", pad_inches=0.05 ) ``` ### Get latex dimensions You can
 find the width and height of your document using the following command:
 ```latex \the\textwidth \the\textheight ``` ### Set and get latex page size
 ```python import latexplotlib as lpl lpl.size.set(200, 400) with
 lpl.size.context(100, 200): lpl.size() # 100, 200 lpl.size() # (200, 400) ```
-### Create figures for latex ```python import matplotlib.pyplot as plt import
-latexplotlib as lpl # A figure filling 75% of the latex page _ = lpl.subplots
-(1, 1) # A subplot filling 80% of the latex page fig, axes = lpl.subplots(3, 2,
-scale=0.8) # A subplot for 3 square plots next to each other fig, axes =
-lpl.subplots(1, 3, scale=0.8, aspect='equal') ``` ### `aspect` keyword The
-`aspect` keyword controls the ratio of height to width. The default is the
-Golden ratio. `aspect` can also be `equal` (i.e. `aspect=1` )or `auto`. In the
-latter case, the figure fills the available space. ```python import
-matplotlib.pyplot as plt import latexplotlib as lpl # A 3 by 2 figure where
+### Create figures for latex ```python import latexplotlib as lpl # A figure
+filling 75% of the latex page _ = lpl.subplots(1, 1) # A subplot filling 80% of
+the latex page fig, axes = lpl.subplots(3, 2, scale=0.8) # A subplot for 3
+square plots next to each other fig, axes = lpl.subplots(1, 3, scale=0.8,
+aspect='equal') ``` ### `aspect` keyword The `aspect` keyword controls the
+ratio of height to width. The default is the Golden ratio. `aspect` can also be
+`equal` (i.e. `aspect=1` )or `auto`. In the latter case, the figure fills the
+available space. ```python import latexplotlib as lpl # A 3 by 2 figure where
 each subplots height to width ratio is the golden ratio fig, axes =
 lpl.subplots(3, 2) # A 3 by 2 figure where each subplot having a height to
 width ratio of 1:1 fig, axes = lpl.subplots(3, 2, aspect=1.0) # A figure that
 is exactly 300pt height and 200pt wide with lpl.size.context(200, 300): fig,
 axes = lpl.subplots(3, 2, aspect="auto") ``` ### Include figures in Latex The
 most important part of including the figures in latex is to not set the size of
 the figure using arguments like `[width=...]`: ```latex \includegraphics
-[width=\textwidth]{test.pdf} ``` Instead, latexplotlib creates figures that are
-already properly sized. As such, figure can be added using only ```latex
-\includegraphics}{test.pdf} ``` ### `plt.tight_layout()` `plt.tight_layout()`
-changes the size of the produced figure. As such it is recommended to not use
-`plt.tight_layout()` with care! The same is true for `savefig(...,
-bbox_inches=None)`! Instead all latexplotlib styles used `constrained_layout`
-by default. `constrained_layout` has a similar functionality compared to
-`tight_layout`, however it is fully deterministic and does not change the size
-of the underlying figure. ## References This package is inspired by the
-following sources: - Code: https://pypi.org/project/SciencePlots/ - Figure
-sizes: https://jwalton.info/Embed-Publication-Matplotlib-Latex/ - Color palette
-(Okabe Ito): https://clauswilke.com/dataviz/color-basics.html
+{test.pdf} ``` Observe that we did NOT adjust the size using arguments like `
+[width=...]`: ```latex \includegraphics[width=\textwidth]{test.pdf} ``` ###
+`plt.tight_layout()` `plt.tight_layout()` changes the size of the produced
+figure. As such it is recommended to not use `plt.tight_layout()` at all! The
+same is true for `savefig(..., bbox_inches=None)`! Instead all latexplotlib
+styles used `constrained_layout` by default. `constrained_layout` has a similar
+functionality compared to `tight_layout`, however it is fully deterministic and
+does not change the size of the underlying figure. ## References This package
+is inspired by the following sources: - Code: https://pypi.org/project/
+SciencePlots/ - Figure sizes: https://jwalton.info/Embed-Publication-
+Matplotlib-Latex/ - Color palette (Okabe Ito): https://clauswilke.com/dataviz/
+color-basics.html - Golden ratio: https://en.wikipedia.org/wiki/Golden_ratio
```

### Comparing `latexplotlib-0.6.1/pyproject.toml` & `latexplotlib-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     "coverage",
     "pytest",
     "pytest-cov",
     "pytest-mock"
 ]
 
 [project.urls]
+Changelog = "https://github.com/cgahr/latexplotlib/blob/main/CHANGES.md"
 Homepage = "https://github.com/cgahr/latexplotlib"
 Issues = "https://github.com/cgahr/latexplotlib/issues"
 
 [tool.black]
 line_length = 88
 
 [tool.coverage.report]
```

### Comparing `latexplotlib-0.6.1/src/latexplotlib/_cleanup.py` & `latexplotlib-0.7.0/src/latexplotlib/_cleanup.py`

 * *Files identical despite different names*

### Comparing `latexplotlib-0.6.1/src/latexplotlib/_config.py` & `latexplotlib-0.7.0/src/latexplotlib/_config.py`

 * *Files identical despite different names*

### Comparing `latexplotlib-0.6.1/src/latexplotlib/_latexplotlib.py` & `latexplotlib-0.7.0/src/latexplotlib/_latexplotlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     References
     ----------
     - https://www.overleaf.com/learn/latex/Lengths_in_LaTeX
     """
     return inches * 864.0 * 250.0 / 249.0 / 12.0
 
 
-def figsize(
+def figsize(  # noqa: PLR0913
     nrows: int = 1,
     ncols: int = 1,
     *,
     scale: float = 1.0,
     aspect: Aspect = GOLDEN_RATIO,
     height_ratios: Optional[Sequence[float]] = None,
     width_ratios: Optional[Sequence[float]] = None,
```

### Comparing `latexplotlib-0.6.1/src/latexplotlib/styles/latex10pt.mplstyle` & `latexplotlib-0.7.0/src/latexplotlib/styles/latex10pt.mplstyle`

 * *Files identical despite different names*

### Comparing `latexplotlib-0.6.1/src/latexplotlib/styles/latex11pt.mplstyle` & `latexplotlib-0.7.0/src/latexplotlib/styles/latex11pt.mplstyle`

 * *Files identical despite different names*

### Comparing `latexplotlib-0.6.1/src/latexplotlib/styles/latex12pt.mplstyle` & `latexplotlib-0.7.0/src/latexplotlib/styles/latex12pt.mplstyle`

 * *Files identical despite different names*

### Comparing `latexplotlib-0.6.1/src/latexplotlib/styles/latex9pt.mplstyle` & `latexplotlib-0.7.0/src/latexplotlib/styles/latex9pt.mplstyle`

 * *Files identical despite different names*

### Comparing `latexplotlib-0.6.1/src/latexplotlib.egg-info/PKG-INFO` & `latexplotlib-0.7.0/src/latexplotlib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: latexplotlib
-Version: 0.6.1
+Version: 0.7.0
 Summary: Perfect matplotlib figures for latex
 Author-email: Constantin Gahr <latexplotlib.gvxel@aleeas.com>
 License: MIT
+Project-URL: Changelog, https://github.com/cgahr/latexplotlib/blob/main/CHANGES.md
 Project-URL: Homepage, https://github.com/cgahr/latexplotlib
 Project-URL: Issues, https://github.com/cgahr/latexplotlib/issues
 Keywords: latex,matplotlib-figures,matplotlib-style-sheets,matplotlib-styles,python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -38,19 +39,19 @@
 ```python
 pip install latexplotlib
 ```
 2. import latexplotlib and use latexplotlib style
 ```python
 import latexplotlib as lpl
 
-plt.style.use('latex10pt')
+lpl.style.use('latex10pt')
 # lpl.style.use('latex10pt-minimal')
 ```
 
-3. replace all `plt.subplots` with `lpl.subplots`:
+3. replace all usages of `plt` with `lpl`. Only `plt.subplots` changes its behavior:
 ```python
 #  fig, axes = plt.subplots(2, 3)
 fig, axes = lpl.subplots(2, 3)
 ```
 
 Optional:
 
@@ -87,15 +88,15 @@
 
 ```python
 import matplotlib.pyplot as plt
 import numpy as np
 
 import latexplotlib as lpl
 
-plt.style.use("latex10pt-minimal")
+lpl.style.use("latex10pt-minimal")
 # lpl.size.set(200, 400)
 with lpl.size.context(200, 400):
     fig, ax = lpl.subplots(1, 1)
 
 x = np.linspace(1, 5, 100)
 
 for t in range(4):
@@ -103,32 +104,31 @@
     ax.plot(x, x ** t, label=label)
 
 ax.set_yscale("log")
 ax.set_title("Perfect matplotlib figures for \\LaTeX")
 ax.grid()
 
 fig.legend()
-plt.savefig("example_poly_minimal")
-plt.savefig("example_poly_minimal.png")
+fig.savefig("example_poly_minimal")
+fig.savefig("example_poly_minimal.png")
 ```
 
 <p align="center">
 <img src="https://github.com/ConstantinGahr/latexplotlib/blob/main/examples/example_poly_minimal.png?raw=true" width="500">
 </p>
 
 
 The non-minimal versions set additional defaults to create figures that are accessible for color-blind people:
 
 ```python
 import matplotlib.pyplot as plt
 import numpy as np
-import latexplotlib as lpl
 
 
-plt.style.use("latex10pt")
+lpl.style.use("latex10pt")
 
 # lpl.size.set(200, 400)
 with lpl.size.context(200, 400):
     fig, ax = lpl.subplots(1, 1)
 
 x = np.linspace(1, 5, 100)
 
@@ -147,15 +147,15 @@
 <p align="center">
 <img src="https://github.com/ConstantinGahr/latexplotlib/blob/main/examples/example_poly.png?raw=true" width="500">
 </p>
 
 Both styles change the defaults of the `plt.savefig` command. The new defaults are
 
 ```python
-plt.savefig(
+lpl.savefig(
     ...,
     bbox_inches=None,
     dpi=300,
     format="pdf",
     orientation="portrait",
     pad_inches=0.05
 )
@@ -181,16 +181,14 @@
     lpl.size()  # 100, 200
 
 lpl.size()  # (200, 400)
 ```
 
 ### Create figures for latex
 ```python
-import matplotlib.pyplot as plt
-
 import latexplotlib as lpl
 
 
 # A figure filling 75% of the latex page
 _ = lpl.subplots(1, 1)
 
 # A subplot filling 80% of the latex page
@@ -200,16 +198,14 @@
 fig, axes = lpl.subplots(1, 3, scale=0.8, aspect='equal')
 ```
 
 ### `aspect` keyword
 The `aspect` keyword controls the ratio of height to width. The default is the Golden ratio. `aspect` can also be `equal` (i.e. `aspect=1` )or `auto`. In the latter case, the figure fills the available space.
 
 ```python
-import matplotlib.pyplot as plt
-
 import latexplotlib as lpl
 
 # A 3 by 2 figure where each subplots height to width ratio is the golden ratio
 fig, axes = lpl.subplots(3, 2)
 
 # A 3 by 2 figure where each subplot having a height to width ratio of 1:1
 fig, axes = lpl.subplots(3, 2, aspect=1.0)
@@ -220,28 +216,28 @@
 ```
 
 
 ### Include figures in Latex
 
 The most important part of including the figures in latex is to not set the size of the figure using arguments like `[width=...]`:
 ```latex
-\includegraphics[width=\textwidth]{test.pdf}
+\includegraphics{test.pdf}
 ```
-
-Instead, latexplotlib creates figures that are already properly sized. As such, figure can be added using only
+Observe that we did NOT adjust the size using arguments like `[width=...]`:
 ```latex
-\includegraphics}{test.pdf}
+\includegraphics[width=\textwidth]{test.pdf}
 ```
 
 ### `plt.tight_layout()`
 
-`plt.tight_layout()` changes the size of the produced figure. As such it is recommended to not use `plt.tight_layout()` with care! The same is true for `savefig(..., bbox_inches=None)`!
+`plt.tight_layout()` changes the size of the produced figure. As such it is recommended to not use `plt.tight_layout()` at all! The same is true for `savefig(..., bbox_inches=None)`!
 
 Instead all latexplotlib styles used `constrained_layout` by default. `constrained_layout` has a similar functionality compared to `tight_layout`, however it is fully deterministic and does not change the size of the underlying figure.
 
 ## References
 
 This package is inspired by the following sources:
 
 - Code: https://pypi.org/project/SciencePlots/
 - Figure sizes: https://jwalton.info/Embed-Publication-Matplotlib-Latex/
 - Color palette (Okabe Ito): https://clauswilke.com/dataviz/color-basics.html
+- Golden ratio: https://en.wikipedia.org/wiki/Golden_ratio
```

#### html2text {}

```diff
@@ -1,95 +1,95 @@
-Metadata-Version: 2.1 Name: latexplotlib Version: 0.6.1 Summary: Perfect
+Metadata-Version: 2.1 Name: latexplotlib Version: 0.7.0 Summary: Perfect
 matplotlib figures for latex Author-email: Constantin Gahr
-gvxel@aleeas.com> License: MIT Project-URL: Homepage, https://github.com/cgahr/
-latexplotlib Project-URL: Issues, https://github.com/cgahr/latexplotlib/issues
-Keywords: latex,matplotlib-figures,matplotlib-style-sheets,matplotlib-
-styles,python Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: License :: OSI Approved ::
-MIT License Classifier: Operating System :: OS Independent Requires-Python:
->=3.7.1 Description-Content-Type: text/markdown Provides-Extra: tests License-
-File: LICENSE # latexplotlib [![image](https://img.shields.io/pypi/v/
-latexplotlib.svg)](https://pypi.python.org/pypi/latexplotlib) [![image](https:/
-/img.shields.io/pypi/l/latexplotlib.svg)](https://pypi.python.org/pypi/
-latexplotlib) [![image](https://img.shields.io/pypi/pyversions/
-latexplotlib.svg)](https://pypi.python.org/pypi/latexplotlib) [![Actions
-status](https://github.com/cgahr/latexplotlib/actions/workflows/main.yml/
-badge.svg)](https://github.com/cgahr/latexplotlib/actions) [![Coverage Status]
-(https://coveralls.io/repos/github/cgahr/latexplotlib/badge.svg?branch=main)]
-(https://coveralls.io/github/cgahr/latexplotlib?branch=main) [Code_style:
-black] [![Ruff](https://img.shields.io/endpoint?url=https://
-raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https:
-//github.com/charliermarsh/ruff) Perfect matplotlib figures for latex. ##
-Quickstart 1. install `latexplotlib`: ```python pip install latexplotlib ``` 2.
-import latexplotlib and use latexplotlib style ```python import latexplotlib as
-lpl plt.style.use('latex10pt') # lpl.style.use('latex10pt-minimal') ``` 3.
-replace all `plt.subplots` with `lpl.subplots`: ```python # fig, axes =
-plt.subplots(2, 3) fig, axes = lpl.subplots(2, 3) ``` Optional: 4. get size of
-latex document ```latex (\the\textwidth, \the\textheight) % (412.123pt,
-346.564pt) ``` 5. set `lpl.size` to size of latex document ```python
-lpl.size.set(412.123, 346.564) ``` ## Usage This package has two basic
-functionalities. On the one hand, it sets sensible defaults for creating
-perfect figures for latex. This includes a color scheme optimized for color-
-blind people, correct font and font sizes, and sensible defaults to store the
-figure. On the other hand, it provides some functions to create perfectly sized
-figures. These figures fit your latex document without scaling and have the
-correct font size for your document. ### latexplotlib styles There are 6
-different styles for matplotlib: - `latex10pt-minimal` - `latex11pt-minimal` -
-`latex12pt-minimal` - `latex10pt` - `latex11pt` - `latex12pt` The `*minimal`
-versions change the font and the font sizes to ensure that the figures fonts
-match the latex font. This style is fully compatible with other styles:
-```python import matplotlib.pyplot as plt import numpy as np import
-latexplotlib as lpl plt.style.use("latex10pt-minimal") # lpl.size.set(200, 400)
-with lpl.size.context(200, 400): fig, ax = lpl.subplots(1, 1) x = np.linspace
-(1, 5, 100) for t in range(4): label = f"$x^{t}$" ax.plot(x, x ** t,
-label=label) ax.set_yscale("log") ax.set_title("Perfect matplotlib figures for
-\\LaTeX") ax.grid() fig.legend() plt.savefig("example_poly_minimal")
-plt.savefig("example_poly_minimal.png") ```
+gvxel@aleeas.com> License: MIT Project-URL: Changelog, https://github.com/
+cgahr/latexplotlib/blob/main/CHANGES.md Project-URL: Homepage, https://
+github.com/cgahr/latexplotlib Project-URL: Issues, https://github.com/cgahr/
+latexplotlib/issues Keywords: latex,matplotlib-figures,matplotlib-style-
+sheets,matplotlib-styles,python Classifier: Programming Language :: Python ::
+3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7.1 Description-Content-Type: text/markdown Provides-
+Extra: tests License-File: LICENSE # latexplotlib [![image](https://
+img.shields.io/pypi/v/latexplotlib.svg)](https://pypi.python.org/pypi/
+latexplotlib) [![image](https://img.shields.io/pypi/l/latexplotlib.svg)](https:
+//pypi.python.org/pypi/latexplotlib) [![image](https://img.shields.io/pypi/
+pyversions/latexplotlib.svg)](https://pypi.python.org/pypi/latexplotlib) [!
+[Actions status](https://github.com/cgahr/latexplotlib/actions/workflows/
+main.yml/badge.svg)](https://github.com/cgahr/latexplotlib/actions) [![Coverage
+Status](https://coveralls.io/repos/github/cgahr/latexplotlib/
+badge.svg?branch=main)](https://coveralls.io/github/cgahr/
+latexplotlib?branch=main) [Code_style:_black] [![Ruff](https://img.shields.io/
+endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/
+badge/v1.json)](https://github.com/charliermarsh/ruff) Perfect matplotlib
+figures for latex. ## Quickstart 1. install `latexplotlib`: ```python pip
+install latexplotlib ``` 2. import latexplotlib and use latexplotlib style
+```python import latexplotlib as lpl lpl.style.use('latex10pt') # lpl.style.use
+('latex10pt-minimal') ``` 3. replace all usages of `plt` with `lpl`. Only
+`plt.subplots` changes its behavior: ```python # fig, axes = plt.subplots(2, 3)
+fig, axes = lpl.subplots(2, 3) ``` Optional: 4. get size of latex document
+```latex (\the\textwidth, \the\textheight) % (412.123pt, 346.564pt) ``` 5. set
+`lpl.size` to size of latex document ```python lpl.size.set(412.123, 346.564)
+``` ## Usage This package has two basic functionalities. On the one hand, it
+sets sensible defaults for creating perfect figures for latex. This includes a
+color scheme optimized for color-blind people, correct font and font sizes, and
+sensible defaults to store the figure. On the other hand, it provides some
+functions to create perfectly sized figures. These figures fit your latex
+document without scaling and have the correct font size for your document. ###
+latexplotlib styles There are 6 different styles for matplotlib: - `latex10pt-
+minimal` - `latex11pt-minimal` - `latex12pt-minimal` - `latex10pt` -
+`latex11pt` - `latex12pt` The `*minimal` versions change the font and the font
+sizes to ensure that the figures fonts match the latex font. This style is
+fully compatible with other styles: ```python import matplotlib.pyplot as plt
+import numpy as np import latexplotlib as lpl lpl.style.use("latex10pt-
+minimal") # lpl.size.set(200, 400) with lpl.size.context(200, 400): fig, ax =
+lpl.subplots(1, 1) x = np.linspace(1, 5, 100) for t in range(4): label = f"$x^
+{t}$" ax.plot(x, x ** t, label=label) ax.set_yscale("log") ax.set_title
+("Perfect matplotlib figures for \\LaTeX") ax.grid() fig.legend() fig.savefig
+("example_poly_minimal") fig.savefig("example_poly_minimal.png") ```
       [https://github.com/ConstantinGahr/latexplotlib/blob/main/examples/
                       example_poly_minimal.png?raw=true]
 The non-minimal versions set additional defaults to create figures that are
 accessible for color-blind people: ```python import matplotlib.pyplot as plt
-import numpy as np import latexplotlib as lpl plt.style.use("latex10pt") #
-lpl.size.set(200, 400) with lpl.size.context(200, 400): fig, ax = lpl.subplots
-(1, 1) x = np.linspace(1, 5, 100) for t in range(4): label = f"$x^{t}$" ax.plot
-(x, x ** t, label=label) ax.set_yscale("log") ax.set_title("Perfect matplotlib
-figures for \\LaTeX") ax.grid() fig.legend() fig.savefig("example_poly")
-fig.savefig("example_poly.png") ```
+import numpy as np lpl.style.use("latex10pt") # lpl.size.set(200, 400) with
+lpl.size.context(200, 400): fig, ax = lpl.subplots(1, 1) x = np.linspace(1, 5,
+100) for t in range(4): label = f"$x^{t}$" ax.plot(x, x ** t, label=label)
+ax.set_yscale("log") ax.set_title("Perfect matplotlib figures for \\LaTeX")
+ax.grid() fig.legend() fig.savefig("example_poly") fig.savefig
+("example_poly.png") ```
       [https://github.com/ConstantinGahr/latexplotlib/blob/main/examples/
                           example_poly.png?raw=true]
 Both styles change the defaults of the `plt.savefig` command. The new defaults
-are ```python plt.savefig( ..., bbox_inches=None, dpi=300, format="pdf",
+are ```python lpl.savefig( ..., bbox_inches=None, dpi=300, format="pdf",
 orientation="portrait", pad_inches=0.05 ) ``` ### Get latex dimensions You can
 find the width and height of your document using the following command:
 ```latex \the\textwidth \the\textheight ``` ### Set and get latex page size
 ```python import latexplotlib as lpl lpl.size.set(200, 400) with
 lpl.size.context(100, 200): lpl.size() # 100, 200 lpl.size() # (200, 400) ```
-### Create figures for latex ```python import matplotlib.pyplot as plt import
-latexplotlib as lpl # A figure filling 75% of the latex page _ = lpl.subplots
-(1, 1) # A subplot filling 80% of the latex page fig, axes = lpl.subplots(3, 2,
-scale=0.8) # A subplot for 3 square plots next to each other fig, axes =
-lpl.subplots(1, 3, scale=0.8, aspect='equal') ``` ### `aspect` keyword The
-`aspect` keyword controls the ratio of height to width. The default is the
-Golden ratio. `aspect` can also be `equal` (i.e. `aspect=1` )or `auto`. In the
-latter case, the figure fills the available space. ```python import
-matplotlib.pyplot as plt import latexplotlib as lpl # A 3 by 2 figure where
+### Create figures for latex ```python import latexplotlib as lpl # A figure
+filling 75% of the latex page _ = lpl.subplots(1, 1) # A subplot filling 80% of
+the latex page fig, axes = lpl.subplots(3, 2, scale=0.8) # A subplot for 3
+square plots next to each other fig, axes = lpl.subplots(1, 3, scale=0.8,
+aspect='equal') ``` ### `aspect` keyword The `aspect` keyword controls the
+ratio of height to width. The default is the Golden ratio. `aspect` can also be
+`equal` (i.e. `aspect=1` )or `auto`. In the latter case, the figure fills the
+available space. ```python import latexplotlib as lpl # A 3 by 2 figure where
 each subplots height to width ratio is the golden ratio fig, axes =
 lpl.subplots(3, 2) # A 3 by 2 figure where each subplot having a height to
 width ratio of 1:1 fig, axes = lpl.subplots(3, 2, aspect=1.0) # A figure that
 is exactly 300pt height and 200pt wide with lpl.size.context(200, 300): fig,
 axes = lpl.subplots(3, 2, aspect="auto") ``` ### Include figures in Latex The
 most important part of including the figures in latex is to not set the size of
 the figure using arguments like `[width=...]`: ```latex \includegraphics
-[width=\textwidth]{test.pdf} ``` Instead, latexplotlib creates figures that are
-already properly sized. As such, figure can be added using only ```latex
-\includegraphics}{test.pdf} ``` ### `plt.tight_layout()` `plt.tight_layout()`
-changes the size of the produced figure. As such it is recommended to not use
-`plt.tight_layout()` with care! The same is true for `savefig(...,
-bbox_inches=None)`! Instead all latexplotlib styles used `constrained_layout`
-by default. `constrained_layout` has a similar functionality compared to
-`tight_layout`, however it is fully deterministic and does not change the size
-of the underlying figure. ## References This package is inspired by the
-following sources: - Code: https://pypi.org/project/SciencePlots/ - Figure
-sizes: https://jwalton.info/Embed-Publication-Matplotlib-Latex/ - Color palette
-(Okabe Ito): https://clauswilke.com/dataviz/color-basics.html
+{test.pdf} ``` Observe that we did NOT adjust the size using arguments like `
+[width=...]`: ```latex \includegraphics[width=\textwidth]{test.pdf} ``` ###
+`plt.tight_layout()` `plt.tight_layout()` changes the size of the produced
+figure. As such it is recommended to not use `plt.tight_layout()` at all! The
+same is true for `savefig(..., bbox_inches=None)`! Instead all latexplotlib
+styles used `constrained_layout` by default. `constrained_layout` has a similar
+functionality compared to `tight_layout`, however it is fully deterministic and
+does not change the size of the underlying figure. ## References This package
+is inspired by the following sources: - Code: https://pypi.org/project/
+SciencePlots/ - Figure sizes: https://jwalton.info/Embed-Publication-
+Matplotlib-Latex/ - Color palette (Okabe Ito): https://clauswilke.com/dataviz/
+color-basics.html - Golden ratio: https://en.wikipedia.org/wiki/Golden_ratio
```

### Comparing `latexplotlib-0.6.1/src/latexplotlib.egg-info/SOURCES.txt` & `latexplotlib-0.7.0/src/latexplotlib.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -21,8 +21,9 @@
 src/latexplotlib/styles/latex12pt.mplstyle
 src/latexplotlib/styles/latex9pt-minimal.mplstyle
 src/latexplotlib/styles/latex9pt.mplstyle
 tests/test_00_styles.py
 tests/test_10_config.py
 tests/test_20_cleanup.py
 tests/test_30_latexplotlib.py
+tests/test_plt_available.py
 tests/test_styles_available.py
```

### Comparing `latexplotlib-0.6.1/tests/test_00_styles.py` & `latexplotlib-0.7.0/tests/test_00_styles.py`

 * *Files identical despite different names*

### Comparing `latexplotlib-0.6.1/tests/test_10_config.py` & `latexplotlib-0.7.0/tests/test_10_config.py`

 * *Files identical despite different names*

### Comparing `latexplotlib-0.6.1/tests/test_20_cleanup.py` & `latexplotlib-0.7.0/tests/test_20_cleanup.py`

 * *Files identical despite different names*

### Comparing `latexplotlib-0.6.1/tests/test_30_latexplotlib.py` & `latexplotlib-0.7.0/tests/test_30_latexplotlib.py`

 * *Files identical despite different names*

