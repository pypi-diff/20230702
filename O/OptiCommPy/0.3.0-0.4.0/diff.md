# Comparing `tmp/OptiCommPy-0.3.0.tar.gz` & `tmp/OptiCommPy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OptiCommPy-0.3.0.tar", last modified: Thu Mar 16 01:38:53 2023, max compression
+gzip compressed data, was "OptiCommPy-0.4.0.tar", last modified: Sun Jul  2 19:40:57 2023, max compression
```

## Comparing `OptiCommPy-0.3.0.tar` & `OptiCommPy-0.4.0.tar`

### file list

```diff
@@ -1,29 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-16 01:38:53.934403 OptiCommPy-0.3.0/
--rw-rw-rw-   0        0        0    35823 2023-03-16 01:35:04.000000 OptiCommPy-0.3.0/LICENSE
-drwxrwxrwx   0        0        0        0 2023-03-16 01:38:53.914395 OptiCommPy-0.3.0/OptiCommPy.egg-info/
--rw-rw-rw-   0        0        0     3869 2023-03-16 01:38:53.000000 OptiCommPy-0.3.0/OptiCommPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      458 2023-03-16 01:38:53.000000 OptiCommPy-0.3.0/OptiCommPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-16 01:38:53.000000 OptiCommPy-0.3.0/OptiCommPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2023-03-16 01:38:53.000000 OptiCommPy-0.3.0/OptiCommPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-03-16 01:38:53.000000 OptiCommPy-0.3.0/OptiCommPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3869 2023-03-16 01:38:53.933401 OptiCommPy-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3182 2023-03-16 01:35:04.000000 OptiCommPy-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-16 01:38:53.932401 OptiCommPy-0.3.0/optic/
--rw-rw-rw-   0        0        0       14 2023-03-16 01:35:04.000000 OptiCommPy-0.3.0/optic/__init__.py
--rw-rw-rw-   0        0        0    24484 2023-03-16 01:35:04.000000 OptiCommPy-0.3.0/optic/amplification.py
--rw-rw-rw-   0        0        0     7815 2023-03-16 01:35:04.000000 OptiCommPy-0.3.0/optic/carrierRecovery.py
--rw-rw-rw-   0        0        0      105 2023-03-16 01:35:04.000000 OptiCommPy-0.3.0/optic/core.py
--rw-rw-rw-   0        0        0     8160 2023-03-16 01:35:04.000000 OptiCommPy-0.3.0/optic/dsp.py
--rw-rw-rw-   0        0        0      892 2023-03-16 01:35:04.000000 OptiCommPy-0.3.0/optic/dspGPU.py
--rw-rw-rw-   0        0        0    17446 2023-03-16 01:35:04.000000 OptiCommPy-0.3.0/optic/equalization.py
--rw-rw-rw-   0        0        0     1644 2023-03-16 01:35:04.000000 OptiCommPy-0.3.0/optic/fec.py
--rw-rw-rw-   0        0        0    18045 2023-03-16 01:35:05.000000 OptiCommPy-0.3.0/optic/metrics.py
--rw-rw-rw-   0        0        0    20396 2023-03-16 01:35:05.000000 OptiCommPy-0.3.0/optic/models.py
--rw-rw-rw-   0        0        0    13547 2023-03-16 01:35:05.000000 OptiCommPy-0.3.0/optic/modelsGPU.py
--rw-rw-rw-   0        0        0     5687 2023-03-16 01:35:05.000000 OptiCommPy-0.3.0/optic/modulation.py
--rw-rw-rw-   0        0        0     5703 2023-03-16 01:35:05.000000 OptiCommPy-0.3.0/optic/ofdm.py
--rw-rw-rw-   0        0        0     8324 2023-03-16 01:35:05.000000 OptiCommPy-0.3.0/optic/plot.py
--rw-rw-rw-   0        0        0     5650 2023-03-16 01:35:05.000000 OptiCommPy-0.3.0/optic/tx.py
--rw-rw-rw-   0        0        0      307 2023-03-16 01:35:05.000000 OptiCommPy-0.3.0/runner
--rw-rw-rw-   0        0        0       42 2023-03-16 01:38:53.934403 OptiCommPy-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     2106 2023-03-16 01:37:20.000000 OptiCommPy-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 19:40:57.100672 OptiCommPy-0.4.0/
+-rw-rw-rw-   0        0        0    35823 2022-08-27 14:09:58.000000 OptiCommPy-0.4.0/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-02 19:40:57.094671 OptiCommPy-0.4.0/OptiCommPy.egg-info/
+-rw-rw-rw-   0        0        0     3869 2023-07-02 19:40:56.000000 OptiCommPy-0.4.0/OptiCommPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-07-02 19:40:56.000000 OptiCommPy-0.4.0/OptiCommPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 19:40:56.000000 OptiCommPy-0.4.0/OptiCommPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      158 2023-07-02 19:40:56.000000 OptiCommPy-0.4.0/OptiCommPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-02 19:40:56.000000 OptiCommPy-0.4.0/OptiCommPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3869 2023-07-02 19:40:57.099670 OptiCommPy-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3182 2023-04-06 02:54:53.000000 OptiCommPy-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 19:40:57.098668 OptiCommPy-0.4.0/optic/
+-rw-rw-rw-   0        0        0       14 2022-08-27 14:09:58.000000 OptiCommPy-0.4.0/optic/__init__.py
+-rw-rw-rw-   0        0        0      105 2022-08-27 14:09:58.000000 OptiCommPy-0.4.0/optic/core.py
+-rw-rw-rw-   0        0        0     9450 2023-07-02 19:21:41.000000 OptiCommPy-0.4.0/optic/plot.py
+-rw-rw-rw-   0        0        0      307 2022-08-27 14:09:58.000000 OptiCommPy-0.4.0/runner
+-rw-rw-rw-   0        0        0       42 2023-07-02 19:40:57.100672 OptiCommPy-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     2123 2023-07-02 19:34:49.000000 OptiCommPy-0.4.0/setup.py
```

### Comparing `OptiCommPy-0.3.0/LICENSE` & `OptiCommPy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `OptiCommPy-0.3.0/OptiCommPy.egg-info/PKG-INFO` & `OptiCommPy-0.4.0/OptiCommPy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OptiCommPy
-Version: 0.3.0
+Version: 0.4.0
 Summary: Optical Communications Algorithms with Python
 Home-page: https://github.com/edsonportosilva/OptiCommPy
 Maintainer: Edson Porto da Silva
 Maintainer-email: edsonporto88@gmail.com
 License: BSD 3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `OptiCommPy-0.3.0/PKG-INFO` & `OptiCommPy-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OptiCommPy
-Version: 0.3.0
+Version: 0.4.0
 Summary: Optical Communications Algorithms with Python
 Home-page: https://github.com/edsonportosilva/OptiCommPy
 Maintainer: Edson Porto da Silva
 Maintainer-email: edsonporto88@gmail.com
 License: BSD 3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `OptiCommPy-0.3.0/README.md` & `OptiCommPy-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `OptiCommPy-0.3.0/optic/plot.py` & `OptiCommPy-0.4.0/optic/plot.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,26 +3,56 @@
 from matplotlib import cm
 import mpl_scatter_density
 import numpy as np
 import copy
 from scipy.interpolate import interp1d
 from scipy.ndimage.filters import gaussian_filter
 
-from optic.dsp import pnorm
-from optic.metrics import signal_power
+from optic.dsp.core import pnorm, signal_power
 import warnings
 
 warnings.filterwarnings('ignore', r'All-NaN (slice|axis) encountered')
 
 def pconst(x, lim=True, R=1.25, pType="fancy", cmap="turbo", whiteb=True):
     """
     Plot signal constellations.
-
-    :param x: complex signals or list of complex signals
-
+    
+    Parameters
+    ----------
+    x : complex signals or list of complex signals
+        Input signals.
+    
+    lim : bool, optional
+        Flag indicating whether to limit the axes to the radius of the signal. 
+        Defaults to True.
+    
+    R : float, optional
+        Scaling factor for the radius of the signal. 
+        Defaults to 1.25.
+    
+    pType : str, optional
+        Type of plot. "fancy" for scatter_density plot, "fast" for fast plot.
+        Defaults to "fancy".
+    
+    cmap : str, optional
+        Color map for scatter_density plot.
+        Defaults to "turbo".
+    
+    whiteb : bool, optional
+        Flag indicating whether to use white background for scatter_density plot.
+        Defaults to True.
+    
+    Returns
+    -------
+    fig : Figure
+        Figure object.
+    
+    ax : Axes or array of Axes
+        Axes object(s).
+    
     """
     if type(x) == list:
         for ind, _ in enumerate(x):
             x[ind] = pnorm(x[ind])
         try:
             x[0].shape[1]
         except IndexError:
@@ -148,22 +178,38 @@
     return ax
 
 
 def eyediagram(sigIn, Nsamples, SpS, n=3, ptype="fast", plotlabel=None):
     """
     Plot the eye diagram of a modulated signal waveform.
 
-    :param Nsamples: number os samples to be plotted
-    :param SpS: samples per symbol
-    :param n: number of symbol periods
-    :param type: 'fast' or 'fancy'
-    :param plotlabel: label for the plot legend
+    Parameters
+    ----------
+    sigIn : array-like
+        Input signal waveform.
+    Nsamples : int
+        Number of samples to be plotted.
+    SpS : int
+        Samples per symbol.
+    n : int, optional
+        Number of symbol periods. Defaults to 3.
+    ptype : str, optional
+        Type of eye diagram. Can be 'fast' or 'fancy'. Defaults to 'fast'.
+    plotlabel : str, optional
+        Label for the plot legend. Defaults to None.
+
+    Returns
+    -------
+    None
     """
     sig = sigIn.copy()
 
+    if not plotlabel:
+        plotlabel = " "
+
     if np.iscomplex(sig).any():
         d = 1
         plotlabel_ = f"{plotlabel} [real]" if plotlabel else "[real]"
     else:
         d = 0
         plotlabel_ = plotlabel
 
@@ -175,62 +221,61 @@
             y = sig[:Nsamples].imag
 
             plotlabel_ = f"{plotlabel} [imag]" if plotlabel else "[imag]"
         plt.figure()
         if ptype == "fancy":
             f = interp1d(np.arange(y.size), y, kind="cubic")
 
-            Nup = 20 * SpS
+            Nup = 40 * SpS
             tnew = np.arange(y.size) * (1 / Nup)
             y_ = f(tnew)
 
             taxis = (np.arange(y.size) % (n * SpS * Nup)) * (1 / Nup)
             imRange = np.array(
                 [
                     [min(taxis), max(taxis)],
-                    [min(y) - 0.1 * np.mean(y), 1.1 * max(y)],
+                    [min(y) - 0.1 * np.mean(np.abs(y)), 1.1 * max(y)],
                 ]
             )
 
             H, xedges, yedges = np.histogram2d(
                 taxis, y_, bins=350, range=imRange
             )
 
             H = H.T
-            H = gaussian_filter(H, sigma=0.9)
+            H = gaussian_filter(H, sigma=1.0)
 
-            # plt.figure(figsize=(10, 3))
             plt.imshow(
                 H,
                 cmap="turbo",
                 origin="lower",
                 aspect="auto",
                 extent=[0, n, yedges[0], yedges[-1]],
             )
-            plt.xlabel("symbol period (Ts)")
-            plt.ylabel("amplitude")
+
         elif ptype == "fast":
             y[x == n * SpS] = np.nan
             y[x == 0] = np.nan
 
             plt.plot(x / SpS, y, color="blue", alpha=0.8, label=plotlabel_)
-            plt.xlim(min(x / SpS), max(x / SpS))
-            plt.xlabel("symbol period (Ts)")
-            plt.ylabel("amplitude")
-            plt.title("eye diagram")
+            plt.xlim(min(x / SpS), max(x / SpS)) 
 
             if plotlabel is not None:
                 plt.legend(loc="upper left")
 
-            plt.grid()
-            plt.show()
+        plt.xlabel("symbol period (Ts)")
+        plt.ylabel("amplitude")
+        plt.title(f"eye diagram {plotlabel_}")        
+        plt.grid(alpha=0.15)
+        plt.show()
+
     return None
 
 
-def plotPSD(sig, Fs=1, Fc=0, NFFT=4096, fig=[], label=[]):
+def plotPSD(sig, Fs=1, Fc=0, NFFT=4096, fig=None, label=None):
     """
     Plot the power spectrum density (PSD) of a signal.
 
     Parameters
     ----------
     sig : np.array
         input signal.
@@ -249,31 +294,35 @@
     -------
     fig : matplotlib figure object
         matplotlib figure object where the plot is generated.
     matplotlib axes object
         matplotlib axes object where the plot is displayed.
 
     """
+    if fig is None:
+        fig = []
+    if label is None:
+        label = []
     if not fig:
         fig = plt.figure()
 
     if not label:
         label = " "
 
     try:
        sig.shape[1]       
     except IndexError:
        sig = sig.reshape(len(sig), 1)
-       
+
     for indMode in range(sig.shape[1]):
         plt.psd(
             sig[:, indMode],
             Fs=Fs,
             Fc=Fc,
             NFFT=NFFT,
             sides="twosided",
-            label=label + ": Mode " + str(indMode),
+            label=f"{label}: Mode {str(indMode)}",
         )
     plt.legend(loc="lower left")
     plt.xlim(Fc - Fs / 2, Fc + Fs / 2)
 
     return fig, plt.gca()
```

### Comparing `OptiCommPy-0.3.0/setup.py` & `OptiCommPy-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 DISTNAME = 'OptiCommPy'
 DESCRIPTION = 'Optical Communications Algorithms with Python'
 LONG_DESCRIPTION = open('README.md', encoding="utf8").read()
 MAINTAINER = 'Edson Porto da Silva'
 MAINTAINER_EMAIL = 'edsonporto88@gmail.com'
 URL = 'https://github.com/edsonportosilva/OptiCommPy'
 LICENSE = 'BSD 3-Clause'
-VERSION = '0.3.0'
+VERSION = '0.4.0'
 
 #This is a list of files to install, and where
 #(relative to the 'root' dir, where setup.py is)
 #You could be more specific.
 files = ["optic/*"]
 
 setup(
@@ -35,16 +35,17 @@
           'numpy>=1.9.2',
           'scipy>=0.15.0',
           'matplotlib>=3.7.0',
           'sympy',
           'tqdm>=4.64.1',
           'numba>=0.54.1',
           'scikit-commpy>=0.7.0',
-	    'simple-pid>=1.0.1',
-	    'mpl-scatter-density>=0.7.0'
+	  'simple-pid>=1.0.1',
+	  'mpl-scatter-density>=0.7.0',
+	  'pandas>=2.0.0'
     ],
     #'package' package must contain files (see list above)
     #This dict maps the package name =to=> directories
     #It says, package *needs* these files.
     package_data={'optic': files},
     #'runner' is in the root.
     scripts=["runner"],
```

