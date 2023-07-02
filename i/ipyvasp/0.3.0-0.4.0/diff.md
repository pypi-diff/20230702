# Comparing `tmp/ipyvasp-0.3.0.tar.gz` & `tmp/ipyvasp-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyvasp-0.3.0.tar", last modified: Tue Jun 27 19:26:57 2023, max compression
+gzip compressed data, was "ipyvasp-0.4.0.tar", last modified: Sun Jul  2 19:27:38 2023, max compression
```

## Comparing `ipyvasp-0.3.0.tar` & `ipyvasp-0.4.0.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 19:26:57.348920 ipyvasp-0.3.0/
--rw-rw-rw-   0        0        0     1263 2023-02-22 21:17:10.000000 ipyvasp-0.3.0/LICENSE
--rw-rw-rw-   0        0        0       77 2023-06-27 19:26:57.347425 ipyvasp-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1228 2023-06-24 22:17:33.000000 ipyvasp-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 19:26:57.330775 ipyvasp-0.3.0/ipyvasp/
--rw-rw-rw-   0        0        0     1803 2023-06-27 19:25:12.000000 ipyvasp-0.3.0/ipyvasp/__init__.py
--rw-rw-rw-   0        0        0    38535 2023-06-26 16:58:40.000000 ipyvasp-0.3.0/ipyvasp/_enplots.py
--rw-rw-rw-   0        0        0    88069 2023-06-26 17:49:02.000000 ipyvasp-0.3.0/ipyvasp/_lattice.py
--rw-rw-rw-   0        0        0    30580 2023-06-25 15:31:44.000000 ipyvasp-0.3.0/ipyvasp/bsdos.py
--rw-rw-rw-   0        0        0     2712 2023-06-24 19:19:43.000000 ipyvasp-0.3.0/ipyvasp/cli.py
-drwxrwxrwx   0        0        0        0 2023-06-27 19:26:57.347425 ipyvasp-0.3.0/ipyvasp/core/
--rw-rw-rw-   0        0        0        0 2023-06-24 01:13:48.000000 ipyvasp-0.3.0/ipyvasp/core/__init__.py
--rw-rw-rw-   0        0        0    37749 2023-06-25 19:45:39.000000 ipyvasp-0.3.0/ipyvasp/core/parser.py
--rw-rw-rw-   0        0        0    34873 2023-06-25 19:28:26.000000 ipyvasp-0.3.0/ipyvasp/core/plot_toolkit.py
--rw-rw-rw-   0        0        0    27729 2023-06-25 15:48:45.000000 ipyvasp-0.3.0/ipyvasp/core/serializer.py
--rw-rw-rw-   0        0        0    11584 2023-06-25 16:42:49.000000 ipyvasp-0.3.0/ipyvasp/core/spatial_toolkit.py
--rw-rw-rw-   0        0        0    25081 2023-06-27 18:35:21.000000 ipyvasp-0.3.0/ipyvasp/lattice.py
--rw-rw-rw-   0        0        0     1317 2023-06-25 00:23:12.000000 ipyvasp-0.3.0/ipyvasp/misc.py
--rw-rw-rw-   0        0        0    11416 2023-06-26 16:58:55.000000 ipyvasp-0.3.0/ipyvasp/potential.py
--rw-rw-rw-   0        0        0    23766 2023-06-25 19:47:03.000000 ipyvasp-0.3.0/ipyvasp/surface.py
--rw-rw-rw-   0        0        0    15028 2023-06-25 16:39:20.000000 ipyvasp-0.3.0/ipyvasp/utils.py
--rw-rw-rw-   0        0        0    44839 2023-06-25 16:39:34.000000 ipyvasp-0.3.0/ipyvasp/widgets.py
-drwxrwxrwx   0        0        0        0 2023-06-27 19:26:57.343142 ipyvasp-0.3.0/ipyvasp.egg-info/
--rw-rw-rw-   0        0        0       77 2023-06-27 19:26:57.000000 ipyvasp-0.3.0/ipyvasp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2023-06-27 19:26:57.000000 ipyvasp-0.3.0/ipyvasp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 19:26:57.000000 ipyvasp-0.3.0/ipyvasp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-27 19:26:57.000000 ipyvasp-0.3.0/ipyvasp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 19:26:57.348920 ipyvasp-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0       86 2023-06-27 19:25:05.000000 ipyvasp-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 19:27:38.169940 ipyvasp-0.4.0/
+-rw-rw-rw-   0        0        0     1263 2023-02-22 21:17:10.000000 ipyvasp-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     1862 2023-07-02 19:27:38.169940 ipyvasp-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1228 2023-06-24 22:17:33.000000 ipyvasp-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 19:27:38.083671 ipyvasp-0.4.0/ipyvasp/
+-rw-rw-rw-   0        0        0     1844 2023-07-02 19:12:11.000000 ipyvasp-0.4.0/ipyvasp/__init__.py
+-rw-rw-rw-   0        0        0    38535 2023-06-26 16:58:40.000000 ipyvasp-0.4.0/ipyvasp/_enplots.py
+-rw-rw-rw-   0        0        0    88362 2023-07-02 19:00:28.000000 ipyvasp-0.4.0/ipyvasp/_lattice.py
+-rw-rw-rw-   0        0        0       23 2023-07-02 19:26:08.000000 ipyvasp-0.4.0/ipyvasp/_version.py
+-rw-rw-rw-   0        0        0    30580 2023-06-25 15:31:44.000000 ipyvasp-0.4.0/ipyvasp/bsdos.py
+-rw-rw-rw-   0        0        0     2712 2023-06-24 19:19:43.000000 ipyvasp-0.4.0/ipyvasp/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-02 19:27:38.160705 ipyvasp-0.4.0/ipyvasp/core/
+-rw-rw-rw-   0        0        0        0 2023-06-24 01:13:48.000000 ipyvasp-0.4.0/ipyvasp/core/__init__.py
+-rw-rw-rw-   0        0        0    37726 2023-07-02 17:25:50.000000 ipyvasp-0.4.0/ipyvasp/core/parser.py
+-rw-rw-rw-   0        0        0    34144 2023-07-01 01:10:51.000000 ipyvasp-0.4.0/ipyvasp/core/plot_toolkit.py
+-rw-rw-rw-   0        0        0    28883 2023-07-01 23:07:24.000000 ipyvasp-0.4.0/ipyvasp/core/serializer.py
+-rw-rw-rw-   0        0        0    11706 2023-07-01 21:50:03.000000 ipyvasp-0.4.0/ipyvasp/core/spatial_toolkit.py
+-rw-rw-rw-   0        0        0    19335 2023-07-02 18:12:36.000000 ipyvasp-0.4.0/ipyvasp/evals_dataframe.py
+-rw-rw-rw-   0        0        0    25929 2023-07-02 19:05:49.000000 ipyvasp-0.4.0/ipyvasp/lattice.py
+-rw-rw-rw-   0        0        0     1317 2023-06-25 00:23:12.000000 ipyvasp-0.4.0/ipyvasp/misc.py
+-rw-rw-rw-   0        0        0    11406 2023-07-02 18:28:53.000000 ipyvasp-0.4.0/ipyvasp/potential.py
+-rw-rw-rw-   0        0        0    15160 2023-07-01 23:51:05.000000 ipyvasp-0.4.0/ipyvasp/utils.py
+-rw-rw-rw-   0        0        0    44823 2023-07-01 01:09:38.000000 ipyvasp-0.4.0/ipyvasp/widgets.py
+drwxrwxrwx   0        0        0        0 2023-07-02 19:27:38.147929 ipyvasp-0.4.0/ipyvasp.egg-info/
+-rw-rw-rw-   0        0        0     1862 2023-07-02 19:27:37.000000 ipyvasp-0.4.0/ipyvasp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2023-07-02 19:27:37.000000 ipyvasp-0.4.0/ipyvasp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 19:27:37.000000 ipyvasp-0.4.0/ipyvasp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      190 2023-07-02 19:27:37.000000 ipyvasp-0.4.0/ipyvasp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-02 19:27:37.000000 ipyvasp-0.4.0/ipyvasp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 19:27:38.169940 ipyvasp-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     3676 2023-07-02 19:25:02.000000 ipyvasp-0.4.0/setup.py
```

### Comparing `ipyvasp-0.3.0/LICENSE` & `ipyvasp-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.3.0/README.md` & `ipyvasp-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.3.0/ipyvasp/__init__.py` & `ipyvasp-0.4.0/ipyvasp/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 """ipyvasp is a processing tool for VASP DFT input/output processing.
 
 It is designed to primarily be used in Jupyter Notebook because it offers
 widgets for interactive visualization and bulk analysis.
 """
 
-__version__ = "0.3.0"
 
 __all__ = [  # For documentation purpose
     "get_axes",
     "plt2text",
     "plt2html",
     "iplot2html",
     "iplot2widget",
     "webshow",
     "list_files",
     "parse_text",
     "summarize",
     "OUTCAR",
 ]
 
+from ._version import __version__
 from .core.parser import *
 from .core.serializer import *
 from .misc import *
 from .lattice import *
 from .bsdos import *
 from .potential import *
-from .surface import *
+from .evals_dataframe import *
 from .utils import *
 from .widgets import summarize, BandsWidget, KpathWidget, FilesWidget
 from .core import plot_toolkit, spatial_toolkit
 from .core.spatial_toolkit import to_basis, to_R3, get_TM, get_bz, rotation
 from .core.plot_toolkit import (
     get_axes,  # other options are available as attributes of get_axes
     global_matplotlib_settings,
     plt2text,
     plt2html,
     iplot2html,
     iplot2widget,
     webshow,
 )
 
-
+version = __version__
 # Set global matplotlib settings for notebook.
 from cycler import cycler as __cycler
 
 global_matplotlib_settings(
     {
         "figure.dpi": 144,  # Better to See
         "figure.figsize": [4, 2.8],
```

### Comparing `ipyvasp-0.3.0/ipyvasp/_enplots.py` & `ipyvasp-0.4.0/ipyvasp/_enplots.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.3.0/ipyvasp/_lattice.py` & `ipyvasp-0.4.0/ipyvasp/_lattice.py`

 * *Files 0% similar despite different names*

```diff
@@ -882,18 +882,22 @@
 
     Returns
     -------
     matplotlib.pyplot.Axes
         Matplotlib's 2D axes if `plane=None` otherswise 3D axes.
     """
     vname = "a" if bz_data.__class__.__name__ == "CellData" else "b"
+    if vname == "b":  # These needed for splot_kpath internally
+        type(bz_data)._splot_kws = dict(plane=plane, zoffset=zoffset)
+
     label = r"$k_{}/2π$" if vname == "b" else "{}"
     if not ax:  # For both 3D and 2D, initialize 2D axis.
         ax = ptk.get_axes(figsize=(3.4, 3.4))  # For better display
 
+    type(bz_data)._splot_kws["ax"] = ax  # For splot_kpath
     _label = r"\vec{" + vname + "}"  # For both
 
     if vectors and not isinstance(vectors, (tuple, list)):
         raise ValueError(f"`vectors` expects tuple or list, got {vectors!r}")
 
     if vectors is None:
         vectors = ()  # Empty tuple to make things work below
@@ -973,19 +977,19 @@
                     lw=0.9,
                     color="navy",
                     angles="xy",
                     scale_units="xy",
                     scale=1,
                 )
 
-        ax.set_xlabel(label.format(idxs[plane][0]))
-        ax.set_ylabel(label.format(idxs[plane][1]))
+        ax.set_xlabel(label.format(plane[0]))
+        ax.set_ylabel(label.format(plane[1]))
         if is3d:
-            ind = [i for i in range(3) if i not in idxs[plane]][0]
-            ax.set_zlabel(label.format(ind))
+            lab = [v for v in "xyz" if v not in plane][0]
+            ax.set_zlabel(label.format(lab))
             ax.set_aspect("equal")
             zmin, zmax = ax.get_zlim()
             if zoffset > zmax:
                 zmax = zoffset
             elif zoffset < zmin:
                 zmin = zoffset
             ax.set_zlim([zmin, zmax])
@@ -998,14 +1002,15 @@
         else:
             pos = ax.get_position()
             fig = ax.get_figure()
             ax.remove()
             ax3d = fig.add_axes(
                 pos, projection="3d", azim=45, elev=30, proj_type="ortho"
             )
+            type(bz_data)._splot_kws["ax"] = ax3d
 
         if fill:
             if colormap:
                 colormap = colormap if colormap in plt.colormaps() else "viridis"
                 cz = [
                     np.mean(np.unique(f, axis=0), axis=0)[2]
                     for f in bz_data.faces_coords
@@ -1015,17 +1020,15 @@
             else:
                 colors = np.array(
                     [[*mplc.to_rgb(color)] for f in bz_data.faces_coords]
                 )  # Single color.
 
             poly = Poly3DCollection(
                 bz_data.faces_coords,
-                edgecolors=[
-                    color,
-                ],
+                edgecolors=[color],
                 facecolors=colors,
                 alpha=alpha,
                 shade=shade,
                 label=name,
                 **kwargs,
             )
 
@@ -1083,15 +1086,16 @@
     bz_data : Output of `get_bz`.
     fill : bool
         False by defult, determines whether to fill surface of BZ or not.
     color : str
         Color to fill surface 'rgba(168,204,216,0.4)` by default. This sholud be a valid Plotly color.
     special_kpoints : bool or callable
         True by default, determines whether to plot special points or not.
-        You can also proivide a mask function f(x,y,z) -> bool which will be used to filter special points based on their fractional coordinates.
+        You can also proivide a mask function f(x,y,z) -> bool which will be used to filter special points
+        based on their fractional coordinates. This is ignored if BZ is primitive.
     alpha : float
         Opacity of BZ planes.
     ortho3d : bool
         Default is True, decides whether x,y,z are orthogonal or perspective.
     fig : plotly.graph_objects.Figure
         Plotly's `go.Figure`. If you want to plot on another plotly's figure, provide that.
 
@@ -1214,16 +1218,16 @@
                 alphahull=0,
                 lighting=dict(diffuse=0.5),
                 legendgroup=zone_name,
                 name=zone_name,
             )
         )
 
-    # Special Points only if in reciprocal space.
-    if vname == "b" and special_kpoints:
+    # Special Points only if in reciprocal space and regular BZ
+    if vname == "b" and (not getattr(bz_data, "primitive", False)) and special_kpoints:
         if callable(special_kpoints):
             skpts = bz_data.specials.masked(special_kpoints)
         else:
             skpts = bz_data.specials
 
         for tr in fig.data:  # hide all traces hover made before
             tr.hoverinfo = "none"  # avoid overlapping with special points
```

### Comparing `ipyvasp-0.3.0/ipyvasp/bsdos.py` & `ipyvasp-0.4.0/ipyvasp/bsdos.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.3.0/ipyvasp/cli.py` & `ipyvasp-0.4.0/ipyvasp/cli.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.3.0/ipyvasp/core/parser.py` & `ipyvasp-0.4.0/ipyvasp/core/parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,14 +56,20 @@
         if not hasattr(self, "_poscar"):
             from ..lattice import POSCAR
 
             self._poscar = POSCAR(data=self.get_structure())
 
         return self._poscar  # keep same instance to avoid data loss
 
+    def get_evals_dataframe(self, spins=[0], bands=[0], atoms=None, orbs=None):
+        """Initialize and return an EvalsDataFrame instance, with the given parameters."""
+        from ..evals_dataframe import EvalsDataFrame
+
+        return EvalsDataFrame(self, spins=spins, bands=bands, atoms=atoms, orbs=orbs)
+
     # Following methods should be implemented in a subclass
     def get_summary(self):
         raise NotImplementedError(
             "`get_summary` should be implemented in a subclass. See Vasprun.get_summary as example."
         )
 
     def get_structure(self):
@@ -95,57 +101,38 @@
         raise NotImplementedError(
             "`get_scsteps` should be implemented in a subclass. See Vasprun.get_scsteps as example."
         )
 
 
 class Vaspout(DataSource):
     "Read data from vaspout.h5 file on demand."
+    # These methods are accessible from parent class, but need here for including in sphinx documentation
+    get_evals_dataframe = DataSource.get_evals_dataframe
+    poscar = DataSource.poscar
+    dos = DataSource.dos
+    bands = DataSource.bands
 
     def __init__(self, path):
         raise NotImplementedError("Vaspout is not implemented yet.")
 
-    @property
-    def bands(self):
-        "Access ipyvasp.bsdos.Bands class singleton instance for current Vaspout class."
-        return super().bands
-
-    @property
-    def dos(self):
-        "Access ipyvasp.bsdos.DOS class singleton instance for current Vaspout class."
-        return super().dos
-
-    @property
-    def poscar(self):
-        "Access ipyvasp.lattice.POSCAR class instance."
-        return super().poscar
 
 class Vasprun(DataSource):
     "Reads vasprun.xml file lazily. It reads only the required data from the file when a plot or data access is requested."
+    # These methods are accessible from parent class, but need here for including in sphinx documentation
+    get_evals_dataframe = DataSource.get_evals_dataframe
+    poscar = DataSource.poscar
+    dos = DataSource.dos
+    bands = DataSource.bands
 
     def __init__(self, path="./vasprun.xml", skipk=None):
         super().__init__(path)
         self._skipk = (
             skipk if isinstance(skipk, (int, np.integer)) else self.get_skipk()
         )
 
-    @property
-    def bands(self):
-        "Access ipyvasp.bsdos.Bands class singleton instance for current Vasprun class."
-        return super().bands
-
-    @property
-    def dos(self):
-        "Access ipyvasp.bsdos.DOS class singleton instance for current Vasprun class."
-        return super().dos
-
-    @property
-    def poscar(self):
-        "Access ipyvasp.lattice.POSCAR class instance."
-        return super().poscar
-
     def read(self, start_match, stop_match, nth_match=1, skip_last=False):
         """Reads a part of the file between start_match and stop_match and returns a generator. It is lazy and fast.
         `start_match` and `stop_match` are regular expressions. `nth_match` is the number of occurence of start_match to start reading.
         `skip_last` is used to determine whether to keep or skip last line.
         """
         if "|" in start_match:
             raise ValueError(
@@ -516,17 +503,18 @@
                     "bands should be a list, tuple or range got {}".format(type(bands))
                 )
             for b in bands:
                 if (not isinstance(b, (int, np.integer))) and (b < 0):
                     raise TypeError(
                         "bands should be a tuple/list/range of of positive integers"
                     )
-            evals = evals[:, :, (bands,)]
-            occs = occs[:, :, (bands,)]
-            bands_range = bands
+            _bands = list(bands)
+            evals = evals[:, :, _bands]
+            occs = occs[:, :, _bands]
+            bands_range = _bands
         elif elim:
             if (not isinstance(elim, (list, tuple))) and (len(elim) != 2):
                 raise TypeError("elim should be a tuple of length 2")
 
             if ezero is not None:
                 if not isinstance(ezero, (int, np.integer, float)):
                     raise TypeError("ezero should be a float or integer")
```

### Comparing `ipyvasp-0.3.0/ipyvasp/core/plot_toolkit.py` & `ipyvasp-0.4.0/ipyvasp/core/plot_toolkit.py`

 * *Files 1% similar despite different names*

```diff
@@ -840,15 +840,15 @@
 
     return cax
 
 
 def webshow(transparent=False):
     """Displays all available figures in browser without blocking terminal"""
     for i in plt.get_fignums():
-        svg = plt2html(plt.figure(i), transparent=transparent, dash_html=False)
+        svg = plt2html(plt.figure(i), transparent=transparent)
         html_str = """\
 <!DOCTYPE html>
 <head></head>
 <body>
     <div>
     {}
     </div>
@@ -929,76 +929,61 @@
             f.write(out_str)
     else:
         # For loop is important for printing lines, otherwise breaks appear.
         for line in out_str.splitlines():
             print(line)
 
 
-def plt2html(plt_fig=None, transparent=True, out_string=False):
-    """
-    Display svg image in notebook, or return <svg> or show image from terminal.
+def plt2html(plt_fig=None, transparent=True):
+    """Returns ``ipython.display.HTML(<svg of figure>)``. It clears figure after use. So ``plt.show()`` will not work after this.
 
     Parameters
     ----------
     plt_fig : Matplotlib's figure instance, auto picks as well.
     transparent : True of False for fig background.
-    out_string : If True, returns <svg> string.
     """
     if plt_fig is None:
         plt_fig = plt.gcf()
     plot_bytes = BytesIO()
     plt.savefig(plot_bytes, format="svg", transparent=transparent)
 
-    if out_string:
-        _ = plt.clf()  # Clear image
-        return "<svg" + plot_bytes.getvalue().decode("utf-8").split("<svg")[1]
-    else:
-        try:
-            shell = get_ipython().__class__.__name__
-            if (
-                shell == "ZMQInteractiveShell" or shell == "Shell"
-            ):  # Shell for Colab. Don't know why Google ...
-                _ = plt.clf()  # Clear other display
-                return HTML(
-                    "<svg" + plot_bytes.getvalue().decode("utf-8").split("<svg")[1]
-                )
-        except:
-            return plt.show()
+    _ = plt.clf()  # Clear other display
+    return HTML("<svg" + plot_bytes.getvalue().decode("utf-8").split("<svg")[1])
 
 
-def iplot2html(fig, filename=None, out_string=False, modebar=True):
-    """
-    Writes plotly's figure as HTML file or display in IPython which is accessible when online. It is different than plotly's `fig.to_html` as it is minimal in memory. If you need to have offline working file, just use `fig.write_html('file.html')` which will be larger in size.
+def iplot2html(fig, outfile=None, modebar=True):
+    """Writes plotly's figure as HTML file or display in IPython which is accessible when online.
+    It is different than plotly's `fig.to_html` as it is minimal in memory. If you need to have
+    offline working file, just use `fig.write_html('file.html')` which will be larger in size.
 
     Parameters
     ----------
     fig : A plotly's figure object.
-    filename : Name of file to save fig. Defualt is None and show plot in Colab/Online or return hrml string.
-    out_string : If True, returns HTML string, if False displays graph if possible.
+    outfile : Name of file to save fig. Defualt is None and show plot in Notebook.
     modebar : If True, shows modebar in graph. Default is True. Not used if saving to file.
     """
     div_id = "graph-{}".format(uuid1())
     fig_json = fig.to_json()
     # a simple HTML template
-    if filename:
+    if outfile:
         template = """<html>
         <head>
         <script src="https://cdn.plot.ly/plotly-latest.min.js"></script>
         </head>
         <body>
             <div id='{}'></div>
             <script>
                 var fig_data = {}
                 Plotly.react('{}', fig_data.data, fig_data.layout);
             </script>
         </body>
         </html>"""
 
         # write the JSON to the HTML template
-        with open(filename, "w") as f:
+        with open(outfile, "w") as f:
             f.write(template.format(div_id, fig_json, div_id))
 
     else:
         if modebar == True:  # Only for docs issue
             config = "{displayModeBar: true,scrollZoom: true}"
         else:
             config = "{displayModeBar: false,scrollZoom: true}"
@@ -1009,18 +994,15 @@
                 var data = {};
                 var config = {};
                 Plotly.newPlot('{}', data.data,data.layout,config);
             </script>
         </div>""".format(
             div_id, fig_json, config, div_id
         )
-        if out_string is True:
-            return template
-        else:
-            return HTML(template)
+        return HTML(template)
 
 
 def iplot2widget(fig, fig_widget=None, template=None):
     "Converts plotly's figure to FigureWidget by copying attributes and data. If fig_widget is provided, it will update it. Adds template if provided."
     if not isinstance(fig, go.Figure):
         raise ValueError("fig must be instance of plotly.graph_objects.Figure")
```

### Comparing `ipyvasp-0.3.0/ipyvasp/core/serializer.py` & `ipyvasp-0.4.0/ipyvasp/core/serializer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,27 @@
-__all__ = ["dump", "load", "dict2tuple", "Dict2Data"]
+__all__ = [
+    "dump",
+    "load",
+    "dict2tuple",
+    "Dict2Data",
+    "PoscarData",
+    "BrZoneData",
+    "CellData",
+]
 
-import json
+import json, re
 import pickle
 import inspect
 from collections import namedtuple
 from copy import deepcopy
 from pathlib import Path
 
 import numpy as np
 
-from .spatial_toolkit import angle_deg, to_basis, to_R3, kpoints2bz
+from .spatial_toolkit import angle_deg, to_basis, to_R3, kpoints2bz, get_bz
 
 
 def dict2tuple(name: str, d: dict):
     """
     Converts a dictionary (nested as well) to namedtuple, accessible via index and dot notation as well as by unpacking.
 
     Parameters
@@ -121,25 +129,25 @@
         Dumps a `Dict2Data` object (root or nested level) to json.
 
         Parameters
         ----------
         outfile : str, Default is None and returns string. If given, writes to file.
         indent : int, JSON indent. Default is 1.
         """
-        return dump(self, dump_to="json", outfile=outfile, indent=indent)
+        return dump(self, format="json", outfile=outfile, indent=indent)
 
     def to_pickle(self, outfile: str = None):
         """
         Dumps a `Dict2Data` or subclass object (root or nested level) to pickle.
 
         Parameters
         ---------
         outfile : str, Default is None and returns string. If given, writes to file.
         """
-        return dump(self, dump_to="pickle", outfile=outfile)
+        return dump(self, format="pickle", outfile=outfile)
 
     def to_tuple(self):
         """Creates a namedtuple."""
         return dict2tuple("Data", self.to_dict())
 
     def __repr__(self):
         items = []
@@ -414,35 +422,57 @@
 class SubZoneData(Dict2Data):
     _req_keys = ("vertices", "faces", "specials")
 
     def __init__(self, d):
         super().__init__(d)
 
     def splot(plane=None):
+        # Implemenet using splot under BrZoneData
         raise NotImplementedError("Not implemented yet")
 
     def iplot():
+        # Implemenet using iplot under BrZoneData
         raise NotImplementedError("Not implemented yet")
 
 
+def _methods_imported():
+    # These imports work as methods of the class
+    from .._lattice import splot_bz as splot, iplot_bz as iplot  # Avoid circular import
+
+    splot.__doc__ = re.sub(  # This replaces orginal docstring too. That is strange
+        "bz_data :.*plane :", "plane :", splot.__doc__, flags=re.DOTALL
+    )
+    iplot.__doc__ = re.sub(
+        "bz_data :.*fill :", "fill :", iplot.__doc__, flags=re.DOTALL
+    )
+    return splot, iplot
+
+
 class BrZoneData(Dict2Data):
+    splot, iplot = _methods_imported()
     _req_keys = ("basis", "faces", "vertices", "primitive")
 
     def __init__(self, d):
         super().__init__(d)
 
     def get_special_points(self, orderby=(1, 1, 1)):
-        "Returns the special points in the brillouin zone in the order relative to a given point in cartesian coordinates. Gamma is always first."
+        """Returns the special points in the brillouin zone in the order relative
+        to a given point in cartesian coordinates. Gamma is always first."""
+        if self.primitive:
+            return SpecialPoints(
+                {"coords": np.empty((0, 3)), "kpoints": np.empty((0, 3))}
+            )  # Primitive Zone has no meaning for special points
+
         mid_faces = np.array(
             [np.mean(np.unique(face, axis=0), axis=0) for face in self.faces_coords]
         )
         mid_edges = []
         for f in self.faces_coords:
             for i in range(len(f) - 1):
-                # Do not insert point between unique vertices
+                # NOTE: Do not insert point between unique vertices, is it necessary?
                 if np.isclose(np.linalg.norm(f[i]), np.linalg.norm(f[i + 1])):
                     mid_edges.append(np.mean([f[i], f[i + 1]], axis=0))
 
         if mid_edges != []:
             mid_edges = np.unique(mid_edges, axis=0)  # because faces share edges
             mid_faces = np.concatenate([mid_faces, mid_edges])
 
@@ -515,28 +545,33 @@
             raise TypeError(
                 f"other must be a {self.__class__} object, got {type(other)}"
             )
         return other.to_fractional(self.to_cartesian(kpoints))
 
     def translate_inside(self, kpoints, shift=0):
         """Brings kpoints inside BZ. Mostly useful for regular kmesh to bring all kpoints inside BZ.
-        `shift` is a number or a list of three numbers that will be added to kpoints before any other operation, in case points are not symmetric around origin.
+        `shift` is a number or a list of three numbers that will be added to kpoints before any other operation,
+        in case points are not symmetric around origin.
+
+        .. warning::
+            If you made cartesian kpoints, you should not translate them with this function, just shift them by adding a vector.
         """
         return kpoints2bz(self, kpoints, shift=shift)
 
     def get_subzone(self, func):
         # Disclaimer: Reuduction totally depends on given function, we only test for volume to satify the condition V_old = N * V_new
         # This should add an attrivute to not recalculate special points, just return old points including in this zone
         # How to plot the reduced zone, as it will be nowhere? or make this a plotting function? or add new namespace to POSACR? like splot_bzr(func), thing?
         # return SubZoneData({"vertices","faces", "specials"})
         # specials here should not be recalculated, old ones with in this zone
         raise NotImplementedError("Not implemented yet")
 
 
 class CellData(Dict2Data):
+    splot, iplot = _methods_imported()
     _req_keys = ("basis", "faces", "vertices")
 
     def __init__(self, d):
         super().__init__({k: v for k, v in d.items() if k != "primitive"})
 
     @property
     def faces_coords(self):
@@ -651,46 +686,45 @@
             return np.array(obj["_value_"])
         elif kind == "range":
             value = obj["_value_"]
             return range(value[0], value[-1])
         return obj
 
 
-def dump(
-    dict_data, dump_to: str = "pickle", outfile: str = None, indent: int = 1
-) -> None:
-    """
-    Dump ``Dict2Data`` or subclass object or any dictionary to json or pickle string/file.
+def dump(data, format: str = "pickle", outfile: str = None, indent: int = 1) -> None:
+    """Dump ``Dict2Data`` or subclass object or any dictionary to json or pickle string/file.
 
     Parameters
     ----------
-    dict_data : dict or instance of Dict2Data, Any dictionary/Dict2Data(or subclass Data) object containg numpy arrays.
-    dump_to : str, Defualt is ``pickle`` or ``json``.
-    outfile : str, Defualt is None and return string. File name does not require extension.
-    indent : int, Defualt is 1. Only works for json.
+    data : dict or instance of Dict2Data
+        Any dictionary/Dict2Data(or subclass Data) object can be saved.
+    format : str,
+        Defualt is ``pickle``. Should be ``pickle`` or ``json``.
+    outfile : str
+        Defualt is None and return string. File name does not require extension as it is added from ``format``.
+    indent : int
+        Defualt is 1. Only works for json.
     """
-    if dump_to not in ["pickle", "json"]:
-        raise ValueError(
-            "`dump_to` expects 'pickle' or 'json', got '{}'".format(dump_to)
-        )
+    if format not in ["pickle", "json"]:
+        raise ValueError("`format` expects 'pickle' or 'json', got '{}'".format(format))
     try:
-        dict_obj = dict_data.to_dict()  # Change Data object to dictionary
+        dict_obj = data.to_dict()  # Change Data object to dictionary
         dict_obj = {
-            "_loader_": dict_data.__class__.__name__,
+            "_loader_": data.__class__.__name__,
             "_data_": dict_obj,
         }  # Add class name to dictionary for reconstruction
     except:
-        dict_obj = dict_data
-    if dump_to == "pickle":
+        dict_obj = data
+    if format == "pickle":
         if outfile == None:
             return pickle.dumps(dict_obj)
         outfile = Path(outfile).stem + ".pickle"
         with open(outfile, "wb") as f:
             pickle.dump(dict_obj, f)
-    if dump_to == "json":
+    if format == "json":
         if outfile == None:
             return json.dumps(dict_obj, cls=EncodeFromNumpy, indent=indent)
         outfile = Path(outfile).stem + ".json"
         with open(outfile, "w") as f:
             json.dump(dict_obj, f, cls=EncodeFromNumpy, indent=indent)
     return None
```

### Comparing `ipyvasp-0.3.0/ipyvasp/core/spatial_toolkit.py` & `ipyvasp-0.4.0/ipyvasp/core/spatial_toolkit.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,22 +295,24 @@
     }
     from .serializer import BrZoneData  # to avoid circular import
 
     return BrZoneData(out_dict)
 
 
 def kpoints2bz(bz_data, kpoints, shift=0):
-    """
-    Brings KPOINTS inside BZ. Applies `to_R3` only if bz_data is for primitive BZ.
+    """Brings KPOINTS inside BZ. Applies `to_R3` only if bz_data is for primitive BZ.
 
     Parameters
     ----------
     bz_data : Output of get_bz().
     kpoints : List or array of KPOINTS to transorm into BZ or R3.
     shift : This value is added to kpoints before any other operation, single number of list of 3 numbers for each direction.
+
+    .. warning::
+        Do not use this function to translate kpoints created as cartesian, just shift by adding a vector.
     """
     kpoints = np.array(kpoints) + shift
     if bz_data.primitive:
         return to_R3(bz_data.basis, kpoints)
 
     cent_planes = [
         np.mean(np.unique(face, axis=0), axis=0) for face in bz_data.faces_coords
```

### Comparing `ipyvasp-0.3.0/ipyvasp/lattice.py` & `ipyvasp-0.4.0/ipyvasp/lattice.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
     "POSCAR",
     "download_structure",
     "periodic_table",
     "get_kpath",
     "get_kmesh",
     "splot_bz",
     "iplot_bz",
+    "ngl_viewer",
 ]
 
 from pathlib import Path
 from contextlib import redirect_stdout
 from io import StringIO
-from functools import partial
 
 import numpy as np
 from pandas.io.clipboard import clipboard_get, clipboard_set
 import matplotlib.colors as mcolors
 
 
 from .core import serializer
@@ -76,14 +76,15 @@
     plot_cell=True,
     linewidth=0.05,
     color=[0, 0, 0.2],
     bond_color="whitesmoke",
     width="400px",
     height="400px",
     plot_vectors=True,
+    dashboard=False,
 ):
     """Display structure in Jupyter notebook using nglview.
 
     Parameters
     ----------
     poscar : ipyvasp.POSCAR
     colors : list or str
@@ -103,22 +104,27 @@
         Color of bonds. Default "whitesmoke". Can be "element" or any other scheme from `nglview`.
     width : str
         Width of viewer. Default "400px".
     height : str
         Height of viewer. Default "400px".
     plot_vectors : bool
         Plot vectors. Default True. Only works if `plot_cell = True`.
+    dashboard : bool
+        Show dashboard. Default False. It just sets `view.gui_style = 'NGL'`.
 
     Returns
     -------
     NGLWidget
         An instance of nglview.NGLWidget object. You can use `.render_image()`, `.download_image()` etc. on it or can add more representations.
 
     .. note::
         `nglview` sometimes does not work in Jupyter lab. You can switch to classic notebook in that case.
+
+    .. tip::
+        See `Advanced NGLView usage <https://projects.volkamerlab.org/teachopencadd/talktorials/T017_advanced_nglview_usage.html>`_.
     """
     if not isinstance(poscar, POSCAR):
         raise TypeError("poscar must be an instance of POSCAR class.")
 
     try:
         import nglview as nv
     except ImportError:
@@ -160,30 +166,34 @@
         view.add_spacefill(radius=r, selection=f"#{e}", color=c)
 
     view.add_ball_and_stick(color=bond_color)
     view.camera = "orthographic"
     view.center()
 
     if plot_cell:
+        # arrays.tolist() is important for nglview to write json
         shape = nv.shape.Shape(view=view)
         _color = mcolors.to_rgb(color)  # convert to rgb for nglview
         cell = poscar.get_cell()
         for face in cell.faces_coords:
             for p1, p2 in zip(face[1:], face[:-1]):
-                shape.add_cylinder(p1, p2, _color, linewidth)
+                shape.add_cylinder(p1.tolist(), p2.tolist(), _color, linewidth)
 
         for v in cell.vertices:
-            shape.add_sphere(v, _color, linewidth)
+            shape.add_sphere(v.tolist(), _color, linewidth)
 
         if plot_vectors:
             for i, b in enumerate(cell.basis, start=1):
                 tail = b - b / np.linalg.norm(b)
-                shape.add_cone(tail, b, _color, linewidth * 3, f"a{i}")
-                shape.add_text(b / 2, [0.2, 0.15, 0.2], 2, f"a{i}")
-
+                shape.add_cone(
+                    tail.tolist(), b.tolist(), _color, linewidth * 3, f"a{i}"
+                )
+                shape.add_text((b / 2).tolist(), [0.2, 0.15, 0.2], 2, f"a{i}")
+    if dashboard:
+        view.gui_style = "NGL"
     return view
 
 
 class POSCAR:
     _cb_instance = {}  # Loads last clipboard data if not changed
     _mp_instance = {}  # Loads last mp data if not changed
 
@@ -206,16 +216,14 @@
         if data:
             self._data = serializer.PoscarData.validated(data)
         else:
             self._data = plat.export_poscar(path=str(self.path), content=content)
         # These after data to work with data
         self._bz = self.get_bz(primitive=False)  # Get defualt regular BZ from sio
         self._cell = self.get_cell()  # Get defualt cell
-        self._plane = None  # Get defualt plane, changed with splot_bz
-        self._ax = None  # Get defualt axis, changed with splot_bz
 
     def __repr__(self):
         atoms = ", ".join([f"{k}={len(v)}" for k, v in self._data.types.items()])
         lat = ", ".join(
             [
                 f"{k}={v}"
                 for k, v in zip(
@@ -260,14 +268,18 @@
         data should be volumetric data for ase.visualize.view, such as charge density, spin density, etc.
 
         .. tip::
             Use ``self.view_ngl()`` if you don't want to pass ``viewer = 'nglview'`` to ASE viewer or not showing volumetric data.
         """
         if viewer is None:
             return plat.view_poscar(self.data, **kwargs)
+        elif viewer in "nglview":
+            return print(
+                f"Use `self.view_ngl()` for better customization in case of viewer={viewer!r}"
+            )
         else:
             from ase.visualize import view
 
             return view(self.to_ase(), viewer=viewer, data=kwargs.get("data", None))
 
     @_sub_doc(ngl_viewer, {"poscar :.*colors :": "colors :"})
     @_sig_kwargs(ngl_viewer, ("poscar",))
@@ -436,39 +448,39 @@
     @property
     def cell(self):
         return self._cell
 
     @_sub_doc(stk.get_bz, {"basis :.*loop :": "loop :"})
     @_sig_kwargs(stk.get_bz, ("basis",))
     def get_bz(self, **kwargs):
-        self._bz = stk.get_bz(self._data.rec_basis, **kwargs)
+        self.set_bz(**kwargs)  # set bz to current data
         return self._bz
 
+    def set_bz(self, primitive=False, loop=True):
+        """Set BZ to primitve/regular on demand. All successive operations follow the current set BZ."""
+        self._bz = stk.get_bz(self._data.rec_basis, primitive=primitive, loop=loop)
+
     def get_cell(self, loop=True):
         "See docs of `get_bz`, same except space is inverted and no factor of 2pi."
         self._cell = serializer.CellData(
             stk.get_bz(  # data.basis makes prmitive cell in direct space
                 basis=self.data.basis, loop=loop, primitive=True
             ).to_dict()
         )  # cell must be primitive
         return self._cell
 
     @_sub_doc(plat.splot_bz, {"bz_data :.*plane :": "plane :"})
     @_sig_kwargs(plat.splot_bz, ("bz_data",))
     def splot_bz(self, plane=None, **kwargs):
-        self._plane = plane  # Set plane for splot_kpath
-        new_ax = plat.splot_bz(bz_data=self._bz, plane=plane, **kwargs)
-        self._ax = new_ax  # Set ax for splot_kpath
-        self._zoffset = kwargs.get("zoffset", 0)  # Set zoffset for splot_kpath
-        return new_ax
+        return plat.splot_bz(bz_data=self._bz, plane=plane, **kwargs)
 
     def splot_kpath(
         self, kpoints, labels=None, fmt_label=lambda x: (x, {"color": "blue"}), **kwargs
     ):
-        """Plot k-path over existing BZ.
+        """Plot k-path over existing BZ. It will take ``ax``, ``plane`` and ``zoffset`` internally from most recent call to ``self.splot_bz``/``self.bz.splot``.
 
         Parameters
         ----------
         kpoints : array_like
             List of k-points in fractional coordinates. e.g. [(0,0,0),(0.5,0.5,0.5),(1,1,1)] in order of path.
         labels : list
             List of labels for each k-point in same order as kpoints.
@@ -480,77 +492,84 @@
 
         You can get ``kpoints = POSCAR.get_bz().specials.masked(lambda x,y,z : (-0.1 < z 0.1) & (x >= 0) & (y >= 0))`` to get k-points in positive xy plane.
         Then you can reorder them by an indexer like ``kpoints = kpoints[[0,1,2,0,7,6]]``, note double brackets, and also that point at zero index is taken twice.
 
         .. tip::
             You can use this function multiple times to plot multiple/broken paths over same BZ.
         """
-        if not self._bz or not self._ax:
-            raise ValueError("BZ not found, use `splot_bz` first")
+        if not self._bz or not hasattr(self._bz, "_splot_kws"):
+            raise ValueError(
+                "BZ data or plot not found, use `self.splot_bz` or `self.bz.splot` first"
+            )
 
         if not np.ndim(kpoints) == 2 and np.shape(kpoints)[-1] == 3:
             raise ValueError("kpoints must be 2D array of shape (N,3)")
 
+        plane, ax, zoffset = [
+            self._bz._splot_kws.get(attr, default)  # class level attributes
+            for attr, default in zip(["plane", "ax", "zoffset"], [None, None, 0])
+        ]
+
         ijk = [0, 1, 2]
         _mapping = {
             "xy": [0, 1],
             "xz": [0, 2],
             "yz": [1, 2],
             "zx": [2, 0],
             "zy": [2, 1],
             "yx": [1, 0],
         }
         _zoffset = [0, 0, 0]
-        if self._plane:
+        if plane:
             _zoffset = (
-                [0, 0, self._zoffset]
-                if self._plane in "xyx"
-                else [0, self._zoffset, 0]
-                if self._plane in "xzx"
-                else [self._zoffset, 0, 0]
+                [0, 0, zoffset]
+                if plane in "xyx"
+                else [0, zoffset, 0]
+                if plane in "xzx"
+                else [zoffset, 0, 0]
             )
 
-        if isinstance(self._plane, str) and self._plane in _mapping:
-            if getattr(self._ax, "name", None) != "3d":
+        if isinstance(plane, str) and plane in _mapping:
+            if getattr(ax, "name", None) != "3d":
                 ijk = _mapping[
-                    self._plane
+                    plane
                 ]  # only change indices if axes is not 3d, even if plane is given
 
         if not labels:
             labels = [
                 "[{0:5.2f}, {1:5.2f}, {2:5.2f}]".format(x, y, z) for x, y, z in kpoints
             ]
 
         plat._validate_label_func(fmt_label, labels[0])
 
         coords = self.bz.to_cartesian(kpoints)
-        if _zoffset and self._plane:
+        if _zoffset and plane:
             normal = (
                 [0, 0, 1]
-                if self._plane in "xyx"
+                if plane in "xyx"
                 else [0, 1, 0]
-                if self._plane in "xzx"
+                if plane in "xzx"
                 else [1, 0, 0]
             )
             coords = plat.to_plane(normal, coords) + _zoffset
 
         coords = coords[:, ijk]  # select only required indices
         kwargs = {
             **dict(color="blue", linewidth=0.8, marker=".", markersize=10),
             **kwargs,
         }  # need some defaults
-        self._ax.plot(*coords.T, **kwargs)
+        ax.plot(*coords.T, **kwargs)
 
         for c, text in zip(coords, labels):
             lab, textkws = fmt_label(text), {}
             if isinstance(lab, (list, tuple)):
                 lab, textkws = lab
-            self._ax.text(*c, lab, **textkws)
+            ax.text(*c, lab, **textkws)
 
-        return self._ax
+        return ax
 
     @_sig_kwargs(plat.splot_bz, ("bz_data",))
     def splot_cell(self, plane=None, **kwargs):
         "See docs of `splot_bz`, everything is same except space is inverted."
         return plat.splot_bz(bz_data=self._cell, plane=plane, **kwargs)
 
     @_sub_doc(plat.iplot_bz, {"bz_data :.*fill :": "fill :"})
```

### Comparing `ipyvasp-0.3.0/ipyvasp/misc.py` & `ipyvasp-0.4.0/ipyvasp/misc.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.3.0/ipyvasp/potential.py` & `ipyvasp-0.4.0/ipyvasp/potential.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,16 +194,15 @@
         operation: str = "mean_c",
         interface=0.5,
         lr_pos=(0.25, 0.75),
         smoothness=2,
         figsize=(5, 3),
         **kwargs,
     ):
-        """
-        Check periodicity using ipywidgets interactive plot.
+        """Check periodicity using ipywidgets interactive plot.
 
         Parameters
         ----------
         operation : What to do, such as 'mean_c' or 'mean_a' etc.
         interface : Interface in range [0,1] to divide left and right halves.
         lr_pos : Tuple of (left,right) positions in range [0,1] to get ΔV of right relative to left.
         smoothness : int. Default is 2. Smoothing parameter for rolling mean. Larger is better.
```

### Comparing `ipyvasp-0.3.0/ipyvasp/surface.py` & `ipyvasp-0.4.0/ipyvasp/evals_dataframe.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,244 +1,116 @@
-__all__ = ["SpinDataFrame"]
+__all__ = ["EvalsDataFrame"]
 
 import numpy as np
 import pandas as pd
 from scipy.interpolate import griddata
 import matplotlib.pyplot as plt
 
 # Inside packages import
-from .core import parser as vp, serializer
+from .core.parser import DataSource
 from .core import plot_toolkit as ptk
-from .lattice import POSCAR
-from .bsdos import _format_input
 
 
-# Need to get it from source like Vasprun, and then get_evals
-def _collect_spin_data(source, bands=[0], projections={"A": ([0], [0])}):
-    if not isinstance(bands, (list, tuple)):
-        raise TypeError("`bands` must be list/tuple of integer.")
-    atoms, orbs, *_ = _format_input(projections, sys_info=source.summary)
-
-    def per_band_data(band):
-        kpoints = source.kpoints
-        evals = {k: v[..., band] for k, v in source.evals.items() if k in "eud"}
-        spins = {k: v[..., band, :] for k, v in source.spins.items() if k in "sxyzud"}
-
-        df_dict = {f"k{k}": v for k, v in zip("xyz", kpoints.T)}
-        df_dict["band"] = [
-            (band + source.evals.indices[0] + 1) for i in range(len(kpoints))
-        ]
+def _collect_data(source, spins=None, bands=None, atoms=None, orbs=None):
+    if not isinstance(source, DataSource):
+        raise TypeError("`source` must be a valid `DataSource` object.")
 
-        for k, v in evals.items():
-            df_dict[k if k == "e" else f"e{k}"] = v.T.flatten() - source.summary.EFERMI
+    kpoints = source.get_kpoints()  # data object, not single array
+    evals = source.get_evals(spins=spins, bands=bands, atoms=atoms, orbs=orbs)
+    NS, NK, NB = evals.evals.shape
 
-        for i, (a, o) in enumerate(zip(atoms, orbs)):
-            for k, v in spins.items():
-                if k in "sxyzud":
-                    key = k if k == "s" else f"s{k}"
-                    df_dict[f"{key}_{i}"] = (
-                        v.take(a, axis=0)
-                        .take(o, axis=2)
-                        .sum(axis=2)
-                        .sum(axis=0)
-                        .T.flatten()
-                    )
+    df_dict = {}
+    for arr, name in zip(kpoints.kpoints.T, "xyz"):
+        df_dict[f"k{name}"] = np.array([arr for _ in range(NB)]).flatten()
 
-        return df_dict
+    for arr, name in zip(kpoints.coords.T, "xyz"):
+        df_dict[f"{name}"] = np.array([arr for _ in range(NB)]).flatten()
 
-    main_dict = per_band_data(bands[0])
-    for b in bands[1:]:
-        data = per_band_data(b)
-        for k, v in main_dict.items():
-            main_dict[k] = [*main_dict[k], *data[k]]
-
-    if (
-        atoms
-    ):  # NOTE: Make room for negative peak to peak. Only scale if projections given
-        _max = []
-        for k, v in main_dict.items():
-            if k.startswith("s"):
-                _max.append(np.abs(v).max())
-
-        _max = max(_max)
-        for k, v in main_dict.items():
-            if k.startswith("s"):
-                main_dict[k] = v / (_max if _max != 0 else 1)
-    return main_dict
+    df_dict["kpt"] = np.array([[i for i in range(NK)] for _ in evals.bands]).flatten()
+    df_dict["band"] = np.array([[i for _ in range(NK)] for i in evals.bands]).flatten()
 
+    for s in range(NS):
+        key = "e" + "ud"[s] if NS == 2 else "e"
+        df_dict[key] = evals.evals[s].T.flatten()
 
-class SpinDataFrame(pd.DataFrame):
-    """
-    Spin data from vasprun.xml is converted to a dataframe.
+    if hasattr(evals, "orbs"):  # If projections are given
+        _orbs = range(evals.pros.shape[-1]) if evals.orbs == -1 else evals.orbs
+        _atoms = range(evals.pros.shape[-2]) if evals.atoms == -1 else evals.atoms
+
+        for a in _atoms:
+            for o in _orbs:
+                for s in range(NS):  # looking spin together in columns is better
+                    key = "ud"[s] if NS == 2 else "sxyz"[s]
+                    df_dict[f"{key}{a}_{o}"] = evals.pros[s, a, o, ...].T.flatten()
+
+    return df_dict, source.summary, source.poscar, evals.ezero
+
+
+class EvalsDataFrame(pd.DataFrame):
+    """Format eigenvalues from a data source to dataframe.
 
     Parameters
     ----------
-    path : path to `vasprun.xml` or auto picks in current directory.
-    bands : list of band indices [zero based here], In output data frame you will see corresponding band number based on full data.
-    atoms : list of atoms to plot. inner list contains ions indices. Can leave empty to discard projection data.
-    orbs : list of orbitals to plot. inner list contains orbitals indices. Can leave empty to discard projection data
-    skipk : if not None, auto skipped unnecessary k-points.
-    elim : if not None, filtered out unnecessary bands.
-    data : if not None, data is loaded from given data/pickle/json/dict and validated. Many other parameters are ignored when data is given.
+    source : DataSource
+        Data source to collect data from. Could be ``ipyvasp.Vasprun`` or ``ipyvasp.Vaspout``.  Alternatively you can use ``DataSource.get_dataframe`` method to get dataframe directly.
+    spins : list
+
+    bands : list
+        of band indices [zero based here], In output data frame you will see corresponding band number based on full data.
+    atoms : list
+        of atoms to plot. inner list contains ions indices. Can leave empty to discard projection data.
+    orbs : list
+        of orbitals to plot. inner list contains orbitals indices. Can leave empty to discard projection data
+
+
+    kwargs are not used during initialization, they are internally used by dataframe operations.
 
     Returns
     -------
-    SpinDataFrame : dataframe with colums as k-points, eigenvalues[with fermi energy subtracted], spin components projected over selected ions and orbtials.
+    EvalsDataFrame
+        A subclass of DataFrame with extra methods and attributes.
+
+    Attributes
+    ----------
+    poscar : ipyvasp.POSCAR
+    summary : ipyvasp.DataSource.summary
 
     Methods
     -------
     sliced : Slice data in a plane orthogonal to given `column` at given `value`.
     masked : Mask data over a constant value in a given column. Useful for plotting fermi level/surface.
     splot : plot data in a 2D plot.
     splot3d : plot data in a 3D plot.
-    join/append/concat/+/+= : Append another SpinDataFrame to this one with same columns and copy metadata.
-    send_metadata : Copy metadata from this to another SpinDataFrame, some methods may not carry over metadata, useful in that case.
-    get_data : Return data as collection of numpy arrays with kpoints already sent to BZ. Use .to_json() to export to json for plotting in other libraries/languages like Mathematica.
+    send_metadata : Copy metadata from this to another EvalsDataFrame, some methods may not carry over metadata, useful in that case.
 
-    All other methods are inherited from pd.DataFrame. If you apply some method that do not pass metadat, then use `send_metadata` to copy metadata to traget SpinDataFrame.
+    All other methods are inherited from pd.DataFrame. If you apply some method that do not pass metadat, then use `send_metadata` to copy metadata to traget EvalsDataFrame.
     """
 
-    _metadata = [
-        "_current_attrs",
-        "sys_info",
-        "poscar",
-        "projection",
-    ]  # These are passed after operations to new dataframe.
-
-    def __init__(
-        self,
-        *args,
-        path=None,
-        bands=[0],
-        projections={"A": ([0], [0])},
-        elim=None,
-        skipk=None,
-        data=None,
-        **kwargs,
-    ):
-        raise NotImplementedError("This class is not ready yet.")
-        if not (
-            path or args
-        ):  # It works fine without path given, but it is not recommended.
-            path = "./vasprun.xml"
-        if path or data:  # Don't updates args otherwise
-            for k in kwargs.keys():  # Do not let pass parameters to kwargs in this case
-                raise ValueError(f"SpinDataFrame got unexpected keyword argument {k!r}")
-
-            spin_data = None  # To avoid access before assignment
-            if data:
-                spin_data = serializer.SpinData.validated(data)
-            elif isinstance(path, str):
-                try:  # Check if 4 sets of data are there.
-                    spin_data = vp.export_spin_data(
-                        path, spins="sxyz", skipk=skipk, elim=elim
-                    )
-                except:  # If not 4 sets
-                    spin_data = vp.export_spin_data(
-                        path, spins="s", skipk=skipk, elim=elim
-                    )
-            else:
-                raise ValueError("Invalid path or data!")
-
-            if spin_data:
-                out_dict = _collect_spin_data(
-                    spin_data, bands=bands, atoms=atoms, orbs=orbs
-                )
-                super().__init__(out_dict)
-                self.sys_info = spin_data.sys_info
-                atoms, orbs, *_ = _format_input(projections, sys_info=self.sys_info)
-                self.projection = serializer.Dict2Data(
-                    {
-                        f"_{i}": {"ions": e, "orbs": o}
-                        for i, (e, o) in enumerate(zip(atoms, orbs))
-                    }
-                )
-                # Path below is used to get kpoints info
-                self.poscar = POSCAR(path=path, data=spin_data.poscar)
-                self._current_attrs = {
-                    "cmap": "viridis"
-                }  # To store attributes of current plot for use in colorbar.
+    current_attrs = {}
+    _metadata = ["current_attrs", "source", "ezero", "summary", "poscar"]
 
-        else:  # This part is only for operations on dataframe.
-            if (
-                len(args) == 1
-            ):  # This gives hack to load data from a file in current directory.
-                if (args[0] is None) or isinstance(
-                    args[0], str
-                ):  # If path is given as positional argument
-                    raise ValueError("SpinDataFrame expects no positional argument!")
-            super().__init__(*args, **kwargs)
+    def __init__(self, *source, spins=[0], bands=[0], atoms=None, orbs=None, **kwargs):
+        if len(source) == 1 and isinstance(source[0], DataSource):
+            df_dict, self.summary, self.poscar, self.ezero = _collect_data(
+                source[0], spins=spins, bands=bands, atoms=atoms, orbs=orbs
+            )
+            super().__init__(df_dict)
+            self.source = source[0]  # Need to be there for other types of operations
+        elif len(source) > 1:
+            for s in source:
+                if isinstance(s, DataSource):
+                    raise TypeError("source must be a single DataSource object!")
+            raise ValueError("source must be a single DataSource object!")
+        else:
+            super().__init__(*source, **kwargs)  # For other opertaions on dataframe
 
     @property
     def _constructor(self):
         "That's main hero of this class. This is called when you apply some method of slice it."
-        return SpinDataFrame
-
-    @property
-    def fermi(self):
-        "Fermi energy based on occupancy. Returns `self.Fermi` if occupancies cannot be resolved."
-        return self.sys_info.fermi
-
-    @property
-    def Fermi(self):
-        "Fermi energy given in vasprun.xml."
-        return self.sys_info.Fermi
-
-    def append(self, other):
-        "Append another SpinDataFrame to this one with same columns."
-        for k in other.columns:
-            if k not in self.columns:
-                raise ValueError(f"Column {k} in other is not not in this DataFrame!")
-        if len(self.columns) != len(other.columns):
-            raise ValueError("Columns are not same!")
-        out_df = super().append(other)
-        self.send_metadata(out_df)
-        return out_df
-
-    def join(self, other):
-        "Same as self.append"
-        return self.append(other)
-
-    def concat(self, other):
-        "Same as self.append"
-        return self.append(other)
-
-    def __add__(self, other):
-        "Same as self.append"
-        return self.append(other)
-
-    def get_data(self, shift=0):
-        """Access Data with transformed KPOINTS based on current Brillouin Zone.
-        shift is used to shift kpoints before any other operation.
-        If You need to have kpoints in primitive/regular BZ, first use .poscar.get_bz() that set that kind of BZ.
-        """
-        bands = np.unique(self["band"].to_numpy()).astype(int)
-        out_dict = {"SYSTEM": self.sys_info.SYSTEM}
-        out_dict["atoms"] = self.poscar.data.types
-        out_dict["orbitals"] = self.sys_info.fields
-        out_dict["projection"] = self.projection
-        out_dict["bz"] = self.poscar.bz.to_dict()
-        out_dict["bz"]["specials"] = self.poscar.bz.specials.to_dict()
-        out_dict["bz"][
-            "normals"
-        ] = self.poscar.bz.normals._asdict()  # Named tuple to dict
-
-        for band in bands:
-            name = f"band_{band}"
-            df = self[self["band"] == band].sort_values(by=["kx", "ky", "kz"])
-            kx, ky, kz = df.poscar.bring_in_bz(
-                df[["kx", "ky", "kz"]].to_numpy(), sys_info=df.sys_info, shift=shift
-            ).T
-            out_dict[name] = {"kx": kx, "ky": ky, "kz": kz}
-
-            for k in df.columns:
-                if k not in ("band", *out_dict[name].keys()):
-                    out_dict[name][k] = df[k].to_numpy()
-
-        return serializer.Dict2Data(out_dict)
+        return EvalsDataFrame
 
     def masked(self, column, value, tol=1e-2, n=None, band=None, method="linear"):
         """Mask dataframe with a given value, using a tolerance.
         If n is given, (band should also be given to avoid multivalued interpolation error) data values are interpolated to grid of size (l,m,n) where n is longest side.
         n could be arbirarily large as mask will filter out data outside the tolerance.
         """
         if n and not isinstance(n, (int, np.integer)):
@@ -329,15 +201,15 @@
         # Sort based on distance, so arrows are drawn in correct order
         out_df = df[
             np.logical_and((df[column] < (value + tol)), (df[column] > (value - tol)))
         ]
         return out_df.sort_values(by=["kx", "ky", "kz"])
 
     def send_metadata(self, target_spin_dataframe):
-        "Copy metadata from this to another SpinDataFrame."
+        "Copy metadata from this to another EvalsDataFrame."
         for k in self._metadata:
             setattr(target_spin_dataframe, k, getattr(self, k))
 
     def sliced(self, column="kz", value=0):
         "Slice data in a plane orthogonal to given `column` at given `value`"
         return self[self[column] == value]
 
@@ -353,26 +225,28 @@
         return np.array(arrows_data).T
 
     def _collect_kxyz(self, *xyz, shift=0):
         "Return tuple(kxyz, k_order)"
         _kxyz = ["kx", "ky", "kz"]
         kij = [_kxyz.index(a) for a in xyz if a in _kxyz]
         kxyz = self[["kx", "ky", "kz"]].to_numpy()
-        kxyz = self.poscar.bring_in_bz(kxyz, sys_info=self.sys_info, shift=shift)
+        kxyz = self.poscar.bz.translate_inside(kxyz, shift=shift)
 
         # Handle third axis as energy as well
         if len(xyz) == 3 and xyz[2].startswith("e"):
             kxyz[:, 2] = self[xyz[2]].to_numpy()
             kij = [*kij, 2]  # Add energy to kij, it must be of size 2 before
 
         return kxyz, kij
 
     def _validate_columns(self, *args):
         for arg in args:
-            if arg not in self.columns:
+            if (
+                isinstance(arg, str) and arg not in self.columns
+            ):  # Allow other data as well
                 raise ValueError(f"{arg!r} is not a column in the dataframe")
 
     def splot(
         self,
         *args,
         arrows=[],
         every=1,
@@ -412,15 +286,15 @@
                 "splot takes 3 or 4 positional arguments [X,Y,E,[Anything]], last one is colormapped if kwargs don't have color."
             )
 
         self._validate_columns(*args)
         kxyz, kij = self._collect_kxyz(*args[:2], shift=shift)
         ax = ax or ptk.get_axes()
         minmax_c = [0, 1]
-        cmap = kwargs.get("cmap", self._current_attrs["cmap"])
+        cmap = kwargs.get("cmap", self.current_attrs["cmap"])
 
         if arrows:
             arrows_data = self._collect_arrows_data(arrows)
             cmap = quiver_kws.get("cmap", cmap)
             if "color" in quiver_kws:
                 cmap = None  # No colorbar for color only
                 arrows_data = arrows_data[:, :2]  # color takes precedence
@@ -439,15 +313,15 @@
                 del kwargs["color"]  # keep one
                 cmap = None  # No colorbar
 
             kwargs["c"] = kwargs.get("c", _C)
             ax.scatter(*kxyz.T[kij], **kwargs)
             minmax_c = [min(_C), max(_C)]
 
-        self._current_attrs = {"ax": ax, "minmax_c": minmax_c, "cmap": cmap}
+        self.__class__.current_attrs = {"ax": ax, "minmax_c": minmax_c, "cmap": cmap}
         return ax
 
     def splot3d(
         self,
         *args,
         arrows=[],
         every=1,
@@ -490,15 +364,15 @@
         if not args[2][0] in "ek":
             raise ValueError("Z axis must be in [kx,ky,kz, energy]!")
 
         self._validate_columns(*args)
         kxyz, kij = self._collect_kxyz(*args[:3], shift=shift)
         ax = ax or ptk.get_axes(axes_3d=True)
         minmax_c = [0, 1]
-        cmap = kwargs.get("cmap", self._current_attrs["cmap"])
+        cmap = kwargs.get("cmap", self.current_attrs["cmap"])
 
         if arrows:
             arrows_data = self._collect_arrows_data(arrows)
             cmap = quiver_kws.get("cmap", cmap)
             if "color" in quiver_kws:  # color takes precedence
                 quiver_kws["C"] = quiver_kws["color"]
                 quiver_kws.pop("color")  # It is not in FancyArrowPatch
@@ -532,35 +406,54 @@
                 del kwargs["color"]  # keep one
                 cmap = None  # No colorbar
 
             kwargs["c"] = kwargs.get("c", _C)
             ax.scatter(*kxyz.T[kij], **kwargs)
             minmax_c = [min(_C), max(_C)]
 
-        self._current_attrs = {"ax": ax, "minmax_c": minmax_c, "cmap": cmap}
+        self.__class__.current_attrs = {"ax": ax, "minmax_c": minmax_c, "cmap": cmap}
         return ax
 
     def colorbar(self, cax=None, nticks=6, digits=2, **kwargs):
         "Add colobar to most recent plot. kwargs are passed to ipyvasp.splots.add_colorbar"
-        if not self._current_attrs["ax"]:
+        if not self.current_attrs["ax"]:
             raise ValueError(
                 "No plot has been made yet by using `splot, splot3d` or already consumed by `colorbar`"
             )
-        if not self._current_attrs["cmap"]:
+        if not self.current_attrs["cmap"]:
             raise ValueError("No Mappable for colorbar found!")
 
-        ax = self._current_attrs["ax"]
-        cmap = self._current_attrs["cmap"]
-        minmax_c = self._current_attrs["minmax_c"]
-        self._current_attrs["ax"] = None  # Reset
-        self._current_attrs["cmap"] = None  # Reset
+        ax = self.current_attrs["ax"]
+        cmap = self.current_attrs["cmap"]
+        minmax_c = self.current_attrs["minmax_c"]
+        self.current_attrs["ax"] = None  # Reset
+        self.current_attrs["cmap"] = None  # Reset
         if ax.name == "3d":
             cax = cax or plt.gcf().add_axes([0.85, 0.15, 0.03, 0.7])
 
         return ptk.add_colorbar(
             ax,
             cmap,
             cax=cax,
             ticks=np.linspace(*minmax_c, nticks, endpoint=True),
             digits=digits,
             **kwargs,
         )
+
+    @property
+    def kpoints(self):
+        "Returns kpoints as numpy array"
+        return self["kx ky kz".split()].to_numpy()
+
+    @property
+    def coords(self):
+        "Returns cartesian coodinates of kpoints as numpy array"
+        return self["x y z".split()].to_numpy()
+
+
+# from ipywidgets import interact
+# import matplotlib.pyplot as plt
+# import numpy as np
+
+# @interact(x = df.columns, y = df.columns, color=df.columns, band = [str(i) for i in np.unique(df.band.to_numpy())])
+# def plot(x,y,color, band):
+#     df[df.band == int(band)].plot(x,y, c=color, kind='scatter',cmap='turbo',s=200, marker='s', figsize=(3,2.6))
```

### Comparing `ipyvasp-0.3.0/ipyvasp/utils.py` & `ipyvasp-0.4.0/ipyvasp/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,20 @@
         return func
 
     return wrapper
 
 
 @contextmanager
 def set_dir(path: str):
-    "Context manager to work in some directory and come back"
+    """Context manager to work in some directory and come back.
+    
+    >>> with set_dir('some_folder'):
+    >>>    do_something()
+    >>> # Now you are back in starting directory
+    """
     current = os.getcwd()  # not available in pathlib yet
     try:
         os.chdir(path)
         yield
     finally:
         os.chdir(current)
```

### Comparing `ipyvasp-0.3.0/ipyvasp/widgets.py` & `ipyvasp-0.4.0/ipyvasp/widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,31 +279,31 @@
         new_fw = self.__class__(
             path=self._widgets["input"].value,
             glob=self._widgets["glob"].value,
             exclude=self._widgets["exclude"].value,
         )
         info = ipw.HTML().add_class("FW-Progess")
 
-        def interact_func(filename, **kwargs):
-            if filename:  # This would be None if no file is selected
+        def interact_func(fname, **kwargs):
+            if fname:  # This would be None if no file is selected
                 info.value = _progress_svg
                 try:
                     start = time()
                     print(
-                        f"Running {func.__name__}({filename!r}, {kwargs})"
+                        f"Running {func.__name__}({fname!r}, {kwargs})"
                     )  # it also serves as removing the output errors
                     func(
-                        Path(filename).absolute(), **kwargs
+                        Path(fname).absolute(), **kwargs
                     )  # Have Path object absolue if user changes directory
                     print(f"Finished in {time() - start:.3f} seconds.")
                 finally:
                     info.value = ""
 
         out = ipw.interactive(
-            interact_func, options, filename=new_fw._widgets["files"], **kwargs
+            interact_func, options, fname=new_fw._widgets["files"], **kwargs
         )
 
         out.files_widget = new_fw  # save reference to FilesWidget
         out.output_widget = out.children[
             -1
         ]  # save reference to output widget for other widgets to use
 
@@ -794,15 +794,15 @@
                         for key, value in data_dict.items()
                         if key not in ("so_max", "so_min")
                     )
                 )
 
             serializer.dump(
                 data_dict,
-                dump_to="json",
+                format="json",
                 outfile=self.files_widget.selected.parent / "result.json",
             )
 
         if (
             change is None
         ):  # called from other functions but not from store_clicked_data
             return _show_and_save(self._result)
```

