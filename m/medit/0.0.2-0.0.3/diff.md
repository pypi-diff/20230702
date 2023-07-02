# Comparing `tmp/medit-0.0.2.tar.gz` & `tmp/medit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medit-0.0.2.tar", max compression
+gzip compressed data, was "medit-0.0.3.tar", max compression
```

## Comparing `medit-0.0.2.tar` & `medit-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,19 @@
--rw-r--r--   0        0        0     1837 2023-07-02 11:33:38.540816 medit-0.0.2/Readme.md
--rw-r--r--   0        0        0        0 2023-06-18 13:03:52.329049 medit-0.0.2/medit/__init__.py
--rwxr-xr-x   0        0        0     2392 2023-07-02 11:33:38.540816 medit-0.0.2/medit/cli.py
--rw-r--r--   0        0        0     4619 2023-07-02 15:32:07.351200 medit-0.0.2/medit/meditor.py
--rw-r--r--   0        0        0     7055 2023-07-02 14:04:10.012757 medit-0.0.2/medit/mview.py
--rwxr-xr-x   0        0        0     6984 2023-07-02 15:29:24.360828 medit-0.0.2/medit/ui.py
--rw-r--r--   0        0        0     2389 2023-07-02 11:32:00.577590 medit-0.0.2/medit/utils.py
--rw-r--r--   0        0        0     2232 2023-07-02 15:34:15.036636 medit-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2736 1970-01-01 00:00:00.000000 medit-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1837 2023-07-02 11:33:38.540816 medit-0.0.3/Readme.md
+-rw-r--r--   0        0        0        0 2023-06-18 13:03:52.329049 medit-0.0.3/medit/__init__.py
+-rwxr-xr-x   0        0        0     2392 2023-07-02 11:33:38.540816 medit-0.0.3/medit/cli.py
+-rw-r--r--   0        0        0     1862 2023-07-02 11:32:00.577590 medit-0.0.3/medit/medit.ui
+-rw-r--r--   0        0        0     4732 2023-07-02 15:46:12.488227 medit-0.0.3/medit/meditor.py
+-rw-r--r--   0        0        0     7055 2023-07-02 14:04:10.012757 medit-0.0.3/medit/mview.py
+-rw-r--r--   0        0        0        0 2023-07-02 15:40:29.959990 medit-0.0.3/medit/styles/__init__.py
+-rw-r--r--   0        0        0    18966 2023-07-02 11:33:38.541816 medit-0.0.3/medit/styles/external/github-markdown-dark.css
+-rw-r--r--   0        0        0    18979 2023-07-02 11:33:38.541816 medit-0.0.3/medit/styles/external/github-markdown-light.css
+-rw-r--r--   0        0        0     5061 2023-07-02 11:33:38.541816 medit-0.0.3/medit/styles/external/pygments-solarized-style/solarized-dark.css
+-rw-r--r--   0        0        0     5061 2023-07-02 11:33:38.541816 medit-0.0.3/medit/styles/external/pygments-solarized-style/solarized-light.css
+-rw-r--r--   0        0        0    36899 2023-07-02 11:33:38.541816 medit-0.0.3/medit/styles/external/solarized-dark-all-sites.css
+-rw-r--r--   0        0        0    36890 2023-07-02 11:33:38.542816 medit-0.0.3/medit/styles/external/solarized-light-all-sites.css
+-rw-r--r--   0        0        0     4282 2023-07-02 11:33:38.542816 medit-0.0.3/medit/styles/external/thomasf-solarized-css/solarized-dark.css
+-rw-r--r--   0        0        0     4282 2023-07-02 11:33:38.542816 medit-0.0.3/medit/styles/external/thomasf-solarized-css/solarized-light.css
+-rwxr-xr-x   0        0        0     6985 2023-07-02 15:43:07.140557 medit-0.0.3/medit/ui.py
+-rw-r--r--   0        0        0     2389 2023-07-02 11:32:00.577590 medit-0.0.3/medit/utils.py
+-rw-r--r--   0        0        0     2294 2023-07-02 15:46:49.941362 medit-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2736 1970-01-01 00:00:00.000000 medit-0.0.3/PKG-INFO
```

### Comparing `medit-0.0.2/Readme.md` & `medit-0.0.3/Readme.md`

 * *Files identical despite different names*

### Comparing `medit-0.0.2/medit/cli.py` & `medit-0.0.3/medit/cli.py`

 * *Files identical despite different names*

### Comparing `medit-0.0.2/medit/meditor.py` & `medit-0.0.3/medit/meditor.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         # self.markerDefine(QsciScintilla.RightArrow, self.ARROW_MARKER_NUM)
         # self.setMarkerBackgroundColor(QColor("#ee1111"), self.ARROW_MARKER_NUM)
 
         self.setBraceMatching(self.BraceMatch.SloppyBraceMatch)
 
         # Current line visible with special background color
         self.setCaretLineVisible(True)
-        #self.setCaretLineBackgroundColor(QtGui.QColor("#ffe4e4"))
+        self.setCaretLineBackgroundColor(QtGui.QColor("#eee8d5"))
 
         self.SendScintilla(Qsci.QsciScintilla.SCI_STYLESETFONT, 1, "Courier".encode())
 
         # Don't want to see the horizontal scrollbar at all
         # Use raw message to Scintilla here (all messages are documented
         # here: http://www.scintilla.org/ScintillaDoc.html)
         self.SendScintilla(Qsci.QsciScintilla.SCI_SETHSCROLLBAR, 0)
@@ -79,16 +79,19 @@
             Qsci.QsciLexerBash() if suffix in {".sh"} else
             Qsci.QsciLexerPython() if suffix in {".py"} else
             Qsci.QsciLexerXML() if suffix in {".xml", ".svg"} else
             None
         )
         if lexer:
             lexer.setFont(self.font())
-            lexer.setPaper(QtGui.QColor("#073642"))
-            lexer.setDefaultPaper(QtGui.QColor("#073642"))
+            #lexer.setPaper(QtGui.QColor("#073642"))
+            #lexer.setDefaultPaper(QtGui.QColor("#073642"))
+            lexer.setPaper(QtGui.QColor("#fdf6e3"))
+            lexer.setDefaultPaper(QtGui.QColor("#fdf6e3"))
+
         self.setLexer(lexer)
 
         with open(path) as textFile:
             self.setText(textFile.read())
 
 
     def view_state(self):
```

### Comparing `medit-0.0.2/medit/mview.py` & `medit-0.0.3/medit/mview.py`

 * *Files identical despite different names*

### Comparing `medit-0.0.2/medit/ui.py` & `medit-0.0.3/medit/ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 
     import qdarktheme
 
 
     logging.getLogger().setLevel(logging.INFO)
     app = QtWidgets.QApplication(sys.argv)
 
-    qdarktheme.setup_theme("dark")
+    qdarktheme.setup_theme("light")
 
     window = MEditWindow(path)
 
     for s in (signal.SIGABRT, signal.SIGINT, signal.SIGSEGV, signal.SIGTERM):
         signal.signal(s, lambda signal, frame: window.close())
 
     # catch the interpreter every now and then to be able to catch signals
```

### Comparing `medit-0.0.2/medit/utils.py` & `medit-0.0.3/medit/utils.py`

 * *Files identical despite different names*

### Comparing `medit-0.0.2/pyproject.toml` & `medit-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 [tool.poetry]
 name = "medit"
-version = "0.0.2"
+version = "0.0.3"
 description = "Markup Editor"
 authors = ["Frans Fürst <frans.fuerst+gitlab@protonmail.com>"]
 repository = "https://projects.om-office.de/frans/medit.git"
 readme = "Readme.md"
 packages = [
-  {include = "medit/**/*.py"}
+  {include = "medit/**/*.py"},
+  {include = "medit/**/*.ui"},
+  {include = "medit/styles"},
 ]
 
 [tool.poetry.scripts]
 medit = 'medit.cli:main'
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
```

### Comparing `medit-0.0.2/PKG-INFO` & `medit-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medit
-Version: 0.0.2
+Version: 0.0.3
 Summary: Markup Editor
 Home-page: https://projects.om-office.de/frans/medit.git
 Author: Frans Fürst
 Author-email: frans.fuerst+gitlab@protonmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

